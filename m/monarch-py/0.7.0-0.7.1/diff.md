# Comparing `tmp/monarch_py-0.7.0.tar.gz` & `tmp/monarch_py-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monarch_py-0.7.0.tar", max compression
+gzip compressed data, was "monarch_py-0.7.1.tar", max compression
```

## Comparing `monarch_py-0.7.0.tar` & `monarch_py-0.7.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0      955 2023-05-03 19:21:04.825506 monarch_py-0.7.0/pyproject.toml
--rw-r--r--   0        0        0       77 2023-05-03 19:21:04.825506 monarch_py-0.7.0/src/monarch_py/__init__.py
--rw-r--r--   0        0        0     1587 2023-05-03 19:21:04.825506 monarch_py-0.7.0/src/monarch_py/association_type_mappings.yaml
--rw-r--r--   0        0        0     6347 2023-05-03 19:21:04.825506 monarch_py-0.7.0/src/monarch_py/cli.py
--rw-r--r--   0        0        0        0 2023-05-03 19:21:04.829506 monarch_py-0.7.0/src/monarch_py/datamodels/__init__.py
--rw-r--r--   0        0        0     7976 2023-05-03 19:21:04.829506 monarch_py-0.7.0/src/monarch_py/datamodels/model.py
--rw-r--r--   0        0        0     7215 2023-05-03 19:21:04.829506 monarch_py-0.7.0/src/monarch_py/datamodels/model.yaml
--rw-r--r--   0        0        0     3300 2023-05-03 19:21:04.829506 monarch_py-0.7.0/src/monarch_py/datamodels/solr.py
--rw-r--r--   0        0        0        0 2023-05-03 19:21:04.829506 monarch_py-0.7.0/src/monarch_py/implementations/__init__.py
--rw-r--r--   0        0        0        0 2023-05-03 19:21:04.829506 monarch_py-0.7.0/src/monarch_py/implementations/solr/__init__.py
--rw-r--r--   0        0        0    16913 2023-05-03 19:21:04.829506 monarch_py-0.7.0/src/monarch_py/implementations/solr/solr_implementation.py
--rw-r--r--   0        0        0        0 2023-05-03 19:21:04.829506 monarch_py-0.7.0/src/monarch_py/implementations/sql/__init__.py
--rw-r--r--   0        0        0     8909 2023-05-03 19:21:04.829506 monarch_py-0.7.0/src/monarch_py/implementations/sql/sql_implementation.py
--rw-r--r--   0        0        0        0 2023-05-03 19:21:04.829506 monarch_py-0.7.0/src/monarch_py/interfaces/__init__.py
--rw-r--r--   0        0        0     2343 2023-05-03 19:21:04.829506 monarch_py-0.7.0/src/monarch_py/interfaces/association_interface.py
--rw-r--r--   0        0        0      985 2023-05-03 19:21:04.829506 monarch_py-0.7.0/src/monarch_py/interfaces/entity_interface.py
--rw-r--r--   0        0        0      890 2023-05-03 19:21:04.829506 monarch_py-0.7.0/src/monarch_py/interfaces/query_interface.py
--rw-r--r--   0        0        0     3737 2023-05-03 19:21:04.829506 monarch_py-0.7.0/src/monarch_py/interfaces/search_interface.py
--rw-r--r--   0        0        0        0 2023-05-03 19:21:04.829506 monarch_py-0.7.0/src/monarch_py/service/__init__.py
--rw-r--r--   0        0        0     2052 2023-05-03 19:21:04.829506 monarch_py-0.7.0/src/monarch_py/service/solr_service.py
--rw-r--r--   0        0        0     9114 2023-05-03 19:21:04.829506 monarch_py-0.7.0/src/monarch_py/solr_cli.py
--rw-r--r--   0        0        0     3792 2023-05-03 19:21:04.829506 monarch_py-0.7.0/src/monarch_py/sql_cli.py
--rw-r--r--   0        0        0        0 2023-05-03 19:21:04.829506 monarch_py-0.7.0/src/monarch_py/utils/__init__.py
--rw-r--r--   0        0        0     4052 2023-05-03 19:21:04.829506 monarch_py-0.7.0/src/monarch_py/utils/association_type_utils.py
--rw-r--r--   0        0        0     3959 2023-05-03 19:21:04.829506 monarch_py-0.7.0/src/monarch_py/utils/solr_cli_utils.py
--rw-r--r--   0        0        0     4469 2023-05-03 19:21:04.829506 monarch_py-0.7.0/src/monarch_py/utils/utils.py
--rw-r--r--   0        0        0      711 1970-01-01 00:00:00.000000 monarch_py-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0      955 2023-05-04 00:46:19.213279 monarch_py-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0       77 2023-05-04 00:46:19.213279 monarch_py-0.7.1/src/monarch_py/__init__.py
+-rw-r--r--   0        0        0     1587 2023-05-04 00:46:19.213279 monarch_py-0.7.1/src/monarch_py/association_type_mappings.yaml
+-rw-r--r--   0        0        0     6581 2023-05-04 00:46:19.213279 monarch_py-0.7.1/src/monarch_py/cli.py
+-rw-r--r--   0        0        0        0 2023-05-04 00:46:19.213279 monarch_py-0.7.1/src/monarch_py/datamodels/__init__.py
+-rw-r--r--   0        0        0     8251 2023-05-04 00:46:19.213279 monarch_py-0.7.1/src/monarch_py/datamodels/model.py
+-rw-r--r--   0        0        0     7319 2023-05-04 00:46:19.213279 monarch_py-0.7.1/src/monarch_py/datamodels/model.yaml
+-rw-r--r--   0        0        0     3300 2023-05-04 00:46:19.213279 monarch_py-0.7.1/src/monarch_py/datamodels/solr.py
+-rw-r--r--   0        0        0        0 2023-05-04 00:46:19.213279 monarch_py-0.7.1/src/monarch_py/implementations/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-04 00:46:19.213279 monarch_py-0.7.1/src/monarch_py/implementations/solr/__init__.py
+-rw-r--r--   0        0        0    17565 2023-05-04 00:46:19.213279 monarch_py-0.7.1/src/monarch_py/implementations/solr/solr_implementation.py
+-rw-r--r--   0        0        0        0 2023-05-04 00:46:19.213279 monarch_py-0.7.1/src/monarch_py/implementations/sql/__init__.py
+-rw-r--r--   0        0        0     8909 2023-05-04 00:46:19.213279 monarch_py-0.7.1/src/monarch_py/implementations/sql/sql_implementation.py
+-rw-r--r--   0        0        0        0 2023-05-04 00:46:19.213279 monarch_py-0.7.1/src/monarch_py/interfaces/__init__.py
+-rw-r--r--   0        0        0     2343 2023-05-04 00:46:19.213279 monarch_py-0.7.1/src/monarch_py/interfaces/association_interface.py
+-rw-r--r--   0        0        0      985 2023-05-04 00:46:19.213279 monarch_py-0.7.1/src/monarch_py/interfaces/entity_interface.py
+-rw-r--r--   0        0        0      890 2023-05-04 00:46:19.213279 monarch_py-0.7.1/src/monarch_py/interfaces/query_interface.py
+-rw-r--r--   0        0        0     3737 2023-05-04 00:46:19.213279 monarch_py-0.7.1/src/monarch_py/interfaces/search_interface.py
+-rw-r--r--   0        0        0        0 2023-05-04 00:46:19.213279 monarch_py-0.7.1/src/monarch_py/service/__init__.py
+-rw-r--r--   0        0        0     2052 2023-05-04 00:46:19.213279 monarch_py-0.7.1/src/monarch_py/service/solr_service.py
+-rw-r--r--   0        0        0     8133 2023-05-04 00:46:19.213279 monarch_py-0.7.1/src/monarch_py/solr_cli.py
+-rw-r--r--   0        0        0     3330 2023-05-04 00:46:19.213279 monarch_py-0.7.1/src/monarch_py/sql_cli.py
+-rw-r--r--   0        0        0        0 2023-05-04 00:46:19.213279 monarch_py-0.7.1/src/monarch_py/utils/__init__.py
+-rw-r--r--   0        0        0     4052 2023-05-04 00:46:19.213279 monarch_py-0.7.1/src/monarch_py/utils/association_type_utils.py
+-rw-r--r--   0        0        0     3964 2023-05-04 00:46:19.217279 monarch_py-0.7.1/src/monarch_py/utils/solr_cli_utils.py
+-rw-r--r--   0        0        0     4937 2023-05-04 00:46:19.217279 monarch_py-0.7.1/src/monarch_py/utils/utils.py
+-rw-r--r--   0        0        0      711 1970-01-01 00:00:00.000000 monarch_py-0.7.1/PKG-INFO
```

### Comparing `monarch_py-0.7.0/pyproject.toml` & `monarch_py-0.7.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "monarch-py"
-version = "0.7.0"
+version = "0.7.1"
 description = "Monarch Initiative data access library"
 authors = [
     "Kevin Schaper <kevin@tislab.org>",
     "Glass Elsarboukh <glass@tislab.org>",
     "The Monarch Initiative <info@monarchinitiative.org>"
 ]
 packages = [
```

### Comparing `monarch_py-0.7.0/src/monarch_py/association_type_mappings.yaml` & `monarch_py-0.7.1/src/monarch_py/association_type_mappings.yaml`

 * *Files identical despite different names*

### Comparing `monarch_py-0.7.0/src/monarch_py/cli.py` & `monarch_py-0.7.1/src/monarch_py/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -38,26 +38,29 @@
 ### "Aliases" for Solr CLI ###
 
 
 @app.command("entity")
 def entity(
     id: str = typer.Argument(None, help="The identifier of the entity to be retrieved"),
     fmt: str = typer.Option(
-        "json", "--format", "-f", help="The format of the output (TSV, YAML, JSON)"
+        "json",
+        "--format",
+        "-f",
+        help="The format of the output (json, yaml, tsv, table)",
     ),
     output: str = typer.Option(
         None, "--output", "-o", help="The path to the output file"
     ),
 ):
     """
     Retrieve an entity by ID
 
     Args:
         id: The identifier of the entity to be retrieved
-        fmt: The format of the output (TSV, YAML, JSON)
+        fmt: The format of the output (json, yaml, tsv, table)
         output: The path to the output file (stdout if not specified)
 
     """
     solr_cli.entity(**locals())
 
 
 @app.command("associations")
@@ -69,15 +72,18 @@
     entity: str = typer.Option(None, "--entity", "-e"),
     between: str = typer.Option(None, "--between"),
     direct: bool = typer.Option(False, "--direct"),
     association_type: str = typer.Option(None, "--label"),
     limit: int = typer.Option(20, "--limit", "-l"),
     offset: int = typer.Option(0, "--offset"),
     fmt: str = typer.Option(
-        "json", "--format", "-f", help="The format of the output (TSV, YAML, JSON)"
+        "json",
+        "--format",
+        "-f",
+        help="The format of the output (json, yaml, tsv, table)",
     ),
     output: str = typer.Option(
         None, "--output", "-o", help="The path to the output file"
     ),
 ):
     """
     Paginate through associations
@@ -89,110 +95,122 @@
         object: The object of the association
         entity: The subject or object of the association
         between: The subject and object of the association
         association_type: The label of the association
         limit: The number of associations to return
         direct: Whether to exclude associations with subject/object as ancestors
         offset: The offset of the first association to be retrieved
-        fmt: The format of the output (TSV, YAML, JSON)
+        fmt: The format of the output (json, yaml, tsv, table)
         output: The path to the output file (stdout if not specified)
     """
     solr_cli.associations(**locals())
 
 
 @app.command("search")
 def search(
     q: str = typer.Option(None, "--query", "-q"),
     category: str = typer.Option(None, "--category"),
     taxon: str = typer.Option(None, "--taxon"),
     limit: int = typer.Option(20, "--limit"),
     offset: int = typer.Option(0, "--offset"),
     fmt: str = typer.Option(
-        "json", "--format", "-f", help="The format of the output (TSV, YAML, JSON)"
+        "json",
+        "--format",
+        "-f",
+        help="The format of the output (json, yaml, tsv, table)",
     ),
     output: str = typer.Option(
         None, "--output", "-o", help="The path to the output file"
     ),
 ):
     """
     Search for entities
 
     Args:
         q: The query string to search for
         category: The category of the entity
         taxon: The taxon of the entity
         limit: The number of entities to return
         offset: The offset of the first entity to be retrieved
-        fmt: The format of the output (TSV, YAML, JSON)
+        fmt: The format of the output (json, yaml, tsv, table)
         output: The path to the output file (stdout if not specified)
     """
     solr_cli.search(**locals())
 
 
 @app.command("autocomplete")
 def autocomplete(
     q: str = typer.Argument(None, help="Query string to autocomplete against"),
     fmt: str = typer.Option(
-        "json", "--format", "-f", help="The format of the output (TSV, YAML, JSON)"
+        "json",
+        "--format",
+        "-f",
+        help="The format of the output (json, yaml, tsv, table)",
     ),
     output: str = typer.Option(
         None, "--output", "-o", help="The path to the output file"
     ),
 ):
     """
     Return entity autcomplete matches for a query string
 
     Args:
         q: The query string to autocomplete against
-        fmt: The format of the output (TSV, YAML, JSON)
+        fmt: The format of the output (json, yaml, tsv, table)
         output: The path to the output file (stdout if not specified)
 
     """
     solr_cli.autocomplete(**locals())
 
 
 @app.command("histopheno")
 def histopheno(
     subject: str = typer.Argument(None, help="The subject of the association"),
     fmt: str = typer.Option(
-        "json", "--format", "-f", help="The format of the output (TSV, YAML, JSON)"
+        "json",
+        "--format",
+        "-f",
+        help="The format of the output (json, yaml, tsv, table)",
     ),
     output: str = typer.Option(
         None, "--output", "-o", help="The path to the output file"
     ),
 ):
     """
     Retrieve the histopheno data for an entity by ID
 
     Args:
         subject: The subject of the association
 
     Optional Args:
-        fmt (str): The format of the output (TSV, YAML, JSON). Default JSON
+        fmt (str): The format of the output (json, yaml, tsv, table). Default JSON
         output (str): The path to the output file. Default stdout
     """
     solr_cli.histopheno(**locals())
 
 
 @app.command("association-counts")
 def association_counts(
     entity: str = typer.Argument(None, help="The entity to get association counts for"),
     fmt: str = typer.Option(
-        "json", "--format", "-f", help="The format of the output (TSV, YAML, JSON)"
+        "json",
+        "--format",
+        "-f",
+        help="The format of the output (json, yaml, tsv, table)",
     ),
     output: str = typer.Option(
         None, "--output", "-o", help="The path to the output file"
     ),
 ):
     """
     Retrieve association counts for an entity by ID
 
     Args:
         entity: The entity to get association counts for
-        fmt: The format of the output (TSV, YAML, JSON). Default JSON
+        fmt: The format of the output (json, yaml, tsv, table). Default JSON
         output: The path to the output file. Default stdout
 
     Returns:
         A list of association counts for the given entity containing association type, label and count
     """
     solr_cli.association_counts(**locals())
