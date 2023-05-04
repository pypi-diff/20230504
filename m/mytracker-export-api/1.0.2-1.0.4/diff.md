# Comparing `tmp/mytracker_export_api-1.0.2.tar.gz` & `tmp/mytracker_export_api-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mytracker_export_api-1.0.2.tar", last modified: Mon Jan 23 14:16:53 2023, max compression
+gzip compressed data, was "mytracker_export_api-1.0.4.tar", last modified: Thu May  4 13:26:51 2023, max compression
```

## Comparing `mytracker_export_api-1.0.2.tar` & `mytracker_export_api-1.0.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 a.novopolsky   (503) staff       (20)        0 2023-01-23 14:16:53.609394 mytracker_export_api-1.0.2/
--rw-r--r--   0 a.novopolsky   (503) staff       (20)     1835 2022-06-29 14:57:53.000000 mytracker_export_api-1.0.2/.gitignore
--rw-r--r--   0 a.novopolsky   (503) staff       (20)     1063 2022-06-29 14:57:53.000000 mytracker_export_api-1.0.2/LICENSE
--rw-r--r--   0 a.novopolsky   (503) staff       (20)     1341 2023-01-23 14:16:53.609079 mytracker_export_api-1.0.2/PKG-INFO
--rw-r--r--   0 a.novopolsky   (503) staff       (20)      857 2022-07-01 13:49:40.000000 mytracker_export_api-1.0.2/README.md
-drwxr-xr-x   0 a.novopolsky   (503) staff       (20)        0 2023-01-23 14:16:53.599724 mytracker_export_api-1.0.2/examples/
--rw-r--r--   0 a.novopolsky   (503) staff       (20)     6778 2022-07-01 11:29:52.000000 mytracker_export_api-1.0.2/examples/raw_data.ipynb
--rw-r--r--   0 a.novopolsky   (503) staff       (20)     5503 2022-07-01 11:30:17.000000 mytracker_export_api-1.0.2/examples/report.ipynb
--rw-r--r--   0 a.novopolsky   (503) staff       (20)     1863 2022-06-29 15:28:06.000000 mytracker_export_api-1.0.2/examples/segment.ipynb
-drwxr-xr-x   0 a.novopolsky   (503) staff       (20)        0 2023-01-23 14:16:53.603331 mytracker_export_api-1.0.2/mytracker_export_api/
--rw-r--r--   0 a.novopolsky   (503) staff       (20)       72 2022-06-29 14:57:53.000000 mytracker_export_api-1.0.2/mytracker_export_api/__init__.py
--rw-r--r--   0 a.novopolsky   (503) staff       (20)       42 2022-06-29 14:57:53.000000 mytracker_export_api-1.0.2/mytracker_export_api/exceptions.py
--rw-r--r--   0 a.novopolsky   (503) staff       (20)    16244 2023-01-23 14:04:08.000000 mytracker_export_api-1.0.2/mytracker_export_api/mytracker.py
-drwxr-xr-x   0 a.novopolsky   (503) staff       (20)        0 2023-01-23 14:16:53.608578 mytracker_export_api-1.0.2/mytracker_export_api.egg-info/
--rw-r--r--   0 a.novopolsky   (503) staff       (20)     1341 2023-01-23 14:16:53.000000 mytracker_export_api-1.0.2/mytracker_export_api.egg-info/PKG-INFO
--rw-r--r--   0 a.novopolsky   (503) staff       (20)      487 2023-01-23 14:16:53.000000 mytracker_export_api-1.0.2/mytracker_export_api.egg-info/SOURCES.txt
--rw-r--r--   0 a.novopolsky   (503) staff       (20)        1 2023-01-23 14:16:53.000000 mytracker_export_api-1.0.2/mytracker_export_api.egg-info/dependency_links.txt
--rw-r--r--   0 a.novopolsky   (503) staff       (20)        1 2023-01-23 14:16:53.000000 mytracker_export_api-1.0.2/mytracker_export_api.egg-info/not-zip-safe
--rw-r--r--   0 a.novopolsky   (503) staff       (20)       31 2023-01-23 14:16:53.000000 mytracker_export_api-1.0.2/mytracker_export_api.egg-info/requires.txt
--rw-r--r--   0 a.novopolsky   (503) staff       (20)       21 2023-01-23 14:16:53.000000 mytracker_export_api-1.0.2/mytracker_export_api.egg-info/top_level.txt
--rw-r--r--   0 a.novopolsky   (503) staff       (20)       31 2022-08-25 14:45:19.000000 mytracker_export_api-1.0.2/requirements.txt
--rw-r--r--   0 a.novopolsky   (503) staff       (20)       38 2023-01-23 14:16:53.609508 mytracker_export_api-1.0.2/setup.cfg
--rw-r--r--   0 a.novopolsky   (503) staff       (20)      703 2023-01-23 11:11:22.000000 mytracker_export_api-1.0.2/setup.py
+drwxr-xr-x   0 a.novopolsky   (503) staff       (20)        0 2023-05-04 13:26:51.961665 mytracker_export_api-1.0.4/
+-rw-r--r--   0 a.novopolsky   (503) staff       (20)     1835 2022-06-29 14:57:53.000000 mytracker_export_api-1.0.4/.gitignore
+-rw-r--r--   0 a.novopolsky   (503) staff       (20)     1063 2022-06-29 14:57:53.000000 mytracker_export_api-1.0.4/LICENSE
+-rw-r--r--   0 a.novopolsky   (503) staff       (20)     1341 2023-05-04 13:26:51.961084 mytracker_export_api-1.0.4/PKG-INFO
+-rw-r--r--   0 a.novopolsky   (503) staff       (20)      857 2022-07-01 13:49:40.000000 mytracker_export_api-1.0.4/README.md
+drwxr-xr-x   0 a.novopolsky   (503) staff       (20)        0 2023-05-04 13:26:51.951412 mytracker_export_api-1.0.4/examples/
+-rw-r--r--   0 a.novopolsky   (503) staff       (20)     6778 2022-07-01 11:29:52.000000 mytracker_export_api-1.0.4/examples/raw_data.ipynb
+-rw-r--r--   0 a.novopolsky   (503) staff       (20)     5503 2023-04-26 15:54:56.000000 mytracker_export_api-1.0.4/examples/report.ipynb
+-rw-r--r--   0 a.novopolsky   (503) staff       (20)     1863 2022-06-29 15:28:06.000000 mytracker_export_api-1.0.4/examples/segment.ipynb
+drwxr-xr-x   0 a.novopolsky   (503) staff       (20)        0 2023-05-04 13:26:51.954400 mytracker_export_api-1.0.4/mytracker_export_api/
+-rw-r--r--   0 a.novopolsky   (503) staff       (20)       72 2022-06-29 14:57:53.000000 mytracker_export_api-1.0.4/mytracker_export_api/__init__.py
+-rw-r--r--   0 a.novopolsky   (503) staff       (20)       42 2022-06-29 14:57:53.000000 mytracker_export_api-1.0.4/mytracker_export_api/exceptions.py
+-rw-r--r--   0 a.novopolsky   (503) staff       (20)    15826 2023-05-04 13:16:12.000000 mytracker_export_api-1.0.4/mytracker_export_api/mytracker.py
+drwxr-xr-x   0 a.novopolsky   (503) staff       (20)        0 2023-05-04 13:26:51.960313 mytracker_export_api-1.0.4/mytracker_export_api.egg-info/
+-rw-r--r--   0 a.novopolsky   (503) staff       (20)     1341 2023-05-04 13:26:51.000000 mytracker_export_api-1.0.4/mytracker_export_api.egg-info/PKG-INFO
+-rw-r--r--   0 a.novopolsky   (503) staff       (20)      487 2023-05-04 13:26:51.000000 mytracker_export_api-1.0.4/mytracker_export_api.egg-info/SOURCES.txt
+-rw-r--r--   0 a.novopolsky   (503) staff       (20)        1 2023-05-04 13:26:51.000000 mytracker_export_api-1.0.4/mytracker_export_api.egg-info/dependency_links.txt
+-rw-r--r--   0 a.novopolsky   (503) staff       (20)        1 2023-05-04 13:26:51.000000 mytracker_export_api-1.0.4/mytracker_export_api.egg-info/not-zip-safe
+-rw-r--r--   0 a.novopolsky   (503) staff       (20)       47 2023-05-04 13:26:51.000000 mytracker_export_api-1.0.4/mytracker_export_api.egg-info/requires.txt
+-rw-r--r--   0 a.novopolsky   (503) staff       (20)       21 2023-05-04 13:26:51.000000 mytracker_export_api-1.0.4/mytracker_export_api.egg-info/top_level.txt
+-rw-r--r--   0 a.novopolsky   (503) staff       (20)       47 2023-05-04 12:53:06.000000 mytracker_export_api-1.0.4/requirements.txt
+-rw-r--r--   0 a.novopolsky   (503) staff       (20)       38 2023-05-04 13:26:51.961943 mytracker_export_api-1.0.4/setup.cfg
+-rw-r--r--   0 a.novopolsky   (503) staff       (20)      703 2023-05-04 13:26:22.000000 mytracker_export_api-1.0.4/setup.py
```

### Comparing `mytracker_export_api-1.0.2/.gitignore` & `mytracker_export_api-1.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `mytracker_export_api-1.0.2/LICENSE` & `mytracker_export_api-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mytracker_export_api-1.0.2/PKG-INFO` & `mytracker_export_api-1.0.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mytracker_export_api
-Version: 1.0.2
+Version: 1.0.4
 Summary: Python wrapper for MyTracker Export API.
 Home-page: UNKNOWN
 Author: Artyom Novopolsky
 Author-email: a.novopolsky@corp.mail.ru
 License: UNKNOWN
 Project-URL: Documentation, https://tracker.my.com/docs/api/export-api/about
 Project-URL: Source, https://github.com/tracker-my-com/mytracker-export-api-python
```

