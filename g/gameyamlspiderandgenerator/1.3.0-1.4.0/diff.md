# Comparing `tmp/gameyamlspiderandgenerator-1.3.0.tar.gz` & `tmp/gameyamlspiderandgenerator-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gameyamlspiderandgenerator-1.3.0.tar", max compression
+gzip compressed data, was "gameyamlspiderandgenerator-1.4.0.tar", max compression
```

## Comparing `gameyamlspiderandgenerator-1.3.0.tar` & `gameyamlspiderandgenerator-1.4.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
--rwxr-xr-x   0        0        0     1069 2023-04-20 06:26:01.842563 gameyamlspiderandgenerator-1.3.0/LICENSE
--rwxr-xr-x   0        0        0      809 2023-04-20 06:26:01.842841 gameyamlspiderandgenerator-1.3.0/README.md
--rwxr-xr-x   0        0        0      604 2023-04-20 08:11:44.723735 gameyamlspiderandgenerator-1.3.0/gameyamlspiderandgenerator/__init__.py
--rwxr-xr-x   0        0        0      980 2023-04-20 06:26:01.843615 gameyamlspiderandgenerator-1.3.0/gameyamlspiderandgenerator/__main__.py
--rwxr-xr-x   0        0        0      753 2023-04-20 06:26:01.843909 gameyamlspiderandgenerator-1.3.0/gameyamlspiderandgenerator/exception.py
--rwxr-xr-x   0        0        0       52 2023-04-20 06:26:01.844401 gameyamlspiderandgenerator-1.3.0/gameyamlspiderandgenerator/hook/__init__.py
--rwxr-xr-x   0        0        0      194 2023-04-20 06:26:01.844722 gameyamlspiderandgenerator-1.3.0/gameyamlspiderandgenerator/hook/_base.py
--rwxr-xr-x   0        0        0     2659 2023-04-20 08:17:40.725993 gameyamlspiderandgenerator-1.3.0/gameyamlspiderandgenerator/hook/search.py
--rwxr-xr-x   0        0        0       56 2023-04-20 06:26:01.845620 gameyamlspiderandgenerator-1.3.0/gameyamlspiderandgenerator/plugin/__init__.py
--rwxr-xr-x   0        0        0     2586 2023-04-20 08:13:25.308014 gameyamlspiderandgenerator-1.3.0/gameyamlspiderandgenerator/plugin/_base.py
--rwxr-xr-x   0        0        0     7013 2023-04-20 07:59:29.061316 gameyamlspiderandgenerator-1.3.0/gameyamlspiderandgenerator/plugin/itchio.py
--rwxr-xr-x   0        0        0     7706 2023-04-20 08:13:03.423899 gameyamlspiderandgenerator-1.3.0/gameyamlspiderandgenerator/plugin/steam.py
--rwxr-xr-x   0        0        0        0 2023-04-20 06:26:01.847280 gameyamlspiderandgenerator-1.3.0/gameyamlspiderandgenerator/util/__init__.py
--rwxr-xr-x   0        0        0     1133 2023-04-20 06:26:01.847686 gameyamlspiderandgenerator-1.3.0/gameyamlspiderandgenerator/util/config.py
--rwxr-xr-x   0        0        0     1459 2023-04-20 08:19:19.429134 gameyamlspiderandgenerator-1.3.0/gameyamlspiderandgenerator/util/fgi.py
--rwxr-xr-x   0        0        0     1908 2023-04-20 06:26:01.848348 gameyamlspiderandgenerator-1.3.0/gameyamlspiderandgenerator/util/fgi_yaml.py
--rwxr-xr-x   0        0        0     1944 2023-04-20 06:26:01.848713 gameyamlspiderandgenerator-1.3.0/gameyamlspiderandgenerator/util/plugin_manager.py
--rwxr-xr-x   0        0        0     2611 2023-04-20 06:26:01.849061 gameyamlspiderandgenerator-1.3.0/gameyamlspiderandgenerator/util/spider.py
--rwxr-xr-x   0        0        0      639 2023-04-20 08:23:07.635645 gameyamlspiderandgenerator-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     1827 1970-01-01 00:00:00.000000 gameyamlspiderandgenerator-1.3.0/PKG-INFO
+-rwxr-xr-x   0        0        0     1069 2023-04-20 06:26:01.842563 gameyamlspiderandgenerator-1.4.0/LICENSE
+-rwxr-xr-x   0        0        0      809 2023-04-20 06:26:01.842841 gameyamlspiderandgenerator-1.4.0/README.md
+-rwxr-xr-x   0        0        0      568 2023-05-04 05:49:53.911342 gameyamlspiderandgenerator-1.4.0/gameyamlspiderandgenerator/__init__.py
+-rwxr-xr-x   0        0        0     1751 2023-05-04 05:14:28.057718 gameyamlspiderandgenerator-1.4.0/gameyamlspiderandgenerator/__main__.py
+-rwxr-xr-x   0        0        0      753 2023-04-20 06:26:01.843909 gameyamlspiderandgenerator-1.4.0/gameyamlspiderandgenerator/exception.py
+-rwxr-xr-x   0        0        0       52 2023-04-20 06:26:01.844401 gameyamlspiderandgenerator-1.4.0/gameyamlspiderandgenerator/hook/__init__.py
+-rwxr-xr-x   0        0        0      194 2023-04-20 06:26:01.844722 gameyamlspiderandgenerator-1.4.0/gameyamlspiderandgenerator/hook/_base.py
+-rwxr-xr-x   0        0        0     3689 2023-05-04 05:33:16.574689 gameyamlspiderandgenerator-1.4.0/gameyamlspiderandgenerator/hook/search.py
+-rwxr-xr-x   0        0        0      594 2023-05-04 05:33:16.693167 gameyamlspiderandgenerator-1.4.0/gameyamlspiderandgenerator/hook/validate.py
+-rwxr-xr-x   0        0        0       56 2023-04-20 06:26:01.845620 gameyamlspiderandgenerator-1.4.0/gameyamlspiderandgenerator/plugin/__init__.py
+-rwxr-xr-x   0        0        0     2608 2023-05-04 05:41:40.944094 gameyamlspiderandgenerator-1.4.0/gameyamlspiderandgenerator/plugin/_base.py
+-rwxr-xr-x   0        0        0     7013 2023-05-04 05:01:11.453272 gameyamlspiderandgenerator-1.4.0/gameyamlspiderandgenerator/plugin/itchio.py
+-rwxr-xr-x   0        0        0     7709 2023-05-04 05:01:29.119132 gameyamlspiderandgenerator-1.4.0/gameyamlspiderandgenerator/plugin/steam.py
+-rwxr-xr-x   0        0        0        0 2023-04-20 06:26:01.847280 gameyamlspiderandgenerator-1.4.0/gameyamlspiderandgenerator/util/__init__.py
+-rwxr-xr-x   0        0        0     1132 2023-05-03 13:24:54.468858 gameyamlspiderandgenerator-1.4.0/gameyamlspiderandgenerator/util/config.py
+-rwxr-xr-x   0        0        0     1459 2023-04-20 08:19:19.429134 gameyamlspiderandgenerator-1.4.0/gameyamlspiderandgenerator/util/fgi.py
+-rwxr-xr-x   0        0        0     1892 2023-05-04 02:54:35.897355 gameyamlspiderandgenerator-1.4.0/gameyamlspiderandgenerator/util/fgi_yaml.py
+-rwxr-xr-x   0        0        0     1944 2023-05-04 03:20:05.673595 gameyamlspiderandgenerator-1.4.0/gameyamlspiderandgenerator/util/plugin_manager.py
+-rwxr-xr-x   0        0        0     2611 2023-04-20 06:26:01.849061 gameyamlspiderandgenerator-1.4.0/gameyamlspiderandgenerator/util/spider.py
+-rwxr-xr-x   0        0        0      646 2023-05-04 05:57:56.690154 gameyamlspiderandgenerator-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1842 1970-01-01 00:00:00.000000 gameyamlspiderandgenerator-1.4.0/PKG-INFO
```

### Comparing `gameyamlspiderandgenerator-1.3.0/LICENSE` & `gameyamlspiderandgenerator-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.3.0/README.md` & `gameyamlspiderandgenerator-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.3.0/gameyamlspiderandgenerator/__init__.py` & `gameyamlspiderandgenerator-1.4.0/gameyamlspiderandgenerator/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 from loguru import logger
 
 from .plugin import BasePlugin
 from .util.fgi_yaml import YamlData
 from .util.plugin_manager import pkg
 
 
