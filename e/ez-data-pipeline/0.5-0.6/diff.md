# Comparing `tmp/ez_data_pipeline-0.5-py3-none-any.whl.zip` & `tmp/ez_data_pipeline-0.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 6973 bytes, number of entries: 15
+Zip file size: 6959 bytes, number of entries: 15
 -rw-rw-rw-  2.0 fat       36 b- defN 23-Apr-30 22:16 ez_data_pipeline/__init__.py
 -rw-rw-rw-  2.0 fat       39 b- defN 23-Apr-30 22:16 ez_data_pipeline/Foundation/__init__.py
 -rw-rw-rw-  2.0 fat      517 b- defN 23-Apr-29 21:09 ez_data_pipeline/Foundation/utils.py
--rw-rw-rw-  2.0 fat      525 b- defN 23-May-04 04:16 ez_data_pipeline/Foundation/default_pipeline/Iimporter.py
+-rw-rw-rw-  2.0 fat      521 b- defN 23-May-04 04:32 ez_data_pipeline/Foundation/default_pipeline/Iimporter.py
 -rw-rw-rw-  2.0 fat      412 b- defN 23-Apr-29 21:09 ez_data_pipeline/Foundation/default_pipeline/Imodel.py
--rw-rw-rw-  2.0 fat     1044 b- defN 23-May-04 04:16 ez_data_pipeline/Foundation/default_pipeline/Ipipeline.py
--rw-rw-rw-  2.0 fat     1149 b- defN 23-May-04 04:16 ez_data_pipeline/Foundation/default_pipeline/Iproccess.py
--rw-rw-rw-  2.0 fat     1291 b- defN 23-May-04 04:16 ez_data_pipeline/Foundation/default_pipeline/IproccessMethod.py
+-rw-rw-rw-  2.0 fat     1036 b- defN 23-May-04 04:32 ez_data_pipeline/Foundation/default_pipeline/Ipipeline.py
+-rw-rw-rw-  2.0 fat     1145 b- defN 23-May-04 04:32 ez_data_pipeline/Foundation/default_pipeline/Iproccess.py
+-rw-rw-rw-  2.0 fat     1279 b- defN 23-May-04 04:32 ez_data_pipeline/Foundation/default_pipeline/IproccessMethod.py
 -rw-rw-rw-  2.0 fat      346 b- defN 23-Apr-30 21:53 ez_data_pipeline/Foundation/default_pipeline/Isave.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Apr-27 02:12 ez_data_pipeline/Foundation/default_pipeline/__init__.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Apr-27 02:12 ez_data_pipeline/Pipeline/__init__.py
--rw-rw-rw-  2.0 fat     6613 b- defN 23-May-04 04:21 ez_data_pipeline-0.5.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-04 04:21 ez_data_pipeline-0.5.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       17 b- defN 23-May-04 04:21 ez_data_pipeline-0.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1476 b- defN 23-May-04 04:21 ez_data_pipeline-0.5.dist-info/RECORD
-15 files, 13557 bytes uncompressed, 4425 bytes compressed:  67.4%
+-rw-rw-rw-  2.0 fat     6613 b- defN 23-May-04 04:32 ez_data_pipeline-0.6.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-04 04:32 ez_data_pipeline-0.6.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       17 b- defN 23-May-04 04:32 ez_data_pipeline-0.6.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     1476 b- defN 23-May-04 04:32 ez_data_pipeline-0.6.dist-info/RECORD
+15 files, 13529 bytes uncompressed, 4411 bytes compressed:  67.4%
```

## zipnote {}

```diff
@@ -27,20 +27,20 @@
 
 Filename: ez_data_pipeline/Foundation/default_pipeline/__init__.py
 Comment: 
 
 Filename: ez_data_pipeline/Pipeline/__init__.py
 Comment: 
 
-Filename: ez_data_pipeline-0.5.dist-info/METADATA
+Filename: ez_data_pipeline-0.6.dist-info/METADATA
 Comment: 
 
-Filename: ez_data_pipeline-0.5.dist-info/WHEEL
+Filename: ez_data_pipeline-0.6.dist-info/WHEEL
 Comment: 
 
-Filename: ez_data_pipeline-0.5.dist-info/top_level.txt
+Filename: ez_data_pipeline-0.6.dist-info/top_level.txt
 Comment: 
 
-Filename: ez_data_pipeline-0.5.dist-info/RECORD
+Filename: ez_data_pipeline-0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ez_data_pipeline/Foundation/default_pipeline/Iimporter.py

```diff
@@ -1,9 +1,9 @@
 from abc import ABC, abstractmethod
-from src.ez_data_pipeline.Foundation import utils
+from ez_data_pipeline.Foundation import utils
 
 
 class IImporter(ABC):
     """
     Generalized Interface for changing the source and import to accommodate the return_data abstract method
     """
```

## ez_data_pipeline/Foundation/default_pipeline/Ipipeline.py

```diff
@@ -1,9 +1,9 @@
-from src.ez_data_pipeline.Foundation.default_pipeline.Imodel import Imodel
-from src.ez_data_pipeline.Foundation.default_pipeline.IproccessMethod import ProcessingMethod
+from ez_data_pipeline.Foundation.default_pipeline.Imodel import Imodel
+from ez_data_pipeline.Foundation.default_pipeline.IproccessMethod import ProcessingMethod
 
 
 class ModelPipeline:
     """
     This combines all previous classes Imodel, and ProcessingMethod
     to return dataframe for prediction
     """
```