### Comparing `mytracker_export_api-1.0.2/README.md` & `mytracker_export_api-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `mytracker_export_api-1.0.2/examples/raw_data.ipynb` & `mytracker_export_api-1.0.4/examples/raw_data.ipynb`

 * *Files identical despite different names*

### Comparing `mytracker_export_api-1.0.2/examples/report.ipynb` & `mytracker_export_api-1.0.4/examples/report.ipynb`

 * *Files identical despite different names*

### Comparing `mytracker_export_api-1.0.2/examples/segment.ipynb` & `mytracker_export_api-1.0.4/examples/segment.ipynb`

 * *Files identical despite different names*

### Comparing `mytracker_export_api-1.0.2/mytracker_export_api/mytracker.py` & `mytracker_export_api-1.0.4/mytracker_export_api/mytracker.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,209 +1,214 @@
+import io
 import hashlib
 import hmac
 import base64
 import time
+import warnings
 import requests
 import pandas as pd
-from binascii import b2a_base64
 from urllib.parse import urlencode, quote_plus
-from urllib.request import ProxyHandler, build_opener, install_opener, urlopen 
+from urllib3.exceptions import InsecureRequestWarning
 from .exceptions import MyTrackerError
 
 
 class MyTracker:
-    
     METHOD_GET = 'GET'
     METHOD_POST = 'POST'
