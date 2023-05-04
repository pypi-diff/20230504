# Comparing `tmp/konsepy-0.0.5.tar.gz` & `tmp/konsepy-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "konsepy-0.0.5.tar", last modified: Mon Apr 17 20:39:17 2023, max compression
+gzip compressed data, was "konsepy-0.0.6.tar", last modified: Thu May  4 19:07:12 2023, max compression
```

## Comparing `konsepy-0.0.5.tar` & `konsepy-0.0.6.tar`

### file list

```diff
@@ -1,17 +1,18 @@
--rw-r--r--   0        0        0      996 2023-04-17 20:39:09.203511 konsepy-0.0.5/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0        0        0       41 2023-04-17 20:39:09.203511 konsepy-0.0.5/.gitignore
--rw-r--r--   0        0        0      607 2023-04-17 20:39:09.203511 konsepy-0.0.5/CHANGELOG.md
--rw-r--r--   0        0        0      335 2023-04-17 20:39:09.203511 konsepy-0.0.5/README.md
--rw-r--r--   0        0        0      905 2023-04-17 20:39:09.203511 konsepy-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      110 2023-04-17 20:39:09.203511 konsepy-0.0.5/src/konsepy/__init__.py
--rw-r--r--   0        0        0     4077 2023-04-17 20:39:09.203511 konsepy-0.0.5/src/konsepy/bio_tag.py
--rw-r--r--   0        0        0     2888 2023-04-17 20:39:09.203511 konsepy-0.0.5/src/konsepy/cli.py
--rw-r--r--   0        0        0      104 2023-04-17 20:39:09.203511 konsepy-0.0.5/src/konsepy/constants.py
--rw-r--r--   0        0        0     4249 2023-04-17 20:39:09.203511 konsepy-0.0.5/src/konsepy/get_text_snippets.py
--rw-r--r--   0        0        0     1564 2023-04-17 20:39:09.203511 konsepy-0.0.5/src/konsepy/importer.py
--rw-r--r--   0        0        0     5284 2023-04-17 20:39:09.203511 konsepy-0.0.5/src/konsepy/regex.py
--rw-r--r--   0        0        0     2390 2023-04-17 20:39:09.203511 konsepy-0.0.5/src/konsepy/run_all.py
--rw-r--r--   0        0        0      654 2023-04-17 20:39:09.203511 konsepy-0.0.5/src/konsepy/rxutils.py
--rw-r--r--   0        0        0     3738 2023-04-17 20:39:09.203511 konsepy-0.0.5/src/konsepy/textio.py
--rw-r--r--   0        0        0      202 2023-04-17 20:39:09.203511 konsepy-0.0.5/src/konsepy/types.py
--rw-r--r--   0        0        0     1212 1970-01-01 00:00:00.000000 konsepy-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      996 2023-05-04 19:07:07.877667 konsepy-0.0.6/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0        0        0       41 2023-05-04 19:07:07.877667 konsepy-0.0.6/.gitignore
+-rw-r--r--   0        0        0      803 2023-05-04 19:07:07.877667 konsepy-0.0.6/CHANGELOG.md
+-rw-r--r--   0        0        0      335 2023-05-04 19:07:07.877667 konsepy-0.0.6/README.md
+-rw-r--r--   0        0        0      905 2023-05-04 19:07:07.877667 konsepy-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0      110 2023-05-04 19:07:07.877667 konsepy-0.0.6/src/konsepy/__init__.py
+-rw-r--r--   0        0        0     4116 2023-05-04 19:07:07.877667 konsepy-0.0.6/src/konsepy/bio_tag.py
+-rw-r--r--   0        0        0     3056 2023-05-04 19:07:07.877667 konsepy-0.0.6/src/konsepy/cli.py
+-rw-r--r--   0        0        0      104 2023-05-04 19:07:07.877667 konsepy-0.0.6/src/konsepy/constants.py
+-rw-r--r--   0        0        0     4480 2023-05-04 19:07:07.877667 konsepy-0.0.6/src/konsepy/get_text_snippets.py
+-rw-r--r--   0        0        0     1564 2023-05-04 19:07:07.877667 konsepy-0.0.6/src/konsepy/importer.py
+-rw-r--r--   0        0        0     5284 2023-05-04 19:07:07.877667 konsepy-0.0.6/src/konsepy/regex.py
+-rw-r--r--   0        0        0     2469 2023-05-04 19:07:07.877667 konsepy-0.0.6/src/konsepy/run_all.py
+-rw-r--r--   0        0        0      654 2023-05-04 19:07:07.877667 konsepy-0.0.6/src/konsepy/rxutils.py
+-rw-r--r--   0        0        0     5285 2023-05-04 19:07:07.877667 konsepy-0.0.6/src/konsepy/textio.py
+-rw-r--r--   0        0        0      202 2023-05-04 19:07:07.877667 konsepy-0.0.6/src/konsepy/types.py
+-rw-r--r--   0        0        0     1297 2023-05-04 19:07:07.877667 konsepy-0.0.6/test/build.ps1
+-rw-r--r--   0        0        0     1212 1970-01-01 00:00:00.000000 konsepy-0.0.6/PKG-INFO
```

### Comparing `konsepy-0.0.5/.github/workflows/publish-to-pypi.yml` & `konsepy-0.0.6/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `konsepy-0.0.5/CHANGELOG.md` & `konsepy-0.0.6/CHANGELOG.md`

 * *Files 14% similar despite different names*

