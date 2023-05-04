# Comparing `tmp/async_pjsekai-0.0.10.dev0.tar.gz` & `tmp/async_pjsekai-0.0.10.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async_pjsekai-0.0.10.dev0.tar", max compression
+gzip compressed data, was "async_pjsekai-0.0.10.dev1.tar", max compression
```

## Comparing `async_pjsekai-0.0.10.dev0.tar` & `async_pjsekai-0.0.10.dev1.tar`

### file list

```diff
@@ -1,12 +1,21 @@
--rw-r--r--   0        0        0      679 2023-04-30 12:42:40.730476 async_pjsekai-0.0.10.dev0/README.md
--rw-r--r--   0        0        0    25166 2023-04-29 12:18:24.696369 async_pjsekai-0.0.10.dev0/async_pjsekai/api.py
--rw-r--r--   0        0        0     2698 2023-04-27 03:52:06.469294 async_pjsekai-0.0.10.dev0/async_pjsekai/asset.py
--rw-r--r--   0        0        0     1133 2023-04-18 05:14:42.794216 async_pjsekai-0.0.10.dev0/async_pjsekai/asset_bundle.py
--rw-r--r--   0        0        0    38285 2023-04-29 12:20:19.906369 async_pjsekai-0.0.10.dev0/async_pjsekai/client.py
--rw-r--r--   0        0        0     1049 2023-04-27 03:52:06.449294 async_pjsekai-0.0.10.dev0/async_pjsekai/models/asset_bundle_info.py
--rw-r--r--   0        0        0     2622 2023-04-27 03:52:06.469294 async_pjsekai-0.0.10.dev0/async_pjsekai/models/converters.py
--rw-r--r--   0        0        0   109574 2023-04-27 03:52:08.579294 async_pjsekai-0.0.10.dev0/async_pjsekai/models/master_data.py
--rw-r--r--   0        0        0     1031 2023-04-29 11:31:04.476365 async_pjsekai-0.0.10.dev0/async_pjsekai/models/system_info.py
--rw-r--r--   0        0        0     1280 2023-04-18 05:14:42.854215 async_pjsekai-0.0.10.dev0/async_pjsekai/utilities.py
--rw-r--r--   0        0        0      859 2023-05-04 13:37:23.102709 async_pjsekai-0.0.10.dev0/pyproject.toml
--rw-r--r--   0        0        0     1834 1970-01-01 00:00:00.000000 async_pjsekai-0.0.10.dev0/PKG-INFO
+-rw-r--r--   0        0        0      679 2023-04-30 12:42:40.730476 async_pjsekai-0.0.10.dev1/README.md
+-rw-r--r--   0        0        0    25762 2023-05-04 16:57:48.864214 async_pjsekai-0.0.10.dev1/async_pjsekai/api.py
+-rw-r--r--   0        0        0     2711 2023-05-04 15:51:11.814207 async_pjsekai-0.0.10.dev1/async_pjsekai/asset.py
+-rw-r--r--   0        0        0     1133 2023-04-18 05:14:42.794216 async_pjsekai-0.0.10.dev1/async_pjsekai/asset_bundle.py
+-rw-r--r--   0        0        0    38661 2023-05-04 17:04:41.634214 async_pjsekai-0.0.10.dev1/async_pjsekai/client.py
+-rw-r--r--   0        0        0    23209 2023-05-04 16:57:48.834214 async_pjsekai-0.0.10.dev1/async_pjsekai/enums/enums.py
+-rw-r--r--   0        0        0      577 2023-05-04 16:57:48.494214 async_pjsekai-0.0.10.dev1/async_pjsekai/enums/information.py
+-rw-r--r--   0        0        0     2433 2023-05-04 16:57:48.534214 async_pjsekai-0.0.10.dev1/async_pjsekai/enums/platform.py
+-rw-r--r--   0        0        0     1593 2023-05-04 16:57:48.514214 async_pjsekai-0.0.10.dev1/async_pjsekai/enums/tutorial_status.py
+-rw-r--r--   0        0        0      847 2023-05-04 16:57:48.504214 async_pjsekai-0.0.10.dev1/async_pjsekai/enums/unknown.py
+-rw-r--r--   0        0        0     2205 2023-05-04 16:57:48.534214 async_pjsekai-0.0.10.dev1/async_pjsekai/exceptions.py
+-rw-r--r--   0        0        0     5914 2023-05-04 16:57:48.614214 async_pjsekai-0.0.10.dev1/async_pjsekai/live.py
+-rw-r--r--   0        0        0     1159 2023-05-04 16:48:32.164213 async_pjsekai-0.0.10.dev1/async_pjsekai/models/asset_bundle_info.py
+-rw-r--r--   0        0        0     2921 2023-05-04 16:57:48.564214 async_pjsekai-0.0.10.dev1/async_pjsekai/models/converters.py
+-rw-r--r--   0        0        0      680 2023-05-04 16:57:48.524214 async_pjsekai-0.0.10.dev1/async_pjsekai/models/game_version.py
+-rw-r--r--   0        0        0     1232 2023-05-04 16:57:48.544214 async_pjsekai-0.0.10.dev1/async_pjsekai/models/information.py
+-rw-r--r--   0        0        0   111626 2023-05-04 16:57:50.874214 async_pjsekai-0.0.10.dev1/async_pjsekai/models/master_data.py
+-rw-r--r--   0        0        0     1106 2023-05-04 16:48:32.164213 async_pjsekai-0.0.10.dev1/async_pjsekai/models/system_info.py
+-rw-r--r--   0        0        0     2023 2023-05-04 16:57:48.574214 async_pjsekai-0.0.10.dev1/async_pjsekai/utilities.py
+-rw-r--r--   0        0        0      896 2023-05-04 17:10:31.814215 async_pjsekai-0.0.10.dev1/pyproject.toml
+-rw-r--r--   0        0        0     1911 1970-01-01 00:00:00.000000 async_pjsekai-0.0.10.dev1/PKG-INFO
```

### Comparing `async_pjsekai-0.0.10.dev0/README.md` & `async_pjsekai-0.0.10.dev1/README.md`

 * *Files identical despite different names*

### Comparing `async_pjsekai-0.0.10.dev0/async_pjsekai/api.py` & `async_pjsekai-0.0.10.dev1/async_pjsekai/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,21 +8,21 @@
 from typing import Optional, Union
 from uuid import uuid4
 
 from aiohttp import ClientSession
 from aiohttp.http_exceptions import HttpProcessingError
 from jwt import encode as jwtEncode
 
-from pjsekai.models import GameVersion, AssetOS
+from async_pjsekai.models.game_version import GameVersion
 from async_pjsekai.models.system_info import SystemInfo
 from async_pjsekai.asset_bundle import AssetBundle
-from pjsekai.exceptions import UpdateRequired, SessionExpired, MissingJWTScecret
-from pjsekai.enums.tutorial_status import TutorialStatus
-from pjsekai.enums.platform import Platform
-from pjsekai.utilities import encrypt, decrypt, msgpack, unmsgpack
+from async_pjsekai.exceptions import UpdateRequired, SessionExpired, MissingJWTScecret
+from async_pjsekai.enums.tutorial_status import TutorialStatus
+from async_pjsekai.enums.platform import AssetOS, Platform
+from async_pjsekai.utilities import encrypt, decrypt, msgpack, unmsgpack
 
 
 class API:
     platform: Platform
     domains: dict[str, str]
     key: Optional[bytes]
     iv: Optional[bytes]
@@ -160,15 +160,15 @@
         server_number: Optional[int] = None,
     ) -> None:
         self.platform = platform
         self._session = ClientSession()
         self.key = key
         self.iv = iv
         self.jwt_secret = jwt_secret
-        self.system_info = SystemInfo.create()  # type: ignore
+        self.system_info = SystemInfo.create()
         if system_info is not None:
             self.system_info = system_info
         self.api_domain = api_domain
         self._asset_bundle_domain = asset_bundle_domain
         self._asset_bundle_info_domain = asset_bundle_info_domain
         self._game_version_domain = game_version_domain
         self._signature_domain = signature_domain
@@ -176,15 +176,15 @@
         self.enable_asset_bundle_encryption = enable_asset_bundle_encryption
         self.enable_asset_bundle_info_encryption = enable_asset_bundle_info_encryption
         self.enable_game_version_encryption = enable_game_version_encryption
         self.enable_signature_encryption = enable_signature_encryption
         self.server_number = server_number
 
         self._session_token = None
-        self.game_version = GameVersion()  # type: ignore
+        self.game_version = GameVersion().create()
 
     async def close(self):
         await self.session.close()
 
     def _pack(
         self, plaintext_dict: Optional[dict], enable_encryption: bool = True
     ) -> bytes:
@@ -250,22 +250,22 @@
             url,
             headers=self._generate_headers(system_info),
             data=self._pack(None, enable_signature_encryption),
         ) as response:
             response.raise_for_status()
             return response.headers["Set-Cookie"]
 
-    async def get_game_version(
+    async def get_game_version_packed(
         self,
         app_version: Optional[str] = None,
         app_hash: Optional[str] = None,
         game_version_domain: Optional[str] = None,
         enable_game_version_encryption: Optional[bool] = None,
         system_info: Optional[SystemInfo] = None,
-    ) -> dict:
+    ):
         if game_version_domain is None:
             game_version_domain = self.game_version_domain
         if enable_game_version_encryption is None:
             enable_game_version_encryption = self.enable_game_version_encryption
         if app_version is None:
             if system_info is None:
                 app_version = self.system_info.app_version
@@ -278,15 +278,33 @@
                 app_hash = system_info.app_hash
         url: str = f"https://{game_version_domain}/{app_version}/{app_hash}"
         async with self.session.get(
             url,
             headers=self._generate_headers(system_info),
         ) as response:
             response.raise_for_status()
