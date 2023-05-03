# Comparing `tmp/pomice-2.5.0.tar.gz` & `tmp/pomice-2.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pomice-2.5.0.tar", last modified: Tue May  2 01:06:04 2023, max compression
+gzip compressed data, was "pomice-2.5.1.tar", last modified: Wed May  3 23:49:48 2023, max compression
```

## Comparing `pomice-2.5.0.tar` & `pomice-2.5.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-05-02 01:06:04.770781 pomice-2.5.0/
--rw-rw-rw-   0        0        0    35823 2021-09-25 18:02:32.000000 pomice-2.5.0/LICENSE
--rw-rw-rw-   0        0        0     5445 2023-05-02 01:06:04.768782 pomice-2.5.0/PKG-INFO
--rw-rw-rw-   0        0        0     4680 2023-04-23 18:14:31.000000 pomice-2.5.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-02 01:06:04.673258 pomice-2.5.0/pomice/
--rw-rw-rw-   0        0        0      853 2023-05-02 01:03:25.000000 pomice-2.5.0/pomice/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-02 01:06:04.738954 pomice-2.5.0/pomice/applemusic/
--rw-rw-rw-   0        0        0      146 2023-04-29 18:05:44.000000 pomice-2.5.0/pomice/applemusic/__init__.py
--rw-rw-rw-   0        0        0     6682 2023-05-02 00:58:27.000000 pomice-2.5.0/pomice/applemusic/client.py
--rw-rw-rw-   0        0        0      321 2023-03-11 15:22:18.000000 pomice-2.5.0/pomice/applemusic/exceptions.py
--rw-rw-rw-   0        0        0     3573 2023-03-11 15:28:02.000000 pomice-2.5.0/pomice/applemusic/objects.py
--rw-rw-rw-   0        0        0     8145 2023-03-27 02:36:38.000000 pomice-2.5.0/pomice/enums.py
--rw-rw-rw-   0        0        0     6038 2023-03-13 23:36:22.000000 pomice-2.5.0/pomice/events.py
--rw-rw-rw-   0        0        0     2746 2023-03-12 15:44:18.000000 pomice-2.5.0/pomice/exceptions.py
--rw-rw-rw-   0        0        0    14832 2023-03-11 15:25:46.000000 pomice-2.5.0/pomice/filters.py
--rw-rw-rw-   0        0        0     5302 2023-04-23 18:14:31.000000 pomice-2.5.0/pomice/objects.py
--rw-rw-rw-   0        0        0    23884 2023-05-01 11:42:50.000000 pomice-2.5.0/pomice/player.py
--rw-rw-rw-   0        0        0    35277 2023-05-02 01:01:04.000000 pomice-2.5.0/pomice/pool.py
--rw-rw-rw-   0        0        0        0 2023-03-10 02:46:40.000000 pomice-2.5.0/pomice/py.typed
--rw-rw-rw-   0        0        0    12184 2023-03-27 02:26:04.000000 pomice-2.5.0/pomice/queue.py
--rw-rw-rw-   0        0        0     1069 2023-03-11 15:22:18.000000 pomice-2.5.0/pomice/routeplanner.py
-drwxrwxrwx   0        0        0        0 2023-05-02 01:06:04.765737 pomice-2.5.0/pomice/spotify/
--rw-rw-rw-   0        0        0      147 2023-03-11 15:22:18.000000 pomice-2.5.0/pomice/spotify/__init__.py
--rw-rw-rw-   0        0        0     6235 2023-05-02 01:01:06.000000 pomice-2.5.0/pomice/spotify/client.py
--rw-rw-rw-   0        0        0      301 2023-03-11 15:22:18.000000 pomice-2.5.0/pomice/spotify/exceptions.py
--rw-rw-rw-   0        0        0     3445 2023-04-23 18:14:31.000000 pomice-2.5.0/pomice/spotify/objects.py
--rw-rw-rw-   0        0        0     8697 2023-03-13 02:58:40.000000 pomice-2.5.0/pomice/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-02 01:06:04.721193 pomice-2.5.0/pomice.egg-info/
--rw-rw-rw-   0        0        0     5445 2023-05-02 01:06:04.000000 pomice-2.5.0/pomice.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      628 2023-05-02 01:06:04.000000 pomice-2.5.0/pomice.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-02 01:06:04.000000 pomice-2.5.0/pomice.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-05-02 01:06:04.000000 pomice-2.5.0/pomice.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-02 01:06:04.000000 pomice-2.5.0/pomice.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      369 2023-03-13 23:16:18.000000 pomice-2.5.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-02 01:06:04.771781 pomice-2.5.0/setup.cfg
--rw-rw-rw-   0        0        0     2171 2023-04-29 18:06:01.000000 pomice-2.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-03 23:49:48.056567 pomice-2.5.1/
+-rw-rw-rw-   0        0        0    35823 2021-09-25 18:02:32.000000 pomice-2.5.1/LICENSE
+-rw-rw-rw-   0        0        0     5445 2023-05-03 23:49:48.054563 pomice-2.5.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4680 2023-04-23 18:14:31.000000 pomice-2.5.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-03 23:49:47.985417 pomice-2.5.1/pomice/
+-rw-rw-rw-   0        0        0      853 2023-05-03 23:48:41.000000 pomice-2.5.1/pomice/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-03 23:49:48.042346 pomice-2.5.1/pomice/applemusic/
+-rw-rw-rw-   0        0        0      146 2023-04-29 18:05:44.000000 pomice-2.5.1/pomice/applemusic/__init__.py
+-rw-rw-rw-   0        0        0     6682 2023-05-02 00:58:27.000000 pomice-2.5.1/pomice/applemusic/client.py
+-rw-rw-rw-   0        0        0      321 2023-03-11 15:22:18.000000 pomice-2.5.1/pomice/applemusic/exceptions.py
+-rw-rw-rw-   0        0        0     3573 2023-03-11 15:28:02.000000 pomice-2.5.1/pomice/applemusic/objects.py
+-rw-rw-rw-   0        0        0     8043 2023-05-03 23:47:11.000000 pomice-2.5.1/pomice/enums.py
+-rw-rw-rw-   0        0        0     6038 2023-03-13 23:36:22.000000 pomice-2.5.1/pomice/events.py
+-rw-rw-rw-   0        0        0     2746 2023-03-12 15:44:18.000000 pomice-2.5.1/pomice/exceptions.py
+-rw-rw-rw-   0        0        0    14832 2023-03-11 15:25:46.000000 pomice-2.5.1/pomice/filters.py
+-rw-rw-rw-   0        0        0     5302 2023-04-23 18:14:31.000000 pomice-2.5.1/pomice/objects.py
+-rw-rw-rw-   0        0        0    23884 2023-05-01 11:42:50.000000 pomice-2.5.1/pomice/player.py
+-rw-rw-rw-   0        0        0    35055 2023-05-03 23:47:13.000000 pomice-2.5.1/pomice/pool.py
+-rw-rw-rw-   0        0        0        0 2023-03-10 02:46:40.000000 pomice-2.5.1/pomice/py.typed
+-rw-rw-rw-   0        0        0    12184 2023-03-27 02:26:04.000000 pomice-2.5.1/pomice/queue.py
+-rw-rw-rw-   0        0        0     1069 2023-03-11 15:22:18.000000 pomice-2.5.1/pomice/routeplanner.py
+drwxrwxrwx   0        0        0        0 2023-05-03 23:49:48.052423 pomice-2.5.1/pomice/spotify/
+-rw-rw-rw-   0        0        0      147 2023-03-11 15:22:18.000000 pomice-2.5.1/pomice/spotify/__init__.py
+-rw-rw-rw-   0        0        0     6235 2023-05-02 01:01:06.000000 pomice-2.5.1/pomice/spotify/client.py
+-rw-rw-rw-   0        0        0      301 2023-03-11 15:22:18.000000 pomice-2.5.1/pomice/spotify/exceptions.py
+-rw-rw-rw-   0        0        0     3445 2023-04-23 18:14:31.000000 pomice-2.5.1/pomice/spotify/objects.py
+-rw-rw-rw-   0        0        0     8697 2023-03-13 02:58:40.000000 pomice-2.5.1/pomice/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-03 23:49:48.033822 pomice-2.5.1/pomice.egg-info/
+-rw-rw-rw-   0        0        0     5445 2023-05-03 23:49:47.000000 pomice-2.5.1/pomice.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      628 2023-05-03 23:49:47.000000 pomice-2.5.1/pomice.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-03 23:49:47.000000 pomice-2.5.1/pomice.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-05-03 23:49:47.000000 pomice-2.5.1/pomice.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-03 23:49:47.000000 pomice-2.5.1/pomice.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      369 2023-03-13 23:16:18.000000 pomice-2.5.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-03 23:49:48.056567 pomice-2.5.1/setup.cfg
+-rw-rw-rw-   0        0        0     2171 2023-04-29 18:06:01.000000 pomice-2.5.1/setup.py
```

### Comparing `pomice-2.5.0/LICENSE` & `pomice-2.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pomice-2.5.0/PKG-INFO` & `pomice-2.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pomice
-Version: 2.5.0
+Version: 2.5.1
 Summary: The modern Lavalink wrapper designed for Discord.py
 Home-page: https://github.com/cloudwithax/pomice
 Author: cloudwithax
 License: GPL
 Keywords: pomice,lavalink,discord.py
 Classifier: Framework :: AsyncIO
 Classifier: Operating System :: OS Independent