```diff
@@ -11,12 +11,19 @@
 * `Added`: for new features.
 * `Changed`: for changes in existing functionality.
 * `Deprecated`: for soon-to-be removed features.
 * `Removed`: for now removed features.
 * `Fixed`: for any bug fixes.
 * `Security`: in case of vulnerabilities.
 
+## [0.0.6] - 2023-05-04
+
+### Added
+
+* Added `noteorder_label` to allow notes to appear in a delined form (with multiple rows for a note)
+* Powershell script to test konsepy_nlp_template tutorial
+
 ## [0.0.5] - 2023-04-17
 
 ### Fixed
 
 * Argument descriptions for column labels
```

### Comparing `konsepy-0.0.5/pyproject.toml` & `konsepy-0.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `konsepy-0.0.5/src/konsepy/bio_tag.py` & `konsepy-0.0.6/src/konsepy/bio_tag.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,16 @@
         raise ValueError('Specify name of package.')
     return {concept.name: concept.run_func for concept in get_all_concepts(package_name)}
 
 
 def get_bio_tags(input_files, outdir: Path, *, package_name: str = None, regexes: RegexDict = None,
                  sentence_model='senter',
                  id_label=ID_LABEL, noteid_label=NOTEID_LABEL,
-                 notedate_label=NOTEDATE_LABEL, notetext_label=NOTETEXT_LABEL):
+                 notedate_label=NOTEDATE_LABEL, notetext_label=NOTETEXT_LABEL,
+                 noteorder_label=None):
     """
 
     """
     outdir.mkdir(exist_ok=True)
 
     # prepare sentence splitter
     nlp = get_pipeline(sentence_model)
```

### Comparing `konsepy-0.0.5/src/konsepy/cli.py` & `konsepy-0.0.6/src/konsepy/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -49,8 +49,10 @@
                         help='Column label for individual id')
     parser.add_argument('--noteid-label', default=NOTEID_LABEL,
                         help='Column label for note id')
     parser.add_argument('--notedate-label', default=NOTEDATE_LABEL,
                         help='Column label for date of note')
     parser.add_argument('--notetext-label', default=NOTETEXT_LABEL,
                         help='Column label for note text')
+    parser.add_argument('--noteorder-label', default=None,
+                        help='Specify column that enumerates the order of multiple parts of a single note.')
     return parser
```

### Comparing `konsepy-0.0.5/src/konsepy/get_text_snippets.py` & `konsepy-0.0.6/src/konsepy/get_text_snippets.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,29 +9,31 @@
 from konsepy.importer import get_all_concepts
 from konsepy.textio import iterate_csv_file
 
 
 def get_text_snippets_regexes(input_files, outdir, regexes, *, start_after=0, stop_after=None, window_size=50,
                               id_label=ID_LABEL, noteid_label=NOTEID_LABEL,
                               notedate_label=NOTEDATE_LABEL, notetext_label=NOTETEXT_LABEL,
+                              noteorder_label=None,
                               select_probability=1.0, label='snippets', stop_after_regex_count=None, **kwargs):
     dt = datetime.datetime.now().strftime('%Y%m%d_%H%M%S')
     logger.warning('Snippets will have spaces normalized:'
                    ' multiple spaces/newlines/tabs will be converted'
                    ' to a single space in the output.')
     rx_count = 0
     outdir.mkdir(exist_ok=True)
     with open(outdir / f'{label}_{dt}.csv', 'w', newline='') as out:
         writer = csv.writer(out)
         writer.writerow(['id', 'studyid', 'note_id', 'date', 'regex_name', 'precontext', 'term', 'postcontext'])
         for _, studyid, note_id, note_date, text in iterate_csv_file(
                 input_files, start_after=start_after, stop_after=stop_after,
                 id_label=id_label, noteid_label=noteid_label,
                 notetext_label=notetext_label, notedate_label=notedate_label,
-                select_probability=select_probability
+                noteorder_label=noteorder_label,
+                select_probability=select_probability,
         ):
             text = ' '.join(text.split())  # remove newlines, etc. (bad for snippets in Excel)
             for regex_ in regexes:
                 name, regex = regex_.split('==')
                 if isinstance(regex, str):
                     regex = re.compile(regex, re.I)
                 for m in regex.finditer(text):
