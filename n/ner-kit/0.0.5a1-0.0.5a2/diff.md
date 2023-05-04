# Comparing `tmp/ner-kit-0.0.5a1.tar.gz` & `tmp/ner-kit-0.0.5a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\UIBE??\?????\????\ner-kit\dist\tmpi_5f5b85\ner-kit-0.0.5a1.tar", last modified: Mon Jan 31 23:58:13 2022, max compression
+gzip compressed data, was "D:\UIBE??\?????\????\ner-kit\dist\tmpqm12rn9p\ner-kit-0.0.5a2.tar", last modified: Tue Feb  1 07:17:26 2022, max compression
```

## Comparing `ner-kit-0.0.5a1.tar` & `ner-kit-0.0.5a2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2022-01-31 23:58:13.000000 ner-kit-0.0.5a1/
--rw-rw-rw-   0        0        0     1086 2022-01-01 02:12:11.000000 ner-kit-0.0.5a1/LICENSE
--rw-rw-rw-   0        0        0      278 2022-01-16 05:22:04.000000 ner-kit-0.0.5a1/MANIFEST.in
--rw-rw-rw-   0        0        0     6969 2022-01-31 23:58:13.000000 ner-kit-0.0.5a1/PKG-INFO
--rw-rw-rw-   0        0        0     5701 2022-01-22 20:40:02.000000 ner-kit-0.0.5a1/README.md
--rw-rw-rw-   0        0        0       81 2022-01-31 23:58:13.000000 ner-kit-0.0.5a1/setup.cfg
--rw-rw-rw-   0        0        0     8602 2022-01-31 23:57:31.000000 ner-kit-0.0.5a1/setup.py
-drwxrwxrwx   0        0        0        0 2022-01-31 23:58:13.000000 ner-kit-0.0.5a1/src/
-drwxrwxrwx   0        0        0        0 2022-01-31 23:58:13.000000 ner-kit-0.0.5a1/src/nerkit/
--rw-rw-rw-   0        0        0      599 2022-01-15 14:44:59.000000 ner-kit-0.0.5a1/src/nerkit/HanLP.py
--rw-rw-rw-   0        0        0      265 2022-01-17 20:00:48.000000 ner-kit-0.0.5a1/src/nerkit/StanfordCoreNLP.py
--rw-rw-rw-   0        0        0    15832 2022-01-31 23:28:15.000000 ner-kit-0.0.5a1/src/nerkit/StanzaApi.py
-drwxrwxrwx   0        0        0        0 2022-01-31 23:58:13.000000 ner-kit-0.0.5a1/src/nerkit/triples/
--rw-rw-rw-   0        0        0     6797 2022-01-18 06:03:01.000000 ner-kit-0.0.5a1/src/nerkit/triples/ltp.py
--rw-rw-rw-   0        0        0    23042 2022-01-18 06:08:31.000000 ner-kit-0.0.5a1/src/nerkit/triples/patterns.py
--rw-rw-rw-   0        0        0     3484 2022-01-17 23:38:03.000000 ner-kit-0.0.5a1/src/nerkit/triples/sentence_parser.py
--rw-rw-rw-   0        0        0     3236 2022-01-18 13:23:23.000000 ner-kit-0.0.5a1/src/nerkit/triples/text.py
--rw-rw-rw-   0        0        0        0 2022-01-15 13:21:50.000000 ner-kit-0.0.5a1/src/nerkit/triples/__init__.py
-drwxrwxrwx   0        0        0        0 2022-01-31 23:58:13.000000 ner-kit-0.0.5a1/src/nerkit/triples/__pycache__/
--rw-rw-rw-   0        0        0     4431 2022-01-18 06:04:22.000000 ner-kit-0.0.5a1/src/nerkit/triples/__pycache__/ltp.cpython-36.pyc
--rw-rw-rw-   0        0        0    23086 2022-01-17 23:42:48.000000 ner-kit-0.0.5a1/src/nerkit/triples/__pycache__/patterns.cpython-36.pyc
--rw-rw-rw-   0        0        0     3013 2022-01-17 23:38:03.000000 ner-kit-0.0.5a1/src/nerkit/triples/__pycache__/sentence_parser.cpython-36.pyc
--rw-rw-rw-   0        0        0     1152 2022-01-18 10:52:56.000000 ner-kit-0.0.5a1/src/nerkit/triples/__pycache__/text.cpython-36.pyc
--rw-rw-rw-   0        0        0      167 2022-01-18 00:15:50.000000 ner-kit-0.0.5a1/src/nerkit/triples/__pycache__/__init__.cpython-36.pyc
--rw-rw-rw-   0        0        0        0 2022-01-15 13:21:50.000000 ner-kit-0.0.5a1/src/nerkit/__init__.py
-drwxrwxrwx   0        0        0        0 2022-01-31 23:58:13.000000 ner-kit-0.0.5a1/src/nerkit/__pycache__/
--rw-rw-rw-   0        0        0      587 2022-01-15 14:46:52.000000 ner-kit-0.0.5a1/src/nerkit/__pycache__/HanLP.cpython-36.pyc
--rw-rw-rw-   0        0        0      471 2022-01-15 14:23:58.000000 ner-kit-0.0.5a1/src/nerkit/__pycache__/StanfordCoreNLP.cpython-36.pyc
--rw-rw-rw-   0        0        0    13014 2022-01-17 22:16:42.000000 ner-kit-0.0.5a1/src/nerkit/__pycache__/StanzaApi.cpython-36.pyc
--rw-rw-rw-   0        0        0      159 2022-01-15 14:15:16.000000 ner-kit-0.0.5a1/src/nerkit/__pycache__/__init__.cpython-36.pyc
-drwxrwxrwx   0        0        0        0 2022-01-31 23:58:13.000000 ner-kit-0.0.5a1/src/ner_kit.egg-info/
--rw-rw-rw-   0        0        0        1 2022-01-31 23:58:13.000000 ner-kit-0.0.5a1/src/ner_kit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     6969 2022-01-31 23:58:13.000000 ner-kit-0.0.5a1/src/ner_kit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      108 2022-01-31 23:58:13.000000 ner-kit-0.0.5a1/src/ner_kit.egg-info/requires.txt
--rw-rw-rw-   0        0        0      938 2022-01-31 23:58:13.000000 ner-kit-0.0.5a1/src/ner_kit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        7 2022-01-31 23:58:13.000000 ner-kit-0.0.5a1/src/ner_kit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2022-02-01 07:17:26.000000 ner-kit-0.0.5a2/
+-rw-rw-rw-   0        0        0     1086 2022-01-01 02:12:11.000000 ner-kit-0.0.5a2/LICENSE
+-rw-rw-rw-   0        0        0      278 2022-01-16 05:22:04.000000 ner-kit-0.0.5a2/MANIFEST.in
+-rw-rw-rw-   0        0        0     6969 2022-02-01 07:17:26.000000 ner-kit-0.0.5a2/PKG-INFO
+-rw-rw-rw-   0        0        0     5701 2022-01-22 20:40:02.000000 ner-kit-0.0.5a2/README.md
+-rw-rw-rw-   0        0        0       81 2022-02-01 07:17:26.000000 ner-kit-0.0.5a2/setup.cfg
+-rw-rw-rw-   0        0        0     8602 2022-02-01 07:16:56.000000 ner-kit-0.0.5a2/setup.py
+drwxrwxrwx   0        0        0        0 2022-02-01 07:17:26.000000 ner-kit-0.0.5a2/src/
+drwxrwxrwx   0        0        0        0 2022-02-01 07:17:26.000000 ner-kit-0.0.5a2/src/nerkit/
+-rw-rw-rw-   0        0        0      599 2022-01-15 14:44:59.000000 ner-kit-0.0.5a2/src/nerkit/HanLP.py
+-rw-rw-rw-   0        0        0      265 2022-01-17 20:00:48.000000 ner-kit-0.0.5a2/src/nerkit/StanfordCoreNLP.py
+-rw-rw-rw-   0        0        0    15912 2022-02-01 07:12:12.000000 ner-kit-0.0.5a2/src/nerkit/StanzaApi.py
+drwxrwxrwx   0        0        0        0 2022-02-01 07:17:26.000000 ner-kit-0.0.5a2/src/nerkit/triples/
+-rw-rw-rw-   0        0        0     6797 2022-01-18 06:03:01.000000 ner-kit-0.0.5a2/src/nerkit/triples/ltp.py
+-rw-rw-rw-   0        0        0    23042 2022-01-18 06:08:31.000000 ner-kit-0.0.5a2/src/nerkit/triples/patterns.py
+-rw-rw-rw-   0        0        0     3484 2022-01-17 23:38:03.000000 ner-kit-0.0.5a2/src/nerkit/triples/sentence_parser.py
+-rw-rw-rw-   0        0        0     3236 2022-01-18 13:23:23.000000 ner-kit-0.0.5a2/src/nerkit/triples/text.py
+-rw-rw-rw-   0        0        0        0 2022-01-15 13:21:50.000000 ner-kit-0.0.5a2/src/nerkit/triples/__init__.py
+drwxrwxrwx   0        0        0        0 2022-02-01 07:17:26.000000 ner-kit-0.0.5a2/src/nerkit/triples/__pycache__/
+-rw-rw-rw-   0        0        0     4431 2022-01-18 06:04:22.000000 ner-kit-0.0.5a2/src/nerkit/triples/__pycache__/ltp.cpython-36.pyc
+-rw-rw-rw-   0        0        0    23086 2022-01-17 23:42:48.000000 ner-kit-0.0.5a2/src/nerkit/triples/__pycache__/patterns.cpython-36.pyc
+-rw-rw-rw-   0        0        0     3013 2022-01-17 23:38:03.000000 ner-kit-0.0.5a2/src/nerkit/triples/__pycache__/sentence_parser.cpython-36.pyc
+-rw-rw-rw-   0        0        0     1152 2022-01-18 10:52:56.000000 ner-kit-0.0.5a2/src/nerkit/triples/__pycache__/text.cpython-36.pyc
+-rw-rw-rw-   0        0        0      167 2022-01-18 00:15:50.000000 ner-kit-0.0.5a2/src/nerkit/triples/__pycache__/__init__.cpython-36.pyc
+-rw-rw-rw-   0        0        0        0 2022-01-15 13:21:50.000000 ner-kit-0.0.5a2/src/nerkit/__init__.py
+drwxrwxrwx   0        0        0        0 2022-02-01 07:17:26.000000 ner-kit-0.0.5a2/src/nerkit/__pycache__/
+-rw-rw-rw-   0        0        0      587 2022-01-15 14:46:52.000000 ner-kit-0.0.5a2/src/nerkit/__pycache__/HanLP.cpython-36.pyc
+-rw-rw-rw-   0        0        0      471 2022-01-15 14:23:58.000000 ner-kit-0.0.5a2/src/nerkit/__pycache__/StanfordCoreNLP.cpython-36.pyc
+-rw-rw-rw-   0        0        0    13476 2022-02-01 07:07:27.000000 ner-kit-0.0.5a2/src/nerkit/__pycache__/StanzaApi.cpython-36.pyc
+-rw-rw-rw-   0        0        0      159 2022-01-15 14:15:16.000000 ner-kit-0.0.5a2/src/nerkit/__pycache__/__init__.cpython-36.pyc
+drwxrwxrwx   0        0        0        0 2022-02-01 07:17:26.000000 ner-kit-0.0.5a2/src/ner_kit.egg-info/
+-rw-rw-rw-   0        0        0        1 2022-02-01 07:17:26.000000 ner-kit-0.0.5a2/src/ner_kit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     6969 2022-02-01 07:17:26.000000 ner-kit-0.0.5a2/src/ner_kit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      108 2022-02-01 07:17:26.000000 ner-kit-0.0.5a2/src/ner_kit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      938 2022-02-01 07:17:26.000000 ner-kit-0.0.5a2/src/ner_kit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        7 2022-02-01 07:17:26.000000 ner-kit-0.0.5a2/src/ner_kit.egg-info/top_level.txt
```

### Comparing `ner-kit-0.0.5a1/LICENSE` & `ner-kit-0.0.5a2/LICENSE`

 * *Files identical despite different names*

### Comparing `ner-kit-0.0.5a1/PKG-INFO` & `ner-kit-0.0.5a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ner-kit
-Version: 0.0.5a1
+Version: 0.0.5a2
 Summary: Named Entity Recognition Toolkit
 Home-page: https://github.com/dhchenx/ner-kit
 Author: Donghua Chen
 Author-email: douglaschan@126.com
 License: MIT
 Project-URL: Bug Reports, https://github.com/dhchenx/ner-kit/issues
 Project-URL: Source, https://github.com/dhchenx/ner-kit
```

### Comparing `ner-kit-0.0.5a1/README.md` & `ner-kit-0.0.5a2/README.md`

 * *Files identical despite different names*

### Comparing `ner-kit-0.0.5a1/setup.py` & `ner-kit-0.0.5a2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='0.0.5a1',  # Required
+    version='0.0.5a2',  # Required
 
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description='Named Entity Recognition Toolkit',  # Optional
 
     # This is an optional longer description of your project that represents
```

### Comparing `ner-kit-0.0.5a1/src/nerkit/HanLP.py` & `ner-kit-0.0.5a2/src/nerkit/HanLP.py`

 * *Files identical despite different names*

### Comparing `ner-kit-0.0.5a1/src/nerkit/StanzaApi.py` & `ner-kit-0.0.5a2/src/nerkit/StanzaApi.py`

 * *Files 1% similar despite different names*

```diff
@@ -224,23 +224,25 @@
         doc = nlp(text)
         if self.should_print_result:
             print(*[
             f'id: {word.id}\tword: {word.text}\thead id: {word.head}\thead: {sent.words[word.head - 1].text if word.head > 0 else "root"}\tdeprel: {word.deprel}'
             for sent in doc.sentences for word in sent.words], sep='\n')
         list_result = []
         for sent in doc.sentences:
+            list_token=[]
             for word in sent.words:
                 model = {
-                    "id": word.id,
+                    "id": str(word.id),
                     "text": word.text,
-                    "head id": word.head,
+                    "head id": str(word.head),
                     "head": sent.words[word.head - 1].text if word.head > 0 else "root",
                     "deprel":word.deprel
                 }
-                list_result.append(model)
+                list_token.append(model)
+            list_result.append(list_token)
         return list_result
 
     def ner(self,text,lang='en',processors='tokenize,ner',verbose=False,tokenize_pretokenized=False):
         nlp = stanza.Pipeline(lang=lang, processors=processors,verbose=verbose,tokenize_pretokenized=tokenize_pretokenized,use_gpu=self.use_gpu)
         doc = nlp(text)
         if self.should_print_result:
             print(*[f'entity: {ent.text}\ttype: {ent.type}' for ent in doc.ents], sep='\n')