```

### Comparing `pomice-2.5.0/README.md` & `pomice-2.5.1/README.md`

 * *Files identical despite different names*

### Comparing `pomice-2.5.0/pomice/__init__.py` & `pomice-2.5.1/pomice/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
     raise DiscordPyOutdated(
         "You must have discord.py (v2.0 or greater) to use this library. "
         "Uninstall your current version and install discord.py 2.0 "
         "using 'pip install discord.py'",
     )
 
-__version__ = "2.5.0"
+__version__ = "2.5.1"
 __title__ = "pomice"
 __author__ = "cloudwithax"
 __license__ = "GPL-3.0"
 __copyright__ = "Copyright (c) 2023, cloudwithax"
 
 from .enums import *
 from .events import *
```

### Comparing `pomice-2.5.0/pomice/applemusic/client.py` & `pomice-2.5.1/pomice/applemusic/client.py`

 * *Files identical despite different names*

### Comparing `pomice-2.5.0/pomice/applemusic/objects.py` & `pomice-2.5.1/pomice/applemusic/objects.py`

 * *Files identical despite different names*

### Comparing `pomice-2.5.0/pomice/enums.py` & `pomice-2.5.1/pomice/enums.py`

 * *Files 2% similar despite different names*

```diff
@@ -213,18 +213,14 @@
         r"(\/(?:[\w\-]+\?v=|embed\/|v\/)?)([\w\-]+)(\S+)?$",
     )
 
     YOUTUBE_PLAYLIST_URL = re.compile(
         r"^((?:https?:)?\/\/)?((?:www|m)\.)?((?:youtube\.com|youtu.be))/playlist\?list=.*",
     )
 
