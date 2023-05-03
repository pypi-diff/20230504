# Comparing `tmp/linkml_transformer-0.1.3.tar.gz` & `tmp/linkml_transformer-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linkml_transformer-0.1.3.tar", max compression
+gzip compressed data, was "linkml_transformer-0.1.4.tar", max compression
```

## Comparing `linkml_transformer-0.1.3.tar` & `linkml_transformer-0.1.4.tar`

### file list

```diff
@@ -1,27 +1,31 @@
--rw-r--r--   0        0        0     4047 2023-04-23 11:43:40.995420 linkml_transformer-0.1.3/README.md
--rw-r--r--   0        0        0      532 2023-04-23 11:44:20.391766 linkml_transformer-0.1.3/pyproject.toml
--rw-r--r--   0        0        0       22 2023-04-23 11:43:41.011420 linkml_transformer-0.1.3/src/linkml_transformer/__init__.py
--rw-r--r--   0        0        0        0 2023-04-23 11:43:41.011420 linkml_transformer-0.1.3/src/linkml_transformer/cli/__init__.py
--rw-r--r--   0        0        0     3834 2023-04-23 11:43:41.011420 linkml_transformer-0.1.3/src/linkml_transformer/cli/cli.py
--rw-r--r--   0        0        0        0 2023-04-23 11:43:41.011420 linkml_transformer-0.1.3/src/linkml_transformer/compiler/__init__.py
--rw-r--r--   0        0        0      486 2023-04-23 11:43:41.011420 linkml_transformer-0.1.3/src/linkml_transformer/compiler/awk_compiler.py
--rw-r--r--   0        0        0      848 2023-04-23 11:43:41.011420 linkml_transformer-0.1.3/src/linkml_transformer/compiler/compiler.py
--rw-r--r--   0        0        0      422 2023-04-23 11:43:41.011420 linkml_transformer-0.1.3/src/linkml_transformer/compiler/r2rml_compiler.py
--rw-r--r--   0        0        0      434 2023-04-23 11:43:41.011420 linkml_transformer-0.1.3/src/linkml_transformer/compiler/sparql_compiler.py
--rw-r--r--   0        0        0      450 2023-04-23 11:43:41.011420 linkml_transformer-0.1.3/src/linkml_transformer/compiler/sql_compiler.py
--rw-r--r--   0        0        0      499 2023-04-23 11:43:41.011420 linkml_transformer-0.1.3/src/linkml_transformer/compiler/sssom_compiler.py
--rw-r--r--   0        0        0      440 2023-04-23 11:43:41.011420 linkml_transformer-0.1.3/src/linkml_transformer/datamodel/specification_view.py
--rw-r--r--   0        0        0    31775 2023-04-23 11:43:41.011420 linkml_transformer-0.1.3/src/linkml_transformer/datamodel/transformer_model.py
--rw-r--r--   0        0        0     7478 2023-04-23 11:43:41.011420 linkml_transformer-0.1.3/src/linkml_transformer/datamodel/transformer_model.yaml
--rw-r--r--   0        0        0        0 2023-04-23 11:43:41.011420 linkml_transformer-0.1.3/src/linkml_transformer/importer/__init__.py
--rw-r--r--   0        0        0      723 2023-04-23 11:43:41.011420 linkml_transformer-0.1.3/src/linkml_transformer/importer/importer.py
--rw-r--r--   0        0        0        0 2023-04-23 11:43:41.011420 linkml_transformer-0.1.3/src/linkml_transformer/schema_mapper/__init__.py
--rw-r--r--   0        0        0     3487 2023-04-23 11:43:41.011420 linkml_transformer-0.1.3/src/linkml_transformer/schema_mapper/schema_mapper.py
--rw-r--r--   0        0        0        0 2023-04-23 11:43:41.011420 linkml_transformer-0.1.3/src/linkml_transformer/transformer/__init__.py
--rw-r--r--   0        0        0     6222 2023-04-23 11:43:41.011420 linkml_transformer-0.1.3/src/linkml_transformer/transformer/object_transformer.py
--rw-r--r--   0        0        0      436 2023-04-23 11:43:41.011420 linkml_transformer-0.1.3/src/linkml_transformer/transformer/rdflib_transformer.py
--rw-r--r--   0        0        0     3673 2023-04-23 11:43:41.011420 linkml_transformer-0.1.3/src/linkml_transformer/transformer/transformer.py
--rw-r--r--   0        0        0        0 2023-04-23 11:43:41.011420 linkml_transformer-0.1.3/src/linkml_transformer/utils/__init__.py
--rw-r--r--   0        0        0     1306 2023-04-23 11:43:41.011420 linkml_transformer-0.1.3/src/linkml_transformer/utils/dynamic_object.py
--rw-r--r--   0        0        0      235 2023-04-23 11:43:41.011420 linkml_transformer-0.1.3/src/linkml_transformer/utils/inverter.py
--rw-r--r--   0        0        0     4537 1970-01-01 00:00:00.000000 linkml_transformer-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     4047 2023-05-03 23:35:01.794835 linkml_transformer-0.1.4/README.md
+-rw-r--r--   0        0        0      742 2023-05-03 23:35:40.643670 linkml_transformer-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-05-03 23:35:01.806836 linkml_transformer-0.1.4/src/linkml_transformer/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-03 23:35:01.806836 linkml_transformer-0.1.4/src/linkml_transformer/cli/__init__.py
+-rw-r--r--   0        0        0     3627 2023-05-03 23:35:01.806836 linkml_transformer-0.1.4/src/linkml_transformer/cli/cli.py
+-rw-r--r--   0        0        0       61 2023-05-03 23:35:01.806836 linkml_transformer-0.1.4/src/linkml_transformer/compiler/__init__.py
+-rw-r--r--   0        0        0      463 2023-05-03 23:35:01.806836 linkml_transformer-0.1.4/src/linkml_transformer/compiler/awk_compiler.py
+-rw-r--r--   0        0        0     1124 2023-05-03 23:35:01.806836 linkml_transformer-0.1.4/src/linkml_transformer/compiler/compiler.py
+-rw-r--r--   0        0        0     2353 2023-05-03 23:35:01.806836 linkml_transformer-0.1.4/src/linkml_transformer/compiler/python_compiler.py
+-rw-r--r--   0        0        0      399 2023-05-03 23:35:01.806836 linkml_transformer-0.1.4/src/linkml_transformer/compiler/r2rml_compiler.py
+-rw-r--r--   0        0        0      411 2023-05-03 23:35:01.806836 linkml_transformer-0.1.4/src/linkml_transformer/compiler/sparql_compiler.py
+-rw-r--r--   0        0        0      427 2023-05-03 23:35:01.806836 linkml_transformer-0.1.4/src/linkml_transformer/compiler/sql_compiler.py
+-rw-r--r--   0        0        0      476 2023-05-03 23:35:01.806836 linkml_transformer-0.1.4/src/linkml_transformer/compiler/sssom_compiler.py
+-rw-r--r--   0        0        0      480 2023-05-03 23:35:01.806836 linkml_transformer-0.1.4/src/linkml_transformer/datamodel/specification_view.py
+-rw-r--r--   0        0        0    12387 2023-05-03 23:35:01.806836 linkml_transformer-0.1.4/src/linkml_transformer/datamodel/transformer_model.py
+-rw-r--r--   0        0        0     7874 2023-05-03 23:35:01.806836 linkml_transformer-0.1.4/src/linkml_transformer/datamodel/transformer_model.yaml
+-rw-r--r--   0        0        0        0 2023-05-03 23:35:01.806836 linkml_transformer-0.1.4/src/linkml_transformer/importer/__init__.py
+-rw-r--r--   0        0        0      642 2023-05-03 23:35:01.806836 linkml_transformer-0.1.4/src/linkml_transformer/importer/importer.py
+-rw-r--r--   0        0        0        0 2023-05-03 23:35:01.806836 linkml_transformer-0.1.4/src/linkml_transformer/schema_mapper/__init__.py
+-rw-r--r--   0        0        0     5265 2023-05-03 23:35:01.806836 linkml_transformer-0.1.4/src/linkml_transformer/schema_mapper/schema_mapper.py
+-rw-r--r--   0        0        0        0 2023-05-03 23:35:01.806836 linkml_transformer-0.1.4/src/linkml_transformer/transformer/__init__.py
+-rw-r--r--   0        0        0     1373 2023-05-03 23:35:01.806836 linkml_transformer-0.1.4/src/linkml_transformer/transformer/inference.py
+-rw-r--r--   0        0        0     6691 2023-05-03 23:35:01.806836 linkml_transformer-0.1.4/src/linkml_transformer/transformer/object_transformer.py
+-rw-r--r--   0        0        0      247 2023-05-03 23:35:01.806836 linkml_transformer-0.1.4/src/linkml_transformer/transformer/rdflib_transformer.py
+-rw-r--r--   0        0        0     5753 2023-05-03 23:35:01.810835 linkml_transformer-0.1.4/src/linkml_transformer/transformer/transformer.py
+-rw-r--r--   0        0        0        0 2023-05-03 23:35:01.810835 linkml_transformer-0.1.4/src/linkml_transformer/utils/__init__.py
+-rw-r--r--   0        0        0     1306 2023-05-03 23:35:01.810835 linkml_transformer-0.1.4/src/linkml_transformer/utils/dynamic_object.py
+-rw-r--r--   0        0        0      242 2023-05-03 23:35:01.810835 linkml_transformer-0.1.4/src/linkml_transformer/utils/inverter.py
+-rw-r--r--   0        0        0      783 2023-05-03 23:35:01.810835 linkml_transformer-0.1.4/src/linkml_transformer/utils/loaders.py
+-rw-r--r--   0        0        0     9492 2023-05-03 23:35:01.810835 linkml_transformer-0.1.4/src/linkml_transformer/utils/multi_file_transformer.py
+-rw-r--r--   0        0        0     4530 1970-01-01 00:00:00.000000 linkml_transformer-0.1.4/PKG-INFO
```

### Comparing `linkml_transformer-0.1.3/README.md` & `linkml_transformer-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `linkml_transformer-0.1.3/src/linkml_transformer/cli/cli.py` & `linkml_transformer-0.1.4/src/linkml_transformer/cli/cli.py`

 * *Files 17% similar despite different names*

