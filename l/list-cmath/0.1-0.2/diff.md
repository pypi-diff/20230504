# Comparing `tmp/list_cmath-0.1.tar.gz` & `tmp/list_cmath-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "list_cmath-0.1.tar", last modified: Thu May  4 11:04:58 2023, max compression
+gzip compressed data, was "list_cmath-0.2.tar", last modified: Thu May  4 11:10:34 2023, max compression
```

## Comparing `list_cmath-0.1.tar` & `list_cmath-0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-05-04 11:04:58.785654 list_cmath-0.1/
--rw-r--r--   0 mac        (501) staff       (20)     1068 2023-04-30 12:04:30.000000 list_cmath-0.1/LICENSE.txt
--rw-r--r--   0 mac        (501) staff       (20)     4319 2023-05-04 11:04:58.785069 list_cmath-0.1/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)     3903 2023-05-04 11:04:03.000000 list_cmath-0.1/README.md
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-05-04 11:04:58.781004 list_cmath-0.1/list_cmath/
--rw-r--r--   0 mac        (501) staff       (20)     1722 2023-05-03 09:12:13.000000 list_cmath-0.1/list_cmath/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)     1502 2023-05-03 04:52:00.000000 list_cmath-0.1/list_cmath/mandelbrot.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-05-04 11:04:58.784342 list_cmath-0.1/list_cmath.egg-info/
--rw-r--r--   0 mac        (501) staff       (20)     4319 2023-05-04 11:04:58.000000 list_cmath-0.1/list_cmath.egg-info/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)      214 2023-05-04 11:04:58.000000 list_cmath-0.1/list_cmath.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (501) staff       (20)        1 2023-05-04 11:04:58.000000 list_cmath-0.1/list_cmath.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (501) staff       (20)       11 2023-05-04 11:04:58.000000 list_cmath-0.1/list_cmath.egg-info/top_level.txt
--rw-r--r--   0 mac        (501) staff       (20)       38 2023-05-04 11:04:58.785805 list_cmath-0.1/setup.cfg
--rw-r--r--   0 mac        (501) staff       (20)     3359 2023-05-03 04:59:23.000000 list_cmath-0.1/setup.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-05-04 11:10:34.438862 list_cmath-0.2/
+-rw-r--r--   0 mac        (501) staff       (20)     1068 2023-04-30 12:04:30.000000 list_cmath-0.2/LICENSE.txt
+-rw-r--r--   0 mac        (501) staff       (20)     3815 2023-05-04 11:10:34.438429 list_cmath-0.2/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)     3399 2023-05-04 11:09:31.000000 list_cmath-0.2/README.md
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-05-04 11:10:34.435840 list_cmath-0.2/list_cmath/
+-rw-r--r--   0 mac        (501) staff       (20)     1722 2023-05-03 09:12:13.000000 list_cmath-0.2/list_cmath/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)     1502 2023-05-03 04:52:00.000000 list_cmath-0.2/list_cmath/mandelbrot.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-05-04 11:10:34.437832 list_cmath-0.2/list_cmath.egg-info/
+-rw-r--r--   0 mac        (501) staff       (20)     3815 2023-05-04 11:10:34.000000 list_cmath-0.2/list_cmath.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)      214 2023-05-04 11:10:34.000000 list_cmath-0.2/list_cmath.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (501) staff       (20)        1 2023-05-04 11:10:34.000000 list_cmath-0.2/list_cmath.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (501) staff       (20)       11 2023-05-04 11:10:34.000000 list_cmath-0.2/list_cmath.egg-info/top_level.txt
+-rw-r--r--   0 mac        (501) staff       (20)       38 2023-05-04 11:10:34.439013 list_cmath-0.2/setup.cfg
+-rw-r--r--   0 mac        (501) staff       (20)     3359 2023-05-04 11:08:28.000000 list_cmath-0.2/setup.py
```

### Comparing `list_cmath-0.1/LICENSE.txt` & `list_cmath-0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `list_cmath-0.1/PKG-INFO` & `list_cmath-0.2/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: list_cmath
-Version: 0.1
+Version: 0.2
 Summary: Using list to save complex.
 Home-page: https://github.com/JunzePeng/list_cmath
 Author: JunzePeng
 Author-email: gxp@bupt.edu.cn
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -18,109 +18,109 @@
 > Tips: Lists may like this:[0.125,0.625] is equivalent to 0.125+0.625i and python complex (0.125+0.625j).  
 it will be call "complex list" after this tip.
 # functions
 ## ```cAdd(a,b)```
 ### introduction:
 ```cAdd(a,b)``` returns the sum of two complex numbers.
 ### argument:
-```list``````(``````a``````)```: A complex list.  
-```list``````(``````b``````)```: Another complex list.
+```list(a)```: A complex list.  
+```list(b)```: Another complex list.
 ### output
-```list``````(``````<re>``````)```: A complex list.  
+```list(<re>)```: A complex list.  
 > Notes: ```<re>``` means a representation.
 
 ## ```cMult(u,v)```
 ### introduction:
 ```cMult(u,v)``` returns the product of two complex numbers.
 ### argument:
-```list``````(``````u``````)```: A complex list.  
-```list``````(``````v``````)```: Another complex list.
+```list(u)```: A complex list.  
+```list(v)```: Another complex list.
 ### output
-```list``````(``````<re>``````)```: A complex list. 
+```list(<re>)```: A complex list. 
 
 ## ```cPow(x,n)```
 ### introduction:
 ```cPow(x,n)``` returns the n-th power of complex number x.
 ### argument:
-```list``````(``````x``````)```: A complex list.  
-```int``````(``````n``````)```: Power of ```x```.
+```list(x)```: A complex list.  
+```int(n)```: Power of ```x```.
 ### output
-```list``````(``````t``````)```: A complex list. 
+```list(t)```: A complex list. 
 
 ## ```listToComplex(z)```
 ### introduction:
 ```listToComplex(z)``` returns a python buit-in ```complex``` that equal to the input complex list.
 ### argument:
-```list``````(``````x``````)```: A complex list.  
+```list(x)```: A complex list.  
 ### output
-```list``````(``````<re>``````)```: A complex equal to ```x```. 
+```list(<re>)```: A complex equal to ```x```. 
 
 ## ```complexToList(z)```
 ### introduction:
 ```complexToList(z)``` returns a complex list that equal to the input python buit-in ```complex```.
 ### argument:
-```complex``````(``````x``````)```: A complex.  
+```complex(x)```: A complex.  
 ### output
-```list``````(``````<re>``````)```: A complex list equal to ```x```. 
+```list(<re>)```: A complex list equal to ```x```. 
 
 ## ```listsToComplexes(lists)```
 ### introduction:
 ```listsToComplexes(lists)``` returns a list of complex.
 ### argument:
-```list``````(``````lists``````)```: A list of list complex.  
+```list(lists)```: A list of list complex.  
 > Notes: example of "list of list complex":
 > ```python
 > [[0.125,0.75],
 >  [0.625,0.25],
 >  [1.525,25.5]]
 > ```
 
 ### output
-```list``````(``````complexes``````)```: A list of complex,ietms in it are all equal to items in ```lists```. 
+```list(complexes)```: A list of complex,ietms in it are all equal to items in ```lists```. 
 
 ## ```complexesToLists(complexes)```
 ### introduction:
 ```complexesToLists(complexes)``` returns a list of list complex.
 ### argument:
-```list``````(``````complexes``````)```: A list of complex.  
+```list(complexes)```: A list of complex.  
 ### output
-```list``````(``````lists``````)```: A list of list complex,ietms in it are all equal to items in ```complexes```. 
+```list(lists)```: A list of list complex,ietms in it are all equal to items in ```complexes```. 
 
 
 ## ```lcSum(clist)```
 ### introduction:
 ```lSum(clist)``` returns the sum of one-list of complex numbers.
 ### argument:
-```list``````(``````clist``````)```: A list of list complex.  
+```list(clist)```: A list of list complex.  
 ### output
-```list``````(``````<re>``````)```: A list complex. 
+```list(<re>)```: A list complex. 
 
 ## ```lcMult(clist)```
 ### introduction:
 ```lcMult(clist)``` returns the product of one-list of complex numbers.
 ### argument:
-```list``````(``````clist``````)```: A list of list complex.  
+```list(clist)```: A list of list complex.  
 ### output
-```list``````(``````s``````)```: A list complex. 
+```list(s)```: A list complex. 
 
 ## ```lmagnitude(clist)```
 ### introduction:
 ```lmagnitude(clist)``` returns the absolute value of one-list of complex number.
 ### argument:
-```list``````(``````clist``````)```: A list of list complex.  
+```list(clist)```: A list of list complex.  
 ### output
-```list``````(``````r``````)```: A list complex. 
+```list(r)```: A list complex. 
 
 ## ```mandelbrot.mandelbrot(z,num)``` ```mandelbrot.mandelbrot_p(z,num,n)``` ```mandelbrot.mandelbrot_e(z,num,a)```
 ### introduction:
 These funcions retuun the process num times and return the number of diverging times.
 ### argument:
-```list``````(``````z``````)```: A list of list complex.  
-```int``````(``````num``````)```: A list of list complex.  
-```int``````(``````n``````)```: A list of list complex.  
-```string``````(``````a``````)```: A re.
+```list(z)```: A list of list complex.  
+```int(num)```: A list of list complex.  
+```int(n)```: A list of list complex.  
+```string(a)```: A re.
 ### output
-```int``````(``````count``````)```: The number of diverging times. 
+```int(count)```: The number of diverging times. 
 
 # others
 This is the first version of 'list_complex' package,so it may be some bugs.  
 Plese visit ```README.html``` in the package to get colorful options.
```