-    YOUTUBE_VID_IN_PLAYLIST = re.compile(
-        r"(?P<video>^.*?v.*?)(?P<list>&list.*)",
-    )
-
     YOUTUBE_TIMESTAMP = re.compile(
         r"(?P<video>^.*?)(\?t|&start)=(?P<time>\d+)?.*",
     )
 
     AM_URL = re.compile(
         r"https?://music.apple.com/(?P<country>[a-zA-Z]{2})/"
         r"(?P<type>album|playlist|song|artist)/(?P<name>.+)/(?P<id>[^?]+)",
```

### Comparing `pomice-2.5.0/pomice/events.py` & `pomice-2.5.1/pomice/events.py`

 * *Files identical despite different names*

### Comparing `pomice-2.5.0/pomice/exceptions.py` & `pomice-2.5.1/pomice/exceptions.py`

 * *Files identical despite different names*

### Comparing `pomice-2.5.0/pomice/filters.py` & `pomice-2.5.1/pomice/filters.py`

 * *Files identical despite different names*

### Comparing `pomice-2.5.0/pomice/objects.py` & `pomice-2.5.1/pomice/objects.py`

 * *Files identical despite different names*

### Comparing `pomice-2.5.0/pomice/player.py` & `pomice-2.5.1/pomice/player.py`

 * *Files identical despite different names*

### Comparing `pomice-2.5.0/pomice/pool.py` & `pomice-2.5.1/pomice/pool.py`

 * *Files 1% similar despite different names*

```diff
@@ -155,21 +155,22 @@
             "Authorization": self._password,
             "User-Id": str(self._bot_user.id),
             "Client-Name": f"Pomice/{__version__}",
         }
 
         self._players: Dict[int, Player] = {}
 
