# Comparing `tmp/smartsheet-pydantic-1.4.2.tar.gz` & `tmp/smartsheet-pydantic-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartsheet-pydantic-1.4.2.tar", last modified: Tue May  2 18:16:41 2023, max compression
+gzip compressed data, was "smartsheet-pydantic-1.4.3.tar", last modified: Wed May  3 23:07:24 2023, max compression
```

## Comparing `smartsheet-pydantic-1.4.2.tar` & `smartsheet-pydantic-1.4.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 agile     (1000) agile     (1000)        0 2023-05-02 18:16:41.685139 smartsheet-pydantic-1.4.2/
--rw-rw-r--   0 agile     (1000) agile     (1000)     1091 2023-05-01 22:13:12.000000 smartsheet-pydantic-1.4.2/LICENSE
--rw-rw-r--   0 agile     (1000) agile     (1000)     8575 2023-05-02 18:16:41.685139 smartsheet-pydantic-1.4.2/PKG-INFO
--rw-rw-r--   0 agile     (1000) agile     (1000)     6925 2023-05-01 22:13:12.000000 smartsheet-pydantic-1.4.2/README.md
--rw-rw-r--   0 agile     (1000) agile     (1000)      811 2023-05-02 18:16:18.000000 smartsheet-pydantic-1.4.2/pyproject.toml
--rw-rw-r--   0 agile     (1000) agile     (1000)       38 2023-05-02 18:16:41.685139 smartsheet-pydantic-1.4.2/setup.cfg
-drwxrwxr-x   0 agile     (1000) agile     (1000)        0 2023-05-02 18:16:41.685139 smartsheet-pydantic-1.4.2/src/
-drwxrwxr-x   0 agile     (1000) agile     (1000)        0 2023-05-02 18:16:41.685139 smartsheet-pydantic-1.4.2/src/smartsheet_pydantic/
--rw-rw-r--   0 agile     (1000) agile     (1000)        0 2023-05-01 22:13:12.000000 smartsheet-pydantic-1.4.2/src/smartsheet_pydantic/__init__.py
--rw-rw-r--   0 agile     (1000) agile     (1000)     7617 2023-05-02 18:16:18.000000 smartsheet-pydantic-1.4.2/src/smartsheet_pydantic/controller.py
--rw-rw-r--   0 agile     (1000) agile     (1000)      493 2023-05-01 22:13:12.000000 smartsheet-pydantic-1.4.2/src/smartsheet_pydantic/debug_logger.py
--rw-rw-r--   0 agile     (1000) agile     (1000)     2816 2023-05-01 22:13:12.000000 smartsheet-pydantic-1.4.2/src/smartsheet_pydantic/filters.py
--rw-rw-r--   0 agile     (1000) agile     (1000)    12396 2023-05-01 22:13:12.000000 smartsheet-pydantic-1.4.2/src/smartsheet_pydantic/smartmodels.py
--rw-rw-r--   0 agile     (1000) agile     (1000)     3087 2023-05-01 22:53:34.000000 smartsheet-pydantic-1.4.2/src/smartsheet_pydantic/sources.py
--rw-rw-r--   0 agile     (1000) agile     (1000)     2329 2023-05-01 22:13:12.000000 smartsheet-pydantic-1.4.2/src/smartsheet_pydantic/transformer.py
-drwxrwxr-x   0 agile     (1000) agile     (1000)        0 2023-05-02 18:16:41.685139 smartsheet-pydantic-1.4.2/src/smartsheet_pydantic.egg-info/
--rw-rw-r--   0 agile     (1000) agile     (1000)     8575 2023-05-02 18:16:41.000000 smartsheet-pydantic-1.4.2/src/smartsheet_pydantic.egg-info/PKG-INFO
--rw-rw-r--   0 agile     (1000) agile     (1000)      622 2023-05-02 18:16:41.000000 smartsheet-pydantic-1.4.2/src/smartsheet_pydantic.egg-info/SOURCES.txt
--rw-rw-r--   0 agile     (1000) agile     (1000)        1 2023-05-02 18:16:41.000000 smartsheet-pydantic-1.4.2/src/smartsheet_pydantic.egg-info/dependency_links.txt
--rw-rw-r--   0 agile     (1000) agile     (1000)      102 2023-05-02 18:16:41.000000 smartsheet-pydantic-1.4.2/src/smartsheet_pydantic.egg-info/requires.txt
--rw-rw-r--   0 agile     (1000) agile     (1000)       20 2023-05-02 18:16:41.000000 smartsheet-pydantic-1.4.2/src/smartsheet_pydantic.egg-info/top_level.txt
-drwxrwxr-x   0 agile     (1000) agile     (1000)        0 2023-05-02 18:16:41.685139 smartsheet-pydantic-1.4.2/tests/
--rw-rw-r--   0 agile     (1000) agile     (1000)     4686 2023-05-01 22:13:12.000000 smartsheet-pydantic-1.4.2/tests/test_controller.py
--rw-rw-r--   0 agile     (1000) agile     (1000)     3527 2023-05-01 22:13:12.000000 smartsheet-pydantic-1.4.2/tests/test_filters.py
--rw-rw-r--   0 agile     (1000) agile     (1000)    13872 2023-05-01 22:13:12.000000 smartsheet-pydantic-1.4.2/tests/test_smartmodel.py
--rw-rw-r--   0 agile     (1000) agile     (1000)     1714 2023-05-01 22:13:12.000000 smartsheet-pydantic-1.4.2/tests/test_sources.py
+drwxrwxr-x   0 agile     (1000) agile     (1000)        0 2023-05-03 23:07:24.515820 smartsheet-pydantic-1.4.3/
+-rw-rw-r--   0 agile     (1000) agile     (1000)     1091 2023-05-01 22:13:12.000000 smartsheet-pydantic-1.4.3/LICENSE
+-rw-rw-r--   0 agile     (1000) agile     (1000)     8773 2023-05-03 23:07:24.515820 smartsheet-pydantic-1.4.3/PKG-INFO
+-rw-rw-r--   0 agile     (1000) agile     (1000)     7123 2023-05-03 23:07:07.000000 smartsheet-pydantic-1.4.3/README.md
+-rw-rw-r--   0 agile     (1000) agile     (1000)      811 2023-05-03 23:07:07.000000 smartsheet-pydantic-1.4.3/pyproject.toml
+-rw-rw-r--   0 agile     (1000) agile     (1000)       38 2023-05-03 23:07:24.515820 smartsheet-pydantic-1.4.3/setup.cfg
+drwxrwxr-x   0 agile     (1000) agile     (1000)        0 2023-05-03 23:07:24.507820 smartsheet-pydantic-1.4.3/src/
+drwxrwxr-x   0 agile     (1000) agile     (1000)        0 2023-05-03 23:07:24.511820 smartsheet-pydantic-1.4.3/src/smartsheet_pydantic/
+-rw-rw-r--   0 agile     (1000) agile     (1000)        0 2023-05-01 22:13:12.000000 smartsheet-pydantic-1.4.3/src/smartsheet_pydantic/__init__.py
+-rw-rw-r--   0 agile     (1000) agile     (1000)     7623 2023-05-03 23:07:07.000000 smartsheet-pydantic-1.4.3/src/smartsheet_pydantic/controller.py
+-rw-rw-r--   0 agile     (1000) agile     (1000)      493 2023-05-01 22:13:12.000000 smartsheet-pydantic-1.4.3/src/smartsheet_pydantic/debug_logger.py
+-rw-rw-r--   0 agile     (1000) agile     (1000)     2816 2023-05-01 22:13:12.000000 smartsheet-pydantic-1.4.3/src/smartsheet_pydantic/filters.py
+-rw-rw-r--   0 agile     (1000) agile     (1000)    12506 2023-05-03 23:07:07.000000 smartsheet-pydantic-1.4.3/src/smartsheet_pydantic/smartmodels.py
+-rw-rw-r--   0 agile     (1000) agile     (1000)     3087 2023-05-01 22:53:34.000000 smartsheet-pydantic-1.4.3/src/smartsheet_pydantic/sources.py
+-rw-rw-r--   0 agile     (1000) agile     (1000)     2329 2023-05-01 22:13:12.000000 smartsheet-pydantic-1.4.3/src/smartsheet_pydantic/transformer.py
+drwxrwxr-x   0 agile     (1000) agile     (1000)        0 2023-05-03 23:07:24.515820 smartsheet-pydantic-1.4.3/src/smartsheet_pydantic.egg-info/
+-rw-rw-r--   0 agile     (1000) agile     (1000)     8773 2023-05-03 23:07:24.000000 smartsheet-pydantic-1.4.3/src/smartsheet_pydantic.egg-info/PKG-INFO
+-rw-rw-r--   0 agile     (1000) agile     (1000)      622 2023-05-03 23:07:24.000000 smartsheet-pydantic-1.4.3/src/smartsheet_pydantic.egg-info/SOURCES.txt
+-rw-rw-r--   0 agile     (1000) agile     (1000)        1 2023-05-03 23:07:24.000000 smartsheet-pydantic-1.4.3/src/smartsheet_pydantic.egg-info/dependency_links.txt
+-rw-rw-r--   0 agile     (1000) agile     (1000)      102 2023-05-03 23:07:24.000000 smartsheet-pydantic-1.4.3/src/smartsheet_pydantic.egg-info/requires.txt
+-rw-rw-r--   0 agile     (1000) agile     (1000)       20 2023-05-03 23:07:24.000000 smartsheet-pydantic-1.4.3/src/smartsheet_pydantic.egg-info/top_level.txt
+drwxrwxr-x   0 agile     (1000) agile     (1000)        0 2023-05-03 23:07:24.515820 smartsheet-pydantic-1.4.3/tests/
+-rw-rw-r--   0 agile     (1000) agile     (1000)     6597 2023-05-03 23:07:07.000000 smartsheet-pydantic-1.4.3/tests/test_controller.py
+-rw-rw-r--   0 agile     (1000) agile     (1000)     3527 2023-05-01 22:13:12.000000 smartsheet-pydantic-1.4.3/tests/test_filters.py
+-rw-rw-r--   0 agile     (1000) agile     (1000)    14465 2023-05-03 23:07:07.000000 smartsheet-pydantic-1.4.3/tests/test_smartmodel.py
+-rw-rw-r--   0 agile     (1000) agile     (1000)     1714 2023-05-01 22:13:12.000000 smartsheet-pydantic-1.4.3/tests/test_sources.py
```

### Comparing `smartsheet-pydantic-1.4.2/LICENSE` & `smartsheet-pydantic-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `smartsheet-pydantic-1.4.2/PKG-INFO` & `smartsheet-pydantic-1.4.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartsheet-pydantic
-Version: 1.4.2
+Version: 1.4.3
 Summary: Smartsheet Python SDK and Pydantic Wrapper
 Author: Takahiro Watanabe
 License: The MIT License (MIT)
         Copyright © 2023 <copyright holders>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
@@ -58,33 +58,37 @@
 ## Defining the Controller
 
 In order to generate the Controller we will use the __SheetDetail__ class to collect the necessary details.
 
 1. __sheet_id__: Every Smartsheet grid has a unique id, this is used to target the Smartsheet.
 2. __description__: User defined description of the target Smartsheet to give some context. Can be anything.
 3. __smart_model__: A __smartsheet-pydantic__ model we will create to aid in data validation (Extension of Pydantic BaseModel).
-4. __source__: A __smartsheet-pydantic__ model we will create which contains the connection detail so data can be extracted from, and written into the target Smartsheet.
+4. __source__: default None. This field is used to override a Smartmodels default DataSource for unit testing purposes. Omit for normal use.
 
 ```python
