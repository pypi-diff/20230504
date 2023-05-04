# Comparing `tmp/bioregistry-0.9.3.tar.gz` & `tmp/bioregistry-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bioregistry-0.9.3.tar", last modified: Wed May  3 01:25:12 2023, max compression
+gzip compressed data, was "bioregistry-0.9.4.tar", last modified: Thu May  4 01:23:46 2023, max compression
```

## Comparing `bioregistry-0.9.3.tar` & `bioregistry-0.9.4.tar`

### file list

```diff
@@ -1,340 +1,340 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:25:12.742037 bioregistry-0.9.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-03 00:46:38.000000 bioregistry-0.9.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-03 00:46:38.000000 bioregistry-0.9.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    31510 2023-05-03 01:25:12.742037 bioregistry-0.9.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    30194 2023-05-03 00:46:38.000000 bioregistry-0.9.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:25:12.662032 bioregistry-0.9.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-05-03 00:46:38.000000 bioregistry-0.9.3/docs/bulk_prefix_request_template.tsv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:25:12.666033 bioregistry-0.9.3/docs/img/
--rw-r--r--   0 runner    (1001) docker     (123)    48331 2023-05-03 01:12:01.000000 bioregistry-0.9.3/docs/img/bibliography_years.svg
--rw-r--r--   0 runner    (1001) docker     (123)   156964 2023-05-03 01:12:20.000000 bioregistry-0.9.3/docs/img/bioregistry_coverage.svg
--rw-r--r--   0 runner    (1001) docker     (123)   107017 2023-05-03 01:12:19.000000 bioregistry-0.9.3/docs/img/bioregistry_coverage_bar.svg
--rw-r--r--   0 runner    (1001) docker     (123)    84693 2023-05-03 01:12:20.000000 bioregistry-0.9.3/docs/img/bioregistry_coverage_bar_short.svg
--rw-r--r--   0 runner    (1001) docker     (123)    77372 2023-05-03 00:46:38.000000 bioregistry-0.9.3/docs/img/datamodel_umls.svg
--rw-r--r--   0 runner    (1001) docker     (123)  1382073 2023-05-03 01:16:08.000000 bioregistry-0.9.3/docs/img/external_overlap.svg
--rw-r--r--   0 runner    (1001) docker     (123)    72498 2023-05-03 01:12:45.000000 bioregistry-0.9.3/docs/img/has_attribute.svg
--rw-r--r--   0 runner    (1001) docker     (123)    28419 2023-05-03 01:16:09.000000 bioregistry-0.9.3/docs/img/providers.svg
--rw-r--r--   0 runner    (1001) docker     (123)    22303 2023-05-03 01:16:10.000000 bioregistry-0.9.3/docs/img/regex_report.svg
--rw-r--r--   0 runner    (1001) docker     (123)    51528 2023-05-03 01:12:18.000000 bioregistry-0.9.3/docs/img/xrefs.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:25:12.666033 bioregistry-0.9.3/docs/source/
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-03 00:46:38.000000 bioregistry-0.9.3/docs/source/alignment.rst
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-03 00:46:38.000000 bioregistry-0.9.3/docs/source/cli.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7033 2023-05-03 01:25:02.000000 bioregistry-0.9.3/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     8480 2023-05-03 00:46:38.000000 bioregistry-0.9.3/docs/source/deployment.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-05-03 00:46:38.000000 bioregistry-0.9.3/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)   214468 2023-05-03 00:46:38.000000 bioregistry-0.9.3/docs/source/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-03 00:46:38.000000 bioregistry-0.9.3/docs/source/pandas.rst
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-03 00:46:38.000000 bioregistry-0.9.3/docs/source/reference.rst
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-03 00:46:38.000000 bioregistry-0.9.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-05-03 01:25:12.742037 bioregistry-0.9.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:25:12.654032 bioregistry-0.9.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:25:12.670033 bioregistry-0.9.3/src/bioregistry/
--rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:25:12.674033 bioregistry-0.9.3/src/bioregistry/align/
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/align/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/align/aberowl.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/align/bartoc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/align/biocontext.py
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/align/biolink.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/align/bioportal.py
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/align/cellosaurus.py
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/align/cheminf.py
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/align/cropoct.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/align/edam.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/align/fairsharing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2544 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/align/go.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/align/hl7.py
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/align/miriam.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/align/n2t.py
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/align/ncbi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/align/obofoundry.py
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/align/ols.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/align/ontobee.py
--rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/align/prefixcommons.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/align/re3data.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/align/uniprot.py
--rw-r--r--   0 runner    (1001) docker     (123)    10718 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/align/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/align/wikidata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:25:12.674033 bioregistry-0.9.3/src/bioregistry/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5007 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/analysis/title_tfidf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:25:12.674033 bioregistry-0.9.3/src/bioregistry/app/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17624 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/app/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/app/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/app/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    10179 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/app/impl.py
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/app/proxies.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:25:12.678033 bioregistry-0.9.3/src/bioregistry/app/static/
--rw-r--r--   0 runner    (1001) docker     (123)   801449 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/app/static/logo.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:25:12.678033 bioregistry-0.9.3/src/bioregistry/app/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     9662 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/app/templates/base.html
--rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/app/templates/collection.html
--rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/app/templates/collections.html
--rw-r--r--   0 runner    (1001) docker     (123)     6758 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/app/templates/context.html
--rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/app/templates/contexts.html
--rw-r--r--   0 runner    (1001) docker     (123)     7134 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/app/templates/contributor.html
--rw-r--r--   0 runner    (1001) docker     (123)     4670 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/app/templates/contributors.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:25:12.678033 bioregistry-0.9.3/src/bioregistry/app/templates/highlights/
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/app/templates/highlights/keywords.html
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/app/templates/highlights/owners.html
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/app/templates/highlights/relations.html
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/app/templates/highlights/twitter.html
--rw-r--r--   0 runner    (1001) docker     (123)    15622 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/app/templates/home.html
--rw-r--r--   0 runner    (1001) docker     (123)     7351 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/app/templates/macros.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:25:12.682034 bioregistry-0.9.3/src/bioregistry/app/templates/meta/
--rw-r--r--   0 runner    (1001) docker     (123)     5577 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/app/templates/meta/access.html
--rw-r--r--   0 runner    (1001) docker     (123)    19835 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/app/templates/meta/acknowledgements.html
--rw-r--r--   0 runner    (1001) docker     (123)    10695 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/app/templates/meta/download.html
--rw-r--r--   0 runner    (1001) docker     (123)    16544 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/app/templates/meta/related.html
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/app/templates/meta/schema.html
--rw-r--r--   0 runner    (1001) docker     (123)    19312 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/app/templates/meta/summary.html
--rw-r--r--   0 runner    (1001) docker     (123)     8813 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/app/templates/meta/sustainability.html
--rw-r--r--   0 runner    (1001) docker     (123)     8460 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/app/templates/metaresource.html
--rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/app/templates/metaresources.html
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/app/templates/prose.html
--rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/app/templates/reference.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:25:12.682034 bioregistry-0.9.3/src/bioregistry/app/templates/resolve_errors/
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/app/templates/resolve_errors/disallowed_identifier.html
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/app/templates/resolve_errors/invalid_identifier.html
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/app/templates/resolve_errors/missing_prefix.html
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/app/templates/resolve_errors/missing_providers.html
--rw-r--r--   0 runner    (1001) docker     (123)    32484 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/app/templates/resource.html
--rw-r--r--   0 runner    (1001) docker     (123)     3765 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/app/templates/resources.html
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/app/test.py
--rw-r--r--   0 runner    (1001) docker     (123)    19423 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/app/ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     8073 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/app/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/app/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:25:12.682034 bioregistry-0.9.3/src/bioregistry/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/benchmarks/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/benchmarks/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/benchmarks/curie_parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/benchmarks/curie_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/benchmarks/uri_parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/bibliometrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/collection_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    23802 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/compare.py
--rw-r--r--   0 runner    (1001) docker     (123)     5293 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:25:12.686034 bioregistry-0.9.3/src/bioregistry/curation/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/curation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/curation/add_co_providers.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/curation/add_descriptions_from_gs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/curation/add_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/curation/add_examples_from_javert.py
--rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/curation/add_examples_from_ols.py
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/curation/add_ontology_regexes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/curation/bulk_import.py
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/curation/clean_licenses.py
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/curation/clean_name_suffixes.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/curation/clean_publications.py
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/curation/cleanup_authors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/curation/deprecation_diff.py
--rw-r--r--   0 runner    (1001) docker     (123)     4940 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/curation/enrich_publications.py
--rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/curation/import_pc_semiautomatic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/curation/make_description_curation_sheet.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/curation/map_bartoc_via_wikidata.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/curation/map_re3data_via_fairsharing.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/curation/rename_metaprefix.py
--rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/curation/review_pc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/curation/suggest_author_curation.py
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/curation/suggest_uniprot_providers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:25:12.694034 bioregistry-0.9.3/src/bioregistry/data/
--rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/data/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  4590753 2023-05-03 01:10:07.000000 bioregistry-0.9.3/src/bioregistry/data/bioregistry.json
--rw-r--r--   0 runner    (1001) docker     (123)    11750 2023-05-03 01:10:07.000000 bioregistry-0.9.3/src/bioregistry/data/collections.json
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-03 01:10:07.000000 bioregistry-0.9.3/src/bioregistry/data/contexts.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:25:12.658032 bioregistry-0.9.3/src/bioregistry/data/external/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:25:12.694034 bioregistry-0.9.3/src/bioregistry/data/external/aberowl/
--rw-r--r--   0 runner    (1001) docker     (123)   302925 2023-05-03 00:55:02.000000 bioregistry-0.9.3/src/bioregistry/data/external/aberowl/curation.tsv
--rw-r--r--   0 runner    (1001) docker     (123)   623701 2023-05-03 00:55:01.000000 bioregistry-0.9.3/src/bioregistry/data/external/aberowl/processed.json
--rw-r--r--   0 runner    (1001) docker     (123)  1280745 2023-05-03 00:54:54.000000 bioregistry-0.9.3/src/bioregistry/data/external/aberowl/raw.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:25:12.694034 bioregistry-0.9.3/src/bioregistry/data/external/agroportal/
--rw-r--r--   0 runner    (1001) docker     (123)    42168 2023-05-03 01:10:02.000000 bioregistry-0.9.3/src/bioregistry/data/external/agroportal/curation.tsv
--rw-r--r--   0 runner    (1001) docker     (123)   124136 2023-05-03 01:10:01.000000 bioregistry-0.9.3/src/bioregistry/data/external/agroportal/processed.json
--rw-r--r--   0 runner    (1001) docker     (123)   663568 2023-05-03 01:10:01.000000 bioregistry-0.9.3/src/bioregistry/data/external/agroportal/raw.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:25:12.698035 bioregistry-0.9.3/src/bioregistry/data/external/bartoc/
--rw-r--r--   0 runner    (1001) docker     (123)  1835101 2023-05-03 01:10:06.000000 bioregistry-0.9.3/src/bioregistry/data/external/bartoc/curation.tsv
--rw-r--r--   0 runner    (1001) docker     (123)  2216766 2023-05-03 01:10:06.000000 bioregistry-0.9.3/src/bioregistry/data/external/bartoc/processed.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:25:12.702035 bioregistry-0.9.3/src/bioregistry/data/external/biocontext/
--rw-r--r--   0 runner    (1001) docker     (123)     5057 2023-05-03 01:05:57.000000 bioregistry-0.9.3/src/bioregistry/data/external/biocontext/curation.tsv
--rw-r--r--   0 runner    (1001) docker     (123)    74913 2023-05-03 01:05:56.000000 bioregistry-0.9.3/src/bioregistry/data/external/biocontext/processed.json
--rw-r--r--   0 runner    (1001) docker     (123)    55878 2023-05-03 01:05:56.000000 bioregistry-0.9.3/src/bioregistry/data/external/biocontext/raw.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:25:12.702035 bioregistry-0.9.3/src/bioregistry/data/external/biolink/
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-05-03 01:06:04.000000 bioregistry-0.9.3/src/bioregistry/data/external/biolink/curation.tsv
--rw-r--r--   0 runner    (1001) docker     (123)    10406 2023-05-03 01:06:04.000000 bioregistry-0.9.3/src/bioregistry/data/external/biolink/processed.json
--rw-r--r--   0 runner    (1001) docker     (123)   354352 2023-05-03 01:06:03.000000 bioregistry-0.9.3/src/bioregistry/data/external/biolink/raw.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:25:12.706035 bioregistry-0.9.3/src/bioregistry/data/external/bioportal/
--rw-r--r--   0 runner    (1001) docker     (123)   253653 2023-05-03 01:05:51.000000 bioregistry-0.9.3/src/bioregistry/data/external/bioportal/curation.tsv
--rw-r--r--   0 runner    (1001) docker     (123)   606697 2023-05-03 01:05:50.000000 bioregistry-0.9.3/src/bioregistry/data/external/bioportal/processed.json
--rw-r--r--   0 runner    (1001) docker     (123)  3539114 2023-05-03 01:05:50.000000 bioregistry-0.9.3/src/bioregistry/data/external/bioportal/raw.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:25:12.710035 bioregistry-0.9.3/src/bioregistry/data/external/cellosaurus/
--rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-05-03 01:01:21.000000 bioregistry-0.9.3/src/bioregistry/data/external/cellosaurus/curation.tsv
--rw-r--r--   0 runner    (1001) docker     (123)    28730 2023-05-03 01:01:20.000000 bioregistry-0.9.3/src/bioregistry/data/external/cellosaurus/processed.json
--rw-r--r--   0 runner    (1001) docker     (123)    32374 2023-05-03 01:01:20.000000 bioregistry-0.9.3/src/bioregistry/data/external/cellosaurus/raw.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:25:12.710035 bioregistry-0.9.3/src/bioregistry/data/external/cheminf/
--rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-05-03 01:08:37.000000 bioregistry-0.9.3/src/bioregistry/data/external/cheminf/processed.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:25:12.710035 bioregistry-0.9.3/src/bioregistry/data/external/cropoct/
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-05-03 01:01:29.000000 bioregistry-0.9.3/src/bioregistry/data/external/cropoct/curation.tsv
--rw-r--r--   0 runner    (1001) docker     (123)    11407 2023-05-03 01:01:29.000000 bioregistry-0.9.3/src/bioregistry/data/external/cropoct/processed.json
--rw-r--r--   0 runner    (1001) docker     (123)    25353 2023-05-03 01:01:29.000000 bioregistry-0.9.3/src/bioregistry/data/external/cropoct/raw.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:25:12.710035 bioregistry-0.9.3/src/bioregistry/data/external/ecoportal/
--rw-r--r--   0 runner    (1001) docker     (123)     9198 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/data/external/ecoportal/curation.tsv
--rw-r--r--   0 runner    (1001) docker     (123)    18773 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/data/external/ecoportal/processed.json
--rw-r--r--   0 runner    (1001) docker     (123)    98149 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/data/external/ecoportal/raw.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:25:12.710035 bioregistry-0.9.3/src/bioregistry/data/external/edam/
--rw-r--r--   0 runner    (1001) docker     (123)    14599 2023-05-03 01:08:34.000000 bioregistry-0.9.3/src/bioregistry/data/external/edam/curation.tsv
--rw-r--r--   0 runner    (1001) docker     (123)    45616 2023-05-03 01:08:34.000000 bioregistry-0.9.3/src/bioregistry/data/external/edam/processed.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:25:12.710035 bioregistry-0.9.3/src/bioregistry/data/external/fairsharing/
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/data/external/fairsharing/README.md
--rw-r--r--   0 runner    (1001) docker     (123)   253585 2023-05-03 01:01:14.000000 bioregistry-0.9.3/src/bioregistry/data/external/fairsharing/curation.tsv
--rw-r--r--   0 runner    (1001) docker     (123)   744872 2023-05-03 01:01:13.000000 bioregistry-0.9.3/src/bioregistry/data/external/fairsharing/processed.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:25:12.714036 bioregistry-0.9.3/src/bioregistry/data/external/go/
--rw-r--r--   0 runner    (1001) docker     (123)     7502 2023-05-03 01:08:25.000000 bioregistry-0.9.3/src/bioregistry/data/external/go/curation.tsv
--rw-r--r--   0 runner    (1001) docker     (123)   143024 2023-05-03 01:08:24.000000 bioregistry-0.9.3/src/bioregistry/data/external/go/processed.json
--rw-r--r--   0 runner    (1001) docker     (123)   115035 2023-05-03 01:08:24.000000 bioregistry-0.9.3/src/bioregistry/data/external/go/raw.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:25:12.714036 bioregistry-0.9.3/src/bioregistry/data/external/hl7/
--rw-r--r--   0 runner    (1001) docker     (123)   157660 2023-05-03 01:01:23.000000 bioregistry-0.9.3/src/bioregistry/data/external/hl7/curation.tsv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:25:12.714036 bioregistry-0.9.3/src/bioregistry/data/external/miriam/
--rw-r--r--   0 runner    (1001) docker     (123)   576520 2023-05-03 01:06:00.000000 bioregistry-0.9.3/src/bioregistry/data/external/miriam/processed.json
--rw-r--r--   0 runner    (1001) docker     (123)  1987182 2023-05-03 01:06:00.000000 bioregistry-0.9.3/src/bioregistry/data/external/miriam/raw.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:25:12.718036 bioregistry-0.9.3/src/bioregistry/data/external/n2t/
--rw-r--r--   0 runner    (1001) docker     (123)   425371 2023-05-03 01:01:37.000000 bioregistry-0.9.3/src/bioregistry/data/external/n2t/processed.json
--rw-r--r--   0 runner    (1001) docker     (123)  1278753 2023-05-03 01:01:32.000000 bioregistry-0.9.3/src/bioregistry/data/external/n2t/raw.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:25:12.718036 bioregistry-0.9.3/src/bioregistry/data/external/ncbi/
--rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-05-03 01:01:26.000000 bioregistry-0.9.3/src/bioregistry/data/external/ncbi/curation.tsv
--rw-r--r--   0 runner    (1001) docker     (123)    18072 2023-05-03 01:01:26.000000 bioregistry-0.9.3/src/bioregistry/data/external/ncbi/processed.json
--rw-r--r--   0 runner    (1001) docker     (123)   103465 2023-05-03 01:01:26.000000 bioregistry-0.9.3/src/bioregistry/data/external/ncbi/raw.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:25:12.718036 bioregistry-0.9.3/src/bioregistry/data/external/obofoundry/
--rw-r--r--   0 runner    (1001) docker     (123)   212323 2023-05-03 01:08:41.000000 bioregistry-0.9.3/src/bioregistry/data/external/obofoundry/processed.json
--rw-r--r--   0 runner    (1001) docker     (123)   350196 2023-05-03 01:08:39.000000 bioregistry-0.9.3/src/bioregistry/data/external/obofoundry/raw.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:25:12.722036 bioregistry-0.9.3/src/bioregistry/data/external/ols/
--rw-r--r--   0 runner    (1001) docker     (123)   141937 2023-05-03 00:54:46.000000 bioregistry-0.9.3/src/bioregistry/data/external/ols/processed.json
--rw-r--r--   0 runner    (1001) docker     (123)   805618 2023-05-03 00:54:46.000000 bioregistry-0.9.3/src/bioregistry/data/external/ols/raw.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:25:12.722036 bioregistry-0.9.3/src/bioregistry/data/external/ontobee/
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-05-03 01:08:28.000000 bioregistry-0.9.3/src/bioregistry/data/external/ontobee/curation.tsv
--rw-r--r--   0 runner    (1001) docker     (123)    23684 2023-05-03 01:08:27.000000 bioregistry-0.9.3/src/bioregistry/data/external/ontobee/processed.json
--rw-r--r--   0 runner    (1001) docker     (123)   192177 2023-05-03 01:08:27.000000 bioregistry-0.9.3/src/bioregistry/data/external/ontobee/raw.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:25:12.722036 bioregistry-0.9.3/src/bioregistry/data/external/prefixcommons/
--rw-r--r--   0 runner    (1001) docker     (123)   111600 2023-05-03 01:01:17.000000 bioregistry-0.9.3/src/bioregistry/data/external/prefixcommons/curation.tsv
--rw-r--r--   0 runner    (1001) docker     (123)   505834 2023-05-03 01:01:17.000000 bioregistry-0.9.3/src/bioregistry/data/external/prefixcommons/processed.json
--rw-r--r--   0 runner    (1001) docker     (123)   883990 2023-05-03 01:01:17.000000 bioregistry-0.9.3/src/bioregistry/data/external/prefixcommons/raw.tsv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:25:12.726036 bioregistry-0.9.3/src/bioregistry/data/external/re3data/
--rw-r--r--   0 runner    (1001) docker     (123)  1742293 2023-05-03 00:54:41.000000 bioregistry-0.9.3/src/bioregistry/data/external/re3data/curation.tsv
--rw-r--r--   0 runner    (1001) docker     (123)  2438516 2023-05-03 00:54:40.000000 bioregistry-0.9.3/src/bioregistry/data/external/re3data/processed.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:25:12.730037 bioregistry-0.9.3/src/bioregistry/data/external/uniprot/
--rw-r--r--   0 runner    (1001) docker     (123)    10813 2023-05-03 01:05:54.000000 bioregistry-0.9.3/src/bioregistry/data/external/uniprot/curation.tsv
--rw-r--r--   0 runner    (1001) docker     (123)    67298 2023-05-03 01:05:54.000000 bioregistry-0.9.3/src/bioregistry/data/external/uniprot/processed.json
--rw-r--r--   0 runner    (1001) docker     (123)    89651 2023-05-03 01:05:54.000000 bioregistry-0.9.3/src/bioregistry/data/external/uniprot/raw.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:25:12.730037 bioregistry-0.9.3/src/bioregistry/data/external/wikidata/
--rw-r--r--   0 runner    (1001) docker     (123)   125505 2023-05-03 01:08:22.000000 bioregistry-0.9.3/src/bioregistry/data/external/wikidata/curation.tsv
--rw-r--r--   0 runner    (1001) docker     (123)   319146 2023-05-03 01:08:21.000000 bioregistry-0.9.3/src/bioregistry/data/external/wikidata/processed.json
--rw-r--r--   0 runner    (1001) docker     (123)    47301 2023-05-03 01:10:07.000000 bioregistry-0.9.3/src/bioregistry/data/metaregistry.json
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-05-03 01:10:07.000000 bioregistry-0.9.3/src/bioregistry/data/mismatch.json
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/data/processing_biolink.json
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/data/processing_go.json
--rw-r--r--   0 runner    (1001) docker     (123)    29821 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/data/processing_ols.json
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/data/processing_wikidata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:25:12.734037 bioregistry-0.9.3/src/bioregistry/export/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/export/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/export/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/export/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/export/prefix_maps.py
--rw-r--r--   0 runner    (1001) docker     (123)     8861 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/export/rdf_export.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/export/schema_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/export/sssom_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     8994 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/export/tables_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/export/tsv_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     4617 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/export/warnings_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/export/yaml_export.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:25:12.734037 bioregistry-0.9.3/src/bioregistry/external/
--rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/external/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/external/aberowl.py
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/external/bartoc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/external/biocontext.py
--rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/external/biolink.py
--rw-r--r--   0 runner    (1001) docker     (123)     6997 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/external/bioportal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/external/cellosaurus.py
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/external/cheminf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/external/cropoct.py
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/external/edam.py
--rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/external/fairsharing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/external/go.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:25:12.738037 bioregistry-0.9.3/src/bioregistry/external/hl7/
--rw-r--r--   0 runner    (1001) docker     (123)   319976 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/external/hl7/OID_Report.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/external/hl7/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/external/miriam.py
--rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/external/n2t.py
--rw-r--r--   0 runner    (1001) docker     (123)     4839 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/external/ncbi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/external/obofoundry.py
--rw-r--r--   0 runner    (1001) docker     (123)     7610 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/external/ols.py
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/external/ontobee.py
--rw-r--r--   0 runner    (1001) docker     (123)     4154 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/external/prefixcommons.py
--rw-r--r--   0 runner    (1001) docker     (123)     6191 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/external/re3data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/external/uniprot.py
--rw-r--r--   0 runner    (1001) docker     (123)     7988 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/external/wikidata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:25:12.738037 bioregistry-0.9.3/src/bioregistry/gh/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/gh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8350 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/gh/github_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9789 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/gh/new_prefix.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:25:12.738037 bioregistry-0.9.3/src/bioregistry/health/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/health/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/health/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/health/check_homepages.py
--rw-r--r--   0 runner    (1001) docker     (123)     7053 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/health/check_providers.py
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/health/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     8571 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/license_standardizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/lint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/metaresource_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18936 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/parse_iri.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    13281 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/record_accumulator.py
--rw-r--r--   0 runner    (1001) docker     (123)    33164 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/resolve.py
--rw-r--r--   0 runner    (1001) docker     (123)    17532 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/resolve_identifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    63936 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/resource_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:25:12.738037 bioregistry-0.9.3/src/bioregistry/schema/
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13218 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/schema/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    42222 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/schema/schema.json
--rw-r--r--   0 runner    (1001) docker     (123)   106399 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/schema/struct.py
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/schema/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8188 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/schema_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10183 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     5517 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/upload_ndex.py
--rw-r--r--   0 runner    (1001) docker     (123)     7175 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/uri_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     8067 2023-05-03 00:46:38.000000 bioregistry-0.9.3/src/bioregistry/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-03 01:25:02.000000 bioregistry-0.9.3/src/bioregistry/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:25:12.670033 bioregistry-0.9.3/src/bioregistry.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    31510 2023-05-03 01:25:12.000000 bioregistry-0.9.3/src/bioregistry.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11234 2023-05-03 01:25:12.000000 bioregistry-0.9.3/src/bioregistry.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 01:25:12.000000 bioregistry-0.9.3/src/bioregistry.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-03 01:25:12.000000 bioregistry-0.9.3/src/bioregistry.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 00:46:53.000000 bioregistry-0.9.3/src/bioregistry.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-05-03 01:25:12.000000 bioregistry-0.9.3/src/bioregistry.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-03 01:25:12.000000 bioregistry-0.9.3/src/bioregistry.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:25:12.742037 bioregistry-0.9.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-03 00:46:38.000000 bioregistry-0.9.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-05-03 00:46:38.000000 bioregistry-0.9.3/tests/test_acquisition.py
--rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-05-03 00:46:38.000000 bioregistry-0.9.3/tests/test_collections.py
--rw-r--r--   0 runner    (1001) docker     (123)     5177 2023-05-03 00:46:38.000000 bioregistry-0.9.3/tests/test_contexts.py
--rw-r--r--   0 runner    (1001) docker     (123)    46880 2023-05-03 00:46:38.000000 bioregistry-0.9.3/tests/test_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-05-03 00:46:38.000000 bioregistry-0.9.3/tests/test_duplicates.py
--rw-r--r--   0 runner    (1001) docker     (123)     6904 2023-05-03 00:46:38.000000 bioregistry-0.9.3/tests/test_identifiers_org.py
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-05-03 00:46:38.000000 bioregistry-0.9.3/tests/test_indra.py
--rw-r--r--   0 runner    (1001) docker     (123)     9604 2023-05-03 00:46:38.000000 bioregistry-0.9.3/tests/test_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     7039 2023-05-03 00:46:38.000000 bioregistry-0.9.3/tests/test_metaregistry.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-03 00:46:38.000000 bioregistry-0.9.3/tests/test_obofoundry.py
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-03 00:46:38.000000 bioregistry-0.9.3/tests/test_ols.py
--rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-05-03 00:46:38.000000 bioregistry-0.9.3/tests/test_pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     6658 2023-05-03 00:46:38.000000 bioregistry-0.9.3/tests/test_resolve.py
--rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-05-03 00:46:38.000000 bioregistry-0.9.3/tests/test_sparql.py
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-05-03 00:46:38.000000 bioregistry-0.9.3/tests/test_usages.py
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-05-03 00:46:38.000000 bioregistry-0.9.3/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 01:25:12.742037 bioregistry-0.9.3/tests/test_web/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-03 00:46:38.000000 bioregistry-0.9.3/tests/test_web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7947 2023-05-03 00:46:38.000000 bioregistry-0.9.3/tests/test_web/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7824 2023-05-03 00:46:38.000000 bioregistry-0.9.3/tests/test_web/test_ui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 01:23:46.695975 bioregistry-0.9.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-04 00:46:17.000000 bioregistry-0.9.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-04 00:46:17.000000 bioregistry-0.9.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    31510 2023-05-04 01:23:46.695975 bioregistry-0.9.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    30194 2023-05-04 00:46:17.000000 bioregistry-0.9.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 01:23:46.615974 bioregistry-0.9.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-05-04 00:46:17.000000 bioregistry-0.9.4/docs/bulk_prefix_request_template.tsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 01:23:46.619974 bioregistry-0.9.4/docs/img/
+-rw-r--r--   0 runner    (1001) docker     (123)    48331 2023-05-04 01:11:47.000000 bioregistry-0.9.4/docs/img/bibliography_years.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   156964 2023-05-04 01:12:04.000000 bioregistry-0.9.4/docs/img/bioregistry_coverage.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   107017 2023-05-04 01:12:03.000000 bioregistry-0.9.4/docs/img/bioregistry_coverage_bar.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    84693 2023-05-04 01:12:05.000000 bioregistry-0.9.4/docs/img/bioregistry_coverage_bar_short.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    77372 2023-05-04 00:46:17.000000 bioregistry-0.9.4/docs/img/datamodel_umls.svg
+-rw-r--r--   0 runner    (1001) docker     (123)  1382073 2023-05-04 01:15:28.000000 bioregistry-0.9.4/docs/img/external_overlap.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    72498 2023-05-04 01:12:27.000000 bioregistry-0.9.4/docs/img/has_attribute.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    28419 2023-05-04 01:15:29.000000 bioregistry-0.9.4/docs/img/providers.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    22303 2023-05-04 01:15:30.000000 bioregistry-0.9.4/docs/img/regex_report.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    51528 2023-05-04 01:12:03.000000 bioregistry-0.9.4/docs/img/xrefs.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 01:23:46.619974 bioregistry-0.9.4/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-04 00:46:17.000000 bioregistry-0.9.4/docs/source/alignment.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-04 00:46:17.000000 bioregistry-0.9.4/docs/source/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7033 2023-05-04 01:23:37.000000 bioregistry-0.9.4/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8480 2023-05-04 00:46:17.000000 bioregistry-0.9.4/docs/source/deployment.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-05-04 00:46:17.000000 bioregistry-0.9.4/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)   214468 2023-05-04 00:46:17.000000 bioregistry-0.9.4/docs/source/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-04 00:46:17.000000 bioregistry-0.9.4/docs/source/pandas.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-04 00:46:17.000000 bioregistry-0.9.4/docs/source/reference.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-04 00:46:17.000000 bioregistry-0.9.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-05-04 01:23:46.695975 bioregistry-0.9.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 01:23:46.611974 bioregistry-0.9.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 01:23:46.623974 bioregistry-0.9.4/src/bioregistry/
+-rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 01:23:46.627974 bioregistry-0.9.4/src/bioregistry/align/
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/align/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/align/aberowl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/align/bartoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/align/biocontext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/align/biolink.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/align/bioportal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/align/cellosaurus.py
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/align/cheminf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/align/cropoct.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/align/edam.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/align/fairsharing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2544 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/align/go.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/align/hl7.py
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/align/miriam.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/align/n2t.py
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/align/ncbi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/align/obofoundry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/align/ols.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/align/ontobee.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/align/prefixcommons.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/align/re3data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/align/uniprot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10718 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/align/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/align/wikidata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 01:23:46.627974 bioregistry-0.9.4/src/bioregistry/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5007 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/analysis/title_tfidf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 01:23:46.627974 bioregistry-0.9.4/src/bioregistry/app/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17624 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/app/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/app/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/app/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10179 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/app/impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/app/proxies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 01:23:46.627974 bioregistry-0.9.4/src/bioregistry/app/static/
+-rw-r--r--   0 runner    (1001) docker     (123)   801449 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/app/static/logo.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 01:23:46.631974 bioregistry-0.9.4/src/bioregistry/app/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     9662 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/app/templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/app/templates/collection.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/app/templates/collections.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6758 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/app/templates/context.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/app/templates/contexts.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7134 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/app/templates/contributor.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4670 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/app/templates/contributors.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 01:23:46.631974 bioregistry-0.9.4/src/bioregistry/app/templates/highlights/
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/app/templates/highlights/keywords.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/app/templates/highlights/owners.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/app/templates/highlights/relations.html
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/app/templates/highlights/twitter.html
+-rw-r--r--   0 runner    (1001) docker     (123)    15622 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/app/templates/home.html
+-rw-r--r--   0 runner    (1001) docker     (123)     7351 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/app/templates/macros.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 01:23:46.631974 bioregistry-0.9.4/src/bioregistry/app/templates/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)     5577 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/app/templates/meta/access.html
+-rw-r--r--   0 runner    (1001) docker     (123)    19835 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/app/templates/meta/acknowledgements.html
+-rw-r--r--   0 runner    (1001) docker     (123)    10695 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/app/templates/meta/download.html
+-rw-r--r--   0 runner    (1001) docker     (123)    16544 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/app/templates/meta/related.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/app/templates/meta/schema.html
+-rw-r--r--   0 runner    (1001) docker     (123)    19312 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/app/templates/meta/summary.html
+-rw-r--r--   0 runner    (1001) docker     (123)     8813 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/app/templates/meta/sustainability.html
+-rw-r--r--   0 runner    (1001) docker     (123)     8460 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/app/templates/metaresource.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2303 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/app/templates/metaresources.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/app/templates/prose.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2437 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/app/templates/reference.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 01:23:46.635974 bioregistry-0.9.4/src/bioregistry/app/templates/resolve_errors/
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/app/templates/resolve_errors/disallowed_identifier.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/app/templates/resolve_errors/invalid_identifier.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/app/templates/resolve_errors/missing_prefix.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/app/templates/resolve_errors/missing_providers.html
+-rw-r--r--   0 runner    (1001) docker     (123)    32484 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/app/templates/resource.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3765 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/app/templates/resources.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/app/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19423 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/app/ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8073 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/app/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/app/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 01:23:46.635974 bioregistry-0.9.4/src/bioregistry/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/benchmarks/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/benchmarks/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/benchmarks/curie_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/benchmarks/curie_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/benchmarks/uri_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/bibliometrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/collection_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23802 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5293 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 01:23:46.635974 bioregistry-0.9.4/src/bioregistry/curation/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/curation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/curation/add_co_providers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/curation/add_descriptions_from_gs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/curation/add_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/curation/add_examples_from_javert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2278 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/curation/add_examples_from_ols.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/curation/add_ontology_regexes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/curation/bulk_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/curation/clean_licenses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/curation/clean_name_suffixes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/curation/clean_publications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/curation/cleanup_authors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/curation/deprecation_diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4940 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/curation/enrich_publications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/curation/import_pc_semiautomatic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2774 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/curation/make_description_curation_sheet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/curation/map_bartoc_via_wikidata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/curation/map_re3data_via_fairsharing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/curation/rename_metaprefix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/curation/review_pc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/curation/suggest_author_curation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/curation/suggest_uniprot_providers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 01:23:46.643974 bioregistry-0.9.4/src/bioregistry/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/data/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  4590753 2023-05-04 01:10:07.000000 bioregistry-0.9.4/src/bioregistry/data/bioregistry.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11750 2023-05-04 01:10:07.000000 bioregistry-0.9.4/src/bioregistry/data/collections.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-04 01:10:07.000000 bioregistry-0.9.4/src/bioregistry/data/contexts.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 01:23:46.615974 bioregistry-0.9.4/src/bioregistry/data/external/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 01:23:46.643974 bioregistry-0.9.4/src/bioregistry/data/external/aberowl/
+-rw-r--r--   0 runner    (1001) docker     (123)   302925 2023-05-04 00:53:43.000000 bioregistry-0.9.4/src/bioregistry/data/external/aberowl/curation.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)   623701 2023-05-04 00:53:43.000000 bioregistry-0.9.4/src/bioregistry/data/external/aberowl/processed.json
+-rw-r--r--   0 runner    (1001) docker     (123)  1280745 2023-05-04 00:53:37.000000 bioregistry-0.9.4/src/bioregistry/data/external/aberowl/raw.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 01:23:46.647974 bioregistry-0.9.4/src/bioregistry/data/external/agroportal/
+-rw-r--r--   0 runner    (1001) docker     (123)    42168 2023-05-04 01:10:03.000000 bioregistry-0.9.4/src/bioregistry/data/external/agroportal/curation.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)   124136 2023-05-04 01:10:03.000000 bioregistry-0.9.4/src/bioregistry/data/external/agroportal/processed.json
+-rw-r--r--   0 runner    (1001) docker     (123)   663568 2023-05-04 01:10:03.000000 bioregistry-0.9.4/src/bioregistry/data/external/agroportal/raw.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 01:23:46.651975 bioregistry-0.9.4/src/bioregistry/data/external/bartoc/
+-rw-r--r--   0 runner    (1001) docker     (123)  1835101 2023-05-04 01:10:07.000000 bioregistry-0.9.4/src/bioregistry/data/external/bartoc/curation.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)  2216766 2023-05-04 01:10:07.000000 bioregistry-0.9.4/src/bioregistry/data/external/bartoc/processed.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 01:23:46.651975 bioregistry-0.9.4/src/bioregistry/data/external/biocontext/
+-rw-r--r--   0 runner    (1001) docker     (123)     5057 2023-05-04 01:08:10.000000 bioregistry-0.9.4/src/bioregistry/data/external/biocontext/curation.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)    74913 2023-05-04 01:08:09.000000 bioregistry-0.9.4/src/bioregistry/data/external/biocontext/processed.json
+-rw-r--r--   0 runner    (1001) docker     (123)    55878 2023-05-04 01:08:09.000000 bioregistry-0.9.4/src/bioregistry/data/external/biocontext/raw.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 01:23:46.655974 bioregistry-0.9.4/src/bioregistry/data/external/biolink/
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-05-04 01:08:16.000000 bioregistry-0.9.4/src/bioregistry/data/external/biolink/curation.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)    10406 2023-05-04 01:08:16.000000 bioregistry-0.9.4/src/bioregistry/data/external/biolink/processed.json
+-rw-r--r--   0 runner    (1001) docker     (123)   354352 2023-05-04 01:08:15.000000 bioregistry-0.9.4/src/bioregistry/data/external/biolink/raw.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 01:23:46.655974 bioregistry-0.9.4/src/bioregistry/data/external/bioportal/
+-rw-r--r--   0 runner    (1001) docker     (123)   253653 2023-05-04 01:08:05.000000 bioregistry-0.9.4/src/bioregistry/data/external/bioportal/curation.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)   606721 2023-05-04 01:08:04.000000 bioregistry-0.9.4/src/bioregistry/data/external/bioportal/processed.json
+-rw-r--r--   0 runner    (1001) docker     (123)  3539138 2023-05-04 01:08:04.000000 bioregistry-0.9.4/src/bioregistry/data/external/bioportal/raw.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 01:23:46.659974 bioregistry-0.9.4/src/bioregistry/data/external/cellosaurus/
+-rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-05-04 00:59:34.000000 bioregistry-0.9.4/src/bioregistry/data/external/cellosaurus/curation.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)    28730 2023-05-04 00:59:33.000000 bioregistry-0.9.4/src/bioregistry/data/external/cellosaurus/processed.json
+-rw-r--r--   0 runner    (1001) docker     (123)    32374 2023-05-04 00:59:33.000000 bioregistry-0.9.4/src/bioregistry/data/external/cellosaurus/raw.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 01:23:46.659974 bioregistry-0.9.4/src/bioregistry/data/external/cheminf/
+-rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-05-04 01:08:48.000000 bioregistry-0.9.4/src/bioregistry/data/external/cheminf/processed.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 01:23:46.659974 bioregistry-0.9.4/src/bioregistry/data/external/cropoct/
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-05-04 00:59:41.000000 bioregistry-0.9.4/src/bioregistry/data/external/cropoct/curation.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)    11407 2023-05-04 00:59:41.000000 bioregistry-0.9.4/src/bioregistry/data/external/cropoct/processed.json
+-rw-r--r--   0 runner    (1001) docker     (123)    25353 2023-05-04 00:59:41.000000 bioregistry-0.9.4/src/bioregistry/data/external/cropoct/raw.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 01:23:46.659974 bioregistry-0.9.4/src/bioregistry/data/external/ecoportal/
+-rw-r--r--   0 runner    (1001) docker     (123)     9198 2023-05-04 01:08:30.000000 bioregistry-0.9.4/src/bioregistry/data/external/ecoportal/curation.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)    18773 2023-05-04 01:08:29.000000 bioregistry-0.9.4/src/bioregistry/data/external/ecoportal/processed.json
+-rw-r--r--   0 runner    (1001) docker     (123)    98149 2023-05-04 01:08:29.000000 bioregistry-0.9.4/src/bioregistry/data/external/ecoportal/raw.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 01:23:46.663975 bioregistry-0.9.4/src/bioregistry/data/external/edam/
+-rw-r--r--   0 runner    (1001) docker     (123)    14599 2023-05-04 01:08:46.000000 bioregistry-0.9.4/src/bioregistry/data/external/edam/curation.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)    45616 2023-05-04 01:08:46.000000 bioregistry-0.9.4/src/bioregistry/data/external/edam/processed.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 01:23:46.663975 bioregistry-0.9.4/src/bioregistry/data/external/fairsharing/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/data/external/fairsharing/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)   253879 2023-05-04 00:59:28.000000 bioregistry-0.9.4/src/bioregistry/data/external/fairsharing/curation.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)   745109 2023-05-04 00:59:27.000000 bioregistry-0.9.4/src/bioregistry/data/external/fairsharing/processed.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 01:23:46.663975 bioregistry-0.9.4/src/bioregistry/data/external/go/
+-rw-r--r--   0 runner    (1001) docker     (123)     7502 2023-05-04 01:08:39.000000 bioregistry-0.9.4/src/bioregistry/data/external/go/curation.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)   143024 2023-05-04 01:08:39.000000 bioregistry-0.9.4/src/bioregistry/data/external/go/processed.json
+-rw-r--r--   0 runner    (1001) docker     (123)   115035 2023-05-04 01:08:38.000000 bioregistry-0.9.4/src/bioregistry/data/external/go/raw.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 01:23:46.663975 bioregistry-0.9.4/src/bioregistry/data/external/hl7/
+-rw-r--r--   0 runner    (1001) docker     (123)   157660 2023-05-04 00:59:36.000000 bioregistry-0.9.4/src/bioregistry/data/external/hl7/curation.tsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 01:23:46.667975 bioregistry-0.9.4/src/bioregistry/data/external/miriam/
+-rw-r--r--   0 runner    (1001) docker     (123)   576520 2023-05-04 01:08:13.000000 bioregistry-0.9.4/src/bioregistry/data/external/miriam/processed.json
+-rw-r--r--   0 runner    (1001) docker     (123)  1987182 2023-05-04 01:08:13.000000 bioregistry-0.9.4/src/bioregistry/data/external/miriam/raw.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 01:23:46.667975 bioregistry-0.9.4/src/bioregistry/data/external/n2t/
+-rw-r--r--   0 runner    (1001) docker     (123)   425371 2023-05-04 00:59:48.000000 bioregistry-0.9.4/src/bioregistry/data/external/n2t/processed.json
+-rw-r--r--   0 runner    (1001) docker     (123)  1278934 2023-05-04 00:59:44.000000 bioregistry-0.9.4/src/bioregistry/data/external/n2t/raw.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 01:23:46.671975 bioregistry-0.9.4/src/bioregistry/data/external/ncbi/
+-rw-r--r--   0 runner    (1001) docker     (123)     3748 2023-05-04 00:59:38.000000 bioregistry-0.9.4/src/bioregistry/data/external/ncbi/curation.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)    18072 2023-05-04 00:59:38.000000 bioregistry-0.9.4/src/bioregistry/data/external/ncbi/processed.json
+-rw-r--r--   0 runner    (1001) docker     (123)   103465 2023-05-04 00:59:38.000000 bioregistry-0.9.4/src/bioregistry/data/external/ncbi/raw.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 01:23:46.671975 bioregistry-0.9.4/src/bioregistry/data/external/obofoundry/
+-rw-r--r--   0 runner    (1001) docker     (123)   212323 2023-05-04 01:08:52.000000 bioregistry-0.9.4/src/bioregistry/data/external/obofoundry/processed.json
+-rw-r--r--   0 runner    (1001) docker     (123)   350196 2023-05-04 01:08:51.000000 bioregistry-0.9.4/src/bioregistry/data/external/obofoundry/raw.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 01:23:46.671975 bioregistry-0.9.4/src/bioregistry/data/external/ols/
+-rw-r--r--   0 runner    (1001) docker     (123)   141937 2023-05-04 00:53:30.000000 bioregistry-0.9.4/src/bioregistry/data/external/ols/processed.json
+-rw-r--r--   0 runner    (1001) docker     (123)   805618 2023-05-04 00:53:30.000000 bioregistry-0.9.4/src/bioregistry/data/external/ols/raw.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 01:23:46.675975 bioregistry-0.9.4/src/bioregistry/data/external/ontobee/
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-05-04 01:08:42.000000 bioregistry-0.9.4/src/bioregistry/data/external/ontobee/curation.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)    23684 2023-05-04 01:08:42.000000 bioregistry-0.9.4/src/bioregistry/data/external/ontobee/processed.json
+-rw-r--r--   0 runner    (1001) docker     (123)   192177 2023-05-04 01:08:41.000000 bioregistry-0.9.4/src/bioregistry/data/external/ontobee/raw.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 01:23:46.675975 bioregistry-0.9.4/src/bioregistry/data/external/prefixcommons/
+-rw-r--r--   0 runner    (1001) docker     (123)   111600 2023-05-04 00:59:31.000000 bioregistry-0.9.4/src/bioregistry/data/external/prefixcommons/curation.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)   505834 2023-05-04 00:59:31.000000 bioregistry-0.9.4/src/bioregistry/data/external/prefixcommons/processed.json
+-rw-r--r--   0 runner    (1001) docker     (123)   883990 2023-05-04 00:59:30.000000 bioregistry-0.9.4/src/bioregistry/data/external/prefixcommons/raw.tsv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 01:23:46.679975 bioregistry-0.9.4/src/bioregistry/data/external/re3data/
+-rw-r--r--   0 runner    (1001) docker     (123)  1742450 2023-05-04 00:53:26.000000 bioregistry-0.9.4/src/bioregistry/data/external/re3data/curation.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)  2438947 2023-05-04 00:53:26.000000 bioregistry-0.9.4/src/bioregistry/data/external/re3data/processed.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 01:23:46.679975 bioregistry-0.9.4/src/bioregistry/data/external/uniprot/
+-rw-r--r--   0 runner    (1001) docker     (123)    10765 2023-05-04 01:08:07.000000 bioregistry-0.9.4/src/bioregistry/data/external/uniprot/curation.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)    67268 2023-05-04 01:08:07.000000 bioregistry-0.9.4/src/bioregistry/data/external/uniprot/processed.json
+-rw-r--r--   0 runner    (1001) docker     (123)    89621 2023-05-04 01:08:07.000000 bioregistry-0.9.4/src/bioregistry/data/external/uniprot/raw.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 01:23:46.683975 bioregistry-0.9.4/src/bioregistry/data/external/wikidata/
+-rw-r--r--   0 runner    (1001) docker     (123)   125505 2023-05-04 01:08:37.000000 bioregistry-0.9.4/src/bioregistry/data/external/wikidata/curation.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)   319146 2023-05-04 01:08:36.000000 bioregistry-0.9.4/src/bioregistry/data/external/wikidata/processed.json
+-rw-r--r--   0 runner    (1001) docker     (123)    47301 2023-05-04 01:10:07.000000 bioregistry-0.9.4/src/bioregistry/data/metaregistry.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-05-04 01:10:07.000000 bioregistry-0.9.4/src/bioregistry/data/mismatch.json
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/data/processing_biolink.json
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/data/processing_go.json
+-rw-r--r--   0 runner    (1001) docker     (123)    29821 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/data/processing_ols.json
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/data/processing_wikidata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 01:23:46.683975 bioregistry-0.9.4/src/bioregistry/export/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/export/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/export/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/export/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4489 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/export/prefix_maps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8861 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/export/rdf_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/export/schema_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3434 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/export/sssom_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8994 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/export/tables_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/export/tsv_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4617 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/export/warnings_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/export/yaml_export.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 01:23:46.687975 bioregistry-0.9.4/src/bioregistry/external/
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/external/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/external/aberowl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/external/bartoc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/external/biocontext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/external/biolink.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6997 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/external/bioportal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/external/cellosaurus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/external/cheminf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/external/cropoct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/external/edam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3385 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/external/fairsharing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/external/go.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 01:23:46.687975 bioregistry-0.9.4/src/bioregistry/external/hl7/
+-rw-r--r--   0 runner    (1001) docker     (123)   319976 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/external/hl7/OID_Report.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/external/hl7/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/external/miriam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2175 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/external/n2t.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4839 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/external/ncbi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/external/obofoundry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7610 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/external/ols.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/external/ontobee.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4154 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/external/prefixcommons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6191 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/external/re3data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/external/uniprot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7988 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/external/wikidata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 01:23:46.691975 bioregistry-0.9.4/src/bioregistry/gh/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/gh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8350 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/gh/github_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9789 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/gh/new_prefix.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 01:23:46.691975 bioregistry-0.9.4/src/bioregistry/health/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/health/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/health/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/health/check_homepages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7053 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/health/check_providers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/health/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8571 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/license_standardizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/lint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/metaresource_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18936 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/parse_iri.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    13281 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/record_accumulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33164 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/resolve.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17532 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/resolve_identifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63936 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/resource_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 01:23:46.691975 bioregistry-0.9.4/src/bioregistry/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13218 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/schema/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42222 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/schema/schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)   106399 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/schema/struct.py
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/schema/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8188 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/schema_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10183 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5517 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/upload_ndex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7175 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/uri_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8067 2023-05-04 00:46:17.000000 bioregistry-0.9.4/src/bioregistry/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-04 01:23:37.000000 bioregistry-0.9.4/src/bioregistry/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 01:23:46.623974 bioregistry-0.9.4/src/bioregistry.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    31510 2023-05-04 01:23:46.000000 bioregistry-0.9.4/src/bioregistry.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11234 2023-05-04 01:23:46.000000 bioregistry-0.9.4/src/bioregistry.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 01:23:46.000000 bioregistry-0.9.4/src/bioregistry.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-04 01:23:46.000000 bioregistry-0.9.4/src/bioregistry.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 00:46:27.000000 bioregistry-0.9.4/src/bioregistry.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-05-04 01:23:46.000000 bioregistry-0.9.4/src/bioregistry.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-04 01:23:46.000000 bioregistry-0.9.4/src/bioregistry.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 01:23:46.695975 bioregistry-0.9.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-04 00:46:17.000000 bioregistry-0.9.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-05-04 00:46:17.000000 bioregistry-0.9.4/tests/test_acquisition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-05-04 00:46:17.000000 bioregistry-0.9.4/tests/test_collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5177 2023-05-04 00:46:17.000000 bioregistry-0.9.4/tests/test_contexts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46880 2023-05-04 00:46:17.000000 bioregistry-0.9.4/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-05-04 00:46:17.000000 bioregistry-0.9.4/tests/test_duplicates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6904 2023-05-04 00:46:17.000000 bioregistry-0.9.4/tests/test_identifiers_org.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-05-04 00:46:17.000000 bioregistry-0.9.4/tests/test_indra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9604 2023-05-04 00:46:17.000000 bioregistry-0.9.4/tests/test_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7039 2023-05-04 00:46:17.000000 bioregistry-0.9.4/tests/test_metaregistry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-04 00:46:17.000000 bioregistry-0.9.4/tests/test_obofoundry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-04 00:46:17.000000 bioregistry-0.9.4/tests/test_ols.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-05-04 00:46:17.000000 bioregistry-0.9.4/tests/test_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6658 2023-05-04 00:46:17.000000 bioregistry-0.9.4/tests/test_resolve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-05-04 00:46:17.000000 bioregistry-0.9.4/tests/test_sparql.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-05-04 00:46:17.000000 bioregistry-0.9.4/tests/test_usages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-05-04 00:46:17.000000 bioregistry-0.9.4/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 01:23:46.695975 bioregistry-0.9.4/tests/test_web/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-04 00:46:17.000000 bioregistry-0.9.4/tests/test_web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7947 2023-05-04 00:46:17.000000 bioregistry-0.9.4/tests/test_web/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7824 2023-05-04 00:46:17.000000 bioregistry-0.9.4/tests/test_web/test_ui.py
```

### Comparing `bioregistry-0.9.3/LICENSE` & `bioregistry-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/MANIFEST.in` & `bioregistry-0.9.4/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/PKG-INFO` & `bioregistry-0.9.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bioregistry
-Version: 0.9.3
+Version: 0.9.4
 Summary: Integrated registry of biological databases and nomenclatures
 Home-page: https://github.com/biopragmatics/bioregistry
 Download-URL: https://github.com/biopragmatics/bioregistry/releases
 Author: Charles Tapley Hoyt
 Author-email: cthoyt@gmail.com
 Maintainer: Charles Tapley Hoyt
 Maintainer-email: cthoyt@gmail.com
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: bioregistry Version: 0.9.3 Summary: Integrated
+Metadata-Version: 2.1 Name: bioregistry Version: 0.9.4 Summary: Integrated
 registry of biological databases and nomenclatures Home-page: https://
 github.com/biopragmatics/bioregistry Download-URL: https://github.com/
 biopragmatics/bioregistry/releases Author: Charles Tapley Hoyt Author-email:
 cthoyt@gmail.com Maintainer: Charles Tapley Hoyt Maintainer-email:
 cthoyt@gmail.com License: MIT Project-URL: Bug Tracker, https://github.com/
 biopragmatics/bioregistry/issues Keywords: databases,biological
 databases,biomedical databases Classifier: Development Status :: 4 - Beta
```

### Comparing `bioregistry-0.9.3/README.md` & `bioregistry-0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/docs/bulk_prefix_request_template.tsv` & `bioregistry-0.9.4/docs/bulk_prefix_request_template.tsv`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/docs/img/bibliography_years.svg` & `bioregistry-0.9.4/docs/img/bibliography_years.svg`

 * *Files 11% similar despite different names*

```diff
@@ -29,16 +29,16 @@
 000001c0: 3032 2f32 322d 7264 662d 7379 6e74 6178  02/22-rdf-syntax
 000001d0: 2d6e 7323 223e 0a20 2020 3c63 633a 576f  -ns#">.   <cc:Wo
 000001e0: 726b 3e0a 2020 2020 3c64 633a 7479 7065  rk>.    <dc:type
 000001f0: 2072 6466 3a72 6573 6f75 7263 653d 2268   rdf:resource="h
 00000200: 7474 703a 2f2f 7075 726c 2e6f 7267 2f64  ttp://purl.org/d
 00000210: 632f 6463 6d69 7479 7065 2f53 7469 6c6c  c/dcmitype/Still
 00000220: 496d 6167 6522 2f3e 0a20 2020 203c 6463  Image"/>.    <dc
-00000230: 3a64 6174 653e 3230 3233 2d30 352d 3033  :date>2023-05-03
-00000240: 5430 313a 3132 3a30 312e 3830 3738 3332  T01:12:01.807832
+00000230: 3a64 6174 653e 3230 3233 2d30 352d 3034  :date>2023-05-04
+00000240: 5430 313a 3131 3a34 372e 3733 3535 3432  T01:11:47.735542
 00000250: 3c2f 6463 3a64 6174 653e 0a20 2020 203c  </dc:date>.    <
 00000260: 6463 3a66 6f72 6d61 743e 696d 6167 652f  dc:format>image/
 00000270: 7376 672b 786d 6c3c 2f64 633a 666f 726d  svg+xml</dc:form
 00000280: 6174 3e0a 2020 2020 3c64 633a 6372 6561  at>.    <dc:crea
 00000290: 746f 723e 0a20 2020 2020 3c63 633a 4167  tor>.     <cc:Ag
 000002a0: 656e 743e 0a20 2020 2020 203c 6463 3a74  ent>.      <dc:t
 000002b0: 6974 6c65 3e4d 6174 706c 6f74 6c69 6220  itle>Matplotlib 
@@ -78,392 +78,392 @@
 000004d0: 3c70 6174 6820 643d 224d 2034 362e 3238  <path d="M 46.28
 000004e0: 3836 3535 2032 3038 2e39 3938 3731 3420  8655 208.998714 
 000004f0: 0a4c 2036 302e 3033 3738 3939 2032 3038  .L 60.037899 208
 00000500: 2e39 3938 3731 3420 0a4c 2036 302e 3033  .998714 .L 60.03
 00000510: 3738 3939 2032 3038 2e39 3938 3731 3420  7899 208.998714 
 00000520: 0a4c 2034 362e 3238 3836 3535 2032 3038  .L 46.288655 208
 00000530: 2e39 3938 3731 3420 0a7a 0a22 2063 6c69  .998714 .z." cli
-00000540: 702d 7061 7468 3d22 7572 6c28 2370 6132  p-path="url(#pa2
-00000550: 3766 3363 3536 3361 2922 2073 7479 6c65  7f3c563a)" style
+00000540: 702d 7061 7468 3d22 7572 6c28 2370 3033  p-path="url(#p03
+00000550: 6539 3338 3966 3838 2922 2073 7479 6c65  e9389f88)" style
 00000560: 3d22 6669 6c6c 3a20 2365 6139 3661 3322  ="fill: #ea96a3"
 00000570: 2f3e 0a20 2020 3c2f 673e 0a20 2020 3c67  />.   </g>.   <g
 00000580: 2069 643d 2270 6174 6368 5f34 223e 0a20   id="patch_4">. 
 00000590: 2020 203c 7061 7468 2064 3d22 4d20 3633     <path d="M 63
 000005a0: 2e34 3735 3231 2032 3038 2e39 3938 3731  .47521 208.99871
 000005b0: 3420 0a4c 2037 372e 3232 3434 3534 2032  4 .L 77.224454 2
 000005c0: 3038 2e39 3938 3731 3420 0a4c 2037 372e  08.998714 .L 77.
 000005d0: 3232 3434 3534 2032 3033 2e38 3937 3335  224454 203.89735
 000005e0: 200a 4c20 3633 2e34 3735 3231 2032 3033   .L 63.47521 203
 000005f0: 2e38 3937 3335 200a 7a0a 2220 636c 6970  .89735 .z." clip
-00000600: 2d70 6174 683d 2275 726c 2823 7061 3237  -path="url(#pa27
-00000610: 6633 6335 3633 6129 2220 7374 796c 653d  f3c563a)" style=
+00000600: 2d70 6174 683d 2275 726c 2823 7030 3365  -path="url(#p03e
+00000610: 3933 3839 6638 3829 2220 7374 796c 653d  9389f88)" style=
 00000620: 2266 696c 6c3a 2023 6539 3937 3931 222f  "fill: #e99791"/
 00000630: 3e0a 2020 203c 2f67 3e0a 2020 203c 6720  >.   </g>.   <g 
 00000640: 6964 3d22 7061 7463 685f 3522 3e0a 2020  id="patch_5">.  
 00000650: 2020 3c70 6174 6820 643d 224d 2038 302e    <path d="M 80.
 00000660: 3636 3137 3635 2032 3038 2e39 3938 3731  661765 208.99871
 00000670: 3420 0a4c 2039 342e 3431 3130 3038 2032  4 .L 94.411008 2
 00000680: 3038 2e39 3938 3731 3420 0a4c 2039 342e  08.998714 .L 94.
 00000690: 3431 3130 3038 2031 3938 2e37 3935 3938  411008 198.79598
 000006a0: 3520 0a4c 2038 302e 3636 3137 3635 2031  5 .L 80.661765 1
 000006b0: 3938 2e37 3935 3938 3520 0a7a 0a22 2063  98.795985 .z." c
 000006c0: 6c69 702d 7061 7468 3d22 7572 6c28 2370  lip-path="url(#p
-000006d0: 6132 3766 3363 3536 3361 2922 2073 7479  a27f3c563a)" sty
+000006d0: 3033 6539 3338 3966 3838 2922 2073 7479  03e9389f88)" sty
 000006e0: 6c65 3d22 6669 6c6c 3a20 2365 3539 3437  le="fill: #e5947
 000006f0: 3122 2f3e 0a20 2020 3c2f 673e 0a20 2020  1"/>.   </g>.   
 00000700: 3c67 2069 643d 2270 6174 6368 5f36 223e  <g id="patch_6">
 00000710: 0a20 2020 203c 7061 7468 2064 3d22 4d20  .    <path d="M 
 00000720: 3937 2e38 3438 3331 3920 3230 382e 3939  97.848319 208.99
 00000730: 3837 3134 200a 4c20 3131 312e 3539 3735  8714 .L 111.5975
 00000740: 3633 2032 3038 2e39 3938 3731 3420 0a4c  63 208.998714 .L
 00000750: 2031 3131 2e35 3937 3536 3320 3137 382e   111.597563 178.
 00000760: 3339 3035 3237 200a 4c20 3937 2e38 3438  390527 .L 97.848
 00000770: 3331 3920 3137 382e 3339 3035 3237 200a  319 178.390527 .
 00000780: 7a0a 2220 636c 6970 2d70 6174 683d 2275  z." clip-path="u
-00000790: 726c 2823 7061 3237 6633 6335 3633 6129  rl(#pa27f3c563a)
+00000790: 726c 2823 7030 3365 3933 3839 6638 3829  rl(#p03e9389f88)
 000007a0: 2220 7374 796c 653d 2266 696c 6c3a 2023  " style="fill: #
 000007b0: 6437 3934 3465 222f 3e0a 2020 203c 2f67  d7944e"/>.   </g
 000007c0: 3e0a 2020 203c 6720 6964 3d22 7061 7463  >.   <g id="patc
 000007d0: 685f 3722 3e0a 2020 2020 3c70 6174 6820  h_7">.    <path 
 000007e0: 643d 224d 2031 3135 2e30 3334 3837 3420  d="M 115.034874 
 000007f0: 3230 382e 3939 3837 3134 200a 4c20 3132  208.998714 .L 12
 00000800: 382e 3738 3431 3137 2032 3038 2e39 3938  8.784117 208.998
 00000810: 3731 3420 0a4c 2031 3238 2e37 3834 3131  714 .L 128.78411
 00000820: 3720 3138 382e 3539 3332 3536 200a 4c20  7 188.593256 .L 
 00000830: 3131 352e 3033 3438 3734 2031 3838 2e35  115.034874 188.5
 00000840: 3933 3235 3620 0a7a 0a22 2063 6c69 702d  93256 .z." clip-
-00000850: 7061 7468 3d22 7572 6c28 2370 6132 3766  path="url(#pa27f
-00000860: 3363 3536 3361 2922 2073 7479 6c65 3d22  3c563a)" style="
+00000850: 7061 7468 3d22 7572 6c28 2370 3033 6539  path="url(#p03e9
+00000860: 3338 3966 3838 2922 2073 7479 6c65 3d22  389f88)" style="
 00000870: 6669 6c6c 3a20 2363 3639 3934 6222 2f3e  fill: #c6994b"/>
 00000880: 0a20 2020 3c2f 673e 0a20 2020 3c67 2069  .   </g>.   <g i
 00000890: 643d 2270 6174 6368 5f38 223e 0a20 2020  d="patch_8">.   
 000008a0: 203c 7061 7468 2064 3d22 4d20 3133 322e   <path d="M 132.
 000008b0: 3232 3134 3238 2032 3038 2e39 3938 3731  221428 208.99871
 000008c0: 3420 0a4c 2031 3435 2e39 3730 3637 3220  4 .L 145.970672 
 000008d0: 3230 382e 3939 3837 3134 200a 4c20 3134  208.998714 .L 14
 000008e0: 352e 3937 3036 3732 2031 3733 2e32 3839  5.970672 173.289
 000008f0: 3136 3220 0a4c 2031 3332 2e32 3231 3432  162 .L 132.22142
 00000900: 3820 3137 332e 3238 3931 3632 200a 7a0a  8 173.289162 .z.
 00000910: 2220 636c 6970 2d70 6174 683d 2275 726c  " clip-path="url
-00000920: 2823 7061 3237 6633 6335 3633 6129 2220  (#pa27f3c563a)" 
+00000920: 2823 7030 3365 3933 3839 6638 3829 2220  (#p03e9389f88)" 
 00000930: 7374 796c 653d 2266 696c 6c3a 2023 6238  style="fill: #b8
 00000940: 3963 3439 222f 3e0a 2020 203c 2f67 3e0a  9c49"/>.   </g>.
 00000950: 2020 203c 6720 6964 3d22 7061 7463 685f     <g id="patch_
 00000960: 3922 3e0a 2020 2020 3c70 6174 6820 643d  9">.    <path d=
 00000970: 224d 2031 3439 2e34 3037 3938 3320 3230  "M 149.407983 20
 00000980: 382e 3939 3837 3134 200a 4c20 3136 332e  8.998714 .L 163.
 00000990: 3135 3732 3236 2032 3038 2e39 3938 3731  157226 208.99871
 000009a0: 3420 0a4c 2031 3633 2e31 3537 3232 3620  4 .L 163.157226 
 000009b0: 3135 372e 3938 3530 3639 200a 4c20 3134  157.985069 .L 14
 000009c0: 392e 3430 3739 3833 2031 3537 2e39 3835  9.407983 157.985
 000009d0: 3036 3920 0a7a 0a22 2063 6c69 702d 7061  069 .z." clip-pa
-000009e0: 7468 3d22 7572 6c28 2370 6132 3766 3363  th="url(#pa27f3c
-000009f0: 3536 3361 2922 2073 7479 6c65 3d22 6669  563a)" style="fi
+000009e0: 7468 3d22 7572 6c28 2370 3033 6539 3338  th="url(#p03e938
+000009f0: 3966 3838 2922 2073 7479 6c65 3d22 6669  9f88)" style="fi
 00000a00: 6c6c 3a20 2361 6239 6534 3722 2f3e 0a20  ll: #ab9e47"/>. 
 00000a10: 2020 3c2f 673e 0a20 2020 3c67 2069 643d    </g>.   <g id=
 00000a20: 2270 6174 6368 5f31 3022 3e0a 2020 2020  "patch_10">.    
 00000a30: 3c70 6174 6820 643d 224d 2031 3636 2e35  <path d="M 166.5
 00000a40: 3934 3533 3720 3230 382e 3939 3837 3134  94537 208.998714
 00000a50: 200a 4c20 3138 302e 3334 3337 3831 2032   .L 180.343781 2
 00000a60: 3038 2e39 3938 3731 3420 0a4c 2031 3830  08.998714 .L 180
 00000a70: 2e33 3433 3738 3120 3138 332e 3439 3138  .343781 183.4918
 00000a80: 3932 200a 4c20 3136 362e 3539 3435 3337  92 .L 166.594537
 00000a90: 2031 3833 2e34 3931 3839 3220 0a7a 0a22   183.491892 .z."
 00000aa0: 2063 6c69 702d 7061 7468 3d22 7572 6c28   clip-path="url(
-00000ab0: 2370 6132 3766 3363 3536 3361 2922 2073  #pa27f3c563a)" s
+00000ab0: 2370 3033 6539 3338 3966 3838 2922 2073  #p03e9389f88)" s
 00000ac0: 7479 6c65 3d22 6669 6c6c 3a20 2339 6561  tyle="fill: #9ea
 00000ad0: 3034 3522 2f3e 0a20 2020 3c2f 673e 0a20  045"/>.   </g>. 
 00000ae0: 2020 3c67 2069 643d 2270 6174 6368 5f31    <g id="patch_1
 00000af0: 3122 3e0a 2020 2020 3c70 6174 6820 643d  1">.    <path d=
 00000b00: 224d 2031 3833 2e37 3831 3039 3220 3230  "M 183.781092 20
 00000b10: 382e 3939 3837 3134 200a 4c20 3139 372e  8.998714 .L 197.
 00000b20: 3533 3033 3335 2032 3038 2e39 3938 3731  530335 208.99871
 00000b30: 3420 0a4c 2031 3937 2e35 3330 3333 3520  4 .L 197.530335 
 00000b40: 3133 372e 3537 3936 3131 200a 4c20 3138  137.579611 .L 18
 00000b50: 332e 3738 3130 3932 2031 3337 2e35 3739  3.781092 137.579
 00000b60: 3631 3120 0a7a 0a22 2063 6c69 702d 7061  611 .z." clip-pa
-00000b70: 7468 3d22 7572 6c28 2370 6132 3766 3363  th="url(#pa27f3c
-00000b80: 3536 3361 2922 2073 7479 6c65 3d22 6669  563a)" style="fi
+00000b70: 7468 3d22 7572 6c28 2370 3033 6539 3338  th="url(#p03e938
+00000b80: 3966 3838 2922 2073 7479 6c65 3d22 6669  9f88)" style="fi
 00000b90: 6c6c 3a20 2339 3161 3434 3622 2f3e 0a20  ll: #91a446"/>. 
 00000ba0: 2020 3c2f 673e 0a20 2020 3c67 2069 643d    </g>.   <g id=
 00000bb0: 2270 6174 6368 5f31 3222 3e0a 2020 2020  "patch_12">.    
 00000bc0: 3c70 6174 6820 643d 224d 2032 3030 2e39  <path d="M 200.9
 00000bd0: 3637 3634 3620 3230 382e 3939 3837 3134  67646 208.998714
 00000be0: 200a 4c20 3231 342e 3731 3638 3920 3230   .L 214.71689 20
 00000bf0: 382e 3939 3837 3134 200a 4c20 3231 342e  8.998714 .L 214.
 00000c00: 3731 3638 3920 3133 322e 3437 3832 3436  71689 132.478246
 00000c10: 200a 4c20 3230 302e 3936 3736 3436 2031   .L 200.967646 1
 00000c20: 3332 2e34 3738 3234 3620 0a7a 0a22 2063  32.478246 .z." c
 00000c30: 6c69 702d 7061 7468 3d22 7572 6c28 2370  lip-path="url(#p
-00000c40: 6132 3766 3363 3536 3361 2922 2073 7479  a27f3c563a)" sty
+00000c40: 3033 6539 3338 3966 3838 2922 2073 7479  03e9389f88)" sty
 00000c50: 6c65 3d22 6669 6c6c 3a20 2337 6661 3934  le="fill: #7fa94
 00000c60: 3622 2f3e 0a20 2020 3c2f 673e 0a20 2020  6"/>.   </g>.   
 00000c70: 3c67 2069 643d 2270 6174 6368 5f31 3322  <g id="patch_13"
 00000c80: 3e0a 2020 2020 3c70 6174 6820 643d 224d  >.    <path d="M
 00000c90: 2032 3138 2e31 3534 3230 3120 3230 382e   218.154201 208.
 00000ca0: 3939 3837 3134 200a 4c20 3233 312e 3930  998714 .L 231.90
 00000cb0: 3334 3435 2032 3038 2e39 3938 3731 3420  3445 208.998714 
 00000cc0: 0a4c 2032 3331 2e39 3033 3434 3520 3335  .L 231.903445 35
 00000cd0: 2e35 3532 3332 200a 4c20 3231 382e 3135  .55232 .L 218.15
 00000ce0: 3432 3031 2033 352e 3535 3233 3220 0a7a  4201 35.55232 .z
 00000cf0: 0a22 2063 6c69 702d 7061 7468 3d22 7572  ." clip-path="ur
-00000d00: 6c28 2370 6132 3766 3363 3536 3361 2922  l(#pa27f3c563a)"
+00000d00: 6c28 2370 3033 6539 3338 3966 3838 2922  l(#p03e9389f88)"
 00000d10: 2073 7479 6c65 3d22 6669 6c6c 3a20 2336   style="fill: #6
 00000d20: 3061 6534 3722 2f3e 0a20 2020 3c2f 673e  0ae47"/>.   </g>
 00000d30: 0a20 2020 3c67 2069 643d 2270 6174 6368  .   <g id="patch
 00000d40: 5f31 3422 3e0a 2020 2020 3c70 6174 6820  _14">.    <path 
 00000d50: 643d 224d 2032 3335 2e33 3430 3735 3520  d="M 235.340755 
 00000d60: 3230 382e 3939 3837 3134 200a 4c20 3234  208.998714 .L 24
 00000d70: 392e 3038 3939 3939 2032 3038 2e39 3938  9.089999 208.998
 00000d80: 3731 3420 0a4c 2032 3439 2e30 3839 3939  714 .L 249.08999
 00000d90: 3920 3831 2e34 3634 3630 3120 0a4c 2032  9 81.464601 .L 2
 00000da0: 3335 2e33 3430 3735 3520 3831 2e34 3634  35.340755 81.464
 00000db0: 3630 3120 0a7a 0a22 2063 6c69 702d 7061  601 .z." clip-pa
-00000dc0: 7468 3d22 7572 6c28 2370 6132 3766 3363  th="url(#pa27f3c
-00000dd0: 3536 3361 2922 2073 7479 6c65 3d22 6669  563a)" style="fi
+00000dc0: 7468 3d22 7572 6c28 2370 3033 6539 3338  th="url(#p03e938
+00000dd0: 3966 3838 2922 2073 7479 6c65 3d22 6669  9f88)" style="fi
 00000de0: 6c6c 3a20 2334 3862 3036 6122 2f3e 0a20  ll: #48b06a"/>. 
 00000df0: 2020 3c2f 673e 0a20 2020 3c67 2069 643d    </g>.   <g id=
 00000e00: 2270 6174 6368 5f31 3522 3e0a 2020 2020  "patch_15">.    
 00000e10: 3c70 6174 6820 643d 224d 2032 3532 2e35  <path d="M 252.5
 00000e20: 3237 3331 2032 3038 2e39 3938 3731 3420  2731 208.998714 
 00000e30: 0a4c 2032 3636 2e32 3736 3535 3420 3230  .L 266.276554 20
 00000e40: 382e 3939 3837 3134 200a 4c20 3236 362e  8.998714 .L 266.
 00000e50: 3237 3635 3534 2034 302e 3635 3336 3834  276554 40.653684
 00000e60: 200a 4c20 3235 322e 3532 3733 3120 3430   .L 252.52731 40
 00000e70: 2e36 3533 3638 3420 0a7a 0a22 2063 6c69  .653684 .z." cli
-00000e80: 702d 7061 7468 3d22 7572 6c28 2370 6132  p-path="url(#pa2
-00000e90: 3766 3363 3536 3361 2922 2073 7479 6c65  7f3c563a)" style
+00000e80: 702d 7061 7468 3d22 7572 6c28 2370 3033  p-path="url(#p03
+00000e90: 6539 3338 3966 3838 2922 2073 7479 6c65  e9389f88)" style
 00000ea0: 3d22 6669 6c6c 3a20 2334 3961 6538 3322  ="fill: #49ae83"
 00000eb0: 2f3e 0a20 2020 3c2f 673e 0a20 2020 3c67  />.   </g>.   <g
 00000ec0: 2069 643d 2270 6174 6368 5f31 3622 3e0a   id="patch_16">.
 00000ed0: 2020 2020 3c70 6174 6820 643d 224d 2032      <path d="M 2
 00000ee0: 3639 2e37 3133 3836 3520 3230 382e 3939  69.713865 208.99
 00000ef0: 3837 3134 200a 4c20 3238 332e 3436 3331  8714 .L 283.4631
 00000f00: 3038 2032 3038 2e39 3938 3731 3420 0a4c  08 208.998714 .L
 00000f10: 2032 3833 2e34 3633 3130 3820 3631 2e30   283.463108 61.0
 00000f20: 3539 3134 3220 0a4c 2032 3639 2e37 3133  59142 .L 269.713
 00000f30: 3836 3520 3631 2e30 3539 3134 3220 0a7a  865 61.059142 .z
 00000f40: 0a22 2063 6c69 702d 7061 7468 3d22 7572  ." clip-path="ur
-00000f50: 6c28 2370 6132 3766 3363 3536 3361 2922  l(#pa27f3c563a)"
+00000f50: 6c28 2370 3033 6539 3338 3966 3838 2922  l(#p03e9389f88)"
 00000f60: 2073 7479 6c65 3d22 6669 6c6c 3a20 2334   style="fill: #4
 00000f70: 6161 6439 3122 2f3e 0a20 2020 3c2f 673e  aad91"/>.   </g>
 00000f80: 0a20 2020 3c67 2069 643d 2270 6174 6368  .   <g id="patch
 00000f90: 5f31 3722 3e0a 2020 2020 3c70 6174 6820  _17">.    <path 
 00000fa0: 643d 224d 2032 3836 2e39 3030 3431 3920  d="M 286.900419 
 00000fb0: 3230 382e 3939 3837 3134 200a 4c20 3330  208.998714 .L 30
 00000fc0: 302e 3634 3936 3633 2032 3038 2e39 3938  0.649663 208.998
 00000fd0: 3731 3420 0a4c 2033 3030 2e36 3439 3636  714 .L 300.64966
 00000fe0: 3320 3335 2e35 3532 3332 200a 4c20 3238  3 35.55232 .L 28
 00000ff0: 362e 3930 3034 3139 2033 352e 3535 3233  6.900419 35.5523
 00001000: 3220 0a7a 0a22 2063 6c69 702d 7061 7468  2 .z." clip-path
-00001010: 3d22 7572 6c28 2370 6132 3766 3363 3536  ="url(#pa27f3c56
-00001020: 3361 2922 2073 7479 6c65 3d22 6669 6c6c  3a)" style="fill
+00001010: 3d22 7572 6c28 2370 3033 6539 3338 3966  ="url(#p03e9389f
+00001020: 3838 2922 2073 7479 6c65 3d22 6669 6c6c  88)" style="fill
 00001030: 3a20 2334 6161 6339 6222 2f3e 0a20 2020  : #4aac9b"/>.   
 00001040: 3c2f 673e 0a20 2020 3c67 2069 643d 2270  </g>.   <g id="p
 00001050: 6174 6368 5f31 3822 3e0a 2020 2020 3c70  atch_18">.    <p
 00001060: 6174 6820 643d 224d 2033 3034 2e30 3836  ath d="M 304.086
 00001070: 3937 3420 3230 382e 3939 3837 3134 200a  974 208.998714 .
 00001080: 4c20 3331 372e 3833 3632 3137 2032 3038  L 317.836217 208
 00001090: 2e39 3938 3731 3420 0a4c 2033 3137 2e38  .998714 .L 317.8
 000010a0: 3336 3231 3720 3731 2e32 3631 3837 3220  36217 71.261872 
 000010b0: 0a4c 2033 3034 2e30 3836 3937 3420 3731  .L 304.086974 71
 000010c0: 2e32 3631 3837 3220 0a7a 0a22 2063 6c69  .261872 .z." cli
-000010d0: 702d 7061 7468 3d22 7572 6c28 2370 6132  p-path="url(#pa2
-000010e0: 3766 3363 3536 3361 2922 2073 7479 6c65  7f3c563a)" style
+000010d0: 702d 7061 7468 3d22 7572 6c28 2370 3033  p-path="url(#p03
+000010e0: 6539 3338 3966 3838 2922 2073 7479 6c65  e9389f88)" style
 000010f0: 3d22 6669 6c6c 3a20 2334 6261 6261 3422  ="fill: #4baba4"
 00001100: 2f3e 0a20 2020 3c2f 673e 0a20 2020 3c67  />.   </g>.   <g
 00001110: 2069 643d 2270 6174 6368 5f31 3922 3e0a   id="patch_19">.
 00001120: 2020 2020 3c70 6174 6820 643d 224d 2033      <path d="M 3
 00001130: 3231 2e32 3733 3532 3820 3230 382e 3939  21.273528 208.99
 00001140: 3837 3134 200a 4c20 3333 352e 3032 3237  8714 .L 335.0227
 00001150: 3732 2032 3038 2e39 3938 3731 3420 0a4c  72 208.998714 .L
 00001160: 2033 3335 2e30 3232 3737 3220 3631 2e30   335.022772 61.0
 00001170: 3539 3134 3220 0a4c 2033 3231 2e32 3733  59142 .L 321.273
 00001180: 3532 3820 3631 2e30 3539 3134 3220 0a7a  528 61.059142 .z
 00001190: 0a22 2063 6c69 702d 7061 7468 3d22 7572  ." clip-path="ur
-000011a0: 6c28 2370 6132 3766 3363 3536 3361 2922  l(#pa27f3c563a)"
+000011a0: 6c28 2370 3033 6539 3338 3966 3838 2922  l(#p03e9389f88)"
 000011b0: 2073 7479 6c65 3d22 6669 6c6c 3a20 2334   style="fill: #4
 000011c0: 6361 6261 6422 2f3e 0a20 2020 3c2f 673e  cabad"/>.   </g>
 000011d0: 0a20 2020 3c67 2069 643d 2270 6174 6368  .   <g id="patch
 000011e0: 5f32 3022 3e0a 2020 2020 3c70 6174 6820  _20">.    <path 
 000011f0: 643d 224d 2033 3338 2e34 3630 3038 3320  d="M 338.460083 
 00001200: 3230 382e 3939 3837 3134 200a 4c20 3335  208.998714 .L 35
 00001210: 322e 3230 3933 3236 2032 3038 2e39 3938  2.209326 208.998
 00001220: 3731 3420 0a4c 2033 3532 2e32 3039 3332  714 .L 352.20932
 00001230: 3620 3335 2e35 3532 3332 200a 4c20 3333  6 35.55232 .L 33
 00001240: 382e 3436 3030 3833 2033 352e 3535 3233  8.460083 35.5523
 00001250: 3220 0a7a 0a22 2063 6c69 702d 7061 7468  2 .z." clip-path
-00001260: 3d22 7572 6c28 2370 6132 3766 3363 3536  ="url(#pa27f3c56
-00001270: 3361 2922 2073 7479 6c65 3d22 6669 6c6c  3a)" style="fill
+00001260: 3d22 7572 6c28 2370 3033 6539 3338 3966  ="url(#p03e9389f
+00001270: 3838 2922 2073 7479 6c65 3d22 6669 6c6c  88)" style="fill
 00001280: 3a20 2334 6561 6262 3722 2f3e 0a20 2020  : #4eabb7"/>.   
 00001290: 3c2f 673e 0a20 2020 3c67 2069 643d 2270  </g>.   <g id="p
 000012a0: 6174 6368 5f32 3122 3e0a 2020 2020 3c70  atch_21">.    <p
 000012b0: 6174 6820 643d 224d 2033 3535 2e36 3436  ath d="M 355.646
 000012c0: 3633 3720 3230 382e 3939 3837 3134 200a  637 208.998714 .
 000012d0: 4c20 3336 392e 3339 3538 3831 2032 3038  L 369.395881 208
 000012e0: 2e39 3938 3731 3420 0a4c 2033 3639 2e33  .998714 .L 369.3
 000012f0: 3935 3838 3120 3530 2e38 3536 3431 3320  95881 50.856413 
 00001300: 0a4c 2033 3535 2e36 3436 3633 3720 3530  .L 355.646637 50
 00001310: 2e38 3536 3431 3320 0a7a 0a22 2063 6c69  .856413 .z." cli
-00001320: 702d 7061 7468 3d22 7572 6c28 2370 6132  p-path="url(#pa2
-00001330: 3766 3363 3536 3361 2922 2073 7479 6c65  7f3c563a)" style
+00001320: 702d 7061 7468 3d22 7572 6c28 2370 3033  p-path="url(#p03
+00001330: 6539 3338 3966 3838 2922 2073 7479 6c65  e9389f88)" style
 00001340: 3d22 6669 6c6c 3a20 2335 3061 6363 3322  ="fill: #50acc3"
 00001350: 2f3e 0a20 2020 3c2f 673e 0a20 2020 3c67  />.   </g>.   <g
 00001360: 2069 643d 2270 6174 6368 5f32 3222 3e0a   id="patch_22">.
 00001370: 2020 2020 3c70 6174 6820 643d 224d 2033      <path d="M 3
 00001380: 3732 2e38 3333 3139 3220 3230 382e 3939  72.833192 208.99
 00001390: 3837 3134 200a 4c20 3338 362e 3538 3234  8714 .L 386.5824
 000013a0: 3335 2032 3038 2e39 3938 3731 3420 0a4c  35 208.998714 .L
 000013b0: 2033 3836 2e35 3832 3433 3520 3435 2e37   386.582435 45.7
 000013c0: 3535 3034 3920 0a4c 2033 3732 2e38 3333  55049 .L 372.833
 000013d0: 3139 3220 3435 2e37 3535 3034 3920 0a7a  192 45.755049 .z
 000013e0: 0a22 2063 6c69 702d 7061 7468 3d22 7572  ." clip-path="ur
-000013f0: 6c28 2370 6132 3766 3363 3536 3361 2922  l(#pa27f3c563a)"
+000013f0: 6c28 2370 3033 6539 3338 3966 3838 2922  l(#p03e9389f88)"
 00001400: 2073 7479 6c65 3d22 6669 6c6c 3a20 2335   style="fill: #5
 00001410: 3461 6364 3122 2f3e 0a20 2020 3c2f 673e  4acd1"/>.   </g>
 00001420: 0a20 2020 3c67 2069 643d 2270 6174 6368  .   <g id="patch
 00001430: 5f32 3322 3e0a 2020 2020 3c70 6174 6820  _23">.    <path 
 00001440: 643d 224d 2033 3930 2e30 3139 3734 3620  d="M 390.019746 
 00001450: 3230 382e 3939 3837 3134 200a 4c20 3430  208.998714 .L 40
 00001460: 332e 3736 3839 3920 3230 382e 3939 3837  3.76899 208.9987
 00001470: 3134 200a 4c20 3430 332e 3736 3839 3920  14 .L 403.76899 
 00001480: 3131 322e 3037 3237 3838 200a 4c20 3339  112.072788 .L 39
 00001490: 302e 3031 3937 3436 2031 3132 2e30 3732  0.019746 112.072
 000014a0: 3738 3820 0a7a 0a22 2063 6c69 702d 7061  788 .z." clip-pa
-000014b0: 7468 3d22 7572 6c28 2370 6132 3766 3363  th="url(#pa27f3c
-000014c0: 3536 3361 2922 2073 7479 6c65 3d22 6669  563a)" style="fi
+000014b0: 7468 3d22 7572 6c28 2370 3033 6539 3338  th="url(#p03e938
+000014c0: 3966 3838 2922 2073 7479 6c65 3d22 6669  9f88)" style="fi
 000014d0: 6c6c 3a20 2336 6461 6565 3222 2f3e 0a20  ll: #6daee2"/>. 
 000014e0: 2020 3c2f 673e 0a20 2020 3c67 2069 643d    </g>.   <g id=
 000014f0: 2270 6174 6368 5f32 3422 3e0a 2020 2020  "patch_24">.    
 00001500: 3c70 6174 6820 643d 224d 2034 3037 2e32  <path d="M 407.2
 00001510: 3036 3330 3120 3230 382e 3939 3837 3134  06301 208.998714
 00001520: 200a 4c20 3432 302e 3935 3535 3435 2032   .L 420.955545 2
 00001530: 3038 2e39 3938 3731 3420 0a4c 2034 3230  08.998714 .L 420
 00001540: 2e39 3535 3534 3520 3132 322e 3237 3535  .955545 122.2755
 00001550: 3137 200a 4c20 3430 372e 3230 3633 3031  17 .L 407.206301
 00001560: 2031 3232 2e32 3735 3531 3720 0a7a 0a22   122.275517 .z."
 00001570: 2063 6c69 702d 7061 7468 3d22 7572 6c28   clip-path="url(
-00001580: 2370 6132 3766 3363 3536 3361 2922 2073  #pa27f3c563a)" s
+00001580: 2370 3033 6539 3338 3966 3838 2922 2073  #p03e9389f88)" s
 00001590: 7479 6c65 3d22 6669 6c6c 3a20 2339 3461  tyle="fill: #94a
 000015a0: 6565 3822 2f3e 0a20 2020 3c2f 673e 0a20  ee8"/>.   </g>. 
 000015b0: 2020 3c67 2069 643d 2270 6174 6368 5f32    <g id="patch_2
 000015c0: 3522 3e0a 2020 2020 3c70 6174 6820 643d  5">.    <path d=
 000015d0: 224d 2034 3234 2e33 3932 3835 3520 3230  "M 424.392855 20
 000015e0: 382e 3939 3837 3134 200a 4c20 3433 382e  8.998714 .L 438.
 000015f0: 3134 3230 3939 2032 3038 2e39 3938 3731  142099 208.99871
 00001600: 3420 0a4c 2034 3338 2e31 3432 3039 3920  4 .L 438.142099 
 00001610: 3831 2e34 3634 3630 3120 0a4c 2034 3234  81.464601 .L 424
 00001620: 2e33 3932 3835 3520 3831 2e34 3634 3630  .392855 81.46460
 00001630: 3120 0a7a 0a22 2063 6c69 702d 7061 7468  1 .z." clip-path
-00001640: 3d22 7572 6c28 2370 6132 3766 3363 3536  ="url(#pa27f3c56
-00001650: 3361 2922 2073 7479 6c65 3d22 6669 6c6c  3a)" style="fill
+00001640: 3d22 7572 6c28 2370 3033 6539 3338 3966  ="url(#p03e9389f
+00001650: 3838 2922 2073 7479 6c65 3d22 6669 6c6c  88)" style="fill
 00001660: 3a20 2361 6461 6265 6222 2f3e 0a20 2020  : #adabeb"/>.   
 00001670: 3c2f 673e 0a20 2020 3c67 2069 643d 2270  </g>.   <g id="p
 00001680: 6174 6368 5f32 3622 3e0a 2020 2020 3c70  atch_26">.    <p
 00001690: 6174 6820 643d 224d 2034 3431 2e35 3739  ath d="M 441.579
 000016a0: 3431 2032 3038 2e39 3938 3731 3420 0a4c  41 208.998714 .L
 000016b0: 2034 3535 2e33 3238 3635 3420 3230 382e   455.328654 208.
 000016c0: 3939 3837 3134 200a 4c20 3435 352e 3332  998714 .L 455.32
 000016d0: 3836 3534 2031 3638 2e31 3837 3739 3820  8654 168.187798 
 000016e0: 0a4c 2034 3431 2e35 3739 3431 2031 3638  .L 441.57941 168
 000016f0: 2e31 3837 3739 3820 0a7a 0a22 2063 6c69  .187798 .z." cli
-00001700: 702d 7061 7468 3d22 7572 6c28 2370 6132  p-path="url(#pa2
-00001710: 3766 3363 3536 3361 2922 2073 7479 6c65  7f3c563a)" style
+00001700: 702d 7061 7468 3d22 7572 6c28 2370 3033  p-path="url(#p03
+00001710: 6539 3338 3966 3838 2922 2073 7479 6c65  e9389f88)" style
 00001720: 3d22 6669 6c6c 3a20 2362 6561 3465 6122  ="fill: #bea4ea"
 00001730: 2f3e 0a20 2020 3c2f 673e 0a20 2020 3c67  />.   </g>.   <g
 00001740: 2069 643d 2270 6174 6368 5f32 3722 3e0a   id="patch_27">.
 00001750: 2020 2020 3c70 6174 6820 643d 224d 2034      <path d="M 4
 00001760: 3538 2e37 3635 3936 3520 3230 382e 3939  58.765965 208.99
 00001770: 3837 3134 200a 4c20 3437 322e 3531 3532  8714 .L 472.5152
 00001780: 3038 2032 3038 2e39 3938 3731 3420 0a4c  08 208.998714 .L
 00001790: 2034 3732 2e35 3135 3230 3820 3135 322e   472.515208 152.
 000017a0: 3838 3337 3034 200a 4c20 3435 382e 3736  883704 .L 458.76
 000017b0: 3539 3635 2031 3532 2e38 3833 3730 3420  5965 152.883704 
 000017c0: 0a7a 0a22 2063 6c69 702d 7061 7468 3d22  .z." clip-path="
-000017d0: 7572 6c28 2370 6132 3766 3363 3536 3361  url(#pa27f3c563a
+000017d0: 7572 6c28 2370 3033 6539 3338 3966 3838  url(#p03e9389f88
 000017e0: 2922 2073 7479 6c65 3d22 6669 6c6c 3a20  )" style="fill: 
 000017f0: 2363 6539 6265 3922 2f3e 0a20 2020 3c2f  #ce9be9"/>.   </
 00001800: 673e 0a20 2020 3c67 2069 643d 2270 6174  g>.   <g id="pat
 00001810: 6368 5f32 3822 3e0a 2020 2020 3c70 6174  ch_28">.    <pat
 00001820: 6820 643d 224d 2034 3735 2e39 3532 3531  h d="M 475.95251
 00001830: 3920 3230 382e 3939 3837 3134 200a 4c20  9 208.998714 .L 
 00001840: 3438 392e 3730 3137 3633 2032 3038 2e39  489.701763 208.9
 00001850: 3938 3731 3420 0a4c 2034 3839 2e37 3031  98714 .L 489.701
 00001860: 3736 3320 3134 372e 3738 3233 3420 0a4c  763 147.78234 .L
 00001870: 2034 3735 2e39 3532 3531 3920 3134 372e   475.952519 147.
 00001880: 3738 3233 3420 0a7a 0a22 2063 6c69 702d  78234 .z." clip-
-00001890: 7061 7468 3d22 7572 6c28 2370 6132 3766  path="url(#pa27f
-000018a0: 3363 3536 3361 2922 2073 7479 6c65 3d22  3c563a)" style="
+00001890: 7061 7468 3d22 7572 6c28 2370 3033 6539  path="url(#p03e9
+000018a0: 3338 3966 3838 2922 2073 7479 6c65 3d22  389f88)" style="
 000018b0: 6669 6c6c 3a20 2364 6638 6665 3722 2f3e  fill: #df8fe7"/>
 000018c0: 0a20 2020 3c2f 673e 0a20 2020 3c67 2069  .   </g>.   <g i
 000018d0: 643d 2270 6174 6368 5f32 3922 3e0a 2020  d="patch_29">.  
 000018e0: 2020 3c70 6174 6820 643d 224d 2034 3933    <path d="M 493
 000018f0: 2e31 3339 3037 3420 3230 382e 3939 3837  .139074 208.9987
 00001900: 3134 200a 4c20 3530 362e 3838 3833 3137  14 .L 506.888317
 00001910: 2032 3038 2e39 3938 3731 3420 0a4c 2035   208.998714 .L 5
 00001920: 3036 2e38 3838 3331 3720 3134 322e 3638  06.888317 142.68
 00001930: 3039 3735 200a 4c20 3439 332e 3133 3930  0975 .L 493.1390
 00001940: 3734 2031 3432 2e36 3830 3937 3520 0a7a  74 142.680975 .z
 00001950: 0a22 2063 6c69 702d 7061 7468 3d22 7572  ." clip-path="ur
-00001960: 6c28 2370 6132 3766 3363 3536 3361 2922  l(#pa27f3c563a)"
+00001960: 6c28 2370 3033 6539 3338 3966 3838 2922  l(#p03e9389f88)"
 00001970: 2073 7479 6c65 3d22 6669 6c6c 3a20 2365   style="fill: #e
 00001980: 3738 6264 6222 2f3e 0a20 2020 3c2f 673e  78bdb"/>.   </g>
 00001990: 0a20 2020 3c67 2069 643d 2270 6174 6368  .   <g id="patch
 000019a0: 5f33 3022 3e0a 2020 2020 3c70 6174 6820  _30">.    <path 
 000019b0: 643d 224d 2035 3130 2e33 3235 3632 3820  d="M 510.325628 
 000019c0: 3230 382e 3939 3837 3134 200a 4c20 3532  208.998714 .L 52
 000019d0: 342e 3037 3438 3732 2032 3038 2e39 3938  4.074872 208.998
 000019e0: 3731 3420 0a4c 2035 3234 2e30 3734 3837  714 .L 524.07487
 000019f0: 3220 3133 372e 3537 3936 3131 200a 4c20  2 137.579611 .L 
 00001a00: 3531 302e 3332 3536 3238 2031 3337 2e35  510.325628 137.5
 00001a10: 3739 3631 3120 0a7a 0a22 2063 6c69 702d  79611 .z." clip-
-00001a20: 7061 7468 3d22 7572 6c28 2370 6132 3766  path="url(#pa27f
-00001a30: 3363 3536 3361 2922 2073 7479 6c65 3d22  3c563a)" style="
+00001a20: 7061 7468 3d22 7572 6c28 2370 3033 6539  path="url(#p03e9
+00001a30: 3338 3966 3838 2922 2073 7479 6c65 3d22  389f88)" style="
 00001a40: 6669 6c6c 3a20 2365 3838 6663 6322 2f3e  fill: #e88fcc"/>
 00001a50: 0a20 2020 3c2f 673e 0a20 2020 3c67 2069  .   </g>.   <g i
 00001a60: 643d 2270 6174 6368 5f33 3122 3e0a 2020  d="patch_31">.  
 00001a70: 2020 3c70 6174 6820 643d 224d 2035 3237    <path d="M 527
 00001a80: 2e35 3132 3138 3320 3230 382e 3939 3837  .512183 208.9987
 00001a90: 3134 200a 4c20 3534 312e 3236 3134 3236  14 .L 541.261426
 00001aa0: 2032 3038 2e39 3938 3731 3420 0a4c 2035   208.998714 .L 5
 00001ab0: 3431 2e32 3631 3432 3620 3136 382e 3138  41.261426 168.18
 00001ac0: 3737 3938 200a 4c20 3532 372e 3531 3231  7798 .L 527.5121
 00001ad0: 3833 2031 3638 2e31 3837 3739 3820 0a7a  83 168.187798 .z
 00001ae0: 0a22 2063 6c69 702d 7061 7468 3d22 7572  ." clip-path="ur
-00001af0: 6c28 2370 6132 3766 3363 3536 3361 2922  l(#pa27f3c563a)"
+00001af0: 6c28 2370 3033 6539 3338 3966 3838 2922  l(#p03e9389f88)"
 00001b00: 2073 7479 6c65 3d22 6669 6c6c 3a20 2365   style="fill: #e
 00001b10: 3839 3162 6622 2f3e 0a20 2020 3c2f 673e  891bf"/>.   </g>
 00001b20: 0a20 2020 3c67 2069 643d 2270 6174 6368  .   <g id="patch
 00001b30: 5f33 3222 3e0a 2020 2020 3c70 6174 6820  _32">.    <path 
 00001b40: 643d 224d 2035 3434 2e36 3938 3733 3720  d="M 544.698737 
 00001b50: 3230 382e 3939 3837 3134 200a 4c20 3535  208.998714 .L 55
 00001b60: 382e 3434 3739 3831 2032 3038 2e39 3938  8.447981 208.998
 00001b70: 3731 3420 0a4c 2035 3538 2e34 3437 3938  714 .L 558.44798
 00001b80: 3120 3139 332e 3639 3436 3231 200a 4c20  1 193.694621 .L 
 00001b90: 3534 342e 3639 3837 3337 2031 3933 2e36  544.698737 193.6
 00001ba0: 3934 3632 3120 0a7a 0a22 2063 6c69 702d  94621 .z." clip-
-00001bb0: 7061 7468 3d22 7572 6c28 2370 6132 3766  path="url(#pa27f
-00001bc0: 3363 3536 3361 2922 2073 7479 6c65 3d22  3c563a)" style="
+00001bb0: 7061 7468 3d22 7572 6c28 2370 3033 6539  path="url(#p03e9
+00001bc0: 3338 3966 3838 2922 2073 7479 6c65 3d22  389f88)" style="
 00001bd0: 6669 6c6c 3a20 2365 3939 3462 3222 2f3e  fill: #e994b2"/>
 00001be0: 0a20 2020 3c2f 673e 0a20 2020 3c67 2069  .   </g>.   <g i
 00001bf0: 643d 226d 6174 706c 6f74 6c69 622e 6178  d="matplotlib.ax
 00001c00: 6973 5f31 223e 0a20 2020 203c 6720 6964  is_1">.    <g id
 00001c10: 3d22 7874 6963 6b5f 3122 3e0a 2020 2020  ="xtick_1">.    
 00001c20: 203c 6720 6964 3d22 6c69 6e65 3264 5f31   <g id="line2d_1
 00001c30: 223e 0a20 2020 2020 203c 6465 6673 3e0a  ">.      <defs>.
 00001c40: 2020 2020 2020 203c 7061 7468 2069 643d         <path id=
-00001c50: 226d 6566 3433 3538 6334 6235 2220 643d  "mef4358c4b5" d=
+00001c50: 226d 6265 3139 3430 3333 3865 2220 643d  "mbe1940338e" d=
 00001c60: 224d 2030 2030 200a 4c20 3020 332e 3520  "M 0 0 .L 0 3.5 
 00001c70: 0a22 2073 7479 6c65 3d22 7374 726f 6b65  ." style="stroke
 00001c80: 3a20 2330 3030 3030 303b 2073 7472 6f6b  : #000000; strok
 00001c90: 652d 7769 6474 683a 2030 2e38 222f 3e0a  e-width: 0.8"/>.
 00001ca0: 2020 2020 2020 3c2f 6465 6673 3e0a 2020        </defs>.  
 00001cb0: 2020 2020 3c67 3e0a 2020 2020 2020 203c      <g>.       <
 00001cc0: 7573 6520 786c 696e 6b3a 6872 6566 3d22  use xlink:href="
-00001cd0: 236d 6566 3433 3538 6334 6235 2220 783d  #mef4358c4b5" x=
+00001cd0: 236d 6265 3139 3430 3333 3865 2220 783d  #mbe1940338e" x=
 00001ce0: 2235 332e 3136 3332 3737 2220 793d 2232  "53.163277" y="2
 00001cf0: 3038 2e39 3938 3731 3422 2073 7479 6c65  08.998714" style
 00001d00: 3d22 7374 726f 6b65 3a20 2330 3030 3030  ="stroke: #00000
 00001d10: 303b 2073 7472 6f6b 652d 7769 6474 683a  0; stroke-width:
 00001d20: 2030 2e38 222f 3e0a 2020 2020 2020 3c2f   0.8"/>.      </
 00001d30: 673e 0a20 2020 2020 3c2f 673e 0a20 2020  g>.     </g>.   
 00001d40: 2020 3c67 2069 643d 2274 6578 745f 3122    <g id="text_1"
@@ -561,15 +561,15 @@
 00002300: 222f 3e0a 2020 2020 2020 3c2f 673e 0a20  "/>.      </g>. 
 00002310: 2020 2020 3c2f 673e 0a20 2020 203c 2f67      </g>.    </g
 00002320: 3e0a 2020 2020 3c67 2069 643d 2278 7469  >.    <g id="xti
 00002330: 636b 5f32 223e 0a20 2020 2020 3c67 2069  ck_2">.     <g i
 00002340: 643d 226c 696e 6532 645f 3222 3e0a 2020  d="line2d_2">.  
 00002350: 2020 2020 3c67 3e0a 2020 2020 2020 203c      <g>.       <
 00002360: 7573 6520 786c 696e 6b3a 6872 6566 3d22  use xlink:href="
-00002370: 236d 6566 3433 3538 6334 6235 2220 783d  #mef4358c4b5" x=
+00002370: 236d 6265 3139 3430 3333 3865 2220 783d  #mbe1940338e" x=
 00002380: 2237 302e 3334 3938 3332 2220 793d 2232  "70.349832" y="2
 00002390: 3038 2e39 3938 3731 3422 2073 7479 6c65  08.998714" style
 000023a0: 3d22 7374 726f 6b65 3a20 2330 3030 3030  ="stroke: #00000
 000023b0: 303b 2073 7472 6f6b 652d 7769 6474 683a  0; stroke-width:
 000023c0: 2030 2e38 222f 3e0a 2020 2020 2020 3c2f   0.8"/>.      </
 000023d0: 673e 0a20 2020 2020 3c2f 673e 0a20 2020  g>.     </g>.   
 000023e0: 2020 3c67 2069 643d 2274 6578 745f 3222    <g id="text_2"
@@ -628,16 +628,16 @@
 00002730: 783d 2231 3930 2e38 3639 3134 3122 2f3e  x="190.869141"/>
 00002740: 0a20 2020 2020 203c 2f67 3e0a 2020 2020  .      </g>.    
 00002750: 203c 2f67 3e0a 2020 2020 3c2f 673e 0a20   </g>.    </g>. 
 00002760: 2020 203c 6720 6964 3d22 7874 6963 6b5f     <g id="xtick_
 00002770: 3322 3e0a 2020 2020 203c 6720 6964 3d22  3">.     <g id="
 00002780: 6c69 6e65 3264 5f33 223e 0a20 2020 2020  line2d_3">.     
 00002790: 203c 673e 0a20 2020 2020 2020 3c75 7365   <g>.       <use
-000027a0: 2078 6c69 6e6b 3a68 7265 663d 2223 6d65   xlink:href="#me
-000027b0: 6634 3335 3863 3462 3522 2078 3d22 3837  f4358c4b5" x="87
+000027a0: 2078 6c69 6e6b 3a68 7265 663d 2223 6d62   xlink:href="#mb
+000027b0: 6531 3934 3033 3338 6522 2078 3d22 3837  e1940338e" x="87
 000027c0: 2e35 3336 3338 3622 2079 3d22 3230 382e  .536386" y="208.
 000027d0: 3939 3837 3134 2220 7374 796c 653d 2273  998714" style="s
 000027e0: 7472 6f6b 653a 2023 3030 3030 3030 3b20  troke: #000000; 
 000027f0: 7374 726f 6b65 2d77 6964 7468 3a20 302e  stroke-width: 0.
 00002800: 3822 2f3e 0a20 2020 2020 203c 2f67 3e0a  8"/>.      </g>.
 00002810: 2020 2020 203c 2f67 3e0a 2020 2020 203c       </g>.     <
 00002820: 6720 6964 3d22 7465 7874 5f33 223e 0a20  g id="text_3">. 
@@ -705,16 +705,16 @@
 00002c00: 2e38 3639 3134 3122 2f3e 0a20 2020 2020  .869141"/>.     
 00002c10: 203c 2f67 3e0a 2020 2020 203c 2f67 3e0a   </g>.     </g>.
 00002c20: 2020 2020 3c2f 673e 0a20 2020 203c 6720      </g>.    <g 
 00002c30: 6964 3d22 7874 6963 6b5f 3422 3e0a 2020  id="xtick_4">.  
 00002c40: 2020 203c 6720 6964 3d22 6c69 6e65 3264     <g id="line2d
 00002c50: 5f34 223e 0a20 2020 2020 203c 673e 0a20  _4">.      <g>. 
 00002c60: 2020 2020 2020 3c75 7365 2078 6c69 6e6b        <use xlink
-00002c70: 3a68 7265 663d 2223 6d65 6634 3335 3863  :href="#mef4358c
-00002c80: 3462 3522 2078 3d22 3130 342e 3732 3239  4b5" x="104.7229
+00002c70: 3a68 7265 663d 2223 6d62 6531 3934 3033  :href="#mbe19403
+00002c80: 3338 6522 2078 3d22 3130 342e 3732 3239  38e" x="104.7229
 00002c90: 3431 2220 793d 2232 3038 2e39 3938 3731  41" y="208.99871
 00002ca0: 3422 2073 7479 6c65 3d22 7374 726f 6b65  4" style="stroke
 00002cb0: 3a20 2330 3030 3030 303b 2073 7472 6f6b  : #000000; strok
 00002cc0: 652d 7769 6474 683a 2030 2e38 222f 3e0a  e-width: 0.8"/>.
 00002cd0: 2020 2020 2020 3c2f 673e 0a20 2020 2020        </g>.     
 00002ce0: 3c2f 673e 0a20 2020 2020 3c67 2069 643d  </g>.     <g id=
 00002cf0: 2274 6578 745f 3422 3e0a 2020 2020 2020  "text_4">.      
@@ -752,15 +752,15 @@
 00002ef0: 3122 2f3e 0a20 2020 2020 203c 2f67 3e0a  1"/>.      </g>.
 00002f00: 2020 2020 203c 2f67 3e0a 2020 2020 3c2f       </g>.    </
 00002f10: 673e 0a20 2020 203c 6720 6964 3d22 7874  g>.    <g id="xt
 00002f20: 6963 6b5f 3522 3e0a 2020 2020 203c 6720  ick_5">.     <g 
 00002f30: 6964 3d22 6c69 6e65 3264 5f35 223e 0a20  id="line2d_5">. 
 00002f40: 2020 2020 203c 673e 0a20 2020 2020 2020       <g>.       
 00002f50: 3c75 7365 2078 6c69 6e6b 3a68 7265 663d  <use xlink:href=
-00002f60: 2223 6d65 6634 3335 3863 3462 3522 2078  "#mef4358c4b5" x
+00002f60: 2223 6d62 6531 3934 3033 3338 6522 2078  "#mbe1940338e" x
 00002f70: 3d22 3132 312e 3930 3934 3935 2220 793d  ="121.909495" y=
 00002f80: 2232 3038 2e39 3938 3731 3422 2073 7479  "208.998714" sty
 00002f90: 6c65 3d22 7374 726f 6b65 3a20 2330 3030  le="stroke: #000
 00002fa0: 3030 303b 2073 7472 6f6b 652d 7769 6474  000; stroke-widt
 00002fb0: 683a 2030 2e38 222f 3e0a 2020 2020 2020  h: 0.8"/>.      
 00002fc0: 3c2f 673e 0a20 2020 2020 3c2f 673e 0a20  </g>.     </g>. 
 00002fd0: 2020 2020 3c67 2069 643d 2274 6578 745f      <g id="text_
@@ -840,15 +840,15 @@
 00003470: 2f3e 0a20 2020 2020 203c 2f67 3e0a 2020  />.      </g>.  
 00003480: 2020 203c 2f67 3e0a 2020 2020 3c2f 673e     </g>.    </g>
 00003490: 0a20 2020 203c 6720 6964 3d22 7874 6963  .    <g id="xtic
 000034a0: 6b5f 3622 3e0a 2020 2020 203c 6720 6964  k_6">.     <g id
 000034b0: 3d22 6c69 6e65 3264 5f36 223e 0a20 2020  ="line2d_6">.   
 000034c0: 2020 203c 673e 0a20 2020 2020 2020 3c75     <g>.       <u
 000034d0: 7365 2078 6c69 6e6b 3a68 7265 663d 2223  se xlink:href="#
-000034e0: 6d65 6634 3335 3863 3462 3522 2078 3d22  mef4358c4b5" x="
+000034e0: 6d62 6531 3934 3033 3338 6522 2078 3d22  mbe1940338e" x="
 000034f0: 3133 392e 3039 3630 3522 2079 3d22 3230  139.09605" y="20
 00003500: 382e 3939 3837 3134 2220 7374 796c 653d  8.998714" style=
 00003510: 2273 7472 6f6b 653a 2023 3030 3030 3030  "stroke: #000000
 00003520: 3b20 7374 726f 6b65 2d77 6964 7468 3a20  ; stroke-width: 
 00003530: 302e 3822 2f3e 0a20 2020 2020 203c 2f67  0.8"/>.      </g
 00003540: 3e0a 2020 2020 203c 2f67 3e0a 2020 2020  >.     </g>.    
 00003550: 203c 6720 6964 3d22 7465 7874 5f36 223e   <g id="text_6">
@@ -874,16 +874,16 @@
 00003690: 302e 3836 3931 3431 222f 3e0a 2020 2020  0.869141"/>.    
 000036a0: 2020 3c2f 673e 0a20 2020 2020 3c2f 673e    </g>.     </g>
 000036b0: 0a20 2020 203c 2f67 3e0a 2020 2020 3c67  .    </g>.    <g
 000036c0: 2069 643d 2278 7469 636b 5f37 223e 0a20   id="xtick_7">. 
 000036d0: 2020 2020 3c67 2069 643d 226c 696e 6532      <g id="line2
 000036e0: 645f 3722 3e0a 2020 2020 2020 3c67 3e0a  d_7">.      <g>.
 000036f0: 2020 2020 2020 203c 7573 6520 786c 696e         <use xlin
-00003700: 6b3a 6872 6566 3d22 236d 6566 3433 3538  k:href="#mef4358
-00003710: 6334 6235 2220 783d 2231 3536 2e32 3832  c4b5" x="156.282
+00003700: 6b3a 6872 6566 3d22 236d 6265 3139 3430  k:href="#mbe1940
+00003710: 3333 3865 2220 783d 2231 3536 2e32 3832  338e" x="156.282
 00003720: 3630 3522 2079 3d22 3230 382e 3939 3837  605" y="208.9987
 00003730: 3134 2220 7374 796c 653d 2273 7472 6f6b  14" style="strok
 00003740: 653a 2023 3030 3030 3030 3b20 7374 726f  e: #000000; stro
 00003750: 6b65 2d77 6964 7468 3a20 302e 3822 2f3e  ke-width: 0.8"/>
 00003760: 0a20 2020 2020 203c 2f67 3e0a 2020 2020  .      </g>.    
 00003770: 203c 2f67 3e0a 2020 2020 203c 6720 6964   </g>.     <g id
 00003780: 3d22 7465 7874 5f37 223e 0a20 2020 2020  ="text_7">.     
@@ -970,15 +970,15 @@
 00003c90: 3931 3431 222f 3e0a 2020 2020 2020 3c2f  9141"/>.      </
 00003ca0: 673e 0a20 2020 2020 3c2f 673e 0a20 2020  g>.     </g>.   
 00003cb0: 203c 2f67 3e0a 2020 2020 3c67 2069 643d   </g>.    <g id=
 00003cc0: 2278 7469 636b 5f38 223e 0a20 2020 2020  "xtick_8">.     
 00003cd0: 3c67 2069 643d 226c 696e 6532 645f 3822  <g id="line2d_8"
 00003ce0: 3e0a 2020 2020 2020 3c67 3e0a 2020 2020  >.      <g>.    
 00003cf0: 2020 203c 7573 6520 786c 696e 6b3a 6872     <use xlink:hr
-00003d00: 6566 3d22 236d 6566 3433 3538 6334 6235  ef="#mef4358c4b5
+00003d00: 6566 3d22 236d 6265 3139 3430 3333 3865  ef="#mbe1940338e
 00003d10: 2220 783d 2231 3733 2e34 3639 3135 3922  " x="173.469159"
 00003d20: 2079 3d22 3230 382e 3939 3837 3134 2220   y="208.998714" 
 00003d30: 7374 796c 653d 2273 7472 6f6b 653a 2023  style="stroke: #
 00003d40: 3030 3030 3030 3b20 7374 726f 6b65 2d77  000000; stroke-w
 00003d50: 6964 7468 3a20 302e 3822 2f3e 0a20 2020  idth: 0.8"/>.   
 00003d60: 2020 203c 2f67 3e0a 2020 2020 203c 2f67     </g>.     </g
 00003d70: 3e0a 2020 2020 203c 6720 6964 3d22 7465  >.     <g id="te
@@ -1005,15 +1005,15 @@
 00003ec0: 3e0a 2020 2020 2020 3c2f 673e 0a20 2020  >.      </g>.   
 00003ed0: 2020 3c2f 673e 0a20 2020 203c 2f67 3e0a    </g>.    </g>.
 00003ee0: 2020 2020 3c67 2069 643d 2278 7469 636b      <g id="xtick
 00003ef0: 5f39 223e 0a20 2020 2020 3c67 2069 643d  _9">.     <g id=
 00003f00: 226c 696e 6532 645f 3922 3e0a 2020 2020  "line2d_9">.    
 00003f10: 2020 3c67 3e0a 2020 2020 2020 203c 7573    <g>.       <us
 00003f20: 6520 786c 696e 6b3a 6872 6566 3d22 236d  e xlink:href="#m
-00003f30: 6566 3433 3538 6334 6235 2220 783d 2231  ef4358c4b5" x="1
+00003f30: 6265 3139 3430 3333 3865 2220 783d 2231  be1940338e" x="1
 00003f40: 3930 2e36 3535 3731 3422 2079 3d22 3230  90.655714" y="20
 00003f50: 382e 3939 3837 3134 2220 7374 796c 653d  8.998714" style=
 00003f60: 2273 7472 6f6b 653a 2023 3030 3030 3030  "stroke: #000000
 00003f70: 3b20 7374 726f 6b65 2d77 6964 7468 3a20  ; stroke-width: 
 00003f80: 302e 3822 2f3e 0a20 2020 2020 203c 2f67  0.8"/>.      </g
 00003f90: 3e0a 2020 2020 203c 2f67 3e0a 2020 2020  >.     </g>.    
 00003fa0: 203c 6720 6964 3d22 7465 7874 5f39 223e   <g id="text_9">
@@ -1039,16 +1039,16 @@
 000040e0: 302e 3836 3931 3431 222f 3e0a 2020 2020  0.869141"/>.    
 000040f0: 2020 3c2f 673e 0a20 2020 2020 3c2f 673e    </g>.     </g>
 00004100: 0a20 2020 203c 2f67 3e0a 2020 2020 3c67  .    </g>.    <g
 00004110: 2069 643d 2278 7469 636b 5f31 3022 3e0a   id="xtick_10">.
 00004120: 2020 2020 203c 6720 6964 3d22 6c69 6e65       <g id="line
 00004130: 3264 5f31 3022 3e0a 2020 2020 2020 3c67  2d_10">.      <g
 00004140: 3e0a 2020 2020 2020 203c 7573 6520 786c  >.       <use xl
-00004150: 696e 6b3a 6872 6566 3d22 236d 6566 3433  ink:href="#mef43
-00004160: 3538 6334 6235 2220 783d 2232 3037 2e38  58c4b5" x="207.8
+00004150: 696e 6b3a 6872 6566 3d22 236d 6265 3139  ink:href="#mbe19
+00004160: 3430 3333 3865 2220 783d 2232 3037 2e38  40338e" x="207.8
 00004170: 3432 3236 3822 2079 3d22 3230 382e 3939  42268" y="208.99
 00004180: 3837 3134 2220 7374 796c 653d 2273 7472  8714" style="str
 00004190: 6f6b 653a 2023 3030 3030 3030 3b20 7374  oke: #000000; st
 000041a0: 726f 6b65 2d77 6964 7468 3a20 302e 3822  roke-width: 0.8"
 000041b0: 2f3e 0a20 2020 2020 203c 2f67 3e0a 2020  />.      </g>.  
 000041c0: 2020 203c 2f67 3e0a 2020 2020 203c 6720     </g>.     <g 
 000041d0: 6964 3d22 7465 7874 5f31 3022 3e0a 2020  id="text_10">.  
@@ -1118,16 +1118,16 @@
 000045d0: 3639 3134 3122 2f3e 0a20 2020 2020 203c  69141"/>.      <
 000045e0: 2f67 3e0a 2020 2020 203c 2f67 3e0a 2020  /g>.     </g>.  
 000045f0: 2020 3c2f 673e 0a20 2020 203c 6720 6964    </g>.    <g id
 00004600: 3d22 7874 6963 6b5f 3131 223e 0a20 2020  ="xtick_11">.   
 00004610: 2020 3c67 2069 643d 226c 696e 6532 645f    <g id="line2d_
 00004620: 3131 223e 0a20 2020 2020 203c 673e 0a20  11">.      <g>. 
 00004630: 2020 2020 2020 3c75 7365 2078 6c69 6e6b        <use xlink
-00004640: 3a68 7265 663d 2223 6d65 6634 3335 3863  :href="#mef4358c
-00004650: 3462 3522 2078 3d22 3232 352e 3032 3838  4b5" x="225.0288
+00004640: 3a68 7265 663d 2223 6d62 6531 3934 3033  :href="#mbe19403
+00004650: 3338 6522 2078 3d22 3232 352e 3032 3838  38e" x="225.0288
 00004660: 3233 2220 793d 2232 3038 2e39 3938 3731  23" y="208.99871
 00004670: 3422 2073 7479 6c65 3d22 7374 726f 6b65  4" style="stroke
 00004680: 3a20 2330 3030 3030 303b 2073 7472 6f6b  : #000000; strok
 00004690: 652d 7769 6474 683a 2030 2e38 222f 3e0a  e-width: 0.8"/>.
 000046a0: 2020 2020 2020 3c2f 673e 0a20 2020 2020        </g>.     
 000046b0: 3c2f 673e 0a20 2020 2020 3c67 2069 643d  </g>.     <g id=
 000046c0: 2274 6578 745f 3131 223e 0a20 2020 2020  "text_11">.     
@@ -1153,15 +1153,15 @@
 00004800: 3431 222f 3e0a 2020 2020 2020 3c2f 673e  41"/>.      </g>
 00004810: 0a20 2020 2020 3c2f 673e 0a20 2020 203c  .     </g>.    <
 00004820: 2f67 3e0a 2020 2020 3c67 2069 643d 2278  /g>.    <g id="x
 00004830: 7469 636b 5f31 3222 3e0a 2020 2020 203c  tick_12">.     <
 00004840: 6720 6964 3d22 6c69 6e65 3264 5f31 3222  g id="line2d_12"
 00004850: 3e0a 2020 2020 2020 3c67 3e0a 2020 2020  >.      <g>.    
 00004860: 2020 203c 7573 6520 786c 696e 6b3a 6872     <use xlink:hr
-00004870: 6566 3d22 236d 6566 3433 3538 6334 6235  ef="#mef4358c4b5
+00004870: 6566 3d22 236d 6265 3139 3430 3333 3865  ef="#mbe1940338e
 00004880: 2220 783d 2232 3432 2e32 3135 3337 3722  " x="242.215377"
 00004890: 2079 3d22 3230 382e 3939 3837 3134 2220   y="208.998714" 
 000048a0: 7374 796c 653d 2273 7472 6f6b 653a 2023  style="stroke: #
 000048b0: 3030 3030 3030 3b20 7374 726f 6b65 2d77  000000; stroke-w
 000048c0: 6964 7468 3a20 302e 3822 2f3e 0a20 2020  idth: 0.8"/>.   
 000048d0: 2020 203c 2f67 3e0a 2020 2020 203c 2f67     </g>.     </g
 000048e0: 3e0a 2020 2020 203c 6720 6964 3d22 7465  >.     <g id="te
@@ -1188,15 +1188,15 @@
 00004a30: 2f3e 0a20 2020 2020 203c 2f67 3e0a 2020  />.      </g>.  
 00004a40: 2020 203c 2f67 3e0a 2020 2020 3c2f 673e     </g>.    </g>
 00004a50: 0a20 2020 203c 6720 6964 3d22 7874 6963  .    <g id="xtic
 00004a60: 6b5f 3133 223e 0a20 2020 2020 3c67 2069  k_13">.     <g i
 00004a70: 643d 226c 696e 6532 645f 3133 223e 0a20  d="line2d_13">. 
 00004a80: 2020 2020 203c 673e 0a20 2020 2020 2020       <g>.       
 00004a90: 3c75 7365 2078 6c69 6e6b 3a68 7265 663d  <use xlink:href=
-00004aa0: 2223 6d65 6634 3335 3863 3462 3522 2078  "#mef4358c4b5" x
+00004aa0: 2223 6d62 6531 3934 3033 3338 6522 2078  "#mbe1940338e" x
 00004ab0: 3d22 3235 392e 3430 3139 3332 2220 793d  ="259.401932" y=
 00004ac0: 2232 3038 2e39 3938 3731 3422 2073 7479  "208.998714" sty
 00004ad0: 6c65 3d22 7374 726f 6b65 3a20 2330 3030  le="stroke: #000
 00004ae0: 3030 303b 2073 7472 6f6b 652d 7769 6474  000; stroke-widt
 00004af0: 683a 2030 2e38 222f 3e0a 2020 2020 2020  h: 0.8"/>.      
 00004b00: 3c2f 673e 0a20 2020 2020 3c2f 673e 0a20  </g>.     </g>. 
 00004b10: 2020 2020 3c67 2069 643d 2274 6578 745f      <g id="text_
@@ -1223,15 +1223,15 @@
 00004c60: 2020 2020 2020 3c2f 673e 0a20 2020 2020        </g>.     
 00004c70: 3c2f 673e 0a20 2020 203c 2f67 3e0a 2020  </g>.    </g>.  
 00004c80: 2020 3c67 2069 643d 2278 7469 636b 5f31    <g id="xtick_1
 00004c90: 3422 3e0a 2020 2020 203c 6720 6964 3d22  4">.     <g id="
 00004ca0: 6c69 6e65 3264 5f31 3422 3e0a 2020 2020  line2d_14">.    
 00004cb0: 2020 3c67 3e0a 2020 2020 2020 203c 7573    <g>.       <us
 00004cc0: 6520 786c 696e 6b3a 6872 6566 3d22 236d  e xlink:href="#m
-00004cd0: 6566 3433 3538 6334 6235 2220 783d 2232  ef4358c4b5" x="2
+00004cd0: 6265 3139 3430 3333 3865 2220 783d 2232  be1940338e" x="2
 00004ce0: 3736 2e35 3838 3438 3622 2079 3d22 3230  76.588486" y="20
 00004cf0: 382e 3939 3837 3134 2220 7374 796c 653d  8.998714" style=
 00004d00: 2273 7472 6f6b 653a 2023 3030 3030 3030  "stroke: #000000
 00004d10: 3b20 7374 726f 6b65 2d77 6964 7468 3a20  ; stroke-width: 
 00004d20: 302e 3822 2f3e 0a20 2020 2020 203c 2f67  0.8"/>.      </g
 00004d30: 3e0a 2020 2020 203c 2f67 3e0a 2020 2020  >.     </g>.    
 00004d40: 203c 6720 6964 3d22 7465 7874 5f31 3422   <g id="text_14"
@@ -1257,16 +1257,16 @@
 00004e80: 3930 2e38 3639 3134 3122 2f3e 0a20 2020  90.869141"/>.   
 00004e90: 2020 203c 2f67 3e0a 2020 2020 203c 2f67     </g>.     </g
 00004ea0: 3e0a 2020 2020 3c2f 673e 0a20 2020 203c  >.    </g>.    <
 00004eb0: 6720 6964 3d22 7874 6963 6b5f 3135 223e  g id="xtick_15">
 00004ec0: 0a20 2020 2020 3c67 2069 643d 226c 696e  .     <g id="lin
 00004ed0: 6532 645f 3135 223e 0a20 2020 2020 203c  e2d_15">.      <
 00004ee0: 673e 0a20 2020 2020 2020 3c75 7365 2078  g>.       <use x
-00004ef0: 6c69 6e6b 3a68 7265 663d 2223 6d65 6634  link:href="#mef4
-00004f00: 3335 3863 3462 3522 2078 3d22 3239 332e  358c4b5" x="293.
+00004ef0: 6c69 6e6b 3a68 7265 663d 2223 6d62 6531  link:href="#mbe1
+00004f00: 3934 3033 3338 6522 2078 3d22 3239 332e  940338e" x="293.
 00004f10: 3737 3530 3431 2220 793d 2232 3038 2e39  775041" y="208.9
 00004f20: 3938 3731 3422 2073 7479 6c65 3d22 7374  98714" style="st
 00004f30: 726f 6b65 3a20 2330 3030 3030 303b 2073  roke: #000000; s
 00004f40: 7472 6f6b 652d 7769 6474 683a 2030 2e38  troke-width: 0.8
 00004f50: 222f 3e0a 2020 2020 2020 3c2f 673e 0a20  "/>.      </g>. 
 00004f60: 2020 2020 3c2f 673e 0a20 2020 2020 3c67      </g>.     <g
 00004f70: 2069 643d 2274 6578 745f 3135 223e 0a20   id="text_15">. 
@@ -1292,16 +1292,16 @@
 000050b0: 3639 3134 3122 2f3e 0a20 2020 2020 203c  69141"/>.      <
 000050c0: 2f67 3e0a 2020 2020 203c 2f67 3e0a 2020  /g>.     </g>.  
 000050d0: 2020 3c2f 673e 0a20 2020 203c 6720 6964    </g>.    <g id
 000050e0: 3d22 7874 6963 6b5f 3136 223e 0a20 2020  ="xtick_16">.   
 000050f0: 2020 3c67 2069 643d 226c 696e 6532 645f    <g id="line2d_
 00005100: 3136 223e 0a20 2020 2020 203c 673e 0a20  16">.      <g>. 
 00005110: 2020 2020 2020 3c75 7365 2078 6c69 6e6b        <use xlink
-00005120: 3a68 7265 663d 2223 6d65 6634 3335 3863  :href="#mef4358c
-00005130: 3462 3522 2078 3d22 3331 302e 3936 3135  4b5" x="310.9615
+00005120: 3a68 7265 663d 2223 6d62 6531 3934 3033  :href="#mbe19403
+00005130: 3338 6522 2078 3d22 3331 302e 3936 3135  38e" x="310.9615
 00005140: 3935 2220 793d 2232 3038 2e39 3938 3731  95" y="208.99871
 00005150: 3422 2073 7479 6c65 3d22 7374 726f 6b65  4" style="stroke
 00005160: 3a20 2330 3030 3030 303b 2073 7472 6f6b  : #000000; strok
 00005170: 652d 7769 6474 683a 2030 2e38 222f 3e0a  e-width: 0.8"/>.
 00005180: 2020 2020 2020 3c2f 673e 0a20 2020 2020        </g>.     
 00005190: 3c2f 673e 0a20 2020 2020 3c67 2069 643d  </g>.     <g id=
 000051a0: 2274 6578 745f 3136 223e 0a20 2020 2020  "text_16">.     
@@ -1327,15 +1327,15 @@
 000052e0: 3431 222f 3e0a 2020 2020 2020 3c2f 673e  41"/>.      </g>
 000052f0: 0a20 2020 2020 3c2f 673e 0a20 2020 203c  .     </g>.    <
 00005300: 2f67 3e0a 2020 2020 3c67 2069 643d 2278  /g>.    <g id="x
 00005310: 7469 636b 5f31 3722 3e0a 2020 2020 203c  tick_17">.     <
 00005320: 6720 6964 3d22 6c69 6e65 3264 5f31 3722  g id="line2d_17"
 00005330: 3e0a 2020 2020 2020 3c67 3e0a 2020 2020  >.      <g>.    
 00005340: 2020 203c 7573 6520 786c 696e 6b3a 6872     <use xlink:hr
-00005350: 6566 3d22 236d 6566 3433 3538 6334 6235  ef="#mef4358c4b5
+00005350: 6566 3d22 236d 6265 3139 3430 3333 3865  ef="#mbe1940338e
 00005360: 2220 783d 2233 3238 2e31 3438 3135 2220  " x="328.14815" 
 00005370: 793d 2232 3038 2e39 3938 3731 3422 2073  y="208.998714" s
 00005380: 7479 6c65 3d22 7374 726f 6b65 3a20 2330  tyle="stroke: #0
 00005390: 3030 3030 303b 2073 7472 6f6b 652d 7769  00000; stroke-wi
 000053a0: 6474 683a 2030 2e38 222f 3e0a 2020 2020  dth: 0.8"/>.    
 000053b0: 2020 3c2f 673e 0a20 2020 2020 3c2f 673e    </g>.     </g>
 000053c0: 0a20 2020 2020 3c67 2069 643d 2274 6578  .     <g id="tex
@@ -1362,15 +1362,15 @@
 00005510: 3e0a 2020 2020 2020 3c2f 673e 0a20 2020  >.      </g>.   
 00005520: 2020 3c2f 673e 0a20 2020 203c 2f67 3e0a    </g>.    </g>.
 00005530: 2020 2020 3c67 2069 643d 2278 7469 636b      <g id="xtick
 00005540: 5f31 3822 3e0a 2020 2020 203c 6720 6964  _18">.     <g id
 00005550: 3d22 6c69 6e65 3264 5f31 3822 3e0a 2020  ="line2d_18">.  
 00005560: 2020 2020 3c67 3e0a 2020 2020 2020 203c      <g>.       <
 00005570: 7573 6520 786c 696e 6b3a 6872 6566 3d22  use xlink:href="
-00005580: 236d 6566 3433 3538 6334 6235 2220 783d  #mef4358c4b5" x=
+00005580: 236d 6265 3139 3430 3333 3865 2220 783d  #mbe1940338e" x=
 00005590: 2233 3435 2e33 3334 3730 3522 2079 3d22  "345.334705" y="
 000055a0: 3230 382e 3939 3837 3134 2220 7374 796c  208.998714" styl
 000055b0: 653d 2273 7472 6f6b 653a 2023 3030 3030  e="stroke: #0000
 000055c0: 3030 3b20 7374 726f 6b65 2d77 6964 7468  00; stroke-width
 000055d0: 3a20 302e 3822 2f3e 0a20 2020 2020 203c  : 0.8"/>.      <
 000055e0: 2f67 3e0a 2020 2020 203c 2f67 3e0a 2020  /g>.     </g>.  
 000055f0: 2020 203c 6720 6964 3d22 7465 7874 5f31     <g id="text_1
@@ -1396,16 +1396,16 @@
 00005730: 2231 3930 2e38 3639 3134 3122 2f3e 0a20  "190.869141"/>. 
 00005740: 2020 2020 203c 2f67 3e0a 2020 2020 203c       </g>.     <
 00005750: 2f67 3e0a 2020 2020 3c2f 673e 0a20 2020  /g>.    </g>.   
 00005760: 203c 6720 6964 3d22 7874 6963 6b5f 3139   <g id="xtick_19
 00005770: 223e 0a20 2020 2020 3c67 2069 643d 226c  ">.     <g id="l
 00005780: 696e 6532 645f 3139 223e 0a20 2020 2020  ine2d_19">.     
 00005790: 203c 673e 0a20 2020 2020 2020 3c75 7365   <g>.       <use
-000057a0: 2078 6c69 6e6b 3a68 7265 663d 2223 6d65   xlink:href="#me
-000057b0: 6634 3335 3863 3462 3522 2078 3d22 3336  f4358c4b5" x="36
+000057a0: 2078 6c69 6e6b 3a68 7265 663d 2223 6d62   xlink:href="#mb
+000057b0: 6531 3934 3033 3338 6522 2078 3d22 3336  e1940338e" x="36
 000057c0: 322e 3532 3132 3539 2220 793d 2232 3038  2.521259" y="208
 000057d0: 2e39 3938 3731 3422 2073 7479 6c65 3d22  .998714" style="
 000057e0: 7374 726f 6b65 3a20 2330 3030 3030 303b  stroke: #000000;
 000057f0: 2073 7472 6f6b 652d 7769 6474 683a 2030   stroke-width: 0
 00005800: 2e38 222f 3e0a 2020 2020 2020 3c2f 673e  .8"/>.      </g>
 00005810: 0a20 2020 2020 3c2f 673e 0a20 2020 2020  .     </g>.     
 00005820: 3c67 2069 643d 2274 6578 745f 3139 223e  <g id="text_19">
@@ -1431,16 +1431,16 @@
 00005960: 302e 3836 3931 3431 222f 3e0a 2020 2020  0.869141"/>.    
 00005970: 2020 3c2f 673e 0a20 2020 2020 3c2f 673e    </g>.     </g>
 00005980: 0a20 2020 203c 2f67 3e0a 2020 2020 3c67  .    </g>.    <g
 00005990: 2069 643d 2278 7469 636b 5f32 3022 3e0a   id="xtick_20">.
 000059a0: 2020 2020 203c 6720 6964 3d22 6c69 6e65       <g id="line
 000059b0: 3264 5f32 3022 3e0a 2020 2020 2020 3c67  2d_20">.      <g
 000059c0: 3e0a 2020 2020 2020 203c 7573 6520 786c  >.       <use xl
-000059d0: 696e 6b3a 6872 6566 3d22 236d 6566 3433  ink:href="#mef43
-000059e0: 3538 6334 6235 2220 783d 2233 3739 2e37  58c4b5" x="379.7
+000059d0: 696e 6b3a 6872 6566 3d22 236d 6265 3139  ink:href="#mbe19
+000059e0: 3430 3333 3865 2220 783d 2233 3739 2e37  40338e" x="379.7
 000059f0: 3037 3831 3422 2079 3d22 3230 382e 3939  07814" y="208.99
 00005a00: 3837 3134 2220 7374 796c 653d 2273 7472  8714" style="str
 00005a10: 6f6b 653a 2023 3030 3030 3030 3b20 7374  oke: #000000; st
 00005a20: 726f 6b65 2d77 6964 7468 3a20 302e 3822  roke-width: 0.8"
 00005a30: 2f3e 0a20 2020 2020 203c 2f67 3e0a 2020  />.      </g>.  
 00005a40: 2020 203c 2f67 3e0a 2020 2020 203c 6720     </g>.     <g 
 00005a50: 6964 3d22 7465 7874 5f32 3022 3e0a 2020  id="text_20">.  
@@ -1466,16 +1466,16 @@
 00005b90: 3639 3134 3122 2f3e 0a20 2020 2020 203c  69141"/>.      <
 00005ba0: 2f67 3e0a 2020 2020 203c 2f67 3e0a 2020  /g>.     </g>.  
 00005bb0: 2020 3c2f 673e 0a20 2020 203c 6720 6964    </g>.    <g id
 00005bc0: 3d22 7874 6963 6b5f 3231 223e 0a20 2020  ="xtick_21">.   
 00005bd0: 2020 3c67 2069 643d 226c 696e 6532 645f    <g id="line2d_
 00005be0: 3231 223e 0a20 2020 2020 203c 673e 0a20  21">.      <g>. 
 00005bf0: 2020 2020 2020 3c75 7365 2078 6c69 6e6b        <use xlink
-00005c00: 3a68 7265 663d 2223 6d65 6634 3335 3863  :href="#mef4358c
-00005c10: 3462 3522 2078 3d22 3339 362e 3839 3433  4b5" x="396.8943
+00005c00: 3a68 7265 663d 2223 6d62 6531 3934 3033  :href="#mbe19403
+00005c10: 3338 6522 2078 3d22 3339 362e 3839 3433  38e" x="396.8943
 00005c20: 3638 2220 793d 2232 3038 2e39 3938 3731  68" y="208.99871
 00005c30: 3422 2073 7479 6c65 3d22 7374 726f 6b65  4" style="stroke
 00005c40: 3a20 2330 3030 3030 303b 2073 7472 6f6b  : #000000; strok
 00005c50: 652d 7769 6474 683a 2030 2e38 222f 3e0a  e-width: 0.8"/>.
 00005c60: 2020 2020 2020 3c2f 673e 0a20 2020 2020        </g>.     
 00005c70: 3c2f 673e 0a20 2020 2020 3c67 2069 643d  </g>.     <g id=
 00005c80: 2274 6578 745f 3231 223e 0a20 2020 2020  "text_21">.     
@@ -1501,15 +1501,15 @@
 00005dc0: 3431 222f 3e0a 2020 2020 2020 3c2f 673e  41"/>.      </g>
 00005dd0: 0a20 2020 2020 3c2f 673e 0a20 2020 203c  .     </g>.    <
 00005de0: 2f67 3e0a 2020 2020 3c67 2069 643d 2278  /g>.    <g id="x
 00005df0: 7469 636b 5f32 3222 3e0a 2020 2020 203c  tick_22">.     <
 00005e00: 6720 6964 3d22 6c69 6e65 3264 5f32 3222  g id="line2d_22"
 00005e10: 3e0a 2020 2020 2020 3c67 3e0a 2020 2020  >.      <g>.    
 00005e20: 2020 203c 7573 6520 786c 696e 6b3a 6872     <use xlink:hr
-00005e30: 6566 3d22 236d 6566 3433 3538 6334 6235  ef="#mef4358c4b5
+00005e30: 6566 3d22 236d 6265 3139 3430 3333 3865  ef="#mbe1940338e
 00005e40: 2220 783d 2234 3134 2e30 3830 3932 3322  " x="414.080923"
 00005e50: 2079 3d22 3230 382e 3939 3837 3134 2220   y="208.998714" 
 00005e60: 7374 796c 653d 2273 7472 6f6b 653a 2023  style="stroke: #
 00005e70: 3030 3030 3030 3b20 7374 726f 6b65 2d77  000000; stroke-w
 00005e80: 6964 7468 3a20 302e 3822 2f3e 0a20 2020  idth: 0.8"/>.   
 00005e90: 2020 203c 2f67 3e0a 2020 2020 203c 2f67     </g>.     </g
 00005ea0: 3e0a 2020 2020 203c 6720 6964 3d22 7465  >.     <g id="te
@@ -1536,15 +1536,15 @@
 00005ff0: 2f3e 0a20 2020 2020 203c 2f67 3e0a 2020  />.      </g>.  
 00006000: 2020 203c 2f67 3e0a 2020 2020 3c2f 673e     </g>.    </g>
 00006010: 0a20 2020 203c 6720 6964 3d22 7874 6963  .    <g id="xtic
 00006020: 6b5f 3233 223e 0a20 2020 2020 3c67 2069  k_23">.     <g i
 00006030: 643d 226c 696e 6532 645f 3233 223e 0a20  d="line2d_23">. 
 00006040: 2020 2020 203c 673e 0a20 2020 2020 2020       <g>.       
 00006050: 3c75 7365 2078 6c69 6e6b 3a68 7265 663d  <use xlink:href=
-00006060: 2223 6d65 6634 3335 3863 3462 3522 2078  "#mef4358c4b5" x
+00006060: 2223 6d62 6531 3934 3033 3338 6522 2078  "#mbe1940338e" x
 00006070: 3d22 3433 312e 3236 3734 3737 2220 793d  ="431.267477" y=
 00006080: 2232 3038 2e39 3938 3731 3422 2073 7479  "208.998714" sty
 00006090: 6c65 3d22 7374 726f 6b65 3a20 2330 3030  le="stroke: #000
 000060a0: 3030 303b 2073 7472 6f6b 652d 7769 6474  000; stroke-widt
 000060b0: 683a 2030 2e38 222f 3e0a 2020 2020 2020  h: 0.8"/>.      
 000060c0: 3c2f 673e 0a20 2020 2020 3c2f 673e 0a20  </g>.     </g>. 
 000060d0: 2020 2020 3c67 2069 643d 2274 6578 745f      <g id="text_
@@ -1571,15 +1571,15 @@
 00006220: 2020 2020 2020 3c2f 673e 0a20 2020 2020        </g>.     
 00006230: 3c2f 673e 0a20 2020 203c 2f67 3e0a 2020  </g>.    </g>.  
 00006240: 2020 3c67 2069 643d 2278 7469 636b 5f32    <g id="xtick_2
 00006250: 3422 3e0a 2020 2020 203c 6720 6964 3d22  4">.     <g id="
 00006260: 6c69 6e65 3264 5f32 3422 3e0a 2020 2020  line2d_24">.    
 00006270: 2020 3c67 3e0a 2020 2020 2020 203c 7573    <g>.       <us
 00006280: 6520 786c 696e 6b3a 6872 6566 3d22 236d  e xlink:href="#m
-00006290: 6566 3433 3538 6334 6235 2220 783d 2234  ef4358c4b5" x="4
+00006290: 6265 3139 3430 3333 3865 2220 783d 2234  be1940338e" x="4
 000062a0: 3438 2e34 3534 3033 3222 2079 3d22 3230  48.454032" y="20
 000062b0: 382e 3939 3837 3134 2220 7374 796c 653d  8.998714" style=
 000062c0: 2273 7472 6f6b 653a 2023 3030 3030 3030  "stroke: #000000
 000062d0: 3b20 7374 726f 6b65 2d77 6964 7468 3a20  ; stroke-width: 
 000062e0: 302e 3822 2f3e 0a20 2020 2020 203c 2f67  0.8"/>.      </g
 000062f0: 3e0a 2020 2020 203c 2f67 3e0a 2020 2020  >.     </g>.    
 00006300: 203c 6720 6964 3d22 7465 7874 5f32 3422   <g id="text_24"
@@ -1605,16 +1605,16 @@
 00006440: 3930 2e38 3639 3134 3122 2f3e 0a20 2020  90.869141"/>.   
 00006450: 2020 203c 2f67 3e0a 2020 2020 203c 2f67     </g>.     </g
 00006460: 3e0a 2020 2020 3c2f 673e 0a20 2020 203c  >.    </g>.    <
 00006470: 6720 6964 3d22 7874 6963 6b5f 3235 223e  g id="xtick_25">
 00006480: 0a20 2020 2020 3c67 2069 643d 226c 696e  .     <g id="lin
 00006490: 6532 645f 3235 223e 0a20 2020 2020 203c  e2d_25">.      <
 000064a0: 673e 0a20 2020 2020 2020 3c75 7365 2078  g>.       <use x
-000064b0: 6c69 6e6b 3a68 7265 663d 2223 6d65 6634  link:href="#mef4
-000064c0: 3335 3863 3462 3522 2078 3d22 3436 352e  358c4b5" x="465.
+000064b0: 6c69 6e6b 3a68 7265 663d 2223 6d62 6531  link:href="#mbe1
+000064c0: 3934 3033 3338 6522 2078 3d22 3436 352e  940338e" x="465.
 000064d0: 3634 3035 3836 2220 793d 2232 3038 2e39  640586" y="208.9
 000064e0: 3938 3731 3422 2073 7479 6c65 3d22 7374  98714" style="st
 000064f0: 726f 6b65 3a20 2330 3030 3030 303b 2073  roke: #000000; s
 00006500: 7472 6f6b 652d 7769 6474 683a 2030 2e38  troke-width: 0.8
 00006510: 222f 3e0a 2020 2020 2020 3c2f 673e 0a20  "/>.      </g>. 
 00006520: 2020 2020 3c2f 673e 0a20 2020 2020 3c67      </g>.     <g
 00006530: 2069 643d 2274 6578 745f 3235 223e 0a20   id="text_25">. 
@@ -1640,16 +1640,16 @@
 00006670: 3836 3931 3431 222f 3e0a 2020 2020 2020  869141"/>.      
 00006680: 3c2f 673e 0a20 2020 2020 3c2f 673e 0a20  </g>.     </g>. 
 00006690: 2020 203c 2f67 3e0a 2020 2020 3c67 2069     </g>.    <g i
 000066a0: 643d 2278 7469 636b 5f32 3622 3e0a 2020  d="xtick_26">.  
 000066b0: 2020 203c 6720 6964 3d22 6c69 6e65 3264     <g id="line2d
 000066c0: 5f32 3622 3e0a 2020 2020 2020 3c67 3e0a  _26">.      <g>.
 000066d0: 2020 2020 2020 203c 7573 6520 786c 696e         <use xlin
-000066e0: 6b3a 6872 6566 3d22 236d 6566 3433 3538  k:href="#mef4358
-000066f0: 6334 6235 2220 783d 2234 3832 2e38 3237  c4b5" x="482.827
+000066e0: 6b3a 6872 6566 3d22 236d 6265 3139 3430  k:href="#mbe1940
+000066f0: 3333 3865 2220 783d 2234 3832 2e38 3237  338e" x="482.827
 00006700: 3134 3122 2079 3d22 3230 382e 3939 3837  141" y="208.9987
 00006710: 3134 2220 7374 796c 653d 2273 7472 6f6b  14" style="strok
 00006720: 653a 2023 3030 3030 3030 3b20 7374 726f  e: #000000; stro
 00006730: 6b65 2d77 6964 7468 3a20 302e 3822 2f3e  ke-width: 0.8"/>
 00006740: 0a20 2020 2020 203c 2f67 3e0a 2020 2020  .      </g>.    
 00006750: 203c 2f67 3e0a 2020 2020 203c 6720 6964   </g>.     <g id
 00006760: 3d22 7465 7874 5f32 3622 3e0a 2020 2020  ="text_26">.    
@@ -1675,15 +1675,15 @@
 000068a0: 3431 222f 3e0a 2020 2020 2020 3c2f 673e  41"/>.      </g>
 000068b0: 0a20 2020 2020 3c2f 673e 0a20 2020 203c  .     </g>.    <
 000068c0: 2f67 3e0a 2020 2020 3c67 2069 643d 2278  /g>.    <g id="x
 000068d0: 7469 636b 5f32 3722 3e0a 2020 2020 203c  tick_27">.     <
 000068e0: 6720 6964 3d22 6c69 6e65 3264 5f32 3722  g id="line2d_27"
 000068f0: 3e0a 2020 2020 2020 3c67 3e0a 2020 2020  >.      <g>.    
 00006900: 2020 203c 7573 6520 786c 696e 6b3a 6872     <use xlink:hr
-00006910: 6566 3d22 236d 6566 3433 3538 6334 6235  ef="#mef4358c4b5
+00006910: 6566 3d22 236d 6265 3139 3430 3333 3865  ef="#mbe1940338e
 00006920: 2220 783d 2235 3030 2e30 3133 3639 3522  " x="500.013695"
 00006930: 2079 3d22 3230 382e 3939 3837 3134 2220   y="208.998714" 
 00006940: 7374 796c 653d 2273 7472 6f6b 653a 2023  style="stroke: #
 00006950: 3030 3030 3030 3b20 7374 726f 6b65 2d77  000000; stroke-w
 00006960: 6964 7468 3a20 302e 3822 2f3e 0a20 2020  idth: 0.8"/>.   
 00006970: 2020 203c 2f67 3e0a 2020 2020 203c 2f67     </g>.     </g
 00006980: 3e0a 2020 2020 203c 6720 6964 3d22 7465  >.     <g id="te
@@ -1710,15 +1710,15 @@
 00006ad0: 2f3e 0a20 2020 2020 203c 2f67 3e0a 2020  />.      </g>.  
 00006ae0: 2020 203c 2f67 3e0a 2020 2020 3c2f 673e     </g>.    </g>
 00006af0: 0a20 2020 203c 6720 6964 3d22 7874 6963  .    <g id="xtic
 00006b00: 6b5f 3238 223e 0a20 2020 2020 3c67 2069  k_28">.     <g i
 00006b10: 643d 226c 696e 6532 645f 3238 223e 0a20  d="line2d_28">. 
 00006b20: 2020 2020 203c 673e 0a20 2020 2020 2020       <g>.       
 00006b30: 3c75 7365 2078 6c69 6e6b 3a68 7265 663d  <use xlink:href=
-00006b40: 2223 6d65 6634 3335 3863 3462 3522 2078  "#mef4358c4b5" x
+00006b40: 2223 6d62 6531 3934 3033 3338 6522 2078  "#mbe1940338e" x
 00006b50: 3d22 3531 372e 3230 3032 3522 2079 3d22  ="517.20025" y="
 00006b60: 3230 382e 3939 3837 3134 2220 7374 796c  208.998714" styl
 00006b70: 653d 2273 7472 6f6b 653a 2023 3030 3030  e="stroke: #0000
 00006b80: 3030 3b20 7374 726f 6b65 2d77 6964 7468  00; stroke-width
 00006b90: 3a20 302e 3822 2f3e 0a20 2020 2020 203c  : 0.8"/>.      <
 00006ba0: 2f67 3e0a 2020 2020 203c 2f67 3e0a 2020  /g>.     </g>.  
 00006bb0: 2020 203c 6720 6964 3d22 7465 7874 5f32     <g id="text_2
@@ -1744,16 +1744,16 @@
 00006cf0: 2231 3930 2e38 3639 3134 3122 2f3e 0a20  "190.869141"/>. 
 00006d00: 2020 2020 203c 2f67 3e0a 2020 2020 203c       </g>.     <
 00006d10: 2f67 3e0a 2020 2020 3c2f 673e 0a20 2020  /g>.    </g>.   
 00006d20: 203c 6720 6964 3d22 7874 6963 6b5f 3239   <g id="xtick_29
 00006d30: 223e 0a20 2020 2020 3c67 2069 643d 226c  ">.     <g id="l
 00006d40: 696e 6532 645f 3239 223e 0a20 2020 2020  ine2d_29">.     
 00006d50: 203c 673e 0a20 2020 2020 2020 3c75 7365   <g>.       <use
-00006d60: 2078 6c69 6e6b 3a68 7265 663d 2223 6d65   xlink:href="#me
-00006d70: 6634 3335 3863 3462 3522 2078 3d22 3533  f4358c4b5" x="53
+00006d60: 2078 6c69 6e6b 3a68 7265 663d 2223 6d62   xlink:href="#mb
+00006d70: 6531 3934 3033 3338 6522 2078 3d22 3533  e1940338e" x="53
 00006d80: 342e 3338 3638 3035 2220 793d 2232 3038  4.386805" y="208
 00006d90: 2e39 3938 3731 3422 2073 7479 6c65 3d22  .998714" style="
 00006da0: 7374 726f 6b65 3a20 2330 3030 3030 303b  stroke: #000000;
 00006db0: 2073 7472 6f6b 652d 7769 6474 683a 2030   stroke-width: 0
 00006dc0: 2e38 222f 3e0a 2020 2020 2020 3c2f 673e  .8"/>.      </g>
 00006dd0: 0a20 2020 2020 3c2f 673e 0a20 2020 2020  .     </g>.     
 00006de0: 3c67 2069 643d 2274 6578 745f 3239 223e  <g id="text_29">
@@ -1779,16 +1779,16 @@
 00006f20: 302e 3836 3931 3431 222f 3e0a 2020 2020  0.869141"/>.    
 00006f30: 2020 3c2f 673e 0a20 2020 2020 3c2f 673e    </g>.     </g>
 00006f40: 0a20 2020 203c 2f67 3e0a 2020 2020 3c67  .    </g>.    <g
 00006f50: 2069 643d 2278 7469 636b 5f33 3022 3e0a   id="xtick_30">.
 00006f60: 2020 2020 203c 6720 6964 3d22 6c69 6e65       <g id="line
 00006f70: 3264 5f33 3022 3e0a 2020 2020 2020 3c67  2d_30">.      <g
 00006f80: 3e0a 2020 2020 2020 203c 7573 6520 786c  >.       <use xl
-00006f90: 696e 6b3a 6872 6566 3d22 236d 6566 3433  ink:href="#mef43
-00006fa0: 3538 6334 6235 2220 783d 2235 3531 2e35  58c4b5" x="551.5
+00006f90: 696e 6b3a 6872 6566 3d22 236d 6265 3139  ink:href="#mbe19
+00006fa0: 3430 3333 3865 2220 783d 2235 3531 2e35  40338e" x="551.5
 00006fb0: 3733 3335 3922 2079 3d22 3230 382e 3939  73359" y="208.99
 00006fc0: 3837 3134 2220 7374 796c 653d 2273 7472  8714" style="str
 00006fd0: 6f6b 653a 2023 3030 3030 3030 3b20 7374  oke: #000000; st
 00006fe0: 726f 6b65 2d77 6964 7468 3a20 302e 3822  roke-width: 0.8"
 00006ff0: 2f3e 0a20 2020 2020 203c 2f67 3e0a 2020  />.      </g>.  
 00007000: 2020 203c 2f67 3e0a 2020 2020 203c 6720     </g>.     <g 
 00007010: 6964 3d22 7465 7874 5f33 3022 3e0a 2020  id="text_30">.  
@@ -1816,24 +1816,24 @@
 00007170: 2020 3c2f 673e 0a20 2020 3c2f 673e 0a20    </g>.   </g>. 
 00007180: 2020 3c67 2069 643d 226d 6174 706c 6f74    <g id="matplot
 00007190: 6c69 622e 6178 6973 5f32 223e 0a20 2020  lib.axis_2">.   
 000071a0: 203c 6720 6964 3d22 7974 6963 6b5f 3122   <g id="ytick_1"
 000071b0: 3e0a 2020 2020 203c 6720 6964 3d22 6c69  >.     <g id="li
 000071c0: 6e65 3264 5f33 3122 3e0a 2020 2020 2020  ne2d_31">.      
 000071d0: 3c64 6566 733e 0a20 2020 2020 2020 3c70  <defs>.       <p
-000071e0: 6174 6820 6964 3d22 6d38 3138 3138 6439  ath id="m81818d9
-000071f0: 3832 3822 2064 3d22 4d20 3020 3020 0a4c  828" d="M 0 0 .L
+000071e0: 6174 6820 6964 3d22 6d35 3637 6662 3464  ath id="m567fb4d
+000071f0: 3861 3422 2064 3d22 4d20 3020 3020 0a4c  8a4" d="M 0 0 .L
 00007200: 202d 332e 3520 3020 0a22 2073 7479 6c65   -3.5 0 ." style
 00007210: 3d22 7374 726f 6b65 3a20 2330 3030 3030  ="stroke: #00000
 00007220: 303b 2073 7472 6f6b 652d 7769 6474 683a  0; stroke-width:
 00007230: 2030 2e38 222f 3e0a 2020 2020 2020 3c2f   0.8"/>.      </
 00007240: 6465 6673 3e0a 2020 2020 2020 3c67 3e0a  defs>.      <g>.
 00007250: 2020 2020 2020 203c 7573 6520 786c 696e         <use xlin
-00007260: 6b3a 6872 6566 3d22 236d 3831 3831 3864  k:href="#m81818d
-00007270: 3938 3238 2220 783d 2234 342e 3537 2220  9828" x="44.57" 
+00007260: 6b3a 6872 6566 3d22 236d 3536 3766 6234  k:href="#m567fb4
+00007270: 6438 6134 2220 783d 2234 342e 3537 2220  d8a4" x="44.57" 
 00007280: 793d 2232 3038 2e39 3938 3731 3422 2073  y="208.998714" s
 00007290: 7479 6c65 3d22 7374 726f 6b65 3a20 2330  tyle="stroke: #0
 000072a0: 3030 3030 303b 2073 7472 6f6b 652d 7769  00000; stroke-wi
 000072b0: 6474 683a 2030 2e38 222f 3e0a 2020 2020  dth: 0.8"/>.    
 000072c0: 2020 3c2f 673e 0a20 2020 2020 3c2f 673e    </g>.     </g>
 000072d0: 0a20 2020 2020 3c67 2069 643d 2274 6578  .     <g id="tex
 000072e0: 745f 3331 223e 0a20 2020 2020 203c 212d  t_31">.      <!-
@@ -1847,15 +1847,15 @@
 00007360: 3330 222f 3e0a 2020 2020 2020 3c2f 673e  30"/>.      </g>
 00007370: 0a20 2020 2020 3c2f 673e 0a20 2020 203c  .     </g>.    <
 00007380: 2f67 3e0a 2020 2020 3c67 2069 643d 2279  /g>.    <g id="y
 00007390: 7469 636b 5f32 223e 0a20 2020 2020 3c67  tick_2">.     <g
 000073a0: 2069 643d 226c 696e 6532 645f 3332 223e   id="line2d_32">
 000073b0: 0a20 2020 2020 203c 673e 0a20 2020 2020  .      <g>.     
 000073c0: 2020 3c75 7365 2078 6c69 6e6b 3a68 7265    <use xlink:hre
-000073d0: 663d 2223 6d38 3138 3138 6439 3832 3822  f="#m81818d9828"
+000073d0: 663d 2223 6d35 3637 6662 3464 3861 3422  f="#m567fb4d8a4"
 000073e0: 2078 3d22 3434 2e35 3722 2079 3d22 3138   x="44.57" y="18
 000073f0: 332e 3439 3138 3932 2220 7374 796c 653d  3.491892" style=
 00007400: 2273 7472 6f6b 653a 2023 3030 3030 3030  "stroke: #000000
 00007410: 3b20 7374 726f 6b65 2d77 6964 7468 3a20  ; stroke-width: 
 00007420: 302e 3822 2f3e 0a20 2020 2020 203c 2f67  0.8"/>.      </g
 00007430: 3e0a 2020 2020 203c 2f67 3e0a 2020 2020  >.     </g>.    
 00007440: 203c 6720 6964 3d22 7465 7874 5f33 3222   <g id="text_32"
@@ -1869,16 +1869,16 @@
 000074c0: 656a 6156 7553 616e 732d 3335 222f 3e0a  ejaVuSans-35"/>.
 000074d0: 2020 2020 2020 3c2f 673e 0a20 2020 2020        </g>.     
 000074e0: 3c2f 673e 0a20 2020 203c 2f67 3e0a 2020  </g>.    </g>.  
 000074f0: 2020 3c67 2069 643d 2279 7469 636b 5f33    <g id="ytick_3
 00007500: 223e 0a20 2020 2020 3c67 2069 643d 226c  ">.     <g id="l
 00007510: 696e 6532 645f 3333 223e 0a20 2020 2020  ine2d_33">.     
 00007520: 203c 673e 0a20 2020 2020 2020 3c75 7365   <g>.       <use
-00007530: 2078 6c69 6e6b 3a68 7265 663d 2223 6d38   xlink:href="#m8
-00007540: 3138 3138 6439 3832 3822 2078 3d22 3434  1818d9828" x="44
+00007530: 2078 6c69 6e6b 3a68 7265 663d 2223 6d35   xlink:href="#m5
+00007540: 3637 6662 3464 3861 3422 2078 3d22 3434  67fb4d8a4" x="44
 00007550: 2e35 3722 2079 3d22 3135 372e 3938 3530  .57" y="157.9850
 00007560: 3639 2220 7374 796c 653d 2273 7472 6f6b  69" style="strok
 00007570: 653a 2023 3030 3030 3030 3b20 7374 726f  e: #000000; stro
 00007580: 6b65 2d77 6964 7468 3a20 302e 3822 2f3e  ke-width: 0.8"/>
 00007590: 0a20 2020 2020 203c 2f67 3e0a 2020 2020  .      </g>.    
 000075a0: 203c 2f67 3e0a 2020 2020 203c 6720 6964   </g>.     <g id
 000075b0: 3d22 7465 7874 5f33 3322 3e0a 2020 2020  ="text_33">.    
@@ -1896,15 +1896,15 @@
 00007670: 2f3e 0a20 2020 2020 203c 2f67 3e0a 2020  />.      </g>.  
 00007680: 2020 203c 2f67 3e0a 2020 2020 3c2f 673e     </g>.    </g>
 00007690: 0a20 2020 203c 6720 6964 3d22 7974 6963  .    <g id="ytic
 000076a0: 6b5f 3422 3e0a 2020 2020 203c 6720 6964  k_4">.     <g id
 000076b0: 3d22 6c69 6e65 3264 5f33 3422 3e0a 2020  ="line2d_34">.  
 000076c0: 2020 2020 3c67 3e0a 2020 2020 2020 203c      <g>.       <
 000076d0: 7573 6520 786c 696e 6b3a 6872 6566 3d22  use xlink:href="
-000076e0: 236d 3831 3831 3864 3938 3238 2220 783d  #m81818d9828" x=
+000076e0: 236d 3536 3766 6234 6438 6134 2220 783d  #m567fb4d8a4" x=
 000076f0: 2234 342e 3537 2220 793d 2231 3332 2e34  "44.57" y="132.4
 00007700: 3738 3234 3622 2073 7479 6c65 3d22 7374  78246" style="st
 00007710: 726f 6b65 3a20 2330 3030 3030 303b 2073  roke: #000000; s
 00007720: 7472 6f6b 652d 7769 6474 683a 2030 2e38  troke-width: 0.8
 00007730: 222f 3e0a 2020 2020 2020 3c2f 673e 0a20  "/>.      </g>. 
 00007740: 2020 2020 3c2f 673e 0a20 2020 2020 3c67      </g>.     <g
 00007750: 2069 643d 2274 6578 745f 3334 223e 0a20   id="text_34">. 
@@ -1922,15 +1922,15 @@
 00007810: 3437 222f 3e0a 2020 2020 2020 3c2f 673e  47"/>.      </g>
 00007820: 0a20 2020 2020 3c2f 673e 0a20 2020 203c  .     </g>.    <
 00007830: 2f67 3e0a 2020 2020 3c67 2069 643d 2279  /g>.    <g id="y
 00007840: 7469 636b 5f35 223e 0a20 2020 2020 3c67  tick_5">.     <g
 00007850: 2069 643d 226c 696e 6532 645f 3335 223e   id="line2d_35">
 00007860: 0a20 2020 2020 203c 673e 0a20 2020 2020  .      <g>.     
 00007870: 2020 3c75 7365 2078 6c69 6e6b 3a68 7265    <use xlink:hre
-00007880: 663d 2223 6d38 3138 3138 6439 3832 3822  f="#m81818d9828"
+00007880: 663d 2223 6d35 3637 6662 3464 3861 3422  f="#m567fb4d8a4"
 00007890: 2078 3d22 3434 2e35 3722 2079 3d22 3130   x="44.57" y="10
 000078a0: 362e 3937 3134 3233 2220 7374 796c 653d  6.971423" style=
 000078b0: 2273 7472 6f6b 653a 2023 3030 3030 3030  "stroke: #000000
 000078c0: 3b20 7374 726f 6b65 2d77 6964 7468 3a20  ; stroke-width: 
 000078d0: 302e 3822 2f3e 0a20 2020 2020 203c 2f67  0.8"/>.      </g
 000078e0: 3e0a 2020 2020 203c 2f67 3e0a 2020 2020  >.     </g>.    
 000078f0: 203c 6720 6964 3d22 7465 7874 5f33 3522   <g id="text_35"
@@ -1948,16 +1948,16 @@
 000079b0: 3233 3034 3722 2f3e 0a20 2020 2020 203c  23047"/>.      <
 000079c0: 2f67 3e0a 2020 2020 203c 2f67 3e0a 2020  /g>.     </g>.  
 000079d0: 2020 3c2f 673e 0a20 2020 203c 6720 6964    </g>.    <g id
 000079e0: 3d22 7974 6963 6b5f 3622 3e0a 2020 2020  ="ytick_6">.    
 000079f0: 203c 6720 6964 3d22 6c69 6e65 3264 5f33   <g id="line2d_3
 00007a00: 3622 3e0a 2020 2020 2020 3c67 3e0a 2020  6">.      <g>.  
 00007a10: 2020 2020 203c 7573 6520 786c 696e 6b3a       <use xlink:
-00007a20: 6872 6566 3d22 236d 3831 3831 3864 3938  href="#m81818d98
-00007a30: 3238 2220 783d 2234 342e 3537 2220 793d  28" x="44.57" y=
+00007a20: 6872 6566 3d22 236d 3536 3766 6234 6438  href="#m567fb4d8
+00007a30: 6134 2220 783d 2234 342e 3537 2220 793d  a4" x="44.57" y=
 00007a40: 2238 312e 3436 3436 3031 2220 7374 796c  "81.464601" styl
 00007a50: 653d 2273 7472 6f6b 653a 2023 3030 3030  e="stroke: #0000
 00007a60: 3030 3b20 7374 726f 6b65 2d77 6964 7468  00; stroke-width
 00007a70: 3a20 302e 3822 2f3e 0a20 2020 2020 203c  : 0.8"/>.      <
 00007a80: 2f67 3e0a 2020 2020 203c 2f67 3e0a 2020  /g>.     </g>.  
 00007a90: 2020 203c 6720 6964 3d22 7465 7874 5f33     <g id="text_3
 00007aa0: 3622 3e0a 2020 2020 2020 3c21 2d2d 2032  6">.      <!-- 2
@@ -1974,16 +1974,16 @@
 00007b50: 3632 3330 3437 222f 3e0a 2020 2020 2020  623047"/>.      
 00007b60: 3c2f 673e 0a20 2020 2020 3c2f 673e 0a20  </g>.     </g>. 
 00007b70: 2020 203c 2f67 3e0a 2020 2020 3c67 2069     </g>.    <g i
 00007b80: 643d 2279 7469 636b 5f37 223e 0a20 2020  d="ytick_7">.   
 00007b90: 2020 3c67 2069 643d 226c 696e 6532 645f    <g id="line2d_
 00007ba0: 3337 223e 0a20 2020 2020 203c 673e 0a20  37">.      <g>. 
 00007bb0: 2020 2020 2020 3c75 7365 2078 6c69 6e6b        <use xlink
-00007bc0: 3a68 7265 663d 2223 6d38 3138 3138 6439  :href="#m81818d9
-00007bd0: 3832 3822 2078 3d22 3434 2e35 3722 2079  828" x="44.57" y
+00007bc0: 3a68 7265 663d 2223 6d35 3637 6662 3464  :href="#m567fb4d
+00007bd0: 3861 3422 2078 3d22 3434 2e35 3722 2079  8a4" x="44.57" y
 00007be0: 3d22 3535 2e39 3537 3737 3822 2073 7479  ="55.957778" sty
 00007bf0: 6c65 3d22 7374 726f 6b65 3a20 2330 3030  le="stroke: #000
 00007c00: 3030 303b 2073 7472 6f6b 652d 7769 6474  000; stroke-widt
 00007c10: 683a 2030 2e38 222f 3e0a 2020 2020 2020  h: 0.8"/>.      
 00007c20: 3c2f 673e 0a20 2020 2020 3c2f 673e 0a20  </g>.     </g>. 
 00007c30: 2020 2020 3c67 2069 643d 2274 6578 745f      <g id="text_
 00007c40: 3337 223e 0a20 2020 2020 203c 212d 2d20  37">.      <!-- 
@@ -2000,16 +2000,16 @@
 00007cf0: 2e36 3233 3034 3722 2f3e 0a20 2020 2020  .623047"/>.     
 00007d00: 203c 2f67 3e0a 2020 2020 203c 2f67 3e0a   </g>.     </g>.
 00007d10: 2020 2020 3c2f 673e 0a20 2020 203c 6720      </g>.    <g 
 00007d20: 6964 3d22 7974 6963 6b5f 3822 3e0a 2020  id="ytick_8">.  
 00007d30: 2020 203c 6720 6964 3d22 6c69 6e65 3264     <g id="line2d
 00007d40: 5f33 3822 3e0a 2020 2020 2020 3c67 3e0a  _38">.      <g>.
 00007d50: 2020 2020 2020 203c 7573 6520 786c 696e         <use xlin
-00007d60: 6b3a 6872 6566 3d22 236d 3831 3831 3864  k:href="#m81818d
-00007d70: 3938 3238 2220 783d 2234 342e 3537 2220  9828" x="44.57" 
+00007d60: 6b3a 6872 6566 3d22 236d 3536 3766 6234  k:href="#m567fb4
+00007d70: 6438 6134 2220 783d 2234 342e 3537 2220  d8a4" x="44.57" 
 00007d80: 793d 2233 302e 3435 3039 3535 2220 7374  y="30.450955" st
 00007d90: 796c 653d 2273 7472 6f6b 653a 2023 3030  yle="stroke: #00
 00007da0: 3030 3030 3b20 7374 726f 6b65 2d77 6964  0000; stroke-wid
 00007db0: 7468 3a20 302e 3822 2f3e 0a20 2020 2020  th: 0.8"/>.     
 00007dc0: 203c 2f67 3e0a 2020 2020 203c 2f67 3e0a   </g>.     </g>.
 00007dd0: 2020 2020 203c 6720 6964 3d22 7465 7874       <g id="text
 00007de0: 5f33 3822 3e0a 2020 2020 2020 3c21 2d2d  _38">.      <!--
@@ -2354,289 +2354,289 @@
 00009310: 6b3a 6872 6566 3d22 2344 656a 6156 7553  k:href="#DejaVuS
 00009320: 616e 732d 3733 2220 783d 2235 3438 2e37  ans-73" x="548.7
 00009330: 3837 3130 3922 2f3e 0a20 2020 2020 3c2f  87109"/>.     </
 00009340: 673e 0a20 2020 203c 2f67 3e0a 2020 203c  g>.    </g>.   <
 00009350: 2f67 3e0a 2020 203c 6720 6964 3d22 6c69  /g>.   <g id="li
 00009360: 6e65 3264 5f33 3922 3e0a 2020 2020 3c70  ne2d_39">.    <p
 00009370: 6174 6820 636c 6970 2d70 6174 683d 2275  ath clip-path="u
-00009380: 726c 2823 7061 3237 6633 6335 3633 6129  rl(#pa27f3c563a)
+00009380: 726c 2823 7030 3365 3933 3839 6638 3829  rl(#p03e9389f88)
 00009390: 2220 7374 796c 653d 2266 696c 6c3a 206e  " style="fill: n
 000093a0: 6f6e 653b 2073 7472 6f6b 653a 2023 3432  one; stroke: #42
 000093b0: 3432 3432 3b20 7374 726f 6b65 2d77 6964  4242; stroke-wid
 000093c0: 7468 3a20 322e 373b 2073 7472 6f6b 652d  th: 2.7; stroke-
 000093d0: 6c69 6e65 6361 703a 2073 7175 6172 6522  linecap: square"
 000093e0: 2f3e 0a20 2020 3c2f 673e 0a20 2020 3c67  />.   </g>.   <g
 000093f0: 2069 643d 226c 696e 6532 645f 3430 223e   id="line2d_40">
 00009400: 0a20 2020 203c 7061 7468 2063 6c69 702d  .    <path clip-
-00009410: 7061 7468 3d22 7572 6c28 2370 6132 3766  path="url(#pa27f
-00009420: 3363 3536 3361 2922 2073 7479 6c65 3d22  3c563a)" style="
+00009410: 7061 7468 3d22 7572 6c28 2370 3033 6539  path="url(#p03e9
+00009420: 3338 3966 3838 2922 2073 7479 6c65 3d22  389f88)" style="
 00009430: 6669 6c6c 3a20 6e6f 6e65 3b20 7374 726f  fill: none; stro
 00009440: 6b65 3a20 2334 3234 3234 323b 2073 7472  ke: #424242; str
 00009450: 6f6b 652d 7769 6474 683a 2032 2e37 3b20  oke-width: 2.7; 
 00009460: 7374 726f 6b65 2d6c 696e 6563 6170 3a20  stroke-linecap: 
 00009470: 7371 7561 7265 222f 3e0a 2020 203c 2f67  square"/>.   </g
 00009480: 3e0a 2020 203c 6720 6964 3d22 6c69 6e65  >.   <g id="line
 00009490: 3264 5f34 3122 3e0a 2020 2020 3c70 6174  2d_41">.    <pat
 000094a0: 6820 636c 6970 2d70 6174 683d 2275 726c  h clip-path="url
-000094b0: 2823 7061 3237 6633 6335 3633 6129 2220  (#pa27f3c563a)" 
+000094b0: 2823 7030 3365 3933 3839 6638 3829 2220  (#p03e9389f88)" 
 000094c0: 7374 796c 653d 2266 696c 6c3a 206e 6f6e  style="fill: non
 000094d0: 653b 2073 7472 6f6b 653a 2023 3432 3432  e; stroke: #4242
 000094e0: 3432 3b20 7374 726f 6b65 2d77 6964 7468  42; stroke-width
 000094f0: 3a20 322e 373b 2073 7472 6f6b 652d 6c69  : 2.7; stroke-li
 00009500: 6e65 6361 703a 2073 7175 6172 6522 2f3e  necap: square"/>
 00009510: 0a20 2020 3c2f 673e 0a20 2020 3c67 2069  .   </g>.   <g i
 00009520: 643d 226c 696e 6532 645f 3432 223e 0a20  d="line2d_42">. 
 00009530: 2020 203c 7061 7468 2063 6c69 702d 7061     <path clip-pa
-00009540: 7468 3d22 7572 6c28 2370 6132 3766 3363  th="url(#pa27f3c
-00009550: 3536 3361 2922 2073 7479 6c65 3d22 6669  563a)" style="fi
+00009540: 7468 3d22 7572 6c28 2370 3033 6539 3338  th="url(#p03e938
+00009550: 3966 3838 2922 2073 7479 6c65 3d22 6669  9f88)" style="fi
 00009560: 6c6c 3a20 6e6f 6e65 3b20 7374 726f 6b65  ll: none; stroke
 00009570: 3a20 2334 3234 3234 323b 2073 7472 6f6b  : #424242; strok
 00009580: 652d 7769 6474 683a 2032 2e37 3b20 7374  e-width: 2.7; st
 00009590: 726f 6b65 2d6c 696e 6563 6170 3a20 7371  roke-linecap: sq
 000095a0: 7561 7265 222f 3e0a 2020 203c 2f67 3e0a  uare"/>.   </g>.
 000095b0: 2020 203c 6720 6964 3d22 6c69 6e65 3264     <g id="line2d
 000095c0: 5f34 3322 3e0a 2020 2020 3c70 6174 6820  _43">.    <path 
 000095d0: 636c 6970 2d70 6174 683d 2275 726c 2823  clip-path="url(#
-000095e0: 7061 3237 6633 6335 3633 6129 2220 7374  pa27f3c563a)" st
+000095e0: 7030 3365 3933 3839 6638 3829 2220 7374  p03e9389f88)" st
 000095f0: 796c 653d 2266 696c 6c3a 206e 6f6e 653b  yle="fill: none;
 00009600: 2073 7472 6f6b 653a 2023 3432 3432 3432   stroke: #424242
 00009610: 3b20 7374 726f 6b65 2d77 6964 7468 3a20  ; stroke-width: 
 00009620: 322e 373b 2073 7472 6f6b 652d 6c69 6e65  2.7; stroke-line
 00009630: 6361 703a 2073 7175 6172 6522 2f3e 0a20  cap: square"/>. 
 00009640: 2020 3c2f 673e 0a20 2020 3c67 2069 643d    </g>.   <g id=
 00009650: 226c 696e 6532 645f 3434 223e 0a20 2020  "line2d_44">.   
 00009660: 203c 7061 7468 2063 6c69 702d 7061 7468   <path clip-path
-00009670: 3d22 7572 6c28 2370 6132 3766 3363 3536  ="url(#pa27f3c56
-00009680: 3361 2922 2073 7479 6c65 3d22 6669 6c6c  3a)" style="fill
+00009670: 3d22 7572 6c28 2370 3033 6539 3338 3966  ="url(#p03e9389f
+00009680: 3838 2922 2073 7479 6c65 3d22 6669 6c6c  88)" style="fill
 00009690: 3a20 6e6f 6e65 3b20 7374 726f 6b65 3a20  : none; stroke: 
 000096a0: 2334 3234 3234 323b 2073 7472 6f6b 652d  #424242; stroke-
 000096b0: 7769 6474 683a 2032 2e37 3b20 7374 726f  width: 2.7; stro
 000096c0: 6b65 2d6c 696e 6563 6170 3a20 7371 7561  ke-linecap: squa
 000096d0: 7265 222f 3e0a 2020 203c 2f67 3e0a 2020  re"/>.   </g>.  
 000096e0: 203c 6720 6964 3d22 6c69 6e65 3264 5f34   <g id="line2d_4
 000096f0: 3522 3e0a 2020 2020 3c70 6174 6820 636c  5">.    <path cl
-00009700: 6970 2d70 6174 683d 2275 726c 2823 7061  ip-path="url(#pa
-00009710: 3237 6633 6335 3633 6129 2220 7374 796c  27f3c563a)" styl
+00009700: 6970 2d70 6174 683d 2275 726c 2823 7030  ip-path="url(#p0
+00009710: 3365 3933 3839 6638 3829 2220 7374 796c  3e9389f88)" styl
 00009720: 653d 2266 696c 6c3a 206e 6f6e 653b 2073  e="fill: none; s
 00009730: 7472 6f6b 653a 2023 3432 3432 3432 3b20  troke: #424242; 
 00009740: 7374 726f 6b65 2d77 6964 7468 3a20 322e  stroke-width: 2.
 00009750: 373b 2073 7472 6f6b 652d 6c69 6e65 6361  7; stroke-lineca
 00009760: 703a 2073 7175 6172 6522 2f3e 0a20 2020  p: square"/>.   
 00009770: 3c2f 673e 0a20 2020 3c67 2069 643d 226c  </g>.   <g id="l
 00009780: 696e 6532 645f 3436 223e 0a20 2020 203c  ine2d_46">.    <
 00009790: 7061 7468 2063 6c69 702d 7061 7468 3d22  path clip-path="
-000097a0: 7572 6c28 2370 6132 3766 3363 3536 3361  url(#pa27f3c563a
+000097a0: 7572 6c28 2370 3033 6539 3338 3966 3838  url(#p03e9389f88
 000097b0: 2922 2073 7479 6c65 3d22 6669 6c6c 3a20  )" style="fill: 
 000097c0: 6e6f 6e65 3b20 7374 726f 6b65 3a20 2334  none; stroke: #4
 000097d0: 3234 3234 323b 2073 7472 6f6b 652d 7769  24242; stroke-wi
 000097e0: 6474 683a 2032 2e37 3b20 7374 726f 6b65  dth: 2.7; stroke
 000097f0: 2d6c 696e 6563 6170 3a20 7371 7561 7265  -linecap: square
 00009800: 222f 3e0a 2020 203c 2f67 3e0a 2020 203c  "/>.   </g>.   <
 00009810: 6720 6964 3d22 6c69 6e65 3264 5f34 3722  g id="line2d_47"
 00009820: 3e0a 2020 2020 3c70 6174 6820 636c 6970  >.    <path clip
-00009830: 2d70 6174 683d 2275 726c 2823 7061 3237  -path="url(#pa27
-00009840: 6633 6335 3633 6129 2220 7374 796c 653d  f3c563a)" style=
+00009830: 2d70 6174 683d 2275 726c 2823 7030 3365  -path="url(#p03e
+00009840: 3933 3839 6638 3829 2220 7374 796c 653d  9389f88)" style=
 00009850: 2266 696c 6c3a 206e 6f6e 653b 2073 7472  "fill: none; str
 00009860: 6f6b 653a 2023 3432 3432 3432 3b20 7374  oke: #424242; st
 00009870: 726f 6b65 2d77 6964 7468 3a20 322e 373b  roke-width: 2.7;
 00009880: 2073 7472 6f6b 652d 6c69 6e65 6361 703a   stroke-linecap:
 00009890: 2073 7175 6172 6522 2f3e 0a20 2020 3c2f   square"/>.   </
 000098a0: 673e 0a20 2020 3c67 2069 643d 226c 696e  g>.   <g id="lin
 000098b0: 6532 645f 3438 223e 0a20 2020 203c 7061  e2d_48">.    <pa
 000098c0: 7468 2063 6c69 702d 7061 7468 3d22 7572  th clip-path="ur
-000098d0: 6c28 2370 6132 3766 3363 3536 3361 2922  l(#pa27f3c563a)"
+000098d0: 6c28 2370 3033 6539 3338 3966 3838 2922  l(#p03e9389f88)"
 000098e0: 2073 7479 6c65 3d22 6669 6c6c 3a20 6e6f   style="fill: no
 000098f0: 6e65 3b20 7374 726f 6b65 3a20 2334 3234  ne; stroke: #424
 00009900: 3234 323b 2073 7472 6f6b 652d 7769 6474  242; stroke-widt
 00009910: 683a 2032 2e37 3b20 7374 726f 6b65 2d6c  h: 2.7; stroke-l
 00009920: 696e 6563 6170 3a20 7371 7561 7265 222f  inecap: square"/
 00009930: 3e0a 2020 203c 2f67 3e0a 2020 203c 6720  >.   </g>.   <g 
 00009940: 6964 3d22 6c69 6e65 3264 5f34 3922 3e0a  id="line2d_49">.
 00009950: 2020 2020 3c70 6174 6820 636c 6970 2d70      <path clip-p
-00009960: 6174 683d 2275 726c 2823 7061 3237 6633  ath="url(#pa27f3
-00009970: 6335 3633 6129 2220 7374 796c 653d 2266  c563a)" style="f
+00009960: 6174 683d 2275 726c 2823 7030 3365 3933  ath="url(#p03e93
+00009970: 3839 6638 3829 2220 7374 796c 653d 2266  89f88)" style="f
 00009980: 696c 6c3a 206e 6f6e 653b 2073 7472 6f6b  ill: none; strok
 00009990: 653a 2023 3432 3432 3432 3b20 7374 726f  e: #424242; stro
 000099a0: 6b65 2d77 6964 7468 3a20 322e 373b 2073  ke-width: 2.7; s
 000099b0: 7472 6f6b 652d 6c69 6e65 6361 703a 2073  troke-linecap: s
 000099c0: 7175 6172 6522 2f3e 0a20 2020 3c2f 673e  quare"/>.   </g>
 000099d0: 0a20 2020 3c67 2069 643d 226c 696e 6532  .   <g id="line2
 000099e0: 645f 3530 223e 0a20 2020 203c 7061 7468  d_50">.    <path
 000099f0: 2063 6c69 702d 7061 7468 3d22 7572 6c28   clip-path="url(
-00009a00: 2370 6132 3766 3363 3536 3361 2922 2073  #pa27f3c563a)" s
+00009a00: 2370 3033 6539 3338 3966 3838 2922 2073  #p03e9389f88)" s
 00009a10: 7479 6c65 3d22 6669 6c6c 3a20 6e6f 6e65  tyle="fill: none
 00009a20: 3b20 7374 726f 6b65 3a20 2334 3234 3234  ; stroke: #42424
 00009a30: 323b 2073 7472 6f6b 652d 7769 6474 683a  2; stroke-width:
 00009a40: 2032 2e37 3b20 7374 726f 6b65 2d6c 696e   2.7; stroke-lin
 00009a50: 6563 6170 3a20 7371 7561 7265 222f 3e0a  ecap: square"/>.
 00009a60: 2020 203c 2f67 3e0a 2020 203c 6720 6964     </g>.   <g id
 00009a70: 3d22 6c69 6e65 3264 5f35 3122 3e0a 2020  ="line2d_51">.  
 00009a80: 2020 3c70 6174 6820 636c 6970 2d70 6174    <path clip-pat
-00009a90: 683d 2275 726c 2823 7061 3237 6633 6335  h="url(#pa27f3c5
-00009aa0: 3633 6129 2220 7374 796c 653d 2266 696c  63a)" style="fil
+00009a90: 683d 2275 726c 2823 7030 3365 3933 3839  h="url(#p03e9389
+00009aa0: 6638 3829 2220 7374 796c 653d 2266 696c  f88)" style="fil
 00009ab0: 6c3a 206e 6f6e 653b 2073 7472 6f6b 653a  l: none; stroke:
 00009ac0: 2023 3432 3432 3432 3b20 7374 726f 6b65   #424242; stroke
 00009ad0: 2d77 6964 7468 3a20 322e 373b 2073 7472  -width: 2.7; str
 00009ae0: 6f6b 652d 6c69 6e65 6361 703a 2073 7175  oke-linecap: squ
 00009af0: 6172 6522 2f3e 0a20 2020 3c2f 673e 0a20  are"/>.   </g>. 
 00009b00: 2020 3c67 2069 643d 226c 696e 6532 645f    <g id="line2d_
 00009b10: 3532 223e 0a20 2020 203c 7061 7468 2063  52">.    <path c
 00009b20: 6c69 702d 7061 7468 3d22 7572 6c28 2370  lip-path="url(#p
-00009b30: 6132 3766 3363 3536 3361 2922 2073 7479  a27f3c563a)" sty
+00009b30: 3033 6539 3338 3966 3838 2922 2073 7479  03e9389f88)" sty
 00009b40: 6c65 3d22 6669 6c6c 3a20 6e6f 6e65 3b20  le="fill: none; 
 00009b50: 7374 726f 6b65 3a20 2334 3234 3234 323b  stroke: #424242;
 00009b60: 2073 7472 6f6b 652d 7769 6474 683a 2032   stroke-width: 2
 00009b70: 2e37 3b20 7374 726f 6b65 2d6c 696e 6563  .7; stroke-linec
 00009b80: 6170 3a20 7371 7561 7265 222f 3e0a 2020  ap: square"/>.  
 00009b90: 203c 2f67 3e0a 2020 203c 6720 6964 3d22   </g>.   <g id="
 00009ba0: 6c69 6e65 3264 5f35 3322 3e0a 2020 2020  line2d_53">.    
 00009bb0: 3c70 6174 6820 636c 6970 2d70 6174 683d  <path clip-path=
-00009bc0: 2275 726c 2823 7061 3237 6633 6335 3633  "url(#pa27f3c563
-00009bd0: 6129 2220 7374 796c 653d 2266 696c 6c3a  a)" style="fill:
+00009bc0: 2275 726c 2823 7030 3365 3933 3839 6638  "url(#p03e9389f8
+00009bd0: 3829 2220 7374 796c 653d 2266 696c 6c3a  8)" style="fill:
 00009be0: 206e 6f6e 653b 2073 7472 6f6b 653a 2023   none; stroke: #
 00009bf0: 3432 3432 3432 3b20 7374 726f 6b65 2d77  424242; stroke-w
 00009c00: 6964 7468 3a20 322e 373b 2073 7472 6f6b  idth: 2.7; strok
 00009c10: 652d 6c69 6e65 6361 703a 2073 7175 6172  e-linecap: squar
 00009c20: 6522 2f3e 0a20 2020 3c2f 673e 0a20 2020  e"/>.   </g>.   
 00009c30: 3c67 2069 643d 226c 696e 6532 645f 3534  <g id="line2d_54
 00009c40: 223e 0a20 2020 203c 7061 7468 2063 6c69  ">.    <path cli
-00009c50: 702d 7061 7468 3d22 7572 6c28 2370 6132  p-path="url(#pa2
-00009c60: 3766 3363 3536 3361 2922 2073 7479 6c65  7f3c563a)" style
+00009c50: 702d 7061 7468 3d22 7572 6c28 2370 3033  p-path="url(#p03
+00009c60: 6539 3338 3966 3838 2922 2073 7479 6c65  e9389f88)" style
 00009c70: 3d22 6669 6c6c 3a20 6e6f 6e65 3b20 7374  ="fill: none; st
 00009c80: 726f 6b65 3a20 2334 3234 3234 323b 2073  roke: #424242; s
 00009c90: 7472 6f6b 652d 7769 6474 683a 2032 2e37  troke-width: 2.7
 00009ca0: 3b20 7374 726f 6b65 2d6c 696e 6563 6170  ; stroke-linecap
 00009cb0: 3a20 7371 7561 7265 222f 3e0a 2020 203c  : square"/>.   <
 00009cc0: 2f67 3e0a 2020 203c 6720 6964 3d22 6c69  /g>.   <g id="li
 00009cd0: 6e65 3264 5f35 3522 3e0a 2020 2020 3c70  ne2d_55">.    <p
 00009ce0: 6174 6820 636c 6970 2d70 6174 683d 2275  ath clip-path="u
-00009cf0: 726c 2823 7061 3237 6633 6335 3633 6129  rl(#pa27f3c563a)
+00009cf0: 726c 2823 7030 3365 3933 3839 6638 3829  rl(#p03e9389f88)
 00009d00: 2220 7374 796c 653d 2266 696c 6c3a 206e  " style="fill: n
 00009d10: 6f6e 653b 2073 7472 6f6b 653a 2023 3432  one; stroke: #42
 00009d20: 3432 3432 3b20 7374 726f 6b65 2d77 6964  4242; stroke-wid
 00009d30: 7468 3a20 322e 373b 2073 7472 6f6b 652d  th: 2.7; stroke-
 00009d40: 6c69 6e65 6361 703a 2073 7175 6172 6522  linecap: square"
 00009d50: 2f3e 0a20 2020 3c2f 673e 0a20 2020 3c67  />.   </g>.   <g
 00009d60: 2069 643d 226c 696e 6532 645f 3536 223e   id="line2d_56">
 00009d70: 0a20 2020 203c 7061 7468 2063 6c69 702d  .    <path clip-
-00009d80: 7061 7468 3d22 7572 6c28 2370 6132 3766  path="url(#pa27f
-00009d90: 3363 3536 3361 2922 2073 7479 6c65 3d22  3c563a)" style="
+00009d80: 7061 7468 3d22 7572 6c28 2370 3033 6539  path="url(#p03e9
+00009d90: 3338 3966 3838 2922 2073 7479 6c65 3d22  389f88)" style="
 00009da0: 6669 6c6c 3a20 6e6f 6e65 3b20 7374 726f  fill: none; stro
 00009db0: 6b65 3a20 2334 3234 3234 323b 2073 7472  ke: #424242; str
 00009dc0: 6f6b 652d 7769 6474 683a 2032 2e37 3b20  oke-width: 2.7; 
 00009dd0: 7374 726f 6b65 2d6c 696e 6563 6170 3a20  stroke-linecap: 
 00009de0: 7371 7561 7265 222f 3e0a 2020 203c 2f67  square"/>.   </g
 00009df0: 3e0a 2020 203c 6720 6964 3d22 6c69 6e65  >.   <g id="line
 00009e00: 3264 5f35 3722 3e0a 2020 2020 3c70 6174  2d_57">.    <pat
 00009e10: 6820 636c 6970 2d70 6174 683d 2275 726c  h clip-path="url
-00009e20: 2823 7061 3237 6633 6335 3633 6129 2220  (#pa27f3c563a)" 
+00009e20: 2823 7030 3365 3933 3839 6638 3829 2220  (#p03e9389f88)" 
 00009e30: 7374 796c 653d 2266 696c 6c3a 206e 6f6e  style="fill: non
 00009e40: 653b 2073 7472 6f6b 653a 2023 3432 3432  e; stroke: #4242
 00009e50: 3432 3b20 7374 726f 6b65 2d77 6964 7468  42; stroke-width
 00009e60: 3a20 322e 373b 2073 7472 6f6b 652d 6c69  : 2.7; stroke-li
 00009e70: 6e65 6361 703a 2073 7175 6172 6522 2f3e  necap: square"/>
 00009e80: 0a20 2020 3c2f 673e 0a20 2020 3c67 2069  .   </g>.   <g i
 00009e90: 643d 226c 696e 6532 645f 3538 223e 0a20  d="line2d_58">. 
 00009ea0: 2020 203c 7061 7468 2063 6c69 702d 7061     <path clip-pa
-00009eb0: 7468 3d22 7572 6c28 2370 6132 3766 3363  th="url(#pa27f3c
-00009ec0: 3536 3361 2922 2073 7479 6c65 3d22 6669  563a)" style="fi
+00009eb0: 7468 3d22 7572 6c28 2370 3033 6539 3338  th="url(#p03e938
+00009ec0: 3966 3838 2922 2073 7479 6c65 3d22 6669  9f88)" style="fi
 00009ed0: 6c6c 3a20 6e6f 6e65 3b20 7374 726f 6b65  ll: none; stroke
 00009ee0: 3a20 2334 3234 3234 323b 2073 7472 6f6b  : #424242; strok
 00009ef0: 652d 7769 6474 683a 2032 2e37 3b20 7374  e-width: 2.7; st
 00009f00: 726f 6b65 2d6c 696e 6563 6170 3a20 7371  roke-linecap: sq
 00009f10: 7561 7265 222f 3e0a 2020 203c 2f67 3e0a  uare"/>.   </g>.
 00009f20: 2020 203c 6720 6964 3d22 6c69 6e65 3264     <g id="line2d
 00009f30: 5f35 3922 3e0a 2020 2020 3c70 6174 6820  _59">.    <path 
 00009f40: 636c 6970 2d70 6174 683d 2275 726c 2823  clip-path="url(#
-00009f50: 7061 3237 6633 6335 3633 6129 2220 7374  pa27f3c563a)" st
+00009f50: 7030 3365 3933 3839 6638 3829 2220 7374  p03e9389f88)" st
 00009f60: 796c 653d 2266 696c 6c3a 206e 6f6e 653b  yle="fill: none;
 00009f70: 2073 7472 6f6b 653a 2023 3432 3432 3432   stroke: #424242
 00009f80: 3b20 7374 726f 6b65 2d77 6964 7468 3a20  ; stroke-width: 
 00009f90: 322e 373b 2073 7472 6f6b 652d 6c69 6e65  2.7; stroke-line
 00009fa0: 6361 703a 2073 7175 6172 6522 2f3e 0a20  cap: square"/>. 
 00009fb0: 2020 3c2f 673e 0a20 2020 3c67 2069 643d    </g>.   <g id=
 00009fc0: 226c 696e 6532 645f 3630 223e 0a20 2020  "line2d_60">.   
 00009fd0: 203c 7061 7468 2063 6c69 702d 7061 7468   <path clip-path
-00009fe0: 3d22 7572 6c28 2370 6132 3766 3363 3536  ="url(#pa27f3c56
-00009ff0: 3361 2922 2073 7479 6c65 3d22 6669 6c6c  3a)" style="fill
+00009fe0: 3d22 7572 6c28 2370 3033 6539 3338 3966  ="url(#p03e9389f
+00009ff0: 3838 2922 2073 7479 6c65 3d22 6669 6c6c  88)" style="fill
 0000a000: 3a20 6e6f 6e65 3b20 7374 726f 6b65 3a20  : none; stroke: 
 0000a010: 2334 3234 3234 323b 2073 7472 6f6b 652d  #424242; stroke-
 0000a020: 7769 6474 683a 2032 2e37 3b20 7374 726f  width: 2.7; stro
 0000a030: 6b65 2d6c 696e 6563 6170 3a20 7371 7561  ke-linecap: squa
 0000a040: 7265 222f 3e0a 2020 203c 2f67 3e0a 2020  re"/>.   </g>.  
 0000a050: 203c 6720 6964 3d22 6c69 6e65 3264 5f36   <g id="line2d_6
 0000a060: 3122 3e0a 2020 2020 3c70 6174 6820 636c  1">.    <path cl
-0000a070: 6970 2d70 6174 683d 2275 726c 2823 7061  ip-path="url(#pa
-0000a080: 3237 6633 6335 3633 6129 2220 7374 796c  27f3c563a)" styl
+0000a070: 6970 2d70 6174 683d 2275 726c 2823 7030  ip-path="url(#p0
+0000a080: 3365 3933 3839 6638 3829 2220 7374 796c  3e9389f88)" styl
 0000a090: 653d 2266 696c 6c3a 206e 6f6e 653b 2073  e="fill: none; s
 0000a0a0: 7472 6f6b 653a 2023 3432 3432 3432 3b20  troke: #424242; 
 0000a0b0: 7374 726f 6b65 2d77 6964 7468 3a20 322e  stroke-width: 2.
 0000a0c0: 373b 2073 7472 6f6b 652d 6c69 6e65 6361  7; stroke-lineca
 0000a0d0: 703a 2073 7175 6172 6522 2f3e 0a20 2020  p: square"/>.   
 0000a0e0: 3c2f 673e 0a20 2020 3c67 2069 643d 226c  </g>.   <g id="l
 0000a0f0: 696e 6532 645f 3632 223e 0a20 2020 203c  ine2d_62">.    <
 0000a100: 7061 7468 2063 6c69 702d 7061 7468 3d22  path clip-path="
-0000a110: 7572 6c28 2370 6132 3766 3363 3536 3361  url(#pa27f3c563a
+0000a110: 7572 6c28 2370 3033 6539 3338 3966 3838  url(#p03e9389f88
 0000a120: 2922 2073 7479 6c65 3d22 6669 6c6c 3a20  )" style="fill: 
 0000a130: 6e6f 6e65 3b20 7374 726f 6b65 3a20 2334  none; stroke: #4
 0000a140: 3234 3234 323b 2073 7472 6f6b 652d 7769  24242; stroke-wi
 0000a150: 6474 683a 2032 2e37 3b20 7374 726f 6b65  dth: 2.7; stroke
 0000a160: 2d6c 696e 6563 6170 3a20 7371 7561 7265  -linecap: square
 0000a170: 222f 3e0a 2020 203c 2f67 3e0a 2020 203c  "/>.   </g>.   <
 0000a180: 6720 6964 3d22 6c69 6e65 3264 5f36 3322  g id="line2d_63"
 0000a190: 3e0a 2020 2020 3c70 6174 6820 636c 6970  >.    <path clip
-0000a1a0: 2d70 6174 683d 2275 726c 2823 7061 3237  -path="url(#pa27
-0000a1b0: 6633 6335 3633 6129 2220 7374 796c 653d  f3c563a)" style=
+0000a1a0: 2d70 6174 683d 2275 726c 2823 7030 3365  -path="url(#p03e
+0000a1b0: 3933 3839 6638 3829 2220 7374 796c 653d  9389f88)" style=
 0000a1c0: 2266 696c 6c3a 206e 6f6e 653b 2073 7472  "fill: none; str
 0000a1d0: 6f6b 653a 2023 3432 3432 3432 3b20 7374  oke: #424242; st
 0000a1e0: 726f 6b65 2d77 6964 7468 3a20 322e 373b  roke-width: 2.7;
 0000a1f0: 2073 7472 6f6b 652d 6c69 6e65 6361 703a   stroke-linecap:
 0000a200: 2073 7175 6172 6522 2f3e 0a20 2020 3c2f   square"/>.   </
 0000a210: 673e 0a20 2020 3c67 2069 643d 226c 696e  g>.   <g id="lin
 0000a220: 6532 645f 3634 223e 0a20 2020 203c 7061  e2d_64">.    <pa
 0000a230: 7468 2063 6c69 702d 7061 7468 3d22 7572  th clip-path="ur
-0000a240: 6c28 2370 6132 3766 3363 3536 3361 2922  l(#pa27f3c563a)"
+0000a240: 6c28 2370 3033 6539 3338 3966 3838 2922  l(#p03e9389f88)"
 0000a250: 2073 7479 6c65 3d22 6669 6c6c 3a20 6e6f   style="fill: no
 0000a260: 6e65 3b20 7374 726f 6b65 3a20 2334 3234  ne; stroke: #424
 0000a270: 3234 323b 2073 7472 6f6b 652d 7769 6474  242; stroke-widt
 0000a280: 683a 2032 2e37 3b20 7374 726f 6b65 2d6c  h: 2.7; stroke-l
 0000a290: 696e 6563 6170 3a20 7371 7561 7265 222f  inecap: square"/
 0000a2a0: 3e0a 2020 203c 2f67 3e0a 2020 203c 6720  >.   </g>.   <g 
 0000a2b0: 6964 3d22 6c69 6e65 3264 5f36 3522 3e0a  id="line2d_65">.
 0000a2c0: 2020 2020 3c70 6174 6820 636c 6970 2d70      <path clip-p
-0000a2d0: 6174 683d 2275 726c 2823 7061 3237 6633  ath="url(#pa27f3
-0000a2e0: 6335 3633 6129 2220 7374 796c 653d 2266  c563a)" style="f
+0000a2d0: 6174 683d 2275 726c 2823 7030 3365 3933  ath="url(#p03e93
+0000a2e0: 3839 6638 3829 2220 7374 796c 653d 2266  89f88)" style="f
 0000a2f0: 696c 6c3a 206e 6f6e 653b 2073 7472 6f6b  ill: none; strok
 0000a300: 653a 2023 3432 3432 3432 3b20 7374 726f  e: #424242; stro
 0000a310: 6b65 2d77 6964 7468 3a20 322e 373b 2073  ke-width: 2.7; s
 0000a320: 7472 6f6b 652d 6c69 6e65 6361 703a 2073  troke-linecap: s
 0000a330: 7175 6172 6522 2f3e 0a20 2020 3c2f 673e  quare"/>.   </g>
 0000a340: 0a20 2020 3c67 2069 643d 226c 696e 6532  .   <g id="line2
 0000a350: 645f 3636 223e 0a20 2020 203c 7061 7468  d_66">.    <path
 0000a360: 2063 6c69 702d 7061 7468 3d22 7572 6c28   clip-path="url(
-0000a370: 2370 6132 3766 3363 3536 3361 2922 2073  #pa27f3c563a)" s
+0000a370: 2370 3033 6539 3338 3966 3838 2922 2073  #p03e9389f88)" s
 0000a380: 7479 6c65 3d22 6669 6c6c 3a20 6e6f 6e65  tyle="fill: none
 0000a390: 3b20 7374 726f 6b65 3a20 2334 3234 3234  ; stroke: #42424
 0000a3a0: 323b 2073 7472 6f6b 652d 7769 6474 683a  2; stroke-width:
 0000a3b0: 2032 2e37 3b20 7374 726f 6b65 2d6c 696e   2.7; stroke-lin
 0000a3c0: 6563 6170 3a20 7371 7561 7265 222f 3e0a  ecap: square"/>.
 0000a3d0: 2020 203c 2f67 3e0a 2020 203c 6720 6964     </g>.   <g id
 0000a3e0: 3d22 6c69 6e65 3264 5f36 3722 3e0a 2020  ="line2d_67">.  
 0000a3f0: 2020 3c70 6174 6820 636c 6970 2d70 6174    <path clip-pat
-0000a400: 683d 2275 726c 2823 7061 3237 6633 6335  h="url(#pa27f3c5
-0000a410: 3633 6129 2220 7374 796c 653d 2266 696c  63a)" style="fil
+0000a400: 683d 2275 726c 2823 7030 3365 3933 3839  h="url(#p03e9389
+0000a410: 6638 3829 2220 7374 796c 653d 2266 696c  f88)" style="fil
 0000a420: 6c3a 206e 6f6e 653b 2073 7472 6f6b 653a  l: none; stroke:
 0000a430: 2023 3432 3432 3432 3b20 7374 726f 6b65   #424242; stroke
 0000a440: 2d77 6964 7468 3a20 322e 373b 2073 7472  -width: 2.7; str
 0000a450: 6f6b 652d 6c69 6e65 6361 703a 2073 7175  oke-linecap: squ
 0000a460: 6172 6522 2f3e 0a20 2020 3c2f 673e 0a20  are"/>.   </g>. 
 0000a470: 2020 3c67 2069 643d 226c 696e 6532 645f    <g id="line2d_
 0000a480: 3638 223e 0a20 2020 203c 7061 7468 2063  68">.    <path c
 0000a490: 6c69 702d 7061 7468 3d22 7572 6c28 2370  lip-path="url(#p
-0000a4a0: 6132 3766 3363 3536 3361 2922 2073 7479  a27f3c563a)" sty
+0000a4a0: 3033 6539 3338 3966 3838 2922 2073 7479  03e9389f88)" sty
 0000a4b0: 6c65 3d22 6669 6c6c 3a20 6e6f 6e65 3b20  le="fill: none; 
 0000a4c0: 7374 726f 6b65 3a20 2334 3234 3234 323b  stroke: #424242;
 0000a4d0: 2073 7472 6f6b 652d 7769 6474 683a 2032   stroke-width: 2
 0000a4e0: 2e37 3b20 7374 726f 6b65 2d6c 696e 6563  .7; stroke-linec
 0000a4f0: 6170 3a20 7371 7561 7265 222f 3e0a 2020  ap: square"/>.  
 0000a500: 203c 2f67 3e0a 2020 203c 6720 6964 3d22   </g>.   <g id="
 0000a510: 7061 7463 685f 3333 223e 0a20 2020 203c  patch_33">.    <
@@ -3007,15 +3007,15 @@
 0000bbe0: 392e 3936 3837 3522 2f3e 0a20 2020 2020  9.96875"/>.     
 0000bbf0: 3c75 7365 2078 6c69 6e6b 3a68 7265 663d  <use xlink:href=
 0000bc00: 2223 4465 6a61 5675 5361 6e73 2d37 3322  "#DejaVuSans-73"
 0000bc10: 2078 3d22 3231 3931 2e34 3932 3138 3822   x="2191.492188"
 0000bc20: 2f3e 0a20 2020 203c 2f67 3e0a 2020 203c  />.    </g>.   <
 0000bc30: 2f67 3e0a 2020 3c2f 673e 0a20 3c2f 673e  /g>.  </g>. </g>
 0000bc40: 0a20 3c64 6566 733e 0a20 203c 636c 6970  . <defs>.  <clip
-0000bc50: 5061 7468 2069 643d 2270 6132 3766 3363  Path id="pa27f3c
-0000bc60: 3536 3361 223e 0a20 2020 3c72 6563 7420  563a">.   <rect 
+0000bc50: 5061 7468 2069 643d 2270 3033 6539 3338  Path id="p03e938
+0000bc60: 3966 3838 223e 0a20 2020 3c72 6563 7420  9f88">.   <rect 
 0000bc70: 783d 2234 342e 3537 2220 793d 2232 362e  x="44.57" y="26.
 0000bc80: 3838 2220 7769 6474 683d 2235 3135 2e35  88" width="515.5
 0000bc90: 3936 3633 3622 2068 6569 6768 743d 2231  96636" height="1
 0000bca0: 3832 2e31 3138 3731 3422 2f3e 0a20 203c  82.118714"/>.  <
 0000bcb0: 2f63 6c69 7050 6174 683e 0a20 3c2f 6465  /clipPath>. </de
 0000bcc0: 6673 3e0a 3c2f 7376 673e 0a              fs>.</svg>.
```

### Comparing `bioregistry-0.9.3/docs/img/bioregistry_coverage.svg` & `bioregistry-0.9.4/docs/img/bioregistry_coverage.svg`

 * *Files 0% similar despite different names*

```diff
@@ -30,16 +30,16 @@
 000001d0: 6178 2d6e 7323 223e 0a20 2020 3c63 633a  ax-ns#">.   <cc:
 000001e0: 576f 726b 3e0a 2020 2020 3c64 633a 7479  Work>.    <dc:ty
 000001f0: 7065 2072 6466 3a72 6573 6f75 7263 653d  pe rdf:resource=
 00000200: 2268 7474 703a 2f2f 7075 726c 2e6f 7267  "http://purl.org
 00000210: 2f64 632f 6463 6d69 7479 7065 2f53 7469  /dc/dcmitype/Sti
 00000220: 6c6c 496d 6167 6522 2f3e 0a20 2020 203c  llImage"/>.    <
 00000230: 6463 3a64 6174 653e 3230 3233 2d30 352d  dc:date>2023-05-
-00000240: 3033 5430 313a 3132 3a32 302e 3039 3231  03T01:12:20.0921
-00000250: 3032 3c2f 6463 3a64 6174 653e 0a20 2020  02</dc:date>.   
+00000240: 3034 5430 313a 3132 3a30 342e 3638 3032  04T01:12:04.6802
+00000250: 3434 3c2f 6463 3a64 6174 653e 0a20 2020  44</dc:date>.   
 00000260: 203c 6463 3a66 6f72 6d61 743e 696d 6167   <dc:format>imag
 00000270: 652f 7376 672b 786d 6c3c 2f64 633a 666f  e/svg+xml</dc:fo
 00000280: 726d 6174 3e0a 2020 2020 3c64 633a 6372  rmat>.    <dc:cr
 00000290: 6561 746f 723e 0a20 2020 2020 3c63 633a  eator>.     <cc:
 000002a0: 4167 656e 743e 0a20 2020 2020 203c 6463  Agent>.      <dc
 000002b0: 3a74 6974 6c65 3e4d 6174 706c 6f74 6c69  :title>Matplotli
 000002c0: 6220 7633 2e37 2e31 2c20 6874 7470 733a  b v3.7.1, https:
@@ -9347,15 +9347,15 @@
 00024820: 3930 3632 222f 3e0a 2020 2020 3c2f 673e  9062"/>.    </g>
 00024830: 0a20 2020 3c2f 673e 0a20 203c 2f67 3e0a  .   </g>.  </g>.
 00024840: 2020 3c67 2069 643d 2274 6578 745f 3132    <g id="text_12
 00024850: 3122 3e0a 2020 203c 212d 2d20 6874 7470  1">.   <!-- http
 00024860: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f62  s://github.com/b
 00024870: 696f 7072 6167 6d61 7469 6373 2f62 696f  iopragmatics/bio
 00024880: 7265 6769 7374 7279 2028 3230 3233 2d30  registry (2023-0
-00024890: 352d 3033 2920 2d2d 3e0a 2020 203c 6720  5-03) -->.   <g 
+00024890: 352d 3034 2920 2d2d 3e0a 2020 203c 6720  5-04) -->.   <g 
 000248a0: 7374 796c 653d 2266 696c 6c3a 2023 3830  style="fill: #80
 000248b0: 3830 3830 3b20 6f70 6163 6974 793a 2030  8080; opacity: 0
 000248c0: 2e35 2220 7472 616e 7366 6f72 6d3d 2274  .5" transform="t
 000248d0: 7261 6e73 6c61 7465 2832 3333 2e36 3736  ranslate(233.676
 000248e0: 3235 2031 3135 302e 3333 3632 3529 2073  25 1150.33625) s
 000248f0: 6361 6c65 2830 2e30 3820 2d30 2e30 3829  cale(0.08 -0.08)
 00024900: 223e 0a20 2020 203c 6465 6673 3e0a 2020  ">.    <defs>.  
@@ -9614,15 +9614,15 @@
 000258d0: 5675 5361 6e73 2d32 6422 2078 3d22 3237  VuSans-2d" x="27
 000258e0: 3330 2e37 3537 3831 3222 2f3e 0a20 2020  30.757812"/>.   
 000258f0: 203c 7573 6520 786c 696e 6b3a 6872 6566   <use xlink:href
 00025900: 3d22 2344 656a 6156 7553 616e 732d 3330  ="#DejaVuSans-30
 00025910: 2220 783d 2232 3736 362e 3834 3137 3937  " x="2766.841797
 00025920: 222f 3e0a 2020 2020 3c75 7365 2078 6c69  "/>.    <use xli
 00025930: 6e6b 3a68 7265 663d 2223 4465 6a61 5675  nk:href="#DejaVu
-00025940: 5361 6e73 2d33 3322 2078 3d22 3238 3330  Sans-33" x="2830
+00025940: 5361 6e73 2d33 3422 2078 3d22 3238 3330  Sans-34" x="2830
 00025950: 2e34 3634 3834 3422 2f3e 0a20 2020 203c  .464844"/>.    <
 00025960: 7573 6520 786c 696e 6b3a 6872 6566 3d22  use xlink:href="
 00025970: 2344 656a 6156 7553 616e 732d 3239 2220  #DejaVuSans-29" 
 00025980: 783d 2232 3839 342e 3038 3738 3931 222f  x="2894.087891"/
 00025990: 3e0a 2020 203c 2f67 3e0a 2020 3c2f 673e  >.   </g>.  </g>
 000259a0: 0a20 3c2f 673e 0a20 3c64 6566 733e 0a20  . </g>. <defs>. 
 000259b0: 203c 636c 6970 5061 7468 2069 643d 2270   <clipPath id="p
```

### Comparing `bioregistry-0.9.3/docs/img/bioregistry_coverage_bar.svg` & `bioregistry-0.9.4/docs/img/bioregistry_coverage_bar.svg`

 * *Files 0% similar despite different names*

```diff
@@ -29,16 +29,16 @@
 000001c0: 3032 2f32 322d 7264 662d 7379 6e74 6178  02/22-rdf-syntax
 000001d0: 2d6e 7323 223e 0a20 2020 3c63 633a 576f  -ns#">.   <cc:Wo
 000001e0: 726b 3e0a 2020 2020 3c64 633a 7479 7065  rk>.    <dc:type
 000001f0: 2072 6466 3a72 6573 6f75 7263 653d 2268   rdf:resource="h
 00000200: 7474 703a 2f2f 7075 726c 2e6f 7267 2f64  ttp://purl.org/d
 00000210: 632f 6463 6d69 7479 7065 2f53 7469 6c6c  c/dcmitype/Still
 00000220: 496d 6167 6522 2f3e 0a20 2020 203c 6463  Image"/>.    <dc
-00000230: 3a64 6174 653e 3230 3233 2d30 352d 3033  :date>2023-05-03
-00000240: 5430 313a 3132 3a31 392e 3039 3938 3433  T01:12:19.099843
+00000230: 3a64 6174 653e 3230 3233 2d30 352d 3034  :date>2023-05-04
+00000240: 5430 313a 3132 3a30 332e 3736 3636 3934  T01:12:03.766694
 00000250: 3c2f 6463 3a64 6174 653e 0a20 2020 203c  </dc:date>.    <
 00000260: 6463 3a66 6f72 6d61 743e 696d 6167 652f  dc:format>image/
 00000270: 7376 672b 786d 6c3c 2f64 633a 666f 726d  svg+xml</dc:form
 00000280: 6174 3e0a 2020 2020 3c64 633a 6372 6561  at>.    <dc:crea
 00000290: 746f 723e 0a20 2020 2020 3c63 633a 4167  tor>.     <cc:Ag
 000002a0: 656e 743e 0a20 2020 2020 203c 6463 3a74  ent>.      <dc:t
 000002b0: 6974 6c65 3e4d 6174 706c 6f74 6c69 6220  itle>Matplotlib
```

### Comparing `bioregistry-0.9.3/docs/img/bioregistry_coverage_bar_short.svg` & `bioregistry-0.9.4/docs/img/bioregistry_coverage_bar_short.svg`

 * *Files 1% similar despite different names*

```diff
@@ -29,16 +29,16 @@
 000001c0: 3032 2f32 322d 7264 662d 7379 6e74 6178  02/22-rdf-syntax
 000001d0: 2d6e 7323 223e 0a20 2020 3c63 633a 576f  -ns#">.   <cc:Wo
 000001e0: 726b 3e0a 2020 2020 3c64 633a 7479 7065  rk>.    <dc:type
 000001f0: 2072 6466 3a72 6573 6f75 7263 653d 2268   rdf:resource="h
 00000200: 7474 703a 2f2f 7075 726c 2e6f 7267 2f64  ttp://purl.org/d
 00000210: 632f 6463 6d69 7479 7065 2f53 7469 6c6c  c/dcmitype/Still
 00000220: 496d 6167 6522 2f3e 0a20 2020 203c 6463  Image"/>.    <dc
-00000230: 3a64 6174 653e 3230 3233 2d30 352d 3033  :date>2023-05-03
-00000240: 5430 313a 3132 3a32 302e 3435 3936 3332  T01:12:20.459632
+00000230: 3a64 6174 653e 3230 3233 2d30 352d 3034  :date>2023-05-04
+00000240: 5430 313a 3132 3a30 352e 3032 3039 3937  T01:12:05.020997
 00000250: 3c2f 6463 3a64 6174 653e 0a20 2020 203c  </dc:date>.    <
 00000260: 6463 3a66 6f72 6d61 743e 696d 6167 652f  dc:format>image/
 00000270: 7376 672b 786d 6c3c 2f64 633a 666f 726d  svg+xml</dc:form
 00000280: 6174 3e0a 2020 2020 3c64 633a 6372 6561  at>.    <dc:crea
 00000290: 746f 723e 0a20 2020 2020 3c63 633a 4167  tor>.     <cc:Ag
 000002a0: 656e 743e 0a20 2020 2020 203c 6463 3a74  ent>.      <dc:t
 000002b0: 6974 6c65 3e4d 6174 706c 6f74 6c69 6220  itle>Matplotlib
```

### Comparing `bioregistry-0.9.3/docs/img/datamodel_umls.svg` & `bioregistry-0.9.4/docs/img/datamodel_umls.svg`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/docs/img/external_overlap.svg` & `bioregistry-0.9.4/docs/img/external_overlap.svg`

 * *Files 0% similar despite different names*

```diff
@@ -30,16 +30,16 @@
 000001d0: 6e74 6178 2d6e 7323 223e 0a20 2020 3c63  ntax-ns#">.   <c
 000001e0: 633a 576f 726b 3e0a 2020 2020 3c64 633a  c:Work>.    <dc:
 000001f0: 7479 7065 2072 6466 3a72 6573 6f75 7263  type rdf:resourc
 00000200: 653d 2268 7474 703a 2f2f 7075 726c 2e6f  e="http://purl.o
 00000210: 7267 2f64 632f 6463 6d69 7479 7065 2f53  rg/dc/dcmitype/S
 00000220: 7469 6c6c 496d 6167 6522 2f3e 0a20 2020  tillImage"/>.   
 00000230: 203c 6463 3a64 6174 653e 3230 3233 2d30   <dc:date>2023-0
-00000240: 352d 3033 5430 313a 3136 3a30 362e 3337  5-03T01:16:06.37
-00000250: 3336 3038 3c2f 6463 3a64 6174 653e 0a20  3608</dc:date>. 
+00000240: 352d 3034 5430 313a 3135 3a32 362e 3830  5-04T01:15:26.80
+00000250: 3537 3730 3c2f 6463 3a64 6174 653e 0a20  5770</dc:date>. 
 00000260: 2020 203c 6463 3a66 6f72 6d61 743e 696d     <dc:format>im
 00000270: 6167 652f 7376 672b 786d 6c3c 2f64 633a  age/svg+xml</dc:
 00000280: 666f 726d 6174 3e0a 2020 2020 3c64 633a  format>.    <dc:
 00000290: 6372 6561 746f 723e 0a20 2020 2020 3c63  creator>.     <c
 000002a0: 633a 4167 656e 743e 0a20 2020 2020 203c  c:Agent>.      <
 000002b0: 6463 3a74 6974 6c65 3e4d 6174 706c 6f74  dc:title>Matplot
 000002c0: 6c69 6220 7633 2e37 2e31 2c20 6874 7470  lib v3.7.1, http
@@ -83946,15 +83946,15 @@
 00147e90: 3339 3036 3222 2f3e 0a20 2020 203c 2f67  39062"/>.    </g
 00147ea0: 3e0a 2020 203c 2f67 3e0a 2020 3c2f 673e  >.   </g>.  </g>
 00147eb0: 0a20 203c 6720 6964 3d22 7465 7874 5f31  .  <g id="text_1
 00147ec0: 3334 3822 3e0a 2020 203c 212d 2d20 6874  348">.   <!-- ht
 00147ed0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
 00147ee0: 2f62 696f 7072 6167 6d61 7469 6373 2f62  /biopragmatics/b
 00147ef0: 696f 7265 6769 7374 7279 2028 3230 3233  ioregistry (2023
-00147f00: 2d30 352d 3033 2920 2d2d 3e0a 2020 203c  -05-03) -->.   <
+00147f00: 2d30 352d 3034 2920 2d2d 3e0a 2020 203c  -05-04) -->.   <
 00147f10: 6720 7374 796c 653d 2266 696c 6c3a 2023  g style="fill: #
 00147f20: 3830 3830 3830 3b20 6f70 6163 6974 793a  808080; opacity:
 00147f30: 2030 2e35 2220 7472 616e 7366 6f72 6d3d   0.5" transform=
 00147f40: 2274 7261 6e73 6c61 7465 2832 3236 2e36  "translate(226.6
 00147f50: 3833 3433 3720 3132 3431 372e 3038 3834  83437 12417.0884
 00147f60: 3338 2920 7363 616c 6528 302e 3134 202d  38) scale(0.14 -
 00147f70: 302e 3134 2922 3e0a 2020 2020 3c64 6566  0.14)">.    <def
@@ -84232,15 +84232,15 @@
 00149070: 5361 6e73 2d32 6422 2078 3d22 3237 3330  Sans-2d" x="2730
 00149080: 2e37 3537 3831 3222 2f3e 0a20 2020 203c  .757812"/>.    <
 00149090: 7573 6520 786c 696e 6b3a 6872 6566 3d22  use xlink:href="
 001490a0: 2344 656a 6156 7553 616e 732d 3330 2220  #DejaVuSans-30" 
 001490b0: 783d 2232 3736 362e 3834 3137 3937 222f  x="2766.841797"/
 001490c0: 3e0a 2020 2020 3c75 7365 2078 6c69 6e6b  >.    <use xlink
 001490d0: 3a68 7265 663d 2223 4465 6a61 5675 5361  :href="#DejaVuSa
-001490e0: 6e73 2d33 3322 2078 3d22 3238 3330 2e34  ns-33" x="2830.4
+001490e0: 6e73 2d33 3422 2078 3d22 3238 3330 2e34  ns-34" x="2830.4
 001490f0: 3634 3834 3422 2f3e 0a20 2020 203c 7573  64844"/>.    <us
 00149100: 6520 786c 696e 6b3a 6872 6566 3d22 2344  e xlink:href="#D
 00149110: 656a 6156 7553 616e 732d 3239 2220 783d  ejaVuSans-29" x=
 00149120: 2232 3839 342e 3038 3738 3931 222f 3e0a  "2894.087891"/>.
 00149130: 2020 203c 2f67 3e0a 2020 3c2f 673e 0a20     </g>.  </g>. 
 00149140: 3c2f 673e 0a20 3c64 6566 733e 0a20 203c  </g>. <defs>.  <
 00149150: 636c 6970 5061 7468 2069 643d 2270 3334  clipPath id="p34
```

### Comparing `bioregistry-0.9.3/docs/img/has_attribute.svg` & `bioregistry-0.9.4/docs/img/has_attribute.svg`

 * *Files 0% similar despite different names*

```diff
@@ -29,16 +29,16 @@
 000001c0: 3032 2f32 322d 7264 662d 7379 6e74 6178  02/22-rdf-syntax
 000001d0: 2d6e 7323 223e 0a20 2020 3c63 633a 576f  -ns#">.   <cc:Wo
 000001e0: 726b 3e0a 2020 2020 3c64 633a 7479 7065  rk>.    <dc:type
 000001f0: 2072 6466 3a72 6573 6f75 7263 653d 2268   rdf:resource="h
 00000200: 7474 703a 2f2f 7075 726c 2e6f 7267 2f64  ttp://purl.org/d
 00000210: 632f 6463 6d69 7479 7065 2f53 7469 6c6c  c/dcmitype/Still
 00000220: 496d 6167 6522 2f3e 0a20 2020 203c 6463  Image"/>.    <dc
-00000230: 3a64 6174 653e 3230 3233 2d30 352d 3033  :date>2023-05-03
-00000240: 5430 313a 3132 3a34 352e 3630 3833 3734  T01:12:45.608374
+00000230: 3a64 6174 653e 3230 3233 2d30 352d 3034  :date>2023-05-04
+00000240: 5430 313a 3132 3a32 372e 3533 3933 3238  T01:12:27.539328
 00000250: 3c2f 6463 3a64 6174 653e 0a20 2020 203c  </dc:date>.    <
 00000260: 6463 3a66 6f72 6d61 743e 696d 6167 652f  dc:format>image/
 00000270: 7376 672b 786d 6c3c 2f64 633a 666f 726d  svg+xml</dc:form
 00000280: 6174 3e0a 2020 2020 3c64 633a 6372 6561  at>.    <dc:crea
 00000290: 746f 723e 0a20 2020 2020 3c63 633a 4167  tor>.     <cc:Ag
 000002a0: 656e 743e 0a20 2020 2020 203c 6463 3a74  ent>.      <dc:t
 000002b0: 6974 6c65 3e4d 6174 706c 6f74 6c69 6220  itle>Matplotlib 
@@ -4243,15 +4243,15 @@
 00010920: 3c2f 673e 0a20 203c 6720 6964 3d22 6178  </g>.  <g id="ax
 00010930: 6573 5f31 3522 2f3e 0a20 203c 6720 6964  es_15"/>.  <g id
 00010940: 3d22 6178 6573 5f31 3622 2f3e 0a20 203c  ="axes_16"/>.  <
 00010950: 6720 6964 3d22 7465 7874 5f37 3522 3e0a  g id="text_75">.
 00010960: 2020 203c 212d 2d20 6874 7470 733a 2f2f     <!-- https://
 00010970: 6769 7468 7562 2e63 6f6d 2f62 696f 7072  github.com/biopr
 00010980: 6167 6d61 7469 6373 2f62 696f 7265 6769  agmatics/bioregi
-00010990: 7374 7279 2028 3230 3233 2d30 352d 3033  stry (2023-05-03
+00010990: 7374 7279 2028 3230 3233 2d30 352d 3034  stry (2023-05-04
 000109a0: 2920 2d2d 3e0a 2020 203c 6720 7374 796c  ) -->.   <g styl
 000109b0: 653d 2266 696c 6c3a 2023 3830 3830 3830  e="fill: #808080
 000109c0: 3b20 6f70 6163 6974 793a 2030 2e35 2220  ; opacity: 0.5" 
 000109d0: 7472 616e 7366 6f72 6d3d 2274 7261 6e73  transform="trans
 000109e0: 6c61 7465 2832 3738 2e36 3736 3235 2035  late(278.67625 5
 000109f0: 3734 2e33 3336 3235 2920 7363 616c 6528  74.33625) scale(
 00010a00: 302e 3038 202d 302e 3038 2922 3e0a 2020  0.08 -0.08)">.  
@@ -4518,15 +4518,15 @@
 00011a50: 4465 6a61 5675 5361 6e73 2d32 6422 2078  DejaVuSans-2d" x
 00011a60: 3d22 3237 3330 2e37 3537 3831 3222 2f3e  ="2730.757812"/>
 00011a70: 0a20 2020 203c 7573 6520 786c 696e 6b3a  .    <use xlink:
 00011a80: 6872 6566 3d22 2344 656a 6156 7553 616e  href="#DejaVuSan
 00011a90: 732d 3330 2220 783d 2232 3736 362e 3834  s-30" x="2766.84
 00011aa0: 3137 3937 222f 3e0a 2020 2020 3c75 7365  1797"/>.    <use
 00011ab0: 2078 6c69 6e6b 3a68 7265 663d 2223 4465   xlink:href="#De
-00011ac0: 6a61 5675 5361 6e73 2d33 3322 2078 3d22  jaVuSans-33" x="
+00011ac0: 6a61 5675 5361 6e73 2d33 3422 2078 3d22  jaVuSans-34" x="
 00011ad0: 3238 3330 2e34 3634 3834 3422 2f3e 0a20  2830.464844"/>. 
 00011ae0: 2020 203c 7573 6520 786c 696e 6b3a 6872     <use xlink:hr
 00011af0: 6566 3d22 2344 656a 6156 7553 616e 732d  ef="#DejaVuSans-
 00011b00: 3239 2220 783d 2232 3839 342e 3038 3738  29" x="2894.0878
 00011b10: 3931 222f 3e0a 2020 203c 2f67 3e0a 2020  91"/>.   </g>.  
 00011b20: 3c2f 673e 0a20 3c2f 673e 0a3c 2f73 7667  </g>. </g>.</svg
 00011b30: 3e0a                                     >.
```

### Comparing `bioregistry-0.9.3/docs/img/providers.svg` & `bioregistry-0.9.4/docs/img/providers.svg`

 * *Files 0% similar despite different names*

```diff
@@ -29,16 +29,16 @@
 000001c0: 3032 2f32 322d 7264 662d 7379 6e74 6178  02/22-rdf-syntax
 000001d0: 2d6e 7323 223e 0a20 2020 3c63 633a 576f  -ns#">.   <cc:Wo
 000001e0: 726b 3e0a 2020 2020 3c64 633a 7479 7065  rk>.    <dc:type
 000001f0: 2072 6466 3a72 6573 6f75 7263 653d 2268   rdf:resource="h
 00000200: 7474 703a 2f2f 7075 726c 2e6f 7267 2f64  ttp://purl.org/d
 00000210: 632f 6463 6d69 7479 7065 2f53 7469 6c6c  c/dcmitype/Still
 00000220: 496d 6167 6522 2f3e 0a20 2020 203c 6463  Image"/>.    <dc
-00000230: 3a64 6174 653e 3230 3233 2d30 352d 3033  :date>2023-05-03
-00000240: 5430 313a 3136 3a30 392e 3230 3731 3737  T01:16:09.207177
+00000230: 3a64 6174 653e 3230 3233 2d30 352d 3034  :date>2023-05-04
+00000240: 5430 313a 3135 3a32 392e 3238 3237 3739  T01:15:29.282779
 00000250: 3c2f 6463 3a64 6174 653e 0a20 2020 203c  </dc:date>.    <
 00000260: 6463 3a66 6f72 6d61 743e 696d 6167 652f  dc:format>image/
 00000270: 7376 672b 786d 6c3c 2f64 633a 666f 726d  svg+xml</dc:form
 00000280: 6174 3e0a 2020 2020 3c64 633a 6372 6561  at>.    <dc:crea
 00000290: 746f 723e 0a20 2020 2020 3c63 633a 4167  tor>.     <cc:Ag
 000002a0: 656e 743e 0a20 2020 2020 203c 6463 3a74  ent>.      <dc:t
 000002b0: 6974 6c65 3e4d 6174 706c 6f74 6c69 6220  itle>Matplotlib 
@@ -1304,15 +1304,15 @@
 00005170: 3b20 7374 726f 6b65 2d6c 696e 6563 6170  ; stroke-linecap
 00005180: 3a20 7371 7561 7265 222f 3e0a 2020 203c  : square"/>.   <
 00005190: 2f67 3e0a 2020 3c2f 673e 0a20 203c 6720  /g>.  </g>.  <g 
 000051a0: 6964 3d22 7465 7874 5f31 3522 3e0a 2020  id="text_15">.  
 000051b0: 203c 212d 2d20 6874 7470 733a 2f2f 6769   <!-- https://gi
 000051c0: 7468 7562 2e63 6f6d 2f62 696f 7072 6167  thub.com/bioprag
 000051d0: 6d61 7469 6373 2f62 696f 7265 6769 7374  matics/bioregist
-000051e0: 7279 2028 3230 3233 2d30 352d 3033 2920  ry (2023-05-03) 
+000051e0: 7279 2028 3230 3233 2d30 352d 3034 2920  ry (2023-05-04) 
 000051f0: 2d2d 3e0a 2020 203c 6720 7374 796c 653d  -->.   <g style=
 00005200: 2266 696c 6c3a 2023 3830 3830 3830 3b20  "fill: #808080; 
 00005210: 6f70 6163 6974 793a 2030 2e35 2220 7472  opacity: 0.5" tr
 00005220: 616e 7366 6f72 6d3d 2274 7261 6e73 6c61  ansform="transla
 00005230: 7465 2835 3932 2e33 3336 3235 2032 3433  te(592.33625 243
 00005240: 2e33 3233 3735 2920 726f 7461 7465 282d  .32375) rotate(-
 00005250: 3930 2920 7363 616c 6528 302e 3038 202d  90) scale(0.08 -
@@ -1755,15 +1755,15 @@
 00006da0: 656a 6156 7553 616e 732d 3264 2220 783d  ejaVuSans-2d" x=
 00006db0: 2232 3733 302e 3735 3738 3132 222f 3e0a  "2730.757812"/>.
 00006dc0: 2020 2020 3c75 7365 2078 6c69 6e6b 3a68      <use xlink:h
 00006dd0: 7265 663d 2223 4465 6a61 5675 5361 6e73  ref="#DejaVuSans
 00006de0: 2d33 3022 2078 3d22 3237 3636 2e38 3431  -30" x="2766.841
 00006df0: 3739 3722 2f3e 0a20 2020 203c 7573 6520  797"/>.    <use 
 00006e00: 786c 696e 6b3a 6872 6566 3d22 2344 656a  xlink:href="#Dej
-00006e10: 6156 7553 616e 732d 3333 2220 783d 2232  aVuSans-33" x="2
+00006e10: 6156 7553 616e 732d 3334 2220 783d 2232  aVuSans-34" x="2
 00006e20: 3833 302e 3436 3438 3434 222f 3e0a 2020  830.464844"/>.  
 00006e30: 2020 3c75 7365 2078 6c69 6e6b 3a68 7265    <use xlink:hre
 00006e40: 663d 2223 4465 6a61 5675 5361 6e73 2d32  f="#DejaVuSans-2
 00006e50: 3922 2078 3d22 3238 3934 2e30 3837 3839  9" x="2894.08789
 00006e60: 3122 2f3e 0a20 2020 3c2f 673e 0a20 203c  1"/>.   </g>.  <
 00006e70: 2f67 3e0a 203c 2f67 3e0a 203c 6465 6673  /g>. </g>. <defs
 00006e80: 3e0a 2020 3c63 6c69 7050 6174 6820 6964  >.  <clipPath id
```

### Comparing `bioregistry-0.9.3/docs/img/regex_report.svg` & `bioregistry-0.9.4/docs/img/regex_report.svg`

 * *Files 0% similar despite different names*

```diff
@@ -29,16 +29,16 @@
 000001c0: 3032 2f32 322d 7264 662d 7379 6e74 6178  02/22-rdf-syntax
 000001d0: 2d6e 7323 223e 0a20 2020 3c63 633a 576f  -ns#">.   <cc:Wo
 000001e0: 726b 3e0a 2020 2020 3c64 633a 7479 7065  rk>.    <dc:type
 000001f0: 2072 6466 3a72 6573 6f75 7263 653d 2268   rdf:resource="h
 00000200: 7474 703a 2f2f 7075 726c 2e6f 7267 2f64  ttp://purl.org/d
 00000210: 632f 6463 6d69 7479 7065 2f53 7469 6c6c  c/dcmitype/Still
 00000220: 496d 6167 6522 2f3e 0a20 2020 203c 6463  Image"/>.    <dc
-00000230: 3a64 6174 653e 3230 3233 2d30 352d 3033  :date>2023-05-03
-00000240: 5430 313a 3136 3a31 302e 3132 3238 3035  T01:16:10.122805
+00000230: 3a64 6174 653e 3230 3233 2d30 352d 3034  :date>2023-05-04
+00000240: 5430 313a 3135 3a33 302e 3038 3033 3338  T01:15:30.080338
 00000250: 3c2f 6463 3a64 6174 653e 0a20 2020 203c  </dc:date>.    <
 00000260: 6463 3a66 6f72 6d61 743e 696d 6167 652f  dc:format>image/
 00000270: 7376 672b 786d 6c3c 2f64 633a 666f 726d  svg+xml</dc:form
 00000280: 6174 3e0a 2020 2020 3c64 633a 6372 6561  at>.    <dc:crea
 00000290: 746f 723e 0a20 2020 2020 3c63 633a 4167  tor>.     <cc:Ag
 000002a0: 656e 743e 0a20 2020 2020 203c 6463 3a74  ent>.      <dc:t
 000002b0: 6974 6c65 3e4d 6174 706c 6f74 6c69 6220  itle>Matplotlib
```

### Comparing `bioregistry-0.9.3/docs/img/xrefs.svg` & `bioregistry-0.9.4/docs/img/xrefs.svg`

 * *Files 0% similar despite different names*

```diff
@@ -29,16 +29,16 @@
 000001c0: 3032 2f32 322d 7264 662d 7379 6e74 6178  02/22-rdf-syntax
 000001d0: 2d6e 7323 223e 0a20 2020 3c63 633a 576f  -ns#">.   <cc:Wo
 000001e0: 726b 3e0a 2020 2020 3c64 633a 7479 7065  rk>.    <dc:type
 000001f0: 2072 6466 3a72 6573 6f75 7263 653d 2268   rdf:resource="h
 00000200: 7474 703a 2f2f 7075 726c 2e6f 7267 2f64  ttp://purl.org/d
 00000210: 632f 6463 6d69 7479 7065 2f53 7469 6c6c  c/dcmitype/Still
 00000220: 496d 6167 6522 2f3e 0a20 2020 203c 6463  Image"/>.    <dc
-00000230: 3a64 6174 653e 3230 3233 2d30 352d 3033  :date>2023-05-03
-00000240: 5430 313a 3132 3a31 382e 3733 3531 3237  T01:12:18.735127
+00000230: 3a64 6174 653e 3230 3233 2d30 352d 3034  :date>2023-05-04
+00000240: 5430 313a 3132 3a30 332e 3433 3136 3733  T01:12:03.431673
 00000250: 3c2f 6463 3a64 6174 653e 0a20 2020 203c  </dc:date>.    <
 00000260: 6463 3a66 6f72 6d61 743e 696d 6167 652f  dc:format>image/
 00000270: 7376 672b 786d 6c3c 2f64 633a 666f 726d  svg+xml</dc:form
 00000280: 6174 3e0a 2020 2020 3c64 633a 6372 6561  at>.    <dc:crea
 00000290: 746f 723e 0a20 2020 2020 3c63 633a 4167  tor>.     <cc:Ag
 000002a0: 656e 743e 0a20 2020 2020 203c 6463 3a74  ent>.      <dc:t
 000002b0: 6974 6c65 3e4d 6174 706c 6f74 6c69 6220  itle>Matplotlib 
@@ -2920,15 +2920,15 @@
 0000b670: 352e 3638 3535 3437 222f 3e0a 2020 2020  5.685547"/>.    
 0000b680: 3c2f 673e 0a20 2020 3c2f 673e 0a20 203c  </g>.   </g>.  <
 0000b690: 2f67 3e0a 2020 3c67 2069 643d 2274 6578  /g>.  <g id="tex
 0000b6a0: 745f 3438 223e 0a20 2020 3c21 2d2d 2068  t_48">.   <!-- h
 0000b6b0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
 0000b6c0: 6d2f 6269 6f70 7261 676d 6174 6963 732f  m/biopragmatics/
 0000b6d0: 6269 6f72 6567 6973 7472 7920 2832 3032  bioregistry (202
-0000b6e0: 332d 3035 2d30 3329 202d 2d3e 0a20 2020  3-05-03) -->.   
+0000b6e0: 332d 3035 2d30 3429 202d 2d3e 0a20 2020  3-05-04) -->.   
 0000b6f0: 3c67 2073 7479 6c65 3d22 6669 6c6c 3a20  <g style="fill: 
 0000b700: 2338 3038 3038 303b 206f 7061 6369 7479  #808080; opacity
 0000b710: 3a20 302e 3522 2074 7261 6e73 666f 726d  : 0.5" transform
 0000b720: 3d22 7472 616e 736c 6174 6528 3539 322e  ="translate(592.
 0000b730: 3333 3632 3520 3234 332e 3332 3337 3529  33625 243.32375)
 0000b740: 2072 6f74 6174 6528 2d39 3029 2073 6361   rotate(-90) sca
 0000b750: 6c65 2830 2e30 3820 2d30 2e30 3829 223e  le(0.08 -0.08)">
@@ -3199,15 +3199,15 @@
 0000c7e0: 7553 616e 732d 3264 2220 783d 2232 3733  uSans-2d" x="273
 0000c7f0: 302e 3735 3738 3132 222f 3e0a 2020 2020  0.757812"/>.    
 0000c800: 3c75 7365 2078 6c69 6e6b 3a68 7265 663d  <use xlink:href=
 0000c810: 2223 4465 6a61 5675 5361 6e73 2d33 3022  "#DejaVuSans-30"
 0000c820: 2078 3d22 3237 3636 2e38 3431 3739 3722   x="2766.841797"
 0000c830: 2f3e 0a20 2020 203c 7573 6520 786c 696e  />.    <use xlin
 0000c840: 6b3a 6872 6566 3d22 2344 656a 6156 7553  k:href="#DejaVuS
-0000c850: 616e 732d 3333 2220 783d 2232 3833 302e  ans-33" x="2830.
+0000c850: 616e 732d 3334 2220 783d 2232 3833 302e  ans-34" x="2830.
 0000c860: 3436 3438 3434 222f 3e0a 2020 2020 3c75  464844"/>.    <u
 0000c870: 7365 2078 6c69 6e6b 3a68 7265 663d 2223  se xlink:href="#
 0000c880: 4465 6a61 5675 5361 6e73 2d32 3922 2078  DejaVuSans-29" x
 0000c890: 3d22 3238 3934 2e30 3837 3839 3122 2f3e  ="2894.087891"/>
 0000c8a0: 0a20 2020 3c2f 673e 0a20 203c 2f67 3e0a  .   </g>.  </g>.
 0000c8b0: 203c 2f67 3e0a 203c 6465 6673 3e0a 2020   </g>. <defs>.  
 0000c8c0: 3c63 6c69 7050 6174 6820 6964 3d22 7031  <clipPath id="p1
```

### Comparing `bioregistry-0.9.3/docs/source/conf.py` & `bioregistry-0.9.4/docs/source/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 # -- Project information -----------------------------------------------------
 
 project = "bioregistry"
 copyright = f"{date.today().year}, Charles Tapley Hoyt"
 author = "Charles Tapley Hoyt"
 
 # The full version, including alpha/beta/rc tags.
-release = "0.9.3"
+release = "0.9.4"
 
 # The short X.Y version.
 parsed_version = re.match(
     "(?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(?:-(?P<release>[0-9A-Za-z-]+(?:\.[0-9A-Za-z-]+)*))?(?:\+(?P<build>[0-9A-Za-z-]+(?:\.[0-9A-Za-z-]+)*))?",
     release,
 )
 version = parsed_version.expand("\g<major>.\g<minor>.\g<patch>")
```

### Comparing `bioregistry-0.9.3/docs/source/deployment.rst` & `bioregistry-0.9.4/docs/source/deployment.rst`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/docs/source/index.rst` & `bioregistry-0.9.4/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/docs/source/logo.png` & `bioregistry-0.9.4/docs/source/logo.png`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/setup.cfg` & `bioregistry-0.9.4/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = bioregistry
-version = 0.9.3
+version = 0.9.4
 description = Integrated registry of biological databases and nomenclatures
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/biopragmatics/bioregistry
 download_url = https://github.com/biopragmatics/bioregistry/releases
 project_urls = 
 	Bug Tracker = https://github.com/biopragmatics/bioregistry/issues
```

### Comparing `bioregistry-0.9.3/src/bioregistry/__init__.py` & `bioregistry-0.9.4/src/bioregistry/__init__.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/align/__init__.py` & `bioregistry-0.9.4/src/bioregistry/align/__init__.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/align/biocontext.py` & `bioregistry-0.9.4/src/bioregistry/align/biocontext.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/align/biolink.py` & `bioregistry-0.9.4/src/bioregistry/align/biolink.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/align/bioportal.py` & `bioregistry-0.9.4/src/bioregistry/align/bioportal.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/align/cellosaurus.py` & `bioregistry-0.9.4/src/bioregistry/align/cellosaurus.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/align/cheminf.py` & `bioregistry-0.9.4/src/bioregistry/align/cheminf.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/align/edam.py` & `bioregistry-0.9.4/src/bioregistry/align/edam.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/align/fairsharing.py` & `bioregistry-0.9.4/src/bioregistry/align/fairsharing.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/align/go.py` & `bioregistry-0.9.4/src/bioregistry/align/go.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/align/hl7.py` & `bioregistry-0.9.4/src/bioregistry/align/hl7.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/align/n2t.py` & `bioregistry-0.9.4/src/bioregistry/align/n2t.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/align/ncbi.py` & `bioregistry-0.9.4/src/bioregistry/align/ncbi.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/align/obofoundry.py` & `bioregistry-0.9.4/src/bioregistry/align/obofoundry.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/align/ols.py` & `bioregistry-0.9.4/src/bioregistry/align/ols.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/align/ontobee.py` & `bioregistry-0.9.4/src/bioregistry/align/ontobee.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/align/prefixcommons.py` & `bioregistry-0.9.4/src/bioregistry/align/prefixcommons.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/align/re3data.py` & `bioregistry-0.9.4/src/bioregistry/align/re3data.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/align/uniprot.py` & `bioregistry-0.9.4/src/bioregistry/align/uniprot.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/align/utils.py` & `bioregistry-0.9.4/src/bioregistry/align/utils.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/align/wikidata.py` & `bioregistry-0.9.4/src/bioregistry/align/wikidata.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/analysis/title_tfidf.py` & `bioregistry-0.9.4/src/bioregistry/analysis/title_tfidf.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/app/api.py` & `bioregistry-0.9.4/src/bioregistry/app/api.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/app/cli.py` & `bioregistry-0.9.4/src/bioregistry/app/cli.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/app/constants.py` & `bioregistry-0.9.4/src/bioregistry/app/constants.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/app/impl.py` & `bioregistry-0.9.4/src/bioregistry/app/impl.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/app/static/logo.svg` & `bioregistry-0.9.4/src/bioregistry/app/static/logo.svg`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/app/templates/base.html` & `bioregistry-0.9.4/src/bioregistry/app/templates/base.html`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/app/templates/collection.html` & `bioregistry-0.9.4/src/bioregistry/app/templates/collection.html`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/app/templates/collections.html` & `bioregistry-0.9.4/src/bioregistry/app/templates/collections.html`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/app/templates/context.html` & `bioregistry-0.9.4/src/bioregistry/app/templates/context.html`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/app/templates/contexts.html` & `bioregistry-0.9.4/src/bioregistry/app/templates/contexts.html`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/app/templates/contributor.html` & `bioregistry-0.9.4/src/bioregistry/app/templates/contributor.html`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/app/templates/contributors.html` & `bioregistry-0.9.4/src/bioregistry/app/templates/contributors.html`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/app/templates/highlights/keywords.html` & `bioregistry-0.9.4/src/bioregistry/app/templates/highlights/keywords.html`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/app/templates/highlights/owners.html` & `bioregistry-0.9.4/src/bioregistry/app/templates/highlights/owners.html`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/app/templates/highlights/relations.html` & `bioregistry-0.9.4/src/bioregistry/app/templates/highlights/relations.html`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/app/templates/highlights/twitter.html` & `bioregistry-0.9.4/src/bioregistry/app/templates/highlights/twitter.html`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/app/templates/home.html` & `bioregistry-0.9.4/src/bioregistry/app/templates/home.html`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/app/templates/macros.html` & `bioregistry-0.9.4/src/bioregistry/app/templates/macros.html`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/app/templates/meta/access.html` & `bioregistry-0.9.4/src/bioregistry/app/templates/meta/access.html`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/app/templates/meta/acknowledgements.html` & `bioregistry-0.9.4/src/bioregistry/app/templates/meta/acknowledgements.html`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/app/templates/meta/download.html` & `bioregistry-0.9.4/src/bioregistry/app/templates/meta/download.html`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/app/templates/meta/related.html` & `bioregistry-0.9.4/src/bioregistry/app/templates/meta/related.html`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/app/templates/meta/schema.html` & `bioregistry-0.9.4/src/bioregistry/app/templates/meta/schema.html`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/app/templates/meta/summary.html` & `bioregistry-0.9.4/src/bioregistry/app/templates/meta/summary.html`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/app/templates/meta/sustainability.html` & `bioregistry-0.9.4/src/bioregistry/app/templates/meta/sustainability.html`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/app/templates/metaresource.html` & `bioregistry-0.9.4/src/bioregistry/app/templates/metaresource.html`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/app/templates/metaresources.html` & `bioregistry-0.9.4/src/bioregistry/app/templates/metaresources.html`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/app/templates/prose.html` & `bioregistry-0.9.4/src/bioregistry/app/templates/prose.html`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/app/templates/reference.html` & `bioregistry-0.9.4/src/bioregistry/app/templates/reference.html`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/app/templates/resolve_errors/disallowed_identifier.html` & `bioregistry-0.9.4/src/bioregistry/app/templates/resolve_errors/disallowed_identifier.html`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/app/templates/resolve_errors/invalid_identifier.html` & `bioregistry-0.9.4/src/bioregistry/app/templates/resolve_errors/invalid_identifier.html`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/app/templates/resolve_errors/missing_prefix.html` & `bioregistry-0.9.4/src/bioregistry/app/templates/resolve_errors/missing_prefix.html`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/app/templates/resolve_errors/missing_providers.html` & `bioregistry-0.9.4/src/bioregistry/app/templates/resolve_errors/missing_providers.html`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/app/templates/resource.html` & `bioregistry-0.9.4/src/bioregistry/app/templates/resource.html`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/app/templates/resources.html` & `bioregistry-0.9.4/src/bioregistry/app/templates/resources.html`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/app/test.py` & `bioregistry-0.9.4/src/bioregistry/app/test.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/app/ui.py` & `bioregistry-0.9.4/src/bioregistry/app/ui.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/app/utils.py` & `bioregistry-0.9.4/src/bioregistry/app/utils.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/benchmarks/cli.py` & `bioregistry-0.9.4/src/bioregistry/benchmarks/cli.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/benchmarks/curie_parsing.py` & `bioregistry-0.9.4/src/bioregistry/benchmarks/curie_parsing.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/benchmarks/curie_validation.py` & `bioregistry-0.9.4/src/bioregistry/benchmarks/curie_validation.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/benchmarks/uri_parsing.py` & `bioregistry-0.9.4/src/bioregistry/benchmarks/uri_parsing.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/bibliometrics.py` & `bioregistry-0.9.4/src/bioregistry/bibliometrics.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/cli.py` & `bioregistry-0.9.4/src/bioregistry/cli.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/collection_api.py` & `bioregistry-0.9.4/src/bioregistry/collection_api.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/compare.py` & `bioregistry-0.9.4/src/bioregistry/compare.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/constants.py` & `bioregistry-0.9.4/src/bioregistry/constants.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/curation/add_co_providers.py` & `bioregistry-0.9.4/src/bioregistry/curation/add_co_providers.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/curation/add_descriptions_from_gs.py` & `bioregistry-0.9.4/src/bioregistry/curation/add_descriptions_from_gs.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/curation/add_examples.py` & `bioregistry-0.9.4/src/bioregistry/curation/add_examples.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/curation/add_examples_from_javert.py` & `bioregistry-0.9.4/src/bioregistry/curation/add_examples_from_javert.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/curation/add_examples_from_ols.py` & `bioregistry-0.9.4/src/bioregistry/curation/add_examples_from_ols.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/curation/add_ontology_regexes.py` & `bioregistry-0.9.4/src/bioregistry/curation/add_ontology_regexes.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/curation/bulk_import.py` & `bioregistry-0.9.4/src/bioregistry/curation/bulk_import.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/curation/clean_licenses.py` & `bioregistry-0.9.4/src/bioregistry/curation/clean_licenses.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/curation/clean_name_suffixes.py` & `bioregistry-0.9.4/src/bioregistry/curation/clean_name_suffixes.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/curation/clean_publications.py` & `bioregistry-0.9.4/src/bioregistry/curation/clean_publications.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/curation/cleanup_authors.py` & `bioregistry-0.9.4/src/bioregistry/curation/cleanup_authors.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/curation/deprecation_diff.py` & `bioregistry-0.9.4/src/bioregistry/curation/deprecation_diff.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/curation/enrich_publications.py` & `bioregistry-0.9.4/src/bioregistry/curation/enrich_publications.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/curation/import_pc_semiautomatic.py` & `bioregistry-0.9.4/src/bioregistry/curation/import_pc_semiautomatic.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/curation/make_description_curation_sheet.py` & `bioregistry-0.9.4/src/bioregistry/curation/make_description_curation_sheet.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/curation/map_bartoc_via_wikidata.py` & `bioregistry-0.9.4/src/bioregistry/curation/map_bartoc_via_wikidata.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/curation/map_re3data_via_fairsharing.py` & `bioregistry-0.9.4/src/bioregistry/curation/map_re3data_via_fairsharing.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/curation/rename_metaprefix.py` & `bioregistry-0.9.4/src/bioregistry/curation/rename_metaprefix.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/curation/review_pc.py` & `bioregistry-0.9.4/src/bioregistry/curation/review_pc.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/curation/suggest_author_curation.py` & `bioregistry-0.9.4/src/bioregistry/curation/suggest_author_curation.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/curation/suggest_uniprot_providers.py` & `bioregistry-0.9.4/src/bioregistry/curation/suggest_uniprot_providers.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/data/README.md` & `bioregistry-0.9.4/src/bioregistry/data/README.md`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/data/bioregistry.json` & `bioregistry-0.9.4/src/bioregistry/data/bioregistry.json`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/data/collections.json` & `bioregistry-0.9.4/src/bioregistry/data/collections.json`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/data/contexts.json` & `bioregistry-0.9.4/src/bioregistry/data/contexts.json`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/data/external/aberowl/curation.tsv` & `bioregistry-0.9.4/src/bioregistry/data/external/aberowl/curation.tsv`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/data/external/aberowl/processed.json` & `bioregistry-0.9.4/src/bioregistry/data/external/aberowl/processed.json`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/data/external/aberowl/raw.json` & `bioregistry-0.9.4/src/bioregistry/data/external/aberowl/raw.json`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/data/external/agroportal/curation.tsv` & `bioregistry-0.9.4/src/bioregistry/data/external/agroportal/curation.tsv`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/data/external/agroportal/processed.json` & `bioregistry-0.9.4/src/bioregistry/data/external/agroportal/processed.json`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/data/external/agroportal/raw.json` & `bioregistry-0.9.4/src/bioregistry/data/external/agroportal/raw.json`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/data/external/bartoc/curation.tsv` & `bioregistry-0.9.4/src/bioregistry/data/external/bartoc/curation.tsv`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/data/external/bartoc/processed.json` & `bioregistry-0.9.4/src/bioregistry/data/external/bartoc/processed.json`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/data/external/biocontext/curation.tsv` & `bioregistry-0.9.4/src/bioregistry/data/external/biocontext/curation.tsv`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/data/external/biocontext/processed.json` & `bioregistry-0.9.4/src/bioregistry/data/external/biocontext/processed.json`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/data/external/biocontext/raw.json` & `bioregistry-0.9.4/src/bioregistry/data/external/biocontext/raw.json`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/data/external/biolink/curation.tsv` & `bioregistry-0.9.4/src/bioregistry/data/external/biolink/curation.tsv`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/data/external/biolink/processed.json` & `bioregistry-0.9.4/src/bioregistry/data/external/biolink/processed.json`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/data/external/biolink/raw.yaml` & `bioregistry-0.9.4/src/bioregistry/data/external/biolink/raw.yaml`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/data/external/bioportal/curation.tsv` & `bioregistry-0.9.4/src/bioregistry/data/external/bioportal/curation.tsv`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/data/external/bioportal/processed.json` & `bioregistry-0.9.4/src/bioregistry/data/external/bioportal/processed.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998514760990769%*

 * *Differences: {"'GFF-M4M'": "{'version': '0.1.0'}",*

 * * "'MAXO'": "{'version': '2023-05-02'}",*

 * * "'NBO'": "{'version': '2023-05-02'}"}*

```diff
@@ -3775,15 +3775,16 @@
             "email": "barbara.magagna@gmail.com",
             "name": "Barbara Magagna"
         },
         "description": "Controlled vocabularies allow an accurate and controlled approach in describing physical and digital assets (e.g., data). One of such controlled vocabulary is M4M Vocabulary. This controlled vocabulary is produced in Metadata 4 Machine (M4M) Workshop. sheet2rdf is used to build and serve M4M Vocabulary, while PURL is used to persist identifiers for the vocabulary: http://purl.org/m4m/",
         "homepage": "https://github.com/gofair-foundation/m4m-vocabulary",
         "name": "GoFair M4M",
         "prefix": "GFF-M4M",
-        "publication": "https://github.com/gofair-foundation/m4m-vocabulary"
+        "publication": "https://github.com/gofair-foundation/m4m-vocabulary",
+        "version": "0.1.0"
     },
     "GFFO": {
         "contact": {
             "email": "carsten.fortmann-grote@evolbio.mpg.de",
             "name": "Carsten Fortmann-Grote"
         },
         "description": "An ontology to represent genome feature annotations in gff3 format.",
@@ -5819,15 +5820,15 @@
             "email": "Leigh.Carmody@jax.org",
             "name": "Leigh Carmody"
         },
         "description": "The Medical Action Ontology (MAxO) provides a structured vocabulary for medical procedures, interventions, therapies, and treatments for disease with an emphasis on rare disease (RD). It is often difficult to find relevant clinical literature about strategies to manage RD patients. Responding to this need, MAxO provides a vocabulary to annotate diseases and phenotypes with recommended treatments and interventions.",
         "homepage": "https://github.com/monarch-initiative/MAxO",
         "name": "Medical Action Ontology",
         "prefix": "MAXO",
-        "version": "2023-04-18"
+        "version": "2023-05-02"
     },
     "MCBCC": {
         "contact": {
             "email": "arathi@molecularconnections.com",
             "name": "Arathi Raghunath"
         },
         "description": "Contains a comprehensive list of cell lines derived from breast tissue, both normal and pathological. The ontology in built in OWL with cross relation to classes- genetic variation, pathological condition, genes, chemicals and drugs. The relations built enable semantic query across different classes",
@@ -6550,15 +6551,15 @@
             "email": "g.gkoutos@gmail.com",
             "name": "George Gkoutos"
         },
         "description": "The Neurobehavior Ontology (NBO) consists of two main components, an ontology of behavioral processes and an ontology of behavioral phenotypes. The behavioral process branch of NBO contains a classification of behavior processes complementing and extending GO\u2019s process ontology. The behavior phenotype branch of NBO consists of a classification of both normal and abnormal behavioral characteristics of organisms.",
         "homepage": "https://github.com/obo-behavior/behavior-ontology/",
         "name": "Neuro Behavior Ontology",
         "prefix": "NBO",
-        "version": "2023-02-21"
+        "version": "2023-05-02"
     },
     "NCBITAXON": {
         "contact": {
             "email": "info@ncbi.nlm.nih.gov",
             "name": "NCBI information"
         },
         "description": "The NCBI Taxonomy Database is a curated classification and nomenclature for all of the organisms in the public sequence databases.",
```

### Comparing `bioregistry-0.9.3/src/bioregistry/data/external/bioportal/raw.json` & `bioregistry-0.9.4/src/bioregistry/data/external/bioportal/raw.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998327807828769%*

 * *Differences: {'1014': "{'version': '2023-05-02'}",*

 * * '356': "{'version': '0.1.0'}",*

 * * '784': "{'version': '2023-05-02'}"}*

```diff
@@ -19532,15 +19532,16 @@
             "single_class": "https://data.bioontology.org/ontologies/GFF-M4M/classes/{class_id}",
             "submissions": "https://data.bioontology.org/ontologies/GFF-M4M/submissions",
             "ui": "http://bioportal.bioontology.org/ontologies/GFF-M4M",
             "views": "https://data.bioontology.org/ontologies/GFF-M4M/views"
         },
         "name": "GoFair M4M",
         "ontologyType": "https://data.bioontology.org/ontology_types/ONTOLOGY",
-        "publication": "https://github.com/gofair-foundation/m4m-vocabulary"
+        "publication": "https://github.com/gofair-foundation/m4m-vocabulary",
+        "version": "0.1.0"
     },
     {
         "@id": "https://data.bioontology.org/ontologies/VODANA-MIGRANTS",
         "@type": "http://data.bioontology.org/metadata/Ontology",
         "acronym": "VODANA-MIGRANTS",
         "administeredBy": [
             "https://data.bioontology.org/users/Ghardallou"
@@ -42980,15 +42981,15 @@
             "single_class": "https://data.bioontology.org/ontologies/MAXO/classes/{class_id}",
             "submissions": "https://data.bioontology.org/ontologies/MAXO/submissions",
             "ui": "http://bioportal.bioontology.org/ontologies/MAXO",
             "views": "https://data.bioontology.org/ontologies/MAXO/views"
         },
         "name": "Medical Action Ontology",
         "ontologyType": "https://data.bioontology.org/ontology_types/ONTOLOGY",
-        "version": "2023-04-18"
+        "version": "2023-05-02"
     },
     {
         "@id": "https://data.bioontology.org/ontologies/MFO",
         "@type": "http://data.bioontology.org/metadata/Ontology",
         "acronym": "MFO",
         "administeredBy": [
             "https://data.bioontology.org/users/Thorsten.Henrich%40embl-heidelberg.de"
@@ -55565,15 +55566,15 @@
             "single_class": "https://data.bioontology.org/ontologies/NBO/classes/{class_id}",
             "submissions": "https://data.bioontology.org/ontologies/NBO/submissions",
             "ui": "http://bioportal.bioontology.org/ontologies/NBO",
             "views": "https://data.bioontology.org/ontologies/NBO/views"
         },
         "name": "Neuro Behavior Ontology",
         "ontologyType": "https://data.bioontology.org/ontology_types/ONTOLOGY",
-        "version": "2023-02-21"
+        "version": "2023-05-02"
     },
     {
         "@id": "https://data.bioontology.org/ontologies/TCDO",
         "@type": "http://data.bioontology.org/metadata/Ontology",
         "acronym": "TCDO",
         "administeredBy": [
             "https://data.bioontology.org/users/zhuyan166",
```

### Comparing `bioregistry-0.9.3/src/bioregistry/data/external/cellosaurus/curation.tsv` & `bioregistry-0.9.4/src/bioregistry/data/external/cellosaurus/curation.tsv`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/data/external/cellosaurus/processed.json` & `bioregistry-0.9.4/src/bioregistry/data/external/cellosaurus/processed.json`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/data/external/cellosaurus/raw.txt` & `bioregistry-0.9.4/src/bioregistry/data/external/cellosaurus/raw.txt`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/data/external/cheminf/processed.json` & `bioregistry-0.9.4/src/bioregistry/data/external/cheminf/processed.json`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/data/external/cropoct/processed.json` & `bioregistry-0.9.4/src/bioregistry/data/external/cropoct/processed.json`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/data/external/cropoct/raw.yaml` & `bioregistry-0.9.4/src/bioregistry/data/external/cropoct/raw.yaml`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/data/external/ecoportal/curation.tsv` & `bioregistry-0.9.4/src/bioregistry/data/external/ecoportal/curation.tsv`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/data/external/ecoportal/processed.json` & `bioregistry-0.9.4/src/bioregistry/data/external/ecoportal/processed.json`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/data/external/ecoportal/raw.json` & `bioregistry-0.9.4/src/bioregistry/data/external/ecoportal/raw.json`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/data/external/edam/curation.tsv` & `bioregistry-0.9.4/src/bioregistry/data/external/edam/curation.tsv`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/data/external/edam/processed.json` & `bioregistry-0.9.4/src/bioregistry/data/external/edam/processed.json`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/data/external/fairsharing/curation.tsv` & `bioregistry-0.9.4/src/bioregistry/data/external/fairsharing/curation.tsv`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 FAIRsharing.18je7e	ONSTR	Ontology for Newborn Screening Follow-up and Translational Research	Ontology for Newborn Screening Follow-up and Translational Research (ONSTR) is an application ontology for representing data entities, practices and knowledge in the domain of newborn screening and short-­‐ and long-­‐term follow-­‐up of patients diagnosed with inheritable and congenital disorders. No project homepage could be found, and the resource has not been updated recently. Please get in touch if you have information about this resource.
 FAIRsharing.1b84nz	BCT	Behaviour Change Technique Taxonomy	The BCT Taxonomy Version 1 (BCTTv1) project are to (i) develop a reliable and generalisable nomenclature of behaviour change techniques as a method for specifying, evaluating and implementing complex behavioural change interventions and (ii) achieve its multidisciplinary and international acceptance and use to allow for its continuous development. Although this resource is available at BioPortal, and described at the listed homepage, the project homepage cannot be found. Please get in touch if you have any information
 FAIRsharing.1d817c	AGLDWG PID Namespace	Australian Government Link Data Working Group Persistent Identification Namespace	"The Australian Government Linked Data Working Group (AGLDWG) advocates the use of Linked Data as a particular set of technologies to be used for Internet-distributed, machine-readable data and, due to this, advocates the use of Internationalized Resource Identifiers (IRIs) as identifiers for things.
 
 The linked.data.gov.au namespace was implemented by the AGLDWG to govern Linked Data resources for Australia. The namespace uses pattern which can be used to create individual PIDs for infinitely many persistent identifiers for Australian Government Linked Data resources. The namespace uses a domain name that is not coupled to a particular agency's name or function. Use of this namespace was initiated in 2016 and then strengthened in 2018 with multiple Australian government agencies signing a Memorandum of Understanding to reserve the use of linked.data.gov.au for PID IRIs and to ensure its operational stability. The AGLDWG has adopted the IS0 19135 for IRI registration procedure and roles and issued Guidelines that details its PID allocation process."
 FAIRsharing.1dppze	MEDO	Mouse Experimental Design Ontology	Record does not exist anymore: Mouse Experimental Design Ontology. The record with identifier content 10.25504/FAIRsharing.1dppze was invalid.
 FAIRsharing.1esk4f	AI/RHEUM	Artificial Intelligence Rheumatology Consultant System Ontology	AI/RHEUM is used for the diagnosis of rheumatologic diseases. AI/RHEUM contains findings, such as clinical signs, symptoms, laboratory test results, radiologic observations, tissue biopsy results, and intermediate diagnosis hypotheses. Findings and hypotheses, which include definitions, are used to reach diagnostic conclusions with definite, probable, or possible certainty. AI/RHEUM is used by clinicians and informatics researchers.
-FAIRsharing.1g5j3h	BMT	Biomedical Topics	An ontology of biological and biomedical topics, created from merging the EDAM Topics sub-ontology with auxiliary topics that are out of scope of EDAM.
+FAIRsharing.1g5j3h	BMT	Biomedical Topics	Record does not exist anymore: Biomedical Topics. The record with identifier content 10.25504/FAIRsharing.1g5j3h was invalid.
 FAIRsharing.1h49c6	UNITSONT	Sleep Domain Units Ontology	An ontology for the units of measurement developed during the development of the Sleep Domain Ontology (SDO). It supports the use of SDO within the PhysioMIMI application. No official homepage for this resource can be found.
 FAIRsharing.1sgm8q		BioModels Ontology	The BioModels Ontology is an OWL Representation of the models in the BioModels repository. This resource has not been updated recently within BioPortal, and no official homepage can be found, therefore we have marked its status as Uncertain. Please get in touch with us if you have any information on this project.
 FAIRsharing.1wm8em	HRDO	Disease core ontology applied to Rare Diseases	This resource was designed during a PhD in medical informatics (funded by INSERM, 2010-2012). Its components are (i) a core ontology consistent with a metamodel (disorders and groups of disorders, genes, clinical signs and their relations) and (ii) an instantiation of this metamodel with Orphanet Data (available on http://orphadata.org). </ br> Research experiments demonstrated (i) efficient classifications generation based on SPARQL Construct, (ii) perspectives in semantic audit of a knowledge base, (iii) semantic comparison with OMIM (www.omim.org) using proximity measurements and (iv) opened perspectives in knowledge sharing (LORD, http://lord.bndmr.fr).  Current production services of Orphanet developed ORDO, released in 2014, an ontology synchronized with their production database. This ontology is now available on Bioportal.
 FAIRsharing.1xr6v0	SSE	Surgical Secondary Events	Memorial Sloan-Kettering Cancer Center Surgical Secondary Events Ontology (Adverse Events)
 FAIRsharing.1z28wz	suicideo	suicideonto	ontology for suicidology
 FAIRsharing.21gwxs	WHO-ART	WHO Adverse Reaction Terminology	WHO Adverse Reaction Terminology is a standardization of the vocabulary for adverse reactions.
 FAIRsharing.22j4p7	PO_PAE	Plant Anatomy	Plant Anatomy is a controlled vocabulary of plant morphological and anatomical structures representing organs, tissues, cell types, and their biological relationships based on spatial and developmental organization. This standard is now part of PO.
@@ -162,15 +162,14 @@
 FAIRsharing.97z25b	GML3.0	Ontology for Geography Markup Language	The Geography Markup Language (GML) is an RDF encoding for the transport and storage of geographic information, including both the geometry and properties of geographic features. Vocabulary terms are declared using OWL language to support RDF applications.
 FAIRsharing.9918b9	PATHLEX	Anatomic Pathology Lexicon	PathLex, a comprehensive lexicon—a unified language of anatomic pathology terms—for standardized indexing and retrieval of anatomic pathology information resources.
 FAIRsharing.99t4hg	ADMIN	Nurse Administrator	This is an ontology showing a nurse administrator's process domain
 FAIRsharing.9d08ks	NMOBR	NeuroMorpho.Org brain region ontologies	"The NeuroMorpho.Org brain region ontologies adopts and integrates relevant portions of available taxonomies (or lineages) ""as needed"" based on the existing knowledge that is openly accessible. For standardization purposes, cell types and other experimental metadata hierarchies are also added to OntoSearch v2.0. Concepts with insufficient knowledge are not classified as hierarchies, such as molecular, firing, and ""other"" unclassifiable properties of cell types. The species, brain regions and cell types are integrated into a single ontology for enabling OntoSearch functionality to mine NeuroMorpho.Org."
 FAIRsharing.9d38e2	URL	Uniform Resource Locator	"URL (Uniform Resource Locator) – the typical ""address"" of web content. It is a kind of URI (Uniform Resource Identifier) that begins with ""http://"" and consists of a string of characters used to identify or name a resource on the Internet. Such identification enables interaction with representations of the resource over a network, typically the World Wide Web, using the HTTP protocol. Well-managed URL redirection can make URLs as persistent as any identifier. Resolution depends on HTTP redirection and can be managed through an API or a user interface. A URL is a type of URI that identifies a resource via a representation of its primary access mechanism (e.g., its network ""location""), rather than by some other attributes it may have (see https://www.w3.org/TR/uri-clarification/#contemporary)."
 FAIRsharing.9pm45h	DDO	Diabetes Mellitus Diagnosis Ontology	An ontology for diagnosis of diabetes containing the diabetes related complications, symptoms, drugs, lab tests, etc.
 FAIRsharing.9psjsk	OPE	Ontology of Physical Exercises	The Ontology of Physical Exercises (OPE) provides a reference for describing an exercise in terms of functional movements, engaged musculoskeletal system parts, related equipment or monitoring devices, intended health outcomes, as well as target ailments for which the exercise might be employed as a treatment or preventative measure.
-FAIRsharing.9ry4cz	GMM	GoMapMan	GoMapMan is an open web-accessible resource for gene functional annotations in the plant sciences. It was developed to facilitate improvement, consolidation and visualization of gene annotations across several plant species.
 FAIRsharing.9sza27	GMO	Growth Medium Onotology	A structured controlled vocabulary for describing ingredients that constitute microbial growth media used in biological research centers.
 FAIRsharing.9thw6y	HIVCRS	HIVCompoundRels	The Ontology to express the ternary relations of HIV1
 FAIRsharing.9xcr4z	CIDOC-CRM	CIDOC Conceptual Reference Model	"The CIDOC Conceptual Reference Model (CRM) provides definitions and a formal structure for describing the implicit and explicit concepts and relationships used in cultural heritage documentation. The overall scope of the CIDOC CRM can be summarised in simple terms as the curated, factual knowledge
 about the past at a human scale. The CIDOC CRM is intended to promote a shared understanding of cultural heritage information by providing a common and extensible semantic framework that any cultural heritage information can be mapped to. It is intended to be a common language for domain experts and implementers to formulate requirements for information systems and to serve as a guide for good practice of conceptual modelling. In this way, it can provide the ""semantic glue"" needed to mediate between different sources of cultural heritage information, such as that published by museums, libraries and archives. The ISO 21127:2014 specification (Information and documentation — A reference ontology for the interchange of cultural heritage information) was created from the CIDOC CRM, although the CIDOC CRM Special Interest Group continues to maintain this original document as well."
 FAIRsharing.9y3gv0	ESFO	Enzyme Structure Function Ontology	The ESFO provides a new paradigm for organizing enzyme sequence, structure, and function information, whereby specific elements of enzyme sequence and structure are mapped to specific conserved aspects of function, thus facilitating the functional annotation of uncharacterized enzymes. The ESFO helps prevent misannotation by emphasizing annotation of enzymes only at the level of functional granularity warranted by available information. The archive is a static snapshot of the data in the SFLD as of April 2019, and will not be updated
 FAIRsharing.9yf7w3	GDCO	Data Collection Ontology	The Data Collection Ontology (DCO) is an ontology designed for data collection providing classes and relations on top of the Basic Formal Ontology (BFO) to facilitate data collection processes, subjects, and data anaylsis through the use of classifiers. DCO is based on the notion of reasoning to validate incoming data through their definitions based on classifiers.
 FAIRsharing.9yHHCp		Electronics and Optoelectronics Vocabulary	Vocabulary used for indexing bibliographical records dealing with “Electronics” in the PASCAL database, until 2014. This resource consists of 4454 entries in 3 languages (English, French and Spanish) classified under 19 collections.
@@ -319,14 +318,15 @@
 FAIRsharing.gt5K7W		Vocabulary of Heat Transfers	Controlled vocabulary used for indexing bibliographical records dealing with “Classical Thermodynamics / Heat Transfers” in the PASCAL database (1972 à 2015). This vocabulary reflects the content of the indexed articles, including the experimental and/or theoretical context in which the heat transfer phenomena were studied. The resource is aligned with Rameau and LCSH. It consists of 1462 entries in 2 languages (English, French) grouped under 7 collections.
 FAIRsharing.gvr3p6	APAEDUCLUSTER	Educational Cluster	APA Educational Cluster, URI based ontology load
 FAIRsharing.GWEIFA	landform	ASLS - Landform classifiers	Machine-readable representation of the classifiers described in chapter 5 Landform, by J.G. Speight, in Australian soil and land survey field handbook (3rd edn). In this technique for describing landforms, the whole land surface is viewed as a mosaic of tiles of odd shapes and sizes. The scheme is intended to produce a record of observations rather than inferences. The data was converted from the print representation to this linked-data form by Linda Gregory assisted by Simon J D Cox.
 FAIRsharing.h0can5	DOCCC	Diagnosis Ontology of Clinical Care Classification	Record does not exist anymore: Diagnosis Ontology of Clinical Care Classification. The record with identifier content 10.25504/FAIRsharing.h0can5 was invalid.
 FAIRsharing.h1gmb7	DURUM_WHEAT	Durum Wheat	The durum wheat ontology (DURUM_WHEAT) is dedicated to the sustainability analysis of the durum wheat chain. Current data available on this ontology concern durum wheat quality control criteria used in different countries (Moisture content rate, chemical content, etc.).
 FAIRsharing.h4rs6h	GO-PLUS	GO-PLUS	This is the fully axiomatised version of the Gene Ontology (GO). It includes cross-ontology relationships (axioms) and imports additional required ontologies including ChEBI, Cell Ontology and Uberon. It also includes a complete set of relationship types including some not in go.obo/go.owl. This version is only available in OWL format.
 FAIRsharing.h94kv6	OntoVIP	Medical image simulation	The OntoVIP ontology was developed in the context of the Virtual Imaging Platform project (VIP), a french project supported by ANR (ANR-09-COSI-03 grant) aiming at sharing medical image simulation resources. This ontology describes the content of the models used in medical image simulation. This ontology can be used to annotate such models in order to highlight the different entities that are present in the 3D scene to be imaged, i.e. anatomical structures, pathological structures, foreign bodies, contrast agents etc. The model allows also to associate to these entities information about their physical qualities, which are used in the medical image simulation process (to mimick physical phenomena involved in CT, MR, US and PET imaging). This ontology partly relies on the OntoNeuroLOG ontology (ONL-DP ONL-MR-DA), as well as PATO, RadLex, FMA and ChEBI.
+FAIRsharing.hgsFLe	DwC-germplasm	Darwin Core Germplasm	The Darwin Core germplasm extension (DwC-germplasm) was developed to provide a bridge between the established standards in use by the genebank community for plant genetic resources for food and agriculture (PGRFA) and the standards maintained by the Biodiversity Information Standards/Taxonomic Databases Working Group (TDWG). The DwC-germplasm provides an extension to the Darwin Core standard of the TDWG for occurrences. Darwin Core can be seen as an extension to the Dublin Core Metadata Data Initiative (DCMI) terms.
 FAIRsharing.hmhzhy	CNO_ACRONYM	CNO_NAME	Record does not exist anymore: CNO_NAME. The record with identifier content 10.25504/FAIRsharing.hmhzhy was invalid.
 FAIRsharing.hpmpyx	CanCO	Cancer Chemoprevention Ontology	The Cancer Chemoprevention Ontology constitutes a vocabulary that is able to describe and semantically interconnect the different paradigms of the cancer chemoprevention domain.
 FAIRsharing.hqyeb7	FIRE	Fire Ontology	The ontology of Fire was created in order to represent the set of concepts about the fire occurring in natural vegetation, its characteristics, causes and effects, with focus on Cerrado vegetation domain. The fire plays a determinant role on the structure and composition of Cerrado physiognomies.
 FAIRsharing.hs43fc	FISHO	Fish Ontology	"This Fish Ontology is an ontology created as how the author views the fish structure following the book ""The Diversity of Fishes: Biology, Evolution and Ecology"" as the main reference, which covers one part of view on ichthyology, with an emphasis on diversity and adaptation. This ontology is created with the mindset of categorizing fish automatically based on the attributes and terms mined from the fish specimen. Most of the basic organization from this ontology follows Nelson's research due to its synthetic and broad approach, while recognizing that Nelson's conclusions are one of many alternative interpretations of the literature, which is mostly agreed by our main references, and many fish and fisheries researchers. Most of the classification used in this ontology is in no means completed and just following the recent classification provided by the books For now our work focused more on two group of fish which is early jawless fish, and advanced jawed fishes. The classification from both of this group are structured following the reference."
 FAIRsharing.htq39f	COMODI	COMODI	An ontology to characterise differences in versions of computational models in biology
 FAIRsharing.hve0ac	TRANSMAT	Matter Transfer Ontology	The Matter Transfer ontology is dedicated to matter transfer (eg O2, CO2, H2O) and mechanical properties of materials especially with respect to food, bacteria and packaging fields.
 FAIRsharing.hw5gr6	HEIO	Regional Healthcare System Interoperability and Information Exchange Measurement Ontology	The purpose of this ontology is to develop a model for regional healthcare system interoperability and information exchange quantification (measured by the electronic health information exchange (eHIE) indicator). The eHIE is hypothesized as a leading measure of regional healthcare system integration. A publication associated with this ontology is currently under review.
```

### Comparing `bioregistry-0.9.3/src/bioregistry/data/external/fairsharing/processed.json` & `bioregistry-0.9.4/src/bioregistry/data/external/fairsharing/processed.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9975388463175819%*

 * *Differences: {"'FAIRsharing.1g5j3h'": "{'description': 'Record does not exist anymore: Biomedical Topics. The "*

 * *                         'record with identifier content 10.25504/FAIRsharing.1g5j3h was '*

 * *                         "invalid.', 'subjects': {delete: [2]}}",*

 * * "'FAIRsharing.4bcrzk'": "{'subjects': {delete: [2]}}",*

 * * "'FAIRsharing.fe4816'": "{'subjects': {delete: [2]}}",*

 * * "'FAIRsharing.gkw1w8'": "{'description': 'Record does not exist anymore: Psychology Ontology. The "*

 * *                         'record with ident […]*

```diff
@@ -413,22 +413,21 @@
             "Chemical Biology",
             "Biomedical Science",
             "Biology"
         ]
     },
     "FAIRsharing.1g5j3h": {
         "abbreviation": "BMT",
-        "description": "An ontology of biological and biomedical topics, created from merging the EDAM Topics sub-ontology with auxiliary topics that are out of scope of EDAM.",
+        "description": "Record does not exist anymore: Biomedical Topics. The record with identifier content 10.25504/FAIRsharing.1g5j3h was invalid.",
         "homepage": "http://bioportal.bioontology.org/ontologies/BMT",
         "name": "Biomedical Topics",
         "publications": [],
         "subjects": [
             "Engineering Science",
-            "Life Science",
-            "Ontology and Terminology"
+            "Life Science"
         ]
     },
     "FAIRsharing.1gr4tz": {
         "abbreviation": "EFO",
         "contact": {
             "email": "siiraa@ebi.ac.uk",
             "name": "Sirarat Sarntivijai",
@@ -1785,16 +1784,15 @@
         "abbreviation": "CYTO",
         "description": "It is flat ontology showing cytokine synonyms. It has been produced by merging cytokine branches, using SOMA (Synonym Ontology Mapping Approach) method, of 10 Bioportal ontologies.",
         "homepage": "http://bioportal.bioontology.org/ontologies/CYTO",
         "name": "CYTOKINE",
         "publications": [],
         "subjects": [
             "Molecular Infection Biology",
-            "Immunology",
-            "Ontology and Terminology"
+            "Immunology"
         ]
     },
     "FAIRsharing.4c0b6b": {
         "abbreviation": "UBERON",
         "description": "Uberon is an integrated cross-species anatomy ontology covering animals and bridging multiple species-specific ontologies. It represents a variety of entities classified according to traditional anatomical criteria such as structure, function and developmental lineage. The ontology includes comprehensive relationships to taxon-specific anatomical ontologies, allowing integration of functional, phenotype and expression data.",
         "homepage": "http://uberon.org/",
         "license": "CC-BY-3.0",
@@ -4281,32 +4279,14 @@
         "subjects": [
             "Functional Genomics",
             "Biomedical Science",
             "Epidemiology",
             "Population Genetics"
         ]
     },
-    "FAIRsharing.9ry4cz": {
-        "abbreviation": "GMM",
-        "description": "GoMapMan is an open web-accessible resource for gene functional annotations in the plant sciences. It was developed to facilitate improvement, consolidation and visualization of gene annotations across several plant species.",
-        "homepage": "https://gomapman.nib.si/",
-        "license": "CC BY-NC-SA 3.0",
-        "name": "GoMapMan",
-        "publications": [
-            {
-                "doi": "10.1093/nar/gkt1056",
-                "pubmed_id": null,
-                "title": "GoMapMan: integration, consolidation and visualization of plant gene annotations within the MapMan ontology"
-            }
-        ],
-        "subjects": [
-            "Proteomics",
-            "Ontology and Terminology"
-        ]
-    },
     "FAIRsharing.9sza27": {
         "abbreviation": "GMO",
         "description": "A structured controlled vocabulary for describing ingredients that constitute microbial growth media used in biological research centers.",
         "homepage": "https://github.com/skwsm/gmo",
         "name": "Growth Medium Onotology",
         "publications": [],
         "subjects": [
@@ -8073,16 +8053,15 @@
                 "doi": "10.1038/d41586-019-01715-4",
                 "pubmed_id": null,
                 "title": "Credit data generators for data reuse"
             }
         ],
         "subjects": [
             "Data Quality",
-            "Subject Agnostic",
-            "Ontology and Terminology"
+            "Subject Agnostic"
         ],
         "twitter": "contrib_roles"
     },
     "FAIRsharing.fee65c": {
         "abbreviation": null,
         "description": "The iDAI.world thesaurus collects and unifies all thesauri and vocabularies of the libraries and the projects of the German Archaeological Institute. It was developed between 2015 and 2019, since 2020 it is continuously updated and implemented. The core structure is based on the  BackBoneThesaurus (https://vocabs.dariah.eu/bbt/en/). Please note that while a majority of this site is in German, the thesaurus itself is mainly multi-lingual. ",
         "homepage": "http://thesauri.dainst.org/de.html",
@@ -8494,21 +8473,20 @@
         ],
         "subjects": [
             "Biomedical Science"
         ]
     },
     "FAIRsharing.gkw1w8": {
         "abbreviation": "APAONTO",
-        "description": "APA thesaurus . Flat ontology file",
+        "description": "Record does not exist anymore: Psychology Ontology. The record with identifier content 10.25504/FAIRsharing.gkw1w8 was invalid.",
         "homepage": "http://bioportal.bioontology.org/ontologies/APAONTO",
         "name": "Psychology Ontology",
         "publications": [],
         "subjects": [
-            "Psychology",
-            "Ontology and Terminology"
+            "Psychology"
         ]
     },
     "FAIRsharing.gq1xtx": {
         "abbreviation": "IAO",
         "contact": {
             "email": "alanruttenberg@gmail.com",
             "name": "Alan Ruttenberg",
@@ -8638,14 +8616,34 @@
             }
         ],
         "repository": "https://github.com/OBF/FALDO",
         "subjects": [
             "Genetics"
         ]
     },
+    "FAIRsharing.hgsFLe": {
+        "abbreviation": "DwC-germplasm",
+        "contact": {
+            "email": "dag.endresen@gmail.com",
+            "name": "Dag Endresen",
+            "orcid": "0000-0002-2352-5497"
+        },
+        "description": "The Darwin Core germplasm extension (DwC-germplasm) was developed to provide a bridge between the established standards in use by the genebank community for plant genetic resources for food and agriculture (PGRFA) and the standards maintained by the Biodiversity Information Standards/Taxonomic Databases Working Group (TDWG). The DwC-germplasm provides an extension to the Darwin Core standard of the TDWG for occurrences. Darwin Core can be seen as an extension to the Dublin Core Metadata Data Initiative (DCMI) terms.",
+        "homepage": "https://github.com/dagendresen/darwincore-germplasm",
+        "license": "CC0-1.0",
+        "name": "Darwin Core Germplasm",
+        "publications": [],
+        "subjects": [
+            "Genetics",
+            "Biodiversity",
+            "Agriculture",
+            "Biology",
+            "Plant Genetics"
+        ]
+    },
     "FAIRsharing.hmhzhy": {
         "abbreviation": "CNO_ACRONYM",
         "description": "Record does not exist anymore: CNO_NAME. The record with identifier content 10.25504/FAIRsharing.hmhzhy was invalid.",
         "homepage": "http://bioportal.bioontology.org/ontologies/CNO_ACRONYM",
         "name": "CNO_NAME",
         "publications": [],
         "subjects": []
```

### Comparing `bioregistry-0.9.3/src/bioregistry/data/external/go/curation.tsv` & `bioregistry-0.9.4/src/bioregistry/data/external/go/curation.tsv`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/data/external/go/processed.json` & `bioregistry-0.9.4/src/bioregistry/data/external/go/processed.json`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/data/external/go/raw.yml` & `bioregistry-0.9.4/src/bioregistry/data/external/go/raw.yml`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/data/external/hl7/curation.tsv` & `bioregistry-0.9.4/src/bioregistry/data/external/hl7/curation.tsv`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/data/external/miriam/processed.json` & `bioregistry-0.9.4/src/bioregistry/data/external/miriam/processed.json`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/data/external/miriam/raw.json` & `bioregistry-0.9.4/src/bioregistry/data/external/miriam/raw.json`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/data/external/n2t/processed.json` & `bioregistry-0.9.4/src/bioregistry/data/external/n2t/processed.json`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/data/external/n2t/raw.yml` & `bioregistry-0.9.4/src/bioregistry/data/external/n2t/raw.yml`

 * *Files 0% similar despite different names*

```diff
@@ -8829,14 +8829,22 @@
   type: "naan"
   manager: "n2t"
   name: "Congo Research Papers (=) CRP"
   date: "2023.04.25"
   redirect: "https://congoresearchpapers.net/ark:$id"
   na_policy: "NP | (:unkn) unknown | 2023 |"
 
+ark:/19500:
+  type: "naan"
+  manager: "n2t"
+  name: "HiRADa (=) MAFIL"
+  date: "2023.05.02"
+  redirect: "http://www.mafil.org/ark:$id"
+  na_policy: "NP | (:unkn) unknown | 2023 |"
+
 ark:/99166/p9:
   type: "shoulder"
   name: "EZID CDL agents (=) EZAGENTS"
   date: "2010.09.01"
   redirect: "https://n2t.net/ark:$id"
   how: "NP | NR, OP, CC | 2010 |"
 
@@ -38435,8 +38443,8 @@
   redirect: "http://purl.obolibrary.org/obo/$id"
 
 zifdb:
   type: "commonspfx"
   redirect: "http://bindr.gdcb.iastate.edu:8080/ZiFDB/controller/checkArticle?artId=$id"
 
 
-# 4335 added prefixes
+# 4336 added prefixes
```

### Comparing `bioregistry-0.9.3/src/bioregistry/data/external/ncbi/curation.tsv` & `bioregistry-0.9.4/src/bioregistry/data/external/ncbi/curation.tsv`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/data/external/ncbi/processed.json` & `bioregistry-0.9.4/src/bioregistry/data/external/ncbi/processed.json`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/data/external/ncbi/raw.html` & `bioregistry-0.9.4/src/bioregistry/data/external/ncbi/raw.html`

 * *Files 0% similar despite different names*

#### Comparing `bioregistry-0.9.3/src/bioregistry/data/external/ncbi/raw.html` & `bioregistry-0.9.4/src/bioregistry/data/external/ncbi/raw.html`

```diff
@@ -30,15 +30,15 @@
     <meta name="modified" content="2021-10-25T17:46:25Z"/>
     <meta xmlns:ncbi-portal="http://ncbi.gov/portal/XSLT/namespace" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" name="cms-edit-aux-url" content="http://cms.ncbi.nlm.nih.gov/node//edit"/>
     <!-- Page headcontent end -->
     <!-- PageFixtures resources begin -->
     <link xmlns="http://www.w3.org/1999/xhtml" type="text/css" rel="stylesheet" href="//static.pubmed.gov/portal/portal3rc.fcgi/4208398/css/4207974/4206132.css" xml:base="http://127.0.0.1/sites/static/header_footer"/>
     <!-- PageFixtures resources end -->
     <link rel="shortcut icon" href="//www.ncbi.nlm.nih.gov/favicon.ico"/>
-    <meta name="ncbi_phid" content="CE8934E745199A210000000003200290.m_6"/>
+    <meta name="ncbi_phid" content="CE8A3634452C72C100000000085006A1.m_5"/>
     <meta name="referrer" content="origin-when-cross-origin"/>
     <link type="text/css" rel="stylesheet" href="//static.pubmed.gov/portal/portal3rc.fcgi/4181609/css/4121862/3974050/3917732/251717/4108189/14534/45193/3534283/4128070/3407145/4005757/4062871.css"/>
     <link type="text/css" rel="stylesheet" href="//static.pubmed.gov/portal/portal3rc.fcgi/4181609/css/3529741/3529739.css" media="print"/>
   </head>
   <body class=" col2  custom-page">
     <div class="grid">
       <div class="col twelve_col nomargin shadow">
@@ -3248,17 +3248,17 @@
             <div id="NCBIFooter_dynamic">
               <div class="breadcrumbs">
                 You are here:
                 <span id="breadcrumb_text">
                   <a href="/guide/">NCBI</a>
                 </span>
               </div>
-              <a id="help-desk-link" class="help_desk" href="https://support.ncbi.nlm.nih.gov/ics/support/default.asp?Time=2023-05-02T21:01:25-04:00&amp;Snapshot=%2Fprojects%2Fstaticsites%2Fgenbank%2Fgenbank@2.20&amp;Host=portal102&amp;ncbi_phid=CE8934E745199A210000000003200290&amp;ncbi_session=CE8934E7451B2651_0800SID&amp;from=https%3A%2F%2Fwww.ncbi.nlm.nih.gov%2Fgenbank%2Fcollab%2Fdb_xref%2F&amp;Ncbi_App=genbank&amp;Page=custom-page&amp;style=classic&amp;deptID=28049" target="_blank">Support Center</a>
+              <a id="help-desk-link" class="help_desk" href="https://support.ncbi.nlm.nih.gov/ics/support/default.asp?Time=2023-05-03T20:59:38-04:00&amp;Snapshot=%2Fprojects%2Fstaticsites%2Fgenbank%2Fgenbank@2.20&amp;Host=portal103&amp;ncbi_phid=CE8A3634452C72C100000000085006A1&amp;ncbi_session=CE8A363445303791_2128SID&amp;from=https%3A%2F%2Fwww.ncbi.nlm.nih.gov%2Fgenbank%2Fcollab%2Fdb_xref%2F&amp;Ncbi_App=genbank&amp;Page=custom-page&amp;style=classic&amp;deptID=28049" target="_blank">Support Center</a>
               <noscript>
-                <img alt="" src="/stat?jsdisabled=true&amp;ncbi_app=genbank&amp;ncbi_db=&amp;ncbi_pdid=custom-page&amp;ncbi_phid=CE8934E745199A210000000003200290"/>
+                <img alt="" src="/stat?jsdisabled=true&amp;ncbi_app=genbank&amp;ncbi_db=&amp;ncbi_pdid=custom-page&amp;ncbi_phid=CE8A3634452C72C100000000085006A1"/>
               </noscript>
             </div>
             <div xmlns:xi="http://www.w3.org/2001/XInclude">
               <div xmlns="http://www.w3.org/1999/xhtml" class="footer" id="footer" xml:base="http://127.0.0.1/sites/static/header_footer">
                 <section class="icon-section">
                   <div id="icon-section-header" class="icon-section_header">Follow NCBI</div>
                   <div class="grid-container container">
@@ -3465,12 +3465,12 @@
         <span class="PAFAppResources"/>
       </div>
       <!-- /.twelve_col -->
     </div>
     <!-- /.grid -->
     <!-- usually for JS scripts at page bottom -->
     <span class="pagefixtures"/>
-    <!-- CE8934E7451B2651_0800SID /projects/staticsites/genbank/genbank@2.20 portal102 v4.1.r643667 Fri, Jan 14 2022 01:18:35 -->
-    <span id="portal-csrf-token" style="display:none" data-token="CE8934E7451B2651_0800SID"/>
+    <!-- CE8A363445303791_2128SID /projects/staticsites/genbank/genbank@2.20 portal103 v4.1.r643667 Fri, Jan 14 2022 01:18:35 -->
+    <span id="portal-csrf-token" style="display:none" data-token="CE8A363445303791_2128SID"/>
     <script type="text/javascript" src="//static.pubmed.gov/portal/portal3rc.fcgi/4181609/js/3879255/4121861/1490097/4087685.js" snapshot="genbank"/>
   </body>
 </html>
```

### Comparing `bioregistry-0.9.3/src/bioregistry/data/external/obofoundry/processed.json` & `bioregistry-0.9.4/src/bioregistry/data/external/obofoundry/processed.json`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/data/external/obofoundry/raw.yaml` & `bioregistry-0.9.4/src/bioregistry/data/external/obofoundry/raw.yaml`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/data/external/ols/processed.json` & `bioregistry-0.9.4/src/bioregistry/data/external/ols/processed.json`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/data/external/ols/raw.json` & `bioregistry-0.9.4/src/bioregistry/data/external/ols/raw.json`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/data/external/ontobee/curation.tsv` & `bioregistry-0.9.4/src/bioregistry/data/external/ontobee/curation.tsv`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/data/external/ontobee/processed.json` & `bioregistry-0.9.4/src/bioregistry/data/external/ontobee/processed.json`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/data/external/ontobee/raw.html` & `bioregistry-0.9.4/src/bioregistry/data/external/ontobee/raw.html`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/data/external/prefixcommons/curation.tsv` & `bioregistry-0.9.4/src/bioregistry/data/external/prefixcommons/curation.tsv`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/data/external/prefixcommons/processed.json` & `bioregistry-0.9.4/src/bioregistry/data/external/prefixcommons/processed.json`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/data/external/prefixcommons/raw.tsv` & `bioregistry-0.9.4/src/bioregistry/data/external/prefixcommons/raw.tsv`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/data/external/re3data/curation.tsv` & `bioregistry-0.9.4/src/bioregistry/data/external/re3data/curation.tsv`

 * *Files 0% similar despite different names*

```diff
@@ -3589,15 +3589,15 @@
 r3d100013298	Coronavirus Antiviral Research Database	https://covdb.stanford.edu/	The Coronavirus Antiviral Research Database is designed to expedite the development of SARS-CoV-2 antiviral therapy. It will benefit global coronavirus drug development efforts by (1) promoting uniform reporting of experimental results to facilitate comparisons between different candidate antiviral compounds; (2) identifying gaps in coronavirus antiviral drug development research; (3) helping scientists, clinical investigators, public health officials, and funding agencies prioritize the most promising compounds and repurposed drugs for further development; (4) providing an objective, evidenced-based, source of information for the public; and (5) creating a hub for the exchange of ideas among coronavirus researchers whose feedback is sought and welcomed. By comprehensively reviewing all published laboratory, animal model, and clinical data on potential coronavirus therapies, the Database makes it unlikely that promising treatment approaches will be overlooked. In addition, by making it possible to compare the underlying data associated with competing treatment strategies, stakeholders will be better positioned to prioritize the most promising anti-coronavirus compounds for further development.
 r3d100013299	Liverpool COVID-19 Drug Interactions	https://www.covid19-druginteractions.org/	The COVID-19 pandemic has affected every country in the world. It is well documented that those most susceptible to the worst outcomes of COVID-19 are the immunocompromised and those with underlying comorbidities. Therefore, patients requiring treatment for COVID-19 will also be on additional medication, posing a risk for drug-drug interactions (DDIs). In order to address this, the Liverpool Drug Interactions website team developed this freely available drug interactions resource to provide information on the likelihood of interactions between the experimental agents used for the treatment of COVID-19 and commonly prescribed co-medications.
 r3d100013300	COVID-19 Research Collaborations	https://covid19.elsevierpure.com/	"Research Collaborators & Institutions related to Coronavirus Epidemic
 Aim: Identify potential research experts or collaborators in areas related to the coronavirus epidemic across basic science, translational research, or clinical practice.
 Scope: A selection of Researchers active or cited in the area of Coronavirus, Middle East Respiratory Syndrome (MERS), SARS, etc."
 r3d100013301	DisGeNET	http://www.disgenet.org	DisGeNET is a discovery platform containing one of the largest publicly available collections of genes and variants associated to human diseases.  DisGeNET integrates data from expert curated repositories, GWAS catalogues, animal models and the scientific literature. DisGeNET data are homogeneously annotated with controlled vocabularies and community-driven ontologies. Additionally, several original metrics are provided to assist the prioritization of genotype–phenotype relationships.
 r3d100013302	EU Clinical Trial Register	https://www.clinicaltrialsregister.eu/	The European Union Clinical Trials Register allows you to search for protocol and results information on interventional clinical trials that are conducted in the European Union (EU) and the European Economic Area (EEA) and clinical trials conducted outside the EU / EEA that are linked to European paediatric-medicine development. The EU Clinical Trials Register is part of EudraPharm, which is the community database of authorised medicinal products. The website provides public access to information extracted from the  European Union Drug Regulating Authorities Clinical Trials Database, EudraCT.
-r3d100013303	Risklayer Explorer	http://risklayer-explorer.com/	"Risklayer Explorer is a collaboration between Risklayer GmbH and the Karlsruhe Institute of Technology's Center for Disaster Risk Management and Risk Reduction Technology (CEDIM). This website is still under development, but we are going live with it already, because we want to present data on the Novel Coronavirus (COVID-19) to help inform the public of the current situation.
+r3d100013303	Risklayer Explorer	https://www.risklayer-explorer.com/	"Risklayer Explorer is a collaboration between Risklayer GmbH and the Karlsruhe Institute of Technology's Center for Disaster Risk Management and Risk Reduction Technology (CEDIM). This website is still under development, but we are going live with it already, because we want to present data on the Novel Coronavirus (COVID-19) to help inform the public of the current situation.
 You will be able to track disaster events and read about our analysis here. Our work is a continuation of a new style of disaster research started by CEDIM in 2011 to analyze disasters immediately after their occurrence, assess the impacts, and retrace the temporal development of disaster events. We are already analyzing damaging earthquakes globally, providing you with event characteristics, earthquake's intensity footprints, as well as the population affected by earthquakes. In addition to earthquake events, we expect to be tracking and analyzing tropical cyclone, volcano and extreme weather events in 2020."
 r3d100013304	European Centre for Disease Prevention and Control	https://www.ecdc.europa.eu/en	"ECDC is an EU agency aimed at strengthening Europe's defences against infectious diseases. The core functions cover a wide spectrum of activities: surveillance, epidemic intelligence, response, scientific advice, microbiology, preparedness, public health training, international relations, health communication, and the scientific journal Eurosurveillance.
 Within the field of its mission, the Centre shall:  search for, collect, collate, evaluate and disseminate relevant scientific and technical data; provide scientific opinions and scientific and technical assistance including training; provide timely information to the Commission, the Member States, Community agencies and international organisations active within the field of public health; coordinate the European networking of bodies operating in the fields within the Centre's mission, including networks that emerge from public health activities supported by the Commission and operating the dedicated surveillance networks; exchange information, expertise and best practices, and facilitate the development and implementation of joint actions."
 r3d100013305	Facebook Data for Good	https://dataforgood.fb.com/	To help flattening the COVID-19 curve  public health systems need better information on whether preventive measures are working and how the virus may spread. Facebook Data for Good offer maps on population movement that researchers and nonprofits are already using to understand the coronavirus crisis, using aggregated data to protect people’s privacy.
 r3d100013307	ISRCTN Registry	http://www.isrctn.com/	"The ISRCTN registry is a primary clinical trial registry recognised by WHO and ICMJE that accepts all clinical research studies (whether proposed, ongoing or completed), providing content validation and curation and the unique identification number necessary for publication. All study records in the database are freely accessible and searchable.
 ISRCTN supports transparency in clinical research, helps reduce selective reporting of results and ensures an unbiased and complete evidence base.
 ISRCTN accepts all studies involving human subjects or populations with outcome measures assessing effects on human health and well-being, including studies in healthcare, social care, education, workplace safety and economic development."
@@ -3644,15 +3644,15 @@
 r3d100013355	GePaRD	https://www.bips-institut.de/forschung/forschungsinfrastrukturen/gepard.html	Since 2004, the Leibniz Institute for Prevention Research and Epidemiology – BIPS has been working on the establishment and maintenance of the project-based German Pharmacoepidemiological Research Database (short GePaRD). GePaRD is based on claims data from statutory health insurance (SHI) providers and currently includes information on about 20 million persons who have been insured with one of the participating providers since 2004. Per data year, there is information on approximately 17% of the general population from all geographical regions of Germany.
 r3d100013356	Data Center - SAFE	https://safe-frankfurt.de/de/data-center.html	"Research on German and European financial markets suffers from a lack of pan-European data sets. Also, existing sets do not provide a standard identification of, for example, companies. Therefore, researchers often utilize data from the United States where the integration of different databases is more advanced. As a consequence, empirical analyses are mostly based on non-European data. Because of the institutional differences, political recommendations that result from these analyses cannot – or only in a limited scope – be transferred to Europe.
 Against this background, the SAFE Research Data Center not only draws on the usual international data sources but also creates new European data sets, brings existing data together and processes them. The aim is to place the central research areas of SAFE on a common European data footing.
 Data access is provided by 'SAFE data sources' https://datacenter.safefrankfurt.de/datacenter/_databases/ and 'FiF - Repositorium für Forschungsdaten aus dem Finanzbereich (Preview version)' https://fif.safe-frankfurt.de/xmlui/"
 r3d100013358	Infectious Diseases Data Observatory	https://www.iddo.org/	"The Infectious Diseases Data Observatory (IDDO) assembles clinical, laboratory and epidemiological data on a collaborative platform to be shared with the research and humanitarian communities. The data are analysed to generate reliable evidence and innovative resources that enable research-driven responses to the major challenges of emerging and neglected infections. Access is available to individual patient data held for malaria and Ebola virus disease. Resources for visceral leishmaniasis, schistosomiasis and soil transmitted helminths, Chagas disease and COVID-19 are under development.
 IDDO contains the following repositories : COVID-19 Data Platform, Chagas Data Platform, Schistosomiasis & Soil Transmitted Helminths Data Platform, Visceral Leishmaniasis Data Platform, Ebola Data Platform, WorldWide Antimalarial Resistance Network (WWARN)"
 r3d100013359	KORDS	https://kcl.figshare.com/	KORDS is a research data repository service providing long term storage and public access for datasets that support published research and/or have long term value.
-r3d100013362	Mountain Scholar	https://mountainscholar.org/	Mountain Scholar is an open access repository service that collects, preserves, and provides access to digitized library collections and other scholarly and creative works from several academic entities within the states of Colorado and Wyoming.
+r3d100013362	Mountain Scholar	https://mountainscholar.org/	Mountain Scholar is an open access repository service that collects, preserves, and provides access to digitized library collections and other scholarly and creative works from several academic entities within the state of Colorado. Colorado State University research data from the fall of 2022 and forward is available in Dryad; CSU legacy research data prior to fall 2022 is in Mountain Scholar.
 r3d100013364	Open Access Power-Grid Frequency Database	https://osf.io/m43tg/	"This repository stores and links the openly available power-grid frequency recordings across the globe.
 This database is comprised of open data existent across three dimensions: - TSO data: Transmission System's Operator (TSO) recordings made public; - Research projects: Open-data database research projects; - Independent Gatherings: Industrial, private, or personal recordings that were made publicly available."
 r3d100013365	IAGOS Data Centre	http://www.iagos-data.fr/	"IAGOS aims to provide long-term, regular and spatially resolved in situ observations of the atmospheric composition. The observation systems are deployed on a fleet of 10 to 15 commercial aircraft measuring atmospheric chemistry concentrations and meteorological fields.
 The IAGOS Data Centre manages and gives access to all the data produced within the project."
 r3d100013366	Most Wiedzy Open Research Data Catalog	https://mostwiedzy.pl/en/open-research-data/	"The nature of the ‘Bridge of Data’ project is to design and build a platform that allows collecting, searching, analyzing and sharing open research data and to provide it with unique data collected from the three most important Pomeranian universities: Gdańsk University of Technology, Medical University of Gdańsk and the University of Gdańsk. These data will be made available free of charge to the scientific community, entrepreneurs and the public. A bridge will be built to allow reuse of Open Research Data.
 
 The available research data will be described by standards developed by dedicated, experienced scientific teams. The metadata will allow other external computer systems to interpret the collected data. ORD descriptions will also include data reuse or reduction scenarios to facilitate further processing."
```

### Comparing `bioregistry-0.9.3/src/bioregistry/data/external/re3data/processed.json` & `bioregistry-0.9.4/src/bioregistry/data/external/re3data/processed.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998538246969209%*

 * *Differences: {"'r3d100011311'": "{'xrefs': {'fairsharing': 'FAIRsharing.1bb2c9'}}",*

 * * "'r3d100012504'": "{'xrefs': OrderedDict([('fairsharing', 'FAIRsharing.M2wo0O')])}",*

 * * "'r3d100012622'": "{'xrefs': {'fairsharing': 'FAIRsharing.a1c2cd'}}",*

 * * "'r3d100013107'": "{'xrefs': OrderedDict([('fairsharing.legacy', '4726')])}",*

 * * "'r3d100013303'": "{'homepage': 'https://www.risklayer-explorer.com/'}",*

 * * "'r3d100013325'": "{'xrefs': {'scr': '019260'}}",*

 * * "'r3d100013362'": "{'description': 'Mountain Scholar is an open access reposito […]*

```diff
@@ -12024,15 +12024,16 @@
         "name": "Taiwan Forestry Research Institute Data Catalog",
         "prefix": "r3d100011311",
         "synonyms": [
             "TFRI Data Catalog",
             "\u6797  \u696d  \u8a66  \u9a57  \u6240  \u7814  \u7a76  \u8cc7  \u6599  \u76ee  \u9304"
         ],
         "xrefs": {
-            "biodbcore": "001743"
+            "biodbcore": "001743",
+            "fairsharing": "FAIRsharing.1bb2c9"
         }
     },
     "r3d100011312": {
         "description": "Data from selected studies from the Abdul Latif Jameel Poverty Action Lab (J-PAL), povertyactionlab.org. A number of other studies from J-PAL have data posted on the MacArthur Dataverse: http://dvn.iq.harvard.edu/dvn/dv/macarthur.",
         "homepage": "https://dataverse.harvard.edu/dataverse/jpal",
         "name": "The Abdul Latif Jameel Poverty Action Lab",
         "prefix": "r3d100011312",
@@ -21290,15 +21291,18 @@
         "name": "NASA Image and Video Library",
         "prefix": "r3d100012503"
     },
     "r3d100012504": {
         "description": "NASA funded OpenAltimetry facilitates the advanced discovery, processing, and visualization services for ICESat and ICESat-2 altimeter data.",
         "homepage": "https://www.openaltimetry.org",
         "name": "OpenAltimetry",
-        "prefix": "r3d100012504"
+        "prefix": "r3d100012504",
+        "xrefs": {
+            "fairsharing": "FAIRsharing.M2wo0O"
+        }
     },
     "r3d100012505": {
         "description": "ORDaR is a data repository for research data in geoscience.",
         "homepage": "https://ordar.otelo.univ-lorraine.fr/accueil",
         "name": "ORDaR",
         "prefix": "r3d100012505",
         "synonyms": [
@@ -22112,15 +22116,16 @@
         "homepage": "https://edsf13.ingv.it/",
         "name": "The European Database of Seismogenic Faults",
         "prefix": "r3d100012622",
         "synonyms": [
             "EDSF"
         ],
         "xrefs": {
-            "doi": "10.6092/ingv.it-share-edsf"
+            "doi": "10.6092/ingv.it-share-edsf",
+            "fairsharing": "FAIRsharing.a1c2cd"
         }
     },
     "r3d100012623": {
         "description": "Yoda publishes research data on behalf of researchers that are affiliated with Utrecht University, its research institutes and consortia where it acts as a coordinating body.\nData packages are not limited to a particular field of research or license.\nYoda publishes data packages via Datacite. To find data publications use: https://public.yoda.uu.nl/ , or the Datacite search engine: https://search.datacite.org/repositories/delft.uu",
         "homepage": "https://www.uu.nl/en/research/yoda",
         "name": "Yoda",
         "prefix": "r3d100012623",
@@ -25305,15 +25310,18 @@
         "name": "e-Depot of the National Archives of the Netherlands",
         "prefix": "r3d100013106"
     },
     "r3d100013107": {
         "description": "PsychArchives is a disciplinary repository for psychological science and neighboring disciplines. Accommodating 20 different digital research object (DRO) types, including articles, preprints, research data, code, supplements, preregistrations, tests and multimedia objects, PsychArchives provides a digital space that integrates all research-related content relevant to psychology. PsychArchives is committed to the FAIR principles, facilitating the findability, accessibility, interoperability and reusability of research and research data.",
         "homepage": "https://www.psycharchives.org/",
         "name": "PsychArchives",
-        "prefix": "r3d100013107"
+        "prefix": "r3d100013107",
+        "xrefs": {
+            "fairsharing.legacy": "4726"
+        }
     },
     "r3d100013108": {
         "description": "The University of Chile Research Data Repository preserves, disseminates and provides access to the research data generated by its academics and researchers, in order to give visibility, guarantee its preservation and facilitate its access and reuse.",
         "homepage": "http://datos.uchile.cl/",
         "name": "Repositorio de Datos de Investigaci\u00f3n de la Universidad de Chile",
         "prefix": "r3d100013108"
     },
@@ -26474,15 +26482,15 @@
         ],
         "xrefs": {
             "fairsharing": "FAIRsharing.566n8c"
         }
     },
     "r3d100013303": {
         "description": "Risklayer Explorer is a collaboration between Risklayer GmbH and the Karlsruhe Institute of Technology's Center for Disaster Risk Management and Risk Reduction Technology (CEDIM). This website is still under development, but we are going live with it already, because we want to present data on the Novel Coronavirus (COVID-19) to help inform the public of the current situation.\nYou will be able to track disaster events and read about our analysis here. Our work is a continuation of a new style of disaster research started by CEDIM in 2011 to analyze disasters immediately after their occurrence, assess the impacts, and retrace the temporal development of disaster events. We are already analyzing damaging earthquakes globally, providing you with event characteristics, earthquake's intensity footprints, as well as the population affected by earthquakes. In addition to earthquake events, we expect to be tracking and analyzing tropical cyclone, volcano and extreme weather events in 2020.",
-        "homepage": "http://risklayer-explorer.com/",
+        "homepage": "https://www.risklayer-explorer.com/",
         "name": "Risklayer Explorer",
         "prefix": "r3d100013303"
     },
     "r3d100013304": {
         "description": "ECDC is an EU agency aimed at strengthening Europe's defences against infectious diseases. The core functions cover a wide spectrum of activities: surveillance, epidemic intelligence, response, scientific advice, microbiology, preparedness, public health training, international relations, health communication, and the scientific journal Eurosurveillance.\nWithin the field of its mission, the Centre shall:  search for, collect, collate, evaluate and disseminate relevant scientific and technical data; provide scientific opinions and scientific and technical assistance including training; provide timely information to the Commission, the Member States, Community agencies and international organisations active within the field of public health; coordinate the European networking of bodies operating in the fields within the Centre's mission, including networks that emerge from public health activities supported by the Commission and operating the dedicated surveillance networks; exchange information, expertise and best practices, and facilitate the development and implementation of joint actions.",
         "homepage": "https://www.ecdc.europa.eu/en",
         "name": "European Centre for Disease Prevention and Control",
@@ -26643,15 +26651,16 @@
     },
     "r3d100013325": {
         "description": "EBRAINS offers one of the most comprehensive platforms for sharing brain research data ranging in type as well as spatial and temporal scale. We provide the guidance and tools needed to overcome the hurdles associated with sharing data. The EBRAINS data curation service ensures that your dataset will be shared with maximum impact, visibility, reusability, and longevity, https://ebrains.eu/services/data-knowledge/share-data. Find data - the user interface of the EBRAINS Knowledge Graph - allows you to easily find data of interest. EBRAINS hosts a wide range of data types and models from different species. All data are well described and can be accessed immediately for further analysis.",
         "homepage": "https://ebrains.eu/",
         "name": "EBRAINS",
         "prefix": "r3d100013325",
         "xrefs": {
-            "fairsharing": "FAIRsharing.XO6ppp"
+            "fairsharing": "FAIRsharing.XO6ppp",
+            "scr": "019260"
         }
     },
     "r3d100013328": {
         "description": "The long term goal of the Software Heritage initiative is to collect all publicly available software in source code form together with its development history, replicate it massively to ensure its preservation, and share it with everyone who needs it. The Software Heritage archive is growing over time as we crawl new source code from software projects and development forges.",
         "homepage": "https://archive.softwareheritage.org/",
         "name": "Software Heritage Archive",
         "prefix": "r3d100013328",
@@ -26868,15 +26877,15 @@
         "name": "BioSimulations",
         "prefix": "r3d100013361",
         "xrefs": {
             "scr": "018733"
         }
     },
     "r3d100013362": {
-        "description": "Mountain Scholar is an open access repository service that collects, preserves, and provides access to digitized library collections and other scholarly and creative works from several academic entities within the states of Colorado and Wyoming.",
+        "description": "Mountain Scholar is an open access repository service that collects, preserves, and provides access to digitized library collections and other scholarly and creative works from several academic entities within the state of Colorado. Colorado State University research data from the fall of 2022 and forward is available in Dryad; CSU legacy research data prior to fall 2022 is in Mountain Scholar.",
         "homepage": "https://mountainscholar.org/",
         "name": "Mountain Scholar",
         "prefix": "r3d100013362",
         "synonyms": [
             "Digital Collections of Colorado"
         ],
         "xrefs": {
@@ -28328,15 +28337,18 @@
     "r3d100013617": {
         "description": "Data catalogue and repository for New Zealand's Biological Heritage National Science Challenge",
         "homepage": "https://data.bioheritage.nz/",
         "name": "New Zealand's Biological Heritage National Science Challenge Data Repository",
         "prefix": "r3d100013617",
         "synonyms": [
             "NZ BioHeritage National Science Challenge Data Repository"
-        ]
+        ],
+        "xrefs": {
+            "scr": "023141"
+        }
     },
     "r3d100013623": {
         "description": "The MHKDR is the repository for all data collected using funds from the Water Power Technologies Office (WPTO) of the U.S. Department of Energy (DOE). It was established to receive, manage, and make available all water power relevant data generated from projects funded by the DOE Water Power Technologies Office. This includes data from WPTO-funded projects associated with any portion of the water power project life-cycle (exploration, development, operation), as well as data produced by WPTO-funded research.",
         "homepage": "https://mhkdr.openei.org/",
         "name": "MHKDR",
         "prefix": "r3d100013623",
         "synonyms": [
```

### Comparing `bioregistry-0.9.3/src/bioregistry/data/external/uniprot/curation.tsv` & `bioregistry-0.9.4/src/bioregistry/data/external/uniprot/curation.tsv`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 DB-0025	euHCVdb	European Hepatitis C Virus Database	https://euhcvdb.lyon.inserm.fr/euHCVdb/do/displayHCVEntry?primaryAC=$1	Organism-specific databases
 DB-0029	Gene3D	Gene3D Structural and Functional Annotation of Protein Families	http://www.cathdb.info/superfamily/$1	Family and domain databases
 DB-0039	Gramene	Gramene; a comparative resource for plants	https://ensembl.gramene.org/id/$1	Genome annotation databases
 DB-0047	UCD-2DPAGE	University College Dublin 2-DE Proteome Database	https://proteomics-portal.ucd.ie/cgi-bin/2d/2d.cgi?$1	2D gel databases
 DB-0050	IMGT_GENE-DB	The international ImMunoGeneTics information system	https://www.imgt.org/IMGT_GENE-DB/GENElect?query=2+$1&species=Homo+sapiens	Protein family/group databases
 DB-0054	LegioList	Legionella pneumophila genome database	http://genolist.pasteur.fr/LegioList/genome.cgi?external_query+$1	Organism-specific databases
 DB-0055	Leproma	Mycobacterium leprae genome database	https://mycobrowser.epfl.ch/genes/$1	Organism-specific databases
-DB-0059	MEROPS	MEROPS protease database	https://www.ebi.ac.uk/merops/cgi-bin/pepsum?mid=$1	Protein family/group databases
+DB-0059	MEROPS	MEROPS protease database	https://www.ebi.ac.uk/merops/cgi-bin/pepsum?id=$1	Protein family/group databases
 DB-0063	ModBase	Database of comparative protein structure models	https://salilab.org/modbase-cgi/model_search.cgi?searchkw=name&kword=$1	3D structure databases
 DB-0067	OGP	USC-OGP 2-DE database	http://usc_ogp_2ddatabase.cesga.es/cgi-bin/2d/2d.cgi?$1	2D gel databases
 DB-0078	PIR	Protein sequence database of the Protein Information Resource	https://proteininformationresource.org/cgi-bin/nbrfget?uid=$1	Sequence databases
 DB-0086	PseudoCAP	Pseudomonas genome database	https://www.pseudomonas.com/feature/show?locus_tag=$1	Organism-specific databases
 DB-0090	REPRODUCTION-2DPAGE	REPRODUCTION-2DPAGE	http://reprod.njmu.edu.cn/cgi-bin/2d/2d.cgi?$1	2D gel databases
 DB-0098	SMR	SWISS-MODEL Repository - a database of annotated 3D protein structure models	https://swissmodel.expasy.org/repository/uniprot/$1?csm=%d	3D structure databases
 DB-0099	SOURCE	The Stanford Online Universal Resource for Clones and ESTs	https://puma.princeton.edu/cgi-bin/source/sourceResult?criteria=$1&choice=Gene&option=Symbol&organism=%d	Miscellaneous databases
@@ -57,15 +57,15 @@
 DB-0225	CarbonylDB	CarbonylDB database of protein carbonylation sites	http://digbio.missouri.edu/CarbonylDB/index.php/detail/protein/$1	PTM databases
 DB-0227	GlyConnect	GlyConnect protein glycosylation platform	https://glyconnect.expasy.org/browser/proteins/$1	PTM databases
 DB-0229	ProteomicsDB	ProteomicsDB	https://www.proteomicsdb.org/proteomicsdb/#protein/proteinDetails/$1	Proteomic databases
 DB-0230	MoonDB	MoonDB Database of extreme multifunctional and moonlighting proteins	http://moondb.hb.univ-amu.fr/protein/$1	Protein family/group databases
 DB-0231	UniLectin	UniLectin database of carbohydrate-binding proteins	https://www.unilectin.eu/curated/protein/$1	Protein family/group databases
 DB-0233	jPOST	jPOST - Japan Proteome Standard Repository/Database	https://globe.jpostdb.org/protein?id=$1	Proteomic databases
 DB-0234	SWISS-MODEL-Workspace	SWISS-MODEL Interactive Workspace	https://swissmodel.expasy.org/interactive/?ac=$1	3D structure databases
-DB-0237	NIAGADS	NIAGADS Genomics Database	https://www.niagads.org/genomics/showRecord.do?name=GeneRecordClasses.GeneRecordClass&source_id=$1	Organism-specific databases
+DB-0237	NIAGADS	NIAGADS Genomics Database	https://www.niagads.org/genomics/app/record/gene/$1	Organism-specific databases
 DB-0238	CPTAC	The CPTAC Assay portal	https://assays.cancer.gov/$1	Proteomic databases
 DB-0240	Pharos	Pharos NIH Druggable Genome Knowledgebase	https://pharos.nih.gov/targets/$1	Miscellaneous databases
 DB-0244	PDBe-KB	Protein Data Bank in Europe - Knowledge Base	https://pdbe-kb.org/proteins/$1	3D structure databases
 DB-0246	RNAct	RNAct, Protein-RNA interaction predictions for model organisms.	https://rnact.crg.eu/%d?query=$1	Miscellaneous databases
 DB-0247	MetOSite	MetOSite database of methionine sulfoxide sites	https://metosite.uma.es/scan/$1	PTM databases
 DB-0248	PHI-base	Pathogen-Host Interaction database	http://www.phi-base.org/searchFacet.htm?queryTerm=$1	Miscellaneous databases
 DB-0249	Antibodypedia	Antibodypedia a portal for validated antibodies	https://antibodypedia.com/gene/$1	Protocols and materials databases
```

### Comparing `bioregistry-0.9.3/src/bioregistry/data/external/uniprot/processed.json` & `bioregistry-0.9.4/src/bioregistry/data/external/uniprot/processed.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9981494413407822%*

 * *Differences: {"'DB-0052'": "{'publications': {0: {'doi': '10.1093/nar/gkac993', 'pubmed': '36350672'}}}",*

 * * "'DB-0059'": "{'uri_format': 'https://www.ebi.ac.uk/merops/cgi-bin/pepsum?id=$1'}",*

 * * "'DB-0073'": "{'homepage': 'http://pfam-legacy.xfam.org/', 'publications': {0: {'doi': "*

 * *              "'10.1093/nar/gkaa913', 'pubmed': '33125078'}}, 'uri_format': "*

 * *              "'https://www.ebi.ac.uk/interpro/entry/pfam/$1'}",*

 * * "'DB-0174'": "{'homepage': 'https://www.ebi.ac.uk/chembl', 'publications': {0: {'doi': "*

 * *            […]*

```diff
@@ -406,16 +406,16 @@
     "DB-0052": {
         "abbreviation": "InterPro",
         "category": "Family and domain databases",
         "homepage": "https://www.ebi.ac.uk/interpro/",
         "name": "Integrated resource of protein families, domains and functional sites",
         "publications": [
             {
-                "doi": "10.1093/nar/gkaa977",
-                "pubmed": "33156333"
+                "doi": "10.1093/nar/gkac993",
+                "pubmed": "36350672"
             }
         ],
         "uri_format": "https://www.ebi.ac.uk/interpro/entry/$1"
     },
     "DB-0053": {
         "abbreviation": "KEGG",
         "category": "Genome annotation databases",
@@ -469,15 +469,15 @@
         "name": "MEROPS protease database",
         "publications": [
             {
                 "doi": "10.1093/nar/gkx1134",
                 "pubmed": "29145643"
             }
         ],
-        "uri_format": "https://www.ebi.ac.uk/merops/cgi-bin/pepsum?mid=$1"
+        "uri_format": "https://www.ebi.ac.uk/merops/cgi-bin/pepsum?id=$1"
     },
     "DB-0060": {
         "abbreviation": "MGI",
         "category": "Organism-specific databases",
         "homepage": "http://www.informatics.jax.org/",
         "name": "Mouse genome database (MGD) from Mouse Genome Informatics (MGI)",
         "publications": [
@@ -579,23 +579,23 @@
             }
         ],
         "uri_format": "http://peroxibase.toulouse.inra.fr/display_perox/view_perox/$1"
     },
     "DB-0073": {
         "abbreviation": "Pfam",
         "category": "Family and domain databases",
-        "homepage": "https://pfam.xfam.org/",
+        "homepage": "http://pfam-legacy.xfam.org/",
         "name": "Pfam protein domain database",
         "publications": [
             {
-                "doi": "10.1093/nar/gky995",
-                "pubmed": "30357350"
+                "doi": "10.1093/nar/gkaa913",
+                "pubmed": "33125078"
             }
         ],
-        "uri_format": "https://pfam.xfam.org/family/$1"
+        "uri_format": "https://www.ebi.ac.uk/interpro/entry/pfam/$1"
     },
     "DB-0074": {
         "abbreviation": "PharmGKB",
         "category": "Organism-specific databases",
         "homepage": "https://www.pharmgkb.org/",
         "name": "The Pharmacogenetics and Pharmacogenomics Knowledge Base",
         "publications": [
@@ -1365,23 +1365,23 @@
             }
         ],
         "uri_format": "https://pax-db.org/#!protein/$1"
     },
     "DB-0174": {
         "abbreviation": "ChEMBL",
         "category": "Chemistry databases",
-        "homepage": "https://www.ebi.ac.uk/chembldb",
+        "homepage": "https://www.ebi.ac.uk/chembl",
         "name": "ChEMBL database of bioactive drug-like small molecules",
         "publications": [
             {
-                "doi": "10.1093/nar/gkr777",
-                "pubmed": "21948594"
+                "doi": "10.1093/nar/gky1075",
+                "pubmed": "30398643"
             }
         ],
-        "uri_format": "https://www.ebi.ac.uk/chembldb/target/inspect/$1"
+        "uri_format": "https://www.ebi.ac.uk/chembl/target/inspect/$1"
     },
     "DB-0175": {
         "abbreviation": "CLAE",
         "category": "Protein family/group databases",
         "homepage": "https://clae.fungalgenomics.ca/",
         "name": "CLAE, a database of fungal genes encoding lignocellulose-active proteins",
         "publications": [
@@ -1953,15 +1953,15 @@
         "uri_format": "https://web.expasy.org/cgi-bin/abcd/search_abcd.pl?input=$1"
     },
     "DB-0237": {
         "abbreviation": "NIAGADS",
         "category": "Organism-specific databases",
         "homepage": "https://www.niagads.org/genomics/",
         "name": "NIAGADS Genomics Database",
-        "uri_format": "https://www.niagads.org/genomics/showRecord.do?name=GeneRecordClasses.GeneRecordClass&source_id=$1"
+        "uri_format": "https://www.niagads.org/genomics/app/record/gene/$1"
     },
     "DB-0238": {
         "abbreviation": "CPTAC",
         "category": "Proteomic databases",
         "homepage": "https://assays.cancer.gov/",
         "name": "The CPTAC Assay portal",
         "publications": [
@@ -2243,13 +2243,13 @@
         "abbreviation": "GlyCosmos",
         "category": "PTM databases",
         "homepage": "https://glycosmos.org/",
         "name": "GlyCosmos Portal integrating glycosciences with life sciences",
         "publications": [
             {
                 "doi": "10.1038/s41592-020-0879-8",
-                "pubmed": "2572234"
+                "pubmed": "32572234"
             }
         ],
         "uri_format": "https://glycosmos.org/glycoproteins/show/uniprot/$1"
     }
 }
```

### Comparing `bioregistry-0.9.3/src/bioregistry/data/external/uniprot/raw.json` & `bioregistry-0.9.4/src/bioregistry/data/external/uniprot/raw.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9901928592995162%*

 * *Differences: {"'results'": "{0: {'statistics': {'reviewedProteinCount': 52786, 'unreviewedProteinCount': "*

 * *              "608930}}, 1: {'statistics': {'reviewedProteinCount': 54743, "*

 * *              "'unreviewedProteinCount': 533104}}, 6: {'statistics': {'reviewedProteinCount': "*

 * *              "17490, 'unreviewedProteinCount': 3015}}, 7: {'statistics': {'reviewedProteinCount': "*

 * *              "1728, 'unreviewedProteinCount': 200}}, 9: {'statistics': {'reviewedProteinCount': "*

 * *              "4770}}, 11: {'statistics': {'r […]*

```diff
@@ -7,31 +7,31 @@
             "doiId": "10.1093/nar/gkz947",
             "id": "DB-0004",
             "linkType": "Explicit",
             "name": "ExpressionAtlas, Differential and Baseline Expression",
             "pubMedId": "31665515",
             "server": "https://www.ebi.ac.uk/gxa",
             "statistics": {
-                "reviewedProteinCount": 52753,
-                "unreviewedProteinCount": 609382
+                "reviewedProteinCount": 52786,
+                "unreviewedProteinCount": 608930
             }
         },
         {
             "abbrev": "BioCyc",
             "category": "Enzyme and pathway databases",
             "dbUrl": "https://biocyc.org/getid?id=%s",
             "doiId": "10.1093/nar/gkv1164",
             "id": "DB-0005",
             "linkType": "Explicit",
             "name": "BioCyc Collection of Pathway/Genome Databases",
             "pubMedId": "26527732",
             "server": "https://www.biocyc.org/",
             "statistics": {
-                "reviewedProteinCount": 54700,
-                "unreviewedProteinCount": 541981
+                "reviewedProteinCount": 54743,
+                "unreviewedProteinCount": 533104
             }
         },
         {
             "abbrev": "COMPLUYEAST-2DPAGE",
             "category": "2D gel databases",
             "dbUrl": "http://compluyeast2dpage.dacya.ucm.es/cgi-bin/2d/2d.cgi?ac=%s",
             "doiId": "10.1016/S1570-0232(02)00762-6",
@@ -97,31 +97,31 @@
             "doiId": "10.1093/nar/gkh086",
             "id": "DB-0016",
             "linkType": "Explicit",
             "name": "Database of interacting proteins",
             "pubMedId": "14681454",
             "server": "https://dip.doe-mbi.ucla.edu/",
             "statistics": {
-                "reviewedProteinCount": 17487,
-                "unreviewedProteinCount": 3018
+                "reviewedProteinCount": 17490,
+                "unreviewedProteinCount": 3015
             }
         },
         {
             "abbrev": "DisProt",
             "category": "Family and domain databases",
             "dbUrl": "https://disprot.org/%s",
             "doiId": "10.1093/bioinformatics/bth476",
             "id": "DB-0017",
             "linkType": "Explicit",
             "name": "Database of protein disorder",
             "pubMedId": "15310560",
             "server": "https://disprot.org",
             "statistics": {
-                "reviewedProteinCount": 1742,
-                "unreviewedProteinCount": 201
+                "reviewedProteinCount": 1728,
+                "unreviewedProteinCount": 200
             }
         },
         {
             "abbrev": "DOSAC-COBS-2DPAGE",
             "category": "2D gel databases",
             "dbUrl": "http://www.dosac.unipa.it/cgi-bin/2d/2d.cgi?ac=%u",
             "id": "DB-0018",
@@ -140,15 +140,15 @@
             "doiId": "10.1093/nar/gkj067",
             "id": "DB-0019",
             "linkType": "Explicit",
             "name": "Drug and drug target database",
             "pubMedId": "16381955",
             "server": "https://www.drugbank.ca/",
             "statistics": {
-                "reviewedProteinCount": 4742,
+                "reviewedProteinCount": 4770,
                 "unreviewedProteinCount": 450
             }
         },
         {
             "abbrev": "EchoBASE",
             "category": "Organism-specific databases",
             "dbUrl": "https://www.york.ac.uk/res/thomas/Gene.cfm?recordID=%s",
@@ -170,31 +170,31 @@
             "doiId": "10.1093/nar/gkaa1028",
             "id": "DB-0022",
             "linkType": "Explicit",
             "name": "EMBL nucleotide sequence database",
             "pubMedId": "33175160",
             "server": "https://www.ebi.ac.uk/ena",
             "statistics": {
-                "reviewedProteinCount": 556568,
-                "unreviewedProteinCount": 230974938
+                "reviewedProteinCount": 556846,
+                "unreviewedProteinCount": 234394364
             }
         },
         {
             "abbrev": "Ensembl",
             "category": "Genome annotation databases",
             "dbUrl": "https://www.ensembl.org/id/%s",
             "doiId": "10.1093/nar/gkz966",
             "id": "DB-0023",
             "linkType": "Explicit",
             "name": "Ensembl eukaryotic genome annotation project",
             "pubMedId": "31691826",
             "server": "https://www.ensembl.org/",
             "statistics": {
-                "reviewedProteinCount": 48400,
-                "unreviewedProteinCount": 8870782
+                "reviewedProteinCount": 48420,
+                "unreviewedProteinCount": 8838708
             }
         },
         {
             "abbrev": "ENZYME",
             "category": "Enzyme and pathway databases",
             "dbUrl": "https://enzyme.expasy.org/EC/%s",
             "doiId": "10.1093/nar/28.1.304",
@@ -230,16 +230,16 @@
             "doiId": "10.1093/nar/gky1003",
             "id": "DB-0026",
             "linkType": "Explicit",
             "name": "Drosophila genome database",
             "pubMedId": "30364959",
             "server": "https://flybase.org/",
             "statistics": {
-                "reviewedProteinCount": 3996,
-                "unreviewedProteinCount": 28336
+                "reviewedProteinCount": 3999,
+                "unreviewedProteinCount": 28330
             }
         },
         {
             "abbrev": "GenAtlas",
             "category": "Organism-specific databases",
             "dbUrl": "http://genatlas.medecine.univ-paris5.fr/fiche.php?symbol=%s",
             "doiId": "10.1016/S0764-4469(99)80021-3",
@@ -275,31 +275,31 @@
             "doiId": "10.1093/nar/gkx1069",
             "id": "DB-0029",
             "linkType": "Explicit",
             "name": "Gene3D Structural and Functional Annotation of Protein Families",
             "pubMedId": "29112716",
             "server": "http://gene3d.biochem.ucl.ac.uk/Gene3D/",
             "statistics": {
-                "reviewedProteinCount": 457643,
-                "unreviewedProteinCount": 149120447
+                "reviewedProteinCount": 457864,
+                "unreviewedProteinCount": 160203228
             }
         },
         {
             "abbrev": "GeneCards",
             "category": "Organism-specific databases",
             "dbUrl": "https://www.genecards.org/cgi-bin/carddisp.pl?gene=%s",
             "doiId": "10.1093/bioinformatics/18.11.1542",
             "id": "DB-0030",
             "linkType": "Explicit",
             "name": "GeneCards",
             "pubMedId": "12424129",
             "server": "https://www.genecards.org/",
             "statistics": {
-                "reviewedProteinCount": 20202,
-                "unreviewedProteinCount": 1279
+                "reviewedProteinCount": 20230,
+                "unreviewedProteinCount": 1310
             }
         },
         {
             "abbrev": "PomBase",
             "category": "Organism-specific databases",
             "dbUrl": "https://www.pombase.org/gene/%s",
             "doiId": "10.1093/nar/gky961",
@@ -320,16 +320,16 @@
             "doiId": "10.1093/nar/gky1055",
             "id": "DB-0037",
             "linkType": "Explicit",
             "name": "Gene Ontology",
             "pubMedId": "30395331",
             "server": "http://geneontology.org/",
             "statistics": {
-                "reviewedProteinCount": 545442,
-                "unreviewedProteinCount": 157853630
+                "reviewedProteinCount": 545707,
+                "unreviewedProteinCount": 160826991
             }
         },
         {
             "abbrev": "GPCRDB",
             "category": "Protein family/group databases",
             "dbUrl": "https://gpcrdb.org/protein/%u/",
             "doiId": "10.1093/nar/29.1.346",
@@ -350,61 +350,61 @@
             "doiId": "10.1093/nar/gkx1111",
             "id": "DB-0039",
             "linkType": "Explicit",
             "name": "Gramene; a comparative resource for plants",
             "pubMedId": "29165610",
             "server": "https://www.gramene.org/",
             "statistics": {
-                "reviewedProteinCount": 21987,
-                "unreviewedProteinCount": 3131296
+                "reviewedProteinCount": 22054,
+                "unreviewedProteinCount": 3130240
             }
         },
         {
             "abbrev": "HAMAP",
             "category": "Family and domain databases",
             "dbUrl": "https://hamap.expasy.org/signature/%s",
             "doiId": "10.1093/nar/gku1002",
             "id": "DB-0041",
             "linkType": "Explicit",
             "name": "HAMAP database of protein families",
             "pubMedId": "25348399",
             "server": "https://hamap.expasy.org/",
             "statistics": {
-                "reviewedProteinCount": 327896,
-                "unreviewedProteinCount": 23901893
+                "reviewedProteinCount": 327913,
+                "unreviewedProteinCount": 25751139
             }
         },
         {
             "abbrev": "HGNC",
             "category": "Organism-specific databases",
             "dbUrl": "https://www.genenames.org/data/gene-symbol-report/#!/hgnc_id/%s",
             "doiId": "10.1093/nar/gkaa980",
             "id": "DB-0042",
             "linkType": "Explicit",
             "name": "Human Gene Nomenclature Database",
             "pubMedId": "33152070",
             "server": "https://www.genenames.org/",
             "statistics": {
                 "reviewedProteinCount": 20235,
-                "unreviewedProteinCount": 60587
+                "unreviewedProteinCount": 61269
             }
         },
         {
             "abbrev": "HOGENOM",
             "category": "Phylogenomic databases",
             "dbUrl": "http://hogenom.univ-lyon1.fr/query_sequence?seq=%u",
             "doiId": "10.1101/gr.10.3.379",
             "id": "DB-0044",
             "linkType": "Explicit",
             "name": "The HOGENOM Database of Homologous Genes from Fully Sequenced Organisms",
             "pubMedId": "10720578",
             "server": "http://hogenom.univ-lyon1.fr/",
             "statistics": {
-                "reviewedProteinCount": 426187,
-                "unreviewedProteinCount": 16226698
+                "reviewedProteinCount": 426368,
+                "unreviewedProteinCount": 16188438
             }
         },
         {
             "abbrev": "HPA",
             "category": "Organism-specific databases",
             "dbUrl": "https://www.proteinatlas.org/%s",
             "doiId": "10.1126/science.1260419",
@@ -468,46 +468,46 @@
             "doiId": "10.1093/nar/gkt1115",
             "id": "DB-0051",
             "linkType": "Explicit",
             "name": "Protein interaction database and analysis system",
             "pubMedId": "24234451",
             "server": "https://www.ebi.ac.uk/intact/",
             "statistics": {
-                "reviewedProteinCount": 56773,
-                "unreviewedProteinCount": 24860
+                "reviewedProteinCount": 56792,
+                "unreviewedProteinCount": 23572
             }
         },
         {
             "abbrev": "InterPro",
             "category": "Family and domain databases",
             "dbUrl": "https://www.ebi.ac.uk/interpro/entry/%s",
-            "doiId": "10.1093/nar/gkaa977",
+            "doiId": "10.1093/nar/gkac993",
             "id": "DB-0052",
             "linkType": "Explicit",
             "name": "Integrated resource of protein families, domains and functional sites",
-            "pubMedId": "33156333",
+            "pubMedId": "36350672",
             "server": "https://www.ebi.ac.uk/interpro/",
             "statistics": {
-                "reviewedProteinCount": 550043,
-                "unreviewedProteinCount": 185803220
+                "reviewedProteinCount": 550318,
+                "unreviewedProteinCount": 199254721
             }
         },
         {
             "abbrev": "KEGG",
             "category": "Genome annotation databases",
             "dbUrl": "https://www.genome.jp/dbget-bin/www_bget?%s",
             "doiId": "10.1093/nar/gkw1092",
             "id": "DB-0053",
             "linkType": "Explicit",
             "name": "KEGG",
             "pubMedId": "27899662",
             "server": "https://www.genome.jp/kegg/",
             "statistics": {
-                "reviewedProteinCount": 478544,
-                "unreviewedProteinCount": 22639552
+                "reviewedProteinCount": 478903,
+                "unreviewedProteinCount": 22867949
             }
         },
         {
             "abbrev": "LegioList",
             "category": "Organism-specific databases",
             "dbUrl": "http://genolist.pasteur.fr/LegioList/genome.cgi?external_query+%s",
             "doiId": "10.1186/1471-2164-6-14",
@@ -548,53 +548,53 @@
                 "reviewedProteinCount": 524,
                 "unreviewedProteinCount": 0
             }
         },
         {
             "abbrev": "MEROPS",
             "category": "Protein family/group databases",
-            "dbUrl": "https://www.ebi.ac.uk/merops/cgi-bin/pepsum?mid=%s",
+            "dbUrl": "https://www.ebi.ac.uk/merops/cgi-bin/pepsum?id=%s",
             "doiId": "10.1093/nar/gkx1134",
             "id": "DB-0059",
             "linkType": "Explicit",
             "name": "MEROPS protease database",
             "pubMedId": "29145643",
             "server": "https://www.ebi.ac.uk/merops/",
             "statistics": {
-                "reviewedProteinCount": 13757,
-                "unreviewedProteinCount": 295023
+                "reviewedProteinCount": 13769,
+                "unreviewedProteinCount": 294419
             }
         },
         {
             "abbrev": "MGI",
             "category": "Organism-specific databases",
             "dbUrl": "http://www.informatics.jax.org/marker/%s",
             "doiId": "10.1093/nar/gky1056",
             "id": "DB-0060",
             "linkType": "Explicit",
             "name": "Mouse genome database (MGD) from Mouse Genome Informatics (MGI)",
             "pubMedId": "30407599",
             "server": "http://www.informatics.jax.org/",
             "statistics": {
-                "reviewedProteinCount": 17011,
-                "unreviewedProteinCount": 63147
+                "reviewedProteinCount": 17025,
+                "unreviewedProteinCount": 63129
             }
         },
         {
             "abbrev": "MIM",
             "category": "Organism-specific databases",
             "dbUrl": "https://www.omim.org/entry/%s",
             "doiId": "10.1093/nar/gku1205",
             "id": "DB-0062",
             "linkType": "Explicit",
             "name": "Online Mendelian Inheritance in Man (OMIM)",
             "pubMedId": "25428349",
             "server": "https://www.omim.org/",
             "statistics": {
-                "reviewedProteinCount": 15905,
+                "reviewedProteinCount": 15948,
                 "unreviewedProteinCount": 0
             }
         },
         {
             "abbrev": "ModBase",
             "category": "3D structure databases",
             "dbUrl": "https://salilab.org/modbase-cgi/model_search.cgi?searchkw=name&kword=%u",
@@ -627,209 +627,209 @@
             "category": "Organism-specific databases",
             "dbUrl": "https://www.orpha.net/consor/cgi-bin/OC_Exp.php?Lng=GB&Expert=%s",
             "id": "DB-0068",
             "linkType": "Explicit",
             "name": "Orphanet; a database dedicated to information on rare diseases and orphan drugs",
             "server": "https://www.orpha.net/consor/cgi-bin/index.php",
             "statistics": {
-                "reviewedProteinCount": 4348,
+                "reviewedProteinCount": 4352,
                 "unreviewedProteinCount": 0
             }
         },
         {
             "abbrev": "PANTHER",
             "category": "Family and domain databases",
             "dbUrl": "http://www.pantherdb.org/panther/family.do?clsAccession=%s",
             "doiId": "10.1093/nar/gky1038",
             "id": "DB-0069",
             "linkType": "Explicit",
             "name": "The PANTHER Classification System",
             "pubMedId": "30407594",
             "server": "http://www.pantherdb.org/",
             "statistics": {
-                "reviewedProteinCount": 500948,
-                "unreviewedProteinCount": 155394625
+                "reviewedProteinCount": 501169,
+                "unreviewedProteinCount": 166090930
             }
         },
         {
             "abbrev": "PDB",
             "category": "3D structure databases",
             "dbUrl": "https://www.ebi.ac.uk/pdbe-srv/view/entry/%s",
             "doiId": "10.1093/nar/gkz990",
             "id": "DB-0070",
             "linkType": "Explicit",
             "name": "Protein Data Bank Europe",
             "pubMedId": "31691821",
             "server": "https://www.ebi.ac.uk/pdbe/",
             "statistics": {
-                "reviewedProteinCount": 33056,
-                "unreviewedProteinCount": 27044
+                "reviewedProteinCount": 33106,
+                "unreviewedProteinCount": 27523
             }
         },
         {
             "abbrev": "PeptideAtlas",
             "category": "Proteomic databases",
             "dbUrl": "https://db.systemsbiology.net/sbeams/cgi/PeptideAtlas/Search?action=GO&search_key=%s",
             "doiId": "10.1093/nar/gkj040",
             "id": "DB-0071",
             "linkType": "Explicit",
             "name": "PeptideAtlas",
             "pubMedId": "16381952",
             "server": "http://www.peptideatlas.org",
             "statistics": {
-                "reviewedProteinCount": 39579,
-                "unreviewedProteinCount": 162374
+                "reviewedProteinCount": 39432,
+                "unreviewedProteinCount": 162875
             }
         },
         {
             "abbrev": "PeroxiBase",
             "category": "Protein family/group databases",
             "dbUrl": "http://peroxibase.toulouse.inra.fr/display_perox/view_perox/%s",
             "doiId": "10.1093/nar/gks1083",
             "id": "DB-0072",
             "linkType": "Explicit",
             "name": "PeroxiBase, a peroxidase database",
             "pubMedId": "23180785",
             "server": "http://peroxibase.toulouse.inra.fr/",
             "statistics": {
-                "reviewedProteinCount": 769,
+                "reviewedProteinCount": 770,
                 "unreviewedProteinCount": 2524
             }
         },
         {
             "abbrev": "Pfam",
             "category": "Family and domain databases",
-            "dbUrl": "https://pfam.xfam.org/family/%s",
-            "doiId": "10.1093/nar/gky995",
+            "dbUrl": "https://www.ebi.ac.uk/interpro/entry/pfam/%s",
+            "doiId": "10.1093/nar/gkaa913",
             "id": "DB-0073",
             "linkType": "Explicit",
             "name": "Pfam protein domain database",
-            "pubMedId": "30357350",
-            "server": "https://pfam.xfam.org/",
+            "pubMedId": "33125078",
+            "server": "http://pfam-legacy.xfam.org/",
             "statistics": {
-                "reviewedProteinCount": 538122,
-                "unreviewedProteinCount": 175288986
+                "reviewedProteinCount": 538372,
+                "unreviewedProteinCount": 187886283
             }
         },
         {
             "abbrev": "PharmGKB",
             "category": "Organism-specific databases",
             "dbUrl": "https://www.pharmgkb.org/gene/%s",
             "doiId": "10.1385/1-59259-957-5:179",
             "id": "DB-0074",
             "linkType": "Explicit",
             "name": "The Pharmacogenetics and Pharmacogenomics Knowledge Base",
             "pubMedId": "16100408",
             "server": "https://www.pharmgkb.org/",
             "statistics": {
-                "reviewedProteinCount": 18015,
+                "reviewedProteinCount": 18014,
                 "unreviewedProteinCount": 3076
             }
         },
         {
             "abbrev": "PIR",
             "category": "Sequence databases",
             "dbUrl": "https://proteininformationresource.org/cgi-bin/nbrfget?uid=%s",
             "id": "DB-0078",
             "linkType": "Explicit",
             "name": "Protein sequence database of the Protein Information Resource",
             "server": "https://proteininformationresource.org/",
             "statistics": {
-                "reviewedProteinCount": 114600,
-                "unreviewedProteinCount": 129208
+                "reviewedProteinCount": 114649,
+                "unreviewedProteinCount": 129080
             }
         },
         {
             "abbrev": "PIRSF",
             "category": "Family and domain databases",
             "dbUrl": "https://proteininformationresource.org/cgi-bin/ipcSF?id=%s",
             "doiId": "10.1093/nar/gkh097",
             "id": "DB-0079",
             "linkType": "Explicit",
             "name": "PIRSF; a whole-protein classification database",
             "pubMedId": "14681371",
             "server": "https://proteininformationresource.org/pirwww/dbinfo/pirsf.shtml",
             "statistics": {
-                "reviewedProteinCount": 109612,
-                "unreviewedProteinCount": 19525876
+                "reviewedProteinCount": 109629,
+                "unreviewedProteinCount": 20914236
             }
         },
         {
             "abbrev": "PRINTS",
             "category": "Family and domain databases",
             "dbUrl": "http://umber.sbs.man.ac.uk/cgi-bin/dbbrowser/sprint/searchprintss.cgi?display_opts=Prints&category=None&queryform=false&prints_accn=%s",
             "doiId": "10.1093/database/bas019",
             "id": "DB-0082",
             "linkType": "Explicit",
             "name": "Protein Motif fingerprint database; a protein domain database",
             "pubMedId": "22508994",
             "server": "http://www.bioinf.manchester.ac.uk/dbbrowser/PRINTS/",
             "statistics": {
-                "reviewedProteinCount": 129197,
-                "unreviewedProteinCount": 31517347
+                "reviewedProteinCount": 129260,
+                "unreviewedProteinCount": 33400061
             }
         },
         {
             "abbrev": "PROSITE",
             "category": "Family and domain databases",
             "dbUrl": "https://prosite.expasy.org/doc/%s",
             "doiId": "10.1093/nar/gks1067",
             "id": "DB-0084",
             "linkType": "Explicit",
             "name": "PROSITE; a protein domain and family database",
             "pubMedId": "23161676",
             "server": "https://prosite.expasy.org/",
             "statistics": {
-                "reviewedProteinCount": 309536,
-                "unreviewedProteinCount": 86246574
+                "reviewedProteinCount": 310067,
+                "unreviewedProteinCount": 91823656
             }
         },
         {
             "abbrev": "PseudoCAP",
             "category": "Organism-specific databases",
             "dbUrl": "https://www.pseudomonas.com/feature/show?locus_tag=%s",
             "doiId": "10.1093/nar/gki047",
             "id": "DB-0086",
             "linkType": "Explicit",
             "name": "Pseudomonas genome database",
             "pubMedId": "15608211",
             "server": "https://www.pseudomonas.com/",
             "statistics": {
-                "reviewedProteinCount": 1439,
-                "unreviewedProteinCount": 4327
+                "reviewedProteinCount": 1440,
+                "unreviewedProteinCount": 4326
             }
         },
         {
             "abbrev": "Reactome",
             "category": "Enzyme and pathway databases",
             "dbUrl": "https://www.reactome.org/PathwayBrowser/#%s&FLG=%u",
             "doiId": "10.1093/nar/gkz1031",
             "id": "DB-0088",
             "linkType": "Explicit",
             "name": "Reactome - a knowledgebase of biological pathways and processes",
             "pubMedId": "31691815",
             "server": "https://reactome.org",
             "statistics": {
-                "reviewedProteinCount": 37755,
-                "unreviewedProteinCount": 37865
+                "reviewedProteinCount": 37889,
+                "unreviewedProteinCount": 37857
             }
         },
         {
             "abbrev": "REBASE",
             "category": "Protein family/group databases",
             "dbUrl": "http://rebase.neb.com/rebase/enz/%s.html",
             "doiId": "10.1093/nar/gku1046",
             "id": "DB-0089",
             "linkType": "Explicit",
             "name": "Restriction enzymes and methylases database",
             "pubMedId": "25378308",
             "server": "http://rebase.neb.com/rebase/rebase.html",
             "statistics": {
-                "reviewedProteinCount": 399,
-                "unreviewedProteinCount": 102437
+                "reviewedProteinCount": 396,
+                "unreviewedProteinCount": 98911
             }
         },
         {
             "abbrev": "REPRODUCTION-2DPAGE",
             "category": "2D gel databases",
             "dbUrl": "http://reprod.njmu.edu.cn/cgi-bin/2d/2d.cgi?%s",
             "id": "DB-0090",
@@ -848,16 +848,16 @@
             "doiId": "10.1093/nar/gkz1041",
             "id": "DB-0091",
             "linkType": "Explicit",
             "name": "Rat Genome Database",
             "pubMedId": "31713623",
             "server": "https://rgd.mcw.edu/",
             "statistics": {
-                "reviewedProteinCount": 8103,
-                "unreviewedProteinCount": 43529
+                "reviewedProteinCount": 8107,
+                "unreviewedProteinCount": 43542
             }
         },
         {
             "abbrev": "Rouge",
             "category": "Organism-specific databases",
             "dbUrl": "http://www.kazusa.or.jp/rouge/gfpage/%s",
             "doiId": "10.1093/nar/gkh035",
@@ -893,31 +893,31 @@
             "doiId": "10.1093/nar/gkx922",
             "id": "DB-0097",
             "linkType": "Explicit",
             "name": "Simple Modular Architecture Research Tool; a protein domain database",
             "pubMedId": "29040681",
             "server": "http://smart.embl.de/",
             "statistics": {
-                "reviewedProteinCount": 147794,
-                "unreviewedProteinCount": 46804790
+                "reviewedProteinCount": 147892,
+                "unreviewedProteinCount": 49645958
             }
         },
         {
             "abbrev": "SMR",
             "category": "3D structure databases",
             "dbUrl": "https://swissmodel.expasy.org/repository/uniprot/%s?csm=%d",
             "doiId": "10.1093/nar/gkw1132",
             "id": "DB-0098",
             "linkType": "Explicit",
             "name": "SWISS-MODEL Repository - a database of annotated 3D protein structure models",
             "pubMedId": "27899672",
             "server": "https://swissmodel.expasy.org/repository/",
             "statistics": {
-                "reviewedProteinCount": 508433,
-                "unreviewedProteinCount": 2784302
+                "reviewedProteinCount": 509063,
+                "unreviewedProteinCount": 2840327
             }
         },
         {
             "abbrev": "SOURCE",
             "category": "Miscellaneous databases",
             "dbUrl": "https://puma.princeton.edu/cgi-bin/source/sourceResult?criteria=%s&choice=Gene&option=Symbol&organism=%d",
             "id": "DB-0099",
@@ -951,121 +951,121 @@
             "doiId": "10.1093/nar/gkr1090",
             "id": "DB-0102",
             "linkType": "Explicit",
             "name": "The Arabidopsis Information Resource",
             "pubMedId": "22140109",
             "server": "https://www.arabidopsis.org/",
             "statistics": {
-                "reviewedProteinCount": 15025,
-                "unreviewedProteinCount": 11351
+                "reviewedProteinCount": 15741,
+                "unreviewedProteinCount": 23011
             }
         },
         {
             "abbrev": "TIGRFAMs",
             "category": "Family and domain databases",
             "dbUrl": "https://www.ncbi.nlm.nih.gov/genome/annotation_prok/evidence/%s/",
             "doiId": "10.1093/nar/gks1234",
             "id": "DB-0104",
             "linkType": "Explicit",
             "name": "TIGRFAMs; a protein family database",
             "pubMedId": "23197656",
             "server": "https://www.ncbi.nlm.nih.gov/genome/annotation_prok/tigrfams/",
             "statistics": {
-                "reviewedProteinCount": 274529,
-                "unreviewedProteinCount": 42363484
+                "reviewedProteinCount": 274562,
+                "unreviewedProteinCount": 41931305
             }
         },
         {
             "abbrev": "TubercuList",
             "category": "Organism-specific databases",
             "dbUrl": "https://mycobrowser.epfl.ch/genes/%s",
             "doiId": "10.1016/j.tube.2010.09.006",
             "id": "DB-0106",
             "linkType": "Explicit",
             "name": "Mycobacterium tuberculosis strain H37Rv genome database",
             "pubMedId": "20980200",
             "server": "https://mycobrowser.epfl.ch/",
             "statistics": {
-                "reviewedProteinCount": 2274,
+                "reviewedProteinCount": 2275,
                 "unreviewedProteinCount": 929
             }
         },
         {
             "abbrev": "WormBase",
             "category": "Organism-specific databases",
             "dbUrl": "https://wormbase.org/db/seq/protein?name=%s;class=CDS",
             "doiId": "10.1093/nar/gkz920",
             "id": "DB-0110",
             "linkType": "Explicit",
             "name": "WormBase",
             "pubMedId": "31642470",
             "server": "https://www.wormbase.org/",
             "statistics": {
-                "reviewedProteinCount": 5033,
-                "unreviewedProteinCount": 61386
+                "reviewedProteinCount": 5046,
+                "unreviewedProteinCount": 61365
             }
         },
         {
             "abbrev": "ZFIN",
             "category": "Organism-specific databases",
             "dbUrl": "https://zfin.org/%s",
             "doiId": "10.1093/nar/gky1090",
             "id": "DB-0113",
             "linkType": "Explicit",
             "name": "Zebrafish Information Network genome database",
             "pubMedId": "30407545",
             "server": "https://zfin.org/",
             "statistics": {
-                "reviewedProteinCount": 3233,
-                "unreviewedProteinCount": 19677
+                "reviewedProteinCount": 3242,
+                "unreviewedProteinCount": 19282
             }
         },
         {
             "abbrev": "RefSeq",
             "category": "Sequence databases",
             "dbUrl": "https://www.ncbi.nlm.nih.gov/protein/%s",
             "doiId": "10.1093/nar/gkv1189",
             "id": "DB-0117",
             "linkType": "Explicit",
             "name": "NCBI Reference Sequences",
             "pubMedId": "26553804",
             "server": "https://www.ncbi.nlm.nih.gov/refseq/",
             "statistics": {
-                "reviewedProteinCount": 475767,
-                "unreviewedProteinCount": 50116869
+                "reviewedProteinCount": 476147,
+                "unreviewedProteinCount": 49906891
             }
         },
         {
             "abbrev": "GeneID",
             "category": "Genome annotation databases",
             "dbUrl": "https://www.ncbi.nlm.nih.gov/gene/%s",
             "doiId": "10.1093/nar/gkq1237",
             "id": "DB-0118",
             "linkType": "Explicit",
             "name": "Database of genes from NCBI RefSeq genomes",
             "pubMedId": "21115458",
             "server": "https://www.ncbi.nlm.nih.gov/gene",
             "statistics": {
-                "reviewedProteinCount": 286927,
-                "unreviewedProteinCount": 13417605
+                "reviewedProteinCount": 286029,
+                "unreviewedProteinCount": 13097509
             }
         },
         {
             "abbrev": "PDBsum",
             "category": "3D structure databases",
             "dbUrl": "https://www.ebi.ac.uk/pdbsum/%s",
             "doiId": "10.1002/pro.3289",
             "id": "DB-0119",
             "linkType": "Explicit",
             "name": "PDBsum; at-a-glance overview of macromolecular structures",
             "pubMedId": "28875543",
             "server": "https://www.ebi.ac.uk/pdbsum/",
             "statistics": {
-                "reviewedProteinCount": 33056,
-                "unreviewedProteinCount": 20497
+                "reviewedProteinCount": 33106,
+                "unreviewedProteinCount": 20449
             }
         },
         {
             "abbrev": "World-2DPAGE",
             "category": "2D gel databases",
             "dbUrl": "https://world-2dpage.expasy.org/repository/%s",
             "doiId": "10.1016/j.jprot.2008.02.005",
@@ -1087,75 +1087,75 @@
             "id": "DB-0123",
             "linkType": "Explicit",
             "name": "Comprehensive resource for the study of protein post-translational modifications (PTMs) in human, mouse and rat.",
             "pubMedId": "25514926",
             "server": "https://www.phosphosite.org",
             "statistics": {
                 "reviewedProteinCount": 39622,
-                "unreviewedProteinCount": 2059
+                "unreviewedProteinCount": 2058
             }
         },
         {
             "abbrev": "ProMEX",
             "category": "Proteomic databases",
             "dbUrl": "http://promex.pph.univie.ac.at/promex/?ac=%s",
             "doiId": "10.3389/fpls.2012.00125",
             "id": "DB-0124",
             "linkType": "Explicit",
             "name": "Protein Mass spectra EXtraction",
             "pubMedId": "22685450",
             "server": "http://promex.pph.univie.ac.at/promex/",
             "statistics": {
-                "reviewedProteinCount": 484,
-                "unreviewedProteinCount": 2180
+                "reviewedProteinCount": 485,
+                "unreviewedProteinCount": 2153
             }
         },
         {
             "abbrev": "CGD",
             "category": "Organism-specific databases",
             "dbUrl": "http://www.candidagenome.org/cgi-bin/locus.pl?dbid=%s",
             "doiId": "10.1093/nar/gkw924",
             "id": "DB-0126",
             "linkType": "Explicit",
             "name": "Candida Genome Database",
             "pubMedId": "27738138",
             "server": "http://www.candidagenome.org/",
             "statistics": {
-                "reviewedProteinCount": 2073,
-                "unreviewedProteinCount": 20627
+                "reviewedProteinCount": 2046,
+                "unreviewedProteinCount": 20610
             }
         },
         {
             "abbrev": "BindingDB",
             "category": "Chemistry databases",
             "dbUrl": "https://www.bindingdb.org/uniprot/%u",
             "doiId": "10.1093/nar/gkv1072",
             "id": "DB-0127",
             "linkType": "Explicit",
             "name": "BindingDB database of measured binding affinities",
             "pubMedId": "26481362",
             "server": "https://www.bindingdb.org/",
             "statistics": {
-                "reviewedProteinCount": 6413,
-                "unreviewedProteinCount": 823
+                "reviewedProteinCount": 6415,
+                "unreviewedProteinCount": 801
             }
         },
         {
             "abbrev": "Xenbase",
             "category": "Organism-specific databases",
             "dbUrl": "https://www.xenbase.org/gene/showgene.do?method=display&geneId=%s",
             "doiId": "10.1093/nar/gkx936",
             "id": "DB-0129",
             "linkType": "Explicit",
             "name": "Xenopus laevis and tropicalis biology and genomics resource",
             "pubMedId": "29059324",
             "server": "https://www.xenbase.org/",
             "statistics": {
-                "reviewedProteinCount": 4560,
-                "unreviewedProteinCount": 48886
+                "reviewedProteinCount": 4829,
+                "unreviewedProteinCount": 62984
             }
         },
         {
             "abbrev": "PRIDE",
             "category": "Proteomic databases",
             "dbUrl": "https://www.ebi.ac.uk/pride/searchSummary.do?queryTypeSelected=identification%20accession%20number&identificationAccessionNumber=%s",
             "doiId": "10.1093/nar/gky1106",
@@ -1176,150 +1176,150 @@
             "doiId": "10.1093/nar/gky1048",
             "id": "DB-0131",
             "linkType": "Explicit",
             "name": "BRENDA Comprehensive Enzyme Information System",
             "pubMedId": "30395242",
             "server": "https://www.brenda-enzymes.org",
             "statistics": {
-                "reviewedProteinCount": 18446,
-                "unreviewedProteinCount": 17324
+                "reviewedProteinCount": 18471,
+                "unreviewedProteinCount": 17284
             }
         },
         {
             "abbrev": "Bgee",
             "category": "Gene expression databases",
             "dbUrl": "https://bgee.org/gene/%s",
             "doiId": "10.1007/978-3-540-69828-9",
             "id": "DB-0133",
             "linkType": "Explicit",
             "name": "Bgee dataBase for Gene Expression Evolution",
             "server": "https://bgee.org",
             "statistics": {
-                "reviewedProteinCount": 61178,
-                "unreviewedProteinCount": 1345223
+                "reviewedProteinCount": 61237,
+                "unreviewedProteinCount": 1344732
             }
         },
         {
             "abbrev": "TCDB",
             "category": "Protein family/group databases",
             "dbUrl": "http://www.tcdb.org/search/result.php?tc=%s",
             "doiId": "10.1093/nar/gkv1103",
             "id": "DB-0135",
             "linkType": "Explicit",
             "name": "Transport Classification Database",
             "pubMedId": "19022853",
             "server": "http://www.tcdb.org/",
             "statistics": {
-                "reviewedProteinCount": 8196,
-                "unreviewedProteinCount": 8695
+                "reviewedProteinCount": 8231,
+                "unreviewedProteinCount": 8698
             }
         },
         {
             "abbrev": "CAZy",
             "category": "Protein family/group databases",
             "dbUrl": "http://www.cazy.org/fam/%s.html",
             "doiId": "10.1093/nar/gkt1178",
             "id": "DB-0136",
             "linkType": "Explicit",
             "name": "Carbohydrate-Active enZymes",
             "pubMedId": "24270786",
             "server": "http://www.cazy.org/",
             "statistics": {
-                "reviewedProteinCount": 8643,
-                "unreviewedProteinCount": 117848
+                "reviewedProteinCount": 8644,
+                "unreviewedProteinCount": 117678
             }
         },
         {
             "abbrev": "OMA",
             "category": "Phylogenomic databases",
             "dbUrl": "https://omabrowser.org/oma/group/%u",
             "doiId": "10.1093/nar/gkaa1007",
             "id": "DB-0137",
             "linkType": "Explicit",
             "name": "Identification of Orthologs from Complete Genome Data",
             "pubMedId": "33174605",
             "server": "https://omabrowser.org/",
             "statistics": {
-                "reviewedProteinCount": 430151,
-                "unreviewedProteinCount": 10358914
+                "reviewedProteinCount": 429864,
+                "unreviewedProteinCount": 11690033
             }
         },
         {
             "abbrev": "UCSC",
             "category": "Genome annotation databases",
             "dbUrl": "https://genome.ucsc.edu/cgi-bin/hgLinkIn?resource=uniprot&id=%u",
             "doiId": "10.1093/nar/gky1095",
             "id": "DB-0139",
             "linkType": "Explicit",
             "name": "UCSC genome browser",
             "pubMedId": "30407534",
             "server": "https://genome.ucsc.edu/",
             "statistics": {
-                "reviewedProteinCount": 46305,
-                "unreviewedProteinCount": 88722
+                "reviewedProteinCount": 46331,
+                "unreviewedProteinCount": 88676
             }
         },
         {
             "abbrev": "CTD",
             "category": "Organism-specific databases",
             "dbUrl": "https://ctdbase.org/detail.go?type=gene&db=GENE&acc=%s",
             "doiId": "10.1093/nar/gkaa891",
             "id": "DB-0140",
             "linkType": "Explicit",
             "name": "Comparative Toxicogenomics Database",
             "pubMedId": "33068428",
             "server": "https://ctdbase.org/",
             "statistics": {
-                "reviewedProteinCount": 75142,
-                "unreviewedProteinCount": 1958320
+                "reviewedProteinCount": 75243,
+                "unreviewedProteinCount": 1963313
             }
         },
         {
             "abbrev": "STRING",
             "category": "Protein-protein interaction databases",
             "dbUrl": "https://string-db.org/network/%s",
             "doiId": "10.1093/nar/gky1131",
             "id": "DB-0141",
             "linkType": "Explicit",
             "name": "STRING",
             "pubMedId": "30476243",
             "server": "https://string-db.org/",
             "statistics": {
-                "reviewedProteinCount": 366062,
-                "unreviewedProteinCount": 33260284
+                "reviewedProteinCount": 366207,
+                "unreviewedProteinCount": 33206660
             }
         },
         {
             "abbrev": "OrthoDB",
             "category": "Phylogenomic databases",
             "dbUrl": "https://www.orthodb.org/?gene=%u",
             "doiId": "10.1093/nar/gky1053",
             "id": "DB-0143",
             "linkType": "Explicit",
             "name": "Database of Orthologous Groups",
             "pubMedId": "30395283",
             "server": "https://www.orthodb.org",
             "statistics": {
-                "reviewedProteinCount": 274272,
-                "unreviewedProteinCount": 53898491
+                "reviewedProteinCount": 274409,
+                "unreviewedProteinCount": 53793844
             }
         },
         {
             "abbrev": "PhylomeDB",
             "category": "Phylogenomic databases",
             "dbUrl": "http://phylomedb.org/search_phylome/?seqid=%u",
             "doiId": "10.1093/nar/gkt1177",
             "id": "DB-0144",
             "linkType": "Explicit",
             "name": "Database for complete collections of gene phylogenies",
             "pubMedId": "24275491",
             "server": "http://phylomedb.org/",
             "statistics": {
-                "reviewedProteinCount": 115376,
-                "unreviewedProteinCount": 586134
+                "reviewedProteinCount": 115402,
+                "unreviewedProteinCount": 582698
             }
         },
         {
             "abbrev": "ArachnoServer",
             "category": "Organism-specific databases",
             "dbUrl": "http://www.arachnoserver.org",
             "doiId": "10.1093/bioinformatics/btx661",
@@ -1340,136 +1340,136 @@
             "doiId": "10.1093/nar/gkm1020",
             "id": "DB-0146",
             "linkType": "Explicit",
             "name": "InParanoid",
             "pubMedId": "18055500",
             "server": "https://inparanoid.sbc.su.se/",
             "statistics": {
-                "reviewedProteinCount": 141829,
-                "unreviewedProteinCount": 1972266
+                "reviewedProteinCount": 141883,
+                "unreviewedProteinCount": 1971941
             }
         },
         {
             "abbrev": "EnsemblBacteria",
             "category": "Genome annotation databases",
             "dbUrl": "https://www.ensemblgenomes.org/id/%s",
             "doiId": "10.1093/nar/gkz890",
             "id": "DB-0147",
             "linkType": "Explicit",
             "name": "Ensembl bacterial and archaeal genome annotation project",
             "pubMedId": "31598706",
             "server": "https://bacteria.ensembl.org/",
             "statistics": {
-                "reviewedProteinCount": 298242,
-                "unreviewedProteinCount": 72031958
+                "reviewedProteinCount": 298299,
+                "unreviewedProteinCount": 71712318
             }
         },
         {
             "abbrev": "EnsemblFungi",
             "category": "Genome annotation databases",
             "dbUrl": "https://www.ensemblgenomes.org/id/%s",
             "doiId": "10.1093/nar/gkz890",
             "id": "DB-0148",
             "linkType": "Explicit",
             "name": "Ensembl fungal genome annotation project",
             "pubMedId": "31598706",
             "server": "https://fungi.ensembl.org/",
             "statistics": {
-                "reviewedProteinCount": 22519,
-                "unreviewedProteinCount": 777944
+                "reviewedProteinCount": 22522,
+                "unreviewedProteinCount": 777938
             }
         },
         {
             "abbrev": "EnsemblMetazoa",
             "category": "Genome annotation databases",
             "dbUrl": "https://www.ensemblgenomes.org/id/%s",
             "doiId": "10.1093/nar/gkz890",
             "id": "DB-0149",
             "linkType": "Explicit",
             "name": "Ensembl metazoan genome annotation project",
             "pubMedId": "31598706",
             "server": "https://metazoa.ensembl.org/",
             "statistics": {
-                "reviewedProteinCount": 11357,
-                "unreviewedProteinCount": 2150818
+                "reviewedProteinCount": 11375,
+                "unreviewedProteinCount": 2150771
             }
         },
         {
             "abbrev": "EnsemblPlants",
             "category": "Genome annotation databases",
             "dbUrl": "https://www.ensemblgenomes.org/id/%s",
             "doiId": "10.1093/nar/gkz890",
             "id": "DB-0150",
             "linkType": "Explicit",
             "name": "Ensembl plant genome annotation project",
             "pubMedId": "31598706",
             "server": "https://plants.ensembl.org/",
             "statistics": {
-                "reviewedProteinCount": 21987,
-                "unreviewedProteinCount": 3156852
+                "reviewedProteinCount": 22054,
+                "unreviewedProteinCount": 3156794
             }
         },
         {
             "abbrev": "EnsemblProtists",
             "category": "Genome annotation databases",
             "dbUrl": "https://www.ensemblgenomes.org/id/%s",
             "doiId": "10.1093/nar/gkz890",
             "id": "DB-0151",
             "linkType": "Explicit",
             "name": "Ensembl protists genome annotation project",
             "pubMedId": "31598706",
             "server": "https://protists.ensembl.org/",
             "statistics": {
-                "reviewedProteinCount": 5042,
-                "unreviewedProteinCount": 1584389
+                "reviewedProteinCount": 5054,
+                "unreviewedProteinCount": 1584378
             }
         },
         {
             "abbrev": "eggNOG",
             "category": "Phylogenomic databases",
             "dbUrl": "http://eggnogdb.embl.de/#/app/results?seqid=%u&target_nogs=%s",
             "doiId": "10.1093/nar/gkac1022",
             "id": "DB-0152",
             "linkType": "Explicit",
             "name": "evolutionary genealogy of genes",
             "pubMedId": "36399505",
             "server": "http://eggnogdb.embl.de/",
             "statistics": {
-                "reviewedProteinCount": 332694,
-                "unreviewedProteinCount": 12563914
+                "reviewedProteinCount": 332846,
+                "unreviewedProteinCount": 12537058
             }
         },
         {
             "abbrev": "VEuPathDB",
             "category": "Organism-specific databases",
             "dbUrl": "https://www.veupathdb.org/gene/%s",
             "doiId": "10.1093/nar/gkw1105",
             "id": "DB-0153",
             "linkType": "Explicit",
             "name": "Eukaryotic Pathogen, Vector and Host Database Resources",
             "pubMedId": "27903906",
             "server": "https://veupathdb.org/veupathdb/app",
             "statistics": {
-                "reviewedProteinCount": 73836,
-                "unreviewedProteinCount": 4685200
+                "reviewedProteinCount": 74308,
+                "unreviewedProteinCount": 4822891
             }
         },
         {
             "abbrev": "SUPFAM",
             "category": "Family and domain databases",
             "dbUrl": "https://supfam.org/SUPERFAMILY/cgi-bin/scop.cgi?ipid=%s",
             "doiId": "10.1006/jmbi.2001.5080",
             "id": "DB-0155",
             "linkType": "Explicit",
             "name": "Superfamily database of structural and functional annotation",
             "pubMedId": "11697912",
             "server": "https://supfam.org",
             "statistics": {
-                "reviewedProteinCount": 458240,
-                "unreviewedProteinCount": 145900407
+                "reviewedProteinCount": 458455,
+                "unreviewedProteinCount": 156828541
             }
         },
         {
             "abbrev": "ConoServer",
             "category": "Organism-specific databases",
             "dbUrl": "https://www.conoserver.org/?page=card&table=protein&id=%s",
             "doiId": "10.1093/nar/gkr886",
@@ -1490,16 +1490,16 @@
             "doiId": "10.1093/nar/gkr930",
             "id": "DB-0158",
             "linkType": "Explicit",
             "name": "Molecular INTeraction database",
             "pubMedId": "22096227",
             "server": "https://mint.bio.uniroma2.it/",
             "statistics": {
-                "reviewedProteinCount": 23435,
-                "unreviewedProteinCount": 3075
+                "reviewedProteinCount": 23449,
+                "unreviewedProteinCount": 3195
             }
         },
         {
             "abbrev": "Allergome",
             "category": "Protein family/group databases",
             "dbUrl": "https://www.allergome.org/script/dettaglio.php?id_molecule=%s",
             "doiId": "10.1007/s11882-009-0055-9",
@@ -1520,46 +1520,46 @@
             "doiId": "10.1093/nar/gkw1062",
             "id": "DB-0161",
             "linkType": "Explicit",
             "name": "neXtProt; the human protein knowledge platform",
             "pubMedId": "27899619",
             "server": "https://www.nextprot.org/",
             "statistics": {
-                "reviewedProteinCount": 20330,
+                "reviewedProteinCount": 20328,
                 "unreviewedProteinCount": 0
             }
         },
         {
             "abbrev": "GeneTree",
             "category": "Phylogenomic databases",
             "dbUrl": "https://www.ensemblgenomes.org/id-genetree/%s",
             "doiId": "10.1093/database/bav096",
             "id": "DB-0162",
             "linkType": "Explicit",
             "name": "Ensembl GeneTree",
             "pubMedId": "26896847",
             "server": "https://ensemblgenomes.org",
             "statistics": {
-                "reviewedProteinCount": 58895,
-                "unreviewedProteinCount": 5953308
+                "reviewedProteinCount": 56985,
+                "unreviewedProteinCount": 5939575
             }
         },
         {
             "abbrev": "PATRIC",
             "category": "Genome annotation databases",
             "dbUrl": "https://www.patricbrc.org/view/Feature/%s",
             "doiId": "10.1093/nar/gkz943",
             "id": "DB-0165",
             "linkType": "Explicit",
             "name": "Pathosystems Resource Integration Center (PATRIC)",
             "pubMedId": "31667520",
             "server": "https://patricbrc.org/",
             "statistics": {
-                "reviewedProteinCount": 92820,
-                "unreviewedProteinCount": 13382185
+                "reviewedProteinCount": 92845,
+                "unreviewedProteinCount": 13289167
             }
         },
         {
             "abbrev": "DMDM",
             "category": "Genetic variation databases",
             "dbUrl": "https://bioinf.umbc.edu/dmdm/gene_prot_page.php?search_type=protein&id=%s",
             "doiId": "10.1093/bioinformatics/btq447",
@@ -1580,61 +1580,61 @@
             "doiId": "10.1007/s10969-011-9100-8",
             "id": "DB-0167",
             "linkType": "Explicit",
             "name": "The DNASU plasmid repository",
             "pubMedId": "21360289",
             "server": "https://dnasu.org/DNASU/",
             "statistics": {
-                "reviewedProteinCount": 48176,
-                "unreviewedProteinCount": 94805
+                "reviewedProteinCount": 48194,
+                "unreviewedProteinCount": 94762
             }
         },
         {
             "abbrev": "EvolutionaryTrace",
             "category": "Miscellaneous databases",
             "dbUrl": "http://mammoth.bcm.tmc.edu/cgi-bin/report_maker_ls/uniprotTraceServerResults.pl?identifier=%s",
             "doiId": "10.1007/978-1-61779-465-0_3",
             "id": "DB-0168",
             "linkType": "Explicit",
             "name": "Relative evolutionary importance of amino acids within a protein sequence",
             "pubMedId": "22183528",
             "server": "http://lichtargelab.org/software/ETserver",
             "statistics": {
-                "reviewedProteinCount": 16750,
-                "unreviewedProteinCount": 5890
+                "reviewedProteinCount": 16760,
+                "unreviewedProteinCount": 5875
             }
         },
         {
             "abbrev": "GenomeRNAi",
             "category": "Miscellaneous databases",
             "dbUrl": "http://genomernai.org/genedetails/%s",
             "doiId": "10.1093/nar/gks1170",
             "id": "DB-0169",
             "linkType": "Explicit",
             "name": "Database of phenotypes from RNA interference screens in Drosophila and Homo sapiens",
             "pubMedId": "23193271",
             "server": "http://genomernai.dkfz.de/",
             "statistics": {
-                "reviewedProteinCount": 22243,
-                "unreviewedProteinCount": 31491
+                "reviewedProteinCount": 22245,
+                "unreviewedProteinCount": 31487
             }
         },
         {
             "abbrev": "UniPathway",
             "category": "Enzyme and pathway databases",
             "dbUrl": "http://www.unipathway.org?upid=%s&entryac=%u",
             "doiId": "10.1093/nar/gkr1023",
             "id": "DB-0170",
             "linkType": "Explicit",
             "name": "UniPathway",
             "pubMedId": "22102589",
             "server": "http://www.unipathway.org",
             "statistics": {
-                "reviewedProteinCount": 126046,
-                "unreviewedProteinCount": 14018914
+                "reviewedProteinCount": 126077,
+                "unreviewedProteinCount": 13904203
             }
         },
         {
             "abbrev": "RCSB-PDB",
             "category": "3D structure databases",
             "dbUrl": "https://www.rcsb.org/structure/%s",
             "doiId": "10.1093/nar/gkj120",
@@ -1670,31 +1670,31 @@
             "doiId": "10.1074/mcp.O111.014704",
             "id": "DB-0173",
             "linkType": "Explicit",
             "name": "PaxDb, a database of protein abundance averages across all three domains of life",
             "pubMedId": "22535208",
             "server": "https://pax-db.org",
             "statistics": {
-                "reviewedProteinCount": 126414,
-                "unreviewedProteinCount": 207575
+                "reviewedProteinCount": 126433,
+                "unreviewedProteinCount": 207217
             }
         },
         {
             "abbrev": "ChEMBL",
             "category": "Chemistry databases",
-            "dbUrl": "https://www.ebi.ac.uk/chembldb/target/inspect/%s",
-            "doiId": "10.1093/nar/gkr777",
+            "dbUrl": "https://www.ebi.ac.uk/chembl/target/inspect/%s",
+            "doiId": "10.1093/nar/gky1075",
             "id": "DB-0174",
             "linkType": "Explicit",
             "name": "ChEMBL database of bioactive drug-like small molecules",
-            "pubMedId": "21948594",
-            "server": "https://www.ebi.ac.uk/chembldb",
+            "pubMedId": "30398643",
+            "server": "https://www.ebi.ac.uk/chembl",
             "statistics": {
-                "reviewedProteinCount": 8623,
-                "unreviewedProteinCount": 1132
+                "reviewedProteinCount": 8626,
+                "unreviewedProteinCount": 1128
             }
         },
         {
             "abbrev": "CLAE",
             "category": "Protein family/group databases",
             "dbUrl": "https://clae.fungalgenomics.ca/enzyme/%s",
             "doiId": "10.1093/database/bav008",
@@ -1715,46 +1715,46 @@
             "doiId": "10.1093/nar/gkz1025",
             "id": "DB-0176",
             "linkType": "Explicit",
             "name": "ChiTaRS",
             "pubMedId": "31747015",
             "server": "http://chitars.md.biu.ac.il/",
             "statistics": {
-                "reviewedProteinCount": 29668,
-                "unreviewedProteinCount": 171036
+                "reviewedProteinCount": 29676,
+                "unreviewedProteinCount": 170984
             }
         },
         {
             "abbrev": "SABIO-RK",
             "category": "Enzyme and pathway databases",
             "dbUrl": "https://sabiork.h-its.org/newSearch?q=UniProtKB_AC:%u",
             "doiId": "10.1093/nar/gkr1046",
             "id": "DB-0177",
             "linkType": "Explicit",
             "name": "SABIO-RK",
             "pubMedId": "22102587",
             "server": "https://sabiork.h-its.org/",
             "statistics": {
-                "reviewedProteinCount": 5328,
-                "unreviewedProteinCount": 831
+                "reviewedProteinCount": 5575,
+                "unreviewedProteinCount": 880
             }
         },
         {
             "abbrev": "SignaLink",
             "category": "Enzyme and pathway databases",
             "dbUrl": "http://signalink.org/protein/%u",
             "doiId": "10.1093/bioinformatics/btq310",
             "id": "DB-0179",
             "linkType": "Explicit",
             "name": "SignaLink",
             "pubMedId": "20542890",
             "server": "http://signalink.org/",
             "statistics": {
-                "reviewedProteinCount": 19961,
-                "unreviewedProteinCount": 30
+                "reviewedProteinCount": 19960,
+                "unreviewedProteinCount": 29
             }
         },
         {
             "abbrev": "GeneWiki",
             "category": "Miscellaneous databases",
             "dbUrl": "https://en.wikipedia.org/wiki/%s",
             "doiId": "10.1371/journal.pbio.0060175",
@@ -1775,30 +1775,30 @@
             "doiId": "10.1093/nar/gkt1173",
             "id": "DB-0181",
             "linkType": "Explicit",
             "name": "Protein Ontology",
             "pubMedId": "24270789",
             "server": "https://proconsortium.org/",
             "statistics": {
-                "reviewedProteinCount": 98139,
-                "unreviewedProteinCount": 2056
+                "reviewedProteinCount": 98140,
+                "unreviewedProteinCount": 2053
             }
         },
         {
             "abbrev": "GuidetoPHARMACOLOGY",
             "category": "Chemistry databases",
             "dbUrl": "https://www.guidetopharmacology.org/GRAC/ObjectDisplayForward?objectId=%s",
             "doiId": "10.1093/nar/gkab1010",
             "id": "DB-0182",
             "linkType": "Explicit",
             "name": "IUPHAR/BPS Guide to PHARMACOLOGY",
             "pubMedId": "34718737",
             "server": "https://www.guidetopharmacology.org",
             "statistics": {
-                "reviewedProteinCount": 2137,
+                "reviewedProteinCount": 2144,
                 "unreviewedProteinCount": 22
             }
         },
         {
             "abbrev": "MobiDB",
             "category": "Family and domain databases",
             "dbUrl": "https://mobidb.bio.unipd.it/entries/%u",
@@ -1820,73 +1820,73 @@
             "doiId": "10.1093/nar/gkq1116",
             "id": "DB-0184",
             "linkType": "Explicit",
             "name": "The Biological General Repository for Interaction Datasets (BioGRID)",
             "pubMedId": "21071413",
             "server": "https://thebiogrid.org/",
             "statistics": {
-                "reviewedProteinCount": 59122,
+                "reviewedProteinCount": 59224,
                 "unreviewedProteinCount": 0
             }
         },
         {
             "abbrev": "TreeFam",
             "category": "Phylogenomic databases",
             "dbUrl": "http://www.treefam.org/family/%s",
             "doiId": "10.1093/nar/gkt1055",
             "id": "DB-0185",
             "linkType": "Explicit",
             "name": "TreeFam database of animal gene trees",
             "pubMedId": "24194607",
             "server": "http://www.treefam.org",
             "statistics": {
-                "reviewedProteinCount": 46017,
-                "unreviewedProteinCount": 472861
+                "reviewedProteinCount": 46041,
+                "unreviewedProteinCount": 472578
             }
         },
         {
             "abbrev": "MaxQB",
             "category": "Proteomic databases",
             "dbUrl": "http://maxqb.biochem.mpg.de/mxdb/protein/show/%u",
             "doiId": "10.1074/mcp.M111.014068",
             "id": "DB-0186",
             "linkType": "Explicit",
             "name": "MaxQB - The MaxQuant DataBase",
             "pubMedId": "22301388",
             "server": "http://maxqb.biochem.mpg.de/mxdb/",
             "statistics": {
-                "reviewedProteinCount": 33703,
-                "unreviewedProteinCount": 37951
+                "reviewedProteinCount": 33704,
+                "unreviewedProteinCount": 37737
             }
         },
         {
             "abbrev": "CCDS",
             "category": "Sequence databases",
             "dbUrl": "https://www.ncbi.nlm.nih.gov/CCDS/CcdsBrowse.cgi?REQUEST=CCDS&GO=MainBrowse&DATA=%s",
             "doiId": "10.1101/gr.080531.108",
             "id": "DB-0187",
             "linkType": "Explicit",
             "name": "The Consensus CDS (CCDS) project",
             "pubMedId": "19498102",
             "server": "https://www.ncbi.nlm.nih.gov/CCDS",
             "statistics": {
-                "reviewedProteinCount": 34555,
+                "reviewedProteinCount": 34570,
                 "unreviewedProteinCount": 0
             }
         },
         {
             "abbrev": "GeneReviews",
             "category": "Organism-specific databases",
             "dbUrl": "https://www.ncbi.nlm.nih.gov/books/NBK1116/?term=%s",
             "id": "DB-0188",
             "linkType": "Explicit",
             "name": "GeneReviews a resource of expert-authored, peer-reviewed disease descriptions.",
             "server": "https://www.ncbi.nlm.nih.gov/books/NBK1116",
             "statistics": {
-                "reviewedProteinCount": 1553,
+                "reviewedProteinCount": 1559,
                 "unreviewedProteinCount": 0
             }
         },
         {
             "abbrev": "MoonProt",
             "category": "Protein family/group databases",
             "dbUrl": "http://www.moonlightingproteins.org/proteins/?q=%u",
@@ -1894,15 +1894,15 @@
             "id": "DB-0189",
             "linkType": "Explicit",
             "name": "MoonProt database of moonlighting proteins",
             "pubMedId": "10087914",
             "server": "http://www.moonlightingproteins.org/",
             "statistics": {
                 "reviewedProteinCount": 281,
-                "unreviewedProteinCount": 50
+                "unreviewedProteinCount": 49
             }
         },
         {
             "abbrev": "DEPOD",
             "category": "PTM databases",
             "dbUrl": "http://depod.bioss.uni-freiburg.de/showp.php?name=%s",
             "doiId": "doi",
@@ -1923,61 +1923,61 @@
             "doiId": "10.1093/nar/gkr981",
             "id": "DB-0191",
             "linkType": "Explicit",
             "name": "Proteomes",
             "pubMedId": "22102590",
             "server": "https://www.uniprot.org/proteomes",
             "statistics": {
-                "reviewedProteinCount": 461476,
-                "unreviewedProteinCount": 217445989
+                "reviewedProteinCount": 462193,
+                "unreviewedProteinCount": 221575743
             }
         },
         {
             "abbrev": "BioMuta",
             "category": "Genetic variation databases",
             "dbUrl": "https://hive.biochemistry.gwu.edu/tools/biomuta/biomuta.php?gene=%s",
             "doiId": "10.1093/database/bau022",
             "id": "DB-0192",
             "linkType": "Explicit",
             "name": "BioMuta curated single-nucleotide variation and disease association database",
             "pubMedId": "24667251",
             "server": "https://hive.biochemistry.gwu.edu/tools/biomuta/",
             "statistics": {
-                "reviewedProteinCount": 20283,
-                "unreviewedProteinCount": 913
+                "reviewedProteinCount": 20282,
+                "unreviewedProteinCount": 912
             }
         },
         {
             "abbrev": "ESTHER",
             "category": "Protein family/group databases",
             "dbUrl": "https://bioweb.supagro.inra.fr/ESTHER/gene_locus?name=%s&class=Gene_locus",
             "doiId": "10.1093/nar/gks1154",
             "id": "DB-0193",
             "linkType": "Explicit",
             "name": "ESTHER database of the Alpha/Beta-hydrolase fold superfamily of proteins",
             "pubMedId": "23193256",
             "server": "https://bioweb.supagro.inra.fr/ESTHER/general?what=index",
             "statistics": {
-                "reviewedProteinCount": 2973,
-                "unreviewedProteinCount": 83719
+                "reviewedProteinCount": 2977,
+                "unreviewedProteinCount": 83530
             }
         },
         {
             "abbrev": "Genevisible",
             "category": "Gene expression databases",
             "dbUrl": "https://genevisible.com/tissues/%d/UniProt/%u",
             "doiId": "10.1104/pp.104.900198",
             "id": "DB-0194",
             "linkType": "Explicit",
             "name": "Genevisible search portal to normalized and curated expression data from Genevestigator",
             "pubMedId": "16896229",
             "server": "https://genevisible.com/search",
             "statistics": {
                 "reviewedProteinCount": 55270,
-                "unreviewedProteinCount": 15098
+                "unreviewedProteinCount": 15093
             }
         },
         {
             "abbrev": "WBParaSite",
             "category": "Genome annotation databases",
             "dbUrl": "https://parasite.wormbase.org/id/%s",
             "doiId": "10.1093/nar/gkt1063",
@@ -1998,15 +1998,15 @@
             "doiId": "10.1002/0471250953.bi0124s47",
             "id": "DB-0196",
             "linkType": "Explicit",
             "name": "MalaCards human disease database",
             "pubMedId": "25199789",
             "server": "https://www.malacards.org",
             "statistics": {
-                "reviewedProteinCount": 5358,
+                "reviewedProteinCount": 5525,
                 "unreviewedProteinCount": 94
             }
         },
         {
             "abbrev": "SwissLipids",
             "category": "Chemistry databases",
             "dbUrl": "https://www.swisslipids.org/#/entity/%s/",
@@ -2043,166 +2043,166 @@
             "doiId": "10.1093/nar/gkx1104",
             "id": "DB-0200",
             "linkType": "Explicit",
             "name": "iPTMnet integrated resource for PTMs in systems biology context",
             "pubMedId": "29145615",
             "server": "https://research.bioinformatics.udel.edu/iptmnet/",
             "statistics": {
-                "reviewedProteinCount": 54133,
-                "unreviewedProteinCount": 9832
+                "reviewedProteinCount": 54142,
+                "unreviewedProteinCount": 7651
             }
         },
         {
             "abbrev": "SwissPalm",
             "category": "PTM databases",
             "dbUrl": "https://swisspalm.org/proteins/%u",
             "doiId": "10.12688/f1000research.6464.1",
             "id": "DB-0201",
             "linkType": "Explicit",
             "name": "SwissPalm database of S-palmitoylation events",
             "pubMedId": "26339475",
             "server": "https://swisspalm.org",
             "statistics": {
-                "reviewedProteinCount": 13324,
-                "unreviewedProteinCount": 4342
+                "reviewedProteinCount": 13328,
+                "unreviewedProteinCount": 4651
             }
         },
         {
             "abbrev": "TopDownProteomics",
             "category": "Proteomic databases",
             "dbUrl": "http://repository.topdownproteomics.org/Proteoforms?query=%u",
             "doiId": "10.1002/pmic.201300438",
             "id": "DB-0204",
             "linkType": "Explicit",
             "name": "Consortium for Top Down Proteomics",
             "pubMedId": "24644084",
             "server": "http://repository.topdownproteomics.org/",
             "statistics": {
-                "reviewedProteinCount": 2956,
-                "unreviewedProteinCount": 270
+                "reviewedProteinCount": 2957,
+                "unreviewedProteinCount": 268
             }
         },
         {
             "abbrev": "EPD",
             "category": "Proteomic databases",
             "dbUrl": "https://www.peptracker.com/epd/analytics/?protein_id=%u",
             "doiId": "10.1093/nar/gkx807",
             "id": "DB-0205",
             "linkType": "Explicit",
             "name": "Encyclopedia of Proteome Dynamics",
             "pubMedId": "28981707",
             "server": "https://www.peptracker.com/epd/analytics/",
             "statistics": {
-                "reviewedProteinCount": 23236,
-                "unreviewedProteinCount": 11891
+                "reviewedProteinCount": 23243,
+                "unreviewedProteinCount": 11882
             }
         },
         {
             "abbrev": "SIGNOR",
             "category": "Enzyme and pathway databases",
             "dbUrl": "https://signor.uniroma2.it/relation_result.php?id=%u",
             "doiId": "10.1093/nar/gkv1048",
             "id": "DB-0206",
             "linkType": "Explicit",
             "name": "SIGNOR Signaling Network Open Resource",
             "pubMedId": "26467481",
             "server": "https://signor.uniroma2.it/",
             "statistics": {
-                "reviewedProteinCount": 7065,
-                "unreviewedProteinCount": 4
+                "reviewedProteinCount": 7117,
+                "unreviewedProteinCount": 5
             }
         },
         {
             "abbrev": "CDD",
             "category": "Family and domain databases",
             "dbUrl": "https://www.ncbi.nlm.nih.gov/Structure/cdd/cddsrv.cgi?uid=%s",
             "doiId": "DOI",
             "id": "DB-0214",
             "linkType": "Explicit",
             "name": "Conserved Domains Database",
             "pubMedId": "25414356",
             "server": "https://www.ncbi.nlm.nih.gov/cdd",
             "statistics": {
-                "reviewedProteinCount": 294774,
-                "unreviewedProteinCount": 76193264
+                "reviewedProteinCount": 300384,
+                "unreviewedProteinCount": 82484082
             }
         },
         {
             "abbrev": "DisGeNET",
             "category": "Organism-specific databases",
             "dbUrl": "https://disgenet.org/search?q=%s",
             "doiId": "10.1093/nar/gkz1021",
             "id": "DB-0218",
             "linkType": "Explicit",
             "name": "DisGeNET",
             "pubMedId": "31680165",
             "server": "https://www.disgenet.org/",
             "statistics": {
-                "reviewedProteinCount": 16796,
+                "reviewedProteinCount": 16795,
                 "unreviewedProteinCount": 0
             }
         },
         {
             "abbrev": "OpenTargets",
             "category": "Organism-specific databases",
             "dbUrl": "https://platform.opentargets.org/target/%s/associations",
             "doiId": "10.1093/nar/gkw1055",
             "id": "DB-0219",
             "linkType": "Explicit",
             "name": "Open Targets",
             "pubMedId": "27899665",
             "server": "https://platform.opentargets.org/",
             "statistics": {
-                "reviewedProteinCount": 18243,
+                "reviewedProteinCount": 18250,
                 "unreviewedProteinCount": 587
             }
         },
         {
             "abbrev": "SFLD",
             "category": "Family and domain databases",
             "dbUrl": "https://www.ebi.ac.uk/interpro/entry/sfld/%s",
             "doiId": "10.1093/nar/gkt1130",
             "id": "DB-0220",
             "linkType": "Explicit",
             "name": "Structure-Function Linkage Database",
             "pubMedId": "24271399",
             "server": "http://sfld.rbvi.ucsf.edu/archive/django/index.html",
             "statistics": {
-                "reviewedProteinCount": 9031,
-                "unreviewedProteinCount": 2150249
+                "reviewedProteinCount": 9036,
+                "unreviewedProteinCount": 2316604
             }
         },
         {
             "abbrev": "Araport",
             "category": "Organism-specific databases",
             "dbUrl": "https://bar.utoronto.ca/thalemine/portal.do?externalids=%s",
             "doiId": "10.1093/nar/gku1200",
             "id": "DB-0221",
             "linkType": "Explicit",
             "name": "Arabidopsis Information Portal",
             "pubMedId": "25414324",
             "server": "https://bar.utoronto.ca/thalemine/begin.do",
             "statistics": {
-                "reviewedProteinCount": 16221,
-                "unreviewedProteinCount": 29812
+                "reviewedProteinCount": 16267,
+                "unreviewedProteinCount": 29765
             }
         },
         {
             "abbrev": "ELM",
             "category": "Protein-protein interaction databases",
             "dbUrl": "http://elm.eu.org/instances.html?q=%u",
             "doiId": "10.1093/nar/gkz1030",
             "id": "DB-0223",
             "linkType": "Explicit",
             "name": "The Eukaryotic Linear Motif resource for Functional Sites in Proteins",
             "pubMedId": "31680160",
             "server": "http://elm.eu.org/",
             "statistics": {
-                "reviewedProteinCount": 1813,
-                "unreviewedProteinCount": 78
+                "reviewedProteinCount": 1814,
+                "unreviewedProteinCount": 77
             }
         },
         {
             "abbrev": "CORUM",
             "category": "Protein-protein interaction databases",
             "dbUrl": "http://mips.helmholtz-muenchen.de/corum/#?uniprotID=%u",
             "doiId": "10.1093/nar/gky973",
@@ -2238,16 +2238,16 @@
             "doiId": "10.1093/nar/gkaa980",
             "id": "DB-0226",
             "linkType": "Explicit",
             "name": "Vertebrate Gene Nomenclature Database",
             "pubMedId": "33152070",
             "server": "https://vertebrate.genenames.org/",
             "statistics": {
-                "reviewedProteinCount": 4468,
-                "unreviewedProteinCount": 231985
+                "reviewedProteinCount": 4477,
+                "unreviewedProteinCount": 231935
             }
         },
         {
             "abbrev": "GlyConnect",
             "category": "PTM databases",
             "dbUrl": "https://glyconnect.expasy.org/browser/proteins/%s",
             "doiId": "10.1021/acs.jproteome.8b00766",
@@ -2283,16 +2283,16 @@
             "doiId": "10.1093/nar/gkz974",
             "id": "DB-0229",
             "linkType": "Explicit",
             "name": "ProteomicsDB",
             "pubMedId": "31665479",
             "server": "https://www.proteomicsdb.org/",
             "statistics": {
-                "reviewedProteinCount": 45270,
-                "unreviewedProteinCount": 70982
+                "reviewedProteinCount": 45321,
+                "unreviewedProteinCount": 70905
             }
         },
         {
             "abbrev": "MoonDB",
             "category": "Protein family/group databases",
             "dbUrl": "http://moondb.hb.univ-amu.fr/protein/%u",
             "doiId": "10.1093/nar/gky1039",
@@ -2313,31 +2313,31 @@
             "doiId": "10.1093/nar/gky832",
             "id": "DB-0231",
             "linkType": "Explicit",
             "name": "UniLectin database of carbohydrate-binding proteins",
             "pubMedId": "30239928",
             "server": "https://unilectin.eu",
             "statistics": {
-                "reviewedProteinCount": 312,
-                "unreviewedProteinCount": 214
+                "reviewedProteinCount": 315,
+                "unreviewedProteinCount": 231
             }
         },
         {
             "abbrev": "jPOST",
             "category": "Proteomic databases",
             "dbUrl": "https://globe.jpostdb.org/protein?id=%u",
             "doiId": "10.1093/nar/gkw1080",
             "id": "DB-0233",
             "linkType": "Explicit",
             "name": "jPOST - Japan Proteome Standard Repository/Database",
             "pubMedId": "27899654",
             "server": "https://globe.jpostdb.org/",
             "statistics": {
-                "reviewedProteinCount": 26405,
-                "unreviewedProteinCount": 10866
+                "reviewedProteinCount": 26406,
+                "unreviewedProteinCount": 10861
             }
         },
         {
             "abbrev": "SWISS-MODEL-Workspace",
             "category": "3D structure databases",
             "dbUrl": "https://swissmodel.expasy.org/interactive/?ac=%u",
             "doiId": "10.1093/nar/gky427",
@@ -2357,21 +2357,21 @@
             "dbUrl": "https://web.expasy.org/cgi-bin/abcd/search_abcd.pl?input=%u",
             "id": "DB-0236",
             "linkType": "Explicit",
             "name": "ABCD curated depository of sequenced antibodies",
             "server": "https://web.expasy.org/abcd",
             "statistics": {
                 "reviewedProteinCount": 3011,
-                "unreviewedProteinCount": 521
+                "unreviewedProteinCount": 517
             }
         },
         {
             "abbrev": "NIAGADS",
             "category": "Organism-specific databases",
-            "dbUrl": "https://www.niagads.org/genomics/showRecord.do?name=GeneRecordClasses.GeneRecordClass&source_id=%s",
+            "dbUrl": "https://www.niagads.org/genomics/app/record/gene/%s",
             "id": "DB-0237",
             "linkType": "Explicit",
             "name": "NIAGADS Genomics Database",
             "server": "https://www.niagads.org/genomics/",
             "statistics": {
                 "reviewedProteinCount": 69,
                 "unreviewedProteinCount": 255
@@ -2399,45 +2399,45 @@
             "doiId": "10.1093/nar/gky963",
             "id": "DB-0239",
             "linkType": "Explicit",
             "name": "DrugCentral",
             "pubMedId": "30371892",
             "server": "https://drugcentral.org/",
             "statistics": {
-                "reviewedProteinCount": 2564,
-                "unreviewedProteinCount": 158
+                "reviewedProteinCount": 2565,
+                "unreviewedProteinCount": 156
             }
         },
         {
             "abbrev": "Pharos",
             "category": "Miscellaneous databases",
             "dbUrl": "https://pharos.nih.gov/targets/%u",
             "doiId": "10.1093/nar/gkw1072",
             "id": "DB-0240",
             "linkType": "Explicit",
             "name": "Pharos NIH Druggable Genome Knowledgebase",
             "pubMedId": "27903890",
             "server": "https://pharos.nih.gov",
             "statistics": {
-                "reviewedProteinCount": 20231,
+                "reviewedProteinCount": 20228,
                 "unreviewedProteinCount": 0
             }
         },
         {
             "abbrev": "MassIVE",
             "category": "Proteomic databases",
             "dbUrl": "https://massive.ucsd.edu/ProteoSAFe/protein_explorer.jsp?libraries=2&protein_name=%u",
             "doiId": "10.1016/j.cels.2018.08.004",
             "id": "DB-0241",
             "linkType": "Explicit",
             "name": "MassIVE - Mass Spectrometry Interactive Virtual Environment",
             "pubMedId": "30172843",
             "server": "https://massive.ucsd.edu/",
             "statistics": {
-                "reviewedProteinCount": 18718,
+                "reviewedProteinCount": 18717,
                 "unreviewedProteinCount": 0
             }
         },
         {
             "abbrev": "PlantReactome",
             "category": "Enzyme and pathway databases",
             "dbUrl": "https://plantreactome.gramene.org/PathwayBrowser/#/%s&FLG=%u",
@@ -2445,15 +2445,15 @@
             "id": "DB-0243",
             "linkType": "Explicit",
             "name": "Reactome - a knowledgebase of biological pathways and processes for plant species",
             "pubMedId": "27799469",
             "server": "https://plantreactome.gramene.org",
             "statistics": {
                 "reviewedProteinCount": 750,
-                "unreviewedProteinCount": 864
+                "unreviewedProteinCount": 881
             }
         },
         {
             "abbrev": "PDBe-KB",
             "category": "3D structure databases",
             "dbUrl": "https://pdbe-kb.org/proteins/%u",
             "doiId": "10.1093/nar/gkz853",
@@ -2474,16 +2474,16 @@
             "doiId": "10.1093/nar/gky967",
             "id": "DB-0246",
             "linkType": "Explicit",
             "name": "RNAct, Protein-RNA interaction predictions for model organisms.",
             "pubMedId": "30445601",
             "server": "https://rnact.crg.eu",
             "statistics": {
-                "reviewedProteinCount": 43057,
-                "unreviewedProteinCount": 2658
+                "reviewedProteinCount": 43058,
+                "unreviewedProteinCount": 2654
             }
         },
         {
             "abbrev": "MetOSite",
             "category": "PTM databases",
             "dbUrl": "https://metosite.uma.es/scan/%u",
             "doiId": "10.1093/bioinformatics/btz462",
@@ -2504,31 +2504,31 @@
             "doiId": "10.1093/nar/gkw1089",
             "id": "DB-0248",
             "linkType": "Explicit",
             "name": "Pathogen-Host Interaction database",
             "pubMedId": "24972168",
             "server": "http://www.phi-base.org/",
             "statistics": {
-                "reviewedProteinCount": 1264,
-                "unreviewedProteinCount": 4185
+                "reviewedProteinCount": 1266,
+                "unreviewedProteinCount": 4182
             }
         },
         {
             "abbrev": "Antibodypedia",
             "category": "Protocols and materials databases",
             "dbUrl": "https://antibodypedia.com/gene/%s",
             "doiId": "10.1074/mcp.M800264-MCP200",
             "id": "DB-0249",
             "linkType": "Explicit",
             "name": "Antibodypedia a portal for validated antibodies",
             "pubMedId": "18667413",
             "server": "https://antibodypedia.com/",
             "statistics": {
-                "reviewedProteinCount": 32091,
-                "unreviewedProteinCount": 74557
+                "reviewedProteinCount": 32103,
+                "unreviewedProteinCount": 74523
             }
         },
         {
             "abbrev": "IDEAL",
             "category": "Family and domain databases",
             "dbUrl": "https://www.ideal-db.org/ideal.php?id=%s",
             "doiId": "10.1093/nar/gkt1010",
@@ -2549,61 +2549,61 @@
             "doiId": "10.1093/nar/gky1079",
             "id": "DB-0252",
             "linkType": "Explicit",
             "name": "BioGRID ORCS database of CRISPR phenotype screens",
             "pubMedId": "30476227",
             "server": "https://orcs.thebiogrid.org",
             "statistics": {
-                "reviewedProteinCount": 44286,
-                "unreviewedProteinCount": 59028
+                "reviewedProteinCount": 44302,
+                "unreviewedProteinCount": 59005
             }
         },
         {
             "abbrev": "PathwayCommons",
             "category": "Enzyme and pathway databases",
             "dbUrl": "http://apps.pathwaycommons.org/search?q=%u",
             "doiId": "10.1093/nar/gkq1039",
             "id": "DB-0253",
             "linkType": "Explicit",
             "name": "Pathway Commons web resource for biological pathway data",
             "pubMedId": "21071392",
             "server": "http://www.pathwaycommons.org",
             "statistics": {
-                "reviewedProteinCount": 19457,
+                "reviewedProteinCount": 19455,
                 "unreviewedProteinCount": 0
             }
         },
         {
             "abbrev": "GlyGen",
             "category": "PTM databases",
             "dbUrl": "https://glygen.org/protein/%u#glycosylation",
             "doiId": "10.1093/glycob/cwz080",
             "id": "DB-0254",
             "linkType": "Explicit",
             "name": "GlyGen",
             "pubMedId": "31616925",
             "server": "https://glygen.org",
             "statistics": {
-                "reviewedProteinCount": 15684,
-                "unreviewedProteinCount": 17
+                "reviewedProteinCount": 21280,
+                "unreviewedProteinCount": 252
             }
         },
         {
             "abbrev": "BMRB",
             "category": "3D structure databases",
             "dbUrl": "https://bmrb.io/data_library/summary/protein.php?uniprot=%u",
             "doiId": "10.1093/nar/gkm957",
             "id": "DB-0256",
             "linkType": "Explicit",
             "name": "Biological Magnetic Resonance Data Bank",
             "pubMedId": "17984079",
             "server": "https://bmrb.io/",
             "statistics": {
-                "reviewedProteinCount": 6899,
-                "unreviewedProteinCount": 317
+                "reviewedProteinCount": 6901,
+                "unreviewedProteinCount": 338
             }
         },
         {
             "abbrev": "PCDDB",
             "category": "3D structure databases",
             "dbUrl": "https://pcddb.cryst.bbk.ac.uk/uniprot/%u",
             "doiId": "10.1093/nar/gkw796",
@@ -2624,59 +2624,59 @@
             "doiId": "10.1002/pro.3731",
             "id": "DB-0258",
             "linkType": "Explicit",
             "name": "Small Angle Scattering Biological Data Bank",
             "pubMedId": "31576635",
             "server": "https://www.sasbdb.org/",
             "statistics": {
-                "reviewedProteinCount": 710,
-                "unreviewedProteinCount": 207
+                "reviewedProteinCount": 736,
+                "unreviewedProteinCount": 231
             }
         },
         {
             "abbrev": "CPTC",
             "category": "Protocols and materials databases",
             "dbUrl": "https://antibodies.cancer.gov/uniprot/%u",
             "id": "DB-0259",
             "linkType": "Explicit",
             "name": "The CPTC Antibody Portal",
             "server": "https://antibodies.cancer.gov",
             "statistics": {
-                "reviewedProteinCount": 374,
+                "reviewedProteinCount": 379,
                 "unreviewedProteinCount": 0
             }
         },
         {
             "abbrev": "MANE-Select",
             "category": "Genome annotation databases",
             "dbUrl": "https://www.ensembl.org/id/%s",
             "doiId": "10.1038/s41586-022-04558-8",
             "id": "DB-0261",
             "linkType": "Explicit",
             "name": "Matched Annotation from NCBI and EMBL-EBI (MANE) - Phase one",
             "pubMedId": "35388217",
             "server": "https://www.ensembl.org/info/genome/genebuild/mane.html",
             "statistics": {
-                "reviewedProteinCount": 18049,
-                "unreviewedProteinCount": 4779
+                "reviewedProteinCount": 18055,
+                "unreviewedProteinCount": 4776
             }
         },
         {
             "abbrev": "AlphaFoldDB",
             "category": "3D structure databases",
             "dbUrl": "https://alphafold.ebi.ac.uk/entry/%u",
             "doiId": "10.1093/nar/gkab1061",
             "id": "DB-0262",
             "linkType": "Explicit",
             "name": "AlphaFold Protein Structure Database",
             "pubMedId": "34791371",
             "server": "https://alphafold.ebi.ac.uk/",
             "statistics": {
-                "reviewedProteinCount": 545443,
-                "unreviewedProteinCount": 194751822
+                "reviewedProteinCount": 545675,
+                "unreviewedProteinCount": 193678189
             }
         },
         {
             "abbrev": "ClinGen",
             "category": "Genetic variation databases",
             "dbUrl": "https://search.clinicalgenome.org/kb/genes/%s",
             "doiId": "10.1056/NEJMsr1406261",
@@ -2712,28 +2712,28 @@
             "doiId": "10.1093/nar/gkz813",
             "id": "DB-0266",
             "linkType": "Explicit",
             "name": "The Alliance of Genome Resources",
             "pubMedId": "31552413",
             "server": "https://alliancegenome.org/",
             "statistics": {
-                "reviewedProteinCount": 60026,
-                "unreviewedProteinCount": 137026
+                "reviewedProteinCount": 60054,
+                "unreviewedProteinCount": 136950
             }
         },
         {
             "abbrev": "GlyCosmos",
             "category": "PTM databases",
             "dbUrl": "https://glycosmos.org/glycoproteins/show/uniprot/%u",
             "doiId": "10.1038/s41592-020-0879-8",
             "id": "DB-0267",
             "linkType": "Explicit",
             "name": "GlyCosmos Portal integrating glycosciences with life sciences",
-            "pubMedId": "2572234",
+            "pubMedId": "32572234",
             "server": "https://glycosmos.org/",
             "statistics": {
-                "reviewedProteinCount": 28903,
-                "unreviewedProteinCount": 39361
+                "reviewedProteinCount": 28904,
+                "unreviewedProteinCount": 38708
             }
         }
     ]
 }
```

### Comparing `bioregistry-0.9.3/src/bioregistry/data/external/wikidata/curation.tsv` & `bioregistry-0.9.4/src/bioregistry/data/external/wikidata/curation.tsv`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/data/external/wikidata/processed.json` & `bioregistry-0.9.4/src/bioregistry/data/external/wikidata/processed.json`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/data/metaregistry.json` & `bioregistry-0.9.4/src/bioregistry/data/metaregistry.json`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/data/mismatch.json` & `bioregistry-0.9.4/src/bioregistry/data/mismatch.json`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/data/processing_ols.json` & `bioregistry-0.9.4/src/bioregistry/data/processing_ols.json`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/export/cli.py` & `bioregistry-0.9.4/src/bioregistry/export/cli.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/export/prefix_maps.py` & `bioregistry-0.9.4/src/bioregistry/export/prefix_maps.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/export/rdf_export.py` & `bioregistry-0.9.4/src/bioregistry/export/rdf_export.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/export/sssom_export.py` & `bioregistry-0.9.4/src/bioregistry/export/sssom_export.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/export/tables_export.py` & `bioregistry-0.9.4/src/bioregistry/export/tables_export.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/export/tsv_export.py` & `bioregistry-0.9.4/src/bioregistry/export/tsv_export.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/export/warnings_export.py` & `bioregistry-0.9.4/src/bioregistry/export/warnings_export.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/export/yaml_export.py` & `bioregistry-0.9.4/src/bioregistry/export/yaml_export.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/external/__init__.py` & `bioregistry-0.9.4/src/bioregistry/external/__init__.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/external/aberowl.py` & `bioregistry-0.9.4/src/bioregistry/external/aberowl.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/external/bartoc.py` & `bioregistry-0.9.4/src/bioregistry/external/bartoc.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/external/biocontext.py` & `bioregistry-0.9.4/src/bioregistry/external/biocontext.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/external/biolink.py` & `bioregistry-0.9.4/src/bioregistry/external/biolink.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/external/bioportal.py` & `bioregistry-0.9.4/src/bioregistry/external/bioportal.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/external/cellosaurus.py` & `bioregistry-0.9.4/src/bioregistry/external/cellosaurus.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/external/cheminf.py` & `bioregistry-0.9.4/src/bioregistry/external/cheminf.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/external/cropoct.py` & `bioregistry-0.9.4/src/bioregistry/external/cropoct.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/external/edam.py` & `bioregistry-0.9.4/src/bioregistry/external/edam.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/external/fairsharing.py` & `bioregistry-0.9.4/src/bioregistry/external/fairsharing.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/external/go.py` & `bioregistry-0.9.4/src/bioregistry/external/go.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/external/hl7/OID_Report.csv` & `bioregistry-0.9.4/src/bioregistry/external/hl7/OID_Report.csv`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/external/hl7/__init__.py` & `bioregistry-0.9.4/src/bioregistry/external/hl7/__init__.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/external/miriam.py` & `bioregistry-0.9.4/src/bioregistry/external/miriam.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/external/n2t.py` & `bioregistry-0.9.4/src/bioregistry/external/n2t.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/external/ncbi.py` & `bioregistry-0.9.4/src/bioregistry/external/ncbi.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/external/obofoundry.py` & `bioregistry-0.9.4/src/bioregistry/external/obofoundry.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/external/ols.py` & `bioregistry-0.9.4/src/bioregistry/external/ols.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/external/ontobee.py` & `bioregistry-0.9.4/src/bioregistry/external/ontobee.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/external/prefixcommons.py` & `bioregistry-0.9.4/src/bioregistry/external/prefixcommons.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/external/re3data.py` & `bioregistry-0.9.4/src/bioregistry/external/re3data.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/external/uniprot.py` & `bioregistry-0.9.4/src/bioregistry/external/uniprot.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/external/wikidata.py` & `bioregistry-0.9.4/src/bioregistry/external/wikidata.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/gh/github_client.py` & `bioregistry-0.9.4/src/bioregistry/gh/github_client.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/gh/new_prefix.py` & `bioregistry-0.9.4/src/bioregistry/gh/new_prefix.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/health/check_homepages.py` & `bioregistry-0.9.4/src/bioregistry/health/check_homepages.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/health/check_providers.py` & `bioregistry-0.9.4/src/bioregistry/health/check_providers.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/health/cli.py` & `bioregistry-0.9.4/src/bioregistry/health/cli.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/license_standardizer.py` & `bioregistry-0.9.4/src/bioregistry/license_standardizer.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/lint.py` & `bioregistry-0.9.4/src/bioregistry/lint.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/metaresource_api.py` & `bioregistry-0.9.4/src/bioregistry/metaresource_api.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/pandas.py` & `bioregistry-0.9.4/src/bioregistry/pandas.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/parse_iri.py` & `bioregistry-0.9.4/src/bioregistry/parse_iri.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/record_accumulator.py` & `bioregistry-0.9.4/src/bioregistry/record_accumulator.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/resolve.py` & `bioregistry-0.9.4/src/bioregistry/resolve.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/resolve_identifier.py` & `bioregistry-0.9.4/src/bioregistry/resolve_identifier.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/resource_manager.py` & `bioregistry-0.9.4/src/bioregistry/resource_manager.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/schema/constants.py` & `bioregistry-0.9.4/src/bioregistry/schema/constants.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/schema/schema.json` & `bioregistry-0.9.4/src/bioregistry/schema/schema.json`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/schema/struct.py` & `bioregistry-0.9.4/src/bioregistry/schema/struct.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/schema/utils.py` & `bioregistry-0.9.4/src/bioregistry/schema/utils.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/schema_utils.py` & `bioregistry-0.9.4/src/bioregistry/schema_utils.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/summary.py` & `bioregistry-0.9.4/src/bioregistry/summary.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/upload_ndex.py` & `bioregistry-0.9.4/src/bioregistry/upload_ndex.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/uri_format.py` & `bioregistry-0.9.4/src/bioregistry/uri_format.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/utils.py` & `bioregistry-0.9.4/src/bioregistry/utils.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry/version.py` & `bioregistry-0.9.4/src/bioregistry/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 __all__ = [
     "VERSION",
     "get_version",
     "get_git_hash",
 ]
 
-VERSION = "0.9.3"
+VERSION = "0.9.4"
 
 
 def get_git_hash() -> Optional[str]:
     """Get the bioregistry git hash."""
     with open(os.devnull, "w") as devnull:
         try:
             ret = check_output(  # noqa: S603,S607
```

### Comparing `bioregistry-0.9.3/src/bioregistry.egg-info/PKG-INFO` & `bioregistry-0.9.4/src/bioregistry.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bioregistry
-Version: 0.9.3
+Version: 0.9.4
 Summary: Integrated registry of biological databases and nomenclatures
 Home-page: https://github.com/biopragmatics/bioregistry
 Download-URL: https://github.com/biopragmatics/bioregistry/releases
 Author: Charles Tapley Hoyt
 Author-email: cthoyt@gmail.com
 Maintainer: Charles Tapley Hoyt
 Maintainer-email: cthoyt@gmail.com
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: bioregistry Version: 0.9.3 Summary: Integrated
+Metadata-Version: 2.1 Name: bioregistry Version: 0.9.4 Summary: Integrated
 registry of biological databases and nomenclatures Home-page: https://
 github.com/biopragmatics/bioregistry Download-URL: https://github.com/
 biopragmatics/bioregistry/releases Author: Charles Tapley Hoyt Author-email:
 cthoyt@gmail.com Maintainer: Charles Tapley Hoyt Maintainer-email:
 cthoyt@gmail.com License: MIT Project-URL: Bug Tracker, https://github.com/
 biopragmatics/bioregistry/issues Keywords: databases,biological
 databases,biomedical databases Classifier: Development Status :: 4 - Beta
```

### Comparing `bioregistry-0.9.3/src/bioregistry.egg-info/SOURCES.txt` & `bioregistry-0.9.4/src/bioregistry.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/src/bioregistry.egg-info/requires.txt` & `bioregistry-0.9.4/src/bioregistry.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/tests/test_collections.py` & `bioregistry-0.9.4/tests/test_collections.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/tests/test_contexts.py` & `bioregistry-0.9.4/tests/test_contexts.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/tests/test_data.py` & `bioregistry-0.9.4/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/tests/test_duplicates.py` & `bioregistry-0.9.4/tests/test_duplicates.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/tests/test_identifiers_org.py` & `bioregistry-0.9.4/tests/test_identifiers_org.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/tests/test_indra.py` & `bioregistry-0.9.4/tests/test_indra.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/tests/test_manager.py` & `bioregistry-0.9.4/tests/test_manager.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/tests/test_metaregistry.py` & `bioregistry-0.9.4/tests/test_metaregistry.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/tests/test_ols.py` & `bioregistry-0.9.4/tests/test_ols.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/tests/test_pandas.py` & `bioregistry-0.9.4/tests/test_pandas.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/tests/test_resolve.py` & `bioregistry-0.9.4/tests/test_resolve.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/tests/test_sparql.py` & `bioregistry-0.9.4/tests/test_sparql.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/tests/test_usages.py` & `bioregistry-0.9.4/tests/test_usages.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/tests/test_utils.py` & `bioregistry-0.9.4/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/tests/test_web/test_api.py` & `bioregistry-0.9.4/tests/test_web/test_api.py`

 * *Files identical despite different names*

### Comparing `bioregistry-0.9.3/tests/test_web/test_ui.py` & `bioregistry-0.9.4/tests/test_web/test_ui.py`

 * *Files identical despite different names*

