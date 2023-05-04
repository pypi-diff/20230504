# Comparing `tmp/oobabot-0.1.0.tar.gz` & `tmp/oobabot-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oobabot-0.1.0.tar", max compression
+gzip compressed data, was "oobabot-0.1.2.tar", max compression
```

## Comparing `oobabot-0.1.0.tar` & `oobabot-0.1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1067 2023-05-04 00:39:46.200078 oobabot-0.1.0/LICENSE
--rw-r--r--   0        0        0     7464 2023-05-04 05:25:50.455313 oobabot-0.1.0/README.md
--rw-r--r--   0        0        0      557 2023-05-04 02:10:58.898559 oobabot-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       45 2023-05-04 00:39:46.200078 oobabot-0.1.0/src/oobabot/__init__.py
--rw-r--r--   0        0        0       69 2023-05-04 00:39:46.200078 oobabot-0.1.0/src/oobabot/__main__.py
--rw-r--r--   0        0        0     9368 2023-05-04 04:16:20.656470 oobabot-0.1.0/src/oobabot/discord_bot.py
--rw-r--r--   0        0        0     1560 2023-05-04 00:39:46.200078 oobabot-0.1.0/src/oobabot/fancy_logging.py
--rw-r--r--   0        0        0     2939 2023-05-04 00:39:46.200078 oobabot-0.1.0/src/oobabot/ooba_client.py
--rwxr-xr-x   0        0        0     2159 2023-05-04 04:15:27.736485 oobabot-0.1.0/src/oobabot/oobabot.py
--rw-r--r--   0        0        0     6658 2023-05-04 00:39:46.200078 oobabot-0.1.0/src/oobabot/response_stats.py
--rw-r--r--   0        0        0     2729 2023-05-04 00:39:46.200078 oobabot-0.1.0/src/oobabot/sentence_splitter.py
--rw-r--r--   0        0        0     3867 2023-05-04 04:15:11.386489 oobabot-0.1.0/src/oobabot/settings.py
--rw-r--r--   0        0        0     8187 1970-01-01 00:00:00.000000 oobabot-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-05-04 00:39:46.200078 oobabot-0.1.2/LICENSE
+-rw-r--r--   0        0        0     7464 2023-05-04 05:25:50.455313 oobabot-0.1.2/README.md
+-rw-r--r--   0        0        0      609 2023-05-04 06:11:36.022566 oobabot-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0       45 2023-05-04 06:11:56.742561 oobabot-0.1.2/src/oobabot/__init__.py
+-rw-r--r--   0        0        0       69 2023-05-04 00:39:46.200078 oobabot-0.1.2/src/oobabot/__main__.py
+-rw-r--r--   0        0        0     9425 2023-05-04 05:57:27.632802 oobabot-0.1.2/src/oobabot/discord_bot.py
+-rw-r--r--   0        0        0     1560 2023-05-04 00:39:46.200078 oobabot-0.1.2/src/oobabot/fancy_logging.py
+-rw-r--r--   0        0        0     2939 2023-05-04 00:39:46.200078 oobabot-0.1.2/src/oobabot/ooba_client.py
+-rwxr-xr-x   0        0        0     2159 2023-05-04 04:15:27.736485 oobabot-0.1.2/src/oobabot/oobabot.py
+-rw-r--r--   0        0        0     6658 2023-05-04 00:39:46.200078 oobabot-0.1.2/src/oobabot/response_stats.py
+-rw-r--r--   0        0        0     2729 2023-05-04 00:39:46.200078 oobabot-0.1.2/src/oobabot/sentence_splitter.py
+-rw-r--r--   0        0        0     3899 2023-05-04 06:00:50.732746 oobabot-0.1.2/src/oobabot/settings.py
+-rw-r--r--   0        0        0     8297 1970-01-01 00:00:00.000000 oobabot-0.1.2/PKG-INFO
```

### Comparing `oobabot-0.1.0/LICENSE` & `oobabot-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `oobabot-0.1.0/README.md` & `oobabot-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `oobabot-0.1.0/pyproject.toml` & `oobabot-0.1.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 [tool.poetry]
 name = "oobabot"
