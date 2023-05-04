# Comparing `tmp/sra-pylib-1.4.1.tar.gz` & `tmp/sra-pylib-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sra-pylib-1.4.1.tar", last modified: Tue Apr 11 14:23:20 2023, max compression
+gzip compressed data, was "sra-pylib-1.4.2.tar", last modified: Thu May  4 07:28:44 2023, max compression
```

## Comparing `sra-pylib-1.4.1.tar` & `sra-pylib-1.4.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:23:20.262072 sra-pylib-1.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-04-11 14:22:56.000000 sra-pylib-1.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-04-11 14:23:20.262072 sra-pylib-1.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-04-11 14:22:56.000000 sra-pylib-1.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 14:23:20.262072 sra-pylib-1.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-04-11 14:22:56.000000 sra-pylib-1.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:23:20.262072 sra-pylib-1.4.1/sra/
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-11 14:22:56.000000 sra-pylib-1.4.1/sra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20783 2023-04-11 14:22:56.000000 sra-pylib-1.4.1/sra/animal.py
--rw-r--r--   0 runner    (1001) docker     (123)     9383 2023-04-11 14:22:56.000000 sra-pylib-1.4.1/sra/animu.py
--rw-r--r--   0 runner    (1001) docker     (123)    96923 2023-04-11 14:22:56.000000 sra-pylib-1.4.1/sra/canvas.py
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-04-11 14:22:56.000000 sra-pylib-1.4.1/sra/chatbot.py
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-04-11 14:22:56.000000 sra-pylib-1.4.1/sra/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-04-11 14:22:56.000000 sra-pylib-1.4.1/sra/facts.py
--rw-r--r--   0 runner    (1001) docker     (123)    23111 2023-04-11 14:22:56.000000 sra-pylib-1.4.1/sra/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     9339 2023-04-11 14:22:56.000000 sra-pylib-1.4.1/sra/others.py
--rw-r--r--   0 runner    (1001) docker     (123)     8585 2023-04-11 14:22:56.000000 sra-pylib-1.4.1/sra/pokemon.py
--rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-04-11 14:22:56.000000 sra-pylib-1.4.1/sra/welcome.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 14:23:20.262072 sra-pylib-1.4.1/sra_pylib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3838 2023-04-11 14:23:20.000000 sra-pylib-1.4.1/sra_pylib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-11 14:23:20.000000 sra-pylib-1.4.1/sra_pylib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 14:23:20.000000 sra-pylib-1.4.1/sra_pylib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-11 14:23:20.000000 sra-pylib-1.4.1/sra_pylib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-11 14:23:20.000000 sra-pylib-1.4.1/sra_pylib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:28:44.695573 sra-pylib-1.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-05-04 07:28:28.000000 sra-pylib-1.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4488 2023-05-04 07:28:44.695573 sra-pylib-1.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-05-04 07:28:28.000000 sra-pylib-1.4.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 07:28:44.695573 sra-pylib-1.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-05-04 07:28:28.000000 sra-pylib-1.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:28:44.695573 sra-pylib-1.4.2/sra/
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-05-04 07:28:28.000000 sra-pylib-1.4.2/sra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20792 2023-05-04 07:28:28.000000 sra-pylib-1.4.2/sra/animal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9388 2023-05-04 07:28:28.000000 sra-pylib-1.4.2/sra/animu.py
+-rw-r--r--   0 runner    (1001) docker     (123)    96967 2023-05-04 07:28:28.000000 sra-pylib-1.4.2/sra/canvas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-05-04 07:28:28.000000 sra-pylib-1.4.2/sra/chatbot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-05-04 07:28:28.000000 sra-pylib-1.4.2/sra/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5756 2023-05-04 07:28:28.000000 sra-pylib-1.4.2/sra/facts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23122 2023-05-04 07:28:28.000000 sra-pylib-1.4.2/sra/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9347 2023-05-04 07:28:28.000000 sra-pylib-1.4.2/sra/others.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8589 2023-05-04 07:28:28.000000 sra-pylib-1.4.2/sra/pokemon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4410 2023-05-04 07:28:28.000000 sra-pylib-1.4.2/sra/welcome.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 07:28:44.695573 sra-pylib-1.4.2/sra_pylib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4488 2023-05-04 07:28:44.000000 sra-pylib-1.4.2/sra_pylib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-05-04 07:28:44.000000 sra-pylib-1.4.2/sra_pylib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 07:28:44.000000 sra-pylib-1.4.2/sra_pylib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-04 07:28:44.000000 sra-pylib-1.4.2/sra_pylib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-04 07:28:44.000000 sra-pylib-1.4.2/sra_pylib.egg-info/top_level.txt
```

### Comparing `sra-pylib-1.4.1/LICENSE` & `sra-pylib-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sra-pylib-1.4.1/PKG-INFO` & `sra-pylib-1.4.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sra-pylib
-Version: 1.4.1
+Version: 1.4.2
 Summary: A Wrapper of some-random-api for Python
 Home-page: https://github.com/Sayad-Uddin-Tahsin/sra-pylib
 Author: Sayad Uddin Tahsin
 Author-email: mr.pluto012@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/Sayad-Uddin-Tahsin/sra-pylib/wiki
 Project-URL: Bug Tracker, https://github.com/Sayad-Uddin-Tahsin/sra-pylib/issues
