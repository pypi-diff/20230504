# Comparing `tmp/kedro_azureml-0.4.0.tar.gz` & `tmp/kedro_azureml-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kedro_azureml-0.4.0.tar", max compression
+gzip compressed data, was "kedro_azureml-0.4.1.tar", max compression
```

## Comparing `kedro_azureml-0.4.0.tar` & `kedro_azureml-0.4.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0    11338 2023-04-28 13:30:42.924832 kedro_azureml-0.4.0/LICENSE
--rw-r--r--   0        0        0     2441 2023-04-28 13:30:42.924832 kedro_azureml-0.4.0/README.md
--rw-r--r--   0        0        0       96 2023-04-28 13:30:42.932833 kedro_azureml-0.4.0/kedro_azureml/__init__.py
--rw-r--r--   0        0        0    10195 2023-04-28 13:30:42.936833 kedro_azureml-0.4.0/kedro_azureml/cli.py
--rw-r--r--   0        0        0     5018 2023-04-28 13:30:42.936833 kedro_azureml-0.4.0/kedro_azureml/cli_functions.py
--rw-r--r--   0        0        0     3270 2023-04-28 13:30:42.936833 kedro_azureml-0.4.0/kedro_azureml/client.py
--rw-r--r--   0        0        0     4475 2023-04-28 13:30:42.936833 kedro_azureml-0.4.0/kedro_azureml/config.py
--rw-r--r--   0        0        0      323 2023-04-28 13:30:42.936833 kedro_azureml-0.4.0/kedro_azureml/constants.py
--rw-r--r--   0        0        0      508 2023-04-28 13:30:42.936833 kedro_azureml-0.4.0/kedro_azureml/datasets/__init__.py
--rw-r--r--   0        0        0    10959 2023-04-28 13:30:42.936833 kedro_azureml-0.4.0/kedro_azureml/datasets/file_dataset.py
--rw-r--r--   0        0        0     5305 2023-04-28 13:30:42.936833 kedro_azureml-0.4.0/kedro_azureml/datasets/pandas_dataset.py
--rw-r--r--   0        0        0     4254 2023-04-28 13:30:42.936833 kedro_azureml-0.4.0/kedro_azureml/datasets/pipeline_dataset.py
--rw-r--r--   0        0        0     2653 2023-04-28 13:30:42.936833 kedro_azureml-0.4.0/kedro_azureml/datasets/runner_dataset.py
--rw-r--r--   0        0        0      906 2023-04-28 13:30:42.936833 kedro_azureml-0.4.0/kedro_azureml/datasets/utils.py
--rw-r--r--   0        0        0      149 2023-04-28 13:30:42.936833 kedro_azureml-0.4.0/kedro_azureml/distributed/__init__.py
--rw-r--r--   0        0        0      453 2023-04-28 13:30:42.936833 kedro_azureml-0.4.0/kedro_azureml/distributed/config.py
--rw-r--r--   0        0        0      701 2023-04-28 13:30:42.936833 kedro_azureml-0.4.0/kedro_azureml/distributed/decorators.py
--rw-r--r--   0        0        0     1220 2023-04-28 13:30:42.936833 kedro_azureml-0.4.0/kedro_azureml/distributed/utils.py
--rw-r--r--   0        0        0    12385 2023-04-28 13:30:42.936833 kedro_azureml-0.4.0/kedro_azureml/generator.py
--rw-r--r--   0        0        0     2784 2023-04-28 13:30:42.936833 kedro_azureml-0.4.0/kedro_azureml/manager.py
--rw-r--r--   0        0        0     3509 2023-04-28 13:30:42.936833 kedro_azureml-0.4.0/kedro_azureml/runner.py
--rw-r--r--   0        0        0      568 2023-04-28 13:30:42.936833 kedro_azureml-0.4.0/kedro_azureml/utils.py
--rw-r--r--   0        0        0     1676 2023-04-28 13:30:42.936833 kedro_azureml-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     3837 1970-01-01 00:00:00.000000 kedro_azureml-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0    11338 2023-05-04 14:46:00.977920 kedro_azureml-0.4.1/LICENSE
+-rw-r--r--   0        0        0     2441 2023-05-04 14:46:00.977920 kedro_azureml-0.4.1/README.md
+-rw-r--r--   0        0        0       96 2023-05-04 14:46:00.989920 kedro_azureml-0.4.1/kedro_azureml/__init__.py
+-rw-r--r--   0        0        0    11456 2023-05-04 14:46:00.989920 kedro_azureml-0.4.1/kedro_azureml/cli.py
+-rw-r--r--   0        0        0     5018 2023-05-04 14:46:00.989920 kedro_azureml-0.4.1/kedro_azureml/cli_functions.py
+-rw-r--r--   0        0        0     3270 2023-05-04 14:46:00.989920 kedro_azureml-0.4.1/kedro_azureml/client.py
+-rw-r--r--   0        0        0     4613 2023-05-04 14:46:00.989920 kedro_azureml-0.4.1/kedro_azureml/config.py
+-rw-r--r--   0        0        0      323 2023-05-04 14:46:00.989920 kedro_azureml-0.4.1/kedro_azureml/constants.py
+-rw-r--r--   0        0        0      508 2023-05-04 14:46:00.989920 kedro_azureml-0.4.1/kedro_azureml/datasets/__init__.py
+-rw-r--r--   0        0        0    10959 2023-05-04 14:46:00.989920 kedro_azureml-0.4.1/kedro_azureml/datasets/file_dataset.py
+-rw-r--r--   0        0        0     5305 2023-05-04 14:46:00.989920 kedro_azureml-0.4.1/kedro_azureml/datasets/pandas_dataset.py
+-rw-r--r--   0        0        0     4254 2023-05-04 14:46:00.989920 kedro_azureml-0.4.1/kedro_azureml/datasets/pipeline_dataset.py
+-rw-r--r--   0        0        0     2653 2023-05-04 14:46:00.989920 kedro_azureml-0.4.1/kedro_azureml/datasets/runner_dataset.py
+-rw-r--r--   0        0        0      906 2023-05-04 14:46:00.989920 kedro_azureml-0.4.1/kedro_azureml/datasets/utils.py
+-rw-r--r--   0        0        0      149 2023-05-04 14:46:00.989920 kedro_azureml-0.4.1/kedro_azureml/distributed/__init__.py
+-rw-r--r--   0        0        0      453 2023-05-04 14:46:00.989920 kedro_azureml-0.4.1/kedro_azureml/distributed/config.py
+-rw-r--r--   0        0        0      701 2023-05-04 14:46:00.989920 kedro_azureml-0.4.1/kedro_azureml/distributed/decorators.py
+-rw-r--r--   0        0        0     1220 2023-05-04 14:46:00.989920 kedro_azureml-0.4.1/kedro_azureml/distributed/utils.py
+-rw-r--r--   0        0        0    12187 2023-05-04 14:46:00.989920 kedro_azureml-0.4.1/kedro_azureml/generator.py
+-rw-r--r--   0        0        0     2784 2023-05-04 14:46:00.989920 kedro_azureml-0.4.1/kedro_azureml/manager.py
+-rw-r--r--   0        0        0     3502 2023-05-04 14:46:00.989920 kedro_azureml-0.4.1/kedro_azureml/runner.py
+-rw-r--r--   0        0        0      695 2023-05-04 14:46:00.989920 kedro_azureml-0.4.1/kedro_azureml/utils.py
+-rw-r--r--   0        0        0     1703 2023-05-04 14:46:00.989920 kedro_azureml-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     3877 1970-01-01 00:00:00.000000 kedro_azureml-0.4.1/PKG-INFO
```

### Comparing `kedro_azureml-0.4.0/LICENSE` & `kedro_azureml-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kedro_azureml-0.4.0/README.md` & `kedro_azureml-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `kedro_azureml-0.4.0/kedro_azureml/cli.py` & `kedro_azureml-0.4.1/kedro_azureml/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,71 +53,107 @@
 
 @azureml_group.command()
 @click.argument("subscription_id")
 @click.argument("resource_group")
 @click.argument("workspace_name")
 @click.argument("experiment_name")
 @click.argument("cluster_name")
-@click.argument("environment_name")
-@click.option("-a", "--storage_account_name")
-@click.option("-c", "--storage_container")
-@click.option("--use-pipeline-data-passing", is_flag=True, default=False)
+@click.option(
+    "--azureml-environment",
+    "--aml-env",
+    default=None,
+    type=str,
+    help="Azure ML environment to use with code flow",
+)
+@click.option(
+    "-d", "--docker-image", default=None, type=str, help="Docker image to use"
+)
+@click.option(
+    "-a",
+    "--storage-account-name",
+    help="Name of the storage account (if you want to use Azure Blob Storage for temporary data)",
+)
+@click.option(
+    "-c",
+    "--storage-container",
+    help="Name of the storage container (if you want to use Azure Blob Storage for temporary data)",
+)
+@click.option(
+    "--use-pipeline-data-passing",
+    is_flag=True,
+    default=False,
+    help="(flag) Set, to use EXPERIMENTAL pipeline data passing",
+)
 @click.pass_obj
 def init(
     ctx: CliContext,
     subscription_id,
     resource_group,
     workspace_name,
     experiment_name,
     cluster_name,
-    environment_name,
+    azureml_environment: Optional[str],
+    docker_image: Optional[str],
     storage_account_name,
     storage_container,
     use_pipeline_data_passing: bool,
 ):
     """
     Creates basic configuration for Kedro AzureML plugin
     """
 
+    # Check whether docker_image and azure_ml_environment are specified, they cannot be, they are mutually exclusive
+    if docker_image and azureml_environment:
+        raise click.UsageError(
+            "You cannot specify both --docker_image/-d and --azure_ml_environment/--aml_env"
+        )
+    elif not (docker_image or azureml_environment):
+        raise click.UsageError(
+            "You must specify either --docker_image/-d or --azure_ml_environment/--aml_env"
+        )
+
     if (
         not (storage_account_name and storage_container)
         and not use_pipeline_data_passing
     ):
         raise click.UsageError(
             "You need to specify storage account (-a) and container name (-c) "
-            "or enable pipeline data passing (--use-pipeline-data-passing)"
+            "or enable pipeline data passing (--use_pipeline_data_passing)"
         )
 
     target_path = Path.cwd().joinpath("conf/base/azureml.yml")
     cfg = CONFIG_TEMPLATE_YAML.format(
         **{
             "subscription_id": subscription_id,
             "resource_group": resource_group,
             "workspace_name": workspace_name,
             "experiment_name": experiment_name,
             "cluster_name": cluster_name,
             "storage_account_name": storage_account_name or "~",
             "storage_container": storage_container or "~",
-            "environment_name": environment_name,
+            "environment_name": azureml_environment or "~",
             "pipeline_data_passing": use_pipeline_data_passing,
+            "docker_image": docker_image or "~",
+            "code_directory": "." if azureml_environment else "~",
         }
     )
     target_path.write_text(cfg)
 
     click.echo(f"Configuration generated in {target_path}")
 
-    click.echo(
-        click.style(
-            f"It's recommended to set Lifecycle management rule for storage container {storage_container} "
-            f"to avoid costs of long-term storage of the temporary data."
-            f"\nTemporary data will be stored under abfs://{storage_container}/{KEDRO_AZURE_BLOB_TEMP_DIR_NAME} path"  # noqa
-            f"\nSee https://docs.microsoft.com/en-us/azure/storage/blobs/lifecycle-management-policy-configure?tabs=azure-portal",  # noqa
-            fg="green",
+    if storage_account_name and storage_container:
+        click.echo(
+            click.style(
+                f"It's recommended to set Lifecycle management rule for storage container {storage_container} "
+                f"to avoid costs of long-term storage of the temporary data."
+                f"\nTemporary data will be stored under abfs://{storage_container}/{KEDRO_AZURE_BLOB_TEMP_DIR_NAME} path"  # noqa
+                f"\nSee https://docs.microsoft.com/en-us/azure/storage/blobs/lifecycle-management-policy-configure?tabs=azure-portal",  # noqa
+                fg="green",
+            )
         )
-    )
 
     aml_ignore = Path.cwd().joinpath(".amlignore")
     if aml_ignore.exists():
         click.echo(
             click.style(
                 ".amlignore file already exist, make sure that all of the relevant files"
                 "\nwill get uploaded to Azure ML if you're using Code Upload option with this plugin",
@@ -127,22 +163,22 @@
     else:
         aml_ignore.write_text("")
 
 
 @azureml_group.command()
 @click.option(
     "-s",
-    "--subscription_id",
+    "--subscription-id",
     help=f"Azure Subscription ID. Defaults to env `{AZURE_SUBSCRIPTION_ID}`",
     default=lambda: os.getenv(AZURE_SUBSCRIPTION_ID, ""),
     type=str,
 )
 @click.option(
-    "--azureml_environment",
-    "--aml_env",
+    "--azureml-environment",
+    "--aml-env",
     "aml_env",
     type=str,
     help="Azure ML Environment to use for pipeline execution.",
 )
 @click.option(
     "-i",
     "--image",
@@ -229,16 +265,16 @@
             )
 
         click_context.exit(exit_code)
 
 
 @azureml_group.command()
 @click.option(
-    "--azureml_environment",
-    "--aml_env",
+    "--azureml-environment",
+    "--aml-env",
     "aml_env",
     type=str,
     help="Azure ML Environment to use for pipeline execution.",
 )
 @click.option(
     "-i",
     "--image",
```

