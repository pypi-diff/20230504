# Comparing `tmp/aplr-2.6.0-pp39-pypy39_pp73-win_amd64.whl.zip` & `tmp/aplr-2.7.0-pp39-pypy39_pp73-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 293000 bytes, number of entries: 9
--rw-rw-rw-  2.0 fat   322560 b- defN 23-May-02 15:54 aplr_cpp.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat   333824 b- defN 23-May-02 15:58 aplr_cpp.pypy39-pp73-win_amd64.pyd
--rw-rw-rw-  2.0 fat       19 b- defN 23-May-02 15:48 aplr/__init__.py
--rw-rw-rw-  2.0 fat     6151 b- defN 23-May-02 15:48 aplr/aplr.py
--rw-rw-rw-  2.0 fat     1134 b- defN 23-May-02 15:58 aplr-2.6.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      626 b- defN 23-May-02 15:58 aplr-2.6.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat      107 b- defN 23-May-02 15:58 aplr-2.6.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       14 b- defN 23-May-02 15:58 aplr-2.6.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      690 b- defN 23-May-02 15:58 aplr-2.6.0.dist-info/RECORD
-9 files, 665125 bytes uncompressed, 291828 bytes compressed:  56.1%
+Zip file size: 293690 bytes, number of entries: 9
+-rw-rw-rw-  2.0 fat   323072 b- defN 23-May-04 15:05 aplr_cpp.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat   335360 b- defN 23-May-04 15:09 aplr_cpp.pypy39-pp73-win_amd64.pyd
+-rw-rw-rw-  2.0 fat       19 b- defN 23-May-04 15:01 aplr/__init__.py
+-rw-rw-rw-  2.0 fat     6214 b- defN 23-May-04 15:01 aplr/aplr.py
+-rw-rw-rw-  2.0 fat     1134 b- defN 23-May-04 15:09 aplr-2.7.0.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      626 b- defN 23-May-04 15:09 aplr-2.7.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      107 b- defN 23-May-04 15:09 aplr-2.7.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       14 b- defN 23-May-04 15:09 aplr-2.7.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      690 b- defN 23-May-04 15:09 aplr-2.7.0.dist-info/RECORD
+9 files, 667236 bytes uncompressed, 292518 bytes compressed:  56.2%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: aplr/__init__.py
 Comment: 
 
 Filename: aplr/aplr.py
 Comment: 
 
-Filename: aplr-2.6.0.dist-info/LICENSE
+Filename: aplr-2.7.0.dist-info/LICENSE
 Comment: 
 
-Filename: aplr-2.6.0.dist-info/METADATA
+Filename: aplr-2.7.0.dist-info/METADATA
 Comment: 
 
-Filename: aplr-2.6.0.dist-info/WHEEL
+Filename: aplr-2.7.0.dist-info/WHEEL
 Comment: 
 
-Filename: aplr-2.6.0.dist-info/top_level.txt
+Filename: aplr-2.7.0.dist-info/top_level.txt
 Comment: 
 
-Filename: aplr-2.6.0.dist-info/RECORD
+Filename: aplr-2.7.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## aplr/aplr.py

```diff
@@ -46,17 +46,17 @@
         self.APLRRegressor.ineligible_boosting_steps_added=self.ineligible_boosting_steps_added
         self.APLRRegressor.max_eligible_terms=self.max_eligible_terms
         self.APLRRegressor.verbosity=self.verbosity
         self.APLRRegressor.tweedie_power=self.tweedie_power
         self.APLRRegressor.validation_tuning_metric=self.validation_tuning_metric
         self.APLRRegressor.quantile=self.quantile
 
-    def fit(self, X:npt.ArrayLike, y:npt.ArrayLike, sample_weight:npt.ArrayLike = np.empty(0), X_names:List[str]=[], validation_set_indexes:List[int]=[], prioritized_predictors_indexes:List[int]=[], monotonic_constraints:List[int]=[],group:npt.ArrayLike = np.empty(0)):
+    def fit(self, X:npt.ArrayLike, y:npt.ArrayLike, sample_weight:npt.ArrayLike = np.empty(0), X_names:List[str]=[], validation_set_indexes:List[int]=[], prioritized_predictors_indexes:List[int]=[], monotonic_constraints:List[int]=[], group:npt.ArrayLike = np.empty(0), interaction_constraints:List[int]=[]):
         self.__set_params_cpp()
-        self.APLRRegressor.fit(X,y,sample_weight,X_names,validation_set_indexes,prioritized_predictors_indexes,monotonic_constraints,group)
+        self.APLRRegressor.fit(X,y,sample_weight,X_names,validation_set_indexes,prioritized_predictors_indexes,monotonic_constraints,group,interaction_constraints)
 
     def predict(self, X:npt.ArrayLike, cap_predictions_to_minmax_in_training:bool=True)->npt.ArrayLike:
         return self.APLRRegressor.predict(X, cap_predictions_to_minmax_in_training)
 
     def set_term_names(self, X_names:List[str]):
         self.APLRRegressor.set_term_names(X_names)
```

