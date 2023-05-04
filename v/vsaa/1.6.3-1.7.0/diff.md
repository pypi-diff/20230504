# Comparing `tmp/vsaa-1.6.3.tar.gz` & `tmp/vsaa-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vsaa-1.6.3.tar", last modified: Sun Mar 26 17:39:13 2023, max compression
+gzip compressed data, was "vsaa-1.7.0.tar", last modified: Thu May  4 21:58:48 2023, max compression
```

## Comparing `vsaa-1.6.3.tar` & `vsaa-1.7.0.tar`

### file list

```diff
@@ -1,27 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 17:39:13.110822 vsaa-1.6.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-03-26 17:38:51.000000 vsaa-1.6.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-03-26 17:39:13.110822 vsaa-1.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-03-26 17:38:51.000000 vsaa-1.6.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-03-26 17:39:13.110822 vsaa-1.6.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-03-26 17:38:51.000000 vsaa-1.6.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 17:39:13.106822 vsaa-1.6.3/vsaa/
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-03-26 17:38:51.000000 vsaa-1.6.3/vsaa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-03-26 17:38:51.000000 vsaa-1.6.3/vsaa/_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     9385 2023-03-26 17:38:51.000000 vsaa-1.6.3/vsaa/abstract.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 17:39:13.110822 vsaa-1.6.3/vsaa/antialiasers/
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-03-26 17:38:51.000000 vsaa-1.6.3/vsaa/antialiasers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-03-26 17:38:51.000000 vsaa-1.6.3/vsaa/antialiasers/eedi2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-03-26 17:38:51.000000 vsaa-1.6.3/vsaa/antialiasers/eedi3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-03-26 17:38:51.000000 vsaa-1.6.3/vsaa/antialiasers/nnedi3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-03-26 17:38:51.000000 vsaa-1.6.3/vsaa/antialiasers/sangnom.py
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-03-26 17:38:51.000000 vsaa-1.6.3/vsaa/antialiasers/znedi3.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-03-26 17:38:51.000000 vsaa-1.6.3/vsaa/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)    13803 2023-03-26 17:38:51.000000 vsaa-1.6.3/vsaa/funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-03-26 17:38:51.000000 vsaa-1.6.3/vsaa/mask.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-26 17:38:51.000000 vsaa-1.6.3/vsaa/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 17:39:13.110822 vsaa-1.6.3/vsaa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-03-26 17:39:13.000000 vsaa-1.6.3/vsaa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-03-26 17:39:13.000000 vsaa-1.6.3/vsaa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-26 17:39:13.000000 vsaa-1.6.3/vsaa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-03-26 17:39:13.000000 vsaa-1.6.3/vsaa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-03-26 17:39:13.000000 vsaa-1.6.3/vsaa.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:58:48.346152 vsaa-1.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-04 21:58:22.000000 vsaa-1.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-05-04 21:58:48.346152 vsaa-1.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-05-04 21:58:22.000000 vsaa-1.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-04 21:58:48.346152 vsaa-1.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-05-04 21:58:22.000000 vsaa-1.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:58:48.346152 vsaa-1.7.0/vsaa/
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-04 21:58:22.000000 vsaa-1.7.0/vsaa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-04 21:58:22.000000 vsaa-1.7.0/vsaa/_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10178 2023-05-04 21:58:22.000000 vsaa-1.7.0/vsaa/abstract.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:58:48.346152 vsaa-1.7.0/vsaa/antialiasers/
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-04 21:58:22.000000 vsaa-1.7.0/vsaa/antialiasers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-05-04 21:58:22.000000 vsaa-1.7.0/vsaa/antialiasers/eedi2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-05-04 21:58:22.000000 vsaa-1.7.0/vsaa/antialiasers/eedi3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-05-04 21:58:22.000000 vsaa-1.7.0/vsaa/antialiasers/nnedi3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-05-04 21:58:22.000000 vsaa-1.7.0/vsaa/antialiasers/sangnom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-04 21:58:22.000000 vsaa-1.7.0/vsaa/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13725 2023-05-04 21:58:22.000000 vsaa-1.7.0/vsaa/funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-04 21:58:22.000000 vsaa-1.7.0/vsaa/mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 21:58:22.000000 vsaa-1.7.0/vsaa/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:58:48.346152 vsaa-1.7.0/vsaa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-05-04 21:58:48.000000 vsaa-1.7.0/vsaa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-04 21:58:48.000000 vsaa-1.7.0/vsaa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 21:58:48.000000 vsaa-1.7.0/vsaa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-04 21:58:48.000000 vsaa-1.7.0/vsaa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-04 21:58:48.000000 vsaa-1.7.0/vsaa.egg-info/top_level.txt
```

### Comparing `vsaa-1.6.3/LICENSE` & `vsaa-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vsaa-1.6.3/PKG-INFO` & `vsaa-1.7.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vsaa
-Version: 1.6.3
+Version: 1.7.0
 Summary: VapourSynth anti aliasing and scaling functions
 Author: Setsugen no ao
 Author-email: setsugen@setsugen.dev
 Maintainer: Setsugen no ao
 Maintainer-email: setsugen@setsugen.dev
 Project-URL: Source Code, https://github.com/Irrational-Encoding-Wizardry/vs-aa
 Project-URL: Documentation, https://vsaa.encode.moe/en/latest/