### Comparing `list_cmath-0.1/README.md` & `list_cmath-0.2/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -3,109 +3,109 @@
 > Tips: Lists may like this:[0.125,0.625] is equivalent to 0.125+0.625i and python complex (0.125+0.625j).  
 it will be call "complex list" after this tip.
 # functions
 ## ```cAdd(a,b)```
 ### introduction:
 ```cAdd(a,b)``` returns the sum of two complex numbers.
 ### argument:
-```list``````(``````a``````)```: A complex list.  
-```list``````(``````b``````)```: Another complex list.
+```list(a)```: A complex list.  
+```list(b)```: Another complex list.
 ### output
-```list``````(``````<re>``````)```: A complex list.  
+```list(<re>)```: A complex list.  
 > Notes: ```<re>``` means a representation.
 
 ## ```cMult(u,v)```
 ### introduction:
 ```cMult(u,v)``` returns the product of two complex numbers.
 ### argument:
-```list``````(``````u``````)```: A complex list.  
-```list``````(``````v``````)```: Another complex list.
+```list(u)```: A complex list.  
+```list(v)```: Another complex list.
 ### output
-```list``````(``````<re>``````)```: A complex list. 
+```list(<re>)```: A complex list. 
 
 ## ```cPow(x,n)```
 ### introduction:
 ```cPow(x,n)``` returns the n-th power of complex number x.
 ### argument:
-```list``````(``````x``````)```: A complex list.  
-```int``````(``````n``````)```: Power of ```x```.
+```list(x)```: A complex list.  
+```int(n)```: Power of ```x```.
 ### output
-```list``````(``````t``````)```: A complex list. 
+```list(t)```: A complex list. 
 
 ## ```listToComplex(z)```
 ### introduction:
 ```listToComplex(z)``` returns a python buit-in ```complex``` that equal to the input complex list.
 ### argument:
-```list``````(``````x``````)```: A complex list.  
+```list(x)```: A complex list.  
 ### output
-```list``````(``````<re>``````)```: A complex equal to ```x```. 
+```list(<re>)```: A complex equal to ```x```. 
 
 ## ```complexToList(z)```
 ### introduction:
 ```complexToList(z)``` returns a complex list that equal to the input python buit-in ```complex```.
 ### argument:
-```complex``````(``````x``````)```: A complex.  
+```complex(x)```: A complex.  
 ### output
-```list``````(``````<re>``````)```: A complex list equal to ```x```. 
+```list(<re>)```: A complex list equal to ```x```. 
 
 ## ```listsToComplexes(lists)```
 ### introduction:
 ```listsToComplexes(lists)``` returns a list of complex.
 ### argument:
-```list``````(``````lists``````)```: A list of list complex.  
+```list(lists)```: A list of list complex.  
 > Notes: example of "list of list complex":
 > ```python
 > [[0.125,0.75],
 >  [0.625,0.25],
 >  [1.525,25.5]]
 > ```
 
 ### output
-```list``````(``````complexes``````)```: A list of complex,ietms in it are all equal to items in ```lists```. 
+```list(complexes)```: A list of complex,ietms in it are all equal to items in ```lists```. 
 
 ## ```complexesToLists(complexes)```
 ### introduction:
 ```complexesToLists(complexes)``` returns a list of list complex.
 ### argument:
-```list``````(``````complexes``````)```: A list of complex.  
+```list(complexes)```: A list of complex.  
 ### output
