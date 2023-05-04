# Comparing `tmp/iosense_connect-2.1.0.tar.gz` & `tmp/iosense_connect-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\iosense_connect-2.1.0.tar", last modified: Wed Apr 19 09:43:56 2023, max compression
+gzip compressed data, was "dist\iosense_connect-2.1.1.tar", last modified: Thu May  4 07:23:40 2023, max compression
```

## Comparing `iosense_connect-2.1.0.tar` & `iosense_connect-2.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 09:43:56.005913 iosense_connect-2.1.0/
--rw-rw-rw-   0        0        0     1087 2023-04-18 04:21:30.000000 iosense_connect-2.1.0/LICENSE.txt
--rw-rw-rw-   0        0        0     1046 2023-04-19 09:43:56.003913 iosense_connect-2.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      674 2023-04-15 12:45:17.000000 iosense_connect-2.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-19 09:43:55.936887 iosense_connect-2.1.0/iosense_connect/
--rw-rw-rw-   0        0        0       37 2023-03-23 09:15:17.000000 iosense_connect-2.1.0/iosense_connect/__init__.py
--rw-rw-rw-   0        0        0    19815 2023-04-19 09:43:47.000000 iosense_connect-2.1.0/iosense_connect/data_access.py
-drwxrwxrwx   0        0        0        0 2023-04-19 09:43:55.991814 iosense_connect-2.1.0/iosense_connect.egg-info/
--rw-rw-rw-   0        0        0     1046 2023-04-19 09:43:55.000000 iosense_connect-2.1.0/iosense_connect.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      245 2023-04-19 09:43:55.000000 iosense_connect-2.1.0/iosense_connect.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 09:43:55.000000 iosense_connect-2.1.0/iosense_connect.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-04-19 09:43:55.000000 iosense_connect-2.1.0/iosense_connect.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-19 09:43:56.006916 iosense_connect-2.1.0/setup.cfg
--rw-rw-rw-   0        0        0      612 2023-04-19 09:43:47.000000 iosense_connect-2.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 07:23:40.056099 iosense_connect-2.1.1/
+-rw-rw-rw-   0        0        0     1087 2023-04-28 09:03:25.000000 iosense_connect-2.1.1/LICENSE.txt
+-rw-rw-rw-   0        0        0     1062 2023-05-04 07:23:40.056099 iosense_connect-2.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      690 2023-04-28 09:03:25.000000 iosense_connect-2.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-04 07:23:40.009220 iosense_connect-2.1.1/iosense_connect/
+-rw-rw-rw-   0        0        0       37 2023-03-23 09:15:17.000000 iosense_connect-2.1.1/iosense_connect/__init__.py
+-rw-rw-rw-   0        0        0    19576 2023-05-04 07:23:32.000000 iosense_connect-2.1.1/iosense_connect/data_access.py
+drwxrwxrwx   0        0        0        0 2023-05-04 07:23:40.056099 iosense_connect-2.1.1/iosense_connect.egg-info/
+-rw-rw-rw-   0        0        0     1062 2023-05-04 07:23:39.000000 iosense_connect-2.1.1/iosense_connect.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      245 2023-05-04 07:23:39.000000 iosense_connect-2.1.1/iosense_connect.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 07:23:39.000000 iosense_connect-2.1.1/iosense_connect.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-05-04 07:23:39.000000 iosense_connect-2.1.1/iosense_connect.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-04 07:23:40.056099 iosense_connect-2.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      614 2023-05-04 07:23:31.000000 iosense_connect-2.1.1/setup.py
```

### Comparing `iosense_connect-2.1.0/LICENSE.txt` & `iosense_connect-2.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `iosense_connect-2.1.0/PKG-INFO` & `iosense_connect-2.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iosense_connect
-Version: 2.1.0
+Version: 2.1.1
 Summary: iosense connect library
 Author: Faclon-Labs
 Author-email: reachus@faclon.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -14,17 +14,17 @@
 ### Project description
 Faclon I/O Sense Data Access Library
 ​
 #### Where to get it
 https://pypi.org/project/iosense/
 
 #### Installation
-pip install iosense
+pip install iosense-connect
 
-pip3 install iosense
+pip3 install iosense-connect
 
 #### Features
 Retrives following details:
 
 - User information.
 - Device Details.
 - Device metaData.
```

### Comparing `iosense_connect-2.1.0/README.md` & `iosense_connect-2.1.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 ### Project description
 Faclon I/O Sense Data Access Library
 ​
 #### Where to get it
 https://pypi.org/project/iosense/
 
 #### Installation
