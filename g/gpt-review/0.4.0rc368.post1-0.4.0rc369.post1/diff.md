# Comparing `tmp/gpt-review-0.4.0rc368.post1.tar.gz` & `tmp/gpt-review-0.4.0rc369.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt-review-0.4.0rc368.post1.tar", last modified: Wed May  3 23:02:42 2023, max compression
+gzip compressed data, was "gpt-review-0.4.0rc369.post1.tar", last modified: Wed May  3 23:17:07 2023, max compression
```

## Comparing `gpt-review-0.4.0rc368.post1.tar` & `gpt-review-0.4.0rc369.post1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0      336 2023-05-03 23:02:34.148043 gpt-review-0.4.0rc368.post1/.devcontainer/Dockerfile
--rw-r--r--   0        0        0     1595 2023-05-03 23:02:34.152043 gpt-review-0.4.0rc368.post1/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0     1445 2023-05-03 23:02:34.152043 gpt-review-0.4.0rc368.post1/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0        0        0      611 2023-05-03 23:02:34.152043 gpt-review-0.4.0rc368.post1/.github/dependabot.yml
--rw-r--r--   0        0        0      697 2023-05-03 23:02:34.152043 gpt-review-0.4.0rc368.post1/.github/pull_request_template.md
--rw-r--r--   0        0        0     1336 2023-05-03 23:02:34.152043 gpt-review-0.4.0rc368.post1/.github/workflows/codeql.yml
--rw-r--r--   0        0        0      885 2023-05-03 23:02:34.152043 gpt-review-0.4.0rc368.post1/.github/workflows/dependency-review.yml
--rw-r--r--   0        0        0     1818 2023-05-03 23:02:34.152043 gpt-review-0.4.0rc368.post1/.github/workflows/on-push-create-draft-release.yml
--rw-r--r--   0        0        0     4335 2023-05-03 23:02:34.152043 gpt-review-0.4.0rc368.post1/.github/workflows/python.yml
--rw-r--r--   0        0        0      314 2023-05-03 23:02:34.152043 gpt-review-0.4.0rc368.post1/.github/workflows/semantic-pr-check.yml
--rw-r--r--   0        0        0     1341 2023-05-03 23:02:34.152043 gpt-review-0.4.0rc368.post1/.github/workflows/test-action.yml
--rw-r--r--   0        0        0     1808 2023-05-03 23:02:34.152043 gpt-review-0.4.0rc368.post1/.gitignore
--rw-r--r--   0        0        0      158 2023-05-03 23:02:34.152043 gpt-review-0.4.0rc368.post1/.pypirc
--rw-r--r--   0        0        0     1125 2023-05-03 23:02:34.152043 gpt-review-0.4.0rc368.post1/.vscode/settings.json
--rw-r--r--   0        0        0     1070 2023-05-03 23:02:34.152043 gpt-review-0.4.0rc368.post1/LICENSE
--rw-r--r--   0        0        0     3017 2023-05-03 23:02:34.152043 gpt-review-0.4.0rc368.post1/README.md
--rw-r--r--   0        0        0     4920 2023-05-03 23:02:34.152043 gpt-review-0.4.0rc368.post1/action.yml
--rw-r--r--   0        0        0     8252 2023-05-03 23:02:34.152043 gpt-review-0.4.0rc368.post1/pyproject.toml
--rw-r--r--   0        0        0      366 2023-05-03 23:02:42.204349 gpt-review-0.4.0rc368.post1/src/gpt_review/__init__.py
--rw-r--r--   0        0        0    11455 2023-05-03 23:02:34.152043 gpt-review-0.4.0rc368.post1/src/gpt_review/_ask.py
--rw-r--r--   0        0        0      394 2023-05-03 23:02:34.152043 gpt-review-0.4.0rc368.post1/src/gpt_review/_command.py
--rw-r--r--   0        0        0     1924 2023-05-03 23:02:34.152043 gpt-review-0.4.0rc368.post1/src/gpt_review/_git.py
--rw-r--r--   0        0        0     5738 2023-05-03 23:02:34.152043 gpt-review-0.4.0rc368.post1/src/gpt_review/_github.py
--rw-r--r--   0        0        0     1402 2023-05-03 23:02:34.152043 gpt-review-0.4.0rc368.post1/src/gpt_review/_gpt_cli.py
--rw-r--r--   0        0        0      788 2023-05-03 23:02:34.152043 gpt-review-0.4.0rc368.post1/src/gpt_review/_repository.py
--rw-r--r--   0        0        0     6730 2023-05-03 23:02:34.152043 gpt-review-0.4.0rc368.post1/src/gpt_review/_review.py
--rw-r--r--   0        0        0      464 2023-05-03 23:02:34.152043 gpt-review-0.4.0rc368.post1/src/gpt_review/constants.py
--rw-r--r--   0        0        0      488 2023-05-03 23:02:34.152043 gpt-review-0.4.0rc368.post1/src/gpt_review/main.py
--rw-r--r--   0        0        0     2566 2023-05-03 23:02:34.152043 gpt-review-0.4.0rc368.post1/tests/conftest.py
--rw-r--r--   0        0        0      639 2023-05-03 23:02:34.152043 gpt-review-0.4.0rc368.post1/tests/mock.diff
--rw-r--r--   0        0        0      462 2023-05-03 23:02:34.152043 gpt-review-0.4.0rc368.post1/tests/test_git.py
--rw-r--r--   0        0        0     1363 2023-05-03 23:02:34.152043 gpt-review-0.4.0rc368.post1/tests/test_github.py
--rw-r--r--   0        0        0     5987 2023-05-03 23:02:34.152043 gpt-review-0.4.0rc368.post1/tests/test_gpt_cli.py
--rw-r--r--   0        0        0      420 2023-05-03 23:02:34.152043 gpt-review-0.4.0rc368.post1/tests/test_review.py
--rw-r--r--   0        0        0     5076 1970-01-01 00:00:00.000000 gpt-review-0.4.0rc368.post1/PKG-INFO
+-rw-r--r--   0        0        0      336 2023-05-03 23:16:59.054087 gpt-review-0.4.0rc369.post1/.devcontainer/Dockerfile
+-rw-r--r--   0        0        0     1595 2023-05-03 23:16:59.054087 gpt-review-0.4.0rc369.post1/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0     1445 2023-05-03 23:16:59.054087 gpt-review-0.4.0rc369.post1/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0        0        0      611 2023-05-03 23:16:59.054087 gpt-review-0.4.0rc369.post1/.github/dependabot.yml
+-rw-r--r--   0        0        0      697 2023-05-03 23:16:59.054087 gpt-review-0.4.0rc369.post1/.github/pull_request_template.md
+-rw-r--r--   0        0        0     1336 2023-05-03 23:16:59.054087 gpt-review-0.4.0rc369.post1/.github/workflows/codeql.yml
+-rw-r--r--   0        0        0      885 2023-05-03 23:16:59.054087 gpt-review-0.4.0rc369.post1/.github/workflows/dependency-review.yml
+-rw-r--r--   0        0        0     2098 2023-05-03 23:16:59.054087 gpt-review-0.4.0rc369.post1/.github/workflows/on-push-create-draft-release.yml
+-rw-r--r--   0        0        0     4335 2023-05-03 23:16:59.054087 gpt-review-0.4.0rc369.post1/.github/workflows/python.yml
+-rw-r--r--   0        0        0      314 2023-05-03 23:16:59.054087 gpt-review-0.4.0rc369.post1/.github/workflows/semantic-pr-check.yml
+-rw-r--r--   0        0        0     1341 2023-05-03 23:16:59.054087 gpt-review-0.4.0rc369.post1/.github/workflows/test-action.yml
+-rw-r--r--   0        0        0     1808 2023-05-03 23:16:59.054087 gpt-review-0.4.0rc369.post1/.gitignore
+-rw-r--r--   0        0        0      158 2023-05-03 23:16:59.058087 gpt-review-0.4.0rc369.post1/.pypirc
+-rw-r--r--   0        0        0     1125 2023-05-03 23:16:59.058087 gpt-review-0.4.0rc369.post1/.vscode/settings.json
+-rw-r--r--   0        0        0     1070 2023-05-03 23:16:59.058087 gpt-review-0.4.0rc369.post1/LICENSE
+-rw-r--r--   0        0        0     3017 2023-05-03 23:16:59.058087 gpt-review-0.4.0rc369.post1/README.md
+-rw-r--r--   0        0        0     4920 2023-05-03 23:16:59.058087 gpt-review-0.4.0rc369.post1/action.yml
+-rw-r--r--   0        0        0     8252 2023-05-03 23:16:59.058087 gpt-review-0.4.0rc369.post1/pyproject.toml
+-rw-r--r--   0        0        0      366 2023-05-03 23:17:07.070705 gpt-review-0.4.0rc369.post1/src/gpt_review/__init__.py
+-rw-r--r--   0        0        0    11455 2023-05-03 23:16:59.058087 gpt-review-0.4.0rc369.post1/src/gpt_review/_ask.py
+-rw-r--r--   0        0        0      394 2023-05-03 23:16:59.058087 gpt-review-0.4.0rc369.post1/src/gpt_review/_command.py
+-rw-r--r--   0        0        0     1924 2023-05-03 23:16:59.058087 gpt-review-0.4.0rc369.post1/src/gpt_review/_git.py
+-rw-r--r--   0        0        0     5738 2023-05-03 23:16:59.058087 gpt-review-0.4.0rc369.post1/src/gpt_review/_github.py
+-rw-r--r--   0        0        0     1402 2023-05-03 23:16:59.058087 gpt-review-0.4.0rc369.post1/src/gpt_review/_gpt_cli.py
+-rw-r--r--   0        0        0      788 2023-05-03 23:16:59.058087 gpt-review-0.4.0rc369.post1/src/gpt_review/_repository.py
+-rw-r--r--   0        0        0     6730 2023-05-03 23:16:59.058087 gpt-review-0.4.0rc369.post1/src/gpt_review/_review.py
+-rw-r--r--   0        0        0      464 2023-05-03 23:16:59.058087 gpt-review-0.4.0rc369.post1/src/gpt_review/constants.py
+-rw-r--r--   0        0        0      488 2023-05-03 23:16:59.058087 gpt-review-0.4.0rc369.post1/src/gpt_review/main.py
+-rw-r--r--   0        0        0     2566 2023-05-03 23:16:59.058087 gpt-review-0.4.0rc369.post1/tests/conftest.py
+-rw-r--r--   0        0        0      639 2023-05-03 23:16:59.058087 gpt-review-0.4.0rc369.post1/tests/mock.diff
+-rw-r--r--   0        0        0      462 2023-05-03 23:16:59.058087 gpt-review-0.4.0rc369.post1/tests/test_git.py
+-rw-r--r--   0        0        0     1363 2023-05-03 23:16:59.058087 gpt-review-0.4.0rc369.post1/tests/test_github.py
+-rw-r--r--   0        0        0     5987 2023-05-03 23:16:59.058087 gpt-review-0.4.0rc369.post1/tests/test_gpt_cli.py
+-rw-r--r--   0        0        0      420 2023-05-03 23:16:59.058087 gpt-review-0.4.0rc369.post1/tests/test_review.py
+-rw-r--r--   0        0        0     5076 1970-01-01 00:00:00.000000 gpt-review-0.4.0rc369.post1/PKG-INFO
```

### Comparing `gpt-review-0.4.0rc368.post1/.devcontainer/devcontainer.json` & `gpt-review-0.4.0rc369.post1/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `gpt-review-0.4.0rc368.post1/.github/ISSUE_TEMPLATE/bug_report.yml` & `gpt-review-0.4.0rc369.post1/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.4.0rc368.post1/.github/dependabot.yml` & `gpt-review-0.4.0rc369.post1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.4.0rc368.post1/.github/pull_request_template.md` & `gpt-review-0.4.0rc369.post1/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `gpt-review-0.4.0rc368.post1/.github/workflows/codeql.yml` & `gpt-review-0.4.0rc369.post1/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.4.0rc368.post1/.github/workflows/dependency-review.yml` & `gpt-review-0.4.0rc369.post1/.github/workflows/dependency-review.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.4.0rc368.post1/.github/workflows/on-push-create-draft-release.yml` & `gpt-review-0.4.0rc369.post1/.github/workflows/on-push-create-draft-release.yml`

 * *Files 8% similar despite different names*

```diff
@@ -39,14 +39,24 @@
         if: steps.tag_version.outputs.release_type
         with:
           message: Update Version to ${{ steps.tag_version.outputs.new_version }} [no ci]
           committer_name: GitHub Actions
           committer_email: actions@github.com
           add: "src/gpt_review/__init__.py"
 
