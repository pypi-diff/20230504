# Comparing `tmp/penne-0.3.9.tar.gz` & `tmp/penne-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "penne-0.3.9.tar", last modified: Fri Mar  3 20:27:55 2023, max compression
+gzip compressed data, was "penne-0.4.0.tar", last modified: Thu May  4 16:21:34 2023, max compression
```

## Comparing `penne-0.3.9.tar` & `penne-0.4.0.tar`

### file list

```diff
@@ -1,12 +1,7 @@
--rw-r--r--   0        0        0     3118 2023-02-23 17:19:56.260855 penne-0.3.9/.gitignore
--rw-r--r--   0        0        0     1101 2022-07-26 21:32:06.694759 penne-0.3.9/LICENSE
--rw-r--r--   0        0        0     4951 2022-07-27 16:10:53.985946 penne-0.3.9/README.md
--rw-r--r--   0        0        0      606 2023-03-03 20:27:51.495849 penne-0.3.9/penne/__init__.py
--rw-r--r--   0        0        0     1960 2023-03-02 18:53:25.335169 penne-0.3.9/penne/client.py
--rw-r--r--   0        0        0     9814 2023-03-02 18:54:41.999758 penne-0.3.9/penne/core.py
--rw-r--r--   0        0        0    26505 2023-03-03 20:24:19.820632 penne-0.3.9/penne/delegates.py
--rw-r--r--   0        0        0     5694 2023-03-02 18:55:20.767636 penne-0.3.9/penne/handlers.py
--rw-r--r--   0        0        0      629 2023-02-24 18:18:56.116031 penne-0.3.9/pyproject.toml
--rw-r--r--   0        0        0     8036 2023-02-23 17:18:22.179813 penne-0.3.9/test_plottyn.py
--rw-r--r--   0        0        0      978 2023-03-02 18:56:21.281831 penne-0.3.9/test_server_conformance.py
--rw-r--r--   0        0        0     5484 1970-01-01 00:00:00.000000 penne-0.3.9/PKG-INFO
+-rw-r--r--   0        0        0     5781 2023-05-04 16:21:24.833092 penne-0.4.0/README.md
+-rw-r--r--   0        0        0      564 2023-05-04 16:21:24.837092 penne-0.4.0/penne/__init__.py
+-rw-r--r--   0        0        0    10169 2023-05-04 16:21:24.837092 penne-0.4.0/penne/core.py
+-rw-r--r--   0        0        0    27611 2023-05-04 16:21:24.837092 penne-0.4.0/penne/delegates.py
+-rw-r--r--   0        0        0     5470 2023-05-04 16:21:24.837092 penne-0.4.0/penne/handlers.py
+-rw-r--r--   0        0        0      737 2023-05-04 16:21:24.837092 penne-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     6516 1970-01-01 00:00:00.000000 penne-0.4.0/PKG-INFO
```

### Comparing `penne-0.3.9/README.md` & `penne-0.4.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,15 @@
 # PENNE
