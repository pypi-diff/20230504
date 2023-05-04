# Comparing `tmp/cognite_gql_pygen-0.4.0.tar.gz` & `tmp/cognite_gql_pygen-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognite_gql_pygen-0.4.0.tar", max compression
+gzip compressed data, was "cognite_gql_pygen-0.4.1.tar", max compression
```

## Comparing `cognite_gql_pygen-0.4.0.tar` & `cognite_gql_pygen-0.4.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0    11349 2023-04-27 14:28:28.759462 cognite_gql_pygen-0.4.0/LICENSE
--rw-r--r--   0        0        0     4486 2023-04-27 14:28:28.759462 cognite_gql_pygen-0.4.0/README.md
--rw-r--r--   0        0        0     8657 2023-04-27 14:28:28.759462 cognite_gql_pygen-0.4.0/cognite/dm_clients/README.md
--rw-r--r--   0        0        0        0 2023-04-27 14:28:28.759462 cognite_gql_pygen-0.4.0/cognite/dm_clients/__init__.py
--rw-r--r--   0        0        0      167 2023-04-27 14:28:28.759462 cognite_gql_pygen-0.4.0/cognite/dm_clients/cdf/__init__.py
--rw-r--r--   0        0        0    18972 2023-04-27 14:28:28.759462 cognite_gql_pygen-0.4.0/cognite/dm_clients/cdf/client_dm_v3.py
--rw-r--r--   0        0        0     3909 2023-04-27 14:28:28.759462 cognite_gql_pygen-0.4.0/cognite/dm_clients/cdf/data_classes_dm_v3.py
--rw-r--r--   0        0        0     2629 2023-04-27 14:28:28.759462 cognite_gql_pygen-0.4.0/cognite/dm_clients/cdf/get_client.py
--rwxr-xr-x   0        0        0      346 2023-04-27 14:28:28.759462 cognite_gql_pygen-0.4.0/cognite/dm_clients/config.py
--rw-r--r--   0        0        0      192 2023-04-27 14:28:28.759462 cognite_gql_pygen-0.4.0/cognite/dm_clients/custom_types/__init__.py
--rw-r--r--   0        0        0      236 2023-04-27 14:28:28.759462 cognite_gql_pygen-0.4.0/cognite/dm_clients/custom_types/_scalars.py
--rw-r--r--   0        0        0      760 2023-04-27 14:28:28.759462 cognite_gql_pygen-0.4.0/cognite/dm_clients/custom_types/jsonobject.py
--rw-r--r--   0        0        0     4724 2023-04-27 14:28:28.759462 cognite_gql_pygen-0.4.0/cognite/dm_clients/custom_types/timestamp.py
--rw-r--r--   0        0        0      196 2023-04-27 14:28:28.759462 cognite_gql_pygen-0.4.0/cognite/dm_clients/domain_modeling/__init__.py
--rw-r--r--   0        0        0     6324 2023-04-27 14:28:28.759462 cognite_gql_pygen-0.4.0/cognite/dm_clients/domain_modeling/domain_client.py
--rw-r--r--   0        0        0     3046 2023-04-27 14:28:28.759462 cognite_gql_pygen-0.4.0/cognite/dm_clients/domain_modeling/domain_model.py
--rw-r--r--   0        0        0    16000 2023-04-27 14:28:28.759462 cognite_gql_pygen-0.4.0/cognite/dm_clients/domain_modeling/domain_model_api.py
--rw-r--r--   0        0        0     3607 2023-04-27 14:28:28.759462 cognite_gql_pygen-0.4.0/cognite/dm_clients/domain_modeling/relationship_api.py
--rw-r--r--   0        0        0     7060 2023-04-27 14:28:28.759462 cognite_gql_pygen-0.4.0/cognite/dm_clients/domain_modeling/schema.py
--rw-r--r--   0        0        0     1423 2023-04-27 14:28:28.759462 cognite_gql_pygen-0.4.0/cognite/dm_clients/misc.py
--rw-r--r--   0        0        0        0 2023-04-27 14:28:28.759462 cognite_gql_pygen-0.4.0/cognite/dm_clients/py.typed
--rw-r--r--   0        0        0       76 2023-04-27 14:28:28.759462 cognite_gql_pygen-0.4.0/cognite/gqlpygen/__init__.py
--rw-r--r--   0        0        0     1868 2023-04-27 14:28:28.759462 cognite_gql_pygen-0.4.0/cognite/gqlpygen/data_classes.py
--rw-r--r--   0        0        0     1560 2023-04-27 14:28:28.759462 cognite_gql_pygen-0.4.0/cognite/gqlpygen/generator.py
--rw-r--r--   0        0        0     7728 2023-04-27 14:28:28.759462 cognite_gql_pygen-0.4.0/cognite/gqlpygen/main.py
--rw-r--r--   0        0        0      596 2023-04-27 14:28:28.759462 cognite_gql_pygen-0.4.0/cognite/gqlpygen/misc.py
--rw-r--r--   0        0        0     1288 2023-04-27 14:28:28.759462 cognite_gql_pygen-0.4.0/cognite/gqlpygen/parser.py
--rw-r--r--   0        0        0     1333 2023-04-27 14:28:28.759462 cognite_gql_pygen-0.4.0/cognite/gqlpygen/templates/client.txt
--rw-r--r--   0        0        0      803 2023-04-27 14:28:28.759462 cognite_gql_pygen-0.4.0/cognite/gqlpygen/templates/schema.txt
--rw-r--r--   0        0        0       22 2023-04-27 14:28:28.763462 cognite_gql_pygen-0.4.0/cognite/gqlpygen/version.py
--rw-r--r--   0        0        0     1995 2023-04-27 14:28:28.763462 cognite_gql_pygen-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     5538 1970-01-01 00:00:00.000000 cognite_gql_pygen-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0    11349 2023-05-04 09:28:32.239169 cognite_gql_pygen-0.4.1/LICENSE
+-rw-r--r--   0        0        0     4486 2023-05-04 09:28:32.239169 cognite_gql_pygen-0.4.1/README.md
+-rw-r--r--   0        0        0     8651 2023-05-04 09:28:32.243169 cognite_gql_pygen-0.4.1/cognite/dm_clients/README.md
+-rw-r--r--   0        0        0        0 2023-05-04 09:28:32.243169 cognite_gql_pygen-0.4.1/cognite/dm_clients/__init__.py
+-rw-r--r--   0        0        0      167 2023-05-04 09:28:32.243169 cognite_gql_pygen-0.4.1/cognite/dm_clients/cdf/__init__.py
+-rw-r--r--   0        0        0    19000 2023-05-04 09:28:32.243169 cognite_gql_pygen-0.4.1/cognite/dm_clients/cdf/client_dm_v3.py
+-rw-r--r--   0        0        0     3909 2023-05-04 09:28:32.243169 cognite_gql_pygen-0.4.1/cognite/dm_clients/cdf/data_classes_dm_v3.py
+-rw-r--r--   0        0        0     2629 2023-05-04 09:28:32.243169 cognite_gql_pygen-0.4.1/cognite/dm_clients/cdf/get_client.py
+-rwxr-xr-x   0        0        0      346 2023-05-04 09:28:32.243169 cognite_gql_pygen-0.4.1/cognite/dm_clients/config.py
+-rw-r--r--   0        0        0      192 2023-05-04 09:28:32.243169 cognite_gql_pygen-0.4.1/cognite/dm_clients/custom_types/__init__.py
+-rw-r--r--   0        0        0      236 2023-05-04 09:28:32.243169 cognite_gql_pygen-0.4.1/cognite/dm_clients/custom_types/_scalars.py
+-rw-r--r--   0        0        0      760 2023-05-04 09:28:32.243169 cognite_gql_pygen-0.4.1/cognite/dm_clients/custom_types/jsonobject.py
+-rw-r--r--   0        0        0     4724 2023-05-04 09:28:32.243169 cognite_gql_pygen-0.4.1/cognite/dm_clients/custom_types/timestamp.py
+-rw-r--r--   0        0        0      196 2023-05-04 09:28:32.243169 cognite_gql_pygen-0.4.1/cognite/dm_clients/domain_modeling/__init__.py
+-rw-r--r--   0        0        0     6324 2023-05-04 09:28:32.243169 cognite_gql_pygen-0.4.1/cognite/dm_clients/domain_modeling/domain_client.py
+-rw-r--r--   0        0        0     3863 2023-05-04 09:28:32.243169 cognite_gql_pygen-0.4.1/cognite/dm_clients/domain_modeling/domain_model.py
+-rw-r--r--   0        0        0    19106 2023-05-04 09:28:32.243169 cognite_gql_pygen-0.4.1/cognite/dm_clients/domain_modeling/domain_model_api.py
+-rw-r--r--   0        0        0     5929 2023-05-04 09:28:32.243169 cognite_gql_pygen-0.4.1/cognite/dm_clients/domain_modeling/relationship_api.py
+-rw-r--r--   0        0        0     7060 2023-05-04 09:28:32.243169 cognite_gql_pygen-0.4.1/cognite/dm_clients/domain_modeling/schema.py
+-rw-r--r--   0        0        0     1423 2023-05-04 09:28:32.243169 cognite_gql_pygen-0.4.1/cognite/dm_clients/misc.py
+-rw-r--r--   0        0        0        0 2023-05-04 09:28:32.243169 cognite_gql_pygen-0.4.1/cognite/dm_clients/py.typed
+-rw-r--r--   0        0        0       76 2023-05-04 09:28:32.243169 cognite_gql_pygen-0.4.1/cognite/gqlpygen/__init__.py
+-rw-r--r--   0        0        0     1868 2023-05-04 09:28:32.243169 cognite_gql_pygen-0.4.1/cognite/gqlpygen/data_classes.py
+-rw-r--r--   0        0        0     1560 2023-05-04 09:28:32.243169 cognite_gql_pygen-0.4.1/cognite/gqlpygen/generator.py
+-rw-r--r--   0        0        0     7728 2023-05-04 09:28:32.243169 cognite_gql_pygen-0.4.1/cognite/gqlpygen/main.py
+-rw-r--r--   0        0        0      596 2023-05-04 09:28:32.243169 cognite_gql_pygen-0.4.1/cognite/gqlpygen/misc.py
+-rw-r--r--   0        0        0     1288 2023-05-04 09:28:32.243169 cognite_gql_pygen-0.4.1/cognite/gqlpygen/parser.py
+-rw-r--r--   0        0        0     1333 2023-05-04 09:28:32.243169 cognite_gql_pygen-0.4.1/cognite/gqlpygen/templates/client.txt
+-rw-r--r--   0        0        0      803 2023-05-04 09:28:32.243169 cognite_gql_pygen-0.4.1/cognite/gqlpygen/templates/schema.txt
+-rw-r--r--   0        0        0       22 2023-05-04 09:28:32.243169 cognite_gql_pygen-0.4.1/cognite/gqlpygen/version.py
+-rw-r--r--   0        0        0     2024 2023-05-04 09:28:32.247169 cognite_gql_pygen-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     5588 1970-01-01 00:00:00.000000 cognite_gql_pygen-0.4.1/PKG-INFO
```

### Comparing `cognite_gql_pygen-0.4.0/LICENSE` & `cognite_gql_pygen-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.4.0/README.md` & `cognite_gql_pygen-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.4.0/cognite/dm_clients/README.md` & `cognite_gql_pygen-0.4.1/cognite/dm_clients/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -134,15 +134,15 @@
 
 > Note: Depending on the changes made to the schema, you might be required to update the schema version in config.yaml.
 > This happens when the changes are not backwards-compatible, e.g. deleting a field.
 
 
 ### Manipulate Items
 