@@ -52,14 +54,15 @@
                         return
 
 
 def get_text_snippets_for_concept_algorithm(package, input_files, outdir, *, concepts=None,
                                             start_after=0, stop_after=None, window_size=50,
                                             id_label=ID_LABEL, noteid_label=NOTEID_LABEL,
                                             notedate_label=NOTEDATE_LABEL, notetext_label=NOTETEXT_LABEL,
+                                            noteorder_label=None,
                                             select_probability=1.0, label='snippets', stop_after_regex_count=None,
                                             **kwargs):
     regexes = [(regex, category)
                for concept in get_all_concepts(package, *concepts)
                for regex, category in concept.regexes]
 
     get_text_snippets_regexes(input_files, outdir, regexes,
@@ -67,14 +70,15 @@
                               stop_after=stop_after,
                               window_size=window_size,
                               select_probability=select_probability,
                               id_label=id_label,
                               noteid_label=noteid_label,
                               notedate_label=notedate_label,
                               notetext_label=notetext_label,
+                              noteorder_label=noteorder_label,
                               label=label,
                               stop_after_regex_count=stop_after_regex_count,
                               )
 
 
 def get_text_snippets_cli(package_name=None):
     kwargs = snippet_cli()
```

### Comparing `konsepy-0.0.5/src/konsepy/importer.py` & `konsepy-0.0.6/src/konsepy/importer.py`

 * *Files identical despite different names*

### Comparing `konsepy-0.0.5/src/konsepy/regex.py` & `konsepy-0.0.6/src/konsepy/regex.py`

 * *Files identical despite different names*

### Comparing `konsepy-0.0.5/src/konsepy/run_all.py` & `konsepy-0.0.6/src/konsepy/run_all.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from konsepy.regex import extract_categories
 from konsepy.textio import iterate_csv_file, output_results
 
 
 def run_all(input_files, outdir: pathlib.Path, package_name: str, *,
             id_label=ID_LABEL, noteid_label=NOTEID_LABEL,
             notedate_label=NOTEDATE_LABEL, notetext_label=NOTETEXT_LABEL,
+            noteorder_label=None,
             ):
     dt = datetime.datetime.now().strftime("%Y%m%d_%H%M%S")
     curr_outdir = outdir / f'run_all_{dt}'
     curr_outdir.mkdir(parents=True)
     logger.add(curr_outdir / f'run_all_{dt}.log')
     count = 0  # default value; received from forloop below
     cat_counter_notes = Counter()
