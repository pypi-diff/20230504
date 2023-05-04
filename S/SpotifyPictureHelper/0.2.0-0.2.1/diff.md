# Comparing `tmp/SpotifyPictureHelper-0.2.0.tar.gz` & `tmp/SpotifyPictureHelper-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SpotifyPictureHelper-0.2.0.tar", last modified: Wed May  3 04:04:44 2023, max compression
+gzip compressed data, was "SpotifyPictureHelper-0.2.1.tar", last modified: Thu May  4 17:15:55 2023, max compression
```

## Comparing `SpotifyPictureHelper-0.2.0.tar` & `SpotifyPictureHelper-0.2.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 daisyye    (501) staff       (20)        0 2023-05-03 04:04:44.377290 SpotifyPictureHelper-0.2.0/
--rw-r--r--   0 daisyye    (501) staff       (20)      588 2023-05-02 21:22:44.000000 SpotifyPictureHelper-0.2.0/CONTRIBUTING.md
--rw-r--r--   0 daisyye    (501) staff       (20)    11357 2023-05-02 21:22:44.000000 SpotifyPictureHelper-0.2.0/LICENSE
--rw-r--r--   0 daisyye    (501) staff       (20)      380 2023-05-02 21:22:44.000000 SpotifyPictureHelper-0.2.0/MANIFEST.in
--rw-r--r--   0 daisyye    (501) staff       (20)     1136 2023-05-02 21:22:44.000000 SpotifyPictureHelper-0.2.0/Makefile
--rw-r--r--   0 daisyye    (501) staff       (20)      336 2023-05-03 04:04:44.377493 SpotifyPictureHelper-0.2.0/PKG-INFO
--rw-r--r--   0 daisyye    (501) staff       (20)     4718 2023-05-03 03:54:37.000000 SpotifyPictureHelper-0.2.0/README.md
-drwxr-xr-x   0 daisyye    (501) staff       (20)        0 2023-05-03 04:04:44.358539 SpotifyPictureHelper-0.2.0/SpotifyPictureHelper/
--rw-r--r--   0 daisyye    (501) staff       (20)        0 2023-05-02 21:22:44.000000 SpotifyPictureHelper-0.2.0/SpotifyPictureHelper/__init__.py
--rw-r--r--   0 daisyye    (501) staff       (20)       22 2023-05-02 21:22:44.000000 SpotifyPictureHelper-0.2.0/SpotifyPictureHelper/_version.py
--rw-r--r--   0 daisyye    (501) staff       (20)    10051 2023-05-03 03:54:37.000000 SpotifyPictureHelper-0.2.0/SpotifyPictureHelper/main.py
-drwxr-xr-x   0 daisyye    (501) staff       (20)        0 2023-05-03 04:04:44.376468 SpotifyPictureHelper-0.2.0/SpotifyPictureHelper/tests/
--rw-r--r--   0 daisyye    (501) staff       (20)    17435 2023-05-03 03:54:37.000000 SpotifyPictureHelper-0.2.0/SpotifyPictureHelper/tests/blackWhite.png
--rw-r--r--   0 daisyye    (501) staff       (20)   269272 2023-05-02 21:22:44.000000 SpotifyPictureHelper-0.2.0/SpotifyPictureHelper/tests/fakeArtist.html
--rw-r--r--   0 daisyye    (501) staff       (20)   307980 2023-05-02 21:22:44.000000 SpotifyPictureHelper-0.2.0/SpotifyPictureHelper/tests/fakePlaylist.html
--rw-r--r--   0 daisyye    (501) staff       (20)    59842 2023-05-02 21:22:44.000000 SpotifyPictureHelper-0.2.0/SpotifyPictureHelper/tests/fakeUser.html
--rw-r--r--   0 daisyye    (501) staff       (20)     1541 2023-05-03 03:54:37.000000 SpotifyPictureHelper-0.2.0/SpotifyPictureHelper/tests/overlay.png
--rw-r--r--   0 daisyye    (501) staff       (20)    14988 2023-05-03 03:54:37.000000 SpotifyPictureHelper-0.2.0/SpotifyPictureHelper/tests/test2.png
--rw-r--r--   0 daisyye    (501) staff       (20)     7458 2023-05-03 03:54:37.000000 SpotifyPictureHelper-0.2.0/SpotifyPictureHelper/tests/test_all.py
-drwxr-xr-x   0 daisyye    (501) staff       (20)        0 2023-05-03 04:04:44.362295 SpotifyPictureHelper-0.2.0/SpotifyPictureHelper.egg-info/
--rw-r--r--   0 daisyye    (501) staff       (20)      336 2023-05-03 04:04:44.000000 SpotifyPictureHelper-0.2.0/SpotifyPictureHelper.egg-info/PKG-INFO
--rw-r--r--   0 daisyye    (501) staff       (20)      778 2023-05-03 04:04:44.000000 SpotifyPictureHelper-0.2.0/SpotifyPictureHelper.egg-info/SOURCES.txt
--rw-r--r--   0 daisyye    (501) staff       (20)        1 2023-05-03 04:04:44.000000 SpotifyPictureHelper-0.2.0/SpotifyPictureHelper.egg-info/dependency_links.txt
--rw-r--r--   0 daisyye    (501) staff       (20)       64 2023-05-03 04:04:44.000000 SpotifyPictureHelper-0.2.0/SpotifyPictureHelper.egg-info/entry_points.txt
--rw-r--r--   0 daisyye    (501) staff       (20)        1 2023-05-03 04:04:44.000000 SpotifyPictureHelper-0.2.0/SpotifyPictureHelper.egg-info/not-zip-safe
--rw-r--r--   0 daisyye    (501) staff       (20)      119 2023-05-03 04:04:44.000000 SpotifyPictureHelper-0.2.0/SpotifyPictureHelper.egg-info/requires.txt
--rw-r--r--   0 daisyye    (501) staff       (20)       21 2023-05-03 04:04:44.000000 SpotifyPictureHelper-0.2.0/SpotifyPictureHelper.egg-info/top_level.txt
--rw-r--r--   0 daisyye    (501) staff       (20)     1431 2023-05-03 03:54:37.000000 SpotifyPictureHelper-0.2.0/pyproject.toml
--rw-r--r--   0 daisyye    (501) staff       (20)      721 2023-05-03 04:04:44.378330 SpotifyPictureHelper-0.2.0/setup.cfg
--rw-r--r--   0 daisyye    (501) staff       (20)       38 2023-05-02 21:22:44.000000 SpotifyPictureHelper-0.2.0/setup.py
+drwxr-xr-x   0 daisyye    (501) staff       (20)        0 2023-05-04 17:15:55.633168 SpotifyPictureHelper-0.2.1/
+-rw-r--r--   0 daisyye    (501) staff       (20)      588 2023-05-02 21:22:44.000000 SpotifyPictureHelper-0.2.1/CONTRIBUTING.md
+-rw-r--r--   0 daisyye    (501) staff       (20)    11357 2023-05-02 21:22:44.000000 SpotifyPictureHelper-0.2.1/LICENSE
+-rw-r--r--   0 daisyye    (501) staff       (20)      380 2023-05-02 21:22:44.000000 SpotifyPictureHelper-0.2.1/MANIFEST.in
+-rw-r--r--   0 daisyye    (501) staff       (20)     1136 2023-05-02 21:22:44.000000 SpotifyPictureHelper-0.2.1/Makefile
+-rw-r--r--   0 daisyye    (501) staff       (20)      336 2023-05-04 17:15:55.633457 SpotifyPictureHelper-0.2.1/PKG-INFO
+-rw-r--r--   0 daisyye    (501) staff       (20)     4697 2023-05-04 16:58:59.000000 SpotifyPictureHelper-0.2.1/README.md
+drwxr-xr-x   0 daisyye    (501) staff       (20)        0 2023-05-04 17:15:55.619990 SpotifyPictureHelper-0.2.1/SpotifyPictureHelper/
+-rw-r--r--   0 daisyye    (501) staff       (20)        0 2023-05-02 21:22:44.000000 SpotifyPictureHelper-0.2.1/SpotifyPictureHelper/__init__.py
+-rw-r--r--   0 daisyye    (501) staff       (20)       22 2023-05-02 21:22:44.000000 SpotifyPictureHelper-0.2.1/SpotifyPictureHelper/_version.py
+-rw-r--r--   0 daisyye    (501) staff       (20)    10796 2023-05-04 17:00:15.000000 SpotifyPictureHelper-0.2.1/SpotifyPictureHelper/main.py
+drwxr-xr-x   0 daisyye    (501) staff       (20)        0 2023-05-04 17:15:55.632431 SpotifyPictureHelper-0.2.1/SpotifyPictureHelper/tests/
+-rw-r--r--   0 daisyye    (501) staff       (20)    17435 2023-05-03 03:54:37.000000 SpotifyPictureHelper-0.2.1/SpotifyPictureHelper/tests/blackWhite.png
+-rw-r--r--   0 daisyye    (501) staff       (20)   269272 2023-05-02 21:22:44.000000 SpotifyPictureHelper-0.2.1/SpotifyPictureHelper/tests/fakeArtist.html
+-rw-r--r--   0 daisyye    (501) staff       (20)   307980 2023-05-02 21:22:44.000000 SpotifyPictureHelper-0.2.1/SpotifyPictureHelper/tests/fakePlaylist.html
+-rw-r--r--   0 daisyye    (501) staff       (20)    59842 2023-05-02 21:22:44.000000 SpotifyPictureHelper-0.2.1/SpotifyPictureHelper/tests/fakeUser.html
+-rw-r--r--   0 daisyye    (501) staff       (20)     1541 2023-05-03 03:54:37.000000 SpotifyPictureHelper-0.2.1/SpotifyPictureHelper/tests/overlay.png
+-rw-r--r--   0 daisyye    (501) staff       (20)    14988 2023-05-03 03:54:37.000000 SpotifyPictureHelper-0.2.1/SpotifyPictureHelper/tests/test2.png
+-rw-r--r--   0 daisyye    (501) staff       (20)    10681 2023-05-04 16:58:59.000000 SpotifyPictureHelper-0.2.1/SpotifyPictureHelper/tests/test_all.py
+drwxr-xr-x   0 daisyye    (501) staff       (20)        0 2023-05-04 17:15:55.622994 SpotifyPictureHelper-0.2.1/SpotifyPictureHelper.egg-info/
+-rw-r--r--   0 daisyye    (501) staff       (20)      336 2023-05-04 17:15:55.000000 SpotifyPictureHelper-0.2.1/SpotifyPictureHelper.egg-info/PKG-INFO
+-rw-r--r--   0 daisyye    (501) staff       (20)      778 2023-05-04 17:15:55.000000 SpotifyPictureHelper-0.2.1/SpotifyPictureHelper.egg-info/SOURCES.txt
+-rw-r--r--   0 daisyye    (501) staff       (20)        1 2023-05-04 17:15:55.000000 SpotifyPictureHelper-0.2.1/SpotifyPictureHelper.egg-info/dependency_links.txt
+-rw-r--r--   0 daisyye    (501) staff       (20)       64 2023-05-04 17:15:55.000000 SpotifyPictureHelper-0.2.1/SpotifyPictureHelper.egg-info/entry_points.txt
+-rw-r--r--   0 daisyye    (501) staff       (20)        1 2023-05-03 04:04:44.000000 SpotifyPictureHelper-0.2.1/SpotifyPictureHelper.egg-info/not-zip-safe
+-rw-r--r--   0 daisyye    (501) staff       (20)      119 2023-05-04 17:15:55.000000 SpotifyPictureHelper-0.2.1/SpotifyPictureHelper.egg-info/requires.txt
+-rw-r--r--   0 daisyye    (501) staff       (20)       21 2023-05-04 17:15:55.000000 SpotifyPictureHelper-0.2.1/SpotifyPictureHelper.egg-info/top_level.txt
+-rw-r--r--   0 daisyye    (501) staff       (20)     1431 2023-05-04 17:03:48.000000 SpotifyPictureHelper-0.2.1/pyproject.toml
+-rw-r--r--   0 daisyye    (501) staff       (20)      721 2023-05-04 17:15:55.634202 SpotifyPictureHelper-0.2.1/setup.cfg
+-rw-r--r--   0 daisyye    (501) staff       (20)       38 2023-05-02 21:22:44.000000 SpotifyPictureHelper-0.2.1/setup.py
```

### Comparing `SpotifyPictureHelper-0.2.0/CONTRIBUTING.md` & `SpotifyPictureHelper-0.2.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `SpotifyPictureHelper-0.2.0/LICENSE` & `SpotifyPictureHelper-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `SpotifyPictureHelper-0.2.0/Makefile` & `SpotifyPictureHelper-0.2.1/Makefile`

 * *Files identical despite different names*

### Comparing `SpotifyPictureHelper-0.2.0/README.md` & `SpotifyPictureHelper-0.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SpotifyPictureHelper [![PyPI](https://img.shields.io/pypi/v/pyobjectify?style=flat-square&color=222222)](https://pypi.org/project/SpotifyPictureHelper)[![docs](https://img.shields.io/badge/-docs-black?style=flat-square)](https://daisyye0730.github.io/SpotifyPictureHelper/docs/_build/html/index.html) 
+# SpotifyPictureHelper [![PyPI](https://img.shields.io/pypi/v/SpotifyPictureHelper)](https://pypi.org/project/SpotifyPictureHelper)[![docs](https://img.shields.io/badge/-docs-black?style=flat-square)](https://daisyye0730.github.io/SpotifyPictureHelper/docs/_build/html/index.html) 
 This is a library of helper functions that allows users to process images in Spotify. 
 
 ![Hex.pm](https://img.shields.io/hexpm/l/apa?style=plastic)
 ![Hex.pm](https://img.shields.io/github/issues/daisyye0730/spotify_find_beats)
 [![Package Status](https://img.shields.io/github/actions/workflow/status/daisyye0730/spotify_find_beats/build.yml)](https://github.com/daisyye0730/spotify_find_beats/)
 [![codecov](https://codecov.io/gh/daisyye0730/SpotifyPictureHelper/branch/main/graph/badge.svg)](https://codecov.io/gh/daisyye0730/SpotifyPictureHelper)
 [![PyPI](https://img.shields.io/pypi/v/SpotifyPictureHelper)](https://pypi.org/project/SpotifyPictureHelper/)
@@ -56,8 +56,8 @@
 4. get_individual_album_covers_from_mosaic('https://mosaic.scdn.co/300/ab67616d00001e022a6ab83ec179747bc3b190dcab67616d00001e02335534788cbc39cfd23ee993ab67616d00001e02d6df3bccf3ec41ea2f76debcab67616d00001e02f0855ff71aa79ab842164fc6') will return the four individual images from this mosaic image 
 5. get_playlist_profile_pic(get_soup(make_request('https://open.spotify.com/playlist/6snlZhdBpJK0cxYURvqhFU?si=8e7eb1f3db5f438b&nd=1'))) will return the profile pic of this playlist
 6. process_artist_album(get_soup(make_request('https://open.spotify.com/artist/06HL4z0CvFAxyc27GXpf02'))) will return all the artist albums on the artist page.
 7. filter_all_other_color("SpotifyPictureHelper/tests/test2.png", (0, 0, 0), (25, 25, 25)) leaves the image with pixels that fall between (0, 0, 0) and (25, 25, 25)
 8. filter_this_color("SpotifyPictureHelper/tests/test2.png", (0, 0, 0), (25, 25, 25)) filters all pixels that fall between (0, 0, 0) and (25, 25, 25)
 9. smooth_img("SpotifyPictureHelper/tests/test2.png") will smooth the image with the kernel size (5,5)
 10. return_most_common_color("SpotifyPictureHelper/tests/test2.png") will return the most common color in this image file 
-11. overlay_two_images("SpotifyPictureHelper/tests/test2.png", "SpotifyPictureHelper/tests/blackWhite.png", 0.5, 0.5) will return a blended image with the first image weighing 50% and the second image weighing also 50%
+11. overlay_two_images("SpotifyPictureHelper/tests/test2.png", "SpotifyPictureHelper/tests/blackWhite.png", 0.5, 0.5) will return a blended image with the first image weighing 50% and the second image weighing also 50%
```

### Comparing `SpotifyPictureHelper-0.2.0/SpotifyPictureHelper/main.py` & `SpotifyPictureHelper-0.2.1/SpotifyPictureHelper/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     Returns:
         Beautiful Soup Object
 
     """
     return BeautifulSoup(request.content, "html.parser")
 
 
-def process_user_profile_pic(soup: BeautifulSoup):
+def process_user_profile_pic(soup: BeautifulSoup, img_path=None):
     """Finds the user profile picture given its soup
 
     Finds and saves the user profile picture locally.
 
     Args:
         soup (Beautiful Soup object): the beautiful soup object to be analyzed
 
@@ -52,54 +52,58 @@
     # this is the profile image
     pic = make_request(f"{src}")
     # this is the user name
     head = soup.find("head")
     title = head.find("title")
     username = title.text.split(" ")[0]
     if pic.status_code == 200:
-        with open(f"./images/{username}.jpg", "wb") as f:
+        path = img_path if img_path else f"./images/{username}.jpg"
+        with open(path, "wb") as f:
             f.write(pic.content)
     else:
         raise Exception("Failed to fetch picture")
     return (username, src)
 
 
-def get_public_playlists_albums(soup: BeautifulSoup):
+def get_public_playlists_albums(soup: BeautifulSoup, img_path=None):
     """Fetches and saves the public playlist album pictures
 
     Given a user's profile's soup, fetches and saves all the album pictures of the public playlists the user has.
 
     Args:
         soup (BeautifulSoup object): return value of get_soup
+        img_path (string): the path to save the image. If none, the program will save to images directory.
 
     Returns:
         tuple: returns username and the number of public playlists found
 
     """
     res = soup.findAll("img")[1:]
     head = soup.find("head")
     title = head.find("title")
     username = title.text.split(" ")[0]
     for i in range(0, len(res)):
         ele = res[i]
         src = ele.get("src")
         pic = make_request(f"{src}")
         if pic.status_code == 200:
-            with open(f"./images/{username}_playlist_{i}.jpg", "wb") as f:
+            path = img_path if img_path else f"./images/{username}_playlist_{i}.jpg"
+            with open(path, "wb") as f:
                 f.write(pic.content)
     return (username, len(res))
 
 
-def get_individual_album_covers_from_mosaic(link):
+def get_individual_album_covers_from_mosaic(link, img_path=None):
     """Take one mosaic album cover and save four individual covers from it
 
     This is the function to get individual pictures from a mosaic album cover
 
     Args:
         link (string): The link of the mosaic album picture
+        img_path (string): the path to save the image. If none, the program will save to images directory.
 
     Returns:
         list: a list of individual album picture links
 
     """
     # For example: "https://mosaic.scdn.co/300/ab67616d00001e022a6ab83ec179747bc3b190dcab67616d00001e02335534788cbc39cfd23ee993ab67616d00001e02d6df3bccf3ec41ea2f76debcab67616d00001e02f0855ff71aa79ab842164fc6"
     if "https://mosaic.scdn.co/" not in link:
@@ -112,47 +116,51 @@
     if len(imgs) != 160:
         return Exception("Sorry this link cannot be broken down")
     pre = "https://lite-images-i.scdn.co/image/"
     for i in range(0, 4):
         li_imgs.append(pre + imgs[i * 40 : (i + 1) * 40])
         pic = make_request(pre + imgs[i * 40 : (i + 1) * 40])
         if pic.status_code == 200:
-            with open(f"./images/mosaic_{i}.jpg", "wb") as f:
+            path = img_path if img_path else f"./images/mosaic_{i}.jpg"
+            with open(path, "wb") as f:
                 f.write(pic.content)
     return li_imgs
 
 
-def get_playlist_profile_pic(soup):
+def get_playlist_profile_pic(soup, img_path=None):
     """Fetches and saves the cover picture of a playlist
 
     Args:
         soup (BeautifulSoup object): return value of get_soup
+        img_path (string): the path to save the image. If none, the program will save to images directory.
 
     Returns:
         tuple: the name of the playlist and the link of the image
 
     """
     res = soup.findAll("img")[0]
     # find playlist name
     name = soup.find("h1")
     playlist_name = name.text
     pic = make_request(res.get("src"))
     if pic.status_code == 200:
-        with open(f"./images/{playlist_name}_profile.jpg", "wb") as f:
+        path = img_path if img_path else f"./images/{playlist_name}_profile.jpg"
+        with open(path, "wb") as f:
             f.write(pic.content)
     return (playlist_name, res.get("src"))
 
 
-def process_artist_album(soup: BeautifulSoup):
+def process_artist_album(soup: BeautifulSoup, img_path=None):
     """Gets and saves the album covers given an artist
 
     Given the soup of the artist page, fetches all the album covers on that page and saves them locally.
 
     Args:
         soup (BeautifulSoup object): Return value of get_soup
+        img_path (string): the path to save the image. If none, the program will save to images directory.
 
     Returns:
         list: a list of dictionaries, each dictionary contains the albumName, albumLink, albumImageUrl, and albumSlug
 
     """
     # Find the h2 tag with text of Albums
     albumHeading = soup.find("h2", string="Albums")
@@ -181,15 +189,16 @@
         }
 
         albumObj.append(albumDetails)
 
         # Download the image at the image URL and save it in an images folder
         pic = make_request(f"{albumImage}")
         if pic.status_code == 200:
-            with open(f"./images/{albumSlug}.jpg", "wb") as f:
+            path = img_path if img_path else f"./images/{albumSlug}.jpg"
+            with open(path, "wb") as f:
                 f.write(pic.content)
     return albumObj
 
 
 def filter_all_other_color(path_to_img, threshold_low, threshold_high):
     """Returns a new image that only contains color within a certain range
```

### Comparing `SpotifyPictureHelper-0.2.0/SpotifyPictureHelper/tests/blackWhite.png` & `SpotifyPictureHelper-0.2.1/SpotifyPictureHelper/tests/blackWhite.png`

 * *Files identical despite different names*

### Comparing `SpotifyPictureHelper-0.2.0/SpotifyPictureHelper/tests/fakeArtist.html` & `SpotifyPictureHelper-0.2.1/SpotifyPictureHelper/tests/fakeArtist.html`

 * *Files identical despite different names*

### Comparing `SpotifyPictureHelper-0.2.0/SpotifyPictureHelper/tests/fakePlaylist.html` & `SpotifyPictureHelper-0.2.1/SpotifyPictureHelper/tests/fakePlaylist.html`

 * *Files identical despite different names*

### Comparing `SpotifyPictureHelper-0.2.0/SpotifyPictureHelper/tests/fakeUser.html` & `SpotifyPictureHelper-0.2.1/SpotifyPictureHelper/tests/fakeUser.html`

 * *Files identical despite different names*

### Comparing `SpotifyPictureHelper-0.2.0/SpotifyPictureHelper/tests/overlay.png` & `SpotifyPictureHelper-0.2.1/SpotifyPictureHelper/tests/overlay.png`

 * *Files identical despite different names*

### Comparing `SpotifyPictureHelper-0.2.0/SpotifyPictureHelper/tests/test2.png` & `SpotifyPictureHelper-0.2.1/SpotifyPictureHelper/tests/test2.png`

 * *Files identical despite different names*

### Comparing `SpotifyPictureHelper-0.2.0/SpotifyPictureHelper/tests/test_all.py` & `SpotifyPictureHelper-0.2.1/SpotifyPictureHelper/tests/test_all.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,14 +3,21 @@
 from bs4 import BeautifulSoup
 import os
 import pytest
 import cv2
 import numpy as np
 
 
+def check_file_exists_and_delete(path):
+    f = open(path, "rb")
+    yield f
+    f.close()
+    os.remove(path)
+
+
 class TestSpotifyHelper:
     def test_make_request(self):
         response = spotify.make_request('https://open.spotify.com/user/rosycarina')
         assert response.url == 'https://open.spotify.com/user/rosycarina'
 
     @patch('requests.get')
     def test_get_soup(self, mock_requests):
@@ -27,27 +34,61 @@
             fake_html = f.read()
             soup = BeautifulSoup(fake_html, "html.parser")
             assert spotify.process_user_profile_pic(soup) == (
                 'rosycarina',
                 'https://i.scdn.co/image/ab6775700000ee85c88b63d30ae5472bf4bee010',
             )
 
+    def test_process_user_profile_pic_with_path(self):
+        # fake HTML to create BeautifulSoup object
+        with open(os.path.join(os.sys.path[0], "fakeUser.html"), "r") as f:
+            fake_html = f.read()
+            soup = BeautifulSoup(fake_html, "html.parser")
+            assert spotify.process_user_profile_pic(soup, img_path='./images/test_img_user.jpg') == (
+                'rosycarina',
+                'https://i.scdn.co/image/ab6775700000ee85c88b63d30ae5472bf4bee010',
+            ) and check_file_exists_and_delete('./images/test_img_user.jpg')
+
     def test_get_public_playlists_albums(self):
         with open(os.path.join(os.sys.path[0], "fakeUser.html"), "r") as f:
             fake_html = f.read()
             soup = BeautifulSoup(fake_html, "html.parser")
             assert spotify.get_public_playlists_albums(soup) == ('rosycarina', 10)
 
+    def test_get_public_playlists_albums_with_path(self):
+        with open(os.path.join(os.sys.path[0], "fakeUser.html"), "r") as f:
+            fake_html = f.read()
+            soup = BeautifulSoup(fake_html, "html.parser")
+            assert spotify.get_public_playlists_albums(soup, img_path='./images/test_img_playlist.jpg') == (
+                'rosycarina',
+                10,
+            ) and check_file_exists_and_delete('./images/test_img_playlist.jpg')
+
     def test_get_individual_album_covers_from_mosaic(self):
         pre = "https://lite-images-i.scdn.co/image/"
         string = "ab67616d00001e022a6ab83ec179747bc3b190dcab67616d00001e02335534788cbc39cfd23ee993ab67616d00001e02d6df3bccf3ec41ea2f76debcab67616d00001e02f0855ff71aa79ab842164fc6"
         assert spotify.get_individual_album_covers_from_mosaic(
             'https://mosaic.scdn.co/300/ab67616d00001e022a6ab83ec179747bc3b190dcab67616d00001e02335534788cbc39cfd23ee993ab67616d00001e02d6df3bccf3ec41ea2f76debcab67616d00001e02f0855ff71aa79ab842164fc6'
         ) == [pre + string[:40], pre + string[40:80], pre + string[80:120], pre + string[120:]]
 
+    def test_get_individual_album_covers_from_mosaic_with_path(self):
+        pre = "https://lite-images-i.scdn.co/image/"
+        string = "ab67616d00001e022a6ab83ec179747bc3b190dcab67616d00001e02335534788cbc39cfd23ee993ab67616d00001e02d6df3bccf3ec41ea2f76debcab67616d00001e02f0855ff71aa79ab842164fc6"
+        assert spotify.get_individual_album_covers_from_mosaic(
+            'https://mosaic.scdn.co/300/ab67616d00001e022a6ab83ec179747bc3b190dcab67616d00001e02335534788cbc39cfd23ee993ab67616d00001e02d6df3bccf3ec41ea2f76debcab67616d00001e02f0855ff71aa79ab842164fc6',
+            './images/test_mosaic.jpg',
+        ) == [
+            pre + string[:40],
+            pre + string[40:80],
+            pre + string[80:120],
+            pre + string[120:],
+        ] and check_file_exists_and_delete(
+            './images/test_mosaic.jpg'
+        )
+
     def test_get_individual_album_covers_from_mosaic_invalid_html(self):
         html = "skjfslf;ls"
         with pytest.raises(Exception):
             spotify.get_individual_album_covers_from_mosaic(html)
 
     def test_get_individual_album_covers_from_mosaic_incomplete_html(self):
         html = "https://mosaic.scdn.co/"
@@ -64,26 +105,47 @@
             fake_html = f.read()
             soup = BeautifulSoup(fake_html, "html.parser")
             assert spotify.get_playlist_profile_pic(soup) == (
                 'Daily Mix 4',
                 "https://dailymix-images.scdn.co/v2/img/ab6761610000e5eb2f8dfdfeb85c3fc2d11b2ae2/4/en/default",
             )
 
+    def test_get_playlist_profile_pic_with_path(self):
+        with open(os.path.join(os.sys.path[0], "fakePlaylist.html"), "r") as f:
+            fake_html = f.read()
+            soup = BeautifulSoup(fake_html, "html.parser")
+            assert spotify.get_playlist_profile_pic(soup, img_path='./images/test_img_profile.jpg') == (
+                'Daily Mix 4',
+                "https://dailymix-images.scdn.co/v2/img/ab6761610000e5eb2f8dfdfeb85c3fc2d11b2ae2/4/en/default",
+            ) and check_file_exists_and_delete('./images/test_img_profile.jpg')
+
     def test_process_artist_album(self):
         fake_html = ''
         with open(os.path.join(os.sys.path[0], "fakeArtist.html"), "r") as f:
             fake_html = f.read()
         soup = BeautifulSoup(fake_html, "html.parser")
         assert spotify.process_artist_album(soup)[0] == {
             'albumName': 'Midnights (3am Edition)',
             'albumLink': '/album/3lS1y25WAhcqJDATJK70Mq',
             'albumImageUrl': 'https://i.scdn.co/image/ab67616d00001e02e0b60c608586d88252b8fbc0',
             'albumSlug': 'midnights-(3am-edition)',
         }
 
+    def test_process_artist_album_with_path(self):
+        fake_html = ''
+        with open(os.path.join(os.sys.path[0], "fakeArtist.html"), "r") as f:
+            fake_html = f.read()
+        soup = BeautifulSoup(fake_html, "html.parser")
+        assert spotify.process_artist_album(soup, img_path='./images/test_img_slug.jpg')[0] == {
+            'albumName': 'Midnights (3am Edition)',
+            'albumLink': '/album/3lS1y25WAhcqJDATJK70Mq',
+            'albumImageUrl': 'https://i.scdn.co/image/ab67616d00001e02e0b60c608586d88252b8fbc0',
+            'albumSlug': 'midnights-(3am-edition)',
+        } and check_file_exists_and_delete('./images/test_img_slug.jpg')
+
     def test_filter_all_other_color(self):
         fake_path_to_img = "SpotifyPictureHelper/tests/blackWhite.png"
         fake_threshold_low = (0, 0, 0)
         fake_threshold_high = (30, 30, 30)
         new_img = spotify.filter_all_other_color(fake_path_to_img, fake_threshold_low, fake_threshold_high)
         count = len(new_img) * len(new_img[0])
         c = 0
```

### Comparing `SpotifyPictureHelper-0.2.0/SpotifyPictureHelper.egg-info/SOURCES.txt` & `SpotifyPictureHelper-0.2.1/SpotifyPictureHelper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SpotifyPictureHelper-0.2.0/pyproject.toml` & `SpotifyPictureHelper-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 build-backend="setuptools.build_meta"
 
 [project]
 name = "SpotifyPictureHelper"
 authors = [{name = "Daisy Ye", email = "daisyye20010730@gmail.com"}]
 description="A python library that helps with the analysis of Spotify pictures."
 readme = "README.md"
-version = "0.2.0"
+version = "0.2.1"
 requires-python = ">=3.7"
 
 dependencies = ['requests','bs4', 'numpy', 'opencv-python']
 
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Programming Language :: Python :: Implementation :: CPython",
```

### Comparing `SpotifyPictureHelper-0.2.0/setup.cfg` & `SpotifyPictureHelper-0.2.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = SpotifyPictureHelper
-version = v0.2.0
+version = v0.2.1
 author = Daisy ye
 author_email = daisyye20010730@gmail.com
 description = A python library that helps with the analysis of Spotify pictures.
 
 [options]
 zip_safe = False
 include_package_data = True
```

