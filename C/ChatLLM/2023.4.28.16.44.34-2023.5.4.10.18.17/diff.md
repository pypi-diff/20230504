# Comparing `tmp/ChatLLM-2023.4.28.16.44.34.tar.gz` & `tmp/ChatLLM-2023.5.4.10.18.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ChatLLM-2023.4.28.16.44.34.tar", last modified: Fri Apr 28 08:44:34 2023, max compression
+gzip compressed data, was "ChatLLM-2023.5.4.10.18.17.tar", last modified: Thu May  4 02:18:17 2023, max compression
```

## Comparing `ChatLLM-2023.4.28.16.44.34.tar` & `ChatLLM-2023.5.4.10.18.17.tar`

### file list

```diff
@@ -1,105 +1,106 @@
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 08:44:34.303230 ChatLLM-2023.4.28.16.44.34/
--rw-r--r--   0 betterme   (501) staff       (20)      292 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.16.44.34/.editorconfig
--rw-r--r--   0 betterme   (501) staff       (20)     1196 2023-04-20 11:38:14.000000 ChatLLM-2023.4.28.16.44.34/.gitignore
--rw-r--r--   0 betterme   (501) staff       (20)      697 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.16.44.34/.travis.yml
--rw-r--r--   0 betterme   (501) staff       (20)      149 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.16.44.34/AUTHORS.rst
--rw-r--r--   0 betterme   (501) staff       (20)     3530 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.16.44.34/CONTRIBUTING.rst
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 08:44:34.283469 ChatLLM-2023.4.28.16.44.34/ChatLLM.egg-info/
--rw-r--r--   0 betterme   (501) staff       (20)     5810 2023-04-28 08:44:34.000000 ChatLLM-2023.4.28.16.44.34/ChatLLM.egg-info/PKG-INFO
--rw-r--r--   0 betterme   (501) staff       (20)     1963 2023-04-28 08:44:34.000000 ChatLLM-2023.4.28.16.44.34/ChatLLM.egg-info/SOURCES.txt
--rw-r--r--   0 betterme   (501) staff       (20)        1 2023-04-28 08:44:34.000000 ChatLLM-2023.4.28.16.44.34/ChatLLM.egg-info/dependency_links.txt
--rw-r--r--   0 betterme   (501) staff       (20)       53 2023-04-28 08:44:34.000000 ChatLLM-2023.4.28.16.44.34/ChatLLM.egg-info/entry_points.txt
--rw-r--r--   0 betterme   (501) staff       (20)        1 2023-04-28 08:44:34.000000 ChatLLM-2023.4.28.16.44.34/ChatLLM.egg-info/not-zip-safe
--rw-r--r--   0 betterme   (501) staff       (20)      172 2023-04-28 08:44:34.000000 ChatLLM-2023.4.28.16.44.34/ChatLLM.egg-info/requires.txt
--rw-r--r--   0 betterme   (501) staff       (20)        8 2023-04-28 08:44:34.000000 ChatLLM-2023.4.28.16.44.34/ChatLLM.egg-info/top_level.txt
--rw-r--r--   0 betterme   (501) staff       (20)       89 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.16.44.34/HISTORY.rst
--rw-r--r--   0 betterme   (501) staff       (20)     1066 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.16.44.34/LICENSE
--rw-r--r--   0 betterme   (501) staff       (20)      289 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.16.44.34/MANIFEST.in
--rw-r--r--   0 betterme   (501) staff       (20)     2215 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.16.44.34/Makefile
--rw-r--r--   0 betterme   (501) staff       (20)     5810 2023-04-28 08:44:34.303057 ChatLLM-2023.4.28.16.44.34/PKG-INFO
--rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-26 04:55:25.000000 ChatLLM-2023.4.28.16.44.34/README.bak.md
--rw-r--r--   0 betterme   (501) staff       (20)     4907 2023-04-28 07:55:35.000000 ChatLLM-2023.4.28.16.44.34/README.md
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 08:44:34.283831 ChatLLM-2023.4.28.16.44.34/chatllm/
--rw-r--r--   0 betterme   (501) staff       (20)      199 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.16.44.34/chatllm/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 08:44:34.284342 ChatLLM-2023.4.28.16.44.34/chatllm/_his/
--rw-r--r--   0 betterme   (501) staff       (20)     1482 2023-04-20 12:23:09.000000 ChatLLM-2023.4.28.16.44.34/chatllm/_his/FaissANN.py
--rw-r--r--   0 betterme   (501) staff       (20)      286 2023-04-27 10:06:48.000000 ChatLLM-2023.4.28.16.44.34/chatllm/_his/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1812 2023-04-25 08:31:06.000000 ChatLLM-2023.4.28.16.44.34/chatllm/_his/_chatllm.py
--rw-r--r--   0 betterme   (501) staff       (20)     2493 2023-04-27 10:06:48.000000 ChatLLM-2023.4.28.16.44.34/chatllm/_his/_qa.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 08:44:34.284608 ChatLLM-2023.4.28.16.44.34/chatllm/api/
--rw-r--r--   0 betterme   (501) staff       (20)      270 2023-04-28 01:04:39.000000 ChatLLM-2023.4.28.16.44.34/chatllm/api/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1827 2023-04-28 02:36:43.000000 ChatLLM-2023.4.28.16.44.34/chatllm/api/stream_api.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 08:44:34.286242 ChatLLM-2023.4.28.16.44.34/chatllm/applications/
--rw-r--r--   0 betterme   (501) staff       (20)     3532 2023-04-25 01:19:43.000000 ChatLLM-2023.4.28.16.44.34/chatllm/applications/Question2Answer.py
--rw-r--r--   0 betterme   (501) staff       (20)      294 2023-04-25 08:32:56.000000 ChatLLM-2023.4.28.16.44.34/chatllm/applications/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2805 2023-04-27 04:33:02.000000 ChatLLM-2023.4.28.16.44.34/chatllm/applications/chatann.py
--rw-r--r--   0 betterme   (501) staff       (20)     3838 2023-04-28 07:06:18.000000 ChatLLM-2023.4.28.16.44.34/chatllm/applications/chatbase.py
--rw-r--r--   0 betterme   (501) staff       (20)     1176 2023-04-26 01:00:01.000000 ChatLLM-2023.4.28.16.44.34/chatllm/applications/chatcrawler.py
--rw-r--r--   0 betterme   (501) staff       (20)      266 2023-04-25 01:23:41.000000 ChatLLM-2023.4.28.16.44.34/chatllm/applications/chatdoc.py
--rw-r--r--   0 betterme   (501) staff       (20)     1357 2023-04-28 07:16:03.000000 ChatLLM-2023.4.28.16.44.34/chatllm/applications/chatpdf.py
--rw-r--r--   0 betterme   (501) staff       (20)      269 2023-04-26 00:59:00.000000 ChatLLM-2023.4.28.16.44.34/chatllm/applications/chatsearch.py
--rw-r--r--   0 betterme   (501) staff       (20)      266 2023-04-25 01:23:41.000000 ChatLLM-2023.4.28.16.44.34/chatllm/applications/chatweb.py
--rw-r--r--   0 betterme   (501) staff       (20)     1895 2023-04-27 02:58:56.000000 ChatLLM-2023.4.28.16.44.34/chatllm/applications/chatwhoosh.py
--rw-r--r--   0 betterme   (501) staff       (20)      286 2023-04-21 05:42:37.000000 ChatLLM-2023.4.28.16.44.34/chatllm/applications/pipeline.py
--rw-r--r--   0 betterme   (501) staff       (20)     1964 2023-04-27 09:24:25.000000 ChatLLM-2023.4.28.16.44.34/chatllm/chatyuan.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 08:44:34.286621 ChatLLM-2023.4.28.16.44.34/chatllm/clis/
--rw-r--r--   0 betterme   (501) staff       (20)      413 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.16.44.34/chatllm/clis/README.md
--rw-r--r--   0 betterme   (501) staff       (20)      279 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.16.44.34/chatllm/clis/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1334 2023-04-28 07:03:35.000000 ChatLLM-2023.4.28.16.44.34/chatllm/clis/cli.py
--rw-r--r--   0 betterme   (501) staff       (20)     1439 2023-04-27 01:39:42.000000 ChatLLM-2023.4.28.16.44.34/chatllm/embedding.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 08:44:34.286892 ChatLLM-2023.4.28.16.44.34/chatllm/parse_utils/
--rw-r--r--   0 betterme   (501) staff       (20)      302 2023-04-25 01:22:30.000000 ChatLLM-2023.4.28.16.44.34/chatllm/parse_utils/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      273 2023-04-21 04:20:09.000000 ChatLLM-2023.4.28.16.44.34/chatllm/parse_utils/doc_parse.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 08:44:34.287397 ChatLLM-2023.4.28.16.44.34/chatllm/utils/
--rw-r--r--   0 betterme   (501) staff       (20)      278 2023-04-28 04:20:30.000000 ChatLLM-2023.4.28.16.44.34/chatllm/utils/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      271 2023-04-28 04:37:16.000000 ChatLLM-2023.4.28.16.44.34/chatllm/utils/_textsplitter.py
--rw-r--r--   0 betterme   (501) staff       (20)     2142 2023-04-28 07:05:00.000000 ChatLLM-2023.4.28.16.44.34/chatllm/utils/common.py
--rw-r--r--   0 betterme   (501) staff       (20)     3208 2023-04-28 04:38:58.000000 ChatLLM-2023.4.28.16.44.34/chatllm/utils/gpu_utils.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 08:44:34.288167 ChatLLM-2023.4.28.16.44.34/chatllm/webui/
--rw-r--r--   0 betterme   (501) staff       (20)      270 2023-04-20 02:48:59.000000 ChatLLM-2023.4.28.16.44.34/chatllm/webui/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1488 2023-04-26 01:00:01.000000 ChatLLM-2023.4.28.16.44.34/chatllm/webui/chatbase.py
--rw-r--r--   0 betterme   (501) staff       (20)     3017 2023-04-28 06:43:45.000000 ChatLLM-2023.4.28.16.44.34/chatllm/webui/chatpdf.py
--rw-r--r--   0 betterme   (501) staff       (20)     4311 2023-04-26 01:00:01.000000 ChatLLM-2023.4.28.16.44.34/chatllm/webui/gradio_ui.py
--rw-r--r--   0 betterme   (501) staff       (20)     1819 2023-04-25 03:04:12.000000 ChatLLM-2023.4.28.16.44.34/chatllm/webui/nice_ui.py
--rw-r--r--   0 betterme   (501) staff       (20)      220 2023-04-26 07:34:11.000000 ChatLLM-2023.4.28.16.44.34/chatllm/webui/run.sh
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 08:44:34.291668 ChatLLM-2023.4.28.16.44.34/data/
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 08:44:34.293144 ChatLLM-2023.4.28.16.44.34/data/imgs/
--rw-r--r--   0 betterme   (501) staff       (20)   206137 2023-04-26 05:39:20.000000 ChatLLM-2023.4.28.16.44.34/data/imgs/LLM.drawio.png
--rw-r--r--   0 betterme   (501) staff       (20)   206363 2023-04-26 05:33:47.000000 ChatLLM-2023.4.28.16.44.34/data/imgs/LLM.png
--rw-r--r--   0 betterme   (501) staff       (20)  1230065 2023-04-26 08:27:23.000000 ChatLLM-2023.4.28.16.44.34/data/imgs/chatpdf.gif
--rw-r--r--   0 betterme   (501) staff       (20)    45633 2023-04-26 04:24:13.000000 ChatLLM-2023.4.28.16.44.34/data/imgs/chatpdf_ann_df.png
--rw-r--r--   0 betterme   (501) staff       (20)    29400 2023-04-27 10:24:48.000000 ChatLLM-2023.4.28.16.44.34/data/imgs/role.png
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 08:44:34.295270 ChatLLM-2023.4.28.16.44.34/data/医/
--rw-r--r--   0 betterme   (501) staff       (20)  3891700 2023-04-20 11:48:19.000000 ChatLLM-2023.4.28.16.44.34/data/医/500种中药现代研究.txt
--rw-r--r--   0 betterme   (501) staff       (20)  4926489 2023-04-20 11:46:24.000000 ChatLLM-2023.4.28.16.44.34/data/医/古今医统大全.txt
--rw-r--r--   0 betterme   (501) staff       (20)     1633 2023-04-20 07:17:41.000000 ChatLLM-2023.4.28.16.44.34/data/姚明.txt
--rw-r--r--   0 betterme   (501) staff       (20)      946 2023-04-20 07:17:41.000000 ChatLLM-2023.4.28.16.44.34/data/王治郅.txt
--rw-r--r--   0 betterme   (501) staff       (20)     1291 2023-04-20 07:17:41.000000 ChatLLM-2023.4.28.16.44.34/data/科比.txt
--rw-r--r--   0 betterme   (501) staff       (20)  3051914 2023-04-25 02:58:13.000000 ChatLLM-2023.4.28.16.44.34/data/财报.pdf
--rw-r--r--   0 betterme   (501) staff       (20)      493 2023-04-20 07:17:41.000000 ChatLLM-2023.4.28.16.44.34/data/马保国.txt
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 08:44:34.302345 ChatLLM-2023.4.28.16.44.34/docs/
--rw-r--r--   0 betterme   (501) staff       (20)      564 2023-04-26 04:55:25.000000 ChatLLM-2023.4.28.16.44.34/docs/INSTALL.md
--rw-r--r--   0 betterme   (501) staff       (20)      608 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.16.44.34/docs/Makefile
--rw-r--r--   0 betterme   (501) staff       (20)     4846 2023-04-27 11:05:23.000000 ChatLLM-2023.4.28.16.44.34/docs/README.md
--rw-r--r--   0 betterme   (501) staff       (20)       26 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.16.44.34/docs/_config.yml
--rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.16.44.34/docs/authors.rst
--rwxr-xr-x   0 betterme   (501) staff       (20)     4763 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.16.44.34/docs/conf.py
--rw-r--r--   0 betterme   (501) staff       (20)       33 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.16.44.34/docs/contributing.rst
--rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.16.44.34/docs/history.rst
--rw-r--r--   0 betterme   (501) staff       (20)      304 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.16.44.34/docs/index.rst
--rw-r--r--   0 betterme   (501) staff       (20)      805 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.16.44.34/docs/make.bat
--rw-r--r--   0 betterme   (501) staff       (20)       27 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.16.44.34/docs/readme.rst
--rw-r--r--   0 betterme   (501) staff       (20)       69 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.16.44.34/docs/usage.rst
--rwxr-xr-x   0 betterme   (501) staff       (20)      269 2023-04-28 07:55:35.000000 ChatLLM-2023.4.28.16.44.34/git_init.sh
--rwxr-xr-x   0 betterme   (501) staff       (20)      152 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.16.44.34/pypi.sh
--rw-r--r--   0 betterme   (501) staff       (20)       78 2023-04-28 08:43:50.000000 ChatLLM-2023.4.28.16.44.34/requirements.txt
--rw-r--r--   0 betterme   (501) staff       (20)       14 2023-04-28 08:44:21.000000 ChatLLM-2023.4.28.16.44.34/requirements_api.txt
--rw-r--r--   0 betterme   (501) staff       (20)       18 2023-04-28 08:44:32.000000 ChatLLM-2023.4.28.16.44.34/requirements_pdf.txt
--rw-r--r--   0 betterme   (501) staff       (20)       10 2023-04-28 08:44:32.000000 ChatLLM-2023.4.28.16.44.34/requirements_streamlit.txt
--rw-r--r--   0 betterme   (501) staff       (20)       38 2023-04-28 08:44:34.303293 ChatLLM-2023.4.28.16.44.34/setup.cfg
--rw-r--r--   0 betterme   (501) staff       (20)     1897 2023-04-28 08:42:35.000000 ChatLLM-2023.4.28.16.44.34/setup.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-04-28 08:44:34.302761 ChatLLM-2023.4.28.16.44.34/tests/
--rw-r--r--   0 betterme   (501) staff       (20)       37 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.16.44.34/tests/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      852 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.16.44.34/tests/test_llm4gpt.py
--rw-r--r--   0 betterme   (501) staff       (20)    51173 2023-04-21 11:31:44.000000 ChatLLM-2023.4.28.16.44.34/tests/内存型.ipynb
--rw-r--r--   0 betterme   (501) staff       (20)      288 2023-04-11 04:23:57.000000 ChatLLM-2023.4.28.16.44.34/tox.ini
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 02:18:17.847090 ChatLLM-2023.5.4.10.18.17/
+-rw-r--r--   0 betterme   (501) staff       (20)      292 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.10.18.17/.editorconfig
+-rw-r--r--   0 betterme   (501) staff       (20)     1196 2023-04-20 11:38:14.000000 ChatLLM-2023.5.4.10.18.17/.gitignore
+-rw-r--r--   0 betterme   (501) staff       (20)      697 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.10.18.17/.travis.yml
+-rw-r--r--   0 betterme   (501) staff       (20)      149 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.10.18.17/AUTHORS.rst
+-rw-r--r--   0 betterme   (501) staff       (20)     3530 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.10.18.17/CONTRIBUTING.rst
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 02:18:17.805790 ChatLLM-2023.5.4.10.18.17/ChatLLM.egg-info/
+-rw-r--r--   0 betterme   (501) staff       (20)     5809 2023-05-04 02:18:17.000000 ChatLLM-2023.5.4.10.18.17/ChatLLM.egg-info/PKG-INFO
+-rw-r--r--   0 betterme   (501) staff       (20)     1997 2023-05-04 02:18:17.000000 ChatLLM-2023.5.4.10.18.17/ChatLLM.egg-info/SOURCES.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        1 2023-05-04 02:18:17.000000 ChatLLM-2023.5.4.10.18.17/ChatLLM.egg-info/dependency_links.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       53 2023-05-04 02:18:17.000000 ChatLLM-2023.5.4.10.18.17/ChatLLM.egg-info/entry_points.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        1 2023-05-04 02:18:17.000000 ChatLLM-2023.5.4.10.18.17/ChatLLM.egg-info/not-zip-safe
+-rw-r--r--   0 betterme   (501) staff       (20)      186 2023-05-04 02:18:17.000000 ChatLLM-2023.5.4.10.18.17/ChatLLM.egg-info/requires.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        8 2023-05-04 02:18:17.000000 ChatLLM-2023.5.4.10.18.17/ChatLLM.egg-info/top_level.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       89 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.10.18.17/HISTORY.rst
+-rw-r--r--   0 betterme   (501) staff       (20)     1066 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.10.18.17/LICENSE
+-rw-r--r--   0 betterme   (501) staff       (20)      289 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.10.18.17/MANIFEST.in
+-rw-r--r--   0 betterme   (501) staff       (20)     2215 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.10.18.17/Makefile
+-rw-r--r--   0 betterme   (501) staff       (20)     5809 2023-05-04 02:18:17.846905 ChatLLM-2023.5.4.10.18.17/PKG-INFO
+-rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-26 04:55:25.000000 ChatLLM-2023.5.4.10.18.17/README.bak.md
+-rw-r--r--   0 betterme   (501) staff       (20)     4907 2023-04-28 07:55:35.000000 ChatLLM-2023.5.4.10.18.17/README.md
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 02:18:17.806254 ChatLLM-2023.5.4.10.18.17/chatllm/
+-rw-r--r--   0 betterme   (501) staff       (20)      199 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.10.18.17/chatllm/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 02:18:17.807337 ChatLLM-2023.5.4.10.18.17/chatllm/_his/
+-rw-r--r--   0 betterme   (501) staff       (20)     1482 2023-04-20 12:23:09.000000 ChatLLM-2023.5.4.10.18.17/chatllm/_his/FaissANN.py
+-rw-r--r--   0 betterme   (501) staff       (20)      286 2023-04-27 10:06:48.000000 ChatLLM-2023.5.4.10.18.17/chatllm/_his/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1812 2023-04-25 08:31:06.000000 ChatLLM-2023.5.4.10.18.17/chatllm/_his/_chatllm.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2493 2023-04-27 10:06:48.000000 ChatLLM-2023.5.4.10.18.17/chatllm/_his/_qa.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 02:18:17.807748 ChatLLM-2023.5.4.10.18.17/chatllm/api/
+-rw-r--r--   0 betterme   (501) staff       (20)      270 2023-04-28 01:04:39.000000 ChatLLM-2023.5.4.10.18.17/chatllm/api/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1827 2023-04-28 02:36:43.000000 ChatLLM-2023.5.4.10.18.17/chatllm/api/stream_api.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 02:18:17.809885 ChatLLM-2023.5.4.10.18.17/chatllm/applications/
+-rw-r--r--   0 betterme   (501) staff       (20)     3532 2023-04-25 01:19:43.000000 ChatLLM-2023.5.4.10.18.17/chatllm/applications/Question2Answer.py
+-rw-r--r--   0 betterme   (501) staff       (20)      294 2023-04-25 08:32:56.000000 ChatLLM-2023.5.4.10.18.17/chatllm/applications/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2805 2023-04-27 04:33:02.000000 ChatLLM-2023.5.4.10.18.17/chatllm/applications/chatann.py
+-rw-r--r--   0 betterme   (501) staff       (20)      267 2023-05-04 01:43:23.000000 ChatLLM-2023.5.4.10.18.17/chatllm/applications/chataudio.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3458 2023-05-04 02:16:53.000000 ChatLLM-2023.5.4.10.18.17/chatllm/applications/chatbase.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1176 2023-04-26 01:00:01.000000 ChatLLM-2023.5.4.10.18.17/chatllm/applications/chatcrawler.py
+-rw-r--r--   0 betterme   (501) staff       (20)      266 2023-04-25 01:23:41.000000 ChatLLM-2023.5.4.10.18.17/chatllm/applications/chatdoc.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1357 2023-04-28 07:16:03.000000 ChatLLM-2023.5.4.10.18.17/chatllm/applications/chatpdf.py
+-rw-r--r--   0 betterme   (501) staff       (20)      269 2023-04-26 00:59:00.000000 ChatLLM-2023.5.4.10.18.17/chatllm/applications/chatsearch.py
+-rw-r--r--   0 betterme   (501) staff       (20)      266 2023-04-25 01:23:41.000000 ChatLLM-2023.5.4.10.18.17/chatllm/applications/chatweb.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1895 2023-04-27 02:58:56.000000 ChatLLM-2023.5.4.10.18.17/chatllm/applications/chatwhoosh.py
+-rw-r--r--   0 betterme   (501) staff       (20)      286 2023-04-21 05:42:37.000000 ChatLLM-2023.5.4.10.18.17/chatllm/applications/pipeline.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1964 2023-04-27 09:24:25.000000 ChatLLM-2023.5.4.10.18.17/chatllm/chatyuan.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 02:18:17.810496 ChatLLM-2023.5.4.10.18.17/chatllm/clis/
+-rw-r--r--   0 betterme   (501) staff       (20)      413 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.10.18.17/chatllm/clis/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)      279 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.10.18.17/chatllm/clis/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1334 2023-04-28 07:03:35.000000 ChatLLM-2023.5.4.10.18.17/chatllm/clis/cli.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1439 2023-04-27 01:39:42.000000 ChatLLM-2023.5.4.10.18.17/chatllm/embedding.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 02:18:17.811067 ChatLLM-2023.5.4.10.18.17/chatllm/parse_utils/
+-rw-r--r--   0 betterme   (501) staff       (20)      302 2023-04-25 01:22:30.000000 ChatLLM-2023.5.4.10.18.17/chatllm/parse_utils/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      273 2023-04-21 04:20:09.000000 ChatLLM-2023.5.4.10.18.17/chatllm/parse_utils/doc_parse.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 02:18:17.811958 ChatLLM-2023.5.4.10.18.17/chatllm/utils/
+-rw-r--r--   0 betterme   (501) staff       (20)      278 2023-04-28 04:20:30.000000 ChatLLM-2023.5.4.10.18.17/chatllm/utils/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      271 2023-04-28 04:37:16.000000 ChatLLM-2023.5.4.10.18.17/chatllm/utils/_textsplitter.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2176 2023-05-04 01:37:09.000000 ChatLLM-2023.5.4.10.18.17/chatllm/utils/common.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3208 2023-04-28 04:38:58.000000 ChatLLM-2023.5.4.10.18.17/chatllm/utils/gpu_utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 02:18:17.813403 ChatLLM-2023.5.4.10.18.17/chatllm/webui/
+-rw-r--r--   0 betterme   (501) staff       (20)      270 2023-04-20 02:48:59.000000 ChatLLM-2023.5.4.10.18.17/chatllm/webui/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1488 2023-04-26 01:00:01.000000 ChatLLM-2023.5.4.10.18.17/chatllm/webui/chatbase.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3017 2023-04-28 06:43:45.000000 ChatLLM-2023.5.4.10.18.17/chatllm/webui/chatpdf.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4311 2023-04-26 01:00:01.000000 ChatLLM-2023.5.4.10.18.17/chatllm/webui/gradio_ui.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1819 2023-04-25 03:04:12.000000 ChatLLM-2023.5.4.10.18.17/chatllm/webui/nice_ui.py
+-rw-r--r--   0 betterme   (501) staff       (20)      220 2023-04-26 07:34:11.000000 ChatLLM-2023.5.4.10.18.17/chatllm/webui/run.sh
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 02:18:17.817349 ChatLLM-2023.5.4.10.18.17/data/
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 02:18:17.823607 ChatLLM-2023.5.4.10.18.17/data/imgs/
+-rw-r--r--   0 betterme   (501) staff       (20)   206137 2023-04-26 05:39:20.000000 ChatLLM-2023.5.4.10.18.17/data/imgs/LLM.drawio.png
+-rw-r--r--   0 betterme   (501) staff       (20)   206363 2023-04-26 05:33:47.000000 ChatLLM-2023.5.4.10.18.17/data/imgs/LLM.png
+-rw-r--r--   0 betterme   (501) staff       (20)  1230065 2023-04-26 08:27:23.000000 ChatLLM-2023.5.4.10.18.17/data/imgs/chatpdf.gif
+-rw-r--r--   0 betterme   (501) staff       (20)    45633 2023-04-26 04:24:13.000000 ChatLLM-2023.5.4.10.18.17/data/imgs/chatpdf_ann_df.png
+-rw-r--r--   0 betterme   (501) staff       (20)    29400 2023-04-27 10:24:48.000000 ChatLLM-2023.5.4.10.18.17/data/imgs/role.png
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 02:18:17.828740 ChatLLM-2023.5.4.10.18.17/data/医/
+-rw-r--r--   0 betterme   (501) staff       (20)  3891700 2023-04-20 11:48:19.000000 ChatLLM-2023.5.4.10.18.17/data/医/500种中药现代研究.txt
+-rw-r--r--   0 betterme   (501) staff       (20)  4926489 2023-04-20 11:46:24.000000 ChatLLM-2023.5.4.10.18.17/data/医/古今医统大全.txt
+-rw-r--r--   0 betterme   (501) staff       (20)     1633 2023-04-20 07:17:41.000000 ChatLLM-2023.5.4.10.18.17/data/姚明.txt
+-rw-r--r--   0 betterme   (501) staff       (20)      946 2023-04-20 07:17:41.000000 ChatLLM-2023.5.4.10.18.17/data/王治郅.txt
+-rw-r--r--   0 betterme   (501) staff       (20)     1291 2023-04-20 07:17:41.000000 ChatLLM-2023.5.4.10.18.17/data/科比.txt
+-rw-r--r--   0 betterme   (501) staff       (20)  3051914 2023-04-25 02:58:13.000000 ChatLLM-2023.5.4.10.18.17/data/财报.pdf
+-rw-r--r--   0 betterme   (501) staff       (20)      493 2023-04-20 07:17:41.000000 ChatLLM-2023.5.4.10.18.17/data/马保国.txt
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 02:18:17.844447 ChatLLM-2023.5.4.10.18.17/docs/
+-rw-r--r--   0 betterme   (501) staff       (20)      564 2023-04-26 04:55:25.000000 ChatLLM-2023.5.4.10.18.17/docs/INSTALL.md
+-rw-r--r--   0 betterme   (501) staff       (20)      608 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.10.18.17/docs/Makefile
+-rw-r--r--   0 betterme   (501) staff       (20)     4846 2023-04-27 11:05:23.000000 ChatLLM-2023.5.4.10.18.17/docs/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)       26 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.10.18.17/docs/_config.yml
+-rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.10.18.17/docs/authors.rst
+-rwxr-xr-x   0 betterme   (501) staff       (20)     4763 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.10.18.17/docs/conf.py
+-rw-r--r--   0 betterme   (501) staff       (20)       33 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.10.18.17/docs/contributing.rst
+-rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.10.18.17/docs/history.rst
+-rw-r--r--   0 betterme   (501) staff       (20)      304 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.10.18.17/docs/index.rst
+-rw-r--r--   0 betterme   (501) staff       (20)      805 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.10.18.17/docs/make.bat
+-rw-r--r--   0 betterme   (501) staff       (20)       27 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.10.18.17/docs/readme.rst
+-rw-r--r--   0 betterme   (501) staff       (20)       69 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.10.18.17/docs/usage.rst
+-rwxr-xr-x   0 betterme   (501) staff       (20)      269 2023-04-28 07:55:35.000000 ChatLLM-2023.5.4.10.18.17/git_init.sh
+-rwxr-xr-x   0 betterme   (501) staff       (20)      152 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.10.18.17/pypi.sh
+-rw-r--r--   0 betterme   (501) staff       (20)       78 2023-04-28 08:43:50.000000 ChatLLM-2023.5.4.10.18.17/requirements.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       14 2023-04-28 08:44:21.000000 ChatLLM-2023.5.4.10.18.17/requirements_api.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       25 2023-04-28 08:44:53.000000 ChatLLM-2023.5.4.10.18.17/requirements_pdf.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       10 2023-04-28 08:44:32.000000 ChatLLM-2023.5.4.10.18.17/requirements_streamlit.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       38 2023-05-04 02:18:17.847143 ChatLLM-2023.5.4.10.18.17/setup.cfg
+-rw-r--r--   0 betterme   (501) staff       (20)     1897 2023-04-28 08:42:35.000000 ChatLLM-2023.5.4.10.18.17/setup.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 02:18:17.845031 ChatLLM-2023.5.4.10.18.17/tests/
+-rw-r--r--   0 betterme   (501) staff       (20)       37 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.10.18.17/tests/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      852 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.10.18.17/tests/test_llm4gpt.py
+-rw-r--r--   0 betterme   (501) staff       (20)    51173 2023-04-21 11:31:44.000000 ChatLLM-2023.5.4.10.18.17/tests/内存型.ipynb
+-rw-r--r--   0 betterme   (501) staff       (20)      288 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.10.18.17/tox.ini
```

### Comparing `ChatLLM-2023.4.28.16.44.34/.gitignore` & `ChatLLM-2023.5.4.10.18.17/.gitignore`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.16.44.34/.travis.yml` & `ChatLLM-2023.5.4.10.18.17/.travis.yml`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.16.44.34/CONTRIBUTING.rst` & `ChatLLM-2023.5.4.10.18.17/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.16.44.34/ChatLLM.egg-info/PKG-INFO` & `ChatLLM-2023.5.4.10.18.17/ChatLLM.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ChatLLM
-Version: 2023.4.28.16.44.34
+Version: 2023.5.4.10.18.17
 Summary: Create a Python package.
 Home-page: https://github.com/yuanjie-ai/ChatLLM
 Author: yuanjie
 Author-email: 313303303@qq.com
 License: MIT license
 Keywords: chatllm
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `ChatLLM-2023.4.28.16.44.34/ChatLLM.egg-info/SOURCES.txt` & `ChatLLM-2023.5.4.10.18.17/ChatLLM.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 chatllm/_his/_chatllm.py
 chatllm/_his/_qa.py
 chatllm/api/__init__.py
 chatllm/api/stream_api.py
 chatllm/applications/Question2Answer.py
 chatllm/applications/__init__.py
 chatllm/applications/chatann.py
+chatllm/applications/chataudio.py
 chatllm/applications/chatbase.py
 chatllm/applications/chatcrawler.py
 chatllm/applications/chatdoc.py
 chatllm/applications/chatpdf.py
 chatllm/applications/chatsearch.py
 chatllm/applications/chatweb.py
 chatllm/applications/chatwhoosh.py
```

