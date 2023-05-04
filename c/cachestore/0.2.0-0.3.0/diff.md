# Comparing `tmp/cachestore-0.2.0.tar.gz` & `tmp/cachestore-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cachestore-0.2.0.tar", max compression
+gzip compressed data, was "cachestore-0.3.0.tar", max compression
```

## Comparing `cachestore-0.2.0.tar` & `cachestore-0.3.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1064 2022-08-14 11:47:07.815126 cachestore-0.2.0/LICENSE
--rw-r--r--   0        0        0     1630 2022-08-14 11:47:07.815126 cachestore-0.2.0/README.md
--rw-r--r--   0        0        0      526 2022-08-14 11:47:07.815126 cachestore-0.2.0/cachestore/__init__.py
--rw-r--r--   0        0        0      447 2022-08-14 11:47:07.815126 cachestore-0.2.0/cachestore/__main__.py
--rw-r--r--   0        0        0     8096 2022-08-14 11:47:07.815126 cachestore-0.2.0/cachestore/cache.py
--rw-r--r--   0        0        0      677 2022-08-14 11:47:07.815126 cachestore-0.2.0/cachestore/commands/__init__.py
--rw-r--r--   0        0        0     3762 2022-08-14 11:47:07.819126 cachestore-0.2.0/cachestore/commands/list.py
--rw-r--r--   0        0        0      965 2022-08-14 11:47:07.819126 cachestore-0.2.0/cachestore/commands/prune.py
--rw-r--r--   0        0        0     2217 2022-08-14 11:47:07.819126 cachestore-0.2.0/cachestore/commands/remove.py
--rw-r--r--   0        0        0     3633 2022-08-14 11:47:07.819126 cachestore-0.2.0/cachestore/commands/subcommand.py
--rw-r--r--   0        0        0      180 2022-08-14 11:47:07.819126 cachestore-0.2.0/cachestore/common/__init__.py
--rw-r--r--   0        0        0     1021 2022-08-14 11:47:07.819126 cachestore-0.2.0/cachestore/common/filelock.py
--rw-r--r--   0        0        0     2059 2022-08-14 11:47:07.819126 cachestore-0.2.0/cachestore/common/selector.py
--rw-r--r--   0        0        0     4515 2022-08-14 11:47:07.819126 cachestore-0.2.0/cachestore/common/table.py
--rw-r--r--   0        0        0     4993 2022-08-14 11:47:07.819126 cachestore-0.2.0/cachestore/config.py
--rw-r--r--   0        0        0      149 2022-08-14 11:47:07.819126 cachestore-0.2.0/cachestore/formatters/__init__.py
--rw-r--r--   0        0        0      565 2022-08-14 11:47:07.819126 cachestore-0.2.0/cachestore/formatters/formatter.py
--rw-r--r--   0        0        0      576 2022-08-14 11:47:07.819126 cachestore-0.2.0/cachestore/formatters/pickle_formatter.py
--rw-r--r--   0        0        0      131 2022-08-14 11:47:07.819126 cachestore-0.2.0/cachestore/hashers/__init__.py
--rw-r--r--   0        0        0      407 2022-08-14 11:47:07.819126 cachestore-0.2.0/cachestore/hashers/hasher.py
--rw-r--r--   0        0        0      594 2022-08-14 11:47:07.819126 cachestore-0.2.0/cachestore/hashers/pickle_hasher.py
--rw-r--r--   0        0        0     5853 2022-08-14 11:47:07.819126 cachestore-0.2.0/cachestore/metadata.py
--rw-r--r--   0        0        0        0 2022-08-14 11:47:07.819126 cachestore-0.2.0/cachestore/py.typed
--rw-r--r--   0        0        0      135 2022-08-14 11:47:07.819126 cachestore-0.2.0/cachestore/storages/__init__.py
--rw-r--r--   0        0        0     2300 2022-08-14 11:47:07.819126 cachestore-0.2.0/cachestore/storages/local_storage.py
--rw-r--r--   0        0        0      908 2022-08-14 11:47:07.819126 cachestore-0.2.0/cachestore/storages/storage.py
--rw-r--r--   0        0        0     2480 2022-08-14 11:47:07.819126 cachestore-0.2.0/cachestore/util.py
--rw-r--r--   0        0        0     1463 2022-08-14 11:47:07.819126 cachestore-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2489 2022-08-14 11:47:28.155532 cachestore-0.2.0/setup.py
--rw-r--r--   0        0        0     2191 2022-08-14 11:47:28.155862 cachestore-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-05-04 07:15:15.940263 cachestore-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1630 2023-05-04 07:15:15.940263 cachestore-0.3.0/README.md
+-rw-r--r--   0        0        0      526 2023-05-04 07:15:15.940263 cachestore-0.3.0/cachestore/__init__.py
+-rw-r--r--   0        0        0      447 2023-05-04 07:15:15.940263 cachestore-0.3.0/cachestore/__main__.py
+-rw-r--r--   0        0        0     8487 2023-05-04 07:15:15.940263 cachestore-0.3.0/cachestore/cache.py
+-rw-r--r--   0        0        0      677 2023-05-04 07:15:15.944263 cachestore-0.3.0/cachestore/commands/__init__.py
+-rw-r--r--   0        0        0     3849 2023-05-04 07:15:15.944263 cachestore-0.3.0/cachestore/commands/list.py
+-rw-r--r--   0        0        0      965 2023-05-04 07:15:15.944263 cachestore-0.3.0/cachestore/commands/prune.py
+-rw-r--r--   0        0        0     2519 2023-05-04 07:15:15.944263 cachestore-0.3.0/cachestore/commands/remove.py
+-rw-r--r--   0        0        0     3633 2023-05-04 07:15:15.944263 cachestore-0.3.0/cachestore/commands/subcommand.py
+-rw-r--r--   0        0        0      246 2023-05-04 07:15:15.944263 cachestore-0.3.0/cachestore/common/__init__.py
+-rw-r--r--   0        0        0     1995 2023-05-04 07:15:15.944263 cachestore-0.3.0/cachestore/common/astnorm.py
+-rw-r--r--   0        0        0     1021 2023-05-04 07:15:15.944263 cachestore-0.3.0/cachestore/common/filelock.py
+-rw-r--r--   0        0        0     2059 2023-05-04 07:15:15.944263 cachestore-0.3.0/cachestore/common/selector.py
+-rw-r--r--   0        0        0     4515 2023-05-04 07:15:15.944263 cachestore-0.3.0/cachestore/common/table.py
+-rw-r--r--   0        0        0     4963 2023-05-04 07:15:15.944263 cachestore-0.3.0/cachestore/config.py
+-rw-r--r--   0        0        0      149 2023-05-04 07:15:15.944263 cachestore-0.3.0/cachestore/formatters/__init__.py
+-rw-r--r--   0        0        0      565 2023-05-04 07:15:15.944263 cachestore-0.3.0/cachestore/formatters/formatter.py
+-rw-r--r--   0        0        0     1883 2023-05-04 07:15:15.944263 cachestore-0.3.0/cachestore/formatters/pickle_formatter.py
+-rw-r--r--   0        0        0      131 2023-05-04 07:15:15.944263 cachestore-0.3.0/cachestore/hashers/__init__.py
+-rw-r--r--   0        0        0      407 2023-05-04 07:15:15.944263 cachestore-0.3.0/cachestore/hashers/hasher.py
+-rw-r--r--   0        0        0      594 2023-05-04 07:15:15.944263 cachestore-0.3.0/cachestore/hashers/pickle_hasher.py
+-rw-r--r--   0        0        0     6048 2023-05-04 07:15:15.944263 cachestore-0.3.0/cachestore/metadata.py
+-rw-r--r--   0        0        0        0 2023-05-04 07:15:15.944263 cachestore-0.3.0/cachestore/py.typed
+-rw-r--r--   0        0        0      135 2023-05-04 07:15:15.944263 cachestore-0.3.0/cachestore/storages/__init__.py
+-rw-r--r--   0        0        0     2284 2023-05-04 07:15:15.944263 cachestore-0.3.0/cachestore/storages/local_storage.py
+-rw-r--r--   0        0        0      908 2023-05-04 07:15:15.944263 cachestore-0.3.0/cachestore/storages/storage.py
+-rw-r--r--   0        0        0     2766 2023-05-04 07:15:15.944263 cachestore-0.3.0/cachestore/util.py
+-rw-r--r--   0        0        0     1451 2023-05-04 07:15:15.944263 cachestore-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2242 1970-01-01 00:00:00.000000 cachestore-0.3.0/PKG-INFO
```

### Comparing `cachestore-0.2.0/LICENSE` & `cachestore-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cachestore-0.2.0/README.md` & `cachestore-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `cachestore-0.2.0/cachestore/__init__.py` & `cachestore-0.3.0/cachestore/__init__.py`

 * *Files identical despite different names*

