# Comparing `tmp/vmn-0.8.1-py3-none-any.whl.zip` & `tmp/vmn-0.8.2rc1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 44970 bytes, number of entries: 10
+Zip file size: 45389 bytes, number of entries: 10
 -rw-r--r--  2.0 unx      152 b- defN 21-Jul-06 16:25 version_stamp/__init__.py
 -rw-r--r--  2.0 unx    53098 b- defN 23-Apr-16 14:06 version_stamp/stamp_utils.py
--rw-r--r--  2.0 unx       50 b- defN 23-Apr-20 15:47 version_stamp/version.py
--rw-r--r--  2.0 unx   109439 b- defN 23-Apr-20 12:54 version_stamp/vmn.py
--rw-r--r--  2.0 unx    35127 b- defN 23-Apr-20 15:47 vmn-0.8.1.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      468 b- defN 23-Apr-20 15:47 vmn-0.8.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-20 15:47 vmn-0.8.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       47 b- defN 23-Apr-20 15:47 vmn-0.8.1.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       14 b- defN 23-Apr-20 15:47 vmn-0.8.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      786 b- defN 23-Apr-20 15:47 vmn-0.8.1.dist-info/RECORD
-10 files, 199273 bytes uncompressed, 43636 bytes compressed:  78.1%
+-rw-r--r--  2.0 unx       58 b- defN 23-May-04 07:59 version_stamp/version.py
+-rw-r--r--  2.0 unx   112040 b- defN 23-May-04 07:40 version_stamp/vmn.py
+-rw-r--r--  2.0 unx    35127 b- defN 23-May-04 07:59 vmn-0.8.2rc1.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      470 b- defN 23-May-04 07:59 vmn-0.8.2rc1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-04 07:59 vmn-0.8.2rc1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       47 b- defN 23-May-04 07:59 vmn-0.8.2rc1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       14 b- defN 23-May-04 07:59 vmn-0.8.2rc1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      804 b- defN 23-May-04 07:59 vmn-0.8.2rc1.dist-info/RECORD
+10 files, 201902 bytes uncompressed, 44019 bytes compressed:  78.2%
```

## zipnote {}

```diff
@@ -6,26 +6,26 @@
 
 Filename: version_stamp/version.py
 Comment: 
 
 Filename: version_stamp/vmn.py
 Comment: 
 
-Filename: vmn-0.8.1.dist-info/LICENSE.txt
+Filename: vmn-0.8.2rc1.dist-info/LICENSE.txt
 Comment: 
 
-Filename: vmn-0.8.1.dist-info/METADATA
+Filename: vmn-0.8.2rc1.dist-info/METADATA
 Comment: 
 
-Filename: vmn-0.8.1.dist-info/WHEEL
+Filename: vmn-0.8.2rc1.dist-info/WHEEL
 Comment: 
 
-Filename: vmn-0.8.1.dist-info/entry_points.txt
+Filename: vmn-0.8.2rc1.dist-info/entry_points.txt
 Comment: 
 
-Filename: vmn-0.8.1.dist-info/top_level.txt
+Filename: vmn-0.8.2rc1.dist-info/top_level.txt
 Comment: 
 
-Filename: vmn-0.8.1.dist-info/RECORD
+Filename: vmn-0.8.2rc1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## version_stamp/version.py

```diff
@@ -1,3 +1,3 @@
 name = "vmn"
-version = "0.8.1"
-_version = "0.8.1"
+version = "0.8.2-rc1"
+_version = "0.8.2-rc1"
```

## version_stamp/vmn.py