### Comparing `ChatLLM-2023.4.28.16.44.34/LICENSE` & `ChatLLM-2023.5.4.10.18.17/LICENSE`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.16.44.34/Makefile` & `ChatLLM-2023.5.4.10.18.17/Makefile`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.16.44.34/PKG-INFO` & `ChatLLM-2023.5.4.10.18.17/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ChatLLM
-Version: 2023.4.28.16.44.34
+Version: 2023.5.4.10.18.17
 Summary: Create a Python package.
 Home-page: https://github.com/yuanjie-ai/ChatLLM
 Author: yuanjie
 Author-email: 313303303@qq.com
 License: MIT license
 Keywords: chatllm
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `ChatLLM-2023.4.28.16.44.34/README.md` & `ChatLLM-2023.5.4.10.18.17/README.md`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.16.44.34/chatllm/_his/FaissANN.py` & `ChatLLM-2023.5.4.10.18.17/chatllm/_his/FaissANN.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.16.44.34/chatllm/_his/_chatllm.py` & `ChatLLM-2023.5.4.10.18.17/chatllm/_his/_chatllm.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.16.44.34/chatllm/_his/_qa.py` & `ChatLLM-2023.5.4.10.18.17/chatllm/_his/_qa.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.16.44.34/chatllm/api/stream_api.py` & `ChatLLM-2023.5.4.10.18.17/chatllm/api/stream_api.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.16.44.34/chatllm/applications/Question2Answer.py` & `ChatLLM-2023.5.4.10.18.17/chatllm/applications/Question2Answer.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.16.44.34/chatllm/applications/chatann.py` & `ChatLLM-2023.5.4.10.18.17/chatllm/applications/chatann.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.16.44.34/chatllm/applications/chatbase.py` & `ChatLLM-2023.5.4.10.18.17/chatllm/applications/chatbase.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,14 +19,17 @@
     def __init__(self, chat_func=None):
         self.chat_func = chat_func
         #
         self.history = []
         self.knowledge_base = None
         self.role = None
 
