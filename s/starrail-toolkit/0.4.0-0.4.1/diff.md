# Comparing `tmp/starrail-toolkit-0.4.0.tar.gz` & `tmp/starrail-toolkit-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starrail-toolkit-0.4.0.tar", last modified: Thu May  4 08:07:26 2023, max compression
+gzip compressed data, was "starrail-toolkit-0.4.1.tar", last modified: Thu May  4 18:30:41 2023, max compression
```

## Comparing `starrail-toolkit-0.4.0.tar` & `starrail-toolkit-0.4.1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-04 08:07:26.818370 starrail-toolkit-0.4.0/
--rw-r--r--   0 littlenyima   (501) staff       (20)    35149 2023-04-29 06:29:57.000000 starrail-toolkit-0.4.0/LICENSE
--rw-r--r--   0 littlenyima   (501) staff       (20)     4227 2023-05-04 08:07:26.818242 starrail-toolkit-0.4.0/PKG-INFO
--rw-r--r--   0 littlenyima   (501) staff       (20)     3720 2023-05-04 08:05:55.000000 starrail-toolkit-0.4.0/README.md
--rw-r--r--   0 littlenyima   (501) staff       (20)       38 2023-05-04 08:07:26.818404 starrail-toolkit-0.4.0/setup.cfg
--rw-r--r--   0 littlenyima   (501) staff       (20)     4153 2023-04-30 15:17:38.000000 starrail-toolkit-0.4.0/setup.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-04 08:07:26.814707 starrail-toolkit-0.4.0/starrail/
--rw-r--r--   0 littlenyima   (501) staff       (20)      724 2023-05-01 17:01:35.000000 starrail-toolkit-0.4.0/starrail/__init__.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      996 2023-05-02 18:12:29.000000 starrail-toolkit-0.4.0/starrail/config.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-04 08:07:26.815137 starrail-toolkit-0.4.0/starrail/entry/
--rw-r--r--   0 littlenyima   (501) staff       (20)       49 2023-04-30 15:17:38.000000 starrail-toolkit-0.4.0/starrail/entry/__init__.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     1581 2023-05-04 07:54:24.000000 starrail-toolkit-0.4.0/starrail/entry/cli.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      285 2023-05-02 18:12:29.000000 starrail-toolkit-0.4.0/starrail/entry/gui.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     1301 2023-05-04 08:06:33.000000 starrail-toolkit-0.4.0/starrail/entry/setup.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-04 08:07:26.816146 starrail-toolkit-0.4.0/starrail/gacha/
--rw-r--r--   0 littlenyima   (501) staff       (20)       49 2023-04-30 15:17:38.000000 starrail-toolkit-0.4.0/starrail/gacha/__init__.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     3634 2023-05-04 08:06:33.000000 starrail-toolkit-0.4.0/starrail/gacha/autodet.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     6599 2023-04-30 15:17:38.000000 starrail-toolkit-0.4.0/starrail/gacha/database.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      806 2023-05-04 07:39:52.000000 starrail-toolkit-0.4.0/starrail/gacha/fetch.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     5178 2023-05-02 18:12:29.000000 starrail-toolkit-0.4.0/starrail/gacha/fileio.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     5088 2023-05-02 17:23:42.000000 starrail-toolkit-0.4.0/starrail/gacha/parse.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     3400 2023-05-04 08:06:33.000000 starrail-toolkit-0.4.0/starrail/gacha/service.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      501 2023-04-30 15:17:38.000000 starrail-toolkit-0.4.0/starrail/gacha/type.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     3448 2023-04-30 15:17:38.000000 starrail-toolkit-0.4.0/starrail/gacha/url.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-04 08:07:26.816381 starrail-toolkit-0.4.0/starrail/gui/
--rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-05-01 17:01:35.000000 starrail-toolkit-0.4.0/starrail/gui/__init__.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      183 2023-05-02 18:12:29.000000 starrail-toolkit-0.4.0/starrail/gui/application.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-04 08:07:26.816741 starrail-toolkit-0.4.0/starrail/utils/
--rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-04-30 15:17:38.000000 starrail-toolkit-0.4.0/starrail/utils/__init__.py
--rw-r--r--   0 littlenyima   (501) staff       (20)        6 2023-05-04 03:25:45.000000 starrail-toolkit-0.4.0/starrail/utils/auto_update.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-04 08:07:26.817431 starrail-toolkit-0.4.0/starrail/utils/babelfish/
--rw-r--r--   0 littlenyima   (501) staff       (20)      408 2023-05-02 18:12:29.000000 starrail-toolkit-0.4.0/starrail/utils/babelfish/__init__.py
--rw-r--r--   0 littlenyima   (501) staff       (20)     1387 2023-05-02 18:12:29.000000 starrail-toolkit-0.4.0/starrail/utils/babelfish/dictionary.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      373 2023-05-04 08:06:33.000000 starrail-toolkit-0.4.0/starrail/utils/babelfish/locale.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      586 2023-05-02 18:12:29.000000 starrail-toolkit-0.4.0/starrail/utils/babelfish/multilingual.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      165 2023-05-02 18:12:29.000000 starrail-toolkit-0.4.0/starrail/utils/babelfish/translate.py
--rw-r--r--   0 littlenyima   (501) staff       (20)      551 2023-05-02 18:12:29.000000 starrail-toolkit-0.4.0/starrail/utils/loggings.py
--rw-r--r--   0 littlenyima   (501) staff       (20)       22 2023-05-04 07:56:08.000000 starrail-toolkit-0.4.0/starrail/version.py
-drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-04 08:07:26.818081 starrail-toolkit-0.4.0/starrail_toolkit.egg-info/
--rw-r--r--   0 littlenyima   (501) staff       (20)     4227 2023-05-04 08:07:26.000000 starrail-toolkit-0.4.0/starrail_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 littlenyima   (501) staff       (20)      974 2023-05-04 08:07:26.000000 starrail-toolkit-0.4.0/starrail_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 littlenyima   (501) staff       (20)        1 2023-05-04 08:07:26.000000 starrail-toolkit-0.4.0/starrail_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 littlenyima   (501) staff       (20)       54 2023-05-04 08:07:26.000000 starrail-toolkit-0.4.0/starrail_toolkit.egg-info/entry_points.txt
--rw-r--r--   0 littlenyima   (501) staff       (20)       46 2023-05-04 08:07:26.000000 starrail-toolkit-0.4.0/starrail_toolkit.egg-info/requires.txt
--rw-r--r--   0 littlenyima   (501) staff       (20)        9 2023-05-04 08:07:26.000000 starrail-toolkit-0.4.0/starrail_toolkit.egg-info/top_level.txt
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-04 18:30:41.691133 starrail-toolkit-0.4.1/
+-rw-r--r--   0 littlenyima   (501) staff       (20)    35149 2023-05-04 18:27:16.000000 starrail-toolkit-0.4.1/LICENSE
+-rw-r--r--   0 littlenyima   (501) staff       (20)     4593 2023-05-04 18:30:41.690971 starrail-toolkit-0.4.1/PKG-INFO
+-rw-r--r--   0 littlenyima   (501) staff       (20)     4086 2023-05-04 18:22:59.000000 starrail-toolkit-0.4.1/README.md
+-rw-r--r--   0 littlenyima   (501) staff       (20)       38 2023-05-04 18:30:41.691312 starrail-toolkit-0.4.1/setup.cfg
+-rw-r--r--   0 littlenyima   (501) staff       (20)     4153 2023-05-04 18:27:16.000000 starrail-toolkit-0.4.1/setup.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-04 18:30:41.686674 starrail-toolkit-0.4.1/starrail/
+-rw-r--r--   0 littlenyima   (501) staff       (20)      724 2023-05-04 18:27:16.000000 starrail-toolkit-0.4.1/starrail/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      996 2023-05-04 18:27:16.000000 starrail-toolkit-0.4.1/starrail/config.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-04 18:30:41.687245 starrail-toolkit-0.4.1/starrail/entry/
+-rw-r--r--   0 littlenyima   (501) staff       (20)       49 2023-05-04 18:27:16.000000 starrail-toolkit-0.4.1/starrail/entry/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     1581 2023-05-04 18:27:16.000000 starrail-toolkit-0.4.1/starrail/entry/cli.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      285 2023-05-04 18:27:16.000000 starrail-toolkit-0.4.1/starrail/entry/gui.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     1301 2023-05-04 18:27:16.000000 starrail-toolkit-0.4.1/starrail/entry/setup.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-04 18:30:41.688566 starrail-toolkit-0.4.1/starrail/gacha/
+-rw-r--r--   0 littlenyima   (501) staff       (20)       49 2023-05-04 18:27:16.000000 starrail-toolkit-0.4.1/starrail/gacha/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     3636 2023-05-04 18:29:24.000000 starrail-toolkit-0.4.1/starrail/gacha/autodet.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     6599 2023-05-04 18:27:16.000000 starrail-toolkit-0.4.1/starrail/gacha/database.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      806 2023-05-04 18:27:16.000000 starrail-toolkit-0.4.1/starrail/gacha/fetch.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     5178 2023-05-04 18:27:16.000000 starrail-toolkit-0.4.1/starrail/gacha/fileio.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     5088 2023-05-04 18:27:16.000000 starrail-toolkit-0.4.1/starrail/gacha/parse.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     3400 2023-05-04 18:27:16.000000 starrail-toolkit-0.4.1/starrail/gacha/service.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      501 2023-05-04 18:27:16.000000 starrail-toolkit-0.4.1/starrail/gacha/type.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     3448 2023-05-04 18:27:16.000000 starrail-toolkit-0.4.1/starrail/gacha/url.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-04 18:30:41.688840 starrail-toolkit-0.4.1/starrail/gui/
+-rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-05-04 18:27:16.000000 starrail-toolkit-0.4.1/starrail/gui/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      183 2023-05-04 18:27:16.000000 starrail-toolkit-0.4.1/starrail/gui/application.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-04 18:30:41.689234 starrail-toolkit-0.4.1/starrail/utils/
+-rw-r--r--   0 littlenyima   (501) staff       (20)        0 2023-05-04 18:27:16.000000 starrail-toolkit-0.4.1/starrail/utils/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)        6 2023-05-04 18:27:16.000000 starrail-toolkit-0.4.1/starrail/utils/auto_update.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-04 18:30:41.689885 starrail-toolkit-0.4.1/starrail/utils/babelfish/
+-rw-r--r--   0 littlenyima   (501) staff       (20)      408 2023-05-04 18:27:16.000000 starrail-toolkit-0.4.1/starrail/utils/babelfish/__init__.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)     1387 2023-05-04 18:27:16.000000 starrail-toolkit-0.4.1/starrail/utils/babelfish/dictionary.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      373 2023-05-04 18:27:16.000000 starrail-toolkit-0.4.1/starrail/utils/babelfish/locale.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      586 2023-05-04 18:27:16.000000 starrail-toolkit-0.4.1/starrail/utils/babelfish/multilingual.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      165 2023-05-04 18:27:16.000000 starrail-toolkit-0.4.1/starrail/utils/babelfish/translate.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)      551 2023-05-04 18:27:16.000000 starrail-toolkit-0.4.1/starrail/utils/loggings.py
+-rw-r--r--   0 littlenyima   (501) staff       (20)       22 2023-05-04 18:28:29.000000 starrail-toolkit-0.4.1/starrail/version.py
+drwxr-xr-x   0 littlenyima   (501) staff       (20)        0 2023-05-04 18:30:41.690749 starrail-toolkit-0.4.1/starrail_toolkit.egg-info/
+-rw-r--r--   0 littlenyima   (501) staff       (20)     4593 2023-05-04 18:30:41.000000 starrail-toolkit-0.4.1/starrail_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 littlenyima   (501) staff       (20)      974 2023-05-04 18:30:41.000000 starrail-toolkit-0.4.1/starrail_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 littlenyima   (501) staff       (20)        1 2023-05-04 18:30:41.000000 starrail-toolkit-0.4.1/starrail_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 littlenyima   (501) staff       (20)       54 2023-05-04 18:30:41.000000 starrail-toolkit-0.4.1/starrail_toolkit.egg-info/entry_points.txt
+-rw-r--r--   0 littlenyima   (501) staff       (20)       46 2023-05-04 18:30:41.000000 starrail-toolkit-0.4.1/starrail_toolkit.egg-info/requires.txt
+-rw-r--r--   0 littlenyima   (501) staff       (20)        9 2023-05-04 18:30:41.000000 starrail-toolkit-0.4.1/starrail_toolkit.egg-info/top_level.txt
```

### Comparing `starrail-toolkit-0.4.0/LICENSE` & `starrail-toolkit-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.4.0/PKG-INFO` & `starrail-toolkit-0.4.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,18 @@
-Metadata-Version: 2.1
-Name: starrail-toolkit
-Version: 0.4.0
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
-|   0.4.0    |    0.4.0     |   0.4.0   |
+|   0.4.0    |    0.4.1     |   0.4.1   |
 
 - [x] 支持命令行导出 csv、xlsx、json 格式抽卡记录
 - [x] 支持命令行显示抽卡报告
 - [x] 支持导出 markdown 格式抽卡报告
 - [x] 支持导出网页版抽卡报告
 - [x] 支持中英文多语言导出
 - [x] 支持 Windows 平台游戏中自动检测 API URL