+      - name: Set Configurations
+        if: steps.tag_version.outputs.release_type
+        shell: bash
+        env:
+          TITLE: ${{ steps.tag_version.outputs.new_tag }}
+        run: |
+          hub release delete \
+            --include-drafts
+            latest || exit 0
+
       - uses: dciborow/action-github-releases@v1.0.1
         if: steps.tag_version.outputs.release_type
         with:
           repo_token: "${{ secrets.GITHUB_TOKEN }}"
           automatic_release_tag: "latest"
           draft: true
           title: ${{ steps.tag_version.outputs.new_tag }}
```

### Comparing `gpt-review-0.4.0rc368.post1/.github/workflows/python.yml` & `gpt-review-0.4.0rc369.post1/.github/workflows/python.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.4.0rc368.post1/.github/workflows/test-action.yml` & `gpt-review-0.4.0rc369.post1/.github/workflows/test-action.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.4.0rc368.post1/.gitignore` & `gpt-review-0.4.0rc369.post1/.gitignore`

 * *Files identical despite different names*

### Comparing `gpt-review-0.4.0rc368.post1/.vscode/settings.json` & `gpt-review-0.4.0rc369.post1/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `gpt-review-0.4.0rc368.post1/LICENSE` & `gpt-review-0.4.0rc369.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt-review-0.4.0rc368.post1/README.md` & `gpt-review-0.4.0rc369.post1/README.md`

 * *Files identical despite different names*

