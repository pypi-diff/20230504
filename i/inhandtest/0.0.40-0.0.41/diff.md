# Comparing `tmp/inhandtest-0.0.40.tar.gz` & `tmp/inhandtest-0.0.41.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\inhandtest-0.0.40.tar", last modified: Fri Apr 28 07:44:29 2023, max compression
+gzip compressed data, was "dist\inhandtest-0.0.41.tar", last modified: Thu May  4 02:53:57 2023, max compression
```

## Comparing `inhandtest-0.0.40.tar` & `inhandtest-0.0.41.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-04-28 07:44:29.000000 inhandtest-0.0.40/
--rw-rw-rw-   0        0        0      535 2023-04-28 07:44:29.000000 inhandtest-0.0.40/PKG-INFO
--rw-rw-rw-   0        0        0    12238 2023-02-27 03:43:37.000000 inhandtest-0.0.40/README.md
-drwxrwxrwx   0        0        0        0 2023-04-28 07:44:29.000000 inhandtest-0.0.40/inhandtest/
--rw-rw-rw-   0        0        0        0 2023-01-31 08:41:58.000000 inhandtest-0.0.40/inhandtest/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-28 07:44:29.000000 inhandtest-0.0.40/inhandtest/base_page/
--rw-rw-rw-   0        0        0      134 2023-03-15 06:05:35.000000 inhandtest-0.0.40/inhandtest/base_page/__init__.py
--rw-rw-rw-   0        0        0    61990 2023-03-31 06:55:18.000000 inhandtest-0.0.40/inhandtest/base_page/_vg710_contents_locators.py
--rw-rw-rw-   0        0        0    43917 2023-03-31 07:28:55.000000 inhandtest-0.0.40/inhandtest/base_page/base_page.py
--rw-rw-rw-   0        0        0    10436 2023-04-18 03:34:40.000000 inhandtest-0.0.40/inhandtest/base_page/table_tr.py
--rw-rw-rw-   0        0        0      608 2023-03-31 07:18:06.000000 inhandtest-0.0.40/inhandtest/exception.py
--rw-rw-rw-   0        0        0     3890 2023-03-30 10:08:49.000000 inhandtest-0.0.40/inhandtest/file.py
--rw-rw-rw-   0        0        0    11858 2023-04-28 07:43:52.000000 inhandtest-0.0.40/inhandtest/inmodbus.py
--rw-rw-rw-   0        0        0     4880 2023-04-27 01:05:22.000000 inhandtest-0.0.40/inhandtest/inmongodb.py
--rw-rw-rw-   0        0        0    22049 2023-03-30 10:08:49.000000 inhandtest-0.0.40/inhandtest/inmqtt.py
--rw-rw-rw-   0        0        0    45529 2023-04-24 06:54:53.000000 inhandtest-0.0.40/inhandtest/inrequest.py
--rw-rw-rw-   0        0        0    12335 2023-04-06 06:40:29.000000 inhandtest-0.0.40/inhandtest/insocket.py
--rw-rw-rw-   0        0        0     6088 2023-03-30 10:30:59.000000 inhandtest-0.0.40/inhandtest/inssh.py
--rw-rw-rw-   0        0        0     1144 2023-03-30 10:18:47.000000 inhandtest-0.0.40/inhandtest/ip.py
--rw-rw-rw-   0        0        0     3628 2023-04-23 10:47:45.000000 inhandtest-0.0.40/inhandtest/mail.py
--rw-rw-rw-   0        0        0     1224 2023-04-28 06:53:30.000000 inhandtest-0.0.40/inhandtest/pytest_email.html
--rw-rw-rw-   0        0        0    32413 2023-04-21 10:20:01.000000 inhandtest-0.0.40/inhandtest/telnet.py
--rw-rw-rw-   0        0        0    25167 2023-04-28 06:14:33.000000 inhandtest-0.0.40/inhandtest/tools.py
--rw-rw-rw-   0        0        0      117 2023-04-28 07:34:58.000000 inhandtest-0.0.40/requirements.txt
--rw-rw-rw-   0        0        0     1421 2023-04-28 07:44:17.000000 inhandtest-0.0.40/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 02:53:57.000000 inhandtest-0.0.41/
+-rw-rw-rw-   0        0        0      535 2023-05-04 02:53:57.000000 inhandtest-0.0.41/PKG-INFO
+-rw-rw-rw-   0        0        0    12238 2023-02-27 03:43:37.000000 inhandtest-0.0.41/README.md
+drwxrwxrwx   0        0        0        0 2023-05-04 02:53:57.000000 inhandtest-0.0.41/inhandtest/
+-rw-rw-rw-   0        0        0        0 2023-01-31 08:41:58.000000 inhandtest-0.0.41/inhandtest/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 02:53:57.000000 inhandtest-0.0.41/inhandtest/base_page/
+-rw-rw-rw-   0        0        0      134 2023-03-15 06:05:35.000000 inhandtest-0.0.41/inhandtest/base_page/__init__.py
+-rw-rw-rw-   0        0        0    61990 2023-03-31 06:55:18.000000 inhandtest-0.0.41/inhandtest/base_page/_vg710_contents_locators.py
+-rw-rw-rw-   0        0        0    43917 2023-03-31 07:28:55.000000 inhandtest-0.0.41/inhandtest/base_page/base_page.py
+-rw-rw-rw-   0        0        0    10436 2023-04-18 03:34:40.000000 inhandtest-0.0.41/inhandtest/base_page/table_tr.py
+-rw-rw-rw-   0        0        0      608 2023-03-31 07:18:06.000000 inhandtest-0.0.41/inhandtest/exception.py
+-rw-rw-rw-   0        0        0     3890 2023-03-30 10:08:49.000000 inhandtest-0.0.41/inhandtest/file.py
+-rw-rw-rw-   0        0        0    11860 2023-04-28 07:50:11.000000 inhandtest-0.0.41/inhandtest/inmodbus.py
+-rw-rw-rw-   0        0        0     4880 2023-04-27 01:05:22.000000 inhandtest-0.0.41/inhandtest/inmongodb.py
+-rw-rw-rw-   0        0        0    22049 2023-03-30 10:08:49.000000 inhandtest-0.0.41/inhandtest/inmqtt.py
+-rw-rw-rw-   0        0        0    45529 2023-04-24 06:54:53.000000 inhandtest-0.0.41/inhandtest/inrequest.py
+-rw-rw-rw-   0        0        0    12335 2023-04-06 06:40:29.000000 inhandtest-0.0.41/inhandtest/insocket.py
+-rw-rw-rw-   0        0        0     6088 2023-03-30 10:30:59.000000 inhandtest-0.0.41/inhandtest/inssh.py
+-rw-rw-rw-   0        0        0     1144 2023-03-30 10:18:47.000000 inhandtest-0.0.41/inhandtest/ip.py
+-rw-rw-rw-   0        0        0     4736 2023-05-04 02:38:53.000000 inhandtest-0.0.41/inhandtest/mail.py
+-rw-rw-rw-   0        0        0     1224 2023-04-28 06:53:30.000000 inhandtest-0.0.41/inhandtest/pytest_email.html
+-rw-rw-rw-   0        0        0    32413 2023-04-21 10:20:01.000000 inhandtest-0.0.41/inhandtest/telnet.py
+-rw-rw-rw-   0        0        0    25167 2023-04-28 06:14:33.000000 inhandtest-0.0.41/inhandtest/tools.py
+-rw-rw-rw-   0        0        0      117 2023-04-28 07:34:58.000000 inhandtest-0.0.41/requirements.txt
+-rw-rw-rw-   0        0        0     1421 2023-05-04 02:52:29.000000 inhandtest-0.0.41/setup.py
```

### Comparing `inhandtest-0.0.40/README.md` & `inhandtest-0.0.41/README.md`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.40/inhandtest/base_page/_vg710_contents_locators.py` & `inhandtest-0.0.41/inhandtest/base_page/_vg710_contents_locators.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.40/inhandtest/base_page/base_page.py` & `inhandtest-0.0.41/inhandtest/base_page/base_page.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.40/inhandtest/base_page/table_tr.py` & `inhandtest-0.0.41/inhandtest/base_page/table_tr.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.40/inhandtest/exception.py` & `inhandtest-0.0.41/inhandtest/exception.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.40/inhandtest/file.py` & `inhandtest-0.0.41/inhandtest/file.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.40/inhandtest/inmodbus.py` & `inhandtest-0.0.41/inhandtest/inmodbus.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import logging
 import ctypes
 import re
 from modbus_tk import modbus_rtu, modbus_tcp, utils
 
 
 class ModbusMaster:
-    __doc__ = "使用前需安装serial modbus-tk"
+    __doc__ = "使用前需安装pyserial modbus-tk"
 
     def __init__(self, protocol: str, host: str, port=502, slave_id=1, baud_rate=9600, bytesize=8, parity='N',
                  stop_bits=1):
         """
         创建modbus master
         :param protocol: 协议类型| TCP| RTU
         :param host: 当协议为TCP时，填入IP地址，当协议为RTU时，填入串口号
```

