# Comparing `tmp/st-searchbar-0.0.8.tar.gz` & `tmp/st-searchbar-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "st-searchbar-0.0.8.tar", last modified: Mon Jul 18 16:18:21 2022, max compression
+gzip compressed data, was "st-searchbar-0.0.9.tar", last modified: Thu May  4 16:16:58 2023, max compression
```

## Comparing `st-searchbar-0.0.8.tar` & `st-searchbar-0.0.9.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2022-07-18 16:18:21.947271 st-searchbar-0.0.8/
--rw-rw-rw-   0        0        0     1082 2022-07-08 18:16:58.000000 st-searchbar-0.0.8/LICENSE
--rw-rw-rw-   0        0        0       49 2022-07-08 18:26:47.000000 st-searchbar-0.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0      350 2022-07-18 16:18:21.944278 st-searchbar-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0       42 2022-07-18 16:18:21.948268 st-searchbar-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      685 2022-07-18 16:12:53.000000 st-searchbar-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2022-07-18 16:18:21.015759 st-searchbar-0.0.8/st_searchbar/
--rw-rw-rw-   0        0        0     3871 2022-07-18 16:12:47.000000 st-searchbar-0.0.8/st_searchbar/__init__.py
-drwxrwxrwx   0        0        0        0 2022-07-18 16:18:20.798339 st-searchbar-0.0.8/st_searchbar/frontend/
-drwxrwxrwx   0        0        0        0 2022-07-18 16:18:21.404719 st-searchbar-0.0.8/st_searchbar/frontend/build/
--rw-rw-rw-   0        0        0     1047 2022-07-18 16:15:16.000000 st-searchbar-0.0.8/st_searchbar/frontend/build/asset-manifest.json
--rw-rw-rw-   0        0        0   206960 2022-07-08 18:16:58.000000 st-searchbar-0.0.8/st_searchbar/frontend/build/bootstrap.min.css
--rw-rw-rw-   0        0        0     2168 2022-07-18 16:15:16.000000 st-searchbar-0.0.8/st_searchbar/frontend/build/index.html
--rw-rw-rw-   0        0        0      663 2022-07-18 16:15:16.000000 st-searchbar-0.0.8/st_searchbar/frontend/build/precache-manifest.0e11f5be7ece44b52359d9e1ee04a7d5.js
--rw-rw-rw-   0        0        0     1183 2022-07-18 16:15:16.000000 st-searchbar-0.0.8/st_searchbar/frontend/build/service-worker.js
-drwxrwxrwx   0        0        0        0 2022-07-18 16:18:20.831251 st-searchbar-0.0.8/st_searchbar/frontend/build/static/
-drwxrwxrwx   0        0        0        0 2022-07-18 16:18:21.512430 st-searchbar-0.0.8/st_searchbar/frontend/build/static/css/
--rw-rw-rw-   0        0        0     1971 2022-07-18 16:15:16.000000 st-searchbar-0.0.8/st_searchbar/frontend/build/static/css/main.cb79e1e0.chunk.css
--rw-rw-rw-   0        0        0     4137 2022-07-18 16:15:16.000000 st-searchbar-0.0.8/st_searchbar/frontend/build/static/css/main.cb79e1e0.chunk.css.map
-drwxrwxrwx   0        0        0        0 2022-07-18 16:18:21.932318 st-searchbar-0.0.8/st_searchbar/frontend/build/static/js/
--rw-rw-rw-   0        0        0   590239 2022-07-18 16:15:16.000000 st-searchbar-0.0.8/st_searchbar/frontend/build/static/js/2.522574df.chunk.js
--rw-rw-rw-   0        0        0     1803 2022-07-18 16:15:16.000000 st-searchbar-0.0.8/st_searchbar/frontend/build/static/js/2.522574df.chunk.js.LICENSE.txt
--rw-rw-rw-   0        0        0  1553141 2022-07-18 16:15:16.000000 st-searchbar-0.0.8/st_searchbar/frontend/build/static/js/2.522574df.chunk.js.map
--rw-rw-rw-   0        0        0     4525 2022-07-18 16:15:16.000000 st-searchbar-0.0.8/st_searchbar/frontend/build/static/js/main.7bc6fb59.chunk.js
--rw-rw-rw-   0        0        0    11462 2022-07-18 16:15:16.000000 st-searchbar-0.0.8/st_searchbar/frontend/build/static/js/main.7bc6fb59.chunk.js.map
--rw-rw-rw-   0        0        0     1598 2022-07-18 16:15:16.000000 st-searchbar-0.0.8/st_searchbar/frontend/build/static/js/runtime-main.11ec9aca.js
--rw-rw-rw-   0        0        0     8317 2022-07-18 16:15:16.000000 st-searchbar-0.0.8/st_searchbar/frontend/build/static/js/runtime-main.11ec9aca.js.map
-drwxrwxrwx   0        0        0        0 2022-07-18 16:18:21.083577 st-searchbar-0.0.8/st_searchbar.egg-info/
--rw-rw-rw-   0        0        0      350 2022-07-18 16:18:16.000000 st-searchbar-0.0.8/st_searchbar.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1069 2022-07-18 16:18:18.000000 st-searchbar-0.0.8/st_searchbar.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-07-18 16:18:16.000000 st-searchbar-0.0.8/st_searchbar.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2022-07-18 16:18:17.000000 st-searchbar-0.0.8/st_searchbar.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2022-07-18 16:18:17.000000 st-searchbar-0.0.8/st_searchbar.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-04 16:16:58.112430 st-searchbar-0.0.9/
+-rw-rw-rw-   0        0        0     1082 2022-07-08 18:16:58.000000 st-searchbar-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0       49 2022-07-08 18:26:47.000000 st-searchbar-0.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0      350 2023-05-04 16:16:58.108441 st-searchbar-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-05-04 16:16:58.114424 st-searchbar-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      685 2023-05-04 16:16:00.000000 st-searchbar-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 16:16:57.276532 st-searchbar-0.0.9/st_searchbar/
+-rw-rw-rw-   0        0        0     3871 2023-05-04 16:09:59.000000 st-searchbar-0.0.9/st_searchbar/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 16:16:57.160493 st-searchbar-0.0.9/st_searchbar/frontend/
+drwxrwxrwx   0        0        0        0 2023-05-04 16:16:57.593761 st-searchbar-0.0.9/st_searchbar/frontend/build/
+-rw-rw-rw-   0        0        0     1047 2023-05-04 16:11:01.000000 st-searchbar-0.0.9/st_searchbar/frontend/build/asset-manifest.json
+-rw-rw-rw-   0        0        0   206960 2022-07-08 18:16:58.000000 st-searchbar-0.0.9/st_searchbar/frontend/build/bootstrap.min.css
+-rw-rw-rw-   0        0        0     2168 2023-05-04 16:11:01.000000 st-searchbar-0.0.9/st_searchbar/frontend/build/index.html
+-rw-rw-rw-   0        0        0      663 2023-05-04 16:11:01.000000 st-searchbar-0.0.9/st_searchbar/frontend/build/precache-manifest.c81079ac31c6a8533bc89850ea3aa800.js
+-rw-rw-rw-   0        0        0     1183 2023-05-04 16:11:01.000000 st-searchbar-0.0.9/st_searchbar/frontend/build/service-worker.js
+drwxrwxrwx   0        0        0        0 2023-05-04 16:16:57.168470 st-searchbar-0.0.9/st_searchbar/frontend/build/static/
+drwxrwxrwx   0        0        0        0 2023-05-04 16:16:57.687489 st-searchbar-0.0.9/st_searchbar/frontend/build/static/css/
+-rw-rw-rw-   0        0        0     1997 2023-05-04 16:11:01.000000 st-searchbar-0.0.9/st_searchbar/frontend/build/static/css/main.d8757a26.chunk.css
+-rw-rw-rw-   0        0        0     4200 2023-05-04 16:11:01.000000 st-searchbar-0.0.9/st_searchbar/frontend/build/static/css/main.d8757a26.chunk.css.map
+drwxrwxrwx   0        0        0        0 2023-05-04 16:16:58.096329 st-searchbar-0.0.9/st_searchbar/frontend/build/static/js/
+-rw-rw-rw-   0        0        0   590239 2023-05-04 16:11:01.000000 st-searchbar-0.0.9/st_searchbar/frontend/build/static/js/2.522574df.chunk.js
+-rw-rw-rw-   0        0        0     1803 2023-05-04 16:11:01.000000 st-searchbar-0.0.9/st_searchbar/frontend/build/static/js/2.522574df.chunk.js.LICENSE.txt
+-rw-rw-rw-   0        0        0  1553141 2023-05-04 16:11:01.000000 st-searchbar-0.0.9/st_searchbar/frontend/build/static/js/2.522574df.chunk.js.map
+-rw-rw-rw-   0        0        0     4653 2023-05-04 16:11:01.000000 st-searchbar-0.0.9/st_searchbar/frontend/build/static/js/main.bf54b1a2.chunk.js
+-rw-rw-rw-   0        0        0    11916 2023-05-04 16:11:01.000000 st-searchbar-0.0.9/st_searchbar/frontend/build/static/js/main.bf54b1a2.chunk.js.map
+-rw-rw-rw-   0        0        0     1598 2023-05-04 16:11:01.000000 st-searchbar-0.0.9/st_searchbar/frontend/build/static/js/runtime-main.11ec9aca.js
+-rw-rw-rw-   0        0        0     8317 2023-05-04 16:11:01.000000 st-searchbar-0.0.9/st_searchbar/frontend/build/static/js/runtime-main.11ec9aca.js.map
+drwxrwxrwx   0        0        0        0 2023-05-04 16:16:57.342550 st-searchbar-0.0.9/st_searchbar.egg-info/
+-rw-rw-rw-   0        0        0      350 2023-05-04 16:16:52.000000 st-searchbar-0.0.9/st_searchbar.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1069 2023-05-04 16:16:55.000000 st-searchbar-0.0.9/st_searchbar.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 16:16:53.000000 st-searchbar-0.0.9/st_searchbar.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-05-04 16:16:54.000000 st-searchbar-0.0.9/st_searchbar.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-04 16:16:54.000000 st-searchbar-0.0.9/st_searchbar.egg-info/top_level.txt
```

### Comparing `st-searchbar-0.0.8/LICENSE` & `st-searchbar-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `st-searchbar-0.0.8/setup.py` & `st-searchbar-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="st-searchbar",
-    version="0.0.8",
+    version="0.0.9",
     author=" Asvin Ragunathan",
     author_email="r.asvin@hotmail.com",
     description="A search bar component for streamlit with audio input and suggestions.",
     long_description="",
     long_description_content_type="text/plain",
     url="",
     packages=setuptools.find_packages(),
```