@@ -39,54 +24,63 @@
 目前仅提供命令行版本（*我会尽快编译一个可以直接下载运行的应用程序版本*），用户交互界面版本正在开发中。
 
 ### 命令行安装
 
 Python 用户可以直接使用 pip 安装本工具：
 
 ```shell
-pip install starrail-toolkit --upgrade -i https://pypi.tuna.tsinghua.edu.cn/simple
+python3 -m pip install starrail-toolkit --upgrade -i https://pypi.tuna.tsinghua.edu.cn/simple
 ```
 
 ### 从源码安装
 
 若需要使用尚未推送到 PyPI 版本的功能，可通过源码安装：
 
 ```shell
 git clone git@github.com:LittleNyima/honkai-starrail-toolkit.git
 cd honkai-starrail-toolkit
-python setup.py install
+python3 setup.py install
 ```
 
 ## 使用指南
 
 ### 获取抽卡查询 API URL
 
 请参考[【这个教程】](docs/how-to-get-api-url.md)获取查询链接。
 
 由此可以获得一个形如 `https://api-takumi.mihoyo.com/common/gacha_record/api/getGachaLog?xxxxx` 的 URL，后续步骤使用的就是这个 URL。注意：API URL 会在一定时间（大约 24 小时）后过期，过期后需要重新获取。
 