```

### Comparing `monarch_py-0.7.0/src/monarch_py/datamodels/model.py` & `monarch_py-0.7.1/src/monarch_py/datamodels/model.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,50 +1,46 @@
 from __future__ import annotations
-
+from datetime import datetime, date
 from enum import Enum
-from typing import Dict, List, Optional
-
-from pydantic import BaseModel as BaseModel
-from pydantic import Field
+from typing import List, Dict, Optional, Any, Union, Literal
+from pydantic import BaseModel as BaseModel, Field
+from linkml_runtime.linkml_model import Decimal
 
 metamodel_version = "None"
 version = "None"
 
-
 class WeakRefShimBaseModel(BaseModel):
-    __slots__ = "__weakref__"
-
-
-class ConfiguredBaseModel(
-    WeakRefShimBaseModel,
-    validate_assignment=True,
-    validate_all=True,
-    underscore_attrs_are_private=True,
-    extra="forbid",
-    arbitrary_types_allowed=True,
-):
-    pass
+   __slots__ = '__weakref__'
+    
+class ConfiguredBaseModel(WeakRefShimBaseModel,
+                validate_assignment = True, 
+                validate_all = True, 
+                underscore_attrs_are_private = True, 
+                extra = 'forbid', 
+                arbitrary_types_allowed = True):
+    pass                    
 
 
 class AssociationTypeEnum(str, Enum):