-            return self._unpack(await response.read(), enable_game_version_encryption)
+            return self._decrypt(await response.read(), enable_game_version_encryption)
+
+    async def get_game_version(
+        self,
+        app_version: Optional[str] = None,
+        app_hash: Optional[str] = None,
+        game_version_domain: Optional[str] = None,
+        enable_game_version_encryption: Optional[bool] = None,
+        system_info: Optional[SystemInfo] = None,
+    ) -> dict:
+        return unmsgpack(
+            await self.get_game_version_packed(
+                app_version,
+                app_hash,
+                game_version_domain,
+                enable_game_version_encryption,
+                system_info,
+            )
+        )
 
     async def get_asset_bundle_info_packed(
         self,
         asset_version: Optional[str] = None,
         asset_bundle_info_domain: Optional[str] = None,
         enable_asset_bundle_info_encryption: Optional[bool] = None,
         system_info: Optional[SystemInfo] = None,
```

### Comparing `async_pjsekai-0.0.10.dev0/async_pjsekai/asset.py` & `async_pjsekai-0.0.10.dev1/async_pjsekai/asset.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from contextlib import asynccontextmanager
 from typing import Optional
 from pathlib import Path
 
 from async_pjsekai.api import API
 from async_pjsekai.models.asset_bundle_info import AssetBundleInfo
 
-from .models.converters import msgpack_converter
+from async_pjsekai.models.converters import msgpack_converter
 
 
 class Asset:
     _path: Optional[Path]
 
     @property
     def path(self) -> Optional[Path]:
```

### Comparing `async_pjsekai-0.0.10.dev0/async_pjsekai/asset_bundle.py` & `async_pjsekai-0.0.10.dev1/async_pjsekai/asset_bundle.py`

 * *Files identical despite different names*

### Comparing `async_pjsekai-0.0.10.dev0/async_pjsekai/client.py` & `async_pjsekai-0.0.10.dev1/async_pjsekai/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,32 +3,40 @@
 #
 # SPDX-License-Identifier: MIT
 
 from asyncio.locks import Lock
 from contextlib import asynccontextmanager
 import dataclasses
 from functools import wraps
-from typing import AsyncIterator, Coroutine, Callable, Optional, TypeVar
+from typing import AsyncIterator, Coroutine, Callable, Optional, TypeVar, Union
 from typing_extensions import ParamSpec, Concatenate
 from json import load, dump, JSONDecodeError
 from pathlib import Path
 
 from aiohttp.abc import AbstractCookieJar
 
+from async_pjsekai.enums.tutorial_status import TutorialStatus, Unit
 from async_pjsekai.models.master_data import MasterData
-from async_pjsekai.models.system_info import SystemInfo
-from pjsekai.models.asset_bundle_info import *
-from pjsekai.models.game_version import *
-from pjsekai.models.information import *
-from pjsekai.enums import *
-from async_pjsekai.api import API
+from async_pjsekai.models.system_info import SystemInfo, AppVersionStatus
+from async_pjsekai.models.game_version import GameVersion
+from async_pjsekai.models.information import Information
+from async_pjsekai.api import API, Platform
 from async_pjsekai.asset import Asset
-from pjsekai.exceptions import *
-from pjsekai.utilities import *
-from pjsekai.live import *
+from async_pjsekai.exceptions import (
+    AppUpdateRequired,
+    AssetUpdateRequired,
+    DataUpdateRequired,
+    MultipleUpdatesRequired,
+    NoAvailableVersions,
+    NotAuthenticatedException,
+    SessionExpired,
+    ServerInMaintenance,
+    UpdateRequired,
+)
+from async_pjsekai.live import SoloLive, LiveNotActive, LiveDead
 
 from .models.converters import msgpack_converter
 
 P = ParamSpec("P")
 R = TypeVar("R")
 
 
@@ -516,15 +524,17 @@
 
         if self.api_manager.key is None or self.api_manager.iv is None:
             return
 
         if self._system_info.app_version is None or self._system_info.app_hash is None:
             await self.update_app()
 
-        self.game_version = GameVersion(**await self.api_manager.get_game_version())
+        self.game_version = msgpack_converter.loads(
+            await self.api_manager.get_game_version_packed(), GameVersion
+        )
         if self._api_domain is not None:
             self.api_domain = self._api_domain
         else:
             if self.game_version.domain is not None:
                 self.api_domain = self.game_version.domain
             else:
                 self.api_domain = API.DEFAULT_API_DOMAIN
@@ -755,15 +765,15 @@
             return True
         except DataUpdateRequired as e:
             await self.update_data(e.data_version, e.app_version_status)
             return True
         return False
 
     async def refresh_signed_cookie(self) -> AbstractCookieJar:
-        cookies: Dict[str, str] = {
+        cookies: dict[str, str] = {
             k: v
             for k, v in (
                 cookie.split("=")
                 for cookie in (
                     c.strip()
                     for c in (await self.api_manager.get_signed_cookie()).split(";")
                 )
@@ -779,15 +789,15 @@
     async def ping(self) -> dict:
         return await self.api_manager.ping()
 
     @_auto_update
     @_auto_session_refresh
     async def get_notices(self) -> list[Information]:
         return [
-            Information(**information)
+            msgpack_converter.structure(information, Information)
             for information in (await self.api_manager.get_notices())["informations"]
         ]
 
     @_auto_update
     @_auth_required
     @_auto_session_refresh
     async def transfer_out(self, password: str) -> dict:
```

### Comparing `async_pjsekai-0.0.10.dev0/async_pjsekai/models/asset_bundle_info.py` & `async_pjsekai-0.0.10.dev1/async_pjsekai/models/asset_bundle_info.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 # SPDX-FileCopyrightText: 2022-2023 Erik Chan <erikchan002@gmail.com>
 # SPDX-FileCopyrightText: 2023-present TheerapakG <theerapakg@gmail.com>
 #
 # SPDX-License-Identifier: MIT
 
 from dataclasses import dataclass, field
-from typing import List, Optional, Union, Dict
+from typing import Optional, Union
 
-from pjsekai.enums import *
+from async_pjsekai.enums.enums import BundleCategory
+from async_pjsekai.enums.platform import AssetOS
+from async_pjsekai.enums.unknown import Unknown
 
 
 @dataclass(slots=True)
 class Bundle:
     bundle_name: Optional[str] = field(default=None)
     cache_directory_name: Optional[str] = field(default=None)
     hash: Optional[str] = field(default=None)
     category: Union[BundleCategory, Unknown, None] = field(default=None)
     crc: Optional[int] = field(default=None)
     file_size: Optional[int] = field(default=None)
-    dependencies: Optional[List[str]] = field(default=None)
-    paths: Optional[List[str]] = field(default=None)
+    dependencies: Optional[list[str]] = field(default=None)
+    paths: Optional[list[str]] = field(default=None)
     is_builtin: Optional[bool] = field(default=None)
 
 
 @dataclass(slots=True)
 class AssetBundleInfo:
     version: Optional[str] = field(default=None)
     os: Union[AssetOS, Unknown, None] = field(default=None)
-    bundles: Optional[Dict[str, Bundle]] = field(default=None)
+    bundles: Optional[dict[str, Bundle]] = field(default=None)
```

### Comparing `async_pjsekai-0.0.10.dev0/async_pjsekai/models/converters.py` & `async_pjsekai-0.0.10.dev1/async_pjsekai/models/converters.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,26 +3,38 @@
 # SPDX-License-Identifier: MIT
 
 from dataclasses import fields, is_dataclass
 from datetime import datetime
 from functools import partial
 from typing import Union, get_args, get_origin
 
-from pjsekai.enums.unknown import Unknown
-from pjsekai.models.model import to_pjsekai_camel
+from async_pjsekai.enums.unknown import Unknown
 
 from cattrs.converters import BaseConverter
 from cattrs.preconf.json import make_converter as make_json_converter
 from cattrs.preconf.msgpack import make_converter as make_msgpack_converter
 from cattrs.gen import make_dict_unstructure_fn, make_dict_structure_fn, override
 
 json_converter = make_json_converter()
 msgpack_converter = make_msgpack_converter()
 
 
+def to_lower_camel(string: str) -> str:
+    split = string.split("_")
+    return "".join((split[0].lower(), *(word.capitalize() for word in split[1:])))
+
+
+def to_pjsekai_camel(string: str) -> str:
+    return (
+        to_lower_camel(string)
+        .replace("AssetBundle", "Assetbundle")
+        .replace("assetBundle", "assetbundle")
+    )
+
+
 def to_pjsekai_camel_unstructure(converter: BaseConverter, cls):
     return make_dict_unstructure_fn(
         cls,
         converter,
         **{a.name: override(rename=to_pjsekai_camel(a.name)) for a in fields(cls)}
     )
```

### Comparing `async_pjsekai-0.0.10.dev0/async_pjsekai/models/master_data.py` & `async_pjsekai-0.0.10.dev1/async_pjsekai/models/master_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,41 +4,45 @@
 # SPDX-License-Identifier: MIT
 
 
 from dataclasses import dataclass, field, fields
 from datetime import datetime
 from typing import Optional, Type, TypeVar, Union
 
-from pjsekai.enums import *
+import async_pjsekai.enums.enums as pjenums
+from async_pjsekai.enums.platform import Platform
+from async_pjsekai.enums.unknown import Unknown
 
 
 @dataclass(slots=True)
 class GameCharacter:
     id: Optional[int] = field(default=None)
     seq: Optional[int] = field(default=None)
     resource_id: Optional[int] = field(default=None)
     first_name: Optional[str] = field(default=None)
     given_name: Optional[str] = field(default=None)
     first_name_ruby: Optional[str] = field(default=None)
     given_name_ruby: Optional[str] = field(default=None)
-    gender: Optional[Union[Gender, Unknown]] = field(default=None)
+    gender: Optional[Union[pjenums.Gender, Unknown]] = field(default=None)
     height: Optional[float] = field(default=None)
     live2d_height_adjustment: Optional[float] = field(default=None)
-    figure: Optional[Union[Figure, Unknown]] = field(default=None)
-    breast_size: Optional[Union[BreastSize, Unknown]] = field(default=None)
+    figure: Optional[Union[pjenums.Figure, Unknown]] = field(default=None)
+    breast_size: Optional[Union[pjenums.BreastSize, Unknown]] = field(default=None)
     model_name: Optional[str] = field(default=None)
-    unit: Optional[Union[Unit, Unknown]] = field(default=None)
-    support_unit_type: Optional[Union[SupportUnitType, Unknown]] = field(default=None)
+    unit: Optional[Union[pjenums.Unit, Unknown]] = field(default=None)
+    support_unit_type: Optional[Union[pjenums.SupportUnitType, Unknown]] = field(
+        default=None
+    )
 
 
 @dataclass(slots=True)
 class GameCharacterUnit:
     id: Optional[int] = field(default=None)
     game_character_id: Optional[int] = field(default=None)
-    unit: Optional[Union[Unit, Unknown]] = field(default=None)
+    unit: Optional[Union[pjenums.Unit, Unknown]] = field(default=None)
     color_code: Optional[str] = field(default=None)
     skin_color_code: Optional[str] = field(default=None)
     skin_shadow_color_code1: Optional[str] = field(default=None)
     skin_shadow_color_code2: Optional[str] = field(default=None)
 
 
 @dataclass(slots=True)
@@ -47,29 +51,33 @@
     seq: Optional[int] = field(default=None)
     name: Optional[str] = field(default=None)
 
 
 @dataclass(slots=True)
 class Character3d:
     id: Optional[int] = field(default=None)
-    character_type: Optional[Union[CharacterType, Unknown]] = field(default=None)
+    character_type: Optional[Union[pjenums.CharacterType, Unknown]] = field(
+        default=None
+    )
     character_id: Optional[int] = field(default=None)
-    unit: Optional[Union[Unit, Unknown]] = field(default=None)
+    unit: Optional[Union[pjenums.Unit, Unknown]] = field(default=None)
     name: Optional[str] = field(default=None)
     head_costume3d_id: Optional[int] = field(default=None)
     hair_costume3d_id: Optional[int] = field(default=None)
     body_costume3d_id: Optional[int] = field(default=None)
 
 
 @dataclass(slots=True)
 class Character2d:
     id: Optional[int] = field(default=None)
-    character_type: Optional[Union[CharacterType, Unknown]] = field(default=None)
+    character_type: Optional[Union[pjenums.CharacterType, Unknown]] = field(
+        default=None
+    )
     character_id: Optional[int] = field(default=None)
-    unit: Optional[Union[Unit, Unknown]] = field(default=None)
+    unit: Optional[Union[pjenums.Unit, Unknown]] = field(default=None)
     asset_name: Optional[str] = field(default=None)
 
 
 @dataclass(slots=True)
 class CharacterProfile:
     character_id: Optional[int] = field(default=None)
     character_voice: Optional[str] = field(default=None)
@@ -94,15 +102,15 @@
     character_id2: Optional[int] = field(default=None)
 
 
 @dataclass(slots=True)
 class Live2d:
     id: Optional[int] = field(default=None)
     character_id: Optional[int] = field(default=None)
-    unit: Optional[Union[Unit, Unknown]] = field(default=None)
+    unit: Optional[Union[pjenums.Unit, Unknown]] = field(default=None)
     asset_bundle_name: Optional[str] = field(default=None)
     motion: Optional[str] = field(default=None)
     expression: Optional[str] = field(default=None)
     weight: Optional[int] = field(default=None)
 
 
 @dataclass(slots=True)
@@ -113,43 +121,45 @@
 @dataclass(slots=True)
 class BondsRankUpLive2d(Live2d):
     default_flg: Optional[bool] = field(default=None)
 
 
 @dataclass(slots=True)
 class UnitProfile:
-    unit: Optional[Union[Unit, Unknown]] = field(default=None)
+    unit: Optional[Union[pjenums.Unit, Unknown]] = field(default=None)
     unit_name: Optional[str] = field(default=None)
     seq: Optional[int] = field(default=None)
     profile_sentence: Optional[str] = field(default=None)
     color_code: Optional[str] = field(default=None)
 
 
 @dataclass(slots=True)
 class ActionSet:
     id: Optional[int] = field(default=None)
     area_id: Optional[int] = field(default=None)
     script_id: Optional[str] = field(default=None)
     character_ids: Optional[list[int]] = field(default=None)
-    archive_display_type: Optional[Union[ArchiveDisplayType, Unknown]] = field(
+    archive_display_type: Optional[Union[pjenums.ArchiveDisplayType, Unknown]] = field(
         default=None
     )
     archive_published_at: Optional[datetime] = field(default=None)
     release_condition_id: Optional[datetime] = field(default=None)
     scenario_id: Optional[str] = field(default=None)
-    action_set_type: Optional[Union[ActionSetType, Unknown]] = field(default=None)
+    action_set_type: Optional[Union[pjenums.ActionSetType, Unknown]] = field(
+        default=None
+    )
     special_season_id: Optional[int] = field(default=None)
 
 
 @dataclass(slots=True)
 class Area:
     id: Optional[int] = field(default=None)
     asset_bundle_name: Optional[str] = field(default=None)
-    area_type: Optional[Union[AreaType, Unknown]] = field(default=None)
-    view_type: Optional[Union[ViewType, Unknown]] = field(default=None)
+    area_type: Optional[Union[pjenums.AreaType, Unknown]] = field(default=None)
+    view_type: Optional[Union[pjenums.ViewType, Unknown]] = field(default=None)
     name: Optional[str] = field(default=None)
     release_condition_id: Optional[int] = field(default=None)
     label: Optional[str] = field(default=None)
     start_at: Optional[datetime] = field(default=None)
     end_at: Optional[datetime] = field(default=None)
 
 
@@ -164,15 +174,15 @@
 
 
 @dataclass(slots=True)
 class MobCharacter:
     id: Optional[int] = field(default=None)
     seq: Optional[int] = field(default=None)
     name: Optional[str] = field(default=None)
-    gender: Optional[Union[Gender, Unknown]] = field(default=None)
+    gender: Optional[Union[pjenums.Gender, Unknown]] = field(default=None)
 
 
 @dataclass(slots=True)
 class CharacterCostume:
     id: Optional[int] = field(default=None)
     character_id: Optional[int] = field(default=None)
     costume_id: Optional[int] = field(default=None)
@@ -187,24 +197,24 @@
 
 
 @dataclass(slots=True)
 class CardParameter:
     id: Optional[int] = field(default=None)
     card_id: Optional[int] = field(default=None)
     card_level: Optional[int] = field(default=None)
-    card_parameter_type: Optional[Union[CardParameterType, Unknown]] = field(
+    card_parameter_type: Optional[Union[pjenums.CardParameterType, Unknown]] = field(
         default=None
     )
     power: Optional[int] = field(default=None)
 
 
 @dataclass(slots=True)
 class Cost:
     resource_id: Optional[int] = field(default=None)
-    resource_type: Optional[Union[ResourceType, Unknown]] = field(default=None)
+    resource_type: Optional[Union[pjenums.ResourceType, Unknown]] = field(default=None)
     resource_level: Optional[int] = field(default=None)
     quantity: Optional[int] = field(default=None)
 
 
 @dataclass(slots=True)
 class SpecialTrainingCost:
     card_id: Optional[int] = field(default=None)
@@ -221,77 +231,83 @@
 
 
 @dataclass(slots=True)
 class Card:
     id: Optional[int] = field(default=None)
     seq: Optional[int] = field(default=None)
     character_id: Optional[int] = field(default=None)
-    card_rarity_type: Optional[Union[CardRarityType, Unknown]] = field(default=None)
+    card_rarity_type: Optional[Union[pjenums.CardRarityType, Unknown]] = field(
+        default=None
+    )
     special_training_power1_bonus_fixed: Optional[int] = field(default=None)
     special_training_power2_bonus_fixed: Optional[int] = field(default=None)
     special_training_power3_bonus_fixed: Optional[int] = field(default=None)
-    attr: Optional[Union[CardAttr, Unknown]] = field(default=None)
-    support_unit: Optional[Union[Unit, Unknown]] = field(default=None)
+    attr: Optional[Union[pjenums.CardAttr, Unknown]] = field(default=None)
+    support_unit: Optional[Union[pjenums.Unit, Unknown]] = field(default=None)
     skill_id: Optional[int] = field(default=None)
     card_skill_name: Optional[str] = field(default=None)
     prefix: Optional[str] = field(default=None)
     asset_bundle_name: Optional[str] = field(default=None)
     gacha_phrase: Optional[str] = field(default=None)
     flavor_text: Optional[str] = field(default=None)
     release_at: Optional[datetime] = field(default=None)
     archive_published_at: Optional[datetime] = field(default=None)
     card_parameters: Optional[list[CardParameter]] = field(default=None)
     special_training_costs: Optional[list[SpecialTrainingCost]] = field(default=None)
     master_lesson_achieve_resources: Optional[
         list[MasterLessonAchieveResource]
     ] = field(default=None)
-    archive_display_type: Optional[Union[ArchiveDisplayType, Unknown]] = field(
+    archive_display_type: Optional[Union[pjenums.ArchiveDisplayType, Unknown]] = field(
         default=None
     )
 
 
 @dataclass(slots=True)
 class SkillEffectDetail:
     id: Optional[int] = field(default=None)
     level: Optional[int] = field(default=None)
     activate_effect_duration: Optional[float] = field(default=None)
     activate_effect_value_type: Optional[
-        Union[ActivateEffectValueType, Unknown]
+        Union[pjenums.ActivateEffectValueType, Unknown]
     ] = field(default=None)
     activate_effect_value: Optional[int] = field(default=None)
 
 
 @dataclass(slots=True)
 class SkillEnhanceCondition:
     id: Optional[int] = field(default=None)
     seq: Optional[int] = field(default=None)
-    unit: Optional[Union[Unit, Unknown]] = field(default=None)
+    unit: Optional[Union[pjenums.Unit, Unknown]] = field(default=None)
 
 
 @dataclass(slots=True)
 class SkillEnhance:
     id: Optional[int] = field(default=None)
-    skill_enhance_type: Optional[Union[SkillEnhanceType, Unknown]] = field(default=None)
+    skill_enhance_type: Optional[Union[pjenums.SkillEnhanceType, Unknown]] = field(
+        default=None
+    )
     activate_effect_value_type: Optional[
-        Union[ActivateEffectValueType, Unknown]
+        Union[pjenums.ActivateEffectValueType, Unknown]
     ] = field(default=None)
     activate_effect_value: Optional[int] = field(default=None)
     skill_enhance_condition: Optional[SkillEnhanceCondition] = field(default=None)
 
 
 @dataclass(slots=True)
 class SkillEffect:
     id: Optional[int] = field(default=None)
-    skill_effect_type: Optional[Union[SkillEffectType, Unknown]] = field(default=None)
-    activate_notes_judgment_type: Optional[Union[IngameNoteJudgeType, Unknown]] = field(
+    skill_effect_type: Optional[Union[pjenums.SkillEffectType, Unknown]] = field(
         default=None
     )
+    activate_notes_judgment_type: Optional[
+        Union[pjenums.IngameNoteJudgeType, Unknown]
+    ] = field(default=None)
     skill_effect_details: Optional[list[SkillEffectDetail]] = field(default=None)
     activate_life: Optional[int] = field(default=None)
-    condition_type: Optional[Union[SkillEffectConditionType, Unknown]] = field(
+    condition_type: Optional[Union[pjenums.SkillEffectConditionType, Unknown]] = field(
         default=None
     )
     skill_enhance: Optional[SkillEnhance] = field(default=None)
 
 
 @dataclass(slots=True)
 class Skill:
@@ -313,22 +329,24 @@
     asset_bundle_name: Optional[str] = field(default=None)
     release_condition_id: Optional[int] = field(default=None)
     power1_bonus_fixed: Optional[int] = field(default=None)
     power2_bonus_fixed: Optional[int] = field(default=None)
     power3_bonus_fixed: Optional[int] = field(default=None)
     reward_resource_box_ids: Optional[list[int]] = field(default=None)
     costs: Optional[list[Cost]] = field(default=None)
-    card_episode_part_type: Optional[Union[CardEpisodePartType, Unknown]] = field(
-        default=None
-    )
+    card_episode_part_type: Optional[
+        Union[pjenums.CardEpisodePartType, Unknown]
+    ] = field(default=None)
 
 
 @dataclass(slots=True)
 class CardRarity:
-    card_rarity_type: Optional[Union[CardRarityType, Unknown]] = field(default=None)
+    card_rarity_type: Optional[Union[pjenums.CardRarityType, Unknown]] = field(
+        default=None
+    )
     seq: Optional[int] = field(default=None)
     max_level: Optional[int] = field(default=None)
     max_skill_level: Optional[int] = field(default=None)
     training_max_level: Optional[int] = field(default=None)
 
 
 @dataclass(slots=True)
@@ -339,15 +357,17 @@
 
 
 @dataclass(slots=True)
 class Music:
     id: Optional[int] = field(default=None)
     seq: Optional[int] = field(default=None)
     release_condition_id: Optional[int] = field(default=None)
-    categories: Optional[list[Union[MusicCategory, Unknown]]] = field(default=None)
+    categories: Optional[list[Union[pjenums.MusicCategory, Unknown]]] = field(
+        default=None
+    )
     title: Optional[str] = field(default=None)
     pronunciation: Optional[str] = field(default=None)
     lyricist: Optional[str] = field(default=None)
     composer: Optional[str] = field(default=None)
     arranger: Optional[str] = field(default=None)
     dancer_count: Optional[int] = field(default=None)
     self_dancer_position: Optional[int] = field(default=None)
@@ -367,96 +387,106 @@
     seq: Optional[int] = field(default=None)
 
 
 @dataclass(slots=True)
 class MusicDifficulty:
     id: Optional[int] = field(default=None)
     music_id: Optional[int] = field(default=None)
-    music_difficulty: Optional[Union[MusicDifficultyType, Unknown]] = field(
+    music_difficulty: Optional[Union[pjenums.MusicDifficultyType, Unknown]] = field(
         default=None
     )
     play_level: Optional[int] = field(default=None)
     release_condition_id: Optional[int] = field(default=None)
     total_note_count: Optional[int] = field(default=None)
 
 
 @dataclass(slots=True)
 class Character:
     id: Optional[int] = field(default=None)
     music_id: Optional[int] = field(default=None)
     music_vocal_id: Optional[int] = field(default=None)
-    character_type: Optional[Union[CharacterType, Unknown]] = field(default=None)
+    character_type: Optional[Union[pjenums.CharacterType, Unknown]] = field(
+        default=None
+    )
     character_id: Optional[int] = field(default=None)
     seq: Optional[int] = field(default=None)
 
 
 @dataclass(slots=True)
 class MusicVocal:
     id: Optional[int] = field(default=None)
     music_id: Optional[int] = field(default=None)
-    music_vocal_type: Optional[Union[MusicVocalType, Unknown]] = field(default=None)
+    music_vocal_type: Optional[Union[pjenums.MusicVocalType, Unknown]] = field(
+        default=None
+    )
     seq: Optional[int] = field(default=None)
     release_condition_id: Optional[int] = field(default=None)
     caption: Optional[str] = field(default=None)
     characters: Optional[list[Character]] = field(default=None)
     asset_bundle_name: Optional[str] = field(default=None)
     archive_published_at: Optional[datetime] = field(default=None)
     special_season_id: Optional[int] = field(default=None)
-    archive_display_type: Optional[Union[ArchiveDisplayType, Unknown]] = field(
+    archive_display_type: Optional[Union[pjenums.ArchiveDisplayType, Unknown]] = field(
         default=None
     )
 
 
 @dataclass(slots=True)
 class MusicDanceMember:
     id: Optional[int] = field(default=None)
     music_id: Optional[int] = field(default=None)
-    default_music_type: Optional[Union[DefaultMusicType, Unknown]] = field(default=None)
+    default_music_type: Optional[Union[pjenums.DefaultMusicType, Unknown]] = field(
+        default=None
+    )
     character_id1: Optional[int] = field(default=None)
-    unit1: Optional[Union[Unit, Unknown]] = field(default=None)
+    unit1: Optional[Union[pjenums.Unit, Unknown]] = field(default=None)
     character_id2: Optional[int] = field(default=None)
-    unit2: Optional[Union[Unit, Unknown]] = field(default=None)
+    unit2: Optional[Union[pjenums.Unit, Unknown]] = field(default=None)
     character_id3: Optional[int] = field(default=None)
-    unit3: Optional[Union[Unit, Unknown]] = field(default=None)
+    unit3: Optional[Union[pjenums.Unit, Unknown]] = field(default=None)
     character_id4: Optional[int] = field(default=None)
-    unit4: Optional[Union[Unit, Unknown]] = field(default=None)
+    unit4: Optional[Union[pjenums.Unit, Unknown]] = field(default=None)
     character_id5: Optional[int] = field(default=None)
-    unit5: Optional[Union[Unit, Unknown]] = field(default=None)
+    unit5: Optional[Union[pjenums.Unit, Unknown]] = field(default=None)
 
 
 @dataclass(slots=True)
 class MusicAchievement:
     id: Optional[int] = field(default=None)
-    music_achievement_type: Optional[Union[MusicAchievementType, Unknown]] = field(
-        default=None
-    )
+    music_achievement_type: Optional[
+        Union[pjenums.MusicAchievementType, Unknown]
+    ] = field(default=None)
     music_achievement_type_value: Optional[str] = field(default=None)
     resource_box_id: Optional[int] = field(default=None)
-    music_difficulty_type: Optional[Union[MusicDifficultyType, Unknown]] = field(
-        default=None
-    )
+    music_difficulty_type: Optional[
+        Union[pjenums.MusicDifficultyType, Unknown]
+    ] = field(default=None)
 
 
 @dataclass(slots=True)
 class MusicVideoCharacter:
     id: Optional[int] = field(default=None)
     music_id: Optional[int] = field(default=None)
-    default_music_type: Optional[Union[DefaultMusicType, Unknown]] = field(default=None)
+    default_music_type: Optional[Union[pjenums.DefaultMusicType, Unknown]] = field(
+        default=None
+    )
     game_character_unit_id: Optional[int] = field(default=None)
     dance_priority: Optional[int] = field(default=None)
     seq: Optional[int] = field(default=None)
     priority: Optional[int] = field(default=None)
 
 
 @dataclass(slots=True)
 class MusicAssetVariant:
     id: Optional[int] = field(default=None)
     music_vocal_id: Optional[int] = field(default=None)
     seq: Optional[int] = field(default=None)
-    music_asset_type: Optional[Union[MusicAssetType, Unknown]] = field(default=None)
+    music_asset_type: Optional[Union[pjenums.MusicAssetType, Unknown]] = field(
+        default=None
+    )
     asset_bundle_name: Optional[str] = field(default=None)
 
 
 @dataclass(slots=True)
 class MusicCollaboration:
     id: Optional[int] = field(default=None)
     label: Optional[str] = field(default=None)
@@ -473,25 +503,25 @@
     character3d_id5: Optional[int] = field(default=None)
 
 
 @dataclass(slots=True)
 class ReleaseCondition:
     id: Optional[int] = field(default=None)
     sentence: Optional[str] = field(default=None)
-    release_condition_type: Optional[Union[ReleaseConditionType, Unknown]] = field(
-        default=None
-    )
+    release_condition_type: Optional[
+        Union[pjenums.ReleaseConditionType, Unknown]
+    ] = field(default=None)
     release_condition_type_level: Optional[int] = field(default=None)
     release_condition_type_id: Optional[int] = field(default=None)
     release_condition_type_quantity: Optional[int] = field(default=None)
 
 
 @dataclass(slots=True)
 class PlayLevelScore:
-    live_type: Optional[Union[LiveType, Unknown]] = field(default=None)
+    live_type: Optional[Union[pjenums.LiveType, Unknown]] = field(default=None)
     play_level: Optional[int] = field(default=None)
     s: Optional[int] = field(default=None)
     a: Optional[int] = field(default=None)
     b: Optional[int] = field(default=None)
     c: Optional[int] = field(default=None)
 
 
@@ -502,63 +532,67 @@
     to_count: Optional[int] = field(default=None)
     score_coefficient: Optional[float] = field(default=None)
 
 
 @dataclass(slots=True)
 class IngameNote:
     id: Optional[int] = field(default=None)
-    ingame_note_type: Optional[Union[IngameNoteType, Unknown]] = field(default=None)
+    ingame_note_type: Optional[Union[pjenums.IngameNoteType, Unknown]] = field(
+        default=None
+    )
     score_coefficient: Optional[float] = field(default=None)
     damage_bad: Optional[int] = field(default=None)
     damage_miss: Optional[int] = field(default=None)
 
 
 @dataclass(slots=True)
 class IngameNoteJudge:
     id: Optional[int] = field(default=None)
-    ingame_note_jadge_type: Optional[Union[IngameNoteJudgeType, Unknown]] = field(
-        default=None
-    )
+    ingame_note_jadge_type: Optional[
+        Union[pjenums.IngameNoteJudgeType, Unknown]
+    ] = field(default=None)
     score_coefficient: Optional[float] = field(default=None)
     damage: Optional[int] = field(default=None)
 
 
 @dataclass(slots=True)
 class IngamePlayLevel:
     play_level: Optional[int] = field(default=None)
     score_coefficient: Optional[float] = field(default=None)
 
 
 @dataclass(slots=True)
 class IngameCutin:
     id: Optional[int] = field(default=None)
-    music_difficulty: Optional[Union[MusicDifficultyType, Unknown]] = field(
+    music_difficulty: Optional[Union[pjenums.MusicDifficultyType, Unknown]] = field(
         default=None
     )
     combo: Optional[int] = field(default=None)
 
 
 @dataclass(slots=True)
 class IngameCutinCharacter:
     id: Optional[int] = field(default=None)
     ingame_cutin_character_type: Optional[
-        Union[IngameCutinCharacterType, Unknown]
+        Union[pjenums.IngameCutinCharacterType, Unknown]
     ] = field(default=None)
     priority: Optional[int] = field(default=None)
     game_character_unit_id1: Optional[int] = field(default=None)
     game_character_unit_id2: Optional[int] = field(default=None)
     asset_bundle_name1: Optional[str] = field(default=None)
     asset_bundle_name2: Optional[str] = field(default=None)
     release_condition_id: Optional[int] = field(default=None)
 
 
 @dataclass(slots=True)
 class IngameJudgeFrame:
     id: Optional[int] = field(default=None)
-    ingame_note_type: Optional[Union[IngameNoteType, Unknown]] = field(default=None)
+    ingame_note_type: Optional[Union[pjenums.IngameNoteType, Unknown]] = field(
+        default=None
+    )
     perfect: Optional[float] = field(default=None)
     great: Optional[float] = field(default=None)
     good: Optional[float] = field(default=None)
     bad: Optional[float] = field(default=None)
     perfect_before: Optional[float] = field(default=None)
     perfect_after: Optional[float] = field(default=None)
     great_before: Optional[float] = field(default=None)
@@ -568,26 +602,26 @@
     bad_before: Optional[float] = field(default=None)
     bad_after: Optional[float] = field(default=None)
 
 
 @dataclass(slots=True)
 class IngameNoteJudgeTechnicalScore:
     id: Optional[int] = field(default=None)
-    live_type: Optional[Union[LiveType, Unknown]] = field(default=None)
-    ingame_note_jadge_type: Optional[Union[IngameNoteJudgeType, Unknown]] = field(
-        default=None
-    )
+    live_type: Optional[Union[pjenums.LiveType, Unknown]] = field(default=None)
+    ingame_note_jadge_type: Optional[
+        Union[pjenums.IngameNoteJudgeType, Unknown]
+    ] = field(default=None)
     score: Optional[int] = field(default=None)
 
 
 @dataclass(slots=True)
 class Shop:
     id: Optional[int] = field(default=None)
     seq: Optional[int] = field(default=None)
-    shop_type: Optional[Union[ShopType, Unknown]] = field(default=None)
+    shop_type: Optional[Union[pjenums.ShopType, Unknown]] = field(default=None)
     area_id: Optional[int] = field(default=None)
     name: Optional[str] = field(default=None)
     release_condition_id: Optional[int] = field(default=None)
 
 
 @dataclass(slots=True)
 class ShopItemCost:
@@ -637,16 +671,16 @@
     asset_bundle_name: Optional[str] = field(default=None)
 
 
 @dataclass(slots=True)
 class AreaItemLevel:
     area_item_id: Optional[int] = field(default=None)
     level: Optional[int] = field(default=None)
-    targetunit: Optional[Union[Unit, Unknown]] = field(default=None)
-    target_card_attr: Optional[Union[CardAttr, Unknown]] = field(default=None)
+    targetunit: Optional[Union[pjenums.Unit, Unknown]] = field(default=None)
+    target_card_attr: Optional[Union[pjenums.CardAttr, Unknown]] = field(default=None)
     target_game_character_id: Optional[int] = field(default=None)
     power1_bonus_rate: Optional[float] = field(default=None)
     power1_all_match_bonus_rate: Optional[float] = field(default=None)
     power2_bonus_rate: Optional[float] = field(default=None)
     power2_all_match_bonus_rate: Optional[float] = field(default=None)
     power3_bonus_rate: Optional[float] = field(default=None)
     power3_all_match_bonus_rate: Optional[float] = field(default=None)
@@ -655,23 +689,25 @@
 
 @dataclass(slots=True)
 class Material:
     id: Optional[int] = field(default=None)
     seq: Optional[int] = field(default=None)
     name: Optional[str] = field(default=None)
     flavor_text: Optional[str] = field(default=None)
-    material_type: Optional[Union[MaterialType, Unknown]] = field(default=None)
+    material_type: Optional[Union[pjenums.MaterialType, Unknown]] = field(default=None)
 
 
 @dataclass(slots=True)
 class GachaCardRarityRate:
     id: Optional[int] = field(default=None)
     group_id: Optional[int] = field(default=None)
-    card_rarity_type: Optional[Union[CardRarityType, Unknown]] = field(default=None)
-    lottery_type: Optional[Union[LotteryType, Unknown]] = field(default=None)
+    card_rarity_type: Optional[Union[pjenums.CardRarityType, Unknown]] = field(
+        default=None
+    )
+    lottery_type: Optional[Union[pjenums.LotteryType, Unknown]] = field(default=None)
     rate: Optional[float] = field(default=None)
 
 
 @dataclass(slots=True)
 class GachaDetail:
     id: Optional[int] = field(default=None)
     gacha_id: Optional[int] = field(default=None)
@@ -682,44 +718,48 @@
 
 @dataclass(slots=True)
 class GachaBehavior:
     id: Optional[int] = field(default=None)
     gacha_id: Optional[int] = field(default=None)
     group_id: Optional[int] = field(default=None)
     priority: Optional[int] = field(default=None)
-    gacha_behavior_type: Optional[Union[GachaBehaviorType, Unknown]] = field(
+    gacha_behavior_type: Optional[Union[pjenums.GachaBehaviorType, Unknown]] = field(
+        default=None
+    )
+    cost_resource_type: Optional[Union[pjenums.ResourceType, Unknown]] = field(
         default=None
     )
-    cost_resource_type: Optional[Union[ResourceType, Unknown]] = field(default=None)
     cost_resource_quantity: Optional[int] = field(default=None)
     spin_count: Optional[int] = field(default=None)
     execute_limit: Optional[int] = field(default=None)
     cost_resource_id: Optional[int] = field(default=None)
     gacha_extra_id: Optional[int] = field(default=None)
 
 
 @dataclass(slots=True)
 class GachaPickup:
     id: Optional[int] = field(default=None)
     gacha_id: Optional[int] = field(default=None)
     card_id: Optional[int] = field(default=None)
-    gacha_pickup_type: Optional[Union[GachaPickupType, Unknown]] = field(default=None)
+    gacha_pickup_type: Optional[Union[pjenums.GachaPickupType, Unknown]] = field(
+        default=None
+    )
 
 
 @dataclass(slots=True)
 class GachaInformation:
     gacha_id: Optional[int] = field(default=None)
     summary: Optional[str] = field(default=None)
     description: Optional[str] = field(default=None)
 
 
 @dataclass(slots=True)
 class Gacha:
     id: Optional[int] = field(default=None)
-    gacha_type: Optional[Union[GachaType, Unknown]] = field(default=None)
+    gacha_type: Optional[Union[pjenums.GachaType, Unknown]] = field(default=None)
     name: Optional[str] = field(default=None)
     seq: Optional[int] = field(default=None)
     asset_bundle_name: Optional[str] = field(default=None)
     gacha_card_rarity_rate_group_id: Optional[int] = field(default=None)
     start_at: Optional[datetime] = field(default=None)
     end_at: Optional[datetime] = field(default=None)
     is_show_period: Optional[bool] = field(default=None)
@@ -742,15 +782,15 @@
 class GachaBonus:
     id: Optional[int] = field(default=None)
 
 
 @dataclass(slots=True)
 class GachaBonusPoint:
     id: Optional[int] = field(default=None)
-    resource_type: Optional[Union[ResourceType, Unknown]] = field(default=None)
+    resource_type: Optional[Union[pjenums.ResourceType, Unknown]] = field(default=None)
     point: Optional[float] = field(default=None)
 
 
 @dataclass(slots=True)
 class GachaExtra:
     id: Optional[int] = field(default=None)
     resource_box_id: Optional[int] = field(default=None)
@@ -776,15 +816,15 @@
 class SkillPracticeTicket(PracticeTicket):
     pass
 
 
 @dataclass(slots=True)
 class Level:
     id: Optional[int] = field(default=None)
-    level_type: Optional[Union[LevelType, Unknown]] = field(default=None)
+    level_type: Optional[Union[pjenums.LevelType, Unknown]] = field(default=None)
     level: Optional[int] = field(default=None)
     total_exp: Optional[int] = field(default=None)
 
 
 @dataclass(slots=True)
 class Episode:
     id: Optional[int] = field(default=None)
@@ -794,36 +834,36 @@
     scenario_id: Optional[str] = field(default=None)
     release_condition_id: Optional[int] = field(default=None)
     reward_resource_box_ids: Optional[list[int]] = field(default=None)
 
 
 @dataclass(slots=True)
 class UnitStoryEpisode(Episode):
-    unit: Optional[Union[Unit, Unknown]] = field(default=None)
+    unit: Optional[Union[pjenums.Unit, Unknown]] = field(default=None)
     chapter_no: Optional[int] = field(default=None)
-    unit_episode_category: Optional[Union[Unit, Unknown]] = field(default=None)
+    unit_episode_category: Optional[Union[pjenums.Unit, Unknown]] = field(default=None)
     episode_no_label: Optional[str] = field(default=None)
     limited_release_start_at: Optional[datetime] = field(default=None)
     limited_release_end_at: Optional[datetime] = field(default=None)
     and_release_condition_id: Optional[int] = field(default=None)
 
 
 @dataclass(slots=True)
 class Chapter:
     id: Optional[int] = field(default=None)
-    unit: Optional[Union[Unit, Unknown]] = field(default=None)
+    unit: Optional[Union[pjenums.Unit, Unknown]] = field(default=None)
     chapter_no: Optional[int] = field(default=None)
     title: Optional[str] = field(default=None)
     asset_bundle_name: Optional[str] = field(default=None)
     episodes: Optional[list[UnitStoryEpisode]] = field(default=None)
 
 
 @dataclass(slots=True)
 class UnitStory:
-    unit: Optional[Union[Unit, Unknown]] = field(default=None)
+    unit: Optional[Union[pjenums.Unit, Unknown]] = field(default=None)
     seq: Optional[int] = field(default=None)
     asset_bundle_name: Optional[str] = field(default=None)
     chapters: Optional[list[Chapter]] = field(default=None)
 
 
 @dataclass(slots=True)
 class SpecialStoryEpisode(Episode):
@@ -851,73 +891,77 @@
     value: Optional[str] = field(default=None)
 
 
 @dataclass(slots=True)
 class ClientConfig:
     id: Optional[int] = field(default=None)
     value: Optional[str] = field(default=None)
-    type: Optional[Union[ClientConfigType, Unknown]] = field(default=None)
+    type: Optional[Union[pjenums.ClientConfigType, Unknown]] = field(default=None)
 
 
 @dataclass(slots=True)
 class Wording:
     wording_key: Optional[str] = field(default=None)
     value: Optional[str] = field(default=None)
 
 
 @dataclass(slots=True)
 class Costume3d:
     id: Optional[int] = field(default=None)
     seq: Optional[int] = field(default=None)
     costume3d_group_id: Optional[int] = field(default=None)
-    costume3d_type: Optional[Union[Costume3dType, Unknown]] = field(default=None)
+    costume3d_type: Optional[Union[pjenums.Costume3dType, Unknown]] = field(
+        default=None
+    )
     name: Optional[str] = field(default=None)
-    part_type: Optional[Union[PartType, Unknown]] = field(default=None)
+    part_type: Optional[Union[pjenums.PartType, Unknown]] = field(default=None)
     color_id: Optional[int] = field(default=None)
     color_name: Optional[str] = field(default=None)
     character_id: Optional[int] = field(default=None)
-    costume3d_rarity: Optional[Union[Costume3dRarity, Unknown]] = field(default=None)
+    costume3d_rarity: Optional[Union[pjenums.Costume3dRarity, Unknown]] = field(
+        default=None
+    )
     how_to_obtain: Optional[str] = field(default=None)
     asset_bundle_name: Optional[str] = field(default=None)
     designer: Optional[str] = field(default=None)
-    archive_display_type: Optional[Union[ArchiveDisplayType, Unknown]] = field(
+    archive_display_type: Optional[Union[pjenums.ArchiveDisplayType, Unknown]] = field(
         default=None
     )
     archive_published_at: Optional[datetime] = field(default=None)
     published_at: Optional[datetime] = field(default=None)
 
 
 @dataclass(slots=True)
 class Costume3dModel:
     id: Optional[int] = field(default=None)
     costume3d_id: Optional[int] = field(default=None)
-    unit: Optional[Union[Unit, Unknown]] = field(default=None)
+    unit: Optional[Union[pjenums.Unit, Unknown]] = field(default=None)
     head_costume3d_asset_bundle_type: Optional[
-        Union[HeadCostume3dAssetBundleType, Unknown]
+        Union[pjenums.HeadCostume3dAssetBundleType, Unknown]
     ] = field(default=None)
     thumbnail_asset_bundle_name: Optional[str] = field(default=None)
     asset_bundle_name: Optional[str] = field(default=None)
     color_asset_bundle_name: Optional[str] = field(default=None)
     part: Optional[str] = field(default=None)
 
 
 @dataclass(slots=True)
 class Costume3dModelAvailablePattern:
     id: Optional[int] = field(default=None)
     head_costume3d_id: Optional[int] = field(default=None)
     hair_costume3d_id: Optional[int] = field(default=None)
-    unit: Optional[Union[Unit, Unknown]] = field(default=None)
+    unit: Optional[Union[pjenums.Unit, Unknown]] = field(default=None)
     is_default: Optional[bool] = field(default=None)
 
 
 @dataclass(slots=True)
 class GameCharacterUnit3dMotion:
     id: Optional[int] = field(default=None)
     game_character_unit_id: Optional[int] = field(default=None)
-    motion_type: Optional[Union[MotionType, Unknown]] = field(default=None)
+    motion_type: Optional[Union[pjenums.MotionType, Unknown]] = field(default=None)
     asset_bundle_name: Optional[str] = field(default=None)
 
 
 @dataclass(slots=True)
 class Costume2d:
     id: Optional[int] = field(default=None)
     costume2d_group_id: Optional[int] = field(default=None)
@@ -933,68 +977,74 @@
     id: Optional[int] = field(default=None)
     name: Optional[str] = field(default=None)
 
 
 @dataclass(slots=True)
 class Topic:
     id: Optional[int] = field(default=None)
-    topic_type: Optional[Union[TopicType, Unknown]] = field(default=None)
+    topic_type: Optional[Union[pjenums.TopicType, Unknown]] = field(default=None)
     topic_type_id: Optional[int] = field(default=None)
     release_condition_id: Optional[int] = field(default=None)
 
 
 @dataclass(slots=True)
 class LiveStage:
     id: Optional[int] = field(default=None)
     name: Optional[str] = field(default=None)
     asset_bundle_name: Optional[str] = field(default=None)
 
 
 @dataclass(slots=True)
 class Stamp:
     id: Optional[int] = field(default=None)
-    stamp_type: Optional[Union[StampType, Unknown]] = field(default=None)
+    stamp_type: Optional[Union[pjenums.StampType, Unknown]] = field(default=None)
     seq: Optional[int] = field(default=None)
     name: Optional[str] = field(default=None)
     asset_bundle_name: Optional[str] = field(default=None)
     balloon_asset_bundle_name: Optional[str] = field(default=None)
     character_id1: Optional[int] = field(default=None)
     game_character_unit_id: Optional[int] = field(default=None)
     archive_published_at: Optional[datetime] = field(default=None)
     description: Optional[str] = field(default=None)
-    archive_display_type: Optional[Union[ArchiveDisplayType, Unknown]] = field(
+    archive_display_type: Optional[Union[pjenums.ArchiveDisplayType, Unknown]] = field(
         default=None
     )
 
 
 @dataclass(slots=True)
 class MultiLiveLobby:
     id: Optional[int] = field(default=None)
     seq: Optional[int] = field(default=None)
     name: Optional[str] = field(default=None)
     photon_lobby_name: Optional[str] = field(default=None)
-    matching_logic: Optional[Union[MatchingLogic, Unknown]] = field(default=None)
+    matching_logic: Optional[Union[pjenums.MatchingLogic, Unknown]] = field(
+        default=None
+    )
     total_power: Optional[int] = field(default=None)
     asset_bundle_name: Optional[str] = field(default=None)
-    multi_live_lobby_type: Optional[Union[MultiLiveLobbyType, Unknown]] = field(
+    multi_live_lobby_type: Optional[Union[pjenums.MultiLiveLobbyType, Unknown]] = field(
         default=None
     )
 
 
 @dataclass(slots=True)
 class MasterLessonCost(Cost):
     id: Optional[int] = field(default=None)
-    card_rarity_type: Optional[Union[CardRarityType, Unknown]] = field(default=None)
+    card_rarity_type: Optional[Union[pjenums.CardRarityType, Unknown]] = field(
+        default=None
+    )
     master_rank: Optional[int] = field(default=None)
     seq: Optional[int] = field(default=None)
 
 
 @dataclass(slots=True)
 class MasterLesson:
-    card_rarity_type: Optional[Union[CardRarityType, Unknown]] = field(default=None)
+    card_rarity_type: Optional[Union[pjenums.CardRarityType, Unknown]] = field(
+        default=None
+    )
     master_rank: Optional[int] = field(default=None)
     power1_bonus_fixed: Optional[int] = field(default=None)
     power2_bonus_fixed: Optional[int] = field(default=None)
     power3_bonus_fixed: Optional[int] = field(default=None)
     character_rank_exp: Optional[int] = field(default=None)
     costs: Optional[list[MasterLessonCost]] = field(default=None)
     rewards: Optional[list[Union[dict, str, int]]] = field(default=None)
@@ -1008,15 +1058,17 @@
     seq: Optional[int] = field(default=None)
     resource_box_id: Optional[int] = field(default=None)
     card_rarity: Optional[int] = field(default=None)
 
 
 @dataclass(slots=True)
 class CardExchangeResource:
-    card_rarity_type: Optional[Union[CardRarityType, Unknown]] = field(default=None)
+    card_rarity_type: Optional[Union[pjenums.CardRarityType, Unknown]] = field(
+        default=None
+    )
     seq: Optional[int] = field(default=None)
     resource_box_id: Optional[int] = field(default=None)
 
 
 @dataclass(slots=True)
 class MaterialExchangeCost(Cost):
     material_exchange_id: Optional[int] = field(default=None)
@@ -1026,28 +1078,30 @@
 
 @dataclass(slots=True)
 class MaterialExchange:
     id: Optional[int] = field(default=None)
     material_exchange_summary_id: Optional[int] = field(default=None)
     seq: Optional[int] = field(default=None)
     resource_box_id: Optional[int] = field(default=None)
-    refresh_cycle: Optional[Union[RefreshCycle, Unknown]] = field(default=None)
+    refresh_cycle: Optional[Union[pjenums.RefreshCycle, Unknown]] = field(default=None)
     costs: Optional[list[MaterialExchangeCost]] = field(default=None)
     exchange_limit: Optional[int] = field(default=None)
     start_at: Optional[datetime] = field(default=None)
 
 
 @dataclass(slots=True)
 class MaterialExchangeSummary:
     id: Optional[int] = field(default=None)
     seq: Optional[int] = field(default=None)
-    exchange_category: Optional[Union[ExchangeCategory, Unknown]] = field(default=None)
-    material_exchange_type: Optional[Union[MaterialExchangeType, Unknown]] = field(
+    exchange_category: Optional[Union[pjenums.ExchangeCategory, Unknown]] = field(
         default=None
     )
+    material_exchange_type: Optional[
+        Union[pjenums.MaterialExchangeType, Unknown]
+    ] = field(default=None)
     name: Optional[str] = field(default=None)
     asset_bundle_name: Optional[str] = field(default=None)
     start_at: Optional[datetime] = field(default=None)
     material_exchanges: Optional[list[MaterialExchange]] = field(default=None)
     end_at: Optional[datetime] = field(default=None)
     notification_remain_hour: Optional[int] = field(default=None)
 
@@ -1072,35 +1126,37 @@
     unit_price: Optional[float] = field(default=None)
 
 
 @dataclass(slots=True)
 class BillingShopItem:
     id: Optional[int] = field(default=None)
     seq: Optional[int] = field(default=None)
-    billing_shop_item_type: Optional[Union[BillingShopItemType, Unknown]] = field(
-        default=None
-    )
+    billing_shop_item_type: Optional[
+        Union[pjenums.BillingShopItemType, Unknown]
+    ] = field(default=None)
     billing_product_group_id: Optional[int] = field(default=None)
     name: Optional[str] = field(default=None)
     description: Optional[str] = field(default=None)
-    billable_limit_type: Optional[Union[BillableLimitType, Unknown]] = field(
+    billable_limit_type: Optional[Union[pjenums.BillableLimitType, Unknown]] = field(
         default=None
     )
     billable_limit_reset_interval_type: Optional[
-        Union[BillableLimitResetIntervalType, Unknown]
+        Union[pjenums.BillableLimitResetIntervalType, Unknown]
     ] = field(default=None)
     asset_bundle_name: Optional[str] = field(default=None)
     resource_box_id: Optional[int] = field(default=None)
     billable_limit_value: Optional[int] = field(default=None)
     bonus_resource_box_id: Optional[int] = field(default=None)
     label: Optional[str] = field(default=None)
     end_at: Optional[datetime] = field(default=None)
     start_at: Optional[datetime] = field(default=None)
     billable_limit_reset_interval_value: Optional[int] = field(default=None)
-    purchase_option: Optional[Union[PurchaseOption, Unknown]] = field(default=None)
+    purchase_option: Optional[Union[pjenums.PurchaseOption, Unknown]] = field(
+        default=None
+    )
 
 
 @dataclass(slots=True)
 class BillingShopItemExchangeCost(Cost):
     id: Optional[int] = field(default=None)
     billing_shop_item_id: Optional[int] = field(default=None)
 
@@ -1117,15 +1173,15 @@
     live_point_multiple: Optional[int] = field(default=None)
 
 
 @dataclass(slots=True)
 class JewelBehavior:
     id: Optional[int] = field(default=None)
     seq: Optional[int] = field(default=None)
-    jewel_behavior_type: Optional[Union[JewelBehaviorType, Unknown]] = field(
+    jewel_behavior_type: Optional[Union[pjenums.JewelBehaviorType, Unknown]] = field(
         default=None
     )
     jewel_behavior_type_quantity: Optional[int] = field(default=None)
     amount: Optional[int] = field(default=None)
 
 
 @dataclass(slots=True)
@@ -1149,17 +1205,17 @@
         list[CharacterRankAchieveResource]
     ] = field(default=None)
 
 
 @dataclass(slots=True)
 class CharacterMissionV2:
     id: Optional[int] = field(default=None)
-    character_mission_type: Optional[Union[CharacterMissionType, Unknown]] = field(
-        default=None
-    )
+    character_mission_type: Optional[
+        Union[pjenums.CharacterMissionType, Unknown]
+    ] = field(default=None)
     character_id: Optional[int] = field(default=None)
     parameter_group_id: Optional[int] = field(default=None)
     sentence: Optional[str] = field(default=None)
     progress_sentence: Optional[str] = field(default=None)
     is_achievement_mission: Optional[bool] = field(default=None)
 
 
@@ -1170,87 +1226,89 @@
     requirement: Optional[int] = field(default=None)
     exp: Optional[int] = field(default=None)
 
 
 @dataclass(slots=True)
 class CharacterMissionV2AreaItem:
     id: Optional[int] = field(default=None)
-    character_mission_type: Optional[Union[CharacterMissionType, Unknown]] = field(
-        default=None
-    )
+    character_mission_type: Optional[
+        Union[pjenums.CharacterMissionType, Unknown]
+    ] = field(default=None)
     area_item_id: Optional[int] = field(default=None)
     character_id: Optional[int] = field(default=None)
-    unit: Optional[Union[Unit, Unknown]] = field(default=None)
+    unit: Optional[Union[pjenums.Unit, Unknown]] = field(default=None)
 
 
 @dataclass(slots=True)
 class SystemLive2d(Live2d):
     serif: Optional[str] = field(default=None)
     voice: Optional[str] = field(default=None)
     published_at: Optional[datetime] = field(default=None)
     closed_at: Optional[datetime] = field(default=None)
     special_season_id: Optional[int] = field(default=None)
 
 
 @dataclass(slots=True)
 class Reward:
     id: Optional[int] = field(default=None)
-    mission_type: Optional[Union[MissionType, Unknown]] = field(default=None)
+    mission_type: Optional[Union[pjenums.MissionType, Unknown]] = field(default=None)
     mission_id: Optional[int] = field(default=None)
     seq: Optional[int] = field(default=None)
     resource_box_id: Optional[int] = field(default=None)
 
 
 @dataclass(slots=True)
 class NormalMission:
     id: Optional[int] = field(default=None)
     seq: Optional[int] = field(default=None)
-    normal_mission_type: Optional[Union[NormalMissionType, Unknown]] = field(
+    normal_mission_type: Optional[Union[pjenums.NormalMissionType, Unknown]] = field(
         default=None
     )
     requirement: Optional[int] = field(default=None)
     sentence: Optional[str] = field(default=None)
     rewards: Optional[list[Reward]] = field(default=None)
 
 
 @dataclass(slots=True)
 class BeginnerMission:
     id: Optional[int] = field(default=None)
     seq: Optional[int] = field(default=None)
-    beginner_mission_type: Optional[Union[BeginnerMissionType, Unknown]] = field(
-        default=None
-    )
+    beginner_mission_type: Optional[
+        Union[pjenums.BeginnerMissionType, Unknown]
+    ] = field(default=None)
     beginner_mission_category: Optional[
-        Union[BeginnerMissionCategory, Unknown]
+        Union[pjenums.BeginnerMissionCategory, Unknown]
     ] = field(default=None)
     requirement: Optional[int] = field(default=None)
     sentence: Optional[str] = field(default=None)
     rewards: Optional[list[Reward]] = field(default=None)
 
 
 @dataclass(slots=True)
 class Detail:
-    resource_box_purpose: Optional[Union[ResourceBoxPurpose, Unknown]] = field(
+    resource_box_purpose: Optional[Union[pjenums.ResourceBoxPurpose, Unknown]] = field(
         default=None
     )
     resource_box_id: Optional[int] = field(default=None)
     seq: Optional[int] = field(default=None)
-    resource_type: Optional[Union[ResourceType, Unknown]] = field(default=None)
+    resource_type: Optional[Union[pjenums.ResourceType, Unknown]] = field(default=None)
     resource_quantity: Optional[int] = field(default=None)
     resource_id: Optional[int] = field(default=None)
     resource_level: Optional[int] = field(default=None)
 
 
 @dataclass(slots=True)
 class ResourceBox:
-    resource_box_purpose: Optional[Union[ResourceBoxPurpose, Unknown]] = field(
+    resource_box_purpose: Optional[Union[pjenums.ResourceBoxPurpose, Unknown]] = field(
         default=None
     )
     id: Optional[int] = field(default=None)
-    resource_box_type: Optional[Union[ResourceBoxType, Unknown]] = field(default=None)
+    resource_box_type: Optional[Union[pjenums.ResourceBoxType, Unknown]] = field(
+        default=None
+    )
     details: Optional[list[Detail]] = field(default=None)
     description: Optional[str] = field(default=None)
     name: Optional[str] = field(default=None)
     asset_bundle_name: Optional[str] = field(default=None)
 
 
 @dataclass(slots=True)
@@ -1261,15 +1319,17 @@
     sentence: Optional[str] = field(default=None)
 
 
 @dataclass(slots=True)
 class LiveMission:
     id: Optional[int] = field(default=None)
     live_mission_period_id: Optional[int] = field(default=None)
-    live_mission_type: Optional[Union[LiveMissionType, Unknown]] = field(default=None)
+    live_mission_type: Optional[Union[pjenums.LiveMissionType, Unknown]] = field(
+        default=None
+    )
     requirement: Optional[int] = field(default=None)
     rewards: Optional[list[Reward]] = field(default=None)
 
 
 @dataclass(slots=True)
 class LiveMissionPass:
     id: Optional[int] = field(default=None)
@@ -1285,30 +1345,30 @@
 class PenlightColor:
     id: Optional[int] = field(default=None)
     seq: Optional[int] = field(default=None)
     name: Optional[str] = field(default=None)
     description: Optional[str] = field(default=None)
     color_code: Optional[str] = field(default=None)
     character_id: Optional[int] = field(default=None)
-    unit: Optional[Union[Unit, Unknown]] = field(default=None)
+    unit: Optional[Union[pjenums.Unit, Unknown]] = field(default=None)
 
 
 @dataclass(slots=True)
 class Penlight:
     id: Optional[int] = field(default=None)
     seq: Optional[int] = field(default=None)
     name: Optional[str] = field(default=None)
     default_penlight_color_id: Optional[int] = field(default=None)
     asset_bundle_name: Optional[str] = field(default=None)
 
 
 @dataclass(slots=True)
 class LiveTalk:
     id: Optional[int] = field(default=None)
-    live_talk_type: Optional[Union[LiveTalkType, Unknown]] = field(default=None)
+    live_talk_type: Optional[Union[pjenums.LiveTalkType, Unknown]] = field(default=None)
     scenario_id: Optional[str] = field(default=None)
     character_id1: Optional[int] = field(default=None)
     character_id2: Optional[int] = field(default=None)
 
 
 @dataclass(slots=True)
 class Tip:
@@ -1352,15 +1412,15 @@
     end_at: Optional[datetime] = field(default=None)
     gacha_ceil_exchange_cost: Optional[GachaCeilExchangeCost] = field(default=None)
     gacha_ceil_exchange_substitute_costs: Optional[
         list[GachaCeilExchangeSubstituteCost]
     ] = field(default=None)
     exchange_limit: Optional[int] = field(default=None)
     gacha_ceil_exchange_label_type: Optional[
-        Union[GachaCeilExchangeLabelType, Unknown]
+        Union[pjenums.GachaCeilExchangeLabelType, Unknown]
     ] = field(default=None)
     substitute_limit: Optional[int] = field(default=None)
 
 
 @dataclass(slots=True)
 class GachaCeilExchangeSummary:
     id: Optional[int] = field(default=None)
@@ -1388,15 +1448,15 @@
     asset_bundle_name: Optional[str] = field(default=None)
 
 
 @dataclass(slots=True)
 class HonorGroup:
     id: Optional[int] = field(default=None)
     name: Optional[str] = field(default=None)
-    honor_type: Optional[Union[HonorType, Unknown]] = field(default=None)
+    honor_type: Optional[Union[pjenums.HonorType, Unknown]] = field(default=None)
     archive_published_at: Optional[datetime] = field(default=None)
     background_asset_bundle_name: Optional[str] = field(default=None)
 
 
 @dataclass(slots=True)
 class HonorLevel:
     honor_id: Optional[int] = field(default=None)
@@ -1406,26 +1466,28 @@
 
 
 @dataclass(slots=True)
 class Honor:
     id: Optional[int] = field(default=None)
     seq: Optional[int] = field(default=None)
     group_id: Optional[int] = field(default=None)
-    honor_rarity: Optional[Union[HonorRarity, Unknown]] = field(default=None)
+    honor_rarity: Optional[Union[pjenums.HonorRarity, Unknown]] = field(default=None)
     name: Optional[str] = field(default=None)
     asset_bundle_name: Optional[str] = field(default=None)
     levels: Optional[list[HonorLevel]] = field(default=None)
     honor_type_id: Optional[int] = field(default=None)
 
 
 @dataclass(slots=True)
 class HonorMission:
     id: Optional[int] = field(default=None)
     seq: Optional[int] = field(default=None)
-    honor_mission_type: Optional[Union[HonorMissionType, Unknown]] = field(default=None)
+    honor_mission_type: Optional[Union[pjenums.HonorMissionType, Unknown]] = field(
+        default=None
+    )
     requirement: Optional[int] = field(default=None)
     sentence: Optional[str] = field(default=None)
     rewards: Optional[list[Reward]] = field(default=None)
 
 
 @dataclass(slots=True)
 class BondsHonorLevel:
@@ -1438,15 +1500,15 @@
 @dataclass(slots=True)
 class BondsHonor:
     id: Optional[int] = field(default=None)
     seq: Optional[int] = field(default=None)
     bonds_group_id: Optional[int] = field(default=None)
     game_character_unit_id1: Optional[int] = field(default=None)
     game_character_unit_id2: Optional[int] = field(default=None)
-    honor_rarity: Optional[Union[HonorRarity, Unknown]] = field(default=None)
+    honor_rarity: Optional[Union[pjenums.HonorRarity, Unknown]] = field(default=None)
     name: Optional[str] = field(default=None)
     description: Optional[str] = field(default=None)
     levels: Optional[list[BondsHonorLevel]] = field(default=None)
     configurable_unit_virtual_singer: Optional[bool] = field(default=None)
 
 
 @dataclass(slots=True)
@@ -1461,24 +1523,28 @@
 
 @dataclass(slots=True)
 class BondsReward:
     id: Optional[int] = field(default=None)
     bonds_group_id: Optional[int] = field(default=None)
     rank: Optional[int] = field(default=None)
     seq: Optional[int] = field(default=None)
-    bonds_reward_type: Optional[Union[BondsRewardType, Unknown]] = field(default=None)
+    bonds_reward_type: Optional[Union[pjenums.BondsRewardType, Unknown]] = field(
+        default=None
+    )
     resource_box_id: Optional[int] = field(default=None)
     description: Optional[str] = field(default=None)
 
 
 @dataclass(slots=True)
 class ChallengeLiveDetail:
     id: Optional[int] = field(default=None)
     challenge_live_id: Optional[int] = field(default=None)
-    challenge_live_type: Optional[Union[LiveType, Unknown]] = field(default=None)
+    challenge_live_type: Optional[Union[pjenums.LiveType, Unknown]] = field(
+        default=None
+    )
 
 
 @dataclass(slots=True)
 class ChallengeLive:
     id: Optional[int] = field(default=None)
     playable_count: Optional[int] = field(default=None)
     challenge_live_details: Optional[list[ChallengeLiveDetail]] = field(default=None)
@@ -1552,17 +1618,17 @@
 
 
 @dataclass(slots=True)
 class VirtualLiveSetlist:
     id: Optional[int] = field(default=None)
     virtual_live_id: Optional[int] = field(default=None)
     seq: Optional[int] = field(default=None)
-    virtual_live_setlist_type: Optional[Union[VirtualLiveSetlistType, Unknown]] = field(
-        default=None
-    )
+    virtual_live_setlist_type: Optional[
+        Union[pjenums.VirtualLiveSetlistType, Unknown]
+    ] = field(default=None)
     asset_bundle_name: Optional[str] = field(default=None)
     virtual_live_stage_id: Optional[int] = field(default=None)
     music_id: Optional[int] = field(default=None)
     music_vocal_id: Optional[int] = field(default=None)
     character3d_id1: Optional[int] = field(default=None)
     character3d_id2: Optional[int] = field(default=None)
     character3d_id3: Optional[int] = field(default=None)
@@ -1571,15 +1637,15 @@
     character3d_id6: Optional[int] = field(default=None)
 
 
 @dataclass(slots=True)
 class VirtualLiveBeginnerSchedule:
     id: Optional[int] = field(default=None)
     virtual_live_id: Optional[int] = field(default=None)
-    day_of_week: Optional[Union[DayOfWeek, Unknown]] = field(default=None)
+    day_of_week: Optional[Union[pjenums.DayOfWeek, Unknown]] = field(default=None)
     start_time: Optional[str] = field(default=None)
     end_time: Optional[str] = field(default=None)
 
 
 @dataclass(slots=True)
 class VirtualLiveSchedule:
     id: Optional[int] = field(default=None)
@@ -1597,15 +1663,17 @@
     game_character_unit_id: Optional[int] = field(default=None)
     seq: Optional[int] = field(default=None)
 
 
 @dataclass(slots=True)
 class VirtualLiveReward:
     id: Optional[int] = field(default=None)
-    virtual_live_type: Optional[Union[VirtualLiveType, Unknown]] = field(default=None)
+    virtual_live_type: Optional[Union[pjenums.VirtualLiveType, Unknown]] = field(
+        default=None
+    )
     virtual_live_id: Optional[int] = field(default=None)
     resource_box_id: Optional[int] = field(default=None)
 
 
 @dataclass(slots=True)
 class VirtualLiveWaitingRoom:
     id: Optional[int] = field(default=None)
@@ -1615,56 +1683,58 @@
     end_at: Optional[datetime] = field(default=None)
     lobby_asset_bundle_name: Optional[str] = field(default=None)
 
 
 @dataclass(slots=True)
 class VirtualItem:
     id: Optional[int] = field(default=None)
-    virtual_item_category: Optional[Union[VirtualItemCategory, Unknown]] = field(
-        default=None
-    )
+    virtual_item_category: Optional[
+        Union[pjenums.VirtualItemCategory, Unknown]
+    ] = field(default=None)
     seq: Optional[int] = field(default=None)
     priority: Optional[int] = field(default=None)
     name: Optional[str] = field(default=None)
     asset_bundle_name: Optional[str] = field(default=None)
     cost_virtual_coin: Optional[int] = field(default=None)
     cost_jewel: Optional[int] = field(default=None)
     cheer_point: Optional[int] = field(default=None)
     effect_asset_bundle_name: Optional[str] = field(default=None)
-    effect_expression_type: Optional[Union[EffectExpressionType, Unknown]] = field(
-        default=None
-    )
-    unit: Optional[Union[Unit, Unknown]] = field(default=None)
+    effect_expression_type: Optional[
+        Union[pjenums.EffectExpressionType, Unknown]
+    ] = field(default=None)
+    unit: Optional[Union[pjenums.Unit, Unknown]] = field(default=None)
     game_character_unit_id: Optional[int] = field(default=None)
-    virtual_item_label_type: Optional[Union[VirtualItemLabelType, Unknown]] = field(
-        default=None
-    )
+    virtual_item_label_type: Optional[
+        Union[pjenums.VirtualItemLabelType, Unknown]
+    ] = field(default=None)
 
 
 @dataclass(slots=True)
 class VirtualLiveAppeal:
     id: Optional[int] = field(default=None)
     virtual_live_id: Optional[int] = field(default=None)
-    virtual_live_stage_status: Optional[Union[VirtualLiveStageStatus, Unknown]] = field(
-        default=None
-    )
+    virtual_live_stage_status: Optional[
+        Union[pjenums.VirtualLiveStageStatus, Unknown]
+    ] = field(default=None)
     appeal_text: Optional[str] = field(default=None)
 
 
 @dataclass(slots=True)
 class VirtualLiveInformation:
     virtual_live_id: Optional[int] = field(default=None)
     summary: Optional[str] = field(default=None)
     description: Optional[str] = field(default=None)
 
 
 @dataclass(slots=True)
 class VirtualLive:
     id: Optional[int] = field(default=None)
-    virtual_live_type: Optional[Union[VirtualLiveType, Unknown]] = field(default=None)
+    virtual_live_type: Optional[Union[pjenums.VirtualLiveType, Unknown]] = field(
+        default=None
+    )
     virtual_live_platform: Optional[str] = field(default=None)
     seq: Optional[int] = field(default=None)
     name: Optional[str] = field(default=None)
     asset_bundle_name: Optional[str] = field(default=None)
     screen_mv_music_vocal_id: Optional[int] = field(default=None)
     start_at: Optional[datetime] = field(default=None)
     end_at: Optional[datetime] = field(default=None)
@@ -1688,17 +1758,17 @@
     virtual_live_ticket_id: Optional[int] = field(default=None)
 
 
 @dataclass(slots=True)
 class VirtualShopItem:
     id: Optional[int] = field(default=None)
     virtual_shop_id: Optional[int] = field(default=None)
-    virtual_shop_item_type: Optional[Union[VirtualShopItemType, Unknown]] = field(
-        default=None
-    )
+    virtual_shop_item_type: Optional[
+        Union[pjenums.VirtualShopItemType, Unknown]
+    ] = field(default=None)
     seq: Optional[int] = field(default=None)
     resource_box_id: Optional[int] = field(default=None)
     cost_virtual_coin: Optional[int] = field(default=None)
     cost_jewel: Optional[int] = field(default=None)
     start_at: Optional[datetime] = field(default=None)
     cost_paid_jewel: Optional[int] = field(default=None)
     end_at: Optional[datetime] = field(default=None)
@@ -1707,23 +1777,27 @@
 
 @dataclass(slots=True)
 class VirtualShop:
     id: Optional[int] = field(default=None)
     seq: Optional[int] = field(default=None)
     name: Optional[str] = field(default=None)
     virtual_shop_items: Optional[list[VirtualShopItem]] = field(default=None)
-    virtual_shop_type: Optional[Union[VirtualShopType, Unknown]] = field(default=None)
+    virtual_shop_type: Optional[Union[pjenums.VirtualShopType, Unknown]] = field(
+        default=None
+    )
     virtual_live_id: Optional[int] = field(default=None)
 
 
 @dataclass(slots=True)
 class VirtualLiveCheerMessage:
     id: Optional[int] = field(default=None)
-    virtual_live_type: Optional[Union[VirtualLiveType, Unknown]] = field(default=None)
-    resource_type: Optional[Union[ResourceType, Unknown]] = field(default=None)
+    virtual_live_type: Optional[Union[pjenums.VirtualLiveType, Unknown]] = field(
+        default=None
+    )
+    resource_type: Optional[Union[pjenums.ResourceType, Unknown]] = field(default=None)
     from_cost_virtual_coin: Optional[int] = field(default=None)
     to_cost_virtual_coin: Optional[int] = field(default=None)
     from_cost: Optional[int] = field(default=None)
     to_cost: Optional[int] = field(default=None)
     asset_bundle_name: Optional[str] = field(default=None)
     message_length_limit: Optional[int] = field(default=None)
     display_sec: Optional[float] = field(default=None)
@@ -1738,17 +1812,17 @@
     display_limit: Optional[int] = field(default=None)
 
 
 @dataclass(slots=True)
 class VirtualLiveTicket:
     id: Optional[int] = field(default=None)
     virtual_live_id: Optional[int] = field(default=None)
-    virtual_live_ticket_type: Optional[Union[VirtualLiveTicketType, Unknown]] = field(
-        default=None
-    )
+    virtual_live_ticket_type: Optional[
+        Union[pjenums.VirtualLiveTicketType, Unknown]
+    ] = field(default=None)
     name: Optional[str] = field(default=None)
     flavor_text: Optional[str] = field(default=None)
     asset_bundle_name: Optional[str] = field(default=None)
 
 
 @dataclass(slots=True)
 class VirtualLivePamphlet:
@@ -1760,15 +1834,15 @@
 
 
 @dataclass(slots=True)
 class AvatarAccessory:
     id: Optional[int] = field(default=None)
     seq: Optional[int] = field(default=None)
     name: Optional[str] = field(default=None)
-    part: Optional[Union[AccessoryPart, Unknown]] = field(default=None)
+    part: Optional[Union[pjenums.AccessoryPart, Unknown]] = field(default=None)
     asset_bundle_name: Optional[str] = field(default=None)
 
 
 @dataclass(slots=True)
 class AvatarCostume:
     id: Optional[int] = field(default=None)
     seq: Optional[int] = field(default=None)
@@ -1798,45 +1872,49 @@
 class AvatarCoordinate:
     id: Optional[int] = field(default=None)
     seq: Optional[int] = field(default=None)
     name: Optional[str] = field(default=None)
     asset_bundle_name: Optional[str] = field(default=None)
     skin_color_code: Optional[str] = field(default=None)
     costume_asset_bundle_name: Optional[str] = field(default=None)
-    accessory_part: Optional[Union[AccessoryPart, Unknown]] = field(default=None)
+    accessory_part: Optional[Union[pjenums.AccessoryPart, Unknown]] = field(
+        default=None
+    )
     accessory_asset_bundle_name: Optional[str] = field(default=None)
 
 
 @dataclass(slots=True)
 class NgWord:
     id: Optional[int] = field(default=None)
     word: Optional[str] = field(default=None)
 
 
 @dataclass(slots=True)
 class RuleSlide:
     id: Optional[int] = field(default=None)
-    rule_slide_type: Optional[Union[RuleSlideType, Unknown]] = field(default=None)
+    rule_slide_type: Optional[Union[pjenums.RuleSlideType, Unknown]] = field(
+        default=None
+    )
     asset_bundle_name: Optional[str] = field(default=None)
 
 
 @dataclass(slots=True)
 class Facility:
     id: Optional[int] = field(default=None)
-    facility_type: Optional[Union[FacilityType, Unknown]] = field(default=None)
+    facility_type: Optional[Union[pjenums.FacilityType, Unknown]] = field(default=None)
     release_condition_id: Optional[int] = field(default=None)
     and_release_condition_id: Optional[int] = field(default=None)
 
 
 @dataclass(slots=True)
 class OneTimeBehavior:
     id: Optional[int] = field(default=None)
-    one_time_behavior_type: Optional[Union[OneTimeBehaviorType, Unknown]] = field(
-        default=None
-    )
+    one_time_behavior_type: Optional[
+        Union[pjenums.OneTimeBehaviorType, Unknown]
+    ] = field(default=None)
     release_condition_id: Optional[int] = field(default=None)
 
 
 @dataclass(slots=True)
 class LoginBonus:
     id: Optional[int] = field(default=None)
     day: Optional[int] = field(default=None)
@@ -1904,26 +1982,26 @@
     to_rank: Optional[int] = field(default=None)
     event_ranking_rewards: Optional[list[EventRankingReward]] = field(default=None)
 
 
 @dataclass(slots=True)
 class Event:
     id: Optional[int] = field(default=None)
-    event_type: Optional[Union[EventType, Unknown]] = field(default=None)
+    event_type: Optional[Union[pjenums.EventType, Unknown]] = field(default=None)
     name: Optional[str] = field(default=None)
     asset_bundle_name: Optional[str] = field(default=None)
     bgm_asset_bundle_name: Optional[str] = field(default=None)
     start_at: Optional[datetime] = field(default=None)
     aggregate_at: Optional[datetime] = field(default=None)
     ranking_announce_at: Optional[datetime] = field(default=None)
     distribution_start_at: Optional[datetime] = field(default=None)
     closed_at: Optional[datetime] = field(default=None)
     distribution_end_at: Optional[datetime] = field(default=None)
     virtual_live_id: Optional[int] = field(default=None)
-    unit: Optional[Union[Unit, Unknown]] = field(default=None)
+    unit: Optional[Union[pjenums.Unit, Unknown]] = field(default=None)
     event_ranking_reward_ranges: Optional[list[EventRankingRewardRange]] = field(
         default=None
     )
     event_point_asset_bundle_name: Optional[str] = field(default=None)
 
 
 @dataclass(slots=True)
@@ -1935,22 +2013,24 @@
 
 
 @dataclass(slots=True)
 class EventDeckBonus:
     id: Optional[int] = field(default=None)
     event_id: Optional[int] = field(default=None)
     game_character_unit_id: Optional[int] = field(default=None)
-    card_attr: Optional[Union[CardAttr, Unknown]] = field(default=None)
+    card_attr: Optional[Union[pjenums.CardAttr, Unknown]] = field(default=None)
     bonus_rate: Optional[float] = field(default=None)
 
 
 @dataclass(slots=True)
 class EventRarityBonusRate:
     id: Optional[int] = field(default=None)
-    card_rarity_type: Optional[Union[CardRarityType, Unknown]] = field(default=None)
+    card_rarity_type: Optional[Union[pjenums.CardRarityType, Unknown]] = field(
+        default=None
+    )
     master_rank: Optional[int] = field(default=None)
     bonus_rate: Optional[float] = field(default=None)
 
 
 @dataclass(slots=True)
 class EventItem:
     id: Optional[int] = field(default=None)
@@ -1958,15 +2038,15 @@
     name: Optional[str] = field(default=None)
     flavor_text: Optional[str] = field(default=None)
     asset_bundle_name: Optional[str] = field(default=None)
 
 
 @dataclass(slots=True)
 class EpisodeReward:
-    story_type: Optional[Union[StoryType, Unknown]] = field(default=None)
+    story_type: Optional[Union[pjenums.StoryType, Unknown]] = field(default=None)
     resource_box_id: Optional[int] = field(default=None)
 
 
 @dataclass(slots=True)
 class EventStoryEpisode:
     id: Optional[int] = field(default=None)
     event_story_id: Optional[int] = field(default=None)
@@ -2013,18 +2093,18 @@
 
 
 @dataclass(slots=True)
 class EventStoryUnit:
     id: Optional[int] = field(default=None)
     seq: Optional[int] = field(default=None)
     event_story_id: Optional[int] = field(default=None)
-    unit: Optional[Union[Unit, Unknown]] = field(default=None)
-    event_story_unit_relation: Optional[Union[EventStoryUnitRelation, Unknown]] = field(
-        default=None
-    )
+    unit: Optional[Union[pjenums.Unit, Unknown]] = field(default=None)
+    event_story_unit_relation: Optional[
+        Union[pjenums.EventStoryUnitRelation, Unknown]
+    ] = field(default=None)
 
 
 @dataclass(slots=True)
 class EventCard:
     id: Optional[int] = field(default=None)
     card_id: Optional[int] = field(default=None)
     event_id: Optional[int] = field(default=None)
@@ -2046,15 +2126,15 @@
     music_id: Optional[int] = field(default=None)
 
 
 @dataclass(slots=True)
 class PreliminaryTournament:
     id: Optional[int] = field(default=None)
     preliminary_tournament_type: Optional[
-        Union[PreliminaryTournamentType, Unknown]
+        Union[pjenums.PreliminaryTournamentType, Unknown]
     ] = field(default=None)
     start_at: Optional[datetime] = field(default=None)
     end_at: Optional[datetime] = field(default=None)
     release_condition_id: Optional[int] = field(default=None)
     preliminary_tournament_cards: Optional[list[PreliminaryTournamentCard]] = field(
         default=None
     )
@@ -2115,32 +2195,34 @@
 
 
 @dataclass(slots=True)
 class CheerfulCarnivalResultReward:
     id: Optional[int] = field(default=None)
     event_id: Optional[int] = field(default=None)
     cheerful_carnival_team_point_term_type: Optional[
-        Union[CheerfulCarnivalTeamPointTermType, Unknown]
+        Union[pjenums.CheerfulCarnivalTeamPointTermType, Unknown]
     ] = field(default=None)
     cheerful_carnival_result_type: Optional[
-        Union[CheerfulCarnivalResultType, Unknown]
+        Union[pjenums.CheerfulCarnivalResultType, Unknown]
     ] = field(default=None)
     resource_box_id: Optional[int] = field(default=None)
 
 
 @dataclass(slots=True)
 class Appeal:
     id: Optional[int] = field(default=None)
     seq: Optional[int] = field(default=None)
-    appeal_target_type: Optional[Union[AppealTargetType, Unknown]] = field(default=None)
-    appeal_type: Optional[Union[AppealType, Unknown]] = field(default=None)
+    appeal_target_type: Optional[Union[pjenums.AppealTargetType, Unknown]] = field(
+        default=None
+    )
+    appeal_type: Optional[Union[pjenums.AppealType, Unknown]] = field(default=None)
     start_at: Optional[datetime] = field(default=None)
     end_at: Optional[datetime] = field(default=None)
     appeal_read_condition_type: Optional[
-        Union[AppealReadConditionType, Unknown]
+        Union[pjenums.AppealReadConditionType, Unknown]
     ] = field(default=None)
     text: Optional[str] = field(default=None)
 
 
 @dataclass(slots=True)
 class Boost:
     id: Optional[int] = field(default=None)
@@ -2170,15 +2252,15 @@
 
 
 @dataclass(slots=True)
 class EpisodeCharacter:
     id: Optional[int] = field(default=None)
     seq: Optional[int] = field(default=None)
     character2d_id: Optional[int] = field(default=None)
-    story_type: Optional[Union[StoryType, Unknown]] = field(default=None)
+    story_type: Optional[Union[pjenums.StoryType, Unknown]] = field(default=None)
     episode_id: Optional[int] = field(default=None)
 
 
 @dataclass(slots=True)
 class CustomProfileTextColor:
     id: Optional[int] = field(default=None)
     seq: Optional[int] = field(default=None)
@@ -2192,20 +2274,22 @@
     font_name: Optional[str] = field(default=None)
     asset_bundle_name: Optional[str] = field(default=None)
 
 
 @dataclass(slots=True)
 class CustomProfileResource:
     custom_profile_resource_type: Optional[
-        Union[CustomProfileResourceType, Unknown]
+        Union[pjenums.CustomProfileResourceType, Unknown]
     ] = field(default=None)
     id: Optional[int] = field(default=None)
     seq: Optional[int] = field(default=None)
     name: Optional[str] = field(default=None)
-    resource_load_type: Optional[Union[ResourceLoadType, Unknown]] = field(default=None)
+    resource_load_type: Optional[Union[pjenums.ResourceLoadType, Unknown]] = field(
+        default=None
+    )
     resource_load_val: Optional[str] = field(default=None)
     file_name: Optional[str] = field(default=None)
 
 
 @dataclass(slots=True)
 class CustomProfilePlayerInfoResource(CustomProfileResource):
     pass
@@ -2220,15 +2304,15 @@
 class CustomProfileStoryBackgroundResource(CustomProfileResource):
     pass
 
 
 @dataclass(slots=True)
 class CustomProfileCollectionResource(CustomProfileResource):
     custom_profile_resource_collection_type: Optional[
-        Union[CustomProfileResourceCollectionType, Unknown]
+        Union[pjenums.CustomProfileResourceCollectionType, Unknown]
     ] = field(default=None)
     group_id: Optional[int] = field(default=None)
 
 
 @dataclass(slots=True)
 class CustomProfileMemberStandingPictureResource(CustomProfileResource):
     character_id: Optional[int] = field(default=None)
@@ -2245,25 +2329,27 @@
 
 
 @dataclass(slots=True)
 class CustomProfileGachaBehavior:
     id: Optional[int] = field(default=None)
     custom_profile_gacha_id: Optional[int] = field(default=None)
     seq: Optional[int] = field(default=None)
-    cost_resource_type: Optional[Union[ResourceType, Unknown]] = field(default=None)
+    cost_resource_type: Optional[Union[pjenums.ResourceType, Unknown]] = field(
+        default=None
+    )
     cost_resource_quantity: Optional[int] = field(default=None)
     spin_count: Optional[int] = field(default=None)
 
 
 @dataclass(slots=True)
 class CustomProfileGachaDetail:
     id: Optional[int] = field(default=None)
     custom_profile_gacha_id: Optional[int] = field(default=None)
     custom_profile_resource_type: Optional[
-        Union[CustomProfileResourceType, Unknown]
+        Union[pjenums.CustomProfileResourceType, Unknown]
     ] = field(default=None)
     custom_profile_resource_id: Optional[int] = field(default=None)
     custom_profile_resource_quantity: Optional[int] = field(default=None)
     weight: Optional[int] = field(default=None)
 
 
 @dataclass(slots=True)
@@ -2291,16 +2377,16 @@
     music_vocal_id: Optional[int] = field(default=None)
 
 
 @dataclass(slots=True)
 class Omikuji:
     id: Optional[int] = field(default=None)
     omikuji_group_id: Optional[int] = field(default=None)
-    unit: Optional[Union[Unit, Unknown]] = field(default=None)
-    fortune_type: Optional[Union[FortuneType, Unknown]] = field(default=None)
+    unit: Optional[Union[pjenums.Unit, Unknown]] = field(default=None)
+    fortune_type: Optional[Union[pjenums.FortuneType, Unknown]] = field(default=None)
     summary: Optional[str] = field(default=None)
     title1: Optional[str] = field(default=None)
     description1: Optional[str] = field(default=None)
     title2: Optional[str] = field(default=None)
     description2: Optional[str] = field(default=None)
     title3: Optional[str] = field(default=None)
     description3: Optional[str] = field(default=None)
@@ -2323,15 +2409,15 @@
     sound_asset_bundle_name: Optional[str] = field(default=None)
 
 
 @dataclass(slots=True)
 class OmikujiRate:
     id: Optional[int] = field(default=None)
     omikuji_group_id: Optional[int] = field(default=None)
-    fortune_type: Optional[Union[FortuneType, Unknown]] = field(default=None)
+    fortune_type: Optional[Union[pjenums.FortuneType, Unknown]] = field(default=None)
     rate: Optional[float] = field(default=None)
 
 
 @dataclass(slots=True)
 class OmikujiCost(Cost):
     id: Optional[int] = field(default=None)
     omikuji_group_id: Optional[int] = field(default=None)
@@ -2339,33 +2425,33 @@
 
 
 @dataclass(slots=True)
 class OmikujiReward:
     id: Optional[int] = field(default=None)
     omikuji_group_id: Optional[int] = field(default=None)
     seq: Optional[int] = field(default=None)
-    resource_type: Optional[Union[ResourceType, Unknown]] = field(default=None)
+    resource_type: Optional[Union[pjenums.ResourceType, Unknown]] = field(default=None)
     resource_id: Optional[int] = field(default=None)
     resource_quantity: Optional[int] = field(default=None)
 
 
 @dataclass(slots=True)
 class VirtualBoothShop:
     id: Optional[int] = field(default=None)
     virtual_live_id: Optional[int] = field(default=None)
-    virtual_booth_shop_type: Optional[Union[VirtualBoothShopType, Unknown]] = field(
-        default=None
-    )
+    virtual_booth_shop_type: Optional[
+        Union[pjenums.VirtualBoothShopType, Unknown]
+    ] = field(default=None)
     target_id: Optional[int] = field(default=None)
 
 
 @dataclass(slots=True)
 class SpecialSeason:
     id: Optional[int] = field(default=None)
-    special_season_type: Optional[Union[SpecialSeasonType, Unknown]] = field(
+    special_season_type: Optional[Union[pjenums.SpecialSeasonType, Unknown]] = field(
         default=None
     )
     start_at: Optional[datetime] = field(default=None)
     end_at: Optional[datetime] = field(default=None)
     priority: Optional[int] = field(default=None)
 
 
@@ -2373,46 +2459,48 @@
 class SpecialSeasonArea:
     id: Optional[int] = field(default=None)
     special_season_id: Optional[int] = field(default=None)
     area_id: Optional[int] = field(default=None)
     asset_bundle_name: Optional[str] = field(default=None)
     file_name: Optional[str] = field(default=None)
     special_season_area_use_type: Optional[
-        Union[SpecialSeasonAreaUseType, Unknown]
+        Union[pjenums.SpecialSeasonAreaUseType, Unknown]
     ] = field(default=None)
 
 
 @dataclass(slots=True)
 class RankMatchPenalty:
     id: Optional[int] = field(default=None)
     count: Optional[int] = field(default=None)
-    rank_match_penalty_type: Optional[Union[RankMatchPenaltyType, Unknown]] = field(
-        default=None
-    )
+    rank_match_penalty_type: Optional[
+        Union[pjenums.RankMatchPenaltyType, Unknown]
+    ] = field(default=None)
     rank_match_penalty_type_value: Optional[int] = field(default=None)
 
 
 @dataclass(slots=True)
 class RankMatchPlacement:
     id: Optional[int] = field(default=None)
     rank_match_placement_condition_type: Optional[str] = field(default=None)
-    tier_behavior_type: Optional[Union[TierBehaviorType, Unknown]] = field(default=None)
+    tier_behavior_type: Optional[Union[pjenums.TierBehaviorType, Unknown]] = field(
+        default=None
+    )
     tier_behavior_type_value: Optional[int] = field(default=None)
     rank_match_placement_condition_type_value: Optional[int] = field(default=None)
 
 
 @dataclass(slots=True)
 class RankMatchBonusPointCondition:
     id: Optional[int] = field(default=None)
     rank_match_bonus_point_condition_type: Optional[
-        Union[RankMatchBonusPointConditionType, Unknown]
+        Union[pjenums.RankMatchBonusPointConditionType, Unknown]
     ] = field(default=None)
     group_id: Optional[int] = field(default=None)
     priority: Optional[int] = field(default=None)
-    calc_type: Optional[Union[CalcType, Unknown]] = field(default=None)
+    calc_type: Optional[Union[pjenums.CalcType, Unknown]] = field(default=None)
     bonus_point: Optional[int] = field(default=None)
 
 
 @dataclass(slots=True)
 class RankMatchSeasonPlayableTime:
     id: Optional[int] = field(default=None)
     rank_match_season_id: Optional[int] = field(default=None)
```

### Comparing `async_pjsekai-0.0.10.dev0/async_pjsekai/models/system_info.py` & `async_pjsekai-0.0.10.dev1/async_pjsekai/models/system_info.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 # SPDX-FileCopyrightText: 2023-present TheerapakG <theerapakg@gmail.com>
 #
 # SPDX-License-Identifier: MIT
 
 from dataclasses import dataclass, field, fields
 from typing import Optional, Union, Type, TypeVar
 
-from pjsekai.enums import *
+from async_pjsekai.enums.enums import AppVersionStatus
+from async_pjsekai.enums.unknown import Unknown
 
 
 T_SystemInfo = TypeVar("T_SystemInfo", bound="SystemInfo")
 
 
 @dataclass(frozen=True, slots=True)
 class SystemInfo:
```

### Comparing `async_pjsekai-0.0.10.dev0/pyproject.toml` & `async_pjsekai-0.0.10.dev1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "async-pjsekai"
-version = "0.0.10.dev0"
+version = "0.0.10.dev1"
 description = "Asynchronous reverse engineered client for the game Project SEKAI COLORFUL STAGE! feat. Hatsune Miku"
 readme = "README.md"
 repository = "https://github.com/TheerapakG/sekai-monorepo"
 license = "MIT"
 authors = [
     "TheerapakG <theerapakg@gmail.com>",
 ]
@@ -25,10 +25,12 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 
-pypjsekai = "^0.0.10"
-aiohttp = "^3.8.4"
-cattrs = "^22.2.0"
+aiohttp = "~3.8.4"
+cattrs = "~22.2.0"
+msgpack = "~1.0.5"
+pycryptodome = "~3.17"
+PyJWT = "~2.6.0"
```

### Comparing `async_pjsekai-0.0.10.dev0/PKG-INFO` & `async_pjsekai-0.0.10.dev1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: async-pjsekai
-Version: 0.0.10.dev0
+Version: 0.0.10.dev1
 Summary: Asynchronous reverse engineered client for the game Project SEKAI COLORFUL STAGE! feat. Hatsune Miku
 Home-page: https://github.com/TheerapakG/sekai-monorepo
 License: MIT
 Author: TheerapakG
 Author-email: theerapakg@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -15,17 +15,19 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
-Requires-Dist: cattrs (>=22.2.0,<23.0.0)
-Requires-Dist: pypjsekai (>=0.0.10,<0.0.11)
+Requires-Dist: PyJWT (>=2.6.0,<2.7.0)
+Requires-Dist: aiohttp (>=3.8.4,<3.9.0)
+Requires-Dist: cattrs (>=22.2.0,<22.3.0)
+Requires-Dist: msgpack (>=1.0.5,<1.1.0)
+Requires-Dist: pycryptodome (>=3.17,<3.18)
 Project-URL: Repository, https://github.com/TheerapakG/sekai-monorepo
 Description-Content-Type: text/markdown
 
 # async-pjsekai
 
 [![PyPI - Version](https://img.shields.io/pypi/v/async-pjsekai.svg)](https://pypi.org/project/async-pjsekai)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/async-pjsekai.svg)](https://pypi.org/project/async-pjsekai)
```

