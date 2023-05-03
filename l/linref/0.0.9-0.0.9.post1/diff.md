# Comparing `tmp/linref-0.0.9.tar.gz` & `tmp/linref-0.0.9.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linref-0.0.9.tar", last modified: Fri Mar  3 00:29:01 2023, max compression
+gzip compressed data, was "linref-0.0.9.post1.tar", last modified: Fri Mar  3 00:37:54 2023, max compression
```

## Comparing `linref-0.0.9.tar` & `linref-0.0.9.post1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-03-03 00:29:01.292563 linref-0.0.9/
--rw-rw-rw-   0        0        0     1092 2022-04-11 17:08:21.000000 linref-0.0.9/LICENSE.md
--rw-rw-rw-   0        0        0     7609 2023-03-03 00:29:01.290568 linref-0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0     6453 2023-03-03 00:22:27.000000 linref-0.0.9/README.md
-drwxrwxrwx   0        0        0        0 2023-03-03 00:29:01.202803 linref-0.0.9/linref/
--rw-rw-rw-   0        0        0      262 2022-12-02 18:51:56.000000 linref-0.0.9/linref/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-03 00:29:01.257657 linref-0.0.9/linref/events/
--rw-rw-rw-   0        0        0      202 2022-10-12 16:40:07.000000 linref-0.0.9/linref/events/__init__.py
--rw-rw-rw-   0        0        0    91238 2023-03-03 00:20:36.000000 linref-0.0.9/linref/events/collection.py
--rw-rw-rw-   0        0        0    37058 2023-01-25 17:32:24.000000 linref-0.0.9/linref/events/merge.py
--rw-rw-rw-   0        0        0     7977 2022-03-04 18:22:00.000000 linref-0.0.9/linref/events/spatial.py
--rw-rw-rw-   0        0        0     8598 2022-12-22 23:37:06.000000 linref-0.0.9/linref/events/union.py
-drwxrwxrwx   0        0        0        0 2023-03-03 00:29:01.274611 linref-0.0.9/linref/experimental/
--rw-rw-rw-   0        0        0        0 2022-01-04 20:58:17.000000 linref-0.0.9/linref/experimental/__init__.py
--rw-rw-rw-   0        0        0    14521 2022-01-31 19:10:03.000000 linref-0.0.9/linref/experimental/analysis.py
--rw-rw-rw-   0        0        0     8832 2021-10-25 22:27:40.000000 linref-0.0.9/linref/experimental/curves.py
--rw-rw-rw-   0        0        0    43195 2022-12-22 23:24:45.000000 linref-0.0.9/linref/route.py
-drwxrwxrwx   0        0        0        0 2023-03-03 00:29:01.284584 linref-0.0.9/linref/various/
--rw-rw-rw-   0        0        0        0 2022-01-04 21:04:59.000000 linref-0.0.9/linref/various/__init__.py
--rw-rw-rw-   0        0        0     2179 2022-05-12 22:27:33.000000 linref-0.0.9/linref/various/geospatial.py
-drwxrwxrwx   0        0        0        0 2023-03-03 00:29:01.230734 linref-0.0.9/linref.egg-info/
--rw-rw-rw-   0        0        0     7609 2023-03-03 00:28:59.000000 linref-0.0.9/linref.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      488 2023-03-03 00:29:00.000000 linref-0.0.9/linref.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-03 00:28:59.000000 linref-0.0.9/linref.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       74 2023-03-03 00:28:59.000000 linref-0.0.9/linref.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-03-03 00:28:59.000000 linref-0.0.9/linref.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-03 00:29:01.293566 linref-0.0.9/setup.cfg
--rw-rw-rw-   0        0        0     1170 2023-03-03 00:27:38.000000 linref-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-03-03 00:37:54.922126 linref-0.0.9.post1/
+-rw-rw-rw-   0        0        0     1092 2022-04-11 17:08:21.000000 linref-0.0.9.post1/LICENSE.md
+-rw-rw-rw-   0        0        0     7211 2023-03-03 00:37:54.920128 linref-0.0.9.post1/PKG-INFO
+-rw-rw-rw-   0        0        0     6477 2023-03-03 00:33:41.000000 linref-0.0.9.post1/README.md
+drwxrwxrwx   0        0        0        0 2023-03-03 00:37:54.809424 linref-0.0.9.post1/linref/
+-rw-rw-rw-   0        0        0      262 2022-12-02 18:51:56.000000 linref-0.0.9.post1/linref/__init__.py
+drwxrwxrwx   0        0        0        0 2023-03-03 00:37:54.876247 linref-0.0.9.post1/linref/events/
+-rw-rw-rw-   0        0        0      202 2022-10-12 16:40:07.000000 linref-0.0.9.post1/linref/events/__init__.py
+-rw-rw-rw-   0        0        0    91238 2023-03-03 00:20:36.000000 linref-0.0.9.post1/linref/events/collection.py
+-rw-rw-rw-   0        0        0    37058 2023-01-25 17:32:24.000000 linref-0.0.9.post1/linref/events/merge.py
+-rw-rw-rw-   0        0        0     7977 2022-03-04 18:22:00.000000 linref-0.0.9.post1/linref/events/spatial.py
+-rw-rw-rw-   0        0        0     8598 2022-12-22 23:37:06.000000 linref-0.0.9.post1/linref/events/union.py
+drwxrwxrwx   0        0        0        0 2023-03-03 00:37:54.908162 linref-0.0.9.post1/linref/experimental/
+-rw-rw-rw-   0        0        0        0 2022-01-04 20:58:17.000000 linref-0.0.9.post1/linref/experimental/__init__.py
+-rw-rw-rw-   0        0        0    14521 2022-01-31 19:10:03.000000 linref-0.0.9.post1/linref/experimental/analysis.py
+-rw-rw-rw-   0        0        0     8832 2021-10-25 22:27:40.000000 linref-0.0.9.post1/linref/experimental/curves.py
+-rw-rw-rw-   0        0        0    43195 2022-12-22 23:24:45.000000 linref-0.0.9.post1/linref/route.py
+drwxrwxrwx   0        0        0        0 2023-03-03 00:37:54.916139 linref-0.0.9.post1/linref/various/
+-rw-rw-rw-   0        0        0        0 2022-01-04 21:04:59.000000 linref-0.0.9.post1/linref/various/__init__.py
+-rw-rw-rw-   0        0        0     2179 2022-05-12 22:27:33.000000 linref-0.0.9.post1/linref/various/geospatial.py
+drwxrwxrwx   0        0        0        0 2023-03-03 00:37:54.835355 linref-0.0.9.post1/linref.egg-info/
+-rw-rw-rw-   0        0        0     7211 2023-03-03 00:37:53.000000 linref-0.0.9.post1/linref.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      488 2023-03-03 00:37:54.000000 linref-0.0.9.post1/linref.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-03-03 00:37:53.000000 linref-0.0.9.post1/linref.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       74 2023-03-03 00:37:54.000000 linref-0.0.9.post1/linref.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-03-03 00:37:54.000000 linref-0.0.9.post1/linref.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-03-03 00:37:54.923123 linref-0.0.9.post1/setup.cfg
+-rw-rw-rw-   0        0        0     1185 2023-03-03 00:36:52.000000 linref-0.0.9.post1/setup.py
```

### Comparing `linref-0.0.9/LICENSE.md` & `linref-0.0.9.post1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `linref-0.0.9/PKG-INFO` & `linref-0.0.9.post1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linref
-Version: 0.0.9
+Version: 0.0.9.post1
 Summary: Linearly referenced data management, manipulation, and operations
 Author: Tariq Shihadah
 Author-email: <tariq.shihadah@gmail.com>
 License: UNKNOWN
 Keywords: python,geospatial,linear,data,event,dissolve,overlay,range,numeric,interval
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
@@ -13,9 +13,116 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
-['# Overview\n', 'The `linref` library builds on tabular and geospatial libraries `pandas` and `geopandas` to implement powerful features for linearly referenced data through `EventsCollection` and other object classes. Linear referencing operations powered by the `numpy`, `shapely`, and `rangel` open-source libraries allow for optimized implementations of common and advanced linearly referenced data management, manipulation, and analysis operations.\n', '\n', 'Some of the main features of this library include:\n', '- Event dissolves using `EventsCollection.dissolve()`\n', '- Merging and overlaying multiple tables of events with the `EventsCollection.merge()` method and the `EventsMerge` class API and its many linearly-weighted overlay aggregators\n', '- Linear aggregations of data such as sliding window analysis with the powerful `EventsMerge.distribute()` method\n', '- Resegmentation of linear data with `EventsCollection.to_windows()` and related methods\n', '- Creating unions of multiple `EventsCollection` instances with the `EventsUnion` object class.\n', '\n', '# Code Snippets\n', 'Create an events collection for a sample roadway events dataframe with unique  \n', "route identifier represented by the 'Route' column and data for multiple years, \n", "represented by the 'Year' column. The begin and end mile points are defined by \n", "the 'Begin' and 'End' columns.\n", "`>>> ec = EventsCollection(df, keys=['Route','Year'], beg='Begin', end='End')`\n", '\n', 'To select events from a specific route and a specific year, indexing for all \n', 'keys can be used, producing an EventsGroup.\n', "`>>> eg = ec['Route 50', 2018]`\n", '\n', 'To select events on all routes but only those from a specific year, indexing \n', 'for only some keys can be used.\n', '`>>> ec_2018 = ec[:, 2018]`\n', '\n', 'To get all events which intersect with a numeric range, the intersecting() \n', 'method can be used on an EventsGroup instance.\n', "`>>> df_intersecting = eg.intersecting(0.5, 1.5, closed='left_mod')`\n", '\n', 'The intersecting() method can also be used for point locations by ommitting the \n', 'second location attribute.\n', "`>>> df_intersecting = eg.intersecting(0.75, closed='both')`\n", '\n', 'The linearly weighted average of one or more attributes can be obtained using \n', 'the overlay_average() method.\n', "`>>> df_overlay = eg.overlay_average(0.5, 1.5, cols=['Speed_Limit','Volume'])`\n", '\n', 'If the events include information on the roadway speed limit and number of \n', 'lanes, they can be dissolved on these attributes. During the dissolve, other \n', 'attributes can be aggregated, providing a list of associated values or \n', 'performing an aggregation function over these values.\n', "`>>> ec_dissolved = ec.dissolve(attr=['Speed_Limit','Lanes'], aggs=['County'])`\n", '\n', '# Version Notes\n', '## 0.0.9 (2023-03-02)\n', 'First update of 2023. Been a quiet start to the year.\n', '- Add missing .any() aggregation method to EventsMergeAttribute API. Was previously available but missed during a previous update.\n', '- Performance improvements\n', '- Various bug fixes, minor features\n', '\n', '## 0.0.8.post2 (2022-12-23)\n', 'Final update of 2022 including small feature updates and bug fixes from 0.0.8. Happy Holidays!\n', "- Add .set_df() method for in-line modification of an EventsFrame's dataframe, inplace or not.\n", '- Addition of suffixes parameter and default setting to EventsUnion.union() method.\n', '- Performance improvements\n', '- Various bug fixes, minor features\n', '\n', '## 0.0.8.post1 (2022-12-16)\n', '- Improve performance of .project() method when nearest=False by removing dependence on join_nearby() function and using native gpd features.\n', '- Add .size and .shape properties to EventsFrames and subclasses.\n', '- Various bug fixes, minor features\n', '\n', '## 0.0.8 (2022-12-14)\n', '- Improve performance of essential .get_group() method, reducing superfluous initialization of empty dataframes and events collections and improving logging of initialized groups.\n', '- Improve performance of .union() method with updated RangeCollection.union() features and optimized iteration and aggregation of unified data. Performance times are significantly improved, especially for large datasets with many events groups.\n', '- Improve distribute method performance which was added in recent versions.\n', "- Drop duplicates in .project() method when using sjoin_nearest with newer versions of geopandas. Improved validation in .project() method, address edge case where projecting geometry column has a non-standard label (e.g., not 'geometry').\n", '- Added .sort() method to events collection. Default sorting methods remain unchanged.\n', '- Added warnings for missing data in target columns when initializing an EventsFrames through standard methods.\n', '- Remove .project_old() method from events collection due to deprecation.\n', '- Performance improvements\n', '- Various bug fixes, minor features\n', '\n', '## 0.0.7 (2022-10-14)\n', '- Refactoring of EventsMerge system from 2D to 3D vectorized relationships for improved performance and accuracy. API and aggregation methods are largely the same.\n', '- Modified closed parameter use in merge relationships in accordance with rangel v0.0.6, which now performs intersections which honor the closed parameter on the left collection as well as the right collection. This provides more accurate results for events which fall on the edges of intersecting events when using left_mod or right_mod closed parameters.\n', '- Updates to account for rangel 0.0.6 version which is now a minimum version requirement. Added other minimum version requirements for related packages.\n', '- Performance improvements\n', '- Various bug fixes, minor features\n', '\n', '## 0.0.5.post1 (2022-09-06)\n', '- Address deprecation of length of and iteration over multi-part geometries in shapely\n', '- Remove code redundancies in linref.events.collection for get_most and get_mode\n', '\n', '## 0.0.5 (2022-09-01)\n', '- Added sumproduct and count aggregators to EventsMergeAttribute class\n', '- Address deprecation of length of and iteration over multi-part geometries in shapely\n', '- Performance improvements\n', '- Various bug fixes, minor features\n', '\n', '## 0.0.4 (2022-06-24)\n', '- Minor feature additions\n', '- Performance improvements\n', '- Addition of logos in github repo\n', '- Various bug fixes, minor features\n', '\n', '## 0.0.3 (2022-06-07)\n', '- Various updates for geopandas 0.10+ dependency including improved performance of project methods\n', '- Automatic sorting of events dataframe prior to performing dissolve\n', '- Performance improvements\n', '- Various bug fixes, minor features\n', '\n', '## 0.0.2 (2022-04-11)\n', '- Various bug fixes, minor features\n', '\n', '## 0.0.1 (2022-03-31)\n', '- Original experimental release.']
+# Overview
+The `linref` library builds on tabular and geospatial libraries `pandas` and `geopandas` to implement powerful features for linearly referenced data through `EventsCollection` and other object classes. Linear referencing operations powered by the `numpy`, `shapely`, and `rangel` open-source libraries allow for optimized implementations of common and advanced linearly referenced data management, manipulation, and analysis operations.
+
+Some of the main features of this library include:
+- Event dissolves using `EventsCollection.dissolve()`
+- Merging and overlaying multiple tables of events with the `EventsCollection.merge()` method and the `EventsMerge` class API and its many linearly-weighted overlay aggregators
+- Linear aggregations of data such as sliding window analysis with the powerful `EventsMerge.distribute()` method
+- Resegmentation of linear data with `EventsCollection.to_windows()` and related methods
+- Creating unions of multiple `EventsCollection` instances with the `EventsUnion` object class.
+
+# Code Snippets
+Create an events collection for a sample roadway events dataframe with unique  
+route identifier represented by the 'Route' column and data for multiple years, 
+represented by the 'Year' column. The begin and end mile points are defined by 
+the 'Begin' and 'End' columns.
+`>>> ec = EventsCollection(df, keys=['Route','Year'], beg='Begin', end='End')`
+
+To select events from a specific route and a specific year, indexing for all 
+keys can be used, producing an EventsGroup.
+`>>> eg = ec['Route 50', 2018]`
+
+To select events on all routes but only those from a specific year, indexing 
+for only some keys can be used.
+`>>> ec_2018 = ec[:, 2018]`
+
+To get all events which intersect with a numeric range, the intersecting() 
+method can be used on an EventsGroup instance.
+`>>> df_intersecting = eg.intersecting(0.5, 1.5, closed='left_mod')`
+
+The intersecting() method can also be used for point locations by ommitting the 
+second location attribute.
+`>>> df_intersecting = eg.intersecting(0.75, closed='both')`
+
+The linearly weighted average of one or more attributes can be obtained using 
+the overlay_average() method.
+`>>> df_overlay = eg.overlay_average(0.5, 1.5, cols=['Speed_Limit','Volume'])`
+
+If the events include information on the roadway speed limit and number of 
+lanes, they can be dissolved on these attributes. During the dissolve, other 
+attributes can be aggregated, providing a list of associated values or 
+performing an aggregation function over these values.
+`>>> ec_dissolved = ec.dissolve(attr=['Speed_Limit','Lanes'], aggs=['County'])`
+
+# Version Notes
+## 0.0.9 (2023-03-02)
+First update of 2023. Been a quiet start to the year.
+- Add missing .any() aggregation method to EventsMergeAttribute API. Was previously available but missed during a previous update.
+- Update documentation
+- Performance improvements
+- Various bug fixes, minor features
+
+## 0.0.8.post2 (2022-12-23)
+Final update of 2022 including small feature updates and bug fixes from 0.0.8. Happy Holidays!
+- Add .set_df() method for in-line modification of an EventsFrame's dataframe, inplace or not.
+- Addition of suffixes parameter and default setting to EventsUnion.union() method.
+- Performance improvements
+- Various bug fixes, minor features
+
+## 0.0.8.post1 (2022-12-16)
+- Improve performance of .project() method when nearest=False by removing dependence on join_nearby() function and using native gpd features.
+- Add .size and .shape properties to EventsFrames and subclasses.
+- Various bug fixes, minor features
+
+## 0.0.8 (2022-12-14)
+- Improve performance of essential .get_group() method, reducing superfluous initialization of empty dataframes and events collections and improving logging of initialized groups.
+- Improve performance of .union() method with updated RangeCollection.union() features and optimized iteration and aggregation of unified data. Performance times are significantly improved, especially for large datasets with many events groups.
+- Improve distribute method performance which was added in recent versions.
+- Drop duplicates in .project() method when using sjoin_nearest with newer versions of geopandas. Improved validation in .project() method, address edge case where projecting geometry column has a non-standard label (e.g., not 'geometry').
+- Added .sort() method to events collection. Default sorting methods remain unchanged.
+- Added warnings for missing data in target columns when initializing an EventsFrames through standard methods.
+- Remove .project_old() method from events collection due to deprecation.
+- Performance improvements
+- Various bug fixes, minor features
+
+## 0.0.7 (2022-10-14)
+- Refactoring of EventsMerge system from 2D to 3D vectorized relationships for improved performance and accuracy. API and aggregation methods are largely the same.
+- Modified closed parameter use in merge relationships in accordance with rangel v0.0.6, which now performs intersections which honor the closed parameter on the left collection as well as the right collection. This provides more accurate results for events which fall on the edges of intersecting events when using left_mod or right_mod closed parameters.
+- Updates to account for rangel 0.0.6 version which is now a minimum version requirement. Added other minimum version requirements for related packages.
+- Performance improvements
+- Various bug fixes, minor features
+
+## 0.0.5.post1 (2022-09-06)
+- Address deprecation of length of and iteration over multi-part geometries in shapely
+- Remove code redundancies in linref.events.collection for get_most and get_mode
+
+## 0.0.5 (2022-09-01)
+- Added sumproduct and count aggregators to EventsMergeAttribute class
+- Address deprecation of length of and iteration over multi-part geometries in shapely
+- Performance improvements
+- Various bug fixes, minor features
+
+## 0.0.4 (2022-06-24)
+- Minor feature additions
+- Performance improvements
+- Addition of logos in github repo
+- Various bug fixes, minor features
+
+## 0.0.3 (2022-06-07)
+- Various updates for geopandas 0.10+ dependency including improved performance of project methods
+- Automatic sorting of events dataframe prior to performing dissolve
+- Performance improvements
+- Various bug fixes, minor features
+
+## 0.0.2 (2022-04-11)
+- Various bug fixes, minor features
+
+## 0.0.1 (2022-03-31)
+- Original experimental release.
```

