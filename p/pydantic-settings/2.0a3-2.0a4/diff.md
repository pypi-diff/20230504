# Comparing `tmp/pydantic_settings-2.0a3.tar.gz` & `tmp/pydantic_settings-2.0a4.tar.gz`

## Comparing `pydantic_settings-2.0a3.tar` & `pydantic_settings-2.0a4.tar`

### file list

```diff
@@ -1,23 +1,24 @@
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 pydantic_settings-2.0a3/.pre-commit-config.yaml
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 pydantic_settings-2.0a3/Makefile
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 pydantic_settings-2.0a3/.github/FUNDING.yml
--rw-r--r--   0        0        0     2739 2020-02-02 00:00:00.000000 pydantic_settings-2.0a3/.github/workflows/ci.yml
--rw-r--r--   0        0        0    18107 2020-02-02 00:00:00.000000 pydantic_settings-2.0a3/docs/index.md
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 pydantic_settings-2.0a3/pydantic_settings/__init__.py
--rw-r--r--   0        0        0     4758 2020-02-02 00:00:00.000000 pydantic_settings-2.0a3/pydantic_settings/main.py
--rw-r--r--   0        0        0    19763 2020-02-02 00:00:00.000000 pydantic_settings-2.0a3/pydantic_settings/sources.py
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 pydantic_settings-2.0a3/pydantic_settings/utils.py
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 pydantic_settings-2.0a3/pydantic_settings/version.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 pydantic_settings-2.0a3/requirements/all.txt
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 pydantic_settings-2.0a3/requirements/linting.in
--rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 pydantic_settings-2.0a3/requirements/linting.txt
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 pydantic_settings-2.0a3/requirements/pyproject.txt
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 pydantic_settings-2.0a3/requirements/testing.in
--rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 pydantic_settings-2.0a3/requirements/testing.txt
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 pydantic_settings-2.0a3/tests/conftest.py
--rw-r--r--   0        0        0    43806 2020-02-02 00:00:00.000000 pydantic_settings-2.0a3/tests/test_settings.py
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 pydantic_settings-2.0a3/.gitignore
--rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 pydantic_settings-2.0a3/LICENSE
--rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 pydantic_settings-2.0a3/README.md
--rw-r--r--   0        0        0     3455 2020-02-02 00:00:00.000000 pydantic_settings-2.0a3/pyproject.toml
--rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 pydantic_settings-2.0a3/PKG-INFO
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 pydantic_settings-2.0a4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 pydantic_settings-2.0a4/Makefile
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 pydantic_settings-2.0a4/.github/FUNDING.yml
+-rw-r--r--   0        0        0     2739 2020-02-02 00:00:00.000000 pydantic_settings-2.0a4/.github/workflows/ci.yml
+-rw-r--r--   0        0        0    18379 2020-02-02 00:00:00.000000 pydantic_settings-2.0a4/docs/index.md
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 pydantic_settings-2.0a4/pydantic_settings/__init__.py
+-rw-r--r--   0        0        0     4668 2020-02-02 00:00:00.000000 pydantic_settings-2.0a4/pydantic_settings/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pydantic_settings-2.0a4/pydantic_settings/py.typed
+-rw-r--r--   0        0        0    20460 2020-02-02 00:00:00.000000 pydantic_settings-2.0a4/pydantic_settings/sources.py
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 pydantic_settings-2.0a4/pydantic_settings/utils.py
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 pydantic_settings-2.0a4/pydantic_settings/version.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 pydantic_settings-2.0a4/requirements/all.txt
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 pydantic_settings-2.0a4/requirements/linting.in
+-rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 pydantic_settings-2.0a4/requirements/linting.txt
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 pydantic_settings-2.0a4/requirements/pyproject.txt
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 pydantic_settings-2.0a4/requirements/testing.in
+-rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 pydantic_settings-2.0a4/requirements/testing.txt
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 pydantic_settings-2.0a4/tests/conftest.py
+-rw-r--r--   0        0        0    45543 2020-02-02 00:00:00.000000 pydantic_settings-2.0a4/tests/test_settings.py
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 pydantic_settings-2.0a4/.gitignore
+-rw-r--r--   0        0        0     1103 2020-02-02 00:00:00.000000 pydantic_settings-2.0a4/LICENSE
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 pydantic_settings-2.0a4/README.md
+-rw-r--r--   0        0        0     3518 2020-02-02 00:00:00.000000 pydantic_settings-2.0a4/pyproject.toml
+-rw-r--r--   0        0        0     2853 2020-02-02 00:00:00.000000 pydantic_settings-2.0a4/PKG-INFO
```