```diff
@@ -7,18 +7,15 @@
 __all__ = [
     "main",
 ]
 
 import yaml
 from linkml_runtime import SchemaView
 from linkml_runtime.dumpers import yaml_dumper
-from linkml_runtime.loaders import yaml_loader
 
-from linkml_transformer.datamodel.transformer_model import \
-    TransformationSpecification
 from linkml_transformer.schema_mapper.schema_mapper import SchemaMapper
 from linkml_transformer.transformer.object_transformer import ObjectTransformer
 
 schema_option = click.option("-s", "--schema", help="Path to source schema.")
 transformer_specification_option = click.option(
     "-T", "--transformer-specification", help="Path to transformer specification."
 )
@@ -70,31 +67,27 @@
     source_type,
     transformer_specification,
     output,
     output_format,
     **kwargs,
 ):
     """Map data in a source schema using a transformation."""
-    logging.info(
-        f"Transforming {input} conforming to {schema} using {transformer_specification}"
-    )
+    logging.info(f"Transforming {input} conforming to {schema} using {transformer_specification}")
     tr = ObjectTransformer()
     tr.source_schemaview = SchemaView(schema)
-    tr.specification = yaml_loader.load(
-        transformer_specification, target_class=TransformationSpecification
-    )
+    tr.load_transformer_specification(transformer_specification)
     with open(input) as file:
         input_obj = yaml.safe_load(file)
     tr.index(input_obj, source_type)
     tr_obj = tr.transform(input_obj, source_type)
     if output:
-        file = open(output, "w", encoding="utf-8")
+        outfile = open(output, "w", encoding="utf-8")
     else:
-        file = sys.stdout
-    file.write(yaml_dumper.dumps(tr_obj))
+        outfile = sys.stdout
+    outfile.write(yaml_dumper.dumps(tr_obj))
 
 
 @main.command()
 @output_option
 @transformer_specification_option
 @output_format_options
 @click.argument("schema")
@@ -110,22 +103,21 @@
         linkml, e.g. there may be "dangling" references.
 
     Example:
 
         linkml-tr derive-schema -T transform/personinfo-to-agent.transform.yaml source/personinfo.yaml
     """
     logging.info(f"Transforming {schema} using {transformer_specification}")
-    tr = SchemaMapper()
-    tr.source_schemaview = SchemaView(schema)
-    specification = yaml_loader.load(
-        transformer_specification, target_class=TransformationSpecification
-    )
-    target_schema = tr.derive_schema(specification)
+    tr = ObjectTransformer()
+    tr.load_transformer_specification(transformer_specification)
+    mapper = SchemaMapper(transformer=tr)
+    mapper.source_schemaview = SchemaView(schema)
+    target_schema = mapper.derive_schema()
     if output:
-        file = open(output, "w", encoding="utf-8")
+        outfile = open(output, "w", encoding="utf-8")
     else:
-        file = sys.stdout
-    file.write(yaml_dumper.dumps(target_schema))
+        outfile = sys.stdout
+    outfile.write(yaml_dumper.dumps(target_schema))
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `linkml_transformer-0.1.3/src/linkml_transformer/datamodel/transformer_model.yaml` & `linkml_transformer-0.1.4/src/linkml_transformer/datamodel/transformer_model.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,17 @@
       id:
         identifier: true
         description: Unique identifier for this transformation specification
       title:
         description: human readable title for this transformation specification
       prefixes:
         description: maps prefixes to URL expansions
