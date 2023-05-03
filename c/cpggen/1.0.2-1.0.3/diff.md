# Comparing `tmp/cpggen-1.0.2.tar.gz` & `tmp/cpggen-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cpggen-1.0.2.tar", max compression
+gzip compressed data, was "cpggen-1.0.3.tar", max compression
```

## Comparing `cpggen-1.0.2.tar` & `cpggen-1.0.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11357 2023-04-02 23:17:25.658994 cpggen-1.0.2/LICENSE
--rw-r--r--   0        0        0     8804 2023-05-03 23:34:20.117294 cpggen-1.0.2/README.md
--rw-r--r--   0        0        0        0 2023-04-02 23:17:25.658994 cpggen-1.0.2/cpggen/__init__.py
--rw-r--r--   0        0        0    15322 2023-05-03 22:51:29.854536 cpggen-1.0.2/cpggen/cli.py
--rw-r--r--   0        0        0    35184 2023-05-03 23:14:38.146112 cpggen-1.0.2/cpggen/executor.py
--rw-r--r--   0        0        0     1015 2023-04-21 15:09:29.991680 cpggen-1.0.2/cpggen/logger.py
--rw-r--r--   0        0        0    11219 2023-04-19 13:04:00.729394 cpggen-1.0.2/cpggen/utils.py
--rw-r--r--   0        0        0     1269 2023-05-03 23:31:22.367109 cpggen-1.0.2/pyproject.toml
--rw-r--r--   0        0        0    10132 1970-01-01 00:00:00.000000 cpggen-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-03 23:53:48.127528 cpggen-1.0.3/LICENSE
+-rw-r--r--   0        0        0     8804 2023-05-03 23:53:48.127528 cpggen-1.0.3/README.md
+-rw-r--r--   0        0        0        0 2023-05-03 23:53:48.131528 cpggen-1.0.3/cpggen/__init__.py
+-rw-r--r--   0        0        0    15322 2023-05-03 23:53:48.131528 cpggen-1.0.3/cpggen/cli.py
+-rw-r--r--   0        0        0    35417 2023-05-03 23:53:48.131528 cpggen-1.0.3/cpggen/executor.py
+-rw-r--r--   0        0        0     1015 2023-05-03 23:53:48.131528 cpggen-1.0.3/cpggen/logger.py
+-rw-r--r--   0        0        0    11547 2023-05-03 23:53:48.131528 cpggen-1.0.3/cpggen/utils.py
+-rw-r--r--   0        0        0     1269 2023-05-03 23:53:48.131528 cpggen-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0    10132 1970-01-01 00:00:00.000000 cpggen-1.0.3/PKG-INFO
```

### Comparing `cpggen-1.0.2/LICENSE` & `cpggen-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cpggen-1.0.2/README.md` & `cpggen-1.0.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -27,23 +27,23 @@
 Download the executable binary for your operating system from the [releases page](https://github.com/appthreat/cpggen/releases). These binary bundle the following:
 
 - Joern with all the CPG frontends
 - cpggen with Python 3.10
 - cdxgen with Node.js 18 - Generates SBoM
 
 ```bash
-curl -LO https://github.com/AppThreat/cpggen/releases/download/v1.0.2/cpggen-linux-amd64
+curl -LO https://github.com/AppThreat/cpggen/releases/download/v1.0.3/cpggen-linux-amd64
 chmod +x cpggen-linux-amd64
 ./cpggen-linux-amd64 --help
 ```
 
 On Windows,
 
 ```powershell
-curl -LO https://github.com/appthreat/cpggen/releases/download/v1.0.2/cpggen.exe
+curl -LO https://github.com/appthreat/cpggen/releases/download/v1.0.3/cpggen.exe
 .\cpggen.exe --help
 ```
 
 NOTE: On Windows, antivirus and antimalware could prevent this single executable from functioning properly. Depending on the system, administrative privileges might also be required. Use container-based execution as a fallback.
 
 ### OCI Artifacts via ORAS cli
```

### Comparing `cpggen-1.0.2/cpggen/cli.py` & `cpggen-1.0.3/cpggen/cli.py`

 * *Files identical despite different names*

### Comparing `cpggen-1.0.2/cpggen/executor.py` & `cpggen-1.0.3/cpggen/executor.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,14 +127,15 @@
 cpg_tools_map = {
     "c": "%(joern_home)sc2cpg%(bin_ext)s -J-Xmx%(memory)s -o %(cpg_out)s %(src)s",
     "cpp": "%(joern_home)sc2cpg%(bin_ext)s -J-Xmx%(memory)s -o %(cpg_out)s %(src)s",
     "c-with-deps": "%(joern_home)sc2cpg%(bin_ext)s -J-Xmx%(memory)s -o %(cpg_out)s %(src)s --with-include-auto-discovery",
     "cpp-with-deps": "%(joern_home)sc2cpg%(bin_ext)s -J-Xmx%(memory)s -o %(cpg_out)s %(src)s --with-include-auto-discovery",
     "java": "%(joern_home)sjavasrc2cpg -J-Xmx%(memory)s -o %(cpg_out)s %(src)s",
     "java-with-deps": "%(joern_home)sjavasrc2cpg -J-Xmx%(memory)s -o %(cpg_out)s %(src)s --fetch-dependencies --inference-jar-paths %(home_dir)s/.m2",
+    "java-with-gradle-deps": "%(joern_home)sjavasrc2cpg -J-Xmx%(memory)s -o %(cpg_out)s %(src)s --fetch-dependencies --inference-jar-paths %(home_dir)s/.gradle/caches/modules-2/files-2.1",
     "binary": "%(joern_home)sghidra2cpg -J-Xmx%(memory)s -o %(cpg_out)s %(src)s",
     "js": "%(joern_home)sjssrc2cpg%(bin_ext)s -J-Xmx%(memory)s -o %(cpg_out)s %(src)s",
     "ts": "%(joern_home)sjssrc2cpg%(bin_ext)s -J-Xmx%(memory)s -o %(cpg_out)s %(src)s",
     "kotlin": "%(joern_home)skotlin2cpg -J-Xmx%(memory)s -o %(cpg_out)s %(src)s",
     "kotlin-with-deps": "%(joern_home)skotlin2cpg -J-Xmx%(memory)s -o %(cpg_out)s %(src)s --download-dependencies",
     "kotlin-with-classpath": "%(joern_home)skotlin2cpg -J-Xmx%(memory)s -o %(cpg_out)s %(src)s --classpath %(home_dir)s/.m2 --classpath %(home_dir)s/.gradle/caches/modules-2/files-2.1",
     "php": "%(joern_home)sphp2cpg -J-Xmx%(memory)s -o %(cpg_out)s %(src)s",
@@ -422,14 +423,15 @@
         redirect_stderr=False,
         redirect_stdout=False,
         refresh_per_second=1,
     ) as progress:
         task = None
         lang_build_crashes = {}
         app_manifest_list = []
+        tool_lang_simple = tool_lang.split("-")[0]
         if cwd:
             if os.path.isfile(cwd):
                 cwd = os.path.dirname(cwd)
             else:
                 cwd = os.path.abspath(cwd)
         if joern_home and not joern_home.endswith(os.path.sep):
             joern_home = f"{joern_home}{os.path.sep}"
@@ -511,15 +513,15 @@
                         cpg_out_dir
                         if cpg_out_dir.endswith(".bin.zip")
                         or cpg_out_dir.endswith(".bin")
                         or cpg_out_dir.endswith(".cpg")
                         else os.path.abspath(
                             os.path.join(
                                 cpg_out_dir,
-                                f"{os.path.basename(amodule)}-{tool_lang}-cpg.bin.zip",
+                                f"{os.path.basename(amodule)}-{tool_lang_simple}-cpg.bin.zip",
                             )
                         )
                     )
                     sbom_out = (
                         cpg_out.replace(".bin.zip", ".bom.xml")
                         if cpg_out.endswith(".bin.zip")
                         else f"{cpg_out}.bom.xml"
@@ -541,15 +543,15 @@
                     tool_lang=tool_lang,
                     sbom_out=sbom_out,
                     slice_out=slice_out,
                     cpggen_bin_dir=os.getenv("CPGGEN_BIN_DIR", "/usr/local/bin"),
                     bin_ext=bin_ext,
                     **extra_args,
                 )
