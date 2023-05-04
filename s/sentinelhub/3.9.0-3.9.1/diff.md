# Comparing `tmp/sentinelhub-3.9.0.tar.gz` & `tmp/sentinelhub-3.9.1.tar.gz`

## Comparing `sentinelhub-3.9.0.tar` & `sentinelhub-3.9.1.tar`

### file list

```diff
@@ -1,62 +1,62 @@
--rw-r--r--   0        0        0   768447 2020-02-02 00:00:00.000000 sentinelhub-3.9.0/sentinelhub/.utmzones.geojson
--rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 sentinelhub-3.9.0/sentinelhub/__init__.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 sentinelhub-3.9.0/sentinelhub/_version.py
--rw-r--r--   0        0        0    32015 2020-02-02 00:00:00.000000 sentinelhub-3.9.0/sentinelhub/areas.py
--rw-r--r--   0        0        0    12923 2020-02-02 00:00:00.000000 sentinelhub-3.9.0/sentinelhub/base.py
--rw-r--r--   0        0        0     3295 2020-02-02 00:00:00.000000 sentinelhub-3.9.0/sentinelhub/commands.py
--rw-r--r--   0        0        0     9426 2020-02-02 00:00:00.000000 sentinelhub-3.9.0/sentinelhub/config.py
--rw-r--r--   0        0        0    13474 2020-02-02 00:00:00.000000 sentinelhub-3.9.0/sentinelhub/constants.py
--rw-r--r--   0        0        0    24221 2020-02-02 00:00:00.000000 sentinelhub-3.9.0/sentinelhub/data_collections.py
--rw-r--r--   0        0        0    11241 2020-02-02 00:00:00.000000 sentinelhub-3.9.0/sentinelhub/data_collections_bands.py
--rw-r--r--   0        0        0     7075 2020-02-02 00:00:00.000000 sentinelhub-3.9.0/sentinelhub/data_utils.py
--rw-r--r--   0        0        0     6680 2020-02-02 00:00:00.000000 sentinelhub-3.9.0/sentinelhub/decoding.py
--rw-r--r--   0        0        0     4678 2020-02-02 00:00:00.000000 sentinelhub-3.9.0/sentinelhub/evalscript.py
--rw-r--r--   0        0        0     3646 2020-02-02 00:00:00.000000 sentinelhub-3.9.0/sentinelhub/exceptions.py
--rw-r--r--   0        0        0     8245 2020-02-02 00:00:00.000000 sentinelhub-3.9.0/sentinelhub/geo_utils.py
--rw-r--r--   0        0        0    23187 2020-02-02 00:00:00.000000 sentinelhub-3.9.0/sentinelhub/geometry.py
--rw-r--r--   0        0        0     5373 2020-02-02 00:00:00.000000 sentinelhub-3.9.0/sentinelhub/io_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sentinelhub-3.9.0/sentinelhub/py.typed
--rw-r--r--   0        0        0     2373 2020-02-02 00:00:00.000000 sentinelhub-3.9.0/sentinelhub/testing_utils.py
--rw-r--r--   0        0        0     8096 2020-02-02 00:00:00.000000 sentinelhub-3.9.0/sentinelhub/time_utils.py
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 sentinelhub-3.9.0/sentinelhub/types.py
--rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 sentinelhub-3.9.0/sentinelhub/api/__init__.py
--rw-r--r--   0        0        0     4094 2020-02-02 00:00:00.000000 sentinelhub-3.9.0/sentinelhub/api/base.py
--rw-r--r--   0        0        0     9583 2020-02-02 00:00:00.000000 sentinelhub-3.9.0/sentinelhub/api/base_request.py
--rw-r--r--   0        0        0    12169 2020-02-02 00:00:00.000000 sentinelhub-3.9.0/sentinelhub/api/byoc.py
--rw-r--r--   0        0        0    14063 2020-02-02 00:00:00.000000 sentinelhub-3.9.0/sentinelhub/api/catalog.py
--rw-r--r--   0        0        0     6467 2020-02-02 00:00:00.000000 sentinelhub-3.9.0/sentinelhub/api/fis.py
--rw-r--r--   0        0        0    30356 2020-02-02 00:00:00.000000 sentinelhub-3.9.0/sentinelhub/api/ogc.py
--rw-r--r--   0        0        0     7746 2020-02-02 00:00:00.000000 sentinelhub-3.9.0/sentinelhub/api/opensearch.py
--rw-r--r--   0        0        0    13657 2020-02-02 00:00:00.000000 sentinelhub-3.9.0/sentinelhub/api/process.py
--rw-r--r--   0        0        0     5316 2020-02-02 00:00:00.000000 sentinelhub-3.9.0/sentinelhub/api/statistical.py
--rw-r--r--   0        0        0     3147 2020-02-02 00:00:00.000000 sentinelhub-3.9.0/sentinelhub/api/utils.py
--rw-r--r--   0        0        0     7648 2020-02-02 00:00:00.000000 sentinelhub-3.9.0/sentinelhub/api/wfs.py
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 sentinelhub-3.9.0/sentinelhub/api/batch/__init__.py
--rw-r--r--   0        0        0     4230 2020-02-02 00:00:00.000000 sentinelhub-3.9.0/sentinelhub/api/batch/base.py
--rw-r--r--   0        0        0    24234 2020-02-02 00:00:00.000000 sentinelhub-3.9.0/sentinelhub/api/batch/process.py
--rw-r--r--   0        0        0     8077 2020-02-02 00:00:00.000000 sentinelhub-3.9.0/sentinelhub/api/batch/statistical.py
--rw-r--r--   0        0        0    10771 2020-02-02 00:00:00.000000 sentinelhub-3.9.0/sentinelhub/api/batch/utils.py
--rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 sentinelhub-3.9.0/sentinelhub/aws/__init__.py
--rw-r--r--   0        0        0     4135 2020-02-02 00:00:00.000000 sentinelhub-3.9.0/sentinelhub/aws/batch.py
--rw-r--r--   0        0        0     4616 2020-02-02 00:00:00.000000 sentinelhub-3.9.0/sentinelhub/aws/client.py
--rw-r--r--   0        0        0     2842 2020-02-02 00:00:00.000000 sentinelhub-3.9.0/sentinelhub/aws/commands.py
--rw-r--r--   0        0        0     6427 2020-02-02 00:00:00.000000 sentinelhub-3.9.0/sentinelhub/aws/constants.py
--rw-r--r--   0        0        0    30113 2020-02-02 00:00:00.000000 sentinelhub-3.9.0/sentinelhub/aws/data.py
--rw-r--r--   0        0        0    18453 2020-02-02 00:00:00.000000 sentinelhub-3.9.0/sentinelhub/aws/data_safe.py
--rw-r--r--   0        0        0    10871 2020-02-02 00:00:00.000000 sentinelhub-3.9.0/sentinelhub/aws/request.py
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 sentinelhub-3.9.0/sentinelhub/download/__init__.py
--rw-r--r--   0        0        0    11659 2020-02-02 00:00:00.000000 sentinelhub-3.9.0/sentinelhub/download/client.py
--rw-r--r--   0        0        0     5458 2020-02-02 00:00:00.000000 sentinelhub-3.9.0/sentinelhub/download/handlers.py
--rw-r--r--   0        0        0    10103 2020-02-02 00:00:00.000000 sentinelhub-3.9.0/sentinelhub/download/models.py
--rw-r--r--   0        0        0     4952 2020-02-02 00:00:00.000000 sentinelhub-3.9.0/sentinelhub/download/rate_limit.py
--rw-r--r--   0        0        0     8784 2020-02-02 00:00:00.000000 sentinelhub-3.9.0/sentinelhub/download/sentinelhub_client.py
--rw-r--r--   0        0        0     4443 2020-02-02 00:00:00.000000 sentinelhub-3.9.0/sentinelhub/download/sentinelhub_statistical_client.py
--rw-r--r--   0        0        0    14689 2020-02-02 00:00:00.000000 sentinelhub-3.9.0/sentinelhub/download/session.py
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 sentinelhub-3.9.0/sentinelhub/geopedia/__init__.py
--rw-r--r--   0        0        0    16486 2020-02-02 00:00:00.000000 sentinelhub-3.9.0/sentinelhub/geopedia/core.py
--rw-r--r--   0        0        0     6629 2020-02-02 00:00:00.000000 sentinelhub-3.9.0/sentinelhub/geopedia/request.py
--rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 sentinelhub-3.9.0/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 sentinelhub-3.9.0/LICENSE.md
--rw-r--r--   0        0        0     6022 2020-02-02 00:00:00.000000 sentinelhub-3.9.0/README.md
--rw-r--r--   0        0        0     4091 2020-02-02 00:00:00.000000 sentinelhub-3.9.0/pyproject.toml
--rw-r--r--   0        0        0    10391 2020-02-02 00:00:00.000000 sentinelhub-3.9.0/PKG-INFO
+-rw-r--r--   0        0        0   768447 2020-02-02 00:00:00.000000 sentinelhub-3.9.1/sentinelhub/.utmzones.geojson
+-rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 sentinelhub-3.9.1/sentinelhub/__init__.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 sentinelhub-3.9.1/sentinelhub/_version.py
+-rw-r--r--   0        0        0    32015 2020-02-02 00:00:00.000000 sentinelhub-3.9.1/sentinelhub/areas.py
+-rw-r--r--   0        0        0    12923 2020-02-02 00:00:00.000000 sentinelhub-3.9.1/sentinelhub/base.py
+-rw-r--r--   0        0        0     3295 2020-02-02 00:00:00.000000 sentinelhub-3.9.1/sentinelhub/commands.py
+-rw-r--r--   0        0        0    10067 2020-02-02 00:00:00.000000 sentinelhub-3.9.1/sentinelhub/config.py
+-rw-r--r--   0        0        0    13474 2020-02-02 00:00:00.000000 sentinelhub-3.9.1/sentinelhub/constants.py
+-rw-r--r--   0        0        0    24353 2020-02-02 00:00:00.000000 sentinelhub-3.9.1/sentinelhub/data_collections.py
+-rw-r--r--   0        0        0    11241 2020-02-02 00:00:00.000000 sentinelhub-3.9.1/sentinelhub/data_collections_bands.py
+-rw-r--r--   0        0        0     7075 2020-02-02 00:00:00.000000 sentinelhub-3.9.1/sentinelhub/data_utils.py
+-rw-r--r--   0        0        0     6680 2020-02-02 00:00:00.000000 sentinelhub-3.9.1/sentinelhub/decoding.py
+-rw-r--r--   0        0        0     4606 2020-02-02 00:00:00.000000 sentinelhub-3.9.1/sentinelhub/evalscript.py
+-rw-r--r--   0        0        0     3646 2020-02-02 00:00:00.000000 sentinelhub-3.9.1/sentinelhub/exceptions.py
+-rw-r--r--   0        0        0     8245 2020-02-02 00:00:00.000000 sentinelhub-3.9.1/sentinelhub/geo_utils.py
+-rw-r--r--   0        0        0    23253 2020-02-02 00:00:00.000000 sentinelhub-3.9.1/sentinelhub/geometry.py
+-rw-r--r--   0        0        0     5373 2020-02-02 00:00:00.000000 sentinelhub-3.9.1/sentinelhub/io_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sentinelhub-3.9.1/sentinelhub/py.typed
+-rw-r--r--   0        0        0     2373 2020-02-02 00:00:00.000000 sentinelhub-3.9.1/sentinelhub/testing_utils.py
+-rw-r--r--   0        0        0     8096 2020-02-02 00:00:00.000000 sentinelhub-3.9.1/sentinelhub/time_utils.py
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 sentinelhub-3.9.1/sentinelhub/types.py
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 sentinelhub-3.9.1/sentinelhub/api/__init__.py
+-rw-r--r--   0        0        0     4094 2020-02-02 00:00:00.000000 sentinelhub-3.9.1/sentinelhub/api/base.py
+-rw-r--r--   0        0        0     9583 2020-02-02 00:00:00.000000 sentinelhub-3.9.1/sentinelhub/api/base_request.py
+-rw-r--r--   0        0        0    12169 2020-02-02 00:00:00.000000 sentinelhub-3.9.1/sentinelhub/api/byoc.py
+-rw-r--r--   0        0        0    14064 2020-02-02 00:00:00.000000 sentinelhub-3.9.1/sentinelhub/api/catalog.py
+-rw-r--r--   0        0        0     6467 2020-02-02 00:00:00.000000 sentinelhub-3.9.1/sentinelhub/api/fis.py
+-rw-r--r--   0        0        0    30356 2020-02-02 00:00:00.000000 sentinelhub-3.9.1/sentinelhub/api/ogc.py
+-rw-r--r--   0        0        0     7746 2020-02-02 00:00:00.000000 sentinelhub-3.9.1/sentinelhub/api/opensearch.py
+-rw-r--r--   0        0        0    13657 2020-02-02 00:00:00.000000 sentinelhub-3.9.1/sentinelhub/api/process.py
+-rw-r--r--   0        0        0     5316 2020-02-02 00:00:00.000000 sentinelhub-3.9.1/sentinelhub/api/statistical.py
+-rw-r--r--   0        0        0     3147 2020-02-02 00:00:00.000000 sentinelhub-3.9.1/sentinelhub/api/utils.py
+-rw-r--r--   0        0        0     7648 2020-02-02 00:00:00.000000 sentinelhub-3.9.1/sentinelhub/api/wfs.py
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 sentinelhub-3.9.1/sentinelhub/api/batch/__init__.py
+-rw-r--r--   0        0        0     4230 2020-02-02 00:00:00.000000 sentinelhub-3.9.1/sentinelhub/api/batch/base.py
+-rw-r--r--   0        0        0    24234 2020-02-02 00:00:00.000000 sentinelhub-3.9.1/sentinelhub/api/batch/process.py
+-rw-r--r--   0        0        0     8077 2020-02-02 00:00:00.000000 sentinelhub-3.9.1/sentinelhub/api/batch/statistical.py
+-rw-r--r--   0        0        0    10771 2020-02-02 00:00:00.000000 sentinelhub-3.9.1/sentinelhub/api/batch/utils.py
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 sentinelhub-3.9.1/sentinelhub/aws/__init__.py
+-rw-r--r--   0        0        0     4135 2020-02-02 00:00:00.000000 sentinelhub-3.9.1/sentinelhub/aws/batch.py
+-rw-r--r--   0        0        0     4616 2020-02-02 00:00:00.000000 sentinelhub-3.9.1/sentinelhub/aws/client.py
+-rw-r--r--   0        0        0     2842 2020-02-02 00:00:00.000000 sentinelhub-3.9.1/sentinelhub/aws/commands.py
+-rw-r--r--   0        0        0     6427 2020-02-02 00:00:00.000000 sentinelhub-3.9.1/sentinelhub/aws/constants.py
+-rw-r--r--   0        0        0    30113 2020-02-02 00:00:00.000000 sentinelhub-3.9.1/sentinelhub/aws/data.py
+-rw-r--r--   0        0        0    18453 2020-02-02 00:00:00.000000 sentinelhub-3.9.1/sentinelhub/aws/data_safe.py
+-rw-r--r--   0        0        0    10871 2020-02-02 00:00:00.000000 sentinelhub-3.9.1/sentinelhub/aws/request.py
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 sentinelhub-3.9.1/sentinelhub/download/__init__.py
+-rw-r--r--   0        0        0    11659 2020-02-02 00:00:00.000000 sentinelhub-3.9.1/sentinelhub/download/client.py
+-rw-r--r--   0        0        0     5458 2020-02-02 00:00:00.000000 sentinelhub-3.9.1/sentinelhub/download/handlers.py
+-rw-r--r--   0        0        0    10103 2020-02-02 00:00:00.000000 sentinelhub-3.9.1/sentinelhub/download/models.py
+-rw-r--r--   0        0        0     4952 2020-02-02 00:00:00.000000 sentinelhub-3.9.1/sentinelhub/download/rate_limit.py
+-rw-r--r--   0        0        0     8784 2020-02-02 00:00:00.000000 sentinelhub-3.9.1/sentinelhub/download/sentinelhub_client.py
+-rw-r--r--   0        0        0     4443 2020-02-02 00:00:00.000000 sentinelhub-3.9.1/sentinelhub/download/sentinelhub_statistical_client.py
+-rw-r--r--   0        0        0    14673 2020-02-02 00:00:00.000000 sentinelhub-3.9.1/sentinelhub/download/session.py
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 sentinelhub-3.9.1/sentinelhub/geopedia/__init__.py
+-rw-r--r--   0        0        0    16486 2020-02-02 00:00:00.000000 sentinelhub-3.9.1/sentinelhub/geopedia/core.py
+-rw-r--r--   0        0        0     6629 2020-02-02 00:00:00.000000 sentinelhub-3.9.1/sentinelhub/geopedia/request.py
+-rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 sentinelhub-3.9.1/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 sentinelhub-3.9.1/LICENSE.md
+-rw-r--r--   0        0        0     6022 2020-02-02 00:00:00.000000 sentinelhub-3.9.1/README.md
+-rw-r--r--   0        0        0     4122 2020-02-02 00:00:00.000000 sentinelhub-3.9.1/pyproject.toml
+-rw-r--r--   0        0        0    10403 2020-02-02 00:00:00.000000 sentinelhub-3.9.1/PKG-INFO
```

