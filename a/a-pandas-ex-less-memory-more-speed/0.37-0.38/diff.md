# Comparing `tmp/a_pandas_ex_less_memory_more_speed-0.37.tar.gz` & `tmp/a_pandas_ex_less_memory_more_speed-0.38.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "a_pandas_ex_less_memory_more_speed-0.37.tar", last modified: Fri Jan  6 03:45:14 2023, max compression
+gzip compressed data, was "a_pandas_ex_less_memory_more_speed-0.38.tar", last modified: Thu May  4 14:27:32 2023, max compression
```

## Comparing `a_pandas_ex_less_memory_more_speed-0.37.tar` & `a_pandas_ex_less_memory_more_speed-0.38.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-01-06 03:45:14.912525 a_pandas_ex_less_memory_more_speed-0.37/
--rw-rw-rw-   0        0        0     1148 2023-01-06 03:45:05.000000 a_pandas_ex_less_memory_more_speed-0.37/LICENSE.rst
--rw-rw-rw-   0        0        0      225 2023-01-06 03:45:04.000000 a_pandas_ex_less_memory_more_speed-0.37/MANIFEST.in
--rw-rw-rw-   0        0        0    17333 2023-01-06 03:45:14.913500 a_pandas_ex_less_memory_more_speed-0.37/PKG-INFO
--rw-rw-rw-   0        0        0    15773 2022-10-09 04:52:01.000000 a_pandas_ex_less_memory_more_speed-0.37/README.md
-drwxrwxrwx   0        0        0        0 2023-01-06 03:45:14.908620 a_pandas_ex_less_memory_more_speed-0.37/a_pandas_ex_less_memory_more_speed/
--rw-rw-rw-   0        0        0     1069 2023-01-04 04:49:17.000000 a_pandas_ex_less_memory_more_speed-0.37/a_pandas_ex_less_memory_more_speed/LICENSE
--rw-rw-rw-   0        0        0    15773 2022-10-09 04:52:01.000000 a_pandas_ex_less_memory_more_speed-0.37/a_pandas_ex_less_memory_more_speed/README.MD
--rw-rw-rw-   0        0        0    34338 2023-01-06 03:43:15.000000 a_pandas_ex_less_memory_more_speed-0.37/a_pandas_ex_less_memory_more_speed/__init__.py
--rw-rw-rw-   0        0        0       44 2023-01-06 03:45:13.000000 a_pandas_ex_less_memory_more_speed-0.37/a_pandas_ex_less_memory_more_speed/requirements.txt
--rw-rw-rw-   0        0        0        2 2023-01-06 03:45:13.000000 a_pandas_ex_less_memory_more_speed-0.37/a_pandas_ex_less_memory_more_speed/thirdparty.json
-drwxrwxrwx   0        0        0        0 2023-01-06 03:45:14.912525 a_pandas_ex_less_memory_more_speed-0.37/a_pandas_ex_less_memory_more_speed.egg-info/
--rw-rw-rw-   0        0        0    17333 2023-01-06 03:45:14.000000 a_pandas_ex_less_memory_more_speed-0.37/a_pandas_ex_less_memory_more_speed.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      579 2023-01-06 03:45:14.000000 a_pandas_ex_less_memory_more_speed-0.37/a_pandas_ex_less_memory_more_speed.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-06 03:45:14.000000 a_pandas_ex_less_memory_more_speed-0.37/a_pandas_ex_less_memory_more_speed.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       42 2023-01-06 03:45:14.000000 a_pandas_ex_less_memory_more_speed-0.37/a_pandas_ex_less_memory_more_speed.egg-info/requires.txt
--rw-rw-rw-   0        0        0       35 2023-01-06 03:45:14.000000 a_pandas_ex_less_memory_more_speed-0.37/a_pandas_ex_less_memory_more_speed.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      115 2023-01-06 03:45:14.913500 a_pandas_ex_less_memory_more_speed-0.37/setup.cfg
--rw-rw-rw-   0        0        0     1755 2023-01-06 03:45:13.000000 a_pandas_ex_less_memory_more_speed-0.37/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 14:27:32.770896 a_pandas_ex_less_memory_more_speed-0.38/
+-rw-rw-rw-   0        0        0     1148 2023-05-04 14:27:22.000000 a_pandas_ex_less_memory_more_speed-0.38/LICENSE.rst
+-rw-rw-rw-   0        0        0      225 2023-05-04 14:27:21.000000 a_pandas_ex_less_memory_more_speed-0.38/MANIFEST.in
+-rw-rw-rw-   0        0        0    20546 2023-05-04 14:27:32.771896 a_pandas_ex_less_memory_more_speed-0.38/PKG-INFO
+-rw-rw-rw-   0        0        0    17128 2023-05-04 14:23:56.000000 a_pandas_ex_less_memory_more_speed-0.38/README.md
+drwxrwxrwx   0        0        0        0 2023-05-04 14:27:32.766907 a_pandas_ex_less_memory_more_speed-0.38/a_pandas_ex_less_memory_more_speed/
+-rw-rw-rw-   0        0        0     1069 2023-05-03 02:33:15.000000 a_pandas_ex_less_memory_more_speed-0.38/a_pandas_ex_less_memory_more_speed/LICENSE
+-rw-rw-rw-   0        0        0    17128 2023-05-04 14:23:56.000000 a_pandas_ex_less_memory_more_speed-0.38/a_pandas_ex_less_memory_more_speed/README.MD
+-rw-rw-rw-   0        0        0    43716 2023-05-04 14:21:29.000000 a_pandas_ex_less_memory_more_speed-0.38/a_pandas_ex_less_memory_more_speed/__init__.py
+-rw-rw-rw-   0        0        0       69 2023-05-04 14:27:31.000000 a_pandas_ex_less_memory_more_speed-0.38/a_pandas_ex_less_memory_more_speed/requirements.txt
+-rw-rw-rw-   0        0        0    53338 2023-05-04 14:27:31.000000 a_pandas_ex_less_memory_more_speed-0.38/a_pandas_ex_less_memory_more_speed/thirdparty.json
+drwxrwxrwx   0        0        0        0 2023-05-04 14:27:32.769898 a_pandas_ex_less_memory_more_speed-0.38/a_pandas_ex_less_memory_more_speed.egg-info/
+-rw-rw-rw-   0        0        0    20546 2023-05-04 14:27:32.000000 a_pandas_ex_less_memory_more_speed-0.38/a_pandas_ex_less_memory_more_speed.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      579 2023-05-04 14:27:32.000000 a_pandas_ex_less_memory_more_speed-0.38/a_pandas_ex_less_memory_more_speed.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 14:27:32.000000 a_pandas_ex_less_memory_more_speed-0.38/a_pandas_ex_less_memory_more_speed.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       65 2023-05-04 14:27:32.000000 a_pandas_ex_less_memory_more_speed-0.38/a_pandas_ex_less_memory_more_speed.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       35 2023-05-04 14:27:32.000000 a_pandas_ex_less_memory_more_speed-0.38/a_pandas_ex_less_memory_more_speed.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2023-05-04 14:27:32.771896 a_pandas_ex_less_memory_more_speed-0.38/setup.cfg
+-rw-rw-rw-   0        0        0     1729 2023-05-04 14:27:31.000000 a_pandas_ex_less_memory_more_speed-0.38/setup.py
```

### Comparing `a_pandas_ex_less_memory_more_speed-0.37/LICENSE.rst` & `a_pandas_ex_less_memory_more_speed-0.38/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `a_pandas_ex_less_memory_more_speed-0.37/PKG-INFO` & `a_pandas_ex_less_memory_more_speed-0.38/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,450 +1,456 @@
-Metadata-Version: 2.1
-Name: a_pandas_ex_less_memory_more_speed
-Version: 0.37
-Summary: A Python package to reduce the memory usage of pandas DataFrames. It speeds up your workflow and reduces the risk of running out of memory.
-Home-page: https://github.com/hansalemaos/a_pandas_ex_less_memory_more_speed
-Author: Johannes Fischer
-Author-email: <aulasparticularesdealemaosp@gmail.com>
-License: MIT
-Keywords: flatten,pandas,dict,list,numpy,tuple,Tagsiter,nested,iterable,listsoflists,flattenjson,iter,explode,squeeze,nan,pd.NA,np.nan
-Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Topic :: Scientific/Engineering :: Visualization
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Text Editors :: Text Processing
-Classifier: Topic :: Text Processing :: General
-Classifier: Topic :: Text Processing :: Indexing
-Classifier: Topic :: Text Processing :: Filters
-Classifier: Topic :: Utilities
-Description-Content-Type: text/markdown
-License-File: LICENSE.rst
-
-
-## Less memory usage - more speed
-
-A Python package to reduce the memory usage of pandas DataFrames without changing the underlying data. It speeds up your workflow and reduces the risk of running out of memory.
-
-## Installation
-
-```python
-pip install a-pandas-ex-less-memory-more-speed
-```
-
-```python
-from a_pandas_ex_less_memory_more_speed import pd_add_less_memory_more_speed
-pd_add_less_memory_more_speed()
-import pandas as pd
-df = pd.read_csv(    "https://github.com/pandas-dev/pandas/raw/main/doc/data/titanic.csv",)
-df.ds_reduce_memory_size()
-```
-
-## Update 2022/10/08
-
-```python
-#added pandas.Series.ds_optimize_int / pandas.DataFrame.ds_optimize_int
-#to optimize only ints
-
-     PassengerId  Survived  Pclass  ...     Fare Cabin  Embarked
-0              1         0       3  ...   7.2500   NaN         S
-1              2         1       1  ...  71.2833   C85         C
-2              3         1       3  ...   7.9250   NaN         S
-3              4         1       1  ...  53.1000  C123         S
-4              5         0       3  ...   8.0500   NaN         S
-..           ...       ...     ...  ...      ...   ...       ...
-886          887         0       2  ...  13.0000   NaN         S
-887          888         1       1  ...  30.0000   B42         S
-888          889         0       3  ...  23.4500   NaN         S
-889          890         1       1  ...  30.0000  C148         C
-890          891         0       3  ...   7.7500   NaN         Q
-[891 rows x 12 columns]    
-
-
-df.ds_optimize_int()
-df.PassengerId: Using dtype: np.uint16
-df.Survived: Using dtype: np.uint8
-df.Pclass: Using dtype: np.uint8
-df.SibSp: Using dtype: np.uint8
-df.Parch: Using dtype: np.uint8
-Out[7]: 
-     PassengerId  Survived  Pclass  ...     Fare Cabin  Embarked
-0              1         0       3  ...   7.2500   NaN         S
-1              2         1       1  ...  71.2833   C85         C
-2              3         1       3  ...   7.9250   NaN         S
-3              4         1       1  ...  53.1000  C123         S
-4              5         0       3  ...   8.0500   NaN         S
-..           ...       ...     ...  ...      ...   ...       ...
-886          887         0       2  ...  13.0000   NaN         S
-887          888         1       1  ...  30.0000   B42         S
-888          889         0       3  ...  23.4500   NaN         S
-889          890         1       1  ...  30.0000  C148         C
-890          891         0       3  ...   7.7500   NaN         Q
-```
-
-## Usage
-
-```python
-df = pd.read_csv(    "https://github.com/pandas-dev/pandas/raw/main/doc/data/titanic.csv",)
-from random import choice
-
-#Let's add some more data types
-truefalse = lambda: choice([True, False])
-df['truefalse'] = [truefalse() for x in range(len(df))]
-
-df['onlynan'] = pd.NA
-
-df['nestedlists'] = [[[1]*10]] * len(df)
-
-mixedstuff = lambda: choice([True, False, 'right', 'wrong', 1,2,23,343.555,23.444, [442,553,44], [],''])
-df['mixedstuff'] =[mixedstuff() for x in range(len(df))]
-
-floatnumbers = lambda: choice([33.44,344.42424265,15.0,3222.33])
-df['floatnumbers']=[floatnumbers() for x in range(len(df))]
-
-floatnumbers0 = lambda: choice([33.0,344.0,15.0,3222.0])
-df['floatnumbers0']=[floatnumbers0() for x in range(len(df))]
-
-intwithnan = lambda: choice([1,2,3,4,5,pd.NA])
-df['intwithnan']=[intwithnan() for x in range(len(df))]
-
-
-df2 = optimize_dtypes(
-    dframe=df,
-    point_zero_to_int=True,
-    categorylimit=15,
-    verbose=True,
-    include_na_strings_in_pd_na=True,
-    include_empty_iters_in_pd_na=True,
-    include_0_len_string_in_pd_na=True,
-    convert_float=True,
-    check_float_difference=True,
-    float_tolerance_negative=-0.1,
-    float_tolerance_positive=0.1,
-)
-print(df)
-print(df2)
-print(df.dtypes)
-print(df2.dtypes)
-
-
-Memory usage of dataframe is: 0.12333202362060547 MB
-█████████████████████████████
-Analyzing df.PassengerId
-----------------
-df.PassengerId Is numeric!
-df.PassengerId Max: 891
-df.PassengerId Min: 1
-df.PassengerId: Only .000 in columns -> Using int - Checking which size fits best ...
-df.PassengerId: Using dtype: np.uint16
-█████████████████████████████
-Analyzing df.Survived
-----------------
-df.Survived Is numeric!
-df.Survived Max: 1
-df.Survived Min: 0
-df.Survived: Only .000 in columns -> Using int - Checking which size fits best ...
-df.Survived: Using dtype: np.uint8
-█████████████████████████████
-Analyzing df.Pclass
-----------------
-df.Pclass Is numeric!
-df.Pclass Max: 3
-df.Pclass Min: 1
-df.Pclass: Only .000 in columns -> Using int - Checking which size fits best ...
-df.Pclass: Using dtype: np.uint8
-█████████████████████████████
-Analyzing df.Name
-----------------
-df.Name: Using dtype: string
-█████████████████████████████
-Analyzing df.Sex
-----------------
-df.Sex: Using dtype: category
-█████████████████████████████
-Analyzing df.Age
-----------------
-df.Age Is numeric!
-df.Age Max: 80.0
-df.Age Min: 0.42
-df.Age: Using dtype: Float64
-█████████████████████████████
-Analyzing df.SibSp
-----------------
-df.SibSp Is numeric!
-df.SibSp Max: 8
-df.SibSp Min: 0
-df.SibSp: Only .000 in columns -> Using int - Checking which size fits best ...
-df.SibSp: Using dtype: np.uint8
-█████████████████████████████
-Analyzing df.Parch
-----------------
-df.Parch Is numeric!
-df.Parch Max: 6
-df.Parch Min: 0
-df.Parch: Only .000 in columns -> Using int - Checking which size fits best ...
-df.Parch: Using dtype: np.uint8
-█████████████████████████████
-Analyzing df.Ticket
-----------------
-df.Ticket: Using dtype: string
-█████████████████████████████
-Analyzing df.Fare
-----------------
-df.Fare Is numeric!
-df.Fare Max: 512.3292
-df.Fare Min: 0.0
-xxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
-Max. positive difference - limit 0.1
-498   -0.05
-305   -0.05
-708   -0.05
-Max. negative difference - limit -0.1
-679    0.1708
-258    0.1708
-737    0.1708
-xxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
-------------- <class 'numpy.float16'> ------------- not right for df.Fare
-Checking next dtype...
-True -> within the desired range: 0.1 / -0.1
-False      5
-True     886
--------------------
-xxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
-Max. positive difference - limit 0.1
-0      0.0
-587    0.0
-588    0.0
-Max. negative difference - limit -0.1
-0      0.0
-598    0.0
-587    0.0
-xxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
-+++++++++++++ <class 'numpy.float32'> +++++++++++++ right for df.Fare
-True -> within the desired range: 0.1 / -0.1
-True    891
--------------------
-df.Fare: Using dtype: np.float32
-█████████████████████████████
-Analyzing df.Cabin
-----------------
-df.Cabin: Using dtype: string
-█████████████████████████████
-Analyzing df.Embarked
-----------------
-df.Embarked: Using dtype: category
-█████████████████████████████
-Analyzing df.truefalse
-----------------
-df.truefalse: Using dtype: np.bool_
-█████████████████████████████
-Analyzing df.onlynan
-----------------
-df.onlynan Is numeric!
-df.onlynan Max: nan
-df.onlynan Min: nan
-df.onlynan: Only nan in column, continue ...
-█████████████████████████████
-Analyzing df.nestedlists
-----------------
-█████████████████████████████
-Analyzing df.mixedstuff
-----------------
-█████████████████████████████
-Analyzing df.floatnumbers
-----------------
-df.floatnumbers Is numeric!
-df.floatnumbers Max: 3222.33
-df.floatnumbers Min: 15.0
-xxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
-Max. positive difference - limit 0.1
-890   -0.33
-597   -0.33
-592   -0.33
-Max. negative difference - limit -0.1
-527    0.075757
-190    0.075757
-171    0.075757
-xxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
-------------- <class 'numpy.float16'> ------------- not right for df.floatnumbers
-Checking next dtype...
-True -> within the desired range: 0.1 / -0.1
-False    219
-True     672
--------------------
-xxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
-Max. positive difference - limit 0.1
-0      0.0
-587    0.0
-588    0.0
-Max. negative difference - limit -0.1
-0      0.0
-598    0.0
-587    0.0
-xxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
-+++++++++++++ <class 'numpy.float32'> +++++++++++++ right for df.floatnumbers
-True -> within the desired range: 0.1 / -0.1
-True    891
--------------------
-df.floatnumbers: Using dtype: np.float32
-█████████████████████████████
-Analyzing df.floatnumbers0
-----------------
-df.floatnumbers0 Is numeric!
-df.floatnumbers0 Max: 3222.0
-df.floatnumbers0 Min: 15.0
-df.floatnumbers0: Only .000 in columns -> Using int - Checking which size fits best ...
-df.floatnumbers0: Using dtype: np.uint16
-█████████████████████████████
-Analyzing df.intwithnan
-----------------
-df.intwithnan Is numeric!
-df.intwithnan Max: 5
-df.intwithnan Min: 1
-df.intwithnan: Only .000 in columns -> Using int - Checking which size fits best ...
-df.intwithnan: Using dtype: Int64
-█████████████████████████████
-Memory usage of dataframe was: 0.12333202362060547 MB
-Memory usage of dataframe is now: 0.07259273529052734 MB
-This is  58.85959960718511 % of the initial size
-█████████████████████████████
-█████████████████████████████
-     PassengerId  Survived  Pclass  ... floatnumbers floatnumbers0  intwithnan
-0              1         0       3  ...    33.440000          33.0           4
-1              2         1       1  ...  3222.330000          15.0           5
-2              3         1       3  ...    33.440000          33.0           3
-3              4         1       1  ...    15.000000          33.0           1
-4              5         0       3  ...    15.000000         344.0           2
-..           ...       ...     ...  ...          ...           ...         ...
-886          887         0       2  ...   344.424243         344.0           5
-887          888         1       1  ...    15.000000          15.0           4
-888          889         0       3  ...   344.424243        3222.0           2
-889          890         1       1  ...   344.424243        3222.0           4
-890          891         0       3  ...  3222.330000        3222.0        <NA>
-[891 rows x 19 columns]
-     PassengerId  Survived  Pclass  ... floatnumbers floatnumbers0  intwithnan
-0              1         0       3  ...    33.439999            33           4
-1              2         1       1  ...  3222.330078            15           5
-2              3         1       3  ...    33.439999            33           3
-3              4         1       1  ...    15.000000            33           1
-4              5         0       3  ...    15.000000           344           2
-..           ...       ...     ...  ...          ...           ...         ...
-886          887         0       2  ...   344.424255           344           5
-887          888         1       1  ...    15.000000            15           4
-888          889         0       3  ...   344.424255          3222           2
-889          890         1       1  ...   344.424255          3222           4
-890          891         0       3  ...  3222.330078          3222        <NA>
-[891 rows x 19 columns]
-PassengerId        int64
-Survived           int64
-Pclass             int64
-Name              object
-Sex               object
-Age              float64
-SibSp              int64
-Parch              int64
-Ticket            object
-Fare             float64
-Cabin             object
-Embarked          object
-truefalse           bool
-onlynan           object
-nestedlists       object
-mixedstuff        object
-floatnumbers     float64
-floatnumbers0    float64
-intwithnan        object
-dtype: object
-PassengerId        uint16
-Survived            uint8
-Pclass              uint8
-Name               string
-Sex              category
-Age               Float64
-SibSp               uint8
-Parch               uint8
-Ticket             string
-Fare              float32
-Cabin              string
-Embarked         category
-truefalse            bool
-onlynan            object
-nestedlists        object
-mixedstuff         object
-floatnumbers      float32
-floatnumbers0      uint16
-intwithnan          Int64
-dtype: object
-
-    Parameters:
-        dframe: Union[pd.Series, pd.DataFrame]
-            pd.Series, pd.DataFrame
-        point_zero_to_int: bool
-            Convert float to int if all float numbers in the column end with .0+
-            (default = True)
-        categorylimit: int
-            Convert strings to category, when ratio len(df) / len(df.value_counts) >= categorylimit
-            (default = 4)
-        verbose: bool
-            Keep track of what is happening
-            (default = True)
-        include_na_strings_in_pd_na: bool
-            When True -> treated as nan:
-
-            [
-            "<NA>",
-            "<NAN>",
-            "<nan>",
-            "np.nan",
-            "NoneType",
-            "None",
-            "-1.#IND",
-            "1.#QNAN",
-            "1.#IND",
-            "-1.#QNAN",
-            "#N/A N/A",
-            "#N/A",
-            "N/A",
-            "n/a",
-            "NA",
-            "#NA",
-            "NULL",
-            "null",
-            "NaN",
-            "-NaN",
-            "nan",
-            "-nan",
-            ]
-
-            (default =True)
-        include_empty_iters_in_pd_na: bool
-            When True -> [], {} are treated as nan (default = False )
-
-        include_0_len_string_in_pd_na: bool
-            When True -> '' is treated as nan (default = False )
-        convert_float: bool
-            Don't convert columns containing float numbers.
-            Comparing the 2 dataframes from the example, one can see that float numbers frequently
-            don't have the exact same value as the original float number.
-            If decimal digits are important for your work, disable it!
-            (default=True)
-        check_float_difference: bool
-            If a little difference between float dtypes is fine for you, use True
-            Ignored if convert_float=False
-            (default=True)
-        float_tolerance_negative: float
-
-            The negative tolerance you can live with, e.g.
-            3222.330078 - 3222.330000 = 0.000078 is fine for you
-
-            Ignored if convert_float=False
-            (default= 0)
-
-        float_tolerance_positive: float = 0,
-            The positive tolerance you can live with
-            3222.340078 - 3222.330000 = 0.010078 is fine for you
-             Ignored if convert_float=False
-            (default= 0.05)
-
-    Returns:
-        Union[pd.DataFrame, pd.Series]
-```
+## Less memory usage - more speed
+
+A Python package to reduce the memory usage of pandas DataFrames without changing the underlying data. It speeds up your workflow and reduces the risk of running out of memory.
+
+## Installation
+
+```python
+pip install a-pandas-ex-less-memory-more-speed
+```
+
+```python
+from a_pandas_ex_less_memory_more_speed import pd_add_less_memory_more_speed
+pd_add_less_memory_more_speed()
+import pandas as pd
+df = pd.read_csv(    "https://github.com/pandas-dev/pandas/raw/main/doc/data/titanic.csv",)
+df.ds_reduce_memory_size()
+
+```
+
+## Update 2023/05/04
+```python
+
+# to carefully handle callables, iterables and other objects in cells 
+
+df.ds_reduce_memory_size_carefully()
+
+
+    Optimizes the memory usage of a pandas DataFrame or Series by converting data types and reducing memory size.
+
+    Args:
+    df_ (pd.Series | pd.DataFrame): The DataFrame or Series to be optimized.
+    ignore_columns (tuple | list, optional): A tuple or list of column names to ignore during optimization. Defaults to ().
+    not_allowed_to_convert (tuple | list, optional): A tuple or list of modules that should not be converted during optimization. Defaults to ("shapely",).
+    allowed_to_convert (tuple | list, optional): A tuple or list of modules that are allowed to be converted during optimization. Defaults to ("pandas", "numpy").
+    include_empty_iters_in_pd_na (bool, optional): If True, empty iterators will be converted to pd.NA during optimization. Defaults to False.
+    include_0_len_string_in_pd_na (bool, optional): If True, zero-length strings will be converted to pd.NA during optimization. Defaults to False.
+    verbose (bool, optional): If True, print information about the memory usage before and after optimization. Defaults to True.
+
+    Returns:
+    pd.DataFrame | pd.Series: The optimized DataFrame or Series.
+
+    Raises:
+    None.
+    
+    
+```
+
+## Update 2022/10/08
+
+```python
+#added pandas.Series.ds_optimize_int / pandas.DataFrame.ds_optimize_int
+#to optimize only ints
+
+     PassengerId  Survived  Pclass  ...     Fare Cabin  Embarked
+0              1         0       3  ...   7.2500   NaN         S
+1              2         1       1  ...  71.2833   C85         C
+2              3         1       3  ...   7.9250   NaN         S
+3              4         1       1  ...  53.1000  C123         S
+4              5         0       3  ...   8.0500   NaN         S
+..           ...       ...     ...  ...      ...   ...       ...
+886          887         0       2  ...  13.0000   NaN         S
+887          888         1       1  ...  30.0000   B42         S
+888          889         0       3  ...  23.4500   NaN         S
+889          890         1       1  ...  30.0000  C148         C
+890          891         0       3  ...   7.7500   NaN         Q
+[891 rows x 12 columns]    
+
+
+df.ds_optimize_int()
+df.PassengerId: Using dtype: np.uint16
+df.Survived: Using dtype: np.uint8
+df.Pclass: Using dtype: np.uint8
+df.SibSp: Using dtype: np.uint8
+df.Parch: Using dtype: np.uint8
+Out[7]: 
+     PassengerId  Survived  Pclass  ...     Fare Cabin  Embarked
+0              1         0       3  ...   7.2500   NaN         S
+1              2         1       1  ...  71.2833   C85         C
+2              3         1       3  ...   7.9250   NaN         S
+3              4         1       1  ...  53.1000  C123         S
+4              5         0       3  ...   8.0500   NaN         S
+..           ...       ...     ...  ...      ...   ...       ...
+886          887         0       2  ...  13.0000   NaN         S
+887          888         1       1  ...  30.0000   B42         S
+888          889         0       3  ...  23.4500   NaN         S
+889          890         1       1  ...  30.0000  C148         C
+890          891         0       3  ...   7.7500   NaN         Q
+```
+
+## Usage
+
+```python
+df = pd.read_csv(    "https://github.com/pandas-dev/pandas/raw/main/doc/data/titanic.csv",)
+from random import choice
+
+#Let's add some more data types
+truefalse = lambda: choice([True, False])
+df['truefalse'] = [truefalse() for x in range(len(df))]
+
+df['onlynan'] = pd.NA
+
+df['nestedlists'] = [[[1]*10]] * len(df)
+
+mixedstuff = lambda: choice([True, False, 'right', 'wrong', 1,2,23,343.555,23.444, [442,553,44], [],''])
+df['mixedstuff'] =[mixedstuff() for x in range(len(df))]
+
+floatnumbers = lambda: choice([33.44,344.42424265,15.0,3222.33])
+df['floatnumbers']=[floatnumbers() for x in range(len(df))]
+
+floatnumbers0 = lambda: choice([33.0,344.0,15.0,3222.0])
+df['floatnumbers0']=[floatnumbers0() for x in range(len(df))]
+
+intwithnan = lambda: choice([1,2,3,4,5,pd.NA])
+df['intwithnan']=[intwithnan() for x in range(len(df))]
+
+
+df2 = optimize_dtypes(
+    dframe=df,
+    point_zero_to_int=True,
+    categorylimit=15,
+    verbose=True,
+    include_na_strings_in_pd_na=True,
+    include_empty_iters_in_pd_na=True,
+    include_0_len_string_in_pd_na=True,
+    convert_float=True,
+    check_float_difference=True,
+    float_tolerance_negative=-0.1,
+    float_tolerance_positive=0.1,
+)
+print(df)
+print(df2)
+print(df.dtypes)
+print(df2.dtypes)
+
+
+Memory usage of dataframe is: 0.12333202362060547 MB
+█████████████████████████████
+Analyzing df.PassengerId
+----------------
+df.PassengerId Is numeric!
+df.PassengerId Max: 891
+df.PassengerId Min: 1
+df.PassengerId: Only .000 in columns -> Using int - Checking which size fits best ...
+df.PassengerId: Using dtype: np.uint16
+█████████████████████████████
+Analyzing df.Survived
+----------------
+df.Survived Is numeric!
+df.Survived Max: 1
+df.Survived Min: 0
+df.Survived: Only .000 in columns -> Using int - Checking which size fits best ...
+df.Survived: Using dtype: np.uint8
+█████████████████████████████
+Analyzing df.Pclass
+----------------
+df.Pclass Is numeric!
+df.Pclass Max: 3
+df.Pclass Min: 1
+df.Pclass: Only .000 in columns -> Using int - Checking which size fits best ...
+df.Pclass: Using dtype: np.uint8
+█████████████████████████████
+Analyzing df.Name
+----------------
+df.Name: Using dtype: string
+█████████████████████████████
+Analyzing df.Sex
+----------------
+df.Sex: Using dtype: category
+█████████████████████████████
+Analyzing df.Age
+----------------
+df.Age Is numeric!
+df.Age Max: 80.0
+df.Age Min: 0.42
+df.Age: Using dtype: Float64
+█████████████████████████████
+Analyzing df.SibSp
+----------------
+df.SibSp Is numeric!
+df.SibSp Max: 8
+df.SibSp Min: 0
+df.SibSp: Only .000 in columns -> Using int - Checking which size fits best ...
+df.SibSp: Using dtype: np.uint8
+█████████████████████████████
+Analyzing df.Parch
+----------------
+df.Parch Is numeric!
+df.Parch Max: 6
+df.Parch Min: 0
+df.Parch: Only .000 in columns -> Using int - Checking which size fits best ...
+df.Parch: Using dtype: np.uint8
+█████████████████████████████
+Analyzing df.Ticket
+----------------
+df.Ticket: Using dtype: string
+█████████████████████████████
+Analyzing df.Fare
+----------------
+df.Fare Is numeric!
+df.Fare Max: 512.3292
+df.Fare Min: 0.0
+xxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
+Max. positive difference - limit 0.1
+498   -0.05
+305   -0.05
+708   -0.05
+Max. negative difference - limit -0.1
+679    0.1708
+258    0.1708
+737    0.1708
+xxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
+------------- <class 'numpy.float16'> ------------- not right for df.Fare
+Checking next dtype...
+True -> within the desired range: 0.1 / -0.1
+False      5
+True     886
+-------------------
+xxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
+Max. positive difference - limit 0.1
+0      0.0
+587    0.0
+588    0.0
+Max. negative difference - limit -0.1
+0      0.0
+598    0.0
+587    0.0
+xxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
++++++++++++++ <class 'numpy.float32'> +++++++++++++ right for df.Fare
+True -> within the desired range: 0.1 / -0.1
+True    891
+-------------------
+df.Fare: Using dtype: np.float32
+█████████████████████████████
+Analyzing df.Cabin
+----------------
+df.Cabin: Using dtype: string
+█████████████████████████████
+Analyzing df.Embarked
+----------------
+df.Embarked: Using dtype: category
+█████████████████████████████
+Analyzing df.truefalse
+----------------
+df.truefalse: Using dtype: np.bool_
+█████████████████████████████
+Analyzing df.onlynan
+----------------
+df.onlynan Is numeric!
+df.onlynan Max: nan
+df.onlynan Min: nan
+df.onlynan: Only nan in column, continue ...
+█████████████████████████████
+Analyzing df.nestedlists
+----------------
+█████████████████████████████
+Analyzing df.mixedstuff
+----------------
+█████████████████████████████
+Analyzing df.floatnumbers
+----------------
+df.floatnumbers Is numeric!
+df.floatnumbers Max: 3222.33
+df.floatnumbers Min: 15.0
+xxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
+Max. positive difference - limit 0.1
+890   -0.33
+597   -0.33
+592   -0.33
+Max. negative difference - limit -0.1
+527    0.075757
+190    0.075757
+171    0.075757
+xxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
+------------- <class 'numpy.float16'> ------------- not right for df.floatnumbers
+Checking next dtype...
+True -> within the desired range: 0.1 / -0.1
+False    219
+True     672
+-------------------
+xxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
+Max. positive difference - limit 0.1
+0      0.0
+587    0.0
+588    0.0
+Max. negative difference - limit -0.1
+0      0.0
+598    0.0
+587    0.0
+xxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
++++++++++++++ <class 'numpy.float32'> +++++++++++++ right for df.floatnumbers
+True -> within the desired range: 0.1 / -0.1
+True    891
+-------------------
+df.floatnumbers: Using dtype: np.float32
+█████████████████████████████
+Analyzing df.floatnumbers0
+----------------
+df.floatnumbers0 Is numeric!
+df.floatnumbers0 Max: 3222.0
+df.floatnumbers0 Min: 15.0
+df.floatnumbers0: Only .000 in columns -> Using int - Checking which size fits best ...
+df.floatnumbers0: Using dtype: np.uint16
+█████████████████████████████
+Analyzing df.intwithnan
+----------------
+df.intwithnan Is numeric!
+df.intwithnan Max: 5
+df.intwithnan Min: 1
+df.intwithnan: Only .000 in columns -> Using int - Checking which size fits best ...
+df.intwithnan: Using dtype: Int64
+█████████████████████████████
+Memory usage of dataframe was: 0.12333202362060547 MB
+Memory usage of dataframe is now: 0.07259273529052734 MB
+This is  58.85959960718511 % of the initial size
+█████████████████████████████
+█████████████████████████████
+     PassengerId  Survived  Pclass  ... floatnumbers floatnumbers0  intwithnan
+0              1         0       3  ...    33.440000          33.0           4
+1              2         1       1  ...  3222.330000          15.0           5
+2              3         1       3  ...    33.440000          33.0           3
+3              4         1       1  ...    15.000000          33.0           1
+4              5         0       3  ...    15.000000         344.0           2
+..           ...       ...     ...  ...          ...           ...         ...
+886          887         0       2  ...   344.424243         344.0           5
+887          888         1       1  ...    15.000000          15.0           4
+888          889         0       3  ...   344.424243        3222.0           2
+889          890         1       1  ...   344.424243        3222.0           4
+890          891         0       3  ...  3222.330000        3222.0        <NA>
+[891 rows x 19 columns]
+     PassengerId  Survived  Pclass  ... floatnumbers floatnumbers0  intwithnan
+0              1         0       3  ...    33.439999            33           4
+1              2         1       1  ...  3222.330078            15           5
+2              3         1       3  ...    33.439999            33           3
+3              4         1       1  ...    15.000000            33           1
+4              5         0       3  ...    15.000000           344           2
+..           ...       ...     ...  ...          ...           ...         ...
+886          887         0       2  ...   344.424255           344           5
+887          888         1       1  ...    15.000000            15           4
+888          889         0       3  ...   344.424255          3222           2
+889          890         1       1  ...   344.424255          3222           4
+890          891         0       3  ...  3222.330078          3222        <NA>
+[891 rows x 19 columns]
+PassengerId        int64
+Survived           int64
+Pclass             int64
+Name              object
+Sex               object
+Age              float64
+SibSp              int64
+Parch              int64
+Ticket            object
+Fare             float64
+Cabin             object
+Embarked          object
+truefalse           bool
+onlynan           object
+nestedlists       object
+mixedstuff        object
+floatnumbers     float64
+floatnumbers0    float64
+intwithnan        object
+dtype: object
+PassengerId        uint16
+Survived            uint8
+Pclass              uint8
+Name               string
+Sex              category
+Age               Float64
+SibSp               uint8
+Parch               uint8
+Ticket             string
+Fare              float32
+Cabin              string
+Embarked         category
+truefalse            bool
+onlynan            object
+nestedlists        object
+mixedstuff         object
+floatnumbers      float32
+floatnumbers0      uint16
+intwithnan          Int64
+dtype: object
+
+    Parameters:
+        dframe: Union[pd.Series, pd.DataFrame]
+            pd.Series, pd.DataFrame
+        point_zero_to_int: bool
+            Convert float to int if all float numbers in the column end with .0+
+            (default = True)
+        categorylimit: int
+            Convert strings to category, when ratio len(df) / len(df.value_counts) >= categorylimit
+            (default = 4)
+        verbose: bool
+            Keep track of what is happening
+            (default = True)
+        include_na_strings_in_pd_na: bool
+            When True -> treated as nan:
+
+            [
+            "<NA>",
+            "<NAN>",
+            "<nan>",
+            "np.nan",
+            "NoneType",
+            "None",
+            "-1.#IND",
+            "1.#QNAN",
+            "1.#IND",
+            "-1.#QNAN",
+            "#N/A N/A",
+            "#N/A",
+            "N/A",
+            "n/a",
+            "NA",
+            "#NA",
+            "NULL",
+            "null",
+            "NaN",
+            "-NaN",
+            "nan",
+            "-nan",
+            ]
+
+            (default =True)
+        include_empty_iters_in_pd_na: bool
+            When True -> [], {} are treated as nan (default = False )
+
+        include_0_len_string_in_pd_na: bool
+            When True -> '' is treated as nan (default = False )
+        convert_float: bool
+            Don't convert columns containing float numbers.
+            Comparing the 2 dataframes from the example, one can see that float numbers frequently
+            don't have the exact same value as the original float number.
+            If decimal digits are important for your work, disable it!
+            (default=True)
+        check_float_difference: bool
+            If a little difference between float dtypes is fine for you, use True
+            Ignored if convert_float=False
+            (default=True)
+        float_tolerance_negative: float
+
+            The negative tolerance you can live with, e.g.
+            3222.330078 - 3222.330000 = 0.000078 is fine for you
+
+            Ignored if convert_float=False
+            (default= 0)
+
+        float_tolerance_positive: float = 0,
+            The positive tolerance you can live with
+            3222.340078 - 3222.330000 = 0.010078 is fine for you
+             Ignored if convert_float=False
+            (default= 0.05)
+
+    Returns:
+        Union[pd.DataFrame, pd.Series]
+```
```

