# Comparing `tmp/ChatLLM-2023.5.4.10.47.32.tar.gz` & `tmp/ChatLLM-2023.5.4.10.54.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ChatLLM-2023.5.4.10.47.32.tar", last modified: Thu May  4 02:47:33 2023, max compression
+gzip compressed data, was "ChatLLM-2023.5.4.10.54.16.tar", last modified: Thu May  4 02:54:17 2023, max compression
```

## Comparing `ChatLLM-2023.5.4.10.47.32.tar` & `ChatLLM-2023.5.4.10.54.16.tar`

### file list

```diff
@@ -1,106 +1,106 @@
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 02:47:33.114286 ChatLLM-2023.5.4.10.47.32/
--rw-r--r--   0 betterme   (501) staff       (20)      292 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.10.47.32/.editorconfig
--rw-r--r--   0 betterme   (501) staff       (20)     1196 2023-04-20 11:38:14.000000 ChatLLM-2023.5.4.10.47.32/.gitignore
--rw-r--r--   0 betterme   (501) staff       (20)      697 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.10.47.32/.travis.yml
--rw-r--r--   0 betterme   (501) staff       (20)      149 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.10.47.32/AUTHORS.rst
--rw-r--r--   0 betterme   (501) staff       (20)     3530 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.10.47.32/CONTRIBUTING.rst
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 02:47:33.072131 ChatLLM-2023.5.4.10.47.32/ChatLLM.egg-info/
--rw-r--r--   0 betterme   (501) staff       (20)     5809 2023-05-04 02:47:32.000000 ChatLLM-2023.5.4.10.47.32/ChatLLM.egg-info/PKG-INFO
--rw-r--r--   0 betterme   (501) staff       (20)     1997 2023-05-04 02:47:32.000000 ChatLLM-2023.5.4.10.47.32/ChatLLM.egg-info/SOURCES.txt
--rw-r--r--   0 betterme   (501) staff       (20)        1 2023-05-04 02:47:32.000000 ChatLLM-2023.5.4.10.47.32/ChatLLM.egg-info/dependency_links.txt
--rw-r--r--   0 betterme   (501) staff       (20)       53 2023-05-04 02:47:32.000000 ChatLLM-2023.5.4.10.47.32/ChatLLM.egg-info/entry_points.txt
--rw-r--r--   0 betterme   (501) staff       (20)        1 2023-05-04 02:47:32.000000 ChatLLM-2023.5.4.10.47.32/ChatLLM.egg-info/not-zip-safe
--rw-r--r--   0 betterme   (501) staff       (20)      186 2023-05-04 02:47:32.000000 ChatLLM-2023.5.4.10.47.32/ChatLLM.egg-info/requires.txt
--rw-r--r--   0 betterme   (501) staff       (20)        8 2023-05-04 02:47:32.000000 ChatLLM-2023.5.4.10.47.32/ChatLLM.egg-info/top_level.txt
--rw-r--r--   0 betterme   (501) staff       (20)       89 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.10.47.32/HISTORY.rst
--rw-r--r--   0 betterme   (501) staff       (20)     1066 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.10.47.32/LICENSE
--rw-r--r--   0 betterme   (501) staff       (20)      289 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.10.47.32/MANIFEST.in
--rw-r--r--   0 betterme   (501) staff       (20)     2215 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.10.47.32/Makefile
--rw-r--r--   0 betterme   (501) staff       (20)     5809 2023-05-04 02:47:33.114134 ChatLLM-2023.5.4.10.47.32/PKG-INFO
--rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-26 04:55:25.000000 ChatLLM-2023.5.4.10.47.32/README.bak.md
--rw-r--r--   0 betterme   (501) staff       (20)     4907 2023-04-28 07:55:35.000000 ChatLLM-2023.5.4.10.47.32/README.md
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 02:47:33.072745 ChatLLM-2023.5.4.10.47.32/chatllm/
--rw-r--r--   0 betterme   (501) staff       (20)      199 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.10.47.32/chatllm/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 02:47:33.073961 ChatLLM-2023.5.4.10.47.32/chatllm/_his/
--rw-r--r--   0 betterme   (501) staff       (20)     1482 2023-04-20 12:23:09.000000 ChatLLM-2023.5.4.10.47.32/chatllm/_his/FaissANN.py
--rw-r--r--   0 betterme   (501) staff       (20)      286 2023-04-27 10:06:48.000000 ChatLLM-2023.5.4.10.47.32/chatllm/_his/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1812 2023-04-25 08:31:06.000000 ChatLLM-2023.5.4.10.47.32/chatllm/_his/_chatllm.py
--rw-r--r--   0 betterme   (501) staff       (20)     2493 2023-04-27 10:06:48.000000 ChatLLM-2023.5.4.10.47.32/chatllm/_his/_qa.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 02:47:33.074404 ChatLLM-2023.5.4.10.47.32/chatllm/api/
--rw-r--r--   0 betterme   (501) staff       (20)      270 2023-04-28 01:04:39.000000 ChatLLM-2023.5.4.10.47.32/chatllm/api/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1827 2023-04-28 02:36:43.000000 ChatLLM-2023.5.4.10.47.32/chatllm/api/stream_api.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 02:47:33.077507 ChatLLM-2023.5.4.10.47.32/chatllm/applications/
--rw-r--r--   0 betterme   (501) staff       (20)     3532 2023-04-25 01:19:43.000000 ChatLLM-2023.5.4.10.47.32/chatllm/applications/Question2Answer.py
--rw-r--r--   0 betterme   (501) staff       (20)      294 2023-04-25 08:32:56.000000 ChatLLM-2023.5.4.10.47.32/chatllm/applications/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2805 2023-04-27 04:33:02.000000 ChatLLM-2023.5.4.10.47.32/chatllm/applications/chatann.py
--rw-r--r--   0 betterme   (501) staff       (20)      267 2023-05-04 01:43:23.000000 ChatLLM-2023.5.4.10.47.32/chatllm/applications/chataudio.py
--rw-r--r--   0 betterme   (501) staff       (20)     3446 2023-05-04 02:44:32.000000 ChatLLM-2023.5.4.10.47.32/chatllm/applications/chatbase.py
--rw-r--r--   0 betterme   (501) staff       (20)     1176 2023-04-26 01:00:01.000000 ChatLLM-2023.5.4.10.47.32/chatllm/applications/chatcrawler.py
--rw-r--r--   0 betterme   (501) staff       (20)      266 2023-04-25 01:23:41.000000 ChatLLM-2023.5.4.10.47.32/chatllm/applications/chatdoc.py
--rw-r--r--   0 betterme   (501) staff       (20)     1357 2023-04-28 07:16:03.000000 ChatLLM-2023.5.4.10.47.32/chatllm/applications/chatpdf.py
--rw-r--r--   0 betterme   (501) staff       (20)      269 2023-04-26 00:59:00.000000 ChatLLM-2023.5.4.10.47.32/chatllm/applications/chatsearch.py
--rw-r--r--   0 betterme   (501) staff       (20)      266 2023-04-25 01:23:41.000000 ChatLLM-2023.5.4.10.47.32/chatllm/applications/chatweb.py
--rw-r--r--   0 betterme   (501) staff       (20)     1895 2023-04-27 02:58:56.000000 ChatLLM-2023.5.4.10.47.32/chatllm/applications/chatwhoosh.py
--rw-r--r--   0 betterme   (501) staff       (20)      286 2023-04-21 05:42:37.000000 ChatLLM-2023.5.4.10.47.32/chatllm/applications/pipeline.py
--rw-r--r--   0 betterme   (501) staff       (20)     1964 2023-04-27 09:24:25.000000 ChatLLM-2023.5.4.10.47.32/chatllm/chatyuan.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 02:47:33.078188 ChatLLM-2023.5.4.10.47.32/chatllm/clis/
--rw-r--r--   0 betterme   (501) staff       (20)      413 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.10.47.32/chatllm/clis/README.md
--rw-r--r--   0 betterme   (501) staff       (20)      279 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.10.47.32/chatllm/clis/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1334 2023-04-28 07:03:35.000000 ChatLLM-2023.5.4.10.47.32/chatllm/clis/cli.py
--rw-r--r--   0 betterme   (501) staff       (20)     1439 2023-04-27 01:39:42.000000 ChatLLM-2023.5.4.10.47.32/chatllm/embedding.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 02:47:33.078859 ChatLLM-2023.5.4.10.47.32/chatllm/parse_utils/
--rw-r--r--   0 betterme   (501) staff       (20)      302 2023-04-25 01:22:30.000000 ChatLLM-2023.5.4.10.47.32/chatllm/parse_utils/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      273 2023-04-21 04:20:09.000000 ChatLLM-2023.5.4.10.47.32/chatllm/parse_utils/doc_parse.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 02:47:33.079948 ChatLLM-2023.5.4.10.47.32/chatllm/utils/
--rw-r--r--   0 betterme   (501) staff       (20)      278 2023-04-28 04:20:30.000000 ChatLLM-2023.5.4.10.47.32/chatllm/utils/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      271 2023-04-28 04:37:16.000000 ChatLLM-2023.5.4.10.47.32/chatllm/utils/_textsplitter.py
--rw-r--r--   0 betterme   (501) staff       (20)     2176 2023-05-04 01:37:09.000000 ChatLLM-2023.5.4.10.47.32/chatllm/utils/common.py
--rw-r--r--   0 betterme   (501) staff       (20)     3208 2023-04-28 04:38:58.000000 ChatLLM-2023.5.4.10.47.32/chatllm/utils/gpu_utils.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 02:47:33.081800 ChatLLM-2023.5.4.10.47.32/chatllm/webui/
--rw-r--r--   0 betterme   (501) staff       (20)      270 2023-04-20 02:48:59.000000 ChatLLM-2023.5.4.10.47.32/chatllm/webui/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1488 2023-04-26 01:00:01.000000 ChatLLM-2023.5.4.10.47.32/chatllm/webui/chatbase.py
--rw-r--r--   0 betterme   (501) staff       (20)     3017 2023-04-28 06:43:45.000000 ChatLLM-2023.5.4.10.47.32/chatllm/webui/chatpdf.py
--rw-r--r--   0 betterme   (501) staff       (20)     4311 2023-04-26 01:00:01.000000 ChatLLM-2023.5.4.10.47.32/chatllm/webui/gradio_ui.py
--rw-r--r--   0 betterme   (501) staff       (20)     1819 2023-04-25 03:04:12.000000 ChatLLM-2023.5.4.10.47.32/chatllm/webui/nice_ui.py
--rw-r--r--   0 betterme   (501) staff       (20)      220 2023-04-26 07:34:11.000000 ChatLLM-2023.5.4.10.47.32/chatllm/webui/run.sh
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 02:47:33.085860 ChatLLM-2023.5.4.10.47.32/data/
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 02:47:33.094142 ChatLLM-2023.5.4.10.47.32/data/imgs/
--rw-r--r--   0 betterme   (501) staff       (20)   206137 2023-04-26 05:39:20.000000 ChatLLM-2023.5.4.10.47.32/data/imgs/LLM.drawio.png
--rw-r--r--   0 betterme   (501) staff       (20)   206363 2023-04-26 05:33:47.000000 ChatLLM-2023.5.4.10.47.32/data/imgs/LLM.png
--rw-r--r--   0 betterme   (501) staff       (20)  1230065 2023-04-26 08:27:23.000000 ChatLLM-2023.5.4.10.47.32/data/imgs/chatpdf.gif
--rw-r--r--   0 betterme   (501) staff       (20)    45633 2023-04-26 04:24:13.000000 ChatLLM-2023.5.4.10.47.32/data/imgs/chatpdf_ann_df.png
--rw-r--r--   0 betterme   (501) staff       (20)    29400 2023-04-27 10:24:48.000000 ChatLLM-2023.5.4.10.47.32/data/imgs/role.png
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 02:47:33.098075 ChatLLM-2023.5.4.10.47.32/data/医/
--rw-r--r--   0 betterme   (501) staff       (20)  3891700 2023-04-20 11:48:19.000000 ChatLLM-2023.5.4.10.47.32/data/医/500种中药现代研究.txt
--rw-r--r--   0 betterme   (501) staff       (20)  4926489 2023-04-20 11:46:24.000000 ChatLLM-2023.5.4.10.47.32/data/医/古今医统大全.txt
--rw-r--r--   0 betterme   (501) staff       (20)     1633 2023-04-20 07:17:41.000000 ChatLLM-2023.5.4.10.47.32/data/姚明.txt
--rw-r--r--   0 betterme   (501) staff       (20)      946 2023-04-20 07:17:41.000000 ChatLLM-2023.5.4.10.47.32/data/王治郅.txt
--rw-r--r--   0 betterme   (501) staff       (20)     1291 2023-04-20 07:17:41.000000 ChatLLM-2023.5.4.10.47.32/data/科比.txt
--rw-r--r--   0 betterme   (501) staff       (20)  3051914 2023-04-25 02:58:13.000000 ChatLLM-2023.5.4.10.47.32/data/财报.pdf
--rw-r--r--   0 betterme   (501) staff       (20)      493 2023-04-20 07:17:41.000000 ChatLLM-2023.5.4.10.47.32/data/马保国.txt
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 02:47:33.111713 ChatLLM-2023.5.4.10.47.32/docs/
--rw-r--r--   0 betterme   (501) staff       (20)      564 2023-04-26 04:55:25.000000 ChatLLM-2023.5.4.10.47.32/docs/INSTALL.md
--rw-r--r--   0 betterme   (501) staff       (20)      608 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.10.47.32/docs/Makefile
--rw-r--r--   0 betterme   (501) staff       (20)     4846 2023-04-27 11:05:23.000000 ChatLLM-2023.5.4.10.47.32/docs/README.md
--rw-r--r--   0 betterme   (501) staff       (20)       26 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.10.47.32/docs/_config.yml
--rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.10.47.32/docs/authors.rst
--rwxr-xr-x   0 betterme   (501) staff       (20)     4763 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.10.47.32/docs/conf.py
--rw-r--r--   0 betterme   (501) staff       (20)       33 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.10.47.32/docs/contributing.rst
--rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.10.47.32/docs/history.rst
--rw-r--r--   0 betterme   (501) staff       (20)      304 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.10.47.32/docs/index.rst
--rw-r--r--   0 betterme   (501) staff       (20)      805 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.10.47.32/docs/make.bat
--rw-r--r--   0 betterme   (501) staff       (20)       27 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.10.47.32/docs/readme.rst
--rw-r--r--   0 betterme   (501) staff       (20)       69 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.10.47.32/docs/usage.rst
--rwxr-xr-x   0 betterme   (501) staff       (20)      269 2023-04-28 07:55:35.000000 ChatLLM-2023.5.4.10.47.32/git_init.sh
--rwxr-xr-x   0 betterme   (501) staff       (20)      152 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.10.47.32/pypi.sh
--rw-r--r--   0 betterme   (501) staff       (20)       78 2023-04-28 08:43:50.000000 ChatLLM-2023.5.4.10.47.32/requirements.txt
--rw-r--r--   0 betterme   (501) staff       (20)       14 2023-04-28 08:44:21.000000 ChatLLM-2023.5.4.10.47.32/requirements_api.txt
--rw-r--r--   0 betterme   (501) staff       (20)       25 2023-04-28 08:44:53.000000 ChatLLM-2023.5.4.10.47.32/requirements_pdf.txt
--rw-r--r--   0 betterme   (501) staff       (20)       10 2023-04-28 08:44:32.000000 ChatLLM-2023.5.4.10.47.32/requirements_streamlit.txt
--rw-r--r--   0 betterme   (501) staff       (20)       38 2023-05-04 02:47:33.114331 ChatLLM-2023.5.4.10.47.32/setup.cfg
--rw-r--r--   0 betterme   (501) staff       (20)     1897 2023-04-28 08:42:35.000000 ChatLLM-2023.5.4.10.47.32/setup.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 02:47:33.112195 ChatLLM-2023.5.4.10.47.32/tests/
--rw-r--r--   0 betterme   (501) staff       (20)       37 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.10.47.32/tests/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      852 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.10.47.32/tests/test_llm4gpt.py
--rw-r--r--   0 betterme   (501) staff       (20)    51173 2023-04-21 11:31:44.000000 ChatLLM-2023.5.4.10.47.32/tests/内存型.ipynb
--rw-r--r--   0 betterme   (501) staff       (20)      288 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.10.47.32/tox.ini
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 02:54:17.211509 ChatLLM-2023.5.4.10.54.16/
+-rw-r--r--   0 betterme   (501) staff       (20)      292 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.10.54.16/.editorconfig
+-rw-r--r--   0 betterme   (501) staff       (20)     1196 2023-04-20 11:38:14.000000 ChatLLM-2023.5.4.10.54.16/.gitignore
+-rw-r--r--   0 betterme   (501) staff       (20)      697 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.10.54.16/.travis.yml
+-rw-r--r--   0 betterme   (501) staff       (20)      149 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.10.54.16/AUTHORS.rst
+-rw-r--r--   0 betterme   (501) staff       (20)     3530 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.10.54.16/CONTRIBUTING.rst
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 02:54:17.168223 ChatLLM-2023.5.4.10.54.16/ChatLLM.egg-info/
+-rw-r--r--   0 betterme   (501) staff       (20)     5809 2023-05-04 02:54:17.000000 ChatLLM-2023.5.4.10.54.16/ChatLLM.egg-info/PKG-INFO
+-rw-r--r--   0 betterme   (501) staff       (20)     1997 2023-05-04 02:54:17.000000 ChatLLM-2023.5.4.10.54.16/ChatLLM.egg-info/SOURCES.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        1 2023-05-04 02:54:17.000000 ChatLLM-2023.5.4.10.54.16/ChatLLM.egg-info/dependency_links.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       53 2023-05-04 02:54:17.000000 ChatLLM-2023.5.4.10.54.16/ChatLLM.egg-info/entry_points.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        1 2023-05-04 02:54:17.000000 ChatLLM-2023.5.4.10.54.16/ChatLLM.egg-info/not-zip-safe
+-rw-r--r--   0 betterme   (501) staff       (20)      186 2023-05-04 02:54:17.000000 ChatLLM-2023.5.4.10.54.16/ChatLLM.egg-info/requires.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        8 2023-05-04 02:54:17.000000 ChatLLM-2023.5.4.10.54.16/ChatLLM.egg-info/top_level.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       89 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.10.54.16/HISTORY.rst
+-rw-r--r--   0 betterme   (501) staff       (20)     1066 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.10.54.16/LICENSE
+-rw-r--r--   0 betterme   (501) staff       (20)      289 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.10.54.16/MANIFEST.in
+-rw-r--r--   0 betterme   (501) staff       (20)     2215 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.10.54.16/Makefile
+-rw-r--r--   0 betterme   (501) staff       (20)     5809 2023-05-04 02:54:17.211355 ChatLLM-2023.5.4.10.54.16/PKG-INFO
+-rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-26 04:55:25.000000 ChatLLM-2023.5.4.10.54.16/README.bak.md
+-rw-r--r--   0 betterme   (501) staff       (20)     4907 2023-04-28 07:55:35.000000 ChatLLM-2023.5.4.10.54.16/README.md
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 02:54:17.168832 ChatLLM-2023.5.4.10.54.16/chatllm/
+-rw-r--r--   0 betterme   (501) staff       (20)      199 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.10.54.16/chatllm/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 02:54:17.170038 ChatLLM-2023.5.4.10.54.16/chatllm/_his/
+-rw-r--r--   0 betterme   (501) staff       (20)     1482 2023-04-20 12:23:09.000000 ChatLLM-2023.5.4.10.54.16/chatllm/_his/FaissANN.py
+-rw-r--r--   0 betterme   (501) staff       (20)      286 2023-04-27 10:06:48.000000 ChatLLM-2023.5.4.10.54.16/chatllm/_his/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1812 2023-04-25 08:31:06.000000 ChatLLM-2023.5.4.10.54.16/chatllm/_his/_chatllm.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2493 2023-04-27 10:06:48.000000 ChatLLM-2023.5.4.10.54.16/chatllm/_his/_qa.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 02:54:17.170618 ChatLLM-2023.5.4.10.54.16/chatllm/api/
+-rw-r--r--   0 betterme   (501) staff       (20)      270 2023-04-28 01:04:39.000000 ChatLLM-2023.5.4.10.54.16/chatllm/api/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1827 2023-04-28 02:36:43.000000 ChatLLM-2023.5.4.10.54.16/chatllm/api/stream_api.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 02:54:17.173521 ChatLLM-2023.5.4.10.54.16/chatllm/applications/
+-rw-r--r--   0 betterme   (501) staff       (20)     3532 2023-04-25 01:19:43.000000 ChatLLM-2023.5.4.10.54.16/chatllm/applications/Question2Answer.py
+-rw-r--r--   0 betterme   (501) staff       (20)      294 2023-04-25 08:32:56.000000 ChatLLM-2023.5.4.10.54.16/chatllm/applications/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2805 2023-04-27 04:33:02.000000 ChatLLM-2023.5.4.10.54.16/chatllm/applications/chatann.py
+-rw-r--r--   0 betterme   (501) staff       (20)      267 2023-05-04 01:43:23.000000 ChatLLM-2023.5.4.10.54.16/chatllm/applications/chataudio.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3446 2023-05-04 02:44:32.000000 ChatLLM-2023.5.4.10.54.16/chatllm/applications/chatbase.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1176 2023-04-26 01:00:01.000000 ChatLLM-2023.5.4.10.54.16/chatllm/applications/chatcrawler.py
+-rw-r--r--   0 betterme   (501) staff       (20)      266 2023-04-25 01:23:41.000000 ChatLLM-2023.5.4.10.54.16/chatllm/applications/chatdoc.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1357 2023-04-28 07:16:03.000000 ChatLLM-2023.5.4.10.54.16/chatllm/applications/chatpdf.py
+-rw-r--r--   0 betterme   (501) staff       (20)      269 2023-04-26 00:59:00.000000 ChatLLM-2023.5.4.10.54.16/chatllm/applications/chatsearch.py
+-rw-r--r--   0 betterme   (501) staff       (20)      266 2023-04-25 01:23:41.000000 ChatLLM-2023.5.4.10.54.16/chatllm/applications/chatweb.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1895 2023-04-27 02:58:56.000000 ChatLLM-2023.5.4.10.54.16/chatllm/applications/chatwhoosh.py
+-rw-r--r--   0 betterme   (501) staff       (20)      286 2023-04-21 05:42:37.000000 ChatLLM-2023.5.4.10.54.16/chatllm/applications/pipeline.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1964 2023-04-27 09:24:25.000000 ChatLLM-2023.5.4.10.54.16/chatllm/chatyuan.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 02:54:17.174219 ChatLLM-2023.5.4.10.54.16/chatllm/clis/
+-rw-r--r--   0 betterme   (501) staff       (20)      413 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.10.54.16/chatllm/clis/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)      279 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.10.54.16/chatllm/clis/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1334 2023-04-28 07:03:35.000000 ChatLLM-2023.5.4.10.54.16/chatllm/clis/cli.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1439 2023-04-27 01:39:42.000000 ChatLLM-2023.5.4.10.54.16/chatllm/embedding.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 02:54:17.174668 ChatLLM-2023.5.4.10.54.16/chatllm/parse_utils/
+-rw-r--r--   0 betterme   (501) staff       (20)      302 2023-04-25 01:22:30.000000 ChatLLM-2023.5.4.10.54.16/chatllm/parse_utils/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      273 2023-04-21 04:20:09.000000 ChatLLM-2023.5.4.10.54.16/chatllm/parse_utils/doc_parse.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 02:54:17.175426 ChatLLM-2023.5.4.10.54.16/chatllm/utils/
+-rw-r--r--   0 betterme   (501) staff       (20)      278 2023-04-28 04:20:30.000000 ChatLLM-2023.5.4.10.54.16/chatllm/utils/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      271 2023-04-28 04:37:16.000000 ChatLLM-2023.5.4.10.54.16/chatllm/utils/_textsplitter.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2218 2023-05-04 02:54:09.000000 ChatLLM-2023.5.4.10.54.16/chatllm/utils/common.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3208 2023-04-28 04:38:58.000000 ChatLLM-2023.5.4.10.54.16/chatllm/utils/gpu_utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 02:54:17.177124 ChatLLM-2023.5.4.10.54.16/chatllm/webui/
+-rw-r--r--   0 betterme   (501) staff       (20)      270 2023-04-20 02:48:59.000000 ChatLLM-2023.5.4.10.54.16/chatllm/webui/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1488 2023-04-26 01:00:01.000000 ChatLLM-2023.5.4.10.54.16/chatllm/webui/chatbase.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3017 2023-04-28 06:43:45.000000 ChatLLM-2023.5.4.10.54.16/chatllm/webui/chatpdf.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4311 2023-04-26 01:00:01.000000 ChatLLM-2023.5.4.10.54.16/chatllm/webui/gradio_ui.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1819 2023-04-25 03:04:12.000000 ChatLLM-2023.5.4.10.54.16/chatllm/webui/nice_ui.py
+-rw-r--r--   0 betterme   (501) staff       (20)      220 2023-04-26 07:34:11.000000 ChatLLM-2023.5.4.10.54.16/chatllm/webui/run.sh
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 02:54:17.180963 ChatLLM-2023.5.4.10.54.16/data/
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 02:54:17.190311 ChatLLM-2023.5.4.10.54.16/data/imgs/
+-rw-r--r--   0 betterme   (501) staff       (20)   206137 2023-04-26 05:39:20.000000 ChatLLM-2023.5.4.10.54.16/data/imgs/LLM.drawio.png
+-rw-r--r--   0 betterme   (501) staff       (20)   206363 2023-04-26 05:33:47.000000 ChatLLM-2023.5.4.10.54.16/data/imgs/LLM.png
+-rw-r--r--   0 betterme   (501) staff       (20)  1230065 2023-04-26 08:27:23.000000 ChatLLM-2023.5.4.10.54.16/data/imgs/chatpdf.gif
+-rw-r--r--   0 betterme   (501) staff       (20)    45633 2023-04-26 04:24:13.000000 ChatLLM-2023.5.4.10.54.16/data/imgs/chatpdf_ann_df.png
+-rw-r--r--   0 betterme   (501) staff       (20)    29400 2023-04-27 10:24:48.000000 ChatLLM-2023.5.4.10.54.16/data/imgs/role.png
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 02:54:17.194063 ChatLLM-2023.5.4.10.54.16/data/医/
+-rw-r--r--   0 betterme   (501) staff       (20)  3891700 2023-04-20 11:48:19.000000 ChatLLM-2023.5.4.10.54.16/data/医/500种中药现代研究.txt
+-rw-r--r--   0 betterme   (501) staff       (20)  4926489 2023-04-20 11:46:24.000000 ChatLLM-2023.5.4.10.54.16/data/医/古今医统大全.txt
+-rw-r--r--   0 betterme   (501) staff       (20)     1633 2023-04-20 07:17:41.000000 ChatLLM-2023.5.4.10.54.16/data/姚明.txt
+-rw-r--r--   0 betterme   (501) staff       (20)      946 2023-04-20 07:17:41.000000 ChatLLM-2023.5.4.10.54.16/data/王治郅.txt
+-rw-r--r--   0 betterme   (501) staff       (20)     1291 2023-04-20 07:17:41.000000 ChatLLM-2023.5.4.10.54.16/data/科比.txt
+-rw-r--r--   0 betterme   (501) staff       (20)  3051914 2023-04-25 02:58:13.000000 ChatLLM-2023.5.4.10.54.16/data/财报.pdf
+-rw-r--r--   0 betterme   (501) staff       (20)      493 2023-04-20 07:17:41.000000 ChatLLM-2023.5.4.10.54.16/data/马保国.txt
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 02:54:17.210231 ChatLLM-2023.5.4.10.54.16/docs/
+-rw-r--r--   0 betterme   (501) staff       (20)      564 2023-04-26 04:55:25.000000 ChatLLM-2023.5.4.10.54.16/docs/INSTALL.md
+-rw-r--r--   0 betterme   (501) staff       (20)      608 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.10.54.16/docs/Makefile
+-rw-r--r--   0 betterme   (501) staff       (20)     4846 2023-04-27 11:05:23.000000 ChatLLM-2023.5.4.10.54.16/docs/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)       26 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.10.54.16/docs/_config.yml
+-rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.10.54.16/docs/authors.rst
+-rwxr-xr-x   0 betterme   (501) staff       (20)     4763 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.10.54.16/docs/conf.py
+-rw-r--r--   0 betterme   (501) staff       (20)       33 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.10.54.16/docs/contributing.rst
+-rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.10.54.16/docs/history.rst
+-rw-r--r--   0 betterme   (501) staff       (20)      304 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.10.54.16/docs/index.rst
+-rw-r--r--   0 betterme   (501) staff       (20)      805 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.10.54.16/docs/make.bat
+-rw-r--r--   0 betterme   (501) staff       (20)       27 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.10.54.16/docs/readme.rst
+-rw-r--r--   0 betterme   (501) staff       (20)       69 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.10.54.16/docs/usage.rst
+-rwxr-xr-x   0 betterme   (501) staff       (20)      269 2023-04-28 07:55:35.000000 ChatLLM-2023.5.4.10.54.16/git_init.sh
+-rwxr-xr-x   0 betterme   (501) staff       (20)      152 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.10.54.16/pypi.sh
+-rw-r--r--   0 betterme   (501) staff       (20)       78 2023-04-28 08:43:50.000000 ChatLLM-2023.5.4.10.54.16/requirements.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       14 2023-04-28 08:44:21.000000 ChatLLM-2023.5.4.10.54.16/requirements_api.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       25 2023-04-28 08:44:53.000000 ChatLLM-2023.5.4.10.54.16/requirements_pdf.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       10 2023-04-28 08:44:32.000000 ChatLLM-2023.5.4.10.54.16/requirements_streamlit.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       38 2023-05-04 02:54:17.211559 ChatLLM-2023.5.4.10.54.16/setup.cfg
+-rw-r--r--   0 betterme   (501) staff       (20)     1897 2023-04-28 08:42:35.000000 ChatLLM-2023.5.4.10.54.16/setup.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 02:54:17.210682 ChatLLM-2023.5.4.10.54.16/tests/
+-rw-r--r--   0 betterme   (501) staff       (20)       37 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.10.54.16/tests/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      852 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.10.54.16/tests/test_llm4gpt.py
+-rw-r--r--   0 betterme   (501) staff       (20)    51173 2023-04-21 11:31:44.000000 ChatLLM-2023.5.4.10.54.16/tests/内存型.ipynb
+-rw-r--r--   0 betterme   (501) staff       (20)      288 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.10.54.16/tox.ini
```

### Comparing `ChatLLM-2023.5.4.10.47.32/.gitignore` & `ChatLLM-2023.5.4.10.54.16/.gitignore`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.5.4.10.47.32/.travis.yml` & `ChatLLM-2023.5.4.10.54.16/.travis.yml`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.5.4.10.47.32/CONTRIBUTING.rst` & `ChatLLM-2023.5.4.10.54.16/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.5.4.10.47.32/ChatLLM.egg-info/PKG-INFO` & `ChatLLM-2023.5.4.10.54.16/ChatLLM.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ChatLLM
-Version: 2023.5.4.10.47.32
+Version: 2023.5.4.10.54.16
 Summary: Create a Python package.
 Home-page: https://github.com/yuanjie-ai/ChatLLM
 Author: yuanjie
 Author-email: 313303303@qq.com
 License: MIT license
 Keywords: chatllm
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `ChatLLM-2023.5.4.10.47.32/ChatLLM.egg-info/SOURCES.txt` & `ChatLLM-2023.5.4.10.54.16/ChatLLM.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.5.4.10.47.32/LICENSE` & `ChatLLM-2023.5.4.10.54.16/LICENSE`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.5.4.10.47.32/Makefile` & `ChatLLM-2023.5.4.10.54.16/Makefile`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.5.4.10.47.32/PKG-INFO` & `ChatLLM-2023.5.4.10.54.16/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ChatLLM
-Version: 2023.5.4.10.47.32
+Version: 2023.5.4.10.54.16
 Summary: Create a Python package.
 Home-page: https://github.com/yuanjie-ai/ChatLLM
 Author: yuanjie
 Author-email: 313303303@qq.com
 License: MIT license
 Keywords: chatllm
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `ChatLLM-2023.5.4.10.47.32/README.md` & `ChatLLM-2023.5.4.10.54.16/README.md`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.5.4.10.47.32/chatllm/_his/FaissANN.py` & `ChatLLM-2023.5.4.10.54.16/chatllm/_his/FaissANN.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.5.4.10.47.32/chatllm/_his/_chatllm.py` & `ChatLLM-2023.5.4.10.54.16/chatllm/_his/_chatllm.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.5.4.10.47.32/chatllm/_his/_qa.py` & `ChatLLM-2023.5.4.10.54.16/chatllm/_his/_qa.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.5.4.10.47.32/chatllm/api/stream_api.py` & `ChatLLM-2023.5.4.10.54.16/chatllm/api/stream_api.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.5.4.10.47.32/chatllm/applications/Question2Answer.py` & `ChatLLM-2023.5.4.10.54.16/chatllm/applications/Question2Answer.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.5.4.10.47.32/chatllm/applications/chatann.py` & `ChatLLM-2023.5.4.10.54.16/chatllm/applications/chatann.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.5.4.10.47.32/chatllm/applications/chatbase.py` & `ChatLLM-2023.5.4.10.54.16/chatllm/applications/chatbase.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.5.4.10.47.32/chatllm/applications/chatcrawler.py` & `ChatLLM-2023.5.4.10.54.16/chatllm/applications/chatcrawler.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.5.4.10.47.32/chatllm/applications/chatpdf.py` & `ChatLLM-2023.5.4.10.54.16/chatllm/applications/chatpdf.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.5.4.10.47.32/chatllm/applications/chatwhoosh.py` & `ChatLLM-2023.5.4.10.54.16/chatllm/applications/chatwhoosh.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.5.4.10.47.32/chatllm/chatyuan.py` & `ChatLLM-2023.5.4.10.54.16/chatllm/chatyuan.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.5.4.10.47.32/chatllm/clis/cli.py` & `ChatLLM-2023.5.4.10.54.16/chatllm/clis/cli.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.5.4.10.47.32/chatllm/embedding.py` & `ChatLLM-2023.5.4.10.54.16/chatllm/embedding.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.5.4.10.47.32/chatllm/utils/common.py` & `ChatLLM-2023.5.4.10.54.16/chatllm/utils/common.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,14 +17,16 @@
     os.environ['DEVICE'] if 'DEVICE' in os.environ
     else "cuda" if torch.cuda.is_available()
     else "mps" if torch.backends.mps.is_available()
     else "cpu"
 )
 if LOCAL_HOST.startswith('10.219'):
     MODEL_PATH = "/Users/betterme/PycharmProjects/AI/CHAT_MODEL/chatglm"
+else:
+    MODEL_PATH = "THUDM/chatglm-6b"
 
 
 # todo 多卡 https://github.com/THUDM/ChatGLM-6B#%E5%A4%9A%E5%8D%A1%E9%83%A8%E7%BD%B2
 
 def textsplitter(text, chunk_size=512, overlap_rate=0.2, sep=''):  # 简单粗暴
     return text.lower().split() | xjoin(sep) | xgroup(chunk_size, overlap_rate)
```

