# Comparing `tmp/ChatLLM-2023.5.4.11.53.35.tar.gz` & `tmp/ChatLLM-2023.5.4.11.58.59.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ChatLLM-2023.5.4.11.53.35.tar", last modified: Thu May  4 03:53:35 2023, max compression
+gzip compressed data, was "ChatLLM-2023.5.4.11.58.59.tar", last modified: Thu May  4 03:58:59 2023, max compression
```

## Comparing `ChatLLM-2023.5.4.11.53.35.tar` & `ChatLLM-2023.5.4.11.58.59.tar`

### file list

```diff
@@ -1,107 +1,107 @@
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 03:53:35.482502 ChatLLM-2023.5.4.11.53.35/
--rw-r--r--   0 betterme   (501) staff       (20)      292 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.11.53.35/.editorconfig
--rw-r--r--   0 betterme   (501) staff       (20)     1196 2023-04-20 11:38:14.000000 ChatLLM-2023.5.4.11.53.35/.gitignore
--rw-r--r--   0 betterme   (501) staff       (20)      697 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.11.53.35/.travis.yml
--rw-r--r--   0 betterme   (501) staff       (20)      149 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.11.53.35/AUTHORS.rst
--rw-r--r--   0 betterme   (501) staff       (20)     3530 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.11.53.35/CONTRIBUTING.rst
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 03:53:35.440825 ChatLLM-2023.5.4.11.53.35/ChatLLM.egg-info/
--rw-r--r--   0 betterme   (501) staff       (20)     5809 2023-05-04 03:53:35.000000 ChatLLM-2023.5.4.11.53.35/ChatLLM.egg-info/PKG-INFO
--rw-r--r--   0 betterme   (501) staff       (20)     2030 2023-05-04 03:53:35.000000 ChatLLM-2023.5.4.11.53.35/ChatLLM.egg-info/SOURCES.txt
--rw-r--r--   0 betterme   (501) staff       (20)        1 2023-05-04 03:53:35.000000 ChatLLM-2023.5.4.11.53.35/ChatLLM.egg-info/dependency_links.txt
--rw-r--r--   0 betterme   (501) staff       (20)       53 2023-05-04 03:53:35.000000 ChatLLM-2023.5.4.11.53.35/ChatLLM.egg-info/entry_points.txt
--rw-r--r--   0 betterme   (501) staff       (20)        1 2023-05-04 03:53:35.000000 ChatLLM-2023.5.4.11.53.35/ChatLLM.egg-info/not-zip-safe
--rw-r--r--   0 betterme   (501) staff       (20)      186 2023-05-04 03:53:35.000000 ChatLLM-2023.5.4.11.53.35/ChatLLM.egg-info/requires.txt
--rw-r--r--   0 betterme   (501) staff       (20)        8 2023-05-04 03:53:35.000000 ChatLLM-2023.5.4.11.53.35/ChatLLM.egg-info/top_level.txt
--rw-r--r--   0 betterme   (501) staff       (20)       89 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.11.53.35/HISTORY.rst
--rw-r--r--   0 betterme   (501) staff       (20)     1066 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.11.53.35/LICENSE
--rw-r--r--   0 betterme   (501) staff       (20)      289 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.11.53.35/MANIFEST.in
--rw-r--r--   0 betterme   (501) staff       (20)     2215 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.11.53.35/Makefile
--rw-r--r--   0 betterme   (501) staff       (20)     5809 2023-05-04 03:53:35.482318 ChatLLM-2023.5.4.11.53.35/PKG-INFO
--rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-26 04:55:25.000000 ChatLLM-2023.5.4.11.53.35/README.bak.md
--rw-r--r--   0 betterme   (501) staff       (20)     4907 2023-04-28 07:55:35.000000 ChatLLM-2023.5.4.11.53.35/README.md
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 03:53:35.441466 ChatLLM-2023.5.4.11.53.35/chatllm/
--rw-r--r--   0 betterme   (501) staff       (20)      199 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.11.53.35/chatllm/__init__.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 03:53:35.442716 ChatLLM-2023.5.4.11.53.35/chatllm/_his/
--rw-r--r--   0 betterme   (501) staff       (20)     1482 2023-04-20 12:23:09.000000 ChatLLM-2023.5.4.11.53.35/chatllm/_his/FaissANN.py
--rw-r--r--   0 betterme   (501) staff       (20)      286 2023-04-27 10:06:48.000000 ChatLLM-2023.5.4.11.53.35/chatllm/_his/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1812 2023-04-25 08:31:06.000000 ChatLLM-2023.5.4.11.53.35/chatllm/_his/_chatllm.py
--rw-r--r--   0 betterme   (501) staff       (20)     2493 2023-04-27 10:06:48.000000 ChatLLM-2023.5.4.11.53.35/chatllm/_his/_qa.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 03:53:35.443218 ChatLLM-2023.5.4.11.53.35/chatllm/api/
--rw-r--r--   0 betterme   (501) staff       (20)      270 2023-04-28 01:04:39.000000 ChatLLM-2023.5.4.11.53.35/chatllm/api/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1827 2023-04-28 02:36:43.000000 ChatLLM-2023.5.4.11.53.35/chatllm/api/stream_api.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 03:53:35.446888 ChatLLM-2023.5.4.11.53.35/chatllm/applications/
--rw-r--r--   0 betterme   (501) staff       (20)     3532 2023-04-25 01:19:43.000000 ChatLLM-2023.5.4.11.53.35/chatllm/applications/Question2Answer.py
--rw-r--r--   0 betterme   (501) staff       (20)      294 2023-04-25 08:32:56.000000 ChatLLM-2023.5.4.11.53.35/chatllm/applications/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     2805 2023-04-27 04:33:02.000000 ChatLLM-2023.5.4.11.53.35/chatllm/applications/chatann.py
--rw-r--r--   0 betterme   (501) staff       (20)      267 2023-05-04 01:43:23.000000 ChatLLM-2023.5.4.11.53.35/chatllm/applications/chataudio.py
--rw-r--r--   0 betterme   (501) staff       (20)     3642 2023-05-04 03:53:33.000000 ChatLLM-2023.5.4.11.53.35/chatllm/applications/chatbase.py
--rw-r--r--   0 betterme   (501) staff       (20)     1176 2023-04-26 01:00:01.000000 ChatLLM-2023.5.4.11.53.35/chatllm/applications/chatcrawler.py
--rw-r--r--   0 betterme   (501) staff       (20)      266 2023-04-25 01:23:41.000000 ChatLLM-2023.5.4.11.53.35/chatllm/applications/chatdoc.py
--rw-r--r--   0 betterme   (501) staff       (20)      316 2023-05-04 03:46:23.000000 ChatLLM-2023.5.4.11.53.35/chatllm/applications/chatmind.py
--rw-r--r--   0 betterme   (501) staff       (20)     1357 2023-04-28 07:16:03.000000 ChatLLM-2023.5.4.11.53.35/chatllm/applications/chatpdf.py
--rw-r--r--   0 betterme   (501) staff       (20)      269 2023-04-26 00:59:00.000000 ChatLLM-2023.5.4.11.53.35/chatllm/applications/chatsearch.py
--rw-r--r--   0 betterme   (501) staff       (20)      266 2023-04-25 01:23:41.000000 ChatLLM-2023.5.4.11.53.35/chatllm/applications/chatweb.py
--rw-r--r--   0 betterme   (501) staff       (20)     1895 2023-04-27 02:58:56.000000 ChatLLM-2023.5.4.11.53.35/chatllm/applications/chatwhoosh.py
--rw-r--r--   0 betterme   (501) staff       (20)      286 2023-04-21 05:42:37.000000 ChatLLM-2023.5.4.11.53.35/chatllm/applications/pipeline.py
--rw-r--r--   0 betterme   (501) staff       (20)     1964 2023-04-27 09:24:25.000000 ChatLLM-2023.5.4.11.53.35/chatllm/chatyuan.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 03:53:35.447502 ChatLLM-2023.5.4.11.53.35/chatllm/clis/
--rw-r--r--   0 betterme   (501) staff       (20)      413 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.11.53.35/chatllm/clis/README.md
--rw-r--r--   0 betterme   (501) staff       (20)      279 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.11.53.35/chatllm/clis/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1334 2023-04-28 07:03:35.000000 ChatLLM-2023.5.4.11.53.35/chatllm/clis/cli.py
--rw-r--r--   0 betterme   (501) staff       (20)     1439 2023-04-27 01:39:42.000000 ChatLLM-2023.5.4.11.53.35/chatllm/embedding.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 03:53:35.447952 ChatLLM-2023.5.4.11.53.35/chatllm/parse_utils/
--rw-r--r--   0 betterme   (501) staff       (20)      302 2023-04-25 01:22:30.000000 ChatLLM-2023.5.4.11.53.35/chatllm/parse_utils/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      273 2023-04-21 04:20:09.000000 ChatLLM-2023.5.4.11.53.35/chatllm/parse_utils/doc_parse.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 03:53:35.449179 ChatLLM-2023.5.4.11.53.35/chatllm/utils/
--rw-r--r--   0 betterme   (501) staff       (20)      278 2023-04-28 04:20:30.000000 ChatLLM-2023.5.4.11.53.35/chatllm/utils/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      271 2023-04-28 04:37:16.000000 ChatLLM-2023.5.4.11.53.35/chatllm/utils/_textsplitter.py
--rw-r--r--   0 betterme   (501) staff       (20)     2218 2023-05-04 02:54:09.000000 ChatLLM-2023.5.4.11.53.35/chatllm/utils/common.py
--rw-r--r--   0 betterme   (501) staff       (20)     3208 2023-04-28 04:38:58.000000 ChatLLM-2023.5.4.11.53.35/chatllm/utils/gpu_utils.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 03:53:35.451149 ChatLLM-2023.5.4.11.53.35/chatllm/webui/
--rw-r--r--   0 betterme   (501) staff       (20)      270 2023-04-20 02:48:59.000000 ChatLLM-2023.5.4.11.53.35/chatllm/webui/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)     1488 2023-04-26 01:00:01.000000 ChatLLM-2023.5.4.11.53.35/chatllm/webui/chatbase.py
--rw-r--r--   0 betterme   (501) staff       (20)     3017 2023-04-28 06:43:45.000000 ChatLLM-2023.5.4.11.53.35/chatllm/webui/chatpdf.py
--rw-r--r--   0 betterme   (501) staff       (20)     4311 2023-04-26 01:00:01.000000 ChatLLM-2023.5.4.11.53.35/chatllm/webui/gradio_ui.py
--rw-r--r--   0 betterme   (501) staff       (20)     1819 2023-04-25 03:04:12.000000 ChatLLM-2023.5.4.11.53.35/chatllm/webui/nice_ui.py
--rw-r--r--   0 betterme   (501) staff       (20)      220 2023-04-26 07:34:11.000000 ChatLLM-2023.5.4.11.53.35/chatllm/webui/run.sh
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 03:53:35.455316 ChatLLM-2023.5.4.11.53.35/data/
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 03:53:35.462895 ChatLLM-2023.5.4.11.53.35/data/imgs/
--rw-r--r--   0 betterme   (501) staff       (20)   206137 2023-04-26 05:39:20.000000 ChatLLM-2023.5.4.11.53.35/data/imgs/LLM.drawio.png
--rw-r--r--   0 betterme   (501) staff       (20)   206363 2023-04-26 05:33:47.000000 ChatLLM-2023.5.4.11.53.35/data/imgs/LLM.png
--rw-r--r--   0 betterme   (501) staff       (20)  1230065 2023-04-26 08:27:23.000000 ChatLLM-2023.5.4.11.53.35/data/imgs/chatpdf.gif
--rw-r--r--   0 betterme   (501) staff       (20)    45633 2023-04-26 04:24:13.000000 ChatLLM-2023.5.4.11.53.35/data/imgs/chatpdf_ann_df.png
--rw-r--r--   0 betterme   (501) staff       (20)    29400 2023-04-27 10:24:48.000000 ChatLLM-2023.5.4.11.53.35/data/imgs/role.png
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 03:53:35.468312 ChatLLM-2023.5.4.11.53.35/data/医/
--rw-r--r--   0 betterme   (501) staff       (20)  3891700 2023-04-20 11:48:19.000000 ChatLLM-2023.5.4.11.53.35/data/医/500种中药现代研究.txt
--rw-r--r--   0 betterme   (501) staff       (20)  4926489 2023-04-20 11:46:24.000000 ChatLLM-2023.5.4.11.53.35/data/医/古今医统大全.txt
--rw-r--r--   0 betterme   (501) staff       (20)     1633 2023-04-20 07:17:41.000000 ChatLLM-2023.5.4.11.53.35/data/姚明.txt
--rw-r--r--   0 betterme   (501) staff       (20)      946 2023-04-20 07:17:41.000000 ChatLLM-2023.5.4.11.53.35/data/王治郅.txt
--rw-r--r--   0 betterme   (501) staff       (20)     1291 2023-04-20 07:17:41.000000 ChatLLM-2023.5.4.11.53.35/data/科比.txt
--rw-r--r--   0 betterme   (501) staff       (20)  3051914 2023-04-25 02:58:13.000000 ChatLLM-2023.5.4.11.53.35/data/财报.pdf
--rw-r--r--   0 betterme   (501) staff       (20)      493 2023-04-20 07:17:41.000000 ChatLLM-2023.5.4.11.53.35/data/马保国.txt
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 03:53:35.481153 ChatLLM-2023.5.4.11.53.35/docs/
--rw-r--r--   0 betterme   (501) staff       (20)      564 2023-04-26 04:55:25.000000 ChatLLM-2023.5.4.11.53.35/docs/INSTALL.md
--rw-r--r--   0 betterme   (501) staff       (20)      608 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.11.53.35/docs/Makefile
--rw-r--r--   0 betterme   (501) staff       (20)     4846 2023-04-27 11:05:23.000000 ChatLLM-2023.5.4.11.53.35/docs/README.md
--rw-r--r--   0 betterme   (501) staff       (20)       26 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.11.53.35/docs/_config.yml
--rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.11.53.35/docs/authors.rst
--rwxr-xr-x   0 betterme   (501) staff       (20)     4763 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.11.53.35/docs/conf.py
--rw-r--r--   0 betterme   (501) staff       (20)       33 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.11.53.35/docs/contributing.rst
--rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.11.53.35/docs/history.rst
--rw-r--r--   0 betterme   (501) staff       (20)      304 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.11.53.35/docs/index.rst
--rw-r--r--   0 betterme   (501) staff       (20)      805 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.11.53.35/docs/make.bat
--rw-r--r--   0 betterme   (501) staff       (20)       27 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.11.53.35/docs/readme.rst
--rw-r--r--   0 betterme   (501) staff       (20)       69 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.11.53.35/docs/usage.rst
--rwxr-xr-x   0 betterme   (501) staff       (20)      269 2023-04-28 07:55:35.000000 ChatLLM-2023.5.4.11.53.35/git_init.sh
--rwxr-xr-x   0 betterme   (501) staff       (20)      152 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.11.53.35/pypi.sh
--rw-r--r--   0 betterme   (501) staff       (20)       78 2023-04-28 08:43:50.000000 ChatLLM-2023.5.4.11.53.35/requirements.txt
--rw-r--r--   0 betterme   (501) staff       (20)       14 2023-04-28 08:44:21.000000 ChatLLM-2023.5.4.11.53.35/requirements_api.txt
--rw-r--r--   0 betterme   (501) staff       (20)       25 2023-04-28 08:44:53.000000 ChatLLM-2023.5.4.11.53.35/requirements_pdf.txt
--rw-r--r--   0 betterme   (501) staff       (20)       10 2023-04-28 08:44:32.000000 ChatLLM-2023.5.4.11.53.35/requirements_streamlit.txt
--rw-r--r--   0 betterme   (501) staff       (20)       38 2023-05-04 03:53:35.482561 ChatLLM-2023.5.4.11.53.35/setup.cfg
--rw-r--r--   0 betterme   (501) staff       (20)     1897 2023-04-28 08:42:35.000000 ChatLLM-2023.5.4.11.53.35/setup.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 03:53:35.481610 ChatLLM-2023.5.4.11.53.35/tests/
--rw-r--r--   0 betterme   (501) staff       (20)       37 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.11.53.35/tests/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)      852 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.11.53.35/tests/test_llm4gpt.py
--rw-r--r--   0 betterme   (501) staff       (20)    51173 2023-04-21 11:31:44.000000 ChatLLM-2023.5.4.11.53.35/tests/内存型.ipynb
--rw-r--r--   0 betterme   (501) staff       (20)      288 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.11.53.35/tox.ini
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 03:58:59.734383 ChatLLM-2023.5.4.11.58.59/
+-rw-r--r--   0 betterme   (501) staff       (20)      292 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.11.58.59/.editorconfig
+-rw-r--r--   0 betterme   (501) staff       (20)     1196 2023-04-20 11:38:14.000000 ChatLLM-2023.5.4.11.58.59/.gitignore
+-rw-r--r--   0 betterme   (501) staff       (20)      697 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.11.58.59/.travis.yml
+-rw-r--r--   0 betterme   (501) staff       (20)      149 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.11.58.59/AUTHORS.rst
+-rw-r--r--   0 betterme   (501) staff       (20)     3530 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.11.58.59/CONTRIBUTING.rst
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 03:58:59.695903 ChatLLM-2023.5.4.11.58.59/ChatLLM.egg-info/
+-rw-r--r--   0 betterme   (501) staff       (20)     5809 2023-05-04 03:58:59.000000 ChatLLM-2023.5.4.11.58.59/ChatLLM.egg-info/PKG-INFO
+-rw-r--r--   0 betterme   (501) staff       (20)     2030 2023-05-04 03:58:59.000000 ChatLLM-2023.5.4.11.58.59/ChatLLM.egg-info/SOURCES.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        1 2023-05-04 03:58:59.000000 ChatLLM-2023.5.4.11.58.59/ChatLLM.egg-info/dependency_links.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       53 2023-05-04 03:58:59.000000 ChatLLM-2023.5.4.11.58.59/ChatLLM.egg-info/entry_points.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        1 2023-05-04 03:58:59.000000 ChatLLM-2023.5.4.11.58.59/ChatLLM.egg-info/not-zip-safe
+-rw-r--r--   0 betterme   (501) staff       (20)      186 2023-05-04 03:58:59.000000 ChatLLM-2023.5.4.11.58.59/ChatLLM.egg-info/requires.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        8 2023-05-04 03:58:59.000000 ChatLLM-2023.5.4.11.58.59/ChatLLM.egg-info/top_level.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       89 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.11.58.59/HISTORY.rst
+-rw-r--r--   0 betterme   (501) staff       (20)     1066 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.11.58.59/LICENSE
+-rw-r--r--   0 betterme   (501) staff       (20)      289 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.11.58.59/MANIFEST.in
+-rw-r--r--   0 betterme   (501) staff       (20)     2215 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.11.58.59/Makefile
+-rw-r--r--   0 betterme   (501) staff       (20)     5809 2023-05-04 03:58:59.734207 ChatLLM-2023.5.4.11.58.59/PKG-INFO
+-rw-r--r--   0 betterme   (501) staff       (20)        0 2023-04-26 04:55:25.000000 ChatLLM-2023.5.4.11.58.59/README.bak.md
+-rw-r--r--   0 betterme   (501) staff       (20)     4907 2023-04-28 07:55:35.000000 ChatLLM-2023.5.4.11.58.59/README.md
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 03:58:59.696568 ChatLLM-2023.5.4.11.58.59/chatllm/
+-rw-r--r--   0 betterme   (501) staff       (20)      199 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.11.58.59/chatllm/__init__.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 03:58:59.697687 ChatLLM-2023.5.4.11.58.59/chatllm/_his/
+-rw-r--r--   0 betterme   (501) staff       (20)     1482 2023-04-20 12:23:09.000000 ChatLLM-2023.5.4.11.58.59/chatllm/_his/FaissANN.py
+-rw-r--r--   0 betterme   (501) staff       (20)      286 2023-04-27 10:06:48.000000 ChatLLM-2023.5.4.11.58.59/chatllm/_his/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1812 2023-04-25 08:31:06.000000 ChatLLM-2023.5.4.11.58.59/chatllm/_his/_chatllm.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2493 2023-04-27 10:06:48.000000 ChatLLM-2023.5.4.11.58.59/chatllm/_his/_qa.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 03:58:59.698118 ChatLLM-2023.5.4.11.58.59/chatllm/api/
+-rw-r--r--   0 betterme   (501) staff       (20)      270 2023-04-28 01:04:39.000000 ChatLLM-2023.5.4.11.58.59/chatllm/api/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1827 2023-04-28 02:36:43.000000 ChatLLM-2023.5.4.11.58.59/chatllm/api/stream_api.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 03:58:59.701104 ChatLLM-2023.5.4.11.58.59/chatllm/applications/
+-rw-r--r--   0 betterme   (501) staff       (20)     3532 2023-04-25 01:19:43.000000 ChatLLM-2023.5.4.11.58.59/chatllm/applications/Question2Answer.py
+-rw-r--r--   0 betterme   (501) staff       (20)      294 2023-04-25 08:32:56.000000 ChatLLM-2023.5.4.11.58.59/chatllm/applications/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2805 2023-04-27 04:33:02.000000 ChatLLM-2023.5.4.11.58.59/chatllm/applications/chatann.py
+-rw-r--r--   0 betterme   (501) staff       (20)      267 2023-05-04 01:43:23.000000 ChatLLM-2023.5.4.11.58.59/chatllm/applications/chataudio.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3582 2023-05-04 03:58:57.000000 ChatLLM-2023.5.4.11.58.59/chatllm/applications/chatbase.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1176 2023-04-26 01:00:01.000000 ChatLLM-2023.5.4.11.58.59/chatllm/applications/chatcrawler.py
+-rw-r--r--   0 betterme   (501) staff       (20)      266 2023-04-25 01:23:41.000000 ChatLLM-2023.5.4.11.58.59/chatllm/applications/chatdoc.py
+-rw-r--r--   0 betterme   (501) staff       (20)      316 2023-05-04 03:46:23.000000 ChatLLM-2023.5.4.11.58.59/chatllm/applications/chatmind.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1357 2023-04-28 07:16:03.000000 ChatLLM-2023.5.4.11.58.59/chatllm/applications/chatpdf.py
+-rw-r--r--   0 betterme   (501) staff       (20)      269 2023-04-26 00:59:00.000000 ChatLLM-2023.5.4.11.58.59/chatllm/applications/chatsearch.py
+-rw-r--r--   0 betterme   (501) staff       (20)      266 2023-04-25 01:23:41.000000 ChatLLM-2023.5.4.11.58.59/chatllm/applications/chatweb.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1895 2023-04-27 02:58:56.000000 ChatLLM-2023.5.4.11.58.59/chatllm/applications/chatwhoosh.py
+-rw-r--r--   0 betterme   (501) staff       (20)      286 2023-04-21 05:42:37.000000 ChatLLM-2023.5.4.11.58.59/chatllm/applications/pipeline.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1964 2023-04-27 09:24:25.000000 ChatLLM-2023.5.4.11.58.59/chatllm/chatyuan.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 03:58:59.701661 ChatLLM-2023.5.4.11.58.59/chatllm/clis/
+-rw-r--r--   0 betterme   (501) staff       (20)      413 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.11.58.59/chatllm/clis/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)      279 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.11.58.59/chatllm/clis/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1334 2023-04-28 07:03:35.000000 ChatLLM-2023.5.4.11.58.59/chatllm/clis/cli.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1439 2023-04-27 01:39:42.000000 ChatLLM-2023.5.4.11.58.59/chatllm/embedding.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 03:58:59.702115 ChatLLM-2023.5.4.11.58.59/chatllm/parse_utils/
+-rw-r--r--   0 betterme   (501) staff       (20)      302 2023-04-25 01:22:30.000000 ChatLLM-2023.5.4.11.58.59/chatllm/parse_utils/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      273 2023-04-21 04:20:09.000000 ChatLLM-2023.5.4.11.58.59/chatllm/parse_utils/doc_parse.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 03:58:59.703042 ChatLLM-2023.5.4.11.58.59/chatllm/utils/
+-rw-r--r--   0 betterme   (501) staff       (20)      278 2023-04-28 04:20:30.000000 ChatLLM-2023.5.4.11.58.59/chatllm/utils/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      271 2023-04-28 04:37:16.000000 ChatLLM-2023.5.4.11.58.59/chatllm/utils/_textsplitter.py
+-rw-r--r--   0 betterme   (501) staff       (20)     2218 2023-05-04 02:54:09.000000 ChatLLM-2023.5.4.11.58.59/chatllm/utils/common.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3208 2023-04-28 04:38:58.000000 ChatLLM-2023.5.4.11.58.59/chatllm/utils/gpu_utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 03:58:59.704508 ChatLLM-2023.5.4.11.58.59/chatllm/webui/
+-rw-r--r--   0 betterme   (501) staff       (20)      270 2023-04-20 02:48:59.000000 ChatLLM-2023.5.4.11.58.59/chatllm/webui/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1488 2023-04-26 01:00:01.000000 ChatLLM-2023.5.4.11.58.59/chatllm/webui/chatbase.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3017 2023-04-28 06:43:45.000000 ChatLLM-2023.5.4.11.58.59/chatllm/webui/chatpdf.py
+-rw-r--r--   0 betterme   (501) staff       (20)     4311 2023-04-26 01:00:01.000000 ChatLLM-2023.5.4.11.58.59/chatllm/webui/gradio_ui.py
+-rw-r--r--   0 betterme   (501) staff       (20)     1819 2023-04-25 03:04:12.000000 ChatLLM-2023.5.4.11.58.59/chatllm/webui/nice_ui.py
+-rw-r--r--   0 betterme   (501) staff       (20)      220 2023-04-26 07:34:11.000000 ChatLLM-2023.5.4.11.58.59/chatllm/webui/run.sh
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 03:58:59.708522 ChatLLM-2023.5.4.11.58.59/data/
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 03:58:59.714482 ChatLLM-2023.5.4.11.58.59/data/imgs/
+-rw-r--r--   0 betterme   (501) staff       (20)   206137 2023-04-26 05:39:20.000000 ChatLLM-2023.5.4.11.58.59/data/imgs/LLM.drawio.png
+-rw-r--r--   0 betterme   (501) staff       (20)   206363 2023-04-26 05:33:47.000000 ChatLLM-2023.5.4.11.58.59/data/imgs/LLM.png
+-rw-r--r--   0 betterme   (501) staff       (20)  1230065 2023-04-26 08:27:23.000000 ChatLLM-2023.5.4.11.58.59/data/imgs/chatpdf.gif
+-rw-r--r--   0 betterme   (501) staff       (20)    45633 2023-04-26 04:24:13.000000 ChatLLM-2023.5.4.11.58.59/data/imgs/chatpdf_ann_df.png
+-rw-r--r--   0 betterme   (501) staff       (20)    29400 2023-04-27 10:24:48.000000 ChatLLM-2023.5.4.11.58.59/data/imgs/role.png
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 03:58:59.719708 ChatLLM-2023.5.4.11.58.59/data/医/
+-rw-r--r--   0 betterme   (501) staff       (20)  3891700 2023-04-20 11:48:19.000000 ChatLLM-2023.5.4.11.58.59/data/医/500种中药现代研究.txt
+-rw-r--r--   0 betterme   (501) staff       (20)  4926489 2023-04-20 11:46:24.000000 ChatLLM-2023.5.4.11.58.59/data/医/古今医统大全.txt
+-rw-r--r--   0 betterme   (501) staff       (20)     1633 2023-04-20 07:17:41.000000 ChatLLM-2023.5.4.11.58.59/data/姚明.txt
+-rw-r--r--   0 betterme   (501) staff       (20)      946 2023-04-20 07:17:41.000000 ChatLLM-2023.5.4.11.58.59/data/王治郅.txt
+-rw-r--r--   0 betterme   (501) staff       (20)     1291 2023-04-20 07:17:41.000000 ChatLLM-2023.5.4.11.58.59/data/科比.txt
+-rw-r--r--   0 betterme   (501) staff       (20)  3051914 2023-04-25 02:58:13.000000 ChatLLM-2023.5.4.11.58.59/data/财报.pdf
+-rw-r--r--   0 betterme   (501) staff       (20)      493 2023-04-20 07:17:41.000000 ChatLLM-2023.5.4.11.58.59/data/马保国.txt
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 03:58:59.732231 ChatLLM-2023.5.4.11.58.59/docs/
+-rw-r--r--   0 betterme   (501) staff       (20)      564 2023-04-26 04:55:25.000000 ChatLLM-2023.5.4.11.58.59/docs/INSTALL.md
+-rw-r--r--   0 betterme   (501) staff       (20)      608 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.11.58.59/docs/Makefile
+-rw-r--r--   0 betterme   (501) staff       (20)     4846 2023-04-27 11:05:23.000000 ChatLLM-2023.5.4.11.58.59/docs/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)       26 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.11.58.59/docs/_config.yml
+-rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.11.58.59/docs/authors.rst
+-rwxr-xr-x   0 betterme   (501) staff       (20)     4763 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.11.58.59/docs/conf.py
+-rw-r--r--   0 betterme   (501) staff       (20)       33 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.11.58.59/docs/contributing.rst
+-rw-r--r--   0 betterme   (501) staff       (20)       28 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.11.58.59/docs/history.rst
+-rw-r--r--   0 betterme   (501) staff       (20)      304 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.11.58.59/docs/index.rst
+-rw-r--r--   0 betterme   (501) staff       (20)      805 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.11.58.59/docs/make.bat
+-rw-r--r--   0 betterme   (501) staff       (20)       27 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.11.58.59/docs/readme.rst
+-rw-r--r--   0 betterme   (501) staff       (20)       69 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.11.58.59/docs/usage.rst
+-rwxr-xr-x   0 betterme   (501) staff       (20)      269 2023-04-28 07:55:35.000000 ChatLLM-2023.5.4.11.58.59/git_init.sh
+-rwxr-xr-x   0 betterme   (501) staff       (20)      152 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.11.58.59/pypi.sh
+-rw-r--r--   0 betterme   (501) staff       (20)       78 2023-04-28 08:43:50.000000 ChatLLM-2023.5.4.11.58.59/requirements.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       14 2023-04-28 08:44:21.000000 ChatLLM-2023.5.4.11.58.59/requirements_api.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       25 2023-04-28 08:44:53.000000 ChatLLM-2023.5.4.11.58.59/requirements_pdf.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       10 2023-04-28 08:44:32.000000 ChatLLM-2023.5.4.11.58.59/requirements_streamlit.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       38 2023-05-04 03:58:59.734437 ChatLLM-2023.5.4.11.58.59/setup.cfg
+-rw-r--r--   0 betterme   (501) staff       (20)     1897 2023-04-28 08:42:35.000000 ChatLLM-2023.5.4.11.58.59/setup.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-04 03:58:59.732745 ChatLLM-2023.5.4.11.58.59/tests/
+-rw-r--r--   0 betterme   (501) staff       (20)       37 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.11.58.59/tests/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)      852 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.11.58.59/tests/test_llm4gpt.py
+-rw-r--r--   0 betterme   (501) staff       (20)    51173 2023-04-21 11:31:44.000000 ChatLLM-2023.5.4.11.58.59/tests/内存型.ipynb
+-rw-r--r--   0 betterme   (501) staff       (20)      288 2023-04-11 04:23:57.000000 ChatLLM-2023.5.4.11.58.59/tox.ini
```

### Comparing `ChatLLM-2023.5.4.11.53.35/.gitignore` & `ChatLLM-2023.5.4.11.58.59/.gitignore`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.5.4.11.53.35/.travis.yml` & `ChatLLM-2023.5.4.11.58.59/.travis.yml`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.5.4.11.53.35/CONTRIBUTING.rst` & `ChatLLM-2023.5.4.11.58.59/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.5.4.11.53.35/ChatLLM.egg-info/PKG-INFO` & `ChatLLM-2023.5.4.11.58.59/ChatLLM.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ChatLLM
-Version: 2023.5.4.11.53.35
+Version: 2023.5.4.11.58.59
 Summary: Create a Python package.
 Home-page: https://github.com/yuanjie-ai/ChatLLM
 Author: yuanjie
 Author-email: 313303303@qq.com
 License: MIT license
 Keywords: chatllm
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `ChatLLM-2023.5.4.11.53.35/ChatLLM.egg-info/SOURCES.txt` & `ChatLLM-2023.5.4.11.58.59/ChatLLM.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.5.4.11.53.35/LICENSE` & `ChatLLM-2023.5.4.11.58.59/LICENSE`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.5.4.11.53.35/Makefile` & `ChatLLM-2023.5.4.11.58.59/Makefile`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.5.4.11.53.35/PKG-INFO` & `ChatLLM-2023.5.4.11.58.59/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ChatLLM
-Version: 2023.5.4.11.53.35
+Version: 2023.5.4.11.58.59
 Summary: Create a Python package.
 Home-page: https://github.com/yuanjie-ai/ChatLLM
 Author: yuanjie
 Author-email: 313303303@qq.com
 License: MIT license
 Keywords: chatllm
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `ChatLLM-2023.5.4.11.53.35/README.md` & `ChatLLM-2023.5.4.11.58.59/README.md`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.5.4.11.53.35/chatllm/_his/FaissANN.py` & `ChatLLM-2023.5.4.11.58.59/chatllm/_his/FaissANN.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.5.4.11.53.35/chatllm/_his/_chatllm.py` & `ChatLLM-2023.5.4.11.58.59/chatllm/_his/_chatllm.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.5.4.11.53.35/chatllm/_his/_qa.py` & `ChatLLM-2023.5.4.11.58.59/chatllm/_his/_qa.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.5.4.11.53.35/chatllm/api/stream_api.py` & `ChatLLM-2023.5.4.11.58.59/chatllm/api/stream_api.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.5.4.11.53.35/chatllm/applications/Question2Answer.py` & `ChatLLM-2023.5.4.11.58.59/chatllm/applications/Question2Answer.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.5.4.11.53.35/chatllm/applications/chatann.py` & `ChatLLM-2023.5.4.11.58.59/chatllm/applications/chatann.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.5.4.11.53.35/chatllm/applications/chatbase.py` & `ChatLLM-2023.5.4.11.58.59/chatllm/applications/chatbase.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,18 +37,17 @@
         self.chat_func = partial(self.chat_func, **kwargs)
 
     @clear_cuda_cache
     def _qa(self, query, knowledge_base='', role='', max_turns=1):
         self.role = role or os.environ.get('LLM_ROLE', '')
         self.knowledge_base = knowledge_base.strip()
         if self.knowledge_base:
-            self.prompt_template = """{role}\n{question}"""  # 简化模版
-            query = """{role}\n{question}""".format(question=query, role=self.role).strip()
-        else:
             query = self.prompt_template.format(context=self.knowledge_base, question=query, role=self.role).strip()
+        else:
+            query = """{role}\n{question}""".format(question=query, role=self.role).strip()  # 简化模版
 
         _history = self.history[-(max_turns - 1):] if max_turns > 1 else []
         result = self.chat_func(query=query, history=_history)
 
         if isinstance(result, types.GeneratorType):
             return self._stream(result)
         else:
```