-See in [examples/cinematography_domain/__main__.py](../../examples/cinematography_domain/__main__.py) for a simple
+See in [examples/cinematography_domain/usage.py](../../examples/cinematography_domain/usage.py) for a simple
 usage example.
 
 A few general notes:
 
  * `DomainClient` dynamically instantiates a `DomainModelAPI` for every model in the schema.
    * These APIs are named after the model name.
      * e.g. if the model class is names `MyModel`, the API will be accessible at `my_domain_client.my_model`.
```

### Comparing `cognite_gql_pygen-0.4.0/cognite/dm_clients/cdf/client_dm_v3.py` & `cognite_gql_pygen-0.4.1/cognite/dm_clients/cdf/client_dm_v3.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,28 +43,28 @@
         """
         Request data from API, potentially making multiple request if `limit` is not set in `data`.
         For POST requests: `data` is sent as JSON in the body
         For GET requests: `data` is sent se url query params (url-encoded)
         """
         follow_cursor = data.get("limit") is None
         data = data.copy()
-        logger.debug(f"{method} to {url}, data:\n{pformat(data)}")
         response = self._make_request(method, url, data)
         response.raise_for_status()
         result = response.json()
         while follow_cursor and (cursor := result.get("nextCursor")):
             data["cursor"] = cursor
             another_response = self._make_request(method, url, data)
             another_response.raise_for_status()
             another_result = another_response.json()
             result["items"].extend(another_result["items"])
             result["nextCursor"] = another_result.get("nextCursor")
         with suppress(KeyError):
             del result["nextCursor"]
             del result["cursor"]