### Comparing `a_pandas_ex_less_memory_more_speed-0.37/README.md` & `a_pandas_ex_less_memory_more_speed-0.38/a_pandas_ex_less_memory_more_speed/README.MD`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,43 @@
 
 ```python
 from a_pandas_ex_less_memory_more_speed import pd_add_less_memory_more_speed
 pd_add_less_memory_more_speed()
 import pandas as pd
 df = pd.read_csv(    "https://github.com/pandas-dev/pandas/raw/main/doc/data/titanic.csv",)
 df.ds_reduce_memory_size()
+
+```
+
+## Update 2023/05/04
+```python
+
+# to carefully handle callables, iterables and other objects in cells 
+
+df.ds_reduce_memory_size_carefully()
+
+
+    Optimizes the memory usage of a pandas DataFrame or Series by converting data types and reducing memory size.
+
+    Args:
+    df_ (pd.Series | pd.DataFrame): The DataFrame or Series to be optimized.
+    ignore_columns (tuple | list, optional): A tuple or list of column names to ignore during optimization. Defaults to ().
+    not_allowed_to_convert (tuple | list, optional): A tuple or list of modules that should not be converted during optimization. Defaults to ("shapely",).
+    allowed_to_convert (tuple | list, optional): A tuple or list of modules that are allowed to be converted during optimization. Defaults to ("pandas", "numpy").
+    include_empty_iters_in_pd_na (bool, optional): If True, empty iterators will be converted to pd.NA during optimization. Defaults to False.
+    include_0_len_string_in_pd_na (bool, optional): If True, zero-length strings will be converted to pd.NA during optimization. Defaults to False.
+    verbose (bool, optional): If True, print information about the memory usage before and after optimization. Defaults to True.
+
+    Returns:
+    pd.DataFrame | pd.Series: The optimized DataFrame or Series.
+
+    Raises:
+    None.
+    
+    
 ```
 
 ## Update 2022/10/08
 
 ```python
 #added pandas.Series.ds_optimize_int / pandas.DataFrame.ds_optimize_int
 #to optimize only ints
```

