# Comparing `tmp/timerdo-0.0.3.tar.gz` & `tmp/timerdo-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timerdo-0.0.3.tar", last modified: Fri Apr  7 10:44:27 2023, max compression
+gzip compressed data, was "timerdo-0.0.4.tar", last modified: Thu May  4 19:59:54 2023, max compression
```

## Comparing `timerdo-0.0.3.tar` & `timerdo-0.0.4.tar`

### file list

```diff
@@ -1,53 +1,44 @@
--rw-r--r--   0        0        0       99 2023-04-07 10:44:07.420468 timerdo-0.0.3/.flake8
--rw-r--r--   0        0        0      569 2023-04-07 10:44:07.420468 timerdo-0.0.3/.github/workflows/publish_docs.yml
--rw-r--r--   0        0        0      506 2023-04-07 10:44:07.420468 timerdo-0.0.3/.github/workflows/publish_pypi.yml
--rw-r--r--   0        0        0      566 2023-04-07 10:44:07.420468 timerdo-0.0.3/.github/workflows/test_suite.yml
--rw-r--r--   0        0        0      101 2023-04-07 10:44:07.420468 timerdo-0.0.3/.gitignore
--rw-r--r--   0        0        0      203 2023-04-07 10:44:07.420468 timerdo-0.0.3/Makefile
--rw-r--r--   0        0        0     1537 2023-04-07 10:44:07.420468 timerdo-0.0.3/README.md
--rw-r--r--   0        0        0     1211 2023-04-07 10:44:07.420468 timerdo-0.0.3/UNLICENSE
--rw-r--r--   0        0        0        0 2023-04-07 10:44:07.420468 timerdo-0.0.3/docs/how_to_guides.md
--rw-r--r--   0        0        0    37426 2023-04-07 10:44:07.424468 timerdo-0.0.3/docs/img/favicon.png
--rw-r--r--   0        0        0    76201 2023-04-07 10:44:07.424468 timerdo-0.0.3/docs/img/logo.png
--rw-r--r--   0        0        0     3681 2023-04-07 10:44:07.424468 timerdo-0.0.3/docs/index.md
--rw-r--r--   0        0        0       48 2023-04-07 10:44:07.424468 timerdo-0.0.3/docs/stylesheets/extra.css
--rw-r--r--   0        0        0        0 2023-04-07 10:44:07.424468 timerdo-0.0.3/docs/tutorials.md
--rw-r--r--   0        0        0     7991 2023-04-07 10:44:07.424468 timerdo-0.0.3/images/add_1.png
--rw-r--r--   0        0        0    31536 2023-04-07 10:44:07.424468 timerdo-0.0.3/images/add_help.png
--rw-r--r--   0        0        0    75032 2023-04-07 10:44:07.424468 timerdo-0.0.3/images/edit_help.png
--rw-r--r--   0        0        0    44084 2023-04-07 10:44:07.424468 timerdo-0.0.3/images/help.png
--rw-r--r--   0        0        0     3278 2023-04-07 10:44:07.424468 timerdo-0.0.3/images/pip_install.png
--rw-r--r--   0        0        0    20946 2023-04-07 10:44:07.424468 timerdo-0.0.3/images/projects.png
--rw-r--r--   0        0        0    28272 2023-04-07 10:44:07.424468 timerdo-0.0.3/images/projects_help.png
--rw-r--r--   0        0        0    28113 2023-04-07 10:44:07.424468 timerdo-0.0.3/images/report.png
--rw-r--r--   0        0        0     7335 2023-04-07 10:44:07.424468 timerdo-0.0.3/images/select_project.png
--rw-r--r--   0        0        0     5791 2023-04-07 10:44:07.424468 timerdo-0.0.3/images/start_1.png
--rw-r--r--   0        0        0    23340 2023-04-07 10:44:07.424468 timerdo-0.0.3/images/start_help.png
--rw-r--r--   0        0        0     5714 2023-04-07 10:44:07.424468 timerdo-0.0.3/images/stop_1.png
--rw-r--r--   0        0        0    15677 2023-04-07 10:44:07.424468 timerdo-0.0.3/images/stop_help.png
--rw-r--r--   0        0        0    22017 2023-04-07 10:44:07.428468 timerdo-0.0.3/images/task.png
--rw-r--r--   0        0        0    18478 2023-04-07 10:44:07.428468 timerdo-0.0.3/images/task_help.png
--rw-r--r--   0        0        0    22267 2023-04-07 10:44:07.428468 timerdo-0.0.3/images/timerdo.png
--rw-r--r--   0        0        0    25066 2023-04-07 10:44:07.428468 timerdo-0.0.3/images/view.png
--rw-r--r--   0        0        0    19519 2023-04-07 10:44:07.428468 timerdo-0.0.3/images/view_help.png
--rw-r--r--   0        0        0       61 2023-04-07 10:44:07.428468 timerdo-0.0.3/includes/abbreviations.md
--rw-r--r--   0        0        0     2218 2023-04-07 10:44:07.428468 timerdo-0.0.3/mkdocs.yml
--rw-r--r--   0        0        0     1161 2023-04-07 10:44:07.428468 timerdo-0.0.3/pyproject.toml
--rwxr-xr-x   0        0        0      210 2023-04-07 10:44:07.428468 timerdo-0.0.3/scripts/bootstrap.sh
--rwxr-xr-x   0        0        0      154 2023-04-07 10:44:07.428468 timerdo-0.0.3/scripts/docs_preview.sh
--rwxr-xr-x   0        0        0      101 2023-04-07 10:44:07.428468 timerdo-0.0.3/scripts/docs_publish.sh
--rwxr-xr-x   0        0        0      240 2023-04-07 10:44:07.428468 timerdo-0.0.3/scripts/format.sh
--rwxr-xr-x   0        0        0      110 2023-04-07 10:44:07.428468 timerdo-0.0.3/scripts/publish.sh
--rwxr-xr-x   0        0        0      246 2023-04-07 10:44:07.428468 timerdo-0.0.3/scripts/tests.sh
--rw-r--r--   0        0        0        0 2023-04-07 10:44:07.428468 timerdo-0.0.3/test/__init__.py
--rw-r--r--   0        0        0     1128 2023-04-07 10:44:07.428468 timerdo-0.0.3/test/conftest.py
--rw-r--r--   0        0        0     6115 2023-04-07 10:44:07.428468 timerdo-0.0.3/test/test_core.py
--rw-r--r--   0        0        0     1486 2023-04-07 10:44:07.428468 timerdo-0.0.3/test/test_main.py
--rw-r--r--   0        0        0      100 2023-04-07 10:44:07.428468 timerdo-0.0.3/timerdo/__init__.py
--rw-r--r--   0        0        0      926 2023-04-07 10:44:07.428468 timerdo-0.0.3/timerdo/config.py
--rw-r--r--   0        0        0     6128 2023-04-07 10:44:07.428468 timerdo-0.0.3/timerdo/core.py
--rw-r--r--   0        0        0     1075 2023-04-07 10:44:07.428468 timerdo-0.0.3/timerdo/database.py
--rw-r--r--   0        0        0      630 2023-04-07 10:44:07.428468 timerdo-0.0.3/timerdo/exceptions.py
--rw-r--r--   0        0        0     3902 2023-04-07 10:44:07.428468 timerdo-0.0.3/timerdo/main.py
--rw-r--r--   0        0        0     1681 2023-04-07 10:44:07.428468 timerdo-0.0.3/timerdo/models.py
--rw-r--r--   0        0        0     2695 1970-01-01 00:00:00.000000 timerdo-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0       30 2023-05-04 19:59:13.280237 timerdo-0.0.4/.coveragerc
+-rw-r--r--   0        0        0       99 2023-05-04 19:59:13.280237 timerdo-0.0.4/.flake8
+-rw-r--r--   0        0        0      569 2023-05-04 19:59:13.280237 timerdo-0.0.4/.github/workflows/publish_docs.yml
+-rw-r--r--   0        0        0      506 2023-05-04 19:59:13.280237 timerdo-0.0.4/.github/workflows/publish_pypi.yml
+-rw-r--r--   0        0        0      566 2023-05-04 19:59:13.280237 timerdo-0.0.4/.github/workflows/test_suite.yml
+-rw-r--r--   0        0        0      101 2023-05-04 19:59:13.280237 timerdo-0.0.4/.gitignore
+-rw-r--r--   0        0        0      292 2023-05-04 19:59:13.284237 timerdo-0.0.4/Makefile
+-rw-r--r--   0        0        0     1793 2023-05-04 19:59:13.284237 timerdo-0.0.4/README.md
+-rw-r--r--   0        0        0     1211 2023-05-04 19:59:13.284237 timerdo-0.0.4/UNLICENSE
+-rw-r--r--   0        0        0     3400 2023-05-04 19:59:13.284237 timerdo-0.0.4/docs/cli_reference.md
+-rw-r--r--   0        0        0    37426 2023-05-04 19:59:13.284237 timerdo-0.0.4/docs/img/favicon.png
+-rw-r--r--   0        0        0    76201 2023-05-04 19:59:13.284237 timerdo-0.0.4/docs/img/logo.png
+-rw-r--r--   0        0        0    75292 2023-05-04 19:59:13.284237 timerdo-0.0.4/docs/img/screenshot_timerdo_report.png
+-rw-r--r--   0        0        0    13786 2023-05-04 19:59:13.284237 timerdo-0.0.4/docs/img/timerdo_no_args.png
+-rw-r--r--   0        0        0     1891 2023-05-04 19:59:13.284237 timerdo-0.0.4/docs/index.md
+-rw-r--r--   0        0        0     2502 2023-05-04 19:59:13.284237 timerdo-0.0.4/docs/install.md
+-rw-r--r--   0        0        0     4267 2023-05-04 19:59:13.284237 timerdo-0.0.4/docs/start.md
+-rw-r--r--   0        0        0       48 2023-05-04 19:59:13.284237 timerdo-0.0.4/docs/stylesheets/extra.css
+-rw-r--r--   0        0        0    19982 2023-05-04 19:59:13.284237 timerdo-0.0.4/docs/tutorial_1.md
+-rw-r--r--   0        0        0      376 2023-05-04 19:59:13.284237 timerdo-0.0.4/docs/tutorial_2.md
+-rw-r--r--   0        0        0      138 2023-05-04 19:59:13.284237 timerdo-0.0.4/includes/abbreviations.md
+-rw-r--r--   0        0        0     2240 2023-05-04 19:59:13.284237 timerdo-0.0.4/mkdocs.yml
+-rw-r--r--   0        0        0     1242 2023-05-04 19:59:13.284237 timerdo-0.0.4/pyproject.toml
+-rwxr-xr-x   0        0        0      210 2023-05-04 19:59:13.284237 timerdo-0.0.4/scripts/bootstrap.sh
+-rw-r--r--   0        0        0      157 2023-05-04 19:59:13.284237 timerdo-0.0.4/scripts/build_cli_ref.sh
+-rw-r--r--   0        0        0      816 2023-05-04 19:59:13.284237 timerdo-0.0.4/scripts/docs_db.py
+-rwxr-xr-x   0        0        0      241 2023-05-04 19:59:13.284237 timerdo-0.0.4/scripts/docs_preview.sh
+-rwxr-xr-x   0        0        0      101 2023-05-04 19:59:13.284237 timerdo-0.0.4/scripts/docs_publish.sh
+-rwxr-xr-x   0        0        0      354 2023-05-04 19:59:13.284237 timerdo-0.0.4/scripts/format.sh
+-rw-r--r--   0        0        0      207 2023-05-04 19:59:13.284237 timerdo-0.0.4/scripts/gen_docs_db.sh
+-rwxr-xr-x   0        0        0      110 2023-05-04 19:59:13.284237 timerdo-0.0.4/scripts/publish.sh
+-rwxr-xr-x   0        0        0      277 2023-05-04 19:59:13.284237 timerdo-0.0.4/scripts/tests.sh
+-rw-r--r--   0        0        0        0 2023-05-04 19:59:13.284237 timerdo-0.0.4/test/__init__.py
+-rw-r--r--   0        0        0     1128 2023-05-04 19:59:13.284237 timerdo-0.0.4/test/conftest.py
+-rw-r--r--   0        0        0     6658 2023-05-04 19:59:13.284237 timerdo-0.0.4/test/test_core.py
+-rw-r--r--   0        0        0     2559 2023-05-04 19:59:13.284237 timerdo-0.0.4/test/test_main.py
+-rw-r--r--   0        0        0      100 2023-05-04 19:59:13.284237 timerdo-0.0.4/timerdo/__init__.py
+-rw-r--r--   0        0        0      955 2023-05-04 19:59:13.284237 timerdo-0.0.4/timerdo/config.py
+-rw-r--r--   0        0        0    11739 2023-05-04 19:59:13.288237 timerdo-0.0.4/timerdo/core.py
+-rw-r--r--   0        0        0     1075 2023-05-04 19:59:13.288237 timerdo-0.0.4/timerdo/database.py
+-rw-r--r--   0        0        0      630 2023-05-04 19:59:13.288237 timerdo-0.0.4/timerdo/exceptions.py
+-rw-r--r--   0        0        0     5417 2023-05-04 19:59:13.288237 timerdo-0.0.4/timerdo/main.py
+-rw-r--r--   0        0        0     1681 2023-05-04 19:59:13.288237 timerdo-0.0.4/timerdo/models.py
+-rw-r--r--   0        0        0     3066 1970-01-01 00:00:00.000000 timerdo-0.0.4/PKG-INFO
```

### Comparing `timerdo-0.0.3/.github/workflows/publish_docs.yml` & `timerdo-0.0.4/.github/workflows/publish_docs.yml`

 * *Files identical despite different names*

### Comparing `timerdo-0.0.3/.github/workflows/test_suite.yml` & `timerdo-0.0.4/.github/workflows/test_suite.yml`

 * *Files identical despite different names*

### Comparing `timerdo-0.0.3/README.md` & `timerdo-0.0.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,17 @@
 <p align="center">
 <a href="https://github.com/caiomts/timerdo/actions?query=workflow%3ATests" targe>
     <img src="https://github.com/caiomts/timerdo/actions/workflows/test_suite.yml/badge.svg" alt="Test">
     </a> 
     <a href="https://github.com/caiomts/timerdo/actions?query=workflow%3ADocs" targe>
     <img src="https://github.com/caiomts/timerdo/actions/workflows/publish_docs.yml/badge.svg" alt="Docs">
 </a>
