# Comparing `tmp/emdfile-0.0.5.tar.gz` & `tmp/emdfile-0.0.6.tar.gz`

## Comparing `emdfile-0.0.5.tar` & `emdfile-0.0.6.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 emdfile-0.0.5/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 emdfile-0.0.5/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 emdfile-0.0.5/.pytest_cache/README.md
--rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 emdfile-0.0.5/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 emdfile-0.0.5/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 emdfile-0.0.5/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 emdfile-0.0.5/src/emdfile/__init__.py
--rw-r--r--   0        0        0    10788 2020-02-02 00:00:00.000000 emdfile-0.0.5/src/emdfile/read.py
--rw-r--r--   0        0        0     2413 2020-02-02 00:00:00.000000 emdfile-0.0.5/src/emdfile/tqdmnd.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 emdfile-0.0.5/src/emdfile/version.py
--rw-r--r--   0        0        0    31055 2020-02-02 00:00:00.000000 emdfile-0.0.5/src/emdfile/write.py
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 emdfile-0.0.5/src/emdfile/classes/__init__.py
--rw-r--r--   0        0        0    22633 2020-02-02 00:00:00.000000 emdfile-0.0.5/src/emdfile/classes/array.py
--rw-r--r--   0        0        0     2715 2020-02-02 00:00:00.000000 emdfile-0.0.5/src/emdfile/classes/custom.py
--rw-r--r--   0        0        0    10249 2020-02-02 00:00:00.000000 emdfile-0.0.5/src/emdfile/classes/metadata.py
--rw-r--r--   0        0        0     6671 2020-02-02 00:00:00.000000 emdfile-0.0.5/src/emdfile/classes/pointlist.py
--rw-r--r--   0        0        0     6155 2020-02-02 00:00:00.000000 emdfile-0.0.5/src/emdfile/classes/pointlistarray.py
--rw-r--r--   0        0        0    23786 2020-02-02 00:00:00.000000 emdfile-0.0.5/src/emdfile/classes/tree.py
--rw-r--r--   0        0        0     2240 2020-02-02 00:00:00.000000 emdfile-0.0.5/src/emdfile/classes/utils.py
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 emdfile-0.0.5/test/clear_h5_files.py
--rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 emdfile-0.0.5/test/test_base_classes.py
--rw-r--r--   0        0        0     3178 2020-02-02 00:00:00.000000 emdfile-0.0.5/test/test_emd.py
--rw-r--r--   0        0        0     3083 2020-02-02 00:00:00.000000 emdfile-0.0.5/test/test_header.py
--rw-r--r--   0        0        0    28996 2020-02-02 00:00:00.000000 emdfile-0.0.5/test/test_tree.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 emdfile-0.0.5/test/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 emdfile-0.0.5/test/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 emdfile-0.0.5/test/.pytest_cache/README.md
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 emdfile-0.0.5/test/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 emdfile-0.0.5/test/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 emdfile-0.0.5/test/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0   384837 2020-02-02 00:00:00.000000 emdfile-0.0.5/tutorials/emdfile_intro_example.ipynb
--rw-r--r--   0        0        0   167826 2020-02-02 00:00:00.000000 emdfile-0.0.5/tutorials/emdfile_package_walkthrough.ipynb
--rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 emdfile-0.0.5/tutorials/test_custom_classes.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 emdfile-0.0.5/tutorials/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 emdfile-0.0.5/tutorials/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 emdfile-0.0.5/tutorials/.pytest_cache/README.md
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 emdfile-0.0.5/tutorials/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 emdfile-0.0.5/tutorials/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 emdfile-0.0.5/tutorials/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0    81358 2020-02-02 00:00:00.000000 emdfile-0.0.5/tutorials/pngs/node.png
--rw-r--r--   0        0        0    41590 2020-02-02 00:00:00.000000 emdfile-0.0.5/tutorials/pngs/tree.png
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 emdfile-0.0.5/tutorials/sample_custom_emd_classes/__init__.py
--rw-r--r--   0        0        0     2924 2020-02-02 00:00:00.000000 emdfile-0.0.5/tutorials/sample_custom_emd_classes/my_custom_classes.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 emdfile-0.0.5/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 emdfile-0.0.5/LICENSE
--rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 emdfile-0.0.5/README.md
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 emdfile-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 emdfile-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 emdfile-0.0.6/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 emdfile-0.0.6/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 emdfile-0.0.6/.pytest_cache/README.md
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 emdfile-0.0.6/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 emdfile-0.0.6/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 emdfile-0.0.6/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0      888 2020-02-02 00:00:00.000000 emdfile-0.0.6/src/emdfile/__init__.py
+-rw-r--r--   0        0        0    10788 2020-02-02 00:00:00.000000 emdfile-0.0.6/src/emdfile/read.py
+-rw-r--r--   0        0        0     2413 2020-02-02 00:00:00.000000 emdfile-0.0.6/src/emdfile/tqdmnd.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 emdfile-0.0.6/src/emdfile/version.py
+-rw-r--r--   0        0        0    31055 2020-02-02 00:00:00.000000 emdfile-0.0.6/src/emdfile/write.py
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 emdfile-0.0.6/src/emdfile/classes/__init__.py
+-rw-r--r--   0        0        0    22633 2020-02-02 00:00:00.000000 emdfile-0.0.6/src/emdfile/classes/array.py
+-rw-r--r--   0        0        0     2715 2020-02-02 00:00:00.000000 emdfile-0.0.6/src/emdfile/classes/custom.py
+-rw-r--r--   0        0        0    10249 2020-02-02 00:00:00.000000 emdfile-0.0.6/src/emdfile/classes/metadata.py
+-rw-r--r--   0        0        0     6671 2020-02-02 00:00:00.000000 emdfile-0.0.6/src/emdfile/classes/pointlist.py
+-rw-r--r--   0        0        0     6155 2020-02-02 00:00:00.000000 emdfile-0.0.6/src/emdfile/classes/pointlistarray.py
+-rw-r--r--   0        0        0    23911 2020-02-02 00:00:00.000000 emdfile-0.0.6/src/emdfile/classes/tree.py
+-rw-r--r--   0        0        0     2240 2020-02-02 00:00:00.000000 emdfile-0.0.6/src/emdfile/classes/utils.py
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 emdfile-0.0.6/test/clear_h5_files.py
+-rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 emdfile-0.0.6/test/test_base_classes.py
+-rw-r--r--   0        0        0     3178 2020-02-02 00:00:00.000000 emdfile-0.0.6/test/test_emd.py
+-rw-r--r--   0        0        0     3083 2020-02-02 00:00:00.000000 emdfile-0.0.6/test/test_header.py
+-rw-r--r--   0        0        0    28996 2020-02-02 00:00:00.000000 emdfile-0.0.6/test/test_tree.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 emdfile-0.0.6/test/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 emdfile-0.0.6/test/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 emdfile-0.0.6/test/.pytest_cache/README.md
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 emdfile-0.0.6/test/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 emdfile-0.0.6/test/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 emdfile-0.0.6/test/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0   384837 2020-02-02 00:00:00.000000 emdfile-0.0.6/tutorials/emdfile_intro_example.ipynb
+-rw-r--r--   0        0        0   167826 2020-02-02 00:00:00.000000 emdfile-0.0.6/tutorials/emdfile_package_walkthrough.ipynb
+-rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 emdfile-0.0.6/tutorials/test_custom_classes.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 emdfile-0.0.6/tutorials/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 emdfile-0.0.6/tutorials/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 emdfile-0.0.6/tutorials/.pytest_cache/README.md
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 emdfile-0.0.6/tutorials/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 emdfile-0.0.6/tutorials/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 emdfile-0.0.6/tutorials/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0    81358 2020-02-02 00:00:00.000000 emdfile-0.0.6/tutorials/pngs/node.png
+-rw-r--r--   0        0        0    41590 2020-02-02 00:00:00.000000 emdfile-0.0.6/tutorials/pngs/tree.png
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 emdfile-0.0.6/tutorials/sample_custom_emd_classes/__init__.py
+-rw-r--r--   0        0        0     2924 2020-02-02 00:00:00.000000 emdfile-0.0.6/tutorials/sample_custom_emd_classes/my_custom_classes.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 emdfile-0.0.6/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 emdfile-0.0.6/LICENSE
+-rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 emdfile-0.0.6/README.md
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 emdfile-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 emdfile-0.0.6/PKG-INFO
```

### Comparing `emdfile-0.0.5/.pytest_cache/v/cache/lastfailed` & `emdfile-0.0.6/.pytest_cache/v/cache/nodeids`

 * *Files 26% similar despite different names*

#### Pretty-printed

```diff
@@ -1,32 +1,37 @@
-{
-    "test/test_base_classes.py::test_Array": true,
-    "test/test_base_classes.py::test_Metadata": true,
-    "test/test_base_classes.py::test_Node": true,
-    "test/test_base_classes.py::test_PointList": true,
-    "test/test_base_classes.py::test_PointListArray": true,
-    "test/test_emd.py::TestEmd": true,
-    "test/test_emd.py::TestEmd::test_array": true,
-    "test/test_emd.py::TestEmd::test_array2": true,
-    "test/test_tree.py::TestTree": true,
-    "test/test_tree.py::TestTree::test_branchcut": true,
-    "test/test_tree.py::TestTree::test_branchcut_copy_metadata": true,
-    "test/test_tree.py::TestTree::test_branchcut_no_metadata": true,
-    "test/test_tree.py::TestTree::test_graft": true,
-    "test/test_tree.py::TestTree::test_graft2": true,
-    "test/test_tree.py::TestTree::test_graft3": true,
-    "test/test_tree.py::TestTree::test_nodes": true,
-    "test/test_tree.py::TestTree::test_structure": true,
-    "test/test_tree.py::TestTreeIO": true,
-    "test/test_tree.py::TestTreeIO::test_append_over_io": true,
-    "test/test_tree.py::TestTreeIO::test_append_to_io": true,
-    "test/test_tree.py::TestTreeIO::test_file_validity": true,
-    "test/test_tree.py::TestTreeIO::test_hdf5_group_paths": true,
-    "test/test_tree.py::TestTreeIO::test_single_node_io": true,
-    "test/test_tree.py::TestTreeIO::test_single_node_io_emdpath": true,
-    "test/test_tree.py::TestTreeIO::test_subtree_io": true,
-    "test/test_tree.py::TestTreeIO::test_subtree_noroot_io": true,
-    "test/test_tree.py::TestTreeIO::test_unrooted_node_io": true,
-    "test/test_tree.py::TestTreeIO::test_whole_tree_io": true,
-    "test/test_tree.py::TestTreeIO::test_whole_tree_io_treeIsFalse": true,
-    "tutorials/test_custom_class.py": true
-}
+[
+    "emd/test/test_base_classes.py::test_Array",
+    "emd/test/test_base_classes.py::test_Metadata",
+    "emd/test/test_base_classes.py::test_Node",
+    "emd/test/test_base_classes.py::test_PointList",
+    "emd/test/test_base_classes.py::test_PointListArray",
+    "emd/test/test_emd.py::TestEmd::test_array",
+    "emd/test/test_emd.py::TestEmd::test_array2",
+    "test/test_base_classes.py::test_Array",
+    "test/test_base_classes.py::test_Metadata",
+    "test/test_base_classes.py::test_Node",
+    "test/test_base_classes.py::test_PointList",
+    "test/test_base_classes.py::test_PointListArray",
+    "test/test_emd.py::TestEmd::test_array",
+    "test/test_emd.py::TestEmd::test_array2",
+    "test/test_header.py::TestHeader::test_header",
+    "test/test_header.py::TestHeader::test_header2",
+    "test/test_tree.py::TestTree::test_branchcut",
+    "test/test_tree.py::TestTree::test_branchcut_copy_metadata",
+    "test/test_tree.py::TestTree::test_branchcut_no_metadata",
+    "test/test_tree.py::TestTree::test_graft",
+    "test/test_tree.py::TestTree::test_graft2",
+    "test/test_tree.py::TestTree::test_graft3",
+    "test/test_tree.py::TestTree::test_nodes",
+    "test/test_tree.py::TestTree::test_structure",
+    "test/test_tree.py::TestTreeIO::test_append_over_io",
+    "test/test_tree.py::TestTreeIO::test_append_to_io",
+    "test/test_tree.py::TestTreeIO::test_file_validity",
+    "test/test_tree.py::TestTreeIO::test_hdf5_group_paths",
+    "test/test_tree.py::TestTreeIO::test_single_node_io",
+    "test/test_tree.py::TestTreeIO::test_single_node_io_emdpath",
+    "test/test_tree.py::TestTreeIO::test_subtree_io",
+    "test/test_tree.py::TestTreeIO::test_subtree_noroot_io",
+    "test/test_tree.py::TestTreeIO::test_unrooted_node_io",
+    "test/test_tree.py::TestTreeIO::test_whole_tree_io",
+    "test/test_tree.py::TestTreeIO::test_whole_tree_io_treeIsFalse"
+]
```

### Comparing `emdfile-0.0.5/src/emdfile/__init__.py` & `emdfile-0.0.6/src/emdfile/__init__.py`

 * *Files identical despite different names*

### Comparing `emdfile-0.0.5/src/emdfile/read.py` & `emdfile-0.0.6/src/emdfile/read.py`

 * *Files identical despite different names*

### Comparing `emdfile-0.0.5/src/emdfile/tqdmnd.py` & `emdfile-0.0.6/src/emdfile/tqdmnd.py`

 * *Files identical despite different names*

### Comparing `emdfile-0.0.5/src/emdfile/write.py` & `emdfile-0.0.6/src/emdfile/write.py`

 * *Files identical despite different names*

### Comparing `emdfile-0.0.5/src/emdfile/classes/array.py` & `emdfile-0.0.6/src/emdfile/classes/array.py`

 * *Files identical despite different names*

### Comparing `emdfile-0.0.5/src/emdfile/classes/custom.py` & `emdfile-0.0.6/src/emdfile/classes/custom.py`

 * *Files identical despite different names*

### Comparing `emdfile-0.0.5/src/emdfile/classes/metadata.py` & `emdfile-0.0.6/src/emdfile/classes/metadata.py`

 * *Files identical despite different names*

### Comparing `emdfile-0.0.5/src/emdfile/classes/pointlist.py` & `emdfile-0.0.6/src/emdfile/classes/pointlist.py`

 * *Files identical despite different names*

### Comparing `emdfile-0.0.5/src/emdfile/classes/pointlistarray.py` & `emdfile-0.0.6/src/emdfile/classes/pointlistarray.py`

 * *Files identical despite different names*

### Comparing `emdfile-0.0.5/src/emdfile/classes/tree.py` & `emdfile-0.0.6/src/emdfile/classes/tree.py`

 * *Files 0% similar despite different names*

```diff
@@ -156,28 +156,32 @@
     def metadata(self):
         return self._metadata
     @metadata.setter
     def metadata(self,x):
         assert(isinstance(x,Metadata))
         self._metadata[x.name] = x
 