-**注：若为 Windows 平台，可以使用本工具自动检测 API URL。**首先登陆游戏，进入抽卡查询页面，当显示出一页抽卡查询结果后，运行本工具，即可检测到抽卡查询 URL。如果需要切换账号，建议使用上述教程中的方法获取每个账号的 API URL，以便精确控制导出的账号。
+**注：若为 Windows 平台，可以使用本工具自动检测 API URL。** 首先登陆游戏，进入抽卡查询页面，当显示出一页抽卡查询结果后，运行本工具，即可检测到抽卡查询 URL。如果需要切换账号，建议使用上述教程中的方法获取每个账号的 API URL，以便精确控制导出的账号。
 
 ### 导出抽卡记录
 
 #### 命令行导出
 
 可以使用如下命令导出：
 
 ```shell
+# 非 Windows 平台
 hksr --api https://api-takumi.mihoyo.com/xxx
+# Windows 平台无需 --api 参数
+hksr
 ```
 
 **参数说明：**
 
 - `--api`：（Windows 平台可选）API URL 地址。若为 Windows 平台，可以不填这个参数，而使用自动检测功能。
 - `--export`：（可选）导出格式选项。默认为导出全部格式，若仅需导出部分格式，可以替换对应参数。目前支持的格式有 `csv`、`html`、`json`、`md`、`xlsx`。例如，若只需要 json 与 xlsx 格式数据，可以替换为 `--export json xlsx`。
 - `--locale`：（可选）控制输出语言。默认为输出简体中文，可选值为 `en`（英语）、`chs`（简体中文）。
 - `--log-level`：（可选）日志等级。控制日志的输出等级，默认为 `DEBUG`。若感觉输出的日志过多影响观感，建议将日志等级更改为 `INFO`，例如：`--log-level INFO`。（注意：若设置的日志等级过高，可能导致基本的信息无法显示，例如导出进度、导出位置、命令行版抽卡报告等）从高到低的可选值为 `CRITICAL`、`ERROR`、`WARNING`、`INFO`、`DEBUG`。
 