-    
+
     CREATE_RAW_DATA_URL = 'https://tracker.my.com/api/raw/v1/export/create.json'
     GET_RAW_DATA_URL = 'https://tracker.my.com/api/raw/v1/export/get.json'
     CANCEL_RAW_DATA_URL = 'https://tracker.my.com/api/raw/v1/export/cancel.json'
-    
+
     CREATE_REPORT_URL = 'https://tracker.my.com/api/report/v1/file/create.json'
     GET_REPORT_URL = 'https://tracker.my.com/api/report/v1/file/get.json'
-    
+
     CREATE_SEGMENT_URL = 'https://tracker.my.com/api/segment/v1/export/create.json'
     GET_SEGMENT_URL = 'https://tracker.my.com/api/segment/v1/export/get.json'
-    
-    
-    def __init__(self, api_user_id, api_secret_key, proxies=None):
-        '''
-        MyTracker class initialization. 
+
+    def __init__(self, api_user_id, api_secret_key, proxies=None, ssl_verify=True):
+        """
+        MyTracker class initialization.
 
         -----------
         Parameters:
             api_user_id (int): API User ID
             api_secret_key (str): API Secret Key
             proxies (dict, optional): dictionary mapping protocol to the URL of the proxy
+            ssl_verify (bool, optional): SSL/TLS certificate check flag
 
         Example:
             proxies = {
                'http': 'http://proxy.example.com:8080',
                'https': 'http://secureproxy.example.com:8090',
             }
-        '''
-        
+        """
+
         self.api_user_id = api_user_id
         self.api_secret_key = api_secret_key
         self.proxies = proxies
-    
+        self.ssl_verify = ssl_verify
+
     def _get_signature(self, url, method, data='') -> str:
-        ''' Getting a signature. '''
-        
+        """ Getting a signature. """
+
         base_string = '&'.join([method.upper(), quote_plus(url, safe='~'), quote_plus(data, safe='~')])
-        signature = base64.b64encode(hmac.new(bytes(self.api_secret_key, 'UTF-8'), 
-                                              bytes(base_string, 'UTF-8'), 
+        signature = base64.b64encode(hmac.new(bytes(self.api_secret_key, 'UTF-8'),
+                                              bytes(base_string, 'UTF-8'),
                                               hashlib.sha1).digest())
         signature = str(signature, 'UTF-8').rstrip('\n')
         return f'AuthHMAC {self.api_user_id}:{signature}'
 
     def _send_request(self, url, method, headers=None):
-        ''' Sending a request. '''
-        
+        """ Sending a request. """
+
         if not headers:
-            headers = {}
-        headers['Authorization'] = self._get_signature(url, method)
-        if method.upper() == 'GET':
-            return requests.get(url=url, headers=headers, proxies=self.proxies)
-        elif method.upper() == 'POST':
-            return requests.post(url=url, headers=headers, proxies=self.proxies)
-    
+            headers = {
+                'Authorization': self._get_signature(url, method)
+            }
+
+        with warnings.catch_warnings():
+            if not self.ssl_verify:
+                warnings.simplefilter('ignore', InsecureRequestWarning)
+            if method.upper() == 'GET':
+                return requests.get(url=url, headers=headers, proxies=self.proxies, verify=self.ssl_verify)
+            elif method.upper() == 'POST':
+                return requests.post(url=url, headers=headers, proxies=self.proxies, verify=self.ssl_verify)
+
     def create_export(self, create_params, url):
-        ''' 
-        Data export request. 
+        """
+        Data export request.
 
         -----------
         Parameters:
             create_params (dict): a dictionary with data export parameters
             url (str): API endpoint to send request
 
         Example:
             create_params = {
                 'dateFrom': '2022-05-01',
                 'dateTo': '2022-05-31',
                 'selectors': 'idAdEventTypeTitle,tsClick,tsView,dtEvent,tsEvent,idPartnerTitle,advertisingId',
-                'idApp': 1,  
+                'idApp': 1,
                 'event': 'installs'
             }