```

### Comparing `vsaa-1.6.3/setup.cfg` & `vsaa-1.7.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `vsaa-1.6.3/setup.py` & `vsaa-1.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `vsaa-1.6.3/vsaa/abstract.py` & `vsaa-1.7.0/vsaa/abstract.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from dataclasses import dataclass
 from dataclasses import field as dc_field
 from dataclasses import replace
 from itertools import zip_longest
 from math import ceil, log2
 from typing import Any, Callable, overload
 
+from vsexprtools import norm_expr
 from vskernels import Catrom, Kernel, KernelT, NoShift, Scaler, ScalerT
 from vstools import T, core, inject_self, vs, vs_object
 
 from .enums import AADirection
 
 __all__ = [
     'SuperSampler',
@@ -18,14 +19,23 @@
     'Antialiaser'
 ]
 
 
 class _SingleInterpolate(vs_object):
     _shift: float
 
+    def _post_interpolate(
+        self, clip: vs.VideoNode, aa_clip: vs.VideoNode, double_y: bool,
+        mclip: vs.VideoNode | None = None, **kwargs: Any
+    ) -> vs.VideoNode:
+        if not double_y and isinstance(mclip, vs.VideoNode):
+            return norm_expr([clip, aa_clip, mclip], 'z y x ?')
+
+        return aa_clip
+
     def interpolate(self, clip: vs.VideoNode, double_y: bool, **kwargs: Any) -> vs.VideoNode:
         raise NotImplementedError
 
 
 @dataclass
 class _Antialiaser(_SingleInterpolate):
     field: int = dc_field(default=0, kw_only=True)
@@ -42,26 +52,25 @@
 
     def preprocess_clip(self, clip: vs.VideoNode) -> vs.VideoNode:
         return clip
 
     def get_aa_args(self, clip: vs.VideoNode, **kwargs: Any) -> dict[str, Any]:
         return {}
 
-    def shift_interpolate(self, clip: vs.VideoNode, inter: vs.VideoNode, double_y: bool) -> vs.VideoNode:
-        if double_y:
-            return inter
-        elif self.drop_fields:
-            return inter
+    def shift_interpolate(
+        self, clip: vs.VideoNode, inter: vs.VideoNode, double_y: bool, **kwargs: Any
+    ) -> vs.VideoNode:
+        if not double_y and not self.drop_fields:
+            shift = (self._shift * int(not self.field), 0)
 
-        shift = (self._shift * int(not self.field), 0)
+            inter = (self._scaler if self._scaler else self._shifter).scale(inter, clip.width, clip.height, shift)
 
-        if self._scaler:
-            return self._scaler.scale(inter, clip.width, clip.height, shift)
+            return self._post_interpolate(clip, inter, double_y, **kwargs)
 
-        return self._shifter.scale(inter, clip.width, clip.height, shift)
+        return inter
 
     @inject_self
     def copy(self: T, **kwargs: Any) -> T:
         return replace(self, **kwargs)
 
 
 class _FullInterpolate(_SingleInterpolate):
@@ -158,23 +167,26 @@
 
 
 class SingleRater(_Antialiaser):
     def get_sr_args(self, clip: vs.VideoNode, **kwargs: Any) -> dict[str, Any]:
         return {}
 
     @overload
