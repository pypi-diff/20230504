# Comparing `tmp/vsrgtools-1.4.3.tar.gz` & `tmp/vsrgtools-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vsrgtools-1.4.3.tar", last modified: Sun Mar 26 17:38:51 2023, max compression
+gzip compressed data, was "vsrgtools-1.4.4.tar", last modified: Thu May  4 21:57:54 2023, max compression
```

## Comparing `vsrgtools-1.4.3.tar` & `vsrgtools-1.4.4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 17:38:51.359207 vsrgtools-1.4.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-03-26 17:38:26.000000 vsrgtools-1.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-03-26 17:38:51.359207 vsrgtools-1.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-03-26 17:38:26.000000 vsrgtools-1.4.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-03-26 17:38:51.359207 vsrgtools-1.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-03-26 17:38:26.000000 vsrgtools-1.4.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 17:38:51.359207 vsrgtools-1.4.3/vsrgtools/
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-03-26 17:38:26.000000 vsrgtools-1.4.3/vsrgtools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-03-26 17:38:26.000000 vsrgtools-1.4.3/vsrgtools/_metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 17:38:51.359207 vsrgtools-1.4.3/vsrgtools/aka_expr/
--rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-03-26 17:38:26.000000 vsrgtools-1.4.3/vsrgtools/aka_expr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11783 2023-03-26 17:38:26.000000 vsrgtools-1.4.3/vsrgtools/aka_expr/_rg.py
--rw-r--r--   0 runner    (1001) docker     (123)    14266 2023-03-26 17:38:26.000000 vsrgtools-1.4.3/vsrgtools/aka_expr/_rp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-03-26 17:38:26.000000 vsrgtools-1.4.3/vsrgtools/bilateral.cu
--rw-r--r--   0 runner    (1001) docker     (123)    14533 2023-03-26 17:38:26.000000 vsrgtools-1.4.3/vsrgtools/blur.py
--rw-r--r--   0 runner    (1001) docker     (123)     8272 2023-03-26 17:38:26.000000 vsrgtools-1.4.3/vsrgtools/contra.py
--rw-r--r--   0 runner    (1001) docker     (123)     6330 2023-03-26 17:38:26.000000 vsrgtools-1.4.3/vsrgtools/enum.py
--rw-r--r--   0 runner    (1001) docker     (123)     6130 2023-03-26 17:38:26.000000 vsrgtools-1.4.3/vsrgtools/freqs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-03-26 17:38:26.000000 vsrgtools-1.4.3/vsrgtools/func.py
--rw-r--r--   0 runner    (1001) docker     (123)     5417 2023-03-26 17:38:26.000000 vsrgtools-1.4.3/vsrgtools/limit.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-26 17:38:26.000000 vsrgtools-1.4.3/vsrgtools/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     4622 2023-03-26 17:38:26.000000 vsrgtools-1.4.3/vsrgtools/rgtools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-03-26 17:38:26.000000 vsrgtools-1.4.3/vsrgtools/sharp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-03-26 17:38:26.000000 vsrgtools-1.4.3/vsrgtools/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 17:38:51.359207 vsrgtools-1.4.3/vsrgtools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-03-26 17:38:51.000000 vsrgtools-1.4.3/vsrgtools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-03-26 17:38:51.000000 vsrgtools-1.4.3/vsrgtools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-26 17:38:51.000000 vsrgtools-1.4.3/vsrgtools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-03-26 17:38:51.000000 vsrgtools-1.4.3/vsrgtools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-26 17:38:51.000000 vsrgtools-1.4.3/vsrgtools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:57:54.528355 vsrgtools-1.4.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-05-04 21:57:29.000000 vsrgtools-1.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-05-04 21:57:54.528355 vsrgtools-1.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-04 21:57:29.000000 vsrgtools-1.4.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-04 21:57:54.528355 vsrgtools-1.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-05-04 21:57:29.000000 vsrgtools-1.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:57:54.528355 vsrgtools-1.4.4/vsrgtools/
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-04 21:57:29.000000 vsrgtools-1.4.4/vsrgtools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-04 21:57:29.000000 vsrgtools-1.4.4/vsrgtools/_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:57:54.528355 vsrgtools-1.4.4/vsrgtools/aka_expr/
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-05-04 21:57:29.000000 vsrgtools-1.4.4/vsrgtools/aka_expr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11783 2023-05-04 21:57:29.000000 vsrgtools-1.4.4/vsrgtools/aka_expr/_rg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14266 2023-05-04 21:57:29.000000 vsrgtools-1.4.4/vsrgtools/aka_expr/_rp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3807 2023-05-04 21:57:29.000000 vsrgtools-1.4.4/vsrgtools/bilateral.cu
+-rw-r--r--   0 runner    (1001) docker     (123)    14524 2023-05-04 21:57:29.000000 vsrgtools-1.4.4/vsrgtools/blur.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8273 2023-05-04 21:57:29.000000 vsrgtools-1.4.4/vsrgtools/contra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6463 2023-05-04 21:57:29.000000 vsrgtools-1.4.4/vsrgtools/enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5824 2023-05-04 21:57:29.000000 vsrgtools-1.4.4/vsrgtools/freqs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-05-04 21:57:29.000000 vsrgtools-1.4.4/vsrgtools/func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5417 2023-05-04 21:57:29.000000 vsrgtools-1.4.4/vsrgtools/limit.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 21:57:29.000000 vsrgtools-1.4.4/vsrgtools/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     4622 2023-05-04 21:57:29.000000 vsrgtools-1.4.4/vsrgtools/rgtools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-05-04 21:57:29.000000 vsrgtools-1.4.4/vsrgtools/sharp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-05-04 21:57:29.000000 vsrgtools-1.4.4/vsrgtools/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:57:54.528355 vsrgtools-1.4.4/vsrgtools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-05-04 21:57:54.000000 vsrgtools-1.4.4/vsrgtools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-04 21:57:54.000000 vsrgtools-1.4.4/vsrgtools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 21:57:54.000000 vsrgtools-1.4.4/vsrgtools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-04 21:57:54.000000 vsrgtools-1.4.4/vsrgtools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-04 21:57:54.000000 vsrgtools-1.4.4/vsrgtools.egg-info/top_level.txt
```

### Comparing `vsrgtools-1.4.3/LICENSE` & `vsrgtools-1.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `vsrgtools-1.4.3/PKG-INFO` & `vsrgtools-1.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vsrgtools
-Version: 1.4.3
+Version: 1.4.4
 Summary: Wrapper for RGVS, RGSF, and various other functions
 Author: Irrational Encoding Wizardry
 Author-email: wizards@encode.moe
 Maintainer: Setsugen no ao
 Maintainer-email: setsugen@setsugen.dev
 Project-URL: Source Code, https://github.com/Irrational-Encoding-Wizardry/vs-rgtools
 Project-URL: Documentation, https://vsrgtools.encode.moe/en/latest/
```