-            
-            If you want to get data for multiple apps (accounts, etc.), 
+
+            If you want to get data for multiple apps (accounts, etc.),
             then add square brackets to the key 'idApp[]': [1, 2, 3],
             or specify the desired values in the string separated by commas 'idApp': '1,2,3'.
 
         -----------
-        Returns: 
+        Returns:
             response (dict): a dictionary with the response from the server
-        '''
-        
-        encoded_params = urlencode(create_params, doseq=True).replace('%2C', ',')        
+        """
+
+        encoded_params = urlencode(create_params, doseq=True).replace('%2C', ',')
         response = self._send_request(method=self.METHOD_POST, url=f'{url}?{encoded_params}').json()
-        
+
         nl = '\n'
         if response['code'] != 200:
             if response['code'] == 400:
                 raise MyTrackerError(f'Bad request. {response["data"]["error"]["detail"]}.{nl}Response: {response}')
             elif response['code'] == 403:
                 raise MyTrackerError(f'Access denied. Maybe you made mistakes or forgot to send authorization data.{nl}Response: {response}')
             else:
                 raise MyTrackerError(f'Unknown error.{nl}Response: {response}')
-        
+
         return response
-    
+
     def get_export(self, get_params, url):
-        ''' 
-        Checking the status of the data export request. 
+        """
+        Checking the status of the data export request.
 
         -----------
         Parameters:
             get_params (dict): a dictionary with export ID parameter
             url (str): API endpoint to send request
 
         Example:
             First you need to get the export ID (create_export method)
-        
+
             - Raw Data
             get_params = {
                 'idRawExport': create_export_response['data']['idRawExport']
             }
-            
+
             - Report
             get_params = {
                 'idReportFile': create_export_response['data']['idReportFile']
             }
-            
+
             - Segment
             get_params = {
                 'idSegmentExport': create_export_response['data']['idSegmentExport']
             }
-        
+
         -----------
-        Returns: 
+        Returns:
             response (dict): a dictionary with the response from the server
-        '''
-        
+        """
+
         encoded_params = urlencode(get_params)
         response = self._send_request(method=self.METHOD_GET, url=f'{url}?{encoded_params}').json()
         return response