-
+    
     disease_phenotype = "disease_phenotype"
     gene_phenotype = "gene_phenotype"
     gene_interaction = "gene_interaction"
     gene_pathway = "gene_pathway"
     gene_expression = "gene_expression"
     gene_orthology = "gene_orthology"
     chemical_pathway = "chemical_pathway"
     gene_function = "gene_function"
     correlated_gene = "correlated_gene"
     causal_gene = "causal_gene"
-
+    
+    
 
 class Association(ConfiguredBaseModel):
-
+    
     aggregator_knowledge_source: Optional[List[str]] = Field(default_factory=list)
     id: Optional[str] = Field(None)
     subject: Optional[str] = Field(None)
     original_subject: Optional[str] = Field(None)
     subject_namespace: Optional[str] = Field(None)
     subject_category: Optional[List[str]] = Field(default_factory=list)
     subject_closure: Optional[List[str]] = Field(default_factory=list)
@@ -68,167 +64,156 @@
     has_evidence: Optional[str] = Field(None)
     onset_qualifier: Optional[str] = Field(None)
     sex_qualifier: Optional[str] = Field(None)
     source: Optional[str] = Field(None)
     stage_qualifier: Optional[str] = Field(None)
     pathway: Optional[str] = Field(None)
     relation: Optional[str] = Field(None)
+    
 
 
 class Entity(ConfiguredBaseModel):
-
+    
     id: Optional[str] = Field(None)
     category: Optional[List[str]] = Field(default_factory=list)
     name: Optional[str] = Field(None)
     description: Optional[str] = Field(None)
     xref: Optional[List[str]] = Field(default_factory=list)
     provided_by: Optional[str] = Field(None)
     in_taxon: Optional[str] = Field(None)
     source: Optional[str] = Field(None)
     symbol: Optional[str] = Field(None)
     type: Optional[str] = Field(None)
     synonym: Optional[List[str]] = Field(default_factory=list)
+    
 
 
 class HistoPheno(ConfiguredBaseModel):
-
+    
     id: Optional[str] = Field(None)
-    items: Optional[List[AssociationCount]] = Field(
-        default_factory=list,
-        description="""A collection of items, with the type to be overriden by slot_usage""",
-    )
+    items: Optional[List[HistoBin]] = Field(default_factory=list, description="""A collection of items, with the type to be overriden by slot_usage""")
+    
 
 
 class Results(ConfiguredBaseModel):
-
+    
     limit: Optional[int] = Field(None)
     offset: Optional[int] = Field(None)
     total: Optional[int] = Field(None)
+    
 
 
 class AssociationResults(Results):
-
-    items: Optional[List[Association]] = Field(
-        default_factory=list,
-        description="""A collection of items, with the type to be overriden by slot_usage""",
-    )
+    
+    items: Optional[List[Association]] = Field(default_factory=list, description="""A collection of items, with the type to be overriden by slot_usage""")
     limit: Optional[int] = Field(None)
     offset: Optional[int] = Field(None)
     total: Optional[int] = Field(None)
+    
 
 
 class EntityResults(Results):
-
-    items: Optional[List[Entity]] = Field(
-        default_factory=list,
-        description="""A collection of items, with the type to be overriden by slot_usage""",
-    )
+    
+    items: Optional[List[Entity]] = Field(default_factory=list, description="""A collection of items, with the type to be overriden by slot_usage""")
     limit: Optional[int] = Field(None)
     offset: Optional[int] = Field(None)
     total: Optional[int] = Field(None)
+    
 
 
 class SearchResult(Entity):
-
-    highlight: Optional[str] = Field(
-        None, description="""matching text snippet containing html tags"""
-    )
+    
+    highlight: Optional[str] = Field(None, description="""matching text snippet containing html tags""")
     score: Optional[float] = Field(None)
     id: Optional[str] = Field(None)
     category: Optional[List[str]] = Field(default_factory=list)
     name: Optional[str] = Field(None)
     description: Optional[str] = Field(None)
     xref: Optional[List[str]] = Field(default_factory=list)
     provided_by: Optional[str] = Field(None)
     in_taxon: Optional[str] = Field(None)
     source: Optional[str] = Field(None)
     symbol: Optional[str] = Field(None)
     type: Optional[str] = Field(None)
     synonym: Optional[List[str]] = Field(default_factory=list)
