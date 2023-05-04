# Comparing `tmp/yeref-0.1.53.tar.gz` & `tmp/yeref-0.1.54.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yeref-0.1.53.tar", last modified: Thu May  4 10:46:07 2023, max compression
+gzip compressed data, was "yeref-0.1.54.tar", last modified: Thu May  4 14:51:02 2023, max compression
```

## Comparing `yeref-0.1.53.tar` & `yeref-0.1.54.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-04 10:46:07.726801 yeref-0.1.53/
--rw-r--r--   0 mark       (501) staff       (20)       85 2023-05-04 10:46:07.726997 yeref-0.1.53/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)       38 2023-05-04 10:46:07.727731 yeref-0.1.53/setup.cfg
--rw-r--r--   0 mark       (501) staff       (20)     1305 2023-05-04 10:45:53.000000 yeref-0.1.53/setup.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-04 10:46:07.717374 yeref-0.1.53/yeref/
--rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.1.53/yeref/__init__.py
--rw-r--r--   0 mark       (501) staff       (20)   507270 2023-05-04 10:45:38.000000 yeref-0.1.53/yeref/l_.py
--rw-r--r--   0 mark       (501) staff       (20)   196882 2023-05-02 12:09:42.000000 yeref-0.1.53/yeref/yeref.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-04 10:46:07.726038 yeref-0.1.53/yeref.egg-info/
--rw-r--r--   0 mark       (501) staff       (20)       85 2023-05-04 10:46:07.000000 yeref-0.1.53/yeref.egg-info/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)      179 2023-05-04 10:46:07.000000 yeref-0.1.53/yeref.egg-info/SOURCES.txt
--rw-r--r--   0 mark       (501) staff       (20)        1 2023-05-04 10:46:07.000000 yeref-0.1.53/yeref.egg-info/dependency_links.txt
--rw-r--r--   0 mark       (501) staff       (20)        6 2023-05-04 10:46:07.000000 yeref-0.1.53/yeref.egg-info/top_level.txt
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-04 14:51:02.605005 yeref-0.1.54/
+-rw-r--r--   0 mark       (501) staff       (20)       85 2023-05-04 14:51:02.605188 yeref-0.1.54/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)       38 2023-05-04 14:51:02.605824 yeref-0.1.54/setup.cfg
+-rw-r--r--   0 mark       (501) staff       (20)     1305 2023-05-04 14:50:49.000000 yeref-0.1.54/setup.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-04 14:51:02.599314 yeref-0.1.54/yeref/
+-rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.1.54/yeref/__init__.py
+-rw-r--r--   0 mark       (501) staff       (20)   508262 2023-05-04 14:44:17.000000 yeref-0.1.54/yeref/l_.py
+-rw-r--r--   0 mark       (501) staff       (20)   196882 2023-05-02 12:09:42.000000 yeref-0.1.54/yeref/yeref.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-04 14:51:02.604210 yeref-0.1.54/yeref.egg-info/
+-rw-r--r--   0 mark       (501) staff       (20)       85 2023-05-04 14:51:02.000000 yeref-0.1.54/yeref.egg-info/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)      179 2023-05-04 14:51:02.000000 yeref-0.1.54/yeref.egg-info/SOURCES.txt
+-rw-r--r--   0 mark       (501) staff       (20)        1 2023-05-04 14:51:02.000000 yeref-0.1.54/yeref.egg-info/dependency_links.txt
+-rw-r--r--   0 mark       (501) staff       (20)        6 2023-05-04 14:51:02.000000 yeref-0.1.54/yeref.egg-info/top_level.txt
```

### Comparing `yeref-0.1.53/setup.py` & `yeref-0.1.54/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
       name='yeref',
-      version='0.1.53',
+      version='0.1.54',
       description='desc-f',
       author='john smith',
       packages=['yeref'],
       # install_requires=[
       #       "httplib2>=0.20.4",
       #       "moviepy>=1.0.3",
       #       "Pillow>=9.2.0",
@@ -39,14 +39,14 @@
 # python setup.py bdist_wheel
 # endregion
 
 # python -m build
 
 # twine upload dist/*
 
-# python3 -m pip install --force-reinstall /Users/mark/PycharmProjects/AUTOBOT/yeref/dist/yeref-0.1.53-py3-none-any.whl
+# python3 -m pip install --force-reinstall /Users/mark/PycharmProjects/AUTOBOT/yeref/dist/yeref-0.1.54-py3-none-any.whl
 
 # python3 -m pip install --upgrade yeref
 
 # pip install --force-reinstall -v "yeref==0.1.30"
 # pip install https://github.com/aiogram/aiogram/archive/refs/heads/dev-3.x.zip
 # pip show aiogram
