# Comparing `tmp/srtk-0.0.1.tar.gz` & `tmp/srtk-0.0.2.tar.gz`

## Comparing `srtk-0.0.1.tar` & `srtk-0.0.2.tar`

### file list

```diff
@@ -1,44 +1,45 @@
--rw-r--r--   0        0        0     5656 2020-02-02 00:00:00.000000 srtk-0.0.1/graphs-for-paper.ipynb
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 srtk-0.0.1/requirements.txt
--rw-r--r--   0        0        0    10348 2020-02-02 00:00:00.000000 srtk-0.0.1/test.pdf
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 srtk-0.0.1/train_qald.ipynb
--rw-r--r--   0        0        0    22960 2020-02-02 00:00:00.000000 srtk-0.0.1/train_wd_simple.ipynb
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 srtk-0.0.1/.github/workflows/pytest.yml
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 srtk-0.0.1/resources/wikimapper/index_enwiki.db -> /home/wiss/liao/shen/flamingo-gnn/data/kilt/index_enwiki-latest-uncased.db
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 srtk-0.0.1/src/srtk/__init__.py
--rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 srtk-0.0.1/src/srtk/cli.py
--rw-r--r--   0        0        0     4006 2020-02-02 00:00:00.000000 srtk-0.0.1/src/srtk/link_wikidata.py
--rw-r--r--   0        0        0     5408 2020-02-02 00:00:00.000000 srtk-0.0.1/src/srtk/preprocess.py
--rw-r--r--   0        0        0    14019 2020-02-02 00:00:00.000000 srtk-0.0.1/src/srtk/retrieve.py
--rw-r--r--   0        0        0     5753 2020-02-02 00:00:00.000000 srtk-0.0.1/src/srtk/train.py
--rw-r--r--   0        0        0     4636 2020-02-02 00:00:00.000000 srtk-0.0.1/src/srtk/visualize.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 srtk-0.0.1/src/srtk/entity_linking/freebase.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 srtk-0.0.1/src/srtk/knowledge_graph/__init__.py
--rw-r--r--   0        0        0     8254 2020-02-02 00:00:00.000000 srtk-0.0.1/src/srtk/knowledge_graph/freebase.py
--rw-r--r--   0        0        0     2875 2020-02-02 00:00:00.000000 srtk-0.0.1/src/srtk/knowledge_graph/graph_base.py
--rw-r--r--   0        0        0    10620 2020-02-02 00:00:00.000000 srtk-0.0.1/src/srtk/knowledge_graph/wikidata.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 srtk-0.0.1/src/srtk/preprocessing/__init__.py
--rw-r--r--   0        0        0     2367 2020-02-02 00:00:00.000000 srtk-0.0.1/src/srtk/preprocessing/load_dataset.py
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 srtk-0.0.1/src/srtk/preprocessing/merge_ground.py
--rw-r--r--   0        0        0    10074 2020-02-02 00:00:00.000000 srtk-0.0.1/src/srtk/preprocessing/negative_sampling.py
--rw-r--r--   0        0        0     4081 2020-02-02 00:00:00.000000 srtk-0.0.1/src/srtk/preprocessing/score_path.py
--rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 srtk-0.0.1/src/srtk/preprocessing/search_path.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 srtk-0.0.1/src/srtk/scorer/__init__.py
--rw-r--r--   0        0        0     5052 2020-02-02 00:00:00.000000 srtk-0.0.1/src/srtk/scorer/encoder.py
--rw-r--r--   0        0        0     3211 2020-02-02 00:00:00.000000 srtk-0.0.1/src/srtk/scorer/scorer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 srtk-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 srtk-0.0.1/tests/test_encoder.py
--rw-r--r--   0        0        0     2991 2020-02-02 00:00:00.000000 srtk-0.0.1/tests/test_freebase.py
--rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 srtk-0.0.1/tests/test_scorer.py
--rw-r--r--   0        0        0     2617 2020-02-02 00:00:00.000000 srtk-0.0.1/tests/test_wikidata.py
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 srtk-0.0.1/tutorials/1.get_started.ipynb
--rw-r--r--   0        0        0    25547 2020-02-02 00:00:00.000000 srtk-0.0.1/tutorials/2.end_to_end_subgraph_retrieval.ipynb
--rw-r--r--   0        0        0    24937 2020-02-02 00:00:00.000000 srtk-0.0.1/tutorials/3.weak_train_wikidata.ipynb
--rw-r--r--   0        0        0    17127 2020-02-02 00:00:00.000000 srtk-0.0.1/tutorials/4.weak_train_freebase.ipynb
--rw-r--r--   0        0        0    22909 2020-02-02 00:00:00.000000 srtk-0.0.1/tutorials/5.supervised_train_wikidata.ipynb
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 srtk-0.0.1/tutorials/6.extend_to_new_kg.ipynb
--rw-r--r--   0        0        0     1954 2020-02-02 00:00:00.000000 srtk-0.0.1/.gitignore
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 srtk-0.0.1/LICENSE
--rw-r--r--   0        0        0     5156 2020-02-02 00:00:00.000000 srtk-0.0.1/README.md
--rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 srtk-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     5919 2020-02-02 00:00:00.000000 srtk-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     8300 2020-02-02 00:00:00.000000 srtk-0.0.2/graphs-for-paper.ipynb
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 srtk-0.0.2/requirements.txt
+-rw-r--r--   0        0        0     4679 2020-02-02 00:00:00.000000 srtk-0.0.2/sample_commands.ipynb
+-rw-r--r--   0        0        0    10348 2020-02-02 00:00:00.000000 srtk-0.0.2/test.pdf
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 srtk-0.0.2/train_qald.ipynb
+-rw-r--r--   0        0        0    23773 2020-02-02 00:00:00.000000 srtk-0.0.2/train_wd_simple.ipynb
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 srtk-0.0.2/.github/workflows/pytest.yml
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 srtk-0.0.2/resources/wikimapper/index_enwiki.db -> /home/wiss/liao/shen/flamingo-gnn/data/kilt/index_enwiki-latest-uncased.db
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 srtk-0.0.2/src/srtk/__init__.py
+-rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 srtk-0.0.2/src/srtk/cli.py
+-rw-r--r--   0        0        0     4201 2020-02-02 00:00:00.000000 srtk-0.0.2/src/srtk/link.py
+-rw-r--r--   0        0        0     5420 2020-02-02 00:00:00.000000 srtk-0.0.2/src/srtk/preprocess.py
+-rw-r--r--   0        0        0    14027 2020-02-02 00:00:00.000000 srtk-0.0.2/src/srtk/retrieve.py
+-rw-r--r--   0        0        0     5755 2020-02-02 00:00:00.000000 srtk-0.0.2/src/srtk/train.py
+-rw-r--r--   0        0        0     4646 2020-02-02 00:00:00.000000 srtk-0.0.2/src/srtk/visualize.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 srtk-0.0.2/src/srtk/entity_linking/freebase.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 srtk-0.0.2/src/srtk/knowledge_graph/__init__.py
+-rw-r--r--   0        0        0     8254 2020-02-02 00:00:00.000000 srtk-0.0.2/src/srtk/knowledge_graph/freebase.py
+-rw-r--r--   0        0        0     2875 2020-02-02 00:00:00.000000 srtk-0.0.2/src/srtk/knowledge_graph/graph_base.py
+-rw-r--r--   0        0        0    10620 2020-02-02 00:00:00.000000 srtk-0.0.2/src/srtk/knowledge_graph/wikidata.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 srtk-0.0.2/src/srtk/preprocessing/__init__.py
+-rw-r--r--   0        0        0     2367 2020-02-02 00:00:00.000000 srtk-0.0.2/src/srtk/preprocessing/load_dataset.py
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 srtk-0.0.2/src/srtk/preprocessing/merge_ground.py
+-rw-r--r--   0        0        0    10074 2020-02-02 00:00:00.000000 srtk-0.0.2/src/srtk/preprocessing/negative_sampling.py
+-rw-r--r--   0        0        0     4081 2020-02-02 00:00:00.000000 srtk-0.0.2/src/srtk/preprocessing/score_path.py
+-rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 srtk-0.0.2/src/srtk/preprocessing/search_path.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 srtk-0.0.2/src/srtk/scorer/__init__.py
+-rw-r--r--   0        0        0     5052 2020-02-02 00:00:00.000000 srtk-0.0.2/src/srtk/scorer/encoder.py
+-rw-r--r--   0        0        0     3211 2020-02-02 00:00:00.000000 srtk-0.0.2/src/srtk/scorer/scorer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 srtk-0.0.2/tests/__init__.py
+-rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 srtk-0.0.2/tests/test_encoder.py
+-rw-r--r--   0        0        0     2991 2020-02-02 00:00:00.000000 srtk-0.0.2/tests/test_freebase.py
+-rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 srtk-0.0.2/tests/test_scorer.py
+-rw-r--r--   0        0        0     2617 2020-02-02 00:00:00.000000 srtk-0.0.2/tests/test_wikidata.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 srtk-0.0.2/tutorials/1.get_started.ipynb
+-rw-r--r--   0        0        0    25547 2020-02-02 00:00:00.000000 srtk-0.0.2/tutorials/2.end_to_end_subgraph_retrieval.ipynb
+-rw-r--r--   0        0        0    24937 2020-02-02 00:00:00.000000 srtk-0.0.2/tutorials/3.weak_train_wikidata.ipynb
+-rw-r--r--   0        0        0    17127 2020-02-02 00:00:00.000000 srtk-0.0.2/tutorials/4.weak_train_freebase.ipynb
+-rw-r--r--   0        0        0    22909 2020-02-02 00:00:00.000000 srtk-0.0.2/tutorials/5.supervised_train_wikidata.ipynb
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 srtk-0.0.2/tutorials/6.extend_to_new_kg.ipynb
+-rw-r--r--   0        0        0     1954 2020-02-02 00:00:00.000000 srtk-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 srtk-0.0.2/LICENSE
+-rw-r--r--   0        0        0     5374 2020-02-02 00:00:00.000000 srtk-0.0.2/README.md
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 srtk-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     6187 2020-02-02 00:00:00.000000 srtk-0.0.2/PKG-INFO
```

