# Comparing `tmp/heic_to_jpg-0.1.8.tar.gz` & `tmp/heic_to_jpg-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/heic_to_jpg-0.1.8.tar", last modified: Mon Nov 30 09:55:04 2020, max compression
+gzip compressed data, was "heic_to_jpg-0.1.9.tar", last modified: Thu May  4 18:49:30 2023, max compression
```

## Comparing `heic_to_jpg-0.1.8.tar` & `heic_to_jpg-0.1.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 creimers   (501) staff       (20)        0 2020-11-30 09:55:04.000000 heic_to_jpg-0.1.8/
--rw-r--r--   0 creimers   (501) staff       (20)     1076 2020-11-29 21:59:19.000000 heic_to_jpg-0.1.8/LICENSE
--rw-r--r--   0 creimers   (501) staff       (20)      242 2020-11-29 21:59:19.000000 heic_to_jpg-0.1.8/MANIFEST.in
--rw-r--r--   0 creimers   (501) staff       (20)     1647 2020-11-30 09:55:04.000000 heic_to_jpg-0.1.8/PKG-INFO
--rw-r--r--   0 creimers   (501) staff       (20)      685 2020-11-30 09:54:27.000000 heic_to_jpg-0.1.8/README.md
-drwxr-xr-x   0 creimers   (501) staff       (20)        0 2020-11-30 09:55:03.000000 heic_to_jpg-0.1.8/heic_to_jpg/
--rw-r--r--   0 creimers   (501) staff       (20)      184 2020-11-30 09:54:56.000000 heic_to_jpg-0.1.8/heic_to_jpg/__init__.py
--rw-r--r--   0 creimers   (501) staff       (20)     1998 2020-11-30 09:03:56.000000 heic_to_jpg-0.1.8/heic_to_jpg/cli.py
-drwxr-xr-x   0 creimers   (501) staff       (20)        0 2020-11-30 09:55:04.000000 heic_to_jpg-0.1.8/heic_to_jpg.egg-info/
--rw-r--r--   0 creimers   (501) staff       (20)     1647 2020-11-30 09:55:03.000000 heic_to_jpg-0.1.8/heic_to_jpg.egg-info/PKG-INFO
--rw-r--r--   0 creimers   (501) staff       (20)      381 2020-11-30 09:55:03.000000 heic_to_jpg-0.1.8/heic_to_jpg.egg-info/SOURCES.txt
--rw-r--r--   0 creimers   (501) staff       (20)        1 2020-11-30 09:55:03.000000 heic_to_jpg-0.1.8/heic_to_jpg.egg-info/dependency_links.txt
--rw-r--r--   0 creimers   (501) staff       (20)       86 2020-11-30 09:55:03.000000 heic_to_jpg-0.1.8/heic_to_jpg.egg-info/entry_points.txt
--rw-r--r--   0 creimers   (501) staff       (20)        1 2020-11-30 09:55:03.000000 heic_to_jpg-0.1.8/heic_to_jpg.egg-info/not-zip-safe
--rw-r--r--   0 creimers   (501) staff       (20)       11 2020-11-30 09:55:03.000000 heic_to_jpg-0.1.8/heic_to_jpg.egg-info/requires.txt
--rw-r--r--   0 creimers   (501) staff       (20)       12 2020-11-30 09:55:03.000000 heic_to_jpg-0.1.8/heic_to_jpg.egg-info/top_level.txt
--rw-r--r--   0 creimers   (501) staff       (20)      443 2020-11-30 09:55:04.000000 heic_to_jpg-0.1.8/setup.cfg
--rw-r--r--   0 creimers   (501) staff       (20)     1599 2020-11-30 09:54:56.000000 heic_to_jpg-0.1.8/setup.py
-drwxr-xr-x   0 creimers   (501) staff       (20)        0 2020-11-30 09:55:04.000000 heic_to_jpg-0.1.8/tests/
--rw-r--r--   0 creimers   (501) staff       (20)       41 2020-11-29 21:59:19.000000 heic_to_jpg-0.1.8/tests/__init__.py
--rw-r--r--   0 creimers   (501) staff       (20)      999 2020-11-29 21:59:19.000000 heic_to_jpg-0.1.8/tests/test_heic_to_jpg.py
+drwxr-xr-x   0 creimers   (501) staff       (20)        0 2023-05-04 18:49:30.362438 heic_to_jpg-0.1.9/
+-rw-r--r--   0 creimers   (501) staff       (20)     1076 2023-05-04 18:44:35.000000 heic_to_jpg-0.1.9/LICENSE
+-rw-r--r--   0 creimers   (501) staff       (20)      242 2023-05-04 18:44:35.000000 heic_to_jpg-0.1.9/MANIFEST.in
+-rw-r--r--   0 creimers   (501) staff       (20)     1908 2023-05-04 18:49:30.362501 heic_to_jpg-0.1.9/PKG-INFO
+-rw-r--r--   0 creimers   (501) staff       (20)     1103 2023-05-04 18:44:35.000000 heic_to_jpg-0.1.9/README.md
+drwxr-xr-x   0 creimers   (501) staff       (20)        0 2023-05-04 18:49:30.361402 heic_to_jpg-0.1.9/heic_to_jpg/
+-rw-r--r--   0 creimers   (501) staff       (20)      184 2023-05-04 18:48:25.000000 heic_to_jpg-0.1.9/heic_to_jpg/__init__.py
+-rw-r--r--   0 creimers   (501) staff       (20)     1908 2023-05-04 18:44:35.000000 heic_to_jpg-0.1.9/heic_to_jpg/cli.py
+drwxr-xr-x   0 creimers   (501) staff       (20)        0 2023-05-04 18:49:30.362136 heic_to_jpg-0.1.9/heic_to_jpg.egg-info/
+-rw-r--r--   0 creimers   (501) staff       (20)     1908 2023-05-04 18:49:30.000000 heic_to_jpg-0.1.9/heic_to_jpg.egg-info/PKG-INFO
+-rw-r--r--   0 creimers   (501) staff       (20)      381 2023-05-04 18:49:30.000000 heic_to_jpg-0.1.9/heic_to_jpg.egg-info/SOURCES.txt
+-rw-r--r--   0 creimers   (501) staff       (20)        1 2023-05-04 18:49:30.000000 heic_to_jpg-0.1.9/heic_to_jpg.egg-info/dependency_links.txt
+-rw-r--r--   0 creimers   (501) staff       (20)       86 2023-05-04 18:49:30.000000 heic_to_jpg-0.1.9/heic_to_jpg.egg-info/entry_points.txt
+-rw-r--r--   0 creimers   (501) staff       (20)        1 2023-05-04 18:49:30.000000 heic_to_jpg-0.1.9/heic_to_jpg.egg-info/not-zip-safe
+-rw-r--r--   0 creimers   (501) staff       (20)       11 2023-05-04 18:49:30.000000 heic_to_jpg-0.1.9/heic_to_jpg.egg-info/requires.txt
+-rw-r--r--   0 creimers   (501) staff       (20)       12 2023-05-04 18:49:30.000000 heic_to_jpg-0.1.9/heic_to_jpg.egg-info/top_level.txt
+-rw-r--r--   0 creimers   (501) staff       (20)      443 2023-05-04 18:49:30.362855 heic_to_jpg-0.1.9/setup.cfg
+-rw-r--r--   0 creimers   (501) staff       (20)     1599 2023-05-04 18:48:25.000000 heic_to_jpg-0.1.9/setup.py
+drwxr-xr-x   0 creimers   (501) staff       (20)        0 2023-05-04 18:49:30.362342 heic_to_jpg-0.1.9/tests/
+-rw-r--r--   0 creimers   (501) staff       (20)       41 2023-05-04 18:44:35.000000 heic_to_jpg-0.1.9/tests/__init__.py
+-rw-r--r--   0 creimers   (501) staff       (20)      999 2023-05-04 18:44:35.000000 heic_to_jpg-0.1.9/tests/test_heic_to_jpg.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `heic_to_jpg-0.1.8/LICENSE` & `heic_to_jpg-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `heic_to_jpg-0.1.8/README.md` & `heic_to_jpg-0.1.9/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 # `heic-to-jpg` 📸
 
 CLI tool for converting `HEIC` images to `jpg`.
 