### Comparing `vsrgtools-1.4.3/setup.cfg` & `vsrgtools-1.4.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `vsrgtools-1.4.3/setup.py` & `vsrgtools-1.4.4/setup.py`

 * *Files identical despite different names*

### Comparing `vsrgtools-1.4.3/vsrgtools/aka_expr/__init__.py` & `vsrgtools-1.4.4/vsrgtools/aka_expr/__init__.py`

 * *Files identical despite different names*

### Comparing `vsrgtools-1.4.3/vsrgtools/aka_expr/_rg.py` & `vsrgtools-1.4.4/vsrgtools/aka_expr/_rg.py`

 * *Files identical despite different names*

### Comparing `vsrgtools-1.4.3/vsrgtools/aka_expr/_rp.py` & `vsrgtools-1.4.4/vsrgtools/aka_expr/_rp.py`

 * *Files identical despite different names*

### Comparing `vsrgtools-1.4.3/vsrgtools/bilateral.cu` & `vsrgtools-1.4.4/vsrgtools/bilateral.cu`

 * *Files 2% similar despite different names*

```diff
@@ -10,17 +10,14 @@
 __device__ static const int kernel_size_x = 2 * radius + ${block_x};
 __device__ static const int kernel_size_y = 2 * radius + ${block_y};
 
 extern "C"
 __global__ void bilateral(const ${data_type} * __restrict__ src, ${data_type} * __restrict__ dst) {
     const int x = threadIdx.x + blockIdx.x * blockDim.x;
     const int y = threadIdx.y + blockIdx.y * blockDim.y;
-    
-    if (x >= width || y >= height)
-        return;
 
     float num {};
     float den {};
 
     float center {};
     float value {};
 
@@ -33,14 +30,17 @@
                 int sx = min(max(cx - static_cast<int>(threadIdx.x) - radius + x, 0), width - 1);
                 buffer[cy * kernel_size_x + cx] = src[sy * width + sx];
             }
         }
 
         __syncthreads();
 
+        if (x >= width || y >= height)
+            return;
+
         if constexpr (is_float) {
             center = src[y * width + x];
         } else {
             center = (float)(src[y * width + x]) / peak;
         }
         
         #pragma unroll 4
@@ -68,14 +68,17 @@
         
         if constexpr (is_float) {
             dst[y * width + x] = num / den;
         } else {
             dst[y * width + x] = __float2int_rn(num / den * peak);
         }
     } else {
+        if (x >= width || y >= height)
+            return;
+
         if constexpr (is_float) {
             center = src[y * width + x];
         } else {
             center = (float)(src[y * width + x]) / peak;
         }
         
         #pragma unroll 4
```

