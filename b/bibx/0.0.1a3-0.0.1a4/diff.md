# Comparing `tmp/bibx-0.0.1a3.tar.gz` & `tmp/bibx-0.0.1a4.tar.gz`

## Comparing `bibx-0.0.1a3.tar` & `bibx-0.0.1a4.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 bibx-0.0.1a3/.pre-commit-config.yaml
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 bibx-0.0.1a3/Makefile
--rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 bibx-0.0.1a3/.github/workflows/cd.yml
--rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 bibx-0.0.1a3/.github/workflows/ci.yml
--rw-r--r--   0        0        0  2221838 2020-02-02 00:00:00.000000 bibx-0.0.1a3/docs/examples/bit-pattern-savedrecs.txt
--rw-r--r--   0        0        0  5022778 2020-02-02 00:00:00.000000 bibx-0.0.1a3/docs/examples/scopus.bib
--rw-r--r--   0        0        0  2955913 2020-02-02 00:00:00.000000 bibx-0.0.1a3/docs/examples/scopus.ris
--rw-r--r--   0        0        0     4911 2020-02-02 00:00:00.000000 bibx-0.0.1a3/docs/examples/single-article.txt
--rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 bibx-0.0.1a3/src/bibx/__init__.py
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 bibx-0.0.1a3/src/bibx/__main__.py
--rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 bibx-0.0.1a3/src/bibx/exceptions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bibx-0.0.1a3/src/bibx/_entities/__init__.py
--rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 bibx-0.0.1a3/src/bibx/_entities/article.py
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 bibx-0.0.1a3/src/bibx/_entities/collection.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bibx-0.0.1a3/src/bibx/_entities/collection_builders/__init__.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 bibx-0.0.1a3/src/bibx/_entities/collection_builders/base.py
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 bibx-0.0.1a3/src/bibx/_entities/collection_builders/cross_ref.py
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 bibx-0.0.1a3/src/bibx/_entities/collection_builders/generic.py
--rw-r--r--   0        0        0     2571 2020-02-02 00:00:00.000000 bibx-0.0.1a3/src/bibx/_entities/collection_builders/scopus_bib.py
--rw-r--r--   0        0        0     5976 2020-02-02 00:00:00.000000 bibx-0.0.1a3/src/bibx/_entities/collection_builders/scopus_ris.py
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 bibx-0.0.1a3/src/bibx/_entities/collection_builders/simple.py
--rw-r--r--   0        0        0    13199 2020-02-02 00:00:00.000000 bibx-0.0.1a3/src/bibx/_entities/collection_builders/wos.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bibx-0.0.1a3/src/bibx/algorithms/__init__.py
--rw-r--r--   0        0        0    11115 2020-02-02 00:00:00.000000 bibx-0.0.1a3/src/bibx/algorithms/sap.py
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 bibx-0.0.1a3/tests/test_works.py
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 bibx-0.0.1a3/tests/algorithms/test_sap.py
--rw-r--r--   0        0        0     6876 2020-02-02 00:00:00.000000 bibx-0.0.1a3/tests/entities/collection_builders/test_scopus_bib.py
--rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 bibx-0.0.1a3/tests/entities/collection_builders/test_scopus_ris.py
--rw-r--r--   0        0        0     6580 2020-02-02 00:00:00.000000 bibx-0.0.1a3/tests/entities/collection_builders/test_wos.py
--rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 bibx-0.0.1a3/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 bibx-0.0.1a3/LICENSE
--rw-r--r--   0        0        0     1869 2020-02-02 00:00:00.000000 bibx-0.0.1a3/README.md
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 bibx-0.0.1a3/pyproject.toml
--rw-r--r--   0        0        0     2467 2020-02-02 00:00:00.000000 bibx-0.0.1a3/PKG-INFO
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 bibx-0.0.1a4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 bibx-0.0.1a4/Makefile
+-rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 bibx-0.0.1a4/.github/workflows/cd.yml
+-rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 bibx-0.0.1a4/.github/workflows/ci.yml
+-rw-r--r--   0        0        0  2221838 2020-02-02 00:00:00.000000 bibx-0.0.1a4/docs/examples/bit-pattern-savedrecs.txt
+-rw-r--r--   0        0        0  5022778 2020-02-02 00:00:00.000000 bibx-0.0.1a4/docs/examples/scopus.bib
+-rw-r--r--   0        0        0  2955913 2020-02-02 00:00:00.000000 bibx-0.0.1a4/docs/examples/scopus.ris
+-rw-r--r--   0        0        0     4911 2020-02-02 00:00:00.000000 bibx-0.0.1a4/docs/examples/single-article.txt
+-rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 bibx-0.0.1a4/src/bibx/__init__.py
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 bibx-0.0.1a4/src/bibx/__main__.py
+-rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 bibx-0.0.1a4/src/bibx/exceptions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bibx-0.0.1a4/src/bibx/_entities/__init__.py
+-rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 bibx-0.0.1a4/src/bibx/_entities/article.py
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 bibx-0.0.1a4/src/bibx/_entities/collection.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bibx-0.0.1a4/src/bibx/_entities/collection_builders/__init__.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 bibx-0.0.1a4/src/bibx/_entities/collection_builders/base.py
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 bibx-0.0.1a4/src/bibx/_entities/collection_builders/cross_ref.py
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 bibx-0.0.1a4/src/bibx/_entities/collection_builders/generic.py
+-rw-r--r--   0        0        0     2571 2020-02-02 00:00:00.000000 bibx-0.0.1a4/src/bibx/_entities/collection_builders/scopus_bib.py
+-rw-r--r--   0        0        0     6202 2020-02-02 00:00:00.000000 bibx-0.0.1a4/src/bibx/_entities/collection_builders/scopus_ris.py
+-rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 bibx-0.0.1a4/src/bibx/_entities/collection_builders/simple.py
+-rw-r--r--   0        0        0    13156 2020-02-02 00:00:00.000000 bibx-0.0.1a4/src/bibx/_entities/collection_builders/wos.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bibx-0.0.1a4/src/bibx/algorithms/__init__.py
+-rw-r--r--   0        0        0    11115 2020-02-02 00:00:00.000000 bibx-0.0.1a4/src/bibx/algorithms/sap.py
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 bibx-0.0.1a4/tests/test_works.py
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 bibx-0.0.1a4/tests/algorithms/test_sap.py
+-rw-r--r--   0        0        0     6876 2020-02-02 00:00:00.000000 bibx-0.0.1a4/tests/entities/collection_builders/test_scopus_bib.py
+-rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 bibx-0.0.1a4/tests/entities/collection_builders/test_scopus_ris.py
+-rw-r--r--   0        0        0     6580 2020-02-02 00:00:00.000000 bibx-0.0.1a4/tests/entities/collection_builders/test_wos.py
+-rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 bibx-0.0.1a4/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 bibx-0.0.1a4/LICENSE
+-rw-r--r--   0        0        0     1869 2020-02-02 00:00:00.000000 bibx-0.0.1a4/README.md
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 bibx-0.0.1a4/pyproject.toml
+-rw-r--r--   0        0        0     2467 2020-02-02 00:00:00.000000 bibx-0.0.1a4/PKG-INFO
```

### Comparing `bibx-0.0.1a3/.pre-commit-config.yaml` & `bibx-0.0.1a4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `bibx-0.0.1a3/.github/workflows/cd.yml` & `bibx-0.0.1a4/.github/workflows/cd.yml`

 * *Files identical despite different names*

