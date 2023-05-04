# Comparing `tmp/youtube-webscrape-api-0.0.2.tar.gz` & `tmp/youtube-webscrape-api-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "youtube-webscrape-api-0.0.2.tar", last modified: Wed Mar 22 20:14:20 2023, max compression
+gzip compressed data, was "youtube-webscrape-api-0.0.3.tar", last modified: Thu May  4 13:18:30 2023, max compression
```

## Comparing `youtube-webscrape-api-0.0.2.tar` & `youtube-webscrape-api-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-03-22 20:14:20.721549 youtube-webscrape-api-0.0.2/
--rw-rw-rw-   0        0        0     1094 2023-03-21 08:14:45.000000 youtube-webscrape-api-0.0.2/LICENSE.md
--rw-rw-rw-   0        0        0     6112 2023-03-22 20:14:20.721549 youtube-webscrape-api-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     5374 2023-03-22 20:14:09.000000 youtube-webscrape-api-0.0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-03-22 20:14:20.721549 youtube-webscrape-api-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1240 2023-03-22 20:14:00.000000 youtube-webscrape-api-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-22 20:14:20.674609 youtube-webscrape-api-0.0.2/test/
--rw-rw-rw-   0        0        0      970 2023-03-22 19:35:12.000000 youtube-webscrape-api-0.0.2/test/test_scraper.py
-drwxrwxrwx   0        0        0        0 2023-03-22 20:14:20.690235 youtube-webscrape-api-0.0.2/youtube_webscrape_api.egg-info/
--rw-rw-rw-   0        0        0     6112 2023-03-22 20:14:20.000000 youtube-webscrape-api-0.0.2/youtube_webscrape_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      360 2023-03-22 20:14:20.000000 youtube-webscrape-api-0.0.2/youtube_webscrape_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-22 20:14:20.000000 youtube-webscrape-api-0.0.2/youtube_webscrape_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-03-22 20:14:20.000000 youtube-webscrape-api-0.0.2/youtube_webscrape_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-03-22 20:14:20.000000 youtube-webscrape-api-0.0.2/youtube_webscrape_api.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-03-22 20:14:20.705919 youtube-webscrape-api-0.0.2/yt_scrape/
--rw-rw-rw-   0        0        0       80 2023-03-22 19:35:12.000000 youtube-webscrape-api-0.0.2/yt_scrape/__init__.py
--rw-rw-rw-   0        0        0      178 2023-03-22 19:57:53.000000 youtube-webscrape-api-0.0.2/yt_scrape/exceptions.py
--rw-rw-rw-   0        0        0     7699 2023-03-22 19:36:29.000000 youtube-webscrape-api-0.0.2/yt_scrape/scraper.py
--rw-rw-rw-   0        0        0     1540 2023-03-22 19:35:12.000000 youtube-webscrape-api-0.0.2/yt_scrape/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-04 13:18:30.672636 youtube-webscrape-api-0.0.3/
+-rw-rw-rw-   0        0        0     1094 2023-03-21 08:14:45.000000 youtube-webscrape-api-0.0.3/LICENSE.md
+-rw-rw-rw-   0        0        0     6112 2023-05-04 13:18:30.672636 youtube-webscrape-api-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     5374 2023-03-22 20:14:09.000000 youtube-webscrape-api-0.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-04 13:18:30.672636 youtube-webscrape-api-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1240 2023-05-04 13:18:15.000000 youtube-webscrape-api-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 13:18:30.648637 youtube-webscrape-api-0.0.3/test/
+-rw-rw-rw-   0        0        0      970 2023-03-22 19:35:12.000000 youtube-webscrape-api-0.0.3/test/test_scraper.py
+drwxrwxrwx   0        0        0        0 2023-05-04 13:18:30.672636 youtube-webscrape-api-0.0.3/youtube_webscrape_api.egg-info/
+-rw-rw-rw-   0        0        0     6112 2023-05-04 13:18:30.000000 youtube-webscrape-api-0.0.3/youtube_webscrape_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      360 2023-05-04 13:18:30.000000 youtube-webscrape-api-0.0.3/youtube_webscrape_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 13:18:30.000000 youtube-webscrape-api-0.0.3/youtube_webscrape_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-05-04 13:18:30.000000 youtube-webscrape-api-0.0.3/youtube_webscrape_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-04 13:18:30.000000 youtube-webscrape-api-0.0.3/youtube_webscrape_api.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-04 13:18:30.672636 youtube-webscrape-api-0.0.3/yt_scrape/
+-rw-rw-rw-   0        0        0       80 2023-03-22 19:35:12.000000 youtube-webscrape-api-0.0.3/yt_scrape/__init__.py
+-rw-rw-rw-   0        0        0      178 2023-03-22 19:57:53.000000 youtube-webscrape-api-0.0.3/yt_scrape/exceptions.py
+-rw-rw-rw-   0        0        0     7813 2023-05-04 12:37:18.000000 youtube-webscrape-api-0.0.3/yt_scrape/scraper.py
+-rw-rw-rw-   0        0        0     1540 2023-05-04 12:21:31.000000 youtube-webscrape-api-0.0.3/yt_scrape/utils.py
```

### Comparing `youtube-webscrape-api-0.0.2/LICENSE.md` & `youtube-webscrape-api-0.0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `youtube-webscrape-api-0.0.2/PKG-INFO` & `youtube-webscrape-api-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: youtube-webscrape-api
-Version: 0.0.2
+Version: 0.0.3
 Summary: Webscrape based youtube api, free of cost
 Home-page: https://github.com/huzai786/Youtube-Scraper
 Author: Muhammad Huzaifa
 Author-email: muhammadhuzaifagamer123@gmail.com
 License: MIT
 Keywords: youtube-api,youtube-scraper,Youtube-scrape
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `youtube-webscrape-api-0.0.2/README.md` & `youtube-webscrape-api-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `youtube-webscrape-api-0.0.2/setup.py` & `youtube-webscrape-api-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     "beautifulsoup4",
     "requests",
     "fake_useragent"
 ]
 
 setup(
     name="youtube-webscrape-api",
-    version="0.0.2",
+    version="0.0.3",
     author="Muhammad Huzaifa",
     author_email="muhammadhuzaifagamer123@gmail.com",
     url="https://github.com/huzai786/Youtube-Scraper",
     description="Webscrape based youtube api, free of cost",
     license="MIT",
     packages=find_packages(exclude=['test']),
     long_description=long_description,
```