### Comparing `ChatLLM-2023.5.4.10.47.32/chatllm/utils/gpu_utils.py` & `ChatLLM-2023.5.4.10.54.16/chatllm/utils/gpu_utils.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.5.4.10.47.32/chatllm/webui/chatbase.py` & `ChatLLM-2023.5.4.10.54.16/chatllm/webui/chatbase.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.5.4.10.47.32/chatllm/webui/chatpdf.py` & `ChatLLM-2023.5.4.10.54.16/chatllm/webui/chatpdf.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.5.4.10.47.32/chatllm/webui/gradio_ui.py` & `ChatLLM-2023.5.4.10.54.16/chatllm/webui/gradio_ui.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.5.4.10.47.32/chatllm/webui/nice_ui.py` & `ChatLLM-2023.5.4.10.54.16/chatllm/webui/nice_ui.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.5.4.10.47.32/data/imgs/LLM.drawio.png` & `ChatLLM-2023.5.4.10.54.16/data/imgs/LLM.drawio.png`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.5.4.10.47.32/data/imgs/LLM.png` & `ChatLLM-2023.5.4.10.54.16/data/imgs/LLM.png`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.5.4.10.47.32/data/imgs/chatpdf.gif` & `ChatLLM-2023.5.4.10.54.16/data/imgs/chatpdf.gif`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.5.4.10.47.32/data/imgs/chatpdf_ann_df.png` & `ChatLLM-2023.5.4.10.54.16/data/imgs/chatpdf_ann_df.png`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.5.4.10.47.32/data/imgs/role.png` & `ChatLLM-2023.5.4.10.54.16/data/imgs/role.png`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.5.4.10.47.32/data/医/500种中药现代研究.txt` & `ChatLLM-2023.5.4.10.54.16/data/医/500种中药现代研究.txt`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.5.4.10.47.32/data/医/古今医统大全.txt` & `ChatLLM-2023.5.4.10.54.16/data/医/古今医统大全.txt`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.5.4.10.47.32/data/姚明.txt` & `ChatLLM-2023.5.4.10.54.16/data/姚明.txt`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.5.4.10.47.32/data/王治郅.txt` & `ChatLLM-2023.5.4.10.54.16/data/王治郅.txt`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.5.4.10.47.32/data/科比.txt` & `ChatLLM-2023.5.4.10.54.16/data/科比.txt`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.5.4.10.47.32/data/财报.pdf` & `ChatLLM-2023.5.4.10.54.16/data/财报.pdf`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.5.4.10.47.32/docs/INSTALL.md` & `ChatLLM-2023.5.4.10.54.16/docs/INSTALL.md`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.5.4.10.47.32/docs/Makefile` & `ChatLLM-2023.5.4.10.54.16/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.5.4.10.47.32/docs/README.md` & `ChatLLM-2023.5.4.10.54.16/docs/README.md`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.5.4.10.47.32/docs/conf.py` & `ChatLLM-2023.5.4.10.54.16/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.5.4.10.47.32/docs/make.bat` & `ChatLLM-2023.5.4.10.54.16/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.5.4.10.47.32/setup.py` & `ChatLLM-2023.5.4.10.54.16/setup.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.5.4.10.47.32/tests/test_llm4gpt.py` & `ChatLLM-2023.5.4.10.54.16/tests/test_llm4gpt.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.5.4.10.47.32/tests/内存型.ipynb` & `ChatLLM-2023.5.4.10.54.16/tests/内存型.ipynb`

 * *Files identical despite different names*