+本项目目前正处于快速迭代阶段，使用方式可能会发生改变，更新时请留意本部分关于使用方式的说明。
+
+### Troubleshooting
+
+- 遇到 `PermissionError: [Errno 13] Permission denied`：应该是因为缓存文件被占用，建议退出游戏后重试。
+
 ## 导出结果示例
 
 - Excel 结果示例（为保护隐私已隐藏部分信息）
 
   <img src="https://s1.ax1x.com/2023/05/02/p9GJKts.png" alt="xlsx" style="width: 600px;" />
 
 - Markdown 结果示例：
```

### Comparing `starrail-toolkit-0.4.0/README.md` & `starrail-toolkit-0.4.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,33 @@
+Metadata-Version: 2.1
+Name: starrail-toolkit
+Version: 0.4.1
+Summary: Honkai Star Rail Toolkit
+Home-page: https://github.com/LittleNyima/honkai-starrail-toolkit
+Author: LittleNyima
+Author-email: littlenyima@163.com
+License: GPLv3
+Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # 《崩坏：星穹铁道》工具箱
 
 <div align="center">
 <img src="https://s1.ax1x.com/2023/04/30/p98Cv26.png" alt="logo" />
 </div>
 
 ## 开发状态
 
 | 主分支版本 | 开发分支版本 | PyPI 版本 |
 | :--------: | :----------: | :-------: |