-        
+
     def get_raw_data(self, params, return_df=True):
-        ''' 
+        """
         Uploading data via Raw Data API.
-        
+
         -----------
         Parameters:
             params (dict): a dictionary with raw data export parameters (see on https://tracker.my.com/docs/api/export-api/raw/create)
             return_df (bool, default True): if True, then return a raw pd.DataFrame
                                             if False, then return a dictionary with the response from the server
-            
+
         Example:
             params = {
                 'dateFrom': '2022-05-01',
                 'dateTo': '2022-05-31',
                 'selectors': 'idAdEventTypeTitle,tsClick,tsView,dtEvent,tsEvent,idPartnerTitle,advertisingId',
-                'idApp': 1,  
+                'idApp': 1,
                 'event': 'installs'
             }
-            
-            If you want to get data for multiple apps (accounts, etc.), 
+
+            If you want to get data for multiple apps (accounts, etc.),
             then add square brackets to the key 'idApp[]': [1, 2, 3],
             or specify the desired values in the string separated by commas 'idApp': '1,2,3'.
         -----------
         Returns: pd.DataFrame or dict
             raw_data (pd.DataFrame): raw dataframe
             or
             response (dict): a dictionary with the response from the server
-        '''
-        
+        """
+
         create_response = self.create_export(params, url=self.CREATE_RAW_DATA_URL)
         nl = '\n'
-        
+
         get_params = {
             'idRawExport': create_response['data']['idRawExport'],
         }
         while True:
-            
+
             try:
                 get_response = self.get_export(get_params, url=self.GET_RAW_DATA_URL)
             except KeyboardInterrupt:
                 self.cancel_raw_data_export(get_params['idRawExport'])
                 raise MyTrackerError(f'The program was interrupted. The request was canceled.')
-            
+
             if get_response['code'] == 200:
                 if get_response['data']['status'] == 'Success!':
                     if return_df is True:
                         raw_data = []
-                        install_opener(build_opener(ProxyHandler(self.proxies)))
                         for file in get_response['data']['files']:
                             link = file['link']
-                            with urlopen(link, timeout=10) as f:
-                                raw_file = pd.read_csv(f, compression='gzip')
+                            raw_bytes = io.BytesIO(self._send_request(link, self.METHOD_GET).content)
+                            raw_file = pd.read_csv(raw_bytes, compression='gzip')
                             raw_data.append(raw_file)
                         raw_data = pd.concat(raw_data, ignore_index=True)
-                        break
+                        return raw_data
                     elif return_df is False:
                         return dict(get_response)
                     else:
                         raise MyTrackerError('Parameter return_df must be True or False.')
 
                 elif get_response['data']['status'] in ('In progress', 'Error occurred'):
                     try:
@@ -211,182 +216,177 @@
                         continue
                     except KeyboardInterrupt:
                         self.cancel_raw_data_export(get_params['idRawExport'])
                         raise MyTrackerError(f'The program was interrupted. The request was canceled.')
 
                 elif get_response['data']['status'] == 'User error occurred':
                     raise MyTrackerError(f'{get_response["data"]["errorMessage"]}.{nl}Response: {get_response}')
-                    
+
                 elif get_response['data']['status'] == 'Canceled by user':
                     raise MyTrackerError(f'The request was canceled.{nl}Response: {get_response}')
-                    
+
             elif get_response['code'] == 404:
                 raise MyTrackerError(f'The request is unavailable or could not be found.{nl}Response: {get_response}')
-            
+
             elif get_response['code'] == 403:
                 raise MyTrackerError(f'Access denied. Maybe you made mistakes or forgot to send authorization data.{nl}Response: {get_response}')
-                
+
             elif get_response['code'] == 429:
                 raise MyTrackerError(f'Too many requests.{nl}Response: {get_response}')
-                
+
             else:
                 raise MyTrackerError(f'Unknown error.{nl}Response: {get_response}')
 
-        return raw_data
-    
     def cancel_raw_data_export(self, id_raw_export):
-        ''' 
-        Cancel uploading raw data. 
-        
+        """
+        Cancel uploading raw data.
+
         -----------
         Parameters:
             id_raw_export (int): unique raw export integer value