+        # 重写 chat函数会更好 prompt += "[Round {}]\n问：{}\n答：{}\n".format(i, old_query, response) # 根据角色配置模板
+        self.prompt_template = os.environ.get('PROMPT_TEMPLATE', '{role}')
+
     def __call__(self, **kwargs):
         return self.qa(**kwargs)
 
     def qa(self, query, knowledge_base='', **kwargs):
         """重写"""
         return self._qa(query, knowledge_base, **kwargs)
 
@@ -59,26 +62,14 @@
             yield response, history
         # self.history_ = history  # 历史所有
         self.history += [[None, response]]  # 置空知识
 
     def load_llm4chat(self, model_name_or_path="THUDM/chatglm-6b", device=DEVICE, stream=True, **kwargs):
         self.chat_func = load_llm4chat(model_name_or_path, device, stream, **kwargs)
 
-    @property
-    def prompt_template(self):
-        # 重写 chat函数会更好 prompt += "[Round {}]\n问：{}\n答：{}\n".format(i, old_query, response)
-        # 根据角色配置模板
-        return """
-            {role}
-            基于以下已知信息，简洁和专业的来回答问题。
-            如果无法从中得到答案，请说 "根据已知信息无法回答该问题" 或 "没有提供足够的信息"，不允许在答案中添加编造成分，答案请使用中文。
-            已知信息: {context}
-            问题: {question}
-            """.strip()
-
     def run_serving(self, host='127.0.0.1', port=8000, path='/'):
         from flask import Flask, Response, jsonify, request
 
         app = Flask(__name__)
 
         def gen(**input):
             for response, _ in self.qa(**input):
