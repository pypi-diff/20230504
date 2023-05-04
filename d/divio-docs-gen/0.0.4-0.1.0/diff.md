# Comparing `tmp/divio_docs_gen-0.0.4.tar.gz` & `tmp/divio_docs_gen-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "divio_docs_gen-0.0.4.tar", last modified: Tue Apr 18 11:34:43 2023, max compression
+gzip compressed data, was "divio_docs_gen-0.1.0.tar", last modified: Thu May  4 13:13:11 2023, max compression
```

## Comparing `divio_docs_gen-0.0.4.tar` & `divio_docs_gen-0.1.0.tar`

### file list

```diff
@@ -1,23 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 11:34:43.593698 divio_docs_gen-0.0.4/
--rw-r--r--   0 root         (0) root         (0)     1067 2023-04-18 11:34:33.000000 divio_docs_gen-0.0.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)     5748 2023-04-18 11:34:43.593698 divio_docs_gen-0.0.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4954 2023-04-18 11:34:33.000000 divio_docs_gen-0.0.4/README.md
--rw-r--r--   0 root         (0) root         (0)      916 2023-04-18 11:34:33.000000 divio_docs_gen-0.0.4/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-18 11:34:43.593698 divio_docs_gen-0.0.4/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 11:34:43.593698 divio_docs_gen-0.0.4/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 11:34:43.593698 divio_docs_gen-0.0.4/src/divio_docs_gen/
--rw-r--r--   0 root         (0) root         (0)      135 2023-04-18 11:34:33.000000 divio_docs_gen-0.0.4/src/divio_docs_gen/__init__.py
--rw-r--r--   0 root         (0) root         (0)      131 2023-04-18 11:34:33.000000 divio_docs_gen-0.0.4/src/divio_docs_gen/__main__.py
--rw-r--r--   0 root         (0) root         (0)     6275 2023-04-18 11:34:33.000000 divio_docs_gen-0.0.4/src/divio_docs_gen/args.py
--rw-r--r--   0 root         (0) root         (0)      548 2023-04-18 11:34:33.000000 divio_docs_gen-0.0.4/src/divio_docs_gen/colourstring.py
--rw-r--r--   0 root         (0) root         (0)     5316 2023-04-18 11:34:33.000000 divio_docs_gen-0.0.4/src/divio_docs_gen/docsgen.py
--rw-r--r--   0 root         (0) root         (0)     7748 2023-04-18 11:34:33.000000 divio_docs_gen-0.0.4/src/divio_docs_gen/index.py
--rw-r--r--   0 root         (0) root         (0)     5531 2023-04-18 11:34:33.000000 divio_docs_gen-0.0.4/src/divio_docs_gen/repo.py
--rw-r--r--   0 root         (0) root         (0)     5411 2023-04-18 11:34:33.000000 divio_docs_gen-0.0.4/src/divio_docs_gen/sections.py
--rw-r--r--   0 root         (0) root         (0)      925 2023-04-18 11:34:33.000000 divio_docs_gen-0.0.4/src/divio_docs_gen/table.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 11:34:43.593698 divio_docs_gen-0.0.4/src/divio_docs_gen.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5748 2023-04-18 11:34:43.000000 divio_docs_gen-0.0.4/src/divio_docs_gen.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      513 2023-04-18 11:34:43.000000 divio_docs_gen-0.0.4/src/divio_docs_gen.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-18 11:34:43.000000 divio_docs_gen-0.0.4/src/divio_docs_gen.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       64 2023-04-18 11:34:43.000000 divio_docs_gen-0.0.4/src/divio_docs_gen.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       15 2023-04-18 11:34:43.000000 divio_docs_gen-0.0.4/src/divio_docs_gen.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 13:13:11.668909 divio_docs_gen-0.1.0/
+-rw-r--r--   0 root         (0) root         (0)     1067 2023-05-04 13:13:01.000000 divio_docs_gen-0.1.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     6045 2023-05-04 13:13:11.664909 divio_docs_gen-0.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5251 2023-05-04 13:13:01.000000 divio_docs_gen-0.1.0/README.md
+-rw-r--r--   0 root         (0) root         (0)      907 2023-05-04 13:13:01.000000 divio_docs_gen-0.1.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-04 13:13:11.668909 divio_docs_gen-0.1.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 13:13:11.664909 divio_docs_gen-0.1.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 13:13:11.664909 divio_docs_gen-0.1.0/src/divio_docs_gen/
+-rw-r--r--   0 root         (0) root         (0)     7564 2023-05-04 13:13:01.000000 divio_docs_gen-0.1.0/src/divio_docs_gen/Args.py
+-rw-r--r--   0 root         (0) root         (0)     3892 2023-05-04 13:13:01.000000 divio_docs_gen-0.1.0/src/divio_docs_gen/DivioDocsEntry.py
+-rw-r--r--   0 root         (0) root         (0)     2951 2023-05-04 13:13:01.000000 divio_docs_gen-0.1.0/src/divio_docs_gen/Repo.py
+-rw-r--r--   0 root         (0) root         (0)     5417 2023-05-04 13:13:01.000000 divio_docs_gen-0.1.0/src/divio_docs_gen/Section.py
+-rw-r--r--   0 root         (0) root         (0)      191 2023-05-04 13:13:01.000000 divio_docs_gen-0.1.0/src/divio_docs_gen/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      113 2023-05-04 13:13:01.000000 divio_docs_gen-0.1.0/src/divio_docs_gen/__main__.py
+-rw-r--r--   0 root         (0) root         (0)     1273 2023-05-04 13:13:01.000000 divio_docs_gen-0.1.0/src/divio_docs_gen/index.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 13:13:11.664909 divio_docs_gen-0.1.0/src/divio_docs_gen/write_to_disk/
+-rw-r--r--   0 root         (0) root         (0)     1732 2023-05-04 13:13:01.000000 divio_docs_gen-0.1.0/src/divio_docs_gen/write_to_disk/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3312 2023-05-04 13:13:01.000000 divio_docs_gen-0.1.0/src/divio_docs_gen/write_to_disk/nav.py
+-rw-r--r--   0 root         (0) root         (0)      611 2023-05-04 13:13:01.000000 divio_docs_gen-0.1.0/src/divio_docs_gen/write_to_disk/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 13:13:11.664909 divio_docs_gen-0.1.0/src/divio_docs_gen.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6045 2023-05-04 13:13:11.000000 divio_docs_gen-0.1.0/src/divio_docs_gen.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      583 2023-05-04 13:13:11.000000 divio_docs_gen-0.1.0/src/divio_docs_gen.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-04 13:13:11.000000 divio_docs_gen-0.1.0/src/divio_docs_gen.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       55 2023-05-04 13:13:11.000000 divio_docs_gen-0.1.0/src/divio_docs_gen.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-05-04 13:13:11.000000 divio_docs_gen-0.1.0/src/divio_docs_gen.egg-info/top_level.txt
```

### Comparing `divio_docs_gen-0.0.4/LICENSE` & `divio_docs_gen-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `divio_docs_gen-0.0.4/PKG-INFO` & `divio_docs_gen-0.1.0/src/divio_docs_gen.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: divio_docs_gen
-Version: 0.0.4
+Name: divio-docs-gen
+Version: 0.1.0
 Summary: Turn all the markdown files in your repos into one big, divio structrured documentation
 Author-email: Denperidge <denperidge@gmail.com>
 Project-URL: Homepage, https://github.com/Denperidge-Redpencil/divio-docs-gen
 Project-URL: Bug Tracker, https://github.com/Denperidge-Redpencil/divio-docs-gen/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Information Technology
@@ -18,19 +18,21 @@
 
 # Divio Docs Generator
 
 Automatically collect, aggregate and structure all your [divio-style documentation](https://documentation.divio.com/) into a tree of .md files.
 ```
 /{reponame}
     /tutorials