-def verify(url: str) -> Optional[BasePlugin]:
+def verify(url: str):
     verify_list = [
         [
             pkg.plugin[n].verify,
             pkg.plugin[n],
         ]
         for n in pkg.plugin
     ]
     return next((cls for func, cls in verify_list if func(url)), None)
 
 
 def produce_yaml(url: str) -> Optional[YamlData]:
-    ret: BasePlugin = verify(url)
+    ret = verify(url)
     if ret is None:
         logger.error("URL is invalid")
         return
     return ret(url).to_yaml()
```

### Comparing `gameyamlspiderandgenerator-1.3.0/gameyamlspiderandgenerator/exception.py` & `gameyamlspiderandgenerator-1.4.0/gameyamlspiderandgenerator/exception.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.3.0/gameyamlspiderandgenerator/hook/search.py` & `gameyamlspiderandgenerator-1.4.0/gameyamlspiderandgenerator/hook/search.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,64 +2,96 @@
 from urllib.parse import quote_plus
 
 from bs4 import BeautifulSoup
 from loguru import logger
 
 from ..hook import BaseHook
 from ..util.config import config
-from ..util.spider import get_json, get_text
+from ..util.spider import get_json
 
-print(config, type(config))
+# print(config, type(config))
 
 
 class Search(BaseHook):
     @staticmethod
