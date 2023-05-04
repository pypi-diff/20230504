# Comparing `tmp/acltldr-0.1.0.tar.gz` & `tmp/acltldr-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acltldr-0.1.0.tar", max compression
+gzip compressed data, was "acltldr-0.1.1.tar", max compression
```

## Comparing `acltldr-0.1.0.tar` & `acltldr-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      522 2023-05-04 11:53:53.350322 acltldr-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-05-04 08:40:30.986017 acltldr-0.1.0/acltldr/__init__.py
--rw-r--r--   0        0        0     1871 2023-05-04 11:48:43.687192 acltldr-0.1.0/acltldr/main.py
--rw-r--r--   0        0        0      324 2023-05-04 11:48:40.790060 acltldr-0.1.0/acltldr/utils.py
--rw-r--r--   0        0        0      567 2023-05-04 11:50:46.658115 acltldr-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1354 1970-01-01 00:00:00.000000 acltldr-0.1.0/setup.py
--rw-r--r--   0        0        0     1116 1970-01-01 00:00:00.000000 acltldr-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      522 2023-05-04 11:53:53.350322 acltldr-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-05-04 08:40:30.986017 acltldr-0.1.1/acltldr/__init__.py
+-rw-r--r--   0        0        0     1857 2023-05-04 12:13:42.555175 acltldr-0.1.1/acltldr/main.py
+-rw-r--r--   0        0        0      324 2023-05-04 11:48:40.790060 acltldr-0.1.1/acltldr/utils.py
+-rw-r--r--   0        0        0      567 2023-05-04 12:13:47.282592 acltldr-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1354 1970-01-01 00:00:00.000000 acltldr-0.1.1/setup.py
+-rw-r--r--   0        0        0     1116 1970-01-01 00:00:00.000000 acltldr-0.1.1/PKG-INFO
```

### Comparing `acltldr-0.1.0/README.md` & `acltldr-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `acltldr-0.1.0/acltldr/main.py` & `acltldr-0.1.1/acltldr/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,14 @@
                 "title": _title,
                 "authors": _authors,
                 "abstract": _abst,
                 "tldr": model([_abst])[0] if isinstance(_abst, str) else "",
                 "url": _url,
             }
         )
-        break
 
     sienna.save(papers, os.path.join(odir, f"{prefix}.papers.jsonl"))
 
     md_items = papers_to_markdown_items(papers)
     with open(os.path.join(odir, f"{prefix}.papers.md"), "w") as f:
         f.write("\n".join(md_items))
```

### Comparing `acltldr-0.1.0/pyproject.toml` & `acltldr-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "acltldr"
-version = "0.1.0"
+version = "0.1.1"
 description = ""
 authors = ["sobamchan <oh.sore.sore.soutarou@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 sienna = "^0.2.2"
```

### Comparing `acltldr-0.1.0/setup.py` & `acltldr-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
  'tqdm>=4.65.0,<5.0.0']
 
 entry_points = \
 {'console_scripts': ['acltldr = acltldr.main:run']}
 
 setup_kwargs = {
     'name': 'acltldr',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': '',
     'long_description': '# ACLTLDR\n\nThis is a python-based CLI tool used to generate summaries for ACL conference papers on [this page](https://sotaro.io/tldrs).\n\n\n## Installation\n\n```\npip install acltldr\n```\n\n\n## Usage\n\nAn example command to generate summaries for the proceedings of EACL 2021.\nFollowing command will generate a jsonl file with all the data, and a markdown file for the post.\n\n```\nacltldr https://raw.githubusercontent.com/acl-org/acl-anthology/master/data/xml/2021.eacl.xml \\\n        ./ \\\n\t--prefix "2021.eacl" \\\n\t--use-gpu\n```\n',
     'author': 'sobamchan',
     'author_email': 'oh.sore.sore.soutarou@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `acltldr-0.1.0/PKG-INFO` & `acltldr-0.1.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acltldr
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: sobamchan
 Author-email: oh.sore.sore.soutarou@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

