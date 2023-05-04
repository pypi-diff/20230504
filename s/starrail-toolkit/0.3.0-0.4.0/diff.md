# Comparing `tmp/starrail-toolkit-0.3.0.tar.gz` & `tmp/starrail-toolkit-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starrail-toolkit-0.3.0.tar", last modified: Tue May  2 18:11:20 2023, max compression
+gzip compressed data, was "starrail-toolkit-0.4.0.tar", last modified: Thu May  4 08:07:26 2023, max compression
```

## Comparing `starrail-toolkit-0.3.0.tar` & `starrail-toolkit-0.4.0.tar`

### file list

```diff
@@ -1,43 +1,45 @@
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-02 18:11:20.093640 starrail-toolkit-0.3.0/
--rw-r--r--   0 littlenyima   (501) staff       (20)    35149 2023-04-29 06:29:57.000000 starrail-toolkit-0.3.0/LICENSE
--rw-r--r--   0 littlenyima   (501) staff       (20)     3353 2023-05-02 18:11:20.093516 starrail-toolkit-0.3.0/PKG-INFO
--rw-r--r--   0 littlenyima   (501) staff       (20)     2846 2023-05-02 18:09:34.000000 starrail-toolkit-0.3.0/README.md
--rw-r--r--   0 littlenyima   (501) staff       (20)       38 2023-05-02 18:11:20.093675 starrail-toolkit-0.3.0/setup.cfg
--rw-r--r--   0 littlenyima   (501) staff       (20)     4153 2023-04-30 15:17:38.000000 starrail-toolkit-0.3.0/setup.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-02 18:11:20.089565 starrail-toolkit-0.3.0/starrail/
--rw-r--r--   0 littlenyima   (501) staff       (20)      724 2023-05-01 17:01:35.000000 starrail-toolkit-0.3.0/starrail/__init__.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      996 2023-05-02 10:02:46.000000 starrail-toolkit-0.3.0/starrail/config.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-02 18:11:20.090248 starrail-toolkit-0.3.0/starrail/entry/
--rw-r--r--   0 littlenyima   (501) staff       (20)       49 2023-04-30 15:17:38.000000 starrail-toolkit-0.3.0/starrail/entry/__init__.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     1364 2023-05-02 18:09:52.000000 starrail-toolkit-0.3.0/starrail/entry/cli.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      285 2023-05-02 10:06:31.000000 starrail-toolkit-0.3.0/starrail/entry/gui.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     1211 2023-05-02 18:03:42.000000 starrail-toolkit-0.3.0/starrail/entry/setup.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-02 18:11:20.091412 starrail-toolkit-0.3.0/starrail/gacha/
--rw-r--r--   0 littlenyima   (501) staff       (20)       49 2023-04-30 15:17:38.000000 starrail-toolkit-0.3.0/starrail/gacha/__init__.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     6599 2023-04-30 15:17:38.000000 starrail-toolkit-0.3.0/starrail/gacha/database.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      817 2023-04-30 15:17:38.000000 starrail-toolkit-0.3.0/starrail/gacha/fetch.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     5178 2023-05-02 17:49:24.000000 starrail-toolkit-0.3.0/starrail/gacha/fileio.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     5088 2023-05-02 17:23:42.000000 starrail-toolkit-0.3.0/starrail/gacha/parse.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     3365 2023-05-02 07:38:24.000000 starrail-toolkit-0.3.0/starrail/gacha/service.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      501 2023-04-30 15:17:38.000000 starrail-toolkit-0.3.0/starrail/gacha/type.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     3448 2023-04-30 15:17:38.000000 starrail-toolkit-0.3.0/starrail/gacha/url.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-02 18:11:20.091650 starrail-toolkit-0.3.0/starrail/gui/
--rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-05-01 17:01:35.000000 starrail-toolkit-0.3.0/starrail/gui/__init__.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      183 2023-05-02 10:06:34.000000 starrail-toolkit-0.3.0/starrail/gui/application.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-02 18:11:20.092117 starrail-toolkit-0.3.0/starrail/utils/
--rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-04-30 15:17:38.000000 starrail-toolkit-0.3.0/starrail/utils/__init__.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-02 18:11:20.092664 starrail-toolkit-0.3.0/starrail/utils/babelfish/
--rw-r--r--   0 littlenyima   (501) staff       (20)      408 2023-05-02 17:44:53.000000 starrail-toolkit-0.3.0/starrail/utils/babelfish/__init__.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     1387 2023-05-02 17:50:07.000000 starrail-toolkit-0.3.0/starrail/utils/babelfish/dictionary.py
--rw-r--r--   0 littlenyima   (501) staff       (20)       68 2023-05-02 15:17:12.000000 starrail-toolkit-0.3.0/starrail/utils/babelfish/locale.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      586 2023-05-02 17:37:53.000000 starrail-toolkit-0.3.0/starrail/utils/babelfish/multilingual.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      165 2023-05-02 16:15:22.000000 starrail-toolkit-0.3.0/starrail/utils/babelfish/translate.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      551 2023-05-02 18:03:04.000000 starrail-toolkit-0.3.0/starrail/utils/loggings.py
--rw-r--r--   0 littlenyima   (501) staff       (20)       22 2023-05-02 18:09:46.000000 starrail-toolkit-0.3.0/starrail/version.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-02 18:11:20.093337 starrail-toolkit-0.3.0/starrail_toolkit.egg-info/
--rw-r--r--   0 littlenyima   (501) staff       (20)     3353 2023-05-02 18:11:20.000000 starrail-toolkit-0.3.0/starrail_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 littlenyima   (501) staff       (20)      918 2023-05-02 18:11:20.000000 starrail-toolkit-0.3.0/starrail_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 littlenyima   (501) staff       (20)        1 2023-05-02 18:11:20.000000 starrail-toolkit-0.3.0/starrail_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 littlenyima   (501) staff       (20)       54 2023-05-02 18:11:20.000000 starrail-toolkit-0.3.0/starrail_toolkit.egg-info/entry_points.txt
--rw-r--r--   0 littlenyima   (501) staff       (20)       46 2023-05-02 18:11:20.000000 starrail-toolkit-0.3.0/starrail_toolkit.egg-info/requires.txt
--rw-r--r--   0 littlenyima   (501) staff       (20)        9 2023-05-02 18:11:20.000000 starrail-toolkit-0.3.0/starrail_toolkit.egg-info/top_level.txt
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-04 08:07:26.818370 starrail-toolkit-0.4.0/
+-rw-r--r--   0 littlenyima   (501) staff       (20)    35149 2023-04-29 06:29:57.000000 starrail-toolkit-0.4.0/LICENSE
+-rw-r--r--   0 littlenyima   (501) staff       (20)     4227 2023-05-04 08:07:26.818242 starrail-toolkit-0.4.0/PKG-INFO
+-rw-r--r--   0 littlenyima   (501) staff       (20)     3720 2023-05-04 08:05:55.000000 starrail-toolkit-0.4.0/README.md
+-rw-r--r--   0 littlenyima   (501) staff       (20)       38 2023-05-04 08:07:26.818404 starrail-toolkit-0.4.0/setup.cfg
+-rw-r--r--   0 littlenyima   (501) staff       (20)     4153 2023-04-30 15:17:38.000000 starrail-toolkit-0.4.0/setup.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-04 08:07:26.814707 starrail-toolkit-0.4.0/starrail/
+-rw-r--r--   0 littlenyima   (501) staff       (20)      724 2023-05-01 17:01:35.000000 starrail-toolkit-0.4.0/starrail/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      996 2023-05-02 18:12:29.000000 starrail-toolkit-0.4.0/starrail/config.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-04 08:07:26.815137 starrail-toolkit-0.4.0/starrail/entry/
+-rw-r--r--   0 littlenyima   (501) staff       (20)       49 2023-04-30 15:17:38.000000 starrail-toolkit-0.4.0/starrail/entry/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     1581 2023-05-04 07:54:24.000000 starrail-toolkit-0.4.0/starrail/entry/cli.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      285 2023-05-02 18:12:29.000000 starrail-toolkit-0.4.0/starrail/entry/gui.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     1301 2023-05-04 08:06:33.000000 starrail-toolkit-0.4.0/starrail/entry/setup.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-04 08:07:26.816146 starrail-toolkit-0.4.0/starrail/gacha/
+-rw-r--r--   0 littlenyima   (501) staff       (20)       49 2023-04-30 15:17:38.000000 starrail-toolkit-0.4.0/starrail/gacha/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     3634 2023-05-04 08:06:33.000000 starrail-toolkit-0.4.0/starrail/gacha/autodet.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     6599 2023-04-30 15:17:38.000000 starrail-toolkit-0.4.0/starrail/gacha/database.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      806 2023-05-04 07:39:52.000000 starrail-toolkit-0.4.0/starrail/gacha/fetch.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     5178 2023-05-02 18:12:29.000000 starrail-toolkit-0.4.0/starrail/gacha/fileio.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     5088 2023-05-02 17:23:42.000000 starrail-toolkit-0.4.0/starrail/gacha/parse.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     3400 2023-05-04 08:06:33.000000 starrail-toolkit-0.4.0/starrail/gacha/service.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      501 2023-04-30 15:17:38.000000 starrail-toolkit-0.4.0/starrail/gacha/type.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     3448 2023-04-30 15:17:38.000000 starrail-toolkit-0.4.0/starrail/gacha/url.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-04 08:07:26.816381 starrail-toolkit-0.4.0/starrail/gui/
+-rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-05-01 17:01:35.000000 starrail-toolkit-0.4.0/starrail/gui/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      183 2023-05-02 18:12:29.000000 starrail-toolkit-0.4.0/starrail/gui/application.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-04 08:07:26.816741 starrail-toolkit-0.4.0/starrail/utils/
+-rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-04-30 15:17:38.000000 starrail-toolkit-0.4.0/starrail/utils/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)        6 2023-05-04 03:25:45.000000 starrail-toolkit-0.4.0/starrail/utils/auto_update.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-04 08:07:26.817431 starrail-toolkit-0.4.0/starrail/utils/babelfish/
+-rw-r--r--   0 littlenyima   (501) staff       (20)      408 2023-05-02 18:12:29.000000 starrail-toolkit-0.4.0/starrail/utils/babelfish/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     1387 2023-05-02 18:12:29.000000 starrail-toolkit-0.4.0/starrail/utils/babelfish/dictionary.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      373 2023-05-04 08:06:33.000000 starrail-toolkit-0.4.0/starrail/utils/babelfish/locale.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      586 2023-05-02 18:12:29.000000 starrail-toolkit-0.4.0/starrail/utils/babelfish/multilingual.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      165 2023-05-02 18:12:29.000000 starrail-toolkit-0.4.0/starrail/utils/babelfish/translate.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      551 2023-05-02 18:12:29.000000 starrail-toolkit-0.4.0/starrail/utils/loggings.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)       22 2023-05-04 07:56:08.000000 starrail-toolkit-0.4.0/starrail/version.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-04 08:07:26.818081 starrail-toolkit-0.4.0/starrail_toolkit.egg-info/
+-rw-r--r--   0 littlenyima   (501) staff       (20)     4227 2023-05-04 08:07:26.000000 starrail-toolkit-0.4.0/starrail_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 littlenyima   (501) staff       (20)      974 2023-05-04 08:07:26.000000 starrail-toolkit-0.4.0/starrail_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 littlenyima   (501) staff       (20)        1 2023-05-04 08:07:26.000000 starrail-toolkit-0.4.0/starrail_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 littlenyima   (501) staff       (20)       54 2023-05-04 08:07:26.000000 starrail-toolkit-0.4.0/starrail_toolkit.egg-info/entry_points.txt
+-rw-r--r--   0 littlenyima   (501) staff       (20)       46 2023-05-04 08:07:26.000000 starrail-toolkit-0.4.0/starrail_toolkit.egg-info/requires.txt
+-rw-r--r--   0 littlenyima   (501) staff       (20)        9 2023-05-04 08:07:26.000000 starrail-toolkit-0.4.0/starrail_toolkit.egg-info/top_level.txt
```

### Comparing `starrail-toolkit-0.3.0/LICENSE` & `starrail-toolkit-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.3.0/PKG-INFO` & `starrail-toolkit-0.4.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,46 +1,31 @@
-Metadata-Version: 2.1
-Name: starrail-toolkit
-Version: 0.3.0
-Summary: Honkai Star Rail Toolkit
-Home-page: https://github.com/LittleNyima/honkai-starrail-toolkit
-Author: LittleNyima
-Author-email: littlenyima@163.com
-License: GPLv3
-Classifier: Development Status :: 4 - Beta
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # 《崩坏：星穹铁道》工具箱
 
 <div align="center">
 <img src="https://s1.ax1x.com/2023/04/30/p98Cv26.png" alt="logo" />
 </div>
 
 ## 开发状态
 
 | 主分支版本 | 开发分支版本 | PyPI 版本 |
 | :--------: | :----------: | :-------: |