+        range: KeyVal
+        multivalued: true
+        inlined: true
       source_schema:
         description: name of the schema that describes the source (input) objects
       target_schema:
         description: name of the schema that describes the target (output) objects
       class_derivations:
         description: >-
           Instructions on how to derive a set of classes in the target schema
@@ -73,14 +76,19 @@
       name:
         key: true
         description: Name of the element in the target schema
       copy_directives:
         range: CopyDirective
         multivalued: true
         inlined: true
+      overrides:
+        description: overrides source schema slots
+        range: Any
+        #multivalued: true
+        #inlined: true
       is_a:
         range: ElementDerivation
       mixins:
         range: ElementDerivation
         multivalued: true
         inlined: true
       value_mappings:
@@ -104,17 +112,17 @@
 
 
   ClassDerivation:
     is_a: ElementDerivation
     description: >-
       A specification of how to derive a target class from a source class.
     attributes:
-      name:
-        key: true
-        description: Name of the class in the target schema
+      #name:
+      #  key: true
+      #  description: Name of the class in the target schema
       populated_from:
         range: string
         description: Name of the class in the source schema
       joins:
         range: AliasedClass
         multivalued: true
         inlined: true
@@ -146,14 +154,17 @@
         range: string
         description: Source slot name
       expr:
         range: string
         description: >-
           An expression to be evaluated on the source object to derive the target slot.
           Should be specified using the LinkML expression language.