-Essentially, this is just a wrapper around imagemagick's [`convert`](https://imagemagick.org/script/convert.php) cli.
+Essentially, this is just a thin wrapper around imagemagick's [`convert`](https://imagemagick.org/script/convert.php) cli.
 
 Motivation: When transfering images from an iPhone to a Mac via airdrop, they are being transfered as `HEIC`. Oftentime though, another format (such as `jpg`) is required to further make use of those images.
 
+👉 ⚠️ Please note that [imagemagick](https://imagemagick.org/script/download.php) is a prerequisite for this to work.
+
+👉 ⚠️ Please note that this has been tested on macOS only. There might be issues on other operating systems ([Linux](https://github.com/creimers/heic-to-jpg/issues/1), [Windows](https://github.com/creimers/heic-to-jpg/issues/2)).
+
 ## installation
 
 `pip install heic-to-jpg`
 
 ## usage
 
-`heic-to-jpg -s ~/path/to/source [--keep]`
+`heic-to-jpg -s ~/path/to/source [--keep] [--debug None|Trace|All]`
 
 or
 
-`heic2jpg -s ~/path/to/source [--keep]`
+`heic2jpg -s ~/path/to/source [--keep] [--debug None|Trace|All]` 
 
 `~/path/to/source` can both be a directory or a single `.HEIC` file. Without the `--keep` flag, the original file is deleted after conversion.
```

### Comparing `heic_to_jpg-0.1.8/heic_to_jpg/cli.py` & `heic_to_jpg-0.1.9/heic_to_jpg/cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,72 +14,68 @@
 @click.option(
     "--src",
     "-s",
     type=click.Path(exists=True),
     help="Source directory of images to process or path to single image",
     required=True,
 )
-def main(keep, src):
+@click.option(
+    "--debug",
+    default="None",
+    help="Print convert debug info",
+    type=click.Choice(["None", "Trace", "All"], case_sensitive=False),
+)
+def main(keep, src, debug):
     # check for 'convert'
     try:
         cmd = ["which", "convert"]
         subprocess.check_output(cmd)
     except Exception:
         click.secho("Program 'convert' not found!", fg="red")
         return
 
+    image_to_convert = []
     if os.path.isdir(src):
-
         ###########
         # DIRECTORY
         ###########
-
-        image_to_convert = []
         for filename in os.listdir(src):
-            if filename.endswith(".heic") or filename.endswith(".HEIC"):
+            if filename.lower().endswith(".heic"):
                 absolute_filename = os.path.join(src, filename)
-                # convert_image(absolute_filename)
                 image_to_convert.append(absolute_filename)
-
-        pwd = os.getcwd()
-        os.chdir(src)
-        command = [
-            "convert",
-            "*.HEIC",
-            "-set",
-            "filename:base",
-            "%[basename]",
-            "%[filename:base].jpg",
-        ]
-        subprocess.call(command)
-        os.chdir(pwd)
-
-        # remove?
-        if not keep:
-            for filename in image_to_convert:
-                os.remove(filename)
-    elif src.endswith(".heic") or src.endswith(".HEIC"):
-
+        target = "*.[hH][eE][iI][cC]*"
+        src_dir = src
+    elif src.lower().endswith(".heic"):
         #############
         # SINGLE FILE
         #############
-
-        pwd = os.getcwd()
-        src_folder = os.path.abspath(os.path.dirname(src))
-        os.chdir(src_folder)
-        command = [
-            "convert",
-            src,
-            "-set",
-            "filename:base",
-            "%[basename]",
-            "%[filename:base].jpg",
-        ]
-        subprocess.call(command)
+        target = src
+        image_to_convert.append(src)
+        src_dir = os.path.abspath(os.path.dirname(src))
+
+    pwd = os.getcwd()
+    os.chdir(src_dir)
+
+    command = [
+        "convert",
+        "-debug",
+        debug,
+        target,
+        "-set",
+        "filename:base",
+        "%[basename]",
+        "%[filename:base].jpg",
+    ]
+    if debug in ("Trace", "All"):
+        print(f"{command=}")
+    subprocess.call(command)
+    if os.path.isdir(src):
         os.chdir(pwd)
 
-        if not keep:
-            os.remove(src)
+    # remove?
+    if not keep:
+        for filename in image_to_convert:
+            os.remove(filename)
 
 
 if __name__ == "__main__":
     sys.exit(main())  # pragma: no cover
```

### Comparing `heic_to_jpg-0.1.8/setup.py` & `heic_to_jpg-0.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,10 +50,10 @@
     name="heic_to_jpg",
     py_modules=["heic_to_jpg"],
     packages=find_packages(include=["heic_to_jpg", "heic_to_jpg.*"]),
     setup_requires=setup_requirements,
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/creimers/heic-to-jpg",
-    version="0.1.8",
+    version="0.1.9",
     zip_safe=False,
 )
```

### Comparing `heic_to_jpg-0.1.8/tests/test_heic_to_jpg.py` & `heic_to_jpg-0.1.9/tests/test_heic_to_jpg.py`

 * *Files identical despite different names*

