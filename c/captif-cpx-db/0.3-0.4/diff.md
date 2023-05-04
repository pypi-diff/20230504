# Comparing `tmp/captif_cpx_db-0.3.tar.gz` & `tmp/captif_cpx_db-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "captif_cpx_db-0.3.tar", max compression
+gzip compressed data, was "captif_cpx_db-0.4.tar", max compression
```

## Comparing `captif_cpx_db-0.3.tar` & `captif_cpx_db-0.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1084 2023-04-26 22:21:52.906596 captif_cpx_db-0.3/LICENSE
--rw-r--r--   0        0        0       16 2023-04-26 22:21:52.906596 captif_cpx_db-0.3/README.md
--rw-r--r--   0        0        0      257 2023-04-26 22:21:52.906596 captif_cpx_db-0.3/captif_cpx_db/__init__.py
--rw-r--r--   0        0        0       30 2023-04-26 22:21:52.906596 captif_cpx_db-0.3/captif_cpx_db/constants.py
--rw-r--r--   0        0        0     2060 2023-04-26 22:21:52.906596 captif_cpx_db-0.3/captif_cpx_db/models/__init__.py
--rw-r--r--   0        0        0      244 2023-04-26 22:21:52.906596 captif_cpx_db-0.3/captif_cpx_db/models/sa_helpers.py
--rw-r--r--   0        0        0    10574 2023-04-26 22:21:52.906596 captif_cpx_db-0.3/captif_cpx_db/models/segment.py
--rw-r--r--   0        0        0     7648 2023-04-26 22:21:52.906596 captif_cpx_db-0.3/captif_cpx_db/models/session.py
--rw-r--r--   0        0        0      504 2023-04-26 22:21:52.906596 captif_cpx_db-0.3/pyproject.toml
--rw-r--r--   0        0        0      494 1970-01-01 00:00:00.000000 captif_cpx_db-0.3/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-05-04 02:08:23.865137 captif_cpx_db-0.4/LICENSE
+-rw-r--r--   0        0        0       16 2023-05-04 02:08:23.865137 captif_cpx_db-0.4/README.md
+-rw-r--r--   0        0        0      257 2023-05-04 02:08:23.865137 captif_cpx_db-0.4/captif_cpx_db/__init__.py
+-rw-r--r--   0        0        0       30 2023-05-04 02:08:23.865137 captif_cpx_db-0.4/captif_cpx_db/constants.py
+-rw-r--r--   0        0        0     3284 2023-05-04 02:08:23.865137 captif_cpx_db-0.4/captif_cpx_db/models/__init__.py
+-rw-r--r--   0        0        0      244 2023-05-04 02:08:23.865137 captif_cpx_db-0.4/captif_cpx_db/models/sa_helpers.py
+-rw-r--r--   0        0        0    11287 2023-05-04 02:08:23.865137 captif_cpx_db-0.4/captif_cpx_db/models/segment.py
+-rw-r--r--   0        0        0     7437 2023-05-04 02:08:23.865137 captif_cpx_db-0.4/captif_cpx_db/models/session.py
+-rw-r--r--   0        0        0      504 2023-05-04 02:08:23.865137 captif_cpx_db-0.4/pyproject.toml
+-rw-r--r--   0        0        0      494 1970-01-01 00:00:00.000000 captif_cpx_db-0.4/PKG-INFO
```

### Comparing `captif_cpx_db-0.3/LICENSE` & `captif_cpx_db-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `captif_cpx_db-0.3/captif_cpx_db/models/__init__.py` & `captif_cpx_db-0.4/captif_cpx_db/models/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from datetime import date
+from pydantic import condecimal
 from sqlmodel import Field, SQLModel, Relationship
 from typing import TYPE_CHECKING, List, Optional
 
 from . import session, segment  # noqa: F401
 
 if TYPE_CHECKING:  # pragma: no cover
     from .session import SessionDetails
@@ -51,14 +52,48 @@
     segment_length_m: Optional[float] = Field(
         default=None,
         description=(
             "length of the road segment in metres. Set to None if results use "
             "a variable segment length."
         ),
     )
+    reference_speed_kph: int = Field(
+        nullable=False,
+        description="reference speed in km/h",
+    )
+    speed_correction_coefficient: condecimal(max_digits=5, decimal_places=3) = Field(
+        nullable=False,
+        description="speed constant used to calculate speed correction",
+    )
+    reference_temperature: float = Field(
+        nullable=False,
+        description="reference temperature in degrees C",
+    )
+    temperature_correction_type: str = Field(
+        nullable=False,
+        description="temperature correction basis ('air', 'tyre' or 'road')",
+    )
+    temperature_correction_coefficient: condecimal(
+        max_digits=5,
+        decimal_places=4,
+    ) = Field(
+        nullable=False,
+        description="temperature correction coefficient",
+    )
+    gps_acceleration_threshold_kph_sec: float = Field(
+        description=(
+            "threshold for determining if the GPS acceleration is valid in " "km/h/sec"
+        ),
+    )
+    rsrp_database: str = Field(
+        description="name of the RSRP database used to generate the results set",
+    )
+    rsrp_date: date = Field(
+        description="date that the RSRP database was accessed",
+    )
     notes: Optional[str] = Field(
         default=None,
         description="reason for the results set being generated",
     )
     include_in_map_service: bool = Field(
         default=True,
         description=("whether or not to include the results set in the map service"),
```