## ez_data_pipeline/Foundation/default_pipeline/Iproccess.py

```diff
@@ -1,9 +1,9 @@
 from abc import ABC, abstractmethod, ABCMeta
-from src.ez_data_pipeline.Foundation.utils import ImportData
+from ez_data_pipeline.Foundation.utils import ImportData
 
 
 class Processor(ABC):
     @abstractmethod
     def process(self, import_data: ImportData) -> ImportData:
         pass
```

## ez_data_pipeline/Foundation/default_pipeline/IproccessMethod.py

```diff
@@ -1,10 +1,10 @@
-from src.ez_data_pipeline.Foundation.default_pipeline.Isave import Isave
-from src.ez_data_pipeline.Foundation.default_pipeline.Iproccess import ProcessPipeline
-from src.ez_data_pipeline.Foundation.default_pipeline.Iimporter import IImporter
+from ez_data_pipeline.Foundation.default_pipeline.Isave import Isave
+from ez_data_pipeline.Foundation.default_pipeline.Iproccess import ProcessPipeline
+from ez_data_pipeline.Foundation.default_pipeline.Iimporter import IImporter
 
 
 # Any way to type-hint
 # Fix later
 class ProcessingMethod:
 
     def __init__(self, data_importer: IImporter, process_pipeline: ProcessPipeline, saver: Isave, ticker: str):
```

## Comparing `ez_data_pipeline-0.5.dist-info/METADATA` & `ez_data_pipeline-0.6.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ez-data-pipeline
-Version: 0.5
+Version: 0.6
 Summary: Object Oriented Library to create data pipelines
 Home-page: https://github.com/VexedIOS/open_data_pipeline
 Author: Juan(VexedIOS)
 Author-email: juanteams@outlook.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
```

## Comparing `ez_data_pipeline-0.5.dist-info/RECORD` & `ez_data_pipeline-0.6.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ez_data_pipeline/__init__.py,sha256=32nMcMk-ElxjMSJLRqsBO9lt4q5So2SMLYrf7gu6QxE,36
 ez_data_pipeline/Foundation/__init__.py,sha256=cSn4BPRy1QyQ5SRqHk8ywREhcnLkj-WcwiRkgfTa-e8,39
 ez_data_pipeline/Foundation/utils.py,sha256=30S3dj4xpuEQiX2foZPiVSJwcehthWNa8JBB-C5S2vU,517
-ez_data_pipeline/Foundation/default_pipeline/Iimporter.py,sha256=MI-5S_JAjDRnQYnEAOZ6nnCWQdLfpV92_YF5HJor7xo,525
+ez_data_pipeline/Foundation/default_pipeline/Iimporter.py,sha256=NI_vFGLFO6VW4KCI_0HfxR1EoIuUXKaXdOoCmhCrQnE,521
 ez_data_pipeline/Foundation/default_pipeline/Imodel.py,sha256=8K1uhi2ScMcGkBbBug1HSr4mrCeq8pHDJCpjuERcLQA,412
-ez_data_pipeline/Foundation/default_pipeline/Ipipeline.py,sha256=92tQKSGLAiRiaIipjJQ8Y_vsXrfsVuKMht9xVzeJqhI,1044
-ez_data_pipeline/Foundation/default_pipeline/Iproccess.py,sha256=FRkH-QnRBS6UASEXS4aaqUwKQyCF7AEGA5H8giskmNA,1149
-ez_data_pipeline/Foundation/default_pipeline/IproccessMethod.py,sha256=-AKJdKiLlaJcQuokXSsaRSwOCSB2XuzuU1Zaaqj7pes,1291
+ez_data_pipeline/Foundation/default_pipeline/Ipipeline.py,sha256=jvSTIz0zSea6D8H590K7meiPawNIIXKTNpuxFhqdlMg,1036
+ez_data_pipeline/Foundation/default_pipeline/Iproccess.py,sha256=qgpE0tCqT9lA1UhGh5EAjAV-W89T3eYFlb9hL4yStBc,1145
+ez_data_pipeline/Foundation/default_pipeline/IproccessMethod.py,sha256=B-442UM5uYiPVF8u70iEhEuyBhAtHDuJApd3tgwCAZY,1279
 ez_data_pipeline/Foundation/default_pipeline/Isave.py,sha256=MhkBiWz9qoMdzeZGth-VfqfVac1ouZo8L4PPeETB9Zg,346
 ez_data_pipeline/Foundation/default_pipeline/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 ez_data_pipeline/Pipeline/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-ez_data_pipeline-0.5.dist-info/METADATA,sha256=DWNwOooRRv4iNBJ4fUlYxfTmKdoYhYp_7ZiEpMH1hE4,6613
-ez_data_pipeline-0.5.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-ez_data_pipeline-0.5.dist-info/top_level.txt,sha256=RqWalU1CYCMUT00p1mVmo21Ghy9KCAeCNDKcIfFmLNY,17
-ez_data_pipeline-0.5.dist-info/RECORD,,
+ez_data_pipeline-0.6.dist-info/METADATA,sha256=n022bDnE58HhrnOBIqkzudrxMv3kV8PXr6pteDBmXuM,6613
+ez_data_pipeline-0.6.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+ez_data_pipeline-0.6.dist-info/top_level.txt,sha256=RqWalU1CYCMUT00p1mVmo21Ghy9KCAeCNDKcIfFmLNY,17
+ez_data_pipeline-0.6.dist-info/RECORD,,
```

