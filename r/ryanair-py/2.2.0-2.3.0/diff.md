# Comparing `tmp/ryanair-py-2.2.0.tar.gz` & `tmp/ryanair-py-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ryanair-py-2.2.0.tar", last modified: Tue Apr 18 22:32:10 2023, max compression
+gzip compressed data, was "ryanair-py-2.3.0.tar", last modified: Wed May  3 22:22:54 2023, max compression
```

## Comparing `ryanair-py-2.2.0.tar` & `ryanair-py-2.3.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 ciaran    (1000) ciaran    (1000)        0 2023-04-18 22:32:10.991868 ryanair-py-2.2.0/
--rw-rw-r--   0 ciaran    (1000) ciaran    (1000)     1097 2023-03-11 14:18:49.000000 ryanair-py-2.2.0/LICENSE.md
--rw-rw-r--   0 ciaran    (1000) ciaran    (1000)     5463 2023-04-18 22:32:10.987868 ryanair-py-2.2.0/PKG-INFO
--rw-rw-r--   0 ciaran    (1000) ciaran    (1000)     5056 2023-04-18 22:28:28.000000 ryanair-py-2.2.0/README.md
-drwxrwxr-x   0 ciaran    (1000) ciaran    (1000)        0 2023-04-18 22:32:10.987868 ryanair-py-2.2.0/ryanair/
--rw-rw-r--   0 ciaran    (1000) ciaran    (1000)       37 2023-03-11 14:18:49.000000 ryanair-py-2.2.0/ryanair/__init__.py
--rw-r--r--   0 ciaran    (1000) ciaran    (1000)     1516 2022-09-17 10:38:33.000000 ryanair-py-2.2.0/ryanair/airport_utils.py
--rw-r--r--   0 ciaran    (1000) ciaran    (1000)  9857193 2022-09-17 10:38:33.000000 ryanair-py-2.2.0/ryanair/airports.csv
--rw-rw-r--   0 ciaran    (1000) ciaran    (1000)    11141 2023-04-18 22:28:28.000000 ryanair-py-2.2.0/ryanair/ryanair.py
--rw-rw-r--   0 ciaran    (1000) ciaran    (1000)      281 2023-04-18 22:28:28.000000 ryanair-py-2.2.0/ryanair/types.py
-drwxrwxr-x   0 ciaran    (1000) ciaran    (1000)        0 2023-04-18 22:32:10.987868 ryanair-py-2.2.0/ryanair_py.egg-info/
--rw-rw-r--   0 ciaran    (1000) ciaran    (1000)     5463 2023-04-18 22:32:10.000000 ryanair-py-2.2.0/ryanair_py.egg-info/PKG-INFO
--rw-rw-r--   0 ciaran    (1000) ciaran    (1000)      300 2023-04-18 22:32:10.000000 ryanair-py-2.2.0/ryanair_py.egg-info/SOURCES.txt
--rw-rw-r--   0 ciaran    (1000) ciaran    (1000)        1 2023-04-18 22:32:10.000000 ryanair-py-2.2.0/ryanair_py.egg-info/dependency_links.txt
--rw-rw-r--   0 ciaran    (1000) ciaran    (1000)       28 2023-04-18 22:32:10.000000 ryanair-py-2.2.0/ryanair_py.egg-info/requires.txt
--rw-rw-r--   0 ciaran    (1000) ciaran    (1000)        8 2023-04-18 22:32:10.000000 ryanair-py-2.2.0/ryanair_py.egg-info/top_level.txt
--rw-rw-r--   0 ciaran    (1000) ciaran    (1000)       38 2023-04-18 22:32:10.991868 ryanair-py-2.2.0/setup.cfg
--rw-rw-r--   0 ciaran    (1000) ciaran    (1000)     1009 2023-04-18 22:29:05.000000 ryanair-py-2.2.0/setup.py
+drwxrwxr-x   0 ciaran    (1000) ciaran    (1000)        0 2023-05-03 22:22:54.795221 ryanair-py-2.3.0/
+-rw-rw-r--   0 ciaran    (1000) ciaran    (1000)     1097 2023-03-11 14:18:49.000000 ryanair-py-2.3.0/LICENSE.md
+-rw-rw-r--   0 ciaran    (1000) ciaran    (1000)     5463 2023-05-03 22:22:54.795221 ryanair-py-2.3.0/PKG-INFO
+-rw-rw-r--   0 ciaran    (1000) ciaran    (1000)     5056 2023-04-18 22:28:28.000000 ryanair-py-2.3.0/README.md
+drwxrwxr-x   0 ciaran    (1000) ciaran    (1000)        0 2023-05-03 22:22:54.795221 ryanair-py-2.3.0/ryanair/
+-rw-rw-r--   0 ciaran    (1000) ciaran    (1000)       37 2023-03-11 14:18:49.000000 ryanair-py-2.3.0/ryanair/__init__.py
+-rw-r--r--   0 ciaran    (1000) ciaran    (1000)     1516 2022-09-17 10:38:33.000000 ryanair-py-2.3.0/ryanair/airport_utils.py
+-rw-r--r--   0 ciaran    (1000) ciaran    (1000)  9857193 2022-09-17 10:38:33.000000 ryanair-py-2.3.0/ryanair/airports.csv
+-rw-rw-r--   0 ciaran    (1000) ciaran    (1000)    13594 2023-05-03 22:20:23.000000 ryanair-py-2.3.0/ryanair/ryanair.py
+-rw-rw-r--   0 ciaran    (1000) ciaran    (1000)      281 2023-04-18 22:28:28.000000 ryanair-py-2.3.0/ryanair/types.py
+drwxrwxr-x   0 ciaran    (1000) ciaran    (1000)        0 2023-05-03 22:22:54.795221 ryanair-py-2.3.0/ryanair_py.egg-info/
+-rw-rw-r--   0 ciaran    (1000) ciaran    (1000)     5463 2023-05-03 22:22:54.000000 ryanair-py-2.3.0/ryanair_py.egg-info/PKG-INFO
+-rw-rw-r--   0 ciaran    (1000) ciaran    (1000)      300 2023-05-03 22:22:54.000000 ryanair-py-2.3.0/ryanair_py.egg-info/SOURCES.txt
+-rw-rw-r--   0 ciaran    (1000) ciaran    (1000)        1 2023-05-03 22:22:54.000000 ryanair-py-2.3.0/ryanair_py.egg-info/dependency_links.txt
+-rw-rw-r--   0 ciaran    (1000) ciaran    (1000)       28 2023-05-03 22:22:54.000000 ryanair-py-2.3.0/ryanair_py.egg-info/requires.txt
+-rw-rw-r--   0 ciaran    (1000) ciaran    (1000)        8 2023-05-03 22:22:54.000000 ryanair-py-2.3.0/ryanair_py.egg-info/top_level.txt
+-rw-rw-r--   0 ciaran    (1000) ciaran    (1000)       38 2023-05-03 22:22:54.795221 ryanair-py-2.3.0/setup.cfg
+-rw-rw-r--   0 ciaran    (1000) ciaran    (1000)     1009 2023-05-03 22:21:20.000000 ryanair-py-2.3.0/setup.py
```

### Comparing `ryanair-py-2.2.0/LICENSE.md` & `ryanair-py-2.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ryanair-py-2.2.0/PKG-INFO` & `ryanair-py-2.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ryanair-py
-Version: 2.2.0
+Version: 2.3.0
 Summary: A module which allows you to retrieve data about the cheapest one-way and return flights in a date range, or all available flights on a given day for a given route.
 Home-page: https://github.com/cohaolain/ryanair-py
 Author: Ciarán Ó hAoláin
 Author-email: ciaran@cohaolain.ie
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `ryanair-py-2.2.0/README.md` & `ryanair-py-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `ryanair-py-2.2.0/ryanair/airport_utils.py` & `ryanair-py-2.3.0/ryanair/airport_utils.py`

 * *Files identical despite different names*

### Comparing `ryanair-py-2.2.0/ryanair/airports.csv` & `ryanair-py-2.3.0/ryanair/airports.csv`

 * *Files identical despite different names*

### Comparing `ryanair-py-2.2.0/ryanair/ryanair.py` & `ryanair-py-2.3.0/ryanair/ryanair.py`

 * *Files 18% similar despite different names*

```diff
@@ -21,40 +21,44 @@
 console_handler = logging.StreamHandler()
 formatter = logging.Formatter('%(asctime)s.%(msecs)03d %(levelname)s:%(message)s', datefmt="%Y-%m-%d %I:%M:%S")
 
 console_handler.setFormatter(formatter)
 logger.addHandler(console_handler)
 
 
