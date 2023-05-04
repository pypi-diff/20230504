# Comparing `tmp/ontogpt-0.2.3.tar.gz` & `tmp/ontogpt-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ontogpt-0.2.3.tar", max compression
+gzip compressed data, was "ontogpt-0.2.4.tar", max compression
```

## Comparing `ontogpt-0.2.3.tar` & `ontogpt-0.2.4.tar`

### file list

```diff
@@ -1,102 +1,107 @@
--rw-r--r--   0        0        0     1485 2023-05-02 00:11:00.168373 ontogpt-0.2.3/LICENSE
--rw-r--r--   0        0        0    11172 2023-05-02 00:11:00.168373 ontogpt-0.2.3/README.md
--rw-r--r--   0        0        0     2330 2023-05-02 00:12:03.172317 ontogpt-0.2.3/pyproject.toml
--rw-r--r--   0        0        0      219 2023-05-02 00:11:00.200373 ontogpt-0.2.3/src/ontogpt/__init__.py
--rw-r--r--   0        0        0    32137 2023-05-02 00:11:00.200373 ontogpt-0.2.3/src/ontogpt/cli.py
--rw-r--r--   0        0        0      244 2023-05-02 00:11:00.200373 ontogpt-0.2.3/src/ontogpt/clients/__init__.py
--rw-r--r--   0        0        0     6962 2023-05-02 00:11:00.200373 ontogpt-0.2.3/src/ontogpt/clients/openai_client.py
--rw-r--r--   0        0        0     2921 2023-05-02 00:11:00.200373 ontogpt-0.2.3/src/ontogpt/clients/pubmed_client.py
--rw-r--r--   0        0        0      617 2023-05-02 00:11:00.200373 ontogpt-0.2.3/src/ontogpt/clients/soup_client.py
--rw-r--r--   0        0        0     1122 2023-05-02 00:11:00.200373 ontogpt-0.2.3/src/ontogpt/clients/wikipedia_client.py
--rw-r--r--   0        0        0      684 2023-05-02 00:11:00.200373 ontogpt-0.2.3/src/ontogpt/conf/synonymizer-conf.yaml
--rw-r--r--   0        0        0       81 2023-05-02 00:11:00.200373 ontogpt-0.2.3/src/ontogpt/converters/__init__.py
--rw-r--r--   0        0        0     5289 2023-05-02 00:11:00.200373 ontogpt-0.2.3/src/ontogpt/converters/ontology_converter.py
--rw-r--r--   0        0        0       59 2023-05-02 00:11:00.200373 ontogpt-0.2.3/src/ontogpt/engines/__init__.py
--rw-r--r--   0        0        0     3748 2023-05-02 00:11:00.200373 ontogpt-0.2.3/src/ontogpt/engines/embedding_similarity_engine.py
--rw-r--r--   0        0        0    11314 2023-05-02 00:11:00.200373 ontogpt-0.2.3/src/ontogpt/engines/enrichment.py
--rw-r--r--   0        0        0    19185 2023-05-02 00:11:00.200373 ontogpt-0.2.3/src/ontogpt/engines/halo_engine.py
--rw-r--r--   0        0        0    23173 2023-05-02 00:11:00.200373 ontogpt-0.2.3/src/ontogpt/engines/knowledge_engine.py
--rw-r--r--   0        0        0      752 2023-05-02 00:11:00.200373 ontogpt-0.2.3/src/ontogpt/engines/resolver.py
--rw-r--r--   0        0        0    17537 2023-05-02 00:11:00.200373 ontogpt-0.2.3/src/ontogpt/engines/spires_engine.py
--rw-r--r--   0        0        0      719 2023-05-02 00:11:00.200373 ontogpt-0.2.3/src/ontogpt/engines/synonym_engine.py
--rw-r--r--   0        0        0       70 2023-05-02 00:11:00.200373 ontogpt-0.2.3/src/ontogpt/evaluation/__init__.py
--rw-r--r--   0        0        0        0 2023-05-02 00:11:00.204373 ontogpt-0.2.3/src/ontogpt/evaluation/ctd/__init__.py
--rw-r--r--   0        0        0   425228 2023-05-02 00:11:00.204373 ontogpt-0.2.3/src/ontogpt/evaluation/ctd/database/CDR_TestSet.BioC.xml.gz
--rw-r--r--   0        0        0   409439 2023-05-02 00:11:00.204373 ontogpt-0.2.3/src/ontogpt/evaluation/ctd/database/CDR_TrainSet.BioC.xml.gz
--rw-r--r--   0        0        0   413985 2023-05-02 00:11:00.204373 ontogpt-0.2.3/src/ontogpt/evaluation/ctd/database/synonyms.yaml
--rw-r--r--   0        0        0    10390 2023-05-02 00:11:00.204373 ontogpt-0.2.3/src/ontogpt/evaluation/ctd/eval_ctd.py
--rw-r--r--   0        0        0        0 2023-05-02 00:11:00.204373 ontogpt-0.2.3/src/ontogpt/evaluation/drugmechdb/__init__.py
--rw-r--r--   0        0        0     2145 2023-05-02 00:11:00.204373 ontogpt-0.2.3/src/ontogpt/evaluation/drugmechdb/datamodel/drugmechdb.py
--rw-r--r--   0        0        0     2027 2023-05-02 00:11:00.204373 ontogpt-0.2.3/src/ontogpt/evaluation/drugmechdb/datamodel/drugmechdb.yaml
--rw-r--r--   0        0        0    10670 2023-05-02 00:11:00.204373 ontogpt-0.2.3/src/ontogpt/evaluation/drugmechdb/eval_drugmechdb.py
--rw-r--r--   0        0        0        0 2023-05-02 00:11:00.204373 ontogpt-0.2.3/src/ontogpt/evaluation/enrichment/__init__.py
--rw-r--r--   0        0        0    13318 2023-05-02 00:11:00.204373 ontogpt-0.2.3/src/ontogpt/evaluation/enrichment/eval_enrichment.py
--rw-r--r--   0        0        0     2950 2023-05-02 00:11:00.204373 ontogpt-0.2.3/src/ontogpt/evaluation/evaluation_engine.py
--rw-r--r--   0        0        0     6164 2023-05-02 00:11:00.204373 ontogpt-0.2.3/src/ontogpt/evaluation/go/eval_go.py
--rw-r--r--   0        0        0        0 2023-05-02 00:11:00.204373 ontogpt-0.2.3/src/ontogpt/evaluation/hpoa/__init__.py
--rw-r--r--   0        0        0     8973 2023-05-02 00:11:00.204373 ontogpt-0.2.3/src/ontogpt/evaluation/hpoa/eval_hpoa.py
--rw-r--r--   0        0        0     1191 2023-05-02 00:11:00.204373 ontogpt-0.2.3/src/ontogpt/evaluation/ibd/PMC6386158_fig2_legend.txt
--rw-r--r--   0        0        0        0 2023-05-02 00:11:00.204373 ontogpt-0.2.3/src/ontogpt/evaluation/ibd/PMC6386158_fig2_legend.txt~
--rw-r--r--   0        0        0     4791 2023-05-02 00:11:00.204373 ontogpt-0.2.3/src/ontogpt/evaluation/ibd/PMC6386158_fig2_legend.yaml
--rwxr-xr-x   0        0        0       95 2023-05-02 00:11:00.204373 ontogpt-0.2.3/src/ontogpt/evaluation/ibd/run.sh
--rwxr-xr-x   0        0        0       99 2023-05-02 00:11:00.204373 ontogpt-0.2.3/src/ontogpt/evaluation/ibd/run.sh~
--rw-r--r--   0        0        0      586 2023-05-02 00:11:00.204373 ontogpt-0.2.3/src/ontogpt/evaluation/resolver.py
--rw-r--r--   0        0        0        0 2023-05-02 00:11:00.204373 ontogpt-0.2.3/src/ontogpt/io/__init__.py
--rw-r--r--   0        0        0      386 2023-05-02 00:11:00.204373 ontogpt-0.2.3/src/ontogpt/io/exporter.py
--rw-r--r--   0        0        0     4329 2023-05-02 00:11:00.204373 ontogpt-0.2.3/src/ontogpt/io/html_exporter.py
--rw-r--r--   0        0        0     3255 2023-05-02 00:11:00.204373 ontogpt-0.2.3/src/ontogpt/io/markdown_exporter.py
--rw-r--r--   0        0        0     2350 2023-05-02 00:11:00.204373 ontogpt-0.2.3/src/ontogpt/io/owl_exporter.py
--rw-r--r--   0        0        0     1440 2023-05-02 00:11:00.204373 ontogpt-0.2.3/src/ontogpt/io/rdf_exporter.py
--rw-r--r--   0        0        0      899 2023-05-02 00:11:00.204373 ontogpt-0.2.3/src/ontogpt/io/yaml_wrapper.py
--rw-r--r--   0        0        0        0 2023-05-02 00:11:00.204373 ontogpt-0.2.3/src/ontogpt/prompts/__init__.py
--rw-r--r--   0        0        0      159 2023-05-02 00:11:00.204373 ontogpt-0.2.3/src/ontogpt/prompts/enrichment/__init__.py
--rw-r--r--   0        0        0     1079 2023-05-02 00:11:00.204373 ontogpt-0.2.3/src/ontogpt/prompts/enrichment/gene_set_summarization.jinja2
--rw-r--r--   0        0        0      993 2023-05-02 00:11:00.204373 ontogpt-0.2.3/src/ontogpt/prompts/enrichment/gene_set_summarization_with_p_values.jinja2
--rw-r--r--   0        0        0      560 2023-05-02 00:11:00.204373 ontogpt-0.2.3/src/ontogpt/prompts/similarity/connections.jinja2
--rw-r--r--   0        0        0       68 2023-05-02 00:11:00.204373 ontogpt-0.2.3/src/ontogpt/templates/__init__.py
--rw-r--r--   0        0        0      401 2023-05-02 00:11:00.204373 ontogpt-0.2.3/src/ontogpt/templates/all.yaml
--rw-r--r--   0        0        0     5942 2023-05-02 00:11:00.204373 ontogpt-0.2.3/src/ontogpt/templates/biological_process.py
--rw-r--r--   0        0        0     2027 2023-05-02 00:11:00.204373 ontogpt-0.2.3/src/ontogpt/templates/biological_process.yaml
--rw-r--r--   0        0        0     2938 2023-05-02 00:11:00.208373 ontogpt-0.2.3/src/ontogpt/templates/class_enrichment.py
--rw-r--r--   0        0        0     3192 2023-05-02 00:11:00.208373 ontogpt-0.2.3/src/ontogpt/templates/class_enrichment.yaml
--rw-r--r--   0        0        0     3593 2023-05-02 00:11:00.208373 ontogpt-0.2.3/src/ontogpt/templates/core.py
--rw-r--r--   0        0        0     3098 2023-05-02 00:11:00.208373 ontogpt-0.2.3/src/ontogpt/templates/core.yaml
--rw-r--r--   0        0        0     6210 2023-05-02 00:11:00.208373 ontogpt-0.2.3/src/ontogpt/templates/ctd.py
--rw-r--r--   0        0        0     6683 2023-05-02 00:11:00.208373 ontogpt-0.2.3/src/ontogpt/templates/ctd.yaml
--rw-r--r--   0        0        0     5466 2023-05-02 00:11:00.208373 ontogpt-0.2.3/src/ontogpt/templates/drug.py
--rw-r--r--   0        0        0     1856 2023-05-02 00:11:00.208373 ontogpt-0.2.3/src/ontogpt/templates/drug.yaml
--rw-r--r--   0        0        0     6092 2023-05-02 00:11:00.208373 ontogpt-0.2.3/src/ontogpt/templates/environmental_sample.py
--rw-r--r--   0        0        0     2880 2023-05-02 00:11:00.208373 ontogpt-0.2.3/src/ontogpt/templates/environmental_sample.yaml
--rw-r--r--   0        0        0     4709 2023-05-02 00:11:00.208373 ontogpt-0.2.3/src/ontogpt/templates/gene_description_term.py
--rw-r--r--   0        0        0     1614 2023-05-02 00:11:00.208373 ontogpt-0.2.3/src/ontogpt/templates/gene_description_term.yaml
--rw-r--r--   0        0        0     8172 2023-05-02 00:11:00.208373 ontogpt-0.2.3/src/ontogpt/templates/gocam.py
--rw-r--r--   0        0        0     4871 2023-05-02 00:11:00.208373 ontogpt-0.2.3/src/ontogpt/templates/gocam.yaml
--rw-r--r--   0        0        0     6813 2023-05-02 00:11:00.208373 ontogpt-0.2.3/src/ontogpt/templates/halo.py
--rw-r--r--   0        0        0     2367 2023-05-02 00:11:00.208373 ontogpt-0.2.3/src/ontogpt/templates/halo.yaml
--rw-r--r--   0        0        0     8165 2023-05-02 00:11:00.208373 ontogpt-0.2.3/src/ontogpt/templates/ibd.py
--rw-r--r--   0        0        0     4869 2023-05-02 00:11:00.208373 ontogpt-0.2.3/src/ontogpt/templates/ibd.yaml
--rw-r--r--   0        0        0     6097 2023-05-02 00:11:00.208373 ontogpt-0.2.3/src/ontogpt/templates/mendelian_disease.py
--rw-r--r--   0        0        0     3130 2023-05-02 00:11:00.208373 ontogpt-0.2.3/src/ontogpt/templates/mendelian_disease.yaml
--rw-r--r--   0        0        0     5384 2023-05-02 00:11:00.208373 ontogpt-0.2.3/src/ontogpt/templates/metabolic_process.py
--rw-r--r--   0        0        0     1633 2023-05-02 00:11:00.208373 ontogpt-0.2.3/src/ontogpt/templates/metabolic_process.yaml
--rw-r--r--   0        0        0     7156 2023-05-02 00:11:00.208373 ontogpt-0.2.3/src/ontogpt/templates/metagenome_study.py
--rw-r--r--   0        0        0     3910 2023-05-02 00:11:00.208373 ontogpt-0.2.3/src/ontogpt/templates/metagenome_study.yaml
--rw-r--r--   0        0        0     5072 2023-05-02 00:11:00.208373 ontogpt-0.2.3/src/ontogpt/templates/ontology_class.py
--rw-r--r--   0        0        0     2686 2023-05-02 00:11:00.208373 ontogpt-0.2.3/src/ontogpt/templates/ontology_class.yaml
--rw-r--r--   0        0        0     4887 2023-05-02 00:11:00.208373 ontogpt-0.2.3/src/ontogpt/templates/phenotype.py
--rw-r--r--   0        0        0     1532 2023-05-02 00:11:00.208373 ontogpt-0.2.3/src/ontogpt/templates/phenotype.yaml
--rw-r--r--   0        0        0     7501 2023-05-02 00:11:00.208373 ontogpt-0.2.3/src/ontogpt/templates/reaction.py
--rw-r--r--   0        0        0     3187 2023-05-02 00:11:00.208373 ontogpt-0.2.3/src/ontogpt/templates/reaction.yaml
--rw-r--r--   0        0        0     7222 2023-05-02 00:11:00.208373 ontogpt-0.2.3/src/ontogpt/templates/recipe.py
--rw-r--r--   0        0        0     5792 2023-05-02 00:11:00.208373 ontogpt-0.2.3/src/ontogpt/templates/recipe.yaml
--rw-r--r--   0        0        0     7847 2023-05-02 00:11:00.208373 ontogpt-0.2.3/src/ontogpt/templates/treatment.py
--rw-r--r--   0        0        0     4485 2023-05-02 00:11:00.208373 ontogpt-0.2.3/src/ontogpt/templates/treatment.yaml
--rw-r--r--   0        0        0        0 2023-05-02 00:11:00.208373 ontogpt-0.2.3/src/ontogpt/utils/__init__.py
--rw-r--r--   0        0        0     5708 2023-05-02 00:11:00.208373 ontogpt-0.2.3/src/ontogpt/utils/gene_set_utils.py
--rw-r--r--   0        0        0        0 2023-05-02 00:11:00.208373 ontogpt-0.2.3/src/ontogpt/webapp/__init__.py
--rw-r--r--   0        0        0      861 2023-05-02 00:11:00.208373 ontogpt-0.2.3/src/ontogpt/webapp/html/form.html
--rw-r--r--   0        0        0      201 2023-05-02 00:11:00.208373 ontogpt-0.2.3/src/ontogpt/webapp/html/results.html
--rw-r--r--   0        0        0      819 2023-05-02 00:11:00.208373 ontogpt-0.2.3/src/ontogpt/webapp/html/spindoctor/form.html
--rw-r--r--   0        0        0      205 2023-05-02 00:11:00.208373 ontogpt-0.2.3/src/ontogpt/webapp/html/spindoctor/results.html
--rw-r--r--   0        0        0     2722 2023-05-02 00:11:00.208373 ontogpt-0.2.3/src/ontogpt/webapp/main.py
--rw-r--r--   0        0        0    13422 1970-01-01 00:00:00.000000 ontogpt-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0     1485 2023-05-04 00:13:25.772353 ontogpt-0.2.4/LICENSE
+-rw-r--r--   0        0        0    11172 2023-05-04 00:13:25.772353 ontogpt-0.2.4/README.md
+-rw-r--r--   0        0        0     2356 2023-05-04 00:14:29.715690 ontogpt-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0      219 2023-05-04 00:13:25.952350 ontogpt-0.2.4/src/ontogpt/__init__.py
+-rw-r--r--   0        0        0    32662 2023-05-04 00:13:25.952350 ontogpt-0.2.4/src/ontogpt/cli.py
+-rw-r--r--   0        0        0      244 2023-05-04 00:13:25.952350 ontogpt-0.2.4/src/ontogpt/clients/__init__.py
+-rw-r--r--   0        0        0     6962 2023-05-04 00:13:25.952350 ontogpt-0.2.4/src/ontogpt/clients/openai_client.py
+-rw-r--r--   0        0        0     2921 2023-05-04 00:13:25.952350 ontogpt-0.2.4/src/ontogpt/clients/pubmed_client.py
+-rw-r--r--   0        0        0      617 2023-05-04 00:13:25.952350 ontogpt-0.2.4/src/ontogpt/clients/soup_client.py
+-rw-r--r--   0        0        0     1122 2023-05-04 00:13:25.952350 ontogpt-0.2.4/src/ontogpt/clients/wikipedia_client.py
+-rw-r--r--   0        0        0      684 2023-05-04 00:13:25.952350 ontogpt-0.2.4/src/ontogpt/conf/synonymizer-conf.yaml
+-rw-r--r--   0        0        0       81 2023-05-04 00:13:25.952350 ontogpt-0.2.4/src/ontogpt/converters/__init__.py
+-rw-r--r--   0        0        0     5289 2023-05-04 00:13:25.952350 ontogpt-0.2.4/src/ontogpt/converters/ontology_converter.py
+-rw-r--r--   0        0        0       59 2023-05-04 00:13:25.952350 ontogpt-0.2.4/src/ontogpt/engines/__init__.py
+-rw-r--r--   0        0        0     3748 2023-05-04 00:13:25.952350 ontogpt-0.2.4/src/ontogpt/engines/embedding_similarity_engine.py
+-rw-r--r--   0        0        0    12334 2023-05-04 00:13:25.952350 ontogpt-0.2.4/src/ontogpt/engines/enrichment.py
+-rw-r--r--   0        0        0    19185 2023-05-04 00:13:25.952350 ontogpt-0.2.4/src/ontogpt/engines/halo_engine.py
+-rw-r--r--   0        0        0    24067 2023-05-04 00:13:25.952350 ontogpt-0.2.4/src/ontogpt/engines/knowledge_engine.py
+-rw-r--r--   0        0        0      752 2023-05-04 00:13:25.952350 ontogpt-0.2.4/src/ontogpt/engines/resolver.py
+-rw-r--r--   0        0        0    18520 2023-05-04 00:13:25.952350 ontogpt-0.2.4/src/ontogpt/engines/spires_engine.py
+-rw-r--r--   0        0        0      719 2023-05-04 00:13:25.952350 ontogpt-0.2.4/src/ontogpt/engines/synonym_engine.py
+-rw-r--r--   0        0        0       70 2023-05-04 00:13:25.952350 ontogpt-0.2.4/src/ontogpt/evaluation/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-04 00:13:25.952350 ontogpt-0.2.4/src/ontogpt/evaluation/ctd/__init__.py
+-rw-r--r--   0        0        0   425228 2023-05-04 00:13:25.952350 ontogpt-0.2.4/src/ontogpt/evaluation/ctd/database/CDR_TestSet.BioC.xml.gz
+-rw-r--r--   0        0        0   409439 2023-05-04 00:13:25.956350 ontogpt-0.2.4/src/ontogpt/evaluation/ctd/database/CDR_TrainSet.BioC.xml.gz
+-rw-r--r--   0        0        0   413985 2023-05-04 00:13:25.956350 ontogpt-0.2.4/src/ontogpt/evaluation/ctd/database/synonyms.yaml
+-rw-r--r--   0        0        0    10390 2023-05-04 00:13:25.956350 ontogpt-0.2.4/src/ontogpt/evaluation/ctd/eval_ctd.py
+-rw-r--r--   0        0        0        0 2023-05-04 00:13:25.956350 ontogpt-0.2.4/src/ontogpt/evaluation/drugmechdb/__init__.py
+-rw-r--r--   0        0        0     2145 2023-05-04 00:13:25.956350 ontogpt-0.2.4/src/ontogpt/evaluation/drugmechdb/datamodel/drugmechdb.py
+-rw-r--r--   0        0        0     2027 2023-05-04 00:13:25.956350 ontogpt-0.2.4/src/ontogpt/evaluation/drugmechdb/datamodel/drugmechdb.yaml
+-rw-r--r--   0        0        0    10670 2023-05-04 00:13:25.956350 ontogpt-0.2.4/src/ontogpt/evaluation/drugmechdb/eval_drugmechdb.py
+-rw-r--r--   0        0        0        0 2023-05-04 00:13:25.956350 ontogpt-0.2.4/src/ontogpt/evaluation/enrichment/__init__.py
+-rw-r--r--   0        0        0    13679 2023-05-04 00:13:25.956350 ontogpt-0.2.4/src/ontogpt/evaluation/enrichment/eval_enrichment.py
+-rw-r--r--   0        0        0     2950 2023-05-04 00:13:25.956350 ontogpt-0.2.4/src/ontogpt/evaluation/evaluation_engine.py
+-rw-r--r--   0        0        0     6164 2023-05-04 00:13:25.956350 ontogpt-0.2.4/src/ontogpt/evaluation/go/eval_go.py
+-rw-r--r--   0        0        0        0 2023-05-04 00:13:25.956350 ontogpt-0.2.4/src/ontogpt/evaluation/hpoa/__init__.py
+-rw-r--r--   0        0        0     8973 2023-05-04 00:13:25.956350 ontogpt-0.2.4/src/ontogpt/evaluation/hpoa/eval_hpoa.py
+-rw-r--r--   0        0        0     1191 2023-05-04 00:13:25.956350 ontogpt-0.2.4/src/ontogpt/evaluation/ibd/PMC6386158_fig2_legend.txt
+-rw-r--r--   0        0        0        0 2023-05-04 00:13:25.956350 ontogpt-0.2.4/src/ontogpt/evaluation/ibd/PMC6386158_fig2_legend.txt~
+-rw-r--r--   0        0        0     4791 2023-05-04 00:13:25.956350 ontogpt-0.2.4/src/ontogpt/evaluation/ibd/PMC6386158_fig2_legend.yaml
+-rwxr-xr-x   0        0        0       95 2023-05-04 00:13:25.956350 ontogpt-0.2.4/src/ontogpt/evaluation/ibd/run.sh
+-rwxr-xr-x   0        0        0       99 2023-05-04 00:13:25.956350 ontogpt-0.2.4/src/ontogpt/evaluation/ibd/run.sh~
+-rw-r--r--   0        0        0      586 2023-05-04 00:13:25.956350 ontogpt-0.2.4/src/ontogpt/evaluation/resolver.py
+-rw-r--r--   0        0        0        0 2023-05-04 00:13:25.956350 ontogpt-0.2.4/src/ontogpt/io/__init__.py
+-rw-r--r--   0        0        0      386 2023-05-04 00:13:25.956350 ontogpt-0.2.4/src/ontogpt/io/exporter.py
+-rw-r--r--   0        0        0     4329 2023-05-04 00:13:25.956350 ontogpt-0.2.4/src/ontogpt/io/html_exporter.py
+-rw-r--r--   0        0        0     3255 2023-05-04 00:13:25.956350 ontogpt-0.2.4/src/ontogpt/io/markdown_exporter.py
+-rw-r--r--   0        0        0     2350 2023-05-04 00:13:25.956350 ontogpt-0.2.4/src/ontogpt/io/owl_exporter.py
+-rw-r--r--   0        0        0     1440 2023-05-04 00:13:25.956350 ontogpt-0.2.4/src/ontogpt/io/rdf_exporter.py
+-rw-r--r--   0        0        0      899 2023-05-04 00:13:25.956350 ontogpt-0.2.4/src/ontogpt/io/yaml_wrapper.py
+-rw-r--r--   0        0        0        0 2023-05-04 00:13:25.956350 ontogpt-0.2.4/src/ontogpt/prompts/__init__.py
+-rw-r--r--   0        0        0      159 2023-05-04 00:13:25.956350 ontogpt-0.2.4/src/ontogpt/prompts/enrichment/__init__.py
+-rw-r--r--   0        0        0     1257 2023-05-04 00:13:25.956350 ontogpt-0.2.4/src/ontogpt/prompts/enrichment/gene_set_summarization.jinja2
+-rw-r--r--   0        0        0     1016 2023-05-04 00:13:25.956350 ontogpt-0.2.4/src/ontogpt/prompts/enrichment/gene_set_summarization_with_p_values.jinja2
+-rw-r--r--   0        0        0      993 2023-05-04 00:13:25.956350 ontogpt-0.2.4/src/ontogpt/prompts/enrichment/gene_set_summarization_with_p_values_0.jinja2
+-rw-r--r--   0        0        0      994 2023-05-04 00:13:25.956350 ontogpt-0.2.4/src/ontogpt/prompts/enrichment/gene_set_summarization_with_p_values_1.jinja2
+-rw-r--r--   0        0        0      995 2023-05-04 00:13:25.956350 ontogpt-0.2.4/src/ontogpt/prompts/enrichment/gene_set_summarization_with_p_values_2.jinja2
+-rw-r--r--   0        0        0      560 2023-05-04 00:13:25.956350 ontogpt-0.2.4/src/ontogpt/prompts/similarity/connections.jinja2
+-rw-r--r--   0        0        0       68 2023-05-04 00:13:25.956350 ontogpt-0.2.4/src/ontogpt/templates/__init__.py
+-rw-r--r--   0        0        0      401 2023-05-04 00:13:25.956350 ontogpt-0.2.4/src/ontogpt/templates/all.yaml
+-rw-r--r--   0        0        0     5942 2023-05-04 00:13:25.956350 ontogpt-0.2.4/src/ontogpt/templates/biological_process.py
+-rw-r--r--   0        0        0     2027 2023-05-04 00:13:25.956350 ontogpt-0.2.4/src/ontogpt/templates/biological_process.yaml
+-rw-r--r--   0        0        0     2938 2023-05-04 00:13:25.956350 ontogpt-0.2.4/src/ontogpt/templates/class_enrichment.py
+-rw-r--r--   0        0        0     3192 2023-05-04 00:13:25.956350 ontogpt-0.2.4/src/ontogpt/templates/class_enrichment.yaml
+-rw-r--r--   0        0        0     3593 2023-05-04 00:13:25.956350 ontogpt-0.2.4/src/ontogpt/templates/core.py
+-rw-r--r--   0        0        0     3098 2023-05-04 00:13:25.956350 ontogpt-0.2.4/src/ontogpt/templates/core.yaml
+-rw-r--r--   0        0        0     6210 2023-05-04 00:13:25.956350 ontogpt-0.2.4/src/ontogpt/templates/ctd.py
+-rw-r--r--   0        0        0     6683 2023-05-04 00:13:25.956350 ontogpt-0.2.4/src/ontogpt/templates/ctd.yaml
+-rw-r--r--   0        0        0     5466 2023-05-04 00:13:25.956350 ontogpt-0.2.4/src/ontogpt/templates/drug.py
+-rw-r--r--   0        0        0     1856 2023-05-04 00:13:25.956350 ontogpt-0.2.4/src/ontogpt/templates/drug.yaml
+-rw-r--r--   0        0        0     6092 2023-05-04 00:13:25.956350 ontogpt-0.2.4/src/ontogpt/templates/environmental_sample.py
+-rw-r--r--   0        0        0     2880 2023-05-04 00:13:25.956350 ontogpt-0.2.4/src/ontogpt/templates/environmental_sample.yaml
+-rw-r--r--   0        0        0     4709 2023-05-04 00:13:25.956350 ontogpt-0.2.4/src/ontogpt/templates/gene_description_term.py
+-rw-r--r--   0        0        0     1614 2023-05-04 00:13:25.956350 ontogpt-0.2.4/src/ontogpt/templates/gene_description_term.yaml
+-rw-r--r--   0        0        0     8172 2023-05-04 00:13:25.960350 ontogpt-0.2.4/src/ontogpt/templates/gocam.py
+-rw-r--r--   0        0        0     4871 2023-05-04 00:13:25.960350 ontogpt-0.2.4/src/ontogpt/templates/gocam.yaml
+-rw-r--r--   0        0        0     6813 2023-05-04 00:13:25.960350 ontogpt-0.2.4/src/ontogpt/templates/halo.py
+-rw-r--r--   0        0        0     2367 2023-05-04 00:13:25.960350 ontogpt-0.2.4/src/ontogpt/templates/halo.yaml
+-rw-r--r--   0        0        0     8165 2023-05-04 00:13:25.960350 ontogpt-0.2.4/src/ontogpt/templates/ibd.py
+-rw-r--r--   0        0        0     4869 2023-05-04 00:13:25.960350 ontogpt-0.2.4/src/ontogpt/templates/ibd.yaml
+-rw-r--r--   0        0        0     6097 2023-05-04 00:13:25.960350 ontogpt-0.2.4/src/ontogpt/templates/mendelian_disease.py
+-rw-r--r--   0        0        0     3130 2023-05-04 00:13:25.960350 ontogpt-0.2.4/src/ontogpt/templates/mendelian_disease.yaml
+-rw-r--r--   0        0        0     5384 2023-05-04 00:13:25.960350 ontogpt-0.2.4/src/ontogpt/templates/metabolic_process.py
+-rw-r--r--   0        0        0     1633 2023-05-04 00:13:25.960350 ontogpt-0.2.4/src/ontogpt/templates/metabolic_process.yaml
+-rw-r--r--   0        0        0     7156 2023-05-04 00:13:25.960350 ontogpt-0.2.4/src/ontogpt/templates/metagenome_study.py
+-rw-r--r--   0        0        0     3910 2023-05-04 00:13:25.960350 ontogpt-0.2.4/src/ontogpt/templates/metagenome_study.yaml
+-rw-r--r--   0        0        0     5072 2023-05-04 00:13:25.960350 ontogpt-0.2.4/src/ontogpt/templates/ontology_class.py
+-rw-r--r--   0        0        0     2686 2023-05-04 00:13:25.960350 ontogpt-0.2.4/src/ontogpt/templates/ontology_class.yaml
+-rw-r--r--   0        0        0     6136 2023-05-04 00:13:25.960350 ontogpt-0.2.4/src/ontogpt/templates/ontology_issue.py
+-rw-r--r--   0        0        0     3383 2023-05-04 00:13:25.960350 ontogpt-0.2.4/src/ontogpt/templates/ontology_issue.yaml
+-rw-r--r--   0        0        0     4887 2023-05-04 00:13:25.960350 ontogpt-0.2.4/src/ontogpt/templates/phenotype.py
+-rw-r--r--   0        0        0     1532 2023-05-04 00:13:25.960350 ontogpt-0.2.4/src/ontogpt/templates/phenotype.yaml
+-rw-r--r--   0        0        0     7501 2023-05-04 00:13:25.960350 ontogpt-0.2.4/src/ontogpt/templates/reaction.py
+-rw-r--r--   0        0        0     3187 2023-05-04 00:13:25.960350 ontogpt-0.2.4/src/ontogpt/templates/reaction.yaml
+-rw-r--r--   0        0        0     7222 2023-05-04 00:13:25.960350 ontogpt-0.2.4/src/ontogpt/templates/recipe.py
+-rw-r--r--   0        0        0     5792 2023-05-04 00:13:25.960350 ontogpt-0.2.4/src/ontogpt/templates/recipe.yaml
+-rw-r--r--   0        0        0     7847 2023-05-04 00:13:25.960350 ontogpt-0.2.4/src/ontogpt/templates/treatment.py
+-rw-r--r--   0        0        0     4485 2023-05-04 00:13:25.960350 ontogpt-0.2.4/src/ontogpt/templates/treatment.yaml
+-rw-r--r--   0        0        0        0 2023-05-04 00:13:25.960350 ontogpt-0.2.4/src/ontogpt/utils/__init__.py
+-rw-r--r--   0        0        0     7510 2023-05-04 00:13:25.960350 ontogpt-0.2.4/src/ontogpt/utils/gene_set_utils.py
+-rw-r--r--   0        0        0        0 2023-05-04 00:13:25.960350 ontogpt-0.2.4/src/ontogpt/webapp/__init__.py
+-rw-r--r--   0        0        0      861 2023-05-04 00:13:25.960350 ontogpt-0.2.4/src/ontogpt/webapp/html/form.html
+-rw-r--r--   0        0        0      201 2023-05-04 00:13:25.960350 ontogpt-0.2.4/src/ontogpt/webapp/html/results.html
+-rw-r--r--   0        0        0      819 2023-05-04 00:13:25.960350 ontogpt-0.2.4/src/ontogpt/webapp/html/spindoctor/form.html
+-rw-r--r--   0        0        0      205 2023-05-04 00:13:25.960350 ontogpt-0.2.4/src/ontogpt/webapp/html/spindoctor/results.html
+-rw-r--r--   0        0        0     2722 2023-05-04 00:13:25.960350 ontogpt-0.2.4/src/ontogpt/webapp/main.py
+-rw-r--r--   0        0        0    13469 1970-01-01 00:00:00.000000 ontogpt-0.2.4/PKG-INFO
```

### Comparing `ontogpt-0.2.3/LICENSE` & `ontogpt-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.3/README.md` & `ontogpt-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.3/pyproject.toml` & `ontogpt-0.2.4/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "ontogpt"
-version = "0.2.3"
+version = "0.2.4"
 description = "OntoGPT"
 authors = ["Chris Mungall <cjmungall@lbl.gov>"]
 license = "BSD-3"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 click = "^8.1.3"
 importlib = "^1.0.4"
 openai = "^0.27.4"