### Comparing `inhandtest-0.0.40/inhandtest/inmongodb.py` & `inhandtest-0.0.41/inhandtest/inmongodb.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.40/inhandtest/inmqtt.py` & `inhandtest-0.0.41/inhandtest/inmqtt.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.40/inhandtest/inrequest.py` & `inhandtest-0.0.41/inhandtest/inrequest.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.40/inhandtest/insocket.py` & `inhandtest-0.0.41/inhandtest/insocket.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.40/inhandtest/inssh.py` & `inhandtest-0.0.41/inhandtest/inssh.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.40/inhandtest/ip.py` & `inhandtest-0.0.41/inhandtest/ip.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.40/inhandtest/mail.py` & `inhandtest-0.0.41/inhandtest/mail.py`

 * *Files 23% similar despite different names*

```diff
@@ -4,51 +4,69 @@
 # @File    : mail.py
 """
 mail
 
 """
 import datetime
 import logging
+import subprocess
+import re
 import emails
 import os
+import json
+from inhandtest.tools import kill_windows_port
 
 
 def pytest_send_report_mail(mail_to: str or list, mail_from: tuple or list, render: dict):
-    """使用已配置好的邮件模板，发送邮件内容
+    """使用已配置好的邮件模板，发送邮件内容, 且使用node.js anywhere启动一个本地服务，用于分享报告,
 
     :param mail_to:  发送给谁
     :param mail_from: 元组($email, $password)
     :param render: 字典类型，需要将报告的内容传入 key值如下：
-                             model：测试设备型号， 如VG710
-                             fun: 测试功能
-                             version: 测试的版本, 如 VG7-V209bfd4(test)-2023-03-31-14-52-02.bin
-                             host: 测试主机， 10.5.24.107
-                             report_url： 报告的链接
-                             summary: 字典类型 从报告中的/allure-results/widgets/summary.json 获取内容
+                             model：必填 测试设备型号， 如VG710
+                             fun: 必填 测试功能
+                             version: 必填 测试的版本, 如 VG7-V209bfd4(test)-2023-03-31-14-52-02.bin
+                             host: 必填 测试主机， 10.5.24.107
+                             port： 必填 分享报告端口， 63330
+                             allure_results_path: 必填 报告中的/allure-results 路径
 
     :return:
     """
+    port = render.get('port') if render.get('port') else 63330
+    # 杀掉端口, 防止端口占用
+    kill_windows_port(render.get('host'), [port, port+1])  # port+1 是https端口
+    # 启动本地服务，分享报告
+    p = subprocess.Popen(f'npx anywhere -h {render.get("host")} -p {port}', cwd=render.get('allure_results_path'),
+                         shell=True,
+                         stdout=subprocess.PIPE, stderr=subprocess.STDOUT, encoding='gbk')
+    while True:
+        output = p.stdout.readline()
+        logging.info(output)
+        if len(re.findall(r'Running at (.*)/', output)) < 1:  # 无论是否启动成功，都会退出循环
+            break
+    # 读取报告中的summary.json文件，获取测试结果
+    summary = json.load(open(os.path.join(render.get('allure_results_path'), 'widgets', 'summary.json'), 'r', encoding='utf-8'))
     html_file_path = os.path.join(os.path.dirname(__file__), 'pytest_email.html')
     from emails.template import JinjaTemplate as Te
 
     message = emails.html(html=Te(open(html_file_path, encoding='utf-8').read()),
                           subject=f'{render.get("model")}自动化测试',
                           mail_from=('映翰通网络测试', mail_from[0]))
-    render.update(render.get('summary').get('statistic'))
-    start = datetime.datetime.fromtimestamp(render.get('summary').get('time').get("start") / 1000.0).strftime(
-        '%Y-%m-%d %H:%M:%S')
-    stop = datetime.datetime.fromtimestamp(render.get('summary').get('time').get("stop") / 1000.0).strftime(
-        '%Y-%m-%d %H:%M:%S')
+    render.update(summary.get('statistic'))
+    start = datetime.datetime.fromtimestamp(summary.get('time').get("start") / 1000.0).strftime('%Y-%m-%d %H:%M:%S')
+    stop = datetime.datetime.fromtimestamp(summary.get('time').get("stop") / 1000.0).strftime('%Y-%m-%d %H:%M:%S')
     render.update({'start': start, 'stop': stop})
-    render.pop('summary')
-    r = message.send(mail_to, smtp={'host': 'smtp.exmail.qq.com', 'port': 465, 'user': mail_from[0], 'ssl': True,
-                                    'password': mail_from[1]},
-                     render=render)
-    assert r.status_code == 250, 'send email failed'
-    logging.info(f'send {mail_to} test result success!')
+    render.update({'report_url': f'http://{render.get("host")}:{port}'})
+    # 发送邮件
+    if mail_to:
+        r = message.send(mail_to, smtp={'host': 'smtp.exmail.qq.com', 'port': 465, 'user': mail_from[0], 'ssl': True,
+                                        'password': mail_from[1]},
+                         render=render)
+        assert r.status_code == 250, 'send email failed'
+        logging.info(f'send {mail_to} test result success!')
 
 
 # def get_mail():
 #     import imaplib
 #     import email
 #
 #     # 连接到 IMAP 服务器
```

### Comparing `inhandtest-0.0.40/inhandtest/pytest_email.html` & `inhandtest-0.0.41/inhandtest/pytest_email.html`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.40/inhandtest/telnet.py` & `inhandtest-0.0.41/inhandtest/telnet.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.40/inhandtest/tools.py` & `inhandtest-0.0.41/inhandtest/tools.py`

 * *Files identical despite different names*

### Comparing `inhandtest-0.0.40/setup.py` & `inhandtest-0.0.41/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 setup
 
 """
 from distutils.core import setup
 
 setup(
     name='inhandtest',
-    version='0.0.40',
+    version='0.0.41',
     author='liwei',
     author_email='liwei@inhand.com.cn',
     description='inhand test tools, so easy',
     maintainer='liwei',
     maintainer_email='liwei@inhand.com.cn',
     # py_modules=['inhandtest.tools', 'inhandtest.telnet', 'inhandtest.inmodbus', 'inhandtest.inmqtt', 'inhandtest.file',
     #             'inhandtest.inrequest', 'inhandtest.inssh', 'inhandtest.base_page'],
```

