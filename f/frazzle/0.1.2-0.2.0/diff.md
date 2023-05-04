# Comparing `tmp/frazzle-0.1.2.tar.gz` & `tmp/frazzle-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frazzle-0.1.2.tar", last modified: Thu May  4 16:06:49 2023, max compression
+gzip compressed data, was "frazzle-0.2.0.tar", max compression
```

## Comparing `frazzle-0.1.2.tar` & `frazzle-0.2.0.tar`

### file list

```diff
@@ -1,36 +1,4 @@
-drwxrwxrwx   0        0        0        0 2023-05-04 16:06:49.688890 frazzle-0.1.2/
--rw-rw-rw-   0        0        0      342 2023-05-03 05:04:31.000000 frazzle-0.1.2/LICENSE
--rw-rw-rw-   0        0        0       77 2023-05-04 16:06:49.688388 frazzle-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      509 2023-05-04 16:00:43.000000 frazzle-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-04 16:06:49.664889 frazzle-0.1.2/obf-dist/
-drwxrwxrwx   0        0        0        0 2023-05-04 16:06:49.671390 frazzle-0.1.2/obf-dist/frazzle/
--rw-rw-rw-   0        0        0      753 2023-05-04 16:06:38.000000 frazzle-0.1.2/obf-dist/frazzle/__init__.py
--rw-rw-rw-   0        0        0     1989 2023-05-04 16:06:38.000000 frazzle-0.1.2/obf-dist/frazzle/__main__.py
--rw-rw-rw-   0        0        0     6208 2023-05-04 16:06:38.000000 frazzle-0.1.2/obf-dist/frazzle/cli.py
--rw-rw-rw-   0        0        0    15116 2023-05-04 16:06:38.000000 frazzle-0.1.2/obf-dist/frazzle/course.py
-drwxrwxrwx   0        0        0        0 2023-05-04 16:06:49.683388 frazzle-0.1.2/obf-dist/frazzle/cs257/
--rw-rw-rw-   0        0        0     2313 2023-05-04 16:06:38.000000 frazzle-0.1.2/obf-dist/frazzle/cs257/__init__.py
--rw-rw-rw-   0        0        0    44232 2023-05-04 16:06:38.000000 frazzle-0.1.2/obf-dist/frazzle/cs257/goblin.py
--rw-rw-rw-   0        0        0    14430 2023-05-04 16:06:38.000000 frazzle-0.1.2/obf-dist/frazzle/cs257/hello.py
--rw-rw-rw-   0        0        0    24597 2023-05-04 16:06:38.000000 frazzle-0.1.2/obf-dist/frazzle/cs257/hilo.py
-drwxrwxrwx   0        0        0        0 2023-05-04 16:06:49.685388 frazzle-0.1.2/obf-dist/frazzle/cs452/
--rw-rw-rw-   0        0        0     2587 2023-05-04 16:06:38.000000 frazzle-0.1.2/obf-dist/frazzle/cs452/__init__.py
--rw-rw-rw-   0        0        0    44800 2023-05-04 16:06:38.000000 frazzle-0.1.2/obf-dist/frazzle/cs452/lab2.py
--rw-rw-rw-   0        0        0    16481 2023-05-04 16:06:38.000000 frazzle-0.1.2/obf-dist/frazzle/cs452/lab6.py
-drwxrwxrwx   0        0        0        0 2023-05-04 16:06:49.687388 frazzle-0.1.2/obf-dist/frazzle/cs459/
--rw-rw-rw-   0        0        0     4215 2023-05-04 16:06:38.000000 frazzle-0.1.2/obf-dist/frazzle/cs459/__init__.py
--rw-rw-rw-   0        0        0    33058 2023-05-04 16:06:38.000000 frazzle-0.1.2/obf-dist/frazzle/cs459/fatcat.py
--rw-rw-rw-   0        0        0    39300 2023-05-04 16:06:38.000000 frazzle-0.1.2/obf-dist/frazzle/cs459/ps.py
--rw-rw-rw-   0        0        0    29250 2023-05-04 16:06:38.000000 frazzle-0.1.2/obf-dist/frazzle/hint.py
--rw-rw-rw-   0        0        0     6134 2023-05-04 16:06:38.000000 frazzle-0.1.2/obf-dist/frazzle/lab.py
--rw-rw-rw-   0        0        0     6962 2023-05-04 16:06:38.000000 frazzle-0.1.2/obf-dist/frazzle/part.py
-drwxrwxrwx   0        0        0        0 2023-05-04 16:06:49.680891 frazzle-0.1.2/obf-dist/frazzle.egg-info/
--rw-rw-rw-   0        0        0       77 2023-05-04 16:06:49.000000 frazzle-0.1.2/obf-dist/frazzle.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      753 2023-05-04 16:06:49.000000 frazzle-0.1.2/obf-dist/frazzle.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-04 16:06:49.000000 frazzle-0.1.2/obf-dist/frazzle.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2023-05-04 16:06:49.000000 frazzle-0.1.2/obf-dist/frazzle.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-04 16:06:49.687888 frazzle-0.1.2/obf-dist/pyarmor_runtime_005075/
--rw-rw-rw-   0        0        0      101 2023-05-04 16:06:38.000000 frazzle-0.1.2/obf-dist/pyarmor_runtime_005075/__init__.py
--rw-rw-rw-   0        0        0      755 2023-05-04 16:06:28.000000 frazzle-0.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-04 16:06:49.688890 frazzle-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      330 2023-05-04 16:06:20.000000 frazzle-0.1.2/setup.py
+-rw-r--r--   0        0        0     1134 2023-05-04 16:44:44.712519 frazzle-0.2.0/frazzle/client.py
+-rw-r--r--   0        0        0      492 2023-05-04 16:43:57.169326 frazzle-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       15 2023-05-04 16:45:06.940554 frazzle-0.2.0/README.md
+-rw-r--r--   0        0        0      727 1970-01-01 00:00:00.000000 frazzle-0.2.0/PKG-INFO
```