-from smartsheet_pydantic import SheetDetail, SmartModel, DataSource
+from smartsheet_pydantic.controller import SheetDetail
+from smartsheet_pydantic.smartmodels import SmartModel
+from smartsheet_pydantic.sources import DataSource
 
 
 sheet_detail = SheetDetail(
     sheet_id: int = 0123456789
     description: str = "Description of the target Smartsheet"
     smart_model: SmartModel = WeatherModel # we will create this in the subsequent steps
-    source: DataSource = ExamplePostgres   # we will create this in the subsequent steps
 )
 ```
 
 ---
 ## Defining a DataSource
 There are options when creating a data source. One is a RESTful API endpoint, where the you can extend the __DataSourceAPI__ class, and provide a __url__ attribute. The other is a PostgreSQL database source using __DataSourcePostgres__, where you can provide the access details as well as the query to use, and the column name designations. We will use the latter in this example.
 
 ```python
+from smartsheet_pydantic.sources import DataSourceAPI, DataSourcePostgres
+
+
 # DataSource class to call a RESTful API endpoint.
 class WeatherRestAPI(DataSourceAPI):
     url = 'http://127.0.0.1:8000/weather_data'
 
 
 # DataSource class for PostgreSQL database
 class ExamplePostgres(DataSourcePostgres):