### Comparing `srtk-0.0.1/test.pdf` & `srtk-0.0.2/test.pdf`

 * *Files identical despite different names*

### Comparing `srtk-0.0.1/train_qald.ipynb` & `srtk-0.0.2/train_qald.ipynb`

 * *Files identical despite different names*

### Comparing `srtk-0.0.1/train_wd_simple.ipynb` & `srtk-0.0.2/train_wd_simple.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9954749103942653%*

 * *Differences: {"'cells'": "{11: {'execution_count': 3}, 23: {'source': {insert: [(7, '    --max-epochs 20')], "*

 * *            "delete: [7]}}, insert: [(15, OrderedDict([('cell_type', 'code'), ('execution_count', "*

 * *            "4), ('metadata', OrderedDict()), ('outputs', [OrderedDict([('name', 'stdout'), "*

 * *            "('output_type', 'stream'), ('text', ['Number of entities: 26688\\n', 'Number of "*

 * *            "relations: 75\\n'])])]), ('source', ['entity_set = set()\\n', 'relation_set = "*

 * *            "set()\\n', 'for spl […]*

```diff
@@ -131,15 +131,15 @@
             "metadata": {},
             "source": [
                 "### 1.2 Remove reverse relations"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
+            "execution_count": 3,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
                         "Full train size: 19481\n",
@@ -231,14 +231,43 @@
                 "        samples.append(sample)\n",
                 "    save_path = os.path.join(intermediate_dir, f'scores_{split}.jsonl')\n",
                 "    srsly.write_jsonl(save_path, samples)\n",
                 "    print(f'Saved {split} scored paths file to {save_path}')"
             ]
         },
         {
+            "cell_type": "code",
+            "execution_count": 4,
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "Number of entities: 26688\n",
+                        "Number of relations: 75\n"
+                    ]
+                }
+            ],
+            "source": [
+                "entity_set = set()\n",
+                "relation_set = set()\n",
+                "for split in splits:\n",
+                "    data = preserved_data[split]\n",
+                "    samples = []\n",
+                "    for idx, line in enumerate(data.values):\n",
+                "        question_entity, relation, answer_entity, question = line\n",
+                "        entity_set.add(question_entity)\n",
+                "        entity_set.add(answer_entity)\n",
+                "        relation_set.add(relation)\n",
+                "print(f'Number of entities: {len(entity_set)}')\n",
+                "print(f'Number of relations: {len(relation_set)}')"
+            ]
+        },
+        {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Step 2. Preprocessing\n",
                 "\n",
                 "Use the `srtk preprocess` command to creating training samples. Do not pass `--search-path` beacuse the paths are already provided in the dataset. This step mainly involves negative sampling and dataset generation."
@@ -414,15 +443,15 @@
                 "!CUDA_VISIBLE_DEVICES=3 srtk train -t data/wikidata-simplequestions/dataset/train.jsonl \\\n",
                 "    -v data/wikidata-simplequestions/dataset/valid.jsonl \\\n",
                 "    --model-name-or-path roberta-base \\\n",
                 "    --output-dir artifacts/models/wd_simple_e10 \\\n",
                 "    --accelerator gpu \\\n",
                 "    --learning-rate 1e-5 \\\n",
                 "    --batch-size 96 \\\n",
-                "    --max-epochs 10"
+                "    --max-epochs 20"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
```

### Comparing `srtk-0.0.1/.github/workflows/pytest.yml` & `srtk-0.0.2/.github/workflows/pytest.yml`

 * *Files identical despite different names*

### Comparing `srtk-0.0.1/src/srtk/cli.py` & `srtk-0.0.2/src/srtk/cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 """Command-line interface for SRTK."""
 import argparse
 
-from .link_wikidata import add_arguments as add_link_wikidata_arguments
-from .link_wikidata import main as link_wikidata
+from .link import add_arguments as add_link_wikidata_arguments
+from .link import link
 from .preprocess import add_arguments as add_preprocess_arguments
-from .preprocess import main as preprocess
+from .preprocess import preprocess
 from .retrieve import add_arguments as add_retrieve_arguments
-from .retrieve import main as retrieve
+from .retrieve import retrieve
 from .train import add_arguments as add_train_arguments
-from .train import main as train
+from .train import train
 from .visualize import add_arguments as add_visualize_arguments
-from .visualize import main as visualize
+from .visualize import visualize
 
 
 def main():
+    """Main entry to the command line interface.
+    """
     parser = argparse.ArgumentParser(description='SRTK: A toolkit for smantic-relevant subgraph retrieval')
     subparsers = parser.add_subparsers(help='sub-command help')
 
-    parser_link_wikidata = subparsers.add_parser('link-wikidata', help='link entities to Wikidata')
+    parser_link_wikidata = subparsers.add_parser('link', help='link entities to a knowledge graph')
     add_link_wikidata_arguments(parser_link_wikidata)
-    parser_link_wikidata.set_defaults(func=link_wikidata)
+    parser_link_wikidata.set_defaults(func=link)
 
     parser_preprocess = subparsers.add_parser('preprocess', help='preprocess the data')
     add_preprocess_arguments(parser_preprocess)
     parser_preprocess.set_defaults(func=preprocess)
 
     parser_train = subparsers.add_parser('train', help='train a subgraph retriever')
     add_train_arguments(parser_train)
```

### Comparing `srtk-0.0.1/src/srtk/link_wikidata.py` & `srtk-0.0.2/src/srtk/link.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         s.close()
         return True
     except Exception as err:
         print(err)
         return False
 
 
-def main(args):
+def link(args):
     try:
         host = args.el_endpoint.split(':')[-2].split('/')[-1]
         port = int(args.el_endpoint.split(':')[-1])
     except Exception as exc:
         raise ValueError(f"Can't parse the endpoint {args.el_endpoint}") from exc
     if not socket_reachable(host, port):
         raise RuntimeError(f"Can't reach the endpoint {args.el_endpoint}")
@@ -88,16 +88,18 @@
     parser.description = '''Entity linking on Wikidata.
     The input is a jsonl file. The field of interest is specified by the argument --ground-on.
     The output is a jsonl file, each line is a dict with keys: id, question_entities, spans, entity_names.
     '''
     parser.add_argument('-i', '--input', type=str, help='Input file path, in which the question is stored')
     parser.add_argument('-o', '--output', type=str, help='Output file path, in which the entity linking result is stored')
     parser.add_argument('-e', '--el-endpoint', type=str, default='http://127.0.0.1:1235', help='REL endpoint')
+    parser.add_argument('-kg', '--knowledge-graph', type=str, default='wikidata', choices=['wikidata'],
+                        help='Knowledge graph to link to, only wikidata is supported now')
     parser.add_argument('--wikimapper-db', type=str, default='resources/wikimapper/index_enwiki.db', help='Wikimapper database path')
     parser.add_argument('--ground-on', type=str, default='question', help='The key to ground on, the corresponding text will be sent to the REL endpoint for entity linking')
     
 
 if __name__ == '__main__':
     parser = argparse.ArgumentParser()
     add_arguments(parser)
     args = parser.parse_args()
-    main(args)
+    link(args)
```

### Comparing `srtk-0.0.1/src/srtk/preprocess.py` & `srtk-0.0.2/src/srtk/preprocess.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from pathlib import Path
 
 from .preprocessing.search_path import main as search_path
 from .preprocessing.score_path import main as score_path
 from .preprocessing.negative_sampling import main as negative_sampling
 
 
-def main(args):
+def preprocess(args):
     output_path = args.output
     # Create parent dir for output if not exists.
     Path(os.path.dirname(output_path)).mkdir(parents=True, exist_ok=True)
     if args.search_path:
         intermediate_dir = args.intermediate_dir
         if intermediate_dir is None:
             intermediate_dir = os.path.dirname(output_path)
@@ -93,8 +93,8 @@
                         a larger training dataset, you can set this value to a smaller value. (default: 0.5)')
 
 
 if __name__ == '__main__':
     parser = argparse.ArgumentParser()
     add_arguments(parser)
     args = parser.parse_args()
-    main(args)
+    preprocess(args)
```

### Comparing `srtk-0.0.1/src/srtk/retrieve.py` & `srtk-0.0.2/src/srtk/retrieve.py`

 * *Files 1% similar despite different names*

```diff
@@ -240,15 +240,15 @@
             'recall': hit / (hit + miss)
         }
     # path/to/subgraph.jsonl -> path/to/subgraph.metric
     recall_path = os.path.splitext(retrieved_path)[0] + '.metric'
     srsly.write_json(recall_path, info)
 
 
