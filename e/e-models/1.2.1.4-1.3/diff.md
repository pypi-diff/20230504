# Comparing `tmp/e-models-1.2.1.4.tar.gz` & `tmp/e-models-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "e-models-1.2.1.4.tar", last modified: Wed May  3 16:31:14 2023, max compression
+gzip compressed data, was "e-models-1.3.tar", last modified: Thu May  4 18:52:44 2023, max compression
```

## Comparing `e-models-1.2.1.4.tar` & `e-models-1.3.tar`

### file list

```diff
@@ -1,30 +1,27 @@
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-05-03 16:31:14.878850 e-models-1.2.1.4/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     1501 2023-03-30 21:13:00.000000 e-models-1.2.1.4/LICENSE
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     3272 2023-05-03 16:31:14.878850 e-models-1.2.1.4/PKG-INFO
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     2730 2023-04-19 14:03:12.000000 e-models-1.2.1.4/README.md
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-05-03 16:31:14.874850 e-models-1.2.1.4/e_models.egg-info/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     3272 2023-05-03 16:31:14.000000 e-models-1.2.1.4/e_models.egg-info/PKG-INFO
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      527 2023-05-03 16:31:14.000000 e-models-1.2.1.4/e_models.egg-info/SOURCES.txt
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        1 2023-05-03 16:31:14.000000 e-models-1.2.1.4/e_models.egg-info/dependency_links.txt
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       37 2023-05-03 16:31:14.000000 e-models-1.2.1.4/e_models.egg-info/requires.txt
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        8 2023-05-03 16:31:14.000000 e-models-1.2.1.4/e_models.egg-info/top_level.txt
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-05-03 16:31:14.874850 e-models-1.2.1.4/emodels/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       24 2023-05-03 16:30:41.000000 e-models-1.2.1.4/emodels/__init__.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      319 2023-04-02 14:00:26.000000 e-models-1.2.1.4/emodels/config.py
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-05-03 16:31:14.874850 e-models-1.2.1.4/emodels/html2text/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    34895 2023-05-03 16:22:16.000000 e-models-1.2.1.4/emodels/html2text/__init__.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     3873 2023-05-03 16:22:42.000000 e-models-1.2.1.4/emodels/html2text/config.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      423 2023-04-01 19:52:48.000000 e-models-1.2.1.4/emodels/html2text/elements.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       71 2023-04-01 19:52:48.000000 e-models-1.2.1.4/emodels/html2text/typing.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     8034 2023-04-01 19:58:24.000000 e-models-1.2.1.4/emodels/html2text/utils.py
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-05-03 16:31:14.874850 e-models-1.2.1.4/emodels/markdown/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        0 2023-05-02 18:53:53.000000 e-models-1.2.1.4/emodels/markdown/__init__.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     8316 2023-05-03 15:09:49.000000 e-models-1.2.1.4/emodels/markdown/tables.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        0 2023-03-30 21:13:53.000000 e-models-1.2.1.4/emodels/py.typed
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     7223 2023-05-03 15:32:59.000000 e-models-1.2.1.4/emodels/scrapyutils.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       31 2023-03-30 21:32:48.000000 e-models-1.2.1.4/pyproject.toml
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       38 2023-05-03 16:31:14.878850 e-models-1.2.1.4/setup.cfg
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      961 2023-05-03 16:30:30.000000 e-models-1.2.1.4/setup.py
-drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-05-03 16:31:14.878850 e-models-1.2.1.4/tests/
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     4419 2023-05-03 16:29:33.000000 e-models-1.2.1.4/tests/test_html2text.py
--rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     7947 2023-05-02 16:31:36.000000 e-models-1.2.1.4/tests/test_scrapyutils.py
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-05-04 18:52:44.296329 e-models-1.3/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     1501 2023-03-30 21:13:00.000000 e-models-1.3/LICENSE
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     3268 2023-05-04 18:52:44.296329 e-models-1.3/PKG-INFO
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     2730 2023-04-19 14:03:12.000000 e-models-1.3/README.md
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-05-04 18:52:44.292329 e-models-1.3/e_models.egg-info/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     3268 2023-05-04 18:52:44.000000 e-models-1.3/e_models.egg-info/PKG-INFO
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      471 2023-05-04 18:52:44.000000 e-models-1.3/e_models.egg-info/SOURCES.txt
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        1 2023-05-04 18:52:44.000000 e-models-1.3/e_models.egg-info/dependency_links.txt
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        7 2023-05-04 18:52:44.000000 e-models-1.3/e_models.egg-info/requires.txt
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        8 2023-05-04 18:52:44.000000 e-models-1.3/e_models.egg-info/top_level.txt
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-05-04 18:52:44.292329 e-models-1.3/emodels/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       20 2023-05-04 18:51:26.000000 e-models-1.3/emodels/__init__.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      319 2023-05-04 18:51:26.000000 e-models-1.3/emodels/config.py
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-05-04 18:52:44.292329 e-models-1.3/emodels/html2text/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)    34895 2023-05-04 18:51:26.000000 e-models-1.3/emodels/html2text/__init__.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     3873 2023-05-04 18:51:26.000000 e-models-1.3/emodels/html2text/config.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      423 2023-05-04 18:51:26.000000 e-models-1.3/emodels/html2text/elements.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       71 2023-05-04 18:51:26.000000 e-models-1.3/emodels/html2text/typing.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     8034 2023-05-04 18:51:26.000000 e-models-1.3/emodels/html2text/utils.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)        0 2023-05-04 18:51:26.000000 e-models-1.3/emodels/py.typed
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     6495 2023-05-04 18:51:26.000000 e-models-1.3/emodels/scrapyutils.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       31 2023-03-30 21:32:48.000000 e-models-1.3/pyproject.toml
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)       38 2023-05-04 18:52:44.296329 e-models-1.3/setup.cfg
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)      905 2023-05-04 18:50:17.000000 e-models-1.3/setup.py
+drwxrwxr-x   0 molveyra  (1001) molveyra  (1001)        0 2023-05-04 18:52:44.296329 e-models-1.3/tests/
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     3181 2023-05-04 18:49:39.000000 e-models-1.3/tests/test_html2text.py
+-rw-rw-r--   0 molveyra  (1001) molveyra  (1001)     7435 2023-05-04 18:49:39.000000 e-models-1.3/tests/test_scrapyutils.py
```

### Comparing `e-models-1.2.1.4/LICENSE` & `e-models-1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `e-models-1.2.1.4/PKG-INFO` & `e-models-1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: e-models
-Version: 1.2.1.4
+Version: 1.3
 Summary: Tools for helping build of extraction models with scrapy spiders.
 Home-page: https://github.com/kalessin/emodels
 Author: Martin Olveyra
 Author-email: molveyra@gmail.com
 License: BSD
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `e-models-1.2.1.4/README.md` & `e-models-1.3/README.md`

 * *Files identical despite different names*

### Comparing `e-models-1.2.1.4/e_models.egg-info/PKG-INFO` & `e-models-1.3/e_models.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: e-models
-Version: 1.2.1.4
+Version: 1.3
 Summary: Tools for helping build of extraction models with scrapy spiders.
 Home-page: https://github.com/kalessin/emodels
 Author: Martin Olveyra
 Author-email: molveyra@gmail.com
 License: BSD
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `e-models-1.2.1.4/emodels/html2text/__init__.py` & `e-models-1.3/emodels/html2text/__init__.py`

 * *Files identical despite different names*

