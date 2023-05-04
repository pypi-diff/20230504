# Comparing `tmp/yeref-0.1.52.tar.gz` & `tmp/yeref-0.1.53.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yeref-0.1.52.tar", last modified: Tue May  2 18:33:13 2023, max compression
+gzip compressed data, was "yeref-0.1.53.tar", last modified: Thu May  4 10:46:07 2023, max compression
```

## Comparing `yeref-0.1.52.tar` & `yeref-0.1.53.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-02 18:33:13.483242 yeref-0.1.52/
--rw-r--r--   0 mark       (501) staff       (20)       85 2023-05-02 18:33:13.483467 yeref-0.1.52/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)       38 2023-05-02 18:33:13.484387 yeref-0.1.52/setup.cfg
--rw-r--r--   0 mark       (501) staff       (20)     1305 2023-05-02 18:32:54.000000 yeref-0.1.52/setup.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-02 18:33:13.477810 yeref-0.1.52/yeref/
--rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.1.52/yeref/__init__.py
--rw-r--r--   0 mark       (501) staff       (20)   507240 2023-05-02 17:29:26.000000 yeref-0.1.52/yeref/l_.py
--rw-r--r--   0 mark       (501) staff       (20)   196882 2023-05-02 12:09:42.000000 yeref-0.1.52/yeref/yeref.py
-drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-02 18:33:13.482548 yeref-0.1.52/yeref.egg-info/
--rw-r--r--   0 mark       (501) staff       (20)       85 2023-05-02 18:33:13.000000 yeref-0.1.52/yeref.egg-info/PKG-INFO
--rw-r--r--   0 mark       (501) staff       (20)      179 2023-05-02 18:33:13.000000 yeref-0.1.52/yeref.egg-info/SOURCES.txt
--rw-r--r--   0 mark       (501) staff       (20)        1 2023-05-02 18:33:13.000000 yeref-0.1.52/yeref.egg-info/dependency_links.txt
--rw-r--r--   0 mark       (501) staff       (20)        6 2023-05-02 18:33:13.000000 yeref-0.1.52/yeref.egg-info/top_level.txt
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-04 10:46:07.726801 yeref-0.1.53/
+-rw-r--r--   0 mark       (501) staff       (20)       85 2023-05-04 10:46:07.726997 yeref-0.1.53/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)       38 2023-05-04 10:46:07.727731 yeref-0.1.53/setup.cfg
+-rw-r--r--   0 mark       (501) staff       (20)     1305 2023-05-04 10:45:53.000000 yeref-0.1.53/setup.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-04 10:46:07.717374 yeref-0.1.53/yeref/
+-rw-r--r--   0 mark       (501) staff       (20)       39 2023-04-21 17:52:00.000000 yeref-0.1.53/yeref/__init__.py
+-rw-r--r--   0 mark       (501) staff       (20)   507270 2023-05-04 10:45:38.000000 yeref-0.1.53/yeref/l_.py
+-rw-r--r--   0 mark       (501) staff       (20)   196882 2023-05-02 12:09:42.000000 yeref-0.1.53/yeref/yeref.py
+drwxr-xr-x   0 mark       (501) staff       (20)        0 2023-05-04 10:46:07.726038 yeref-0.1.53/yeref.egg-info/
+-rw-r--r--   0 mark       (501) staff       (20)       85 2023-05-04 10:46:07.000000 yeref-0.1.53/yeref.egg-info/PKG-INFO
+-rw-r--r--   0 mark       (501) staff       (20)      179 2023-05-04 10:46:07.000000 yeref-0.1.53/yeref.egg-info/SOURCES.txt
+-rw-r--r--   0 mark       (501) staff       (20)        1 2023-05-04 10:46:07.000000 yeref-0.1.53/yeref.egg-info/dependency_links.txt
+-rw-r--r--   0 mark       (501) staff       (20)        6 2023-05-04 10:46:07.000000 yeref-0.1.53/yeref.egg-info/top_level.txt
```

### Comparing `yeref-0.1.52/setup.py` & `yeref-0.1.53/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
       name='yeref',
