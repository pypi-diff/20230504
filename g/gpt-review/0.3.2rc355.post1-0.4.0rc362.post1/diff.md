# Comparing `tmp/gpt-review-0.3.2rc355.post1.tar.gz` & `tmp/gpt-review-0.4.0rc362.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt-review-0.3.2rc355.post1.tar", last modified: Wed May  3 21:58:32 2023, max compression
+gzip compressed data, was "gpt-review-0.4.0rc362.post1.tar", last modified: Wed May  3 22:46:40 2023, max compression
```

## Comparing `gpt-review-0.3.2rc355.post1.tar` & `gpt-review-0.4.0rc362.post1.tar`

### file list

```diff
@@ -1,28 +1,35 @@
--rw-r--r--   0        0        0      336 2023-05-03 21:58:23.734940 gpt-review-0.3.2rc355.post1/.devcontainer/Dockerfile
--rw-r--r--   0        0        0     1595 2023-05-03 21:58:23.734940 gpt-review-0.3.2rc355.post1/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0     1445 2023-05-03 21:58:23.734940 gpt-review-0.3.2rc355.post1/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0        0        0      611 2023-05-03 21:58:23.734940 gpt-review-0.3.2rc355.post1/.github/dependabot.yml
--rw-r--r--   0        0        0      697 2023-05-03 21:58:23.734940 gpt-review-0.3.2rc355.post1/.github/pull_request_template.md
--rw-r--r--   0        0        0     1336 2023-05-03 21:58:23.734940 gpt-review-0.3.2rc355.post1/.github/workflows/codeql.yml
--rw-r--r--   0        0        0      885 2023-05-03 21:58:23.734940 gpt-review-0.3.2rc355.post1/.github/workflows/dependency-review.yml
--rw-r--r--   0        0        0     1367 2023-05-03 21:58:23.734940 gpt-review-0.3.2rc355.post1/.github/workflows/on-push-create-draft-release.yml
--rw-r--r--   0        0        0     4251 2023-05-03 21:58:23.734940 gpt-review-0.3.2rc355.post1/.github/workflows/python.yml
--rw-r--r--   0        0        0      314 2023-05-03 21:58:23.734940 gpt-review-0.3.2rc355.post1/.github/workflows/semantic-pr-check.yml
--rw-r--r--   0        0        0      898 2023-05-03 21:58:23.734940 gpt-review-0.3.2rc355.post1/.github/workflows/test-action.yml
--rw-r--r--   0        0        0     1808 2023-05-03 21:58:23.734940 gpt-review-0.3.2rc355.post1/.gitignore
--rw-r--r--   0        0        0      158 2023-05-03 21:58:23.734940 gpt-review-0.3.2rc355.post1/.pypirc
--rw-r--r--   0        0        0     1125 2023-05-03 21:58:23.734940 gpt-review-0.3.2rc355.post1/.vscode/settings.json
--rw-r--r--   0        0        0     1070 2023-05-03 21:58:23.734940 gpt-review-0.3.2rc355.post1/LICENSE
--rw-r--r--   0        0        0     1617 2023-05-03 21:58:23.734940 gpt-review-0.3.2rc355.post1/README.md
--rw-r--r--   0        0        0     5206 2023-05-03 21:58:23.734940 gpt-review-0.3.2rc355.post1/action.yml
--rw-r--r--   0        0        0     8252 2023-05-03 21:58:23.734940 gpt-review-0.3.2rc355.post1/pyproject.toml
--rw-r--r--   0        0        0    18646 2023-05-03 21:58:23.734940 gpt-review-0.3.2rc355.post1/review.py
--rw-r--r--   0        0        0      366 2023-05-03 21:58:31.855047 gpt-review-0.3.2rc355.post1/src/gpt_review/__init__.py
--rw-r--r--   0        0        0    11455 2023-05-03 21:58:23.734940 gpt-review-0.3.2rc355.post1/src/gpt_review/_ask.py
--rw-r--r--   0        0        0      394 2023-05-03 21:58:23.734940 gpt-review-0.3.2rc355.post1/src/gpt_review/_command.py
--rw-r--r--   0        0        0     1312 2023-05-03 21:58:23.734940 gpt-review-0.3.2rc355.post1/src/gpt_review/_gpt_cli.py
--rw-r--r--   0        0        0      464 2023-05-03 21:58:23.734940 gpt-review-0.3.2rc355.post1/src/gpt_review/constants.py
--rw-r--r--   0        0        0      413 2023-05-03 21:58:23.734940 gpt-review-0.3.2rc355.post1/src/gpt_review/main.py
--rw-r--r--   0        0        0     1340 2023-05-03 21:58:23.734940 gpt-review-0.3.2rc355.post1/tests/conftest.py
--rw-r--r--   0        0        0     5645 2023-05-03 21:58:23.738940 gpt-review-0.3.2rc355.post1/tests/test_gpt_cli.py
--rw-r--r--   0        0        0     3676 1970-01-01 00:00:00.000000 gpt-review-0.3.2rc355.post1/PKG-INFO
+-rw-r--r--   0        0        0      336 2023-05-03 22:46:31.589727 gpt-review-0.4.0rc362.post1/.devcontainer/Dockerfile
+-rw-r--r--   0        0        0     1595 2023-05-03 22:46:31.589727 gpt-review-0.4.0rc362.post1/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0     1445 2023-05-03 22:46:31.589727 gpt-review-0.4.0rc362.post1/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0        0        0      611 2023-05-03 22:46:31.589727 gpt-review-0.4.0rc362.post1/.github/dependabot.yml
+-rw-r--r--   0        0        0      697 2023-05-03 22:46:31.589727 gpt-review-0.4.0rc362.post1/.github/pull_request_template.md
+-rw-r--r--   0        0        0     1336 2023-05-03 22:46:31.589727 gpt-review-0.4.0rc362.post1/.github/workflows/codeql.yml
+-rw-r--r--   0        0        0      885 2023-05-03 22:46:31.589727 gpt-review-0.4.0rc362.post1/.github/workflows/dependency-review.yml
+-rw-r--r--   0        0        0     1744 2023-05-03 22:46:31.589727 gpt-review-0.4.0rc362.post1/.github/workflows/on-push-create-draft-release.yml
+-rw-r--r--   0        0        0     4335 2023-05-03 22:46:31.589727 gpt-review-0.4.0rc362.post1/.github/workflows/python.yml
+-rw-r--r--   0        0        0      314 2023-05-03 22:46:31.593727 gpt-review-0.4.0rc362.post1/.github/workflows/semantic-pr-check.yml
+-rw-r--r--   0        0        0     1341 2023-05-03 22:46:31.593727 gpt-review-0.4.0rc362.post1/.github/workflows/test-action.yml
+-rw-r--r--   0        0        0     1808 2023-05-03 22:46:31.593727 gpt-review-0.4.0rc362.post1/.gitignore
+-rw-r--r--   0        0        0      158 2023-05-03 22:46:31.593727 gpt-review-0.4.0rc362.post1/.pypirc
+-rw-r--r--   0        0        0     1125 2023-05-03 22:46:31.593727 gpt-review-0.4.0rc362.post1/.vscode/settings.json
+-rw-r--r--   0        0        0     1070 2023-05-03 22:46:31.593727 gpt-review-0.4.0rc362.post1/LICENSE
+-rw-r--r--   0        0        0     1617 2023-05-03 22:46:31.593727 gpt-review-0.4.0rc362.post1/README.md
+-rw-r--r--   0        0        0     4920 2023-05-03 22:46:31.593727 gpt-review-0.4.0rc362.post1/action.yml
+-rw-r--r--   0        0        0     8252 2023-05-03 22:46:31.593727 gpt-review-0.4.0rc362.post1/pyproject.toml
+-rw-r--r--   0        0        0      366 2023-05-03 22:46:40.021897 gpt-review-0.4.0rc362.post1/src/gpt_review/__init__.py
+-rw-r--r--   0        0        0    11455 2023-05-03 22:46:31.593727 gpt-review-0.4.0rc362.post1/src/gpt_review/_ask.py
+-rw-r--r--   0        0        0      394 2023-05-03 22:46:31.593727 gpt-review-0.4.0rc362.post1/src/gpt_review/_command.py
+-rw-r--r--   0        0        0     1924 2023-05-03 22:46:31.593727 gpt-review-0.4.0rc362.post1/src/gpt_review/_git.py
+-rw-r--r--   0        0        0     5738 2023-05-03 22:46:31.593727 gpt-review-0.4.0rc362.post1/src/gpt_review/_github.py
+-rw-r--r--   0        0        0     1402 2023-05-03 22:46:31.593727 gpt-review-0.4.0rc362.post1/src/gpt_review/_gpt_cli.py
+-rw-r--r--   0        0        0      788 2023-05-03 22:46:31.593727 gpt-review-0.4.0rc362.post1/src/gpt_review/_repository.py
+-rw-r--r--   0        0        0     6730 2023-05-03 22:46:31.593727 gpt-review-0.4.0rc362.post1/src/gpt_review/_review.py
+-rw-r--r--   0        0        0      464 2023-05-03 22:46:31.593727 gpt-review-0.4.0rc362.post1/src/gpt_review/constants.py
+-rw-r--r--   0        0        0      488 2023-05-03 22:46:31.593727 gpt-review-0.4.0rc362.post1/src/gpt_review/main.py
+-rw-r--r--   0        0        0     2566 2023-05-03 22:46:31.593727 gpt-review-0.4.0rc362.post1/tests/conftest.py
+-rw-r--r--   0        0        0      639 2023-05-03 22:46:31.593727 gpt-review-0.4.0rc362.post1/tests/mock.diff
+-rw-r--r--   0        0        0      462 2023-05-03 22:46:31.593727 gpt-review-0.4.0rc362.post1/tests/test_git.py
+-rw-r--r--   0        0        0     1363 2023-05-03 22:46:31.593727 gpt-review-0.4.0rc362.post1/tests/test_github.py
+-rw-r--r--   0        0        0     5987 2023-05-03 22:46:31.593727 gpt-review-0.4.0rc362.post1/tests/test_gpt_cli.py
+-rw-r--r--   0        0        0      420 2023-05-03 22:46:31.593727 gpt-review-0.4.0rc362.post1/tests/test_review.py
+-rw-r--r--   0        0        0     3676 1970-01-01 00:00:00.000000 gpt-review-0.4.0rc362.post1/PKG-INFO
```

### Comparing `gpt-review-0.3.2rc355.post1/.devcontainer/devcontainer.json` & `gpt-review-0.4.0rc362.post1/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `gpt-review-0.3.2rc355.post1/.github/ISSUE_TEMPLATE/bug_report.yml` & `gpt-review-0.4.0rc362.post1/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.3.2rc355.post1/.github/dependabot.yml` & `gpt-review-0.4.0rc362.post1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.3.2rc355.post1/.github/pull_request_template.md` & `gpt-review-0.4.0rc362.post1/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `gpt-review-0.3.2rc355.post1/.github/workflows/codeql.yml` & `gpt-review-0.4.0rc362.post1/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.3.2rc355.post1/.github/workflows/dependency-review.yml` & `gpt-review-0.4.0rc362.post1/.github/workflows/dependency-review.yml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.3.2rc355.post1/.github/workflows/on-push-create-draft-release.yml` & `gpt-review-0.4.0rc362.post1/.github/workflows/on-push-create-draft-release.yml`

 * *Files 20% similar despite different names*

```diff
@@ -38,7 +38,19 @@
       - uses: EndBug/add-and-commit@v9
         if: steps.tag_version.outputs.release_type
         with:
           message: Update Version to ${{ steps.tag_version.outputs.new_version }} [no ci]
           committer_name: GitHub Actions
           committer_email: actions@github.com
           add: "src/gpt_review/__init__.py"