### Comparing `e-models-1.2.1.4/emodels/html2text/config.py` & `e-models-1.3/emodels/html2text/config.py`

 * *Files identical despite different names*

### Comparing `e-models-1.2.1.4/emodels/html2text/utils.py` & `e-models-1.3/emodels/html2text/utils.py`

 * *Files identical despite different names*

### Comparing `e-models-1.2.1.4/emodels/scrapyutils.py` & `e-models-1.3/emodels/scrapyutils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 import re
 import os
 import json
 import gzip
 from typing import NewType, Dict, Tuple, List, Optional
 
-from markdown import Markdown
 from scrapy.loader import ItemLoader
 from scrapy.http import TextResponse
 from scrapy import Item
 
 from emodels.config import EMODELS_ITEMS_DIR, EMODELS_SAVE_EXTRACT_ITEMS
-from emodels.markdown.tables import TableExtension
 from emodels import html2text
 
 
 MARKDOWN_LINK_RE = re.compile(r"\[(.+?)\]\((.+?)\s*(\".+\")?\)")
 LINK_RSTRIP_RE = re.compile("(%20)+$")
 LINK_LSTRIP_RE = re.compile("^(%20)+")
 COMMENT_RE = re.compile(r"\s<!--.+?-->")
@@ -61,18 +59,14 @@
         """Generate multiple responses from provided xpath selector"""
         result = []
         for html in self.xpath(selector).extract():
             new = self.replace(body=html.encode("utf-8"))
             result.append(new)
         return result
 