-      version='0.1.52',
+      version='0.1.53',
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
 
-# python3 -m pip install --force-reinstall /Users/mark/PycharmProjects/AUTOBOT/yeref/dist/yeref-0.1.52-py3-none-any.whl
+# python3 -m pip install --force-reinstall /Users/mark/PycharmProjects/AUTOBOT/yeref/dist/yeref-0.1.53-py3-none-any.whl
 
 # python3 -m pip install --upgrade yeref
 
 # pip install --force-reinstall -v "yeref==0.1.30"
 # pip install https://github.com/aiogram/aiogram/archive/refs/heads/dev-3.x.zip
 # pip show aiogram
```

### Comparing `yeref-0.1.52/yeref/l_.py` & `yeref-0.1.53/yeref/l_.py`

 * *Files 0% similar despite different names*

```diff
@@ -119,15 +119,15 @@
     'en': "👇🏽 <b>Choose</b> a direction",
     'es': "👇🏽 <b>Elige</b> una dirección",
     'fr': "👇🏽 <b>Choisissez</b> une direction",
     'zh': "👇🏽<b>选择</b>方向",
     'ar': "👇🏽 <b>اختر</b> الاتجاه",
 }
 l_about = {
-    'ru': "<b>🦋 Автоворонки & чат-боты в SocialMedia</b> для:\n\n▪️таргета: @ferey_send_bot\n▪️поиска: @ferey_find_bot\n▪️постов: @ferey_post_bot\n▪️автоответов: @ferey_user_bot\n▪️канала: @ferey_chat_bot\n▪️канала: @ferey_chn_bot\n▪️рекламы: @ferey_advert_bot\n\n❗️все боты общедоступны & для общего пользования",
+    'ru': "<b>👩🏽‍💻 Ferey projects</b>:\n\n▪️projects: @FereyDemoBot\n▪️constructor: @FereyBotBot\n▪️private_posts: @FereyPostBot\n▪️public_media: @FereyMediaBot\n▪️administration: @FereyChannelBot\n▪️moderation: @FereyGroupBot\n▪️search: @FereyFindBot\n▪️target: @FereyTargetBot\n▪️tools: @FereyToolsBot\n▪️vpn: @FereyVPNBot\n▪️ai: @FereyAIBot\n▪️automation: @FereyUserBot\n▪️vacancies: @FereyWorkBot\n▪️advert: @FereyAdsBot",
     'en': "<b>🦋 SocialMedia auto funnels &amp; chatbots</b> for:\n\n▪️target: @ferey_send_bot\n▪️search: @ferey_find_bot\n▪️posts: @ferey_post_bot\n▪️auto-replies: @ferey_user_bot\n▪️channel: @ferey_chat_bot\n▪️ channel: @ferey_chn_bot\n▪️ads: @ferey_advert_bot\n\n❗️all bots are public & public",
     'es': "<b>🦋 Embudos automáticos de redes sociales y chatbots</b> para:\n\n▪️objetivo: @ferey_send_bot\n▪️búsqueda: @ferey_find_bot\n▪️publicaciones: @ferey_post_bot\n▪️respuestas automáticas: @ferey_user_bot\n▪️canal: @ferey_chat_bot\n▪️ canal: @ferey_chn_bot\n▪️anuncios: @ferey_advert_bot\n\n❗️todos los bots son públicos y públicos",
     'fr': "<b>🦋 Entonnoirs automatiques et chatbots des médias sociaux</b> pour :\n\n▪️cible : @ferey_send_bot\n▪️recherche : @ferey_find_bot\n▪️messages : @ferey_post_bot\n▪️réponses automatiques : @ferey_user_bot\n▪️canal : @ferey_chat_bot\n▪️ chaîne : @ferey_chn_bot\n▪️annonces : @ferey_advert_bot\n\n❗️tous les bots sont publics et publics",
     'zh': "<b>🦋 社交媒体自动漏斗和聊天机器人</b>：\n\n▪️目标： @ferey_send_bot\n▪️搜索： @ferey_find_bot\n▪️帖子： @ferey_post_bot\n▪️自动回复： @ferey_user_bot\n▪️频道： @ferey_chat_bot\n▪️频道： @ferey_chn_bot\n▪️广告： @ferey_advert_bot\n\n❗️所有机器人都是公开的和公开的",
     'ar': "<b>🦋 مسارات تحويل SocialMedia التلقائية وروبوتات الدردشة</b> من أجل:\n\n▪️ الهدف: @ferey_send_bot\n▪️search: @ferey_find_bot\n▪️ المشاركات: @ferey_post_bot\n▪️auto-response: @ferey_user_bot\n▪️ القناة: @ferey_chat_bot القناة: @ferey_chn_bot\n▪️ads: @ferey_advert_bot\n\n❗️ جميع البوتات عامة وعامة",
 }
 l_subscribe = {
@@ -2934,15 +2934,14 @@
     'en': "👮🏽 It is necessary add channel for <i>subscribe checking</i> by command:\n\n/channel LINK",
     'es': "👮🏽 Es necesario agregar un canal para <i>comprobar suscripciones</i> mediante el comando:\n\n/channel LINK",
     'fr': "👮🏽 Il est nécessaire d'ajouter un canal pour <i>vérifier l'abonnement</i> par la commande :\n\n/channel LINK",
     'zh': "👮🏽 <i>訂閱檢查</i>需要通過命令添加頻道：\n\n/channel LINK",
     'ar': "👮🏽 من الضروري إضافة قناة لـ <i> فحص الاشتراك </i> بواسطة الأمر: \n\n/channel LINK",
 }
 