```diff
@@ -397,15 +397,15 @@
             del self.backend
             self.backend = None
 
     # Note: this function generates a version (including prerelease)
     def gen_advanced_version(
         self, initial_version, initialprerelease, initialprerelease_count
     ):
-        verstr = self._advance_version(initial_version)
+        verstr = self.advance_version(initial_version, self.release_mode)
 
         prerelease = self.prerelease
         # If user did not specify a change in prerelease,
         # stay with the previous one
         if prerelease is None and self.release_mode is None:
             prerelease = initialprerelease
         prerelease_count = copy.deepcopy(initialprerelease_count)
@@ -454,72 +454,72 @@
         prerelease_count[counter_key] += 1
 
         if self.release_mode is not None:
             prerelease_count = {counter_key: 1}
 
         return counter_key, prerelease_count
 
-    def increase_octet(self, tag_name_prefix: str, version_number_oct: str) -> str:
+    def increase_octet(self, tag_name_prefix: str, version_number_oct: str, release_mode: str, globally: bool) -> str:
         tag = self.backend.get_latest_available_tag(tag_name_prefix)
         version_number_oct = int(version_number_oct)
-        if tag:
+        if tag and globally:
             props = stamp_utils.VMNBackend.deserialize_vmn_tag_name(tag)
-            version_number_oct = max(version_number_oct, int(props[self.release_mode]))
+            version_number_oct = max(version_number_oct, int(props[release_mode]))
         version_number_oct += 1
         return str(version_number_oct)
 
-    def _advance_version(self, version):
+    def advance_version(self, version, release_mode, globally=True):
         # TODO: maybe move up the version validity test
         match = re.search(stamp_utils.VMN_REGEX, version)
         gdict = match.groupdict()
         if gdict["hotfix"] is None:
             gdict["hotfix"] = "0"
 
         major = gdict["major"]
         minor = gdict["minor"]
         patch = gdict["patch"]
         hotfix = gdict["hotfix"]
 
-        if self.release_mode == "major":
+        if release_mode == "major":
             tag_name_prefix = stamp_utils.VMNBackend.app_name_to_git_tag_app_name(
                 self.name
             )
 
             tag_name_prefix = f"{tag_name_prefix}_*"
-            major = self.increase_octet(tag_name_prefix, major)
+            major = self.increase_octet(tag_name_prefix, major, release_mode, globally)
 
             minor = "0"
             patch = "0"
             hotfix = "0"
-        elif self.release_mode == "minor":
+        elif release_mode == "minor":
             tag_name_prefix = stamp_utils.VMNBackend.app_name_to_git_tag_app_name(
                 self.name
             )
 
             tag_name_prefix = f"{tag_name_prefix}_{major}*"
-            minor = self.increase_octet(tag_name_prefix, minor)
+            minor = self.increase_octet(tag_name_prefix, minor, release_mode, globally)
 
             patch = "0"
             hotfix = "0"
-        elif self.release_mode == "patch":
+        elif release_mode == "patch":
             tag_name_prefix = stamp_utils.VMNBackend.app_name_to_git_tag_app_name(
                 self.name
             )
 
             tag_name_prefix = f"{tag_name_prefix}_{major}.{minor}*"
-            patch = self.increase_octet(tag_name_prefix, patch)
+            patch = self.increase_octet(tag_name_prefix, patch, release_mode, globally)
 
             hotfix = "0"
-        elif self.release_mode == "hotfix":
+        elif release_mode == "hotfix":
             tag_name_prefix = stamp_utils.VMNBackend.app_name_to_git_tag_app_name(
                 self.name
             )
 
             tag_name_prefix = f"{tag_name_prefix}_{major}.{minor}.{patch}*"
-            hotfix = self.increase_octet(tag_name_prefix, hotfix)
+            hotfix = self.increase_octet(tag_name_prefix, hotfix, release_mode, globally)
 
         return stamp_utils.VMNBackend.serialize_vmn_version_hotfix(
             self.hide_zero_hotfix,
             major,
             minor,
             patch,
             hotfix,
@@ -1432,32 +1432,24 @@
 
 
 @stamp_utils.measure_runtime_decorator
 def handle_stamp(vmn_ctx):
     vmn_ctx.vcs.prerelease = vmn_ctx.args.pr
     vmn_ctx.vcs.buildmetadata = None
     vmn_ctx.vcs.release_mode = vmn_ctx.args.release_mode
+    vmn_ctx.vcs.optional_release_mode = vmn_ctx.args.orm
     vmn_ctx.vcs.override_root_version = vmn_ctx.args.orv
     vmn_ctx.vcs.override_version = vmn_ctx.args.ov
     vmn_ctx.vcs.dry_run = vmn_ctx.args.dry
 
     # For backward compatibility
     if vmn_ctx.vcs.release_mode == "micro":
         vmn_ctx.vcs.release_mode = "hotfix"
 
-    if vmn_ctx.vcs.tracked and vmn_ctx.vcs.release_mode is None:
-        vmn_ctx.vcs.current_version_info["stamping"]["app"][
-            "release_mode"
-        ] = vmn_ctx.vcs.ver_infos_from_repo[vmn_ctx.vcs.selected_tag]["ver_info"][
-            "stamping"
-        ][
-            "app"
-        ][
-            "release_mode"
-        ]
+    assert vmn_ctx.vcs.release_mode is None or vmn_ctx.vcs.optional_release_mode is None
 
     optional_status = {"modified", "detached"}
     expected_status = {
         "repos_exist_locally",
         "repo_tracked",
         "app_tracked",
         "deps_synced_with_conf",
@@ -1508,14 +1500,57 @@
     ) = VersionControlStamper.get_version_number_from_file(
         vmn_ctx.vcs.version_file_path
     )
 
     if vmn_ctx.vcs.override_version:
         initial_version = vmn_ctx.vcs.override_version
 
+    is_release = vmn_ctx.vcs.ver_infos_from_repo[vmn_ctx.vcs.selected_tag]["ver_info"]["stamping"]["app"][
+                     "prerelease"] == "release"
+    if vmn_ctx.vcs.optional_release_mode and is_release:
+        verstr = vmn_ctx.vcs.advance_version(initial_version, vmn_ctx.vcs.optional_release_mode, globally=False)
+        tag_name_prefix = f'{vmn_ctx.vcs.name.replace("/", "-")}_{verstr}*'
+        tag = vmn_ctx.vcs.backend.get_latest_available_tag(tag_name_prefix)
+        if tag is not None and len(tag) < len(tag_name_prefix):
+            tag = None
+
+        if not tag:
+            vmn_ctx.vcs.release_mode = vmn_ctx.vcs.optional_release_mode
+        else:
+            props = stamp_utils.VMNBackend.deserialize_vmn_tag_name(tag)
+
+            (_, temp_ver_infos_from_repo) = vmn_ctx.vcs.get_version_info_from_verstr(
+                f"{props['version']}-{props['prerelease']}")
+
+            vmn_ctx.vcs.ver_infos_from_repo[vmn_ctx.vcs.selected_tag]["ver_info"]["stamping"]["app"]["_version"] = \
+                temp_ver_infos_from_repo[tag]["ver_info"]["stamping"]["app"]["_version"]
+            vmn_ctx.vcs.ver_infos_from_repo[vmn_ctx.vcs.selected_tag]["ver_info"]["stamping"]["app"]["prerelease"] = \
+                temp_ver_infos_from_repo[tag]["ver_info"]["stamping"]["app"]["prerelease"]
+            vmn_ctx.vcs.ver_infos_from_repo[vmn_ctx.vcs.selected_tag]["ver_info"]["stamping"]["app"][
+                "prerelease_count"] = \
+                temp_ver_infos_from_repo[tag]["ver_info"]["stamping"]["app"]["prerelease_count"]
+            vmn_ctx.vcs.ver_infos_from_repo[vmn_ctx.vcs.selected_tag]["ver_info"]["stamping"]["app"]["release_mode"] = \
+                temp_ver_infos_from_repo[tag]["ver_info"]["stamping"]["app"]["release_mode"]
+
+            initial_version = verstr
+            if prerelease == "release":
+                prerelease = temp_ver_infos_from_repo[tag]["ver_info"]["stamping"]["app"]["prerelease"]
+                prerelease_count = temp_ver_infos_from_repo[tag]["ver_info"]["stamping"]["app"]["prerelease_count"]
+
+    if vmn_ctx.vcs.tracked and vmn_ctx.vcs.release_mode is None:
+        vmn_ctx.vcs.current_version_info["stamping"]["app"][
+            "release_mode"
+        ] = vmn_ctx.vcs.ver_infos_from_repo[vmn_ctx.vcs.selected_tag]["ver_info"][
+            "stamping"
+        ][
+            "app"
+        ][
+            "release_mode"
+        ]
+
     try:
         version = _stamp_version(
             vmn_ctx.vcs,
             vmn_ctx.args.pull,
             vmn_ctx.args.check_vmn_version,
             initial_version,
             prerelease,
@@ -2991,14 +3026,22 @@
         "--release-mode",
         choices=["major", "minor", "patch", "hotfix", "micro"],
         default=None,
         help="major / minor / patch / hotfix",
         metavar="",
     )
     pstamp.add_argument(
+        "--orm",
+        "--optional-release-mode",
+        choices=["major", "minor", "patch", "hotfix"],
+        default=None,
+        help="major / minor / patch / hotfix",
+        metavar="",
+    )
+    pstamp.add_argument(
         "--pr",
         "--prerelease",
         default=None,
         help="Prerelease version. Can be anything really until you decide "
         "to release the version",
     )
     pstamp.add_argument("--pull", dest="pull", action="store_true")
```