### Comparing `sentinelhub-3.9.0/sentinelhub/.utmzones.geojson` & `sentinelhub-3.9.1/sentinelhub/.utmzones.geojson`

 * *Files identical despite different names*

### Comparing `sentinelhub-3.9.0/sentinelhub/__init__.py` & `sentinelhub-3.9.1/sentinelhub/__init__.py`

 * *Files identical despite different names*

### Comparing `sentinelhub-3.9.0/sentinelhub/areas.py` & `sentinelhub-3.9.1/sentinelhub/areas.py`

 * *Files identical despite different names*

### Comparing `sentinelhub-3.9.0/sentinelhub/base.py` & `sentinelhub-3.9.1/sentinelhub/base.py`

 * *Files identical despite different names*

### Comparing `sentinelhub-3.9.0/sentinelhub/commands.py` & `sentinelhub-3.9.1/sentinelhub/commands.py`

 * *Files identical despite different names*

### Comparing `sentinelhub-3.9.0/sentinelhub/config.py` & `sentinelhub-3.9.1/sentinelhub/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,34 +2,38 @@
 Module for managing configuration data from `config.toml`
 """
 from __future__ import annotations
 
 import copy
 import json
 import os
+import warnings
 from dataclasses import asdict, dataclass
 from pathlib import Path
 from typing import Any, Dict, Optional, Union
 
 import tomli
 import tomli_w
 
+from .exceptions import SHDeprecationWarning
+
 DEFAULT_PROFILE = "default-profile"
 SH_PROFILE_ENV_VAR = "SH_PROFILE"
 SH_CLIENT_ID_ENV_VAR = "SH_CLIENT_ID"
 SH_CLIENT_SECRET_ENV_VAR = "SH_CLIENT_SECRET"
 
 
 @dataclass(repr=False)
 class _SHConfig:
     instance_id: str = ""
     sh_client_id: str = ""
     sh_client_secret: str = ""
     sh_base_url: str = "https://services.sentinel-hub.com"
-    sh_auth_base_url: str = "https://services.sentinel-hub.com"
+    sh_auth_base_url: Optional[str] = None
+    sh_token_url: str = "https://services.sentinel-hub.com/oauth/token"
     geopedia_wms_url: str = "https://service.geopedia.world"
     geopedia_rest_url: str = "https://www.geopedia.world/rest"
     aws_access_key_id: str = ""
     aws_secret_access_key: str = ""
     aws_session_token: str = ""
     aws_metadata_url: str = "https://roda.sentinel-hub.com"
     aws_s3_l1c_bucket: str = "sentinel-s2-l1c"
@@ -39,14 +43,25 @@
     max_opensearch_records_per_query: int = 500  # pylint: disable=invalid-name
     max_download_attempts: int = 4
     download_sleep_time: float = 5.0
     download_timeout_seconds: float = 120.0
     number_of_download_processes: int = 1
 
     def __post_init__(self) -> None:
+        if self.sh_auth_base_url is not None:
+            self.sh_token_url = self.sh_auth_base_url + "/oauth/token"
+            warnings.warn(
+                (
+                    "The parameter `sh_auth_base_url` of `SHConfig` has been replaced with `sh_token_url`. Please"
+                    " update your configuration, for now the parameters were automatically adjusted to `sh_token_url ="
+                    " sh_auth_base_url + '/oauth/token'`."
+                ),
+                category=SHDeprecationWarning,
+            )
+
         if self.max_wfs_records_per_query > 100:
             raise ValueError("Value of config parameter `max_wfs_records_per_query` must be at most 100")
         if self.max_opensearch_records_per_query > 500:
             raise ValueError("Value of config parameter `max_opensearch_records_per_query` must be at most 500")
 
 
 class SHConfig(_SHConfig):
@@ -57,16 +72,16 @@
         - `instance_id`: An instance ID for Sentinel Hub service used for OGC requests.
         - `sh_client_id`: User's OAuth client ID for Sentinel Hub service. Can be set via SH_CLIENT_ID environment
           variable. The environment variable has precedence.
         - `sh_client_secret`: User's OAuth client secret for Sentinel Hub service. Can be set via SH_CLIENT_SECRET
           environment variable. The environment variable has precedence.
         - `sh_base_url`: There exist multiple deployed instances of Sentinel Hub service, this parameter defines the
           location of a specific service instance.
-        - `sh_auth_base_url`: Base url for Sentinel Hub Authentication service. Authentication is typically sent to the
-          main service deployment even if `sh_base_url` points to another deployment.
+        - `sh_token_url`: Url for Sentinel Hub Authentication service. Authentication is typically sent to the main
+          service deployment even if `sh_base_url` points to another deployment.
         - `geopedia_wms_url`: Base url for Geopedia WMS services.
         - `geopedia_rest_url`: Base url for Geopedia REST services.
         - `aws_access_key_id`: Access key for AWS Requester Pays buckets.
         - `aws_secret_access_key`: Secret access key for AWS Requester Pays buckets.
         - `aws_session_token`: A session token for your AWS account. It is only needed when you are using temporary
           credentials.
         - `aws_metadata_url`: Base url for publicly available metadata files
```

### Comparing `sentinelhub-3.9.0/sentinelhub/constants.py` & `sentinelhub-3.9.1/sentinelhub/constants.py`

 * *Files identical despite different names*

### Comparing `sentinelhub-3.9.0/sentinelhub/data_collections.py` & `sentinelhub-3.9.1/sentinelhub/data_collections.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 """
 Module defining data collections
 """
 from dataclasses import dataclass, field, fields
-from enum import Enum, EnumMeta
-from typing import Any, Dict, List, Optional, Tuple
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple
 
 from aenum import extend_enum
 
 from .constants import ServiceUrl
 from .data_collections_bands import Band, Bands, MetaBands
 
+if TYPE_CHECKING:
+    from enum import Enum, EnumMeta  # mypy has a custom plugin for enum but not aenum
+else:
+    from aenum import Enum, EnumMeta
+
 
 class _CollectionType:
     """Types of Sentinel Hub data collections"""
 
     SENTINEL1 = "Sentinel-1"
     SENTINEL2 = "Sentinel-2"
     SENTINEL3 = "Sentinel-3"
```

### Comparing `sentinelhub-3.9.0/sentinelhub/data_collections_bands.py` & `sentinelhub-3.9.1/sentinelhub/data_collections_bands.py`

 * *Files identical despite different names*

### Comparing `sentinelhub-3.9.0/sentinelhub/data_utils.py` & `sentinelhub-3.9.1/sentinelhub/data_utils.py`

 * *Files identical despite different names*

### Comparing `sentinelhub-3.9.0/sentinelhub/decoding.py` & `sentinelhub-3.9.1/sentinelhub/decoding.py`

 * *Files identical despite different names*

### Comparing `sentinelhub-3.9.0/sentinelhub/evalscript.py` & `sentinelhub-3.9.1/sentinelhub/evalscript.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,35 +12,35 @@
     bool: "UINT8",
     np.uint8: "UINT8",
     np.uint16: "UINT16",
     np.float32: "FLOAT32",
 }
 
 EVALSCRIPT_TEMPLATE = """