+        logger.debug(f"{method} to {url}\ndata:\n{pformat(data)}\nresult:\n{pformat(result)}")
         return result
 
     def _make_request(
         self, method: Literal["GET", "POST"], url: str, data: Optional[Dict[str, Any]] = None
     ) -> Response:
         if data is not None:
             data = data.copy()
```

### Comparing `cognite_gql_pygen-0.4.0/cognite/dm_clients/cdf/data_classes_dm_v3.py` & `cognite_gql_pygen-0.4.1/cognite/dm_clients/cdf/data_classes_dm_v3.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.4.0/cognite/dm_clients/cdf/get_client.py` & `cognite_gql_pygen-0.4.1/cognite/dm_clients/cdf/get_client.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.4.0/cognite/dm_clients/custom_types/jsonobject.py` & `cognite_gql_pygen-0.4.1/cognite/dm_clients/custom_types/jsonobject.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.4.0/cognite/dm_clients/custom_types/timestamp.py` & `cognite_gql_pygen-0.4.1/cognite/dm_clients/custom_types/timestamp.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.4.0/cognite/dm_clients/domain_modeling/domain_client.py` & `cognite_gql_pygen-0.4.1/cognite/dm_clients/domain_modeling/domain_client.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.4.0/cognite/dm_clients/domain_modeling/domain_model.py` & `cognite_gql_pygen-0.4.1/cognite/dm_clients/domain_modeling/domain_model.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 
 import logging
 from typing import Dict, Optional, Type, get_args
 
 import strawberry
