# Comparing `tmp/kpops-1.1.2.tar.gz` & `tmp/kpops-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kpops-1.1.2.tar", max compression
+gzip compressed data, was "kpops-1.1.3.tar", max compression
```

## Comparing `kpops-1.1.2.tar` & `kpops-1.1.3.tar`

### file list

```diff
@@ -1,63 +1,63 @@
--rw-r--r--   0        0        0     1064 2023-04-27 14:18:20.378846 kpops-1.1.2/LICENSE
--rw-r--r--   0        0        0     2370 2023-04-27 14:18:20.378846 kpops-1.1.2/README.md
--rw-r--r--   0        0        0       22 2023-04-27 14:19:03.610898 kpops-1.1.2/kpops/__init__.py
--rw-r--r--   0        0        0        0 2023-04-27 14:18:20.382846 kpops-1.1.2/kpops/cli/__init__.py
--rw-r--r--   0        0        0      761 2023-04-27 14:18:20.382846 kpops-1.1.2/kpops/cli/custom_formatter.py
--rw-r--r--   0        0        0      122 2023-04-27 14:18:20.382846 kpops-1.1.2/kpops/cli/exception.py
--rw-r--r--   0        0        0    11739 2023-04-27 14:18:20.382846 kpops-1.1.2/kpops/cli/main.py
--rw-r--r--   0        0        0     4206 2023-04-27 14:18:20.382846 kpops-1.1.2/kpops/cli/pipeline_config.py
--rw-r--r--   0        0        0     1711 2023-04-27 14:18:20.382846 kpops-1.1.2/kpops/cli/registry.py
--rw-r--r--   0        0        0      688 2023-04-27 14:18:20.382846 kpops-1.1.2/kpops/component_handlers/__init__.py
--rw-r--r--   0        0        0        0 2023-04-27 14:18:20.382846 kpops-1.1.2/kpops/component_handlers/helm_wrapper/__init__.py
--rw-r--r--   0        0        0       52 2023-04-27 14:18:20.382846 kpops-1.1.2/kpops/component_handlers/helm_wrapper/exception.py
--rw-r--r--   0        0        0     9357 2023-04-27 14:18:20.382846 kpops-1.1.2/kpops/component_handlers/helm_wrapper/helm.py
--rw-r--r--   0        0        0     2152 2023-04-27 14:18:20.382846 kpops-1.1.2/kpops/component_handlers/helm_wrapper/helm_diff.py
--rw-r--r--   0        0        0     4373 2023-04-27 14:18:20.382846 kpops-1.1.2/kpops/component_handlers/helm_wrapper/model.py
--rw-r--r--   0        0        0      667 2023-04-27 14:18:20.382846 kpops-1.1.2/kpops/component_handlers/helm_wrapper/utils.py
--rw-r--r--   0        0        0        0 2023-04-27 14:18:20.382846 kpops-1.1.2/kpops/component_handlers/kafka_connect/__init__.py
--rw-r--r--   0        0        0     8202 2023-04-27 14:18:20.382846 kpops-1.1.2/kpops/component_handlers/kafka_connect/connect_wrapper.py
--rw-r--r--   0        0        0      182 2023-04-27 14:18:20.382846 kpops-1.1.2/kpops/component_handlers/kafka_connect/exception.py
--rw-r--r--   0        0        0     5890 2023-04-27 14:18:20.382846 kpops-1.1.2/kpops/component_handlers/kafka_connect/kafka_connect_handler.py
--rw-r--r--   0        0        0     1851 2023-04-27 14:18:20.382846 kpops-1.1.2/kpops/component_handlers/kafka_connect/model.py
--rw-r--r--   0        0        0      788 2023-04-27 14:18:20.382846 kpops-1.1.2/kpops/component_handlers/kafka_connect/timeout.py
--rw-r--r--   0        0        0        0 2023-04-27 14:18:20.382846 kpops-1.1.2/kpops/component_handlers/schema_handler/__init__.py
--rw-r--r--   0        0        0     6035 2023-04-27 14:18:20.382846 kpops-1.1.2/kpops/component_handlers/schema_handler/schema_handler.py
--rw-r--r--   0        0        0      361 2023-04-27 14:18:20.382846 kpops-1.1.2/kpops/component_handlers/schema_handler/schema_provider.py
--rw-r--r--   0        0        0        0 2023-04-27 14:18:20.382846 kpops-1.1.2/kpops/component_handlers/topic/__init__.py
--rw-r--r--   0        0        0      180 2023-04-27 14:18:20.382846 kpops-1.1.2/kpops/component_handlers/topic/exception.py
--rw-r--r--   0        0        0     9588 2023-04-27 14:18:20.382846 kpops-1.1.2/kpops/component_handlers/topic/handler.py
--rw-r--r--   0        0        0     2503 2023-04-27 14:18:20.382846 kpops-1.1.2/kpops/component_handlers/topic/model.py
--rw-r--r--   0        0        0     6937 2023-04-27 14:18:20.382846 kpops-1.1.2/kpops/component_handlers/topic/proxy_wrapper.py
--rw-r--r--   0        0        0     2385 2023-04-27 14:18:20.382846 kpops-1.1.2/kpops/component_handlers/topic/utils.py
--rw-r--r--   0        0        0        0 2023-04-27 14:18:20.382846 kpops-1.1.2/kpops/component_handlers/utils/__init__.py
--rw-r--r--   0        0        0      630 2023-04-27 14:18:20.382846 kpops-1.1.2/kpops/component_handlers/utils/exception.py
--rw-r--r--   0        0        0      492 2023-04-27 14:18:20.382846 kpops-1.1.2/kpops/components/__init__.py
--rw-r--r--   0        0        0      466 2023-04-27 14:18:20.382846 kpops-1.1.2/kpops/components/base_components/__init__.py
--rw-r--r--   0        0        0     8321 2023-04-27 14:18:20.382846 kpops-1.1.2/kpops/components/base_components/base_defaults_component.py
--rw-r--r--   0        0        0     7457 2023-04-27 14:18:20.382846 kpops-1.1.2/kpops/components/base_components/kafka_app.py
--rw-r--r--   0        0        0    16472 2023-04-27 14:18:20.382846 kpops-1.1.2/kpops/components/base_components/kafka_connector.py
--rw-r--r--   0        0        0     6775 2023-04-27 14:18:20.386846 kpops-1.1.2/kpops/components/base_components/kubernetes_app.py
--rw-r--r--   0        0        0        0 2023-04-27 14:18:20.386846 kpops-1.1.2/kpops/components/base_components/models/__init__.py
--rw-r--r--   0        0        0     2447 2023-04-27 14:18:20.386846 kpops-1.1.2/kpops/components/base_components/models/from_section.py
--rw-r--r--   0        0        0     3272 2023-04-27 14:18:20.386846 kpops-1.1.2/kpops/components/base_components/models/to_section.py
--rw-r--r--   0        0        0    11398 2023-04-27 14:18:20.386846 kpops-1.1.2/kpops/components/base_components/pipeline_component.py
--rw-r--r--   0        0        0      211 2023-04-27 14:18:20.386846 kpops-1.1.2/kpops/components/streams_bootstrap/__init__.py
--rw-r--r--   0        0        0      217 2023-04-27 14:18:20.386846 kpops-1.1.2/kpops/components/streams_bootstrap/app_type.py
--rw-r--r--   0        0        0        0 2023-04-27 14:18:20.386846 kpops-1.1.2/kpops/components/streams_bootstrap/producer/__init__.py
--rw-r--r--   0        0        0     1116 2023-04-27 14:18:20.386846 kpops-1.1.2/kpops/components/streams_bootstrap/producer/model.py
--rw-r--r--   0        0        0     2859 2023-04-27 14:18:20.386846 kpops-1.1.2/kpops/components/streams_bootstrap/producer/producer_app.py
--rw-r--r--   0        0        0        0 2023-04-27 14:18:20.386846 kpops-1.1.2/kpops/components/streams_bootstrap/streams/__init__.py
--rw-r--r--   0        0        0     9097 2023-04-27 14:18:20.386846 kpops-1.1.2/kpops/components/streams_bootstrap/streams/model.py
--rw-r--r--   0        0        0     4080 2023-04-27 14:18:20.386846 kpops-1.1.2/kpops/components/streams_bootstrap/streams/streams_app.py
--rw-r--r--   0        0        0        0 2023-04-27 14:18:20.386846 kpops-1.1.2/kpops/pipeline_generator/__init__.py
--rw-r--r--   0        0        0    10755 2023-04-27 14:18:20.386846 kpops-1.1.2/kpops/pipeline_generator/pipeline.py
--rw-r--r--   0        0        0        0 2023-04-27 14:18:20.386846 kpops-1.1.2/kpops/utils/__init__.py
--rw-r--r--   0        0        0      289 2023-04-27 14:18:20.386846 kpops-1.1.2/kpops/utils/colorify.py
--rw-r--r--   0        0        0     3043 2023-04-27 14:18:20.386846 kpops-1.1.2/kpops/utils/dict_differ.py
--rw-r--r--   0        0        0     2589 2023-04-27 14:18:20.386846 kpops-1.1.2/kpops/utils/docstring.py
--rw-r--r--   0        0        0     5808 2023-04-27 14:18:20.386846 kpops-1.1.2/kpops/utils/gen_schema.py
--rw-r--r--   0        0        0      594 2023-04-27 14:18:20.386846 kpops-1.1.2/kpops/utils/pydantic.py
--rw-r--r--   0        0        0     1189 2023-04-27 14:18:20.386846 kpops-1.1.2/kpops/utils/yaml_loading.py
--rw-r--r--   0        0        0     1892 2023-04-27 14:19:03.590898 kpops-1.1.2/pyproject.toml
--rw-r--r--   0        0        0     3948 1970-01-01 00:00:00.000000 kpops-1.1.2/setup.py
--rw-r--r--   0        0        0     3965 1970-01-01 00:00:00.000000 kpops-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-05-04 10:29:54.081526 kpops-1.1.3/LICENSE
+-rw-r--r--   0        0        0     2370 2023-05-04 10:29:54.081526 kpops-1.1.3/README.md
+-rw-r--r--   0        0        0       22 2023-05-04 10:30:21.117893 kpops-1.1.3/kpops/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:29:54.085526 kpops-1.1.3/kpops/cli/__init__.py
+-rw-r--r--   0        0        0      761 2023-05-04 10:29:54.085526 kpops-1.1.3/kpops/cli/custom_formatter.py
+-rw-r--r--   0        0        0      122 2023-05-04 10:29:54.085526 kpops-1.1.3/kpops/cli/exception.py
+-rw-r--r--   0        0        0    11727 2023-05-04 10:29:54.085526 kpops-1.1.3/kpops/cli/main.py
+-rw-r--r--   0        0        0     4206 2023-05-04 10:29:54.085526 kpops-1.1.3/kpops/cli/pipeline_config.py
+-rw-r--r--   0        0        0     1711 2023-05-04 10:29:54.085526 kpops-1.1.3/kpops/cli/registry.py
+-rw-r--r--   0        0        0      688 2023-05-04 10:29:54.085526 kpops-1.1.3/kpops/component_handlers/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:29:54.085526 kpops-1.1.3/kpops/component_handlers/helm_wrapper/__init__.py
+-rw-r--r--   0        0        0       52 2023-05-04 10:29:54.085526 kpops-1.1.3/kpops/component_handlers/helm_wrapper/exception.py
+-rw-r--r--   0        0        0     9357 2023-05-04 10:29:54.085526 kpops-1.1.3/kpops/component_handlers/helm_wrapper/helm.py
+-rw-r--r--   0        0        0     2152 2023-05-04 10:29:54.085526 kpops-1.1.3/kpops/component_handlers/helm_wrapper/helm_diff.py
+-rw-r--r--   0        0        0     4373 2023-05-04 10:29:54.085526 kpops-1.1.3/kpops/component_handlers/helm_wrapper/model.py
+-rw-r--r--   0        0        0      667 2023-05-04 10:29:54.085526 kpops-1.1.3/kpops/component_handlers/helm_wrapper/utils.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:29:54.085526 kpops-1.1.3/kpops/component_handlers/kafka_connect/__init__.py
+-rw-r--r--   0        0        0     8202 2023-05-04 10:29:54.085526 kpops-1.1.3/kpops/component_handlers/kafka_connect/connect_wrapper.py
+-rw-r--r--   0        0        0      182 2023-05-04 10:29:54.085526 kpops-1.1.3/kpops/component_handlers/kafka_connect/exception.py
+-rw-r--r--   0        0        0     5890 2023-05-04 10:29:54.085526 kpops-1.1.3/kpops/component_handlers/kafka_connect/kafka_connect_handler.py
+-rw-r--r--   0        0        0     1851 2023-05-04 10:29:54.085526 kpops-1.1.3/kpops/component_handlers/kafka_connect/model.py
+-rw-r--r--   0        0        0      788 2023-05-04 10:29:54.085526 kpops-1.1.3/kpops/component_handlers/kafka_connect/timeout.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:29:54.085526 kpops-1.1.3/kpops/component_handlers/schema_handler/__init__.py
+-rw-r--r--   0        0        0     6035 2023-05-04 10:29:54.085526 kpops-1.1.3/kpops/component_handlers/schema_handler/schema_handler.py
+-rw-r--r--   0        0        0      361 2023-05-04 10:29:54.085526 kpops-1.1.3/kpops/component_handlers/schema_handler/schema_provider.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:29:54.085526 kpops-1.1.3/kpops/component_handlers/topic/__init__.py
+-rw-r--r--   0        0        0      180 2023-05-04 10:29:54.085526 kpops-1.1.3/kpops/component_handlers/topic/exception.py
+-rw-r--r--   0        0        0     9588 2023-05-04 10:29:54.085526 kpops-1.1.3/kpops/component_handlers/topic/handler.py
+-rw-r--r--   0        0        0     2503 2023-05-04 10:29:54.085526 kpops-1.1.3/kpops/component_handlers/topic/model.py
+-rw-r--r--   0        0        0     6937 2023-05-04 10:29:54.085526 kpops-1.1.3/kpops/component_handlers/topic/proxy_wrapper.py
+-rw-r--r--   0        0        0     2385 2023-05-04 10:29:54.085526 kpops-1.1.3/kpops/component_handlers/topic/utils.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:29:54.085526 kpops-1.1.3/kpops/component_handlers/utils/__init__.py
+-rw-r--r--   0        0        0      630 2023-05-04 10:29:54.085526 kpops-1.1.3/kpops/component_handlers/utils/exception.py
+-rw-r--r--   0        0        0      492 2023-05-04 10:29:54.085526 kpops-1.1.3/kpops/components/__init__.py
+-rw-r--r--   0        0        0      466 2023-05-04 10:29:54.085526 kpops-1.1.3/kpops/components/base_components/__init__.py
+-rw-r--r--   0        0        0     8321 2023-05-04 10:29:54.085526 kpops-1.1.3/kpops/components/base_components/base_defaults_component.py
+-rw-r--r--   0        0        0     7457 2023-05-04 10:29:54.085526 kpops-1.1.3/kpops/components/base_components/kafka_app.py
+-rw-r--r--   0        0        0    16472 2023-05-04 10:29:54.085526 kpops-1.1.3/kpops/components/base_components/kafka_connector.py
+-rw-r--r--   0        0        0     6775 2023-05-04 10:29:54.085526 kpops-1.1.3/kpops/components/base_components/kubernetes_app.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:29:54.085526 kpops-1.1.3/kpops/components/base_components/models/__init__.py
+-rw-r--r--   0        0        0     2447 2023-05-04 10:29:54.085526 kpops-1.1.3/kpops/components/base_components/models/from_section.py
+-rw-r--r--   0        0        0     3272 2023-05-04 10:29:54.085526 kpops-1.1.3/kpops/components/base_components/models/to_section.py
+-rw-r--r--   0        0        0    11398 2023-05-04 10:29:54.085526 kpops-1.1.3/kpops/components/base_components/pipeline_component.py
+-rw-r--r--   0        0        0      211 2023-05-04 10:29:54.085526 kpops-1.1.3/kpops/components/streams_bootstrap/__init__.py
+-rw-r--r--   0        0        0      217 2023-05-04 10:29:54.085526 kpops-1.1.3/kpops/components/streams_bootstrap/app_type.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:29:54.085526 kpops-1.1.3/kpops/components/streams_bootstrap/producer/__init__.py
+-rw-r--r--   0        0        0     1116 2023-05-04 10:29:54.089526 kpops-1.1.3/kpops/components/streams_bootstrap/producer/model.py
+-rw-r--r--   0        0        0     2859 2023-05-04 10:29:54.089526 kpops-1.1.3/kpops/components/streams_bootstrap/producer/producer_app.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:29:54.089526 kpops-1.1.3/kpops/components/streams_bootstrap/streams/__init__.py
+-rw-r--r--   0        0        0     9097 2023-05-04 10:29:54.089526 kpops-1.1.3/kpops/components/streams_bootstrap/streams/model.py
+-rw-r--r--   0        0        0     4080 2023-05-04 10:29:54.089526 kpops-1.1.3/kpops/components/streams_bootstrap/streams/streams_app.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:29:54.089526 kpops-1.1.3/kpops/pipeline_generator/__init__.py
+-rw-r--r--   0        0        0    10755 2023-05-04 10:29:54.089526 kpops-1.1.3/kpops/pipeline_generator/pipeline.py
+-rw-r--r--   0        0        0        0 2023-05-04 10:29:54.089526 kpops-1.1.3/kpops/utils/__init__.py
+-rw-r--r--   0        0        0      289 2023-05-04 10:29:54.089526 kpops-1.1.3/kpops/utils/colorify.py
+-rw-r--r--   0        0        0     3043 2023-05-04 10:29:54.089526 kpops-1.1.3/kpops/utils/dict_differ.py
+-rw-r--r--   0        0        0     2589 2023-05-04 10:29:54.089526 kpops-1.1.3/kpops/utils/docstring.py
+-rw-r--r--   0        0        0     5808 2023-05-04 10:29:54.089526 kpops-1.1.3/kpops/utils/gen_schema.py
+-rw-r--r--   0        0        0      594 2023-05-04 10:29:54.089526 kpops-1.1.3/kpops/utils/pydantic.py
+-rw-r--r--   0        0        0     1189 2023-05-04 10:29:54.089526 kpops-1.1.3/kpops/utils/yaml_loading.py
+-rw-r--r--   0        0        0     1892 2023-05-04 10:30:21.105893 kpops-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0     3948 1970-01-01 00:00:00.000000 kpops-1.1.3/setup.py
+-rw-r--r--   0        0        0     3965 1970-01-01 00:00:00.000000 kpops-1.1.3/PKG-INFO
```

### Comparing `kpops-1.1.2/LICENSE` & `kpops-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `kpops-1.1.2/README.md` & `kpops-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `kpops-1.1.2/kpops/cli/custom_formatter.py` & `kpops-1.1.3/kpops/cli/custom_formatter.py`

 * *Files identical despite different names*

### Comparing `kpops-1.1.2/kpops/cli/main.py` & `kpops-1.1.3/kpops/cli/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,17 +21,15 @@
 from kpops.utils.gen_schema import SchemaScope, gen_config_schema, gen_pipeline_schema
 
 if TYPE_CHECKING:
     from kpops.components.base_components import PipelineComponent
 
 LOG_DIVIDER = "#" * 100
 