+
+      - uses: "dciborow/action-automatic-releases-2@v1.0.0"
+        if: steps.tag_version.outputs.release_type
+        with:
+          repo_token: "${{ secrets.GITHUB_TOKEN }}"
+          draft: true
+          title: ${{ steps.tag_version.outputs.new_tag }}
+          prerelease: false
+          files: |
+            LICENSE.md
+            dist/*.tar.gz
+            dist/*.whl
```

### Comparing `gpt-review-0.3.2rc355.post1/.github/workflows/python.yml` & `gpt-review-0.4.0rc362.post1/.github/workflows/python.yml`

 * *Files 4% similar despite different names*

```diff
@@ -47,33 +47,35 @@
 
   publish:
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v2
         with:
           ref: ${{ github.event.pull_request.head.sha }}
+          token: ${{ secrets.PAT }}
 
       - uses: actions/setup-python@v1
         with:
           python-version: '3.11.3'
+          cache: 'pip' # caching pip dependencies
 
       - name: Bump version and push tag
         id: tag_version
         uses: mathieudutour/github-tag-action@v6.0
         with:
           github_token: ${{ secrets.GITHUB_TOKEN }}
           dry_run: true
           default_bump: false
 
       - name: Set Configurations
         if: steps.tag_version.outputs.release_type && github.event_name != 'release'
         shell: bash
         env:
           VERSION: ${{ steps.tag_version.outputs.new_version }}
-        run: sed -ri 's/(__version__ = ")([0-9]+\.[0-9]+\.[0-9]+?(.*))(")/\1'"$VERSION"'\3/' "src/gpt_review/__init__.py" || exit 1
+        run: sed -ri 's/(__version__ = ")([0-9]+\.[0-9]+\.[0-9]+?.*)(")/\1'"$VERSION"'\3/' "src/gpt_review/__init__.py" || exit 1
 
       - uses: EndBug/add-and-commit@v9
         if: ${{ github.event_name == 'push' }}
         with:
           message: Update Version to ${{ steps.tag_version.outputs.new_version }} [no ci]
           committer_name: GitHub Actions
           committer_email: actions@github.com
```

### Comparing `gpt-review-0.3.2rc355.post1/.gitignore` & `gpt-review-0.4.0rc362.post1/.gitignore`

 * *Files identical despite different names*

### Comparing `gpt-review-0.3.2rc355.post1/.vscode/settings.json` & `gpt-review-0.4.0rc362.post1/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `gpt-review-0.3.2rc355.post1/LICENSE` & `gpt-review-0.4.0rc362.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `gpt-review-0.3.2rc355.post1/README.md` & `gpt-review-0.4.0rc362.post1/README.md`

 * *Files identical despite different names*

### Comparing `gpt-review-0.3.2rc355.post1/action.yml` & `gpt-review-0.4.0rc362.post1/action.yml`

 * *Files 15% similar despite different names*

```diff
@@ -101,44 +101,36 @@
     default: false
     required: false
     type: string
 
 runs:
   using: "composite"
   steps:
-      - name: Set up Python 3.8
+      - name: Set up Python 3.11
         uses: actions/setup-python@v2
         with:
-          python-version: 3.8
+          python-version: 3.11
       - name: Install
         shell: bash
         run: |
           sudo apt-get update
           python3 -m venv .env
           source .env/bin/activate
           python -m pip install --upgrade pip
-          python -m pip install \
-            requests \
-            openai \
-            pyyaml
-
-      - name: Set env.BRANCH
-        shell: bash
-        if: ${{ github.action_ref == '' }}
-        run: echo "BRANCH=$(echo ${GITHUB_HEAD_REF:-${GITHUB_REF##*/}})" >> $GITHUB_ENV
+          python -m pip install gpt-review
 
       - name: Review PR and make comment
         shell: bash
         run: |
           source .env/bin/activate