-                sbom_lang = tool_lang.split("-")[0]
+                sbom_lang = tool_lang_simple
                 if (
                     tool_lang in ("jar", "scala")
                     or tool_lang.startswith("jar")
                     or tool_lang.startswith("jsp")
                 ):
                     sbom_lang = "java"
                 sbom_cmd_with_args = sbom_cmd_with_args % dict(
@@ -725,15 +727,15 @@
                         )
                     with open(manifest_out, mode="w") as mfp:
                         # In case of github action, we need to convert this to relative path
                         if os.getenv("GITHUB_PATH"):
                             cpg_out = cpg_out.replace("/github/workspace/", "")
                             sbom_out = sbom_out.replace("/github/workspace/", "")
                             amodule = amodule.replace("/github/workspace/", "")
-                        language = tool_lang.split("-")[0]
+                        language = tool_lang_simple
                         # Override the language for jvm
                         if qwiet_lang_map.get(language):
                             language = qwiet_lang_map.get(language)
                         app_base_name = os.path.basename(amodule)
                         # Let's improve the name for github action
                         if app_base_name == "workspace" and os.getenv(
                             "GITHUB_REPOSITORY"
```

### Comparing `cpggen-1.0.2/cpggen/logger.py` & `cpggen-1.0.3/cpggen/logger.py`

 * *Files identical despite different names*

### Comparing `cpggen-1.0.2/cpggen/utils.py` & `cpggen-1.0.3/cpggen/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -343,15 +343,22 @@
         find_files(src_dir, "pom.xml", False, True)
         or find_files(src_dir, ".gradle", False, True)
         or find_files(src_dir, ".java", False, True)
     ):
         if os.getenv("SHIFTLEFT_ACCESS_TOKEN"):
             project_types.append("jar")
         else:
