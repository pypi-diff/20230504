# Comparing `tmp/aiida-shell-0.5.0.tar.gz` & `tmp/aiida-shell-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiida-shell-0.5.0.tar", last modified: Wed May  3 09:34:03 2023, max compression
+gzip compressed data, was "aiida-shell-0.5.1.tar", last modified: Wed May  3 22:10:15 2023, max compression
```

## Comparing `aiida-shell-0.5.0.tar` & `aiida-shell-0.5.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0      184 2023-04-25 15:09:47.669921 aiida-shell-0.5.0/.readthedocs.yml
--rw-r--r--   0        0        0    10653 2023-05-03 09:13:18.263500 aiida-shell-0.5.0/CHANGELOG.md
--rw-r--r--   0        0        0      448 2023-05-03 09:06:02.308511 aiida-shell-0.5.0/CITATION.cff
--rw-r--r--   0        0        0     1076 2022-10-20 00:30:58.784996 aiida-shell-0.5.0/LICENSE.txt
--rw-r--r--   0        0        0      728 2023-04-25 15:09:47.669921 aiida-shell-0.5.0/README.md
--rw-r--r--   0        0        0      638 2023-04-25 15:09:47.669921 aiida-shell-0.5.0/docs/Makefile
--rw-r--r--   0        0        0     1323 2023-04-25 15:09:47.669921 aiida-shell-0.5.0/docs/source/conf.py
--rw-r--r--   0        0        0    15543 2023-05-03 02:58:19.035109 aiida-shell-0.5.0/docs/source/howto.rst
--rw-r--r--   0        0        0    25440 2023-04-25 15:09:47.679921 aiida-shell-0.5.0/docs/source/images/logo-column.png
--rw-r--r--   0        0        0   164551 2023-04-25 15:09:47.679921 aiida-shell-0.5.0/docs/source/images/logo-column.svg
--rw-r--r--   0        0        0   167883 2023-04-25 15:09:47.679921 aiida-shell-0.5.0/docs/source/images/logo-text.svg
--rw-r--r--   0        0        0      429 2023-04-25 15:09:47.679921 aiida-shell-0.5.0/docs/source/index.rst
--rw-r--r--   0        0        0      590 2023-04-25 15:09:47.679921 aiida-shell-0.5.0/docs/source/installation.rst
--rw-r--r--   0        0        0     3191 2023-04-25 15:09:47.679921 aiida-shell-0.5.0/pyproject.toml
--rw-r--r--   0        0        0      239 2023-05-03 09:08:04.335187 aiida-shell-0.5.0/src/aiida_shell/__init__.py
--rw-r--r--   0        0        0      127 2022-10-20 00:30:58.784996 aiida-shell-0.5.0/src/aiida_shell/calculations/__init__.py
--rw-r--r--   0        0        0    13794 2023-04-28 07:05:58.787771 aiida-shell-0.5.0/src/aiida_shell/calculations/shell.py
--rw-r--r--   0        0        0      167 2023-04-25 15:09:47.689921 aiida-shell-0.5.0/src/aiida_shell/data/__init__.py
--rw-r--r--   0        0        0     1624 2022-11-07 18:18:08.659450 aiida-shell-0.5.0/src/aiida_shell/data/code.py
--rw-r--r--   0        0        0     5518 2023-04-25 15:09:47.689921 aiida-shell-0.5.0/src/aiida_shell/data/pickled.py
--rw-r--r--   0        0        0      141 2022-10-20 00:30:58.784996 aiida-shell-0.5.0/src/aiida_shell/engine/__init__.py
--rw-r--r--   0        0        0      151 2022-10-20 00:30:58.784996 aiida-shell-0.5.0/src/aiida_shell/engine/launchers/__init__.py
--rw-r--r--   0        0        0     8654 2023-05-03 02:58:19.035109 aiida-shell-0.5.0/src/aiida_shell/engine/launchers/shell_job.py
--rw-r--r--   0        0        0      128 2022-10-20 00:30:58.784996 aiida-shell-0.5.0/src/aiida_shell/parsers/__init__.py
--rw-r--r--   0        0        0     5572 2023-04-25 15:09:47.689921 aiida-shell-0.5.0/src/aiida_shell/parsers/shell.py
--rw-r--r--   0        0        0     2460 1970-01-01 00:00:00.000000 aiida-shell-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0      184 2023-05-03 22:10:12.642934 aiida-shell-0.5.1/.readthedocs.yml
+-rw-r--r--   0        0        0    11029 2023-05-03 22:10:12.642934 aiida-shell-0.5.1/CHANGELOG.md
+-rw-r--r--   0        0        0      448 2023-05-03 22:10:12.642934 aiida-shell-0.5.1/CITATION.cff
+-rw-r--r--   0        0        0     1076 2023-05-03 22:10:12.642934 aiida-shell-0.5.1/LICENSE.txt
+-rw-r--r--   0        0        0      728 2023-05-03 22:10:12.642934 aiida-shell-0.5.1/README.md
+-rw-r--r--   0        0        0      638 2023-05-03 22:10:12.642934 aiida-shell-0.5.1/docs/Makefile
+-rw-r--r--   0        0        0     1323 2023-05-03 22:10:12.642934 aiida-shell-0.5.1/docs/source/conf.py
+-rw-r--r--   0        0        0    15543 2023-05-03 22:10:12.642934 aiida-shell-0.5.1/docs/source/howto.rst
+-rw-r--r--   0        0        0    25440 2023-05-03 22:10:12.642934 aiida-shell-0.5.1/docs/source/images/logo-column.png
+-rw-r--r--   0        0        0   164551 2023-05-03 22:10:12.642934 aiida-shell-0.5.1/docs/source/images/logo-column.svg
+-rw-r--r--   0        0        0   167883 2023-05-03 22:10:12.642934 aiida-shell-0.5.1/docs/source/images/logo-text.svg
+-rw-r--r--   0        0        0      429 2023-05-03 22:10:12.642934 aiida-shell-0.5.1/docs/source/index.rst
+-rw-r--r--   0        0        0      590 2023-05-03 22:10:12.642934 aiida-shell-0.5.1/docs/source/installation.rst
+-rw-r--r--   0        0        0     3191 2023-05-03 22:10:12.642934 aiida-shell-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0      239 2023-05-03 22:10:12.642934 aiida-shell-0.5.1/src/aiida_shell/__init__.py
+-rw-r--r--   0        0        0      127 2023-05-03 22:10:12.642934 aiida-shell-0.5.1/src/aiida_shell/calculations/__init__.py
+-rw-r--r--   0        0        0    13771 2023-05-03 22:10:12.646934 aiida-shell-0.5.1/src/aiida_shell/calculations/shell.py
+-rw-r--r--   0        0        0      167 2023-05-03 22:10:12.646934 aiida-shell-0.5.1/src/aiida_shell/data/__init__.py
+-rw-r--r--   0        0        0     1624 2023-05-03 22:10:12.646934 aiida-shell-0.5.1/src/aiida_shell/data/code.py
+-rw-r--r--   0        0        0     5518 2023-05-03 22:10:12.646934 aiida-shell-0.5.1/src/aiida_shell/data/pickled.py
+-rw-r--r--   0        0        0      141 2023-05-03 22:10:12.646934 aiida-shell-0.5.1/src/aiida_shell/engine/__init__.py
+-rw-r--r--   0        0        0      151 2023-05-03 22:10:12.646934 aiida-shell-0.5.1/src/aiida_shell/engine/launchers/__init__.py
+-rw-r--r--   0        0        0     8797 2023-05-03 22:10:12.646934 aiida-shell-0.5.1/src/aiida_shell/engine/launchers/shell_job.py
+-rw-r--r--   0        0        0      128 2023-05-03 22:10:12.646934 aiida-shell-0.5.1/src/aiida_shell/parsers/__init__.py
+-rw-r--r--   0        0        0     5572 2023-05-03 22:10:12.646934 aiida-shell-0.5.1/src/aiida_shell/parsers/shell.py
+-rw-r--r--   0        0        0     2460 1970-01-01 00:00:00.000000 aiida-shell-0.5.1/PKG-INFO
```

### Comparing `aiida-shell-0.5.0/CHANGELOG.md` & `aiida-shell-0.5.1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,16 @@
 # Change log
 