-pip install iosense
+pip install iosense-connect
 
-pip3 install iosense
+pip3 install iosense-connect
 
 #### Features
 Retrives following details:
 
 - User information.
 - Device Details.
 - Device metaData.
```

### Comparing `iosense_connect-2.1.0/iosense_connect/data_access.py` & `iosense_connect-2.1.1/iosense_connect/data_access.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,15 +63,14 @@
 
         sensor_spec = 'sensors'
         sensor_param_df = pd.DataFrame(raw_metadata[sensor_spec])
 
         for i in list1:
             sensor_param_df1 = sensor_param_df[sensor_param_df['sensorId'] == i]
             if len(sensor_param_df1) != 0:
-                # print('sensor_param_df',sensor_param_df1)
                 sensor_name = sensor_param_df1.iloc[0]['sensorName']
                 sensor_name = sensor_name + " (" + i + ")"
                 df['sensor'] = df['sensor'].replace(i, sensor_name)
         return df, raw_metadata
 
     def get_caliberation(self, device_id, metadata, df):
         """
@@ -84,38 +83,34 @@
              y = mx + c
              if y is greater than max value replace y with max value
              if y is less than min value replace y with min value
 
         """
         sensor_name_list = list(df.columns)
         sensor_name_list.remove('time')
-        # print(sensor_name_list)
-        sensor_id_list = [s[s.rfind("(") + 1:s.rfind(")")] for s in sensor_name_list]
+
+        if "(" not in sensor_name_list[0]:
+            sensor_id_list = sensor_name_list
+        else:
+            sensor_id_list = [s[s.rfind("(") + 1:s.rfind(")")] for s in sensor_name_list]
+
         if len(metadata) == 0:
             metadata = DataAccess.get_device_metadata(self, device_id)
         data = metadata['params']
 
         for (value1, value2) in zip(sensor_id_list, sensor_name_list):
-            # print(value1, value2)
-            # print(data[str(value1)])
             df_meta = pd.DataFrame(data[str(value1)])
-            # print(df_meta)
             df_meta = df_meta.set_index('paramName').transpose()
-            # print(df_meta)
+
             if 'm' in df_meta.columns and 'c' in df_meta.columns:
-                # print(df_meta.iloc[0]['m'],type(df_meta.iloc[0]['m']))
                 m = float(df_meta.iloc[0]['m'])
-                # print('M value',m)
                 c = int(df_meta.iloc[0]['c'])
-                # print(m, type(c))
-                # print(df[str(value2)])
                 df[str(value2)] = df[str(value2)].replace('BAD 255', '-99999').replace('-', '99999').replace(
                     'BAD undefined', '-99999').replace('BAD 0', '-99999')
                 df[str(value2)] = df[str(value2)].astype('float')
-                # print('==',df[str(value2)])
                 df[str(value2)] = (df[str(value2)] * m) + c
                 if 'min' in df_meta.columns:
                     min = int(df_meta.iloc[0]['min'])
                     df[str(value2)] = np.where(df[str(value2)] <= min, min, df[str(value2)])
                 if 'max' in df_meta.columns:
                     max = int(str(df_meta.iloc[0]['max']).replace('-', '99999').replace(
                         '1000000000000000000000000000', '99999').replace('100000000000', '99999'))
@@ -205,15 +200,15 @@
                 raw_data = json.loads(response.text)['data']
                 return raw_data
 
         except Exception as e:
             print('Failed to fetch user Information')
             print(e)
 
