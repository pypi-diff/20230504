# Comparing `tmp/alpha_trader_python-0.0.1.tar.gz` & `tmp/alpha_trader_python-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alpha_trader_python-0.0.1.tar", max compression
+gzip compressed data, was "alpha_trader_python-0.0.2.tar", max compression
```

## Comparing `alpha_trader_python-0.0.1.tar` & `alpha_trader_python-0.0.2.tar`

### file list

```diff
@@ -1,22 +1,24 @@
--rw-r--r--   0        0        0      255 2023-05-01 16:31:08.618209 alpha_trader_python-0.0.1/README.md
--rw-r--r--   0        0        0       22 2023-05-01 16:31:29.498483 alpha_trader_python-0.0.1/alpha_trader/__init__.py
--rw-r--r--   0        0        0     2074 2023-05-01 16:31:08.618209 alpha_trader_python-0.0.1/alpha_trader/achievement/__init__.py
--rw-r--r--   0        0        0        0 2023-05-01 16:31:08.618209 alpha_trader_python-0.0.1/alpha_trader/authentication/__init__.py
--rw-r--r--   0        0        0      529 2023-05-01 16:31:08.618209 alpha_trader_python-0.0.1/alpha_trader/bank_account/__init__.py
--rw-r--r--   0        0        0     5535 2023-05-01 16:31:08.618209 alpha_trader_python-0.0.1/alpha_trader/client/__init__.py
--rw-r--r--   0        0        0     2449 2023-05-01 16:31:08.618209 alpha_trader_python-0.0.1/alpha_trader/company/__init__.py
--rw-r--r--   0        0        0     1155 2023-05-01 16:31:08.618209 alpha_trader_python-0.0.1/alpha_trader/listing/__init__.py
--rw-r--r--   0        0        0      387 2023-05-01 16:31:08.618209 alpha_trader_python-0.0.1/alpha_trader/logging/__init__.py
--rw-r--r--   0        0        0     4276 2023-05-01 16:31:08.618209 alpha_trader_python-0.0.1/alpha_trader/miner/__init__.py
--rw-r--r--   0        0        0     5904 2023-05-01 16:31:08.618209 alpha_trader_python-0.0.1/alpha_trader/order/__init__.py
--rw-r--r--   0        0        0      470 2023-05-01 16:31:08.618209 alpha_trader_python-0.0.1/alpha_trader/owner/__init__.py
--rw-r--r--   0        0        0       71 2023-05-01 16:31:08.618209 alpha_trader_python-0.0.1/alpha_trader/partner/__init__.py
--rw-r--r--   0        0        0     1629 2023-05-01 16:31:08.618209 alpha_trader_python-0.0.1/alpha_trader/portfolio/__init__.py
--rw-r--r--   0        0        0     1895 2023-05-01 16:31:08.618209 alpha_trader_python-0.0.1/alpha_trader/portfolio/position.py
--rw-r--r--   0        0        0        0 2023-05-01 16:31:08.622209 alpha_trader_python-0.0.1/alpha_trader/price/__init__.py
--rw-r--r--   0        0        0      405 2023-05-01 16:31:08.622209 alpha_trader_python-0.0.1/alpha_trader/price/price.py
--rw-r--r--   0        0        0     1503 2023-05-01 16:31:08.622209 alpha_trader_python-0.0.1/alpha_trader/price/price_spread.py
--rw-r--r--   0        0        0     2771 2023-05-01 16:31:08.622209 alpha_trader_python-0.0.1/alpha_trader/securities_account/__init__.py
--rw-r--r--   0        0        0     7674 2023-05-01 16:31:08.622209 alpha_trader_python-0.0.1/alpha_trader/user/__init__.py
--rw-r--r--   0        0        0      922 2023-05-01 16:31:29.498483 alpha_trader_python-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      805 1970-01-01 00:00:00.000000 alpha_trader_python-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      255 2023-05-04 06:59:39.907919 alpha_trader_python-0.0.2/README.md
+-rw-r--r--   0        0        0       22 2023-05-04 06:59:39.907919 alpha_trader_python-0.0.2/alpha_trader/__init__.py
+-rw-r--r--   0        0        0     2074 2023-05-04 06:59:39.907919 alpha_trader_python-0.0.2/alpha_trader/achievement/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-04 06:59:39.907919 alpha_trader_python-0.0.2/alpha_trader/authentication/__init__.py
+-rw-r--r--   0        0        0      529 2023-05-04 06:59:39.907919 alpha_trader_python-0.0.2/alpha_trader/bank_account/__init__.py
+-rw-r--r--   0        0        0     4768 2023-05-04 06:59:39.907919 alpha_trader_python-0.0.2/alpha_trader/bonds/__init__.py
+-rw-r--r--   0        0        0     7460 2023-05-04 06:59:39.907919 alpha_trader_python-0.0.2/alpha_trader/client/__init__.py
+-rw-r--r--   0        0        0     2993 2023-05-04 06:59:39.907919 alpha_trader_python-0.0.2/alpha_trader/company/__init__.py
+-rw-r--r--   0        0        0      776 2023-05-04 06:59:39.907919 alpha_trader_python-0.0.2/alpha_trader/filter/__init__.py
+-rw-r--r--   0        0        0     1155 2023-05-04 06:59:39.907919 alpha_trader_python-0.0.2/alpha_trader/listing/__init__.py
+-rw-r--r--   0        0        0      387 2023-05-04 06:59:39.907919 alpha_trader_python-0.0.2/alpha_trader/logging/__init__.py
+-rw-r--r--   0        0        0     4276 2023-05-04 06:59:39.907919 alpha_trader_python-0.0.2/alpha_trader/miner/__init__.py
+-rw-r--r--   0        0        0     5904 2023-05-04 06:59:39.907919 alpha_trader_python-0.0.2/alpha_trader/order/__init__.py
+-rw-r--r--   0        0        0      470 2023-05-04 06:59:39.907919 alpha_trader_python-0.0.2/alpha_trader/owner/__init__.py
+-rw-r--r--   0        0        0       71 2023-05-04 06:59:39.907919 alpha_trader_python-0.0.2/alpha_trader/partner/__init__.py
+-rw-r--r--   0        0        0     1629 2023-05-04 06:59:39.907919 alpha_trader_python-0.0.2/alpha_trader/portfolio/__init__.py
+-rw-r--r--   0        0        0     1895 2023-05-04 06:59:39.907919 alpha_trader_python-0.0.2/alpha_trader/portfolio/position.py
+-rw-r--r--   0        0        0        0 2023-05-04 06:59:39.907919 alpha_trader_python-0.0.2/alpha_trader/price/__init__.py
+-rw-r--r--   0        0        0      405 2023-05-04 06:59:39.907919 alpha_trader_python-0.0.2/alpha_trader/price/price.py
+-rw-r--r--   0        0        0     2790 2023-05-04 06:59:39.907919 alpha_trader_python-0.0.2/alpha_trader/price/price_spread.py
+-rw-r--r--   0        0        0     2771 2023-05-04 06:59:39.907919 alpha_trader_python-0.0.2/alpha_trader/securities_account/__init__.py
+-rw-r--r--   0        0        0     7727 2023-05-04 06:59:39.907919 alpha_trader_python-0.0.2/alpha_trader/user/__init__.py
+-rw-r--r--   0        0        0      922 2023-05-04 06:59:39.911919 alpha_trader_python-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      805 1970-01-01 00:00:00.000000 alpha_trader_python-0.0.2/PKG-INFO
```

### Comparing `alpha_trader_python-0.0.1/alpha_trader/achievement/__init__.py` & `alpha_trader_python-0.0.2/alpha_trader/achievement/__init__.py`

 * *Files identical despite different names*

### Comparing `alpha_trader_python-0.0.1/alpha_trader/bank_account/__init__.py` & `alpha_trader_python-0.0.2/alpha_trader/bank_account/__init__.py`

 * *Files identical despite different names*

### Comparing `alpha_trader_python-0.0.1/alpha_trader/client/__init__.py` & `alpha_trader_python-0.0.2/alpha_trader/client/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from __future__ import annotations
 
 from pydantic import BaseModel