@@ -104,53 +108,54 @@
 
 You will also need to define 2 additional Configuration parameters.
 1. __source__: this is the DataSource class you defined in the previous step which is associated with this SmartModel.
 1. __unique_key__: is a list of column names which the model will use to define uniqueness. When data in Smartsheet is updated these columns will be used to find and update the data if the data already exists.
 2. __key_mapping__: if you have defined the data field names that differs from the source data, then this dictionary can be used to map and rename those columns. If the data field names are the same, the value must be set to None.
 
 ```python
+from smartsheet_pydantic.smartmodels import SmartModel
 from datetime import date
 
 
 class WeatherModel(SmartModel):
 
     index: int
     date: date
     temperature: float
     humidity: float
     rain: bool
 
     class Configuration
-        Source = WeatherRestAPI
+        source = WeatherRestAPI
         unique_columns: list[int] = ['index']
         key_mapping: dict = None
 ```
 
 ---
 
 ## Generating the controller
 Now that all of the components are ready we will now take the __SheetDetail__ instance, and provide it to the __SmartsheetControllerFactory__ class to generate a __ControllerFactory__. By calling on the __.get_controller()__ method we can generate the __SmarsheetController__ object.
 
 ```python
-from smartsheet_pydantic import SmartsheetControllerFactory
+from smartsheet_pydantic.controller import SmartsheetController, SmartsheetControllerFactory
 
 controller_factory = SmartsheetControllerFactory()
-controller = controller_factory.get_controller(sheet_detail)
+controller: SmartsheetController = controller_factory.get_controller(sheet_detail)
 ```
 
 ---
 
 ## Using the controller
 
 ### Use the provided data source to refresh the target Smartsheet
 ```python
 controller.refresh_smartsheet_from_source()
 ```
 