### Comparing `vsrgtools-1.4.3/vsrgtools/blur.py` & `vsrgtools-1.4.4/vsrgtools/blur.py`

 * *Files 0% similar despite different names*

```diff
@@ -387,15 +387,15 @@
         if min(sigmaS) < 4 and PyPluginCuda.backend.is_available:
             block_x = fallback(block_x, block_y, 16)
             block_y = fallback(block_y, block_x)
 
             return BilateralFilter(
                 clip, sigmaS, sigmaR, radius,
                 kernel_size=(block_x, block_y),
-                use_shared_memory=False  # use_shared_memory
+                use_shared_memory=use_shared_memory
             ).invoke()
 
         try:
             if hasattr(core, 'bilateralgpu_rtc'):
                 return clip.bilateralgpu_rtc.Bilateral(
                     sigmaS, sigmaR, radius, device_id, num_streams, use_shared_memory, block_x, block_y
                 )
```

### Comparing `vsrgtools-1.4.3/vsrgtools/contra.py` & `vsrgtools-1.4.4/vsrgtools/contra.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,15 +82,15 @@
 @disallow_variable_resolution
 def contrasharpening_dehalo(
     flt: vs.VideoNode, src: vs.VideoNode, level: float = 1.4, alpha: float = 2.49, planes: PlanesT = 0
 ) -> vs.VideoNode:
     """
     :param dehaloed:    Dehaloed clip
     :param src:         Source clip
-    :param level:       Strengh level
+    :param level:       Strength level
     :return:            Contrasharpened clip
     """
     assert check_variable(src, contrasharpening)
     assert check_variable(flt, contrasharpening)
     check_ref_clip(src, flt, contrasharpening)
 
     planes = normalize_planes(flt, planes)
@@ -158,15 +158,15 @@
     mode: RepairModeT = RepairMode.MINMAX_SQUARE_REF3, planes: PlanesT = 0
 ) -> vs.VideoNode:
     """
     :param flt:         Filtered clip.
     :param src:         Source clip.
     :param sharp:       Contrast Adaptive Sharpening's sharpening strength.
                         If it's a list, depending on ``merge_func`` being ``None``,
-                        it will iterate over with different strenghts or merge all with ``merge_func``.
+                        it will iterate over with different strengths or merge all with ``merge_func``.
     :param radius:      Spatial radius for contra-sharpening (1-3). Default is 2 for HD / 1 for SD.
     :param merge_func:  Depending on ``sharp``, this will get all sharpened clips and merge them.
     :param mode:        Mode of rgvs.Repair to limit the difference.
     :param planes:      Planes to process, defaults to None.
     :return:            Contrasharpened clip.
     """