-    def name_filter(s: str, rep: str = ""):
-        return sub("[^A-z]", rep, s.lower())
+    def name_filter(string: str, pattern: str = r"[^A-z]", repl: str = ""):
+        """
+
+        Args:
+            string: The string to be replaced
+            pattern: Regular expression, replace non-English letters by default
+            repl: The string to replace with
+
+        Returns:
+
+        """
+        return sub(pattern, repl, string)
 
     def __init__(self, name: str) -> None:
         logger.info(f"Hook: init {name}")
         self.pure = self.name_filter(name)
-        self.encode = quote_plus(self.name_filter(name, " "))
+        self.encode = quote_plus(self.name_filter(name, repl=" "))
 
-    def search_play(self):
+    def search_play(self)-> tuple:
         data = get_json(
             "https://serpapi.com/search?engine=google_play&apikey="
             f'{config["api"]["google-play"]}&store=apps&q={self.encode}'
         )
         if "organic_results" in data and any(
                 [self.name_filter(i["title"]) == self.pure for i in data["organic_results"][0]["items"]]):
             logger.info("FOUND: google_play")
             return "google-play", {'name': '.play-store',
                                    'uri': f'google-play-store:{data["organic_results"][0]["items"][0]["product_id"]}'}
-        return [[], []]
+        return ([], [])
 
-    def search_apple(self):
+    def search_apple(self)-> tuple:
         data = get_json(
             "https://serpapi.com/search.json?engine=apple_app_store&term="
             f'{self.encode}&apikey={config["api"]["apple"]}'
         )
         if "organic_results" in data and any(
                 [self.name_filter(i["title"]) == self.pure for i in data["organic_results"]]):
             logger.info("FOUND: apple_app_store")
             return "apple-appstore", {'name': '.apple-appstore', 'uri': data["organic_results"][0]["link"]}
-        return [[], []]
+        return ([], [])
 
     def search_all(self) -> list:
         func_list = [
             self.__getattribute__(i)
             for i in (list(filter(lambda x: "__" not in x, self.__dir__())))
         ]
         func_list = filter(
             lambda x: callable(x) and x.__name__.startswith("search") and x.__name__ != "search_all",
             func_list,
         )
         return [ii() for ii in func_list]
 
+    def search_epic(self):
+        from epicstore_api import EpicGamesStoreAPI
+
+        api = EpicGamesStoreAPI().fetch_store_games(keywords="TUNIC", sort_dir="DESC")
+        game_list = api['data']['Catalog']['searchStore']['elements']
+        reg = r"[^A-z\d]"
+        if game_list and any(
+                [self.name_filter(i["title"]) == self.pure for i in game_list]):
+            logger.info("FOUND: epic")
+            return "epic", {'name': '.epic',
+                            'uri': f'https://store.epicgames.com/p/{self.name_filter(game_list[0]["title"], pattern=reg, repl="-")}'}
+        return [[], []]
+
     def setup(self, data: dict):