-### Extracting data from Smartsheet
+### Extracting data from Smartsheet into a list of SmartModel instances.
 ```python
 data: list[WeatherData] = controller.extract_as_smartmodel()
 ```
 
 ### Manually write new data, or update existing data to Smartsheet
 ```python
 data: list[WeatherData]
```

### Comparing `smartsheet-pydantic-1.4.2/README.md` & `smartsheet-pydantic-1.4.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -35,33 +35,37 @@
 ## Defining the Controller
 
 In order to generate the Controller we will use the __SheetDetail__ class to collect the necessary details.
 
 1. __sheet_id__: Every Smartsheet grid has a unique id, this is used to target the Smartsheet.
 2. __description__: User defined description of the target Smartsheet to give some context. Can be anything.
 3. __smart_model__: A __smartsheet-pydantic__ model we will create to aid in data validation (Extension of Pydantic BaseModel).
-4. __source__: A __smartsheet-pydantic__ model we will create which contains the connection detail so data can be extracted from, and written into the target Smartsheet.
+4. __source__: default None. This field is used to override a Smartmodels default DataSource for unit testing purposes. Omit for normal use.
 
 ```python
-from smartsheet_pydantic import SheetDetail, SmartModel, DataSource
+from smartsheet_pydantic.controller import SheetDetail
+from smartsheet_pydantic.smartmodels import SmartModel
+from smartsheet_pydantic.sources import DataSource
 
 
 sheet_detail = SheetDetail(
     sheet_id: int = 0123456789
     description: str = "Description of the target Smartsheet"
     smart_model: SmartModel = WeatherModel # we will create this in the subsequent steps
-    source: DataSource = ExamplePostgres   # we will create this in the subsequent steps
 )
 ```
 
 ---
 ## Defining a DataSource
 There are options when creating a data source. One is a RESTful API endpoint, where the you can extend the __DataSourceAPI__ class, and provide a __url__ attribute. The other is a PostgreSQL database source using __DataSourcePostgres__, where you can provide the access details as well as the query to use, and the column name designations. We will use the latter in this example.
 
 ```python
+from smartsheet_pydantic.sources import DataSourceAPI, DataSourcePostgres
+
+
 # DataSource class to call a RESTful API endpoint.
 class WeatherRestAPI(DataSourceAPI):
     url = 'http://127.0.0.1:8000/weather_data'
 
 
 # DataSource class for PostgreSQL database
 class ExamplePostgres(DataSourcePostgres):
@@ -81,53 +85,54 @@
 
 You will also need to define 2 additional Configuration parameters.
 1. __source__: this is the DataSource class you defined in the previous step which is associated with this SmartModel.
 1. __unique_key__: is a list of column names which the model will use to define uniqueness. When data in Smartsheet is updated these columns will be used to find and update the data if the data already exists.
 2. __key_mapping__: if you have defined the data field names that differs from the source data, then this dictionary can be used to map and rename those columns. If the data field names are the same, the value must be set to None.
 
 ```python