-def main(args):
+def retrieve(args):
     pathlib.Path(os.path.dirname(args.output)).mkdir(parents=True, exist_ok=True)
     if args.knowledge_graph == 'freebase':
         kg = Freebase(args.sparql_endpoint)
     else:
         kg = Wikidata(args.sparql_endpoint, exclude_qualifiers=not args.include_qualifiers)
     device = torch.device('cuda' if torch.cuda.is_available() else 'cpu')
     scorer = Scorer(args.scorer_model_path, device)
@@ -305,8 +305,8 @@
     args = parser.parse_args()
     if not args.sparql_endpoint:
         if args.knowledge_graph == 'freebase':
             args.sparql_endpoint = 'http://localhost:3001/sparql'
         else:
             args.sparql_endpoint = 'http://localhost:1234/api/endpoint/sparql'
         print(f'Using default sparql endpoint for {args.knowledge_graph}: {args.sparql_endpoint}')
-    main(args)
+    retrieve(args)
```

### Comparing `srtk-0.0.1/src/srtk/train.py` & `srtk-0.0.2/src/srtk/train.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     validation_dataset = validation_dataset.map(concate_all, remove_columns=validation_dataset.column_names)
     validation_dataset = validation_dataset.map(tokenize, remove_columns=validation_dataset.column_names)
     train_loader = DataLoader(train_dataset, batch_size=batch_size, shuffle=True, collate_fn=Collator(tokenizer), num_workers=8)
     validation_loader = DataLoader(validation_dataset, batch_size=batch_size, shuffle=False, collate_fn=Collator(tokenizer), num_workers=8)
     return train_loader, validation_loader
 
 