### Comparing `st-searchbar-0.0.8/st_searchbar/__init__.py` & `st-searchbar-0.0.9/st_searchbar/__init__.py`

 * *Files identical despite different names*

### Comparing `st-searchbar-0.0.8/st_searchbar/frontend/build/bootstrap.min.css` & `st-searchbar-0.0.9/st_searchbar/frontend/build/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `st-searchbar-0.0.8/st_searchbar/frontend/build/index.html` & `st-searchbar-0.0.9/st_searchbar/frontend/build/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -1 +1 @@
-<!doctype html><html lang="en"><head><title>Streamlit Component</title><meta charset="UTF-8"/><meta name="viewport" content="width=device-width,initial-scale=1"/><meta name="theme-color" content="#000000"/><meta name="description" content="Streamlit Component"/><link rel="stylesheet" href="bootstrap.min.css"/><link href="./static/css/main.cb79e1e0.chunk.css" rel="stylesheet"></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root"></div><script>!function(e){function t(t){for(var n,l,a=t[0],p=t[1],i=t[2],c=0,s=[];c<a.length;c++)l=a[c],Object.prototype.hasOwnProperty.call(o,l)&&o[l]&&s.push(o[l][0]),o[l]=0;for(n in p)Object.prototype.hasOwnProperty.call(p,n)&&(e[n]=p[n]);for(f&&f(t);s.length;)s.shift()();return u.push.apply(u,i||[]),r()}function r(){for(var e,t=0;t<u.length;t++){for(var r=u[t],n=!0,a=1;a<r.length;a++){var p=r[a];0!==o[p]&&(n=!1)}n&&(u.splice(t--,1),e=l(l.s=r[0]))}return e}var n={},o={1:0},u=[];function l(t){if(n[t])return n[t].exports;var r=n[t]={i:t,l:!1,exports:{}};return e[t].call(r.exports,r,r.exports,l),r.l=!0,r.exports}l.m=e,l.c=n,l.d=function(e,t,r){l.o(e,t)||Object.defineProperty(e,t,{enumerable:!0,get:r})},l.r=function(e){"undefined"!=typeof Symbol&&Symbol.toStringTag&&Object.defineProperty(e,Symbol.toStringTag,{value:"Module"}),Object.defineProperty(e,"__esModule",{value:!0})},l.t=function(e,t){if(1&t&&(e=l(e)),8&t)return e;if(4&t&&"object"==typeof e&&e&&e.__esModule)return e;var r=Object.create(null);if(l.r(r),Object.defineProperty(r,"default",{enumerable:!0,value:e}),2&t&&"string"!=typeof e)for(var n in e)l.d(r,n,function(t){return e[t]}.bind(null,n));return r},l.n=function(e){var t=e&&e.__esModule?function(){return e.default}:function(){return e};return l.d(t,"a",t),t},l.o=function(e,t){return Object.prototype.hasOwnProperty.call(e,t)},l.p="./";var a=this.webpackJsonpstreamlit_component_template=this.webpackJsonpstreamlit_component_template||[],p=a.push.bind(a);a.push=t,a=a.slice();for(var i=0;i<a.length;i++)t(a[i]);var f=p;r()}([])</script><script src="./static/js/2.522574df.chunk.js"></script><script src="./static/js/main.7bc6fb59.chunk.js"></script></body></html>
+<!doctype html><html lang="en"><head><title>Streamlit Component</title><meta charset="UTF-8"/><meta name="viewport" content="width=device-width,initial-scale=1"/><meta name="theme-color" content="#000000"/><meta name="description" content="Streamlit Component"/><link rel="stylesheet" href="bootstrap.min.css"/><link href="./static/css/main.d8757a26.chunk.css" rel="stylesheet"></head><body><noscript>You need to enable JavaScript to run this app.</noscript><div id="root"></div><script>!function(e){function t(t){for(var n,l,a=t[0],p=t[1],i=t[2],c=0,s=[];c<a.length;c++)l=a[c],Object.prototype.hasOwnProperty.call(o,l)&&o[l]&&s.push(o[l][0]),o[l]=0;for(n in p)Object.prototype.hasOwnProperty.call(p,n)&&(e[n]=p[n]);for(f&&f(t);s.length;)s.shift()();return u.push.apply(u,i||[]),r()}function r(){for(var e,t=0;t<u.length;t++){for(var r=u[t],n=!0,a=1;a<r.length;a++){var p=r[a];0!==o[p]&&(n=!1)}n&&(u.splice(t--,1),e=l(l.s=r[0]))}return e}var n={},o={1:0},u=[];function l(t){if(n[t])return n[t].exports;var r=n[t]={i:t,l:!1,exports:{}};return e[t].call(r.exports,r,r.exports,l),r.l=!0,r.exports}l.m=e,l.c=n,l.d=function(e,t,r){l.o(e,t)||Object.defineProperty(e,t,{enumerable:!0,get:r})},l.r=function(e){"undefined"!=typeof Symbol&&Symbol.toStringTag&&Object.defineProperty(e,Symbol.toStringTag,{value:"Module"}),Object.defineProperty(e,"__esModule",{value:!0})},l.t=function(e,t){if(1&t&&(e=l(e)),8&t)return e;if(4&t&&"object"==typeof e&&e&&e.__esModule)return e;var r=Object.create(null);if(l.r(r),Object.defineProperty(r,"default",{enumerable:!0,value:e}),2&t&&"string"!=typeof e)for(var n in e)l.d(r,n,function(t){return e[t]}.bind(null,n));return r},l.n=function(e){var t=e&&e.__esModule?function(){return e.default}:function(){return e};return l.d(t,"a",t),t},l.o=function(e,t){return Object.prototype.hasOwnProperty.call(e,t)},l.p="./";var a=this.webpackJsonpstreamlit_component_template=this.webpackJsonpstreamlit_component_template||[],p=a.push.bind(a);a.push=t,a=a.slice();for(var i=0;i<a.length;i++)t(a[i]);var f=p;r()}([])</script><script src="./static/js/2.522574df.chunk.js"></script><script src="./static/js/main.bf54b1a2.chunk.js"></script></body></html>
```

### Comparing `st-searchbar-0.0.8/st_searchbar/frontend/build/precache-manifest.0e11f5be7ece44b52359d9e1ee04a7d5.js` & `st-searchbar-0.0.9/st_searchbar/frontend/build/precache-manifest.c81079ac31c6a8533bc89850ea3aa800.js`

 * *Files 25% similar despite different names*

#### js-beautify {}

```diff
@@ -1,19 +1,19 @@
 self.__precacheManifest = (self.__precacheManifest || []).concat([{
-    "revision": "f22a32d6c0bf99f3914a672e3aa0373a",
+    "revision": "54968649802b4794685b35493ae19481",
     "url": "./index.html"
 }, {
-    "revision": "185fd26d595f36c3267d",
-    "url": "./static/css/main.cb79e1e0.chunk.css"
+    "revision": "e613c17fd13f8e2a1b3f",
+    "url": "./static/css/main.d8757a26.chunk.css"
 }, {
     "revision": "7ed8f57af007bef77b44",
     "url": "./static/js/2.522574df.chunk.js"
 }, {
     "revision": "3dc2da520b7611f998bec3f8b32ee24e",
     "url": "./static/js/2.522574df.chunk.js.LICENSE.txt"
 }, {
-    "revision": "185fd26d595f36c3267d",
-    "url": "./static/js/main.7bc6fb59.chunk.js"
+    "revision": "e613c17fd13f8e2a1b3f",
+    "url": "./static/js/main.bf54b1a2.chunk.js"
 }, {
     "revision": "7c26bca7e16783d14d15",
     "url": "./static/js/runtime-main.11ec9aca.js"
 }]);