+## `v0.5.1` - 2023-05-04
+
+### Fixes
+- `ShellJob`: Remove `tot_num_mpiprocs` from `resources` default [[5e61c89]](https://github.com/sphuber/aiida-shell/commit/5e61c891958f705eaf56d8b590227011f16706ef)
+- `launch_shell_job`: Only `which` command if code doesn't already exist [[c1c31ab]](https://github.com/sphuber/aiida-shell/commit/c1c31ab404abcad4778accc8c01c3afbb818dfc8)
+
+
 ## `v0.5.0` - 2023-05-03
 
 ### Features
 - `launch_shell_job`: Accept string for the `arguments` argument [[a8af91a]](https://github.com/sphuber/aiida-shell/commit/a8af91a5a0005233c3de4669b74bc185892a8126)
 
     It is now possible to pass the command line arguments for the command as a string, instead of a list of individual arguments:
     ```python
```

### Comparing `aiida-shell-0.5.0/LICENSE.txt` & `aiida-shell-0.5.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aiida-shell-0.5.0/README.md` & `aiida-shell-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `aiida-shell-0.5.0/docs/Makefile` & `aiida-shell-0.5.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `aiida-shell-0.5.0/docs/source/conf.py` & `aiida-shell-0.5.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `aiida-shell-0.5.0/docs/source/howto.rst` & `aiida-shell-0.5.1/docs/source/howto.rst`

 * *Files identical despite different names*

### Comparing `aiida-shell-0.5.0/docs/source/images/logo-column.png` & `aiida-shell-0.5.1/docs/source/images/logo-column.png`

 * *Files identical despite different names*

### Comparing `aiida-shell-0.5.0/docs/source/images/logo-column.svg` & `aiida-shell-0.5.1/docs/source/images/logo-column.svg`

 * *Files identical despite different names*

### Comparing `aiida-shell-0.5.0/docs/source/images/logo-text.svg` & `aiida-shell-0.5.1/docs/source/images/logo-text.svg`

 * *Files identical despite different names*

### Comparing `aiida-shell-0.5.0/docs/source/installation.rst` & `aiida-shell-0.5.1/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `aiida-shell-0.5.0/pyproject.toml` & `aiida-shell-0.5.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aiida-shell-0.5.0/src/aiida_shell/calculations/shell.py` & `aiida-shell-0.5.1/src/aiida_shell/calculations/shell.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,15 @@
             valid_type=list,
             help='List of filepaths that are to be retrieved in addition to defaults and those specified in the '
             '`outputs` input. This is useful if files need to be retrieved for a custom `parser`.'
         )
 
         options = spec.inputs['metadata']['options']  # type: ignore[index]
         options['parser_name'].default = 'core.shell'  # type: ignore[index]
-        options['resources'].default = {'num_machines': 1, 'tot_num_mpiprocs': 1}  # type: ignore[index]
+        options['resources'].default = {'num_machines': 1}  # type: ignore[index]
 
         spec.outputs.dynamic = True
 
         spec.exit_code(
             300,
             'ERROR_OUTPUT_STATUS_MISSING',
             message='Exit status could not be determined: exit status file was not retrieved.'
```

### Comparing `aiida-shell-0.5.0/src/aiida_shell/data/code.py` & `aiida-shell-0.5.1/src/aiida_shell/data/code.py`

 * *Files identical despite different names*

### Comparing `aiida-shell-0.5.0/src/aiida_shell/data/pickled.py` & `aiida-shell-0.5.1/src/aiida_shell/data/pickled.py`

 * *Files identical despite different names*

### Comparing `aiida-shell-0.5.0/src/aiida_shell/engine/launchers/shell_job.py` & `aiida-shell-0.5.1/src/aiida_shell/engine/launchers/shell_job.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,28 +91,30 @@
     This will automatically prepare the computer
 
     :param command: The command that the code should represent. Can be the relative executable name or absolute path.
     :param computer: The computer on which the command should be run. If not defined the localhost will be used.
     :return: A :class:`aiida.orm.nodes.code.abstract.AbstractCode` instance.
     """
     computer = prepare_computer(computer)
-
-    with computer.get_transport() as transport:
-        status, stdout, stderr = transport.exec_command_wait(f'which {command}')
-        executable = stdout.strip()
-
-        if status != 0:
-            raise ValueError(f'failed to determine the absolute path of the command on the computer: {stderr}')
-
     code_label = f'{command}@{computer.label}'
 
     try:
         code: AbstractCode = load_code(code_label)
-    except exceptions.NotExistent:
+    except exceptions.NotExistent as exception:
         LOGGER.info('No code exists yet for `%s`, creating it now.', code_label)
+
+        with computer.get_transport() as transport:
+            status, stdout, stderr = transport.exec_command_wait(f'which {command}')
+            executable = stdout.strip()
+
+            if status != 0:
+                raise ValueError(
+                    f'failed to determine the absolute path of the command on the computer: {stderr}'
+                ) from exception
+
         code = ShellCode(  # type: ignore[assignment]
             label=command, computer=computer, filepath_executable=executable, default_calc_job_plugin='core.shell'
         ).store()
 
     return code
 
 
@@ -143,14 +145,15 @@
                 description='Localhost automatically created by `aiida.engine.launch_shell_job`',
                 transport_type='core.local',
                 scheduler_type='core.direct',
                 workdir=tempfile.gettempdir(),
             ).store()
             computer.configure(safe_interval=0.)
             computer.set_minimum_job_poll_interval(0.)
+            computer.set_default_mpiprocs_per_machine(1)
 
     default_user = computer.backend.default_user
 
     if default_user and not computer.is_user_configured(default_user):
         computer.configure(default_user)
 
     return computer
```

### Comparing `aiida-shell-0.5.0/src/aiida_shell/parsers/shell.py` & `aiida-shell-0.5.1/src/aiida_shell/parsers/shell.py`

 * *Files identical despite different names*

### Comparing `aiida-shell-0.5.0/PKG-INFO` & `aiida-shell-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiida-shell
-Version: 0.5.0
+Version: 0.5.1
 Summary: AiiDA plugin that makes running shell commands easy.
 Keywords: aiida,workflows
 Author-email: "Sebastiaan P. Huber" <mail@sphuber.net>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: AiiDA
```