-```list``````(``````lists``````)```: A list of list complex,ietms in it are all equal to items in ```complexes```. 
+```list(lists)```: A list of list complex,ietms in it are all equal to items in ```complexes```. 
 
 
 ## ```lcSum(clist)```
 ### introduction:
 ```lSum(clist)``` returns the sum of one-list of complex numbers.
 ### argument:
-```list``````(``````clist``````)```: A list of list complex.  
+```list(clist)```: A list of list complex.  
 ### output
-```list``````(``````<re>``````)```: A list complex. 
+```list(<re>)```: A list complex. 
 
 ## ```lcMult(clist)```
 ### introduction:
 ```lcMult(clist)``` returns the product of one-list of complex numbers.
 ### argument:
-```list``````(``````clist``````)```: A list of list complex.  
+```list(clist)```: A list of list complex.  
 ### output
-```list``````(``````s``````)```: A list complex. 
+```list(s)```: A list complex. 
 
 ## ```lmagnitude(clist)```
 ### introduction:
 ```lmagnitude(clist)``` returns the absolute value of one-list of complex number.
 ### argument:
-```list``````(``````clist``````)```: A list of list complex.  
+```list(clist)```: A list of list complex.  
 ### output
-```list``````(``````r``````)```: A list complex. 
+```list(r)```: A list complex. 
 
 ## ```mandelbrot.mandelbrot(z,num)``` ```mandelbrot.mandelbrot_p(z,num,n)``` ```mandelbrot.mandelbrot_e(z,num,a)```
 ### introduction:
 These funcions retuun the process num times and return the number of diverging times.
 ### argument:
-```list``````(``````z``````)```: A list of list complex.  
-```int``````(``````num``````)```: A list of list complex.  
-```int``````(``````n``````)```: A list of list complex.  
-```string``````(``````a``````)```: A re.
+```list(z)```: A list of list complex.  
+```int(num)```: A list of list complex.  
+```int(n)```: A list of list complex.  
+```string(a)```: A re.
 ### output
-```int``````(``````count``````)```: The number of diverging times. 
+```int(count)```: The number of diverging times. 
 
 # others
 This is the first version of 'list_complex' package,so it may be some bugs.  
 Plese visit ```README.html``` in the package to get colorful options.
```

### Comparing `list_cmath-0.1/list_cmath/__init__.py` & `list_cmath-0.2/list_cmath/__init__.py`

 * *Files identical despite different names*

### Comparing `list_cmath-0.1/list_cmath/mandelbrot.py` & `list_cmath-0.2/list_cmath/mandelbrot.py`

 * *Files identical despite different names*

### Comparing `list_cmath-0.1/list_cmath.egg-info/PKG-INFO` & `list_cmath-0.2/list_cmath.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: list-cmath
-Version: 0.1
+Version: 0.2
 Summary: Using list to save complex.
 Home-page: https://github.com/JunzePeng/list_cmath
 Author: JunzePeng
 Author-email: gxp@bupt.edu.cn
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -18,109 +18,109 @@
 > Tips: Lists may like this:[0.125,0.625] is equivalent to 0.125+0.625i and python complex (0.125+0.625j).  
 it will be call "complex list" after this tip.
 # functions
 ## ```cAdd(a,b)```
 ### introduction:
 ```cAdd(a,b)``` returns the sum of two complex numbers.
 ### argument:
-```list``````(``````a``````)```: A complex list.  
-```list``````(``````b``````)```: Another complex list.
+```list(a)```: A complex list.  
+```list(b)```: Another complex list.
 ### output
-```list``````(``````<re>``````)```: A complex list.  
+```list(<re>)```: A complex list.  
 > Notes: ```<re>``` means a representation.
 
 ## ```cMult(u,v)```
 ### introduction:
 ```cMult(u,v)``` returns the product of two complex numbers.
 ### argument:
-```list``````(``````u``````)```: A complex list.  
-```list``````(``````v``````)```: Another complex list.
+```list(u)```: A complex list.  
+```list(v)```: Another complex list.
 ### output
-```list``````(``````<re>``````)```: A complex list. 
+```list(<re>)```: A complex list. 
 
 ## ```cPow(x,n)```
 ### introduction:
 ```cPow(x,n)``` returns the n-th power of complex number x.
 ### argument:
-```list``````(``````x``````)```: A complex list.  
-```int``````(``````n``````)```: Power of ```x```.
+```list(x)```: A complex list.  
+```int(n)```: Power of ```x```.
 ### output
-```list``````(``````t``````)```: A complex list. 
+```list(t)```: A complex list. 
 
 ## ```listToComplex(z)```
 ### introduction:
 ```listToComplex(z)``` returns a python buit-in ```complex``` that equal to the input complex list.
 ### argument:
-```list``````(``````x``````)```: A complex list.  
+```list(x)```: A complex list.  
 ### output
-```list``````(``````<re>``````)```: A complex equal to ```x```. 
+```list(<re>)```: A complex equal to ```x```. 
 
 ## ```complexToList(z)```
 ### introduction:
 ```complexToList(z)``` returns a complex list that equal to the input python buit-in ```complex```.
 ### argument:
-```complex``````(``````x``````)```: A complex.  
+```complex(x)```: A complex.  
 ### output
-```list``````(``````<re>``````)```: A complex list equal to ```x```. 
+```list(<re>)```: A complex list equal to ```x```. 
 
 ## ```listsToComplexes(lists)```
 ### introduction:
 ```listsToComplexes(lists)``` returns a list of complex.
 ### argument:
-```list``````(``````lists``````)```: A list of list complex.  
+```list(lists)```: A list of list complex.  
 > Notes: example of "list of list complex":
 > ```python
 > [[0.125,0.75],
 >  [0.625,0.25],
 >  [1.525,25.5]]
 > ```
 
 ### output
-```list``````(``````complexes``````)```: A list of complex,ietms in it are all equal to items in ```lists```. 
+```list(complexes)```: A list of complex,ietms in it are all equal to items in ```lists```. 
 
 ## ```complexesToLists(complexes)```
 ### introduction:
 ```complexesToLists(complexes)``` returns a list of list complex.
 ### argument:
-```list``````(``````complexes``````)```: A list of complex.  
+```list(complexes)```: A list of complex.  
 ### output
-```list``````(``````lists``````)```: A list of list complex,ietms in it are all equal to items in ```complexes```. 
+```list(lists)```: A list of list complex,ietms in it are all equal to items in ```complexes```. 
 
 
 ## ```lcSum(clist)```
 ### introduction:
 ```lSum(clist)``` returns the sum of one-list of complex numbers.
 ### argument:
-```list``````(``````clist``````)```: A list of list complex.  
+```list(clist)```: A list of list complex.  
 ### output
-```list``````(``````<re>``````)```: A list complex. 
+```list(<re>)```: A list complex. 
 
 ## ```lcMult(clist)```
 ### introduction:
 ```lcMult(clist)``` returns the product of one-list of complex numbers.
 ### argument:
-```list``````(``````clist``````)```: A list of list complex.  
+```list(clist)```: A list of list complex.  
 ### output
-```list``````(``````s``````)```: A list complex. 
+```list(s)```: A list complex. 
 
 ## ```lmagnitude(clist)```
 ### introduction:
 ```lmagnitude(clist)``` returns the absolute value of one-list of complex number.
 ### argument:
-```list``````(``````clist``````)```: A list of list complex.  
+```list(clist)```: A list of list complex.  
 ### output
-```list``````(``````r``````)```: A list complex. 
+```list(r)```: A list complex. 
 
 ## ```mandelbrot.mandelbrot(z,num)``` ```mandelbrot.mandelbrot_p(z,num,n)``` ```mandelbrot.mandelbrot_e(z,num,a)```
 ### introduction:
 These funcions retuun the process num times and return the number of diverging times.
 ### argument:
-```list``````(``````z``````)```: A list of list complex.  
-```int``````(``````num``````)```: A list of list complex.  
-```int``````(``````n``````)```: A list of list complex.  
-```string``````(``````a``````)```: A re.
+```list(z)```: A list of list complex.  
+```int(num)```: A list of list complex.  
+```int(n)```: A list of list complex.  
+```string(a)```: A re.
 ### output
-```int``````(``````count``````)```: The number of diverging times. 
+```int(count)```: The number of diverging times. 
 
 # others
 This is the first version of 'list_complex' package,so it may be some bugs.  
 Plese visit ```README.html``` in the package to get colorful options.
```

### Comparing `list_cmath-0.1/setup.py` & `list_cmath-0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # Package meta-data.
 NAME = 'list_cmath'
 DESCRIPTION = 'Using list to save complex.'
 URL = 'https://github.com/JunzePeng/list_cmath'
 EMAIL = "gxp@bupt.edu.cn"
 AUTHOR = 'JunzePeng'
 REQUIRES_PYTHON = ''
-VERSION = '0.1'
+VERSION = '0.2'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     # 'requests', 'maya', 'records',
 ]
 
 # What packages are optional?
```