### Comparing `linref-0.0.9/README.md` & `linref-0.0.9.post1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -41,14 +41,15 @@
 performing an aggregation function over these values.
 `>>> ec_dissolved = ec.dissolve(attr=['Speed_Limit','Lanes'], aggs=['County'])`
 
 # Version Notes
 ## 0.0.9 (2023-03-02)
 First update of 2023. Been a quiet start to the year.
 - Add missing .any() aggregation method to EventsMergeAttribute API. Was previously available but missed during a previous update.
+- Update documentation
 - Performance improvements
 - Various bug fixes, minor features
 
 ## 0.0.8.post2 (2022-12-23)
 Final update of 2022 including small feature updates and bug fixes from 0.0.8. Happy Holidays!
 - Add .set_df() method for in-line modification of an EventsFrame's dataframe, inplace or not.
 - Addition of suffixes parameter and default setting to EventsUnion.union() method.
```

### Comparing `linref-0.0.9/linref/events/collection.py` & `linref-0.0.9.post1/linref/events/collection.py`

 * *Files identical despite different names*

### Comparing `linref-0.0.9/linref/events/merge.py` & `linref-0.0.9.post1/linref/events/merge.py`

 * *Files identical despite different names*

### Comparing `linref-0.0.9/linref/events/spatial.py` & `linref-0.0.9.post1/linref/events/spatial.py`

 * *Files identical despite different names*

### Comparing `linref-0.0.9/linref/events/union.py` & `linref-0.0.9.post1/linref/events/union.py`

 * *Files identical despite different names*

### Comparing `linref-0.0.9/linref/experimental/analysis.py` & `linref-0.0.9.post1/linref/experimental/analysis.py`

 * *Files identical despite different names*

### Comparing `linref-0.0.9/linref/experimental/curves.py` & `linref-0.0.9.post1/linref/experimental/curves.py`

 * *Files identical despite different names*

### Comparing `linref-0.0.9/linref/route.py` & `linref-0.0.9.post1/linref/route.py`

 * *Files identical despite different names*

### Comparing `linref-0.0.9/linref/various/geospatial.py` & `linref-0.0.9.post1/linref/various/geospatial.py`

 * *Files identical despite different names*

### Comparing `linref-0.0.9/linref.egg-info/PKG-INFO` & `linref-0.0.9.post1/linref.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linref
-Version: 0.0.9
+Version: 0.0.9.post1
 Summary: Linearly referenced data management, manipulation, and operations
 Author: Tariq Shihadah
 Author-email: <tariq.shihadah@gmail.com>
 License: UNKNOWN
 Keywords: python,geospatial,linear,data,event,dissolve,overlay,range,numeric,interval
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
@@ -13,9 +13,116 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
-['# Overview\n', 'The `linref` library builds on tabular and geospatial libraries `pandas` and `geopandas` to implement powerful features for linearly referenced data through `EventsCollection` and other object classes. Linear referencing operations powered by the `numpy`, `shapely`, and `rangel` open-source libraries allow for optimized implementations of common and advanced linearly referenced data management, manipulation, and analysis operations.\n', '\n', 'Some of the main features of this library include:\n', '- Event dissolves using `EventsCollection.dissolve()`\n', '- Merging and overlaying multiple tables of events with the `EventsCollection.merge()` method and the `EventsMerge` class API and its many linearly-weighted overlay aggregators\n', '- Linear aggregations of data such as sliding window analysis with the powerful `EventsMerge.distribute()` method\n', '- Resegmentation of linear data with `EventsCollection.to_windows()` and related methods\n', '- Creating unions of multiple `EventsCollection` instances with the `EventsUnion` object class.\n', '\n', '# Code Snippets\n', 'Create an events collection for a sample roadway events dataframe with unique  \n', "route identifier represented by the 'Route' column and data for multiple years, \n", "represented by the 'Year' column. The begin and end mile points are defined by \n", "the 'Begin' and 'End' columns.\n", "`>>> ec = EventsCollection(df, keys=['Route','Year'], beg='Begin', end='End')`\n", '\n', 'To select events from a specific route and a specific year, indexing for all \n', 'keys can be used, producing an EventsGroup.\n', "`>>> eg = ec['Route 50', 2018]`\n", '\n', 'To select events on all routes but only those from a specific year, indexing \n', 'for only some keys can be used.\n', '`>>> ec_2018 = ec[:, 2018]`\n', '\n', 'To get all events which intersect with a numeric range, the intersecting() \n', 'method can be used on an EventsGroup instance.\n', "`>>> df_intersecting = eg.intersecting(0.5, 1.5, closed='left_mod')`\n", '\n', 'The intersecting() method can also be used for point locations by ommitting the \n', 'second location attribute.\n', "`>>> df_intersecting = eg.intersecting(0.75, closed='both')`\n", '\n', 'The linearly weighted average of one or more attributes can be obtained using \n', 'the overlay_average() method.\n', "`>>> df_overlay = eg.overlay_average(0.5, 1.5, cols=['Speed_Limit','Volume'])`\n", '\n', 'If the events include information on the roadway speed limit and number of \n', 'lanes, they can be dissolved on these attributes. During the dissolve, other \n', 'attributes can be aggregated, providing a list of associated values or \n', 'performing an aggregation function over these values.\n', "`>>> ec_dissolved = ec.dissolve(attr=['Speed_Limit','Lanes'], aggs=['County'])`\n", '\n', '# Version Notes\n', '## 0.0.9 (2023-03-02)\n', 'First update of 2023. Been a quiet start to the year.\n', '- Add missing .any() aggregation method to EventsMergeAttribute API. Was previously available but missed during a previous update.\n', '- Performance improvements\n', '- Various bug fixes, minor features\n', '\n', '## 0.0.8.post2 (2022-12-23)\n', 'Final update of 2022 including small feature updates and bug fixes from 0.0.8. Happy Holidays!\n', "- Add .set_df() method for in-line modification of an EventsFrame's dataframe, inplace or not.\n", '- Addition of suffixes parameter and default setting to EventsUnion.union() method.\n', '- Performance improvements\n', '- Various bug fixes, minor features\n', '\n', '## 0.0.8.post1 (2022-12-16)\n', '- Improve performance of .project() method when nearest=False by removing dependence on join_nearby() function and using native gpd features.\n', '- Add .size and .shape properties to EventsFrames and subclasses.\n', '- Various bug fixes, minor features\n', '\n', '## 0.0.8 (2022-12-14)\n', '- Improve performance of essential .get_group() method, reducing superfluous initialization of empty dataframes and events collections and improving logging of initialized groups.\n', '- Improve performance of .union() method with updated RangeCollection.union() features and optimized iteration and aggregation of unified data. Performance times are significantly improved, especially for large datasets with many events groups.\n', '- Improve distribute method performance which was added in recent versions.\n', "- Drop duplicates in .project() method when using sjoin_nearest with newer versions of geopandas. Improved validation in .project() method, address edge case where projecting geometry column has a non-standard label (e.g., not 'geometry').\n", '- Added .sort() method to events collection. Default sorting methods remain unchanged.\n', '- Added warnings for missing data in target columns when initializing an EventsFrames through standard methods.\n', '- Remove .project_old() method from events collection due to deprecation.\n', '- Performance improvements\n', '- Various bug fixes, minor features\n', '\n', '## 0.0.7 (2022-10-14)\n', '- Refactoring of EventsMerge system from 2D to 3D vectorized relationships for improved performance and accuracy. API and aggregation methods are largely the same.\n', '- Modified closed parameter use in merge relationships in accordance with rangel v0.0.6, which now performs intersections which honor the closed parameter on the left collection as well as the right collection. This provides more accurate results for events which fall on the edges of intersecting events when using left_mod or right_mod closed parameters.\n', '- Updates to account for rangel 0.0.6 version which is now a minimum version requirement. Added other minimum version requirements for related packages.\n', '- Performance improvements\n', '- Various bug fixes, minor features\n', '\n', '## 0.0.5.post1 (2022-09-06)\n', '- Address deprecation of length of and iteration over multi-part geometries in shapely\n', '- Remove code redundancies in linref.events.collection for get_most and get_mode\n', '\n', '## 0.0.5 (2022-09-01)\n', '- Added sumproduct and count aggregators to EventsMergeAttribute class\n', '- Address deprecation of length of and iteration over multi-part geometries in shapely\n', '- Performance improvements\n', '- Various bug fixes, minor features\n', '\n', '## 0.0.4 (2022-06-24)\n', '- Minor feature additions\n', '- Performance improvements\n', '- Addition of logos in github repo\n', '- Various bug fixes, minor features\n', '\n', '## 0.0.3 (2022-06-07)\n', '- Various updates for geopandas 0.10+ dependency including improved performance of project methods\n', '- Automatic sorting of events dataframe prior to performing dissolve\n', '- Performance improvements\n', '- Various bug fixes, minor features\n', '\n', '## 0.0.2 (2022-04-11)\n', '- Various bug fixes, minor features\n', '\n', '## 0.0.1 (2022-03-31)\n', '- Original experimental release.']
+# Overview
+The `linref` library builds on tabular and geospatial libraries `pandas` and `geopandas` to implement powerful features for linearly referenced data through `EventsCollection` and other object classes. Linear referencing operations powered by the `numpy`, `shapely`, and `rangel` open-source libraries allow for optimized implementations of common and advanced linearly referenced data management, manipulation, and analysis operations.
+
+Some of the main features of this library include:
+- Event dissolves using `EventsCollection.dissolve()`
+- Merging and overlaying multiple tables of events with the `EventsCollection.merge()` method and the `EventsMerge` class API and its many linearly-weighted overlay aggregators
+- Linear aggregations of data such as sliding window analysis with the powerful `EventsMerge.distribute()` method
+- Resegmentation of linear data with `EventsCollection.to_windows()` and related methods
+- Creating unions of multiple `EventsCollection` instances with the `EventsUnion` object class.
+
+# Code Snippets
+Create an events collection for a sample roadway events dataframe with unique  
+route identifier represented by the 'Route' column and data for multiple years, 
+represented by the 'Year' column. The begin and end mile points are defined by 
+the 'Begin' and 'End' columns.
+`>>> ec = EventsCollection(df, keys=['Route','Year'], beg='Begin', end='End')`
+
+To select events from a specific route and a specific year, indexing for all 
+keys can be used, producing an EventsGroup.
+`>>> eg = ec['Route 50', 2018]`
+
+To select events on all routes but only those from a specific year, indexing 
+for only some keys can be used.
+`>>> ec_2018 = ec[:, 2018]`
+
+To get all events which intersect with a numeric range, the intersecting() 
+method can be used on an EventsGroup instance.
+`>>> df_intersecting = eg.intersecting(0.5, 1.5, closed='left_mod')`
+
+The intersecting() method can also be used for point locations by ommitting the 
+second location attribute.
+`>>> df_intersecting = eg.intersecting(0.75, closed='both')`
+
+The linearly weighted average of one or more attributes can be obtained using 
+the overlay_average() method.
+`>>> df_overlay = eg.overlay_average(0.5, 1.5, cols=['Speed_Limit','Volume'])`
+
+If the events include information on the roadway speed limit and number of 
+lanes, they can be dissolved on these attributes. During the dissolve, other 
+attributes can be aggregated, providing a list of associated values or 
+performing an aggregation function over these values.
+`>>> ec_dissolved = ec.dissolve(attr=['Speed_Limit','Lanes'], aggs=['County'])`
+
+# Version Notes
+## 0.0.9 (2023-03-02)
+First update of 2023. Been a quiet start to the year.
+- Add missing .any() aggregation method to EventsMergeAttribute API. Was previously available but missed during a previous update.
+- Update documentation
+- Performance improvements
+- Various bug fixes, minor features
+
+## 0.0.8.post2 (2022-12-23)
+Final update of 2022 including small feature updates and bug fixes from 0.0.8. Happy Holidays!
+- Add .set_df() method for in-line modification of an EventsFrame's dataframe, inplace or not.
+- Addition of suffixes parameter and default setting to EventsUnion.union() method.
+- Performance improvements
+- Various bug fixes, minor features
+
+## 0.0.8.post1 (2022-12-16)
+- Improve performance of .project() method when nearest=False by removing dependence on join_nearby() function and using native gpd features.
+- Add .size and .shape properties to EventsFrames and subclasses.
+- Various bug fixes, minor features
+
+## 0.0.8 (2022-12-14)
+- Improve performance of essential .get_group() method, reducing superfluous initialization of empty dataframes and events collections and improving logging of initialized groups.
+- Improve performance of .union() method with updated RangeCollection.union() features and optimized iteration and aggregation of unified data. Performance times are significantly improved, especially for large datasets with many events groups.
+- Improve distribute method performance which was added in recent versions.
+- Drop duplicates in .project() method when using sjoin_nearest with newer versions of geopandas. Improved validation in .project() method, address edge case where projecting geometry column has a non-standard label (e.g., not 'geometry').
+- Added .sort() method to events collection. Default sorting methods remain unchanged.
+- Added warnings for missing data in target columns when initializing an EventsFrames through standard methods.
+- Remove .project_old() method from events collection due to deprecation.
+- Performance improvements
+- Various bug fixes, minor features
+
+## 0.0.7 (2022-10-14)
+- Refactoring of EventsMerge system from 2D to 3D vectorized relationships for improved performance and accuracy. API and aggregation methods are largely the same.
+- Modified closed parameter use in merge relationships in accordance with rangel v0.0.6, which now performs intersections which honor the closed parameter on the left collection as well as the right collection. This provides more accurate results for events which fall on the edges of intersecting events when using left_mod or right_mod closed parameters.
+- Updates to account for rangel 0.0.6 version which is now a minimum version requirement. Added other minimum version requirements for related packages.
+- Performance improvements
+- Various bug fixes, minor features
+
+## 0.0.5.post1 (2022-09-06)
+- Address deprecation of length of and iteration over multi-part geometries in shapely
+- Remove code redundancies in linref.events.collection for get_most and get_mode
+
+## 0.0.5 (2022-09-01)
+- Added sumproduct and count aggregators to EventsMergeAttribute class
+- Address deprecation of length of and iteration over multi-part geometries in shapely
+- Performance improvements
+- Various bug fixes, minor features
+
+## 0.0.4 (2022-06-24)
+- Minor feature additions
+- Performance improvements
+- Addition of logos in github repo
+- Various bug fixes, minor features
+
+## 0.0.3 (2022-06-07)
+- Various updates for geopandas 0.10+ dependency including improved performance of project methods
+- Automatic sorting of events dataframe prior to performing dissolve
+- Performance improvements
+- Various bug fixes, minor features
+
+## 0.0.2 (2022-04-11)
+- Various bug fixes, minor features
+
+## 0.0.1 (2022-03-31)
+- Original experimental release.
```

### Comparing `linref-0.0.9/setup.py` & `linref-0.0.9.post1/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.0.9'
+VERSION = '0.0.9.post1'
 DESCRIPTION = 'Linearly referenced data management, manipulation, and operations'
 with open('README.md') as f:
-    LONG_DESCRIPTION = f.readlines()
+    LONG_DESCRIPTION = ''.join(f.readlines())
 
 # Setting up
 setup(
     name="linref",
     version=VERSION,
     author="Tariq Shihadah",
     author_email="<tariq.shihadah@gmail.com>",
```