-|   0.3.0    |    0.3.0     |   0.3.0   |
+|   0.4.0    |    0.4.0     |   0.4.0   |
 
 - [x] 支持命令行导出 csv、xlsx、json 格式抽卡记录
 - [x] 支持命令行显示抽卡报告
 - [x] 支持导出 markdown 格式抽卡报告
 - [x] 支持导出网页版抽卡报告
 - [x] 支持中英文多语言导出
-- [ ] 支持 Windows 平台游戏中自动检测 API URL
+- [x] 支持 Windows 平台游戏中自动检测 API URL
 - [ ] 实现用户界面并编译到 Windows 与 macOS 平台
 - [ ] 支持自动检查更新
 
 ## 安装方式
 
-目前仅提供命令行版本，用户交互界面版本正在开发中。
+目前仅提供命令行版本（*我会尽快编译一个可以直接下载运行的应用程序版本*），用户交互界面版本正在开发中。
 
 ### 命令行安装
 
 Python 用户可以直接使用 pip 安装本工具：
 
 ```shell
 pip install starrail-toolkit --upgrade -i https://pypi.tuna.tsinghua.edu.cn/simple
@@ -58,35 +43,41 @@
 
 ## 使用指南
 
 ### 获取抽卡查询 API URL
 
 请参考[【这个教程】](docs/how-to-get-api-url.md)获取查询链接。
 
-由此可以获得一个形如 `https://api-takumi.mihoyo.com/common/gacha_record/api/getGachaLog?xxxxx` 的 URL，后续步骤使用的就是这个 URL。注意：API URL 会在一定时间后过期，过期后需要重新获取。
+由此可以获得一个形如 `https://api-takumi.mihoyo.com/common/gacha_record/api/getGachaLog?xxxxx` 的 URL，后续步骤使用的就是这个 URL。注意：API URL 会在一定时间（大约 24 小时）后过期，过期后需要重新获取。
+
+**注：若为 Windows 平台，可以使用本工具自动检测 API URL。**首先登陆游戏，进入抽卡查询页面，当显示出一页抽卡查询结果后，运行本工具，即可检测到抽卡查询 URL。如果需要切换账号，建议使用上述教程中的方法获取每个账号的 API URL，以便精确控制导出的账号。
 
 ### 导出抽卡记录
 
 #### 命令行导出
 
 可以使用如下命令导出：
 
 ```shell
 hksr --api https://api-takumi.mihoyo.com/xxx
 ```
 
 **参数说明：**
 