+from smartsheet_pydantic.smartmodels import SmartModel
 from datetime import date
 
 
 class WeatherModel(SmartModel):
 
     index: int
     date: date
     temperature: float
     humidity: float
     rain: bool
 
     class Configuration
-        Source = WeatherRestAPI
+        source = WeatherRestAPI
         unique_columns: list[int] = ['index']
         key_mapping: dict = None
 ```
 
 ---
 
 ## Generating the controller
 Now that all of the components are ready we will now take the __SheetDetail__ instance, and provide it to the __SmartsheetControllerFactory__ class to generate a __ControllerFactory__. By calling on the __.get_controller()__ method we can generate the __SmarsheetController__ object.
 
 ```python
-from smartsheet_pydantic import SmartsheetControllerFactory
+from smartsheet_pydantic.controller import SmartsheetController, SmartsheetControllerFactory
 
 controller_factory = SmartsheetControllerFactory()
-controller = controller_factory.get_controller(sheet_detail)
+controller: SmartsheetController = controller_factory.get_controller(sheet_detail)
 ```
 
 ---
 
 ## Using the controller
 
 ### Use the provided data source to refresh the target Smartsheet
 ```python
 controller.refresh_smartsheet_from_source()
 ```
 
-### Extracting data from Smartsheet
+### Extracting data from Smartsheet into a list of SmartModel instances.
 ```python
 data: list[WeatherData] = controller.extract_as_smartmodel()
 ```
 
 ### Manually write new data, or update existing data to Smartsheet
 ```python
 data: list[WeatherData]