-from typing import Union, Dict
+from typing import Union, Dict, List
 import requests
 import os
 
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from alpha_trader.miner import Miner
     from alpha_trader.listing import Listing
     from alpha_trader.price.price_spread import PriceSpread
     from alpha_trader.user import User
     from alpha_trader.securities_account import SecuritiesAccount
+    from alpha_trader.bonds import Bond
 
 from alpha_trader.logging import logger
 
 
 class Client(BaseModel):
     """
     Client for interacting with the Alpha Trader API.
@@ -79,42 +80,49 @@
     def __get_headers(self):
         """"""
         headers = {"Authorization": f"Bearer {self.token}"}
 
         return headers
 
     def request(
-        self, method: str, endpoint: str, data: Dict = None
+            self, method: str, endpoint: str, data: Dict = None, json: Dict = None, additional_headers: Dict = None, params: Dict = None
     ) -> requests.Response:
         """Make a request using the authenticated client. This method is mainly used internally by other classes
         to retrieve more information from the API.
 
         Example:
             ```python
             >>> response = client.request("GET", "api/user")
             >>> user_information = response.json()
             >>> user_information["username"]
             Malte
 
         Args:
+            body: body parameters
+            additional_headers: Additional headers to be added to the request
             method: HTTP method
             endpoint: Endpoint
             data: Data
 
         Returns:
             HTTP Response
         """
 
         url = os.path.join(self.base_url, endpoint)
 
         if not self.authenticated:
             raise Exception("Client is not authenticated.")
 
+        if additional_headers is None:
+            headers = self.__get_headers()
+        else:
+            headers = self.__get_headers() | additional_headers
+
         response = requests.request(
-            method, url, data=data, headers=self.__get_headers()
+            method, url, data=data, headers=headers, params=params, json=json
         )
 
         return response
 
     def get_user(self) -> User:
         """Get the user information for the authenticated user.
         Example:
@@ -152,15 +160,15 @@
     def get_listing(self, security_identifier: str) -> Listing:
         """Get the listing information for a security.
         :param security_identifier: Security identifier
         :return: Listing
         """
         from alpha_trader.listing import Listing
 
-        response = self.request("GET", f"/api/listings/{security_identifier}")
+        response = self.request("GET", f"api/listings/{security_identifier}")
 
         return Listing.initialize_from_api_response(response.json(), client=self)
 
     def get_price_spread(self, security_identifier: str) -> PriceSpread:
         """Get the price spread for a security.
         :param security_identifier: Security identifier
         :return: Price spread
@@ -181,7 +189,58 @@
         response = self.request(
             "GET", f"api/v2/securitiesaccountdetails/{securities_account_id}"
         )
 
         return SecuritiesAccount.initialize_from_api_response(
             response.json(), client=self
         )
+
+    def filter_listings(self, filter_id: str = None, filter_definition: Dict = None) -> List[PriceSpread]:
+        """
+
+        Returns:
+            Price Spreads
+
+        """
+        from alpha_trader.price.price_spread import PriceSpread
+
+        if filter_definition is None:
+            filter_definition = {}
+
+        if filter_id is None:
+            params = None
+        else:
+            params = {"filterId": filter_id}
+
+        response = self.request(
+            "POST",
+            "api/v2/filter/pricespreads",
+            json=filter_definition,
+            additional_headers={"Content-Type": "application/json"},
+            params=params
+        )
+
+        return [
+            PriceSpread.initialize_from_filter_api_response(item, client=self) for item in response.json()["results"]
+        ]
+
+    def get_bond(self, security_identifier: str, price_spread: Union[PriceSpread, None] = None) -> Bond:
+        """
+            Get the bond information for a security.
+
+        Args:
+            price_spread: manually set the price spread
+            security_identifier: Security identifier
+
+        Returns:
+            Bond
+        """
+        from alpha_trader.bonds import Bond
+
+        response = self.request("GET", f"api/bonds/securityidentifier/{security_identifier}")
+
+        Bond.update_forward_refs()
+
+        return Bond.initialize_from_api_response(response.json(), client=self, price_spread=price_spread)
+
+    def get_bonds(self, page: int, search: str, page_size: int):
+        pass
```