### Comparing `gpt-review-0.4.0rc368.post1/action.yml` & `gpt-review-0.4.0rc369.post1/action.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.4.0rc368.post1/pyproject.toml` & `gpt-review-0.4.0rc369.post1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.4.0rc368.post1/src/gpt_review/_ask.py` & `gpt-review-0.4.0rc369.post1/src/gpt_review/_ask.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.4.0rc368.post1/src/gpt_review/_git.py` & `gpt-review-0.4.0rc369.post1/src/gpt_review/_git.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.4.0rc368.post1/src/gpt_review/_github.py` & `gpt-review-0.4.0rc369.post1/src/gpt_review/_github.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.4.0rc368.post1/src/gpt_review/_gpt_cli.py` & `gpt-review-0.4.0rc369.post1/src/gpt_review/_gpt_cli.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.4.0rc368.post1/src/gpt_review/_repository.py` & `gpt-review-0.4.0rc369.post1/src/gpt_review/_repository.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.4.0rc368.post1/src/gpt_review/_review.py` & `gpt-review-0.4.0rc369.post1/src/gpt_review/_review.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.4.0rc368.post1/tests/conftest.py` & `gpt-review-0.4.0rc369.post1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.4.0rc368.post1/tests/mock.diff` & `gpt-review-0.4.0rc369.post1/tests/mock.diff`

 * *Files identical despite different names*

### Comparing `gpt-review-0.4.0rc368.post1/tests/test_github.py` & `gpt-review-0.4.0rc369.post1/tests/test_github.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.4.0rc368.post1/tests/test_gpt_cli.py` & `gpt-review-0.4.0rc369.post1/tests/test_gpt_cli.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.4.0rc368.post1/PKG-INFO` & `gpt-review-0.4.0rc369.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-review
-Version: 0.4.0rc368.post1
+Version: 0.4.0rc369.post1
 Summary: Python Project for reviewing GitHub PRs with Open AI and Chat-GPT.
 Author-email: Daniel Ciborowski <dciborow@microsoft.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: gpt-review Version: 0.4.0rc368.post1 Summary:
+Metadata-Version: 2.1 Name: gpt-review Version: 0.4.0rc369.post1 Summary:
 Python Project for reviewing GitHub PRs with Open AI and Chat-GPT. Author-
 email: Daniel Ciborowski
 microsoft.com> Requires-Python: >=3.7 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 :: Only Classifier: Programming Language ::
 Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
```