### Comparing `kedro_azureml-0.4.0/kedro_azureml/cli_functions.py` & `kedro_azureml-0.4.1/kedro_azureml/cli_functions.py`

 * *Files identical despite different names*

### Comparing `kedro_azureml-0.4.0/kedro_azureml/client.py` & `kedro_azureml-0.4.1/kedro_azureml/client.py`

 * *Files identical despite different names*

### Comparing `kedro_azureml-0.4.0/kedro_azureml/config.py` & `kedro_azureml-0.4.1/kedro_azureml/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -76,17 +76,17 @@
   # Azure ML Experiment Name
   experiment_name: "{experiment_name}"
   # Azure resource group to use
   resource_group: "{resource_group}"
   # Azure ML Workspace name
   workspace_name: "{workspace_name}"
   # Azure ML Environment to use during pipeline execution
-  environment_name: "{environment_name}"
+  environment_name: {environment_name}
   # Path to directory to upload, or null to disable code upload
-  code_directory: "."
+  code_directory: {code_directory}
   # Path to the directory in the Docker image to run the code from
   # Ignored when code_directory is set
   working_directory: /home/kedro_docker
   # Use Azure ML pipeline data passing instead of temporary storage
   pipeline_data_passing:
     enabled: {pipeline_data_passing} # disabled by default
 