### Comparing `alpha_trader_python-0.0.1/alpha_trader/company/__init__.py` & `alpha_trader_python-0.0.2/alpha_trader/company/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,17 @@
+from __future__ import annotations
+
 from pydantic import BaseModel
 from typing import Dict
 
 from alpha_trader.client import Client
-from alpha_trader.user import User
 from alpha_trader.listing import Listing
 from alpha_trader.bank_account import BankAccount
+from alpha_trader.bonds import Bond
+from alpha_trader.user import User
 
 
 class Company(BaseModel):
     achievement_count: int
     achievement_count: int
     bank_account: BankAccount
     ceo: User
@@ -19,14 +22,16 @@
     securities_account_id: str
     security_identifier: str
     version: int
     client: Client
 
     @staticmethod
     def initialize_from_api_response(api_response: Dict, client: Client):
+        from alpha_trader.user import User
+
         return Company(
             achievement_count=api_response["achievementCount"],
             bank_account=BankAccount.initialize_from_api_response(
                 api_response["bankAccount"]
             ),
             ceo=User.initialize_from_api_response(api_response["ceo"], client),
             id=api_response["id"],
@@ -64,7 +69,23 @@
 
     def __repr__(self):
         return self.__str__()
 
     @property
     def securities_account(self):
         return self.client.get_securities_account(self.securities_account_id)
+
+    def issue_bonds(
+            self,
+            face_value: float,
+            interest_rate: float,
+            maturity_date: int,
+            number_of_bonds: int
+    ):
+        return Bond.issue(
+            self.id,
+            face_value=face_value,
+            interest_rate=interest_rate,
+            maturity_date=maturity_date,
+            number_of_bonds=number_of_bonds,
+            client=self.client
+        )
```

### Comparing `alpha_trader_python-0.0.1/alpha_trader/listing/__init__.py` & `alpha_trader_python-0.0.2/alpha_trader/listing/__init__.py`

 * *Files identical despite different names*

### Comparing `alpha_trader_python-0.0.1/alpha_trader/miner/__init__.py` & `alpha_trader_python-0.0.2/alpha_trader/miner/__init__.py`

 * *Files identical despite different names*

### Comparing `alpha_trader_python-0.0.1/alpha_trader/order/__init__.py` & `alpha_trader_python-0.0.2/alpha_trader/order/__init__.py`

 * *Files identical despite different names*

### Comparing `alpha_trader_python-0.0.1/alpha_trader/portfolio/__init__.py` & `alpha_trader_python-0.0.2/alpha_trader/portfolio/__init__.py`

 * *Files identical despite different names*

### Comparing `alpha_trader_python-0.0.1/alpha_trader/portfolio/position.py` & `alpha_trader_python-0.0.2/alpha_trader/portfolio/position.py`

 * *Files identical despite different names*

### Comparing `alpha_trader_python-0.0.1/alpha_trader/price/price_spread.py` & `alpha_trader_python-0.0.2/alpha_trader/price/price_spread.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,41 +4,62 @@
 from alpha_trader.listing import Listing
 from alpha_trader.price.price import Price
 from alpha_trader.client import Client
 
 
 class PriceSpread(BaseModel):
     listing: Listing
-    bid_price: float
-    bid_size: int
-    ask_price: float
-    ask_size: int
-    spread_abs: float
-    spread_percent: float
-    date: int
+    bid_price: Union[float, None]
+    bid_size: Union[int, None]
+    ask_price: Union[float, None]
+    ask_size: Union[int, None]
+    spread_abs: Union[float, None]
+    spread_percent: Union[float, None]
+    date: Union[int, None]
     last_price: Price
     end_date: Union[int, None]
     name: str
     security_identifier: str
     start_date: int
     type: str
 
     @staticmethod
     def initialize_from_api_response(api_response: Dict, client: Client):
         return PriceSpread(
             listing=Listing.initialize_from_api_response(
                 api_response["listing"], client=client
             ),
-            bid_price=api_response["bidPrice"],
-            bid_size=api_response["bidSize"],
-            ask_price=api_response["askPrice"],
-            ask_size=api_response["askSize"],
-            spread_abs=api_response["spreadAbs"],
-            spread_percent=api_response["spreadPercent"],
+            bid_price=api_response.get("bidPrice", None),
+            bid_size=api_response.get("bidSize", None),
+            ask_price=api_response.get("askPrice", None),
+            ask_size=api_response.get("askSize", None),
+            spread_abs=api_response.get("spreadAbs", None),
+            spread_percent=api_response.get("spreadPercent", None),
             date=api_response["date"],
             last_price=Price.initialize_from_api_response(api_response["lastPrice"]),
             end_date=api_response["listing"]["endDate"],
             name=api_response["listing"]["name"],
             security_identifier=api_response["listing"]["securityIdentifier"],
             start_date=api_response["listing"]["startDate"],
             type=api_response["listing"]["type"],
         )
+
+    @staticmethod
+    def initialize_from_filter_api_response(api_response: Dict, client: Client):
+        return PriceSpread(
+            listing=Listing.initialize_from_api_response(
+                api_response["listing"], client=client
+            ),
+            bid_price=api_response["price"].get("bidPrice", None),
+            bid_size=api_response["price"].get("bidSize", None),
+            ask_price=api_response["price"].get("askPrice", None),
+            ask_size=api_response["price"].get("askSize", None),
+            spread_abs=api_response["price"].get("spreadAbs", None),
+            spread_percent=api_response["price"].get("spreadPercent", None),
+            date=api_response["price"].get("date", None),
+            last_price=Price.initialize_from_api_response(api_response["price"]["lastPrice"]),
+            end_date=api_response["listing"].get("endDate", None),
+            name=api_response["listing"]["name"],
+            security_identifier=api_response["listing"]["securityIdentifier"],
+            start_date=api_response["listing"]["startDate"],
+            type=api_response["listing"]["type"],
+        )
```

### Comparing `alpha_trader_python-0.0.1/alpha_trader/securities_account/__init__.py` & `alpha_trader_python-0.0.2/alpha_trader/securities_account/__init__.py`

 * *Files identical despite different names*

### Comparing `alpha_trader_python-0.0.1/alpha_trader/user/__init__.py` & `alpha_trader_python-0.0.2/alpha_trader/user/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 from pydantic import BaseModel
-from typing import Dict, Union
+from typing import Dict, Union, List
 
 from alpha_trader.client import Client
 from alpha_trader.achievement import Achievement
 from alpha_trader.logging import logger
 from alpha_trader.securities_account import SecuritiesAccount
 
 from typing import TYPE_CHECKING
@@ -32,16 +32,16 @@
         team_role_description: Team role description of the user
         level_2_user: Level 2 user of the user
         partner: Flag if the user is a partner
         premium: Flag if the user is premium
     """
 
     partner_id: Union[str, None]
-    achievement_count: int
-    achievement_total: int
+    achievement_count: Union[None, int]
+    achievement_total: Union[None, int]
     last_sponsoring_date: Union[None, str]
     level_2_user_end_date: Union[None, str]
     locale: str
     premium_end_date: Union[None, int]
     sponsored_hours: int
     team_department: Union[None, str]
     team_role: str
@@ -118,15 +118,15 @@
             registration_date=api_response["registrationDate"],
             version=api_response["version"],
             my_user=api_response["myUser"],
             client=client,
         )
 
     @property
-    def achievements(self):
+    def achievements(self) -> List[Achievement]:
         """
             Achievements of the user
 
         Returns:
             List of achievements
         """
         response = self.client.request(
@@ -185,15 +185,15 @@
         }
 
         response = self.client.request("POST", "api/companies", data=data)
 
         return Company.initialize_from_api_response(response.json(), self.client)
 
     @property
-    def companies(self) -> list[Company]:
+    def companies(self) -> List[Company]:
         """
             Get all companies that the user is CEO of
         Returns:
             List of companies
         """
         from alpha_trader.company import Company
```

### Comparing `alpha_trader_python-0.0.1/pyproject.toml` & `alpha_trader_python-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "alpha-trader-python"
-version = "0.0.1"
+version = "0.0.2"
 description = "Python SDK for https://alpha-trader.com"
 authors = ["maltemelzer"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "alpha_trader"}]
 
 [tool.poetry.dependencies]
```

### Comparing `alpha_trader_python-0.0.1/PKG-INFO` & `alpha_trader_python-0.0.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alpha-trader-python
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python SDK for https://alpha-trader.com
 License: MIT
 Author: maltemelzer
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