-oaklib = "^0.5.2"
+oaklib = "^0.5.4"
 gilda = "^0.10.3"
 jsonlines = "^3.1.0"
 python-multipart = "^0.0.5"
 linkml-owl = "^0.2.7"
 beautifulsoup4 = "^4.11.1"
 eutils = "^0.6.0"
 class-resolver = "*"
@@ -40,14 +40,15 @@
 sphinx-autodoc-typehints = {version = "^1.19.4", extras = ["docs"], optional = true}
 sphinx-click = {version = "^4.3.0", extras = ["docs"], optional = true}
 myst-parser = {version = "^0.18.1", extras = ["docs"], optional = true}
 recipe-scrapers = {version = "^14.35.0", extras = ["recipes"], optional = true}
 cachier = "^2.1.0"
 wikipedia-api = "^0.5.8"
 rustsim = "^0.1.8"
+requests-cache = "^1.0.1"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.2"
 setuptools = ">=65.5.0"
 tox = "^3.25.1"
 mkdocs-mermaid2-plugin = "^0.6.0"
```

### Comparing `ontogpt-0.2.3/src/ontogpt/cli.py` & `ontogpt-0.2.4/src/ontogpt/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,20 @@
 from ontogpt.engines.knowledge_engine import KnowledgeEngine
 from ontogpt.engines.spires_engine import SPIRESEngine
 from ontogpt.engines.synonym_engine import SynonymEngine
 from ontogpt.evaluation.enrichment.eval_enrichment import EvalEnrichment
 from ontogpt.evaluation.resolver import create_evaluator
 from ontogpt.io.html_exporter import HTMLExporter
 from ontogpt.io.markdown_exporter import MarkdownExporter