-    //VERSION=3
+//VERSION=3
 
-    function setup() {{
-        return {{
-            input: [{{
-                bands: [{input_names}],
-                units: [{input_units}]
-            }}],
-            output: [{output_spec}]
-        }}
+function setup() {{
+    return {{
+        input: [{{
+            bands: [{input_names}],
+            units: [{input_units}]
+        }}],
+        output: [{output_spec}]
     }}
+}}
 
-    function updateOutputMetadata(scenes, inputMetadata, outputMetadata) {{
-        outputMetadata.userData = {{
-            "norm_factor":  inputMetadata.normalizationFactor
-        }}
+function updateOutputMetadata(scenes, inputMetadata, outputMetadata) {{
+    outputMetadata.userData = {{
+        "norm_factor":  inputMetadata.normalizationFactor
     }}
+}}
 
-    function evaluatePixel(sample) {{
-        return {{ {return_spec} }};
-    }}
+function evaluatePixel(sample) {{
+    return {{ {return_spec} }};
+}}
 """
 
 
 def parse_data_collection_bands(data_collection: DataCollection, bands: List[str]) -> List[Band]:
     """Checks that all requested bands are available and returns the band information for further processing
 
     :param data_collection: A collection of requested satellite data.
```

### Comparing `sentinelhub-3.9.0/sentinelhub/exceptions.py` & `sentinelhub-3.9.1/sentinelhub/exceptions.py`

 * *Files identical despite different names*

### Comparing `sentinelhub-3.9.0/sentinelhub/geo_utils.py` & `sentinelhub-3.9.1/sentinelhub/geo_utils.py`

 * *Files identical despite different names*

### Comparing `sentinelhub-3.9.0/sentinelhub/geometry.py` & `sentinelhub-3.9.1/sentinelhub/geometry.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from math import ceil
 from typing import Callable, Dict, Iterator, List, Optional, Tuple, TypeVar, Union, cast
 
 import shapely.geometry
 import shapely.geometry.base
 import shapely.ops
 import shapely.wkt
+from shapely.errors import GeometryTypeError
 from shapely.geometry import MultiPolygon, Polygon
 from typing_extensions import TypeAlias
 
 from .constants import CRS
 from .exceptions import SHDeprecationWarning
 from .geo_utils import transform_point
 
@@ -540,16 +541,17 @@
 
         :param geometry: A representation of the geometry
         :return: Shapely polygon or multipolygon
         :raises TypeError
         """
         if isinstance(geometry, str):
             geometry = shapely.wkt.loads(geometry)
-        elif isinstance(geometry, dict):
-            geometry = shapely.geometry.shape(geometry)
-        elif not isinstance(geometry, shapely.geometry.base.BaseGeometry):
-            raise TypeError("Unsupported geometry representation")
+        else:
+            try:
+                geometry = shapely.geometry.shape(geometry)
+            except (GeometryTypeError, AttributeError) as exception:
+                raise ValueError(f"Unable to parse value {geometry} as a geometry.") from exception
 
         if not isinstance(geometry, (Polygon, MultiPolygon)):
             raise ValueError(f"Supported geometry types are polygon and multipolygon, got {type(geometry)}")
 
         return geometry
```

### Comparing `sentinelhub-3.9.0/sentinelhub/io_utils.py` & `sentinelhub-3.9.1/sentinelhub/io_utils.py`

 * *Files identical despite different names*

### Comparing `sentinelhub-3.9.0/sentinelhub/testing_utils.py` & `sentinelhub-3.9.1/sentinelhub/testing_utils.py`

 * *Files identical despite different names*

### Comparing `sentinelhub-3.9.0/sentinelhub/time_utils.py` & `sentinelhub-3.9.1/sentinelhub/time_utils.py`

 * *Files identical despite different names*

### Comparing `sentinelhub-3.9.0/sentinelhub/api/__init__.py` & `sentinelhub-3.9.1/sentinelhub/api/__init__.py`

 * *Files identical despite different names*

### Comparing `sentinelhub-3.9.0/sentinelhub/api/base.py` & `sentinelhub-3.9.1/sentinelhub/api/base.py`

 * *Files identical despite different names*

### Comparing `sentinelhub-3.9.0/sentinelhub/api/base_request.py` & `sentinelhub-3.9.1/sentinelhub/api/base_request.py`

 * *Files identical despite different names*

### Comparing `sentinelhub-3.9.0/sentinelhub/api/byoc.py` & `sentinelhub-3.9.1/sentinelhub/api/byoc.py`

 * *Files identical despite different names*

### Comparing `sentinelhub-3.9.0/sentinelhub/api/catalog.py` & `sentinelhub-3.9.1/sentinelhub/api/catalog.py`

 * *Files 1% similar despite different names*

```diff
@@ -271,15 +271,15 @@
 def get_available_timestamps(
     bbox: BBox,
     time_interval: Optional[RawTimeIntervalType],
     data_collection: DataCollection,
     *,
     time_difference: Optional[dt.timedelta] = None,
     ignore_tz: bool = True,
-    maxcc: Optional[float] = 1.0,
+    maxcc: Optional[float] = None,
     config: Optional[SHConfig] = None,
 ) -> List[dt.datetime]:
     """Helper function to search for all available timestamps for a given area and query parameters.
 
     :param bbox: A bounding box of the search area.
     :param data_collection: A collection specifying the satellite data source for finding available timestamps.
     :param time_interval: A time interval from which to provide the timestamps.
```

### Comparing `sentinelhub-3.9.0/sentinelhub/api/fis.py` & `sentinelhub-3.9.1/sentinelhub/api/fis.py`

 * *Files identical despite different names*

### Comparing `sentinelhub-3.9.0/sentinelhub/api/ogc.py` & `sentinelhub-3.9.1/sentinelhub/api/ogc.py`

 * *Files identical despite different names*

### Comparing `sentinelhub-3.9.0/sentinelhub/api/opensearch.py` & `sentinelhub-3.9.1/sentinelhub/api/opensearch.py`

 * *Files identical despite different names*

### Comparing `sentinelhub-3.9.0/sentinelhub/api/process.py` & `sentinelhub-3.9.1/sentinelhub/api/process.py`

 * *Files identical despite different names*

### Comparing `sentinelhub-3.9.0/sentinelhub/api/statistical.py` & `sentinelhub-3.9.1/sentinelhub/api/statistical.py`

 * *Files identical despite different names*

### Comparing `sentinelhub-3.9.0/sentinelhub/api/utils.py` & `sentinelhub-3.9.1/sentinelhub/api/utils.py`

 * *Files identical despite different names*

### Comparing `sentinelhub-3.9.0/sentinelhub/api/wfs.py` & `sentinelhub-3.9.1/sentinelhub/api/wfs.py`

 * *Files identical despite different names*

### Comparing `sentinelhub-3.9.0/sentinelhub/api/batch/base.py` & `sentinelhub-3.9.1/sentinelhub/api/batch/base.py`

 * *Files identical despite different names*

### Comparing `sentinelhub-3.9.0/sentinelhub/api/batch/process.py` & `sentinelhub-3.9.1/sentinelhub/api/batch/process.py`

 * *Files identical despite different names*

### Comparing `sentinelhub-3.9.0/sentinelhub/api/batch/statistical.py` & `sentinelhub-3.9.1/sentinelhub/api/batch/statistical.py`

 * *Files identical despite different names*

### Comparing `sentinelhub-3.9.0/sentinelhub/api/batch/utils.py` & `sentinelhub-3.9.1/sentinelhub/api/batch/utils.py`

 * *Files identical despite different names*

### Comparing `sentinelhub-3.9.0/sentinelhub/aws/batch.py` & `sentinelhub-3.9.1/sentinelhub/aws/batch.py`

 * *Files identical despite different names*

### Comparing `sentinelhub-3.9.0/sentinelhub/aws/client.py` & `sentinelhub-3.9.1/sentinelhub/aws/client.py`

 * *Files identical despite different names*

### Comparing `sentinelhub-3.9.0/sentinelhub/aws/commands.py` & `sentinelhub-3.9.1/sentinelhub/aws/commands.py`

 * *Files identical despite different names*

### Comparing `sentinelhub-3.9.0/sentinelhub/aws/constants.py` & `sentinelhub-3.9.1/sentinelhub/aws/constants.py`

 * *Files identical despite different names*

### Comparing `sentinelhub-3.9.0/sentinelhub/aws/data.py` & `sentinelhub-3.9.1/sentinelhub/aws/data.py`

 * *Files identical despite different names*

### Comparing `sentinelhub-3.9.0/sentinelhub/aws/data_safe.py` & `sentinelhub-3.9.1/sentinelhub/aws/data_safe.py`

 * *Files identical despite different names*

### Comparing `sentinelhub-3.9.0/sentinelhub/aws/request.py` & `sentinelhub-3.9.1/sentinelhub/aws/request.py`

 * *Files identical despite different names*

### Comparing `sentinelhub-3.9.0/sentinelhub/download/client.py` & `sentinelhub-3.9.1/sentinelhub/download/client.py`

 * *Files identical despite different names*

### Comparing `sentinelhub-3.9.0/sentinelhub/download/handlers.py` & `sentinelhub-3.9.1/sentinelhub/download/handlers.py`

 * *Files identical despite different names*

### Comparing `sentinelhub-3.9.0/sentinelhub/download/models.py` & `sentinelhub-3.9.1/sentinelhub/download/models.py`

 * *Files identical despite different names*

### Comparing `sentinelhub-3.9.0/sentinelhub/download/rate_limit.py` & `sentinelhub-3.9.1/sentinelhub/download/rate_limit.py`

 * *Files identical despite different names*

### Comparing `sentinelhub-3.9.0/sentinelhub/download/sentinelhub_client.py` & `sentinelhub-3.9.1/sentinelhub/download/sentinelhub_client.py`

 * *Files identical despite different names*

### Comparing `sentinelhub-3.9.0/sentinelhub/download/sentinelhub_statistical_client.py` & `sentinelhub-3.9.1/sentinelhub/download/sentinelhub_statistical_client.py`

 * *Files identical despite different names*

### Comparing `sentinelhub-3.9.0/sentinelhub/download/session.py` & `sentinelhub-3.9.1/sentinelhub/download/session.py`

 * *Files 1% similar despite different names*

```diff
@@ -121,15 +121,15 @@
 
     def _collect_new_token(self) -> JsonDict:
         """Creates a download request and fetches a token from the service.
 
         Note that the `DownloadRequest` object is created only because retry decorators of `_fetch_token` method
         require it.
         """
-        request = DownloadRequest(url=f"{self.config.sh_auth_base_url}/oauth/token")
+        request = DownloadRequest(url=f"{self.config.sh_token_url}")
         return self._fetch_token(request)
 
     @retry_temporary_errors
     @fail_user_errors
     def _fetch_token(self, request: DownloadRequest) -> JsonDict:
         """Collects a new token from Sentinel Hub service"""
         oauth_client = BackendApplicationClient(client_id=self.config.sh_client_id)
```

### Comparing `sentinelhub-3.9.0/sentinelhub/geopedia/core.py` & `sentinelhub-3.9.1/sentinelhub/geopedia/core.py`

 * *Files identical despite different names*

### Comparing `sentinelhub-3.9.0/sentinelhub/geopedia/request.py` & `sentinelhub-3.9.1/sentinelhub/geopedia/request.py`

 * *Files identical despite different names*

### Comparing `sentinelhub-3.9.0/.gitignore` & `sentinelhub-3.9.1/.gitignore`

 * *Files identical despite different names*

### Comparing `sentinelhub-3.9.0/LICENSE.md` & `sentinelhub-3.9.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sentinelhub-3.9.0/README.md` & `sentinelhub-3.9.1/README.md`

 * *Files identical despite different names*

### Comparing `sentinelhub-3.9.0/pyproject.toml` & `sentinelhub-3.9.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     "Operating System :: Microsoft :: Windows",
     "Operating System :: Unix",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Topic :: Scientific/Engineering",
     "Topic :: Software Development",
 ]
 dependencies = [
     "aenum>=2.1.4",
     "click",
     "dataclasses-json",
@@ -66,15 +67,14 @@
     "sphinx_rtd_theme",
 ]
 dev = [
     "basemap",
     "boto3-stubs>=1.20.0",
     "build",
     "click>=8.0.0",
-    "codecov",
     "fs",
     "mypy>=0.990",
     "moto",
     "pandas",
     "pre-commit",
     "pylint>=2.14.0",
     "pytest>=4.0.0",
@@ -128,15 +128,15 @@
     "unspecified-encoding",
     "unnecessary-ellipsis",
     "use-dict-literal",
 ]
 
 [tool.pylint.design]
 max-args = 10
-max-attributes = 20
+max-attributes = 21
 max-locals = 20
 min-public-methods = 0
 
 [tool.pylint.similarities]
 min-similarity-lines = 5
 
 [tool.pylint.classes]
```

### Comparing `sentinelhub-3.9.0/PKG-INFO` & `sentinelhub-3.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentinelhub
-Version: 3.9.0
+Version: 3.9.1
 Summary: Python API for Sentinel Hub
 Project-URL: Homepage, https://github.com/sentinel-hub/sentinelhub-py
 Project-URL: Documentation, https://sentinelhub-py.readthedocs.io
 Project-URL: Issues, https://github.com/sentinel-hub/sentinelhub-py/issues
 Project-URL: Source, https://github.com/sentinel-hub/sentinelhub-py
 Project-URL: Forum, https://forum.sentinel-hub.com
 Author-email: Sinergise EO research team <eoresearch@sinergise.com>
@@ -39,14 +39,15 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Requires-Python: >=3.8
 Requires-Dist: aenum>=2.1.4
 Requires-Dist: click
 Requires-Dist: dataclasses-json
 Requires-Dist: numpy
@@ -67,15 +68,14 @@
 Requires-Dist: boto3; extra == 'aws'
 Requires-Dist: botocore; extra == 'aws'
 Provides-Extra: dev
 Requires-Dist: basemap; extra == 'dev'
 Requires-Dist: boto3-stubs>=1.20.0; extra == 'dev'
 Requires-Dist: build; extra == 'dev'
 Requires-Dist: click>=8.0.0; extra == 'dev'
-Requires-Dist: codecov; extra == 'dev'
 Requires-Dist: fs; extra == 'dev'
 Requires-Dist: moto; extra == 'dev'
 Requires-Dist: mypy>=0.990; extra == 'dev'
 Requires-Dist: pandas; extra == 'dev'
 Requires-Dist: pre-commit; extra == 'dev'
 Requires-Dist: pylint>=2.14.0; extra == 'dev'
 Requires-Dist: pytest-cov; extra == 'dev'
```