-from pydantic import Extra
+from pydantic import Extra, PrivateAttr
+from typing_extensions import Self
 
 from cognite.dm_clients.cdf.data_classes_dm_v3 import DataModelBase
 
 __all__ = [
     "DomainModel",
 ]
 
@@ -23,22 +24,39 @@
     A bit of nomenclature: instances of DomainModel we call "items".
     This is pretty much because all other words I can think of have been taken by DM >:]
 
     Even this is confusing... A data model in DM is a collection of domain models.
     """
 
     externalId: strawberry.Private[Optional[str]] = None
-    # Private ^ means the field will not be exposed in GraphQL schema
-    # Used here because actual objects (returned from the API) have these fields. These are "implicit" field.
+    _reference: strawberry.Private[bool] = PrivateAttr(False)
+    # strawberry.Private ^ means the field will not be exposed in GraphQL schema
+    # Used on externalID because actual objects (returned from the API) have these fields. These are "implicit" field.
+    # PrivateAttr is telling pydantic to allow the use of this as a regular (non-pydantic) attribute.
 
     class Config:
         extra = Extra.forbid
         #  ^ raises exception if extra fields are passed to the constructor. Very useful for development.
         arbitrary_types_allowed = True
 
+    def __init__(self, *args, _reference: bool = False, **kwargs):
+        if _reference:
+            for field_name, field in self.__fields__.items():
+                if field.required and field_name not in kwargs:
+                    kwargs[field_name] = field.type_()
+        super().__init__(*args, **kwargs)
+        self._reference = _reference
+
+    def as_reference(self) -> Self:
+        return type(self)(externalId=self.externalId, _reference=True)
+
+    @classmethod
+    def ref(cls, externalId: str):  # noqa: N803
+        return cls(externalId=externalId, _reference=True)
+
     @classmethod
     def get_one_to_many_attrs(cls) -> Dict[str, Type[DomainModel]]:
         """
         Get attributes which describe one-to-many relationships.
         These attributes usually require additional considerations with DM.
         """
         attrs = {}
```

### Comparing `cognite_gql_pygen-0.4.0/cognite/dm_clients/domain_modeling/domain_model_api.py` & `cognite_gql_pygen-0.4.1/cognite/dm_clients/domain_modeling/domain_model_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from __future__ import annotations
 
 import logging
 from collections import defaultdict
 from concurrent.futures import ThreadPoolExecutor
-from typing import Any, Dict, Generic, Iterable, List, Optional, Tuple, Type, TypeVar, get_args
+from typing import Any, Dict, Generic, Iterable, List, Optional, Set, Tuple, Type, TypeVar, get_args
 from uuid import uuid4
 
 from cognite.dm_clients.cdf.client_dm_v3 import EdgesAPI, NodesAPI
 from cognite.dm_clients.cdf.data_classes_dm_v3 import Node, View
 
 from .domain_client import DomainClient
 from .domain_model import DomainModel
-from .relationship_api import RelationshipAPI
+from .relationship_api import RelationshipAPI, RelationshipProxy
 
 __all__ = [
     "DomainModelAPI",
 ]
 
 
-_PendingEdgeT = Tuple[str, str, str]
+_PendingEdgeT = Tuple[str, str, str]  # attr, start_ext_id, end_ext_id
 
 logger = logging.getLogger(__name__)
 
 
 DomainModelT = TypeVar("DomainModelT", bound=DomainModel)
 
 
@@ -46,18 +46,20 @@
     ):
         self.domain_model = domain_model
         self.view = view
         self.nodes_api = nodes_api
         self.relationships = RelationshipAPI(
             edges_api,
             domain_model,
+            self,
             view,
             schema_version,
             space_id,
         )
+        self.connect = RelationshipProxy(self)
         # TODO it would make more sense to pass RelationshipAPI directly instead of EdgesAPI
         self.domain_client = domain_client
         self.space_id = space_id
         self.schema_version = schema_version
         self.api_version = api_version
 
         self.model_external_id: str = f"{domain_model.__name__}_{schema_version}"
@@ -88,32 +90,49 @@
         This is a multy-step job:
           0. Prepare the nodes - create random externalIDs if missing
           1. Create all nested nodes in new one-to-one relationships.
           2. Create all nested nodes in new one-to-many relationships.
           3. Create nodes.
           4. Create edges for those one-to-many relationships.
         """