```

### Comparing `yeref-0.1.53/yeref/l_.py` & `yeref-0.1.54/yeref/l_.py`

 * *Files 0% similar despite different names*

```diff
@@ -1266,23 +1266,23 @@
     'en': "🌱 {0}, welcome to <i>the landing bot</i> of the Ferey project:\n\n▪️ <b>openvpn</b>\n▪️ <b>wireguard</b>\n\n❗️ you can also order the development of a chat bot in our Ferey studio",
     'es': "🌱 {0}, bienvenido al <i>bot de aterrizaje</i> del proyecto Ferey:\n\n▪️ <b>openvpn</b>\n▪️ <b>wireguard</b>\n\n❗️ también puedes encargar el desarrollo de un chat bot en nuestro estudio Ferey",
     'fr': "🌱 {0}, bienvenue sur <i>le landing bot</i> du projet Ferey :\n\n▪️ <b>openvpn</b>\n▪️ <b>wireguard</b>\n\n❗️ vous pouvez également commander le développement d'un chat bot dans notre studio Ferey",
     'zh': "🌱 {0}，欢迎来到 Ferey 项目的<i>落地机器人</i>：\n\n▪️ <b>openvpn</b>\n▪️ <b>wireguard</b>\n\n❗️您也可以在我们的Ferey工作室订购聊天机器人的开发",
     'ar': "🌱 {0} ، مرحبًا بك في <i>روبوت الهبوط</i> الخاص بمشروع Ferey:\n\n▪️ <b>openvpn</b>\n▪️ <b>wireguard</b>\n\n❗️ يمكنك أيضًا طلب تطوير روبوت محادثة في استوديو Ferey",
 }
 l_vpn_1 = {
-    'ru': "👩🏽‍💻 <b>Open VPN</b>\n\n*config by special utm link",
+    'ru': "👩🏽‍💻 <b>Open VPN</b>\n\n{0}",
     'en': "👩🏽‍💻 <b>Open VPN</b>\n\n*config by special utm link",
     'es': "👩🏽‍💻 <b>Abrir VPN</b>\n\n*config por enlace utm especial",
     'fr': "👩🏽‍💻 <b>Ouvrez VPN</b>\n\n*config par lien utm spécial",
     'zh': "👩🏽‍💻 通过特殊的 utm 链接<b>打开 VPN</b>\n\n*config",
     'ar': "👩🏽‍💻 <b>افتح VPN</b>\n\n* التكوين عن طريق ارتباط utm خاص",
 }
 l_vpn_2 = {
-    'ru': "👩🏽‍💻 <b>Wire Guard</b>",
+    'ru': "👩🏽‍💻 <b>Wire Guard</b>\n\n{0}",
     'en': "👩🏽‍💻 <b>Wire Guard</b>",
     'es': "👩🏽‍💻 <b>Protector de alambre</b>",
     'fr': "👩🏽‍💻 <b>Grille de protection</b>",
     'zh': "👩🏽‍💻<b>护线</b>",
     'ar': "👩🏽‍💻 <b>واقي سلكي</b>",
 }
 # endregion
@@ -7464,15 +7464,15 @@
     'en': "🎁 <b>Break</b> one of cookies to get your present",
     'es': '🌬 Sobre',
     'fr': '🌬 À propos de',
     'zh': '🌬 關於',
     'ar': '🌬 حول',
 }
 l_extra_bot_my_blog = {
-    'ru': "📑 Мой Блог",
+    'ru': "📑 <b> Мой блог</b>",
     'en': "📑 My Blog",
     'es': '🌬 Sobre',
     'fr': '🌬 À propos de',
     'zh': '🌬 關於',
     'ar': '🌬 حول',
 }
 l_extra_bot_start = {
@@ -7520,16 +7520,24 @@
     'en': "😔 <b>Here</b> is empty",
     'es': '🌬 Sobre',
     'fr': '🌬 À propos de',
     'zh': '🌬 關於',
     'ar': '🌬 حول',
 }
 
-l_show_admin_panel = {
-    'ru': "<b>👩🏽‍💻 Создание и редактирование публикаций</b>\n\n👩🏽‍💻 Вы зашли как <b>Администратор</b> - вы можете создавать и редактировать блоги, но не удалять их\n\n - Жми на кнопку [👩🏽‍💻 Авторизация] (у нее короткое время жизни)\n2 - Затем: на нужную ссылку (она скопируется), чтобы открыть ее в браузере для редактирования:\n\n",
+l_show_admin_panel_md = {
+    'ru': "*👩🏽‍💻 Создание и редактирование блога*\n\n👩🏽‍💻 Вы зашли как *Администратор* и можете создавать и редактировать блоги, но не удалять их\n\n¹ Авторизация по ссылке в браузере:\n`{0}`\n\n² Перейди (в течение 10сек) по нужной ссылке для редактирования публикации (жми, чтобы скопировать):\n\n",
+    'en': "<b>👩🏽‍💻 Blog-publication creating & editing</b>\n\n👩🏽‍💻 You entered as <b>Administrator</b> - you can create and edit blog-publication, but not to delete them\n\n - Push the button [👩🏽‍💻 Authorization] (it has short lifetime)\n2 - Then: click on the nessesary link (for copy) to open it on a browser for editing:\n\n",
+    'es': "🔙 Volver..",
+    'fr': "🔙 Retour..",
+    'zh': "🔙 回來..",
+    'ar': "🔙 رجوع ..",
+}
+l_show_admin_panel_html = {
+    'ru': "<b>👩🏽‍💻 Создание и редактирование блога</b>\n\n👩🏽‍💻 Вы зашли как <b>Администратор</b> и можете создавать и редактировать блоги, но не удалять их\n\n1. Авторизация по ссылке в браузере:\n<code>{0}</code>\n\n2. Перейди (в течение 10сек) по нужной ссылке для редактирования публикации (жми, чтобы скопировать):\n\n",
     'en': "<b>👩🏽‍💻 Blog-publication creating & editing</b>\n\n👩🏽‍💻 You entered as <b>Administrator</b> - you can create and edit blog-publication, but not to delete them\n\n - Push the button [👩🏽‍💻 Authorization] (it has short lifetime)\n2 - Then: click on the nessesary link (for copy) to open it on a browser for editing:\n\n",
     'es': "🔙 Volver..",
     'fr': "🔙 Retour..",
     'zh': "🔙 回來..",
     'ar': "🔙 رجوع ..",
 }
 l_show_admin_panel_create = {
```

### Comparing `yeref-0.1.53/yeref/yeref.py` & `yeref-0.1.54/yeref/yeref.py`

 * *Files identical despite different names*