+    
 
 
 class SearchResults(Results):
-
-    items: Optional[List[SearchResult]] = Field(
-        default_factory=list,
-        description="""A collection of items, with the type to be overriden by slot_usage""",
-    )
+    
+    items: Optional[List[SearchResult]] = Field(default_factory=list, description="""A collection of items, with the type to be overriden by slot_usage""")
     facet_fields: Optional[Dict[str, FacetField]] = Field(default_factory=dict)
     facet_queries: Optional[Dict[str, FacetValue]] = Field(default_factory=dict)
     limit: Optional[int] = Field(None)
     offset: Optional[int] = Field(None)
     total: Optional[int] = Field(None)
+    
 
 
 class FacetValue(ConfiguredBaseModel):
+    
+    label: Optional[str] = Field(None)
+    count: Optional[int] = Field(None, description="""number of items a this facet value""")
+    
+
 
+class HistoBin(FacetValue):
+    
+    id: Optional[str] = Field(None)
     label: Optional[str] = Field(None)
-    count: Optional[int] = Field(
-        None, description="""number of items a this facet value"""
-    )
+    count: Optional[int] = Field(None, description="""number of items a this facet value""")
+    
 
 
 class FacetField(ConfiguredBaseModel):
-
+    
     label: Optional[str] = Field(None)
     facet_values: Optional[Dict[str, FacetValue]] = Field(default_factory=dict)
+    
 
 
 class AssociationTypeMapping(ConfiguredBaseModel):
     """
     A data class to hold the necessary information to produce association type counts for given  entities with appropriate directional labels
     """
-
     association_type: Optional[AssociationTypeEnum] = Field(None)
-    subject_label: Optional[str] = Field(
-        None,
-        description="""A label to describe the subjects of the association type as a whole for use in the UI""",
-    )
-    object_label: Optional[str] = Field(
-        None,
-        description="""A label to describe the objects of the association type as a whole for use in the UI""",
-    )
-    category: Optional[List[str]] = Field(
-        default_factory=list,
-        description="""The biolink categories to use in queries for this association type, assuming OR semantics""",
-    )
-    predicate: Optional[List[str]] = Field(
-        default_factory=list,
-        description="""The biolink predicate to use in queries for this association type, assuming OR semantics""",
-    )
+    subject_label: Optional[str] = Field(None, description="""A label to describe the subjects of the association type as a whole for use in the UI""")
+    object_label: Optional[str] = Field(None, description="""A label to describe the objects of the association type as a whole for use in the UI""")
+    category: Optional[List[str]] = Field(default_factory=list, description="""The biolink categories to use in queries for this association type, assuming OR semantics""")
+    predicate: Optional[List[str]] = Field(default_factory=list, description="""The biolink predicate to use in queries for this association type, assuming OR semantics""")
+    
 
 
 class AssociationCount(FacetValue):
-
+    
     association_type: Optional[AssociationTypeEnum] = Field(None)
     label: Optional[str] = Field(None)
-    count: Optional[int] = Field(
-        None, description="""number of items a this facet value"""
-    )
+    count: Optional[int] = Field(None, description="""number of items a this facet value""")
+    
 
 
 class AssociationCountList(ConfiguredBaseModel):
     """
     Container class for a list of association counts
     """
+    items: Optional[List[AssociationCount]] = Field(default_factory=list, description="""A collection of items, with the type to be overriden by slot_usage""")
+    
 
-    items: Optional[List[AssociationCount]] = Field(
-        default_factory=list,
-        description="""A collection of items, with the type to be overriden by slot_usage""",
-    )
 
 
 # Update forward refs
 # see https://pydantic-docs.helpmanual.io/usage/postponed_annotations/
 Association.update_forward_refs()
 Entity.update_forward_refs()
 HistoPheno.update_forward_refs()
 Results.update_forward_refs()
 AssociationResults.update_forward_refs()
 EntityResults.update_forward_refs()
 SearchResult.update_forward_refs()
 SearchResults.update_forward_refs()
 FacetValue.update_forward_refs()
+HistoBin.update_forward_refs()
 FacetField.update_forward_refs()
 AssociationTypeMapping.update_forward_refs()
 AssociationCount.update_forward_refs()
 AssociationCountList.update_forward_refs()
+
```

### Comparing `monarch_py-0.7.0/src/monarch_py/datamodels/model.yaml` & `monarch_py-0.7.1/src/monarch_py/datamodels/model.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 prefixes:
   linkml: https://w3id.org/linkml/
   biolink: https://w3id.org/biolink/
 description: Data datamodels for the Monarch Initiative data access library
 imports:
 - linkml:types
 default_range: string
+
 enums:
   AssociationTypeEnum:
     description: >-
       A grouping label for association types, which are not necessarily 1:1 with
       biolink categories or predicates
     permissible_values:
       disease_phenotype:
@@ -116,15 +117,22 @@
         range: Entity
   HistoPheno:
     slots:
       - id
       - items
     slot_usage:
       items:
-        range: AssociationCount
+        range: HistoBin
+  HistoBin:
+    is_a: FacetValue
+    slots:
+      - id
+    slot_usage:
+      label:
+        identifier: false
   Results:
     abstract: true
     slots:
       - limit
       - offset
       - total
   SearchResult:
@@ -183,14 +191,15 @@
   AssociationCountList:
     description: Container class for a list of association counts
     slots:
       - items
     slot_usage:
       items:
         range: AssociationCount
+
 slots:
   aggregator_knowledge_source:
     multivalued: true
   association_type:
     range: AssociationTypeEnum
   category:
     multivalued: true
```

### Comparing `monarch_py-0.7.0/src/monarch_py/datamodels/solr.py` & `monarch_py-0.7.1/src/monarch_py/datamodels/solr.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.7.0/src/monarch_py/implementations/solr/solr_implementation.py` & `monarch_py-0.7.1/src/monarch_py/implementations/solr/solr_implementation.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     Association,
     AssociationCount,
     AssociationResults,
     AssociationTypeEnum,
     Entity,
     FacetField,
     FacetValue,
+    HistoBin,
     HistoPheno,
     SearchResult,
     SearchResults,
 )
 from monarch_py.datamodels.solr import HistoPhenoKeys, SolrQuery, core
 from monarch_py.interfaces.association_interface import AssociationInterface
 from monarch_py.interfaces.entity_interface import EntityInterface
@@ -145,41 +146,58 @@
         offset: int = 0,
         limit: int = 20,
     ) -> SolrQuery:
         """Populate a SolrQuery object with association filters"""
 
         query = SolrQuery(start=offset, rows=limit)
 
-        subject_field = "subject" if direct else "subject_closure"
-        object_field = "object" if direct else "object_closure"
-
         if category:
             query.add_field_filter_query("category", category)
         if predicate:
             query.add_field_filter_query("predicate", predicate)
         if subject:
-            query.add_field_filter_query(subject_field, subject)
+            if direct:
+                query.add_field_filter_query("subject", subject)
+            else:
+                query.add_filter_query(
+                    f'subject:"{subject}" OR subject_closure:"{subject}"'
+                )
         if subject_closure:
             query.add_field_filter_query("subject_closure", subject_closure)
         if object:
-            query.add_field_filter_query(object_field, object)
+            if direct:
+                query.add_field_filter_query("object", object)
+            else:
+                query.add_filter_query(
+                    f'object:"{object}" OR object_closure:"{object}"'
+                )
         if object_closure:
             query.add_field_filter_query("object_closure", object_closure)
         if between:
             # todo: handle error reporting / parsing, think about another way to pass this?
             b = between.split(",")
             e1 = escape(b[0])
             e2 = escape(b[1])
-            query.add_filter_query(
-                f'({subject_field}:"{e1}" AND {object_field}:"{e2}") OR ({subject_field}:"{e2}" AND {object_field}:"{e1}")'
-            )
+            if direct:
+                query.add_filter_query(
+                    f'(subject:"{e1}" AND object:"{e2}") OR (subject:"{e2}" AND object:"{e1}")'
+                )
+            else:
+                query.add_filter_query(
+                    f'((subject:"{e1}" OR subject_closure:"{e1}") AND (object:"{e2}" OR object_closure:"{e2}")) OR ((subject:"{e2}" OR subject_closure:"{e2}") AND (object:"{e1}" OR object_closure:"{e1}"))'
+                )
         if entity:
-            query.add_filter_query(
-                f'{subject_field}:"{escape(entity)}" OR {object_field}:"{escape(entity)}"'
-            )
+            if direct:
+                query.add_filter_query(
+                    f'subject:"{escape(entity)}" OR subject_closure:"{escape(entity)}" OR object:"{escape(entity)}" OR object_closure:"{escape(entity)}"'
+                )
+            else:
+                query.add_filter_query(
+                    f'subject:"{escape(entity)}" OR object:"{escape(entity)}"'
+                )
         if association_type:
             query.add_filter_query(
                 get_solr_query_fragment(
                     AssociationTypeMappings().get_mapping(association_type)
                 )
             )
 
@@ -360,46 +378,38 @@
         )
 
         hpkeys = [i.value for i in HistoPhenoKeys]
 
         query.facet_queries = [f'object_closure:"{i}"' for i in hpkeys]
         query_result = solr.query(query)
 
-        association_counts = []
+        bins = []
         for k, v in query_result.facet_counts.facet_queries.items():
             id = f"{k.split(':')[1]}:{k.split(':')[2]}".replace('"', "")
             label = HistoPhenoKeys(id).name
-            association_counts.append(AssociationCount(id=id, label=label, count=v))
-
-        association_counts = sorted(
-            association_counts, key=lambda x: x.count, reverse=True
-        )
-
-        hp = HistoPheno(
-            id=subject_closure,
-            items=association_counts,
-        )
+            bins.append(HistoBin(id=id, label=label, count=v))
+        bins = sorted(bins, key=lambda x: x.count, reverse=True)
 
-        return hp
+        return HistoPheno(id=subject_closure, items=bins)
 
     def get_association_counts(self, entity: str) -> List[AssociationCount]:
         """
         Get association counts for a given entity
 
         This method uses chunks of solr query syntax mapped to the association type
         Args:
             entity:
 
         Returns:
 
         """
         query = self._populate_association_query(entity=entity)
         facet_queries = []
-        subject_query = f'AND subject_closure:"{entity}"'
-        object_query = f'AND object_closure:"{entity}"'
+        subject_query = f'AND (subject:"{entity}" OR subject_closure:"{entity}")'
+        object_query = f'AND (object:"{entity}" OR object_closure:"{entity}")'
         # Run the same facet_queries constrained to matches against either the subject or object
         # to know which kind of label will be needed in the UI to refer to the opposite side of the association
         for field_query in [subject_query, object_query]:
             for agm in AssociationTypeMappings.get_mappings():
                 association_type_query = get_solr_query_fragment(agm)
                 facet_queries.append(f"({association_type_query}) {field_query}")
         query.facet_queries = facet_queries
```

### Comparing `monarch_py-0.7.0/src/monarch_py/implementations/sql/sql_implementation.py` & `monarch_py-0.7.1/src/monarch_py/implementations/sql/sql_implementation.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.7.0/src/monarch_py/interfaces/association_interface.py` & `monarch_py-0.7.1/src/monarch_py/interfaces/association_interface.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.7.0/src/monarch_py/interfaces/entity_interface.py` & `monarch_py-0.7.1/src/monarch_py/interfaces/entity_interface.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.7.0/src/monarch_py/interfaces/query_interface.py` & `monarch_py-0.7.1/src/monarch_py/interfaces/query_interface.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.7.0/src/monarch_py/interfaces/search_interface.py` & `monarch_py-0.7.1/src/monarch_py/interfaces/search_interface.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.7.0/src/monarch_py/service/solr_service.py` & `monarch_py-0.7.1/src/monarch_py/service/solr_service.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.7.0/src/monarch_py/solr_cli.py` & `monarch_py-0.7.1/src/monarch_py/solr_cli.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,20 +5,22 @@
 from monarch_py.utils.solr_cli_utils import (
     check_solr_permissions,
     get_solr,
     solr_status,
     start_solr,
     stop_solr,
 )
-from monarch_py.utils.utils import console, to_json, to_tsv, to_yaml
+from monarch_py.utils.utils import console, format_output
 
 solr_app = typer.Typer()
 monarchstow = pystow.module("monarch")
 
+############################
 ### SOLR DOCKER COMMANDS ###
+############################
 
 
 @solr_app.command("start")
 def start(update: bool = False):
     """Starts a local Solr container."""
     check_solr_permissions(update=False)
     start_solr()
@@ -29,64 +31,62 @@
     """Stops the local Solr container."""
     stop_solr()
     raise typer.Exit()
 
 
 @solr_app.command("status")
 def status():
+    """Checks the status of the local Solr container."""
     solr_status()
     raise typer.Exit()
 
 
 @solr_app.command("download")
 def download():
+    """Download the Monarch Solr KG."""
     get_solr(update=True)
     raise typer.Exit()
 
 
+###########################
 ### SOLR QUERY COMMANDS ###
+###########################
 
 
 @solr_app.command("entity")
 def entity(
     id: str = typer.Argument(None, help="The identifier of the entity to be retrieved"),
     fmt: str = typer.Option(
-        "json", "--format", "-f", help="The format of the output (TSV, YAML, JSON)"
+        "json",
+        "--format",
+        "-f",
+        help="The format of the output (json, yaml, tsv, table)",
     ),
     output: str = typer.Option(
         None, "--output", "-o", help="The path to the output file"
     ),
 ):
     """
     Retrieve an entity by ID
 
     Args:
         id (str): The identifier of the entity to be retrieved
 
     Optional Args:
-        fmt (str): The format of the output (TSV, YAML, JSON). Default JSON
+        fmt (str): The format of the output (json, yaml, tsv, table). Default JSON
         output (str): The path to the output file. Default stdout
     """
 
     if not id:
         console.print("\n[bold red]Entity ID required.[/]\n")
         raise typer.Exit(1)
 
     data = get_solr(update=False)
     response = data.get_entity(id)
