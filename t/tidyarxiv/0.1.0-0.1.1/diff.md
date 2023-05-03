# Comparing `tmp/tidyarxiv-0.1.0.tar.gz` & `tmp/tidyarxiv-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tidyarxiv-0.1.0.tar", max compression
+gzip compressed data, was "tidyarxiv-0.1.1.tar", max compression
```

## Comparing `tidyarxiv-0.1.0.tar` & `tidyarxiv-0.1.1.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     3722 2023-05-02 23:40:53.218435 tidyarxiv-0.1.0/README.md
--rw-r--r--   0        0        0      459 2023-05-03 23:29:59.409670 tidyarxiv-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     4762 2023-05-03 23:26:29.201288 tidyarxiv-0.1.0/tidyarxiv/tidyarxiv.py
--rw-r--r--   0        0        0     4230 1970-01-01 00:00:00.000000 tidyarxiv-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     3722 2023-05-02 23:40:53.218435 tidyarxiv-0.1.1/README.md
+-rw-r--r--   0        0        0      459 2023-05-03 23:32:19.217516 tidyarxiv-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4760 2023-05-03 23:32:04.509729 tidyarxiv-0.1.1/tidyarxiv/tidyarxiv.py
+-rw-r--r--   0        0        0     4230 1970-01-01 00:00:00.000000 tidyarxiv-0.1.1/PKG-INFO
```

### Comparing `tidyarxiv-0.1.0/README.md` & `tidyarxiv-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `tidyarxiv-0.1.0/tidyarxiv/tidyarxiv.py` & `tidyarxiv-0.1.1/tidyarxiv/tidyarxiv.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
   with open(filepath, 'r', encoding='utf-8') as f:
     contents = [filter_comment(l) for l in f.readlines()]
 
   with open(filepath, 'w', encoding='utf-8') as f:
     f.write(''.join(contents))
 
-def arxiv():
+def main():
   try:
     with open(CONFIG_NAME, encoding='utf-8') as f:
       config = json.loads(f.read())
   except FileNotFoundError:
     print('No ${CONFIG_NAME} file found. Create a ${CONFIG_NAME} file in the root of your project.')
     sys.exit(1)
 
@@ -153,8 +153,8 @@
 
     shutil.copy(os.path.join(tmpdirname, f'{target}.pdf'), f'{target}_{build_time}.pdf')
 
     print('Tarball created: ', f'{target}_{build_time}.tar.gz')
     print('PDF created: ', f'{target}_{build_time}.pdf')
 
 if __name__ == '__main__':
-  arxiv()
+  main()
```

### Comparing `tidyarxiv-0.1.0/PKG-INFO` & `tidyarxiv-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tidyarxiv
-Version: 0.1.0
+Version: 0.1.1
 Summary: A simple script to prepare your LaTeX paper for arXiv submission
 License: GPL-3.0-only
 Author: Dionysis Zindros
 Author-email: dionyziz@stanford.edu
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

