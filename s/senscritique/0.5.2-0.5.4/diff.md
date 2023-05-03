# Comparing `tmp/senscritique-0.5.2.tar.gz` & `tmp/senscritique-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/senscritique-0.5.2.tar", last modified: Wed Oct 28 15:32:38 2020, max compression
+gzip compressed data, was "senscritique-0.5.4.tar", last modified: Wed May  3 22:44:11 2023, max compression
```

## Comparing `senscritique-0.5.2.tar` & `senscritique-0.5.4.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-28 15:32:38.501838 senscritique-0.5.2/
--rw-r--r--   0 runner    (1001) docker     (116)     3683 2020-10-28 15:32:38.501838 senscritique-0.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     2327 2020-10-28 15:32:29.000000 senscritique-0.5.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-28 15:32:38.501838 senscritique-0.5.2/senscritique/
--rw-r--r--   0 runner    (1001) docker     (116)       56 2020-10-28 15:32:29.000000 senscritique-0.5.2/senscritique/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      454 2020-10-28 15:32:29.000000 senscritique-0.5.2/senscritique/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (116)      525 2020-10-28 15:32:29.000000 senscritique-0.5.2/senscritique/parse_utils.py
--rw-r--r--   0 runner    (1001) docker     (116)     1830 2020-10-28 15:32:29.000000 senscritique-0.5.2/senscritique/process_collection.py
--rw-r--r--   0 runner    (1001) docker     (116)     2795 2020-10-28 15:32:29.000000 senscritique-0.5.2/senscritique/process_critiques.py
--rw-r--r--   0 runner    (1001) docker     (116)     1739 2020-10-28 15:32:29.000000 senscritique-0.5.2/senscritique/process_generic.py
--rw-r--r--   0 runner    (1001) docker     (116)     3025 2020-10-28 15:32:29.000000 senscritique-0.5.2/senscritique/process_listes.py
--rw-r--r--   0 runner    (1001) docker     (116)     1825 2020-10-28 15:32:29.000000 senscritique-0.5.2/senscritique/takeout.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-28 15:32:38.501838 senscritique-0.5.2/senscritique/tests/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-10-28 15:32:29.000000 senscritique-0.5.2/senscritique/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1454 2020-10-28 15:32:29.000000 senscritique-0.5.2/senscritique/tests/test_senscritique.py
--rw-r--r--   0 runner    (1001) docker     (116)      951 2020-10-28 15:32:29.000000 senscritique-0.5.2/senscritique/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-28 15:32:38.501838 senscritique-0.5.2/senscritique.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     3683 2020-10-28 15:32:38.000000 senscritique-0.5.2/senscritique.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      536 2020-10-28 15:32:38.000000 senscritique-0.5.2/senscritique.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-10-28 15:32:38.000000 senscritique-0.5.2/senscritique.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       29 2020-10-28 15:32:38.000000 senscritique-0.5.2/senscritique.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       13 2020-10-28 15:32:38.000000 senscritique-0.5.2/senscritique.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)      118 2020-10-28 15:32:38.501838 senscritique-0.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1107 2020-10-28 15:32:29.000000 senscritique-0.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:44:11.059105 senscritique-0.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-03 22:43:57.000000 senscritique-0.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-05-03 22:44:11.059105 senscritique-0.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-05-03 22:43:57.000000 senscritique-0.5.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:44:11.059105 senscritique-0.5.4/senscritique/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-03 22:43:57.000000 senscritique-0.5.4/senscritique/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-03 22:43:57.000000 senscritique-0.5.4/senscritique/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-05-03 22:43:57.000000 senscritique-0.5.4/senscritique/parse_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-05-03 22:43:57.000000 senscritique-0.5.4/senscritique/process_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-05-03 22:43:57.000000 senscritique-0.5.4/senscritique/process_critiques.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2057 2023-05-03 22:43:57.000000 senscritique-0.5.4/senscritique/process_generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-05-03 22:43:57.000000 senscritique-0.5.4/senscritique/process_listes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-05-03 22:43:57.000000 senscritique-0.5.4/senscritique/takeout.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:44:11.059105 senscritique-0.5.4/senscritique/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 22:43:57.000000 senscritique-0.5.4/senscritique/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-05-03 22:43:57.000000 senscritique-0.5.4/senscritique/tests/test_senscritique.py
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-05-03 22:43:57.000000 senscritique-0.5.4/senscritique/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 22:44:11.059105 senscritique-0.5.4/senscritique.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3049 2023-05-03 22:44:10.000000 senscritique-0.5.4/senscritique.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-05-03 22:44:11.000000 senscritique-0.5.4/senscritique.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 22:44:10.000000 senscritique-0.5.4/senscritique.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-03 22:44:10.000000 senscritique-0.5.4/senscritique.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-03 22:44:10.000000 senscritique-0.5.4/senscritique.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-03 22:44:11.059105 senscritique-0.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-05-03 22:43:57.000000 senscritique-0.5.4/setup.py
```

### Comparing `senscritique-0.5.2/README.md` & `senscritique-0.5.4/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 # SensCritique Takeout
 
 [![PyPI status][pypi-image]][pypi]
 [![Build status][build-image]][build]