```

### Comparing `vsrgtools-1.4.3/vsrgtools/enum.py` & `vsrgtools-1.4.4/vsrgtools/enum.py`

 * *Files 2% similar despite different names*

```diff
@@ -215,14 +215,18 @@
 
         kernel = [x * 1023 / high for x in kernel]
         kernel = [*kernel[::-1], 1023, *kernel]
 
         return BaseBlurMatrix[float](kernel)
 
     @classmethod
+    def gauss_from_radius(cls, radius: int) -> BaseBlurMatrix[float]:
+        return cls.gauss((radius + 1.0) / 3)
+
+    @classmethod
     def log(cls, radius: int = 1, strength: float = 100.0) -> BaseBlurMatrix[float]:
         strength = max(1e-6, min(log2(3) * strength / 100, log2(3)))
 
         weight = 0.5 ** strength / ((1 - 0.5 ** strength) * 0.5)
 
         matrix = [1.0]
```

### Comparing `vsrgtools-1.4.3/vsrgtools/freqs.py` & `vsrgtools-1.4.4/vsrgtools/freqs.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,18 +111,14 @@
     filter: VSFunction | list[VSFunction] = partial(box_blur, radius=3, passes=2),
     planes: PlanesT = None
 ) -> vs.VideoNode:
     """
     Merge multiple sources.
 
     :param clips:           Clips to be merged together.
-                            If using multiple sources, first should be the "best" one,
-                            then the other a lowpassed or worse source overall.
-                            If the clips are filtered, first is src and
-                            others the denoised/debanded/whatever.
     :param filter:          Filter to be applied to clips to isolate high frequencies.
                             If a list, each filter will be mapped to corresponding clip at same index.
                             If not enough filters are passed, the last one will be reused.
     :param planes:          Planes to be processed.
 
     :return:                Merged clips.
     """
```

### Comparing `vsrgtools-1.4.3/vsrgtools/func.py` & `vsrgtools-1.4.4/vsrgtools/func.py`

 * *Files identical despite different names*

### Comparing `vsrgtools-1.4.3/vsrgtools/limit.py` & `vsrgtools-1.4.4/vsrgtools/limit.py`

 * *Files identical despite different names*

### Comparing `vsrgtools-1.4.3/vsrgtools/rgtools.py` & `vsrgtools-1.4.4/vsrgtools/rgtools.py`

 * *Files identical despite different names*

### Comparing `vsrgtools-1.4.3/vsrgtools/sharp.py` & `vsrgtools-1.4.4/vsrgtools/sharp.py`

 * *Files identical despite different names*

### Comparing `vsrgtools-1.4.3/vsrgtools/util.py` & `vsrgtools-1.4.4/vsrgtools/util.py`

 * *Files identical despite different names*

### Comparing `vsrgtools-1.4.3/vsrgtools.egg-info/PKG-INFO` & `vsrgtools-1.4.4/vsrgtools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vsrgtools
-Version: 1.4.3
+Version: 1.4.4
 Summary: Wrapper for RGVS, RGSF, and various other functions
 Author: Irrational Encoding Wizardry
 Author-email: wizards@encode.moe
 Maintainer: Setsugen no ao
 Maintainer-email: setsugen@setsugen.dev
 Project-URL: Source Code, https://github.com/Irrational-Encoding-Wizardry/vs-rgtools
 Project-URL: Documentation, https://vsrgtools.encode.moe/en/latest/
```

### Comparing `vsrgtools-1.4.3/vsrgtools.egg-info/SOURCES.txt` & `vsrgtools-1.4.4/vsrgtools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