-- `--api`：（必选）API URL 地址。*注：未来将支持自动获取 API URL，届时本参数将变为可选。*
+- `--api`：（Windows 平台可选）API URL 地址。若为 Windows 平台，可以不填这个参数，而使用自动检测功能。
 - `--export`：（可选）导出格式选项。默认为导出全部格式，若仅需导出部分格式，可以替换对应参数。目前支持的格式有 `csv`、`html`、`json`、`md`、`xlsx`。例如，若只需要 json 与 xlsx 格式数据，可以替换为 `--export json xlsx`。
 - `--locale`：（可选）控制输出语言。默认为输出简体中文，可选值为 `en`（英语）、`chs`（简体中文）。
-- `--log-level`：（可选）日志等级。控制日志的输出等级，默认为 `DEBUG`。若感觉输出的日志过多影响观感，建议将日志等级更改为 `INFO`，例如：`--log-level INFO`。从高到低的可选值为 `CRITICAL`、`ERROR`、`WARNING`、`INFO`、`DEBUG`。
+- `--log-level`：（可选）日志等级。控制日志的输出等级，默认为 `DEBUG`。若感觉输出的日志过多影响观感，建议将日志等级更改为 `INFO`，例如：`--log-level INFO`。（注意：若设置的日志等级过高，可能导致基本的信息无法显示，例如导出进度、导出位置、命令行版抽卡报告等）从高到低的可选值为 `CRITICAL`、`ERROR`、`WARNING`、`INFO`、`DEBUG`。
 
 ## 导出结果示例
 
 - Excel 结果示例（为保护隐私已隐藏部分信息）
 
   <img src="https://s1.ax1x.com/2023/05/02/p9GJKts.png" alt="xlsx" style="width: 600px;" />
 
 - Markdown 结果示例：
 
   <img src="https://s1.ax1x.com/2023/05/02/p9GYNKf.png" alt="markdown" style="width: 600px;" />