-    def aa(self, clip: vs.VideoNode, dir: AADirection = AADirection.VERTICAL, /, **kwargs: Any) -> vs.VideoNode:
+    @inject_self.init_kwargs.clean
+    def aa(self, clip: vs.VideoNode, dir: AADirection = AADirection.BOTH, /, **kwargs: Any) -> vs.VideoNode:
         ...
 
     @overload
-    def aa(self, clip: vs.VideoNode, y: bool = True, x: bool = False, /, **kwargs: Any) -> vs.VideoNode:
+    @inject_self.init_kwargs.clean
+    def aa(self, clip: vs.VideoNode, y: bool = True, x: bool = True, /, **kwargs: Any) -> vs.VideoNode:
         ...
 
+    @inject_self.init_kwargs.clean
     def aa(
-        self, clip: vs.VideoNode, y_or_dir: bool | AADirection = True, x: bool = False, /, **kwargs: Any
+        self, clip: vs.VideoNode, y_or_dir: bool | AADirection = True, x: bool = True, /, **kwargs: Any
     ) -> vs.VideoNode:
         if isinstance(y_or_dir, AADirection):
             y, x = y_or_dir.to_yx()
         else:
             y = y_or_dir
 
         clip = self.preprocess_clip(clip)
@@ -190,14 +202,17 @@
             nonlocal upscaled
 
             before = self.transpose_first if before else not self.transpose_first
 
             if ((before or not y) if is_width else (before and x)):
                 upscaled = upscaled.std.Transpose()
 
+                if 'mclip' in kwargs:
+                    kwargs.update(mclip=kwargs.get('mclip').std.Transpose())
+
         for isx, val in enumerate([y, x]):
             if val:
                 _transpose(True, isx)
 
                 if isinstance(self, _FullInterpolate) and self.is_full_interpolate_enabled(x, y):
                     upscaled = self.full_interpolate(upscaled, False, False, **kwargs)
                 else:
@@ -230,45 +245,51 @@
     def scale(  # type: ignore[override]
         self, clip: vs.VideoNode, width: int, height: int, shift: tuple[float, float] = (0, 0), **kwargs: Any
     ) -> vs.VideoNode:
         """Scale with this antialiaser"""
         return SuperSampler.scale(self, clip, width, height, shift, **kwargs)
 
     @overload
-    def aa(self, clip: vs.VideoNode, dir: AADirection = AADirection.VERTICAL, /, **kwargs: Any) -> vs.VideoNode:
+    @inject_self.init_kwargs.clean
+    def aa(self, clip: vs.VideoNode, dir: AADirection = AADirection.BOTH, /, **kwargs: Any) -> vs.VideoNode:
         ...
 
     @overload
-    def aa(self, clip: vs.VideoNode, y: bool = True, x: bool = False, /, **kwargs: Any) -> vs.VideoNode:
+    @inject_self.init_kwargs.clean
+    def aa(self, clip: vs.VideoNode, y: bool = True, x: bool = True, /, **kwargs: Any) -> vs.VideoNode:
         ...
 
+    @inject_self.init_kwargs.clean
     def aa(
-        self, clip: vs.VideoNode, y_or_dir: bool | AADirection = True, x: bool = False, /, **kwargs: Any
+        self, clip: vs.VideoNode, y_or_dir: bool | AADirection = True, x: bool = True, /, **kwargs: Any
     ) -> vs.VideoNode:
         """Single rate aa with this antialiaser"""
 
         if isinstance(y_or_dir, AADirection):
             y, x = y_or_dir.to_yx()
         else:
             y = y_or_dir
 
         clip = self.preprocess_clip(clip)
 
         return SingleRater._aa(self, clip, y, x, **kwargs)
 
     @overload
-    def draa(self, clip: vs.VideoNode, dir: AADirection = AADirection.VERTICAL, /, **kwargs: Any) -> vs.VideoNode:
+    @inject_self.init_kwargs.clean
+    def draa(self, clip: vs.VideoNode, dir: AADirection = AADirection.BOTH, /, **kwargs: Any) -> vs.VideoNode:
         ...
 
     @overload
-    def draa(self, clip: vs.VideoNode, y: bool = True, x: bool = False, /, **kwargs: Any) -> vs.VideoNode:
+    @inject_self.init_kwargs.clean
+    def draa(self, clip: vs.VideoNode, y: bool = True, x: bool = True, /, **kwargs: Any) -> vs.VideoNode:
         ...
 
