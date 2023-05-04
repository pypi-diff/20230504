# Comparing `tmp/aiotubes-3.4.tar.gz` & `tmp/aiotubes-3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiotubes-3.4.tar", last modified: Mon May  1 10:29:33 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `aiotubes-3.4.tar` & `aiotubes-3.5.tar`

### file list

```diff
@@ -1,23 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 10:29:33.292484 aiotubes-3.4/
--rw-rw-rw-   0        0        0     1084 2022-10-11 08:30:57.000000 aiotubes-3.4/LICENSE
--rw-rw-rw-   0        0        0      697 2023-05-01 10:29:33.292484 aiotubes-3.4/PKG-INFO
--rw-rw-rw-   0        0        0      361 2023-04-23 14:57:43.000000 aiotubes-3.4/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-01 10:29:33.275530 aiotubes-3.4/aiotube/
--rw-rw-rw-   0        0        0       58 2023-04-23 14:53:51.000000 aiotubes-3.4/aiotube/__init__.py
--rw-rw-rw-   0        0        0     2990 2023-05-01 10:10:21.000000 aiotubes-3.4/aiotube/client.py
--rw-rw-rw-   0        0        0     1122 2023-05-01 09:27:21.000000 aiotubes-3.4/aiotube/constants.py
--rw-rw-rw-   0        0        0     2511 2023-04-23 14:53:45.000000 aiotubes-3.4/aiotube/exceptions.py
--rw-rw-rw-   0        0        0     5405 2023-04-23 14:53:51.000000 aiotubes-3.4/aiotube/extractors.py
--rw-rw-rw-   0        0        0     2015 2023-04-24 06:32:12.000000 aiotubes-3.4/aiotube/helpers.py
--rw-rw-rw-   0        0        0     4427 2023-02-24 13:57:51.000000 aiotubes-3.4/aiotube/itags.py
--rw-rw-rw-   0        0        0     2226 2023-04-23 14:53:51.000000 aiotubes-3.4/aiotube/playlist.py
--rw-rw-rw-   0        0        0     8126 2023-05-01 10:28:02.000000 aiotubes-3.4/aiotube/streams.py
--rw-rw-rw-   0        0        0     4946 2023-05-01 10:10:39.000000 aiotubes-3.4/aiotube/video.py
-drwxrwxrwx   0        0        0        0 2023-05-01 10:29:33.291489 aiotubes-3.4/aiotubes.egg-info/
--rw-rw-rw-   0        0        0      697 2023-05-01 10:29:33.000000 aiotubes-3.4/aiotubes.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      381 2023-05-01 10:29:33.000000 aiotubes-3.4/aiotubes.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 10:29:33.000000 aiotubes-3.4/aiotubes.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-05-01 10:29:33.000000 aiotubes-3.4/aiotubes.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-01 10:29:33.000000 aiotubes-3.4/aiotubes.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-01 10:29:33.293481 aiotubes-3.4/setup.cfg
--rw-rw-rw-   0        0        0      666 2023-05-01 10:29:25.000000 aiotubes-3.4/setup.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 aiotubes-3.5/aiotube/__init__.py
+-rw-r--r--   0        0        0     2990 2020-02-02 00:00:00.000000 aiotubes-3.5/aiotube/client.py
+-rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 aiotubes-3.5/aiotube/constants.py
+-rw-r--r--   0        0        0     2511 2020-02-02 00:00:00.000000 aiotubes-3.5/aiotube/exceptions.py
+-rw-r--r--   0        0        0     5405 2020-02-02 00:00:00.000000 aiotubes-3.5/aiotube/extractors.py
+-rw-r--r--   0        0        0     2015 2020-02-02 00:00:00.000000 aiotubes-3.5/aiotube/helpers.py
+-rw-r--r--   0        0        0     4427 2020-02-02 00:00:00.000000 aiotubes-3.5/aiotube/itags.py
+-rw-r--r--   0        0        0     2226 2020-02-02 00:00:00.000000 aiotubes-3.5/aiotube/playlist.py
+-rw-r--r--   0        0        0     8162 2020-02-02 00:00:00.000000 aiotubes-3.5/aiotube/streams.py
+-rw-r--r--   0        0        0     4974 2020-02-02 00:00:00.000000 aiotubes-3.5/aiotube/video.py
+-rw-r--r--   0        0        0     1951 2020-02-02 00:00:00.000000 aiotubes-3.5/.gitignore
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 aiotubes-3.5/LICENSE
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 aiotubes-3.5/README.md
+-rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 aiotubes-3.5/pyproject.toml
+-rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 aiotubes-3.5/PKG-INFO
```