-from ontogpt.utils.gene_set_utils import GeneSet, parse_gene_set
+from ontogpt.utils.gene_set_utils import (
+    GeneSet,
+    _is_human,
+    fill_missing_gene_set_values,
+    parse_gene_set,
+)
 
 __all__ = [
     "main",
 ]
 
 from ontogpt.io.owl_exporter import OWLExporter
 from ontogpt.io.rdf_exporter import RDFExporter
@@ -459,14 +464,15 @@
 
 
 @main.command()
 @output_option_txt
 @output_format_options
 @click.option(
     "--annotation-path",
+    "-A",
     required=True,
 )
 @click.argument("term")
 def create_gene_set(term, output, output_format, annotation_path, **kwargs):
     """Create a gene set."""
     logging.info(f"Creating for {term}")
     evaluator = EvalEnrichment()
@@ -474,22 +480,25 @@
     gene_set = evaluator.create_gene_set_from_term(term)
     print(yaml.dump(gene_set.dict(), sort_keys=False))
 
 
 @main.command()
 @output_option_txt
 @output_format_options
+@click.option("--fill/--no-fill", default=False)
 @click.option(
     "--input-file",
     "-U",
     help="File with gene IDs to enrich (if not passed as arguments)",
 )
-def convert_geneset(input_file, output, output_format, **kwargs):
+def convert_geneset(input_file, output, output_format, fill, **kwargs):
     """Convert gene set to YAML."""
     gene_set = parse_gene_set(input_file)
