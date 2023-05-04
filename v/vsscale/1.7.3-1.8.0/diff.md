# Comparing `tmp/vsscale-1.7.3.tar.gz` & `tmp/vsscale-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vsscale-1.7.3.tar", last modified: Sun Mar 26 17:39:57 2023, max compression
+gzip compressed data, was "vsscale-1.8.0.tar", last modified: Thu May  4 21:58:58 2023, max compression
```

## Comparing `vsscale-1.7.3.tar` & `vsscale-1.8.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 17:39:57.003572 vsscale-1.7.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-03-26 17:39:35.000000 vsscale-1.7.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-03-26 17:39:57.003572 vsscale-1.7.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-03-26 17:39:35.000000 vsscale-1.7.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-03-26 17:39:57.003572 vsscale-1.7.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-03-26 17:39:35.000000 vsscale-1.7.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 17:39:56.999572 vsscale-1.7.3/vsscale/
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-03-26 17:39:35.000000 vsscale-1.7.3/vsscale/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-03-26 17:39:35.000000 vsscale-1.7.3/vsscale/_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-03-26 17:39:35.000000 vsscale-1.7.3/vsscale/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    20314 2023-03-26 17:39:35.000000 vsscale-1.7.3/vsscale/descale.py
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-03-26 17:39:35.000000 vsscale-1.7.3/vsscale/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9952 2023-03-26 17:39:35.000000 vsscale-1.7.3/vsscale/funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-03-26 17:39:35.000000 vsscale-1.7.3/vsscale/gamma.py
--rw-r--r--   0 runner    (1001) docker     (123)     5968 2023-03-26 17:39:35.000000 vsscale-1.7.3/vsscale/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4536 2023-03-26 17:39:35.000000 vsscale-1.7.3/vsscale/mask.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-26 17:39:35.000000 vsscale-1.7.3/vsscale/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    12697 2023-03-26 17:39:35.000000 vsscale-1.7.3/vsscale/scale.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 17:39:57.003572 vsscale-1.7.3/vsscale/shaders/
--rw-r--r--   0 runner    (1001) docker     (123)   246177 2023-03-26 17:39:35.000000 vsscale-1.7.3/vsscale/shaders/FSRCNNX_x2_16-0-4-1.glsl
--rw-r--r--   0 runner    (1001) docker     (123)   362441 2023-03-26 17:39:35.000000 vsscale-1.7.3/vsscale/shaders/FSRCNNX_x2_56-16-4-1.glsl
--rw-r--r--   0 runner    (1001) docker     (123)    70598 2023-03-26 17:39:35.000000 vsscale-1.7.3/vsscale/shaders/FSRCNNX_x2_8-0-4-1.glsl
--rw-r--r--   0 runner    (1001) docker     (123)     7444 2023-03-26 17:39:35.000000 vsscale-1.7.3/vsscale/shaders/SSimDownscaler.glsl
--rw-r--r--   0 runner    (1001) docker     (123)     7316 2023-03-26 17:39:35.000000 vsscale-1.7.3/vsscale/shaders/SSimSuperRes.glsl
--rw-r--r--   0 runner    (1001) docker     (123)     6240 2023-03-26 17:39:35.000000 vsscale-1.7.3/vsscale/shaders.py
--rw-r--r--   0 runner    (1001) docker     (123)     5548 2023-03-26 17:39:35.000000 vsscale-1.7.3/vsscale/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 17:39:56.999572 vsscale-1.7.3/vsscale.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-03-26 17:39:56.000000 vsscale-1.7.3/vsscale.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      620 2023-03-26 17:39:56.000000 vsscale-1.7.3/vsscale.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-26 17:39:56.000000 vsscale-1.7.3/vsscale.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-03-26 17:39:56.000000 vsscale-1.7.3/vsscale.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-26 17:39:56.000000 vsscale-1.7.3/vsscale.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:58:58.075980 vsscale-1.8.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-04 21:58:30.000000 vsscale-1.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-05-04 21:58:58.075980 vsscale-1.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-04 21:58:30.000000 vsscale-1.8.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-05-04 21:58:58.079980 vsscale-1.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-05-04 21:58:30.000000 vsscale-1.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:58:58.075980 vsscale-1.8.0/vsscale/
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-04 21:58:30.000000 vsscale-1.8.0/vsscale/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-04 21:58:30.000000 vsscale-1.8.0/vsscale/_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-05-04 21:58:30.000000 vsscale-1.8.0/vsscale/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20260 2023-05-04 21:58:30.000000 vsscale-1.8.0/vsscale/descale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-04 21:58:30.000000 vsscale-1.8.0/vsscale/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10001 2023-05-04 21:58:30.000000 vsscale-1.8.0/vsscale/funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-05-04 21:58:30.000000 vsscale-1.8.0/vsscale/gamma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5968 2023-05-04 21:58:30.000000 vsscale-1.8.0/vsscale/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4536 2023-05-04 21:58:30.000000 vsscale-1.8.0/vsscale/mask.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 21:58:30.000000 vsscale-1.8.0/vsscale/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    13778 2023-05-04 21:58:30.000000 vsscale-1.8.0/vsscale/scale.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:58:58.075980 vsscale-1.8.0/vsscale/shaders/
+-rw-r--r--   0 runner    (1001) docker     (123)   246177 2023-05-04 21:58:30.000000 vsscale-1.8.0/vsscale/shaders/FSRCNNX_x2_16-0-4-1.glsl
+-rw-r--r--   0 runner    (1001) docker     (123)   362441 2023-05-04 21:58:30.000000 vsscale-1.8.0/vsscale/shaders/FSRCNNX_x2_56-16-4-1.glsl
+-rw-r--r--   0 runner    (1001) docker     (123)    70598 2023-05-04 21:58:30.000000 vsscale-1.8.0/vsscale/shaders/FSRCNNX_x2_8-0-4-1.glsl
+-rw-r--r--   0 runner    (1001) docker     (123)     7444 2023-05-04 21:58:30.000000 vsscale-1.8.0/vsscale/shaders/SSimDownscaler.glsl
+-rw-r--r--   0 runner    (1001) docker     (123)     7316 2023-05-04 21:58:30.000000 vsscale-1.8.0/vsscale/shaders/SSimSuperRes.glsl
+-rw-r--r--   0 runner    (1001) docker     (123)     6240 2023-05-04 21:58:30.000000 vsscale-1.8.0/vsscale/shaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6205 2023-05-04 21:58:30.000000 vsscale-1.8.0/vsscale/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:58:58.075980 vsscale-1.8.0/vsscale.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-05-04 21:58:58.000000 vsscale-1.8.0/vsscale.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-04 21:58:58.000000 vsscale-1.8.0/vsscale.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 21:58:58.000000 vsscale-1.8.0/vsscale.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-04 21:58:58.000000 vsscale-1.8.0/vsscale.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-04 21:58:58.000000 vsscale-1.8.0/vsscale.egg-info/top_level.txt
```

### Comparing `vsscale-1.7.3/LICENSE` & `vsscale-1.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vsscale-1.7.3/PKG-INFO` & `vsscale-1.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vsscale
-Version: 1.7.3
+Version: 1.8.0
 Summary: VapourSynth (de)scaling functions
 Author: Setsugen no ao
 Author-email: setsugen@setsugen.dev
 Maintainer: Setsugen no ao
 Maintainer-email: setsugen@setsugen.dev
 Project-URL: Source Code, https://github.com/Irrational-Encoding-Wizardry/vs-scale
 Project-URL: Documentation, https://vsscale.encode.moe/en/latest/