-def main(args):
+def train(args):
     torch.set_float32_matmul_precision('medium')
     model = LitSentenceEncoder(args.model_name_or_path, lr=args.learning_rate)
     tokenizer = AutoTokenizer.from_pretrained(args.model_name_or_path)
     train_loader, validation_loader = prepare_dataloaders(args.train_dataset, args.validation_dataset, tokenizer, args.batch_size)
     day_hour = datetime.datetime.now().strftime('%m%d%H%M')
     wandb_logger = WandbLogger(project='retrieval', name=day_hour , group='contrastive', save_dir='artifacts')
     trainer = pl.Trainer(accelerator=args.accelerator, default_root_dir=args.output_dir,
@@ -106,8 +106,8 @@
                         help='fast dev run for debugging, only use 1 batch for training and validation')
 
 if __name__ == '__main__':
     parser = argparse.ArgumentParser()
     add_arguments(parser)
     args = parser.parse_args()
 
-    main(args)
+    train(args)
```

### Comparing `srtk-0.0.1/src/srtk/visualize.py` & `srtk-0.0.2/src/srtk/visualize.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     soup.head.append(style_tag)
     p_tag = soup.new_tag('p', attrs={'class': 'background-text'}, style="white-space:pre-wrap")
     p_tag.string = text
     soup.body.append(p_tag)
     return soup.prettify()
     
 