### Comparing `pydantic_settings-2.0a3/.pre-commit-config.yaml` & `pydantic_settings-2.0a4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pydantic_settings-2.0a3/Makefile` & `pydantic_settings-2.0a4/Makefile`

 * *Files identical despite different names*

### Comparing `pydantic_settings-2.0a3/.github/workflows/ci.yml` & `pydantic_settings-2.0a4/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `pydantic_settings-2.0a3/docs/index.md` & `pydantic_settings-2.0a4/docs/index.md`

 * *Files 2% similar despite different names*

```diff
@@ -295,14 +295,18 @@
 You can also use the keyword argument override to tell Pydantic not to load any file at all (even if one is set in
 the `model_config` class) by passing `None` as the instantiation keyword argument, e.g. `settings = Settings(_env_file=None)`.
 
 Because python-dotenv is used to parse the file, bash-like semantics such as `export` can be used which
 (depending on your OS and environment) may allow your dotenv file to also be used with `source`,
 see [python-dotenv's documentation](https://saurabh-kumar.com/python-dotenv/#usages) for more details.
 
+Pydantic settings consider `extra` config in case of dotenv file. It means if you set the `extra=forbid`
+on `model_config` and your dotenv file contains an entry for a field that is not defined in settings model,
+it will raise `ValidationError` in settings construction.
+
 ## Secret Support
 
 Placing secret values in files is a common pattern to provide sensitive configuration to an application.
 
 A secret file follows the same principal as a dotenv file except it only contains a single value and the file name
 is used as the key. A secret file will look like the following:
```

### Comparing `pydantic_settings-2.0a3/pydantic_settings/main.py` & `pydantic_settings-2.0a4/pydantic_settings/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations as _annotations
 
 from pathlib import Path