+<a href="https://github.com/caiomts/timerdo/actions?query=workflow%3APublish" targe>
+    <img src="https://github.com/caiomts/timerdo/actions/workflows/publish_pypi.yml/badge.svg" alt="Docs">
+</a>
 <a href="https://pypi.org/project/timerdo/">
     <img src="https://badge.fury.io/py/timerdo.svg" alt="Package version">
 </a>
 </p>
 
 A minimalist to-do list with built-in timer to keep your tasks on track. 
 
@@ -32,14 +35,16 @@
 
 **Documentation:** http://caiomts.github.io/timerdo
 
 :warning: Early stage project[^2]
 
 ---
 
+![timerdo_report](docs/img/screenshot_timerdo_report.png)
+
 ## Getting started
 
 http://caiomts.github.io/timerdo/#getting-started
 
 ## CLI Reference
 
 http://caiomts.github.io/timerdo/#CLI-Reference
```

#### html2text {}

```diff
@@ -1,13 +1,14 @@
                                    [timerdo]
-                        [Test] [Docs] [Package_version]
+                    [Test] [Docs] [Docs] [Package_version]
 A minimalist to-do list with built-in timer to keep your tasks on track.
 Timerdo is an intuitive CLI application that will help you focus on what really
 matters. --- ## Requirements Python 3.11+ No fear of the command-line interface
 :laughing:. --- **Source Code:** https://github.com/caiomts/timerdo
 **Documentation:** http://caiomts.github.io/timerdo :warning: Early stage