-|   0.4.0    |    0.4.0     |   0.4.0   |
+|   0.4.0    |    0.4.1     |   0.4.1   |
 
 - [x] 支持命令行导出 csv、xlsx、json 格式抽卡记录
 - [x] 支持命令行显示抽卡报告
 - [x] 支持导出 markdown 格式抽卡报告
 - [x] 支持导出网页版抽卡报告
 - [x] 支持中英文多语言导出
 - [x] 支持 Windows 平台游戏中自动检测 API URL
@@ -24,54 +39,63 @@
 目前仅提供命令行版本（*我会尽快编译一个可以直接下载运行的应用程序版本*），用户交互界面版本正在开发中。
 
 ### 命令行安装
 
 Python 用户可以直接使用 pip 安装本工具：
 
 ```shell
-pip install starrail-toolkit --upgrade -i https://pypi.tuna.tsinghua.edu.cn/simple
+python3 -m pip install starrail-toolkit --upgrade -i https://pypi.tuna.tsinghua.edu.cn/simple
 ```
 
 ### 从源码安装
 
 若需要使用尚未推送到 PyPI 版本的功能，可通过源码安装：
 
 ```shell
 git clone git@github.com:LittleNyima/honkai-starrail-toolkit.git
 cd honkai-starrail-toolkit
-python setup.py install
+python3 setup.py install
 ```
 
 ## 使用指南
 
 ### 获取抽卡查询 API URL
 
 请参考[【这个教程】](docs/how-to-get-api-url.md)获取查询链接。
 
 由此可以获得一个形如 `https://api-takumi.mihoyo.com/common/gacha_record/api/getGachaLog?xxxxx` 的 URL，后续步骤使用的就是这个 URL。注意：API URL 会在一定时间（大约 24 小时）后过期，过期后需要重新获取。
 
-**注：若为 Windows 平台，可以使用本工具自动检测 API URL。**首先登陆游戏，进入抽卡查询页面，当显示出一页抽卡查询结果后，运行本工具，即可检测到抽卡查询 URL。如果需要切换账号，建议使用上述教程中的方法获取每个账号的 API URL，以便精确控制导出的账号。
+**注：若为 Windows 平台，可以使用本工具自动检测 API URL。** 首先登陆游戏，进入抽卡查询页面，当显示出一页抽卡查询结果后，运行本工具，即可检测到抽卡查询 URL。如果需要切换账号，建议使用上述教程中的方法获取每个账号的 API URL，以便精确控制导出的账号。
 
 ### 导出抽卡记录
 
 #### 命令行导出
 
 可以使用如下命令导出：
 
 ```shell
+# 非 Windows 平台
 hksr --api https://api-takumi.mihoyo.com/xxx
+# Windows 平台无需 --api 参数
+hksr
 ```
 
 **参数说明：**
 
 - `--api`：（Windows 平台可选）API URL 地址。若为 Windows 平台，可以不填这个参数，而使用自动检测功能。
 - `--export`：（可选）导出格式选项。默认为导出全部格式，若仅需导出部分格式，可以替换对应参数。目前支持的格式有 `csv`、`html`、`json`、`md`、`xlsx`。例如，若只需要 json 与 xlsx 格式数据，可以替换为 `--export json xlsx`。
 - `--locale`：（可选）控制输出语言。默认为输出简体中文，可选值为 `en`（英语）、`chs`（简体中文）。
 - `--log-level`：（可选）日志等级。控制日志的输出等级，默认为 `DEBUG`。若感觉输出的日志过多影响观感，建议将日志等级更改为 `INFO`，例如：`--log-level INFO`。（注意：若设置的日志等级过高，可能导致基本的信息无法显示，例如导出进度、导出位置、命令行版抽卡报告等）从高到低的可选值为 `CRITICAL`、`ERROR`、`WARNING`、`INFO`、`DEBUG`。
 