+    if fill:
+        fill_missing_gene_set_values(gene_set)
     output.write(dump_minimal_yaml(gene_set.dict()))
 
 
 @main.command()
 @output_option_txt
 @output_format_options
 @model_option
@@ -531,14 +540,18 @@
 @click.option(
     "--combined-synopsis/--no-combined-synopsis",
     default=False,
     show_default=True,
     help="If set, both gene descriptions",
 )
 @click.option(
+    "--end-marker",
+    help="For testing minor variants of prompts",
+)
+@click.option(
     "--annotations/--no-annotations",
     default=True,
     show_default=True,
     help="If set, include annotations in the prompt",
 )
 @prompt_template_option
 @interactive_option
@@ -548,14 +561,15 @@
     context,
     input_file,
     resolver,
     output,
     model,
     show_prompt,
     interactive,
+    end_marker,
     output_format,
     randomize_gene_descriptions_using_file,
     **kwargs,
 ):
     """Gene class enrichment.
 
     Algorithm:
@@ -584,14 +598,16 @@
     if input_file:
         if genes:
             raise ValueError("Either genes or input file must be passed")
         gene_set = parse_gene_set(input_file)
     if not gene_set:
         raise ValueError("No genes passed")
     ke = create_engine(None, EnrichmentEngine, model=model)
+    if end_marker:
+        ke.end_marker = end_marker
     if interactive:
         ke.client.interactive = True
     if settings.cache_db:
         ke.client.cache_db_path = settings.cache_db
     if not isinstance(ke, EnrichmentEngine):
         raise ValueError(f"Expected EnrichmentEngine, got {type(ke)}")
     if resolver:
@@ -813,15 +829,14 @@
 # @click.option(
 #    "--randomize-gene-descriptions/--no-randomize-gene-descriptions",
 #    help="DO NOT USE EXCEPT FOR EVALUATION PUPOSES."
 # )
 @click.option(
     "--annotations-path",
     "-A",
-    default="tests/input/genes2go.tsv.gz",
     help="Path to annotations",
 )
 @click.argument("genes", nargs=-1)
 def eval_enrichment(genes, input_file, number_to_drop, annotations_path, output, **kwargs):
     """Run enrichment using multiple methods."""
     if not genes and not input_file:
         raise ValueError("Either genes or input file must be passed")
@@ -829,14 +844,19 @@
         gene_set = GeneSet(name="TEMP", gene_symbols=genes)
     if input_file:
         if genes:
             raise ValueError("Either genes or input file must be passed")
         gene_set = parse_gene_set(input_file)
     if not gene_set:
         raise ValueError("No genes passed")
+    fill_missing_gene_set_values(gene_set)
+    if not annotations_path:
+        if not _is_human(gene_set):
+            raise ValueError("No annotations path passed")
+        annotations_path = "tests/input/genes2go.tsv.gz"
     eval_engine = EvalEnrichment()
     eval_engine.load_annotations(annotations_path)
     comps = eval_engine.evaluate_methods_on_gene_set(gene_set, n=number_to_drop, **kwargs)
     output.write(dump_minimal_yaml(comps))
 
 
 @main.command()
```

### Comparing `ontogpt-0.2.3/src/ontogpt/clients/openai_client.py` & `ontogpt-0.2.4/src/ontogpt/clients/openai_client.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.3/src/ontogpt/clients/pubmed_client.py` & `ontogpt-0.2.4/src/ontogpt/clients/pubmed_client.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.3/src/ontogpt/clients/soup_client.py` & `ontogpt-0.2.4/src/ontogpt/clients/soup_client.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.3/src/ontogpt/clients/wikipedia_client.py` & `ontogpt-0.2.4/src/ontogpt/clients/wikipedia_client.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.3/src/ontogpt/conf/synonymizer-conf.yaml` & `ontogpt-0.2.4/src/ontogpt/conf/synonymizer-conf.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.3/src/ontogpt/converters/ontology_converter.py` & `ontogpt-0.2.4/src/ontogpt/converters/ontology_converter.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.3/src/ontogpt/engines/embedding_similarity_engine.py` & `ontogpt-0.2.4/src/ontogpt/engines/embedding_similarity_engine.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.3/src/ontogpt/engines/enrichment.py` & `ontogpt-0.2.4/src/ontogpt/engines/enrichment.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,24 +5,25 @@
 from dataclasses import dataclass, field
 from enum import Enum
 from pathlib import Path
 from typing import Dict, List, Optional, Tuple, Union
 
 from jinja2 import Template
 from oaklib import BasicOntologyInterface, get_adapter
+from pydantic import BaseModel
 
 from ontogpt.engines.knowledge_engine import KnowledgeEngine
 from ontogpt.prompts.enrichment import DEFAULT_ENRICHMENT_PROMPT
+from ontogpt.templates.class_enrichment import ClassEnrichmentResult
 from ontogpt.templates.gene_description_term import GeneDescriptionTerm
 from ontogpt.utils.gene_set_utils import (
     ENTITY_ID,
     GENE_TUPLE,
-    EnrichmentPayload,
     GeneSet,
-    gene_info,
+    fill_missing_gene_set_values,
 )
 
 logger = logging.getLogger(__name__)
 
 
 SUMMARY_KEYWORD = "Summary"
 MECHANISM_KEYWORD = "Mechanism"
@@ -34,14 +35,59 @@
     ONTOLOGICAL_SYNOPSIS = "ontological"
     NARRATIVE_SYNOPSIS = "narrative"
     COMBINED_SYNOPSIS = "combined"
     WIKIPEDIA = "wikipedia"
     PUBMED = "pubmed"
 
 
+class EnrichmentPayload(BaseModel):
+    """Payload for enrichment."""
+
+    prompt: str = None
+    """The prompt to use for the summarization task (only filled for LLMs)."""
+
+    response_text: str = None
+    """The response text from the summarization task (only filled for LLMs)."""
+
+    truncation_factor: float = None
+    """Fraction of gene descriptions retained after trimming to fit token limit."""
+
+    summary: str = None
+    """The summary of the gene set generated by the LLM."""
+
+    term_strings: List[str] = []
+    """The raw term labels parsed from the LLM completion payload"""
+
+    term_ids: List[str] = []
+    """The normalized terms"""
+
+    ontological_synopsis: bool = None
+    """True if the gene descriptions used the ontological synopsis"""
+
+    combined_synopsis: bool = None
+    """True if the gene descriptions used both ontological and narrative synopses"""
+
+    annotations: bool = None
+    """True if the gene descriptions used the annotations (vs latent KB)"""
+
+    response_token_length: int = None
+    """The number of tokens in the response text"""
+
+    model: str = None
+    """The model used for the summarization task (only filled for LLMs)."""
+
+    method: str = None
+    """The method used for the summarization task."""
+
+    prompt_variant: str = None
+
+    enrichment_results: List[ClassEnrichmentResult] = None
+    """Enrichment results (only filled for non-LLMs)"""
+
+
 @dataclass
 class EnrichmentEngine(KnowledgeEngine):
     """Engine for performing term enrichment.
 
     Algorithm: SPINDOCTOR
 
     Summarizing Proteins Interpolating Narrative