+
+## 安全提醒
+
+本仓库代码完全开源，且用户数据全部保存在本地，**本项目不会上传任何用户数据**。本项目仅在该 GitHub 仓库及 PyPI 进行分发，请仔细甄别下载到的程序，防止遭遇恶意程序。
```

### Comparing `starrail-toolkit-0.3.0/setup.py` & `starrail-toolkit-0.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.3.0/starrail/__init__.py` & `starrail-toolkit-0.4.0/starrail/__init__.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.3.0/starrail/config.py` & `starrail-toolkit-0.4.0/starrail/config.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.3.0/starrail/entry/cli.py` & `starrail-toolkit-0.4.0/starrail/entry/cli.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import argparse
+import traceback
 
 from starrail.config import configuration as cfg
 from starrail.entry.setup import setup
 from starrail.gacha.service import export_gacha_from_api
 from starrail.utils import loggings
 
 logger = loggings.get_logger(__file__)
@@ -14,15 +15,15 @@
         description='Honkai: Star Rail Toolkit',
     )
     parser.add_argument(
         '--api', type=str,
         help='URL of the gacha api, please refer to README.md for details.',
     )
     parser.add_argument(
-        '--export', nargs='+', type=str,
+        '--export', nargs='+', type=str, default=['all'],
         choices=['all', 'csv', 'html', 'json', 'md', 'xlsx'],
         help='Types of expected export formats.',
     )
     parser.add_argument(
         '--locale', type=str, default='zhs',
         choices=['en', 'zhs'],
         help=(
@@ -37,11 +38,20 @@
     )
 
     return parser.parse_args()
 
 
 def cli_entry():
     args = parse_args()
-    setup(log_level=args.log_level)
+    setup(log_level=args.log_level, locale=args.locale)
     logger.info(args)
     logger.info(cfg)
     export_gacha_from_api(api_url=args.api, export=args.export)
+
+
+if __name__ == '__main__':
+    try:
+        cli_entry()
+    except Exception:
+        traceback.print_exc()
+    finally:
+        input('Press `Enter` to exit.')
```

### Comparing `starrail-toolkit-0.3.0/starrail/gacha/database.py` & `starrail-toolkit-0.4.0/starrail/gacha/database.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.3.0/starrail/gacha/fetch.py` & `starrail-toolkit-0.4.0/starrail/gacha/fetch.py`

 * *Files 11% similar despite different names*

```diff
@@ -24,8 +24,8 @@
         if 200 <= r.status_code < 300:
             content = r.content.decode('utf-8')
             payload = json.loads(content)
             logger.debug(json.dumps(payload, ensure_ascii=False, indent=2))
             return payload, r.status_code
     except Exception:
         traceback.print_exc()
-    return None, r.status_code
+    return None, -1
```

### Comparing `starrail-toolkit-0.3.0/starrail/gacha/fileio.py` & `starrail-toolkit-0.4.0/starrail/gacha/fileio.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.3.0/starrail/gacha/parse.py` & `starrail-toolkit-0.4.0/starrail/gacha/parse.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.3.0/starrail/gacha/service.py` & `starrail-toolkit-0.4.0/starrail/gacha/service.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import os
 from datetime import datetime
 
 import starrail.gacha.fileio as fileio
+from starrail.gacha.autodet import detect_api_url
 from starrail.gacha.fetch import fetch_json
 from starrail.gacha.parse import GachaDataManager
 from starrail.gacha.type import GachaType
 from starrail.gacha.url import get_api_url, get_url_template
 from starrail.utils import loggings
 
 logger = loggings.get_logger(__file__)
@@ -55,20 +56,21 @@
         data_list = response['data']['list']
         r.extend(data_list)
         end_id = data_list[-1]['id']
     return r
 
 
 def export_gacha_from_api(api_url, export):
-    assert api_url, 'API URL should be provided, auto-detect is coming soon'
+    if not api_url:
+        api_url = detect_api_url()
     response, code = fetch_json(api_url)
     valid = check_response(response, code)
     if not valid:
         logger.fatal('Error while checking response from api URL, exitting')
-        raise ValueError('Invalid api URL, please check your input')
+        raise ValueError('Invalid or expired api, please check your input')
 
     api_template = get_url_template(api_url)
 
     uid = response['data']['list'][0]['uid']
     manager = GachaDataManager(uid)
     logger.info(f'Successfully connected to cache of uid {uid}')
     manager.log_stats()
```

### Comparing `starrail-toolkit-0.3.0/starrail/gacha/url.py` & `starrail-toolkit-0.4.0/starrail/gacha/url.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.3.0/starrail/utils/babelfish/dictionary.py` & `starrail-toolkit-0.4.0/starrail/utils/babelfish/dictionary.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.3.0/starrail/utils/babelfish/multilingual.py` & `starrail-toolkit-0.4.0/starrail/utils/babelfish/multilingual.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.3.0/starrail/utils/loggings.py` & `starrail-toolkit-0.4.0/starrail/utils/loggings.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.3.0/starrail_toolkit.egg-info/PKG-INFO` & `starrail-toolkit-0.4.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starrail-toolkit
-Version: 0.3.0
+Version: 0.4.0
 Summary: Honkai Star Rail Toolkit
 Home-page: https://github.com/LittleNyima/honkai-starrail-toolkit
 Author: LittleNyima
 Author-email: littlenyima@163.com
 License: GPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -19,28 +19,28 @@
 <img src="https://s1.ax1x.com/2023/04/30/p98Cv26.png" alt="logo" />
 </div>
 
 ## 开发状态
 
 | 主分支版本 | 开发分支版本 | PyPI 版本 |
 | :--------: | :----------: | :-------: |
-|   0.3.0    |    0.3.0     |   0.3.0   |
+|   0.4.0    |    0.4.0     |   0.4.0   |
 
 - [x] 支持命令行导出 csv、xlsx、json 格式抽卡记录
 - [x] 支持命令行显示抽卡报告
 - [x] 支持导出 markdown 格式抽卡报告
 - [x] 支持导出网页版抽卡报告
 - [x] 支持中英文多语言导出
-- [ ] 支持 Windows 平台游戏中自动检测 API URL
+- [x] 支持 Windows 平台游戏中自动检测 API URL
 - [ ] 实现用户界面并编译到 Windows 与 macOS 平台
 - [ ] 支持自动检查更新
 
 ## 安装方式
 
-目前仅提供命令行版本，用户交互界面版本正在开发中。
+目前仅提供命令行版本（*我会尽快编译一个可以直接下载运行的应用程序版本*），用户交互界面版本正在开发中。
 
 ### 命令行安装
 
 Python 用户可以直接使用 pip 安装本工具：
 
 ```shell
 pip install starrail-toolkit --upgrade -i https://pypi.tuna.tsinghua.edu.cn/simple
@@ -58,35 +58,41 @@
 
 ## 使用指南
 
 ### 获取抽卡查询 API URL
 
 请参考[【这个教程】](docs/how-to-get-api-url.md)获取查询链接。
 
-由此可以获得一个形如 `https://api-takumi.mihoyo.com/common/gacha_record/api/getGachaLog?xxxxx` 的 URL，后续步骤使用的就是这个 URL。注意：API URL 会在一定时间后过期，过期后需要重新获取。
+由此可以获得一个形如 `https://api-takumi.mihoyo.com/common/gacha_record/api/getGachaLog?xxxxx` 的 URL，后续步骤使用的就是这个 URL。注意：API URL 会在一定时间（大约 24 小时）后过期，过期后需要重新获取。
+
+**注：若为 Windows 平台，可以使用本工具自动检测 API URL。**首先登陆游戏，进入抽卡查询页面，当显示出一页抽卡查询结果后，运行本工具，即可检测到抽卡查询 URL。如果需要切换账号，建议使用上述教程中的方法获取每个账号的 API URL，以便精确控制导出的账号。
 
 ### 导出抽卡记录
 
 #### 命令行导出
 
 可以使用如下命令导出：
 
 ```shell
 hksr --api https://api-takumi.mihoyo.com/xxx
 ```
 
 **参数说明：**
 
-- `--api`：（必选）API URL 地址。*注：未来将支持自动获取 API URL，届时本参数将变为可选。*
+- `--api`：（Windows 平台可选）API URL 地址。若为 Windows 平台，可以不填这个参数，而使用自动检测功能。
 - `--export`：（可选）导出格式选项。默认为导出全部格式，若仅需导出部分格式，可以替换对应参数。目前支持的格式有 `csv`、`html`、`json`、`md`、`xlsx`。例如，若只需要 json 与 xlsx 格式数据，可以替换为 `--export json xlsx`。
 - `--locale`：（可选）控制输出语言。默认为输出简体中文，可选值为 `en`（英语）、`chs`（简体中文）。
-- `--log-level`：（可选）日志等级。控制日志的输出等级，默认为 `DEBUG`。若感觉输出的日志过多影响观感，建议将日志等级更改为 `INFO`，例如：`--log-level INFO`。从高到低的可选值为 `CRITICAL`、`ERROR`、`WARNING`、`INFO`、`DEBUG`。
+- `--log-level`：（可选）日志等级。控制日志的输出等级，默认为 `DEBUG`。若感觉输出的日志过多影响观感，建议将日志等级更改为 `INFO`，例如：`--log-level INFO`。（注意：若设置的日志等级过高，可能导致基本的信息无法显示，例如导出进度、导出位置、命令行版抽卡报告等）从高到低的可选值为 `CRITICAL`、`ERROR`、`WARNING`、`INFO`、`DEBUG`。
 
 ## 导出结果示例
 
 - Excel 结果示例（为保护隐私已隐藏部分信息）
 
   <img src="https://s1.ax1x.com/2023/05/02/p9GJKts.png" alt="xlsx" style="width: 600px;" />
 
 - Markdown 结果示例：
 
   <img src="https://s1.ax1x.com/2023/05/02/p9GYNKf.png" alt="markdown" style="width: 600px;" />
+
+## 安全提醒
+
+本仓库代码完全开源，且用户数据全部保存在本地，**本项目不会上传任何用户数据**。本项目仅在该 GitHub 仓库及 PyPI 进行分发，请仔细甄别下载到的程序，防止遭遇恶意程序。
```

### Comparing `starrail-toolkit-0.3.0/starrail_toolkit.egg-info/SOURCES.txt` & `starrail-toolkit-0.4.0/starrail_toolkit.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -5,24 +5,26 @@
 starrail/config.py
 starrail/version.py
 starrail/entry/__init__.py
 starrail/entry/cli.py
 starrail/entry/gui.py
 starrail/entry/setup.py
 starrail/gacha/__init__.py
+starrail/gacha/autodet.py
 starrail/gacha/database.py
 starrail/gacha/fetch.py
 starrail/gacha/fileio.py
 starrail/gacha/parse.py
 starrail/gacha/service.py
 starrail/gacha/type.py
 starrail/gacha/url.py
 starrail/gui/__init__.py
 starrail/gui/application.py
 starrail/utils/__init__.py
+starrail/utils/auto_update.py
 starrail/utils/loggings.py
 starrail/utils/babelfish/__init__.py
 starrail/utils/babelfish/dictionary.py
 starrail/utils/babelfish/locale.py
 starrail/utils/babelfish/multilingual.py
 starrail/utils/babelfish/translate.py
 starrail_toolkit.egg-info/PKG-INFO
```