+class RyanairException(Exception):
+    def __init__(self, message):
+        super().__init__(f"Ryanair API: {message}")
+
+
+class AvailabilityException(RyanairException):
+    def __init__(self):
+        super().__init__("Availability API declined to provide a result")
+
+
 # noinspection PyBroadException
 class Ryanair:
     BASE_SERVICES_API_URL = "https://services-api.ryanair.com/farfnd/v4/"
     BASE_AVAILABILITY_API_URL = "https://www.ryanair.com/api/booking/v4/"
+    BASE_SITE_FOR_SESSION_URL = "https://www.ryanair.com/ie/en"
 
     def __init__(self, currency: Optional[str] = None):
         self.currency = currency
 
         self._num_queries = 0
+        self.session = requests.Session()
+        self._update_session_cookie()
 
-    @deprecated(version="2.0.0", reason="deprecated in favour of get_cheapest_flights", action="once")
-    def get_flights(self, airport, date_from, date_to, destination_country=None):
-        return self.get_cheapest_flights(airport, date_from, date_to, destination_country)
-
-    @deprecated(version="2.0.0", reason="deprecated in favour of get_cheapest_return_flights", action="once")
-    def get_return_flights(self, source_airport, date_from, date_to,
-                           return_date_from, return_date_to,
-                           destination_country=None):
-        return self.get_cheapest_return_flights(source_airport, date_from, date_to,
-                                                return_date_from, return_date_to, destination_country)
-
-    def get_cheapest_flights(self, airport, date_from, date_to, destination_country=None,
-                             custom_params=None,
+    def get_cheapest_flights(self, airport: str, date_from: Union[datetime, date, str],
+                             date_to: Union[datetime, date, str], destination_country: Optional[str] = None,
+                             custom_params: Optional[dict] = None,
                              departure_time_from: Union[str, time] = "00:00",
                              departure_time_to: Union[str, time] = "23:59",
-                             max_price: int = None
+                             max_price: Optional[int] = None,
+                             destination_airport: Optional[str] = None
                              ):
         query_url = ''.join((Ryanair.BASE_SERVICES_API_URL,
                              "oneWayFares"))
 
         params = {
             "departureAirportIataCode": airport,
             "outboundDepartureDateFrom": self._format_date_for_api(date_from),
@@ -64,57 +68,66 @@
         }
         if self.currency:
             params['currency'] = self.currency
         if destination_country:
             params['arrivalCountryCode'] = destination_country
         if max_price:
             params['priceValueTo'] = max_price
+        if destination_airport:
+            params['arrivalAirportIataCode'] = destination_airport
         if custom_params:
             params.update(custom_params)
 
         try:
             response = self._retryable_query(query_url, params)["fares"]
         except Exception:
             logger.exception(f"Failed to parse response when querying {query_url}")
             return []
 
         if response:
             return [self._parse_cheapest_flight(flight['outbound']) for flight in response]
 
         return []
 
-    def get_cheapest_return_flights(self, source_airport, date_from, date_to,
-                                    return_date_from, return_date_to,
-                                    destination_country=None,
-                                    custom_params=None,
+    def get_cheapest_return_flights(self, source_airport: str,
+                                    date_from: Union[datetime, date, str],
+                                    date_to: Union[datetime, date, str],
+                                    return_date_from: Union[datetime, date, str],
+                                    return_date_to: Union[datetime, date, str],
+                                    destination_country: Optional[str] = None,
+                                    custom_params: Optional[dict] = None,
                                     outbound_departure_time_from: Union[str, time] = "00:00",
                                     outbound_departure_time_to: Union[str, time] = "23:59",
                                     inbound_departure_time_from: Union[str, time] = "00:00",
                                     inbound_departure_time_to: Union[str, time] = "23:59",
-                                    max_price: int = None
+                                    max_price: Optional[int] = None,
+                                    destination_airport: Optional[str] = None
                                     ):
         query_url = ''.join((Ryanair.BASE_SERVICES_API_URL,
                              "roundTripFares"))
 
         params = {
             "departureAirportIataCode": source_airport,
             "outboundDepartureDateFrom": self._format_date_for_api(date_from),
             "outboundDepartureDateTo": self._format_date_for_api(date_to),
             "inboundDepartureDateFrom": self._format_date_for_api(return_date_from),
             "inboundDepartureDateTo": self._format_date_for_api(return_date_to),
-            "currency": self.currency,
             "outboundDepartureTimeFrom": self._format_time_for_api(outbound_departure_time_from),
             "outboundDepartureTimeTo": self._format_time_for_api(outbound_departure_time_to),
             "inboundDepartureTimeFrom": self._format_time_for_api(inbound_departure_time_from),
             "inboundDepartureTimeTo": self._format_time_for_api(inbound_departure_time_to)
         }
+        if self.currency:
+            params['currency'] = self.currency
         if destination_country:
             params['arrivalCountryCode'] = destination_country
         if max_price:
             params['priceValueTo'] = max_price
+        if destination_airport:
+            params['arrivalAirportIataCode'] = destination_airport
         if custom_params:
             params.update(custom_params)
 
         try:
             response = self._retryable_query(query_url, params)["fares"]
         except Exception as e:
             logger.exception(f"Failed to parse response when querying {query_url}")
@@ -122,17 +135,17 @@
 
         if response:
             return [self._parse_cheapest_return_flights_as_trip(trip["outbound"], trip["inbound"])
                     for trip in response]
         else:
             return []
 
-    def get_all_flights(self, origin_airport, date_out, destination,
-                        locale="en-ie", origin_is_mac=False, destination_is_mac=False,
-                        custom_params=None):
+    def get_all_flights(self, origin_airport: str, date_out: Union[datetime, date, str], destination: str,
+                        locale: str = "en-ie", origin_is_mac: bool = False, destination_is_mac: bool = False,
+                        custom_params: Optional[dict] = None):
         query_url = ''.join((Ryanair.BASE_AVAILABILITY_API_URL, f"{locale}/availability"))
 
         params = {
             # Assume single adult ticket only
             "ADT": 1,
             "TEEN": 0,
             "CHD": 0,
@@ -160,42 +173,62 @@
             # "RoundTrip": false,
         }
 
         if custom_params:
             params.update(custom_params)
 
         try:
+            # Try once to get a new session cookie, just in case the old one has expired.
+            # If that fails too, we should raise the exception.
             response = self._retryable_query(query_url, params)
+            if self.check_if_availability_response_is_declined(response):
+                logger.warning("Availability API declined to respond, attempting again with a new session cookie")
+                self._update_session_cookie()
+                response = self._retryable_query(query_url, params)
+                if self.check_if_availability_response_is_declined(response):
+                    raise AvailabilityException
+
             currency = response["currency"]
             trip = response["trips"][0]
             flights = trip['dates'][0]['flights']
             if flights:
                 if self.currency and self.currency != currency:
                     logger.warning(f"Configured to fetch fares in {self.currency} but availability API doesn't support"
                                    f" specifying the currency, so it responded with fares in {currency}")
 
                 return [self._parse_all_flights_availability_result_as_flight(flight,
                                                                               trip['originName'],
                                                                               trip['destinationName'],
                                                                               currency)
                         for flight in flights]
+        except RyanairException:
+            logger.exception(f"Failed to parse response when querying {query_url} with parameters {params}")
+            return []
         except Exception:
-            logger.exception(f"Failed to parse response when querying {query_url}")
+            logger.exception(f"Failed to parse response when querying {query_url} with parameters {params}")
             return []
 
     @staticmethod
+    def check_if_availability_response_is_declined(response: dict) -> bool:
+        return 'message' in response and response['message'] == 'Availability declined'
+
+    @staticmethod
     def _on_query_error(e):
         logger.exception(f"Gave up retrying query, last exception was {e}")
 
     @backoff.on_exception(backoff.expo, Exception, max_tries=5, logger=logger, on_giveup=_on_query_error,
                           raise_on_giveup=False)
     def _retryable_query(self, url, params):
         self._num_queries += 1
 
-        return requests.get(url, params=params).json()
+        return self.session.get(url, params=params).json()
+
+    def _update_session_cookie(self):
+        # Visit main website to get session cookies
+        self.session.get(Ryanair.BASE_SITE_FOR_SESSION_URL)
 
     def _parse_cheapest_flight(self, flight):
         currency = flight['price']['currencyCode']
         if self.currency and self.currency != currency:
             logger.warning(f"Requested cheapest flights in {self.currency} but API responded with fares in {currency}")
         return Flight(
             origin=flight['departureAirport']['iataCode'],
@@ -239,17 +272,28 @@
         if isinstance(d, datetime):
             return d.date().isoformat()
 
         if isinstance(d, date):
             return d.isoformat()
 
     @staticmethod
-    def _format_time_for_api(t):
+    def _format_time_for_api(t: Union[time, str]):
         if isinstance(t, str):
             return t
 
         if isinstance(t, time):
             return t.strftime("%H:%M")
 
     @property
     def num_queries(self):
         return self._num_queries
+
+    @deprecated(version="2.0.0", reason="deprecated in favour of get_cheapest_flights", action="once")
+    def get_flights(self, airport, date_from, date_to, destination_country=None):
+        return self.get_cheapest_flights(airport, date_from, date_to, destination_country)
+
+    @deprecated(version="2.0.0", reason="deprecated in favour of get_cheapest_return_flights", action="once")
+    def get_return_flights(self, source_airport, date_from, date_to,
+                           return_date_from, return_date_to,
+                           destination_country=None):
+        return self.get_cheapest_return_flights(source_airport, date_from, date_to,
+                                                return_date_from, return_date_to, destination_country)
```

### Comparing `ryanair-py-2.2.0/ryanair_py.egg-info/PKG-INFO` & `ryanair-py-2.3.0/ryanair_py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ryanair-py
-Version: 2.2.0
+Version: 2.3.0
 Summary: A module which allows you to retrieve data about the cheapest one-way and return flights in a date range, or all available flights on a given day for a given route.
 Home-page: https://github.com/cohaolain/ryanair-py
 Author: Ciarán Ó hAoláin
 Author-email: ciaran@cohaolain.ie
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `ryanair-py-2.2.0/setup.py` & `ryanair-py-2.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup
 from os import path
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(name='ryanair-py',
-      version='2.2.0',
+      version='2.3.0',
       description='A module which allows you to retrieve data about the cheapest one-way and return flights '
                   'in a date range, or all available flights on a given day for a given route.',
       long_description=long_description,
       long_description_content_type='text/markdown',
       author='Ciarán Ó hAoláin',
       author_email='ciaran@cohaolain.ie',
       url='https://github.com/cohaolain/ryanair-py',
```