@@ -55,14 +101,16 @@
     label_resolvers: Dict[str, BasicOntologyInterface] = field(default_factory=dict)
 
     completion_length = 250
 
     prompt_template: str = None
     """Path to a jinja2 template for the prompt"""
 
+    end_marker = "###"
+
     def __post_init__(self):
         if not self.template:
             self.template = "gene_description_term"
         super().__post_init__()
 
     def __key(self):
         return "enrichment_engine"
@@ -114,44 +162,35 @@
             elif gene_description_source == GeneDescriptionSource.NARRATIVE_SYNOPSIS:
                 ontological_synopsis = False
                 annotations = True
             elif gene_description_source == GeneDescriptionSource.COMBINED_SYNOPSIS:
                 combined_synopsis = True
             else:
                 raise NotImplementedError
-        if not gene_set.gene_ids and not gene_set.gene_symbols:
-            raise ValueError(f"Gene set {gene_set.name} has no gene symbols or ids")
-        # if gene_set.gene_ids and not gene_set.gene_symbols:
-        #    adapter = list(self.label_resolvers.values())[0]
-        #    gene_set.gene_symbols = [adapter.label(x.lower()) for x in gene_set.gene_ids]
-        if not gene_set.gene_ids or normalize:
-            gene_set.gene_ids = list(self.map_labels(gene_set.gene_symbols, strict=strict))
-            logger.info(f"gene ids: {gene_set.gene_ids}")
+        fill_missing_gene_set_values(gene_set)
         gene_tuples = []
-        for gene_id in gene_set.gene_ids:
-            logging.info(f"Looking up gene summary for {gene_id}...")
-            symbol, desc_manual, desc_auto = gene_info(gene_id)
+        for gene in gene_set.genes.values():
+            logging.info(f"Looking up gene summary for {gene.id}...")
             if combined_synopsis:
                 if ontological_synopsis:
-                    desc = desc_auto + "; " + desc_manual
+                    desc = gene.ontological_synopsis + "; " + gene.narrative_synopsis
                     logging.debug(f"Combined synopsis (priority: auto): {desc}")
                 else:
-                    desc = desc_manual + "; " + desc_auto
+                    desc = gene.narrative_synopsis + "; " + gene.ontological_synopsis
                     logging.debug(f"Combined synopsis (priority: manual): {desc}")
             elif ontological_synopsis:
-                desc = desc_auto
+                desc = gene.ontological_synopsis
                 logging.debug(f"Auto synopsis: {desc}")
             else:
-                desc = desc_manual
+                desc = gene.narrative_synopsis
                 logging.debug(f"Manual synopsis: {desc}")
