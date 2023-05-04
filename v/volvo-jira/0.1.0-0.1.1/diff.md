# Comparing `tmp/volvo-jira-0.1.0.tar.gz` & `tmp/volvo-jira-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "volvo-jira-0.1.0.tar", last modified: Wed May  3 09:59:39 2023, max compression
+gzip compressed data, was "volvo-jira-0.1.1.tar", last modified: Thu May  4 12:22:03 2023, max compression
```

## Comparing `volvo-jira-0.1.0.tar` & `volvo-jira-0.1.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 PROBERT4   (502) staff       (20)        0 2023-05-03 09:59:39.172526 volvo-jira-0.1.0/
--rw-r--r--   0 PROBERT4   (502) staff       (20)     1075 2023-04-18 07:10:23.000000 volvo-jira-0.1.0/LICENSE
--rw-r--r--   0 PROBERT4   (502) staff       (20)      947 2023-05-03 09:59:39.172676 volvo-jira-0.1.0/PKG-INFO
--rw-r--r--   0 PROBERT4   (502) staff       (20)      280 2023-04-28 16:17:04.000000 volvo-jira-0.1.0/README.md
--rw-r--r--   0 PROBERT4   (502) staff       (20)      457 2023-05-02 15:16:53.000000 volvo-jira-0.1.0/pyproject.toml
--rw-r--r--   0 PROBERT4   (502) staff       (20)     1068 2023-05-03 09:59:39.174283 volvo-jira-0.1.0/setup.cfg
--rw-r--r--   0 PROBERT4   (502) staff       (20)       69 2023-04-18 07:13:11.000000 volvo-jira-0.1.0/setup.py
-drwxr-xr-x   0 PROBERT4   (502) staff       (20)        0 2023-05-03 09:59:39.135153 volvo-jira-0.1.0/src/
-drwxr-xr-x   0 PROBERT4   (502) staff       (20)        0 2023-05-03 09:59:39.155044 volvo-jira-0.1.0/src/vira/
--rw-r--r--   0 PROBERT4   (502) staff       (20)      149 2023-04-28 15:58:32.000000 volvo-jira-0.1.0/src/vira/__init__.py
--rw-r--r--   0 PROBERT4   (502) staff       (20)        0 2023-04-18 07:34:47.000000 volvo-jira-0.1.0/src/vira/py.typed
--rw-r--r--   0 PROBERT4   (502) staff       (20)     2326 2023-04-28 15:53:36.000000 volvo-jira-0.1.0/src/vira/vira_add_parent.py
--rw-r--r--   0 PROBERT4   (502) staff       (20)     1178 2023-04-27 16:12:57.000000 volvo-jira-0.1.0/src/vira/vira_base.py
--rw-r--r--   0 PROBERT4   (502) staff       (20)     3316 2023-04-28 15:53:36.000000 volvo-jira-0.1.0/src/vira/vira_copy.py
--rw-r--r--   0 PROBERT4   (502) staff       (20)     6700 2023-04-28 15:53:36.000000 volvo-jira-0.1.0/src/vira/vira_deep_copy.py
--rw-r--r--   0 PROBERT4   (502) staff       (20)      560 2023-04-27 16:11:11.000000 volvo-jira-0.1.0/src/vira/vira_error.py
--rw-r--r--   0 PROBERT4   (502) staff       (20)     3165 2023-04-27 16:10:30.000000 volvo-jira-0.1.0/src/vira/vira_issue.py
--rw-r--r--   0 PROBERT4   (502) staff       (20)     1483 2023-04-28 15:14:01.000000 volvo-jira-0.1.0/src/vira/vira_script_utils.py
--rw-r--r--   0 PROBERT4   (502) staff       (20)    18736 2023-04-28 10:36:43.000000 volvo-jira-0.1.0/src/vira/vira_vira.py
-drwxr-xr-x   0 PROBERT4   (502) staff       (20)        0 2023-05-03 09:59:39.166864 volvo-jira-0.1.0/src/volvo_jira.egg-info/
--rw-r--r--   0 PROBERT4   (502) staff       (20)      947 2023-05-03 09:59:39.000000 volvo-jira-0.1.0/src/volvo_jira.egg-info/PKG-INFO
--rw-r--r--   0 PROBERT4   (502) staff       (20)      643 2023-05-03 09:59:39.000000 volvo-jira-0.1.0/src/volvo_jira.egg-info/SOURCES.txt
--rw-r--r--   0 PROBERT4   (502) staff       (20)        1 2023-05-03 09:59:39.000000 volvo-jira-0.1.0/src/volvo_jira.egg-info/dependency_links.txt
--rw-r--r--   0 PROBERT4   (502) staff       (20)      136 2023-05-03 09:59:39.000000 volvo-jira-0.1.0/src/volvo_jira.egg-info/entry_points.txt
--rw-r--r--   0 PROBERT4   (502) staff       (20)        1 2023-05-03 09:58:23.000000 volvo-jira-0.1.0/src/volvo_jira.egg-info/not-zip-safe
--rw-r--r--   0 PROBERT4   (502) staff       (20)       81 2023-05-03 09:59:39.000000 volvo-jira-0.1.0/src/volvo_jira.egg-info/requires.txt
--rw-r--r--   0 PROBERT4   (502) staff       (20)        5 2023-05-03 09:59:39.000000 volvo-jira-0.1.0/src/volvo_jira.egg-info/top_level.txt
-drwxr-xr-x   0 PROBERT4   (502) staff       (20)        0 2023-05-03 09:59:39.171909 volvo-jira-0.1.0/tests/
--rw-r--r--   0 PROBERT4   (502) staff       (20)     2683 2023-04-28 09:40:42.000000 volvo-jira-0.1.0/tests/test_connection.py
--rw-r--r--   0 PROBERT4   (502) staff       (20)     5122 2023-05-03 06:40:42.000000 volvo-jira-0.1.0/tests/test_issue.py
--rw-r--r--   0 PROBERT4   (502) staff       (20)      317 2023-04-18 11:44:54.000000 volvo-jira-0.1.0/tests/test_logging.py
--rw-r--r--   0 PROBERT4   (502) staff       (20)      826 2023-05-03 06:42:44.000000 volvo-jira-0.1.0/tests/test_scripts.py
+drwxr-xr-x   0 PROBERT4   (502) staff       (20)        0 2023-05-04 12:22:03.577893 volvo-jira-0.1.1/
+-rw-r--r--   0 PROBERT4   (502) staff       (20)     1075 2023-04-18 07:10:23.000000 volvo-jira-0.1.1/LICENSE
+-rw-r--r--   0 PROBERT4   (502) staff       (20)      947 2023-05-04 12:22:03.578033 volvo-jira-0.1.1/PKG-INFO
+-rw-r--r--   0 PROBERT4   (502) staff       (20)      280 2023-04-28 16:17:04.000000 volvo-jira-0.1.1/README.md
+-rw-r--r--   0 PROBERT4   (502) staff       (20)      457 2023-05-02 15:16:53.000000 volvo-jira-0.1.1/pyproject.toml
+-rw-r--r--   0 PROBERT4   (502) staff       (20)     1068 2023-05-04 12:22:03.584249 volvo-jira-0.1.1/setup.cfg
+-rw-r--r--   0 PROBERT4   (502) staff       (20)       69 2023-04-18 07:13:11.000000 volvo-jira-0.1.1/setup.py
+drwxr-xr-x   0 PROBERT4   (502) staff       (20)        0 2023-05-04 12:22:03.553365 volvo-jira-0.1.1/src/
+drwxr-xr-x   0 PROBERT4   (502) staff       (20)        0 2023-05-04 12:22:03.566498 volvo-jira-0.1.1/src/vira/
+-rw-r--r--   0 PROBERT4   (502) staff       (20)      149 2023-04-28 15:58:32.000000 volvo-jira-0.1.1/src/vira/__init__.py
+-rw-r--r--   0 PROBERT4   (502) staff       (20)        0 2023-04-18 07:34:47.000000 volvo-jira-0.1.1/src/vira/py.typed
+-rw-r--r--   0 PROBERT4   (502) staff       (20)     2421 2023-05-03 11:00:44.000000 volvo-jira-0.1.1/src/vira/vira_add_parent.py
+-rw-r--r--   0 PROBERT4   (502) staff       (20)     1178 2023-04-27 16:12:57.000000 volvo-jira-0.1.1/src/vira/vira_base.py
+-rw-r--r--   0 PROBERT4   (502) staff       (20)     3325 2023-05-03 10:42:14.000000 volvo-jira-0.1.1/src/vira/vira_copy.py
+-rw-r--r--   0 PROBERT4   (502) staff       (20)     6709 2023-05-03 10:48:47.000000 volvo-jira-0.1.1/src/vira/vira_deep_copy.py
+-rw-r--r--   0 PROBERT4   (502) staff       (20)      559 2023-05-03 14:47:20.000000 volvo-jira-0.1.1/src/vira/vira_error.py
+-rw-r--r--   0 PROBERT4   (502) staff       (20)     3173 2023-05-03 15:16:54.000000 volvo-jira-0.1.1/src/vira/vira_issue.py
+-rw-r--r--   0 PROBERT4   (502) staff       (20)     1483 2023-04-28 15:14:01.000000 volvo-jira-0.1.1/src/vira/vira_script_utils.py
+-rw-r--r--   0 PROBERT4   (502) staff       (20)    18705 2023-05-03 17:33:47.000000 volvo-jira-0.1.1/src/vira/vira_vira.py
+drwxr-xr-x   0 PROBERT4   (502) staff       (20)        0 2023-05-04 12:22:03.572608 volvo-jira-0.1.1/src/volvo_jira.egg-info/
+-rw-r--r--   0 PROBERT4   (502) staff       (20)      947 2023-05-04 12:22:03.000000 volvo-jira-0.1.1/src/volvo_jira.egg-info/PKG-INFO
+-rw-r--r--   0 PROBERT4   (502) staff       (20)      643 2023-05-04 12:22:03.000000 volvo-jira-0.1.1/src/volvo_jira.egg-info/SOURCES.txt
+-rw-r--r--   0 PROBERT4   (502) staff       (20)        1 2023-05-04 12:22:03.000000 volvo-jira-0.1.1/src/volvo_jira.egg-info/dependency_links.txt
+-rw-r--r--   0 PROBERT4   (502) staff       (20)      136 2023-05-04 12:22:03.000000 volvo-jira-0.1.1/src/volvo_jira.egg-info/entry_points.txt
+-rw-r--r--   0 PROBERT4   (502) staff       (20)        1 2023-05-03 17:00:24.000000 volvo-jira-0.1.1/src/volvo_jira.egg-info/not-zip-safe
+-rw-r--r--   0 PROBERT4   (502) staff       (20)       81 2023-05-04 12:22:03.000000 volvo-jira-0.1.1/src/volvo_jira.egg-info/requires.txt
+-rw-r--r--   0 PROBERT4   (502) staff       (20)        5 2023-05-04 12:22:03.000000 volvo-jira-0.1.1/src/volvo_jira.egg-info/top_level.txt
+drwxr-xr-x   0 PROBERT4   (502) staff       (20)        0 2023-05-04 12:22:03.577002 volvo-jira-0.1.1/tests/
+-rw-r--r--   0 PROBERT4   (502) staff       (20)     2683 2023-04-28 09:40:42.000000 volvo-jira-0.1.1/tests/test_connection.py
+-rw-r--r--   0 PROBERT4   (502) staff       (20)     4996 2023-05-03 16:08:47.000000 volvo-jira-0.1.1/tests/test_issue.py
+-rw-r--r--   0 PROBERT4   (502) staff       (20)      317 2023-04-18 11:44:54.000000 volvo-jira-0.1.1/tests/test_logging.py
+-rw-r--r--   0 PROBERT4   (502) staff       (20)     1526 2023-05-03 11:06:38.000000 volvo-jira-0.1.1/tests/test_scripts.py
```

### Comparing `volvo-jira-0.1.0/LICENSE` & `volvo-jira-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `volvo-jira-0.1.0/PKG-INFO` & `volvo-jira-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: volvo-jira
-Version: 0.1.0
+Version: 0.1.1
 Summary: Volvo JIRA (VIRA) package and helper scripts. Contains scripts for deep copy, change parent and more
 Author: Per-Ola Robertsson
 License: MIT
 Platform: unix
 Platform: linux
 Platform: osx
 Platform: cygwin
```