-    def get_dp(self, device_id, sensors, n=1, cal=True, end_time=datetime.now(), IST=True):
+    def get_dp(self, device_id, sensors, n=1, cal=True, alias=True, end_time=datetime.now(), IST=True):
         """
 
         :param device_id: string
         :param sensors: list of sensors
         :param n: number of data points (default: 1)
         :param cal: bool (default: True)
         :param end_time: 'YYYY:MM:DD HH:MM:SS'
@@ -266,28 +261,30 @@
                     raw_data = json.loads(response.text)['data']
                     cursor = json.loads(response.text)['cursor']
                     if len(raw_data) != 0:
                         df = pd.concat([df, pd.DataFrame(raw_data)])
                     counter = counter + 1
                 if cursor['end'] == None:
                     break
-            if len(df) == 0:
-                raise ValueError('No Data')
-            if IST:
-                df['time'] = pd.to_datetime(df['time'], utc=False)
-                df['time'] = df['time'].dt.tz_convert('Asia/Kolkata').dt.tz_localize(None)
-            df, metadata = DataAccess.get_sensor_alias(self, device_id, df, metadata)
-            df = DataAccess.get_cleaned_table(self, df)
-            if str(cal).lower() == 'true':
-                df = DataAccess.get_caliberation(self, device_id, metadata, df)
+            if len(df) != 0:
+                if IST:
+                    df['time'] = pd.to_datetime(df['time'], utc=False)
+                    df['time'] = df['time'].dt.tz_convert('Asia/Kolkata').dt.tz_localize(None)
+                if str(alias).lower() == "true":
+                    df, metadata = DataAccess.get_sensor_alias(self, device_id, df, metadata)
+                df, metadata = DataAccess.get_sensor_alias(self, device_id, df, metadata)
+                df = DataAccess.get_cleaned_table(self, df)
+                if str(cal).lower() == 'true':
+                    df = DataAccess.get_caliberation(self, device_id, metadata, df)
             return df
         except Exception as e:
             print(e)
 
-    def data_query(self, device_id, start_time, end_time=datetime.now(), sensors=None, cal=True, bands=None, IST=True,
+    def data_query(self, device_id, start_time, end_time=datetime.now(), sensors=None, alias=True, cal=True, bands=None,
+                   IST=True,
                    echo=True):
         # df = pd.DataFrame()
         df_devices = DataAccess.get_device_details(self)
         device_list = df_devices['devID'].tolist()
         if device_id not in device_list:
             raise Exception('Message: Device not added')
         metadata = {}
@@ -342,40 +339,38 @@
                     str1 = ","
                     sensor_values = str1.join(sensors)
                     temp = url_api + device_id + "&sensor=" + sensor_values + "&sTime=" + str(
                         cursor['start']) + "&eTime=" + str(cursor['end']) + "&cursor=true&limit=50000"
 
             response = requests.request("GET", temp, headers=header, data=payload)
             raw = json.loads(response.text)
-            # print(raw)
             if response.status_code != 200:
                 raise ValueError(raw)
             if 'success' in raw:
                 raise ValueError(raw)
 
             else:
                 raw_data = json.loads(response.text)['data']
-                # print('====================',raw_data)
                 cursor = json.loads(response.text)['cursor']
                 if len(raw_data) != 0:
                     rawdata_res = rawdata_res + raw_data
                 counter = counter + 1
             if cursor['start'] is None or cursor['end'] is None:
                 break
-        # print(rawdata_res)
         df_raw = pd.DataFrame(rawdata_res)
 
         if len(df_raw) != 0:
             if IST:
                 df_raw['time'] = pd.to_datetime(df_raw['time'], utc=False)
                 df_raw['time'] = df_raw['time'].dt.tz_convert('Asia/Kolkata').dt.tz_localize(None)
             if len(df_raw.columns) == 2:
                 df_raw['sensor'] = sensors[0]
-            df, metadata = DataAccess.get_sensor_alias(self, device_id, df_raw, metadata)
-            df = DataAccess.get_cleaned_table(self, df)
+            if str(alias).lower() == "true":
+                df_raw, metadata = DataAccess.get_sensor_alias(self, device_id, df_raw, metadata)
+            df = DataAccess.get_cleaned_table(self, df_raw)
             if str(cal).lower() == 'true':
                 df = DataAccess.get_caliberation(self, device_id, metadata, df)
             if bands is not None:
                 df = DataAccess.time_grouping(self, df, bands)
         else:
             df = df_raw
         return df
```

### Comparing `iosense_connect-2.1.0/iosense_connect.egg-info/PKG-INFO` & `iosense_connect-2.1.1/iosense_connect.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iosense-connect
-Version: 2.1.0
+Version: 2.1.1
 Summary: iosense connect library
 Author: Faclon-Labs
 Author-email: reachus@faclon.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -14,17 +14,17 @@
 ### Project description
 Faclon I/O Sense Data Access Library
 ​
 #### Where to get it
 https://pypi.org/project/iosense/
 
 #### Installation
-pip install iosense
+pip install iosense-connect
 
-pip3 install iosense
+pip3 install iosense-connect
 
 #### Features
 Retrives following details:
 
 - User information.
 - Device Details.
 - Device metaData.
```

### Comparing `iosense_connect-2.1.0/setup.py` & `iosense_connect-2.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import setuptools
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "iosense_connect",
-    version = "2.1.0",
+    version = "2.1.1",
     author = "Faclon-Labs",
     author_email = "reachus@faclon.com",
     description = "iosense connect library",
     packages = ["iosense_connect"],
     long_description = long_description,
     long_description_content_type = "text/markdown",
     classifiers = [
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ]
-)
+)
```