-def main(args):
+def visualize(args):
     if args.knowledge_graph == 'wikidata':
         knowledge_graph = Wikidata(args.sparql_endpoint)
     else:
         knowledge_graph = Freebase(args.sparql_endpoint)
     samples = srsly.read_jsonl(args.input)
     total = sum(1 for _ in srsly.read_jsonl(args.input))
     total = min(total, args.max_output)
@@ -107,8 +107,8 @@
                         help='The maximum number of graphs to output. This is useful for debugging. (Default: 1000)')
 
 
 if __name__ == '__main__':
     parser = argparse.ArgumentParser()
     add_arguments(parser)
     args = parser.parse_args()
-    main(args)
+    visualize(args)
```

### Comparing `srtk-0.0.1/src/srtk/knowledge_graph/freebase.py` & `srtk-0.0.2/src/srtk/knowledge_graph/freebase.py`

 * *Files identical despite different names*

### Comparing `srtk-0.0.1/src/srtk/knowledge_graph/graph_base.py` & `srtk-0.0.2/src/srtk/knowledge_graph/graph_base.py`

 * *Files identical despite different names*

### Comparing `srtk-0.0.1/src/srtk/knowledge_graph/wikidata.py` & `srtk-0.0.2/src/srtk/knowledge_graph/wikidata.py`

 * *Files identical despite different names*

### Comparing `srtk-0.0.1/src/srtk/preprocessing/load_dataset.py` & `srtk-0.0.2/src/srtk/preprocessing/load_dataset.py`

 * *Files identical despite different names*

### Comparing `srtk-0.0.1/src/srtk/preprocessing/merge_ground.py` & `srtk-0.0.2/src/srtk/preprocessing/merge_ground.py`

 * *Files identical despite different names*

### Comparing `srtk-0.0.1/src/srtk/preprocessing/negative_sampling.py` & `srtk-0.0.2/src/srtk/preprocessing/negative_sampling.py`

 * *Files identical despite different names*

### Comparing `srtk-0.0.1/src/srtk/preprocessing/score_path.py` & `srtk-0.0.2/src/srtk/preprocessing/score_path.py`

 * *Files identical despite different names*

### Comparing `srtk-0.0.1/src/srtk/preprocessing/search_path.py` & `srtk-0.0.2/src/srtk/preprocessing/search_path.py`

 * *Files identical despite different names*

### Comparing `srtk-0.0.1/src/srtk/scorer/encoder.py` & `srtk-0.0.2/src/srtk/scorer/encoder.py`

 * *Files identical despite different names*

### Comparing `srtk-0.0.1/src/srtk/scorer/scorer.py` & `srtk-0.0.2/src/srtk/scorer/scorer.py`

 * *Files identical despite different names*

### Comparing `srtk-0.0.1/tests/test_encoder.py` & `srtk-0.0.2/tests/test_encoder.py`

 * *Files identical despite different names*

### Comparing `srtk-0.0.1/tests/test_freebase.py` & `srtk-0.0.2/tests/test_freebase.py`

 * *Files identical despite different names*

### Comparing `srtk-0.0.1/tests/test_scorer.py` & `srtk-0.0.2/tests/test_scorer.py`

 * *Files identical despite different names*

### Comparing `srtk-0.0.1/tests/test_wikidata.py` & `srtk-0.0.2/tests/test_wikidata.py`

 * *Files identical despite different names*

### Comparing `srtk-0.0.1/tutorials/1.get_started.ipynb` & `srtk-0.0.2/tutorials/1.get_started.ipynb`

 * *Files identical despite different names*

### Comparing `srtk-0.0.1/tutorials/2.end_to_end_subgraph_retrieval.ipynb` & `srtk-0.0.2/tutorials/2.end_to_end_subgraph_retrieval.ipynb`

 * *Files identical despite different names*

### Comparing `srtk-0.0.1/tutorials/3.weak_train_wikidata.ipynb` & `srtk-0.0.2/tutorials/3.weak_train_wikidata.ipynb`

 * *Files identical despite different names*

### Comparing `srtk-0.0.1/tutorials/4.weak_train_freebase.ipynb` & `srtk-0.0.2/tutorials/4.weak_train_freebase.ipynb`

 * *Files identical despite different names*

### Comparing `srtk-0.0.1/tutorials/5.supervised_train_wikidata.ipynb` & `srtk-0.0.2/tutorials/5.supervised_train_wikidata.ipynb`

 * *Files identical despite different names*

### Comparing `srtk-0.0.1/.gitignore` & `srtk-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `srtk-0.0.1/LICENSE` & `srtk-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `srtk-0.0.1/README.md` & `srtk-0.0.2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # Subgraph Retrieval Toolkit
 