-
-    if fmt == "json":
-        to_json(response, output)
-    elif fmt == "tsv":
-        to_tsv(response, output)
-    elif fmt == "yaml":
-        to_yaml(response, output)
-    else:
-        console.print(f"\n[bold red]Format '{fmt}' not supported.[/]\n")
-    raise typer.Exit()
+    format_output(fmt, response, output)
 
 
 @solr_app.command("associations")
 def associations(
     category: str = typer.Option(None, "--category"),
     subject: str = typer.Option(None, "--subject"),
     predicate: str = typer.Option(None, "--predicate"),
@@ -94,15 +94,18 @@
     entity: str = typer.Option(None, "--entity"),
     between: str = typer.Option(None, "--between"),
     direct: bool = typer.Option(False, "--direct"),
     association_type: str = typer.Option(None, "--label"),
     limit: int = typer.Option(20, "--limit"),
     offset: int = typer.Option(0, "--offset"),
     fmt: str = typer.Option(
-        "json", "--format", "-f", help="The format of the output (TSV, YAML, JSON)"
+        "json",
+        "--format",
+        "-f",
+        help="The format of the output (json, yaml, tsv, table)",
     ),
     output: str = typer.Option(
         None, "--output", "-o", help="The path to the output file"
     ),
 ):
     """
     Paginate through associations
@@ -114,184 +117,148 @@
         object (str, optional): The object of the association.
         entity (str, optional): The subject or object of the association.
         between (str, optional): Two comma-separated entities to get bi-directional associations.
         direct (bool, optional): Exclude associations with the specified subject and objects as ancestors. Default False
         association_type (str, optional): The association label of the association
         limit (int, optional): The number of associations to return. Default 20
         offset (int, optional): The offset of the first association to be retrieved. Default 0
-        fmt (str): The format of the output (TSV, YAML, JSON). Default JSON
+        fmt (str): The format of the output (json, yaml, tsv, table). Default JSON
         output (str): The path to the output file. Default stdout
     """
     args = locals()
     args.pop("update", None)
     args.pop("fmt", None)
     args.pop("output", None)
 
     data = get_solr(update=False)
     response = data.get_associations(**args)
-
-    if fmt == "json":
-        to_json(response, output)
-    elif fmt == "tsv":
-        to_tsv(response, output)
-    elif fmt == "yaml":
-        to_yaml(response, output)
-    else:
-        console.print(f"\n[bold red]Format '{fmt}' not supported.[/]\n")
-    raise typer.Exit()
+    format_output(fmt, response, output)
 
 
 @solr_app.command("search")
 def search(
     q: str = typer.Option(None, "--query", "-q"),
     category: str = typer.Option(None, "--category", "-c"),
     taxon: str = typer.Option(None, "--taxon", "-t"),
     limit: int = typer.Option(20, "--limit", "-l"),
     offset: int = typer.Option(0, "--offset"),
     fmt: str = typer.Option(
-        "json", "--format", "-f", help="The format of the output (TSV, YAML, JSON)"
+        "json",
+        "--format",
+        "-f",
+        help="The format of the output (json, yaml, tsv, table)",
     ),
     output: str = typer.Option(
         None, "--output", "-o", help="The path to the output file"
     ),
 ):
     """
     Search for entities
 
     Optional Args:
         q: The query string to search for
         category: The category of the entity
         taxon: The taxon of the entity
         limit: The number of entities to return
         offset: The offset of the first entity to be retrieved
-        fmt (str): The format of the output (TSV, YAML, JSON). Default JSON
+        fmt (str): The format of the output (json, yaml, tsv, table). Default JSON
         output (str): The path to the output file. Default stdout
     """
     data = get_solr(update=False)
-
     response = data.search(
         q=q, category=category, taxon=taxon, limit=limit, offset=offset
     )
-
-    if fmt == "json":
-        to_json(response, output)
-    elif fmt == "tsv":
-        to_tsv(response, output)
-    elif fmt == "yaml":
-        to_yaml(response, output)
-    else:
-        console.print(f"\n[bold red]Format '{fmt}' not supported.[/]\n")
-    raise typer.Exit()
+    format_output(fmt, response, output)
 
 
 @solr_app.command("autocomplete")
 def autocomplete(
     q: str = typer.Argument(None, help="Query string to autocomplete against"),
     fmt: str = typer.Option(
-        "json", "--format", "-f", help="The format of the output (TSV, YAML, JSON)"
+        "json",
+        "--format",
+        "-f",
+        help="The format of the output (json, yaml, tsv, table)",
     ),
     output: str = typer.Option(
         None, "--output", "-o", help="The path to the output file"
     ),
 ):
     """
     Return entity autcomplete matches for a query string
 
     Args:
         q: The query string to autocomplete against
-        fmt: The format of the output (TSV, YAML, JSON)
+        fmt: The format of the output (json, yaml, tsv, table)
         output: The path to the output file (stdout if not specified)
 
     """
-
     data = get_solr(update=False)
     response = data.autocomplete(q)
-
-    if fmt == "json":
-        to_json(response, output)
-    elif fmt == "tsv":
-        to_tsv(response, output)
-    elif fmt == "yaml":
-        to_yaml(response, output)
-    else:
-        console.print(f"\n[bold red]Format '{fmt}' not supported.[/]\n")
-    raise typer.Exit()
+    format_output(fmt, response, output)
 
 
 @solr_app.command("histopheno")
 def histopheno(
     subject: str = typer.Argument(None, help="The subject of the association"),
     fmt: str = typer.Option(
-        "json", "--format", "-f", help="The format of the output (TSV, YAML, JSON)"
+        "json",
+        "--format",
+        "-f",
+        help="The format of the output (json, yaml, tsv, table)",
     ),
     output: str = typer.Option(
         None, "--output", "-o", help="The path to the output file"
     ),
 ):
     """
     Retrieve the histopheno associations for a given subject
 
     Args:
         subject (str): The subject of the association
 
     Optional Args:
         update (bool): Whether to re-download the Monarch KG. Default False
-        fmt (str): The format of the output (TSV, YAML, JSON). Default JSON
+        fmt (str): The format of the output (json, yaml, tsv, table). Default JSON
         output (str): The path to the output file. Default stdout
     """
 
     if not subject:
         console.print("\n[bold red]Subject ID required.[/]\n")
         raise typer.Exit(1)
 
     data = get_solr(update=False)
     response = data.get_histopheno(subject)