```

### Comparing `smartsheet-pydantic-1.4.2/pyproject.toml` & `smartsheet-pydantic-1.4.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools>=67.7.1", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "smartsheet-pydantic"
-version = "1.4.2"
+version = "1.4.3"
 description = "Smartsheet Python SDK and Pydantic Wrapper"
 readme = "README.md"
 authors = [{ name = "Takahiro Watanabe" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `smartsheet-pydantic-1.4.2/src/smartsheet_pydantic/controller.py` & `smartsheet-pydantic-1.4.3/src/smartsheet_pydantic/controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         self.client = client
         self.sheet_id = sheet_detail['sheet_id']
         self.description = sheet_detail['description']
         self.smart_model = sheet_detail['smart_model']
 
         # give an option to override SmartModel's pre-defined source with a
         # user provided source for mock testing purposes only.
-        if sheet_detail.get('source'):
+        if sheet_detail.get('source', None):
             self.source = sheet_detail['source']
         else:
             self.source = self.smart_model.Configuration.source
 
         self.unique_columns = self.smart_model.Configuration.unique_columns
         self.sheet = self._set_sheet(client, self.sheet_id)
```

### Comparing `smartsheet-pydantic-1.4.2/src/smartsheet_pydantic/filters.py` & `smartsheet-pydantic-1.4.3/src/smartsheet_pydantic/filters.py`

 * *Files identical despite different names*

### Comparing `smartsheet-pydantic-1.4.2/src/smartsheet_pydantic/smartmodels.py` & `smartsheet-pydantic-1.4.3/src/smartsheet_pydantic/smartmodels.py`

 * *Files 4% similar despite different names*

```diff
@@ -292,18 +292,19 @@
             __validators__=validators
         )
         return model(**data)
 
     def __lt__(self, other):
         keys: list[str] = self.Configuration.unique_columns
         for key in keys:
-            if self[key] == other[key]:
+            if getattr(self, key) == getattr(other, key):
+                print(getattr(self, key), getattr(other, key))
                 continue
             else:
-                self[key] <= other[key]
+                return getattr(self, key) < getattr(other, key)
 
     def __eq__(self, other):
         return self.__hash__() == other.__hash__()
 
     def __hash__(self):
         """
         Utilize all fields except the row_id to create a unique hash for the
@@ -315,14 +316,15 @@
         trimmed_key: list[str] = [key for key in full_key if key != 'row_id']
         values: list[str] = [
             str(getattr(self, field_name))
             for field_name in trimmed_key
         ]
         values.sort()  # values may come back in various orders from Smartsheet
         return hash("".join(values))
+    
 
     @classmethod
     def identify_incoming_differences(
                 cls,
                 existing_data: set[SmartModel],
                 incoming_data: set[SmartModel]
             ) -> set[SmartModel]:
```

### Comparing `smartsheet-pydantic-1.4.2/src/smartsheet_pydantic/sources.py` & `smartsheet-pydantic-1.4.3/src/smartsheet_pydantic/sources.py`

 * *Files identical despite different names*

### Comparing `smartsheet-pydantic-1.4.2/src/smartsheet_pydantic/transformer.py` & `smartsheet-pydantic-1.4.3/src/smartsheet_pydantic/transformer.py`

 * *Files identical despite different names*

### Comparing `smartsheet-pydantic-1.4.2/src/smartsheet_pydantic.egg-info/PKG-INFO` & `smartsheet-pydantic-1.4.3/src/smartsheet_pydantic.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartsheet-pydantic
-Version: 1.4.2
+Version: 1.4.3
 Summary: Smartsheet Python SDK and Pydantic Wrapper
 Author: Takahiro Watanabe
 License: The MIT License (MIT)
         Copyright © 2023 <copyright holders>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
@@ -58,33 +58,37 @@
 ## Defining the Controller
 
 In order to generate the Controller we will use the __SheetDetail__ class to collect the necessary details.
 
 1. __sheet_id__: Every Smartsheet grid has a unique id, this is used to target the Smartsheet.
 2. __description__: User defined description of the target Smartsheet to give some context. Can be anything.
 3. __smart_model__: A __smartsheet-pydantic__ model we will create to aid in data validation (Extension of Pydantic BaseModel).
-4. __source__: A __smartsheet-pydantic__ model we will create which contains the connection detail so data can be extracted from, and written into the target Smartsheet.
+4. __source__: default None. This field is used to override a Smartmodels default DataSource for unit testing purposes. Omit for normal use.
 
 ```python
-from smartsheet_pydantic import SheetDetail, SmartModel, DataSource
+from smartsheet_pydantic.controller import SheetDetail
+from smartsheet_pydantic.smartmodels import SmartModel
+from smartsheet_pydantic.sources import DataSource
 
 
 sheet_detail = SheetDetail(
     sheet_id: int = 0123456789
     description: str = "Description of the target Smartsheet"
     smart_model: SmartModel = WeatherModel # we will create this in the subsequent steps
-    source: DataSource = ExamplePostgres   # we will create this in the subsequent steps
 )
 ```
 
 ---
 ## Defining a DataSource
 There are options when creating a data source. One is a RESTful API endpoint, where the you can extend the __DataSourceAPI__ class, and provide a __url__ attribute. The other is a PostgreSQL database source using __DataSourcePostgres__, where you can provide the access details as well as the query to use, and the column name designations. We will use the latter in this example.
 
 ```python
+from smartsheet_pydantic.sources import DataSourceAPI, DataSourcePostgres
+
+
 # DataSource class to call a RESTful API endpoint.
 class WeatherRestAPI(DataSourceAPI):
     url = 'http://127.0.0.1:8000/weather_data'
 
 
 # DataSource class for PostgreSQL database
 class ExamplePostgres(DataSourcePostgres):
@@ -104,53 +108,54 @@
 
 You will also need to define 2 additional Configuration parameters.
 1. __source__: this is the DataSource class you defined in the previous step which is associated with this SmartModel.
 1. __unique_key__: is a list of column names which the model will use to define uniqueness. When data in Smartsheet is updated these columns will be used to find and update the data if the data already exists.
 2. __key_mapping__: if you have defined the data field names that differs from the source data, then this dictionary can be used to map and rename those columns. If the data field names are the same, the value must be set to None.
 
 ```python
+from smartsheet_pydantic.smartmodels import SmartModel
 from datetime import date
 
 
 class WeatherModel(SmartModel):
 
     index: int
     date: date
     temperature: float
     humidity: float
     rain: bool
 
     class Configuration
-        Source = WeatherRestAPI
+        source = WeatherRestAPI
         unique_columns: list[int] = ['index']
         key_mapping: dict = None
 ```
 
 ---
 
 ## Generating the controller
 Now that all of the components are ready we will now take the __SheetDetail__ instance, and provide it to the __SmartsheetControllerFactory__ class to generate a __ControllerFactory__. By calling on the __.get_controller()__ method we can generate the __SmarsheetController__ object.
 
 ```python
-from smartsheet_pydantic import SmartsheetControllerFactory
+from smartsheet_pydantic.controller import SmartsheetController, SmartsheetControllerFactory
 
 controller_factory = SmartsheetControllerFactory()
-controller = controller_factory.get_controller(sheet_detail)
+controller: SmartsheetController = controller_factory.get_controller(sheet_detail)
 ```
 
 ---
 
 ## Using the controller
 
 ### Use the provided data source to refresh the target Smartsheet
 ```python
 controller.refresh_smartsheet_from_source()
 ```
 
-### Extracting data from Smartsheet
+### Extracting data from Smartsheet into a list of SmartModel instances.
 ```python
 data: list[WeatherData] = controller.extract_as_smartmodel()
 ```
 
 ### Manually write new data, or update existing data to Smartsheet
 ```python
 data: list[WeatherData]
```

### Comparing `smartsheet-pydantic-1.4.2/src/smartsheet_pydantic.egg-info/SOURCES.txt` & `smartsheet-pydantic-1.4.3/src/smartsheet_pydantic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `smartsheet-pydantic-1.4.2/tests/test_filters.py` & `smartsheet-pydantic-1.4.3/tests/test_filters.py`

 * *Files identical despite different names*

### Comparing `smartsheet-pydantic-1.4.2/tests/test_smartmodel.py` & `smartsheet-pydantic-1.4.3/tests/test_smartmodel.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from copy import deepcopy
 from datetime import date, datetime
-from pydantic import ValidationError
 import pytest
 
 from tests.factories.mock_smartmodel import \
     MockSmartModel, MockSmartModelWithNone
 from tests.factories.mock_source import MockSource
 
 
@@ -430,7 +429,26 @@
         existing_data=set(existing_models),
         incoming_data=set(existing_models_with_new)
     )
     existing = existing_vs_new['existing']
     new = existing_vs_new['new']
     assert existing == set(existing_models)
     assert new == set(addition)
+
+
+def test_smartmodel_sort():
+    """
+    Smartmodel has a custom __lt__ method, based upon user defined unique
+    columns. Test that the unique columns are used properly to sort the
+    SmartModels.
+    """
+
+    dataset = MockSource().get()
+    dataset_shuffled = [dataset[2], dataset[0], dataset[1]]
+    models: list[MockSmartModel] = [
+        MockSmartModel.from_source(data) for data
+        in dataset_shuffled
+    ]
+    models.sort()
+    assert models[0] == MockSmartModel.from_source(dataset[0])
+    assert models[1] == MockSmartModel.from_source(dataset[1])
+    assert models[2] == MockSmartModel.from_source(dataset[2])
```

### Comparing `smartsheet-pydantic-1.4.2/tests/test_sources.py` & `smartsheet-pydantic-1.4.3/tests/test_sources.py`

 * *Files identical despite different names*