+      range:
+        slot_uri: linkml:range
+        range: string
       inverse_of:
         range: Inverse
         description: >-
           Used to specify a class-slot tuple that is the inverse of the derived/target slot.
           This is used primarily for mapping to relational databases or formalisms that do
           not allow multiple values. The class representing the repeated element has a foreign
           key slot inserted in that 'back references' the original multivalued slot.
@@ -223,14 +234,16 @@
     attributes:
       key:
         key: true
       value:
         range: Any
 
   CopyDirective:
+    description: >-
+      Instructs a Schema Mapper in how to map to a target schema. Not used for data transformation.
     attributes:
       element_name:
         key: true
       copy_all:
         range: boolean
       exclude_all:
         range: boolean
```

### Comparing `linkml_transformer-0.1.3/src/linkml_transformer/importer/importer.py` & `linkml_transformer-0.1.4/src/linkml_transformer/importer/importer.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,12 @@
-from abc import ABC
+from abc import ABC, abstractmethod
 from dataclasses import dataclass
 from typing import Any
 
-from linkml_runtime import SchemaView
-from linkml_runtime.utils.yamlutils import YAMLRoot
-
-from linkml_transformer.datamodel.transformer_model import \
-    TransformationSpecification
+from linkml_transformer.datamodel.transformer_model import TransformationSpecification
 
 
 @dataclass
 class Importer(ABC):
     """
     Base class for all importers.
```

### Comparing `linkml_transformer-0.1.3/src/linkml_transformer/schema_mapper/schema_mapper.py` & `linkml_transformer-0.1.4/src/linkml_transformer/schema_mapper/schema_mapper.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,62 +1,86 @@
+import logging
+from collections import defaultdict
 from copy import copy
-from dataclasses import dataclass
+from dataclasses import dataclass, field
+from typing import Dict, List, Optional
 
 from linkml_runtime import SchemaView
-from linkml_runtime.linkml_model import (ClassDefinition, Element,
-                                         SchemaDefinition, SlotDefinition)
+from linkml_runtime.linkml_model import (
+    ClassDefinition,
+    ClassDefinitionName,
+    Element,
+    SchemaDefinition,
+    SlotDefinition,
+)
 
 from linkml_transformer.datamodel.transformer_model import (
-    ClassDerivation, CopyDirective, TransformationSpecification)
+    ClassDerivation,
+    CopyDirective,
+    TransformationSpecification,
+)
+from linkml_transformer.transformer.transformer import Transformer
 
 
 @dataclass
 class SchemaMapper:
     """
     Translates a source schema and transformation specification into a target schema.
     """
 
     source_schemaview: SchemaView = None
 
+    transformer: Transformer = None
+
+    source_to_target_class_mappings: Dict[str, List[str]] = field(
+        default_factory=lambda: defaultdict(list)
+    )
+
     def derive_schema(
-        self, specification: TransformationSpecification
+        self, specification: Optional[TransformationSpecification] = None
     ) -> SchemaDefinition:
         """