```

### Comparing `vsscale-1.7.3/setup.cfg` & `vsscale-1.8.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `vsscale-1.7.3/setup.py` & `vsscale-1.8.0/setup.py`

 * *Files identical despite different names*

### Comparing `vsscale-1.7.3/vsscale/base.py` & `vsscale-1.8.0/vsscale/base.py`

 * *Files identical despite different names*

### Comparing `vsscale-1.7.3/vsscale/descale.py` & `vsscale-1.8.0/vsscale/descale.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from typing import Callable, Iterable, Literal, Sequence, cast, overload
 
 from vsaa import Nnedi3
 from vskernels import Catrom, Kernel, KernelT, Scaler, ScalerT, Spline144
 from vsmasktools import GenericMaskT, normalize_mask
 from vstools import (
     CustomValueError, FieldBased, FieldBasedT, FuncExceptT, core, depth, expect_bits, get_h, get_prop, get_w, get_y,
-    join, normalize_seq, split, vs
+    join, normalize_seq, split, to_arr, vs
 )
 
 from .helpers import scale_var_clip
 from .mask import descale_detail_mask
 from .types import DescaleAttempt, DescaleMode, DescaleModeWithInfo, DescaleResult, PlaneStatsKind
 
 __all__ = [
@@ -260,15 +260,15 @@
     :param result:          Return the :py:class:`DescaleResult` object.
                             If False, return the regularly rescaled output.
                             Default: False.
 
     :raises ValueError:     Number of given heights and width don't match.
     :raises ValueError:     No kernel is specified.
 
-    :returns:               Either a rescaled clip (mask applied, chroma readded),
+    :returns:               Either a rescaled clip (mask applied, chroma re-added),
                             or a :py:class:`DescaleResult` object containing the results from ``descale``.
     """
     assert clip.format
 
     if isinstance(height, int):
         heights = [height]
     else:
@@ -284,19 +284,16 @@
     if dst_width is None and dst_height:
         dest_width, dest_height = get_w(dst_height, clip), dst_height
     elif dst_height is None and dst_width:
         dest_width, dest_height = dst_width, get_h(dst_width, clip)
     else:
         dest_width, dest_height = clip.width, clip.height
 
-    if not isinstance(kernels, Sequence):
-        kernels = [kernels]
-
     norm_resolutions = list(zip(widths, heights))
-    norm_kernels = [Kernel.ensure_obj(kernel, descale) for kernel in kernels]
+    norm_kernels = [Kernel.ensure_obj(kernel, descale) for kernel in to_arr(kernels)]
 
     scaler = Scaler.ensure_obj(scaler, descale)
 
     if len(widths) != len(heights):
         raise CustomValueError('Number of heights and widths specified mismatch!', descale)
 
     if not norm_kernels:
```

### Comparing `vsscale-1.7.3/vsscale/exceptions.py` & `vsscale-1.8.0/vsscale/exceptions.py`

 * *Files identical despite different names*

### Comparing `vsscale-1.7.3/vsscale/funcs.py` & `vsscale-1.8.0/vsscale/funcs.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 
 from vsaa import Nnedi3
 from vsexprtools import ExprOp, combine, norm_expr
 from vskernels import Scaler, ScalerT
 from vsmasktools import ringing_mask
 from vsrgtools import LimitFilterMode, RepairMode, limit_filter, median_clips, repair, unsharp_masked
 from vstools import (
-    EXPR_VARS, ColorRange, CustomIndexError, CustomOverflowError, P, check_ref_clip, inject_self, scale_8bit, vs
+    EXPR_VARS, ColorRange, CustomIndexError, CustomOverflowError, P, check_ref_clip, inject_self, scale_8bit,
+    scale_value, vs
 )
 
 from .helpers import GenericScaler
 from .shaders import FSRCNNXShader, FSRCNNXShaderT
 
 __all__ = [
     'MergeScalers',
@@ -133,56 +134,57 @@
     @inject_self
     def scale(  # type: ignore
         self, clip: vs.VideoNode, width: int, height: int, shift: tuple[float, float] = (0, 0),
         *, smooth: vs.VideoNode | None = None, **kwargs: Any
     ) -> vs.VideoNode:
         assert (self.undershoot or self.undershoot == 0) and (self.overshoot or self.overshoot == 0)
 
-        fsrcnnx = self._ref_scaler.scale(clip, width, height, shift, **kwargs)
+        ref = self._ref_scaler.scale(clip, width, height, shift, **kwargs)
 
         if isinstance(self.reference, vs.VideoNode):
             smooth = self.reference  # type: ignore
 
             if shift != (0, 0):
                 smooth = self._kernel.shift(smooth, shift)  # type: ignore
         else:
             smooth = Scaler.ensure_obj(self.reference, self.__class__).scale(clip, width, height, shift)  # type: ignore
 
         assert smooth
 
-        check_ref_clip(fsrcnnx, smooth)
+        check_ref_clip(ref, smooth)
 
         range_out = ColorRange.from_video(clip, False) if self.range_out is None else self.range_out
 
-        fsr_weight = self.strength / 100
+        merge_weight = self.strength / 100
 
         if self.limit is True:
             expression = [
-                'x {fsr_weight} * y {ref_weight} * + up!',
+                'x {merge_weight} * y {ref_weight} * + up!',
                 '{overshoot} O!', '{undershoot} U!',
                 'up@ z O@ + > z O@ + up@ ? a U@ - < a U@ - up@ z O@ + > z O@ + up@ ? ?'
             ]
 
             if range_out is ColorRange.LIMITED:
                 expression.append(f'{scale_8bit(clip, 16)} {{clamp_max}} clamp')
 
             merged = norm_expr(
-                [fsrcnnx, smooth, smooth.std.Maximum(), smooth.std.Minimum()],
-                expression, fsr_weight=fsr_weight, ref_weight=1.0 - fsr_weight,
-                undershoot=self.undershoot * (2 ** 8), overshoot=self.overshoot * (2 ** 8),
+                [ref, smooth, smooth.std.Maximum(), smooth.std.Minimum()],
+                expression, merge_weight=merge_weight, ref_weight=1.0 - merge_weight,
+                undershoot=scale_value(self.undershoot, 32, clip),
+                overshoot=scale_value(self.overshoot, 32, clip),
                 clamp_max=[scale_8bit(clip, 235), scale_8bit(clip, 240)]
             )
         else:
-            merged = smooth.std.Merge(fsrcnnx, fsr_weight)
+            merged = smooth.std.Merge(ref, merge_weight)
 
             if isinstance(self.limit, RepairMode):
                 merged = repair(merged, smooth, self.limit)
 
         if self.operator is not None:
-            merge2 = combine([smooth, fsrcnnx], ExprOp.MIN)
+            merge2 = combine([smooth, ref], ExprOp.MIN)
 
             if self.masked:
                 merged = merged.std.MaskedMerge(merge2, ringing_mask(smooth))
             else:
                 merged = merge2
         elif self.masked:
             merged.std.MaskedMerge(smooth, ringing_mask(smooth))
```

### Comparing `vsscale-1.7.3/vsscale/gamma.py` & `vsscale-1.8.0/vsscale/gamma.py`

 * *Files identical despite different names*

### Comparing `vsscale-1.7.3/vsscale/helpers.py` & `vsscale-1.8.0/vsscale/helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -116,15 +116,15 @@
 
 def scale_var_clip(
     clip: vs.VideoNode,
     width: int | Callable[[Resolution], int] | None, height: int | Callable[[Resolution], int],
     shift: tuple[float, float] | Callable[[Resolution], tuple[float, float]] = (0, 0),
     scaler: Scaler | Callable[[Resolution], Scaler] = Nnedi3(), debug: bool = False
 ) -> vs.VideoNode:
-    """Scale a variable clip to constant or varibale resolution."""
+    """Scale a variable clip to constant or variable resolution."""
     if not debug:
         try:
             return scaler.scale(clip, width, height, shift)  # type: ignore
         except BaseException:
             pass
 
     _cached_clips = dict[str, vs.VideoNode]()
```

### Comparing `vsscale-1.7.3/vsscale/mask.py` & `vsscale-1.8.0/vsscale/mask.py`

 * *Files identical despite different names*

### Comparing `vsscale-1.7.3/vsscale/scale.py` & `vsscale-1.8.0/vsscale/scale.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,27 +2,27 @@
 
 from dataclasses import dataclass, field
 from functools import partial
 from math import ceil, floor, log2
 from typing import Any, Literal
 
 from vsexprtools import complexpr_available, expr_func, norm_expr
-from vskernels import Catrom, Scaler, ScalerT, SetsuCubic, ZewiaCubic
+from vskernels import Scaler, ScalerT, SetsuCubic, ZewiaCubic
 from vsrgtools import box_blur, gauss_blur
 from vstools import (
-    Matrix, MatrixT, PlanesT, Transfer, VSFunction, check_ref_clip, check_variable, core, depth,
-    fallback, get_depth, get_w, inject_self, vs, padder, DependencyNotFoundError, KwargsT, get_nvidia_version
+    DependencyNotFoundError, KwargsT, Matrix, MatrixT, PlanesT, Transfer, VSFunction, check_ref_clip, check_variable,
+    core, depth, fallback, get_depth, get_nvidia_version, inject_self, padder, vs
 )
 
 from .gamma import gamma2linear, linear2gamma
 from .helpers import GenericScaler
 
 __all__ = [
     'DPID',
-    'SSIM', 'ssim_downsample',
+    'SSIM',
     'DLISR',
     'Waifu2x'
 ]
 
 
 @dataclass
 class DPID(GenericScaler):
@@ -166,28 +166,14 @@
 
         if convert_csp is not None:
             d = self._kernel.resample(d, convert_csp[1], convert_csp[0])
 
         return depth(d, bits)
 
 
-def ssim_downsample(
-    clip: vs.VideoNode, width: int | None = None, height: int = 720,
-    smooth: int | float | VSFunction = ((3 ** 2 - 1) / 12) ** 0.5,
-    scaler: ScalerT = Catrom,
-    curve: Transfer | bool = False, sigmoid: bool = False,
-    shift: tuple[float, float] = (0, 0), epsilon: float = 1e-6
-) -> vs.VideoNode:
-    import warnings
-    warnings.warn("ssim_downsample is deprecated! You should use SSIM directly!", DeprecationWarning)
-    return SSIM(epsilon=epsilon, scaler=scaler).scale(
-        clip, fallback(width, get_w(height, clip)), height, shift, smooth, curve, sigmoid
-    )
-
-
 @dataclass
 class DLISR(GenericScaler):
     """Use Nvidia NGX Technology DLISR DNN to scale up nodes. https://developer.nvidia.com/rtx/ngx"""
 
     scaler: ScalerT = field(default_factory=lambda: DPID(0.5, SetsuCubic))
     """Scaler to use to downscale clip to desired resolution, if necessary."""
 
@@ -223,15 +209,15 @@
 @dataclass
 class Waifu2x(GenericScaler):
     """Use Waifu2x neural network to scale clips."""
 
     cuda: bool | Literal['trt'] | None = None
     """Whether to run this on cpu, gpu, or use trt technology. None will pick the fastest automatically."""
 
-    num_streams: int = 1
+    num_streams: int | None = None
     """Number of gpu streams for the model."""
 
     fp16: bool = True
     """Whether to use float16 precision if available."""
 
     device_id: int = 0
     """Id of the cuda device to use."""
@@ -259,80 +245,115 @@
 
     def __post_init__(self) -> None:
         try:
             from vsmlrt import Backend  # type: ignore
         except ModuleNotFoundError as e:
             raise DependencyNotFoundError(self.__class__, e)
 
-        bkwargs = (self.backend_kwargs or KwargsT()) | KwargsT(
-            num_streams=self.num_streams, fp16=self.fp16, device_id=self.device_id
-        )
+        bkwargs = (self.backend_kwargs or KwargsT()) | KwargsT(fp16=self.fp16, device_id=self.device_id)
 
         cuda = self.cuda
 
+        # All this will eventually be in vs-nn
         if cuda is None:
             try:
-                core.trt.DeviceProperties(self.device_id)
+                data: KwargsT = core.trt.DeviceProperties(self.device_id)  # type: ignore
+                memory = data.get('total_global_memory', 0)
+                def_num_streams = data.get('async_engine_count', 1)
+
                 cuda = 'trt'
+
+                bkwargs = KwargsT(
+                    workspace=memory / (1 << 22) if memory else None,
+                    use_cuda_graph=True, use_cublas=True, use_cudnn=True,
+                    use_edge_mask_convolutions=True, use_jit_convolutions=True,
+                    static_shape=True, heuristic=True, output_format=int(self.fp16),
+                    tf32=not self.fp16, force_fp16=self.fp16, num_streams=def_num_streams
+                ) | bkwargs
+
+                streams_info = 'OK' if bkwargs['num_streams'] == def_num_streams else 'MISMATCH'
+
+                core.log_message(
+                    vs.MESSAGE_TYPE_DEBUG,
+                    f'Selected [{data.get("name", b"<unknown>").decode("utf8")}] '
+                    f'with {f"{(memory / (1 << 30))}GiB" if memory else "<unknown>"} of VRAM, '
+                    f'num_streams={def_num_streams} ({streams_info})'
+                )
             except Exception:
                 cuda = get_nvidia_version() is not None
 
+        if bkwargs.get('num_streams', None) is None:
+            bkwargs.update(num_streams=fallback(self.num_streams, 1))
+
         if cuda is True:
-            self.backend = Backend.ORT_CUDA(**bkwargs)
+            if hasattr(core, 'ort'):
+                self.backend = Backend.ORT_CUDA(**bkwargs)
+            else:
+                self.backend = Backend.OV_GPU(**bkwargs)
         elif cuda is False:
-            self.backend = Backend.NCNN_VK(**bkwargs)
+            if hasattr(core, 'ncnn'):
+                self.backend = Backend.NCNN_VK(**bkwargs)
+            else:
+                bkwargs.pop('device_id')
+
+                if hasattr(core, 'ort'):
+                    self.backend = Backend.ORT_CPU(**bkwargs)
+                else:
+                    self.backend = Backend.OV_CPU(**bkwargs)
         else:
             self.backend = Backend.TRT(**bkwargs)
 
         super().__post_init__()
 
-    @inject_self
+    @inject_self.init_kwargs.clean
     def scale(  # type:ignore
-        self, clip: vs.VideoNode, width: int, height: int, shift: tuple[float, float] = (0, 0),
-        *, matrix: MatrixT | None = None, tiles: int | tuple[int, int] | None = None,
-        tilesize: int | tuple[int, int] | None = None, overlap: int | tuple[int, int] | None = None,
-        **kwargs: Any
+        self, clip: vs.VideoNode, width: int, height: int, shift: tuple[float, float] = (0, 0), **kwargs: Any
     ) -> vs.VideoNode:
         wclip = clip
 
         assert check_variable(clip, self.scale)
 
+        matrix = self.matrix
+        is_gray = clip.format.color_family is vs.GRAY
+        planes = 0 if is_gray else None
+        kwargs.update(tiles=self.tiles, tilesize=self.tilesize, overlap=self.overlap)
+
         if (is_upscale := width > clip.width or height > clip.width):
             from vsmlrt import Waifu2x, Waifu2xModel
 
-            kwargs.setdefault('tiles', tiles or self.tiles)
-            kwargs.setdefault('tilesize', tilesize or self.tilesize)
-            kwargs.setdefault('overlap', overlap or self.overlap)
-
             if clip.format.color_family is vs.YUV:
                 if not matrix:
                     matrix = Matrix.from_param(matrix or self.matrix, self.__class__) or Matrix.from_video(clip, False)
-                wclip = self._kernel.resample(wclip, vs.RGBS, Matrix.RGB, matrix)
+                wclip = self._kernel.resample(wclip, vs.RGBH if self.fp16 else vs.RGBS, Matrix.RGB, matrix)
             else:
-                wclip = depth(wclip, 32)
+                wclip = depth(wclip, 16 if self.fp16 else 32, vs.FLOAT)
 
-                if clip.format.color_family is vs.GRAY:
+                if is_gray:
                     wclip = wclip.std.ShufflePlanes(0, vs.RGB)
 
-            wclip = wclip.std.Limiter()
+            try:
+                wclip = wclip.std.Limiter(planes=planes)
+            except vs.Error:
+                wclip = norm_expr(wclip, 'x 0 1 clamp', planes=planes)
 
             mult = max(int(log2(ceil(size))) for size in (width / wclip.width, height / wclip.height))
 
             for _ in range(mult):
                 padding = self.mod_padding(wclip)
 
                 padded = padder(wclip, *padding)
 
                 upscaled = Waifu2x(
                     padded, noise=-1, scale=2, model=Waifu2xModel.cunet, backend=self.backend, **kwargs
                 )
 
                 cropped = upscaled.std.Crop(*(p * 2 for p in padding))
 
-                cfix = norm_expr(cropped, 'x 0.5 255 / +')
-
-                wclip = cfix.std.Limiter()
+                try:
+                    wclip = norm_expr(cropped, 'x 0.5 255 / + 0 1 clamp', planes=planes)
+                except RuntimeError:
+                    wclip = norm_expr(depth(cropped, 32), 'x 0.5 255 / + 0 max 1 min', planes=planes)
 
-            if clip.format.color_family is vs.GRAY:
+            if is_gray:
                 wclip = wclip.std.ShufflePlanes(0, vs.GRAY)
 
         return self._finish_scale(wclip, clip, width, height, shift, matrix, is_upscale)
```

### Comparing `vsscale-1.7.3/vsscale/shaders/FSRCNNX_x2_16-0-4-1.glsl` & `vsscale-1.8.0/vsscale/shaders/FSRCNNX_x2_16-0-4-1.glsl`

 * *Files identical despite different names*

### Comparing `vsscale-1.7.3/vsscale/shaders/FSRCNNX_x2_56-16-4-1.glsl` & `vsscale-1.8.0/vsscale/shaders/FSRCNNX_x2_56-16-4-1.glsl`

 * *Files identical despite different names*

### Comparing `vsscale-1.7.3/vsscale/shaders/FSRCNNX_x2_8-0-4-1.glsl` & `vsscale-1.8.0/vsscale/shaders/FSRCNNX_x2_8-0-4-1.glsl`

 * *Files identical despite different names*

### Comparing `vsscale-1.7.3/vsscale/shaders/SSimDownscaler.glsl` & `vsscale-1.8.0/vsscale/shaders/SSimDownscaler.glsl`

 * *Files identical despite different names*

### Comparing `vsscale-1.7.3/vsscale/shaders/SSimSuperRes.glsl` & `vsscale-1.8.0/vsscale/shaders/SSimSuperRes.glsl`

 * *Files identical despite different names*

### Comparing `vsscale-1.7.3/vsscale/shaders.py` & `vsscale-1.8.0/vsscale/shaders.py`

 * *Files identical despite different names*

### Comparing `vsscale-1.7.3/vsscale/types.py` & `vsscale-1.8.0/vsscale/types.py`

 * *Files 20% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     rescaled: vs.VideoNode
     """Descaled frame reupscaled with the same kernel."""
 
     diff: vs.VideoNode
     """The subtractive difference between the original and descaled frame."""
 
     kernel: Kernel
-    """Kernel used"""
+    """Kernel used for descaling."""
 
     @classmethod
     def from_args(
         cls, clip: vs.VideoNode, width: int, height: int, shift: tuple[float, float],
         kernel: Kernel, mode: DescaleModeWithInfo, **kwargs: VSMapValue
     ) -> DescaleAttempt:
         """Get a DescaleAttempt from args. Calculate difference nodes too."""
@@ -65,33 +65,46 @@
 
 
 @dataclass
 class DescaleResult:
     """Dataclass representing a complete result of vsscale.descale."""
 
     descaled: vs.VideoNode
-    """Descaled clip, can be var res"""
+    """The descaled clip. Can be a variable resolution."""
 
     rescaled: vs.VideoNode
-    """Rescaled clip, can be var res"""
+    """
+    The descaled clip reupscaled to the source resolution using the same kernel used to descale.
+    Can be a variable resolution clip.
+    """
 
     upscaled: vs.VideoNode | None
-    """Upscaled clip"""
+    """The descaled clip reupscaled using the given upscaler."""
 
     error_mask: vs.VideoNode | None
-    """Descale error mask"""
+    """
+    The descale error mask. This catches the big differences
+    between the source clip and the rescaled clip as a mask.
+    If no \"mask\" is passed, this attribute will be None.
+    """
 
     pproc_mask: vs.VideoNode | None
-    """Post process mask"""
+    """
+    The post-processing mask. This is the second mask passed to \"mask\".
+    If no \"mask\" is passed, this attribute will be None.
+    """
 
     attempts: list[DescaleAttempt]
-    """Descale attempts used"""
+    """
+    Descale attempts made. These are used to determine
+    the correct kernel if multiple \"Kernels\" were passed.
+    """
 
     out: vs.VideoNode
-    """Normal output"""
+    """The final clip that is returned during regular usage with \"result=False\"."""
 
 
 class PlaneStatsKind(CustomStrEnum):
     """Type of PlaneStats comparing to use."""
 
     AVG = 'Average'
     MIN = 'Min'
@@ -178,14 +191,14 @@
     def __hash__(self) -> int:
         return hash(self._name_)
 
 
 @dataclass
 class DescaleModeWithInfo:
     mode: DescaleMode
-    """Actual descale mode"""
+    """Actual descale mode used for descaling."""
 
     thr: float = field(default=5e-8)
     """Diff threshold."""
 
     op: ComparatorFunc = field(default_factory=lambda: max)
     """Operator used for generic sorting."""
```

### Comparing `vsscale-1.7.3/vsscale.egg-info/PKG-INFO` & `vsscale-1.8.0/vsscale.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vsscale
-Version: 1.7.3
+Version: 1.8.0
 Summary: VapourSynth (de)scaling functions
 Author: Setsugen no ao
 Author-email: setsugen@setsugen.dev
 Maintainer: Setsugen no ao
 Maintainer-email: setsugen@setsugen.dev
 Project-URL: Source Code, https://github.com/Irrational-Encoding-Wizardry/vs-scale
 Project-URL: Documentation, https://vsscale.encode.moe/en/latest/
```

### Comparing `vsscale-1.7.3/vsscale.egg-info/SOURCES.txt` & `vsscale-1.8.0/vsscale.egg-info/SOURCES.txt`

 * *Files identical despite different names*