### Comparing `ChatLLM-2023.5.4.11.53.35/chatllm/applications/chatcrawler.py` & `ChatLLM-2023.5.4.11.58.59/chatllm/applications/chatcrawler.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.5.4.11.53.35/chatllm/applications/chatpdf.py` & `ChatLLM-2023.5.4.11.58.59/chatllm/applications/chatpdf.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.5.4.11.53.35/chatllm/applications/chatwhoosh.py` & `ChatLLM-2023.5.4.11.58.59/chatllm/applications/chatwhoosh.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.5.4.11.53.35/chatllm/chatyuan.py` & `ChatLLM-2023.5.4.11.58.59/chatllm/chatyuan.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.5.4.11.53.35/chatllm/clis/cli.py` & `ChatLLM-2023.5.4.11.58.59/chatllm/clis/cli.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.5.4.11.53.35/chatllm/embedding.py` & `ChatLLM-2023.5.4.11.58.59/chatllm/embedding.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.5.4.11.53.35/chatllm/utils/common.py` & `ChatLLM-2023.5.4.11.58.59/chatllm/utils/common.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.5.4.11.53.35/chatllm/utils/gpu_utils.py` & `ChatLLM-2023.5.4.11.58.59/chatllm/utils/gpu_utils.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.5.4.11.53.35/chatllm/webui/chatbase.py` & `ChatLLM-2023.5.4.11.58.59/chatllm/webui/chatbase.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.5.4.11.53.35/chatllm/webui/chatpdf.py` & `ChatLLM-2023.5.4.11.58.59/chatllm/webui/chatpdf.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.5.4.11.53.35/chatllm/webui/gradio_ui.py` & `ChatLLM-2023.5.4.11.58.59/chatllm/webui/gradio_ui.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.5.4.11.53.35/chatllm/webui/nice_ui.py` & `ChatLLM-2023.5.4.11.58.59/chatllm/webui/nice_ui.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.5.4.11.53.35/data/imgs/LLM.drawio.png` & `ChatLLM-2023.5.4.11.58.59/data/imgs/LLM.drawio.png`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.5.4.11.53.35/data/imgs/LLM.png` & `ChatLLM-2023.5.4.11.58.59/data/imgs/LLM.png`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.5.4.11.53.35/data/imgs/chatpdf.gif` & `ChatLLM-2023.5.4.11.58.59/data/imgs/chatpdf.gif`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.5.4.11.53.35/data/imgs/chatpdf_ann_df.png` & `ChatLLM-2023.5.4.11.58.59/data/imgs/chatpdf_ann_df.png`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.5.4.11.53.35/data/imgs/role.png` & `ChatLLM-2023.5.4.11.58.59/data/imgs/role.png`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.5.4.11.53.35/data/医/500种中药现代研究.txt` & `ChatLLM-2023.5.4.11.58.59/data/医/500种中药现代研究.txt`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.5.4.11.53.35/data/医/古今医统大全.txt` & `ChatLLM-2023.5.4.11.58.59/data/医/古今医统大全.txt`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.5.4.11.53.35/data/姚明.txt` & `ChatLLM-2023.5.4.11.58.59/data/姚明.txt`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.5.4.11.53.35/data/王治郅.txt` & `ChatLLM-2023.5.4.11.58.59/data/王治郅.txt`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.5.4.11.53.35/data/科比.txt` & `ChatLLM-2023.5.4.11.58.59/data/科比.txt`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.5.4.11.53.35/data/财报.pdf` & `ChatLLM-2023.5.4.11.58.59/data/财报.pdf`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.5.4.11.53.35/docs/INSTALL.md` & `ChatLLM-2023.5.4.11.58.59/docs/INSTALL.md`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.5.4.11.53.35/docs/Makefile` & `ChatLLM-2023.5.4.11.58.59/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.5.4.11.53.35/docs/README.md` & `ChatLLM-2023.5.4.11.58.59/docs/README.md`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.5.4.11.53.35/docs/conf.py` & `ChatLLM-2023.5.4.11.58.59/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.5.4.11.53.35/docs/make.bat` & `ChatLLM-2023.5.4.11.58.59/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.5.4.11.53.35/setup.py` & `ChatLLM-2023.5.4.11.58.59/setup.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.5.4.11.53.35/tests/test_llm4gpt.py` & `ChatLLM-2023.5.4.11.58.59/tests/test_llm4gpt.py`

 * *Files identical despite different names*

### Comparing `ChatLLM-2023.5.4.11.53.35/tests/内存型.ipynb` & `ChatLLM-2023.5.4.11.58.59/tests/内存型.ipynb`

 * *Files identical despite different names*