-    /how-tos
+    /howtos
     /explanations
     /references
 ```
 
+On a basic level, this repo will only need a list of git url's!
+
 - Any input structure: this script will scan your entire repository for .md files
     - If you have a how-to section in your README, that'll get extracted and put in the right spot
     - Or, if you have an how-to.md file, it'll get added in its entirety!
 - Any output structure: this script generates a simple markdown tree. Nothing proprietary, no vendor-lockin. It can be generated from GitHub Actions and put into a Jekyll pages site just as easily as it is run from a Raspberry Pi and used to render the contents of an Ember application.
 
 All you have to do is simply name your headers and/or files after the divio sections (`tutorial`, `how-to`, `explanation`, `reference`). (Oh, don't worry, the search is done through a case insensitive regex. Add more words as you please) 
 
@@ -66,48 +68,58 @@
 
 ## Discussions
 The Divio structure is built upon splitting your documentation into 4 types of documentations. ![The overview of the divio documentation on their website](https://documentation.divio.com/_images/overview.png). In this repository they're referred to as sections.
 
 
 If you want to know more about the design principles of this project, feel free to check out my writeup [here](https://github.com/Denperidge-Redpencil/Learning.md/blob/main/Notes/docs.md#design-principles)!
 
+Further expansion could be done to this project. For example, a structure like the following...
+```
+/{reponame}
+    /0.0.1
+        /tutorials
+        /how-tos
+        /explanations
+        /references
+```
+... should not be impossible to achieve with some tweaking!
+
 
 ## Reference
 
 ### docs.conf
 #### [DEFAULT] section
 This section is on the top of the file, and defines options that affect the entire configuration
 | Parameter     | Functionality                    |
 | ------------- | -------------------------------- |
-| DefaultOwner | (string) Defines which user or org has to be checked for the repository in case its Path does not explicitly define an owner |
+| DefaultOwner  | (string) Defines which user or org has to be checked for the repository in case its Path does not explicitly define an owner |
 | GenerateNav   | (boolean) Whether to add internal navigation to the top of each generated file. Defaults to `False` |
 | DocsBasedir   | What folder to output the docs in. Defaults to `docs/` |
 | Tutorials     | Sets the output folder name for tutorials. Defaults to `tutorials`    |
-| How-tos       | Sets the output folder name for how-tos. Defaults to `how-tos`    |
+| Howtos        | Sets the output folder name for how-tos. Defaults to `how-tos`    |
 | explanations  | Sets the output folder name for explanations. Defaults to `explanations`    |
 | references    | Sets the output folder name for references. Defaults to `references`    |
 
 
 #### [repo] section
 You can add as many of these as you want. Each one represents a repo you want parsed. You can give any name to `[the-section-header]`, but you should probably avoid duplicates. If no repo sections are defined but you've defined DefaultOwner, all repos of that user or organisation will be parsed.
 
 | Parameter | Functionality                              |
 | --------- | ------------------------------------------ |
 | Path      | (string) Defines which repository to parse |
-| Copy      | (array) Files in the repository that should be copied to a specific section. Syntax: `file.md/sectionname,file2.md/sectionname` |
-| Ignore      | (array) Files in the repository that should be ignored. Syntax: `file.md,file2.md` |
+| Move      | (string) Files in the repository that should be copied to a specific section. Syntax: `docs/file.md/section_id//file2.md/section_id/output_filename` |
+| Ignore      | (string) Files in the repository that should be ignored. Syntax: `file.md//file2.md` |
+
+
+**Example Ignore:** `Ignore=building-a-template.md//why-semantic-microservices.md`
+**Example Move:** `Move=documentation.md/references`
+
 
