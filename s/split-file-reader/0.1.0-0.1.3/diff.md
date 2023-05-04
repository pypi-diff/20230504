# Comparing `tmp/split_file_reader-0.1.0.tar.gz` & `tmp/split_file_reader-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\Xavier\PycharmProjects\SplitFileReaderProject\dist\tmpfd314_ah\split_file_reader-0.1.0.tar", last modified: Thu Jan 20 04:26:46 2022, max compression
+gzip compressed data, was "C:\Users\Xavier\PycharmProjects\SplitFileReaderProject\dist\.tmp-k06dp6dk\split_file_reader-0.1.3.tar", last modified: Thu May  4 01:03:52 2023, max compression
```

## Comparing `split_file_reader-0.1.0.tar` & `split_file_reader-0.1.3.tar`

### file list

```diff
@@ -1,28 +1,25 @@
-drwxrwxrwx   0        0        0        0 2022-01-20 04:26:46.000000 split_file_reader-0.1.0/
--rw-rw-rw-   0        0        0    35769 2022-01-16 22:31:16.000000 split_file_reader-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     9515 2022-01-20 04:26:46.000000 split_file_reader-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     8409 2022-01-19 02:25:49.000000 split_file_reader-0.1.0/README.md
--rw-rw-rw-   0        0        0       60 2022-01-14 02:10:58.000000 split_file_reader-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0      138 2022-01-20 04:26:46.000000 split_file_reader-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     2010 2022-01-20 04:13:06.000000 split_file_reader-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2022-01-20 04:26:46.000000 split_file_reader-0.1.0/split_file_reader/
--rw-rw-rw-   0        0        0     1093 2022-01-20 03:53:15.000000 split_file_reader-0.1.0/split_file_reader/__init__.py
--rw-rw-rw-   0        0        0       84 2021-04-24 18:38:31.000000 split_file_reader-0.1.0/split_file_reader/__main__.py
-drwxrwxrwx   0        0        0        0 2022-01-20 04:26:46.000000 split_file_reader-0.1.0/split_file_reader/http_file_reader/
--rw-rw-rw-   0        0        0       45 2021-04-21 01:34:03.000000 split_file_reader-0.1.0/split_file_reader/http_file_reader/__init__.py
--rw-rw-rw-   0        0        0     9983 2022-01-18 03:05:06.000000 split_file_reader-0.1.0/split_file_reader/http_file_reader/http_file_reader.py
-drwxrwxrwx   0        0        0        0 2022-01-20 04:26:46.000000 split_file_reader-0.1.0/split_file_reader/split_file_reader/
--rw-rw-rw-   0        0        0       47 2021-04-22 02:22:04.000000 split_file_reader-0.1.0/split_file_reader/split_file_reader/__init__.py
--rw-rw-rw-   0        0        0     4704 2022-01-18 02:56:32.000000 split_file_reader-0.1.0/split_file_reader/split_file_reader/__main__.py
--rw-rw-rw-   0        0        0    29573 2022-01-18 03:05:56.000000 split_file_reader-0.1.0/split_file_reader/split_file_reader/split_file_reader.py
-drwxrwxrwx   0        0        0        0 2022-01-20 04:26:46.000000 split_file_reader-0.1.0/split_file_reader/split_file_writer/
--rw-rw-rw-   0        0        0      128 2021-04-27 03:55:49.000000 split_file_reader-0.1.0/split_file_reader/split_file_writer/__init__.py
--rw-rw-rw-   0        0        0    11366 2022-01-18 03:48:12.000000 split_file_reader-0.1.0/split_file_reader/split_file_writer/split_file_writer.py
-drwxrwxrwx   0        0        0        0 2022-01-20 04:26:46.000000 split_file_reader-0.1.0/split_file_reader.egg-info/
--rw-rw-rw-   0        0        0     9515 2022-01-20 04:26:46.000000 split_file_reader-0.1.0/split_file_reader.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1115 2022-01-20 04:26:46.000000 split_file_reader-0.1.0/split_file_reader.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-01-20 04:26:46.000000 split_file_reader-0.1.0/split_file_reader.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       89 2022-01-20 04:26:46.000000 split_file_reader-0.1.0/split_file_reader.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       20 2022-01-20 04:26:46.000000 split_file_reader-0.1.0/split_file_reader.egg-info/requires.txt
--rw-rw-rw-   0        0        0      125 2022-01-20 04:26:46.000000 split_file_reader-0.1.0/split_file_reader.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2022-01-20 03:56:02.000000 split_file_reader-0.1.0/split_file_reader.egg-info/zip-safe
+drwxrwxrwx   0        0        0        0 2023-05-04 01:03:52.000000 split_file_reader-0.1.3/
+-rw-rw-rw-   0        0        0    35769 2022-01-16 22:31:16.000000 split_file_reader-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0      973 2023-05-04 01:03:52.000000 split_file_reader-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     9472 2023-05-01 03:05:10.000000 split_file_reader-0.1.3/README.md
+-rw-rw-rw-   0        0        0     1841 2023-04-30 03:19:06.000000 split_file_reader-0.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-04 01:03:52.000000 split_file_reader-0.1.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-04 01:03:52.000000 split_file_reader-0.1.3/src/
+-rw-rw-rw-   0        0        0     1095 2023-04-29 00:29:50.000000 split_file_reader-0.1.3/src/__init__.py
+-rw-rw-rw-   0        0        0       88 2022-06-26 03:47:31.000000 split_file_reader-0.1.3/src/__main__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 01:03:52.000000 split_file_reader-0.1.3/src/http_file_reader/
+-rw-rw-rw-   0        0        0       46 2022-06-26 03:47:31.000000 split_file_reader-0.1.3/src/http_file_reader/__init__.py
+-rw-rw-rw-   0        0        0    10366 2023-04-29 02:53:13.000000 split_file_reader-0.1.3/src/http_file_reader/http_file_reader.py
+drwxrwxrwx   0        0        0        0 2023-05-04 01:03:52.000000 split_file_reader-0.1.3/src/split_file_reader/
+-rw-rw-rw-   0        0        0       48 2023-04-28 21:33:13.000000 split_file_reader-0.1.3/src/split_file_reader/__init__.py
+-rw-rw-rw-   0        0        0     4584 2023-04-29 00:54:53.000000 split_file_reader-0.1.3/src/split_file_reader/__main__.py
+-rw-rw-rw-   0        0        0    30939 2023-04-29 02:51:32.000000 split_file_reader-0.1.3/src/split_file_reader/split_file_reader.py
+drwxrwxrwx   0        0        0        0 2023-05-04 01:03:52.000000 split_file_reader-0.1.3/src/split_file_reader.egg-info/
+-rw-rw-rw-   0        0        0      973 2023-05-04 01:03:52.000000 split_file_reader-0.1.3/src/split_file_reader.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      554 2023-05-04 01:03:52.000000 split_file_reader-0.1.3/src/split_file_reader.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 01:03:52.000000 split_file_reader-0.1.3/src/split_file_reader.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2023-05-04 01:03:52.000000 split_file_reader-0.1.3/src/split_file_reader.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       71 2023-05-04 01:03:52.000000 split_file_reader-0.1.3/src/split_file_reader.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-04 01:03:52.000000 split_file_reader-0.1.3/src/split_file_writer/
+-rw-rw-rw-   0        0        0       99 2023-04-29 00:29:50.000000 split_file_reader-0.1.3/src/split_file_writer/__init__.py
+-rw-rw-rw-   0        0        0    11399 2023-04-29 02:34:33.000000 split_file_reader-0.1.3/src/split_file_writer/split_file_writer.py
```

### Comparing `split_file_reader-0.1.0/LICENSE` & `split_file_reader-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `split_file_reader-0.1.0/PKG-INFO` & `split_file_reader-0.1.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,7 @@
-Metadata-Version: 2.1
-Name: split_file_reader
-Version: 0.1.0
-Summary: A package to read parted files on disk.
-Home-page: https://gitlab.com/Reivax/split_file_reader
-Author: Xavier Halloran
-Author-email: sfr@reivax.us
-License: UNKNOWN
-Project-URL: Source, https://gitlab.com/Reivax/split_file_reader
-Platform: any
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: System :: Filesystems
-Requires-Python: >=3.5
-Description-Content-Type: text/markdown
-Provides-Extra: network
-License-File: LICENSE
-
 ![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
 ![GitLab CI](https://img.shields.io/badge/GitLabCI-%23181717.svg?style=for-the-badge&logo=gitlab&logoColor=white)
 
 [![pipeline status](https://gitlab.com/Reivax/split_file_reader/badges/master/pipeline.svg)](https://gitlab.com/Reivax/split_file_reader/-/commits/master)
 [![coverage report](https://gitlab.com/Reivax/split_file_reader/badges/master/coverage.svg?job=pytest)](https://gitlab.com/Reivax/split_file_reader/-/commits/master)
 
 # SplitFileReader, SplitFileWriter, and HTTPFileReader
@@ -96,14 +69,41 @@
             for file in files:
                 if file.startswith("random_payload"):
                     zipf.write(os.path.join(root, file))
 ```
 
 Complex file names and mixed file objects are permitted via generators instead.
 