-
 # region commands
 l_update_text = {
     'ru': "👩🏽‍💻 Данные о канале успешно обновлены:\n\n<b>{0}</b> [<code>{1}</code>]\n{2}\n<i>{3}</i>\n\n⚙️ <b>Команды</b> /cmd",
     'en': "➕ Add channel",
     'es': "➕ Agregar grupo",
     'fr': "➕ Ajouter un channele",
     'zh': "➕ 添加組",
@@ -3777,18 +3776,17 @@
     'en': "➕ Add group",
     'es': "➕ Agregar grupo",
     'fr': "➕ Ajouter un groupe",
     'zh': "➕ 添加組",
     'ar': "➕ إضافة مجموعة",
 }
 
-
 # region group
 l_group_config = {
-    ("ccheck",  "👮🏽", "☑"): {
+    ("ccheck", "👮🏽", "☑"): {
         'ru': "Входной контроль",
         'en': "Enter control",
         'es': "Entrar en control",
         'fr': "Prenez le contrôle",
         'zh': "進入控制",
         'ar': "أدخل السيطرة",
     },
@@ -6169,15 +6167,14 @@
     'en': "➕ <b>Create</b>/<code>user extra</code> <i>Telegram</i>-bot via <b>mobile</b> app, and then send its phone <u>number</u>℡\n\n👩🏽‍💻 For example, <code>79331114545</code>",
     'es': "➕ Volver..",
     'fr': "➕ Retour..",
     'zh': "➕ 回來..",
     'ar': "🔙 رجوع ..",
 }
 
-
 # region bot
 l_bot_config = {
     ("cctor", "👩🏽‍💻", "☑"): {
         'ru': "Конструктор ᴺᴱᵂ",
         'en': "Builder ᴺᴱᵂ",
         'es': "Builder ᴺᴱᵂ",
         'fr': "Builder ᴺᴱᵂ",
```

### Comparing `yeref-0.1.52/yeref/yeref.py` & `yeref-0.1.53/yeref/yeref.py`

 * *Files identical despite different names*

