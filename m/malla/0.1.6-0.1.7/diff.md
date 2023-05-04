# Comparing `tmp/malla-0.1.6.tar.gz` & `tmp/malla-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "malla-0.1.6.tar", max compression
+gzip compressed data, was "malla-0.1.7.tar", max compression
```

## Comparing `malla-0.1.6.tar` & `malla-0.1.7.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      526 2023-04-29 16:35:40.386927 malla-0.1.6/README.md
--rw-r--r--   0        0        0        0 2023-04-25 21:01:58.416728 malla-0.1.6/malla/__init__.py
--rw-r--r--   0        0        0     6064 2023-05-03 19:59:00.090070 malla-0.1.6/malla/directed_edge.py
--rw-r--r--   0        0        0      717 2023-04-29 16:59:32.283620 malla-0.1.6/malla/off.py
--rw-r--r--   0        0        0      266 2023-05-03 19:59:20.810070 malla-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      862 1970-01-01 00:00:00.000000 malla-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0      526 2023-04-29 16:35:40.386927 malla-0.1.7/README.md
+-rw-r--r--   0        0        0        0 2023-04-25 21:01:58.416728 malla-0.1.7/malla/__init__.py
+-rw-r--r--   0        0        0     6089 2023-05-04 19:42:06.026765 malla-0.1.7/malla/directed_edge.py
+-rw-r--r--   0        0        0      717 2023-04-29 16:59:32.283620 malla-0.1.7/malla/off.py
+-rw-r--r--   0        0        0      266 2023-05-04 19:45:04.296769 malla-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      862 1970-01-01 00:00:00.000000 malla-0.1.7/PKG-INFO
```

### Comparing `malla-0.1.6/README.md` & `malla-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `malla-0.1.6/malla/directed_edge.py` & `malla-0.1.7/malla/directed_edge.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,18 +116,19 @@
     def number_of_vertices(self) -> int:
         return len(self._vertices)
 
     def number_of_faces(self) -> int:
         return int(len(self.half_edges)/3)
 
     def vertex_neighbors(self, v: int) -> Generator[int, None, None]:
+        h = -1
         for he in self.vertex_halfedges(v):
             yield self.half_edge(he).dst
             h = he
-        if self.half_edge(self.prev(h)).mate == -1: #bordo
+        if h > -1 and self.half_edge(self.prev(h)).mate == -1: #bordo
             yield self.half_edge(self.next(h)).dst
 
     def vertex_halfedges(self, v: int) -> Generator[int, None, None]:
         he = self.vertex(v).half_edge
         if he != -1:
             hn = he
             while True:
@@ -196,8 +197,7 @@
                     if mate != -1:
                         current = self.next(mate)
                     else:
                         self._vertices[v].half_edge = current
                         current = first
         else:
             print("Warning : vetex %d is isolated." % v)
-
```

### Comparing `malla-0.1.6/malla/off.py` & `malla-0.1.7/malla/off.py`

 * *Files identical despite different names*

### Comparing `malla-0.1.6/PKG-INFO` & `malla-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: malla
-Version: 0.1.6
+Version: 0.1.7
 Summary: 
 Author: Dimas Martínez
 Author-email: dimas@ufam.edu.br
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