```

### Comparing `ner-kit-0.0.5a1/src/nerkit/triples/ltp.py` & `ner-kit-0.0.5a2/src/nerkit/triples/ltp.py`

 * *Files identical despite different names*

### Comparing `ner-kit-0.0.5a1/src/nerkit/triples/patterns.py` & `ner-kit-0.0.5a2/src/nerkit/triples/patterns.py`

 * *Files identical despite different names*

### Comparing `ner-kit-0.0.5a1/src/nerkit/triples/sentence_parser.py` & `ner-kit-0.0.5a2/src/nerkit/triples/sentence_parser.py`

 * *Files identical despite different names*

### Comparing `ner-kit-0.0.5a1/src/nerkit/triples/text.py` & `ner-kit-0.0.5a2/src/nerkit/triples/text.py`

 * *Files identical despite different names*

### Comparing `ner-kit-0.0.5a1/src/nerkit/triples/__pycache__/ltp.cpython-36.pyc` & `ner-kit-0.0.5a2/src/nerkit/triples/__pycache__/ltp.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `ner-kit-0.0.5a1/src/nerkit/triples/__pycache__/patterns.cpython-36.pyc` & `ner-kit-0.0.5a2/src/nerkit/triples/__pycache__/patterns.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `ner-kit-0.0.5a1/src/nerkit/triples/__pycache__/sentence_parser.cpython-36.pyc` & `ner-kit-0.0.5a2/src/nerkit/triples/__pycache__/sentence_parser.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `ner-kit-0.0.5a1/src/nerkit/triples/__pycache__/text.cpython-36.pyc` & `ner-kit-0.0.5a2/src/nerkit/triples/__pycache__/text.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `ner-kit-0.0.5a1/src/nerkit/__pycache__/HanLP.cpython-36.pyc` & `ner-kit-0.0.5a2/src/nerkit/__pycache__/HanLP.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `ner-kit-0.0.5a1/src/nerkit/__pycache__/StanzaApi.cpython-36.pyc` & `ner-kit-0.0.5a2/src/nerkit/__pycache__/StanzaApi.cpython-36.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: python 3.6 byte-compiled*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 330d 0d0a caea e561 453c 0000 e300 0000  3......aE<......
+00000000: 330d 0d0a aad9 f861 e23d 0000 e300 0000  3......a.=......
 00000010: 0000 0000 0000 0000 0003 0000 0040 0000  .............@..
 00000020: 0073 6400 0000 6400 6401 6c00 5a00 6400  .sd...d.d.l.Z.d.
 00000030: 6402 6c01 6d02 5a02 6d03 5a03 0100 6400  d.l.m.Z.m.Z...d.
 00000040: 6403 6c04 6d05 5a05 0100 6400 6404 6c06  d.l.m.Z...d.d.l.
 00000050: 6d07 5a07 0100 6400 6405 6c08 6d09 5a09  m.Z...d.d.l.m.Z.
 00000060: 0100 6400 6401 6c0a 5a0a 4700 6406 6407  ..d.d.l.Z.G.d.d.
 00000070: 8400 6407 8302 5a0b 4700 6408 6409 8400  ..d...Z.G.d.d...
@@ -141,674 +141,703 @@
 000008c0: 6c65 5f5f da0c 5f5f 7175 616c 6e61 6d65  le__..__qualname
 000008d0: 5f5f 7219 0000 0072 1400 0000 7222 0000  __r....r....r"..
 000008e0: 0072 2b00 0000 7235 0000 0072 1700 0000  .r+...r5...r....
 000008f0: 7217 0000 0072 1700 0000 7218 0000 0072  r....r....r....r
 00000900: 0700 0000 0700 0000 730a 0000 0008 010a  ........s.......
 00000910: 0e08 0408 0e0a 1f72 0700 0000 6300 0000  .......r....c...
 00000920: 0000 0000 0000 0000 0005 0000 0040 0000  .............@..
-00000930: 0073 e400 0000 6500 5a01 6400 5a02 643b  .s....e.Z.d.Z.d;
-00000940: 6402 6403 8401 5a03 643c 6406 6407 8401  d.d...Z.d<d.d...
-00000950: 5a04 643d 6409 640a 8401 5a05 640b 640c  Z.d=d.d...Z.d.d.
-00000960: 8400 5a06 643e 640e 640f 8401 5a07 643f  ..Z.d>d.d...Z.d?
-00000970: 6410 6411 8401 5a08 6440 6412 6413 8401  d.d...Z.d@d.d...
-00000980: 5a09 6441 6414 6415 8401 5a0a 6442 6417  Z.dAd.d...Z.dBd.
-00000990: 6418 8401 5a0b 6443 641a 641b 8401 5a0c  d...Z.dCd.d...Z.
-000009a0: 6444 641d 641e 8401 5a0d 6445 641f 6420  dDd.d...Z.dEd.d 
-000009b0: 8401 5a0e 6446 6422 6423 8401 5a0f 6447  ..Z.dFd"d#..Z.dG
-000009c0: 6425 6426 8401 5a10 6448 6427 6428 8401  d%d&..Z.dHd'd(..
-000009d0: 5a11 6449 6429 642a 8401 5a12 644a 642b  Z.dId)d*..Z.dJd+
-000009e0: 642c 8401 5a13 644b 642e 642f 8401 5a14  d,..Z.dKd.d/..Z.
-000009f0: 644c 6430 6431 8401 5a15 644d 6433 6434  dLd0d1..Z.dMd3d4
-00000a00: 8401 5a16 644e 6437 6438 8401 5a17 6439  ..Z.dNd7d8..Z.d9
-00000a10: 643a 8400 5a18 6435 5300 294f da0d 5374  d:..Z.d5S.)O..St
-00000a20: 616e 7a61 5772 6170 7065 7246 6304 0000  anzaWrapperFc...
-00000a30: 0000 0000 0004 0000 0003 0000 0043 0000  .............C..
-00000a40: 0073 2600 0000 7c01 7210 7c00 6a00 6401  .s&...|.r.|.j.d.
-00000a50: 6402 8d01 0100 7c02 721c 7c00 6a01 8300  d.....|.r.|.j...
-00000a60: 0100 7c03 7c00 5f02 6400 5300 2903 4e72  ..|.|._.d.S.).Nr
-00000a70: 0800 0000 2901 da04 6c61 6e67 2903 da08  ....)...lang)...
-00000a80: 646f 776e 6c6f 6164 da16 646f 776e 6c6f  download..downlo
-00000a90: 6164 5f63 6869 6e65 7365 5f6d 6f64 656c  ad_chinese_model
-00000aa0: da13 7368 6f75 6c64 5f70 7269 6e74 5f72  ..should_print_r
-00000ab0: 6573 756c 7429 0472 1600 0000 5a10 6175  esult).r....Z.au
-00000ac0: 746f 5f64 6f77 6e6c 6f61 645f 656e 5a10  to_download_enZ.
-00000ad0: 6175 746f 5f64 6f77 6e6c 6f61 645f 7a68  auto_download_zh
-00000ae0: 5a10 7368 6f75 6c64 5f70 7269 6e74 5f6d  Z.should_print_m
-00000af0: 7367 7217 0000 0072 1700 0000 7218 0000  sgr....r....r...
-00000b00: 0072 1900 0000 5900 0000 730a 0000 0000  .r....Y...s.....
-00000b10: 0104 010c 0104 0108 017a 1653 7461 6e7a  .........z.Stanz
-00000b20: 6157 7261 7070 6572 2e5f 5f69 6e69 745f  aWrapper.__init_
-00000b30: 5f72 0800 0000 fa0c 746f 6b65 6e69 7a65  _r......tokenize
-00000b40: 2c70 6f73 6304 0000 0000 0000 0004 0000  ,posc...........
-00000b50: 0005 0000 0043 0000 0073 1400 0000 7400  .....C...s....t.
-00000b60: 6a01 7c01 7c02 7c03 6401 8d03 0100 6400  j.|.|.|.d.....d.
-00000b70: 5300 2902 4e29 02da 0a70 726f 6365 7373  S.).N)...process
-00000b80: 6f72 73da 0776 6572 626f 7365 2902 7213  ors..verbose).r.
-00000b90: 0000 0072 3b00 0000 2904 7216 0000 0072  ...r;...).r....r
-00000ba0: 3a00 0000 723f 0000 0072 4000 0000 7217  :...r?...r@...r.
-00000bb0: 0000 0072 1700 0000 7218 0000 0072 3b00  ...r....r....r;.
-00000bc0: 0000 6000 0000 7302 0000 0000 017a 1653  ..`...s......z.S
-00000bd0: 7461 6e7a 6157 7261 7070 6572 2e64 6f77  tanzaWrapper.dow
-00000be0: 6e6c 6f61 64da 027a 6863 0300 0000 0000  nload..zhc......
-00000bf0: 0000 0300 0000 0400 0000 4300 0000 7312  ..........C...s.
-00000c00: 0000 0074 006a 017c 017c 0264 018d 0201  ...t.j.|.|.d....
-00000c10: 0064 0053 0029 024e 2902 723a 0000 0072  .d.S.).N).r:...r
-00000c20: 4000 0000 2902 7213 0000 0072 3b00 0000  @...).r....r;...
-00000c30: 2903 7216 0000 0072 3a00 0000 5a06 7665  ).r....r:...Z.ve
-00000c40: 7262 6f73 7217 0000 0072 1700 0000 7218  rbosr....r....r.
-00000c50: 0000 0072 3c00 0000 6300 0000 7302 0000  ...r<...c...s...
-00000c60: 0000 017a 2453 7461 6e7a 6157 7261 7070  ...z$StanzaWrapp
-00000c70: 6572 2e64 6f77 6e6c 6f61 645f 6368 696e  er.download_chin
-00000c80: 6573 655f 6d6f 6465 6c63 0200 0000 0000  ese_modelc......
-00000c90: 0000 0200 0000 0400 0000 4300 0000 730e  ..........C...s.
-00000ca0: 0000 007c 006a 007c 0164 0164 028d 0253  ...|.j.|.d.d...S
-00000cb0: 0029 034e 7241 0000 0029 0172 3a00 0000  .).NrA...).r:...
-00000cc0: 2901 720d 0000 0029 0272 1600 0000 721f  ).r....).r....r.
-00000cd0: 0000 0072 1700 0000 7217 0000 0072 1800  ...r....r....r..
-00000ce0: 0000 da10 746f 6b65 6e69 7a65 5f63 6869  ....tokenize_chi
-00000cf0: 6e65 7365 6600 0000 7302 0000 0000 017a  nesef...s......z
-00000d00: 1e53 7461 6e7a 6157 7261 7070 6572 2e74  .StanzaWrapper.t
-00000d10: 6f6b 656e 697a 655f 6368 696e 6573 6572  okenize_chineser
-00000d20: 0d00 0000 6307 0000 0000 0000 000f 0000  ....c...........
-00000d30: 0007 0000 0043 0000 0073 a600 0000 7400  .....C...s....t.
-00000d40: 6a01 7c02 7c03 7c04 7c05 7c06 6401 8d05  j.|.|.|.|.|.d...
-00000d50: 7d07 7c07 7c01 8301 7d08 6700 7d09 7880  }.|.|...}.g.}.x.
-00000d60: 7402 7c08 6a03 8301 4400 5d72 5c02 7d0a  t.|.j...D.]r\.}.
-00000d70: 7d0b 7c00 6a04 7268 7405 6402 7c0a 6403  }.|.j.rht.d.|.d.
-00000d80: 1700 9b00 6404 9d03 8301 0100 7405 6405  ....d.......t.d.
-00000d90: 6406 8400 7c0b 6a06 4400 8301 6407 6408  d...|.j.D...d.d.
-00000da0: 6901 8e01 0100 6700 7d0c 7826 7c0b 6a06  i.....g.}.x&|.j.
-00000db0: 4400 5d1c 7d0d 7c0d 6a07 7c0d 6a08 6409  D.].}.|.j.|.j.d.
-00000dc0: 9c02 7d0e 7c0c 6a09 7c0e 8301 0100 7174  ..}.|.j.|.....qt
-00000dd0: 5700 7c09 6a09 7c0c 8301 0100 712c 5700  W.|.j.|.....q,W.
-00000de0: 7c09 5300 290a 4e29 0572 3a00 0000 723f  |.S.).N).r:...r?
-00000df0: 0000 00da 1274 6f6b 656e 697a 655f 6e6f  .....tokenize_no
-00000e00: 5f73 7370 6c69 74da 1574 6f6b 656e 697a  _ssplit..tokeniz
-00000e10: 655f 7072 6574 6f6b 656e 697a 6564 7240  e_pretokenizedr@
-00000e20: 0000 007a 103d 3d3d 3d3d 3d20 5365 6e74  ...z.====== Sent
-00000e30: 656e 6365 2072 2300 0000 7a0f 2074 6f6b  ence r#...z. tok
-00000e40: 656e 7320 3d3d 3d3d 3d3d 3d63 0100 0000  ens =======c....
-00000e50: 0000 0000 0200 0000 0600 0000 5300 0000  ............S...
-00000e60: 7320 0000 0067 007c 005d 187d 0164 007c  s ...g.|.].}.d.|
-00000e70: 016a 009b 0064 017c 016a 019b 009d 0491  .j...d.|.j......
-00000e80: 0271 0453 0029 027a 0469 643a 207a 0709  .q.S.).z.id: z..
-00000e90: 7465 7874 3a20 2902 da02 6964 721f 0000  text: )...idr...
-00000ea0: 0029 02da 022e 3072 1d00 0000 7217 0000  .)....0r....r...
-00000eb0: 0072 1700 0000 7218 0000 00fa 0a3c 6c69  .r....r......<li
-00000ec0: 7374 636f 6d70 3e71 0000 0073 0200 0000  stcomp>q...s....
-00000ed0: 0600 7a2a 5374 616e 7a61 5772 6170 7065  ..z*StanzaWrappe
-00000ee0: 722e 746f 6b65 6e69 7a65 2e3c 6c6f 6361  r.tokenize.<loca
-00000ef0: 6c73 3e2e 3c6c 6973 7463 6f6d 703e da03  ls>.<listcomp>..
-00000f00: 7365 7072 2d00 0000 2902 7245 0000 0072  sepr-...).rE...r
-00000f10: 1f00 0000 290a 7213 0000 0072 0500 0000  ....).r....r....
-00000f20: da09 656e 756d 6572 6174 65da 0973 656e  ..enumerate..sen
-00000f30: 7465 6e63 6573 723d 0000 00da 0570 7269  tencesr=.....pri
-00000f40: 6e74 da06 746f 6b65 6e73 7245 0000 0072  nt..tokensrE...r
-00000f50: 1f00 0000 721e 0000 0029 0f72 1600 0000  ....r....).r....
-00000f60: 721f 0000 0072 3a00 0000 723f 0000 0072  r....r:...r?...r
-00000f70: 4300 0000 7244 0000 0072 4000 0000 da03  C...rD...r@.....
-00000f80: 6e6c 70da 0364 6f63 da0d 6c69 7374 5f73  nlp..doc..list_s
-00000f90: 656e 7465 6e63 65da 0169 721c 0000 0072  entence..ir....r
-00000fa0: 4c00 0000 721d 0000 0072 2a00 0000 7217  L...r....r*...r.
-00000fb0: 0000 0072 1700 0000 7218 0000 0072 0d00  ...r....r....r..
-00000fc0: 0000 6900 0000 731c 0000 0000 0114 0108  ..i...s.........
-00000fd0: 0104 0214 0106 0114 011a 0104 010c 0204  ................
-00000fe0: 010a 020e 010e 017a 1653 7461 6e7a 6157  .......z.StanzaW
-00000ff0: 7261 7070 6572 2e74 6f6b 656e 697a 6563  rapper.tokenizec
-00001000: 0700 0000 0000 0000 0c00 0000 0700 0000  ................
-00001010: 4300 0000 7370 0000 0074 006a 017c 027c  C...sp...t.j.|.|
-00001020: 037c 047c 057c 0664 018d 057d 077c 077c  .|.|.|.d...}.|.|
-00001030: 0183 017d 0867 007d 0978 4a74 027c 086a  ...}.g.}.xJt.|.j
-00001040: 0383 0144 005d 3c5c 027d 0a7d 0b7c 006a  ...D.]<\.}.}.|.j
-00001050: 0472 5c74 0564 027c 0a64 0317 009b 0064  .r\t.d.|.d.....d
-00001060: 049d 0383 0101 0074 057c 0b6a 0664 0564  .......t.|.j.d.d
-00001070: 068d 0201 007c 096a 077c 0b6a 0683 0101  .....|.j.|.j....
-00001080: 0071 2c57 007c 0953 0029 074e 2905 723a  .q,W.|.S.).N).r:
-00001090: 0000 0072 3f00 0000 7243 0000 0072 4400  ...r?...rC...rD.
-000010a0: 0000 7240 0000 007a 103d 3d3d 3d3d 3d20  ..r@...z.====== 
-000010b0: 5365 6e74 656e 6365 2072 2300 0000 7a0f  Sentence r#...z.
-000010c0: 2074 6f6b 656e 7320 3d3d 3d3d 3d3d 3d72   tokens =======r
-000010d0: 2d00 0000 2901 7248 0000 0029 0872 1300  -...).rH...).r..
-000010e0: 0000 7205 0000 0072 4900 0000 724a 0000  ..r....rI...rJ..
-000010f0: 0072 3d00 0000 724b 0000 0072 1f00 0000  .r=...rK...r....
-00001100: 721e 0000 0029 0c72 1600 0000 721f 0000  r....).r....r...
-00001110: 0072 3a00 0000 723f 0000 0072 4300 0000  .r:...r?...rC...
-00001120: 7244 0000 0072 4000 0000 724d 0000 0072  rD...r@...rM...r
-00001130: 4e00 0000 724f 0000 0072 5000 0000 721c  N...rO...rP...r.
-00001140: 0000 0072 1700 0000 7217 0000 0072 1800  ...r....r....r..
-00001150: 0000 da11 746f 6b65 6e69 7a65 5f73 656e  ....tokenize_sen
-00001160: 7465 6e63 657c 0000 0073 1200 0000 0001  tence|...s......
-00001170: 1401 0801 0401 1401 0601 1401 0e01 1001  ................
-00001180: 7a1f 5374 616e 7a61 5772 6170 7065 722e  z.StanzaWrapper.
-00001190: 746f 6b65 6e69 7a65 5f73 656e 7465 6e63  tokenize_sentenc
-000011a0: 6563 0700 0000 0000 0000 0f00 0000 0700  ec..............
-000011b0: 0000 4300 0000 73a6 0000 0074 006a 017c  ..C...s....t.j.|
-000011c0: 027c 037c 047c 057c 0664 018d 057d 077c  .|.|.|.|.d...}.|
-000011d0: 077c 0183 017d 0867 007d 0978 8074 027c  .|...}.g.}.x.t.|
-000011e0: 086a 0383 0144 005d 725c 027d 0a7d 0b7c  .j...D.]r\.}.}.|
-000011f0: 006a 0472 6874 0564 027c 0a64 0317 009b  .j.rht.d.|.d....
-00001200: 0064 049d 0383 0101 0074 0564 0564 0684  .d.......t.d.d..
-00001210: 007c 0b6a 0644 0083 0164 0764 0869 018e  .|.j.D...d.d.i..
-00001220: 0101 0067 007d 0c78 267c 0b6a 0644 005d  ...g.}.x&|.j.D.]
-00001230: 1c7d 0d7c 0d6a 077c 0d6a 0864 099c 027d  .}.|.j.|.j.d...}
-00001240: 0e7c 0c6a 097c 0e83 0101 0071 7457 007c  .|.j.|.....qtW.|
-00001250: 096a 097c 0c83 0101 0071 2c57 007c 0953  .j.|.....q,W.|.S
-00001260: 0029 0a4e 2905 723a 0000 0072 3f00 0000  .).N).r:...r?...
-00001270: 7243 0000 0072 4400 0000 7240 0000 007a  rC...rD...r@...z
-00001280: 103d 3d3d 3d3d 3d20 5365 6e74 656e 6365  .====== Sentence
-00001290: 2072 2300 0000 7a0f 2074 6f6b 656e 7320   r#...z. tokens 
-000012a0: 3d3d 3d3d 3d3d 3d63 0100 0000 0000 0000  =======c........
-000012b0: 0200 0000 0600 0000 5300 0000 7320 0000  ........S...s ..
-000012c0: 0067 007c 005d 187d 0164 007c 016a 009b  .g.|.].}.d.|.j..
-000012d0: 0064 017c 016a 019b 009d 0491 0271 0453  .d.|.j.......q.S
-000012e0: 0029 027a 0469 643a 207a 0709 7465 7874  .).z.id: z..text
-000012f0: 3a20 2902 7245 0000 0072 1f00 0000 2902  : ).rE...r....).
-00001300: 7246 0000 0072 1d00 0000 7217 0000 0072  rF...r....r....r
-00001310: 1700 0000 7218 0000 0072 4700 0000 8e00  ....r....rG.....
-00001320: 0000 7302 0000 0006 007a 2f53 7461 6e7a  ..s......z/Stanz
-00001330: 6157 7261 7070 6572 2e74 6f6b 656e 697a  aWrapper.tokeniz
-00001340: 655f 6c69 7374 2e3c 6c6f 6361 6c73 3e2e  e_list.<locals>.
-00001350: 3c6c 6973 7463 6f6d 703e 7248 0000 0072  <listcomp>rH...r
-00001360: 2d00 0000 2902 7245 0000 0072 1f00 0000  -...).rE...r....
-00001370: 290a 7213 0000 0072 0500 0000 7249 0000  ).r....r....rI..
-00001380: 0072 4a00 0000 723d 0000 0072 4b00 0000  .rJ...r=...rK...
-00001390: 724c 0000 0072 4500 0000 721f 0000 0072  rL...rE...r....r
-000013a0: 1e00 0000 290f 7216 0000 005a 0b6c 6973  ....).r....Z.lis
-000013b0: 745f 746f 6b65 6e73 723a 0000 0072 3f00  t_tokensr:...r?.
-000013c0: 0000 7243 0000 0072 4400 0000 7240 0000  ..rC...rD...r@..
-000013d0: 0072 4d00 0000 724e 0000 0072 4f00 0000  .rM...rN...rO...
-000013e0: 7250 0000 0072 1c00 0000 724c 0000 0072  rP...r....rL...r
-000013f0: 1d00 0000 722a 0000 0072 1700 0000 7217  ....r*...r....r.
-00001400: 0000 0072 1800 0000 da0d 746f 6b65 6e69  ...r......tokeni
-00001410: 7a65 5f6c 6973 7487 0000 0073 1c00 0000  ze_list....s....
-00001420: 0001 1401 0801 0401 1401 0601 1401 1a01  ................
-00001430: 0401 0c02 0401 0a02 0e01 0e01 7a1b 5374  ............z.St
-00001440: 616e 7a61 5772 6170 7065 722e 746f 6b65  anzaWrapper.toke
-00001450: 6e69 7a65 5f6c 6973 7463 0300 0000 0000  nize_listc......
-00001460: 0000 0c00 0000 0500 0000 4300 0000 73aa  ..........C...s.
-00001470: 0000 0064 0164 0269 017d 0374 006a 0164  ...d.d.i.}.t.j.d
-00001480: 037c 037c 0264 048d 037d 047c 047c 0183  .|.|.d...}.|.|..
-00001490: 017d 0567 007d 0678 8074 027c 056a 0383  .}.g.}.x.t.|.j..
-000014a0: 0144 005d 725c 027d 077d 087c 006a 0472  .D.]r\.}.}.|.j.r
-000014b0: 6c74 0564 057c 0764 0617 009b 0064 079d  lt.d.|.d.....d..
-000014c0: 0383 0101 0074 0564 0864 0984 007c 086a  .....t.d.d...|.j
-000014d0: 0644 0083 0164 0a64 0b69 018e 0101 0067  .D...d.d.i.....g
-000014e0: 007d 0978 267c 086a 0644 005d 1c7d 0a7c  .}.x&|.j.D.].}.|
-000014f0: 0a6a 077c 0a6a 0864 0c9c 027d 0b7c 096a  .j.|.j.d...}.|.j
-00001500: 097c 0b83 0101 0071 7857 007c 066a 097c  .|.....qxW.|.j.|
-00001510: 0983 0101 0071 3057 007c 0653 0029 0d4e  .....q0W.|.S.).N
-00001520: 720d 0000 005a 0573 7061 6379 7208 0000  r....Z.spacyr...
-00001530: 0029 0372 3a00 0000 723f 0000 0072 4000  .).r:...r?...r@.
-00001540: 0000 7a10 3d3d 3d3d 3d3d 2053 656e 7465  ..z.====== Sente
-00001550: 6e63 6520 7223 0000 007a 0f20 746f 6b65  nce r#...z. toke
-00001560: 6e73 203d 3d3d 3d3d 3d3d 6301 0000 0000  ns =======c.....
-00001570: 0000 0002 0000 0006 0000 0053 0000 0073  ...........S...s
-00001580: 2000 0000 6700 7c00 5d18 7d01 6400 7c01   ...g.|.].}.d.|.
-00001590: 6a00 9b00 6401 7c01 6a01 9b00 9d04 9102  j...d.|.j.......
-000015a0: 7104 5300 2902 7a04 6964 3a20 7a07 0974  q.S.).z.id: z..t
-000015b0: 6578 743a 2029 0272 4500 0000 721f 0000  ext: ).rE...r...
-000015c0: 0029 0272 4600 0000 721d 0000 0072 1700  .).rF...r....r..
-000015d0: 0000 7217 0000 0072 1800 0000 7247 0000  ..r....r....rG..
-000015e0: 00a1 0000 0073 0200 0000 0600 7a33 5374  .....s......z3St
-000015f0: 616e 7a61 5772 6170 7065 722e 746f 6b65  anzaWrapper.toke
-00001600: 6e69 7a65 5f62 795f 7370 6163 792e 3c6c  nize_by_spacy.<l
-00001610: 6f63 616c 733e 2e3c 6c69 7374 636f 6d70  ocals>.<listcomp
-00001620: 3e72 4800 0000 722d 0000 0029 0272 4500  >rH...r-...).rE.
-00001630: 0000 721f 0000 0029 0a72 1300 0000 7205  ..r....).r....r.
-00001640: 0000 0072 4900 0000 724a 0000 0072 3d00  ...rI...rJ...r=.
-00001650: 0000 724b 0000 0072 4c00 0000 7245 0000  ..rK...rL...rE..
-00001660: 0072 1f00 0000 721e 0000 0029 0c72 1600  .r....r....).r..
-00001670: 0000 721f 0000 0072 4000 0000 723f 0000  ..r....r@...r?..
-00001680: 0072 4d00 0000 724e 0000 0072 4f00 0000  .rM...rN...rO...
-00001690: 7250 0000 0072 1c00 0000 724c 0000 0072  rP...r....rL...r
-000016a0: 1d00 0000 722a 0000 0072 1700 0000 7217  ....r*...r....r.
-000016b0: 0000 0072 1800 0000 da11 746f 6b65 6e69  ...r......tokeni
-000016c0: 7a65 5f62 795f 7370 6163 7999 0000 0073  ze_by_spacy....s
-000016d0: 1e00 0000 0001 0801 1001 0801 0401 1401  ................
-000016e0: 0601 1401 1a01 0401 0c02 0401 0a02 0e01  ................
-000016f0: 0e01 7a1f 5374 616e 7a61 5772 6170 7065  ..z.StanzaWrappe
-00001700: 722e 746f 6b65 6e69 7a65 5f62 795f 7370  r.tokenize_by_sp
-00001710: 6163 79fa 0c74 6f6b 656e 697a 652c 6d77  acy..tokenize,mw
-00001720: 7463 0500 0000 0000 0000 0c00 0000 0900  tc..............
-00001730: 0000 4300 0000 73a4 0000 0074 006a 017c  ..C...s....t.j.|
-00001740: 027c 037c 0464 018d 037d 057c 057c 0183  .|.|.d...}.|.|..
-00001750: 017d 0667 007d 0778 827c 066a 0244 005d  .}.g.}.x.|.j.D.]
-00001760: 787d 0867 007d 0978 647c 086a 0344 005d  x}.g.}.xd|.j.D.]
-00001770: 5a7d 0a7c 006a 0472 6674 0564 027c 0a6a  Z}.|.j.rft.d.|.j
-00001780: 069b 0064 0364 046a 0764 0564 0684 007c  ...d.d.j.d.d...|
-00001790: 0a6a 0844 0083 0183 019b 009d 0483 0101  .j.D............
-000017a0: 007c 0a6a 0664 046a 0764 0764 0684 007c  .|.j.d.j.d.d...|
-000017b0: 0a6a 0844 0083 0183 0164 089c 027d 0b7c  .j.D.....d...}.|
-000017c0: 096a 097c 0b83 0101 0071 3457 007c 076a  .j.|.....q4W.|.j
-000017d0: 097c 0983 0101 0071 2457 007c 0753 0029  .|.....q$W.|.S.)
-000017e0: 094e 2903 723a 0000 0072 3f00 0000 7240  .N).r:...r?...r@
-000017f0: 0000 007a 0774 6f6b 656e 3a20 7a08 0977  ...z.token: z..w
-00001800: 6f72 6473 3a20 7a02 2c20 6301 0000 0000  ords: z., c.....
-00001810: 0000 0002 0000 0003 0000 0053 0000 0073  ...........S...s
-00001820: 1200 0000 6700 7c00 5d0a 7d01 7c01 6a00  ....g.|.].}.|.j.
-00001830: 9102 7104 5300 7217 0000 0029 0172 1f00  ..q.S.r....).r..
-00001840: 0000 2902 7246 0000 00da 0477 6f72 6472  ..).rF.....wordr
-00001850: 1700 0000 7217 0000 0072 1800 0000 7247  ....r....r....rG
-00001860: 0000 00b5 0000 0073 0200 0000 0600 7a2c  .......s......z,
-00001870: 5374 616e 7a61 5772 6170 7065 722e 6d77  StanzaWrapper.mw
-00001880: 745f 6578 7061 6e64 2e3c 6c6f 6361 6c73  t_expand.<locals
-00001890: 3e2e 3c6c 6973 7463 6f6d 703e 6301 0000  >.<listcomp>c...
-000018a0: 0000 0000 0002 0000 0003 0000 0053 0000  .............S..
-000018b0: 0073 1200 0000 6700 7c00 5d0a 7d01 7c01  .s....g.|.].}.|.
-000018c0: 6a00 9102 7104 5300 7217 0000 0029 0172  j...q.S.r....).r
-000018d0: 1f00 0000 2902 7246 0000 0072 5500 0000  ....).rF...rU...
-000018e0: 7217 0000 0072 1700 0000 7218 0000 0072  r....r....r....r
-000018f0: 4700 0000 b800 0000 7302 0000 0006 0029  G.......s......)
-00001900: 0272 1d00 0000 721f 0000 0029 0a72 1300  .r....r....).r..
-00001910: 0000 7205 0000 0072 4a00 0000 724c 0000  ..r....rJ...rL..
-00001920: 0072 3d00 0000 724b 0000 0072 1f00 0000  .r=...rK...r....
-00001930: da04 6a6f 696e da05 776f 7264 7372 1e00  ..join..wordsr..
-00001940: 0000 290c 7216 0000 0072 1f00 0000 723a  ..).r....r....r:
-00001950: 0000 0072 3f00 0000 7240 0000 0072 4d00  ...r?...r@...rM.
-00001960: 0000 724e 0000 0072 2900 0000 721c 0000  ..rN...r)...r...
-00001970: 0072 2000 0000 721d 0000 0072 2a00 0000  .r ...r....r*...
-00001980: 7217 0000 0072 1700 0000 7218 0000 00da  r....r....r.....
-00001990: 0a6d 7774 5f65 7870 616e 64ac 0000 0073  .mwt_expand....s
-000019a0: 1a00 0000 0002 1001 0801 0401 0c01 0401  ................
-000019b0: 0c01 0601 2802 0401 1a02 0e01 0e01 7a18  ....(.........z.
+00000930: 0073 f400 0000 6500 5a01 6400 5a02 6440  .s....e.Z.d.Z.d@
+00000940: 6403 6404 8401 5a03 6441 6407 6408 8401  d.d...Z.dAd.d...
+00000950: 5a04 6442 640a 640b 8401 5a05 640c 640d  Z.dBd.d...Z.d.d.
+00000960: 8400 5a06 640e 640f 8400 5a07 6410 6411  ..Z.d.d...Z.d.d.
+00000970: 8400 5a08 6443 6413 6414 8401 5a09 6444  ..Z.dCd.d...Z.dD
+00000980: 6415 6416 8401 5a0a 6445 6417 6418 8401  d.d...Z.dEd.d...
+00000990: 5a0b 6446 6419 641a 8401 5a0c 6447 641c  Z.dFd.d...Z.dGd.
+000009a0: 641d 8401 5a0d 6448 641f 6420 8401 5a0e  d...Z.dHd.d ..Z.
+000009b0: 6449 6422 6423 8401 5a0f 644a 6424 6425  dId"d#..Z.dJd$d%
+000009c0: 8401 5a10 644b 6427 6428 8401 5a11 644c  ..Z.dKd'd(..Z.dL
+000009d0: 642a 642b 8401 5a12 644d 642c 642d 8401  d*d+..Z.dMd,d-..
+000009e0: 5a13 644e 642e 642f 8401 5a14 644f 6430  Z.dNd.d/..Z.dOd0
+000009f0: 6431 8401 5a15 6450 6433 6434 8401 5a16  d1..Z.dPd3d4..Z.
+00000a00: 6451 6435 6436 8401 5a17 6452 6438 6439  dQd5d6..Z.dRd8d9
+00000a10: 8401 5a18 6453 643c 643d 8401 5a19 643e  ..Z.dSd<d=..Z.d>
+00000a20: 643f 8400 5a1a 643a 5300 2954 da0d 5374  d?..Z.d:S.)T..St
+00000a30: 616e 7a61 5772 6170 7065 7246 5463 0500  anzaWrapperFTc..
+00000a40: 0000 0000 0000 0500 0000 0300 0000 4300  ..............C.
+00000a50: 0000 732c 0000 007c 0172 107c 006a 0064  ..s,...|.r.|.j.d
+00000a60: 0164 028d 0101 007c 0272 1c7c 006a 0183  .d.....|.r.|.j..
+00000a70: 0001 007c 037c 005f 027c 047c 005f 0364  ...|.|._.|.|._.d
+00000a80: 0053 0029 034e 7208 0000 0029 01da 046c  .S.).Nr....)...l
+00000a90: 616e 6729 04da 0864 6f77 6e6c 6f61 64da  ang)...download.
+00000aa0: 1664 6f77 6e6c 6f61 645f 6368 696e 6573  .download_chines
+00000ab0: 655f 6d6f 6465 6cda 1373 686f 756c 645f  e_model..should_
+00000ac0: 7072 696e 745f 7265 7375 6c74 da07 7573  print_result..us
+00000ad0: 655f 6770 7529 0572 1600 0000 5a10 6175  e_gpu).r....Z.au
+00000ae0: 746f 5f64 6f77 6e6c 6f61 645f 656e 5a10  to_download_enZ.
+00000af0: 6175 746f 5f64 6f77 6e6c 6f61 645f 7a68  auto_download_zh
+00000b00: 5a10 7368 6f75 6c64 5f70 7269 6e74 5f6d  Z.should_print_m
+00000b10: 7367 723e 0000 0072 1700 0000 7217 0000  sgr>...r....r...
+00000b20: 0072 1800 0000 7219 0000 0059 0000 0073  .r....r....Y...s
+00000b30: 0c00 0000 0001 0401 0c01 0401 0801 0601  ................
+00000b40: 7a16 5374 616e 7a61 5772 6170 7065 722e  z.StanzaWrapper.
+00000b50: 5f5f 696e 6974 5f5f 7208 0000 00fa 0c74  __init__r......t
+00000b60: 6f6b 656e 697a 652c 706f 7363 0400 0000  okenize,posc....
+00000b70: 0000 0000 0400 0000 0500 0000 4300 0000  ............C...
+00000b80: 7314 0000 0074 006a 017c 017c 027c 0364  s....t.j.|.|.|.d
+00000b90: 018d 0301 0064 0053 0029 024e 2902 da0a  .....d.S.).N)...
+00000ba0: 7072 6f63 6573 736f 7273 da07 7665 7262  processors..verb
+00000bb0: 6f73 6529 0272 1300 0000 723b 0000 0029  ose).r....r;...)
+00000bc0: 0472 1600 0000 723a 0000 0072 4000 0000  .r....r:...r@...
+00000bd0: 7241 0000 0072 1700 0000 7217 0000 0072  rA...r....r....r
+00000be0: 1800 0000 723b 0000 0061 0000 0073 0200  ....r;...a...s..
+00000bf0: 0000 0001 7a16 5374 616e 7a61 5772 6170  ....z.StanzaWrap
+00000c00: 7065 722e 646f 776e 6c6f 6164 da02 7a68  per.download..zh
+00000c10: 6303 0000 0000 0000 0003 0000 0004 0000  c...............
+00000c20: 0043 0000 0073 1200 0000 7400 6a01 7c01  .C...s....t.j.|.
+00000c30: 7c02 6401 8d02 0100 6400 5300 2902 4e29  |.d.....d.S.).N)
+00000c40: 0272 3a00 0000 7241 0000 0029 0272 1300  .r:...rA...).r..
+00000c50: 0000 723b 0000 0029 0372 1600 0000 723a  ..r;...).r....r:
+00000c60: 0000 005a 0676 6572 626f 7372 1700 0000  ...Z.verbosr....
+00000c70: 7217 0000 0072 1800 0000 723c 0000 0064  r....r....r<...d
+00000c80: 0000 0073 0200 0000 0001 7a24 5374 616e  ...s......z$Stan
+00000c90: 7a61 5772 6170 7065 722e 646f 776e 6c6f  zaWrapper.downlo
+00000ca0: 6164 5f63 6869 6e65 7365 5f6d 6f64 656c  ad_chinese_model
+00000cb0: 6302 0000 0000 0000 0002 0000 0002 0000  c...............
+00000cc0: 0043 0000 0073 0a00 0000 7c01 7c00 5f00  .C...s....|.|._.
+00000cd0: 6400 5300 2901 4e29 0172 3e00 0000 2902  d.S.).N).r>...).
+00000ce0: 7216 0000 0072 3e00 0000 7217 0000 0072  r....r>...r....r
+00000cf0: 1700 0000 7218 0000 00da 0773 6574 5f67  ....r......set_g
+00000d00: 7075 6700 0000 7302 0000 0000 017a 1553  pug...s......z.S
+00000d10: 7461 6e7a 6157 7261 7070 6572 2e73 6574  tanzaWrapper.set
+00000d20: 5f67 7075 6301 0000 0000 0000 0001 0000  _gpuc...........
+00000d30: 0001 0000 0043 0000 0073 0600 0000 7c00  .....C...s....|.
+00000d40: 6a00 5300 2901 4e29 0172 3e00 0000 2901  j.S.).N).r>...).
+00000d50: 7216 0000 0072 1700 0000 7217 0000 0072  r....r....r....r
+00000d60: 1800 0000 da07 6765 745f 6770 756a 0000  ......get_gpuj..
+00000d70: 0073 0200 0000 0001 7a15 5374 616e 7a61  .s......z.Stanza
+00000d80: 5772 6170 7065 722e 6765 745f 6770 7563  Wrapper.get_gpuc
+00000d90: 0200 0000 0000 0000 0200 0000 0400 0000  ................
+00000da0: 4300 0000 730e 0000 007c 006a 007c 0164  C...s....|.j.|.d
+00000db0: 0164 028d 0253 0029 034e 7242 0000 0029  .d...S.).NrB...)
+00000dc0: 0172 3a00 0000 2901 720d 0000 0029 0272  .r:...).r....).r
+00000dd0: 1600 0000 721f 0000 0072 1700 0000 7217  ....r....r....r.
+00000de0: 0000 0072 1800 0000 da10 746f 6b65 6e69  ...r......tokeni
+00000df0: 7a65 5f63 6869 6e65 7365 6d00 0000 7302  ze_chinesem...s.
+00000e00: 0000 0000 017a 1e53 7461 6e7a 6157 7261  .....z.StanzaWra
+00000e10: 7070 6572 2e74 6f6b 656e 697a 655f 6368  pper.tokenize_ch
+00000e20: 696e 6573 6572 0d00 0000 6307 0000 0000  ineser....c.....
+00000e30: 0000 000f 0000 0008 0000 0043 0000 0073  ...........C...s
+00000e40: ae00 0000 7400 6a01 7c02 7c03 7c04 7c05  ....t.j.|.|.|.|.
+00000e50: 7c06 7c00 6a02 6401 8d06 7d07 7c07 7c01  |.|.j.d...}.|.|.
+00000e60: 8301 7d08 6700 7d09 7884 7403 7c08 6a04  ..}.g.}.x.t.|.j.
+00000e70: 8301 4400 5d76 5c02 7d0a 7d0b 7c00 6a05  ..D.]v\.}.}.|.j.
+00000e80: 726c 7406 6402 7c0a 6403 1700 9b00 6404  rlt.d.|.d.....d.
+00000e90: 9d03 8301 0100 7406 6405 6406 8400 7c0b  ......t.d.d...|.
+00000ea0: 6a07 4400 8301 6407 6408 6901 8e01 0100  j.D...d.d.i.....
+00000eb0: 6700 7d0c 782a 7c0b 6a07 4400 5d20 7d0d  g.}.x*|.j.D.] }.
+00000ec0: 7408 7c0d 6a09 8301 7c0d 6a0a 6409 9c02  t.|.j...|.j.d...
+00000ed0: 7d0e 7c0c 6a0b 7c0e 8301 0100 7178 5700  }.|.j.|.....qxW.
+00000ee0: 7c09 6a0b 7c0c 8301 0100 7130 5700 7c09  |.j.|.....q0W.|.
+00000ef0: 5300 290a 4e29 0672 3a00 0000 7240 0000  S.).N).r:...r@..
+00000f00: 00da 1274 6f6b 656e 697a 655f 6e6f 5f73  ...tokenize_no_s
+00000f10: 7370 6c69 74da 1574 6f6b 656e 697a 655f  split..tokenize_
+00000f20: 7072 6574 6f6b 656e 697a 6564 7241 0000  pretokenizedrA..
+00000f30: 0072 3e00 0000 7a10 3d3d 3d3d 3d3d 2053  .r>...z.====== S
+00000f40: 656e 7465 6e63 6520 7223 0000 007a 0f20  entence r#...z. 
+00000f50: 746f 6b65 6e73 203d 3d3d 3d3d 3d3d 6301  tokens =======c.
+00000f60: 0000 0000 0000 0002 0000 0006 0000 0053  ...............S
+00000f70: 0000 0073 2000 0000 6700 7c00 5d18 7d01  ...s ...g.|.].}.
+00000f80: 6400 7c01 6a00 9b00 6401 7c01 6a01 9b00  d.|.j...d.|.j...
+00000f90: 9d04 9102 7104 5300 2902 7a04 6964 3a20  ....q.S.).z.id: 
+00000fa0: 7a07 0974 6578 743a 2029 02da 0269 6472  z..text: )...idr
+00000fb0: 1f00 0000 2902 da02 2e30 721d 0000 0072  ....)....0r....r
+00000fc0: 1700 0000 7217 0000 0072 1800 0000 fa0a  ....r....r......
+00000fd0: 3c6c 6973 7463 6f6d 703e 7800 0000 7302  <listcomp>x...s.
+00000fe0: 0000 0006 007a 2a53 7461 6e7a 6157 7261  .....z*StanzaWra
+00000ff0: 7070 6572 2e74 6f6b 656e 697a 652e 3c6c  pper.tokenize.<l
+00001000: 6f63 616c 733e 2e3c 6c69 7374 636f 6d70  ocals>.<listcomp
+00001010: 3eda 0373 6570 722d 0000 0029 0272 4800  >..sepr-...).rH.
+00001020: 0000 721f 0000 0029 0c72 1300 0000 7205  ..r....).r....r.
+00001030: 0000 0072 3e00 0000 da09 656e 756d 6572  ...r>.....enumer
+00001040: 6174 65da 0973 656e 7465 6e63 6573 723d  ate..sentencesr=
+00001050: 0000 00da 0570 7269 6e74 da06 746f 6b65  .....print..toke
+00001060: 6e73 da03 7374 7272 4800 0000 721f 0000  ns..strrH...r...
+00001070: 0072 1e00 0000 290f 7216 0000 0072 1f00  .r....).r....r..
+00001080: 0000 723a 0000 0072 4000 0000 7246 0000  ..r:...r@...rF..
+00001090: 0072 4700 0000 7241 0000 00da 036e 6c70  .rG...rA.....nlp
+000010a0: da03 646f 63da 0d6c 6973 745f 7365 6e74  ..doc..list_sent
+000010b0: 656e 6365 da01 6972 1c00 0000 724f 0000  ence..ir....rO..
+000010c0: 0072 1d00 0000 722a 0000 0072 1700 0000  .r....r*...r....
+000010d0: 7217 0000 0072 1800 0000 720d 0000 0070  r....r....r....p
+000010e0: 0000 0073 1c00 0000 0001 1801 0801 0402  ...s............
+000010f0: 1401 0601 1401 1a01 0401 0c02 0801 0a02  ................
+00001100: 0e01 0e01 7a16 5374 616e 7a61 5772 6170  ....z.StanzaWrap
+00001110: 7065 722e 746f 6b65 6e69 7a65 6307 0000  per.tokenizec...
+00001120: 0000 0000 000c 0000 0008 0000 0043 0000  .............C..
+00001130: 0073 7400 0000 7400 6a01 7c02 7c03 7c04  .st...t.j.|.|.|.
+00001140: 7c05 7c06 7c00 6a02 6401 8d06 7d07 7c07  |.|.|.j.d...}.|.
+00001150: 7c01 8301 7d08 6700 7d09 784a 7403 7c08  |...}.g.}.xJt.|.
+00001160: 6a04 8301 4400 5d3c 5c02 7d0a 7d0b 7c00  j...D.]<\.}.}.|.
+00001170: 6a05 7260 7406 6402 7c0a 6403 1700 9b00  j.r`t.d.|.d.....
+00001180: 6404 9d03 8301 0100 7406 7c0b 6a07 6405  d.......t.|.j.d.
+00001190: 6406 8d02 0100 7c09 6a08 7c0b 6a07 8301  d.....|.j.|.j...
+000011a0: 0100 7130 5700 7c09 5300 2907 4e29 0672  ..q0W.|.S.).N).r
+000011b0: 3a00 0000 7240 0000 0072 4600 0000 7247  :...r@...rF...rG
+000011c0: 0000 0072 4100 0000 723e 0000 007a 103d  ...rA...r>...z.=
+000011d0: 3d3d 3d3d 3d20 5365 6e74 656e 6365 2072  ===== Sentence r
+000011e0: 2300 0000 7a0f 2074 6f6b 656e 7320 3d3d  #...z. tokens ==
+000011f0: 3d3d 3d3d 3d72 2d00 0000 2901 724b 0000  =====r-...).rK..
+00001200: 0029 0972 1300 0000 7205 0000 0072 3e00  .).r....r....r>.
+00001210: 0000 724c 0000 0072 4d00 0000 723d 0000  ..rL...rM...r=..
+00001220: 0072 4e00 0000 721f 0000 0072 1e00 0000  .rN...r....r....
+00001230: 290c 7216 0000 0072 1f00 0000 723a 0000  ).r....r....r:..
+00001240: 0072 4000 0000 7246 0000 0072 4700 0000  .r@...rF...rG...
+00001250: 7241 0000 0072 5100 0000 7252 0000 0072  rA...rQ...rR...r
+00001260: 5300 0000 7254 0000 0072 1c00 0000 7217  S...rT...r....r.
+00001270: 0000 0072 1700 0000 7218 0000 00da 1174  ...r....r......t
+00001280: 6f6b 656e 697a 655f 7365 6e74 656e 6365  okenize_sentence
+00001290: 8300 0000 7312 0000 0000 0118 0108 0104  ....s...........
+000012a0: 0114 0106 0114 010e 0110 017a 1f53 7461  ...........z.Sta
+000012b0: 6e7a 6157 7261 7070 6572 2e74 6f6b 656e  nzaWrapper.token
+000012c0: 697a 655f 7365 6e74 656e 6365 6307 0000  ize_sentencec...
+000012d0: 0000 0000 000f 0000 0008 0000 0043 0000  .............C..
+000012e0: 0073 aa00 0000 7400 6a01 7c02 7c03 7c04  .s....t.j.|.|.|.
+000012f0: 7c05 7c06 7c00 6a02 6401 8d06 7d07 7c07  |.|.|.j.d...}.|.
+00001300: 7c01 8301 7d08 6700 7d09 7880 7403 7c08  |...}.g.}.x.t.|.
+00001310: 6a04 8301 4400 5d72 5c02 7d0a 7d0b 7c00  j...D.]r\.}.}.|.
+00001320: 6a05 726c 7406 6402 7c0a 6403 1700 9b00  j.rlt.d.|.d.....
+00001330: 6404 9d03 8301 0100 7406 6405 6406 8400  d.......t.d.d...
+00001340: 7c0b 6a07 4400 8301 6407 6408 6901 8e01  |.j.D...d.d.i...
+00001350: 0100 6700 7d0c 7826 7c0b 6a07 4400 5d1c  ..g.}.x&|.j.D.].
+00001360: 7d0d 7c0d 6a08 7c0d 6a09 6409 9c02 7d0e  }.|.j.|.j.d...}.
+00001370: 7c0c 6a0a 7c0e 8301 0100 7178 5700 7c09  |.j.|.....qxW.|.
+00001380: 6a0a 7c0c 8301 0100 7130 5700 7c09 5300  j.|.....q0W.|.S.
+00001390: 290a 4e29 0672 3a00 0000 7240 0000 0072  ).N).r:...r@...r
+000013a0: 4600 0000 7247 0000 0072 4100 0000 723e  F...rG...rA...r>
+000013b0: 0000 007a 103d 3d3d 3d3d 3d20 5365 6e74  ...z.====== Sent
+000013c0: 656e 6365 2072 2300 0000 7a0f 2074 6f6b  ence r#...z. tok
+000013d0: 656e 7320 3d3d 3d3d 3d3d 3d63 0100 0000  ens =======c....
+000013e0: 0000 0000 0200 0000 0600 0000 5300 0000  ............S...
+000013f0: 7320 0000 0067 007c 005d 187d 0164 007c  s ...g.|.].}.d.|
+00001400: 016a 009b 0064 017c 016a 019b 009d 0491  .j...d.|.j......
+00001410: 0271 0453 0029 027a 0469 643a 207a 0709  .q.S.).z.id: z..
+00001420: 7465 7874 3a20 2902 7248 0000 0072 1f00  text: ).rH...r..
+00001430: 0000 2902 7249 0000 0072 1d00 0000 7217  ..).rI...r....r.
+00001440: 0000 0072 1700 0000 7218 0000 0072 4a00  ...r....r....rJ.
+00001450: 0000 9500 0000 7302 0000 0006 007a 2f53  ......s......z/S
+00001460: 7461 6e7a 6157 7261 7070 6572 2e74 6f6b  tanzaWrapper.tok
+00001470: 656e 697a 655f 6c69 7374 2e3c 6c6f 6361  enize_list.<loca
+00001480: 6c73 3e2e 3c6c 6973 7463 6f6d 703e 724b  ls>.<listcomp>rK
+00001490: 0000 0072 2d00 0000 2902 7248 0000 0072  ...r-...).rH...r
+000014a0: 1f00 0000 290b 7213 0000 0072 0500 0000  ....).r....r....
+000014b0: 723e 0000 0072 4c00 0000 724d 0000 0072  r>...rL...rM...r
+000014c0: 3d00 0000 724e 0000 0072 4f00 0000 7248  =...rN...rO...rH
+000014d0: 0000 0072 1f00 0000 721e 0000 0029 0f72  ...r....r....).r
+000014e0: 1600 0000 5a0b 6c69 7374 5f74 6f6b 656e  ....Z.list_token
+000014f0: 7372 3a00 0000 7240 0000 0072 4600 0000  sr:...r@...rF...
+00001500: 7247 0000 0072 4100 0000 7251 0000 0072  rG...rA...rQ...r
+00001510: 5200 0000 7253 0000 0072 5400 0000 721c  R...rS...rT...r.
+00001520: 0000 0072 4f00 0000 721d 0000 0072 2a00  ...rO...r....r*.
+00001530: 0000 7217 0000 0072 1700 0000 7218 0000  ..r....r....r...
+00001540: 00da 0d74 6f6b 656e 697a 655f 6c69 7374  ...tokenize_list
+00001550: 8e00 0000 731c 0000 0000 0118 0108 0104  ....s...........
+00001560: 0114 0106 0114 011a 0104 010c 0204 010a  ................
+00001570: 020e 010e 017a 1b53 7461 6e7a 6157 7261  .....z.StanzaWra
+00001580: 7070 6572 2e74 6f6b 656e 697a 655f 6c69  pper.tokenize_li
+00001590: 7374 6303 0000 0000 0000 000c 0000 0006  stc.............
+000015a0: 0000 0043 0000 0073 ae00 0000 6401 6402  ...C...s....d.d.
+000015b0: 6901 7d03 7400 6a01 6403 7c03 7c02 7c00  i.}.t.j.d.|.|.|.
+000015c0: 6a02 6404 8d04 7d04 7c04 7c01 8301 7d05  j.d...}.|.|...}.
+000015d0: 6700 7d06 7880 7403 7c05 6a04 8301 4400  g.}.x.t.|.j...D.
+000015e0: 5d72 5c02 7d07 7d08 7c00 6a05 7270 7406  ]r\.}.}.|.j.rpt.
+000015f0: 6405 7c07 6406 1700 9b00 6407 9d03 8301  d.|.d.....d.....
+00001600: 0100 7406 6408 6409 8400 7c08 6a07 4400  ..t.d.d...|.j.D.
+00001610: 8301 640a 640b 6901 8e01 0100 6700 7d09  ..d.d.i.....g.}.
+00001620: 7826 7c08 6a07 4400 5d1c 7d0a 7c0a 6a08  x&|.j.D.].}.|.j.
+00001630: 7c0a 6a09 640c 9c02 7d0b 7c09 6a0a 7c0b  |.j.d...}.|.j.|.
+00001640: 8301 0100 717c 5700 7c06 6a0a 7c09 8301  ....q|W.|.j.|...
+00001650: 0100 7134 5700 7c06 5300 290d 4e72 0d00  ..q4W.|.S.).Nr..
+00001660: 0000 5a05 7370 6163 7972 0800 0000 2904  ..Z.spacyr....).
+00001670: 723a 0000 0072 4000 0000 7241 0000 0072  r:...r@...rA...r
+00001680: 3e00 0000 7a10 3d3d 3d3d 3d3d 2053 656e  >...z.====== Sen
+00001690: 7465 6e63 6520 7223 0000 007a 0f20 746f  tence r#...z. to
+000016a0: 6b65 6e73 203d 3d3d 3d3d 3d3d 6301 0000  kens =======c...
+000016b0: 0000 0000 0002 0000 0006 0000 0053 0000  .............S..
+000016c0: 0073 2000 0000 6700 7c00 5d18 7d01 6400  .s ...g.|.].}.d.
+000016d0: 7c01 6a00 9b00 6401 7c01 6a01 9b00 9d04  |.j...d.|.j.....
+000016e0: 9102 7104 5300 2902 7a04 6964 3a20 7a07  ..q.S.).z.id: z.
+000016f0: 0974 6578 743a 2029 0272 4800 0000 721f  .text: ).rH...r.
+00001700: 0000 0029 0272 4900 0000 721d 0000 0072  ...).rI...r....r
+00001710: 1700 0000 7217 0000 0072 1800 0000 724a  ....r....r....rJ
+00001720: 0000 00a8 0000 0073 0200 0000 0600 7a33  .......s......z3
+00001730: 5374 616e 7a61 5772 6170 7065 722e 746f  StanzaWrapper.to
+00001740: 6b65 6e69 7a65 5f62 795f 7370 6163 792e  kenize_by_spacy.
+00001750: 3c6c 6f63 616c 733e 2e3c 6c69 7374 636f  <locals>.<listco
+00001760: 6d70 3e72 4b00 0000 722d 0000 0029 0272  mp>rK...r-...).r
+00001770: 4800 0000 721f 0000 0029 0b72 1300 0000  H...r....).r....
+00001780: 7205 0000 0072 3e00 0000 724c 0000 0072  r....r>...rL...r
+00001790: 4d00 0000 723d 0000 0072 4e00 0000 724f  M...r=...rN...rO
+000017a0: 0000 0072 4800 0000 721f 0000 0072 1e00  ...rH...r....r..
+000017b0: 0000 290c 7216 0000 0072 1f00 0000 7241  ..).r....r....rA
+000017c0: 0000 0072 4000 0000 7251 0000 0072 5200  ...r@...rQ...rR.
+000017d0: 0000 7253 0000 0072 5400 0000 721c 0000  ..rS...rT...r...
+000017e0: 0072 4f00 0000 721d 0000 0072 2a00 0000  .rO...r....r*...
+000017f0: 7217 0000 0072 1700 0000 7218 0000 00da  r....r....r.....
+00001800: 1174 6f6b 656e 697a 655f 6279 5f73 7061  .tokenize_by_spa
+00001810: 6379 a000 0000 731e 0000 0000 0108 0114  cy....s.........
+00001820: 0108 0104 0114 0106 0114 011a 0104 010c  ................
+00001830: 0204 010a 020e 010e 017a 1f53 7461 6e7a  .........z.Stanz
+00001840: 6157 7261 7070 6572 2e74 6f6b 656e 697a  aWrapper.tokeniz
+00001850: 655f 6279 5f73 7061 6379 fa0c 746f 6b65  e_by_spacy..toke
+00001860: 6e69 7a65 2c6d 7774 6305 0000 0000 0000  nize,mwtc.......
+00001870: 000c 0000 0009 0000 0043 0000 0073 a800  .........C...s..
+00001880: 0000 7400 6a01 7c02 7c03 7c04 7c00 6a02  ..t.j.|.|.|.|.j.
+00001890: 6401 8d04 7d05 7c05 7c01 8301 7d06 6700  d...}.|.|...}.g.
+000018a0: 7d07 7882 7c06 6a03 4400 5d78 7d08 6700  }.x.|.j.D.]x}.g.
+000018b0: 7d09 7864 7c08 6a04 4400 5d5a 7d0a 7c00  }.xd|.j.D.]Z}.|.
+000018c0: 6a05 726a 7406 6402 7c0a 6a07 9b00 6403  j.rjt.d.|.j...d.
+000018d0: 6404 6a08 6405 6406 8400 7c0a 6a09 4400  d.j.d.d...|.j.D.
+000018e0: 8301 8301 9b00 9d04 8301 0100 7c0a 6a07  ............|.j.
+000018f0: 6404 6a08 6407 6406 8400 7c0a 6a09 4400  d.j.d.d...|.j.D.
+00001900: 8301 8301 6408 9c02 7d0b 7c09 6a0a 7c0b  ....d...}.|.j.|.
+00001910: 8301 0100 7138 5700 7c07 6a0a 7c09 8301  ....q8W.|.j.|...
+00001920: 0100 7128 5700 7c07 5300 2909 4e29 0472  ..q(W.|.S.).N).r
+00001930: 3a00 0000 7240 0000 0072 4100 0000 723e  :...r@...rA...r>
+00001940: 0000 007a 0774 6f6b 656e 3a20 7a08 0977  ...z.token: z..w
+00001950: 6f72 6473 3a20 7a02 2c20 6301 0000 0000  ords: z., c.....
+00001960: 0000 0002 0000 0003 0000 0053 0000 0073  ...........S...s
+00001970: 1200 0000 6700 7c00 5d0a 7d01 7c01 6a00  ....g.|.].}.|.j.
+00001980: 9102 7104 5300 7217 0000 0029 0172 1f00  ..q.S.r....).r..
+00001990: 0000 2902 7249 0000 00da 0477 6f72 6472  ..).rI.....wordr
+000019a0: 1700 0000 7217 0000 0072 1800 0000 724a  ....r....r....rJ
+000019b0: 0000 00bc 0000 0073 0200 0000 0600 7a2c  .......s......z,
 000019c0: 5374 616e 7a61 5772 6170 7065 722e 6d77  StanzaWrapper.mw
-000019d0: 745f 6578 7061 6e64 fa1b 746f 6b65 6e69  t_expand..tokeni
-000019e0: 7a65 2c6c 656d 6d61 2c70 6f73 2c64 6570  ze,lemma,pos,dep
-000019f0: 7061 7273 6563 0600 0000 0000 0000 0600  parsec..........
-00001a00: 0000 0700 0000 4300 0000 7314 0000 007c  ......C...s....|
-00001a10: 006a 007c 017c 027c 037c 047c 0564 018d  .j.|.|.|.|.|.d..
-00001a20: 0553 0029 024e 2902 7240 0000 0072 4400  .S.).N).r@...rD.
-00001a30: 0000 2901 da03 7461 6729 0672 1600 0000  ..)...tag).r....
-00001a40: 721f 0000 0072 3a00 0000 723f 0000 0072  r....r:...r?...r
-00001a50: 4000 0000 7244 0000 0072 1700 0000 7217  @...rD...r....r.
-00001a60: 0000 0072 1800 0000 da0b 7461 675f 6368  ...r......tag_ch
-00001a70: 696e 6573 65be 0000 0073 0200 0000 0001  inese....s......
-00001a80: 7a19 5374 616e 7a61 5772 6170 7065 722e  z.StanzaWrapper.
-00001a90: 7461 675f 6368 696e 6573 65fa 1074 6f6b  tag_chinese..tok
-00001aa0: 656e 697a 652c 6d77 742c 706f 7363 0600  enize,mwt,posc..
-00001ab0: 0000 0000 0000 0c00 0000 0700 0000 4300  ..............C.
-00001ac0: 0000 738c 0000 0074 006a 017c 027c 037c  ..s....t.j.|.|.|
-00001ad0: 047c 0564 018d 047d 067c 067c 0183 017d  .|.d...}.|.|...}
-00001ae0: 077c 006a 0272 3a74 0364 0264 0384 007c  .|.j.r:t.d.d...|
-00001af0: 076a 0444 0083 0164 0464 0569 018e 0101  .j.D...d.d.i....
-00001b00: 0067 007d 0878 487c 076a 0444 005d 3e7d  .g.}.xH|.j.D.]>}
-00001b10: 0978 387c 096a 0544 005d 2e7d 0a7c 0a6a  .x8|.j.D.].}.|.j
-00001b20: 067c 0a6a 077c 0a6a 087c 0a6a 0972 6e7c  .|.j.|.j.|.j.rn|
-00001b30: 0a6a 096e 0264 0664 079c 047d 0b7c 086a  .j.n.d.d...}.|.j
-00001b40: 0a7c 0b83 0101 0071 5257 0071 4657 007c  .|.....qRW.qFW.|
-00001b50: 0853 0029 084e 2904 723a 0000 0072 3f00  .S.).N).r:...r?.
-00001b60: 0000 7240 0000 0072 4400 0000 6301 0000  ..r@...rD...c...
-00001b70: 0000 0000 0003 0000 000b 0000 0053 0000  .............S..
-00001b80: 0073 4600 0000 6700 7c00 5d3e 7d01 7c01  .sF...g.|.]>}.|.
-00001b90: 6a00 4400 5d32 7d02 6400 7c02 6a01 9b00  j.D.]2}.d.|.j...
-00001ba0: 6401 7c02 6a02 9b00 6402 7c02 6a03 9b00  d.|.j...d.|.j...
-00001bb0: 6403 7c02 6a04 7238 7c02 6a04 6e02 6404  d.|.j.r8|.j.n.d.
-00001bc0: 9b00 9d08 9103 710e 7104 5300 2905 7a06  ......q.q.S.).z.
-00001bd0: 776f 7264 3a20 7a07 0975 706f 733a 207a  word: z..upos: z
-00001be0: 0709 7870 6f73 3a20 7a08 0966 6561 7473  ..xpos: z..feats
-00001bf0: 3a20 da01 5f29 0572 5700 0000 721f 0000  : .._).rW...r...
-00001c00: 00da 0475 706f 73da 0478 706f 73da 0566  ...upos..xpos..f
-00001c10: 6561 7473 2903 7246 0000 00da 0473 656e  eats).rF.....sen
-00001c20: 7472 5500 0000 7217 0000 0072 1700 0000  trU...r....r....
-00001c30: 7218 0000 0072 4700 0000 c600 0000 7302  r....rG.......s.
-00001c40: 0000 0006 017a 2553 7461 6e7a 6157 7261  .....z%StanzaWra
-00001c50: 7070 6572 2e74 6167 2e3c 6c6f 6361 6c73  pper.tag.<locals
-00001c60: 3e2e 3c6c 6973 7463 6f6d 703e 7248 0000  >.<listcomp>rH..
-00001c70: 0072 2d00 0000 725d 0000 0029 0472 5500  .r-...r]...).rU.
-00001c80: 0000 725e 0000 0072 5f00 0000 7260 0000  ..r^...r_...r`..
-00001c90: 0029 0b72 1300 0000 7205 0000 0072 3d00  .).r....r....r=.
-00001ca0: 0000 724b 0000 0072 4a00 0000 7257 0000  ..rK...rJ...rW..
-00001cb0: 0072 1f00 0000 725e 0000 0072 5f00 0000  .r....r^...r_...
-00001cc0: 7260 0000 0072 1e00 0000 290c 7216 0000  r`...r....).r...
-00001cd0: 0072 1f00 0000 723a 0000 0072 3f00 0000  .r....r:...r?...
-00001ce0: 7240 0000 0072 4400 0000 724d 0000 0072  r@...rD...rM...r
-00001cf0: 4e00 0000 7229 0000 0072 6100 0000 7255  N...r)...ra...rU
-00001d00: 0000 0072 2a00 0000 7217 0000 0072 1700  ...r*...r....r..
-00001d10: 0000 7218 0000 0072 5a00 0000 c100 0000  ..r....rZ.......
-00001d20: 731e 0000 0000 0112 0108 0106 0102 0106  s...............
-00001d30: 0112 0104 010c 010c 0204 0104 0104 0114  ................
-00001d40: 0212 017a 1153 7461 6e7a 6157 7261 7070  ...z.StanzaWrapp
-00001d50: 6572 2e74 6167 6305 0000 0000 0000 0005  er.tagc.........
-00001d60: 0000 0006 0000 0043 0000 0073 1200 0000  .......C...s....
-00001d70: 7c00 6a00 7c01 7c02 7c03 7c04 6401 8d04  |.j.|.|.|.|.d...
-00001d80: 5300 2902 4e29 0172 4000 0000 2901 da10  S.).N).r@...)...
-00001d90: 7061 7273 655f 6465 7065 6e64 656e 6379  parse_dependency
-00001da0: 2905 7216 0000 0072 1f00 0000 723a 0000  ).r....r....r:..
-00001db0: 0072 3f00 0000 7240 0000 0072 1700 0000  .r?...r@...r....
-00001dc0: 7217 0000 0072 1800 0000 da18 7061 7273  r....r......pars
-00001dd0: 655f 6465 7065 6e64 656e 6379 5f63 6869  e_dependency_chi
-00001de0: 6e65 7365 d400 0000 7302 0000 0000 017a  nese....s......z
-00001df0: 2653 7461 6e7a 6157 7261 7070 6572 2e70  &StanzaWrapper.p
-00001e00: 6172 7365 5f64 6570 656e 6465 6e63 795f  arse_dependency_
-00001e10: 6368 696e 6573 65fa 1f74 6f6b 656e 697a  chinese..tokeniz
-00001e20: 652c 6d77 742c 706f 732c 6c65 6d6d 612c  e,mwt,pos,lemma,
-00001e30: 6465 7070 6172 7365 6305 0000 0000 0000  depparsec.......
-00001e40: 000b 0000 0008 0000 0043 0000 0073 9e00  .........C...s..
-00001e50: 0000 7400 6a01 7c02 7c03 7c04 6401 8d03  ..t.j.|.|.|.d...
-00001e60: 7d05 7c05 7c01 8301 7d06 7c00 6a02 7238  }.|.|...}.|.j.r8
-00001e70: 7403 6402 6403 8400 7c06 6a04 4400 8301  t.d.d...|.j.D...
-00001e80: 6404 6405 6901 8e01 0100 6700 7d07 785c  d.d.i.....g.}.x\
-00001e90: 7c06 6a04 4400 5d52 7d08 784c 7c08 6a05  |.j.D.]R}.xL|.j.
-00001ea0: 4400 5d42 7d09 7c09 6a06 7c09 6a07 7c09  D.]B}.|.j.|.j.|.
-00001eb0: 6a08 7c09 6a08 6406 6b04 727c 7c08 6a05  j.|.j.d.k.r||.j.
-00001ec0: 7c09 6a08 6407 1800 1900 6a07 6e02 6408  |.j.d.....j.n.d.
-00001ed0: 7c09 6a09 6409 9c05 7d0a 7c07 6a0a 7c0a  |.j.d...}.|.j.|.
-00001ee0: 8301 0100 7150 5700 7144 5700 7c07 5300  ....qPW.qDW.|.S.
-00001ef0: 290a 4e29 0372 3a00 0000 723f 0000 0072  ).N).r:...r?...r
-00001f00: 4000 0000 6301 0000 0000 0000 0003 0000  @...c...........
-00001f10: 000d 0000 0053 0000 0073 5e00 0000 6700  .....S...s^...g.
-00001f20: 7c00 5d56 7d01 7c01 6a00 4400 5d4a 7d02  |.]V}.|.j.D.]J}.
-00001f30: 6400 7c02 6a01 9b00 6401 7c02 6a02 9b00  d.|.j...d.|.j...
-00001f40: 6402 7c02 6a03 9b00 6403 7c02 6a03 6404  d.|.j...d.|.j.d.
-00001f50: 6b04 7248 7c01 6a00 7c02 6a03 6405 1800  k.rH|.j.|.j.d...
-00001f60: 1900 6a02 6e02 6406 9b00 6407 7c02 6a04  ..j.n.d...d.|.j.
-00001f70: 9b00 9d0a 9103 710e 7104 5300 2908 7a04  ......q.q.S.).z.
-00001f80: 6964 3a20 7a07 0977 6f72 643a 207a 0a09  id: z..word: z..
-00001f90: 6865 6164 2069 643a 207a 0709 6865 6164  head id: z..head
-00001fa0: 3a20 7201 0000 0072 2300 0000 da04 726f  : r....r#.....ro
-00001fb0: 6f74 7a09 0964 6570 7265 6c3a 2029 0572  otz..deprel: ).r
-00001fc0: 5700 0000 7245 0000 0072 1f00 0000 da04  W...rE...r......
-00001fd0: 6865 6164 da06 6465 7072 656c 2903 7246  head..deprel).rF
-00001fe0: 0000 0072 6100 0000 7255 0000 0072 1700  ...ra...rU...r..
-00001ff0: 0000 7217 0000 0072 1800 0000 7247 0000  ..r....r....rG..
-00002000: 00dc 0000 0073 0200 0000 0601 7a32 5374  .....s......z2St
-00002010: 616e 7a61 5772 6170 7065 722e 7061 7273  anzaWrapper.pars
-00002020: 655f 6465 7065 6e64 656e 6379 2e3c 6c6f  e_dependency.<lo
-00002030: 6361 6c73 3e2e 3c6c 6973 7463 6f6d 703e  cals>.<listcomp>
-00002040: 7248 0000 0072 2d00 0000 7201 0000 0072  rH...r-...r....r
-00002050: 2300 0000 7265 0000 0029 0572 4500 0000  #...re...).rE...
-00002060: 721f 0000 007a 0768 6561 6420 6964 7266  r....z.head idrf
-00002070: 0000 0072 6700 0000 290b 7213 0000 0072  ...rg...).r....r
-00002080: 0500 0000 723d 0000 0072 4b00 0000 724a  ....r=...rK...rJ
-00002090: 0000 0072 5700 0000 7245 0000 0072 1f00  ...rW...rE...r..
-000020a0: 0000 7266 0000 0072 6700 0000 721e 0000  ..rf...rg...r...
-000020b0: 0029 0b72 1600 0000 721f 0000 0072 3a00  .).r....r....r:.
-000020c0: 0000 723f 0000 0072 4000 0000 724d 0000  ..r?...r@...rM..
-000020d0: 0072 4e00 0000 7229 0000 0072 6100 0000  .rN...r)...ra...
-000020e0: 7255 0000 0072 2a00 0000 7217 0000 0072  rU...r*...r....r
-000020f0: 1700 0000 7218 0000 0072 6200 0000 d700  ....r....rb.....
-00002100: 0000 7320 0000 0000 0110 0108 0106 0102  ..s ............
-00002110: 0106 0112 0104 010c 010c 0204 0104 0104  ................
-00002120: 011e 010a 0212 017a 1e53 7461 6e7a 6157  .......z.StanzaW
-00002130: 7261 7070 6572 2e70 6172 7365 5f64 6570  rapper.parse_dep
-00002140: 656e 6465 6e63 79fa 0c74 6f6b 656e 697a  endency..tokeniz
-00002150: 652c 6e65 7263 0600 0000 0000 0000 0b00  e,nerc..........
-00002160: 0000 0600 0000 4300 0000 736a 0000 0074  ......C...sj...t
-00002170: 006a 017c 027c 037c 047c 0564 018d 047d  .j.|.|.|.|.d...}
-00002180: 067c 067c 0183 017d 077c 006a 0272 3a74  .|.|...}.|.j.r:t
-00002190: 0364 0264 0384 007c 076a 0444 0083 0164  .d.d...|.j.D...d
-000021a0: 0464 0569 018e 0101 0067 007d 0878 267c  .d.i.....g.}.x&|
-000021b0: 076a 0444 005d 1c7d 097c 096a 057c 096a  .j.D.].}.|.j.|.j
-000021c0: 0664 069c 027d 0a7c 086a 077c 0a83 0101  .d...}.|.j.|....
-000021d0: 0071 4657 007c 0853 0029 074e 2904 723a  .qFW.|.S.).N).r:
-000021e0: 0000 0072 3f00 0000 7240 0000 0072 4400  ...r?...r@...rD.
-000021f0: 0000 6301 0000 0000 0000 0002 0000 0006  ..c.............
-00002200: 0000 0053 0000 0073 2000 0000 6700 7c00  ...S...s ...g.|.
-00002210: 5d18 7d01 6400 7c01 6a00 9b00 6401 7c01  ].}.d.|.j...d.|.
-00002220: 6a01 9b00 9d04 9102 7104 5300 2902 7a08  j.......q.S.).z.
-00002230: 656e 7469 7479 3a20 7a07 0974 7970 653a  entity: z..type:
-00002240: 2029 0272 1f00 0000 da04 7479 7065 2902   ).r......type).
-00002250: 7246 0000 00da 0365 6e74 7217 0000 0072  rF.....entr....r
-00002260: 1700 0000 7218 0000 0072 4700 0000 ef00  ....r....rG.....
-00002270: 0000 7302 0000 0006 007a 2553 7461 6e7a  ..s......z%Stanz
-00002280: 6157 7261 7070 6572 2e6e 6572 2e3c 6c6f  aWrapper.ner.<lo
-00002290: 6361 6c73 3e2e 3c6c 6973 7463 6f6d 703e  cals>.<listcomp>
-000022a0: 7248 0000 0072 2d00 0000 2902 5a06 656e  rH...r-...).Z.en
-000022b0: 7469 7479 7269 0000 0029 0872 1300 0000  tityri...).r....
-000022c0: 7205 0000 0072 3d00 0000 724b 0000 005a  r....r=...rK...Z
-000022d0: 0465 6e74 7372 1f00 0000 7269 0000 0072  .entsr....ri...r
-000022e0: 1e00 0000 290b 7216 0000 0072 1f00 0000  ....).r....r....
-000022f0: 723a 0000 0072 3f00 0000 7240 0000 0072  r:...r?...r@...r
-00002300: 4400 0000 724d 0000 0072 4e00 0000 7229  D...rM...rN...r)
-00002310: 0000 0072 6a00 0000 722a 0000 0072 1700  ...rj...r*...r..
-00002320: 0000 7217 0000 0072 1800 0000 720f 0000  ..r....r....r...
-00002330: 00eb 0000 0073 1400 0000 0001 1201 0801  .....s..........
-00002340: 0601 1a01 0401 0c02 0401 0a02 0e01 7a11  ..............z.
-00002350: 5374 616e 7a61 5772 6170 7065 722e 6e65  StanzaWrapper.ne
-00002360: 7263 0600 0000 0000 0000 0600 0000 0700  rc..............
-00002370: 0000 4300 0000 7314 0000 007c 006a 007c  ..C...s....|.j.|
-00002380: 017c 027c 037c 047c 0564 018d 0553 0029  .|.|.|.|.d...S.)
-00002390: 024e 2902 7240 0000 0072 4400 0000 2901  .N).r@...rD...).
-000023a0: 720f 0000 0029 0672 1600 0000 721f 0000  r....).r....r...
-000023b0: 0072 3a00 0000 723f 0000 0072 4000 0000  .r:...r?...r@...
-000023c0: 7244 0000 0072 1700 0000 7217 0000 0072  rD...r....r....r
-000023d0: 1800 0000 da0b 6e65 725f 6368 696e 6573  ......ner_chines
-000023e0: 65f9 0000 0073 0200 0000 0001 7a19 5374  e....s......z.St
-000023f0: 616e 7a61 5772 6170 7065 722e 6e65 725f  anzaWrapper.ner_
-00002400: 6368 696e 6573 6563 0500 0000 0000 0000  chinesec........
-00002410: 0500 0000 0600 0000 4300 0000 7312 0000  ........C...s...
-00002420: 007c 006a 007c 017c 027c 037c 0464 018d  .|.j.|.|.|.|.d..
-00002430: 0453 0029 024e 2901 7240 0000 0029 01da  .S.).N).r@...)..
-00002440: 096e 6572 5f74 6f6b 656e 2905 7216 0000  .ner_token).r...
-00002450: 0072 1f00 0000 723a 0000 0072 3f00 0000  .r....r:...r?...
-00002460: 7240 0000 0072 1700 0000 7217 0000 0072  r@...r....r....r
-00002470: 1800 0000 da11 6e65 725f 746f 6b65 6e5f  ......ner_token_
-00002480: 6368 696e 6573 65fc 0000 0073 0200 0000  chinese....s....
-00002490: 0001 7a1f 5374 616e 7a61 5772 6170 7065  ..z.StanzaWrappe
-000024a0: 722e 6e65 725f 746f 6b65 6e5f 6368 696e  r.ner_token_chin
-000024b0: 6573 6563 0500 0000 0000 0000 0b00 0000  esec............
-000024c0: 0600 0000 4300 0000 737c 0000 0074 006a  ....C...s|...t.j
-000024d0: 017c 027c 037c 0464 018d 037d 057c 057c  .|.|.|.d...}.|.|
-000024e0: 0183 017d 067c 006a 0272 3874 0364 0264  ...}.|.j.r8t.d.d
-000024f0: 0384 007c 066a 0444 0083 0164 0464 0569  ...|.j.D...d.d.i
-00002500: 018e 0101 0067 007d 0778 3a7c 066a 0444  .....g.}.x:|.j.D
-00002510: 005d 307d 0878 2a7c 086a 0544 005d 207d  .]0}.x*|.j.D.] }
-00002520: 097c 096a 067c 096a 077c 096a 0864 069c  .|.j.|.j.|.j.d..
-00002530: 037d 0a7c 076a 097c 0a83 0101 0071 5057  .}.|.j.|.....qPW
-00002540: 0071 4457 007c 0753 0029 074e 2903 723a  .qDW.|.S.).N).r:
-00002550: 0000 0072 3f00 0000 7240 0000 0063 0100  ...r?...r@...c..
-00002560: 0000 0000 0000 0300 0000 0700 0000 5300  ..............S.
-00002570: 0000 732c 0000 0067 007c 005d 247d 017c  ..s,...g.|.]$}.|
-00002580: 016a 0044 005d 187d 0264 007c 026a 019b  .j.D.].}.d.|.j..
-00002590: 0064 017c 026a 029b 009d 0491 0371 0e71  .d.|.j.......q.q
-000025a0: 0453 0029 027a 0774 6f6b 656e 3a20 7a06  .S.).z.token: z.
-000025b0: 096e 6572 3a20 2903 724c 0000 0072 1f00  .ner: ).rL...r..
-000025c0: 0000 720f 0000 0029 0372 4600 0000 7261  ..r....).rF...ra
-000025d0: 0000 0072 1d00 0000 7217 0000 0072 1700  ...r....r....r..
-000025e0: 0000 7218 0000 0072 4700 0000 0301 0000  ..r....rG.......
-000025f0: 7302 0000 0006 007a 2b53 7461 6e7a 6157  s......z+StanzaW
-00002600: 7261 7070 6572 2e6e 6572 5f74 6f6b 656e  rapper.ner_token
-00002610: 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973 7463  .<locals>.<listc
-00002620: 6f6d 703e 7248 0000 0072 2d00 0000 2903  omp>rH...r-...).
-00002630: 721d 0000 0072 0f00 0000 720e 0000 0029  r....r....r....)
-00002640: 0a72 1300 0000 7205 0000 0072 3d00 0000  .r....r....r=...
-00002650: 724b 0000 0072 4a00 0000 724c 0000 0072  rK...rJ...rL...r
-00002660: 1f00 0000 720f 0000 0072 0e00 0000 721e  ....r....r....r.
-00002670: 0000 0029 0b72 1600 0000 721f 0000 0072  ...).r....r....r
-00002680: 3a00 0000 723f 0000 0072 4000 0000 724d  :...r?...r@...rM
-00002690: 0000 0072 4e00 0000 7229 0000 0072 6100  ...rN...r)...ra.
-000026a0: 0000 721d 0000 0072 2a00 0000 7217 0000  ..r....r*...r...
-000026b0: 0072 1700 0000 7218 0000 0072 6c00 0000  .r....r....rl...
-000026c0: ff00 0000 7318 0000 0000 0110 0108 0106  ....s...........
-000026d0: 011a 0104 010c 010c 0204 0104 010a 0212  ................
-000026e0: 017a 1753 7461 6e7a 6157 7261 7070 6572  .z.StanzaWrapper
-000026f0: 2e6e 6572 5f74 6f6b 656e fa12 746f 6b65  .ner_token..toke
-00002700: 6e69 7a65 2c73 656e 7469 6d65 6e74 6305  nize,sentimentc.
-00002710: 0000 0000 0000 0005 0000 0006 0000 0043  ...............C
-00002720: 0000 0073 1200 0000 7c00 6a00 7c01 7c02  ...s....|.j.|.|.
-00002730: 7c03 7c04 6401 8d04 5300 2902 4e29 0372  |.|.d...S.).N).r
-00002740: 3a00 0000 723f 0000 0072 4000 0000 2901  :...r?...r@...).
-00002750: da09 7365 6e74 696d 656e 7429 0572 1600  ..sentiment).r..
-00002760: 0000 721f 0000 0072 3a00 0000 723f 0000  ..r....r:...r?..
-00002770: 0072 4000 0000 7217 0000 0072 1700 0000  .r@...r....r....
-00002780: 7218 0000 00da 1173 656e 7469 6d65 6e74  r......sentiment
-00002790: 5f63 6869 6e65 7365 0f01 0000 7302 0000  _chinese....s...
-000027a0: 0000 017a 1f53 7461 6e7a 6157 7261 7070  ...z.StanzaWrapp
-000027b0: 6572 2e73 656e 7469 6d65 6e74 5f63 6869  er.sentiment_chi
-000027c0: 6e65 7365 6305 0000 0000 0000 000b 0000  nesec...........
-000027d0: 0005 0000 0043 0000 0073 5000 0000 7400  .....C...sP...t.
-000027e0: 6a01 7c02 7c03 7c04 6401 8d03 7d05 7c05  j.|.|.|.d...}.|.
-000027f0: 7c01 8301 7d06 6700 7d07 782e 7402 7c06  |...}.g.}.x.t.|.
-00002800: 6a03 8301 4400 5d20 5c02 7d08 7d09 7c09  j...D.] \.}.}.|.
-00002810: 6a04 7c09 6a05 6402 9c02 7d0a 7c07 6a06  j.|.j.d...}.|.j.
-00002820: 7c0a 8301 0100 7128 5700 7c07 5300 2903  |.....q(W.|.S.).
-00002830: 4e29 0372 3a00 0000 723f 0000 0072 4000  N).r:...r?...r@.
-00002840: 0000 2902 721c 0000 0072 6f00 0000 2907  ..).r....ro...).
-00002850: 7213 0000 0072 0500 0000 7249 0000 0072  r....r....rI...r
-00002860: 4a00 0000 721f 0000 0072 6f00 0000 721e  J...r....ro...r.
-00002870: 0000 0029 0b72 1600 0000 721f 0000 0072  ...).r....r....r
-00002880: 3a00 0000 723f 0000 0072 4000 0000 724d  :...r?...r@...rM
-00002890: 0000 0072 4e00 0000 7229 0000 0072 5000  ...rN...r)...rP.
-000028a0: 0000 721c 0000 0072 2a00 0000 7217 0000  ..r....r*...r...
-000028b0: 0072 1700 0000 7218 0000 0072 6f00 0000  .r....r....ro...
-000028c0: 1201 0000 7310 0000 0000 0110 0108 0104  ....s...........
-000028d0: 0114 0304 010a 020e 017a 1753 7461 6e7a  .........z.Stanz
-000028e0: 6157 7261 7070 6572 2e73 656e 7469 6d65  aWrapper.sentime
-000028f0: 6e74 da0c 6d75 6c74 696c 696e 6775 616c  nt..multilingual
-00002900: 6305 0000 0000 0000 000a 0000 0006 0000  c...............
-00002910: 0043 0000 0073 8200 0000 7400 6a01 6401  .C...s....t.j.d.
-00002920: 6402 8d01 0100 7402 7c02 6403 7c03 7c04  d.....t.|.d.|.|.
-00002930: 6404 8d04 7d05 7c01 7d06 6405 6406 8400  d...}.|.}.d.d...
-00002940: 7c06 4400 8301 7d06 7c05 7c06 8301 0100  |.D...}.|.|.....
-00002950: 7c00 6a03 7254 7404 6407 6a05 6408 6409  |.j.rTt.d.j.d.d.
-00002960: 8400 7c06 4400 8301 8301 8301 0100 6700  ..|.D.........g.
-00002970: 7d07 7824 7c06 4400 5d1c 7d08 7c08 6a06  }.x$|.D.].}.|.j.
-00002980: 7c08 6a07 640a 9c02 7d09 7c07 6a08 7c09  |.j.d...}.|.j.|.
-00002990: 8301 0100 715e 5700 7c07 5300 290b 4e72  ....q^W.|.S.).Nr
-000029a0: 7100 0000 2901 723a 0000 005a 066c 616e  q...).r:...Z.lan
-000029b0: 6769 6429 0472 3a00 0000 723f 0000 00da  gid).r:...r?....
-000029c0: 116c 616e 6769 645f 636c 6561 6e5f 7465  .langid_clean_te
-000029d0: 7874 7240 0000 0063 0100 0000 0000 0000  xtr@...c........
-000029e0: 0200 0000 0600 0000 5300 0000 7318 0000  ........S...s...
-000029f0: 0067 007c 005d 107d 0174 0067 007c 0164  .g.|.].}.t.g.|.d
-00002a00: 008d 0291 0271 0453 0029 0129 0172 1f00  .....q.S.).).r..
-00002a10: 0000 2901 7204 0000 0029 0272 4600 0000  ..).r....).rF...
-00002a20: 721f 0000 0072 1700 0000 7217 0000 0072  r....r....r....r
-00002a30: 1800 0000 7247 0000 0023 0100 0073 0200  ....rG...#...s..
-00002a40: 0000 0600 7a26 5374 616e 7a61 5772 6170  ....z&StanzaWrap
-00002a50: 7065 722e 6c61 6e67 2e3c 6c6f 6361 6c73  per.lang.<locals
-00002a60: 3e2e 3c6c 6973 7463 6f6d 703e 722d 0000  >.<listcomp>r-..
-00002a70: 0063 0100 0000 0000 0000 0200 0000 0400  .c..............
-00002a80: 0000 7300 0000 7320 0000 007c 005d 187d  ..s...s ...|.].}
-00002a90: 017c 016a 009b 0064 007c 016a 019b 009d  .|.j...d.|.j....
-00002aa0: 0356 0001 0071 0264 0153 0029 02fa 0109  .V...q.d.S.)....
-00002ab0: 4e29 0272 1f00 0000 723a 0000 0029 0272  N).r....r:...).r
-00002ac0: 4600 0000 724e 0000 0072 1700 0000 7217  F...rN...r....r.
-00002ad0: 0000 0072 1800 0000 fa09 3c67 656e 6578  ...r......<genex
-00002ae0: 7072 3e26 0100 0073 0200 0000 0400 7a25  pr>&...s......z%
-00002af0: 5374 616e 7a61 5772 6170 7065 722e 6c61  StanzaWrapper.la
-00002b00: 6e67 2e3c 6c6f 6361 6c73 3e2e 3c67 656e  ng.<locals>.<gen
-00002b10: 6578 7072 3e29 0272 1f00 0000 723a 0000  expr>).r....r:..
-00002b20: 0029 0972 1300 0000 723b 0000 0072 0500  .).r....r;...r..
-00002b30: 0000 723d 0000 0072 4b00 0000 7256 0000  ..r=...rK...rV..
-00002b40: 0072 1f00 0000 723a 0000 0072 1e00 0000  .r....r:...r....
-00002b50: 290a 7216 0000 00da 096c 6973 745f 7465  ).r......list_te
-00002b60: 7874 723a 0000 0072 7200 0000 7240 0000  xtr:...rr...r@..
-00002b70: 0072 4d00 0000 da04 646f 6373 7229 0000  .rM.....docsr)..
-00002b80: 0072 4e00 0000 722a 0000 0072 1700 0000  .rN...r*...r....
-00002b90: 7217 0000 0072 1800 0000 723a 0000 001f  r....r....r:....
-00002ba0: 0100 0073 1a00 0000 0001 0c01 1001 0401  ...s............
-00002bb0: 0e01 0801 0601 1801 0401 0a02 0401 0a02  ................
-00002bc0: 0e01 7a12 5374 616e 7a61 5772 6170 7065  ..z.StanzaWrappe
-00002bd0: 722e 6c61 6e67 4e72 0b00 0000 6304 0000  r.langNr....c...
-00002be0: 0000 0000 000a 0000 0005 0000 0043 0000  .............C..
-00002bf0: 0073 bc00 0000 7c03 6401 6b03 7228 781e  .s....|.d.k.r(x.
-00002c00: 7c03 6a00 6402 8301 4400 5d10 7d04 7401  |.j.d...D.].}.t.
-00002c10: 6a02 7c04 6403 8d01 0100 7114 5700 7403  j.|.d.....q.W.t.
-00002c20: 8300 7d05 7c01 7d06 7c05 7c06 8301 7d06  ..}.|.}.|.|...}.
-00002c30: 6700 7d07 7878 7c06 4400 5d70 7d08 7c00  g.}.xx|.D.]p}.|.
-00002c40: 6a04 728a 7405 6404 8301 0100 7405 6405  j.r.t.d.....t.d.
-00002c50: 7c08 6a06 9b00 9d02 8301 0100 7405 6406  |.j.........t.d.
-00002c60: 7c08 6a07 9b00 9d02 8301 0100 7405 7c08  |.j.........t.|.
-00002c70: 6a08 6407 1900 6a09 8300 9b00 8301 0100  j.d...j.........
-00002c80: 7c08 6a06 7c08 6a07 7c08 6408 9c03 7d09  |.j.|.j.|.d...}.
-00002c90: 7c02 6400 6b03 72aa 7c02 7c09 8301 0100  |.d.k.r.|.|.....
-00002ca0: 7c07 6a0a 7c09 8301 0100 7144 5700 7c07  |.j.|.....qDW.|.
-00002cb0: 5300 2909 4e72 0b00 0000 fa01 2c29 0172  S.).Nr......,).r
-00002cc0: 3a00 0000 7a03 2d2d 2d7a 0674 6578 743a  :...z.---z.text:
-00002cd0: 207a 066c 616e 673a 2072 0100 0000 2903   z.lang: r....).
-00002ce0: 721f 0000 0072 3a00 0000 724e 0000 0029  r....r:...rN...)
-00002cf0: 0b72 3200 0000 7213 0000 0072 3b00 0000  .r2...r....r;...
-00002d00: 7206 0000 0072 3d00 0000 724b 0000 0072  r....r=...rK...r
-00002d10: 1f00 0000 723a 0000 0072 4a00 0000 5a13  ....r:...rJ...Z.
-00002d20: 6465 7065 6e64 656e 6369 6573 5f73 7472  dependencies_str
-00002d30: 696e 6772 1e00 0000 290a 7216 0000 0072  ingr....).r....r
-00002d40: 7500 0000 5a0c 6675 6e63 5f70 726f 6365  u...Z.func_proce
-00002d50: 7373 5a0d 646f 776e 6c6f 6164 5f6c 616e  ssZ.download_lan
-00002d60: 67da 016c 724d 0000 0072 7600 0000 7229  g..lrM...rv...r)
-00002d70: 0000 0072 4e00 0000 722a 0000 0072 1700  ...rN...r*...r..
-00002d80: 0000 7217 0000 0072 1800 0000 da0a 6c61  ..r....r......la
-00002d90: 6e67 5f6d 756c 7469 3001 0000 7328 0000  ng_multi0...s(..
-00002da0: 0000 0108 0110 0110 0106 0104 0108 0104  ................
-00002db0: 010a 0106 0108 0110 0110 0114 0204 0104  ................
-00002dc0: 0108 0208 0108 010e 017a 1853 7461 6e7a  .........z.Stanz
-00002dd0: 6157 7261 7070 6572 2e6c 616e 675f 6d75  aWrapper.lang_mu
-00002de0: 6c74 6963 0200 0000 0000 0000 0a00 0000  ltic............
-00002df0: 0700 0000 4300 0000 7356 0100 007c 0164  ....C...sV...|.d
-00002e00: 006b 0273 1474 007c 0183 0164 016b 0272  .k.s.t.|...d.k.r
-00002e10: 2074 0164 0283 0101 0064 0053 0090 0178   t.d.....d.S...x
-00002e20: 2e74 027c 0183 0144 0090 015d 205c 027d  .t.|...D...] \.}
-00002e30: 027d 0374 017c 0283 0101 0074 037c 0383  .}.t.|.....t.|..
-00002e40: 0174 046b 0272 ae74 057c 0164 0119 006a  .t.k.r.t.|.d...j
-00002e50: 0683 0083 017d 0474 0164 0364 046a 077c  .....}.t.d.d.j.|
-00002e60: 0483 0117 0083 0101 0067 007d 0578 227c  .........g.}.x"|
-00002e70: 036a 0683 0044 005d 167d 067c 056a 0874  .j...D.].}.|.j.t
-00002e80: 097c 037c 0619 0083 0183 0101 0071 7a57  .|.|.........qzW
-00002e90: 0064 046a 077c 0583 017d 0774 0164 037c  .d.j.|...}.t.d.|
-00002ea0: 079b 009d 0283 0101 0071 2c74 037c 0383  .........q,t.|..
-00002eb0: 0174 056b 0272 2c74 057c 0364 0119 006a  .t.k.r,t.|.d...j
-00002ec0: 0683 0083 017d 0474 0164 0364 046a 077c  .....}.t.d.d.j.|
-00002ed0: 0483 0117 0083 0101 0078 7074 027c 0383  .........xpt.|..
-00002ee0: 0144 005d 645c 027d 087d 0974 037c 0983  .D.]d\.}.}.t.|..
-00002ef0: 0174 046b 0290 0172 4067 007d 0578 247c  .t.k...r@g.}.x$|
-00002f00: 096a 0683 0044 005d 187d 067c 056a 0874  .j...D.].}.|.j.t
-00002f10: 097c 097c 0619 0083 0183 0101 0090 0171  .|.|...........q
-00002f20: 0a57 0064 046a 077c 0583 017d 0774 0164  .W.d.j.|...}.t.d
-00002f30: 037c 079b 009d 0283 0101 0071 e674 0164  .|.........q.t.d
-00002f40: 037c 0983 0201 0071 e657 0071 2c57 0064  .|.....q.W.q,W.d
-00002f50: 0053 0029 054e 7201 0000 007a 0a4e 6f20  .S.).Nr....z.No 
-00002f60: 5265 7375 6c74 217a 0209 0972 7300 0000  Result!z...rs...
-00002f70: 290a da03 6c65 6e72 4b00 0000 7249 0000  )...lenrK...rI..
-00002f80: 0072 6900 0000 da04 6469 6374 da04 6c69  .ri.....dict..li
-00002f90: 7374 da04 6b65 7973 7256 0000 0072 1e00  st..keysrV...r..
-00002fa0: 0000 da03 7374 7229 0a72 1600 0000 da06  ....str).r......
-00002fb0: 7265 7375 6c74 5a03 6964 78da 0469 7465  resultZ.idx..ite
-00002fc0: 6d5a 0666 6965 6c64 735a 066c 6973 745f  mZ.fieldsZ.list_
-00002fd0: 76da 016b 7234 0000 005a 0469 6478 315a  v..kr4...Z.idx1Z
-00002fe0: 026c 6972 1700 0000 7217 0000 0072 1800  .lir....r....r..
-00002ff0: 0000 da0c 7072 696e 745f 7265 7375 6c74  ....print_result
-00003000: 4801 0000 7330 0000 0000 0114 0108 0104  H...s0..........
-00003010: 0116 0108 010c 0110 0112 0104 010e 0116  ................
-00003020: 010a 0110 010c 0110 0112 0112 020e 0104  ................
-00003030: 010e 0118 020a 0110 027a 1a53 7461 6e7a  .........z.Stanz
-00003040: 6157 7261 7070 6572 2e70 7269 6e74 5f72  aWrapper.print_r
-00003050: 6573 756c 7429 0346 4646 2903 7208 0000  esult).FFF).r...
-00003060: 0072 3e00 0000 4629 0272 4100 0000 4629  .r>...F).rA...F)
-00003070: 0572 0800 0000 720d 0000 0046 4646 2905  .r....r....FFF).
-00003080: 7208 0000 0072 0d00 0000 4646 4629 0572  r....r....FFF).r
-00003090: 0800 0000 720d 0000 0046 4646 2901 4629  ....r....FFF).F)
-000030a0: 0372 0800 0000 7254 0000 0046 2904 7241  .r....rT...F).rA
-000030b0: 0000 0072 5900 0000 4646 2904 7208 0000  ...rY...FF).r...
-000030c0: 0072 5c00 0000 4646 2903 7241 0000 0072  .r\...FF).rA...r
-000030d0: 5900 0000 4629 0372 0800 0000 7264 0000  Y...F).r....rd..
-000030e0: 0046 2904 7208 0000 0072 6800 0000 4646  .F).r....rh...FF
-000030f0: 2904 7241 0000 0072 6800 0000 4646 2903  ).rA...rh...FF).
-00003100: 7241 0000 0072 6800 0000 4629 0372 0800  rA...rh...F).r..
-00003110: 0000 7268 0000 0046 2903 7241 0000 0072  ..rh...F).rA...r
-00003120: 6e00 0000 4629 0372 0800 0000 726e 0000  n...F).r....rn..
-00003130: 0046 2903 7271 0000 0046 4629 024e 720b  .F).rq...FF).Nr.
-00003140: 0000 0029 1972 3600 0000 7237 0000 0072  ...).r6...r7...r
-00003150: 3800 0000 7219 0000 0072 3b00 0000 723c  8...r....r;...r<
-00003160: 0000 0072 4200 0000 720d 0000 0072 5100  ...rB...r....rQ.
-00003170: 0000 7252 0000 0072 5300 0000 7258 0000  ..rR...rS...rX..
-00003180: 0072 5b00 0000 725a 0000 0072 6300 0000  .r[...rZ...rc...
-00003190: 7262 0000 0072 0f00 0000 726b 0000 0072  rb...r....rk...r
-000031a0: 6d00 0000 726c 0000 0072 7000 0000 726f  m...rl...rp...ro
-000031b0: 0000 0072 3a00 0000 7279 0000 0072 8200  ...r:...ry...r..
-000031c0: 0000 7217 0000 0072 1700 0000 7217 0000  ..r....r....r...
-000031d0: 0072 1800 0000 7239 0000 0058 0000 0073  .r....r9...X...s
-000031e0: 2c00 0000 0801 0a07 0a03 0a03 0803 0a13  ,...............
-000031f0: 0a0b 0a12 0a13 0a12 0a03 0a13 0a03 0a14  ................
-00003200: 0a0e 0a03 0a03 0a10 0a03 0a0d 0a11 0a18  ................
-00003210: 7239 0000 0029 0d72 1300 0000 5a0d 7374  r9...).r....Z.st
-00003220: 616e 7a61 2e73 6572 7665 7272 0200 0000  anza.serverr....
-00003230: 7203 0000 005a 1873 7461 6e7a 612e 6d6f  r....Z.stanza.mo
-00003240: 6465 6c73 2e63 6f6d 6d6f 6e2e 646f 6372  dels.common.docr
-00003250: 0400 0000 5a14 7374 616e 7a61 2e70 6970  ....Z.stanza.pip
-00003260: 656c 696e 652e 636f 7265 7205 0000 005a  eline.corer....Z
-00003270: 1c73 7461 6e7a 612e 7069 7065 6c69 6e65  .stanza.pipeline
-00003280: 2e6d 756c 7469 6c69 6e67 7561 6c72 0600  .multilingualr..
-00003290: 0000 722f 0000 0072 0700 0000 7239 0000  ..r/...r....r9..
-000032a0: 0072 1700 0000 7217 0000 0072 1700 0000  .r....r....r....
-000032b0: 7218 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
-000032c0: 0000 0073 0e00 0000 0801 1001 0c01 0c01  ...s............
-000032d0: 0c01 0801 0e51                           .....Q
+000019d0: 745f 6578 7061 6e64 2e3c 6c6f 6361 6c73  t_expand.<locals
+000019e0: 3e2e 3c6c 6973 7463 6f6d 703e 6301 0000  >.<listcomp>c...
+000019f0: 0000 0000 0002 0000 0003 0000 0053 0000  .............S..
+00001a00: 0073 1200 0000 6700 7c00 5d0a 7d01 7c01  .s....g.|.].}.|.
+00001a10: 6a00 9102 7104 5300 7217 0000 0029 0172  j...q.S.r....).r
+00001a20: 1f00 0000 2902 7249 0000 0072 5900 0000  ....).rI...rY...
+00001a30: 7217 0000 0072 1700 0000 7218 0000 0072  r....r....r....r
+00001a40: 4a00 0000 bf00 0000 7302 0000 0006 0029  J.......s......)
+00001a50: 0272 1d00 0000 721f 0000 0029 0b72 1300  .r....r....).r..
+00001a60: 0000 7205 0000 0072 3e00 0000 724d 0000  ..r....r>...rM..
+00001a70: 0072 4f00 0000 723d 0000 0072 4e00 0000  .rO...r=...rN...
+00001a80: 721f 0000 00da 046a 6f69 6eda 0577 6f72  r......join..wor
+00001a90: 6473 721e 0000 0029 0c72 1600 0000 721f  dsr....).r....r.
+00001aa0: 0000 0072 3a00 0000 7240 0000 0072 4100  ...r:...r@...rA.
+00001ab0: 0000 7251 0000 0072 5200 0000 7229 0000  ..rQ...rR...r)..
+00001ac0: 0072 1c00 0000 7220 0000 0072 1d00 0000  .r....r ...r....
+00001ad0: 722a 0000 0072 1700 0000 7217 0000 0072  r*...r....r....r
+00001ae0: 1800 0000 da0a 6d77 745f 6578 7061 6e64  ......mwt_expand
+00001af0: b300 0000 731a 0000 0000 0214 0108 0104  ....s...........
+00001b00: 010c 0104 010c 0106 0128 0204 011a 020e  .........(......
+00001b10: 010e 017a 1853 7461 6e7a 6157 7261 7070  ...z.StanzaWrapp
+00001b20: 6572 2e6d 7774 5f65 7870 616e 64fa 1b74  er.mwt_expand..t
+00001b30: 6f6b 656e 697a 652c 6c65 6d6d 612c 706f  okenize,lemma,po
+00001b40: 732c 6465 7070 6172 7365 6306 0000 0000  s,depparsec.....
+00001b50: 0000 0006 0000 0007 0000 0043 0000 0073  ...........C...s
+00001b60: 1400 0000 7c00 6a00 7c01 7c02 7c03 7c04  ....|.j.|.|.|.|.
+00001b70: 7c05 6401 8d05 5300 2902 4e29 0272 4100  |.d...S.).N).rA.
+00001b80: 0000 7247 0000 0029 01da 0374 6167 2906  ..rG...)...tag).
+00001b90: 7216 0000 0072 1f00 0000 723a 0000 0072  r....r....r:...r
+00001ba0: 4000 0000 7241 0000 0072 4700 0000 7217  @...rA...rG...r.
+00001bb0: 0000 0072 1700 0000 7218 0000 00da 0b74  ...r....r......t
+00001bc0: 6167 5f63 6869 6e65 7365 c500 0000 7302  ag_chinese....s.
+00001bd0: 0000 0000 017a 1953 7461 6e7a 6157 7261  .....z.StanzaWra
+00001be0: 7070 6572 2e74 6167 5f63 6869 6e65 7365  pper.tag_chinese
+00001bf0: fa10 746f 6b65 6e69 7a65 2c6d 7774 2c70  ..tokenize,mwt,p
+00001c00: 6f73 6306 0000 0000 0000 000c 0000 0007  osc.............
+00001c10: 0000 0043 0000 0073 9000 0000 7400 6a01  ...C...s....t.j.
+00001c20: 7c02 7c03 7c04 7c05 7c00 6a02 6401 8d05  |.|.|.|.|.j.d...
+00001c30: 7d06 7c06 7c01 8301 7d07 7c00 6a03 723e  }.|.|...}.|.j.r>
+00001c40: 7404 6402 6403 8400 7c07 6a05 4400 8301  t.d.d...|.j.D...
+00001c50: 6404 6405 6901 8e01 0100 6700 7d08 7848  d.d.i.....g.}.xH
+00001c60: 7c07 6a05 4400 5d3e 7d09 7838 7c09 6a06  |.j.D.]>}.x8|.j.
+00001c70: 4400 5d2e 7d0a 7c0a 6a07 7c0a 6a08 7c0a  D.].}.|.j.|.j.|.
+00001c80: 6a09 7c0a 6a0a 7272 7c0a 6a0a 6e02 6406  j.|.j.rr|.j.n.d.
+00001c90: 6407 9c04 7d0b 7c08 6a0b 7c0b 8301 0100  d...}.|.j.|.....
+00001ca0: 7156 5700 714a 5700 7c08 5300 2908 4e29  qVW.qJW.|.S.).N)
+00001cb0: 0572 3a00 0000 7240 0000 0072 4100 0000  .r:...r@...rA...
+00001cc0: 7247 0000 0072 3e00 0000 6301 0000 0000  rG...r>...c.....
+00001cd0: 0000 0003 0000 000b 0000 0053 0000 0073  ...........S...s
+00001ce0: 4600 0000 6700 7c00 5d3e 7d01 7c01 6a00  F...g.|.]>}.|.j.
+00001cf0: 4400 5d32 7d02 6400 7c02 6a01 9b00 6401  D.]2}.d.|.j...d.
+00001d00: 7c02 6a02 9b00 6402 7c02 6a03 9b00 6403  |.j...d.|.j...d.
+00001d10: 7c02 6a04 7238 7c02 6a04 6e02 6404 9b00  |.j.r8|.j.n.d...
+00001d20: 9d08 9103 710e 7104 5300 2905 7a06 776f  ....q.q.S.).z.wo
+00001d30: 7264 3a20 7a07 0975 706f 733a 207a 0709  rd: z..upos: z..
+00001d40: 7870 6f73 3a20 7a08 0966 6561 7473 3a20  xpos: z..feats: 
+00001d50: da01 5f29 0572 5b00 0000 721f 0000 00da  .._).r[...r.....
+00001d60: 0475 706f 73da 0478 706f 73da 0566 6561  .upos..xpos..fea
+00001d70: 7473 2903 7249 0000 00da 0473 656e 7472  ts).rI.....sentr
+00001d80: 5900 0000 7217 0000 0072 1700 0000 7218  Y...r....r....r.
+00001d90: 0000 0072 4a00 0000 cd00 0000 7302 0000  ...rJ.......s...
+00001da0: 0006 017a 2553 7461 6e7a 6157 7261 7070  ...z%StanzaWrapp
+00001db0: 6572 2e74 6167 2e3c 6c6f 6361 6c73 3e2e  er.tag.<locals>.
+00001dc0: 3c6c 6973 7463 6f6d 703e 724b 0000 0072  <listcomp>rK...r
+00001dd0: 2d00 0000 7261 0000 0029 0472 5900 0000  -...ra...).rY...
+00001de0: 7262 0000 0072 6300 0000 7264 0000 0029  rb...rc...rd...)
+00001df0: 0c72 1300 0000 7205 0000 0072 3e00 0000  .r....r....r>...
+00001e00: 723d 0000 0072 4e00 0000 724d 0000 0072  r=...rN...rM...r
+00001e10: 5b00 0000 721f 0000 0072 6200 0000 7263  [...r....rb...rc
+00001e20: 0000 0072 6400 0000 721e 0000 0029 0c72  ...rd...r....).r
+00001e30: 1600 0000 721f 0000 0072 3a00 0000 7240  ....r....r:...r@
+00001e40: 0000 0072 4100 0000 7247 0000 0072 5100  ...rA...rG...rQ.
+00001e50: 0000 7252 0000 0072 2900 0000 7265 0000  ..rR...r)...re..
+00001e60: 0072 5900 0000 722a 0000 0072 1700 0000  .rY...r*...r....
+00001e70: 7217 0000 0072 1800 0000 725e 0000 00c8  r....r....r^....
+00001e80: 0000 0073 1e00 0000 0001 1601 0801 0601  ...s............
+00001e90: 0201 0601 1201 0401 0c01 0c02 0401 0401  ................
+00001ea0: 0401 1402 1201 7a11 5374 616e 7a61 5772  ......z.StanzaWr
+00001eb0: 6170 7065 722e 7461 6763 0500 0000 0000  apper.tagc......
+00001ec0: 0000 0500 0000 0600 0000 4300 0000 7312  ..........C...s.
+00001ed0: 0000 007c 006a 007c 017c 027c 037c 0464  ...|.j.|.|.|.|.d
+00001ee0: 018d 0453 0029 024e 2901 7241 0000 0029  ...S.).N).rA...)
+00001ef0: 01da 1070 6172 7365 5f64 6570 656e 6465  ...parse_depende
+00001f00: 6e63 7929 0572 1600 0000 721f 0000 0072  ncy).r....r....r
+00001f10: 3a00 0000 7240 0000 0072 4100 0000 7217  :...r@...rA...r.
+00001f20: 0000 0072 1700 0000 7218 0000 00da 1870  ...r....r......p
+00001f30: 6172 7365 5f64 6570 656e 6465 6e63 795f  arse_dependency_
+00001f40: 6368 696e 6573 65db 0000 0073 0200 0000  chinese....s....
+00001f50: 0001 7a26 5374 616e 7a61 5772 6170 7065  ..z&StanzaWrappe
+00001f60: 722e 7061 7273 655f 6465 7065 6e64 656e  r.parse_dependen
+00001f70: 6379 5f63 6869 6e65 7365 fa1f 746f 6b65  cy_chinese..toke
+00001f80: 6e69 7a65 2c6d 7774 2c70 6f73 2c6c 656d  nize,mwt,pos,lem
+00001f90: 6d61 2c64 6570 7061 7273 6563 0500 0000  ma,depparsec....
+00001fa0: 0000 0000 0b00 0000 0800 0000 4300 0000  ............C...
+00001fb0: 73aa 0000 0074 006a 017c 027c 037c 047c  s....t.j.|.|.|.|
+00001fc0: 006a 0264 018d 047d 057c 057c 0183 017d  .j.d...}.|.|...}
+00001fd0: 067c 006a 0372 3c74 0464 0264 0384 007c  .|.j.r<t.d.d...|
+00001fe0: 066a 0544 0083 0164 0464 0569 018e 0101  .j.D...d.d.i....
+00001ff0: 0067 007d 0778 647c 066a 0544 005d 5a7d  .g.}.xd|.j.D.]Z}
+00002000: 0878 547c 086a 0644 005d 4a7d 0974 077c  .xT|.j.D.]J}.t.|
+00002010: 096a 0883 017c 096a 0974 077c 096a 0a83  .j...|.j.t.|.j..
+00002020: 017c 096a 0a64 066b 0472 887c 086a 067c  .|.j.d.k.r.|.j.|
+00002030: 096a 0a64 0718 0019 006a 096e 0264 087c  .j.d.....j.n.d.|
+00002040: 096a 0b64 099c 057d 0a7c 076a 0c7c 0a83  .j.d...}.|.j.|..
+00002050: 0101 0071 5457 0071 4857 007c 0753 0029  ...qTW.qHW.|.S.)
+00002060: 0a4e 2904 723a 0000 0072 4000 0000 7241  .N).r:...r@...rA
+00002070: 0000 0072 3e00 0000 6301 0000 0000 0000  ...r>...c.......
+00002080: 0003 0000 000d 0000 0053 0000 0073 5e00  .........S...s^.
+00002090: 0000 6700 7c00 5d56 7d01 7c01 6a00 4400  ..g.|.]V}.|.j.D.
+000020a0: 5d4a 7d02 6400 7c02 6a01 9b00 6401 7c02  ]J}.d.|.j...d.|.
+000020b0: 6a02 9b00 6402 7c02 6a03 9b00 6403 7c02  j...d.|.j...d.|.
+000020c0: 6a03 6404 6b04 7248 7c01 6a00 7c02 6a03  j.d.k.rH|.j.|.j.
+000020d0: 6405 1800 1900 6a02 6e02 6406 9b00 6407  d.....j.n.d...d.
+000020e0: 7c02 6a04 9b00 9d0a 9103 710e 7104 5300  |.j.......q.q.S.
+000020f0: 2908 7a04 6964 3a20 7a07 0977 6f72 643a  ).z.id: z..word:
+00002100: 207a 0a09 6865 6164 2069 643a 207a 0709   z..head id: z..
+00002110: 6865 6164 3a20 7201 0000 0072 2300 0000  head: r....r#...
+00002120: da04 726f 6f74 7a09 0964 6570 7265 6c3a  ..rootz..deprel:
+00002130: 2029 0572 5b00 0000 7248 0000 0072 1f00   ).r[...rH...r..
+00002140: 0000 da04 6865 6164 da06 6465 7072 656c  ....head..deprel
+00002150: 2903 7249 0000 0072 6500 0000 7259 0000  ).rI...re...rY..
+00002160: 0072 1700 0000 7217 0000 0072 1800 0000  .r....r....r....
+00002170: 724a 0000 00e3 0000 0073 0200 0000 0601  rJ.......s......
+00002180: 7a32 5374 616e 7a61 5772 6170 7065 722e  z2StanzaWrapper.
+00002190: 7061 7273 655f 6465 7065 6e64 656e 6379  parse_dependency
+000021a0: 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973 7463  .<locals>.<listc
+000021b0: 6f6d 703e 724b 0000 0072 2d00 0000 7201  omp>rK...r-...r.
+000021c0: 0000 0072 2300 0000 7269 0000 0029 0572  ...r#...ri...).r
+000021d0: 4800 0000 721f 0000 007a 0768 6561 6420  H...r....z.head 
+000021e0: 6964 726a 0000 0072 6b00 0000 290d 7213  idrj...rk...).r.
+000021f0: 0000 0072 0500 0000 723e 0000 0072 3d00  ...r....r>...r=.
+00002200: 0000 724e 0000 0072 4d00 0000 725b 0000  ..rN...rM...r[..
+00002210: 0072 5000 0000 7248 0000 0072 1f00 0000  .rP...rH...r....
+00002220: 726a 0000 0072 6b00 0000 721e 0000 0029  rj...rk...r....)
+00002230: 0b72 1600 0000 721f 0000 0072 3a00 0000  .r....r....r:...
+00002240: 7240 0000 0072 4100 0000 7251 0000 0072  r@...rA...rQ...r
+00002250: 5200 0000 7229 0000 0072 6500 0000 7259  R...r)...re...rY
+00002260: 0000 0072 2a00 0000 7217 0000 0072 1700  ...r*...r....r..
+00002270: 0000 7218 0000 0072 6600 0000 de00 0000  ..r....rf.......
+00002280: 7320 0000 0000 0114 0108 0106 0102 0106  s ..............
+00002290: 0112 0104 010c 010c 0208 0104 0108 011e  ................
+000022a0: 010a 0212 017a 1e53 7461 6e7a 6157 7261  .....z.StanzaWra
+000022b0: 7070 6572 2e70 6172 7365 5f64 6570 656e  pper.parse_depen
+000022c0: 6465 6e63 79fa 0c74 6f6b 656e 697a 652c  dency..tokenize,
+000022d0: 6e65 7263 0600 0000 0000 0000 0b00 0000  nerc............
+000022e0: 0700 0000 4300 0000 736e 0000 0074 006a  ....C...sn...t.j
+000022f0: 017c 027c 037c 047c 057c 006a 0264 018d  .|.|.|.|.|.j.d..
+00002300: 057d 067c 067c 0183 017d 077c 006a 0372  .}.|.|...}.|.j.r
+00002310: 3e74 0464 0264 0384 007c 076a 0544 0083  >t.d.d...|.j.D..
+00002320: 0164 0464 0569 018e 0101 0067 007d 0878  .d.d.i.....g.}.x
+00002330: 267c 076a 0544 005d 1c7d 097c 096a 067c  &|.j.D.].}.|.j.|
+00002340: 096a 0764 069c 027d 0a7c 086a 087c 0a83  .j.d...}.|.j.|..
+00002350: 0101 0071 4a57 007c 0853 0029 074e 2905  ...qJW.|.S.).N).
+00002360: 723a 0000 0072 4000 0000 7241 0000 0072  r:...r@...rA...r
+00002370: 4700 0000 723e 0000 0063 0100 0000 0000  G...r>...c......
+00002380: 0000 0200 0000 0600 0000 5300 0000 7320  ..........S...s 
+00002390: 0000 0067 007c 005d 187d 0164 007c 016a  ...g.|.].}.d.|.j
+000023a0: 009b 0064 017c 016a 019b 009d 0491 0271  ...d.|.j.......q
+000023b0: 0453 0029 027a 0865 6e74 6974 793a 207a  .S.).z.entity: z
+000023c0: 0709 7479 7065 3a20 2902 721f 0000 00da  ..type: ).r.....
+000023d0: 0474 7970 6529 0272 4900 0000 da03 656e  .type).rI.....en
+000023e0: 7472 1700 0000 7217 0000 0072 1800 0000  tr....r....r....
+000023f0: 724a 0000 00f6 0000 0073 0200 0000 0600  rJ.......s......
+00002400: 7a25 5374 616e 7a61 5772 6170 7065 722e  z%StanzaWrapper.
+00002410: 6e65 722e 3c6c 6f63 616c 733e 2e3c 6c69  ner.<locals>.<li
+00002420: 7374 636f 6d70 3e72 4b00 0000 722d 0000  stcomp>rK...r-..
+00002430: 0029 025a 0665 6e74 6974 7972 6d00 0000  .).Z.entityrm...
+00002440: 2909 7213 0000 0072 0500 0000 723e 0000  ).r....r....r>..
+00002450: 0072 3d00 0000 724e 0000 005a 0465 6e74  .r=...rN...Z.ent
+00002460: 7372 1f00 0000 726d 0000 0072 1e00 0000  sr....rm...r....
+00002470: 290b 7216 0000 0072 1f00 0000 723a 0000  ).r....r....r:..
+00002480: 0072 4000 0000 7241 0000 0072 4700 0000  .r@...rA...rG...
+00002490: 7251 0000 0072 5200 0000 7229 0000 0072  rQ...rR...r)...r
+000024a0: 6e00 0000 722a 0000 0072 1700 0000 7217  n...r*...r....r.
+000024b0: 0000 0072 1800 0000 720f 0000 00f2 0000  ...r....r.......
+000024c0: 0073 1400 0000 0001 1601 0801 0601 1a01  .s..............
+000024d0: 0401 0c02 0401 0a02 0e01 7a11 5374 616e  ..........z.Stan
+000024e0: 7a61 5772 6170 7065 722e 6e65 7263 0600  zaWrapper.nerc..
+000024f0: 0000 0000 0000 0600 0000 0700 0000 4300  ..............C.
+00002500: 0000 7314 0000 007c 006a 007c 017c 027c  ..s....|.j.|.|.|
+00002510: 037c 047c 0564 018d 0553 0029 024e 2902  .|.|.d...S.).N).
+00002520: 7241 0000 0072 4700 0000 2901 720f 0000  rA...rG...).r...
+00002530: 0029 0672 1600 0000 721f 0000 0072 3a00  .).r....r....r:.
+00002540: 0000 7240 0000 0072 4100 0000 7247 0000  ..r@...rA...rG..
+00002550: 0072 1700 0000 7217 0000 0072 1800 0000  .r....r....r....
+00002560: da0b 6e65 725f 6368 696e 6573 6500 0100  ..ner_chinese...
+00002570: 0073 0200 0000 0001 7a19 5374 616e 7a61  .s......z.Stanza
+00002580: 5772 6170 7065 722e 6e65 725f 6368 696e  Wrapper.ner_chin
+00002590: 6573 6563 0500 0000 0000 0000 0500 0000  esec............
+000025a0: 0600 0000 4300 0000 7312 0000 007c 006a  ....C...s....|.j
+000025b0: 007c 017c 027c 037c 0464 018d 0453 0029  .|.|.|.|.d...S.)
+000025c0: 024e 2901 7241 0000 0029 01da 096e 6572  .N).rA...)...ner
+000025d0: 5f74 6f6b 656e 2905 7216 0000 0072 1f00  _token).r....r..
+000025e0: 0000 723a 0000 0072 4000 0000 7241 0000  ..r:...r@...rA..
+000025f0: 0072 1700 0000 7217 0000 0072 1800 0000  .r....r....r....
+00002600: da11 6e65 725f 746f 6b65 6e5f 6368 696e  ..ner_token_chin
+00002610: 6573 6503 0100 0073 0200 0000 0001 7a1f  ese....s......z.
+00002620: 5374 616e 7a61 5772 6170 7065 722e 6e65  StanzaWrapper.ne
+00002630: 725f 746f 6b65 6e5f 6368 696e 6573 6563  r_token_chinesec
+00002640: 0500 0000 0000 0000 0b00 0000 0600 0000  ................
+00002650: 4300 0000 7380 0000 0074 006a 017c 027c  C...s....t.j.|.|
+00002660: 037c 047c 006a 0264 018d 047d 057c 057c  .|.|.j.d...}.|.|
+00002670: 0183 017d 067c 006a 0372 3c74 0464 0264  ...}.|.j.r<t.d.d
+00002680: 0384 007c 066a 0544 0083 0164 0464 0569  ...|.j.D...d.d.i
+00002690: 018e 0101 0067 007d 0778 3a7c 066a 0544  .....g.}.x:|.j.D
+000026a0: 005d 307d 0878 2a7c 086a 0644 005d 207d  .]0}.x*|.j.D.] }
+000026b0: 097c 096a 077c 096a 087c 096a 0964 069c  .|.j.|.j.|.j.d..
+000026c0: 037d 0a7c 076a 0a7c 0a83 0101 0071 5457  .}.|.j.|.....qTW
+000026d0: 0071 4857 007c 0753 0029 074e 2904 723a  .qHW.|.S.).N).r:
+000026e0: 0000 0072 4000 0000 7241 0000 0072 3e00  ...r@...rA...r>.
+000026f0: 0000 6301 0000 0000 0000 0003 0000 0007  ..c.............
+00002700: 0000 0053 0000 0073 2c00 0000 6700 7c00  ...S...s,...g.|.
+00002710: 5d24 7d01 7c01 6a00 4400 5d18 7d02 6400  ]$}.|.j.D.].}.d.
+00002720: 7c02 6a01 9b00 6401 7c02 6a02 9b00 9d04  |.j...d.|.j.....
+00002730: 9103 710e 7104 5300 2902 7a07 746f 6b65  ..q.q.S.).z.toke
+00002740: 6e3a 207a 0609 6e65 723a 2029 0372 4f00  n: z..ner: ).rO.
+00002750: 0000 721f 0000 0072 0f00 0000 2903 7249  ..r....r....).rI
+00002760: 0000 0072 6500 0000 721d 0000 0072 1700  ...re...r....r..
+00002770: 0000 7217 0000 0072 1800 0000 724a 0000  ..r....r....rJ..
+00002780: 000a 0100 0073 0200 0000 0600 7a2b 5374  .....s......z+St
+00002790: 616e 7a61 5772 6170 7065 722e 6e65 725f  anzaWrapper.ner_
+000027a0: 746f 6b65 6e2e 3c6c 6f63 616c 733e 2e3c  token.<locals>.<
+000027b0: 6c69 7374 636f 6d70 3e72 4b00 0000 722d  listcomp>rK...r-
+000027c0: 0000 0029 0372 1d00 0000 720f 0000 0072  ...).r....r....r
+000027d0: 0e00 0000 290b 7213 0000 0072 0500 0000  ....).r....r....
+000027e0: 723e 0000 0072 3d00 0000 724e 0000 0072  r>...r=...rN...r
+000027f0: 4d00 0000 724f 0000 0072 1f00 0000 720f  M...rO...r....r.
+00002800: 0000 0072 0e00 0000 721e 0000 0029 0b72  ...r....r....).r
+00002810: 1600 0000 721f 0000 0072 3a00 0000 7240  ....r....r:...r@
+00002820: 0000 0072 4100 0000 7251 0000 0072 5200  ...rA...rQ...rR.
+00002830: 0000 7229 0000 0072 6500 0000 721d 0000  ..r)...re...r...
+00002840: 0072 2a00 0000 7217 0000 0072 1700 0000  .r*...r....r....
+00002850: 7218 0000 0072 7000 0000 0601 0000 7318  r....rp.......s.
+00002860: 0000 0000 0114 0108 0106 011a 0104 010c  ................
+00002870: 010c 0204 0104 010a 0212 017a 1753 7461  ...........z.Sta
+00002880: 6e7a 6157 7261 7070 6572 2e6e 6572 5f74  nzaWrapper.ner_t
+00002890: 6f6b 656e fa12 746f 6b65 6e69 7a65 2c73  oken..tokenize,s
+000028a0: 656e 7469 6d65 6e74 6305 0000 0000 0000  entimentc.......
+000028b0: 0005 0000 0006 0000 0043 0000 0073 1200  .........C...s..
+000028c0: 0000 7c00 6a00 7c01 7c02 7c03 7c04 6401  ..|.j.|.|.|.|.d.
+000028d0: 8d04 5300 2902 4e29 0372 3a00 0000 7240  ..S.).N).r:...r@
+000028e0: 0000 0072 4100 0000 2901 da09 7365 6e74  ...rA...)...sent
+000028f0: 696d 656e 7429 0572 1600 0000 721f 0000  iment).r....r...
+00002900: 0072 3a00 0000 7240 0000 0072 4100 0000  .r:...r@...rA...
+00002910: 7217 0000 0072 1700 0000 7218 0000 00da  r....r....r.....
+00002920: 1173 656e 7469 6d65 6e74 5f63 6869 6e65  .sentiment_chine
+00002930: 7365 1601 0000 7302 0000 0000 017a 1f53  se....s......z.S
+00002940: 7461 6e7a 6157 7261 7070 6572 2e73 656e  tanzaWrapper.sen
+00002950: 7469 6d65 6e74 5f63 6869 6e65 7365 6305  timent_chinesec.
+00002960: 0000 0000 0000 000b 0000 0006 0000 0043  ...............C
+00002970: 0000 0073 5800 0000 7400 6a01 7c02 7c03  ...sX...t.j.|.|.
+00002980: 7c04 7c00 6a02 6401 8d04 7d05 7c05 7c01  |.|.j.d...}.|.|.
+00002990: 8301 7d06 6700 7d07 7832 7403 7c06 6a04  ..}.g.}.x2t.|.j.
+000029a0: 8301 4400 5d24 5c02 7d08 7d09 7c09 6a05  ..D.]$\.}.}.|.j.
+000029b0: 7406 7c09 6a07 8301 6402 9c02 7d0a 7c07  t.|.j...d...}.|.
+000029c0: 6a08 7c0a 8301 0100 712c 5700 7c07 5300  j.|.....q,W.|.S.
+000029d0: 2903 4e29 0472 3a00 0000 7240 0000 0072  ).N).r:...r@...r
+000029e0: 4100 0000 723e 0000 0029 0272 1c00 0000  A...r>...).r....
+000029f0: 7273 0000 0029 0972 1300 0000 7205 0000  rs...).r....r...
+00002a00: 0072 3e00 0000 724c 0000 0072 4d00 0000  .r>...rL...rM...
+00002a10: 721f 0000 0072 5000 0000 7273 0000 0072  r....rP...rs...r
+00002a20: 1e00 0000 290b 7216 0000 0072 1f00 0000  ....).r....r....
+00002a30: 723a 0000 0072 4000 0000 7241 0000 0072  r:...r@...rA...r
+00002a40: 5100 0000 7252 0000 0072 2900 0000 7254  Q...rR...r)...rT
+00002a50: 0000 0072 1c00 0000 722a 0000 0072 1700  ...r....r*...r..
+00002a60: 0000 7217 0000 0072 1800 0000 7273 0000  ..r....r....rs..
+00002a70: 0019 0100 0073 1000 0000 0001 1401 0801  .....s..........
+00002a80: 0401 1403 0401 0e02 0e01 7a17 5374 616e  ..........z.Stan
+00002a90: 7a61 5772 6170 7065 722e 7365 6e74 696d  zaWrapper.sentim
+00002aa0: 656e 74da 0c6d 756c 7469 6c69 6e67 7561  ent..multilingua
+00002ab0: 6c63 0500 0000 0000 0000 0a00 0000 0700  lc..............
+00002ac0: 0000 4300 0000 7386 0000 0074 006a 0164  ..C...s....t.j.d
+00002ad0: 0164 028d 0101 0074 027c 0264 037c 037c  .d.....t.|.d.|.|
+00002ae0: 047c 006a 0364 048d 057d 057c 017d 0664  .|.j.d...}.|.}.d
+00002af0: 0564 0684 007c 0644 0083 017d 067c 057c  .d...|.D...}.|.|
+00002b00: 0683 0101 007c 006a 0472 5874 0564 076a  .....|.j.rXt.d.j
+00002b10: 0664 0864 0984 007c 0644 0083 0183 0183  .d.d...|.D......
+00002b20: 0101 0067 007d 0778 247c 0644 005d 1c7d  ...g.}.x$|.D.].}
+00002b30: 087c 086a 077c 086a 0864 0a9c 027d 097c  .|.j.|.j.d...}.|
+00002b40: 076a 097c 0983 0101 0071 6257 007c 0753  .j.|.....qbW.|.S
+00002b50: 0029 0b4e 7275 0000 0029 0172 3a00 0000  .).Nru...).r:...
+00002b60: 5a06 6c61 6e67 6964 2905 723a 0000 0072  Z.langid).r:...r
+00002b70: 4000 0000 da11 6c61 6e67 6964 5f63 6c65  @.....langid_cle
+00002b80: 616e 5f74 6578 7472 4100 0000 723e 0000  an_textrA...r>..
+00002b90: 0063 0100 0000 0000 0000 0200 0000 0600  .c..............
+00002ba0: 0000 5300 0000 7318 0000 0067 007c 005d  ..S...s....g.|.]
+00002bb0: 107d 0174 0067 007c 0164 008d 0291 0271  .}.t.g.|.d.....q
+00002bc0: 0453 0029 0129 0172 1f00 0000 2901 7204  .S.).).r....).r.
+00002bd0: 0000 0029 0272 4900 0000 721f 0000 0072  ...).rI...r....r
+00002be0: 1700 0000 7217 0000 0072 1800 0000 724a  ....r....r....rJ
+00002bf0: 0000 002a 0100 0073 0200 0000 0600 7a26  ...*...s......z&
+00002c00: 5374 616e 7a61 5772 6170 7065 722e 6c61  StanzaWrapper.la
+00002c10: 6e67 2e3c 6c6f 6361 6c73 3e2e 3c6c 6973  ng.<locals>.<lis
+00002c20: 7463 6f6d 703e 722d 0000 0063 0100 0000  tcomp>r-...c....
+00002c30: 0000 0000 0200 0000 0400 0000 7300 0000  ............s...
+00002c40: 7320 0000 007c 005d 187d 017c 016a 009b  s ...|.].}.|.j..
+00002c50: 0064 007c 016a 019b 009d 0356 0001 0071  .d.|.j.....V...q
+00002c60: 0264 0153 0029 02fa 0109 4e29 0272 1f00  .d.S.)....N).r..
+00002c70: 0000 723a 0000 0029 0272 4900 0000 7252  ..r:...).rI...rR
+00002c80: 0000 0072 1700 0000 7217 0000 0072 1800  ...r....r....r..
+00002c90: 0000 fa09 3c67 656e 6578 7072 3e2d 0100  ....<genexpr>-..
+00002ca0: 0073 0200 0000 0400 7a25 5374 616e 7a61  .s......z%Stanza
+00002cb0: 5772 6170 7065 722e 6c61 6e67 2e3c 6c6f  Wrapper.lang.<lo
+00002cc0: 6361 6c73 3e2e 3c67 656e 6578 7072 3e29  cals>.<genexpr>)
+00002cd0: 0272 1f00 0000 723a 0000 0029 0a72 1300  .r....r:...).r..
+00002ce0: 0000 723b 0000 0072 0500 0000 723e 0000  ..r;...r....r>..
+00002cf0: 0072 3d00 0000 724e 0000 0072 5a00 0000  .r=...rN...rZ...
+00002d00: 721f 0000 0072 3a00 0000 721e 0000 0029  r....r:...r....)
+00002d10: 0a72 1600 0000 da09 6c69 7374 5f74 6578  .r......list_tex
+00002d20: 7472 3a00 0000 7276 0000 0072 4100 0000  tr:...rv...rA...
+00002d30: 7251 0000 00da 0464 6f63 7372 2900 0000  rQ.....docsr)...
+00002d40: 7252 0000 0072 2a00 0000 7217 0000 0072  rR...r*...r....r
+00002d50: 1700 0000 7218 0000 0072 3a00 0000 2601  ....r....r:...&.
+00002d60: 0000 731a 0000 0000 010c 0114 0104 010e  ..s.............
+00002d70: 0108 0106 0118 0104 010a 0204 010a 020e  ................
+00002d80: 017a 1253 7461 6e7a 6157 7261 7070 6572  .z.StanzaWrapper
+00002d90: 2e6c 616e 674e 720b 0000 0063 0400 0000  .langNr....c....
+00002da0: 0000 0000 0a00 0000 0500 0000 4300 0000  ............C...
+00002db0: 73bc 0000 007c 0364 016b 0372 2878 1e7c  s....|.d.k.r(x.|
+00002dc0: 036a 0064 0283 0144 005d 107d 0474 016a  .j.d...D.].}.t.j
+00002dd0: 027c 0464 038d 0101 0071 1457 0074 0383  .|.d.....q.W.t..
+00002de0: 007d 057c 017d 067c 057c 0683 017d 0667  .}.|.}.|.|...}.g
+00002df0: 007d 0778 787c 0644 005d 707d 087c 006a  .}.xx|.D.]p}.|.j
+00002e00: 0472 8a74 0564 0483 0101 0074 0564 057c  .r.t.d.....t.d.|
+00002e10: 086a 069b 009d 0283 0101 0074 0564 067c  .j.........t.d.|
+00002e20: 086a 079b 009d 0283 0101 0074 057c 086a  .j.........t.|.j
+00002e30: 0864 0719 006a 0983 009b 0083 0101 007c  .d...j.........|
+00002e40: 086a 067c 086a 077c 0864 089c 037d 097c  .j.|.j.|.d...}.|
+00002e50: 0264 006b 0372 aa7c 027c 0983 0101 007c  .d.k.r.|.|.....|
+00002e60: 076a 0a7c 0983 0101 0071 4457 007c 0753  .j.|.....qDW.|.S
+00002e70: 0029 094e 720b 0000 00fa 012c 2901 723a  .).Nr......,).r:
+00002e80: 0000 007a 032d 2d2d 7a06 7465 7874 3a20  ...z.---z.text: 
+00002e90: 7a06 6c61 6e67 3a20 7201 0000 0029 0372  z.lang: r....).r
+00002ea0: 1f00 0000 723a 0000 0072 5200 0000 290b  ....r:...rR...).
+00002eb0: 7232 0000 0072 1300 0000 723b 0000 0072  r2...r....r;...r
+00002ec0: 0600 0000 723d 0000 0072 4e00 0000 721f  ....r=...rN...r.
+00002ed0: 0000 0072 3a00 0000 724d 0000 005a 1364  ...r:...rM...Z.d
+00002ee0: 6570 656e 6465 6e63 6965 735f 7374 7269  ependencies_stri
+00002ef0: 6e67 721e 0000 0029 0a72 1600 0000 7279  ngr....).r....ry
+00002f00: 0000 005a 0c66 756e 635f 7072 6f63 6573  ...Z.func_proces
+00002f10: 735a 0d64 6f77 6e6c 6f61 645f 6c61 6e67  sZ.download_lang
+00002f20: da01 6c72 5100 0000 727a 0000 0072 2900  ..lrQ...rz...r).
+00002f30: 0000 7252 0000 0072 2a00 0000 7217 0000  ..rR...r*...r...
+00002f40: 0072 1700 0000 7218 0000 00da 0a6c 616e  .r....r......lan
+00002f50: 675f 6d75 6c74 6937 0100 0073 2800 0000  g_multi7...s(...
+00002f60: 0001 0801 1001 1001 0601 0401 0801 0401  ................
+00002f70: 0a01 0601 0801 1001 1001 1402 0401 0401  ................
+00002f80: 0802 0801 0801 0e01 7a18 5374 616e 7a61  ........z.Stanza
+00002f90: 5772 6170 7065 722e 6c61 6e67 5f6d 756c  Wrapper.lang_mul
+00002fa0: 7469 6302 0000 0000 0000 000a 0000 0007  tic.............
+00002fb0: 0000 0043 0000 0073 5601 0000 7c01 6400  ...C...sV...|.d.
+00002fc0: 6b02 7314 7400 7c01 8301 6401 6b02 7220  k.s.t.|...d.k.r 
+00002fd0: 7401 6402 8301 0100 6400 5300 9001 782e  t.d.....d.S...x.
+00002fe0: 7402 7c01 8301 4400 9001 5d20 5c02 7d02  t.|...D...] \.}.
+00002ff0: 7d03 7401 7c02 8301 0100 7403 7c03 8301  }.t.|.....t.|...
+00003000: 7404 6b02 72ae 7405 7c01 6401 1900 6a06  t.k.r.t.|.d...j.
+00003010: 8300 8301 7d04 7401 6403 6404 6a07 7c04  ....}.t.d.d.j.|.
+00003020: 8301 1700 8301 0100 6700 7d05 7822 7c03  ........g.}.x"|.
+00003030: 6a06 8300 4400 5d16 7d06 7c05 6a08 7409  j...D.].}.|.j.t.
+00003040: 7c03 7c06 1900 8301 8301 0100 717a 5700  |.|.........qzW.
+00003050: 6404 6a07 7c05 8301 7d07 7401 6403 7c07  d.j.|...}.t.d.|.
+00003060: 9b00 9d02 8301 0100 712c 7403 7c03 8301  ........q,t.|...
+00003070: 7405 6b02 722c 7405 7c03 6401 1900 6a06  t.k.r,t.|.d...j.
+00003080: 8300 8301 7d04 7401 6403 6404 6a07 7c04  ....}.t.d.d.j.|.
+00003090: 8301 1700 8301 0100 7870 7402 7c03 8301  ........xpt.|...
+000030a0: 4400 5d64 5c02 7d08 7d09 7403 7c09 8301  D.]d\.}.}.t.|...
+000030b0: 7404 6b02 9001 7240 6700 7d05 7824 7c09  t.k...r@g.}.x$|.
+000030c0: 6a06 8300 4400 5d18 7d06 7c05 6a08 7409  j...D.].}.|.j.t.
+000030d0: 7c09 7c06 1900 8301 8301 0100 9001 710a  |.|...........q.
+000030e0: 5700 6404 6a07 7c05 8301 7d07 7401 6403  W.d.j.|...}.t.d.
+000030f0: 7c07 9b00 9d02 8301 0100 71e6 7401 6403  |.........q.t.d.
+00003100: 7c09 8302 0100 71e6 5700 712c 5700 6400  |.....q.W.q,W.d.
+00003110: 5300 2905 4e72 0100 0000 7a0a 4e6f 2052  S.).Nr....z.No R
+00003120: 6573 756c 7421 7a02 0909 7277 0000 0029  esult!z...rw...)
+00003130: 0ada 036c 656e 724e 0000 0072 4c00 0000  ...lenrN...rL...
+00003140: 726d 0000 00da 0464 6963 74da 046c 6973  rm.....dict..lis
+00003150: 74da 046b 6579 7372 5a00 0000 721e 0000  t..keysrZ...r...
+00003160: 0072 5000 0000 290a 7216 0000 00da 0672  .rP...).r......r
+00003170: 6573 756c 745a 0369 6478 da04 6974 656d  esultZ.idx..item
+00003180: 5a06 6669 656c 6473 5a06 6c69 7374 5f76  Z.fieldsZ.list_v
+00003190: da01 6b72 3400 0000 5a04 6964 7831 5a02  ..kr4...Z.idx1Z.
+000031a0: 6c69 7217 0000 0072 1700 0000 7218 0000  lir....r....r...
+000031b0: 00da 0c70 7269 6e74 5f72 6573 756c 744f  ...print_resultO
+000031c0: 0100 0073 3000 0000 0001 1401 0801 0401  ...s0...........
+000031d0: 1601 0801 0c01 1001 1201 0401 0e01 1601  ................
+000031e0: 0a01 1001 0c01 1001 1201 1202 0e01 0401  ................
+000031f0: 0e01 1802 0a01 1002 7a1a 5374 616e 7a61  ........z.Stanza
+00003200: 5772 6170 7065 722e 7072 696e 745f 7265  Wrapper.print_re
+00003210: 7375 6c74 2904 4646 4654 2903 7208 0000  sult).FFFT).r...
+00003220: 0072 3f00 0000 4629 0272 4200 0000 4629  .r?...F).rB...F)
+00003230: 0572 0800 0000 720d 0000 0046 4646 2905  .r....r....FFF).
+00003240: 7208 0000 0072 0d00 0000 4646 4629 0572  r....r....FFF).r
+00003250: 0800 0000 720d 0000 0046 4646 2901 4629  ....r....FFF).F)
+00003260: 0372 0800 0000 7258 0000 0046 2904 7242  .r....rX...F).rB
+00003270: 0000 0072 5d00 0000 4646 2904 7208 0000  ...r]...FF).r...
+00003280: 0072 6000 0000 4646 2903 7242 0000 0072  .r`...FF).rB...r
+00003290: 5d00 0000 4629 0372 0800 0000 7268 0000  ]...F).r....rh..
+000032a0: 0046 2904 7208 0000 0072 6c00 0000 4646  .F).r....rl...FF
+000032b0: 2904 7242 0000 0072 6c00 0000 4646 2903  ).rB...rl...FF).
+000032c0: 7242 0000 0072 6c00 0000 4629 0372 0800  rB...rl...F).r..
+000032d0: 0000 726c 0000 0046 2903 7242 0000 0072  ..rl...F).rB...r
+000032e0: 7200 0000 4629 0372 0800 0000 7272 0000  r...F).r....rr..
+000032f0: 0046 2903 7275 0000 0046 4629 024e 720b  .F).ru...FF).Nr.
+00003300: 0000 0029 1b72 3600 0000 7237 0000 0072  ...).r6...r7...r
+00003310: 3800 0000 7219 0000 0072 3b00 0000 723c  8...r....r;...r<
+00003320: 0000 0072 4300 0000 7244 0000 0072 4500  ...rC...rD...rE.
+00003330: 0000 720d 0000 0072 5500 0000 7256 0000  ..r....rU...rV..
+00003340: 0072 5700 0000 725c 0000 0072 5f00 0000  .rW...r\...r_...
+00003350: 725e 0000 0072 6700 0000 7266 0000 0072  r^...rg...rf...r
+00003360: 0f00 0000 726f 0000 0072 7100 0000 7270  ....ro...rq...rp
+00003370: 0000 0072 7400 0000 7273 0000 0072 3a00  ...rt...rs...r:.
+00003380: 0000 727d 0000 0072 8500 0000 7217 0000  ..r}...r....r...
+00003390: 0072 1700 0000 7217 0000 0072 1800 0000  .r....r....r....
+000033a0: 7239 0000 0058 0000 0073 3000 0000 0801  r9...X...s0.....
+000033b0: 0a08 0a03 0a03 0803 0803 0803 0a13 0a0b  ................
+000033c0: 0a12 0a13 0a12 0a03 0a13 0a03 0a14 0a0e  ................
+000033d0: 0a03 0a03 0a10 0a03 0a0d 0a11 0a18 7239  ..............r9
+000033e0: 0000 0029 0d72 1300 0000 5a0d 7374 616e  ...).r....Z.stan
+000033f0: 7a61 2e73 6572 7665 7272 0200 0000 7203  za.serverr....r.
+00003400: 0000 005a 1873 7461 6e7a 612e 6d6f 6465  ...Z.stanza.mode
+00003410: 6c73 2e63 6f6d 6d6f 6e2e 646f 6372 0400  ls.common.docr..
+00003420: 0000 5a14 7374 616e 7a61 2e70 6970 656c  ..Z.stanza.pipel
+00003430: 696e 652e 636f 7265 7205 0000 005a 1c73  ine.corer....Z.s
+00003440: 7461 6e7a 612e 7069 7065 6c69 6e65 2e6d  tanza.pipeline.m
+00003450: 756c 7469 6c69 6e67 7561 6c72 0600 0000  ultilingualr....
+00003460: 722f 0000 0072 0700 0000 7239 0000 0072  r/...r....r9...r
+00003470: 1700 0000 7217 0000 0072 1700 0000 7218  ....r....r....r.
+00003480: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
+00003490: 0073 0e00 0000 0801 1001 0c01 0c01 0c01  .s..............
+000034a0: 0801 0e51                                ...Q
```

### Comparing `ner-kit-0.0.5a1/src/ner_kit.egg-info/PKG-INFO` & `ner-kit-0.0.5a2/src/ner_kit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ner-kit
-Version: 0.0.5a1
+Version: 0.0.5a2
 Summary: Named Entity Recognition Toolkit
 Home-page: https://github.com/dhchenx/ner-kit
 Author: Donghua Chen
 Author-email: douglaschan@126.com
 License: MIT
 Project-URL: Bug Reports, https://github.com/dhchenx/ner-kit/issues
 Project-URL: Source, https://github.com/dhchenx/ner-kit
```

### Comparing `ner-kit-0.0.5a1/src/ner_kit.egg-info/SOURCES.txt` & `ner-kit-0.0.5a2/src/ner_kit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

