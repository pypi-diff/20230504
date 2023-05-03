# Comparing `tmp/cpggen-1.0.1.tar.gz` & `tmp/cpggen-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cpggen-1.0.1.tar", max compression
+gzip compressed data, was "cpggen-1.0.2.tar", max compression
```

## Comparing `cpggen-1.0.1.tar` & `cpggen-1.0.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11357 2023-04-28 20:14:32.037230 cpggen-1.0.1/LICENSE
--rw-r--r--   0        0        0     7673 2023-04-28 20:14:32.037230 cpggen-1.0.1/README.md
--rw-r--r--   0        0        0        0 2023-04-28 20:14:32.037230 cpggen-1.0.1/cpggen/__init__.py
--rw-r--r--   0        0        0    13913 2023-04-28 20:14:32.037230 cpggen-1.0.1/cpggen/cli.py
--rw-r--r--   0        0        0    33758 2023-04-28 20:14:32.037230 cpggen-1.0.1/cpggen/executor.py
--rw-r--r--   0        0        0     1015 2023-04-28 20:14:32.037230 cpggen-1.0.1/cpggen/logger.py
--rw-r--r--   0        0        0    11219 2023-04-28 20:14:32.037230 cpggen-1.0.1/cpggen/utils.py
--rw-r--r--   0        0        0     1245 2023-04-28 20:14:32.037230 cpggen-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     9001 1970-01-01 00:00:00.000000 cpggen-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-02 23:17:25.658994 cpggen-1.0.2/LICENSE
+-rw-r--r--   0        0        0     8804 2023-05-03 23:34:20.117294 cpggen-1.0.2/README.md
+-rw-r--r--   0        0        0        0 2023-04-02 23:17:25.658994 cpggen-1.0.2/cpggen/__init__.py
+-rw-r--r--   0        0        0    15322 2023-05-03 22:51:29.854536 cpggen-1.0.2/cpggen/cli.py
+-rw-r--r--   0        0        0    35184 2023-05-03 23:14:38.146112 cpggen-1.0.2/cpggen/executor.py
+-rw-r--r--   0        0        0     1015 2023-04-21 15:09:29.991680 cpggen-1.0.2/cpggen/logger.py
+-rw-r--r--   0        0        0    11219 2023-04-19 13:04:00.729394 cpggen-1.0.2/cpggen/utils.py
+-rw-r--r--   0        0        0     1269 2023-05-03 23:31:22.367109 cpggen-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0    10132 1970-01-01 00:00:00.000000 cpggen-1.0.2/PKG-INFO
```

### Comparing `cpggen-1.0.1/LICENSE` & `cpggen-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cpggen-1.0.1/README.md` & `cpggen-1.0.2/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -27,41 +27,59 @@
 Download the executable binary for your operating system from the [releases page](https://github.com/appthreat/cpggen/releases). These binary bundle the following:
 
 - Joern with all the CPG frontends
 - cpggen with Python 3.10
 - cdxgen with Node.js 18 - Generates SBoM
 
 ```bash
-curl -LO https://github.com/AppThreat/cpggen/releases/download/v1.0.1/cpggen-linux-amd64
+curl -LO https://github.com/AppThreat/cpggen/releases/download/v1.0.2/cpggen-linux-amd64
 chmod +x cpggen-linux-amd64
 ./cpggen-linux-amd64 --help
 ```
 
 On Windows,
 
 ```powershell
-curl -LO https://github.com/appthreat/cpggen/releases/download/v1.0.1/cpggen.exe
+curl -LO https://github.com/appthreat/cpggen/releases/download/v1.0.2/cpggen.exe
 .\cpggen.exe --help
 ```
 
 NOTE: On Windows, antivirus and antimalware could prevent this single executable from functioning properly. Depending on the system, administrative privileges might also be required. Use container-based execution as a fallback.
 
 ### OCI Artifacts via ORAS cli
 
-Use [ORAS cli](https://oras.land/cli/) to download the cpggen binary.
+Use [ORAS cli](https://oras.land/docs/cli/installation/) to download the cpggen binary on Linux and Windows.
+
+```bash
+VERSION="1.0.0"
+curl -LO "https://github.com/oras-project/oras/releases/download/v${VERSION}/oras_${VERSION}_linux_amd64.tar.gz"
+mkdir -p oras-install/
+tar -zxf oras_${VERSION}_*.tar.gz -C oras-install/
+sudo mv oras-install/oras /usr/local/bin/
+rm -rf oras_${VERSION}_*.tar.gz oras-install/
+```
 
 ```bash
 oras pull ghcr.io/appthreat/cpggen-bin:v1
 chmod +x cpggen-linux-amd64
 ./cpggen-linux-amd64 --help
 ```
 
 On Windows
 
 ```powershell
+set VERSION="1.0.0"
+curl.exe -sLO  "https://github.com/oras-project/oras/releases/download/v%VERSION%/oras_%VERSION%_windows_amd64.zip"
+tar.exe -xvzf oras_%VERSION%_windows_amd64.zip
+mkdir -p %USERPROFILE%\bin\
+copy oras.exe %USERPROFILE%\bin\
+set PATH=%USERPROFILE%\bin\;%PATH%
+```
+
+```powershell
 Invoke-WebRequest -Uri https://github.com/oras-project/oras/releases/download/v1.0.0/oras_1.0.0_windows_amd64.zip -UseBasicParsing -OutFile oras_1.0.0_windows_amd64.zip
 Expand-Archive -Path oras_1.0.0_windows_amd64.zip -DestinationPath .
 oras.exe pull ghcr.io/appthreat/cpggen-windows-bin:v1
 ```
 
 ### PyPI package
 
@@ -139,14 +157,22 @@
 
 To export `pdg` in `neo4jcsv` format
 
 ```bash
 cpggen -i ~/work/sandbox/crAPI -o ~/work/sandbox/crAPI/cpg_out --build --export --export-out-dir ~/work/sandbox/crAPI/cpg_export --export-repr pdg --export-format neo4jcsv
 ```
 
+### Slicing graphs
+
+Pass `--slice` argument to extract intra-procedural slices from the CPG. By default, slices would be based on `Usages`. Pass `--slice-mode DataFlow` to create a sliced CPG based on `DataFlow`.
+
+```bash
+cpggen -i ~/work/sandbox/crAPI -o ~/work/sandbox/crAPI/cpg_out --slice
+```
+
 ### Artifacts produced
 
 Upon successful completion, cpggen would produce the following artifacts in the directory specified under `out_dir`
 
 - {name}-{lang}-cpg.bin.zip - Code Property Graph for the given language type
 - {name}-{lang}-cpg.bom.xml - SBoM in CycloneDX XML format
 - {name}-{lang}-cpg.bom.json - SBoM in CycloneDX json format
@@ -200,14 +226,16 @@
 | CPGGEN_CONTAINER_CPU    | CPU units to use in container execution mode. Default computed    |
 | CPGGEN_CONTAINER_MEMORY | Memory units to use in container execution mode. Default computed |
 | CPGGEN_MEMORY           | Heap memory to use for frontends. Default computed                |
 | AT_DEBUG_MODE           | Set to debug to enable debug logging                              |
 | CPG_EXPORT              | Set to true to export CPG graphs in dot format                    |
 | CPG_EXPORT_REPR         | Graph to export. Default all                                      |
 | CPG_EXPORT_FORMAT       | Export format. Default dot                                        |
+| CPG_SLICE               | Set to true to slice CPG                                          |
+| CPG_SLICE_MODE          | Slice mode. Default Usages                                        |
 | SHIFTLEFT_ACCESS_TOKEN  | Set to automatically submit the CPG for analysis by Qwiet AI      |
 
 ## GitHub actions
 
 Use the marketplace [action](https://github.com/marketplace/actions/cpggen) to generate CPGs using GitHub actions. Optionally, the upload the generated CPGs as build artifacts use the below step.
 
 ```
```

### Comparing `cpggen-1.0.1/cpggen/cli.py` & `cpggen-1.0.2/cpggen/cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -134,14 +134,28 @@
     parser.add_argument(
         "--skip-sbom",
         action="store_true",
         default=True if not os.getenv("SHIFTLEFT_ACCESS_TOKEN") else False,
         dest="skip_sbom",
         help="Do not generate SBoM",
     )
+    parser.add_argument(
+        "--slice",
+        action="store_true",
+        default=True if os.getenv("CPG_SLICE") in ("true", "1") else False,
+        dest="slice",
+        help="Extract intra-procedural slices from the CPG",
+    )
+    parser.add_argument(
+        "--slice-mode",
+        default=os.getenv("CPG_SLICE_MODE", "Usages"),
+        dest="slice_mode",
+        choices=["Usages", "DataFlow"],
+        help="Mode used for CPG slicing",
+    )
     return parser.parse_args()
 
 
 @app.get("/")
 async def index():
     return {}
 
@@ -162,14 +176,16 @@
     q = request.args
     params = await request.get_json()
     url = ""
     src = ""
     languages = ""
     cpg_out_dir = None
     is_temp_dir = False
+    auto_build = True
+    skip_sbom = True
     app_manifest_list = []
     if not params:
         params = {}
     if q.get("url"):
         url = q.get("url")
     if q.get("src"):
         src = q.get("src")
@@ -181,14 +197,18 @@
         url = params.get("url")
     if not src and params.get("src"):
         src = params.get("src")
     if not languages and params.get("lang"):
         languages = params.get("lang")
     if not cpg_out_dir and params.get("out_dir"):
         cpg_out_dir = params.get("out_dir")
+    if params.get("auto_build", "") in ("false", "0"):
+        auto_build = False
+    if params.get("skip_sbom", "") in ("false", "0"):
+        skip_sbom = False
     if not src and not url:
         return {"error": "true", "message": "path or url is required"}, 500
     # If src contains url, then reassign
     if not url and (src.startswith("http") or src.startswith("git")):
         url = src
     if url.startswith("http") or url.startswith("git"):
         clone_dir = tempfile.mkdtemp(prefix="cpggen")
@@ -197,22 +217,28 @@
     if cpg_out_dir and not os.path.exists(cpg_out_dir):
         os.makedirs(cpg_out_dir, exist_ok=True)
     if not languages or languages == "autodetect":
         languages = utils.detect_project_type(src)
     else:
         languages = languages.split(",")
     for lang in languages:
+        # Use the deps version of the language when using auto build mode
+        if lang in ("c", "cpp", "java", "kotlin") and auto_build:
+            lang = f"{lang}-with-deps"
         mlist = executor.exec_tool(
             lang,
             src,
             cpg_out_dir,
             src,
             joern_home=os.getenv(
                 "JOERN_HOME", str(Path.home() / "bin" / "joern" / "joern-cli")
             ),
+            use_container=False,
+            auto_build=auto_build,
+            extra_args={"skip_sbom": skip_sbom},
         )
         if mlist:
             app_manifest_list += mlist
     if is_temp_dir:
         try:
             os.remove(src)
         except Exception:
@@ -266,22 +292,25 @@
             pool.join()
 
 
 def collect_cpg_manifests(cpg_out_dir):
     return utils.find_files(cpg_out_dir, ".manifest.json")
 
 
-def export_cpg(
+def export_slice_cpg(
     src,
     cpg_out_dir,
     joern_home,
     use_container,
+    export,
     export_repr,
     export_format,
     export_out_dir,
+    slice,
+    slice_mode,
 ):
     if __name__ in ("__main__", "cpggen.cli"):
         with Pool(processes=os.cpu_count(), initializer=init_worker) as pool:
             try:
                 cpg_manifests = collect_cpg_manifests(cpg_out_dir)
                 for amanifest in cpg_manifests:
                     with open(amanifest) as mfp:
@@ -309,30 +338,34 @@
                         # since the manifest would only have relative path
                         if os.getenv("GITHUB_WORKSPACE") and not cpg_path.startswith(
                             os.getenv("GITHUB_WORKSPACE")
                         ):
                             cpg_path = os.path.join(
                                 os.getenv("GITHUB_WORKSPACE"), cpg_path
                             )
-                        LOG.debug(
-                            f"""Exporting CPG for the app {manifest_obj["app"]} from {cpg_path} to {app_export_out_dir}"""
-                        )
+                        if export:
+                            LOG.debug(
+                                f"""Exporting CPG for the app {manifest_obj["app"]} from {cpg_path} to {app_export_out_dir}"""
+                            )
+                        if slice:
+                            cpg_path = manifest_obj["cpg"]
                         pool.apply_async(
                             executor.exec_tool,
                             (
-                                "export",
+                                "export" if export else "slice",
                                 cpg_path,
                                 app_export_out_dir,
                                 cpg_out_dir,
                                 joern_home,
                                 use_container,
                                 False,
                                 {
-                                    "export_repr": export_repr,
-                                    "export_format": export_format,
+                                    "export_repr": export_repr if export else None,
+                                    "export_format": export_format if export else None,
+                                    "slice_mode": slice_mode if slice else None,
                                 },
                             ),
                         )
                 pool.close()
             except KeyboardInterrupt:
                 pool.terminate()
             pool.join()
@@ -399,23 +432,26 @@
         cpg_out_dir,
         languages,
         joern_home=joern_home,
         use_container=use_container,
         auto_build=args.auto_build,
         skip_sbom=args.skip_sbom,
     )
-    if args.export:
-        export_cpg(
+    if args.export or args.slice:
+        export_slice_cpg(
             src,
             cpg_out_dir,
             joern_home=joern_home,
             use_container=use_container,
+            export=args.export,
             export_repr=args.export_repr,
             export_format=args.export_format,
             export_out_dir=export_out_dir,
+            slice=args.slice,
+            slice_mode=args.slice_mode,
         )
     if is_temp_dir:
         try:
             shutil.rmtree(src)
         except Exception:
             # Ignore cleanup errors
             pass
```

### Comparing `cpggen-1.0.1/cpggen/executor.py` & `cpggen-1.0.2/cpggen/executor.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import sys
 import tempfile
 import zipfile
 from pathlib import Path
 
 import psutil
 from psutil._common import bytes2human
-from rich.progress import Progress, SpinnerColumn, TimeElapsedColumn
+from rich.progress import Progress
 
 from cpggen.logger import DEBUG, LOG, console
 from cpggen.utils import (
     check_command,
     find_csharp_artifacts,
     find_files,
     find_go_mods,
@@ -145,14 +145,15 @@
     "jar": "java -Xmx%(memory)s -Dorg.apache.el.parser.SKIP_IDENTIFIER_CHECK=true -jar %(cpggen_bin_dir)s/java2cpg.jar --experimental-langs=scala -su -o %(cpg_out)s %(uber_jar)s",
     "jar-without-blocklist": "java -Xmx%(memory)s -Dorg.apache.el.parser.SKIP_IDENTIFIER_CHECK=true -jar %(cpggen_bin_dir)s/java2cpg.jar -nb --experimental-langs=scala -su -o %(cpg_out)s %(uber_jar)s",
     "scala": "java -Xmx%(memory)s -Dorg.apache.el.parser.SKIP_IDENTIFIER_CHECK=true -jar %(cpggen_bin_dir)s/java2cpg.jar -nojsp --experimental-langs=scala -su -o %(cpg_out)s %(uber_jar)s",
     "jsp": "java -Xmx%(memory)s -Dorg.apache.el.parser.SKIP_IDENTIFIER_CHECK=true -jar %(cpggen_bin_dir)s/java2cpg.jar --experimental-langs=scala -su -o %(cpg_out)s %(uber_jar)s",
     "jsp-without-blocklist": "java -Xmx%(memory)s -Dorg.apache.el.parser.SKIP_IDENTIFIER_CHECK=true -jar %(cpggen_bin_dir)s/java2cpg.jar -nb --experimental-langs=scala -su -o %(cpg_out)s %(uber_jar)s",
     "sbom": "%(cdxgen_cmd)s -r -t %(tool_lang)s -o %(sbom_out)s %(src)s",
     "export": "%(joern_home)sjoern-export --repr=%(export_repr)s --format=%(export_format)s --out %(cpg_out)s %(src)s",
+    "slice": "%(joern_home)sjoern-slice -m %(slice_mode)s --out %(slice_out)s %(cpg_out)s",
     "qwiet": "sl analyze %(policy)s%(vcs_correction)s--tag app.group=%(group)s --app %(app)s --%(language)s --cpgupload --bomupload %(sbom)s %(cpg)s",
     "dot2png": "dot -Tpng %(dot_file)s -o %(png_out)s",
 }
 
 build_tools_map = {
     "csharp": ["dotnet", "build"],
     "jar": {
@@ -436,14 +437,16 @@
             stderr = subprocess.DEVNULL
             if LOG.isEnabledFor(DEBUG):
                 stdout = subprocess.PIPE
                 stderr = stdout
             tool_verb = f"Building CPG with {tool_lang} frontend"
             if tool_lang == "export":
                 tool_verb = "Exporting CPG with joern-export"
+            elif tool_lang == "slice":
+                tool_verb = "Slicing CPG with joern-slice"
             task = progress.add_task(
                 "[green]" + tool_verb,
                 total=100,
                 start=False,
             )
             cmd_with_args = cpg_tools_map.get(tool_lang)
             if not cmd_with_args:
@@ -492,16 +495,21 @@
                         container_cli = "podman"
                     cmd_with_args = f"""{container_cli} run --rm -w {amodule} -v {tempfile.gettempdir()}:/tmp -v {amodule}:{amodule}:rw -v {os.path.abspath(cpg_out_dir)}:{os.path.abspath(cpg_out_dir)}:rw -t {os.getenv("CPGGEN_IMAGE", "ghcr.io/appthreat/cpggen")} {cmd_with_args}"""
                     # We need to fix joern_home to the directory inside the container
                     joern_home = ""
                 sbom_cmd_with_args = cpg_tools_map.get("sbom")
                 sbom_out = ""
                 manifest_out = ""
+                slice_out = ""
                 if tool_lang == "export":
                     cpg_out = os.path.abspath(cpg_out_dir)
+                elif tool_lang == "slice":
+                    cpg_out = src
+                    slice_out = src.replace(".bin.zip", ".slices")
+                    LOG.debug(f"Output file for {tool_lang} is {slice_out}")
                 else:
                     cpg_out = (
                         cpg_out_dir
                         if cpg_out_dir.endswith(".bin.zip")
                         or cpg_out_dir.endswith(".bin")
                         or cpg_out_dir.endswith(".cpg")
                         else os.path.abspath(
@@ -528,19 +536,20 @@
                     joern_home=joern_home,
                     home_dir=str(Path.home()),
                     uber_jar=uber_jar,
                     csharp_artifacts=csharp_artifacts,
                     memory=os.getenv("CPGGEN_MEMORY", max_memory),
                     tool_lang=tool_lang,
                     sbom_out=sbom_out,
+                    slice_out=slice_out,
                     cpggen_bin_dir=os.getenv("CPGGEN_BIN_DIR", "/usr/local/bin"),
                     bin_ext=bin_ext,
                     **extra_args,
                 )
-                sbom_lang = tool_lang
+                sbom_lang = tool_lang.split("-")[0]
                 if (
                     tool_lang in ("jar", "scala")
                     or tool_lang.startswith("jar")
                     or tool_lang.startswith("jsp")
                 ):
                     sbom_lang = "java"
                 sbom_cmd_with_args = sbom_cmd_with_args % dict(
@@ -561,63 +570,82 @@
                             f"{lang_cmd} is not found. Try running cpggen with --use-container argument"
                         )
                     else:
                         LOG.warn(
                             f"{lang_cmd} is not found. Ensure the PATH variable in your container image is set to the bin directory of Joern."
                         )
                     return
-                # Is this an Export task?
-                if tool_lang == "export":
+                # Is this an Export or Slice task?
+                if tool_lang in ("export", "slice"):
                     try:
                         progress.update(
-                            task, description="Exporting CPG", completed=90, total=100
+                            task,
+                            description=f"{tool_lang.capitalize()} CPG",
+                            completed=90,
+                            total=100,
                         )
                         cp = subprocess.run(
                             cmd_list_with_args,
                             stdout=stdout,
                             stderr=stderr,
                             cwd=cwd,
                             env=env,
                             check=False,
                             shell=use_shell,
                             encoding="utf-8",
                         )
                         if cp and cp.returncode and cp.stderr:
-                            LOG.warn(f"Export CPG has failed for {src}")
+                            LOG.warn(
+                                f"{tool_lang.capitalize()} operation has failed for {src}"
+                            )
                             if not os.getenv("AT_DEBUG_MODE"):
                                 LOG.info(
                                     "Set the environment variable AT_DEBUG_MODE to debug to see the debug logs"
                                 )
                             if cp.stdout:
                                 LOG.info(cp.stdout)
                             if cp.stderr:
                                 LOG.info("------------------------------")
                                 LOG.info(cp.stderr)
                                 LOG.info("------------------------------")
                                 LOG.info(
                                     f"Command used {' '.join(cmd_list_with_args)}\nPlease report the above error to https://github.com/joernio/joern/issues"
                                 )
                         else:
-                            if os.path.exists(cpg_out_dir):
-                                LOG.info(
-                                    f"CPG {src} successfully exported to {cpg_out_dir}"
+                            check_dir = (
+                                cpg_out_dir
+                                if tool_lang == "export"
+                                else (
+                                    slice_out
+                                    + (
+                                        ".json"
+                                        if extra_args.get("slice_mode") == "Usages"
+                                        else ".cpg"
+                                    )
                                 )
-                                progress.update(
-                                    task,
-                                    description="Convert exported graph to png",
-                                    completed=95,
-                                    total=100,
+                            )
+                            if os.path.exists(check_dir):
+                                LOG.info(
+                                    f"CPG {src} successfully {tool_lang + ('d' if tool_lang.endswith('e') else 'ed')} to {check_dir}"
                                 )
-                                dot_convert(cpg_out_dir, env)
+                                # Convert dot files to png
+                                if tool_lang == "export":
+                                    progress.update(
+                                        task,
+                                        description="Convert exported graph to png",
+                                        completed=95,
+                                        total=100,
+                                    )
+                                    dot_convert(cpg_out_dir, env)
                             else:
                                 LOG.warn(
-                                    f"Unable to export {src} to {cpg_out_dir}. Try running joern-export manually using the command {' '.join(cmd_list_with_args)}"
+                                    f"Unable to {tool_lang} {src} to {check_dir}. Try running joern-{tool_lang} manually using the command {' '.join(cmd_list_with_args)}"
                                 )
                     except Exception as e:
-                        LOG.warn(f"Unable to export {src} to {cpg_out_dir}")
+                        LOG.warn(f"Unable to {tool_lang} {src} to {cpg_out_dir}")
                         LOG.error(e)
                     progress.update(task, completed=100, total=100)
                     continue
                 LOG.info(
                     '⚡︎ Generating CPG for the {} app "{}" - "{}"'.format(
                         tool_lang,
                         os.path.basename(amodule),
```

### Comparing `cpggen-1.0.1/cpggen/logger.py` & `cpggen-1.0.2/cpggen/logger.py`

 * *Files identical despite different names*

### Comparing `cpggen-1.0.1/cpggen/utils.py` & `cpggen-1.0.2/cpggen/utils.py`

 * *Files identical despite different names*

### Comparing `cpggen-1.0.1/pyproject.toml` & `cpggen-1.0.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cpggen"
-version = "1.0.1"
+version = "1.0.2"
 description = "Generate CPG for multiple languages for use with joern"
 authors = ["Team AppThreat <cloud@appthreat.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{include = "cpggen"}]
 homepage = "https://github.com/AppThreat/cpggen"
 repository = "https://github.com/AppThreat/cpggen"
@@ -20,21 +20,22 @@
     "Programming Language :: Python :: 3.10",
     "Operating System :: OS Independent",
 ]
 exclude = ["contrib", "tests"]
 
 [tool.poetry.scripts]
 cpggen = 'cpggen.cli:main'
+cpg = 'cpggen.cli:main'
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
-rich = "^13.3.2"
+rich = "^13.3.5"
 gitpython = "^3.1.31"
-quart = "^0.18.3"
-psutil = "^5.9.4"
+quart = "^0.18.4"
+psutil = "^5.9.5"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.2"
 black = "^22.3.0"
 flake8 = "^4.0.1"
 pytest-cov = "^3.0.0"
 pyinstaller = "^5.0.1"
```

### Comparing `cpggen-1.0.1/PKG-INFO` & `cpggen-1.0.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpggen
-Version: 1.0.1
+Version: 1.0.2
 Summary: Generate CPG for multiple languages for use with joern
 Home-page: https://github.com/AppThreat/cpggen
 License: Apache-2.0
 Keywords: joern,code analysis,static analysis,cpg,code property graph
 Author: Team AppThreat
 Author-email: cloud@appthreat.com
 Requires-Python: >=3.8,<3.12
@@ -20,17 +20,17 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Security
 Classifier: Topic :: Utilities
 Requires-Dist: gitpython (>=3.1.31,<4.0.0)
-Requires-Dist: psutil (>=5.9.4,<6.0.0)
-Requires-Dist: quart (>=0.18.3,<0.19.0)
-Requires-Dist: rich (>=13.3.2,<14.0.0)
+Requires-Dist: psutil (>=5.9.5,<6.0.0)
+Requires-Dist: quart (>=0.18.4,<0.19.0)
+Requires-Dist: rich (>=13.3.5,<14.0.0)
 Project-URL: Repository, https://github.com/AppThreat/cpggen
 Description-Content-Type: text/markdown
 
 # CPG Generator
 
 ```
  ██████╗██████╗  ██████╗
@@ -59,41 +59,59 @@
 Download the executable binary for your operating system from the [releases page](https://github.com/appthreat/cpggen/releases). These binary bundle the following:
 
 - Joern with all the CPG frontends
 - cpggen with Python 3.10
 - cdxgen with Node.js 18 - Generates SBoM
 
 ```bash
-curl -LO https://github.com/AppThreat/cpggen/releases/download/v1.0.1/cpggen-linux-amd64
+curl -LO https://github.com/AppThreat/cpggen/releases/download/v1.0.2/cpggen-linux-amd64
 chmod +x cpggen-linux-amd64
 ./cpggen-linux-amd64 --help
 ```
 
 On Windows,
 
 ```powershell
-curl -LO https://github.com/appthreat/cpggen/releases/download/v1.0.1/cpggen.exe
+curl -LO https://github.com/appthreat/cpggen/releases/download/v1.0.2/cpggen.exe
 .\cpggen.exe --help
 ```
 
 NOTE: On Windows, antivirus and antimalware could prevent this single executable from functioning properly. Depending on the system, administrative privileges might also be required. Use container-based execution as a fallback.
 
 ### OCI Artifacts via ORAS cli
 
-Use [ORAS cli](https://oras.land/cli/) to download the cpggen binary.
+Use [ORAS cli](https://oras.land/docs/cli/installation/) to download the cpggen binary on Linux and Windows.
+
+```bash
+VERSION="1.0.0"
+curl -LO "https://github.com/oras-project/oras/releases/download/v${VERSION}/oras_${VERSION}_linux_amd64.tar.gz"
+mkdir -p oras-install/
+tar -zxf oras_${VERSION}_*.tar.gz -C oras-install/
+sudo mv oras-install/oras /usr/local/bin/
+rm -rf oras_${VERSION}_*.tar.gz oras-install/
+```
 
 ```bash
 oras pull ghcr.io/appthreat/cpggen-bin:v1
 chmod +x cpggen-linux-amd64
 ./cpggen-linux-amd64 --help
 ```
 
 On Windows
 
 ```powershell
+set VERSION="1.0.0"
+curl.exe -sLO  "https://github.com/oras-project/oras/releases/download/v%VERSION%/oras_%VERSION%_windows_amd64.zip"
+tar.exe -xvzf oras_%VERSION%_windows_amd64.zip
+mkdir -p %USERPROFILE%\bin\
+copy oras.exe %USERPROFILE%\bin\
+set PATH=%USERPROFILE%\bin\;%PATH%
+```
+
+```powershell
 Invoke-WebRequest -Uri https://github.com/oras-project/oras/releases/download/v1.0.0/oras_1.0.0_windows_amd64.zip -UseBasicParsing -OutFile oras_1.0.0_windows_amd64.zip
 Expand-Archive -Path oras_1.0.0_windows_amd64.zip -DestinationPath .
 oras.exe pull ghcr.io/appthreat/cpggen-windows-bin:v1
 ```
 
 ### PyPI package
 
@@ -171,14 +189,22 @@
 
 To export `pdg` in `neo4jcsv` format
 
 ```bash
 cpggen -i ~/work/sandbox/crAPI -o ~/work/sandbox/crAPI/cpg_out --build --export --export-out-dir ~/work/sandbox/crAPI/cpg_export --export-repr pdg --export-format neo4jcsv
 ```
 
+### Slicing graphs
+
+Pass `--slice` argument to extract intra-procedural slices from the CPG. By default, slices would be based on `Usages`. Pass `--slice-mode DataFlow` to create a sliced CPG based on `DataFlow`.
+
+```bash
+cpggen -i ~/work/sandbox/crAPI -o ~/work/sandbox/crAPI/cpg_out --slice
+```
+
 ### Artifacts produced
 
 Upon successful completion, cpggen would produce the following artifacts in the directory specified under `out_dir`
 
 - {name}-{lang}-cpg.bin.zip - Code Property Graph for the given language type
 - {name}-{lang}-cpg.bom.xml - SBoM in CycloneDX XML format
 - {name}-{lang}-cpg.bom.json - SBoM in CycloneDX json format
@@ -232,14 +258,16 @@
 | CPGGEN_CONTAINER_CPU    | CPU units to use in container execution mode. Default computed    |
 | CPGGEN_CONTAINER_MEMORY | Memory units to use in container execution mode. Default computed |
 | CPGGEN_MEMORY           | Heap memory to use for frontends. Default computed                |
 | AT_DEBUG_MODE           | Set to debug to enable debug logging                              |
 | CPG_EXPORT              | Set to true to export CPG graphs in dot format                    |
 | CPG_EXPORT_REPR         | Graph to export. Default all                                      |
 | CPG_EXPORT_FORMAT       | Export format. Default dot                                        |
+| CPG_SLICE               | Set to true to slice CPG                                          |
+| CPG_SLICE_MODE          | Slice mode. Default Usages                                        |
 | SHIFTLEFT_ACCESS_TOKEN  | Set to automatically submit the CPG for analysis by Qwiet AI      |
 
 ## GitHub actions
 
 Use the marketplace [action](https://github.com/marketplace/actions/cpggen) to generate CPGs using GitHub actions. Optionally, the upload the generated CPGs as build artifacts use the below step.
 
 ```
```

