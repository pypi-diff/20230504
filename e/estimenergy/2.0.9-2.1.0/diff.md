# Comparing `tmp/estimenergy-2.0.9.tar.gz` & `tmp/estimenergy-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "estimenergy-2.0.9.tar", max compression
+gzip compressed data, was "estimenergy-2.1.0.tar", max compression
```

## Comparing `estimenergy-2.0.9.tar` & `estimenergy-2.1.0.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0     1089 2023-04-29 01:13:38.355201 estimenergy-2.0.9/LICENSE
--rw-r--r--   0        0        0     4481 2023-04-29 01:13:38.355201 estimenergy-2.0.9/README.md
--rw-r--r--   0        0        0        0 2023-04-29 01:13:38.359201 estimenergy-2.0.9/estimenergy/__init__.py
--rw-r--r--   0        0        0       38 2023-04-29 01:13:38.359201 estimenergy-2.0.9/estimenergy/client/__init__.py
--rw-r--r--   0        0        0      639 2023-04-29 01:13:38.359201 estimenergy-2.0.9/estimenergy/client/client.py
--rw-r--r--   0        0        0      451 2023-04-29 01:13:38.359201 estimenergy-2.0.9/estimenergy/config.py
--rw-r--r--   0        0        0     6030 2023-04-29 01:13:38.359201 estimenergy-2.0.9/estimenergy/const.py
--rw-r--r--   0        0        0      665 2023-04-29 01:13:38.359201 estimenergy-2.0.9/estimenergy/db.py
--rw-r--r--   0        0        0      133 2023-04-29 01:13:38.359201 estimenergy-2.0.9/estimenergy/devices/__init__.py
--rw-r--r--   0        0        0     3140 2023-04-29 01:13:38.359201 estimenergy-2.0.9/estimenergy/devices/base_device.py
--rw-r--r--   0        0        0       99 2023-04-29 01:13:38.359201 estimenergy-2.0.9/estimenergy/devices/device_error.py
--rw-r--r--   0        0        0     4048 2023-04-29 01:13:38.359201 estimenergy-2.0.9/estimenergy/devices/device_registry.py
--rw-r--r--   0        0        0     6226 2023-04-29 01:13:38.359201 estimenergy-2.0.9/estimenergy/devices/glow_device.py
--rw-r--r--   0        0        0      540 2023-04-29 01:13:38.359201 estimenergy-2.0.9/estimenergy/helpers.py
--rw-r--r--   0        0        0      318 2023-04-29 01:13:38.359201 estimenergy-2.0.9/estimenergy/influx.py
--rw-r--r--   0        0        0      613 2023-04-29 01:13:38.359201 estimenergy-2.0.9/estimenergy/log.py
--rw-r--r--   0        0        0     2088 2023-04-29 01:13:38.359201 estimenergy-2.0.9/estimenergy/main.py
--rw-r--r--   0        0        0       94 2023-04-29 01:13:38.359201 estimenergy-2.0.9/estimenergy/models/__init__.py
--rw-r--r--   0        0        0        0 2023-04-29 01:13:38.359201 estimenergy-2.0.9/estimenergy/models/config/__init__.py
--rw-r--r--   0        0        0     1500 2023-04-29 01:13:38.359201 estimenergy-2.0.9/estimenergy/models/config/config.py
--rw-r--r--   0        0        0       86 2023-04-29 01:13:38.359201 estimenergy-2.0.9/estimenergy/models/config/dev_config.py
--rw-r--r--   0        0        0      138 2023-04-29 01:13:38.359201 estimenergy-2.0.9/estimenergy/models/config/influx_config.py
--rw-r--r--   0        0        0      208 2023-04-29 01:13:38.359201 estimenergy-2.0.9/estimenergy/models/config/logging_config.py
--rw-r--r--   0        0        0      279 2023-04-29 01:13:38.359201 estimenergy-2.0.9/estimenergy/models/config/networking_config.py
--rw-r--r--   0        0        0      186 2023-04-29 01:13:38.359201 estimenergy-2.0.9/estimenergy/models/config/sql_config.py
--rw-r--r--   0        0        0      896 2023-04-29 01:13:38.359201 estimenergy-2.0.9/estimenergy/models/day.py
--rw-r--r--   0        0        0      912 2023-04-29 01:13:38.359201 estimenergy-2.0.9/estimenergy/models/device_config.py
--rw-r--r--   0        0        0       76 2023-04-29 01:13:38.359201 estimenergy-2.0.9/estimenergy/models/message.py
--rw-r--r--   0        0        0      874 2023-04-29 01:13:38.359201 estimenergy-2.0.9/estimenergy/models/month.py
--rw-r--r--   0        0        0      335 2023-04-29 01:13:38.359201 estimenergy-2.0.9/estimenergy/models/total.py
--rw-r--r--   0        0        0      799 2023-04-29 01:13:38.359201 estimenergy-2.0.9/estimenergy/models/year.py
--rw-r--r--   0        0        0      479 2023-04-29 01:13:38.359201 estimenergy-2.0.9/estimenergy/prometheus.py
--rw-r--r--   0        0        0        0 2023-04-29 01:13:38.359201 estimenergy-2.0.9/estimenergy/routers/__init__.py
--rw-r--r--   0        0        0     4261 2023-04-29 01:13:38.363201 estimenergy-2.0.9/estimenergy/routers/day_router.py
--rw-r--r--   0        0        0     4293 2023-04-29 01:13:38.363201 estimenergy-2.0.9/estimenergy/routers/device_router.py
--rw-r--r--   0        0        0     1466 2023-04-29 01:13:38.363201 estimenergy-2.0.9/estimenergy/routers/month_router.py
--rw-r--r--   0        0        0     1466 2023-04-29 01:13:38.363201 estimenergy-2.0.9/estimenergy/routers/total_router.py
--rw-r--r--   0        0        0     1436 2023-04-29 01:13:38.363201 estimenergy-2.0.9/estimenergy/routers/year_router.py
--rw-r--r--   0        0        0        0 2023-04-29 01:13:38.363201 estimenergy-2.0.9/estimenergy/services/__init__.py
--rw-r--r--   0        0        0     2663 2023-04-29 01:13:38.363201 estimenergy-2.0.9/estimenergy/services/data_service.py
--rw-r--r--   0        0        0     3098 2023-04-29 01:13:38.363201 estimenergy-2.0.9/estimenergy/services/influx_service.py
--rw-r--r--   0        0        0     4486 2023-04-29 01:13:38.363201 estimenergy-2.0.9/estimenergy/services/prediction_service.py
--rw-r--r--   0        0        0     1725 2023-04-29 01:13:38.363201 estimenergy-2.0.9/estimenergy/services/prometheus_service.py
--rw-r--r--   0        0        0    15611 2023-04-29 01:13:38.363201 estimenergy-2.0.9/estimenergy/services/sql_service.py
--rw-r--r--   0        0        0     2495 2023-04-29 01:14:16.347264 estimenergy-2.0.9/pyproject.toml
--rw-r--r--   0        0        0     5876 1970-01-01 00:00:00.000000 estimenergy-2.0.9/PKG-INFO
+-rw-r--r--   0        0        0     1089 2023-05-04 07:49:15.010812 estimenergy-2.1.0/LICENSE
+-rw-r--r--   0        0        0     4481 2023-05-04 07:49:15.010812 estimenergy-2.1.0/README.md
+-rw-r--r--   0        0        0        0 2023-05-04 07:49:15.014813 estimenergy-2.1.0/estimenergy/__init__.py
+-rw-r--r--   0        0        0       38 2023-05-04 07:49:15.014813 estimenergy-2.1.0/estimenergy/client/__init__.py
+-rw-r--r--   0        0        0      639 2023-05-04 07:49:15.014813 estimenergy-2.1.0/estimenergy/client/client.py
+-rw-r--r--   0        0        0      451 2023-05-04 07:49:15.014813 estimenergy-2.1.0/estimenergy/config.py
+-rw-r--r--   0        0        0     6030 2023-05-04 07:49:15.014813 estimenergy-2.1.0/estimenergy/const.py
+-rw-r--r--   0        0        0      665 2023-05-04 07:49:15.014813 estimenergy-2.1.0/estimenergy/db.py
+-rw-r--r--   0        0        0      133 2023-05-04 07:49:15.014813 estimenergy-2.1.0/estimenergy/devices/__init__.py
+-rw-r--r--   0        0        0     2465 2023-05-04 07:49:15.014813 estimenergy-2.1.0/estimenergy/devices/base_device.py
+-rw-r--r--   0        0        0       99 2023-05-04 07:49:15.014813 estimenergy-2.1.0/estimenergy/devices/device_error.py
+-rw-r--r--   0        0        0     4048 2023-05-04 07:49:15.014813 estimenergy-2.1.0/estimenergy/devices/device_registry.py
+-rw-r--r--   0        0        0     8414 2023-05-04 07:49:15.014813 estimenergy-2.1.0/estimenergy/devices/glow_device.py
+-rw-r--r--   0        0        0      540 2023-05-04 07:49:15.018813 estimenergy-2.1.0/estimenergy/helpers.py
+-rw-r--r--   0        0        0      315 2023-05-04 07:49:15.018813 estimenergy-2.1.0/estimenergy/influx.py
+-rw-r--r--   0        0        0      613 2023-05-04 07:49:15.018813 estimenergy-2.1.0/estimenergy/log.py
+-rw-r--r--   0        0        0     2088 2023-05-04 07:49:15.018813 estimenergy-2.1.0/estimenergy/main.py
+-rw-r--r--   0        0        0       94 2023-05-04 07:49:15.018813 estimenergy-2.1.0/estimenergy/models/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-04 07:49:15.018813 estimenergy-2.1.0/estimenergy/models/config/__init__.py
+-rw-r--r--   0        0        0     1500 2023-05-04 07:49:15.018813 estimenergy-2.1.0/estimenergy/models/config/config.py
+-rw-r--r--   0        0        0       86 2023-05-04 07:49:15.018813 estimenergy-2.1.0/estimenergy/models/config/dev_config.py
+-rw-r--r--   0        0        0      132 2023-05-04 07:49:15.018813 estimenergy-2.1.0/estimenergy/models/config/influx_config.py
+-rw-r--r--   0        0        0      208 2023-05-04 07:49:15.018813 estimenergy-2.1.0/estimenergy/models/config/logging_config.py
+-rw-r--r--   0        0        0      279 2023-05-04 07:49:15.018813 estimenergy-2.1.0/estimenergy/models/config/networking_config.py
+-rw-r--r--   0        0        0      186 2023-05-04 07:49:15.018813 estimenergy-2.1.0/estimenergy/models/config/sql_config.py
+-rw-r--r--   0        0        0      896 2023-05-04 07:49:15.018813 estimenergy-2.1.0/estimenergy/models/day.py
+-rw-r--r--   0        0        0      912 2023-05-04 07:49:15.018813 estimenergy-2.1.0/estimenergy/models/device_config.py
+-rw-r--r--   0        0        0       76 2023-05-04 07:49:15.018813 estimenergy-2.1.0/estimenergy/models/message.py
+-rw-r--r--   0        0        0      874 2023-05-04 07:49:15.018813 estimenergy-2.1.0/estimenergy/models/month.py
+-rw-r--r--   0        0        0      371 2023-05-04 07:49:15.018813 estimenergy-2.1.0/estimenergy/models/total.py
+-rw-r--r--   0        0        0      799 2023-05-04 07:49:15.018813 estimenergy-2.1.0/estimenergy/models/year.py
+-rw-r--r--   0        0        0      479 2023-05-04 07:49:15.018813 estimenergy-2.1.0/estimenergy/prometheus.py
+-rw-r--r--   0        0        0        0 2023-05-04 07:49:15.018813 estimenergy-2.1.0/estimenergy/routers/__init__.py
+-rw-r--r--   0        0        0     4261 2023-05-04 07:49:15.018813 estimenergy-2.1.0/estimenergy/routers/day_router.py
+-rw-r--r--   0        0        0     4293 2023-05-04 07:49:15.018813 estimenergy-2.1.0/estimenergy/routers/device_router.py
+-rw-r--r--   0        0        0     1466 2023-05-04 07:49:15.018813 estimenergy-2.1.0/estimenergy/routers/month_router.py
+-rw-r--r--   0        0        0     1466 2023-05-04 07:49:15.018813 estimenergy-2.1.0/estimenergy/routers/total_router.py
+-rw-r--r--   0        0        0     1436 2023-05-04 07:49:15.018813 estimenergy-2.1.0/estimenergy/routers/year_router.py
+-rw-r--r--   0        0        0        0 2023-05-04 07:49:15.018813 estimenergy-2.1.0/estimenergy/services/__init__.py
+-rw-r--r--   0        0        0      835 2023-05-04 07:49:15.018813 estimenergy-2.1.0/estimenergy/services/data_service.py
+-rw-r--r--   0        0        0     1299 2023-05-04 07:49:15.018813 estimenergy-2.1.0/estimenergy/services/influx_service.py
+-rw-r--r--   0        0        0     4343 2023-05-04 07:49:15.018813 estimenergy-2.1.0/estimenergy/services/prediction_service.py
+-rw-r--r--   0        0        0     1546 2023-05-04 07:49:15.018813 estimenergy-2.1.0/estimenergy/services/prometheus_service.py
+-rw-r--r--   0        0        0    15063 2023-05-04 07:49:15.018813 estimenergy-2.1.0/estimenergy/services/sql_service.py
+-rw-r--r--   0        0        0     2494 2023-05-04 07:49:48.879550 estimenergy-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0     5868 1970-01-01 00:00:00.000000 estimenergy-2.1.0/PKG-INFO
```

### Comparing `estimenergy-2.0.9/LICENSE` & `estimenergy-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `estimenergy-2.0.9/README.md` & `estimenergy-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `estimenergy-2.0.9/estimenergy/client/client.py` & `estimenergy-2.1.0/estimenergy/client/client.py`

 * *Files identical despite different names*

### Comparing `estimenergy-2.0.9/estimenergy/const.py` & `estimenergy-2.1.0/estimenergy/const.py`

 * *Files identical despite different names*

### Comparing `estimenergy-2.0.9/estimenergy/db.py` & `estimenergy-2.1.0/estimenergy/db.py`

 * *Files identical despite different names*

### Comparing `estimenergy-2.0.9/estimenergy/devices/base_device.py` & `estimenergy-2.1.0/estimenergy/devices/base_device.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Abstract class for all devices."""
 from abc import ABC, abstractmethod
 import datetime
+from typing import Optional, Type
 
 from estimenergy.const import Metric
 from estimenergy.models.config.config import Config
-from estimenergy.models.device_config import DeviceConfig, DeviceConfigRead
+from estimenergy.models.device_config import DeviceConfig
 from estimenergy.services.data_service import DataService
 from estimenergy.services.influx_service import InfluxService
 from estimenergy.services.prometheus_service import PrometheusService
 from estimenergy.services.sql_service import SqlService
 
 
 class BaseDevice(ABC):
@@ -29,70 +30,56 @@
         prometheus_service = PrometheusService(sql_service, self.device_config, config)
         self.data_services.append(prometheus_service)
 
         if config.influx_config:
             influx_service = InfluxService(self.device_config, config)
             self.data_services.append(influx_service)
 
-    @property
     @abstractmethod
-    def provided_metrics(self) -> list[Metric]:
-        """Return a list of metrics provided by this device."""
+    async def start(self):
+        """Start the device."""
 
     @abstractmethod
     async def stop(self):
         """Stop the device."""
 
-    @abstractmethod
-    async def start(self):
-        """Start the device."""
-
-    async def increment(
-        self,
-        metric: Metric,
-        value: float,
-        value_dt: datetime.datetime = datetime.datetime.now(),
-    ):
-        """Increment a metric in the database."""
-
-        if metric not in self.provided_metrics:
-            raise ValueError(f"Metric {metric} not provided by this device.")
-
-        for data_service in self.data_services:
-            await data_service.increment(metric, value, value_dt)
-
-    async def decrement(
-        self,
-        metric: Metric,
-        value: float,
-        value_dt: datetime.datetime = datetime.datetime.now(),
-    ):
-        """Decrement a metric in the database."""
-
-        if metric not in self.provided_metrics:
-            raise ValueError(f"Metric {metric} not provided by this device.")
-
-        for data_service in self.data_services:
-            await data_service.decrement(metric, value, value_dt)
-
     async def write(
         self,
         metric: Metric,
         value: float,
-        value_dt: datetime.datetime = datetime.datetime.now(),
+        value_dt: datetime.datetime,
     ):
         """Write a metric to the database."""
 
-        if metric not in self.provided_metrics:
-            raise ValueError(f"Metric {metric} not provided by this device.")
-
         for data_service in self.data_services:
             await data_service.write(metric, value, value_dt)
 
+        await self.update(value_dt)
+
     async def update(
         self,
-        value_dt: datetime.datetime = datetime.datetime.now(),
+        value_dt: datetime.datetime,
     ):
         """Calculate metrics based on other metrics."""
 
         for data_service in self.data_services:
             await data_service.update(value_dt)
+
+    async def last(
+        self,
+        metric: Metric,
+        value_dt: datetime.datetime,
+    ) -> Optional[float]:
+        """Get the last value of a metric."""
+
+        sql_service: SqlService = next(
+            (
+                data_service
+                for data_service in self.data_services
+                if isinstance(data_service, SqlService)
+            ),
+        )
+
+        if sql_service:
+            return await sql_service.last(metric, value_dt)
+
+        return None
```

### Comparing `estimenergy-2.0.9/estimenergy/devices/device_registry.py` & `estimenergy-2.1.0/estimenergy/devices/device_registry.py`

 * *Files identical despite different names*

### Comparing `estimenergy-2.0.9/estimenergy/helpers.py` & `estimenergy-2.1.0/estimenergy/helpers.py`

 * *Files identical despite different names*

### Comparing `estimenergy-2.0.9/estimenergy/log.py` & `estimenergy-2.1.0/estimenergy/log.py`

 * *Files identical despite different names*

### Comparing `estimenergy-2.0.9/estimenergy/main.py` & `estimenergy-2.1.0/estimenergy/main.py`

 * *Files identical despite different names*

### Comparing `estimenergy-2.0.9/estimenergy/models/config/config.py` & `estimenergy-2.1.0/estimenergy/models/config/config.py`

 * *Files identical despite different names*

### Comparing `estimenergy-2.0.9/estimenergy/models/day.py` & `estimenergy-2.1.0/estimenergy/models/day.py`

 * *Files identical despite different names*

### Comparing `estimenergy-2.0.9/estimenergy/models/device_config.py` & `estimenergy-2.1.0/estimenergy/models/device_config.py`

 * *Files identical despite different names*

### Comparing `estimenergy-2.0.9/estimenergy/models/month.py` & `estimenergy-2.1.0/estimenergy/models/month.py`

 * *Files identical despite different names*

### Comparing `estimenergy-2.0.9/estimenergy/models/year.py` & `estimenergy-2.1.0/estimenergy/models/year.py`

 * *Files identical despite different names*

### Comparing `estimenergy-2.0.9/estimenergy/routers/day_router.py` & `estimenergy-2.1.0/estimenergy/routers/day_router.py`

 * *Files identical despite different names*

### Comparing `estimenergy-2.0.9/estimenergy/routers/device_router.py` & `estimenergy-2.1.0/estimenergy/routers/device_router.py`

 * *Files identical despite different names*

### Comparing `estimenergy-2.0.9/estimenergy/routers/month_router.py` & `estimenergy-2.1.0/estimenergy/routers/month_router.py`

 * *Files identical despite different names*

### Comparing `estimenergy-2.0.9/estimenergy/routers/total_router.py` & `estimenergy-2.1.0/estimenergy/routers/total_router.py`

 * *Files identical despite different names*

### Comparing `estimenergy-2.0.9/estimenergy/routers/year_router.py` & `estimenergy-2.1.0/estimenergy/routers/year_router.py`

 * *Files identical despite different names*

### Comparing `estimenergy-2.0.9/estimenergy/services/prediction_service.py` & `estimenergy-2.1.0/estimenergy/services/prediction_service.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         self.device_config = device_config
         self.config = config
 
     async def calculate_cost(
         self,
         metric_period: MetricPeriod,
         energy: float,
-        date: datetime.date = datetime.date.today(),
+        date: datetime.date,
     ) -> float:
         """Calculate the cost."""
 
         if metric_period == MetricPeriod.DAY:
             days_in_month = get_days_in_month(date.month, date.year)
             base_cost = self.device_config.base_cost_per_month / days_in_month
         elif metric_period == MetricPeriod.MONTH:
@@ -40,15 +40,15 @@
 
         return cost
 
     async def calculate_cost_difference(
         self,
         metric_period: MetricPeriod,
         energy: float,
-        date: datetime.date = datetime.date.today(),
+        date: datetime.date,
     ) -> float:
         """Calculate the cost difference."""
 
         if metric_period == MetricPeriod.DAY:
             days_in_month = get_days_in_month(date.month, date.year)
             payment = self.device_config.payment_per_month / days_in_month
         elif metric_period == MetricPeriod.MONTH:
@@ -63,15 +63,15 @@
 
         return cost_difference
 
     async def calculate_accuracy(
         self,
         metric_period: MetricPeriod,
         accuracy_sum: float,
-        date: datetime.date = datetime.date.today(),
+        date: datetime.date,
     ) -> float:
         """Calculate the accuracy."""
 
         if metric_period == MetricPeriod.MONTH:
             day_count = get_days_in_month(date.year, date.month)
         elif metric_period == MetricPeriod.YEAR:
             day_count = get_days_in_year(date.year)
@@ -83,38 +83,39 @@
         return total_accuracy
 
     async def predict_energy(
         self,
         metric_period: MetricPeriod,
         energy: float,
         accurate_day_count: int,
-        date: datetime.date = datetime.date.today(),
+        date: datetime.date,
     ) -> float:
         """Predict the energy."""
 
         if metric_period == MetricPeriod.MONTH:
             day_count = get_days_in_month(date.year, date.month)
         elif metric_period == MetricPeriod.YEAR:
             day_count = get_days_in_year(date.year)
         else:
             return 0
 
         if accurate_day_count == 0:
             return 0
+
         mean_energy_per_day = energy / accurate_day_count
         predicted_energy = mean_energy_per_day * day_count
 
         return predicted_energy
 
     async def predict_cost(
         self,
         metric_period: MetricPeriod,
         energy: float,
         accurate_day_count: int,
-        date: datetime.date = datetime.date.today(),
+        date: datetime.date,
     ) -> float:
         """Predict the cost."""
 
         predicted_energy = await self.predict_energy(
             metric_period, energy, accurate_day_count, date
         )
         predicted_cost = await self.calculate_cost(
@@ -124,15 +125,15 @@
         return predicted_cost
 
     async def predict_cost_difference(
         self,
         metric_period: MetricPeriod,
         energy: float,
         accurate_day_count: int,
-        date: datetime.date = datetime.date.today(),
+        date: datetime.date,
     ) -> float:
         """Predict the cost difference."""
 
         predicted_energy = await self.predict_energy(
             metric_period, energy, accurate_day_count, date
         )
         predicted_cost_difference = await self.calculate_cost_difference(
```

### Comparing `estimenergy-2.0.9/estimenergy/services/prometheus_service.py` & `estimenergy-2.1.0/estimenergy/services/prometheus_service.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import datetime
 
 from prometheus_client import Gauge, Metric as PrometheusMetric
 
 from estimenergy.const import METRICS, Metric
+from estimenergy.log import logger
 from estimenergy.models.config.config import Config
 from estimenergy.models.device_config import DeviceConfig
 from estimenergy.prometheus import metric_registry
 from estimenergy.services.data_service import DataService
 from estimenergy.services.sql_service import SqlService
 
 
@@ -26,41 +27,28 @@
             try:
                 self.gauges[metric] = metric.create_gauge(metric_registry).labels(
                     name=device_config.name
                 )
             except ValueError:
                 pass
 
-    @property
-    def supported_metrics(self):
-        return []
-
-    async def _last(
-        self,
-        metric: Metric,
-        value_dt: datetime.datetime = datetime.datetime.now(),
-    ) -> float:
-        _ = metric
-        _ = value_dt
-
-        return 0
-
-    async def _write(
+    async def write(
         self,
         metric: Metric,
         value: float,
-        value_dt: datetime.datetime = datetime.datetime.now(),
+        value_dt: datetime.datetime,
     ):
         _ = metric
         _ = value
         _ = value_dt
 
     async def update(
         self,
-        value_dt: datetime.datetime = datetime.datetime.now(),
+        value_dt: datetime.datetime,
     ):
-        _ = value_dt
-
         for metric in METRICS:
             last_value = await self.sql_service.last(metric, value_dt)
 
-            self.gauges[metric].set(last_value)
+            try:
+                self.gauges[metric].set(last_value)
+            except KeyError:
+                logger.error(f"Could not find gauge for metric {metric}")
```

### Comparing `estimenergy-2.0.9/estimenergy/services/sql_service.py` & `estimenergy-2.1.0/estimenergy/services/sql_service.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 """Service for writing and reading data from the SQL database."""
 import datetime
-import traceback
 
 from sqlalchemy import extract
 from sqlmodel import Session, select
 from sqlmodel.sql.expression import SelectOfScalar
 
-from estimenergy.const import METRICS, Metric, MetricPeriod, MetricType
+from estimenergy.const import Metric, MetricPeriod
 from estimenergy.db import db_engine
 from estimenergy.models.config.config import Config
 from estimenergy.models.day import Day
 from estimenergy.models.device_config import DeviceConfig
 from estimenergy.models.month import Month
 from estimenergy.models.total import Total
 from estimenergy.models.year import Year
@@ -24,66 +23,58 @@
     prediction_service: PredictionService
 
     def __init__(self, device_config: DeviceConfig, config: Config):
         super().__init__(device_config, config)
 
         self.prediction_service = PredictionService(device_config, config)
 
-    @property
-    def supported_metrics(self) -> list[Metric]:
-        return [
-            metric
-            for metric in METRICS
-            if not metric.is_raw and metric.metric_type != MetricType.POWER
-        ]
-
-    async def _last(
-        self,
-        metric: Metric,
-        value_dt: datetime.datetime = datetime.datetime.now(),
-    ) -> float:
-        """Get a metric value."""
-
-        date = value_dt.date()
-        row = self.get_or_create_row(metric.metric_period, date)
-        value = getattr(row, metric.key, 0)
-
-        return value
-
-    async def _write(
+    async def write(
         self,
         metric: Metric,
         value: float,
-        value_dt: datetime.datetime = datetime.datetime.now(),
+        value_dt: datetime.datetime,
     ):
         """Write a metric value."""
 
         date = value_dt.date()
         row = self.get_or_create_row(metric.metric_period, date)
         setattr(row, metric.key, value)
 
         with Session(db_engine) as session:
             session.add(row)
             session.commit()
 
     async def update(
         self,
-        value_dt: datetime.datetime = datetime.datetime.now(),
+        value_dt: datetime.datetime,
     ):
         """Update all metrics."""
 
         date = value_dt.date()
         await self.update_day(date)
         await self.update_month(date)
         await self.update_year(date)
-        await self.update_total()
+        await self.update_total(date)
+
+    async def last(
+        self,
+        metric: Metric,
+        value_dt: datetime.datetime,
+    ) -> float:
+        """Get a metric value."""
+
+        date = value_dt.date()
+        row = self.get_or_create_row(metric.metric_period, date)
+        value = getattr(row, metric.key, 0)
+
+        return value
 
     async def update_day(
         self,
-        date: datetime.date = datetime.date.today(),
+        date: datetime.date,
     ):
         """Update the day metrics."""
 
         metric_period = MetricPeriod.DAY
 
         with Session(db_engine) as session:
             day = self.get_or_create_row(MetricPeriod.DAY, date)
@@ -92,45 +83,46 @@
                 raise TypeError("day is not of type Day")
 
             day.cost = await self.prediction_service.calculate_cost(
                 metric_period,
                 day.energy,
                 day.date,
             )
+
             day.cost_difference = (
                 await self.prediction_service.calculate_cost_difference(
                     metric_period,
                     day.energy,
                     day.date,
                 )
             )
 
             session.add(day)
             session.commit()
 
     async def update_month(
         self,
-        date: datetime.date = datetime.date.today(),
+        date: datetime.date,
     ):
         """Update the month metrics."""
 
         await self.update_accumulative(MetricPeriod.MONTH, date)
 
     async def update_year(
         self,
-        date: datetime.date = datetime.date.today(),
+        date: datetime.date,
     ):
         """Update the year metrics."""
 
         await self.update_accumulative(MetricPeriod.YEAR, date)
 
     async def update_accumulative(
         self,
         metric_period: MetricPeriod,
-        date: datetime.date = datetime.date.today(),
+        date: datetime.date,
     ):
         """Update accumulative metrics."""
 
         with Session(db_engine) as session:
             row = self.get_or_create_row(metric_period, date)
 
             if metric_period == MetricPeriod.MONTH:
@@ -235,53 +227,54 @@
             row.cost_difference_predicted_raw = cost_difference_predicted_raw
             row.cost_difference_predicted = cost_difference_predicted
             row.accuracy = accuracy
 
             session.add(row)
             session.commit()
 
-    async def update_total(self):
+    async def update_total(self, date: datetime.date):
         """Update the total metrics."""
 
         metric_period = MetricPeriod.TOTAL
 
         with Session(db_engine) as session:
-            total = self.get_or_create_row(metric_period)
+            total = self.get_or_create_row(metric_period, date)
             days = session.exec(select(Day)).all()
             energy = sum(day.energy for day in days)
 
             cost = await self.prediction_service.calculate_cost(
                 metric_period,
                 energy,
+                date,
             )
 
             total.energy = energy
             total.cost = cost
 
             session.add(total)
             session.commit()
 
     def get_or_create_row(
         self,
         metric_period: MetricPeriod,
-        date: datetime.date = datetime.date.today(),
+        date: datetime.date,
     ) -> Day | Month | Year | Total:
         """Get or create a row in the database."""
 
         row = self.get_row(metric_period, date)
 
         if row is None:
             row = self.create_row(metric_period, date)
 
         return row
 
     def create_row(
         self,
         metric_period: MetricPeriod,
-        date: datetime.date = datetime.date.today(),
+        date: datetime.date,
     ) -> Day | Month | Year | Total:
         """Create a row in the database."""
 
         if metric_period == MetricPeriod.DAY:
             return self.create_day(date)
 
         elif metric_period == MetricPeriod.MONTH:
@@ -294,15 +287,15 @@
             return self.create_total()
 
         else:
             raise ValueError(f"Unknown metric period {metric_period}")
 
     def create_day(
         self,
-        date: datetime.date = datetime.date.today(),
+        date: datetime.date,
     ) -> Day:
         """Create a day in the database."""
 
         with Session(db_engine, expire_on_commit=False) as session:
             row = Day(device_name=self.device_config.name, date=date)
             session.add(row)
             session.commit()
@@ -319,15 +312,15 @@
             session.add(row)
             session.commit()
 
         return row
 
     def create_month(
         self,
-        date: datetime.date = datetime.date.today(),
+        date: datetime.date,
     ) -> Month:
         """Create a month in the database."""
 
         with Session(db_engine, expire_on_commit=False) as session:
             date = date.replace(day=1)
             row = Month(device_name=self.device_config.name, date=date)
             session.add(row)
@@ -356,15 +349,15 @@
 
             session.commit()
 
         return row
 
     def create_year(
         self,
-        date: datetime.date = datetime.date.today(),
+        date: datetime.date,
     ) -> Year:
         """Create a year in the database."""
 
         with Session(db_engine, expire_on_commit=False) as session:
             date = date.replace(
                 year=date.year - 1
                 if date.month <= self.device_config.billing_month
@@ -414,15 +407,15 @@
             session.commit()
 
         return row
 
     def get_rows(
         self,
         metric_period: MetricPeriod,
-        date: datetime.date = datetime.date.today(),
+        date: datetime.date,
     ) -> list[Day] | list[Month] | list[Year] | list[Total]:
         """Get rows from the database."""
 
         query: SelectOfScalar[Day] | SelectOfScalar[Month] | SelectOfScalar[
             Year
         ] | SelectOfScalar[Total]
 
@@ -458,15 +451,15 @@
                 raise ValueError(f"Unknown metric period {metric_period}")
 
             return session.exec(query).all()
 
     def get_row(
         self,
         metric_period: MetricPeriod,
-        date: datetime.date = datetime.date.today(),
+        date: datetime.date,
     ) -> Day | Month | Year | Total | None:
         """Get a row from the database."""
 
         rows = self.get_rows(metric_period, date)
 
         if len(rows) == 0:
             return None
```

### Comparing `estimenergy-2.0.9/pyproject.toml` & `estimenergy-2.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 name = "estimenergy"
 description = "Estimate Energy Consumption"
 authors = ["Lennard Beers <l.beers@outlook.de>"]
 repository = "https://github.com/EuleMitKeule/EstimEnergy"
 readme = "README.md"
 packages = [{include = "estimenergy"}]
 license = "MIT"
-version = "2.0.9"
+version = "2.1.0"
 
 [tool.poetry.scripts]
 api = "estimenergy.main:start"
 drop = "estimenergy.db:drop_db"
 generate-openapi = "estimenergy.main:generate_openapi"
 
 [tool.poe.tasks]
@@ -36,15 +36,15 @@
 style = "semver"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 uvicorn = {extras = ["standard"], version = "~0.20.0"}
 fastapi = "~0.92.0"
 fastapi-crudrouter = "~0.8.6"
-aioesphomeapi = "~13.4.0"
+aioesphomeapi = "13.7.2"
 tortoise_orm = "~0.19.3"
 requests = "~2.28.2"
 prometheus_client = "~0.16.0"
 prometheus-fastapi-instrumentator = "~5.10.0"
 python-dotenv = "~0.21.1"
 PyYAML = "~6.0"
 types-requests = "^2.28.11.17"
```

### Comparing `estimenergy-2.0.9/PKG-INFO` & `estimenergy-2.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: estimenergy
-Version: 2.0.9
+Version: 2.1.0
 Summary: Estimate Energy Consumption
 Home-page: https://github.com/EuleMitKeule/EstimEnergy
 License: MIT
 Author: Lennard Beers
 Author-email: l.beers@outlook.de
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: PyYAML (>=6.0,<6.1)
-Requires-Dist: aioesphomeapi (>=13.4.0,<13.5.0)
+Requires-Dist: aioesphomeapi (==13.7.2)
 Requires-Dist: fastapi (>=0.92.0,<0.93.0)
 Requires-Dist: fastapi-crudrouter (>=0.8.6,<0.9.0)
 Requires-Dist: influxdb-client[async] (>=1.36.1,<2.0.0)
 Requires-Dist: prometheus-fastapi-instrumentator (>=5.10.0,<5.11.0)
 Requires-Dist: prometheus_client (>=0.16.0,<0.17.0)
 Requires-Dist: psycopg2-binary (>=2.9.6,<3.0.0)
 Requires-Dist: pydantic-settings-yaml (>=0.1.1,<0.2.0)
```