-            gene_tuples.append((gene_id, symbol, desc))
+            gene_tuples.append((gene.id, gene.symbol, desc))
         logging.info(f"Found {len(gene_tuples)} gene summaries")
-        # if not annotations:
-        #    return self.summarize_annotation_free(gene_tuples)
         if gene_aliases:
+            # for randomization
             gene_tuples = [(id, gene_aliases.get(sym, sym), desc) for id, sym, desc in gene_tuples]
         if not prompt_template:
             prompt_template = str(f"{DEFAULT_ENRICHMENT_PROMPT}.jinja2")
         prompt, tf = self._prompt_from_template(
             gene_tuples,
             template=prompt_template,
             annotations=annotations,
@@ -199,14 +238,15 @@
         prompt = template.render(
             gene_descriptions=gd_tuples,
             annotations=annotations,
             taxon=taxon,
             SUMMARY_KEYWORD=SUMMARY_KEYWORD,
             MECHANISM_KEYWORD=MECHANISM_KEYWORD,
             ENRICHED_TERMS_KEYWORD=ENRICHED_TERMS_KEYWORD,
+            END_MARKER=self.end_marker,
         )
         logging.debug(f"Prompt from template: {prompt}")
         logging.info(f"Prompt [{truncation_factor}] Length: {len(prompt)}")
         # https://help.openai.com/en/articles/4936856-what-are-tokens-and-how-to-count-them
         prompt_length = len(self.encoding.encode(prompt)) + 10
         max_len = 4097 - self.completion_length
         logging.info(
```

### Comparing `ontogpt-0.2.3/src/ontogpt/engines/halo_engine.py` & `ontogpt-0.2.4/src/ontogpt/engines/halo_engine.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.3/src/ontogpt/engines/knowledge_engine.py` & `ontogpt-0.2.4/src/ontogpt/engines/knowledge_engine.py`

 * *Files 6% similar despite different names*

```diff
@@ -466,35 +466,53 @@
             if matching_prefixes:
                 yield matching_prefixes[0] + ":" + id_matches.group(2)
         text_lower = text.lower()
         text_singularized = inflection.singularize(text_lower)
         if text_singularized != text_lower:
             logger.info(f"Singularized {text} to {text_singularized}")
             yield from self.groundings(text_singularized, cls)
+        paren_char = "["
         parenthetical_components = re.findall(r"\[(.*?)\]", text_lower)
         if not parenthetical_components:
+            paren_char = "("
             parenthetical_components = re.findall(r"\((.*?)\)", text_lower)
         if parenthetical_components:
+            logger.info(f"{text_lower} =>paren=> {parenthetical_components}")
             trimmed_text = text_lower
             for component in parenthetical_components:
                 if component:
+                    logger.debug(
+                        f"RECURSIVE GROUNDING OF {component} from {parenthetical_components}"
+                    )
                     yield from self.groundings(component, cls)
-                trimmed_text = trimmed_text.replace(f"({component})", "")
+                if paren_char == "(":
+                    trimmed_text = trimmed_text.replace(f"({component})", "")
+                elif paren_char == "[":
+                    trimmed_text = trimmed_text.replace(f"[{component}]", "")
+                else:
+                    raise AssertionError(f"Unknown paren char {paren_char}")
             trimmed_text = trimmed_text.strip().replace("  ", " ")
             if trimmed_text:
+                if len(trimmed_text) >= len(text_lower):
+                    raise AssertionError(
+                        f"Trimmed text {trimmed_text} is not shorter than {text_lower}"
+                    )
+                logger.debug(
+                    f"{text_lower} =>trimmed=> {trimmed_text}; in {parenthetical_components}"
+                )
                 yield from self.groundings(trimmed_text, cls)
         if self.dictionary and text_lower in self.dictionary:
             obj_id = self.dictionary[text_lower]
-            logger.info(f"Found {text} in dictionary: {obj_id}")
+            logger.debug(f"Found {text} in dictionary: {obj_id}")
             yield obj_id
         if self.dictionary:
             for syn, obj_id in self.dictionary.items():
                 if syn in text_lower:
                     if len(syn) / len(text_lower) > self.min_grounding_text_overlap:
-                        logger.info(f"Found {syn} < {text} in dictionary: {obj_id}")
+                        logger.debug(f"Found {syn} < {text} in dictionary: {obj_id}")
                         yield obj_id
         if self.annotators and cls.name in self.annotators:
             annotators = self.annotators[cls.name]
         else:
             if ANNOTATION_KEY_ANNOTATORS not in cls.annotations:
                 annotators = []
             else:
```

### Comparing `ontogpt-0.2.3/src/ontogpt/engines/resolver.py` & `ontogpt-0.2.4/src/ontogpt/engines/resolver.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.3/src/ontogpt/engines/spires_engine.py` & `ontogpt-0.2.4/src/ontogpt/engines/spires_engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -269,14 +269,18 @@
             elif slot.description:
                 slot_prompt = slot.description
             else:
                 if slot.multivalued:
                     slot_prompt = f"semicolon-separated list of {slot.name}s"
                 else:
                     slot_prompt = f"the value for {slot.name}"
+            if slot.range in self.schemaview.all_enums():
+                enum_def = self.schemaview.get_enum(slot.range)
+                pvs = [str(k) for k in enum_def.permissible_values.keys()]
+                slot_prompt += f"Must be one of: {', '.join(pvs)}"
             prompt += f"{slot.name}: <{slot_prompt}>\n"
         # prompt += "Do not answer if you don't know\n\n"
         prompt = f"{prompt}\n\nText:\n{text}\n\n===\n\n"
         if object:
             if cls is None:
                 cls = self.template_class
             if isinstance(object, pydantic.BaseModel):
@@ -441,14 +445,18 @@
             if isinstance(vals, list):
                 multivalued = True
             else:
                 multivalued = False
                 vals = [vals]
             slot = sv.induced_slot(field, cls.name)
             rng_cls = sv.get_class(slot.range)
+            enum_def = None
+            if slot.range:
+                if slot.range in self.schemaview.all_enums():
+                    enum_def = self.schemaview.get_enum(slot.range)
             new_ann[field] = []
             for val in vals:
                 if not val:
                     continue
                 if isinstance(val, tuple):
                     # special case for pairs
                     sub_slots = sv.class_induced_slots(rng_cls.name)
@@ -461,14 +469,25 @@
                         result = self.normalize_named_entity(val[i], sub_slot.range)
                         obj[sub_slot.name] = result
                 elif isinstance(val, dict):
                     # recurse
                     obj = self.ground_annotation_object(val, rng_cls)
                 else:
                     obj = self.normalize_named_entity(val, slot.range)
+                if enum_def:
+                    found = False
+                    logging.info(f"Looking for {obj} in {enum_def.name}")
+                    for k, _pv in enum_def.permissible_values.items():
+                        if obj.lower() == k.lower():
+                            obj = k
+                            found = True
+                            break
+                    if not found:
+                        logging.info(f"Cannot find enum value for {obj} in {enum_def.name}")
+                        obj = None
                 if multivalued:
                     new_ann[field].append(obj)
                 else:
                     new_ann[field] = obj
         logging.debug(f"Creating object from dict {new_ann}")
         logging.info(new_ann)
         py_cls = self.template_module.__dict__[cls.name]
```

### Comparing `ontogpt-0.2.3/src/ontogpt/engines/synonym_engine.py` & `ontogpt-0.2.4/src/ontogpt/engines/synonym_engine.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.3/src/ontogpt/evaluation/ctd/database/CDR_TestSet.BioC.xml.gz` & `ontogpt-0.2.4/src/ontogpt/evaluation/ctd/database/CDR_TestSet.BioC.xml.gz`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.3/src/ontogpt/evaluation/ctd/database/CDR_TrainSet.BioC.xml.gz` & `ontogpt-0.2.4/src/ontogpt/evaluation/ctd/database/CDR_TrainSet.BioC.xml.gz`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.3/src/ontogpt/evaluation/ctd/database/synonyms.yaml` & `ontogpt-0.2.4/src/ontogpt/evaluation/ctd/database/synonyms.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.3/src/ontogpt/evaluation/ctd/eval_ctd.py` & `ontogpt-0.2.4/src/ontogpt/evaluation/ctd/eval_ctd.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.3/src/ontogpt/evaluation/drugmechdb/datamodel/drugmechdb.py` & `ontogpt-0.2.4/src/ontogpt/evaluation/drugmechdb/datamodel/drugmechdb.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.3/src/ontogpt/evaluation/drugmechdb/datamodel/drugmechdb.yaml` & `ontogpt-0.2.4/src/ontogpt/evaluation/drugmechdb/datamodel/drugmechdb.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.3/src/ontogpt/evaluation/drugmechdb/eval_drugmechdb.py` & `ontogpt-0.2.4/src/ontogpt/evaluation/drugmechdb/eval_drugmechdb.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.3/src/ontogpt/evaluation/enrichment/eval_enrichment.py` & `ontogpt-0.2.4/src/ontogpt/evaluation/enrichment/eval_enrichment.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """Eval enrichment template."""
 import datetime
 import gzip
 import logging
 import random
 from collections import defaultdict
-from copy import copy
 from dataclasses import dataclass, field
 from pathlib import Path
 from typing import Dict, Iterator, List, Optional, Tuple
 
 import tiktoken
 import yaml
 from cachier import cachier
@@ -16,29 +15,24 @@
 from oaklib import get_adapter, get_implementation_from_shorthand
 from oaklib.datamodels.association import Association
 from oaklib.datamodels.vocabulary import EQUIVALENT_CLASS, IS_A, PART_OF
 from oaklib.interfaces.class_enrichment_calculation_interface import (
     ClassEnrichmentCalculationInterface,
 )
 from oaklib.interfaces.obograph_interface import OboGraphInterface
+from oaklib.parsers.association_parser_factory import get_association_parser
 from pydantic import BaseModel
 from tiktoken import Encoding
 
 from ontogpt.engines import create_engine
-from ontogpt.engines.enrichment import ENTITY_ID, EnrichmentEngine
+from ontogpt.engines.enrichment import ENTITY_ID, EnrichmentEngine, EnrichmentPayload
 from ontogpt.engines.knowledge_engine import MODEL_GPT_3_5_TURBO, MODEL_NAME, MODEL_TEXT_DAVINCI_003
 from ontogpt.evaluation.evaluation_engine import EvaluationEngine
 from ontogpt.templates.class_enrichment import ClassEnrichmentResult
-from ontogpt.utils.gene_set_utils import (
-    SYMBOL,
-    EnrichmentPayload,
-    GeneSet,
-    gene_info,
-    populate_ids_and_symbols,
-)
+from ontogpt.utils.gene_set_utils import SYMBOL, GeneSet, drop_genes_from_gene_set, gene_info
 
 THIS_DIR = Path(__file__).parent
 DATABASE_DIR = Path(__file__).parent / "database"
 
 ONTOLOGICAL_SYNOPSIS = "ontological_synopsis"
 NARRATIVE_SYNOPSIS = "narrative_synopsis"
 NO_SYNOPSIS = "no_synopsis"
@@ -64,14 +58,15 @@
     right_jaccard: float = None
     summary_jaccard: float = None
 
 
 class GeneSetComparison(BaseModel):
     name: str
     gene_symbols: List[str]
+    gene_ids: List[str] = None
     model: str = None
     payloads: Dict[str, EnrichmentPayload] = None
     overlaps: Dict[Tuple[str, str], Overlap] = None
     number_of_genes_swapped_out: int = None
 
 
 @cachier(stale_after=datetime.timedelta(days=3))
@@ -118,88 +113,78 @@
         :param randomize_gene_descriptions: use random gene descriptions
         """
         if n < 1:
             raise ValueError(f"n must be greater than 0: {n}")
         if n > 5:
             raise ValueError(f"n must be less than 5: {n}")
         name = gene_set.name
-        hgnc = get_adapter("sqlite:obo:hgnc")
-        populate_ids_and_symbols(gene_set, hgnc)
-        gene_symbols = gene_set.gene_symbols
         comparisons = []
-        if len(gene_symbols) <= 1:
-            raise ValueError(f"Gene set must have at least two genes: {gene_set}")
         for i in range(0, n):
-            logger.info(f"{gene_set.name} [{i}]")
-            expt_name = f"{name}-{i}"
-            expt_gene_symbols = copy(gene_symbols)
-            random.shuffle(expt_gene_symbols)
-            num_to_drop = int(len(expt_gene_symbols) * (i / 10))
-            logger.info(f"Dropping {num_to_drop} genes (iteration: {i})")
-            expt_gene_symbols = expt_gene_symbols[num_to_drop:max_size]
-            for _ in range(0, num_to_drop):
-                random_gene = self.random_gene_symbol()
-                logger.info(f"Adding random gene: {random_gene}")
-                expt_gene_symbols.append(random_gene)
-            logger.info(f"New symbols: {expt_gene_symbols}")
+            perturbed_gene_set = drop_genes_from_gene_set(gene_set, i * 10)
+            perturbed_gene_set.name = f"{name}-{i}"
             comp = self.compare_analysis(
-                expt_gene_symbols, expt_name, number_of_genes_swapped_out=num_to_drop
+                perturbed_gene_set,
             )
             logger.debug(comp)
             logger.info(yaml.dump(comp.dict(), sort_keys=False))
             comparisons.append(comp)
         return comparisons
 
-    def compare_analysis(
-        self, gene_symbols: List[str], name: str = None, **kwargs
-    ) -> GeneSetComparison:
+    def compare_analysis(self, gene_set: GeneSet, **kwargs) -> GeneSetComparison:
         """Compare OntoGPT enrichment vs standard."""
         payloads = {}
-        gene_set = GeneSet(name=name, gene_symbols=gene_symbols)
-        logger.info(f"Gene symbols: {gene_symbols}")
+        logger.info(f"Gene symbols: {gene_set.gene_symbols}")
         for model in ENRICHMENT_MODELS:
             engine = self.engines[model]
             for method in [NO_SYNOPSIS, ONTOLOGICAL_SYNOPSIS, NARRATIVE_SYNOPSIS]:
                 if method == ONTOLOGICAL_SYNOPSIS:
                     args = dict(ontological_synopsis=True)
                 elif method == NARRATIVE_SYNOPSIS:
                     args = dict(ontological_synopsis=False)
                 elif method == NO_SYNOPSIS:
                     args = dict(annotations=False)
                 else:
                     raise AssertionError(f"Unknown method: {method}")
-                payload = engine.summarize(gene_set, normalize=True, **args)
-                payload.method = method
-                model_method = f"{model}.{method}"
-                payloads[model_method] = payload
+                for prompt_variant, end_marker in [("v1", "==="), ("v2", "###")]:
+                    engine.end_marker = end_marker
+                    payload = engine.summarize(gene_set, normalize=True, **args)
+                    payload.method = method
+                    payload.prompt_variant = prompt_variant
+                    model_method = f"{model}.{method}.{prompt_variant}"
+                    payloads[model_method] = payload
         payloads[STANDARD] = self.standard_enrichment(gene_set)
         payloads[STANDARD_NO_ONTOLOGY] = self.standard_enrichment(gene_set, use_ontology=False)
         payloads[RANDOM] = self.random_enrichment(gene_set)
         payloads[RANK_BASED] = self.null_enrichment(gene_set)
         payloads[CLOSURE] = self.gene_term_closure(gene_set)
         for k in [STANDARD, STANDARD_NO_ONTOLOGY, RANDOM, RANK_BASED]:
             payloads[k].method = k
         comp = GeneSetComparison(
-            name=name,
-            gene_symbols=gene_symbols,
+            name=gene_set.name,
+            gene_symbols=gene_set.gene_symbols,
+            gene_ids=gene_set.gene_ids,
+            number_of_genes_swapped_out=gene_set.number_of_genes_dropped,
             payloads=payloads,
             **kwargs,
         )
         return comp
 
     def random_gene_symbol(self) -> ENTITY_ID:
         """Get a random gene."""
         assocs = list(self.ontology.associations())
         logger.debug(f"Got {len(assocs)} associations")
         ann = random.SystemRandom().choice(assocs)
         info = gene_info(ann.subject)
         return info[0]
 
     def standard_enrichment(self, gene_set: GeneSet, use_ontology=True) -> EnrichmentPayload:
-        """Enrichment."""
+        """Perform standard gene set enrichment.
+
+        :param gene_set: GeneSet object, with gene_ids populated
+        """
         gene_ids = gene_set.gene_ids
         if use_ontology:
             predicates = [IS_A, PART_OF]
         else:
             predicates = [EQUIVALENT_CLASS]  # TODO
         results = self.ontology.enriched_classes(
             gene_ids, autolabel=True, object_closure_predicates=predicates
@@ -309,19 +294,40 @@
         symbols = set([sym for sym, _ in tupls])
         m = map_hgnc_symbols(tuple(symbols))
         for sym, _ in tupls:
             if sym in m:
                 yield sym, m[sym]
                 continue
 
-    def load_annotations(self, path=None) -> None:
-        """Load."""
+    def load_annotations(self, path=None, format=None) -> None:
+        """
+        Load annotations from a two-column TSV file or a GAF.
+
+        :param path:
+        :return:
+        """
         if self.loaded:
             return
-        m = get_symbol_to_gene_id_map()
         assocs = []
-        for sym, term_id in self.get_annotation_tuples(path):
-            if sym in m:
-                gene_id = m[sym]
-                assocs.append(Association(subject=gene_id, object=term_id))
+        if not format:
+            if path.endswith(".tsv.gz"):
+                format = "tsv.gz"
+            elif path.endswith(".gaf"):
+                format = "gaf"
+            else:
+                raise ValueError(f"Unknown format: {format}")
+        if format == "tsv.gz":
+            # We have a slightly awkward special case for HGNC as the GO GAFs
+            # use UniProtKB IDs
+            m = get_symbol_to_gene_id_map()
+            for sym, term_id in self.get_annotation_tuples(path):
+                if sym in m:
+                    gene_id = m[sym]
+                    assocs.append(Association(subject=gene_id, object=term_id))
+        elif format == "gaf":
+            association_parser = get_association_parser("gaf")
+            with open(path) as file:
+                assocs = list(association_parser.parse(file))
+        else:
+            raise ValueError(f"Unknown format: {format}")
         self.ontology.add_associations(assocs)
         self.loaded = True
```

### Comparing `ontogpt-0.2.3/src/ontogpt/evaluation/evaluation_engine.py` & `ontogpt-0.2.4/src/ontogpt/evaluation/evaluation_engine.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.3/src/ontogpt/evaluation/go/eval_go.py` & `ontogpt-0.2.4/src/ontogpt/evaluation/go/eval_go.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.3/src/ontogpt/evaluation/hpoa/eval_hpoa.py` & `ontogpt-0.2.4/src/ontogpt/evaluation/hpoa/eval_hpoa.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.3/src/ontogpt/evaluation/ibd/PMC6386158_fig2_legend.txt` & `ontogpt-0.2.4/src/ontogpt/evaluation/ibd/PMC6386158_fig2_legend.txt`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.3/src/ontogpt/evaluation/ibd/PMC6386158_fig2_legend.yaml` & `ontogpt-0.2.4/src/ontogpt/evaluation/ibd/PMC6386158_fig2_legend.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.3/src/ontogpt/evaluation/resolver.py` & `ontogpt-0.2.4/src/ontogpt/evaluation/resolver.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.3/src/ontogpt/io/html_exporter.py` & `ontogpt-0.2.4/src/ontogpt/io/html_exporter.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.3/src/ontogpt/io/markdown_exporter.py` & `ontogpt-0.2.4/src/ontogpt/io/markdown_exporter.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.3/src/ontogpt/io/owl_exporter.py` & `ontogpt-0.2.4/src/ontogpt/io/owl_exporter.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.3/src/ontogpt/io/rdf_exporter.py` & `ontogpt-0.2.4/src/ontogpt/io/rdf_exporter.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.3/src/ontogpt/io/yaml_wrapper.py` & `ontogpt-0.2.4/src/ontogpt/io/yaml_wrapper.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.3/src/ontogpt/prompts/enrichment/gene_set_summarization.jinja2` & `ontogpt-0.2.4/src/ontogpt/prompts/enrichment/gene_set_summarization.jinja2`

 * *Files 10% similar despite different names*

```diff
@@ -10,21 +10,24 @@
 
 Provide results in the format
 
 {{SUMMARY_KEYWORD}}: <high level summary>
 {{MECHANISM_KEYWORD}}: <mechanism>
 {{ENRICHED_TERMS_KEYWORD}}: <term1>; <term2>; <term3>
 
-###
+For the list of terms, be sure to use a semi-colon separator, and do not number the list.
+Always put the list of terms last, after mechanism, summary, or hypotheses.
 
 {% if annotations %}
 Here are the gene summaries:
 
 {% for gd in gene_descriptions %}
 {{ gd[0] }}: {{ gd[1] }}
 {% endfor %}
 {% else %}
 Here are the genes:
 {% for gd in gene_descriptions %}{{ gd[0] }}; {% endfor %}
 {% endif %}
 
+{{END_MARKER}}
+
 Summary and enriched terms:
```

### Comparing `ontogpt-0.2.3/src/ontogpt/prompts/enrichment/gene_set_summarization_with_p_values.jinja2` & `ontogpt-0.2.4/src/ontogpt/prompts/enrichment/gene_set_summarization_with_p_values_0.jinja2`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.3/src/ontogpt/prompts/similarity/connections.jinja2` & `ontogpt-0.2.4/src/ontogpt/prompts/similarity/connections.jinja2`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.3/src/ontogpt/templates/biological_process.py` & `ontogpt-0.2.4/src/ontogpt/templates/biological_process.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.3/src/ontogpt/templates/biological_process.yaml` & `ontogpt-0.2.4/src/ontogpt/templates/biological_process.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.3/src/ontogpt/templates/class_enrichment.py` & `ontogpt-0.2.4/src/ontogpt/templates/class_enrichment.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.3/src/ontogpt/templates/class_enrichment.yaml` & `ontogpt-0.2.4/src/ontogpt/templates/class_enrichment.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.3/src/ontogpt/templates/core.py` & `ontogpt-0.2.4/src/ontogpt/templates/core.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.3/src/ontogpt/templates/core.yaml` & `ontogpt-0.2.4/src/ontogpt/templates/core.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.3/src/ontogpt/templates/ctd.py` & `ontogpt-0.2.4/src/ontogpt/templates/ctd.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.3/src/ontogpt/templates/ctd.yaml` & `ontogpt-0.2.4/src/ontogpt/templates/ctd.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.3/src/ontogpt/templates/drug.py` & `ontogpt-0.2.4/src/ontogpt/templates/drug.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.3/src/ontogpt/templates/drug.yaml` & `ontogpt-0.2.4/src/ontogpt/templates/drug.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.3/src/ontogpt/templates/environmental_sample.py` & `ontogpt-0.2.4/src/ontogpt/templates/environmental_sample.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.3/src/ontogpt/templates/environmental_sample.yaml` & `ontogpt-0.2.4/src/ontogpt/templates/environmental_sample.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.3/src/ontogpt/templates/gene_description_term.py` & `ontogpt-0.2.4/src/ontogpt/templates/gene_description_term.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.3/src/ontogpt/templates/gene_description_term.yaml` & `ontogpt-0.2.4/src/ontogpt/templates/gene_description_term.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.3/src/ontogpt/templates/gocam.py` & `ontogpt-0.2.4/src/ontogpt/templates/gocam.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.3/src/ontogpt/templates/gocam.yaml` & `ontogpt-0.2.4/src/ontogpt/templates/gocam.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.3/src/ontogpt/templates/halo.py` & `ontogpt-0.2.4/src/ontogpt/templates/halo.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.3/src/ontogpt/templates/halo.yaml` & `ontogpt-0.2.4/src/ontogpt/templates/halo.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.3/src/ontogpt/templates/ibd.py` & `ontogpt-0.2.4/src/ontogpt/templates/ibd.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.3/src/ontogpt/templates/ibd.yaml` & `ontogpt-0.2.4/src/ontogpt/templates/ibd.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.3/src/ontogpt/templates/mendelian_disease.py` & `ontogpt-0.2.4/src/ontogpt/templates/mendelian_disease.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.3/src/ontogpt/templates/mendelian_disease.yaml` & `ontogpt-0.2.4/src/ontogpt/templates/mendelian_disease.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.3/src/ontogpt/templates/metabolic_process.py` & `ontogpt-0.2.4/src/ontogpt/templates/metabolic_process.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.3/src/ontogpt/templates/metabolic_process.yaml` & `ontogpt-0.2.4/src/ontogpt/templates/metabolic_process.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.3/src/ontogpt/templates/metagenome_study.py` & `ontogpt-0.2.4/src/ontogpt/templates/metagenome_study.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.3/src/ontogpt/templates/metagenome_study.yaml` & `ontogpt-0.2.4/src/ontogpt/templates/metagenome_study.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.3/src/ontogpt/templates/ontology_class.py` & `ontogpt-0.2.4/src/ontogpt/templates/ontology_class.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.3/src/ontogpt/templates/ontology_class.yaml` & `ontogpt-0.2.4/src/ontogpt/templates/ontology_class.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.3/src/ontogpt/templates/phenotype.py` & `ontogpt-0.2.4/src/ontogpt/templates/phenotype.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.3/src/ontogpt/templates/phenotype.yaml` & `ontogpt-0.2.4/src/ontogpt/templates/phenotype.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.3/src/ontogpt/templates/reaction.py` & `ontogpt-0.2.4/src/ontogpt/templates/reaction.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.3/src/ontogpt/templates/reaction.yaml` & `ontogpt-0.2.4/src/ontogpt/templates/reaction.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.3/src/ontogpt/templates/recipe.py` & `ontogpt-0.2.4/src/ontogpt/templates/recipe.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.3/src/ontogpt/templates/recipe.yaml` & `ontogpt-0.2.4/src/ontogpt/templates/recipe.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.3/src/ontogpt/templates/treatment.py` & `ontogpt-0.2.4/src/ontogpt/templates/treatment.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.3/src/ontogpt/templates/treatment.yaml` & `ontogpt-0.2.4/src/ontogpt/templates/treatment.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.3/src/ontogpt/webapp/html/form.html` & `ontogpt-0.2.4/src/ontogpt/webapp/html/form.html`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.3/src/ontogpt/webapp/html/spindoctor/form.html` & `ontogpt-0.2.4/src/ontogpt/webapp/html/spindoctor/form.html`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.3/src/ontogpt/webapp/main.py` & `ontogpt-0.2.4/src/ontogpt/webapp/main.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.3/PKG-INFO` & `ontogpt-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ontogpt
-Version: 0.2.3
+Version: 0.2.4
 Summary: OntoGPT
 License: BSD-3
 Author: Chris Mungall
 Author-email: cjmungall@lbl.gov
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -33,18 +33,19 @@
 Requires-Dist: inflection (>=0.5.1,<0.6.0)
 Requires-Dist: jsonlines (>=3.1.0,<4.0.0)
 Requires-Dist: linkml (>=1.4.10,<2.0.0)
 Requires-Dist: linkml-owl (>=0.2.7,<0.3.0)
 Requires-Dist: linkml-runtime (>=1.4.9,<2.0.0)
 Requires-Dist: myst-parser[docs] (>=0.18.1,<0.19.0) ; extra == "docs"
 Requires-Dist: nlpcloud (>=1.0.39,<2.0.0)
-Requires-Dist: oaklib (>=0.5.2,<0.6.0)
+Requires-Dist: oaklib (>=0.5.4,<0.6.0)
 Requires-Dist: openai (>=0.27.4,<0.28.0)
 Requires-Dist: python-multipart (>=0.0.5,<0.0.6)
 Requires-Dist: recipe-scrapers[recipes] (>=14.35.0,<15.0.0) ; extra == "recipes"
+Requires-Dist: requests-cache (>=1.0.1,<2.0.0)
 Requires-Dist: rustsim (>=0.1.8,<0.2.0)
 Requires-Dist: sphinx-autodoc-typehints[docs] (>=1.19.4,<2.0.0) ; extra == "docs"
 Requires-Dist: sphinx-click[docs] (>=4.3.0,<5.0.0) ; extra == "docs"
 Requires-Dist: sphinx-rtd-theme[docs] (>=1.0.0,<2.0.0) ; extra == "docs"
 Requires-Dist: sphinx[docs] (>=5.3.0,<6.0.0) ; extra == "docs"
 Requires-Dist: tiktoken (>=0.3.3,<0.4.0)
 Requires-Dist: uvicorn (>=0.20.0,<0.21.0) ; extra == "web"
```