-    def markdown_to_html(self, text: Optional[str] = None):
-        text = text or self.markdown
-        return Markdown(extensions=[TableExtension()]).convert(text).strip()
-
     @staticmethod
     def _clean_markdown(md: str):
         shrink = 0
         for m in MARKDOWN_LINK_RE.finditer(md):
             if m.groups()[1] is not None:
                 start = m.start(2) - shrink
                 end = m.end(2) - shrink
@@ -170,23 +164,14 @@
         )
         if extracted:
             t, s, e = extracted[0]
             if attr not in self.extract_indexes:
                 self.extract_indexes[attr] = (s, e)
                 self.add_value(attr, t, *processors, **kw)
 
-    def add_text_re_as_html(self, attr: str, reg: str, flags: int = 0, *processors, **kw):
-        extracted = self.context["response"].text_re(reg, flags=flags, optimize=True)
-        if extracted:
-            t, s, e = extracted[0]
-            if attr not in self.extract_indexes:
-                cleaned = self.context["response"].markdown_to_html(t)
-                self.add_value(attr, cleaned, *processors, **kw)
-                self.extract_indexes[attr] = (s, e)
-
     def load_item(self) -> Item:
         item = super().load_item()
         self._save_extract_sample()
         return item
 
     def _save_extract_sample(self):
         if EMODELS_SAVE_EXTRACT_ITEMS and self.extract_indexes:
```

### Comparing `e-models-1.2.1.4/setup.py` & `e-models-1.3/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 # Automatically created by: shub deploy
 
 from setuptools import setup, find_packages
 
 setup(
     name         = 'e-models',
-    version      = '1.2.1.4',
+    version      = '1.3',
     description  = 'Tools for helping build of extraction models with scrapy spiders.',
     long_description = open('README.md').read(),
     long_description_content_type = 'text/markdown',
     license      = 'BSD',
     author       = 'Martin Olveyra',
     author_email = 'molveyra@gmail.com',
     url          = 'https://github.com/kalessin/emodels',
     packages     = find_packages(),
     install_requires=(
         "scrapy",
-        "markdown",
-        "markdown-grid-tables",
     ),
     scripts = [],
     classifiers = [
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: BSD License',
         'Operating System :: OS Independent',
```

### Comparing `e-models-1.2.1.4/tests/test_html2text.py` & `e-models-1.3/tests/test_html2text.py`

 * *Files 26% similar despite different names*

```diff
@@ -19,19 +19,14 @@
 this is a line with id <!--#pid1-->
 
 this is another line with id <!--#pid2-->
 """
 
         self.assertEqual(response.markdown_ids, expected)
 
-        expected_html = """<p>this is a line</p>
-<p>this is a line with id</p>
-<p>this is another line with id</p>"""
-        self.assertEqual(response.markdown_to_html(), expected_html)
-
     def test_classes(self):
         html = b"""
 <div id="did">
 <p>this is a line</p>
 <p class="pc1">this is a line with class</p>
 <p id="pid2">this is a line with id</p>
 </div>
@@ -42,19 +37,14 @@
 this is a line with class <!--.pc1-->
 
 this is a line with id
 """
 
         self.assertEqual(response.markdown_classes, expected)
 
-        expected_html = """<p>this is a line</p>
-<p>this is a line with class</p>
-<p>this is a line with id</p>"""
-        self.assertEqual(response.markdown_to_html(), expected_html)
-
     def test_tables_plain(self):
         html = b"""
 <table><tr><td>Data 1</td><td>Data 2</td></tr>
 <tr><td>Data 3</td><td>Data 4</td></tr>
 <tr><td>Data 5</td><td>Data 6</td></tr>
 </table>
 """
@@ -62,32 +52,14 @@
         response = ExtractTextResponse(url="http://example.com/example2.html", status=200, body=html)
         expected = """| Data 1| Data 2|
 | Data 3| Data 4|
 | Data 5| Data 6|
 """
         self.assertEqual(response.markdown, expected)
 
-        expected_html = """<table>
-<tbody>
-<tr>
-<td>Data 1</td>
-<td>Data 2</td>
-</tr>
-<tr>
-<td>Data 3</td>
-<td>Data 4</td>
-</tr>
-<tr>
-<td>Data 5</td>
-<td>Data 6</td>
-</tr>
-</tbody>
-</table>"""
-        self.assertEqual(response.markdown_to_html(), expected_html)
-
     def test_tables_with_header(self):
         html = b"""
 <table><tr><th>Head 1</th><th>Head 2</th></tr>
 <tr><td>Data 1</td><td>Data 2</td></tr>
 <tr><td>Data 3</td><td>Data 4</td></tr>
 </table>
 
@@ -97,34 +69,14 @@
         expected = """| Head 1| Head 2|
 | ---|---|
 | Data 1| Data 2|
 | Data 3| Data 4|
 """
         self.assertEqual(response.markdown, expected)
 
-        expected_html = """<table>
-<thead>
-<tr>
-<th>Head 1</th>
-<th>Head 2</th>
-</tr>
-</thead>
-<tbody>
-<tr>
-<td>Data 1</td>
-<td>Data 2</td>
-</tr>
-<tr>
-<td>Data 3</td>
-<td>Data 4</td>
-</tr>
-</tbody>
-</table>"""
-        self.assertEqual(response.markdown_to_html(), expected_html)
-
     def test_tables_with_br_line_breaks(self):
         html = b"""
 <table><tr><td>Data 1</td><td>Data 2</td></tr>
 <tr><td>Data 3</td><td>Data 4</td></tr>
 <tr><td>Data 5</td><td><p>Data 6</p></td></tr>
 <tr><td>Data 7</td><td>Data 8</td></tr>
 </table>
@@ -136,36 +88,14 @@
 | Data 3| Data 4|
 | Data 5| <br><br>Data 6<br><br>|
 | Data 7| Data 8|
 """
         self.assertEqual(response.markdown, expected)
         html2text.config.LINE_BREAK_WITHIN_TABLE = saved
 
-        expected_html = """<table>
-<tbody>
-<tr>
-<td>Data 1</td>
-<td>Data 2</td>
-</tr>
-<tr>
-<td>Data 3</td>
-<td>Data 4</td>
-</tr>
-<tr>
-<td>Data 5</td>
-<td><br><br>Data 6<br><br></td>
-</tr>
-<tr>
-<td>Data 7</td>
-<td>Data 8</td>
-</tr>
-</tbody>
-</table>"""
-        self.assertEqual(response.markdown_to_html(), expected_html)
-
     def test_tables_with_line_breaks_default(self):
         html = b"""
 <table><tr><td>Data 1</td><td>Data 2</td></tr>
 <tr><td>Data 3</td><td>Data 4</td></tr>
 <tr><td>Data 5</td><td><p>Data 6</p></td></tr>
 <tr><td>Data 7</td><td>Data 8</td></tr>
 </table>
```

### Comparing `e-models-1.2.1.4/tests/test_scrapyutils.py` & `e-models-1.3/tests/test_scrapyutils.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 
 SAMPLES_DIR = os.path.join(os.path.dirname(__file__), "samples")
 
 
 class JobItem(Item):
     job_title = Field()
     description = Field()
-    description_as_html = Field()
     url = Field()
     employment_type = Field()
     apply_url = Field()
     job_id = Field()
     publication_date = Field()
     category = Field()
     closing_date = Field()
@@ -74,39 +73,32 @@
         body = open(sample_file).read().encode("utf8")
         tresponse = TextResponse(url="https://careers.und.edu/jobs/job21.html", body=body, status=200)
         loader = JobItemLoader(response=tresponse)
         loader.add_text_re("job_title", tid="#job_title_2_2")
         loader.add_text_re("employment_type", tid="#employment_type_2_2_0_0")
         loader.add_text_re("job_id", tid="#requisition_identifier_2_2_0")
         loader.add_text_re("description", r"(###\s+.+?)\*\*apply now\*\*", flags=re.S | re.I)
-        loader.add_text_re_as_html("description_as_html", r"(###\s+.+?)\*\*apply now\*\*", flags=re.S | re.I)
 
         item = loader.load_item()
 
+        response = loader.context["response"]
+
         self.assertFalse(COMMENT_RE.findall(item["description"]))
-        self.assertFalse(COMMENT_RE.findall(item["description_as_html"]))
+        self.assertEqual(COMMENT_RE.sub("", response.markdown_ids), response.markdown)
+        self.assertEqual(COMMENT_RE.sub("", response.markdown_classes), response.markdown)
 
         self.assertEqual(
             item["description"][:80],
             "###  Student Athlete Support Services Coord \n\n  * __ 492556 \n\n\n\n  * __ Grand For",
         )
         self.assertEqual(
             item["description"][-80:],
             "arning skills.\n\n\n\n**Please note, all employment postings close at 11:55pm CST.**",
         )
-        self.assertEqual(
-            item["description_as_html"][:80],
-            "<h3>Student Athlete Support Services Coord</h3>\n<ul>\n<li>\n<p>__ 492556 </p>\n</li",
-        )
-        self.assertEqual(
-            item["description_as_html"][-80:],
-            "><strong>Please note, all employment postings close at 11:55pm CST.</strong></p>",
-        )
 
-        response = loader.context["response"]
         self.assertEqual(
             response.markdown[slice(*loader.extract_indexes["job_title"])], "Student Athlete Support Services Coord"
         )
         self.assertEqual(response.markdown[slice(*loader.extract_indexes["job_id"])], "492556")
         self.assertEqual(response.markdown[slice(*loader.extract_indexes["employment_type"])], "Full-time Staff")
 
         with gzip.open(self.jobs_result_file, "rt") as fz:
@@ -117,15 +109,14 @@
         self.assertEqual(
             data["markdown"][slice(*data["indexes"]["job_title"])], "Student Athlete Support Services Coord"
         )
         self.assertEqual(data["markdown"][slice(*data["indexes"]["job_id"])], "492556")
         self.assertEqual(data["markdown"][slice(*data["indexes"]["employment_type"])], "Full-time Staff")
 
         self.assertEqual(data["markdown"][slice(*data["indexes"]["description"])], item["description"])
-        self.assertEqual(data["markdown"][slice(*data["indexes"]["description_as_html"])], item["description"])
 
         self.assertTrue(response.text_re(tid=".job-field job-title"))
 
     def test_example_two(self):
         sample_file = os.path.join(SAMPLES_DIR, "yell.html")
         body = open(sample_file).read().encode("utf8")
         response = ExtractTextResponse(url="https://yell.com/result.html", body=body, status=200)
```