-*Note: for `Copy` and `Ignore` you can choose to be more specific by writing `sub/folder/filename.md`. The check is a `provided_path in full_filepath`, so `sub/folder/filename.md` will apply to `even/further/sub/folder/filename.md`.*
+*Note: for `Move` and `Ignore` you can choose to be more specific by writing `sub/folder/filename.md`. The check is a `provided_path in full_filepath`, so `sub/folder/filename.md` will apply to `even/further/sub/folder/filename.md`.*
 
-##### Allowed Path syntax
-You can use any of the following!
-- `reponame` (if DefaultOwner is defined)
-- `reponame@branch` (if DefaultOwner is defined)
-- `owner/reponame`
-- `owner/reponame@branch`
 
 
 
 ### Synonyms
 For ease of use and freedom of implementation, every section has synonyms.
 
 | Section       | Synonyms                        |
```

### Comparing `divio_docs_gen-0.0.4/README.md` & `divio_docs_gen-0.1.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 # Divio Docs Generator
 
 Automatically collect, aggregate and structure all your [divio-style documentation](https://documentation.divio.com/) into a tree of .md files.
 ```
 /{reponame}
     /tutorials
-    /how-tos
+    /howtos
     /explanations
     /references
 ```
 
+On a basic level, this repo will only need a list of git url's!
+
 - Any input structure: this script will scan your entire repository for .md files
     - If you have a how-to section in your README, that'll get extracted and put in the right spot
     - Or, if you have an how-to.md file, it'll get added in its entirety!
 - Any output structure: this script generates a simple markdown tree. Nothing proprietary, no vendor-lockin. It can be generated from GitHub Actions and put into a Jekyll pages site just as easily as it is run from a Raspberry Pi and used to render the contents of an Ember application.
 
 All you have to do is simply name your headers and/or files after the divio sections (`tutorial`, `how-to`, `explanation`, `reference`). (Oh, don't worry, the search is done through a case insensitive regex. Add more words as you please) 
 
@@ -48,48 +50,58 @@
 
 ## Discussions
 The Divio structure is built upon splitting your documentation into 4 types of documentations. ![The overview of the divio documentation on their website](https://documentation.divio.com/_images/overview.png). In this repository they're referred to as sections.
 
 
 If you want to know more about the design principles of this project, feel free to check out my writeup [here](https://github.com/Denperidge-Redpencil/Learning.md/blob/main/Notes/docs.md#design-principles)!
 
+Further expansion could be done to this project. For example, a structure like the following...
+```
+/{reponame}
+    /0.0.1
+        /tutorials
+        /how-tos
+        /explanations
+        /references
+```
+... should not be impossible to achieve with some tweaking!
+
 
 ## Reference
 
 ### docs.conf
 #### [DEFAULT] section
 This section is on the top of the file, and defines options that affect the entire configuration
 | Parameter     | Functionality                    |
 | ------------- | -------------------------------- |
-| DefaultOwner | (string) Defines which user or org has to be checked for the repository in case its Path does not explicitly define an owner |
+| DefaultOwner  | (string) Defines which user or org has to be checked for the repository in case its Path does not explicitly define an owner |
 | GenerateNav   | (boolean) Whether to add internal navigation to the top of each generated file. Defaults to `False` |
 | DocsBasedir   | What folder to output the docs in. Defaults to `docs/` |
 | Tutorials     | Sets the output folder name for tutorials. Defaults to `tutorials`    |
-| How-tos       | Sets the output folder name for how-tos. Defaults to `how-tos`    |
+| Howtos        | Sets the output folder name for how-tos. Defaults to `how-tos`    |
 | explanations  | Sets the output folder name for explanations. Defaults to `explanations`    |
 | references    | Sets the output folder name for references. Defaults to `references`    |
 
 
 #### [repo] section
 You can add as many of these as you want. Each one represents a repo you want parsed. You can give any name to `[the-section-header]`, but you should probably avoid duplicates. If no repo sections are defined but you've defined DefaultOwner, all repos of that user or organisation will be parsed.
 
 | Parameter | Functionality                              |
 | --------- | ------------------------------------------ |
 | Path      | (string) Defines which repository to parse |
-| Copy      | (array) Files in the repository that should be copied to a specific section. Syntax: `file.md/sectionname,file2.md/sectionname` |
-| Ignore      | (array) Files in the repository that should be ignored. Syntax: `file.md,file2.md` |
+| Move      | (string) Files in the repository that should be copied to a specific section. Syntax: `docs/file.md/section_id//file2.md/section_id/output_filename` |
+| Ignore      | (string) Files in the repository that should be ignored. Syntax: `file.md//file2.md` |
+
+
+**Example Ignore:** `Ignore=building-a-template.md//why-semantic-microservices.md`
+**Example Move:** `Move=documentation.md/references`
+
 
-*Note: for `Copy` and `Ignore` you can choose to be more specific by writing `sub/folder/filename.md`. The check is a `provided_path in full_filepath`, so `sub/folder/filename.md` will apply to `even/further/sub/folder/filename.md`.*
+*Note: for `Move` and `Ignore` you can choose to be more specific by writing `sub/folder/filename.md`. The check is a `provided_path in full_filepath`, so `sub/folder/filename.md` will apply to `even/further/sub/folder/filename.md`.*
 
-##### Allowed Path syntax
-You can use any of the following!
-- `reponame` (if DefaultOwner is defined)
-- `reponame@branch` (if DefaultOwner is defined)
-- `owner/reponame`
-- `owner/reponame@branch`
 
 
 
 ### Synonyms
 For ease of use and freedom of implementation, every section has synonyms.
 
 | Section       | Synonyms                        |
```

### Comparing `divio_docs_gen-0.0.4/pyproject.toml` & `divio_docs_gen-0.1.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "divio_docs_gen"
-version = "0.0.4"
+version = "0.1.0"
 authors = [
     { name="Denperidge", email="denperidge@gmail.com" },
 ]
 description = "Turn all the markdown files in your repos into one big, divio structrured documentation"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -18,12 +18,12 @@
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/Denperidge-Redpencil/divio-docs-gen"
 "Bug Tracker" = "https://github.com/Denperidge-Redpencil/divio-docs-gen/issues"
 
 [project.scripts]
-divio_docs_gen = "divio_docs_gen:generate_docs"
+divio_docs_gen = "divio_docs_gen:main"
 
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
```

### Comparing `divio_docs_gen-0.0.4/src/divio_docs_gen/args.py` & `divio_docs_gen-0.1.0/src/divio_docs_gen/Args.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,154 +1,209 @@
 # Native imports
 from configparser import ConfigParser
 from os import getcwd, path
 from argparse import ArgumentParser
 
+from .Repo import Repo
+
 """Code to handle configuration, through docs.conf or args"""
 
+section_keys = ["tutorials", "howtos", "explanations", "references"]
+class Args:
+    def __init__(self) -> None:
+        # store_true default is False, which means save_conf's output will be too verbose. Use None instead
+        self.save_conf = None  
+        self.write_to_disk = None
+        self.docs_basedir = "docs/"
+        self.generate_nav = None
+
+        self.tutorials, self.howtos, self.explanations, self.references = section_keys
+
+        self.repos = []
+    
+    def get_configured_section_name(self, section_id: str):
+        # TODO look for a cleaner solution
+        if section_id == section_keys[0]:
+            return self.tutorials
+        elif section_id == section_keys[1]:
+            return self.howtos
+        elif section_id == section_keys[2]:
+            return self.explanations
+        elif section_id == section_keys[3]:
+            return self.references
+        print(section_id)
+
+
+    
+    def __str__(self) -> str:
+        return f"""
+        Configured args:
+
+        - save_conf: {self.save_conf} 
+        - write_to_disk: {self.write_to_disk} 
+        - docs_basedir: {self.docs_basedir} 
+        - generate_nav: {self.generate_nav}
+
+        - tutorials: {self.tutorials}
+        - howtos: {self.howtos}
+        - explanations: {self.explanations}
+        - references: {self.references}
+
+        - repos: {self.repos} 
+        """
+
+    def __repr__(self) -> str:
+        return self.__str__()
+
+args = Args()
+
 """ Command-line args """
 parser = ArgumentParser()
 
 conf_sections = {
     "output": "Output Configuration", 
     "naming": "Naming Scheme", 
     "repos": "Repository Selection"
     }
 ouptut_config = parser.add_argument_group(conf_sections["output"])
 ouptut_config.add_argument("--save-conf",
                     dest="SaveConf",
                     help="When used, save the current command line options into ./docs.conf", 
                     action="store_true",
-                    default=None,  # store_true default is False
-                    )
-ouptut_config.add_argument("--generate-nav", "--nav",
-                    dest="GenerateNav",
-                    help="When used, add internal navigation to the top of each generated file", 
-                    action="store_true",
-                    default=None,
-                    )
-ouptut_config.add_argument("--docs-base-dir", "--docs-dir", "--dir", "-d",
-                    dest="DocsBasedir",
-                    help="What folder to output the docs in. Defaults to `docs/", 
+                    default=args.save_conf,  
                     )
 ouptut_config.add_argument("--write-to-disk", "--write",
                            dest="WriteToDisk",
                            help="Whether to write the markdown to disk",
                            action="store_true",
-                           default=None,
+                           default=args.write_to_disk,
                            )
-ouptut_config.add_argument("--dont-remove-tmp", "--tmp",
-                           dest="DontRemoveTmp",
-                           help="When used, the tmp/ folder does not get deleted",
-                           action="store_true",
-                           default=None,
-                           )
-
+ouptut_config.add_argument("--docs-base-dir", "--docs-dir", "--dir", "-d",
+                    dest="DocsBasedir",
+                    help=f"What folder to output the docs in. Defaults to `{args.docs_basedir}`", 
+                    )
+ouptut_config.add_argument("--generate-nav", "--nav",
+                    dest="GenerateNav",
+                    help="When used, add internal navigation to the top of each generated file", 
+                    action="store_true",
+                    default=args.generate_nav,
+                    )
 naming_scheme = parser.add_argument_group(conf_sections["naming"])
-for section_key in ["tutorials", "how-tos", "explanations", "references"]:
+for section_key in section_keys:
     short_hand = section_key[0] if section_key[0] != "h" else "ht"
     naming_scheme.add_argument(f"--{section_key}", f"-{short_hand}", 
                         dest=section_key,
                         help=f"Sets the output folder name for {section_key}. Defaults to `{section_key}`"
                         )
 
 repo_selection = parser.add_argument_group(conf_sections["repos"])
-repo_selection.add_argument("--defaultowner", "--owner", "-do", "-o", 
-                    dest="DefaultOwner",
-                    help="Defines which user or org has to be checked for the repository in case its Path does not explicitly define an owner")
-
 repo_selection.add_argument("--repo",
                             help="""
                             Configures if/how a repo should be parsed
+                            This can be defined multiple times
 
-                            Syntax: OWNER/REPO_NAME [options]
+                            Syntax: --repo git_url
                             Example: denperidge-redpencil/project move=docs/reference/documentation.md
 
                             If none are defined, all repos will be used.
                             Options:
-                            - Copy (array): Files in the repository that should be copied to a specific section. Syntax: move=file.md/sectionname,file2.md/sectionname
-                            - Ignore (array) Files in the repository that should be ignored. Syntax: move=file.md,file2.md
+                            - Move: Files in the repository that should be copied to a specific section. Syntax: move=file.md/sectionname///file2.md/sectionname
+                            - Ignore: Files in the repository that should be ignored. Syntax: ignore=file.md//file2.md
                             """,
                             action="append",
                             dest="repos",
                             nargs="*")
 
-args = parser.parse_args()
-
-
-args_save_conf = bool(getattr(args, "SaveConf")) if hasattr(args, "SaveConf") else False
+cli_args = parser.parse_args()
+args.save_conf = bool(getattr(cli_args, "SaveConf")) if hasattr(cli_args, "SaveConf") else False
 
 """ Conf file """
 conf_file = path.join(getcwd(), "docs.conf")
 use_conf = path.exists(conf_file)
-if use_conf or args_save_conf:
+if use_conf or args.save_conf:
     conf = ConfigParser()
     if use_conf:
         conf.read("docs.conf")
     
     for section_key in conf_sections:
         section = conf_sections[section_key]
         if section not in conf:
             conf.add_section(section)
 
 
-""" Apply & save """
+""" Get config, save if desired, apply"""
 def get_conf_value(section_id, value_id):
     return conf[section_id][value_id] if value_id in conf[section_id] else ""
 
-def get_arg_value(value_id):
-    print(args)
-    return getattr(args, value_id) if hasattr(args, value_id) else None
+def get_cli_arg_value(value_id):
+    return getattr(cli_args, value_id) if hasattr(cli_args, value_id) else None
 
 def get_value(section_id, value_id, default):
     """Gets the arg, whether it be from the config file or CLI"""
     # Get the value from cli if defined. Cli > conf
-    value = get_arg_value(value_id)
+    value = get_cli_arg_value(value_id)
     # If it's undefined in the CLI, check if conf can be used
     if value is None and use_conf:
         value = get_conf_value(section_id, value_id)
     elif value is None:
         value = default
 
-    if args_save_conf:
+    if args.save_conf:
         # If it should be saved, do that
         conf[section_id][value_id] = str(value)
         
     return value
 
-args_default_owner = get_value(conf_sections["repos"], "DefaultOwner", None)  # Used as default repo owner
-args_write_to_disk = bool(get_value(conf_sections["output"], "WriteToDisk", False))
-args_generate_nav = bool(get_value(conf_sections["output"], "GenerateNav", False))
-args_docs_basedir = get_value(conf_sections["output"], "DocsBasedir", "docs/")
-args_dont_remove_tmp = bool(get_value(conf_sections["output"], "DontRemoveTmp", False))
-
-args_section_names = dict()
-for section_name in ["tutorials", "how-tos", "explanations", "references"]:
-    args_section_names[section_name] = get_value(conf_sections["naming"], value_id=section_name, default=section_name).lower()
-print(args_section_names)
-
-args_repoconfigs = []
-if get_arg_value("repos"):
-    for repo_arg in get_arg_value("repos"):
-        repo = dict()
-        repo["path"] = repo_arg[0]
+args.write_to_disk = bool(get_value(conf_sections["output"], "WriteToDisk", False))
+args.generate_nav = bool(get_value(conf_sections["output"], "GenerateNav", False))
+args.docs_basedir = get_value(conf_sections["output"], "DocsBasedir", "docs/")
+
+for i, section_name in enumerate(["tutorials", "howtos", "explanations", "references"]):
+    # TODO cleaner solution
+    value = get_value(conf_sections["naming"], value_id=section_name, default=section_name)
+    if i == 0:
+        args.tutorials = value
+    elif i == 1:
+        args.howtos = value
+    elif i == 2:
+        args.explanations = value
+    elif i == 3:
+        args.references = value
+
+
+if get_cli_arg_value("repos"):
+    for repo_arg in get_cli_arg_value("repos"):
+        repo = Repo(repo_arg[0])
         for arg in repo_arg[1:]:
             key, value = arg.split("=", 1)
-            repo[key] = value
-        args_repoconfigs.append(repo)
-        conf[repo["path"]] = repo
+            key = key.lower()
+            if "ignore" in key:
+                repo.files_to_ignore += value.split("//")
+            elif "move" in key:
+                repo.files_to_move += value.split("//") 
+
+        args.repos.append(repo)
+        conf[repo["url"]] = repo
     
 if use_conf:
     all_conf_sections = conf.sections()
     for conf_section_id in all_conf_sections:
         if conf_section_id in conf_sections.values(): continue
-        
 
         conf_section = conf[conf_section_id]
-        repo = dict(conf_section)
-        if repo not in args_repoconfigs:
-            args_repoconfigs.append(repo)
+        repo_data = dict(conf_section)
+        repo = Repo(repo_data["url"])
+        
+        if "ignore" in repo_data:
+            repo.files_to_ignore += repo_data["ignore"].split("//")
+        if "move" in repo_data:
+            repo.files_to_move += repo_data["move"].split("//")
+
+        if repo not in args.repos:
+            args.repos.append(repo)
         
 
-if args_save_conf:
+if args.save_conf:
     with open("docs.conf", mode="w", encoding="UTF-8") as configfile:
         conf.write(configfile)
+
+print(args)
```

### Comparing `divio_docs_gen-0.0.4/src/divio_docs_gen/sections.py` & `divio_docs_gen-0.1.0/src/divio_docs_gen/Section.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from re import search, RegexFlag, sub, escape
-from .args import args_section_names
+from .Args import args
 
 """Defines section (how-to, getting started...) classes"""
 
 def regex(needle: r"str", haystack: str, flags):
     """Base regex helper"""
     return search(needle, haystack, flags)
 
@@ -17,98 +17,88 @@
     Helper for dotall (. matches newline), case insensitive & multiline regex
     
     For RegexFlag.S, see https://docs.python.org/3/library/re.html#re.S
     """
     return regex(needle, haystack, RegexFlag.IGNORECASE | RegexFlag.MULTILINE | RegexFlag.S)
 
 class Section:
-    """Class to represent a Section (globally)"""
-    def __init__(self, name: str, headertext: str, regex:r"str") -> None:
+    """Class to represent a Section"""
+    def __init__(self, name: str, regex:r"str") -> None:
         self.name = name
-        self.headertext = headertext
         self.regex = regex
     
     @property
-    def regexMdHeader(self):
+    def regex_with_md_header(self):
         """Returns the regex to find this section, accounting for Markdown headers"""
         return r"^#.*" + self.regex
     
 
-    def find_in(self, haystack: str, header = False) -> str:
+    def find_in(self, haystack: str, search_using_markdown_header = False) -> str:
         """Returns the contents of this section from a string"""
-        needle = self.regex if not header else self.regexMdHeader
+        needle = self.regex if not search_using_markdown_header else self.regex_with_md_header
         return regexIM(needle, haystack)
     
-    def found_in(self, haystack: str, header = False) -> bool:
+    def found_in(self, haystack: str, search_using_markdown_header = False) -> bool:
         """Returns True if this section can be found in a string"""
-        return bool(self.find_in(haystack, header))
+        return bool(self.find_in(haystack, search_using_markdown_header))
+    
 
 
-class RepoSection:
-    """Class to represent a Section (in a given repo)"""
-    def __init__(self, section: Section) -> None:
-        self.section = section
-        # sourceContent is the string in which to find the repo section
-        self.sourceContent = str()
-    
-    @property
-    def header(self):
-        """Return the contents of this sections' header"""
-        return self.section.find_in(self.sourceContent, header=True).group()
+     
+    def _get_section_header_from_string(self, input_string: str):
+        """Return the unparsed contents of this sections' header"""
+        return self.find_in(input_string, search_using_markdown_header=True).group()
 
-    @property
-    def headertags(self):
+    def get_header_tags_from_string(self, input_string: str):
         """
         Get the markdown header tags from this header
 
         Example output: ###
         """
         # 
+
         try:
-            return regexIM(r"#*\W", self.header).group()
+            return regexIM(r"#*\W", self._get_section_header_from_string(input_string)).group()
         except AttributeError:
             return None
     
-    # This will return everything between 
-    @property
-    def sectionContent(self):
-        """Find and return everything between the sections header, and the header of the next section"""
+    def _get_content_from_string(self, input_string: str):
+        """Find and return everything between the section header and the header of the next section"""
         # Okay, extracting the content will be a bit complex
         # The regex will contain 3 parts/groups
         # Group 1: the header of the section 
-        regex = r"(^" + escape(self.header) + ")" # Start of line, header, end of line
+        regex = r"(^" + escape(self._get_section_header_from_string(input_string)) + ")" # Start of line, header, end of line
         regex += "(.*)" # All content in between the section header and...
-        regex += escape(self.headertags) + "(\s|\w)"  # The next header of the same size
+        regex += escape(self.get_header_tags_from_string(input_string)) + "(\s|\w)"  # The next header of the same size
         try:
-            return regexIMS(regex, self.sourceContent).groups()[1]  # Use the S flag
+            return regexIMS(regex, input_string).groups()[1]  # Use the S flag
         except AttributeError:
             # If the regex fails, its possible there is no following header
             # TODO cleaner solution
-            regex = r"(^" + escape(self.header) + ")" # Start of line, header, end of line
+            regex = r"(^" + escape(self._get_section_header_from_string(input_string)) + ")" # Start of line, header, end of line
             regex += "(.*)" # All content in between the section header and...
-            return regexIMS(regex, self.sourceContent).groups()[1]  # Use the S flag
+            return regexIMS(regex, input_string).groups()[1]  # Use the S flag
     
-    @property
-    def output(self) -> str:
-        """Outputs the section content with the correct headers"""
+    def extract_and_parse_section_from_string(self, input_string: str) -> str:
+        """Extracts and parses the section content from a string, returning a new string with corrected header tags"""
         # Now we have the unparsed section content,
         # but the headers are all still based on the old file. And our header isn't there!
 
         # To guide you through this, we'll use an example with the following structure
         # ### Tutorials
         # #### First one
         # ##### Subthing
         # #### Second one
 
         #print(self.sourceContent)
         #print(self.section.name)
-        originalBaseHeaderlevel = self.headertags.count('#')  # Example output: 3
+        originalBaseHeaderlevel = self.get_header_tags_from_string(input_string).count('#')  # Example output: 3
         lowerEveryHeaderlevelBy = originalBaseHeaderlevel - 1  # Example output: 2
 
-        output = self.header + self.sectionContent  # Add the original header
+        output = self._get_section_header_from_string(input_string) + self._get_content_from_string(input_string)  # Add the original header
 
 
         header_regex = r"^#*"
         
         def lower_header(match):
             string = match.group()  # Example: ###
             originalHeaderlevel = string.count("#")  # Example: 3
@@ -119,21 +109,20 @@
             
         # run lower_header on every header in here
         output = sub(header_regex, lower_header, output, flags=RegexFlag.IGNORECASE|RegexFlag.MULTILINE)        
 
         return output
 
         
-        
     
 
 """Section definitions. This is where you can customise synonyms"""
 sections = {
-    "tutorials": Section(args_section_names["tutorials"], " tutorials ", r"(tutorial|getting\W*started)"),
-    "howtos": Section(args_section_names["how-tos"], "how to's", r"(how\W*to|guide|usage)"),
-    "explanations": Section(args_section_names["explanations"], "explanation(s)", r"(explanation|discussion|background\W*material)"),
-    "references": Section(args_section_names["references"], "reference(s)", r"(reference|technical)")
+    "tutorials": Section(args.tutorials,       r"(tutorial|getting\W*started)"),
+    "howtos": Section(args.howtos,             r"(how\W*to|guide|usage)"),
+    "explanations": Section(args.explanations, r"(explanation|discussion|background\W*material)"),
+    "references": Section(args.references,     r"(reference|technical)")
 }
```

### Comparing `divio_docs_gen-0.0.4/src/divio_docs_gen.egg-info/PKG-INFO` & `divio_docs_gen-0.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: divio-docs-gen
-Version: 0.0.4
+Name: divio_docs_gen
+Version: 0.1.0
 Summary: Turn all the markdown files in your repos into one big, divio structrured documentation
 Author-email: Denperidge <denperidge@gmail.com>
 Project-URL: Homepage, https://github.com/Denperidge-Redpencil/divio-docs-gen
 Project-URL: Bug Tracker, https://github.com/Denperidge-Redpencil/divio-docs-gen/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Information Technology
@@ -18,19 +18,21 @@
 
 # Divio Docs Generator
 
 Automatically collect, aggregate and structure all your [divio-style documentation](https://documentation.divio.com/) into a tree of .md files.
 ```
 /{reponame}
     /tutorials
-    /how-tos
+    /howtos
     /explanations
     /references
 ```
 
+On a basic level, this repo will only need a list of git url's!
+
 - Any input structure: this script will scan your entire repository for .md files
     - If you have a how-to section in your README, that'll get extracted and put in the right spot
     - Or, if you have an how-to.md file, it'll get added in its entirety!
 - Any output structure: this script generates a simple markdown tree. Nothing proprietary, no vendor-lockin. It can be generated from GitHub Actions and put into a Jekyll pages site just as easily as it is run from a Raspberry Pi and used to render the contents of an Ember application.
 
 All you have to do is simply name your headers and/or files after the divio sections (`tutorial`, `how-to`, `explanation`, `reference`). (Oh, don't worry, the search is done through a case insensitive regex. Add more words as you please) 
 
@@ -66,48 +68,58 @@
 
 ## Discussions
 The Divio structure is built upon splitting your documentation into 4 types of documentations. ![The overview of the divio documentation on their website](https://documentation.divio.com/_images/overview.png). In this repository they're referred to as sections.
 
 
 If you want to know more about the design principles of this project, feel free to check out my writeup [here](https://github.com/Denperidge-Redpencil/Learning.md/blob/main/Notes/docs.md#design-principles)!
 
+Further expansion could be done to this project. For example, a structure like the following...
+```
+/{reponame}
+    /0.0.1
+        /tutorials
+        /how-tos
+        /explanations
+        /references
+```
+... should not be impossible to achieve with some tweaking!
+
 
 ## Reference
 
 ### docs.conf
 #### [DEFAULT] section
 This section is on the top of the file, and defines options that affect the entire configuration
 | Parameter     | Functionality                    |
 | ------------- | -------------------------------- |
-| DefaultOwner | (string) Defines which user or org has to be checked for the repository in case its Path does not explicitly define an owner |
+| DefaultOwner  | (string) Defines which user or org has to be checked for the repository in case its Path does not explicitly define an owner |
 | GenerateNav   | (boolean) Whether to add internal navigation to the top of each generated file. Defaults to `False` |
 | DocsBasedir   | What folder to output the docs in. Defaults to `docs/` |
 | Tutorials     | Sets the output folder name for tutorials. Defaults to `tutorials`    |
-| How-tos       | Sets the output folder name for how-tos. Defaults to `how-tos`    |
+| Howtos        | Sets the output folder name for how-tos. Defaults to `how-tos`    |
 | explanations  | Sets the output folder name for explanations. Defaults to `explanations`    |
 | references    | Sets the output folder name for references. Defaults to `references`    |
 
 
 #### [repo] section
 You can add as many of these as you want. Each one represents a repo you want parsed. You can give any name to `[the-section-header]`, but you should probably avoid duplicates. If no repo sections are defined but you've defined DefaultOwner, all repos of that user or organisation will be parsed.
 
 | Parameter | Functionality                              |
 | --------- | ------------------------------------------ |
 | Path      | (string) Defines which repository to parse |
-| Copy      | (array) Files in the repository that should be copied to a specific section. Syntax: `file.md/sectionname,file2.md/sectionname` |
-| Ignore      | (array) Files in the repository that should be ignored. Syntax: `file.md,file2.md` |
+| Move      | (string) Files in the repository that should be copied to a specific section. Syntax: `docs/file.md/section_id//file2.md/section_id/output_filename` |
+| Ignore      | (string) Files in the repository that should be ignored. Syntax: `file.md//file2.md` |
+
+
+**Example Ignore:** `Ignore=building-a-template.md//why-semantic-microservices.md`
+**Example Move:** `Move=documentation.md/references`
+
 
-*Note: for `Copy` and `Ignore` you can choose to be more specific by writing `sub/folder/filename.md`. The check is a `provided_path in full_filepath`, so `sub/folder/filename.md` will apply to `even/further/sub/folder/filename.md`.*
+*Note: for `Move` and `Ignore` you can choose to be more specific by writing `sub/folder/filename.md`. The check is a `provided_path in full_filepath`, so `sub/folder/filename.md` will apply to `even/further/sub/folder/filename.md`.*
 
-##### Allowed Path syntax
-You can use any of the following!
-- `reponame` (if DefaultOwner is defined)
-- `reponame@branch` (if DefaultOwner is defined)
-- `owner/reponame`
-- `owner/reponame@branch`
 
 
 
 ### Synonyms
 For ease of use and freedom of implementation, every section has synonyms.
 
 | Section       | Synonyms                        |
```