+本项目目前正处于快速迭代阶段，使用方式可能会发生改变，更新时请留意本部分关于使用方式的说明。
+
+### Troubleshooting
+
+- 遇到 `PermissionError: [Errno 13] Permission denied`：应该是因为缓存文件被占用，建议退出游戏后重试。
+
 ## 导出结果示例
 
 - Excel 结果示例（为保护隐私已隐藏部分信息）
 
   <img src="https://s1.ax1x.com/2023/05/02/p9GJKts.png" alt="xlsx" style="width: 600px;" />
 
 - Markdown 结果示例：
```

### Comparing `starrail-toolkit-0.4.0/setup.py` & `starrail-toolkit-0.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.4.0/starrail/__init__.py` & `starrail-toolkit-0.4.1/starrail/__init__.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.4.0/starrail/config.py` & `starrail-toolkit-0.4.1/starrail/config.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.4.0/starrail/entry/cli.py` & `starrail-toolkit-0.4.1/starrail/entry/cli.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.4.0/starrail/entry/setup.py` & `starrail-toolkit-0.4.1/starrail/entry/setup.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.4.0/starrail/gacha/autodet.py` & `starrail-toolkit-0.4.1/starrail/gacha/autodet.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 reg_key_prefix = 'SOFTWARE\\Microsoft\\Windows\\CurrentVersion\\Uninstall\\'
 reg_key_cn = reg_key_prefix + '崩坏：星穹铁道'
 # reg_key_os = reg_key_prefix + 'Star Rail'
 api_pattern = re.compile(r'https://.+/api/getGachaLog.+game_biz=hkrpg.+')
 
 
-@functools.lru_cache
+@functools.lru_cache()
 def lazyload(module_name):
     return importlib.import_module(module_name)
 
 
 def detect_game_install_path():
     logger.info('Detecting game install path')
     winreg = lazyload('winreg')
```

### Comparing `starrail-toolkit-0.4.0/starrail/gacha/database.py` & `starrail-toolkit-0.4.1/starrail/gacha/database.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.4.0/starrail/gacha/fetch.py` & `starrail-toolkit-0.4.1/starrail/gacha/fetch.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.4.0/starrail/gacha/fileio.py` & `starrail-toolkit-0.4.1/starrail/gacha/fileio.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.4.0/starrail/gacha/parse.py` & `starrail-toolkit-0.4.1/starrail/gacha/parse.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.4.0/starrail/gacha/service.py` & `starrail-toolkit-0.4.1/starrail/gacha/service.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.4.0/starrail/gacha/url.py` & `starrail-toolkit-0.4.1/starrail/gacha/url.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.4.0/starrail/utils/babelfish/dictionary.py` & `starrail-toolkit-0.4.1/starrail/utils/babelfish/dictionary.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.4.0/starrail/utils/babelfish/multilingual.py` & `starrail-toolkit-0.4.1/starrail/utils/babelfish/multilingual.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.4.0/starrail/utils/loggings.py` & `starrail-toolkit-0.4.1/starrail/utils/loggings.py`

 * *Files identical despite different names*

### Comparing `starrail-toolkit-0.4.0/starrail_toolkit.egg-info/PKG-INFO` & `starrail-toolkit-0.4.1/starrail_toolkit.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starrail-toolkit
-Version: 0.4.0
+Version: 0.4.1
 Summary: Honkai Star Rail Toolkit
 Home-page: https://github.com/LittleNyima/honkai-starrail-toolkit
 Author: LittleNyima
 Author-email: littlenyima@163.com
 License: GPLv3
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -19,15 +19,15 @@
 <img src="https://s1.ax1x.com/2023/04/30/p98Cv26.png" alt="logo" />
 </div>
 
 ## 开发状态
 
 | 主分支版本 | 开发分支版本 | PyPI 版本 |
 | :--------: | :----------: | :-------: |