-project[^2] --- ## Getting started http://caiomts.github.io/timerdo/#getting-
-started ## CLI Reference http://caiomts.github.io/timerdo/#CLI-Reference ## API
-Reference http://caiomts.github.io/timerdo/#API-Reference ## Releases http://
+project[^2] --- ![timerdo_report](docs/img/screenshot_timerdo_report.png) ##
+Getting started http://caiomts.github.io/timerdo/#getting-started ## CLI
+Reference http://caiomts.github.io/timerdo/#CLI-Reference ## API Reference
+http://caiomts.github.io/timerdo/#API-Reference ## Releases http://
 caiomts.github.io/timerdo/#Releases [^2]: Data models are mostly stable, but
 visualization and queries are in full development and the API can change
 quickly.
```

### Comparing `timerdo-0.0.3/UNLICENSE` & `timerdo-0.0.4/UNLICENSE`

 * *Files identical despite different names*

### Comparing `timerdo-0.0.3/docs/img/favicon.png` & `timerdo-0.0.4/docs/img/favicon.png`

 * *Files identical despite different names*

### Comparing `timerdo-0.0.3/docs/img/logo.png` & `timerdo-0.0.4/docs/img/logo.png`

 * *Files identical despite different names*

### Comparing `timerdo-0.0.3/mkdocs.yml` & `timerdo-0.0.4/mkdocs.yml`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,28 @@
 site_name: Timerdo
 repo_url: https://github.com/caiomts/timerdo
 repo_name: caiomts/timerdo
 edit_uri: edit/master/docs/
 
+nav:
+  - "Home": 
+      - index.md
+      - install.md
+  - "Getting Started":
+    - start.md
+  - "Tutorial - User Guide":
+    - tutorial_1.md
+    - tutorial_2.md
+  - "CLI Reference":
+      - cli_reference.md
+
+
 theme:
+  features:
+    - content.tabs.link
   name: material
   logo: img/favicon.png
   favicon: img/favicon.png
   palette:
     - scheme: default
       primary: deep orange
       accent: deep purple
@@ -29,14 +44,15 @@
     - navigation.top
     - search.suggest
     - search.share
     - header.autohide
     - navigation.footer
     - content.action.edit
     - content.action.view
+    - navigation.indexes
 
 markdown_extensions:
   - attr_list
   - md_in_html
   - abbr
   - admonition
   - footnotes
@@ -52,33 +68,31 @@
   - pymdownx.highlight:
       anchor_linenums: true
       line_spans: __span
       pygments_lang_class: true
       use_pygments: true
   - pymdownx.tasklist:
       custom_checkbox: true
+  - pymdownx.tabbed:
+      alternate_style: true
   - pymdownx.inlinehilite
   - pymdownx.snippets
   - pymdownx.superfences
   - pymdownx.critic
   - pymdownx.caret
   - pymdownx.keys
   - pymdownx.mark
   - pymdownx.tilde
   - pymdownx.betterem
   - pymdownx.details
   - pymdownx.superfences
 
-
 plugins:
   - search
   - tags
-  - git-revision-date-localized:
-      enable_creation_date: true
-      fallback_to_build_date: true
 
 extra:
   social:
     - icon: fontawesome/brands/github
       link: https://github.com/caiomts
       name: github.com/caiomts
 
@@ -86,18 +100,9 @@
       link: https://www.linkedin.com/in/caiomts/
       name: in/caiomts/
 
     - icon: material/web
       link: https://caiomts.github.io/
       name: caiomts.github.io
 
-nav:
-  - Home: index.md
-  - Tutorials: tutorials.md
-  - How-to guides: how_to_guides.md
-  - Reference CLI: ref_cli.md
-  - Reference API: ref_api.md
-  - Releases: releases.md
-  - About: about.md
-
 extra_css:
   - stylesheets/extra.css
```