### Comparing `cachestore-0.2.0/cachestore/cache.py` & `cachestore-0.3.0/cachestore/cache.py`

 * *Files 6% similar despite different names*

```diff
@@ -168,51 +168,59 @@
                         parameters=execinfo.params,
                         expired_at=expired_at,
                         executed_at=executed_at,
                     )
                     with storage.open(metakey, "wt") as file:
                         json.dump(cacheinfo.to_dict(), file)
 
+                    # reopen artifact beacause if artifact is iterator,
+                    # it is consumed when saving cache.
+                    with self.storage.open(key, formatter.READ_MODE) as file:
+                        artifact = cast(T, formatter.read(file))
+
                 return artifact
 
             setattr(wrapper, "__signature__", inspect.signature(func))
             setattr(wrapper, "__annotations__", func.__annotations__)
             setattr(wrapper, "__cachesore_funcinfo", funcinfo)
 
             return wrapper
 
         return decorator
 
     def exists(self, func: Callable[..., Any] | FunctionInfo) -> bool:
         current = datetime.datetime.now()
         exists = False
-        for cacheinfo in self.info(func):
+        for _, cacheinfo in self.info(func):
             exists |= cacheinfo.expired_at is None or cacheinfo.expired_at > current
         return exists
 
-    def remove(self, func: Callable[..., Any] | FunctionInfo) -> None:
+    def remove(
+        self,
+        func: Callable[..., Any] | FunctionInfo,
+        execution_prefix: str | None = None,
+    ) -> None:
         if not isinstance(func, FunctionInfo):
             func = FunctionInfo.build(func)
         prefix = func.hash(self.hasher)
+        if execution_prefix is not None:
+            prefix = f"{prefix}.{execution_prefix}"
         for key in self.storage.filter(prefix=prefix):
             self.storage.remove(key)
 
     def funcinfos(self) -> list[FunctionInfo]:
         return list(self._function_registry.values())
 
-    def info(self, func: Callable[..., Any] | FunctionInfo) -> Iterator[CacheInfo]:
+    def info(self, func: Callable[..., Any] | FunctionInfo) -> Iterator[tuple[str, CacheInfo]]:
         if not isinstance(func, FunctionInfo):
             func = FunctionInfo.build(func)
         prefix = func.hash(self.hasher)
         for key in self.storage.filter(prefix=prefix):
             metakey = self._get_metakey(key)
             with self.storage.open(metakey, "rt") as file:
-                yield CacheInfo.from_dict(json.load(file))
+                yield key, CacheInfo.from_dict(json.load(file))
 
     def prune(self) -> None:
         for key in self.storage.all():
-            if not any(
-                key.startswith(funchash) or key.startswith(self._get_metakey(funchash))
-                for funchash in self._function_registry
-            ):
+            if not any(key.startswith((funchash, self._get_metakey(funchash))) for funchash in self._function_registry):
                 logger.info("remove %s", key)
                 self.storage.remove(key)
```