-|   0.4.0    |    0.4.0     |   0.4.0   |
+|   0.4.0    |    0.4.1     |   0.4.1   |
 
 - [x] 支持命令行导出 csv、xlsx、json 格式抽卡记录
 - [x] 支持命令行显示抽卡报告
 - [x] 支持导出 markdown 格式抽卡报告
 - [x] 支持导出网页版抽卡报告
 - [x] 支持中英文多语言导出
 - [x] 支持 Windows 平台游戏中自动检测 API URL
@@ -39,54 +39,63 @@
 目前仅提供命令行版本（*我会尽快编译一个可以直接下载运行的应用程序版本*），用户交互界面版本正在开发中。
 
 ### 命令行安装
 
 Python 用户可以直接使用 pip 安装本工具：
 
 ```shell
-pip install starrail-toolkit --upgrade -i https://pypi.tuna.tsinghua.edu.cn/simple
+python3 -m pip install starrail-toolkit --upgrade -i https://pypi.tuna.tsinghua.edu.cn/simple
 ```
 
 ### 从源码安装
 
 若需要使用尚未推送到 PyPI 版本的功能，可通过源码安装：
 
 ```shell
 git clone git@github.com:LittleNyima/honkai-starrail-toolkit.git
 cd honkai-starrail-toolkit
-python setup.py install
+python3 setup.py install
 ```
 
 ## 使用指南
 
 ### 获取抽卡查询 API URL
 
 请参考[【这个教程】](docs/how-to-get-api-url.md)获取查询链接。
 
 由此可以获得一个形如 `https://api-takumi.mihoyo.com/common/gacha_record/api/getGachaLog?xxxxx` 的 URL，后续步骤使用的就是这个 URL。注意：API URL 会在一定时间（大约 24 小时）后过期，过期后需要重新获取。
 
-**注：若为 Windows 平台，可以使用本工具自动检测 API URL。**首先登陆游戏，进入抽卡查询页面，当显示出一页抽卡查询结果后，运行本工具，即可检测到抽卡查询 URL。如果需要切换账号，建议使用上述教程中的方法获取每个账号的 API URL，以便精确控制导出的账号。
+**注：若为 Windows 平台，可以使用本工具自动检测 API URL。** 首先登陆游戏，进入抽卡查询页面，当显示出一页抽卡查询结果后，运行本工具，即可检测到抽卡查询 URL。如果需要切换账号，建议使用上述教程中的方法获取每个账号的 API URL，以便精确控制导出的账号。
 
 ### 导出抽卡记录
 
 #### 命令行导出
 
 可以使用如下命令导出：
 
 ```shell
+# 非 Windows 平台
 hksr --api https://api-takumi.mihoyo.com/xxx
+# Windows 平台无需 --api 参数
+hksr
 ```
 
 **参数说明：**
 
 - `--api`：（Windows 平台可选）API URL 地址。若为 Windows 平台，可以不填这个参数，而使用自动检测功能。
 - `--export`：（可选）导出格式选项。默认为导出全部格式，若仅需导出部分格式，可以替换对应参数。目前支持的格式有 `csv`、`html`、`json`、`md`、`xlsx`。例如，若只需要 json 与 xlsx 格式数据，可以替换为 `--export json xlsx`。
 - `--locale`：（可选）控制输出语言。默认为输出简体中文，可选值为 `en`（英语）、`chs`（简体中文）。
 - `--log-level`：（可选）日志等级。控制日志的输出等级，默认为 `DEBUG`。若感觉输出的日志过多影响观感，建议将日志等级更改为 `INFO`，例如：`--log-level INFO`。（注意：若设置的日志等级过高，可能导致基本的信息无法显示，例如导出进度、导出位置、命令行版抽卡报告等）从高到低的可选值为 `CRITICAL`、`ERROR`、`WARNING`、`INFO`、`DEBUG`。
 
+本项目目前正处于快速迭代阶段，使用方式可能会发生改变，更新时请留意本部分关于使用方式的说明。
+
+### Troubleshooting
+
+- 遇到 `PermissionError: [Errno 13] Permission denied`：应该是因为缓存文件被占用，建议退出游戏后重试。
+
 ## 导出结果示例
 
 - Excel 结果示例（为保护隐私已隐藏部分信息）
 
   <img src="https://s1.ax1x.com/2023/05/02/p9GJKts.png" alt="xlsx" style="width: 600px;" />
 
 - Markdown 结果示例：
```

### Comparing `starrail-toolkit-0.4.0/starrail_toolkit.egg-info/SOURCES.txt` & `starrail-toolkit-0.4.1/starrail_toolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