@@ -110,19 +110,22 @@
     # <your_node_tag>:
     #   cluster_name: "<your_cluster_name>"
 docker:
   # This option is for backward compatibility and will be removed in the future versions
   # We suggest using the Azure environment instead
   # See https://kedro-azureml.readthedocs.io/en/0.2.1/source/03_quickstart.html
   # Docker image to use during pipeline execution
-  image: ~
+  image: {docker_image}
 """.strip()
 
 # This auto-validates the template above during import
 _CONFIG_TEMPLATE = KedroAzureMLConfig.parse_obj(
     update_dict(
         yaml.safe_load(CONFIG_TEMPLATE_YAML),
         ("azure.pipeline_data_passing.enabled", False),
         ("azure.temporary_storage.container", ""),
         ("azure.temporary_storage.account_name", ""),
+        ("azure.code_directory", None),
+        ("azure.environment_name", None),
+        ("docker.image", None),
     )
 )
```

### Comparing `kedro_azureml-0.4.0/kedro_azureml/datasets/file_dataset.py` & `kedro_azureml-0.4.1/kedro_azureml/datasets/file_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro_azureml-0.4.0/kedro_azureml/datasets/pandas_dataset.py` & `kedro_azureml-0.4.1/kedro_azureml/datasets/pandas_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro_azureml-0.4.0/kedro_azureml/datasets/pipeline_dataset.py` & `kedro_azureml-0.4.1/kedro_azureml/datasets/pipeline_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro_azureml-0.4.0/kedro_azureml/datasets/runner_dataset.py` & `kedro_azureml-0.4.1/kedro_azureml/datasets/runner_dataset.py`

 * *Files identical despite different names*

### Comparing `kedro_azureml-0.4.0/kedro_azureml/datasets/utils.py` & `kedro_azureml-0.4.1/kedro_azureml/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `kedro_azureml-0.4.0/kedro_azureml/distributed/decorators.py` & `kedro_azureml-0.4.1/kedro_azureml/distributed/decorators.py`

 * *Files identical despite different names*

### Comparing `kedro_azureml-0.4.0/kedro_azureml/distributed/utils.py` & `kedro_azureml-0.4.1/kedro_azureml/distributed/utils.py`

 * *Files identical despite different names*

### Comparing `kedro_azureml-0.4.0/kedro_azureml/generator.py` & `kedro_azureml-0.4.1/kedro_azureml/generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import logging
 import re
-import warnings
 from typing import Any, Dict, Optional, Type, Union
 from uuid import uuid4
 
 from azure.ai.ml import (
     Input,
     MpiDistribution,
     Output,
@@ -130,19 +129,15 @@
             return (params or self.kedro_params)[param_name]
 
     def _resolve_azure_environment(self) -> Union[Environment, str]:
         if image := (
             self.docker_image
             or (self.config.docker.image if self.config.docker else None)
         ):
-            warnings.warn(
-                f"Using docker image: {image} to run the pipeline."
-                f"\nWe recommend to use Azure Environments instead, follow the updated Quickstart documentation",
-                DeprecationWarning,
-            )
+            logger.info(f"Using docker image: {image} to run the pipeline.")
             return Environment(image=image)
         else:
             return self.aml_env or self.config.azure.environment_name
 
     def _from_params_or_value(
         self,
         namespace: Optional[str],
```

### Comparing `kedro_azureml-0.4.0/kedro_azureml/manager.py` & `kedro_azureml-0.4.1/kedro_azureml/manager.py`

 * *Files identical despite different names*

### Comparing `kedro_azureml-0.4.0/kedro_azureml/runner.py` & `kedro_azureml-0.4.1/kedro_azureml/runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import logging
 import os
 from pathlib import Path
 from typing import Any, Dict, Optional
 
-from kedro.extras.datasets.pickle import PickleDataSet
 from kedro.io import AbstractDataSet, DataCatalog
 from kedro.pipeline import Pipeline
 from kedro.runner import SequentialRunner
+from kedro_datasets.pickle import PickleDataSet
 from pluggy import PluginManager
 
 from kedro_azureml.config import KedroAzureRunnerConfig
 from kedro_azureml.constants import KEDRO_AZURE_RUNNER_CONFIG
 from kedro_azureml.datasets import (
     AzureMLPipelineDataSet,
     KedroAzureRunnerDataset,
```

### Comparing `kedro_azureml-0.4.0/kedro_azureml/utils.py` & `kedro_azureml-0.4.1/kedro_azureml/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 @dataclass
 class CliContext:
     env: str
     metadata: Any
 
 
 def update_dict(dictionary, *kv_pairs):
+    """Return a deep copy of dictionary with updated values for the given key-value pairs.
+    Supports nested dictionaries"""
     updated = deepcopy(dictionary)
 
     def traverse(d, key, value):
         s = key.split(".", 1)
         if len(s) > 1:
             if (s[0] not in d) or (not isinstance(d[s[0]], dict)):
                 d[s[0]] = {}
```

### Comparing `kedro_azureml-0.4.0/pyproject.toml` & `kedro_azureml-0.4.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kedro-azureml"
-version = "0.4.0"
+version = "0.4.1"
 description = "Kedro plugin with Azure ML Pipelines support"
 readme = "README.md"
 authors = ['marcin.zablocki <marcin.zablocki@getindata.com>']
 maintainers = ['GetInData MLOPS <mlops@getindata.com>']
 homepage = "https://github.com/getindata/kedro-azureml"
 repository = "https://github.com/getindata/kedro-azureml"
 documentation = "https://kedro-azureml.readthedocs.io/"
@@ -40,14 +40,15 @@
 azureml-mlflow = { version = ">=1.42.0", optional = true}
 pydantic = "~=1.9.1"
 mlflow = {version = "^1.27.0", optional = true}
 backoff = "^2.2.1"
 azure-core = ">=1.26.1"
 azureml-core = "^1.49.0"
 azureml-dataset-runtime = "^1.49.0"
+kedro-datasets = ">=1.0.0"
 
 [tool.poetry.extras]
 mlflow = ["azureml-mlflow", "mlflow"]
 
 [tool.poetry.dev-dependencies]
 pytest = "<7"
 pytest-cov = ">=2.8.0, <4.0.0"
```

### Comparing `kedro_azureml-0.4.0/PKG-INFO` & `kedro_azureml-0.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kedro-azureml
-Version: 0.4.0
+Version: 0.4.1
 Summary: Kedro plugin with Azure ML Pipelines support
 Home-page: https://github.com/getindata/kedro-azureml
 License: Apache-2.0
 Keywords: kedro,mlops,azureml,machinelearning
 Author: marcin.zablocki
 Author-email: marcin.zablocki@getindata.com
 Maintainer: GetInData MLOPS
@@ -22,14 +22,15 @@
 Requires-Dist: azure-core (>=1.26.1)
 Requires-Dist: azureml-core (>=1.49.0,<2.0.0)
 Requires-Dist: azureml-dataset-runtime (>=1.49.0,<2.0.0)
 Requires-Dist: azureml-mlflow (>=1.42.0) ; extra == "mlflow"
 Requires-Dist: backoff (>=2.2.1,<3.0.0)
 Requires-Dist: cloudpickle (>=2.1.0,<3.0.0)
 Requires-Dist: kedro (>=0.18.5,<0.19.0)
+Requires-Dist: kedro-datasets (>=1.0.0)
 Requires-Dist: mlflow (>=1.27.0,<2.0.0) ; extra == "mlflow"
 Requires-Dist: pydantic (>=1.9.1,<1.10.0)
 Project-URL: Documentation, https://kedro-azureml.readthedocs.io/
 Project-URL: Repository, https://github.com/getindata/kedro-azureml
 Description-Content-Type: text/markdown
 
 # Kedro Azure ML Pipelines plugin
```

#### html2text {}

```diff
@@ -1,40 +1,41 @@
-Metadata-Version: 2.1 Name: kedro-azureml Version: 0.4.0 Summary: Kedro plugin
+Metadata-Version: 2.1 Name: kedro-azureml Version: 0.4.1 Summary: Kedro plugin
 with Azure ML Pipelines support Home-page: https://github.com/getindata/kedro-
 azureml License: Apache-2.0 Keywords: kedro,mlops,azureml,machinelearning
 Author: marcin.zablocki Author-email: marcin.zablocki@getindata.com Maintainer:
 GetInData MLOPS Maintainer-email: mlops@getindata.com Requires-Python:
 >=3.8,<3.11 Classifier: Development Status :: 4 - Beta Classifier: License ::
 OSI Approved :: Apache Software License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Provides-Extra: mlflow Requires-Dist: adlfs (>=2022.2.0)
 Requires-Dist: azure-ai-ml (>=1.2.0) Requires-Dist: azure-core (>=1.26.1)
 Requires-Dist: azureml-core (>=1.49.0,<2.0.0) Requires-Dist: azureml-dataset-
 runtime (>=1.49.0,<2.0.0) Requires-Dist: azureml-mlflow (>=1.42.0) ; extra ==
 "mlflow" Requires-Dist: backoff (>=2.2.1,<3.0.0) Requires-Dist: cloudpickle
-(>=2.1.0,<3.0.0) Requires-Dist: kedro (>=0.18.5,<0.19.0) Requires-Dist: mlflow
-(>=1.27.0,<2.0.0) ; extra == "mlflow" Requires-Dist: pydantic (>=1.9.1,<1.10.0)
-Project-URL: Documentation, https://kedro-azureml.readthedocs.io/ Project-URL:
-Repository, https://github.com/getindata/kedro-azureml Description-Content-
-Type: text/markdown # Kedro Azure ML Pipelines plugin [![Python Version](https:
-//img.shields.io/pypi/pyversions/kedro-azureml)](https://github.com/getindata/
-kedro-azureml) [![License](https://img.shields.io/badge/license-Apache%202.0-
-blue.svg)](https://opensource.org/licenses/Apache-2.0) [![SemVer](https://
-img.shields.io/badge/semver-2.0.0-green)](https://semver.org/) [![PyPI version]
-(https://badge.fury.io/py/kedro-azureml.svg)](https://pypi.org/project/kedro-
-azureml/) [![Downloads](https://pepy.tech/badge/kedro-azureml)](https://
-pepy.tech/project/kedro-azureml) [![Maintainability Rating](https://
-sonarcloud.io/api/project_badges/measure?project=getindata_kedro-
-azureml&metric=sqale_rating)](https://sonarcloud.io/summary/
-new_code?id=getindata_kedro-azureml) [![Coverage](https://sonarcloud.io/api/
-project_badges/measure?project=getindata_kedro-azureml&metric=coverage)](https:
-//sonarcloud.io/summary/new_code?id=getindata_kedro-azureml) [![Documentation
-Status](https://readthedocs.org/projects/kedro-vertexai/badge/?version=latest)]
-(https://kedro-azureml.readthedocs.io/en/latest/?badge=latest)
+(>=2.1.0,<3.0.0) Requires-Dist: kedro (>=0.18.5,<0.19.0) Requires-Dist: kedro-
+datasets (>=1.0.0) Requires-Dist: mlflow (>=1.27.0,<2.0.0) ; extra == "mlflow"
+Requires-Dist: pydantic (>=1.9.1,<1.10.0) Project-URL: Documentation, https://
+kedro-azureml.readthedocs.io/ Project-URL: Repository, https://github.com/
+getindata/kedro-azureml Description-Content-Type: text/markdown # Kedro Azure
+ML Pipelines plugin [![Python Version](https://img.shields.io/pypi/pyversions/
+kedro-azureml)](https://github.com/getindata/kedro-azureml) [![License](https:/
+/img.shields.io/badge/license-Apache%202.0-blue.svg)](https://opensource.org/
+licenses/Apache-2.0) [![SemVer](https://img.shields.io/badge/semver-2.0.0-
+green)](https://semver.org/) [![PyPI version](https://badge.fury.io/py/kedro-
+azureml.svg)](https://pypi.org/project/kedro-azureml/) [![Downloads](https://
+pepy.tech/badge/kedro-azureml)](https://pepy.tech/project/kedro-azureml) [!
+[Maintainability Rating](https://sonarcloud.io/api/project_badges/
+measure?project=getindata_kedro-azureml&metric=sqale_rating)](https://
+sonarcloud.io/summary/new_code?id=getindata_kedro-azureml) [![Coverage](https:/
+/sonarcloud.io/api/project_badges/measure?project=getindata_kedro-
+azureml&metric=coverage)](https://sonarcloud.io/summary/
+new_code?id=getindata_kedro-azureml) [![Documentation Status](https://
+readthedocs.org/projects/kedro-vertexai/badge/?version=latest)](https://kedro-
+azureml.readthedocs.io/en/latest/?badge=latest)
                      [https://getindata.com/img/logo.svg]
             **** We help companies turn their data into assets ****
 ## About Following plugin enables running Kedro pipelines on Azure ML Pipelines
 service. We support 2 native Azure Machine Learning types of workflows: * For
 Data Scientists: fast, iterative development with code upload * For MLOps:
 stable, repeatable workflows with Docker ## Documentation For detailed
 documentation refer to https://kedro-azureml.readthedocs.io/ ## Usage guide ```
```