```

### Comparing `st-searchbar-0.0.8/st_searchbar/frontend/build/service-worker.js` & `st-searchbar-0.0.9/st_searchbar/frontend/build/service-worker.js`

 * *Files 11% similar despite different names*

#### js-beautify {}

```diff
@@ -10,15 +10,15 @@
  * and re-run your build process.
  * See https://goo.gl/2aRDsh
  */
 
 importScripts("https://storage.googleapis.com/workbox-cdn/releases/4.3.1/workbox-sw.js");
 
 importScripts(
-    "./precache-manifest.0e11f5be7ece44b52359d9e1ee04a7d5.js"
+    "./precache-manifest.c81079ac31c6a8533bc89850ea3aa800.js"
 );
 
 self.addEventListener('message', (event) => {
     if (event.data && event.data.type === 'SKIP_WAITING') {
         self.skipWaiting();
     }
 });
```

### Comparing `st-searchbar-0.0.8/st_searchbar/frontend/build/static/css/main.cb79e1e0.chunk.css` & `st-searchbar-0.0.9/st_searchbar/frontend/build/static/css/main.d8757a26.chunk.css`

 * *Files 5% similar despite different names*

```diff
@@ -1,2 +1,2 @@
-*,:after,:before{box-sizing:border-box}body{background-color:transparent!important;color:#5a6674!important;font-size:13px;font-family:"Roboto",sans-serif}.search-form{position:relative;left:50%;width:90%;height:40px;border-radius:40px;box-shadow:0 6px 8px rgba(0,0,0,.15);-webkit-transform:translate(-50%);transform:translate(-50%);background:#fff;transition:all .3s ease;overflow:visible}.search-form.focus{box-shadow:0 3px 4px rgba(0,0,0,.15)}.search-input{position:absolute;top:10px;left:38px;font-size:14px;background:none;color:#5a6674;height:20px;border:none;-webkit-appearance:none;appearance:none;outline:none}.search-input::-webkit-search-cancel-button{-webkit-appearance:none;appearance:none}.search-button{position:absolute;top:10px;left:15px;height:20px;width:20px;padding:0;margin:0;border:none;background:none;outline:none!important;cursor:pointer}.search-button svg{width:20px;height:20px;fill:#5a6674}.search-option{position:absolute;text-align:right;top:-4px;right:35px;border:none;outline:none}.search-option div{position:relative;display:inline-block;margin:0 1px;cursor:pointer}.search-option div button{position:absolute;top:0;left:0;background-color:transparent;border:none;outline:none;cursor:pointer}.search-option div svg{height:20px;width:20px;fill:#5a6674;opacity:.6;transition:all .2s ease-in-out;pointer-events:none}.search-option div .recording{fill:#e24040;opacity:1}.search-option div:hover svg{opacity:1}.dropdown{display:flex;overflow:hidden;top:130%;flex-direction:column;border-radius:10px}.scroll{overflow-x:hidden}.scroll::-webkit-scrollbar{width:10px}.scroll::-webkit-scrollbar-thumb{background-color:#d3d3d3;border-radius:20px;border:3px solid #d3d3d3}.scroll::-webkit-scrollbar-thumb:hover{background-color:#c2c2c2;border:3px solid #c2c2c2}.dropdown:empty{border:none}.dropdown-row{padding:10px;cursor:pointer;text-align:start;margin:0}.dropdown-row:hover{background-color:#eee}
-/*# sourceMappingURL=main.cb79e1e0.chunk.css.map */
+*,:after,:before{box-sizing:border-box}body{background-color:transparent!important;color:#5a6674!important;font-size:13px;font-family:"Roboto",sans-serif}.hidden{visibility:hidden}.search-form{position:relative;left:50%;width:90%;height:40px;border-radius:40px;box-shadow:0 6px 8px rgba(0,0,0,.15);-webkit-transform:translate(-50%);transform:translate(-50%);background:#fff;transition:all .3s ease;overflow:visible}.search-form.focus{box-shadow:0 3px 4px rgba(0,0,0,.15)}.search-input{position:absolute;top:10px;left:38px;font-size:14px;background:none;color:#5a6674;height:20px;border:none;-webkit-appearance:none;appearance:none;outline:none}.search-input::-webkit-search-cancel-button{-webkit-appearance:none;appearance:none}.search-button{position:absolute;top:10px;left:15px;height:20px;width:20px;padding:0;margin:0;border:none;background:none;outline:none!important;cursor:pointer}.search-button svg{width:20px;height:20px;fill:#5a6674}.search-option{position:absolute;text-align:right;top:-4px;right:35px;border:none;outline:none}.search-option div{position:relative;display:inline-block;margin:0 1px;cursor:pointer}.search-option div button{position:absolute;top:0;left:0;background-color:transparent;border:none;outline:none;cursor:pointer}.search-option div svg{height:20px;width:20px;fill:#5a6674;opacity:.6;transition:all .2s ease-in-out;pointer-events:none}.search-option div .recording{fill:#e24040;opacity:1}.search-option div:hover svg{opacity:1}.dropdown{display:flex;overflow:hidden;top:130%;flex-direction:column;border-radius:10px}.scroll{overflow-x:hidden}.scroll::-webkit-scrollbar{width:10px}.scroll::-webkit-scrollbar-thumb{background-color:#d3d3d3;border-radius:20px;border:3px solid #d3d3d3}.scroll::-webkit-scrollbar-thumb:hover{background-color:#c2c2c2;border:3px solid #c2c2c2}.dropdown:empty{border:none}.dropdown-row{padding:10px;cursor:pointer;text-align:start;margin:0}.dropdown-row:hover{background-color:#eee}
+/*# sourceMappingURL=main.d8757a26.chunk.css.map */
```

### Comparing `st-searchbar-0.0.8/st_searchbar/frontend/build/static/css/main.cb79e1e0.chunk.css.map` & `st-searchbar-0.0.9/st_searchbar/frontend/build/static/css/main.d8757a26.chunk.css.map`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.75%*

 * *Differences: {"'file'": "'main.d8757a26.chunk.css'",*

 * * "'mappings'": "'AAGA,iBAGE,qBAAA,CAKF,KACE,sCAAA,CACA,uBAAA,CACA,cAAA,CACA,+BAAA,CAGF,QACE,iBAAA,CAMF,aACE,iBAAA,CACA,QAAA,CACA,SAAA,CACA,WAAA,CACA,kBAAA,CACA,oCAAA,CACA,iCAAA,CAAA,yBAAA,CACA,eAAA,CACA,uBAAA,CACA,gBAAA,CAEA,mBACE,oCAAA,CAIJ,cACE,iBAAA,CACA,QAAA,CACA,SAAA,CACA,cAAA,CACA,eAAA,CACA,aAAA,CACA,WAAA,CACA,WAAA,CACA,uBAAA,CAAA,eAAA,CACA,YAAA,CAEA,4CACE,uBAAA,CAAA,eAAA,CAIJ,eACE,iBAAA,CACA,QAAA,CACA,SAAA,CACA,WAAA,CACA,UAAA,CACA,SAAA,CACA,QAAA,CACA,WAAA,CACA, […]*

```diff
@@ -1,12 +1,12 @@
 {
-    "file": "main.cb79e1e0.chunk.css",
-    "mappings": "AAGA,iBAGE,qBAAA,CAKF,KACE,sCAAA,CACA,uBAAA,CACA,cAAA,CACA,+BAAA,CAMF,aACE,iBAAA,CACA,QAAA,CACA,SAAA,CACA,WAAA,CACA,kBAAA,CACA,oCAAA,CACA,iCAAA,CAAA,yBAAA,CACA,eAAA,CACA,uBAAA,CACA,gBAAA,CAEA,mBACE,oCAAA,CAIJ,cACE,iBAAA,CACA,QAAA,CACA,SAAA,CACA,cAAA,CACA,eAAA,CACA,aAAA,CACA,WAAA,CACA,WAAA,CACA,uBAAA,CAAA,eAAA,CACA,YAAA,CAEA,4CACE,uBAAA,CAAA,eAAA,CAIJ,eACE,iBAAA,CACA,QAAA,CACA,SAAA,CACA,WAAA,CACA,UAAA,CACA,SAAA,CACA,QAAA,CACA,WAAA,CACA,eAAA,CACA,sBAAA,CACA,cAAA,CAEA,mBACE,UAAA,CACA,WAAA,CACA,YAAA,CAIJ,eACE,iBAAA,CACA,gBAAA,CACA,QAAA,CACA,UAAA,CACA,WAAA,CACA,YAAA,CAEA,mBACE,iBAAA,CACA,oBAAA,CACA,YAAA,CACA,cAAA,CAEA,0BACE,iBAAA,CACA,KAAA,CACA,MAAA,CACA,4BAAA,CACA,WAAA,CACA,YAAA,CACA,cAAA,CAGF,uBACE,WAAA,CACA,UAAA,CACA,YAAA,CACA,UAAA,CACA,8BAAA,CACA,mBAAA,CAGF,8BACE,YApGE,CAqGF,SAAA,CAGF,6BACE,SAAA,CAKN,UACE,YAAA,CACA,eAAA,CACA,QAAA,CACA,qBAAA,CAEA,kBAAA,CAGF,QACE,iBAAA,CAGF,2BACE,UAAA,CAGF,iCACE,wBAAA,CACA,kBAAA,CACA,wBAAA,CAGF,uCACE,wBAAA,CACA,wBAAA,CAGF,gBACE,WAAA,CAGF,cACE,YAAA,CACA,cAAA,CACA,gBAAA,CACA,QAAA,CAGF,oBACE,qBAAA",
+    "file": "main.d8757a26.chunk.css",
+    "mappings": "AAGA,iBAGE,qBAAA,CAKF,KACE,sCAAA,CACA,uBAAA,CACA,cAAA,CACA,+BAAA,CAGF,QACE,iBAAA,CAMF,aACE,iBAAA,CACA,QAAA,CACA,SAAA,CACA,WAAA,CACA,kBAAA,CACA,oCAAA,CACA,iCAAA,CAAA,yBAAA,CACA,eAAA,CACA,uBAAA,CACA,gBAAA,CAEA,mBACE,oCAAA,CAIJ,cACE,iBAAA,CACA,QAAA,CACA,SAAA,CACA,cAAA,CACA,eAAA,CACA,aAAA,CACA,WAAA,CACA,WAAA,CACA,uBAAA,CAAA,eAAA,CACA,YAAA,CAEA,4CACE,uBAAA,CAAA,eAAA,CAIJ,eACE,iBAAA,CACA,QAAA,CACA,SAAA,CACA,WAAA,CACA,UAAA,CACA,SAAA,CACA,QAAA,CACA,WAAA,CACA,eAAA,CACA,sBAAA,CACA,cAAA,CAEA,mBACE,UAAA,CACA,WAAA,CACA,YAAA,CAIJ,eACE,iBAAA,CACA,gBAAA,CACA,QAAA,CACA,UAAA,CACA,WAAA,CACA,YAAA,CAEA,mBACE,iBAAA,CACA,oBAAA,CACA,YAAA,CACA,cAAA,CAEA,0BACE,iBAAA,CACA,KAAA,CACA,MAAA,CACA,4BAAA,CACA,WAAA,CACA,YAAA,CACA,cAAA,CAGF,uBACE,WAAA,CACA,UAAA,CACA,YAAA,CACA,UAAA,CACA,8BAAA,CACA,mBAAA,CAGF,8BACE,YAxGE,CAyGF,SAAA,CAGF,6BACE,SAAA,CAKN,UACE,YAAA,CACA,eAAA,CACA,QAAA,CACA,qBAAA,CAEA,kBAAA,CAGF,QACE,iBAAA,CAGF,2BACE,UAAA,CAGF,iCACE,wBAAA,CACA,kBAAA,CACA,wBAAA,CAGF,uCACE,wBAAA,CACA,wBAAA,CAGF,gBACE,WAAA,CAGF,cACE,YAAA,CACA,cAAA,CACA,gBAAA,CACA,QAAA,CAGF,oBACE,qBAAA",
     "names": [],
     "sources": [
         "styles.scss"
     ],
     "sourcesContent": [
-        "/*--------------------\r\nBody\r\n--------------------*/\r\n*,\r\n*::before,\r\n*::after {\r\n  box-sizing: border-box;\r\n}\r\n\r\n$color: #e24040;\r\n\r\nbody {\r\n  background-color: transparent !important;\r\n  color: #5a6674 !important;\r\n  font-size: 13px;\r\n  font-family: 'Roboto', sans-serif;\r\n}\r\n\r\n/*--------------------\r\nApp\r\n--------------------*/\r\n.search-form {\r\n  position: relative;\r\n  left: 50%;\r\n  width: 90%;\r\n  height: 40px;\r\n  border-radius: 40px;\r\n  box-shadow: 0 6px 8px rgba(0, 0, 0, 0.15);\r\n  transform: translate(-50%, 0%);\r\n  background: #fff;\r\n  transition: all 0.3s ease;\r\n  overflow:visible;\r\n\r\n  &.focus {\r\n    box-shadow: 0 3px 4px rgba(0, 0, 0, 0.15);\r\n  }\r\n}\r\n\r\n.search-input {\r\n  position: absolute;\r\n  top: 10px;\r\n  left: 38px;\r\n  font-size: 14px;\r\n  background: none;\r\n  color: #5a6674;\r\n  height: 20px;\r\n  border: none;\r\n  appearance: none;\r\n  outline: none;\r\n\r\n  &::-webkit-search-cancel-button {\r\n    appearance: none;\r\n  }\r\n}\r\n\r\n.search-button {\r\n  position: absolute;\r\n  top: 10px;\r\n  left: 15px;\r\n  height: 20px;\r\n  width: 20px;\r\n  padding: 0;\r\n  margin: 0;\r\n  border: none;\r\n  background: none;\r\n  outline: none!important;\r\n  cursor: pointer;\r\n  \r\n  & svg {\r\n    width: 20px;\r\n    height: 20px;\r\n    fill: #5a6674;\r\n  }\r\n}\r\n\r\n.search-option {\r\n  position: absolute;\r\n  text-align: right;\r\n  top: -4px;\r\n  right: 35px;\r\n  border: none;\r\n  outline: none;\r\n\r\n  div {\r\n    position: relative;\r\n    display: inline-block;\r\n    margin: 0 1px;\r\n    cursor: pointer;\r\n    \r\n    button {\r\n      position: absolute;\r\n      top: 0;\r\n      left: 0;\r\n      background-color: transparent;\r\n      border: none;\r\n      outline: none;\r\n      cursor: pointer;\r\n    }\r\n\r\n    svg {\r\n      height: 20px;\r\n      width: 20px;\r\n      fill: #5a6674;\r\n      opacity: 0.6;\r\n      transition: all .2s ease-in-out;\r\n      pointer-events: none;\r\n    }\r\n\r\n    .recording {\r\n      fill: $color;\r\n      opacity: 1;\r\n    }\r\n    \r\n    &:hover svg {\r\n      opacity: 1;\r\n    }\r\n  }\r\n}\r\n\r\n.dropdown {\r\n  display: flex;\r\n  overflow: hidden;\r\n  top: 130%;\r\n  flex-direction: column;\r\n  //border: 1px solid gray;\r\n  border-radius: 10px;\r\n}\r\n\r\n.scroll {\r\n  overflow-x: hidden;\r\n}\r\n\r\n.scroll::-webkit-scrollbar {\r\n  width: 10px;\r\n}\r\n\r\n.scroll::-webkit-scrollbar-thumb {\r\n  background-color: lightgray;\r\n  border-radius: 20px;\r\n  border: 3px solid lightgray;\r\n}\r\n\r\n.scroll::-webkit-scrollbar-thumb:hover {\r\n  background-color: rgb(194, 194, 194);\r\n  border: 3px solid rgb(194, 194, 194);\r\n}\r\n\r\n.dropdown:empty {\r\n  border: none;\r\n}\r\n\r\n.dropdown-row {\r\n  padding: 10px;\r\n  cursor: pointer;\r\n  text-align: start;\r\n  margin: 0;\r\n}\r\n\r\n.dropdown-row:hover {\r\n  background-color: #eee;\r\n}\r\n"
+        "/*--------------------\r\nBody\r\n--------------------*/\r\n*,\r\n*::before,\r\n*::after {\r\n  box-sizing: border-box;\r\n}\r\n\r\n$color: #e24040;\r\n\r\nbody {\r\n  background-color: transparent !important;\r\n  color: #5a6674 !important;\r\n  font-size: 13px;\r\n  font-family: 'Roboto', sans-serif;\r\n}\r\n\r\n.hidden {\r\n  visibility: hidden;\r\n}\r\n\r\n/*--------------------\r\nApp\r\n--------------------*/\r\n.search-form {\r\n  position: relative;\r\n  left: 50%;\r\n  width: 90%;\r\n  height: 40px;\r\n  border-radius: 40px;\r\n  box-shadow: 0 6px 8px rgba(0, 0, 0, 0.15);\r\n  transform: translate(-50%, 0%);\r\n  background: #fff;\r\n  transition: all 0.3s ease;\r\n  overflow:visible;\r\n\r\n  &.focus {\r\n    box-shadow: 0 3px 4px rgba(0, 0, 0, 0.15);\r\n  }\r\n}\r\n\r\n.search-input {\r\n  position: absolute;\r\n  top: 10px;\r\n  left: 38px;\r\n  font-size: 14px;\r\n  background: none;\r\n  color: #5a6674;\r\n  height: 20px;\r\n  border: none;\r\n  appearance: none;\r\n  outline: none;\r\n\r\n  &::-webkit-search-cancel-button {\r\n    appearance: none;\r\n  }\r\n}\r\n\r\n.search-button {\r\n  position: absolute;\r\n  top: 10px;\r\n  left: 15px;\r\n  height: 20px;\r\n  width: 20px;\r\n  padding: 0;\r\n  margin: 0;\r\n  border: none;\r\n  background: none;\r\n  outline: none!important;\r\n  cursor: pointer;\r\n  \r\n  & svg {\r\n    width: 20px;\r\n    height: 20px;\r\n    fill: #5a6674;\r\n  }\r\n}\r\n\r\n.search-option {\r\n  position: absolute;\r\n  text-align: right;\r\n  top: -4px;\r\n  right: 35px;\r\n  border: none;\r\n  outline: none;\r\n\r\n  div {\r\n    position: relative;\r\n    display: inline-block;\r\n    margin: 0 1px;\r\n    cursor: pointer;\r\n    \r\n    button {\r\n      position: absolute;\r\n      top: 0;\r\n      left: 0;\r\n      background-color: transparent;\r\n      border: none;\r\n      outline: none;\r\n      cursor: pointer;\r\n    }\r\n\r\n    svg {\r\n      height: 20px;\r\n      width: 20px;\r\n      fill: #5a6674;\r\n      opacity: 0.6;\r\n      transition: all .2s ease-in-out;\r\n      pointer-events: none;\r\n    }\r\n\r\n    .recording {\r\n      fill: $color;\r\n      opacity: 1;\r\n    }\r\n    \r\n    &:hover svg {\r\n      opacity: 1;\r\n    }\r\n  }\r\n}\r\n\r\n.dropdown {\r\n  display: flex;\r\n  overflow: hidden;\r\n  top: 130%;\r\n  flex-direction: column;\r\n  //border: 1px solid gray;\r\n  border-radius: 10px;\r\n}\r\n\r\n.scroll {\r\n  overflow-x: hidden;\r\n}\r\n\r\n.scroll::-webkit-scrollbar {\r\n  width: 10px;\r\n}\r\n\r\n.scroll::-webkit-scrollbar-thumb {\r\n  background-color: lightgray;\r\n  border-radius: 20px;\r\n  border: 3px solid lightgray;\r\n}\r\n\r\n.scroll::-webkit-scrollbar-thumb:hover {\r\n  background-color: rgb(194, 194, 194);\r\n  border: 3px solid rgb(194, 194, 194);\r\n}\r\n\r\n.dropdown:empty {\r\n  border: none;\r\n}\r\n\r\n.dropdown-row {\r\n  padding: 10px;\r\n  cursor: pointer;\r\n  text-align: start;\r\n  margin: 0;\r\n}\r\n\r\n.dropdown-row:hover {\r\n  background-color: #eee;\r\n}\r\n"
     ],
     "version": 3
 }
```

### Comparing `st-searchbar-0.0.8/st_searchbar/frontend/build/static/js/2.522574df.chunk.js` & `st-searchbar-0.0.9/st_searchbar/frontend/build/static/js/2.522574df.chunk.js`

 * *Files identical despite different names*

### Comparing `st-searchbar-0.0.8/st_searchbar/frontend/build/static/js/2.522574df.chunk.js.LICENSE.txt` & `st-searchbar-0.0.9/st_searchbar/frontend/build/static/js/2.522574df.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `st-searchbar-0.0.8/st_searchbar/frontend/build/static/js/2.522574df.chunk.js.map` & `st-searchbar-0.0.9/st_searchbar/frontend/build/static/js/2.522574df.chunk.js.map`

 * *Files identical despite different names*

### Comparing `st-searchbar-0.0.8/st_searchbar/frontend/build/static/js/main.7bc6fb59.chunk.js` & `st-searchbar-0.0.9/st_searchbar/frontend/build/static/js/main.bf54b1a2.chunk.js`

 * *Files 7% similar despite different names*

#### js-beautify {}

```diff
@@ -6,83 +6,89 @@
         21: function(e, t, n) {},
         22: function(e, t, n) {
             "use strict";
             n.r(t);
             var a = n(5),
                 o = n.n(a),
                 s = n(12),
-                r = n.n(s),
-                l = n(0),
-                i = n(1),
-                u = n(2),
-                c = n(3),
+                i = n.n(s),
+                r = n(0),
+                l = n(1),
+                c = n(2),
+                u = n(3),
                 v = n(8),
                 d = (n(21), function(e) {
-                    Object(u.a)(n, e);
-                    var t = Object(c.a)(n);
+                    Object(c.a)(n, e);
+                    var t = Object(u.a)(n);
 
                     function n(e) {
                         var a;
-                        Object(i.a)(this, n), (a = t.call(this, e)).render = function() {
-                            var e, t, n, s, r = new(0, window.webkitSpeechRecognition);
-                            r.interimResults = !0, r.onresult = function(e) {
-                                var t = Array.from(e.results).map((function(e) {
-                                    return e[0]
-                                })).map((function(e) {
-                                    return e.transcript
-                                })).join("");
-                                a.setState({
-                                    value: t
-                                })
-                            }, r.onend = function() {
-                                a.onSearch(), a.setState({
-                                    isListening: !1
-                                })
-                            };
-                            var l = a.props.args.subtext,
-                                i = a.props.args.suggestions,
-                                u = a.props.args.value,
-                                c = a.props.args.width;
-                            return u && a.setState({
-                                value: u
+                        Object(l.a)(this, n), (a = t.call(this, e)).render = function() {
+                            var e, t, n, s, i = !0,
+                                r = function() {};
+                            if ("SpeechRecognition" in window || "webkitSpeechRecognition" in window) {
+                                var l = new(0, window.webkitSpeechRecognition);
+                                l.interimResults = !0, l.onresult = function(e) {
+                                    var t = Array.from(e.results).map((function(e) {
+                                        return e[0]
+                                    })).map((function(e) {
+                                        return e.transcript
+                                    })).join("");
+                                    a.setState({
+                                        value: t
+                                    })
+                                }, l.onend = function() {
+                                    a.onSearch(), a.setState({
+                                        isListening: !1
+                                    })
+                                }, r = function() {
+                                    var e;
+                                    (null === (e = a.state) || void 0 === e ? void 0 : e.isListening) || l.start(), a.setState({
+                                        isListening: !0
+                                    })
+                                }
+                            } else i = !1;
+                            var c = a.props.args.subtext,
+                                u = a.props.args.suggestions,
+                                v = a.props.args.value,
+                                d = a.props.args.width;
+                            return v && a.setState({
+                                value: v
                             }), o.a.createElement("span", null, o.a.createElement("div", {
                                 className: "search-form"
                             }, o.a.createElement("input", {
                                 type: "text",
                                 onFocus: a.onFocus,
                                 onBlur: a.onBlur,
                                 value: null === (e = a.state) || void 0 === e ? void 0 : e.value,
-                                placeholder: l,
+                                placeholder: c,
                                 onKeyPress: a._handleKeyDown,
                                 onChange: a.onChange,
                                 className: "search-input",
                                 style: {
-                                    width: c
+                                    width: d
                                 }
                             }), o.a.createElement("button", {
                                 type: "button",
                                 className: "search-button",
                                 onClick: a.onSearch
                             }, o.a.createElement("svg", {
                                 className: "submit-button"
                             }, o.a.createElement("use", {
                                 xmlnsXlink: "http://www.w3.org/1999/xlink",
                                 xlinkHref: "#search"
                             }))), o.a.createElement("div", {
                                 className: "search-option"
-                            }, o.a.createElement("div", null, o.a.createElement("button", {
+                            }, o.a.createElement("div", {
+                                className: i ? "" : "hidden"
+                            }, o.a.createElement("button", {
                                 type: "button",
                                 onFocus: a.onFocus,
                                 onBlur: a.onBlur,
-                                onClick: function() {
-                                    var e;
-                                    (null === (e = a.state) || void 0 === e ? void 0 : e.isListening) || r.start(), a.setState({
-                                        isListening: !0
-                                    })
-                                }
+                                onClick: r
                             }, o.a.createElement("svg", {
                                 id: "record-button",
                                 className: (null === (t = a.state) || void 0 === t ? void 0 : t.isListening) ? "recording" : ""
                             }, o.a.createElement("use", {
                                 xmlnsXlink: "http://www.w3.org/1999/xlink",
                                 xlinkHref: "#user"
                             }))))), o.a.createElement("div", {
@@ -93,15 +99,15 @@
                                 }
                             }, o.a.createElement("div", {
                                 className: "scroll",
                                 style: {
                                     maxHeight: (null === (n = a.state) || void 0 === n ? void 0 : n.isActive) ? 100 : "initial",
                                     overflowY: (null === (s = a.state) || void 0 === s ? void 0 : s.isActive) ? "scroll" : "hidden"
                                 }
-                            }, null === i || void 0 === i ? void 0 : i.filter((function(e) {
+                            }, null === u || void 0 === u ? void 0 : u.filter((function(e) {
                                 var t, n;
                                 if (null === (t = a.state) || void 0 === t ? void 0 : t.isActive) {
                                     if (null != (null === (n = a.state) || void 0 === n ? void 0 : n.value) && "" != a.state.value) {
                                         var o = a.state.value.toLowerCase(),
                                             s = e.toLowerCase();
                                         return o && s.startsWith(o) && s !== o
                                     }
@@ -167,18 +173,18 @@
                         var s = a.props.args.default;
                         return null != s && (a.state = {
                             value: s,
                             isListening: !1,
                             isActive: !1
                         }), console.log(s), a
                     }
-                    return Object(l.a)(n)
+                    return Object(r.a)(n)
                 }(v.b)),
                 m = Object(v.c)(d);
-            r.a.render(o.a.createElement(o.a.StrictMode, null, o.a.createElement(m, null)), document.getElementById("root"))
+            i.a.render(o.a.createElement(o.a.StrictMode, null, o.a.createElement(m, null)), document.getElementById("root"))
         }
     },
     [
         [14, 1, 2]
     ]
 ]);
-//# sourceMappingURL=main.7bc6fb59.chunk.js.map
+//# sourceMappingURL=main.bf54b1a2.chunk.js.map
```

### Comparing `st-searchbar-0.0.8/st_searchbar/frontend/build/static/js/main.7bc6fb59.chunk.js.map` & `st-searchbar-0.0.9/st_searchbar/frontend/build/static/js/main.bf54b1a2.chunk.js.map`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8024691358024691%*

 * *Differences: {"'file'": "'static/js/main.bf54b1a2.chunk.js'",*

 * * "'mappings'": "'qRAoBMA,G,wDACJ,WAAmBC,GAAwB,IAAD,uBACxC,cAAMA,IAYDC,OAAS,WAAkB,IAAD,QAC3BC,GAAkB,EAClBC,EAAS,aACb,GAAI,sBAAuBC,QAAU,4BAA6BA,OAClE,CACE,IACMC,EAAS,IAAIC,EADQF,OAAeG,yBAE1CF,EAAOG,gBAAiB,EAExBH,EAAOI,SAAW,SAACC,GACjB,IAAMC,EAAOC,MAAMC,KAAKH,EAAMI,SACzBC,KAAI,SAACC,GAAD,OAAiBA,EAAO,MAC5BD,KAAI,SAACC,GAAD,OAAiBA,EAAOC,cAC5BC,KAAK,IAEV,EAAKC,SAAS,CAACC,MAAOT,KAGxBN,EAAOgB,MAAQ,WACb,EAAKC,WACL,EAAKH,SAAS,CAACI,aAAa,KAG9BpB,EAAS,WAAO,IAAD,GACT,UAAC […]*

```diff
@@ -1,17 +1,19 @@
 {
-    "file": "static/js/main.7bc6fb59.chunk.js",
-    "mappings": "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",
+    "file": "static/js/main.bf54b1a2.chunk.js",
+    "mappings": "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",
     "names": [
         "SearchBarComponent",
         "props",
         "render",
+        "speechAvailable",
+        "listen",
+        "window",
         "speech",
         "SpeechRecognition",
-        "window",
         "webkitSpeechRecognition",
         "interimResults",
         "onresult",
         "event",
         "text",
         "Array",
         "from",
@@ -21,34 +23,34 @@
         "transcript",
         "join",
         "setState",
         "value",
         "onend",
         "onSearch",
         "isListening",
+        "state",
+        "start",
         "subtext",
         "args",
         "suggestions",
         "input",
         "textwidth",
         "className",
         "type",
         "onFocus",
         "onBlur",
-        "state",
         "placeholder",
         "onKeyPress",
         "_handleKeyDown",
         "onChange",
         "style",
         "width",
         "onClick",
         "xmlnsXlink",
         "xlinkHref",
-        "start",
         "id",
         "backgroundColor",
         "boxShadow",
         "maxHeight",
         "isActive",
         "overflowY",
         "filter",
@@ -81,12 +83,12 @@
     ],
     "sourceRoot": "",
     "sources": [
         "SearchBarComponent.tsx",
         "index.tsx"
     ],
     "sourcesContent": [
-        "import {\r\n  ComponentProps,\r\n  Streamlit,\r\n  StreamlitComponentBase,\r\n  withStreamlitConnection,\r\n} from \"streamlit-component-lib\"\r\nimport React, { useState, ReactNode } from \"react\"\r\nimport \"./styles.scss\"\r\nimport { FamilyRestroomOutlined } from \"@mui/icons-material\"\r\n\r\ninterface State {\r\n  value: string\r\n  isListening: boolean\r\n  isActive: boolean\r\n}\r\n\r\n/**\r\n * This is a React-based component template. The `render()` function is called\r\n * automatically when your component should be re-rendered.\r\n */\r\nclass SearchBarComponent extends StreamlitComponentBase<State> {\r\n  public constructor(props: ComponentProps) {\r\n    super(props)\r\n\r\n    // Determine our initially selected index\r\n    const defaultValue = this.props.args[\"default\"]\r\n\r\n    if (defaultValue != null) {\r\n      this.state = { value: defaultValue as string, isListening: false, isActive: false}\r\n    }\r\n\r\n    console.log(defaultValue)\r\n  }\r\n\r\n  public render = (): ReactNode => {    \r\n    const SpeechRecognition = (window as any).webkitSpeechRecognition;\r\n    const speech = new SpeechRecognition();\r\n    speech.interimResults = true;\r\n\r\n    speech.onresult = (event: any) => {\r\n      const text = Array.from(event.results)\r\n          .map((result: any) => result[0])\r\n          .map((result: any) => result.transcript)\r\n          .join('');\r\n\r\n      this.setState({value: text});\r\n    };\r\n\r\n    speech.onend = () => {\r\n      this.onSearch();\r\n      this.setState({isListening: false})\r\n    }\r\n\r\n    const listen = () => {\r\n      if (!this.state?.isListening) {\r\n        speech.start();\r\n      }\r\n      this.setState({isListening: true})\r\n    };\r\n\r\n    const subtext = this.props.args[\"subtext\"]\r\n    const suggestions = this.props.args[\"suggestions\"]\r\n    const input = this.props.args[\"value\"]\r\n    const textwidth: string = this.props.args[\"width\"]\r\n\r\n    if (input) {\r\n      this.setState({value: input});\r\n    }\r\n\r\n    return (\r\n      <span>\r\n        <div className=\"search-form\">\r\n          <input type=\"text\" onFocus={this.onFocus} onBlur={this.onBlur} \r\n                value={this.state?.value} placeholder={subtext} \r\n                onKeyPress={this._handleKeyDown} onChange={this.onChange}\r\n                className=\"search-input\" style={{width: textwidth}}></input>\r\n\r\n          <button type=\"button\" className=\"search-button\" onClick={this.onSearch}>\r\n            <svg className=\"submit-button\">\r\n              <use xmlnsXlink=\"http://www.w3.org/1999/xlink\" xlinkHref=\"#search\"></use>\r\n            </svg>\r\n          </button>\r\n          <div className=\"search-option\">\r\n            <div>\r\n              <button type=\"button\" onFocus={this.onFocus}\r\n                      onBlur={this.onBlur} onClick={listen}>\r\n                <svg id=\"record-button\" className={this.state?.isListening ? \"recording\" : \"\"}>\r\n                  <use xmlnsXlink=\"http://www.w3.org/1999/xlink\" xlinkHref=\"#user\"></use>\r\n                </svg>\r\n              </button>\r\n            </div>\r\n          </div>\r\n          <div className=\"dropdown\" style={{backgroundColor: 'white', \r\n                                            boxShadow: '0 6px 8px rgba(0, 0, 0, 0.15)'}}>\r\n            <div className=\"scroll\" style={{maxHeight: (this.state?.isActive ? 100 : 'initial'),\r\n                                            overflowY: (this.state?.isActive ? 'scroll' : 'hidden')}}>\r\n              {\r\n                suggestions?.filter((item: string) => {\r\n                  if (!this.state?.isActive) {\r\n                    return '';\r\n                  } else if (this.state?.value != null && this.state.value != \"\") {\r\n                    const searchTerm = this.state.value.toLowerCase();\r\n                    const suggestion = item.toLowerCase();\r\n\r\n                    return searchTerm && suggestion.startsWith(searchTerm)\r\n                          && suggestion !== searchTerm;\r\n                  } else {\r\n                    return item;\r\n                  }\r\n                })\r\n                .map((suggestion: string) => \r\n                  <div className=\"dropdown-row\" \r\n                        onMouseDown={() => this.setSuggestion(suggestion)}>\r\n                          {suggestion}\r\n                  </div>)\r\n              }\r\n            </div>\r\n          </div>\r\n          <div className=\"dropdown\">&nbsp;</div>\r\n        </div>\r\n\r\n        <svg xmlns=\"http://www.w3.org/2000/svg\" width=\"0\" height=\"0\" display=\"none\">\r\n          <symbol id=\"search\" viewBox=\"0 0 32 32\">\r\n            <path d=\"M 19.5 3 C 14.26514 3 10 7.2651394 10 12.5 C 10 14.749977 10.810825 16.807458 12.125 18.4375 L 3.28125 27.28125 L 4.71875 28.71875 L 13.5625 19.875 C 15.192542 21.189175 17.250023 22 19.5 22 C 24.73486 22 29 17.73486 29 12.5 C 29 7.2651394 24.73486 3 19.5 3 z M 19.5 5 C 23.65398 5 27 8.3460198 27 12.5 C 27 16.65398 23.65398 20 19.5 20 C 15.34602 20 12 16.65398 12 12.5 C 12 8.3460198 15.34602 5 19.5 5 z\" />\r\n          </symbol>\r\n          <symbol id=\"user\" viewBox=\"0 0 18 18\">\r\n            <path d=\"M3.5 6.5A.5.5 0 0 1 4 7v1a4 4 0 0 0 8 0V7a.5.5 0 0 1 1 0v1a5 5 0 0 1-4.5 4.975V15h3a.5.5 0 0 1 0 1h-7a.5.5 0 0 1 0-1h3v-2.025A5 5 0 0 1 3 8V7a.5.5 0 0 1 .5-.5z\"/>\r\n            <path d=\"M10 8a2 2 0 1 1-4 0V3a2 2 0 1 1 4 0v5zM8 0a3 3 0 0 0-3 3v5a3 3 0 0 0 6 0V3a3 3 0 0 0-3-3z\"/>\r\n          </symbol>\r\n        </svg> \r\n      </span>\r\n    )\r\n  }\r\n\r\n  private onChange = (event: any) => {\r\n    this.setState({value: event.target.value})\r\n  }\r\n\r\n  private setSuggestion = (suggestion: string) => {\r\n    this.setState(\r\n                  {value: suggestion},\r\n                  () => Streamlit.setComponentValue(this.state?.value)\r\n                 )\r\n  }\r\n\r\n  private onFocus = (event: any) => {\r\n    this.setState({isActive: true});\r\n  }\r\n\r\n  private onBlur = (event: any) => {\r\n    this.setState({isActive: false});\r\n  }\r\n\r\n  private onSearch = (): void => {\r\n    this.setState(\r\n      () => Streamlit.setComponentValue(this.state?.value)\r\n    )\r\n  }\r\n\r\n  private _handleKeyDown = (e: React.KeyboardEvent<HTMLInputElement>) => {\r\n    if (e.key === 'Enter') {\r\n      this.setState(\r\n        () => Streamlit.setComponentValue(this.state.value)\r\n      )\r\n    }\r\n  }\r\n\r\n  // /** Click handler for our \"Click Me!\" button. */\r\n  // private onClicked = (): void => {\r\n  //   // Increment state.numClicks, and pass the new value back to\r\n  //   // Streamlit via `Streamlit.setComponentValue`.\r\n  //   this.setState(\r\n  //     prevState => ({ numClicks: prevState.numClicks + 1 }),\r\n  //     () => Streamlit.setComponentValue(this.state.numClicks)\r\n  //   )\r\n  // }\r\n\r\n  // /** Focus handler for our \"Click Me!\" button. */\r\n  // private _onFocus = (): void => {\r\n  //   this.setState({ isFocused: true })\r\n  // }\r\n\r\n  // /** Blur handler for our \"Click Me!\" button. */\r\n  // private _onBlur = (): void => {\r\n  //   this.setState({ isFocused: false })\r\n  // }\r\n}\r\n\r\n// \"withStreamlitConnection\" is a wrapper function. It bootstraps the\r\n// connection between your component and the Streamlit app, and handles\r\n// passing arguments from Python -> Component.\r\n//\r\n// You don't need to edit withStreamlitConnection (but you're welcome to!).\r\nexport default withStreamlitConnection(SearchBarComponent)\r\n",
+        "import {\r\n  ComponentProps,\r\n  Streamlit,\r\n  StreamlitComponentBase,\r\n  withStreamlitConnection,\r\n} from \"streamlit-component-lib\"\r\nimport React, { useState, ReactNode } from \"react\"\r\nimport \"./styles.scss\"\r\nimport { FamilyRestroomOutlined } from \"@mui/icons-material\"\r\n\r\ninterface State {\r\n  value: string\r\n  isListening: boolean\r\n  isActive: boolean\r\n}\r\n\r\n/**\r\n * This is a React-based component template. The `render()` function is called\r\n * automatically when your component should be re-rendered.\r\n */\r\nclass SearchBarComponent extends StreamlitComponentBase<State> {\r\n  public constructor(props: ComponentProps) {\r\n    super(props)\r\n\r\n    // Determine our initially selected index\r\n    const defaultValue = this.props.args[\"default\"]\r\n\r\n    if (defaultValue != null) {\r\n      this.state = { value: defaultValue as string, isListening: false, isActive: false}\r\n    }\r\n\r\n    console.log(defaultValue)\r\n  }\r\n\r\n  public render = (): ReactNode => {\r\n    var speechAvailable = true;\r\n    var listen = () => {};\r\n    if ('SpeechRecognition' in window || 'webkitSpeechRecognition' in window) \r\n    {\r\n      const SpeechRecognition = (window as any).webkitSpeechRecognition;\r\n      const speech = new SpeechRecognition();\r\n      speech.interimResults = true;\r\n  \r\n      speech.onresult = (event: any) => {\r\n        const text = Array.from(event.results)\r\n            .map((result: any) => result[0])\r\n            .map((result: any) => result.transcript)\r\n            .join('');\r\n  \r\n        this.setState({value: text});\r\n      };\r\n  \r\n      speech.onend = () => {\r\n        this.onSearch();\r\n        this.setState({isListening: false})\r\n      }\r\n  \r\n      listen = () => {\r\n        if (!this.state?.isListening) {\r\n          speech.start();\r\n        }\r\n        this.setState({isListening: true})\r\n      };\r\n    } else {\r\n      speechAvailable = false;\r\n    }\r\n\r\n    const subtext = this.props.args[\"subtext\"]\r\n    const suggestions = this.props.args[\"suggestions\"]\r\n    const input = this.props.args[\"value\"]\r\n    const textwidth: string = this.props.args[\"width\"]\r\n\r\n    if (input) {\r\n      this.setState({value: input});\r\n    }\r\n    \r\n    return (\r\n      <span>\r\n        <div className=\"search-form\">\r\n          <input type=\"text\" onFocus={this.onFocus} onBlur={this.onBlur} \r\n                value={this.state?.value} placeholder={subtext} \r\n                onKeyPress={this._handleKeyDown} onChange={this.onChange}\r\n                className=\"search-input\" style={{width: textwidth}}></input>\r\n\r\n          <button type=\"button\" className=\"search-button\" onClick={this.onSearch}>\r\n            <svg className=\"submit-button\">\r\n              <use xmlnsXlink=\"http://www.w3.org/1999/xlink\" xlinkHref=\"#search\"></use>\r\n            </svg>\r\n          </button>\r\n          <div className=\"search-option\">\r\n            <div className={speechAvailable ? \"\" : \"hidden\"}>\r\n              <button type=\"button\" onFocus={this.onFocus}\r\n                      onBlur={this.onBlur} onClick={listen}>\r\n                <svg id=\"record-button\" className={this.state?.isListening ? \"recording\" : \"\"}>\r\n                  <use xmlnsXlink=\"http://www.w3.org/1999/xlink\" xlinkHref=\"#user\"></use>\r\n                </svg>\r\n              </button>\r\n            </div>\r\n          </div>\r\n          <div className=\"dropdown\" style={{backgroundColor: 'white', \r\n                                            boxShadow: '0 6px 8px rgba(0, 0, 0, 0.15)'}}>\r\n            <div className=\"scroll\" style={{maxHeight: (this.state?.isActive ? 100 : 'initial'),\r\n                                            overflowY: (this.state?.isActive ? 'scroll' : 'hidden')}}>\r\n              {\r\n                suggestions?.filter((item: string) => {\r\n                  if (!this.state?.isActive) {\r\n                    return '';\r\n                  } else if (this.state?.value != null && this.state.value != \"\") {\r\n                    const searchTerm = this.state.value.toLowerCase();\r\n                    const suggestion = item.toLowerCase();\r\n\r\n                    return searchTerm && suggestion.startsWith(searchTerm)\r\n                          && suggestion !== searchTerm;\r\n                  } else {\r\n                    return item;\r\n                  }\r\n                })\r\n                .map((suggestion: string) => \r\n                  <div className=\"dropdown-row\" \r\n                        onMouseDown={() => this.setSuggestion(suggestion)}>\r\n                          {suggestion}\r\n                  </div>)\r\n              }\r\n            </div>\r\n          </div>\r\n          <div className=\"dropdown\">&nbsp;</div>\r\n        </div>\r\n\r\n        <svg xmlns=\"http://www.w3.org/2000/svg\" width=\"0\" height=\"0\" display=\"none\">\r\n          <symbol id=\"search\" viewBox=\"0 0 32 32\">\r\n            <path d=\"M 19.5 3 C 14.26514 3 10 7.2651394 10 12.5 C 10 14.749977 10.810825 16.807458 12.125 18.4375 L 3.28125 27.28125 L 4.71875 28.71875 L 13.5625 19.875 C 15.192542 21.189175 17.250023 22 19.5 22 C 24.73486 22 29 17.73486 29 12.5 C 29 7.2651394 24.73486 3 19.5 3 z M 19.5 5 C 23.65398 5 27 8.3460198 27 12.5 C 27 16.65398 23.65398 20 19.5 20 C 15.34602 20 12 16.65398 12 12.5 C 12 8.3460198 15.34602 5 19.5 5 z\" />\r\n          </symbol>\r\n          <symbol id=\"user\" viewBox=\"0 0 18 18\">\r\n            <path d=\"M3.5 6.5A.5.5 0 0 1 4 7v1a4 4 0 0 0 8 0V7a.5.5 0 0 1 1 0v1a5 5 0 0 1-4.5 4.975V15h3a.5.5 0 0 1 0 1h-7a.5.5 0 0 1 0-1h3v-2.025A5 5 0 0 1 3 8V7a.5.5 0 0 1 .5-.5z\"/>\r\n            <path d=\"M10 8a2 2 0 1 1-4 0V3a2 2 0 1 1 4 0v5zM8 0a3 3 0 0 0-3 3v5a3 3 0 0 0 6 0V3a3 3 0 0 0-3-3z\"/>\r\n          </symbol>\r\n        </svg> \r\n      </span>\r\n    )\r\n  }\r\n\r\n  private onChange = (event: any) => {\r\n    this.setState({value: event.target.value})\r\n  }\r\n\r\n  private setSuggestion = (suggestion: string) => {\r\n    this.setState(\r\n                  {value: suggestion},\r\n                  () => Streamlit.setComponentValue(this.state?.value)\r\n                 )\r\n  }\r\n\r\n  private onFocus = (event: any) => {\r\n    this.setState({isActive: true});\r\n  }\r\n\r\n  private onBlur = (event: any) => {\r\n    this.setState({isActive: false});\r\n  }\r\n\r\n  private onSearch = (): void => {\r\n    this.setState(\r\n      () => Streamlit.setComponentValue(this.state?.value)\r\n    )\r\n  }\r\n\r\n  private _handleKeyDown = (e: React.KeyboardEvent<HTMLInputElement>) => {\r\n    if (e.key === 'Enter') {\r\n      this.setState(\r\n        () => Streamlit.setComponentValue(this.state.value)\r\n      )\r\n    }\r\n  }\r\n\r\n  // /** Click handler for our \"Click Me!\" button. */\r\n  // private onClicked = (): void => {\r\n  //   // Increment state.numClicks, and pass the new value back to\r\n  //   // Streamlit via `Streamlit.setComponentValue`.\r\n  //   this.setState(\r\n  //     prevState => ({ numClicks: prevState.numClicks + 1 }),\r\n  //     () => Streamlit.setComponentValue(this.state.numClicks)\r\n  //   )\r\n  // }\r\n\r\n  // /** Focus handler for our \"Click Me!\" button. */\r\n  // private _onFocus = (): void => {\r\n  //   this.setState({ isFocused: true })\r\n  // }\r\n\r\n  // /** Blur handler for our \"Click Me!\" button. */\r\n  // private _onBlur = (): void => {\r\n  //   this.setState({ isFocused: false })\r\n  // }\r\n}\r\n\r\n// \"withStreamlitConnection\" is a wrapper function. It bootstraps the\r\n// connection between your component and the Streamlit app, and handles\r\n// passing arguments from Python -> Component.\r\n//\r\n// You don't need to edit withStreamlitConnection (but you're welcome to!).\r\nexport default withStreamlitConnection(SearchBarComponent)\r\n",
         "import React from \"react\"\r\nimport ReactDOM from \"react-dom\"\r\nimport SearchBarComponent from \"./SearchBarComponent\"\r\n\r\nReactDOM.render(\r\n  <React.StrictMode>\r\n    <SearchBarComponent />\r\n  </React.StrictMode>,\r\n  document.getElementById(\"root\")\r\n)\r\n"
     ],
     "version": 3
 }
```

### Comparing `st-searchbar-0.0.8/st_searchbar/frontend/build/static/js/runtime-main.11ec9aca.js` & `st-searchbar-0.0.9/st_searchbar/frontend/build/static/js/runtime-main.11ec9aca.js`

 * *Files identical despite different names*

### Comparing `st-searchbar-0.0.8/st_searchbar/frontend/build/static/js/runtime-main.11ec9aca.js.map` & `st-searchbar-0.0.9/st_searchbar/frontend/build/static/js/runtime-main.11ec9aca.js.map`

 * *Files identical despite different names*

### Comparing `st-searchbar-0.0.8/st_searchbar.egg-info/SOURCES.txt` & `st-searchbar-0.0.9/st_searchbar.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 st_searchbar.egg-info/SOURCES.txt
 st_searchbar.egg-info/dependency_links.txt
 st_searchbar.egg-info/requires.txt
 st_searchbar.egg-info/top_level.txt
 st_searchbar/frontend/build/asset-manifest.json
 st_searchbar/frontend/build/bootstrap.min.css
 st_searchbar/frontend/build/index.html
-st_searchbar/frontend/build/precache-manifest.0e11f5be7ece44b52359d9e1ee04a7d5.js
+st_searchbar/frontend/build/precache-manifest.c81079ac31c6a8533bc89850ea3aa800.js
 st_searchbar/frontend/build/service-worker.js
-st_searchbar/frontend/build/static/css/main.cb79e1e0.chunk.css
-st_searchbar/frontend/build/static/css/main.cb79e1e0.chunk.css.map
+st_searchbar/frontend/build/static/css/main.d8757a26.chunk.css
+st_searchbar/frontend/build/static/css/main.d8757a26.chunk.css.map
 st_searchbar/frontend/build/static/js/2.522574df.chunk.js
 st_searchbar/frontend/build/static/js/2.522574df.chunk.js.LICENSE.txt
 st_searchbar/frontend/build/static/js/2.522574df.chunk.js.map
-st_searchbar/frontend/build/static/js/main.7bc6fb59.chunk.js
-st_searchbar/frontend/build/static/js/main.7bc6fb59.chunk.js.map
+st_searchbar/frontend/build/static/js/main.bf54b1a2.chunk.js
+st_searchbar/frontend/build/static/js/main.bf54b1a2.chunk.js.map
 st_searchbar/frontend/build/static/js/runtime-main.11ec9aca.js
 st_searchbar/frontend/build/static/js/runtime-main.11ec9aca.js.map
```