### Comparing `captif_cpx_db-0.3/captif_cpx_db/models/segment.py` & `captif_cpx_db-0.4/captif_cpx_db/models/segment.py`

 * *Files 8% similar despite different names*

```diff
@@ -43,14 +43,25 @@
             "run number as per the measurement files. This cannot be relied "
             "on when determining the number of runs across a given road "
             "segment. Instead, count the number of unique "
             "road_id/start_m/end_m/lane_number combinations assocated with "
             "the results set."
         ),
     )
+    run_segment_count: int = Field(
+        nullable=False,
+        description=(
+            "the run segment counter as per the measurement files. This "
+            "is used to indicate a pause in a run. This cannot be relied "
+            "on when determining the number of runs across a given road "
+            "segment. Instead, count the number of unique "
+            "road_id/start_m/end_m/lane_number combinations assocated with "
+            "the results set."
+        ),
+    )
     road_id: int = Field(
         nullable=False,
         description="RAMM road ID",
     )
     start_m: float = Field(
         nullable=False,
         description=(
@@ -85,40 +96,45 @@
         nullable=False,
         description="average speed across the road segment in km/h",
     )
     air_temperature: float = Field(
         nullable=False,
         description=("average air temperature across the road segment in degrees C"),
     )
-    reference_speed_kph: int = Field(
+    speed_correction_db: float = Field(
         nullable=False,
-        description="reference speed in km/h",
+        description="speed correction in dB",
     )
-    speed_constant: condecimal(max_digits=5, decimal_places=3) = Field(
+    temperature_correction_db: float = Field(
         nullable=False,
-        description="speed constant used to calculate speed correction",
+        description="temperature correction in dB",
     )
-    speed_correction_db: float = Field(
+    start_latitude: float = Field(
         nullable=False,
-        description="speed correction in dB",
+        description="latitude of segment start point",
     )
-    temperature_correction_coefficient: condecimal(
-        max_digits=5,
-        decimal_places=4,
-    ) = Field(
+    start_longitude: float = Field(
         nullable=False,
-        description="temperature correction coefficient",
+        description="longitude of segment start point",
     )
-    temperature_correction_db: float = Field(
+    end_latitude: float = Field(
         nullable=False,
-        description="temperature correction in dB",
+        description="latitude of segment end point",
     )
-    event_flag: Optional[str] = Field(
-        default=None,
-        description="event flag (e.g. 'passing vehicle')",
+    end_longitude: float = Field(
+        nullable=False,
+        description="longitude of segment end point",
+    )
+    passing_truck_flag: Optional[bool] = Field(
+        default=False,
+        description="passing truck",
+    )
+    other_flag: Optional[bool] = Field(
+        default=False,
+        description="other flag",
     )
     valid: bool = Field(
         nullable=False,
         description=(
             "indicated whether the road segment results are valid or not, "
             "based on the speed and any event flags"
         ),
@@ -233,14 +249,18 @@
         primary_key=True,
         description="wheel bay name ('left' or 'right')",
     )
     microphone_position: int = Field(
         primary_key=True,
         description="microphone position (1-6) as per ISO 11819-2:2017",
     )
+    laeq_db: float = Field(
+        nullable=False,
+        description="LAeq for the microphone position in dB (no CPX corrections applied)",
+    )
     microphone_third_octave_levels: List["MicrophoneThirdOctaveLevels"] = Relationship()
 
 
 class MicrophoneThirdOctaveLevels(SQLModel, table=True):
     """
     One-third octave band sound pressure levels for each microphone position
     in the wheel bay, measured across one road segment.
```

### Comparing `captif_cpx_db-0.3/captif_cpx_db/models/session.py` & `captif_cpx_db-0.4/captif_cpx_db/models/session.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,22 +28,14 @@
     __tablename__ = "session_details"
 
     results_set_id: int = Field(
         default=None,
         foreign_key="results_set.id",
         primary_key=True,
     )
-    reference_temperature: condecimal(max_digits=5, decimal_places=3) = Field(
-        nullable=False,
-        description="reference temperature in degrees C",
-    )
-    temperature_correction_type: str = Field(
-        nullable=False,
-        description="temperature correction basis ('air', 'tyre' or 'road')",
-    )
     wheel_bay_details: List["SessionWheelBayDetails"] = Relationship()
 
 
 class SessionWheelBayDetails(SQLModel, table=True):
     """
     Session-level wheel bay details for a given results set. Each results set
     can have up to two wheel bay entries.
@@ -199,14 +191,18 @@
         primary_key=True,
         description="wheel bay name ('left' or 'right')",
     )
     tyre: str = Field(
         nullable=False,
         description="tyre name/type (e.g. 'P1', 'H1', etc.)",
     )
+    tyre_purchase_date: date = Field(
+        nullable=False,
+        description="tyre purchase date",
+    )
     reference_hardness: int = Field(
         nullable=False,
         description="reference tyre hardness in Shore A",
     )
     hardness: condecimal(max_digits=3, decimal_places=1) = Field(
         nullable=False,
         description="tyre hardness in Shore A",
```