@@ -20,24 +20,28 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # sra-pylib
-`sra-pylib` is a Python wrapper for [some-random-api](https://some-random-api.ml).
+`sra-pylib` is a Python wrapper for [some-random-api](https://some-random-api.com).
 
 ```python
 import sra
+from sra import animal
 
->>> print(sra.animal.Panda.image_link)  # Prints a Panda Image link
+# Create a new instance of the Panda class
+panda = animal.Panda()
+
+>>> print(panda.image_link)  # Prints a Panda Image link
 "https://i.imgur.com/YVLrUO9.jpg"
->>> print(sra.animal.Panda.fact)  # Prints a Panda Fact
-"Giant pandas have been driven out of the lowland areas where they used to live and now are found only in the Chinese provinces of Sichuan, Gansu, and Shaanxi. The forests in these provinces are very damp and rainy. In one year, a forest may receive up to 50 inches of rain and snow."
->>> sra.animal.Panda.save_image()  # Saves the Image
+>>> print(panda.fact)  # Prints a Panda Fact
+"From 1974-1989, half of the panda’s habitat in China’s Sichuan areas was destroyed by human activity."
+>>> panda.save_image("Cool Panda.png")  # Saves the Image
 ```
 With `sra-pylib`, you can easily access the various endpoints of `some-random-api` in your Python projects, making it a powerful tool for working with image, fact, and other types of data.
 
 <a href="https://pypi.org/project/sra-pylib"><img src="https://img.shields.io/pypi/status/sra-pylib?label=Status&logo=pypi&logoColor=ffffff" height=22></a>
 <a href="https://pypi.org/project/sra-pylib"><img src="https://img.shields.io/pypi/v/sra-pylib?label=PyPI Version&logo=pypi&logoColor=ffffff" height=22></a>
 <a href="https://app.fossa.com/projects/git%2Bgithub.com%2FSayad-Uddin-Tahsin%2Fsra-pylib?ref=badge_shield" alt="FOSSA Status"><img src="https://app.fossa.com/api/projects/git%2Bgithub.com%2FSayad-Uddin-Tahsin%2Fsra-pylib.svg?type=shield" height=22></a>
 <a href="https://python.org"><img src="https://img.shields.io/pypi/pyversions/sra-pylib?label=Python&logo=python&logoColor=ffdd54" height=22></a>
@@ -53,16 +57,30 @@
 `sra-pylib` is synced with some-random-api. It has all the Endpoints provided by some-random-api except the Premium ones.
 
 ## Documentation
 Full documentation for the sra-pylib module can be found on [Wiki](https://github.com/Sayad-Uddin-Tahsin/sra-pylib/wiki). The documentation includes detailed information on how to use the module, including examples and reference documentation for all classes and methods.
 
 If you have any questions or issues with the module, please refer to the documentation or submit a bug report on the [GitHub issues page](https://github.com/Sayad-Uddin-Tahsin/sra-pylib/issues).
 
+
+## Bug Report
+If you encounter any bugs while using sra-pylib, please report them by opening a new issue on the [GitHub repository](https://github.com/Sayad-Uddin-Tahsin/sra-pylib/issues). When reporting a bug, please include the following information:
+
+- A detailed description of the issue, including what you were trying to do when the bug occurred
+- The full traceback or error message, if applicable
+- Steps to reproduce the bug, if possible
+- Any additional information or context that might be relevant to the issue
+
+By reporting bugs, you can help improve the quality and reliability of sra-pylib for all user
+
+
 ## Cloning the Repository
-You also can install sra-pylib directly from Github, by using this pip command:
+You can easily clone this repository by executing the following command:
 ```console
-pip install git+https://github.com/Sayad-Uddin-Tahsin/sra-pylib.git
+git clone https://github.com/Sayad-Uddin-Tahsin/sra-pylib.git
 ```
-This will install the package directly from the repository.
+This will clone the whole repository in your computer.
+
+You can also download the repository as a `zip` file: [Download as zip](https://github.com/Sayad-Uddin-Tahsin/sra-pylib/archive/refs/heads/main.zip)
 
 ## License
 [![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2FSayad-Uddin-Tahsin%2Fsra-pylib.svg?type=large)](https://app.fossa.com/projects/git%2Bgithub.com%2FSayad-Uddin-Tahsin%2Fsra-pylib?ref=badge_large)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1,46 +1,55 @@
-Metadata-Version: 2.1 Name: sra-pylib Version: 1.4.1 Summary: A Wrapper of
+Metadata-Version: 2.1 Name: sra-pylib Version: 1.4.2 Summary: A Wrapper of
 some-random-api for Python Home-page: https://github.com/Sayad-Uddin-Tahsin/
 sra-pylib Author: Sayad Uddin Tahsin Author-email: mr.pluto012@gmail.com
 License: MIT Project-URL: Documentation, https://github.com/Sayad-Uddin-Tahsin/
 sra-pylib/wiki Project-URL: Bug Tracker, https://github.com/Sayad-Uddin-Tahsin/
 sra-pylib/issues Project-URL: PyPI, https://pypi.org/project/sra-pylib/
 Keywords: some-random-api,sra,api-wrapper,sra-pylib,sra-wrapper,tahsin-project
 Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-
 Python: >=3.7 Description-Content-Type: text/markdown License-File: LICENSE #
 sra-pylib `sra-pylib` is a Python wrapper for [some-random-api](https://some-
-random-api.ml). ```python import sra >>> print(sra.animal.Panda.image_link) #
-Prints a Panda Image link "https://i.imgur.com/YVLrUO9.jpg" >>> print
-(sra.animal.Panda.fact) # Prints a Panda Fact "Giant pandas have been driven
-out of the lowland areas where they used to live and now are found only in the
-Chinese provinces of Sichuan, Gansu, and Shaanxi. The forests in these
-provinces are very damp and rainy. In one year, a forest may receive up to 50
-inches of rain and snow." >>> sra.animal.Panda.save_image() # Saves the Image
-``` With `sra-pylib`, you can easily access the various endpoints of `some-
-random-api` in your Python projects, making it a powerful tool for working with
-image, fact, and other types of data. [https://img.shields.io/pypi/status/sra-
+random-api.com). ```python import sra from sra import animal # Create a new
+instance of the Panda class panda = animal.Panda() >>> print(panda.image_link)
+# Prints a Panda Image link "https://i.imgur.com/YVLrUO9.jpg" >>> print
+(panda.fact) # Prints a Panda Fact "From 1974-1989, half of the pandaâs
+habitat in Chinaâs Sichuan areas was destroyed by human activity." >>>
+panda.save_image("Cool Panda.png") # Saves the Image ``` With `sra-pylib`, you
+can easily access the various endpoints of `some-random-api` in your Python
+projects, making it a powerful tool for working with image, fact, and other
+types of data. [https://img.shields.io/pypi/status/sra-
 pylib?label=Status&logo=pypi&logoColor=ffffff] [https://img.shields.io/pypi/v/
 sra-pylib?label=PyPI_Version&logo=pypi&logoColor=ffffff] [https://
 app.fossa.com/api/projects/git%2Bgithub.com%2FSayad-Uddin-Tahsin%2Fsra-
 pylib.svg?type=shield] [https://img.shields.io/pypi/pyversions/sra-
 pylib?label=Python&logo=python&logoColor=ffdd54] ## Installation You can
 install `sra-pylib` using `pip`: ```console python -m pip install sra-pylib ```
 `sra-pylib` requires Python 3.7 or later. ## Endpoints `sra-pylib` is synced
 with some-random-api. It has all the Endpoints provided by some-random-api
 except the Premium ones. ## Documentation Full documentation for the sra-pylib
 module can be found on [Wiki](https://github.com/Sayad-Uddin-Tahsin/sra-pylib/
 wiki). The documentation includes detailed information on how to use the
 module, including examples and reference documentation for all classes and
 methods. If you have any questions or issues with the module, please refer to
 the documentation or submit a bug report on the [GitHub issues page](https://
-github.com/Sayad-Uddin-Tahsin/sra-pylib/issues). ## Cloning the Repository You
-also can install sra-pylib directly from Github, by using this pip command:
-```console pip install git+https://github.com/Sayad-Uddin-Tahsin/sra-pylib.git
-``` This will install the package directly from the repository. ## License [!
-[FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2FSayad-
-Uddin-Tahsin%2Fsra-pylib.svg?type=large)](https://app.fossa.com/projects/
+github.com/Sayad-Uddin-Tahsin/sra-pylib/issues). ## Bug Report If you encounter
+any bugs while using sra-pylib, please report them by opening a new issue on
+the [GitHub repository](https://github.com/Sayad-Uddin-Tahsin/sra-pylib/
+issues). When reporting a bug, please include the following information: - A
+detailed description of the issue, including what you were trying to do when
+the bug occurred - The full traceback or error message, if applicable - Steps
+to reproduce the bug, if possible - Any additional information or context that
+might be relevant to the issue By reporting bugs, you can help improve the
+quality and reliability of sra-pylib for all user ## Cloning the Repository You
+can easily clone this repository by executing the following command: ```console
+git clone https://github.com/Sayad-Uddin-Tahsin/sra-pylib.git ``` This will
+clone the whole repository in your computer. You can also download the
+repository as a `zip` file: [Download as zip](https://github.com/Sayad-Uddin-
+Tahsin/sra-pylib/archive/refs/heads/main.zip) ## License [![FOSSA Status]
+(https://app.fossa.com/api/projects/git%2Bgithub.com%2FSayad-Uddin-
+Tahsin%2Fsra-pylib.svg?type=large)](https://app.fossa.com/projects/
 git%2Bgithub.com%2FSayad-Uddin-Tahsin%2Fsra-pylib?ref=badge_large)
```

### Comparing `sra-pylib-1.4.1/README.md` & `sra-pylib-1.4.2/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,43 +1,61 @@
-# sra-pylib
-`sra-pylib` is a Python wrapper for [some-random-api](https://some-random-api.ml).
-
-```python
-import sra
-
->>> print(sra.animal.Panda.image_link)  # Prints a Panda Image link
-"https://i.imgur.com/YVLrUO9.jpg"
->>> print(sra.animal.Panda.fact)  # Prints a Panda Fact
-"Giant pandas have been driven out of the lowland areas where they used to live and now are found only in the Chinese provinces of Sichuan, Gansu, and Shaanxi. The forests in these provinces are very damp and rainy. In one year, a forest may receive up to 50 inches of rain and snow."
->>> sra.animal.Panda.save_image()  # Saves the Image
-```
-With `sra-pylib`, you can easily access the various endpoints of `some-random-api` in your Python projects, making it a powerful tool for working with image, fact, and other types of data.
-
-<a href="https://pypi.org/project/sra-pylib"><img src="https://img.shields.io/pypi/status/sra-pylib?label=Status&logo=pypi&logoColor=ffffff" height=22></a>
-<a href="https://pypi.org/project/sra-pylib"><img src="https://img.shields.io/pypi/v/sra-pylib?label=PyPI Version&logo=pypi&logoColor=ffffff" height=22></a>
-<a href="https://app.fossa.com/projects/git%2Bgithub.com%2FSayad-Uddin-Tahsin%2Fsra-pylib?ref=badge_shield" alt="FOSSA Status"><img src="https://app.fossa.com/api/projects/git%2Bgithub.com%2FSayad-Uddin-Tahsin%2Fsra-pylib.svg?type=shield" height=22></a>
-<a href="https://python.org"><img src="https://img.shields.io/pypi/pyversions/sra-pylib?label=Python&logo=python&logoColor=ffdd54" height=22></a>
-
-## Installation
-You can install `sra-pylib` using `pip`:
-```console
-python -m pip install sra-pylib
-```
-`sra-pylib` requires Python 3.7 or later.
-
-## Endpoints
-`sra-pylib` is synced with some-random-api. It has all the Endpoints provided by some-random-api except the Premium ones.
-
-## Documentation
-Full documentation for the sra-pylib module can be found on [Wiki](https://github.com/Sayad-Uddin-Tahsin/sra-pylib/wiki). The documentation includes detailed information on how to use the module, including examples and reference documentation for all classes and methods.
-
-If you have any questions or issues with the module, please refer to the documentation or submit a bug report on the [GitHub issues page](https://github.com/Sayad-Uddin-Tahsin/sra-pylib/issues).
-
-## Cloning the Repository
-You also can install sra-pylib directly from Github, by using this pip command:
-```console
-pip install git+https://github.com/Sayad-Uddin-Tahsin/sra-pylib.git
-```
-This will install the package directly from the repository.
-
-## License
-[![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2FSayad-Uddin-Tahsin%2Fsra-pylib.svg?type=large)](https://app.fossa.com/projects/git%2Bgithub.com%2FSayad-Uddin-Tahsin%2Fsra-pylib?ref=badge_large)
+# sra-pylib
+`sra-pylib` is a Python wrapper for [some-random-api](https://some-random-api.com).
+
+```python
+import sra
+from sra import animal
+
+# Create a new instance of the Panda class
+panda = animal.Panda()
+
+>>> print(panda.image_link)  # Prints a Panda Image link
+"https://i.imgur.com/YVLrUO9.jpg"
+>>> print(panda.fact)  # Prints a Panda Fact
+"From 1974-1989, half of the panda’s habitat in China’s Sichuan areas was destroyed by human activity."
+>>> panda.save_image("Cool Panda.png")  # Saves the Image
+```
+With `sra-pylib`, you can easily access the various endpoints of `some-random-api` in your Python projects, making it a powerful tool for working with image, fact, and other types of data.
+
+<a href="https://pypi.org/project/sra-pylib"><img src="https://img.shields.io/pypi/status/sra-pylib?label=Status&logo=pypi&logoColor=ffffff" height=22></a>
+<a href="https://pypi.org/project/sra-pylib"><img src="https://img.shields.io/pypi/v/sra-pylib?label=PyPI Version&logo=pypi&logoColor=ffffff" height=22></a>
+<a href="https://app.fossa.com/projects/git%2Bgithub.com%2FSayad-Uddin-Tahsin%2Fsra-pylib?ref=badge_shield" alt="FOSSA Status"><img src="https://app.fossa.com/api/projects/git%2Bgithub.com%2FSayad-Uddin-Tahsin%2Fsra-pylib.svg?type=shield" height=22></a>
+<a href="https://python.org"><img src="https://img.shields.io/pypi/pyversions/sra-pylib?label=Python&logo=python&logoColor=ffdd54" height=22></a>
+
+## Installation
+You can install `sra-pylib` using `pip`:
+```console
+python -m pip install sra-pylib
+```
+`sra-pylib` requires Python 3.7 or later.
+
+## Endpoints
+`sra-pylib` is synced with some-random-api. It has all the Endpoints provided by some-random-api except the Premium ones.
+
+## Documentation
+Full documentation for the sra-pylib module can be found on [Wiki](https://github.com/Sayad-Uddin-Tahsin/sra-pylib/wiki). The documentation includes detailed information on how to use the module, including examples and reference documentation for all classes and methods.
+
+If you have any questions or issues with the module, please refer to the documentation or submit a bug report on the [GitHub issues page](https://github.com/Sayad-Uddin-Tahsin/sra-pylib/issues).
+
+
+## Bug Report
+If you encounter any bugs while using sra-pylib, please report them by opening a new issue on the [GitHub repository](https://github.com/Sayad-Uddin-Tahsin/sra-pylib/issues). When reporting a bug, please include the following information:
+
+- A detailed description of the issue, including what you were trying to do when the bug occurred
+- The full traceback or error message, if applicable
+- Steps to reproduce the bug, if possible
+- Any additional information or context that might be relevant to the issue
+
+By reporting bugs, you can help improve the quality and reliability of sra-pylib for all user
+
+
+## Cloning the Repository
+You can easily clone this repository by executing the following command:
+```console
+git clone https://github.com/Sayad-Uddin-Tahsin/sra-pylib.git
+```
+This will clone the whole repository in your computer.
+
+You can also download the repository as a `zip` file: [Download as zip](https://github.com/Sayad-Uddin-Tahsin/sra-pylib/archive/refs/heads/main.zip)
+
+## License
+[![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2FSayad-Uddin-Tahsin%2Fsra-pylib.svg?type=large)](https://app.fossa.com/projects/git%2Bgithub.com%2FSayad-Uddin-Tahsin%2Fsra-pylib?ref=badge_large)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1,32 +1,41 @@
 # sra-pylib `sra-pylib` is a Python wrapper for [some-random-api](https://some-
-random-api.ml). ```python import sra >>> print(sra.animal.Panda.image_link) #
-Prints a Panda Image link "https://i.imgur.com/YVLrUO9.jpg" >>> print
-(sra.animal.Panda.fact) # Prints a Panda Fact "Giant pandas have been driven
-out of the lowland areas where they used to live and now are found only in the
-Chinese provinces of Sichuan, Gansu, and Shaanxi. The forests in these
-provinces are very damp and rainy. In one year, a forest may receive up to 50
-inches of rain and snow." >>> sra.animal.Panda.save_image() # Saves the Image
-``` With `sra-pylib`, you can easily access the various endpoints of `some-
-random-api` in your Python projects, making it a powerful tool for working with
-image, fact, and other types of data. [https://img.shields.io/pypi/status/sra-
+random-api.com). ```python import sra from sra import animal # Create a new
+instance of the Panda class panda = animal.Panda() >>> print(panda.image_link)
+# Prints a Panda Image link "https://i.imgur.com/YVLrUO9.jpg" >>> print
+(panda.fact) # Prints a Panda Fact "From 1974-1989, half of the pandaâs
+habitat in Chinaâs Sichuan areas was destroyed by human activity." >>>
+panda.save_image("Cool Panda.png") # Saves the Image ``` With `sra-pylib`, you
+can easily access the various endpoints of `some-random-api` in your Python
+projects, making it a powerful tool for working with image, fact, and other
+types of data. [https://img.shields.io/pypi/status/sra-
 pylib?label=Status&logo=pypi&logoColor=ffffff] [https://img.shields.io/pypi/v/
 sra-pylib?label=PyPI_Version&logo=pypi&logoColor=ffffff] [https://
 app.fossa.com/api/projects/git%2Bgithub.com%2FSayad-Uddin-Tahsin%2Fsra-
 pylib.svg?type=shield] [https://img.shields.io/pypi/pyversions/sra-
 pylib?label=Python&logo=python&logoColor=ffdd54] ## Installation You can
 install `sra-pylib` using `pip`: ```console python -m pip install sra-pylib ```
 `sra-pylib` requires Python 3.7 or later. ## Endpoints `sra-pylib` is synced
 with some-random-api. It has all the Endpoints provided by some-random-api
 except the Premium ones. ## Documentation Full documentation for the sra-pylib
 module can be found on [Wiki](https://github.com/Sayad-Uddin-Tahsin/sra-pylib/
 wiki). The documentation includes detailed information on how to use the
 module, including examples and reference documentation for all classes and
 methods. If you have any questions or issues with the module, please refer to
 the documentation or submit a bug report on the [GitHub issues page](https://
-github.com/Sayad-Uddin-Tahsin/sra-pylib/issues). ## Cloning the Repository You
-also can install sra-pylib directly from Github, by using this pip command:
-```console pip install git+https://github.com/Sayad-Uddin-Tahsin/sra-pylib.git
-``` This will install the package directly from the repository. ## License [!
-[FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2FSayad-
-Uddin-Tahsin%2Fsra-pylib.svg?type=large)](https://app.fossa.com/projects/
+github.com/Sayad-Uddin-Tahsin/sra-pylib/issues). ## Bug Report If you encounter
+any bugs while using sra-pylib, please report them by opening a new issue on
+the [GitHub repository](https://github.com/Sayad-Uddin-Tahsin/sra-pylib/
+issues). When reporting a bug, please include the following information: - A
+detailed description of the issue, including what you were trying to do when
+the bug occurred - The full traceback or error message, if applicable - Steps
+to reproduce the bug, if possible - Any additional information or context that
+might be relevant to the issue By reporting bugs, you can help improve the
+quality and reliability of sra-pylib for all user ## Cloning the Repository You
+can easily clone this repository by executing the following command: ```console
+git clone https://github.com/Sayad-Uddin-Tahsin/sra-pylib.git ``` This will
+clone the whole repository in your computer. You can also download the
+repository as a `zip` file: [Download as zip](https://github.com/Sayad-Uddin-
+Tahsin/sra-pylib/archive/refs/heads/main.zip) ## License [![FOSSA Status]
+(https://app.fossa.com/api/projects/git%2Bgithub.com%2FSayad-Uddin-
+Tahsin%2Fsra-pylib.svg?type=large)](https://app.fossa.com/projects/
 git%2Bgithub.com%2FSayad-Uddin-Tahsin%2Fsra-pylib?ref=badge_large)
```

### Comparing `sra-pylib-1.4.1/setup.py` & `sra-pylib-1.4.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='sra-pylib',
-    version='1.4.1',
+    version='1.4.2',
     author='Sayad Uddin Tahsin',
     author_email='mr.pluto012@gmail.com',
     description='A Wrapper of some-random-api for Python',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/Sayad-Uddin-Tahsin/sra-pylib',
     packages=find_packages(),
```

### Comparing `sra-pylib-1.4.1/sra/__init__.py` & `sra-pylib-1.4.2/sra/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from sra import image
 from sra import others
 from sra import pokemon
 from sra import welcome
 from sra import exceptions
 import datetime
 
-__version__ = "1.4.1"
+__version__ = "1.4.2"
 __copyright__ = f"© Copyright 2023 {('- ' + str(datetime.datetime.today().year) + ' ') if int(datetime.datetime.today().year) != 2023 else ''}Sayad Uddin Tahsin."
 __author__ = "Sayad Uddin Tahsin"
 __author_email__ = "mr.pluto012@gmail.com"
 __documentation__ = "https://github.com/Sayad-Uddin-Tahsin/sra-pylib/wiki"
 __url__ = "https://github.com/Sayad-Uddin-Tahsin/sra-pylib/wiki"
 __bug_report__ = "https://github.com/Sayad-Uddin-Tahsin/sra-pylib/issues"
 __license__ = "MIT"
```

### Comparing `sra-pylib-1.4.1/sra/animal.py` & `sra-pylib-1.4.2/sra/animal.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     :raise APITimeout: API taken too long to respond!
     :raise APIError: Error Returned by API
     """
     def __init__(self):
         self.__resp = None
 
         try:
-            self.__resp = requests.get("https://some-random-api.ml/animal/bird")
+            self.__resp = requests.get("https://some-random-api.com/animal/bird")
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.APITimeout("API taken too long to respond!")
         if self.__resp.status_code != 200:
             if 'error' in self.__resp.json():
                 raise sra.exceptions.APIError(self.__resp.json()['error'])
             else:
                 raise sra.exceptions.APIError(
@@ -69,15 +69,15 @@
     :raise APITimeout: API taken too long to respond!
     :raise APIError: Error Returned by API
     """
     def __init__(self):
         self.__resp = None
 
         try:
-            self.__resp = requests.get("https://some-random-api.ml/animal/cat")
+            self.__resp = requests.get("https://some-random-api.com/animal/cat")
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.APITimeout("API taken too long to respond!")
         if self.__resp.status_code != 200:
             if 'error' in self.__resp.json():
                 raise sra.exceptions.APIError(self.__resp.json()['error'])
             else:
                 raise sra.exceptions.APIError(
@@ -129,15 +129,15 @@
     :raise APITimeout: API taken too long to respond!
     :raise APIError: Error Returned by API
     """
     def __init__(self):
         self.__resp = None
 
         try:
-            self.__resp = requests.get("https://some-random-api.ml/animal/dog")
+            self.__resp = requests.get("https://some-random-api.com/animal/dog")
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.APITimeout("API taken too long to respond!")
         if self.__resp.status_code != 200:
             if 'error' in self.__resp.json():
                 raise sra.exceptions.APIError(self.__resp.json()['error'])
             else:
                 raise sra.exceptions.APIError(
@@ -189,15 +189,15 @@
     :raise APITimeout: API taken too long to respond!
     :raise APIError: Error Returned by API
     """
     def __init__(self):
         self.__resp = None
 
         try:
-            self.__resp = requests.get("https://some-random-api.ml/animal/fox")
+            self.__resp = requests.get("https://some-random-api.com/animal/fox")
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.APITimeout("API taken too long to respond!")
         if self.__resp.status_code != 200:
             if 'error' in self.__resp.json():
                 raise sra.exceptions.APIError(self.__resp.json()['error'])
             else:
                 raise sra.exceptions.APIError(
@@ -249,15 +249,15 @@
     :raise APITimeout: API taken too long to respond!
     :raise APIError: Error Returned by API
     """
     def __init__(self):
         self.__resp = None
 
         try:
-            self.__resp = requests.get("https://some-random-api.ml/animal/kangaroo")
+            self.__resp = requests.get("https://some-random-api.com/animal/kangaroo")
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.APITimeout("API taken too long to respond!")
         if self.__resp.status_code != 200:
             if 'error' in self.__resp.json():
                 raise sra.exceptions.APIError(self.__resp.json()['error'])
             else:
                 raise sra.exceptions.APIError(
@@ -309,15 +309,15 @@
     :raise APITimeout: API taken too long to respond!
     :raise APIError: Error Returned by API
     """
     def __init__(self):
         self.__resp = None
 
         try:
-            self.__resp = requests.get("https://some-random-api.ml/animal/koala")
+            self.__resp = requests.get("https://some-random-api.com/animal/koala")
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.APITimeout("API taken too long to respond!")
         if self.__resp.status_code != 200:
             if 'error' in self.__resp.json():
                 raise sra.exceptions.APIError(self.__resp.json()['error'])
             else:
                 raise sra.exceptions.APIError(
@@ -369,15 +369,15 @@
     :raise APITimeout: API taken too long to respond!
     :raise APIError: Error Returned by API
     """
     def __init__(self):
         self.__resp = None
 
         try:
-            self.__resp = requests.get("https://some-random-api.ml/animal/panda")
+            self.__resp = requests.get("https://some-random-api.com/animal/panda")
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.APITimeout("API taken too long to respond!")
         if self.__resp.status_code != 200:
             if 'error' in self.__resp.json():
                 raise sra.exceptions.APIError(self.__resp.json()['error'])
             else:
                 raise sra.exceptions.APIError(
@@ -429,15 +429,15 @@
     :raise APITimeout: API taken too long to respond!
     :raise APIError: Error Returned by API
     """
     def __init__(self):
         self.__resp = None
 
         try:
-            self.__resp = requests.get("https://some-random-api.ml/animal/raccoon")
+            self.__resp = requests.get("https://some-random-api.com/animal/raccoon")
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.APITimeout("API taken too long to respond!")
         if self.__resp.status_code != 200:
             if 'error' in self.__resp.json():
                 raise sra.exceptions.APIError(self.__resp.json()['error'])
             else:
                 raise sra.exceptions.APIError(
@@ -489,15 +489,15 @@
     :raise APITimeout: API taken too long to respond!
     :raise APIError: Error Returned by API
     """
     def __init__(self):
         self.__resp = None
 
         try:
-            self.__resp = requests.get("https://some-random-api.ml/animal/red_panda")
+            self.__resp = requests.get("https://some-random-api.com/animal/red_panda")
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.APITimeout("API taken too long to respond!")
         if self.__resp.status_code != 200:
             if 'error' in self.__resp.json():
                 raise sra.exceptions.APIError(self.__resp.json()['error'])
             else:
                 raise sra.exceptions.APIError(
```

### Comparing `sra-pylib-1.4.1/sra/animu.py` & `sra-pylib-1.4.2/sra/animu.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     :raise APITimeout: API taken too long to respond!
     :raise APIError: Error Returned by API
     """
     def __init__(self):
         self.__resp = None
 
         try:
-            self.__resp = requests.get("https://some-random-api.ml/animu/face-palm")
+            self.__resp = requests.get("https://some-random-api.com/animu/face-palm")
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.APITimeout("API taken too long to respond!")
         if self.__resp.status_code != 200:
             if 'error' in self.__resp.json():
                 raise sra.exceptions.APIError(self.__resp.json()['error'])
             else:
                 raise sra.exceptions.APIError(
@@ -61,15 +61,15 @@
     :raise APITimeout: API taken too long to respond!
     :raise APIError: Error Returned by API
     """
     def __init__(self):
         self.__resp = None
 
         try:
-            self.__resp = requests.get("https://some-random-api.ml/animu/hug")
+            self.__resp = requests.get("https://some-random-api.com/animu/hug")
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.APITimeout("API taken too long to respond!")
         if self.__resp.status_code != 200:
             if 'error' in self.__resp.json():
                 raise sra.exceptions.APIError(self.__resp.json()['error'])
             else:
                 raise sra.exceptions.APIError(
@@ -113,15 +113,15 @@
     :raise APITimeout: API taken too long to respond!
     :raise APIError: Error Returned by API
     """
     def __init__(self):
         self.__resp = None
 
         try:
-            self.__resp = requests.get("https://some-random-api.ml/animu/pat")
+            self.__resp = requests.get("https://some-random-api.com/animu/pat")
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.APITimeout("API taken too long to respond!")
         if self.__resp.status_code != 200:
             if 'error' in self.__resp.json():
                 raise sra.exceptions.APIError(self.__resp.json()['error'])
             else:
                 raise sra.exceptions.APIError(
@@ -165,15 +165,15 @@
     :raise APITimeout: API taken too long to respond!
     :raise APIError: Error Returned by API
     """
     def __init__(self):
         self.__resp = None
 
         try:
-            self.__resp = requests.get("https://some-random-api.ml/animu/wink")
+            self.__resp = requests.get("https://some-random-api.com/animu/wink")
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.APITimeout("API taken too long to respond!")
         if self.__resp.status_code != 200:
             if 'error' in self.__resp.json():
                 raise sra.exceptions.APIError(self.__resp.json()['error'])
             else:
                 raise sra.exceptions.APIError(
@@ -217,15 +217,15 @@
     :raise APITimeout: API taken too long to respond!
     :raise APIError: Error Returned by API
     """
     def __init__(self):
         self.__resp = None
 
         try:
-            self.__resp = requests.get("https://some-random-api.ml/animu/quote")
+            self.__resp = requests.get("https://some-random-api.com/animu/quote")
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.APITimeout("API taken too long to respond!")
         if self.__resp.status_code != 200:
             if 'error' in self.__resp.json():
                 raise sra.exceptions.APIError(self.__resp.json()['error'])
             else:
                 raise sra.exceptions.APIError(
```

### Comparing `sra-pylib-1.4.1/sra/canvas.py` & `sra-pylib-1.4.2/sra/canvas.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,15 @@
         if not validFormat:
             raise sra.exceptions.InvalidFileFormat(
                 'Invalid File Format given. File Format must be ".png", ".jpg" or "jpeg"!')
 
         path = name
 
         try:
-            self.__resp = requests.get(f"https://some-random-api.ml/canvas/filter/blue?avatar={avatar_url}",
+            self.__resp = requests.get(f"https://some-random-api.com/canvas/filter/blue?avatar={avatar_url}",
                                        stream=True)
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.ImageRetrieveError("Unable to Load the Image!")
         if self.__resp.status_code == 200:
             with open(path, 'wb') as f:
                 f.write(self.__resp.content)
                 return True
@@ -115,15 +115,15 @@
         if not validFormat:
             raise sra.exceptions.InvalidFileFormat(
                 'Invalid File Format given. File Format must be ".png", ".jpg" or "jpeg"!')
 
         path = name
 
         try:
-            self.__resp = requests.get(f"https://some-random-api.ml/canvas/filter/blurple?avatar={avatar_url}",
+            self.__resp = requests.get(f"https://some-random-api.com/canvas/filter/blurple?avatar={avatar_url}",
                                        stream=True)
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.ImageRetrieveError("Unable to Load the Image!")
         if self.__resp.status_code == 200:
             with open(path, 'wb') as f:
                 f.write(self.__resp.content)
                 return True
@@ -162,15 +162,15 @@
         if not validFormat:
             raise sra.exceptions.InvalidFileFormat(
                 'Invalid File Format given. File Format must be ".png", ".jpg" or "jpeg"!')
 
         path = name
 
         try:
-            self.__resp = requests.get(f"https://some-random-api.ml/canvas/filter/blurple2?avatar={avatar_url}",
+            self.__resp = requests.get(f"https://some-random-api.com/canvas/filter/blurple2?avatar={avatar_url}",
                                        stream=True)
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.ImageRetrieveError("Unable to Load the Image!")
         if self.__resp.status_code == 200:
             with open(path, 'wb') as f:
                 f.write(self.__resp.content)
                 return True
@@ -214,15 +214,15 @@
             raise sra.exceptions.InvalidFileFormat(
                 'Invalid File Format given. File Format must be ".png", ".jpg" or "jpeg"!')
 
         path = name
 
         try:
             self.__resp = requests.get(
-                f"https://some-random-api.ml/canvas/filter/brightness?avatar={avatar_url}&brightness={brightness}",
+                f"https://some-random-api.com/canvas/filter/brightness?avatar={avatar_url}&brightness={brightness}",
                 stream=True)
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.ImageRetrieveError("Unable to Load the Image!")
         if self.__resp.status_code == 200:
             with open(path, 'wb') as f:
                 f.write(self.__resp.content)
                 return True
@@ -269,15 +269,15 @@
         if not validFormat:
             raise sra.exceptions.InvalidFileFormat(
                 'Invalid File Format given. File Format must be ".png", ".jpg" or "jpeg"!')
 
         path = name
 
         try:
-            self.__resp = requests.get(f"https://some-random-api.ml/canvas/color?color={color}&avatar={avatar_url}",
+            self.__resp = requests.get(f"https://some-random-api.com/canvas/color?color={color}&avatar={avatar_url}",
                                        stream=True)
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.ImageRetrieveError("Unable to Load the Image!")
         if self.__resp.status_code == 200:
             with open(path, 'wb') as f:
                 f.write(self.__resp.content)
                 return True
@@ -323,15 +323,15 @@
         if not validFormat:
             raise sra.exceptions.InvalidFileFormat(
                 'Invalid File Format given. File Format must be ".png", ".jpg" or "jpeg"!')
 
         path = name
 
         try:
-            self.__resp = requests.get(f"https://some-random-api.ml/canvas/color?color={color}&avatar={avatar_url}",
+            self.__resp = requests.get(f"https://some-random-api.com/canvas/color?color={color}&avatar={avatar_url}",
                                        stream=True)
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.ImageRetrieveError("Unable to Load the Image!")
         if self.__resp.status_code == 200:
             with open(path, 'wb') as f:
                 f.write(self.__resp.content)
                 return True
@@ -370,15 +370,15 @@
         if not validFormat:
             raise sra.exceptions.InvalidFileFormat(
                 'Invalid File Format given. File Format must be ".png", ".jpg" or "jpeg"!')
 
         path = name
 
         try:
-            self.__resp = requests.get(f"https://some-random-api.ml/canvas/filter/green?avatar={avatar_url}",
+            self.__resp = requests.get(f"https://some-random-api.com/canvas/filter/green?avatar={avatar_url}",
                                        stream=True)
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.ImageRetrieveError("Unable to Load the Image!")
         if self.__resp.status_code == 200:
             with open(path, 'wb') as f:
                 f.write(self.__resp.content)
                 return True
@@ -417,15 +417,15 @@
         if not validFormat:
             raise sra.exceptions.InvalidFileFormat(
                 'Invalid File Format given. File Format must be ".png", ".jpg" or "jpeg"!')
 
         path = name
 
         try:
-            self.__resp = requests.get(f"https://some-random-api.ml/canvas/filter/greyscale?avatar={avatar_url}",
+            self.__resp = requests.get(f"https://some-random-api.com/canvas/filter/greyscale?avatar={avatar_url}",
                                        stream=True)
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.ImageRetrieveError("Unable to Load the Image!")
         if self.__resp.status_code == 200:
             with open(path, 'wb') as f:
                 f.write(self.__resp.content)
                 return True
@@ -464,15 +464,15 @@
         if not validFormat:
             raise sra.exceptions.InvalidFileFormat(
                 'Invalid File Format given. File Format must be ".png", ".jpg" or "jpeg"!')
 
         path = name
 
         try:
-            self.__resp = requests.get(f"https://some-random-api.ml/canvas/filter/invertgreyscale?avatar={avatar_url}",
+            self.__resp = requests.get(f"https://some-random-api.com/canvas/filter/invertgreyscale?avatar={avatar_url}",
                                        stream=True)
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.ImageRetrieveError("Unable to Load the Image!")
         if self.__resp.status_code == 200:
             with open(path, 'wb') as f:
                 f.write(self.__resp.content)
                 return True
@@ -511,15 +511,15 @@
         if not validFormat:
             raise sra.exceptions.InvalidFileFormat(
                 'Invalid File Format given. File Format must be ".png", ".jpg" or "jpeg"!')
 
         path = name
 
         try:
-            self.__resp = requests.get(f"https://some-random-api.ml/canvas/filter/red?avatar={avatar_url}", stream=True)
+            self.__resp = requests.get(f"https://some-random-api.com/canvas/filter/red?avatar={avatar_url}", stream=True)
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.ImageRetrieveError("Unable to Load the Image!")
         if self.__resp.status_code == 200:
             with open(path, 'wb') as f:
                 f.write(self.__resp.content)
                 return True
         else:
@@ -557,15 +557,15 @@
         if not validFormat:
             raise sra.exceptions.InvalidFileFormat(
                 'Invalid File Format given. File Format must be ".png", ".jpg" or "jpeg"!')
 
         path = name
 
         try:
-            self.__resp = requests.get(f"https://some-random-api.ml/canvas/filter/sepia?avatar={avatar_url}",
+            self.__resp = requests.get(f"https://some-random-api.com/canvas/filter/sepia?avatar={avatar_url}",
                                        stream=True)
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.ImageRetrieveError("Unable to Load the Image!")
         if self.__resp.status_code == 200:
             with open(path, 'wb') as f:
                 f.write(self.__resp.content)
                 return True
@@ -609,15 +609,15 @@
         if 0 > int(threshold) > 255:
             raise sra.exceptions.ThresholdError("Threshold Power must be within 0 - 255!")
 
         path = name
 
         try:
             self.__resp = requests.get(
-                f"https://some-random-api.ml/canvas/threshold?avatar={avatar_url}&threshold={threshold}", stream=True)
+                f"https://some-random-api.com/canvas/threshold?avatar={avatar_url}&threshold={threshold}", stream=True)
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.ImageRetrieveError("Unable to Load the Image!")
         if self.__resp.status_code == 200:
             with open(path, 'wb') as f:
                 f.write(self.__resp.content)
                 return True
         else:
@@ -664,15 +664,15 @@
         if not validFormat:
             raise sra.exceptions.InvalidFileFormat(
                 'Invalid File Format given. File Format must be ".png", ".jpg" or "jpeg"!')
 
         path = name
 
         try:
-            self.__resp = requests.get(f"https://some-random-api.ml/canvas/misc/bisexual?avatar={avatar_url}",
+            self.__resp = requests.get(f"https://some-random-api.com/canvas/misc/bisexual?avatar={avatar_url}",
                                        stream=True)
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.ImageRetrieveError("Unable to Load the Image!")
         if self.__resp.status_code == 200:
             with open(path, 'wb') as f:
                 f.write(self.__resp.content)
                 return True
@@ -711,15 +711,15 @@
         if not validFormat:
             raise sra.exceptions.InvalidFileFormat(
                 'Invalid File Format given. File Format must be ".png", ".jpg" or "jpeg"!')
 
         path = name
 
         try:
-            self.__resp = requests.get(f"https://some-random-api.ml/canvas/misc/blur?avatar={avatar_url}", stream=True)
+            self.__resp = requests.get(f"https://some-random-api.com/canvas/misc/blur?avatar={avatar_url}", stream=True)
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.ImageRetrieveError("Unable to Load the Image!")
         if self.__resp.status_code == 200:
             with open(path, 'wb') as f:
                 f.write(self.__resp.content)
                 return True
         else:
@@ -753,15 +753,15 @@
         if not validFormat:
             raise sra.exceptions.InvalidFileFormat(
                 'Invalid File Format given. File Format must be ".png", ".jpg" or "jpeg"!')
 
         path = name
 
         try:
-            self.__resp = requests.get(f"https://some-random-api.ml/canvas/misc/crop?avatar={image_url}", stream=True)
+            self.__resp = requests.get(f"https://some-random-api.com/canvas/misc/crop?avatar={image_url}", stream=True)
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.ImageRetrieveError("Unable to Load the Image!")
         if self.__resp.status_code == 200:
             with open(path, 'wb') as f:
                 f.write(self.__resp.content)
                 return True
         else:
@@ -799,15 +799,15 @@
         if not validFormat:
             raise sra.exceptions.InvalidFileFormat(
                 'Invalid File Format given. File Format must be ".png", ".jpg" or "jpeg"!')
 
         path = name
 
         try:
-            self.__resp = requests.get(f"https://some-random-api.ml/canvas/misc/colorviewer?hex={hex}", stream=True)
+            self.__resp = requests.get(f"https://some-random-api.com/canvas/misc/colorviewer?hex={hex}", stream=True)
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.ImageRetrieveError("Unable to Load the Image!")
         if self.__resp.status_code == 200:
             with open(path, 'wb') as f:
                 f.write(self.__resp.content)
                 return True
         else:
@@ -845,15 +845,15 @@
         if not validFormat:
             raise sra.exceptions.InvalidFileFormat(
                 'Invalid File Format given. File Format must be ".png", ".jpg" or "jpeg"!')
 
         path = name
 
         try:
-            self.__resp = requests.get(f"https://some-random-api.ml/canvas/misc/heart?avatar={avatar_url}", stream=True)
+            self.__resp = requests.get(f"https://some-random-api.com/canvas/misc/heart?avatar={avatar_url}", stream=True)
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.ImageRetrieveError("Unable to Load the Image!")
         if self.__resp.status_code == 200:
             with open(path, 'wb') as f:
                 f.write(self.__resp.content)
                 return True
         else:
@@ -871,15 +871,15 @@
         :raise APIError: Error Returned by API
         """
         codes = rgb.split(",")
         if len(codes) != 3:
             raise sra.exceptions.InvalidRGBCode(f"RGB Color Code must contains 3 blocks!")
 
         try:
-            self.__resp = requests.get(f"https://some-random-api.ml/canvas/misc/hex?rgb={rgb}")
+            self.__resp = requests.get(f"https://some-random-api.com/canvas/misc/hex?rgb={rgb}")
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.APITimeout("API taken too long to respond!")
 
         if self.__resp.status_code == 200:
             hex = self.__resp.json()['hex']
             return hex
         else:
@@ -921,15 +921,15 @@
         if not validFormat:
             raise sra.exceptions.InvalidFileFormat(
                 'Invalid File Format given. File Format must be ".png", ".jpg" or "jpeg"!')
 
         path = name
 
         try:
-            self.__resp = requests.get(f"https://some-random-api.ml/canvas/misc/horny?avatar={avatar_url}", stream=True)
+            self.__resp = requests.get(f"https://some-random-api.com/canvas/misc/horny?avatar={avatar_url}", stream=True)
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.ImageRetrieveError("Unable to Load the Image!")
         if self.__resp.status_code == 200:
             with open(path, 'wb') as f:
                 f.write(self.__resp.content)
                 return True
         else:
@@ -967,15 +967,15 @@
         if not validFormat:
             raise sra.exceptions.InvalidFileFormat(
                 'Invalid File Format given. File Format must be ".png", ".jpg" or "jpeg"!')
 
         path = name
 
         try:
-            self.__resp = requests.get(f"https://some-random-api.ml/canvas/misc/its-so-stupid?avatar={avatar_url}",
+            self.__resp = requests.get(f"https://some-random-api.com/canvas/misc/its-so-stupid?avatar={avatar_url}",
                                        stream=True)
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.ImageRetrieveError("Unable to Load the Image!")
         if self.__resp.status_code == 200:
             with open(path, 'wb') as f:
                 f.write(self.__resp.content)
                 return True
@@ -1014,15 +1014,15 @@
         if not validFormat:
             raise sra.exceptions.InvalidFileFormat(
                 'Invalid File Format given. File Format must be ".png", ".jpg" or "jpeg"!')
 
         path = name
 
         try:
-            self.__resp = requests.get(f"https://some-random-api.ml/canvas/misc/jpg?avatar={avatar_url}", stream=True)
+            self.__resp = requests.get(f"https://some-random-api.com/canvas/misc/jpg?avatar={avatar_url}", stream=True)
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.ImageRetrieveError("Unable to Load the Image!")
         if self.__resp.status_code == 200:
             with open(path, 'wb') as f:
                 f.write(self.__resp.content)
                 return True
         else:
@@ -1060,15 +1060,15 @@
         if not validFormat:
             raise sra.exceptions.InvalidFileFormat(
                 'Invalid File Format given. File Format must be ".png", ".jpg" or "jpeg"!')
 
         path = name
 
         try:
-            self.__resp = requests.get(f"https://some-random-api.ml/canvas/misc/lesbian?avatar={avatar_url}",
+            self.__resp = requests.get(f"https://some-random-api.com/canvas/misc/lesbian?avatar={avatar_url}",
                                        stream=True)
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.ImageRetrieveError("Unable to Load the Image!")
         if self.__resp.status_code == 200:
             with open(path, 'wb') as f:
                 f.write(self.__resp.content)
                 return True
@@ -1107,15 +1107,15 @@
         if not validFormat:
             raise sra.exceptions.InvalidFileFormat(
                 'Invalid File Format given. File Format must be ".png", ".jpg" or "jpeg"!')
 
         path = name
 
         try:
-            self.__resp = requests.get(f"https://some-random-api.ml/canvas/misc/lgbt?avatar={avatar_url}", stream=True)
+            self.__resp = requests.get(f"https://some-random-api.com/canvas/misc/lgbt?avatar={avatar_url}", stream=True)
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.ImageRetrieveError("Unable to Load the Image!")
         if self.__resp.status_code == 200:
             with open(path, 'wb') as f:
                 f.write(self.__resp.content)
                 return True
         else:
@@ -1153,15 +1153,15 @@
         if not validFormat:
             raise sra.exceptions.InvalidFileFormat(
                 'Invalid File Format given. File Format must be ".png", ".jpg" or "jpeg"!')
 
         path = name
 
         try:
-            self.__resp = requests.get(f"https://some-random-api.ml/canvas/misc/lolice?avatar={avatar_url}",
+            self.__resp = requests.get(f"https://some-random-api.com/canvas/misc/lolice?avatar={avatar_url}",
                                        stream=True)
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.ImageRetrieveError("Unable to Load the Image!")
         if self.__resp.status_code == 200:
             with open(path, 'wb') as f:
                 f.write(self.__resp.content)
                 return True
@@ -1205,15 +1205,15 @@
             raise sra.exceptions.InvalidFileFormat(
                 'Invalid File Format given. File Format must be ".png", ".jpg" or "jpeg"!')
 
         path = name
 
         try:
             self.__resp = requests.get(
-                f"https://some-random-api.ml/canvas/misc/namecard?avatar={avatar_url}&birthday={birthday}&username={username}{'&description=' + description if description is not None else ''}",
+                f"https://some-random-api.com/canvas/misc/namecard?avatar={avatar_url}&birthday={birthday}&username={username}{'&description=' + description if description is not None else ''}",
                 stream=True)
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.ImageRetrieveError("Unable to Load the Image!")
         if self.__resp.status_code == 200:
             with open(path, 'wb') as f:
                 f.write(self.__resp.content)
                 return True
@@ -1246,15 +1246,15 @@
             raise sra.exceptions.InvalidFileFormat(
                 'Invalid File Format given. File Format must be ".png", ".jpg" or "jpeg"!')
 
         path = name
 
         try:
             self.__resp = requests.get(
-                f"https://some-random-api.ml/canvas/nobitches?no={urllib.parse.quote_plus(text)}",
+                f"https://some-random-api.com/canvas/nobitches?no={urllib.parse.quote_plus(text)}",
                 stream=True)
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.ImageRetrieveError("Unable to Load the Image!")
         if self.__resp.status_code == 200:
             with open(path, 'wb') as f:
                 f.write(self.__resp.content)
                 return True
@@ -1293,15 +1293,15 @@
         if not validFormat:
             raise sra.exceptions.InvalidFileFormat(
                 'Invalid File Format given. File Format must be ".png", ".jpg" or "jpeg"!')
 
         path = name
 
         try:
-            self.__resp = requests.get(f"https://some-random-api.ml/canvas/misc/nonbinary?avatar={avatar_url}",
+            self.__resp = requests.get(f"https://some-random-api.com/canvas/misc/nonbinary?avatar={avatar_url}",
                                        stream=True)
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.ImageRetrieveError("Unable to Load the Image!")
         if self.__resp.status_code == 200:
             with open(path, 'wb') as f:
                 f.write(self.__resp.content)
                 return True
@@ -1334,15 +1334,15 @@
             raise sra.exceptions.InvalidFileFormat(
                 'Invalid File Format given. File Format must be ".png", ".jpg" or "jpeg"!')
 
         path = name
 
         try:
             self.__resp = requests.get(
-                f"https://some-random-api.ml/canvas/misc/oogway?quote={urllib.parse.quote_plus(quote)}", stream=True)
+                f"https://some-random-api.com/canvas/misc/oogway?quote={urllib.parse.quote_plus(quote)}", stream=True)
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.ImageRetrieveError("Unable to Load the Image!")
         if self.__resp.status_code == 200:
             with open(path, 'wb') as f:
                 f.write(self.__resp.content)
                 return True
         else:
@@ -1373,15 +1373,15 @@
             raise sra.exceptions.InvalidFileFormat(
                 'Invalid File Format given. File Format must be ".png", ".jpg" or "jpeg"!')
 
         path = name
 
         try:
             self.__resp = requests.get(
-                f"https://some-random-api.ml/canvas/misc/oogway2?quote={urllib.parse.quote_plus(quote)}", stream=True)
+                f"https://some-random-api.com/canvas/misc/oogway2?quote={urllib.parse.quote_plus(quote)}", stream=True)
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.ImageRetrieveError("Unable to Load the Image!")
         if self.__resp.status_code == 200:
             with open(path, 'wb') as f:
                 f.write(self.__resp.content)
                 return True
         else:
@@ -1419,15 +1419,15 @@
         if not validFormat:
             raise sra.exceptions.InvalidFileFormat(
                 'Invalid File Format given. File Format must be ".png", ".jpg" or "jpeg"!')
 
         path = name
 
         try:
-            self.__resp = requests.get(f"https://some-random-api.ml/canvas/misc/pansexual?avatar={avatar_url}",
+            self.__resp = requests.get(f"https://some-random-api.com/canvas/misc/pansexual?avatar={avatar_url}",
                                        stream=True)
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.ImageRetrieveError("Unable to Load the Image!")
         if self.__resp.status_code == 200:
             with open(path, 'wb') as f:
                 f.write(self.__resp.content)
                 return True
@@ -1466,15 +1466,15 @@
         if not validFormat:
             raise sra.exceptions.InvalidFileFormat(
                 'Invalid File Format given. File Format must be ".png", ".jpg" or "jpeg"!')
 
         path = name
 
         try:
-            self.__resp = requests.get(f"https://some-random-api.ml/canvas/misc/pixelate?avatar={avatar_url}",
+            self.__resp = requests.get(f"https://some-random-api.com/canvas/misc/pixelate?avatar={avatar_url}",
                                        stream=True)
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.ImageRetrieveError("Unable to Load the Image!")
         if self.__resp.status_code == 200:
             with open(path, 'wb') as f:
                 f.write(self.__resp.content)
                 return True
@@ -1496,15 +1496,15 @@
             hex = hex.replace("#", "", 1)
 
         if len(hex) not in [6, 8]:
             raise sra.exceptions.InvalidHEXColor(
                 f"Given HEX Color Code must be 6 or 8 in length, but given code is {len(hex)} in length")
 
         try:
-            self.__resp = requests.get(f"https://some-random-api.ml/canvas/misc/rgb?hex={hex}")
+            self.__resp = requests.get(f"https://some-random-api.com/canvas/misc/rgb?hex={hex}")
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.APITimeout("API taken too long to respond!")
 
         if self.__resp.status_code == 200:
             self.__resp = self.__resp.json()
             rgb = f"{self.__resp['r']}, {self.__resp['g']}, {self.__resp['b']}"
             return rgb
@@ -1547,15 +1547,15 @@
         if not validFormat:
             raise sra.exceptions.InvalidFileFormat(
                 'Invalid File Format given. File Format must be ".png", ".jpg" or "jpeg"!')
 
         path = name
 
         try:
-            self.__resp = requests.get(f"https://some-random-api.ml/canvas/misc/simpcard?avatar={avatar_url}",
+            self.__resp = requests.get(f"https://some-random-api.com/canvas/misc/simpcard?avatar={avatar_url}",
                                        stream=True)
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.ImageRetrieveError("Unable to Load the Image!")
         if self.__resp.status_code == 200:
             with open(path, 'wb') as f:
                 f.write(self.__resp.content)
                 return True
@@ -1594,15 +1594,15 @@
         if not validFormat:
             raise sra.exceptions.InvalidFileFormat(
                 'Invalid File Format given. File Format must be ".png", ".jpg" or "jpeg"!')
 
         path = name
 
         try:
-            self.__resp = requests.get(f"https://some-random-api.ml/canvas/misc/tonikawa?avatar={avatar_url}",
+            self.__resp = requests.get(f"https://some-random-api.com/canvas/misc/tonikawa?avatar={avatar_url}",
                                        stream=True)
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.ImageRetrieveError("Unable to Load the Image!")
         if self.__resp.status_code == 200:
             with open(path, 'wb') as f:
                 f.write(self.__resp.content)
                 return True
@@ -1641,15 +1641,15 @@
         if not validFormat:
             raise sra.exceptions.InvalidFileFormat(
                 'Invalid File Format given. File Format must be ".png", ".jpg" or "jpeg"!')
 
         path = name
 
         try:
-            self.__resp = requests.get(f"https://some-random-api.ml/canvas/misc/transgender?avatar={avatar_url}",
+            self.__resp = requests.get(f"https://some-random-api.com/canvas/misc/transgender?avatar={avatar_url}",
                                        stream=True)
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.ImageRetrieveError("Unable to Load the Image!")
         if self.__resp.status_code == 200:
             with open(path, 'wb') as f:
                 f.write(self.__resp.content)
                 return True
@@ -1713,15 +1713,15 @@
             raise sra.exceptions.InvalidFileFormat(
                 'Invalid File Format given. File Format must be ".png" or ".jpg"!')
 
         path = name
 
         try:
             self.__resp = requests.get(
-                f"https://some-random-api.ml/canvas/tweet?avatar={avatar_url}&displayname={urllib.parse.quote_plus(display_name)}&username={urllib.parse.quote_plus(username)}&comment={urllib.parse.quote_plus(comment)}{'&replies=' + str(replyNumber) if replyNumber is not None else ''}{'&likes=' + str(likeNumber) if likeNumber is not None else ''}{'&retweets=' + str(retweetNumber) if retweetNumber is not None else ''}&theme={theme.lower()}",
+                f"https://some-random-api.com/canvas/tweet?avatar={avatar_url}&displayname={urllib.parse.quote_plus(display_name)}&username={urllib.parse.quote_plus(username)}&comment={urllib.parse.quote_plus(comment)}{'&replies=' + str(replyNumber) if replyNumber is not None else ''}{'&likes=' + str(likeNumber) if likeNumber is not None else ''}{'&retweets=' + str(retweetNumber) if retweetNumber is not None else ''}&theme={theme.lower()}",
                 stream=True)
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.ImageRetrieveError("Unable to Load the Image!")
         if self.__resp.status_code == 200:
             with open(path, 'wb') as f:
                 f.write(self.__resp.content)
                 return True
@@ -1768,15 +1768,15 @@
             raise sra.exceptions.InvalidFileFormat(
                 'Invalid File Format given. File Format must be ".png" or ".jpg"!')
 
         path = name
 
         try:
             self.__resp = requests.get(
-                f"https://some-random-api.ml/canvas/youtube-comment?avatar={avatar_url}&username={urllib.parse.quote_plus(username)}&comment={urllib.parse.quote_plus(comment)}",
+                f"https://some-random-api.com/canvas/youtube-comment?avatar={avatar_url}&username={urllib.parse.quote_plus(username)}&comment={urllib.parse.quote_plus(comment)}",
                 stream=True)
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.ImageRetrieveError("Unable to Load the Image!")
 
         if self.__resp.status_code == 200:
             with open(path, 'wb') as f:
                 f.write(self.__resp.content)
@@ -1825,15 +1825,15 @@
         if not validFormat:
             raise sra.exceptions.InvalidFileFormat(
                 'Invalid File Format given. File Format must be ".png", ".jpg" or "jpeg"!')
 
         path = name
 
         try:
-            self.__resp = requests.get(f"https://some-random-api.ml/canvas/comrade?avatar={avatar_url}", stream=True)
+            self.__resp = requests.get(f"https://some-random-api.com/canvas/comrade?avatar={avatar_url}", stream=True)
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.ImageRetrieveError("Unable to Load the Image!")
         if self.__resp.status_code == 200:
             with open(path, 'wb') as f:
                 f.write(self.__resp.content)
                 return True
         else:
@@ -1871,15 +1871,15 @@
         if not validFormat:
             raise sra.exceptions.InvalidFileFormat(
                 'Invalid File Format given. File Format must be ".png", ".jpg" or "jpeg"!')
 
         path = name
 
         try:
-            self.__resp = requests.get(f"https://some-random-api.ml/canvas/gay?avatar={avatar_url}", stream=True)
+            self.__resp = requests.get(f"https://some-random-api.com/canvas/gay?avatar={avatar_url}", stream=True)
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.ImageRetrieveError("Unable to Load the Image!")
         if self.__resp.status_code == 200:
             with open(path, 'wb') as f:
                 f.write(self.__resp.content)
                 return True
         else:
@@ -1917,15 +1917,15 @@
         if not validFormat:
             raise sra.exceptions.InvalidFileFormat(
                 'Invalid File Format given. File Format must be ".png", ".jpg" or "jpeg"!')
 
         path = name
 
         try:
-            self.__resp = requests.get(f"https://some-random-api.ml/canvas/glass?avatar={avatar_url}", stream=True)
+            self.__resp = requests.get(f"https://some-random-api.com/canvas/glass?avatar={avatar_url}", stream=True)
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.ImageRetrieveError("Unable to Load the Image!")
         if self.__resp.status_code == 200:
             with open(path, 'wb') as f:
                 f.write(self.__resp.content)
                 return True
         else:
@@ -1963,15 +1963,15 @@
         if not validFormat:
             raise sra.exceptions.InvalidFileFormat(
                 'Invalid File Format given. File Format must be ".png", ".jpg" or "jpeg"!')
 
         path = name
 
         try:
-            self.__resp = requests.get(f"https://some-random-api.ml/canvas/jail?avatar={avatar_url}", stream=True)
+            self.__resp = requests.get(f"https://some-random-api.com/canvas/jail?avatar={avatar_url}", stream=True)
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.ImageRetrieveError("Unable to Load the Image!")
         if self.__resp.status_code == 200:
             with open(path, 'wb') as f:
                 f.write(self.__resp.content)
                 return True
         else:
@@ -2009,15 +2009,15 @@
         if not validFormat:
             raise sra.exceptions.InvalidFileFormat(
                 'Invalid File Format given. File Format must be ".png", ".jpg" or "jpeg"!')
 
         path = name
 
         try:
-            self.__resp = requests.get(f"https://some-random-api.ml/canvas/passed?avatar={avatar_url}", stream=True)
+            self.__resp = requests.get(f"https://some-random-api.com/canvas/passed?avatar={avatar_url}", stream=True)
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.ImageRetrieveError("Unable to Load the Image!")
         if self.__resp.status_code == 200:
             with open(path, 'wb') as f:
                 f.write(self.__resp.content)
                 return True
         else:
@@ -2055,15 +2055,15 @@
         if not validFormat:
             raise sra.exceptions.InvalidFileFormat(
                 'Invalid File Format given. File Format must be ".gif"!')
 
         path = name
 
         try:
-            self.__resp = requests.get(f"https://some-random-api.ml/canvas/triggered?avatar={avatar_url}", stream=True)
+            self.__resp = requests.get(f"https://some-random-api.com/canvas/triggered?avatar={avatar_url}", stream=True)
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.ImageRetrieveError("Unable to Load the Image!")
         if self.__resp.status_code == 200:
             with open(path, 'wb') as f:
                 f.write(self.__resp.content)
                 return True
         else:
@@ -2101,15 +2101,15 @@
         if not validFormat:
             raise sra.exceptions.InvalidFileFormat(
                 'Invalid File Format given. File Format must be ".png", ".jpg" or "jpeg"!')
 
         path = name
 
         try:
-            self.__resp = requests.get(f"https://some-random-api.ml/canvas/wasted?avatar={avatar_url}", stream=True)
+            self.__resp = requests.get(f"https://some-random-api.com/canvas/wasted?avatar={avatar_url}", stream=True)
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.ImageRetrieveError("Unable to Load the Image!")
         if self.__resp.status_code == 200:
             with open(path, 'wb') as f:
                 f.write(self.__resp.content)
                 return True
         else:
```

### Comparing `sra-pylib-1.4.1/sra/chatbot.py` & `sra-pylib-1.4.2/sra/chatbot.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
     :param key: API Key (at least tier 1)
     :param prompt: The Prompt (Message that will be sent to the chatbot)
     :return: Chatbot Response
     """
     try:
         __resp = requests.get(
-            f"https://some-random-api.ml/chatbot?message={urllib.parse.quote_plus(prompt)}&key={key}")
+            f"https://some-random-api.com/chatbot?message={urllib.parse.quote_plus(prompt)}&key={key}")
     except requests.exceptions.ConnectionError:
         raise sra.exceptions.APITimeout("API taken too long to respond!")
     if __resp.status_code != 200:
         if 'error' in __resp.json():
             raise sra.exceptions.APIError(__resp.json()['error'])
         else:
             raise sra.exceptions.APIError(
```

### Comparing `sra-pylib-1.4.1/sra/exceptions.py` & `sra-pylib-1.4.2/sra/exceptions.py`

 * *Files identical despite different names*

### Comparing `sra-pylib-1.4.1/sra/facts.py` & `sra-pylib-1.4.2/sra/facts.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
     :raise APITimeout: API taken too long to respond!
     :raise APIError: Error Returned by API
     """
     def __init__(self):
         self.__resp = None
         try:
-            self.__resp = requests.get("https://some-random-api.ml/facts/bird")
+            self.__resp = requests.get("https://some-random-api.com/facts/bird")
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.APITimeout("API taken too long to respond!")
         if self.__resp.status_code != 200:
             if 'error' in self.__resp.json():
                 raise sra.exceptions.APIError(self.__resp.json()['error'])
             else:
                 raise sra.exceptions.APIError(
@@ -36,15 +36,15 @@
 
     :raise APITimeout: API taken too long to respond!
     :raise APIError: Error Returned by API
     """
     def __init__(self):
         self.__resp = None
         try:
-            self.__resp = requests.get("https://some-random-api.ml/facts/cat")
+            self.__resp = requests.get("https://some-random-api.com/facts/cat")
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.APITimeout("API taken too long to respond!")
         if self.__resp.status_code != 200:
             if 'error' in self.__resp.json():
                 raise sra.exceptions.APIError(self.__resp.json()['error'])
             else:
                 raise sra.exceptions.APIError(
@@ -63,15 +63,15 @@
 
     :raise APITimeout: API taken too long to respond!
     :raise APIError: Error Returned by API
     """
     def __init__(self):
         self.__resp = None
         try:
-            self.__resp = requests.get("https://some-random-api.ml/facts/dog")
+            self.__resp = requests.get("https://some-random-api.com/facts/dog")
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.APITimeout("API taken too long to respond!")
         if self.__resp.status_code != 200:
             if 'error' in self.__resp.json():
                 raise sra.exceptions.APIError(self.__resp.json()['error'])
             else:
                 raise sra.exceptions.APIError(
@@ -90,15 +90,15 @@
 
     :raise APITimeout: API taken too long to respond!
     :raise APIError: Error Returned by API
     """
     def __init__(self):
         self.__resp = None
         try:
-            self.__resp = requests.get("https://some-random-api.ml/facts/fox")
+            self.__resp = requests.get("https://some-random-api.com/facts/fox")
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.APITimeout("API taken too long to respond!")
         if self.__resp.status_code != 200:
             if 'error' in self.__resp.json():
                 raise sra.exceptions.APIError(self.__resp.json()['error'])
             else:
                 raise sra.exceptions.APIError(
@@ -117,15 +117,15 @@
 
     :raise APITimeout: API taken too long to respond!
     :raise APIError: Error Returned by API
     """
     def __init__(self):
         self.__resp = None
         try:
-            self.__resp = requests.get("https://some-random-api.ml/facts/koala")
+            self.__resp = requests.get("https://some-random-api.com/facts/koala")
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.APITimeout("API taken too long to respond!")
         if self.__resp.status_code != 200:
             if 'error' in self.__resp.json():
                 raise sra.exceptions.APIError(self.__resp.json()['error'])
             else:
                 raise sra.exceptions.APIError(
@@ -144,15 +144,15 @@
 
     :raise APITimeout: API taken too long to respond!
     :raise APIError: Error Returned by API
     """
     def __init__(self):
         self.__resp = None
         try:
-            self.__resp = requests.get("https://some-random-api.ml/facts/panda")
+            self.__resp = requests.get("https://some-random-api.com/facts/panda")
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.APITimeout("API taken too long to respond!")
         if self.__resp.status_code != 200:
             if 'error' in self.__resp.json():
                 raise sra.exceptions.APIError(self.__resp.json()['error'])
             else:
                 raise sra.exceptions.APIError(
```

### Comparing `sra-pylib-1.4.1/sra/image.py` & `sra-pylib-1.4.2/sra/image.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     Returns a random Image Link of a Bird by attributes
 
 
     :raise APITimeout: API taken too long to respond!
     :raise APIError: Error Returned by API
     """
     try:
-        __resp = requests.get("https://some-random-api.ml/img/bird")
+        __resp = requests.get("https://some-random-api.com/img/bird")
     except requests.exceptions.ConnectionError:
         raise sra.exceptions.APITimeout("API taken too long to respond!")
     if __resp.status_code != 200:
         if 'error' in __resp.json():
             raise sra.exceptions.APIError(__resp.json()['error'])
         else:
             raise sra.exceptions.APIError(
@@ -64,15 +64,15 @@
     Returns a random Image Link of a Cat by attributes
 
 
     :raise APITimeout: API taken too long to respond!
     :raise APIError: Error Returned by API
     """
     try:
-        __resp = requests.get("https://some-random-api.ml/img/cat")
+        __resp = requests.get("https://some-random-api.com/img/cat")
     except requests.exceptions.ConnectionError:
         raise sra.exceptions.APITimeout("API taken too long to respond!")
     if __resp.status_code != 200:
         if 'error' in __resp.json():
             raise sra.exceptions.APIError(__resp.json()['error'])
         else:
             raise sra.exceptions.APIError(
@@ -121,15 +121,15 @@
     Returns a random Image Link of a Dog by attributes
 
 
     :raise APITimeout: API taken too long to respond!
     :raise APIError: Error Returned by API
     """
     try:
-        __resp = requests.get("https://some-random-api.ml/img/dog")
+        __resp = requests.get("https://some-random-api.com/img/dog")
     except requests.exceptions.ConnectionError:
         raise sra.exceptions.APITimeout("API taken too long to respond!")
     if __resp.status_code != 200:
         if 'error' in __resp.json():
             raise sra.exceptions.APIError(__resp.json()['error'])
         else:
             raise sra.exceptions.APIError(
@@ -178,15 +178,15 @@
     Returns a random Image Link of a Fox by attributes
 
 
     :raise APITimeout: API taken too long to respond!
     :raise APIError: Error Returned by API
     """
     try:
-        __resp = requests.get("https://some-random-api.ml/img/fox")
+        __resp = requests.get("https://some-random-api.com/img/fox")
     except requests.exceptions.ConnectionError:
         raise sra.exceptions.APITimeout("API taken too long to respond!")
     if __resp.status_code != 200:
         if 'error' in __resp.json():
             raise sra.exceptions.APIError(__resp.json()['error'])
         else:
             raise sra.exceptions.APIError(
@@ -235,15 +235,15 @@
     Returns a random Image Link of a Kangaroo by attributes
 
 
     :raise APITimeout: API taken too long to respond!
     :raise APIError: Error Returned by API
     """
     try:
-        __resp = requests.get("https://some-random-api.ml/img/kangaroo")
+        __resp = requests.get("https://some-random-api.com/img/kangaroo")
     except requests.exceptions.ConnectionError:
         raise sra.exceptions.APITimeout("API taken too long to respond!")
     if __resp.status_code != 200:
         if 'error' in __resp.json():
             raise sra.exceptions.APIError(__resp.json()['error'])
         else:
             raise sra.exceptions.APIError(
@@ -292,15 +292,15 @@
     Returns a random Image Link of a Koala by attributes
 
 
     :raise APITimeout: API taken too long to respond!
     :raise APIError: Error Returned by API
     """
     try:
-        __resp = requests.get("https://some-random-api.ml/img/koala")
+        __resp = requests.get("https://some-random-api.com/img/koala")
     except requests.exceptions.ConnectionError:
         raise sra.exceptions.APITimeout("API taken too long to respond!")
     if __resp.status_code != 200:
         if 'error' in __resp.json():
             raise sra.exceptions.APIError(__resp.json()['error'])
         else:
             raise sra.exceptions.APIError(
@@ -349,15 +349,15 @@
     Returns a random Image Link of a Panda by attributes
 
 
     :raise APITimeout: API taken too long to respond!
     :raise APIError: Error Returned by API
     """
     try:
-        __resp = requests.get("https://some-random-api.ml/img/panda")
+        __resp = requests.get("https://some-random-api.com/img/panda")
     except requests.exceptions.ConnectionError:
         raise sra.exceptions.APITimeout("API taken too long to respond!")
     if __resp.status_code != 200:
         if 'error' in __resp.json():
             raise sra.exceptions.APIError(__resp.json()['error'])
         else:
             raise sra.exceptions.APIError(
@@ -406,15 +406,15 @@
     Returns a random Image Link of a Pikachu by attributes
 
 
     :raise APITimeout: API taken too long to respond!
     :raise APIError: Error Returned by API
     """
     try:
-        __resp = requests.get("https://some-random-api.ml/img/pikachu")
+        __resp = requests.get("https://some-random-api.com/img/pikachu")
     except requests.exceptions.ConnectionError:
         raise sra.exceptions.APITimeout("API taken too long to respond!")
     if __resp.status_code != 200:
         if 'error' in __resp.json():
             raise sra.exceptions.APIError(__resp.json()['error'])
         else:
             raise sra.exceptions.APIError(
@@ -463,15 +463,15 @@
     Returns a random Image Link of a Raccoon by attributes
 
 
     :raise APITimeout: API taken too long to respond!
     :raise APIError: Error Returned by API
     """
     try:
-        __resp = requests.get("https://some-random-api.ml/img/raccoon")
+        __resp = requests.get("https://some-random-api.com/img/raccoon")
     except requests.exceptions.ConnectionError:
         raise sra.exceptions.APITimeout("API taken too long to respond!")
     if __resp.status_code != 200:
         if 'error' in __resp.json():
             raise sra.exceptions.APIError(__resp.json()['error'])
         else:
             raise sra.exceptions.APIError(
@@ -520,15 +520,15 @@
     Returns a random Image Link of a Red Panda by attributes
 
 
     :raise APITimeout: API taken too long to respond!
     :raise APIError: Error Returned by API
     """
     try:
-        __resp = requests.get("https://some-random-api.ml/img/red_panda")
+        __resp = requests.get("https://some-random-api.com/img/red_panda")
     except requests.exceptions.ConnectionError:
         raise sra.exceptions.APITimeout("API taken too long to respond!")
     if __resp.status_code != 200:
         if 'error' in __resp.json():
             raise sra.exceptions.APIError(__resp.json()['error'])
         else:
             raise sra.exceptions.APIError(
@@ -577,15 +577,15 @@
     Returns a random Image Link of a Whale by attributes
 
 
     :raise APITimeout: API taken too long to respond!
     :raise APIError: Error Returned by API
     """
     try:
-        __resp = requests.get("https://some-random-api.ml/img/whale")
+        __resp = requests.get("https://some-random-api.com/img/whale")
     except requests.exceptions.ConnectionError:
         raise sra.exceptions.APITimeout("API taken too long to respond!")
     if __resp.status_code != 200:
         if 'error' in __resp.json():
             raise sra.exceptions.APIError(__resp.json()['error'])
         else:
             raise sra.exceptions.APIError(
```

### Comparing `sra-pylib-1.4.1/sra/others.py` & `sra-pylib-1.4.2/sra/others.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         :param text: The Human Readable text
         :return: str
         :raise APITimeout: API taken too long to respond!
         :raise APIError: Error Returned by API
         """
 
         try:
-            __resp = requests.get(f"https://some-random-api.ml/base64?encode={urllib.parse.quote_plus(text)}")
+            __resp = requests.get(f"https://some-random-api.com/base64?encode={urllib.parse.quote_plus(text)}")
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.APITimeout("API taken too long to respond!")
         if __resp.status_code != 200:
             try:
                 __resp = __resp.json()
                 if 'error' in __resp:
                     raise sra.exceptions.APIError(__resp['error'])
@@ -46,15 +46,15 @@
         :param base64: The Base64 Encoded Text
         :return: str
         :raise APITimeout: API taken too long to respond!
         :raise APIError: Error Returned by API
         """
 
         try:
-            __resp = requests.get(f"https://some-random-api.ml/base64?decode={urllib.parse.quote_plus(base64)}")
+            __resp = requests.get(f"https://some-random-api.com/base64?decode={urllib.parse.quote_plus(base64)}")
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.APITimeout("API taken too long to respond!")
         if __resp.status_code != 200:
             try:
                 __resp = __resp.json()
                 if 'error' in __resp:
                     raise sra.exceptions.APIError(__resp['error'])
@@ -80,15 +80,15 @@
         :param text: The Human Readable text
         :return: str
         :raise APITimeout: API taken too long to respond!
         :raise APIError: Error Returned by API
         """
 
         try:
-            __resp = requests.get(f"https://some-random-api.ml/binary?encode={urllib.parse.quote_plus(text)}")
+            __resp = requests.get(f"https://some-random-api.com/binary?encode={urllib.parse.quote_plus(text)}")
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.APITimeout("API taken too long to respond!")
         if __resp.status_code != 200:
             try:
                 __resp = __resp.json()
                 if 'error' in __resp:
                     raise sra.exceptions.APIError(__resp['error'])
@@ -108,15 +108,15 @@
         :param binary: The Binary Code
         :return: str
         :raise APITimeout: API taken too long to respond!
         :raise APIError: Error Returned by API
         """
 
         try:
-            __resp = requests.get(f"https://some-random-api.ml/binary?decode={urllib.parse.quote_plus(binary)}")
+            __resp = requests.get(f"https://some-random-api.com/binary?decode={urllib.parse.quote_plus(binary)}")
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.APITimeout("API taken too long to respond!")
         if __resp.status_code != 200:
             try:
                 __resp = __resp.json()
                 if 'error' in __resp:
                     raise sra.exceptions.APIError(__resp['error'])
@@ -137,15 +137,15 @@
     :return: str
     :raise APITimeout: API taken too long to respond!
     :raise APIError: Error Returned by API
     """
     def __init__(self, id: str = None):
         self.__resp = None
         try:
-            self.__resp = requests.get(f"https://some-random-api.ml/bottoken?id={urllib.parse.quote_plus(id)}")
+            self.__resp = requests.get(f"https://some-random-api.com/bottoken?id={urllib.parse.quote_plus(id)}")
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.APITimeout("API taken too long to respond!")
         if self.__resp.status_code != 200:
             if 'error' in self.__resp.json():
                 raise sra.exceptions.APIError(self.__resp.json()['error'])
             else:
                 raise sra.exceptions.APIError(
@@ -164,15 +164,15 @@
     :return: str
     :raise APITimeout: API taken too long to respond!
     :raise APIError: Error Returned by API
     """
     def __init__(self, word: str):
         self.__resp = None
         try:
-            self.__resp = requests.get(f"https://some-random-api.ml/dictionary?word={urllib.parse.quote_plus(word)}")
+            self.__resp = requests.get(f"https://some-random-api.com/dictionary?word={urllib.parse.quote_plus(word)}")
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.APITimeout("API taken too long to respond!")
         if self.__resp.status_code != 200:
             if 'error' in self.__resp.json():
                 raise sra.exceptions.APIError(self.__resp.json()['error'])
             else:
                 raise sra.exceptions.APIError(
@@ -190,15 +190,15 @@
     :return: str
     :raise APITimeout: API taken too long to respond!
     :raise APIError: Error Returned by API
     """
     def __init__(self):
         self.__resp = None
         try:
-            self.__resp = requests.get(f"https://some-random-api.ml/joke")
+            self.__resp = requests.get(f"https://some-random-api.com/joke")
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.APITimeout("API taken too long to respond!")
         if self.__resp.status_code != 200:
             if 'error' in self.__resp.json():
                 raise sra.exceptions.APIError(self.__resp.json()['error'])
             else:
                 raise sra.exceptions.APIError(
@@ -226,15 +226,15 @@
         """
         self.title, self.author, self.lyrics, self.thumbnail, self.link, self.disclaimer, self.raw = self.__search(name)
         self.structured = self.__structured(name)
 
     @staticmethod
     def __search(name: str):
         try:
-            __resp = requests.get(f"https://some-random-api.ml/others/lyrics?title={name}")
+            __resp = requests.get(f"https://some-random-api.com/others/lyrics?title={name}")
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.APITimeout("API taken too long to respond!")
         if __resp.status_code != 200:
             if 'error' in __resp.json():
                 raise sra.exceptions.APIError(__resp.json()['error'])
             else:
                 raise sra.exceptions.APIError(
```

### Comparing `sra-pylib-1.4.1/sra/pokemon.py` & `sra-pylib-1.4.2/sra/pokemon.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         """
         self.id, self.name, self.generation, self.effects, self.description, self.pokemons, self.descriptions, self.raw = self.__getability(
             ability)
 
     @staticmethod
     def __getability(ability):
         try:
-            __resp = requests.get(f"https://some-random-api.ml/pokemon/abilities?ability={urllib.parse.quote_plus(ability)}")
+            __resp = requests.get(f"https://some-random-api.com/pokemon/abilities?ability={urllib.parse.quote_plus(ability)}")
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.APITimeout("API taken too long to respond!")
         if __resp.status_code != 200:
             if 'error' in __resp.json():
                 raise sra.exceptions.APIError(__resp.json()['error'])
             else:
                 raise sra.exceptions.APIError(
@@ -62,15 +62,15 @@
         """
         self.id, self.name, self.effects, self.cost, self.attributes, self.category, self.sprite, self.descriptions, self.raw = self.__getitem(
             item)
 
     @staticmethod
     def __getitem(item):
         try:
-            __resp = requests.get(f"https://some-random-api.ml/pokemon/items?item={urllib.parse.quote_plus(item)}")
+            __resp = requests.get(f"https://some-random-api.com/pokemon/items?item={urllib.parse.quote_plus(item)}")
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.APITimeout("API taken too long to respond!")
         if __resp.status_code != 200:
             if 'error' in __resp.json():
                 raise sra.exceptions.APIError(__resp.json()['error'])
             else:
                 raise sra.exceptions.APIError(
@@ -103,15 +103,15 @@
         """
         self.id, self.name, self.generation, self.effects, self.type, self.category, self.contest, self.pp, self.power, self.accuracy, self.priority, self.pokemon, self.descriptions, self.raw = self.__getmove(
             move)
 
     @staticmethod
     def __getmove(move):
         try:
-            __resp = requests.get(f"https://some-random-api.ml/pokemon/moves?move={urllib.parse.quote_plus(move)}")
+            __resp = requests.get(f"https://some-random-api.com/pokemon/moves?move={urllib.parse.quote_plus(move)}")
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.APITimeout("API taken too long to respond!")
         if __resp.status_code != 200:
             if 'error' in __resp.json():
                 raise sra.exceptions.APIError(__resp.json()['error'])
             else:
                 raise sra.exceptions.APIError(
@@ -148,15 +148,15 @@
         :raise APIError: Error Returned by API
         """
         self.name, self.id, self.type, self.species, self.abilities, self.height, self.weight, self.base_experience, self.gender, self.egg_groups, self.stats, self.family, self.sprites, self.description, self.generation, self.raw = self.__getpokemon(
             pokemon)
 
     def __getpokemon(self, pokemon):
         try:
-            __resp = requests.get(f"https://some-random-api.ml/pokemon/pokedex?pokemon={urllib.parse.quote_plus(pokemon)}")
+            __resp = requests.get(f"https://some-random-api.com/pokemon/pokedex?pokemon={urllib.parse.quote_plus(pokemon)}")
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.APITimeout("API taken too long to respond!")
         if __resp.status_code != 200:
             if 'error' in __resp.json():
                 raise sra.exceptions.APIError(__resp.json()['error'])
             else:
                 raise sra.exceptions.APIError(
```

### Comparing `sra-pylib-1.4.1/sra/welcome.py` & `sra-pylib-1.4.2/sra/welcome.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 
             if not validFormat:
                 raise sra.exceptions.InvalidFileFormat(
                     'Invalid File Format given. File Format must be ".png", ".jpg" or "jpeg"!')
         path = name
 
         try:
-            __resp = requests.get(f"https://some-random-api.ml/welcome/img/{str(template)}/{str(background)}?type={type}&username={username}&avatar={avatar_url}&discriminator={discriminator}&guildName={guildName}&memberCount={memberCount}&textcolor={textcolor}&key={key}{'&font=' + str(font) if font != None else ''}", stream=True)
+            __resp = requests.get(f"https://some-random-api.com/welcome/img/{str(template)}/{str(background)}?type={type}&username={username}&avatar={avatar_url}&discriminator={discriminator}&guildName={guildName}&memberCount={memberCount}&textcolor={textcolor}&key={key}{'&font=' + str(font) if font != None else ''}", stream=True)
         except requests.exceptions.ConnectionError:
             raise sra.exceptions.ImageRetrieveError("Unable to Load the Image!")
         if __resp.status_code == 200:
             with open(path, 'wb') as f:
                 __resp.raw.decode_content = True
                 shutil.copyfileobj(__resp.raw, f)
             return True
```

### Comparing `sra-pylib-1.4.1/sra_pylib.egg-info/PKG-INFO` & `sra-pylib-1.4.2/sra_pylib.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sra-pylib
-Version: 1.4.1
+Version: 1.4.2
 Summary: A Wrapper of some-random-api for Python
 Home-page: https://github.com/Sayad-Uddin-Tahsin/sra-pylib
 Author: Sayad Uddin Tahsin
 Author-email: mr.pluto012@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/Sayad-Uddin-Tahsin/sra-pylib/wiki
 Project-URL: Bug Tracker, https://github.com/Sayad-Uddin-Tahsin/sra-pylib/issues
@@ -20,24 +20,28 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # sra-pylib
-`sra-pylib` is a Python wrapper for [some-random-api](https://some-random-api.ml).
+`sra-pylib` is a Python wrapper for [some-random-api](https://some-random-api.com).
 
 ```python
 import sra
+from sra import animal
 
->>> print(sra.animal.Panda.image_link)  # Prints a Panda Image link
+# Create a new instance of the Panda class
+panda = animal.Panda()
+
+>>> print(panda.image_link)  # Prints a Panda Image link
 "https://i.imgur.com/YVLrUO9.jpg"
->>> print(sra.animal.Panda.fact)  # Prints a Panda Fact
-"Giant pandas have been driven out of the lowland areas where they used to live and now are found only in the Chinese provinces of Sichuan, Gansu, and Shaanxi. The forests in these provinces are very damp and rainy. In one year, a forest may receive up to 50 inches of rain and snow."
->>> sra.animal.Panda.save_image()  # Saves the Image
+>>> print(panda.fact)  # Prints a Panda Fact
+"From 1974-1989, half of the panda’s habitat in China’s Sichuan areas was destroyed by human activity."
+>>> panda.save_image("Cool Panda.png")  # Saves the Image
 ```
 With `sra-pylib`, you can easily access the various endpoints of `some-random-api` in your Python projects, making it a powerful tool for working with image, fact, and other types of data.
 
 <a href="https://pypi.org/project/sra-pylib"><img src="https://img.shields.io/pypi/status/sra-pylib?label=Status&logo=pypi&logoColor=ffffff" height=22></a>
 <a href="https://pypi.org/project/sra-pylib"><img src="https://img.shields.io/pypi/v/sra-pylib?label=PyPI Version&logo=pypi&logoColor=ffffff" height=22></a>
 <a href="https://app.fossa.com/projects/git%2Bgithub.com%2FSayad-Uddin-Tahsin%2Fsra-pylib?ref=badge_shield" alt="FOSSA Status"><img src="https://app.fossa.com/api/projects/git%2Bgithub.com%2FSayad-Uddin-Tahsin%2Fsra-pylib.svg?type=shield" height=22></a>
 <a href="https://python.org"><img src="https://img.shields.io/pypi/pyversions/sra-pylib?label=Python&logo=python&logoColor=ffdd54" height=22></a>
@@ -53,16 +57,30 @@
 `sra-pylib` is synced with some-random-api. It has all the Endpoints provided by some-random-api except the Premium ones.
 
 ## Documentation
 Full documentation for the sra-pylib module can be found on [Wiki](https://github.com/Sayad-Uddin-Tahsin/sra-pylib/wiki). The documentation includes detailed information on how to use the module, including examples and reference documentation for all classes and methods.
 
 If you have any questions or issues with the module, please refer to the documentation or submit a bug report on the [GitHub issues page](https://github.com/Sayad-Uddin-Tahsin/sra-pylib/issues).
 
+
+## Bug Report
+If you encounter any bugs while using sra-pylib, please report them by opening a new issue on the [GitHub repository](https://github.com/Sayad-Uddin-Tahsin/sra-pylib/issues). When reporting a bug, please include the following information:
+
+- A detailed description of the issue, including what you were trying to do when the bug occurred
+- The full traceback or error message, if applicable
+- Steps to reproduce the bug, if possible
+- Any additional information or context that might be relevant to the issue
+
+By reporting bugs, you can help improve the quality and reliability of sra-pylib for all user
+
+
 ## Cloning the Repository
-You also can install sra-pylib directly from Github, by using this pip command:
+You can easily clone this repository by executing the following command:
 ```console
-pip install git+https://github.com/Sayad-Uddin-Tahsin/sra-pylib.git
+git clone https://github.com/Sayad-Uddin-Tahsin/sra-pylib.git
 ```
-This will install the package directly from the repository.
+This will clone the whole repository in your computer.
+
+You can also download the repository as a `zip` file: [Download as zip](https://github.com/Sayad-Uddin-Tahsin/sra-pylib/archive/refs/heads/main.zip)
 
 ## License
 [![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2FSayad-Uddin-Tahsin%2Fsra-pylib.svg?type=large)](https://app.fossa.com/projects/git%2Bgithub.com%2FSayad-Uddin-Tahsin%2Fsra-pylib?ref=badge_large)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1,46 +1,55 @@
-Metadata-Version: 2.1 Name: sra-pylib Version: 1.4.1 Summary: A Wrapper of
+Metadata-Version: 2.1 Name: sra-pylib Version: 1.4.2 Summary: A Wrapper of
 some-random-api for Python Home-page: https://github.com/Sayad-Uddin-Tahsin/
 sra-pylib Author: Sayad Uddin Tahsin Author-email: mr.pluto012@gmail.com
 License: MIT Project-URL: Documentation, https://github.com/Sayad-Uddin-Tahsin/
 sra-pylib/wiki Project-URL: Bug Tracker, https://github.com/Sayad-Uddin-Tahsin/
 sra-pylib/issues Project-URL: PyPI, https://pypi.org/project/sra-pylib/
 Keywords: some-random-api,sra,api-wrapper,sra-pylib,sra-wrapper,tahsin-project
 Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-
 Python: >=3.7 Description-Content-Type: text/markdown License-File: LICENSE #
 sra-pylib `sra-pylib` is a Python wrapper for [some-random-api](https://some-
-random-api.ml). ```python import sra >>> print(sra.animal.Panda.image_link) #
-Prints a Panda Image link "https://i.imgur.com/YVLrUO9.jpg" >>> print
-(sra.animal.Panda.fact) # Prints a Panda Fact "Giant pandas have been driven
-out of the lowland areas where they used to live and now are found only in the
-Chinese provinces of Sichuan, Gansu, and Shaanxi. The forests in these
-provinces are very damp and rainy. In one year, a forest may receive up to 50
-inches of rain and snow." >>> sra.animal.Panda.save_image() # Saves the Image
-``` With `sra-pylib`, you can easily access the various endpoints of `some-
-random-api` in your Python projects, making it a powerful tool for working with
-image, fact, and other types of data. [https://img.shields.io/pypi/status/sra-
+random-api.com). ```python import sra from sra import animal # Create a new
+instance of the Panda class panda = animal.Panda() >>> print(panda.image_link)
+# Prints a Panda Image link "https://i.imgur.com/YVLrUO9.jpg" >>> print
+(panda.fact) # Prints a Panda Fact "From 1974-1989, half of the pandaâs
+habitat in Chinaâs Sichuan areas was destroyed by human activity." >>>
+panda.save_image("Cool Panda.png") # Saves the Image ``` With `sra-pylib`, you
+can easily access the various endpoints of `some-random-api` in your Python
+projects, making it a powerful tool for working with image, fact, and other
+types of data. [https://img.shields.io/pypi/status/sra-
 pylib?label=Status&logo=pypi&logoColor=ffffff] [https://img.shields.io/pypi/v/
 sra-pylib?label=PyPI_Version&logo=pypi&logoColor=ffffff] [https://
 app.fossa.com/api/projects/git%2Bgithub.com%2FSayad-Uddin-Tahsin%2Fsra-
 pylib.svg?type=shield] [https://img.shields.io/pypi/pyversions/sra-
 pylib?label=Python&logo=python&logoColor=ffdd54] ## Installation You can
 install `sra-pylib` using `pip`: ```console python -m pip install sra-pylib ```
 `sra-pylib` requires Python 3.7 or later. ## Endpoints `sra-pylib` is synced
 with some-random-api. It has all the Endpoints provided by some-random-api
 except the Premium ones. ## Documentation Full documentation for the sra-pylib
 module can be found on [Wiki](https://github.com/Sayad-Uddin-Tahsin/sra-pylib/
 wiki). The documentation includes detailed information on how to use the
 module, including examples and reference documentation for all classes and
 methods. If you have any questions or issues with the module, please refer to
 the documentation or submit a bug report on the [GitHub issues page](https://
-github.com/Sayad-Uddin-Tahsin/sra-pylib/issues). ## Cloning the Repository You
-also can install sra-pylib directly from Github, by using this pip command:
-```console pip install git+https://github.com/Sayad-Uddin-Tahsin/sra-pylib.git
-``` This will install the package directly from the repository. ## License [!
-[FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2FSayad-
-Uddin-Tahsin%2Fsra-pylib.svg?type=large)](https://app.fossa.com/projects/
+github.com/Sayad-Uddin-Tahsin/sra-pylib/issues). ## Bug Report If you encounter
+any bugs while using sra-pylib, please report them by opening a new issue on
+the [GitHub repository](https://github.com/Sayad-Uddin-Tahsin/sra-pylib/
+issues). When reporting a bug, please include the following information: - A
+detailed description of the issue, including what you were trying to do when
+the bug occurred - The full traceback or error message, if applicable - Steps
+to reproduce the bug, if possible - Any additional information or context that
+might be relevant to the issue By reporting bugs, you can help improve the
+quality and reliability of sra-pylib for all user ## Cloning the Repository You
+can easily clone this repository by executing the following command: ```console
+git clone https://github.com/Sayad-Uddin-Tahsin/sra-pylib.git ``` This will
+clone the whole repository in your computer. You can also download the
+repository as a `zip` file: [Download as zip](https://github.com/Sayad-Uddin-
+Tahsin/sra-pylib/archive/refs/heads/main.zip) ## License [![FOSSA Status]
+(https://app.fossa.com/api/projects/git%2Bgithub.com%2FSayad-Uddin-
+Tahsin%2Fsra-pylib.svg?type=large)](https://app.fossa.com/projects/
 git%2Bgithub.com%2FSayad-Uddin-Tahsin%2Fsra-pylib?ref=badge_large)
```