+        if ref_items := [item for item in items if item._reference]:
+            raise ValueError(
+                f"References passed into {type(self).__name__}.apply(): {[item.externalId for item in ref_items]}"
+            )
+
         items = self._prepare_items(items, ext_id_prefix)
 
         if not items:
             return []
 
         with self.domain_client._cache_lock:
             self.domain_client.cache.delete_many(*[item.externalId for item in items if item.externalId])
 
         items = self._create_related_o2o_nodes(items)
         items, pending_edges = self._create_related_o2m_items(items)
 
         def _strip_items(item_data: dict) -> dict:
-            return {key: val for key, val in item_data.items() if val is not None}
+            o2m_attr = self.domain_model.get_one_to_many_attrs()
+            return {key: val for key, val in item_data.items() if val is not None and key not in o2m_attr}
+
+        def _make_ref(item_data: dict) -> dict:
+            """Represents one-to-one relationships in CDF DM."""
+            return {
+                "space": self.space_id,  # TODO item.space_id ?
+                "externalId": item_data["externalId"],
+            }
 
         def _properties_data(data: dict) -> dict:
             """strip out reserved keys"""
             reserved_keys = {"externalId"}
-            return {key: val for key, val in data.items() if key not in reserved_keys}
+            return {
+                key: _make_ref(val) if key in self.domain_model.get_one_to_one_attrs() else val
+                for key, val in data.items()
+                if key not in reserved_keys
+            }
 
         def _make_node(data: dict) -> Node:
             return Node(
                 version=str(self.schema_version),
                 space=self.space_id,
                 externalId=data["externalId"],
                 properties={
@@ -124,16 +143,16 @@
             )
 
         created_nodes = [_make_node(_strip_items(item.dict(by_alias=True, exclude_defaults=False))) for item in items]
         self.nodes_api.apply(self.view, nodes=created_nodes)
 
         self._create_related_o2m_edges(pending_edges)
 
-        full_items = self._retrieve_full(created_nodes)
-        return full_items
+        self._cache_created_items(items)
+        return items
 
     def _create_related_o2o_nodes(self, items: List[DomainModelT]) -> List[DomainModelT]:
         """
         Create related nodes that are in a one-to-one relationship with nodes in `items`.
         Replace relevant attributes on individual `items` with references to the created nodes (API understands
         references and not nested objects).
         """
@@ -146,25 +165,16 @@
                 subitem_type = item.__fields__[attr].type_
                 # TODO check:
                 while type_args := get_args(subitem_type):
                     # type is wrapped in `Optional[]`
                     # TODO check that it's actually "Optional" and not something else!
                     subitem_type = type_args[0]
 
-                new_subitems: List[DomainModel] = self.domain_client.apply(
-                    [attr_value],
-                    ext_id_prefix=f"{item.externalId}__",
-                )
-                if not new_subitems:
-                    raise ValueError("attr_value empty, but it should have been created just now.")  # keeps mypy happy
-                attr_value = new_subitems[0]
-
-                # replace nested objects with externalId references:
-                ref_to_subitem = {"space": self.space_id, "externalId": attr_value.externalId}
-                setattr(item, attr, ref_to_subitem)
+                if not attr_value._reference:
+                    self.domain_client.apply([attr_value], ext_id_prefix=f"{item.externalId}__")
         return items
 
     def _create_related_o2m_items(
         self, items: List[DomainModelT]
     ) -> Tuple[List[DomainModelT], Dict[str, List[_PendingEdgeT]]]:
         """
         Create related nodes that are in a one-to-many relationship with the current item(s). Also prepare a list of
@@ -179,20 +189,18 @@
             for attr, attr_value in list(item):
                 if not attr_value or attr not in o2m_edge_attrs:
                     continue
 
                 # We need to:
                 #   1. create related nodes
                 #   2. (after everything else is created) create Edge instances that point to those related nodes
-
-                # clear the attribute value:
-                setattr(item, attr, None)
-
-                created_subitems = self.domain_client.apply(attr_value, ext_id_prefix=f"{item.externalId}__")
-                for subitem in created_subitems:
+                all_subitems = attr_value
+                full_subitems = [subitem for subitem in all_subitems if not subitem._reference]
+                self.domain_client.apply(full_subitems, ext_id_prefix=f"{item.externalId}__")
+                for subitem in all_subitems:
                     pending_edges[attr].append((attr, item.externalId, subitem.externalId))
         return items, pending_edges
 
     def _create_related_o2m_edges(self, pending_edges: Dict[str, List[_PendingEdgeT]]):
         """
         All the nodes have been created at this point, now create the edges between them.
         """
@@ -212,27 +220,74 @@
     def _cache_created_items(self, items: Iterable[DomainModelT]) -> None:
         """
         This caching is not just for performance! It also helps with CDF's "eventual consistency" promise.
         Without this cache, what happens is that we create a node (i.e. a DomainModel instance) and if we want to
         retrieve that same instance very soon, it often just isn't present in the response. After some time (seconds,
         sometimes minutes?) the new node appears in CDF.
         """
-        with self.domain_client._cache_lock:
-            self.domain_client.cache.set_many({item.externalId: item for item in items if item.externalId})
+        for item in (item_ for item_ in items if item_.externalId and not item_._reference):
+            # replace related items with reference dicts
+            # ... one-to-many:
+            o2m_subitems: Dict[str, Iterable[DomainModelT]] = {}
+            for attr in item.get_one_to_many_attrs():
+                o2m_subitems[attr] = getattr(item, attr, None) or []
+                if o2m_subitems[attr]:
+                    self._cache_created_items(o2m_subitems[attr])
+                    setattr(
+                        item,
+                        attr,
+                        [{"space": self.space_id, "externalId": subitem.externalId} for subitem in o2m_subitems[attr]],
+                    )
+            # ... one-to-one:
+            o2o_subitems: Dict[str, Optional[DomainModelT]] = {}
+            for attr in item.get_one_to_one_attrs():
+                subitem = getattr(item, attr, None)
+                o2o_subitems[attr] = subitem
+                if subitem is not None:
+                    self._cache_created_items([subitem])
+                    setattr(item, attr, {"space": self.space_id, "externalId": subitem.externalId})
+            # save to cache:
+            if item.externalId:
+                self.domain_client.cache.set(item.externalId, item)
+            # restore replaced attributes:
+            for attr in o2m_subitems:
+                setattr(item, attr, o2m_subitems[attr])
+            for attr in o2o_subitems:
+                setattr(item, attr, o2o_subitems[attr])
 
     def _get_from_cache(self, external_ids: Iterable[str]) -> Tuple[List[DomainModelT], List[str]]:
         cached_items: List[DomainModelT] = []
-        uncached_external_ids: List[str] = []
+        uncached_external_ids: Set[str] = set()
         for external_id in external_ids:
+            # retrieve item from cache:
             cached_instance: DomainModelT = self.domain_client.cache.get(external_id)
             if cached_instance is not None:
-                cached_items.append(cached_instance)
+                # retrieve related items from cache:
+                # ... one-to-many:
+                for attr in cached_instance.get_one_to_many_attrs():
+                    subitem_ext_ids = [ref["externalId"] for ref in getattr(cached_instance, attr, None) or []]
+                    cached_subs, uncached_sub_ids = self._get_from_cache(subitem_ext_ids)
+                    if uncached_sub_ids:
+                        uncached_external_ids.add(external_id)
+                        break
+                    setattr(cached_instance, attr, cached_subs)
+                # ... one-to-one:
+                for attr in cached_instance.get_one_to_one_attrs():
+                    subitem_ext_id = (getattr(cached_instance, attr, None) or {}).get("externalId")
+                    cached_subs, uncached_sub_ids = self._get_from_cache([subitem_ext_id] if subitem_ext_id else [])
+                    if uncached_sub_ids:
+                        uncached_external_ids.add(external_id)
+                        break
+                    setattr(cached_instance, attr, cached_subs[0] if cached_subs else None)
+                # consider this item "cached" only if all its subitems are also cached:
+                if cached_instance.externalId not in uncached_external_ids:
+                    cached_items.append(cached_instance)
             else:
-                uncached_external_ids.append(external_id)
-        return cached_items, uncached_external_ids
+                uncached_external_ids.add(external_id)
+        return cached_items, list(uncached_external_ids)
 
     def list(self, limit=25, resolve_relationships=True) -> List[DomainModelT]:
         nodes = self.nodes_api.list(self.view, limit=limit)
         if resolve_relationships:
             items = self._retrieve_full(nodes)
         else:
             items = self._retrieve_wo_rels(nodes)
@@ -269,15 +324,15 @@
         external_ids = list({item.externalId for item in items if item.externalId})
         self.nodes_api.delete(self.space_id, external_ids)
         with self.domain_client._cache_lock:
             self.domain_client.cache.delete_many(*external_ids)
 
     def _retrieve_full(self, nodes: Iterable[Node]) -> List[DomainModelT]:
         """