-          
-          ORG_NAME=$(echo ${BRANCH%/*})
-          curl --request GET --url https://raw.githubusercontent.com/$ORG_NAME/gpt-review/$ACTION_REF/review.py > review.py
 
-          python review.py
+          gpt github review \
+            --access-token $GITHUB_TOKEN \
+            --pull-request $PATCH_PR \
+            --repository $PATCH_REPO
         env:
           ACTION_REF: ${{ github.action_ref || env.BRANCH }}
           GIT_COMMIT_HASH: ${{ inputs.GIT_COMMIT_HASH }}
           GITHUB_TOKEN: ${{ inputs.GITHUB_TOKEN }}
           LINK: "https://github.com/${{ inputs.REPOSITORY_NAME }}/pull/${{ inputs.PR_NUMBER }}"
           OPENAI_API_KEY: ${{ inputs.OPENAI_API_KEY }}
           OPENAI_ORG_KEY: ${{ inputs.OPENAI_ORG_KEY }}
```

### Comparing `gpt-review-0.3.2rc355.post1/pyproject.toml` & `gpt-review-0.4.0rc362.post1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gpt-review-0.3.2rc355.post1/src/gpt_review/_ask.py` & `gpt-review-0.4.0rc362.post1/src/gpt_review/_ask.py`

 * *Files identical despite different names*

### Comparing `gpt-review-0.3.2rc355.post1/src/gpt_review/_gpt_cli.py` & `gpt-review-0.4.0rc362.post1/src/gpt_review/_gpt_cli.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 import os
 import sys
 
 from knack import CLI, CLICommandsLoader
 
 from gpt_review import __version__
 from gpt_review._ask import AskCommandGroup
+from gpt_review._git import GitCommandGroup
+from gpt_review._github import GitHubCommandGroup
 
 CLI_NAME = "gpt"
 
 
 class GPTCLI(CLI):
     """Custom CLI implemntation to set version for the GPT CLI."""
 
@@ -19,27 +21,25 @@
 
 
 class GPTCommandsLoader(CLICommandsLoader):
     """The GPT CLI Commands Loader."""
 
     _CommandGroups = [
         AskCommandGroup,
-    ]
-
-    _ArgumentGroups = [
-        AskCommandGroup,
+        GitHubCommandGroup,
+        GitCommandGroup,
     ]
 
     def load_command_table(self, args) -> OrderedDict:
         for command_group in self._CommandGroups:
             command_group.load_command_table(self)
         return OrderedDict(self.command_table)
 
     def load_arguments(self, command) -> None:
-        for argument_group in self._ArgumentGroups:
+        for argument_group in self._CommandGroups:
             argument_group.load_arguments(self)
         super(GPTCommandsLoader, self).load_arguments(command)
 
 
 def cli() -> int:
     """The GPT CLI entry point."""
     gpt = GPTCLI(
```

### Comparing `gpt-review-0.3.2rc355.post1/tests/conftest.py` & `gpt-review-0.4.0rc362.post1/tests/conftest.py`

 * *Files 22% similar despite different names*

```diff
@@ -40,7 +40,55 @@
         return MockResponse()
 
     def from_documents(documents, service_context=None) -> MockIndex:
         return MockIndex()
 
     monkeypatch.setattr("openai.ChatCompletion.create", mock_create)
     monkeypatch.setattr("llama_index.GPTVectorStoreIndex.from_documents", from_documents)
+
+
+@pytest.fixture
+def mock_github(monkeypatch) -> None:
+    """
+    Mock GitHub Functions with monkeypatch
+    - requests.get
+    """
+
+    class MockResponse:
+        def __init__(self) -> None:
+            self.text = "diff --git a/README.md b/README.md"
+
+        def json(self) -> dict:
+            return {"test": "test"}
+
+    def mock_get(url, headers, timeout) -> MockResponse:
+        return MockResponse()
+
+    def mock_put(url, headers, timeout) -> MockResponse:
+        return MockResponse()
+
+    def mock_post(url, headers, data, timeout) -> MockResponse:
+        return MockResponse()
+
+    monkeypatch.setattr("requests.get", mock_get)
+    monkeypatch.setattr("requests.put", mock_put)
+    monkeypatch.setattr("requests.post", mock_post)
+
+
+@pytest.fixture
+def mock_git_commit(monkeypatch) -> None:
+    """Mock git.commit with pytest monkey patch"""
+
+    class MockGit:
+        def __init__(self) -> None:
+            self.git = self
+
+        def commit(self, message) -> str:
+            return "test commit response"
+
+        def diff(self, message, cached) -> str:
+            return "test diff response"
+
+    def mock_init(cls):
+        return MockGit()
+
+    monkeypatch.setattr("git.repo.Repo.init", mock_init)
```

### Comparing `gpt-review-0.3.2rc355.post1/tests/test_gpt_cli.py` & `gpt-review-0.4.0rc362.post1/tests/test_gpt_cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -98,38 +98,30 @@
     ),
     CLICase(
         f"ask how are you --fast --max-tokens={C.MAX_TOKENS_DEFAULT} --temperature {C.TEMPERATURE_DEFAULT} --frequency-penalty {C.FREQUENCY_PENALTY_DEFAULT} --presence-penalty {C.FREQUENCY_PENALTY_MAX}"
     ),
     CLICase(
         f"""ask how are you --fast --max-tokens {C.MAX_TOKENS_DEFAULT} --top-p {C.TOP_P_DEFAULT} --frequency-penalty {C.FREQUENCY_PENALTY_DEFAULT} --presence-penalty {C.FREQUENCY_PENALTY_MAX}"""
     ),
-    CLICase("ask --files review.py --files review.py what programming language is this code written in?"),
-    CLICase("ask --fast -f review.py what programming language is this code written in?"),
+    CLICase(
+        "ask --files src/gpt_review/main.py --files src/gpt_review/main.py what programming language is this code written in?"
+    ),
+    CLICase("git commit --help"),
+    # CLICase("git commit"),
+    CLICase("github review --help"),
+    CLICase("github review"),
+    CLICase(
+        "ask --files src/gpt_review/__init__.py --files src/gpt_review/__init__.py what programming language is this code written in?"
+    ),
+    CLICase("ask --fast -f src/gpt_review/__init__.py what programming language is this code written in?"),
 ]
 
 ARGS = ROOT_COMMANDS + ASK_COMMANDS
 
 
-@pytest.mark.parametrize("command", ARGS)
-@pytest.mark.cli
-def test_cli_gpt_cli(command: CLICase) -> None:
-    """Test gpt commands from installed CLI"""
-
-    command_array = f"gpt {command.command}".split(" ")
-
-    result = subprocess.run(
-        command_array,
-        stdout=subprocess.PIPE,
-        stderr=subprocess.PIPE,
-        check=False,
-    )
-
-    assert result.returncode == command.expected_error_code
-
-
 def gpt_cli_test(command: CLICase) -> None:
     os.environ["GPT_ASK_COMMANDS"] = "1"
 
     sys.argv[1:] = command.command.split(" ")
 
     try:
         exit_code = cli()
@@ -148,7 +140,24 @@
 
 @pytest.mark.parametrize(
     "command",
     ARGS,
 )
 def test_gpt_cli(command: CLICase, mock_openai: None) -> None:
     gpt_cli_test(command)
+
+
+@pytest.mark.parametrize("command", ARGS)
+@pytest.mark.cli
+def test_cli_gpt_cli(command: CLICase) -> None:
+    """Test gpt commands from installed CLI"""
+
+    command_array = f"gpt {command.command}".split(" ")
+
+    result = subprocess.run(
+        command_array,
+        stdout=subprocess.PIPE,
+        stderr=subprocess.PIPE,
+        check=False,
+    )
+
+    assert result.returncode == command.expected_error_code
```

### Comparing `gpt-review-0.3.2rc355.post1/PKG-INFO` & `gpt-review-0.4.0rc362.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpt-review
-Version: 0.3.2rc355.post1
+Version: 0.4.0rc362.post1
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
-Metadata-Version: 2.1 Name: gpt-review Version: 0.3.2rc355.post1 Summary:
+Metadata-Version: 2.1 Name: gpt-review Version: 0.4.0rc362.post1 Summary:
 Python Project for reviewing GitHub PRs with Open AI and Chat-GPT. Author-
 email: Daniel Ciborowski
 microsoft.com> Requires-Python: >=3.7 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 :: Only Classifier: Programming Language ::
 Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
```