-        Compile a transformation specification into a schema.
+        Use a transformation specification to generate a target/profile schema from a source schema.
 
         :param specification:
         :return:
         """
+        if specification is None:
+            specification = self.transformer.specification
         source_schemaview = self.source_schemaview
         source_schema = source_schemaview.schema
         target_schema = SchemaDefinition(id=source_schema.id, name=source_schema.name)
         for class_derivation in specification.class_derivations.values():
             class_definition = self._derive_class(class_derivation)
             target_schema.classes[class_definition.name] = class_definition
+        for cd in target_schema.classes.values():
+            self._rewire_class(cd)
         return target_schema
 
     def _derive_class(self, class_derivation: ClassDerivation) -> ClassDefinition:
         """
         Derive a class from a class derivation.
         """
         populated_from = class_derivation.populated_from
         if not populated_from:
             populated_from = class_derivation.name
         source_class = self.source_schemaview.get_class(populated_from)
         if source_class is None:
+            logging.warning(f"No such class {populated_from}")
             target_class = ClassDefinition(name=class_derivation.name)
         else:
             target_class = copy(source_class)
             target_class.name = class_derivation.name
             target_class.slots = []
             target_class.attributes = {}
             target_class.slot_usage = {}
         for slot_derivation in class_derivation.slot_derivations.values():
             slot_definition = self._derive_slot(slot_derivation)
             target_class.attributes[slot_definition.name] = slot_definition
+        self.source_to_target_class_mappings[populated_from].append(target_class.name)
         return target_class
 
     def _derive_slot(self, slot_derivation) -> SlotDefinition:
         """
         Derive a slot from a slot derivation.
         """
         populated_from = slot_derivation.populated_from
@@ -66,14 +90,36 @@
         if source_slot is None:
             target_slot = SlotDefinition(name=slot_derivation.name)
         else:
             target_slot = copy(source_slot)
             target_slot.name = slot_derivation.name
         return target_slot
 
+    def _rewire_class(self, class_definition: ClassDefinition):
+        if class_definition.is_a:
+            class_definition.is_a = self._rewire_parent(class_definition, class_definition.is_a)
+        mixins = [self._rewire_parent(class_definition, m) for m in class_definition.mixins]
+        class_definition.mixins = [m for m in mixins if m is not None]
+
+    def _rewire_parent(
+        self, class_definition: ClassDefinition, parent: ClassDefinitionName
+    ) -> Optional[str]:
+        if parent in self.source_to_target_class_mappings:
+            new_parents = self.source_to_target_class_mappings[parent]
+            if len(new_parents) > 1:
+                raise ValueError(
+                    f"Cannot rewire to non-isomorphic mappings {parent} => {new_parents}"
+                )
+            if len(new_parents) == 1:
+                return new_parents[0]
+        parent_cls = self.source_schemaview.get_class(parent)
+        if parent_cls.is_a:
+            return self._rewire_parent(class_definition, parent_cls.is_a)
+        return None
+
     def copy_attributes(
         self,
         target_element: Element,
         source_element: Element,
         copy_directive: CopyDirective,
     ) -> None:
         """