+
+#### Memory-only file-like operations
+Sometimes it behooves one to keep track of files strictly in memory, ensuring that the various file sizes remain managable.  This is a way to process each chunk after producing a large file.
+
+```python
+import zipfile
+from io import BytesIO
+from split_file_reader import SplitFileWriter
+chunks = []
+
+xml_file = """<xml>payload</xml>"""
+
+def gen(lst):
+    while True:
+        lst.append(BytesIO())
+        yield lst[-1]
+
+with SplitFileWriter(gen(chunks), 1_000_000) as sfw:
+    with zipfile.ZipFile(sfw, "w") as zip_file:
+        zip_file.writestr("test.xml", xml_file)
+
+for i, chunk in enumerate(chunks):
+    print(f'chunk {i}: {len(chunk.getvalue())}')
+```
+See [this stackoverflow question for a ](https://stackoverflow.com/questions/68983459/split-a-zip-file-into-chunks-with-python/68983810) for a specific example.
+
+  Alternatively, rather than keeping a list of every BytesIO object, after the yield one could manage that buffer on demand, such as by saving it to disk or sending it via HTTP.
 ## HTTPFileReader
 A python module to transparently read files that are hosted on a remote HTTP
 server.  Exposes the `readable`, `read`, `writable`, `write`, `tellable`, 
 `tell`, `seekable`, `seek`, `open` and `close` functions, as well as a Context
 Manager.
 
 This class is fast for skipping over large amounts of data and downloading only select parts.  It is inefficient for
@@ -209,9 +209,8 @@
 #### Examples
 To display the contents of the Zip files included in the test suite of this module, run
 ```bash
 python3 -m split_file_reader -azip --list ./files/archives/files.zip.*
 ```
 The bash autoexpansion of the `*` wildcard will fill in the files in order, correctly.  `--list` will print out the 
 names of the payload files within the zip archive, and the `-azip` flag instructs the module to expect the `Zip`
- archive type.
-
+ archive type.
```

### Comparing `split_file_reader-0.1.0/split_file_reader/__init__.py` & `split_file_reader-0.1.3/src/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,12 @@
 # -*- coding: utf-8 -*-
+import logging
+
+from .split_file_reader import SplitFileReader
+
 """
     A module for the manipulation of disparate data streams.
 """
 """
     split_file_reader
     Copyright (C) 2022  Xavier Halloran, United States
 
@@ -19,15 +23,12 @@
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """
 
 
 __version__ = "0.1.0"
 
-import logging
 
 # Squelch warnings about missing log handlers.
 logging.getLogger(__name__).addHandler(logging.NullHandler())
 
-from .split_file_reader import SplitFileReader
-
 __all__ = ["SplitFileReader"]
```

### Comparing `split_file_reader-0.1.0/split_file_reader/http_file_reader/http_file_reader.py` & `split_file_reader-0.1.3/src/http_file_reader/http_file_reader.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,20 +14,17 @@
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 """
 
+import io
 import logging
 import typing
-import io
-import json
-
-import requests
 
 logger = logging.getLogger(__name__)
 
 
 def trace(val, *args, **kwargs):
     logger.log(logging.DEBUG - 5, val, *args, **kwargs)
 
@@ -50,72 +47,79 @@
         with HTTPFileReader(url="https://gitlab.com/files.zip?inline=false", session=session) as hfr:
             with zipfile.ZipFile(file=hfr, mode="r") as zf:
 
     with requests.Session() as session:
         with HTTPFileReader(url="https://gitlab.com/files.tar?inline=false", session=session) as hfr:
             with tarfile.open(fileobj=hfr, mode="r") as tf:
 
+    with httpx.Client() as session:
+        with HTTPFileReader(url="https://gitlab.com/files.zip?inline=false", session=session) as hfr:
+            with zipfile.ZipFile(file=hfr, mode="r") as zf:
+
+    with httpx.Client() as session:
+        with HTTPFileReader(url="https://gitlab.com/files.tar?inline=false", session=session) as hfr:
+            with tarfile.open(fileobj=hfr, mode="r") as tf:
+
     `close` takes no real action.  The requests.Session is managed externally, and there is no file descriptor or
     buffer.
 
     Ranged queries return `206 Partial Content`.
     Invalid ranges return `416 Range Not Satisfiable`.
     If the service does not process Ranged data, it returns `200 OK` and presents the entire document.
     Dynamic values of the target file may not be supported.
     Dynamic values of the URL parameters or headers are not supported.
     github and gitlab both support Ranged queries for git project files.
 
     This class is not thread-safe; no method is idempotent, all of them affect the object state.  However, since the
     underlying files are all read-only, multiple concurrent instances of this class is allowed.
     """
 
-    def __init__(
+    def __init__(  # noqa:  PLR0913
         self,
         url: str,
-        session: typing.Optional[requests.Session],
+        session,
         mode: str = "rb",
         headers: typing.Optional[typing.Dict] = None,
         raise_for_status: bool = False,
     ) -> None:
         """
         Open an HTTP connection to a remote server, query the file size, and begin random-accessing it.  Ideal for TAR
         or ZIP files.
 
         The HTTP server must support "Range" header options, and reliable HEAD options.
 
         :param url: File target URL.
         :param mode: Must be "r"/"rb", kept only as a parameter to support libraries that expect to set it.
-        :param session: A user-supplied requests.Session object.
+        :param session: A user-supplied requests.Session or httpx.Client object.
         :param headers: Headers to accompany the HTTP traffic.  Not required, `Range` will be overwritten.
         :param raise_for_status: Call the `requests.response.raise_for_status` method to ensure safe HTTP response.
         """
 
-        if mode not in ["rb", "br", "r"]:
+        if mode not in {"rb", "br", "r"}:
             # On Unix, "r" and "rb" are the same.  On windows, "r" will alter line endings.
             raise ValueError("mode must be 'rb', was {}".format(mode))
         self.url: str = url
         # The user-supplied the session object
-        self._session: requests.Session = session
+        self._session = session
         # Possible user-supplied headers.
         self._headers: typing.Dict = headers or {}
         # Max file size, the EOF byte, according to the `Content-Length` in a HEAD request.
         self._size: int = 0
         # Value that `tell()` responds with.
         self._told: int = 0
 
         self.raise_for_status = raise_for_status
 
         res = self._session.head(self.url, headers=self._headers)
-        # print(json.dumps(dict(res.headers), indent='\t'))
         if self.raise_for_status:
             res.raise_for_status()
         try:
             self._size = int(res.headers.get("Content-Length"))
         except TypeError:
-            raise ValueError("URL failed to return a valid Content-Length: {}".format(self.url))
+            raise ValueError("URL failed to return a valid Content-Length: {}".format(self.url)) from TypeError
         debug("File target_size: {}".format(self._size))
 
     def readable(self) -> bool:
         return True
 
     def read(self, target_size: typing.Optional[int] = None) -> typing.AnyStr:
         """
@@ -137,15 +141,14 @@
             range_end = self._size
 
         headers = self._headers.copy()
         headers.update({"Range": "bytes={}-{}".format(range_start, range_end)})
         res = self._session.get(url=self.url, headers=headers)
         if self.raise_for_status:
             res.raise_for_status()
-        # print_xxd_dump(res.content)
         self._told += len(res.content)
         debug("Read {}, currently {}".format(len(res.content), self._told))
         return res.content
 
     def readinto(self, buffer: bytearray) -> typing.Optional[int]:
         """
         This is the copy/paste implementation of `io.FileIO.readinto()`
@@ -160,15 +163,15 @@
     def seekable(self) -> bool:
         return True
 
     def seek(self, offset: int, whence: int = 0) -> int:
         debug("Seeking {} Whence {}, currently {}".format(offset, whence, self._told))
         if whence == 0:
             self._told = 0
-        elif whence == 2:
+        elif whence == 2:  # noqa: PLR2004
             self._told = self._size
         self._told += offset
         # Can't seek off the end.  This will support SplitFilelikeReader and avoid weird HTTP errors.
         self._told = min(self._told, self._size)
         debug("Sought {} Whence {}, currently {}".format(offset, whence, self._told))
         return self._told
 
@@ -213,31 +216,31 @@
     This permits the HTTPFileReader to work within a context that expects the io.IOBase capabilities, such as a 
     TextIOWrapper
     """
 
     def writable(self) -> bool:
         return False
 
-    def write(self, b: typing.Union[bytes, bytearray]) -> typing.Optional[int]:
+    def write(self, b: typing.Union[bytes, bytearray]) -> typing.Optional[int]:  # noqa: ARG002
         """
         No writing allowed with this class.
         :param b:
         :return:
         """
         raise io.UnsupportedOperation("{} cannot write.".format(self.__class__.__name__))
 
-    def writelines(self, lines: typing.Iterable[typing.Union[bytes, bytearray]]) -> None:
+    def writelines(self, lines: typing.Iterable[typing.Union[bytes, bytearray]]) -> None:  # noqa: ARG002
         """
         No writing allowed with this class.
         :param lines:
         :return:
         """
         raise io.UnsupportedOperation("{} cannot write.".format(self.__class__.__name__))
 
-    def truncate(self, size: typing.Optional[int] = ...) -> int:
+    def truncate(self, size: typing.Optional[int] = ...) -> int:  # noqa: ARG002
         """
         No writing allowed with this class.
         :param size:
         :return:
         """
         raise io.UnsupportedOperation("{} cannot truncate.".format(self.__class__.__name__))
 
@@ -249,21 +252,21 @@
         return False
 
     def flush(self) -> None:
         """
         No writing allowed with this class.
         :return:
         """
-        pass
+        pass  # noqa: PIE790
 
     def fileno(self) -> int:
         raise IOError("No current file descriptor in use.")
 
-    def readline(self, size: int = ...) -> bytes:
+    def readline(self, size: int = ...) -> bytes:  # noqa: ARG002
         raise io.UnsupportedOperation(
             "{} cannot decode text, and therefore cannot readline.".format(self.__class__.__name__)
         )
 
-    def readlines(self, hint: int = ...) -> typing.List[bytes]:
+    def readlines(self, hint: int = ...) -> typing.List[bytes]:  # noqa: ARG002
         raise io.UnsupportedOperation(
             "{} cannot decode text, and therefore cannot readlines.".format(self.__class__.__name__)
         )
```

### Comparing `split_file_reader-0.1.0/split_file_reader/split_file_reader/__main__.py` & `split_file_reader-0.1.3/src/split_file_reader/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,20 +14,19 @@
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 """
 import os
-import typing
 import sys
+import typing
 
 from .split_file_reader import SplitFileReader
 
-
 long_description = """
 Identify and process parted archives without manual concat.
 This command line capability provides support only Tar and Zip files; but not 7z or Rar.
 Designed to work for files that have been split via the `split` utility, or any other binary cut;
 but does not support Zip's built-in split capability. 
 The python module supports any arbitrarily split files, regardless of type.
 Copyright (C) 2022  Xavier Haloran
@@ -63,26 +62,22 @@
     group.add_argument("-r", "--read", metavar="<filename>", help="Read out payload file contents to stdout.")
     parser.add_argument(
         "files",
         metavar="<filepath>",
         nargs="+",
         help="In-order list of the parted files on disk.  Use shell expansion, such as ./files.zip.*",
     )
-    if test_args:
-        args = parser.parse_args(test_args)
-    else:
-        args = parser.parse_args()
+    args = parser.parse_args(test_args) if test_args else parser.parse_args()
 
     sfr = SplitFileReader(args.files)
 
     if args.archive in ("zip", "z"):
         import zipfile
 
         with zipfile.ZipFile(sfr, mode="r") as zf:
-            zf: zipfile.ZipFile = zf
             if args.test:
                 zf.testzip()
             elif args.list:
                 for zff in zf.filelist:
                     print(zff.filename)
             elif args.read:
                 import shutil
@@ -98,15 +93,14 @@
 
         with tarfile.TarFile(fileobj=sfr, mode="r") as tf:
             if args.test:
                 tf.getmembers()
                 print(tf.getmembers(), file=sys.stderr)
             elif args.list:
                 for tff in tf:
-                    tff: tarfile.TarInfo = tff
                     print(tff.name)
             elif args.read:
                 import shutil
 
                 tff = tf.extractfile(args.read)
                 # Pytest swaps out the stdout for a StringIO, which has no buffer.
                 if "PYTEST_CURRENT_TEST" not in os.environ:
```

### Comparing `split_file_reader-0.1.0/split_file_reader/split_file_reader/split_file_reader.py` & `split_file_reader-0.1.3/src/split_file_reader/split_file_reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,18 +14,18 @@
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 """
 
+import io
 import logging
 import os
 import typing
-import io
 
 logger = logging.getLogger(__name__)
 
 
 def trace(val, *args, **kwargs):
     logger.log(logging.DEBUG - 5, val, *args, **kwargs)
 
@@ -36,15 +36,15 @@
 
 # The generator has a need to know file direction to set the pointer correctly.
 _BACKWARD = -1
 _STATIONARY = 0
 _FORWARD = 1
 
 
-class SplitFileReader(io.BytesIO):
+class SplitFileReader(io.RawIOBase):
     """
     Acts file-like for a list of files opened readably in binary mode.
     Provides `readable`, `writable`, `seekable`, `tellable`.
     Implements `read`, `readinto`, `seek`, `tell`
     Prohibits `write`, `writelines`, readline`, `readlines`, `truncate`
     Also implements `open`, `close`, `closed`, `__repr__`, `__iter__` and `__next__`., `__enter__`, and `__exit__`
 
@@ -70,15 +70,15 @@
     their own context managers.
 
     This class is not thread-safe; no method is idempotent, all of them affect the object state.  However, since the
     underlying files are all read-only, multiple concurrent instances of this class, attached to the same underlying
     files, is allowed.
     """
 
-    def __init__(
+    def __init__(  # noqa: PLR0913
         self,
         files: typing.List[typing.Union[str, os.PathLike, typing.Any]],
         mode: str = "rb",
         stream_only: bool = False,
         validate_all_readable: bool = False,
         iter_size: int = 1,
     ) -> None:
@@ -87,15 +87,15 @@
         on the first file in the list.
 
         `files` may be any of os.PathLike, a `str` or any `file-like` object available.  If it is a `str` or `PathLike`
         a new `open()` will be called with that value as a parameter in a context manager.  Otherwise, the file-like
         will have `seek`, `tell`, and `read` called on it directly.  Any mix of types is allowed in the list.
 
         :param files: List (or indexable collection) of filepaths or file-like objects for opening, reading, and closing
-        :param mode: Must be "r"/"rb", kept only as a parameter to support libraries that expect to set it.
+        :param mode: Must be "r"/"rb", kept only as a parameter to support libraries that explicitly set it.
         :param stream_only: Determines if Seek will work.  Will be set if iter() is called at any point.
         :param validate_all_readable: Seek over every component file, make sure they can all be read.  This is a
                 coherency check that all the files are adequately specified before being the read operations.
         :param iter_size: The size of the data returned by a next() call to this object.  This is typically 1, but may
                 be any positive integer.  A value of zero will read the entire file on the next call.
         """
         if mode not in ["rb", "br", "r"]:
@@ -130,15 +130,32 @@
         return True
 
     def readall(self) -> bytes:
         """
         Wraps `read(-1)`
         :return:
         """
-        return self._read(-1)
+        return self._read(-1, read_once=False)
+
+    def read1(self, size: typing.Optional[int] = None) -> typing.AnyStr:
+        """
+        Read the specified amount, making underlying file boundaries invisible to the caller.
+
+        If the current file pointer has been set to None, indicating an earlier call to `close()`, raises IOError.
+
+        May make multiple system calls, but will only make a single `read` system call in total.  May close and open
+        a file pointer and attempt a `seek`
+
+        :param size: Expected read size, or -1 or None to read to end.
+        :return: bytes-like list, between zero and `target_size` in length.
+        """
+        if size is None or size < 0:
+            return self._read(-1, read_once=True)
+        else:
+            return self._read(size, read_once=True)
 
     def read(self, size: typing.Optional[int] = None) -> typing.AnyStr:
         """
         Read the specified amount, making underlying file boundaries invisible to the caller.
 
         If the current file pointer has been set to None, indicating an earlier call to `close()`, raises IOError.
 
@@ -148,15 +165,15 @@
         :return: bytes-like list, between zero and `target_size` in length.
         """
         if size is None or size < 0:
             return self.readall()
         else:
             return self._read(size)
 
-    def _read(self, target_size: int):
+    def _read(self, target_size: int, read_once=False):
         """
         TODO: Make read() call readinto(), instead of the other way around, to support memory-optimized operations.
 
         :param target_size: Expected read size, or -1 to read to end.
         :return: bytes-like list, between zero and `target_size` in length.
         """
         debug("Reading {}, currently {}".format(target_size, self._told))
@@ -169,14 +186,17 @@
             remaining = target_size - len(ret)
             # Reads less than the total size are indicative that the end of a file has been reached, and the next one
             # should be cycled in.
             while remaining > 0:
                 if not self._safe_advance_file_desc(_FORWARD):
                     # More requested to be read, but there are no more files to open.
                     break
+                if read_once:
+                    # read1 calls only do a single filestream read, but file pointers still need to advance.
+                    break
                 read = self._current_file_desc.read(remaining)
                 remaining -= len(read)
                 ret += read
             self._told += len(ret)
         else:
             # Read -1/None behaves differently.
             ret = self._current_file_desc.read(target_size)
@@ -189,23 +209,34 @@
 
     def readinto(self, buffer: bytearray) -> typing.Optional[int]:
         """
         This is the copy/paste implementation of `io.FileIO.readinto()`
         :param buffer:
         :return:
         """
-        data = self.read(len(buffer))
+        data = self._read(len(buffer), read_once=False)
+        n = len(data)
+        buffer[:n] = data
+        return n
+
+    def readinto1(self, buffer: bytearray) -> typing.Optional[int]:
+        """
+        This is the copy/paste implementation of `io.FileIO.readinto()`
+        :param buffer:
+        :return:
+        """
+        data = self._read(len(buffer), read_once=True)
         n = len(data)
         buffer[:n] = data
         return n
 
     def seekable(self) -> bool:
         return not self._stream_only
 
-    def seek(self, offset: int, whence: int = 0) -> int:
+    def seek(self, offset: int, whence: int = 0) -> int:  # noqa: PLR0912
         """
         Move the file pointer along a file.  May advance over zero or more actual files.
 
         POSIX allows to seek before or after the end of a file, even in read-only mode.  `seek()` before the start of
         the first file will fail; `seek()` beyond the end of the last file is fine.
 
         If the current file pointer has been set to None, indicating an earlier call to `close()`, raises IOError.
@@ -257,15 +288,15 @@
             if how_far_to_go == 0:
                 trace("Nowhere to go.")
             elif how_far_to_go > 0:
                 self._scan_forward(how_far_to_go)
             elif how_far_to_go < 0:
                 self._scan_backward(how_far_to_go)
 
-        elif whence == 2:
+        elif whence == 2:  # noqa: PLR2004
             # From the end.
             how_far_to_go = offset
             trace("How far to go: {}".format(how_far_to_go))
             # Without a-priori knowledge of the total file sizes, we can't really calculate the offset to go.
             # So, zip all thw way to the end, then navigate as appropriate.
             self._seek_to_tail()
             if how_far_to_go == 0:
@@ -378,15 +409,14 @@
 
         This may be slow if the disk is slow.
 
         This process could be accelerated by doing a one-time pass and counting the file sizes directly, but this may
         not be desirable.  In practice, `seek(x, 2)` is rare, used by ZipFile, and even then, just at the start.
         :return: Nothing
         """
-        # self._seek_to_head()
         trace("Start of seek to tail.  Tell: {}".format(self._told))
         while True:
             trace("Current IDX: {}".format(self._current_file_desc_idx))
             # Save starting position, might not be zero.
             start = self._current_file_desc.tell()
             # The generator for advancing file descriptors will ensure the pointer is at the start of the file part.
             # Go to the end.
@@ -501,14 +531,16 @@
     def tell(self) -> int:
         """
         Logically identical to tell() on any other file-like object.
 
         Returns the offset as a sum of all previous file sizes, plus current file tell()
         :return:
         """
+        if self.closed:
+            raise ValueError("tell on a closed file")
         return self._told
 
     @classmethod
     def open(cls, *args, **kwargs):
         """
         Wraps the init constructor.
 
@@ -596,31 +628,31 @@
     This permits the SplitFileReader to work within a context that expects the io.IOBase capabilities, such as a 
     TextIOWrapper
     """
 
     def writable(self) -> bool:
         return False
 
-    def write(self, b: typing.Union[bytes, bytearray]) -> typing.Optional[int]:
+    def write(self, b: typing.Union[bytes, bytearray]) -> typing.Optional[int]:  # noqa: ARG002
         """
         No writing allowed with this class.
         :param b:
         :return:
         """
         raise io.UnsupportedOperation("{} cannot write.".format(self.__class__.__name__))
 
-    def writelines(self, lines: typing.Iterable[typing.Union[bytes, bytearray]]) -> None:
+    def writelines(self, lines: typing.Iterable[typing.Union[bytes, bytearray]]) -> None:  # noqa: ARG002
         """
         No writing allowed with this class.
         :param lines:
         :return:
         """
         raise io.UnsupportedOperation("{} cannot write.".format(self.__class__.__name__))
 
-    def truncate(self, size: typing.Optional[int] = ...) -> int:
+    def truncate(self, size: typing.Optional[int] = ...) -> int:  # noqa: ARG002
         """
         No writing allowed with this class.
         :param size:
         :return:
         """
         raise io.UnsupportedOperation("{} cannot truncate.".format(self.__class__.__name__))
 
@@ -632,28 +664,21 @@
         return False
 
     def flush(self) -> None:
         """
         No writing allowed with this class.
         :return:
         """
-        pass
 
     def fileno(self) -> int:
         """
-        Pass-through to the underlying file descriptor.  May not have any consistent meaning after any read or seek
+        It is usually used by os.stat to get a filesize, which is meaningless here.
         actions.
         :return:
         """
-        if self._current_file_desc:
-            return self._current_file_desc.fileno()
-        raise IOError("No current file descriptor in use.")
-
-    def readline(self, size: int = ...) -> bytes:
-        raise io.UnsupportedOperation(
-            "{} cannot decode text, and therefore cannot readline.".format(self.__class__.__name__)
-        )
+        raise io.UnsupportedOperation("{} should not return a fileno".format(self.__class__.__name__))
 
-    def readlines(self, hint: int = ...) -> typing.List[bytes]:
-        raise io.UnsupportedOperation(
-            "{} cannot decode text, and therefore cannot readlines.".format(self.__class__.__name__)
-        )
+    def readline(self, size: int = ...) -> bytes:  # noqa: ARG002
+        raise io.UnsupportedOperation("{} cannot decode text; use io.TextIOWrapper.".format(self.__class__.__name__))
+
+    def readlines(self, hint: int = ...) -> typing.List[bytes]:  # noqa: ARG002
+        raise io.UnsupportedOperation("{} cannot decode text; use io.TextIOWrapper.".format(self.__class__.__name__))
```

### Comparing `split_file_reader-0.1.0/split_file_reader/split_file_writer/split_file_writer.py` & `split_file_reader-0.1.3/src/split_file_writer/split_file_writer.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,18 +13,18 @@
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 """
-from abc import ABC, abstractmethod
 import io
 import os
 import typing
+from abc import ABC, abstractmethod
 
 
 class IndexableObject(ABC):  # pragma: no cover
     """
     This class exists strictly for the type hint.  Anything that can have `len()` called on it, and `[]` slicing applied
     to it is acceptable.
 
@@ -83,16 +83,16 @@
 
         :param filenames: A str, PathLike, a list of str or PathLike, or a generator to produce file-like objects.
         :param max_part_size: Max size in bytes for each file chunk; must be a positive integer.
         """
         # Is this output stream closed?  (has `close()` been called on this object?)
         self._closed: bool = False
         # The max file size for a given output part before requesting a new one.
-        assert isinstance(max_part_size, int)
-        assert max_part_size > 0
+        if not isinstance(max_part_size, int) and max_part_size <= 0:
+            raise ValueError("max_part_size must be a positive integer.")
         self._max_part_size: int = max_part_size
 
         # Stored copy of the generator used to open new files.
         # No matter what is passed as an argument, convert it to a generator.
         if isinstance(filenames, os.PathLike):
             filenames = os.fspath(filenames)
         if filenames is None:
@@ -154,19 +154,18 @@
         :return:  Whatever the file pointer flush value is.  Usually, None.
         """
         return self._file_ptr.flush()
 
     def __write_generator(self) -> typing.Generator[None, IndexableObject, None]:
         chunk = None
 
-        # file_gen_iter = iter(self._file_gen)
         # while True:
-        for self._file_ptr in iter(self._file_gen):
+        for fp in iter(self._file_gen):
+            self._file_ptr = fp
             part_wrote = 0
-            # self._file_ptr = next(file_gen_iter)
             while True:
                 if not chunk:
                     chunk = yield
                 available = self._max_part_size - part_wrote
                 size = self._file_ptr.write(chunk[:available])
                 part_wrote += size
                 self._told += size
@@ -185,24 +184,24 @@
 
     def tell(self) -> int:
         return self._told
 
     def seekable(self) -> bool:
         return False
 
-    def seek(self, offset: typing.Optional[int] = ..., whence: typing.Optional[int] = ...) -> int:
+    def seek(self, offset: typing.Optional[int] = ..., whence: typing.Optional[int] = ...) -> int:  # noqa: ARG002
         raise io.UnsupportedOperation("{} cannot seek.".format(self.__class__.__name__))
 
     def readable(self) -> bool:
         return False
 
-    def read(self, size: typing.Optional[int] = ...):
+    def read(self, size: typing.Optional[int] = ...):  # noqa: ARG002
         raise io.UnsupportedOperation("{} cannot read.".format(self.__class__.__name__))
 
-    def truncate(self, size: typing.Optional[int] = ...):
+    def truncate(self, size: typing.Optional[int] = ...):  # noqa: ARG002
         raise io.UnsupportedOperation("{} cannot truncate.".format(self.__class__.__name__))
 
     def fileno(self) -> int:
         if self._file_ptr:
             return self._file_ptr.fileno()
         raise IOError("No current file descriptor in use.")
 
@@ -221,15 +220,14 @@
     :param filename:  `path/to/file.bin.`  Include the trailing dot if desired.
     :param start_from:  Numeric index to start from.
     :param width:  Minimum number of numeric digits to append.
     :return:
     """
     idx = start_from
     formatter = "{{}}{{:0{:d}d}}".format(width)
-    # "{}{:03d}"
     while True:
         name = formatter.format(filename, idx)
         with open(name, mode="wb") as file_ptr:
             yield file_ptr
         idx += 1
 
 
@@ -238,15 +236,15 @@
     For a list of filepaths, open a file pointer for writing.
 
     :param list_of_filenames: A list of str or os.PathLink objects that will be passed to `builtins.open()`
     :return:
     """
     for filename in list_of_filenames:
         if isinstance(filename, os.PathLike):
-            filename = os.fspath(filename)
+            filename = os.fspath(filename)  # noqa: PLW2901
         with open(file=filename, mode="wb") as file_ptr:
             yield file_ptr
 
 
 def splitlike_file_generator(prefix="x", addl_suffix="") -> typing.Generator:
     """
     `split` default names are weird but alphabetical.  Add the filepath to the prefix to write specific places.
```