+    @inject_self.init_kwargs.clean
     def draa(
-        self, clip: vs.VideoNode, y_or_dir: bool | AADirection = True, x: bool = False, /, **kwargs: Any
+        self, clip: vs.VideoNode, y_or_dir: bool | AADirection = True, x: bool = True, /, **kwargs: Any
     ) -> vs.VideoNode:
         """Double rate aa with this antialiaser"""
 
         if isinstance(y_or_dir, AADirection):
             y, x = y_or_dir.to_yx()
         else:
             y = y_or_dir
```

### Comparing `vsaa-1.6.3/vsaa/antialiasers/eedi2.py` & `vsaa-1.7.0/vsaa/antialiasers/eedi2.py`

 * *Files 10% similar despite different names*

```diff
@@ -31,35 +31,35 @@
     def get_aa_args(self, clip: vs.VideoNode, **kwargs: Any) -> dict[str, Any]:
         return dict(
             mthresh=self.mthresh, lthresh=self.lthresh, vthresh=self.vthresh,
             estr=self.estr, dstr=self.dstr, maxd=self.maxd, pp=self.pp
         )
 
     def interpolate(self, clip: vs.VideoNode, double_y: bool, **kwargs: Any) -> vs.VideoNode:
-        interpolated: vs.VideoNode
+        inter: vs.VideoNode
 
         if self.cuda:
-            interpolated = core.eedi2cuda.EEDI2(clip, self.field, **kwargs)  # type: ignore
+            inter = core.eedi2cuda.EEDI2(clip, self.field, **kwargs)  # type: ignore
         else:
-            interpolated = core.eedi2.EEDI2(clip, self.field, **kwargs)  # type: ignore
+            inter = core.eedi2.EEDI2(clip, self.field, **kwargs)  # type: ignore
 
-        if double_y:
-            return interpolated
+        if not double_y:
+            if self.drop_fields:
+                inter = inter.std.SeparateFields(not self.field)[::2]
+
+                inter = self._shifter.shift(inter, (0.5 - 0.75 * self.field, 0))
+            else:
+                shift = (self._shift * int(not self.field), 0)
+
+                if self._scaler:
+                    inter = self._scaler.scale(inter, clip.width, clip.height, shift)
+                else:
+                    inter = self._shifter.scale(inter, clip.width, clip.height, shift)
 
-        if self.drop_fields:
-            interpolated = interpolated.std.SeparateFields(not self.field)[::2]
-
-            return self._shifter.shift(interpolated, (0.5 - 0.75 * self.field, 0))
-
-        shift = (self._shift * int(not self.field), 0)
-
-        if self._scaler:
-            return self._scaler.scale(interpolated, clip.width, clip.height, shift)
-
-        return self._shifter.scale(interpolated, clip.width, clip.height, shift)
+        return self._post_interpolate(clip, inter, double_y, **kwargs)
 
     def full_interpolate(self, clip: vs.VideoNode, double_y: bool, double_x: bool, **kwargs: Any) -> vs.VideoNode:
         return core.eedi2cuda.Enlarge2(clip, **kwargs)  # type: ignore
 
     _shift = -0.5
```

### Comparing `vsaa-1.6.3/vsaa/antialiasers/eedi3.py` & `vsaa-1.7.0/vsaa/antialiasers/eedi3.py`

 * *Files 5% similar despite different names*

```diff
@@ -66,15 +66,17 @@
 
         if self._sclip_aa and ((('sclip' in kwargs) and not kwargs['sclip']) or 'sclip' not in kwargs):
             if self._sclip_aa is True:
                 if double_y:
                     raise CustomValueError("You can't pass sclip_aa=True when supersampling!", self.__class__)
                 aa_kwargs.update(sclip=clip)
             else:
-                sclip_args = self._sclip_aa.get_aa_args(clip)
+                sclip_args = self._sclip_aa.get_aa_args(
+                    clip, **(dict(mclip=kwargs.get('clip') if 'mclip' in kwargs else {}))
+                )
 
                 if double_y:
                     sclip_args |= self._sclip_aa.get_ss_args(clip)
                 else:
                     sclip_args |= self._sclip_aa.get_sr_args(clip)
 
                 aa_kwargs.update(
@@ -83,15 +85,15 @@
 
         function = core.eedi3m.EEDI3CL if self.opencl else core.eedi3m.EEDI3
 
         interpolated = function(  # type: ignore[operator]
             clip, self.field, double_y or not self.drop_fields, **aa_kwargs
         )
 
-        return self.shift_interpolate(clip, interpolated, double_y)
+        return self.shift_interpolate(clip, interpolated, double_y, **kwargs)
 
     _shift = 0.5
 
 
 class Eedi3SS(EEDI3, SuperSampler):
     ...
```

### Comparing `vsaa-1.6.3/vsaa/antialiasers/nnedi3.py` & `vsaa-1.7.0/vsaa/antialiasers/nnedi3.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,19 +10,19 @@
 __all__ = [
     'Nnedi3', 'Nnedi3DR'
 ]
 
 
 @dataclass
 class NNEDI3(_FullInterpolate, _Antialiaser):
-    nsize: int = 4
+    nsize: int = 0
     nns: int = 4
     qual: int = 2
     etype: int = 0
-    pscrn: int = 2
+    pscrn: int = 1
 
     opencl: bool = False
 
     def is_full_interpolate_enabled(self, x: bool, y: bool) -> bool:
         return self.opencl
 
     def get_aa_args(self, clip: vs.VideoNode, **kwargs: Any) -> dict[str, Any]:
@@ -34,15 +34,15 @@
     def interpolate(self, clip: vs.VideoNode, double_y: bool, **kwargs: Any) -> vs.VideoNode:
         interpolated: vs.VideoNode = getattr(
             core, 'znedi3' if hasattr(core, 'znedi3') else 'nnedi3'
         ).nnedi3(
             clip, self.field, double_y or not self.drop_fields, **kwargs
         )
 
-        return self.shift_interpolate(clip, interpolated, double_y)
+        return self.shift_interpolate(clip, interpolated, double_y, **kwargs)
 
     def full_interpolate(self, clip: vs.VideoNode, double_y: bool, double_x: bool, **kwargs: Any) -> vs.VideoNode:
         return core.nnedi3cl.NNEDI3CL(clip, self.field, double_y, double_x, **kwargs)
 
     _shift = 0.5
```

### Comparing `vsaa-1.6.3/vsaa/antialiasers/sangnom.py` & `vsaa-1.7.0/vsaa/antialiasers/sangnom.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         return dict(aa=self.aa_strength, order=0 if self.double_fps else self.field + 1)
 
     def interpolate(self, clip: vs.VideoNode, double_y: bool, **kwargs: Any) -> vs.VideoNode:
         interpolated: vs.VideoNode = core.sangnom.SangNom(  # type: ignore
             clip, dh=double_y or not self.drop_fields, **kwargs
         )
 
-        return self.shift_interpolate(clip, interpolated, double_y)
+        return self.shift_interpolate(clip, interpolated, double_y, **kwargs)
 
     _shift = -0.5
 
 
 class SangNomSS(SANGNOM, SuperSampler):
     ...
```

### Comparing `vsaa-1.6.3/vsaa/funcs.py` & `vsaa-1.7.0/vsaa/funcs.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 from __future__ import annotations
 
-from math import ceil
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, Literal
 
 from vsexprtools import complexpr_available, norm_expr
 from vskernels import Catrom, NoScale, Scaler, ScalerT, Spline144
 from vsmasktools import EdgeDetect, EdgeDetectT, Prewitt, ScharrTCanny
 from vsrgtools import RepairMode, box_blur, contrasharpening_median, median_clips, repair, unsharp_masked
 from vstools import (
-    MISSING, CustomOverflowError, CustomRuntimeError, FunctionUtil, MissingT, PlanesT, check_ref_clip, core, get_h,
-    get_peak_value, get_w, join, normalize_planes, plane, scale_8bit, scale_value, split, vs
+    MISSING, CustomOverflowError, CustomRuntimeError, FunctionUtil, MissingT, PlanesT, check_ref_clip, get_h,
+    get_peak_value, get_w, get_y, join, normalize_planes, plane, scale_8bit, scale_value, split, vs
 )
 
 from .abstract import Antialiaser, SingleRater
 from .antialiasers import Eedi3, Nnedi3
 from .enums import AADirection
 from .mask import resize_aa_mask
 
@@ -133,32 +132,33 @@
     :param aafun:       Antialiasing function.
     :return:            Antialiased clip.
     """
     func = FunctionUtil(clip, transpose_aa, planes)
 
     aafunc = aafunc.copy(transpose_first=True, drop_fields=False)  # type: ignore
 
-    aa = aafunc.aa(func.work_clip, AADirection.BOTH)  # type: ignore
+    aa = aafunc.aa(func.work_clip)  # type: ignore
 
     return func.return_clip(aa)
 
 
 def clamp_aa(
     src: vs.VideoNode, weak: vs.VideoNode, strong: vs.VideoNode,
-    strength: float = 1, planes: PlanesT = 0
+    strength: float = 1, ref: vs.VideoNode | None = None, planes: PlanesT = 0
 ) -> vs.VideoNode:
     """
     Clamp stronger AAs to weaker AAs.
     Useful for clamping :py:func:`upscaled_sraa` or :py:func:`Eedi3`
     to :py:func:`Nnedi3` for a strong but more precise AA.
 
     :param src:         Non-AA'd source clip.
     :param weak:        Weakly-AA'd clip.
     :param strong:      Strongly-AA'd clip.
     :param strength:    Clamping strength.
+    :param ref:         Reference clip for clamping.
     :param planes:      Planes to process.
 
     :return:            Clip with clamped anti-aliasing.
     """
     assert src.format
 
     planes = normalize_planes(src, planes)
@@ -167,38 +167,47 @@
         thr = strength * get_peak_value(src)
     else:
         thr = strength / 219
 
     if thr == 0:
         return median_clips(src, weak, strong, planes=planes)
 
-    if complexpr_available:
-        expr = f'x y - XYD! XYD@ x z - XZD! XZD@ xor x XYD@ abs XZD@ abs < z y {thr} + min y {thr} - max z ? ?'
+    if ref:
+        if complexpr_available:
+            expr = f'y z - ZD! y a - AD! ZD@ AD@ xor x ZD@ abs AD@ abs < a z {thr} + min z {thr} - max a ? ?'
+        else:
+            expr = f'y z - y a - xor x y z - abs y a - abs < a z {thr} + min z {thr} - max a ? ?'
     else:
-        expr = f'x y - x z - xor x x y - abs x z - abs < z y {thr} + min y {thr} - max z ? ?'
+        if complexpr_available:
+            expr = f'x y - XYD! x z - XZD! XYD@ XZD@ xor x XYD@ abs XZD@ abs < z y {thr} + min y {thr} - max z ? ?'
+        else:
+            expr = f'x y - x z - xor x x y - abs x z - abs < z y {thr} + min y {thr} - max z ? ?'
 
-    return norm_expr([src, weak, strong], expr, planes)
+    return norm_expr([src, ref, weak, strong] if ref else [src, weak, strong], expr, planes)
 
 
 def masked_clamp_aa(
     clip: vs.VideoNode, strength: float = 1.0,
     mthr: float = 0.25, mask: vs.VideoNode | EdgeDetectT | None = None,
-    weak_aa: SingleRater | None = None, strong_aa: SingleRater | None = None,
-    opencl: bool | None = False, planes: PlanesT = 0
+    weak_aa: vs.VideoNode | SingleRater = Nnedi3(),
+    strong_aa: vs.VideoNode | SingleRater = Eedi3(),
+    opencl: bool | None = False, ref: vs.VideoNode | None = None,
+    planes: PlanesT = 0
 ) -> vs.VideoNode:
     """
     Clamp a strong aa to a weaker one for the purpose of reducing the stronger's artifacts.
 
     :param clip:                Clip to process.
     :param strength:            Set threshold strength for over/underflow value for clamping.
     :param mthr:                Binarize threshold for the mask, float.
     :param mask:                Clip to use for custom mask or an EdgeDetect to use custom masker.
     :param weak_aa:             SingleRater for the weaker aa.
     :param strong_aa:           SingleRater for the stronger aa.
-    :param opencl:              Wheter to force OpenCL acceleration, None to leave as is.
+    :param opencl:              Whether to force OpenCL acceleration, None to leave as is.
+    :param ref:                 Reference clip for clamping.
 
     :return:                    Antialiased clip.
     """
     assert clip.format
 
     func = FunctionUtil(clip, masked_clamp_aa, planes)
 
@@ -207,30 +216,34 @@
 
         mask = ScharrTCanny.ensure_obj(mask).edgemask(func.work_clip)  # type: ignore
         mask = mask.std.Binarize(bin_thr)
         mask = mask.std.Maximum()
         mask = box_blur(mask)
         mask = mask.std.Minimum().std.Deflate()
 
-    if weak_aa is None:
-        weak_aa = Nnedi3(
-            opencl=hasattr(core, 'nnedi3cl') if opencl is None else opencl
-        )
-    elif opencl is not None and hasattr(weak_aa, 'opencl'):
-        weak_aa.opencl = opencl
-
-    if strong_aa is None:
-        strong_aa = Eedi3(opencl=opencl is None or opencl)
-    elif opencl is not None and hasattr(strong_aa, 'opencl'):
-        strong_aa.opencl = opencl
+    if isinstance(weak_aa, SingleRater):
+        if opencl is not None and hasattr(weak_aa, 'opencl'):
+            weak_aa.opencl = opencl
+
+        weak_aa = transpose_aa(func.work_clip, weak_aa, func.norm_planes)
+    elif func.luma_only:
+        weak_aa = get_y(weak_aa)
+
+    if isinstance(strong_aa, SingleRater):
+        if opencl is not None and hasattr(strong_aa, 'opencl'):
+            strong_aa.opencl = opencl
+
+        strong_aa = transpose_aa(func.work_clip, strong_aa, func.norm_planes)
+    elif func.luma_only:
+        strong_aa = get_y(strong_aa)
 
-    weak = transpose_aa(func.work_clip, weak_aa, func.norm_planes)
-    strong = transpose_aa(func.work_clip, strong_aa, func.norm_planes)
+    if ref and func.luma_only:
+        ref = get_y(ref)
 
-    clamped = clamp_aa(func.work_clip, weak, strong, strength, func.norm_planes)
+    clamped = clamp_aa(func.work_clip, weak_aa, strong_aa, strength, ref, func.norm_planes)
 
     merged = func.work_clip.std.MaskedMerge(clamped, mask, func.norm_planes)  # type: ignore
 
     return func.return_clip(merged)
 
 
 def fine_aa(
@@ -254,49 +267,49 @@
     singlerater = singlerater.copy(shifter=Spline144())  # type: ignore
 
     func = FunctionUtil(clip, fine_aa, planes)
 
     if taa:
         aa = transpose_aa(func.work_clip, singlerater)
     else:
-        aa = singlerater.aa(func.work_clip, AADirection.BOTH)  # type: ignore
+        aa = singlerater.aa(func.work_clip)  # type: ignore
 
     contra = contrasharpening_median(func.work_clip, aa, planes=func.norm_planes)
 
     repaired = repair(contra, func.work_clip, func.norm_seq(rep))
 
     return func.return_clip(repaired)
 
 
 if TYPE_CHECKING:
     from vsdenoise import Prefilter
-    from vsscale import SSIM, FSRCNNXShader, FSRCNNXShaderT, ShaderFile
+    from vsscale import FSRCNNXShader, FSRCNNXShaderT, ShaderFile
 
     def based_aa(
         clip: vs.VideoNode, rfactor: float = 2.0,
         mask_thr: int = 60, lmask: vs.VideoNode | EdgeDetectT = Prewitt,
-        downscaler: ScalerT = SSIM,
+        downscaler: ScalerT = Catrom,
         supersampler: ScalerT | FSRCNNXShaderT | ShaderFile | Path | Literal[False] = FSRCNNXShader.x56,
         antialiaser: Antialiaser = Eedi3(0.125, 0.25, vthresh0=12, vthresh1=24, field=1, sclip_aa=None),
         prefilter: Prefilter | vs.VideoNode = Prefilter.NONE, show_mask: bool = False, planes: PlanesT = 0,
         **kwargs: Any
     ) -> vs.VideoNode:
         ...
 else:
     def based_aa(
         clip: vs.VideoNode, rfactor: float = 2.0,
         mask_thr: int = 60, lmask: vs.VideoNode | EdgeDetectT = Prewitt,
-        downscaler: ScalerT | MissingT = MISSING,
+        downscaler: ScalerT = Catrom,
         supersampler: ScalerT | FSRCNNXShaderT | ShaderFile | Path | Literal[False] | MissingT = MISSING,
         antialiaser: Antialiaser = Eedi3(0.125, 0.25, vthresh0=12, vthresh1=24, field=1, sclip_aa=None),
         prefilter: Prefilter | vs.VideoNode | MissingT = MISSING, show_mask: bool = False, planes: PlanesT = 0,
         **kwargs: Any
     ) -> vs.VideoNode:
         try:
-            from vsscale import SSIM, FSRCNNXShader, PlaceboShader  # noqa: F811
+            from vsscale import FSRCNNXShader, PlaceboShader  # noqa: F811
         except ModuleNotFoundError:
             raise CustomRuntimeError(
                 'You\'re missing the "vsscale" package! You can install it with "pip install vsscale".', based_aa
             )
 
         try:
             from vsdenoise import Prefilter  # noqa: F811
@@ -306,26 +319,20 @@
             )
 
         func = FunctionUtil(clip, based_aa, planes)
 
         if supersampler is False:
             supersampler = downscaler = NoScale
         else:
-            if downscaler is MISSING:
-                downscaler = SSIM
-
             if supersampler is MISSING:
                 supersampler = FSRCNNXShader.x56
 
         if prefilter is MISSING:
             prefilter = Prefilter.NONE
 
-        aaw = (round(clip.width * rfactor) + 1) & ~1
-        aah = (round(clip.height * rfactor) + 1) & ~1
-
         if isinstance(prefilter, vs.VideoNode):
             work_clip = plane(prefilter, 0) if func.luma_only else prefilter
             check_ref_clip(func.work_clip, work_clip, based_aa)
         else:
             work_clip = prefilter(func.work_clip)
 
         antialiaser = antialiaser.copy(**kwargs)
@@ -351,32 +358,21 @@
 
         if isinstance(supersampler, (str, Path)):
             supersampler = PlaceboShader(supersampler)
 
         supersampler = Scaler.ensure_obj(supersampler, based_aa)
         downscaler = Scaler.ensure_obj(downscaler, based_aa)
 
-        aa = func.work_clip.std.Transpose()
-        aa = supersampler.scale(aa, aa.width * ceil(rfactor), aa.height * ceil(rfactor))
-        aa = waa = downscaler.scale(aa, aah, aaw)
-
-        if func.work_clip is not work_clip:
-            waa = work_clip.std.Transpose()
-            waa = supersampler.scale(waa, waa.width * ceil(rfactor), waa.height * ceil(rfactor))
-            waa = downscaler.scale(waa, aah, aaw)
-
-        def _aa_mclip(clip: vs.VideoNode, wclip: vs.VideoNode, mclip: vs.VideoNode) -> vs.VideoNode:
-            return core.std.Expr([
-                clip, antialiaser.interpolate(wclip, False, sclip=wclip), mclip
-            ], 'z y x ?')
+        aaw, aah = [(round(r * rfactor) + 1) & ~1 for r in (clip.width, clip.height)]
 
-        mclip_up = resize_aa_mask(lmask, aa.height, aa.width)
+        aa = supersampler.scale(func.work_clip.std.Transpose(), aah, aaw)
 
-        aa = _aa_mclip(aa, waa, mclip_up.std.Transpose())
+        mclip_up = resize_aa_mask(lmask.std.Transpose(), aa.width, aa.height)
 
-        aa = _aa_mclip(aa.std.Transpose(), waa.std.Transpose(), mclip_up)
+        aa = antialiaser.interpolate(aa, False, sclip=aa, mclip=mclip_up).std.Transpose()
+        aa = antialiaser.interpolate(aa, False, sclip=aa, mclip=mclip_up.std.Transpose())
 
         aa = downscaler.scale(aa, func.work_clip.width, func.work_clip.height)
 
         aa_merge = func.work_clip.std.MaskedMerge(aa, lmask)
 
         return func.return_clip(aa_merge)
```

### Comparing `vsaa-1.6.3/vsaa/mask.py` & `vsaa-1.7.0/vsaa/mask.py`

 * *Files identical despite different names*

### Comparing `vsaa-1.6.3/vsaa.egg-info/PKG-INFO` & `vsaa-1.7.0/vsaa.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vsaa
-Version: 1.6.3
+Version: 1.7.0
 Summary: VapourSynth anti aliasing and scaling functions
 Author: Setsugen no ao
 Author-email: setsugen@setsugen.dev
 Maintainer: Setsugen no ao
 Maintainer-email: setsugen@setsugen.dev
 Project-URL: Source Code, https://github.com/Irrational-Encoding-Wizardry/vs-aa
 Project-URL: Documentation, https://vsaa.encode.moe/en/latest/
```