### Comparing `timerdo-0.0.3/pyproject.toml` & `timerdo-0.0.4/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -6,16 +6,17 @@
 name = "timerdo"
 authors = [{name = "Caio Mescouto Terra de Souza", email = "caiomescouto@gmail.com"}]
 readme = "README.md"
 requires-python = ">=3.11"
 dynamic = ["version", "description"]
 dependencies = [
     "sqlalchemy >=2.0.4, <2.1",
-    "typer >=0.7.0, <0.8",
+    "typer >=0.7.0, <0.9",
     "rich >=13.3, <13.4",
+    "pandas[performance,feather] >=2.0.1, <2.1",
 ]
 
 [project.urls]
 Documentation = "http://caiomts.github.io/timerdo"
 Source = "https://github.com/caiomts/timerdo"
 
 [project.scripts]
@@ -28,14 +29,15 @@
     "Faker >=17.6.0, <17.7", 
 ]
 
 docs = [
 	"mkdocs-material >=9.1.3, <9.2",
 	"mkdocstrings[python] >=0.20, <0.21",
     "mkdocs-git-revision-date-localized-plugin >=1.2.0, <1.3",
+    "typer-cli >=0.0.13, <0.1",
 ]
 
 dev = [
 	"black >=23.1, <23.2",
 	"flake8 >=6.0, <6.1",
 	"isort >=5.12, <5.13",
     "pydocstyle[toml] >=6.3.0, <6.4",
```

### Comparing `timerdo-0.0.3/test/conftest.py` & `timerdo-0.0.4/test/conftest.py`

 * *Files identical despite different names*

### Comparing `timerdo-0.0.3/test/test_core.py` & `timerdo-0.0.4/test/test_core.py`

 * *Files 14% similar despite different names*

```diff
@@ -41,16 +41,17 @@
     assert (
         tconnection.execute(text('SELECT * FROM todo_list')).one().status
         == Status.to_do
     )
 
 
 def test_add_task_without_task(tconnection):
-    with pytest.raises(TypeError):
+    with pytest.raises(SystemExit) as e:
         add_task(session=tconnection)
+        assert e.value.code == 1
 
 
 def test_add_task(tconnection, fake_todo_item):
     task = fake_todo_item.task
     tag = fake_todo_item.tag
     deadline = fake_todo_item.deadline
     add_task(task=task, tag=tag, deadline=deadline, session=tconnection)
@@ -58,61 +59,67 @@
     assert item.task == capwords(task)
     assert item.tag == capwords(tag)
     assert item.deadline == deadline
     assert item.status == Status.to_do
 
 
 def test_add_timer_attribute_error(tconnection):
-    with pytest.raises(IdNotFoundError):
+    with pytest.raises(SystemExit) as e:
         add_timer(1, session=tconnection)
+        assert e.value.code == 1
 
 
 def test_add_timer(tconnection, add_task):
     add_timer(1, session=tconnection)
     assert tconnection.get_id(Timer, 1).id == 1
 
 
 def test_add_timer_done_task(tconnection, done_task):
-    with pytest.raises(DoneTaskError):
+    with pytest.raises(SystemExit) as e:
         add_timer(1, session=tconnection)
+        assert e.value.code == 1
 
 
 def test_add_timer_running_timer(tconnection, running_timer):
-    with pytest.raises(RunningTimerError):
+    with pytest.raises(SystemExit) as e:
         add_timer(1, session=tconnection)
+        assert e.value.code == 1
 
 
 def test_finish_timer(tconnection, running_timer):
-    finish_timer(session=tconnection)
+    finish_timer(done=False, session=tconnection)
     assert (
         tconnection.execute(
             text('SELECT * FROM timer_list WHERE finished_at = NULL')
         ).all()
         == []
     )
 
 
 def test_finish_timer_no_running(tconnection):
-    with pytest.raises(NoTimeRunningError):
-        finish_timer(session=tconnection)
+    with pytest.raises(SystemExit) as e:
+        finish_timer(done=True, session=tconnection)
+        assert e.value.code == 1
 
 
 def test_delete_item(tconnection, add_task):
     delete_item(1, ToDoItem, tconnection)
     assert tconnection.get_id(ToDoItem, 1) is None
 
 
 def test_delete_item_wrong_id(tconnection):
-    with pytest.raises(IdNotFoundError):
+    with pytest.raises(SystemExit) as e:
         delete_item(1, ToDoItem, tconnection)
+        assert e.value.code == 1
 
 
 def test_edit_todo_item_wrong_id(tconnection):
-    with pytest.raises(IdNotFoundError):
+    with pytest.raises(SystemExit) as e:
         edit_todo_item(1, session=tconnection)
+        assert e.value.code == 1
 
 
 def test_edit_todo_item(tconnection, add_task):
     fake = Faker()
     task = fake.sentence()
     tag = fake.word()
     deadline = fake.date_between()
@@ -130,88 +137,95 @@
     assert item.task == capwords(task)
     assert item.tag == capwords(tag)
     assert item.deadline == deadline
     assert item.status == Status.done
 
 
 def test_edit_timer(tconnection, running_timer):
-    finish_timer(session=tconnection)
+    finish_timer(done=False, session=tconnection)
 
     now = datetime.now()
     finished_at = now
     created_at = now - timedelta(hours=1)
 
     edit_timer_item(
         1, created_at=created_at, finished_at=finished_at, session=tconnection
     )
 
     timer = tconnection.get_id(Timer, 1)
     assert timer.finished_at - timer.created_at == timedelta(hours=1)
 
 
 def test_edit_timer_running_timer(tconnection, running_timer):
-    with pytest.raises(RunningTimerError):
+    with pytest.raises(SystemExit) as e:
         edit_timer_item(1, session=tconnection)
+        assert e.value.code == 1
 
 
 def test_edit_timer_no_change_timer(tconnection, running_timer):
-    finish_timer(session=tconnection)
-    with pytest.raises(NoChangingError):
+    finish_timer(done=False, session=tconnection)
+    with pytest.raises(SystemExit) as e:
         edit_timer_item(1, session=tconnection)
+        assert e.value.code == 1
 
 
 def test_edit_timer_no_created_at(tconnection, running_timer):
-    finish_timer(session=tconnection)
+    finish_timer(done=False, session=tconnection)
 
     diff = datetime.utcnow() - datetime.now()
     finished_at = datetime.now()
     finished_at_utc = finished_at + diff
 
     edit_timer_item(1, finished_at=finished_at, session=tconnection)
 
     timer = tconnection.get_id(Timer, 1)
     assert timer.finished_at.second == finished_at_utc.second
     assert timer.finished_at.minute == finished_at_utc.minute
     assert timer.finished_at.hour == finished_at_utc.hour
 
 
 def test_edit_timer_no_finished_at(tconnection, running_timer):
-    finish_timer(session=tconnection)
+    finish_timer(done=False, session=tconnection)
 
     diff = datetime.utcnow() - datetime.now()
     created_at = datetime.now() - timedelta(hours=1)
     created_at_utc = created_at + diff
 
     edit_timer_item(1, created_at=created_at, session=tconnection)
 
     timer = tconnection.get_id(Timer, 1)
     assert timer.created_at.second == created_at_utc.second
     assert timer.created_at.minute == created_at_utc.minute
     assert timer.created_at.hour == created_at_utc.hour
 
 
 def test_edit_timer_created_gt_finished(tconnection, running_timer):
-    with pytest.raises(NegativeIntervalError):
-        finish_timer(session=tconnection)
+    with pytest.raises(SystemExit) as e:
+        finish_timer(done=False, session=tconnection)
 
         created_at = datetime.now() + timedelta(hours=1)
 
         edit_timer_item(1, created_at=created_at, session=tconnection)
+        assert e.value.code == 1
 
 
 def test_edit_timer_no_finished_gt_now(tconnection, running_timer):
-    with pytest.raises(OutOffPeriodError):
-        finish_timer(session=tconnection)
+    with pytest.raises(SystemExit) as e:
+        finish_timer(done=False, session=tconnection)
 
         finished_at = datetime.now() + timedelta(hours=1)
 
         edit_timer_item(1, finished_at=finished_at, session=tconnection)
+        assert e.value.code == 1
 
 
 def test_edit_timer_wrong_id(tconnection):
-    with pytest.raises(IdNotFoundError):
+    with pytest.raises(SystemExit) as e:
         edit_timer_item(2, finished_at=datetime.now(), session=tconnection)
+        assert e.value.code == 1
 
 
 def test_select_all(tconnection, running_timer):
     item = tconnection.get_id(ToDoItem, 1)
-    assert query_with_text(session=tconnection)[0][1] == item.task
+    script = """SELECT * FROM todo_list"""
+    result = query_with_text(script, session=tconnection)
+    assert '{' in result
```

### Comparing `timerdo-0.0.3/timerdo/config.py` & `timerdo-0.0.4/timerdo/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -24,8 +24,8 @@
             return Path(os.environ['TIMERDOTEST']) / 'TimerdoTest'
 
 
 data_dir = get_user_dir() / 'Timerdo'
 config_dir = get_user_dir(dir_data=False)
 
 data_dir.mkdir(parents=True, exist_ok=True)
-config_dir.mkdir(parents=True, exist_ok=True)
+config_dir.mkdir(parents=True, exist_ok=True)  # On hold. Might be useful.
```

### Comparing `timerdo-0.0.3/timerdo/database.py` & `timerdo-0.0.4/timerdo/database.py`

 * *Files identical despite different names*

### Comparing `timerdo-0.0.3/timerdo/exceptions.py` & `timerdo-0.0.4/timerdo/exceptions.py`

 * *Files identical despite different names*

### Comparing `timerdo-0.0.3/timerdo/models.py` & `timerdo-0.0.4/timerdo/models.py`

 * *Files identical despite different names*

### Comparing `timerdo-0.0.3/PKG-INFO` & `timerdo-0.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: timerdo
-Version: 0.0.3
+Version: 0.0.4
 Summary: Minimalist to-do list with built-in timer to keep your tasks on track.
 Author-email: Caio Mescouto Terra de Souza <caiomescouto@gmail.com>
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 Requires-Dist: sqlalchemy >=2.0.4, <2.1
-Requires-Dist: typer >=0.7.0, <0.8
+Requires-Dist: typer >=0.7.0, <0.9
 Requires-Dist: rich >=13.3, <13.4
+Requires-Dist: pandas[performance,feather] >=2.0.1, <2.1
 Requires-Dist: black >=23.1, <23.2 ; extra == "dev"
 Requires-Dist: flake8 >=6.0, <6.1 ; extra == "dev"
 Requires-Dist: isort >=5.12, <5.13 ; extra == "dev"
 Requires-Dist: pydocstyle[toml] >=6.3.0, <6.4 ; extra == "dev"
 Requires-Dist: mkdocs-material >=9.1.3, <9.2 ; extra == "docs"
 Requires-Dist: mkdocstrings[python] >=0.20, <0.21 ; extra == "docs"
 Requires-Dist: mkdocs-git-revision-date-localized-plugin >=1.2.0, <1.3 ; extra == "docs"
+Requires-Dist: typer-cli >=0.0.13, <0.1 ; extra == "docs"
 Requires-Dist: pytest >=7.2.1, <7.3 ; extra == "test"
 Requires-Dist: pytest-cov >=4.0.0, <4.1 ; extra == "test"
 Requires-Dist: Faker >=17.6.0, <17.7 ; extra == "test"
 Project-URL: Documentation, http://caiomts.github.io/timerdo
 Project-URL: Source, https://github.com/caiomts/timerdo
 Provides-Extra: dev
 Provides-Extra: docs
@@ -32,14 +34,17 @@
 <p align="center">
 <a href="https://github.com/caiomts/timerdo/actions?query=workflow%3ATests" targe>
     <img src="https://github.com/caiomts/timerdo/actions/workflows/test_suite.yml/badge.svg" alt="Test">
     </a> 
     <a href="https://github.com/caiomts/timerdo/actions?query=workflow%3ADocs" targe>
     <img src="https://github.com/caiomts/timerdo/actions/workflows/publish_docs.yml/badge.svg" alt="Docs">
 </a>
+<a href="https://github.com/caiomts/timerdo/actions?query=workflow%3APublish" targe>
+    <img src="https://github.com/caiomts/timerdo/actions/workflows/publish_pypi.yml/badge.svg" alt="Docs">
+</a>
 <a href="https://pypi.org/project/timerdo/">
     <img src="https://badge.fury.io/py/timerdo.svg" alt="Package version">
 </a>
 </p>
 
 A minimalist to-do list with built-in timer to keep your tasks on track. 
 
@@ -58,14 +63,16 @@
 
 **Documentation:** http://caiomts.github.io/timerdo
 
 :warning: Early stage project[^2]
 
 ---
 
+![timerdo_report](docs/img/screenshot_timerdo_report.png)
+
 ## Getting started
 
 http://caiomts.github.io/timerdo/#getting-started
 
 ## CLI Reference
 
 http://caiomts.github.io/timerdo/#CLI-Reference
```

#### html2text {}

```diff
@@ -1,29 +1,32 @@
-Metadata-Version: 2.1 Name: timerdo Version: 0.0.3 Summary: Minimalist to-do
+Metadata-Version: 2.1 Name: timerdo Version: 0.0.4 Summary: Minimalist to-do
 list with built-in timer to keep your tasks on track. Author-email: Caio
 Mescouto Terra de Souza
 gmail.com> Requires-Python: >=3.11 Description-Content-Type: text/markdown
-Requires-Dist: sqlalchemy >=2.0.4, <2.1 Requires-Dist: typer >=0.7.0, <0.8
-Requires-Dist: rich >=13.3, <13.4 Requires-Dist: black >=23.1, <23.2 ; extra ==
-"dev" Requires-Dist: flake8 >=6.0, <6.1 ; extra == "dev" Requires-Dist: isort
->=5.12, <5.13 ; extra == "dev" Requires-Dist: pydocstyle[toml] >=6.3.0, <6.4 ;
-extra == "dev" Requires-Dist: mkdocs-material >=9.1.3, <9.2 ; extra == "docs"
-Requires-Dist: mkdocstrings[python] >=0.20, <0.21 ; extra == "docs" Requires-
-Dist: mkdocs-git-revision-date-localized-plugin >=1.2.0, <1.3 ; extra == "docs"
-Requires-Dist: pytest >=7.2.1, <7.3 ; extra == "test" Requires-Dist: pytest-cov
->=4.0.0, <4.1 ; extra == "test" Requires-Dist: Faker >=17.6.0, <17.7 ; extra ==
-"test" Project-URL: Documentation, http://caiomts.github.io/timerdo Project-
-URL: Source, https://github.com/caiomts/timerdo Provides-Extra: dev Provides-
-Extra: docs Provides-Extra: test
+Requires-Dist: sqlalchemy >=2.0.4, <2.1 Requires-Dist: typer >=0.7.0, <0.9
+Requires-Dist: rich >=13.3, <13.4 Requires-Dist: pandas[performance,feather]
+>=2.0.1, <2.1 Requires-Dist: black >=23.1, <23.2 ; extra == "dev" Requires-
+Dist: flake8 >=6.0, <6.1 ; extra == "dev" Requires-Dist: isort >=5.12, <5.13 ;
+extra == "dev" Requires-Dist: pydocstyle[toml] >=6.3.0, <6.4 ; extra == "dev"
+Requires-Dist: mkdocs-material >=9.1.3, <9.2 ; extra == "docs" Requires-Dist:
+mkdocstrings[python] >=0.20, <0.21 ; extra == "docs" Requires-Dist: mkdocs-git-
+revision-date-localized-plugin >=1.2.0, <1.3 ; extra == "docs" Requires-Dist:
+typer-cli >=0.0.13, <0.1 ; extra == "docs" Requires-Dist: pytest >=7.2.1, <7.3
+; extra == "test" Requires-Dist: pytest-cov >=4.0.0, <4.1 ; extra == "test"
+Requires-Dist: Faker >=17.6.0, <17.7 ; extra == "test" Project-URL:
+Documentation, http://caiomts.github.io/timerdo Project-URL: Source, https://
+github.com/caiomts/timerdo Provides-Extra: dev Provides-Extra: docs Provides-
+Extra: test
                                    [timerdo]
-                        [Test] [Docs] [Package_version]
+                    [Test] [Docs] [Docs] [Package_version]
 A minimalist to-do list with built-in timer to keep your tasks on track.
 Timerdo is an intuitive CLI application that will help you focus on what really
 matters. --- ## Requirements Python 3.11+ No fear of the command-line interface
 :laughing:. --- **Source Code:** https://github.com/caiomts/timerdo
 **Documentation:** http://caiomts.github.io/timerdo :warning: Early stage
-project[^2] --- ## Getting started http://caiomts.github.io/timerdo/#getting-
-started ## CLI Reference http://caiomts.github.io/timerdo/#CLI-Reference ## API
-Reference http://caiomts.github.io/timerdo/#API-Reference ## Releases http://
+project[^2] --- ![timerdo_report](docs/img/screenshot_timerdo_report.png) ##
+Getting started http://caiomts.github.io/timerdo/#getting-started ## CLI
+Reference http://caiomts.github.io/timerdo/#CLI-Reference ## API Reference
+http://caiomts.github.io/timerdo/#API-Reference ## Releases http://
 caiomts.github.io/timerdo/#Releases [^2]: Data models are mostly stable, but
 visualization and queries are in full development and the API can change
 quickly.
```