-
-    if fmt == "json":
-        to_json(response, output)
-    elif fmt == "tsv":
-        to_tsv(response, output)
-    elif fmt == "yaml":
-        to_yaml(response, output)
-    else:
-        console.print(f"\n[bold red[Format '{fmt}' not supported.[/]\n")
-    raise typer.Exit()
+    format_output(fmt, response, output)
 
 
 @solr_app.command("association-counts")
 def association_counts(
     entity: str = typer.Argument(None, help="The entity to get association counts for"),
     fmt: str = typer.Option(
-        "json", "--format", "-f", help="The format of the output (TSV, YAML, JSON)"
+        "json",
+        "--format",
+        "-f",
+        help="The format of the output (json, yaml, tsv, table)",
     ),
     output: str = typer.Option(
         None, "--output", "-o", help="The path to the output file"
     ),
 ):
     """
     Retrieve the association counts for a given entity
 
     Args:
         entity (str): The entity to get association counts for
 
     Optional Args:
         update (bool): Whether to re-download the Monarch KG. Default False
-        fmt (str): The format of the output (TSV, YAML, JSON). Default JSON
+        fmt (str): The format of the output (json, yaml, tsv, table). Default JSON
         output (str): The path to the output file. Default stdout
     """
-
     if not entity:
         console.print("\n[bold red]Entity ID required.[/]\n")
         raise typer.Exit(1)
-
     data = get_solr(update=False)
     response = data.get_association_counts(entity)
     counts = AssociationCountList(items=response)
-    if fmt == "json":
-        to_json(counts, output)
-    elif fmt == "tsv":
-        to_tsv(counts, output)
-    elif fmt == "yaml":
-        to_yaml(counts, output)
-    else:
-        console.print(f"\n[bold red[Format '{fmt}' not supported.[/]\n")
-    raise typer.Exit()
+    format_output(fmt, counts, output)
```

### Comparing `monarch_py-0.7.0/src/monarch_py/sql_cli.py` & `monarch_py-0.7.1/src/monarch_py/sql_cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,58 +1,50 @@
 import typer
 
 from monarch_py.implementations.sql.sql_implementation import SQLImplementation
-from monarch_py.utils.utils import console, to_json, to_tsv, to_yaml
+from monarch_py.utils.utils import console, format_output
 
 sql_app = typer.Typer()
 
 
 @sql_app.command()
 def entity(
     id: str = typer.Argument(None, help="The identifier of the entity to be retrieved"),
     update: bool = typer.Option(
         False, "--update", "-u", help="Whether to re-download the Monarch KG"
     ),
     fmt: str = typer.Option(
-        "json", "--format", "-f", help="The format of the output (TSV, YAML, JSON)"
+        "json",
+        "--format",
+        "-f",
+        help="The format of the output (json, yaml, tsv, table)",
     ),
     output: str = typer.Option(
         None, "--output", "-o", help="The path to the output file"
     ),
 ):
     """Retrieve an entity by ID
 
     Args:
         id (str): The identifier of the entity to be retrieved
         update (bool): = Whether to re-download the Monarch KG. Default False
-        fmt (str): The format of the output (TSV, YAML, JSON). Default JSON
+        fmt (str): The format of the output (json, yaml, tsv, table). Default JSON
         output (str): The path to the output file. Default stdout
     """
-
     if not id:
         console.print("\n[bold red]Entity ID required.[/]\n")
         raise typer.Exit(1)
 
     data = SQLImplementation()
     response = data.get_entity(id, update)
 
     if not response:
         console.print(f"\nEntity '{id}' not found.\n")
         raise typer.Exit(1)
-
-    if fmt == "json":
-        to_json(response, output)
-    elif fmt == "tsv":
-        to_tsv(response, output)
-    elif fmt == "yaml":
-        to_yaml(response, output)
-    else:
-        console.print(f"\n[bold red]Format '{fmt}' not supported.[/]\n")
-        raise typer.Exit(1)
-    raise typer.Exit()
+    format_output(fmt, response, output)
 
 
 @sql_app.command()
 def associations(
     category: str = typer.Option(None, "--category"),
     subject: str = typer.Option(None, "--subject"),
     predicate: str = typer.Option(None, "--predicate"),
@@ -60,15 +52,18 @@
     entity: str = typer.Option(None, "--entity"),
     between: str = typer.Option(None, "--between"),
     association_type: str = typer.Option(None, "--label"),
     limit: int = typer.Option(20, "--limit"),
     offset: int = typer.Option(0, "--offset"),
     update: bool = typer.Option(False, "--update"),
     fmt: str = typer.Option(
-        "json", "--format", "-f", help="The format of the output (TSV, YAML, JSON)"
+        "json",
+        "--format",
+        "-f",
+        help="The format of the output (json, yaml, tsv, table)",
     ),
     output: str = typer.Option(
         None, "--output", "-o", help="The path to the output file"
     ),
 ):
     """Paginate through associations
 
@@ -79,27 +74,17 @@
         object (str, optional): The object of the association.
         entity (str, optional): The subject or object of the association.
         between (str, optional): Two comma-separated entities to get bi-directional associations.
         association_type (str, optional): The label of the association.
         limit (int, optional): The number of associations to return. Default 20
         offset (int, optional): The offset of the first association to be retrieved. Default 0
         update (bool, optional): Whether to re-download the Monarch KG. Default False
-        fmt (str): The format of the output (TSV, YAML, JSON). Default JSON
+        fmt (str): The format of the output (json, yaml, tsv, table). Default JSON
         output (str): The path to the output file. Default stdout
     """
     args = locals()
     args.pop("fmt", None)
     args.pop("output", None)
 
     data = SQLImplementation()
     response = data.get_associations(**args)
-
-    if fmt == "json":
-        to_json(response, output)
-    elif fmt == "tsv":
-        to_tsv(response, output)
-    elif fmt == "yaml":
-        to_yaml(response, output)
-    else:
-        console.print(f"\n[bold red]Format '{fmt}' not supported.[/]\n")
-        raise typer.Exit(1)
-    raise typer.Exit()
+    format_output(fmt, response, output)
```

### Comparing `monarch_py-0.7.0/src/monarch_py/utils/association_type_utils.py` & `monarch_py-0.7.1/src/monarch_py/utils/association_type_utils.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.7.0/src/monarch_py/utils/solr_cli_utils.py` & `monarch_py-0.7.1/src/monarch_py/utils/solr_cli_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     if sys.platform in ["linux", "linux2", "darwin"]:
         stat_info = os.stat(data_path)
         if stat_info.st_gid != 8983:
             console.print(
                 f"""
 Solr container requires write access to {monarchstow.base}.
 Please run the following command to set permissions:
-    [grey84 on black]sudo chgrp -R 8983 {monarchstow.base}[/]
+    [grey84 on black]sudo chgrp -R 8983 {monarchstow.base} && \[/]
     [grey84 on black]sudo chmod -R g+w {monarchstow.base}[/]
             """
             )
             sys.exit(1)
 
 
 def check_for_solr(dc: docker.DockerClient, quiet: bool = False):
```

### Comparing `monarch_py-0.7.0/src/monarch_py/utils/utils.py` & `monarch_py-0.7.1/src/monarch_py/utils/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import csv
 import sys
 