### Comparing `a_pandas_ex_less_memory_more_speed-0.37/a_pandas_ex_less_memory_more_speed/LICENSE` & `a_pandas_ex_less_memory_more_speed-0.38/a_pandas_ex_less_memory_more_speed/LICENSE`

 * *Files identical despite different names*

### Comparing `a_pandas_ex_less_memory_more_speed-0.37/a_pandas_ex_less_memory_more_speed/__init__.py` & `a_pandas_ex_less_memory_more_speed-0.38/a_pandas_ex_less_memory_more_speed/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,242 @@
 import operator
 import re
 from typing import Union
 import ast
-import regex
 import numpy as np
 import pandas as pd
-from a_pandas_ex_plode_tool import all_nans_in_df_to_pdNA, qq_s_isnan
+from check_if_nan import is_nan
+from deepcopyall import deepcopy
+from isiter import isiter
 from pandas.core.frame import DataFrame, Series
+from tolerant_isinstance import isinstance_tolerant
+
+
+def qq_s_isnan(
+    wert,
+    nan_back=False,
+    include_na_strings=True,
+    include_empty_iters=False,
+    include_0_len_string=False,
+    *args,
+    **kwargs,
+):
+    isn = is_nan(
+        wert,
+        emptyiters=include_empty_iters,
+        nastrings=include_na_strings,
+        emptystrings=include_0_len_string,
+        emptybytes=False,
+    )
+    if nan_back:
+        if isn:
+            return pd.NA
+        else:
+            return wert
+    return isn
+
+
+def all_nans_in_df_to_pdNA(
+    df: Union[pd.Series, pd.DataFrame],
+    include_na_strings: bool = True,
+    include_empty_iters: bool = False,
+    include_0_len_string: bool = False,
+) -> Union[pd.Series, pd.DataFrame]:
+    isseries = isinstance(df, pd.Series)
+
+    df1 = df.copy()
+    if isseries:
+        df1 = df1.to_frame().copy()
+    for col in df1.columns:
+        df1[col] = df1[col].apply(
+            qq_s_isnan,
+            nan_back=True,
+            include_na_strings=include_na_strings,
+            include_empty_iters=include_empty_iters,
+            include_0_len_string=include_0_len_string,
+        )
+    if isseries:
+        return df1[df1.columns[0]]
+    return df1
+
+
+def optimize_carefully(
+    df_: pd.Series | pd.DataFrame,
+    ignore_columns: tuple | list = (),
+    not_allowed_to_convert: tuple | list = ("shapely",),
+    allowed_to_convert: tuple | list = ("pandas", "numpy"),
+    include_empty_iters_in_pd_na: bool = False,
+    include_0_len_string_in_pd_na: bool = False,
+    verbose: bool = True,
+) -> pd.DataFrame | pd.Series:
+    """
+    Optimizes the memory usage of a pandas DataFrame or Series by converting data types and reducing memory size.
+
+    Args:
+    df_ (pd.Series | pd.DataFrame): The DataFrame or Series to be optimized.
+    ignore_columns (tuple | list, optional): A tuple or list of column names to ignore during optimization. Defaults to ().
+    not_allowed_to_convert (tuple | list, optional): A tuple or list of modules that should not be converted during optimization. Defaults to ("shapely",).
+    allowed_to_convert (tuple | list, optional): A tuple or list of modules that are allowed to be converted during optimization. Defaults to ("pandas", "numpy").
+    include_empty_iters_in_pd_na (bool, optional): If True, empty iterators will be converted to pd.NA during optimization. Defaults to False.
+    include_0_len_string_in_pd_na (bool, optional): If True, zero-length strings will be converted to pd.NA during optimization. Defaults to False.
+    verbose (bool, optional): If True, print information about the memory usage before and after optimization. Defaults to True.
+
+    Returns:
+    pd.DataFrame | pd.Series: The optimized DataFrame or Series.
+
+    Raises:
+    None.
+    """
+    start_mem_usg = df_.memory_usage().sum() / 1024**2
+    df, isseries = series_to_dataframe_no_copy(df_)
+
+    try:
+        copyofdf = df.copy()
+    except Exception:
+        try:
+            copyofdf = deepcopy(df)
+        except Exception:
+            allfr = []
+            for co in df.columns:
+                try:
+                    allfr.append(deepcopy(df[co]))
+                except Exception:
+                    allfr.append(df[co])
+            copyofdf = pd.concat(allfr, axis=1)
+
+    for col in df.columns:
+        if col in ignore_columns:
+            continue
+        try:
+            babanona = df[col].dropna()
+            if not babanona.empty:
+                if isiter(babanona[0], consider_non_iter=(str,)):
+                    continue
+                if callable(babanona[0]):
+                    continue
+                if isinstance_tolerant(babanona[0], (bytes, bytearray)):
+                    continue
+                if not check_if_convert(
+                    babanona[0],
+                    allowed_modules=allowed_to_convert,
+                    not_allowed_modules=not_allowed_to_convert,
+                ):
+                    continue
+
+                if len(q := babanona.unique()) in (1, 2) and (False in q or True in q):
+                    try:
+                        copyofdf[col] = copyofdf[col].astype("bool")
+                        continue
+                    except Exception as fab:
+                        continue
+                if len(q) < 6:
+                    if len(p := set([str(x).strip().lower() for x in q])) in (
+                        1,
+                        2,
+                    ) and ("true" in p or "false" in p):
+                        copyofdf[col] = (
+                            copyofdf[col].ds_to_string().str.lower().str.strip()
+                        )
+                        copyofdf[col] = [
+                            True if h == "true" else False for h in copyofdf[col]
+                        ]
+                        copyofdf[col] = copyofdf[col].astype("bool")
+                        continue
+
+            else:
+                copyofdf[col] = pd.NA
+                continue
+            copyofdf[col] = copyofdf[col].ds_reduce_memory_size(
+                verbose=False,
+                include_empty_iters_in_pd_na=include_empty_iters_in_pd_na,
+                include_0_len_string_in_pd_na=include_0_len_string_in_pd_na,
+            )
+            copyofdf[col] = copyofdf[col].ds_reduce_memory_size(
+                verbose=False,
+                include_empty_iters_in_pd_na=include_empty_iters_in_pd_na,
+                include_0_len_string_in_pd_na=include_0_len_string_in_pd_na,
+            )
+        except Exception as fe:
+            try:
+                copyofdf[col] = copyofdf[col].astype("Float64")
+                if (
+                    copyofdf[col]
+                    .dropna()
+                    .apply(lambda x: pd.NA if x.is_integer() else False)
+                    .dropna()
+                    .empty
+                ):
+                    copyofdf[col] = copyofdf[col].astype("Int64")
+
+            except Exception as fa:
+                continue
+    try:
+        copyofdf = optimize_only_int(copyofdf, verbose=False)
+    except Exception:
+        for co in copyofdf.columns:
+            try:
+                if "int" in str(copyofdf[co].dtype.name).lower():
+                    copyofdf[co] = optimize_only_int(copyofdf[co], verbose=False)
+            except Exception:
+                continue
+
+    if verbose:
+        print("█████████████████████████████")
+
+        mem_usg = copyofdf.memory_usage().sum() / 1024**2
+        print(f"Memory usage of dataframe was: {start_mem_usg} MB")
+        print(f"Memory usage of dataframe is now: {mem_usg} MB")
+        print("This is ", 100 * mem_usg / start_mem_usg, "% of the initial size")
+        print("█████████████████████████████")
+        print("█████████████████████████████\n")
+
+    if isseries:
+        return copyofdf[copyofdf.columns[0]]
+
+    return copyofdf
+
+
+def series_to_dataframe_no_copy(
+    df: Union[pd.Series, pd.DataFrame]
+) -> (Union[pd.Series, pd.DataFrame], bool):
+    dataf = df
+    isseries = False
+    if isinstance(dataf, pd.Series):
+        columnname = dataf.name
+        dataf = dataf.to_frame()
+
+        try:
+            dataf.columns = [columnname]
+        except Exception:
+            dataf.index = [columnname]
+            dataf = dataf.T
+        isseries = True
+
+    return dataf, isseries
+
+
+def check_if_convert(
+    value, allowed_modules=("pandas", "numpy"), not_allowed_modules=("shapely",)
+):
+    modu = str(value.__class__.__module__).lower().split(".")[0]
+    if modu in not_allowed_modules:
+        return False
+
+    try:
+        if modu in allowed_modules:
+            return True
+    except Exception:
+        pass
+
+    try:
+        if not hasattr(value, "__dict__"):
+            return True
+
+    except Exception:
+        return False
 
 
 def check_floats(
     df: pd.DataFrame,
     col: str,
     check_float_difference: bool,
     float_tolerance_negative: float,
@@ -104,398 +330,397 @@
     convert_float: bool = True,
     check_float_difference: bool = True,
     float_tolerance_negative: float = 0,
     float_tolerance_positive: float = 0,
 ) -> Union[pd.Series, pd.DataFrame]:
     """
 
-    How to use
-
-df = pd.read_csv(    "https://github.com/pandas-dev/pandas/raw/main/doc/data/titanic.csv",)
-from random import choice
+        How to use
 
-#Let's add some more data types
-truefalse = lambda: choice([True, False])
-df['truefalse'] = [truefalse() for x in range(len(df))]
+    df = pd.read_csv(    "https://github.com/pandas-dev/pandas/raw/main/doc/data/titanic.csv",)
+    from random import choice
 
-df['onlynan'] = pd.NA
-
-df['nestedlists'] = [[[1]*10]] * len(df)
-
-mixedstuff = lambda: choice([True, False, 'right', 'wrong', 1,2,23,343.555,23.444, [442,553,44], [],''])
-df['mixedstuff'] =[mixedstuff() for x in range(len(df))]
-
-floatnumbers = lambda: choice([33.44,344.42424265,15.0,3222.33])
-df['floatnumbers']=[floatnumbers() for x in range(len(df))]
-
-floatnumbers0 = lambda: choice([33.0,344.0,15.0,3222.0])
-df['floatnumbers0']=[floatnumbers0() for x in range(len(df))]
-
-intwithnan = lambda: choice([1,2,3,4,5,pd.NA])
-df['intwithnan']=[intwithnan() for x in range(len(df))]
+    #Let's add some more data types
+    truefalse = lambda: choice([True, False])
+    df['truefalse'] = [truefalse() for x in range(len(df))]
+
+    df['onlynan'] = pd.NA
+
+    df['nestedlists'] = [[[1]*10]] * len(df)
+
+    mixedstuff = lambda: choice([True, False, 'right', 'wrong', 1,2,23,343.555,23.444, [442,553,44], [],''])
+    df['mixedstuff'] =[mixedstuff() for x in range(len(df))]
+
+    floatnumbers = lambda: choice([33.44,344.42424265,15.0,3222.33])
+    df['floatnumbers']=[floatnumbers() for x in range(len(df))]
+
+    floatnumbers0 = lambda: choice([33.0,344.0,15.0,3222.0])
+    df['floatnumbers0']=[floatnumbers0() for x in range(len(df))]
+
+    intwithnan = lambda: choice([1,2,3,4,5,pd.NA])
+    df['intwithnan']=[intwithnan() for x in range(len(df))]
+
+
+    df2 = optimize_dtypes(
+        dframe=df,
+        point_zero_to_int=True,
+        categorylimit=15,
+        verbose=True,
+        include_na_strings_in_pd_na=True,
+        include_empty_iters_in_pd_na=True,
+        include_0_len_string_in_pd_na=True,
+        convert_float=True,
+        check_float_difference=True,
+        float_tolerance_negative=-0.1,
+        float_tolerance_positive=0.1,
+    )
+    print(df)
+    print(df2)
+    print(df.dtypes)
+    print(df2.dtypes)
+
+
+    Memory usage of dataframe is: 0.12333202362060547 MB
+    █████████████████████████████
+    Analyzing df.PassengerId
+    ----------------
+    df.PassengerId Is numeric!
+    df.PassengerId Max: 891
+    df.PassengerId Min: 1
+    df.PassengerId: Only .000 in columns -> Using int - Checking which size fits best ...
+    df.PassengerId: Using dtype: np.uint16
+    █████████████████████████████
+    Analyzing df.Survived
+    ----------------
+    df.Survived Is numeric!
+    df.Survived Max: 1
+    df.Survived Min: 0
+    df.Survived: Only .000 in columns -> Using int - Checking which size fits best ...
+    df.Survived: Using dtype: np.uint8
+    █████████████████████████████
+    Analyzing df.Pclass
+    ----------------
+    df.Pclass Is numeric!
+    df.Pclass Max: 3
+    df.Pclass Min: 1
+    df.Pclass: Only .000 in columns -> Using int - Checking which size fits best ...
+    df.Pclass: Using dtype: np.uint8
+    █████████████████████████████
+    Analyzing df.Name
+    ----------------
+    df.Name: Using dtype: string
+    █████████████████████████████
+    Analyzing df.Sex
+    ----------------
+    df.Sex: Using dtype: category
+    █████████████████████████████
+    Analyzing df.Age
+    ----------------
+    df.Age Is numeric!
+    df.Age Max: 80.0
+    df.Age Min: 0.42
+    df.Age: Using dtype: Float64
+    █████████████████████████████
+    Analyzing df.SibSp
+    ----------------
+    df.SibSp Is numeric!
+    df.SibSp Max: 8
+    df.SibSp Min: 0
+    df.SibSp: Only .000 in columns -> Using int - Checking which size fits best ...
+    df.SibSp: Using dtype: np.uint8
+    █████████████████████████████
+    Analyzing df.Parch
+    ----------------
+    df.Parch Is numeric!
+    df.Parch Max: 6
+    df.Parch Min: 0
+    df.Parch: Only .000 in columns -> Using int - Checking which size fits best ...
+    df.Parch: Using dtype: np.uint8
+    █████████████████████████████
+    Analyzing df.Ticket
+    ----------------
+    df.Ticket: Using dtype: string
+    █████████████████████████████
+    Analyzing df.Fare
+    ----------------
+    df.Fare Is numeric!
+    df.Fare Max: 512.3292
+    df.Fare Min: 0.0
+    xxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
+    Max. positive difference - limit 0.1
+    498   -0.05
+    305   -0.05
+    708   -0.05
+    Max. negative difference - limit -0.1
+    679    0.1708
+    258    0.1708
+    737    0.1708
+    xxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
+    ------------- <class 'numpy.float16'> ------------- not right for df.Fare
+    Checking next dtype...
+    True -> within the desired range: 0.1 / -0.1
+    False      5
+    True     886
+    -------------------
+    xxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
+    Max. positive difference - limit 0.1
+    0      0.0
+    587    0.0
+    588    0.0
+    Max. negative difference - limit -0.1
+    0      0.0
+    598    0.0
+    587    0.0
+    xxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
+    +++++++++++++ <class 'numpy.float32'> +++++++++++++ right for df.Fare
+    True -> within the desired range: 0.1 / -0.1
+    True    891
+    -------------------
+    df.Fare: Using dtype: np.float32
+    █████████████████████████████
+    Analyzing df.Cabin
+    ----------------
+    df.Cabin: Using dtype: string
+    █████████████████████████████
+    Analyzing df.Embarked
+    ----------------
+    df.Embarked: Using dtype: category
+    █████████████████████████████
+    Analyzing df.truefalse
+    ----------------
+    df.truefalse: Using dtype: np.bool_
+    █████████████████████████████
+    Analyzing df.onlynan
+    ----------------
+    df.onlynan Is numeric!
+    df.onlynan Max: nan
+    df.onlynan Min: nan
+    df.onlynan: Only nan in column, continue ...
+    █████████████████████████████
+    Analyzing df.nestedlists
+    ----------------
+    █████████████████████████████
+    Analyzing df.mixedstuff
+    ----------------
+    █████████████████████████████
+    Analyzing df.floatnumbers
+    ----------------
+    df.floatnumbers Is numeric!
+    df.floatnumbers Max: 3222.33
+    df.floatnumbers Min: 15.0
+    xxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
+    Max. positive difference - limit 0.1
+    890   -0.33
+    597   -0.33
+    592   -0.33
+    Max. negative difference - limit -0.1
+    527    0.075757
+    190    0.075757
+    171    0.075757
+    xxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
+    ------------- <class 'numpy.float16'> ------------- not right for df.floatnumbers
+    Checking next dtype...
+    True -> within the desired range: 0.1 / -0.1
+    False    219
+    True     672
+    -------------------
+    xxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
+    Max. positive difference - limit 0.1
+    0      0.0
+    587    0.0
+    588    0.0
+    Max. negative difference - limit -0.1
+    0      0.0
+    598    0.0
+    587    0.0
+    xxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
+    +++++++++++++ <class 'numpy.float32'> +++++++++++++ right for df.floatnumbers
+    True -> within the desired range: 0.1 / -0.1
+    True    891
+    -------------------
+    df.floatnumbers: Using dtype: np.float32
+    █████████████████████████████
+    Analyzing df.floatnumbers0
+    ----------------
+    df.floatnumbers0 Is numeric!
+    df.floatnumbers0 Max: 3222.0
+    df.floatnumbers0 Min: 15.0
+    df.floatnumbers0: Only .000 in columns -> Using int - Checking which size fits best ...
+    df.floatnumbers0: Using dtype: np.uint16
+    █████████████████████████████
+    Analyzing df.intwithnan
+    ----------------
+    df.intwithnan Is numeric!
+    df.intwithnan Max: 5
+    df.intwithnan Min: 1
+    df.intwithnan: Only .000 in columns -> Using int - Checking which size fits best ...
+    df.intwithnan: Using dtype: Int64
+    █████████████████████████████
+    Memory usage of dataframe was: 0.12333202362060547 MB
+    Memory usage of dataframe is now: 0.07259273529052734 MB
+    This is  58.85959960718511 % of the initial size
+    █████████████████████████████
+    █████████████████████████████
+         PassengerId  Survived  Pclass  ... floatnumbers floatnumbers0  intwithnan
+    0              1         0       3  ...    33.440000          33.0           4
+    1              2         1       1  ...  3222.330000          15.0           5
+    2              3         1       3  ...    33.440000          33.0           3
+    3              4         1       1  ...    15.000000          33.0           1
+    4              5         0       3  ...    15.000000         344.0           2
+    ..           ...       ...     ...  ...          ...           ...         ...
+    886          887         0       2  ...   344.424243         344.0           5
+    887          888         1       1  ...    15.000000          15.0           4
+    888          889         0       3  ...   344.424243        3222.0           2
+    889          890         1       1  ...   344.424243        3222.0           4
+    890          891         0       3  ...  3222.330000        3222.0        <NA>
+    [891 rows x 19 columns]
+         PassengerId  Survived  Pclass  ... floatnumbers floatnumbers0  intwithnan
+    0              1         0       3  ...    33.439999            33           4
+    1              2         1       1  ...  3222.330078            15           5
+    2              3         1       3  ...    33.439999            33           3
+    3              4         1       1  ...    15.000000            33           1
+    4              5         0       3  ...    15.000000           344           2
+    ..           ...       ...     ...  ...          ...           ...         ...
+    886          887         0       2  ...   344.424255           344           5
+    887          888         1       1  ...    15.000000            15           4
+    888          889         0       3  ...   344.424255          3222           2
+    889          890         1       1  ...   344.424255          3222           4
+    890          891         0       3  ...  3222.330078          3222        <NA>
+    [891 rows x 19 columns]
+    PassengerId        int64
+    Survived           int64
+    Pclass             int64
+    Name              object
+    Sex               object
+    Age              float64
+    SibSp              int64
+    Parch              int64
+    Ticket            object
+    Fare             float64
+    Cabin             object
+    Embarked          object
+    truefalse           bool
+    onlynan           object
+    nestedlists       object
+    mixedstuff        object
+    floatnumbers     float64
+    floatnumbers0    float64
+    intwithnan        object
+    dtype: object
+    PassengerId        uint16
+    Survived            uint8
+    Pclass              uint8
+    Name               string
+    Sex              category
+    Age               Float64
+    SibSp               uint8
+    Parch               uint8
+    Ticket             string
+    Fare              float32
+    Cabin              string
+    Embarked         category
+    truefalse            bool
+    onlynan            object
+    nestedlists        object
+    mixedstuff         object
+    floatnumbers      float32
+    floatnumbers0      uint16
+    intwithnan          Int64
+    dtype: object
 
+        Parameters:
+            dframe: Union[pd.Series, pd.DataFrame]
+                pd.Series, pd.DataFrame
+            point_zero_to_int: bool
+                Convert float to int if all float numbers end with .0+
+                (default = True)
+            categorylimit: int
+                Convert strings to category, when ratio len(df) / len(df.value_counts) >= categorylimit
+                (default = 4)
+            verbose: bool
+                Keep track of what is happening
+                (default = True)
+            include_na_strings_in_pd_na: bool
+                When True -> treated as nan:
 
-df2 = optimize_dtypes(
-    dframe=df,
-    point_zero_to_int=True,
-    categorylimit=15,
-    verbose=True,
-    include_na_strings_in_pd_na=True,
-    include_empty_iters_in_pd_na=True,
-    include_0_len_string_in_pd_na=True,
-    convert_float=True,
-    check_float_difference=True,
-    float_tolerance_negative=-0.1,
-    float_tolerance_positive=0.1,
-)
-print(df)
-print(df2)
-print(df.dtypes)
-print(df2.dtypes)
-
-
-Memory usage of dataframe is: 0.12333202362060547 MB
-█████████████████████████████
-Analyzing df.PassengerId
-----------------
-df.PassengerId Is numeric!
-df.PassengerId Max: 891
-df.PassengerId Min: 1
-df.PassengerId: Only .000 in columns -> Using int - Checking which size fits best ...
-df.PassengerId: Using dtype: np.uint16
-█████████████████████████████
-Analyzing df.Survived
-----------------
-df.Survived Is numeric!
-df.Survived Max: 1
-df.Survived Min: 0
-df.Survived: Only .000 in columns -> Using int - Checking which size fits best ...
-df.Survived: Using dtype: np.uint8
-█████████████████████████████
-Analyzing df.Pclass
-----------------
-df.Pclass Is numeric!
-df.Pclass Max: 3
-df.Pclass Min: 1
-df.Pclass: Only .000 in columns -> Using int - Checking which size fits best ...
-df.Pclass: Using dtype: np.uint8
-█████████████████████████████
-Analyzing df.Name
-----------------
-df.Name: Using dtype: string
-█████████████████████████████
-Analyzing df.Sex
-----------------
-df.Sex: Using dtype: category
-█████████████████████████████
-Analyzing df.Age
-----------------
-df.Age Is numeric!
-df.Age Max: 80.0
-df.Age Min: 0.42
-df.Age: Using dtype: Float64
-█████████████████████████████
-Analyzing df.SibSp
-----------------
-df.SibSp Is numeric!
-df.SibSp Max: 8
-df.SibSp Min: 0
-df.SibSp: Only .000 in columns -> Using int - Checking which size fits best ...
-df.SibSp: Using dtype: np.uint8
-█████████████████████████████
-Analyzing df.Parch
-----------------
-df.Parch Is numeric!
-df.Parch Max: 6
-df.Parch Min: 0
-df.Parch: Only .000 in columns -> Using int - Checking which size fits best ...
-df.Parch: Using dtype: np.uint8
-█████████████████████████████
-Analyzing df.Ticket
-----------------
-df.Ticket: Using dtype: string
-█████████████████████████████
-Analyzing df.Fare
-----------------
-df.Fare Is numeric!
-df.Fare Max: 512.3292
-df.Fare Min: 0.0
-xxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
-Max. positive difference - limit 0.1
-498   -0.05
-305   -0.05
-708   -0.05
-Max. negative difference - limit -0.1
-679    0.1708
-258    0.1708
-737    0.1708
-xxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
-------------- <class 'numpy.float16'> ------------- not right for df.Fare
-Checking next dtype...
-True -> within the desired range: 0.1 / -0.1
-False      5
-True     886
--------------------
-xxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
-Max. positive difference - limit 0.1
-0      0.0
-587    0.0
-588    0.0
-Max. negative difference - limit -0.1
-0      0.0
-598    0.0
-587    0.0
-xxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
-+++++++++++++ <class 'numpy.float32'> +++++++++++++ right for df.Fare
-True -> within the desired range: 0.1 / -0.1
-True    891
--------------------
-df.Fare: Using dtype: np.float32
-█████████████████████████████
-Analyzing df.Cabin
-----------------
-df.Cabin: Using dtype: string
-█████████████████████████████
-Analyzing df.Embarked
-----------------
-df.Embarked: Using dtype: category
-█████████████████████████████
-Analyzing df.truefalse
-----------------
-df.truefalse: Using dtype: np.bool_
-█████████████████████████████
-Analyzing df.onlynan
-----------------
-df.onlynan Is numeric!
-df.onlynan Max: nan
-df.onlynan Min: nan
-df.onlynan: Only nan in column, continue ...
-█████████████████████████████
-Analyzing df.nestedlists
-----------------
-█████████████████████████████
-Analyzing df.mixedstuff
-----------------
-█████████████████████████████
-Analyzing df.floatnumbers
-----------------
-df.floatnumbers Is numeric!
-df.floatnumbers Max: 3222.33
-df.floatnumbers Min: 15.0
-xxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
-Max. positive difference - limit 0.1
-890   -0.33
-597   -0.33
-592   -0.33
-Max. negative difference - limit -0.1
-527    0.075757
-190    0.075757
-171    0.075757
-xxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
-------------- <class 'numpy.float16'> ------------- not right for df.floatnumbers
-Checking next dtype...
-True -> within the desired range: 0.1 / -0.1
-False    219
-True     672
--------------------
-xxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
-Max. positive difference - limit 0.1
-0      0.0
-587    0.0
-588    0.0
-Max. negative difference - limit -0.1
-0      0.0
-598    0.0
-587    0.0
-xxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
-+++++++++++++ <class 'numpy.float32'> +++++++++++++ right for df.floatnumbers
-True -> within the desired range: 0.1 / -0.1
-True    891
--------------------
-df.floatnumbers: Using dtype: np.float32
-█████████████████████████████
-Analyzing df.floatnumbers0
-----------------
-df.floatnumbers0 Is numeric!
-df.floatnumbers0 Max: 3222.0
-df.floatnumbers0 Min: 15.0
-df.floatnumbers0: Only .000 in columns -> Using int - Checking which size fits best ...
-df.floatnumbers0: Using dtype: np.uint16
-█████████████████████████████
-Analyzing df.intwithnan
-----------------
-df.intwithnan Is numeric!
-df.intwithnan Max: 5
-df.intwithnan Min: 1
-df.intwithnan: Only .000 in columns -> Using int - Checking which size fits best ...
-df.intwithnan: Using dtype: Int64
-█████████████████████████████
-Memory usage of dataframe was: 0.12333202362060547 MB
-Memory usage of dataframe is now: 0.07259273529052734 MB
-This is  58.85959960718511 % of the initial size
-█████████████████████████████
-█████████████████████████████
-     PassengerId  Survived  Pclass  ... floatnumbers floatnumbers0  intwithnan
-0              1         0       3  ...    33.440000          33.0           4
-1              2         1       1  ...  3222.330000          15.0           5
-2              3         1       3  ...    33.440000          33.0           3
-3              4         1       1  ...    15.000000          33.0           1
-4              5         0       3  ...    15.000000         344.0           2
-..           ...       ...     ...  ...          ...           ...         ...
-886          887         0       2  ...   344.424243         344.0           5
-887          888         1       1  ...    15.000000          15.0           4
-888          889         0       3  ...   344.424243        3222.0           2
-889          890         1       1  ...   344.424243        3222.0           4
-890          891         0       3  ...  3222.330000        3222.0        <NA>
-[891 rows x 19 columns]
-     PassengerId  Survived  Pclass  ... floatnumbers floatnumbers0  intwithnan
-0              1         0       3  ...    33.439999            33           4
-1              2         1       1  ...  3222.330078            15           5
-2              3         1       3  ...    33.439999            33           3
-3              4         1       1  ...    15.000000            33           1
-4              5         0       3  ...    15.000000           344           2
-..           ...       ...     ...  ...          ...           ...         ...
-886          887         0       2  ...   344.424255           344           5
-887          888         1       1  ...    15.000000            15           4
-888          889         0       3  ...   344.424255          3222           2
-889          890         1       1  ...   344.424255          3222           4
-890          891         0       3  ...  3222.330078          3222        <NA>
-[891 rows x 19 columns]
-PassengerId        int64
-Survived           int64
-Pclass             int64
-Name              object
-Sex               object
-Age              float64
-SibSp              int64
-Parch              int64
-Ticket            object
-Fare             float64
-Cabin             object
-Embarked          object
-truefalse           bool
-onlynan           object
-nestedlists       object
-mixedstuff        object
-floatnumbers     float64
-floatnumbers0    float64
-intwithnan        object
-dtype: object
-PassengerId        uint16
-Survived            uint8
-Pclass              uint8
-Name               string
-Sex              category
-Age               Float64
-SibSp               uint8
-Parch               uint8
-Ticket             string
-Fare              float32
-Cabin              string
-Embarked         category
-truefalse            bool
-onlynan            object
-nestedlists        object
-mixedstuff         object
-floatnumbers      float32
-floatnumbers0      uint16
-intwithnan          Int64
-dtype: object
-
-    Parameters:
-        dframe: Union[pd.Series, pd.DataFrame]
-            pd.Series, pd.DataFrame
-        point_zero_to_int: bool
-            Convert float to int if all float numbers end with .0+
-            (default = True)
-        categorylimit: int
-            Convert strings to category, when ratio len(df) / len(df.value_counts) >= categorylimit
-            (default = 4)
-        verbose: bool
-            Keep track of what is happening
-            (default = True)
-        include_na_strings_in_pd_na: bool
-            When True -> treated as nan:
-
-            [
-            "<NA>",
-            "<NAN>",
-            "<nan>",
-            "np.nan",
-            "NoneType",
-            "None",
-            "-1.#IND",
-            "1.#QNAN",
-            "1.#IND",
-            "-1.#QNAN",
-            "#N/A N/A",
-            "#N/A",
-            "N/A",
-            "n/a",
-            "NA",
-            "#NA",
-            "NULL",
-            "null",
-            "NaN",
-            "-NaN",
-            "nan",
-            "-nan",
-            ]
-
-            (default =True)
-        include_empty_iters_in_pd_na: bool
-            When True -> [], {} are treated as nan (default = False )
-
-        include_0_len_string_in_pd_na: bool
-            When True -> '' is treated as nan (default = False )
-        convert_float: bool
-            Don't convert columns containing float numbers.
-            Comparing the 2 dataframes from the example, one can see that float numbers frequently
-            don't have the exact same value as the original float number.
-            If decimal digits are important for your work, disable it!
-            (default=True)
-        check_float_difference: bool
-            If a little difference between float dtypes is fine for you, use True
-            Ignored if convert_float=False
-            (default=True)
-        float_tolerance_negative: float
-
-            The negative tolerance you can live with, e.g.
-            3222.330078 - 3222.330000 = 0.000078 is fine for you
-
-            Ignored if convert_float=False
-            (default= 0)
-
-        float_tolerance_positive: float = 0,
-            The positive tolerance you can live with
-            3222.340078 - 3222.330000 = 0.010078 is fine for you
-             Ignored if convert_float=False
-            (default= 0.05)
+                [
+                "<NA>",
+                "<NAN>",
+                "<nan>",
+                "np.nan",
+                "NoneType",
+                "None",
+                "-1.#IND",
+                "1.#QNAN",
+                "1.#IND",
+                "-1.#QNAN",
+                "#N/A N/A",
+                "#N/A",
+                "N/A",
+                "n/a",
+                "NA",
+                "#NA",
+                "NULL",
+                "null",
+                "NaN",
+                "-NaN",
+                "nan",
+                "-nan",
+                ]
+
+                (default =True)
+            include_empty_iters_in_pd_na: bool
+                When True -> [], {} are treated as nan (default = False )
+
+            include_0_len_string_in_pd_na: bool
+                When True -> '' is treated as nan (default = False )
+            convert_float: bool
+                Don't convert columns containing float numbers.
+                Comparing the 2 dataframes from the example, one can see that float numbers frequently
+                don't have the exact same value as the original float number.
+                If decimal digits are important for your work, disable it!
+                (default=True)
+            check_float_difference: bool
+                If a little difference between float dtypes is fine for you, use True
+                Ignored if convert_float=False
+                (default=True)
+            float_tolerance_negative: float
+
+                The negative tolerance you can live with, e.g.
+                3222.330078 - 3222.330000 = 0.000078 is fine for you
+
+                Ignored if convert_float=False
+                (default= 0)
+
+            float_tolerance_positive: float = 0,
+                The positive tolerance you can live with
+                3222.340078 - 3222.330000 = 0.010078 is fine for you
+                 Ignored if convert_float=False
+                (default= 0.05)
 
-    Returns:
-        Union[pd.DataFrame, pd.Series]
+        Returns:
+            Union[pd.DataFrame, pd.Series]
 
     """
     # df = dframe.copy()
     df, isseries = series_to_dataframe(dframe)
     # isseries = isinstance(df, pd.Series)
     # if isseries:
     #     df = df.to_frame().copy()
     df = all_nans_in_df_to_pdNA(
         df,
         include_na_strings=include_na_strings_in_pd_na,
         include_empty_iters=include_empty_iters_in_pd_na,
         include_0_len_string=include_0_len_string_in_pd_na,
     )  # to only have <NA> not (NaN or nan) to compare strings and to use Int64