-app = typer.Typer(
-    pretty_exceptions_show_locals=False,
-)
+app = typer.Typer(pretty_exceptions_enable=False)
 
 BASE_DIR_PATH_OPTION: Path = typer.Option(
     default=Path("."),
     exists=True,
     dir_okay=True,
     file_okay=False,
     envvar=f"{ENV_PREFIX}PIPELINE_BASE_DIR",
```

### Comparing `kpops-1.1.2/kpops/cli/pipeline_config.py` & `kpops-1.1.3/kpops/cli/pipeline_config.py`

 * *Files identical despite different names*

### Comparing `kpops-1.1.2/kpops/cli/registry.py` & `kpops-1.1.3/kpops/cli/registry.py`

 * *Files identical despite different names*

### Comparing `kpops-1.1.2/kpops/component_handlers/__init__.py` & `kpops-1.1.3/kpops/component_handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `kpops-1.1.2/kpops/component_handlers/helm_wrapper/helm.py` & `kpops-1.1.3/kpops/component_handlers/helm_wrapper/helm.py`

 * *Files identical despite different names*

### Comparing `kpops-1.1.2/kpops/component_handlers/helm_wrapper/helm_diff.py` & `kpops-1.1.3/kpops/component_handlers/helm_wrapper/helm_diff.py`

 * *Files identical despite different names*

### Comparing `kpops-1.1.2/kpops/component_handlers/helm_wrapper/model.py` & `kpops-1.1.3/kpops/component_handlers/helm_wrapper/model.py`

 * *Files identical despite different names*

### Comparing `kpops-1.1.2/kpops/component_handlers/helm_wrapper/utils.py` & `kpops-1.1.3/kpops/component_handlers/helm_wrapper/utils.py`

 * *Files identical despite different names*

### Comparing `kpops-1.1.2/kpops/component_handlers/kafka_connect/connect_wrapper.py` & `kpops-1.1.3/kpops/component_handlers/kafka_connect/connect_wrapper.py`

 * *Files identical despite different names*

### Comparing `kpops-1.1.2/kpops/component_handlers/kafka_connect/kafka_connect_handler.py` & `kpops-1.1.3/kpops/component_handlers/kafka_connect/kafka_connect_handler.py`

 * *Files identical despite different names*

### Comparing `kpops-1.1.2/kpops/component_handlers/kafka_connect/model.py` & `kpops-1.1.3/kpops/component_handlers/kafka_connect/model.py`

 * *Files identical despite different names*

### Comparing `kpops-1.1.2/kpops/component_handlers/kafka_connect/timeout.py` & `kpops-1.1.3/kpops/component_handlers/kafka_connect/timeout.py`

 * *Files identical despite different names*

### Comparing `kpops-1.1.2/kpops/component_handlers/schema_handler/schema_handler.py` & `kpops-1.1.3/kpops/component_handlers/schema_handler/schema_handler.py`

 * *Files identical despite different names*

### Comparing `kpops-1.1.2/kpops/component_handlers/topic/handler.py` & `kpops-1.1.3/kpops/component_handlers/topic/handler.py`

 * *Files identical despite different names*

### Comparing `kpops-1.1.2/kpops/component_handlers/topic/model.py` & `kpops-1.1.3/kpops/component_handlers/topic/model.py`

 * *Files identical despite different names*

### Comparing `kpops-1.1.2/kpops/component_handlers/topic/proxy_wrapper.py` & `kpops-1.1.3/kpops/component_handlers/topic/proxy_wrapper.py`

 * *Files identical despite different names*

### Comparing `kpops-1.1.2/kpops/component_handlers/topic/utils.py` & `kpops-1.1.3/kpops/component_handlers/topic/utils.py`

 * *Files identical despite different names*

### Comparing `kpops-1.1.2/kpops/component_handlers/utils/exception.py` & `kpops-1.1.3/kpops/component_handlers/utils/exception.py`

 * *Files identical despite different names*

### Comparing `kpops-1.1.2/kpops/components/base_components/base_defaults_component.py` & `kpops-1.1.3/kpops/components/base_components/base_defaults_component.py`

 * *Files identical despite different names*

### Comparing `kpops-1.1.2/kpops/components/base_components/kafka_app.py` & `kpops-1.1.3/kpops/components/base_components/kafka_app.py`

 * *Files identical despite different names*

### Comparing `kpops-1.1.2/kpops/components/base_components/kafka_connector.py` & `kpops-1.1.3/kpops/components/base_components/kafka_connector.py`

 * *Files identical despite different names*

### Comparing `kpops-1.1.2/kpops/components/base_components/kubernetes_app.py` & `kpops-1.1.3/kpops/components/base_components/kubernetes_app.py`

 * *Files identical despite different names*

### Comparing `kpops-1.1.2/kpops/components/base_components/models/from_section.py` & `kpops-1.1.3/kpops/components/base_components/models/from_section.py`

 * *Files identical despite different names*

### Comparing `kpops-1.1.2/kpops/components/base_components/models/to_section.py` & `kpops-1.1.3/kpops/components/base_components/models/to_section.py`

 * *Files identical despite different names*

### Comparing `kpops-1.1.2/kpops/components/base_components/pipeline_component.py` & `kpops-1.1.3/kpops/components/base_components/pipeline_component.py`

 * *Files identical despite different names*

### Comparing `kpops-1.1.2/kpops/components/streams_bootstrap/producer/model.py` & `kpops-1.1.3/kpops/components/streams_bootstrap/producer/model.py`

 * *Files identical despite different names*

### Comparing `kpops-1.1.2/kpops/components/streams_bootstrap/producer/producer_app.py` & `kpops-1.1.3/kpops/components/streams_bootstrap/producer/producer_app.py`

 * *Files identical despite different names*

### Comparing `kpops-1.1.2/kpops/components/streams_bootstrap/streams/model.py` & `kpops-1.1.3/kpops/components/streams_bootstrap/streams/model.py`

 * *Files identical despite different names*

### Comparing `kpops-1.1.2/kpops/components/streams_bootstrap/streams/streams_app.py` & `kpops-1.1.3/kpops/components/streams_bootstrap/streams/streams_app.py`

 * *Files identical despite different names*

### Comparing `kpops-1.1.2/kpops/pipeline_generator/pipeline.py` & `kpops-1.1.3/kpops/pipeline_generator/pipeline.py`

 * *Files identical despite different names*

### Comparing `kpops-1.1.2/kpops/utils/dict_differ.py` & `kpops-1.1.3/kpops/utils/dict_differ.py`

 * *Files identical despite different names*

### Comparing `kpops-1.1.2/kpops/utils/docstring.py` & `kpops-1.1.3/kpops/utils/docstring.py`

 * *Files identical despite different names*

### Comparing `kpops-1.1.2/kpops/utils/gen_schema.py` & `kpops-1.1.3/kpops/utils/gen_schema.py`

 * *Files identical despite different names*

### Comparing `kpops-1.1.2/kpops/utils/pydantic.py` & `kpops-1.1.3/kpops/utils/pydantic.py`

 * *Files identical despite different names*

### Comparing `kpops-1.1.2/kpops/utils/yaml_loading.py` & `kpops-1.1.3/kpops/utils/yaml_loading.py`

 * *Files identical despite different names*

### Comparing `kpops-1.1.2/pyproject.toml` & `kpops-1.1.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kpops"
-version = "1.1.2"
+version = "1.1.3"
 description = "KPOps is a tool to deploy Kafka pipelines to Kubernetes"
 authors = ["bakdata <opensource@bakdata.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/bakdata/kpops"
 documentation = "https://bakdata.github.io/kpops/latest"
 keywords = ["kafka", "kubernetes", "stream-processing", "pipelines"]
```

### Comparing `kpops-1.1.2/setup.py` & `kpops-1.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
  'typer[all]>=0.6.1,<0.7.0']
 
 entry_points = \
 {'console_scripts': ['kpops = kpops.cli.main:app']}
 
 setup_kwargs = {
     'name': 'kpops',
-    'version': '1.1.2',
+    'version': '1.1.3',
     'description': 'KPOps is a tool to deploy Kafka pipelines to Kubernetes',
     'long_description': '# KPOps\n\n[![Build status](https://github.com/bakdata/kpops/actions/workflows/ci.yaml/badge.svg)](https://github.com/bakdata/kpops/actions/workflows/ci.yaml)\n[![pypi](https://img.shields.io/pypi/v/kpops.svg)](https://pypi.org/project/kpops)\n[![versions](https://img.shields.io/pypi/pyversions/kpops.svg)](https://github.com/bakdata/kpops)\n[![license](https://img.shields.io/github/license/bakdata/kpops.svg)](https://github.com/bakdata/kpops/blob/main/LICENSE)\n\n## Key features\n\n- **Deploy Kafka apps to Kubernetes**: KPOps allows to deploy consecutive Kafka Streams applications and producers using an easy-to-read and -write pipeline definition.\n- **Manage Kafka Connectors**: KPOps connects with your Kafka Connect cluster and deploys, validates, and deletes your connectors.\n- **Configure multiple pipelines and steps**: KPOps has various abstractions that simplify configuring multiple pipelines and steps within pipelines by sharing common configuration between different components, such as producers or streaming applications.\n- **Handle your topics and schemas**: KPOps not only creates and deletes your topics but also registers and deletes your schemas.\n- **Clean termination of Kafka components**: KPOps removes your pipeline components (i.e., Kafka Streams applications) from the Kubernetes cluster _and_ cleans up the component-related states (i.e., removing/resetting offset of Kafka consumer groups).\n- **Preview your pipeline changes**: With the KPOps dry-run, you can ensure your pipeline definition is set up correctly. This helps to minimize downtime and prevent potential errors or issues that could impact your production environment.\n\n## Documentation\n\nFor detailed usage and installation instructions, check out\nthe [documentation](https://bakdata.github.io/kpops/latest/user/what-is-kpops/).\n\n## Install KPOps\n\nKPOps comes as a [PyPI package](https://pypi.org/project/kpops/). \nYou can install it with [pip](https://github.com/pypa/pip):\n\n```shell\npip install kpops\n```\n\n## Contributing\n\nWe are happy if you want to contribute to this project.\nIf you find any bugs or have suggestions for improvements, please open an issue.\nWe are also happy to accept your PRs.\nJust open an issue beforehand and let us know what you want to do and why.\n\n## License\n\nKPOps is licensed under the [MIT License](https://github.com/bakdata/kpops/blob/main/LICENSE).\n',
     'author': 'bakdata',
     'author_email': 'opensource@bakdata.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/bakdata/kpops',
```

### Comparing `kpops-1.1.2/PKG-INFO` & `kpops-1.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kpops
-Version: 1.1.2
+Version: 1.1.3
 Summary: KPOps is a tool to deploy Kafka pipelines to Kubernetes
 Home-page: https://github.com/bakdata/kpops
 License: MIT
 Keywords: kafka,kubernetes,stream-processing,pipelines
 Author: bakdata
 Author-email: opensource@bakdata.com
 Requires-Python: >=3.10,<4.0
```