-            
+
         -----------
         Returns:
             response (dict): a dictionary with the response from the server
-        '''
-        
+        """
+
         params = {
             'idRawExport': id_raw_export,
         }
         cancel_response = self.get_export(params, url=self.CANCEL_RAW_DATA_URL)
         return dict(cancel_response)
-    
+
     def get_report(self, params, return_df=True):
-        ''' 
+        """
         Uploading data via Report API.
-        
+
         -----------
         Parameters:
             params (dict): a dictionary with report export parameters (see on https://tracker.my.com/docs/api/export-api/report/create)
             return_df (bool, default True): if True, then return a raw pd.DataFrame
                                             if False, then return a dictionary with the response from the server
-            
+
         Example:
             params = {
                 'settings[selectors]': 'date,idPartner,sumCampaignCost',
                 'settings[filter][date][from]': '2022-06-01',
                 'settings[filter][date][to]': '2022-06-10',
                 'settings[filter][dimension][idApp][value]': 1,
                 'settings[filter][dimension][idPartner][value][]': [10006, 10008],
                 'settings[idCurrency]': 840,
                 'settings[tz]': 'Europe/Moscow',
                 'settings[precision]': 5,
                 'settings[retIndent]': 3600,
             }
-            
-            If you want to get data for multiple apps (partners, etc.), 
+
+            If you want to get data for multiple apps (partners, etc.),
             then add square brackets to the key 'settings[filter][dimension][idApp][value][]': [1, 2, 3],
-            or specify the desired values in the string 
+            or specify the desired values in the string
             separated by commas 'settings[filter][dimension][idApp][value]': '1,2,3'.
         -----------
         Returns: pd.DataFrame or dict
             report (pd.DataFrame): report dataframe
             or
             response (dict): a dictionary with the response from the server
-        '''
-        
+        """
+
         if 'fileType' in params.keys():
             params['fileType'] = 'csv'
-        
+
         create_response = self.create_export(params, url=self.CREATE_REPORT_URL)
         nl = '\n'
-        
+
         get_params = {
             'idReportFile': create_response['data']['idReportFile'],
         }
 
         while True:
             get_response = self.get_export(get_params, url=self.GET_REPORT_URL)
-            
+
             if get_response['code'] == 200:
                 if get_response['data']['status'] == 'Success!':
                     if return_df is True:
                         link = get_response['data']['files'][0]['link']
-                        install_opener(build_opener(ProxyHandler(self.proxies)))
-                        with urlopen(link, timeout=10) as file:
-                            report = pd.read_csv(file, compression='gzip')
-                        break
+                        raw_bytes = io.BytesIO(self._send_request(link, self.METHOD_GET).content)
+                        report = pd.read_csv(raw_bytes, compression='gzip')
+                        return report
                     elif return_df is False:
                         return dict(get_response)
                     else:
                         raise MyTrackerError('Parameter return_df must be True or False.')
 
                 elif get_response['data']['status'] == 'In progress':
                     time.sleep(4)
                     continue
 
                 elif get_response['data']['status'] == 'Error occurred':
                     raise MyTrackerError(f'Error ocurred. The file will never be created.{nl}Response: {get_response}')