## Comparing `aplr-2.6.0.dist-info/LICENSE` & `aplr-2.7.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `aplr-2.6.0.dist-info/METADATA` & `aplr-2.7.0.dist-info/METADATA`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aplr
-Version: 2.6.0
+Version: 2.7.0
 Summary: Automatic Piecewise Linear Regression
 Home-page: https://github.com/ottenbreit-data-science/aplr
 Author: Mathias von Ottenbreit
 Author-email: ottenbreitdatascience@gmail.com
 License: MIT
 Platform: Windows
 Platform: Linux
```

## Comparing `aplr-2.6.0.dist-info/RECORD` & `aplr-2.7.0.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-aplr_cpp.cp39-win_amd64.pyd,sha256=7ol9ZgSLuzq8CwiKogEBFFv9I1GSaoijGWlcaxNUakU,322560
-aplr_cpp.pypy39-pp73-win_amd64.pyd,sha256=X7QY2gBAuv-fnuLc7wCKgJt9j6CasElw9kpRvvaI2uw,333824
+aplr_cpp.cp39-win_amd64.pyd,sha256=BmLY2AZTi4mCpCqfKXj5ok-ESeOab0azRPChU9G-HDc,323072
+aplr_cpp.pypy39-pp73-win_amd64.pyd,sha256=w0kgUyH9HM86piRN4tUw1tyuS21LRQBOtbza2iKYfIU,335360
 aplr/__init__.py,sha256=jLHRAp1zq22wmHqFIghBqfVSnMBnd27LjffHgzI07Hw,19
-aplr/aplr.py,sha256=md6z28MbPZsRTD876fKWyOiF7Jo-ttZPhfp-rHP_WKY,6151
-aplr-2.6.0.dist-info/LICENSE,sha256=YOMo-RaL4P7edMZGD96-NskKpxyMZdP3-WiiMMmihNk,1134
-aplr-2.6.0.dist-info/METADATA,sha256=U0MkI2r_VltIkwe5YMkvui0A6HcobequJaqdZJb-4KY,626
-aplr-2.6.0.dist-info/WHEEL,sha256=kbzA5tyEuvWcVsltnhCG02Vwq0RkG0K4o74bVDVA1mQ,107
-aplr-2.6.0.dist-info/top_level.txt,sha256=DXVC0RIFGpzVnPeKWAZTXQdJheOEZL51Wip6Fx7zbR4,14
-aplr-2.6.0.dist-info/RECORD,,
+aplr/aplr.py,sha256=Oj5RqI9fhc-uS8S0FPDyrt34PAhAFEDNpGn_-vPgzb4,6214
+aplr-2.7.0.dist-info/LICENSE,sha256=YOMo-RaL4P7edMZGD96-NskKpxyMZdP3-WiiMMmihNk,1134
+aplr-2.7.0.dist-info/METADATA,sha256=6MP0QX1vul1QU46jzilrceiQ-e61Yvi7PCp85PdzLgE,626
+aplr-2.7.0.dist-info/WHEEL,sha256=kbzA5tyEuvWcVsltnhCG02Vwq0RkG0K4o74bVDVA1mQ,107
+aplr-2.7.0.dist-info/top_level.txt,sha256=DXVC0RIFGpzVnPeKWAZTXQdJheOEZL51Wip6Fx7zbR4,14
+aplr-2.7.0.dist-info/RECORD,,
```