-            project_types.append("java")
+            if os.path.exists(str(Path.home() / ".m2")):
+                project_types.append("java-with-deps")
+            elif os.path.exists(
+                str(Path.home() / ".gradle" / "caches" / "modules-2" / "files-2.1")
+            ):
+                project_types.append("java-with-gradle-deps")
+            else:
+                project_types.append("java")
     if find_files(src_dir, ".bzl", False, True) or find_files(
         src_dir, "BUILD", False, True
     ):
         project_types.append("java")
     if find_files(src_dir, ".jsp", False, True):
         project_types.append("jsp")
     if (
```

### Comparing `cpggen-1.0.2/pyproject.toml` & `cpggen-1.0.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cpggen"
-version = "1.0.2"
+version = "1.0.3"
 description = "Generate CPG for multiple languages for use with joern"
 authors = ["Team AppThreat <cloud@appthreat.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{include = "cpggen"}]
 homepage = "https://github.com/AppThreat/cpggen"
 repository = "https://github.com/AppThreat/cpggen"
```

### Comparing `cpggen-1.0.2/PKG-INFO` & `cpggen-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpggen
-Version: 1.0.2
+Version: 1.0.3
 Summary: Generate CPG for multiple languages for use with joern
 Home-page: https://github.com/AppThreat/cpggen
 License: Apache-2.0
 Keywords: joern,code analysis,static analysis,cpg,code property graph
 Author: Team AppThreat
 Author-email: cloud@appthreat.com
 Requires-Python: >=3.8,<3.12
@@ -59,23 +59,23 @@
 Download the executable binary for your operating system from the [releases page](https://github.com/appthreat/cpggen/releases). These binary bundle the following:
 
 - Joern with all the CPG frontends
 - cpggen with Python 3.10
 - cdxgen with Node.js 18 - Generates SBoM
 
 ```bash
-curl -LO https://github.com/AppThreat/cpggen/releases/download/v1.0.2/cpggen-linux-amd64
+curl -LO https://github.com/AppThreat/cpggen/releases/download/v1.0.3/cpggen-linux-amd64
 chmod +x cpggen-linux-amd64
 ./cpggen-linux-amd64 --help
 ```
 
 On Windows,
 
 ```powershell
-curl -LO https://github.com/appthreat/cpggen/releases/download/v1.0.2/cpggen.exe
+curl -LO https://github.com/appthreat/cpggen/releases/download/v1.0.3/cpggen.exe
 .\cpggen.exe --help
 ```
 
 NOTE: On Windows, antivirus and antimalware could prevent this single executable from functioning properly. Depending on the system, administrative privileges might also be required. Use container-based execution as a fallback.
 
 ### OCI Artifacts via ORAS cli
```