```

### Comparing `linkml_transformer-0.1.3/src/linkml_transformer/transformer/object_transformer.py` & `linkml_transformer-0.1.4/src/linkml_transformer/transformer/object_transformer.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,102 +4,99 @@
 
 from linkml_runtime.index.object_index import ObjectIndex
 from linkml_runtime.utils.eval_utils import eval_expr
 from linkml_runtime.utils.yamlutils import YAMLRoot
 from pydantic import BaseModel
 
 from linkml_transformer.transformer.transformer import OBJECT_TYPE, Transformer
-from linkml_transformer.utils.dynamic_object import DynObj, dynamic_object
+from linkml_transformer.utils.dynamic_object import dynamic_object
 
 DICT_OBJ = Dict[str, Any]
 
 
 logger = logging.getLogger(__name__)
 
 
 @dataclass
 class ObjectTransformer(Transformer):
     """
     A Transformer that works on in-memory dict objects.
 
-    This works by recursively
+    This works recursively
     """
 
     object_index: ObjectIndex = None
 
     def index(self, source_obj: Any, target: str = None):
         """
         Create an index over a container object.
 
-        :param source_obj:
-        :return:
+        :param source_obj: source data structure to be indexed
+        :param target: class to convert source object into
         """
         if isinstance(source_obj, dict):
             if target is None:
                 [target] = [
-                    c.name
-                    for c in self.source_schemaview.all_classes().values()
-                    if c.tree_root
+                    c.name for c in self.source_schemaview.all_classes().values() if c.tree_root
                 ]
             if target is None:
-                raise ValueError(
-                    f"target must be passed if source_obj is dict: {source_obj}"
-                )
-            source_obj_typed = dynamic_object(
-                source_obj, self.source_schemaview, target
-            )
-            self.object_index = ObjectIndex(
-                source_obj_typed, schemaview=self.source_schemaview
-            )
+                raise ValueError(f"target must be passed if source_obj is dict: {source_obj}")
+            source_obj_typed = dynamic_object(source_obj, self.source_schemaview, target)
+            self.object_index = ObjectIndex(source_obj_typed, schemaview=self.source_schemaview)
         else:
-            self.object_index = ObjectIndex(
-                source_obj, schemaview=self.source_schemaview
-            )
+            self.object_index = ObjectIndex(source_obj, schemaview=self.source_schemaview)
 
     def transform(
         self,
         source_obj: OBJECT_TYPE,
         source_type: str = None,
-    ) -> DICT_OBJ:
+        target_type: str = None,
+    ) -> Union[DICT_OBJ, Any]:
         """
         Transform a source object into a target object.
 
         :param source_obj:
         :param source_type:
         :return:
         """
         sv = self.source_schemaview
         if source_type is None:
             [source_type] = [c.name for c in sv.all_classes().values() if c.tree_root]
         if source_type in sv.all_types():
-            # TODO: type derivations
+            if target_type:
+                if target_type == "string":
+                    return str(source_obj)
+                elif target_type == "integer":
+                    return int(source_obj)
+                elif target_type == "float" or target_type == "double":
+                    return float(source_obj)
+                elif target_type == "uri":
+                    return self.expand_curie(source_obj)
+                elif target_type == "curie":
+                    return self.compress_uri(source_obj)
             return source_obj
         if source_type in sv.all_enums():
             # TODO: enum derivations
             return str(source_obj)
         if isinstance(source_obj, (BaseModel, YAMLRoot)):
             source_obj_typed = source_obj
             source_obj = vars(source_obj)
         else:
             source_obj_typed = None
         if not isinstance(source_obj, dict):
             logger.warning(f"Unexpected: {source_obj} for type {source_type}")
             return source_obj
-        source_type_class = sv.get_class(source_type)
         class_deriv = self._get_class_derivation(source_type)
         tgt_attrs = {}
         for slot_derivation in class_deriv.slot_derivations.values():
             v = None
             source_class_slot = None