+import typer
 import yaml
 from rich import print_json
 from rich.console import Console
 from rich.table import Table
 
 from monarch_py.datamodels.model import (
     AssociationCountList,
@@ -19,15 +20,15 @@
     "https://data.monarchinitiative.org/monarch-kg-dev/latest/monarch-kg.db.gz"
 )
 
 
 console = Console(
     color_system="truecolor",
     stderr=True,
-    style="blue1",
+    style="pink1",
 )
 
 
 def strip_json(doc: dict, *fields_to_remove: str):
     for field in fields_to_remove:
         try:
             del doc[field]
@@ -47,14 +48,23 @@
 
 
 ### Output conversion methods ###
 
 FMT_INPUT_ERROR_MSG = "Text conversion method only accepts Entity, HistoPheno, AssociationCountList, or Results objects."
 
 
+def get_headers_from_obj(obj: ConfiguredBaseModel) -> list:
+    """Return a list of headers from a pydantic model."""
+    schema = type(obj).schema()
+    definitions = schema["definitions"]
+    this_ref = schema["properties"]["items"]["items"]["$ref"].split("/")[-1]
+    headers = definitions[this_ref]["properties"].keys()
+    return list(headers)
+
+
 def to_json(obj: ConfiguredBaseModel, file: str):
     """Converts a pydantic model to a JSON string."""
     if file:
         with open(file, "w") as f:
             f.write(obj.json(indent=4))
         console.print(f"\nOutput written to {file}\n")
     else:
@@ -64,82 +74,74 @@
 def to_tsv(obj: ConfiguredBaseModel, file: str) -> str:
     """Converts a pydantic model to a TSV string."""
 
     # Extract headers and rows from object
     if isinstance(obj, Entity):
         headers = obj.dict().keys()
         rows = [list(obj.dict().values())]
-    elif (
-        isinstance(obj, Results)
-        or isinstance(obj, HistoPheno)
-        or isinstance(obj, AssociationCountList)
-    ):
-        headers = obj.items[0].dict().keys()
-        rows = [list(item.dict().values()) for item in obj.items]
+    elif isinstance(obj, (AssociationCountList, HistoPheno, Results)):
+        if not obj.items:
+            headers = get_headers_from_obj(obj)
+            rows = []
+        else:
+            headers = obj.items[0].dict().keys()
+            rows = [list(item.dict().values()) for item in obj.items]
     else:
         raise TypeError(FMT_INPUT_ERROR_MSG)
 
-    # console.print(f"\n{obj.__class__.__name__}\n")
-    # console.print(f"Headers ({type(headers)}): {headers}\n")
-    # console.print(f"Rows ({type(rows)}):")
-    # for row in rows: console.print(row)
-
+    fh = open(file, "w") if file else sys.stdout
+    writer = csv.writer(fh, delimiter="\t")
+    writer.writerow(headers)
+    for row in rows:
+        writer.writerow(list(row))
     if file:
-        fh = open(file, "w")
-        writer = csv.writer(fh, delimiter="\t")
-        writer.writerow(headers)
-        for row in rows:
-            writer.writerow(list(row))
         fh.close()
         console.print(f"\nOutput written to {file}\n")
 
+    return
+
+
+def to_table(obj: ConfiguredBaseModel):
+
+    # Extract headers and rows from object
+    if isinstance(obj, Entity):
+        headers = obj.dict().keys()
+        rows = [list(obj.dict().values())]
+    elif isinstance(obj, (AssociationCountList, HistoPheno, Results)):
+        if not obj.items:
+            headers = get_headers_from_obj(obj)
+            rows = []
+        else:
+            headers = obj.items[0].dict().keys()
+            rows = [list(item.dict().values()) for item in obj.items]
     else:
-        # Convert all to strings
-        for row in rows:
-            for i, value in enumerate(row):
-                if isinstance(value, list):
-                    row[i] = ", ".join(value)
-                elif not isinstance(value, str):
-                    row[i] = str(value)
-        title = (
-            f"{obj.__class__.__name__}: {obj.id}"
-            if hasattr(obj, "id")
-            else obj.__class__.__name__
-        )
-        table = Table(
-            title=console.rule(title),
-            show_header=True,
-            header_style="bold cyan",
-        )
-        for header in headers:
-            table.add_column(header)
-        for row in rows:
-            table.add_row(*row)
-        console.print(table)
-
-    # fh = open(file, "w") if file else sys.stdout
-    # writer = csv.writer(fh, delimiter="\t")
-
-    # if isinstance(obj, Entity):
-    #     headers = obj.dict().keys()
-    #     writer.writerow(headers)
-    #     writer.writerow(obj.dict().values())
-    # elif (isinstance(obj, Results) or isinstance(obj, HistoPheno)):
-    #     headers = obj.items[0].dict().keys()
-    #     writer.writerow(headers)
-    #     for item in obj.items:
-    #         writer.writerow(item.dict().values())
-    # else:
-    #     raise TypeError(FMT_INPUR_ERROR_MSG)
-
-    # if file:
-    #     fh.close()
-    #     console.print(f"\nOutput written to {file}\n")
+        raise TypeError(FMT_INPUT_ERROR_MSG)
 
-    # return
+    for row in rows:
+        for i, value in enumerate(row):
+            if isinstance(value, list):
+                row[i] = ", ".join(value)
+            elif not isinstance(value, str):
+                row[i] = str(value)
+    title = (
+        f"{obj.__class__.__name__}: {obj.id}"
+        if hasattr(obj, "id")
+        else obj.__class__.__name__
+    )
+    table = Table(
+        title=console.rule(title),
+        show_header=True,
+        header_style="bold cyan",
+    )
+    for header in headers:
+        table.add_column(header)
+    for row in rows:
+        table.add_row(*row)
+    console.print(table)
+    return
 
 
 def to_yaml(obj: ConfiguredBaseModel, file: str):
     """Converts a pydantic model to a YAML string."""
 
     fh = open(file, "w") if file else sys.stdout
 
@@ -155,7 +157,22 @@
         raise TypeError(FMT_INPUT_ERROR_MSG)
 
     if file:
         console.print(f"\nOutput written to {file}\n")
         fh.close()
 
     return
+
+
+def format_output(fmt: str, response: ConfiguredBaseModel, output: str):
+    if fmt.lower() == "json":
+        to_json(response, output)
+    elif fmt.lower() == "tsv":
+        to_tsv(response, output)
+    elif fmt.lower() == "yaml":
+        to_yaml(response, output)
+    elif fmt.lower() == "table":
+        to_table(response)
+    else:
+        console.print(f"\n[bold red]Format '{fmt}' not supported.[/]\n")
+        raise typer.Exit(1)
+    raise typer.Exit()
```

### Comparing `monarch_py-0.7.0/PKG-INFO` & `monarch_py-0.7.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monarch-py
-Version: 0.7.0
+Version: 0.7.1
 Summary: Monarch Initiative data access library
 Author: Kevin Schaper
 Author-email: kevin@tislab.org
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