+[![PyPi](https://img.shields.io/pypi/v/srtk)](https://pypi.org/project/srtk/)
+[![Documentation Status](https://readthedocs.org/projects/srtk/badge/?version=latest)](https://srtk.readthedocs.io/en/latest/?badge=latest)
 [![PytestStatus](https://github.com/happen2me/subgraph-retrieval-wikidata/actions/workflows/pytest.yml/badge.svg)](https://github.com/happen2me/subgraph-retrieval-toolkit/actions/workflows/pytest.yml)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 Retrieve subgraphs on Wikidata. The method is based on this [retrieval work](https://github.com/RUCKBReasoning/SubgraphRetrievalKBQA) for Freebase.
 
 ## Prerequisite
```

### Comparing `srtk-0.0.1/pyproject.toml` & `srtk-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling", "hatch-requirements-txt"]
 build-backend = "hatchling.build"
 
 [project]
 name = "srtk"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Yuanchun Shen", email="y.c.shen@tum.de" },
 ]
 description = "A toolkit for semantic-relevant subgraph retrieval from large-scale knowledge graphs."
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `srtk-0.0.1/PKG-INFO` & `srtk-0.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 Metadata-Version: 2.1
 Name: srtk
-Version: 0.0.1
+Version: 0.0.2
 Summary: A toolkit for semantic-relevant subgraph retrieval from large-scale knowledge graphs.
 Project-URL: Homepage, https://github.com/happen2me/subgraph-retrieval-toolkit
 Project-URL: Bug Tracker, https://github.com/happen2me/subgraph-retrieval-toolkit/issues
 Author-email: Yuanchun Shen <y.c.shen@tum.de>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Requires-Dist: beautifulsoup4
+Requires-Dist: datasets
 Requires-Dist: lightning
 Requires-Dist: pyvis
 Requires-Dist: sparqlwrapper
 Requires-Dist: srsly
 Requires-Dist: tqdm
 Requires-Dist: transformers
+Requires-Dist: wikimapper
 Description-Content-Type: text/markdown
 
 # Subgraph Retrieval Toolkit
 
+[![PyPi](https://img.shields.io/pypi/v/srtk)](https://pypi.org/project/srtk/)
+[![Documentation Status](https://readthedocs.org/projects/srtk/badge/?version=latest)](https://srtk.readthedocs.io/en/latest/?badge=latest)
 [![PytestStatus](https://github.com/happen2me/subgraph-retrieval-wikidata/actions/workflows/pytest.yml/badge.svg)](https://github.com/happen2me/subgraph-retrieval-toolkit/actions/workflows/pytest.yml)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 Retrieve subgraphs on Wikidata. The method is based on this [retrieval work](https://github.com/RUCKBReasoning/SubgraphRetrievalKBQA) for Freebase.
 
 ## Prerequisite
```