-    start_mem_usg = df.memory_usage().sum() / 1024 ** 2
+    start_mem_usg = df.memory_usage().sum() / 1024**2
 
     if verbose:
         print(f"Memory usage of dataframe is: {start_mem_usg} MB")
     for col in df.columns:
-
         dropped = df[col].drop_duplicates().astype("string")  # Saves time
         dropped_nonan = dropped.loc[
             ~dropped.str.contains(r"^\b<NA>\b$", regex=True)
         ]  # to know which column is number
 
         dropped_numeric_nan_ = dropped_nonan.str.replace(".", "", regex=False).map(
             lambda x: str(x).isnumeric()
@@ -529,19 +754,19 @@
                         nan_back=False,
                         include_na_strings=include_na_strings_in_pd_na,
                         include_empty_iters=include_empty_iters_in_pd_na,
                         include_0_len_string=include_0_len_string_in_pd_na,
                     ):
                         df[col] = pd.NA
                         if verbose:
-                            print(fr"df.{col}: Only nan in column, continue ...")
+                            print(rf"df.{col}: Only nan in column, continue ...")
                         continue
                     if verbose:
                         print(
-                            fr"df.{col}: Only .000 in columns -> Using int - Checking which size fits best ..."
+                            rf"df.{col}: Only .000 in columns -> Using int - Checking which size fits best ..."
                         )
                 else:
                     isfloat = True
             else:
                 isfloat = "." in dropped.to_string(index=False, header=False)
                 if isfloat:
                     if verbose:
@@ -596,73 +821,63 @@
                         if verbose and converted_successfully:
                             print(f"df.{col}: Using dtype: np.float32")
 
                     if converted_successfully is False:
                         df[col] = df[col].astype(np.float64)
                         # converted_successfully = True
                         if verbose:
-
                             print(f"df.{col}: Using dtype: np.float64")
 
                 except Exception as ba:
-
                     if verbose:
                         print(f"df.{col}: Using dtype: Float64")
                     df[col] = df[col].astype("Float64")
                     # converted_successfully = True
 
             else:
                 try:
                     if mn >= 0:
                         if mx <= 255:
                             df[col] = df[col].astype(np.uint8)
                             if verbose:
-
                                 print(f"df.{col}: Using dtype: np.uint8")
                         elif mx <= 65535:
                             df[col] = df[col].astype(np.uint16)
                             if verbose:
-
                                 print(f"df.{col}: Using dtype: np.uint16")
                         elif mx <= 4294967295:
                             df[col] = df[col].astype(np.uint32)
                             if verbose:
-
                                 print(f"df.{col}: Using dtype: np.uint32")
                         elif mx > 4294967295:
                             df[col] = df[col].astype(np.uint64)
                             if verbose:
-
                                 print(f"df.{col}: Using dtype: np.uint64")
                     else:
                         if mn > np.iinfo(np.int8).min and mx < np.iinfo(np.int8).max:
                             df[col] = df[col].astype(np.int8)
                             if verbose:
-
                                 print(f"df.{col}: Using dtype: np.int8")
                         elif (
                             mn > np.iinfo(np.int16).min and mx < np.iinfo(np.int16).max
                         ):
                             df[col] = df[col].astype(np.int16)
                             if verbose:
-
                                 print(f"df.{col}: Using dtype: np.int16")
                         elif (
                             mn > np.iinfo(np.int32).min and mx < np.iinfo(np.int32).max
                         ):
                             df[col] = df[col].astype(np.int32)
                             if verbose:
-
                                 print(f"df.{col}: Using dtype: np.int32")
                         elif (
                             mn > np.iinfo(np.int64).min and mx < np.iinfo(np.int64).max
                         ):
                             df[col] = df[col].astype(np.int64)
                             if verbose:
-
                                 print(f"df.{col}: Using dtype: np.int64")
                 except Exception as ba:
                     if verbose:
                         print(f"df.{col}: Using dtype: Int64")
                     df[col] = df[col].astype("Int64")
 
         elif (
@@ -707,15 +922,15 @@
                             print(f"df.{col}: Using dtype: string")
                 except Exception as Fehler:
                     pass
 
     if verbose:
         print("█████████████████████████████")
 
-        mem_usg = df.memory_usage().sum() / 1024 ** 2
+        mem_usg = df.memory_usage().sum() / 1024**2
         print(f"Memory usage of dataframe was: {start_mem_usg} MB")
         print(f"Memory usage of dataframe is now: {mem_usg} MB")
         print("This is ", 100 * mem_usg / start_mem_usg, "% of the initial size")
         print("█████████████████████████████")
         print("█████████████████████████████\n")
 
     if isseries:
@@ -785,15 +1000,14 @@
             Union[pd.DataFrame,pd.Series]
 
     """
     df, isseries = series_to_dataframe(dframe)
 
     def ast_convert(vari):
         if isinstance(vari, str):
-
             try:
                 if vari == "None":
                     return pd.NA
                 return ast.literal_eval(vari)
             except Exception as fe:
                 return qq_s_isnan(
                     wert=vari,
@@ -804,18 +1018,18 @@
                     debug=False,
                 )
 
         return vari
 
     for col in df.columns:
         if (
-            regex.search(
+            re.search(
                 r"(?:category)|(?:string)|(?:object)",
                 str(df[col].dtype),
-                flags=regex.IGNORECASE,
+                flags=re.IGNORECASE,
             )
             is None
         ):
             continue
         df[col] = df[col].map(lambda _: ast_convert(_))
     if isseries:
         return df[df.columns[0]]
@@ -873,17 +1087,17 @@
                 (default = True)
         Returns
             Union[pd.DataFrame,pd.Series]
     """
     df, isseries = series_to_dataframe(dframe)
 
     for col in df.columns:
-        if regex.search(r"(?:[iI]nt)|(?:object)", str(df[col].dtype)) is None:
+        if re.search(r"(?:[iI]nt)|(?:object)", str(df[col].dtype)) is None:
             continue
-        if regex.search(r"^\d+$", str(df[col][0])) is None:
+        if re.search(r"^\d+$", str(df[col][0])) is None:
             continue
         try:
             mx = df[col].max()
             mn = df[col].min()
 
             if mn >= 0:
                 if mx <= 255:
@@ -926,12 +1140,16 @@
     if isseries:
         return df[df.columns[0]]
     return df
 
 
 def pd_add_less_memory_more_speed():
     DataFrame.ds_reduce_memory_size = optimize_dtypes
+    DataFrame.ds_reduce_memory_size_carefully = optimize_carefully
+
     DataFrame.ds_optimize_int = optimize_only_int
     DataFrame.ds_string_to_mixed_dtype = string_to_mixed_dtypes
     Series.ds_reduce_memory_size = optimize_dtypes
+    Series.ds_reduce_memory_size_carefully = optimize_carefully
+
     Series.ds_optimize_int = optimize_only_int
     Series.ds_string_to_mixed_dtype = string_to_mixed_dtypes
```

### Comparing `a_pandas_ex_less_memory_more_speed-0.37/a_pandas_ex_less_memory_more_speed.egg-info/SOURCES.txt` & `a_pandas_ex_less_memory_more_speed-0.38/a_pandas_ex_less_memory_more_speed.egg-info/SOURCES.txt`

 * *Files identical despite different names*