-[![Updates][dependency-image]][pyup]
-[![Python 3][python3-image]][pyup]
 [![Code coverage][codecov-image]][codecov]
 [![Code Quality][codacy-image]][codacy]
 
 This repository contains Python code to export your data from [SensCritique.com](https://www.senscritique.com).
 
 ## Installation
 
@@ -57,20 +55,20 @@
 - [Google Takeout](https://en.wikipedia.org/wiki/Google_Takeout)
 
 <!-- Definitions for badges -->
 
 [pypi]: <https://pypi.python.org/pypi/senscritique>
 [pypi-image]: <https://badge.fury.io/py/senscritique.svg>
 
-[build]: <https://github.com/woctezuma/senscritique/actions>
-[build-image]: <https://github.com/woctezuma/senscritique/workflows/Python package/badge.svg?branch=master>
-[publish-image]: <https://github.com/woctezuma/senscritique/workflows/Upload Python Package/badge.svg?branch=master>
-
-[pyup]: <https://pyup.io/repos/github/woctezuma/senscritique/>
-[dependency-image]: <https://pyup.io/repos/github/woctezuma/senscritique/shield.svg>
-[python3-image]: <https://pyup.io/repos/github/woctezuma/senscritique/python-3-shield.svg>
+[build]: <https://github.com/woctezuma/SensCritique-Takeout/actions>
+[build-image]: <https://github.com/woctezuma/SensCritique-Takeout/workflows/Python package/badge.svg?branch=master>
+[publish-image]: <https://github.com/woctezuma/SensCritique-Takeout/workflows/Upload Python Package/badge.svg?branch=master>
+
+[pyup]: <https://pyup.io/repos/github/woctezuma/SensCritique-Takeout/>
+[dependency-image]: <https://pyup.io/repos/github/woctezuma/SensCritique-Takeout/shield.svg>
+[python3-image]: <https://pyup.io/repos/github/woctezuma/SensCritique-Takeout/python-3-shield.svg>
 
-[codecov]: <https://codecov.io/gh/woctezuma/senscritique>
-[codecov-image]: <https://codecov.io/gh/woctezuma/senscritique/branch/master/graph/badge.svg>
+[codecov]: <https://codecov.io/gh/woctezuma/SensCritique-Takeout>
+[codecov-image]: <https://codecov.io/gh/woctezuma/SensCritique-Takeout/branch/master/graph/badge.svg>
 
-[codacy]: <https://www.codacy.com/app/woctezuma/senscritique>
+[codacy]: <https://www.codacy.com/app/woctezuma/SensCritique-Takeout>
 [codacy-image]: <https://api.codacy.com/project/badge/Grade/5414284721184d139b48023a0467858d>
```

### Comparing `senscritique-0.5.2/senscritique/parse_utils.py` & `senscritique-0.5.4/senscritique/parse_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import requests
 from bs4 import BeautifulSoup
 
 
 def get_item_id(soup_name):
-    return soup_name[0].attrs['id'].strip('product-title-')
+    return soup_name[0].attrs['id'].replace('product-title-', '')
 
 
 def get_review_id(soup_name):
     return soup_name[0].attrs['data-sc-review-id']
 
 
 def get_num_pages(url):
```

### Comparing `senscritique-0.5.2/senscritique/process_collection.py` & `senscritique-0.5.4/senscritique/process_collection.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,46 +1,59 @@
+import re
 import requests
 from bs4 import BeautifulSoup
 
-from .parse_utils import get_item_id
-from .utils import get_base_url, read_soup_result
+from senscritique.parse_utils import get_item_id
+from senscritique.utils import get_base_url, read_soup_result
 
 
 def get_collection_url(user_name, page_no=1):
-    url = get_base_url(user_name=user_name) + 'collection/all/all/all/all/all/all/all/all/all/page-' + str(page_no)
+    url = (
+        get_base_url(user_name=user_name)
+        + 'collection/all/all/all/all/all/all/all/all/all/page-'
+        + str(page_no)
+    )
     return url
 
 
 def parse_collection_page(user_name='wok', page_no=1, verbose=False):
     url = get_collection_url(user_name=user_name, page_no=page_no)
     soup = BeautifulSoup(requests.get(url).content, 'lxml')
 
     collection_items = soup.find_all('li', 'elco-collection-item')
 
-    data = dict()
+    data = {}
     for item in collection_items:
         user_rating = item.find_all('div', {'class': 'elco-collection-rating user'})
+        item_type_p = item.find('div', {'class': re.compile("^d-media-[a-z]+$")})
+        item_type = "unknown"
+        if item_type_p:
+            if 'data-sc-play-type' in item_type_p:
+                item_type = item_type_p['data-sc-play-type']
         name = item.find_all('a', {'class': 'elco-anchor'})
         game_system = item.find_all('span', {'class': 'elco-gamesystem'})
         release_date = item.find_all('span', {'class': 'elco-date'})
         description = item.find_all('p', {'class': 'elco-baseline elco-options'})
         author = item.find_all('a', {'class': 'elco-baseline-a'})
         site_rating = item.find_all('a', {'class': 'erra-global'})
 
         item_id = get_item_id(name)
 
-        data[item_id] = dict()
+        data[item_id] = {}
         data[item_id]['name'] = read_soup_result(name)
         data[item_id]['author'] = read_soup_result(author)
         data[item_id]['user_rating'] = read_soup_result(user_rating)
         data[item_id]['site_rating'] = read_soup_result(site_rating)
         data[item_id]['description'] = read_soup_result(description)
         data[item_id]['game_system'] = read_soup_result(game_system)
         data[item_id]['release_date'] = read_soup_result(release_date)
+        data[item_id]['item_type'] = item_type
 
         if verbose:
-            print('-   item n°{}: {}'.format(
-                item_id,
-                data[item_id]['name'],
-            ))
+            print(
+                '-   item n°{}: {}'.format(
+                    item_id,
+                    data[item_id]['name'],
+                ),
+            )
 
     return data
```

### Comparing `senscritique-0.5.2/senscritique/process_critiques.py` & `senscritique-0.5.4/senscritique/process_critiques.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import requests
 from bs4 import BeautifulSoup
 
-from .parse_utils import get_review_id
-from .utils import get_base_url, read_soup_result
+from senscritique.parse_utils import get_review_id
+from senscritique.utils import get_base_url, read_soup_result
 
 
 def get_critiques_url(user_name, page_no=1):
     url = get_base_url(user_name=user_name) + 'critiques/page-' + str(page_no)
 
     return url
 
@@ -14,27 +14,27 @@
 def parse_critiques_page(user_name='wok', page_no=1, verbose=False):
     url = get_critiques_url(user_name=user_name, page_no=page_no)
     print(url)
     soup = BeautifulSoup(requests.get(url).content, 'lxml')
 
     collection_items = soup.find_all('article', {'class': 'ere-review ere-box'})
 
-    review_data = dict()
+    review_data = {}
     for item in collection_items:
         overview = item.find_all('button', {'class': 'ere-review-overview'})
         title = item.find_all('h3', {'class': 'd-heading2 ere-review-heading'})
         excerpt = item.find_all('p', {'class': 'ere-review-excerpt'})
         game_system = item.find_all('span', {'class': 'ere-review-gamesystem'})
         rating = item.find_all('div', {'class': 'elrua-useraction-action'})
         link = item.find_all('a', {'class': 'ere-review-anchor'})
         footer = item.find_all('footer', {'class': 'ere-review-details'})
 
         item_id = get_review_id(overview)
 
-        review_data[item_id] = dict()
+        review_data[item_id] = {}
         review_data[item_id]['title'] = read_soup_result(title)
         review_data[item_id]['excerpt'] = read_soup_result(excerpt)
         review_data[item_id]['game_system'] = read_soup_result(game_system)
         review_data[item_id]['rating'] = read_soup_result(rating)
         review_data[item_id]['link'] = link[0].attrs['href']
         review_data[item_id]['date'] = footer[0].find_all('time')[0].text
 
@@ -53,14 +53,16 @@
             stats = review_item.find_all('div', {'data-rel': 'likebar'})
 
             review_data[item_id]['content'] = read_soup_result(content)
             review_data[item_id]['upvotes'] = stats[0].attrs['data-sc-positive-count']
             review_data[item_id]['downvotes'] = stats[0].attrs['data-sc-negative-count']
 
             if verbose:
-                print('-   item n°{}: (upvotes, downvotes) = ({}, {})'.format(
-                    item_id,
-                    review_data[item_id]['upvotes'],
-                    review_data[item_id]['downvotes'],
-                ))
+                print(
+                    '-   item n°{}: (upvotes, downvotes) = ({}, {})'.format(
+                        item_id,
+                        review_data[item_id]['upvotes'],
+                        review_data[item_id]['downvotes'],
+                    ),
+                )
 
     return review_data
```

### Comparing `senscritique-0.5.2/senscritique/process_generic.py` & `senscritique-0.5.4/senscritique/process_generic.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from .parse_utils import get_num_pages
-from .process_collection import get_collection_url, parse_collection_page
-from .process_critiques import get_critiques_url, parse_critiques_page
-from .process_listes import get_listes_url, parse_listes_page
+from senscritique.parse_utils import get_num_pages
+from senscritique.process_collection import get_collection_url, parse_collection_page
+from senscritique.process_critiques import get_critiques_url, parse_critiques_page
+from senscritique.process_listes import get_listes_url, parse_listes_page
 
 
 def get_keyword_home_url(user_name='wok', keyword='collection'):
     home_page_no = 1
 
     if keyword == 'collection':
         url = get_collection_url(user_name=user_name, page_no=home_page_no)
@@ -15,34 +15,57 @@
         url = get_listes_url(user_name=user_name, page_no=home_page_no)
 
     return url
 
 
 def parse_keyword_page(user_name='wok', keyword='collection', page_no=1, verbose=False):
     if keyword == 'collection':
-        page_data = parse_collection_page(user_name=user_name, page_no=page_no, verbose=verbose)
+        page_data = parse_collection_page(
+            user_name=user_name,
+            page_no=page_no,
+            verbose=verbose,
+        )
     elif keyword == 'critiques':
-        page_data = parse_critiques_page(user_name=user_name, page_no=page_no, verbose=verbose)
+        page_data = parse_critiques_page(
+            user_name=user_name,
+            page_no=page_no,
+            verbose=verbose,
+        )
     else:
-        page_data = parse_listes_page(user_name=user_name, page_no=page_no, verbose=verbose)
+        page_data = parse_listes_page(
+            user_name=user_name,
+            page_no=page_no,
+            verbose=verbose,
+        )
 
     return page_data
 
 
 def parse_keyword(user_name='wok', keyword='collection', verbose=False):
     url = get_keyword_home_url(user_name=user_name, keyword=keyword)
 
     num_pages = get_num_pages(url)
 
-    print('Parsing {} pages of {} by {}.'.format(num_pages, keyword, user_name))
+    print(f'Parsing {num_pages} pages of {keyword} by {user_name}.')
 
-    data = dict()
+    data = {}
     for page_no in range(num_pages):
         real_page_no = page_no + 1
 
-        page_data = parse_keyword_page(user_name=user_name, keyword=keyword, page_no=real_page_no, verbose=verbose)
-
-        print('[{} ; page n°{}] num_items = {}'.format(keyword, real_page_no, len(page_data)))
+        page_data = parse_keyword_page(
+            user_name=user_name,
+            keyword=keyword,
+            page_no=real_page_no,
+            verbose=verbose,
+        )
+
+        print(
+            '[{} ; page n°{}] num_items = {}'.format(
+                keyword,
+                real_page_no,
+                len(page_data),
+            ),
+        )
 
         data.update(page_data)
 
     return data
```

### Comparing `senscritique-0.5.2/senscritique/process_listes.py` & `senscritique-0.5.4/senscritique/process_listes.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,81 +1,94 @@
 import requests
 from bs4 import BeautifulSoup
 
-from .parse_utils import get_item_id, get_num_pages
-from .utils import get_base_url, read_soup_result
-from .utils import get_url_for_liste
+from senscritique.parse_utils import get_item_id, get_num_pages
+from senscritique.utils import get_base_url, get_url_for_liste, read_soup_result
 
 
 def get_listes_url(user_name, page_no=1):
-    url = get_base_url(user_name=user_name) + 'listes/all/all/likes/page-' + str(page_no)
+    url = (
+        get_base_url(user_name=user_name) + 'listes/all/all/likes/page-' + str(page_no)
+    )
     return url
 
 
 def parse_listes_page(user_name='wok', page_no=1, verbose=False):
     url = get_listes_url(user_name=user_name, page_no=page_no)
     print(url)
     soup = BeautifulSoup(requests.get(url).content, 'lxml')
 
     collection_items = soup.find_all('li', {'class': 'elth-thumbnail by3'})
 
-    listes_data = dict()
+    listes_data = {}
     for item in collection_items:
         category = item.find_all('span', {'class': 'elth-universe-label'})
         overview = item.find_all('a', {'class': 'elth-thumbnail-title'})
 
         link = overview[0].attrs['href']
 
         item_id = int(link.rsplit('/')[-1])
 
-        listes_data[item_id] = dict()
+        listes_data[item_id] = {}
         listes_data[item_id]['category'] = read_soup_result(category)
         listes_data[item_id]['name'] = read_soup_result(overview)
         listes_data[item_id]['link'] = link
 
-        print('List n°{}: {}'.format(
-            item_id,
-            listes_data[item_id]['name'],
-        ))
-
-        full_review_url = get_url_for_liste(item_id_for_liste=item_id,
-                                            page_no_within_list=None)
+        print(
+            'List n°{}: {}'.format(
+                item_id,
+                listes_data[item_id]['name'],
+            ),
+        )
+
+        full_review_url = get_url_for_liste(
+            item_id_for_liste=item_id,
+            page_no_within_list=None,
+        )
         num_pages = get_num_pages(full_review_url)
 
-        listes_data[item_id]['elements'] = dict()
+        listes_data[item_id]['elements'] = {}
 
         for page_no_within_list in range(1, num_pages + 1):
-
             if verbose:
-                print('Page n°{}/{}:'.format(
-                    page_no_within_list,
-                    num_pages,
-                ))
-
-            current_url = get_url_for_liste(item_id_for_liste=item_id,
-                                            page_no_within_list=page_no_within_list)
+                print(
+                    'Page n°{}/{}:'.format(
+                        page_no_within_list,
+                        num_pages,
+                    ),
+                )
+
+            current_url = get_url_for_liste(
+                item_id_for_liste=item_id,
+                page_no_within_list=page_no_within_list,
+            )
             full_soup = BeautifulSoup(requests.get(current_url).content, 'lxml')
 
             description = full_soup.find_all('div', {'data-rel': 'list-description'})
             listes_data[item_id]['description'] = read_soup_result(description)
 
             review_items = full_soup.find_all('div', {'class': 'elli-content'})
 
             for review_item in review_items:
                 soup_content = review_item.find_all('a', {'class': 'elco-anchor'})
-                soup_comment = review_item.find_all('div', {'class': 'elli-annotation-content'})
+                soup_comment = review_item.find_all(
+                    'div',
+                    {'class': 'elli-annotation-content'},
+                )
 
                 element = get_item_id(soup_content)
                 name = read_soup_result(soup_content)
                 comment = read_soup_result(soup_comment, simplify_text=False)
 
                 if verbose:
-                    print('-   item n°{}: {}'.format(
-                        element,
-                        name,
-                    ))
+                    print(
+                        '-   item n°{}: {}'.format(
+                            element,
+                            name,
+                        ),
+                    )
 
-                listes_data[item_id]['elements'][element] = dict()
+                listes_data[item_id]['elements'][element] = {}
                 listes_data[item_id]['elements'][element]['name'] = name
                 listes_data[item_id]['elements'][element]['comment'] = comment
 
     return listes_data
```

### Comparing `senscritique-0.5.2/senscritique/takeout.py` & `senscritique-0.5.4/senscritique/takeout.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,47 +1,51 @@
 import json
 import pathlib
+from pathlib import Path
 
-from .data_utils import get_save_filename
-from .process_generic import parse_keyword
-from .utils import get_data_folder
+from senscritique.data_utils import get_save_filename
+from senscritique.process_generic import parse_keyword
+from senscritique.utils import get_data_folder
 
 
 def print_data(data, file_name=None):
     if file_name is None:
         print(data)
     else:
         # Reference of the following line: https://stackoverflow.com/a/14364249
         pathlib.Path(get_data_folder()).mkdir(parents=True, exist_ok=True)
 
-        with open(file_name, 'w', encoding='utf8') as f:
+        with Path(file_name).open('w', encoding='utf8') as f:
             f.write(json.dumps(data))
 
     return
 
 
 def parse(user_name='wok', data_type='collection', verbose=False):
     if data_type == 'collection':
         data = parse_keyword(user_name=user_name, keyword='collection', verbose=verbose)
     elif data_type == 'critiques':
         data = parse_keyword(user_name=user_name, keyword='critiques', verbose=verbose)
     elif data_type == 'listes':
         data = parse_keyword(user_name=user_name, keyword='listes', verbose=verbose)
     else:
-        data = dict()
+        data = {}
 
     return data
 
 
 def parse_and_cache(user_name='wok', data_type='collection', verbose=False):
-    save_file_name = get_data_folder() + get_save_filename(user_name=user_name, data_type=data_type)
+    save_file_name = get_data_folder() + get_save_filename(
+        user_name=user_name,
+        data_type=data_type,
+    )
 
     if pathlib.Path(save_file_name).is_file():
         print('File ' + save_file_name + ' already exists.')
-        with open(save_file_name, 'r', encoding='utf8') as f:
+        with Path(save_file_name).open(encoding='utf8') as f:
             data = json.load(f)
     else:
         data = parse(user_name=user_name, data_type=data_type, verbose=verbose)
         if len(data) > 0:
             print_data(data, save_file_name)
 
     sentence = '[' + data_type + ' by ' + user_name + '] num_items = {}'
```

### Comparing `senscritique-0.5.2/senscritique/tests/test_senscritique.py` & `senscritique-0.5.4/senscritique/tests/test_senscritique.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,53 @@
 import unittest
 
 import senscritique
 
 
 class TestSensCritiqueMethods(unittest.TestCase):
-
     @classmethod
     def test_get_user_example(cls):
-        example_user_name = 'عمرالعرفاوي'
+        example_user_name = 'Pipo'
 
         return example_user_name
 
     def test_parse_with_wrong_arguments(self):
         data = senscritique.parse(user_name='wok', data_type='wrong_argument')
 
         self.assertEqual(len(data), 0)
 
     def test_parse_and_cache(self):
         # Download
-        downloaded_data = senscritique.parse_and_cache(user_name=self.test_get_user_example(), data_type='collection')
+        downloaded_data = senscritique.parse_and_cache(
+            user_name=self.test_get_user_example(),
+            data_type='collection',
+        )
         # Load from cache
-        loaded_data = senscritique.parse_and_cache(user_name=self.test_get_user_example(), data_type='collection')
+        loaded_data = senscritique.parse_and_cache(
+            user_name=self.test_get_user_example(),
+            data_type='collection',
+        )
 
         self.assertDictEqual(downloaded_data, loaded_data)
 
     def test_parse_collection(self):
-        data = senscritique.parse(user_name=self.test_get_user_example(), data_type='collection', verbose=True)
+        data = senscritique.parse(
+            user_name=self.test_get_user_example(),
+            data_type='collection',
+            verbose=True,
+        )
         senscritique.print_data(data)
-        self.assertEqual(len(data), 1)
+        self.assertEqual(len(data), 6)
 
     def test_parse_critiques(self):
-        data = senscritique.parse(user_name='MrMez', data_type='critiques', verbose=True)
+        data = senscritique.parse(
+            user_name='MrMez',
+            data_type='critiques',
+            verbose=True,
+        )
         senscritique.print_data(data)
         self.assertEqual(len(data), 2)
 
     def test_parse_listes(self):
         data = senscritique.parse(user_name='Pop-Dan', data_type='listes', verbose=True)
         senscritique.print_data(data)
         self.assertEqual(len(data), 33)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `senscritique-0.5.2/senscritique/utils.py` & `senscritique-0.5.4/senscritique/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,23 @@
 def get_data_folder():
     return 'data/'
 
 
 def get_base_url(user_name=None):
-    url = 'https://www.senscritique.com/'
+    url = 'https://old.senscritique.com/'
     if user_name is not None:
         url += user_name + '/'
     return url
 
 
-def get_url_for_liste(item_id_for_liste,
-                      page_no_within_list=None):
-    url = get_base_url() + 'sc2/liste/{}/'.format(
-        item_id_for_liste
-    )
+def get_url_for_liste(item_id_for_liste, page_no_within_list=None):
+    url = get_base_url() + f'sc2/liste/{item_id_for_liste}/'
 
     if page_no_within_list is not None:
-        url += 'page-{}.ajax'.format(
-            page_no_within_list
-        )
+        url += f'page-{page_no_within_list}.ajax'
 
     return url
 
 
 def improve_readability(text):
     return text.replace('\n', '').replace('\t', '')
```

### Comparing `senscritique-0.5.2/senscritique.egg-info/SOURCES.txt` & `senscritique-0.5.4/senscritique.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 setup.cfg
 setup.py
 senscritique/__init__.py
 senscritique/data_utils.py
 senscritique/parse_utils.py
 senscritique/process_collection.py
```

### Comparing `senscritique-0.5.2/setup.py` & `senscritique-0.5.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='senscritique',
-    version='0.5.2',
+    version='0.5.4',
     author='Wok',
     author_email='wok@tuta.io',
     description='SensCritique Takeout on PyPI',
     keywords=['senscritique', 'takeout', 'takeaway'],
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/woctezuma/SensCritique-Takeout',
-    download_url='https://github.com/woctezuma/SensCritique-Takeout/archive/0.5.2.tar.gz',
+    download_url='https://github.com/woctezuma/SensCritique-Takeout/archive/0.5.4.tar.gz',
     packages=setuptools.find_packages(),
     install_requires=[
         'beautifulsoup4',
         'requests',
         'lxml',
     ],
     test_suite='nose.collector',
```