### Comparing `youtube-webscrape-api-0.0.2/test/test_scraper.py` & `youtube-webscrape-api-0.0.3/test/test_scraper.py`

 * *Files identical despite different names*

### Comparing `youtube-webscrape-api-0.0.2/youtube_webscrape_api.egg-info/PKG-INFO` & `youtube-webscrape-api-0.0.3/youtube_webscrape_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: youtube-webscrape-api
-Version: 0.0.2
+Version: 0.0.3
 Summary: Webscrape based youtube api, free of cost
 Home-page: https://github.com/huzai786/Youtube-Scraper
 Author: Muhammad Huzaifa
 Author-email: muhammadhuzaifagamer123@gmail.com
 License: MIT
 Keywords: youtube-api,youtube-scraper,Youtube-scrape
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `youtube-webscrape-api-0.0.2/yt_scrape/scraper.py` & `youtube-webscrape-api-0.0.3/yt_scrape/scraper.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-import re
-import traceback
+import datetime
 
 from yt_scrape.exceptions import TooManyRequests, NoVideoFound
 
 from yt_scrape.utils import get_content, data_dict
 
 
 def youtube_results(keyword):
@@ -88,29 +87,43 @@
                                                 "publish_time": publish_time, "view_count": view_count}
                                     if any(data.values()):
                                         videos.append(data)
 
                     else:
                         continue
 
-    except TypeError as e:
-        tb = traceback.format_exc()
-        line = re.findall(r"(line \d+)", tb)
-        print(f"Error: {e} at {line[0]}")
-
-    except KeyError as e:
-        tb = traceback.format_exc()
-        line = re.findall(r"(line \d+)", tb)
-        print(f"Error: {e} at {line[0]}")
+    except TypeError:
+        pass
+
+    except KeyError:
+        pass
 
     if videos:
         return videos
     else:
         raise NoVideoFound("videos not found!")
 
+
+def extract_number(string):
+    num_str = ''
+    for char in string:
+        if char.isdigit() or char == '.':
+            num_str += char
+    number = float(num_str) if '.' in num_str else int(num_str)
+    if 'K' in string:
+        number *= 1000
+    elif 'M' in string:
+        number *= 1_000_000
+
+    return int(number)
+
+def extract_date(string: str):
+    s = string.replace("Joined", "").strip()
+    return datetime.datetime.strptime(s, "%b %d, %Y").date()
+
 def channels_about(channel_id):
     url = f"https://www.youtube.com/{channel_id}/about"
     html = get_content(url)
     obj = data_dict(html)
     if not obj:
         raise TooManyRequests("Please wait 1 or 2 seconds")
 
@@ -136,44 +149,40 @@
         banner = upper_section_data["banner"]["thumbnails"][0]["url"]
         details["banner"] = banner
 
         channel_id = upper_section_data["channelId"]
         details["channel_id"] = channel_id
 
         subscribers = upper_section_data["subscriberCountText"]["simpleText"]
-        details["subscribers"] = subscribers
+        details["subscribers"] = extract_number(subscribers)
 
         videos_count = upper_section_data["videosCountText"]["runs"][0]["text"]
-        details["videos_count"] = videos_count
+        details["videos_count"] = extract_number(videos_count)
 
-    except (KeyError, ValueError) as e:
-        tb = traceback.format_exc()
-        line = re.findall(r"(line \d+)", tb)
-        print(f"{e} at {line[0]}")
+    except (KeyError, ValueError):
         pass
 
     try:
         tabs = obj.get("contents").get("twoColumnBrowseResultsRenderer").get("tabs")
         if tabs:
             for tab in tabs:
                 if tab.get("tabRenderer") and tab.get("tabRenderer").get("content"):
                     content = tab.get("tabRenderer").get("content").get("sectionListRenderer").get("contents")[0]["itemSectionRenderer"]["contents"][0]
 
                     joined_data_list = content["channelAboutFullMetadataRenderer"]["joinedDateText"]["runs"]
                     joined = " ".join([i["text"] for i in joined_data_list]) if isinstance(joined_data_list, list) else None
+                    if joined:
+                        joined = extract_date(joined)
                     details["joined"] = joined
 
                     views_count = content["channelAboutFullMetadataRenderer"]["viewCountText"]["simpleText"]
-                    details["views_count"] = views_count
+                    details["views_count"] = extract_number(views_count)
                     country = content["channelAboutFullMetadataRenderer"]["country"]["simpleText"]
                     details["country"] = country
 
-    except (KeyError, ValueError) as e:
-        tb = traceback.format_exc()
-        line = re.findall(r"(line \d+)", tb)
-        print(f"{e} at {line[0]}")
+    except (KeyError, ValueError):
         pass
 
     if any(details.values()):
         return details
     else:
         return {}
```

### Comparing `youtube-webscrape-api-0.0.2/yt_scrape/utils.py` & `youtube-webscrape-api-0.0.3/yt_scrape/utils.py`

 * *Files identical despite different names*