+        """
+        hook handler
+        Args:
+            data: yaml daya
+
+        Returns:
+            The processed dict data
+
+        """
         temp = data.copy()
         try:
             result = self.search_all()
             publish = [i[0] for i in result] + temp["tags"]['publish']
             link = [i[1] for i in result] + temp["links"]
 
             def rm_empty(s: list):
```

### Comparing `gameyamlspiderandgenerator-1.3.0/gameyamlspiderandgenerator/plugin/_base.py` & `gameyamlspiderandgenerator-1.4.0/gameyamlspiderandgenerator/plugin/_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,18 +24,20 @@
     def __load_hook__(self, data: dict):
         """
         加载钩子
 
         Args:
             data: 钩子数据
         """
+
         from gameyamlspiderandgenerator.util.plugin_manager import pkg
         pkg.__init__()
         for i in pkg.hook.values():
-            return i(self.get_name()).setup(data)
+            data = i(self.get_name()).setup(data)
+        return data
 
     @abc.abstractmethod
     def get_name(self) -> str:
         """
         获取游戏名称
 
         Returns:
@@ -136,7 +138,8 @@
     def to_yaml(self) -> str:
         """
         转换为 YAML
 
         Returns:
             YAML
         """
+
```

### Comparing `gameyamlspiderandgenerator-1.3.0/gameyamlspiderandgenerator/plugin/itchio.py` & `gameyamlspiderandgenerator-1.4.0/gameyamlspiderandgenerator/plugin/itchio.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,15 @@
             "iOS": "ios",
         }
         platforms = self.more_info["Platforms"][0].split(",") if "Platforms" in self.more_info else ["Windows"]
         return [repl[i.strip()] for i in platforms]
 
     def get_authors(self) -> list[dict]:
         temp = self.more_info["Author"]
-        return [{"name": i, "role": "developer"} for i in temp]
+        return [{"name": i, "role": ["producer"]} for i in temp]
 
     def get_tags(self) -> list[str]:
         temp = self.more_info["Genre"] if "Genre" in self.more_info else []
         temp1 = self.more_info["Made with"] if "Made with" in self.more_info else []
         temp2 = self.more_info["Tags"]
         return [i.strip() for i in (temp2 + temp1 + temp)]
 
@@ -142,15 +142,14 @@
                 cache = self.soup.select_one(
                     f"div.info_panel_wrapper > div > table > tbody > tr:nth-child({str(i)})"
                 )
                 temp = [i.get_text() for i in list(cache.children)]
                 d[temp[0]] = temp[1:][0].split(",")
         return d
 
-
     def to_yaml(self) -> YamlData:
         ret = {
             "name": self.get_name(),
             "brief-description": self.get_brief_desc(),
             "description": self.get_desc(),
             "description-format": "markdown",
             "authors": self.get_authors(),
```

### Comparing `gameyamlspiderandgenerator-1.3.0/gameyamlspiderandgenerator/plugin/steam.py` & `gameyamlspiderandgenerator-1.4.0/gameyamlspiderandgenerator/plugin/steam.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,16 +76,16 @@
     def get_brief_desc(self):
         return pss_dedent(
             html2text(self.data[str(self.id)]["data"]["short_description"], bodywidth=0)
         )
 
     def get_authors(self) -> list[dict]:
         temp = self.data[str(self.id)]["data"]
-        developers = [{"name": i, "role": "developer"} for i in temp["developers"]]
-        publishers = [{"name": i, "role": "publisher"} for i in temp["publishers"]]
+        developers = [{"name": i, "role": ["producer"]} for i in temp["developers"]]
+        publishers = [{"name": i, "role": ["publisher"]} for i in temp["publishers"]]
         return developers + publishers
 
     def get_platforms(self):
         temp = self.data[str(self.id)]["data"]["platforms"]
         repl = {"windows": "windows", "mac": "macos", "linux": "linux"}
         return [repl[i] for i in temp if i]
```

### Comparing `gameyamlspiderandgenerator-1.3.0/gameyamlspiderandgenerator/util/config.py` & `gameyamlspiderandgenerator-1.4.0/gameyamlspiderandgenerator/util/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,16 +13,15 @@
         # Compatibility with the old version
         return self.__getattribute__(item)
 
     def __setitem__(self, key, value):
         # Compatibility with the old version
         self.__setattr__(key, value)
 
-
-    def load(self, file_data: str | dict | None):
+    def load(self, file_data: str | dict = None):
         if type(file_data) is dict:
             self.__dict__.update(file_data)
             return
         if file_data is None:
             self.__dict__.update(default_config)
             return
         try:
```

### Comparing `gameyamlspiderandgenerator-1.3.0/gameyamlspiderandgenerator/util/fgi.py` & `gameyamlspiderandgenerator-1.4.0/gameyamlspiderandgenerator/util/fgi.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.3.0/gameyamlspiderandgenerator/util/fgi_yaml.py` & `gameyamlspiderandgenerator-1.4.0/gameyamlspiderandgenerator/util/fgi_yaml.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     for i in list(data.keys())[1:]:
         temp = temp.replace("\n" + i, "\n\n" + i)
     return temp
 
 
 def process_thumbnail(img_byte: bytes):
     img = Image.open(BytesIO(img_byte))
-    if img.size[0] % 360 == img.size[1] % 168:
+    if img.size == (460, 215):
         img_resize = img.resize((360, 168))
         ret_byte = BytesIO()
         img_resize.save(ret_byte, format="PNG", optimize=True, quality=85)
         return ret_byte.getvalue()
     logger.warning("Thumbnails cannot be scaled down.")
     return img_byte
```

### Comparing `gameyamlspiderandgenerator-1.3.0/gameyamlspiderandgenerator/util/plugin_manager.py` & `gameyamlspiderandgenerator-1.4.0/gameyamlspiderandgenerator/util/plugin_manager.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.3.0/gameyamlspiderandgenerator/util/spider.py` & `gameyamlspiderandgenerator-1.4.0/gameyamlspiderandgenerator/util/spider.py`

 * *Files identical despite different names*

### Comparing `gameyamlspiderandgenerator-1.3.0/pyproject.toml` & `gameyamlspiderandgenerator-1.4.0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gameyamlspiderandgenerator"
-version = "1.3.0"
+version = "1.4.0"
 description = ""
 authors = ["kaesinol"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
@@ -12,21 +12,21 @@
 language-data = "^1.1"
 html2text = "^2020.1.16"
 "ruamel.yaml" = "^0.17.21"
 "ruamel.yaml.string" = "^0.1.0"
 urllib3 = "^1.26.14"
 beautifulsoup4 = "^4.11.1"
 pillow = "^9.4.0"
-pygithub = "^1.57"
 requests = "^2.28.2"
 ruamel-base = "^1.0.0"
 loguru = "^0.6.0"
 pyyaml = "^6.0"
 pysocks = "^1.7.1"
-marisa-trie = "0.7.8"
+epicstore-api = "^0.1.6"
+jsonschema = "^4.17.3"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
 profile = "black"
```

### Comparing `gameyamlspiderandgenerator-1.3.0/PKG-INFO` & `gameyamlspiderandgenerator-1.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: gameyamlspiderandgenerator
-Version: 1.3.0
+Version: 1.4.0
 Summary: 
 License: MIT
 Author: kaesinol
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: beautifulsoup4 (>=4.11.1,<5.0.0)
+Requires-Dist: epicstore-api (>=0.1.6,<0.2.0)
 Requires-Dist: html2text (>=2020.1.16,<2021.0.0)
+Requires-Dist: jsonschema (>=4.17.3,<5.0.0)
 Requires-Dist: langcodes (>=3.3.0,<4.0.0)
 Requires-Dist: language-data (>=1.1,<2.0)
 Requires-Dist: loguru (>=0.6.0,<0.7.0)
-Requires-Dist: marisa-trie (==0.7.8)
 Requires-Dist: pillow (>=9.4.0,<10.0.0)
-Requires-Dist: pygithub (>=1.57,<2.0)
 Requires-Dist: pysocks (>=1.7.1,<2.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Requires-Dist: ruamel-base (>=1.0.0,<2.0.0)
 Requires-Dist: ruamel.yaml (>=0.17.21,<0.18.0)
 Requires-Dist: ruamel.yaml.string (>=0.1.0,<0.2.0)
 Requires-Dist: urllib3 (>=1.26.14,<2.0.0)
```