+        self._spotify_client: Optional[spotify.Client] = None
+        self._apple_music_client: Optional[applemusic.Client] = None
+
         self._spotify_client_id: Optional[str] = spotify_client_id
         self._spotify_client_secret: Optional[str] = spotify_client_secret
 
-        self._apple_music_client: Optional[applemusic.Client] = None
-
         if self._spotify_client_id and self._spotify_client_secret:
-            self._spotify_client: spotify.Client = spotify.Client(
+            self._spotify_client = spotify.Client(
                 self._spotify_client_id,
                 self._spotify_client_secret,
             )
 
         if apple_music:
             self._apple_music_client = applemusic.Client()
 
@@ -617,15 +618,15 @@
             if not self._spotify_client_id and not self._spotify_client_secret:
                 raise InvalidSpotifyClientAuthorization(
                     "You did not provide proper Spotify client authorization credentials. "
                     "If you would like to use the Spotify searching feature, "
                     "please obtain Spotify API credentials here: https://developer.spotify.com/",
                 )
 
-            spotify_results = await self._spotify_client.search(query=query)
+            spotify_results = await self._spotify_client.search(query=query)  # type: ignore
 
             if isinstance(spotify_results, spotify.Track):
                 return [
                     Track(
                         track_id=spotify_results.id,
                         ctx=ctx,
                         track_type=TrackType.SPOTIFY,
@@ -740,20 +741,14 @@
                 query = f"{search_type}:{query}"
 
             # If YouTube url contains a timestamp, capture it for use later.
 
             if match := URLRegex.YOUTUBE_TIMESTAMP.match(query):
                 timestamp = float(match.group("time"))
 
-            # If query is a video thats part of a playlist, get the video and queue that instead
-            # (I can't tell you how much i've wanted to implement this in here)
-
-            if match := URLRegex.YOUTUBE_VID_IN_PLAYLIST.match(query):
-                query = match.group("video")
-
             data = await self.send(
                 method="GET",
                 path="loadtracks",
                 query=f"identifier={quote(query)}",
             )
 
         load_type = data.get("loadType")
@@ -815,15 +810,15 @@
         Gets recommendations from either YouTube or Spotify.
         The track that is passed in must be either from
         YouTube or Spotify or else this will not work.
         You can pass in a discord.py Context object to get a
         Context object on all tracks that get recommended.
         """
         if track.track_type == TrackType.SPOTIFY:
-            results = await self._spotify_client.get_recommendations(query=track.uri)
+            results = await self._spotify_client.get_recommendations(query=track.uri)  # type: ignore
             tracks = [
                 Track(
                     track_id=track.id,
                     ctx=ctx,
                     track_type=TrackType.SPOTIFY,
                     info={
                         "title": track.name,
```

### Comparing `pomice-2.5.0/pomice/queue.py` & `pomice-2.5.1/pomice/queue.py`

 * *Files identical despite different names*

### Comparing `pomice-2.5.0/pomice/routeplanner.py` & `pomice-2.5.1/pomice/routeplanner.py`

 * *Files identical despite different names*

### Comparing `pomice-2.5.0/pomice/spotify/client.py` & `pomice-2.5.1/pomice/spotify/client.py`

 * *Files identical despite different names*

### Comparing `pomice-2.5.0/pomice/spotify/objects.py` & `pomice-2.5.1/pomice/spotify/objects.py`

 * *Files identical despite different names*

### Comparing `pomice-2.5.0/pomice/utils.py` & `pomice-2.5.1/pomice/utils.py`

 * *Files identical despite different names*

### Comparing `pomice-2.5.0/pomice.egg-info/PKG-INFO` & `pomice-2.5.1/pomice.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pomice
-Version: 2.5.0
+Version: 2.5.1
 Summary: The modern Lavalink wrapper designed for Discord.py
 Home-page: https://github.com/cloudwithax/pomice
 Author: cloudwithax
 License: GPL
 Keywords: pomice,lavalink,discord.py
 Classifier: Framework :: AsyncIO
 Classifier: Operating System :: OS Independent
```

### Comparing `pomice-2.5.0/pomice.egg-info/SOURCES.txt` & `pomice-2.5.1/pomice.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pomice-2.5.0/setup.py` & `pomice-2.5.1/setup.py`

 * *Files identical despite different names*