-        For every node, make a fully DomainModel item, including all nested (related) objects.
+        For every node, make a full DomainModel item, including all nested (related) objects.
         """
         full_items: Dict[str, DomainModelT]
         uncached_nodes: List[Node]
 
         # 1: retrieve nodes from cache
 
         cached_items, uncached_external_ids = self._get_from_cache([node.externalId for node in nodes])
@@ -332,15 +387,16 @@
         for node in uncached_nodes:
             item = self._make_item_from_node(node)
             if not item.externalId:
                 raise ValueError("Unexpected empty externalId!")
             full_items[item.externalId] = item
 
         items = list(full_items.values())
-        self._cache_created_items(items)
+        with self.domain_client._cache_lock:
+            self._cache_created_items(items)
         return items
 
     def _retrieve_wo_rels(self, nodes: Iterable[Node]) -> List[DomainModelT]:
         """
         For every node make DomainModel item but set any relationship attributes to None.
         """
         # TODO Result should distinguish between unresolved relationships and legitimate `None` values?
```

### Comparing `cognite_gql_pygen-0.4.0/cognite/dm_clients/domain_modeling/schema.py` & `cognite_gql_pygen-0.4.1/cognite/dm_clients/domain_modeling/schema.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.4.0/cognite/dm_clients/misc.py` & `cognite_gql_pygen-0.4.1/cognite/dm_clients/misc.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.4.0/cognite/gqlpygen/data_classes.py` & `cognite_gql_pygen-0.4.1/cognite/gqlpygen/data_classes.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.4.0/cognite/gqlpygen/generator.py` & `cognite_gql_pygen-0.4.1/cognite/gqlpygen/generator.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.4.0/cognite/gqlpygen/main.py` & `cognite_gql_pygen-0.4.1/cognite/gqlpygen/main.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.4.0/cognite/gqlpygen/misc.py` & `cognite_gql_pygen-0.4.1/cognite/gqlpygen/misc.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.4.0/cognite/gqlpygen/parser.py` & `cognite_gql_pygen-0.4.1/cognite/gqlpygen/parser.py`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.4.0/cognite/gqlpygen/templates/client.txt` & `cognite_gql_pygen-0.4.1/cognite/gqlpygen/templates/client.txt`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.4.0/cognite/gqlpygen/templates/schema.txt` & `cognite_gql_pygen-0.4.1/cognite/gqlpygen/templates/schema.txt`

 * *Files identical despite different names*

### Comparing `cognite_gql_pygen-0.4.0/pyproject.toml` & `cognite_gql_pygen-0.4.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cognite-gql-pygen"
-version = "0.4.0"
+version = "0.4.1"
 description = "Cognite graphQL Python generation SDK"
 readme = "README.md"
 authors = ["Cognite <support@cognite.com>"]
 
 packages = [{ include="cognite", from="." }]
 exclude = ["cognite/dm_clients/*.toml"]
 
@@ -40,14 +40,15 @@
 cachelib = "^0.10.2"
 retry = "^0.9.2"
 loguru = "^0.6.0"
 dynaconf = "^3.1.12"
 graphql-core = ">=3.2"
 Jinja2 = ">=3.1"
 packaging = "^23.1"
+typing-extensions = "^4.5.0"
 
 [tool.poetry.dev-dependencies]
 twine = "*"
 pre-commit = "*"
 toml = "*"
 python-dotenv = "*"
 pytest = "*"
```

### Comparing `cognite_gql_pygen-0.4.0/PKG-INFO` & `cognite_gql_pygen-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cognite-gql-pygen
-Version: 0.4.0
+Version: 0.4.1
 Summary: Cognite graphQL Python generation SDK
 Author: Cognite
 Author-email: support@cognite.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -21,14 +21,15 @@
 Requires-Dist: msal (>=1.16.0,<2.0.0)
 Requires-Dist: numpy (>=1.23.2,<2.0.0)
 Requires-Dist: packaging (>=23.1,<24.0)
 Requires-Dist: pydantic (>=1.10)
 Requires-Dist: retry (>=0.9.2,<0.10.0)
 Requires-Dist: strawberry-graphql (>=0.156.4,<0.157.0)
 Requires-Dist: typer[all]
+Requires-Dist: typing-extensions (>=4.5.0,<5.0.0)
 Description-Content-Type: text/markdown
 
 Cognite GraphQL Python Generator
 ==========================
 [![build](https://github.com/cognitedata/cognite-gql-pygen/actions/workflows/release.yaml/badge.svg)](https://github.com/cognitedata/cognite-gql-pygen/actions/workflows/release.yaml)
 [![GitHub](https://img.shields.io/github/license/cognitedata/cognite-gql-pygen)](https://github.com/cognitedata/cognite-gql-pygen/blob/master/LICENSE)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
```