-from typing import Any, Dict, Optional, Tuple, Type, Union
+from typing import Any
 
 from pydantic import ConfigDict
 from pydantic._internal._utils import deep_update
 from pydantic.main import BaseModel
 
 from .sources import (
     DotEnvSettingsSource,
@@ -18,34 +18,34 @@
 
 env_file_sentinel: DotenvType = Path('')
 
 
 class SettingsConfigDict(ConfigDict):
     case_sensitive: bool
     env_prefix: str
-    env_file: Optional[DotenvType]
-    env_file_encoding: Optional[str]
-    env_nested_delimiter: Optional[str]
-    secrets_dir: Optional[Union[str, Path]]
+    env_file: DotenvType | None
+    env_file_encoding: str | None
+    env_nested_delimiter: str | None
+    secrets_dir: str | Path | None
 
 
 class BaseSettings(BaseModel):
     """
     Base class for settings, allowing values to be overridden by environment variables.
 
     This is useful in production for secrets you do not wish to save in code, it plays nicely with docker(-compose),
     Heroku and any 12 factor app design.
     """
 
     def __init__(
         __pydantic_self__,
-        _env_file: Optional[DotenvType] = env_file_sentinel,
-        _env_file_encoding: Optional[str] = None,
-        _env_nested_delimiter: Optional[str] = None,
-        _secrets_dir: Optional[Union[str, Path]] = None,
+        _env_file: DotenvType | None = env_file_sentinel,
+        _env_file_encoding: str | None = None,
+        _env_nested_delimiter: str | None = None,
+        _secrets_dir: str | Path | None = None,
         **values: Any,
     ) -> None:
         # Uses something other than `self` the first arg to allow "self" as a settable attribute
         super().__init__(
             **__pydantic_self__._settings_build_values(
                 values,
                 _env_file=_env_file,
@@ -54,30 +54,30 @@
                 _secrets_dir=_secrets_dir,
             )
         )
 
     @classmethod
     def settings_customise_sources(
         cls,
-        settings_cls: Type[BaseSettings],
+        settings_cls: type[BaseSettings],
         init_settings: PydanticBaseSettingsSource,
         env_settings: PydanticBaseSettingsSource,
         dotenv_settings: PydanticBaseSettingsSource,
         file_secret_settings: PydanticBaseSettingsSource,
-    ) -> Tuple[PydanticBaseSettingsSource, ...]:
+    ) -> tuple[PydanticBaseSettingsSource, ...]:
         return init_settings, env_settings, dotenv_settings, file_secret_settings
 
     def _settings_build_values(
         self,
-        init_kwargs: Dict[str, Any],
-        _env_file: Optional[DotenvType] = None,
-        _env_file_encoding: Optional[str] = None,
-        _env_nested_delimiter: Optional[str] = None,
-        _secrets_dir: Optional[Union[str, Path]] = None,
-    ) -> Dict[str, Any]:
+        init_kwargs: dict[str, Any],
+        _env_file: DotenvType | None = None,
+        _env_file_encoding: str | None = None,
+        _env_nested_delimiter: str | None = None,
+        _secrets_dir: str | Path | None = None,
+    ) -> dict[str, Any]:
         # Configure built-in sources
         init_settings = InitSettingsSource(self.__class__, init_kwargs=init_kwargs)
         env_settings = EnvSettingsSource(
             self.__class__,
             env_nested_delimiter=(
                 _env_nested_delimiter
                 if _env_nested_delimiter is not None
```

### Comparing `pydantic_settings-2.0a3/pydantic_settings/sources.py` & `pydantic_settings-2.0a4/pydantic_settings/sources.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import json
 import os
 import warnings
 from abc import ABC, abstractmethod
 from collections import deque
 from dataclasses import is_dataclass
 from pathlib import Path
-from typing import TYPE_CHECKING, Any, Dict, List, Mapping, Optional, Sequence, Tuple, Type, Union
+from typing import TYPE_CHECKING, Any, List, Mapping, Sequence, Tuple, Union
 
 from pydantic import BaseModel
 from pydantic._internal._typing_extra import origin_is_union
 from pydantic._internal._utils import deep_update, lenient_issubclass
 from pydantic.fields import FieldInfo
 from typing_extensions import get_origin
 
@@ -29,31 +29,31 @@
 
 
 class PydanticBaseSettingsSource(ABC):
     """
     Abstract base class for settings sources, every settings source classes should inherit from it.
     """
 
-    def __init__(self, settings_cls: Type[BaseSettings]):
+    def __init__(self, settings_cls: type[BaseSettings]):
         self.settings_cls = settings_cls
         self.config = settings_cls.model_config
 
     @abstractmethod
-    def get_field_value(self, field: FieldInfo, field_name: str) -> Tuple[Any, str, bool]:
+    def get_field_value(self, field: FieldInfo, field_name: str) -> tuple[Any, str, bool]:
         """
         Gets the value, the key for model creation, and a flag to determine whether value is complex.
 
         This is an abstract method that should be overrided in every settings source classes.
 
         Args:
             field (FieldInfo): The field.
             field_name (str): The field name.
 
         Returns:
-            Tuple[str, Any, bool]: The key, value and a flag to determine whether value is complex.
+            tuple[str, Any, bool]: The key, value and a flag to determine whether value is complex.
         """
         pass
 
     def field_is_complex(self, field: FieldInfo) -> bool:
         """
         Checks whether a field is complex, in which case it will attempt to be parsed as JSON.
 
@@ -79,55 +79,55 @@
             Any: The prepared value.
         """
         if self.field_is_complex(field) or value_is_complex:
             return json.loads(value)
         return value
 
     @abstractmethod
-    def __call__(self) -> Dict[str, Any]:
+    def __call__(self) -> dict[str, Any]:
         pass
 
 
 class InitSettingsSource(PydanticBaseSettingsSource):
-    def __init__(self, settings_cls: Type[BaseSettings], init_kwargs: Dict[str, Any]):
+    def __init__(self, settings_cls: type[BaseSettings], init_kwargs: dict[str, Any]):
         self.init_kwargs = init_kwargs
         super().__init__(settings_cls)
 
-    def get_field_value(self, field: FieldInfo, field_name: str) -> Tuple[Any, str, bool]:
+    def get_field_value(self, field: FieldInfo, field_name: str) -> tuple[Any, str, bool]:
         pass
 
-    def __call__(self) -> Dict[str, Any]:
+    def __call__(self) -> dict[str, Any]:
         return self.init_kwargs
 
     def __repr__(self) -> str:
         return f'InitSettingsSource(init_kwargs={self.init_kwargs!r})'
 
 
 class PydanticBaseEnvSettingsSource(PydanticBaseSettingsSource):
     def _apply_case_sensitive(self, value: str) -> str:
         return value.lower() if not self.config.get('case_sensitive') else value
 
-    def _extract_field_info(self, field: FieldInfo, field_name: str) -> List[Tuple[str, str, bool]]:
+    def _extract_field_info(self, field: FieldInfo, field_name: str) -> list[tuple[str, str, bool]]:
         """
         Extracts field info. This info is used to get the value of field from environment variables.
 
         It returns a list of tuples, each tuple contains:
             * field_key: The key of field that has to be used in model creation.
             * env_name: The environment variable name of the field.
             * value_is_complex: A flag to determine whether the value from environment variable
               is complex and has to be parsed.
 
         Args:
             field (FieldInfo): The field.
             field_name (str): The field name.
 
         Returns:
-            List[Tuple[str, str, bool]]: List of tuples, each tuple contanis field_key, env_name, and value_is_complex.
+            list[tuple[str, str, bool]]: List of tuples, each tuple contanis field_key, env_name, and value_is_complex.
         """
-        field_info: List[Tuple[str, str, bool]] = []
+        field_info: list[tuple[str, str, bool]] = []
         v_alias = field.validation_alias
 
         if v_alias:
             if isinstance(v_alias, list):  # AliasChoices, AliasPath
                 for alias in v_alias:
                     if isinstance(alias, str):  # AliasPath
                         field_info.append((alias, self._apply_case_sensitive(alias), True if len(alias) > 1 else False))
@@ -140,15 +140,15 @@
         else:
             field_info.append(
                 (field_name, self._apply_case_sensitive(self.config.get('env_prefix', '') + field_name), False)
             )
 
         return field_info
 
-    def _replace_field_names_case_insensitively(self, field: FieldInfo, field_values: Dict[str, Any]) -> Dict[str, Any]:
+    def _replace_field_names_case_insensitively(self, field: FieldInfo, field_values: dict[str, Any]) -> dict[str, Any]:
         """
         Replace field names in values dict by looking in models fields insensitively.
 
         By having the following models:
 
             ```py
             class SubSubSub(BaseModel):
@@ -171,18 +171,18 @@
         Then:
             _replace_field_names_case_insensitively(
                 field,
                 {"val1": "v1", "sub_SUB": {"VAL2": "v2", "sub_SUB_sUb": {"vAl3": "v3"}}}
             )
             Returns {'VAL1': 'v1', 'SUB_sub': {'Val2': 'v2', 'SUB_sub_SuB': {'VaL3': 'v3'}}}
         """
-        values: Dict[str, Any] = {}
+        values: dict[str, Any] = {}
 
         for name, value in field_values.items():
-            sub_model_field: Optional[FieldInfo] = None
+            sub_model_field: FieldInfo | None = None
 
             # This is here to make mypy happy
             # Item "None" of "Optional[Type[Any]]" has no attribute "model_fields"
             if not field.annotation or not hasattr(field.annotation, 'model_fields'):
                 values[name] = value
                 continue
 
@@ -199,16 +199,16 @@
             if lenient_issubclass(sub_model_field.annotation, BaseModel):
                 values[sub_model_field_name] = self._replace_field_names_case_insensitively(sub_model_field, value)
             else:
                 values[sub_model_field_name] = value
 
         return values
 
-    def __call__(self) -> Dict[str, Any]:
-        d: Dict[str, Any] = {}
+    def __call__(self) -> dict[str, Any]:
+        data: dict[str, Any] = {}
 
         for field_name, field in self.settings_cls.model_fields.items():
             try:
                 field_value, field_key, value_is_complex = self.get_field_value(field, field_name)
             except Exception as e:
                 raise SettingsError(
                     f'error getting value for field "{field_name}" from source "{self.__class__.__name__}"'
@@ -219,31 +219,31 @@
             except ValueError as e:
                 raise SettingsError(
                     f'error parsing value for field "{field_name}" from source "{self.__class__.__name__}"'
                 ) from e
 
             if field_value is not None:
                 if not self.config.get('case_sensitive', False) and lenient_issubclass(field.annotation, BaseModel):
-                    d[field_key] = self._replace_field_names_case_insensitively(field, field_value)
+                    data[field_key] = self._replace_field_names_case_insensitively(field, field_value)
                 else:
-                    d[field_key] = field_value
+                    data[field_key] = field_value
 
-        return d
+        return data
 
 
 class SecretsSettingsSource(PydanticBaseEnvSettingsSource):
-    def __init__(self, settings_cls: Type[BaseSettings], secrets_dir: Optional[Union[str, Path]]):
+    def __init__(self, settings_cls: type[BaseSettings], secrets_dir: str | Path | None):
         self.secrets_dir = secrets_dir
         super().__init__(settings_cls)
 
-    def __call__(self) -> Dict[str, Any]:
+    def __call__(self) -> dict[str, Any]:
         """
         Build fields from "secrets" files.
         """
-        secrets: Dict[str, Optional[str]] = {}
+        secrets: dict[str, str | None] = {}
 
         if self.secrets_dir is None:
             return secrets
 
         self.secrets_path = Path(self.secrets_dir).expanduser()
 
         if not self.secrets_path.exists():
@@ -252,26 +252,26 @@
 
         if not self.secrets_path.is_dir():
             raise SettingsError(f'secrets_dir must reference a directory, not a {path_type_label(self.secrets_path)}')
 
         return super().__call__()
 
     @classmethod
-    def find_case_path(cls, dir_path: Path, file_name: str, case_sensitive: bool) -> Optional[Path]:
+    def find_case_path(cls, dir_path: Path, file_name: str, case_sensitive: bool) -> Path | None:
         """
         Find a file within path's directory matching filename, optionally ignoring case.
         """
         for f in dir_path.iterdir():
             if f.name == file_name:
                 return f
             elif not case_sensitive and f.name.lower() == file_name.lower():
                 return f
         return None
 
-    def get_field_value(self, field: FieldInfo, field_name: str) -> Tuple[Any, str, bool]:
+    def get_field_value(self, field: FieldInfo, field_name: str) -> tuple[Any, str, bool]:
         for field_key, env_name, value_is_complex in self._extract_field_info(field, field_name):
             path = self.find_case_path(
                 self.secrets_path, env_name, self.settings_cls.model_config.get('case_sensitive', False)
             )
             if not path:
                 # path does not exist, we curently don't return a warning for this
                 continue
@@ -289,32 +289,32 @@
     def __repr__(self) -> str:
         return f'SecretsSettingsSource(secrets_dir={self.secrets_dir!r})'
 
 
 class EnvSettingsSource(PydanticBaseEnvSettingsSource):
     def __init__(
         self,
-        settings_cls: Type[BaseSettings],
-        env_nested_delimiter: Optional[str] = None,
+        settings_cls: type[BaseSettings],
+        env_nested_delimiter: str | None = None,
         env_prefix_len: int = 0,
     ):
         super().__init__(settings_cls)
 
-        self.env_nested_delimiter: Optional[str] = env_nested_delimiter
+        self.env_nested_delimiter: str | None = env_nested_delimiter
         self.env_prefix_len: int = env_prefix_len
 
-        self.env_vars: Mapping[str, Optional[str]] = self._load_env_vars()
+        self.env_vars: Mapping[str, str | None] = self._load_env_vars()
 
-    def _load_env_vars(self) -> Mapping[str, Optional[str]]:
+    def _load_env_vars(self) -> Mapping[str, str | None]:
         if self.settings_cls.model_config.get('case_sensitive'):
             return os.environ
         return {k.lower(): v for k, v in os.environ.items()}
 
-    def get_field_value(self, field: FieldInfo, field_name: str) -> Tuple[Any, str, bool]:
-        env_val: Optional[str] = None
+    def get_field_value(self, field: FieldInfo, field_name: str) -> tuple[Any, str, bool]:
+        env_val: str | None = None
         for field_key, env_name, value_is_complex in self._extract_field_info(field, field_name):
             env_val = self.env_vars.get(env_name)
             if env_val is not None:
                 break
 
         return env_val, field_key, value_is_complex
 
@@ -338,40 +338,40 @@
                     return deep_update(value, self.explode_env_vars(field_name, field, self.env_vars))
                 else:
                     return value
         elif value is not None:
             # simplest case, field is not complex, we only need to add the value if it was found
             return value
 
-    def _field_is_complex(self, field: FieldInfo) -> Tuple[bool, bool]:
+    def _field_is_complex(self, field: FieldInfo) -> tuple[bool, bool]:
         """
         Find out if a field is complex, and if so whether JSON errors should be ignored
         """
         if self.field_is_complex(field):
             allow_parse_failure = False
         elif origin_is_union(get_origin(field.annotation)):
             allow_parse_failure = True
         else:
             return False, False
 
         return True, allow_parse_failure
 
     @staticmethod
-    def next_field(field: Optional[FieldInfo], key: str) -> Optional[FieldInfo]:
+    def next_field(field: FieldInfo | None, key: str) -> FieldInfo | None:
         """
         Find the field in a sub model by key(env name)
 
         By having the following models:
 
             ```py
             class SubSubModel(BaseSettings):
                 dvals: Dict
 
             class SubModel(BaseSettings):
-                vals: List[str]
+                vals: list[str]
                 sub_sub_model: SubSubModel
 
             class Cfg(BaseSettings):
                 sub_model: SubModel
             ```
 
         Then:
@@ -382,35 +382,32 @@
             # no support for Unions of complex BaseSettings fields
             return None
         elif field.annotation and hasattr(field.annotation, 'model_fields') and field.annotation.model_fields.get(key):
             return field.annotation.model_fields[key]
 
         return None
 
-    def explode_env_vars(
-        self, field_name: str, field: FieldInfo, env_vars: Mapping[str, Optional[str]]
-    ) -> Dict[str, Any]:
+    def explode_env_vars(self, field_name: str, field: FieldInfo, env_vars: Mapping[str, str | None]) -> dict[str, Any]:
         """
         Process env_vars and extract the values of keys containing env_nested_delimiter into nested dictionaries.
 
         This is applied to a single field, hence filtering by env_var prefix.
         """
         prefixes = [
             f'{env_name}{self.env_nested_delimiter}' for _, env_name, _ in self._extract_field_info(field, field_name)
         ]
-        result: Dict[str, Any] = {}
+        result: dict[str, Any] = {}
         for env_name, env_val in env_vars.items():
             if not any(env_name.startswith(prefix) for prefix in prefixes):
                 continue
             # we remove the prefix before splitting in case the prefix has characters in common with the delimiter
             env_name_without_prefix = env_name[self.env_prefix_len :]
             _, *keys, last_key = env_name_without_prefix.split(self.env_nested_delimiter)
             env_var = result
-            target_field: Optional[FieldInfo] = field
-
+            target_field: FieldInfo | None = field
             for key in keys:
                 target_field = self.next_field(target_field, key)
                 env_var = env_var.setdefault(key, {})
 
             # get proper field with last_key
             target_field = self.next_field(target_field, last_key)
 
@@ -433,72 +430,90 @@
             f'env_prefix_len={self.env_prefix_len!r})'
         )
 
 
 class DotEnvSettingsSource(EnvSettingsSource):
     def __init__(
         self,
-        settings_cls: Type[BaseSettings],
-        env_file: Optional[DotenvType],
-        env_file_encoding: Optional[str],
-        env_nested_delimiter: Optional[str] = None,
+        settings_cls: type[BaseSettings],
+        env_file: DotenvType | None,
+        env_file_encoding: str | None,
+        env_nested_delimiter: str | None = None,
         env_prefix_len: int = 0,
     ):
-        self.env_file: Optional[DotenvType] = env_file
-        self.env_file_encoding: Optional[str] = env_file_encoding
+        self.env_file: DotenvType | None = env_file
+        self.env_file_encoding: str | None = env_file_encoding
 
         super().__init__(settings_cls, env_nested_delimiter, env_prefix_len)
 
-    def _load_env_vars(self) -> Mapping[str, Optional[str]]:
-        env_vars = super()._load_env_vars()
-        dotenv_vars = self._read_env_files(self.settings_cls.model_config.get('case_sensitive', False))
-        if dotenv_vars:
-            env_vars = {**dotenv_vars, **env_vars}
-
-        return env_vars
+    def _load_env_vars(self) -> Mapping[str, str | None]:
+        return self._read_env_files(self.settings_cls.model_config.get('case_sensitive', False))
 
-    def _read_env_files(self, case_sensitive: bool) -> Mapping[str, Optional[str]]:
+    def _read_env_files(self, case_sensitive: bool) -> Mapping[str, str | None]:
         env_files = self.env_file
         if env_files is None:
             return {}
 
         if isinstance(env_files, (str, os.PathLike)):
             env_files = [env_files]
 
-        dotenv_vars = {}
+        dotenv_vars: dict[str, str | None] = {}
         for env_file in env_files:
             env_path = Path(env_file).expanduser()
             if env_path.is_file():
                 dotenv_vars.update(
                     read_env_file(env_path, encoding=self.env_file_encoding, case_sensitive=case_sensitive)
                 )
 
         return dotenv_vars
 
+    def __call__(self) -> dict[str, Any]:
+        data: dict[str, Any] = super().__call__()
+
+        data_lower_keys: List[str] = []
+        if not self.settings_cls.model_config.get('case_sensitive', False):
+            data_lower_keys = [x.lower() for x in data.keys()]
+
+        # As `extra` config is allowed in dotenv settings source, We have to
+        # update data with extra env variabels from dotenv file.
+        for env_name, env_value in self.env_vars.items():
+            if env_value is not None:
+                env_name_without_prefix = env_name[self.env_prefix_len :]
+                first_key, *_ = env_name_without_prefix.split(self.env_nested_delimiter)
+
+                if (data_lower_keys and first_key not in data_lower_keys) or (
+                    not data_lower_keys and first_key not in data
+                ):
+                    data[first_key] = env_value
+
+        return data
+
     def __repr__(self) -> str:
         return (
             f'DotEnvSettingsSource(env_file={self.env_file!r}, env_file_encoding={self.env_file_encoding!r}, '
             f'env_nested_delimiter={self.env_nested_delimiter!r}, env_prefix_len={self.env_prefix_len!r})'
         )
 
 
-def read_env_file(file_path: Path, *, encoding: str = None, case_sensitive: bool = False) -> Dict[str, Optional[str]]:
+def read_env_file(
+    file_path: Path, *, encoding: str | None = None, case_sensitive: bool = False
+) -> Mapping[str, str | None]:
     try:
         from dotenv import dotenv_values
     except ImportError as e:
         raise ImportError('python-dotenv is not installed, run `pip install pydantic[dotenv]`') from e
 
-    file_vars: Dict[str, Optional[str]] = dotenv_values(file_path, encoding=encoding or 'utf8')
+    file_vars: dict[str, str | None] = dotenv_values(file_path, encoding=encoding or 'utf8')
     if not case_sensitive:
         return {k.lower(): v for k, v in file_vars.items()}
     else:
         return file_vars
 
 
-def find_case_path(dir_path: Path, file_name: str, case_sensitive: bool) -> Optional[Path]:
+def find_case_path(dir_path: Path, file_name: str, case_sensitive: bool) -> Path | None:
     """
     Find a file within path's directory matching filename, optionally ignoring case.
     """
     for f in dir_path.iterdir():
         if f.name == file_name:
             return f
         elif not case_sensitive and f.name.lower() == file_name.lower():
```

### Comparing `pydantic_settings-2.0a3/pydantic_settings/utils.py` & `pydantic_settings-2.0a4/pydantic_settings/utils.py`

 * *Files identical despite different names*

### Comparing `pydantic_settings-2.0a3/requirements/linting.txt` & `pydantic_settings-2.0a4/requirements/linting.txt`

 * *Files identical despite different names*

### Comparing `pydantic_settings-2.0a3/requirements/testing.txt` & `pydantic_settings-2.0a4/requirements/testing.txt`

 * *Files identical despite different names*

### Comparing `pydantic_settings-2.0a3/tests/test_settings.py` & `pydantic_settings-2.0a4/tests/test_settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -676,20 +676,25 @@
     p.write_text(test_env_file)
 
     class Settings(BaseSettings):
         a: str
         b: str
         c: str
 
-        model_config = ConfigDict(env_file=p, case_sensitive=True)
+        model_config = ConfigDict(env_file=p, case_sensitive=True, extra='ignore')
 
     with pytest.raises(ValidationError) as exc_info:
         Settings()
     assert exc_info.value.errors() == [
-        {'type': 'missing', 'loc': ('a',), 'msg': 'Field required', 'input': {'b': 'better string', 'c': 'best string'}}
+        {
+            'type': 'missing',
+            'loc': ('a',),
+            'msg': 'Field required',
+            'input': {'b': 'better string', 'c': 'best string', 'A': 'good string'},
+        }
     ]
 
 
 @pytest.mark.skipif(not dotenv, reason='python-dotenv not installed')
 def test_env_file_export(env, tmp_path):
     p = tmp_path / '.env'
     p.write_text(
@@ -1508,7 +1513,72 @@
 
     env.set('nested', '{"val1": "v1", "sub_SUB": {"VAL2": "v2", "sub_SUB_sUb": {"vAl3": "v3", "VAL4": "v4"}}}')
     s = Settings()
     assert s.nested.VAL1 == 'v1'
     assert s.nested.SUB_sub.Val2 == 'v2'
     assert s.nested.SUB_sub.SUB_sub_SuB.VaL3 == 'v3'
     assert s.nested.SUB_sub.SUB_sub_SuB.val4 == 'v4'
+
+
+@pytest.mark.skipif(not dotenv, reason='python-dotenv not installed')
+def test_dotenv_extra_allow(tmp_path):
+    p = tmp_path / '.env'
+    p.write_text('a=b\nx=y')
+
+    class Settings(BaseSettings):
+        a: str
+
+        model_config = ConfigDict(env_file=p, extra='allow')
+
+    s = Settings()
+    assert s.a == 'b'
+    assert s.x == 'y'
+
+
+@pytest.mark.skipif(not dotenv, reason='python-dotenv not installed')
+def test_dotenv_extra_forbid(tmp_path):
+    p = tmp_path / '.env'
+    p.write_text('a=b\nx=y')
+
+    class Settings(BaseSettings):
+        a: str
+
+        model_config = ConfigDict(env_file=p, extra='forbid')
+
+    with pytest.raises(ValidationError) as exc_info:
+        Settings()
+    assert exc_info.value.errors() == [
+        {'type': 'extra_forbidden', 'loc': ('x',), 'msg': 'Extra inputs are not permitted', 'input': 'y'}
+    ]
+
+
+@pytest.mark.skipif(not dotenv, reason='python-dotenv not installed')
+def test_dotenv_extra_case_insensitive(tmp_path):
+    p = tmp_path / '.env'
+    p.write_text('a=b')
+
+    class Settings(BaseSettings):
+        A: str
+
+        model_config = ConfigDict(env_file=p, extra='forbid')
+
+    s = Settings()
+    assert s.A == 'b'
+
+
+@pytest.mark.skipif(not dotenv, reason='python-dotenv not installed')
+def test_dotenv_extra_sub_model_case_insensitive(tmp_path):
+    p = tmp_path / '.env'
+    p.write_text('a=b\nSUB_model={"v": "v1"}')
+
+    class SubModel(BaseModel):
+        v: str
+
+    class Settings(BaseSettings):
+        A: str
+        sub_MODEL: SubModel
+
+        model_config = ConfigDict(env_file=p, extra='forbid')
+
+    s = Settings()
+    assert s.A == 'b'
+    assert s.sub_MODEL.v == 'v1'
```

### Comparing `pydantic_settings-2.0a3/LICENSE` & `pydantic_settings-2.0a4/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_settings-2.0a3/README.md` & `pydantic_settings-2.0a4/README.md`

 * *Files identical despite different names*

### Comparing `pydantic_settings-2.0a3/pyproject.toml` & `pydantic_settings-2.0a4/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -25,14 +25,16 @@
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
     'Programming Language :: Python :: 3.11',
     'Intended Audience :: Developers',
     'Intended Audience :: Information Technology',
     'Intended Audience :: System Administrators',
     'License :: OSI Approved :: MIT License',
+    'Framework :: Pydantic',
+    'Framework :: Pydantic :: 2',
     'Operating System :: Unix',
     'Operating System :: POSIX :: Linux',
     'Environment :: Console',
     'Environment :: MacOS X',
     'Topic :: Software Development :: Libraries :: Python Modules',
     'Topic :: Internet',
 ]
```

### Comparing `pydantic_settings-2.0a3/PKG-INFO` & `pydantic_settings-2.0a4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: pydantic-settings
-Version: 2.0a3
+Version: 2.0a4
 Summary: Settings management using Pydantic
 Project-URL: Homepage, https://github.com/pydantic/pydantic-settings
 Project-URL: Funding, https://github.com/sponsors/samuelcolvin
 Project-URL: Source, https://github.com/pydantic/pydantic-settings
 Project-URL: Changelog, https://github.com/pydantic/pydantic-settings/releases
 Author-email: Samuel Colvin <s@muelcolvin.com>, Eric Jolibois <em.jolibois@gmail.com>, Hasan Ramezani <hasan.r67@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: MacOS X
+Classifier: Framework :: Pydantic
+Classifier: Framework :: Pydantic :: 2
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python
```