-                    
+
             elif get_response['code'] == 404:
                 raise MyTrackerError(f'The file is unavailable or could not be found.{nl}Response: {get_response}')
-                
+
             elif get_response['code'] == 403:
                 raise MyTrackerError(f'Access denied. Maybe you made mistakes or forgot to send authorization data.{nl}Response: {get_response}')
-                
+
             elif get_response['code'] == 429:
                 raise MyTrackerError(f'Too many requests.{nl}Response: {get_response}')
 
             else:
                 raise MyTrackerError(f'Unknown error.{nl}Response: {get_response}')
-        
-        return report
-    
+
     def get_segment(self, params):
-        '''
+        """
         Uploading data via Segment API.
-        
+
         -----------
         Parameters:
             params (dict): a dictionary with segment export parameters (see on https://tracker.my.com/docs/api/export-api/segment/export/create)
-            
+
         Example:
             params = {
                 'idSegment': 1111,
                 'requestFields': 'idfa',
                 'includeHeaderLine': 1,
                 'registerType': 0,
                 'hashType': 0
             }
-            
-            If you want to get data with multiple requestFields, 
+
+            If you want to get data with multiple requestFields,
             then add square brackets to the key 'requestFields[]': ['idfa', 'gaid'],
             or specify the desired values in the string
             separated by commas 'requestFields': 'idfa,gaid'.
         -----------
         Returns:
             response (dict): a dictionary with the response from the server
-        '''
-    
+        """
+
         create_response = self.create_export(params, url=self.CREATE_SEGMENT_URL)
         nl = '\n'
-        
+
         get_params = {
             'idSegmentExport': create_response['data']['idSegmentExport'],
         }
-        
+
         while True:
             get_response = self.get_export(get_params, url=self.GET_SEGMENT_URL)
-            
+
             if get_response['code'] == 200:
                 if get_response['data']['status'] == 'Success!':
                     break
 
                 elif get_response['data']['status'] in ('In progress', 'Error occurred'):
                     time.sleep(4)
                     continue
 
             elif get_response['code'] == 404:
                 raise MyTrackerError(f'The request is unavailable or could not be found.{nl}Response: {get_response}')
-            
+
             elif get_response['code'] == 403:
                 raise MyTrackerError(f'Access denied. Maybe you made mistakes or forgot to send authorization data.{nl}Response: {get_response}')
-                
+
             elif get_response['code'] == 429:
                 raise MyTrackerError(f'Too many requests.{nl}Response: {get_response}')
-            
+
             else:
                 raise MyTrackerError(f'Unknown error.{nl}Response: {get_response}')
-        
+
         return dict(get_response)
```

### Comparing `mytracker_export_api-1.0.2/mytracker_export_api.egg-info/PKG-INFO` & `mytracker_export_api-1.0.4/mytracker_export_api.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mytracker-export-api
-Version: 1.0.2
+Version: 1.0.4
 Summary: Python wrapper for MyTracker Export API.
 Home-page: UNKNOWN
 Author: Artyom Novopolsky
 Author-email: a.novopolsky@corp.mail.ru
 License: UNKNOWN
 Project-URL: Documentation, https://tracker.my.com/docs/api/export-api/about
 Project-URL: Source, https://github.com/tracker-my-com/mytracker-export-api-python
```

### Comparing `mytracker_export_api-1.0.2/setup.py` & `mytracker_export_api-1.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='mytracker_export_api',
-    version='1.0.2',
+    version='1.0.4',
     description='Python wrapper for MyTracker Export API.',
     packages=['mytracker_export_api'],
     author='Artyom Novopolsky',
     author_email='a.novopolsky@corp.mail.ru',
     install_requires=open('requirements.txt').read().splitlines(),
     python_requires='>=3.6.1',
     long_description=open('README.md').read(),
```