### Comparing `aiotubes-3.4/LICENSE` & `aiotubes-3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `aiotubes-3.4/PKG-INFO` & `aiotubes-3.5/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,32 +1,35 @@
-Metadata-Version: 2.1
-Name: aiotubes
-Version: 3.4
-Summary: Asynchronous Youtube API
-Home-page: https://github.com/sheldygg/aiotube
-Author: sheldy
-License: MIT
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# AIOTUBE
-
-**aiotube** Asynchronous YouTube API
-
-
-### Example
-
-```python
-import asyncio
-
-from aiotube import Video
-
-async def main():
-    client = Video("https://www.youtube.com/watch?v=MZ-cvXEvYI8")
-    stream = (await client.streams()).get_audio_only()
-    await stream.download_filepath(filename="yeat.mp3")
-    
-asyncio.run(main())
-
-```
+Metadata-Version: 2.1
+Name: aiotubes
+Version: 3.5
+Summary: Asynchronous Youtube API
+Project-URL: Homepage, https://github.com/sheldygg/aiotube
+Author: sheldy
+License-Expression: MIT
+License-File: LICENSE
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.10
+Requires-Dist: aiohttp
+Requires-Dist: pydantic
+Description-Content-Type: text/markdown
+
+# AIOTUBE
+
+**aiotube** Asynchronous YouTube API
+
+
+### Example
+
+```python
+import asyncio
+
+from aiotube import Video
+
+async def main():
+    client = Video("https://www.youtube.com/watch?v=MZ-cvXEvYI8")
+    stream = (await client.streams()).get_audio_only()
+    await stream.download_filepath(filename="yeat.mp3")
+    
+asyncio.run(main())
+
+```
```

### Comparing `aiotubes-3.4/aiotube/client.py` & `aiotubes-3.5/aiotube/client.py`

 * *Files identical despite different names*

### Comparing `aiotubes-3.4/aiotube/constants.py` & `aiotubes-3.5/aiotube/constants.py`

 * *Files identical despite different names*

### Comparing `aiotubes-3.4/aiotube/exceptions.py` & `aiotubes-3.5/aiotube/exceptions.py`

 * *Files identical despite different names*

### Comparing `aiotubes-3.4/aiotube/extractors.py` & `aiotubes-3.5/aiotube/extractors.py`

 * *Files identical despite different names*

### Comparing `aiotubes-3.4/aiotube/helpers.py` & `aiotubes-3.5/aiotube/helpers.py`

 * *Files identical despite different names*

### Comparing `aiotubes-3.4/aiotube/itags.py` & `aiotubes-3.5/aiotube/itags.py`

 * *Files identical despite different names*

### Comparing `aiotubes-3.4/aiotube/playlist.py` & `aiotubes-3.5/aiotube/playlist.py`

 * *Files identical despite different names*

### Comparing `aiotubes-3.4/aiotube/streams.py` & `aiotubes-3.5/aiotube/streams.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from .helpers import safe_filename, target_directory
 from .itags import get_format_profile
 
 
 class Stream(BaseModel):
     title: str
     author: str
+    request_client: RequestClient
     url: HttpUrl
     itag: int
     mimeType: str
     bitrate: int
     width: Optional[int]
     height: Optional[int]
     lastModifed: Optional[datetime]
@@ -29,14 +30,17 @@
     averageBitrate: Optional[int]
     audioQuality: Optional[str]
     approxDurationMs: str
     audioSampleRate: Optional[str]
     audioChannels: Optional[int]
     is_otf: bool
 
+    class Config:
+        arbitrary_types_allowed = True
+
     @property
     def itag_profile(self):
         return get_format_profile(self.itag)
 
     @property
     def abr(self):
         return self.itag_profile["abr"]
@@ -92,27 +96,25 @@
         """Whether the stream only contains video.
 
         :rtype: bool
         """
         return self.is_progressive or self.type == "video"
 
     async def filesize(self) -> int:
-        client = RequestClient("ANDROID")
-        response = await client.request(method=HttpMethod.HEAD, url=self.url)
+        response = await self.request_client.request(method=HttpMethod.HEAD, url=self.url)
         return int(response.get("headers", {}).get("Content-Length"))
 
     async def _download(self) -> AsyncGenerator[bytes, None]:
-        client = RequestClient("ANDROID")
         default_range_size = 9437184
         file_size: int = default_range_size
         downloaded = 0
         while downloaded < file_size:
             stop_pos = min(downloaded + default_range_size, file_size) - 1
             range_header = f"bytes={downloaded}-{stop_pos}"
-            request = await client.request(
+            request = await self.request_client.request(
                 method=HttpMethod.GET, url=self.url, headers={"Range": range_header}
             )
             headers = request.get("headers")
             chunk = request.get("response")
             if file_size == default_range_size:
                 content_range = headers.get("Content-Range")
                 file_size = int(content_range.split("/")[1])
```

### Comparing `aiotubes-3.4/aiotube/video.py` & `aiotubes-3.5/aiotube/video.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,15 @@
         if self._fmt_streams:
             return self._fmt_streams
         self._fmt_streams = []
         stream_manifest = apply_descrambler(await self.streaming_data())
         video_title = await self.title()
         video_author = await self.author()
         for stream in stream_manifest:
-            video = Stream(title=video_title, author=video_author, **stream)
+            video = Stream(title=video_title, author=video_author, request_client=self.client, **stream)
             self._fmt_streams.append(video)
         return self._fmt_streams
 
     async def streams(self):
         return StreamQuery(await self.fmt_streams())
 
     async def bypass_age_gate(self):
```