+    @property
+    def treekeys(self):
+        return self._branch.keys()
+
 
     # displays top level contents of the node
     def __repr__(self):
         space = ' '*len(self.__class__.__name__)+'  '
         string = f"{self.__class__.__name__}( A Node called '{self.name}', containing the following top-level objects in its tree:"
         string += "\n"
         for k,v in self._branch.items():
             string += "\n"+space+f"    {k.ljust(24,' ')} \t ({v.__class__.__name__})"
         string += "\n)"
         return string
 
 
 
-    # tree methods
+    ########## .tree methods ###########
 
     def show_tree(self,root=False):
         """
         Display the object tree. If `root` is False, displays the branch
         of the tree downstream from this node.  If `root` is True, displays
         the full tree from the root node.
         """
@@ -375,15 +379,15 @@
                 else:
                     assert(len(v)==2), ".tree(graft=x) requires `x=Node` or `x=(node,metadata)` for some node and `metadata` in (True,False,'copy')"
                     n,m = v
                 return self.graft(node=n,merge_metadata=m)
             else:
                 raise Exception(f'Invalid arg {k}; must be in (show,add,get,cut,graft)')
 
-    ## end tree
+    ########## end .tree methods ###########
 
 
 
     # decorator for storing params which generated new data nodes
 
     @staticmethod
     def newnode(method):