## Comparing `vmn-0.8.1.dist-info/LICENSE.txt` & `vmn-0.8.2rc1.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `vmn-0.8.1.dist-info/RECORD` & `vmn-0.8.2rc1.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 version_stamp/__init__.py,sha256=p_9bnBNpi1jHdKDsmBM7tN2Da3N-QOYEe8s09k9NIrk,152
 version_stamp/stamp_utils.py,sha256=aQupNHxBbWzjJjyFvIze6utVhFgqzD5w_Gb5RjPtMRM,53098
-version_stamp/version.py,sha256=3EFCQXwdLyvdXErZzp_92qEBuhJNHWYFKNxZ0SpHrFM,50
-version_stamp/vmn.py,sha256=Kxt4EkohFxuW8jE9rFHlhjFLWwAEzB8tRY686L-z75o,109439
-vmn-0.8.1.dist-info/LICENSE.txt,sha256=f6flbA23EQX0tZpqCsQCJesFmHb4XNOAOD99egZuaL4,35127
-vmn-0.8.1.dist-info/METADATA,sha256=EG53PFEpW67613AQYPjESMMKIXcB-7HdRJ1ZHj8jihQ,468
-vmn-0.8.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-vmn-0.8.1.dist-info/entry_points.txt,sha256=8JQYxf_iGN3GSYg7ezJs-P8FM3Ss6Hspgg6QcV_s3uk,47
-vmn-0.8.1.dist-info/top_level.txt,sha256=nVR6dU2EinKSe5A4ZJa7NR1aOPNV7QMXvB5Sm-rWbJs,14
-vmn-0.8.1.dist-info/RECORD,,
+version_stamp/version.py,sha256=TG3tt9N6VaM-wPtzpPkyKx8LJqqSP95NRnL04M1dtTE,58
+version_stamp/vmn.py,sha256=FjVwGdRjHO80RaBbB-cFiPhl5xty7hE2VlrME5l3Xio,112040
+vmn-0.8.2rc1.dist-info/LICENSE.txt,sha256=f6flbA23EQX0tZpqCsQCJesFmHb4XNOAOD99egZuaL4,35127
+vmn-0.8.2rc1.dist-info/METADATA,sha256=aiBelMVfrsfATQK0phyOxqNVqXgC9yUcLbAFuNbUHI4,470
+vmn-0.8.2rc1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+vmn-0.8.2rc1.dist-info/entry_points.txt,sha256=8JQYxf_iGN3GSYg7ezJs-P8FM3Ss6Hspgg6QcV_s3uk,47
+vmn-0.8.2rc1.dist-info/top_level.txt,sha256=nVR6dU2EinKSe5A4ZJa7NR1aOPNV7QMXvB5Sm-rWbJs,14
+vmn-0.8.2rc1.dist-info/RECORD,,
```