```

### Comparing `ChatLLM-2023.4.28.16.44.34/chatllm/applications/chatcrawler.py` & `ChatLLM-2023.5.4.10.18.17/chatllm/applications/chatcrawler.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.16.44.34/chatllm/applications/chatpdf.py` & `ChatLLM-2023.5.4.10.18.17/chatllm/applications/chatpdf.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.16.44.34/chatllm/applications/chatwhoosh.py` & `ChatLLM-2023.5.4.10.18.17/chatllm/applications/chatwhoosh.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.16.44.34/chatllm/chatyuan.py` & `ChatLLM-2023.5.4.10.18.17/chatllm/chatyuan.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.16.44.34/chatllm/clis/cli.py` & `ChatLLM-2023.5.4.10.18.17/chatllm/clis/cli.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.16.44.34/chatllm/embedding.py` & `ChatLLM-2023.5.4.10.18.17/chatllm/embedding.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.16.44.34/chatllm/utils/common.py` & `ChatLLM-2023.5.4.10.18.17/chatllm/utils/common.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,18 +10,18 @@
 import torch
 from transformers import AutoTokenizer, AutoModel
 
 from meutils.pipe import *
 from chatllm.utils.gpu_utils import load_chatglm_on_gpus
 
 DEVICE = (
-    os.environ['DEVICE']
-    if 'DEVICE' in os.environ else "cuda"
-    if torch.cuda.is_available() else "mps"
-    if torch.backends.mps.is_available() else "cpu"
+    os.environ['DEVICE'] if 'DEVICE' in os.environ
+    else "cuda" if torch.cuda.is_available()
+    else "mps" if torch.backends.mps.is_available()
+    else "cpu"
 )
 if LOCAL_HOST.startswith('10.219'):
     MODEL_PATH = "/Users/betterme/PycharmProjects/AI/CHAT_MODEL/chatglm"
 
 
 # todo 多卡 https://github.com/THUDM/ChatGLM-6B#%E5%A4%9A%E5%8D%A1%E9%83%A8%E7%BD%B2
 