-            target_class_slot = None
             if slot_derivation.populated_from:
                 v = source_obj.get(slot_derivation.populated_from, None)
-                source_class_slot = sv.induced_slot(
-                    slot_derivation.populated_from, source_type
-                )
+                source_class_slot = sv.induced_slot(slot_derivation.populated_from, source_type)
                 logger.debug(
                     f"Pop slot {slot_derivation.name} => {v} using {slot_derivation.populated_from} // {source_obj}"
                 )
             elif slot_derivation.expr:
                 if self.object_index:
                     if not source_obj_typed:
                         source_obj_dyn = dynamic_object(source_obj, sv, source_type)
@@ -108,35 +105,41 @@
                     ctxt_obj = self.object_index.bless(source_obj_dyn)
                     ctxt_dict = {
                         k: getattr(ctxt_obj, k)
                         for k in ctxt_obj._attributes()
                         if not k.startswith("_")
                     }
                 else:
-                    # ctxt_dict = source_obj
                     do = dynamic_object(source_obj, sv, source_type)
                     ctxt_dict = vars(do)
                 v = eval_expr(slot_derivation.expr, **ctxt_dict, NULL=None)
             else:
                 source_class_slot = sv.induced_slot(slot_derivation.name, source_type)
                 v = source_obj.get(slot_derivation.name, None)
             if source_class_slot and v is not None:
+                target_range = slot_derivation.range
                 source_class_slot_range = source_class_slot.range
                 if source_class_slot.multivalued:
                     if isinstance(v, list):
-                        v = [self.transform(v1, source_class_slot_range) for v1 in v]
+                        v = [self.transform(v1, source_class_slot_range, target_range) for v1 in v]
                     elif isinstance(v, dict):
-                        v = [self.transform(v1, source_class_slot_range) for v1 in v]
+                        v = [self.transform(v1, source_class_slot_range, target_range) for v1 in v]
                     else:
                         v = [v]
                 else:
-                    v = self.transform(v, source_class_slot_range)
-                if self._coerce_to_multivalued(slot_derivation, class_deriv) and v is not None and not isinstance(v, list):
+                    v = self.transform(v, source_class_slot_range, target_range)
+                if (
+                    self._coerce_to_multivalued(slot_derivation, class_deriv)
+                    and v is not None
+                    and not isinstance(v, list)
+                ):
                     v = [v]
-                if self._coerce_to_singlevalued(slot_derivation, class_deriv) and isinstance(v, list):
+                if self._coerce_to_singlevalued(slot_derivation, class_deriv) and isinstance(
+                    v, list
+                ):
                     if len(v) > 1:
                         raise ValueError(f"Cannot coerce multiple values {v}")
                     if len(v) == 0:
                         v = None
                     else:
                         v = v[0]
             tgt_attrs[str(slot_derivation.name)] = v
@@ -153,8 +156,7 @@
         #    source_obj_dict = json_dumper.to_dict(source_obj)
         # elif isinstance(source_obj, BaseModel):
         #    source_obj_dict = source_obj.dict()
         # else:
         #    raise ValueError(f"Do not know how to handle type: {typ}")
         tr_obj_dict = self.transform(source_obj, typ_name)
         return target_class(**tr_obj_dict)
-
```

### Comparing `linkml_transformer-0.1.3/src/linkml_transformer/utils/dynamic_object.py` & `linkml_transformer-0.1.4/src/linkml_transformer/utils/dynamic_object.py`

 * *Files identical despite different names*

### Comparing `linkml_transformer-0.1.3/PKG-INFO` & `linkml_transformer-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: linkml-transformer
-Version: 0.1.3
+Version: 0.1.4
 Summary: 
 Author: cmungall
 Author-email: cjm@berkeleybop.org
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: linkml-runtime (>=1.4.5,<2.0.0)
+Requires-Dist: linkml-runtime (>=1.5.2)
 Description-Content-Type: text/markdown
 
 # linkml-transformer
 
 __Status__: pre-alpha code
 
 See [these slides](https://docs.google.com/presentation/d/1ctgT1IfwPjnFQO2Q0sYlM8qk0wiB2_32JyeKyN4Uf8k/edit)
```