```

### Comparing `emdfile-0.0.5/src/emdfile/classes/utils.py` & `emdfile-0.0.6/src/emdfile/classes/utils.py`

 * *Files identical despite different names*

### Comparing `emdfile-0.0.5/test/clear_h5_files.py` & `emdfile-0.0.6/test/clear_h5_files.py`

 * *Files identical despite different names*

### Comparing `emdfile-0.0.5/test/test_base_classes.py` & `emdfile-0.0.6/test/test_base_classes.py`

 * *Files identical despite different names*

### Comparing `emdfile-0.0.5/test/test_emd.py` & `emdfile-0.0.6/test/test_emd.py`

 * *Files identical despite different names*

### Comparing `emdfile-0.0.5/test/test_header.py` & `emdfile-0.0.6/test/test_header.py`

 * *Files identical despite different names*

### Comparing `emdfile-0.0.5/test/test_tree.py` & `emdfile-0.0.6/test/test_tree.py`

 * *Files identical despite different names*

### Comparing `emdfile-0.0.5/test/.pytest_cache/v/cache/nodeids` & `emdfile-0.0.6/test/.pytest_cache/v/cache/nodeids`

 * *Files identical despite different names*

### Comparing `emdfile-0.0.5/tutorials/emdfile_intro_example.ipynb` & `emdfile-0.0.6/tutorials/emdfile_intro_example.ipynb`

 * *Files identical despite different names*

### Comparing `emdfile-0.0.5/tutorials/emdfile_package_walkthrough.ipynb` & `emdfile-0.0.6/tutorials/emdfile_package_walkthrough.ipynb`

 * *Files identical despite different names*

### Comparing `emdfile-0.0.5/tutorials/test_custom_classes.py` & `emdfile-0.0.6/tutorials/test_custom_classes.py`

 * *Files identical despite different names*

### Comparing `emdfile-0.0.5/tutorials/pngs/node.png` & `emdfile-0.0.6/tutorials/pngs/node.png`

 * *Files identical despite different names*

### Comparing `emdfile-0.0.5/tutorials/pngs/tree.png` & `emdfile-0.0.6/tutorials/pngs/tree.png`

 * *Files identical despite different names*

### Comparing `emdfile-0.0.5/tutorials/sample_custom_emd_classes/my_custom_classes.py` & `emdfile-0.0.6/tutorials/sample_custom_emd_classes/my_custom_classes.py`

 * *Files identical despite different names*

### Comparing `emdfile-0.0.5/LICENSE` & `emdfile-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `emdfile-0.0.5/README.md` & `emdfile-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `emdfile-0.0.5/pyproject.toml` & `emdfile-0.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `emdfile-0.0.5/PKG-INFO` & `emdfile-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emdfile
-Version: 0.0.5
+Version: 0.0.6
 Project-URL: github, https://github.com/py4dstem/emdfile
 Project-URL: emdatasets, https://emdatasets.com/format/
 Author-email: "Benjamin H. Savitzky" <ben.savitzky@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
```