### Comparing `volvo-jira-0.1.0/setup.cfg` & `volvo-jira-0.1.1/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = volvo-jira
-version = 0.1.0
+version = 0.1.1
 description = Volvo JIRA (VIRA) package and helper scripts. Contains scripts for deep copy, change parent and more
 long_description = file: README.md
 long_description_content_type = text/markdown; charset=UTF-8; variant=GFM
 author = Per-Ola Robertsson
 license = MIT
 license_files = LICENSE
 platforms = unix, linux, osx, cygwin, win32
```

### Comparing `volvo-jira-0.1.0/src/vira/vira_add_parent.py` & `volvo-jira-0.1.1/src/vira/vira_add_parent.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 # Release notes
 SCRIPT_RELEASE_NOTES = [
     [SCRIPT_VERSION, "2023-03-20", "Initial alpha release for feedback"],
 ]
 
 
-def main():
+def main() -> int:
     parser = argparse.ArgumentParser(
         description=f"{SCRIPT_NAME} {SCRIPT_VERSION}. Add or moves a VIRA issue to annother parent. Created by {SCRIPT_AURTOUR}.\nRelease notes:\n{SCRIPT_RELEASE_NOTES}"
     )
 
     parser.add_argument("issue", help="The issue")
     parser.add_argument(
         "parent",
@@ -32,18 +32,21 @@
     # Parse the arguments
     args = parser.parse_args()
 
     vira = VIRA(args.vira_url)
 
     # Connect to Jira
     try:
-        vira.connect(user=args.user, password=args.password)
+        if args.token is not None:
+            vira.connect_with_token(token=args.token)
+        else:
+            vira.connect(user=args.user, password=args.password)
     except VIRAError as e:
         print(
-            f"Could not connect to VIRA {args.vira_url}'. Aborting. Details:\n{e.status_code} {e.message}\n{e.jira_error.response.content}"
+            f"Could not connect to VIRA {args.vira_url}'. Aborting. Details:\n{e.status_code} {e.message}"
         )
         exit(1)
 
     try:
         issue = vira.get_issue(args.issue)
     except VIRAError as e:
         print(
@@ -71,10 +74,12 @@
     print(f"Will make {issue.short_str} child of {parent_issue.short_str}")
 
     if not args.force:
         vira_script_utils.ask_for_confirmation()
 
     vira.add_child_issue_to_parent(parent_issue=parent_issue, child_issue=issue)
 
+    return 0
+
 
 if __name__ == "__main__":
     main()
```

### Comparing `volvo-jira-0.1.0/src/vira/vira_base.py` & `volvo-jira-0.1.1/src/vira/vira_base.py`

 * *Files identical despite different names*

### Comparing `volvo-jira-0.1.0/src/vira/vira_copy.py` & `volvo-jira-0.1.1/src/vira/vira_copy.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 # Release notes
 SCRIPT_RELEASE_NOTES = [
     [SCRIPT_VERSION, "2023-03-20", "Initla alpha release for feedback"],
 ]
 
 
-def main():
+def main() -> int:
     parser = argparse.ArgumentParser(
         description=f"{SCRIPT_NAME} {SCRIPT_VERSION}. Deep Copies a VIRA issue. Created by {SCRIPT_AURTOUR}.\nRelease notes:\n{SCRIPT_RELEASE_NOTES}"
     )
 
     parser.add_argument("src_issue", help="The issue to copy from")
     parser.add_argument(
         "-p",
@@ -93,12 +93,12 @@
         log_str = f"Created issue {copy_issue.short_str}"
         if parent_issue is not None:
             log_str += f" and made it a child to {parent_issue.short_str}"
         print(log_str)
     else:
         print("No issues created")
 
-    return
+    return 0
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `volvo-jira-0.1.0/src/vira/vira_deep_copy.py` & `volvo-jira-0.1.1/src/vira/vira_deep_copy.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         print(f"{indent_str}{issue.short_str}")
     for child in children:
         print_children(child, indent_str + "  ")
 
     return indent_str[2:]  # Remove 2 spaces
 
 
-def main():
+def main() -> int:
     parser = argparse.ArgumentParser(
         description=f"{SCRIPT_NAME} {SCRIPT_VERSION}. Deep Copies a VIRA issue. Created by {SCRIPT_AUTHOUR}"
     )
 
     parser.add_argument("src_issue", help="The issue to copy from")
     parser.add_argument(
         "-p",
@@ -172,12 +172,12 @@
 
     print("Summary:")
     if copy_issue is not None:
         print_children(copy_issue)
     else:
         print("No issues created")
 
-    return
+    return 0
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `volvo-jira-0.1.0/src/vira/vira_error.py` & `volvo-jira-0.1.1/src/vira/vira_error.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from jira import JIRAError
 
-
 class VIRAError(Exception):
     """Exception raised for generic VIRA errors.
 
     Attributes:
         message -- The error message
         status_code -- The error status code. Can be None
         jira_exception -- The underlying JIRA error (JIRAError). Can be None
```

### Comparing `volvo-jira-0.1.0/src/vira/vira_issue.py` & `volvo-jira-0.1.1/src/vira/vira_issue.py`

 * *Files 4% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 
     @property
     def short_str(self):
         if self._jira_issue is None:
             return "<None>"
         return f'{BOLD}{self.fields.issuetype.name}{RESET} {self.key} "{self.fields.summary}"'
 
-    def get_children(self):
+    def get_children(self) -> list:
         """Also gets the subtasks of Capabilities, Features, Stories and Tasks"""
 
         children_issues = []
         if self.is_capability:
             # Get the children issues (Features) of the Capability
             children_issues = self._jira.search_issues(
                 f'issueFunction in linkedIssuesOf("issue={self.key}", "is parent of") ORDER BY Rank'
```

### Comparing `volvo-jira-0.1.0/src/vira/vira_script_utils.py` & `volvo-jira-0.1.1/src/vira/vira_script_utils.py`

 * *Files identical despite different names*

### Comparing `volvo-jira-0.1.0/src/vira/vira_vira.py` & `volvo-jira-0.1.1/src/vira/vira_vira.py`

 * *Files 0% similar despite different names*

```diff
@@ -172,17 +172,17 @@
             ), f"Can only add a feature to a capability. Got parent issue {parent_issue} and child issue {child_issue}"
 
             issue_dict = {
                 # customfield_13801 = Capability Name. Example 'SOLSWEP-1201'
                 "customfield_13801": parent_issue.key,
                 # customfield_16500 = Capability ID. Example '3467866' (.id of SOLSWEP-1201)
                 #            'customfield_16500': parent_issue.id
+                "parent": {"id": parent_issue.id},
             }
             child_issue._jira_issue.update(fields=issue_dict)
-            child_issue._jira_issue.update(fields={"parent": {"id": parent_issue.id}})
         elif child_issue.is_story:
             assert (
                 parent_issue.is_feature
             ), f"Can only add a Story to a Feature. Got parent issue {parent_issue} and child issue {child_issue}"
 
             # PROBERT4: Working for now, but with updated VIRA/JIRA this might stop working.
             # As of January 2022, add_issues_to_epic is not supported for next-gen projects
@@ -311,15 +311,15 @@
         dst_summary = self.replace_strings(src_issue.fields.summary)
 
         if self.dry_run:
             log_str = f'Dry run: Would have copied {src_issue.indent_str}{src_issue.short_str} but changed the summary to "{dst_summary}"'
             if parent_issue is not None:
                 log_str += f" and added it as child to {parent_issue.short_str}"
             g_logger.debug(log_str, extra={"console_only": True})
-            return
+            return None
 
         # TODO(probert4) Check these
         read_only_fields = [
             "lastViewed",
             "creator",
             "customfield_15100",
             "subtasks",
```

### Comparing `volvo-jira-0.1.0/src/volvo_jira.egg-info/PKG-INFO` & `volvo-jira-0.1.1/src/volvo_jira.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: volvo-jira
-Version: 0.1.0
+Version: 0.1.1
 Summary: Volvo JIRA (VIRA) package and helper scripts. Contains scripts for deep copy, change parent and more
 Author: Per-Ola Robertsson
 License: MIT
 Platform: unix
 Platform: linux
 Platform: osx
 Platform: cygwin
```

### Comparing `volvo-jira-0.1.0/src/volvo_jira.egg-info/SOURCES.txt` & `volvo-jira-0.1.1/src/volvo_jira.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `volvo-jira-0.1.0/tests/test_connection.py` & `volvo-jira-0.1.1/tests/test_connection.py`

 * *Files identical despite different names*

### Comparing `volvo-jira-0.1.0/tests/test_issue.py` & `volvo-jira-0.1.1/tests/test_issue.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from vira import VIRA
 import pytest
+import inspect
 from tests.credentials import (
     VIRA_TEST_URL,
     VIRA_TEST_ACCESS_TOKEN,
 )
 
 VIRA_PROJECT_KEY = "ARTCSP"
 
@@ -13,76 +14,70 @@
     vira = VIRA(VIRA_TEST_URL)
     vira.connect_with_token(token=VIRA_TEST_ACCESS_TOKEN)
     vira.set_create_comment("Created by unittest")
     return vira
 
 
 @pytest.fixture
-def src_capability_issue(vira):
+def src_capability_issue(vira, scope="session"):
     # SOLSWEP-802 - Capability: 'PRST gen I: Product Capability "Core System Platform State and Power Management"'
     issue = vira.get_issue("SOLSWEP-802")
     return issue
 
 
 def test_get_issue(vira):
     # def get_issue(self, issue_key : str) -> VIRAIssue
     # ARTCSP-34668 - Feature: Test Feature 2'
     issue = vira.get_issue("ARTCSP-34668")
 
     assert issue.key == "ARTCSP-34668"
     assert issue.fields.summary == "Test Feature 2"
+    assert issue.fields.status.name == "Done"
     assert len(issue.get_children()) == 12  # 12 - 11 Features and 1 Subtask
 
-    # SOLSWEP-802 - Capability: 'PRST gen I: Product Capability "Core System Platform State and Power Management"'
-    # Has Sub-Tasks and Features
-    issue = vira.get_issue("SOLSWEP-802")
-
-    assert issue.key == "SOLSWEP-802"
-    assert (
-        issue.fields.summary
-        == 'PRST gen I: Product Capability "Core System Platform State and Power Management"'
-    )
-    assert len(issue.get_children()) == 8  # 8 - 6 Features and 2 Subtasks
-
 
 def calculate_n_children_recursive(issue, n_children=0):
     children = issue.get_children()
     print(f"{issue}, has {len(children)} children")
     n_children += len(children)
     for child in children:
         n_children = calculate_n_children_recursive(child, n_children)
     return n_children
 
 
-def test_get_children(vira, src_capability_issue):
-    def print_children(issue, indent_str: str):
-        children = issue.get_children()
-        print(f"{indent_str}{issue}, has {len(children)} children")
-        for child in children:
-            print_children(child, indent_str + "  ")
+def print_children(issue, indent_str: str = ""):
+    children = issue.get_children()
+    print(f"{indent_str}{issue}, has {len(children)} children")
+    for child in children:
+        print_children(child, indent_str + "  ")
+    return indent_str[2:]  # Remove 2 spaces
+
+
+def _function_name() -> str:
+    return inspect.stack()[1][3]
 
-        return indent_str[2:]  # Remove 2 spaces
 
+def test_get_children(vira, src_capability_issue):
     children = src_capability_issue.get_children()
-    assert len(children) == 8  # 8 - 6 Features and 2 SubTasks
+    assert len(children) == 3  # 3 - 1 Features and 2 SubTasks
 
-    print_children(src_capability_issue, "")
-    assert calculate_n_children_recursive(src_capability_issue) == 58
+    print_children(src_capability_issue)
+    assert calculate_n_children_recursive(src_capability_issue) == 4
 
 
 def test_create_issue(vira):
     # Some field must be set. Like project, issuetype and Summary. TODO(probert4) Add these as parameters in new create_issue_simple() method? That will also set 'Feature Name'
     fields = {
         "project": {"key": VIRA_PROJECT_KEY},
         "issuetype": "Story",
         "summary": "My own Story summary",
         "description": "My own Story description",
     }
 
-    vira.set_create_comment(f"This issue was created by unit test {__name__}")
+    vira.set_create_comment(f"This issue was created by unit test test_create_issue")
 
     issue = vira.create_issue(fields)
 
     assert issue.fields.project.key == VIRA_PROJECT_KEY
     assert issue.fields.issuetype.name == "Story"
     assert issue.fields.summary == "My own Story summary"
     assert issue.fields.description == "My own Story description"
@@ -91,28 +86,30 @@
     assert issue.fields.status.name == "Open"
 
     assert issue.is_story
 
 
 def test_copy_issue(vira):
     src_issue = vira.get_issue("SOLSWEP-803")
+    vira.set_create_comment(f"This issue was created by unit test test_copy_issue")
+
     cpy_issue = vira.copy_issue(src_issue)
 
     assert cpy_issue.key != src_issue.key
     assert cpy_issue.id != src_issue.id
     assert cpy_issue.short_str != src_issue.short_str
     assert len(cpy_issue.get_children()) == 0
     assert cpy_issue.fields.project.key == src_issue.fields.project.key
     assert cpy_issue.fields.summary == src_issue.fields.summary
     assert cpy_issue.fields.description == src_issue.fields.description
     # TODO add more fileds test, status. Maybe even add a cmp overload to VIRAIssue?
 
 
 def test_deep_copy(vira, src_capability_issue):
-    vira.set_create_comment(f"This issue was created by unit test {__name__}")
+    vira.set_create_comment(f"This issue was created by unit test test_deep_copy")
     # def copy_issue_recursive(self, src_issue: VIRAIssue, *, copy_parent_issue: VIRAIssue = None) -> VIRAIssue:
     cpy_issue = vira.copy_issue_recursive(src_capability_issue)
 
     assert cpy_issue.is_capability
 
     assert cpy_issue.fields.summary == src_capability_issue.fields.summary
     assert cpy_issue.fields.description == src_capability_issue.fields.description
@@ -122,14 +119,17 @@
     assert calculate_n_children_recursive(cpy_issue) == calculate_n_children_recursive(
         src_capability_issue
     )
 
 
 def test_deep_copy_to_parent(vira, src_capability_issue):
     parent_capability_issue = vira.copy_issue_by_key("SOLSWEP-803")
+    vira.set_create_comment(
+        f"This issue was created by unit test test_deep_copy_to_parent"
+    )
     parent_n_children_before = calculate_n_children_recursive(parent_capability_issue)
 
     cpy_issue = vira.copy_issue_recursive(
         src_capability_issue, copy_parent_issue=parent_capability_issue
     )
 
     assert cpy_issue == parent_capability_issue  # should return the parent issue
```