### Comparing `cachestore-0.2.0/cachestore/commands/__init__.py` & `cachestore-0.3.0/cachestore/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `cachestore-0.2.0/cachestore/commands/list.py` & `cachestore-0.3.0/cachestore/commands/list.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
         if cache is None:
             print(f"Given cache name is not found: {args.cache}", file=sys.stderr)
             sys.exit(1)
 
         table = Table(columns=["name", "function", "filename", "cache", "last_executed_at"])
         for funcinfo in cache.funcinfos():
-            cacheinfos = list(cache.info(funcinfo))
+            cacheinfos = list(info for _, info in cache.info(funcinfo))
             table.add(
                 {
                     "name": args.cache,
                     "function": funcinfo.name,
                     "filename": str(funcinfo.filename.relative_to(Path.cwd())),
                     "cache": "\033[32m✓\033[39m" if cache.exists(funcinfo) else "",
                     "last_executed_at": max(info.executed_at for info in cacheinfos).strftime("%Y-%m-%d %H:%M:%S")
@@ -68,15 +68,15 @@
             help="function name to show details",
         )
 
     def run(self, args: argparse.Namespace) -> None:
         if args.include_package:
             import_modules(args.include_package)
 
-        table = Table(columns=["cache", "function", "filename", "params", "executed_at", "expired_at"])
+        table = Table(columns=["cache", "function", "filename", "params", "exec", "executed_at", "expired_at"])
 
         cache = safe_import_object(args.cache)
         assert isinstance(cache, Cache)
 
         funcinfos = {info.name: info for info in cache.funcinfos()}
 
         if args.function:
@@ -86,21 +86,22 @@
 
         if not funcname or funcname not in funcinfos:
             print("No information to show.")
             return
 
         funcinfo = funcinfos[funcname]
 
-        for cacheinfo in cache.info(funcinfo):
+        for key, cacheinfo in cache.info(funcinfo):
             table.add(
                 {
                     "cache": args.cache,
                     "function": funcinfo.name,
                     "filename": str(funcinfo.filename.relative_to(Path.cwd())),
                     "params": ", ".join(f"{k}={v}" for k, v in cacheinfo.parameters.items()),
+                    "exec": key.split(".", 1)[1][:8],
                     "executed_at": cacheinfo.executed_at.strftime("%Y-%m-%d %H:%M:%S"),
                     "expired_at": (
                         cacheinfo.expired_at.strftime("%Y-%m-%d %H:%M:%S")
                         if cacheinfo.expired_at > datetime.datetime.now()
                         else f"\033[31m{cacheinfo.expired_at.strftime('%Y-%m-%d %H:%M:%S')}\033[39m"
                     )
                     if cacheinfo.expired_at
```

### Comparing `cachestore-0.2.0/cachestore/commands/prune.py` & `cachestore-0.3.0/cachestore/commands/prune.py`

 * *Files identical despite different names*

### Comparing `cachestore-0.2.0/cachestore/commands/remove.py` & `cachestore-0.3.0/cachestore/commands/remove.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     def setup(self) -> None:
         self.parser.add_argument("cache", help="cache name")
         self.parser.add_argument(
             "-f",
             "--function",
             action="append",
             default=[],
-            help="function names to remove cache",
+            help="function names to remove cache formatted like: function[@exec]",
         )
         self.parser.add_argument(
             "-a",
             "--all",
             action="store_true",
             help="remove all caches of the specified cache",
         )
@@ -48,21 +48,26 @@
         funcinfos = {funcinfo.name: funcinfo for funcinfo in cache.funcinfos() if cache.exists(funcinfo)}
         if args.all:
             funcnames = set(funcinfos.keys())
         elif args.function:
             funcnames = set(args.function)
         else:
             funcnames = set()
-            candidates = [name for name, info in funcinfos.items()]
+            candidates = [name for name in funcinfos.keys()]
             if candidates:
                 selected_funcname = Selector()(candidates)
                 funcnames = set() if selected_funcname is None else {selected_funcname}
 
         if funcnames:
             for funcname in funcnames:
-                if args.all or funcname in funcinfos:
+                if "@" in funcname:
+                    parsed_funcname, execution_prefix = funcname.split("@", 1)
+                else:
+                    parsed_funcname = funcname
+                    execution_prefix = None
+                if args.all or parsed_funcname in funcinfos:
                     print(f"remove: {funcname}")
-                    cache.remove(funcinfos[funcname])
+                    cache.remove(funcinfos[parsed_funcname], execution_prefix=execution_prefix)
                 else:
                     print(f"skip  : {funcname}")
         else:
             print("No caches to remove.")
```

### Comparing `cachestore-0.2.0/cachestore/commands/subcommand.py` & `cachestore-0.3.0/cachestore/commands/subcommand.py`

 * *Files identical despite different names*

### Comparing `cachestore-0.2.0/cachestore/common/filelock.py` & `cachestore-0.3.0/cachestore/common/filelock.py`

 * *Files identical despite different names*

### Comparing `cachestore-0.2.0/cachestore/common/selector.py` & `cachestore-0.3.0/cachestore/common/selector.py`

 * *Files identical despite different names*

### Comparing `cachestore-0.2.0/cachestore/common/table.py` & `cachestore-0.3.0/cachestore/common/table.py`

 * *Files identical despite different names*

### Comparing `cachestore-0.2.0/cachestore/config.py` & `cachestore-0.3.0/cachestore/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,17 +20,17 @@
 
 
 T = TypeVar("T")
 
 
 @dataclasses.dataclass
 class CacheSettings:
-    storage: Storage = dataclasses.field(default_factory=lambda: LocalStorage())
-    formatter: Formatter = dataclasses.field(default_factory=lambda: PickleFormatter())
-    hasher: Hasher = dataclasses.field(default_factory=lambda: PickleHasher())
+    storage: Storage = dataclasses.field(default_factory=LocalStorage)
+    formatter: Formatter = dataclasses.field(default_factory=PickleFormatter)
+    hasher: Hasher = dataclasses.field(default_factory=PickleHasher)
     disable: bool = DISABLE_CACHE
 
 
 @dataclasses.dataclass
 class FunctionSettings:
     ignore: set[str] = dataclasses.field(default_factory=set)
     expire: int | datetime.timedelta | datetime.date | datetime.datetime | None = None
```

### Comparing `cachestore-0.2.0/cachestore/formatters/formatter.py` & `cachestore-0.3.0/cachestore/formatters/formatter.py`

 * *Files identical despite different names*

### Comparing `cachestore-0.2.0/cachestore/hashers/pickle_hasher.py` & `cachestore-0.3.0/cachestore/hashers/pickle_hasher.py`

 * *Files identical despite different names*

### Comparing `cachestore-0.2.0/cachestore/metadata.py` & `cachestore-0.3.0/cachestore/metadata.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 from __future__ import annotations
 
+import ast
 import datetime
 import inspect
+from contextlib import suppress
 from pathlib import Path
 from typing import Any, Callable, NamedTuple
 
+from cachestore.common import ASTNormalizer
 from cachestore.hashers import Hasher
 
 
 class FunctionInfo(NamedTuple):
     name: str
     filename: Path
     source: str
@@ -20,14 +23,16 @@
             assert isinstance(funcinfo, FunctionInfo)
             return funcinfo
         filename = Path(inspect.getabsfile(func))
         modulename = inspect.getmodulename(str(filename)) or ""
         name = f"{modulename}.{func.__qualname__}"
         lines, _ = inspect.getsourcelines(func)
         source = "".join(lines)
+        with suppress(SyntaxError):
+            source = ast.dump(ASTNormalizer().visit(ast.parse(source)))
         return cls(name, filename, source)
 
     def hash(self, hasher: Hasher) -> str:
         return hasher(self)
 
     def to_dict(self) -> dict[str, Any]:
         return {
```

### Comparing `cachestore-0.2.0/cachestore/storages/local_storage.py` & `cachestore-0.3.0/cachestore/storages/local_storage.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from __future__ import annotations
 
-import os
 from configparser import SectionProxy
 from contextlib import contextmanager
 from os import PathLike
 from pathlib import Path
 from typing import IO, Any, Callable, ContextManager, Iterator, Type, TypeVar
 
 from cachestore.common import FileLock
@@ -37,22 +36,22 @@
         lockfile = filename.parent / (filename.name + ".lock")
         filename.parent.mkdir(parents=True, exist_ok=True)
         with FileLock(lockfile):
             try:
                 with self._openfn(filename, mode) as fp:
                     yield fp
             except (Exception, KeyboardInterrupt):
-                os.remove(filename)
+                filename.unlink()
                 raise
             finally:
-                os.remove(lockfile)
+                lockfile.unlink()
 
     def remove(self, key: str) -> None:
         filename = self._root / key
-        os.remove(filename)
+        filename.unlink()
 
     def exists(self, key: str) -> bool:
         return (self._root / key).exists()
 
     def all(self) -> Iterator[str]:
         for filename in self._root.glob("*"):
             yield filename.name
```

### Comparing `cachestore-0.2.0/cachestore/storages/storage.py` & `cachestore-0.3.0/cachestore/storages/storage.py`

 * *Files identical despite different names*

### Comparing `cachestore-0.2.0/cachestore/util.py` & `cachestore-0.3.0/cachestore/util.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 from __future__ import annotations
 
+import bz2
+import gzip
 import importlib
 import inspect
+import lzma
 import pkgutil
 import string
 import sys
+from contextlib import suppress
 from types import ModuleType
-from typing import Any
+from typing import Any, Callable
 
 
 def b62encode(data: bytes) -> str:
     num = int.from_bytes(data, "big")
     characters = string.digits + string.ascii_letters
 
     encoded = ""
@@ -50,21 +54,19 @@
 def import_modules(module_names: list[str]) -> None:
     for module_name in module_names:
         import_submodules(module_name)
 
 
 def safe_import_module(modulename: str) -> ModuleType:
     for name, module in list(sys.modules.items()):
-        try:
+        with suppress(AttributeError):
             if name == modulename or (
                 hasattr(module, "__file__") and modulename == inspect.getmodulename(inspect.getabsfile(module))
             ):
                 return module
-        except AttributeError:
-            pass
     return importlib.import_module(modulename)
 
 
 def safe_import_object(path: str) -> Any:
     if "." not in path and ":" not in path:
         raise ValueError("Cache name must be formatted as path.to.module:name.")
     if ":" in path:
@@ -75,14 +77,22 @@
     return getattr(module, objname)
 
 
 def find_variable_path(obj: Any) -> str | None:
     for modulename, module in list(sys.modules.items()):
         if hasattr(module, "__file__"):
             modulename = inspect.getmodulename(inspect.getabsfile(module)) or modulename
-        try:
+        with suppress(AttributeError):
             for varname, value in module.__dict__.items():
                 if value is obj:
                     return f"{modulename}:{varname}"
-        except AttributeError:
-            pass
     return None
+
+
+def detect_open_fn(file: Any) -> Callable:
+    if isinstance(file, gzip.GzipFile):
+        return gzip.open
+    if isinstance(file, bz2.BZ2File):
+        return bz2.open
+    if isinstance(file, lzma.LZMAFile):
+        return lzma.open
+    return open
```

### Comparing `cachestore-0.2.0/pyproject.toml` & `cachestore-0.3.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [tool.poetry]
 name = "cachestore"
-version = "0.2.0"
+version = "0.3.0"
 description = "Function Cache Management Tool for Python"
 authors = ["altescy <altescy@fastmail.com>"]
 license = "MIT License"
 readme = "README.md"
 homepage = "https://github.com/altescy/cachestore"
 keywords=["python", "cache"]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
 
 [tool.poetry.dev-dependencies]
 python-language-server = "^0.36.2"
-pytest = "^7.1.2"
-pysen = {version = "^0.10.1"}
-black = "^22.3.0"
-isort = "^5.10.1"
-flake8 = "^4.0.1"
-mypy = "^0.950"
+pytest = "^7.3.1"
+pysen = "^0.10.4"
+black = "^23.3.0"
+isort = "^5.12.0"
+flake8 = "^5.0.0"
+mypy = "^1.2.0"
 
 [tool.poetry.scripts]
 cachestore = "cachestore.__main__:run"
 
 [tool.pysen]
 version = "0.10"
```

### Comparing `cachestore-0.2.0/PKG-INFO` & `cachestore-0.3.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: cachestore
-Version: 0.2.0
+Version: 0.3.0
 Summary: Function Cache Management Tool for Python
 Home-page: https://github.com/altescy/cachestore
 License: MIT
 Keywords: python,cache
 Author: altescy
 Author-email: altescy@fastmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 
 # CacheStore
 
 [![Actions Status](https://github.com/altescy/cachestore/workflows/CI/badge.svg)](https://github.com/altescy/cachestore/actions/workflows/ci.yml)
 [![Python version](https://img.shields.io/pypi/pyversions/cachestore)](https://github.com/altescy/cachestore)
 [![License](https://img.shields.io/github/license/altescy/cachestore)](https://github.com/altescy/cachestore/blob/master/LICENSE)
```