@@ -27,14 +28,15 @@
     unique_mrns = set()
     concepts = list(get_all_concepts(package_name))
     logger.info(f'Loaded {len(concepts)} concepts for processing.')
     for count, studyid, note_id, note_date, text in iterate_csv_file(
             input_files,
             id_label=id_label, noteid_label=noteid_label,
             notedate_label=notedate_label, notetext_label=notetext_label,
+            noteorder_label=noteorder_label,
     ):
         if count % 10000 == 0:
             logger.info(f'Completed {count} records for {len(unique_mrns)} MRNs ({datetime.datetime.now()})')
 
         for concept in concepts:
             extract_categories(
                 studyid, note_id, text, concept.run_func,
```

### Comparing `konsepy-0.0.5/src/konsepy/rxutils.py` & `konsepy-0.0.6/src/konsepy/rxutils.py`

 * *Files identical despite different names*

### Comparing `konsepy-0.0.5/src/konsepy/textio.py` & `konsepy-0.0.6/src/konsepy/textio.py`

 * *Files 25% similar despite different names*

```diff
@@ -9,55 +9,92 @@
 
 from konsepy.constants import NOTEDATE_LABEL, ID_LABEL, NOTEID_LABEL, NOTETEXT_LABEL
 
 
 def iterate_csv_file(input_files, *, start_after=0, stop_after=None,
                      id_label=ID_LABEL, noteid_label=NOTEID_LABEL,
                      notedate_label=NOTEDATE_LABEL, notetext_label=NOTETEXT_LABEL,
+                     noteorder_label=None,
                      select_probability=1.0, encoding='latin1'):
     """Return count, mrn, note_id, text for each row in csv file"""
     count = 0
     total_count = 0
     for input_file in input_files:
         func = _extract_sas_file if input_file.endswith('sas7bdat') else _extract_csv_file
-        for mrn, text, note_id, date in func(input_file, encoding, id_label, noteid_label, notedate_label,
-                                             notetext_label):
+        for mrn, text, note_id, date in _deline_lines(
+                func, input_file, encoding, id_label, noteid_label,
+                notedate_label, notetext_label, noteorder_label):
             if random.random() > select_probability:
                 continue
             total_count += 1
             if start_after >= total_count:
                 continue
             count += 1
             yield count, mrn, note_id, date, text
             if stop_after and count > stop_after:
                 return
 
 
-def _extract_sas_file(input_file, encoding, id_label, noteid_label, notedate_label, notetext_label):
+def _deline_lines(func, input_file, encoding, mrn_label, noteid_label,
+                  notedate_label, notetext_label, noteorder_label=None):
+    # variables for delining notes
+    curr_id = None
+    curr_mrn = None
+    curr_date = None
+    curr_doc = []
+    for mrn, text, note_id, date, order in func(
+            input_file, encoding, mrn_label, noteid_label, notedate_label,
+            notetext_label, noteorder_label
+    ):
+        if not order:  # skip delining
+            yield mrn, text, note_id, date
+        else:
+            if curr_id is None:
+                curr_id = note_id
+                curr_mrn = mrn
+                curr_date = date
+            elif note_id != curr_id:
+                yield curr_mrn, ' '.join(text for _, _, text in sorted(curr_doc)), curr_id, curr_date
+                curr_id = note_id
+                curr_mrn = mrn
+                curr_date = date
+                curr_doc = []
+            if isinstance(text, float) or not text:
+                continue  # skip empty text
+            curr_doc.append((note_id, order, text))  # keep track of all text associated with this note
+    if curr_id is not None:
+        yield curr_mrn, ' '.join(text for _, _, text in sorted(curr_doc)), curr_id, curr_date
+
+
+def _extract_sas_file(input_file, encoding, id_label, noteid_label,
+                      notedate_label, notetext_label, noteorder_label=None):
     with SAS7BDAT(input_file, skip_header=False, encoding=encoding) as fh:
         header = []
         for row in fh:
             if not header:
                 header = row
                 continue
             mrn = row[header.index(id_label)]
             date = row[header.index(notedate_label)] if notedate_label else ''
             text = row[header.index(noteid_label)]
             noteid = row[header.index(notetext_label)]
-            yield mrn, text, noteid, date
+            order = row[header.index(noteorder_label)] if noteorder_label else None
+            yield mrn, text, noteid, date, order
 
 
-def _extract_csv_file(input_file, encoding, id_label, noteid_label, notedate_label, notetext_label):
+def _extract_csv_file(input_file, encoding, id_label, noteid_label, notedate_label,
+                      notetext_label, noteorder_label=None):
     with open(input_file, encoding=encoding) as fh:
         for row in csv.DictReader(fh):
             text = row[notetext_label]
             mrn = row[id_label]
             date = row.get(notedate_label, '')
             note_id = row[noteid_label]
-            yield mrn, text, note_id, date
+            order = row.get(noteorder_label, '')
+            yield mrn, text, note_id, date, order
 
 
 def output_results(outdir, *, not_found_text=None,
                    note_counter=None, cat_counter_mrns=None,
                    category_enums=None, note_to_cat=None, mrn_to_cat=None):
     categories = [e for category_enum in category_enums for e in category_enum]
     if not_found_text is not None:
```

### Comparing `konsepy-0.0.5/PKG-INFO` & `konsepy-0.0.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: konsepy
-Version: 0.0.5
+Version: 0.0.6
 Summary: Framework for build NLP information extraction systems using regular expressions.
 Keywords: nlp
 Author-email: dcronkite <dcronkite+pypi@gmail.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
```

