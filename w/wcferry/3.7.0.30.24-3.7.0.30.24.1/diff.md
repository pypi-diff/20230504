# Comparing `tmp/wcferry-3.7.0.30.24.tar.gz` & `tmp/wcferry-3.7.0.30.24.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\wcferry-3.7.0.30.24.tar", last modified: Wed Apr 19 15:46:27 2023, max compression
+gzip compressed data, was "dist/wcferry-3.7.0.30.24.1.tar", last modified: Thu May  4 09:41:52 2023, max compression
```

## Comparing `wcferry-3.7.0.30.24.tar` & `wcferry-3.7.0.30.24.1.tar`

### file list

```diff
@@ -1,18 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 15:46:27.000000 wcferry-3.7.0.30.24/
--rw-rw-rw-   0        0        0       46 2023-03-10 16:21:28.000000 wcferry-3.7.0.30.24/MANIFEST.in
--rw-rw-rw-   0        0        0     7644 2023-04-19 15:46:27.000000 wcferry-3.7.0.30.24/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-04-19 15:46:27.000000 wcferry-3.7.0.30.24/setup.cfg
--rw-rw-rw-   0        0        0     1092 2023-03-10 16:21:28.000000 wcferry-3.7.0.30.24/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-19 15:46:27.000000 wcferry-3.7.0.30.24/wcferry/
--rw-rw-rw-   0        0        0       85 2023-03-10 16:21:28.000000 wcferry-3.7.0.30.24/wcferry/__init__.py
--rw-rw-rw-   0        0        0    16169 2023-04-19 15:32:46.000000 wcferry-3.7.0.30.24/wcferry/client.py
--rw-rw-rw-   0        0        0   629248 2023-04-19 15:39:11.000000 wcferry-3.7.0.30.24/wcferry/spy.dll
--rw-rw-rw-   0        0        0  1151488 2023-04-19 10:56:34.000000 wcferry-3.7.0.30.24/wcferry/spy_debug.dll
--rwxrwxrwx   0        0        0   370688 2023-04-19 15:39:28.000000 wcferry-3.7.0.30.24/wcferry/wcf.exe
--rw-rw-rw-   0        0        0     7175 2023-04-19 11:01:25.000000 wcferry-3.7.0.30.24/wcferry/wcf_pb2.py
-drwxrwxrwx   0        0        0        0 2023-04-19 15:46:27.000000 wcferry-3.7.0.30.24/wcferry.egg-info/
--rw-rw-rw-   0        0        0     7644 2023-04-19 15:46:27.000000 wcferry-3.7.0.30.24/wcferry.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      285 2023-04-19 15:46:27.000000 wcferry-3.7.0.30.24/wcferry.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 15:46:27.000000 wcferry-3.7.0.30.24/wcferry.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2023-04-19 15:46:27.000000 wcferry-3.7.0.30.24/wcferry.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-19 15:46:27.000000 wcferry-3.7.0.30.24/wcferry.egg-info/top_level.txt
+drwxr-xr-x   0 chuck      (501) staff       (20)        0 2023-05-04 09:41:52.000000 wcferry-3.7.0.30.24.1/
+-rw-r--r--   0 chuck      (501) staff       (20)       44 2023-03-04 07:36:00.000000 wcferry-3.7.0.30.24.1/MANIFEST.in
+-rw-r--r--   0 chuck      (501) staff       (20)     6494 2023-05-04 09:41:52.000000 wcferry-3.7.0.30.24.1/PKG-INFO
+-rw-r--r--   0 chuck      (501) staff       (20)       38 2023-05-04 09:41:52.000000 wcferry-3.7.0.30.24.1/setup.cfg
+-rw-r--r--   0 chuck      (501) staff       (20)     1217 2023-05-04 09:37:22.000000 wcferry-3.7.0.30.24.1/setup.py
+drwxr-xr-x   0 chuck      (501) staff       (20)        0 2023-05-04 09:41:52.000000 wcferry-3.7.0.30.24.1/wcferry/
+-rw-r--r--   0 chuck      (501) staff       (20)       81 2023-03-04 07:29:32.000000 wcferry-3.7.0.30.24.1/wcferry/__init__.py
+-rw-r--r--   0 chuck      (501) staff       (20)    16112 2023-05-04 09:37:34.000000 wcferry-3.7.0.30.24.1/wcferry/client.py
+-rw-r--r--   0 chuck      (501) staff       (20)     7210 2023-05-04 09:40:58.000000 wcferry-3.7.0.30.24.1/wcferry/wcf_pb2.py
+drwxr-xr-x   0 chuck      (501) staff       (20)        0 2023-05-04 09:41:52.000000 wcferry-3.7.0.30.24.1/wcferry.egg-info/
+-rw-r--r--   0 chuck      (501) staff       (20)     6494 2023-05-04 09:41:52.000000 wcferry-3.7.0.30.24.1/wcferry.egg-info/PKG-INFO
+-rw-r--r--   0 chuck      (501) staff       (20)      231 2023-05-04 09:41:52.000000 wcferry-3.7.0.30.24.1/wcferry.egg-info/SOURCES.txt
+-rw-r--r--   0 chuck      (501) staff       (20)        1 2023-05-04 09:41:52.000000 wcferry-3.7.0.30.24.1/wcferry.egg-info/dependency_links.txt
+-rw-r--r--   0 chuck      (501) staff       (20)       30 2023-05-04 09:41:52.000000 wcferry-3.7.0.30.24.1/wcferry.egg-info/requires.txt
+-rw-r--r--   0 chuck      (501) staff       (20)        8 2023-05-04 09:41:52.000000 wcferry-3.7.0.30.24.1/wcferry.egg-info/top_level.txt
```

### Comparing `wcferry-3.7.0.30.24/PKG-INFO` & `wcferry-3.7.0.30.24.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,156 +1,157 @@
-Metadata-Version: 2.1
-Name: wcferry
-Version: 3.7.0.30.24
-Summary: 一个玩微信的工具
-Home-page: https://github.com/lich0821/WeChatFerry
-Author: Changhua
-Author-email: lichanghua0821@gmail.com
-License: MIT
-Description: # WeChatFerry Python 客户端
-        ⚠️ **只支持 Windows** ⚠️
-        
-        🤖示例机器人框架：[WeChatRobot](https://github.com/lich0821/WeChatRobot)。
-        
-        ## 快速开始
-        ```sh
-        pip install --upgrade wcferry
-        ```
-        
-        ### 接口清单
-        * 检查登录状态：`is_login`
-        * 获取登录账号的 wxid：`get_self_wxid`
-        * 获取消息类型：`get_msg_types`
-        * 获取所有联系人：`get_contacts`
-        * 获取所有好友：`get_friends`
-        * 获取数据库：`get_dbs`
-        * 获取某数据库下的表：`get_tables`
-        * 获取用户信息：`get_user_info`
-        * 发送文本消息（可 @）：`send_text`
-        * 发送图片：`send_image`
-        * 发送文件：`send_file`
-        * 发送 XML：`send_xml`
-        * 发送表情：`send_emotion`
-        * 允许接收消息：`enable_receiving_msg` 和 `enable_recv_msg（旧接口）`
-        * 停止接收消息：`disable_recv_msg`
-        * 执行 SQL 查询：`query_sql`
-        * 接受好友申请：`accept_new_friend`
-        * 添加群成员：`add_chatroom_members`
-        * 解密图片：`decrypt_image`
-        
-        详情查看 [client.py](wcferry/client.py)。
-        
-        ### Demo：
-        ```py
-        #! /usr/bin/env python3
-        # -*- coding: utf-8 -*-
-        
-        import logging
-        from threading import Thread
-        from time import sleep
-        
-        from wcferry import Wcf
-        
-        logging.basicConfig(level='DEBUG', format="%(asctime)s %(message)s")
-        LOG = logging.getLogger("Demo")
-        
-        
-        def process_msg(wcf: Wcf):
-            """处理接收到的消息"""
-            while wcf.is_receiving_msg():
-                try:
-                    msg = wcf.get_msg()
-                except Exception as e:
-                    continue
-        
-                LOG.info(msg)  # 简单打印
-        
-        
-        def main():
-            LOG.info("Start demo...")
-            wcf = Wcf(debug=True)             # 默认连接本地服务
-            # wcf = Wcf("tcp://127.0.0.1:10086") # 连接远端服务
-        
-            sleep(5)  # 等微信加载好，以免信息显示异常
-            LOG.info(f"已经登录: {True if wcf.is_login() else False}")
-            LOG.info(f"wxid: {wcf.get_self_wxid()}")
-        
-            # 允许接收消息
-            # wcf.enable_recv_msg(LOG.info) # deprecated
-        
-            # 允许接收消息
-            wcf.enable_receiving_msg()
-            Thread(target=process_msg, name="GetMessage", args=(wcf,), daemon=True).start()
-        
-            # wcf.disable_recv_msg() # 当需要停止接收消息时调用
-        
-            ret = wcf.send_text("Hello world.", "filehelper")
-            LOG.info(f"send_text: {ret}")
-        
-            ret = wcf.send_image("TEQuant.jpeg", "filehelper")  # 需要确保图片路径正确
-            LOG.info(f"send_image: {ret}")
-        
-            ret = wcf.send_file("README.MD", "filehelper")  # 需要确保文件路径正确
-            LOG.info(f"send_file: {ret}")
-        
-            LOG.info(f"Message types:\n{wcf.get_msg_types()}")
-            LOG.info(f"Contacts:\n{wcf.get_contacts()}")
-        
-            LOG.info(f"DBs:\n{wcf.get_dbs()}")
-            LOG.info(f"Tables:\n{wcf.get_tables('db')}")
-            LOG.info(f"Results:\n{wcf.query_sql('MicroMsg.db', 'SELECT * FROM Contact LIMIT 1;')}")
-        
-            # 需要真正的 V3、V4 信息
-            # wcf.accept_new_friend("v3", "v4")
-        
-            # 填写正确的群 ID 和成员 wxid
-            # ret = wcf.add_chatroom_members("chatroom id", "wxid1,wxid2,wxid3,...")
-            # LOG.info(f"add_chatroom_members: {ret}")
-        
-            xml = '<?xml version="1.0"?><msg><appmsg appid="" sdkver="0"><title>叮当药房，24小时服务，28分钟送药到家！</title><des>叮当快药首家承诺范围内28分钟送药到家！叮当快药核心区域内7*24小时全天候服务，送药上门！叮当快药官网为您提供快捷便利，正品低价，安全放心的购药、送药服务体验。</des><action>view</action><type>33</type><showtype>0</showtype><content /><url>https://mp.weixin.qq.com/mp/waerrpage?appid=wxc2edadc87077fa2a&amp;type=upgrade&amp;upgradetype=3#wechat_redirect</url><dataurl /><lowurl /><lowdataurl /><recorditem /><thumburl /><messageaction /><md5>7f6f49d301ebf47100199b8a4fcf4de4</md5><extinfo /><sourceusername>gh_c2b88a38c424@app</sourceusername><sourcedisplayname>叮当快药 药店送药到家夜间买药</sourcedisplayname><commenturl /><appattach><totallen>0</totallen><attachid /><emoticonmd5></emoticonmd5><fileext>jpg</fileext><filekey>da0e08f5c7259d03da150d5e7ca6d950</filekey><cdnthumburl>3057020100044b30490201000204e4c0232702032f4ef20204a6bace6f02046401f62d042430326337303430352d333734332d343362652d623335322d6233333566623266376334620204012400030201000405004c537600</cdnthumburl><aeskey>0db26456caf243fbd4efb99058a01d66</aeskey><cdnthumbaeskey>0db26456caf243fbd4efb99058a01d66</cdnthumbaeskey><encryver>1</encryver><cdnthumblength>61558</cdnthumblength><cdnthumbheight>100</cdnthumbheight><cdnthumbwidth>100</cdnthumbwidth></appattach><weappinfo><pagepath>pages/index/index.html</pagepath><username>gh_c2b88a38c424@app</username><appid>wxc2edadc87077fa2a</appid><version>197</version><type>2</type><weappiconurl>http://wx.qlogo.cn/mmhead/Q3auHgzwzM4727n0NQ0ZIPQPlfp15m1WLsnrXbo1kLhFGcolgLyc0A/96</weappiconurl><appservicetype>0</appservicetype><shareId>1_wxc2edadc87077fa2a_29177e9a9b918cb9e75964f80bb8f32e_1677849476_0</shareId></weappinfo><websearch /></appmsg><fromusername>wxid_xxxxxxxxxxxxxx</fromusername><scene>0</scene><appinfo><version>1</version><appname /></appinfo><commenturl /></msg>'
-            ret = wcf.send_xml("filehelper", xml, 0x21)
-            LOG.info(f"send_xml: {ret}")
-        
-            ret = wcf.send_emotion("emo.gif", "filehelper")  # 需要确保 gif 路径正确
-            LOG.info(f"send_emotion: {ret}")
-        
-            # 一直运行
-            wcf.keep_running()
-        
-        
-        if __name__ == "__main__":
-            main()
-        
-        ```
-        
-        ## 一起开发
-        ### 配置环境
-        ```sh
-        # 创建虚拟环境
-        python -m venv .env
-        # 激活虚拟环境
-        source .env/Scripts/activate
-        # 升级 pip
-        pip install --upgrade pip
-        # 安装依赖包
-        pip install grpcio-tools pynng
-        ```
-        
-        ### 重新生成 PB 文件
-        ```sh
-        cd python\wcferry
-        # CMD
-        python -m grpc_tools.protoc --python_out=. --proto_path=..\..\rpc\proto\ wcf.proto
-        
-        # GitBash
-        python -m grpc_tools.protoc --python_out=. --proto_path=../../rpc/proto/ wcf.proto
-        ```
-        
-Platform: UNKNOWN
-Classifier: Environment :: Win32 (MS Windows)
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Customer Service
-Classifier: Topic :: Communications :: Chat
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Programming Language :: Python
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
+Metadata-Version: 2.1
+Name: wcferry
+Version: 3.7.0.30.24.1
+Summary: 一个玩微信的工具
+Home-page: https://github.com/lich0821/WeChatFerry
+Author: Changhua
+Author-email: lichanghua0821@gmail.com
+License: MIT
+Project-URL: Documentation, https://sphinx-autoapi.readthedocs.io/en/latest/
+Project-URL: GitHub, https://github.com/lich0821/WeChatFerry/
+Classifier: Environment :: Win32 (MS Windows)
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Customer Service
+Classifier: Topic :: Communications :: Chat
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Programming Language :: Python
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+
+# WeChatFerry Python 客户端
+⚠️ **只支持 Windows** ⚠️
+
+🤖示例机器人框架：[WeChatRobot](https://github.com/lich0821/WeChatRobot)。
+
+## 快速开始
+```sh
+pip install --upgrade wcferry
+```
+
+### 接口清单
+* 检查登录状态：`is_login`
+* 获取登录账号的 wxid：`get_self_wxid`
+* 获取消息类型：`get_msg_types`
+* 获取所有联系人：`get_contacts`
+* 获取所有好友：`get_friends`
+* 获取数据库：`get_dbs`
+* 获取某数据库下的表：`get_tables`
+* 获取用户信息：`get_user_info`
+* 发送文本消息（可 @）：`send_text`
+* 发送图片：`send_image`
+* 发送文件：`send_file`
+* 发送 XML：`send_xml`
+* 发送表情：`send_emotion`
+* 允许接收消息：`enable_receiving_msg` 和 `enable_recv_msg（旧接口）`
+* 停止接收消息：`disable_recv_msg`
+* 执行 SQL 查询：`query_sql`
+* 接受好友申请：`accept_new_friend`
+* 添加群成员：`add_chatroom_members`
+* 解密图片：`decrypt_image`
+
+详情查看 [client.py](wcferry/client.py)。
+
+### Demo：
+```py
+#! /usr/bin/env python3
+# -*- coding: utf-8 -*-
+
+import logging
+from threading import Thread
+from time import sleep
+
+from wcferry import Wcf
+
+logging.basicConfig(level='DEBUG', format="%(asctime)s %(message)s")
+LOG = logging.getLogger("Demo")
+
+
+def process_msg(wcf: Wcf):
+    """处理接收到的消息"""
+    while wcf.is_receiving_msg():
+        try:
+            msg = wcf.get_msg()
+        except Exception as e:
+            continue
+
+        LOG.info(msg)  # 简单打印
+
+
+def main():
+    LOG.info("Start demo...")
+    wcf = Wcf(debug=True)             # 默认连接本地服务
+    # wcf = Wcf("tcp://127.0.0.1:10086") # 连接远端服务
+
+    sleep(5)  # 等微信加载好，以免信息显示异常
+    LOG.info(f"已经登录: {True if wcf.is_login() else False}")
+    LOG.info(f"wxid: {wcf.get_self_wxid()}")
+
+    # 允许接收消息
+    # wcf.enable_recv_msg(LOG.info) # deprecated
+
+    # 允许接收消息
+    wcf.enable_receiving_msg()
+    Thread(target=process_msg, name="GetMessage", args=(wcf,), daemon=True).start()
+
+    # wcf.disable_recv_msg() # 当需要停止接收消息时调用
+
+    ret = wcf.send_text("Hello world.", "filehelper")
+    LOG.info(f"send_text: {ret}")
+
+    ret = wcf.send_image("TEQuant.jpeg", "filehelper")  # 需要确保图片路径正确
+    LOG.info(f"send_image: {ret}")
+
+    ret = wcf.send_file("README.MD", "filehelper")  # 需要确保文件路径正确
+    LOG.info(f"send_file: {ret}")
+
+    LOG.info(f"Message types:\n{wcf.get_msg_types()}")
+    LOG.info(f"Contacts:\n{wcf.get_contacts()}")
+
+    LOG.info(f"DBs:\n{wcf.get_dbs()}")
+    LOG.info(f"Tables:\n{wcf.get_tables('db')}")
+    LOG.info(f"Results:\n{wcf.query_sql('MicroMsg.db', 'SELECT * FROM Contact LIMIT 1;')}")
+
+    # 需要真正的 V3、V4 信息
+    # wcf.accept_new_friend("v3", "v4")
+
+    # 填写正确的群 ID 和成员 wxid
+    # ret = wcf.add_chatroom_members("chatroom id", "wxid1,wxid2,wxid3,...")
+    # LOG.info(f"add_chatroom_members: {ret}")
+
+    xml = '<?xml version="1.0"?><msg><appmsg appid="" sdkver="0"><title>叮当药房，24小时服务，28分钟送药到家！</title><des>叮当快药首家承诺范围内28分钟送药到家！叮当快药核心区域内7*24小时全天候服务，送药上门！叮当快药官网为您提供快捷便利，正品低价，安全放心的购药、送药服务体验。</des><action>view</action><type>33</type><showtype>0</showtype><content /><url>https://mp.weixin.qq.com/mp/waerrpage?appid=wxc2edadc87077fa2a&amp;type=upgrade&amp;upgradetype=3#wechat_redirect</url><dataurl /><lowurl /><lowdataurl /><recorditem /><thumburl /><messageaction /><md5>7f6f49d301ebf47100199b8a4fcf4de4</md5><extinfo /><sourceusername>gh_c2b88a38c424@app</sourceusername><sourcedisplayname>叮当快药 药店送药到家夜间买药</sourcedisplayname><commenturl /><appattach><totallen>0</totallen><attachid /><emoticonmd5></emoticonmd5><fileext>jpg</fileext><filekey>da0e08f5c7259d03da150d5e7ca6d950</filekey><cdnthumburl>3057020100044b30490201000204e4c0232702032f4ef20204a6bace6f02046401f62d042430326337303430352d333734332d343362652d623335322d6233333566623266376334620204012400030201000405004c537600</cdnthumburl><aeskey>0db26456caf243fbd4efb99058a01d66</aeskey><cdnthumbaeskey>0db26456caf243fbd4efb99058a01d66</cdnthumbaeskey><encryver>1</encryver><cdnthumblength>61558</cdnthumblength><cdnthumbheight>100</cdnthumbheight><cdnthumbwidth>100</cdnthumbwidth></appattach><weappinfo><pagepath>pages/index/index.html</pagepath><username>gh_c2b88a38c424@app</username><appid>wxc2edadc87077fa2a</appid><version>197</version><type>2</type><weappiconurl>http://wx.qlogo.cn/mmhead/Q3auHgzwzM4727n0NQ0ZIPQPlfp15m1WLsnrXbo1kLhFGcolgLyc0A/96</weappiconurl><appservicetype>0</appservicetype><shareId>1_wxc2edadc87077fa2a_29177e9a9b918cb9e75964f80bb8f32e_1677849476_0</shareId></weappinfo><websearch /></appmsg><fromusername>wxid_xxxxxxxxxxxxxx</fromusername><scene>0</scene><appinfo><version>1</version><appname /></appinfo><commenturl /></msg>'
+    ret = wcf.send_xml("filehelper", xml, 0x21)
+    LOG.info(f"send_xml: {ret}")
+
+    ret = wcf.send_emotion("emo.gif", "filehelper")  # 需要确保 gif 路径正确
+    LOG.info(f"send_emotion: {ret}")
+
+    # 一直运行
+    wcf.keep_running()
+
+
+if __name__ == "__main__":
+    main()
+
+```
+
+## 一起开发
+### 配置环境
+```sh
+# 创建虚拟环境
+python -m venv .env
+# 激活虚拟环境
+source .env/Scripts/activate
+# 升级 pip
+pip install --upgrade pip
+# 安装依赖包
+pip install grpcio-tools pynng
+```
+
+### 重新生成 PB 文件
+```sh
+cd python\wcferry
+# CMD
+python -m grpc_tools.protoc --python_out=. --proto_path=..\..\rpc\proto\ wcf.proto
+
+# GitBash
+python -m grpc_tools.protoc --python_out=. --proto_path=../../rpc/proto/ wcf.proto
+```
```

### Comparing `wcferry-3.7.0.30.24/setup.py` & `wcferry-3.7.0.30.24.1/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,40 +1,44 @@
-#! /usr/bin/env python3
-# -*- coding: utf-8 -*-
-
-
-from __future__ import print_function
-from setuptools import setup, find_packages
-
-import wcferry
-
-with open("README.md", "r", encoding="utf-8") as fh:
-    long_description = fh.read()
-
-
-setup(
-    name="wcferry",
-    version=wcferry.__version__,
-    author="Changhua",
-    author_email="lichanghua0821@gmail.com",
-    description="一个玩微信的工具",
-    long_description=long_description,
-    long_description_content_type="text/markdown",
-    license="MIT",
-    url="https://github.com/lich0821/WeChatFerry",
-    python_requires='>=3.7',
-    packages=find_packages(),
-    include_package_data=True,
-    install_requires=[
-        "setuptools",
-        "grpcio-tools",
-        "pynng"
-    ],
-    classifiers=[
-        "Environment :: Win32 (MS Windows)",
-        "Intended Audience :: Developers",
-        "Intended Audience :: Customer Service",
-        "Topic :: Communications :: Chat",
-        "Operating System :: Microsoft :: Windows",
-        "Programming Language :: Python",
-    ],
-)
+#! /usr/bin/env python3
+# -*- coding: utf-8 -*-
+
+
+from __future__ import print_function
+from setuptools import setup, find_packages
+
+import wcferry
+
+with open("README.md", "r", encoding="utf-8") as fh:
+    long_description = fh.read()
+
+
+setup(
+    name="wcferry",
+    version=wcferry.__version__,
+    author="Changhua",
+    author_email="lichanghua0821@gmail.com",
+    description="一个玩微信的工具",
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+    license="MIT",
+    url="https://github.com/lich0821/WeChatFerry",
+    python_requires=">=3.7",
+    packages=find_packages(),
+    include_package_data=True,
+    install_requires=[
+        "setuptools",
+        "grpcio-tools",
+        "pynng"
+    ],
+    classifiers=[
+        "Environment :: Win32 (MS Windows)",
+        "Intended Audience :: Developers",
+        "Intended Audience :: Customer Service",
+        "Topic :: Communications :: Chat",
+        "Operating System :: Microsoft :: Windows",
+        "Programming Language :: Python",
+    ],
+    project_urls={
+        "Documentation": "https://sphinx-autoapi.readthedocs.io/en/latest/",
+        "GitHub": "https://github.com/lich0821/WeChatFerry/",
+    },
+)
```

### Comparing `wcferry-3.7.0.30.24/wcferry/client.py` & `wcferry-3.7.0.30.24.1/wcferry/client.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,471 +1,480 @@
-#! /usr/bin/env python3
-# -*- coding: utf-8 -*-
-
-import atexit
-import base64
-import logging
-import os
-import re
-import sys
-from queue import Queue
-from threading import Thread
-from time import sleep
-from typing import Callable, List, Optional
-
-import pynng
-from google.protobuf import json_format
-
-WCF_ROOT = os.path.abspath(os.path.dirname(__file__))
-sys.path.insert(0, WCF_ROOT)
-import wcf_pb2  # noqa
-
-__version__ = "3.7.0.30.24"
-
-
-def _retry():
-    def decorator(func):
-        """ Retry the function """
-        def wrapper(*args, **kwargs):
-            def logerror(e):
-                func_name = re.findall(r"func: (.*?)\n", str(args[1]))[-1]
-                logging.getLogger("WCF").error(f"Call {func_name} failed: {e}")
-
-            try:
-                ret = func(*args, **kwargs)
-            except pynng.Timeout as _:  # 如果超时，重试
-                try:
-                    ret = func(*args, **kwargs)
-                except Exception as e:
-                    logerror(e)
-                    ret = wcf_pb2.Response()
-            except Exception as e:  # 其他异常，退出
-                logerror(e)
-                sys.exit(-1)
-
-            return ret
-        return wrapper
-    return decorator
-
-
-class Wcf():
-    """WeChatFerry, a tool to play WeChat."""
-    class WxMsg():
-        """微信消息"""
-
-        def __init__(self, msg: wcf_pb2.WxMsg) -> None:
-            self._is_self = msg.is_self
-            self._is_group = msg.is_group
-            self.type = msg.type
-            self.id = msg.id
-            self.xml = msg.xml
-            self.sender = msg.sender
-            self.roomid = msg.roomid
-            self.content = msg.content
-            self.thumb = msg.thumb
-            self.extra = msg.extra
-
-        def __str__(self) -> str:
-            s = f"{'自己发的:' if self._is_self else ''}"
-            s += f"{self.sender}[{self.roomid}]:{self.id}:{self.type}:{self.xml.replace(chr(10), '').replace(chr(9),'')}\n"
-            s += self.content
-            s += f"\n{self.thumb}" if self.thumb else ""
-            s += f"\n{self.extra}" if self.extra else ""
-            return s
-
-        def from_self(self) -> bool:
-            """是否自己发的消息"""
-            return self._is_self == 1
-
-        def from_group(self) -> bool:
-            """是否群聊消息"""
-            return self._is_group
-
-        def is_at(self, wxid) -> bool:
-            """是否被@：群消息，在@名单里，并且不是@所有人"""
-            return self.from_group() and re.findall(
-                f"<atuserlist>.*({wxid}).*</atuserlist>", self.xml) and not re.findall(r"@(?:所有人|all)", self.xml)
-
-        def is_text(self) -> bool:
-            """是否文本消息"""
-            return self.type == 1
-
-    def __init__(self, host: str = None, port: int = 10086, debug: bool = True) -> None:
-        self._local_host = False
-        self._is_running = False
-        self._is_receiving_msg = False
-        self.LOG = logging.getLogger("WCF")
-        self.LOG.info(f"wcferry version: {__version__}")
-        self.port = port
-        self.host = host
-        if host is None:
-            self._local_host = True
-            self.host = "127.0.0.1"
-            cmd = fr'"{WCF_ROOT}\wcf.exe" start {self.port} {"debug" if debug else ""}'
-            if os.system(cmd) != 0:
-                self.LOG.error("初始化失败！")
-                os._exit(-1)
-
-        self.cmd_url = f"tcp://{self.host}:{self.port}"
-
-        # 连接 RPC
-        self.cmd_socket = pynng.Pair1()  # Client --> Server，发送消息
-        self.cmd_socket.send_timeout = 2000  # 发送 2 秒超时
-        self.cmd_socket.recv_timeout = 2000  # 接收 2 秒超时
-        try:
-            self.cmd_socket.dial(self.cmd_url, block=True)
-        except Exception as e:
-            self.LOG.error(f"连接失败: {e}")
-            os._exit(-2)
-
-        self.msg_socket = pynng.Pair1()  # Server --> Client，接收消息
-        self.msg_socket.send_timeout = 2000  # 发送 2 秒超时
-        self.msg_socket.recv_timeout = 2000  # 接收 2 秒超时
-        self.msg_url = self.cmd_url.replace(str(self.port), str(self.port + 1))
-
-        atexit.register(self.cleanup)  # 退出的时候停止消息接收，防止资源占用
-        while not self.is_login():     # 等待微信登录成功
-            sleep(1)
-
-        self._is_running = True
-        self.contacts = []
-        self.msgQ = Queue()
-        self._SQL_TYPES = {1: int, 2: float, 3: lambda x: x.decode("utf-8"), 4: bytes, 5: lambda x: None}
-        self.self_wxid = self.get_self_wxid()
-
-    def __del__(self) -> None:
-        self.cleanup()
-
-    def cleanup(self) -> None:
-        """关闭连接，回收资源"""
-        if not self._is_running:
-            return
-
-        self.disable_recv_msg()
-        self.cmd_socket.close()
-
-        if self._local_host:
-            cmd = fr'"{WCF_ROOT}\wcf.exe" stop'
-            if os.system(cmd) != 0:
-                self.LOG.error("退出失败！")
-                return
-        self._is_running = False
-
-    def keep_running(self):
-        """阻塞进程，让 RPC 一直维持连接"""
-        try:
-            while True:
-                sleep(1)
-        except Exception as e:
-            self.cleanup()
-
-    @_retry()
-    def _send_request(self, req: wcf_pb2.Request) -> wcf_pb2.Response:
-        data = req.SerializeToString()
-        self.cmd_socket.send(data)
-        rsp = wcf_pb2.Response()
-        rsp.ParseFromString(self.cmd_socket.recv_msg().bytes)
-        return rsp
-
-    def is_receiving_msg(self) -> bool:
-        return self._is_receiving_msg
-
-    def is_login(self) -> bool:
-        """是否已经登录"""
-        req = wcf_pb2.Request()
-        req.func = wcf_pb2.FUNC_IS_LOGIN  # FUNC_IS_LOGIN
-        rsp = self._send_request(req)
-
-        return rsp.status == 1
-
-    def get_self_wxid(self) -> str:
-        """获取登录账户的 wxid"""
-        req = wcf_pb2.Request()
-        req.func = wcf_pb2.FUNC_GET_SELF_WXID  # FUNC_GET_SELF_WXID
-        rsp = self._send_request(req)
-
-        return rsp.str
-
-    def get_msg_types(self) -> dict:
-        """获取所有消息类型"""
-        req = wcf_pb2.Request()
-        req.func = wcf_pb2.FUNC_GET_MSG_TYPES  # FUNC_GET_MSG_TYPES
-        rsp = self._send_request(req)
-        types = json_format.MessageToDict(rsp.types).get("types", {})
-        types = {int(k): v for k, v in types.items()}
-
-        return dict(sorted(dict(types).items()))
-
-    def get_contacts(self) -> List[dict]:
-        """获取完整通讯录"""
-        req = wcf_pb2.Request()
-        req.func = wcf_pb2.FUNC_GET_CONTACTS  # FUNC_GET_CONTACTS
-        rsp = self._send_request(req)
-        contacts = json_format.MessageToDict(rsp.contacts).get("contacts", [])
-
-        for cnt in contacts:
-            gender = cnt.get("gender", "")
-            if gender == 1:
-                gender = "男"
-            elif gender == 2:
-                gender = "女"
-            contact = {
-                "wxid": cnt.get("wxid", ""),
-                "code": cnt.get("code", ""),
-                "remark": cnt.get("remark", ""),
-                "name": cnt.get("name", ""),
-                "country": cnt.get("country", ""),
-                "province": cnt.get("province", ""),
-                "city": cnt.get("city", ""),
-                "gender": gender}
-            self.contacts.append(contact)
-        return self.contacts
-
-    def get_dbs(self) -> List[str]:
-        """获取所有数据库"""
-        req = wcf_pb2.Request()
-        req.func = wcf_pb2.FUNC_GET_DB_NAMES  # FUNC_GET_DB_NAMES
-        rsp = self._send_request(req)
-        dbs = json_format.MessageToDict(rsp.dbs).get("names", [])
-
-        return dbs
-
-    def get_tables(self, db: str) -> List[dict]:
-        """获取 db 中所有表"""
-        req = wcf_pb2.Request()
-        req.func = wcf_pb2.FUNC_GET_DB_TABLES  # FUNC_GET_DB_TABLES
-        req.str = db
-        rsp = self._send_request(req)
-        tables = json_format.MessageToDict(rsp.tables).get("tables", [])
-
-        return tables
-
-    def get_user_info(self) -> dict:
-        """获取个人信息"""
-        req = wcf_pb2.Request()
-        req.func = wcf_pb2.FUNC_GET_USER_INFO  # FUNC_GET_USER_INFO
-        rsp = self._send_request(req)
-        ui = json_format.MessageToDict(rsp.ui)
-
-        return ui
-
-    def send_text(self, msg: str, receiver: str, aters: Optional[str] = "") -> int:
-        """发送文本消息"""
-        req = wcf_pb2.Request()
-        req.func = wcf_pb2.FUNC_SEND_TXT  # FUNC_SEND_TXT
-        req.txt.msg = msg
-        req.txt.receiver = receiver
-        if aters:
-            req.txt.aters = aters
-        rsp = self._send_request(req)
-        return rsp.status
-
-    def send_image(self, path: str, receiver: str) -> int:
-        """发送图片"""
-        req = wcf_pb2.Request()
-        req.func = wcf_pb2.FUNC_SEND_IMG  # FUNC_SEND_IMG
-        req.file.path = path
-        req.file.receiver = receiver
-        rsp = self._send_request(req)
-        return rsp.status
-
-    def send_file(self, path: str, receiver: str) -> int:
-        """发送文件"""
-        req = wcf_pb2.Request()
-        req.func = wcf_pb2.FUNC_SEND_FILE  # FUNC_SEND_FILE
-        req.file.path = path
-        req.file.receiver = receiver
-        rsp = self._send_request(req)
-        return rsp.status
-
-    def send_xml(self, receiver: str, xml: str, type: int, path: str = None) -> int:
-        """发送文件"""
-        req = wcf_pb2.Request()
-        req.func = wcf_pb2.FUNC_SEND_XML  # FUNC_SEND_XML
-        req.xml.receiver = receiver
-        req.xml.content = xml
-        req.xml.type = type
-        if path:
-            req.xml.path = path
-        rsp = self._send_request(req)
-        return rsp.status
-
-    def send_emotion(self, path: str, receiver: str) -> int:
-        """发送表情"""
-        req = wcf_pb2.Request()
-        req.func = wcf_pb2.FUNC_SEND_EMOTION  # FUNC_SEND_EMOTION
-        req.file.path = path
-        req.file.receiver = receiver
-        rsp = self._send_request(req)
-        return rsp.status
-
-    def get_msg(self, block=True) -> WxMsg:
-        return self.msgQ.get(block, timeout=1)
-
-    def enable_receiving_msg(self) -> bool:
-        """允许接收消息"""
-        def listening_msg():
-            rsp = wcf_pb2.Response()
-            self.msg_socket.dial(self.msg_url, block=True)
-            while self._is_receiving_msg:
-                try:
-                    rsp.ParseFromString(self.msg_socket.recv_msg().bytes)
-                except Exception as e:
-                    pass
-                else:
-                    self.msgQ.put(self.WxMsg(rsp.wxmsg))
-
-            # 退出前关闭通信通道
-            self.msg_socket.close()
-
-        if self._is_receiving_msg:
-            return True
-
-        req = wcf_pb2.Request()
-        req.func = wcf_pb2.FUNC_ENABLE_RECV_TXT  # FUNC_ENABLE_RECV_TXT
-        rsp = self._send_request(req)
-        if rsp.status != 0:
-            return False
-
-        self._is_receiving_msg = True
-        # 阻塞，把控制权交给用户
-        # self._rpc_get_message(callback)
-
-        # 不阻塞，启动一个新的线程来接收消息
-        Thread(target=listening_msg, name="GetMessage", daemon=True).start()
-
-        return True
-
-    def enable_recv_msg(self, callback: Callable[[WxMsg], None] = None) -> bool:
-        """设置接收消息回调"""
-        def listening_msg():
-            rsp = wcf_pb2.Response()
-            self.msg_socket.dial(self.msg_url, block=True)
-            while self._is_receiving_msg:
-                try:
-                    rsp.ParseFromString(self.msg_socket.recv_msg().bytes)
-                except Exception as e:
-                    pass
-                else:
-                    callback(self.WxMsg(rsp.wxmsg))
-            # 退出前关闭通信通道
-            self.msg_socket.close()
-
-        if self._is_receiving_msg:
-            return True
-
-        if callback is None:
-            return False
-
-        req = wcf_pb2.Request()
-        req.func = wcf_pb2.FUNC_ENABLE_RECV_TXT  # FUNC_ENABLE_RECV_TXT
-        rsp = self._send_request(req)
-        if rsp.status != 0:
-            return False
-
-        self._is_receiving_msg = True
-        # 阻塞，把控制权交给用户
-        # listening_msg()
-
-        # 不阻塞，启动一个新的线程来接收消息
-        Thread(target=listening_msg, name="GetMessage", daemon=True).start()
-
-        return True
-
-    def disable_recv_msg(self) -> int:
-        """停止接收消息"""
-        if not self._is_receiving_msg:
-            return 0
-
-        req = wcf_pb2.Request()
-        req.func = wcf_pb2.FUNC_DISABLE_RECV_TXT  # FUNC_DISABLE_RECV_TXT
-        rsp = self._send_request(req)
-        self._is_receiving_msg = False
-
-        return rsp.status
-
-    def query_sql(self, db: str, sql: str) -> List[dict]:
-        """执行 SQL"""
-        result = []
-        req = wcf_pb2.Request()
-        req.func = wcf_pb2.FUNC_EXEC_DB_QUERY  # FUNC_EXEC_DB_QUERY
-        req.query.db = db
-        req.query.sql = sql
-        rsp = self._send_request(req)
-        rows = json_format.MessageToDict(rsp.rows).get("rows", [])
-        for r in rows:
-            row = {}
-            for f in r["fields"]:
-                c = base64.b64decode(f.get("content", ""))
-                row[f["column"]] = self._SQL_TYPES[f["type"]](c)
-            result.append(row)
-        return result
-
-    def accept_new_friend(self, v3: str, v4: str) -> int:
-        """添加好友"""
-        req = wcf_pb2.Request()
-        req.func = wcf_pb2.FUNC_ACCEPT_FRIEND  # FUNC_ACCEPT_FRIEND
-        req.v.v3 = v3
-        req.v.v4 = v4
-        rsp = self._send_request(req)
-        return rsp.status
-
-    def get_friends(self) -> List[dict]:
-        """获取好友列表"""
-        not_friends = {
-            "fmessage": "朋友推荐消息",
-            "medianote": "语音记事本",
-            "floatbottle": "漂流瓶",
-            "filehelper": "文件传输助手",
-            "newsapp": "新闻",
-        }
-        friends = []
-        for cnt in self.get_contacts():
-            if (cnt["wxid"].endswith("@chatroom")      # 群聊
-                    or cnt["wxid"].startswith("gh_")       # 公众号
-                    or cnt["wxid"] in not_friends.keys()   # 其他杂号
-                ):
-                continue
-            friends.append(cnt)
-
-        return friends
-
-    def add_chatroom_members(self, roomid: str, wxids: str) -> int:
-        """添加群成员"""
-        req = wcf_pb2.Request()
-        req.func = wcf_pb2.FUNC_ADD_ROOM_MEMBERS  # FUNC_ADD_ROOM_MEMBERS
-        req.m.roomid = roomid
-        req.m.wxids = wxids
-        rsp = self._send_request(req)
-        return rsp.status
-
-    def receive_transfer(self, wxid: str, transferid: str) -> int:
-        """接收转账
-        Args:
-            wxid (str): 转账消息里的发送人 wxid
-            transferid (str): 转账消息里的 transferid
-
-        Returns:
-            int: 1 为成功，其他失败
-        """
-        req = wcf_pb2.Request()
-        req.func = wcf_pb2.FUNC_RECV_TRANSFER  # FUNC_RECV_TRANSFER
-        req.tf.wxid = wxid
-        req.tf.tid = transferid
-        rsp = self._send_request(req)
-        return rsp.status
-
-    def decrypt_image(self, src: str, dst: str) -> bool:
-        """解密图片:
-        Args:
-            src (str): 加密的图片路径
-            dst (str): 解密的图片路径
-
-        Returns:
-            bool: 是否成功
-        """
-        req = wcf_pb2.Request()
-        req.func = wcf_pb2.FUNC_DECRYPT_IMAGE  # FUNC_DECRYPT_IMAGE
-        req.dec.src = src
-        req.dec.dst = dst
-        rsp = self._send_request(req)
-        return rsp.status == 1
+#! /usr/bin/env python3
+# -*- coding: utf-8 -*-
+
+import atexit
+import base64
+import logging
+import os
+import re
+import sys
+from queue import Queue
+from threading import Thread
+from time import sleep
+from typing import Callable, List, Optional
+
+import pynng
+from google.protobuf import json_format
+
+WCF_ROOT = os.path.abspath(os.path.dirname(__file__))
+sys.path.insert(0, WCF_ROOT)
+import wcf_pb2  # noqa
+
+__version__ = "3.7.0.30.24.1"
+
+
+def _retry():
+    def decorator(func):
+        """ Retry the function """
+        def wrapper(*args, **kwargs):
+            def logerror(e):
+                func_name = re.findall(r"func: (.*?)\n", str(args[1]))[-1]
+                logging.getLogger("WCF").error(f"Call {func_name} failed: {e}")
+
+            try:
+                ret = func(*args, **kwargs)
+            except pynng.Timeout as _:  # 如果超时，重试
+                try:
+                    ret = func(*args, **kwargs)
+                except Exception as e:
+                    logerror(e)
+                    ret = wcf_pb2.Response()
+            except Exception as e:  # 其他异常，退出
+                logerror(e)
+                sys.exit(-1)
+
+            return ret
+        return wrapper
+    return decorator
+
+
+class Wcf():
+    """WeChatFerry, a tool to play WeChat."""
+    class WxMsg():
+        """微信消息"""
+
+        def __init__(self, msg: wcf_pb2.WxMsg) -> None:
+            self._is_self = msg.is_self
+            self._is_group = msg.is_group
+            self.type = msg.type
+            self.id = msg.id
+            self.xml = msg.xml
+            self.sender = msg.sender
+            self.roomid = msg.roomid
+            self.content = msg.content
+            self.thumb = msg.thumb
+            self.extra = msg.extra
+
+        def __str__(self) -> str:
+            s = f"{'自己发的:' if self._is_self else ''}"
+            s += f"{self.sender}[{self.roomid}]:{self.id}:{self.type}:{self.xml.replace(chr(10), '').replace(chr(9),'')}\n"
+            s += self.content
+            s += f"\n{self.thumb}" if self.thumb else ""
+            s += f"\n{self.extra}" if self.extra else ""
+            return s
+
+        def from_self(self) -> bool:
+            """是否自己发的消息"""
+            return self._is_self == 1
+
+        def from_group(self) -> bool:
+            """是否群聊消息"""
+            return self._is_group
+
+        def is_at(self, wxid) -> bool:
+            """是否被@：群消息，在@名单里，并且不是@所有人"""
+            return self.from_group() and re.findall(
+                f"<atuserlist>.*({wxid}).*</atuserlist>", self.xml) and not re.findall(r"@(?:所有人|all)", self.xml)
+
+        def is_text(self) -> bool:
+            """是否文本消息"""
+            return self.type == 1
+
+    def __init__(self, host: str = None, port: int = 10086, debug: bool = True) -> None:
+        self._local_host = False
+        self._is_running = False
+        self._is_receiving_msg = False
+        self.LOG = logging.getLogger("WCF")
+        self.LOG.info(f"wcferry version: {__version__}")
+        self.port = port
+        self.host = host
+        if host is None:
+            self._local_host = True
+            self.host = "127.0.0.1"
+            cmd = fr'"{WCF_ROOT}\wcf.exe" start {self.port} {"debug" if debug else ""}'
+            if os.system(cmd) != 0:
+                self.LOG.error("初始化失败！")
+                os._exit(-1)
+
+        self.cmd_url = f"tcp://{self.host}:{self.port}"
+
+        # 连接 RPC
+        self.cmd_socket = pynng.Pair1()  # Client --> Server，发送消息
+        self.cmd_socket.send_timeout = 2000  # 发送 2 秒超时
+        self.cmd_socket.recv_timeout = 2000  # 接收 2 秒超时
+        try:
+            self.cmd_socket.dial(self.cmd_url, block=True)
+        except Exception as e:
+            self.LOG.error(f"连接失败: {e}")
+            os._exit(-2)
+
+        self.msg_socket = pynng.Pair1()  # Server --> Client，接收消息
+        self.msg_socket.send_timeout = 2000  # 发送 2 秒超时
+        self.msg_socket.recv_timeout = 2000  # 接收 2 秒超时
+        self.msg_url = self.cmd_url.replace(str(self.port), str(self.port + 1))
+
+        atexit.register(self.cleanup)  # 退出的时候停止消息接收，防止资源占用
+        while not self.is_login():     # 等待微信登录成功
+            sleep(1)
+
+        self._is_running = True
+        self.contacts = []
+        self.msgQ = Queue()
+        self._SQL_TYPES = {1: int, 2: float, 3: lambda x: x.decode("utf-8"), 4: bytes, 5: lambda x: None}
+        self.self_wxid = self.get_self_wxid()
+
+    def __del__(self) -> None:
+        self.cleanup()
+
+    def cleanup(self) -> None:
+        """关闭连接，回收资源"""
+        if not self._is_running:
+            return
+
+        self.disable_recv_msg()
+        self.cmd_socket.close()
+
+        if self._local_host:
+            cmd = fr'"{WCF_ROOT}\wcf.exe" stop'
+            if os.system(cmd) != 0:
+                self.LOG.error("退出失败！")
+                return
+        self._is_running = False
+
+    def keep_running(self):
+        """阻塞进程，让 RPC 一直维持连接"""
+        try:
+            while True:
+                sleep(1)
+        except Exception as e:
+            self.cleanup()
+
+    @_retry()
+    def _send_request(self, req: wcf_pb2.Request) -> wcf_pb2.Response:
+        data = req.SerializeToString()
+        self.cmd_socket.send(data)
+        rsp = wcf_pb2.Response()
+        rsp.ParseFromString(self.cmd_socket.recv_msg().bytes)
+        return rsp
+
+    def is_receiving_msg(self) -> bool:
+        return self._is_receiving_msg
+
+    def is_login(self) -> bool:
+        """是否已经登录"""
+        req = wcf_pb2.Request()
+        req.func = wcf_pb2.FUNC_IS_LOGIN  # FUNC_IS_LOGIN
+        rsp = self._send_request(req)
+
+        return rsp.status == 1
+
+    def get_self_wxid(self) -> str:
+        """获取登录账户的 wxid"""
+        req = wcf_pb2.Request()
+        req.func = wcf_pb2.FUNC_GET_SELF_WXID  # FUNC_GET_SELF_WXID
+        rsp = self._send_request(req)
+
+        return rsp.str
+
+    def get_msg_types(self) -> dict:
+        """获取所有消息类型"""
+        req = wcf_pb2.Request()
+        req.func = wcf_pb2.FUNC_GET_MSG_TYPES  # FUNC_GET_MSG_TYPES
+        rsp = self._send_request(req)
+        types = json_format.MessageToDict(rsp.types).get("types", {})
+        types = {int(k): v for k, v in types.items()}
+
+        return dict(sorted(dict(types).items()))
+
+    def get_contacts(self) -> List[dict]:
+        """获取完整通讯录"""
+        req = wcf_pb2.Request()
+        req.func = wcf_pb2.FUNC_GET_CONTACTS  # FUNC_GET_CONTACTS
+        rsp = self._send_request(req)
+        contacts = json_format.MessageToDict(rsp.contacts).get("contacts", [])
+
+        for cnt in contacts:
+            gender = cnt.get("gender", "")
+            if gender == 1:
+                gender = "男"
+            elif gender == 2:
+                gender = "女"
+            contact = {
+                "wxid": cnt.get("wxid", ""),
+                "code": cnt.get("code", ""),
+                "remark": cnt.get("remark", ""),
+                "name": cnt.get("name", ""),
+                "country": cnt.get("country", ""),
+                "province": cnt.get("province", ""),
+                "city": cnt.get("city", ""),
+                "gender": gender}
+            self.contacts.append(contact)
+        return self.contacts
+
+    def get_dbs(self) -> List[str]:
+        """获取所有数据库"""
+        req = wcf_pb2.Request()
+        req.func = wcf_pb2.FUNC_GET_DB_NAMES  # FUNC_GET_DB_NAMES
+        rsp = self._send_request(req)
+        dbs = json_format.MessageToDict(rsp.dbs).get("names", [])
+
+        return dbs
+
+    def get_tables(self, db: str) -> List[dict]:
+        """获取 db 中所有表"""
+        req = wcf_pb2.Request()
+        req.func = wcf_pb2.FUNC_GET_DB_TABLES  # FUNC_GET_DB_TABLES
+        req.str = db
+        rsp = self._send_request(req)
+        tables = json_format.MessageToDict(rsp.tables).get("tables", [])
+
+        return tables
+
+    def get_user_info(self) -> dict:
+        """获取个人信息"""
+        req = wcf_pb2.Request()
+        req.func = wcf_pb2.FUNC_GET_USER_INFO  # FUNC_GET_USER_INFO
+        rsp = self._send_request(req)
+        ui = json_format.MessageToDict(rsp.ui)
+
+        return ui
+
+    def send_text(self, msg: str, receiver: str, aters: Optional[str] = "") -> int:
+        """发送文本消息"""
+        req = wcf_pb2.Request()
+        req.func = wcf_pb2.FUNC_SEND_TXT  # FUNC_SEND_TXT
+        req.txt.msg = msg
+        req.txt.receiver = receiver
+        if aters:
+            req.txt.aters = aters
+        rsp = self._send_request(req)
+        return rsp.status
+
+    def send_image(self, path: str, receiver: str) -> int:
+        """发送图片"""
+        req = wcf_pb2.Request()
+        req.func = wcf_pb2.FUNC_SEND_IMG  # FUNC_SEND_IMG
+        req.file.path = path
+        req.file.receiver = receiver
+        rsp = self._send_request(req)
+        return rsp.status
+
+    def send_file(self, path: str, receiver: str) -> int:
+        """发送文件"""
+        req = wcf_pb2.Request()
+        req.func = wcf_pb2.FUNC_SEND_FILE  # FUNC_SEND_FILE
+        req.file.path = path
+        req.file.receiver = receiver
+        rsp = self._send_request(req)
+        return rsp.status
+
+    def send_xml(self, receiver: str, xml: str, type: int, path: str = None) -> int:
+        """发送文件"""
+        req = wcf_pb2.Request()
+        req.func = wcf_pb2.FUNC_SEND_XML  # FUNC_SEND_XML
+        req.xml.receiver = receiver
+        req.xml.content = xml
+        req.xml.type = type
+        if path:
+            req.xml.path = path
+        rsp = self._send_request(req)
+        return rsp.status
+
+    def send_emotion(self, path: str, receiver: str) -> int:
+        """发送表情"""
+        req = wcf_pb2.Request()
+        req.func = wcf_pb2.FUNC_SEND_EMOTION  # FUNC_SEND_EMOTION
+        req.file.path = path
+        req.file.receiver = receiver
+        rsp = self._send_request(req)
+        return rsp.status
+
+    def get_msg(self, block=True) -> WxMsg:
+        return self.msgQ.get(block, timeout=1)
+
+    def enable_receiving_msg(self) -> bool:
+        """允许接收消息"""
+        def listening_msg():
+            rsp = wcf_pb2.Response()
+            self.msg_socket.dial(self.msg_url, block=True)
+            while self._is_receiving_msg:
+                try:
+                    rsp.ParseFromString(self.msg_socket.recv_msg().bytes)
+                except Exception as e:
+                    pass
+                else:
+                    self.msgQ.put(self.WxMsg(rsp.wxmsg))
+
+            # 退出前关闭通信通道
+            self.msg_socket.close()
+
+        if self._is_receiving_msg:
+            return True
+
+        req = wcf_pb2.Request()
+        req.func = wcf_pb2.FUNC_ENABLE_RECV_TXT  # FUNC_ENABLE_RECV_TXT
+        rsp = self._send_request(req)
+        if rsp.status != 0:
+            return False
+
+        self._is_receiving_msg = True
+        # 阻塞，把控制权交给用户
+        # self._rpc_get_message(callback)
+
+        # 不阻塞，启动一个新的线程来接收消息
+        Thread(target=listening_msg, name="GetMessage", daemon=True).start()
+
+        return True
+
+    def enable_recv_msg(self, callback: Callable[[WxMsg], None] = None) -> bool:
+        """设置接收消息回调"""
+        def listening_msg():
+            rsp = wcf_pb2.Response()
+            self.msg_socket.dial(self.msg_url, block=True)
+            while self._is_receiving_msg:
+                try:
+                    rsp.ParseFromString(self.msg_socket.recv_msg().bytes)
+                except Exception as e:
+                    pass
+                else:
+                    callback(self.WxMsg(rsp.wxmsg))
+            # 退出前关闭通信通道
+            self.msg_socket.close()
+
+        if self._is_receiving_msg:
+            return True
+
+        if callback is None:
+            return False
+
+        req = wcf_pb2.Request()
+        req.func = wcf_pb2.FUNC_ENABLE_RECV_TXT  # FUNC_ENABLE_RECV_TXT
+        rsp = self._send_request(req)
+        if rsp.status != 0:
+            return False
+
+        self._is_receiving_msg = True
+        # 阻塞，把控制权交给用户
+        # listening_msg()
+
+        # 不阻塞，启动一个新的线程来接收消息
+        Thread(target=listening_msg, name="GetMessage", daemon=True).start()
+
+        return True
+
+    def disable_recv_msg(self) -> int:
+        """停止接收消息"""
+        if not self._is_receiving_msg:
+            return 0
+
+        req = wcf_pb2.Request()
+        req.func = wcf_pb2.FUNC_DISABLE_RECV_TXT  # FUNC_DISABLE_RECV_TXT
+        rsp = self._send_request(req)
+        self._is_receiving_msg = False
+
+        return rsp.status
+
+    def query_sql(self, db: str, sql: str) -> List[dict]:
+        """执行 SQL"""
+        result = []
+        req = wcf_pb2.Request()
+        req.func = wcf_pb2.FUNC_EXEC_DB_QUERY  # FUNC_EXEC_DB_QUERY
+        req.query.db = db
+        req.query.sql = sql
+        rsp = self._send_request(req)
+        rows = json_format.MessageToDict(rsp.rows).get("rows", [])
+        for r in rows:
+            row = {}
+            for f in r["fields"]:
+                c = base64.b64decode(f.get("content", ""))
+                row[f["column"]] = self._SQL_TYPES[f["type"]](c)
+            result.append(row)
+        return result
+
+    def accept_new_friend(self, v3: str, v4: str, scene: int = 30) -> int:
+        """通过好友申请
+        Args:
+            v3 (str): 加密用户名 (好友申请消息里 v3 开头的字符串)
+            v4 (str): Ticket (好友申请消息里 v4 开头的字符串)
+            scene: 申请方式 (好友申请消息里的 scene); 为了兼容旧接口，默认为扫码添加 (30)
+
+        Returns:
+            int: 1 为成功，其他失败
+        """
+        req = wcf_pb2.Request()
+        req.func = wcf_pb2.FUNC_ACCEPT_FRIEND  # FUNC_ACCEPT_FRIEND
+        req.v.v3 = v3
+        req.v.v4 = v4
+        req.v.scene = scene
+        rsp = self._send_request(req)
+        return rsp.status
+
+    def get_friends(self) -> List[dict]:
+        """获取好友列表"""
+        not_friends = {
+            "fmessage": "朋友推荐消息",
+            "medianote": "语音记事本",
+            "floatbottle": "漂流瓶",
+            "filehelper": "文件传输助手",
+            "newsapp": "新闻",
+        }
+        friends = []
+        for cnt in self.get_contacts():
+            if (cnt["wxid"].endswith("@chatroom")      # 群聊
+                    or cnt["wxid"].startswith("gh_")       # 公众号
+                    or cnt["wxid"] in not_friends.keys()   # 其他杂号
+                ):
+                continue
+            friends.append(cnt)
+
+        return friends
+
+    def add_chatroom_members(self, roomid: str, wxids: str) -> int:
+        """添加群成员"""
+        req = wcf_pb2.Request()
+        req.func = wcf_pb2.FUNC_ADD_ROOM_MEMBERS  # FUNC_ADD_ROOM_MEMBERS
+        req.m.roomid = roomid
+        req.m.wxids = wxids
+        rsp = self._send_request(req)
+        return rsp.status
+
+    def receive_transfer(self, wxid: str, transferid: str) -> int:
+        """接收转账
+        Args:
+            wxid (str): 转账消息里的发送人 wxid
+            transferid (str): 转账消息里的 transferid
+
+        Returns:
+            int: 1 为成功，其他失败
+        """
+        req = wcf_pb2.Request()
+        req.func = wcf_pb2.FUNC_RECV_TRANSFER  # FUNC_RECV_TRANSFER
+        req.tf.wxid = wxid
+        req.tf.tid = transferid
+        rsp = self._send_request(req)
+        return rsp.status
+
+    def decrypt_image(self, src: str, dst: str) -> bool:
+        """解密图片:
+        Args:
+            src (str): 加密的图片路径
+            dst (str): 解密的图片路径
+
+        Returns:
+            bool: 是否成功
+        """
+        req = wcf_pb2.Request()
+        req.func = wcf_pb2.FUNC_DECRYPT_IMAGE  # FUNC_DECRYPT_IMAGE
+        req.dec.src = src
+        req.dec.dst = dst
+        rsp = self._send_request(req)
+        return rsp.status == 1
```

### Comparing `wcferry-3.7.0.30.24/wcferry/wcf_pb2.py` & `wcferry-3.7.0.30.24.1/wcferry/wcf_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,26 +9,26 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\twcf.proto\x12\x03wcf\"\xc8\x02\n\x07Request\x12\x1c\n\x04\x66unc\x18\x01 \x01(\x0e\x32\x0e.wcf.Functions\x12\x1b\n\x05\x65mpty\x18\x02 \x01(\x0b\x32\n.wcf.EmptyH\x00\x12\r\n\x03str\x18\x03 \x01(\tH\x00\x12\x1b\n\x03txt\x18\x04 \x01(\x0b\x32\x0c.wcf.TextMsgH\x00\x12\x1c\n\x04\x66ile\x18\x05 \x01(\x0b\x32\x0c.wcf.PathMsgH\x00\x12\x1d\n\x05query\x18\x06 \x01(\x0b\x32\x0c.wcf.DbQueryH\x00\x12\x1e\n\x01v\x18\x07 \x01(\x0b\x32\x11.wcf.VerificationH\x00\x12\x1c\n\x01m\x18\x08 \x01(\x0b\x32\x0f.wcf.AddMembersH\x00\x12\x1a\n\x03xml\x18\t \x01(\x0b\x32\x0b.wcf.XmlMsgH\x00\x12\x1b\n\x03\x64\x65\x63\x18\n \x01(\x0b\x32\x0c.wcf.DecPathH\x00\x12\x1b\n\x02tf\x18\x0b \x01(\x0b\x32\r.wcf.TransferH\x00\x42\x05\n\x03msg\"\xab\x02\n\x08Response\x12\x1c\n\x04\x66unc\x18\x01 \x01(\x0e\x32\x0e.wcf.Functions\x12\x10\n\x06status\x18\x02 \x01(\x05H\x00\x12\r\n\x03str\x18\x03 \x01(\tH\x00\x12\x1b\n\x05wxmsg\x18\x04 \x01(\x0b\x32\n.wcf.WxMsgH\x00\x12\x1e\n\x05types\x18\x05 \x01(\x0b\x32\r.wcf.MsgTypesH\x00\x12$\n\x08\x63ontacts\x18\x06 \x01(\x0b\x32\x10.wcf.RpcContactsH\x00\x12\x1b\n\x03\x64\x62s\x18\x07 \x01(\x0b\x32\x0c.wcf.DbNamesH\x00\x12\x1f\n\x06tables\x18\x08 \x01(\x0b\x32\r.wcf.DbTablesH\x00\x12\x1b\n\x04rows\x18\t \x01(\x0b\x32\x0b.wcf.DbRowsH\x00\x12\x1b\n\x02ui\x18\n \x01(\x0b\x32\r.wcf.UserInfoH\x00\x42\x05\n\x03msg\"\x07\n\x05\x45mpty\"\xa0\x01\n\x05WxMsg\x12\x0f\n\x07is_self\x18\x01 \x01(\x08\x12\x10\n\x08is_group\x18\x02 \x01(\x08\x12\x0c\n\x04type\x18\x03 \x01(\x05\x12\n\n\x02id\x18\x04 \x01(\t\x12\x0b\n\x03xml\x18\x05 \x01(\t\x12\x0e\n\x06sender\x18\x06 \x01(\t\x12\x0e\n\x06roomid\x18\x07 \x01(\t\x12\x0f\n\x07\x63ontent\x18\x08 \x01(\t\x12\r\n\x05thumb\x18\t \x01(\t\x12\r\n\x05\x65xtra\x18\n \x01(\t\"7\n\x07TextMsg\x12\x0b\n\x03msg\x18\x01 \x01(\t\x12\x10\n\x08receiver\x18\x02 \x01(\t\x12\r\n\x05\x61ters\x18\x03 \x01(\t\")\n\x07PathMsg\x12\x0c\n\x04path\x18\x01 \x01(\t\x12\x10\n\x08receiver\x18\x02 \x01(\t\"G\n\x06XmlMsg\x12\x10\n\x08receiver\x18\x01 \x01(\t\x12\x0f\n\x07\x63ontent\x18\x02 \x01(\t\x12\x0c\n\x04path\x18\x03 \x01(\t\x12\x0c\n\x04type\x18\x04 \x01(\x05\"a\n\x08MsgTypes\x12\'\n\x05types\x18\x01 \x03(\x0b\x32\x18.wcf.MsgTypes.TypesEntry\x1a,\n\nTypesEntry\x12\x0b\n\x03key\x18\x01 \x01(\x05\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x87\x01\n\nRpcContact\x12\x0c\n\x04wxid\x18\x01 \x01(\t\x12\x0c\n\x04\x63ode\x18\x02 \x01(\t\x12\x0e\n\x06remark\x18\x03 \x01(\t\x12\x0c\n\x04name\x18\x04 \x01(\t\x12\x0f\n\x07\x63ountry\x18\x05 \x01(\t\x12\x10\n\x08province\x18\x06 \x01(\t\x12\x0c\n\x04\x63ity\x18\x07 \x01(\t\x12\x0e\n\x06gender\x18\x08 \x01(\x05\"0\n\x0bRpcContacts\x12!\n\x08\x63ontacts\x18\x01 \x03(\x0b\x32\x0f.wcf.RpcContact\"\x18\n\x07\x44\x62Names\x12\r\n\x05names\x18\x01 \x03(\t\"$\n\x07\x44\x62Table\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0b\n\x03sql\x18\x02 \x01(\t\"(\n\x08\x44\x62Tables\x12\x1c\n\x06tables\x18\x01 \x03(\x0b\x32\x0c.wcf.DbTable\"\"\n\x07\x44\x62Query\x12\n\n\x02\x64\x62\x18\x01 \x01(\t\x12\x0b\n\x03sql\x18\x02 \x01(\t\"8\n\x07\x44\x62\x46ield\x12\x0c\n\x04type\x18\x01 \x01(\x05\x12\x0e\n\x06\x63olumn\x18\x02 \x01(\t\x12\x0f\n\x07\x63ontent\x18\x03 \x01(\x0c\"%\n\x05\x44\x62Row\x12\x1c\n\x06\x66ields\x18\x01 \x03(\x0b\x32\x0c.wcf.DbField\"\"\n\x06\x44\x62Rows\x12\x18\n\x04rows\x18\x01 \x03(\x0b\x32\n.wcf.DbRow\"&\n\x0cVerification\x12\n\n\x02v3\x18\x01 \x01(\t\x12\n\n\x02v4\x18\x02 \x01(\t\"+\n\nAddMembers\x12\x0e\n\x06roomid\x18\x01 \x01(\t\x12\r\n\x05wxids\x18\x02 \x01(\t\"D\n\x08UserInfo\x12\x0c\n\x04wxid\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0e\n\x06mobile\x18\x03 \x01(\t\x12\x0c\n\x04home\x18\x04 \x01(\t\"#\n\x07\x44\x65\x63Path\x12\x0b\n\x03src\x18\x01 \x01(\t\x12\x0b\n\x03\x64st\x18\x02 \x01(\t\"%\n\x08Transfer\x12\x0c\n\x04wxid\x18\x01 \x01(\t\x12\x0b\n\x03tid\x18\x02 \x01(\t*\xd3\x03\n\tFunctions\x12\x11\n\rFUNC_RESERVED\x10\x00\x12\x11\n\rFUNC_IS_LOGIN\x10\x01\x12\x16\n\x12\x46UNC_GET_SELF_WXID\x10\x10\x12\x16\n\x12\x46UNC_GET_MSG_TYPES\x10\x11\x12\x15\n\x11\x46UNC_GET_CONTACTS\x10\x12\x12\x15\n\x11\x46UNC_GET_DB_NAMES\x10\x13\x12\x16\n\x12\x46UNC_GET_DB_TABLES\x10\x14\x12\x16\n\x12\x46UNC_GET_USER_INFO\x10\x15\x12\x11\n\rFUNC_SEND_TXT\x10 \x12\x11\n\rFUNC_SEND_IMG\x10!\x12\x12\n\x0e\x46UNC_SEND_FILE\x10\"\x12\x11\n\rFUNC_SEND_XML\x10#\x12\x15\n\x11\x46UNC_SEND_EMOTION\x10$\x12\x18\n\x14\x46UNC_ENABLE_RECV_TXT\x10\x30\x12\x19\n\x15\x46UNC_DISABLE_RECV_TXT\x10@\x12\x16\n\x12\x46UNC_EXEC_DB_QUERY\x10P\x12\x16\n\x12\x46UNC_ACCEPT_FRIEND\x10Q\x12\x19\n\x15\x46UNC_ADD_ROOM_MEMBERS\x10R\x12\x16\n\x12\x46UNC_RECV_TRANSFER\x10S\x12\x16\n\x12\x46UNC_DECRYPT_IMAGE\x10`B\r\n\x0b\x63om.iamteerb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\twcf.proto\x12\x03wcf\"\xc8\x02\n\x07Request\x12\x1c\n\x04\x66unc\x18\x01 \x01(\x0e\x32\x0e.wcf.Functions\x12\x1b\n\x05\x65mpty\x18\x02 \x01(\x0b\x32\n.wcf.EmptyH\x00\x12\r\n\x03str\x18\x03 \x01(\tH\x00\x12\x1b\n\x03txt\x18\x04 \x01(\x0b\x32\x0c.wcf.TextMsgH\x00\x12\x1c\n\x04\x66ile\x18\x05 \x01(\x0b\x32\x0c.wcf.PathMsgH\x00\x12\x1d\n\x05query\x18\x06 \x01(\x0b\x32\x0c.wcf.DbQueryH\x00\x12\x1e\n\x01v\x18\x07 \x01(\x0b\x32\x11.wcf.VerificationH\x00\x12\x1c\n\x01m\x18\x08 \x01(\x0b\x32\x0f.wcf.AddMembersH\x00\x12\x1a\n\x03xml\x18\t \x01(\x0b\x32\x0b.wcf.XmlMsgH\x00\x12\x1b\n\x03\x64\x65\x63\x18\n \x01(\x0b\x32\x0c.wcf.DecPathH\x00\x12\x1b\n\x02tf\x18\x0b \x01(\x0b\x32\r.wcf.TransferH\x00\x42\x05\n\x03msg\"\xab\x02\n\x08Response\x12\x1c\n\x04\x66unc\x18\x01 \x01(\x0e\x32\x0e.wcf.Functions\x12\x10\n\x06status\x18\x02 \x01(\x05H\x00\x12\r\n\x03str\x18\x03 \x01(\tH\x00\x12\x1b\n\x05wxmsg\x18\x04 \x01(\x0b\x32\n.wcf.WxMsgH\x00\x12\x1e\n\x05types\x18\x05 \x01(\x0b\x32\r.wcf.MsgTypesH\x00\x12$\n\x08\x63ontacts\x18\x06 \x01(\x0b\x32\x10.wcf.RpcContactsH\x00\x12\x1b\n\x03\x64\x62s\x18\x07 \x01(\x0b\x32\x0c.wcf.DbNamesH\x00\x12\x1f\n\x06tables\x18\x08 \x01(\x0b\x32\r.wcf.DbTablesH\x00\x12\x1b\n\x04rows\x18\t \x01(\x0b\x32\x0b.wcf.DbRowsH\x00\x12\x1b\n\x02ui\x18\n \x01(\x0b\x32\r.wcf.UserInfoH\x00\x42\x05\n\x03msg\"\x07\n\x05\x45mpty\"\xa0\x01\n\x05WxMsg\x12\x0f\n\x07is_self\x18\x01 \x01(\x08\x12\x10\n\x08is_group\x18\x02 \x01(\x08\x12\x0c\n\x04type\x18\x03 \x01(\x05\x12\n\n\x02id\x18\x04 \x01(\t\x12\x0b\n\x03xml\x18\x05 \x01(\t\x12\x0e\n\x06sender\x18\x06 \x01(\t\x12\x0e\n\x06roomid\x18\x07 \x01(\t\x12\x0f\n\x07\x63ontent\x18\x08 \x01(\t\x12\r\n\x05thumb\x18\t \x01(\t\x12\r\n\x05\x65xtra\x18\n \x01(\t\"7\n\x07TextMsg\x12\x0b\n\x03msg\x18\x01 \x01(\t\x12\x10\n\x08receiver\x18\x02 \x01(\t\x12\r\n\x05\x61ters\x18\x03 \x01(\t\")\n\x07PathMsg\x12\x0c\n\x04path\x18\x01 \x01(\t\x12\x10\n\x08receiver\x18\x02 \x01(\t\"G\n\x06XmlMsg\x12\x10\n\x08receiver\x18\x01 \x01(\t\x12\x0f\n\x07\x63ontent\x18\x02 \x01(\t\x12\x0c\n\x04path\x18\x03 \x01(\t\x12\x0c\n\x04type\x18\x04 \x01(\x05\"a\n\x08MsgTypes\x12\'\n\x05types\x18\x01 \x03(\x0b\x32\x18.wcf.MsgTypes.TypesEntry\x1a,\n\nTypesEntry\x12\x0b\n\x03key\x18\x01 \x01(\x05\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x87\x01\n\nRpcContact\x12\x0c\n\x04wxid\x18\x01 \x01(\t\x12\x0c\n\x04\x63ode\x18\x02 \x01(\t\x12\x0e\n\x06remark\x18\x03 \x01(\t\x12\x0c\n\x04name\x18\x04 \x01(\t\x12\x0f\n\x07\x63ountry\x18\x05 \x01(\t\x12\x10\n\x08province\x18\x06 \x01(\t\x12\x0c\n\x04\x63ity\x18\x07 \x01(\t\x12\x0e\n\x06gender\x18\x08 \x01(\x05\"0\n\x0bRpcContacts\x12!\n\x08\x63ontacts\x18\x01 \x03(\x0b\x32\x0f.wcf.RpcContact\"\x18\n\x07\x44\x62Names\x12\r\n\x05names\x18\x01 \x03(\t\"$\n\x07\x44\x62Table\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0b\n\x03sql\x18\x02 \x01(\t\"(\n\x08\x44\x62Tables\x12\x1c\n\x06tables\x18\x01 \x03(\x0b\x32\x0c.wcf.DbTable\"\"\n\x07\x44\x62Query\x12\n\n\x02\x64\x62\x18\x01 \x01(\t\x12\x0b\n\x03sql\x18\x02 \x01(\t\"8\n\x07\x44\x62\x46ield\x12\x0c\n\x04type\x18\x01 \x01(\x05\x12\x0e\n\x06\x63olumn\x18\x02 \x01(\t\x12\x0f\n\x07\x63ontent\x18\x03 \x01(\x0c\"%\n\x05\x44\x62Row\x12\x1c\n\x06\x66ields\x18\x01 \x03(\x0b\x32\x0c.wcf.DbField\"\"\n\x06\x44\x62Rows\x12\x18\n\x04rows\x18\x01 \x03(\x0b\x32\n.wcf.DbRow\"5\n\x0cVerification\x12\n\n\x02v3\x18\x01 \x01(\t\x12\n\n\x02v4\x18\x02 \x01(\t\x12\r\n\x05scene\x18\x03 \x01(\x05\"+\n\nAddMembers\x12\x0e\n\x06roomid\x18\x01 \x01(\t\x12\r\n\x05wxids\x18\x02 \x01(\t\"D\n\x08UserInfo\x12\x0c\n\x04wxid\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0e\n\x06mobile\x18\x03 \x01(\t\x12\x0c\n\x04home\x18\x04 \x01(\t\"#\n\x07\x44\x65\x63Path\x12\x0b\n\x03src\x18\x01 \x01(\t\x12\x0b\n\x03\x64st\x18\x02 \x01(\t\"%\n\x08Transfer\x12\x0c\n\x04wxid\x18\x01 \x01(\t\x12\x0b\n\x03tid\x18\x02 \x01(\t*\xd3\x03\n\tFunctions\x12\x11\n\rFUNC_RESERVED\x10\x00\x12\x11\n\rFUNC_IS_LOGIN\x10\x01\x12\x16\n\x12\x46UNC_GET_SELF_WXID\x10\x10\x12\x16\n\x12\x46UNC_GET_MSG_TYPES\x10\x11\x12\x15\n\x11\x46UNC_GET_CONTACTS\x10\x12\x12\x15\n\x11\x46UNC_GET_DB_NAMES\x10\x13\x12\x16\n\x12\x46UNC_GET_DB_TABLES\x10\x14\x12\x16\n\x12\x46UNC_GET_USER_INFO\x10\x15\x12\x11\n\rFUNC_SEND_TXT\x10 \x12\x11\n\rFUNC_SEND_IMG\x10!\x12\x12\n\x0e\x46UNC_SEND_FILE\x10\"\x12\x11\n\rFUNC_SEND_XML\x10#\x12\x15\n\x11\x46UNC_SEND_EMOTION\x10$\x12\x18\n\x14\x46UNC_ENABLE_RECV_TXT\x10\x30\x12\x19\n\x15\x46UNC_DISABLE_RECV_TXT\x10@\x12\x16\n\x12\x46UNC_EXEC_DB_QUERY\x10P\x12\x16\n\x12\x46UNC_ACCEPT_FRIEND\x10Q\x12\x19\n\x15\x46UNC_ADD_ROOM_MEMBERS\x10R\x12\x16\n\x12\x46UNC_RECV_TRANSFER\x10S\x12\x16\n\x12\x46UNC_DECRYPT_IMAGE\x10`B\r\n\x0b\x63om.iamteerb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'wcf_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\013com.iamteer'
   _MSGTYPES_TYPESENTRY._options = None
   _MSGTYPES_TYPESENTRY._serialized_options = b'8\001'
-  _FUNCTIONS._serialized_start=1790
-  _FUNCTIONS._serialized_end=2257
+  _FUNCTIONS._serialized_start=1805
+  _FUNCTIONS._serialized_end=2272
   _REQUEST._serialized_start=19
   _REQUEST._serialized_end=347
   _RESPONSE._serialized_start=350
   _RESPONSE._serialized_end=649
   _EMPTY._serialized_start=651
   _EMPTY._serialized_end=658
   _WXMSG._serialized_start=661
@@ -58,17 +58,17 @@
   _DBFIELD._serialized_start=1425
   _DBFIELD._serialized_end=1481
   _DBROW._serialized_start=1483
   _DBROW._serialized_end=1520
   _DBROWS._serialized_start=1522
   _DBROWS._serialized_end=1556
   _VERIFICATION._serialized_start=1558
-  _VERIFICATION._serialized_end=1596
-  _ADDMEMBERS._serialized_start=1598
-  _ADDMEMBERS._serialized_end=1641
-  _USERINFO._serialized_start=1643
-  _USERINFO._serialized_end=1711
-  _DECPATH._serialized_start=1713
-  _DECPATH._serialized_end=1748
-  _TRANSFER._serialized_start=1750
-  _TRANSFER._serialized_end=1787
+  _VERIFICATION._serialized_end=1611
+  _ADDMEMBERS._serialized_start=1613
+  _ADDMEMBERS._serialized_end=1656
+  _USERINFO._serialized_start=1658
+  _USERINFO._serialized_end=1726
+  _DECPATH._serialized_start=1728
+  _DECPATH._serialized_end=1763
+  _TRANSFER._serialized_start=1765
+  _TRANSFER._serialized_end=1802
 # @@protoc_insertion_point(module_scope)
```

### Comparing `wcferry-3.7.0.30.24/wcferry.egg-info/PKG-INFO` & `wcferry-3.7.0.30.24.1/wcferry.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,156 +1,157 @@
-Metadata-Version: 2.1
-Name: wcferry
-Version: 3.7.0.30.24
-Summary: 一个玩微信的工具
-Home-page: https://github.com/lich0821/WeChatFerry
-Author: Changhua
-Author-email: lichanghua0821@gmail.com
-License: MIT
-Description: # WeChatFerry Python 客户端
-        ⚠️ **只支持 Windows** ⚠️
-        
-        🤖示例机器人框架：[WeChatRobot](https://github.com/lich0821/WeChatRobot)。
-        
-        ## 快速开始
-        ```sh
-        pip install --upgrade wcferry
-        ```
-        
-        ### 接口清单
-        * 检查登录状态：`is_login`
-        * 获取登录账号的 wxid：`get_self_wxid`
-        * 获取消息类型：`get_msg_types`
-        * 获取所有联系人：`get_contacts`
-        * 获取所有好友：`get_friends`
-        * 获取数据库：`get_dbs`
-        * 获取某数据库下的表：`get_tables`
-        * 获取用户信息：`get_user_info`
-        * 发送文本消息（可 @）：`send_text`
-        * 发送图片：`send_image`
-        * 发送文件：`send_file`
-        * 发送 XML：`send_xml`
-        * 发送表情：`send_emotion`
-        * 允许接收消息：`enable_receiving_msg` 和 `enable_recv_msg（旧接口）`
-        * 停止接收消息：`disable_recv_msg`
-        * 执行 SQL 查询：`query_sql`
-        * 接受好友申请：`accept_new_friend`
-        * 添加群成员：`add_chatroom_members`
-        * 解密图片：`decrypt_image`
-        
-        详情查看 [client.py](wcferry/client.py)。
-        
-        ### Demo：
-        ```py
-        #! /usr/bin/env python3
-        # -*- coding: utf-8 -*-
-        
-        import logging
-        from threading import Thread
-        from time import sleep
-        
-        from wcferry import Wcf
-        
-        logging.basicConfig(level='DEBUG', format="%(asctime)s %(message)s")
-        LOG = logging.getLogger("Demo")
-        
-        
-        def process_msg(wcf: Wcf):
-            """处理接收到的消息"""
-            while wcf.is_receiving_msg():
-                try:
-                    msg = wcf.get_msg()
-                except Exception as e:
-                    continue
-        
-                LOG.info(msg)  # 简单打印
-        
-        
-        def main():
-            LOG.info("Start demo...")
-            wcf = Wcf(debug=True)             # 默认连接本地服务
-            # wcf = Wcf("tcp://127.0.0.1:10086") # 连接远端服务
-        
-            sleep(5)  # 等微信加载好，以免信息显示异常
-            LOG.info(f"已经登录: {True if wcf.is_login() else False}")
-            LOG.info(f"wxid: {wcf.get_self_wxid()}")
-        
-            # 允许接收消息
-            # wcf.enable_recv_msg(LOG.info) # deprecated
-        
-            # 允许接收消息
-            wcf.enable_receiving_msg()
-            Thread(target=process_msg, name="GetMessage", args=(wcf,), daemon=True).start()
-        
-            # wcf.disable_recv_msg() # 当需要停止接收消息时调用
-        
-            ret = wcf.send_text("Hello world.", "filehelper")
-            LOG.info(f"send_text: {ret}")
-        
-            ret = wcf.send_image("TEQuant.jpeg", "filehelper")  # 需要确保图片路径正确
-            LOG.info(f"send_image: {ret}")
-        
-            ret = wcf.send_file("README.MD", "filehelper")  # 需要确保文件路径正确
-            LOG.info(f"send_file: {ret}")
-        
-            LOG.info(f"Message types:\n{wcf.get_msg_types()}")
-            LOG.info(f"Contacts:\n{wcf.get_contacts()}")
-        
-            LOG.info(f"DBs:\n{wcf.get_dbs()}")
-            LOG.info(f"Tables:\n{wcf.get_tables('db')}")
-            LOG.info(f"Results:\n{wcf.query_sql('MicroMsg.db', 'SELECT * FROM Contact LIMIT 1;')}")
-        
-            # 需要真正的 V3、V4 信息
-            # wcf.accept_new_friend("v3", "v4")
-        
-            # 填写正确的群 ID 和成员 wxid
-            # ret = wcf.add_chatroom_members("chatroom id", "wxid1,wxid2,wxid3,...")
-            # LOG.info(f"add_chatroom_members: {ret}")
-        
-            xml = '<?xml version="1.0"?><msg><appmsg appid="" sdkver="0"><title>叮当药房，24小时服务，28分钟送药到家！</title><des>叮当快药首家承诺范围内28分钟送药到家！叮当快药核心区域内7*24小时全天候服务，送药上门！叮当快药官网为您提供快捷便利，正品低价，安全放心的购药、送药服务体验。</des><action>view</action><type>33</type><showtype>0</showtype><content /><url>https://mp.weixin.qq.com/mp/waerrpage?appid=wxc2edadc87077fa2a&amp;type=upgrade&amp;upgradetype=3#wechat_redirect</url><dataurl /><lowurl /><lowdataurl /><recorditem /><thumburl /><messageaction /><md5>7f6f49d301ebf47100199b8a4fcf4de4</md5><extinfo /><sourceusername>gh_c2b88a38c424@app</sourceusername><sourcedisplayname>叮当快药 药店送药到家夜间买药</sourcedisplayname><commenturl /><appattach><totallen>0</totallen><attachid /><emoticonmd5></emoticonmd5><fileext>jpg</fileext><filekey>da0e08f5c7259d03da150d5e7ca6d950</filekey><cdnthumburl>3057020100044b30490201000204e4c0232702032f4ef20204a6bace6f02046401f62d042430326337303430352d333734332d343362652d623335322d6233333566623266376334620204012400030201000405004c537600</cdnthumburl><aeskey>0db26456caf243fbd4efb99058a01d66</aeskey><cdnthumbaeskey>0db26456caf243fbd4efb99058a01d66</cdnthumbaeskey><encryver>1</encryver><cdnthumblength>61558</cdnthumblength><cdnthumbheight>100</cdnthumbheight><cdnthumbwidth>100</cdnthumbwidth></appattach><weappinfo><pagepath>pages/index/index.html</pagepath><username>gh_c2b88a38c424@app</username><appid>wxc2edadc87077fa2a</appid><version>197</version><type>2</type><weappiconurl>http://wx.qlogo.cn/mmhead/Q3auHgzwzM4727n0NQ0ZIPQPlfp15m1WLsnrXbo1kLhFGcolgLyc0A/96</weappiconurl><appservicetype>0</appservicetype><shareId>1_wxc2edadc87077fa2a_29177e9a9b918cb9e75964f80bb8f32e_1677849476_0</shareId></weappinfo><websearch /></appmsg><fromusername>wxid_xxxxxxxxxxxxxx</fromusername><scene>0</scene><appinfo><version>1</version><appname /></appinfo><commenturl /></msg>'
-            ret = wcf.send_xml("filehelper", xml, 0x21)
-            LOG.info(f"send_xml: {ret}")
-        
-            ret = wcf.send_emotion("emo.gif", "filehelper")  # 需要确保 gif 路径正确
-            LOG.info(f"send_emotion: {ret}")
-        
-            # 一直运行
-            wcf.keep_running()
-        
-        
-        if __name__ == "__main__":
-            main()
-        
-        ```
-        
-        ## 一起开发
-        ### 配置环境
-        ```sh
-        # 创建虚拟环境
-        python -m venv .env
-        # 激活虚拟环境
-        source .env/Scripts/activate
-        # 升级 pip
-        pip install --upgrade pip
-        # 安装依赖包
-        pip install grpcio-tools pynng
-        ```
-        
-        ### 重新生成 PB 文件
-        ```sh
-        cd python\wcferry
-        # CMD
-        python -m grpc_tools.protoc --python_out=. --proto_path=..\..\rpc\proto\ wcf.proto
-        
-        # GitBash
-        python -m grpc_tools.protoc --python_out=. --proto_path=../../rpc/proto/ wcf.proto
-        ```
-        
-Platform: UNKNOWN
-Classifier: Environment :: Win32 (MS Windows)
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Customer Service
-Classifier: Topic :: Communications :: Chat
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Programming Language :: Python
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
+Metadata-Version: 2.1
+Name: wcferry
+Version: 3.7.0.30.24.1
+Summary: 一个玩微信的工具
+Home-page: https://github.com/lich0821/WeChatFerry
+Author: Changhua
+Author-email: lichanghua0821@gmail.com
+License: MIT
+Project-URL: Documentation, https://sphinx-autoapi.readthedocs.io/en/latest/
+Project-URL: GitHub, https://github.com/lich0821/WeChatFerry/
+Classifier: Environment :: Win32 (MS Windows)
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Customer Service
+Classifier: Topic :: Communications :: Chat
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Programming Language :: Python
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+
+# WeChatFerry Python 客户端
+⚠️ **只支持 Windows** ⚠️
+
+🤖示例机器人框架：[WeChatRobot](https://github.com/lich0821/WeChatRobot)。
+
+## 快速开始
+```sh
+pip install --upgrade wcferry
+```
+
+### 接口清单
+* 检查登录状态：`is_login`
+* 获取登录账号的 wxid：`get_self_wxid`
+* 获取消息类型：`get_msg_types`
+* 获取所有联系人：`get_contacts`
+* 获取所有好友：`get_friends`
+* 获取数据库：`get_dbs`
+* 获取某数据库下的表：`get_tables`
+* 获取用户信息：`get_user_info`
+* 发送文本消息（可 @）：`send_text`
+* 发送图片：`send_image`
+* 发送文件：`send_file`
+* 发送 XML：`send_xml`
+* 发送表情：`send_emotion`
+* 允许接收消息：`enable_receiving_msg` 和 `enable_recv_msg（旧接口）`
+* 停止接收消息：`disable_recv_msg`
+* 执行 SQL 查询：`query_sql`
+* 接受好友申请：`accept_new_friend`
+* 添加群成员：`add_chatroom_members`
+* 解密图片：`decrypt_image`
+
+详情查看 [client.py](wcferry/client.py)。
+
+### Demo：
+```py
+#! /usr/bin/env python3
+# -*- coding: utf-8 -*-
+
+import logging
+from threading import Thread
+from time import sleep
+
+from wcferry import Wcf
+
+logging.basicConfig(level='DEBUG', format="%(asctime)s %(message)s")
+LOG = logging.getLogger("Demo")
+
+
+def process_msg(wcf: Wcf):
+    """处理接收到的消息"""
+    while wcf.is_receiving_msg():
+        try:
+            msg = wcf.get_msg()
+        except Exception as e:
+            continue
+
+        LOG.info(msg)  # 简单打印
+
+
+def main():
+    LOG.info("Start demo...")
+    wcf = Wcf(debug=True)             # 默认连接本地服务
+    # wcf = Wcf("tcp://127.0.0.1:10086") # 连接远端服务
+
+    sleep(5)  # 等微信加载好，以免信息显示异常
+    LOG.info(f"已经登录: {True if wcf.is_login() else False}")
+    LOG.info(f"wxid: {wcf.get_self_wxid()}")
+
+    # 允许接收消息
+    # wcf.enable_recv_msg(LOG.info) # deprecated
+
+    # 允许接收消息
+    wcf.enable_receiving_msg()
+    Thread(target=process_msg, name="GetMessage", args=(wcf,), daemon=True).start()
+
+    # wcf.disable_recv_msg() # 当需要停止接收消息时调用
+
+    ret = wcf.send_text("Hello world.", "filehelper")
+    LOG.info(f"send_text: {ret}")
+
+    ret = wcf.send_image("TEQuant.jpeg", "filehelper")  # 需要确保图片路径正确
+    LOG.info(f"send_image: {ret}")
+
+    ret = wcf.send_file("README.MD", "filehelper")  # 需要确保文件路径正确
+    LOG.info(f"send_file: {ret}")
+
+    LOG.info(f"Message types:\n{wcf.get_msg_types()}")
+    LOG.info(f"Contacts:\n{wcf.get_contacts()}")
+
+    LOG.info(f"DBs:\n{wcf.get_dbs()}")
+    LOG.info(f"Tables:\n{wcf.get_tables('db')}")
+    LOG.info(f"Results:\n{wcf.query_sql('MicroMsg.db', 'SELECT * FROM Contact LIMIT 1;')}")
+
+    # 需要真正的 V3、V4 信息
+    # wcf.accept_new_friend("v3", "v4")
+
+    # 填写正确的群 ID 和成员 wxid
+    # ret = wcf.add_chatroom_members("chatroom id", "wxid1,wxid2,wxid3,...")
+    # LOG.info(f"add_chatroom_members: {ret}")
+
+    xml = '<?xml version="1.0"?><msg><appmsg appid="" sdkver="0"><title>叮当药房，24小时服务，28分钟送药到家！</title><des>叮当快药首家承诺范围内28分钟送药到家！叮当快药核心区域内7*24小时全天候服务，送药上门！叮当快药官网为您提供快捷便利，正品低价，安全放心的购药、送药服务体验。</des><action>view</action><type>33</type><showtype>0</showtype><content /><url>https://mp.weixin.qq.com/mp/waerrpage?appid=wxc2edadc87077fa2a&amp;type=upgrade&amp;upgradetype=3#wechat_redirect</url><dataurl /><lowurl /><lowdataurl /><recorditem /><thumburl /><messageaction /><md5>7f6f49d301ebf47100199b8a4fcf4de4</md5><extinfo /><sourceusername>gh_c2b88a38c424@app</sourceusername><sourcedisplayname>叮当快药 药店送药到家夜间买药</sourcedisplayname><commenturl /><appattach><totallen>0</totallen><attachid /><emoticonmd5></emoticonmd5><fileext>jpg</fileext><filekey>da0e08f5c7259d03da150d5e7ca6d950</filekey><cdnthumburl>3057020100044b30490201000204e4c0232702032f4ef20204a6bace6f02046401f62d042430326337303430352d333734332d343362652d623335322d6233333566623266376334620204012400030201000405004c537600</cdnthumburl><aeskey>0db26456caf243fbd4efb99058a01d66</aeskey><cdnthumbaeskey>0db26456caf243fbd4efb99058a01d66</cdnthumbaeskey><encryver>1</encryver><cdnthumblength>61558</cdnthumblength><cdnthumbheight>100</cdnthumbheight><cdnthumbwidth>100</cdnthumbwidth></appattach><weappinfo><pagepath>pages/index/index.html</pagepath><username>gh_c2b88a38c424@app</username><appid>wxc2edadc87077fa2a</appid><version>197</version><type>2</type><weappiconurl>http://wx.qlogo.cn/mmhead/Q3auHgzwzM4727n0NQ0ZIPQPlfp15m1WLsnrXbo1kLhFGcolgLyc0A/96</weappiconurl><appservicetype>0</appservicetype><shareId>1_wxc2edadc87077fa2a_29177e9a9b918cb9e75964f80bb8f32e_1677849476_0</shareId></weappinfo><websearch /></appmsg><fromusername>wxid_xxxxxxxxxxxxxx</fromusername><scene>0</scene><appinfo><version>1</version><appname /></appinfo><commenturl /></msg>'
+    ret = wcf.send_xml("filehelper", xml, 0x21)
+    LOG.info(f"send_xml: {ret}")
+
+    ret = wcf.send_emotion("emo.gif", "filehelper")  # 需要确保 gif 路径正确
+    LOG.info(f"send_emotion: {ret}")
+
+    # 一直运行
+    wcf.keep_running()
+
+
+if __name__ == "__main__":
+    main()
+
+```
+
+## 一起开发
+### 配置环境
+```sh
+# 创建虚拟环境
+python -m venv .env
+# 激活虚拟环境
+source .env/Scripts/activate
+# 升级 pip
+pip install --upgrade pip
+# 安装依赖包
+pip install grpcio-tools pynng
+```
+
+### 重新生成 PB 文件
+```sh
+cd python\wcferry
+# CMD
+python -m grpc_tools.protoc --python_out=. --proto_path=..\..\rpc\proto\ wcf.proto
+
+# GitBash
+python -m grpc_tools.protoc --python_out=. --proto_path=../../rpc/proto/ wcf.proto
+```
```