### Comparing `bibx-0.0.1a3/.github/workflows/ci.yml` & `bibx-0.0.1a4/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `bibx-0.0.1a3/docs/examples/bit-pattern-savedrecs.txt` & `bibx-0.0.1a4/docs/examples/bit-pattern-savedrecs.txt`

 * *Files identical despite different names*

### Comparing `bibx-0.0.1a3/docs/examples/scopus.bib` & `bibx-0.0.1a4/docs/examples/scopus.bib`

 * *Files identical despite different names*

### Comparing `bibx-0.0.1a3/docs/examples/scopus.ris` & `bibx-0.0.1a4/docs/examples/scopus.ris`

 * *Files identical despite different names*

### Comparing `bibx-0.0.1a3/docs/examples/single-article.txt` & `bibx-0.0.1a4/docs/examples/single-article.txt`

 * *Files identical despite different names*

### Comparing `bibx-0.0.1a3/src/bibx/__init__.py` & `bibx-0.0.1a4/src/bibx/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     "Sap",
     "read_scopus_bib",
     "read_scopus_ris",
     "read_wos",
     "read_any",
 ]
 
-__version__ = "0.0.1a3"
+__version__ = "0.0.1a4"
 
 
 def read_scopus_bib(*files: TextIO) -> Collection:
     """
     Takes any number of bibtex files from scopus and generates a collection.
 
     :param files: Scopus bib files open.
```

### Comparing `bibx-0.0.1a3/src/bibx/exceptions.py` & `bibx-0.0.1a4/src/bibx/exceptions.py`

 * *Files identical despite different names*

### Comparing `bibx-0.0.1a3/src/bibx/_entities/article.py` & `bibx-0.0.1a4/src/bibx/_entities/article.py`

 * *Files identical despite different names*

### Comparing `bibx-0.0.1a3/src/bibx/_entities/collection.py` & `bibx-0.0.1a4/src/bibx/_entities/collection.py`

 * *Files identical despite different names*

### Comparing `bibx-0.0.1a3/src/bibx/_entities/collection_builders/scopus_bib.py` & `bibx-0.0.1a4/src/bibx/_entities/collection_builders/scopus_bib.py`

 * *Files identical despite different names*

### Comparing `bibx-0.0.1a3/src/bibx/_entities/collection_builders/scopus_ris.py` & `bibx-0.0.1a4/src/bibx/_entities/collection_builders/scopus_ris.py`

 * *Files 4% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
     def build(self) -> Collection:
         articles = self._get_articles_from_files()
         return Collection(list(articles))
 
     def _get_articles_from_files(self) -> Iterable[Article]:
         for file in self._files:
-            yield from self.parse_file(file)
+            yield from self._parse_file(file)
 
     @staticmethod
     def _find_volume_info(ref: str) -> Tuple[Dict[str, str], str]:
         volume_pattern = re.compile(r"(?P<volume>\d+)( \((?P<issue>.+?)\))?")
         page_pattern = re.compile(r"(pp?\. (?P<page>\w+)(-[^,\s]+)?)")
         page = page_pattern.search(ref)
         last_index = 0
@@ -86,48 +86,48 @@
         result = re.search(pattern, ref)
         if result is None or "doi" not in result.groupdict():
             return None, ref
         doi = result.groupdict()["doi"]
         return f"DOI {doi}", ref[result.lastindex :]
 
     @classmethod
-    def _scopus_ref_to_isi(cls, scopusref: str) -> Article:
+    def _article_form_reference(cls, scopusref: str) -> Article:
         authors, year, rest = re.split(r"(\(\d{4}\))", scopusref, maxsplit=1)
         first_name, last_name, *_ = authors.split(", ")
         year = year[1:-1]
         journal, rest = rest.split(", ", 1)
         volume_info, rest = cls._find_volume_info(rest)
         doi, _ = cls._find_doi(scopusref)
-        if not year:
+        if not authors or not year:
             raise MissingCriticalInformation()
         return Article(
             authors=[f"{first_name} {last_name.replace(' ', '').replace('.', '')}"],
             year=int(year),
             journal=journal.strip().replace(".", "").upper()
             if not journal.isspace()
             else None,
             volume=volume_info.get("volume"),
             page=volume_info.get("page"),
             doi=doi,
         )
 
     @classmethod
-    def parse_references(cls, refs: List[str]) -> List[Article]:
+    def _parse_references(cls, refs: List[str]) -> List[Article]:
         if not refs:
             return []
         result = []
         for ref in refs:
             try:
-                result.append(cls._scopus_ref_to_isi(ref))
+                result.append(cls._article_form_reference(ref))
             except (KeyError, IndexError, TypeError, ValueError):
                 logging.debug(f"Ignoring invalid reference {ref}")
         return result
 
     @staticmethod
-    def ris_to_dict(record: str) -> Dict[str, List[str]]:
+    def _ris_to_dict(record: str) -> Dict[str, List[str]]:
         RIS_PATTERN = re.compile(
             r"^(((?P<key>[A-Z0-9]{2}))[ ]{2}-[ ]{1})?(?P<value>(.*))$"
         )
         parsed = defaultdict(list)
         current = None
 
         for line in record.split("\n"):
@@ -147,36 +147,40 @@
                 else:
                     current = data["key"]
             if value and current:
                 parsed[current].append(data.get("value", ""))
         return dict(parsed)
 
     @classmethod
-    def parse_record(cls, record: str) -> Article:
-        data = cls.ris_to_dict(record)
+    def _parse_record(cls, record: str) -> Article:
+        data = cls._ris_to_dict(record)
         year = _int_or_nothing(data.get("PY", []))
-        if not year:
+        authors = data.get("AU", [])
+        if not authors or not year:
             raise MissingCriticalInformation()
         return Article(
             title=_joined(data.get("TI")),
-            authors=data.get("AU", []),
+            authors=authors,
             year=year,
             journal=_joined(data.get("J2")),
             volume=_joined(data.get("VL")),
             issue=_joined(data.get("IS")),
             page=_joined(data.get("SP")),
             doi=_joined(data.get("DO")),
             keywords=data.get("KW", []),
-            references=cls.parse_references(data.get("N1:References", [])),
+            references=cls._parse_references(data.get("N1:References", [])),
             sources={"scopus"},
             extra=data,
         )
 
     @classmethod
-    def parse_file(cls, file: TextIO) -> Iterable[Article]:
+    def _parse_file(cls, file: TextIO) -> Iterable[Article]:
         if not _size(file):
             return []
         for item in file.read().split("\n\n"):
             if item.isspace():
                 continue
-            article = cls.parse_record(item.strip())
-            yield article
+            try:
+                article = cls._parse_record(item.strip())
+                yield article
+            except MissingCriticalInformation:
+                logger.info("Missing critical information for record %s", item)
```

### Comparing `bibx-0.0.1a3/src/bibx/_entities/collection_builders/wos.py` & `bibx-0.0.1a4/src/bibx/_entities/collection_builders/wos.py`

 * *Files 2% similar despite different names*

```diff
@@ -333,27 +333,27 @@
             volume=processed.get("volume"),
             page=processed.get("beginning_page"),
             doi=processed.get("DOI"),
             extra=processed,
             sources={reference},
         )
 
-    @staticmethod
-    def _parse_all(article_data: Dict[str, List[str]]) -> Mapping[str, Any]:
+    @classmethod
+    def _parse_all(cls, article_data: Dict[str, List[str]]) -> Mapping[str, Any]:
         processed_data = {}
         for key, values in article_data.items():
-            parsed_values_dict = WosCollectionBuilder._parse(key, values)
+            parsed_values_dict = cls._parse(key, values)
             processed_data.update(parsed_values_dict)
         return processed_data
 
-    @staticmethod
-    def _parse(key: str, value: List[str]) -> Dict:
+    @classmethod
+    def _parse(cls, key: str, value: List[str]) -> Dict:
         if key in {"FN", "VR", "ER"}:
             return {}
 
-        if key in WosCollectionBuilder.FIELDS:
-            field = WosCollectionBuilder.FIELDS[key]
+        if key in cls.FIELDS:
+            field = cls.FIELDS[key]
             parsed_value = field.parse(value)
             return {new_key: parsed_value for new_key in [field.key, *field.aliases]}
 
         logger.info(f"Found an unknown field with key {key} and value {value}")
         return {key: _ident(value)}
```

### Comparing `bibx-0.0.1a3/src/bibx/algorithms/sap.py` & `bibx-0.0.1a4/src/bibx/algorithms/sap.py`

 * *Files identical despite different names*

### Comparing `bibx-0.0.1a3/tests/algorithms/test_sap.py` & `bibx-0.0.1a4/tests/algorithms/test_sap.py`

 * *Files identical despite different names*

### Comparing `bibx-0.0.1a3/tests/entities/collection_builders/test_scopus_bib.py` & `bibx-0.0.1a4/tests/entities/collection_builders/test_scopus_bib.py`

 * *Files identical despite different names*

### Comparing `bibx-0.0.1a3/tests/entities/collection_builders/test_scopus_ris.py` & `bibx-0.0.1a4/tests/entities/collection_builders/test_scopus_ris.py`

 * *Files identical despite different names*

### Comparing `bibx-0.0.1a3/tests/entities/collection_builders/test_wos.py` & `bibx-0.0.1a4/tests/entities/collection_builders/test_wos.py`

 * *Files identical despite different names*

### Comparing `bibx-0.0.1a3/.gitignore` & `bibx-0.0.1a4/.gitignore`

 * *Files identical despite different names*

### Comparing `bibx-0.0.1a3/LICENSE` & `bibx-0.0.1a4/LICENSE`

 * *Files identical despite different names*

### Comparing `bibx-0.0.1a3/README.md` & `bibx-0.0.1a4/README.md`

 * *Files identical despite different names*

### Comparing `bibx-0.0.1a3/pyproject.toml` & `bibx-0.0.1a4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bibx-0.0.1a3/PKG-INFO` & `bibx-0.0.1a4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bibx
-Version: 0.0.1a3
+Version: 0.0.1a4
 Summary: Python bibliometric tools.
 Author-email: Core of Science Team <technology@coreofscience.org>
 License-Expression: MIT
 License-File: LICENSE
 Keywords: bibliometrics,science,text mining
 Requires-Dist: bibtexparser~=1.4.0
 Requires-Dist: networkx~=3.0
```