@@ -47,14 +47,14 @@
 
     return model.eval(), tokenizer
 
 
 def load_llm4chat(model_name_or_path="THUDM/chatglm-6b", device=DEVICE, num_gpus=1, stream=True, **kwargs):
     model, tokenizer = load_llm(model_name_or_path, device, num_gpus, **kwargs)
     if stream and hasattr(model, 'stream_chat'):
-        return partial(model.stream_chat, tokenizer=tokenizer)
+        return partial(model.stream_chat, tokenizer=tokenizer)  # 可以在每一次生成清GPU
     else:
         return partial(model.chat, tokenizer=tokenizer)
 
 
 if __name__ == '__main__':
     model, tokenizer = load_llm("/CHAT_MODEL/chatglm", device='cpu')
```

### Comparing `ChatLLM-2023.4.28.16.44.34/chatllm/utils/gpu_utils.py` & `ChatLLM-2023.5.4.10.18.17/chatllm/utils/gpu_utils.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.16.44.34/chatllm/webui/chatbase.py` & `ChatLLM-2023.5.4.10.18.17/chatllm/webui/chatbase.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.16.44.34/chatllm/webui/chatpdf.py` & `ChatLLM-2023.5.4.10.18.17/chatllm/webui/chatpdf.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.16.44.34/chatllm/webui/gradio_ui.py` & `ChatLLM-2023.5.4.10.18.17/chatllm/webui/gradio_ui.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.16.44.34/chatllm/webui/nice_ui.py` & `ChatLLM-2023.5.4.10.18.17/chatllm/webui/nice_ui.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.16.44.34/data/imgs/LLM.drawio.png` & `ChatLLM-2023.5.4.10.18.17/data/imgs/LLM.drawio.png`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.16.44.34/data/imgs/LLM.png` & `ChatLLM-2023.5.4.10.18.17/data/imgs/LLM.png`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.16.44.34/data/imgs/chatpdf.gif` & `ChatLLM-2023.5.4.10.18.17/data/imgs/chatpdf.gif`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.16.44.34/data/imgs/chatpdf_ann_df.png` & `ChatLLM-2023.5.4.10.18.17/data/imgs/chatpdf_ann_df.png`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.16.44.34/data/imgs/role.png` & `ChatLLM-2023.5.4.10.18.17/data/imgs/role.png`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.16.44.34/data/医/500种中药现代研究.txt` & `ChatLLM-2023.5.4.10.18.17/data/医/500种中药现代研究.txt`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.16.44.34/data/医/古今医统大全.txt` & `ChatLLM-2023.5.4.10.18.17/data/医/古今医统大全.txt`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.16.44.34/data/姚明.txt` & `ChatLLM-2023.5.4.10.18.17/data/姚明.txt`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.16.44.34/data/王治郅.txt` & `ChatLLM-2023.5.4.10.18.17/data/王治郅.txt`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.16.44.34/data/科比.txt` & `ChatLLM-2023.5.4.10.18.17/data/科比.txt`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.16.44.34/data/财报.pdf` & `ChatLLM-2023.5.4.10.18.17/data/财报.pdf`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.16.44.34/docs/INSTALL.md` & `ChatLLM-2023.5.4.10.18.17/docs/INSTALL.md`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.16.44.34/docs/Makefile` & `ChatLLM-2023.5.4.10.18.17/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.16.44.34/docs/README.md` & `ChatLLM-2023.5.4.10.18.17/docs/README.md`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.16.44.34/docs/conf.py` & `ChatLLM-2023.5.4.10.18.17/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.16.44.34/docs/make.bat` & `ChatLLM-2023.5.4.10.18.17/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.16.44.34/setup.py` & `ChatLLM-2023.5.4.10.18.17/setup.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.16.44.34/tests/test_llm4gpt.py` & `ChatLLM-2023.5.4.10.18.17/tests/test_llm4gpt.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.4.28.16.44.34/tests/内存型.ipynb` & `ChatLLM-2023.5.4.10.18.17/tests/内存型.ipynb`

 * *Files identical despite different names*