-version = "0.1.0"
+version = "0.1.2"
 description = "A Discord bot which talks to Large Language Model AIs running on oobabooga's text-generation-webui"
 authors = ["Christopher Rude <chris@rudesoftware.net>"]
 license = "MIT"
 readme = "README.md"
+repository = "https://github.com/chrisrude/oobabot"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 "discord.py" = "^2.2.2"
 pysbd = "^0.3.4"
 websockets = "^11"
```

### Comparing `oobabot-0.1.0/src/oobabot/discord_bot.py` & `oobabot-0.1.2/src/oobabot/discord_bot.py`

 * *Files 2% similar despite different names*

```diff
@@ -218,15 +218,16 @@
     def log_stats(self) -> None:
         self.average_stats.write_stat_summary_to_log()
 
     async def on_message(self, raw_message: discord.Message) -> None:
         if not self.should_reply_to_message(raw_message):
             return
         try:
-            await self.send_response(raw_message)
+            async with raw_message.channel.typing():
+                await self.send_response(raw_message)
         except Exception as e:
             get_logger().error(
                 f'Exception while sending response: {e}', exc_info=True)
 
     async def send_response(self, raw_message: discord.Message) -> None:
         clean_message = sanitize_message(raw_message)
         author = clean_message['author']
```

### Comparing `oobabot-0.1.0/src/oobabot/fancy_logging.py` & `oobabot-0.1.2/src/oobabot/fancy_logging.py`

 * *Files identical despite different names*

### Comparing `oobabot-0.1.0/src/oobabot/ooba_client.py` & `oobabot-0.1.2/src/oobabot/ooba_client.py`

 * *Files identical despite different names*

### Comparing `oobabot-0.1.0/src/oobabot/oobabot.py` & `oobabot-0.1.2/src/oobabot/oobabot.py`

 * *Files identical despite different names*

### Comparing `oobabot-0.1.0/src/oobabot/response_stats.py` & `oobabot-0.1.2/src/oobabot/response_stats.py`

 * *Files identical despite different names*

### Comparing `oobabot-0.1.0/src/oobabot/sentence_splitter.py` & `oobabot-0.1.2/src/oobabot/sentence_splitter.py`

 * *Files identical despite different names*

### Comparing `oobabot-0.1.0/src/oobabot/settings.py` & `oobabot-0.1.2/src/oobabot/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,14 +70,15 @@
             action='store_true'
         )
         self.add_argument(
             '--log-all-the-things',
             default=False,
             help='prints all oobabooga requests and responses in their ' +
             'entirety to STDOUT',
+            action='store_true'
         )
 
     def settings(self) -> dict[str, str]:
         if self._settings is None:
             self._settings = self.parse_args().__dict__
 
             # this is a bit of a hack, but it's the only setting
```

### Comparing `oobabot-0.1.0/PKG-INFO` & `oobabot-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: oobabot
-Version: 0.1.0
+Version: 0.1.2
 Summary: A Discord bot which talks to Large Language Model AIs running on oobabooga's text-generation-webui
+Home-page: https://github.com/chrisrude/oobabot
 License: MIT
 Author: Christopher Rude
 Author-email: chris@rudesoftware.net
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: discord.py (>=2.2.2,<3.0.0)
 Requires-Dist: pysbd (>=0.3.4,<0.4.0)
 Requires-Dist: websockets (>=11,<12)
+Project-URL: Repository, https://github.com/chrisrude/oobabot
 Description-Content-Type: text/markdown
 
 # `oobabot`
 
 **`oobabot`** is a Discord bot which talks to a Large Language Model AIs (like LLaMA, llama.cpp, etc...), running on [oobabooga's text-generation-webui](https://github.com/oobabooga/text-generation-webui).
 
 [![python lint and test with poetry](https://github.com/chrisrude/oobabot/actions/workflows/python-package.yml/badge.svg)](https://github.com/chrisrude/oobabot/actions/workflows/python-package.yml)
```