+
+![Build Status](https://github.com/InsightCenterNoodles/Penne/workflows/CI/badge.svg)
+![PyPI](https://img.shields.io/pypi/v/Penne)
+![Coverage](tests/coverage/coverage.svg)
+![Coverage](https://github.com/InsightCenterNoodles/Penne/raw/aebac0f/coverage-badge/coverage.svg)
+
+
 Python Client for NOODLES protocol  
 (Python Encoded Native NOODLES Endpoint)
 
 ## Description
 The client library is based on the NOODLES messaging protocol for communicating with serverside data visualisation applications. The client uses a websocket connection to send CBOR encoded messages. To customize its implementation, the
 library offers hooks in the form of delegates classes which can be extended and overwritten.
 
@@ -67,14 +74,28 @@
 ## Getting Started
 1. Install the library
 ```python
 pip install penne
 ```
 2. Create a client using `create_client(address, delegate_hash)`
 ```python
-client: penne.Client = penne.create_client("ws://localhost:50000")
+from penne import Client
+
+with Client(address, delegate_hash) as client:
+    # do stuff
 ```
 - (Optional) use delegate hash to map custom delegates
-- Note: make sure to close client thread at some point - `client.thread.join()`
+- This is the recommended way to create a client as it will automatically close the connection when the client goes out of scope
+- It also manages an 'is_active' flag to signify whether the connection is open and the client is still running
+  - This can be used to poll for callbacks
+- However, you can also instantiate the client and manage the communication thread manually
+```python
+client = Client(address, delegate_hash)
+client.thread.start()  # Starts websocket connection in new thread
+client.connection_established.wait() 
+# do stuff
+client.shutdown()  # Close websocket connection
+client.thread.join()
+```
 3. Explore and manipulate data on the server using client or delegate methods
 - call `show_methods()` on the client to see a list of available methods with documentation
 - call `show_methods()` on a delegate to see a list of available methods for that instance
```

### Comparing `penne-0.3.9/penne/core.py` & `penne-0.4.0/penne/core.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,23 @@
 """Module with Core Implementation of Client"""
 
 from __future__ import annotations
 from typing import Any, List, Type
+
+import queue
 import asyncio
-from queue import Queue
+import logging
+import threading
 
 import websockets
 from cbor2 import loads, dumps
 
 from . import handlers, delegates
 
 
-def uri_tag_hook(decoder, tag, shareable_index=None):
-    """Hook for URI CBOR Tag"""
-
-    if tag.tag != 32:
-        return tag
-    else:
-        return tag.value
-
-
 class HandleInfo(object):
     """Class to organize useful info for processing each type of message
 
     Attributes:
         specifier (str) : keyword for delegate and state maps
         action (str)    : action performed by message
     """
@@ -33,63 +27,63 @@
         self.action = action
 
 
 class Client(object):
     """Client for communicating with server
 
     Attributes:
-        _url (string): 
+        _url (string):
             address used to connect to server
-        _loop (event loop): 
+        _loop (event loop):
             event loop used for network thread
-        delegates (dict): 
+        delegates (dict):
             map for delegate functions
-        thread (thread object): 
+        thread (thread object):
             network thread used by client
-        _socket (WebSocketClientProtocol): 
+        _socket (WebSocketClientProtocol):
             socket to connect to server
-        name (str): 
+        name (str):
             name of the client
-        state (dict): 
+        state (dict):
             dict keeping track of created objects
-        client_message_map (dict): 
+        client_message_map (dict):
             mapping message type to corresponding id
         server_messages (dict):
             mapping message id's to handle info
         _current_invoke (str):
             id for next method invoke
-        callback_map (dict): 
+        callback_map (dict):
             mapping invoke_id to callback function
     """
 
-    def __init__(self, url: str, loop, custom_delegate_hash: dict[str, Type[delegates.Delegate]],
-                 on_connected, callback_queue: Queue, strict=False):
+    def __init__(self, url: str, custom_delegate_hash: dict[str, Type[delegates.Delegate]] = None,
+                 on_connected=None, strict=False):
         """Constructor for the Client Class
 
         Args:
             url (string):
                 address used to connect to server
-            loop (event loop): 
-                event loop used for network thread
-            custom_delegate_hash (dict): 
+            custom_delegate_hash (dict):
                 map for new delegate methods
             on_connected (Callable):
                 callback function to run once client is set up
-            callback_queue (Queue):
-                queue to store callbacks
             strict (bool):
                 flag for strict data validation and throwing hard exceptions
         """
 
+        if not custom_delegate_hash:
+            custom_delegate_hash = {}
+
         self._url = url
-        self._loop = loop
+        self._loop = asyncio.new_event_loop()
         self.on_connected = on_connected
         self.delegates = {}
         self.strict = strict
-        self.thread = None
+        self.thread = threading.Thread(target=self.start_communication_thread)
+        self.connection_established = threading.Event()
         self._socket = None
         self.name = "Python Client"
         self.state = {}
         self.client_message_map = {
             "intro": 0,
             "invoke": 1
         }
@@ -129,28 +123,49 @@
             HandleInfo("document", "reset"),  
             HandleInfo("signals", "invoke"),  
             HandleInfo("methods", "reply"),
             HandleInfo("document", "initialized")
         ]
         self._current_invoke = 0
         self.callback_map = {}
-        self.callback_queue = callback_queue
-        self.is_shutdown = False
+        self.callback_queue = queue.Queue()
+        self.is_active = False
 
         # Hook up delegate map to default or custom based on input hash
         defaults = delegates.default_delegates
         for key in defaults:
             if key not in custom_delegate_hash:
                 self.delegates[key] = defaults[key]
             else:
                 self.delegates[key] = custom_delegate_hash[key]
 
         # Add document delegate as starting element in state
         self.state["document"] = self.delegates["document"](client=self)
 
+    def __enter__(self):
+        """Enter method for context manager"""
+        self.thread.start()
+        self.connection_established.wait()
+        self.is_active = True
+        return self
+
+    def __exit__(self, exc_type, exc_value, traceback):
+        """Exit method for context manager"""
+        self.shutdown()
+        self.is_active = False
+        self.thread.join()
+
+    def start_communication_thread(self):
+        """Starts the communication thread for the client"""
+        try:
+            asyncio.set_event_loop(self._loop)
+            self._loop.run_until_complete(self.run())
+        except Exception as e:
+            logging.warning(f"Connection terminated in communication thread: {e}")
+
     def object_from_name(self, name: str) -> List[int]:
         """Get a delegate's id from its name
 
         Args:
             name (str): name of method
 
         Returns:
@@ -163,15 +178,15 @@
         for delegate in state_delegates:
             if delegate.name == name:
                 return delegate.id
         raise Exception(f"Couldn't find object '{name}' in state")
 
     def get_component(self, component_id):
         """Getter to easily retrieve components from state
-        
+
         Args:
             component_id (ID): id for the component
 
         Returns:
             Component delegate from state
         """
 
@@ -232,56 +247,50 @@
         Args:
             message_dict (dict): dict mapping message attribute to value
             kind (str): either 'invoke' or 'intro' to indicate type of client message
         """
 
         # Construct message with ID from map and converted message object
         message = [self.client_message_map[kind], message_dict]
-        print(f"Sending Message: {message}")
+        logging.debug(f"Sending Message: {message}")
         
         asyncio.run_coroutine_threadsafe(self._socket.send(dumps(message)), self._loop)
 
     async def run(self):
         """Network thread for managing websocket connection"""  
 
         async with websockets.connect(self._url) as websocket:
 
             # update class
             self._socket = websocket
             self.name = f"Python Client @ {self._url}"
+            self.connection_established.set()
+            self.is_active = True
 
             # send intro message
             intro = {"client_name": self.name}
             self.send_message(intro, "intro")
 
             # decode, iterate over, and handle all incoming messages
             async for message in self._socket:
-                raw_message = loads(message, tag_hook=uri_tag_hook)
+                raw_message = loads(message)
                 iterator = iter(raw_message)
                 for tag in iterator:
                     try:
                         handlers.handle(self, tag, next(iterator))
                     except Exception as e:
                         if self.strict:
                             raise e
                         else:
-                            print(f"Exception: {e}")
+                            logging.error(f"Exception: {e} for message {raw_message}")
 
     def show_methods(self):
         """Displays Available Methods to the User"""
-
-        print("\n-- Available Methods to call --")
-        print("client.invoke_method(method_name, args, optional callback function)")
-        print("-------------------------------------------------------------------")
-        for method in self.state["methods"].values():
-            if "noo::" not in method.name:
-                print(method)
+        self.state["document"].show_methods()
 
     def shutdown(self):
         """Method for shutting down the client
         
         Closes websocket connection then blocks to finish all callbacks
         """
-        
         asyncio.run_coroutine_threadsafe(self._socket.close(), self._loop)
-        self.is_shutdown = True
-    
+        self.is_active = False
```

### Comparing `penne-0.3.9/penne/delegates.py` & `penne-0.4.0/penne/delegates.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 """Collection of Noodles Objects
 
 Follows the specification in the cddl document, and
 implements strict validation
 """
 
 from __future__ import annotations
-from typing import Literal, Optional, Any, Union, Callable, List
+
+import logging
+from typing import Literal, Optional, Any, Union, Callable, List, Tuple
 from collections import namedtuple
 from enum import Enum
 from math import pi
-import warnings
 
-from pydantic import BaseModel, root_validator, Extra, ValidationError, validator
+from pydantic import BaseModel, root_validator, Extra, validator
 from pydantic.color import Color
 
 
 """ =============================== ID's ============================= """
 
 IDGroup = namedtuple("IDGroup", ["slot", "gen"])
 
@@ -119,22 +120,20 @@
     """Parent class for all delegates
     
     Defines general methods that should be available for all delegates
     
     Attributes:
         client (Client): Client delegate is attached to
         signals (dict): Signals that can be called on delegate, method name to callable
-        public_methods (list): Specify public methods, used in show_methods()
     """
 
-    client: Client
+    client: object = None
     id: ID = None
     name: Optional[str] = "No-Name Delegate"
     signals: Optional[dict] = {}
-    public_methods: Optional[List] = []
 
     def __repr__(self):
         return f"{self.name} | {type(self)} | {self.id}"
 
     # For all except Document Delegate
     def on_new(self, message: dict):
         pass
@@ -143,32 +142,23 @@
     def on_update(self, message: dict):
         pass
 
     # For all except Document Delegate
     def on_remove(self, message: dict):
         pass
 
-    def show_methods(self):
-        """Show methods available on this delegate"""
-
-        print(f"-- Methods on {self} --")
-        print("--------------------------------------")
-        for name in self.public_methods:
-            method = getattr(self, name)
-            print(f">> '{name}'\n{method.__doc__}")
-
 
 """ ====================== Common Definitions ====================== """
 
-Vec3 = tuple[float, float, float]
-Vec4 = tuple[float, float, float, float]
-Mat3 = tuple[float, float, float,
+Vec3 = Tuple[float, float, float]
+Vec4 = Tuple[float, float, float, float]
+Mat3 = Tuple[float, float, float,
              float, float, float,
              float, float, float]
-Mat4 = tuple[float, float, float, float,
+Mat4 = Tuple[float, float, float, float,
              float, float, float, float,
              float, float, float, float,
              float, float, float, float]
 
 
 class AttributeSemantic(Enum):
     position = "POSITION"
@@ -202,18 +192,14 @@
 
 class SamplerMode(Enum):
     clamp_to_edge = "CLAMP_TO_EDGE"
     mirrored_repeat = "MIRRORED_REPEAT"
     repeat = "REPEAT"
 
 
-class URL(NoodleObject):
-    url: str
-
-
 class SelectionRange(NoodleObject):
     key_from_inclusive: int
     key_to_exclusive: int
 
 
 class Selection(NoodleObject):
     name: str
@@ -273,15 +259,16 @@
     metal_rough_texture: Optional[TextureRef] = None  # assume linear, ONLY RG used
 
     @validator("base_color", pre=True)
     def check_color(cls, value):
 
         # Raise warning if format is wrong
         if len(value) != 4:
-            warnings.warn(f"Base Color is Wrong Color Format: {value}")
+            logging.warning(f"Base Color is Wrong Color Format: {value}")
+        return value
 
 
 class PointLight(NoodleObject):
     range: float = -1.0
 
 
 class SpotLight(NoodleObject):
@@ -433,14 +420,23 @@
     plots: Optional[List[PlotID]] = None
     tags: Optional[List[str]] = None
     methods_list: Optional[List[MethodID]] = None
     signals_list: Optional[List[SignalID]] = None
 
     influence: Optional[BoundingBox] = None
 
+    def show_methods(self):
+        """Show methods available on the entity"""
+
+        print(f"-- Methods on {self.name} --")
+        print("--------------------------------------")
+        for method_id in self.methods_list:
+            method = self.client.get_component(method_id)
+            print(f">> {method}")
+
 
 class Plot(Delegate):
     id: PlotID
     name: Optional[str] = "Unnamed Plot Delegate"
 
     table: Optional[TableID] = None
 
@@ -453,14 +449,23 @@
     @root_validator
     def one_of(cls, values):
         if bool(values['simple_plot']) != bool(values['url_plot']):
             return values
         else:
             raise ValueError("One plot type must be specified")
 
+    def show_methods(self):
+        """Show methods available on the entity"""
+
+        print(f"-- Methods on {self.name} --")
+        print("--------------------------------------")
+        for method_id in self.methods_list:
+            method = self.client.get_component(method_id)
+            print(f">> {method}")
+
 
 class Buffer(Delegate):
     id: BufferID
     name: Optional[str] = "Unnamed Buffer Delegate"
     size: int = None
 
     inline_bytes: bytes = None
@@ -479,24 +484,26 @@
     name: Optional[str] = "Unnamed Buffer-View Delegate"
     source_buffer: BufferID
 
     type: Literal["UNK", "GEOMETRY", "IMAGE"] = "UNK"
     offset: int
     length: int
 
-    # @validator("type")
-    # def coerce_type(cls, value):
-    #     if "UNK" in value:
-    #         return "UNK"
-    #     elif "GEOMETRY" in value:
-    #         return "GEOMETRY"
-    #     elif "IMAGE" in value:
-    #         return "IMAGE"
-    #     else:
-    #         raise ValidationError
+    @validator("type", pre=True)
+    def coerce_type(cls, value):
+        if value in ["UNK", "GEOMETRY", "IMAGE"]:
+            return value
+
+        logging.warning(f"Buffer View Type does not meet the specification: {value} coerced to 'UNK'")
+        if "GEOMETRY" in value:
+            return "GEOMETRY"
+        elif "IMAGE" in value:
+            return "IMAGE"
+        else:
+            return "UNK"
 
 
 class Material(Delegate):
     id: MaterialID
     name: Optional[str] = "Unnamed Material Delegate"
 
     pbr_info: Optional[PBRInfo] = PBRInfo()
@@ -559,15 +566,15 @@
     directional: DirectionalLight = None
 
     @validator("color", pre=True)
     def check_color(cls, value):
 
         # Raise warning if format is wrong
         if len(value) != 3:
-            warnings.warn(f"Color is Wrong Color Format in Light: {value}")
+            logging.warning(f"Color is Wrong Color Format in Light: {value}")
 
         return value
 
     @root_validator
     def one_of(cls, values):
         already_found = False
         for field in ['point', 'spot', 'directional']:
@@ -631,15 +638,15 @@
                 Server response to subscribe which has columns, keys, data, 
                 and possibly selections
         """
 
         # Extract data from init info and transpose rows to cols
         row_data = init_info["data"]
         cols = init_info["columns"]
-        print(f"Table Initialized with cols: {cols} and row data: {row_data}")
+        logging.debug(f"Table Initialized with cols: {cols} and row data: {row_data}")
 
     def _reset_table(self):
         """Reset dataframe and selections to blank objects
 
         Method is linked to 'tbl_reset' signal
         """
 
@@ -650,42 +657,42 @@
 
         Method is linked to 'tbl_rows_removed' signal
 
         Args:
             key_list (list): list of keys corresponding to rows to be removed
         """
 
-        print(f"Removed Rows: {key_list}...\n")
+        logging.debug(f"Removed Rows: {key_list}...\n")
 
     def _update_rows(self, keys: List[int], rows: list):
         """Update rows in table
 
         Method is linked to 'tbl_updated' signal
 
         Args:
             keys (list): 
                 list of keys to update
             rows (list):
                 list of rows containing the values for each new row
         """
 
-        print(f"Updated Rows...{keys}\n")
+        logging.debug(f"Updated Rows...{keys}\n")
 
     def _update_selection(self, selection_obj: Selection):
         """Change selection in delegate's state to new selection object
 
         Method is linked to 'tbl_selection_updated' signal
 
         Args:
             selection_obj (Selection): 
                 obj with new selections to replace obj with same name
         """
 
         self.selections[selection_obj.name] = selection_obj
-        print(f"Made selection {selection_obj.name} = {selection_obj}")
+        logging.debug(f"Made selection {selection_obj.name} = {selection_obj}")
 
     def relink_signals(self):
         """Relink the signals for built-in methods
 
         These should always be linked, along with whatever is injected,
         so relink on new and on update messages
         """
@@ -816,34 +823,50 @@
                 list of keys to be in new selection
             on_done (function, optional): 
                 callback function called when complete
         """
 
         self.tbl_update_selection(on_done, name, {"rows": keys})
 
+    def show_methods(self):
+        """Show methods available on the table"""
+
+        print(f"-- Methods on {self.name} --")
+        print("--------------------------------------")
+        for method_id in self.methods_list:
+            method = self.client.get_component(method_id)
+            print(f">> {method}")
+
 
 class Document(Delegate):
     name: str = "Document"
 
-    methods_list: list[MethodID] = []
-    signals_list: list[SignalID] = []
+    methods_list: List[MethodID] = []
+    signals_list: List[SignalID] = []
 
     def on_update(self, message: dict):
         if "methods_list" in message:
             self.methods_list = [MethodID(*element) for element in message["methods_list"]]
         if "signals_list" in message:
             self.signals_list = [SignalID(*element) for element in message["signals_list"]]
 
-        self.public_methods = [self.client.get_component(id).name for id in self.methods_list]
-
     def reset(self):
         self.client.state = {}
         self.methods_list = []
         self.signals_list = []
 
+    def show_methods(self):
+        """Show methods available on the document"""
+
+        print(f"-- Methods on Document --")
+        print("--------------------------------------")
+        for method_id in self.methods_list:
+            method = self.client.get_component(method_id)
+            print(f">> {method}")
+
 
 """ ====================== Communication Objects ====================== """
 
 
 class Invoke(NoodleObject):
     id: SignalID
     context: Optional[InvokeIDType] = None  # if empty - document
@@ -899,15 +922,15 @@
     Buffer: BufferID,
     BufferView: BufferViewID,
     Document: None
 }
 
 
 class InjectedMethod(object):
-    """Class for representing injected method in delegate
+    """Class for representing injected method in delegate, context automatically set
 
     Attributes:
         method (method): method to be called
         injected (bool): attribute marking method as injected
     """
 
     def __init__(self, method_obj) -> None:
@@ -917,16 +940,17 @@
     def __call__(self, *args, **kwargs):
         self.method(*args, **kwargs)
 
 
 class LinkedMethod(object):
     """Class linking target delegate and method's delegate 
         
-    make a cleaner function call in injected method
-    
+    make a cleaner function call in injected method, its like setting the context automatically
+    This is what actually gets called for the injected method
+
     Attributes:
         _obj_delegate (delegate): 
             delegate method is being linked to
         _method_delegate (MethodDelegate): 
             the method's delegate 
     """
 
@@ -937,25 +961,29 @@
     def __call__(self, on_done=None, *arguments):
         self._method_delegate.invoke(self._obj_delegate, arguments, callback=on_done)
 
 
 def inject_methods(delegate: Delegate, methods: List[MethodID]):
     """Inject methods into a delegate class
 
+    Idea is to inject a method that is from the server to put int into a delegate.
+    Now it looks like the delegate has an instance method that actually calls what
+    is on the server. Context, is automatically taken care of by the linked method
+
     Args:
         delegate (Delegate):
             identifier for delegate to be modified
         methods (list): 
             list of method id's to inject
     """
 
     # Clear out old injected methods
     for field, value in delegate:
         if hasattr(value, "injected"):
-            print(f"Deleting: {field} in inject methods")
+            logging.debug(f"Deleting: {field} in inject methods")
             delattr(delegate, field)
 
     for method_id in methods:
 
         # Get method delegate and manipulate name to exclude noo::
         method = delegate.client.state[method_id]
         name = method.name[5:]
@@ -990,12 +1018,7 @@
     elif isinstance(delegate, Table):
         return {"table": delegate.id}
     elif isinstance(delegate, Plot):
         return {"plot": delegate.id}
     else:
         return None
 
-
-# Update forward refs where model -> client -> model ...
-from penne.core import Client
-for component in id_map:
-    component.update_forward_refs()
```

### Comparing `penne-0.3.9/penne/handlers.py` & `penne-0.4.0/penne/handlers.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from __future__ import annotations
 from typing import TYPE_CHECKING, Any
 if TYPE_CHECKING:
     from penne.core import Client
 
 import weakref
 import warnings
+import logging
 from pydantic import ValidationError
 
 from penne.delegates import Delegate, id_map, default_delegates
 from penne.delegates import TableID, PlotID, EntityID, ID
 
 
 # Helper Methods
@@ -22,24 +23,19 @@
             client to be updated
         message (Message): 
             message containing updates
         component_id (ID):
             ID of the component to be updated
     """
 
-    current_state = client.state[component_id]
-    for attribute, value in message.items():
-        current_attr = getattr(current_state, attribute)
-        attr_type = type(current_attr)
-        if isinstance(value, list):
-            setattr(current_state, attribute, attr_type(*value))
-        elif isinstance(value, dict):
-            setattr(current_state, attribute, attr_type(**value))
-        else:
-            setattr(current_state, attribute, value)
+    current_state = client.state[component_id].dict()
+    current_state.update(message)
+
+    delegate_type = type(client.state[component_id])
+    client.state[component_id] = delegate_type(**current_state)
 
 
 def delegate_from_context(client: Client, context: dict) -> Delegate:
     """Get delegate object from a context message object
     
     Args:
         client (Client): client to get delegate from
@@ -71,15 +67,15 @@
 
 def handle(client: Client, message_id, message: dict[str, Any]):
     """Handle message from server
 
     'Handle' uses the ID attached to message to get handling info, and uses this info 
     to take proper course of action with message. The function has 5 main sections 
     handling create, delete, and update messages along with signal invocation and reply
-    messages. For now all other communication messages are simply printed.
+    messages.
 
     'Handle' is also responsible for managing the client's state and working with the
     delegates in a couple of key ways. This function creates, deletes, and updates
     delegates as well as invoking methods on the delegates using signals.
 
     Args:
         client (Client): client receiving the message
@@ -88,24 +84,25 @@
     """
     
     # Process message using ID from dict
     handle_info = client.server_messages[message_id]
     action = handle_info.action
     specifier = handle_info.specifier
     id_type = id_map[default_delegates[specifier]]
-    print(f"Message: {action} {specifier}")
-    
+    logging.debug(f"Received Message: {action} {specifier} {message}")
+
     # Update state based on map info
     if action == "create":
 
         # Create instance of delegate
         reference = weakref.ref(client)
         reference_obj = reference()
         try:
             delegate: Delegate = client.delegates[specifier](client=reference_obj, **message)
+            delegate.client = client
             client.state[delegate.id] = delegate
             delegate.on_new(message)
         except ValidationError as e:
 
             warnings.warn(str(e))
 
             if client.strict:
@@ -153,19 +150,19 @@
         signal: Delegate = client.state[signal_id]
 
         # Determine the delegate the signal is being invoked on
         context = message.get("context")
         target_delegate = delegate_from_context(client, context)
 
         # Invoke signal attached to target delegate
-        print(f"Invoking {signal.name} w/ args: {signal_data}")
+        logging.debug(f"Invoking {signal.name} w/ args: {signal_data}")
         target_delegate.signals[signal.name](*signal_data)
 
     elif action == "initialized":
 
         if client.on_connected:
             client.callback_queue.put((client.on_connected, None))
 
     else:
         # Document reset messages
         client.state["document"].reset()
-        print("Document Reset")
+        logging.debug("Document Reset")
```

### Comparing `penne-0.3.9/PKG-INFO` & `penne-0.4.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,36 @@
 Metadata-Version: 2.1
 Name: penne
-Version: 0.3.9
+Version: 0.4.0
 Summary: Python Client Library for NOODLES Protocol
 Keywords: noodles,cbor,Websockets,client,NOODLES
 Author: Alex Racapé
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Requires-Dist: websockets
 Requires-Dist: cbor2
 Requires-Dist: pydantic
+Requires-Dist: pytest ; extra == "testing"
+Requires-Dist: rigatoni ; extra == "testing"
+Requires-Dist: pandas ; extra == "testing"
+Requires-Dist: matplotlib ; extra == "testing"
 Project-URL: Source, https://github.com/InsightCenterNoodles/penne
+Provides-Extra: testing
 
 # PENNE
+
+![Build Status](https://github.com/InsightCenterNoodles/Penne/workflows/CI/badge.svg)
+![PyPI](https://img.shields.io/pypi/v/Penne)
+![Coverage](tests/coverage/coverage.svg)
+![Coverage](https://github.com/InsightCenterNoodles/Penne/raw/aebac0f/coverage-badge/coverage.svg)
+
+
 Python Client for NOODLES protocol  
 (Python Encoded Native NOODLES Endpoint)
 
 ## Description
 The client library is based on the NOODLES messaging protocol for communicating with serverside data visualisation applications. The client uses a websocket connection to send CBOR encoded messages. To customize its implementation, the
 library offers hooks in the form of delegates classes which can be extended and overwritten.
 
@@ -83,15 +95,29 @@
 ## Getting Started
 1. Install the library
 ```python
 pip install penne
 ```
 2. Create a client using `create_client(address, delegate_hash)`
 ```python
-client: penne.Client = penne.create_client("ws://localhost:50000")
+from penne import Client
+
+with Client(address, delegate_hash) as client:
+    # do stuff
 ```
 - (Optional) use delegate hash to map custom delegates
-- Note: make sure to close client thread at some point - `client.thread.join()`
+- This is the recommended way to create a client as it will automatically close the connection when the client goes out of scope
+- It also manages an 'is_active' flag to signify whether the connection is open and the client is still running
+  - This can be used to poll for callbacks
+- However, you can also instantiate the client and manage the communication thread manually
+```python
+client = Client(address, delegate_hash)
+client.thread.start()  # Starts websocket connection in new thread
+client.connection_established.wait() 
+# do stuff
+client.shutdown()  # Close websocket connection
+client.thread.join()
+```
 3. Explore and manipulate data on the server using client or delegate methods
 - call `show_methods()` on the client to see a list of available methods with documentation
 - call `show_methods()` on a delegate to see a list of available methods for that instance
```

