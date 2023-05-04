# Comparing `tmp/MoonMag-1.5.2.tar.gz` & `tmp/MoonMag-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MoonMag-1.5.2.tar", last modified: Sat Nov 26 03:04:45 2022, max compression
+gzip compressed data, was "MoonMag-1.5.3.tar", last modified: Thu May  4 10:15:55 2023, max compression
```

## Comparing `MoonMag-1.5.2.tar` & `MoonMag-1.5.3.tar`

### file list

```diff
@@ -1,113 +1,119 @@
-drwxr-xr-x   0 mjstyczi   (503) staff       (20)        0 2022-11-26 03:04:45.962837 MoonMag-1.5.2/
--rw-r--r--   0 mjstyczi   (503) staff       (20)    35141 2022-04-15 18:33:04.000000 MoonMag-1.5.2/LICENSE
--rw-r--r--   0 mjstyczi   (503) staff       (20)      136 2022-05-10 06:48:50.000000 MoonMag-1.5.2/MANIFEST.in
--rw-r--r--   0 mjstyczi   (503) staff       (20)     6873 2022-11-26 03:04:45.962999 MoonMag-1.5.2/PKG-INFO
--rw-r--r--   0 mjstyczi   (503) staff       (20)     6221 2022-11-26 03:02:18.000000 MoonMag-1.5.2/README.md
--rw-r--r--   0 mjstyczi   (503) staff       (20)       85 2022-05-10 03:25:16.000000 MoonMag-1.5.2/pyproject.toml
--rw-r--r--   0 mjstyczi   (503) staff       (20)      928 2022-11-26 03:04:45.963786 MoonMag-1.5.2/setup.cfg
--rw-r--r--   0 mjstyczi   (503) staff       (20)       37 2022-07-26 23:29:26.000000 MoonMag-1.5.2/setup.py
-drwxr-xr-x   0 mjstyczi   (503) staff       (20)        0 2022-11-26 03:04:45.885930 MoonMag-1.5.2/src/
-drwxr-xr-x   0 mjstyczi   (503) staff       (20)        0 2022-11-26 03:04:45.899663 MoonMag-1.5.2/src/MoonMag/
--rw-r--r--   0 mjstyczi   (503) staff       (20)      195 2022-05-10 05:41:07.000000 MoonMag-1.5.2/src/MoonMag/__init__.py
--rw-r--r--   0 mjstyczi   (503) staff       (20)    68660 2022-11-08 22:10:08.000000 MoonMag-1.5.2/src/MoonMag/asymmetry_funcs.py
--rw-r--r--   0 mjstyczi   (503) staff       (20)     2039 2022-04-15 18:33:04.000000 MoonMag-1.5.2/src/MoonMag/calc_Ganymede_induced.py
--rw-r--r--   0 mjstyczi   (503) staff       (20)     7506 2022-05-30 18:41:32.000000 MoonMag-1.5.2/src/MoonMag/calc_trajec_induced.py
--rw-r--r--   0 mjstyczi   (503) staff       (20)     4706 2022-11-26 03:02:25.000000 MoonMag-1.5.2/src/MoonMag/config.py
--rw-r--r--   0 mjstyczi   (503) staff       (20)    21701 2022-11-13 12:39:07.000000 MoonMag-1.5.2/src/MoonMag/eval_induced_field.py
-drwxr-xr-x   0 mjstyczi   (503) staff       (20)        0 2022-11-26 03:04:45.911328 MoonMag-1.5.2/src/MoonMag/excitation/
--rw-r--r--   0 mjstyczi   (503) staff       (20)     1570 2022-04-15 18:33:04.000000 MoonMag-1.5.2/src/MoonMag/excitation/Be1xyz.txt
--rw-r--r--   0 mjstyczi   (503) staff       (20)     1193 2022-04-15 18:33:04.000000 MoonMag-1.5.2/src/MoonMag/excitation/Be1xyz_Callisto.txt
--rw-r--r--   0 mjstyczi   (503) staff       (20)     1570 2022-04-15 18:33:04.000000 MoonMag-1.5.2/src/MoonMag/excitation/Be1xyz_Europa.txt
--rw-r--r--   0 mjstyczi   (503) staff       (20)     1122 2022-04-15 18:33:04.000000 MoonMag-1.5.2/src/MoonMag/excitation/Be1xyz_Miranda.txt
--rw-r--r--   0 mjstyczi   (503) staff       (20)      496 2022-04-15 18:33:04.000000 MoonMag-1.5.2/src/MoonMag/excitation/Be1xyz_Triton.txt
--rw-r--r--   0 mjstyczi   (503) staff       (20)     1066 2022-04-15 18:33:04.000000 MoonMag-1.5.2/src/MoonMag/excitation/Be2xyz.txt
--rw-r--r--   0 mjstyczi   (503) staff       (20)      319 2022-04-15 18:33:04.000000 MoonMag-1.5.2/src/MoonMag/excitation/orbital_Be1xyz_Callisto.txt
--rw-r--r--   0 mjstyczi   (503) staff       (20)      317 2022-04-15 18:33:04.000000 MoonMag-1.5.2/src/MoonMag/excitation/orbital_Be1xyz_Europa.txt
--rw-r--r--   0 mjstyczi   (503) staff       (20)      227 2022-04-15 18:33:04.000000 MoonMag-1.5.2/src/MoonMag/excitation/orbital_Be1xyz_Miranda.txt
--rw-r--r--   0 mjstyczi   (503) staff       (20)      231 2022-04-15 18:33:04.000000 MoonMag-1.5.2/src/MoonMag/excitation/orbital_Be1xyz_Triton.txt
--rw-r--r--   0 mjstyczi   (503) staff       (20)      318 2022-04-15 18:33:04.000000 MoonMag-1.5.2/src/MoonMag/excitation/synodic_Be1xyz_Callisto.txt
--rw-r--r--   0 mjstyczi   (503) staff       (20)      306 2022-04-15 18:33:04.000000 MoonMag-1.5.2/src/MoonMag/excitation/synodic_Be1xyz_Europa.txt
--rw-r--r--   0 mjstyczi   (503) staff       (20)      222 2022-04-15 18:33:04.000000 MoonMag-1.5.2/src/MoonMag/excitation/synodic_Be1xyz_Miranda.txt
--rw-r--r--   0 mjstyczi   (503) staff       (20)      227 2022-04-15 18:33:04.000000 MoonMag-1.5.2/src/MoonMag/excitation/synodic_Be1xyz_Triton.txt
--rw-r--r--   0 mjstyczi   (503) staff       (20)   183760 2022-11-08 22:14:09.000000 MoonMag-1.5.2/src/MoonMag/field_xyz.py
-drwxr-xr-x   0 mjstyczi   (503) staff       (20)        0 2022-11-26 03:04:45.919733 MoonMag-1.5.2/src/MoonMag/induced/
--rw-r--r--   0 mjstyczi   (503) staff       (20)  4460760 2022-05-10 17:37:41.000000 MoonMag-1.5.2/src/MoonMag/induced/Xid_values_n1_p10_np11.mat
--rw-r--r--   0 mjstyczi   (503) staff       (20)    37080 2022-04-15 18:33:04.000000 MoonMag-1.5.2/src/MoonMag/induced/Xid_values_n1_p2_np3.mat
--rw-r--r--   0 mjstyczi   (503) staff       (20)   230616 2022-04-15 18:33:04.000000 MoonMag-1.5.2/src/MoonMag/induced/Xid_values_n1_p4_np5.mat
--rw-r--r--   0 mjstyczi   (503) staff       (20)  2073816 2022-04-15 18:33:04.000000 MoonMag-1.5.2/src/MoonMag/induced/Xid_values_n1_p8_np9.mat
-drwxr-xr-x   0 mjstyczi   (503) staff       (20)        0 2022-11-26 03:04:45.962431 MoonMag-1.5.2/src/MoonMag/interior/
--rw-r--r--   0 mjstyczi   (503) staff       (20)      702 2022-04-15 18:33:04.000000 MoonMag-1.5.2/src/MoonMag/interior/degree1_shapes.txt
--rw-r--r--   0 mjstyczi   (503) staff       (20)      384 2022-04-15 18:33:04.000000 MoonMag-1.5.2/src/MoonMag/interior/degree1_shapes_Callisto.txt
--rw-r--r--   0 mjstyczi   (503) staff       (20)       54 2022-04-15 18:33:04.000000 MoonMag-1.5.2/src/MoonMag/interior/degree1_shapes_Europa_Tobie.txt
--rw-r--r--   0 mjstyczi   (503) staff       (20)       36 2022-04-15 18:33:04.000000 MoonMag-1.5.2/src/MoonMag/interior/degree1_shapes_Europa_prev.txt
--rw-r--r--   0 mjstyczi   (503) staff       (20)      702 2022-04-15 18:33:04.000000 MoonMag-1.5.2/src/MoonMag/interior/degree1_shapes_Miranda.txt
--rw-r--r--   0 mjstyczi   (503) staff       (20)      444 2022-04-15 18:33:04.000000 MoonMag-1.5.2/src/MoonMag/interior/degree1_shapes_Triton.txt
--rw-r--r--   0 mjstyczi   (503) staff       (20)     1247 2022-04-15 18:33:04.000000 MoonMag-1.5.2/src/MoonMag/interior/degree2_shapes.txt
--rw-r--r--   0 mjstyczi   (503) staff       (20)      101 2022-04-15 18:33:04.000000 MoonMag-1.5.2/src/MoonMag/interior/degree2_shapes_Callisto.txt
--rw-r--r--   0 mjstyczi   (503) staff       (20)      521 2022-04-15 18:33:04.000000 MoonMag-1.5.2/src/MoonMag/interior/degree2_shapes_Europa_Tobie.txt
--rw-r--r--   0 mjstyczi   (503) staff       (20)       81 2022-04-15 18:33:04.000000 MoonMag-1.5.2/src/MoonMag/interior/degree2_shapes_Europa_prev.txt
--rw-r--r--   0 mjstyczi   (503) staff       (20)     1247 2022-04-15 18:33:04.000000 MoonMag-1.5.2/src/MoonMag/interior/degree2_shapes_Miranda.txt
--rw-r--r--   0 mjstyczi   (503) staff       (20)      111 2022-04-15 18:33:04.000000 MoonMag-1.5.2/src/MoonMag/interior/degree2_shapes_Triton.txt
--rw-r--r--   0 mjstyczi   (503) staff       (20)     1762 2022-04-15 18:33:04.000000 MoonMag-1.5.2/src/MoonMag/interior/degree3_shapes.txt
--rw-r--r--   0 mjstyczi   (503) staff       (20)      142 2022-04-15 18:33:04.000000 MoonMag-1.5.2/src/MoonMag/interior/degree3_shapes_Callisto.txt
--rw-r--r--   0 mjstyczi   (503) staff       (20)      128 2022-04-15 18:33:04.000000 MoonMag-1.5.2/src/MoonMag/interior/degree3_shapes_Europa_Tobie.txt
--rw-r--r--   0 mjstyczi   (503) staff       (20)       86 2022-04-15 18:33:04.000000 MoonMag-1.5.2/src/MoonMag/interior/degree3_shapes_Europa_prev.txt
--rw-r--r--   0 mjstyczi   (503) staff       (20)     1762 2022-04-15 18:33:04.000000 MoonMag-1.5.2/src/MoonMag/interior/degree3_shapes_Miranda.txt
--rw-r--r--   0 mjstyczi   (503) staff       (20)      156 2022-04-15 18:33:04.000000 MoonMag-1.5.2/src/MoonMag/interior/degree3_shapes_Triton.txt
--rw-r--r--   0 mjstyczi   (503) staff       (20)     2337 2022-04-15 18:33:04.000000 MoonMag-1.5.2/src/MoonMag/interior/degree4_shapes.txt
--rw-r--r--   0 mjstyczi   (503) staff       (20)      183 2022-04-15 18:33:04.000000 MoonMag-1.5.2/src/MoonMag/interior/degree4_shapes_Callisto.txt
--rw-r--r--   0 mjstyczi   (503) staff       (20)      770 2022-04-15 18:33:04.000000 MoonMag-1.5.2/src/MoonMag/interior/degree4_shapes_Europa_Tobie.txt
--rw-r--r--   0 mjstyczi   (503) staff       (20)      111 2022-04-15 18:33:04.000000 MoonMag-1.5.2/src/MoonMag/interior/degree4_shapes_Europa_prev.txt
--rw-r--r--   0 mjstyczi   (503) staff       (20)     2337 2022-04-15 18:33:04.000000 MoonMag-1.5.2/src/MoonMag/interior/degree4_shapes_Miranda.txt
--rw-r--r--   0 mjstyczi   (503) staff       (20)      201 2022-04-15 18:33:04.000000 MoonMag-1.5.2/src/MoonMag/interior/degree4_shapes_Triton.txt
--rw-r--r--   0 mjstyczi   (503) staff       (20)     2870 2022-04-15 18:33:04.000000 MoonMag-1.5.2/src/MoonMag/interior/degree5_shapes.txt
--rw-r--r--   0 mjstyczi   (503) staff       (20)      224 2022-04-15 18:33:04.000000 MoonMag-1.5.2/src/MoonMag/interior/degree5_shapes_Callisto.txt
--rw-r--r--   0 mjstyczi   (503) staff       (20)      202 2022-04-15 18:33:04.000000 MoonMag-1.5.2/src/MoonMag/interior/degree5_shapes_Europa_Tobie.txt
--rw-r--r--   0 mjstyczi   (503) staff       (20)      136 2022-04-15 18:33:04.000000 MoonMag-1.5.2/src/MoonMag/interior/degree5_shapes_Europa_prev.txt
--rw-r--r--   0 mjstyczi   (503) staff       (20)     2870 2022-04-15 18:33:04.000000 MoonMag-1.5.2/src/MoonMag/interior/degree5_shapes_Miranda.txt
--rw-r--r--   0 mjstyczi   (503) staff       (20)      246 2022-04-15 18:33:04.000000 MoonMag-1.5.2/src/MoonMag/interior/degree5_shapes_Triton.txt
--rw-r--r--   0 mjstyczi   (503) staff       (20)     3409 2022-04-15 18:33:04.000000 MoonMag-1.5.2/src/MoonMag/interior/degree6_shapes.txt
--rw-r--r--   0 mjstyczi   (503) staff       (20)      265 2022-04-15 18:33:04.000000 MoonMag-1.5.2/src/MoonMag/interior/degree6_shapes_Callisto.txt
--rw-r--r--   0 mjstyczi   (503) staff       (20)      239 2022-04-15 18:33:04.000000 MoonMag-1.5.2/src/MoonMag/interior/degree6_shapes_Europa_Tobie.txt
--rw-r--r--   0 mjstyczi   (503) staff       (20)      161 2022-04-15 18:33:04.000000 MoonMag-1.5.2/src/MoonMag/interior/degree6_shapes_Europa_prev.txt
--rw-r--r--   0 mjstyczi   (503) staff       (20)     3409 2022-04-15 18:33:04.000000 MoonMag-1.5.2/src/MoonMag/interior/degree6_shapes_Miranda.txt
--rw-r--r--   0 mjstyczi   (503) staff       (20)      291 2022-04-15 18:33:04.000000 MoonMag-1.5.2/src/MoonMag/interior/degree6_shapes_Triton.txt
--rw-r--r--   0 mjstyczi   (503) staff       (20)     4002 2022-04-15 18:33:04.000000 MoonMag-1.5.2/src/MoonMag/interior/degree7_shapes.txt
--rw-r--r--   0 mjstyczi   (503) staff       (20)      306 2022-04-15 18:33:04.000000 MoonMag-1.5.2/src/MoonMag/interior/degree7_shapes_Callisto.txt
--rw-r--r--   0 mjstyczi   (503) staff       (20)      276 2022-04-15 18:33:04.000000 MoonMag-1.5.2/src/MoonMag/interior/degree7_shapes_Europa_Tobie.txt
--rw-r--r--   0 mjstyczi   (503) staff       (20)      186 2022-04-15 18:33:04.000000 MoonMag-1.5.2/src/MoonMag/interior/degree7_shapes_Europa_prev.txt
--rw-r--r--   0 mjstyczi   (503) staff       (20)     4002 2022-04-15 18:33:04.000000 MoonMag-1.5.2/src/MoonMag/interior/degree7_shapes_Miranda.txt
--rw-r--r--   0 mjstyczi   (503) staff       (20)      336 2022-04-15 18:33:04.000000 MoonMag-1.5.2/src/MoonMag/interior/degree7_shapes_Triton.txt
--rw-r--r--   0 mjstyczi   (503) staff       (20)     4505 2022-04-15 18:33:04.000000 MoonMag-1.5.2/src/MoonMag/interior/degree8_shapes.txt
--rw-r--r--   0 mjstyczi   (503) staff       (20)      347 2022-04-15 18:33:04.000000 MoonMag-1.5.2/src/MoonMag/interior/degree8_shapes_Callisto.txt
--rw-r--r--   0 mjstyczi   (503) staff       (20)      313 2022-04-15 18:33:04.000000 MoonMag-1.5.2/src/MoonMag/interior/degree8_shapes_Europa_Tobie.txt
--rw-r--r--   0 mjstyczi   (503) staff       (20)      211 2022-04-15 18:33:04.000000 MoonMag-1.5.2/src/MoonMag/interior/degree8_shapes_Europa_prev.txt
--rw-r--r--   0 mjstyczi   (503) staff       (20)     4505 2022-04-15 18:33:04.000000 MoonMag-1.5.2/src/MoonMag/interior/degree8_shapes_Miranda.txt
--rw-r--r--   0 mjstyczi   (503) staff       (20)      381 2022-04-15 18:33:04.000000 MoonMag-1.5.2/src/MoonMag/interior/degree8_shapes_Triton.txt
--rw-r--r--   0 mjstyczi   (503) staff       (20)     5384 2022-04-15 18:33:04.000000 MoonMag-1.5.2/src/MoonMag/interior/depth_chi_pq_shape_Callisto.txt
--rw-r--r--   0 mjstyczi   (503) staff       (20)     5452 2022-04-15 18:33:04.000000 MoonMag-1.5.2/src/MoonMag/interior/depth_chi_pq_shape_Enceladus.txt
--rw-r--r--   0 mjstyczi   (503) staff       (20)     5392 2022-04-15 18:33:04.000000 MoonMag-1.5.2/src/MoonMag/interior/depth_chi_pq_shape_Europa.txt
--rw-r--r--   0 mjstyczi   (503) staff       (20)     5391 2022-04-15 18:33:04.000000 MoonMag-1.5.2/src/MoonMag/interior/depth_chi_pq_shape_Europa_Tobie.txt
--rw-r--r--   0 mjstyczi   (503) staff       (20)     5446 2022-04-15 18:33:04.000000 MoonMag-1.5.2/src/MoonMag/interior/depth_chi_pq_shape_Miranda.txt
--rw-r--r--   0 mjstyczi   (503) staff       (20)     5386 2022-04-15 18:33:04.000000 MoonMag-1.5.2/src/MoonMag/interior/depth_chi_pq_shape_Triton.txt
--rw-r--r--   0 mjstyczi   (503) staff       (20)     5396 2022-04-15 18:33:04.000000 MoonMag-1.5.2/src/MoonMag/interior/gravity_Europa_Tobie.txt
--rw-r--r--   0 mjstyczi   (503) staff       (20)     3766 2022-04-15 18:33:04.000000 MoonMag-1.5.2/src/MoonMag/interior/interior_model_asym.txt
--rw-r--r--   0 mjstyczi   (503) staff       (20)      224 2022-11-07 13:30:07.000000 MoonMag-1.5.2/src/MoonMag/interior/interior_model_asym_Callisto.txt
--rw-r--r--   0 mjstyczi   (503) staff       (20)      156 2022-11-07 13:30:01.000000 MoonMag-1.5.2/src/MoonMag/interior/interior_model_asym_Enceladus.txt
--rw-r--r--   0 mjstyczi   (503) staff       (20)      226 2022-11-07 13:29:51.000000 MoonMag-1.5.2/src/MoonMag/interior/interior_model_asym_Europa_Tobie_high.txt
--rw-r--r--   0 mjstyczi   (503) staff       (20)      226 2022-11-07 13:29:44.000000 MoonMag-1.5.2/src/MoonMag/interior/interior_model_asym_Europa_Tobie_low.txt
--rw-r--r--   0 mjstyczi   (503) staff       (20)       93 2022-11-07 13:29:57.000000 MoonMag-1.5.2/src/MoonMag/interior/interior_model_asym_Europa_prev.txt
--rw-r--r--   0 mjstyczi   (503) staff       (20)      240 2022-11-07 13:29:46.000000 MoonMag-1.5.2/src/MoonMag/interior/interior_model_asym_Miranda.txt
--rw-r--r--   0 mjstyczi   (503) staff       (20)      244 2022-11-07 13:29:35.000000 MoonMag-1.5.2/src/MoonMag/interior/interior_model_asym_Triton.txt
--rw-r--r--   0 mjstyczi   (503) staff       (20)     1160 2022-04-15 18:33:04.000000 MoonMag-1.5.2/src/MoonMag/plot_Aes.py
--rw-r--r--   0 mjstyczi   (503) staff       (20)    53342 2022-11-26 02:56:09.000000 MoonMag-1.5.2/src/MoonMag/plotting_funcs.py
--rw-r--r--   0 mjstyczi   (503) staff       (20)     1375 2022-11-07 13:25:00.000000 MoonMag-1.5.2/src/MoonMag/reduce_interior_model.py
--rw-r--r--   0 mjstyczi   (503) staff       (20)     7192 2022-11-08 22:26:02.000000 MoonMag-1.5.2/src/MoonMag/run_all.py
--rw-r--r--   0 mjstyczi   (503) staff       (20)    17358 2022-11-08 22:08:20.000000 MoonMag-1.5.2/src/MoonMag/symmetry_funcs.py
--rw-r--r--   0 mjstyczi   (503) staff       (20)    20987 2022-11-07 13:18:43.000000 MoonMag-1.5.2/src/MoonMag/trajec_analysis.py
-drwxr-xr-x   0 mjstyczi   (503) staff       (20)        0 2022-11-26 03:04:45.903256 MoonMag-1.5.2/src/MoonMag.egg-info/
--rw-r--r--   0 mjstyczi   (503) staff       (20)     6873 2022-11-26 03:04:45.000000 MoonMag-1.5.2/src/MoonMag.egg-info/PKG-INFO
--rw-r--r--   0 mjstyczi   (503) staff       (20)     4552 2022-11-26 03:04:45.000000 MoonMag-1.5.2/src/MoonMag.egg-info/SOURCES.txt
--rw-r--r--   0 mjstyczi   (503) staff       (20)        1 2022-11-26 03:04:45.000000 MoonMag-1.5.2/src/MoonMag.egg-info/dependency_links.txt
--rw-r--r--   0 mjstyczi   (503) staff       (20)       75 2022-11-26 03:04:45.000000 MoonMag-1.5.2/src/MoonMag.egg-info/requires.txt
--rw-r--r--   0 mjstyczi   (503) staff       (20)        8 2022-11-26 03:04:45.000000 MoonMag-1.5.2/src/MoonMag.egg-info/top_level.txt
+drwxr-xr-x   0 mjstyczi   (503) staff       (20)        0 2023-05-04 10:15:55.412465 MoonMag-1.5.3/
+-rw-r--r--   0 mjstyczi   (503) staff       (20)    35141 2022-04-15 18:33:04.000000 MoonMag-1.5.3/LICENSE
+-rw-r--r--   0 mjstyczi   (503) staff       (20)      140 2023-04-29 01:19:49.000000 MoonMag-1.5.3/MANIFEST.in
+drwxr-xr-x   0 mjstyczi   (503) staff       (20)        0 2023-05-04 10:15:55.329437 MoonMag-1.5.3/MoonMag/
+-rw-r--r--   0 mjstyczi   (503) staff       (20)      195 2022-05-10 05:41:07.000000 MoonMag-1.5.3/MoonMag/__init__.py
+-rw-r--r--   0 mjstyczi   (503) staff       (20)    78531 2023-05-04 00:52:19.000000 MoonMag-1.5.3/MoonMag/asymmetry_funcs.py
+-rw-r--r--   0 mjstyczi   (503) staff       (20)     2039 2022-04-15 18:33:04.000000 MoonMag-1.5.3/MoonMag/calc_Ganymede_induced.py
+-rw-r--r--   0 mjstyczi   (503) staff       (20)     7506 2022-05-30 18:41:32.000000 MoonMag-1.5.3/MoonMag/calc_trajec_induced.py
+-rw-r--r--   0 mjstyczi   (503) staff       (20)     5413 2023-05-04 10:03:10.000000 MoonMag-1.5.3/MoonMag/config.py
+-rw-r--r--   0 mjstyczi   (503) staff       (20)    22664 2023-05-04 10:12:17.000000 MoonMag-1.5.3/MoonMag/eval_induced_field.py
+drwxr-xr-x   0 mjstyczi   (503) staff       (20)        0 2023-05-04 10:15:55.338642 MoonMag-1.5.3/MoonMag/excitation/
+-rw-r--r--   0 mjstyczi   (503) staff       (20)     1570 2022-04-15 18:33:04.000000 MoonMag-1.5.3/MoonMag/excitation/Be1xyz.txt
+-rw-r--r--   0 mjstyczi   (503) staff       (20)     1193 2023-05-04 07:33:40.000000 MoonMag-1.5.3/MoonMag/excitation/Be1xyz_Callisto.txt
+-rw-r--r--   0 mjstyczi   (503) staff       (20)     1570 2022-04-15 18:33:04.000000 MoonMag-1.5.3/MoonMag/excitation/Be1xyz_Europa.txt
+-rw-r--r--   0 mjstyczi   (503) staff       (20)     1122 2022-04-15 18:33:04.000000 MoonMag-1.5.3/MoonMag/excitation/Be1xyz_Miranda.txt
+-rw-r--r--   0 mjstyczi   (503) staff       (20)      496 2022-04-15 18:33:04.000000 MoonMag-1.5.3/MoonMag/excitation/Be1xyz_Triton.txt
+-rw-r--r--   0 mjstyczi   (503) staff       (20)     1066 2022-04-15 18:33:04.000000 MoonMag-1.5.3/MoonMag/excitation/Be2xyz.txt
+-rw-r--r--   0 mjstyczi   (503) staff       (20)      319 2022-04-15 18:33:04.000000 MoonMag-1.5.3/MoonMag/excitation/orbital_Be1xyz_Callisto.txt
+-rw-r--r--   0 mjstyczi   (503) staff       (20)      317 2022-04-15 18:33:04.000000 MoonMag-1.5.3/MoonMag/excitation/orbital_Be1xyz_Europa.txt
+-rw-r--r--   0 mjstyczi   (503) staff       (20)      227 2022-04-15 18:33:04.000000 MoonMag-1.5.3/MoonMag/excitation/orbital_Be1xyz_Miranda.txt
+-rw-r--r--   0 mjstyczi   (503) staff       (20)      231 2022-04-15 18:33:04.000000 MoonMag-1.5.3/MoonMag/excitation/orbital_Be1xyz_Triton.txt
+-rw-r--r--   0 mjstyczi   (503) staff       (20)      318 2022-04-15 18:33:04.000000 MoonMag-1.5.3/MoonMag/excitation/synodic_Be1xyz_Callisto.txt
+-rw-r--r--   0 mjstyczi   (503) staff       (20)      306 2022-04-15 18:33:04.000000 MoonMag-1.5.3/MoonMag/excitation/synodic_Be1xyz_Europa.txt
+-rw-r--r--   0 mjstyczi   (503) staff       (20)      222 2022-04-15 18:33:04.000000 MoonMag-1.5.3/MoonMag/excitation/synodic_Be1xyz_Miranda.txt
+-rw-r--r--   0 mjstyczi   (503) staff       (20)      227 2022-04-15 18:33:04.000000 MoonMag-1.5.3/MoonMag/excitation/synodic_Be1xyz_Triton.txt
+-rw-r--r--   0 mjstyczi   (503) staff       (20)   183760 2022-11-08 22:14:09.000000 MoonMag-1.5.3/MoonMag/field_xyz.py
+drwxr-xr-x   0 mjstyczi   (503) staff       (20)        0 2023-05-04 10:15:55.353351 MoonMag-1.5.3/MoonMag/induced/
+-rw-r--r--   0 mjstyczi   (503) staff       (20)  4460760 2022-05-10 17:37:41.000000 MoonMag-1.5.3/MoonMag/induced/Xid_values_n1_p10_np11.mat
+-rw-r--r--   0 mjstyczi   (503) staff       (20)    37080 2022-04-15 18:33:04.000000 MoonMag-1.5.3/MoonMag/induced/Xid_values_n1_p2_np3.mat
+-rw-r--r--   0 mjstyczi   (503) staff       (20)   230616 2022-04-15 18:33:04.000000 MoonMag-1.5.3/MoonMag/induced/Xid_values_n1_p4_np5.mat
+-rw-r--r--   0 mjstyczi   (503) staff       (20)  2073816 2022-04-15 18:33:04.000000 MoonMag-1.5.3/MoonMag/induced/Xid_values_n1_p8_np9.mat
+drwxr-xr-x   0 mjstyczi   (503) staff       (20)        0 2023-05-04 10:15:55.410733 MoonMag-1.5.3/MoonMag/interior/
+-rw-r--r--   0 mjstyczi   (503) staff       (20)      205 2023-05-04 10:12:30.000000 MoonMag-1.5.3/MoonMag/interior/chi_pq_Callisto.txt
+-rw-r--r--   0 mjstyczi   (503) staff       (20)      170 2023-05-04 09:53:20.000000 MoonMag-1.5.3/MoonMag/interior/chi_pq_Europa.txt
+-rw-r--r--   0 mjstyczi   (503) staff       (20)     3443 2023-05-04 09:56:44.000000 MoonMag-1.5.3/MoonMag/interior/chi_pq_Miranda.txt
+-rw-r--r--   0 mjstyczi   (503) staff       (20)      156 2023-05-04 09:53:49.000000 MoonMag-1.5.3/MoonMag/interior/chi_pq_Triton.txt
+-rw-r--r--   0 mjstyczi   (503) staff       (20)      702 2022-04-15 18:33:04.000000 MoonMag-1.5.3/MoonMag/interior/degree1_shapes.txt
+-rw-r--r--   0 mjstyczi   (503) staff       (20)      384 2022-04-15 18:33:04.000000 MoonMag-1.5.3/MoonMag/interior/degree1_shapes_Callisto.txt
+-rw-r--r--   0 mjstyczi   (503) staff       (20)       54 2022-04-15 18:33:04.000000 MoonMag-1.5.3/MoonMag/interior/degree1_shapes_Europa_Tobie.txt
+-rw-r--r--   0 mjstyczi   (503) staff       (20)       36 2022-04-15 18:33:04.000000 MoonMag-1.5.3/MoonMag/interior/degree1_shapes_Europa_prev.txt
+-rw-r--r--   0 mjstyczi   (503) staff       (20)      702 2022-04-15 18:33:04.000000 MoonMag-1.5.3/MoonMag/interior/degree1_shapes_Miranda.txt
+-rw-r--r--   0 mjstyczi   (503) staff       (20)      444 2022-04-15 18:33:04.000000 MoonMag-1.5.3/MoonMag/interior/degree1_shapes_Triton.txt
+-rw-r--r--   0 mjstyczi   (503) staff       (20)     1247 2022-04-15 18:33:04.000000 MoonMag-1.5.3/MoonMag/interior/degree2_shapes.txt
+-rw-r--r--   0 mjstyczi   (503) staff       (20)      101 2022-04-15 18:33:04.000000 MoonMag-1.5.3/MoonMag/interior/degree2_shapes_Callisto.txt
+-rw-r--r--   0 mjstyczi   (503) staff       (20)      521 2022-04-15 18:33:04.000000 MoonMag-1.5.3/MoonMag/interior/degree2_shapes_Europa_Tobie.txt
+-rw-r--r--   0 mjstyczi   (503) staff       (20)       81 2022-04-15 18:33:04.000000 MoonMag-1.5.3/MoonMag/interior/degree2_shapes_Europa_prev.txt
+-rw-r--r--   0 mjstyczi   (503) staff       (20)     1247 2022-04-15 18:33:04.000000 MoonMag-1.5.3/MoonMag/interior/degree2_shapes_Miranda.txt
+-rw-r--r--   0 mjstyczi   (503) staff       (20)      111 2022-04-15 18:33:04.000000 MoonMag-1.5.3/MoonMag/interior/degree2_shapes_Triton.txt
+-rw-r--r--   0 mjstyczi   (503) staff       (20)     1762 2022-04-15 18:33:04.000000 MoonMag-1.5.3/MoonMag/interior/degree3_shapes.txt
+-rw-r--r--   0 mjstyczi   (503) staff       (20)      142 2022-04-15 18:33:04.000000 MoonMag-1.5.3/MoonMag/interior/degree3_shapes_Callisto.txt
+-rw-r--r--   0 mjstyczi   (503) staff       (20)      128 2022-04-15 18:33:04.000000 MoonMag-1.5.3/MoonMag/interior/degree3_shapes_Europa_Tobie.txt
+-rw-r--r--   0 mjstyczi   (503) staff       (20)       86 2022-04-15 18:33:04.000000 MoonMag-1.5.3/MoonMag/interior/degree3_shapes_Europa_prev.txt
+-rw-r--r--   0 mjstyczi   (503) staff       (20)     1762 2022-04-15 18:33:04.000000 MoonMag-1.5.3/MoonMag/interior/degree3_shapes_Miranda.txt
+-rw-r--r--   0 mjstyczi   (503) staff       (20)      156 2022-04-15 18:33:04.000000 MoonMag-1.5.3/MoonMag/interior/degree3_shapes_Triton.txt
+-rw-r--r--   0 mjstyczi   (503) staff       (20)     2337 2022-04-15 18:33:04.000000 MoonMag-1.5.3/MoonMag/interior/degree4_shapes.txt
+-rw-r--r--   0 mjstyczi   (503) staff       (20)      183 2022-04-15 18:33:04.000000 MoonMag-1.5.3/MoonMag/interior/degree4_shapes_Callisto.txt
+-rw-r--r--   0 mjstyczi   (503) staff       (20)      770 2022-04-15 18:33:04.000000 MoonMag-1.5.3/MoonMag/interior/degree4_shapes_Europa_Tobie.txt
+-rw-r--r--   0 mjstyczi   (503) staff       (20)      111 2022-04-15 18:33:04.000000 MoonMag-1.5.3/MoonMag/interior/degree4_shapes_Europa_prev.txt
+-rw-r--r--   0 mjstyczi   (503) staff       (20)     2337 2022-04-15 18:33:04.000000 MoonMag-1.5.3/MoonMag/interior/degree4_shapes_Miranda.txt
+-rw-r--r--   0 mjstyczi   (503) staff       (20)      201 2022-04-15 18:33:04.000000 MoonMag-1.5.3/MoonMag/interior/degree4_shapes_Triton.txt
+-rw-r--r--   0 mjstyczi   (503) staff       (20)     2870 2022-04-15 18:33:04.000000 MoonMag-1.5.3/MoonMag/interior/degree5_shapes.txt
+-rw-r--r--   0 mjstyczi   (503) staff       (20)      224 2022-04-15 18:33:04.000000 MoonMag-1.5.3/MoonMag/interior/degree5_shapes_Callisto.txt
+-rw-r--r--   0 mjstyczi   (503) staff       (20)      202 2022-04-15 18:33:04.000000 MoonMag-1.5.3/MoonMag/interior/degree5_shapes_Europa_Tobie.txt
+-rw-r--r--   0 mjstyczi   (503) staff       (20)      136 2022-04-15 18:33:04.000000 MoonMag-1.5.3/MoonMag/interior/degree5_shapes_Europa_prev.txt
+-rw-r--r--   0 mjstyczi   (503) staff       (20)     2870 2022-04-15 18:33:04.000000 MoonMag-1.5.3/MoonMag/interior/degree5_shapes_Miranda.txt
+-rw-r--r--   0 mjstyczi   (503) staff       (20)      246 2022-04-15 18:33:04.000000 MoonMag-1.5.3/MoonMag/interior/degree5_shapes_Triton.txt
+-rw-r--r--   0 mjstyczi   (503) staff       (20)     3409 2022-04-15 18:33:04.000000 MoonMag-1.5.3/MoonMag/interior/degree6_shapes.txt
+-rw-r--r--   0 mjstyczi   (503) staff       (20)      265 2022-04-15 18:33:04.000000 MoonMag-1.5.3/MoonMag/interior/degree6_shapes_Callisto.txt
+-rw-r--r--   0 mjstyczi   (503) staff       (20)      239 2022-04-15 18:33:04.000000 MoonMag-1.5.3/MoonMag/interior/degree6_shapes_Europa_Tobie.txt
+-rw-r--r--   0 mjstyczi   (503) staff       (20)      161 2022-04-15 18:33:04.000000 MoonMag-1.5.3/MoonMag/interior/degree6_shapes_Europa_prev.txt
+-rw-r--r--   0 mjstyczi   (503) staff       (20)     3409 2022-04-15 18:33:04.000000 MoonMag-1.5.3/MoonMag/interior/degree6_shapes_Miranda.txt
+-rw-r--r--   0 mjstyczi   (503) staff       (20)      291 2022-04-15 18:33:04.000000 MoonMag-1.5.3/MoonMag/interior/degree6_shapes_Triton.txt
+-rw-r--r--   0 mjstyczi   (503) staff       (20)     4002 2022-04-15 18:33:04.000000 MoonMag-1.5.3/MoonMag/interior/degree7_shapes.txt
+-rw-r--r--   0 mjstyczi   (503) staff       (20)      306 2022-04-15 18:33:04.000000 MoonMag-1.5.3/MoonMag/interior/degree7_shapes_Callisto.txt
+-rw-r--r--   0 mjstyczi   (503) staff       (20)      276 2022-04-15 18:33:04.000000 MoonMag-1.5.3/MoonMag/interior/degree7_shapes_Europa_Tobie.txt
+-rw-r--r--   0 mjstyczi   (503) staff       (20)      186 2022-04-15 18:33:04.000000 MoonMag-1.5.3/MoonMag/interior/degree7_shapes_Europa_prev.txt
+-rw-r--r--   0 mjstyczi   (503) staff       (20)     4002 2022-04-15 18:33:04.000000 MoonMag-1.5.3/MoonMag/interior/degree7_shapes_Miranda.txt
+-rw-r--r--   0 mjstyczi   (503) staff       (20)      336 2022-04-15 18:33:04.000000 MoonMag-1.5.3/MoonMag/interior/degree7_shapes_Triton.txt
+-rw-r--r--   0 mjstyczi   (503) staff       (20)     4505 2022-04-15 18:33:04.000000 MoonMag-1.5.3/MoonMag/interior/degree8_shapes.txt
+-rw-r--r--   0 mjstyczi   (503) staff       (20)      347 2022-04-15 18:33:04.000000 MoonMag-1.5.3/MoonMag/interior/degree8_shapes_Callisto.txt
+-rw-r--r--   0 mjstyczi   (503) staff       (20)      313 2022-04-15 18:33:04.000000 MoonMag-1.5.3/MoonMag/interior/degree8_shapes_Europa_Tobie.txt
+-rw-r--r--   0 mjstyczi   (503) staff       (20)      211 2022-04-15 18:33:04.000000 MoonMag-1.5.3/MoonMag/interior/degree8_shapes_Europa_prev.txt
+-rw-r--r--   0 mjstyczi   (503) staff       (20)     4505 2022-04-15 18:33:04.000000 MoonMag-1.5.3/MoonMag/interior/degree8_shapes_Miranda.txt
+-rw-r--r--   0 mjstyczi   (503) staff       (20)      381 2022-04-15 18:33:04.000000 MoonMag-1.5.3/MoonMag/interior/degree8_shapes_Triton.txt
+-rw-r--r--   0 mjstyczi   (503) staff       (20)     5384 2022-04-15 18:33:04.000000 MoonMag-1.5.3/MoonMag/interior/depth_chi_pq_shape_Callisto.txt
+-rw-r--r--   0 mjstyczi   (503) staff       (20)     5452 2022-04-15 18:33:04.000000 MoonMag-1.5.3/MoonMag/interior/depth_chi_pq_shape_Enceladus.txt
+-rw-r--r--   0 mjstyczi   (503) staff       (20)     5392 2022-04-15 18:33:04.000000 MoonMag-1.5.3/MoonMag/interior/depth_chi_pq_shape_Europa.txt
+-rw-r--r--   0 mjstyczi   (503) staff       (20)     5391 2022-04-15 18:33:04.000000 MoonMag-1.5.3/MoonMag/interior/depth_chi_pq_shape_Europa_Tobie_high.txt
+-rw-r--r--   0 mjstyczi   (503) staff       (20)     5391 2022-04-15 18:33:04.000000 MoonMag-1.5.3/MoonMag/interior/depth_chi_pq_shape_Europa_Tobie_low.txt
+-rw-r--r--   0 mjstyczi   (503) staff       (20)     5392 2022-04-15 18:33:04.000000 MoonMag-1.5.3/MoonMag/interior/depth_chi_pq_shape_Europa_prev.txt
+-rw-r--r--   0 mjstyczi   (503) staff       (20)     5446 2022-04-15 18:33:04.000000 MoonMag-1.5.3/MoonMag/interior/depth_chi_pq_shape_Miranda.txt
+-rw-r--r--   0 mjstyczi   (503) staff       (20)     5386 2022-04-15 18:33:04.000000 MoonMag-1.5.3/MoonMag/interior/depth_chi_pq_shape_Triton.txt
+-rw-r--r--   0 mjstyczi   (503) staff       (20)     5396 2022-04-15 18:33:04.000000 MoonMag-1.5.3/MoonMag/interior/gravity_Europa_Tobie_high.txt
+-rw-r--r--   0 mjstyczi   (503) staff       (20)     5396 2022-04-15 18:33:04.000000 MoonMag-1.5.3/MoonMag/interior/gravity_Europa_Tobie_low.txt
+-rw-r--r--   0 mjstyczi   (503) staff       (20)     3766 2022-04-15 18:33:04.000000 MoonMag-1.5.3/MoonMag/interior/interior_model_asym.txt
+-rw-r--r--   0 mjstyczi   (503) staff       (20)      224 2023-04-12 07:02:25.000000 MoonMag-1.5.3/MoonMag/interior/interior_model_asym_Callisto.txt
+-rw-r--r--   0 mjstyczi   (503) staff       (20)      156 2022-11-07 13:30:01.000000 MoonMag-1.5.3/MoonMag/interior/interior_model_asym_Enceladus.txt
+-rw-r--r--   0 mjstyczi   (503) staff       (20)      226 2022-11-07 13:29:51.000000 MoonMag-1.5.3/MoonMag/interior/interior_model_asym_Europa_Tobie_high.txt
+-rw-r--r--   0 mjstyczi   (503) staff       (20)      226 2022-11-07 13:29:44.000000 MoonMag-1.5.3/MoonMag/interior/interior_model_asym_Europa_Tobie_low.txt
+-rw-r--r--   0 mjstyczi   (503) staff       (20)       93 2022-11-07 13:29:57.000000 MoonMag-1.5.3/MoonMag/interior/interior_model_asym_Europa_prev.txt
+-rw-r--r--   0 mjstyczi   (503) staff       (20)      240 2022-11-07 13:29:46.000000 MoonMag-1.5.3/MoonMag/interior/interior_model_asym_Miranda.txt
+-rw-r--r--   0 mjstyczi   (503) staff       (20)      244 2022-11-07 13:29:35.000000 MoonMag-1.5.3/MoonMag/interior/interior_model_asym_Triton.txt
+-rw-r--r--   0 mjstyczi   (503) staff       (20)     1160 2022-04-15 18:33:04.000000 MoonMag-1.5.3/MoonMag/plot_Aes.py
+-rw-r--r--   0 mjstyczi   (503) staff       (20)    54036 2023-05-04 04:07:07.000000 MoonMag-1.5.3/MoonMag/plotting_funcs.py
+-rw-r--r--   0 mjstyczi   (503) staff       (20)     1375 2022-11-07 13:25:00.000000 MoonMag-1.5.3/MoonMag/reduce_interior_model.py
+-rw-r--r--   0 mjstyczi   (503) staff       (20)     7704 2023-05-04 09:47:47.000000 MoonMag-1.5.3/MoonMag/run_all.py
+-rw-r--r--   0 mjstyczi   (503) staff       (20)    17358 2022-11-08 22:08:20.000000 MoonMag-1.5.3/MoonMag/symmetry_funcs.py
+-rw-r--r--   0 mjstyczi   (503) staff       (20)    20987 2022-11-07 13:18:43.000000 MoonMag-1.5.3/MoonMag/trajec_analysis.py
+drwxr-xr-x   0 mjstyczi   (503) staff       (20)        0 2023-05-04 10:15:55.332129 MoonMag-1.5.3/MoonMag.egg-info/
+-rw-r--r--   0 mjstyczi   (503) staff       (20)     6919 2023-05-04 10:15:55.000000 MoonMag-1.5.3/MoonMag.egg-info/PKG-INFO
+-rw-r--r--   0 mjstyczi   (503) staff       (20)     4454 2023-05-04 10:15:55.000000 MoonMag-1.5.3/MoonMag.egg-info/SOURCES.txt
+-rw-r--r--   0 mjstyczi   (503) staff       (20)        1 2023-05-04 10:15:55.000000 MoonMag-1.5.3/MoonMag.egg-info/dependency_links.txt
+-rw-r--r--   0 mjstyczi   (503) staff       (20)       76 2023-05-04 10:15:55.000000 MoonMag-1.5.3/MoonMag.egg-info/requires.txt
+-rw-r--r--   0 mjstyczi   (503) staff       (20)        8 2023-05-04 10:15:55.000000 MoonMag-1.5.3/MoonMag.egg-info/top_level.txt
+-rw-r--r--   0 mjstyczi   (503) staff       (20)     6919 2023-05-04 10:15:55.412002 MoonMag-1.5.3/PKG-INFO
+-rw-r--r--   0 mjstyczi   (503) staff       (20)     6288 2023-04-29 01:26:42.000000 MoonMag-1.5.3/README.md
+-rw-r--r--   0 mjstyczi   (503) staff       (20)       85 2022-05-10 03:25:16.000000 MoonMag-1.5.3/pyproject.toml
+-rw-r--r--   0 mjstyczi   (503) staff       (20)       38 2023-05-04 10:15:55.412712 MoonMag-1.5.3/setup.cfg
+-rw-r--r--   0 mjstyczi   (503) staff       (20)     1075 2023-05-04 10:14:36.000000 MoonMag-1.5.3/setup.py
```

### Comparing `MoonMag-1.5.2/LICENSE` & `MoonMag-1.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `MoonMag-1.5.2/PKG-INFO` & `MoonMag-1.5.3/MoonMag.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: MoonMag
-Version: 1.5.2
+Version: 1.5.3
 Summary: Magnetic induction calculations for sounding of icy moons
 Home-page: https://github.com/itsmoosh/MoonMag
 Author: Marshall J. Styczinski
 Author-email: marshall.j.styczinski@jpl.nasa.gov
-Project-URL: Bug Tracker, https://github.com/itsmoosh/MoonMag/issues
+Project-URL: Bug tracker, https://github.com/itsmoosh/MoonMag/issues
 Project-URL: Original publication, https://doi.org/10.1016/j.icarus.2021.114840
-Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # MoonMag
+<img src="misc/MoonMag_logo.png" width=240 title="MoonMag logo"/>
+
 ## Magnetic induction calculations and analysis for sounding of icy moons
 Written in Python 3.8 as supplemental material for "An analytic solution for evaluating the magnetic field induced from an arbitrary, asymmetric ocean world" DOI: [10.1016/j.icarus.2021.114840](https://doi.org/10.1016/j.icarus.2021.114840). For help, please contact M. Styczinski at [marshall.j.styczinski@jpl.nasa.gov](mailto:marshall.j.styczinski@jpl.nasa.gov).
 
 The main repository is mirrored at https://github.com/NASA-Planetary-Science/MoonMag; any pull requests should be submitted to https://github.com/itsmoosh/MoonMag.
 
 ## Acknowledging MoonMag
 Thank you for your interest in MoonMag! Please consider alerting us to your work (marshall.j.styczinski@jpl.nasa.gov). Suggested acknowledgement in publications: "Data used in this work were generated with the open source MoonMag framework hosted on GitHub."
```

### Comparing `MoonMag-1.5.2/README.md` & `MoonMag-1.5.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 # MoonMag
+<img src="misc/MoonMag_logo.png" width=240 title="MoonMag logo"/>
+
 ## Magnetic induction calculations and analysis for sounding of icy moons
 Written in Python 3.8 as supplemental material for "An analytic solution for evaluating the magnetic field induced from an arbitrary, asymmetric ocean world" DOI: [10.1016/j.icarus.2021.114840](https://doi.org/10.1016/j.icarus.2021.114840). For help, please contact M. Styczinski at [marshall.j.styczinski@jpl.nasa.gov](mailto:marshall.j.styczinski@jpl.nasa.gov).
 
 The main repository is mirrored at https://github.com/NASA-Planetary-Science/MoonMag; any pull requests should be submitted to https://github.com/itsmoosh/MoonMag.
 
 ## Acknowledging MoonMag
 Thank you for your interest in MoonMag! Please consider alerting us to your work (marshall.j.styczinski@jpl.nasa.gov). Suggested acknowledgement in publications: "Data used in this work were generated with the open source MoonMag framework hosted on GitHub."
```

### Comparing `MoonMag-1.5.2/src/MoonMag/asymmetry_funcs.py` & `MoonMag-1.5.3/MoonMag/asymmetry_funcs.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,4264 +29,4881 @@
 000001c0: 6f6d 2063 6f6c 6c65 6374 696f 6e73 2e61  om collections.a
 000001d0: 6263 2069 6d70 6f72 7420 4974 6572 6162  bc import Iterab
 000001e0: 6c65 0a66 726f 6d20 6e75 6d70 7920 696d  le.from numpy im
 000001f0: 706f 7274 2073 7172 740a 6672 6f6d 206d  port sqrt.from m
 00000200: 6174 6820 696d 706f 7274 2066 6c6f 6f72  ath import floor
 00000210: 0a66 726f 6d20 7363 6970 792e 7370 6563  .from scipy.spec
 00000220: 6961 6c20 696d 706f 7274 2066 6163 746f  ial import facto
-00000230: 7269 616c 2061 7320 6674 0a0a 696d 706f  rial as ft..impo
-00000240: 7274 206d 706d 6174 6820 6173 206d 700a  rt mpmath as mp.
-00000250: 2320 6d70 6d61 7468 2069 7320 6e65 6564  # mpmath is need
-00000260: 6564 2066 6f72 2065 6e68 616e 6365 6420  ed for enhanced 
-00000270: 7072 6563 6973 696f 6e20 746f 2061 766f  precision to avo
-00000280: 6964 0a23 2064 6976 6964 652d 6279 2d7a  id.# divide-by-z
-00000290: 6572 6f20 6572 726f 7273 2069 6e64 7563  ero errors induc
-000002a0: 6564 2062 7920 756e 6465 7266 6c6f 772e  ed by underflow.
-000002b0: 0a0a 6672 6f6d 204d 6f6f 6e4d 6167 2069  ..from MoonMag i
-000002c0: 6d70 6f72 7420 5f65 7863 6974 6174 696f  mport _excitatio
-000002d0: 6e2c 205f 696e 7465 7269 6f72 2c20 5f69  n, _interior, _i
-000002e0: 6e64 7563 6564 0a66 726f 6d20 4d6f 6f6e  nduced.from Moon
-000002f0: 4d61 672e 636f 6e66 6967 2069 6d70 6f72  Mag.config impor
-00000300: 7420 2a0a 6672 6f6d 204d 6f6f 6e4d 6167  t *.from MoonMag
-00000310: 2e66 6965 6c64 5f78 797a 2069 6d70 6f72  .field_xyz impor
-00000320: 7420 6576 616c 5f42 692c 2065 7661 6c5f  t eval_Bi, eval_
-00000330: 4269 5f53 6368 6d69 6474 0a0a 2320 5061  Bi_Schmidt..# Pa
-00000340: 7261 6c6c 656c 697a 6174 696f 6e20 6973  rallelization is
-00000350: 2074 6872 6f75 6768 206d 756c 7469 7072   through multipr
-00000360: 6f63 6573 7369 6e67 206d 6f64 756c 650a  ocessing module.
-00000370: 696d 706f 7274 206d 756c 7469 7072 6f63  import multiproc
-00000380: 6573 7369 6e67 2061 7320 6d74 700a 696d  essing as mtp.im
-00000390: 706f 7274 2070 6c61 7466 6f72 6d0a 706c  port platform.pl
-000003a0: 6174 203d 2070 6c61 7466 6f72 6d2e 7379  at = platform.sy
-000003b0: 7374 656d 2829 0a69 6620 706c 6174 203d  stem().if plat =
-000003c0: 3d20 2757 696e 646f 7773 273a 0a20 2020  = 'Windows':.   
-000003d0: 206d 7470 5479 7065 203d 2027 7370 6177   mtpType = 'spaw
-000003e0: 6e27 0a65 6c73 653a 0a20 2020 206d 7470  n'.else:.    mtp
-000003f0: 5479 7065 203d 2027 666f 726b 270a 6d74  Type = 'fork'.mt
-00000400: 7043 6f6e 7465 7874 203d 206d 7470 2e67  pContext = mtp.g
-00000410: 6574 5f63 6f6e 7465 7874 286d 7470 5479  et_context(mtpTy
-00000420: 7065 290a 6e75 6d5f 636f 7265 7320 3d20  pe).num_cores = 
-00000430: 6d74 702e 6370 755f 636f 756e 7428 290a  mtp.cpu_count().
-00000440: 0a23 2047 6c6f 6261 6c20 7661 7269 6162  .# Global variab
-00000450: 6c65 7320 616e 6420 7365 7474 696e 6773  les and settings
-00000460: 0a23 2053 6574 206d 6178 696d 756d 2070  .# Set maximum p
-00000470: 7265 6369 7369 6f6e 2066 6f72 206d 706d  recision for mpm
-00000480: 6174 6820 7175 616e 7469 7469 6573 0a6d  ath quantities.m
-00000490: 702e 6d70 2e64 7073 203d 2064 6967 6974  p.mp.dps = digit
-000004a0: 735f 7072 6563 6973 696f 6e0a 2320 4e75  s_precision.# Nu
-000004b0: 6d65 7269 6361 6c20 636f 6e73 7461 6e74  merical constant
-000004c0: 7320 696e 2068 6967 682d 7072 6563 6973  s in high-precis
-000004d0: 696f 6e20 6d70 6d61 7468 2066 6f72 6d61  ion mpmath forma
-000004e0: 740a 7a65 726f 203d 206d 702e 6d70 6628  t.zero = mp.mpf(
-000004f0: 3029 0a6f 6e65 203d 206d 702e 6d70 6628  0).one = mp.mpf(
-00000500: 3129 0a74 776f 203d 206d 702e 6d70 6628  1).two = mp.mpf(
-00000510: 3229 0a6a 203d 206d 702e 6d70 6328 316a  2).j = mp.mpc(1j
-00000520: 290a 6d75 5f6f 203d 206d 702e 6d70 6628  ).mu_o = mp.mpf(
-00000530: 2234 2e30 652d 3722 292a 6d70 2e70 690a  "4.0e-7")*mp.pi.
-00000540: 7371 7274 3220 3d20 7371 7274 2832 290a  sqrt2 = sqrt(2).
-00000550: 7371 7274 3470 6920 3d20 6e70 2e73 7172  sqrt4pi = np.sqr
-00000560: 7428 342a 6e70 2e70 6929 0a0a 2320 4765  t(4*np.pi)..# Ge
-00000570: 7420 7479 7065 206f 626a 6563 7473 2066  t type objects f
-00000580: 6f72 2069 6e69 7469 616c 697a 696e 6720  or initializing 
-00000590: 6e75 6d70 7920 6172 7261 7973 206f 6620  numpy arrays of 
-000005a0: 6d70 662f 6d70 630a 6d70 665f 676c 6f62  mpf/mpc.mpf_glob
-000005b0: 616c 203d 2074 7970 6528 7a65 726f 290a  al = type(zero).
-000005c0: 6d70 635f 676c 6f62 616c 203d 2074 7970  mpc_global = typ
-000005d0: 6528 6a29 0a0a 2323 2323 2323 2323 2323  e(j)..##########
-000005e0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00000230: 7269 616c 2061 7320 6674 2c20 6c70 6d76  rial as ft, lpmv
+00000240: 2061 7320 6c65 6765 6e70 2c20 7370 685f   as legenp, sph_
+00000250: 6861 726d 0a0a 696d 706f 7274 206d 706d  harm..import mpm
+00000260: 6174 6820 6173 206d 700a 2320 6d70 6d61  ath as mp.# mpma
+00000270: 7468 2069 7320 6e65 6564 6564 2066 6f72  th is needed for
+00000280: 2065 6e68 616e 6365 6420 7072 6563 6973   enhanced precis
+00000290: 696f 6e20 746f 2061 766f 6964 0a23 2064  ion to avoid.# d
+000002a0: 6976 6964 652d 6279 2d7a 6572 6f20 6572  ivide-by-zero er
+000002b0: 726f 7273 2069 6e64 7563 6564 2062 7920  rors induced by 
+000002c0: 756e 6465 7266 6c6f 772e 0a0a 6672 6f6d  underflow...from
+000002d0: 204d 6f6f 6e4d 6167 2069 6d70 6f72 7420   MoonMag import 
+000002e0: 5f65 7863 6974 6174 696f 6e2c 205f 696e  _excitation, _in
+000002f0: 7465 7269 6f72 2c20 5f69 6e64 7563 6564  terior, _induced
+00000300: 0a66 726f 6d20 4d6f 6f6e 4d61 672e 636f  .from MoonMag.co
+00000310: 6e66 6967 2069 6d70 6f72 7420 2a0a 6672  nfig import *.fr
+00000320: 6f6d 204d 6f6f 6e4d 6167 2e66 6965 6c64  om MoonMag.field
+00000330: 5f78 797a 2069 6d70 6f72 7420 6576 616c  _xyz import eval
+00000340: 5f42 692c 2065 7661 6c5f 4269 5f53 6368  _Bi, eval_Bi_Sch
+00000350: 6d69 6474 0a0a 2320 5061 7261 6c6c 656c  midt..# Parallel
+00000360: 697a 6174 696f 6e20 6973 2074 6872 6f75  ization is throu
+00000370: 6768 206d 756c 7469 7072 6f63 6573 7369  gh multiprocessi
+00000380: 6e67 206d 6f64 756c 650a 696d 706f 7274  ng module.import
+00000390: 206d 756c 7469 7072 6f63 6573 7369 6e67   multiprocessing
+000003a0: 2061 7320 6d74 700a 696d 706f 7274 2070   as mtp.import p
+000003b0: 6c61 7466 6f72 6d0a 706c 6174 203d 2070  latform.plat = p
+000003c0: 6c61 7466 6f72 6d2e 7379 7374 656d 2829  latform.system()
+000003d0: 0a69 6620 706c 6174 203d 3d20 2757 696e  .if plat == 'Win
+000003e0: 646f 7773 273a 0a20 2020 206d 7470 5479  dows':.    mtpTy
+000003f0: 7065 203d 2027 7370 6177 6e27 0a65 6c73  pe = 'spawn'.els
+00000400: 653a 0a20 2020 206d 7470 5479 7065 203d  e:.    mtpType =
+00000410: 2027 666f 726b 270a 6d74 7043 6f6e 7465   'fork'.mtpConte
+00000420: 7874 203d 206d 7470 2e67 6574 5f63 6f6e  xt = mtp.get_con
+00000430: 7465 7874 286d 7470 5479 7065 290a 6e75  text(mtpType).nu
+00000440: 6d5f 636f 7265 7320 3d20 6d74 702e 6370  m_cores = mtp.cp
+00000450: 755f 636f 756e 7428 290a 0a23 2047 6c6f  u_count()..# Glo
+00000460: 6261 6c20 7661 7269 6162 6c65 7320 616e  bal variables an
+00000470: 6420 7365 7474 696e 6773 0a23 2053 6574  d settings.# Set
+00000480: 206d 6178 696d 756d 2070 7265 6369 7369   maximum precisi
+00000490: 6f6e 2066 6f72 206d 706d 6174 6820 7175  on for mpmath qu
+000004a0: 616e 7469 7469 6573 0a6d 702e 6d70 2e64  antities.mp.mp.d
+000004b0: 7073 203d 2064 6967 6974 735f 7072 6563  ps = digits_prec
+000004c0: 6973 696f 6e0a 2320 4e75 6d65 7269 6361  ision.# Numerica
+000004d0: 6c20 636f 6e73 7461 6e74 7320 696e 2068  l constants in h
+000004e0: 6967 682d 7072 6563 6973 696f 6e20 6d70  igh-precision mp
+000004f0: 6d61 7468 2066 6f72 6d61 740a 7a65 726f  math format.zero
+00000500: 203d 206d 702e 6d70 6628 3029 0a6f 6e65   = mp.mpf(0).one
+00000510: 203d 206d 702e 6d70 6628 3129 0a74 776f   = mp.mpf(1).two
+00000520: 203d 206d 702e 6d70 6628 3229 0a6a 203d   = mp.mpf(2).j =
+00000530: 206d 702e 6d70 6328 316a 290a 6d75 5f6f   mp.mpc(1j).mu_o
+00000540: 203d 206d 702e 6d70 6628 2234 2e30 652d   = mp.mpf("4.0e-
+00000550: 3722 292a 6d70 2e70 690a 7371 7274 3220  7")*mp.pi.sqrt2 
+00000560: 3d20 7371 7274 2832 290a 7371 7274 3470  = sqrt(2).sqrt4p
+00000570: 6920 3d20 6e70 2e73 7172 7428 342a 6e70  i = np.sqrt(4*np
+00000580: 2e70 6929 0a0a 2320 4765 7420 7479 7065  .pi)..# Get type
+00000590: 206f 626a 6563 7473 2066 6f72 2069 6e69   objects for ini
+000005a0: 7469 616c 697a 696e 6720 6e75 6d70 7920  tializing numpy 
+000005b0: 6172 7261 7973 206f 6620 6d70 662f 6d70  arrays of mpf/mp
+000005c0: 630a 6d70 665f 676c 6f62 616c 203d 2074  c.mpf_global = t
+000005d0: 7970 6528 7a65 726f 290a 6d70 635f 676c  ype(zero).mpc_gl
+000005e0: 6f62 616c 203d 2074 7970 6528 6a29 0a0a  obal = type(j)..
 000005f0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00000600: 2323 230a 0a22 2222 0a72 6561 645f 7368  ###..""".read_sh
-00000610: 6170 6528 290a 2020 2020 4765 7420 626f  ape().    Get bo
-00000620: 756e 6461 7279 2073 6861 7065 2070 6172  undary shape par
-00000630: 616d 6574 6572 7320 6672 6f6d 2064 6973  ameters from dis
-00000640: 6b2e 0a20 2020 2055 7361 6765 3a20 6061  k..    Usage: `a
-00000650: 7379 6d5f 7368 6170 6560 203d 2072 6561  sym_shape` = rea
-00000660: 645f 7368 6170 6528 606e 5f62 6473 602c  d_shape(`n_bds`,
-00000670: 2060 705f 6d61 7860 2c20 6072 7363 616c   `p_max`, `rscal
-00000680: 6560 2c20 6062 6f64 796e 616d 653d 4e6f  e`, `bodyname=No
-00000690: 6e65 602c 2060 7265 6c61 7469 7665 3d46  ne`, `relative=F
-000006a0: 616c 7365 602c 2060 6570 735f 7363 616c  alse`, `eps_scal
-000006b0: 6564 3d4e 6f6e 6560 2c0a 2020 2020 2020  ed=None`,.      
-000006c0: 2020 6073 696e 676c 655f 6173 796d 3d4e    `single_asym=N
-000006d0: 6f6e 6560 2c20 6063 6f6e 6365 6e74 7269  one`, `concentri
-000006e0: 633d 5472 7565 602c 2060 6670 6174 683d  c=True`, `fpath=
-000006f0: 4e6f 6e65 602c 2060 725f 6264 733d 4e6f  None`, `r_bds=No
-00000700: 6e65 602c 2060 725f 696f 3d2d 3260 2c20  ne`, `r_io=-2`, 
-00000710: 6061 7070 656e 643d 2222 602c 2060 636f  `append=""`, `co
-00000720: 6e76 6572 745f 6465 7074 685f 746f 5f63  nvert_depth_to_c
-00000730: 6869 7071 3d46 616c 7365 6029 0a20 2020  hipq=False`).   
-00000740: 2052 6574 7572 6e73 3a0a 2020 2020 2020   Returns:.      
-00000750: 2020 6173 796d 5f73 6861 7065 3a20 636f    asym_shape: co
-00000760: 6d70 6c65 782c 2073 6861 7065 286e 5f62  mplex, shape(n_b
-00000770: 6473 2c32 2c70 5f6d 6178 2b31 2c70 5f6d  ds,2,p_max+1,p_m
-00000780: 6178 2b31 292e 2041 206c 6973 7420 6f66  ax+1). A list of
-00000790: 2061 6273 6f6c 7574 6520 626f 756e 6461   absolute bounda
-000007a0: 7279 2073 6861 7065 2070 6172 616d 6574  ry shape paramet
-000007b0: 6572 7320 6368 695f 7071 0a20 2020 2020  ers chi_pq.     
-000007c0: 2020 2020 2020 2066 6f72 2065 6163 6820         for each 
-000007d0: 626f 756e 6461 7279 2069 6e20 6d2c 2063  boundary in m, c
-000007e0: 6f6e 7665 7274 6564 2066 726f 6d20 7661  onverted from va
-000007f0: 6c75 6573 2069 6e20 6b6d 2072 6561 6420  lues in km read 
-00000800: 6672 6f6d 202e 7478 7420 6669 6c65 732e  from .txt files.
-00000810: 0a20 2020 2020 2020 2067 7261 765f 7368  .        grav_sh
-00000820: 6170 653a 2063 6f6d 706c 6578 2c20 7368  ape: complex, sh
-00000830: 6170 6528 6e5f 6264 732c 322c 705f 6d61  ape(n_bds,2,p_ma
-00000840: 782b 312c 705f 6d61 782b 3129 2e20 416e  x+1,p_max+1). An
-00000850: 616c 6f67 6f75 7320 746f 2061 7379 6d5f  alogous to asym_
-00000860: 7368 6170 652c 2062 7574 2064 7565 2074  shape, but due t
-00000870: 6f20 7469 6465 7320 6465 666f 726d 696e  o tides deformin
-00000880: 6720 7468 650a 2020 2020 2020 2020 2020  g the.          
-00000890: 2020 626f 6479 2073 7572 6661 6365 2e20    body surface. 
-000008a0: 4b65 7074 2073 6570 6172 6174 6520 6672  Kept separate fr
-000008b0: 6f6d 2061 7379 6d5f 7368 6170 6520 746f  om asym_shape to
-000008c0: 2070 7265 7365 7276 6520 6963 6520 7368   preserve ice sh
-000008d0: 656c 6c20 7468 6963 6b6e 6573 7320 636f  ell thickness co
-000008e0: 6e74 6f75 7273 2066 6f72 2063 6f6d 7061  ntours for compa
-000008f0: 7269 736f 6e20 746f 2070 7269 6f72 2077  rison to prior w
-00000900: 6f72 6b2e 0a20 2020 2050 6172 616d 6574  ork..    Paramet
-00000910: 6572 733a 0a20 2020 2020 2020 206e 5f62  ers:.        n_b
-00000920: 6473 3a20 696e 7465 6765 722e 204e 756d  ds: integer. Num
-00000930: 6265 7220 6f66 2063 6f6e 6475 6374 696e  ber of conductin
-00000940: 6720 626f 756e 6461 7269 6573 2069 6e20  g boundaries in 
-00000950: 7468 6520 6d6f 6465 6c20 2874 6869 7320  the model (this 
-00000960: 6973 204e 292e 0a20 2020 2020 2020 2070  is N)..        p
-00000970: 5f6d 6178 3a20 696e 7465 6765 722e 204c  _max: integer. L
-00000980: 6172 6765 7374 2064 6567 7265 6520 7020  argest degree p 
-00000990: 696e 2062 6f75 6e64 6172 7920 7368 6170  in boundary shap
-000009a0: 652e 0a20 2020 2020 2020 2072 7363 616c  e..        rscal
-000009b0: 653a 2066 6c6f 6174 2e20 312f 525f 626f  e: float. 1/R_bo
-000009c0: 6479 3b20 7573 6564 2074 6f20 7363 616c  dy; used to scal
-000009d0: 6520 6162 736f 6c75 7465 2061 7379 6d6d  e absolute asymm
-000009e0: 6574 7279 2076 616c 7565 7320 696e 206d  etry values in m
-000009f0: 616b 696e 6720 6173 796d 5f73 6861 7065  aking asym_shape
-00000a00: 2061 7272 6179 732e 0a20 2020 2020 2020   arrays..       
-00000a10: 2062 6f64 796e 616d 653a 2073 7472 696e   bodyname: strin
-00000a20: 6720 284e 6f6e 6529 2e20 426f 6479 206e  g (None). Body n
-00000a30: 616d 6520 6173 2069 7420 6170 7065 6172  ame as it appear
-00000a40: 7320 696e 2066 696c 6520 6e61 6d65 732e  s in file names.
-00000a50: 2049 6620 4e6f 6e65 2c20 6120 6765 6e65   If None, a gene
-00000a60: 7269 6320 6669 6c65 206e 616d 6520 7769  ric file name wi
-00000a70: 6c6c 2062 6520 7365 6172 6368 6564 2066  ll be searched f
-00000a80: 6f72 2e0a 2020 2020 2020 2020 7265 6c61  or..        rela
-00000a90: 7469 7665 3a20 626f 6f6c 6561 6e20 2854  tive: boolean (T
-00000aa0: 7275 6529 2e20 4f70 7469 6f6e 616c 2061  rue). Optional a
-00000ab0: 7267 756d 656e 7420 746f 2074 6f67 676c  rgument to toggl
-00000ac0: 6520 7768 6574 6865 7220 6368 695f 7071  e whether chi_pq
-00000ad0: 2076 616c 7565 7320 6172 6520 6e6f 726d   values are norm
-00000ae0: 616c 697a 6564 0a20 2020 2020 2020 2020  alized.         
-00000af0: 2020 2074 6f20 6263 6465 7620 2854 7275     to bcdev (Tru
-00000b00: 6529 206f 7220 6769 7665 2061 6273 6f6c  e) or give absol
-00000b10: 7574 6520 636f 6566 6669 6369 656e 7473  ute coefficients
-00000b20: 2066 6f72 2074 6865 2064 6576 6961 7469   for the deviati
-00000b30: 6f6e 7320 2846 616c 7365 292e 0a20 2020  ons (False)..   
-00000b40: 2020 2020 2065 7073 5f73 6361 6c65 643a       eps_scaled:
-00000b50: 2066 6c6f 6174 2c20 7368 6170 6528 6e5f   float, shape(n_
-00000b60: 6264 7329 2028 4e6f 6e65 292e 204d 6178  bds) (None). Max
-00000b70: 696d 756d 2062 6f75 6e64 6172 7920 6465  imum boundary de
-00000b80: 7669 6174 696f 6e20 696e 206b 6d2c 2066  viation in km, f
-00000b90: 6f72 2063 6f6e 7665 7274 696e 6720 7265  or converting re
-00000ba0: 6c61 7469 7665 2061 7379 6d5f 7368 6170  lative asym_shap
-00000bb0: 6520 7661 6c75 6573 2074 6f20 6162 736f  e values to abso
-00000bc0: 6c75 7465 2e0a 2020 2020 2020 2020 2020  lute..          
-00000bd0: 2020 5265 7175 6972 6564 2069 6620 7265    Required if re
-00000be0: 6c61 7469 7665 203d 2054 7275 652e 0a20  lative = True.. 
-00000bf0: 2020 2020 2020 2073 696e 676c 655f 6173         single_as
-00000c00: 796d 3a20 696e 7465 6765 7220 284e 6f6e  ym: integer (Non
-00000c10: 6529 2e20 4966 206e 6f74 204e 6f6e 652c  e). If not None,
-00000c20: 2061 7070 6c79 2061 7379 6d6d 6574 7279   apply asymmetry
-00000c30: 206f 6e6c 7920 746f 2074 6865 2062 6f75   only to the bou
-00000c40: 6e64 6172 7920 7769 7468 2074 6869 7320  ndary with this 
-00000c50: 696e 6465 782e 2020 0a20 2020 2020 2020  index.  .       
-00000c60: 2063 6f6e 6365 6e74 7269 633a 2062 6f6f   concentric: boo
-00000c70: 6c65 616e 2028 5472 7565 292e 204f 7074  lean (True). Opt
-00000c80: 696f 6e61 6c20 6172 6775 6d65 6e74 2074  ional argument t
-00000c90: 6f20 746f 6767 6c65 2077 6865 7468 6572  o toggle whether
-00000ca0: 2074 6f20 7573 6520 7468 6520 7361 6d65   to use the same
-00000cb0: 2073 7068 6572 6963 616c 2068 6172 6d6f   spherical harmo
-00000cc0: 6e69 630a 2020 2020 2020 2020 2020 2020  nic.            
-00000cd0: 636f 6566 6669 6369 656e 7473 2066 6f72  coefficients for
-00000ce0: 2065 7665 7279 2062 6f75 6e64 6172 7920   every boundary 
-00000cf0: 2863 6f6e 6365 6e74 7269 6320 6173 796d  (concentric asym
-00000d00: 6d65 7472 7929 2e20 496e 2074 6869 7320  metry). In this 
-00000d10: 6361 7365 2c20 6f6e 6c79 2061 2073 696e  case, only a sin
-00000d20: 676c 6520 6669 6c65 2069 7320 7265 6164  gle file is read
-00000d30: 2069 6e2e 0a20 2020 2020 2020 2020 2020   in..           
-00000d40: 2049 6620 636f 6e63 656e 7472 6963 203d   If concentric =
-00000d50: 2054 7275 652c 2072 5f62 6473 2069 7320   True, r_bds is 
-00000d60: 7265 7175 6972 6564 2e0a 2020 2020 2020  required..      
-00000d70: 2020 6670 6174 683a 2073 7472 696e 6720    fpath: string 
-00000d80: 284e 6f6e 6529 2e20 4f70 7469 6f6e 616c  (None). Optional
-00000d90: 206c 6f63 6174 696f 6e20 746f 2073 6561   location to sea
-00000da0: 7263 6820 666f 7220 2e74 7874 2066 696c  rch for .txt fil
-00000db0: 6573 2e20 4465 6661 756c 7473 2074 6f20  es. Defaults to 
-00000dc0: 2269 6e74 6572 696f 722f 222e 0a20 2020  "interior/"..   
-00000dd0: 2020 2020 2072 5f62 6473 3a20 666c 6f61       r_bds: floa
-00000de0: 742c 2073 6861 7065 286e 5f62 6473 2920  t, shape(n_bds) 
-00000df0: 284e 6f6e 6529 2e20 426f 756e 6461 7279  (None). Boundary
-00000e00: 2072 6164 6969 2069 6e20 6d2e 2052 6571   radii in m. Req
-00000e10: 7569 7265 6420 6966 2063 6f6e 6365 6e74  uired if concent
-00000e20: 7269 6320 3d20 5472 7565 2e0a 2020 2020  ric = True..    
-00000e30: 2020 2020 725f 696f 3a20 696e 7465 6765      r_io: intege
-00000e40: 7220 282d 3229 2e20 5468 6520 696e 6465  r (-2). The inde
-00000e50: 7820 6f66 2072 5f62 6473 2063 6f72 7265  x of r_bds corre
-00000e60: 7370 6f6e 6469 6e67 2074 6f20 7468 6520  sponding to the 
-00000e70: 6963 652d 6f63 6561 6e20 696e 7465 7266  ice-ocean interf
-00000e80: 6163 652c 2077 6865 7265 2061 7379 6d6d  ace, where asymm
-00000e90: 6574 7279 2069 7320 6578 7065 6374 6564  etry is expected
-00000ea0: 2074 6f0a 2020 2020 2020 2020 2020 2020   to.            
-00000eb0: 6265 2069 7473 206d 6f73 7420 7072 6f6e  be its most pron
-00000ec0: 6f75 6e63 6564 2e20 4465 6661 756c 7473  ounced. Defaults
-00000ed0: 2074 6f20 2d32 2c20 692e 652e 206e 6f20   to -2, i.e. no 
-00000ee0: 696f 6e6f 7370 6865 7265 2e20 5365 7420  ionosphere. Set 
-00000ef0: 746f 202d 3320 666f 7220 6120 7379 6d6d  to -3 for a symm
-00000f00: 6574 7269 6320 696f 6e6f 7370 6865 7265  etric ionosphere
-00000f10: 2e0a 2020 2020 2020 2020 6170 7065 6e64  ..        append
-00000f20: 3a20 7374 7269 6e67 2028 2222 292e 204f  : string (""). O
-00000f30: 7074 696f 6e61 6c20 7374 7269 6e67 2061  ptional string a
-00000f40: 7070 656e 6465 6420 746f 2066 696c 6520  ppended to file 
-00000f50: 6e61 6d65 732e 0a20 2020 2020 2020 2063  names..        c
-00000f60: 6f6e 7665 7274 5f64 6570 7468 5f74 6f5f  onvert_depth_to_
-00000f70: 6368 6970 713a 2062 6f6f 6c65 616e 2028  chipq: boolean (
-00000f80: 4661 6c73 6529 2e20 4f70 7469 6f6e 616c  False). Optional
-00000f90: 2066 6c61 6720 746f 2070 7269 6e74 2072   flag to print r
-00000fa0: 656c 6174 6976 6520 6368 695f 7071 2076  elative chi_pq v
-00000fb0: 616c 7565 7320 746f 2064 6973 6b2e 0a20  alues to disk.. 
-00000fc0: 2020 2022 2222 0a64 6566 2072 6561 645f     """.def read_
-00000fd0: 7368 6170 6528 6e5f 6264 732c 2070 5f6d  shape(n_bds, p_m
-00000fe0: 6178 2c20 7273 6361 6c65 2c20 626f 6479  ax, rscale, body
-00000ff0: 6e61 6d65 3d4e 6f6e 652c 2072 656c 6174  name=None, relat
-00001000: 6976 653d 4661 6c73 652c 2065 7073 5f73  ive=False, eps_s
-00001010: 6361 6c65 643d 4e6f 6e65 2c20 7369 6e67  caled=None, sing
-00001020: 6c65 5f61 7379 6d3d 4e6f 6e65 2c20 636f  le_asym=None, co
-00001030: 6e63 656e 7472 6963 3d54 7275 652c 0a20  ncentric=True,. 
-00001040: 2020 2020 2020 2020 2020 2020 2020 6670                fp
-00001050: 6174 683d 4e6f 6e65 2c20 725f 6264 733d  ath=None, r_bds=
-00001060: 4e6f 6e65 2c20 725f 696f 3d2d 322c 2061  None, r_io=-2, a
-00001070: 7070 656e 643d 2222 2c20 636f 6e76 6572  ppend="", conver
-00001080: 745f 6465 7074 685f 746f 5f63 6869 7071  t_depth_to_chipq
-00001090: 3d46 616c 7365 293a 0a20 2020 2069 6620  =False):.    if 
-000010a0: 6670 6174 6820 6973 204e 6f6e 653a 0a20  fpath is None:. 
-000010b0: 2020 2020 2020 2066 7061 7468 203d 205f         fpath = _
-000010c0: 696e 7465 7269 6f72 0a20 2020 2069 6620  interior.    if 
-000010d0: 626f 6479 6e61 6d65 2069 7320 4e6f 6e65  bodyname is None
-000010e0: 3a0a 2020 2020 2020 2020 6266 6e61 6d65  :.        bfname
-000010f0: 203d 2022 220a 2020 2020 656c 7365 3a0a   = "".    else:.
-00001100: 2020 2020 2020 2020 6266 6e61 6d65 203d          bfname =
-00001110: 2066 225f 7b62 6f64 796e 616d 657d 220a   f"_{bodyname}".
-00001120: 0a20 2020 2023 2049 6e69 7469 616c 697a  .    # Initializ
-00001130: 6520 6173 796d 6d65 7472 6963 2073 6861  e asymmetric sha
-00001140: 7065 2061 7272 6179 2e20 5468 6520 6c61  pe array. The la
-00001150: 7474 6572 2033 2069 6e64 6963 6573 2061  tter 3 indices a
-00001160: 7265 0a20 2020 2023 2066 6f72 2071 2070  re.    # for q p
-00001170: 6f73 6974 6976 6520 2830 2920 6f72 206e  ositive (0) or n
-00001180: 6567 6174 6976 6520 2831 292c 2070 2c20  egative (1), p, 
-00001190: 616e 6420 7c71 7c2e 0a20 2020 2061 7379  and |q|..    asy
-000011a0: 6d5f 7368 6170 652c 2067 7261 765f 7368  m_shape, grav_sh
-000011b0: 6170 6520 3d20 2820 6e70 2e7a 6572 6f73  ape = ( np.zeros
-000011c0: 2828 6e5f 6264 732c 322c 705f 6d61 782b  ((n_bds,2,p_max+
-000011d0: 312c 705f 6d61 782b 3129 2c64 7479 7065  1,p_max+1),dtype
-000011e0: 3d6e 702e 636f 6d70 6c65 785f 2920 666f  =np.complex_) fo
-000011f0: 7220 5f20 696e 2072 616e 6765 2832 2920  r _ in range(2) 
-00001200: 290a 0a20 2020 2069 6620 7369 6e67 6c65  )..    if single
-00001210: 5f61 7379 6d20 6973 206e 6f74 204e 6f6e  _asym is not Non
-00001220: 653a 0a20 2020 2020 2020 2061 7379 6d5f  e:.        asym_
-00001230: 6d6f 6465 6c20 3d20 6f73 2e70 6174 682e  model = os.path.
-00001240: 6a6f 696e 2866 7061 7468 2c20 6622 6465  join(fpath, f"de
-00001250: 7074 685f 6368 695f 7071 5f73 6861 7065  pth_chi_pq_shape
-00001260: 7b62 666e 616d 657d 7b61 7070 656e 647d  {bfname}{append}
-00001270: 2e74 7874 2229 0a20 2020 2020 2020 206c  .txt").        l
-00001280: 6f67 2e64 6562 7567 2866 2255 7369 6e67  og.debug(f"Using
-00001290: 2061 7379 6d6d 6574 7279 206d 6f64 656c   asymmetry model
-000012a0: 3a20 7b61 7379 6d5f 6d6f 6465 6c7d 2066  : {asym_model} f
-000012b0: 6f72 206c 6179 6572 2069 6e64 6578 207b  or layer index {
-000012c0: 7369 6e67 6c65 5f61 7379 6d7d 2229 0a20  single_asym}"). 
-000012d0: 2020 2020 2020 2073 6861 7065 5f6e 203d         shape_n =
-000012e0: 206e 702e 6c6f 6164 7478 7428 6173 796d   np.loadtxt(asym
-000012f0: 5f6d 6f64 656c 2c20 736b 6970 726f 7773  _model, skiprows
-00001300: 3d31 2c20 756e 7061 636b 3d46 616c 7365  =1, unpack=False
-00001310: 2c20 6465 6c69 6d69 7465 723d 272c 2729  , delimiter=',')
-00001320: 0a20 2020 2020 2020 2073 6361 6c65 645f  .        scaled_
-00001330: 7261 6420 3d20 725f 6264 7320 2a20 7273  rad = r_bds * rs
-00001340: 6361 6c65 0a20 2020 2020 2020 2066 6f72  cale.        for
-00001350: 2070 2069 6e20 7261 6e67 6528 312c 2070   p in range(1, p
-00001360: 5f6d 6178 202b 2031 293a 0a20 2020 2020  _max + 1):.     
-00001370: 2020 2020 2020 2074 6869 735f 6d69 6e20         this_min 
-00001380: 3d20 696e 7428 7020 2a20 2870 202b 2031  = int(p * (p + 1
-00001390: 2920 2f20 3229 0a20 2020 2020 2020 2020  ) / 2).         
-000013a0: 2020 2074 6869 735f 6d61 7820 3d20 7468     this_max = th
-000013b0: 6973 5f6d 696e 202b 2070 202b 2031 0a20  is_min + p + 1. 
-000013c0: 2020 2020 2020 2020 2020 2023 204e 6567             # Neg
-000013d0: 6174 6520 746f 2063 6f6e 7665 7274 2066  ate to convert f
-000013e0: 726f 6d20 6465 7669 6174 696f 6e73 206f  rom deviations o
-000013f0: 6620 6465 7074 6820 746f 2072 6164 6975  f depth to radiu
-00001400: 730a 2020 2020 2020 2020 2020 2020 4370  s.            Cp
-00001410: 7120 3d20 2d73 6861 7065 5f6e 5b74 6869  q = -shape_n[thi
-00001420: 735f 6d69 6e3a 7468 6973 5f6d 6178 2c20  s_min:this_max, 
-00001430: 325d 0a20 2020 2020 2020 2020 2020 2053  2].            S
-00001440: 7071 203d 202d 7368 6170 655f 6e5b 7468  pq = -shape_n[th
-00001450: 6973 5f6d 696e 3a74 6869 735f 6d61 782c  is_min:this_max,
-00001460: 2033 5d0a 0a20 2020 2020 2020 2020 2020   3]..           
-00001470: 2063 6869 5f70 7173 203d 2067 6574 5f63   chi_pqs = get_c
-00001480: 6869 7071 5f66 726f 6d5f 4353 7071 2870  hipq_from_CSpq(p
-00001490: 2c20 4370 712c 2053 7071 290a 2020 2020  , Cpq, Spq).    
-000014a0: 2020 2020 2020 2020 6173 796d 5f73 6861          asym_sha
-000014b0: 7065 5b73 696e 676c 655f 6173 796d 2c3a  pe[single_asym,:
-000014c0: 2c70 2c3a 702b 315d 203d 2063 6869 5f70  ,p,:p+1] = chi_p
-000014d0: 7173 202a 2031 6533 202a 2073 6361 6c65  qs * 1e3 * scale
-000014e0: 645f 7261 645b 7369 6e67 6c65 5f61 7379  d_rad[single_asy
-000014f0: 6d5d 0a0a 2020 2020 2020 2020 6966 2062  m]..        if b
-00001500: 6f64 796e 616d 6520 3d3d 2022 4d69 7261  odyname == "Mira
-00001510: 6e64 6122 3a0a 2020 2020 2020 2020 2020  nda":.          
-00001520: 2020 2320 5363 616c 6520 6963 6520 7368    # Scale ice sh
-00001530: 656c 6c20 7468 6963 6b6e 6573 7320 7661  ell thickness va
-00001540: 7269 6174 696f 6e73 2066 6f72 2045 6e63  riations for Enc
-00001550: 656c 6164 7573 2074 6f20 4d69 7261 6e64  eladus to Mirand
-00001560: 610a 2020 2020 2020 2020 2020 2020 6173  a.            as
-00001570: 796d 5f73 6861 7065 203d 2061 7379 6d5f  ym_shape = asym_
-00001580: 7368 6170 6520 2a20 3439 2e38 3130 2f32  shape * 49.810/2
-00001590: 302e 3835 320a 2020 2020 656c 6966 2072  0.852.    elif r
-000015a0: 656c 6174 6976 653a 0a20 2020 2020 2020  elative:.       
-000015b0: 2023 2050 7574 2073 6361 6c61 7220 7661   # Put scalar va
-000015c0: 6c75 6520 696e 746f 2061 206c 6973 7420  lue into a list 
-000015d0: 696e 2063 6173 6520 7468 6572 6527 7320  in case there's 
-000015e0: 6f6e 6c79 2061 2073 696e 676c 6520 626f  only a single bo
-000015f0: 756e 6461 7279 0a20 2020 2020 2020 2069  undary.        i
-00001600: 6620 6e6f 7420 6973 696e 7374 616e 6365  f not isinstance
-00001610: 2865 7073 5f73 6361 6c65 642c 2049 7465  (eps_scaled, Ite
-00001620: 7261 626c 6529 3a20 6570 735f 7363 616c  rable): eps_scal
-00001630: 6564 203d 205b 2065 7073 5f73 6361 6c65  ed = [ eps_scale
-00001640: 6420 5d0a 0a20 2020 2020 2020 2061 7379  d ]..        asy
-00001650: 6d5f 6d6f 6465 6c31 203d 206f 732e 7061  m_model1 = os.pa
-00001660: 7468 2e6a 6f69 6e28 6670 6174 682c 2022  th.join(fpath, "
-00001670: 6465 6772 6565 2229 0a0a 2020 2020 2020  degree")..      
-00001680: 2020 666f 7220 7020 696e 2072 616e 6765    for p in range
-00001690: 2831 2c70 5f6d 6178 2b31 293a 0a20 2020  (1,p_max+1):.   
-000016a0: 2020 2020 2020 2020 2074 7279 3a0a 2020           try:.  
-000016b0: 2020 2020 2020 2020 2020 2020 2020 6173                as
-000016c0: 796d 5f6d 6f64 656c 203d 2066 227b 6173  ym_model = f"{as
-000016d0: 796d 5f6d 6f64 656c 317d 7b70 7d5f 7368  ym_model1}{p}_sh
-000016e0: 6170 6573 7b62 666e 616d 657d 7b61 7070  apes{bfname}{app
-000016f0: 656e 647d 2e74 7874 220a 2020 2020 2020  end}.txt".      
-00001700: 2020 2020 2020 2020 2020 7368 6170 655f            shape_
-00001710: 7020 3d20 6e70 2e6c 6f61 6474 7874 2861  p = np.loadtxt(a
-00001720: 7379 6d5f 6d6f 6465 6c2c 2073 6b69 7072  sym_model, skipr
-00001730: 6f77 733d 312c 2075 6e70 6163 6b3d 4661  ows=1, unpack=Fa
-00001740: 6c73 652c 2064 656c 696d 6974 6572 3d27  lse, delimiter='
-00001750: 2c27 2c20 6474 7970 653d 6e70 2e63 6f6d  ,', dtype=np.com
-00001760: 706c 6578 5f29 0a20 2020 2020 2020 2020  plex_).         
-00001770: 2020 2020 2020 206c 6f67 2e64 6562 7567         log.debug
-00001780: 2866 2255 7369 6e67 2061 7379 6d6d 6574  (f"Using asymmet
-00001790: 7279 206d 6f64 656c 3a20 7b61 7379 6d5f  ry model: {asym_
-000017a0: 6d6f 6465 6c7d 2229 0a20 2020 2020 2020  model}").       
-000017b0: 2020 2020 2065 7863 6570 743a 0a20 2020       except:.   
-000017c0: 2020 2020 2020 2020 2020 2020 2061 7379               asy
-000017d0: 6d5f 6d6f 6465 6c20 3d20 6622 7b61 7379  m_model = f"{asy
-000017e0: 6d5f 6d6f 6465 6c31 7d7b 707d 5f73 6861  m_model1}{p}_sha
-000017f0: 7065 732e 7478 7422 0a20 2020 2020 2020  pes.txt".       
-00001800: 2020 2020 2020 2020 2073 6861 7065 5f70           shape_p
-00001810: 203d 206e 702e 6c6f 6164 7478 7428 6173   = np.loadtxt(as
-00001820: 796d 5f6d 6f64 656c 2c20 736b 6970 726f  ym_model, skipro
-00001830: 7773 3d31 2c20 756e 7061 636b 3d46 616c  ws=1, unpack=Fal
-00001840: 7365 2c20 6465 6c69 6d69 7465 723d 272c  se, delimiter=',
-00001850: 272c 2064 7479 7065 3d6e 702e 636f 6d70  ', dtype=np.comp
-00001860: 6c65 785f 290a 2020 2020 2020 2020 2020  lex_).          
-00001870: 2020 2020 2020 6c6f 672e 6465 6275 6728        log.debug(
-00001880: 6622 5573 696e 6720 6173 796d 6d65 7472  f"Using asymmetr
-00001890: 7920 6d6f 6465 6c3a 207b 6173 796d 5f6d  y model: {asym_m
-000018a0: 6f64 656c 7d22 290a 0a20 2020 2020 2020  odel}")..       
-000018b0: 2020 2020 2071 636f 756e 7420 3d20 300a       qcount = 0.
-000018c0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-000018d0: 7120 696e 2072 616e 6765 282d 702c 2070  q in range(-p, p
-000018e0: 2b31 293a 0a20 2020 2020 2020 2020 2020  +1):.           
-000018f0: 2020 2020 2071 7369 676e 203d 2069 6e74       qsign = int
-00001900: 2871 3c30 290a 2020 2020 2020 2020 2020  (q<0).          
-00001910: 2020 2020 2020 7161 6273 203d 2061 6273        qabs = abs
-00001920: 2871 290a 2020 2020 2020 2020 2020 2020  (q).            
-00001930: 2020 2020 666f 7220 6920 696e 2072 616e      for i in ran
-00001940: 6765 286e 5f62 6473 293a 0a20 2020 2020  ge(n_bds):.     
-00001950: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-00001960: 7379 6d5f 7368 6170 655b 692c 7173 6967  sym_shape[i,qsig
-00001970: 6e2c 702c 7161 6273 5d20 3d20 7368 6170  n,p,qabs] = shap
-00001980: 655f 705b 692c 7163 6f75 6e74 5d2a 6570  e_p[i,qcount]*ep
-00001990: 735f 7363 616c 6564 5b69 5d0a 2020 2020  s_scaled[i].    
-000019a0: 2020 2020 2020 2020 2020 2020 7163 6f75              qcou
-000019b0: 6e74 202b 3d20 310a 2020 2020 656c 6966  nt += 1.    elif
-000019c0: 2063 6f6e 6365 6e74 7269 633a 0a20 2020   concentric:.   
-000019d0: 2020 2020 2061 7379 6d5f 6d6f 6465 6c20       asym_model 
-000019e0: 3d20 6f73 2e70 6174 682e 6a6f 696e 2866  = os.path.join(f
-000019f0: 7061 7468 2c20 6622 6465 7074 685f 6368  path, f"depth_ch
-00001a00: 695f 7071 5f73 6861 7065 7b62 666e 616d  i_pq_shape{bfnam
-00001a10: 657d 7b61 7070 656e 647d 2e74 7874 2229  e}{append}.txt")
-00001a20: 0a20 2020 2020 2020 206c 6f67 2e64 6562  .        log.deb
-00001a30: 7567 2866 2255 7369 6e67 2061 7379 6d6d  ug(f"Using asymm
-00001a40: 6574 7279 206d 6f64 656c 3a20 7b61 7379  etry model: {asy
-00001a50: 6d5f 6d6f 6465 6c7d 2063 6f6e 6365 6e74  m_model} concent
-00001a60: 7269 6361 6c6c 792c 2073 6361 6c65 6420  rically, scaled 
-00001a70: 746f 2061 2072 6164 6975 7320 6f66 207b  to a radius of {
-00001a80: 312f 7273 6361 6c65 3a2e 3266 7d22 290a  1/rscale:.2f}").
-00001a90: 2020 2020 2020 2020 7368 6170 655f 6e20          shape_n 
-00001aa0: 3d20 6e70 2e6c 6f61 6474 7874 2861 7379  = np.loadtxt(asy
-00001ab0: 6d5f 6d6f 6465 6c2c 2073 6b69 7072 6f77  m_model, skiprow
-00001ac0: 733d 312c 2075 6e70 6163 6b3d 4661 6c73  s=1, unpack=Fals
-00001ad0: 652c 2064 656c 696d 6974 6572 3d27 2c27  e, delimiter=','
-00001ae0: 290a 2020 2020 2020 2020 7363 616c 6564  ).        scaled
-00001af0: 5f72 6164 203d 2072 5f62 6473 202a 2072  _rad = r_bds * r
-00001b00: 7363 616c 650a 2020 2020 2020 2020 666f  scale.        fo
-00001b10: 7220 7020 696e 2072 616e 6765 2831 2c70  r p in range(1,p
-00001b20: 5f6d 6178 2b31 293a 0a20 2020 2020 2020  _max+1):.       
-00001b30: 2020 2020 2074 6869 735f 6d69 6e20 3d20       this_min = 
-00001b40: 696e 7428 702a 2870 2b31 292f 3229 0a20  int(p*(p+1)/2). 
-00001b50: 2020 2020 2020 2020 2020 2074 6869 735f             this_
-00001b60: 6d61 7820 3d20 7468 6973 5f6d 696e 202b  max = this_min +
-00001b70: 2070 2b31 0a20 2020 2020 2020 2020 2020   p+1.           
-00001b80: 2023 204e 6567 6174 6520 746f 2063 6f6e   # Negate to con
-00001b90: 7665 7274 2066 726f 6d20 6465 7669 6174  vert from deviat
-00001ba0: 696f 6e73 206f 6620 6465 7074 6820 746f  ions of depth to
-00001bb0: 2072 6164 6975 730a 2020 2020 2020 2020   radius.        
-00001bc0: 2020 2020 4370 7120 3d20 2d73 6861 7065      Cpq = -shape
-00001bd0: 5f6e 5b74 6869 735f 6d69 6e3a 7468 6973  _n[this_min:this
-00001be0: 5f6d 6178 2c32 5d0a 2020 2020 2020 2020  _max,2].        
-00001bf0: 2020 2020 5370 7120 3d20 2d73 6861 7065      Spq = -shape
-00001c00: 5f6e 5b74 6869 735f 6d69 6e3a 7468 6973  _n[this_min:this
-00001c10: 5f6d 6178 2c33 5d0a 0a20 2020 2020 2020  _max,3]..       
-00001c20: 2020 2020 2063 6869 5f70 7173 203d 2067       chi_pqs = g
-00001c30: 6574 5f63 6869 7071 5f66 726f 6d5f 4353  et_chipq_from_CS
-00001c40: 7071 2870 2c43 7071 2c53 7071 290a 2020  pq(p,Cpq,Spq).  
-00001c50: 2020 2020 2020 2020 2020 666f 7220 695f            for i_
-00001c60: 6c61 7965 7220 696e 2072 616e 6765 286e  layer in range(n
-00001c70: 5f62 6473 293a 0a20 2020 2020 2020 2020  _bds):.         
-00001c80: 2020 2020 2020 2061 7379 6d5f 7368 6170         asym_shap
-00001c90: 655b 695f 6c61 7965 722c 3a2c 702c 3a70  e[i_layer,:,p,:p
-00001ca0: 2b31 5d20 3d20 6368 695f 7071 732a 3165  +1] = chi_pqs*1e
-00001cb0: 3320 2a20 7363 616c 6564 5f72 6164 5b69  3 * scaled_rad[i
-00001cc0: 5f6c 6179 6572 5d0a 0a20 2020 2065 6c73  _layer]..    els
-00001cd0: 653a 0a20 2020 2020 2020 2023 2049 6620  e:.        # If 
-00001ce0: 7765 2067 6f74 2068 6572 652c 206e 6f6e  we got here, non
-00001cf0: 6520 6f66 2074 6865 206f 7074 696f 6e73  e of the options
-00001d00: 2077 6572 6520 7365 6c65 6374 6564 2e0a   were selected..
-00001d10: 2020 2020 2020 2020 2320 4170 706c 7920          # Apply 
-00001d20: 6173 796d 6d65 7472 7920 696e 6465 7065  asymmetry indepe
-00001d30: 6e64 656e 746c 7920 746f 2065 6163 6820  ndently to each 
-00001d40: 6c61 7965 722c 2061 6e64 2072 6561 6420  layer, and read 
-00001d50: 696e 206f 6e65 2066 696c 6520 7065 7220  in one file per 
-00001d60: 6c61 7965 722e 0a20 2020 2020 2020 2072  layer..        r
-00001d70: 6169 7365 2052 756e 7469 6d65 4572 726f  aise RuntimeErro
-00001d80: 7228 2249 6e64 6570 656e 6465 6e74 6c79  r("Independently
-00001d90: 2061 7379 6d6d 6574 7269 6320 6c61 7965   asymmetric laye
-00001da0: 7273 2061 7265 206e 6f74 2069 6d70 6c65  rs are not imple
-00001db0: 6d65 6e74 6564 2e22 290a 2020 2020 2020  mented.").      
-00001dc0: 2020 666f 7220 6e5f 6c61 7965 7220 696e    for n_layer in
-00001dd0: 2072 616e 6765 2831 2c20 6e5f 6264 732b   range(1, n_bds+
-00001de0: 3129 3a0a 2020 2020 2020 2020 2020 2020  1):.            
-00001df0: 7368 6170 655f 6e20 3d20 6e70 2e6c 6f61  shape_n = np.loa
-00001e00: 6474 7874 286f 732e 7061 7468 2e6a 6f69  dtxt(os.path.joi
-00001e10: 6e28 6670 6174 682c 2066 2264 6570 7468  n(fpath, f"depth
-00001e20: 5f63 6869 5f70 715f 7368 6170 657b 6e5f  _chi_pq_shape{n_
-00001e30: 6c61 7965 727d 5f7b 6266 6e61 6d65 7d2e  layer}_{bfname}.
-00001e40: 7478 7422 292c 2073 6b69 7072 6f77 733d  txt"), skiprows=
-00001e50: 312c 2075 6e70 6163 6b3d 4661 6c73 652c  1, unpack=False,
-00001e60: 2064 656c 696d 6974 6572 3d27 2c27 290a   delimiter=',').
-00001e70: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-00001e80: 7020 696e 2072 616e 6765 2831 2c20 705f  p in range(1, p_
-00001e90: 6d61 782b 3129 3a0a 2020 2020 2020 2020  max+1):.        
-00001ea0: 2020 2020 2020 2020 2222 2220 4e6f 7420          """ Not 
-00001eb0: 7965 7420 696d 706c 656d 656e 7465 642c  yet implemented,
-00001ec0: 2062 7574 2074 6869 7320 6973 2061 2073   but this is a s
-00001ed0: 7461 7274 696e 6720 706f 696e 742e 0a20  tarting point.. 
-00001ee0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-00001ef0: 6869 735f 6d69 6e20 3d20 696e 7428 702a  his_min = int(p*
-00001f00: 2870 2b31 292f 3229 0a20 2020 2020 2020  (p+1)/2).       
-00001f10: 2020 2020 2020 2020 2074 6869 735f 6d61           this_ma
-00001f20: 7820 3d20 7468 6973 5f6d 696e 202b 2070  x = this_min + p
-00001f30: 2b31 0a20 2020 2020 2020 2020 2020 2020  +1.             
-00001f40: 2020 2043 7071 203d 202d 7368 6170 655f     Cpq = -shape_
-00001f50: 6e5b 7468 6973 5f6d 696e 3a74 6869 735f  n[this_min:this_
-00001f60: 6d61 782c 325d 0a20 2020 2020 2020 2020  max,2].         
-00001f70: 2020 2020 2020 2053 7071 203d 202d 7368         Spq = -sh
-00001f80: 6170 655f 6e5b 7468 6973 5f6d 696e 3a74  ape_n[this_min:t
-00001f90: 6869 735f 6d61 782c 335d 0a0a 2020 2020  his_max,3]..    
-00001fa0: 2020 2020 2020 2020 2020 2020 6368 695f              chi_
-00001fb0: 6d69 6e20 3d20 702a 2a32 202d 2031 0a20  min = p**2 - 1. 
-00001fc0: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00001fd0: 6869 5f6d 6178 203d 2028 702b 3129 2a2a  hi_max = (p+1)**
-00001fe0: 3220 2d20 310a 2020 2020 2020 2020 2020  2 - 1.          
-00001ff0: 2020 2020 2020 6173 796d 5f73 6861 7065        asym_shape
-00002000: 5b6e 5f6c 6179 6572 2c63 6869 5f6d 696e  [n_layer,chi_min
-00002010: 3a63 6869 5f6d 6178 5d20 3d20 6765 745f  :chi_max] = get_
-00002020: 6368 6970 715f 6672 6f6d 5f43 5370 7128  chipq_from_CSpq(
-00002030: 702c 4370 712c 5370 7129 2222 220a 0a20  p,Cpq,Spq)""".. 
-00002040: 2020 2069 6620 636f 6e76 6572 745f 6465     if convert_de
-00002050: 7074 685f 746f 5f63 6869 7071 2061 6e64  pth_to_chipq and
-00002060: 206e 6f74 2072 656c 6174 6976 653a 0a20   not relative:. 
-00002070: 2020 2020 2020 2069 6620 626f 6479 6e61         if bodyna
-00002080: 6d65 203d 3d20 2245 7572 6f70 6122 3a0a  me == "Europa":.
-00002090: 2020 2020 2020 2020 2020 2020 6966 2061              if a
-000020a0: 7070 656e 6420 3d3d 2022 5f54 6f62 6965  ppend == "_Tobie
-000020b0: 223a 0a20 2020 2020 2020 2020 2020 2020  ":.             
-000020c0: 2020 2065 7073 5f6d 6178 203d 2032 3530     eps_max = 250
-000020d0: 300a 2020 2020 2020 2020 2020 2020 656c  0.            el
-000020e0: 6966 2061 7070 656e 6420 3d3d 2022 5f70  if append == "_p
-000020f0: 7265 7622 3a0a 2020 2020 2020 2020 2020  rev":.          
-00002100: 2020 2020 2020 6570 735f 6d61 7820 3d20        eps_max = 
-00002110: 3235 3030 0a20 2020 2020 2020 2020 2020  2500.           
-00002120: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-00002130: 2020 2020 2020 2065 7073 5f6d 6178 203d         eps_max =
-00002140: 2033 3030 3030 0a20 2020 2020 2020 2065   30000.        e
-00002150: 6c69 6620 626f 6479 6e61 6d65 203d 3d20  lif bodyname == 
-00002160: 2243 616c 6c69 7374 6f22 3a0a 2020 2020  "Callisto":.    
-00002170: 2020 2020 2020 2020 6570 735f 6d61 7820          eps_max 
-00002180: 3d20 3130 3030 3030 0a20 2020 2020 2020  = 100000.       
-00002190: 2065 6c69 6620 626f 6479 6e61 6d65 203d   elif bodyname =
-000021a0: 3d20 2254 7269 746f 6e22 3a0a 2020 2020  = "Triton":.    
-000021b0: 2020 2020 2020 2020 6570 735f 6d61 7820          eps_max 
-000021c0: 3d20 3130 3030 3030 0a20 2020 2020 2020  = 100000.       
-000021d0: 2065 6c69 6620 626f 6479 6e61 6d65 203d   elif bodyname =
-000021e0: 3d20 224d 6972 616e 6461 223a 0a20 2020  = "Miranda":.   
-000021f0: 2020 2020 2020 2020 2065 7073 5f6d 6178           eps_max
-00002200: 203d 2034 3938 3130 2f32 3038 3532 202a   = 49810/20852 *
-00002210: 2031 3633 3737 2023 2053 6361 6c69 6e67   16377 # Scaling
-00002220: 2075 7020 6672 6f6d 206d 6178 696d 756d   up from maximum
-00002230: 2064 6576 6961 7469 6f6e 2069 6e20 4865   deviation in He
-00002240: 6d69 6e67 7761 7920 616e 6420 4d69 7474  mingway and Mitt
-00002250: 616c 2028 3230 3139 2920 456e 6365 6c61  al (2019) Encela
-00002260: 6475 7320 6d6f 6465 6c20 746f 2074 6869  dus model to thi
-00002270: 636b 6572 204d 6972 616e 6461 2069 6365  cker Miranda ice
-00002280: 2073 6865 6c6c 0a20 2020 2020 2020 2065   shell.        e
-00002290: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-000022a0: 2065 7073 5f6d 6178 203d 2031 3633 3737   eps_max = 16377
-000022b0: 0a20 2020 2020 2020 2023 2057 6865 7468  .        # Wheth
-000022c0: 6572 2074 6f20 7072 696e 7420 6c69 6e65  er to print line
-000022d0: 7320 7375 6974 6162 6c65 2066 6f72 2063  s suitable for c
-000022e0: 6f70 7969 6e67 2074 6f20 626f 756e 6461  opying to bounda
-000022f0: 7279 2073 6861 7065 2066 696c 6573 2c0a  ry shape files,.
-00002300: 2020 2020 2020 2020 2320 6f72 2074 6f20          # or to 
-00002310: 7072 696e 7420 666f 7220 7265 6164 6162  print for readab
-00002320: 696c 6974 7920 696e 7374 6561 640a 2020  ility instead.  
-00002330: 2020 2020 2020 7072 696e 745f 666f 725f        print_for_
-00002340: 636f 7079 203d 2054 7275 650a 2020 2020  copy = True.    
-00002350: 2020 2020 6966 2070 7269 6e74 5f66 6f72      if print_for
-00002360: 5f63 6f70 793a 0a20 2020 2020 2020 2020  _copy:.         
-00002370: 2020 2063 6869 5f68 6561 6420 3d20 6622     chi_head = f"
-00002380: 2070 2c20 6368 6970 7120 282d 712c 202e   p, chipq (-q, .
-00002390: 2e2e 2c20 7129 3b20 6263 6465 763d 7b65  .., q); bcdev={e
-000023a0: 7073 5f6d 6178 7d20 6d5c 6e22 0a20 2020  ps_max} m\n".   
-000023b0: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-000023c0: 2020 2020 2020 2063 6869 5f68 6561 6420         chi_head 
-000023d0: 3d20 6622 2070 2c20 712c 2063 6869 7071  = f" p, q, chipq
-000023e0: 5f72 652c 2063 6869 7071 5f69 6d2c 2062  _re, chipq_im, b
-000023f0: 6364 6576 3d7b 6570 735f 6d61 787d 206d  cdev={eps_max} m
-00002400: 5c6e 220a 2020 2020 2020 2020 6570 7320  \n".        eps 
-00002410: 3d20 6173 796d 5f73 6861 7065 5b72 5f69  = asym_shape[r_i
-00002420: 6f2c 202e 2e2e 5d20 2f20 6570 735f 6d61  o, ...] / eps_ma
-00002430: 780a 2020 2020 2020 2020 6173 796d 5f6f  x.        asym_o
-00002440: 7574 203d 206f 732e 7061 7468 2e6a 6f69  ut = os.path.joi
-00002450: 6e28 6670 6174 682c 2066 2263 6869 5f70  n(fpath, f"chi_p
-00002460: 715f 7b62 6f64 796e 616d 657d 2e74 7874  q_{bodyname}.txt
-00002470: 2229 0a20 2020 2020 2020 2077 6974 6820  ").        with 
-00002480: 6f70 656e 2861 7379 6d5f 6f75 742c 2022  open(asym_out, "
-00002490: 7722 2920 6173 2066 5f63 6869 3a0a 2020  w") as f_chi:.  
-000024a0: 2020 2020 2020 2020 2020 665f 6368 692e            f_chi.
-000024b0: 7772 6974 6528 6368 695f 6865 6164 290a  write(chi_head).
-000024c0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-000024d0: 7020 696e 2072 616e 6765 2831 2c20 705f  p in range(1, p_
-000024e0: 6d61 782b 3129 3a0a 2020 2020 2020 2020  max+1):.        
-000024f0: 2020 2020 2020 2020 6966 2070 7269 6e74          if print
-00002500: 5f66 6f72 5f63 6f70 793a 0a20 2020 2020  _for_copy:.     
-00002510: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-00002520: 6869 735f 6c69 6e65 203d 2022 2022 202b  his_line = " " +
-00002530: 2073 7472 2870 290a 2020 2020 2020 2020   str(p).        
-00002540: 2020 2020 2020 2020 666f 7220 7120 696e          for q in
-00002550: 2072 616e 6765 282d 702c 2070 2b31 293a   range(-p, p+1):
-00002560: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002570: 2020 2020 2071 7369 676e 203d 2069 6e74       qsign = int
-00002580: 2871 3c30 290a 2020 2020 2020 2020 2020  (q<0).          
-00002590: 2020 2020 2020 2020 2020 7161 6273 203d            qabs =
-000025a0: 2061 6273 2871 290a 2020 2020 2020 2020   abs(q).        
-000025b0: 2020 2020 2020 2020 2020 2020 6966 2070              if p
-000025c0: 7269 6e74 5f66 6f72 5f63 6f70 793a 0a20  rint_for_copy:. 
-000025d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000025e0: 2020 2020 2020 2069 6620 6e70 2e69 6d61         if np.ima
-000025f0: 6728 6570 735b 7173 6967 6e2c 2070 2c20  g(eps[qsign, p, 
-00002600: 7161 6273 5d29 203e 3d20 303a 0a20 2020  qabs]) >= 0:.   
-00002610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002620: 2020 2020 2020 2020 2062 7477 5f63 6861           btw_cha
-00002630: 7220 3d20 222b 220a 2020 2020 2020 2020  r = "+".        
+00000600: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00000610: 2323 2323 2323 2323 2323 2323 230a 0a22  #############.."
+00000620: 2222 0a72 6561 645f 7368 6170 6528 290a  "".read_shape().
+00000630: 2020 2020 4765 7420 626f 756e 6461 7279      Get boundary
+00000640: 2073 6861 7065 2070 6172 616d 6574 6572   shape parameter
+00000650: 7320 6672 6f6d 2064 6973 6b2e 0a20 2020  s from disk..   
+00000660: 2055 7361 6765 3a20 6061 7379 6d5f 7368   Usage: `asym_sh
+00000670: 6170 6560 203d 2072 6561 645f 7368 6170  ape` = read_shap
+00000680: 6528 606e 5f62 6473 602c 2060 705f 6d61  e(`n_bds`, `p_ma
+00000690: 7860 2c20 6072 7363 616c 6560 2c20 6062  x`, `rscale`, `b
+000006a0: 6f64 796e 616d 653d 4e6f 6e65 602c 2060  odyname=None`, `
+000006b0: 7265 6c61 7469 7665 3d46 616c 7365 602c  relative=False`,
+000006c0: 2060 6570 735f 7363 616c 6564 3d4e 6f6e   `eps_scaled=Non
+000006d0: 6560 2c0a 2020 2020 2020 2020 6073 696e  e`,.        `sin
+000006e0: 676c 655f 6173 796d 3d4e 6f6e 6560 2c20  gle_asym=None`, 
+000006f0: 6063 6f6e 6365 6e74 7269 633d 5472 7565  `concentric=True
+00000700: 602c 2060 6670 6174 683d 4e6f 6e65 602c  `, `fpath=None`,
+00000710: 2060 725f 6264 733d 4e6f 6e65 602c 2060   `r_bds=None`, `
+00000720: 725f 696f 3d2d 3260 2c20 6061 7070 656e  r_io=-2`, `appen
+00000730: 643d 2222 602c 2060 636f 6e76 6572 745f  d=""`, `convert_
+00000740: 6465 7074 685f 746f 5f63 6869 7071 3d46  depth_to_chipq=F
+00000750: 616c 7365 6029 0a20 2020 2052 6574 7572  alse`).    Retur
+00000760: 6e73 3a0a 2020 2020 2020 2020 6173 796d  ns:.        asym
+00000770: 5f73 6861 7065 3a20 636f 6d70 6c65 782c  _shape: complex,
+00000780: 2073 6861 7065 286e 5f62 6473 2c32 2c70   shape(n_bds,2,p
+00000790: 5f6d 6178 2b31 2c70 5f6d 6178 2b31 292e  _max+1,p_max+1).
+000007a0: 2041 206c 6973 7420 6f66 2061 6273 6f6c   A list of absol
+000007b0: 7574 6520 626f 756e 6461 7279 2073 6861  ute boundary sha
+000007c0: 7065 2070 6172 616d 6574 6572 7320 6368  pe parameters ch
+000007d0: 695f 7071 0a20 2020 2020 2020 2020 2020  i_pq.           
+000007e0: 2066 6f72 2065 6163 6820 626f 756e 6461   for each bounda
+000007f0: 7279 2069 6e20 6d2c 2063 6f6e 7665 7274  ry in m, convert
+00000800: 6564 2066 726f 6d20 7661 6c75 6573 2069  ed from values i
+00000810: 6e20 6b6d 2072 6561 6420 6672 6f6d 202e  n km read from .
+00000820: 7478 7420 6669 6c65 732e 0a20 2020 2020  txt files..     
+00000830: 2020 2067 7261 765f 7368 6170 653a 2063     grav_shape: c
+00000840: 6f6d 706c 6578 2c20 7368 6170 6528 6e5f  omplex, shape(n_
+00000850: 6264 732c 322c 705f 6d61 782b 312c 705f  bds,2,p_max+1,p_
+00000860: 6d61 782b 3129 2e20 416e 616c 6f67 6f75  max+1). Analogou
+00000870: 7320 746f 2061 7379 6d5f 7368 6170 652c  s to asym_shape,
+00000880: 2062 7574 2064 7565 2074 6f20 7469 6465   but due to tide
+00000890: 7320 6465 666f 726d 696e 6720 7468 650a  s deforming the.
+000008a0: 2020 2020 2020 2020 2020 2020 626f 6479              body
+000008b0: 2073 7572 6661 6365 2e20 4b65 7074 2073   surface. Kept s
+000008c0: 6570 6172 6174 6520 6672 6f6d 2061 7379  eparate from asy
+000008d0: 6d5f 7368 6170 6520 746f 2070 7265 7365  m_shape to prese
+000008e0: 7276 6520 6963 6520 7368 656c 6c20 7468  rve ice shell th
+000008f0: 6963 6b6e 6573 7320 636f 6e74 6f75 7273  ickness contours
+00000900: 2066 6f72 2063 6f6d 7061 7269 736f 6e20   for comparison 
+00000910: 746f 2070 7269 6f72 2077 6f72 6b2e 0a20  to prior work.. 
+00000920: 2020 2050 6172 616d 6574 6572 733a 0a20     Parameters:. 
+00000930: 2020 2020 2020 206e 5f62 6473 3a20 696e         n_bds: in
+00000940: 7465 6765 722e 204e 756d 6265 7220 6f66  teger. Number of
+00000950: 2063 6f6e 6475 6374 696e 6720 626f 756e   conducting boun
+00000960: 6461 7269 6573 2069 6e20 7468 6520 6d6f  daries in the mo
+00000970: 6465 6c20 2874 6869 7320 6973 204e 292e  del (this is N).
+00000980: 0a20 2020 2020 2020 2070 5f6d 6178 3a20  .        p_max: 
+00000990: 696e 7465 6765 722e 204c 6172 6765 7374  integer. Largest
+000009a0: 2064 6567 7265 6520 7020 696e 2062 6f75   degree p in bou
+000009b0: 6e64 6172 7920 7368 6170 652e 0a20 2020  ndary shape..   
+000009c0: 2020 2020 2072 7363 616c 653a 2066 6c6f       rscale: flo
+000009d0: 6174 2e20 312f 525f 626f 6479 3b20 7573  at. 1/R_body; us
+000009e0: 6564 2074 6f20 7363 616c 6520 6162 736f  ed to scale abso
+000009f0: 6c75 7465 2061 7379 6d6d 6574 7279 2076  lute asymmetry v
+00000a00: 616c 7565 7320 696e 206d 616b 696e 6720  alues in making 
+00000a10: 6173 796d 5f73 6861 7065 2061 7272 6179  asym_shape array
+00000a20: 732e 0a20 2020 2020 2020 2062 6f64 796e  s..        bodyn
+00000a30: 616d 653a 2073 7472 696e 6720 284e 6f6e  ame: string (Non
+00000a40: 6529 2e20 426f 6479 206e 616d 6520 6173  e). Body name as
+00000a50: 2069 7420 6170 7065 6172 7320 696e 2066   it appears in f
+00000a60: 696c 6520 6e61 6d65 732e 2049 6620 4e6f  ile names. If No
+00000a70: 6e65 2c20 6120 6765 6e65 7269 6320 6669  ne, a generic fi
+00000a80: 6c65 206e 616d 6520 7769 6c6c 2062 6520  le name will be 
+00000a90: 7365 6172 6368 6564 2066 6f72 2e0a 2020  searched for..  
+00000aa0: 2020 2020 2020 7265 6c61 7469 7665 3a20        relative: 
+00000ab0: 626f 6f6c 6561 6e20 2854 7275 6529 2e20  boolean (True). 
+00000ac0: 4f70 7469 6f6e 616c 2061 7267 756d 656e  Optional argumen
+00000ad0: 7420 746f 2074 6f67 676c 6520 7768 6574  t to toggle whet
+00000ae0: 6865 7220 6368 695f 7071 2076 616c 7565  her chi_pq value
+00000af0: 7320 6172 6520 6e6f 726d 616c 697a 6564  s are normalized
+00000b00: 0a20 2020 2020 2020 2020 2020 2074 6f20  .            to 
+00000b10: 6263 6465 7620 2854 7275 6529 206f 7220  bcdev (True) or 
+00000b20: 6769 7665 2061 6273 6f6c 7574 6520 636f  give absolute co
+00000b30: 6566 6669 6369 656e 7473 2066 6f72 2074  efficients for t
+00000b40: 6865 2064 6576 6961 7469 6f6e 7320 2846  he deviations (F
+00000b50: 616c 7365 292e 0a20 2020 2020 2020 2065  alse)..        e
+00000b60: 7073 5f73 6361 6c65 643a 2066 6c6f 6174  ps_scaled: float
+00000b70: 2c20 7368 6170 6528 6e5f 6264 7329 2028  , shape(n_bds) (
+00000b80: 4e6f 6e65 292e 204d 6178 696d 756d 2062  None). Maximum b
+00000b90: 6f75 6e64 6172 7920 6465 7669 6174 696f  oundary deviatio
+00000ba0: 6e20 696e 206b 6d2c 2066 6f72 2063 6f6e  n in km, for con
+00000bb0: 7665 7274 696e 6720 7265 6c61 7469 7665  verting relative
+00000bc0: 2061 7379 6d5f 7368 6170 6520 7661 6c75   asym_shape valu
+00000bd0: 6573 2074 6f20 6162 736f 6c75 7465 2e0a  es to absolute..
+00000be0: 2020 2020 2020 2020 2020 2020 5265 7175              Requ
+00000bf0: 6972 6564 2069 6620 7265 6c61 7469 7665  ired if relative
+00000c00: 203d 2054 7275 652e 0a20 2020 2020 2020   = True..       
+00000c10: 2073 696e 676c 655f 6173 796d 3a20 696e   single_asym: in
+00000c20: 7465 6765 7220 284e 6f6e 6529 2e20 4966  teger (None). If
+00000c30: 206e 6f74 204e 6f6e 652c 2061 7070 6c79   not None, apply
+00000c40: 2061 7379 6d6d 6574 7279 206f 6e6c 7920   asymmetry only 
+00000c50: 746f 2074 6865 2062 6f75 6e64 6172 7920  to the boundary 
+00000c60: 7769 7468 2074 6869 7320 696e 6465 782e  with this index.
+00000c70: 2020 0a20 2020 2020 2020 2063 6f6e 6365    .        conce
+00000c80: 6e74 7269 633a 2062 6f6f 6c65 616e 2028  ntric: boolean (
+00000c90: 5472 7565 292e 204f 7074 696f 6e61 6c20  True). Optional 
+00000ca0: 6172 6775 6d65 6e74 2074 6f20 746f 6767  argument to togg
+00000cb0: 6c65 2077 6865 7468 6572 2074 6f20 7573  le whether to us
+00000cc0: 6520 7468 6520 7361 6d65 2073 7068 6572  e the same spher
+00000cd0: 6963 616c 2068 6172 6d6f 6e69 630a 2020  ical harmonic.  
+00000ce0: 2020 2020 2020 2020 2020 636f 6566 6669            coeffi
+00000cf0: 6369 656e 7473 2066 6f72 2065 7665 7279  cients for every
+00000d00: 2062 6f75 6e64 6172 7920 2863 6f6e 6365   boundary (conce
+00000d10: 6e74 7269 6320 6173 796d 6d65 7472 7929  ntric asymmetry)
+00000d20: 2e20 496e 2074 6869 7320 6361 7365 2c20  . In this case, 
+00000d30: 6f6e 6c79 2061 2073 696e 676c 6520 6669  only a single fi
+00000d40: 6c65 2069 7320 7265 6164 2069 6e2e 0a20  le is read in.. 
+00000d50: 2020 2020 2020 2020 2020 2049 6620 636f             If co
+00000d60: 6e63 656e 7472 6963 203d 2054 7275 652c  ncentric = True,
+00000d70: 2072 5f62 6473 2069 7320 7265 7175 6972   r_bds is requir
+00000d80: 6564 2e0a 2020 2020 2020 2020 6670 6174  ed..        fpat
+00000d90: 683a 2073 7472 696e 6720 284e 6f6e 6529  h: string (None)
+00000da0: 2e20 4f70 7469 6f6e 616c 206c 6f63 6174  . Optional locat
+00000db0: 696f 6e20 746f 2073 6561 7263 6820 666f  ion to search fo
+00000dc0: 7220 2e74 7874 2066 696c 6573 2e20 4465  r .txt files. De
+00000dd0: 6661 756c 7473 2074 6f20 2269 6e74 6572  faults to "inter
+00000de0: 696f 722f 222e 0a20 2020 2020 2020 2072  ior/"..        r
+00000df0: 5f62 6473 3a20 666c 6f61 742c 2073 6861  _bds: float, sha
+00000e00: 7065 286e 5f62 6473 2920 284e 6f6e 6529  pe(n_bds) (None)
+00000e10: 2e20 426f 756e 6461 7279 2072 6164 6969  . Boundary radii
+00000e20: 2069 6e20 6d2e 2052 6571 7569 7265 6420   in m. Required 
+00000e30: 6966 2063 6f6e 6365 6e74 7269 6320 3d20  if concentric = 
+00000e40: 5472 7565 2e0a 2020 2020 2020 2020 725f  True..        r_
+00000e50: 696f 3a20 696e 7465 6765 7220 282d 3229  io: integer (-2)
+00000e60: 2e20 5468 6520 696e 6465 7820 6f66 2072  . The index of r
+00000e70: 5f62 6473 2063 6f72 7265 7370 6f6e 6469  _bds correspondi
+00000e80: 6e67 2074 6f20 7468 6520 6963 652d 6f63  ng to the ice-oc
+00000e90: 6561 6e20 696e 7465 7266 6163 652c 2077  ean interface, w
+00000ea0: 6865 7265 2061 7379 6d6d 6574 7279 2069  here asymmetry i
+00000eb0: 7320 6578 7065 6374 6564 2074 6f0a 2020  s expected to.  
+00000ec0: 2020 2020 2020 2020 2020 6265 2069 7473            be its
+00000ed0: 206d 6f73 7420 7072 6f6e 6f75 6e63 6564   most pronounced
+00000ee0: 2e20 4465 6661 756c 7473 2074 6f20 2d32  . Defaults to -2
+00000ef0: 2c20 692e 652e 206e 6f20 696f 6e6f 7370  , i.e. no ionosp
+00000f00: 6865 7265 2e20 5365 7420 746f 202d 3320  here. Set to -3 
+00000f10: 666f 7220 7468 6520 6963 652d 6f63 6561  for the ice-ocea
+00000f20: 6e20 626f 756e 6461 7279 2077 6865 6e20  n boundary when 
+00000f30: 6120 0a20 2020 2020 2020 2020 2020 2073  a .            s
+00000f40: 796d 6d65 7472 6963 2069 6f6e 6f73 7068  ymmetric ionosph
+00000f50: 6572 6520 286f 6e65 206c 6179 6572 2920  ere (one layer) 
+00000f60: 6973 2069 6e63 6c75 6465 642e 0a20 2020  is included..   
+00000f70: 2020 2020 2061 7070 656e 643a 2073 7472       append: str
+00000f80: 696e 6720 2822 2229 2e20 4f70 7469 6f6e  ing (""). Option
+00000f90: 616c 2073 7472 696e 6720 6170 7065 6e64  al string append
+00000fa0: 6564 2074 6f20 6669 6c65 206e 616d 6573  ed to file names
+00000fb0: 2e0a 2020 2020 2020 2020 636f 6e76 6572  ..        conver
+00000fc0: 745f 6465 7074 685f 746f 5f63 6869 7071  t_depth_to_chipq
+00000fd0: 3a20 626f 6f6c 6561 6e20 2846 616c 7365  : boolean (False
+00000fe0: 292e 204f 7074 696f 6e61 6c20 666c 6167  ). Optional flag
+00000ff0: 2074 6f20 7072 696e 7420 7265 6c61 7469   to print relati
+00001000: 7665 2063 6869 5f70 7120 7661 6c75 6573  ve chi_pq values
+00001010: 2074 6f20 6469 736b 2e0a 2020 2020 2222   to disk..    ""
+00001020: 220a 6465 6620 7265 6164 5f73 6861 7065  ".def read_shape
+00001030: 286e 5f62 6473 2c20 705f 6d61 782c 2072  (n_bds, p_max, r
+00001040: 7363 616c 652c 2062 6f64 796e 616d 653d  scale, bodyname=
+00001050: 4e6f 6e65 2c20 7265 6c61 7469 7665 3d46  None, relative=F
+00001060: 616c 7365 2c20 6570 735f 7363 616c 6564  alse, eps_scaled
+00001070: 3d4e 6f6e 652c 2073 696e 676c 655f 6173  =None, single_as
+00001080: 796d 3d4e 6f6e 652c 2063 6f6e 6365 6e74  ym=None, concent
+00001090: 7269 633d 5472 7565 2c0a 2020 2020 2020  ric=True,.      
+000010a0: 2020 2020 2020 2020 2066 7061 7468 3d4e           fpath=N
+000010b0: 6f6e 652c 2072 5f62 6473 3d4e 6f6e 652c  one, r_bds=None,
+000010c0: 2072 5f69 6f3d 2d32 2c20 6170 7065 6e64   r_io=-2, append
+000010d0: 3d22 222c 2063 6f6e 7665 7274 5f64 6570  ="", convert_dep
+000010e0: 7468 5f74 6f5f 6368 6970 713d 4661 6c73  th_to_chipq=Fals
+000010f0: 6529 3a0a 2020 2020 6966 2066 7061 7468  e):.    if fpath
+00001100: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
+00001110: 2020 6670 6174 6820 3d20 5f69 6e74 6572    fpath = _inter
+00001120: 696f 720a 2020 2020 6966 2062 6f64 796e  ior.    if bodyn
+00001130: 616d 6520 6973 204e 6f6e 653a 0a20 2020  ame is None:.   
+00001140: 2020 2020 2062 666e 616d 6520 3d20 2222       bfname = ""
+00001150: 0a20 2020 2065 6c73 653a 0a20 2020 2020  .    else:.     
+00001160: 2020 2062 666e 616d 6520 3d20 6622 5f7b     bfname = f"_{
+00001170: 626f 6479 6e61 6d65 7d22 0a0a 2020 2020  bodyname}"..    
+00001180: 2320 496e 6974 6961 6c69 7a65 2061 7379  # Initialize asy
+00001190: 6d6d 6574 7269 6320 7368 6170 6520 6172  mmetric shape ar
+000011a0: 7261 792e 2054 6865 206c 6174 7465 7220  ray. The latter 
+000011b0: 3320 696e 6469 6365 7320 6172 650a 2020  3 indices are.  
+000011c0: 2020 2320 666f 7220 7120 706f 7369 7469    # for q positi
+000011d0: 7665 2028 3029 206f 7220 6e65 6761 7469  ve (0) or negati
+000011e0: 7665 2028 3129 2c20 702c 2061 6e64 207c  ve (1), p, and |
+000011f0: 717c 2e0a 2020 2020 6173 796d 5f73 6861  q|..    asym_sha
+00001200: 7065 2c20 6772 6176 5f73 6861 7065 203d  pe, grav_shape =
+00001210: 2028 206e 702e 7a65 726f 7328 286e 5f62   ( np.zeros((n_b
+00001220: 6473 2c32 2c70 5f6d 6178 2b31 2c70 5f6d  ds,2,p_max+1,p_m
+00001230: 6178 2b31 292c 6474 7970 653d 6e70 2e63  ax+1),dtype=np.c
+00001240: 6f6d 706c 6578 5f29 2066 6f72 205f 2069  omplex_) for _ i
+00001250: 6e20 7261 6e67 6528 3229 2029 0a0a 2020  n range(2) )..  
+00001260: 2020 6966 2073 696e 676c 655f 6173 796d    if single_asym
+00001270: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+00001280: 2020 2020 2020 6173 796d 5f6d 6f64 656c        asym_model
+00001290: 203d 206f 732e 7061 7468 2e6a 6f69 6e28   = os.path.join(
+000012a0: 6670 6174 682c 2066 2264 6570 7468 5f63  fpath, f"depth_c
+000012b0: 6869 5f70 715f 7368 6170 657b 6266 6e61  hi_pq_shape{bfna
+000012c0: 6d65 7d7b 6170 7065 6e64 7d2e 7478 7422  me}{append}.txt"
+000012d0: 290a 2020 2020 2020 2020 6c6f 672e 6465  ).        log.de
+000012e0: 6275 6728 6622 5573 696e 6720 6173 796d  bug(f"Using asym
+000012f0: 6d65 7472 7920 6d6f 6465 6c3a 207b 6173  metry model: {as
+00001300: 796d 5f6d 6f64 656c 7d20 666f 7220 6c61  ym_model} for la
+00001310: 7965 7220 696e 6465 7820 7b73 696e 676c  yer index {singl
+00001320: 655f 6173 796d 7d22 290a 2020 2020 2020  e_asym}").      
+00001330: 2020 7368 6170 655f 6e20 3d20 6e70 2e6c    shape_n = np.l
+00001340: 6f61 6474 7874 2861 7379 6d5f 6d6f 6465  oadtxt(asym_mode
+00001350: 6c2c 2073 6b69 7072 6f77 733d 312c 2075  l, skiprows=1, u
+00001360: 6e70 6163 6b3d 4661 6c73 652c 2064 656c  npack=False, del
+00001370: 696d 6974 6572 3d27 2c27 290a 2020 2020  imiter=',').    
+00001380: 2020 2020 7363 616c 6564 5f72 6164 203d      scaled_rad =
+00001390: 2072 5f62 6473 202a 2072 7363 616c 650a   r_bds * rscale.
+000013a0: 2020 2020 2020 2020 666f 7220 7020 696e          for p in
+000013b0: 2072 616e 6765 2831 2c20 705f 6d61 7820   range(1, p_max 
+000013c0: 2b20 3129 3a0a 2020 2020 2020 2020 2020  + 1):.          
+000013d0: 2020 7468 6973 5f6d 696e 203d 2069 6e74    this_min = int
+000013e0: 2870 202a 2028 7020 2b20 3129 202f 2032  (p * (p + 1) / 2
+000013f0: 290a 2020 2020 2020 2020 2020 2020 7468  ).            th
+00001400: 6973 5f6d 6178 203d 2074 6869 735f 6d69  is_max = this_mi
+00001410: 6e20 2b20 7020 2b20 310a 2020 2020 2020  n + p + 1.      
+00001420: 2020 2020 2020 2320 4e65 6761 7465 2074        # Negate t
+00001430: 6f20 636f 6e76 6572 7420 6672 6f6d 2064  o convert from d
+00001440: 6576 6961 7469 6f6e 7320 6f66 2064 6570  eviations of dep
+00001450: 7468 2074 6f20 7261 6469 7573 0a20 2020  th to radius.   
+00001460: 2020 2020 2020 2020 2043 7071 203d 202d           Cpq = -
+00001470: 7368 6170 655f 6e5b 7468 6973 5f6d 696e  shape_n[this_min
+00001480: 3a74 6869 735f 6d61 782c 2032 5d0a 2020  :this_max, 2].  
+00001490: 2020 2020 2020 2020 2020 5370 7120 3d20            Spq = 
+000014a0: 2d73 6861 7065 5f6e 5b74 6869 735f 6d69  -shape_n[this_mi
+000014b0: 6e3a 7468 6973 5f6d 6178 2c20 335d 0a0a  n:this_max, 3]..
+000014c0: 2020 2020 2020 2020 2020 2020 6368 695f              chi_
+000014d0: 7071 7320 3d20 6765 745f 6368 6970 715f  pqs = get_chipq_
+000014e0: 6672 6f6d 5f43 5370 715f 7369 6e67 6c65  from_CSpq_single
+000014f0: 2870 2c20 4370 712c 2053 7071 290a 2020  (p, Cpq, Spq).  
+00001500: 2020 2020 2020 2020 2020 6173 796d 5f73            asym_s
+00001510: 6861 7065 5b73 696e 676c 655f 6173 796d  hape[single_asym
+00001520: 2c3a 2c70 2c3a 702b 315d 203d 2063 6869  ,:,p,:p+1] = chi
+00001530: 5f70 7173 202a 2031 6533 202a 2073 6361  _pqs * 1e3 * sca
+00001540: 6c65 645f 7261 645b 7369 6e67 6c65 5f61  led_rad[single_a
+00001550: 7379 6d5d 0a0a 2020 2020 2020 2020 6966  sym]..        if
+00001560: 2062 6f64 796e 616d 6520 3d3d 2022 4d69   bodyname == "Mi
+00001570: 7261 6e64 6122 3a0a 2020 2020 2020 2020  randa":.        
+00001580: 2020 2020 2320 5363 616c 6520 6963 6520      # Scale ice 
+00001590: 7368 656c 6c20 7468 6963 6b6e 6573 7320  shell thickness 
+000015a0: 7661 7269 6174 696f 6e73 2066 6f72 2045  variations for E
+000015b0: 6e63 656c 6164 7573 2074 6f20 4d69 7261  nceladus to Mira
+000015c0: 6e64 610a 2020 2020 2020 2020 2020 2020  nda.            
+000015d0: 6173 796d 5f73 6861 7065 203d 2061 7379  asym_shape = asy
+000015e0: 6d5f 7368 6170 6520 2a20 3439 2e38 3130  m_shape * 49.810
+000015f0: 2f32 302e 3835 320a 2020 2020 656c 6966  /20.852.    elif
+00001600: 2072 656c 6174 6976 653a 0a20 2020 2020   relative:.     
+00001610: 2020 2023 2050 7574 2073 6361 6c61 7220     # Put scalar 
+00001620: 7661 6c75 6520 696e 746f 2061 206c 6973  value into a lis
+00001630: 7420 696e 2063 6173 6520 7468 6572 6527  t in case there'
+00001640: 7320 6f6e 6c79 2061 2073 696e 676c 6520  s only a single 
+00001650: 626f 756e 6461 7279 0a20 2020 2020 2020  boundary.       
+00001660: 2069 6620 6e6f 7420 6973 696e 7374 616e   if not isinstan
+00001670: 6365 2865 7073 5f73 6361 6c65 642c 2049  ce(eps_scaled, I
+00001680: 7465 7261 626c 6529 3a20 6570 735f 7363  terable): eps_sc
+00001690: 616c 6564 203d 205b 2065 7073 5f73 6361  aled = [ eps_sca
+000016a0: 6c65 6420 5d0a 0a20 2020 2020 2020 2061  led ]..        a
+000016b0: 7379 6d5f 6d6f 6465 6c31 203d 206f 732e  sym_model1 = os.
+000016c0: 7061 7468 2e6a 6f69 6e28 6670 6174 682c  path.join(fpath,
+000016d0: 2022 6465 6772 6565 2229 0a0a 2020 2020   "degree")..    
+000016e0: 2020 2020 666f 7220 7020 696e 2072 616e      for p in ran
+000016f0: 6765 2831 2c70 5f6d 6178 2b31 293a 0a20  ge(1,p_max+1):. 
+00001700: 2020 2020 2020 2020 2020 2074 7279 3a0a             try:.
+00001710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001720: 6173 796d 5f6d 6f64 656c 203d 2066 227b  asym_model = f"{
+00001730: 6173 796d 5f6d 6f64 656c 317d 7b70 7d5f  asym_model1}{p}_
+00001740: 7368 6170 6573 7b62 666e 616d 657d 7b61  shapes{bfname}{a
+00001750: 7070 656e 647d 2e74 7874 220a 2020 2020  ppend}.txt".    
+00001760: 2020 2020 2020 2020 2020 2020 7368 6170              shap
+00001770: 655f 7020 3d20 6e70 2e6c 6f61 6474 7874  e_p = np.loadtxt
+00001780: 2861 7379 6d5f 6d6f 6465 6c2c 2073 6b69  (asym_model, ski
+00001790: 7072 6f77 733d 312c 2075 6e70 6163 6b3d  prows=1, unpack=
+000017a0: 4661 6c73 652c 2064 656c 696d 6974 6572  False, delimiter
+000017b0: 3d27 2c27 2c20 6474 7970 653d 6e70 2e63  =',', dtype=np.c
+000017c0: 6f6d 706c 6578 5f29 0a20 2020 2020 2020  omplex_).       
+000017d0: 2020 2020 2020 2020 206c 6f67 2e64 6562           log.deb
+000017e0: 7567 2866 2255 7369 6e67 2061 7379 6d6d  ug(f"Using asymm
+000017f0: 6574 7279 206d 6f64 656c 3a20 7b61 7379  etry model: {asy
+00001800: 6d5f 6d6f 6465 6c7d 2229 0a20 2020 2020  m_model}").     
+00001810: 2020 2020 2020 2065 7863 6570 743a 0a20         except:. 
+00001820: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+00001830: 7379 6d5f 6d6f 6465 6c20 3d20 6622 7b61  sym_model = f"{a
+00001840: 7379 6d5f 6d6f 6465 6c31 7d7b 707d 5f73  sym_model1}{p}_s
+00001850: 6861 7065 732e 7478 7422 0a20 2020 2020  hapes.txt".     
+00001860: 2020 2020 2020 2020 2020 2073 6861 7065             shape
+00001870: 5f70 203d 206e 702e 6c6f 6164 7478 7428  _p = np.loadtxt(
+00001880: 6173 796d 5f6d 6f64 656c 2c20 736b 6970  asym_model, skip
+00001890: 726f 7773 3d31 2c20 756e 7061 636b 3d46  rows=1, unpack=F
+000018a0: 616c 7365 2c20 6465 6c69 6d69 7465 723d  alse, delimiter=
+000018b0: 272c 272c 2064 7479 7065 3d6e 702e 636f  ',', dtype=np.co
+000018c0: 6d70 6c65 785f 290a 2020 2020 2020 2020  mplex_).        
+000018d0: 2020 2020 2020 2020 6c6f 672e 6465 6275          log.debu
+000018e0: 6728 6622 5573 696e 6720 6173 796d 6d65  g(f"Using asymme
+000018f0: 7472 7920 6d6f 6465 6c3a 207b 6173 796d  try model: {asym
+00001900: 5f6d 6f64 656c 7d22 290a 0a20 2020 2020  _model}")..     
+00001910: 2020 2020 2020 2071 636f 756e 7420 3d20         qcount = 
+00001920: 300a 2020 2020 2020 2020 2020 2020 666f  0.            fo
+00001930: 7220 7120 696e 2072 616e 6765 282d 702c  r q in range(-p,
+00001940: 2070 2b31 293a 0a20 2020 2020 2020 2020   p+1):.         
+00001950: 2020 2020 2020 2071 7369 676e 203d 2069         qsign = i
+00001960: 6e74 2871 3c30 290a 2020 2020 2020 2020  nt(q<0).        
+00001970: 2020 2020 2020 2020 7161 6273 203d 2061          qabs = a
+00001980: 6273 2871 290a 2020 2020 2020 2020 2020  bs(q).          
+00001990: 2020 2020 2020 666f 7220 6920 696e 2072        for i in r
+000019a0: 616e 6765 286e 5f62 6473 293a 0a20 2020  ange(n_bds):.   
+000019b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000019c0: 2061 7379 6d5f 7368 6170 655b 692c 7173   asym_shape[i,qs
+000019d0: 6967 6e2c 702c 7161 6273 5d20 3d20 7368  ign,p,qabs] = sh
+000019e0: 6170 655f 705b 692c 7163 6f75 6e74 5d2a  ape_p[i,qcount]*
+000019f0: 6570 735f 7363 616c 6564 5b69 5d0a 2020  eps_scaled[i].  
+00001a00: 2020 2020 2020 2020 2020 2020 2020 7163                qc
+00001a10: 6f75 6e74 202b 3d20 310a 2020 2020 656c  ount += 1.    el
+00001a20: 6966 2063 6f6e 6365 6e74 7269 633a 0a20  if concentric:. 
+00001a30: 2020 2020 2020 2061 7379 6d5f 6d6f 6465         asym_mode
+00001a40: 6c20 3d20 6f73 2e70 6174 682e 6a6f 696e  l = os.path.join
+00001a50: 2866 7061 7468 2c20 6622 6465 7074 685f  (fpath, f"depth_
+00001a60: 6368 695f 7071 5f73 6861 7065 7b62 666e  chi_pq_shape{bfn
+00001a70: 616d 657d 7b61 7070 656e 647d 2e74 7874  ame}{append}.txt
+00001a80: 2229 0a20 2020 2020 2020 206c 6f67 2e64  ").        log.d
+00001a90: 6562 7567 2866 2255 7369 6e67 2061 7379  ebug(f"Using asy
+00001aa0: 6d6d 6574 7279 206d 6f64 656c 3a20 7b61  mmetry model: {a
+00001ab0: 7379 6d5f 6d6f 6465 6c7d 2063 6f6e 6365  sym_model} conce
+00001ac0: 6e74 7269 6361 6c6c 792c 2073 6361 6c65  ntrically, scale
+00001ad0: 6420 746f 2061 2072 6164 6975 7320 6f66  d to a radius of
+00001ae0: 207b 312f 7273 6361 6c65 3a2e 3266 7d22   {1/rscale:.2f}"
+00001af0: 290a 2020 2020 2020 2020 7368 6170 655f  ).        shape_
+00001b00: 6e20 3d20 6e70 2e6c 6f61 6474 7874 2861  n = np.loadtxt(a
+00001b10: 7379 6d5f 6d6f 6465 6c2c 2073 6b69 7072  sym_model, skipr
+00001b20: 6f77 733d 312c 2075 6e70 6163 6b3d 4661  ows=1, unpack=Fa
+00001b30: 6c73 652c 2064 656c 696d 6974 6572 3d27  lse, delimiter='
+00001b40: 2c27 290a 2020 2020 2020 2020 7363 616c  ,').        scal
+00001b50: 6564 5f72 6164 203d 2072 5f62 6473 202a  ed_rad = r_bds *
+00001b60: 2072 7363 616c 650a 2020 2020 2020 2020   rscale.        
+00001b70: 666f 7220 7020 696e 2072 616e 6765 2831  for p in range(1
+00001b80: 2c70 5f6d 6178 2b31 293a 0a20 2020 2020  ,p_max+1):.     
+00001b90: 2020 2020 2020 2074 6869 735f 6d69 6e20         this_min 
+00001ba0: 3d20 696e 7428 702a 2870 2b31 292f 3229  = int(p*(p+1)/2)
+00001bb0: 0a20 2020 2020 2020 2020 2020 2074 6869  .            thi
+00001bc0: 735f 6d61 7820 3d20 7468 6973 5f6d 696e  s_max = this_min
+00001bd0: 202b 2070 2b31 0a20 2020 2020 2020 2020   + p+1.         
+00001be0: 2020 2023 204e 6567 6174 6520 746f 2063     # Negate to c
+00001bf0: 6f6e 7665 7274 2066 726f 6d20 6465 7669  onvert from devi
+00001c00: 6174 696f 6e73 206f 6620 6465 7074 6820  ations of depth 
+00001c10: 746f 2072 6164 6975 730a 2020 2020 2020  to radius.      
+00001c20: 2020 2020 2020 4370 7120 3d20 2d73 6861        Cpq = -sha
+00001c30: 7065 5f6e 5b74 6869 735f 6d69 6e3a 7468  pe_n[this_min:th
+00001c40: 6973 5f6d 6178 2c32 5d0a 2020 2020 2020  is_max,2].      
+00001c50: 2020 2020 2020 5370 7120 3d20 2d73 6861        Spq = -sha
+00001c60: 7065 5f6e 5b74 6869 735f 6d69 6e3a 7468  pe_n[this_min:th
+00001c70: 6973 5f6d 6178 2c33 5d0a 0a20 2020 2020  is_max,3]..     
+00001c80: 2020 2020 2020 2063 6869 5f70 7173 203d         chi_pqs =
+00001c90: 2067 6574 5f63 6869 7071 5f66 726f 6d5f   get_chipq_from_
+00001ca0: 4353 7071 5f73 696e 676c 6528 702c 4370  CSpq_single(p,Cp
+00001cb0: 712c 5370 7129 0a20 2020 2020 2020 2020  q,Spq).         
+00001cc0: 2020 2066 6f72 2069 5f6c 6179 6572 2069     for i_layer i
+00001cd0: 6e20 7261 6e67 6528 6e5f 6264 7329 3a0a  n range(n_bds):.
+00001ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001cf0: 6173 796d 5f73 6861 7065 5b69 5f6c 6179  asym_shape[i_lay
+00001d00: 6572 2c3a 2c70 2c3a 702b 315d 203d 2063  er,:,p,:p+1] = c
+00001d10: 6869 5f70 7173 2a31 6533 202a 2073 6361  hi_pqs*1e3 * sca
+00001d20: 6c65 645f 7261 645b 695f 6c61 7965 725d  led_rad[i_layer]
+00001d30: 0a0a 2020 2020 656c 7365 3a0a 2020 2020  ..    else:.    
+00001d40: 2020 2020 2320 4966 2077 6520 676f 7420      # If we got 
+00001d50: 6865 7265 2c20 6e6f 6e65 206f 6620 7468  here, none of th
+00001d60: 6520 6f70 7469 6f6e 7320 7765 7265 2073  e options were s
+00001d70: 656c 6563 7465 642e 0a20 2020 2020 2020  elected..       
+00001d80: 2023 2041 7070 6c79 2061 7379 6d6d 6574   # Apply asymmet
+00001d90: 7279 2069 6e64 6570 656e 6465 6e74 6c79  ry independently
+00001da0: 2074 6f20 6561 6368 206c 6179 6572 2c20   to each layer, 
+00001db0: 616e 6420 7265 6164 2069 6e20 6f6e 6520  and read in one 
+00001dc0: 6669 6c65 2070 6572 206c 6179 6572 2e0a  file per layer..
+00001dd0: 2020 2020 2020 2020 7261 6973 6520 5275          raise Ru
+00001de0: 6e74 696d 6545 7272 6f72 2822 496e 6465  ntimeError("Inde
+00001df0: 7065 6e64 656e 746c 7920 6173 796d 6d65  pendently asymme
+00001e00: 7472 6963 206c 6179 6572 7320 6172 6520  tric layers are 
+00001e10: 6e6f 7420 696d 706c 656d 656e 7465 642e  not implemented.
+00001e20: 2229 0a20 2020 2020 2020 2066 6f72 206e  ").        for n
+00001e30: 5f6c 6179 6572 2069 6e20 7261 6e67 6528  _layer in range(
+00001e40: 312c 206e 5f62 6473 2b31 293a 0a20 2020  1, n_bds+1):.   
+00001e50: 2020 2020 2020 2020 2073 6861 7065 5f6e           shape_n
+00001e60: 203d 206e 702e 6c6f 6164 7478 7428 6f73   = np.loadtxt(os
+00001e70: 2e70 6174 682e 6a6f 696e 2866 7061 7468  .path.join(fpath
+00001e80: 2c20 6622 6465 7074 685f 6368 695f 7071  , f"depth_chi_pq
+00001e90: 5f73 6861 7065 7b6e 5f6c 6179 6572 7d5f  _shape{n_layer}_
+00001ea0: 7b62 666e 616d 657d 2e74 7874 2229 2c20  {bfname}.txt"), 
+00001eb0: 736b 6970 726f 7773 3d31 2c20 756e 7061  skiprows=1, unpa
+00001ec0: 636b 3d46 616c 7365 2c20 6465 6c69 6d69  ck=False, delimi
+00001ed0: 7465 723d 272c 2729 0a20 2020 2020 2020  ter=',').       
+00001ee0: 2020 2020 2066 6f72 2070 2069 6e20 7261       for p in ra
+00001ef0: 6e67 6528 312c 2070 5f6d 6178 2b31 293a  nge(1, p_max+1):
+00001f00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00001f10: 2022 2222 204e 6f74 2079 6574 2069 6d70   """ Not yet imp
+00001f20: 6c65 6d65 6e74 6564 2c20 6275 7420 7468  lemented, but th
+00001f30: 6973 2069 7320 6120 7374 6172 7469 6e67  is is a starting
+00001f40: 2070 6f69 6e74 2e0a 2020 2020 2020 2020   point..        
+00001f50: 2020 2020 2020 2020 7468 6973 5f6d 696e          this_min
+00001f60: 203d 2069 6e74 2870 2a28 702b 3129 2f32   = int(p*(p+1)/2
+00001f70: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00001f80: 2020 7468 6973 5f6d 6178 203d 2074 6869    this_max = thi
+00001f90: 735f 6d69 6e20 2b20 702b 310a 2020 2020  s_min + p+1.    
+00001fa0: 2020 2020 2020 2020 2020 2020 4370 7120              Cpq 
+00001fb0: 3d20 2d73 6861 7065 5f6e 5b74 6869 735f  = -shape_n[this_
+00001fc0: 6d69 6e3a 7468 6973 5f6d 6178 2c32 5d0a  min:this_max,2].
+00001fd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001fe0: 5370 7120 3d20 2d73 6861 7065 5f6e 5b74  Spq = -shape_n[t
+00001ff0: 6869 735f 6d69 6e3a 7468 6973 5f6d 6178  his_min:this_max
+00002000: 2c33 5d0a 0a20 2020 2020 2020 2020 2020  ,3]..           
+00002010: 2020 2020 2063 6869 5f6d 696e 203d 2070       chi_min = p
+00002020: 2a2a 3220 2d20 310a 2020 2020 2020 2020  **2 - 1.        
+00002030: 2020 2020 2020 2020 6368 695f 6d61 7820          chi_max 
+00002040: 3d20 2870 2b31 292a 2a32 202d 2031 0a20  = (p+1)**2 - 1. 
+00002050: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+00002060: 7379 6d5f 7368 6170 655b 6e5f 6c61 7965  sym_shape[n_laye
+00002070: 722c 6368 695f 6d69 6e3a 6368 695f 6d61  r,chi_min:chi_ma
+00002080: 785d 203d 2067 6574 5f63 6869 7071 5f66  x] = get_chipq_f
+00002090: 726f 6d5f 4353 7071 5f73 696e 676c 6528  rom_CSpq_single(
+000020a0: 702c 4370 712c 5370 7129 2222 220a 0a20  p,Cpq,Spq)""".. 
+000020b0: 2020 2069 6620 636f 6e76 6572 745f 6465     if convert_de
+000020c0: 7074 685f 746f 5f63 6869 7071 2061 6e64  pth_to_chipq and
+000020d0: 206e 6f74 2072 656c 6174 6976 653a 0a20   not relative:. 
+000020e0: 2020 2020 2020 2069 6620 626f 6479 6e61         if bodyna
+000020f0: 6d65 203d 3d20 2245 7572 6f70 6122 3a0a  me == "Europa":.
+00002100: 2020 2020 2020 2020 2020 2020 6966 2061              if a
+00002110: 7070 656e 6420 3d3d 2022 5f54 6f62 6965  ppend == "_Tobie
+00002120: 223a 0a20 2020 2020 2020 2020 2020 2020  ":.             
+00002130: 2020 2065 7073 5f6d 6178 203d 2032 3530     eps_max = 250
+00002140: 300a 2020 2020 2020 2020 2020 2020 656c  0.            el
+00002150: 6966 2061 7070 656e 6420 3d3d 2022 5f70  if append == "_p
+00002160: 7265 7622 3a0a 2020 2020 2020 2020 2020  rev":.          
+00002170: 2020 2020 2020 6570 735f 6d61 7820 3d20        eps_max = 
+00002180: 3235 3030 0a20 2020 2020 2020 2020 2020  2500.           
+00002190: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+000021a0: 2020 2020 2020 2065 7073 5f6d 6178 203d         eps_max =
+000021b0: 2033 3030 3030 0a20 2020 2020 2020 2065   30000.        e
+000021c0: 6c69 6620 626f 6479 6e61 6d65 203d 3d20  lif bodyname == 
+000021d0: 2243 616c 6c69 7374 6f22 3a0a 2020 2020  "Callisto":.    
+000021e0: 2020 2020 2020 2020 6570 735f 6d61 7820          eps_max 
+000021f0: 3d20 3130 3030 3030 0a20 2020 2020 2020  = 100000.       
+00002200: 2065 6c69 6620 626f 6479 6e61 6d65 203d   elif bodyname =
+00002210: 3d20 2254 7269 746f 6e22 3a0a 2020 2020  = "Triton":.    
+00002220: 2020 2020 2020 2020 6570 735f 6d61 7820          eps_max 
+00002230: 3d20 3130 3030 3030 0a20 2020 2020 2020  = 100000.       
+00002240: 2065 6c69 6620 626f 6479 6e61 6d65 203d   elif bodyname =
+00002250: 3d20 224d 6972 616e 6461 223a 0a20 2020  = "Miranda":.   
+00002260: 2020 2020 2020 2020 2065 7073 5f6d 6178           eps_max
+00002270: 203d 2034 3938 3130 2f32 3038 3532 202a   = 49810/20852 *
+00002280: 2031 3633 3737 2023 2053 6361 6c69 6e67   16377 # Scaling
+00002290: 2075 7020 6672 6f6d 206d 6178 696d 756d   up from maximum
+000022a0: 2064 6576 6961 7469 6f6e 2069 6e20 4865   deviation in He
+000022b0: 6d69 6e67 7761 7920 616e 6420 4d69 7474  mingway and Mitt
+000022c0: 616c 2028 3230 3139 2920 456e 6365 6c61  al (2019) Encela
+000022d0: 6475 7320 6d6f 6465 6c20 746f 2074 6869  dus model to thi
+000022e0: 636b 6572 204d 6972 616e 6461 2069 6365  cker Miranda ice
+000022f0: 2073 6865 6c6c 0a20 2020 2020 2020 2065   shell.        e
+00002300: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+00002310: 2065 7073 5f6d 6178 203d 2031 3633 3737   eps_max = 16377
+00002320: 0a20 2020 2020 2020 2023 2057 6865 7468  .        # Wheth
+00002330: 6572 2074 6f20 7072 696e 7420 6c69 6e65  er to print line
+00002340: 7320 7375 6974 6162 6c65 2066 6f72 2063  s suitable for c
+00002350: 6f70 7969 6e67 2074 6f20 626f 756e 6461  opying to bounda
+00002360: 7279 2073 6861 7065 2066 696c 6573 2c0a  ry shape files,.
+00002370: 2020 2020 2020 2020 2320 6f72 2074 6f20          # or to 
+00002380: 7072 696e 7420 666f 7220 7265 6164 6162  print for readab
+00002390: 696c 6974 7920 696e 7374 6561 640a 2020  ility instead.  
+000023a0: 2020 2020 2020 7072 696e 745f 666f 725f        print_for_
+000023b0: 636f 7079 203d 2054 7275 650a 2020 2020  copy = True.    
+000023c0: 2020 2020 6966 2070 7269 6e74 5f66 6f72      if print_for
+000023d0: 5f63 6f70 793a 0a20 2020 2020 2020 2020  _copy:.         
+000023e0: 2020 2063 6869 5f68 6561 6420 3d20 6622     chi_head = f"
+000023f0: 2070 2c20 6368 6970 7120 282d 712c 202e   p, chipq (-q, .
+00002400: 2e2e 2c20 7129 3b20 6263 6465 763d 7b65  .., q); bcdev={e
+00002410: 7073 5f6d 6178 7d20 6d5c 6e22 0a20 2020  ps_max} m\n".   
+00002420: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+00002430: 2020 2020 2020 2063 6869 5f68 6561 6420         chi_head 
+00002440: 3d20 6622 2070 2c20 712c 2063 6869 7071  = f" p, q, chipq
+00002450: 5f72 652c 2063 6869 7071 5f69 6d2c 2062  _re, chipq_im, b
+00002460: 6364 6576 3d7b 6570 735f 6d61 787d 206d  cdev={eps_max} m
+00002470: 5c6e 220a 2020 2020 2020 2020 6570 7320  \n".        eps 
+00002480: 3d20 6173 796d 5f73 6861 7065 5b72 5f69  = asym_shape[r_i
+00002490: 6f2c 202e 2e2e 5d20 2f20 6570 735f 6d61  o, ...] / eps_ma
+000024a0: 780a 2020 2020 2020 2020 6173 796d 5f6f  x.        asym_o
+000024b0: 7574 203d 206f 732e 7061 7468 2e6a 6f69  ut = os.path.joi
+000024c0: 6e28 6670 6174 682c 2066 2263 6869 5f70  n(fpath, f"chi_p
+000024d0: 715f 7b62 6f64 796e 616d 657d 2e74 7874  q_{bodyname}.txt
+000024e0: 2229 0a20 2020 2020 2020 2077 6974 6820  ").        with 
+000024f0: 6f70 656e 2861 7379 6d5f 6f75 742c 2022  open(asym_out, "
+00002500: 7722 2920 6173 2066 5f63 6869 3a0a 2020  w") as f_chi:.  
+00002510: 2020 2020 2020 2020 2020 665f 6368 692e            f_chi.
+00002520: 7772 6974 6528 6368 695f 6865 6164 290a  write(chi_head).
+00002530: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+00002540: 7020 696e 2072 616e 6765 2831 2c20 705f  p in range(1, p_
+00002550: 6d61 782b 3129 3a0a 2020 2020 2020 2020  max+1):.        
+00002560: 2020 2020 2020 2020 6966 2070 7269 6e74          if print
+00002570: 5f66 6f72 5f63 6f70 793a 0a20 2020 2020  _for_copy:.     
+00002580: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+00002590: 6869 735f 6c69 6e65 203d 2022 2022 202b  his_line = " " +
+000025a0: 2073 7472 2870 290a 2020 2020 2020 2020   str(p).        
+000025b0: 2020 2020 2020 2020 666f 7220 7120 696e          for q in
+000025c0: 2072 616e 6765 282d 702c 2070 2b31 293a   range(-p, p+1):
+000025d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000025e0: 2020 2020 2071 7369 676e 203d 2069 6e74       qsign = int
+000025f0: 2871 3c30 290a 2020 2020 2020 2020 2020  (q<0).          
+00002600: 2020 2020 2020 2020 2020 7161 6273 203d            qabs =
+00002610: 2061 6273 2871 290a 2020 2020 2020 2020   abs(q).        
+00002620: 2020 2020 2020 2020 2020 2020 6966 2070              if p
+00002630: 7269 6e74 5f66 6f72 5f63 6f70 793a 0a20  rint_for_copy:. 
 00002640: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002650: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-00002660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002670: 2020 6274 775f 6368 6172 203d 2022 2d22    btw_char = "-"
-00002680: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002690: 2020 2020 2020 2020 2074 6869 735f 6c69           this_li
-000026a0: 6e65 203d 2066 227b 7468 6973 5f6c 696e  ne = f"{this_lin
-000026b0: 657d 2c20 7b6e 702e 7265 616c 2865 7073  e}, {np.real(eps
-000026c0: 5b71 7369 676e 2c20 702c 2071 6162 735d  [qsign, p, qabs]
-000026d0: 297d 7b62 7477 5f63 6861 727d 7b6e 702e  )}{btw_char}{np.
-000026e0: 6162 7328 6e70 2e69 6d61 6728 6570 735b  abs(np.imag(eps[
-000026f0: 7173 6967 6e2c 2070 2c20 7161 6273 5d29  qsign, p, qabs])
-00002700: 297d 6a22 0a20 2020 2020 2020 2020 2020  )}j".           
-00002710: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
-00002720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002730: 2020 2020 2020 2074 6869 735f 6c69 6e65         this_line
-00002740: 203d 2066 2220 7b70 7d2c 207b 7374 7228   = f" {p}, {str(
-00002750: 7129 2e72 6a75 7374 2832 297d 2c20 7b6e  q).rjust(2)}, {n
-00002760: 702e 7265 616c 2865 7073 5b71 7369 676e  p.real(eps[qsign
-00002770: 2c20 702c 2071 6162 735d 297d 7b62 7477  , p, qabs])}{btw
-00002780: 5f63 6861 727d 7b6e 702e 6162 7328 6e70  _char}{np.abs(np
-00002790: 2e69 6d61 6728 6570 735b 7173 6967 6e2c  .imag(eps[qsign,
-000027a0: 2070 2c20 7161 6273 5d29 297d 5c6e 220a   p, qabs]))}\n".
-000027b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000027c0: 2020 2020 2020 2020 665f 6368 692e 7772          f_chi.wr
-000027d0: 6974 6528 7468 6973 5f6c 696e 6529 0a20  ite(this_line). 
-000027e0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-000027f0: 6620 7072 696e 745f 666f 725f 636f 7079  f print_for_copy
-00002800: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00002810: 2020 2020 2020 665f 6368 692e 7772 6974        f_chi.writ
-00002820: 6528 7468 6973 5f6c 696e 652b 225c 6e22  e(this_line+"\n"
-00002830: 290a 2020 2020 2020 2020 6c6f 672e 6465  ).        log.de
-00002840: 6275 6728 6622 5072 696e 7465 6420 6368  bug(f"Printed ch
-00002850: 695f 7071 2076 616c 7565 7320 746f 207b  i_pq values to {
-00002860: 6173 796d 5f6f 7574 7d22 290a 0a20 2020  asym_out}")..   
-00002870: 2023 2049 6620 7468 6973 2066 696c 6520   # If this file 
-00002880: 6578 6973 7473 2c20 6d6f 6465 6c20 7469  exists, model ti
-00002890: 6461 6c20 7065 7274 7572 6261 7469 6f6e  dal perturbation
-000028a0: 732e 2049 6620 6e6f 742c 2072 6574 7572  s. If not, retur
-000028b0: 6e20 4e6f 6e65 2e0a 2020 2020 6772 6176  n None..    grav
-000028c0: 5f6d 6f64 656c 203d 206f 732e 7061 7468  _model = os.path
-000028d0: 2e6a 6f69 6e28 6670 6174 682c 2066 2267  .join(fpath, f"g
-000028e0: 7261 7669 7479 7b62 666e 616d 657d 7b61  ravity{bfname}{a
-000028f0: 7070 656e 647d 2e74 7874 2229 0a20 2020  ppend}.txt").   
-00002900: 2074 7279 3a0a 2020 2020 2020 2020 675f   try:.        g_
-00002910: 7368 6170 655f 6e20 3d20 6e70 2e6c 6f61  shape_n = np.loa
-00002920: 6474 7874 2867 7261 765f 6d6f 6465 6c2c  dtxt(grav_model,
-00002930: 2073 6b69 7072 6f77 733d 312c 2075 6e70   skiprows=1, unp
-00002940: 6163 6b3d 4661 6c73 652c 2064 656c 696d  ack=False, delim
-00002950: 6974 6572 3d27 2c27 290a 2020 2020 6578  iter=',').    ex
-00002960: 6365 7074 3a0a 2020 2020 2020 2020 6772  cept:.        gr
-00002970: 6176 5f73 6861 7065 203d 204e 6f6e 650a  av_shape = None.
-00002980: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00002990: 2020 6c6f 672e 6465 6275 6728 6622 5573    log.debug(f"Us
-000029a0: 696e 6720 7375 7266 6163 6520 6772 6176  ing surface grav
-000029b0: 6974 7920 7368 6170 653a 207b 6772 6176  ity shape: {grav
-000029c0: 5f6d 6f64 656c 7d22 290a 2020 2020 2020  _model}").      
-000029d0: 2020 666f 7220 7020 696e 2072 616e 6765    for p in range
-000029e0: 2831 2c20 705f 6d61 7820 2b20 3129 3a0a  (1, p_max + 1):.
-000029f0: 2020 2020 2020 2020 2020 2020 7468 6973              this
-00002a00: 5f6d 696e 203d 2069 6e74 2870 202a 2028  _min = int(p * (
-00002a10: 7020 2b20 3129 202f 2032 290a 2020 2020  p + 1) / 2).    
-00002a20: 2020 2020 2020 2020 7468 6973 5f6d 6178          this_max
-00002a30: 203d 2074 6869 735f 6d69 6e20 2b20 7020   = this_min + p 
-00002a40: 2b20 310a 2020 2020 2020 2020 2020 2020  + 1.            
-00002a50: 2320 556e 6c69 6b65 2061 626f 7665 2c20  # Unlike above, 
-00002a60: 7765 2064 6f20 6e6f 7420 6e65 6564 2074  we do not need t
-00002a70: 6f20 6e65 6761 7465 2062 6563 6175 7365  o negate because
-00002a80: 2064 6576 6961 7469 6f6e 7320 6172 6520   deviations are 
-00002a90: 616c 7265 6164 7920 696e 2072 6164 6969  already in radii
-00002aa0: 0a20 2020 2020 2020 2020 2020 2067 4370  .            gCp
-00002ab0: 7120 3d20 675f 7368 6170 655f 6e5b 7468  q = g_shape_n[th
-00002ac0: 6973 5f6d 696e 3a74 6869 735f 6d61 782c  is_min:this_max,
-00002ad0: 2032 5d0a 2020 2020 2020 2020 2020 2020   2].            
-00002ae0: 6753 7071 203d 2067 5f73 6861 7065 5f6e  gSpq = g_shape_n
-00002af0: 5b74 6869 735f 6d69 6e3a 7468 6973 5f6d  [this_min:this_m
-00002b00: 6178 2c20 335d 0a0a 2020 2020 2020 2020  ax, 3]..        
-00002b10: 2020 2020 675f 6368 695f 7071 7320 3d20      g_chi_pqs = 
-00002b20: 6765 745f 6368 6970 715f 6672 6f6d 5f43  get_chipq_from_C
-00002b30: 5370 7128 702c 2067 4370 712c 2067 5370  Spq(p, gCpq, gSp
-00002b40: 7129 0a20 2020 2020 2020 2020 2020 2066  q).            f
-00002b50: 6f72 2069 6920 696e 2072 616e 6765 286e  or ii in range(n
-00002b60: 5f62 6473 202b 2072 5f69 6f20 2b20 3129  _bds + r_io + 1)
-00002b70: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00002b80: 2020 2320 4966 2077 6520 6172 6520 6d6f    # If we are mo
-00002b90: 6465 6c69 6e67 2061 7379 6d6d 6574 7279  deling asymmetry
-00002ba0: 2069 6e20 616e 7920 7375 7266 6163 652c   in any surface,
-00002bb0: 2069 7420 6973 2061 646a 6163 656e 7420   it is adjacent 
-00002bc0: 746f 2061 2063 6f6e 6475 6374 696e 6720  to a conducting 
-00002bd0: 6c61 7965 720a 2020 2020 2020 2020 2020  layer.          
-00002be0: 2020 2020 2020 6966 2028 6173 796d 5f73        if (asym_s
-00002bf0: 6861 7065 5b69 692c 202e 2e2e 5d20 213d  hape[ii, ...] !=
-00002c00: 2030 292e 616e 7928 293a 0a20 2020 2020   0).any():.     
-00002c10: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-00002c20: 2041 7070 6c79 2073 7572 6661 6365 2074   Apply surface t
-00002c30: 6964 616c 2070 6572 7475 7262 6174 696f  idal perturbatio
-00002c40: 6e73 2074 6f20 616c 6c20 6173 796d 6d65  ns to all asymme
-00002c50: 7472 6963 206c 6179 6572 7320 6571 7561  tric layers equa
-00002c60: 6c6c 790a 2020 2020 2020 2020 2020 2020  lly.            
-00002c70: 2020 2020 2020 2020 2320 2874 6f20 7072          # (to pr
-00002c80: 6573 6572 7665 2074 6869 636b 6e65 7373  eserve thickness
-00002c90: 6573 2064 6574 6572 6d69 6e65 6420 6279  es determined by
-00002ca0: 2074 6865 726d 6f64 796e 616d 6963 7329   thermodynamics)
-00002cb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00002cc0: 2020 2020 2067 7261 765f 7368 6170 655b       grav_shape[
-00002cd0: 6969 2c20 3a2c 2070 2c20 3a70 2b31 5d20  ii, :, p, :p+1] 
-00002ce0: 3d20 675f 6368 695f 7071 7320 2a20 3165  = g_chi_pqs * 1e
-00002cf0: 330a 0a20 2020 2020 2020 2020 2020 2023  3..            #
-00002d00: 2041 6c77 6179 7320 6164 6420 7065 7274   Always add pert
-00002d10: 7572 6261 7469 6f6e 2074 6f20 626f 6479  urbation to body
-00002d20: 2073 7572 6661 6365 0a20 2020 2020 2020   surface.       
-00002d30: 2020 2020 2067 7261 765f 7368 6170 655b       grav_shape[
-00002d40: 6e5f 6264 732b 725f 696f 2b31 2c20 3a2c  n_bds+r_io+1, :,
-00002d50: 2070 2c20 3a70 2b31 5d20 3d20 675f 6368   p, :p+1] = g_ch
-00002d60: 695f 7071 7320 2a20 3165 330a 2020 2020  i_pqs * 1e3.    
-00002d70: 7265 7475 726e 2061 7379 6d5f 7368 6170  return asym_shap
-00002d80: 652c 2067 7261 765f 7368 6170 650a 0a23  e, grav_shape..#
-00002d90: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00002da0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00002db0: 2323 2323 2323 2323 2323 2323 0a0a 2222  ############..""
-00002dc0: 220a 6765 745f 6368 6970 715f 6672 6f6d  ".get_chipq_from
-00002dd0: 5f43 5370 7128 290a 2020 2020 436f 6e76  _CSpq().    Conv
-00002de0: 6572 7420 6672 6f6d 2072 6561 6c2c 2034  ert from real, 4
-00002df0: 7069 2d6e 6f72 6d61 6c69 7a65 6420 6861  pi-normalized ha
-00002e00: 726d 6f6e 6963 2063 6f65 6666 6963 6965  rmonic coefficie
-00002e10: 6e74 7320 7769 7468 206e 6f20 436f 6e64  nts with no Cond
-00002e20: 6f6e 2d53 686f 7274 6c65 7920 7068 6173  on-Shortley phas
-00002e30: 650a 2020 2020 2874 6865 2063 6f6d 6d6f  e.    (the commo
-00002e40: 6e20 6e6f 726d 616c 697a 6174 696f 6e20  n normalization 
-00002e50: 696e 2074 6865 2067 656f 6465 7379 2063  in the geodesy c
-00002e60: 6f6d 6d75 6e69 7479 2920 746f 206f 7274  ommunity) to ort
-00002e70: 686f 6e6f 726d 616c 2068 6172 6d6f 6e69  honormal harmoni
-00002e80: 6320 636f 6566 6669 6369 656e 7473 2068  c coefficients h
-00002e90: 6176 696e 670a 2020 2020 7468 6520 432d  aving.    the C-
-00002ea0: 5320 7068 6173 652e 2048 616e 646c 6573  S phase. Handles
-00002eb0: 2061 6c6c 2076 616c 7565 7320 666f 7220   all values for 
-00002ec0: 6120 6769 7665 6e20 7020 6174 206f 6e63  a given p at onc
-00002ed0: 652e 0a20 2020 2055 7361 6765 3a20 6063  e..    Usage: `c
-00002ee0: 6869 7071 6020 3d20 6765 745f 6368 6970  hipq` = get_chip
-00002ef0: 715f 6672 6f6d 5f43 5370 7128 6070 602c  q_from_CSpq(`p`,
-00002f00: 6043 7071 602c 6053 7071 6029 0a20 2020  `Cpq`,`Spq`).   
-00002f10: 2052 6574 7572 6e73 3a0a 2020 2020 2020   Returns:.      
-00002f20: 2020 6368 6970 713a 2063 6f6d 706c 6578    chipq: complex
-00002f30: 2c20 7368 6170 6528 322c 702b 3129 2e20  , shape(2,p+1). 
-00002f40: 6368 695f 7071 2076 616c 7565 7320 666f  chi_pq values fo
-00002f50: 7220 616c 6c20 7120 3d20 5b2d 702c 705d  r all q = [-p,p]
-00002f60: 2c20 6f72 6761 6e69 7a65 6420 7375 6368  , organized such
-00002f70: 2074 6861 7420 6368 6970 715b 696e 7428   that chipq[int(
-00002f80: 713c 3029 2c61 6273 2871 295d 0a20 2020  q<0),abs(q)].   
-00002f90: 2020 2020 2020 2020 2072 6574 7572 6e73           returns
-00002fa0: 2074 6865 2072 6573 756c 7420 666f 7220   the result for 
-00002fb0: 6120 7061 7274 6963 756c 6172 2071 2076  a particular q v
-00002fc0: 616c 7565 2e20 4f72 7468 6f6e 6f72 6d61  alue. Orthonorma
-00002fd0: 6c2c 2077 6974 6820 436f 6e64 6f6e 2d53  l, with Condon-S
-00002fe0: 686f 7274 6c65 7920 7068 6173 652e 0a20  hortley phase.. 
-00002ff0: 2020 2020 2020 2020 2020 204f 7274 686f             Ortho
-00003000: 6e6f 726d 616c 2068 6572 6520 6d65 616e  normal here mean
-00003010: 7320 7468 6520 696e 7465 6772 616c 206f  s the integral o
-00003020: 6620 7c59 6e6d 7c5e 3220 2a20 644f 6d65  f |Ynm|^2 * dOme
-00003030: 6761 206f 7665 7220 6120 756e 6974 2073  ga over a unit s
-00003040: 7068 6572 6520 6973 2031 2066 6f72 2061  phere is 1 for a
-00003050: 6c6c 206e 2061 6e64 206d 2e0a 2020 2020  ll n and m..    
-00003060: 5061 7261 6d65 7465 7273 3a0a 2020 2020  Parameters:.    
-00003070: 2020 2020 703a 2069 6e74 6567 6572 2e20      p: integer. 
-00003080: 4465 6772 6565 206f 6620 626f 756e 6461  Degree of bounda
-00003090: 7279 2073 6861 7065 733b 2072 6573 756c  ry shapes; resul
-000030a0: 7473 2066 6f72 2061 6c6c 2071 2076 616c  ts for all q val
-000030b0: 7565 7320 6172 6520 7265 7475 726e 6564  ues are returned
-000030c0: 2066 6f72 2074 6869 7320 7020 7661 6c75   for this p valu
-000030d0: 652e 0a20 2020 2020 2020 2043 7071 3a20  e..        Cpq: 
-000030e0: 666c 6f61 742e 2053 7068 6572 6963 616c  float. Spherical
-000030f0: 2068 6172 6d6f 6e69 6320 636f 6566 6669   harmonic coeffi
-00003100: 6369 656e 7420 7468 6174 206d 756c 7469  cient that multi
-00003110: 706c 6965 7320 636f 7328 6d2a 7068 6929  plies cos(m*phi)
-00003120: 2066 6f72 2070 2c71 2062 6f75 6e64 6172   for p,q boundar
-00003130: 792e 2034 7069 2d6e 6f72 6d61 6c69 7a65  y. 4pi-normalize
-00003140: 6420 7769 7468 206e 6f20 436f 6e64 6f6e  d with no Condon
-00003150: 2d53 686f 7274 6c65 7920 7068 6173 652e  -Shortley phase.
-00003160: 0a20 2020 2020 2020 2053 7071 3a20 666c  .        Spq: fl
-00003170: 6f61 742e 2053 7068 6572 6963 616c 2068  oat. Spherical h
-00003180: 6172 6d6f 6e69 6320 636f 6566 6669 6369  armonic coeffici
-00003190: 656e 7420 7468 6174 206d 756c 7469 706c  ent that multipl
-000031a0: 6965 7320 7369 6e28 6d2a 7068 6929 2066  ies sin(m*phi) f
-000031b0: 6f72 2070 2c71 2062 6f75 6e64 6172 792e  or p,q boundary.
-000031c0: 2034 7069 2d6e 6f72 6d61 6c69 7a65 6420   4pi-normalized 
-000031d0: 7769 7468 206e 6f20 436f 6e64 6f6e 2d53  with no Condon-S
-000031e0: 686f 7274 6c65 7920 7068 6173 652e 0a20  hortley phase.. 
-000031f0: 2020 2022 2222 0a64 6566 2067 6574 5f63     """.def get_c
-00003200: 6869 7071 5f66 726f 6d5f 4353 7071 2870  hipq_from_CSpq(p
-00003210: 2c43 7071 2c53 7071 293a 0a20 2020 2063  ,Cpq,Spq):.    c
-00003220: 6869 7071 203d 206e 702e 7a65 726f 7328  hipq = np.zeros(
-00003230: 2832 2c70 2b31 292c 6474 7970 653d 6e70  (2,p+1),dtype=np
-00003240: 2e63 6f6d 706c 6578 5f29 0a0a 2020 2020  .complex_)..    
-00003250: 6e6f 726d 203d 2073 7172 7434 7069 202f  norm = sqrt4pi /
-00003260: 2073 7172 7432 0a0a 2020 2020 666f 7220   sqrt2..    for 
-00003270: 7120 696e 2072 616e 6765 2831 2c70 2b31  q in range(1,p+1
-00003280: 293a 0a20 2020 2020 2020 2023 204e 6567  ):.        # Neg
-00003290: 6174 6976 6520 7120 2866 6972 7374 2069  ative q (first i
-000032a0: 6e64 6578 2031 293a 0a20 2020 2020 2020  ndex 1):.       
-000032b0: 2063 6869 7071 5b31 2c71 5d20 3d20 2843   chipq[1,q] = (C
-000032c0: 7071 5b71 5d20 2b20 316a 2a53 7071 5b71  pq[q] + 1j*Spq[q
-000032d0: 5d29 202a 206e 6f72 6d0a 2020 2020 2020  ]) * norm.      
-000032e0: 2020 2320 506f 7369 7469 7665 2071 2028    # Positive q (
-000032f0: 6669 7273 7420 696e 6465 7820 3029 3a0a  first index 0):.
-00003300: 2020 2020 2020 2020 6368 6970 715b 302c          chipq[0,
-00003310: 715d 203d 2028 2d31 292a 2a71 202a 2028  q] = (-1)**q * (
-00003320: 4370 715b 715d 202d 2031 6a2a 5370 715b  Cpq[q] - 1j*Spq[
-00003330: 715d 2920 2a20 6e6f 726d 0a0a 2020 2020  q]) * norm..    
-00003340: 6368 6970 715b 302c 305d 203d 2043 7071  chipq[0,0] = Cpq
-00003350: 5b30 5d20 2a20 7371 7274 3470 690a 0a20  [0] * sqrt4pi.. 
-00003360: 2020 2072 6574 7572 6e20 6368 6970 710a     return chipq.
-00003370: 0a23 2323 2323 2323 2323 2323 2323 2323  .###############
-00003380: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00003390: 2323 2323 2323 2323 2323 2323 2323 0a0a  ##############..
-000033a0: 2222 220a 6765 745f 6768 5f66 726f 6d5f  """.get_gh_from_
-000033b0: 4269 6e6d 2829 0a20 2020 2043 6f6e 7665  Binm().    Conve
-000033c0: 7274 2066 726f 6d20 6f72 7468 6f6e 6f72  rt from orthonor
-000033d0: 6d61 6c20 6861 726d 6f6e 6963 2063 6f65  mal harmonic coe
-000033e0: 6666 6963 6965 6e74 7320 7769 7468 2074  fficients with t
-000033f0: 6865 2043 6f6e 646f 6e2d 5368 6f72 746c  he Condon-Shortl
-00003400: 6579 2070 6861 7365 2028 636f 6d6d 6f6e  ey phase (common
-00003410: 2069 6e20 7068 7973 6963 7329 0a20 2020   in physics).   
-00003420: 2074 6f20 5363 686d 6964 7420 7365 6d69   to Schmidt semi
-00003430: 2d6e 6f72 6d61 6c69 7a65 6420 666f 726d  -normalized form
-00003440: 2077 6974 686f 7574 2074 6865 2043 2d53   without the C-S
-00003450: 2070 6861 7365 2028 636f 6d6d 6f6e 2069   phase (common i
-00003460: 6e20 6765 6f70 6879 7369 6373 292e 0a20  n geophysics).. 
-00003470: 2020 2048 616e 646c 6573 2061 6c6c 2076     Handles all v
-00003480: 616c 7565 7320 666f 7220 6120 6769 7665  alues for a give
-00003490: 6e20 6e20 6174 206f 6e63 652e 0a20 2020  n n at once..   
-000034a0: 2055 7361 6765 3a20 6067 6e6d 2c20 686e   Usage: `gnm, hn
-000034b0: 6d60 203d 2067 6574 5f67 685f 6672 6f6d  m` = get_gh_from
-000034c0: 5f42 696e 6d28 606e 602c 2060 6e5f 6d61  _Binm(`n`, `n_ma
-000034d0: 7860 2c20 6042 696e 6d60 290a 2020 2020  x`, `Binm`).    
-000034e0: 5265 7475 726e 733a 0a20 2020 2020 2020  Returns:.       
-000034f0: 2067 6e6d 2c20 686e 6d3a 2063 6f6d 706c   gnm, hnm: compl
-00003500: 6578 2c20 7368 6170 6528 6e5f 6d61 782b  ex, shape(n_max+
-00003510: 312c 6e5f 6d61 782b 3129 2e20 675f 6e6d  1,n_max+1). g_nm
-00003520: 2061 6e64 2068 5f6e 6d20 7661 6c75 6573   and h_nm values
-00003530: 2066 6f72 2061 6c6c 206d 203d 205b 302c   for all m = [0,
-00003540: 6e5d 2e0a 0a20 2020 2020 2020 2020 2020  n]...           
-00003550: 2053 6368 6d69 6474 206e 6f72 6d61 6c69   Schmidt normali
-00003560: 7a61 7469 6f6e 2068 6572 6520 6d65 616e  zation here mean
-00003570: 7320 7468 6520 696e 7465 6772 616c 206f  s the integral o
-00003580: 6620 7c59 6e6d 7c5e 3220 2a20 644f 6d65  f |Ynm|^2 * dOme
-00003590: 6761 206f 7665 7220 6120 756e 6974 2073  ga over a unit s
-000035a0: 7068 6572 6520 6973 0a20 2020 2020 2020  phere is.       
-000035b0: 2020 2020 2034 7069 2f28 326e 2b31 2920       4pi/(2n+1) 
-000035c0: 666f 7220 616c 6c20 6e20 616e 6420 6d2e  for all n and m.
-000035d0: 204e 6f20 436f 6e64 6f6e 2d53 686f 7274   No Condon-Short
-000035e0: 6c65 7920 7068 6173 652e 0a20 2020 2050  ley phase..    P
-000035f0: 6172 616d 6574 6572 733a 0a20 2020 2020  arameters:.     
-00003600: 2020 206e 5f6d 6178 3a20 696e 7465 6765     n_max: intege
-00003610: 722e 204d 6178 696d 756d 2064 6567 7265  r. Maximum degre
-00003620: 6520 6e20 6f66 2069 6e64 7563 6564 206d  e n of induced m
-00003630: 6f6d 656e 7473 2e0a 2020 2020 2020 2020  oments..        
-00003640: 4269 6e6d 3a20 636f 6d70 6c65 782c 2073  Binm: complex, s
-00003650: 6861 7065 2832 2c6e 5f6d 6178 2b31 2c6e  hape(2,n_max+1,n
-00003660: 5f6d 6178 2b31 292e 2043 6f6d 706c 6578  _max+1). Complex
-00003670: 2069 6e64 7563 6564 206d 6167 6e65 7469   induced magneti
-00003680: 6320 6d6f 6d65 6e74 7320 6361 6c63 756c  c moments calcul
-00003690: 6174 6564 2075 7369 6e67 2066 756c 6c79  ated using fully
-000036a0: 206e 6f72 6d61 6c69 7a65 6420 7370 6865   normalized sphe
-000036b0: 7269 6361 6c20 6861 726d 6f6e 6963 2063  rical harmonic c
-000036c0: 6f65 6666 6963 6965 6e74 732e 0a20 2020  oefficients..   
-000036d0: 2022 2222 0a64 6566 2067 6574 5f67 685f   """.def get_gh_
-000036e0: 6672 6f6d 5f42 696e 6d28 6e5f 6d61 782c  from_Binm(n_max,
-000036f0: 2042 696e 6d29 3a0a 2020 2020 676e 6d2c   Binm):.    gnm,
-00003700: 2068 6e6d 203d 2028 206e 702e 7a65 726f   hnm = ( np.zero
-00003710: 7328 286e 5f6d 6178 2b31 2c6e 5f6d 6178  s((n_max+1,n_max
-00003720: 2b31 292c 6474 7970 653d 6e70 2e63 6f6d  +1),dtype=np.com
-00003730: 706c 6578 5f29 2066 6f72 205f 2069 6e20  plex_) for _ in 
-00003740: 7261 6e67 6528 3229 2029 0a0a 2020 2020  range(2) )..    
-00003750: 666f 7220 6e20 696e 2072 616e 6765 2831  for n in range(1
-00003760: 2c6e 5f6d 6178 2b31 293a 0a20 2020 2020  ,n_max+1):.     
-00003770: 2020 206e 6f72 6d20 3d20 6e70 2e73 7172     norm = np.sqr
-00003780: 7428 322a 6e2b 3129 202f 2073 7172 7432  t(2*n+1) / sqrt2
-00003790: 202f 2073 7172 7434 7069 0a0a 2020 2020   / sqrt4pi..    
-000037a0: 2020 2020 666f 7220 6d20 696e 2072 616e      for m in ran
-000037b0: 6765 2831 2c6e 2b31 293a 0a20 2020 2020  ge(1,n+1):.     
-000037c0: 2020 2020 2020 2023 2067 2074 6572 6d73         # g terms
-000037d0: 3a0a 2020 2020 2020 2020 2020 2020 676e  :.            gn
-000037e0: 6d5b 6e2c 6d5d 203d 2028 282d 3129 2a2a  m[n,m] = ((-1)**
-000037f0: 6d20 2a20 4269 6e6d 5b30 2c6e 2c6d 5d20  m * Binm[0,n,m] 
-00003800: 2b20 4269 6e6d 5b31 2c6e 2c6d 5d29 202a  + Binm[1,n,m]) *
-00003810: 206e 6f72 6d0a 2020 2020 2020 2020 2020   norm.          
-00003820: 2020 2320 6820 7465 726d 733a 0a20 2020    # h terms:.   
-00003830: 2020 2020 2020 2020 2068 6e6d 5b6e 2c6d           hnm[n,m
-00003840: 5d20 3d20 2828 2d31 292a 2a6d 202a 2042  ] = ((-1)**m * B
-00003850: 696e 6d5b 302c 6e2c 6d5d 202d 2042 696e  inm[0,n,m] - Bin
-00003860: 6d5b 312c 6e2c 6d5d 2920 2a20 316a 202a  m[1,n,m]) * 1j *
-00003870: 206e 6f72 6d0a 0a20 2020 2020 2020 2067   norm..        g
-00003880: 6e6d 5b6e 2c30 5d20 3d20 4269 6e6d 5b30  nm[n,0] = Binm[0
-00003890: 2c6e 2c30 5d20 2a20 6e6f 726d 202a 2073  ,n,0] * norm * s
-000038a0: 7172 7432 0a0a 2020 2020 7265 7475 726e  qrt2..    return
-000038b0: 2067 6e6d 2c20 686e 6d0a 0a23 2323 2323   gnm, hnm..#####
-000038c0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000038d0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000038e0: 2323 2323 2323 2323 0a0a 2222 220a 7661  ########..""".va
-000038f0: 6c69 6461 7465 2829 0a20 2020 2043 6865  lidate().    Che
-00003900: 636b 2069 6e70 7574 7320 746f 2062 6520  ck inputs to be 
-00003910: 7375 7265 2065 7665 7279 7468 696e 6720  sure everything 
-00003920: 7769 6c6c 2062 6520 696e 7465 7270 7265  will be interpre
-00003930: 7465 6420 636f 7272 6563 746c 792e 0a20  ted correctly.. 
-00003940: 2020 2055 7361 6765 3a20 6072 5f62 6473     Usage: `r_bds
-00003950: 602c 2060 7369 676d 6173 602c 2060 6f6d  `, `sigmas`, `om
-00003960: 6567 6173 602c 2060 6173 796d 5f73 6861  egas`, `asym_sha
-00003970: 7065 6020 3d20 7661 6c69 6461 7465 2860  pe` = validate(`
-00003980: 725f 6264 7360 2c20 6073 6967 6d61 7360  r_bds`, `sigmas`
-00003990: 2c20 606f 6d65 6761 7360 2c20 6062 6364  , `omegas`, `bcd
-000039a0: 6576 602c 2060 6173 796d 5f73 6861 7065  ev`, `asym_shape
-000039b0: 602c 2060 705f 6d61 7860 290a 2020 2020  `, `p_max`).    
-000039c0: 5265 7475 726e 733a 0a20 2020 2020 2020  Returns:.       
-000039d0: 2072 5f62 6473 3a20 666c 6f61 742c 2073   r_bds: float, s
-000039e0: 6861 7065 286e 5f62 6473 292e 0a20 2020  hape(n_bds)..   
-000039f0: 2020 2020 2073 6967 6d61 733a 2066 6c6f       sigmas: flo
-00003a00: 6174 2c20 7368 6170 6528 6e5f 6264 7329  at, shape(n_bds)
-00003a10: 2e0a 2020 2020 2020 2020 6f6d 6567 6173  ..        omegas
-00003a20: 3a20 666c 6f61 742c 2073 6861 7065 286e  : float, shape(n
-00003a30: 5f70 6561 6b73 292e 0a20 2020 2020 2020  _peaks)..       
-00003a40: 2061 7379 6d5f 7368 6170 653a 2063 6f6d   asym_shape: com
-00003a50: 706c 6578 2c20 7368 6170 6528 6e5f 6264  plex, shape(n_bd
-00003a60: 732c 322c 705f 6d61 782b 312c 705f 6d61  s,2,p_max+1,p_ma
-00003a70: 782b 3129 2e0a 2020 2020 5061 7261 6d65  x+1)..    Parame
-00003a80: 7465 7273 3a0a 2020 2020 2020 2020 725f  ters:.        r_
-00003a90: 6264 733a 2066 6c6f 6174 2c20 7368 6170  bds: float, shap
-00003aa0: 6528 6e5f 6264 7329 2e0a 2020 2020 2020  e(n_bds)..      
-00003ab0: 2020 7369 676d 6173 3a20 666c 6f61 742c    sigmas: float,
-00003ac0: 2073 6861 7065 286e 5f62 6473 292e 0a20   shape(n_bds).. 
-00003ad0: 2020 2020 2020 206f 6d65 6761 733a 2066         omegas: f
-00003ae0: 6c6f 6174 2c20 7368 6170 6528 6e5f 7065  loat, shape(n_pe
-00003af0: 616b 7329 2e0a 2020 2020 2020 2020 6263  aks)..        bc
-00003b00: 6465 763a 2066 6c6f 6174 2c20 7368 6170  dev: float, shap
-00003b10: 6528 6e5f 6264 7329 2e0a 2020 2020 2020  e(n_bds)..      
-00003b20: 2020 6173 796d 5f73 6861 7065 3a20 636f    asym_shape: co
-00003b30: 6d70 6c65 782c 2073 6861 7065 286e 5f62  mplex, shape(n_b
-00003b40: 6473 2c32 2c70 5f6d 6178 2b31 2c70 5f6d  ds,2,p_max+1,p_m
-00003b50: 6178 2b31 292e 0a20 2020 2020 2020 2070  ax+1)..        p
-00003b60: 5f6d 6178 3a20 696e 7465 6765 722e 0a20  _max: integer.. 
-00003b70: 2020 2022 2222 0a64 6566 2076 616c 6964     """.def valid
-00003b80: 6174 6528 725f 6264 732c 2073 6967 6d61  ate(r_bds, sigma
-00003b90: 732c 2062 6364 6576 2c20 6173 796d 5f73  s, bcdev, asym_s
-00003ba0: 6861 7065 2c20 705f 6d61 7829 3a0a 2020  hape, p_max):.  
-00003bb0: 2020 2320 4368 6563 6b20 6c65 6e67 7468    # Check length
-00003bc0: 7320 6f66 206d 6f64 656c 206c 6973 7473  s of model lists
-00003bd0: 0a20 2020 2069 6620 6e70 2e73 6861 7065  .    if np.shape
-00003be0: 2872 5f62 6473 2920 213d 206e 702e 7368  (r_bds) != np.sh
-00003bf0: 6170 6528 7369 676d 6173 293a 0a20 2020  ape(sigmas):.   
-00003c00: 2020 2020 206c 6f67 2e65 7272 6f72 2866       log.error(f
-00003c10: 2262 6f75 6e64 6172 6965 7320 7368 6170  "boundaries shap
-00003c20: 653a 207b 6e70 2e73 6861 7065 2872 5f62  e: {np.shape(r_b
-00003c30: 6473 297d 2229 0a20 2020 2020 2020 206c  ds)}").        l
-00003c40: 6f67 2e65 7272 6f72 2866 2273 6967 6d61  og.error(f"sigma
-00003c50: 7320 7368 6170 653a 207b 6e70 2e73 6861  s shape: {np.sha
-00003c60: 7065 2873 6967 6d61 7329 7d22 290a 2020  pe(sigmas)}").  
-00003c70: 2020 2020 2020 7261 6973 6520 5661 6c75        raise Valu
-00003c80: 6545 7272 6f72 2822 5468 6520 6e75 6d62  eError("The numb
-00003c90: 6572 206f 6620 626f 756e 6461 7269 6573  er of boundaries
-00003ca0: 2069 7320 6e6f 7420 6571 7561 6c20 746f   is not equal to
-00003cb0: 2074 6865 206e 756d 6265 7220 6f66 2063   the number of c
-00003cc0: 6f6e 6475 6374 6976 6974 6965 732e 2229  onductivities.")
-00003cd0: 0a20 2020 2069 6620 6e70 2e73 6861 7065  .    if np.shape
-00003ce0: 2872 5f62 6473 2920 213d 206e 702e 7368  (r_bds) != np.sh
-00003cf0: 6170 6528 6263 6465 7629 3a0a 2020 2020  ape(bcdev):.    
-00003d00: 2020 2020 6c6f 672e 6572 726f 7228 6622      log.error(f"
-00003d10: 626f 756e 6461 7269 6573 2073 6861 7065  boundaries shape
-00003d20: 3a20 7b6e 702e 7368 6170 6528 725f 6264  : {np.shape(r_bd
-00003d30: 7329 7d22 290a 2020 2020 2020 2020 6c6f  s)}").        lo
-00003d40: 672e 6572 726f 7228 6622 6465 7669 6174  g.error(f"deviat
-00003d50: 696f 6e73 2073 6861 7065 3a20 7b6e 702e  ions shape: {np.
-00003d60: 7368 6170 6528 6263 6465 7629 7d22 290a  shape(bcdev)}").
-00003d70: 2020 2020 2020 2020 7261 6973 6520 5661          raise Va
-00003d80: 6c75 6545 7272 6f72 2822 5468 6520 6e75  lueError("The nu
-00003d90: 6d62 6572 206f 6620 626f 756e 6461 7269  mber of boundari
-00003da0: 6573 2069 7320 6e6f 7420 6571 7561 6c20  es is not equal 
-00003db0: 746f 2074 6865 206e 756d 6265 7220 6f66  to the number of
-00003dc0: 2064 6576 6961 7469 6f6e 732e 2229 0a0a   deviations.")..
-00003dd0: 2020 2020 2320 4d61 6b65 2073 7572 6520      # Make sure 
-00003de0: 696e 7465 7269 6f72 206d 6f64 656c 2069  interior model i
-00003df0: 7320 6974 6572 6162 6c65 2028 6974 2773  s iterable (it's
-00003e00: 206e 6f74 2069 6620 7468 6572 6520 6973   not if there is
-00003e10: 206f 6e6c 7920 3120 626f 756e 6461 7279   only 1 boundary
-00003e20: 290a 2020 2020 6966 206e 6f74 2069 7369  ).    if not isi
-00003e30: 6e73 7461 6e63 6528 725f 6264 732c 2049  nstance(r_bds, I
-00003e40: 7465 7261 626c 6529 3a0a 2020 2020 2020  terable):.      
-00003e50: 2020 725f 6264 7320 3d20 5b72 5f62 6473    r_bds = [r_bds
-00003e60: 5d0a 2020 2020 2020 2020 7369 676d 6173  ].        sigmas
-00003e70: 203d 205b 7369 676d 6173 5d0a 2020 2020   = [sigmas].    
-00003e80: 2020 2020 6e70 2e72 6573 6861 7065 2861      np.reshape(a
-00003e90: 7379 6d5f 7368 6170 652c 2028 312c 322c  sym_shape, (1,2,
-00003ea0: 705f 6d61 782b 312c 705f 6d61 782b 3129  p_max+1,p_max+1)
-00003eb0: 290a 0a20 2020 2023 2044 6f75 626c 6520  )..    # Double 
-00003ec0: 6368 6563 6b20 6172 7261 7920 6c65 6e67  check array leng
-00003ed0: 7468 7320 616c 6c20 6d61 7463 6820 7570  ths all match up
-00003ee0: 0a20 2020 2069 6620 6e70 2e73 6861 7065  .    if np.shape
-00003ef0: 2861 7379 6d5f 7368 6170 6529 2021 3d20  (asym_shape) != 
-00003f00: 286e 702e 7369 7a65 2872 5f62 6473 292c  (np.size(r_bds),
-00003f10: 322c 705f 6d61 782b 312c 705f 6d61 782b  2,p_max+1,p_max+
-00003f20: 3129 3a0a 2020 2020 2020 2020 6966 206e  1):.        if n
-00003f30: 702e 7368 6170 6528 725f 6264 7329 2021  p.shape(r_bds) !
-00003f40: 3d20 6e70 2e73 6861 7065 2861 7379 6d5f  = np.shape(asym_
-00003f50: 7368 6170 6529 5b30 5d3a 0a20 2020 2020  shape)[0]:.     
-00003f60: 2020 2020 2020 206c 6f67 2e65 7272 6f72         log.error
-00003f70: 2866 2262 6f75 6e64 6172 6965 7320 6c65  (f"boundaries le
-00003f80: 6e67 7468 3a20 7b6e 702e 7368 6170 6528  ngth: {np.shape(
-00003f90: 725f 6264 7329 7d22 290a 2020 2020 2020  r_bds)}").      
-00003fa0: 2020 2020 2020 6c6f 672e 6572 726f 7228        log.error(
-00003fb0: 6622 6465 7669 6174 696f 6e73 206c 656e  f"deviations len
-00003fc0: 6774 683a 207b 6e70 2e73 6861 7065 2861  gth: {np.shape(a
-00003fd0: 7379 6d5f 7368 6170 6529 5b30 5d7d 2229  sym_shape)[0]}")
-00003fe0: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
-00003ff0: 7365 2056 616c 7565 4572 726f 7228 2254  se ValueError("T
-00004000: 6865 206e 756d 6265 7220 6f66 2062 6f75  he number of bou
-00004010: 6e64 6172 6965 7320 6973 206e 6f74 2065  ndaries is not e
-00004020: 7175 616c 2074 6f20 7468 6520 6e75 6d62  qual to the numb
-00004030: 6572 206f 6620 6465 7669 6174 696f 6e20  er of deviation 
-00004040: 7368 6170 6573 2e22 290a 2020 2020 2020  shapes.").      
-00004050: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-00004060: 2020 2020 7261 6973 6520 5661 6c75 6545      raise ValueE
-00004070: 7272 6f72 2822 5468 6520 6e75 6d62 6572  rror("The number
-00004080: 206f 6620 6465 7669 6174 696f 6e20 7368   of deviation sh
-00004090: 6170 6573 2069 7320 6e6f 7420 6571 7561  apes is not equa
-000040a0: 6c20 746f 2028 705f 6d61 7820 2b20 3129  l to (p_max + 1)
-000040b0: 5e32 202d 2031 2e22 290a 0a20 2020 2072  ^2 - 1.")..    r
-000040c0: 6574 7572 6e20 725f 6264 732c 2073 6967  eturn r_bds, sig
-000040d0: 6d61 732c 2061 7379 6d5f 7368 6170 650a  mas, asym_shape.
-000040e0: 0a23 2323 2323 2323 2323 2323 2323 2323  .###############
-000040f0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00004100: 2323 2323 2323 2323 2323 2323 2323 0a0a  ##############..
-00004110: 2222 220a 6a6e 7828 292c 2079 6e78 2829  """.jnx(), ynx()
-00004120: 2c20 6a64 7828 292c 2079 6478 2829 0a20  , jdx(), ydx(). 
-00004130: 2020 2053 7068 6572 6963 616c 2042 6573     Spherical Bes
-00004140: 7365 6c20 616e 6420 4e65 756d 616e 6e20  sel and Neumann 
-00004150: 6675 6e63 7469 6f6e 7320 666f 7220 6465  functions for de
-00004160: 6772 6565 206e 2061 6e64 2061 7267 756d  gree n and argum
-00004170: 656e 7420 782e 0a20 2020 206a 6478 2061  ent x..    jdx a
-00004180: 6e64 2079 6478 2061 7265 206a 5f6e 5e5c  nd ydx are j_n^\
-00004190: 7374 6172 2061 6e64 2079 5f6e 5e5c 7374  star and y_n^\st
-000041a0: 6172 2069 6e20 7468 6520 6162 6f76 6520  ar in the above 
-000041b0: 7075 626c 6963 6174 696f 6e2c 2061 6e64  publication, and
-000041c0: 2061 7265 0a20 2020 2065 7175 616c 2074   are.    equal t
-000041d0: 6f20 6428 722a 6a6e 7828 6b72 2929 2f64  o d(r*jnx(kr))/d
-000041e0: 7220 616e 6420 6428 722a 796e 7828 6b72  r and d(r*ynx(kr
-000041f0: 2929 2f64 722c 2072 6573 7065 6374 6976  ))/dr, respectiv
-00004200: 656c 792e 0a20 2020 2055 7361 6765 3a20  ely..    Usage: 
-00004210: 6065 7661 6c60 203d 206a 6e78 2860 6e60  `eval` = jnx(`n`
-00004220: 2c20 6078 6029 0a20 2020 2052 6574 7572  , `x`).    Retur
-00004230: 6e73 3a0a 2020 2020 2020 2020 6576 616c  ns:.        eval
-00004240: 3a20 6d70 632c 2073 6861 7065 286c 656e  : mpc, shape(len
-00004250: 2878 2929 2e20 4c69 7374 206f 6620 7265  (x)). List of re
-00004260: 7375 6c74 7320 6f66 2042 6573 7365 6c20  sults of Bessel 
-00004270: 6675 6e63 7469 6f6e 7320 696e 206d 706d  functions in mpm
-00004280: 6174 6820 636f 6d70 6c65 7820 286d 7063  ath complex (mpc
-00004290: 2920 666f 726d 6174 2e20 416c 7761 7973  ) format. Always
-000042a0: 2072 6574 7572 6e73 2061 6e20 6172 7261   returns an arra
-000042b0: 792c 2070 6f73 7369 626c 7920 6f66 206c  y, possibly of l
-000042c0: 656e 6774 6820 312e 0a20 2020 2050 6172  ength 1..    Par
-000042d0: 616d 6574 6572 733a 0a20 2020 2020 2020  ameters:.       
-000042e0: 206e 3a20 6d70 662e 2044 6567 7265 6520   n: mpf. Degree 
-000042f0: 6f66 2073 7068 6572 6963 616c 2042 6573  of spherical Bes
-00004300: 7365 6c20 6675 6e63 7469 6f6e 2e20 5368  sel function. Sh
-00004310: 6f75 6c64 2062 6520 616e 2069 6e74 6567  ould be an integ
-00004320: 6572 2c20 6465 7370 6974 6520 6265 696e  er, despite bein
-00004330: 6720 6f66 206d 7066 2074 7970 6520 286d  g of mpf type (m
-00004340: 7573 7420 6265 2070 6173 7365 6420 6173  ust be passed as
-00004350: 2068 616c 662d 696e 7465 6765 7220 6f72   half-integer or
-00004360: 6465 7220 746f 2062 6573 7365 6c6a 292e  der to besselj).
-00004370: 0a20 2020 2020 2020 2078 3a20 6d70 632c  .        x: mpc,
-00004380: 2073 6861 7065 286e 5f62 6473 292e 2043   shape(n_bds). C
-00004390: 6f6d 706c 6578 2061 7267 756d 656e 7420  omplex argument 
-000043a0: 6f66 2042 6573 7365 6c20 6675 6e63 7469  of Bessel functi
-000043b0: 6f6e 2028 6b72 292e 204d 5553 5420 6265  on (kr). MUST be
-000043c0: 2061 206c 6973 7420 6f72 2074 6869 7320   a list or this 
-000043d0: 7769 6c6c 2062 7265 616b 2e20 4d61 6b65  will break. Make
-000043e0: 2073 696e 676c 6520 7661 6c75 6573 2069   single values i
-000043f0: 6e74 6f20 6c69 7374 7320 7769 7468 2078  nto lists with x
-00004400: 203d 205b 785d 2e0a 2020 2020 2222 220a   = [x]..    """.
-00004410: 6465 6620 6a6e 7828 6e2c 7829 3a0a 2020  def jnx(n,x):.  
-00004420: 2020 7477 6f20 3d20 6d70 2e6d 7066 2832    two = mp.mpf(2
-00004430: 290a 2020 2020 6a6e 7820 3d20 6e70 2e61  ).    jnx = np.a
-00004440: 7272 6179 285b 206d 702e 6265 7373 656c  rray([ mp.bessel
-00004450: 6a28 206e 2b6d 702e 6d70 6628 2230 2e35  j( n+mp.mpf("0.5
-00004460: 2229 2c78 6920 2920 2a20 6d70 2e73 7172  "),xi ) * mp.sqr
-00004470: 7428 6d70 2e70 692f 7477 6f2f 7869 2920  t(mp.pi/two/xi) 
-00004480: 666f 7220 7869 2069 6e20 7820 5d29 0a20  for xi in x ]). 
-00004490: 2020 2072 6574 7572 6e20 6a6e 780a 6465     return jnx.de
-000044a0: 6620 796e 7828 6e2c 7829 3a0a 2020 2020  f ynx(n,x):.    
-000044b0: 7477 6f20 3d20 6d70 2e6d 7066 2832 290a  two = mp.mpf(2).
-000044c0: 2020 2020 796e 7820 3d20 6e70 2e61 7272      ynx = np.arr
-000044d0: 6179 285b 206d 702e 6265 7373 656c 7928  ay([ mp.bessely(
-000044e0: 206e 2b6d 702e 6d70 6628 2230 2e35 2229   n+mp.mpf("0.5")
-000044f0: 2c78 6920 2920 2a20 6d70 2e73 7172 7428  ,xi ) * mp.sqrt(
-00004500: 6d70 2e70 692f 7477 6f2f 7869 2920 666f  mp.pi/two/xi) fo
-00004510: 7220 7869 2069 6e20 7820 5d29 0a20 2020  r xi in x ]).   
-00004520: 2072 6574 7572 6e20 796e 780a 6465 6620   return ynx.def 
-00004530: 6a64 7828 6e2c 7829 3a0a 2020 2020 6f6e  jdx(n,x):.    on
-00004540: 6520 3d20 6d70 2e6d 7066 2831 290a 2020  e = mp.mpf(1).  
-00004550: 2020 6a6e 203d 206a 6e78 286e 2c78 290a    jn = jnx(n,x).
-00004560: 2020 2020 6a50 203d 206a 6e78 286e 2b6f      jP = jnx(n+o
-00004570: 6e65 2c78 290a 2020 2020 6a64 7820 3d20  ne,x).    jdx = 
-00004580: 6e70 2e61 7272 6179 285b 2028 6e2b 6f6e  np.array([ (n+on
-00004590: 6529 2a6a 6e5b 695d 202d 2078 5b69 5d2a  e)*jn[i] - x[i]*
-000045a0: 6a50 5b69 5d20 666f 7220 6920 696e 2072  jP[i] for i in r
-000045b0: 616e 6765 286e 702e 7369 7a65 2878 2929  ange(np.size(x))
-000045c0: 205d 290a 2020 2020 7265 7475 726e 206a   ]).    return j
-000045d0: 6478 0a64 6566 2079 6478 286e 2c78 293a  dx.def ydx(n,x):
-000045e0: 0a20 2020 206f 6e65 203d 206d 702e 6d70  .    one = mp.mp
-000045f0: 6628 3129 0a20 2020 2079 6e20 3d20 796e  f(1).    yn = yn
-00004600: 7828 6e2c 7829 0a20 2020 2079 5020 3d20  x(n,x).    yP = 
-00004610: 796e 7828 6e2b 6f6e 652c 7829 0a20 2020  ynx(n+one,x).   
-00004620: 2079 6478 203d 206e 702e 6172 7261 7928   ydx = np.array(
-00004630: 5b20 286e 2b6f 6e65 292a 796e 5b69 5d20  [ (n+one)*yn[i] 
-00004640: 2d20 785b 695d 2a79 505b 695d 2066 6f72  - x[i]*yP[i] for
-00004650: 2069 2069 6e20 7261 6e67 6528 6e70 2e73   i in range(np.s
-00004660: 697a 6528 7829 2920 5d29 0a20 2020 2072  ize(x)) ]).    r
-00004670: 6574 7572 6e20 7964 780a 0a23 2323 2323  eturn ydx..#####
-00004680: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00004690: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000046a0: 2323 2323 2323 2323 0a0a 2222 220a 7265  ########..""".re
-000046b0: 6164 5f42 656e 6d28 290a 2020 2020 5265  ad_Benm().    Re
-000046c0: 6164 2069 6e20 7468 6520 636f 6d70 6c65  ad in the comple
-000046d0: 7820 6672 6571 7565 6e63 7920 7370 6563  x frequency spec
-000046e0: 7472 756d 206f 6620 6578 6369 7461 7469  trum of excitati
-000046f0: 6f6e 2066 6965 6c64 206f 7363 696c 6c61  on field oscilla
-00004700: 7469 6f6e 7320 666f 7220 7468 6520 7374  tions for the st
-00004710: 726f 6e67 6573 7420 6578 6369 7461 7469  rongest excitati
-00004720: 6f6e 732e 0a20 2020 2055 7361 6765 3a20  ons..    Usage: 
-00004730: 6070 6561 6b5f 7065 7269 6f64 7360 2c20  `peak_periods`, 
-00004740: 6042 656e 6d60 203d 2072 6561 645f 4265  `Benm` = read_Be
-00004750: 6e6d 2860 6e70 726d 5f6d 6178 602c 2060  nm(`nprm_max`, `
-00004760: 705f 6d61 7860 2c20 6062 6f64 796e 616d  p_max`, `bodynam
-00004770: 653d 4e6f 6e65 602c 2060 6670 6174 683d  e=None`, `fpath=
-00004780: 4e6f 6e65 602c 2060 7379 6e6f 6469 633d  None`, `synodic=
-00004790: 4661 6c73 6560 2c20 606f 7262 6974 616c  False`, `orbital
-000047a0: 3d46 616c 7365 6029 0a20 2020 2052 6574  =False`).    Ret
-000047b0: 7572 6e73 3a0a 2020 2020 2020 2020 7065  urns:.        pe
-000047c0: 616b 5f70 6572 696f 6473 3a20 666c 6f61  ak_periods: floa
-000047d0: 742c 2073 6861 7065 286e 5f70 6561 6b73  t, shape(n_peaks
-000047e0: 292e 2050 6572 696f 6473 2069 6e20 6872  ). Periods in hr
-000047f0: 206f 6620 7065 616b 206f 7363 696c 6c61   of peak oscilla
-00004800: 7469 6f6e 732e 2056 616c 7565 7320 7265  tions. Values re
-00004810: 6164 2066 726f 6d20 6669 6c65 7320 6172  ad from files ar
-00004820: 6520 6173 7375 6d65 6420 746f 2062 6520  e assumed to be 
-00004830: 696e 2068 722e 0a20 2020 2020 2020 2042  in hr..        B
-00004840: 656e 6d3a 2063 6f6d 706c 6578 2c20 7368  enm: complex, sh
-00004850: 6170 6528 6e5f 7065 616b 732c 322c 6e70  ape(n_peaks,2,np
-00004860: 726d 5f6d 6178 2b70 5f6d 6178 2b31 2c6e  rm_max+p_max+1,n
-00004870: 7072 6d5f 6d61 782b 705f 6d61 782b 3129  prm_max+p_max+1)
-00004880: 2e20 4578 6369 7461 7469 6f6e 206d 6f6d  . Excitation mom
-00004890: 656e 7473 2066 6f72 2065 6163 6820 7065  ents for each pe
-000048a0: 7269 6f64 2069 6e20 6e54 2e0a 2020 2020  riod in nT..    
-000048b0: 2020 2020 4230 3a20 666c 6f61 742c 2073      B0: float, s
-000048c0: 6861 7065 2833 292e 2053 7461 7469 6320  hape(3). Static 
-000048d0: 6261 636b 6772 6f75 6e64 2066 6965 6c64  background field
-000048e0: 2e20 5573 6564 2074 6f20 7265 636f 6e73  . Used to recons
-000048f0: 7472 7563 7420 7468 6520 6e65 7420 6d61  truct the net ma
-00004900: 676e 6574 6963 2066 6965 6c64 2066 6f72  gnetic field for
-00004910: 206d 6561 7375 7265 6d65 6e74 2063 6f6d   measurement com
-00004920: 7061 7269 736f 6e73 2e0a 2020 2020 5061  parisons..    Pa
-00004930: 7261 6d65 7465 7273 3a0a 2020 2020 2020  rameters:.      
-00004940: 2020 6e70 726d 5f6d 6178 3a20 696e 7465    nprm_max: inte
-00004950: 6765 722e 204d 6178 696d 756d 2064 6567  ger. Maximum deg
-00004960: 7265 6520 6f66 2065 7863 6974 6174 696f  ree of excitatio
-00004970: 6e20 6861 726d 6f6e 6963 7320 746f 2069  n harmonics to i
-00004980: 6e70 7574 2e20 6e27 2076 616c 7565 7320  nput. n' values 
-00004990: 6170 7065 6172 2069 6e20 6669 6c65 206e  appear in file n
-000049a0: 616d 6573 2c20 736f 2061 7070 726f 7072  ames, so appropr
-000049b0: 6961 7465 2066 696c 6573 206d 7573 740a  iate files must.
-000049c0: 2020 2020 2020 2020 2020 2020 616c 6c20              all 
-000049d0: 6265 2070 7265 7365 6e74 2066 726f 6d20  be present from 
-000049e0: 6e27 3d31 2074 6f20 6e27 3d6e 7072 6d5f  n'=1 to n'=nprm_
-000049f0: 6d61 782e 0a20 2020 2020 2020 2070 5f6d  max..        p_m
-00004a00: 6178 3a20 696e 7465 6765 722e 204d 6178  ax: integer. Max
-00004a10: 696d 756d 2064 6567 7265 6520 6f66 2062  imum degree of b
-00004a20: 6f75 6e64 6172 7920 7368 6170 6573 2e20  oundary shapes. 
-00004a30: 5265 7175 6972 6564 2074 6f20 7369 7a65  Required to size
-00004a40: 2042 656e 6d20 6172 7261 7920 636f 7272   Benm array corr
-00004a50: 6563 746c 7920 666f 7220 6661 7374 2063  ectly for fast c
-00004a60: 6f6d 7075 7461 7469 6f6e 206f 6620 626f  omputation of bo
-00004a70: 756e 6461 7279 2063 6f6e 6469 7469 6f6e  undary condition
-00004a80: 732e 0a20 2020 2020 2020 2062 6f64 796e  s..        bodyn
-00004a90: 616d 653a 2073 7472 696e 6720 284e 6f6e  ame: string (Non
-00004aa0: 6529 2e20 426f 6479 206e 616d 6520 6173  e). Body name as
-00004ab0: 2069 7420 6170 7065 6172 7320 696e 2066   it appears in f
-00004ac0: 696c 6520 6e61 6d65 732e 2049 6620 4e6f  ile names. If No
-00004ad0: 6e65 2c20 6120 6765 6e65 7269 6320 6669  ne, a generic fi
-00004ae0: 6c65 206e 616d 6520 7769 6c6c 2062 6520  le name will be 
-00004af0: 7365 6172 6368 6564 2066 6f72 2e0a 2020  searched for..  
-00004b00: 2020 2020 2020 6670 6174 683a 2073 7472        fpath: str
-00004b10: 696e 6720 284e 6f6e 6529 2e20 4f70 7469  ing (None). Opti
-00004b20: 6f6e 616c 206c 6f63 6174 696f 6e20 746f  onal location to
-00004b30: 2073 6561 7263 6820 666f 7220 6578 6369   search for exci
-00004b40: 7461 7469 6f6e 206d 6f6d 656e 7420 6669  tation moment fi
-00004b50: 6c65 732e 2044 6566 6175 6c74 7320 746f  les. Defaults to
-00004b60: 2022 6578 6369 7461 7469 6f6e 2f22 2e0a   "excitation/"..
-00004b70: 2020 2020 2020 2020 7379 6e6f 6469 633a          synodic:
-00004b80: 2062 6f6f 6c65 616e 2028 4661 6c73 6529   boolean (False)
-00004b90: 2e20 4f70 7469 6f6e 2074 6f20 636f 6e73  . Option to cons
-00004ba0: 6964 6572 206f 6e6c 7920 7468 6520 7374  ider only the st
-00004bb0: 726f 6e67 6573 7420 6578 6369 7461 7469  rongest excitati
-00004bc0: 6f6e 2070 6572 696f 642c 2066 6f72 2073  on period, for s
-00004bd0: 696d 706c 6963 6974 792e 0a20 2020 2020  implicity..     
-00004be0: 2020 206f 7262 6974 616c 3a20 626f 6f6c     orbital: bool
-00004bf0: 6561 6e20 2846 616c 7365 292e 204f 7074  ean (False). Opt
-00004c00: 696f 6e20 746f 2063 6f6e 7369 6465 7220  ion to consider 
-00004c10: 6f6e 6c79 2074 6865 206f 7262 6974 616c  only the orbital
-00004c20: 2070 6572 696f 642c 2061 6e61 6c6f 676f   period, analogo
-00004c30: 7573 2074 6f20 7468 6520 7379 6e6f 6469  us to the synodi
-00004c40: 6320 7065 7269 6f64 2061 626f 7665 2e0a  c period above..
-00004c50: 2020 2020 2020 2020 6c69 6d69 745f 6f73          limit_os
-00004c60: 633a 2069 6e74 6567 6572 2028 4e6f 6e65  c: integer (None
-00004c70: 292e 204e 756d 6265 7220 6f66 206f 7363  ). Number of osc
-00004c80: 696c 6c61 7469 6f6e 2066 7265 7175 656e  illation frequen
-00004c90: 6369 6573 2074 6f20 6c69 6d69 7420 6361  cies to limit ca
-00004ca0: 6c63 756c 6174 696f 6e73 2074 6f2c 2077  lculations to, w
-00004cb0: 6865 7265 2031 2069 7320 6a75 7374 2074  here 1 is just t
-00004cc0: 6865 2073 7472 6f6e 6765 7374 206f 7363  he strongest osc
-00004cd0: 696c 6c61 7469 6f6e 2e0a 2020 2020 2020  illation..      
-00004ce0: 2020 6d6f 6465 6c3a 2073 7472 696e 6720    model: string 
-00004cf0: 284e 6f6e 6529 2e20 4f70 7469 6f6e 616c  (None). Optional
-00004d00: 206d 6f64 656c 2063 6f64 6520 746f 2061   model code to a
-00004d10: 7070 656e 6420 746f 2066 696c 6520 6e61  ppend to file na
-00004d20: 6d65 2e0a 2020 2020 2020 2020 664e 616d  me..        fNam
-00004d30: 653a 2073 7472 696e 6720 284e 6f6e 6529  e: string (None)
-00004d40: 2e20 4f70 7469 6f6e 616c 206f 7665 7272  . Optional overr
-00004d50: 6964 6520 6f66 206e 616d 696e 6720 636f  ide of naming co
-00004d60: 6e76 656e 7469 6f6e 7320 746f 2073 7065  nventions to spe
-00004d70: 6369 6679 2066 696c 656e 616d 652e 2020  cify filename.  
-00004d80: 0a20 2020 2022 2222 0a64 6566 2072 6561  .    """.def rea
-00004d90: 645f 4265 6e6d 286e 7072 6d5f 6d61 782c  d_Benm(nprm_max,
-00004da0: 2070 5f6d 6178 2c20 626f 6479 6e61 6d65   p_max, bodyname
-00004db0: 3d4e 6f6e 652c 2066 7061 7468 3d4e 6f6e  =None, fpath=Non
-00004dc0: 652c 2073 796e 6f64 6963 3d46 616c 7365  e, synodic=False
-00004dd0: 2c20 6f72 6269 7461 6c3d 4661 6c73 652c  , orbital=False,
-00004de0: 206c 696d 6974 5f6f 7363 3d4e 6f6e 652c   limit_osc=None,
-00004df0: 0a20 2020 2020 2020 2020 2020 2020 206d  .              m
-00004e00: 6f64 656c 3d4e 6f6e 652c 2066 4e61 6d65  odel=None, fName
-00004e10: 3d4e 6f6e 6529 3a0a 2020 2020 6966 2066  =None):.    if f
-00004e20: 7061 7468 2069 7320 4e6f 6e65 3a0a 2020  path is None:.  
-00004e30: 2020 2020 2020 6670 6174 6820 3d20 5f65        fpath = _e
-00004e40: 7863 6974 6174 696f 6e0a 2020 2020 6966  xcitation.    if
-00004e50: 206d 6f64 656c 2069 7320 4e6f 6e65 3a0a   model is None:.
-00004e60: 2020 2020 2020 2020 6d6f 6465 6c53 7472          modelStr
-00004e70: 203d 2022 220a 2020 2020 656c 7365 3a0a   = "".    else:.
-00004e80: 2020 2020 2020 2020 6d6f 6465 6c53 7472          modelStr
-00004e90: 203d 2066 225f 7b6d 6f64 656c 7d22 0a20   = f"_{model}". 
-00004ea0: 2020 2069 6620 626f 6479 6e61 6d65 2069     if bodyname i
-00004eb0: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
-00004ec0: 6266 6e61 6d65 203d 2066 227b 6d6f 6465  bfname = f"{mode
-00004ed0: 6c53 7472 7d22 0a20 2020 2065 6c73 653a  lStr}".    else:
-00004ee0: 0a20 2020 2020 2020 2062 666e 616d 6520  .        bfname 
-00004ef0: 3d20 6622 5f7b 626f 6479 6e61 6d65 7d7b  = f"_{bodyname}{
-00004f00: 6d6f 6465 6c53 7472 7d22 0a0a 2020 2020  modelStr}"..    
-00004f10: 6966 2073 796e 6f64 6963 2061 6e64 206f  if synodic and o
-00004f20: 7262 6974 616c 3a0a 2020 2020 2020 2020  rbital:.        
-00004f30: 6c6f 672e 7761 726e 696e 6728 2242 6f74  log.warning("Bot
-00004f40: 6820 2773 796e 6f64 6963 2720 616e 6420  h 'synodic' and 
-00004f50: 276f 7262 6974 616c 2720 6f70 7469 6f6e  'orbital' option
-00004f60: 7320 7061 7373 6564 2074 6f20 6173 796d  s passed to asym
-00004f70: 6d65 7472 795f 6675 6e63 732e 7265 6164  metry_funcs.read
-00004f80: 5f42 656e 6d2e 204f 6e6c 7920 7379 6e6f  _Benm. Only syno
-00004f90: 6469 6320 7769 6c6c 2062 6520 7573 6564  dic will be used
-00004fa0: 2e22 290a 2020 2020 2020 2020 6f72 6269  .").        orbi
-00004fb0: 7461 6c20 3d20 4661 6c73 650a 0a20 2020  tal = False..   
-00004fc0: 2069 6620 7379 6e6f 6469 633a 0a20 2020   if synodic:.   
-00004fd0: 2020 2020 206c 6f67 2e77 6172 6e69 6e67       log.warning
-00004fe0: 2822 436f 6e73 6964 6572 696e 6720 7379  ("Considering sy
-00004ff0: 6e6f 6469 6320 7065 7269 6f64 206f 6e6c  nodic period onl
-00005000: 7920 666f 7220 6578 6369 7461 7469 6f6e  y for excitation
-00005010: 2e22 290a 2020 2020 2020 2020 6966 2066  .").        if f
-00005020: 4e61 6d65 2069 7320 4e6f 6e65 3a0a 2020  Name is None:.  
-00005030: 2020 2020 2020 2020 2020 4265 6e6d 5f6d            Benm_m
-00005040: 6f6d 656e 7473 203d 206f 732e 7061 7468  oments = os.path
-00005050: 2e6a 6f69 6e28 6670 6174 682c 2066 2273  .join(fpath, f"s
-00005060: 796e 6f64 6963 5f42 6531 7879 7a7b 6266  ynodic_Be1xyz{bf
-00005070: 6e61 6d65 7d2e 7478 7422 290a 2020 2020  name}.txt").    
-00005080: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00005090: 2020 2020 2020 6c69 6d69 745f 6f73 6320        limit_osc 
-000050a0: 3d20 310a 2020 2020 2020 2020 2020 2020  = 1.            
-000050b0: 4265 6e6d 5f6d 6f6d 656e 7473 203d 206f  Benm_moments = o
-000050c0: 732e 7061 7468 2e6a 6f69 6e28 6670 6174  s.path.join(fpat
-000050d0: 682c 2066 227b 664e 616d 657d 2e74 7874  h, f"{fName}.txt
-000050e0: 2229 0a20 2020 2065 6c69 6620 6f72 6269  ").    elif orbi
-000050f0: 7461 6c3a 0a20 2020 2020 2020 206c 6f67  tal:.        log
-00005100: 2e77 6172 6e69 6e67 2822 436f 6e73 6964  .warning("Consid
-00005110: 6572 696e 6720 6f72 6269 7461 6c20 7065  ering orbital pe
-00005120: 7269 6f64 206f 6e6c 7920 666f 7220 6578  riod only for ex
-00005130: 6369 7461 7469 6f6e 2e22 290a 2020 2020  citation.").    
-00005140: 2020 2020 6966 2062 6f64 796e 616d 6520      if bodyname 
-00005150: 3d3d 2022 4575 726f 7061 223a 0a20 2020  == "Europa":.   
-00005160: 2020 2020 2020 2020 206c 6f67 2e77 6172           log.war
-00005170: 6e69 6e67 2822 4578 7472 6120 7761 726e  ning("Extra warn
-00005180: 696e 673a 2054 6869 7320 6578 6369 7461  ing: This excita
-00005190: 7469 6f6e 2069 7320 4150 5052 4f58 494d  tion is APPROXIM
-000051a0: 4154 452c 2069 6e20 7468 6174 2074 776f  ATE, in that two
-000051b0: 2063 6c6f 7365 6c79 2d73 7061 6365 6420   closely-spaced 
-000051c0: 7065 7269 6f64 7320 6861 7665 2062 6565  periods have bee
-000051d0: 6e20 7375 6d6d 6564 2074 6f67 6574 6865  n summed togethe
-000051e0: 7220 616e 6420 7365 7420 746f 2054 203d  r and set to T =
-000051f0: 2038 352e 3220 682e 2229 0a20 2020 2020   85.2 h.").     
-00005200: 2020 2042 656e 6d5f 6d6f 6d65 6e74 7320     Benm_moments 
-00005210: 3d20 6f73 2e70 6174 682e 6a6f 696e 2866  = os.path.join(f
-00005220: 7061 7468 2c20 6622 6f72 6269 7461 6c5f  path, f"orbital_
-00005230: 4265 3178 797a 7b62 666e 616d 657d 2e74  Be1xyz{bfname}.t
-00005240: 7874 2229 0a20 2020 2065 6c73 653a 0a20  xt").    else:. 
-00005250: 2020 2020 2020 2069 6620 664e 616d 6520         if fName 
-00005260: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
-00005270: 2020 2020 2066 4e61 6d65 203d 2066 2742       fName = f'B
-00005280: 6531 7879 7a7b 6266 6e61 6d65 7d27 0a20  e1xyz{bfname}'. 
-00005290: 2020 2020 2020 2042 656e 6d5f 6d6f 6d65         Benm_mome
-000052a0: 6e74 7320 3d20 6f73 2e70 6174 682e 6a6f  nts = os.path.jo
-000052b0: 696e 2866 7061 7468 2c20 6622 7b66 4e61  in(fpath, f"{fNa
-000052c0: 6d65 7d2e 7478 7422 290a 2020 2020 6c6f  me}.txt").    lo
-000052d0: 672e 6465 6275 6728 6622 5573 696e 6720  g.debug(f"Using 
-000052e0: 6578 6369 7461 7469 6f6e 206d 6f6d 656e  excitation momen
-000052f0: 7473 3a20 7b42 656e 6d5f 6d6f 6d65 6e74  ts: {Benm_moment
-00005300: 737d 2229 0a20 2020 2070 6561 6b5f 7065  s}").    peak_pe
-00005310: 7231 2c20 4230 782c 2042 3079 2c20 4230  r1, B0x, B0y, B0
-00005320: 7a2c 2042 6578 5f52 652c 2042 6578 5f49  z, Bex_Re, Bex_I
-00005330: 6d2c 2042 6579 5f52 652c 2042 6579 5f49  m, Bey_Re, Bey_I
-00005340: 6d2c 2042 657a 5f52 652c 2042 657a 5f49  m, Bez_Re, Bez_I
-00005350: 6d20 3d20 6e70 2e6c 6f61 6474 7874 2842  m = np.loadtxt(B
-00005360: 656e 6d5f 6d6f 6d65 6e74 732c 2073 6b69  enm_moments, ski
-00005370: 7072 6f77 733d 312c 2075 6e70 6163 6b3d  prows=1, unpack=
-00005380: 5472 7565 2c20 6465 6c69 6d69 7465 723d  True, delimiter=
-00005390: 272c 2729 0a20 2020 206e 5f70 6561 6b73  ',').    n_peaks
-000053a0: 315f 7072 656c 696d 203d 2070 6561 6b5f  1_prelim = peak_
-000053b0: 7065 7231 2e73 697a 650a 0a20 2020 2042  per1.size..    B
-000053c0: 6578 203d 2042 6578 5f52 6520 2b20 316a  ex = Bex_Re + 1j
-000053d0: 202a 2042 6578 5f49 6d0a 2020 2020 4265   * Bex_Im.    Be
-000053e0: 7920 3d20 4265 795f 5265 202b 2031 6a20  y = Bey_Re + 1j 
-000053f0: 2a20 4265 795f 496d 0a20 2020 2042 657a  * Bey_Im.    Bez
-00005400: 203d 2042 657a 5f52 6520 2b20 316a 202a   = Bez_Re + 1j *
-00005410: 2042 657a 5f49 6d0a 0a20 2020 2069 6620   Bez_Im..    if 
-00005420: 6c69 6d69 745f 6f73 6320 6973 204e 6f6e  limit_osc is Non
-00005430: 653a 0a20 2020 2020 2020 206c 696d 6974  e:.        limit
-00005440: 5f6f 7363 203d 2030 0a20 2020 2065 6c69  _osc = 0.    eli
-00005450: 6620 6c69 6d69 745f 6f73 6320 213d 2030  f limit_osc != 0
-00005460: 3a0a 2020 2020 2020 2020 6966 206e 5f70  :.        if n_p
-00005470: 6561 6b73 315f 7072 656c 696d 203c 3d20  eaks1_prelim <= 
-00005480: 6c69 6d69 745f 6f73 633a 0a20 2020 2020  limit_osc:.     
-00005490: 2020 2020 2020 206c 6f67 2e64 6562 7567         log.debug
-000054a0: 2866 226c 696d 6974 5f6f 7363 2069 7320  (f"limit_osc is 
-000054b0: 7365 7420 746f 207b 6c69 6d69 745f 6f73  set to {limit_os
-000054c0: 637d 2c20 6275 7420 7b42 656e 6d5f 6d6f  c}, but {Benm_mo
-000054d0: 6d65 6e74 737d 2063 6f6e 7461 696e 7320  ments} contains 
-000054e0: 6f6e 6c79 207b 6e5f 7065 616b 7331 5f70  only {n_peaks1_p
-000054f0: 7265 6c69 6d7d 206f 7363 696c 6c61 7469  relim} oscillati
-00005500: 6f6e 2070 6572 696f 6473 2e20 496e 636c  on periods. Incl
-00005510: 7564 696e 6720 616c 6c20 6f73 6369 6c6c  uding all oscill
-00005520: 6174 696f 6e73 2069 6e20 6361 6c63 756c  ations in calcul
-00005530: 6174 696f 6e73 2e22 290a 2020 2020 2020  ations.").      
-00005540: 2020 2020 2020 6c69 6d69 745f 6f73 6320        limit_osc 
-00005550: 3d20 300a 2020 2020 2020 2020 656c 7365  = 0.        else
-00005560: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
-00005570: 206c 696d 6974 5f6f 7363 203c 2030 3a20   limit_osc < 0: 
-00005580: 6c69 6d69 745f 6f73 6320 3d20 6162 7328  limit_osc = abs(
-00005590: 6c69 6d69 745f 6f73 6329 0a20 2020 2020  limit_osc).     
-000055a0: 2020 2020 2020 206c 6f67 2e64 6562 7567         log.debug
-000055b0: 2866 224c 696d 6974 696e 6720 4265 6e6d  (f"Limiting Benm
-000055c0: 2074 6f20 7374 726f 6e67 6573 7420 7b6c   to strongest {l
-000055d0: 696d 6974 5f6f 7363 7d20 6f73 6369 6c6c  imit_osc} oscill
-000055e0: 6174 696f 6e73 2e22 290a 2020 2020 6162  ations.").    ab
-000055f0: 7342 656e 6d20 3d20 6e70 2e73 7172 7428  sBenm = np.sqrt(
-00005600: 4265 785f 5265 2a2a 3220 2b20 4265 785f  Bex_Re**2 + Bex_
-00005610: 496d 2a2a 3220 2b20 4265 795f 5265 2a2a  Im**2 + Bey_Re**
-00005620: 3220 2b20 4265 795f 496d 2a2a 3220 2b20  2 + Bey_Im**2 + 
-00005630: 4265 7a5f 5265 2a2a 3220 2b20 4265 7a5f  Bez_Re**2 + Bez_
-00005640: 496d 2a2a 3229 0a20 2020 2069 6620 7379  Im**2).    if sy
-00005650: 6e6f 6469 6320 6f72 206f 7262 6974 616c  nodic or orbital
-00005660: 3a0a 2020 2020 2020 2020 694d 6178 536f  :.        iMaxSo
-00005670: 7274 203d 2030 0a20 2020 2065 6c73 653a  rt = 0.    else:
-00005680: 0a20 2020 2020 2020 2069 4d61 7820 3d20  .        iMax = 
-00005690: 6e70 2e61 7267 7061 7274 6974 696f 6e28  np.argpartition(
-000056a0: 6162 7342 656e 6d2c 202d 6c69 6d69 745f  absBenm, -limit_
-000056b0: 6f73 6329 5b2d 6c69 6d69 745f 6f73 633a  osc)[-limit_osc:
-000056c0: 5d0a 2020 2020 2020 2020 7065 616b 5f70  ].        peak_p
-000056d0: 6572 315f 6c69 6d20 3d20 6e70 2e73 6f72  er1_lim = np.sor
-000056e0: 7428 7065 616b 5f70 6572 315b 694d 6178  t(peak_per1[iMax
-000056f0: 5d29 0a20 2020 2020 2020 2069 4d61 7853  ]).        iMaxS
-00005700: 6f72 7420 3d20 6e70 2e61 7272 6179 285b  ort = np.array([
-00005710: 6e70 2e61 7267 7768 6572 6528 7065 616b  np.argwhere(peak
-00005720: 5f70 6572 3120 3d3d 2070 6561 6b5f 7065  _per1 == peak_pe
-00005730: 7231 5f6c 696d 5b69 5d29 2066 6f72 2069  r1_lim[i]) for i
-00005740: 2069 6e20 7261 6e67 6528 6e70 2e73 697a   in range(np.siz
-00005750: 6528 7065 616b 5f70 6572 315f 6c69 6d29  e(peak_per1_lim)
-00005760: 295d 292e 666c 6174 7465 6e28 290a 0a20  )]).flatten().. 
-00005770: 2020 2020 2020 2070 6561 6b5f 7065 7231         peak_per1
-00005780: 203d 2070 6561 6b5f 7065 7231 5b69 4d61   = peak_per1[iMa
-00005790: 7853 6f72 745d 0a20 2020 2020 2020 2042  xSort].        B
-000057a0: 6578 203d 2042 6578 5b69 4d61 7853 6f72  ex = Bex[iMaxSor
-000057b0: 745d 0a20 2020 2020 2020 2042 6579 203d  t].        Bey =
-000057c0: 2042 6579 5b69 4d61 7853 6f72 745d 0a20   Bey[iMaxSort]. 
-000057d0: 2020 2020 2020 2042 657a 203d 2042 657a         Bez = Bez
-000057e0: 5b69 4d61 7853 6f72 745d 0a20 2020 2020  [iMaxSort].     
-000057f0: 2020 200a 2020 2020 6e5f 7065 616b 7331     .    n_peaks1
-00005800: 203d 206e 702e 7369 7a65 2870 6561 6b5f   = np.size(peak_
-00005810: 7065 7231 290a 0a20 2020 2042 656e 6d31  per1)..    Benm1
-00005820: 203d 206e 702e 7a65 726f 7328 286e 5f70   = np.zeros((n_p
-00005830: 6561 6b73 312c 322c 6e70 726d 5f6d 6178  eaks1,2,nprm_max
-00005840: 2b70 5f6d 6178 2b31 2c6e 7072 6d5f 6d61  +p_max+1,nprm_ma
-00005850: 782b 705f 6d61 782b 3129 2c64 7479 7065  x+p_max+1),dtype
-00005860: 3d6e 702e 636f 6d70 6c65 785f 290a 0a20  =np.complex_).. 
-00005870: 2020 2041 3120 3d20 7371 7274 2832 2a6e     A1 = sqrt(2*n
-00005880: 702e 7069 2f33 290a 0a20 2020 2042 656e  p.pi/3)..    Ben
-00005890: 6d31 5b3a 2c31 2c31 2c31 5d20 3d20 2d41  m1[:,1,1,1] = -A
-000058a0: 3120 2a20 2842 6578 202b 2031 6a2a 4265  1 * (Bex + 1j*Be
-000058b0: 7929 0a20 2020 2042 656e 6d31 5b3a 2c30  y).    Benm1[:,0
-000058c0: 2c31 2c30 5d20 3d20 2d41 312a 7371 7274  ,1,0] = -A1*sqrt
-000058d0: 2832 2920 2a20 4265 7a0a 2020 2020 4265  (2) * Bez.    Be
-000058e0: 6e6d 315b 3a2c 302c 312c 315d 203d 2020  nm1[:,0,1,1] =  
-000058f0: 4131 202a 2028 4265 7820 2d20 316a 2a42  A1 * (Bex - 1j*B
-00005900: 6579 290a 0a20 2020 2023 2047 6574 2073  ey)..    # Get s
-00005910: 7461 7469 6320 6261 636b 6772 6f75 6e64  tatic background
-00005920: 2066 6965 6c64 0a20 2020 2042 3020 3d20   field.    B0 = 
-00005930: 6e70 2e61 7272 6179 285b 6e70 2e6d 6561  np.array([np.mea
-00005940: 6e28 4230 7829 2c20 6e70 2e6d 6561 6e28  n(B0x), np.mean(
-00005950: 4230 7929 2c20 6e70 2e6d 6561 6e28 4230  B0y), np.mean(B0
-00005960: 7a29 5d29 0a20 2020 200a 2020 2020 6966  z)]).    .    if
-00005970: 206e 7072 6d5f 6d61 7820 3e20 313a 0a20   nprm_max > 1:. 
-00005980: 2020 2020 2020 206c 6f67 2e77 6172 6e69         log.warni
-00005990: 6e67 2822 6e27 3d32 2065 7863 6974 6174  ng("n'=2 excitat
-000059a0: 696f 6e20 6d6f 6d65 6e74 7320 6172 6520  ion moments are 
-000059b0: 6265 696e 6720 636f 6e73 6964 6572 6564  being considered
-000059c0: 2c20 6275 7420 7468 6520 616d 706c 6974  , but the amplit
-000059d0: 7564 6573 2061 7265 206a 7573 7420 6120  udes are just a 
-000059e0: 706c 6163 6568 6f6c 6465 7221 2052 656d  placeholder! Rem
-000059f0: 6f76 6520 7468 6973 2077 6172 6e69 6e67  ove this warning
-00005a00: 2077 6865 6e20 636f 7272 6563 7420 4265   when correct Be
-00005a10: 3278 797a 2068 6176 6520 6265 656e 2069  2xyz have been i
-00005a20: 6e73 7461 6c6c 6564 2e22 290a 2020 2020  nstalled.").    
-00005a30: 2020 2020 666f 7220 6e6e 2069 6e20 7261      for nn in ra
-00005a40: 6e67 6528 312c 6e70 726d 5f6d 6178 2b31  nge(1,nprm_max+1
-00005a50: 293a 0a20 2020 2020 2020 2020 2020 2069  ):.            i
-00005a60: 6620 6e6e 203d 3d20 323a 0a20 2020 2020  f nn == 2:.     
-00005a70: 2020 2020 2020 2020 2020 2070 6561 6b5f             peak_
-00005a80: 7065 7232 2c20 7842 6578 5f52 652c 2078  per2, xBex_Re, x
-00005a90: 4265 785f 496d 2c20 7842 6579 5f52 652c  Bex_Im, xBey_Re,
-00005aa0: 2078 4265 795f 496d 2c20 7842 657a 5f52   xBey_Im, xBez_R
-00005ab0: 652c 2078 4265 7a5f 496d 2c20 7942 657a  e, xBez_Im, yBez
-00005ac0: 5f52 652c 2079 4265 7a5f 496d 2c20 7a42  _Re, yBez_Im, zB
-00005ad0: 657a 5f52 652c 207a 4265 7a5f 496d 2020  ez_Re, zBez_Im  
-00005ae0: 2020 5c0a 2020 2020 2020 2020 2020 2020    \.            
-00005af0: 2020 2020 2020 2020 3d20 6e70 2e6c 6f61          = np.loa
-00005b00: 6474 7874 286f 732e 7061 7468 2e6a 6f69  dtxt(os.path.joi
-00005b10: 6e28 6670 6174 682c 2066 2242 6532 7879  n(fpath, f"Be2xy
-00005b20: 7a7b 6266 6e61 6d65 7d2e 7478 7422 292c  z{bfname}.txt"),
-00005b30: 2073 6b69 7072 6f77 733d 312c 2075 6e70   skiprows=1, unp
-00005b40: 6163 6b3d 5472 7565 2c20 6465 6c69 6d69  ack=True, delimi
-00005b50: 7465 723d 272c 2729 0a20 2020 2020 2020  ter=',').       
-00005b60: 2020 2020 2020 2020 206e 5f70 6561 6b73           n_peaks
-00005b70: 3220 3d20 6e70 2e73 697a 6528 7065 616b  2 = np.size(peak
-00005b80: 5f70 6572 3229 0a20 2020 2020 2020 2020  _per2).         
-00005b90: 2020 2020 2020 2042 656e 6d32 203d 206e         Benm2 = n
-00005ba0: 702e 7a65 726f 7328 286e 5f70 6561 6b73  p.zeros((n_peaks
-00005bb0: 322c 322c 6e70 726d 5f6d 6178 2b70 5f6d  2,2,nprm_max+p_m
-00005bc0: 6178 2b31 2c6e 7072 6d5f 6d61 782b 705f  ax+1,nprm_max+p_
-00005bd0: 6d61 782b 3129 2c20 6474 7970 653d 6e70  max+1), dtype=np
-00005be0: 2e63 6f6d 706c 6578 5f29 0a0a 2020 2020  .complex_)..    
-00005bf0: 2020 2020 2020 2020 2020 2020 7842 6578              xBex
-00005c00: 203d 2078 4265 785f 5265 202b 2031 6a2a   = xBex_Re + 1j*
-00005c10: 7842 6578 5f49 6d0a 2020 2020 2020 2020  xBex_Im.        
-00005c20: 2020 2020 2020 2020 7842 6579 203d 2078          xBey = x
-00005c30: 4265 795f 5265 202b 2031 6a2a 7842 6579  Bey_Re + 1j*xBey
-00005c40: 5f49 6d0a 2020 2020 2020 2020 2020 2020  _Im.            
-00005c50: 2020 2020 7842 657a 203d 2078 4265 7a5f      xBez = xBez_
-00005c60: 5265 202b 2031 6a2a 7842 657a 5f49 6d0a  Re + 1j*xBez_Im.
-00005c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005c80: 7942 657a 203d 2079 4265 7a5f 5265 202b  yBez = yBez_Re +
-00005c90: 2031 6a2a 7942 657a 5f49 6d0a 2020 2020   1j*yBez_Im.    
-00005ca0: 2020 2020 2020 2020 2020 2020 7a42 657a              zBez
-00005cb0: 203d 207a 4265 7a5f 5265 202b 2031 6a2a   = zBez_Re + 1j*
-00005cc0: 7a42 657a 5f49 6d0a 0a20 2020 2020 2020  zBez_Im..       
-00005cd0: 2020 2020 2020 2020 206f 7274 3820 3d20           ort8 = 
-00005ce0: 312f 7371 7274 2838 290a 2020 2020 2020  1/sqrt(8).      
-00005cf0: 2020 2020 2020 2020 2020 4132 203d 202d            A2 = -
-00005d00: 7371 7274 2836 2a6e 702e 7069 2f35 290a  sqrt(6*np.pi/5).
-00005d10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005d20: 2042 656e 6d32 5b3a 2c31 2c32 2c32 5d20   Benm2[:,1,2,2] 
-00005d30: 3d20 2041 3220 2a20 2878 4265 7820 2b20  =  A2 * (xBex + 
-00005d40: 316a 2a78 4265 7920 2b20 6f72 7438 2a78  1j*xBey + ort8*x
-00005d50: 4265 7a29 0a20 2020 2020 2020 2020 2020  Bez).           
-00005d60: 2020 2020 2042 656e 6d32 5b3a 2c31 2c32       Benm2[:,1,2
-00005d70: 2c31 5d20 3d20 2041 3220 2a20 2878 4265  ,1] =  A2 * (xBe
-00005d80: 7a20 2d20 316a 2a79 4265 7a29 0a20 2020  z - 1j*yBez).   
-00005d90: 2020 2020 2020 2020 2020 2020 2042 656e               Ben
-00005da0: 6d32 5b3a 2c30 2c32 2c30 5d20 3d20 2041  m2[:,0,2,0] =  A
-00005db0: 3220 2a20 7371 7274 2833 2f32 2920 2a20  2 * sqrt(3/2) * 
-00005dc0: 7a42 657a 0a20 2020 2020 2020 2020 2020  zBez.           
-00005dd0: 2020 2020 2042 656e 6d32 5b3a 2c30 2c32       Benm2[:,0,2
-00005de0: 2c31 5d20 3d20 2d41 3220 2a20 2878 4265  ,1] = -A2 * (xBe
-00005df0: 7a20 2b20 316a 2a79 4265 7a29 0a20 2020  z + 1j*yBez).   
-00005e00: 2020 2020 2020 2020 2020 2020 2042 656e               Ben
-00005e10: 6d32 5b3a 2c30 2c32 2c32 5d20 3d20 2041  m2[:,0,2,2] =  A
-00005e20: 3220 2a20 2878 4265 7820 2d20 316a 2a78  2 * (xBex - 1j*x
-00005e30: 4265 7920 2b20 6f72 7438 2a78 4265 7a29  Bey + ort8*xBez)
-00005e40: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00005e50: 2020 4265 6e6d 203d 206e 702e 7a65 726f    Benm = np.zero
-00005e60: 7328 286e 5f70 6561 6b73 312b 6e5f 7065  s((n_peaks1+n_pe
-00005e70: 616b 7332 2c32 2c6e 7072 6d5f 6d61 782b  aks2,2,nprm_max+
-00005e80: 705f 6d61 782b 312c 6e70 726d 5f6d 6178  p_max+1,nprm_max
-00005e90: 2b70 5f6d 6178 2b31 292c 6474 7970 653d  +p_max+1),dtype=
-00005ea0: 6e70 2e63 6f6d 706c 6578 5f29 0a0a 2020  np.complex_)..  
-00005eb0: 2020 2020 2020 2020 2020 2020 2020 4265                Be
-00005ec0: 6e6d 5b3a 6e5f 7065 616b 7331 2c3a 2c3a  nm[:n_peaks1,:,:
-00005ed0: 2c3a 5d20 3d20 4265 6e6d 310a 2020 2020  ,:] = Benm1.    
-00005ee0: 2020 2020 2020 2020 2020 2020 4265 6e6d              Benm
-00005ef0: 5b6e 5f70 6561 6b73 313a 2c3a 2c3a 2c3a  [n_peaks1:,:,:,:
-00005f00: 5d20 3d20 4265 6e6d 320a 2020 2020 2020  ] = Benm2.      
-00005f10: 2020 2020 2020 2020 2020 7065 616b 5f70            peak_p
-00005f20: 6572 696f 6473 203d 206e 702e 6170 7065  eriods = np.appe
-00005f30: 6e64 2870 6561 6b5f 7065 7231 2c70 6561  nd(peak_per1,pea
-00005f40: 6b5f 7065 7232 290a 0a20 2020 2020 2020  k_per2)..       
-00005f50: 2020 2020 2065 6c69 6620 6e6e 203e 2032       elif nn > 2
-00005f60: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00005f70: 2020 7261 6973 6520 5661 6c75 6545 7272    raise ValueErr
-00005f80: 6f72 2822 6e5f 6d61 7820 3e3d 2033 2069  or("n_max >= 3 i
-00005f90: 7320 6e6f 7420 696d 706c 656d 656e 7465  s not implemente
-00005fa0: 642e 2229 0a20 2020 2065 6c73 653a 0a20  d.").    else:. 
-00005fb0: 2020 2020 2020 2042 656e 6d20 3d20 4265         Benm = Be
-00005fc0: 6e6d 310a 2020 2020 2020 2020 7065 616b  nm1.        peak
-00005fd0: 5f70 6572 696f 6473 203d 2070 6561 6b5f  _periods = peak_
-00005fe0: 7065 7231 0a0a 2020 2020 7265 7475 726e  per1..    return
-00005ff0: 2070 6561 6b5f 7065 7269 6f64 732c 2042   peak_periods, B
-00006000: 656e 6d2c 2042 300a 0a23 2323 2323 2323  enm, B0..#######
-00006010: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00006020: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00006030: 2323 2323 2323 0a0a 2222 220a 4269 4c69  ######..""".BiLi
-00006040: 7374 2829 0a20 2020 2045 7661 6c75 6174  st().    Evaluat
-00006050: 6520 7468 6520 696e 6475 6365 6420 6d61  e the induced ma
-00006060: 676e 6574 6963 206d 6f6d 656e 7473 2042  gnetic moments B
-00006070: 696e 6d20 666f 7220 7468 6520 6769 7665  inm for the give
-00006080: 6e20 6578 6369 7461 7469 6f6e 206d 6f6d  n excitation mom
-00006090: 656e 7473 2042 656e 6d2c 0a20 2020 2066  ents Benm,.    f
-000060a0: 6f72 2074 6865 2067 6976 656e 2069 6e74  or the given int
-000060b0: 6572 696f 7220 7374 7275 6374 7572 6520  erior structure 
-000060c0: 6465 7363 7269 6265 6420 6279 2072 5f62  described by r_b
-000060d0: 6473 2c20 7369 676d 6173 2c20 616e 6420  ds, sigmas, and 
-000060e0: 6173 796d 5f73 6861 7065 2061 6e64 2066  asym_shape and f
-000060f0: 6f72 2061 206c 6973 7420 6f66 206f 6d65  or a list of ome
-00006100: 6761 2076 616c 7565 732e 0a20 2020 2055  ga values..    U
-00006110: 7361 6765 3a20 6042 696e 6d73 6020 3d20  sage: `Binms` = 
-00006120: 4269 4c69 7374 2860 725f 6264 7360 2c20  BiList(`r_bds`, 
-00006130: 6073 6967 6d61 7360 2c20 6070 6561 6b5f  `sigmas`, `peak_
-00006140: 6f6d 6567 6173 602c 2060 6173 796d 5f73  omegas`, `asym_s
-00006150: 6861 7065 602c 2060 4265 6e6d 602c 2060  hape`, `Benm`, `
-00006160: 6e70 726d 7661 6c73 602c 2060 6d70 726d  nprmvals`, `mprm
-00006170: 7661 6c73 602c 2060 7273 6361 6c65 5f6d  vals`, `rscale_m
-00006180: 6f6d 656e 7473 602c 0a20 2020 2020 2020  oments`,.       
-00006190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000061a0: 2020 6070 7661 6c73 602c 2060 7176 616c    `pvals`, `qval
-000061b0: 7360 2c20 606e 7661 6c73 602c 2060 6d76  s`, `nvals`, `mv
-000061c0: 616c 7360 2c20 606e 7072 6d5f 6d61 7860  als`, `nprm_max`
-000061d0: 2c20 6070 5f6d 6178 602c 2060 7772 6974  , `p_max`, `writ
-000061e0: 656f 7574 3d54 7275 6560 2c20 6070 6174  eout=True`, `pat
-000061f0: 683d 4e6f 6e65 602c 0a20 2020 2020 2020  h=None`,.       
-00006200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006210: 2020 6061 7070 656e 643d 2222 602c 2060    `append=""`, `
-00006220: 6465 6275 673d 4661 6c73 6560 290a 2020  debug=False`).  
-00006230: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
-00006240: 2020 2042 696e 6d73 3a20 636f 6d70 6c65     Binms: comple
-00006250: 782c 2073 6861 7065 286e 5f70 6561 6b73  x, shape(n_peaks
-00006260: 2c32 2c6e 5f6d 6178 2b31 2c6e 5f6d 6178  ,2,n_max+1,n_max
-00006270: 2b31 292e 204c 6973 7420 6f66 2063 6f6d  +1). List of com
-00006280: 706c 6578 2069 6e64 7563 6564 206d 6167  plex induced mag
-00006290: 6e65 7469 6320 6d6f 6d65 6e74 7320 666f  netic moments fo
-000062a0: 7220 7468 6520 6769 7665 6e20 7061 7261  r the given para
-000062b0: 6d65 7465 7273 2e0a 2020 2020 5061 7261  meters..    Para
-000062c0: 6d65 7465 7273 3a0a 2020 2020 2020 2020  meters:.        
-000062d0: 725f 6264 733a 2066 6c6f 6174 2c20 7368  r_bds: float, sh
-000062e0: 6170 6528 6e5f 6264 7329 2e20 4c69 7374  ape(n_bds). List
-000062f0: 206f 6620 6d65 616e 2072 6164 6969 2066   of mean radii f
-00006300: 6f72 2065 6163 6820 626f 756e 6461 7279  or each boundary
-00006310: 2073 7572 6661 6365 2069 6e20 6d2e 0a20   surface in m.. 
-00006320: 2020 2020 2020 2073 6967 6d61 733a 2066         sigmas: f
-00006330: 6c6f 6174 2c20 7368 6170 6528 6e5f 6264  loat, shape(n_bd
-00006340: 7329 2e20 4c69 7374 206f 6620 636f 6e64  s). List of cond
-00006350: 7563 7469 7669 7479 2076 616c 7565 7320  uctivity values 
-00006360: 666f 7220 6561 6368 206c 6179 6572 2075  for each layer u
-00006370: 6e64 6572 6e65 6174 6820 7468 6520 636f  nderneath the co
-00006380: 7272 6573 706f 6e64 696e 6720 626f 756e  rresponding boun
-00006390: 6461 7279 2069 6e20 532f 6d2e 0a20 2020  dary in S/m..   
-000063a0: 2020 2020 2070 6561 6b5f 6f6d 6567 6173       peak_omegas
-000063b0: 3a20 666c 6f61 742c 2073 6861 7065 286e  : float, shape(n
-000063c0: 5f70 6561 6b73 292e 204c 6973 7420 6f66  _peaks). List of
-000063d0: 2061 6e67 756c 6172 2066 7265 7175 656e   angular frequen
-000063e0: 6369 6573 2069 6e20 7261 642f 7320 746f  cies in rad/s to
-000063f0: 2065 7661 6c75 6174 652e 2054 7970 6963   evaluate. Typic
-00006400: 616c 6c79 206f 6e6c 7920 7468 6520 7065  ally only the pe
-00006410: 616b 7320 6f66 0a20 2020 2020 2020 2020  aks of.         
-00006420: 2020 2074 6865 2046 6f75 7269 6572 2073     the Fourier s
-00006430: 7065 6374 7261 2e0a 2020 2020 2020 2020  pectra..        
-00006440: 6173 796d 5f73 6861 7065 5f6c 6179 6572  asym_shape_layer
-00006450: 733a 2063 6f6d 706c 6578 2c20 7368 6170  s: complex, shap
-00006460: 6528 6e5f 6264 732c 322c 705f 6d61 782b  e(n_bds,2,p_max+
-00006470: 312c 705f 6d61 782b 3129 2e20 4162 736f  1,p_max+1). Abso
-00006480: 6c75 7465 2064 6576 6961 7469 6f6e 7320  lute deviations 
-00006490: 666f 7220 6561 6368 2062 6f75 6e64 6172  for each boundar
-000064a0: 7920 696e 206d 2c20 6967 6e6f 7269 6e67  y in m, ignoring
-000064b0: 0a20 2020 2020 2020 2020 2020 2067 7261  .            gra
-000064c0: 7669 7461 7469 6f6e 616c 2070 6572 7475  vitational pertu
-000064d0: 7262 6174 696f 6e73 2e0a 2020 2020 2020  rbations..      
-000064e0: 2020 6772 6176 5f73 6861 7065 3a20 636f    grav_shape: co
-000064f0: 6d70 6c65 782c 2073 6861 7065 286e 5f62  mplex, shape(n_b
-00006500: 6473 2c32 2c70 5f6d 6178 2b31 2c70 5f6d  ds,2,p_max+1,p_m
-00006510: 6178 2b31 292e 2041 6273 6f6c 7574 6520  ax+1). Absolute 
-00006520: 6465 7669 6174 696f 6e73 2066 6f72 2065  deviations for e
-00006530: 6163 6820 2863 6f6e 6475 6374 696e 6729  ach (conducting)
-00006540: 2062 6f75 6e64 6172 7920 696e 206d 2c0a   boundary in m,.
-00006550: 2020 2020 2020 2020 2020 2020 6475 6520              due 
-00006560: 746f 2067 7261 7669 7461 7469 6f6e 616c  to gravitational
-00006570: 2070 6572 7475 7262 6174 696f 6e73 2e0a   perturbations..
-00006580: 2020 2020 2020 2020 4265 6e6d 3a20 636f          Benm: co
-00006590: 6d70 6c65 782c 2073 6861 7065 2832 2c6e  mplex, shape(2,n
-000065a0: 5f6d 6178 2b31 2c6e 5f6d 6178 2b31 292e  _max+1,n_max+1).
-000065b0: 2045 7863 6974 6174 696f 6e20 6d6f 6d65   Excitation mome
-000065c0: 6e74 7320 666f 7220 6561 6368 2064 6567  nts for each deg
-000065d0: 7265 6520 616e 6420 6f72 6465 7220 6e27  ree and order n'
-000065e0: 2c6d 272e 0a20 2020 2020 2020 2072 7363  ,m'..        rsc
-000065f0: 616c 655f 6d6f 6d65 6e74 733a 2066 6c6f  ale_moments: flo
-00006600: 6174 2e20 4571 7561 6c20 746f 2031 2f52  at. Equal to 1/R
-00006610: 5f62 6f64 7920 696e 2075 6e69 7473 206f  _body in units o
-00006620: 6620 312f 6d2e 2046 6f72 2070 726f 7065  f 1/m. For prope
-00006630: 7220 7363 616c 696e 6720 7768 656e 2063  r scaling when c
-00006640: 6f6e 6475 6374 696e 6720 626f 756e 6461  onducting bounda
-00006650: 7269 6573 0a20 2020 2020 2020 2020 2020  ries.           
-00006660: 206d 6179 206f 7220 6d61 7920 6e6f 7420   may or may not 
-00006670: 636f 696e 6369 6465 2077 6974 6820 7468  coincide with th
-00006680: 6520 626f 6479 2073 7572 6661 6365 2e0a  e body surface..
-00006690: 2020 2020 2020 2020 6e76 616c 732c 206d          nvals, m
-000066a0: 7661 6c73 3a20 696e 7465 6765 722c 2073  vals: integer, s
-000066b0: 6861 7065 284e 6e6d 292e 204c 696e 6561  hape(Nnm). Linea
-000066c0: 7220 6172 7261 7973 206f 6620 7061 6972  r arrays of pair
-000066d0: 6564 206e 2c6d 2076 616c 7565 7320 666f  ed n,m values fo
-000066e0: 7220 7061 7261 6c6c 656c 2063 6f6d 7075  r parallel compu
-000066f0: 7461 7469 6f6e 2e0a 2020 2020 2020 2020  tation..        
-00006700: 705f 6d61 783a 2069 6e74 6567 6572 2e20  p_max: integer. 
-00006710: 4d61 7869 6d75 6d20 6465 6772 6565 2070  Maximum degree p
-00006720: 206f 6620 626f 756e 6461 7279 2073 6861   of boundary sha
-00006730: 7065 732e 0a20 2020 2020 2020 206e 7072  pes..        npr
-00006740: 6d5f 6d61 783a 2069 6e74 6567 6572 2028  m_max: integer (
-00006750: 3129 2e20 4d61 7869 6d75 6d20 6465 6772  1). Maximum degr
-00006760: 6565 206e 2720 6f66 2042 656e 6d20 746f  ee n' of Benm to
-00006770: 2065 7661 6c75 6174 652e 206e 273d 3120   evaluate. n'=1 
-00006780: 6973 2075 6e69 666f 726d 2066 6965 6c64  is uniform field
-00006790: 2076 6563 746f 722e 0a20 2020 2020 2020   vector..       
-000067a0: 2077 7269 7465 6f75 743a 2062 6f6f 6c65   writeout: boole
-000067b0: 616e 2028 5472 7565 292e 2057 6865 7468  an (True). Wheth
-000067c0: 6572 2074 6f20 7361 7665 2063 6f6d 7075  er to save compu
-000067d0: 7465 6420 7661 6c75 6573 2074 6f20 6469  ted values to di
-000067e0: 736b 2066 6f72 2072 6170 6964 2072 6570  sk for rapid rep
-000067f0: 6c6f 7474 696e 672e 0a20 2020 2020 2020  lotting..       
-00006800: 2070 6174 683a 2073 7472 696e 6720 284e   path: string (N
-00006810: 6f6e 6529 2e20 5061 7468 2072 656c 6174  one). Path relat
-00006820: 6976 6520 746f 2072 756e 2064 6972 6563  ive to run direc
-00006830: 746f 7279 2074 6f20 7072 696e 7420 6f75  tory to print ou
-00006840: 7470 7574 2064 6174 6120 746f 2e20 4465  tput data to. De
-00006850: 6661 756c 7473 2074 6f20 223c 696e 7374  faults to "<inst
-00006860: 616c 6c5f 6c6f 633e 2f4d 6f6f 6e4d 6167  all_loc>/MoonMag
-00006870: 2f69 6e64 7563 6564 2f22 2e0a 2020 2020  /induced/"..    
-00006880: 2020 2020 626f 6479 6e61 6d65 3a20 7374      bodyname: st
-00006890: 7269 6e67 2028 4e6f 6e65 292e 2042 6f64  ring (None). Bod
-000068a0: 7920 6e61 6d65 2074 6f20 696e 636c 7564  y name to includ
-000068b0: 6520 696e 2077 7269 7465 6f75 7420 6669  e in writeout fi
-000068c0: 6c65 6e61 6d65 2e0a 2020 2020 2020 2020  lename..        
-000068d0: 7665 7262 6f73 653a 2062 6f6f 6c65 616e  verbose: boolean
-000068e0: 2028 5472 7565 292e 2057 6865 7468 6572   (True). Whether
-000068f0: 2074 6f20 7072 696e 7420 7072 6f67 7265   to print progre
-00006900: 7373 2075 7064 6174 6573 2074 6f20 7468  ss updates to th
-00006910: 6520 7465 726d 696e 616c 2e0a 2020 2020  e terminal..    
-00006920: 2020 2020 6170 7065 6e64 3a20 7374 7269      append: stri
-00006930: 6e67 2028 2222 292e 204f 7074 696f 6e61  ng (""). Optiona
-00006940: 6c20 7374 7269 6e67 2061 7070 656e 6465  l string appende
-00006950: 6420 746f 2064 6566 6175 6c74 2066 696c  d to default fil
-00006960: 6520 6e61 6d65 732e 0a20 2020 2020 2020  e names..       
-00006970: 2064 6562 7567 3a20 626f 6f6c 6561 6e20   debug: boolean 
-00006980: 2846 616c 7365 292e 2053 7065 6369 616c  (False). Special
-00006990: 2075 7365 2066 6c61 672e 0a20 2020 2020   use flag..     
-000069a0: 2020 2064 6f5f 7061 7261 6c6c 656c 3a20     do_parallel: 
-000069b0: 626f 6f6c 6561 6e20 2854 7275 6529 2e20  boolean (True). 
-000069c0: 546f 6767 6c65 2066 6f72 2072 756e 6e69  Toggle for runni
-000069d0: 6e67 2063 6572 7461 696e 2063 616c 6375  ng certain calcu
-000069e0: 6c61 7469 6f6e 7320 696e 2070 6172 616c  lations in paral
-000069f0: 6c65 6c2e 0a20 2020 2020 2020 206f 7574  lel..        out
-00006a00: 466e 616d 653a 2073 7472 696e 6720 284e  Fname: string (N
-00006a10: 6f6e 6529 2e20 4f75 7470 7574 2066 696c  one). Output fil
-00006a20: 656e 616d 6520 746f 2075 7365 2077 6865  ename to use whe
-00006a30: 6e20 7772 6974 656f 7574 203d 2054 7275  n writeout = Tru
-00006a40: 652e 0a20 2020 2020 2020 206f 7574 466e  e..        outFn
-00006a50: 616d 6553 3a20 7374 7269 6e67 2028 4e6f  ameS: string (No
-00006a60: 6e65 292e 2041 7320 6162 6f76 652c 2066  ne). As above, f
-00006a70: 6f72 206f 7574 7075 7420 4761 7573 7320  or output Gauss 
-00006a80: 636f 6566 6669 6369 656e 7473 2069 6e20  coefficients in 
-00006a90: 7468 6520 5363 686d 6964 7420 6e6f 726d  the Schmidt norm
-00006aa0: 616c 697a 6174 696f 6e2e 0a20 2020 2020  alization..     
-00006ab0: 2020 2058 6964 3a20 636f 6d70 6c65 7820     Xid: complex 
-00006ac0: 284e 6f6e 652c 2073 6861 7065 202e 2e2e  (None, shape ...
-00006ad0: 292e 204f 7074 696f 6e20 746f 2070 6173  ). Option to pas
-00006ae0: 7320 696e 2058 6964 2074 6f20 6176 6f69  s in Xid to avoi
-00006af0: 6420 6e65 6564 696e 6720 746f 2072 656c  d needing to rel
-00006b00: 6f61 6420 6672 6f6d 2064 6973 6b20 6f72  oad from disk or
-00006b10: 2072 6563 616c 6375 6c61 7465 2e0a 2020   recalculate..  
-00006b20: 2020 2222 220a 6465 6620 4269 4c69 7374    """.def BiList
-00006b30: 2872 5f62 6473 2c20 7369 676d 6173 2c20  (r_bds, sigmas, 
-00006b40: 7065 616b 5f6f 6d65 6761 732c 2061 7379  peak_omegas, asy
-00006b50: 6d5f 7368 6170 655f 6c61 7965 7273 2c20  m_shape_layers, 
-00006b60: 6772 6176 5f73 6861 7065 2c20 4265 6e6d  grav_shape, Benm
-00006b70: 2c20 7273 6361 6c65 5f6d 6f6d 656e 7473  , rscale_moments
-00006b80: 2c20 6e76 616c 732c 206d 7661 6c73 2c20  , nvals, mvals, 
-00006b90: 705f 6d61 782c 206e 7072 6d5f 6d61 783d  p_max, nprm_max=
-00006ba0: 312c 2077 7269 7465 6f75 743d 5472 7565  1, writeout=True
-00006bb0: 2c20 7061 7468 3d4e 6f6e 652c 2062 6f64  , path=None, bod
-00006bc0: 796e 616d 653d 4e6f 6e65 2c0a 2020 2020  yname=None,.    
-00006bd0: 2020 2020 2020 2076 6572 626f 7365 3d54         verbose=T
-00006be0: 7275 652c 2061 7070 656e 643d 2222 2c20  rue, append="", 
-00006bf0: 6465 6275 673d 4661 6c73 652c 2064 6f5f  debug=False, do_
-00006c00: 7061 7261 6c6c 656c 3d54 7275 652c 2053  parallel=True, S
-00006c10: 6368 6d69 6474 3d46 616c 7365 2c20 6f75  chmidt=False, ou
-00006c20: 7446 6e61 6d65 3d4e 6f6e 652c 206f 7574  tFname=None, out
-00006c30: 466e 616d 6553 3d4e 6f6e 652c 2058 6964  FnameS=None, Xid
-00006c40: 3d4e 6f6e 6529 3a0a 0a20 2020 2023 2043  =None):..    # C
-00006c50: 6c65 616e 2069 6e70 7574 7320 616e 6420  lean inputs and 
-00006c60: 696e 6974 6961 6c69 7a65 0a20 2020 2069  initialize.    i
-00006c70: 6620 6e6f 7420 6973 696e 7374 616e 6365  f not isinstance
-00006c80: 2870 6561 6b5f 6f6d 6567 6173 2c20 4974  (peak_omegas, It
-00006c90: 6572 6162 6c65 293a 0a20 2020 2020 2020  erable):.       
-00006ca0: 2070 6561 6b5f 6f6d 6567 6173 203d 205b   peak_omegas = [
-00006cb0: 7065 616b 5f6f 6d65 6761 735d 0a20 2020  peak_omegas].   
-00006cc0: 206e 5f70 6561 6b73 203d 206e 702e 7369   n_peaks = np.si
-00006cd0: 7a65 2870 6561 6b5f 6f6d 6567 6173 290a  ze(peak_omegas).
-00006ce0: 2020 2020 4e6e 6d20 3d20 6e70 2e73 697a      Nnm = np.siz
-00006cf0: 6528 6e76 616c 7329 0a20 2020 206e 5f6d  e(nvals).    n_m
-00006d00: 6178 203d 206e 7072 6d5f 6d61 7820 2b20  ax = nprm_max + 
-00006d10: 705f 6d61 780a 2020 2020 4269 6e6d 7320  p_max.    Binms 
-00006d20: 3d20 6e70 2e7a 6572 6f73 2828 6e5f 7065  = np.zeros((n_pe
-00006d30: 616b 732c 2032 2c20 6e5f 6d61 782b 312c  aks, 2, n_max+1,
-00006d40: 206e 5f6d 6178 2b31 292c 2064 7479 7065   n_max+1), dtype
-00006d50: 3d6e 702e 636f 6d70 6c65 785f 290a 2020  =np.complex_).  
-00006d60: 2020 6c6f 672e 6465 6275 6728 6622 4361    log.debug(f"Ca
-00006d70: 6c63 756c 6174 696e 6720 6173 796d 6d65  lculating asymme
-00006d80: 7472 6963 2042 5f69 6e6d 2066 6f72 207b  tric B_inm for {
-00006d90: 6e70 2e73 697a 6528 7065 616b 5f6f 6d65  np.size(peak_ome
-00006da0: 6761 7329 7d20 7065 7269 6f64 732e 2229  gas)} periods.")
-00006db0: 0a20 2020 2069 6620 7772 6974 656f 7574  .    if writeout
-00006dc0: 3a0a 2020 2020 2020 2020 6966 2062 6f64  :.        if bod
-00006dd0: 796e 616d 6520 6973 204e 6f6e 653a 0a20  yname is None:. 
-00006de0: 2020 2020 2020 2020 2020 2062 666e 616d             bfnam
-00006df0: 6520 3d20 2222 0a20 2020 2020 2020 2065  e = "".        e
-00006e00: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-00006e10: 2062 666e 616d 6520 3d20 6622 7b62 6f64   bfname = f"{bod
-00006e20: 796e 616d 657d 5f22 0a20 2020 2069 6620  yname}_".    if 
-00006e30: 7273 6361 6c65 5f6d 6f6d 656e 7473 203d  rscale_moments =
-00006e40: 3d20 312e 303a 0a20 2020 2020 2020 2072  = 1.0:.        r
-00006e50: 7363 616c 696e 6720 3d20 7273 6361 6c65  scaling = rscale
-00006e60: 5f6d 6f6d 656e 7473 0a20 2020 2065 6c73  _moments.    els
-00006e70: 653a 0a20 2020 2020 2020 2072 7363 616c  e:.        rscal
-00006e80: 696e 6720 203d 2072 7363 616c 655f 6d6f  ing  = rscale_mo
-00006e90: 6d65 6e74 7320 2a20 725f 6264 735b 2d31  ments * r_bds[-1
-00006ea0: 5d0a 2020 2020 6966 2067 7261 765f 7368  ].    if grav_sh
-00006eb0: 6170 6520 6973 204e 6f6e 653a 0a20 2020  ape is None:.   
-00006ec0: 2020 2020 2061 7379 6d5f 7368 6170 6520       asym_shape 
-00006ed0: 3d20 6173 796d 5f73 6861 7065 5f6c 6179  = asym_shape_lay
-00006ee0: 6572 730a 2020 2020 656c 7365 3a0a 2020  ers.    else:.  
-00006ef0: 2020 2020 2020 6173 796d 5f73 6861 7065        asym_shape
-00006f00: 203d 2061 7379 6d5f 7368 6170 655f 6c61   = asym_shape_la
-00006f10: 7965 7273 202b 2067 7261 765f 7368 6170  yers + grav_shap
-00006f20: 650a 0a20 2020 2023 2047 6574 206d 6978  e..    # Get mix
-00006f30: 696e 6720 636f 6566 6669 6369 656e 7473  ing coefficients
-00006f40: 0a20 2020 2069 6620 5869 6420 6973 204e  .    if Xid is N
-00006f50: 6f6e 653a 0a20 2020 2020 2020 2058 6964  one:.        Xid
-00006f60: 203d 2067 6574 5f61 6c6c 5f58 6964 286e   = get_all_Xid(n
-00006f70: 7072 6d5f 6d61 782c 2070 5f6d 6178 2c20  prm_max, p_max, 
-00006f80: 6e70 726d 5f6d 6178 2b70 5f6d 6178 2c20  nprm_max+p_max, 
-00006f90: 6e76 616c 732c 206d 7661 6c73 2c20 7265  nvals, mvals, re
-00006fa0: 6c6f 6164 3d54 7275 652c 2064 6f5f 7061  load=True, do_pa
-00006fb0: 7261 6c6c 656c 3d64 6f5f 7061 7261 6c6c  rallel=do_parall
-00006fc0: 656c 2c20 6670 6174 683d 7061 7468 290a  el, fpath=path).
-00006fd0: 0a20 2020 2069 6620 646f 5f70 6172 616c  .    if do_paral
-00006fe0: 6c65 6c20 616e 6420 6e6f 7420 6465 6275  lel and not debu
-00006ff0: 673a 0a20 2020 2020 2020 2070 6172 5f6b  g:.        par_k
-00007000: 7720 3d20 7b27 6e70 726d 5f6d 6178 273a  w = {'nprm_max':
-00007010: 6e70 726d 5f6d 6178 2c20 2776 6572 626f  nprm_max, 'verbo
-00007020: 7365 273a 7665 7262 6f73 657d 0a20 2020  se':verbose}.   
-00007030: 2020 2020 2023 2046 6f72 2065 6163 6820       # For each 
-00007040: 6f6d 6567 612c 2065 7661 6c75 6174 6520  omega, evaluate 
-00007050: 4269 3a0a 2020 2020 2020 2020 706f 6f6c  Bi:.        pool
-00007060: 203d 206d 7470 436f 6e74 6578 742e 506f   = mtpContext.Po
-00007070: 6f6c 286e 702e 6d69 6e69 6d75 6d28 6e75  ol(np.minimum(nu
-00007080: 6d5f 636f 7265 732c 6e5f 7065 616b 7329  m_cores,n_peaks)
-00007090: 290a 2020 2020 2020 2020 7061 725f 7265  ).        par_re
-000070a0: 7375 6c74 203d 205b 706f 6f6c 2e61 7070  sult = [pool.app
-000070b0: 6c79 5f61 7379 6e63 2820 4269 6e6d 5265  ly_async( BinmRe
-000070c0: 7370 6f6e 7365 2c20 2872 5f62 6473 2c73  sponse, (r_bds,s
-000070d0: 6967 6d61 732c 7065 616b 5f6f 6d65 6761  igmas,peak_omega
-000070e0: 735b 695f 6f6d 5d2c 6173 796d 5f73 6861  s[i_om],asym_sha
-000070f0: 7065 2c42 656e 6d5b 695f 6f6d 2c2e 2e2e  pe,Benm[i_om,...
-00007100: 5d2c 5869 642c 705f 6d61 782c 7273 6361  ],Xid,p_max,rsca
-00007110: 6c69 6e67 292c 2070 6172 5f6b 7720 2920  ling), par_kw ) 
-00007120: 666f 7220 695f 6f6d 2069 6e20 7261 6e67  for i_om in rang
-00007130: 6528 6e5f 7065 616b 7329 5d0a 2020 2020  e(n_peaks)].    
-00007140: 2020 2020 706f 6f6c 2e63 6c6f 7365 2829      pool.close()
-00007150: 0a20 2020 2020 2020 2070 6f6f 6c2e 6a6f  .        pool.jo
-00007160: 696e 2829 0a0a 2020 2020 2020 2020 666f  in()..        fo
-00007170: 7220 695f 6f6d 2069 6e20 7261 6e67 6528  r i_om in range(
-00007180: 6e5f 7065 616b 7329 3a0a 2020 2020 2020  n_peaks):.      
-00007190: 2020 2020 2020 4269 6e6d 735b 695f 6f6d        Binms[i_om
-000071a0: 2c20 2e2e 2e5d 203d 2070 6172 5f72 6573  , ...] = par_res
-000071b0: 756c 745b 695f 6f6d 5d2e 6765 7428 290a  ult[i_om].get().
-000071c0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-000071d0: 2020 6966 2064 6562 7567 3a0a 2020 2020    if debug:.    
-000071e0: 2020 2020 2020 2020 4165 732c 2041 7473          Aes, Ats
-000071f0: 2c20 4164 7320 3d20 5b20 6e70 2e7a 6572  , Ads = [ np.zer
-00007200: 6f73 2828 6e5f 7065 616b 732c 206e 7072  os((n_peaks, npr
-00007210: 6d5f 6d61 782b 705f 6d61 7829 2c20 6474  m_max+p_max), dt
-00007220: 7970 653d 6e70 2e63 6f6d 706c 6578 5f29  ype=np.complex_)
-00007230: 2066 6f72 205f 2069 6e20 7261 6e67 6528   for _ in range(
-00007240: 3329 205d 0a20 2020 2020 2020 2020 2020  3) ].           
-00007250: 206b 7276 616c 7320 3d20 6e70 2e7a 6572   krvals = np.zer
-00007260: 6f73 286e 5f70 6561 6b73 2c20 6474 7970  os(n_peaks, dtyp
-00007270: 653d 6e70 2e63 6f6d 706c 6578 5f29 0a20  e=np.complex_). 
-00007280: 2020 2020 2020 2020 2020 2066 6f72 2069             for i
-00007290: 5f6f 6d20 696e 2072 616e 6765 286e 5f70  _om in range(n_p
-000072a0: 6561 6b73 293a 0a20 2020 2020 2020 2020  eaks):.         
-000072b0: 2020 2020 2020 2042 696e 6d73 5b30 2c20         Binms[0, 
-000072c0: 2e2e 2e5d 2c20 4165 735b 695f 6f6d 2c20  ...], Aes[i_om, 
-000072d0: 3a5d 2c20 4174 735b 695f 6f6d 2c20 3a5d  :], Ats[i_om, :]
-000072e0: 2c20 4164 735b 695f 6f6d 2c20 3a5d 2c20  , Ads[i_om, :], 
-000072f0: 6b72 7661 6c73 5b69 5f6f 6d5d 203d 2042  krvals[i_om] = B
-00007300: 696e 6d52 6573 706f 6e73 6528 725f 6264  inmResponse(r_bd
-00007310: 732c 2073 6967 6d61 732c 2070 6561 6b5f  s, sigmas, peak_
-00007320: 6f6d 6567 6173 5b69 5f6f 6d5d 2c20 6173  omegas[i_om], as
-00007330: 796d 5f73 6861 7065 2c20 4265 6e6d 5b30  ym_shape, Benm[0
-00007340: 2c20 2e2e 2e5d 2c20 5869 642c 2070 5f6d  , ...], Xid, p_m
-00007350: 6178 2c20 7273 6361 6c69 6e67 2c20 6e70  ax, rscaling, np
-00007360: 726d 5f6d 6178 3d6e 7072 6d5f 6d61 782c  rm_max=nprm_max,
-00007370: 2076 6572 626f 7365 3d76 6572 626f 7365   verbose=verbose
-00007380: 2c20 6465 6275 673d 6465 6275 6729 0a20  , debug=debug). 
-00007390: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-000073a0: 6620 2869 5f6f 6d2b 3129 2025 2031 3020  f (i_om+1) % 10 
-000073b0: 3d3d 2030 3a20 6c6f 672e 6465 6275 6728  == 0: log.debug(
-000073c0: 6622 7b69 5f6f 6d20 2b20 317d 206f 6620  f"{i_om + 1} of 
-000073d0: 7b6e 5f70 6561 6b73 7d20 636f 6d70 6c65  {n_peaks} comple
-000073e0: 7465 2e22 290a 2020 2020 2020 2020 656c  te.").        el
-000073f0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-00007400: 666f 7220 695f 6f6d 2069 6e20 7261 6e67  for i_om in rang
-00007410: 6528 6e5f 7065 616b 7329 3a0a 2020 2020  e(n_peaks):.    
-00007420: 2020 2020 2020 2020 2020 2020 4269 6e6d              Binm
-00007430: 735b 695f 6f6d 2c20 2e2e 2e5d 203d 2042  s[i_om, ...] = B
-00007440: 696e 6d52 6573 706f 6e73 6528 725f 6264  inmResponse(r_bd
-00007450: 732c 2073 6967 6d61 732c 2070 6561 6b5f  s, sigmas, peak_
-00007460: 6f6d 6567 6173 5b69 5f6f 6d5d 2c20 6173  omegas[i_om], as
-00007470: 796d 5f73 6861 7065 2c20 4265 6e6d 5b69  ym_shape, Benm[i
-00007480: 5f6f 6d2c 202e 2e2e 5d2c 2058 6964 2c20  _om, ...], Xid, 
-00007490: 705f 6d61 782c 2072 7363 616c 696e 672c  p_max, rscaling,
-000074a0: 206e 7072 6d5f 6d61 783d 6e70 726d 5f6d   nprm_max=nprm_m
-000074b0: 6178 2c20 7665 7262 6f73 653d 7665 7262  ax, verbose=verb
-000074c0: 6f73 6529 0a20 2020 2020 2020 2020 2020  ose).           
-000074d0: 2020 2020 206c 6f67 2e64 6562 7567 2866       log.debug(f
-000074e0: 227b 695f 6f6d 202b 2031 7d20 6f66 207b  "{i_om + 1} of {
-000074f0: 6e5f 7065 616b 737d 2063 6f6d 706c 6574  n_peaks} complet
-00007500: 652e 2229 0a0a 2020 2020 6966 2077 7269  e.")..    if wri
-00007510: 7465 6f75 743a 0a20 2020 2020 2020 2069  teout:.        i
-00007520: 6620 7061 7468 2069 7320 4e6f 6e65 3a0a  f path is None:.
-00007530: 2020 2020 2020 2020 2020 2020 7061 7468              path
-00007540: 203d 205f 696e 6475 6365 640a 2020 2020   = _induced.    
-00007550: 2020 2020 6966 206f 7574 466e 616d 6520      if outFname 
-00007560: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
-00007570: 2020 2020 206f 7574 466e 616d 6520 3d20       outFname = 
-00007580: 6627 7b62 666e 616d 657d 4269 6e6d 5f61  f'{bfname}Binm_a
-00007590: 7379 6d7b 6170 7065 6e64 7d27 0a20 2020  sym{append}'.   
-000075a0: 2020 2020 2066 7061 7468 203d 206f 732e       fpath = os.
-000075b0: 7061 7468 2e6a 6f69 6e28 7061 7468 2c20  path.join(path, 
-000075c0: 6622 7b6f 7574 466e 616d 657d 2e64 6174  f"{outFname}.dat
-000075d0: 2229 0a20 2020 2020 2020 2066 6f75 7420  ").        fout 
-000075e0: 3d20 6f70 656e 2866 7061 7468 2c20 2277  = open(fpath, "w
-000075f0: 2229 0a20 2020 2020 2020 2068 6561 6465  ").        heade
-00007600: 7220 3d20 227b 3a3c 3133 7d2c 207b 3a3c  r = "{:<13}, {:<
-00007610: 347d 2c20 7b3a 3c34 7d2c 207b 3a3c 3234  4}, {:<4}, {:<24
-00007620: 7d2c 207b 3a3c 3234 7d5c 6e22 2e66 6f72  }, {:<24}\n".for
-00007630: 6d61 7428 2250 6572 696f 6420 2868 7229  mat("Period (hr)
-00007640: 2022 2c20 226e 2022 2c20 226d 2022 2c20   ", "n ", "m ", 
-00007650: 2242 696e 6d5f 5265 2028 6e54 2922 2c20  "Binm_Re (nT)", 
-00007660: 2242 696e 6d5f 496d 2028 6e54 2922 290a  "Binm_Im (nT)").
-00007670: 2020 2020 2020 2020 666f 7574 2e77 7269          fout.wri
-00007680: 7465 2868 6561 6465 7229 0a20 2020 2020  te(header).     
-00007690: 2020 2066 6f72 2069 2069 6e20 7261 6e67     for i in rang
-000076a0: 6528 6e70 2e73 697a 6528 7065 616b 5f6f  e(np.size(peak_o
-000076b0: 6d65 6761 7329 293a 0a20 2020 2020 2020  megas)):.       
-000076c0: 2020 2020 2054 5f68 7273 203d 2032 2a6e       T_hrs = 2*n
-000076d0: 702e 7069 2f70 6561 6b5f 6f6d 6567 6173  p.pi/peak_omegas
-000076e0: 5b69 5d2f 3336 3030 0a20 2020 2020 2020  [i]/3600.       
-000076f0: 2020 2020 2066 6f72 2069 5f6e 6d20 696e       for i_nm in
-00007700: 2072 616e 6765 284e 6e6d 293a 0a20 2020   range(Nnm):.   
-00007710: 2020 2020 2020 2020 2020 2020 2073 6967               sig
-00007720: 6e20 3d20 696e 7428 6d76 616c 735b 695f  n = int(mvals[i_
-00007730: 6e6d 5d3c 3029 0a20 2020 2020 2020 2020  nm]<0).         
-00007740: 2020 2020 2020 2074 6869 735f 4269 6e6d         this_Binm
-00007750: 203d 2042 696e 6d73 5b69 2c73 6967 6e2c   = Binms[i,sign,
-00007760: 6e76 616c 735b 695f 6e6d 5d2c 6162 7328  nvals[i_nm],abs(
-00007770: 6d76 616c 735b 695f 6e6d 5d29 5d0a 2020  mvals[i_nm])].  
-00007780: 2020 2020 2020 2020 2020 2020 2020 666f                fo
-00007790: 7574 2e77 7269 7465 2820 227b 3a3c 3133  ut.write( "{:<13
-000077a0: 7d2c 207b 3a3c 347d 2c20 7b3a 3c34 7d2c  }, {:<4}, {:<4},
-000077b0: 207b 3a3c 3234 7d2c 207b 3a3c 3234 7d5c   {:<24}, {:<24}\
-000077c0: 6e22 2e66 6f72 6d61 7428 726f 756e 6428  n".format(round(
-000077d0: 545f 6872 732c 3529 2c20 6e76 616c 735b  T_hrs,5), nvals[
-000077e0: 695f 6e6d 5d2c 206d 7661 6c73 5b69 5f6e  i_nm], mvals[i_n
-000077f0: 6d5d 2c20 6e70 2e72 6561 6c28 7468 6973  m], np.real(this
-00007800: 5f42 696e 6d29 2c20 6e70 2e69 6d61 6728  _Binm), np.imag(
-00007810: 7468 6973 5f42 696e 6d29 2920 290a 2020  this_Binm)) ).  
-00007820: 2020 2020 2020 666f 7574 2e63 6c6f 7365        fout.close
-00007830: 2829 0a20 2020 2020 2020 206c 6f67 2e69  ().        log.i
-00007840: 6e66 6f28 6622 4461 7461 2066 6f72 2061  nfo(f"Data for a
-00007850: 7379 6d6d 6574 7269 6320 4269 6e6d 2077  symmetric Binm w
-00007860: 7269 7474 656e 2074 6f20 6669 6c65 3a20  ritten to file: 
-00007870: 7b66 7061 7468 7d22 290a 0a20 2020 2020  {fpath}")..     
-00007880: 2020 2069 6620 5363 686d 6964 743a 0a20     if Schmidt:. 
-00007890: 2020 2020 2020 2020 2020 2069 6620 6f75             if ou
-000078a0: 7446 6e61 6d65 5320 6973 204e 6f6e 653a  tFnameS is None:
-000078b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000078c0: 206f 7574 466e 616d 6553 203d 2066 277b   outFnameS = f'{
-000078d0: 6266 6e61 6d65 7d67 686e 6d5f 6173 796d  bfname}ghnm_asym
-000078e0: 7b61 7070 656e 647d 270a 2020 2020 2020  {append}'.      
-000078f0: 2020 2020 2020 6670 6174 6820 3d20 6f73        fpath = os
-00007900: 2e70 6174 682e 6a6f 696e 2870 6174 682c  .path.join(path,
-00007910: 2066 227b 6f75 7446 6e61 6d65 537d 2e64   f"{outFnameS}.d
-00007920: 6174 2229 0a20 2020 2020 2020 2020 2020  at").           
-00007930: 2066 6f75 7420 3d20 6f70 656e 2866 7061   fout = open(fpa
-00007940: 7468 2c20 2277 2229 0a20 2020 2020 2020  th, "w").       
-00007950: 2020 2020 2068 6561 6465 7220 3d20 227b       header = "{
-00007960: 3a3c 3133 7d2c 207b 3a3c 347d 2c20 7b3a  :<13}, {:<4}, {:
-00007970: 3c34 7d2c 207b 3a3c 3234 7d2c 207b 3a3c  <4}, {:<24}, {:<
-00007980: 3234 7d2c 207b 3a3c 3234 7d2c 207b 3a3c  24}, {:<24}, {:<
-00007990: 3234 7d5c 6e22 2e66 6f72 6d61 7428 2250  24}\n".format("P
-000079a0: 6572 696f 6420 2868 7229 2022 2c20 226e  eriod (hr) ", "n
-000079b0: 2022 2c20 226d 2022 2c20 2267 5f6e 6d5f   ", "m ", "g_nm_
-000079c0: 5265 2028 6e54 2922 2c20 2267 5f6e 6d5f  Re (nT)", "g_nm_
-000079d0: 496d 2028 6e54 2922 2c20 2268 5f6e 6d5f  Im (nT)", "h_nm_
-000079e0: 5265 2028 6e54 2922 2c20 2268 5f6e 6d5f  Re (nT)", "h_nm_
-000079f0: 496d 2028 6e54 2922 290a 2020 2020 2020  Im (nT)").      
-00007a00: 2020 2020 2020 666f 7574 2e77 7269 7465        fout.write
-00007a10: 2868 6561 6465 7229 0a20 2020 2020 2020  (header).       
-00007a20: 2020 2020 2066 6f72 2069 2069 6e20 7261       for i in ra
-00007a30: 6e67 6528 6e70 2e73 697a 6528 7065 616b  nge(np.size(peak
-00007a40: 5f6f 6d65 6761 7329 293a 0a20 2020 2020  _omegas)):.     
-00007a50: 2020 2020 2020 2020 2020 2054 5f68 7273             T_hrs
-00007a60: 203d 2032 2a6e 702e 7069 2f70 6561 6b5f   = 2*np.pi/peak_
-00007a70: 6f6d 6567 6173 5b69 5d2f 3336 3030 0a20  omegas[i]/3600. 
-00007a80: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-00007a90: 6869 735f 676e 6d2c 2074 6869 735f 686e  his_gnm, this_hn
-00007aa0: 6d20 3d20 6765 745f 6768 5f66 726f 6d5f  m = get_gh_from_
-00007ab0: 4269 6e6d 286e 5f6d 6178 2c42 696e 6d73  Binm(n_max,Binms
-00007ac0: 5b69 2c2e 2e2e 5d29 0a20 2020 2020 2020  [i,...]).       
-00007ad0: 2020 2020 2020 2020 2066 6f72 206e 2069           for n i
-00007ae0: 6e20 7261 6e67 6528 312c 6e5f 6d61 782b  n range(1,n_max+
-00007af0: 3129 3a0a 2020 2020 2020 2020 2020 2020  1):.            
-00007b00: 2020 2020 2020 2020 666f 7220 6d20 696e          for m in
-00007b10: 2072 616e 6765 286e 2b31 293a 0a20 2020   range(n+1):.   
-00007b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007b30: 2020 2020 2066 6f75 742e 7772 6974 6528       fout.write(
-00007b40: 2022 7b3a 3c31 337d 2c20 7b3a 3c34 7d2c   "{:<13}, {:<4},
-00007b50: 207b 3a3c 347d 2c20 7b3a 3c32 347d 2c20   {:<4}, {:<24}, 
-00007b60: 7b3a 3c32 347d 2c20 7b3a 3c32 347d 2c20  {:<24}, {:<24}, 
-00007b70: 7b3a 3c32 347d 5c6e 222e 666f 726d 6174  {:<24}\n".format
-00007b80: 2872 6f75 6e64 2854 5f68 7273 2c35 292c  (round(T_hrs,5),
-00007b90: 206e 2c20 6d2c 206e 702e 7265 616c 2874   n, m, np.real(t
-00007ba0: 6869 735f 676e 6d5b 6e2c 6d5d 292c 206e  his_gnm[n,m]), n
-00007bb0: 702e 696d 6167 2874 6869 735f 676e 6d5b  p.imag(this_gnm[
-00007bc0: 6e2c 6d5d 292c 206e 702e 7265 616c 2874  n,m]), np.real(t
-00007bd0: 6869 735f 686e 6d5b 6e2c 6d5d 292c 206e  his_hnm[n,m]), n
-00007be0: 702e 696d 6167 2874 6869 735f 686e 6d5b  p.imag(this_hnm[
-00007bf0: 6e2c 6d5d 2929 2029 0a20 2020 2020 2020  n,m])) ).       
-00007c00: 2020 2020 2066 6f75 742e 636c 6f73 6528       fout.close(
-00007c10: 290a 2020 2020 2020 2020 2020 2020 6c6f  ).            lo
-00007c20: 672e 696e 666f 2866 2244 6174 6120 666f  g.info(f"Data fo
-00007c30: 7220 6173 796d 6d65 7472 6963 2c20 5363  r asymmetric, Sc
-00007c40: 686d 6964 7420 7365 6d69 2d6e 6f72 6d61  hmidt semi-norma
-00007c50: 6c69 7a65 6420 675f 6e6d 2061 6e64 2068  lized g_nm and h
-00007c60: 5f6e 6d20 7772 6974 7465 6e20 746f 2066  _nm written to f
-00007c70: 696c 653a 207b 6670 6174 687d 2229 0a0a  ile: {fpath}")..
-00007c80: 2020 2020 6966 2064 6562 7567 3a0a 2020      if debug:.  
-00007c90: 2020 2020 2020 7265 7475 726e 2042 696e        return Bin
-00007ca0: 6d73 2c20 4165 732c 2041 7473 2c20 4164  ms, Aes, Ats, Ad
-00007cb0: 732c 206b 7276 616c 730a 2020 2020 656c  s, krvals.    el
-00007cc0: 7365 3a0a 2020 2020 2020 2020 7265 7475  se:.        retu
-00007cd0: 726e 2042 696e 6d73 0a0a 2323 2323 2323  rn Binms..######
-00007ce0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00007cf0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-00007d00: 2323 2323 2323 230a 0a22 2222 0a42 696e  #######..""".Bin
-00007d10: 6d52 6573 706f 6e73 6528 290a 2020 2020  mResponse().    
-00007d20: 5468 6520 696e 6475 6365 6420 6d61 676e  The induced magn
-00007d30: 6574 6963 206d 6f6d 656e 7473 2042 696e  etic moments Bin
-00007d40: 6d20 666f 7220 616c 6c20 696e 7075 7420  m for all input 
-00007d50: 6465 6772 6565 206e 2061 6e64 206f 7264  degree n and ord
-00007d60: 6572 206d 2c0a 2020 2020 7769 7468 2061  er m,.    with a
-00007d70: 2073 7065 6369 6669 6564 2061 7379 6d6d   specified asymm
-00007d80: 6574 7269 6320 626f 756e 6461 7279 2073  etric boundary s
-00007d90: 6861 7065 2061 7379 6d5f 7368 6170 6520  hape asym_shape 
-00007da0: 616e 6420 666f 7220 7468 6520 696e 7075  and for the inpu
-00007db0: 740a 2020 2020 4265 6e6d 2061 7420 6120  t.    Benm at a 
-00007dc0: 7369 6e67 6c65 2066 7265 7175 656e 6379  single frequency
-00007dd0: 206f 6d65 6761 2e0a 2020 2020 5573 6167   omega..    Usag
-00007de0: 653a 2060 4269 6e6d 6020 3d20 4269 6e6d  e: `Binm` = Binm
-00007df0: 5265 7370 6f6e 7365 2860 725f 6264 7360  Response(`r_bds`
-00007e00: 2c20 6073 6967 6d61 7360 2c20 606f 6d65  , `sigmas`, `ome
-00007e10: 6761 602c 2060 6173 796d 5f73 6861 7065  ga`, `asym_shape
-00007e20: 602c 2060 4265 6e6d 602c 2060 5869 6460  `, `Benm`, `Xid`
-00007e30: 2c20 6070 5f6d 6178 602c 2060 7273 6361  , `p_max`, `rsca
-00007e40: 6c69 6e67 602c 2060 6e70 726d 5f6d 6178  ling`, `nprm_max
-00007e50: 3d31 602c 2060 7665 7262 6f73 653d 5472  =1`, `verbose=Tr
-00007e60: 7565 602c 2060 6465 6275 673d 4661 6c73  ue`, `debug=Fals
-00007e70: 6560 290a 2020 2020 5265 7475 726e 733a  e`).    Returns:
-00007e80: 0a20 2020 2020 2020 2042 696e 6d3a 2063  .        Binm: c
-00007e90: 6f6d 706c 6578 2c20 7368 6170 6528 322c  omplex, shape(2,
-00007ea0: 6e5f 6d61 782b 312c 6e5f 6d61 782b 3129  n_max+1,n_max+1)
-00007eb0: 2e20 5468 6520 636f 6d70 6c65 7820 696e  . The complex in
-00007ec0: 6475 6365 6420 6d6f 6d65 6e74 7320 666f  duced moments fo
-00007ed0: 7220 7468 6520 6769 7665 6e20 4265 6e6d  r the given Benm
-00007ee0: 2061 6e64 2061 7379 6d6d 6574 7269 6320   and asymmetric 
-00007ef0: 696e 7465 7269 6f72 2073 7472 7563 7475  interior structu
-00007f00: 7265 2c0a 2020 2020 2020 2020 2020 2020  re,.            
-00007f10: 6576 616c 7561 7465 6420 666f 7220 6120  evaluated for a 
-00007f20: 7369 6e67 6c65 2061 6e67 756c 6172 2066  single angular f
-00007f30: 7265 7175 656e 6379 206f 6620 6f73 6369  requency of osci
-00007f40: 6c6c 6174 696f 6e20 6f6d 6567 612e 0a20  llation omega.. 
-00007f50: 2020 2050 6172 616d 6574 6572 733a 0a20     Parameters:. 
-00007f60: 2020 2020 2020 2072 5f62 6473 3a20 666c         r_bds: fl
-00007f70: 6f61 742c 2073 6861 7065 286e 5f62 6473  oat, shape(n_bds
-00007f80: 292e 2052 6164 6969 2066 6f72 2065 6163  ). Radii for eac
-00007f90: 6820 626f 756e 6461 7279 2073 7572 6661  h boundary surfa
-00007fa0: 6365 2069 6e20 6d2e 0a20 2020 2020 2020  ce in m..       
-00007fb0: 2073 6967 6d61 733a 2066 6c6f 6174 2c20   sigmas: float, 
-00007fc0: 7368 6170 6528 6e5f 6264 7329 2e20 436f  shape(n_bds). Co
-00007fd0: 6e64 7563 7469 7669 7479 2066 6f72 2065  nductivity for e
-00007fe0: 6163 6820 6c61 7965 7220 756e 6465 7220  ach layer under 
-00007ff0: 7468 6520 636f 7272 6573 706f 6e64 696e  the correspondin
-00008000: 6720 626f 756e 6461 7279 2069 6e20 532f  g boundary in S/
-00008010: 6d2e 0a20 2020 2020 2020 206f 6d65 6761  m..        omega
-00008020: 3a20 666c 6f61 742e 2041 6e67 756c 6172  : float. Angular
-00008030: 2066 7265 7175 656e 6379 206f 6620 6d61   frequency of ma
-00008040: 676e 6574 6963 206f 7363 696c 6c61 7469  gnetic oscillati
-00008050: 6f6e 7320 696e 2072 6164 2f73 2e0a 2020  ons in rad/s..  
-00008060: 2020 2020 2020 6173 796d 5f73 6861 7065        asym_shape
-00008070: 3a20 636f 6d70 6c65 782c 2073 6861 7065  : complex, shape
-00008080: 286e 5f62 6473 2c32 2c70 5f6d 6178 2b31  (n_bds,2,p_max+1
-00008090: 2c70 5f6d 6178 2b31 292e 2041 206c 6973  ,p_max+1). A lis
-000080a0: 7420 6f66 2062 6f75 6e64 6172 7920 7368  t of boundary sh
-000080b0: 6170 6520 7061 7261 6d65 7465 7273 2063  ape parameters c
-000080c0: 6869 5f70 7120 666f 7220 6561 6368 2062  hi_pq for each b
-000080d0: 6f75 6e64 6172 792e 0a20 2020 2020 2020  oundary..       
-000080e0: 2042 656e 6d3a 2063 6f6d 706c 6578 2c20   Benm: complex, 
-000080f0: 7368 6170 6528 322c 6e5f 6d61 782b 312c  shape(2,n_max+1,
-00008100: 6e5f 6d61 782b 3129 2e20 4578 6369 7461  n_max+1). Excita
-00008110: 7469 6f6e 206d 6f6d 656e 7473 2066 6f72  tion moments for
-00008120: 2065 6163 6820 6e27 2061 6e64 206d 272c   each n' and m',
-00008130: 2070 6164 6465 6420 7769 7468 207a 6572   padded with zer
-00008140: 6f73 2066 6f72 206e 203e 206e 272e 0a20  os for n > n'.. 
-00008150: 2020 2020 2020 2058 6964 3a20 6d70 662c         Xid: mpf,
-00008160: 2073 6861 7065 2832 2c6e 7072 6d5f 6d61   shape(2,nprm_ma
-00008170: 782b 312c 6e70 726d 5f6d 6178 2b31 2c20  x+1,nprm_max+1, 
-00008180: 322c 705f 6d61 782b 312c 705f 6d61 782b  2,p_max+1,p_max+
-00008190: 312c 2032 2c6e 5f6d 6178 2b31 2c6e 5f6d  1, 2,n_max+1,n_m
-000081a0: 6178 2b31 292e 204d 6978 696e 6720 636f  ax+1). Mixing co
-000081b0: 6566 6669 6369 656e 7473 0a20 2020 2020  efficients.     
-000081c0: 2020 2020 2020 2072 6573 756c 7469 6e67         resulting
-000081d0: 2066 726f 6d20 6d75 6c74 6970 6c69 6361   from multiplica
-000081e0: 7469 6f6e 206f 6620 7370 6865 7269 6361  tion of spherica
-000081f0: 6c20 6861 726d 6f6e 6963 732e 205c 5869  l harmonics. \Xi
-00008200: 5e7b 5c73 7461 7220 6e6d 7d5f 7b6e 276d  ^{\star nm}_{n'm
-00008210: 2770 717d 2066 726f 6d20 7468 6520 7061  'pq} from the pa
-00008220: 7065 722e 0a20 2020 2020 2020 2070 5f6d  per..        p_m
-00008230: 6178 3a20 696e 7465 6765 722e 204c 6172  ax: integer. Lar
-00008240: 6765 7374 2064 6567 7265 6520 7020 696e  gest degree p in
-00008250: 2069 6e74 6572 696f 7220 6d6f 6465 6c20   interior model 
-00008260: 626f 756e 6461 7279 2073 6861 7065 732e  boundary shapes.
-00008270: 0a20 2020 2020 2020 2072 7363 616c 696e  .        rscalin
-00008280: 673a 2066 6c6f 6174 2e20 5261 7469 6f20  g: float. Ratio 
-00008290: 6f66 206f 7574 6572 6d6f 7374 2063 6f6e  of outermost con
-000082a0: 6475 6374 696e 6720 626f 756e 6461 7279  ducting boundary
-000082b0: 2074 6f20 626f 6479 2072 6164 6975 732e   to body radius.
-000082c0: 0a20 2020 2020 2020 206e 7072 6d5f 6d61  .        nprm_ma
-000082d0: 783a 2069 6e74 6567 6572 2028 3129 2e20  x: integer (1). 
-000082e0: 4d61 7869 6d75 6d20 6465 6772 6565 206e  Maximum degree n
-000082f0: 2720 6f66 2042 656e 6d20 746f 2065 7661  ' of Benm to eva
-00008300: 6c75 6174 652e 206e 273d 3120 6973 2075  luate. n'=1 is u
-00008310: 6e69 666f 726d 2066 6965 6c64 2076 6563  niform field vec
-00008320: 746f 722e 0a20 2020 2020 2020 2076 6572  tor..        ver
-00008330: 626f 7365 3a20 626f 6f6c 6561 6e20 2854  bose: boolean (T
-00008340: 7275 6529 2e20 5768 6574 6865 7220 746f  rue). Whether to
-00008350: 2070 7269 6e74 2070 726f 6772 6573 7320   print progress 
-00008360: 7570 6461 7465 7320 746f 2074 6865 2074  updates to the t
-00008370: 6572 6d69 6e61 6c2e 0a20 2020 2020 2020  erminal..       
-00008380: 2064 6562 7567 3a20 626f 6f6c 6561 6e20   debug: boolean 
-00008390: 2846 616c 7365 292e 2053 7065 6369 616c  (False). Special
-000083a0: 2075 7365 2066 6c61 672e 0a20 2020 2022   use flag..    "
-000083b0: 2222 0a64 6566 2042 696e 6d52 6573 706f  "".def BinmRespo
-000083c0: 6e73 6528 725f 6264 732c 2073 6967 6d61  nse(r_bds, sigma
-000083d0: 732c 206f 6d65 6761 2c20 6173 796d 5f73  s, omega, asym_s
-000083e0: 6861 7065 2c20 4265 6e6d 2c20 5869 642c  hape, Benm, Xid,
-000083f0: 2070 5f6d 6178 2c20 7273 6361 6c69 6e67   p_max, rscaling
-00008400: 2c20 6e70 726d 5f6d 6178 3d31 2c20 7665  , nprm_max=1, ve
-00008410: 7262 6f73 653d 5472 7565 2c20 6465 6275  rbose=True, debu
-00008420: 673d 4661 6c73 6529 3a0a 2020 2020 6e5f  g=False):.    n_
-00008430: 6d61 7820 3d20 6e70 726d 5f6d 6178 202b  max = nprm_max +
-00008440: 2070 5f6d 6178 0a20 2020 2042 696e 6d20   p_max.    Binm 
-00008450: 3d20 6e70 2e7a 6572 6f73 2828 322c 206e  = np.zeros((2, n
-00008460: 5f6d 6178 2b31 2c20 6e5f 6d61 782b 3129  _max+1, n_max+1)
-00008470: 2c20 6474 7970 653d 6e70 2e63 6f6d 706c  , dtype=np.compl
-00008480: 6578 5f29 0a20 2020 206e 5f62 6473 203d  ex_).    n_bds =
-00008490: 206e 702e 7369 7a65 2872 5f62 6473 290a   np.size(r_bds).
-000084a0: 2020 2020 6e5f 696e 6e65 7220 3d20 6e5f      n_inner = n_
-000084b0: 6264 7320 2d20 310a 0a20 2020 206e 695f  bds - 1..    ni_
-000084c0: 6264 7320 3d20 6e5f 6264 7320 2d20 310a  bds = n_bds - 1.
-000084d0: 2020 2020 6e69 5f69 6e6e 6572 203d 206e      ni_inner = n
-000084e0: 5f69 6e6e 6572 202d 2031 0a20 2020 206c  _inner - 1.    l
-000084f0: 6f6e 6520 3d20 6f6e 650a 2020 2020 637a  one = one.    cz
-00008500: 6572 6f20 3d20 6d70 2e6d 7063 2830 290a  ero = mp.mpc(0).
-00008510: 0a20 2020 2023 2047 6574 2074 7970 6520  .    # Get type 
-00008520: 6f62 6a65 6374 2066 6f72 2069 6e69 7469  object for initi
-00008530: 616c 697a 696e 6720 6e75 6d70 7920 6172  alizing numpy ar
-00008540: 7261 7973 206f 6620 6d70 630a 2020 2020  rays of mpc.    
-00008550: 6d70 6320 3d20 6d70 635f 676c 6f62 616c  mpc = mpc_global
-00008560: 0a0a 2020 2020 2320 436f 6e76 6572 7420  ..    # Convert 
-00008570: 696e 7075 7420 6461 7461 2066 6f72 206b  input data for k
-00008580: 2076 616c 7565 7320 696e 746f 206d 706d   values into mpm
-00008590: 6174 6820 666c 6f61 7473 0a20 2020 2023  ath floats.    #
-000085a0: 2057 6865 6e20 7765 2077 6f6e 2774 206e   When we won't n
-000085b0: 6565 6420 746f 2065 7870 6c69 6369 746c  eed to explicitl
-000085c0: 7920 6c6f 6f70 206f 7665 7220 696e 6469  y loop over indi
-000085d0: 6365 732c 2075 7365 206e 756d 7079 0a20  ces, use numpy. 
-000085e0: 2020 2023 2061 7272 6179 7320 746f 2065     # arrays to e
-000085f0: 6e61 626c 6520 7665 6374 6f72 697a 6564  nable vectorized
-00008600: 2063 6f6d 7075 7461 7469 6f6e 2e0a 2020   computation..  
-00008610: 2020 6e20 3d20 6e70 2e61 7272 6179 285b    n = np.array([
-00008620: 206d 702e 6d70 6628 6e69 2920 666f 7220   mp.mpf(ni) for 
-00008630: 6e69 2069 6e20 7261 6e67 6528 312c 6e5f  ni in range(1,n_
-00008640: 6d61 782b 3129 205d 290a 2020 2020 6966  max+1) ]).    if
-00008650: 206e 6f74 2069 7369 6e73 7461 6e63 6528   not isinstance(
-00008660: 725f 6264 732c 2049 7465 7261 626c 6529  r_bds, Iterable)
-00008670: 3a0a 2020 2020 2020 2020 725f 6264 7320  :.        r_bds 
-00008680: 3d20 5b6d 702e 6d70 6628 725f 6264 7329  = [mp.mpf(r_bds)
-00008690: 5d0a 2020 2020 2020 2020 7369 676d 6173  ].        sigmas
-000086a0: 203d 205b 6d70 2e6d 7066 2873 6967 6d61   = [mp.mpf(sigma
-000086b0: 7329 5d0a 2020 2020 656c 7365 3a0a 2020  s)].    else:.  
-000086c0: 2020 2020 2020 725f 6264 7320 3d20 5b6d        r_bds = [m
-000086d0: 702e 6d70 6628 725f 6929 2066 6f72 2072  p.mpf(r_i) for r
-000086e0: 5f69 2069 6e20 725f 6264 735d 0a20 2020  _i in r_bds].   
-000086f0: 2020 2020 2073 6967 6d61 7320 3d20 5b6d       sigmas = [m
-00008700: 702e 6d70 6628 7369 675f 6929 2066 6f72  p.mpf(sig_i) for
-00008710: 2073 6967 5f69 2069 6e20 7369 676d 6173   sig_i in sigmas
-00008720: 5d0a 0a20 2020 2069 6620 6e6f 7420 6465  ]..    if not de
-00008730: 6275 673a 0a20 2020 2020 2020 206f 6d65  bug:.        ome
-00008740: 6761 203d 206d 702e 6d70 6628 6f6d 6567  ga = mp.mpf(omeg
-00008750: 6129 0a0a 2020 2020 2020 2020 2320 4d61  a)..        # Ma
-00008760: 6b65 206c 6973 7473 206f 6620 6b20 7661  ke lists of k va
-00008770: 6c75 6573 0a20 2020 2020 2020 206b 725f  lues.        kr_
-00008780: 6c6c 203d 206e 702e 6172 7261 7928 5b20  ll = np.array([ 
-00008790: 6d70 2e73 7172 7428 6a2a 6f6d 6567 612a  mp.sqrt(j*omega*
-000087a0: 6d75 5f6f 2a73 6967 6d61 735b 695f 6264  mu_o*sigmas[i_bd
-000087b0: 795d 292a 725f 6264 735b 695f 6264 795d  y])*r_bds[i_bdy]
-000087c0: 2066 6f72 2069 5f62 6479 2069 6e20 7261   for i_bdy in ra
-000087d0: 6e67 6528 6e5f 696e 6e65 7229 205d 290a  nge(n_inner) ]).
-000087e0: 2020 2020 2020 2020 6b72 5f75 6c20 3d20          kr_ul = 
-000087f0: 6e70 2e61 7272 6179 285b 206d 702e 7371  np.array([ mp.sq
-00008800: 7274 286a 2a6f 6d65 6761 2a6d 755f 6f2a  rt(j*omega*mu_o*
-00008810: 7369 676d 6173 5b69 5f62 6479 2b31 5d29  sigmas[i_bdy+1])
-00008820: 2a72 5f62 6473 5b69 5f62 6479 5d20 666f  *r_bds[i_bdy] fo
-00008830: 7220 695f 6264 7920 696e 2072 616e 6765  r i_bdy in range
-00008840: 286e 5f69 6e6e 6572 2920 5d29 0a20 2020  (n_inner) ]).   
-00008850: 2020 2020 2023 206b 6120 7661 6c75 6520       # ka value 
-00008860: 6174 206f 7574 6572 2062 6f75 6e64 6172  at outer boundar
-00008870: 790a 2020 2020 2020 2020 6b72 5f65 7820  y.        kr_ex 
-00008880: 3d20 6d70 2e73 7172 7428 6a2a 6f6d 6567  = mp.sqrt(j*omeg
-00008890: 612a 6d75 5f6f 2a73 6967 6d61 735b 2d31  a*mu_o*sigmas[-1
-000088a0: 5d29 2a72 5f62 6473 5b2d 315d 0a20 2020  ])*r_bds[-1].   
-000088b0: 2065 6c73 653a 0a20 2020 2020 2020 206e   else:.        n
-000088c0: 5f62 6473 203d 2031 0a20 2020 2020 2020  _bds = 1.       
-000088d0: 2023 2046 6f72 2064 6562 7567 2070 7572   # For debug pur
-000088e0: 706f 7365 732c 206f 6d65 6761 2069 7320  poses, omega is 
-000088f0: 7061 7373 6564 2069 6e20 6173 2061 206b  passed in as a k
-00008900: 7220 7661 6c75 650a 2020 2020 2020 2020  r value.        
-00008910: 6b72 5f65 7820 3d20 6d70 2e73 7172 7428  kr_ex = mp.sqrt(
-00008920: 6a29 202a 206d 702e 6d70 6628 6f6d 6567  j) * mp.mpf(omeg
-00008930: 6129 0a0a 2020 2020 2320 496e 7365 7274  a)..    # Insert
-00008940: 206b 7220 696e 746f 2042 6573 7365 6c20   kr into Bessel 
-00008950: 6675 6e63 7469 6f6e 7320 666f 7220 6f75  functions for ou
-00008960: 7465 7220 6264 7920 6f6e 6c79 2066 6972  ter bdy only fir
-00008970: 7374 0a20 2020 206a 6e5f 6578 203d 206e  st.    jn_ex = n
-00008980: 702e 7a65 726f 7328 6e5f 6d61 782c 2064  p.zeros(n_max, d
-00008990: 7479 7065 3d6d 7063 290a 2020 2020 6a64  type=mpc).    jd
-000089a0: 5f65 7820 3d20 6e70 2e7a 6572 6f73 286e  _ex = np.zeros(n
-000089b0: 5f6d 6178 2c20 6474 7970 653d 6d70 6329  _max, dtype=mpc)
-000089c0: 0a20 2020 2079 6e5f 6578 203d 206e 702e  .    yn_ex = np.
-000089d0: 7a65 726f 7328 6e5f 6d61 782c 2064 7479  zeros(n_max, dty
-000089e0: 7065 3d6d 7063 290a 2020 2020 7964 5f65  pe=mpc).    yd_e
-000089f0: 7820 3d20 6e70 2e7a 6572 6f73 286e 5f6d  x = np.zeros(n_m
-00008a00: 6178 2c20 6474 7970 653d 6d70 6329 0a20  ax, dtype=mpc). 
-00008a10: 2020 2066 6f72 206e 6920 696e 2072 616e     for ni in ran
-00008a20: 6765 286e 5f6d 6178 293a 0a20 2020 2020  ge(n_max):.     
-00008a30: 2020 206a 6e5f 6578 5b6e 695d 203d 206a     jn_ex[ni] = j
-00008a40: 6e78 286e 5b6e 695d 2c5b 6b72 5f65 785d  nx(n[ni],[kr_ex]
-00008a50: 295b 305d 0a20 2020 2020 2020 206a 645f  )[0].        jd_
-00008a60: 6578 5b6e 695d 203d 206a 6478 286e 5b6e  ex[ni] = jdx(n[n
-00008a70: 695d 2c5b 6b72 5f65 785d 295b 305d 0a20  i],[kr_ex])[0]. 
-00008a80: 2020 2020 2020 2079 6e5f 6578 5b6e 695d         yn_ex[ni]
-00008a90: 203d 2079 6e78 286e 5b6e 695d 2c5b 6b72   = ynx(n[ni],[kr
-00008aa0: 5f65 785d 295b 305d 0a20 2020 2020 2020  _ex])[0].       
-00008ab0: 2079 645f 6578 5b6e 695d 203d 2079 6478   yd_ex[ni] = ydx
-00008ac0: 286e 5b6e 695d 2c5b 6b72 5f65 785d 295b  (n[ni],[kr_ex])[
-00008ad0: 305d 0a0a 2020 2020 2320 4361 6c63 756c  0]..    # Calcul
-00008ae0: 6174 6520 6f75 7465 7220 626f 756e 6461  ate outer bounda
-00008af0: 7279 2074 7261 6e73 6665 7220 7175 616e  ry transfer quan
-00008b00: 7469 7469 6573 2e0a 2020 2020 2320 416c  tities..    # Al
-00008b10: 6c20 7375 6368 2071 7561 6e74 6974 6965  l such quantitie
-00008b20: 7320 2868 6572 6520 616e 6420 6d6f 7265  s (here and more
-00008b30: 2062 656c 6f77 2920 6861 7665 2051 2061   below) have Q a
-00008b40: 7070 656e 6465 642d 2d2d 7468 6520 2251  ppended---the "Q
-00008b50: 2072 6573 706f 6e73 6522 2069 7320 616e   response" is an
-00008b60: 616c 6f67 6f75 7320 746f 205c 6d61 7468  alogous to \math
-00008b70: 6361 6c7b 417d 2e0a 2020 2020 616c 7068  cal{A}..    alph
-00008b80: 5120 3d20 312f 6b72 5f65 780a 2020 2020  Q = 1/kr_ex.    
-00008b90: 6265 7461 5120 3d20 6a64 5f65 7820 2d20  betaQ = jd_ex - 
-00008ba0: 286e 2b6f 6e65 292a 6a6e 5f65 780a 2020  (n+one)*jn_ex.  
-00008bb0: 2020 6761 6d6d 5120 3d20 7964 5f65 7820    gammQ = yd_ex 
-00008bc0: 2d20 286e 2b6f 6e65 292a 796e 5f65 780a  - (n+one)*yn_ex.
-00008bd0: 2020 2020 6465 6c74 5120 3d20 6e2a 6a6e      deltQ = n*jn
-00008be0: 5f65 7820 2b20 6a64 5f65 780a 2020 2020  _ex + jd_ex.    
-00008bf0: 6570 7369 5120 3d20 6e2a 796e 5f65 7820  epsiQ = n*yn_ex 
-00008c00: 2b20 7964 5f65 780a 2020 2020 7869 5f5f  + yd_ex.    xi__
-00008c10: 5120 3d20 2d6b 725f 6578 2a2a 3220 2a20  Q = -kr_ex**2 * 
-00008c20: 6a6e 5f65 785b 3a6e 7072 6d5f 6d61 785d  jn_ex[:nprm_max]
-00008c30: 0a20 2020 2072 686f 5f51 203d 202d 6b72  .    rho_Q = -kr
-00008c40: 5f65 782a 2a32 202a 2079 6e5f 6578 5b3a  _ex**2 * yn_ex[:
-00008c50: 6e70 726d 5f6d 6178 5d0a 2020 2020 7a65  nprm_max].    ze
-00008c60: 7461 5120 3d20 6e2a 6a6e 5f65 780a 2020  taQ = n*jn_ex.  
-00008c70: 2020 6574 615f 5120 3d20 6e2a 796e 5f65    eta_Q = n*yn_e
-00008c80: 780a 0a20 2020 206c 6f67 2e64 6562 7567  x..    log.debug
-00008c90: 2822 2020 2020 496e 6974 6961 6c69 7a65  ("    Initialize
-00008ca0: 6420 7472 616e 7366 6572 2063 616c 6375  d transfer calcu
-00008cb0: 6c61 7469 6f6e 732e 2e2e 2229 0a0a 2020  lations...")..  
-00008cc0: 2020 2320 4966 2074 6865 7265 2773 206f    # If there's o
-00008cd0: 6e6c 7920 6f6e 6520 626f 756e 6461 7279  nly one boundary
-00008ce0: 2c20 6b72 5f6c 6c20 616e 6420 6b72 5f75  , kr_ll and kr_u
-00008cf0: 6c20 6172 6520 656d 7074 7920 616e 6420  l are empty and 
-00008d00: 7765 2063 616e 2069 6d6d 6564 6961 7465  we can immediate
-00008d10: 6c79 2063 616c 6375 6c61 7465 2041 2066  ly calculate A f
-00008d20: 756e 6374 696f 6e20 7661 6c75 6573 2e0a  unction values..
-00008d30: 2020 2020 6966 206e 5f62 6473 203e 2031      if n_bds > 1
-00008d40: 3a0a 2020 2020 2020 2020 2320 496e 6974  :.        # Init
-00008d50: 6961 6c69 7a65 2042 6573 7365 6c20 6675  ialize Bessel fu
-00008d60: 6e63 7469 6f6e 2072 6573 756c 7473 0a20  nction results. 
-00008d70: 2020 2020 2020 206a 6e5f 6c6c 2c20 6a64         jn_ll, jd
-00008d80: 5f6c 6c2c 2079 6e5f 6c6c 2c20 7964 5f6c  _ll, yn_ll, yd_l
-00008d90: 6c20 3d20 2820 6e70 2e7a 6572 6f73 2828  l = ( np.zeros((
-00008da0: 6e5f 6d61 782c 6e5f 696e 6e65 7229 2c20  n_max,n_inner), 
-00008db0: 6474 7970 653d 6d70 6329 2066 6f72 205f  dtype=mpc) for _
-00008dc0: 2069 6e20 7261 6e67 6528 3429 2029 0a20   in range(4) ). 
-00008dd0: 2020 2020 2020 206a 6e5f 756c 2c20 6a64         jn_ul, jd
-00008de0: 5f75 6c2c 2079 6e5f 756c 2c20 7964 5f75  _ul, yn_ul, yd_u
-00008df0: 6c20 3d20 2820 6e70 2e7a 6572 6f73 2828  l = ( np.zeros((
-00008e00: 6e5f 6d61 782c 6e5f 696e 6e65 7229 2c20  n_max,n_inner), 
-00008e10: 6474 7970 653d 6d70 6329 2066 6f72 205f  dtype=mpc) for _
-00008e20: 2069 6e20 7261 6e67 6528 3429 2029 0a0a   in range(4) )..
-00008e30: 2020 2020 2020 2020 2320 436f 6e74 696e          # Contin
-00008e40: 7565 2069 6e73 6572 7469 6e67 206b 7220  ue inserting kr 
-00008e50: 696e 746f 2042 6573 7365 6c20 6675 6e63  into Bessel func
-00008e60: 7469 6f6e 730a 2020 2020 2020 2020 666f  tions.        fo
-00008e70: 7220 6e69 2069 6e20 7261 6e67 6528 6e5f  r ni in range(n_
-00008e80: 6d61 7829 3a0a 2020 2020 2020 2020 2020  max):.          
-00008e90: 2020 6a6e 5f6c 6c5b 6e69 2c3a 5d20 3d20    jn_ll[ni,:] = 
-00008ea0: 6a6e 7828 6e5b 6e69 5d2c 6b72 5f6c 6c29  jnx(n[ni],kr_ll)
-00008eb0: 0a20 2020 2020 2020 2020 2020 206a 645f  .            jd_
-00008ec0: 6c6c 5b6e 692c 3a5d 203d 206a 6478 286e  ll[ni,:] = jdx(n
-00008ed0: 5b6e 695d 2c6b 725f 6c6c 290a 2020 2020  [ni],kr_ll).    
-00008ee0: 2020 2020 2020 2020 796e 5f6c 6c5b 6e69          yn_ll[ni
-00008ef0: 2c3a 5d20 3d20 796e 7828 6e5b 6e69 5d2c  ,:] = ynx(n[ni],
-00008f00: 6b72 5f6c 6c29 0a20 2020 2020 2020 2020  kr_ll).         
-00008f10: 2020 2079 645f 6c6c 5b6e 692c 3a5d 203d     yd_ll[ni,:] =
-00008f20: 2079 6478 286e 5b6e 695d 2c6b 725f 6c6c   ydx(n[ni],kr_ll
-00008f30: 290a 0a20 2020 2020 2020 2020 2020 206a  )..            j
-00008f40: 6e5f 756c 5b6e 692c 3a5d 203d 206a 6e78  n_ul[ni,:] = jnx
-00008f50: 286e 5b6e 695d 2c6b 725f 756c 290a 2020  (n[ni],kr_ul).  
-00008f60: 2020 2020 2020 2020 2020 6a64 5f75 6c5b            jd_ul[
-00008f70: 6e69 2c3a 5d20 3d20 6a64 7828 6e5b 6e69  ni,:] = jdx(n[ni
-00008f80: 5d2c 6b72 5f75 6c29 0a20 2020 2020 2020  ],kr_ul).       
-00008f90: 2020 2020 2079 6e5f 756c 5b6e 692c 3a5d       yn_ul[ni,:]
-00008fa0: 203d 2079 6e78 286e 5b6e 695d 2c6b 725f   = ynx(n[ni],kr_
-00008fb0: 756c 290a 2020 2020 2020 2020 2020 2020  ul).            
-00008fc0: 7964 5f75 6c5b 6e69 2c3a 5d20 3d20 7964  yd_ul[ni,:] = yd
-00008fd0: 7828 6e5b 6e69 5d2c 6b72 5f75 6c29 0a0a  x(n[ni],kr_ul)..
-00008fe0: 2020 2020 2020 2020 2320 4361 6c63 756c          # Calcul
-00008ff0: 6174 6520 6c61 7965 7220 7472 616e 7366  ate layer transf
-00009000: 6572 2071 7561 6e74 6974 6965 730a 2020  er quantities.  
-00009010: 2020 2020 2020 616c 7068 203d 206e 702e        alph = np.
-00009020: 7a65 726f 7328 286e 5f6d 6178 2c6e 5f69  zeros((n_max,n_i
-00009030: 6e6e 6572 292c 2064 7479 7065 3d6d 7063  nner), dtype=mpc
-00009040: 290a 2020 2020 2020 2020 616c 7068 5b3a  ).        alph[:
-00009050: 2c3a 2d31 5d20 3d20 6a6e 5f6c 6c5b 3a2c  ,:-1] = jn_ll[:,
-00009060: 313a 5d2a 7964 5f6c 6c5b 3a2c 313a 5d20  1:]*yd_ll[:,1:] 
-00009070: 2d20 6a64 5f6c 6c5b 3a2c 313a 5d2a 796e  - jd_ll[:,1:]*yn
-00009080: 5f6c 6c5b 3a2c 313a 5d0a 2020 2020 2020  _ll[:,1:].      
-00009090: 2020 616c 7068 5b3a 2c2d 315d 203d 206a    alph[:,-1] = j
-000090a0: 6e5f 6578 2a79 645f 6578 202d 206a 645f  n_ex*yd_ex - jd_
-000090b0: 6578 2a79 6e5f 6578 0a20 2020 2020 2020  ex*yn_ex.       
-000090c0: 2062 6574 6120 3d20 6a6e 5f6c 6c2a 7964   beta = jn_ll*yd
-000090d0: 5f75 6c20 2d20 796e 5f75 6c2a 6a64 5f6c  _ul - yn_ul*jd_l
-000090e0: 6c0a 2020 2020 2020 2020 6761 6d6d 203d  l.        gamm =
-000090f0: 2079 6e5f 6c6c 2a79 645f 756c 202d 2079   yn_ll*yd_ul - y
-00009100: 6e5f 756c 2a79 645f 6c6c 0a20 2020 2020  n_ul*yd_ll.     
-00009110: 2020 2064 656c 7420 3d20 6a6e 5f75 6c2a     delt = jn_ul*
-00009120: 6a64 5f6c 6c20 2d20 6a6e 5f6c 6c2a 6a64  jd_ll - jn_ll*jd
-00009130: 5f75 6c0a 2020 2020 2020 2020 6570 7369  _ul.        epsi
-00009140: 203d 206a 6e5f 756c 2a79 645f 6c6c 202d   = jn_ul*yd_ll -
-00009150: 2079 6e5f 6c6c 2a6a 645f 756c 0a0a 2020   yn_ll*jd_ul..  
-00009160: 2020 2020 2020 2320 4d61 6b65 2074 6865        # Make the
-00009170: 2073 7068 6572 6963 616c 6c79 2073 796d   spherically sym
-00009180: 6d65 7472 6963 2072 6563 7572 7369 6f6e  metric recursion
-00009190: 3a0a 2020 2020 2020 2020 4c61 6d62 6420  :.        Lambd 
-000091a0: 3d20 6576 616c 5f69 6e6e 6572 5f72 6563  = eval_inner_rec
-000091b0: 7572 5f73 796d 286e 5f6d 6178 2c20 6e5f  ur_sym(n_max, n_
-000091c0: 6264 732c 2062 6574 612c 2067 616d 6d2c  bds, beta, gamm,
-000091d0: 2064 656c 742c 2065 7073 6929 0a0a 2020   delt, epsi)..  
-000091e0: 2020 2020 2020 2320 4576 616c 7561 7465        # Evaluate
-000091f0: 2074 6572 6d73 2066 6f72 2074 6865 206c   terms for the l
-00009200: 6179 6572 2073 6572 6965 733a 0a20 2020  ayer series:.   
-00009210: 2020 2020 2054 7261 6e73 6665 7251 7473       TransferQts
-00009220: 3120 3d20 286a 6e5f 6c6c 2c20 796e 5f6c  1 = (jn_ll, yn_l
-00009230: 6c2c 206a 6e5f 756c 2c20 796e 5f75 6c2c  l, jn_ul, yn_ul,
-00009240: 206a 645f 6c6c 2c20 7964 5f6c 6c2c 206b   jd_ll, yd_ll, k
-00009250: 725f 6578 2c20 6a6e 5f65 782c 2079 6e5f  r_ex, jn_ex, yn_
-00009260: 6578 2c20 616c 7068 2c20 6265 7461 2c20  ex, alph, beta, 
-00009270: 6761 6d6d 2c20 6465 6c74 2c20 6570 7369  gamm, delt, epsi
-00009280: 2c20 6465 6c74 512c 2065 7073 6951 2c20  , deltQ, epsiQ, 
-00009290: 4c61 6d62 6429 0a20 2020 2020 2020 2041  Lambd).        A
-000092a0: 742c 204b 6e2c 2061 4261 7220 3d20 6765  t, Kn, aBar = ge
-000092b0: 745f 7365 7269 6573 5f74 6572 6d73 286e  t_series_terms(n
-000092c0: 5f6d 6178 2c20 6e70 726d 5f6d 6178 2c20  _max, nprm_max, 
-000092d0: 6e2c 206e 5f62 6473 2c20 5472 616e 7366  n, n_bds, Transf
-000092e0: 6572 5174 7331 2c20 725f 6264 735b 2d31  erQts1, r_bds[-1
-000092f0: 5d2c 2042 656e 6d29 0a0a 2020 2020 2020  ], Benm)..      
-00009300: 2020 5472 616e 7366 6572 5174 7332 203d    TransferQts2 =
-00009310: 2028 6b72 5f6c 6c2c 206b 725f 756c 2c20   (kr_ll, kr_ul, 
-00009320: 6a6e 5f6c 6c2c 2079 6e5f 6c6c 2c20 4c61  jn_ll, yn_ll, La
-00009330: 6d62 6429 0a0a 2020 2020 656c 7365 3a0a  mbd)..    else:.
-00009340: 2020 2020 2020 2020 4c61 6d62 6420 3d20          Lambd = 
-00009350: 6e70 2e7a 6572 6f73 2828 6e5f 6d61 782c  np.zeros((n_max,
-00009360: 3129 2c20 6474 7970 653d 6d70 6329 0a20  1), dtype=mpc). 
-00009370: 2020 2020 2020 2041 7420 3d20 6e70 2e7a         At = np.z
-00009380: 6572 6f73 2828 6e5f 6d61 782c 3129 2c20  eros((n_max,1), 
-00009390: 6474 7970 653d 6d70 6329 0a20 2020 2020  dtype=mpc).     
-000093a0: 2020 204b 6e20 3d20 6e70 2e6f 6e65 7328     Kn = np.ones(
-000093b0: 286e 5f6d 6178 2c31 292c 2064 7479 7065  (n_max,1), dtype
-000093c0: 3d6d 7063 290a 2020 2020 2020 2020 6142  =mpc).        aB
-000093d0: 6172 203d 206e 702e 7a65 726f 7328 2832  ar = np.zeros((2
-000093e0: 2c6e 7072 6d5f 6d61 782b 312c 6e70 726d  ,nprm_max+1,nprm
-000093f0: 5f6d 6178 2b31 2c31 292c 2064 7479 7065  _max+1,1), dtype
-00009400: 3d6d 7063 2920 2023 2054 6869 7320 7769  =mpc)  # This wi
-00009410: 6c6c 206e 6f74 2062 6520 7573 6564 0a20  ll not be used. 
-00009420: 2020 2020 2020 2041 745b 3a2c 305d 203d         At[:,0] =
-00009430: 206a 6e5f 6578 2f64 656c 7451 0a20 2020   jn_ex/deltQ.   
-00009440: 2020 2020 2054 7261 6e73 6665 7251 7473       TransferQts
-00009450: 3220 3d20 286b 725f 6578 2c20 6b72 5f65  2 = (kr_ex, kr_e
-00009460: 782c 206a 6e5f 6578 2c20 796e 5f65 782c  x, jn_ex, yn_ex,
-00009470: 204c 616d 6264 2920 2023 2054 6865 7365   Lambd)  # These
-00009480: 2077 696c 6c20 6e6f 7420 6265 2075 7365   will not be use
-00009490: 640a 0a20 2020 2041 6420 3d20 2878 695f  d..    Ad = (xi_
-000094a0: 5f51 202b 204c 616d 6264 5b3a 6e70 726d  _Q + Lambd[:nprm
-000094b0: 5f6d 6178 2c6e 695f 6264 735d 2a72 686f  _max,ni_bds]*rho
-000094c0: 5f51 2920 2f20 2864 656c 7451 5b3a 6e70  _Q) / (deltQ[:np
-000094d0: 726d 5f6d 6178 5d20 2b20 4c61 6d62 645b  rm_max] + Lambd[
-000094e0: 3a6e 7072 6d5f 6d61 782c 6e69 5f62 6473  :nprm_max,ni_bds
-000094f0: 5d2a 6570 7369 515b 3a6e 7072 6d5f 6d61  ]*epsiQ[:nprm_ma
-00009500: 785d 290a 0a20 2020 206c 6f67 2e64 6562  x])..    log.deb
-00009510: 7567 2822 2020 2020 4361 6c63 756c 6174  ug("    Calculat
-00009520: 696e 6720 7365 7269 6573 2072 6573 756c  ing series resul
-00009530: 7473 2e2e 2e22 290a 0a20 2020 2023 2046  ts...")..    # F
-00009540: 696e 616c 6c79 2c20 6576 616c 7561 7465  inally, evaluate
-00009550: 2074 6865 2061 7379 6d6d 6574 7279 2073   the asymmetry s
-00009560: 6572 6965 7320 7465 726d 733a 0a20 2020  eries terms:.   
-00009570: 2044 656c 7461 203d 2067 6574 5f44 656c   Delta = get_Del
-00009580: 7461 6e6d 6928 6e5f 6d61 782c 2070 5f6d  tanmi(n_max, p_m
-00009590: 6178 2c20 6e70 726d 5f6d 6178 2c20 6e2c  ax, nprm_max, n,
-000095a0: 206e 5f62 6473 2c20 725f 6264 732c 2042   n_bds, r_bds, B
-000095b0: 656e 6d2c 2061 7379 6d5f 7368 6170 652c  enm, asym_shape,
-000095c0: 2058 6964 2c20 6142 6172 2c20 4164 2c20   Xid, aBar, Ad, 
-000095d0: 5472 616e 7366 6572 5174 7332 290a 0a20  TransferQts2).. 
-000095e0: 2020 2023 2041 6e64 2074 6865 2073 6572     # And the ser
-000095f0: 6965 7320 6974 7365 6c66 3a0a 2020 2020  ies itself:.    
-00009600: 414b 4473 6572 6965 7320 3d20 6e70 2e7a  AKDseries = np.z
-00009610: 6572 6f73 2828 322c 6e5f 6d61 782b 312c  eros((2,n_max+1,
-00009620: 6e5f 6d61 782b 3129 2c20 6474 7970 653d  n_max+1), dtype=
-00009630: 6d70 6329 0a20 2020 2066 6f72 2069 2069  mpc).    for i i
-00009640: 6e20 7261 6e67 6528 6e5f 6264 7329 3a0a  n range(n_bds):.
-00009650: 2020 2020 2020 2020 666f 7220 6e6e 2069          for nn i
-00009660: 6e20 7261 6e67 6528 312c 6e5f 6d61 782b  n range(1,n_max+
-00009670: 3129 3a0a 2020 2020 2020 2020 2020 2020  1):.            
-00009680: 6e69 203d 206e 6e20 2d20 310a 2020 2020  ni = nn - 1.    
-00009690: 2020 2020 2020 2020 414b 4473 6572 6965          AKDserie
-000096a0: 735b 3a2c 6e6e 2c3a 5d20 2b3d 2041 745b  s[:,nn,:] += At[
-000096b0: 6e69 2c69 5d20 2a20 4b6e 5b6e 692c 695d  ni,i] * Kn[ni,i]
-000096c0: 202a 2044 656c 7461 5b3a 2c6e 6e2c 3a2c   * Delta[:,nn,:,
-000096d0: 695d 0a0a 2020 2020 6966 2076 6572 626f  i]..    if verbo
-000096e0: 7365 3a0a 2020 2020 2020 2020 545f 6872  se:.        T_hr
-000096f0: 7320 3d20 726f 756e 6428 322a 6e70 2e70  s = round(2*np.p
-00009700: 692f 6f6d 6567 612f 3336 3030 2c20 3229  i/omega/3600, 2)
-00009710: 0a20 2020 2020 2020 206c 6f67 2e64 6562  .        log.deb
-00009720: 7567 2866 2220 2020 2045 7661 6c75 6174  ug(f"    Evaluat
-00009730: 696e 6720 6669 6e61 6c20 7072 6f64 7563  ing final produc
-00009740: 7473 2066 6f72 2054 203d 207b 545f 6872  ts for T = {T_hr
-00009750: 737d 2e2e 2e22 290a 0a20 2020 2023 2046  s}...")..    # F
-00009760: 696e 616c 6c79 2c20 7a69 7020 6974 2061  inally, zip it a
-00009770: 6c6c 2074 6f67 6574 6865 723a 0a20 2020  ll together:.   
-00009780: 2041 6520 3d20 6370 785f 6469 7628 2028   Ae = cpx_div( (
-00009790: 6265 7461 5120 2b20 4c61 6d62 645b 3a2c  betaQ + Lambd[:,
-000097a0: 2d31 5d20 2a20 6761 6d6d 5129 2c20 2864  -1] * gammQ), (d
-000097b0: 656c 7451 202b 204c 616d 6264 5b3a 2c2d  eltQ + Lambd[:,-
-000097c0: 315d 202a 2065 7073 6951 2920 290a 2020  1] * epsiQ) ).  
-000097d0: 2020 666f 7220 6e6e 2069 6e20 7261 6e67    for nn in rang
-000097e0: 6528 312c 6e5f 6d61 782b 3129 3a0a 2020  e(1,n_max+1):.  
-000097f0: 2020 2020 2020 6e69 203d 206e 6e20 2d20        ni = nn - 
-00009800: 310a 2020 2020 2020 2020 6e76 203d 206e  1.        nv = n
-00009810: 5b6e 695d 0a20 2020 2020 2020 2042 696e  [ni].        Bin
-00009820: 6d5b 3a2c 6e6e 2c3a 5d20 3d20 286e 762f  m[:,nn,:] = (nv/
-00009830: 286e 762b 6c6f 6e65 2920 2a20 4165 5b6e  (nv+lone) * Ae[n
-00009840: 695d 2a42 656e 6d5b 3a2c 6e6e 2c3a 5d20  i]*Benm[:,nn,:] 
-00009850: 2b20 6e76 2a41 4b44 7365 7269 6573 5b3a  + nv*AKDseries[:
-00009860: 2c6e 6e2c 3a5d 2920 2a20 7273 6361 6c69  ,nn,:]) * rscali
-00009870: 6e67 2a2a 286e 6e2b 3229 0a0a 2020 2020  ng**(nn+2)..    
-00009880: 6966 2064 6562 7567 3a0a 2020 2020 2020  if debug:.      
-00009890: 2020 7265 7475 726e 2042 696e 6d2c 2041    return Binm, A
-000098a0: 652c 2041 742c 2041 642c 206b 725f 6578  e, At, Ad, kr_ex
-000098b0: 0a20 2020 2065 6c73 653a 0a20 2020 2020  .    else:.     
-000098c0: 2020 2072 6574 7572 6e20 4269 6e6d 0a0a     return Binm..
-000098d0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000098e0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-000098f0: 2323 2323 2323 2323 2323 2323 230a 0a22  #############.."
-00009900: 2222 0a67 6574 5f73 6572 6965 735f 7465  "".get_series_te
-00009910: 726d 7328 290a 2020 2020 4361 6c63 756c  rms().    Calcul
-00009920: 6174 6520 7175 616e 7469 7469 6573 2074  ate quantities t
-00009930: 6861 7420 6170 7065 6172 2069 6e20 7375  hat appear in su
-00009940: 6d73 206f 7665 7220 6c61 7965 7273 2e0a  ms over layers..
-00009950: 2020 2020 5573 6167 653a 2060 4174 602c      Usage: `At`,
-00009960: 2060 4b6e 602c 2060 6142 6172 6020 3d20   `Kn`, `aBar` = 
-00009970: 6765 745f 7365 7269 6573 5f74 6572 6d73  get_series_terms
-00009980: 2860 6e5f 6d61 7860 2c20 606e 7072 6d5f  (`n_max`, `nprm_
-00009990: 6d61 7860 2c20 606e 602c 2060 6e5f 6264  max`, `n`, `n_bd
-000099a0: 7360 2c20 6054 7261 6e73 6665 7251 7473  s`, `TransferQts
-000099b0: 602c 2060 5260 2c20 6042 656e 6d60 290a  `, `R`, `Benm`).
-000099c0: 2020 2020 5265 7475 726e 733a 0a20 2020      Returns:.   
-000099d0: 2020 2020 2041 743a 206d 7063 2c20 7368       At: mpc, sh
-000099e0: 6170 6528 6e5f 6d61 782c 6e5f 6264 7329  ape(n_max,n_bds)
-000099f0: 2e20 5363 616c 696e 6720 616d 706c 6974  . Scaling amplit
-00009a00: 7564 6520 6465 7465 726d 696e 696e 6720  ude determining 
-00009a10: 7468 6520 7374 7265 6e67 7468 206f 6620  the strength of 
-00009a20: 696e 6475 6365 6420 6669 656c 6420 6672  induced field fr
-00009a30: 6f6d 2065 6163 6820 6c61 7965 722e 0a20  om each layer.. 
-00009a40: 2020 2020 2020 2020 2020 2054 6869 7320             This 
-00009a50: 6973 205c 6d61 7468 6361 6c7b 417d 5f6e  is \mathcal{A}_n
-00009a60: 5e7b 742c 697d 2069 6e20 7468 6520 7061  ^{t,i} in the pa
-00009a70: 7065 722e 0a20 2020 2020 2020 204b 6e3a  per..        Kn:
-00009a80: 206d 7063 2c20 7368 6170 6528 6e5f 6d61   mpc, shape(n_ma
-00009a90: 782c 6e5f 6264 7329 2e20 5472 616e 7366  x,n_bds). Transf
-00009aa0: 6572 2070 726f 6475 6374 2070 726f 7061  er product propa
-00009ab0: 6761 7469 6e67 2069 6e64 7563 6564 206d  gating induced m
-00009ac0: 6f6d 656e 7473 2072 6573 756c 7469 6e67  oments resulting
-00009ad0: 0a20 2020 2020 2020 2020 2020 2066 726f  .            fro
-00009ae0: 6d20 6173 796d 6d65 7472 7920 6672 6f6d  m asymmetry from
-00009af0: 2074 6865 2061 7379 6d6d 6574 7269 6320   the asymmetric 
-00009b00: 6c61 7965 7220 746f 2074 6865 206f 7574  layer to the out
-00009b10: 6572 6d6f 7374 2062 6f75 6e64 6172 792e  ermost boundary.
-00009b20: 2054 6869 7320 6973 204b 5f6e 5e69 2069   This is K_n^i i
-00009b30: 6e20 7468 6520 7061 7065 722e 0a20 2020  n the paper..   
-00009b40: 2020 2020 2061 4261 723a 206d 7063 2c20       aBar: mpc, 
-00009b50: 7368 6170 6528 322c 6e70 726d 5f6d 6178  shape(2,nprm_max
-00009b60: 2b31 2c6e 7072 6d5f 6d61 782b 312c 6e5f  +1,nprm_max+1,n_
-00009b70: 6264 7329 2e20 536f 6c75 7469 6f6e 7320  bds). Solutions 
-00009b80: 666f 7220 7468 6520 4265 7373 656c 2066  for the Bessel f
-00009b90: 756e 6374 696f 6e20 636f 6566 6669 6369  unction coeffici
-00009ba0: 656e 7473 0a20 2020 2020 2020 2020 2020  ents.           
-00009bb0: 2061 5e69 5f7b 6e27 6d27 7d20 666f 7220   a^i_{n'm'} for 
-00009bc0: 7468 6520 6361 7365 206f 6620 7370 6865  the case of sphe
-00009bd0: 7269 6361 6c20 7379 6d6d 6574 7279 2e20  rical symmetry. 
-00009be0: 5468 6973 2069 7320 5c6f 7665 726c 696e  This is \overlin
-00009bf0: 657b 617d 5e5c 6d61 7468 726d 7b69 7d5f  e{a}^\mathrm{i}_
-00009c00: 7b6e 276d 277d 2069 6e20 7468 6520 7061  {n'm'} in the pa
-00009c10: 7065 722e 0a20 2020 2050 6172 616d 6574  per..    Paramet
-00009c20: 6572 733a 0a20 2020 2020 2020 206e 5f6d  ers:.        n_m
-00009c30: 6178 3a20 696e 7465 6765 722e 204d 6178  ax: integer. Max
-00009c40: 696d 756d 2064 6567 7265 6520 6e20 6f66  imum degree n of
-00009c50: 2069 6e64 7563 6564 206d 6f6d 656e 7473   induced moments
-00009c60: 2e0a 2020 2020 2020 2020 6e70 726d 5f6d  ..        nprm_m
-00009c70: 6178 3a20 696e 7465 6765 722e 204d 6178  ax: integer. Max
-00009c80: 696d 756d 2064 6567 7265 6520 6e27 206f  imum degree n' o
-00009c90: 6620 6578 6369 7461 7469 6f6e 206d 6f6d  f excitation mom
-00009ca0: 656e 7473 2e0a 2020 2020 2020 2020 6e3a  ents..        n:
-00009cb0: 206d 7066 2c20 7368 6170 6528 6e5f 6d61   mpf, shape(n_ma
-00009cc0: 7829 2e20 496e 7465 6765 7220 7661 6c75  x). Integer valu
-00009cd0: 6573 206f 6620 6e20 696e 206d 706d 6174  es of n in mpmat
-00009ce0: 6820 666c 6f61 7420 666f 726d 6174 2e0a  h float format..
-00009cf0: 2020 2020 2020 2020 6e5f 6264 733a 2069          n_bds: i
-00009d00: 6e74 6567 6572 2e20 4e75 6d62 6572 206f  nteger. Number o
-00009d10: 6620 626f 756e 6461 7269 6573 2070 7265  f boundaries pre
-00009d20: 7365 6e74 2069 6e20 7468 6520 696e 7465  sent in the inte
-00009d30: 7269 6f72 206d 6f64 656c 2e0a 2020 2020  rior model..    
-00009d40: 2020 2020 5472 616e 7366 6572 5174 733a      TransferQts:
-00009d50: 2054 7570 6c65 206f 6620 4265 7373 656c   Tuple of Bessel
-00009d60: 2066 756e 6374 696f 6e73 2061 6e64 2076   functions and v
-00009d70: 6172 696f 7573 2071 7561 6e74 6974 6965  arious quantitie
-00009d80: 7320 7573 696e 6720 7468 656d 2c20 616c  s using them, al
-00009d90: 6c20 6f66 2074 7970 6520 6d70 632e 2053  l of type mpc. S
-00009da0: 6565 2042 696e 6d52 6573 706f 6e73 652e  ee BinmResponse.
-00009db0: 0a20 2020 2020 2020 2052 3a20 666c 6f61  .        R: floa
-00009dc0: 742e 2052 6164 6975 7320 6f66 2074 6865  t. Radius of the
-00009dd0: 206f 7574 6572 6d6f 7374 2063 6f6e 6475   outermost condu
-00009de0: 6374 696e 6720 626f 756e 6461 7279 2069  cting boundary i
-00009df0: 6e20 6d2e 0a20 2020 2020 2020 2042 656e  n m..        Ben
-00009e00: 6d3a 206d 7063 2c20 7368 6170 6528 322c  m: mpc, shape(2,
-00009e10: 6e70 726d 5f6d 6178 2b31 2c6e 7072 6d5f  nprm_max+1,nprm_
-00009e20: 6d61 782b 3129 2e20 436f 6d70 6c65 7820  max+1). Complex 
-00009e30: 616d 706c 6974 7564 6573 206f 6620 6578  amplitudes of ex
-00009e40: 6369 7461 7469 6f6e 206d 6f6d 656e 7473  citation moments
-00009e50: 2066 6f72 2074 6869 7320 7065 7269 6f64   for this period
-00009e60: 2e0a 2020 2020 2222 220a 6465 6620 6765  ..    """.def ge
-00009e70: 745f 7365 7269 6573 5f74 6572 6d73 286e  t_series_terms(n
-00009e80: 5f6d 6178 2c20 6e70 726d 5f6d 6178 2c20  _max, nprm_max, 
-00009e90: 6e2c 206e 5f62 6473 2c20 5472 616e 7366  n, n_bds, Transf
-00009ea0: 6572 5174 732c 2052 2c20 4265 6e6d 293a  erQts, R, Benm):
-00009eb0: 0a20 2020 206d 7063 203d 206d 7063 5f67  .    mpc = mpc_g
-00009ec0: 6c6f 6261 6c0a 2020 2020 6c6f 6e65 203d  lobal.    lone =
-00009ed0: 206f 6e65 0a20 2020 206c 7477 6f20 3d20   one.    ltwo = 
-00009ee0: 7477 6f0a 2020 2020 6e5f 696e 6e65 7220  two.    n_inner 
-00009ef0: 3d20 6e5f 6264 7320 2d20 310a 2020 2020  = n_bds - 1.    
-00009f00: 6a6e 5f6c 6c2c 2079 6e5f 6c6c 2c20 6a6e  jn_ll, yn_ll, jn
-00009f10: 5f75 6c2c 2079 6e5f 756c 2c20 6a64 5f6c  _ul, yn_ul, jd_l
-00009f20: 6c2c 2079 645f 6c6c 2c20 6b72 5f65 782c  l, yd_ll, kr_ex,
-00009f30: 206a 6e5f 6578 2c20 796e 5f65 782c 2061   jn_ex, yn_ex, a
-00009f40: 6c70 682c 2062 6574 612c 2067 616d 6d2c  lph, beta, gamm,
-00009f50: 2064 656c 742c 2065 7073 692c 2064 656c   delt, epsi, del
-00009f60: 7451 2c20 6570 7369 512c 204c 616d 6264  tQ, epsiQ, Lambd
-00009f70: 203d 2054 7261 6e73 6665 7251 7473 0a0a   = TransferQts..
-00009f80: 2020 2020 4174 2c20 4b6e 203d 2028 206e      At, Kn = ( n
-00009f90: 702e 6f6e 6573 2828 6e5f 6d61 782c 6e5f  p.ones((n_max,n_
-00009fa0: 6264 7329 2c20 6474 7970 653d 6d70 6329  bds), dtype=mpc)
-00009fb0: 2066 6f72 205f 2069 6e20 7261 6e67 6528   for _ in range(
-00009fc0: 3229 2029 0a20 2020 2061 4261 7220 3d20  2) ).    aBar = 
-00009fd0: 6e70 2e7a 6572 6f73 2828 322c 6e70 726d  np.zeros((2,nprm
-00009fe0: 5f6d 6178 2b31 2c6e 7072 6d5f 6d61 782b  _max+1,nprm_max+
-00009ff0: 312c 6e5f 6264 7329 2c20 6474 7970 653d  1,n_bds), dtype=
-0000a000: 6d70 6329 0a0a 2020 2020 6465 6e6f 6d20  mpc)..    denom 
-0000a010: 3d20 6465 6c74 5120 2b20 4c61 6d62 645b  = deltQ + Lambd[
-0000a020: 3a2c 2d31 5d20 2a20 6570 7369 510a 0a20  :,-1] * epsiQ.. 
-0000a030: 2020 2061 4261 7242 6173 6520 3d20 2d52     aBarBase = -R
-0000a040: 2a42 656e 6d5b 3a2c 3a6e 7072 6d5f 6d61  *Benm[:,:nprm_ma
-0000a050: 782b 312c 3a6e 7072 6d5f 6d61 782b 315d  x+1,:nprm_max+1]
-0000a060: 0a20 2020 2066 6f72 206e 6e70 2069 6e20  .    for nnp in 
-0000a070: 7261 6e67 6528 312c 206e 7072 6d5f 6d61  range(1, nprm_ma
-0000a080: 782b 3129 3a0a 2020 2020 2020 2020 6e76  x+1):.        nv
-0000a090: 203d 206e 5b6e 6e70 2d31 5d0a 2020 2020   = n[nnp-1].    
-0000a0a0: 2020 2020 666f 7220 6d6d 7020 696e 2072      for mmp in r
-0000a0b0: 616e 6765 282d 6e6e 702c 6e6e 702b 3129  ange(-nnp,nnp+1)
-0000a0c0: 3a0a 2020 2020 2020 2020 2020 2020 6d70  :.            mp
-0000a0d0: 7369 676e 203d 2069 6e74 286d 6d70 3c30  sign = int(mmp<0
-0000a0e0: 290a 2020 2020 2020 2020 2020 2020 6d70  ).            mp
-0000a0f0: 6162 7320 3d20 6162 7328 6d6d 7029 0a20  abs = abs(mmp). 
-0000a100: 2020 2020 2020 2020 2020 2061 4261 725b             aBar[
-0000a110: 6d70 7369 676e 2c6e 6e70 2c6d 7061 6273  mpsign,nnp,mpabs
-0000a120: 2c2d 315d 203d 2063 7078 5f64 6976 5f76  ,-1] = cpx_div_v
-0000a130: 616c 2820 6142 6172 4261 7365 5b6d 7073  al( aBarBase[mps
-0000a140: 6967 6e2c 6e6e 702c 6d70 6162 735d 202a  ign,nnp,mpabs] *
-0000a150: 2028 6c74 776f 2a6e 7620 2b20 6c6f 6e65   (ltwo*nv + lone
-0000a160: 292f 286e 7620 2b20 6c6f 6e65 292c 2064  )/(nv + lone), d
-0000a170: 656e 6f6d 5b6e 6e70 2d31 5d20 290a 0a20  enom[nnp-1] ).. 
-0000a180: 2020 2041 745b 3a2c 2d31 5d20 3d20 6e20     At[:,-1] = n 
-0000a190: 2a20 286a 6e5f 6578 202b 204c 616d 6264  * (jn_ex + Lambd
-0000a1a0: 5b3a 2c2d 315d 2a79 6e5f 6578 2920 2f20  [:,-1]*yn_ex) / 
-0000a1b0: 6465 6e6f 6d0a 2020 2020 666f 7220 6920  denom.    for i 
-0000a1c0: 696e 2072 616e 6765 286e 5f69 6e6e 6572  in range(n_inner
-0000a1d0: 2d31 2c20 2d31 2c20 2d31 293a 0a20 2020  -1, -1, -1):.   
-0000a1e0: 2020 2020 2041 745b 3a2c 695d 203d 2063       At[:,i] = c
-0000a1f0: 7078 5f64 6976 2820 286a 6e5f 6c6c 5b3a  px_div( (jn_ll[:
-0000a200: 2c69 5d20 2b20 4c61 6d62 645b 3a2c 695d  ,i] + Lambd[:,i]
-0000a210: 2a79 6e5f 6c6c 5b3a 2c69 5d29 2c20 6465  *yn_ll[:,i]), de
-0000a220: 6e6f 6d29 0a0a 2020 2020 2020 2020 4b6e  nom)..        Kn
-0000a230: 5b3a 2c69 5d20 3d20 6370 785f 6469 7628  [:,i] = cpx_div(
-0000a240: 2028 4b6e 5b3a 2c69 2b31 5d20 2a20 616c   (Kn[:,i+1] * al
-0000a250: 7068 5b3a 2c69 5d29 2c20 2862 6574 615b  ph[:,i]), (beta[
-0000a260: 3a2c 695d 202b 204c 616d 6264 5b3a 2c69  :,i] + Lambd[:,i
-0000a270: 5d2a 6761 6d6d 5b3a 2c69 5d29 2029 0a0a  ]*gamm[:,i]) )..
-0000a280: 2020 2020 2020 2020 666f 7220 6e6e 7020          for nnp 
-0000a290: 696e 2072 616e 6765 2831 2c6e 7072 6d5f  in range(1,nprm_
-0000a2a0: 6d61 782b 3129 3a0a 2020 2020 2020 2020  max+1):.        
-0000a2b0: 2020 2020 6e70 6920 3d20 6e6e 7020 2d31      npi = nnp -1
-0000a2c0: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
-0000a2d0: 206d 6d70 2069 6e20 7261 6e67 6528 2d6e   mmp in range(-n
-0000a2e0: 6e70 2c6e 6e70 2b31 293a 0a20 2020 2020  np,nnp+1):.     
-0000a2f0: 2020 2020 2020 2020 2020 206d 7073 6967             mpsig
-0000a300: 6e20 3d20 696e 7428 6d6d 7020 3c20 3029  n = int(mmp < 0)
-0000a310: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000a320: 206d 7061 6273 203d 2061 6273 286d 6d70   mpabs = abs(mmp
-0000a330: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0000a340: 2020 6142 6172 5b6d 7073 6967 6e2c 6e6e    aBar[mpsign,nn
-0000a350: 702c 6d70 6162 732c 695d 203d 2063 7078  p,mpabs,i] = cpx
-0000a360: 5f64 6976 5f76 616c 2820 2861 4261 725b  _div_val( (aBar[
-0000a370: 6d70 7369 676e 2c6e 6e70 2c6d 7061 6273  mpsign,nnp,mpabs
-0000a380: 2c69 2b31 5d20 2a20 286a 6e5f 756c 5b6e  ,i+1] * (jn_ul[n
-0000a390: 7069 2c69 5d20 2b20 4c61 6d62 645b 6e70  pi,i] + Lambd[np
-0000a3a0: 692c 692b 315d 2a79 6e5f 756c 5b6e 7069  i,i+1]*yn_ul[npi
-0000a3b0: 2c69 5d29 292c 2028 6a6e 5f6c 6c5b 6e70  ,i])), (jn_ll[np
-0000a3c0: 692c 695d 202b 204c 616d 6264 5b6e 7069  i,i] + Lambd[npi
-0000a3d0: 2c69 5d2a 796e 5f6c 6c5b 6e70 692c 695d  ,i]*yn_ll[npi,i]
-0000a3e0: 2920 290a 0a20 2020 2072 6574 7572 6e20  ) )..    return 
-0000a3f0: 4174 2c20 4b6e 2c20 6142 6172 0a0a 2323  At, Kn, aBar..##
-0000a400: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0000a410: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0000a420: 2323 2323 2323 2323 2323 230a 0a22 2222  ###########.."""
-0000a430: 0a67 6574 5f44 656c 7461 6e6d 6928 290a  .get_Deltanmi().
-0000a440: 2020 2020 4361 6c63 756c 6174 6520 4465      Calculate De
-0000a450: 6c74 612c 2077 6869 6368 2072 6570 7265  lta, which repre
-0000a460: 7365 6e74 7320 7468 6520 616d 6f75 6e74  sents the amount
-0000a470: 206f 6620 226d 6978 696e 6722 2066 726f   of "mixing" fro
-0000a480: 6d20 6578 6369 7461 7469 6f6e 206d 6f6d  m excitation mom
-0000a490: 656e 7473 2069 6e74 6f0a 2020 2020 2020  ents into.      
-0000a4a0: 2020 696e 6475 6365 6420 6d6f 6d65 6e74    induced moment
-0000a4b0: 7320 6f66 206f 7468 6572 206e 2c6d 2064  s of other n,m d
-0000a4c0: 7565 2074 6f20 6173 796d 6d65 7472 792e  ue to asymmetry.
-0000a4d0: 0a20 2020 2055 7361 6765 3a20 6044 656c  .    Usage: `Del
-0000a4e0: 7461 6020 3d20 6765 745f 4465 6c74 616e  ta` = get_Deltan
-0000a4f0: 6d69 2860 6e5f 6d61 7860 2c20 6070 5f6d  mi(`n_max`, `p_m
-0000a500: 6178 602c 2060 6e70 726d 5f6d 6178 602c  ax`, `nprm_max`,
-0000a510: 2060 6e60 2c20 606e 5f62 6473 602c 2060   `n`, `n_bds`, `
-0000a520: 725f 6264 7360 2c20 6042 656e 6d60 2c20  r_bds`, `Benm`, 
-0000a530: 6061 7379 6d5f 7368 6170 6560 2c20 6058  `asym_shape`, `X
-0000a540: 6964 602c 2060 6142 6172 602c 2060 4164  id`, `aBar`, `Ad
-0000a550: 602c 2060 5472 616e 7366 6572 5174 7360  `, `TransferQts`
-0000a560: 290a 2020 2020 5265 7475 726e 733a 0a20  ).    Returns:. 
-0000a570: 2020 2020 2020 2044 656c 7461 3a20 6d70         Delta: mp
-0000a580: 632c 2073 6861 7065 2832 2c6e 5f6d 6178  c, shape(2,n_max
-0000a590: 2b31 2c6e 5f6d 6178 2b31 2c6e 5f62 6473  +1,n_max+1,n_bds
-0000a5a0: 292e 2054 6869 7320 6973 205c 4465 6c74  ). This is \Delt
-0000a5b0: 615e 5c6d 6174 6872 6d7b 697d 5f7b 6e6d  a^\mathrm{i}_{nm
-0000a5c0: 7d20 696e 2074 6865 2070 6170 6572 2e0a  } in the paper..
-0000a5d0: 2020 2020 5061 7261 6d65 7465 7273 3a0a      Parameters:.
-0000a5e0: 2020 2020 2020 2020 6e5f 6d61 783a 2069          n_max: i
-0000a5f0: 6e74 6567 6572 2e20 4d61 7869 6d75 6d20  nteger. Maximum 
-0000a600: 6465 6772 6565 206e 206f 6620 696e 6475  degree n of indu
-0000a610: 6365 6420 6d6f 6d65 6e74 732e 0a20 2020  ced moments..   
-0000a620: 2020 2020 2070 5f6d 6178 3a20 696e 7465       p_max: inte
-0000a630: 6765 722e 204c 6172 6765 7374 2064 6567  ger. Largest deg
-0000a640: 7265 6520 7020 696e 2069 6e74 6572 696f  ree p in interio
-0000a650: 7220 6d6f 6465 6c20 626f 756e 6461 7279  r model boundary
-0000a660: 2073 6861 7065 732e 0a20 2020 2020 2020   shapes..       
-0000a670: 206e 7072 6d5f 6d61 783a 2069 6e74 6567   nprm_max: integ
-0000a680: 6572 2e20 4d61 7869 6d75 6d20 6465 6772  er. Maximum degr
-0000a690: 6565 206e 2720 6f66 2065 7863 6974 6174  ee n' of excitat
-0000a6a0: 696f 6e20 6d6f 6d65 6e74 732e 0a20 2020  ion moments..   
-0000a6b0: 2020 2020 206e 3a20 6d70 662c 2073 6861       n: mpf, sha
-0000a6c0: 7065 286e 5f6d 6178 292e 2049 6e74 6567  pe(n_max). Integ
-0000a6d0: 6572 2076 616c 7565 7320 6f66 206e 2069  er values of n i
-0000a6e0: 6e20 6d70 6d61 7468 2066 6c6f 6174 2066  n mpmath float f
-0000a6f0: 6f72 6d61 742e 0a20 2020 2020 2020 206e  ormat..        n
-0000a700: 5f62 6473 3a20 696e 7465 6765 722e 204e  _bds: integer. N
-0000a710: 756d 6265 7220 6f66 2062 6f75 6e64 6172  umber of boundar
-0000a720: 6965 7320 7072 6573 656e 7420 696e 2074  ies present in t
-0000a730: 6865 2069 6e74 6572 696f 7220 6d6f 6465  he interior mode
-0000a740: 6c2e 0a20 2020 2020 2020 2072 5f62 6473  l..        r_bds
-0000a750: 3a20 666c 6f61 742c 2073 6861 7065 286e  : float, shape(n
-0000a760: 5f62 6473 292e 2052 6164 6969 2066 6f72  _bds). Radii for
-0000a770: 2065 6163 6820 626f 756e 6461 7279 2073   each boundary s
-0000a780: 7572 6661 6365 2069 6e20 6d2e 0a20 2020  urface in m..   
-0000a790: 2020 2020 2042 656e 6d3a 2063 6f6d 706c       Benm: compl
-0000a7a0: 6578 2c20 7368 6170 6528 322c 6e5f 6d61  ex, shape(2,n_ma
-0000a7b0: 782b 312c 6e5f 6d61 782b 3129 2e20 436f  x+1,n_max+1). Co
-0000a7c0: 6d70 6c65 7820 6578 6369 7461 7469 6f6e  mplex excitation
-0000a7d0: 206d 6f6d 656e 7473 2066 6f72 2074 6869   moments for thi
-0000a7e0: 7320 7065 7269 6f64 0a20 2020 2020 2020  s period.       
-0000a7f0: 2020 2020 206f 6620 6f73 6369 6c6c 6174       of oscillat
-0000a800: 696f 6e2e 2054 6869 7320 6973 2042 5e7b  ion. This is B^{
-0000a810: 657d 5f7b 6e6d 7d20 696e 2074 6865 2070  e}_{nm} in the p
-0000a820: 6170 6572 2e0a 2020 2020 2020 2020 6173  aper..        as
-0000a830: 796d 5f73 6861 7065 3a20 636f 6d70 6c65  ym_shape: comple
-0000a840: 782c 2073 6861 7065 286e 5f62 6473 2c32  x, shape(n_bds,2
-0000a850: 2c70 5f6d 6178 2b31 2c70 5f6d 6178 2b31  ,p_max+1,p_max+1
-0000a860: 292e 2041 206c 6973 7420 6f66 2062 6f75  ). A list of bou
-0000a870: 6e64 6172 7920 7368 6170 6520 7061 7261  ndary shape para
-0000a880: 6d65 7465 7273 2063 6869 5f70 7120 666f  meters chi_pq fo
-0000a890: 7220 6561 6368 2062 6f75 6e64 6172 792e  r each boundary.
-0000a8a0: 0a20 2020 2020 2020 2058 6964 3a20 6d70  .        Xid: mp
-0000a8b0: 662c 2073 6861 7065 2832 2c6e 7072 6d5f  f, shape(2,nprm_
-0000a8c0: 6d61 782b 312c 6e70 726d 5f6d 6178 2b31  max+1,nprm_max+1
-0000a8d0: 2c20 322c 705f 6d61 782b 312c 705f 6d61  , 2,p_max+1,p_ma
-0000a8e0: 782b 312c 2032 2c6e 5f6d 6178 2b31 2c6e  x+1, 2,n_max+1,n
-0000a8f0: 5f6d 6178 2b31 292e 204d 6978 696e 6720  _max+1). Mixing 
-0000a900: 636f 6566 6669 6369 656e 7473 0a20 2020  coefficients.   
-0000a910: 2020 2020 2020 2020 2072 6573 756c 7469           resulti
-0000a920: 6e67 2066 726f 6d20 6d75 6c74 6970 6c69  ng from multipli
-0000a930: 6361 7469 6f6e 206f 6620 7370 6865 7269  cation of spheri
-0000a940: 6361 6c20 6861 726d 6f6e 6963 732e 205c  cal harmonics. \
-0000a950: 5869 5e7b 5c73 7461 7220 6e6d 7d5f 7b6e  Xi^{\star nm}_{n
-0000a960: 276d 2770 717d 2066 726f 6d20 7468 6520  'm'pq} from the 
-0000a970: 7061 7065 722e 0a20 2020 2020 2020 2061  paper..        a
-0000a980: 4261 723a 206d 7063 2c20 7368 6170 6528  Bar: mpc, shape(
-0000a990: 6e5f 6264 732c 322c 6e5f 6d61 782b 312c  n_bds,2,n_max+1,
-0000a9a0: 6e5f 6d61 782b 3129 2e20 436f 6d70 6c65  n_max+1). Comple
-0000a9b0: 7820 636f 6566 6669 6369 656e 7473 2066  x coefficients f
-0000a9c0: 6f72 2074 6865 2069 6e74 6572 6e61 6c20  or the internal 
-0000a9d0: 6d61 676e 6574 6963 2066 6965 6c64 2066  magnetic field f
-0000a9e0: 726f 6d20 7468 650a 2020 2020 2020 2020  rom the.        
-0000a9f0: 2020 2020 7370 6865 7269 6361 6c6c 7920      spherically 
-0000aa00: 7379 6d6d 6574 7269 6320 736f 6c75 7469  symmetric soluti
-0000aa10: 6f6e 732e 2054 6869 7320 6973 205c 6f76  ons. This is \ov
-0000aa20: 6572 6c69 6e65 7b61 7d5e 5c6d 6174 6872  erline{a}^\mathr
-0000aa30: 6d7b 697d 5f7b 6e27 6d27 7d20 6672 6f6d  m{i}_{n'm'} from
-0000aa40: 2074 6865 2070 6170 6572 2e0a 2020 2020   the paper..    
-0000aa50: 2020 2020 4164 3a20 6d70 632c 2073 6861      Ad: mpc, sha
-0000aa60: 7065 286e 7072 6d5f 6d61 7829 2e20 436f  pe(nprm_max). Co
-0000aa70: 6d70 6c65 7820 616d 706c 6974 7564 6520  mplex amplitude 
-0000aa80: 6d69 7869 6e67 2066 726f 6d20 7468 6520  mixing from the 
-0000aa90: 6578 6369 7461 7469 6f6e 2068 6172 6d6f  excitation harmo
-0000aaa0: 6e69 6373 2069 6e74 6f20 7468 6520 0a20  nics into the . 
-0000aab0: 2020 2020 2020 2020 2020 2069 6e64 7563             induc
-0000aac0: 6564 2068 6172 6d6f 6e69 6373 2e20 5468  ed harmonics. Th
-0000aad0: 6973 2069 7320 5c6d 6174 6863 616c 7b41  is is \mathcal{A
-0000aae0: 7d5e 7b5c 7374 6172 7d5f 7b6e 277d 2066  }^{\star}_{n'} f
-0000aaf0: 726f 6d20 7468 6520 7061 7065 722e 0a20  rom the paper.. 
-0000ab00: 2020 2022 2222 0a64 6566 2067 6574 5f44     """.def get_D
-0000ab10: 656c 7461 6e6d 6928 6e5f 6d61 782c 2070  eltanmi(n_max, p
-0000ab20: 5f6d 6178 2c20 6e70 726d 5f6d 6178 2c20  _max, nprm_max, 
-0000ab30: 6e2c 206e 5f62 6473 2c20 725f 6264 732c  n, n_bds, r_bds,
-0000ab40: 2042 656e 6d2c 2061 7379 6d5f 7368 6170   Benm, asym_shap
-0000ab50: 652c 2058 6964 2c20 6142 6172 2c20 4164  e, Xid, aBar, Ad
-0000ab60: 2c20 5472 616e 7366 6572 5174 7329 3a0a  , TransferQts):.
-0000ab70: 2020 2020 6d70 6320 3d20 6d70 635f 676c      mpc = mpc_gl
-0000ab80: 6f62 616c 0a20 2020 206c 6f6e 6520 3d20  obal.    lone = 
-0000ab90: 6f6e 650a 2020 2020 6c74 776f 203d 2074  one.    ltwo = t
-0000aba0: 776f 0a20 2020 2044 656c 7461 203d 206e  wo.    Delta = n
-0000abb0: 702e 7a65 726f 7328 2832 2c6e 5f6d 6178  p.zeros((2,n_max
-0000abc0: 2b31 2c6e 5f6d 6178 2b31 2c6e 5f62 6473  +1,n_max+1,n_bds
-0000abd0: 292c 2064 7479 7065 3d6d 7063 290a 2020  ), dtype=mpc).  
-0000abe0: 2020 6b72 5f6c 6c2c 206b 725f 756c 2c20    kr_ll, kr_ul, 
-0000abf0: 6a6e 5f6c 6c2c 2079 6e5f 6c6c 2c20 4c61  jn_ll, yn_ll, La
-0000ac00: 6d62 6420 3d20 5472 616e 7366 6572 5174  mbd = TransferQt
-0000ac10: 730a 2020 2020 6d69 7873 756d 5f69 6e69  s.    mixsum_ini
-0000ac20: 7420 3d20 6e70 2e7a 6572 6f73 2828 322c  t = np.zeros((2,
-0000ac30: 6e70 726d 5f6d 6178 2b31 2c6e 7072 6d5f  nprm_max+1,nprm_
-0000ac40: 6d61 782b 312c 2032 2c6e 5f6d 6178 2b31  max+1, 2,n_max+1
-0000ac50: 2c6e 5f6d 6178 2b31 2c20 6e5f 6264 7329  ,n_max+1, n_bds)
-0000ac60: 2c20 6474 7970 653d 6d70 6329 0a0a 2020  , dtype=mpc)..  
-0000ac70: 2020 666f 7220 6e6e 2069 6e20 7261 6e67    for nn in rang
-0000ac80: 6528 312c 6e5f 6d61 782b 3129 3a0a 2020  e(1,n_max+1):.  
-0000ac90: 2020 2020 2020 6e69 203d 206e 6e20 2d20        ni = nn - 
-0000aca0: 310a 2020 2020 2020 2020 6e76 203d 206e  1.        nv = n
-0000acb0: 5b6e 695d 0a20 2020 2020 2020 2066 6f72  [ni].        for
-0000acc0: 206d 6d20 696e 2072 616e 6765 282d 6e6e   mm in range(-nn
-0000acd0: 2c6e 6e2b 3129 3a0a 2020 2020 2020 2020  ,nn+1):.        
-0000ace0: 2020 2020 6d73 6967 6e20 3d20 696e 7428      msign = int(
-0000acf0: 6d6d 3c30 290a 2020 2020 2020 2020 2020  mm<0).          
-0000ad00: 2020 6d61 6273 203d 2061 6273 286d 6d29    mabs = abs(mm)
-0000ad10: 0a0a 2020 2020 2020 2020 2020 2020 666f  ..            fo
-0000ad20: 7220 6e6e 7020 696e 2072 616e 6765 2831  r nnp in range(1
-0000ad30: 2c6e 7072 6d5f 6d61 782b 3129 3a0a 2020  ,nprm_max+1):.  
-0000ad40: 2020 2020 2020 2020 2020 2020 2020 6e70                np
-0000ad50: 6920 3d20 6e6e 7020 2d20 310a 2020 2020  i = nnp - 1.    
-0000ad60: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-0000ad70: 6d6d 7020 696e 2072 616e 6765 282d 6e6e  mmp in range(-nn
-0000ad80: 702c 6e6e 702b 3129 3a0a 2020 2020 2020  p,nnp+1):.      
-0000ad90: 2020 2020 2020 2020 2020 2020 2020 6d70                mp
-0000ada0: 7369 676e 203d 2069 6e74 286d 6d70 3c30  sign = int(mmp<0
-0000adb0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0000adc0: 2020 2020 2020 6d70 6162 7320 3d20 6162        mpabs = ab
-0000add0: 7328 6d6d 7029 0a0a 2020 2020 2020 2020  s(mmp)..        
-0000ade0: 2020 2020 2020 2020 2020 2020 6d69 7873              mixs
-0000adf0: 756d 203d 206d 6978 7375 6d5f 696e 6974  um = mixsum_init
-0000ae00: 202b 2030 0a0a 2020 2020 2020 2020 2020   + 0..          
-0000ae10: 2020 2020 2020 2020 2020 666f 7220 7070            for pp
-0000ae20: 2069 6e20 7261 6e67 6528 312c 705f 6d61   in range(1,p_ma
-0000ae30: 782b 3129 3a0a 2020 2020 2020 2020 2020  x+1):.          
-0000ae40: 2020 2020 2020 2020 2020 2020 2020 7070                pp
-0000ae50: 6920 3d20 7070 202d 2031 0a20 2020 2020  i = pp - 1.     
-0000ae60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ae70: 2020 2066 6f72 2071 7120 696e 2072 616e     for qq in ran
-0000ae80: 6765 282d 7070 2c70 702b 3129 3a0a 2020  ge(-pp,pp+1):.  
-0000ae90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000aea0: 2020 2020 2020 2020 2020 7173 6967 6e20            qsign 
-0000aeb0: 3d20 696e 7428 7171 3c30 290a 2020 2020  = int(qq<0).    
-0000aec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000aed0: 2020 2020 2020 2020 7161 6273 203d 2061          qabs = a
-0000aee0: 6273 2871 7129 0a0a 2020 2020 2020 2020  bs(qq)..        
-0000aef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000af00: 2020 2020 6d69 7873 756d 5b6d 7073 6967      mixsum[mpsig
-0000af10: 6e2c 6e6e 702c 6d70 6162 732c 206d 7369  n,nnp,mpabs, msi
-0000af20: 676e 2c6e 6e2c 6d61 6273 2c20 3a5d 202b  gn,nn,mabs, :] +
-0000af30: 3d20 6173 796d 5f73 6861 7065 5b3a 2c71  = asym_shape[:,q
-0000af40: 7369 676e 2c70 702c 7161 6273 5d2f 725f  sign,pp,qabs]/r_
-0000af50: 6264 735b 3a5d 202a 205c 0a20 2020 2020  bds[:] * \.     
-0000af60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000af70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000af80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000af90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000afa0: 2020 2020 2058 6964 5b6d 7073 6967 6e2c       Xid[mpsign,
-0000afb0: 6e6e 702c 6d70 6162 732c 2071 7369 676e  nnp,mpabs, qsign
-0000afc0: 2c70 702c 7161 6273 2c20 6d73 6967 6e2c  ,pp,qabs, msign,
-0000afd0: 6e6e 2c6d 6162 735d 0a0a 2020 2020 2020  nn,mabs]..      
-0000afe0: 2020 2020 2020 2020 2020 2020 2020 666f                fo
-0000aff0: 7220 6920 696e 2072 616e 6765 286e 5f62  r i in range(n_b
-0000b000: 6473 2d31 293a 0a20 2020 2020 2020 2020  ds-1):.         
-0000b010: 2020 2020 2020 2020 2020 2020 2020 2044                 D
-0000b020: 656c 7461 5b6d 7369 676e 2c6e 6e2c 6d61  elta[msign,nn,ma
-0000b030: 6273 2c20 695d 202b 3d20 6d69 7873 756d  bs, i] += mixsum
-0000b040: 5b6d 7073 6967 6e2c 6e6e 702c 6d70 6162  [mpsign,nnp,mpab
-0000b050: 732c 206d 7369 676e 2c6e 6e2c 6d61 6273  s, msign,nn,mabs
-0000b060: 2c20 695d 2f72 5f62 6473 5b2d 315d 202a  , i]/r_bds[-1] *
-0000b070: 205c 0a20 2020 2020 2020 2020 2020 2020   \.             
-0000b080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b090: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b0a0: 2020 2020 2020 6142 6172 5b6d 7073 6967        aBar[mpsig
-0000b0b0: 6e2c 6e6e 702c 6d70 6162 732c 2069 5d20  n,nnp,mpabs, i] 
-0000b0c0: 2a20 286a 6e5f 6c6c 5b6e 7069 2c69 5d20  * (jn_ll[npi,i] 
-0000b0d0: 2b20 4c61 6d62 645b 6e70 692c 695d 2a79  + Lambd[npi,i]*y
-0000b0e0: 6e5f 6c6c 5b6e 7069 2c69 5d29 202a 2028  n_ll[npi,i]) * (
-0000b0f0: 6b72 5f6c 6c5b 695d 2a2a 3220 2d20 6b72  kr_ll[i]**2 - kr
-0000b100: 5f75 6c5b 695d 2a2a 3229 0a0a 2020 2020  _ul[i]**2)..    
-0000b110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b120: 4465 6c74 615b 6d73 6967 6e2c 6e6e 2c6d  Delta[msign,nn,m
-0000b130: 6162 732c 2d31 5d20 2b3d 206d 6978 7375  abs,-1] += mixsu
-0000b140: 6d5b 6d70 7369 676e 2c6e 6e70 2c6d 7061  m[mpsign,nnp,mpa
-0000b150: 6273 2c20 6d73 6967 6e2c 6e6e 2c6d 6162  bs, msign,nn,mab
-0000b160: 732c 202d 315d 202a 205c 0a20 2020 2020  s, -1] * \.     
-0000b170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b190: 2020 2020 2020 2020 2020 286c 7477 6f2a            (ltwo*
-0000b1a0: 6e76 202b 206c 6f6e 6529 2f28 6e76 202b  nv + lone)/(nv +
-0000b1b0: 206c 6f6e 6529 202a 2042 656e 6d5b 6d70   lone) * Benm[mp
-0000b1c0: 7369 676e 2c6e 6e70 2c6d 7061 6273 5d20  sign,nnp,mpabs] 
-0000b1d0: 2a20 4164 5b6e 7069 5d0a 0a20 2020 2072  * Ad[npi]..    r
-0000b1e0: 6574 7572 6e20 4465 6c74 610a 0a23 2323  eturn Delta..###
-0000b1f0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0000b200: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0000b210: 2323 2323 2323 2323 2323 0a0a 2222 220a  ##########..""".
-0000b220: 6576 616c 5f69 6e6e 6572 5f72 6563 7572  eval_inner_recur
-0000b230: 5f73 796d 2829 0a20 2020 2045 7661 6c75  _sym().    Evalu
-0000b240: 6174 6520 7468 6520 7370 6865 7269 6361  ate the spherica
-0000b250: 6c6c 7920 7379 6d6d 6574 7269 6320 696e  lly symmetric in
-0000b260: 6e65 7220 7265 6375 7273 696f 6e20 7265  ner recursion re
-0000b270: 6c61 7469 6f6e 7320 746f 206f 6274 6169  lations to obtai
-0000b280: 6e20 4c61 6d62 6442 6172 2c20 7768 6963  n LambdBar, whic
-0000b290: 6820 6973 0a20 2020 2065 7861 6374 6c79  h is.    exactly
-0000b2a0: 2074 6865 2073 7068 6572 6963 616c 6c79   the spherically
-0000b2b0: 2073 796d 6d65 7472 6963 2073 6f6c 7574   symmetric solut
-0000b2c0: 696f 6e20 746f 2074 6865 2062 6f75 6e64  ion to the bound
-0000b2d0: 6172 7920 636f 6e64 6974 696f 6e73 2e20  ary conditions. 
-0000b2e0: 5468 6973 2071 7561 6e74 6974 7920 6170  This quantity ap
-0000b2f0: 7065 6172 730a 2020 2020 696e 2074 6865  pears.    in the
-0000b300: 2061 7379 6d6d 6574 7269 6320 7265 6375   asymmetric recu
-0000b310: 7273 696f 6e73 2c20 616e 6420 7765 206e  rsions, and we n
-0000b320: 6565 6420 746f 2065 7661 6c75 6174 6520  eed to evaluate 
-0000b330: 6974 2066 6f72 2061 6c6c 206e 2028 6e6f  it for all n (no
-0000b340: 7420 6a75 7374 2074 6865 2065 7863 6974  t just the excit
-0000b350: 6174 696f 6e73 0a20 2020 2074 6861 7420  ations.    that 
-0000b360: 7265 7375 6c74 2069 6e20 7468 6520 6361  result in the ca
-0000b370: 7365 206f 6620 7370 6865 7269 6361 6c20  se of spherical 
-0000b380: 7379 6d6d 6574 7279 292e 0a20 2020 2055  symmetry)..    U
-0000b390: 7361 6765 3a20 604c 616d 6264 4261 7260  sage: `LambdBar`
-0000b3a0: 203d 2065 7661 6c5f 696e 6e65 725f 7265   = eval_inner_re
-0000b3b0: 6375 725f 7379 6d28 606e 5f6d 6178 602c  cur_sym(`n_max`,
-0000b3c0: 2060 6e5f 6264 7360 2c20 6062 6574 6160   `n_bds`, `beta`
-0000b3d0: 2c20 6067 616d 6d60 2c20 6064 656c 7460  , `gamm`, `delt`
-0000b3e0: 2c20 6065 7073 6960 290a 2020 2020 5265  , `epsi`).    Re
-0000b3f0: 7475 726e 733a 0a20 2020 2020 2020 204c  turns:.        L
-0000b400: 616d 6264 4261 723a 206d 7063 2c20 7368  ambdBar: mpc, sh
-0000b410: 6170 6528 6e5f 6d61 782c 6e5f 6264 7329  ape(n_max,n_bds)
-0000b420: 2e20 5468 6973 2069 7320 5c6f 7665 726c  . This is \overl
-0000b430: 696e 657b 5c4c 616d 6264 617d 5e7b 6c7d  ine{\Lambda}^{l}
-0000b440: 5f7b 6e7d 2069 6e20 7468 6520 7061 7065  _{n} in the pape
-0000b450: 722e 0a20 2020 2050 6172 616d 6574 6572  r..    Parameter
-0000b460: 733a 0a20 2020 2020 2020 206e 5f6d 6178  s:.        n_max
-0000b470: 3a20 696e 7465 6765 722e 204d 6178 696d  : integer. Maxim
-0000b480: 756d 2064 6567 7265 6520 6e20 6f66 2069  um degree n of i
-0000b490: 6e64 7563 6564 206d 6f6d 656e 7473 2e0a  nduced moments..
-0000b4a0: 2020 2020 2020 2020 6e5f 6264 733a 2069          n_bds: i
-0000b4b0: 6e74 6567 6572 2e20 4e75 6d62 6572 206f  nteger. Number o
-0000b4c0: 6620 626f 756e 6461 7269 6573 2070 7265  f boundaries pre
-0000b4d0: 7365 6e74 2069 6e20 7468 6520 696e 7465  sent in the inte
-0000b4e0: 7269 6f72 206d 6f64 656c 2e0a 2020 2020  rior model..    
-0000b4f0: 2020 2020 6265 7461 2c20 6761 6d6d 2c20      beta, gamm, 
-0000b500: 6465 6c74 2c20 6570 7369 3a20 6d70 632c  delt, epsi: mpc,
-0000b510: 2073 6861 7065 286e 5f6d 6178 2c6e 5f62   shape(n_max,n_b
-0000b520: 6473 292e 2052 6563 7572 7369 6f6e 2071  ds). Recursion q
-0000b530: 7561 6e74 6974 6965 7320 6465 7269 7665  uantities derive
-0000b540: 6420 6672 6f6d 0a20 2020 2020 2020 2020  d from.         
-0000b550: 2020 2042 6573 7365 6c20 6675 6e63 7469     Bessel functi
-0000b560: 6f6e 732e 2054 6865 7365 2061 7265 205c  ons. These are \
-0000b570: 6265 7461 2c20 5c67 616d 6d61 2c20 5c64  beta, \gamma, \d
-0000b580: 656c 7461 2c20 616e 6420 5c65 7073 696c  elta, and \epsil
-0000b590: 6f6e 2066 726f 6d20 7468 6520 7061 7065  on from the pape
-0000b5a0: 722e 0a20 2020 2020 2020 2020 2020 2053  r..            S
-0000b5b0: 6565 2042 696e 6d52 6573 706f 6e73 6520  ee BinmResponse 
-0000b5c0: 666f 7220 6d6f 7265 2064 6574 6169 6c73  for more details
-0000b5d0: 2e0a 2020 2020 2222 220a 6465 6620 6576  ..    """.def ev
-0000b5e0: 616c 5f69 6e6e 6572 5f72 6563 7572 5f73  al_inner_recur_s
-0000b5f0: 796d 286e 5f6d 6178 2c20 6e5f 6264 732c  ym(n_max, n_bds,
-0000b600: 2062 6574 612c 2067 616d 6d2c 2064 656c   beta, gamm, del
-0000b610: 742c 2065 7073 6929 3a0a 2020 2020 4c61  t, epsi):.    La
-0000b620: 6d62 6420 3d20 6e70 2e7a 6572 6f73 2828  mbd = np.zeros((
-0000b630: 6e5f 6d61 782c 6e5f 6264 7329 2c20 6474  n_max,n_bds), dt
-0000b640: 7970 653d 6d70 635f 676c 6f62 616c 290a  ype=mpc_global).
-0000b650: 2020 2020 666f 7220 6920 696e 2072 616e      for i in ran
-0000b660: 6765 286e 5f62 6473 2d31 293a 0a20 2020  ge(n_bds-1):.   
-0000b670: 2020 2020 204c 616d 6264 5b3a 2c69 2b31       Lambd[:,i+1
-0000b680: 5d20 3d20 6370 785f 6469 7628 2864 656c  ] = cpx_div((del
-0000b690: 745b 3a2c 695d 202b 204c 616d 6264 5b3a  t[:,i] + Lambd[:
-0000b6a0: 2c69 5d2a 6570 7369 5b3a 2c69 5d29 202c  ,i]*epsi[:,i]) ,
-0000b6b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000b6c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b6d0: 2862 6574 615b 3a2c 695d 202b 204c 616d  (beta[:,i] + Lam
-0000b6e0: 6264 5b3a 2c69 5d2a 6761 6d6d 5b3a 2c69  bd[:,i]*gamm[:,i
-0000b6f0: 5d29 290a 0a20 2020 2072 6574 7572 6e20  ]))..    return 
-0000b700: 4c61 6d62 640a 0a23 2041 766f 6964 7320  Lambd..# Avoids 
-0000b710: 6469 7669 6465 2d62 792d 7a65 726f 2065  divide-by-zero e
-0000b720: 7272 6f72 7320 7768 656e 204c 616d 6264  rrors when Lambd
-0000b730: 2069 7320 7665 7279 2063 6c6f 7365 2074   is very close t
-0000b740: 6f20 6920 2868 6967 6820 636f 6e64 7563  o i (high conduc
-0000b750: 7469 7669 7469 6573 290a 6465 6620 6370  tivities).def cp
-0000b760: 785f 6469 7628 612c 2062 293a 0a20 2020  x_div(a, b):.   
-0000b770: 206e 7661 6c73 203d 206e 702e 7369 7a65   nvals = np.size
-0000b780: 2861 290a 2020 2020 616d 6167 203d 205b  (a).    amag = [
-0000b790: 206d 702e 6661 6273 2861 6929 2066 6f72   mp.fabs(ai) for
-0000b7a0: 2061 6920 696e 2061 205d 0a20 2020 2061   ai in a ].    a
-0000b7b0: 6172 6720 3d20 5b20 6d70 2e61 7461 6e32  arg = [ mp.atan2
-0000b7c0: 286d 702e 696d 2861 6929 2c20 6d70 2e72  (mp.im(ai), mp.r
-0000b7d0: 6528 6169 2929 2066 6f72 2061 6920 696e  e(ai)) for ai in
-0000b7e0: 2061 205d 0a20 2020 2062 6d61 6720 3d20   a ].    bmag = 
-0000b7f0: 5b20 6d70 2e66 6162 7328 6269 2920 666f  [ mp.fabs(bi) fo
-0000b800: 7220 6269 2069 6e20 6220 5d0a 2020 2020  r bi in b ].    
-0000b810: 6261 7267 203d 205b 206d 702e 6174 616e  barg = [ mp.atan
-0000b820: 3228 6d70 2e69 6d28 6269 292c 206d 702e  2(mp.im(bi), mp.
-0000b830: 7265 2862 6929 2920 666f 7220 6269 2069  re(bi)) for bi i
-0000b840: 6e20 6220 5d0a 0a20 2020 2064 6976 5f6d  n b ]..    div_m
-0000b850: 6167 203d 205b 2061 6d61 675b 695d 202f  ag = [ amag[i] /
-0000b860: 2062 6d61 675b 695d 2066 6f72 2069 2069   bmag[i] for i i
-0000b870: 6e20 7261 6e67 6528 6e76 616c 7329 205d  n range(nvals) ]
-0000b880: 0a20 2020 2064 6976 5f61 7267 203d 205b  .    div_arg = [
-0000b890: 2061 6172 675b 695d 202d 2062 6172 675b   aarg[i] - barg[
-0000b8a0: 695d 2066 6f72 2069 2069 6e20 7261 6e67  i] for i in rang
-0000b8b0: 6528 6e76 616c 7329 205d 0a20 2020 2071  e(nvals) ].    q
-0000b8c0: 756f 7469 656e 7420 3d20 6e70 2e61 7272  uotient = np.arr
-0000b8d0: 6179 285b 2064 6976 5f6d 6167 5b69 5d20  ay([ div_mag[i] 
-0000b8e0: 2a20 6d70 2e65 7870 286a 202a 2064 6976  * mp.exp(j * div
-0000b8f0: 5f61 7267 5b69 5d29 2066 6f72 2069 2069  _arg[i]) for i i
-0000b900: 6e20 7261 6e67 6528 6e76 616c 7329 205d  n range(nvals) ]
-0000b910: 290a 2020 2020 7265 7475 726e 2071 756f  ).    return quo
-0000b920: 7469 656e 740a 6465 6620 6370 785f 6469  tient.def cpx_di
-0000b930: 765f 7661 6c28 612c 2062 293a 0a20 2020  v_val(a, b):.   
-0000b940: 2061 6d61 6720 3d20 6d70 2e66 6162 7328   amag = mp.fabs(
-0000b950: 6129 0a20 2020 2061 6172 6720 3d20 6d70  a).    aarg = mp
-0000b960: 2e61 7461 6e32 286d 702e 696d 2861 292c  .atan2(mp.im(a),
-0000b970: 206d 702e 7265 2861 2929 0a20 2020 2062   mp.re(a)).    b
-0000b980: 6d61 6720 3d20 6d70 2e66 6162 7328 6229  mag = mp.fabs(b)
-0000b990: 0a20 2020 2062 6172 6720 3d20 6d70 2e61  .    barg = mp.a
-0000b9a0: 7461 6e32 286d 702e 696d 2862 292c 206d  tan2(mp.im(b), m
-0000b9b0: 702e 7265 2862 2929 0a0a 2020 2020 6469  p.re(b))..    di
-0000b9c0: 765f 6d61 6720 3d20 616d 6167 202f 2062  v_mag = amag / b
-0000b9d0: 6d61 670a 2020 2020 6469 765f 6172 6720  mag.    div_arg 
-0000b9e0: 3d20 6161 7267 202d 2062 6172 670a 2020  = aarg - barg.  
-0000b9f0: 2020 7175 6f74 6965 6e74 203d 2064 6976    quotient = div
-0000ba00: 5f6d 6167 202a 206d 702e 6578 7028 6a20  _mag * mp.exp(j 
-0000ba10: 2a20 6469 765f 6172 6729 0a20 2020 2072  * div_arg).    r
-0000ba20: 6574 7572 6e20 7175 6f74 6965 6e74 0a0a  eturn quotient..
-0000ba30: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0000ba40: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0000ba50: 2323 2323 2323 2323 2323 2323 230a 2320  #############.# 
-0000ba60: 4e4f 5445 2054 4845 204e 4f54 4154 494f  NOTE THE NOTATIO
-0000ba70: 4e20 464f 5220 6e27 2041 4e44 206e 2049  N FOR n' AND n I
-0000ba80: 5320 5245 5645 5253 4544 2049 4e20 5448  S REVERSED IN TH
-0000ba90: 4953 2043 4f44 4520 424c 4f43 4b20 434f  IS CODE BLOCK CO
-0000baa0: 4d50 4152 4544 2054 4f20 4d4f 5354 204f  MPARED TO MOST O
-0000bab0: 4620 5448 4520 4f54 4845 5220 434f 4445  F THE OTHER CODE
-0000bac0: 0a23 2054 6869 7320 6973 2066 6f72 2063  .# This is for c
-0000bad0: 6f6e 7369 7374 656e 6379 2077 6974 6820  onsistency with 
-0000bae0: 7468 6520 7061 7065 7220 616e 6420 666f  the paper and fo
-0000baf0: 7220 7368 6f72 7465 7220 6c69 6e65 7320  r shorter lines 
-0000bb00: 6f66 2063 6f64 652e 0a23 2049 6e20 7468  of code..# In th
-0000bb10: 6973 2062 6c6f 636b 2c20 6e2c 6d20 6973  is block, n,m is
-0000bb20: 2074 6865 2065 7863 6974 6174 696f 6e20   the excitation 
-0000bb30: 6861 726d 6f6e 6963 2061 6e64 206e 272c  harmonic and n',
-0000bb40: 6d27 2069 7320 7468 6520 696e 6475 6365  m' is the induce
-0000bb50: 6420 6861 726d 6f6e 6963 2e0a 2323 2323  d harmonic..####
-0000bb60: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0000bb70: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0000bb80: 2323 2323 2323 2323 230a 0a22 2222 0a67  #########..""".g
-0000bb90: 6574 5f61 6c6c 5f58 6964 2829 0a20 2020  et_all_Xid().   
-0000bba0: 2052 6574 7572 6e73 206d 6978 696e 6720   Returns mixing 
-0000bbb0: 636f 6566 6669 6369 656e 7473 2074 6861  coefficients tha
-0000bbc0: 7420 7265 7375 6c74 2066 726f 6d20 6d75  t result from mu
-0000bbd0: 6c74 6970 6c69 6361 7469 6f6e 206f 6620  ltiplication of 
-0000bbe0: 7370 6865 7269 6361 6c20 6861 726d 6f6e  spherical harmon
-0000bbf0: 6963 732e 0a20 2020 2055 7361 6765 3a20  ics..    Usage: 
-0000bc00: 6058 6964 6020 3d20 6765 745f 616c 6c5f  `Xid` = get_all_
-0000bc10: 5869 6428 606e 5f6d 6178 602c 2060 705f  Xid(`n_max`, `p_
-0000bc20: 6d61 7860 2c20 606e 7072 6d5f 6d61 7860  max`, `nprm_max`
-0000bc30: 2c20 606e 7072 6d76 616c 7360 2c20 606d  , `nprmvals`, `m
-0000bc40: 7072 6d76 616c 7360 290a 2020 2020 5265  prmvals`).    Re
-0000bc50: 7475 726e 733a 0a20 2020 2020 2020 2058  turns:.        X
-0000bc60: 6964 3a20 6d70 662c 2073 6861 7065 2832  id: mpf, shape(2
-0000bc70: 2c6e 5f6d 6178 2b31 2c6e 5f6d 6178 2b31  ,n_max+1,n_max+1
-0000bc80: 2c20 322c 705f 6d61 782b 312c 705f 6d61  , 2,p_max+1,p_ma
-0000bc90: 782b 312c 2032 2c6e 7072 6d5f 6d61 782b  x+1, 2,nprm_max+
-0000bca0: 312c 6e70 726d 5f6d 6178 2b31 292e 2041  1,nprm_max+1). A
-0000bcb0: 6d6f 756e 7420 6f66 2059 6e6d 2074 6861  mount of Ynm tha
-0000bcc0: 7420 7265 7375 6c74 730a 2020 2020 2020  t results.      
-0000bcd0: 2020 2020 2020 6672 6f6d 206d 756c 7469        from multi
-0000bce0: 706c 7969 6e67 2059 6e6d 2062 7920 5970  plying Ynm by Yp
-0000bcf0: 712e 2056 616c 7565 7320 666f 7220 616c  q. Values for al
-0000bd00: 6c20 636f 6d62 696e 6174 696f 6e73 206f  l combinations o
-0000bd10: 6620 6e2c 6d2c 702c 712c 6e27 2c6d 2720  f n,m,p,q,n',m' 
-0000bd20: 6172 6520 7265 7475 726e 6564 2e0a 2020  are returned..  
-0000bd30: 2020 5061 7261 6d65 7465 7273 3a0a 2020    Parameters:.  
-0000bd40: 2020 2020 2020 6e5f 6d61 783a 2069 6e74        n_max: int
-0000bd50: 6567 6572 2e20 4d61 7869 6d75 6d20 6465  eger. Maximum de
-0000bd60: 6772 6565 206e 206f 6620 6578 6369 7461  gree n of excita
-0000bd70: 7469 6f6e 206d 6f6d 656e 7473 2e0a 2020  tion moments..  
-0000bd80: 2020 2020 2020 705f 6d61 783a 2069 6e74        p_max: int
-0000bd90: 6567 6572 2e20 4d61 7869 6d75 6d20 6465  eger. Maximum de
-0000bda0: 6772 6565 2070 206f 6620 626f 756e 6461  gree p of bounda
-0000bdb0: 7279 2073 6861 7065 732e 0a20 2020 2020  ry shapes..     
-0000bdc0: 2020 206e 7072 6d5f 6d61 783a 2069 6e74     nprm_max: int
-0000bdd0: 6567 6572 2e20 4d61 7869 6d75 6d20 6465  eger. Maximum de
-0000bde0: 6772 6565 206e 7072 6d20 6f66 2069 6e64  gree nprm of ind
-0000bdf0: 7563 6564 206d 6f6d 656e 7473 2e20 5479  uced moments. Ty
-0000be00: 7069 6361 6c6c 7920 6e6d 6178 202b 2070  pically nmax + p
-0000be10: 6d61 782e 0a20 2020 2020 2020 206e 7072  max..        npr
-0000be20: 6d76 616c 733a 2069 6e74 6567 6572 2c20  mvals: integer, 
-0000be30: 7368 6170 6528 286e 7072 6d5f 6d61 782b  shape((nprm_max+
-0000be40: 3129 2a2a 322d 3129 2e20 466c 6174 7465  1)**2-1). Flatte
-0000be50: 6e65 6420 6172 7261 7920 6f66 206e 7072  ned array of npr
-0000be60: 6d20 7661 6c75 6573 2e0a 2020 2020 2020  m values..      
-0000be70: 2020 6d70 726d 7661 6c73 3a20 696e 7465    mprmvals: inte
-0000be80: 6765 722c 2073 6861 7065 2828 6e70 726d  ger, shape((nprm
-0000be90: 5f6d 6178 2b31 292a 2a32 2d31 292e 2046  _max+1)**2-1). F
-0000bea0: 6c61 7474 656e 6564 2061 7272 6179 206f  lattened array o
-0000beb0: 6620 6d70 726d 2076 616c 7565 7320 636f  f mprm values co
-0000bec0: 7272 6573 706f 6e64 696e 6720 746f 2065  rresponding to e
-0000bed0: 6163 6820 6e72 706d 2061 626f 7665 2e0a  ach nrpm above..
-0000bee0: 2020 2020 2222 220a 6465 6620 6765 745f      """.def get_
-0000bef0: 616c 6c5f 5869 6428 6e5f 6d61 782c 2070  all_Xid(n_max, p
-0000bf00: 5f6d 6178 2c20 6e70 726d 5f6d 6178 2c20  _max, nprm_max, 
-0000bf10: 6e70 726d 7661 6c73 2c20 6d70 726d 7661  nprmvals, mprmva
-0000bf20: 6c73 2c20 646f 5f70 6172 616c 6c65 6c3d  ls, do_parallel=
-0000bf30: 5472 7565 2c0a 2020 2020 2020 2020 2020  True,.          
-0000bf40: 2020 2020 2020 7772 6974 656f 7574 3d54        writeout=T
-0000bf50: 7275 652c 2072 656c 6f61 643d 4661 6c73  rue, reload=Fals
-0000bf60: 652c 2066 7061 7468 3d4e 6f6e 652c 2066  e, fpath=None, f
-0000bf70: 6e61 6d65 3d4e 6f6e 6529 3a0a 2020 2020  name=None):.    
-0000bf80: 6966 2077 7269 7465 6f75 7420 6f72 2072  if writeout or r
-0000bf90: 656c 6f61 643a 0a20 2020 2020 2020 2069  eload:.        i
-0000bfa0: 6620 6670 6174 6820 6973 204e 6f6e 653a  f fpath is None:
-0000bfb0: 0a20 2020 2020 2020 2020 2020 2066 7061  .            fpa
-0000bfc0: 7468 203d 205f 696e 6475 6365 640a 2020  th = _induced.  
-0000bfd0: 2020 2020 2020 6966 2066 6e61 6d65 2069        if fname i
-0000bfe0: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
-0000bff0: 2020 2020 666e 616d 6520 3d20 6622 5869      fname = f"Xi
-0000c000: 645f 7661 6c75 6573 5f6e 7b6e 5f6d 6178  d_values_n{n_max
-0000c010: 7d5f 707b 705f 6d61 787d 5f6e 707b 6e70  }_p{p_max}_np{np
-0000c020: 726d 5f6d 6178 7d22 0a0a 2020 2020 2020  rm_max}"..      
-0000c030: 2020 6675 6c6c 4669 6c65 203d 206f 732e    fullFile = os.
-0000c040: 7061 7468 2e6a 6f69 6e28 6670 6174 682c  path.join(fpath,
-0000c050: 2066 6e61 6d65 2b22 2e6d 6174 2229 0a20   fname+".mat"). 
-0000c060: 2020 2020 2020 2066 696c 6545 7869 7374         fileExist
-0000c070: 7320 3d20 6f73 2e70 6174 682e 6973 6669  s = os.path.isfi
-0000c080: 6c65 2866 756c 6c46 696c 6529 0a20 2020  le(fullFile).   
-0000c090: 2020 2020 2069 6620 7265 6c6f 6164 2061       if reload a
-0000c0a0: 6e64 206e 6f74 2066 696c 6545 7869 7374  nd not fileExist
-0000c0b0: 733a 0a20 2020 2020 2020 2020 2020 206c  s:.            l
-0000c0c0: 6f67 2e77 6172 6e69 6e67 2866 2758 6964  og.warning(f'Xid
-0000c0d0: 2066 696c 6520 7b66 756c 6c46 696c 657d   file {fullFile}
-0000c0e0: 2064 6f65 7320 6e6f 7420 6578 6973 742c   does not exist,
-0000c0f0: 2062 7574 2072 656c 6f61 6420 6973 2054   but reload is T
-0000c100: 7275 652e 2043 616c 6375 6c61 7469 6e67  rue. Calculating
-0000c110: 2069 6e73 7465 6164 2e27 290a 2020 2020   instead.').    
-0000c120: 2020 2020 2020 2020 7265 6c6f 6164 203d          reload =
-0000c130: 2046 616c 7365 0a20 2020 2020 2020 2020   False.         
-0000c140: 2020 2077 7269 7465 6f75 7420 3d20 5472     writeout = Tr
-0000c150: 7565 0a0a 2020 2020 6966 2072 656c 6f61  ue..    if reloa
-0000c160: 643a 0a20 2020 2020 2020 2058 6964 203d  d:.        Xid =
-0000c170: 206c 6f61 646d 6174 2866 756c 6c46 696c   loadmat(fullFil
-0000c180: 6529 5b27 5869 6427 5d0a 2020 2020 656c  e)['Xid'].    el
-0000c190: 7365 3a0a 2020 2020 2020 2020 5869 6420  se:.        Xid 
-0000c1a0: 3d20 6e70 2e7a 6572 6f73 2828 322c 6e5f  = np.zeros((2,n_
-0000c1b0: 6d61 782b 312c 6e5f 6d61 782b 312c 2032  max+1,n_max+1, 2
-0000c1c0: 2c70 5f6d 6178 2b31 2c70 5f6d 6178 2b31  ,p_max+1,p_max+1
-0000c1d0: 2c20 322c 6e70 726d 5f6d 6178 2b31 2c6e  , 2,nprm_max+1,n
-0000c1e0: 7072 6d5f 6d61 782b 3129 2c20 6474 7970  prm_max+1), dtyp
-0000c1f0: 653d 6d70 665f 676c 6f62 616c 290a 2020  e=mpf_global).  
-0000c200: 2020 2020 2020 4e6e 6d70 726d 203d 206e        Nnmprm = n
-0000c210: 702e 7369 7a65 286e 7072 6d76 616c 7329  p.size(nprmvals)
-0000c220: 0a0a 2020 2020 2020 2020 666f 7220 6e20  ..        for n 
-0000c230: 696e 2072 616e 6765 2831 2c6e 5f6d 6178  in range(1,n_max
-0000c240: 2b31 293a 0a20 2020 2020 2020 2020 2020  +1):.           
-0000c250: 2066 6f72 206d 2069 6e20 7261 6e67 6528   for m in range(
-0000c260: 2d6e 2c6e 2b31 293a 0a20 2020 2020 2020  -n,n+1):.       
-0000c270: 2020 2020 2020 2020 206d 7369 676e 203d           msign =
-0000c280: 2069 6e74 286d 3c30 290a 2020 2020 2020   int(m<0).      
-0000c290: 2020 2020 2020 2020 2020 6d61 6273 203d            mabs =
-0000c2a0: 2061 6273 286d 290a 0a20 2020 2020 2020   abs(m)..       
-0000c2b0: 2020 2020 2020 2020 2066 6f72 2070 2069           for p i
-0000c2c0: 6e20 7261 6e67 6528 312c 705f 6d61 782b  n range(1,p_max+
-0000c2d0: 3129 3a0a 2020 2020 2020 2020 2020 2020  1):.            
-0000c2e0: 2020 2020 2020 2020 666f 7220 7120 696e          for q in
-0000c2f0: 2072 616e 6765 282d 702c 702b 3129 3a0a   range(-p,p+1):.
-0000c300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c310: 2020 2020 2020 2020 7173 6967 6e20 3d20          qsign = 
-0000c320: 696e 7428 713c 3029 0a20 2020 2020 2020  int(q<0).       
-0000c330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c340: 2071 6162 7320 3d20 6162 7328 7129 0a0a   qabs = abs(q)..
-0000c350: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c360: 2020 2020 2020 2020 6966 2064 6f5f 7061          if do_pa
-0000c370: 7261 6c6c 656c 3a0a 2020 2020 2020 2020  rallel:.        
-0000c380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c390: 2020 2020 706f 6f6c 203d 206d 7470 436f      pool = mtpCo
-0000c3a0: 6e74 6578 742e 506f 6f6c 286e 756d 5f63  ntext.Pool(num_c
-0000c3b0: 6f72 6573 290a 2020 2020 2020 2020 2020  ores).          
-0000c3c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c3d0: 2020 7061 725f 7265 7375 6c74 203d 205b    par_result = [
-0000c3e0: 706f 6f6c 2e61 7070 6c79 5f61 7379 6e63  pool.apply_async
-0000c3f0: 2820 6361 6c63 5f58 6964 2c20 6172 6773  ( calc_Xid, args
-0000c400: 3d28 6e2c 6d2c 702c 712c 6e70 726d 7661  =(n,m,p,q,nprmva
-0000c410: 6c73 5b69 4e5d 2c6d 7072 6d76 616c 735b  ls[iN],mprmvals[
-0000c420: 694e 5d2c 6e70 726d 5f6d 6178 2920 2920  iN],nprm_max) ) 
-0000c430: 666f 7220 694e 2069 6e20 7261 6e67 6528  for iN in range(
-0000c440: 4e6e 6d70 726d 295d 0a20 2020 2020 2020  Nnmprm)].       
-0000c450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c460: 2020 2020 2070 6f6f 6c2e 636c 6f73 6528       pool.close(
-0000c470: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0000c480: 2020 2020 2020 2020 2020 2020 2020 706f                po
-0000c490: 6f6c 2e6a 6f69 6e28 290a 0a20 2020 2020  ol.join()..     
-0000c4a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c4b0: 2020 2066 6f72 2069 4e20 696e 2072 616e     for iN in ran
-0000c4c0: 6765 284e 6e6d 7072 6d29 3a0a 2020 2020  ge(Nnmprm):.    
-0000c4d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c4e0: 2020 2020 2020 2020 6e70 726d 203d 206e          nprm = n
-0000c4f0: 7072 6d76 616c 735b 694e 5d0a 2020 2020  prmvals[iN].    
-0000c500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c510: 2020 2020 2020 2020 6d70 7369 676e 203d          mpsign =
-0000c520: 2069 6e74 286d 7072 6d76 616c 735b 694e   int(mprmvals[iN
-0000c530: 5d3c 3029 0a20 2020 2020 2020 2020 2020  ]<0).           
-0000c540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c550: 206d 7061 6273 203d 2061 6273 286d 7072   mpabs = abs(mpr
-0000c560: 6d76 616c 735b 694e 5d29 0a20 2020 2020  mvals[iN]).     
-0000c570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c580: 2020 2020 2020 2069 6620 646f 5f70 6172         if do_par
-0000c590: 616c 6c65 6c3a 0a20 2020 2020 2020 2020  allel:.         
-0000c5a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c5b0: 2020 2020 2020 2058 6964 5b6d 7369 676e         Xid[msign
-0000c5c0: 2c6e 2c6d 6162 732c 2071 7369 676e 2c70  ,n,mabs, qsign,p
-0000c5d0: 2c71 6162 732c 206d 7073 6967 6e2c 6e70  ,qabs, mpsign,np
-0000c5e0: 726d 2c6d 7061 6273 5d20 3d20 7061 725f  rm,mpabs] = par_
-0000c5f0: 7265 7375 6c74 5b69 4e5d 2e67 6574 2829  result[iN].get()
-0000c600: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000c610: 2020 2020 2020 2020 2020 2020 2065 6c73               els
-0000c620: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-0000c630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c640: 2020 2058 6964 5b6d 7369 676e 2c20 6e2c     Xid[msign, n,
-0000c650: 206d 6162 732c 2071 7369 676e 2c20 702c   mabs, qsign, p,
-0000c660: 2071 6162 732c 206d 7073 6967 6e2c 206e   qabs, mpsign, n
-0000c670: 7072 6d2c 206d 7061 6273 5d20 3d20 6361  prm, mpabs] = ca
-0000c680: 6c63 5f58 6964 286e 2c6d 2c70 2c71 2c6e  lc_Xid(n,m,p,q,n
-0000c690: 7072 6d76 616c 735b 694e 5d2c 6d70 726d  prmvals[iN],mprm
-0000c6a0: 7661 6c73 5b69 4e5d 2c6e 7072 6d5f 6d61  vals[iN],nprm_ma
-0000c6b0: 7829 0a20 2020 2020 2020 2069 6620 7772  x).        if wr
-0000c6c0: 6974 656f 7574 3a0a 2020 2020 2020 2020  iteout:.        
-0000c6d0: 2020 2020 7361 7665 6d61 7428 6675 6c6c      savemat(full
-0000c6e0: 4669 6c65 2c20 7b27 5869 6427 3a20 5869  File, {'Xid': Xi
-0000c6f0: 642e 6173 7479 7065 286e 702e 666c 6f61  d.astype(np.floa
-0000c700: 745f 297d 290a 2020 2020 2020 2020 2020  t_)}).          
-0000c710: 2020 6c6f 672e 6465 6275 6728 6627 5361    log.debug(f'Sa
-0000c720: 7665 6420 5869 6420 7661 6c75 6573 2074  ved Xid values t
-0000c730: 6f20 6669 6c65 3a20 7b66 756c 6c46 696c  o file: {fullFil
-0000c740: 657d 2729 0a0a 2020 2020 7265 7475 726e  e}')..    return
-0000c750: 2058 6964 0a0a 2222 220a 7072 696e 745f   Xid..""".print_
-0000c760: 5869 645f 7461 626c 6528 290a 2020 2020  Xid_table().    
-0000c770: 5072 696e 7473 2061 2074 6162 6c65 2074  Prints a table t
-0000c780: 6f20 7468 6520 7465 726d 696e 616c 206f  o the terminal o
-0000c790: 6620 7661 6c75 6573 2066 6f72 2061 6c6c  f values for all
-0000c7a0: 2058 6964 2066 6f72 2064 6562 7567 2070   Xid for debug p
-0000c7b0: 7572 706f 7365 732e 0a20 2020 2055 7361  urposes..    Usa
-0000c7c0: 6765 3a20 7072 696e 745f 5869 645f 7461  ge: print_Xid_ta
-0000c7d0: 626c 6528 6058 6964 602c 2060 6e5f 6d61  ble(`Xid`, `n_ma
-0000c7e0: 7860 2c20 6070 5f6d 6178 602c 2060 6e70  x`, `p_max`, `np
-0000c7f0: 726d 5f6d 6178 6029 0a20 2020 2052 6574  rm_max`).    Ret
-0000c800: 7572 6e73 3a0a 2020 2020 2020 2020 4e6f  urns:.        No
-0000c810: 6e65 2e0a 2020 2020 5061 7261 6d65 7465  ne..    Paramete
-0000c820: 7273 3a0a 2020 2020 2020 2020 5869 643a  rs:.        Xid:
-0000c830: 206d 7066 2c20 7368 6170 6528 322c 6e5f   mpf, shape(2,n_
-0000c840: 6d61 782b 312c 6e5f 6d61 782b 312c 2032  max+1,n_max+1, 2
-0000c850: 2c70 5f6d 6178 2b31 2c70 5f6d 6178 2b31  ,p_max+1,p_max+1
-0000c860: 2c20 322c 6e70 726d 5f6d 6178 2b31 2c6e  , 2,nprm_max+1,n
-0000c870: 7072 6d5f 6d61 782b 3129 2e20 5869 6420  prm_max+1). Xid 
-0000c880: 7661 6c75 6573 2074 6f20 7072 696e 742e  values to print.
-0000c890: 0a20 2020 2020 2020 206e 5f6d 6178 3a20  .        n_max: 
-0000c8a0: 696e 7465 6765 722e 204d 6178 696d 756d  integer. Maximum
-0000c8b0: 2064 6567 7265 6520 6e20 6f66 2065 7863   degree n of exc
-0000c8c0: 6974 6174 696f 6e20 6d6f 6d65 6e74 732e  itation moments.
-0000c8d0: 0a20 2020 2020 2020 2070 5f6d 6178 3a20  .        p_max: 
-0000c8e0: 696e 7465 6765 722e 204d 6178 696d 756d  integer. Maximum
-0000c8f0: 2064 6567 7265 6520 7020 6f66 2062 6f75   degree p of bou
-0000c900: 6e64 6172 7920 7368 6170 6573 2e0a 2020  ndary shapes..  
-0000c910: 2020 2020 2020 6e70 726d 5f6d 6178 3a20        nprm_max: 
-0000c920: 696e 7465 6765 722e 204d 6178 696d 756d  integer. Maximum
-0000c930: 2064 6567 7265 6520 6e70 726d 206f 6620   degree nprm of 
-0000c940: 696e 6475 6365 6420 6d6f 6d65 6e74 732e  induced moments.
-0000c950: 2054 7970 6963 616c 6c79 206e 6d61 7820   Typically nmax 
-0000c960: 2b20 706d 6178 2e0a 2020 2020 2222 220a  + pmax..    """.
-0000c970: 6465 6620 7072 696e 745f 5869 645f 7461  def print_Xid_ta
-0000c980: 626c 6528 5869 642c 206e 5f6d 6178 2c20  ble(Xid, n_max, 
-0000c990: 705f 6d61 782c 206e 7072 6d5f 6d61 7829  p_max, nprm_max)
-0000c9a0: 3a0a 2020 2020 2320 5072 696e 7420 7461  :.    # Print ta
-0000c9b0: 626c 6520 6865 6164 6572 0a20 2020 2068  ble header.    h
-0000c9c0: 6561 645f 726f 7720 3d20 2220 2020 2022  ead_row = "    "
-0000c9d0: 0a20 2020 2066 6f72 206e 2069 6e20 7261  .    for n in ra
-0000c9e0: 6e67 6528 312c 206e 5f6d 6178 2b31 293a  nge(1, n_max+1):
-0000c9f0: 0a20 2020 2020 2020 2066 6f72 206d 2069  .        for m i
-0000ca00: 6e20 7261 6e67 6528 2d6e 2c20 6e2b 3129  n range(-n, n+1)
-0000ca10: 3a0a 2020 2020 2020 2020 2020 2020 6865  :.            he
-0000ca20: 6164 5f72 6f77 203d 2068 6561 645f 726f  ad_row = head_ro
-0000ca30: 7720 2b20 6622 7c20 2020 2059 7b6e 7d7b  w + f"|    Y{n}{
-0000ca40: 6d7d 2020 2020 222e 6c6a 7573 7428 3235  m}    ".ljust(25
-0000ca50: 290a 2020 2020 6865 6164 5f72 6f77 203d  ).    head_row =
-0000ca60: 2066 227b 6865 6164 5f72 6f77 7d7c 220a   f"{head_row}|".
-0000ca70: 2020 2020 7072 696e 7428 6865 6164 5f72      print(head_r
-0000ca80: 6f77 290a 2020 2020 2320 5072 696e 7420  ow).    # Print 
-0000ca90: 7368 6170 6573 2061 7320 726f 7773 0a20  shapes as rows. 
-0000caa0: 2020 2066 6f72 2070 2069 6e20 7261 6e67     for p in rang
-0000cab0: 6528 312c 2070 5f6d 6178 2b31 293a 0a20  e(1, p_max+1):. 
-0000cac0: 2020 2020 2020 2066 6f72 2071 2069 6e20         for q in 
-0000cad0: 7261 6e67 6528 2d70 2c20 702b 3129 3a0a  range(-p, p+1):.
-0000cae0: 2020 2020 2020 2020 2020 2020 7173 6967              qsig
-0000caf0: 6e20 3d20 696e 7428 713c 3029 0a20 2020  n = int(q<0).   
-0000cb00: 2020 2020 2020 2020 2071 6162 7320 3d20           qabs = 
-0000cb10: 6162 7328 7129 0a20 2020 2020 2020 2020  abs(q).         
-0000cb20: 2020 2072 6f77 5f73 7472 203d 2066 2253     row_str = f"S
-0000cb30: 7b70 7d7b 717d 222e 6c6a 7573 7428 3429  {p}{q}".ljust(4)
-0000cb40: 0a0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
-0000cb50: 5072 696e 7420 6578 6369 7461 7469 6f6e  Print excitation
-0000cb60: 206d 6f6d 656e 7473 2061 7320 636f 6c75   moments as colu
-0000cb70: 6d6e 730a 2020 2020 2020 2020 2020 2020  mns.            
-0000cb80: 666f 7220 6e20 696e 2072 616e 6765 2831  for n in range(1
-0000cb90: 2c20 6e5f 6d61 782b 3129 3a0a 2020 2020  , n_max+1):.    
-0000cba0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-0000cbb0: 6d20 696e 2072 616e 6765 282d 6e2c 206e  m in range(-n, n
-0000cbc0: 2b31 293a 0a20 2020 2020 2020 2020 2020  +1):.           
-0000cbd0: 2020 2020 2020 2020 206d 7369 676e 203d           msign =
-0000cbe0: 2069 6e74 286d 3c30 290a 2020 2020 2020   int(m<0).      
-0000cbf0: 2020 2020 2020 2020 2020 2020 2020 6d61                ma
-0000cc00: 6273 203d 2061 6273 286d 290a 2020 2020  bs = abs(m).    
-0000cc10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cc20: 6365 6c6c 5f73 7472 203d 2022 7c20 220a  cell_str = "| ".
-0000cc30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000cc40: 2020 2020 2023 2050 7269 6e74 206e 6f6e       # Print non
-0000cc50: 2d7a 6572 6f20 7465 726d 7320 666f 7220  -zero terms for 
-0000cc60: 6561 6368 2063 656c 6c0a 2020 2020 2020  each cell.      
-0000cc70: 2020 2020 2020 2020 2020 2020 2020 666f                fo
-0000cc80: 7220 6e70 726d 2069 6e20 7261 6e67 6528  r nprm in range(
-0000cc90: 6e70 726d 5f6d 6178 2c20 302c 202d 3129  nprm_max, 0, -1)
-0000cca0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000ccb0: 2020 2020 2020 2020 2020 6d70 726d 203d            mprm =
-0000ccc0: 206d 202b 2071 0a20 2020 2020 2020 2020   m + q.         
-0000ccd0: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-0000cce0: 7073 6967 6e20 3d20 696e 7428 6d70 726d  psign = int(mprm
-0000ccf0: 3c30 290a 2020 2020 2020 2020 2020 2020  <0).            
-0000cd00: 2020 2020 2020 2020 2020 2020 6d70 6162              mpab
-0000cd10: 7320 3d20 6162 7328 6d70 726d 290a 0a20  s = abs(mprm).. 
-0000cd20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cd30: 2020 2020 2020 2074 6869 735f 5869 6420         this_Xid 
-0000cd40: 3d20 5869 645b 6d73 6967 6e2c 6e2c 6d61  = Xid[msign,n,ma
-0000cd50: 6273 2c20 7173 6967 6e2c 702c 7161 6273  bs, qsign,p,qabs
-0000cd60: 2c20 6d70 7369 676e 2c6e 7072 6d2c 6d70  , mpsign,nprm,mp
-0000cd70: 6162 735d 0a20 2020 2020 2020 2020 2020  abs].           
-0000cd80: 2020 2020 2020 2020 2020 2020 2061 6273               abs
-0000cd90: 5f58 6920 3d20 6162 7328 7468 6973 5f58  _Xi = abs(this_X
-0000cda0: 6964 290a 2020 2020 2020 2020 2020 2020  id).            
-0000cdb0: 2020 2020 2020 2020 2020 2020 726f 756e              roun
-0000cdc0: 645f 5869 203d 2072 6f75 6e64 2861 6273  d_Xi = round(abs
-0000cdd0: 2874 6869 735f 5869 6429 2c33 290a 2020  (this_Xid),3).  
-0000cde0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cdf0: 2020 2020 2020 6966 2861 6273 5f58 6920        if(abs_Xi 
-0000ce00: 3e20 3165 2d31 3829 3a0a 2020 2020 2020  > 1e-18):.      
-0000ce10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ce20: 2020 2020 2020 6966 2863 656c 6c5f 7374        if(cell_st
-0000ce30: 7220 213d 2022 7c20 2229 3a0a 2020 2020  r != "| "):.    
-0000ce40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ce50: 2020 2020 2020 2020 2020 2020 6966 2869              if(i
-0000ce60: 6e74 2874 6869 735f 5869 643e 3029 206f  nt(this_Xid>0) o
-0000ce70: 7220 726f 756e 645f 5869 3d3d 302e 3029  r round_Xi==0.0)
-0000ce80: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000ce90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cea0: 2020 2020 2020 6365 6c6c 5f73 7472 203d        cell_str =
-0000ceb0: 2066 227b 6365 6c6c 5f73 7472 7d2b 2022   f"{cell_str}+ "
-0000cec0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000ced0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cee0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-0000cef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cf00: 2020 2020 2020 2020 2020 2063 656c 6c5f             cell_
-0000cf10: 7374 7220 3d20 6622 7b63 656c 6c5f 7374  str = f"{cell_st
-0000cf20: 727d 2d20 220a 2020 2020 2020 2020 2020  r}- ".          
-0000cf30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cf40: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-0000cf50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cf60: 2020 2020 2020 2020 6966 2869 6e74 2874          if(int(t
-0000cf70: 6869 735f 5869 643e 3029 206f 7220 726f  his_Xid>0) or ro
-0000cf80: 756e 645f 5869 3d3d 302e 3029 3a0a 2020  und_Xi==0.0):.  
+00002650: 2020 2020 2020 2069 6620 6e70 2e69 6d61         if np.ima
+00002660: 6728 6570 735b 7173 6967 6e2c 2070 2c20  g(eps[qsign, p, 
+00002670: 7161 6273 5d29 203e 3d20 303a 0a20 2020  qabs]) >= 0:.   
+00002680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002690: 2020 2020 2020 2020 2062 7477 5f63 6861           btw_cha
+000026a0: 7220 3d20 222b 220a 2020 2020 2020 2020  r = "+".        
+000026b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000026c0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+000026d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000026e0: 2020 6274 775f 6368 6172 203d 2022 2d22    btw_char = "-"
+000026f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002700: 2020 2020 2020 2020 2074 6869 735f 6c69           this_li
+00002710: 6e65 203d 2066 227b 7468 6973 5f6c 696e  ne = f"{this_lin
+00002720: 657d 2c20 7b6e 702e 7265 616c 2865 7073  e}, {np.real(eps
+00002730: 5b71 7369 676e 2c20 702c 2071 6162 735d  [qsign, p, qabs]
+00002740: 297d 7b62 7477 5f63 6861 727d 7b6e 702e  )}{btw_char}{np.
+00002750: 6162 7328 6e70 2e69 6d61 6728 6570 735b  abs(np.imag(eps[
+00002760: 7173 6967 6e2c 2070 2c20 7161 6273 5d29  qsign, p, qabs])
+00002770: 297d 6a22 0a20 2020 2020 2020 2020 2020  )}j".           
+00002780: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
+00002790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000027a0: 2020 2020 2020 2074 6869 735f 6c69 6e65         this_line
+000027b0: 203d 2066 2220 7b70 7d2c 207b 7374 7228   = f" {p}, {str(
+000027c0: 7129 2e72 6a75 7374 2832 297d 2c20 7b6e  q).rjust(2)}, {n
+000027d0: 702e 7265 616c 2865 7073 5b71 7369 676e  p.real(eps[qsign
+000027e0: 2c20 702c 2071 6162 735d 297d 7b62 7477  , p, qabs])}{btw
+000027f0: 5f63 6861 727d 7b6e 702e 6162 7328 6e70  _char}{np.abs(np
+00002800: 2e69 6d61 6728 6570 735b 7173 6967 6e2c  .imag(eps[qsign,
+00002810: 2070 2c20 7161 6273 5d29 297d 5c6e 220a   p, qabs]))}\n".
+00002820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002830: 2020 2020 2020 2020 665f 6368 692e 7772          f_chi.wr
+00002840: 6974 6528 7468 6973 5f6c 696e 6529 0a20  ite(this_line). 
+00002850: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00002860: 6620 7072 696e 745f 666f 725f 636f 7079  f print_for_copy
+00002870: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00002880: 2020 2020 2020 665f 6368 692e 7772 6974        f_chi.writ
+00002890: 6528 7468 6973 5f6c 696e 652b 225c 6e22  e(this_line+"\n"
+000028a0: 290a 2020 2020 2020 2020 6c6f 672e 6465  ).        log.de
+000028b0: 6275 6728 6622 5072 696e 7465 6420 6368  bug(f"Printed ch
+000028c0: 695f 7071 2076 616c 7565 7320 746f 207b  i_pq values to {
+000028d0: 6173 796d 5f6f 7574 7d22 290a 0a20 2020  asym_out}")..   
+000028e0: 2023 2049 6620 7468 6973 2066 696c 6520   # If this file 
+000028f0: 6578 6973 7473 2c20 6d6f 6465 6c20 7469  exists, model ti
+00002900: 6461 6c20 7065 7274 7572 6261 7469 6f6e  dal perturbation
+00002910: 732e 2049 6620 6e6f 742c 2072 6574 7572  s. If not, retur
+00002920: 6e20 4e6f 6e65 2e0a 2020 2020 6772 6176  n None..    grav
+00002930: 5f6d 6f64 656c 203d 206f 732e 7061 7468  _model = os.path
+00002940: 2e6a 6f69 6e28 6670 6174 682c 2066 2267  .join(fpath, f"g
+00002950: 7261 7669 7479 7b62 666e 616d 657d 7b61  ravity{bfname}{a
+00002960: 7070 656e 647d 2e74 7874 2229 0a20 2020  ppend}.txt").   
+00002970: 2074 7279 3a0a 2020 2020 2020 2020 675f   try:.        g_
+00002980: 7368 6170 655f 6e20 3d20 6e70 2e6c 6f61  shape_n = np.loa
+00002990: 6474 7874 2867 7261 765f 6d6f 6465 6c2c  dtxt(grav_model,
+000029a0: 2073 6b69 7072 6f77 733d 312c 2075 6e70   skiprows=1, unp
+000029b0: 6163 6b3d 4661 6c73 652c 2064 656c 696d  ack=False, delim
+000029c0: 6974 6572 3d27 2c27 290a 2020 2020 6578  iter=',').    ex
+000029d0: 6365 7074 3a0a 2020 2020 2020 2020 6772  cept:.        gr
+000029e0: 6176 5f73 6861 7065 203d 204e 6f6e 650a  av_shape = None.
+000029f0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00002a00: 2020 6c6f 672e 6465 6275 6728 6622 5573    log.debug(f"Us
+00002a10: 696e 6720 7375 7266 6163 6520 6772 6176  ing surface grav
+00002a20: 6974 7920 7368 6170 653a 207b 6772 6176  ity shape: {grav
+00002a30: 5f6d 6f64 656c 7d22 290a 2020 2020 2020  _model}").      
+00002a40: 2020 666f 7220 7020 696e 2072 616e 6765    for p in range
+00002a50: 2831 2c20 705f 6d61 782b 3129 3a0a 2020  (1, p_max+1):.  
+00002a60: 2020 2020 2020 2020 2020 7468 6973 5f6d            this_m
+00002a70: 696e 203d 2069 6e74 2870 202a 2028 702b  in = int(p * (p+
+00002a80: 3129 202f 2032 290a 2020 2020 2020 2020  1) / 2).        
+00002a90: 2020 2020 7468 6973 5f6d 6178 203d 2074      this_max = t
+00002aa0: 6869 735f 6d69 6e20 2b20 702b 310a 2020  his_min + p+1.  
+00002ab0: 2020 2020 2020 2020 2020 2320 556e 6c69            # Unli
+00002ac0: 6b65 2061 626f 7665 2c20 7765 2064 6f20  ke above, we do 
+00002ad0: 6e6f 7420 6e65 6564 2074 6f20 6e65 6761  not need to nega
+00002ae0: 7465 2062 6563 6175 7365 2064 6576 6961  te because devia
+00002af0: 7469 6f6e 7320 6172 6520 616c 7265 6164  tions are alread
+00002b00: 7920 696e 2072 6164 6969 0a20 2020 2020  y in radii.     
+00002b10: 2020 2020 2020 2067 4370 7120 3d20 675f         gCpq = g_
+00002b20: 7368 6170 655f 6e5b 7468 6973 5f6d 696e  shape_n[this_min
+00002b30: 3a74 6869 735f 6d61 782c 2032 5d0a 2020  :this_max, 2].  
+00002b40: 2020 2020 2020 2020 2020 6753 7071 203d            gSpq =
+00002b50: 2067 5f73 6861 7065 5f6e 5b74 6869 735f   g_shape_n[this_
+00002b60: 6d69 6e3a 7468 6973 5f6d 6178 2c20 335d  min:this_max, 3]
+00002b70: 0a0a 2020 2020 2020 2020 2020 2020 675f  ..            g_
+00002b80: 6368 695f 7071 7320 3d20 6765 745f 6368  chi_pqs = get_ch
+00002b90: 6970 715f 6672 6f6d 5f43 5370 715f 7369  ipq_from_CSpq_si
+00002ba0: 6e67 6c65 2870 2c20 6743 7071 2c20 6753  ngle(p, gCpq, gS
+00002bb0: 7071 290a 2020 2020 2020 2020 2020 2020  pq).            
+00002bc0: 666f 7220 6969 2069 6e20 7261 6e67 6528  for ii in range(
+00002bd0: 6e5f 6264 7320 2b20 725f 696f 202b 2031  n_bds + r_io + 1
+00002be0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00002bf0: 2020 2023 2049 6620 7765 2061 7265 206d     # If we are m
+00002c00: 6f64 656c 696e 6720 6173 796d 6d65 7472  odeling asymmetr
+00002c10: 7920 696e 2061 6e79 2073 7572 6661 6365  y in any surface
+00002c20: 2c20 6974 2069 7320 6164 6a61 6365 6e74  , it is adjacent
+00002c30: 2074 6f20 6120 636f 6e64 7563 7469 6e67   to a conducting
+00002c40: 206c 6179 6572 0a20 2020 2020 2020 2020   layer.         
+00002c50: 2020 2020 2020 2069 6620 2861 7379 6d5f         if (asym_
+00002c60: 7368 6170 655b 6969 2c20 2e2e 2e5d 2021  shape[ii, ...] !
+00002c70: 3d20 3029 2e61 6e79 2829 3a0a 2020 2020  = 0).any():.    
+00002c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002c90: 2320 4170 706c 7920 7375 7266 6163 6520  # Apply surface 
+00002ca0: 7469 6461 6c20 7065 7274 7572 6261 7469  tidal perturbati
+00002cb0: 6f6e 7320 746f 2061 6c6c 2061 7379 6d6d  ons to all asymm
+00002cc0: 6574 7269 6320 6c61 7965 7273 2065 7175  etric layers equ
+00002cd0: 616c 6c79 0a20 2020 2020 2020 2020 2020  ally.           
+00002ce0: 2020 2020 2020 2020 2023 2028 746f 2070           # (to p
+00002cf0: 7265 7365 7276 6520 7468 6963 6b6e 6573  reserve thicknes
+00002d00: 7365 7320 6465 7465 726d 696e 6564 2062  ses determined b
+00002d10: 7920 7468 6572 6d6f 6479 6e61 6d69 6373  y thermodynamics
+00002d20: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00002d30: 2020 2020 2020 6772 6176 5f73 6861 7065        grav_shape
+00002d40: 5b69 692c 203a 2c20 702c 203a 702b 315d  [ii, :, p, :p+1]
+00002d50: 203d 2067 5f63 6869 5f70 7173 202a 2031   = g_chi_pqs * 1
+00002d60: 6533 0a0a 2020 2020 2020 2020 2020 2020  e3..            
+00002d70: 2320 416c 7761 7973 2061 6464 2070 6572  # Always add per
+00002d80: 7475 7262 6174 696f 6e20 746f 2062 6f64  turbation to bod
+00002d90: 7920 7375 7266 6163 650a 2020 2020 2020  y surface.      
+00002da0: 2020 2020 2020 6772 6176 5f73 6861 7065        grav_shape
+00002db0: 5b6e 5f62 6473 2b72 5f69 6f2b 312c 203a  [n_bds+r_io+1, :
+00002dc0: 2c20 702c 203a 702b 315d 203d 2067 5f63  , p, :p+1] = g_c
+00002dd0: 6869 5f70 7173 202a 2031 6533 0a20 2020  hi_pqs * 1e3.   
+00002de0: 2072 6574 7572 6e20 6173 796d 5f73 6861   return asym_sha
+00002df0: 7065 2c20 6772 6176 5f73 6861 7065 0a0a  pe, grav_shape..
+00002e00: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00002e10: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00002e20: 2323 2323 2323 2323 2323 2323 230a 0a22  #############.."
+00002e30: 2222 0a67 6574 5f63 6869 7071 5f66 726f  "".get_chipq_fro
+00002e40: 6d5f 4353 7071 5f73 696e 676c 6528 290a  m_CSpq_single().
+00002e50: 2020 2020 436f 6e76 6572 7420 6672 6f6d      Convert from
+00002e60: 2072 6561 6c2c 2034 7069 2d6e 6f72 6d61   real, 4pi-norma
+00002e70: 6c69 7a65 6420 6861 726d 6f6e 6963 2063  lized harmonic c
+00002e80: 6f65 6666 6963 6965 6e74 7320 7769 7468  oefficients with
+00002e90: 206e 6f20 436f 6e64 6f6e 2d53 686f 7274   no Condon-Short
+00002ea0: 6c65 7920 7068 6173 650a 2020 2020 2874  ley phase.    (t
+00002eb0: 6865 2063 6f6d 6d6f 6e20 6e6f 726d 616c  he common normal
+00002ec0: 697a 6174 696f 6e20 696e 2074 6865 2067  ization in the g
+00002ed0: 656f 6465 7379 2063 6f6d 6d75 6e69 7479  eodesy community
+00002ee0: 2920 746f 206f 7274 686f 6e6f 726d 616c  ) to orthonormal
+00002ef0: 2068 6172 6d6f 6e69 6320 636f 6566 6669   harmonic coeffi
+00002f00: 6369 656e 7473 2068 6176 696e 670a 2020  cients having.  
+00002f10: 2020 7468 6520 432d 5320 7068 6173 652e    the C-S phase.
+00002f20: 2048 616e 646c 6573 2061 6c6c 2076 616c   Handles all val
+00002f30: 7565 7320 666f 7220 6120 6769 7665 6e20  ues for a given 
+00002f40: 7020 6174 206f 6e63 652e 0a20 2020 2055  p at once..    U
+00002f50: 7361 6765 3a20 6063 6869 7071 6020 3d20  sage: `chipq` = 
+00002f60: 6765 745f 6368 6970 715f 6672 6f6d 5f43  get_chipq_from_C
+00002f70: 5370 715f 7369 6e67 6c65 2860 7060 2c60  Spq_single(`p`,`
+00002f80: 4370 7160 2c60 5370 7160 290a 2020 2020  Cpq`,`Spq`).    
+00002f90: 5265 7475 726e 733a 0a20 2020 2020 2020  Returns:.       
+00002fa0: 2063 6869 7071 3a20 636f 6d70 6c65 782c   chipq: complex,
+00002fb0: 2073 6861 7065 2832 2c70 2b31 292e 2063   shape(2,p+1). c
+00002fc0: 6869 5f70 7120 7661 6c75 6573 2066 6f72  hi_pq values for
+00002fd0: 2061 6c6c 2071 203d 205b 2d70 2c70 5d2c   all q = [-p,p],
+00002fe0: 206f 7267 616e 697a 6564 2073 7563 6820   organized such 
+00002ff0: 7468 6174 2063 6869 7071 5b69 6e74 2871  that chipq[int(q
+00003000: 3c30 292c 6162 7328 7129 5d0a 2020 2020  <0),abs(q)].    
+00003010: 2020 2020 2020 2020 7265 7475 726e 7320          returns 
+00003020: 7468 6520 7265 7375 6c74 2066 6f72 2061  the result for a
+00003030: 2070 6172 7469 6375 6c61 7220 7120 7661   particular q va
+00003040: 6c75 652e 204f 7274 686f 6e6f 726d 616c  lue. Orthonormal
+00003050: 2c20 7769 7468 2043 6f6e 646f 6e2d 5368  , with Condon-Sh
+00003060: 6f72 746c 6579 2070 6861 7365 2e0a 2020  ortley phase..  
+00003070: 2020 2020 2020 2020 2020 4f72 7468 6f6e            Orthon
+00003080: 6f72 6d61 6c20 6865 7265 206d 6561 6e73  ormal here means
+00003090: 2074 6865 2069 6e74 6567 7261 6c20 6f66   the integral of
+000030a0: 207c 596e 6d7c 5e32 202a 2064 4f6d 6567   |Ynm|^2 * dOmeg
+000030b0: 6120 6f76 6572 2061 2075 6e69 7420 7370  a over a unit sp
+000030c0: 6865 7265 2069 7320 3120 666f 7220 616c  here is 1 for al
+000030d0: 6c20 6e20 616e 6420 6d2e 0a20 2020 2050  l n and m..    P
+000030e0: 6172 616d 6574 6572 733a 0a20 2020 2020  arameters:.     
+000030f0: 2020 2070 3a20 696e 7465 6765 722e 2044     p: integer. D
+00003100: 6567 7265 6520 6f66 2062 6f75 6e64 6172  egree of boundar
+00003110: 7920 7368 6170 6573 3b20 7265 7375 6c74  y shapes; result
+00003120: 7320 666f 7220 616c 6c20 7120 7661 6c75  s for all q valu
+00003130: 6573 2061 7265 2072 6574 7572 6e65 6420  es are returned 
+00003140: 666f 7220 7468 6973 2070 2076 616c 7565  for this p value
+00003150: 2e0a 2020 2020 2020 2020 4370 713a 2066  ..        Cpq: f
+00003160: 6c6f 6174 2e20 5370 6865 7269 6361 6c20  loat. Spherical 
+00003170: 6861 726d 6f6e 6963 2063 6f65 6666 6963  harmonic coeffic
+00003180: 6965 6e74 2074 6861 7420 6d75 6c74 6970  ient that multip
+00003190: 6c69 6573 2063 6f73 286d 2a70 6869 2920  lies cos(m*phi) 
+000031a0: 666f 7220 702c 7120 626f 756e 6461 7279  for p,q boundary
+000031b0: 2e20 3470 692d 6e6f 726d 616c 697a 6564  . 4pi-normalized
+000031c0: 2077 6974 6820 6e6f 2043 6f6e 646f 6e2d   with no Condon-
+000031d0: 5368 6f72 746c 6579 2070 6861 7365 2e0a  Shortley phase..
+000031e0: 2020 2020 2020 2020 5370 713a 2066 6c6f          Spq: flo
+000031f0: 6174 2e20 5370 6865 7269 6361 6c20 6861  at. Spherical ha
+00003200: 726d 6f6e 6963 2063 6f65 6666 6963 6965  rmonic coefficie
+00003210: 6e74 2074 6861 7420 6d75 6c74 6970 6c69  nt that multipli
+00003220: 6573 2073 696e 286d 2a70 6869 2920 666f  es sin(m*phi) fo
+00003230: 7220 702c 7120 626f 756e 6461 7279 2e20  r p,q boundary. 
+00003240: 3470 692d 6e6f 726d 616c 697a 6564 2077  4pi-normalized w
+00003250: 6974 6820 6e6f 2043 6f6e 646f 6e2d 5368  ith no Condon-Sh
+00003260: 6f72 746c 6579 2070 6861 7365 2e0a 2020  ortley phase..  
+00003270: 2020 2020 2020 4353 6368 616e 6765 3a20        CSchange: 
+00003280: 626f 6f6c 2028 5472 7565 292e 2049 6620  bool (True). If 
+00003290: 4661 6c73 652c 2064 6f20 4e4f 5420 636f  False, do NOT co
+000032a0: 7272 6563 7420 666f 7220 436f 6e64 6f6e  rrect for Condon
+000032b0: 2d53 686f 7274 6c65 7920 7068 6173 652c  -Shortley phase,
+000032c0: 2069 2e65 2e20 7265 7475 726e 2067 6e6d   i.e. return gnm
+000032d0: 2c20 686e 6d0a 2020 2020 2020 2020 2020  , hnm.          
+000032e0: 2020 7468 6174 2063 6f6e 7461 696e 2074    that contain t
+000032f0: 6865 2043 5320 7068 6173 652e 0a20 2020  he CS phase..   
+00003300: 2022 2222 0a64 6566 2067 6574 5f63 6869   """.def get_chi
+00003310: 7071 5f66 726f 6d5f 4353 7071 5f73 696e  pq_from_CSpq_sin
+00003320: 676c 6528 702c 2043 7071 2c20 5370 712c  gle(p, Cpq, Spq,
+00003330: 2043 5363 6861 6e67 653d 5472 7565 293a   CSchange=True):
+00003340: 0a20 2020 2063 6869 7071 203d 206e 702e  .    chipq = np.
+00003350: 7a65 726f 7328 2832 2c70 2b31 292c 6474  zeros((2,p+1),dt
+00003360: 7970 653d 6e70 2e63 6f6d 706c 6578 5f29  ype=np.complex_)
+00003370: 0a0a 2020 2020 6e6f 726d 203d 2073 7172  ..    norm = sqr
+00003380: 7434 7069 202f 2073 7172 7432 0a0a 2020  t4pi / sqrt2..  
+00003390: 2020 666f 7220 7120 696e 2072 616e 6765    for q in range
+000033a0: 2831 2c70 2b31 293a 0a20 2020 2020 2020  (1,p+1):.       
+000033b0: 2023 204e 6567 6174 6976 6520 7120 2866   # Negative q (f
+000033c0: 6972 7374 2069 6e64 6578 2031 293a 0a20  irst index 1):. 
+000033d0: 2020 2020 2020 2063 6869 7071 5b31 2c71         chipq[1,q
+000033e0: 5d20 3d20 2843 7071 5b71 5d20 2b20 316a  ] = (Cpq[q] + 1j
+000033f0: 2a53 7071 5b71 5d29 202a 206e 6f72 6d0a  *Spq[q]) * norm.
+00003400: 2020 2020 2020 2020 2320 506f 7369 7469          # Positi
+00003410: 7665 2071 2028 6669 7273 7420 696e 6465  ve q (first inde
+00003420: 7820 3029 3a0a 2020 2020 2020 2020 6368  x 0):.        ch
+00003430: 6970 715b 302c 715d 203d 2028 2d31 292a  ipq[0,q] = (-1)*
+00003440: 2a28 712a 4353 6368 616e 6765 2920 2a20  *(q*CSchange) * 
+00003450: 2843 7071 5b71 5d20 2d20 316a 2a53 7071  (Cpq[q] - 1j*Spq
+00003460: 5b71 5d29 202a 206e 6f72 6d0a 0a20 2020  [q]) * norm..   
+00003470: 2063 6869 7071 5b30 2c30 5d20 3d20 4370   chipq[0,0] = Cp
+00003480: 715b 305d 202a 2073 7172 7434 7069 0a0a  q[0] * sqrt4pi..
+00003490: 2020 2020 7265 7475 726e 2063 6869 7071      return chipq
+000034a0: 0a0a 2323 2323 2323 2323 2323 2323 2323  ..##############
+000034b0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000034c0: 2323 2323 2323 2323 2323 2323 2323 230a  ###############.
+000034d0: 0a22 2222 0a67 6574 5f63 6869 7071 5f66  .""".get_chipq_f
+000034e0: 726f 6d5f 4353 7071 2829 0a20 2020 2043  rom_CSpq().    C
+000034f0: 6f6e 7665 7274 2066 726f 6d20 7265 616c  onvert from real
+00003500: 2c20 3470 692d 6e6f 726d 616c 697a 6564  , 4pi-normalized
+00003510: 2068 6172 6d6f 6e69 6320 636f 6566 6669   harmonic coeffi
+00003520: 6369 656e 7473 2077 6974 6820 6e6f 2043  cients with no C
+00003530: 6f6e 646f 6e2d 5368 6f72 746c 6579 2070  ondon-Shortley p
+00003540: 6861 7365 0a20 2020 2028 7468 6520 636f  hase.    (the co
+00003550: 6d6d 6f6e 206e 6f72 6d61 6c69 7a61 7469  mmon normalizati
+00003560: 6f6e 2069 6e20 7468 6520 6765 6f64 6573  on in the geodes
+00003570: 7920 636f 6d6d 756e 6974 7929 2074 6f20  y community) to 
+00003580: 6f72 7468 6f6e 6f72 6d61 6c20 6861 726d  orthonormal harm
+00003590: 6f6e 6963 2063 6f65 6666 6963 6965 6e74  onic coefficient
+000035a0: 7320 6861 7669 6e67 0a20 2020 2074 6865  s having.    the
+000035b0: 2043 2d53 2070 6861 7365 2e20 4861 6e64   C-S phase. Hand
+000035c0: 6c65 7320 616c 6c20 7661 6c75 6573 2061  les all values a
+000035d0: 7420 6f6e 6365 2e0a 2020 2020 5573 6167  t once..    Usag
+000035e0: 653a 2060 6368 6970 7160 203d 2067 6574  e: `chipq` = get
+000035f0: 5f63 6869 7071 5f66 726f 6d5f 4353 7071  _chipq_from_CSpq
+00003600: 2860 706d 6178 602c 6043 7071 602c 6053  (`pmax`,`Cpq`,`S
+00003610: 7071 6029 0a20 2020 2052 6574 7572 6e73  pq`).    Returns
+00003620: 3a0a 2020 2020 2020 2020 6368 6970 713a  :.        chipq:
+00003630: 2063 6f6d 706c 6578 2c20 7368 6170 6528   complex, shape(
+00003640: 322c 706d 6178 2b31 2c70 6d61 782b 3129  2,pmax+1,pmax+1)
+00003650: 2e20 6368 695f 7071 2076 616c 7565 7320  . chi_pq values 
+00003660: 666f 7220 616c 6c20 7120 3d20 5b2d 702c  for all q = [-p,
+00003670: 705d 2066 6f72 2070 2075 7020 746f 2070  p] for p up to p
+00003680: 6d61 782c 0a20 2020 2020 2020 2020 2020  max,.           
+00003690: 206f 7267 616e 697a 6564 2073 7563 6820   organized such 
+000036a0: 7468 6174 2063 6869 7071 5b69 6e74 2871  that chipq[int(q
+000036b0: 3c30 292c 702c 6162 7328 7129 5d20 7265  <0),p,abs(q)] re
+000036c0: 7475 726e 7320 7468 6520 7265 7375 6c74  turns the result
+000036d0: 2066 6f72 2061 2070 6172 7469 6375 6c61   for a particula
+000036e0: 7220 7120 7661 6c75 652e 0a20 2020 2020  r q value..     
+000036f0: 2020 2020 2020 204f 7274 686f 6e6f 726d         Orthonorm
+00003700: 616c 2c20 7769 7468 2043 6f6e 646f 6e2d  al, with Condon-
+00003710: 5368 6f72 746c 6579 2070 6861 7365 2e20  Shortley phase. 
+00003720: 4f72 7468 6f6e 6f72 6d61 6c20 6865 7265  Orthonormal here
+00003730: 206d 6561 6e73 2074 6865 2069 6e74 6567   means the integ
+00003740: 7261 6c20 6f66 0a20 2020 2020 2020 2020  ral of.         
+00003750: 2020 207c 596e 6d7c 5e32 202a 2064 4f6d     |Ynm|^2 * dOm
+00003760: 6567 6120 6f76 6572 2061 2075 6e69 7420  ega over a unit 
+00003770: 7370 6865 7265 2069 7320 3120 666f 7220  sphere is 1 for 
+00003780: 616c 6c20 6e20 616e 6420 6d2e 0a20 2020  all n and m..   
+00003790: 2050 6172 616d 6574 6572 733a 0a20 2020   Parameters:.   
+000037a0: 2020 2020 2070 6d61 783a 2069 6e74 6567       pmax: integ
+000037b0: 6572 2e20 4d61 7869 6d75 6d20 6465 6772  er. Maximum degr
+000037c0: 6565 206f 6620 626f 756e 6461 7279 2073  ee of boundary s
+000037d0: 6861 7065 733b 2072 6573 756c 7473 2066  hapes; results f
+000037e0: 6f72 2061 6c6c 2070 2061 6e64 2071 2076  or all p and q v
+000037f0: 616c 7565 7320 7570 2074 6f20 7468 6973  alues up to this
+00003800: 2070 6d61 7820 6172 6520 7265 7475 726e   pmax are return
+00003810: 6564 2e0a 2020 2020 2020 2020 4370 713a  ed..        Cpq:
+00003820: 2066 6c6f 6174 2c20 7368 6170 6528 706d   float, shape(pm
+00003830: 6178 2b31 2c70 6d61 782b 3129 2e20 5370  ax+1,pmax+1). Sp
+00003840: 6865 7269 6361 6c20 6861 726d 6f6e 6963  herical harmonic
+00003850: 2063 6f65 6666 6963 6965 6e74 2074 6861   coefficient tha
+00003860: 7420 6d75 6c74 6970 6c69 6573 2063 6f73  t multiplies cos
+00003870: 286d 2a70 6869 2920 666f 7220 702c 7120  (m*phi) for p,q 
+00003880: 626f 756e 6461 7279 2e20 3470 692d 6e6f  boundary. 4pi-no
+00003890: 726d 616c 697a 6564 2077 6974 6820 6e6f  rmalized with no
+000038a0: 2043 6f6e 646f 6e2d 5368 6f72 746c 6579   Condon-Shortley
+000038b0: 2070 6861 7365 2e0a 2020 2020 2020 2020   phase..        
+000038c0: 5370 713a 2066 6c6f 6174 2c20 7368 6170  Spq: float, shap
+000038d0: 6528 706d 6178 2b31 2c70 6d61 782b 3129  e(pmax+1,pmax+1)
+000038e0: 2e20 5370 6865 7269 6361 6c20 6861 726d  . Spherical harm
+000038f0: 6f6e 6963 2063 6f65 6666 6963 6965 6e74  onic coefficient
+00003900: 2074 6861 7420 6d75 6c74 6970 6c69 6573   that multiplies
+00003910: 2073 696e 286d 2a70 6869 2920 666f 7220   sin(m*phi) for 
+00003920: 702c 7120 626f 756e 6461 7279 2e20 3470  p,q boundary. 4p
+00003930: 692d 6e6f 726d 616c 697a 6564 2077 6974  i-normalized wit
+00003940: 6820 6e6f 2043 6f6e 646f 6e2d 5368 6f72  h no Condon-Shor
+00003950: 746c 6579 2070 6861 7365 2e0a 2020 2020  tley phase..    
+00003960: 2020 2020 4353 6368 616e 6765 3a20 626f      CSchange: bo
+00003970: 6f6c 2028 5472 7565 292e 2049 6620 4661  ol (True). If Fa
+00003980: 6c73 652c 2064 6f20 4e4f 5420 636f 7272  lse, do NOT corr
+00003990: 6563 7420 666f 7220 436f 6e64 6f6e 2d53  ect for Condon-S
+000039a0: 686f 7274 6c65 7920 7068 6173 652c 2069  hortley phase, i
+000039b0: 2e65 2e20 7265 7475 726e 2067 6e6d 2c20  .e. return gnm, 
+000039c0: 686e 6d0a 2020 2020 2020 2020 2020 2020  hnm.            
+000039d0: 7468 6174 2063 6f6e 7461 696e 2074 6865  that contain the
+000039e0: 2043 5320 7068 6173 652e 0a20 2020 2022   CS phase..    "
+000039f0: 2222 0a64 6566 2067 6574 5f63 6869 7071  "".def get_chipq
+00003a00: 5f66 726f 6d5f 4353 7071 2870 6d61 782c  _from_CSpq(pmax,
+00003a10: 2043 7071 2c20 5370 712c 2043 5363 6861   Cpq, Spq, CScha
+00003a20: 6e67 653d 5472 7565 293a 0a20 2020 2063  nge=True):.    c
+00003a30: 6869 7071 203d 206e 702e 7a65 726f 7328  hipq = np.zeros(
+00003a40: 2832 2c70 6d61 782b 312c 706d 6178 2b31  (2,pmax+1,pmax+1
+00003a50: 292c 6474 7970 653d 6e70 2e63 6f6d 706c  ),dtype=np.compl
+00003a60: 6578 5f29 0a0a 2020 2020 6e6f 726d 203d  ex_)..    norm =
+00003a70: 2073 7172 7434 7069 202f 2073 7172 7432   sqrt4pi / sqrt2
+00003a80: 0a0a 2020 2020 666f 7220 7020 696e 2072  ..    for p in r
+00003a90: 616e 6765 2870 6d61 782b 3129 3a0a 2020  ange(pmax+1):.  
+00003aa0: 2020 2020 2020 666f 7220 7120 696e 2072        for q in r
+00003ab0: 616e 6765 2831 2c20 702b 3129 3a0a 2020  ange(1, p+1):.  
+00003ac0: 2020 2020 2020 2020 2020 2320 4e65 6761            # Nega
+00003ad0: 7469 7665 2071 2028 6669 7273 7420 696e  tive q (first in
+00003ae0: 6465 7820 3129 3a0a 2020 2020 2020 2020  dex 1):.        
+00003af0: 2020 2020 6368 6970 715b 312c 702c 715d      chipq[1,p,q]
+00003b00: 203d 2028 4370 715b 702c 715d 202b 2031   = (Cpq[p,q] + 1
+00003b10: 6a2a 5370 715b 702c 715d 2920 2a20 6e6f  j*Spq[p,q]) * no
+00003b20: 726d 0a20 2020 2020 2020 2020 2020 2023  rm.            #
+00003b30: 2050 6f73 6974 6976 6520 7120 2866 6972   Positive q (fir
+00003b40: 7374 2069 6e64 6578 2030 293a 0a20 2020  st index 0):.   
+00003b50: 2020 2020 2020 2020 2063 6869 7071 5b30           chipq[0
+00003b60: 2c70 2c71 5d20 3d20 282d 3129 2a2a 2871  ,p,q] = (-1)**(q
+00003b70: 2a43 5363 6861 6e67 6529 202a 2028 4370  *CSchange) * (Cp
+00003b80: 715b 702c 715d 202d 2031 6a2a 5370 715b  q[p,q] - 1j*Spq[
+00003b90: 702c 715d 2920 2a20 6e6f 726d 0a0a 2020  p,q]) * norm..  
+00003ba0: 2020 2020 2020 6368 6970 715b 302c 702c        chipq[0,p,
+00003bb0: 305d 203d 2043 7071 5b70 2c30 5d20 2a20  0] = Cpq[p,0] * 
+00003bc0: 7371 7274 3470 690a 0a20 2020 2072 6574  sqrt4pi..    ret
+00003bd0: 7572 6e20 6368 6970 710a 0a23 2323 2323  urn chipq..#####
+00003be0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00003bf0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00003c00: 2323 2323 2323 2323 0a0a 2222 220a 6765  ########..""".ge
+00003c10: 745f 4353 7071 5f66 726f 6d5f 6368 6970  t_CSpq_from_chip
+00003c20: 7128 290a 2020 2020 436f 6e76 6572 7420  q().    Convert 
+00003c30: 6672 6f6d 206f 7274 686f 6e6f 726d 616c  from orthonormal
+00003c40: 2068 6172 6d6f 6e69 6320 636f 6566 6669   harmonic coeffi
+00003c50: 6369 656e 7473 2068 6176 696e 6720 7468  cients having th
+00003c60: 6520 432d 5320 7068 6173 6520 746f 2072  e C-S phase to r
+00003c70: 6561 6c2c 2034 7069 2d6e 6f72 6d61 6c69  eal, 4pi-normali
+00003c80: 7a65 640a 2020 2020 6861 726d 6f6e 6963  zed.    harmonic
+00003c90: 2063 6f65 6666 6963 6965 6e74 7320 7769   coefficients wi
+00003ca0: 7468 206e 6f20 436f 6e64 6f6e 2d53 686f  th no Condon-Sho
+00003cb0: 7274 6c65 7920 7068 6173 652e 2048 616e  rtley phase. Han
+00003cc0: 646c 6573 2061 6c6c 2076 616c 7565 7320  dles all values 
+00003cd0: 6174 206f 6e63 652e 0a20 2020 2055 7361  at once..    Usa
+00003ce0: 6765 3a20 6043 7071 602c 2060 5370 7160  ge: `Cpq`, `Spq`
+00003cf0: 203d 2067 6574 5f63 6869 7071 5f66 726f   = get_chipq_fro
+00003d00: 6d5f 4353 7071 2860 706d 6178 602c 6063  m_CSpq(`pmax`,`c
+00003d10: 6869 7071 6029 0a20 2020 2052 6574 7572  hipq`).    Retur
+00003d20: 6e73 3a0a 2020 2020 2020 2020 4370 713a  ns:.        Cpq:
+00003d30: 2066 6c6f 6174 2c20 7368 6170 6528 706d   float, shape(pm
+00003d40: 6178 2b31 2c70 6d61 782b 3129 2e20 5370  ax+1,pmax+1). Sp
+00003d50: 6865 7269 6361 6c20 6861 726d 6f6e 6963  herical harmonic
+00003d60: 2063 6f65 6666 6963 6965 6e74 2074 6861   coefficient tha
+00003d70: 7420 6d75 6c74 6970 6c69 6573 2063 6f73  t multiplies cos
+00003d80: 286d 2a70 6869 2920 666f 7220 702c 7120  (m*phi) for p,q 
+00003d90: 626f 756e 6461 7279 2e20 3470 692d 6e6f  boundary. 4pi-no
+00003da0: 726d 616c 697a 6564 2077 6974 6820 6e6f  rmalized with no
+00003db0: 2043 6f6e 646f 6e2d 5368 6f72 746c 6579   Condon-Shortley
+00003dc0: 2070 6861 7365 2e0a 2020 2020 2020 2020   phase..        
+00003dd0: 5370 713a 2066 6c6f 6174 2c20 7368 6170  Spq: float, shap
+00003de0: 6528 706d 6178 2b31 2c70 6d61 782b 3129  e(pmax+1,pmax+1)
+00003df0: 2e20 5370 6865 7269 6361 6c20 6861 726d  . Spherical harm
+00003e00: 6f6e 6963 2063 6f65 6666 6963 6965 6e74  onic coefficient
+00003e10: 2074 6861 7420 6d75 6c74 6970 6c69 6573   that multiplies
+00003e20: 2073 696e 286d 2a70 6869 2920 666f 7220   sin(m*phi) for 
+00003e30: 702c 7120 626f 756e 6461 7279 2e20 3470  p,q boundary. 4p
+00003e40: 692d 6e6f 726d 616c 697a 6564 2077 6974  i-normalized wit
+00003e50: 6820 6e6f 2043 6f6e 646f 6e2d 5368 6f72  h no Condon-Shor
+00003e60: 746c 6579 2070 6861 7365 2e0a 2020 2020  tley phase..    
+00003e70: 5061 7261 6d65 7465 7273 3a0a 2020 2020  Parameters:.    
+00003e80: 2020 2020 706d 6178 3a20 696e 7465 6765      pmax: intege
+00003e90: 722e 204d 6178 696d 756d 2064 6567 7265  r. Maximum degre
+00003ea0: 6520 6f66 2062 6f75 6e64 6172 7920 7368  e of boundary sh
+00003eb0: 6170 6573 3b20 7265 7375 6c74 7320 666f  apes; results fo
+00003ec0: 7220 616c 6c20 7020 616e 6420 7120 7661  r all p and q va
+00003ed0: 6c75 6573 2075 7020 746f 2074 6869 7320  lues up to this 
+00003ee0: 706d 6178 2061 7265 2072 6574 7572 6e65  pmax are returne
+00003ef0: 642e 0a20 2020 2020 2020 2063 6869 7071  d..        chipq
+00003f00: 3a20 636f 6d70 6c65 782c 2073 6861 7065  : complex, shape
+00003f10: 2832 2c70 6d61 782b 312c 706d 6178 2b31  (2,pmax+1,pmax+1
+00003f20: 292e 2063 6869 5f70 7120 7661 6c75 6573  ). chi_pq values
+00003f30: 2066 6f72 2061 6c6c 2071 203d 205b 2d70   for all q = [-p
+00003f40: 2c70 5d20 666f 7220 7020 7570 2074 6f20  ,p] for p up to 
+00003f50: 706d 6178 2c0a 2020 2020 2020 2020 2020  pmax,.          
+00003f60: 2020 6f72 6761 6e69 7a65 6420 7375 6368    organized such
+00003f70: 2074 6861 7420 6368 6970 715b 696e 7428   that chipq[int(
+00003f80: 713c 3029 2c70 2c61 6273 2871 295d 2072  q<0),p,abs(q)] r
+00003f90: 6574 7572 6e73 2074 6865 2072 6573 756c  eturns the resul
+00003fa0: 7420 666f 7220 6120 7061 7274 6963 756c  t for a particul
+00003fb0: 6172 2071 2076 616c 7565 2e0a 2020 2020  ar q value..    
+00003fc0: 2020 2020 2020 2020 4f72 7468 6f6e 6f72          Orthonor
+00003fd0: 6d61 6c2c 2077 6974 6820 436f 6e64 6f6e  mal, with Condon
+00003fe0: 2d53 686f 7274 6c65 7920 7068 6173 652e  -Shortley phase.
+00003ff0: 204f 7274 686f 6e6f 726d 616c 2068 6572   Orthonormal her
+00004000: 6520 6d65 616e 7320 7468 6520 696e 7465  e means the inte
+00004010: 6772 616c 206f 660a 2020 2020 2020 2020  gral of.        
+00004020: 2020 2020 7c59 6e6d 7c5e 3220 2a20 644f      |Ynm|^2 * dO
+00004030: 6d65 6761 206f 7665 7220 6120 756e 6974  mega over a unit
+00004040: 2073 7068 6572 6520 6973 2031 2066 6f72   sphere is 1 for
+00004050: 2061 6c6c 206e 2061 6e64 206d 2e0a 2020   all n and m..  
+00004060: 2020 2020 2020 4353 6368 616e 6765 3a20        CSchange: 
+00004070: 626f 6f6c 2028 5472 7565 292e 2049 6620  bool (True). If 
+00004080: 4661 6c73 652c 2064 6f20 4e4f 5420 636f  False, do NOT co
+00004090: 7272 6563 7420 666f 7220 436f 6e64 6f6e  rrect for Condon
+000040a0: 2d53 686f 7274 6c65 7920 7068 6173 652c  -Shortley phase,
+000040b0: 2069 2e65 2e20 7265 7475 726e 2067 6e6d   i.e. return gnm
+000040c0: 2c20 686e 6d0a 2020 2020 2020 2020 2020  , hnm.          
+000040d0: 2020 7468 6174 2063 6f6e 7461 696e 2074    that contain t
+000040e0: 6865 2043 5320 7068 6173 652e 0a20 2020  he CS phase..   
+000040f0: 2020 2020 206e 6f52 656e 6f72 6d3a 2062       noRenorm: b
+00004100: 6f6f 6c20 2846 616c 7365 292e 2049 6620  ool (False). If 
+00004110: 5472 7565 2c20 7265 7475 726e 2043 7071  True, return Cpq
+00004120: 2061 6e64 2053 7071 2061 7320 6675 6c6c   and Spq as full
+00004130: 7920 6e6f 726d 616c 697a 6564 2c20 7265  y normalized, re
+00004140: 616c 2068 6172 6d6f 6e69 6320 636f 6566  al harmonic coef
+00004150: 6669 6369 656e 7473 2e0a 2020 2020 2222  ficients..    ""
+00004160: 220a 6465 6620 6765 745f 4353 7071 5f66  ".def get_CSpq_f
+00004170: 726f 6d5f 6368 6970 7128 706d 6178 2c20  rom_chipq(pmax, 
+00004180: 6368 6970 712c 2043 5363 6861 6e67 653d  chipq, CSchange=
+00004190: 5472 7565 2c20 6e6f 5265 6e6f 726d 3d46  True, noRenorm=F
+000041a0: 616c 7365 293a 0a20 2020 2043 7071 2c20  alse):.    Cpq, 
+000041b0: 5370 7120 3d20 2820 6e70 2e7a 6572 6f73  Spq = ( np.zeros
+000041c0: 2828 706d 6178 2b31 2c70 6d61 782b 3129  ((pmax+1,pmax+1)
+000041d0: 2920 666f 7220 5f20 696e 2072 616e 6765  ) for _ in range
+000041e0: 2832 2920 290a 0a20 2020 2069 6620 6e6f  (2) )..    if no
+000041f0: 5265 6e6f 726d 3a0a 2020 2020 2020 2020  Renorm:.        
+00004200: 6e6f 726d 203d 2031 0a20 2020 2020 2020  norm = 1.       
+00004210: 206e 6f72 6d30 203d 2031 0a20 2020 2065   norm0 = 1.    e
+00004220: 6c73 653a 0a20 2020 2020 2020 206e 6f72  lse:.        nor
+00004230: 6d20 3d20 3120 2f20 7371 7274 3470 6920  m = 1 / sqrt4pi 
+00004240: 2f20 7371 7274 320a 2020 2020 2020 2020  / sqrt2.        
+00004250: 6e6f 726d 3020 3d20 6e6f 726d 202a 2073  norm0 = norm * s
+00004260: 7172 7432 0a0a 2020 2020 666f 7220 7120  qrt2..    for q 
+00004270: 696e 2072 616e 6765 2831 2c20 706d 6178  in range(1, pmax
+00004280: 2b31 293a 0a20 2020 2020 2020 2043 5320  +1):.        CS 
+00004290: 3d20 282d 3129 2a2a 2871 2a28 6e6f 7420  = (-1)**(q*(not 
+000042a0: 4353 6368 616e 6765 2929 0a20 2020 2020  CSchange)).     
+000042b0: 2020 2023 2063 6f73 286d 2a70 6869 2920     # cos(m*phi) 
+000042c0: 7061 7274 3a0a 2020 2020 2020 2020 4370  part:.        Cp
+000042d0: 715b 3a2c 715d 203d 206e 702e 7265 616c  q[:,q] = np.real
+000042e0: 2828 282d 3129 2a2a 7120 2a20 6368 6970  (((-1)**q * chip
+000042f0: 715b 302c 3a2c 715d 202b 2063 6869 7071  q[0,:,q] + chipq
+00004300: 5b31 2c3a 2c71 5d29 202a 206e 6f72 6d29  [1,:,q]) * norm)
+00004310: 202a 2043 530a 2020 2020 2020 2020 2320   * CS.        # 
+00004320: 7369 6e28 6d2a 7068 6929 2070 6172 743a  sin(m*phi) part:
+00004330: 0a20 2020 2020 2020 2053 7071 5b3a 2c71  .        Spq[:,q
+00004340: 5d20 3d20 6e70 2e72 6561 6c28 2828 2d31  ] = np.real(((-1
+00004350: 292a 2a71 202a 2063 6869 7071 5b30 2c3a  )**q * chipq[0,:
+00004360: 2c71 5d20 2d20 6368 6970 715b 312c 3a2c  ,q] - chipq[1,:,
+00004370: 715d 2920 2a20 316a 202a 206e 6f72 6d29  q]) * 1j * norm)
+00004380: 202a 2043 530a 0a20 2020 2043 7071 5b3a   * CS..    Cpq[:
+00004390: 2c30 5d20 3d20 6e70 2e72 6561 6c28 6368  ,0] = np.real(ch
+000043a0: 6970 715b 302c 3a2c 305d 202a 206e 6f72  ipq[0,:,0] * nor
+000043b0: 6d30 290a 0a20 2020 2072 6574 7572 6e20  m0)..    return 
+000043c0: 4370 712c 2053 7071 0a0a 2323 2323 2323  Cpq, Spq..######
+000043d0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000043e0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000043f0: 2323 2323 2323 230a 0a22 2222 0a67 6574  #######..""".get
+00004400: 5f61 7071 5f66 726f 6d5f 6368 6970 7128  _apq_from_chipq(
+00004410: 290a 2020 2020 436f 6e76 6572 7420 636f  ).    Convert co
+00004420: 6d70 6c65 7820 6f72 7468 6f6e 6f72 6d61  mplex orthonorma
+00004430: 6c20 6861 726d 6f6e 6963 2063 6f65 6666  l harmonic coeff
+00004440: 6963 6965 6e74 7320 7769 7468 2074 6865  icients with the
+00004450: 2043 6f6e 646f 6e2d 5368 6f72 746c 6579   Condon-Shortley
+00004460: 2070 6861 7365 2074 6f20 0a20 2020 2074   phase to .    t
+00004470: 6865 2066 6f72 6d61 7420 6578 7065 6374  he format expect
+00004480: 6564 2062 7920 6865 616c 7079 2072 6f75  ed by healpy rou
+00004490: 7469 6e65 732c 2069 2e65 2e20 6120 6c69  tines, i.e. a li
+000044a0: 6e65 6172 206c 6973 7420 7769 7468 2074  near list with t
+000044b0: 6865 206d 3c30 2076 616c 7565 730a 2020  he m<0 values.  
+000044c0: 2020 6578 636c 7564 6564 2e20 4861 6e64    excluded. Hand
+000044d0: 6c65 7320 616c 6c20 7661 6c75 6573 2061  les all values a
+000044e0: 7420 6f6e 6365 2e0a 2020 2020 5573 6167  t once..    Usag
+000044f0: 653a 2060 6170 7160 203d 2067 6574 5f61  e: `apq` = get_a
+00004500: 7071 5f66 726f 6d5f 6368 6970 7128 6070  pq_from_chipq(`p
+00004510: 7661 6c73 602c 2060 7176 616c 7360 2c20  vals`, `qvals`, 
+00004520: 6063 6869 7071 6029 0a20 2020 2052 6574  `chipq`).    Ret
+00004530: 7572 6e73 3a0a 2020 2020 2020 2020 6170  urns:.        ap
+00004540: 713a 2063 6f6d 706c 6578 2c20 7368 6170  q: complex, shap
+00004550: 6528 7076 616c 7329 2e20 4f72 7468 6f6e  e(pvals). Orthon
+00004560: 6f72 6d61 6c20 7370 6865 7269 6361 6c20  ormal spherical 
+00004570: 6861 726d 6f6e 6963 2063 6f65 6666 6963  harmonic coeffic
+00004580: 6965 6e74 7320 7769 7468 2074 6865 2043  ients with the C
+00004590: 2d53 2070 6861 7365 2066 6f72 206d 3e30  -S phase for m>0
+000045a0: 206f 6e6c 792e 200a 2020 2020 2020 2020   only. .        
+000045b0: 2020 2020 436f 6566 6669 6369 656e 7473      Coefficients
+000045c0: 2066 6f72 206d 3c30 2061 7265 2073 696d   for m<0 are sim
+000045d0: 706c 7920 6469 7363 6172 6465 643b 2074  ply discarded; t
+000045e0: 6865 2076 616c 7565 7320 6172 6520 696e  he values are in
+000045f0: 6665 7272 6564 2066 726f 6d20 7768 6174  ferred from what
+00004600: 2074 6865 7920 6d75 7374 2062 6520 746f   they must be to
+00004610: 206d 6174 6368 2074 6865 0a20 2020 2020   match the.     
+00004620: 2020 2020 2020 206d 3e30 2076 616c 7565         m>0 value
+00004630: 7320 696e 206f 7264 6572 2074 6f20 7265  s in order to re
+00004640: 7475 726e 2061 2072 6561 6c2d 7661 6c75  turn a real-valu
+00004650: 6564 206d 6170 2066 726f 6d20 6865 616c  ed map from heal
+00004660: 7079 2e61 6c6d 326d 6170 2e0a 2020 2020  py.alm2map..    
+00004670: 5061 7261 6d65 7465 7273 3a0a 2020 2020  Parameters:.    
+00004680: 2020 2020 7076 616c 732c 2071 7661 6c73      pvals, qvals
+00004690: 3a20 696e 7465 6765 722c 2073 6861 7065  : integer, shape
+000046a0: 284e 7071 292e 204c 6973 7420 6f66 2070  (Npq). List of p
+000046b0: 6169 7265 6420 7020 616e 6420 7120 696e  aired p and q in
+000046c0: 6469 6365 7320 666f 7220 6170 712c 2061  dices for apq, a
+000046d0: 7320 7265 7475 726e 6564 2066 726f 6d20  s returned from 
+000046e0: 6865 616c 7079 2e73 7068 7466 756e 632e  healpy.sphtfunc.
+000046f0: 416c 6d2e 6765 746c 6d28 706d 6178 292e  Alm.getlm(pmax).
+00004700: 0a20 2020 2020 2020 2063 6869 7071 3a20  .        chipq: 
+00004710: 636f 6d70 6c65 782c 2073 6861 7065 2832  complex, shape(2
+00004720: 2c70 6d61 782b 312c 706d 6178 2b31 292e  ,pmax+1,pmax+1).
+00004730: 2063 6869 5f70 7120 7661 6c75 6573 2066   chi_pq values f
+00004740: 6f72 2061 6c6c 2071 203d 205b 2d70 2c70  or all q = [-p,p
+00004750: 5d20 666f 7220 7020 7570 2074 6f20 706d  ] for p up to pm
+00004760: 6178 2c0a 2020 2020 2020 2020 2020 2020  ax,.            
+00004770: 6f72 6761 6e69 7a65 6420 7375 6368 2074  organized such t
+00004780: 6861 7420 6368 6970 715b 696e 7428 713c  hat chipq[int(q<
+00004790: 3029 2c70 2c61 6273 2871 295d 2072 6574  0),p,abs(q)] ret
+000047a0: 7572 6e73 2074 6865 2072 6573 756c 7420  urns the result 
+000047b0: 666f 7220 6120 7061 7274 6963 756c 6172  for a particular
+000047c0: 2070 2c71 2070 6169 722e 0a20 2020 2020   p,q pair..     
+000047d0: 2020 2020 2020 204f 7274 686f 6e6f 726d         Orthonorm
+000047e0: 616c 2c20 7769 7468 2043 6f6e 646f 6e2d  al, with Condon-
+000047f0: 5368 6f72 746c 6579 2070 6861 7365 2e20  Shortley phase. 
+00004800: 4f72 7468 6f6e 6f72 6d61 6c20 6865 7265  Orthonormal here
+00004810: 206d 6561 6e73 2074 6865 2069 6e74 6567   means the integ
+00004820: 7261 6c20 6f66 0a20 2020 2020 2020 2020  ral of.         
+00004830: 2020 207c 596e 6d7c 5e32 202a 2064 4f6d     |Ynm|^2 * dOm
+00004840: 6567 6120 6f76 6572 2061 2075 6e69 7420  ega over a unit 
+00004850: 7370 6865 7265 2069 7320 3120 666f 7220  sphere is 1 for 
+00004860: 616c 6c20 6e20 616e 6420 6d2e 0a20 2020  all n and m..   
+00004870: 2022 2222 0a64 6566 2067 6574 5f61 7071   """.def get_apq
+00004880: 5f66 726f 6d5f 6368 6970 7128 7076 616c  _from_chipq(pval
+00004890: 732c 2071 7661 6c73 2c20 6368 6970 7129  s, qvals, chipq)
+000048a0: 3a0a 2020 2020 2320 4172 7261 6e67 6520  :.    # Arrange 
+000048b0: 696e 746f 2061 206c 696e 6561 7220 6c69  into a linear li
+000048c0: 7374 2063 6f6d 7061 7469 626c 6520 7769  st compatible wi
+000048d0: 7468 2068 6561 6c70 7920 6576 616c 7561  th healpy evalua
+000048e0: 7469 6f6e 2072 6f75 7469 6e65 730a 2020  tion routines.  
+000048f0: 2020 6170 7120 3d20 6e70 2e61 7272 6179    apq = np.array
+00004900: 285b 6368 6970 715b 302c 702c 715d 2066  ([chipq[0,p,q] f
+00004910: 6f72 2070 2c71 2069 6e20 7a69 7028 7076  or p,q in zip(pv
+00004920: 616c 732c 2071 7661 6c73 295d 290a 0a20  als, qvals)]).. 
+00004930: 2020 2072 6574 7572 6e20 6170 710a 0a23     return apq..#
+00004940: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00004950: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00004960: 2323 2323 2323 2323 2323 2323 0a0a 2222  ############..""
+00004970: 220a 6765 745f 6368 6970 715f 6672 6f6d  ".get_chipq_from
+00004980: 5f61 7071 2829 0a20 2020 2043 6f6e 7665  _apq().    Conve
+00004990: 7274 2063 6f6d 706c 6578 206f 7274 686f  rt complex ortho
+000049a0: 6e6f 726d 616c 2068 6172 6d6f 6e69 6320  normal harmonic 
+000049b0: 636f 6566 6669 6369 656e 7473 2077 6974  coefficients wit
+000049c0: 6820 7468 6520 436f 6e64 6f6e 2d53 686f  h the Condon-Sho
+000049d0: 7274 6c65 7920 7068 6173 6520 6672 6f6d  rtley phase from
+000049e0: 200a 2020 2020 7468 6520 666f 726d 6174   .    the format
+000049f0: 2065 7870 6563 7465 6420 6279 2068 6561   expected by hea
+00004a00: 6c70 7920 726f 7574 696e 6573 2c20 692e  lpy routines, i.
+00004a10: 652e 2061 206c 696e 6561 7220 6c69 7374  e. a linear list
+00004a20: 2077 6974 6820 7468 6520 6d3c 3020 7661   with the m<0 va
+00004a30: 6c75 6573 0a20 2020 2065 7863 6c75 6465  lues.    exclude
+00004a40: 642c 2074 6f20 7468 6520 6675 6c6c 2073  d, to the full s
+00004a50: 6574 2066 6f72 2061 6c6c 2076 616c 7565  et for all value
+00004a60: 7320 6f66 202d 7020 3c3d 206d 203c 3d20  s of -p <= m <= 
+00004a70: 702e 2048 616e 646c 6573 2061 6c6c 2076  p. Handles all v
+00004a80: 616c 7565 7320 6174 206f 6e63 652e 0a20  alues at once.. 
+00004a90: 2020 2055 7361 6765 3a20 6063 6869 7071     Usage: `chipq
+00004aa0: 6020 3d20 6765 745f 6368 6970 715f 6672  ` = get_chipq_fr
+00004ab0: 6f6d 5f61 7071 2860 7076 616c 7360 2c20  om_apq(`pvals`, 
+00004ac0: 6071 7661 6c73 602c 2060 6170 7160 290a  `qvals`, `apq`).
+00004ad0: 2020 2020 5265 7475 726e 733a 0a20 2020      Returns:.   
+00004ae0: 2020 2020 2063 6869 7071 3a20 636f 6d70       chipq: comp
+00004af0: 6c65 782c 2073 6861 7065 2832 2c70 6d61  lex, shape(2,pma
+00004b00: 782b 312c 706d 6178 2b31 292e 2063 6869  x+1,pmax+1). chi
+00004b10: 5f70 7120 7661 6c75 6573 2066 6f72 2061  _pq values for a
+00004b20: 6c6c 2071 203d 205b 2d70 2c70 5d20 666f  ll q = [-p,p] fo
+00004b30: 7220 7020 7570 2074 6f20 706d 6178 2c0a  r p up to pmax,.
+00004b40: 2020 2020 2020 2020 2020 2020 6f72 6761              orga
+00004b50: 6e69 7a65 6420 7375 6368 2074 6861 7420  nized such that 
+00004b60: 6368 6970 715b 696e 7428 713c 3029 2c70  chipq[int(q<0),p
+00004b70: 2c61 6273 2871 295d 2072 6574 7572 6e73  ,abs(q)] returns
+00004b80: 2074 6865 2072 6573 756c 7420 666f 7220   the result for 
+00004b90: 6120 7061 7274 6963 756c 6172 2070 2c71  a particular p,q
+00004ba0: 2070 6169 722e 0a20 2020 2020 2020 2020   pair..         
+00004bb0: 2020 204f 7274 686f 6e6f 726d 616c 2c20     Orthonormal, 
+00004bc0: 7769 7468 2043 6f6e 646f 6e2d 5368 6f72  with Condon-Shor
+00004bd0: 746c 6579 2070 6861 7365 2e20 4f72 7468  tley phase. Orth
+00004be0: 6f6e 6f72 6d61 6c20 6865 7265 206d 6561  onormal here mea
+00004bf0: 6e73 2074 6865 2069 6e74 6567 7261 6c20  ns the integral 
+00004c00: 6f66 0a20 2020 2020 2020 2020 2020 207c  of.            |
+00004c10: 596e 6d7c 5e32 202a 2064 4f6d 6567 6120  Ynm|^2 * dOmega 
+00004c20: 6f76 6572 2061 2075 6e69 7420 7370 6865  over a unit sphe
+00004c30: 7265 2069 7320 3120 666f 7220 616c 6c20  re is 1 for all 
+00004c40: 6e20 616e 6420 6d2e 0a20 2020 2050 6172  n and m..    Par
+00004c50: 616d 6574 6572 733a 0a20 2020 2020 2020  ameters:.       
+00004c60: 2070 7661 6c73 2c20 7176 616c 733a 2069   pvals, qvals: i
+00004c70: 6e74 6567 6572 2c20 7368 6170 6528 4e70  nteger, shape(Np
+00004c80: 7129 2e20 4c69 7374 206f 6620 7061 6972  q). List of pair
+00004c90: 6564 2070 2061 6e64 2071 2069 6e64 6963  ed p and q indic
+00004ca0: 6573 2066 6f72 2061 7071 2c20 6173 2072  es for apq, as r
+00004cb0: 6574 7572 6e65 6420 6672 6f6d 2068 6561  eturned from hea
+00004cc0: 6c70 792e 7370 6874 6675 6e63 2e41 6c6d  lpy.sphtfunc.Alm
+00004cd0: 2e67 6574 6c6d 2870 6d61 7829 2e0a 2020  .getlm(pmax)..  
+00004ce0: 2020 2020 2020 6170 713a 2063 6f6d 706c        apq: compl
+00004cf0: 6578 2c20 7368 6170 6528 7076 616c 7329  ex, shape(pvals)
+00004d00: 2e20 4f72 7468 6f6e 6f72 6d61 6c20 7370  . Orthonormal sp
+00004d10: 6865 7269 6361 6c20 6861 726d 6f6e 6963  herical harmonic
+00004d20: 2063 6f65 6666 6963 6965 6e74 7320 7769   coefficients wi
+00004d30: 7468 2074 6865 2043 2d53 2070 6861 7365  th the C-S phase
+00004d40: 2066 6f72 206d 3e30 206f 6e6c 792e 200a   for m>0 only. .
+00004d50: 2020 2020 2020 2020 2020 2020 436f 6566              Coef
+00004d60: 6669 6369 656e 7473 2066 6f72 206d 3c30  ficients for m<0
+00004d70: 2061 7265 2073 696d 706c 7920 6469 7363   are simply disc
+00004d80: 6172 6465 643b 2074 6865 2076 616c 7565  arded; the value
+00004d90: 7320 6172 6520 696e 6665 7272 6564 2066  s are inferred f
+00004da0: 726f 6d20 7768 6174 2074 6865 7920 6d75  rom what they mu
+00004db0: 7374 2062 6520 746f 206d 6174 6368 2074  st be to match t
+00004dc0: 6865 0a20 2020 2020 2020 2020 2020 206d  he.            m
+00004dd0: 3e30 2076 616c 7565 7320 696e 206f 7264  >0 values in ord
+00004de0: 6572 2074 6f20 7265 7475 726e 2061 2072  er to return a r
+00004df0: 6561 6c2d 7661 6c75 6564 206d 6170 2066  eal-valued map f
+00004e00: 726f 6d20 6865 616c 7079 2e61 6c6d 326d  rom healpy.alm2m
+00004e10: 6170 2e0a 2020 2020 2222 220a 6465 6620  ap..    """.def 
+00004e20: 6765 745f 6368 6970 715f 6672 6f6d 5f61  get_chipq_from_a
+00004e30: 7071 2870 7661 6c73 2c20 7176 616c 732c  pq(pvals, qvals,
+00004e40: 2061 7071 293a 0a20 2020 2023 2052 6563   apq):.    # Rec
+00004e50: 6f6e 7374 7275 6374 2061 6c6c 2063 6f6d  onstruct all com
+00004e60: 706c 6578 2063 6f65 6666 6963 6965 6e74  plex coefficient
+00004e70: 7320 6173 206e 6565 6465 6420 746f 2072  s as needed to r
+00004e80: 6573 756c 7420 696e 2072 6561 6c2d 7661  esult in real-va
+00004e90: 6c75 6564 206f 7574 7075 7473 0a20 2020  lued outputs.   
+00004ea0: 2070 6d61 7820 3d20 6e70 2e6d 6178 2870   pmax = np.max(p
+00004eb0: 7661 6c73 290a 2020 2020 6368 6970 7120  vals).    chipq 
+00004ec0: 3d20 6e70 2e7a 6572 6f73 2828 322c 706d  = np.zeros((2,pm
+00004ed0: 6178 2b31 2c70 6d61 782b 3129 2c20 6474  ax+1,pmax+1), dt
+00004ee0: 7970 653d 6e70 2e63 6f6d 706c 6578 5f29  ype=np.complex_)
+00004ef0: 0a20 2020 2066 6f72 2061 2c70 2c71 2069  .    for a,p,q i
+00004f00: 6e20 7a69 7028 6170 712c 2070 7661 6c73  n zip(apq, pvals
+00004f10: 2c20 7176 616c 7329 3a0a 2020 2020 2020  , qvals):.      
+00004f20: 2020 6368 6970 715b 302c 702c 715d 203d    chipq[0,p,q] =
+00004f30: 2061 0a20 2020 2020 2020 2063 6869 7071   a.        chipq
+00004f40: 5b31 2c70 2c71 5d20 3d20 6e70 2e63 6f6e  [1,p,q] = np.con
+00004f50: 6a28 6129 202a 2028 2d31 292a 2a71 0a0a  j(a) * (-1)**q..
+00004f60: 2020 2020 7265 7475 726e 2063 6869 7071      return chipq
+00004f70: 0a0a 2323 2323 2323 2323 2323 2323 2323  ..##############
+00004f80: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00004f90: 2323 2323 2323 2323 2323 2323 2323 230a  ###############.
+00004fa0: 0a22 2222 0a67 6574 5f67 685f 6672 6f6d  .""".get_gh_from
+00004fb0: 5f42 696e 6d28 290a 2020 2020 436f 6e76  _Binm().    Conv
+00004fc0: 6572 7420 6672 6f6d 206f 7274 686f 6e6f  ert from orthono
+00004fd0: 726d 616c 2068 6172 6d6f 6e69 6320 636f  rmal harmonic co
+00004fe0: 6566 6669 6369 656e 7473 2077 6974 6820  efficients with 
+00004ff0: 7468 6520 436f 6e64 6f6e 2d53 686f 7274  the Condon-Short
+00005000: 6c65 7920 7068 6173 6520 2863 6f6d 6d6f  ley phase (commo
+00005010: 6e20 696e 2070 6879 7369 6373 290a 2020  n in physics).  
+00005020: 2020 746f 2053 6368 6d69 6474 2073 656d    to Schmidt sem
+00005030: 692d 6e6f 726d 616c 697a 6564 2066 6f72  i-normalized for
+00005040: 6d20 7769 7468 6f75 7420 7468 6520 432d  m without the C-
+00005050: 5320 7068 6173 6520 2863 6f6d 6d6f 6e20  S phase (common 
+00005060: 696e 2067 656f 7068 7973 6963 7329 2e0a  in geophysics)..
+00005070: 2020 2020 4861 6e64 6c65 7320 616c 6c20      Handles all 
+00005080: 7661 6c75 6573 2066 6f72 2061 2067 6976  values for a giv
+00005090: 656e 206e 2061 7420 6f6e 6365 2e0a 2020  en n at once..  
+000050a0: 2020 5573 6167 653a 2060 676e 6d60 2c20    Usage: `gnm`, 
+000050b0: 6068 6e6d 6020 3d20 6765 745f 6768 5f66  `hnm` = get_gh_f
+000050c0: 726f 6d5f 4269 6e6d 2860 6e60 2c20 606e  rom_Binm(`n`, `n
+000050d0: 5f6d 6178 602c 2060 4269 6e6d 6029 0a20  _max`, `Binm`). 
+000050e0: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
+000050f0: 2020 2020 676e 6d2c 2068 6e6d 3a20 636f      gnm, hnm: co
+00005100: 6d70 6c65 782c 2073 6861 7065 286e 5f6d  mplex, shape(n_m
+00005110: 6178 2b31 2c6e 5f6d 6178 2b31 292e 2067  ax+1,n_max+1). g
+00005120: 5f6e 6d20 616e 6420 685f 6e6d 2076 616c  _nm and h_nm val
+00005130: 7565 7320 666f 7220 616c 6c20 6d20 3d20  ues for all m = 
+00005140: 5b30 2c6e 5d2e 0a0a 2020 2020 2020 2020  [0,n]...        
+00005150: 2020 2020 5363 686d 6964 7420 6e6f 726d      Schmidt norm
+00005160: 616c 697a 6174 696f 6e20 6865 7265 206d  alization here m
+00005170: 6561 6e73 2074 6865 2069 6e74 6567 7261  eans the integra
+00005180: 6c20 6f66 207c 596e 6d7c 5e32 202a 2064  l of |Ynm|^2 * d
+00005190: 4f6d 6567 6120 6f76 6572 2061 2075 6e69  Omega over a uni
+000051a0: 7420 7370 6865 7265 2069 730a 2020 2020  t sphere is.    
+000051b0: 2020 2020 2020 2020 3470 692f 2832 6e2b          4pi/(2n+
+000051c0: 3129 2066 6f72 2061 6c6c 206e 2061 6e64  1) for all n and
+000051d0: 206d 2e20 4e6f 2043 6f6e 646f 6e2d 5368   m. No Condon-Sh
+000051e0: 6f72 746c 6579 2070 6861 7365 2e0a 2020  ortley phase..  
+000051f0: 2020 5061 7261 6d65 7465 7273 3a0a 2020    Parameters:.  
+00005200: 2020 2020 2020 6e5f 6d61 783a 2069 6e74        n_max: int
+00005210: 6567 6572 2e20 4d61 7869 6d75 6d20 6465  eger. Maximum de
+00005220: 6772 6565 206e 206f 6620 696e 6475 6365  gree n of induce
+00005230: 6420 6d6f 6d65 6e74 732e 0a20 2020 2020  d moments..     
+00005240: 2020 2042 696e 6d3a 2063 6f6d 706c 6578     Binm: complex
+00005250: 2c20 7368 6170 6528 322c 6e5f 6d61 782b  , shape(2,n_max+
+00005260: 312c 6e5f 6d61 782b 3129 2e20 436f 6d70  1,n_max+1). Comp
+00005270: 6c65 7820 696e 6475 6365 6420 6d61 676e  lex induced magn
+00005280: 6574 6963 206d 6f6d 656e 7473 2063 616c  etic moments cal
+00005290: 6375 6c61 7465 6420 7573 696e 6720 6675  culated using fu
+000052a0: 6c6c 7920 6e6f 726d 616c 697a 6564 2073  lly normalized s
+000052b0: 7068 6572 6963 616c 2068 6172 6d6f 6e69  pherical harmoni
+000052c0: 6320 636f 6566 6669 6369 656e 7473 2e0a  c coefficients..
+000052d0: 2020 2020 2222 220a 6465 6620 6765 745f      """.def get_
+000052e0: 6768 5f66 726f 6d5f 4269 6e6d 286e 5f6d  gh_from_Binm(n_m
+000052f0: 6178 2c20 4269 6e6d 293a 0a20 2020 2067  ax, Binm):.    g
+00005300: 6e6d 2c20 686e 6d20 3d20 2820 6e70 2e7a  nm, hnm = ( np.z
+00005310: 6572 6f73 2828 6e5f 6d61 782b 312c 6e5f  eros((n_max+1,n_
+00005320: 6d61 782b 3129 2c20 6474 7970 653d 6e70  max+1), dtype=np
+00005330: 2e63 6f6d 706c 6578 5f29 2066 6f72 205f  .complex_) for _
+00005340: 2069 6e20 7261 6e67 6528 3229 2029 0a0a   in range(2) )..
+00005350: 2020 2020 666f 7220 6e20 696e 2072 616e      for n in ran
+00005360: 6765 2831 2c6e 5f6d 6178 2b31 293a 0a20  ge(1,n_max+1):. 
+00005370: 2020 2020 2020 206e 6f72 6d20 3d20 6e70         norm = np
+00005380: 2e73 7172 7428 322a 6e2b 3129 202f 2073  .sqrt(2*n+1) / s
+00005390: 7172 7432 202f 2073 7172 7434 7069 0a0a  qrt2 / sqrt4pi..
+000053a0: 2020 2020 2020 2020 666f 7220 6d20 696e          for m in
+000053b0: 2072 616e 6765 2831 2c20 6e2b 3129 3a0a   range(1, n+1):.
+000053c0: 2020 2020 2020 2020 2020 2020 2320 6720              # g 
+000053d0: 7465 726d 733a 0a20 2020 2020 2020 2020  terms:.         
+000053e0: 2020 2067 6e6d 5b6e 2c6d 5d20 3d20 2828     gnm[n,m] = ((
+000053f0: 2d31 292a 2a6d 202a 2042 696e 6d5b 302c  -1)**m * Binm[0,
+00005400: 6e2c 6d5d 202b 2042 696e 6d5b 312c 6e2c  n,m] + Binm[1,n,
+00005410: 6d5d 2920 2a20 6e6f 726d 0a20 2020 2020  m]) * norm.     
+00005420: 2020 2020 2020 2023 2068 2074 6572 6d73         # h terms
+00005430: 3a0a 2020 2020 2020 2020 2020 2020 686e  :.            hn
+00005440: 6d5b 6e2c 6d5d 203d 2028 282d 3129 2a2a  m[n,m] = ((-1)**
+00005450: 6d20 2a20 4269 6e6d 5b30 2c6e 2c6d 5d20  m * Binm[0,n,m] 
+00005460: 2d20 4269 6e6d 5b31 2c6e 2c6d 5d29 202a  - Binm[1,n,m]) *
+00005470: 2031 6a20 2a20 6e6f 726d 0a0a 2020 2020   1j * norm..    
+00005480: 2020 2020 676e 6d5b 6e2c 305d 203d 2042      gnm[n,0] = B
+00005490: 696e 6d5b 302c 6e2c 305d 202a 206e 6f72  inm[0,n,0] * nor
+000054a0: 6d20 2a20 7371 7274 320a 0a20 2020 2072  m * sqrt2..    r
+000054b0: 6574 7572 6e20 676e 6d2c 2068 6e6d 0a0a  eturn gnm, hnm..
+000054c0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000054d0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000054e0: 2323 2323 2323 2323 2323 2323 230a 0a64  #############..d
+000054f0: 6566 2067 6574 5f42 696e 6d5f 6672 6f6d  ef get_Binm_from
+00005500: 5f67 6828 6e5f 6d61 782c 2067 6e6d 2c20  _gh(n_max, gnm, 
+00005510: 686e 6d29 3a0a 2020 2020 2222 220a 2020  hnm):.    """.  
+00005520: 2020 436f 6e76 6572 7420 6672 6f6d 2053    Convert from S
+00005530: 6368 6d69 6474 2073 656d 692d 6e6f 726d  chmidt semi-norm
+00005540: 616c 697a 6564 2066 6f72 6d20 7769 7468  alized form with
+00005550: 6f75 7420 7468 6520 432d 5320 7068 6173  out the C-S phas
+00005560: 6520 2863 6f6d 6d6f 6e20 696e 2067 656f  e (common in geo
+00005570: 7068 7973 6963 7329 0a20 2020 2074 6f20  physics).    to 
+00005580: 6f72 7468 6f6e 6f72 6d61 6c20 6861 726d  orthonormal harm
+00005590: 6f6e 6963 2063 6f65 6666 6963 6965 6e74  onic coefficient
+000055a0: 7320 7769 7468 2074 6865 2043 6f6e 646f  s with the Condo
+000055b0: 6e2d 5368 6f72 746c 6579 2070 6861 7365  n-Shortley phase
+000055c0: 2028 636f 6d6d 6f6e 2069 6e20 7068 7973   (common in phys
+000055d0: 6963 7329 2e0a 2020 2020 4861 6e64 6c65  ics)..    Handle
+000055e0: 7320 616c 6c20 7661 6c75 6573 2066 6f72  s all values for
+000055f0: 2061 2067 6976 656e 206e 2061 7420 6f6e   a given n at on
+00005600: 6365 2e0a 2020 2020 4172 6773 3a0a 2020  ce..    Args:.  
+00005610: 2020 2020 2020 6e5f 6d61 783a 2069 6e74        n_max: int
+00005620: 2e20 4d61 7869 6d75 6d20 6465 6772 6565  . Maximum degree
+00005630: 206e 206f 6620 696e 6475 6365 6420 6d6f   n of induced mo
+00005640: 6d65 6e74 732e 0a20 2020 2020 2020 2067  ments..        g
+00005650: 6e6d 2c20 686e 6d3a 2063 6f6d 706c 6578  nm, hnm: complex
+00005660: 2c20 7368 6170 6528 6e5f 6d61 782b 312c  , shape(n_max+1,
+00005670: 6e5f 6d61 782b 3129 2e20 675f 6e6d 2061  n_max+1). g_nm a
+00005680: 6e64 2068 5f6e 6d20 7661 6c75 6573 2066  nd h_nm values f
+00005690: 6f72 2061 6c6c 206d 203d 205b 302c 6e5d  or all m = [0,n]
+000056a0: 2e0a 2020 2020 2020 2020 2020 2020 5363  ..            Sc
+000056b0: 686d 6964 7420 6e6f 726d 616c 697a 6174  hmidt normalizat
+000056c0: 696f 6e20 6865 7265 206d 6561 6e73 2074  ion here means t
+000056d0: 6865 2069 6e74 6567 7261 6c20 6f66 207c  he integral of |
+000056e0: 596e 6d7c 5e32 202a 2064 4f6d 6567 6120  Ynm|^2 * dOmega 
+000056f0: 6f76 6572 2061 2075 6e69 7420 7370 6865  over a unit sphe
+00005700: 7265 2069 730a 2020 2020 2020 2020 2020  re is.          
+00005710: 2020 3470 692f 2832 6e2b 3129 2066 6f72    4pi/(2n+1) for
+00005720: 2061 6c6c 206e 2061 6e64 206d 2e20 4e6f   all n and m. No
+00005730: 2043 6f6e 646f 6e2d 5368 6f72 746c 6579   Condon-Shortley
+00005740: 2070 6861 7365 2e0a 0a20 2020 2052 6574   phase...    Ret
+00005750: 7572 6e73 3a0a 2020 2020 2020 2020 4269  urns:.        Bi
+00005760: 6e6d 3a20 636f 6d70 6c65 782c 2073 6861  nm: complex, sha
+00005770: 7065 2832 2c6e 5f6d 6178 2b31 2c6e 5f6d  pe(2,n_max+1,n_m
+00005780: 6178 2b31 292e 2043 6f6d 706c 6578 2069  ax+1). Complex i
+00005790: 6e64 7563 6564 206d 6167 6e65 7469 6320  nduced magnetic 
+000057a0: 6d6f 6d65 6e74 7320 666f 7220 6675 6c6c  moments for full
+000057b0: 7920 6e6f 726d 616c 697a 6564 2073 7068  y normalized sph
+000057c0: 6572 6963 616c 2068 6172 6d6f 6e69 6373  erical harmonics
+000057d0: 2e0a 2020 2020 2222 220a 2020 2020 4269  ..    """.    Bi
+000057e0: 6e6d 203d 206e 702e 7a65 726f 7328 2832  nm = np.zeros((2
+000057f0: 2c6e 5f6d 6178 2b31 2c6e 5f6d 6178 2b31  ,n_max+1,n_max+1
+00005800: 292c 2064 7479 7065 3d6e 702e 636f 6d70  ), dtype=np.comp
+00005810: 6c65 785f 290a 0a20 2020 2066 6f72 206e  lex_)..    for n
+00005820: 2069 6e20 7261 6e67 6528 312c 206e 5f6d   in range(1, n_m
+00005830: 6178 2b31 293a 0a20 2020 2020 2020 206e  ax+1):.        n
+00005840: 6f72 6d20 3d20 7371 7274 3470 6920 2f20  orm = sqrt4pi / 
+00005850: 6e70 2e73 7172 7428 322a 6e2b 3129 202f  np.sqrt(2*n+1) /
+00005860: 2073 7172 7432 0a0a 2020 2020 2020 2020   sqrt2..        
+00005870: 666f 7220 6d20 696e 2072 616e 6765 2831  for m in range(1
+00005880: 2c20 6e2b 3129 3a0a 2020 2020 2020 2020  , n+1):.        
+00005890: 2020 2020 2320 6d3e 3020 7465 726d 733a      # m>0 terms:
+000058a0: 0a20 2020 2020 2020 2020 2020 2042 696e  .            Bin
+000058b0: 6d5b 302c 6e2c 6d5d 203d 2028 2d31 292a  m[0,n,m] = (-1)*
+000058c0: 2a6d 202a 206e 6f72 6d20 2a20 2867 6e6d  *m * norm * (gnm
+000058d0: 5b6e 2c6d 5d20 2d20 316a 202a 2068 6e6d  [n,m] - 1j * hnm
+000058e0: 5b6e 2c6d 5d29 0a20 2020 2020 2020 2020  [n,m]).         
+000058f0: 2020 2023 206d 3c30 2074 6572 6d73 3a0a     # m<0 terms:.
+00005900: 2020 2020 2020 2020 2020 2020 4269 6e6d              Binm
+00005910: 5b31 2c6e 2c6d 5d20 3d20 2020 2020 2020  [1,n,m] =       
+00005920: 2020 2020 6e6f 726d 202a 2028 676e 6d5b      norm * (gnm[
+00005930: 6e2c 6d5d 202b 2031 6a20 2a20 686e 6d5b  n,m] + 1j * hnm[
+00005940: 6e2c 6d5d 290a 0a20 2020 2020 2020 2042  n,m])..        B
+00005950: 696e 6d5b 302c 6e2c 305d 203d 206e 6f72  inm[0,n,0] = nor
+00005960: 6d20 2a20 7371 7274 3220 2a20 676e 6d5b  m * sqrt2 * gnm[
+00005970: 6e2c 305d 0a0a 2020 2020 7265 7475 726e  n,0]..    return
+00005980: 2042 696e 6d0a 0a23 2323 2323 2323 2323   Binm..#########
+00005990: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000059a0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000059b0: 2323 2323 0a0a 2222 220a 7661 6c69 6461  ####..""".valida
+000059c0: 7465 2829 0a20 2020 2043 6865 636b 2069  te().    Check i
+000059d0: 6e70 7574 7320 746f 2062 6520 7375 7265  nputs to be sure
+000059e0: 2065 7665 7279 7468 696e 6720 7769 6c6c   everything will
+000059f0: 2062 6520 696e 7465 7270 7265 7465 6420   be interpreted 
+00005a00: 636f 7272 6563 746c 792e 0a20 2020 2055  correctly..    U
+00005a10: 7361 6765 3a20 6072 5f62 6473 602c 2060  sage: `r_bds`, `
+00005a20: 7369 676d 6173 602c 2060 6f6d 6567 6173  sigmas`, `omegas
+00005a30: 602c 2060 6173 796d 5f73 6861 7065 6020  `, `asym_shape` 
+00005a40: 3d20 7661 6c69 6461 7465 2860 725f 6264  = validate(`r_bd
+00005a50: 7360 2c20 6073 6967 6d61 7360 2c20 606f  s`, `sigmas`, `o
+00005a60: 6d65 6761 7360 2c20 6062 6364 6576 602c  megas`, `bcdev`,
+00005a70: 2060 6173 796d 5f73 6861 7065 602c 2060   `asym_shape`, `
+00005a80: 705f 6d61 7860 290a 2020 2020 5265 7475  p_max`).    Retu
+00005a90: 726e 733a 0a20 2020 2020 2020 2072 5f62  rns:.        r_b
+00005aa0: 6473 3a20 666c 6f61 742c 2073 6861 7065  ds: float, shape
+00005ab0: 286e 5f62 6473 292e 0a20 2020 2020 2020  (n_bds)..       
+00005ac0: 2073 6967 6d61 733a 2066 6c6f 6174 2c20   sigmas: float, 
+00005ad0: 7368 6170 6528 6e5f 6264 7329 2e0a 2020  shape(n_bds)..  
+00005ae0: 2020 2020 2020 6f6d 6567 6173 3a20 666c        omegas: fl
+00005af0: 6f61 742c 2073 6861 7065 286e 5f70 6561  oat, shape(n_pea
+00005b00: 6b73 292e 0a20 2020 2020 2020 2061 7379  ks)..        asy
+00005b10: 6d5f 7368 6170 653a 2063 6f6d 706c 6578  m_shape: complex
+00005b20: 2c20 7368 6170 6528 6e5f 6264 732c 322c  , shape(n_bds,2,
+00005b30: 705f 6d61 782b 312c 705f 6d61 782b 3129  p_max+1,p_max+1)
+00005b40: 2e0a 2020 2020 5061 7261 6d65 7465 7273  ..    Parameters
+00005b50: 3a0a 2020 2020 2020 2020 725f 6264 733a  :.        r_bds:
+00005b60: 2066 6c6f 6174 2c20 7368 6170 6528 6e5f   float, shape(n_
+00005b70: 6264 7329 2e0a 2020 2020 2020 2020 7369  bds)..        si
+00005b80: 676d 6173 3a20 666c 6f61 742c 2073 6861  gmas: float, sha
+00005b90: 7065 286e 5f62 6473 292e 0a20 2020 2020  pe(n_bds)..     
+00005ba0: 2020 206f 6d65 6761 733a 2066 6c6f 6174     omegas: float
+00005bb0: 2c20 7368 6170 6528 6e5f 7065 616b 7329  , shape(n_peaks)
+00005bc0: 2e0a 2020 2020 2020 2020 6263 6465 763a  ..        bcdev:
+00005bd0: 2066 6c6f 6174 2c20 7368 6170 6528 6e5f   float, shape(n_
+00005be0: 6264 7329 2e0a 2020 2020 2020 2020 6173  bds)..        as
+00005bf0: 796d 5f73 6861 7065 3a20 636f 6d70 6c65  ym_shape: comple
+00005c00: 782c 2073 6861 7065 286e 5f62 6473 2c32  x, shape(n_bds,2
+00005c10: 2c70 5f6d 6178 2b31 2c70 5f6d 6178 2b31  ,p_max+1,p_max+1
+00005c20: 292e 0a20 2020 2020 2020 2070 5f6d 6178  )..        p_max
+00005c30: 3a20 696e 7465 6765 722e 0a20 2020 2022  : integer..    "
+00005c40: 2222 0a64 6566 2076 616c 6964 6174 6528  "".def validate(
+00005c50: 725f 6264 732c 2073 6967 6d61 732c 2062  r_bds, sigmas, b
+00005c60: 6364 6576 2c20 6173 796d 5f73 6861 7065  cdev, asym_shape
+00005c70: 2c20 705f 6d61 7829 3a0a 2020 2020 2320  , p_max):.    # 
+00005c80: 4368 6563 6b20 6c65 6e67 7468 7320 6f66  Check lengths of
+00005c90: 206d 6f64 656c 206c 6973 7473 0a20 2020   model lists.   
+00005ca0: 2069 6620 6e70 2e73 6861 7065 2872 5f62   if np.shape(r_b
+00005cb0: 6473 2920 213d 206e 702e 7368 6170 6528  ds) != np.shape(
+00005cc0: 7369 676d 6173 293a 0a20 2020 2020 2020  sigmas):.       
+00005cd0: 206c 6f67 2e65 7272 6f72 2866 2262 6f75   log.error(f"bou
+00005ce0: 6e64 6172 6965 7320 7368 6170 653a 207b  ndaries shape: {
+00005cf0: 6e70 2e73 6861 7065 2872 5f62 6473 297d  np.shape(r_bds)}
+00005d00: 2229 0a20 2020 2020 2020 206c 6f67 2e65  ").        log.e
+00005d10: 7272 6f72 2866 2273 6967 6d61 7320 7368  rror(f"sigmas sh
+00005d20: 6170 653a 207b 6e70 2e73 6861 7065 2873  ape: {np.shape(s
+00005d30: 6967 6d61 7329 7d22 290a 2020 2020 2020  igmas)}").      
+00005d40: 2020 7261 6973 6520 5661 6c75 6545 7272    raise ValueErr
+00005d50: 6f72 2822 5468 6520 6e75 6d62 6572 206f  or("The number o
+00005d60: 6620 626f 756e 6461 7269 6573 2069 7320  f boundaries is 
+00005d70: 6e6f 7420 6571 7561 6c20 746f 2074 6865  not equal to the
+00005d80: 206e 756d 6265 7220 6f66 2063 6f6e 6475   number of condu
+00005d90: 6374 6976 6974 6965 732e 2229 0a20 2020  ctivities.").   
+00005da0: 2069 6620 6e70 2e73 6861 7065 2872 5f62   if np.shape(r_b
+00005db0: 6473 2920 213d 206e 702e 7368 6170 6528  ds) != np.shape(
+00005dc0: 6263 6465 7629 3a0a 2020 2020 2020 2020  bcdev):.        
+00005dd0: 6c6f 672e 6572 726f 7228 6622 626f 756e  log.error(f"boun
+00005de0: 6461 7269 6573 2073 6861 7065 3a20 7b6e  daries shape: {n
+00005df0: 702e 7368 6170 6528 725f 6264 7329 7d22  p.shape(r_bds)}"
+00005e00: 290a 2020 2020 2020 2020 6c6f 672e 6572  ).        log.er
+00005e10: 726f 7228 6622 6465 7669 6174 696f 6e73  ror(f"deviations
+00005e20: 2073 6861 7065 3a20 7b6e 702e 7368 6170   shape: {np.shap
+00005e30: 6528 6263 6465 7629 7d22 290a 2020 2020  e(bcdev)}").    
+00005e40: 2020 2020 7261 6973 6520 5661 6c75 6545      raise ValueE
+00005e50: 7272 6f72 2822 5468 6520 6e75 6d62 6572  rror("The number
+00005e60: 206f 6620 626f 756e 6461 7269 6573 2069   of boundaries i
+00005e70: 7320 6e6f 7420 6571 7561 6c20 746f 2074  s not equal to t
+00005e80: 6865 206e 756d 6265 7220 6f66 2064 6576  he number of dev
+00005e90: 6961 7469 6f6e 732e 2229 0a0a 2020 2020  iations.")..    
+00005ea0: 2320 4d61 6b65 2073 7572 6520 696e 7465  # Make sure inte
+00005eb0: 7269 6f72 206d 6f64 656c 2069 7320 6974  rior model is it
+00005ec0: 6572 6162 6c65 2028 6974 2773 206e 6f74  erable (it's not
+00005ed0: 2069 6620 7468 6572 6520 6973 206f 6e6c   if there is onl
+00005ee0: 7920 3120 626f 756e 6461 7279 290a 2020  y 1 boundary).  
+00005ef0: 2020 6966 206e 6f74 2069 7369 6e73 7461    if not isinsta
+00005f00: 6e63 6528 725f 6264 732c 2049 7465 7261  nce(r_bds, Itera
+00005f10: 626c 6529 3a0a 2020 2020 2020 2020 725f  ble):.        r_
+00005f20: 6264 7320 3d20 5b72 5f62 6473 5d0a 2020  bds = [r_bds].  
+00005f30: 2020 2020 2020 7369 676d 6173 203d 205b        sigmas = [
+00005f40: 7369 676d 6173 5d0a 2020 2020 2020 2020  sigmas].        
+00005f50: 6e70 2e72 6573 6861 7065 2861 7379 6d5f  np.reshape(asym_
+00005f60: 7368 6170 652c 2028 312c 322c 705f 6d61  shape, (1,2,p_ma
+00005f70: 782b 312c 705f 6d61 782b 3129 290a 0a20  x+1,p_max+1)).. 
+00005f80: 2020 2023 2044 6f75 626c 6520 6368 6563     # Double chec
+00005f90: 6b20 6172 7261 7920 6c65 6e67 7468 7320  k array lengths 
+00005fa0: 616c 6c20 6d61 7463 6820 7570 0a20 2020  all match up.   
+00005fb0: 2069 6620 6e70 2e73 6861 7065 2861 7379   if np.shape(asy
+00005fc0: 6d5f 7368 6170 6529 2021 3d20 286e 702e  m_shape) != (np.
+00005fd0: 7369 7a65 2872 5f62 6473 292c 322c 705f  size(r_bds),2,p_
+00005fe0: 6d61 782b 312c 705f 6d61 782b 3129 3a0a  max+1,p_max+1):.
+00005ff0: 2020 2020 2020 2020 6966 206e 702e 7368          if np.sh
+00006000: 6170 6528 725f 6264 7329 2021 3d20 6e70  ape(r_bds) != np
+00006010: 2e73 6861 7065 2861 7379 6d5f 7368 6170  .shape(asym_shap
+00006020: 6529 5b30 5d3a 0a20 2020 2020 2020 2020  e)[0]:.         
+00006030: 2020 206c 6f67 2e65 7272 6f72 2866 2262     log.error(f"b
+00006040: 6f75 6e64 6172 6965 7320 6c65 6e67 7468  oundaries length
+00006050: 3a20 7b6e 702e 7368 6170 6528 725f 6264  : {np.shape(r_bd
+00006060: 7329 7d22 290a 2020 2020 2020 2020 2020  s)}").          
+00006070: 2020 6c6f 672e 6572 726f 7228 6622 6465    log.error(f"de
+00006080: 7669 6174 696f 6e73 206c 656e 6774 683a  viations length:
+00006090: 207b 6e70 2e73 6861 7065 2861 7379 6d5f   {np.shape(asym_
+000060a0: 7368 6170 6529 5b30 5d7d 2229 0a20 2020  shape)[0]}").   
+000060b0: 2020 2020 2020 2020 2072 6169 7365 2056           raise V
+000060c0: 616c 7565 4572 726f 7228 2254 6865 206e  alueError("The n
+000060d0: 756d 6265 7220 6f66 2062 6f75 6e64 6172  umber of boundar
+000060e0: 6965 7320 6973 206e 6f74 2065 7175 616c  ies is not equal
+000060f0: 2074 6f20 7468 6520 6e75 6d62 6572 206f   to the number o
+00006100: 6620 6465 7669 6174 696f 6e20 7368 6170  f deviation shap
+00006110: 6573 2e22 290a 2020 2020 2020 2020 656c  es.").        el
+00006120: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+00006130: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
+00006140: 2822 5468 6520 6e75 6d62 6572 206f 6620  ("The number of 
+00006150: 6465 7669 6174 696f 6e20 7368 6170 6573  deviation shapes
+00006160: 2069 7320 6e6f 7420 6571 7561 6c20 746f   is not equal to
+00006170: 2028 705f 6d61 7820 2b20 3129 5e32 202d   (p_max + 1)^2 -
+00006180: 2031 2e22 290a 0a20 2020 2072 6574 7572   1.")..    retur
+00006190: 6e20 725f 6264 732c 2073 6967 6d61 732c  n r_bds, sigmas,
+000061a0: 2061 7379 6d5f 7368 6170 650a 0a23 2323   asym_shape..###
+000061b0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000061c0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000061d0: 2323 2323 2323 2323 2323 0a0a 2222 220a  ##########..""".
+000061e0: 6a6e 7828 292c 2079 6e78 2829 2c20 6a64  jnx(), ynx(), jd
+000061f0: 7828 292c 2079 6478 2829 0a20 2020 2053  x(), ydx().    S
+00006200: 7068 6572 6963 616c 2042 6573 7365 6c20  pherical Bessel 
+00006210: 616e 6420 4e65 756d 616e 6e20 6675 6e63  and Neumann func
+00006220: 7469 6f6e 7320 666f 7220 6465 6772 6565  tions for degree
+00006230: 206e 2061 6e64 2061 7267 756d 656e 7420   n and argument 
+00006240: 782e 0a20 2020 206a 6478 2061 6e64 2079  x..    jdx and y
+00006250: 6478 2061 7265 206a 5f6e 5e5c 7374 6172  dx are j_n^\star
+00006260: 2061 6e64 2079 5f6e 5e5c 7374 6172 2069   and y_n^\star i
+00006270: 6e20 7468 6520 6162 6f76 6520 7075 626c  n the above publ
+00006280: 6963 6174 696f 6e2c 2061 6e64 2061 7265  ication, and are
+00006290: 0a20 2020 2065 7175 616c 2074 6f20 6428  .    equal to d(
+000062a0: 722a 6a6e 7828 6b72 2929 2f64 7220 616e  r*jnx(kr))/dr an
+000062b0: 6420 6428 722a 796e 7828 6b72 2929 2f64  d d(r*ynx(kr))/d
+000062c0: 722c 2072 6573 7065 6374 6976 656c 792e  r, respectively.
+000062d0: 0a20 2020 2055 7361 6765 3a20 6065 7661  .    Usage: `eva
+000062e0: 6c60 203d 206a 6e78 2860 6e60 2c20 6078  l` = jnx(`n`, `x
+000062f0: 6029 0a20 2020 2052 6574 7572 6e73 3a0a  `).    Returns:.
+00006300: 2020 2020 2020 2020 6576 616c 3a20 6d70          eval: mp
+00006310: 632c 2073 6861 7065 286c 656e 2878 2929  c, shape(len(x))
+00006320: 2e20 4c69 7374 206f 6620 7265 7375 6c74  . List of result
+00006330: 7320 6f66 2042 6573 7365 6c20 6675 6e63  s of Bessel func
+00006340: 7469 6f6e 7320 696e 206d 706d 6174 6820  tions in mpmath 
+00006350: 636f 6d70 6c65 7820 286d 7063 2920 666f  complex (mpc) fo
+00006360: 726d 6174 2e20 416c 7761 7973 2072 6574  rmat. Always ret
+00006370: 7572 6e73 2061 6e20 6172 7261 792c 2070  urns an array, p
+00006380: 6f73 7369 626c 7920 6f66 206c 656e 6774  ossibly of lengt
+00006390: 6820 312e 0a20 2020 2050 6172 616d 6574  h 1..    Paramet
+000063a0: 6572 733a 0a20 2020 2020 2020 206e 3a20  ers:.        n: 
+000063b0: 6d70 662e 2044 6567 7265 6520 6f66 2073  mpf. Degree of s
+000063c0: 7068 6572 6963 616c 2042 6573 7365 6c20  pherical Bessel 
+000063d0: 6675 6e63 7469 6f6e 2e20 5368 6f75 6c64  function. Should
+000063e0: 2062 6520 616e 2069 6e74 6567 6572 2c20   be an integer, 
+000063f0: 6465 7370 6974 6520 6265 696e 6720 6f66  despite being of
+00006400: 206d 7066 2074 7970 6520 286d 7573 7420   mpf type (must 
+00006410: 6265 2070 6173 7365 6420 6173 2068 616c  be passed as hal
+00006420: 662d 696e 7465 6765 7220 6f72 6465 7220  f-integer order 
+00006430: 746f 2062 6573 7365 6c6a 292e 0a20 2020  to besselj)..   
+00006440: 2020 2020 2078 3a20 6d70 632c 2073 6861       x: mpc, sha
+00006450: 7065 286e 5f62 6473 292e 2043 6f6d 706c  pe(n_bds). Compl
+00006460: 6578 2061 7267 756d 656e 7420 6f66 2042  ex argument of B
+00006470: 6573 7365 6c20 6675 6e63 7469 6f6e 2028  essel function (
+00006480: 6b72 292e 204d 5553 5420 6265 2061 206c  kr). MUST be a l
+00006490: 6973 7420 6f72 2074 6869 7320 7769 6c6c  ist or this will
+000064a0: 2062 7265 616b 2e20 4d61 6b65 2073 696e   break. Make sin
+000064b0: 676c 6520 7661 6c75 6573 2069 6e74 6f20  gle values into 
+000064c0: 6c69 7374 7320 7769 7468 2078 203d 205b  lists with x = [
+000064d0: 785d 2e0a 2020 2020 2222 220a 6465 6620  x]..    """.def 
+000064e0: 6a6e 7828 6e2c 7829 3a0a 2020 2020 7477  jnx(n,x):.    tw
+000064f0: 6f20 3d20 6d70 2e6d 7066 2832 290a 2020  o = mp.mpf(2).  
+00006500: 2020 6a6e 7820 3d20 6e70 2e61 7272 6179    jnx = np.array
+00006510: 285b 206d 702e 6265 7373 656c 6a28 206e  ([ mp.besselj( n
+00006520: 2b6d 702e 6d70 6628 2230 2e35 2229 2c78  +mp.mpf("0.5"),x
+00006530: 6920 2920 2a20 6d70 2e73 7172 7428 6d70  i ) * mp.sqrt(mp
+00006540: 2e70 692f 7477 6f2f 7869 2920 666f 7220  .pi/two/xi) for 
+00006550: 7869 2069 6e20 7820 5d29 0a20 2020 2072  xi in x ]).    r
+00006560: 6574 7572 6e20 6a6e 780a 6465 6620 796e  eturn jnx.def yn
+00006570: 7828 6e2c 7829 3a0a 2020 2020 7477 6f20  x(n,x):.    two 
+00006580: 3d20 6d70 2e6d 7066 2832 290a 2020 2020  = mp.mpf(2).    
+00006590: 796e 7820 3d20 6e70 2e61 7272 6179 285b  ynx = np.array([
+000065a0: 206d 702e 6265 7373 656c 7928 206e 2b6d   mp.bessely( n+m
+000065b0: 702e 6d70 6628 2230 2e35 2229 2c78 6920  p.mpf("0.5"),xi 
+000065c0: 2920 2a20 6d70 2e73 7172 7428 6d70 2e70  ) * mp.sqrt(mp.p
+000065d0: 692f 7477 6f2f 7869 2920 666f 7220 7869  i/two/xi) for xi
+000065e0: 2069 6e20 7820 5d29 0a20 2020 2072 6574   in x ]).    ret
+000065f0: 7572 6e20 796e 780a 6465 6620 6a64 7828  urn ynx.def jdx(
+00006600: 6e2c 7829 3a0a 2020 2020 6f6e 6520 3d20  n,x):.    one = 
+00006610: 6d70 2e6d 7066 2831 290a 2020 2020 6a6e  mp.mpf(1).    jn
+00006620: 203d 206a 6e78 286e 2c78 290a 2020 2020   = jnx(n,x).    
+00006630: 6a50 203d 206a 6e78 286e 2b6f 6e65 2c78  jP = jnx(n+one,x
+00006640: 290a 2020 2020 6a64 7820 3d20 6e70 2e61  ).    jdx = np.a
+00006650: 7272 6179 285b 2028 6e2b 6f6e 6529 2a6a  rray([ (n+one)*j
+00006660: 6e5b 695d 202d 2078 5b69 5d2a 6a50 5b69  n[i] - x[i]*jP[i
+00006670: 5d20 666f 7220 6920 696e 2072 616e 6765  ] for i in range
+00006680: 286e 702e 7369 7a65 2878 2929 205d 290a  (np.size(x)) ]).
+00006690: 2020 2020 7265 7475 726e 206a 6478 0a64      return jdx.d
+000066a0: 6566 2079 6478 286e 2c78 293a 0a20 2020  ef ydx(n,x):.   
+000066b0: 206f 6e65 203d 206d 702e 6d70 6628 3129   one = mp.mpf(1)
+000066c0: 0a20 2020 2079 6e20 3d20 796e 7828 6e2c  .    yn = ynx(n,
+000066d0: 7829 0a20 2020 2079 5020 3d20 796e 7828  x).    yP = ynx(
+000066e0: 6e2b 6f6e 652c 7829 0a20 2020 2079 6478  n+one,x).    ydx
+000066f0: 203d 206e 702e 6172 7261 7928 5b20 286e   = np.array([ (n
+00006700: 2b6f 6e65 292a 796e 5b69 5d20 2d20 785b  +one)*yn[i] - x[
+00006710: 695d 2a79 505b 695d 2066 6f72 2069 2069  i]*yP[i] for i i
+00006720: 6e20 7261 6e67 6528 6e70 2e73 697a 6528  n range(np.size(
+00006730: 7829 2920 5d29 0a20 2020 2072 6574 7572  x)) ]).    retur
+00006740: 6e20 7964 780a 0a23 2323 2323 2323 2323  n ydx..#########
+00006750: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00006760: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00006770: 2323 2323 0a0a 2222 220a 7265 6164 5f42  ####..""".read_B
+00006780: 656e 6d28 290a 2020 2020 5265 6164 2069  enm().    Read i
+00006790: 6e20 7468 6520 636f 6d70 6c65 7820 6672  n the complex fr
+000067a0: 6571 7565 6e63 7920 7370 6563 7472 756d  equency spectrum
+000067b0: 206f 6620 6578 6369 7461 7469 6f6e 2066   of excitation f
+000067c0: 6965 6c64 206f 7363 696c 6c61 7469 6f6e  ield oscillation
+000067d0: 7320 666f 7220 7468 6520 7374 726f 6e67  s for the strong
+000067e0: 6573 7420 6578 6369 7461 7469 6f6e 732e  est excitations.
+000067f0: 0a20 2020 2055 7361 6765 3a20 6070 6561  .    Usage: `pea
+00006800: 6b5f 7065 7269 6f64 7360 2c20 6042 656e  k_periods`, `Ben
+00006810: 6d60 203d 2072 6561 645f 4265 6e6d 2860  m` = read_Benm(`
+00006820: 6e70 726d 5f6d 6178 602c 2060 705f 6d61  nprm_max`, `p_ma
+00006830: 7860 2c20 6062 6f64 796e 616d 653d 4e6f  x`, `bodyname=No
+00006840: 6e65 602c 2060 6670 6174 683d 4e6f 6e65  ne`, `fpath=None
+00006850: 602c 2060 7379 6e6f 6469 633d 4661 6c73  `, `synodic=Fals
+00006860: 6560 2c20 606f 7262 6974 616c 3d46 616c  e`, `orbital=Fal
+00006870: 7365 6029 0a20 2020 2052 6574 7572 6e73  se`).    Returns
+00006880: 3a0a 2020 2020 2020 2020 7065 616b 5f70  :.        peak_p
+00006890: 6572 696f 6473 3a20 666c 6f61 742c 2073  eriods: float, s
+000068a0: 6861 7065 286e 5f70 6561 6b73 292e 2050  hape(n_peaks). P
+000068b0: 6572 696f 6473 2069 6e20 6872 206f 6620  eriods in hr of 
+000068c0: 7065 616b 206f 7363 696c 6c61 7469 6f6e  peak oscillation
+000068d0: 732e 2056 616c 7565 7320 7265 6164 2066  s. Values read f
+000068e0: 726f 6d20 6669 6c65 7320 6172 6520 6173  rom files are as
+000068f0: 7375 6d65 6420 746f 2062 6520 696e 2068  sumed to be in h
+00006900: 722e 0a20 2020 2020 2020 2042 656e 6d3a  r..        Benm:
+00006910: 2063 6f6d 706c 6578 2c20 7368 6170 6528   complex, shape(
+00006920: 6e5f 7065 616b 732c 322c 6e70 726d 5f6d  n_peaks,2,nprm_m
+00006930: 6178 2b70 5f6d 6178 2b31 2c6e 7072 6d5f  ax+p_max+1,nprm_
+00006940: 6d61 782b 705f 6d61 782b 3129 2e20 4578  max+p_max+1). Ex
+00006950: 6369 7461 7469 6f6e 206d 6f6d 656e 7473  citation moments
+00006960: 2066 6f72 2065 6163 6820 7065 7269 6f64   for each period
+00006970: 2069 6e20 6e54 2e0a 2020 2020 2020 2020   in nT..        
+00006980: 4230 3a20 666c 6f61 742c 2073 6861 7065  B0: float, shape
+00006990: 2833 292e 2053 7461 7469 6320 6261 636b  (3). Static back
+000069a0: 6772 6f75 6e64 2066 6965 6c64 2e20 5573  ground field. Us
+000069b0: 6564 2074 6f20 7265 636f 6e73 7472 7563  ed to reconstruc
+000069c0: 7420 7468 6520 6e65 7420 6d61 676e 6574  t the net magnet
+000069d0: 6963 2066 6965 6c64 2066 6f72 206d 6561  ic field for mea
+000069e0: 7375 7265 6d65 6e74 2063 6f6d 7061 7269  surement compari
+000069f0: 736f 6e73 2e0a 2020 2020 5061 7261 6d65  sons..    Parame
+00006a00: 7465 7273 3a0a 2020 2020 2020 2020 6e70  ters:.        np
+00006a10: 726d 5f6d 6178 3a20 696e 7465 6765 722e  rm_max: integer.
+00006a20: 204d 6178 696d 756d 2064 6567 7265 6520   Maximum degree 
+00006a30: 6f66 2065 7863 6974 6174 696f 6e20 6861  of excitation ha
+00006a40: 726d 6f6e 6963 7320 746f 2069 6e70 7574  rmonics to input
+00006a50: 2e20 6e27 2076 616c 7565 7320 6170 7065  . n' values appe
+00006a60: 6172 2069 6e20 6669 6c65 206e 616d 6573  ar in file names
+00006a70: 2c20 736f 2061 7070 726f 7072 6961 7465  , so appropriate
+00006a80: 2066 696c 6573 206d 7573 740a 2020 2020   files must.    
+00006a90: 2020 2020 2020 2020 616c 6c20 6265 2070          all be p
+00006aa0: 7265 7365 6e74 2066 726f 6d20 6e27 3d31  resent from n'=1
+00006ab0: 2074 6f20 6e27 3d6e 7072 6d5f 6d61 782e   to n'=nprm_max.
+00006ac0: 0a20 2020 2020 2020 2070 5f6d 6178 3a20  .        p_max: 
+00006ad0: 696e 7465 6765 722e 204d 6178 696d 756d  integer. Maximum
+00006ae0: 2064 6567 7265 6520 6f66 2062 6f75 6e64   degree of bound
+00006af0: 6172 7920 7368 6170 6573 2e20 5265 7175  ary shapes. Requ
+00006b00: 6972 6564 2074 6f20 7369 7a65 2042 656e  ired to size Ben
+00006b10: 6d20 6172 7261 7920 636f 7272 6563 746c  m array correctl
+00006b20: 7920 666f 7220 6661 7374 2063 6f6d 7075  y for fast compu
+00006b30: 7461 7469 6f6e 206f 6620 626f 756e 6461  tation of bounda
+00006b40: 7279 2063 6f6e 6469 7469 6f6e 732e 0a20  ry conditions.. 
+00006b50: 2020 2020 2020 2062 6f64 796e 616d 653a         bodyname:
+00006b60: 2073 7472 696e 6720 284e 6f6e 6529 2e20   string (None). 
+00006b70: 426f 6479 206e 616d 6520 6173 2069 7420  Body name as it 
+00006b80: 6170 7065 6172 7320 696e 2066 696c 6520  appears in file 
+00006b90: 6e61 6d65 732e 2049 6620 4e6f 6e65 2c20  names. If None, 
+00006ba0: 6120 6765 6e65 7269 6320 6669 6c65 206e  a generic file n
+00006bb0: 616d 6520 7769 6c6c 2062 6520 7365 6172  ame will be sear
+00006bc0: 6368 6564 2066 6f72 2e0a 2020 2020 2020  ched for..      
+00006bd0: 2020 6670 6174 683a 2073 7472 696e 6720    fpath: string 
+00006be0: 284e 6f6e 6529 2e20 4f70 7469 6f6e 616c  (None). Optional
+00006bf0: 206c 6f63 6174 696f 6e20 746f 2073 6561   location to sea
+00006c00: 7263 6820 666f 7220 6578 6369 7461 7469  rch for excitati
+00006c10: 6f6e 206d 6f6d 656e 7420 6669 6c65 732e  on moment files.
+00006c20: 2044 6566 6175 6c74 7320 746f 2022 6578   Defaults to "ex
+00006c30: 6369 7461 7469 6f6e 2f22 2e0a 2020 2020  citation/"..    
+00006c40: 2020 2020 7379 6e6f 6469 633a 2062 6f6f      synodic: boo
+00006c50: 6c65 616e 2028 4661 6c73 6529 2e20 4f70  lean (False). Op
+00006c60: 7469 6f6e 2074 6f20 636f 6e73 6964 6572  tion to consider
+00006c70: 206f 6e6c 7920 7468 6520 7374 726f 6e67   only the strong
+00006c80: 6573 7420 6578 6369 7461 7469 6f6e 2070  est excitation p
+00006c90: 6572 696f 642c 2066 6f72 2073 696d 706c  eriod, for simpl
+00006ca0: 6963 6974 792e 0a20 2020 2020 2020 206f  icity..        o
+00006cb0: 7262 6974 616c 3a20 626f 6f6c 6561 6e20  rbital: boolean 
+00006cc0: 2846 616c 7365 292e 204f 7074 696f 6e20  (False). Option 
+00006cd0: 746f 2063 6f6e 7369 6465 7220 6f6e 6c79  to consider only
+00006ce0: 2074 6865 206f 7262 6974 616c 2070 6572   the orbital per
+00006cf0: 696f 642c 2061 6e61 6c6f 676f 7573 2074  iod, analogous t
+00006d00: 6f20 7468 6520 7379 6e6f 6469 6320 7065  o the synodic pe
+00006d10: 7269 6f64 2061 626f 7665 2e0a 2020 2020  riod above..    
+00006d20: 2020 2020 6c69 6d69 745f 6f73 633a 2069      limit_osc: i
+00006d30: 6e74 6567 6572 2028 4e6f 6e65 292e 204e  nteger (None). N
+00006d40: 756d 6265 7220 6f66 206f 7363 696c 6c61  umber of oscilla
+00006d50: 7469 6f6e 2066 7265 7175 656e 6369 6573  tion frequencies
+00006d60: 2074 6f20 6c69 6d69 7420 6361 6c63 756c   to limit calcul
+00006d70: 6174 696f 6e73 2074 6f2c 2077 6865 7265  ations to, where
+00006d80: 2031 2069 7320 6a75 7374 2074 6865 2073   1 is just the s
+00006d90: 7472 6f6e 6765 7374 206f 7363 696c 6c61  trongest oscilla
+00006da0: 7469 6f6e 2e0a 2020 2020 2020 2020 6d6f  tion..        mo
+00006db0: 6465 6c3a 2073 7472 696e 6720 284e 6f6e  del: string (Non
+00006dc0: 6529 2e20 4f70 7469 6f6e 616c 206d 6f64  e). Optional mod
+00006dd0: 656c 2063 6f64 6520 746f 2061 7070 656e  el code to appen
+00006de0: 6420 746f 2066 696c 6520 6e61 6d65 2e0a  d to file name..
+00006df0: 2020 2020 2020 2020 664e 616d 653a 2073          fName: s
+00006e00: 7472 696e 6720 284e 6f6e 6529 2e20 4f70  tring (None). Op
+00006e10: 7469 6f6e 616c 206f 7665 7272 6964 6520  tional override 
+00006e20: 6f66 206e 616d 696e 6720 636f 6e76 656e  of naming conven
+00006e30: 7469 6f6e 7320 746f 2073 7065 6369 6679  tions to specify
+00006e40: 2066 696c 656e 616d 652e 2020 0a20 2020   filename.  .   
+00006e50: 2022 2222 0a64 6566 2072 6561 645f 4265   """.def read_Be
+00006e60: 6e6d 286e 7072 6d5f 6d61 782c 2070 5f6d  nm(nprm_max, p_m
+00006e70: 6178 2c20 626f 6479 6e61 6d65 3d4e 6f6e  ax, bodyname=Non
+00006e80: 652c 2066 7061 7468 3d4e 6f6e 652c 2073  e, fpath=None, s
+00006e90: 796e 6f64 6963 3d46 616c 7365 2c20 6f72  ynodic=False, or
+00006ea0: 6269 7461 6c3d 4661 6c73 652c 206c 696d  bital=False, lim
+00006eb0: 6974 5f6f 7363 3d4e 6f6e 652c 0a20 2020  it_osc=None,.   
+00006ec0: 2020 2020 2020 2020 2020 206d 6f64 656c             model
+00006ed0: 3d4e 6f6e 652c 2066 4e61 6d65 3d4e 6f6e  =None, fName=Non
+00006ee0: 6529 3a0a 2020 2020 6966 2066 7061 7468  e):.    if fpath
+00006ef0: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
+00006f00: 2020 6670 6174 6820 3d20 5f65 7863 6974    fpath = _excit
+00006f10: 6174 696f 6e0a 2020 2020 6966 206d 6f64  ation.    if mod
+00006f20: 656c 2069 7320 4e6f 6e65 3a0a 2020 2020  el is None:.    
+00006f30: 2020 2020 6d6f 6465 6c53 7472 203d 2022      modelStr = "
+00006f40: 220a 2020 2020 656c 7365 3a0a 2020 2020  ".    else:.    
+00006f50: 2020 2020 6d6f 6465 6c53 7472 203d 2066      modelStr = f
+00006f60: 225f 7b6d 6f64 656c 7d22 0a20 2020 2069  "_{model}".    i
+00006f70: 6620 626f 6479 6e61 6d65 2069 7320 4e6f  f bodyname is No
+00006f80: 6e65 3a0a 2020 2020 2020 2020 6266 6e61  ne:.        bfna
+00006f90: 6d65 203d 2066 227b 6d6f 6465 6c53 7472  me = f"{modelStr
+00006fa0: 7d22 0a20 2020 2065 6c73 653a 0a20 2020  }".    else:.   
+00006fb0: 2020 2020 2062 666e 616d 6520 3d20 6622       bfname = f"
+00006fc0: 5f7b 626f 6479 6e61 6d65 7d7b 6d6f 6465  _{bodyname}{mode
+00006fd0: 6c53 7472 7d22 0a0a 2020 2020 6966 2073  lStr}"..    if s
+00006fe0: 796e 6f64 6963 2061 6e64 206f 7262 6974  ynodic and orbit
+00006ff0: 616c 3a0a 2020 2020 2020 2020 6c6f 672e  al:.        log.
+00007000: 7761 726e 696e 6728 2242 6f74 6820 2773  warning("Both 's
+00007010: 796e 6f64 6963 2720 616e 6420 276f 7262  ynodic' and 'orb
+00007020: 6974 616c 2720 6f70 7469 6f6e 7320 7061  ital' options pa
+00007030: 7373 6564 2074 6f20 6173 796d 6d65 7472  ssed to asymmetr
+00007040: 795f 6675 6e63 732e 7265 6164 5f42 656e  y_funcs.read_Ben
+00007050: 6d2e 204f 6e6c 7920 7379 6e6f 6469 6320  m. Only synodic 
+00007060: 7769 6c6c 2062 6520 7573 6564 2e22 290a  will be used.").
+00007070: 2020 2020 2020 2020 6f72 6269 7461 6c20          orbital 
+00007080: 3d20 4661 6c73 650a 0a20 2020 2069 6620  = False..    if 
+00007090: 7379 6e6f 6469 633a 0a20 2020 2020 2020  synodic:.       
+000070a0: 206c 6f67 2e77 6172 6e69 6e67 2822 436f   log.warning("Co
+000070b0: 6e73 6964 6572 696e 6720 7379 6e6f 6469  nsidering synodi
+000070c0: 6320 7065 7269 6f64 206f 6e6c 7920 666f  c period only fo
+000070d0: 7220 6578 6369 7461 7469 6f6e 2e22 290a  r excitation.").
+000070e0: 2020 2020 2020 2020 6966 2066 4e61 6d65          if fName
+000070f0: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
+00007100: 2020 2020 2020 4265 6e6d 5f6d 6f6d 656e        Benm_momen
+00007110: 7473 203d 206f 732e 7061 7468 2e6a 6f69  ts = os.path.joi
+00007120: 6e28 6670 6174 682c 2066 2273 796e 6f64  n(fpath, f"synod
+00007130: 6963 5f42 6531 7879 7a7b 6266 6e61 6d65  ic_Be1xyz{bfname
+00007140: 7d2e 7478 7422 290a 2020 2020 2020 2020  }.txt").        
+00007150: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+00007160: 2020 6c69 6d69 745f 6f73 6320 3d20 310a    limit_osc = 1.
+00007170: 2020 2020 2020 2020 2020 2020 4265 6e6d              Benm
+00007180: 5f6d 6f6d 656e 7473 203d 206f 732e 7061  _moments = os.pa
+00007190: 7468 2e6a 6f69 6e28 6670 6174 682c 2066  th.join(fpath, f
+000071a0: 227b 664e 616d 657d 2e74 7874 2229 0a20  "{fName}.txt"). 
+000071b0: 2020 2065 6c69 6620 6f72 6269 7461 6c3a     elif orbital:
+000071c0: 0a20 2020 2020 2020 206c 6f67 2e77 6172  .        log.war
+000071d0: 6e69 6e67 2822 436f 6e73 6964 6572 696e  ning("Considerin
+000071e0: 6720 6f72 6269 7461 6c20 7065 7269 6f64  g orbital period
+000071f0: 206f 6e6c 7920 666f 7220 6578 6369 7461   only for excita
+00007200: 7469 6f6e 2e22 290a 2020 2020 2020 2020  tion.").        
+00007210: 6966 2062 6f64 796e 616d 6520 3d3d 2022  if bodyname == "
+00007220: 4575 726f 7061 223a 0a20 2020 2020 2020  Europa":.       
+00007230: 2020 2020 206c 6f67 2e77 6172 6e69 6e67       log.warning
+00007240: 2822 4578 7472 6120 7761 726e 696e 673a  ("Extra warning:
+00007250: 2054 6869 7320 6578 6369 7461 7469 6f6e   This excitation
+00007260: 2069 7320 4150 5052 4f58 494d 4154 452c   is APPROXIMATE,
+00007270: 2069 6e20 7468 6174 2074 776f 2063 6c6f   in that two clo
+00007280: 7365 6c79 2d73 7061 6365 6420 7065 7269  sely-spaced peri
+00007290: 6f64 7320 6861 7665 2062 6565 6e20 7375  ods have been su
+000072a0: 6d6d 6564 2074 6f67 6574 6865 7220 616e  mmed together an
+000072b0: 6420 7365 7420 746f 2054 203d 2038 352e  d set to T = 85.
+000072c0: 3220 682e 2229 0a20 2020 2020 2020 2042  2 h.").        B
+000072d0: 656e 6d5f 6d6f 6d65 6e74 7320 3d20 6f73  enm_moments = os
+000072e0: 2e70 6174 682e 6a6f 696e 2866 7061 7468  .path.join(fpath
+000072f0: 2c20 6622 6f72 6269 7461 6c5f 4265 3178  , f"orbital_Be1x
+00007300: 797a 7b62 666e 616d 657d 2e74 7874 2229  yz{bfname}.txt")
+00007310: 0a20 2020 2065 6c73 653a 0a20 2020 2020  .    else:.     
+00007320: 2020 2069 6620 664e 616d 6520 6973 204e     if fName is N
+00007330: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00007340: 2066 4e61 6d65 203d 2066 2742 6531 7879   fName = f'Be1xy
+00007350: 7a7b 6266 6e61 6d65 7d27 0a20 2020 2020  z{bfname}'.     
+00007360: 2020 2042 656e 6d5f 6d6f 6d65 6e74 7320     Benm_moments 
+00007370: 3d20 6f73 2e70 6174 682e 6a6f 696e 2866  = os.path.join(f
+00007380: 7061 7468 2c20 6622 7b66 4e61 6d65 7d2e  path, f"{fName}.
+00007390: 7478 7422 290a 2020 2020 6c6f 672e 6465  txt").    log.de
+000073a0: 6275 6728 6622 5573 696e 6720 6578 6369  bug(f"Using exci
+000073b0: 7461 7469 6f6e 206d 6f6d 656e 7473 3a20  tation moments: 
+000073c0: 7b42 656e 6d5f 6d6f 6d65 6e74 737d 2229  {Benm_moments}")
+000073d0: 0a20 2020 2070 6561 6b5f 7065 7231 2c20  .    peak_per1, 
+000073e0: 4230 782c 2042 3079 2c20 4230 7a2c 2042  B0x, B0y, B0z, B
+000073f0: 6578 5f52 652c 2042 6578 5f49 6d2c 2042  ex_Re, Bex_Im, B
+00007400: 6579 5f52 652c 2042 6579 5f49 6d2c 2042  ey_Re, Bey_Im, B
+00007410: 657a 5f52 652c 2042 657a 5f49 6d20 3d20  ez_Re, Bez_Im = 
+00007420: 6e70 2e6c 6f61 6474 7874 2842 656e 6d5f  np.loadtxt(Benm_
+00007430: 6d6f 6d65 6e74 732c 2073 6b69 7072 6f77  moments, skiprow
+00007440: 733d 312c 2075 6e70 6163 6b3d 5472 7565  s=1, unpack=True
+00007450: 2c20 6465 6c69 6d69 7465 723d 272c 2729  , delimiter=',')
+00007460: 0a20 2020 206e 5f70 6561 6b73 315f 7072  .    n_peaks1_pr
+00007470: 656c 696d 203d 2070 6561 6b5f 7065 7231  elim = peak_per1
+00007480: 2e73 697a 650a 0a20 2020 2042 6578 203d  .size..    Bex =
+00007490: 2042 6578 5f52 6520 2b20 316a 202a 2042   Bex_Re + 1j * B
+000074a0: 6578 5f49 6d0a 2020 2020 4265 7920 3d20  ex_Im.    Bey = 
+000074b0: 4265 795f 5265 202b 2031 6a20 2a20 4265  Bey_Re + 1j * Be
+000074c0: 795f 496d 0a20 2020 2042 657a 203d 2042  y_Im.    Bez = B
+000074d0: 657a 5f52 6520 2b20 316a 202a 2042 657a  ez_Re + 1j * Bez
+000074e0: 5f49 6d0a 0a20 2020 2069 6620 6c69 6d69  _Im..    if limi
+000074f0: 745f 6f73 6320 6973 204e 6f6e 653a 0a20  t_osc is None:. 
+00007500: 2020 2020 2020 206c 696d 6974 5f6f 7363         limit_osc
+00007510: 203d 2030 0a20 2020 2065 6c69 6620 6c69   = 0.    elif li
+00007520: 6d69 745f 6f73 6320 213d 2030 3a0a 2020  mit_osc != 0:.  
+00007530: 2020 2020 2020 6966 206e 5f70 6561 6b73        if n_peaks
+00007540: 315f 7072 656c 696d 203c 3d20 6c69 6d69  1_prelim <= limi
+00007550: 745f 6f73 633a 0a20 2020 2020 2020 2020  t_osc:.         
+00007560: 2020 206c 6f67 2e64 6562 7567 2866 226c     log.debug(f"l
+00007570: 696d 6974 5f6f 7363 2069 7320 7365 7420  imit_osc is set 
+00007580: 746f 207b 6c69 6d69 745f 6f73 637d 2c20  to {limit_osc}, 
+00007590: 6275 7420 7b42 656e 6d5f 6d6f 6d65 6e74  but {Benm_moment
+000075a0: 737d 2063 6f6e 7461 696e 7320 6f6e 6c79  s} contains only
+000075b0: 207b 6e5f 7065 616b 7331 5f70 7265 6c69   {n_peaks1_preli
+000075c0: 6d7d 206f 7363 696c 6c61 7469 6f6e 2070  m} oscillation p
+000075d0: 6572 696f 6473 2e20 496e 636c 7564 696e  eriods. Includin
+000075e0: 6720 616c 6c20 6f73 6369 6c6c 6174 696f  g all oscillatio
+000075f0: 6e73 2069 6e20 6361 6c63 756c 6174 696f  ns in calculatio
+00007600: 6e73 2e22 290a 2020 2020 2020 2020 2020  ns.").          
+00007610: 2020 6c69 6d69 745f 6f73 6320 3d20 300a    limit_osc = 0.
+00007620: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+00007630: 2020 2020 2020 2020 2020 6966 206c 696d            if lim
+00007640: 6974 5f6f 7363 203c 2030 3a20 6c69 6d69  it_osc < 0: limi
+00007650: 745f 6f73 6320 3d20 6162 7328 6c69 6d69  t_osc = abs(limi
+00007660: 745f 6f73 6329 0a20 2020 2020 2020 2020  t_osc).         
+00007670: 2020 206c 6f67 2e64 6562 7567 2866 224c     log.debug(f"L
+00007680: 696d 6974 696e 6720 4265 6e6d 2074 6f20  imiting Benm to 
+00007690: 7374 726f 6e67 6573 7420 7b6c 696d 6974  strongest {limit
+000076a0: 5f6f 7363 7d20 6f73 6369 6c6c 6174 696f  _osc} oscillatio
+000076b0: 6e73 2e22 290a 2020 2020 6162 7342 656e  ns.").    absBen
+000076c0: 6d20 3d20 6e70 2e73 7172 7428 4265 785f  m = np.sqrt(Bex_
+000076d0: 5265 2a2a 3220 2b20 4265 785f 496d 2a2a  Re**2 + Bex_Im**
+000076e0: 3220 2b20 4265 795f 5265 2a2a 3220 2b20  2 + Bey_Re**2 + 
+000076f0: 4265 795f 496d 2a2a 3220 2b20 4265 7a5f  Bey_Im**2 + Bez_
+00007700: 5265 2a2a 3220 2b20 4265 7a5f 496d 2a2a  Re**2 + Bez_Im**
+00007710: 3229 0a20 2020 2069 6620 7379 6e6f 6469  2).    if synodi
+00007720: 6320 6f72 206f 7262 6974 616c 3a0a 2020  c or orbital:.  
+00007730: 2020 2020 2020 694d 6178 536f 7274 203d        iMaxSort =
+00007740: 2030 0a20 2020 2065 6c73 653a 0a20 2020   0.    else:.   
+00007750: 2020 2020 2069 4d61 7820 3d20 6e70 2e61       iMax = np.a
+00007760: 7267 7061 7274 6974 696f 6e28 6162 7342  rgpartition(absB
+00007770: 656e 6d2c 202d 6c69 6d69 745f 6f73 6329  enm, -limit_osc)
+00007780: 5b2d 6c69 6d69 745f 6f73 633a 5d0a 2020  [-limit_osc:].  
+00007790: 2020 2020 2020 7065 616b 5f70 6572 315f        peak_per1_
+000077a0: 6c69 6d20 3d20 6e70 2e73 6f72 7428 7065  lim = np.sort(pe
+000077b0: 616b 5f70 6572 315b 694d 6178 5d29 0a20  ak_per1[iMax]). 
+000077c0: 2020 2020 2020 2069 4d61 7853 6f72 7420         iMaxSort 
+000077d0: 3d20 6e70 2e61 7272 6179 285b 6e70 2e61  = np.array([np.a
+000077e0: 7267 7768 6572 6528 7065 616b 5f70 6572  rgwhere(peak_per
+000077f0: 3120 3d3d 2070 6561 6b5f 7065 7231 5f6c  1 == peak_per1_l
+00007800: 696d 5b69 5d29 2066 6f72 2069 2069 6e20  im[i]) for i in 
+00007810: 7261 6e67 6528 6e70 2e73 697a 6528 7065  range(np.size(pe
+00007820: 616b 5f70 6572 315f 6c69 6d29 295d 292e  ak_per1_lim))]).
+00007830: 666c 6174 7465 6e28 290a 0a20 2020 2020  flatten()..     
+00007840: 2020 2070 6561 6b5f 7065 7231 203d 2070     peak_per1 = p
+00007850: 6561 6b5f 7065 7231 5b69 4d61 7853 6f72  eak_per1[iMaxSor
+00007860: 745d 0a20 2020 2020 2020 2042 6578 203d  t].        Bex =
+00007870: 2042 6578 5b69 4d61 7853 6f72 745d 0a20   Bex[iMaxSort]. 
+00007880: 2020 2020 2020 2042 6579 203d 2042 6579         Bey = Bey
+00007890: 5b69 4d61 7853 6f72 745d 0a20 2020 2020  [iMaxSort].     
+000078a0: 2020 2042 657a 203d 2042 657a 5b69 4d61     Bez = Bez[iMa
+000078b0: 7853 6f72 745d 0a20 2020 2020 2020 200a  xSort].        .
+000078c0: 2020 2020 6e5f 7065 616b 7331 203d 206e      n_peaks1 = n
+000078d0: 702e 7369 7a65 2870 6561 6b5f 7065 7231  p.size(peak_per1
+000078e0: 290a 0a20 2020 2042 656e 6d31 203d 206e  )..    Benm1 = n
+000078f0: 702e 7a65 726f 7328 286e 5f70 6561 6b73  p.zeros((n_peaks
+00007900: 312c 322c 6e70 726d 5f6d 6178 2b70 5f6d  1,2,nprm_max+p_m
+00007910: 6178 2b31 2c6e 7072 6d5f 6d61 782b 705f  ax+1,nprm_max+p_
+00007920: 6d61 782b 3129 2c64 7479 7065 3d6e 702e  max+1),dtype=np.
+00007930: 636f 6d70 6c65 785f 290a 0a20 2020 2041  complex_)..    A
+00007940: 3120 3d20 7371 7274 2832 2a6e 702e 7069  1 = sqrt(2*np.pi
+00007950: 2f33 290a 0a20 2020 2042 656e 6d31 5b3a  /3)..    Benm1[:
+00007960: 2c31 2c31 2c31 5d20 3d20 2d41 3120 2a20  ,1,1,1] = -A1 * 
+00007970: 2842 6578 202b 2031 6a2a 4265 7929 0a20  (Bex + 1j*Bey). 
+00007980: 2020 2042 656e 6d31 5b3a 2c30 2c31 2c30     Benm1[:,0,1,0
+00007990: 5d20 3d20 2d41 312a 7371 7274 2832 2920  ] = -A1*sqrt(2) 
+000079a0: 2a20 4265 7a0a 2020 2020 4265 6e6d 315b  * Bez.    Benm1[
+000079b0: 3a2c 302c 312c 315d 203d 2020 4131 202a  :,0,1,1] =  A1 *
+000079c0: 2028 4265 7820 2d20 316a 2a42 6579 290a   (Bex - 1j*Bey).
+000079d0: 0a20 2020 2023 2047 6574 2073 7461 7469  .    # Get stati
+000079e0: 6320 6261 636b 6772 6f75 6e64 2066 6965  c background fie
+000079f0: 6c64 0a20 2020 2042 3020 3d20 6e70 2e61  ld.    B0 = np.a
+00007a00: 7272 6179 285b 6e70 2e6d 6561 6e28 4230  rray([np.mean(B0
+00007a10: 7829 2c20 6e70 2e6d 6561 6e28 4230 7929  x), np.mean(B0y)
+00007a20: 2c20 6e70 2e6d 6561 6e28 4230 7a29 5d29  , np.mean(B0z)])
+00007a30: 0a20 2020 200a 2020 2020 6966 206e 7072  .    .    if npr
+00007a40: 6d5f 6d61 7820 3e20 313a 0a20 2020 2020  m_max > 1:.     
+00007a50: 2020 206c 6f67 2e77 6172 6e69 6e67 2822     log.warning("
+00007a60: 6e27 3d32 2065 7863 6974 6174 696f 6e20  n'=2 excitation 
+00007a70: 6d6f 6d65 6e74 7320 6172 6520 6265 696e  moments are bein
+00007a80: 6720 636f 6e73 6964 6572 6564 2c20 6275  g considered, bu
+00007a90: 7420 7468 6520 616d 706c 6974 7564 6573  t the amplitudes
+00007aa0: 2061 7265 206a 7573 7420 6120 706c 6163   are just a plac
+00007ab0: 6568 6f6c 6465 7221 2052 656d 6f76 6520  eholder! Remove 
+00007ac0: 7468 6973 2077 6172 6e69 6e67 2077 6865  this warning whe
+00007ad0: 6e20 636f 7272 6563 7420 4265 3278 797a  n correct Be2xyz
+00007ae0: 2068 6176 6520 6265 656e 2069 6e73 7461   have been insta
+00007af0: 6c6c 6564 2e22 290a 2020 2020 2020 2020  lled.").        
+00007b00: 666f 7220 6e6e 2069 6e20 7261 6e67 6528  for nn in range(
+00007b10: 312c 6e70 726d 5f6d 6178 2b31 293a 0a20  1,nprm_max+1):. 
+00007b20: 2020 2020 2020 2020 2020 2069 6620 6e6e             if nn
+00007b30: 203d 3d20 323a 0a20 2020 2020 2020 2020   == 2:.         
+00007b40: 2020 2020 2020 2070 6561 6b5f 7065 7232         peak_per2
+00007b50: 2c20 7842 6578 5f52 652c 2078 4265 785f  , xBex_Re, xBex_
+00007b60: 496d 2c20 7842 6579 5f52 652c 2078 4265  Im, xBey_Re, xBe
+00007b70: 795f 496d 2c20 7842 657a 5f52 652c 2078  y_Im, xBez_Re, x
+00007b80: 4265 7a5f 496d 2c20 7942 657a 5f52 652c  Bez_Im, yBez_Re,
+00007b90: 2079 4265 7a5f 496d 2c20 7a42 657a 5f52   yBez_Im, zBez_R
+00007ba0: 652c 207a 4265 7a5f 496d 2020 2020 5c0a  e, zBez_Im    \.
+00007bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007bc0: 2020 2020 3d20 6e70 2e6c 6f61 6474 7874      = np.loadtxt
+00007bd0: 286f 732e 7061 7468 2e6a 6f69 6e28 6670  (os.path.join(fp
+00007be0: 6174 682c 2066 2242 6532 7879 7a7b 6266  ath, f"Be2xyz{bf
+00007bf0: 6e61 6d65 7d2e 7478 7422 292c 2073 6b69  name}.txt"), ski
+00007c00: 7072 6f77 733d 312c 2075 6e70 6163 6b3d  prows=1, unpack=
+00007c10: 5472 7565 2c20 6465 6c69 6d69 7465 723d  True, delimiter=
+00007c20: 272c 2729 0a20 2020 2020 2020 2020 2020  ',').           
+00007c30: 2020 2020 206e 5f70 6561 6b73 3220 3d20       n_peaks2 = 
+00007c40: 6e70 2e73 697a 6528 7065 616b 5f70 6572  np.size(peak_per
+00007c50: 3229 0a20 2020 2020 2020 2020 2020 2020  2).             
+00007c60: 2020 2042 656e 6d32 203d 206e 702e 7a65     Benm2 = np.ze
+00007c70: 726f 7328 286e 5f70 6561 6b73 322c 322c  ros((n_peaks2,2,
+00007c80: 6e70 726d 5f6d 6178 2b70 5f6d 6178 2b31  nprm_max+p_max+1
+00007c90: 2c6e 7072 6d5f 6d61 782b 705f 6d61 782b  ,nprm_max+p_max+
+00007ca0: 3129 2c20 6474 7970 653d 6e70 2e63 6f6d  1), dtype=np.com
+00007cb0: 706c 6578 5f29 0a0a 2020 2020 2020 2020  plex_)..        
+00007cc0: 2020 2020 2020 2020 7842 6578 203d 2078          xBex = x
+00007cd0: 4265 785f 5265 202b 2031 6a2a 7842 6578  Bex_Re + 1j*xBex
+00007ce0: 5f49 6d0a 2020 2020 2020 2020 2020 2020  _Im.            
+00007cf0: 2020 2020 7842 6579 203d 2078 4265 795f      xBey = xBey_
+00007d00: 5265 202b 2031 6a2a 7842 6579 5f49 6d0a  Re + 1j*xBey_Im.
+00007d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007d20: 7842 657a 203d 2078 4265 7a5f 5265 202b  xBez = xBez_Re +
+00007d30: 2031 6a2a 7842 657a 5f49 6d0a 2020 2020   1j*xBez_Im.    
+00007d40: 2020 2020 2020 2020 2020 2020 7942 657a              yBez
+00007d50: 203d 2079 4265 7a5f 5265 202b 2031 6a2a   = yBez_Re + 1j*
+00007d60: 7942 657a 5f49 6d0a 2020 2020 2020 2020  yBez_Im.        
+00007d70: 2020 2020 2020 2020 7a42 657a 203d 207a          zBez = z
+00007d80: 4265 7a5f 5265 202b 2031 6a2a 7a42 657a  Bez_Re + 1j*zBez
+00007d90: 5f49 6d0a 0a20 2020 2020 2020 2020 2020  _Im..           
+00007da0: 2020 2020 206f 7274 3820 3d20 312f 7371       ort8 = 1/sq
+00007db0: 7274 2838 290a 2020 2020 2020 2020 2020  rt(8).          
+00007dc0: 2020 2020 2020 4132 203d 202d 7371 7274        A2 = -sqrt
+00007dd0: 2836 2a6e 702e 7069 2f35 290a 0a20 2020  (6*np.pi/5)..   
+00007de0: 2020 2020 2020 2020 2020 2020 2042 656e               Ben
+00007df0: 6d32 5b3a 2c31 2c32 2c32 5d20 3d20 2041  m2[:,1,2,2] =  A
+00007e00: 3220 2a20 2878 4265 7820 2b20 316a 2a78  2 * (xBex + 1j*x
+00007e10: 4265 7920 2b20 6f72 7438 2a78 4265 7a29  Bey + ort8*xBez)
+00007e20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007e30: 2042 656e 6d32 5b3a 2c31 2c32 2c31 5d20   Benm2[:,1,2,1] 
+00007e40: 3d20 2041 3220 2a20 2878 4265 7a20 2d20  =  A2 * (xBez - 
+00007e50: 316a 2a79 4265 7a29 0a20 2020 2020 2020  1j*yBez).       
+00007e60: 2020 2020 2020 2020 2042 656e 6d32 5b3a           Benm2[:
+00007e70: 2c30 2c32 2c30 5d20 3d20 2041 3220 2a20  ,0,2,0] =  A2 * 
+00007e80: 7371 7274 2833 2f32 2920 2a20 7a42 657a  sqrt(3/2) * zBez
+00007e90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007ea0: 2042 656e 6d32 5b3a 2c30 2c32 2c31 5d20   Benm2[:,0,2,1] 
+00007eb0: 3d20 2d41 3220 2a20 2878 4265 7a20 2b20  = -A2 * (xBez + 
+00007ec0: 316a 2a79 4265 7a29 0a20 2020 2020 2020  1j*yBez).       
+00007ed0: 2020 2020 2020 2020 2042 656e 6d32 5b3a           Benm2[:
+00007ee0: 2c30 2c32 2c32 5d20 3d20 2041 3220 2a20  ,0,2,2] =  A2 * 
+00007ef0: 2878 4265 7820 2d20 316a 2a78 4265 7920  (xBex - 1j*xBey 
+00007f00: 2b20 6f72 7438 2a78 4265 7a29 0a0a 2020  + ort8*xBez)..  
+00007f10: 2020 2020 2020 2020 2020 2020 2020 4265                Be
+00007f20: 6e6d 203d 206e 702e 7a65 726f 7328 286e  nm = np.zeros((n
+00007f30: 5f70 6561 6b73 312b 6e5f 7065 616b 7332  _peaks1+n_peaks2
+00007f40: 2c32 2c6e 7072 6d5f 6d61 782b 705f 6d61  ,2,nprm_max+p_ma
+00007f50: 782b 312c 6e70 726d 5f6d 6178 2b70 5f6d  x+1,nprm_max+p_m
+00007f60: 6178 2b31 292c 6474 7970 653d 6e70 2e63  ax+1),dtype=np.c
+00007f70: 6f6d 706c 6578 5f29 0a0a 2020 2020 2020  omplex_)..      
+00007f80: 2020 2020 2020 2020 2020 4265 6e6d 5b3a            Benm[:
+00007f90: 6e5f 7065 616b 7331 2c3a 2c3a 2c3a 5d20  n_peaks1,:,:,:] 
+00007fa0: 3d20 4265 6e6d 310a 2020 2020 2020 2020  = Benm1.        
+00007fb0: 2020 2020 2020 2020 4265 6e6d 5b6e 5f70          Benm[n_p
+00007fc0: 6561 6b73 313a 2c3a 2c3a 2c3a 5d20 3d20  eaks1:,:,:,:] = 
+00007fd0: 4265 6e6d 320a 2020 2020 2020 2020 2020  Benm2.          
+00007fe0: 2020 2020 2020 7065 616b 5f70 6572 696f        peak_perio
+00007ff0: 6473 203d 206e 702e 6170 7065 6e64 2870  ds = np.append(p
+00008000: 6561 6b5f 7065 7231 2c70 6561 6b5f 7065  eak_per1,peak_pe
+00008010: 7232 290a 0a20 2020 2020 2020 2020 2020  r2)..           
+00008020: 2065 6c69 6620 6e6e 203e 2032 3a0a 2020   elif nn > 2:.  
+00008030: 2020 2020 2020 2020 2020 2020 2020 7261                ra
+00008040: 6973 6520 5661 6c75 6545 7272 6f72 2822  ise ValueError("
+00008050: 6e5f 6d61 7820 3e3d 2033 2069 7320 6e6f  n_max >= 3 is no
+00008060: 7420 696d 706c 656d 656e 7465 642e 2229  t implemented.")
+00008070: 0a20 2020 2065 6c73 653a 0a20 2020 2020  .    else:.     
+00008080: 2020 2042 656e 6d20 3d20 4265 6e6d 310a     Benm = Benm1.
+00008090: 2020 2020 2020 2020 7065 616b 5f70 6572          peak_per
+000080a0: 696f 6473 203d 2070 6561 6b5f 7065 7231  iods = peak_per1
+000080b0: 0a0a 2020 2020 7265 7475 726e 2070 6561  ..    return pea
+000080c0: 6b5f 7065 7269 6f64 732c 2042 656e 6d2c  k_periods, Benm,
+000080d0: 2042 300a 0a23 2323 2323 2323 2323 2323   B0..###########
+000080e0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000080f0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00008100: 2323 0a0a 2222 220a 4269 4c69 7374 2829  ##..""".BiList()
+00008110: 0a20 2020 2045 7661 6c75 6174 6520 7468  .    Evaluate th
+00008120: 6520 696e 6475 6365 6420 6d61 676e 6574  e induced magnet
+00008130: 6963 206d 6f6d 656e 7473 2042 696e 6d20  ic moments Binm 
+00008140: 666f 7220 7468 6520 6769 7665 6e20 6578  for the given ex
+00008150: 6369 7461 7469 6f6e 206d 6f6d 656e 7473  citation moments
+00008160: 2042 656e 6d2c 0a20 2020 2066 6f72 2074   Benm,.    for t
+00008170: 6865 2067 6976 656e 2069 6e74 6572 696f  he given interio
+00008180: 7220 7374 7275 6374 7572 6520 6465 7363  r structure desc
+00008190: 7269 6265 6420 6279 2072 5f62 6473 2c20  ribed by r_bds, 
+000081a0: 7369 676d 6173 2c20 616e 6420 6173 796d  sigmas, and asym
+000081b0: 5f73 6861 7065 2061 6e64 2066 6f72 2061  _shape and for a
+000081c0: 206c 6973 7420 6f66 206f 6d65 6761 2076   list of omega v
+000081d0: 616c 7565 732e 0a20 2020 2055 7361 6765  alues..    Usage
+000081e0: 3a20 6042 696e 6d73 6020 3d20 4269 4c69  : `Binms` = BiLi
+000081f0: 7374 2860 725f 6264 7360 2c20 6073 6967  st(`r_bds`, `sig
+00008200: 6d61 7360 2c20 6070 6561 6b5f 6f6d 6567  mas`, `peak_omeg
+00008210: 6173 602c 2060 6173 796d 5f73 6861 7065  as`, `asym_shape
+00008220: 602c 2060 4265 6e6d 602c 2060 6e70 726d  `, `Benm`, `nprm
+00008230: 7661 6c73 602c 2060 6d70 726d 7661 6c73  vals`, `mprmvals
+00008240: 602c 2060 7273 6361 6c65 5f6d 6f6d 656e  `, `rscale_momen
+00008250: 7473 602c 0a20 2020 2020 2020 2020 2020  ts`,.           
+00008260: 2020 2020 2020 2020 2020 2020 2020 6070                `p
+00008270: 7661 6c73 602c 2060 7176 616c 7360 2c20  vals`, `qvals`, 
+00008280: 606e 7661 6c73 602c 2060 6d76 616c 7360  `nvals`, `mvals`
+00008290: 2c20 606e 7072 6d5f 6d61 7860 2c20 6070  , `nprm_max`, `p
+000082a0: 5f6d 6178 602c 2060 7772 6974 656f 7574  _max`, `writeout
+000082b0: 3d54 7275 6560 2c20 6070 6174 683d 4e6f  =True`, `path=No
+000082c0: 6e65 602c 0a20 2020 2020 2020 2020 2020  ne`,.           
+000082d0: 2020 2020 2020 2020 2020 2020 2020 6061                `a
+000082e0: 7070 656e 643d 2222 602c 2060 6465 6275  ppend=""`, `debu
+000082f0: 673d 4661 6c73 6560 290a 2020 2020 5265  g=False`).    Re
+00008300: 7475 726e 733a 0a20 2020 2020 2020 2042  turns:.        B
+00008310: 696e 6d73 3a20 636f 6d70 6c65 782c 2073  inms: complex, s
+00008320: 6861 7065 286e 5f70 6561 6b73 2c32 2c6e  hape(n_peaks,2,n
+00008330: 5f6d 6178 2b31 2c6e 5f6d 6178 2b31 292e  _max+1,n_max+1).
+00008340: 204c 6973 7420 6f66 2063 6f6d 706c 6578   List of complex
+00008350: 2069 6e64 7563 6564 206d 6167 6e65 7469   induced magneti
+00008360: 6320 6d6f 6d65 6e74 7320 666f 7220 7468  c moments for th
+00008370: 6520 6769 7665 6e20 7061 7261 6d65 7465  e given paramete
+00008380: 7273 2e0a 2020 2020 5061 7261 6d65 7465  rs..    Paramete
+00008390: 7273 3a0a 2020 2020 2020 2020 725f 6264  rs:.        r_bd
+000083a0: 733a 2066 6c6f 6174 2c20 7368 6170 6528  s: float, shape(
+000083b0: 6e5f 6264 7329 2e20 4c69 7374 206f 6620  n_bds). List of 
+000083c0: 6d65 616e 2072 6164 6969 2066 6f72 2065  mean radii for e
+000083d0: 6163 6820 626f 756e 6461 7279 2073 7572  ach boundary sur
+000083e0: 6661 6365 2069 6e20 6d2e 0a20 2020 2020  face in m..     
+000083f0: 2020 2073 6967 6d61 733a 2066 6c6f 6174     sigmas: float
+00008400: 2c20 7368 6170 6528 6e5f 6264 7329 2e20  , shape(n_bds). 
+00008410: 4c69 7374 206f 6620 636f 6e64 7563 7469  List of conducti
+00008420: 7669 7479 2076 616c 7565 7320 666f 7220  vity values for 
+00008430: 6561 6368 206c 6179 6572 2075 6e64 6572  each layer under
+00008440: 6e65 6174 6820 7468 6520 636f 7272 6573  neath the corres
+00008450: 706f 6e64 696e 6720 626f 756e 6461 7279  ponding boundary
+00008460: 2069 6e20 532f 6d2e 0a20 2020 2020 2020   in S/m..       
+00008470: 2070 6561 6b5f 6f6d 6567 6173 3a20 666c   peak_omegas: fl
+00008480: 6f61 742c 2073 6861 7065 286e 5f70 6561  oat, shape(n_pea
+00008490: 6b73 292e 204c 6973 7420 6f66 2061 6e67  ks). List of ang
+000084a0: 756c 6172 2066 7265 7175 656e 6369 6573  ular frequencies
+000084b0: 2069 6e20 7261 642f 7320 746f 2065 7661   in rad/s to eva
+000084c0: 6c75 6174 652e 2054 7970 6963 616c 6c79  luate. Typically
+000084d0: 206f 6e6c 7920 7468 6520 7065 616b 7320   only the peaks 
+000084e0: 6f66 0a20 2020 2020 2020 2020 2020 2074  of.            t
+000084f0: 6865 2046 6f75 7269 6572 2073 7065 6374  he Fourier spect
+00008500: 7261 2e0a 2020 2020 2020 2020 6173 796d  ra..        asym
+00008510: 5f73 6861 7065 5f6c 6179 6572 733a 2063  _shape_layers: c
+00008520: 6f6d 706c 6578 2c20 7368 6170 6528 6e5f  omplex, shape(n_
+00008530: 6264 732c 322c 705f 6d61 782b 312c 705f  bds,2,p_max+1,p_
+00008540: 6d61 782b 3129 2e20 4162 736f 6c75 7465  max+1). Absolute
+00008550: 2064 6576 6961 7469 6f6e 7320 666f 7220   deviations for 
+00008560: 6561 6368 2062 6f75 6e64 6172 7920 696e  each boundary in
+00008570: 206d 2c20 6967 6e6f 7269 6e67 0a20 2020   m, ignoring.   
+00008580: 2020 2020 2020 2020 2067 7261 7669 7461           gravita
+00008590: 7469 6f6e 616c 2070 6572 7475 7262 6174  tional perturbat
+000085a0: 696f 6e73 2e0a 2020 2020 2020 2020 6772  ions..        gr
+000085b0: 6176 5f73 6861 7065 3a20 636f 6d70 6c65  av_shape: comple
+000085c0: 782c 2073 6861 7065 286e 5f62 6473 2c32  x, shape(n_bds,2
+000085d0: 2c70 5f6d 6178 2b31 2c70 5f6d 6178 2b31  ,p_max+1,p_max+1
+000085e0: 292e 2041 6273 6f6c 7574 6520 6465 7669  ). Absolute devi
+000085f0: 6174 696f 6e73 2066 6f72 2065 6163 6820  ations for each 
+00008600: 2863 6f6e 6475 6374 696e 6729 2062 6f75  (conducting) bou
+00008610: 6e64 6172 7920 696e 206d 2c0a 2020 2020  ndary in m,.    
+00008620: 2020 2020 2020 2020 6475 6520 746f 2067          due to g
+00008630: 7261 7669 7461 7469 6f6e 616c 2070 6572  ravitational per
+00008640: 7475 7262 6174 696f 6e73 2e0a 2020 2020  turbations..    
+00008650: 2020 2020 4265 6e6d 3a20 636f 6d70 6c65      Benm: comple
+00008660: 782c 2073 6861 7065 2832 2c6e 5f6d 6178  x, shape(2,n_max
+00008670: 2b31 2c6e 5f6d 6178 2b31 292e 2045 7863  +1,n_max+1). Exc
+00008680: 6974 6174 696f 6e20 6d6f 6d65 6e74 7320  itation moments 
+00008690: 666f 7220 6561 6368 2064 6567 7265 6520  for each degree 
+000086a0: 616e 6420 6f72 6465 7220 6e27 2c6d 272e  and order n',m'.
+000086b0: 0a20 2020 2020 2020 2072 7363 616c 655f  .        rscale_
+000086c0: 6d6f 6d65 6e74 733a 2066 6c6f 6174 2e20  moments: float. 
+000086d0: 4571 7561 6c20 746f 2031 2f52 5f62 6f64  Equal to 1/R_bod
+000086e0: 7920 696e 2075 6e69 7473 206f 6620 312f  y in units of 1/
+000086f0: 6d2e 2046 6f72 2070 726f 7065 7220 7363  m. For proper sc
+00008700: 616c 696e 6720 7768 656e 2063 6f6e 6475  aling when condu
+00008710: 6374 696e 6720 626f 756e 6461 7269 6573  cting boundaries
+00008720: 0a20 2020 2020 2020 2020 2020 206d 6179  .            may
+00008730: 206f 7220 6d61 7920 6e6f 7420 636f 696e   or may not coin
+00008740: 6369 6465 2077 6974 6820 7468 6520 626f  cide with the bo
+00008750: 6479 2073 7572 6661 6365 2e0a 2020 2020  dy surface..    
+00008760: 2020 2020 6e76 616c 732c 206d 7661 6c73      nvals, mvals
+00008770: 3a20 696e 7465 6765 722c 2073 6861 7065  : integer, shape
+00008780: 284e 6e6d 292e 204c 696e 6561 7220 6172  (Nnm). Linear ar
+00008790: 7261 7973 206f 6620 7061 6972 6564 206e  rays of paired n
+000087a0: 2c6d 2076 616c 7565 7320 666f 7220 7061  ,m values for pa
+000087b0: 7261 6c6c 656c 2063 6f6d 7075 7461 7469  rallel computati
+000087c0: 6f6e 2e0a 2020 2020 2020 2020 705f 6d61  on..        p_ma
+000087d0: 783a 2069 6e74 6567 6572 2e20 4d61 7869  x: integer. Maxi
+000087e0: 6d75 6d20 6465 6772 6565 2070 206f 6620  mum degree p of 
+000087f0: 626f 756e 6461 7279 2073 6861 7065 732e  boundary shapes.
+00008800: 0a20 2020 2020 2020 206e 7072 6d5f 6d61  .        nprm_ma
+00008810: 783a 2069 6e74 6567 6572 2028 3129 2e20  x: integer (1). 
+00008820: 4d61 7869 6d75 6d20 6465 6772 6565 206e  Maximum degree n
+00008830: 2720 6f66 2042 656e 6d20 746f 2065 7661  ' of Benm to eva
+00008840: 6c75 6174 652e 206e 273d 3120 6973 2075  luate. n'=1 is u
+00008850: 6e69 666f 726d 2066 6965 6c64 2076 6563  niform field vec
+00008860: 746f 722e 0a20 2020 2020 2020 2077 7269  tor..        wri
+00008870: 7465 6f75 743a 2062 6f6f 6c65 616e 2028  teout: boolean (
+00008880: 5472 7565 292e 2057 6865 7468 6572 2074  True). Whether t
+00008890: 6f20 7361 7665 2063 6f6d 7075 7465 6420  o save computed 
+000088a0: 7661 6c75 6573 2074 6f20 6469 736b 2066  values to disk f
+000088b0: 6f72 2072 6170 6964 2072 6570 6c6f 7474  or rapid replott
+000088c0: 696e 672e 0a20 2020 2020 2020 2070 6174  ing..        pat
+000088d0: 683a 2073 7472 696e 6720 284e 6f6e 6529  h: string (None)
+000088e0: 2e20 5061 7468 2072 656c 6174 6976 6520  . Path relative 
+000088f0: 746f 2072 756e 2064 6972 6563 746f 7279  to run directory
+00008900: 2074 6f20 7072 696e 7420 6f75 7470 7574   to print output
+00008910: 2064 6174 6120 746f 2e20 4465 6661 756c   data to. Defaul
+00008920: 7473 2074 6f20 223c 696e 7374 616c 6c5f  ts to "<install_
+00008930: 6c6f 633e 2f4d 6f6f 6e4d 6167 2f69 6e64  loc>/MoonMag/ind
+00008940: 7563 6564 2f22 2e0a 2020 2020 2020 2020  uced/"..        
+00008950: 626f 6479 6e61 6d65 3a20 7374 7269 6e67  bodyname: string
+00008960: 2028 4e6f 6e65 292e 2042 6f64 7920 6e61   (None). Body na
+00008970: 6d65 2074 6f20 696e 636c 7564 6520 696e  me to include in
+00008980: 2077 7269 7465 6f75 7420 6669 6c65 6e61   writeout filena
+00008990: 6d65 2e0a 2020 2020 2020 2020 7665 7262  me..        verb
+000089a0: 6f73 653a 2062 6f6f 6c65 616e 2028 5472  ose: boolean (Tr
+000089b0: 7565 292e 2057 6865 7468 6572 2074 6f20  ue). Whether to 
+000089c0: 7072 696e 7420 7072 6f67 7265 7373 2075  print progress u
+000089d0: 7064 6174 6573 2074 6f20 7468 6520 7465  pdates to the te
+000089e0: 726d 696e 616c 2e0a 2020 2020 2020 2020  rminal..        
+000089f0: 6170 7065 6e64 3a20 7374 7269 6e67 2028  append: string (
+00008a00: 2222 292e 204f 7074 696f 6e61 6c20 7374  ""). Optional st
+00008a10: 7269 6e67 2061 7070 656e 6465 6420 746f  ring appended to
+00008a20: 2064 6566 6175 6c74 2066 696c 6520 6e61   default file na
+00008a30: 6d65 732e 0a20 2020 2020 2020 2064 6562  mes..        deb
+00008a40: 7567 3a20 626f 6f6c 6561 6e20 2846 616c  ug: boolean (Fal
+00008a50: 7365 292e 2053 7065 6369 616c 2075 7365  se). Special use
+00008a60: 2066 6c61 672e 0a20 2020 2020 2020 2064   flag..        d
+00008a70: 6f5f 7061 7261 6c6c 656c 3a20 626f 6f6c  o_parallel: bool
+00008a80: 6561 6e20 2854 7275 6529 2e20 546f 6767  ean (True). Togg
+00008a90: 6c65 2066 6f72 2072 756e 6e69 6e67 2063  le for running c
+00008aa0: 6572 7461 696e 2063 616c 6375 6c61 7469  ertain calculati
+00008ab0: 6f6e 7320 696e 2070 6172 616c 6c65 6c2e  ons in parallel.
+00008ac0: 0a20 2020 2020 2020 206f 7574 466e 616d  .        outFnam
+00008ad0: 653a 2073 7472 696e 6720 284e 6f6e 6529  e: string (None)
+00008ae0: 2e20 4f75 7470 7574 2066 696c 656e 616d  . Output filenam
+00008af0: 6520 746f 2075 7365 2077 6865 6e20 7772  e to use when wr
+00008b00: 6974 656f 7574 203d 2054 7275 652e 0a20  iteout = True.. 
+00008b10: 2020 2020 2020 206f 7574 466e 616d 6553         outFnameS
+00008b20: 3a20 7374 7269 6e67 2028 4e6f 6e65 292e  : string (None).
+00008b30: 2041 7320 6162 6f76 652c 2066 6f72 206f   As above, for o
+00008b40: 7574 7075 7420 4761 7573 7320 636f 6566  utput Gauss coef
+00008b50: 6669 6369 656e 7473 2069 6e20 7468 6520  ficients in the 
+00008b60: 5363 686d 6964 7420 6e6f 726d 616c 697a  Schmidt normaliz
+00008b70: 6174 696f 6e2e 0a20 2020 2020 2020 2058  ation..        X
+00008b80: 6964 3a20 636f 6d70 6c65 7820 284e 6f6e  id: complex (Non
+00008b90: 652c 2073 6861 7065 202e 2e2e 292e 204f  e, shape ...). O
+00008ba0: 7074 696f 6e20 746f 2070 6173 7320 696e  ption to pass in
+00008bb0: 2058 6964 2074 6f20 6176 6f69 6420 6e65   Xid to avoid ne
+00008bc0: 6564 696e 6720 746f 2072 656c 6f61 6420  eding to reload 
+00008bd0: 6672 6f6d 2064 6973 6b20 6f72 2072 6563  from disk or rec
+00008be0: 616c 6375 6c61 7465 2e0a 2020 2020 2222  alculate..    ""
+00008bf0: 220a 6465 6620 4269 4c69 7374 2872 5f62  ".def BiList(r_b
+00008c00: 6473 2c20 7369 676d 6173 2c20 7065 616b  ds, sigmas, peak
+00008c10: 5f6f 6d65 6761 732c 2061 7379 6d5f 7368  _omegas, asym_sh
+00008c20: 6170 655f 6c61 7965 7273 2c20 6772 6176  ape_layers, grav
+00008c30: 5f73 6861 7065 2c20 4265 6e6d 2c20 7273  _shape, Benm, rs
+00008c40: 6361 6c65 5f6d 6f6d 656e 7473 2c20 6e76  cale_moments, nv
+00008c50: 616c 732c 206d 7661 6c73 2c20 705f 6d61  als, mvals, p_ma
+00008c60: 782c 206e 7072 6d5f 6d61 783d 312c 2077  x, nprm_max=1, w
+00008c70: 7269 7465 6f75 743d 5472 7565 2c20 7061  riteout=True, pa
+00008c80: 7468 3d4e 6f6e 652c 2062 6f64 796e 616d  th=None, bodynam
+00008c90: 653d 4e6f 6e65 2c0a 2020 2020 2020 2020  e=None,.        
+00008ca0: 2020 2076 6572 626f 7365 3d54 7275 652c     verbose=True,
+00008cb0: 2061 7070 656e 643d 2222 2c20 6465 6275   append="", debu
+00008cc0: 673d 4661 6c73 652c 2064 6f5f 7061 7261  g=False, do_para
+00008cd0: 6c6c 656c 3d54 7275 652c 2053 6368 6d69  llel=True, Schmi
+00008ce0: 6474 3d46 616c 7365 2c20 6f75 7446 6e61  dt=False, outFna
+00008cf0: 6d65 3d4e 6f6e 652c 206f 7574 466e 616d  me=None, outFnam
+00008d00: 6553 3d4e 6f6e 652c 2058 6964 3d4e 6f6e  eS=None, Xid=Non
+00008d10: 6529 3a0a 0a20 2020 2023 2043 6c65 616e  e):..    # Clean
+00008d20: 2069 6e70 7574 7320 616e 6420 696e 6974   inputs and init
+00008d30: 6961 6c69 7a65 0a20 2020 2069 6620 6e6f  ialize.    if no
+00008d40: 7420 6973 696e 7374 616e 6365 2870 6561  t isinstance(pea
+00008d50: 6b5f 6f6d 6567 6173 2c20 4974 6572 6162  k_omegas, Iterab
+00008d60: 6c65 293a 0a20 2020 2020 2020 2070 6561  le):.        pea
+00008d70: 6b5f 6f6d 6567 6173 203d 205b 7065 616b  k_omegas = [peak
+00008d80: 5f6f 6d65 6761 735d 0a20 2020 206e 5f70  _omegas].    n_p
+00008d90: 6561 6b73 203d 206e 702e 7369 7a65 2870  eaks = np.size(p
+00008da0: 6561 6b5f 6f6d 6567 6173 290a 2020 2020  eak_omegas).    
+00008db0: 4e6e 6d20 3d20 6e70 2e73 697a 6528 6e76  Nnm = np.size(nv
+00008dc0: 616c 7329 0a20 2020 206e 5f6d 6178 203d  als).    n_max =
+00008dd0: 206e 7072 6d5f 6d61 7820 2b20 705f 6d61   nprm_max + p_ma
+00008de0: 780a 2020 2020 4269 6e6d 7320 3d20 6e70  x.    Binms = np
+00008df0: 2e7a 6572 6f73 2828 6e5f 7065 616b 732c  .zeros((n_peaks,
+00008e00: 2032 2c20 6e5f 6d61 782b 312c 206e 5f6d   2, n_max+1, n_m
+00008e10: 6178 2b31 292c 2064 7479 7065 3d6e 702e  ax+1), dtype=np.
+00008e20: 636f 6d70 6c65 785f 290a 2020 2020 6c6f  complex_).    lo
+00008e30: 672e 6465 6275 6728 6622 4361 6c63 756c  g.debug(f"Calcul
+00008e40: 6174 696e 6720 6173 796d 6d65 7472 6963  ating asymmetric
+00008e50: 2042 5f69 6e6d 2066 6f72 207b 6e70 2e73   B_inm for {np.s
+00008e60: 697a 6528 7065 616b 5f6f 6d65 6761 7329  ize(peak_omegas)
+00008e70: 7d20 7065 7269 6f64 732e 2229 0a20 2020  } periods.").   
+00008e80: 2069 6620 7772 6974 656f 7574 3a0a 2020   if writeout:.  
+00008e90: 2020 2020 2020 6966 2062 6f64 796e 616d        if bodynam
+00008ea0: 6520 6973 204e 6f6e 653a 0a20 2020 2020  e is None:.     
+00008eb0: 2020 2020 2020 2062 666e 616d 6520 3d20         bfname = 
+00008ec0: 2222 0a20 2020 2020 2020 2065 6c73 653a  "".        else:
+00008ed0: 0a20 2020 2020 2020 2020 2020 2062 666e  .            bfn
+00008ee0: 616d 6520 3d20 6622 7b62 6f64 796e 616d  ame = f"{bodynam
+00008ef0: 657d 5f22 0a20 2020 2069 6620 7273 6361  e}_".    if rsca
+00008f00: 6c65 5f6d 6f6d 656e 7473 203d 3d20 312e  le_moments == 1.
+00008f10: 303a 0a20 2020 2020 2020 2072 7363 616c  0:.        rscal
+00008f20: 696e 6720 3d20 7273 6361 6c65 5f6d 6f6d  ing = rscale_mom
+00008f30: 656e 7473 0a20 2020 2065 6c73 653a 0a20  ents.    else:. 
+00008f40: 2020 2020 2020 2072 7363 616c 696e 6720         rscaling 
+00008f50: 203d 2072 7363 616c 655f 6d6f 6d65 6e74   = rscale_moment
+00008f60: 7320 2a20 725f 6264 735b 2d31 5d0a 2020  s * r_bds[-1].  
+00008f70: 2020 6966 2067 7261 765f 7368 6170 6520    if grav_shape 
+00008f80: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
+00008f90: 2061 7379 6d5f 7368 6170 6520 3d20 6173   asym_shape = as
+00008fa0: 796d 5f73 6861 7065 5f6c 6179 6572 730a  ym_shape_layers.
+00008fb0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00008fc0: 2020 6173 796d 5f73 6861 7065 203d 2061    asym_shape = a
+00008fd0: 7379 6d5f 7368 6170 655f 6c61 7965 7273  sym_shape_layers
+00008fe0: 202b 2067 7261 765f 7368 6170 650a 0a20   + grav_shape.. 
+00008ff0: 2020 2023 2047 6574 206d 6978 696e 6720     # Get mixing 
+00009000: 636f 6566 6669 6369 656e 7473 0a20 2020  coefficients.   
+00009010: 2069 6620 5869 6420 6973 204e 6f6e 653a   if Xid is None:
+00009020: 0a20 2020 2020 2020 2058 6964 203d 2067  .        Xid = g
+00009030: 6574 5f61 6c6c 5f58 6964 286e 7072 6d5f  et_all_Xid(nprm_
+00009040: 6d61 782c 2070 5f6d 6178 2c20 6e70 726d  max, p_max, nprm
+00009050: 5f6d 6178 2b70 5f6d 6178 2c20 6e76 616c  _max+p_max, nval
+00009060: 732c 206d 7661 6c73 2c20 7265 6c6f 6164  s, mvals, reload
+00009070: 3d54 7275 652c 2064 6f5f 7061 7261 6c6c  =True, do_parall
+00009080: 656c 3d64 6f5f 7061 7261 6c6c 656c 2c20  el=do_parallel, 
+00009090: 6670 6174 683d 7061 7468 290a 0a20 2020  fpath=path)..   
+000090a0: 2069 6620 646f 5f70 6172 616c 6c65 6c20   if do_parallel 
+000090b0: 616e 6420 6e6f 7420 6465 6275 673a 0a20  and not debug:. 
+000090c0: 2020 2020 2020 2070 6172 5f6b 7720 3d20         par_kw = 
+000090d0: 7b27 6e70 726d 5f6d 6178 273a 6e70 726d  {'nprm_max':nprm
+000090e0: 5f6d 6178 2c20 2776 6572 626f 7365 273a  _max, 'verbose':
+000090f0: 7665 7262 6f73 657d 0a20 2020 2020 2020  verbose}.       
+00009100: 2023 2046 6f72 2065 6163 6820 6f6d 6567   # For each omeg
+00009110: 612c 2065 7661 6c75 6174 6520 4269 3a0a  a, evaluate Bi:.
+00009120: 2020 2020 2020 2020 706f 6f6c 203d 206d          pool = m
+00009130: 7470 436f 6e74 6578 742e 506f 6f6c 286e  tpContext.Pool(n
+00009140: 702e 6d69 6e69 6d75 6d28 6e75 6d5f 636f  p.minimum(num_co
+00009150: 7265 732c 6e5f 7065 616b 7329 290a 2020  res,n_peaks)).  
+00009160: 2020 2020 2020 7061 725f 7265 7375 6c74        par_result
+00009170: 203d 205b 706f 6f6c 2e61 7070 6c79 5f61   = [pool.apply_a
+00009180: 7379 6e63 2820 4269 6e6d 5265 7370 6f6e  sync( BinmRespon
+00009190: 7365 2c20 2872 5f62 6473 2c73 6967 6d61  se, (r_bds,sigma
+000091a0: 732c 7065 616b 5f6f 6d65 6761 735b 695f  s,peak_omegas[i_
+000091b0: 6f6d 5d2c 6173 796d 5f73 6861 7065 2c42  om],asym_shape,B
+000091c0: 656e 6d5b 695f 6f6d 2c2e 2e2e 5d2c 5869  enm[i_om,...],Xi
+000091d0: 642c 705f 6d61 782c 7273 6361 6c69 6e67  d,p_max,rscaling
+000091e0: 292c 2070 6172 5f6b 7720 2920 666f 7220  ), par_kw ) for 
+000091f0: 695f 6f6d 2069 6e20 7261 6e67 6528 6e5f  i_om in range(n_
+00009200: 7065 616b 7329 5d0a 2020 2020 2020 2020  peaks)].        
+00009210: 706f 6f6c 2e63 6c6f 7365 2829 0a20 2020  pool.close().   
+00009220: 2020 2020 2070 6f6f 6c2e 6a6f 696e 2829       pool.join()
+00009230: 0a0a 2020 2020 2020 2020 666f 7220 695f  ..        for i_
+00009240: 6f6d 2069 6e20 7261 6e67 6528 6e5f 7065  om in range(n_pe
+00009250: 616b 7329 3a0a 2020 2020 2020 2020 2020  aks):.          
+00009260: 2020 4269 6e6d 735b 695f 6f6d 2c20 2e2e    Binms[i_om, ..
+00009270: 2e5d 203d 2070 6172 5f72 6573 756c 745b  .] = par_result[
+00009280: 695f 6f6d 5d2e 6765 7428 290a 2020 2020  i_om].get().    
+00009290: 656c 7365 3a0a 2020 2020 2020 2020 6966  else:.        if
+000092a0: 2064 6562 7567 3a0a 2020 2020 2020 2020   debug:.        
+000092b0: 2020 2020 4165 732c 2041 7473 2c20 4164      Aes, Ats, Ad
+000092c0: 7320 3d20 5b20 6e70 2e7a 6572 6f73 2828  s = [ np.zeros((
+000092d0: 6e5f 7065 616b 732c 206e 7072 6d5f 6d61  n_peaks, nprm_ma
+000092e0: 782b 705f 6d61 7829 2c20 6474 7970 653d  x+p_max), dtype=
+000092f0: 6e70 2e63 6f6d 706c 6578 5f29 2066 6f72  np.complex_) for
+00009300: 205f 2069 6e20 7261 6e67 6528 3329 205d   _ in range(3) ]
+00009310: 0a20 2020 2020 2020 2020 2020 206b 7276  .            krv
+00009320: 616c 7320 3d20 6e70 2e7a 6572 6f73 286e  als = np.zeros(n
+00009330: 5f70 6561 6b73 2c20 6474 7970 653d 6e70  _peaks, dtype=np
+00009340: 2e63 6f6d 706c 6578 5f29 0a20 2020 2020  .complex_).     
+00009350: 2020 2020 2020 2066 6f72 2069 5f6f 6d20         for i_om 
+00009360: 696e 2072 616e 6765 286e 5f70 6561 6b73  in range(n_peaks
+00009370: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00009380: 2020 2042 696e 6d73 5b30 2c20 2e2e 2e5d     Binms[0, ...]
+00009390: 2c20 4165 735b 695f 6f6d 2c20 3a5d 2c20  , Aes[i_om, :], 
+000093a0: 4174 735b 695f 6f6d 2c20 3a5d 2c20 4164  Ats[i_om, :], Ad
+000093b0: 735b 695f 6f6d 2c20 3a5d 2c20 6b72 7661  s[i_om, :], krva
+000093c0: 6c73 5b69 5f6f 6d5d 203d 2042 696e 6d52  ls[i_om] = BinmR
+000093d0: 6573 706f 6e73 6528 725f 6264 732c 2073  esponse(r_bds, s
+000093e0: 6967 6d61 732c 2070 6561 6b5f 6f6d 6567  igmas, peak_omeg
+000093f0: 6173 5b69 5f6f 6d5d 2c20 6173 796d 5f73  as[i_om], asym_s
+00009400: 6861 7065 2c20 4265 6e6d 5b30 2c20 2e2e  hape, Benm[0, ..
+00009410: 2e5d 2c20 5869 642c 2070 5f6d 6178 2c20  .], Xid, p_max, 
+00009420: 7273 6361 6c69 6e67 2c20 6e70 726d 5f6d  rscaling, nprm_m
+00009430: 6178 3d6e 7072 6d5f 6d61 782c 2076 6572  ax=nprm_max, ver
+00009440: 626f 7365 3d76 6572 626f 7365 2c20 6465  bose=verbose, de
+00009450: 6275 673d 6465 6275 6729 0a20 2020 2020  bug=debug).     
+00009460: 2020 2020 2020 2020 2020 2069 6620 2869             if (i
+00009470: 5f6f 6d2b 3129 2025 2031 3020 3d3d 2030  _om+1) % 10 == 0
+00009480: 3a20 6c6f 672e 6465 6275 6728 6622 7b69  : log.debug(f"{i
+00009490: 5f6f 6d20 2b20 317d 206f 6620 7b6e 5f70  _om + 1} of {n_p
+000094a0: 6561 6b73 7d20 636f 6d70 6c65 7465 2e22  eaks} complete."
+000094b0: 290a 2020 2020 2020 2020 656c 7365 3a0a  ).        else:.
+000094c0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+000094d0: 695f 6f6d 2069 6e20 7261 6e67 6528 6e5f  i_om in range(n_
+000094e0: 7065 616b 7329 3a0a 2020 2020 2020 2020  peaks):.        
+000094f0: 2020 2020 2020 2020 4269 6e6d 735b 695f          Binms[i_
+00009500: 6f6d 2c20 2e2e 2e5d 203d 2042 696e 6d52  om, ...] = BinmR
+00009510: 6573 706f 6e73 6528 725f 6264 732c 2073  esponse(r_bds, s
+00009520: 6967 6d61 732c 2070 6561 6b5f 6f6d 6567  igmas, peak_omeg
+00009530: 6173 5b69 5f6f 6d5d 2c20 6173 796d 5f73  as[i_om], asym_s
+00009540: 6861 7065 2c20 4265 6e6d 5b69 5f6f 6d2c  hape, Benm[i_om,
+00009550: 202e 2e2e 5d2c 2058 6964 2c20 705f 6d61   ...], Xid, p_ma
+00009560: 782c 2072 7363 616c 696e 672c 206e 7072  x, rscaling, npr
+00009570: 6d5f 6d61 783d 6e70 726d 5f6d 6178 2c20  m_max=nprm_max, 
+00009580: 7665 7262 6f73 653d 7665 7262 6f73 6529  verbose=verbose)
+00009590: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000095a0: 206c 6f67 2e64 6562 7567 2866 227b 695f   log.debug(f"{i_
+000095b0: 6f6d 202b 2031 7d20 6f66 207b 6e5f 7065  om + 1} of {n_pe
+000095c0: 616b 737d 2063 6f6d 706c 6574 652e 2229  aks} complete.")
+000095d0: 0a0a 2020 2020 6966 2077 7269 7465 6f75  ..    if writeou
+000095e0: 743a 0a20 2020 2020 2020 2069 6620 7061  t:.        if pa
+000095f0: 7468 2069 7320 4e6f 6e65 3a0a 2020 2020  th is None:.    
+00009600: 2020 2020 2020 2020 7061 7468 203d 205f          path = _
+00009610: 696e 6475 6365 640a 2020 2020 2020 2020  induced.        
+00009620: 6966 206f 7574 466e 616d 6520 6973 204e  if outFname is N
+00009630: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00009640: 206f 7574 466e 616d 6520 3d20 6627 7b62   outFname = f'{b
+00009650: 666e 616d 657d 4269 6e6d 5f61 7379 6d7b  fname}Binm_asym{
+00009660: 6170 7065 6e64 7d27 0a20 2020 2020 2020  append}'.       
+00009670: 2066 7061 7468 203d 206f 732e 7061 7468   fpath = os.path
+00009680: 2e6a 6f69 6e28 7061 7468 2c20 6622 7b6f  .join(path, f"{o
+00009690: 7574 466e 616d 657d 2e64 6174 2229 0a20  utFname}.dat"). 
+000096a0: 2020 2020 2020 2066 6f75 7420 3d20 6f70         fout = op
+000096b0: 656e 2866 7061 7468 2c20 2277 2229 0a20  en(fpath, "w"). 
+000096c0: 2020 2020 2020 2068 6561 6465 7220 3d20         header = 
+000096d0: 227b 3a3c 3133 7d2c 207b 3a3c 347d 2c20  "{:<13}, {:<4}, 
+000096e0: 7b3a 3c34 7d2c 207b 3a3c 3234 7d2c 207b  {:<4}, {:<24}, {
+000096f0: 3a3c 3234 7d5c 6e22 2e66 6f72 6d61 7428  :<24}\n".format(
+00009700: 2250 6572 696f 6420 2868 7229 2022 2c20  "Period (hr) ", 
+00009710: 226e 2022 2c20 226d 2022 2c20 2242 696e  "n ", "m ", "Bin
+00009720: 6d5f 5265 2028 6e54 2922 2c20 2242 696e  m_Re (nT)", "Bin
+00009730: 6d5f 496d 2028 6e54 2922 290a 2020 2020  m_Im (nT)").    
+00009740: 2020 2020 666f 7574 2e77 7269 7465 2868      fout.write(h
+00009750: 6561 6465 7229 0a20 2020 2020 2020 2066  eader).        f
+00009760: 6f72 2069 2069 6e20 7261 6e67 6528 6e70  or i in range(np
+00009770: 2e73 697a 6528 7065 616b 5f6f 6d65 6761  .size(peak_omega
+00009780: 7329 293a 0a20 2020 2020 2020 2020 2020  s)):.           
+00009790: 2054 5f68 7273 203d 2032 2a6e 702e 7069   T_hrs = 2*np.pi
+000097a0: 2f70 6561 6b5f 6f6d 6567 6173 5b69 5d2f  /peak_omegas[i]/
+000097b0: 3336 3030 0a20 2020 2020 2020 2020 2020  3600.           
+000097c0: 2066 6f72 2069 5f6e 6d20 696e 2072 616e   for i_nm in ran
+000097d0: 6765 284e 6e6d 293a 0a20 2020 2020 2020  ge(Nnm):.       
+000097e0: 2020 2020 2020 2020 2073 6967 6e20 3d20           sign = 
+000097f0: 696e 7428 6d76 616c 735b 695f 6e6d 5d3c  int(mvals[i_nm]<
+00009800: 3029 0a20 2020 2020 2020 2020 2020 2020  0).             
+00009810: 2020 2074 6869 735f 4269 6e6d 203d 2042     this_Binm = B
+00009820: 696e 6d73 5b69 2c73 6967 6e2c 6e76 616c  inms[i,sign,nval
+00009830: 735b 695f 6e6d 5d2c 6162 7328 6d76 616c  s[i_nm],abs(mval
+00009840: 735b 695f 6e6d 5d29 5d0a 2020 2020 2020  s[i_nm])].      
+00009850: 2020 2020 2020 2020 2020 666f 7574 2e77            fout.w
+00009860: 7269 7465 2820 227b 3a3c 3133 7d2c 207b  rite( "{:<13}, {
+00009870: 3a3c 347d 2c20 7b3a 3c34 7d2c 207b 3a3c  :<4}, {:<4}, {:<
+00009880: 3234 7d2c 207b 3a3c 3234 7d5c 6e22 2e66  24}, {:<24}\n".f
+00009890: 6f72 6d61 7428 726f 756e 6428 545f 6872  ormat(round(T_hr
+000098a0: 732c 3529 2c20 6e76 616c 735b 695f 6e6d  s,5), nvals[i_nm
+000098b0: 5d2c 206d 7661 6c73 5b69 5f6e 6d5d 2c20  ], mvals[i_nm], 
+000098c0: 6e70 2e72 6561 6c28 7468 6973 5f42 696e  np.real(this_Bin
+000098d0: 6d29 2c20 6e70 2e69 6d61 6728 7468 6973  m), np.imag(this
+000098e0: 5f42 696e 6d29 2920 290a 2020 2020 2020  _Binm)) ).      
+000098f0: 2020 666f 7574 2e63 6c6f 7365 2829 0a20    fout.close(). 
+00009900: 2020 2020 2020 206c 6f67 2e69 6e66 6f28         log.info(
+00009910: 6622 4461 7461 2066 6f72 2061 7379 6d6d  f"Data for asymm
+00009920: 6574 7269 6320 4269 6e6d 2077 7269 7474  etric Binm writt
+00009930: 656e 2074 6f20 6669 6c65 3a20 7b66 7061  en to file: {fpa
+00009940: 7468 7d22 290a 0a20 2020 2020 2020 2069  th}")..        i
+00009950: 6620 5363 686d 6964 743a 0a20 2020 2020  f Schmidt:.     
+00009960: 2020 2020 2020 2069 6620 6f75 7446 6e61         if outFna
+00009970: 6d65 5320 6973 204e 6f6e 653a 0a20 2020  meS is None:.   
+00009980: 2020 2020 2020 2020 2020 2020 206f 7574               out
+00009990: 466e 616d 6553 203d 2066 277b 6266 6e61  FnameS = f'{bfna
+000099a0: 6d65 7d67 686e 6d5f 6173 796d 7b61 7070  me}ghnm_asym{app
+000099b0: 656e 647d 270a 2020 2020 2020 2020 2020  end}'.          
+000099c0: 2020 6670 6174 6820 3d20 6f73 2e70 6174    fpath = os.pat
+000099d0: 682e 6a6f 696e 2870 6174 682c 2066 227b  h.join(path, f"{
+000099e0: 6f75 7446 6e61 6d65 537d 2e64 6174 2229  outFnameS}.dat")
+000099f0: 0a20 2020 2020 2020 2020 2020 2066 6f75  .            fou
+00009a00: 7420 3d20 6f70 656e 2866 7061 7468 2c20  t = open(fpath, 
+00009a10: 2277 2229 0a20 2020 2020 2020 2020 2020  "w").           
+00009a20: 2068 6561 6465 7220 3d20 227b 3a3c 3133   header = "{:<13
+00009a30: 7d2c 207b 3a3c 347d 2c20 7b3a 3c34 7d2c  }, {:<4}, {:<4},
+00009a40: 207b 3a3c 3234 7d2c 207b 3a3c 3234 7d2c   {:<24}, {:<24},
+00009a50: 207b 3a3c 3234 7d2c 207b 3a3c 3234 7d5c   {:<24}, {:<24}\
+00009a60: 6e22 2e66 6f72 6d61 7428 2250 6572 696f  n".format("Perio
+00009a70: 6420 2868 7229 2022 2c20 226e 2022 2c20  d (hr) ", "n ", 
+00009a80: 226d 2022 2c20 2267 5f6e 6d5f 5265 2028  "m ", "g_nm_Re (
+00009a90: 6e54 2922 2c20 2267 5f6e 6d5f 496d 2028  nT)", "g_nm_Im (
+00009aa0: 6e54 2922 2c20 2268 5f6e 6d5f 5265 2028  nT)", "h_nm_Re (
+00009ab0: 6e54 2922 2c20 2268 5f6e 6d5f 496d 2028  nT)", "h_nm_Im (
+00009ac0: 6e54 2922 290a 2020 2020 2020 2020 2020  nT)").          
+00009ad0: 2020 666f 7574 2e77 7269 7465 2868 6561    fout.write(hea
+00009ae0: 6465 7229 0a20 2020 2020 2020 2020 2020  der).           
+00009af0: 2066 6f72 2069 2069 6e20 7261 6e67 6528   for i in range(
+00009b00: 6e70 2e73 697a 6528 7065 616b 5f6f 6d65  np.size(peak_ome
+00009b10: 6761 7329 293a 0a20 2020 2020 2020 2020  gas)):.         
+00009b20: 2020 2020 2020 2054 5f68 7273 203d 2032         T_hrs = 2
+00009b30: 2a6e 702e 7069 2f70 6561 6b5f 6f6d 6567  *np.pi/peak_omeg
+00009b40: 6173 5b69 5d2f 3336 3030 0a20 2020 2020  as[i]/3600.     
+00009b50: 2020 2020 2020 2020 2020 2074 6869 735f             this_
+00009b60: 676e 6d2c 2074 6869 735f 686e 6d20 3d20  gnm, this_hnm = 
+00009b70: 6765 745f 6768 5f66 726f 6d5f 4269 6e6d  get_gh_from_Binm
+00009b80: 286e 5f6d 6178 2c42 696e 6d73 5b69 2c2e  (n_max,Binms[i,.
+00009b90: 2e2e 5d29 0a20 2020 2020 2020 2020 2020  ..]).           
+00009ba0: 2020 2020 2066 6f72 206e 2069 6e20 7261       for n in ra
+00009bb0: 6e67 6528 312c 6e5f 6d61 782b 3129 3a0a  nge(1,n_max+1):.
+00009bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009bd0: 2020 2020 666f 7220 6d20 696e 2072 616e      for m in ran
+00009be0: 6765 286e 2b31 293a 0a20 2020 2020 2020  ge(n+1):.       
+00009bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009c00: 2066 6f75 742e 7772 6974 6528 2022 7b3a   fout.write( "{:
+00009c10: 3c31 337d 2c20 7b3a 3c34 7d2c 207b 3a3c  <13}, {:<4}, {:<
+00009c20: 347d 2c20 7b3a 3c32 347d 2c20 7b3a 3c32  4}, {:<24}, {:<2
+00009c30: 347d 2c20 7b3a 3c32 347d 2c20 7b3a 3c32  4}, {:<24}, {:<2
+00009c40: 347d 5c6e 222e 666f 726d 6174 2872 6f75  4}\n".format(rou
+00009c50: 6e64 2854 5f68 7273 2c35 292c 206e 2c20  nd(T_hrs,5), n, 
+00009c60: 6d2c 206e 702e 7265 616c 2874 6869 735f  m, np.real(this_
+00009c70: 676e 6d5b 6e2c 6d5d 292c 206e 702e 696d  gnm[n,m]), np.im
+00009c80: 6167 2874 6869 735f 676e 6d5b 6e2c 6d5d  ag(this_gnm[n,m]
+00009c90: 292c 206e 702e 7265 616c 2874 6869 735f  ), np.real(this_
+00009ca0: 686e 6d5b 6e2c 6d5d 292c 206e 702e 696d  hnm[n,m]), np.im
+00009cb0: 6167 2874 6869 735f 686e 6d5b 6e2c 6d5d  ag(this_hnm[n,m]
+00009cc0: 2929 2029 0a20 2020 2020 2020 2020 2020  )) ).           
+00009cd0: 2066 6f75 742e 636c 6f73 6528 290a 2020   fout.close().  
+00009ce0: 2020 2020 2020 2020 2020 6c6f 672e 696e            log.in
+00009cf0: 666f 2866 2244 6174 6120 666f 7220 6173  fo(f"Data for as
+00009d00: 796d 6d65 7472 6963 2c20 5363 686d 6964  ymmetric, Schmid
+00009d10: 7420 7365 6d69 2d6e 6f72 6d61 6c69 7a65  t semi-normalize
+00009d20: 6420 675f 6e6d 2061 6e64 2068 5f6e 6d20  d g_nm and h_nm 
+00009d30: 7772 6974 7465 6e20 746f 2066 696c 653a  written to file:
+00009d40: 207b 6670 6174 687d 2229 0a0a 2020 2020   {fpath}")..    
+00009d50: 6966 2064 6562 7567 3a0a 2020 2020 2020  if debug:.      
+00009d60: 2020 7265 7475 726e 2042 696e 6d73 2c20    return Binms, 
+00009d70: 4165 732c 2041 7473 2c20 4164 732c 206b  Aes, Ats, Ads, k
+00009d80: 7276 616c 730a 2020 2020 656c 7365 3a0a  rvals.    else:.
+00009d90: 2020 2020 2020 2020 7265 7475 726e 2042          return B
+00009da0: 696e 6d73 0a0a 2323 2323 2323 2323 2323  inms..##########
+00009db0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00009dc0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00009dd0: 2323 230a 0a22 2222 0a42 696e 6d52 6573  ###..""".BinmRes
+00009de0: 706f 6e73 6528 290a 2020 2020 5468 6520  ponse().    The 
+00009df0: 696e 6475 6365 6420 6d61 676e 6574 6963  induced magnetic
+00009e00: 206d 6f6d 656e 7473 2042 696e 6d20 666f   moments Binm fo
+00009e10: 7220 616c 6c20 696e 7075 7420 6465 6772  r all input degr
+00009e20: 6565 206e 2061 6e64 206f 7264 6572 206d  ee n and order m
+00009e30: 2c0a 2020 2020 7769 7468 2061 2073 7065  ,.    with a spe
+00009e40: 6369 6669 6564 2061 7379 6d6d 6574 7269  cified asymmetri
+00009e50: 6320 626f 756e 6461 7279 2073 6861 7065  c boundary shape
+00009e60: 2061 7379 6d5f 7368 6170 6520 616e 6420   asym_shape and 
+00009e70: 666f 7220 7468 6520 696e 7075 740a 2020  for the input.  
+00009e80: 2020 4265 6e6d 2061 7420 6120 7369 6e67    Benm at a sing
+00009e90: 6c65 2066 7265 7175 656e 6379 206f 6d65  le frequency ome
+00009ea0: 6761 2e0a 2020 2020 5573 6167 653a 2060  ga..    Usage: `
+00009eb0: 4269 6e6d 6020 3d20 4269 6e6d 5265 7370  Binm` = BinmResp
+00009ec0: 6f6e 7365 2860 725f 6264 7360 2c20 6073  onse(`r_bds`, `s
+00009ed0: 6967 6d61 7360 2c20 606f 6d65 6761 602c  igmas`, `omega`,
+00009ee0: 2060 6173 796d 5f73 6861 7065 602c 2060   `asym_shape`, `
+00009ef0: 4265 6e6d 602c 2060 5869 6460 2c20 6070  Benm`, `Xid`, `p
+00009f00: 5f6d 6178 602c 2060 7273 6361 6c69 6e67  _max`, `rscaling
+00009f10: 602c 2060 6e70 726d 5f6d 6178 3d31 602c  `, `nprm_max=1`,
+00009f20: 2060 7665 7262 6f73 653d 5472 7565 602c   `verbose=True`,
+00009f30: 2060 6465 6275 673d 4661 6c73 6560 290a   `debug=False`).
+00009f40: 2020 2020 5265 7475 726e 733a 0a20 2020      Returns:.   
+00009f50: 2020 2020 2042 696e 6d3a 2063 6f6d 706c       Binm: compl
+00009f60: 6578 2c20 7368 6170 6528 322c 6e5f 6d61  ex, shape(2,n_ma
+00009f70: 782b 312c 6e5f 6d61 782b 3129 2e20 5468  x+1,n_max+1). Th
+00009f80: 6520 636f 6d70 6c65 7820 696e 6475 6365  e complex induce
+00009f90: 6420 6d6f 6d65 6e74 7320 666f 7220 7468  d moments for th
+00009fa0: 6520 6769 7665 6e20 4265 6e6d 2061 6e64  e given Benm and
+00009fb0: 2061 7379 6d6d 6574 7269 6320 696e 7465   asymmetric inte
+00009fc0: 7269 6f72 2073 7472 7563 7475 7265 2c0a  rior structure,.
+00009fd0: 2020 2020 2020 2020 2020 2020 6576 616c              eval
+00009fe0: 7561 7465 6420 666f 7220 6120 7369 6e67  uated for a sing
+00009ff0: 6c65 2061 6e67 756c 6172 2066 7265 7175  le angular frequ
+0000a000: 656e 6379 206f 6620 6f73 6369 6c6c 6174  ency of oscillat
+0000a010: 696f 6e20 6f6d 6567 612e 0a20 2020 2050  ion omega..    P
+0000a020: 6172 616d 6574 6572 733a 0a20 2020 2020  arameters:.     
+0000a030: 2020 2072 5f62 6473 3a20 666c 6f61 742c     r_bds: float,
+0000a040: 2073 6861 7065 286e 5f62 6473 292e 2052   shape(n_bds). R
+0000a050: 6164 6969 2066 6f72 2065 6163 6820 626f  adii for each bo
+0000a060: 756e 6461 7279 2073 7572 6661 6365 2069  undary surface i
+0000a070: 6e20 6d2e 0a20 2020 2020 2020 2073 6967  n m..        sig
+0000a080: 6d61 733a 2066 6c6f 6174 2c20 7368 6170  mas: float, shap
+0000a090: 6528 6e5f 6264 7329 2e20 436f 6e64 7563  e(n_bds). Conduc
+0000a0a0: 7469 7669 7479 2066 6f72 2065 6163 6820  tivity for each 
+0000a0b0: 6c61 7965 7220 756e 6465 7220 7468 6520  layer under the 
+0000a0c0: 636f 7272 6573 706f 6e64 696e 6720 626f  corresponding bo
+0000a0d0: 756e 6461 7279 2069 6e20 532f 6d2e 0a20  undary in S/m.. 
+0000a0e0: 2020 2020 2020 206f 6d65 6761 3a20 666c         omega: fl
+0000a0f0: 6f61 742e 2041 6e67 756c 6172 2066 7265  oat. Angular fre
+0000a100: 7175 656e 6379 206f 6620 6d61 676e 6574  quency of magnet
+0000a110: 6963 206f 7363 696c 6c61 7469 6f6e 7320  ic oscillations 
+0000a120: 696e 2072 6164 2f73 2e0a 2020 2020 2020  in rad/s..      
+0000a130: 2020 6173 796d 5f73 6861 7065 3a20 636f    asym_shape: co
+0000a140: 6d70 6c65 782c 2073 6861 7065 286e 5f62  mplex, shape(n_b
+0000a150: 6473 2c32 2c70 5f6d 6178 2b31 2c70 5f6d  ds,2,p_max+1,p_m
+0000a160: 6178 2b31 292e 2041 206c 6973 7420 6f66  ax+1). A list of
+0000a170: 2062 6f75 6e64 6172 7920 7368 6170 6520   boundary shape 
+0000a180: 7061 7261 6d65 7465 7273 2063 6869 5f70  parameters chi_p
+0000a190: 7120 666f 7220 6561 6368 2062 6f75 6e64  q for each bound
+0000a1a0: 6172 792e 0a20 2020 2020 2020 2042 656e  ary..        Ben
+0000a1b0: 6d3a 2063 6f6d 706c 6578 2c20 7368 6170  m: complex, shap
+0000a1c0: 6528 322c 6e5f 6d61 782b 312c 6e5f 6d61  e(2,n_max+1,n_ma
+0000a1d0: 782b 3129 2e20 4578 6369 7461 7469 6f6e  x+1). Excitation
+0000a1e0: 206d 6f6d 656e 7473 2066 6f72 2065 6163   moments for eac
+0000a1f0: 6820 6e27 2061 6e64 206d 272c 2070 6164  h n' and m', pad
+0000a200: 6465 6420 7769 7468 207a 6572 6f73 2066  ded with zeros f
+0000a210: 6f72 206e 203e 206e 272e 0a20 2020 2020  or n > n'..     
+0000a220: 2020 2058 6964 3a20 6d70 662c 2073 6861     Xid: mpf, sha
+0000a230: 7065 2832 2c6e 7072 6d5f 6d61 782b 312c  pe(2,nprm_max+1,
+0000a240: 6e70 726d 5f6d 6178 2b31 2c20 322c 705f  nprm_max+1, 2,p_
+0000a250: 6d61 782b 312c 705f 6d61 782b 312c 2032  max+1,p_max+1, 2
+0000a260: 2c6e 5f6d 6178 2b31 2c6e 5f6d 6178 2b31  ,n_max+1,n_max+1
+0000a270: 292e 204d 6978 696e 6720 636f 6566 6669  ). Mixing coeffi
+0000a280: 6369 656e 7473 0a20 2020 2020 2020 2020  cients.         
+0000a290: 2020 2072 6573 756c 7469 6e67 2066 726f     resulting fro
+0000a2a0: 6d20 6d75 6c74 6970 6c69 6361 7469 6f6e  m multiplication
+0000a2b0: 206f 6620 7370 6865 7269 6361 6c20 6861   of spherical ha
+0000a2c0: 726d 6f6e 6963 732e 205c 5869 5e7b 5c73  rmonics. \Xi^{\s
+0000a2d0: 7461 7220 6e6d 7d5f 7b6e 276d 2770 717d  tar nm}_{n'm'pq}
+0000a2e0: 2066 726f 6d20 7468 6520 7061 7065 722e   from the paper.
+0000a2f0: 0a20 2020 2020 2020 2070 5f6d 6178 3a20  .        p_max: 
+0000a300: 696e 7465 6765 722e 204c 6172 6765 7374  integer. Largest
+0000a310: 2064 6567 7265 6520 7020 696e 2069 6e74   degree p in int
+0000a320: 6572 696f 7220 6d6f 6465 6c20 626f 756e  erior model boun
+0000a330: 6461 7279 2073 6861 7065 732e 0a20 2020  dary shapes..   
+0000a340: 2020 2020 2072 7363 616c 696e 673a 2066       rscaling: f
+0000a350: 6c6f 6174 2e20 5261 7469 6f20 6f66 206f  loat. Ratio of o
+0000a360: 7574 6572 6d6f 7374 2063 6f6e 6475 6374  utermost conduct
+0000a370: 696e 6720 626f 756e 6461 7279 2074 6f20  ing boundary to 
+0000a380: 626f 6479 2072 6164 6975 732e 0a20 2020  body radius..   
+0000a390: 2020 2020 206e 7072 6d5f 6d61 783a 2069       nprm_max: i
+0000a3a0: 6e74 6567 6572 2028 3129 2e20 4d61 7869  nteger (1). Maxi
+0000a3b0: 6d75 6d20 6465 6772 6565 206e 2720 6f66  mum degree n' of
+0000a3c0: 2042 656e 6d20 746f 2065 7661 6c75 6174   Benm to evaluat
+0000a3d0: 652e 206e 273d 3120 6973 2075 6e69 666f  e. n'=1 is unifo
+0000a3e0: 726d 2066 6965 6c64 2076 6563 746f 722e  rm field vector.
+0000a3f0: 0a20 2020 2020 2020 2076 6572 626f 7365  .        verbose
+0000a400: 3a20 626f 6f6c 6561 6e20 2854 7275 6529  : boolean (True)
+0000a410: 2e20 5768 6574 6865 7220 746f 2070 7269  . Whether to pri
+0000a420: 6e74 2070 726f 6772 6573 7320 7570 6461  nt progress upda
+0000a430: 7465 7320 746f 2074 6865 2074 6572 6d69  tes to the termi
+0000a440: 6e61 6c2e 0a20 2020 2020 2020 2064 6562  nal..        deb
+0000a450: 7567 3a20 626f 6f6c 6561 6e20 2846 616c  ug: boolean (Fal
+0000a460: 7365 292e 2053 7065 6369 616c 2075 7365  se). Special use
+0000a470: 2066 6c61 672e 0a20 2020 2022 2222 0a64   flag..    """.d
+0000a480: 6566 2042 696e 6d52 6573 706f 6e73 6528  ef BinmResponse(
+0000a490: 725f 6264 732c 2073 6967 6d61 732c 206f  r_bds, sigmas, o
+0000a4a0: 6d65 6761 2c20 6173 796d 5f73 6861 7065  mega, asym_shape
+0000a4b0: 2c20 4265 6e6d 2c20 5869 642c 2070 5f6d  , Benm, Xid, p_m
+0000a4c0: 6178 2c20 7273 6361 6c69 6e67 2c20 6e70  ax, rscaling, np
+0000a4d0: 726d 5f6d 6178 3d31 2c20 7665 7262 6f73  rm_max=1, verbos
+0000a4e0: 653d 5472 7565 2c20 6465 6275 673d 4661  e=True, debug=Fa
+0000a4f0: 6c73 6529 3a0a 2020 2020 6e5f 6d61 7820  lse):.    n_max 
+0000a500: 3d20 6e70 726d 5f6d 6178 202b 2070 5f6d  = nprm_max + p_m
+0000a510: 6178 0a20 2020 2042 696e 6d20 3d20 6e70  ax.    Binm = np
+0000a520: 2e7a 6572 6f73 2828 322c 206e 5f6d 6178  .zeros((2, n_max
+0000a530: 2b31 2c20 6e5f 6d61 782b 3129 2c20 6474  +1, n_max+1), dt
+0000a540: 7970 653d 6e70 2e63 6f6d 706c 6578 5f29  ype=np.complex_)
+0000a550: 0a20 2020 206e 5f62 6473 203d 206e 702e  .    n_bds = np.
+0000a560: 7369 7a65 2872 5f62 6473 290a 2020 2020  size(r_bds).    
+0000a570: 6e5f 696e 6e65 7220 3d20 6e5f 6264 7320  n_inner = n_bds 
+0000a580: 2d20 310a 0a20 2020 206e 695f 6264 7320  - 1..    ni_bds 
+0000a590: 3d20 6e5f 6264 7320 2d20 310a 2020 2020  = n_bds - 1.    
+0000a5a0: 6e69 5f69 6e6e 6572 203d 206e 5f69 6e6e  ni_inner = n_inn
+0000a5b0: 6572 202d 2031 0a20 2020 206c 6f6e 6520  er - 1.    lone 
+0000a5c0: 3d20 6f6e 650a 2020 2020 637a 6572 6f20  = one.    czero 
+0000a5d0: 3d20 6d70 2e6d 7063 2830 290a 0a20 2020  = mp.mpc(0)..   
+0000a5e0: 2023 2047 6574 2074 7970 6520 6f62 6a65   # Get type obje
+0000a5f0: 6374 2066 6f72 2069 6e69 7469 616c 697a  ct for initializ
+0000a600: 696e 6720 6e75 6d70 7920 6172 7261 7973  ing numpy arrays
+0000a610: 206f 6620 6d70 630a 2020 2020 6d70 6320   of mpc.    mpc 
+0000a620: 3d20 6d70 635f 676c 6f62 616c 0a0a 2020  = mpc_global..  
+0000a630: 2020 2320 436f 6e76 6572 7420 696e 7075    # Convert inpu
+0000a640: 7420 6461 7461 2066 6f72 206b 2076 616c  t data for k val
+0000a650: 7565 7320 696e 746f 206d 706d 6174 6820  ues into mpmath 
+0000a660: 666c 6f61 7473 0a20 2020 2023 2057 6865  floats.    # Whe
+0000a670: 6e20 7765 2077 6f6e 2774 206e 6565 6420  n we won't need 
+0000a680: 746f 2065 7870 6c69 6369 746c 7920 6c6f  to explicitly lo
+0000a690: 6f70 206f 7665 7220 696e 6469 6365 732c  op over indices,
+0000a6a0: 2075 7365 206e 756d 7079 0a20 2020 2023   use numpy.    #
+0000a6b0: 2061 7272 6179 7320 746f 2065 6e61 626c   arrays to enabl
+0000a6c0: 6520 7665 6374 6f72 697a 6564 2063 6f6d  e vectorized com
+0000a6d0: 7075 7461 7469 6f6e 2e0a 2020 2020 6e20  putation..    n 
+0000a6e0: 3d20 6e70 2e61 7272 6179 285b 206d 702e  = np.array([ mp.
+0000a6f0: 6d70 6628 6e69 2920 666f 7220 6e69 2069  mpf(ni) for ni i
+0000a700: 6e20 7261 6e67 6528 312c 6e5f 6d61 782b  n range(1,n_max+
+0000a710: 3129 205d 290a 2020 2020 6966 206e 6f74  1) ]).    if not
+0000a720: 2069 7369 6e73 7461 6e63 6528 725f 6264   isinstance(r_bd
+0000a730: 732c 2049 7465 7261 626c 6529 3a0a 2020  s, Iterable):.  
+0000a740: 2020 2020 2020 725f 6264 7320 3d20 5b6d        r_bds = [m
+0000a750: 702e 6d70 6628 725f 6264 7329 5d0a 2020  p.mpf(r_bds)].  
+0000a760: 2020 2020 2020 7369 676d 6173 203d 205b        sigmas = [
+0000a770: 6d70 2e6d 7066 2873 6967 6d61 7329 5d0a  mp.mpf(sigmas)].
+0000a780: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+0000a790: 2020 725f 6264 7320 3d20 5b6d 702e 6d70    r_bds = [mp.mp
+0000a7a0: 6628 725f 6929 2066 6f72 2072 5f69 2069  f(r_i) for r_i i
+0000a7b0: 6e20 725f 6264 735d 0a20 2020 2020 2020  n r_bds].       
+0000a7c0: 2073 6967 6d61 7320 3d20 5b6d 702e 6d70   sigmas = [mp.mp
+0000a7d0: 6628 7369 675f 6929 2066 6f72 2073 6967  f(sig_i) for sig
+0000a7e0: 5f69 2069 6e20 7369 676d 6173 5d0a 0a20  _i in sigmas].. 
+0000a7f0: 2020 2069 6620 6e6f 7420 6465 6275 673a     if not debug:
+0000a800: 0a20 2020 2020 2020 206f 6d65 6761 203d  .        omega =
+0000a810: 206d 702e 6d70 6628 6f6d 6567 6129 0a0a   mp.mpf(omega)..
+0000a820: 2020 2020 2020 2020 2320 4d61 6b65 206c          # Make l
+0000a830: 6973 7473 206f 6620 6b20 7661 6c75 6573  ists of k values
+0000a840: 0a20 2020 2020 2020 206b 725f 6c6c 203d  .        kr_ll =
+0000a850: 206e 702e 6172 7261 7928 5b20 6d70 2e73   np.array([ mp.s
+0000a860: 7172 7428 6a2a 6f6d 6567 612a 6d75 5f6f  qrt(j*omega*mu_o
+0000a870: 2a73 6967 6d61 735b 695f 6264 795d 292a  *sigmas[i_bdy])*
+0000a880: 725f 6264 735b 695f 6264 795d 2066 6f72  r_bds[i_bdy] for
+0000a890: 2069 5f62 6479 2069 6e20 7261 6e67 6528   i_bdy in range(
+0000a8a0: 6e5f 696e 6e65 7229 205d 290a 2020 2020  n_inner) ]).    
+0000a8b0: 2020 2020 6b72 5f75 6c20 3d20 6e70 2e61      kr_ul = np.a
+0000a8c0: 7272 6179 285b 206d 702e 7371 7274 286a  rray([ mp.sqrt(j
+0000a8d0: 2a6f 6d65 6761 2a6d 755f 6f2a 7369 676d  *omega*mu_o*sigm
+0000a8e0: 6173 5b69 5f62 6479 2b31 5d29 2a72 5f62  as[i_bdy+1])*r_b
+0000a8f0: 6473 5b69 5f62 6479 5d20 666f 7220 695f  ds[i_bdy] for i_
+0000a900: 6264 7920 696e 2072 616e 6765 286e 5f69  bdy in range(n_i
+0000a910: 6e6e 6572 2920 5d29 0a20 2020 2020 2020  nner) ]).       
+0000a920: 2023 206b 6120 7661 6c75 6520 6174 206f   # ka value at o
+0000a930: 7574 6572 2062 6f75 6e64 6172 790a 2020  uter boundary.  
+0000a940: 2020 2020 2020 6b72 5f65 7820 3d20 6d70        kr_ex = mp
+0000a950: 2e73 7172 7428 6a2a 6f6d 6567 612a 6d75  .sqrt(j*omega*mu
+0000a960: 5f6f 2a73 6967 6d61 735b 2d31 5d29 2a72  _o*sigmas[-1])*r
+0000a970: 5f62 6473 5b2d 315d 0a20 2020 2065 6c73  _bds[-1].    els
+0000a980: 653a 0a20 2020 2020 2020 206e 5f62 6473  e:.        n_bds
+0000a990: 203d 2031 0a20 2020 2020 2020 2023 2046   = 1.        # F
+0000a9a0: 6f72 2064 6562 7567 2070 7572 706f 7365  or debug purpose
+0000a9b0: 732c 206f 6d65 6761 2069 7320 7061 7373  s, omega is pass
+0000a9c0: 6564 2069 6e20 6173 2061 206b 7220 7661  ed in as a kr va
+0000a9d0: 6c75 650a 2020 2020 2020 2020 6b72 5f65  lue.        kr_e
+0000a9e0: 7820 3d20 6d70 2e73 7172 7428 6a29 202a  x = mp.sqrt(j) *
+0000a9f0: 206d 702e 6d70 6628 6f6d 6567 6129 0a0a   mp.mpf(omega)..
+0000aa00: 2020 2020 2320 496e 7365 7274 206b 7220      # Insert kr 
+0000aa10: 696e 746f 2042 6573 7365 6c20 6675 6e63  into Bessel func
+0000aa20: 7469 6f6e 7320 666f 7220 6f75 7465 7220  tions for outer 
+0000aa30: 6264 7920 6f6e 6c79 2066 6972 7374 0a20  bdy only first. 
+0000aa40: 2020 206a 6e5f 6578 203d 206e 702e 7a65     jn_ex = np.ze
+0000aa50: 726f 7328 6e5f 6d61 782c 2064 7479 7065  ros(n_max, dtype
+0000aa60: 3d6d 7063 290a 2020 2020 6a64 5f65 7820  =mpc).    jd_ex 
+0000aa70: 3d20 6e70 2e7a 6572 6f73 286e 5f6d 6178  = np.zeros(n_max
+0000aa80: 2c20 6474 7970 653d 6d70 6329 0a20 2020  , dtype=mpc).   
+0000aa90: 2079 6e5f 6578 203d 206e 702e 7a65 726f   yn_ex = np.zero
+0000aaa0: 7328 6e5f 6d61 782c 2064 7479 7065 3d6d  s(n_max, dtype=m
+0000aab0: 7063 290a 2020 2020 7964 5f65 7820 3d20  pc).    yd_ex = 
+0000aac0: 6e70 2e7a 6572 6f73 286e 5f6d 6178 2c20  np.zeros(n_max, 
+0000aad0: 6474 7970 653d 6d70 6329 0a20 2020 2066  dtype=mpc).    f
+0000aae0: 6f72 206e 6920 696e 2072 616e 6765 286e  or ni in range(n
+0000aaf0: 5f6d 6178 293a 0a20 2020 2020 2020 206a  _max):.        j
+0000ab00: 6e5f 6578 5b6e 695d 203d 206a 6e78 286e  n_ex[ni] = jnx(n
+0000ab10: 5b6e 695d 2c5b 6b72 5f65 785d 295b 305d  [ni],[kr_ex])[0]
+0000ab20: 0a20 2020 2020 2020 206a 645f 6578 5b6e  .        jd_ex[n
+0000ab30: 695d 203d 206a 6478 286e 5b6e 695d 2c5b  i] = jdx(n[ni],[
+0000ab40: 6b72 5f65 785d 295b 305d 0a20 2020 2020  kr_ex])[0].     
+0000ab50: 2020 2079 6e5f 6578 5b6e 695d 203d 2079     yn_ex[ni] = y
+0000ab60: 6e78 286e 5b6e 695d 2c5b 6b72 5f65 785d  nx(n[ni],[kr_ex]
+0000ab70: 295b 305d 0a20 2020 2020 2020 2079 645f  )[0].        yd_
+0000ab80: 6578 5b6e 695d 203d 2079 6478 286e 5b6e  ex[ni] = ydx(n[n
+0000ab90: 695d 2c5b 6b72 5f65 785d 295b 305d 0a0a  i],[kr_ex])[0]..
+0000aba0: 2020 2020 2320 4361 6c63 756c 6174 6520      # Calculate 
+0000abb0: 6f75 7465 7220 626f 756e 6461 7279 2074  outer boundary t
+0000abc0: 7261 6e73 6665 7220 7175 616e 7469 7469  ransfer quantiti
+0000abd0: 6573 2e0a 2020 2020 2320 416c 6c20 7375  es..    # All su
+0000abe0: 6368 2071 7561 6e74 6974 6965 7320 2868  ch quantities (h
+0000abf0: 6572 6520 616e 6420 6d6f 7265 2062 656c  ere and more bel
+0000ac00: 6f77 2920 6861 7665 2051 2061 7070 656e  ow) have Q appen
+0000ac10: 6465 642d 2d2d 7468 6520 2251 2072 6573  ded---the "Q res
+0000ac20: 706f 6e73 6522 2069 7320 616e 616c 6f67  ponse" is analog
+0000ac30: 6f75 7320 746f 205c 6d61 7468 6361 6c7b  ous to \mathcal{
+0000ac40: 417d 2e0a 2020 2020 616c 7068 5120 3d20  A}..    alphQ = 
+0000ac50: 312f 6b72 5f65 780a 2020 2020 6265 7461  1/kr_ex.    beta
+0000ac60: 5120 3d20 6a64 5f65 7820 2d20 286e 2b6f  Q = jd_ex - (n+o
+0000ac70: 6e65 292a 6a6e 5f65 780a 2020 2020 6761  ne)*jn_ex.    ga
+0000ac80: 6d6d 5120 3d20 7964 5f65 7820 2d20 286e  mmQ = yd_ex - (n
+0000ac90: 2b6f 6e65 292a 796e 5f65 780a 2020 2020  +one)*yn_ex.    
+0000aca0: 6465 6c74 5120 3d20 6e2a 6a6e 5f65 7820  deltQ = n*jn_ex 
+0000acb0: 2b20 6a64 5f65 780a 2020 2020 6570 7369  + jd_ex.    epsi
+0000acc0: 5120 3d20 6e2a 796e 5f65 7820 2b20 7964  Q = n*yn_ex + yd
+0000acd0: 5f65 780a 2020 2020 7869 5f5f 5120 3d20  _ex.    xi__Q = 
+0000ace0: 2d6b 725f 6578 2a2a 3220 2a20 6a6e 5f65  -kr_ex**2 * jn_e
+0000acf0: 785b 3a6e 7072 6d5f 6d61 785d 0a20 2020  x[:nprm_max].   
+0000ad00: 2072 686f 5f51 203d 202d 6b72 5f65 782a   rho_Q = -kr_ex*
+0000ad10: 2a32 202a 2079 6e5f 6578 5b3a 6e70 726d  *2 * yn_ex[:nprm
+0000ad20: 5f6d 6178 5d0a 2020 2020 7a65 7461 5120  _max].    zetaQ 
+0000ad30: 3d20 6e2a 6a6e 5f65 780a 2020 2020 6574  = n*jn_ex.    et
+0000ad40: 615f 5120 3d20 6e2a 796e 5f65 780a 0a20  a_Q = n*yn_ex.. 
+0000ad50: 2020 206c 6f67 2e64 6562 7567 2822 2020     log.debug("  
+0000ad60: 2020 496e 6974 6961 6c69 7a65 6420 7472    Initialized tr
+0000ad70: 616e 7366 6572 2063 616c 6375 6c61 7469  ansfer calculati
+0000ad80: 6f6e 732e 2e2e 2229 0a0a 2020 2020 2320  ons...")..    # 
+0000ad90: 4966 2074 6865 7265 2773 206f 6e6c 7920  If there's only 
+0000ada0: 6f6e 6520 626f 756e 6461 7279 2c20 6b72  one boundary, kr
+0000adb0: 5f6c 6c20 616e 6420 6b72 5f75 6c20 6172  _ll and kr_ul ar
+0000adc0: 6520 656d 7074 7920 616e 6420 7765 2063  e empty and we c
+0000add0: 616e 2069 6d6d 6564 6961 7465 6c79 2063  an immediately c
+0000ade0: 616c 6375 6c61 7465 2041 2066 756e 6374  alculate A funct
+0000adf0: 696f 6e20 7661 6c75 6573 2e0a 2020 2020  ion values..    
+0000ae00: 6966 206e 5f62 6473 203e 2031 3a0a 2020  if n_bds > 1:.  
+0000ae10: 2020 2020 2020 2320 496e 6974 6961 6c69        # Initiali
+0000ae20: 7a65 2042 6573 7365 6c20 6675 6e63 7469  ze Bessel functi
+0000ae30: 6f6e 2072 6573 756c 7473 0a20 2020 2020  on results.     
+0000ae40: 2020 206a 6e5f 6c6c 2c20 6a64 5f6c 6c2c     jn_ll, jd_ll,
+0000ae50: 2079 6e5f 6c6c 2c20 7964 5f6c 6c20 3d20   yn_ll, yd_ll = 
+0000ae60: 2820 6e70 2e7a 6572 6f73 2828 6e5f 6d61  ( np.zeros((n_ma
+0000ae70: 782c 6e5f 696e 6e65 7229 2c20 6474 7970  x,n_inner), dtyp
+0000ae80: 653d 6d70 6329 2066 6f72 205f 2069 6e20  e=mpc) for _ in 
+0000ae90: 7261 6e67 6528 3429 2029 0a20 2020 2020  range(4) ).     
+0000aea0: 2020 206a 6e5f 756c 2c20 6a64 5f75 6c2c     jn_ul, jd_ul,
+0000aeb0: 2079 6e5f 756c 2c20 7964 5f75 6c20 3d20   yn_ul, yd_ul = 
+0000aec0: 2820 6e70 2e7a 6572 6f73 2828 6e5f 6d61  ( np.zeros((n_ma
+0000aed0: 782c 6e5f 696e 6e65 7229 2c20 6474 7970  x,n_inner), dtyp
+0000aee0: 653d 6d70 6329 2066 6f72 205f 2069 6e20  e=mpc) for _ in 
+0000aef0: 7261 6e67 6528 3429 2029 0a0a 2020 2020  range(4) )..    
+0000af00: 2020 2020 2320 436f 6e74 696e 7565 2069      # Continue i
+0000af10: 6e73 6572 7469 6e67 206b 7220 696e 746f  nserting kr into
+0000af20: 2042 6573 7365 6c20 6675 6e63 7469 6f6e   Bessel function
+0000af30: 730a 2020 2020 2020 2020 666f 7220 6e69  s.        for ni
+0000af40: 2069 6e20 7261 6e67 6528 6e5f 6d61 7829   in range(n_max)
+0000af50: 3a0a 2020 2020 2020 2020 2020 2020 6a6e  :.            jn
+0000af60: 5f6c 6c5b 6e69 2c3a 5d20 3d20 6a6e 7828  _ll[ni,:] = jnx(
+0000af70: 6e5b 6e69 5d2c 6b72 5f6c 6c29 0a20 2020  n[ni],kr_ll).   
+0000af80: 2020 2020 2020 2020 206a 645f 6c6c 5b6e           jd_ll[n
+0000af90: 692c 3a5d 203d 206a 6478 286e 5b6e 695d  i,:] = jdx(n[ni]
+0000afa0: 2c6b 725f 6c6c 290a 2020 2020 2020 2020  ,kr_ll).        
+0000afb0: 2020 2020 796e 5f6c 6c5b 6e69 2c3a 5d20      yn_ll[ni,:] 
+0000afc0: 3d20 796e 7828 6e5b 6e69 5d2c 6b72 5f6c  = ynx(n[ni],kr_l
+0000afd0: 6c29 0a20 2020 2020 2020 2020 2020 2079  l).            y
+0000afe0: 645f 6c6c 5b6e 692c 3a5d 203d 2079 6478  d_ll[ni,:] = ydx
+0000aff0: 286e 5b6e 695d 2c6b 725f 6c6c 290a 0a20  (n[ni],kr_ll).. 
+0000b000: 2020 2020 2020 2020 2020 206a 6e5f 756c             jn_ul
+0000b010: 5b6e 692c 3a5d 203d 206a 6e78 286e 5b6e  [ni,:] = jnx(n[n
+0000b020: 695d 2c6b 725f 756c 290a 2020 2020 2020  i],kr_ul).      
+0000b030: 2020 2020 2020 6a64 5f75 6c5b 6e69 2c3a        jd_ul[ni,:
+0000b040: 5d20 3d20 6a64 7828 6e5b 6e69 5d2c 6b72  ] = jdx(n[ni],kr
+0000b050: 5f75 6c29 0a20 2020 2020 2020 2020 2020  _ul).           
+0000b060: 2079 6e5f 756c 5b6e 692c 3a5d 203d 2079   yn_ul[ni,:] = y
+0000b070: 6e78 286e 5b6e 695d 2c6b 725f 756c 290a  nx(n[ni],kr_ul).
+0000b080: 2020 2020 2020 2020 2020 2020 7964 5f75              yd_u
+0000b090: 6c5b 6e69 2c3a 5d20 3d20 7964 7828 6e5b  l[ni,:] = ydx(n[
+0000b0a0: 6e69 5d2c 6b72 5f75 6c29 0a0a 2020 2020  ni],kr_ul)..    
+0000b0b0: 2020 2020 2320 4361 6c63 756c 6174 6520      # Calculate 
+0000b0c0: 6c61 7965 7220 7472 616e 7366 6572 2071  layer transfer q
+0000b0d0: 7561 6e74 6974 6965 730a 2020 2020 2020  uantities.      
+0000b0e0: 2020 616c 7068 203d 206e 702e 7a65 726f    alph = np.zero
+0000b0f0: 7328 286e 5f6d 6178 2c6e 5f69 6e6e 6572  s((n_max,n_inner
+0000b100: 292c 2064 7479 7065 3d6d 7063 290a 2020  ), dtype=mpc).  
+0000b110: 2020 2020 2020 616c 7068 5b3a 2c3a 2d31        alph[:,:-1
+0000b120: 5d20 3d20 6a6e 5f6c 6c5b 3a2c 313a 5d2a  ] = jn_ll[:,1:]*
+0000b130: 7964 5f6c 6c5b 3a2c 313a 5d20 2d20 6a64  yd_ll[:,1:] - jd
+0000b140: 5f6c 6c5b 3a2c 313a 5d2a 796e 5f6c 6c5b  _ll[:,1:]*yn_ll[
+0000b150: 3a2c 313a 5d0a 2020 2020 2020 2020 616c  :,1:].        al
+0000b160: 7068 5b3a 2c2d 315d 203d 206a 6e5f 6578  ph[:,-1] = jn_ex
+0000b170: 2a79 645f 6578 202d 206a 645f 6578 2a79  *yd_ex - jd_ex*y
+0000b180: 6e5f 6578 0a20 2020 2020 2020 2062 6574  n_ex.        bet
+0000b190: 6120 3d20 6a6e 5f6c 6c2a 7964 5f75 6c20  a = jn_ll*yd_ul 
+0000b1a0: 2d20 796e 5f75 6c2a 6a64 5f6c 6c0a 2020  - yn_ul*jd_ll.  
+0000b1b0: 2020 2020 2020 6761 6d6d 203d 2079 6e5f        gamm = yn_
+0000b1c0: 6c6c 2a79 645f 756c 202d 2079 6e5f 756c  ll*yd_ul - yn_ul
+0000b1d0: 2a79 645f 6c6c 0a20 2020 2020 2020 2064  *yd_ll.        d
+0000b1e0: 656c 7420 3d20 6a6e 5f75 6c2a 6a64 5f6c  elt = jn_ul*jd_l
+0000b1f0: 6c20 2d20 6a6e 5f6c 6c2a 6a64 5f75 6c0a  l - jn_ll*jd_ul.
+0000b200: 2020 2020 2020 2020 6570 7369 203d 206a          epsi = j
+0000b210: 6e5f 756c 2a79 645f 6c6c 202d 2079 6e5f  n_ul*yd_ll - yn_
+0000b220: 6c6c 2a6a 645f 756c 0a0a 2020 2020 2020  ll*jd_ul..      
+0000b230: 2020 2320 4d61 6b65 2074 6865 2073 7068    # Make the sph
+0000b240: 6572 6963 616c 6c79 2073 796d 6d65 7472  erically symmetr
+0000b250: 6963 2072 6563 7572 7369 6f6e 3a0a 2020  ic recursion:.  
+0000b260: 2020 2020 2020 4c61 6d62 6420 3d20 6576        Lambd = ev
+0000b270: 616c 5f69 6e6e 6572 5f72 6563 7572 5f73  al_inner_recur_s
+0000b280: 796d 286e 5f6d 6178 2c20 6e5f 6264 732c  ym(n_max, n_bds,
+0000b290: 2062 6574 612c 2067 616d 6d2c 2064 656c   beta, gamm, del
+0000b2a0: 742c 2065 7073 6929 0a0a 2020 2020 2020  t, epsi)..      
+0000b2b0: 2020 2320 4576 616c 7561 7465 2074 6572    # Evaluate ter
+0000b2c0: 6d73 2066 6f72 2074 6865 206c 6179 6572  ms for the layer
+0000b2d0: 2073 6572 6965 733a 0a20 2020 2020 2020   series:.       
+0000b2e0: 2054 7261 6e73 6665 7251 7473 3120 3d20   TransferQts1 = 
+0000b2f0: 286a 6e5f 6c6c 2c20 796e 5f6c 6c2c 206a  (jn_ll, yn_ll, j
+0000b300: 6e5f 756c 2c20 796e 5f75 6c2c 206a 645f  n_ul, yn_ul, jd_
+0000b310: 6c6c 2c20 7964 5f6c 6c2c 206b 725f 6578  ll, yd_ll, kr_ex
+0000b320: 2c20 6a6e 5f65 782c 2079 6e5f 6578 2c20  , jn_ex, yn_ex, 
+0000b330: 616c 7068 2c20 6265 7461 2c20 6761 6d6d  alph, beta, gamm
+0000b340: 2c20 6465 6c74 2c20 6570 7369 2c20 6465  , delt, epsi, de
+0000b350: 6c74 512c 2065 7073 6951 2c20 4c61 6d62  ltQ, epsiQ, Lamb
+0000b360: 6429 0a20 2020 2020 2020 2041 742c 204b  d).        At, K
+0000b370: 6e2c 2061 4261 7220 3d20 6765 745f 7365  n, aBar = get_se
+0000b380: 7269 6573 5f74 6572 6d73 286e 5f6d 6178  ries_terms(n_max
+0000b390: 2c20 6e70 726d 5f6d 6178 2c20 6e2c 206e  , nprm_max, n, n
+0000b3a0: 5f62 6473 2c20 5472 616e 7366 6572 5174  _bds, TransferQt
+0000b3b0: 7331 2c20 725f 6264 735b 2d31 5d2c 2042  s1, r_bds[-1], B
+0000b3c0: 656e 6d29 0a0a 2020 2020 2020 2020 5472  enm)..        Tr
+0000b3d0: 616e 7366 6572 5174 7332 203d 2028 6b72  ansferQts2 = (kr
+0000b3e0: 5f6c 6c2c 206b 725f 756c 2c20 6a6e 5f6c  _ll, kr_ul, jn_l
+0000b3f0: 6c2c 2079 6e5f 6c6c 2c20 4c61 6d62 6429  l, yn_ll, Lambd)
+0000b400: 0a0a 2020 2020 656c 7365 3a0a 2020 2020  ..    else:.    
+0000b410: 2020 2020 4c61 6d62 6420 3d20 6e70 2e7a      Lambd = np.z
+0000b420: 6572 6f73 2828 6e5f 6d61 782c 3129 2c20  eros((n_max,1), 
+0000b430: 6474 7970 653d 6d70 6329 0a20 2020 2020  dtype=mpc).     
+0000b440: 2020 2041 7420 3d20 6e70 2e7a 6572 6f73     At = np.zeros
+0000b450: 2828 6e5f 6d61 782c 3129 2c20 6474 7970  ((n_max,1), dtyp
+0000b460: 653d 6d70 6329 0a20 2020 2020 2020 204b  e=mpc).        K
+0000b470: 6e20 3d20 6e70 2e6f 6e65 7328 286e 5f6d  n = np.ones((n_m
+0000b480: 6178 2c31 292c 2064 7479 7065 3d6d 7063  ax,1), dtype=mpc
+0000b490: 290a 2020 2020 2020 2020 6142 6172 203d  ).        aBar =
+0000b4a0: 206e 702e 7a65 726f 7328 2832 2c6e 7072   np.zeros((2,npr
+0000b4b0: 6d5f 6d61 782b 312c 6e70 726d 5f6d 6178  m_max+1,nprm_max
+0000b4c0: 2b31 2c31 292c 2064 7479 7065 3d6d 7063  +1,1), dtype=mpc
+0000b4d0: 2920 2023 2054 6869 7320 7769 6c6c 206e  )  # This will n
+0000b4e0: 6f74 2062 6520 7573 6564 0a20 2020 2020  ot be used.     
+0000b4f0: 2020 2041 745b 3a2c 305d 203d 206a 6e5f     At[:,0] = jn_
+0000b500: 6578 2f64 656c 7451 0a20 2020 2020 2020  ex/deltQ.       
+0000b510: 2054 7261 6e73 6665 7251 7473 3220 3d20   TransferQts2 = 
+0000b520: 286b 725f 6578 2c20 6b72 5f65 782c 206a  (kr_ex, kr_ex, j
+0000b530: 6e5f 6578 2c20 796e 5f65 782c 204c 616d  n_ex, yn_ex, Lam
+0000b540: 6264 2920 2023 2054 6865 7365 2077 696c  bd)  # These wil
+0000b550: 6c20 6e6f 7420 6265 2075 7365 640a 0a20  l not be used.. 
+0000b560: 2020 2041 6420 3d20 2878 695f 5f51 202b     Ad = (xi__Q +
+0000b570: 204c 616d 6264 5b3a 6e70 726d 5f6d 6178   Lambd[:nprm_max
+0000b580: 2c6e 695f 6264 735d 2a72 686f 5f51 2920  ,ni_bds]*rho_Q) 
+0000b590: 2f20 2864 656c 7451 5b3a 6e70 726d 5f6d  / (deltQ[:nprm_m
+0000b5a0: 6178 5d20 2b20 4c61 6d62 645b 3a6e 7072  ax] + Lambd[:npr
+0000b5b0: 6d5f 6d61 782c 6e69 5f62 6473 5d2a 6570  m_max,ni_bds]*ep
+0000b5c0: 7369 515b 3a6e 7072 6d5f 6d61 785d 290a  siQ[:nprm_max]).
+0000b5d0: 0a20 2020 206c 6f67 2e64 6562 7567 2822  .    log.debug("
+0000b5e0: 2020 2020 4361 6c63 756c 6174 696e 6720      Calculating 
+0000b5f0: 7365 7269 6573 2072 6573 756c 7473 2e2e  series results..
+0000b600: 2e22 290a 0a20 2020 2023 2046 696e 616c  .")..    # Final
+0000b610: 6c79 2c20 6576 616c 7561 7465 2074 6865  ly, evaluate the
+0000b620: 2061 7379 6d6d 6574 7279 2073 6572 6965   asymmetry serie
+0000b630: 7320 7465 726d 733a 0a20 2020 2044 656c  s terms:.    Del
+0000b640: 7461 203d 2067 6574 5f44 656c 7461 6e6d  ta = get_Deltanm
+0000b650: 6928 6e5f 6d61 782c 2070 5f6d 6178 2c20  i(n_max, p_max, 
+0000b660: 6e70 726d 5f6d 6178 2c20 6e2c 206e 5f62  nprm_max, n, n_b
+0000b670: 6473 2c20 725f 6264 732c 2042 656e 6d2c  ds, r_bds, Benm,
+0000b680: 2061 7379 6d5f 7368 6170 652c 2058 6964   asym_shape, Xid
+0000b690: 2c20 6142 6172 2c20 4164 2c20 5472 616e  , aBar, Ad, Tran
+0000b6a0: 7366 6572 5174 7332 290a 0a20 2020 2023  sferQts2)..    #
+0000b6b0: 2041 6e64 2074 6865 2073 6572 6965 7320   And the series 
+0000b6c0: 6974 7365 6c66 3a0a 2020 2020 414b 4473  itself:.    AKDs
+0000b6d0: 6572 6965 7320 3d20 6e70 2e7a 6572 6f73  eries = np.zeros
+0000b6e0: 2828 322c 6e5f 6d61 782b 312c 6e5f 6d61  ((2,n_max+1,n_ma
+0000b6f0: 782b 3129 2c20 6474 7970 653d 6d70 6329  x+1), dtype=mpc)
+0000b700: 0a20 2020 2066 6f72 2069 2069 6e20 7261  .    for i in ra
+0000b710: 6e67 6528 6e5f 6264 7329 3a0a 2020 2020  nge(n_bds):.    
+0000b720: 2020 2020 666f 7220 6e6e 2069 6e20 7261      for nn in ra
+0000b730: 6e67 6528 312c 6e5f 6d61 782b 3129 3a0a  nge(1,n_max+1):.
+0000b740: 2020 2020 2020 2020 2020 2020 6e69 203d              ni =
+0000b750: 206e 6e20 2d20 310a 2020 2020 2020 2020   nn - 1.        
+0000b760: 2020 2020 414b 4473 6572 6965 735b 3a2c      AKDseries[:,
+0000b770: 6e6e 2c3a 5d20 2b3d 2041 745b 6e69 2c69  nn,:] += At[ni,i
+0000b780: 5d20 2a20 4b6e 5b6e 692c 695d 202a 2044  ] * Kn[ni,i] * D
+0000b790: 656c 7461 5b3a 2c6e 6e2c 3a2c 695d 0a0a  elta[:,nn,:,i]..
+0000b7a0: 2020 2020 6966 2076 6572 626f 7365 3a0a      if verbose:.
+0000b7b0: 2020 2020 2020 2020 545f 6872 7320 3d20          T_hrs = 
+0000b7c0: 726f 756e 6428 322a 6e70 2e70 692f 6f6d  round(2*np.pi/om
+0000b7d0: 6567 612f 3336 3030 2c20 3229 0a20 2020  ega/3600, 2).   
+0000b7e0: 2020 2020 206c 6f67 2e64 6562 7567 2866       log.debug(f
+0000b7f0: 2220 2020 2045 7661 6c75 6174 696e 6720  "    Evaluating 
+0000b800: 6669 6e61 6c20 7072 6f64 7563 7473 2066  final products f
+0000b810: 6f72 2054 203d 207b 545f 6872 737d 2e2e  or T = {T_hrs}..
+0000b820: 2e22 290a 0a20 2020 2023 2046 696e 616c  .")..    # Final
+0000b830: 6c79 2c20 7a69 7020 6974 2061 6c6c 2074  ly, zip it all t
+0000b840: 6f67 6574 6865 723a 0a20 2020 2041 6520  ogether:.    Ae 
+0000b850: 3d20 6370 785f 6469 7628 2028 6265 7461  = cpx_div( (beta
+0000b860: 5120 2b20 4c61 6d62 645b 3a2c 2d31 5d20  Q + Lambd[:,-1] 
+0000b870: 2a20 6761 6d6d 5129 2c20 2864 656c 7451  * gammQ), (deltQ
+0000b880: 202b 204c 616d 6264 5b3a 2c2d 315d 202a   + Lambd[:,-1] *
+0000b890: 2065 7073 6951 2920 290a 2020 2020 666f   epsiQ) ).    fo
+0000b8a0: 7220 6e6e 2069 6e20 7261 6e67 6528 312c  r nn in range(1,
+0000b8b0: 6e5f 6d61 782b 3129 3a0a 2020 2020 2020  n_max+1):.      
+0000b8c0: 2020 6e69 203d 206e 6e20 2d20 310a 2020    ni = nn - 1.  
+0000b8d0: 2020 2020 2020 6e76 203d 206e 5b6e 695d        nv = n[ni]
+0000b8e0: 0a20 2020 2020 2020 2042 696e 6d5b 3a2c  .        Binm[:,
+0000b8f0: 6e6e 2c3a 5d20 3d20 286e 762f 286e 762b  nn,:] = (nv/(nv+
+0000b900: 6c6f 6e65 2920 2a20 4165 5b6e 695d 2a42  lone) * Ae[ni]*B
+0000b910: 656e 6d5b 3a2c 6e6e 2c3a 5d20 2b20 6e76  enm[:,nn,:] + nv
+0000b920: 2a41 4b44 7365 7269 6573 5b3a 2c6e 6e2c  *AKDseries[:,nn,
+0000b930: 3a5d 2920 2a20 7273 6361 6c69 6e67 2a2a  :]) * rscaling**
+0000b940: 286e 6e2b 3229 0a0a 2020 2020 6966 2064  (nn+2)..    if d
+0000b950: 6562 7567 3a0a 2020 2020 2020 2020 7265  ebug:.        re
+0000b960: 7475 726e 2042 696e 6d2c 2041 652c 2041  turn Binm, Ae, A
+0000b970: 742c 2041 642c 206b 725f 6578 0a20 2020  t, Ad, kr_ex.   
+0000b980: 2065 6c73 653a 0a20 2020 2020 2020 2072   else:.        r
+0000b990: 6574 7572 6e20 4269 6e6d 0a0a 2323 2323  eturn Binm..####
+0000b9a0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0000b9b0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0000b9c0: 2323 2323 2323 2323 230a 0a22 2222 0a67  #########..""".g
+0000b9d0: 6574 5f73 6572 6965 735f 7465 726d 7328  et_series_terms(
+0000b9e0: 290a 2020 2020 4361 6c63 756c 6174 6520  ).    Calculate 
+0000b9f0: 7175 616e 7469 7469 6573 2074 6861 7420  quantities that 
+0000ba00: 6170 7065 6172 2069 6e20 7375 6d73 206f  appear in sums o
+0000ba10: 7665 7220 6c61 7965 7273 2e0a 2020 2020  ver layers..    
+0000ba20: 5573 6167 653a 2060 4174 602c 2060 4b6e  Usage: `At`, `Kn
+0000ba30: 602c 2060 6142 6172 6020 3d20 6765 745f  `, `aBar` = get_
+0000ba40: 7365 7269 6573 5f74 6572 6d73 2860 6e5f  series_terms(`n_
+0000ba50: 6d61 7860 2c20 606e 7072 6d5f 6d61 7860  max`, `nprm_max`
+0000ba60: 2c20 606e 602c 2060 6e5f 6264 7360 2c20  , `n`, `n_bds`, 
+0000ba70: 6054 7261 6e73 6665 7251 7473 602c 2060  `TransferQts`, `
+0000ba80: 5260 2c20 6042 656e 6d60 290a 2020 2020  R`, `Benm`).    
+0000ba90: 5265 7475 726e 733a 0a20 2020 2020 2020  Returns:.       
+0000baa0: 2041 743a 206d 7063 2c20 7368 6170 6528   At: mpc, shape(
+0000bab0: 6e5f 6d61 782c 6e5f 6264 7329 2e20 5363  n_max,n_bds). Sc
+0000bac0: 616c 696e 6720 616d 706c 6974 7564 6520  aling amplitude 
+0000bad0: 6465 7465 726d 696e 696e 6720 7468 6520  determining the 
+0000bae0: 7374 7265 6e67 7468 206f 6620 696e 6475  strength of indu
+0000baf0: 6365 6420 6669 656c 6420 6672 6f6d 2065  ced field from e
+0000bb00: 6163 6820 6c61 7965 722e 0a20 2020 2020  ach layer..     
+0000bb10: 2020 2020 2020 2054 6869 7320 6973 205c         This is \
+0000bb20: 6d61 7468 6361 6c7b 417d 5f6e 5e7b 742c  mathcal{A}_n^{t,
+0000bb30: 697d 2069 6e20 7468 6520 7061 7065 722e  i} in the paper.
+0000bb40: 0a20 2020 2020 2020 204b 6e3a 206d 7063  .        Kn: mpc
+0000bb50: 2c20 7368 6170 6528 6e5f 6d61 782c 6e5f  , shape(n_max,n_
+0000bb60: 6264 7329 2e20 5472 616e 7366 6572 2070  bds). Transfer p
+0000bb70: 726f 6475 6374 2070 726f 7061 6761 7469  roduct propagati
+0000bb80: 6e67 2069 6e64 7563 6564 206d 6f6d 656e  ng induced momen
+0000bb90: 7473 2072 6573 756c 7469 6e67 0a20 2020  ts resulting.   
+0000bba0: 2020 2020 2020 2020 2066 726f 6d20 6173           from as
+0000bbb0: 796d 6d65 7472 7920 6672 6f6d 2074 6865  ymmetry from the
+0000bbc0: 2061 7379 6d6d 6574 7269 6320 6c61 7965   asymmetric laye
+0000bbd0: 7220 746f 2074 6865 206f 7574 6572 6d6f  r to the outermo
+0000bbe0: 7374 2062 6f75 6e64 6172 792e 2054 6869  st boundary. Thi
+0000bbf0: 7320 6973 204b 5f6e 5e69 2069 6e20 7468  s is K_n^i in th
+0000bc00: 6520 7061 7065 722e 0a20 2020 2020 2020  e paper..       
+0000bc10: 2061 4261 723a 206d 7063 2c20 7368 6170   aBar: mpc, shap
+0000bc20: 6528 322c 6e70 726d 5f6d 6178 2b31 2c6e  e(2,nprm_max+1,n
+0000bc30: 7072 6d5f 6d61 782b 312c 6e5f 6264 7329  prm_max+1,n_bds)
+0000bc40: 2e20 536f 6c75 7469 6f6e 7320 666f 7220  . Solutions for 
+0000bc50: 7468 6520 4265 7373 656c 2066 756e 6374  the Bessel funct
+0000bc60: 696f 6e20 636f 6566 6669 6369 656e 7473  ion coefficients
+0000bc70: 0a20 2020 2020 2020 2020 2020 2061 5e69  .            a^i
+0000bc80: 5f7b 6e27 6d27 7d20 666f 7220 7468 6520  _{n'm'} for the 
+0000bc90: 6361 7365 206f 6620 7370 6865 7269 6361  case of spherica
+0000bca0: 6c20 7379 6d6d 6574 7279 2e20 5468 6973  l symmetry. This
+0000bcb0: 2069 7320 5c6f 7665 726c 696e 657b 617d   is \overline{a}
+0000bcc0: 5e5c 6d61 7468 726d 7b69 7d5f 7b6e 276d  ^\mathrm{i}_{n'm
+0000bcd0: 277d 2069 6e20 7468 6520 7061 7065 722e  '} in the paper.
+0000bce0: 0a20 2020 2050 6172 616d 6574 6572 733a  .    Parameters:
+0000bcf0: 0a20 2020 2020 2020 206e 5f6d 6178 3a20  .        n_max: 
+0000bd00: 696e 7465 6765 722e 204d 6178 696d 756d  integer. Maximum
+0000bd10: 2064 6567 7265 6520 6e20 6f66 2069 6e64   degree n of ind
+0000bd20: 7563 6564 206d 6f6d 656e 7473 2e0a 2020  uced moments..  
+0000bd30: 2020 2020 2020 6e70 726d 5f6d 6178 3a20        nprm_max: 
+0000bd40: 696e 7465 6765 722e 204d 6178 696d 756d  integer. Maximum
+0000bd50: 2064 6567 7265 6520 6e27 206f 6620 6578   degree n' of ex
+0000bd60: 6369 7461 7469 6f6e 206d 6f6d 656e 7473  citation moments
+0000bd70: 2e0a 2020 2020 2020 2020 6e3a 206d 7066  ..        n: mpf
+0000bd80: 2c20 7368 6170 6528 6e5f 6d61 7829 2e20  , shape(n_max). 
+0000bd90: 496e 7465 6765 7220 7661 6c75 6573 206f  Integer values o
+0000bda0: 6620 6e20 696e 206d 706d 6174 6820 666c  f n in mpmath fl
+0000bdb0: 6f61 7420 666f 726d 6174 2e0a 2020 2020  oat format..    
+0000bdc0: 2020 2020 6e5f 6264 733a 2069 6e74 6567      n_bds: integ
+0000bdd0: 6572 2e20 4e75 6d62 6572 206f 6620 626f  er. Number of bo
+0000bde0: 756e 6461 7269 6573 2070 7265 7365 6e74  undaries present
+0000bdf0: 2069 6e20 7468 6520 696e 7465 7269 6f72   in the interior
+0000be00: 206d 6f64 656c 2e0a 2020 2020 2020 2020   model..        
+0000be10: 5472 616e 7366 6572 5174 733a 2054 7570  TransferQts: Tup
+0000be20: 6c65 206f 6620 4265 7373 656c 2066 756e  le of Bessel fun
+0000be30: 6374 696f 6e73 2061 6e64 2076 6172 696f  ctions and vario
+0000be40: 7573 2071 7561 6e74 6974 6965 7320 7573  us quantities us
+0000be50: 696e 6720 7468 656d 2c20 616c 6c20 6f66  ing them, all of
+0000be60: 2074 7970 6520 6d70 632e 2053 6565 2042   type mpc. See B
+0000be70: 696e 6d52 6573 706f 6e73 652e 0a20 2020  inmResponse..   
+0000be80: 2020 2020 2052 3a20 666c 6f61 742e 2052       R: float. R
+0000be90: 6164 6975 7320 6f66 2074 6865 206f 7574  adius of the out
+0000bea0: 6572 6d6f 7374 2063 6f6e 6475 6374 696e  ermost conductin
+0000beb0: 6720 626f 756e 6461 7279 2069 6e20 6d2e  g boundary in m.
+0000bec0: 0a20 2020 2020 2020 2042 656e 6d3a 206d  .        Benm: m
+0000bed0: 7063 2c20 7368 6170 6528 322c 6e70 726d  pc, shape(2,nprm
+0000bee0: 5f6d 6178 2b31 2c6e 7072 6d5f 6d61 782b  _max+1,nprm_max+
+0000bef0: 3129 2e20 436f 6d70 6c65 7820 616d 706c  1). Complex ampl
+0000bf00: 6974 7564 6573 206f 6620 6578 6369 7461  itudes of excita
+0000bf10: 7469 6f6e 206d 6f6d 656e 7473 2066 6f72  tion moments for
+0000bf20: 2074 6869 7320 7065 7269 6f64 2e0a 2020   this period..  
+0000bf30: 2020 2222 220a 6465 6620 6765 745f 7365    """.def get_se
+0000bf40: 7269 6573 5f74 6572 6d73 286e 5f6d 6178  ries_terms(n_max
+0000bf50: 2c20 6e70 726d 5f6d 6178 2c20 6e2c 206e  , nprm_max, n, n
+0000bf60: 5f62 6473 2c20 5472 616e 7366 6572 5174  _bds, TransferQt
+0000bf70: 732c 2052 2c20 4265 6e6d 293a 0a20 2020  s, R, Benm):.   
+0000bf80: 206d 7063 203d 206d 7063 5f67 6c6f 6261   mpc = mpc_globa
+0000bf90: 6c0a 2020 2020 6c6f 6e65 203d 206f 6e65  l.    lone = one
+0000bfa0: 0a20 2020 206c 7477 6f20 3d20 7477 6f0a  .    ltwo = two.
+0000bfb0: 2020 2020 6e5f 696e 6e65 7220 3d20 6e5f      n_inner = n_
+0000bfc0: 6264 7320 2d20 310a 2020 2020 6a6e 5f6c  bds - 1.    jn_l
+0000bfd0: 6c2c 2079 6e5f 6c6c 2c20 6a6e 5f75 6c2c  l, yn_ll, jn_ul,
+0000bfe0: 2079 6e5f 756c 2c20 6a64 5f6c 6c2c 2079   yn_ul, jd_ll, y
+0000bff0: 645f 6c6c 2c20 6b72 5f65 782c 206a 6e5f  d_ll, kr_ex, jn_
+0000c000: 6578 2c20 796e 5f65 782c 2061 6c70 682c  ex, yn_ex, alph,
+0000c010: 2062 6574 612c 2067 616d 6d2c 2064 656c   beta, gamm, del
+0000c020: 742c 2065 7073 692c 2064 656c 7451 2c20  t, epsi, deltQ, 
+0000c030: 6570 7369 512c 204c 616d 6264 203d 2054  epsiQ, Lambd = T
+0000c040: 7261 6e73 6665 7251 7473 0a0a 2020 2020  ransferQts..    
+0000c050: 4174 2c20 4b6e 203d 2028 206e 702e 6f6e  At, Kn = ( np.on
+0000c060: 6573 2828 6e5f 6d61 782c 6e5f 6264 7329  es((n_max,n_bds)
+0000c070: 2c20 6474 7970 653d 6d70 6329 2066 6f72  , dtype=mpc) for
+0000c080: 205f 2069 6e20 7261 6e67 6528 3229 2029   _ in range(2) )
+0000c090: 0a20 2020 2061 4261 7220 3d20 6e70 2e7a  .    aBar = np.z
+0000c0a0: 6572 6f73 2828 322c 6e70 726d 5f6d 6178  eros((2,nprm_max
+0000c0b0: 2b31 2c6e 7072 6d5f 6d61 782b 312c 6e5f  +1,nprm_max+1,n_
+0000c0c0: 6264 7329 2c20 6474 7970 653d 6d70 6329  bds), dtype=mpc)
+0000c0d0: 0a0a 2020 2020 6465 6e6f 6d20 3d20 6465  ..    denom = de
+0000c0e0: 6c74 5120 2b20 4c61 6d62 645b 3a2c 2d31  ltQ + Lambd[:,-1
+0000c0f0: 5d20 2a20 6570 7369 510a 0a20 2020 2061  ] * epsiQ..    a
+0000c100: 4261 7242 6173 6520 3d20 2d52 2a42 656e  BarBase = -R*Ben
+0000c110: 6d5b 3a2c 3a6e 7072 6d5f 6d61 782b 312c  m[:,:nprm_max+1,
+0000c120: 3a6e 7072 6d5f 6d61 782b 315d 0a20 2020  :nprm_max+1].   
+0000c130: 2066 6f72 206e 6e70 2069 6e20 7261 6e67   for nnp in rang
+0000c140: 6528 312c 206e 7072 6d5f 6d61 782b 3129  e(1, nprm_max+1)
+0000c150: 3a0a 2020 2020 2020 2020 6e76 203d 206e  :.        nv = n
+0000c160: 5b6e 6e70 2d31 5d0a 2020 2020 2020 2020  [nnp-1].        
+0000c170: 666f 7220 6d6d 7020 696e 2072 616e 6765  for mmp in range
+0000c180: 282d 6e6e 702c 6e6e 702b 3129 3a0a 2020  (-nnp,nnp+1):.  
+0000c190: 2020 2020 2020 2020 2020 6d70 7369 676e            mpsign
+0000c1a0: 203d 2069 6e74 286d 6d70 3c30 290a 2020   = int(mmp<0).  
+0000c1b0: 2020 2020 2020 2020 2020 6d70 6162 7320            mpabs 
+0000c1c0: 3d20 6162 7328 6d6d 7029 0a20 2020 2020  = abs(mmp).     
+0000c1d0: 2020 2020 2020 2061 4261 725b 6d70 7369         aBar[mpsi
+0000c1e0: 676e 2c6e 6e70 2c6d 7061 6273 2c2d 315d  gn,nnp,mpabs,-1]
+0000c1f0: 203d 2063 7078 5f64 6976 5f76 616c 2820   = cpx_div_val( 
+0000c200: 6142 6172 4261 7365 5b6d 7073 6967 6e2c  aBarBase[mpsign,
+0000c210: 6e6e 702c 6d70 6162 735d 202a 2028 6c74  nnp,mpabs] * (lt
+0000c220: 776f 2a6e 7620 2b20 6c6f 6e65 292f 286e  wo*nv + lone)/(n
+0000c230: 7620 2b20 6c6f 6e65 292c 2064 656e 6f6d  v + lone), denom
+0000c240: 5b6e 6e70 2d31 5d20 290a 0a20 2020 2041  [nnp-1] )..    A
+0000c250: 745b 3a2c 2d31 5d20 3d20 6e20 2a20 286a  t[:,-1] = n * (j
+0000c260: 6e5f 6578 202b 204c 616d 6264 5b3a 2c2d  n_ex + Lambd[:,-
+0000c270: 315d 2a79 6e5f 6578 2920 2f20 6465 6e6f  1]*yn_ex) / deno
+0000c280: 6d0a 2020 2020 666f 7220 6920 696e 2072  m.    for i in r
+0000c290: 616e 6765 286e 5f69 6e6e 6572 2d31 2c20  ange(n_inner-1, 
+0000c2a0: 2d31 2c20 2d31 293a 0a20 2020 2020 2020  -1, -1):.       
+0000c2b0: 2041 745b 3a2c 695d 203d 2063 7078 5f64   At[:,i] = cpx_d
+0000c2c0: 6976 2820 286a 6e5f 6c6c 5b3a 2c69 5d20  iv( (jn_ll[:,i] 
+0000c2d0: 2b20 4c61 6d62 645b 3a2c 695d 2a79 6e5f  + Lambd[:,i]*yn_
+0000c2e0: 6c6c 5b3a 2c69 5d29 2c20 6465 6e6f 6d29  ll[:,i]), denom)
+0000c2f0: 0a0a 2020 2020 2020 2020 4b6e 5b3a 2c69  ..        Kn[:,i
+0000c300: 5d20 3d20 6370 785f 6469 7628 2028 4b6e  ] = cpx_div( (Kn
+0000c310: 5b3a 2c69 2b31 5d20 2a20 616c 7068 5b3a  [:,i+1] * alph[:
+0000c320: 2c69 5d29 2c20 2862 6574 615b 3a2c 695d  ,i]), (beta[:,i]
+0000c330: 202b 204c 616d 6264 5b3a 2c69 5d2a 6761   + Lambd[:,i]*ga
+0000c340: 6d6d 5b3a 2c69 5d29 2029 0a0a 2020 2020  mm[:,i]) )..    
+0000c350: 2020 2020 666f 7220 6e6e 7020 696e 2072      for nnp in r
+0000c360: 616e 6765 2831 2c6e 7072 6d5f 6d61 782b  ange(1,nprm_max+
+0000c370: 3129 3a0a 2020 2020 2020 2020 2020 2020  1):.            
+0000c380: 6e70 6920 3d20 6e6e 7020 2d31 0a20 2020  npi = nnp -1.   
+0000c390: 2020 2020 2020 2020 2066 6f72 206d 6d70           for mmp
+0000c3a0: 2069 6e20 7261 6e67 6528 2d6e 6e70 2c6e   in range(-nnp,n
+0000c3b0: 6e70 2b31 293a 0a20 2020 2020 2020 2020  np+1):.         
+0000c3c0: 2020 2020 2020 206d 7073 6967 6e20 3d20         mpsign = 
+0000c3d0: 696e 7428 6d6d 7020 3c20 3029 0a20 2020  int(mmp < 0).   
+0000c3e0: 2020 2020 2020 2020 2020 2020 206d 7061               mpa
+0000c3f0: 6273 203d 2061 6273 286d 6d70 290a 2020  bs = abs(mmp).  
+0000c400: 2020 2020 2020 2020 2020 2020 2020 6142                aB
+0000c410: 6172 5b6d 7073 6967 6e2c 6e6e 702c 6d70  ar[mpsign,nnp,mp
+0000c420: 6162 732c 695d 203d 2063 7078 5f64 6976  abs,i] = cpx_div
+0000c430: 5f76 616c 2820 2861 4261 725b 6d70 7369  _val( (aBar[mpsi
+0000c440: 676e 2c6e 6e70 2c6d 7061 6273 2c69 2b31  gn,nnp,mpabs,i+1
+0000c450: 5d20 2a20 286a 6e5f 756c 5b6e 7069 2c69  ] * (jn_ul[npi,i
+0000c460: 5d20 2b20 4c61 6d62 645b 6e70 692c 692b  ] + Lambd[npi,i+
+0000c470: 315d 2a79 6e5f 756c 5b6e 7069 2c69 5d29  1]*yn_ul[npi,i])
+0000c480: 292c 2028 6a6e 5f6c 6c5b 6e70 692c 695d  ), (jn_ll[npi,i]
+0000c490: 202b 204c 616d 6264 5b6e 7069 2c69 5d2a   + Lambd[npi,i]*
+0000c4a0: 796e 5f6c 6c5b 6e70 692c 695d 2920 290a  yn_ll[npi,i]) ).
+0000c4b0: 0a20 2020 2072 6574 7572 6e20 4174 2c20  .    return At, 
+0000c4c0: 4b6e 2c20 6142 6172 0a0a 2323 2323 2323  Kn, aBar..######
+0000c4d0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0000c4e0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0000c4f0: 2323 2323 2323 230a 0a22 2222 0a67 6574  #######..""".get
+0000c500: 5f44 656c 7461 6e6d 6928 290a 2020 2020  _Deltanmi().    
+0000c510: 4361 6c63 756c 6174 6520 4465 6c74 612c  Calculate Delta,
+0000c520: 2077 6869 6368 2072 6570 7265 7365 6e74   which represent
+0000c530: 7320 7468 6520 616d 6f75 6e74 206f 6620  s the amount of 
+0000c540: 226d 6978 696e 6722 2066 726f 6d20 6578  "mixing" from ex
+0000c550: 6369 7461 7469 6f6e 206d 6f6d 656e 7473  citation moments
+0000c560: 2069 6e74 6f0a 2020 2020 2020 2020 696e   into.        in
+0000c570: 6475 6365 6420 6d6f 6d65 6e74 7320 6f66  duced moments of
+0000c580: 206f 7468 6572 206e 2c6d 2064 7565 2074   other n,m due t
+0000c590: 6f20 6173 796d 6d65 7472 792e 0a20 2020  o asymmetry..   
+0000c5a0: 2055 7361 6765 3a20 6044 656c 7461 6020   Usage: `Delta` 
+0000c5b0: 3d20 6765 745f 4465 6c74 616e 6d69 2860  = get_Deltanmi(`
+0000c5c0: 6e5f 6d61 7860 2c20 6070 5f6d 6178 602c  n_max`, `p_max`,
+0000c5d0: 2060 6e70 726d 5f6d 6178 602c 2060 6e60   `nprm_max`, `n`
+0000c5e0: 2c20 606e 5f62 6473 602c 2060 725f 6264  , `n_bds`, `r_bd
+0000c5f0: 7360 2c20 6042 656e 6d60 2c20 6061 7379  s`, `Benm`, `asy
+0000c600: 6d5f 7368 6170 6560 2c20 6058 6964 602c  m_shape`, `Xid`,
+0000c610: 2060 6142 6172 602c 2060 4164 602c 2060   `aBar`, `Ad`, `
+0000c620: 5472 616e 7366 6572 5174 7360 290a 2020  TransferQts`).  
+0000c630: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
+0000c640: 2020 2044 656c 7461 3a20 6d70 632c 2073     Delta: mpc, s
+0000c650: 6861 7065 2832 2c6e 5f6d 6178 2b31 2c6e  hape(2,n_max+1,n
+0000c660: 5f6d 6178 2b31 2c6e 5f62 6473 292e 2054  _max+1,n_bds). T
+0000c670: 6869 7320 6973 205c 4465 6c74 615e 5c6d  his is \Delta^\m
+0000c680: 6174 6872 6d7b 697d 5f7b 6e6d 7d20 696e  athrm{i}_{nm} in
+0000c690: 2074 6865 2070 6170 6572 2e0a 2020 2020   the paper..    
+0000c6a0: 5061 7261 6d65 7465 7273 3a0a 2020 2020  Parameters:.    
+0000c6b0: 2020 2020 6e5f 6d61 783a 2069 6e74 6567      n_max: integ
+0000c6c0: 6572 2e20 4d61 7869 6d75 6d20 6465 6772  er. Maximum degr
+0000c6d0: 6565 206e 206f 6620 696e 6475 6365 6420  ee n of induced 
+0000c6e0: 6d6f 6d65 6e74 732e 0a20 2020 2020 2020  moments..       
+0000c6f0: 2070 5f6d 6178 3a20 696e 7465 6765 722e   p_max: integer.
+0000c700: 204c 6172 6765 7374 2064 6567 7265 6520   Largest degree 
+0000c710: 7020 696e 2069 6e74 6572 696f 7220 6d6f  p in interior mo
+0000c720: 6465 6c20 626f 756e 6461 7279 2073 6861  del boundary sha
+0000c730: 7065 732e 0a20 2020 2020 2020 206e 7072  pes..        npr
+0000c740: 6d5f 6d61 783a 2069 6e74 6567 6572 2e20  m_max: integer. 
+0000c750: 4d61 7869 6d75 6d20 6465 6772 6565 206e  Maximum degree n
+0000c760: 2720 6f66 2065 7863 6974 6174 696f 6e20  ' of excitation 
+0000c770: 6d6f 6d65 6e74 732e 0a20 2020 2020 2020  moments..       
+0000c780: 206e 3a20 6d70 662c 2073 6861 7065 286e   n: mpf, shape(n
+0000c790: 5f6d 6178 292e 2049 6e74 6567 6572 2076  _max). Integer v
+0000c7a0: 616c 7565 7320 6f66 206e 2069 6e20 6d70  alues of n in mp
+0000c7b0: 6d61 7468 2066 6c6f 6174 2066 6f72 6d61  math float forma
+0000c7c0: 742e 0a20 2020 2020 2020 206e 5f62 6473  t..        n_bds
+0000c7d0: 3a20 696e 7465 6765 722e 204e 756d 6265  : integer. Numbe
+0000c7e0: 7220 6f66 2062 6f75 6e64 6172 6965 7320  r of boundaries 
+0000c7f0: 7072 6573 656e 7420 696e 2074 6865 2069  present in the i
+0000c800: 6e74 6572 696f 7220 6d6f 6465 6c2e 0a20  nterior model.. 
+0000c810: 2020 2020 2020 2072 5f62 6473 3a20 666c         r_bds: fl
+0000c820: 6f61 742c 2073 6861 7065 286e 5f62 6473  oat, shape(n_bds
+0000c830: 292e 2052 6164 6969 2066 6f72 2065 6163  ). Radii for eac
+0000c840: 6820 626f 756e 6461 7279 2073 7572 6661  h boundary surfa
+0000c850: 6365 2069 6e20 6d2e 0a20 2020 2020 2020  ce in m..       
+0000c860: 2042 656e 6d3a 2063 6f6d 706c 6578 2c20   Benm: complex, 
+0000c870: 7368 6170 6528 322c 6e5f 6d61 782b 312c  shape(2,n_max+1,
+0000c880: 6e5f 6d61 782b 3129 2e20 436f 6d70 6c65  n_max+1). Comple
+0000c890: 7820 6578 6369 7461 7469 6f6e 206d 6f6d  x excitation mom
+0000c8a0: 656e 7473 2066 6f72 2074 6869 7320 7065  ents for this pe
+0000c8b0: 7269 6f64 0a20 2020 2020 2020 2020 2020  riod.           
+0000c8c0: 206f 6620 6f73 6369 6c6c 6174 696f 6e2e   of oscillation.
+0000c8d0: 2054 6869 7320 6973 2042 5e7b 657d 5f7b   This is B^{e}_{
+0000c8e0: 6e6d 7d20 696e 2074 6865 2070 6170 6572  nm} in the paper
+0000c8f0: 2e0a 2020 2020 2020 2020 6173 796d 5f73  ..        asym_s
+0000c900: 6861 7065 3a20 636f 6d70 6c65 782c 2073  hape: complex, s
+0000c910: 6861 7065 286e 5f62 6473 2c32 2c70 5f6d  hape(n_bds,2,p_m
+0000c920: 6178 2b31 2c70 5f6d 6178 2b31 292e 2041  ax+1,p_max+1). A
+0000c930: 206c 6973 7420 6f66 2062 6f75 6e64 6172   list of boundar
+0000c940: 7920 7368 6170 6520 7061 7261 6d65 7465  y shape paramete
+0000c950: 7273 2063 6869 5f70 7120 666f 7220 6561  rs chi_pq for ea
+0000c960: 6368 2062 6f75 6e64 6172 792e 0a20 2020  ch boundary..   
+0000c970: 2020 2020 2058 6964 3a20 6d70 662c 2073       Xid: mpf, s
+0000c980: 6861 7065 2832 2c6e 7072 6d5f 6d61 782b  hape(2,nprm_max+
+0000c990: 312c 6e70 726d 5f6d 6178 2b31 2c20 322c  1,nprm_max+1, 2,
+0000c9a0: 705f 6d61 782b 312c 705f 6d61 782b 312c  p_max+1,p_max+1,
+0000c9b0: 2032 2c6e 5f6d 6178 2b31 2c6e 5f6d 6178   2,n_max+1,n_max
+0000c9c0: 2b31 292e 204d 6978 696e 6720 636f 6566  +1). Mixing coef
+0000c9d0: 6669 6369 656e 7473 0a20 2020 2020 2020  ficients.       
+0000c9e0: 2020 2020 2072 6573 756c 7469 6e67 2066       resulting f
+0000c9f0: 726f 6d20 6d75 6c74 6970 6c69 6361 7469  rom multiplicati
+0000ca00: 6f6e 206f 6620 7370 6865 7269 6361 6c20  on of spherical 
+0000ca10: 6861 726d 6f6e 6963 732e 205c 5869 5e7b  harmonics. \Xi^{
+0000ca20: 5c73 7461 7220 6e6d 7d5f 7b6e 276d 2770  \star nm}_{n'm'p
+0000ca30: 717d 2066 726f 6d20 7468 6520 7061 7065  q} from the pape
+0000ca40: 722e 0a20 2020 2020 2020 2061 4261 723a  r..        aBar:
+0000ca50: 206d 7063 2c20 7368 6170 6528 6e5f 6264   mpc, shape(n_bd
+0000ca60: 732c 322c 6e5f 6d61 782b 312c 6e5f 6d61  s,2,n_max+1,n_ma
+0000ca70: 782b 3129 2e20 436f 6d70 6c65 7820 636f  x+1). Complex co
+0000ca80: 6566 6669 6369 656e 7473 2066 6f72 2074  efficients for t
+0000ca90: 6865 2069 6e74 6572 6e61 6c20 6d61 676e  he internal magn
+0000caa0: 6574 6963 2066 6965 6c64 2066 726f 6d20  etic field from 
+0000cab0: 7468 650a 2020 2020 2020 2020 2020 2020  the.            
+0000cac0: 7370 6865 7269 6361 6c6c 7920 7379 6d6d  spherically symm
+0000cad0: 6574 7269 6320 736f 6c75 7469 6f6e 732e  etric solutions.
+0000cae0: 2054 6869 7320 6973 205c 6f76 6572 6c69   This is \overli
+0000caf0: 6e65 7b61 7d5e 5c6d 6174 6872 6d7b 697d  ne{a}^\mathrm{i}
+0000cb00: 5f7b 6e27 6d27 7d20 6672 6f6d 2074 6865  _{n'm'} from the
+0000cb10: 2070 6170 6572 2e0a 2020 2020 2020 2020   paper..        
+0000cb20: 4164 3a20 6d70 632c 2073 6861 7065 286e  Ad: mpc, shape(n
+0000cb30: 7072 6d5f 6d61 7829 2e20 436f 6d70 6c65  prm_max). Comple
+0000cb40: 7820 616d 706c 6974 7564 6520 6d69 7869  x amplitude mixi
+0000cb50: 6e67 2066 726f 6d20 7468 6520 6578 6369  ng from the exci
+0000cb60: 7461 7469 6f6e 2068 6172 6d6f 6e69 6373  tation harmonics
+0000cb70: 2069 6e74 6f20 7468 6520 0a20 2020 2020   into the .     
+0000cb80: 2020 2020 2020 2069 6e64 7563 6564 2068         induced h
+0000cb90: 6172 6d6f 6e69 6373 2e20 5468 6973 2069  armonics. This i
+0000cba0: 7320 5c6d 6174 6863 616c 7b41 7d5e 7b5c  s \mathcal{A}^{\
+0000cbb0: 7374 6172 7d5f 7b6e 277d 2066 726f 6d20  star}_{n'} from 
+0000cbc0: 7468 6520 7061 7065 722e 0a20 2020 2022  the paper..    "
+0000cbd0: 2222 0a64 6566 2067 6574 5f44 656c 7461  "".def get_Delta
+0000cbe0: 6e6d 6928 6e5f 6d61 782c 2070 5f6d 6178  nmi(n_max, p_max
+0000cbf0: 2c20 6e70 726d 5f6d 6178 2c20 6e2c 206e  , nprm_max, n, n
+0000cc00: 5f62 6473 2c20 725f 6264 732c 2042 656e  _bds, r_bds, Ben
+0000cc10: 6d2c 2061 7379 6d5f 7368 6170 652c 2058  m, asym_shape, X
+0000cc20: 6964 2c20 6142 6172 2c20 4164 2c20 5472  id, aBar, Ad, Tr
+0000cc30: 616e 7366 6572 5174 7329 3a0a 2020 2020  ansferQts):.    
+0000cc40: 6d70 6320 3d20 6d70 635f 676c 6f62 616c  mpc = mpc_global
+0000cc50: 0a20 2020 206c 6f6e 6520 3d20 6f6e 650a  .    lone = one.
+0000cc60: 2020 2020 6c74 776f 203d 2074 776f 0a20      ltwo = two. 
+0000cc70: 2020 2044 656c 7461 203d 206e 702e 7a65     Delta = np.ze
+0000cc80: 726f 7328 2832 2c6e 5f6d 6178 2b31 2c6e  ros((2,n_max+1,n
+0000cc90: 5f6d 6178 2b31 2c6e 5f62 6473 292c 2064  _max+1,n_bds), d
+0000cca0: 7479 7065 3d6d 7063 290a 2020 2020 6b72  type=mpc).    kr
+0000ccb0: 5f6c 6c2c 206b 725f 756c 2c20 6a6e 5f6c  _ll, kr_ul, jn_l
+0000ccc0: 6c2c 2079 6e5f 6c6c 2c20 4c61 6d62 6420  l, yn_ll, Lambd 
+0000ccd0: 3d20 5472 616e 7366 6572 5174 730a 2020  = TransferQts.  
+0000cce0: 2020 6d69 7873 756d 5f69 6e69 7420 3d20    mixsum_init = 
+0000ccf0: 6e70 2e7a 6572 6f73 2828 322c 6e70 726d  np.zeros((2,nprm
+0000cd00: 5f6d 6178 2b31 2c6e 7072 6d5f 6d61 782b  _max+1,nprm_max+
+0000cd10: 312c 2032 2c6e 5f6d 6178 2b31 2c6e 5f6d  1, 2,n_max+1,n_m
+0000cd20: 6178 2b31 2c20 6e5f 6264 7329 2c20 6474  ax+1, n_bds), dt
+0000cd30: 7970 653d 6d70 6329 0a0a 2020 2020 666f  ype=mpc)..    fo
+0000cd40: 7220 6e6e 2069 6e20 7261 6e67 6528 312c  r nn in range(1,
+0000cd50: 6e5f 6d61 782b 3129 3a0a 2020 2020 2020  n_max+1):.      
+0000cd60: 2020 6e69 203d 206e 6e20 2d20 310a 2020    ni = nn - 1.  
+0000cd70: 2020 2020 2020 6e76 203d 206e 5b6e 695d        nv = n[ni]
+0000cd80: 0a20 2020 2020 2020 2066 6f72 206d 6d20  .        for mm 
+0000cd90: 696e 2072 616e 6765 282d 6e6e 2c6e 6e2b  in range(-nn,nn+
+0000cda0: 3129 3a0a 2020 2020 2020 2020 2020 2020  1):.            
+0000cdb0: 6d73 6967 6e20 3d20 696e 7428 6d6d 3c30  msign = int(mm<0
+0000cdc0: 290a 2020 2020 2020 2020 2020 2020 6d61  ).            ma
+0000cdd0: 6273 203d 2061 6273 286d 6d29 0a0a 2020  bs = abs(mm)..  
+0000cde0: 2020 2020 2020 2020 2020 666f 7220 6e6e            for nn
+0000cdf0: 7020 696e 2072 616e 6765 2831 2c6e 7072  p in range(1,npr
+0000ce00: 6d5f 6d61 782b 3129 3a0a 2020 2020 2020  m_max+1):.      
+0000ce10: 2020 2020 2020 2020 2020 6e70 6920 3d20            npi = 
+0000ce20: 6e6e 7020 2d20 310a 2020 2020 2020 2020  nnp - 1.        
+0000ce30: 2020 2020 2020 2020 666f 7220 6d6d 7020          for mmp 
+0000ce40: 696e 2072 616e 6765 282d 6e6e 702c 6e6e  in range(-nnp,nn
+0000ce50: 702b 3129 3a0a 2020 2020 2020 2020 2020  p+1):.          
+0000ce60: 2020 2020 2020 2020 2020 6d70 7369 676e            mpsign
+0000ce70: 203d 2069 6e74 286d 6d70 3c30 290a 2020   = int(mmp<0).  
+0000ce80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ce90: 2020 6d70 6162 7320 3d20 6162 7328 6d6d    mpabs = abs(mm
+0000cea0: 7029 0a0a 2020 2020 2020 2020 2020 2020  p)..            
+0000ceb0: 2020 2020 2020 2020 6d69 7873 756d 203d          mixsum =
+0000cec0: 206d 6978 7375 6d5f 696e 6974 202b 2030   mixsum_init + 0
+0000ced0: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000cee0: 2020 2020 2020 666f 7220 7070 2069 6e20        for pp in 
+0000cef0: 7261 6e67 6528 312c 705f 6d61 782b 3129  range(1,p_max+1)
+0000cf00: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000cf10: 2020 2020 2020 2020 2020 7070 6920 3d20            ppi = 
+0000cf20: 7070 202d 2031 0a20 2020 2020 2020 2020  pp - 1.         
+0000cf30: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+0000cf40: 6f72 2071 7120 696e 2072 616e 6765 282d  or qq in range(-
+0000cf50: 7070 2c70 702b 3129 3a0a 2020 2020 2020  pp,pp+1):.      
+0000cf60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cf70: 2020 2020 2020 7173 6967 6e20 3d20 696e        qsign = in
+0000cf80: 7428 7171 3c30 290a 2020 2020 2020 2020  t(qq<0).        
 0000cf90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cfa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cfb0: 2020 6365 6c6c 5f73 7472 203d 2066 227b    cell_str = f"{
-0000cfc0: 6365 6c6c 5f73 7472 7d20 220a 2020 2020  cell_str} ".    
-0000cfd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cfe0: 2020 2020 2020 2020 2020 2020 656c 7365              else
-0000cff0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000d000: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d010: 2020 2020 2020 6365 6c6c 5f73 7472 203d        cell_str =
-0000d020: 2066 227b 6365 6c6c 5f73 7472 7d2d 220a   f"{cell_str}-".
+0000cfa0: 2020 2020 7161 6273 203d 2061 6273 2871      qabs = abs(q
+0000cfb0: 7129 0a0a 2020 2020 2020 2020 2020 2020  q)..            
+0000cfc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000cfd0: 6d69 7873 756d 5b6d 7073 6967 6e2c 6e6e  mixsum[mpsign,nn
+0000cfe0: 702c 6d70 6162 732c 206d 7369 676e 2c6e  p,mpabs, msign,n
+0000cff0: 6e2c 6d61 6273 2c20 3a5d 202b 3d20 6173  n,mabs, :] += as
+0000d000: 796d 5f73 6861 7065 5b3a 2c71 7369 676e  ym_shape[:,qsign
+0000d010: 2c70 702c 7161 6273 5d2f 725f 6264 735b  ,pp,qabs]/r_bds[
+0000d020: 3a5d 202a 205c 0a20 2020 2020 2020 2020  :] * \.         
 0000d030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d040: 2020 2020 2020 2020 2020 2020 6365 6c6c              cell
-0000d050: 5f73 7472 203d 2066 227b 6365 6c6c 5f73  _str = f"{cell_s
-0000d060: 7472 7d7b 726f 756e 645f 5869 7d59 7b6e  tr}{round_Xi}Y{n
-0000d070: 7072 6d7d 7b6d 7072 6d7d 2022 2e6c 6a75  prm}{mprm} ".lju
-0000d080: 7374 2831 3329 0a0a 2020 2020 2020 2020  st(13)..        
-0000d090: 2020 2020 2020 2020 2020 2020 726f 775f              row_
-0000d0a0: 7374 7220 3d20 6622 7b72 6f77 5f73 7472  str = f"{row_str
-0000d0b0: 7d7b 6365 6c6c 5f73 7472 2e6c 6a75 7374  }{cell_str.ljust
-0000d0c0: 2832 3529 7d22 0a0a 2020 2020 2020 2020  (25)}"..        
-0000d0d0: 2020 2020 726f 775f 7374 7220 3d20 6622      row_str = f"
-0000d0e0: 7b72 6f77 5f73 7472 7d7c 220a 2020 2020  {row_str}|".    
-0000d0f0: 2020 2020 2020 2020 7072 696e 7428 726f          print(ro
-0000d100: 775f 7374 7229 0a0a 2020 2020 7265 7475  w_str)..    retu
-0000d110: 726e 0a0a 2222 220a 7072 696e 745f 5869  rn..""".print_Xi
-0000d120: 5f74 6162 6c65 2829 0a20 2020 2050 7269  _table().    Pri
-0000d130: 6e74 7320 6120 7461 626c 6520 746f 2074  nts a table to t
-0000d140: 6865 2074 6572 6d69 6e61 6c20 6f66 2076  he terminal of v
-0000d150: 616c 7565 7320 666f 7220 616c 6c20 5869  alues for all Xi
-0000d160: 2066 6f72 2064 6562 7567 2070 7572 706f   for debug purpo
-0000d170: 7365 732e 0a20 2020 2055 7361 6765 3a20  ses..    Usage: 
-0000d180: 7072 696e 745f 5869 5f74 6162 6c65 2860  print_Xi_table(`
-0000d190: 6e5f 6d61 7860 2c20 6070 5f6d 6178 602c  n_max`, `p_max`,
-0000d1a0: 2060 6e70 726d 5f6d 6178 6029 0a20 2020   `nprm_max`).   
-0000d1b0: 2052 6574 7572 6e73 3a0a 2020 2020 2020   Returns:.      
-0000d1c0: 2020 4e6f 6e65 2e0a 2020 2020 5061 7261    None..    Para
-0000d1d0: 6d65 7465 7273 3a0a 2020 2020 2020 2020  meters:.        
-0000d1e0: 6e5f 6d61 783a 2069 6e74 6567 6572 2e20  n_max: integer. 
-0000d1f0: 4d61 7869 6d75 6d20 6465 6772 6565 206e  Maximum degree n
-0000d200: 206f 6620 6578 6369 7461 7469 6f6e 206d   of excitation m
-0000d210: 6f6d 656e 7473 2e0a 2020 2020 2020 2020  oments..        
-0000d220: 705f 6d61 783a 2069 6e74 6567 6572 2e20  p_max: integer. 
-0000d230: 4d61 7869 6d75 6d20 6465 6772 6565 2070  Maximum degree p
-0000d240: 206f 6620 626f 756e 6461 7279 2073 6861   of boundary sha
-0000d250: 7065 732e 0a20 2020 2020 2020 206e 7072  pes..        npr
-0000d260: 6d5f 6d61 783a 2069 6e74 6567 6572 2e20  m_max: integer. 
-0000d270: 4d61 7869 6d75 6d20 6465 6772 6565 206e  Maximum degree n
-0000d280: 7072 6d20 6f66 2069 6e64 7563 6564 206d  prm of induced m
-0000d290: 6f6d 656e 7473 2e20 5479 7069 6361 6c6c  oments. Typicall
-0000d2a0: 7920 6e6d 6178 202b 2070 6d61 782e 0a20  y nmax + pmax.. 
-0000d2b0: 2020 2022 2222 0a64 6566 2070 7269 6e74     """.def print
-0000d2c0: 5f58 695f 7461 626c 6528 6e5f 6d61 782c  _Xi_table(n_max,
-0000d2d0: 2070 5f6d 6178 2c20 6e70 726d 5f6d 6178   p_max, nprm_max
-0000d2e0: 293a 0a20 2020 2023 2050 7269 6e74 2074  ):.    # Print t
-0000d2f0: 6162 6c65 2068 6561 6465 720a 2020 2020  able header.    
-0000d300: 6865 6164 5f72 6f77 203d 2022 2020 2020  head_row = "    
-0000d310: 220a 2020 2020 666f 7220 6e20 696e 2072  ".    for n in r
-0000d320: 616e 6765 2831 2c20 6e5f 6d61 782b 3129  ange(1, n_max+1)
-0000d330: 3a0a 2020 2020 2020 2020 666f 7220 6d20  :.        for m 
-0000d340: 696e 2072 616e 6765 282d 6e2c 206e 2b31  in range(-n, n+1
-0000d350: 293a 0a20 2020 2020 2020 2020 2020 2068  ):.            h
-0000d360: 6561 645f 726f 7720 3d20 6622 7b68 6561  ead_row = f"{hea
-0000d370: 645f 726f 777d 7c20 2020 2059 7b6e 7d7b  d_row}|    Y{n}{
-0000d380: 6d7d 2020 2020 222e 6c6a 7573 7428 3235  m}    ".ljust(25
-0000d390: 290a 2020 2020 6865 6164 5f72 6f77 203d  ).    head_row =
-0000d3a0: 2066 227b 6865 6164 5f72 6f77 7d7c 220a   f"{head_row}|".
-0000d3b0: 2020 2020 7072 696e 7428 6865 6164 5f72      print(head_r
-0000d3c0: 6f77 290a 2020 2020 2320 5072 696e 7420  ow).    # Print 
-0000d3d0: 7368 6170 6573 2061 7320 726f 7773 0a20  shapes as rows. 
-0000d3e0: 2020 2066 6f72 2070 2069 6e20 7261 6e67     for p in rang
-0000d3f0: 6528 312c 2070 5f6d 6178 2b31 293a 0a20  e(1, p_max+1):. 
-0000d400: 2020 2020 2020 2066 6f72 2071 2069 6e20         for q in 
-0000d410: 7261 6e67 6528 2d70 2c20 702b 3129 3a0a  range(-p, p+1):.
-0000d420: 2020 2020 2020 2020 2020 2020 726f 775f              row_
-0000d430: 7374 7220 3d20 6622 537b 707d 7b71 7d22  str = f"S{p}{q}"
-0000d440: 2e6c 6a75 7374 2834 290a 0a20 2020 2020  .ljust(4)..     
-0000d450: 2020 2020 2020 2023 2050 7269 6e74 2065         # Print e
-0000d460: 7863 6974 6174 696f 6e20 6d6f 6d65 6e74  xcitation moment
-0000d470: 7320 6173 2063 6f6c 756d 6e73 0a20 2020  s as columns.   
-0000d480: 2020 2020 2020 2020 2066 6f72 206e 2069           for n i
-0000d490: 6e20 7261 6e67 6528 312c 206e 5f6d 6178  n range(1, n_max
-0000d4a0: 2b31 293a 0a20 2020 2020 2020 2020 2020  +1):.           
-0000d4b0: 2020 2020 2066 6f72 206d 2069 6e20 7261       for m in ra
-0000d4c0: 6e67 6528 2d6e 2c20 6e2b 3129 3a0a 2020  nge(-n, n+1):.  
-0000d4d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d4e0: 2020 6365 6c6c 5f73 7472 203d 2022 7c20    cell_str = "| 
-0000d4f0: 220a 0a20 2020 2020 2020 2020 2020 2020  "..             
-0000d500: 2020 2020 2020 2023 2050 7269 6e74 206e         # Print n
-0000d510: 6f6e 2d7a 6572 6f20 7465 726d 7320 666f  on-zero terms fo
-0000d520: 7220 6561 6368 2063 656c 6c0a 2020 2020  r each cell.    
-0000d530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d540: 666f 7220 6e70 726d 2069 6e20 7261 6e67  for nprm in rang
-0000d550: 6528 6e70 726d 5f6d 6178 2c20 302c 202d  e(nprm_max, 0, -
-0000d560: 3129 3a0a 2020 2020 2020 2020 2020 2020  1):.            
-0000d570: 2020 2020 2020 2020 2020 2020 6d70 726d              mprm
-0000d580: 203d 206d 202b 2071 0a0a 2020 2020 2020   = m + q..      
-0000d590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d5a0: 2020 7468 6973 5f58 6920 3d20 6361 6c63    this_Xi = calc
-0000d5b0: 5f58 6928 6e2c 6d2c 702c 712c 6e70 726d  _Xi(n,m,p,q,nprm
-0000d5c0: 2c6d 7072 6d29 0a20 2020 2020 2020 2020  ,mprm).         
-0000d5d0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0000d5e0: 6620 6162 7328 7468 6973 5f58 6929 203e  f abs(this_Xi) >
-0000d5f0: 2030 2e30 3030 3031 3a0a 2020 2020 2020   0.00001:.      
-0000d600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d610: 2020 2020 2020 6966 2063 656c 6c5f 7374        if cell_st
-0000d620: 7220 213d 2022 7c20 223a 0a20 2020 2020  r != "| ":.     
-0000d630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d640: 2020 2020 2020 2020 2020 2069 6628 696e             if(in
-0000d650: 7428 7468 6973 5f58 693c 3029 293a 0a20  t(this_Xi<0)):. 
-0000d660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d670: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d680: 2020 2063 656c 6c5f 7374 7220 3d20 6622     cell_str = f"
-0000d690: 7b63 656c 6c5f 7374 727d 2d20 220a 2020  {cell_str}- ".  
-0000d6a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d6b0: 2020 2020 2020 2020 2020 2020 2020 656c                el
-0000d6c0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-0000d6d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d6e0: 2020 2020 2020 2020 6365 6c6c 5f73 7472          cell_str
-0000d6f0: 203d 2066 227b 6365 6c6c 5f73 7472 7d2b   = f"{cell_str}+
-0000d700: 2022 0a20 2020 2020 2020 2020 2020 2020   ".             
-0000d710: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-0000d720: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-0000d730: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d740: 2020 2020 2069 6628 696e 7428 7468 6973       if(int(this
-0000d750: 5f58 693c 3029 293a 0a20 2020 2020 2020  _Xi<0)):.       
-0000d760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d770: 2020 2020 2020 2020 2020 2020 2063 656c               cel
-0000d780: 6c5f 7374 7220 3d20 6622 7b63 656c 6c5f  l_str = f"{cell_
-0000d790: 7374 727d 2d22 0a20 2020 2020 2020 2020  str}-".         
-0000d7a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d7b0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-0000d7c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d7d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d7e0: 2063 656c 6c5f 7374 7220 3d20 6622 7b63   cell_str = f"{c
-0000d7f0: 656c 6c5f 7374 727d 2022 0a20 2020 2020  ell_str} ".     
-0000d800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d810: 2020 2020 2020 2063 656c 6c5f 7374 7220         cell_str 
-0000d820: 3d20 6622 7b63 656c 6c5f 7374 727d 7b61  = f"{cell_str}{a
-0000d830: 6273 2874 6869 735f 5869 293a 2e33 667d  bs(this_Xi):.3f}
-0000d840: 597b 6e70 726d 7d7b 6d70 726d 7d20 222e  Y{nprm}{mprm} ".
-0000d850: 6c6a 7573 7428 3133 290a 0a20 2020 2020  ljust(13)..     
-0000d860: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-0000d870: 6f77 5f73 7472 203d 2066 227b 726f 775f  ow_str = f"{row_
-0000d880: 7374 727d 7b63 656c 6c5f 7374 727d 222e  str}{cell_str}".
-0000d890: 6c6a 7573 7428 3235 290a 0a20 2020 2020  ljust(25)..     
-0000d8a0: 2020 2020 2020 2072 6f77 5f73 7472 203d         row_str =
-0000d8b0: 2066 227b 726f 775f 7374 727d 7c22 0a20   f"{row_str}|". 
-0000d8c0: 2020 2020 2020 2020 2020 2070 7269 6e74             print
-0000d8d0: 2872 6f77 5f73 7472 290a 0a20 2020 2072  (row_str)..    r
-0000d8e0: 6574 7572 6e0a 0a22 2222 0a54 6865 2072  eturn..""".The r
-0000d8f0: 656d 6169 6e69 6e67 2066 756e 6374 696f  emaining functio
-0000d900: 6e73 2069 6e20 7468 6973 2062 6c6f 636b  ns in this block
-0000d910: 2061 7265 2061 6c6c 2073 7465 7073 2061   are all steps a
-0000d920: 6e64 2073 7562 7374 6570 7320 696e 2063  nd substeps in c
-0000d930: 616c 6375 6c61 7469 6e67 2058 6964 0a20  alculating Xid. 
-0000d940: 2020 2061 7320 696e 2065 7175 6174 696f     as in equatio
-0000d950: 6e73 2053 3931 2d53 3130 3320 6672 6f6d  ns S91-S103 from
-0000d960: 2074 6865 2070 6170 6572 2e0a 2020 2020   the paper..    
-0000d970: 2222 220a 6465 6620 6361 6c63 5f58 6964  """.def calc_Xid
-0000d980: 286e 2c6d 2c70 2c71 2c6e 7072 6d2c 6d70  (n,m,p,q,nprm,mp
-0000d990: 726d 2c20 6e70 726d 5f6d 6178 293a 0a20  rm, nprm_max):. 
-0000d9a0: 2020 2074 6869 735f 5869 645f 6e75 6d20     this_Xid_num 
-0000d9b0: 3d20 2020 2020 2020 2063 616c 635f 5869  =        calc_Xi
-0000d9c0: 7728 6e2c 206d 2c20 702c 2071 2c20 6e70  w(n, m, p, q, np
-0000d9d0: 726d 2c20 6d70 726d 2920 2b20 205c 0a20  rm, mprm) +  \. 
-0000d9e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d9f0: 2020 2058 6964 5365 7269 6573 4c6f 7765     XidSeriesLowe
-0000da00: 7228 6e2c 206d 2c20 702c 2071 2c20 6e70  r(n, m, p, q, np
-0000da10: 726d 2c20 6d70 726d 2920 2b20 205c 0a20  rm, mprm) +  \. 
-0000da20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000da30: 2020 2058 6964 5365 7269 6573 5570 7065     XidSeriesUppe
-0000da40: 7228 6e2c 206d 2c20 702c 2071 2c20 6e70  r(n, m, p, q, np
-0000da50: 726d 2c20 6d70 726d 2c20 6e70 726d 5f6d  rm, mprm, nprm_m
-0000da60: 6178 290a 2020 2020 6966 2074 6869 735f  ax).    if this_
-0000da70: 5869 645f 6e75 6d20 213d 2030 3a0a 2020  Xid_num != 0:.  
-0000da80: 2020 2020 2020 5869 6420 3d20 7468 6973        Xid = this
-0000da90: 5f58 6964 5f6e 756d 202f 2058 6964 4465  _Xid_num / XidDe
-0000daa0: 6e6f 6d28 6e70 726d 2c6d 7072 6d2c 6e70  nom(nprm,mprm,np
-0000dab0: 726d 5f6d 6178 290a 2020 2020 656c 7365  rm_max).    else
-0000dac0: 3a0a 2020 2020 2020 2020 5869 6420 3d20  :.        Xid = 
-0000dad0: 7a65 726f 0a20 2020 2072 6574 7572 6e20  zero.    return 
-0000dae0: 5869 640a 0a64 6566 2063 616c 635f 5869  Xid..def calc_Xi
-0000daf0: 286e 2c20 6d2c 2070 2c20 712c 206e 7072  (n, m, p, q, npr
-0000db00: 6d2c 206d 7072 6d29 3a0a 2020 2020 7472  m, mprm):.    tr
-0000db10: 6961 6e67 203d 2028 6162 7328 6e20 2d20  iang = (abs(n - 
-0000db20: 7029 203c 3d20 6e70 726d 2920 616e 6420  p) <= nprm) and 
-0000db30: 286e 7072 6d20 3c3d 206e 202b 2070 290a  (nprm <= n + p).
-0000db40: 2020 2020 6576 656e 203d 2028 6e20 2b20      even = (n + 
-0000db50: 7020 2b20 6e70 726d 2920 2520 3220 3d3d  p + nprm) % 2 ==
-0000db60: 2030 0a20 2020 206d 5f6d 6174 6368 203d   0.    m_match =
-0000db70: 2028 6d20 2b20 7120 3d3d 206d 7072 6d29   (m + q == mprm)
-0000db80: 0a0a 2020 2020 6966 2074 7269 616e 6720  ..    if triang 
-0000db90: 616e 6420 6576 656e 2061 6e64 206d 5f6d  and even and m_m
-0000dba0: 6174 6368 3a0a 2020 2020 2020 2020 6e75  atch:.        nu
-0000dbb0: 203d 2069 6e74 2828 6e20 2b20 7020 2d20   = int((n + p - 
-0000dbc0: 6e70 726d 292f 3229 0a20 2020 2020 2020  nprm)/2).       
-0000dbd0: 2063 735f 7369 676e 203d 2028 2d31 292a   cs_sign = (-1)*
-0000dbe0: 2a6e 750a 0a20 2020 2020 2020 206b 6170  *nu..        kap
-0000dbf0: 5f6d 696e 203d 206d 6178 2830 2c20 322a  _min = max(0, 2*
-0000dc00: 6e75 2d28 6e2b 6d29 2c20 322a 6e75 2d28  nu-(n+m), 2*nu-(
-0000dc10: 702d 7129 290a 2020 2020 2020 2020 6b61  p-q)).        ka
-0000dc20: 705f 6d61 7820 3d20 6d69 6e28 322a 6e75  p_max = min(2*nu
-0000dc30: 2c20 6e2d 6d2c 2070 2b71 290a 0a20 2020  , n-m, p+q)..   
-0000dc40: 2020 2020 206e 6f72 6d20 3d20 6e70 2e73       norm = np.s
-0000dc50: 7172 7428 2832 2a6e 202b 2031 2920 2a20  qrt((2*n + 1) * 
-0000dc60: 2832 2a70 202b 2031 2920 2a20 2832 2a6e  (2*p + 1) * (2*n
-0000dc70: 7072 6d20 2b20 3129 202f 2034 202f 206e  prm + 1) / 4 / n
-0000dc80: 702e 7069 290a 2020 2020 2020 2020 6674  p.pi).        ft
-0000dc90: 5f73 7172 7420 3d20 6e70 2e73 7172 7428  _sqrt = np.sqrt(
-0000dca0: 2066 7428 6e2b 6d29 2a66 7428 6e2d 6d29   ft(n+m)*ft(n-m)
-0000dcb0: 2a66 7428 702b 7129 2a66 7428 702d 7129  *ft(p+q)*ft(p-q)
-0000dcc0: 2a66 7428 6e70 726d 2b6d 7072 6d29 2a66  *ft(nprm+mprm)*f
-0000dcd0: 7428 6e70 726d 2d6d 7072 6d29 2029 0a20  t(nprm-mprm) ). 
-0000dce0: 2020 2020 2020 2066 745f 6672 6163 203d         ft_frac =
-0000dcf0: 2066 7428 322a 6e75 292f 6674 286e 7529   ft(2*nu)/ft(nu)
-0000dd00: 202a 2066 7428 322a 6e2d 322a 6e75 292f   * ft(2*n-2*nu)/
-0000dd10: 6674 286e 2d6e 7529 202a 2066 7428 322a  ft(n-nu) * ft(2*
-0000dd20: 702d 322a 6e75 292f 6674 2870 2d6e 7529  p-2*nu)/ft(p-nu)
-0000dd30: 202a 2066 7428 6e70 726d 2b6e 7529 2f66   * ft(nprm+nu)/f
-0000dd40: 7428 322a 6e70 726d 2b31 2b32 2a6e 7529  t(2*nprm+1+2*nu)
-0000dd50: 0a0a 2020 2020 2020 2020 6b61 705f 7375  ..        kap_su
-0000dd60: 6d20 3d20 6e70 2e73 756d 285b 2028 2d31  m = np.sum([ (-1
-0000dd70: 292a 2a6b 6170 202f 2028 2066 7428 6b61  )**kap / ( ft(ka
-0000dd80: 7029 2a66 7428 322a 6e75 2d6b 6170 2920  p)*ft(2*nu-kap) 
-0000dd90: 2a20 6674 286e 2d6d 2d6b 6170 292a 6674  * ft(n-m-kap)*ft
-0000dda0: 286e 2b6d 2d28 322a 6e75 2d6b 6170 2929  (n+m-(2*nu-kap))
-0000ddb0: 202a 0a20 2020 2020 2020 2020 2020 2066   *.            f
-0000ddc0: 7428 702b 712d 6b61 7029 2a66 7428 702d  t(p+q-kap)*ft(p-
-0000ddd0: 712d 2832 2a6e 752d 6b61 7029 2920 2920  q-(2*nu-kap)) ) 
-0000dde0: 666f 7220 6b61 7020 696e 2072 616e 6765  for kap in range
-0000ddf0: 286b 6170 5f6d 696e 2c6b 6170 5f6d 6178  (kap_min,kap_max
-0000de00: 2b31 2920 5d29 0a0a 2020 2020 2020 2020  +1) ])..        
-0000de10: 5869 203d 2063 735f 7369 676e 202a 206e  Xi = cs_sign * n
-0000de20: 6f72 6d20 2a20 6674 5f66 7261 6320 2a20  orm * ft_frac * 
-0000de30: 6674 5f73 7172 7420 2a20 6b61 705f 7375  ft_sqrt * kap_su
-0000de40: 6d0a 2020 2020 656c 7365 3a0a 2020 2020  m.    else:.    
-0000de50: 2020 2020 5869 203d 207a 6572 6f0a 0a20      Xi = zero.. 
-0000de60: 2020 2072 6574 7572 6e20 5869 0a0a 6465     return Xi..de
-0000de70: 6620 775f 4d28 6e2c 6d29 3a0a 2020 2020  f w_M(n,m):.    
-0000de80: 776d 203d 206d 702e 7265 2820 286e 2b31  wm = mp.re( (n+1
-0000de90: 292a 6d70 2e73 7172 7428 6e2a 2a32 202d  )*mp.sqrt(n**2 -
-0000dea0: 206d 2a2a 3229 202f 206d 702e 7371 7274   m**2) / mp.sqrt
-0000deb0: 2828 322a 6e2d 3129 202a 2028 322a 6e2b  ((2*n-1) * (2*n+
-0000dec0: 3129 2920 290a 2020 2020 7265 7475 726e  1)) ).    return
-0000ded0: 2077 6d0a 0a64 6566 2077 5f50 286e 2c6d   wm..def w_P(n,m
-0000dee0: 293a 0a20 2020 2077 7020 3d20 6e2a 6d70  ):.    wp = n*mp
-0000def0: 2e72 6528 206d 702e 7371 7274 2828 6e2b  .re( mp.sqrt((n+
-0000df00: 3129 2a2a 3220 2d20 6d2a 2a32 2920 2f20  1)**2 - m**2) / 
-0000df10: 6d70 2e73 7172 7428 2832 2a6e 2b31 292a  mp.sqrt((2*n+1)*
-0000df20: 2832 2a6e 2b33 2929 2029 0a20 2020 2072  (2*n+3)) ).    r
-0000df30: 6574 7572 6e20 7770 0a0a 6465 6620 6361  eturn wp..def ca
-0000df40: 6c63 5f58 6977 286e 2c20 6d2c 2070 2c20  lc_Xiw(n, m, p, 
-0000df50: 712c 206e 7072 6d2c 206d 7072 6d29 3a0a  q, nprm, mprm):.
-0000df60: 2020 2020 6d61 6273 203d 2061 6273 286d      mabs = abs(m
-0000df70: 290a 2020 2020 6d70 6162 7320 3d20 6162  ).    mpabs = ab
-0000df80: 7328 6d70 726d 290a 0a20 2020 2077 4d6e  s(mprm)..    wMn
-0000df90: 203d 2077 5f4d 286e 2c6d 6162 7329 0a20   = w_M(n,mabs). 
-0000dfa0: 2020 2077 506e 203d 2077 5f50 286e 2c6d     wPn = w_P(n,m
-0000dfb0: 6162 7329 0a20 2020 2077 4d6e 7020 3d20  abs).    wMnp = 
-0000dfc0: 775f 4d28 6e70 726d 2c6d 7061 6273 290a  w_M(nprm,mpabs).
-0000dfd0: 2020 2020 7750 6e70 203d 2077 5f50 286e      wPnp = w_P(n
-0000dfe0: 7072 6d2c 6d70 6162 7329 0a0a 2020 2020  prm,mpabs)..    
-0000dff0: 5869 7720 3d20 2077 4d6e 202a 2077 4d6e  Xiw =  wMn * wMn
-0000e000: 7020 2a20 6361 6c63 5f58 6928 6e2d 312c  p * calc_Xi(n-1,
-0000e010: 206d 2c20 702c 2071 2c20 6e70 726d 2d31   m, p, q, nprm-1
-0000e020: 2c20 6d70 726d 2920 2020 205c 0a20 2020  , mprm)    \.   
-0000e030: 2020 2020 2020 2b20 7750 6e20 2a20 7750        + wPn * wP
-0000e040: 6e70 202a 2063 616c 635f 5869 286e 2b31  np * calc_Xi(n+1
-0000e050: 2c20 6d2c 2070 2c20 712c 206e 7072 6d2b  , m, p, q, nprm+
-0000e060: 312c 206d 7072 6d29 2020 2020 5c0a 2020  1, mprm)    \.  
-0000e070: 2020 2020 2020 202d 2077 4d6e 202a 2077         - wMn * w
-0000e080: 506e 7020 2a20 6361 6c63 5f58 6928 6e2d  Pnp * calc_Xi(n-
-0000e090: 312c 206d 2c20 702c 2071 2c20 6e70 726d  1, m, p, q, nprm
-0000e0a0: 2b31 2c20 6d70 726d 2920 2020 205c 0a20  +1, mprm)    \. 
-0000e0b0: 2020 2020 2020 2020 2d20 7750 6e20 2a20          - wPn * 
-0000e0c0: 774d 6e70 202a 2063 616c 635f 5869 286e  wMnp * calc_Xi(n
-0000e0d0: 2b31 2c20 6d2c 2070 2c20 712c 206e 7072  +1, m, p, q, npr
-0000e0e0: 6d2d 312c 206d 7072 6d29 0a0a 2020 2020  m-1, mprm)..    
-0000e0f0: 7265 7475 726e 2058 6977 0a0a 6465 6620  return Xiw..def 
-0000e100: 465f 4d28 6e2c 206d 2c20 7477 6f6b 6170  F_M(n, m, twokap
-0000e110: 293a 0a20 2020 2069 6620 6e20 3c20 3320  ):.    if n < 3 
-0000e120: 6f72 2074 776f 6b61 7020 3e20 6e2d 6162  or twokap > n-ab
-0000e130: 7328 6d29 2d32 3a0a 2020 2020 2020 2020  s(m)-2:.        
-0000e140: 7265 7475 726e 207a 6572 6f0a 2020 2020  return zero.    
-0000e150: 656c 7365 3a0a 2020 2020 2020 2020 6e5f  else:.        n_
-0000e160: 7468 6973 203d 206e 2d74 776f 6b61 700a  this = n-twokap.
-0000e170: 2020 2020 2020 2020 6e5f 646f 776e 203d          n_down =
-0000e180: 206e 2d28 7477 6f6b 6170 2b32 290a 2020   n-(twokap+2).  
-0000e190: 2020 2020 2020 6e5f 646f 776e 3220 3d20        n_down2 = 
-0000e1a0: 6e2d 2874 776f 6b61 702b 3429 0a20 2020  n-(twokap+4).   
-0000e1b0: 2020 2020 2069 6620 775f 4d28 6e5f 7468       if w_M(n_th
-0000e1c0: 6973 2c6d 293d 3d30 206f 7220 775f 5028  is,m)==0 or w_P(
-0000e1d0: 6e5f 646f 776e 2c6d 293d 3d30 3a0a 2020  n_down,m)==0:.  
-0000e1e0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-0000e1f0: 207a 6572 6f0a 2020 2020 2020 2020 656c   zero.        el
-0000e200: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-0000e210: 466d 203d 2077 5f4d 286e 5f74 6869 732c  Fm = w_M(n_this,
-0000e220: 6d29 2a77 5f50 286e 5f64 6f77 6e2c 6d29  m)*w_P(n_down,m)
-0000e230: 202f 2020 2020 5c0a 2020 2020 2020 2020   /    \.        
-0000e240: 2020 2020 2820 775f 4d28 6e5f 646f 776e      ( w_M(n_down
-0000e250: 2c6d 292a 2a32 202b 2077 5f50 286e 5f64  ,m)**2 + w_P(n_d
-0000e260: 6f77 6e2c 6d29 2a2a 3220 2d0a 2020 2020  own,m)**2 -.    
-0000e270: 2020 2020 2020 2020 2020 2020 775f 4d28              w_M(
-0000e280: 6e5f 646f 776e 2c6d 292a 775f 5028 6e5f  n_down,m)*w_P(n_
-0000e290: 646f 776e 322c 6d29 2a46 5f4d 286e 2c6d  down2,m)*F_M(n,m
-0000e2a0: 2c74 776f 6b61 702b 3229 2029 0a0a 2020  ,twokap+2) )..  
-0000e2b0: 2020 7265 7475 726e 2046 6d0a 0a64 6566    return Fm..def
-0000e2c0: 2046 5f50 286e 2c20 6d2c 2074 776f 6b61   F_P(n, m, twoka
-0000e2d0: 702c 206e 7072 6d5f 6d61 7829 3a0a 2020  p, nprm_max):.  
-0000e2e0: 2020 6966 2074 776f 6b61 7020 3e20 6e70    if twokap > np
-0000e2f0: 726d 5f6d 6178 2d6e 3a0a 2020 2020 2020  rm_max-n:.      
-0000e300: 2020 7265 7475 726e 207a 6572 6f0a 2020    return zero.  
-0000e310: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-0000e320: 6e5f 7468 6973 203d 206e 2b74 776f 6b61  n_this = n+twoka
-0000e330: 700a 2020 2020 2020 2020 6e5f 7570 203d  p.        n_up =
-0000e340: 206e 2b28 7477 6f6b 6170 2b32 290a 2020   n+(twokap+2).  
-0000e350: 2020 2020 2020 6e5f 7570 3220 3d20 6e2b        n_up2 = n+
-0000e360: 2874 776f 6b61 702b 3429 0a20 2020 2020  (twokap+4).     
-0000e370: 2020 2046 7020 3d20 775f 5028 6e5f 7468     Fp = w_P(n_th
-0000e380: 6973 2c6d 292a 775f 4d28 6e5f 7570 2c6d  is,m)*w_M(n_up,m
-0000e390: 2920 2f20 2020 205c 0a20 2020 2020 2020  ) /    \.       
-0000e3a0: 2028 2077 5f4d 286e 5f75 702c 6d29 2a2a   ( w_M(n_up,m)**
-0000e3b0: 3220 2b20 775f 5028 6e5f 7570 2c6d 292a  2 + w_P(n_up,m)*
-0000e3c0: 2a32 202d 0a20 2020 2020 2020 2020 2020  *2 -.           
-0000e3d0: 2077 5f50 286e 5f75 702c 6d29 2a77 5f4d   w_P(n_up,m)*w_M
-0000e3e0: 286e 5f75 7032 2c6d 292a 465f 5028 6e2c  (n_up2,m)*F_P(n,
-0000e3f0: 6d2c 7477 6f6b 6170 2b32 2c6e 7072 6d5f  m,twokap+2,nprm_
-0000e400: 6d61 7829 2029 0a0a 2020 2020 7265 7475  max) )..    retu
-0000e410: 726e 2046 700a 0a23 204e 6f74 6520 7468  rn Fp..# Note th
-0000e420: 6174 2061 6c74 686f 7567 6820 7468 6973  at although this
-0000e430: 2074 6572 6d20 6973 2063 616c 6c65 6420   term is called 
-0000e440: 5365 7269 6573 4c6f 7765 722c 2069 7420  SeriesLower, it 
-0000e450: 636f 6e74 6169 6e73 206d 6978 696e 6720  contains mixing 
-0000e460: 7465 726d 7320 6672 6f6d 2068 6967 6865  terms from highe
-0000e470: 7220 6465 6772 6565 206e 2727 2069 6e74  r degree n'' int
-0000e480: 6f20 7468 6520 6c6f 7765 7220 6e27 0a64  o the lower n'.d
-0000e490: 6566 2058 6964 5365 7269 6573 4c6f 7765  ef XidSeriesLowe
-0000e4a0: 7228 6e2c 206d 2c20 702c 2071 2c20 6e70  r(n, m, p, q, np
-0000e4b0: 726d 2c20 6d70 726d 293a 0a20 2020 2069  rm, mprm):.    i
-0000e4c0: 6620 6e70 726d 203e 3d20 333a 0a20 2020  f nprm >= 3:.   
-0000e4d0: 2020 2020 2067 6d61 785f 6c20 3d20 666c       gmax_l = fl
-0000e4e0: 6f6f 7228 286e 7072 6d2d 6162 7328 6d70  oor((nprm-abs(mp
-0000e4f0: 726d 2929 2f32 290a 2020 2020 656c 7365  rm))/2).    else
-0000e500: 3a0a 2020 2020 2020 2020 676d 6178 5f6c  :.        gmax_l
-0000e510: 203d 2030 0a20 2020 2074 6869 734c 6f77   = 0.    thisLow
-0000e520: 6572 203d 2030 0a20 2020 2066 6f72 2067  er = 0.    for g
-0000e530: 2069 6e20 7261 6e67 6528 312c 676d 6178   in range(1,gmax
-0000e540: 5f6c 2b31 293a 0a20 2020 2020 2020 2074  _l+1):.        t
-0000e550: 6869 7350 726f 6420 3d20 310a 2020 2020  hisProd = 1.    
-0000e560: 2020 2020 666f 7220 6b61 7020 696e 2072      for kap in r
-0000e570: 616e 6765 2867 293a 0a20 2020 2020 2020  ange(g):.       
-0000e580: 2020 2020 2074 6869 7350 726f 6420 3d20       thisProd = 
-0000e590: 7468 6973 5072 6f64 202a 2046 5f4d 286e  thisProd * F_M(n
-0000e5a0: 7072 6d2c 6d70 726d 2c32 2a6b 6170 290a  prm,mprm,2*kap).
-0000e5b0: 0a20 2020 2020 2020 2074 6869 734c 6f77  .        thisLow
-0000e5c0: 6572 203d 2074 6869 734c 6f77 6572 202b  er = thisLower +
-0000e5d0: 2063 616c 635f 5869 7728 6e2c 206d 2c20   calc_Xiw(n, m, 
-0000e5e0: 702c 2071 2c20 6e70 726d 2d32 2a67 2c20  p, q, nprm-2*g, 
-0000e5f0: 6d70 726d 292a 7468 6973 5072 6f64 0a0a  mprm)*thisProd..
-0000e600: 2020 2020 7365 7269 6573 4c6f 7765 7220      seriesLower 
-0000e610: 3d20 7468 6973 4c6f 7765 720a 2020 2020  = thisLower.    
-0000e620: 7265 7475 726e 2073 6572 6965 734c 6f77  return seriesLow
-0000e630: 6572 0a0a 2320 4e6f 7465 2074 6861 7420  er..# Note that 
-0000e640: 616c 7468 6f75 6768 2074 6869 7320 7465  although this te
-0000e650: 726d 2069 7320 6361 6c6c 6564 2053 6572  rm is called Ser
-0000e660: 6965 7355 7070 6572 2c20 6974 2063 6f6e  iesUpper, it con
-0000e670: 7461 696e 7320 6d69 7869 6e67 2074 6572  tains mixing ter
-0000e680: 6d73 2066 726f 6d20 6c6f 7765 7220 6465  ms from lower de
-0000e690: 6772 6565 206e 2727 2069 6e74 6f20 7468  gree n'' into th
-0000e6a0: 6520 6869 6768 6572 206e 270a 6465 6620  e higher n'.def 
-0000e6b0: 5869 6453 6572 6965 7355 7070 6572 286e  XidSeriesUpper(n
-0000e6c0: 2c20 6d2c 2070 2c20 712c 206e 7072 6d2c  , m, p, q, nprm,
-0000e6d0: 206d 7072 6d2c 206e 7072 6d5f 6d61 7829   mprm, nprm_max)
-0000e6e0: 3a0a 2020 2020 676d 6178 5f75 203d 2066  :.    gmax_u = f
-0000e6f0: 6c6f 6f72 2828 6e70 726d 5f6d 6178 2d6e  loor((nprm_max-n
-0000e700: 7072 6d29 2f32 290a 2020 2020 7468 6973  prm)/2).    this
-0000e710: 5570 7065 7220 3d20 300a 2020 2020 666f  Upper = 0.    fo
-0000e720: 7220 6720 696e 2072 616e 6765 2831 2c67  r g in range(1,g
-0000e730: 6d61 785f 752b 3129 3a0a 2020 2020 2020  max_u+1):.      
-0000e740: 2020 7468 6973 5072 6f64 203d 2031 0a20    thisProd = 1. 
-0000e750: 2020 2020 2020 2066 6f72 206b 6170 2069         for kap i
-0000e760: 6e20 7261 6e67 6528 6729 3a0a 2020 2020  n range(g):.    
-0000e770: 2020 2020 2020 2020 7468 6973 5072 6f64          thisProd
-0000e780: 203d 2074 6869 7350 726f 6420 2a20 465f   = thisProd * F_
-0000e790: 5028 6e70 726d 2c6d 7072 6d2c 322a 6b61  P(nprm,mprm,2*ka
-0000e7a0: 702c 6e70 726d 5f6d 6178 290a 0a20 2020  p,nprm_max)..   
-0000e7b0: 2020 2020 2074 6869 7355 7070 6572 203d       thisUpper =
-0000e7c0: 2074 6869 7355 7070 6572 202b 2063 616c   thisUpper + cal
-0000e7d0: 635f 5869 7728 6e2c 206d 2c20 702c 2071  c_Xiw(n, m, p, q
-0000e7e0: 2c20 6e70 726d 2b32 2a67 2c20 6d70 726d  , nprm+2*g, mprm
-0000e7f0: 292a 7468 6973 5072 6f64 0a0a 2020 2020  )*thisProd..    
-0000e800: 7365 7269 6573 5570 7065 7220 3d20 7468  seriesUpper = th
-0000e810: 6973 5570 7065 720a 2020 2020 7265 7475  isUpper.    retu
-0000e820: 726e 2073 6572 6965 7355 7070 6572 0a0a  rn seriesUpper..
-0000e830: 6465 6620 5869 6444 656e 6f6d 286e 2c20  def XidDenom(n, 
-0000e840: 6d2c 206e 7072 6d5f 6d61 7829 3a0a 2020  m, nprm_max):.  
-0000e850: 2020 5869 6444 656e 6f6d 203d 2077 5f4d    XidDenom = w_M
-0000e860: 286e 2c6d 292a 2a32 202b 2077 5f50 286e  (n,m)**2 + w_P(n
-0000e870: 2c6d 292a 2a32 202d 2077 5f4d 286e 2c6d  ,m)**2 - w_M(n,m
-0000e880: 292a 775f 5028 6e2d 322c 6d29 2a46 5f4d  )*w_P(n-2,m)*F_M
-0000e890: 286e 2c6d 2c30 2920 2d20 775f 5028 6e2c  (n,m,0) - w_P(n,
-0000e8a0: 6d29 2a77 5f4d 286e 2b32 2c6d 292a 465f  m)*w_M(n+2,m)*F_
-0000e8b0: 5028 6e2c 6d2c 302c 6e70 726d 5f6d 6178  P(n,m,0,nprm_max
-0000e8c0: 290a 2020 2020 7265 7475 726e 2058 6964  ).    return Xid
-0000e8d0: 4465 6e6f 6d0a 0a23 2323 2323 2323 2323  Denom..#########
-0000e8e0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0000e8f0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0000e900: 2323 2323 0a23 202d 2d20 454e 4420 5245  ####.# -- END RE
-0000e910: 5645 5253 4544 206e 2c20 6e27 204e 4f54  VERSED n, n' NOT
-0000e920: 4154 494f 4e20 2d2d 0a23 2323 2323 2323  ATION --.#######
-0000e930: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0000e940: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0000e950: 2323 2323 2323 0a0a 2222 220a 6576 616c  ######..""".eval
-0000e960: 5f64 6576 2829 0a20 2020 2045 7661 6c75  _dev().    Evalu
-0000e970: 6174 6573 2074 6865 2064 6576 6961 7469  ates the deviati
-0000e980: 6f6e 2066 726f 6d20 7370 6865 7269 6361  on from spherica
-0000e990: 6c20 7379 6d6d 6574 7279 2061 7320 6120  l symmetry as a 
-0000e9a0: 6675 6e63 7469 6f6e 206f 6620 6c61 742f  function of lat/
-0000e9b0: 6c6f 6e20 666f 7220 6120 6769 7665 6e20  lon for a given 
-0000e9c0: 6465 6772 6565 2070 2061 6e64 206f 7264  degree p and ord
-0000e9d0: 6572 2071 206f 6620 626f 756e 6461 7279  er q of boundary
-0000e9e0: 2073 6861 7065 2e0a 2020 2020 5661 6c75   shape..    Valu
-0000e9f0: 6573 2066 6f72 2063 6869 5f70 7120 6172  es for chi_pq ar
-0000ea00: 6520 636f 6566 6669 6369 656e 7473 2074  e coefficients t
-0000ea10: 6861 7420 6d75 6c74 6970 6c79 2074 6865  hat multiply the
-0000ea20: 2061 7373 6f63 6961 7465 6420 6f72 7468   associated orth
-0000ea30: 6f6e 6f72 6d61 6c20 7370 6865 7269 6361  onormal spherica
-0000ea40: 6c20 6861 726d 6f6e 6963 2061 6e64 2074  l harmonic and t
-0000ea50: 6865 6e0a 2020 2020 6172 6520 6164 6465  hen.    are adde
-0000ea60: 6420 746f 2074 6865 206e 6f6d 696e 616c  d to the nominal
-0000ea70: 2072 6164 6975 732e 2052 6574 7572 6e73   radius. Returns
-0000ea80: 2073 616d 6520 756e 6974 7320 6173 2069   same units as i
-0000ea90: 6e70 7574 2063 6869 5f70 712e 0a20 2020  nput chi_pq..   
-0000eaa0: 2055 7361 6765 3a20 6074 6869 735f 6465   Usage: `this_de
-0000eab0: 7673 6020 3d20 6576 616c 5f64 6576 2860  vs` = eval_dev(`
-0000eac0: 7060 2c20 6071 602c 2060 6368 695f 7071  p`, `q`, `chi_pq
-0000ead0: 602c 2060 6c74 6874 602c 2060 6c70 6869  `, `ltht`, `lphi
-0000eae0: 602c 2060 6c6c 656e 7960 2c20 606c 6c65  `, `lleny`, `lle
-0000eaf0: 6e78 6029 0a20 2020 2052 6574 7572 6e73  nx`).    Returns
-0000eb00: 3a0a 2020 2020 2020 2020 7468 6973 5f64  :.        this_d
-0000eb10: 6576 733a 2066 6c6f 6174 2c20 7368 6170  evs: float, shap
-0000eb20: 6528 6c6c 656e 792c 6c6c 656e 7829 2e20  e(lleny,llenx). 
-0000eb30: 426f 756e 6461 7279 2073 6861 7065 2064  Boundary shape d
-0000eb40: 6576 6961 7469 6f6e 7320 6475 6520 746f  eviations due to
-0000eb50: 2074 6869 7320 7061 7274 6963 756c 6172   this particular
-0000eb60: 2070 2c71 2063 6f6d 6269 6e61 7469 6f6e   p,q combination
-0000eb70: 2e0a 2020 2020 5061 7261 6d65 7465 7273  ..    Parameters
-0000eb80: 3a0a 2020 2020 2020 2020 703a 2069 6e74  :.        p: int
-0000eb90: 6567 6572 2e20 4465 6772 6565 206f 6620  eger. Degree of 
-0000eba0: 7368 6170 6520 6861 726d 6f6e 6963 2074  shape harmonic t
-0000ebb0: 6f20 6265 2065 7661 6c75 6174 6564 2e0a  o be evaluated..
-0000ebc0: 2020 2020 2020 2020 713a 2069 6e74 6567          q: integ
-0000ebd0: 6572 2e20 4f72 6465 7220 6f66 2073 6861  er. Order of sha
-0000ebe0: 7065 2068 6172 6d6f 6e69 6320 746f 2062  pe harmonic to b
-0000ebf0: 6520 6576 616c 7561 7465 642e 0a20 2020  e evaluated..   
-0000ec00: 2020 2020 2063 6869 5f70 713a 2063 6f6d       chi_pq: com
-0000ec10: 706c 6578 2e20 436f 6566 6669 6369 656e  plex. Coefficien
-0000ec20: 7420 666f 7220 7370 6865 7269 6361 6c20  t for spherical 
-0000ec30: 6861 726d 6f6e 6963 7320 6f66 2064 6567  harmonics of deg
-0000ec40: 7265 6520 616e 6420 6f72 6465 7220 702c  ree and order p,
-0000ec50: 712c 0a20 2020 2020 2020 2020 2020 2073  q,.            s
-0000ec60: 7563 6820 7468 6174 2072 2874 6865 7461  uch that r(theta
-0000ec70: 2c20 7068 6929 203d 2052 202b 2053 756d  , phi) = R + Sum
-0000ec80: 5b63 6869 5f70 7120 2a20 5970 7128 7468  [chi_pq * Ypq(th
-0000ec90: 6574 612c 2070 6869 295d 2e0a 2020 2020  eta, phi)]..    
-0000eca0: 2020 2020 6c74 6874 3a20 666c 6f61 742c      ltht: float,
-0000ecb0: 2073 6861 7065 286c 6c65 6e79 292e 204c   shape(lleny). L
-0000ecc0: 6f63 616c 2063 6f70 7920 6f66 2074 6865  ocal copy of the
-0000ecd0: 7461 2067 7269 6420 7661 6c75 6573 2028  ta grid values (
-0000ece0: 6661 7374 6572 2065 7865 6375 7469 6f6e  faster execution
-0000ecf0: 2074 6861 6e20 7265 6665 7265 6e63 696e   than referencin
-0000ed00: 6720 6120 676c 6f62 616c 2076 6172 6961  g a global varia
-0000ed10: 626c 6529 2e0a 2020 2020 2020 2020 6c70  ble)..        lp
-0000ed20: 6869 3a20 666c 6f61 742c 2073 6861 7065  hi: float, shape
-0000ed30: 286c 6c65 6e79 292e 204c 6f63 616c 2063  (lleny). Local c
-0000ed40: 6f70 7920 6f66 2070 6869 2067 7269 6420  opy of phi grid 
-0000ed50: 7661 6c75 6573 2e0a 2020 2020 2020 2020  values..        
-0000ed60: 6c6c 656e 793a 2069 6e74 6567 6572 2e20  lleny: integer. 
-0000ed70: 4c6f 6361 6c20 636f 7079 206f 6620 6c65  Local copy of le
-0000ed80: 6e79 2c20 7468 6520 6e75 6d62 6572 206f  ny, the number o
-0000ed90: 6620 7920 2874 6865 7461 2920 6772 6964  f y (theta) grid
-0000eda0: 2076 616c 7565 732e 2050 6173 7365 6420   values. Passed 
-0000edb0: 746f 2061 766f 6964 2072 6570 6561 7465  to avoid repeate
-0000edc0: 6420 6361 6c6c 7320 696e 2070 6172 616c  d calls in paral
-0000edd0: 6c65 6c20 6578 6563 7574 696f 6e2e 0a20  lel execution.. 
-0000ede0: 2020 2020 2020 206c 6c65 6e78 3a20 696e         llenx: in
-0000edf0: 7465 6765 722e 204c 6f63 616c 2063 6f70  teger. Local cop
-0000ee00: 7920 6f66 206c 656e 782c 2074 6865 206e  y of lenx, the n
-0000ee10: 756d 6265 7220 6f66 2078 2028 7068 6929  umber of x (phi)
-0000ee20: 2067 7269 6420 7661 6c75 6573 2e0a 2020   grid values..  
-0000ee30: 2020 2222 220a 6465 6620 6576 616c 5f64    """.def eval_d
-0000ee40: 6576 2870 2c20 712c 2063 6869 5f70 712c  ev(p, q, chi_pq,
-0000ee50: 206c 7468 742c 206c 7068 692c 206c 6c65   ltht, lphi, lle
-0000ee60: 6e79 2c20 6c6c 656e 7829 3a0a 2020 2020  ny, llenx):.    
-0000ee70: 6966 2063 6869 5f70 7120 3d3d 2030 3a0a  if chi_pq == 0:.
-0000ee80: 2020 2020 2020 2020 7468 6973 5f64 6576          this_dev
-0000ee90: 7320 3d20 6e70 2e7a 6572 6f73 2828 6c6c  s = np.zeros((ll
-0000eea0: 656e 792c 6c6c 656e 7829 2c20 6474 7970  eny,llenx), dtyp
-0000eeb0: 653d 6e70 2e66 6c6f 6174 5f29 0a20 2020  e=np.float_).   
-0000eec0: 2065 6c73 653a 0a20 2020 2020 2020 2074   else:.        t
-0000eed0: 6869 735f 6465 7673 203d 206e 702e 6172  his_devs = np.ar
-0000eee0: 7261 7928 5b20 6e70 2e72 6561 6c28 2063  ray([ np.real( c
-0000eef0: 6869 5f70 712a 636f 6d70 6c65 7828 6d70  hi_pq*complex(mp
-0000ef00: 2e73 7068 6572 6861 726d 2870 2c71 2c74  .spherharm(p,q,t
-0000ef10: 6874 692c 7068 6969 2929 2029 2066 6f72  hti,phii)) ) for
-0000ef20: 2074 6874 6920 696e 206c 7468 7420 666f   thti in ltht fo
-0000ef30: 7220 7068 6969 2069 6e20 6c70 6869 205d  r phii in lphi ]
-0000ef40: 290a 2020 2020 2020 2020 7468 6973 5f64  ).        this_d
-0000ef50: 6576 7320 3d20 6e70 2e72 6573 6861 7065  evs = np.reshape
-0000ef60: 2874 6869 735f 6465 7673 2c28 6c6c 656e  (this_devs,(llen
-0000ef70: 792c 6c6c 656e 7829 290a 2020 2020 6c6f  y,llenx)).    lo
-0000ef80: 672e 6465 6275 6728 6622 702c 7120 3d20  g.debug(f"p,q = 
-0000ef90: 7b70 7d7b 717d 2063 6f6d 706c 6574 6564  {p}{q} completed
-0000efa0: 2229 0a20 2020 2072 6574 7572 6e20 7468  ").    return th
-0000efb0: 6973 5f64 6576 730a 0a23 2323 2323 2323  is_devs..#######
-0000efc0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0000efd0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0000efe0: 2323 2323 2323 0a0a 2222 220a 6765 745f  ######..""".get_
-0000eff0: 7273 7572 6628 290a 2020 2020 4361 6c63  rsurf().    Calc
-0000f000: 756c 6174 6573 2072 2874 6865 7461 2c20  ulates r(theta, 
-0000f010: 7068 6929 2066 726f 6d20 725f 6d65 616e  phi) from r_mean
-0000f020: 2061 6e64 2063 6869 5f70 712c 2077 6865   and chi_pq, whe
-0000f030: 7265 2072 2874 6865 7461 2c20 7068 6929  re r(theta, phi)
-0000f040: 203d 2072 5f6d 6561 6e20 2b20 5375 6d5b   = r_mean + Sum[
-0000f050: 6368 695f 7071 2a59 7071 2874 6865 7461  chi_pq*Ypq(theta
-0000f060: 2c20 7068 6929 5d2e 0a20 2020 2055 7361  , phi)]..    Usa
-0000f070: 6765 3a20 6765 745f 7273 7572 6628 6042  ge: get_rsurf(`B
-0000f080: 696e 6d60 2c20 606e 5f6d 6178 602c 2060  inm`, `n_max`, `
-0000f090: 6670 6174 683d 4e6f 6e65 602c 2060 6469  fpath=None`, `di
-0000f0a0: 6666 6572 656e 6365 3d54 7275 6560 2c20  fference=True`, 
-0000f0b0: 6042 696e 6d5f 7370 683d 4e6f 6e65 6029  `Binm_sph=None`)
-0000f0c0: 0a20 2020 2052 6574 7572 6e73 3a0a 2020  .    Returns:.  
-0000f0d0: 2020 2020 2020 7375 7266 3a20 666c 6f61        surf: floa
-0000f0e0: 742c 2073 6861 7065 286c 6c65 6e79 2c6c  t, shape(lleny,l
-0000f0f0: 6c65 6e78 292e 2072 2874 6865 7461 2c20  lenx). r(theta, 
-0000f100: 7068 6929 2076 616c 7565 7320 636f 7272  phi) values corr
-0000f110: 6573 706f 6e64 696e 6720 746f 2074 6865  esponding to the
-0000f120: 2069 6e70 7574 2067 7269 6420 6f66 0a20   input grid of. 
-0000f130: 2020 2020 2020 2020 2020 206c 7468 7420             ltht 
-0000f140: 616e 6420 6c70 6869 2076 616c 7565 732e  and lphi values.
-0000f150: 2053 616d 6520 756e 6974 7320 6173 2061   Same units as a
-0000f160: 7379 6d5f 7368 6170 6520 616e 6420 725f  sym_shape and r_
-0000f170: 6d65 616e 2e0a 2020 2020 5061 7261 6d65  mean..    Parame
-0000f180: 7465 7273 3a0a 2020 2020 2020 2020 7076  ters:.        pv
-0000f190: 616c 732c 2071 7661 6c73 3a20 696e 7465  als, qvals: inte
-0000f1a0: 6765 722c 2073 6861 7065 284e 7071 292e  ger, shape(Npq).
-0000f1b0: 204c 696e 6561 7220 6172 7261 7973 206f   Linear arrays o
-0000f1c0: 6620 7061 6972 6564 2070 2c71 2076 616c  f paired p,q val
-0000f1d0: 7565 7320 666f 7220 7061 7261 6c6c 656c  ues for parallel
-0000f1e0: 2063 6f6d 7075 7461 7469 6f6e 2e0a 2020   computation..  
-0000f1f0: 2020 2020 2020 6173 796d 5f73 6861 7065        asym_shape
-0000f200: 3a20 636f 6d70 6c65 782c 2073 6861 7065  : complex, shape
-0000f210: 2832 2c70 5f6d 6178 2b31 2c70 5f6d 6178  (2,p_max+1,p_max
-0000f220: 2b31 292e 2041 6273 6f6c 7574 6520 626f  +1). Absolute bo
-0000f230: 756e 6461 7279 2064 6576 6961 7469 6f6e  undary deviation
-0000f240: 7320 666f 7220 616c 6c20 702c 7120 7661  s for all p,q va
-0000f250: 6c75 6573 2066 6f72 2074 6865 0a20 2020  lues for the.   
-0000f260: 2020 2020 2020 2020 2063 6f6e 7369 6465           conside
-0000f270: 7265 6420 7375 7266 6163 652e 2055 6e69  red surface. Uni
-0000f280: 7473 206d 7573 7420 6d61 7463 6820 725f  ts must match r_
-0000f290: 6d65 616e 2e0a 2020 2020 2020 2020 725f  mean..        r_
-0000f2a0: 6d65 616e 3a20 666c 6f61 742e 204d 6561  mean: float. Mea
-0000f2b0: 6e20 7661 6c75 6520 6f66 2072 6164 6975  n value of radiu
-0000f2c0: 7320 666f 7220 7468 6520 636f 6e73 6964  s for the consid
-0000f2d0: 6572 6564 2073 7572 6661 6365 2e20 556e  ered surface. Un
-0000f2e0: 6974 7320 6d75 7374 206d 6174 6368 2061  its must match a
-0000f2f0: 7379 6d5f 7368 6170 652e 0a20 2020 2020  sym_shape..     
-0000f300: 2020 206c 7468 743a 2066 6c6f 6174 2c20     ltht: float, 
-0000f310: 7368 6170 6528 6c6c 656e 7929 2e20 4c6f  shape(lleny). Lo
-0000f320: 6361 6c20 636f 7079 206f 6620 7468 6574  cal copy of thet
-0000f330: 6120 6772 6964 2076 616c 7565 7320 2866  a grid values (f
-0000f340: 6173 7465 7220 6578 6563 7574 696f 6e20  aster execution 
-0000f350: 7468 616e 2072 6566 6572 656e 6369 6e67  than referencing
-0000f360: 2061 2067 6c6f 6261 6c20 7661 7269 6162   a global variab
-0000f370: 6c65 292e 0a20 2020 2020 2020 206c 7068  le)..        lph
-0000f380: 693a 2066 6c6f 6174 2c20 7368 6170 6528  i: float, shape(
-0000f390: 6c6c 656e 7929 2e20 4c6f 6361 6c20 636f  lleny). Local co
-0000f3a0: 7079 206f 6620 7068 6920 6772 6964 2076  py of phi grid v
-0000f3b0: 616c 7565 732e 0a20 2020 2022 2222 0a64  alues..    """.d
-0000f3c0: 6566 2067 6574 5f72 7375 7266 2870 7661  ef get_rsurf(pva
-0000f3d0: 6c73 2c71 7661 6c73 2c61 7379 6d5f 7368  ls,qvals,asym_sh
-0000f3e0: 6170 652c 2072 5f6d 6561 6e2c 6c74 6874  ape, r_mean,ltht
-0000f3f0: 2c6c 7068 692c 2064 6f5f 7061 7261 6c6c  ,lphi, do_parall
-0000f400: 656c 3d54 7275 6529 3a0a 2020 2020 4e70  el=True):.    Np
-0000f410: 7120 3d20 6e70 2e73 697a 6528 7076 616c  q = np.size(pval
-0000f420: 7329 0a20 2020 206c 6c65 6e79 203d 206e  s).    lleny = n
-0000f430: 702e 7369 7a65 286c 7468 7429 0a20 2020  p.size(ltht).   
-0000f440: 206c 6c65 6e78 203d 206e 702e 7369 7a65   llenx = np.size
-0000f450: 286c 7068 6929 0a20 2020 2064 6576 7320  (lphi).    devs 
-0000f460: 3d20 6e70 2e7a 6572 6f73 2828 6c6c 656e  = np.zeros((llen
-0000f470: 792c 6c6c 656e 7829 290a 0a20 2020 206c  y,llenx))..    l
-0000f480: 696e 5f62 645f 7368 6170 6520 3d20 6e70  in_bd_shape = np
-0000f490: 2e61 7272 6179 285b 2061 7379 6d5f 7368  .array([ asym_sh
-0000f4a0: 6170 655b 696e 7428 7176 616c 735b 694e  ape[int(qvals[iN
-0000f4b0: 5d3c 3029 2c70 7661 6c73 5b69 4e5d 2c61  ]<0),pvals[iN],a
-0000f4c0: 6273 2871 7661 6c73 5b69 4e5d 295d 2066  bs(qvals[iN])] f
-0000f4d0: 6f72 2069 4e20 696e 2072 616e 6765 284e  or iN in range(N
-0000f4e0: 7071 2920 5d29 0a0a 2020 2020 6966 2064  pq) ])..    if d
-0000f4f0: 6f5f 7061 7261 6c6c 656c 3a0a 2020 2020  o_parallel:.    
-0000f500: 2020 2020 706f 6f6c 203d 206d 7470 436f      pool = mtpCo
-0000f510: 6e74 6578 742e 506f 6f6c 286e 756d 5f63  ntext.Pool(num_c
-0000f520: 6f72 6573 290a 2020 2020 2020 2020 7061  ores).        pa
-0000f530: 725f 7265 7375 6c74 203d 205b 706f 6f6c  r_result = [pool
-0000f540: 2e61 7070 6c79 5f61 7379 6e63 2820 6576  .apply_async( ev
-0000f550: 616c 5f64 6576 2c20 6172 6773 3d28 7076  al_dev, args=(pv
-0000f560: 616c 735b 694e 5d2c 7176 616c 735b 694e  als[iN],qvals[iN
-0000f570: 5d2c 6c69 6e5f 6264 5f73 6861 7065 5b69  ],lin_bd_shape[i
-0000f580: 4e5d 2c6c 7468 742c 6c70 6869 2c6c 6c65  N],ltht,lphi,lle
-0000f590: 6e79 2c6c 6c65 6e78 2920 2920 666f 7220  ny,llenx) ) for 
-0000f5a0: 694e 2069 6e20 7261 6e67 6528 4e70 7129  iN in range(Npq)
-0000f5b0: 5d0a 2020 2020 2020 2020 706f 6f6c 2e63  ].        pool.c
-0000f5c0: 6c6f 7365 2829 0a20 2020 2020 2020 2070  lose().        p
-0000f5d0: 6f6f 6c2e 6a6f 696e 2829 0a0a 2020 2020  ool.join()..    
-0000f5e0: 2020 2020 2320 556e 7061 636b 2074 6865      # Unpack the
-0000f5f0: 2070 6172 616c 6c65 6c20 7072 6f63 6573   parallel proces
-0000f600: 7369 6e67 2072 6573 756c 7473 2061 6e64  sing results and
-0000f610: 2073 756d 2074 6865 6d20 746f 6765 7468   sum them togeth
-0000f620: 6572 0a20 2020 2020 2020 2066 6f72 2072  er.        for r
-0000f630: 6573 2069 6e20 7061 725f 7265 7375 6c74  es in par_result
-0000f640: 3a0a 2020 2020 2020 2020 2020 2020 6465  :.            de
-0000f650: 7673 203d 2064 6576 7320 2b20 7265 732e  vs = devs + res.
-0000f660: 6765 7428 290a 2020 2020 656c 7365 3a0a  get().    else:.
-0000f670: 2020 2020 2020 2020 666f 7220 694e 2069          for iN i
-0000f680: 6e20 7261 6e67 6528 4e70 7129 3a0a 2020  n range(Npq):.  
-0000f690: 2020 2020 2020 2020 2020 6465 7673 203d            devs =
-0000f6a0: 2064 6576 7320 2b20 6576 616c 5f64 6576   devs + eval_dev
-0000f6b0: 2870 7661 6c73 5b69 4e5d 2c71 7661 6c73  (pvals[iN],qvals
-0000f6c0: 5b69 4e5d 2c6c 696e 5f62 645f 7368 6170  [iN],lin_bd_shap
-0000f6d0: 655b 694e 5d2c 6c74 6874 2c6c 7068 692c  e[iN],ltht,lphi,
-0000f6e0: 6c6c 656e 792c 6c6c 656e 7829 0a0a 2020  lleny,llenx)..  
-0000f6f0: 2020 7375 7266 203d 2064 6576 7320 2b20    surf = devs + 
-0000f700: 725f 6d65 616e 0a20 2020 2072 6574 7572  r_mean.    retur
-0000f710: 6e20 7375 7266 0a0a 2323 2323 2323 2323  n surf..########
-0000f720: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0000f730: 2323 2323 2323 2323 2323 2323 2323 2323  ################
-0000f740: 2323 2323 230a 0a22 2222 0a67 6574 4d61  #####..""".getMa
-0000f750: 6753 7572 6628 290a 2020 2020 4576 616c  gSurf().    Eval
-0000f760: 7561 7465 7320 7468 6520 696e 6475 6365  uates the induce
-0000f770: 6420 6d61 676e 6574 6963 2066 6965 6c64  d magnetic field
-0000f780: 2061 7420 7468 6520 7375 7266 6163 6520   at the surface 
-0000f790: 666f 7220 616c 6c20 6d61 676e 6574 6963  for all magnetic
-0000f7a0: 206d 6f6d 656e 7473 2042 696e 6d2e 0a20   moments Binm.. 
-0000f7b0: 2020 2055 7361 6765 3a20 6042 7860 2c20     Usage: `Bx`, 
-0000f7c0: 6042 7960 2c20 6042 7a60 203d 2067 6574  `By`, `Bz` = get
-0000f7d0: 4d61 6753 7572 6628 606e 7661 6c73 602c  MagSurf(`nvals`,
-0000f7e0: 2060 6d76 616c 7360 2c20 6042 696e 6d60   `mvals`, `Binm`
-0000f7f0: 2c20 6072 5f74 685f 7068 602c 2060 6c74  , `r_th_ph`, `lt
-0000f800: 6874 602c 2060 6c70 6869 602c 2060 6e6d  ht`, `lphi`, `nm
-0000f810: 6178 5f70 6c6f 743d 3460 2c20 6053 6368  ax_plot=4`, `Sch
-0000f820: 6d69 6474 3d46 616c 7365 6029 0a20 2020  midt=False`).   
-0000f830: 2052 6574 7572 6e73 3a0a 2020 2020 2020   Returns:.      
-0000f840: 2020 4278 2c42 792c 427a 2028 6561 6368    Bx,By,Bz (each
-0000f850: 293a 2063 6f6d 706c 6578 2c20 7368 6170  ): complex, shap
-0000f860: 6528 6c6c 656e 792c 6c6c 656e 7829 2e20  e(lleny,llenx). 
-0000f870: 4120 286c 6c65 6e79 2c6c 6c65 6e78 2920  A (lleny,llenx) 
-0000f880: 6172 7261 7920 6f66 2066 6965 6c64 2076  array of field v
-0000f890: 616c 7565 7320 6475 6520 746f 2074 6865  alues due to the
-0000f8a0: 2070 6172 7469 6375 6c61 7220 4269 6e6d   particular Binm
-0000f8b0: 2076 616c 7565 7320 7061 7373 6564 2e0a   values passed..
-0000f8c0: 2020 2020 2020 2020 2020 2020 4669 656c              Fiel
-0000f8d0: 6420 7661 6c75 6573 2063 616e 2062 6520  d values can be 
-0000f8e0: 6f62 7461 696e 6564 2066 6f72 2061 6e79  obtained for any
-0000f8f0: 2066 7574 7572 6520 7469 6d65 2062 7920   future time by 
-0000f900: 6d75 6c74 6970 6c79 696e 6720 6561 6368  multiplying each
-0000f910: 2042 696e 6d5b 692c 3a2c 3a2c 3a5d 2062   Binm[i,:,:,:] b
-0000f920: 7920 7468 6520 636f 7272 6573 706f 6e64  y the correspond
-0000f930: 696e 6720 655e 2d69 cf89 7420 6661 6374  ing e^-i..t fact
-0000f940: 6f72 2e0a 2020 2020 2020 2020 2020 2020  or..            
-0000f950: 743d 3020 6973 2064 6566 696e 6564 2074  t=0 is defined t
-0000f960: 6f20 6265 2074 6865 204a 3230 3030 2065  o be the J2000 e
-0000f970: 706f 6368 2e0a 2020 2020 5061 7261 6d65  poch..    Parame
-0000f980: 7465 7273 3a0a 2020 2020 2020 2020 6e76  ters:.        nv
-0000f990: 616c 733a 2069 6e74 6567 6572 2c20 7368  als: integer, sh
-0000f9a0: 6170 6528 4e6e 6d29 2e20 4c69 6e65 6172  ape(Nnm). Linear
-0000f9b0: 206c 6973 7420 6f66 206d 6167 6e65 7469   list of magneti
-0000f9c0: 6320 6d6f 6d65 6e74 2064 6567 7265 6573  c moment degrees
-0000f9d0: 2074 6f20 6265 2065 7661 6c75 6174 6564   to be evaluated
-0000f9e0: 2e0a 2020 2020 2020 2020 6d76 616c 733a  ..        mvals:
-0000f9f0: 2069 6e74 6567 6572 2c20 7368 6170 6528   integer, shape(
-0000fa00: 4e6e 6d29 2e20 4c69 6e65 6172 206c 6973  Nnm). Linear lis
-0000fa10: 7420 6f66 206d 6167 6e65 7469 6320 6d6f  t of magnetic mo
-0000fa20: 6d65 6e74 206f 7264 6572 7320 746f 2062  ment orders to b
-0000fa30: 6520 6576 616c 7561 7465 642c 2063 6f72  e evaluated, cor
-0000fa40: 7265 7370 6f6e 6469 6e67 2074 6f20 6e76  responding to nv
-0000fa50: 616c 7320 6f66 2074 6865 2073 616d 6520  als of the same 
-0000fa60: 696e 6465 782e 0a20 2020 2020 2020 2042  index..        B
-0000fa70: 696e 6d3a 2063 6f6d 706c 6578 2c20 7368  inm: complex, sh
-0000fa80: 6170 6528 322c 6e5f 6d61 782b 312c 6e5f  ape(2,n_max+1,n_
-0000fa90: 6d61 782b 3129 204f 5220 7368 6170 6528  max+1) OR shape(
-0000faa0: 4e6e 6d29 3b20 6966 2053 6368 6d69 6474  Nnm); if Schmidt
-0000fab0: 3d54 7275 652c 2074 7570 6c65 206f 6620  =True, tuple of 
-0000fac0: 2867 6e6d 2c68 6e6d 292e 204d 6167 6e65  (gnm,hnm). Magne
-0000fad0: 7469 6320 6d6f 6d65 6e74 206f 6620 6465  tic moment of de
-0000fae0: 6772 6565 2061 6e64 0a20 2020 2020 2020  gree and.       
-0000faf0: 2020 2020 206f 7264 6572 206e 2c6d 2074       order n,m t
-0000fb00: 6861 7420 6361 6e20 6265 2069 6e64 6578  hat can be index
-0000fb10: 6564 2062 7920 7468 6520 6d61 7463 6865  ed by the matche
-0000fb20: 6420 656e 7472 6965 7320 696e 206e 7661  d entries in nva
-0000fb30: 6c73 2061 6e64 206d 7661 6c73 2e20 556e  ls and mvals. Un
-0000fb40: 6974 7320 6d61 7463 6820 7468 6520 6f75  its match the ou
-0000fb50: 7470 7574 2066 6965 6c64 2e0a 2020 2020  tput field..    
-0000fb60: 2020 2020 725f 7468 5f70 683a 2066 6c6f      r_th_ph: flo
-0000fb70: 6174 2c20 7368 6170 6528 6c6c 656e 792c  at, shape(lleny,
-0000fb80: 6c6c 656e 7829 2e20 4d65 7368 6772 6964  llenx). Meshgrid
-0000fb90: 2061 7272 6179 206f 6620 7228 7468 6574   array of r(thet
-0000fba0: 612c 2070 6869 2920 7661 6c75 6573 2063  a, phi) values c
-0000fbb0: 6f72 7265 7370 6f6e 6469 6e67 2074 6f20  orresponding to 
-0000fbc0: 7468 6520 666f 6c6c 6f77 696e 6720 7468  the following th
-0000fbd0: 7420 616e 6420 7068 6920 7661 6c75 6573  t and phi values
-0000fbe0: 2e0a 2020 2020 2020 2020 2020 2020 725f  ..            r_
-0000fbf0: 7468 5f70 6820 6861 7320 756e 6974 7320  th_ph has units 
-0000fc00: 6f66 2052 5f62 6f64 792c 2069 2e65 2e20  of R_body, i.e. 
-0000fc10: 7468 6520 7068 7973 6963 616c 2073 7572  the physical sur
-0000fc20: 6661 6365 2069 7320 312e 302e 0a20 2020  face is 1.0..   
-0000fc30: 2020 2020 206c 7468 743a 2066 6c6f 6174       ltht: float
-0000fc40: 2c20 7368 6170 6528 6c6c 656e 7929 2e20  , shape(lleny). 
-0000fc50: 4172 7261 7920 6f66 2074 6865 7461 2076  Array of theta v
-0000fc60: 616c 7565 7320 6f76 6572 2077 6869 6368  alues over which
-0000fc70: 2074 6f20 6576 616c 7561 7465 2074 6865   to evaluate the
-0000fc80: 2066 6965 6c64 2063 6f6d 706f 6e65 6e74   field component
-0000fc90: 732e 0a20 2020 2020 2020 206c 7068 693a  s..        lphi:
-0000fca0: 2066 6c6f 6174 2c20 7368 6170 6528 6c6c   float, shape(ll
-0000fcb0: 656e 7829 2e20 4172 7261 7920 6f66 2070  enx). Array of p
-0000fcc0: 6869 2076 616c 7565 7320 6f76 6572 2077  hi values over w
-0000fcd0: 6869 6368 2074 6f20 6576 616c 7561 7465  hich to evaluate
-0000fce0: 2074 6865 2066 6965 6c64 2063 6f6d 706f   the field compo
-0000fcf0: 6e65 6e74 732e 0a20 2020 2020 2020 206e  nents..        n
-0000fd00: 6d61 785f 706c 6f74 3a20 696e 7465 6765  max_plot: intege
-0000fd10: 7220 2834 292e 204d 6178 696d 756d 2076  r (4). Maximum v
-0000fd20: 616c 7565 206f 6620 6e20 666f 7220 6576  alue of n for ev
-0000fd30: 616c 7561 7469 6e67 206d 6167 6e65 7469  aluating magneti
-0000fd40: 6320 6669 656c 6473 2e20 6576 616c 5f42  c fields. eval_B
-0000fd50: 6920 6d75 7374 2068 6176 6520 6561 6368  i must have each
-0000fd60: 206e 2065 7870 6c69 6369 746c 7920 6861   n explicitly ha
-0000fd70: 7264 2d63 6f64 6564 2c0a 2020 2020 2020  rd-coded,.      
-0000fd80: 2020 2020 2020 7768 6963 6820 6861 7320        which has 
-0000fd90: 6f6e 6c79 2062 6565 6e20 646f 6e65 2075  only been done u
-0000fda0: 7020 746f 206e 3d34 2062 6563 6175 7365  p to n=4 because
-0000fdb0: 206c 6172 6765 722d 6465 6772 6565 206d   larger-degree m
-0000fdc0: 6f6d 656e 7473 2061 7265 2065 7870 6563  oments are expec
-0000fdd0: 7465 6420 746f 2068 6176 6520 736d 616c  ted to have smal
-0000fde0: 6c20 636f 6e74 7269 6275 7469 6f6e 7320  l contributions 
-0000fdf0: 6174 2061 6c74 6974 7564 652e 0a20 2020  at altitude..   
-0000fe00: 2020 2020 2053 6368 6d69 6474 3a20 626f       Schmidt: bo
-0000fe10: 6f6c 6561 6e20 2846 616c 7365 292e 2057  olean (False). W
-0000fe20: 6865 7468 6572 2069 6e70 7574 206d 6167  hether input mag
-0000fe30: 6e65 7469 6320 6d6f 6d65 6e74 7320 6172  netic moments ar
-0000fe40: 6520 696e 2053 6368 6d69 6474 2073 656d  e in Schmidt sem
-0000fe50: 692d 6e6f 726d 616c 697a 6564 2066 6f72  i-normalized for
-0000fe60: 6d20 7769 7468 6f75 7420 436f 6e64 6f6e  m without Condon
-0000fe70: 2d53 686f 7274 6c65 790a 2020 2020 2020  -Shortley.      
-0000fe80: 2020 2020 2020 7068 6173 652e 2049 6620        phase. If 
-0000fe90: 4661 6c73 652c 206d 6f6d 656e 7473 206d  False, moments m
-0000fea0: 7573 7420 6265 2069 6e20 6675 6c6c 7920  ust be in fully 
-0000feb0: 6e6f 726d 616c 697a 6564 2066 6f72 6d20  normalized form 
-0000fec0: 7769 7468 2074 6865 2043 6f6e 646f 6e2d  with the Condon-
-0000fed0: 5368 6f72 746c 6579 2070 6861 7365 2e0a  Shortley phase..
-0000fee0: 2020 2020 2020 2020 676e 6d2c 2068 6e6d          gnm, hnm
-0000fef0: 3a20 636f 6d70 6c65 782c 2073 6861 7065  : complex, shape
-0000ff00: 286e 5f6d 6178 2b31 2c6e 5f6d 6178 2b31  (n_max+1,n_max+1
-0000ff10: 292e 2053 6368 6d69 6474 2073 656d 692d  ). Schmidt semi-
-0000ff20: 6e6f 726d 616c 697a 6564 206d 6167 6e65  normalized magne
-0000ff30: 7469 6320 6d6f 6d65 6e74 732e 2050 6173  tic moments. Pas
-0000ff40: 7365 6420 6173 2061 2074 7570 6c65 2069  sed as a tuple i
-0000ff50: 6e20 4269 6e6d 2e0a 2020 2020 2222 220a  n Binm..    """.
-0000ff60: 6465 6620 6765 744d 6167 5375 7266 286e  def getMagSurf(n
-0000ff70: 7661 6c73 2c6d 7661 6c73 2c42 696e 6d2c  vals,mvals,Binm,
-0000ff80: 2072 5f74 685f 7068 2c6c 7468 742c 6c70   r_th_ph,ltht,lp
-0000ff90: 6869 2c20 6e6d 6178 5f70 6c6f 743d 3130  hi, nmax_plot=10
-0000ffa0: 2c20 5363 686d 6964 743d 4661 6c73 652c  , Schmidt=False,
-0000ffb0: 2064 6f5f 7061 7261 6c6c 656c 3d54 7275   do_parallel=Tru
-0000ffc0: 6529 3a0a 2020 2020 6966 206e 6d61 785f  e):.    if nmax_
-0000ffd0: 706c 6f74 203e 2031 303a 0a20 2020 2020  plot > 10:.     
-0000ffe0: 2020 206e 6d61 785f 706c 6f74 203d 2031     nmax_plot = 1
-0000fff0: 300a 2020 2020 2020 2020 6c6f 672e 7761  0.        log.wa
-00010000: 726e 696e 6728 6622 4576 616c 7561 7469  rning(f"Evaluati
-00010010: 6f6e 206f 6620 6d61 676e 6574 6963 2066  on of magnetic f
-00010020: 6965 6c64 7320 6973 2073 7570 706f 7274  ields is support
-00010030: 6564 206f 6e6c 7920 7570 2074 6f20 6e3d  ed only up to n=
-00010040: 7b6e 6d61 785f 706c 6f74 7d2e 206e 6d61  {nmax_plot}. nma
-00010050: 785f 706c 6f74 2068 6173 2062 6565 6e20  x_plot has been 
-00010060: 7365 7420 746f 207b 6e6d 6178 5f70 6c6f  set to {nmax_plo
-00010070: 747d 2e22 290a 0a20 2020 2069 6620 5363  t}.")..    if Sc
-00010080: 686d 6964 743a 0a20 2020 2020 2020 204e  hmidt:.        N
-00010090: 6e6d 203d 206d 696e 2820 696e 7428 286e  nm = min( int((n
-000100a0: 6d61 785f 706c 6f74 2b31 292a 286e 6d61  max_plot+1)*(nma
-000100b0: 785f 706c 6f74 2b32 292f 3229 202d 2031  x_plot+2)/2) - 1
-000100c0: 2c20 6e70 2e73 697a 6528 6e76 616c 7329  , np.size(nvals)
-000100d0: 2029 0a20 2020 2020 2020 2067 6e6d 2c20   ).        gnm, 
-000100e0: 686e 6d20 3d20 4269 6e6d 0a20 2020 2020  hnm = Binm.     
-000100f0: 2020 2069 6620 6e70 2e73 697a 6528 6e70     if np.size(np
-00010100: 2e73 6861 7065 2867 6e6d 2929 203e 2031  .shape(gnm)) > 1
-00010110: 3a0a 2020 2020 2020 2020 2020 2020 6c69  :.            li
-00010120: 6e5f 676e 6d20 3d20 6e70 2e61 7272 6179  n_gnm = np.array
-00010130: 285b 676e 6d5b 6e76 616c 735b 694e 5d2c  ([gnm[nvals[iN],
-00010140: 206d 7661 6c73 5b69 4e5d 5d20 666f 7220   mvals[iN]] for 
-00010150: 694e 2069 6e20 7261 6e67 6528 4e6e 6d29  iN in range(Nnm)
-00010160: 5d29 0a20 2020 2020 2020 2020 2020 206c  ]).            l
-00010170: 696e 5f68 6e6d 203d 206e 702e 6172 7261  in_hnm = np.arra
-00010180: 7928 5b68 6e6d 5b6e 7661 6c73 5b69 4e5d  y([hnm[nvals[iN]
-00010190: 2c20 6d76 616c 735b 694e 5d5d 2066 6f72  , mvals[iN]] for
-000101a0: 2069 4e20 696e 2072 616e 6765 284e 6e6d   iN in range(Nnm
-000101b0: 295d 290a 2020 2020 2020 2020 656c 7365  )]).        else
-000101c0: 3a0a 2020 2020 2020 2020 2020 2020 6c69  :.            li
-000101d0: 6e5f 676e 6d20 3d20 676e 6d0a 2020 2020  n_gnm = gnm.    
-000101e0: 2020 2020 2020 2020 6c69 6e5f 686e 6d20          lin_hnm 
-000101f0: 3d20 686e 6d0a 2020 2020 656c 7365 3a0a  = hnm.    else:.
-00010200: 2020 2020 2020 2020 4e6e 6d20 3d20 6d69          Nnm = mi
-00010210: 6e28 286e 6d61 785f 706c 6f74 202b 2031  n((nmax_plot + 1
-00010220: 2920 2a2a 2032 202d 2031 2c20 6e70 2e73  ) ** 2 - 1, np.s
-00010230: 697a 6528 6e76 616c 7329 290a 2020 2020  ize(nvals)).    
-00010240: 2020 2020 6966 206e 702e 7369 7a65 286e      if np.size(n
-00010250: 702e 7368 6170 6528 4269 6e6d 2929 203e  p.shape(Binm)) >
-00010260: 2032 3a0a 2020 2020 2020 2020 2020 2020   2:.            
-00010270: 6c69 6e5f 4269 6e6d 203d 206e 702e 6172  lin_Binm = np.ar
-00010280: 7261 7928 5b20 4269 6e6d 5b69 6e74 286d  ray([ Binm[int(m
-00010290: 7661 6c73 5b69 4e5d 3c30 292c 6e76 616c  vals[iN]<0),nval
-000102a0: 735b 694e 5d2c 6162 7328 6d76 616c 735b  s[iN],abs(mvals[
-000102b0: 694e 5d29 5d20 666f 7220 694e 2069 6e20  iN])] for iN in 
-000102c0: 7261 6e67 6528 4e6e 6d29 205d 290a 2020  range(Nnm) ]).  
-000102d0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-000102e0: 2020 2020 2020 2020 6c69 6e5f 4269 6e6d          lin_Binm
-000102f0: 203d 2042 696e 6d0a 0a20 2020 206c 6c65   = Binm..    lle
-00010300: 6e79 203d 206e 702e 7369 7a65 286c 7468  ny = np.size(lth
-00010310: 7429 0a20 2020 206c 6c65 6e78 203d 206e  t).    llenx = n
-00010320: 702e 7369 7a65 286c 7068 6929 0a20 2020  p.size(lphi).   
-00010330: 2042 782c 2042 792c 2042 7a20 3d20 2820   Bx, By, Bz = ( 
-00010340: 6e70 2e7a 6572 6f73 2828 312c 6c6c 656e  np.zeros((1,llen
-00010350: 792a 6c6c 656e 7829 2c20 6474 7970 653d  y*llenx), dtype=
-00010360: 6e70 2e63 6f6d 706c 6578 5f29 2066 6f72  np.complex_) for
-00010370: 205f 2069 6e20 7261 6e67 6528 3329 2029   _ in range(3) )
-00010380: 0a0a 2020 2020 2320 4966 2077 6520 7061  ..    # If we pa
-00010390: 7373 2061 2073 696e 676c 6520 7661 6c75  ss a single valu
-000103a0: 6520 666f 7220 7228 7468 6574 612c 2070  e for r(theta, p
-000103b0: 6869 2920 3d20 522c 2065 7661 6c75 6174  hi) = R, evaluat
-000103c0: 6520 6f76 6572 2061 2073 7068 6572 6520  e over a sphere 
-000103d0: 7769 7468 2074 6861 7420 7261 6469 7573  with that radius
-000103e0: 2e0a 2020 2020 2320 4f74 6865 7277 6973  ..    # Otherwis
-000103f0: 652c 2065 7661 6c75 6174 6520 2a61 742a  e, evaluate *at*
-00010400: 2074 6865 2061 7379 6d6d 6574 7269 6320   the asymmetric 
-00010410: 3344 2073 7572 6661 6365 2e0a 2020 2020  3D surface..    
-00010420: 6966 206e 6f74 2069 7369 6e73 7461 6e63  if not isinstanc
-00010430: 6528 725f 7468 5f70 682c 2049 7465 7261  e(r_th_ph, Itera
-00010440: 626c 6529 3a0a 2020 2020 2020 2020 7820  ble):.        x 
-00010450: 3d20 6e70 2e61 7272 6179 285b 2072 5f74  = np.array([ r_t
-00010460: 685f 7068 2a6e 702e 7369 6e28 7468 7469  h_ph*np.sin(thti
-00010470: 292a 6e70 2e63 6f73 2870 6869 6929 2066  )*np.cos(phii) f
-00010480: 6f72 2074 6874 6920 696e 206c 7468 7420  or thti in ltht 
-00010490: 666f 7220 7068 6969 2069 6e20 6c70 6869  for phii in lphi
-000104a0: 205d 290a 2020 2020 2020 2020 7920 3d20   ]).        y = 
-000104b0: 6e70 2e61 7272 6179 285b 2072 5f74 685f  np.array([ r_th_
-000104c0: 7068 2a6e 702e 7369 6e28 7468 7469 292a  ph*np.sin(thti)*
-000104d0: 6e70 2e73 696e 2870 6869 6929 2066 6f72  np.sin(phii) for
-000104e0: 2074 6874 6920 696e 206c 7468 7420 666f   thti in ltht fo
-000104f0: 7220 7068 6969 2069 6e20 6c70 6869 205d  r phii in lphi ]
-00010500: 290a 2020 2020 2020 2020 7a20 3d20 6e70  ).        z = np
-00010510: 2e61 7272 6179 285b 2072 5f74 685f 7068  .array([ r_th_ph
-00010520: 2a6e 702e 636f 7328 7468 7469 2920 666f  *np.cos(thti) fo
-00010530: 7220 7468 7469 2069 6e20 6c74 6874 2066  r thti in ltht f
-00010540: 6f72 205f 2069 6e20 6c70 6869 205d 290a  or _ in lphi ]).
-00010550: 2020 2020 2020 2020 7220 3d20 6e70 2e7a          r = np.z
-00010560: 6572 6f73 2828 312c 6c6c 656e 792a 6c6c  eros((1,lleny*ll
-00010570: 656e 7829 2920 2b20 725f 7468 5f70 680a  enx)) + r_th_ph.
-00010580: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00010590: 2020 7820 3d20 6e70 2e61 7272 6179 285b    x = np.array([
-000105a0: 2072 5f74 685f 7068 5b69 5f74 682c 695f   r_th_ph[i_th,i_
-000105b0: 7068 5d2a 6e70 2e73 696e 286c 7468 745b  ph]*np.sin(ltht[
-000105c0: 695f 7468 5d29 2a6e 702e 636f 7328 6c70  i_th])*np.cos(lp
-000105d0: 6869 5b69 5f70 685d 2920 666f 7220 695f  hi[i_ph]) for i_
-000105e0: 7468 2069 6e20 7261 6e67 6528 6c6c 656e  th in range(llen
-000105f0: 7929 2066 6f72 2069 5f70 6820 696e 2072  y) for i_ph in r
-00010600: 616e 6765 286c 6c65 6e78 2920 5d29 0a20  ange(llenx) ]). 
-00010610: 2020 2020 2020 2079 203d 206e 702e 6172         y = np.ar
-00010620: 7261 7928 5b20 725f 7468 5f70 685b 695f  ray([ r_th_ph[i_
-00010630: 7468 2c69 5f70 685d 2a6e 702e 7369 6e28  th,i_ph]*np.sin(
-00010640: 6c74 6874 5b69 5f74 685d 292a 6e70 2e73  ltht[i_th])*np.s
-00010650: 696e 286c 7068 695b 695f 7068 5d29 2066  in(lphi[i_ph]) f
-00010660: 6f72 2069 5f74 6820 696e 2072 616e 6765  or i_th in range
-00010670: 286c 6c65 6e79 2920 666f 7220 695f 7068  (lleny) for i_ph
-00010680: 2069 6e20 7261 6e67 6528 6c6c 656e 7829   in range(llenx)
-00010690: 205d 290a 2020 2020 2020 2020 7a20 3d20   ]).        z = 
-000106a0: 6e70 2e61 7272 6179 285b 2072 5f74 685f  np.array([ r_th_
-000106b0: 7068 5b69 5f74 682c 695f 7068 5d2a 6e70  ph[i_th,i_ph]*np
-000106c0: 2e63 6f73 286c 7468 745b 695f 7468 5d29  .cos(ltht[i_th])
-000106d0: 2066 6f72 2069 5f74 6820 696e 2072 616e   for i_th in ran
-000106e0: 6765 286c 6c65 6e79 2920 666f 7220 695f  ge(lleny) for i_
-000106f0: 7068 2069 6e20 7261 6e67 6528 6c6c 656e  ph in range(llen
-00010700: 7829 205d 290a 2020 2020 2020 2020 7220  x) ]).        r 
-00010710: 3d20 6e70 2e72 6573 6861 7065 2872 5f74  = np.reshape(r_t
-00010720: 685f 7068 2c20 2831 2c6c 6c65 6e79 2a6c  h_ph, (1,lleny*l
-00010730: 6c65 6e78 2929 0a0a 2020 2020 6966 2064  lenx))..    if d
-00010740: 6f5f 7061 7261 6c6c 656c 3a0a 2020 2020  o_parallel:.    
-00010750: 2020 2020 6966 2053 6368 6d69 6474 3a0a      if Schmidt:.
-00010760: 2020 2020 2020 2020 2020 2020 706f 6f6c              pool
-00010770: 203d 206d 7470 436f 6e74 6578 742e 506f   = mtpContext.Po
-00010780: 6f6c 286e 756d 5f63 6f72 6573 290a 2020  ol(num_cores).  
-00010790: 2020 2020 2020 2020 2020 7061 725f 7265            par_re
-000107a0: 7375 6c74 203d 205b 706f 6f6c 2e61 7070  sult = [pool.app
-000107b0: 6c79 5f61 7379 6e63 2820 6576 616c 5f42  ly_async( eval_B
-000107c0: 695f 5363 686d 6964 742c 2061 7267 733d  i_Schmidt, args=
-000107d0: 286e 7661 6c73 5b69 4e5d 2c6d 7661 6c73  (nvals[iN],mvals
-000107e0: 5b69 4e5d 2c6c 696e 5f67 6e6d 5b69 4e5d  [iN],lin_gnm[iN]
-000107f0: 2c6c 696e 5f68 6e6d 5b69 4e5d 2c20 782c  ,lin_hnm[iN], x,
-00010800: 792c 7a2c 7229 2029 2066 6f72 2069 4e20  y,z,r) ) for iN 
-00010810: 696e 2072 616e 6765 284e 6e6d 295d 0a20  in range(Nnm)]. 
-00010820: 2020 2020 2020 2020 2020 2070 6f6f 6c2e             pool.
-00010830: 636c 6f73 6528 290a 2020 2020 2020 2020  close().        
-00010840: 2020 2020 706f 6f6c 2e6a 6f69 6e28 290a      pool.join().
-00010850: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-00010860: 2020 2020 2020 2020 2020 706f 6f6c 203d            pool =
-00010870: 206d 7470 436f 6e74 6578 742e 506f 6f6c   mtpContext.Pool
-00010880: 286e 756d 5f63 6f72 6573 290a 2020 2020  (num_cores).    
-00010890: 2020 2020 2020 2020 7061 725f 7265 7375          par_resu
-000108a0: 6c74 203d 205b 706f 6f6c 2e61 7070 6c79  lt = [pool.apply
-000108b0: 5f61 7379 6e63 2820 6576 616c 5f42 692c  _async( eval_Bi,
-000108c0: 2061 7267 733d 286e 7661 6c73 5b69 4e5d   args=(nvals[iN]
-000108d0: 2c6d 7661 6c73 5b69 4e5d 2c6c 696e 5f42  ,mvals[iN],lin_B
-000108e0: 696e 6d5b 694e 5d2c 2078 2c79 2c7a 2c72  inm[iN], x,y,z,r
-000108f0: 2920 2920 666f 7220 694e 2069 6e20 7261  ) ) for iN in ra
-00010900: 6e67 6528 4e6e 6d29 5d0a 2020 2020 2020  nge(Nnm)].      
-00010910: 2020 2020 2020 706f 6f6c 2e63 6c6f 7365        pool.close
-00010920: 2829 0a20 2020 2020 2020 2020 2020 2070  ().            p
-00010930: 6f6f 6c2e 6a6f 696e 2829 0a20 2020 2020  ool.join().     
-00010940: 2020 2023 2055 6e70 6163 6b20 7265 7375     # Unpack resu
-00010950: 6c74 7320 6672 6f6d 2070 6172 616c 6c65  lts from paralle
-00010960: 6c20 7072 6f63 6573 7369 6e67 2061 6e64  l processing and
-00010970: 2073 756d 2074 6865 6d0a 2020 2020 2020   sum them.      
-00010980: 2020 666f 7220 7265 7320 696e 2070 6172    for res in par
-00010990: 5f72 6573 756c 743a 0a20 2020 2020 2020  _result:.       
-000109a0: 2020 2020 2074 6869 735f 4278 2c20 7468       this_Bx, th
-000109b0: 6973 5f42 792c 2074 6869 735f 427a 203d  is_By, this_Bz =
-000109c0: 2072 6573 2e67 6574 2829 0a20 2020 2020   res.get().     
-000109d0: 2020 2020 2020 2042 7820 3d20 4278 202b         Bx = Bx +
-000109e0: 2074 6869 735f 4278 0a20 2020 2020 2020   this_Bx.       
-000109f0: 2020 2020 2042 7920 3d20 4279 202b 2074       By = By + t
-00010a00: 6869 735f 4279 0a20 2020 2020 2020 2020  his_By.         
-00010a10: 2020 2042 7a20 3d20 427a 202b 2074 6869     Bz = Bz + thi
-00010a20: 735f 427a 0a20 2020 2065 6c73 653a 0a20  s_Bz.    else:. 
-00010a30: 2020 2020 2020 2066 6f72 2069 4e20 696e         for iN in
-00010a40: 2072 616e 6765 284e 6e6d 293a 0a20 2020   range(Nnm):.   
-00010a50: 2020 2020 2020 2020 2069 6620 5363 686d           if Schm
-00010a60: 6964 743a 0a20 2020 2020 2020 2020 2020  idt:.           
-00010a70: 2020 2020 2074 6869 735f 4278 2c20 7468       this_Bx, th
-00010a80: 6973 5f42 792c 2074 6869 735f 427a 203d  is_By, this_Bz =
-00010a90: 2065 7661 6c5f 4269 5f53 6368 6d69 6474   eval_Bi_Schmidt
-00010aa0: 286e 7661 6c73 5b69 4e5d 2c20 6d76 616c  (nvals[iN], mval
-00010ab0: 735b 694e 5d2c 206c 696e 5f67 6e6d 5b69  s[iN], lin_gnm[i
-00010ac0: 4e5d 2c20 6c69 6e5f 686e 6d5b 694e 5d2c  N], lin_hnm[iN],
-00010ad0: 2078 2c20 792c 207a 2c20 7229 0a20 2020   x, y, z, r).   
-00010ae0: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
-00010af0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-00010b00: 6869 735f 4278 2c20 7468 6973 5f42 792c  his_Bx, this_By,
-00010b10: 2074 6869 735f 427a 203d 2065 7661 6c5f   this_Bz = eval_
-00010b20: 4269 286e 7661 6c73 5b69 4e5d 2c6d 7661  Bi(nvals[iN],mva
-00010b30: 6c73 5b69 4e5d 2c6c 696e 5f42 696e 6d5b  ls[iN],lin_Binm[
-00010b40: 694e 5d2c 2078 2c79 2c7a 2c72 290a 2020  iN], x,y,z,r).  
-00010b50: 2020 2020 2020 2020 2020 4278 203d 2042            Bx = B
-00010b60: 7820 2b20 7468 6973 5f42 780a 2020 2020  x + this_Bx.    
-00010b70: 2020 2020 2020 2020 4279 203d 2042 7920          By = By 
-00010b80: 2b20 7468 6973 5f42 790a 2020 2020 2020  + this_By.      
-00010b90: 2020 2020 2020 427a 203d 2042 7a20 2b20        Bz = Bz + 
-00010ba0: 7468 6973 5f42 7a0a 0a20 2020 2042 7820  this_Bz..    Bx 
-00010bb0: 3d20 6e70 2e72 6573 6861 7065 2842 782c  = np.reshape(Bx,
-00010bc0: 2028 6c6c 656e 792c 6c6c 656e 7829 290a   (lleny,llenx)).
-00010bd0: 2020 2020 4279 203d 206e 702e 7265 7368      By = np.resh
-00010be0: 6170 6528 4279 2c20 286c 6c65 6e79 2c6c  ape(By, (lleny,l
-00010bf0: 6c65 6e78 2929 0a20 2020 2042 7a20 3d20  lenx)).    Bz = 
-00010c00: 6e70 2e72 6573 6861 7065 2842 7a2c 2028  np.reshape(Bz, (
-00010c10: 6c6c 656e 792c 6c6c 656e 7829 290a 2020  lleny,llenx)).  
-00010c20: 2020 7265 7475 726e 2042 782c 2042 792c    return Bx, By,
-00010c30: 2042 7a0a                                 Bz.
+0000d040: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d070: 2058 6964 5b6d 7073 6967 6e2c 6e6e 702c   Xid[mpsign,nnp,
+0000d080: 6d70 6162 732c 2071 7369 676e 2c70 702c  mpabs, qsign,pp,
+0000d090: 7161 6273 2c20 6d73 6967 6e2c 6e6e 2c6d  qabs, msign,nn,m
+0000d0a0: 6162 735d 0a0a 2020 2020 2020 2020 2020  abs]..          
+0000d0b0: 2020 2020 2020 2020 2020 666f 7220 6920            for i 
+0000d0c0: 696e 2072 616e 6765 286e 5f62 6473 2d31  in range(n_bds-1
+0000d0d0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+0000d0e0: 2020 2020 2020 2020 2020 2044 656c 7461             Delta
+0000d0f0: 5b6d 7369 676e 2c6e 6e2c 6d61 6273 2c20  [msign,nn,mabs, 
+0000d100: 695d 202b 3d20 6d69 7873 756d 5b6d 7073  i] += mixsum[mps
+0000d110: 6967 6e2c 6e6e 702c 6d70 6162 732c 206d  ign,nnp,mpabs, m
+0000d120: 7369 676e 2c6e 6e2c 6d61 6273 2c20 695d  sign,nn,mabs, i]
+0000d130: 2f72 5f62 6473 5b2d 315d 202a 205c 0a20  /r_bds[-1] * \. 
+0000d140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d170: 2020 6142 6172 5b6d 7073 6967 6e2c 6e6e    aBar[mpsign,nn
+0000d180: 702c 6d70 6162 732c 2069 5d20 2a20 286a  p,mpabs, i] * (j
+0000d190: 6e5f 6c6c 5b6e 7069 2c69 5d20 2b20 4c61  n_ll[npi,i] + La
+0000d1a0: 6d62 645b 6e70 692c 695d 2a79 6e5f 6c6c  mbd[npi,i]*yn_ll
+0000d1b0: 5b6e 7069 2c69 5d29 202a 2028 6b72 5f6c  [npi,i]) * (kr_l
+0000d1c0: 6c5b 695d 2a2a 3220 2d20 6b72 5f75 6c5b  l[i]**2 - kr_ul[
+0000d1d0: 695d 2a2a 3229 0a0a 2020 2020 2020 2020  i]**2)..        
+0000d1e0: 2020 2020 2020 2020 2020 2020 4465 6c74              Delt
+0000d1f0: 615b 6d73 6967 6e2c 6e6e 2c6d 6162 732c  a[msign,nn,mabs,
+0000d200: 2d31 5d20 2b3d 206d 6978 7375 6d5b 6d70  -1] += mixsum[mp
+0000d210: 7369 676e 2c6e 6e70 2c6d 7061 6273 2c20  sign,nnp,mpabs, 
+0000d220: 6d73 6967 6e2c 6e6e 2c6d 6162 732c 202d  msign,nn,mabs, -
+0000d230: 315d 202a 205c 0a20 2020 2020 2020 2020  1] * \.         
+0000d240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d260: 2020 2020 2020 286c 7477 6f2a 6e76 202b        (ltwo*nv +
+0000d270: 206c 6f6e 6529 2f28 6e76 202b 206c 6f6e   lone)/(nv + lon
+0000d280: 6529 202a 2042 656e 6d5b 6d70 7369 676e  e) * Benm[mpsign
+0000d290: 2c6e 6e70 2c6d 7061 6273 5d20 2a20 4164  ,nnp,mpabs] * Ad
+0000d2a0: 5b6e 7069 5d0a 0a20 2020 2072 6574 7572  [npi]..    retur
+0000d2b0: 6e20 4465 6c74 610a 0a23 2323 2323 2323  n Delta..#######
+0000d2c0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0000d2d0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0000d2e0: 2323 2323 2323 0a0a 2222 220a 6576 616c  ######..""".eval
+0000d2f0: 5f69 6e6e 6572 5f72 6563 7572 5f73 796d  _inner_recur_sym
+0000d300: 2829 0a20 2020 2045 7661 6c75 6174 6520  ().    Evaluate 
+0000d310: 7468 6520 7370 6865 7269 6361 6c6c 7920  the spherically 
+0000d320: 7379 6d6d 6574 7269 6320 696e 6e65 7220  symmetric inner 
+0000d330: 7265 6375 7273 696f 6e20 7265 6c61 7469  recursion relati
+0000d340: 6f6e 7320 746f 206f 6274 6169 6e20 4c61  ons to obtain La
+0000d350: 6d62 6442 6172 2c20 7768 6963 6820 6973  mbdBar, which is
+0000d360: 0a20 2020 2065 7861 6374 6c79 2074 6865  .    exactly the
+0000d370: 2073 7068 6572 6963 616c 6c79 2073 796d   spherically sym
+0000d380: 6d65 7472 6963 2073 6f6c 7574 696f 6e20  metric solution 
+0000d390: 746f 2074 6865 2062 6f75 6e64 6172 7920  to the boundary 
+0000d3a0: 636f 6e64 6974 696f 6e73 2e20 5468 6973  conditions. This
+0000d3b0: 2071 7561 6e74 6974 7920 6170 7065 6172   quantity appear
+0000d3c0: 730a 2020 2020 696e 2074 6865 2061 7379  s.    in the asy
+0000d3d0: 6d6d 6574 7269 6320 7265 6375 7273 696f  mmetric recursio
+0000d3e0: 6e73 2c20 616e 6420 7765 206e 6565 6420  ns, and we need 
+0000d3f0: 746f 2065 7661 6c75 6174 6520 6974 2066  to evaluate it f
+0000d400: 6f72 2061 6c6c 206e 2028 6e6f 7420 6a75  or all n (not ju
+0000d410: 7374 2074 6865 2065 7863 6974 6174 696f  st the excitatio
+0000d420: 6e73 0a20 2020 2074 6861 7420 7265 7375  ns.    that resu
+0000d430: 6c74 2069 6e20 7468 6520 6361 7365 206f  lt in the case o
+0000d440: 6620 7370 6865 7269 6361 6c20 7379 6d6d  f spherical symm
+0000d450: 6574 7279 292e 0a20 2020 2055 7361 6765  etry)..    Usage
+0000d460: 3a20 604c 616d 6264 4261 7260 203d 2065  : `LambdBar` = e
+0000d470: 7661 6c5f 696e 6e65 725f 7265 6375 725f  val_inner_recur_
+0000d480: 7379 6d28 606e 5f6d 6178 602c 2060 6e5f  sym(`n_max`, `n_
+0000d490: 6264 7360 2c20 6062 6574 6160 2c20 6067  bds`, `beta`, `g
+0000d4a0: 616d 6d60 2c20 6064 656c 7460 2c20 6065  amm`, `delt`, `e
+0000d4b0: 7073 6960 290a 2020 2020 5265 7475 726e  psi`).    Return
+0000d4c0: 733a 0a20 2020 2020 2020 204c 616d 6264  s:.        Lambd
+0000d4d0: 4261 723a 206d 7063 2c20 7368 6170 6528  Bar: mpc, shape(
+0000d4e0: 6e5f 6d61 782c 6e5f 6264 7329 2e20 5468  n_max,n_bds). Th
+0000d4f0: 6973 2069 7320 5c6f 7665 726c 696e 657b  is is \overline{
+0000d500: 5c4c 616d 6264 617d 5e7b 6c7d 5f7b 6e7d  \Lambda}^{l}_{n}
+0000d510: 2069 6e20 7468 6520 7061 7065 722e 0a20   in the paper.. 
+0000d520: 2020 2050 6172 616d 6574 6572 733a 0a20     Parameters:. 
+0000d530: 2020 2020 2020 206e 5f6d 6178 3a20 696e         n_max: in
+0000d540: 7465 6765 722e 204d 6178 696d 756d 2064  teger. Maximum d
+0000d550: 6567 7265 6520 6e20 6f66 2069 6e64 7563  egree n of induc
+0000d560: 6564 206d 6f6d 656e 7473 2e0a 2020 2020  ed moments..    
+0000d570: 2020 2020 6e5f 6264 733a 2069 6e74 6567      n_bds: integ
+0000d580: 6572 2e20 4e75 6d62 6572 206f 6620 626f  er. Number of bo
+0000d590: 756e 6461 7269 6573 2070 7265 7365 6e74  undaries present
+0000d5a0: 2069 6e20 7468 6520 696e 7465 7269 6f72   in the interior
+0000d5b0: 206d 6f64 656c 2e0a 2020 2020 2020 2020   model..        
+0000d5c0: 6265 7461 2c20 6761 6d6d 2c20 6465 6c74  beta, gamm, delt
+0000d5d0: 2c20 6570 7369 3a20 6d70 632c 2073 6861  , epsi: mpc, sha
+0000d5e0: 7065 286e 5f6d 6178 2c6e 5f62 6473 292e  pe(n_max,n_bds).
+0000d5f0: 2052 6563 7572 7369 6f6e 2071 7561 6e74   Recursion quant
+0000d600: 6974 6965 7320 6465 7269 7665 6420 6672  ities derived fr
+0000d610: 6f6d 0a20 2020 2020 2020 2020 2020 2042  om.            B
+0000d620: 6573 7365 6c20 6675 6e63 7469 6f6e 732e  essel functions.
+0000d630: 2054 6865 7365 2061 7265 205c 6265 7461   These are \beta
+0000d640: 2c20 5c67 616d 6d61 2c20 5c64 656c 7461  , \gamma, \delta
+0000d650: 2c20 616e 6420 5c65 7073 696c 6f6e 2066  , and \epsilon f
+0000d660: 726f 6d20 7468 6520 7061 7065 722e 0a20  rom the paper.. 
+0000d670: 2020 2020 2020 2020 2020 2053 6565 2042             See B
+0000d680: 696e 6d52 6573 706f 6e73 6520 666f 7220  inmResponse for 
+0000d690: 6d6f 7265 2064 6574 6169 6c73 2e0a 2020  more details..  
+0000d6a0: 2020 2222 220a 6465 6620 6576 616c 5f69    """.def eval_i
+0000d6b0: 6e6e 6572 5f72 6563 7572 5f73 796d 286e  nner_recur_sym(n
+0000d6c0: 5f6d 6178 2c20 6e5f 6264 732c 2062 6574  _max, n_bds, bet
+0000d6d0: 612c 2067 616d 6d2c 2064 656c 742c 2065  a, gamm, delt, e
+0000d6e0: 7073 6929 3a0a 2020 2020 4c61 6d62 6420  psi):.    Lambd 
+0000d6f0: 3d20 6e70 2e7a 6572 6f73 2828 6e5f 6d61  = np.zeros((n_ma
+0000d700: 782c 6e5f 6264 7329 2c20 6474 7970 653d  x,n_bds), dtype=
+0000d710: 6d70 635f 676c 6f62 616c 290a 2020 2020  mpc_global).    
+0000d720: 666f 7220 6920 696e 2072 616e 6765 286e  for i in range(n
+0000d730: 5f62 6473 2d31 293a 0a20 2020 2020 2020  _bds-1):.       
+0000d740: 204c 616d 6264 5b3a 2c69 2b31 5d20 3d20   Lambd[:,i+1] = 
+0000d750: 6370 785f 6469 7628 2864 656c 745b 3a2c  cpx_div((delt[:,
+0000d760: 695d 202b 204c 616d 6264 5b3a 2c69 5d2a  i] + Lambd[:,i]*
+0000d770: 6570 7369 5b3a 2c69 5d29 202c 0a20 2020  epsi[:,i]) ,.   
+0000d780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d790: 2020 2020 2020 2020 2020 2020 2862 6574              (bet
+0000d7a0: 615b 3a2c 695d 202b 204c 616d 6264 5b3a  a[:,i] + Lambd[:
+0000d7b0: 2c69 5d2a 6761 6d6d 5b3a 2c69 5d29 290a  ,i]*gamm[:,i])).
+0000d7c0: 0a20 2020 2072 6574 7572 6e20 4c61 6d62  .    return Lamb
+0000d7d0: 640a 0a23 2041 766f 6964 7320 6469 7669  d..# Avoids divi
+0000d7e0: 6465 2d62 792d 7a65 726f 2065 7272 6f72  de-by-zero error
+0000d7f0: 7320 7768 656e 204c 616d 6264 2069 7320  s when Lambd is 
+0000d800: 7665 7279 2063 6c6f 7365 2074 6f20 6920  very close to i 
+0000d810: 2868 6967 6820 636f 6e64 7563 7469 7669  (high conductivi
+0000d820: 7469 6573 290a 6465 6620 6370 785f 6469  ties).def cpx_di
+0000d830: 7628 612c 2062 293a 0a20 2020 206e 7661  v(a, b):.    nva
+0000d840: 6c73 203d 206e 702e 7369 7a65 2861 290a  ls = np.size(a).
+0000d850: 2020 2020 616d 6167 203d 205b 206d 702e      amag = [ mp.
+0000d860: 6661 6273 2861 6929 2066 6f72 2061 6920  fabs(ai) for ai 
+0000d870: 696e 2061 205d 0a20 2020 2061 6172 6720  in a ].    aarg 
+0000d880: 3d20 5b20 6d70 2e61 7461 6e32 286d 702e  = [ mp.atan2(mp.
+0000d890: 696d 2861 6929 2c20 6d70 2e72 6528 6169  im(ai), mp.re(ai
+0000d8a0: 2929 2066 6f72 2061 6920 696e 2061 205d  )) for ai in a ]
+0000d8b0: 0a20 2020 2062 6d61 6720 3d20 5b20 6d70  .    bmag = [ mp
+0000d8c0: 2e66 6162 7328 6269 2920 666f 7220 6269  .fabs(bi) for bi
+0000d8d0: 2069 6e20 6220 5d0a 2020 2020 6261 7267   in b ].    barg
+0000d8e0: 203d 205b 206d 702e 6174 616e 3228 6d70   = [ mp.atan2(mp
+0000d8f0: 2e69 6d28 6269 292c 206d 702e 7265 2862  .im(bi), mp.re(b
+0000d900: 6929 2920 666f 7220 6269 2069 6e20 6220  i)) for bi in b 
+0000d910: 5d0a 0a20 2020 2064 6976 5f6d 6167 203d  ]..    div_mag =
+0000d920: 205b 2061 6d61 675b 695d 202f 2062 6d61   [ amag[i] / bma
+0000d930: 675b 695d 2066 6f72 2069 2069 6e20 7261  g[i] for i in ra
+0000d940: 6e67 6528 6e76 616c 7329 205d 0a20 2020  nge(nvals) ].   
+0000d950: 2064 6976 5f61 7267 203d 205b 2061 6172   div_arg = [ aar
+0000d960: 675b 695d 202d 2062 6172 675b 695d 2066  g[i] - barg[i] f
+0000d970: 6f72 2069 2069 6e20 7261 6e67 6528 6e76  or i in range(nv
+0000d980: 616c 7329 205d 0a20 2020 2071 756f 7469  als) ].    quoti
+0000d990: 656e 7420 3d20 6e70 2e61 7272 6179 285b  ent = np.array([
+0000d9a0: 2064 6976 5f6d 6167 5b69 5d20 2a20 6d70   div_mag[i] * mp
+0000d9b0: 2e65 7870 286a 202a 2064 6976 5f61 7267  .exp(j * div_arg
+0000d9c0: 5b69 5d29 2066 6f72 2069 2069 6e20 7261  [i]) for i in ra
+0000d9d0: 6e67 6528 6e76 616c 7329 205d 290a 2020  nge(nvals) ]).  
+0000d9e0: 2020 7265 7475 726e 2071 756f 7469 656e    return quotien
+0000d9f0: 740a 6465 6620 6370 785f 6469 765f 7661  t.def cpx_div_va
+0000da00: 6c28 612c 2062 293a 0a20 2020 2061 6d61  l(a, b):.    ama
+0000da10: 6720 3d20 6d70 2e66 6162 7328 6129 0a20  g = mp.fabs(a). 
+0000da20: 2020 2061 6172 6720 3d20 6d70 2e61 7461     aarg = mp.ata
+0000da30: 6e32 286d 702e 696d 2861 292c 206d 702e  n2(mp.im(a), mp.
+0000da40: 7265 2861 2929 0a20 2020 2062 6d61 6720  re(a)).    bmag 
+0000da50: 3d20 6d70 2e66 6162 7328 6229 0a20 2020  = mp.fabs(b).   
+0000da60: 2062 6172 6720 3d20 6d70 2e61 7461 6e32   barg = mp.atan2
+0000da70: 286d 702e 696d 2862 292c 206d 702e 7265  (mp.im(b), mp.re
+0000da80: 2862 2929 0a0a 2020 2020 6469 765f 6d61  (b))..    div_ma
+0000da90: 6720 3d20 616d 6167 202f 2062 6d61 670a  g = amag / bmag.
+0000daa0: 2020 2020 6469 765f 6172 6720 3d20 6161      div_arg = aa
+0000dab0: 7267 202d 2062 6172 670a 2020 2020 7175  rg - barg.    qu
+0000dac0: 6f74 6965 6e74 203d 2064 6976 5f6d 6167  otient = div_mag
+0000dad0: 202a 206d 702e 6578 7028 6a20 2a20 6469   * mp.exp(j * di
+0000dae0: 765f 6172 6729 0a20 2020 2072 6574 7572  v_arg).    retur
+0000daf0: 6e20 7175 6f74 6965 6e74 0a0a 2323 2323  n quotient..####
+0000db00: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0000db10: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0000db20: 2323 2323 2323 2323 230a 2320 4e4f 5445  #########.# NOTE
+0000db30: 2054 4845 204e 4f54 4154 494f 4e20 464f   THE NOTATION FO
+0000db40: 5220 6e27 2041 4e44 206e 2049 5320 5245  R n' AND n IS RE
+0000db50: 5645 5253 4544 2049 4e20 5448 4953 2043  VERSED IN THIS C
+0000db60: 4f44 4520 424c 4f43 4b20 434f 4d50 4152  ODE BLOCK COMPAR
+0000db70: 4544 2054 4f20 4d4f 5354 204f 4620 5448  ED TO MOST OF TH
+0000db80: 4520 4f54 4845 5220 434f 4445 0a23 2054  E OTHER CODE.# T
+0000db90: 6869 7320 6973 2066 6f72 2063 6f6e 7369  his is for consi
+0000dba0: 7374 656e 6379 2077 6974 6820 7468 6520  stency with the 
+0000dbb0: 7061 7065 7220 616e 6420 666f 7220 7368  paper and for sh
+0000dbc0: 6f72 7465 7220 6c69 6e65 7320 6f66 2063  orter lines of c
+0000dbd0: 6f64 652e 0a23 2049 6e20 7468 6973 2062  ode..# In this b
+0000dbe0: 6c6f 636b 2c20 6e2c 6d20 6973 2074 6865  lock, n,m is the
+0000dbf0: 2065 7863 6974 6174 696f 6e20 6861 726d   excitation harm
+0000dc00: 6f6e 6963 2061 6e64 206e 272c 6d27 2069  onic and n',m' i
+0000dc10: 7320 7468 6520 696e 6475 6365 6420 6861  s the induced ha
+0000dc20: 726d 6f6e 6963 2e0a 2323 2323 2323 2323  rmonic..########
+0000dc30: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0000dc40: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+0000dc50: 2323 2323 230a 0a22 2222 0a67 6574 5f61  #####..""".get_a
+0000dc60: 6c6c 5f58 6964 2829 0a20 2020 2052 6574  ll_Xid().    Ret
+0000dc70: 7572 6e73 206d 6978 696e 6720 636f 6566  urns mixing coef
+0000dc80: 6669 6369 656e 7473 2074 6861 7420 7265  ficients that re
+0000dc90: 7375 6c74 2066 726f 6d20 6d75 6c74 6970  sult from multip
+0000dca0: 6c69 6361 7469 6f6e 206f 6620 7370 6865  lication of sphe
+0000dcb0: 7269 6361 6c20 6861 726d 6f6e 6963 732e  rical harmonics.
+0000dcc0: 0a20 2020 2055 7361 6765 3a20 6058 6964  .    Usage: `Xid
+0000dcd0: 6020 3d20 6765 745f 616c 6c5f 5869 6428  ` = get_all_Xid(
+0000dce0: 606e 5f6d 6178 602c 2060 705f 6d61 7860  `n_max`, `p_max`
+0000dcf0: 2c20 606e 7072 6d5f 6d61 7860 2c20 606e  , `nprm_max`, `n
+0000dd00: 7072 6d76 616c 7360 2c20 606d 7072 6d76  prmvals`, `mprmv
+0000dd10: 616c 7360 290a 2020 2020 5265 7475 726e  als`).    Return
+0000dd20: 733a 0a20 2020 2020 2020 2058 6964 3a20  s:.        Xid: 
+0000dd30: 6d70 662c 2073 6861 7065 2832 2c6e 5f6d  mpf, shape(2,n_m
+0000dd40: 6178 2b31 2c6e 5f6d 6178 2b31 2c20 322c  ax+1,n_max+1, 2,
+0000dd50: 705f 6d61 782b 312c 705f 6d61 782b 312c  p_max+1,p_max+1,
+0000dd60: 2032 2c6e 7072 6d5f 6d61 782b 312c 6e70   2,nprm_max+1,np
+0000dd70: 726d 5f6d 6178 2b31 292e 2041 6d6f 756e  rm_max+1). Amoun
+0000dd80: 7420 6f66 2059 6e6d 2074 6861 7420 7265  t of Ynm that re
+0000dd90: 7375 6c74 730a 2020 2020 2020 2020 2020  sults.          
+0000dda0: 2020 6672 6f6d 206d 756c 7469 706c 7969    from multiplyi
+0000ddb0: 6e67 2059 6e6d 2062 7920 5970 712e 2056  ng Ynm by Ypq. V
+0000ddc0: 616c 7565 7320 666f 7220 616c 6c20 636f  alues for all co
+0000ddd0: 6d62 696e 6174 696f 6e73 206f 6620 6e2c  mbinations of n,
+0000dde0: 6d2c 702c 712c 6e27 2c6d 2720 6172 6520  m,p,q,n',m' are 
+0000ddf0: 7265 7475 726e 6564 2e0a 2020 2020 5061  returned..    Pa
+0000de00: 7261 6d65 7465 7273 3a0a 2020 2020 2020  rameters:.      
+0000de10: 2020 6e5f 6d61 783a 2069 6e74 6567 6572    n_max: integer
+0000de20: 2e20 4d61 7869 6d75 6d20 6465 6772 6565  . Maximum degree
+0000de30: 206e 206f 6620 6578 6369 7461 7469 6f6e   n of excitation
+0000de40: 206d 6f6d 656e 7473 2e0a 2020 2020 2020   moments..      
+0000de50: 2020 705f 6d61 783a 2069 6e74 6567 6572    p_max: integer
+0000de60: 2e20 4d61 7869 6d75 6d20 6465 6772 6565  . Maximum degree
+0000de70: 2070 206f 6620 626f 756e 6461 7279 2073   p of boundary s
+0000de80: 6861 7065 732e 0a20 2020 2020 2020 206e  hapes..        n
+0000de90: 7072 6d5f 6d61 783a 2069 6e74 6567 6572  prm_max: integer
+0000dea0: 2e20 4d61 7869 6d75 6d20 6465 6772 6565  . Maximum degree
+0000deb0: 206e 7072 6d20 6f66 2069 6e64 7563 6564   nprm of induced
+0000dec0: 206d 6f6d 656e 7473 2e20 5479 7069 6361   moments. Typica
+0000ded0: 6c6c 7920 6e6d 6178 202b 2070 6d61 782e  lly nmax + pmax.
+0000dee0: 0a20 2020 2020 2020 206e 7072 6d76 616c  .        nprmval
+0000def0: 733a 2069 6e74 6567 6572 2c20 7368 6170  s: integer, shap
+0000df00: 6528 286e 7072 6d5f 6d61 782b 3129 2a2a  e((nprm_max+1)**
+0000df10: 322d 3129 2e20 466c 6174 7465 6e65 6420  2-1). Flattened 
+0000df20: 6172 7261 7920 6f66 206e 7072 6d20 7661  array of nprm va
+0000df30: 6c75 6573 2e0a 2020 2020 2020 2020 6d70  lues..        mp
+0000df40: 726d 7661 6c73 3a20 696e 7465 6765 722c  rmvals: integer,
+0000df50: 2073 6861 7065 2828 6e70 726d 5f6d 6178   shape((nprm_max
+0000df60: 2b31 292a 2a32 2d31 292e 2046 6c61 7474  +1)**2-1). Flatt
+0000df70: 656e 6564 2061 7272 6179 206f 6620 6d70  ened array of mp
+0000df80: 726d 2076 616c 7565 7320 636f 7272 6573  rm values corres
+0000df90: 706f 6e64 696e 6720 746f 2065 6163 6820  ponding to each 
+0000dfa0: 6e72 706d 2061 626f 7665 2e0a 2020 2020  nrpm above..    
+0000dfb0: 2222 220a 6465 6620 6765 745f 616c 6c5f  """.def get_all_
+0000dfc0: 5869 6428 6e5f 6d61 782c 2070 5f6d 6178  Xid(n_max, p_max
+0000dfd0: 2c20 6e70 726d 5f6d 6178 2c20 6e70 726d  , nprm_max, nprm
+0000dfe0: 7661 6c73 2c20 6d70 726d 7661 6c73 2c20  vals, mprmvals, 
+0000dff0: 646f 5f70 6172 616c 6c65 6c3d 5472 7565  do_parallel=True
+0000e000: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000e010: 2020 7772 6974 656f 7574 3d54 7275 652c    writeout=True,
+0000e020: 2072 656c 6f61 643d 4661 6c73 652c 2066   reload=False, f
+0000e030: 7061 7468 3d4e 6f6e 652c 2066 6e61 6d65  path=None, fname
+0000e040: 3d4e 6f6e 6529 3a0a 2020 2020 6966 2077  =None):.    if w
+0000e050: 7269 7465 6f75 7420 6f72 2072 656c 6f61  riteout or reloa
+0000e060: 643a 0a20 2020 2020 2020 2069 6620 6670  d:.        if fp
+0000e070: 6174 6820 6973 204e 6f6e 653a 0a20 2020  ath is None:.   
+0000e080: 2020 2020 2020 2020 2066 7061 7468 203d           fpath =
+0000e090: 205f 696e 6475 6365 640a 2020 2020 2020   _induced.      
+0000e0a0: 2020 6966 2066 6e61 6d65 2069 7320 4e6f    if fname is No
+0000e0b0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+0000e0c0: 666e 616d 6520 3d20 6622 5869 645f 7661  fname = f"Xid_va
+0000e0d0: 6c75 6573 5f6e 7b6e 5f6d 6178 7d5f 707b  lues_n{n_max}_p{
+0000e0e0: 705f 6d61 787d 5f6e 707b 6e70 726d 5f6d  p_max}_np{nprm_m
+0000e0f0: 6178 7d22 0a0a 2020 2020 2020 2020 6675  ax}"..        fu
+0000e100: 6c6c 4669 6c65 203d 206f 732e 7061 7468  llFile = os.path
+0000e110: 2e6a 6f69 6e28 6670 6174 682c 2066 6e61  .join(fpath, fna
+0000e120: 6d65 2b22 2e6d 6174 2229 0a20 2020 2020  me+".mat").     
+0000e130: 2020 2066 696c 6545 7869 7374 7320 3d20     fileExists = 
+0000e140: 6f73 2e70 6174 682e 6973 6669 6c65 2866  os.path.isfile(f
+0000e150: 756c 6c46 696c 6529 0a20 2020 2020 2020  ullFile).       
+0000e160: 2069 6620 7265 6c6f 6164 2061 6e64 206e   if reload and n
+0000e170: 6f74 2066 696c 6545 7869 7374 733a 0a20  ot fileExists:. 
+0000e180: 2020 2020 2020 2020 2020 206c 6f67 2e77             log.w
+0000e190: 6172 6e69 6e67 2866 2758 6964 2066 696c  arning(f'Xid fil
+0000e1a0: 6520 7b66 756c 6c46 696c 657d 2064 6f65  e {fullFile} doe
+0000e1b0: 7320 6e6f 7420 6578 6973 742c 2062 7574  s not exist, but
+0000e1c0: 2072 656c 6f61 6420 6973 2054 7275 652e   reload is True.
+0000e1d0: 2043 616c 6375 6c61 7469 6e67 2069 6e73   Calculating ins
+0000e1e0: 7465 6164 2e27 290a 2020 2020 2020 2020  tead.').        
+0000e1f0: 2020 2020 7265 6c6f 6164 203d 2046 616c      reload = Fal
+0000e200: 7365 0a20 2020 2020 2020 2020 2020 2077  se.            w
+0000e210: 7269 7465 6f75 7420 3d20 5472 7565 0a0a  riteout = True..
+0000e220: 2020 2020 6966 2072 656c 6f61 643a 0a20      if reload:. 
+0000e230: 2020 2020 2020 2058 6964 203d 206c 6f61         Xid = loa
+0000e240: 646d 6174 2866 756c 6c46 696c 6529 5b27  dmat(fullFile)['
+0000e250: 5869 6427 5d0a 2020 2020 656c 7365 3a0a  Xid'].    else:.
+0000e260: 2020 2020 2020 2020 5869 6420 3d20 6e70          Xid = np
+0000e270: 2e7a 6572 6f73 2828 322c 6e5f 6d61 782b  .zeros((2,n_max+
+0000e280: 312c 6e5f 6d61 782b 312c 2032 2c70 5f6d  1,n_max+1, 2,p_m
+0000e290: 6178 2b31 2c70 5f6d 6178 2b31 2c20 322c  ax+1,p_max+1, 2,
+0000e2a0: 6e70 726d 5f6d 6178 2b31 2c6e 7072 6d5f  nprm_max+1,nprm_
+0000e2b0: 6d61 782b 3129 2c20 6474 7970 653d 6d70  max+1), dtype=mp
+0000e2c0: 665f 676c 6f62 616c 290a 2020 2020 2020  f_global).      
+0000e2d0: 2020 4e6e 6d70 726d 203d 206e 702e 7369    Nnmprm = np.si
+0000e2e0: 7a65 286e 7072 6d76 616c 7329 0a0a 2020  ze(nprmvals)..  
+0000e2f0: 2020 2020 2020 666f 7220 6e20 696e 2072        for n in r
+0000e300: 616e 6765 2831 2c6e 5f6d 6178 2b31 293a  ange(1,n_max+1):
+0000e310: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
+0000e320: 206d 2069 6e20 7261 6e67 6528 2d6e 2c6e   m in range(-n,n
+0000e330: 2b31 293a 0a20 2020 2020 2020 2020 2020  +1):.           
+0000e340: 2020 2020 206d 7369 676e 203d 2069 6e74       msign = int
+0000e350: 286d 3c30 290a 2020 2020 2020 2020 2020  (m<0).          
+0000e360: 2020 2020 2020 6d61 6273 203d 2061 6273        mabs = abs
+0000e370: 286d 290a 0a20 2020 2020 2020 2020 2020  (m)..           
+0000e380: 2020 2020 2066 6f72 2070 2069 6e20 7261       for p in ra
+0000e390: 6e67 6528 312c 705f 6d61 782b 3129 3a0a  nge(1,p_max+1):.
+0000e3a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e3b0: 2020 2020 666f 7220 7120 696e 2072 616e      for q in ran
+0000e3c0: 6765 282d 702c 702b 3129 3a0a 2020 2020  ge(-p,p+1):.    
+0000e3d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e3e0: 2020 2020 7173 6967 6e20 3d20 696e 7428      qsign = int(
+0000e3f0: 713c 3029 0a20 2020 2020 2020 2020 2020  q<0).           
+0000e400: 2020 2020 2020 2020 2020 2020 2071 6162               qab
+0000e410: 7320 3d20 6162 7328 7129 0a0a 2020 2020  s = abs(q)..    
+0000e420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e430: 2020 2020 6966 2064 6f5f 7061 7261 6c6c      if do_parall
+0000e440: 656c 3a0a 2020 2020 2020 2020 2020 2020  el:.            
+0000e450: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e460: 706f 6f6c 203d 206d 7470 436f 6e74 6578  pool = mtpContex
+0000e470: 742e 506f 6f6c 286e 756d 5f63 6f72 6573  t.Pool(num_cores
+0000e480: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0000e490: 2020 2020 2020 2020 2020 2020 2020 7061                pa
+0000e4a0: 725f 7265 7375 6c74 203d 205b 706f 6f6c  r_result = [pool
+0000e4b0: 2e61 7070 6c79 5f61 7379 6e63 2820 6361  .apply_async( ca
+0000e4c0: 6c63 5f58 6964 2c20 6172 6773 3d28 6e2c  lc_Xid, args=(n,
+0000e4d0: 6d2c 702c 712c 6e70 726d 7661 6c73 5b69  m,p,q,nprmvals[i
+0000e4e0: 4e5d 2c6d 7072 6d76 616c 735b 694e 5d2c  N],mprmvals[iN],
+0000e4f0: 6e70 726d 5f6d 6178 2920 2920 666f 7220  nprm_max) ) for 
+0000e500: 694e 2069 6e20 7261 6e67 6528 4e6e 6d70  iN in range(Nnmp
+0000e510: 726d 295d 0a20 2020 2020 2020 2020 2020  rm)].           
+0000e520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e530: 2070 6f6f 6c2e 636c 6f73 6528 290a 2020   pool.close().  
+0000e540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e550: 2020 2020 2020 2020 2020 706f 6f6c 2e6a            pool.j
+0000e560: 6f69 6e28 290a 0a20 2020 2020 2020 2020  oin()..         
+0000e570: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+0000e580: 6f72 2069 4e20 696e 2072 616e 6765 284e  or iN in range(N
+0000e590: 6e6d 7072 6d29 3a0a 2020 2020 2020 2020  nmprm):.        
+0000e5a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e5b0: 2020 2020 6e70 726d 203d 206e 7072 6d76      nprm = nprmv
+0000e5c0: 616c 735b 694e 5d0a 2020 2020 2020 2020  als[iN].        
+0000e5d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e5e0: 2020 2020 6d70 7369 676e 203d 2069 6e74      mpsign = int
+0000e5f0: 286d 7072 6d76 616c 735b 694e 5d3c 3029  (mprmvals[iN]<0)
+0000e600: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e610: 2020 2020 2020 2020 2020 2020 206d 7061               mpa
+0000e620: 6273 203d 2061 6273 286d 7072 6d76 616c  bs = abs(mprmval
+0000e630: 735b 694e 5d29 0a20 2020 2020 2020 2020  s[iN]).         
+0000e640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e650: 2020 2069 6620 646f 5f70 6172 616c 6c65     if do_paralle
+0000e660: 6c3a 0a20 2020 2020 2020 2020 2020 2020  l:.             
+0000e670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e680: 2020 2058 6964 5b6d 7369 676e 2c6e 2c6d     Xid[msign,n,m
+0000e690: 6162 732c 2071 7369 676e 2c70 2c71 6162  abs, qsign,p,qab
+0000e6a0: 732c 206d 7073 6967 6e2c 6e70 726d 2c6d  s, mpsign,nprm,m
+0000e6b0: 7061 6273 5d20 3d20 7061 725f 7265 7375  pabs] = par_resu
+0000e6c0: 6c74 5b69 4e5d 2e67 6574 2829 0a20 2020  lt[iN].get().   
+0000e6d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e6e0: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
+0000e6f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e700: 2020 2020 2020 2020 2020 2020 2020 2058                 X
+0000e710: 6964 5b6d 7369 676e 2c20 6e2c 206d 6162  id[msign, n, mab
+0000e720: 732c 2071 7369 676e 2c20 702c 2071 6162  s, qsign, p, qab
+0000e730: 732c 206d 7073 6967 6e2c 206e 7072 6d2c  s, mpsign, nprm,
+0000e740: 206d 7061 6273 5d20 3d20 6361 6c63 5f58   mpabs] = calc_X
+0000e750: 6964 286e 2c6d 2c70 2c71 2c6e 7072 6d76  id(n,m,p,q,nprmv
+0000e760: 616c 735b 694e 5d2c 6d70 726d 7661 6c73  als[iN],mprmvals
+0000e770: 5b69 4e5d 2c6e 7072 6d5f 6d61 7829 0a20  [iN],nprm_max). 
+0000e780: 2020 2020 2020 2069 6620 7772 6974 656f         if writeo
+0000e790: 7574 3a0a 2020 2020 2020 2020 2020 2020  ut:.            
+0000e7a0: 7361 7665 6d61 7428 6675 6c6c 4669 6c65  savemat(fullFile
+0000e7b0: 2c20 7b27 5869 6427 3a20 5869 642e 6173  , {'Xid': Xid.as
+0000e7c0: 7479 7065 286e 702e 666c 6f61 745f 297d  type(np.float_)}
+0000e7d0: 290a 2020 2020 2020 2020 2020 2020 6c6f  ).            lo
+0000e7e0: 672e 6465 6275 6728 6627 5361 7665 6420  g.debug(f'Saved 
+0000e7f0: 5869 6420 7661 6c75 6573 2074 6f20 6669  Xid values to fi
+0000e800: 6c65 3a20 7b66 756c 6c46 696c 657d 2729  le: {fullFile}')
+0000e810: 0a0a 2020 2020 7265 7475 726e 2058 6964  ..    return Xid
+0000e820: 0a0a 2222 220a 7072 696e 745f 5869 645f  ..""".print_Xid_
+0000e830: 7461 626c 6528 290a 2020 2020 5072 696e  table().    Prin
+0000e840: 7473 2061 2074 6162 6c65 2074 6f20 7468  ts a table to th
+0000e850: 6520 7465 726d 696e 616c 206f 6620 7661  e terminal of va
+0000e860: 6c75 6573 2066 6f72 2061 6c6c 2058 6964  lues for all Xid
+0000e870: 2066 6f72 2064 6562 7567 2070 7572 706f   for debug purpo
+0000e880: 7365 732e 0a20 2020 2055 7361 6765 3a20  ses..    Usage: 
+0000e890: 7072 696e 745f 5869 645f 7461 626c 6528  print_Xid_table(
+0000e8a0: 6058 6964 602c 2060 6e5f 6d61 7860 2c20  `Xid`, `n_max`, 
+0000e8b0: 6070 5f6d 6178 602c 2060 6e70 726d 5f6d  `p_max`, `nprm_m
+0000e8c0: 6178 6029 0a20 2020 2052 6574 7572 6e73  ax`).    Returns
+0000e8d0: 3a0a 2020 2020 2020 2020 4e6f 6e65 2e0a  :.        None..
+0000e8e0: 2020 2020 5061 7261 6d65 7465 7273 3a0a      Parameters:.
+0000e8f0: 2020 2020 2020 2020 5869 643a 206d 7066          Xid: mpf
+0000e900: 2c20 7368 6170 6528 322c 6e5f 6d61 782b  , shape(2,n_max+
+0000e910: 312c 6e5f 6d61 782b 312c 2032 2c70 5f6d  1,n_max+1, 2,p_m
+0000e920: 6178 2b31 2c70 5f6d 6178 2b31 2c20 322c  ax+1,p_max+1, 2,
+0000e930: 6e70 726d 5f6d 6178 2b31 2c6e 7072 6d5f  nprm_max+1,nprm_
+0000e940: 6d61 782b 3129 2e20 5869 6420 7661 6c75  max+1). Xid valu
+0000e950: 6573 2074 6f20 7072 696e 742e 0a20 2020  es to print..   
+0000e960: 2020 2020 206e 5f6d 6178 3a20 696e 7465       n_max: inte
+0000e970: 6765 722e 204d 6178 696d 756d 2064 6567  ger. Maximum deg
+0000e980: 7265 6520 6e20 6f66 2065 7863 6974 6174  ree n of excitat
+0000e990: 696f 6e20 6d6f 6d65 6e74 732e 0a20 2020  ion moments..   
+0000e9a0: 2020 2020 2070 5f6d 6178 3a20 696e 7465       p_max: inte
+0000e9b0: 6765 722e 204d 6178 696d 756d 2064 6567  ger. Maximum deg
+0000e9c0: 7265 6520 7020 6f66 2062 6f75 6e64 6172  ree p of boundar
+0000e9d0: 7920 7368 6170 6573 2e0a 2020 2020 2020  y shapes..      
+0000e9e0: 2020 6e70 726d 5f6d 6178 3a20 696e 7465    nprm_max: inte
+0000e9f0: 6765 722e 204d 6178 696d 756d 2064 6567  ger. Maximum deg
+0000ea00: 7265 6520 6e70 726d 206f 6620 696e 6475  ree nprm of indu
+0000ea10: 6365 6420 6d6f 6d65 6e74 732e 2054 7970  ced moments. Typ
+0000ea20: 6963 616c 6c79 206e 6d61 7820 2b20 706d  ically nmax + pm
+0000ea30: 6178 2e0a 2020 2020 2222 220a 6465 6620  ax..    """.def 
+0000ea40: 7072 696e 745f 5869 645f 7461 626c 6528  print_Xid_table(
+0000ea50: 5869 642c 206e 5f6d 6178 2c20 705f 6d61  Xid, n_max, p_ma
+0000ea60: 782c 206e 7072 6d5f 6d61 7829 3a0a 2020  x, nprm_max):.  
+0000ea70: 2020 2320 5072 696e 7420 7461 626c 6520    # Print table 
+0000ea80: 6865 6164 6572 0a20 2020 2068 6561 645f  header.    head_
+0000ea90: 726f 7720 3d20 2220 2020 2022 0a20 2020  row = "    ".   
+0000eaa0: 2066 6f72 206e 2069 6e20 7261 6e67 6528   for n in range(
+0000eab0: 312c 206e 5f6d 6178 2b31 293a 0a20 2020  1, n_max+1):.   
+0000eac0: 2020 2020 2066 6f72 206d 2069 6e20 7261       for m in ra
+0000ead0: 6e67 6528 2d6e 2c20 6e2b 3129 3a0a 2020  nge(-n, n+1):.  
+0000eae0: 2020 2020 2020 2020 2020 6865 6164 5f72            head_r
+0000eaf0: 6f77 203d 2068 6561 645f 726f 7720 2b20  ow = head_row + 
+0000eb00: 6622 7c20 2020 2059 7b6e 7d7b 6d7d 2020  f"|    Y{n}{m}  
+0000eb10: 2020 222e 6c6a 7573 7428 3235 290a 2020    ".ljust(25).  
+0000eb20: 2020 6865 6164 5f72 6f77 203d 2066 227b    head_row = f"{
+0000eb30: 6865 6164 5f72 6f77 7d7c 220a 2020 2020  head_row}|".    
+0000eb40: 7072 696e 7428 6865 6164 5f72 6f77 290a  print(head_row).
+0000eb50: 2020 2020 2320 5072 696e 7420 7368 6170      # Print shap
+0000eb60: 6573 2061 7320 726f 7773 0a20 2020 2066  es as rows.    f
+0000eb70: 6f72 2070 2069 6e20 7261 6e67 6528 312c  or p in range(1,
+0000eb80: 2070 5f6d 6178 2b31 293a 0a20 2020 2020   p_max+1):.     
+0000eb90: 2020 2066 6f72 2071 2069 6e20 7261 6e67     for q in rang
+0000eba0: 6528 2d70 2c20 702b 3129 3a0a 2020 2020  e(-p, p+1):.    
+0000ebb0: 2020 2020 2020 2020 7173 6967 6e20 3d20          qsign = 
+0000ebc0: 696e 7428 713c 3029 0a20 2020 2020 2020  int(q<0).       
+0000ebd0: 2020 2020 2071 6162 7320 3d20 6162 7328       qabs = abs(
+0000ebe0: 7129 0a20 2020 2020 2020 2020 2020 2072  q).            r
+0000ebf0: 6f77 5f73 7472 203d 2066 2253 7b70 7d7b  ow_str = f"S{p}{
+0000ec00: 717d 222e 6c6a 7573 7428 3429 0a0a 2020  q}".ljust(4)..  
+0000ec10: 2020 2020 2020 2020 2020 2320 5072 696e            # Prin
+0000ec20: 7420 6578 6369 7461 7469 6f6e 206d 6f6d  t excitation mom
+0000ec30: 656e 7473 2061 7320 636f 6c75 6d6e 730a  ents as columns.
+0000ec40: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+0000ec50: 6e20 696e 2072 616e 6765 2831 2c20 6e5f  n in range(1, n_
+0000ec60: 6d61 782b 3129 3a0a 2020 2020 2020 2020  max+1):.        
+0000ec70: 2020 2020 2020 2020 666f 7220 6d20 696e          for m in
+0000ec80: 2072 616e 6765 282d 6e2c 206e 2b31 293a   range(-n, n+1):
+0000ec90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000eca0: 2020 2020 206d 7369 676e 203d 2069 6e74       msign = int
+0000ecb0: 286d 3c30 290a 2020 2020 2020 2020 2020  (m<0).          
+0000ecc0: 2020 2020 2020 2020 2020 6d61 6273 203d            mabs =
+0000ecd0: 2061 6273 286d 290a 2020 2020 2020 2020   abs(m).        
+0000ece0: 2020 2020 2020 2020 2020 2020 6365 6c6c              cell
+0000ecf0: 5f73 7472 203d 2022 7c20 220a 0a20 2020  _str = "| "..   
+0000ed00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ed10: 2023 2050 7269 6e74 206e 6f6e 2d7a 6572   # Print non-zer
+0000ed20: 6f20 7465 726d 7320 666f 7220 6561 6368  o terms for each
+0000ed30: 2063 656c 6c0a 2020 2020 2020 2020 2020   cell.          
+0000ed40: 2020 2020 2020 2020 2020 666f 7220 6e70            for np
+0000ed50: 726d 2069 6e20 7261 6e67 6528 6e70 726d  rm in range(nprm
+0000ed60: 5f6d 6178 2c20 302c 202d 3129 3a0a 2020  _max, 0, -1):.  
+0000ed70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ed80: 2020 2020 2020 6d70 726d 203d 206d 202b        mprm = m +
+0000ed90: 2071 0a20 2020 2020 2020 2020 2020 2020   q.             
+0000eda0: 2020 2020 2020 2020 2020 206d 7073 6967             mpsig
+0000edb0: 6e20 3d20 696e 7428 6d70 726d 3c30 290a  n = int(mprm<0).
+0000edc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000edd0: 2020 2020 2020 2020 6d70 6162 7320 3d20          mpabs = 
+0000ede0: 6162 7328 6d70 726d 290a 0a20 2020 2020  abs(mprm)..     
+0000edf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ee00: 2020 2074 6869 735f 5869 6420 3d20 5869     this_Xid = Xi
+0000ee10: 645b 6d73 6967 6e2c 6e2c 6d61 6273 2c20  d[msign,n,mabs, 
+0000ee20: 7173 6967 6e2c 702c 7161 6273 2c20 6d70  qsign,p,qabs, mp
+0000ee30: 7369 676e 2c6e 7072 6d2c 6d70 6162 735d  sign,nprm,mpabs]
+0000ee40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000ee50: 2020 2020 2020 2020 2061 6273 5f58 6920           abs_Xi 
+0000ee60: 3d20 6162 7328 7468 6973 5f58 6964 290a  = abs(this_Xid).
+0000ee70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ee80: 2020 2020 2020 2020 726f 756e 645f 5869          round_Xi
+0000ee90: 203d 2072 6f75 6e64 2861 6273 2874 6869   = round(abs(thi
+0000eea0: 735f 5869 6429 2c33 290a 2020 2020 2020  s_Xid),3).      
+0000eeb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000eec0: 2020 6966 2861 6273 5f58 6920 3e20 3165    if(abs_Xi > 1e
+0000eed0: 2d31 3829 3a0a 2020 2020 2020 2020 2020  -18):.          
+0000eee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000eef0: 2020 6966 2863 656c 6c5f 7374 7220 213d    if(cell_str !=
+0000ef00: 2022 7c20 2229 3a0a 2020 2020 2020 2020   "| "):.        
+0000ef10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ef20: 2020 2020 2020 2020 6966 2869 6e74 2874          if(int(t
+0000ef30: 6869 735f 5869 643e 3029 206f 7220 726f  his_Xid>0) or ro
+0000ef40: 756e 645f 5869 3d3d 302e 3029 3a0a 2020  und_Xi==0.0):.  
+0000ef50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ef60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ef70: 2020 6365 6c6c 5f73 7472 203d 2066 227b    cell_str = f"{
+0000ef80: 6365 6c6c 5f73 7472 7d2b 2022 0a20 2020  cell_str}+ ".   
+0000ef90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000efa0: 2020 2020 2020 2020 2020 2020 2065 6c73               els
+0000efb0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+0000efc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000efd0: 2020 2020 2020 2063 656c 6c5f 7374 7220         cell_str 
+0000efe0: 3d20 6622 7b63 656c 6c5f 7374 727d 2d20  = f"{cell_str}- 
+0000eff0: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
+0000f000: 2020 2020 2020 2020 2020 2020 2020 656c                el
+0000f010: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+0000f020: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f030: 2020 2020 6966 2869 6e74 2874 6869 735f      if(int(this_
+0000f040: 5869 643e 3029 206f 7220 726f 756e 645f  Xid>0) or round_
+0000f050: 5869 3d3d 302e 3029 3a0a 2020 2020 2020  Xi==0.0):.      
+0000f060: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f070: 2020 2020 2020 2020 2020 2020 2020 6365                ce
+0000f080: 6c6c 5f73 7472 203d 2066 227b 6365 6c6c  ll_str = f"{cell
+0000f090: 5f73 7472 7d20 220a 2020 2020 2020 2020  _str} ".        
+0000f0a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f0b0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+0000f0c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f0d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f0e0: 2020 6365 6c6c 5f73 7472 203d 2066 227b    cell_str = f"{
+0000f0f0: 6365 6c6c 5f73 7472 7d2d 220a 2020 2020  cell_str}-".    
+0000f100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f110: 2020 2020 2020 2020 6365 6c6c 5f73 7472          cell_str
+0000f120: 203d 2066 227b 6365 6c6c 5f73 7472 7d7b   = f"{cell_str}{
+0000f130: 726f 756e 645f 5869 7d59 7b6e 7072 6d7d  round_Xi}Y{nprm}
+0000f140: 7b6d 7072 6d7d 2022 2e6c 6a75 7374 2831  {mprm} ".ljust(1
+0000f150: 3329 0a0a 2020 2020 2020 2020 2020 2020  3)..            
+0000f160: 2020 2020 2020 2020 726f 775f 7374 7220          row_str 
+0000f170: 3d20 6622 7b72 6f77 5f73 7472 7d7b 6365  = f"{row_str}{ce
+0000f180: 6c6c 5f73 7472 2e6c 6a75 7374 2832 3529  ll_str.ljust(25)
+0000f190: 7d22 0a0a 2020 2020 2020 2020 2020 2020  }"..            
+0000f1a0: 726f 775f 7374 7220 3d20 6622 7b72 6f77  row_str = f"{row
+0000f1b0: 5f73 7472 7d7c 220a 2020 2020 2020 2020  _str}|".        
+0000f1c0: 2020 2020 7072 696e 7428 726f 775f 7374      print(row_st
+0000f1d0: 7229 0a0a 2020 2020 7265 7475 726e 0a0a  r)..    return..
+0000f1e0: 2222 220a 7072 696e 745f 5869 5f74 6162  """.print_Xi_tab
+0000f1f0: 6c65 2829 0a20 2020 2050 7269 6e74 7320  le().    Prints 
+0000f200: 6120 7461 626c 6520 746f 2074 6865 2074  a table to the t
+0000f210: 6572 6d69 6e61 6c20 6f66 2076 616c 7565  erminal of value
+0000f220: 7320 666f 7220 616c 6c20 5869 2066 6f72  s for all Xi for
+0000f230: 2064 6562 7567 2070 7572 706f 7365 732e   debug purposes.
+0000f240: 0a20 2020 2055 7361 6765 3a20 7072 696e  .    Usage: prin
+0000f250: 745f 5869 5f74 6162 6c65 2860 6e5f 6d61  t_Xi_table(`n_ma
+0000f260: 7860 2c20 6070 5f6d 6178 602c 2060 6e70  x`, `p_max`, `np
+0000f270: 726d 5f6d 6178 6029 0a20 2020 2052 6574  rm_max`).    Ret
+0000f280: 7572 6e73 3a0a 2020 2020 2020 2020 4e6f  urns:.        No
+0000f290: 6e65 2e0a 2020 2020 5061 7261 6d65 7465  ne..    Paramete
+0000f2a0: 7273 3a0a 2020 2020 2020 2020 6e5f 6d61  rs:.        n_ma
+0000f2b0: 783a 2069 6e74 6567 6572 2e20 4d61 7869  x: integer. Maxi
+0000f2c0: 6d75 6d20 6465 6772 6565 206e 206f 6620  mum degree n of 
+0000f2d0: 6578 6369 7461 7469 6f6e 206d 6f6d 656e  excitation momen
+0000f2e0: 7473 2e0a 2020 2020 2020 2020 705f 6d61  ts..        p_ma
+0000f2f0: 783a 2069 6e74 6567 6572 2e20 4d61 7869  x: integer. Maxi
+0000f300: 6d75 6d20 6465 6772 6565 2070 206f 6620  mum degree p of 
+0000f310: 626f 756e 6461 7279 2073 6861 7065 732e  boundary shapes.
+0000f320: 0a20 2020 2020 2020 206e 7072 6d5f 6d61  .        nprm_ma
+0000f330: 783a 2069 6e74 6567 6572 2e20 4d61 7869  x: integer. Maxi
+0000f340: 6d75 6d20 6465 6772 6565 206e 7072 6d20  mum degree nprm 
+0000f350: 6f66 2069 6e64 7563 6564 206d 6f6d 656e  of induced momen
+0000f360: 7473 2e20 5479 7069 6361 6c6c 7920 6e6d  ts. Typically nm
+0000f370: 6178 202b 2070 6d61 782e 0a20 2020 2022  ax + pmax..    "
+0000f380: 2222 0a64 6566 2070 7269 6e74 5f58 695f  "".def print_Xi_
+0000f390: 7461 626c 6528 6e5f 6d61 782c 2070 5f6d  table(n_max, p_m
+0000f3a0: 6178 2c20 6e70 726d 5f6d 6178 293a 0a20  ax, nprm_max):. 
+0000f3b0: 2020 2023 2050 7269 6e74 2074 6162 6c65     # Print table
+0000f3c0: 2068 6561 6465 720a 2020 2020 6865 6164   header.    head
+0000f3d0: 5f72 6f77 203d 2022 2020 2020 220a 2020  _row = "    ".  
+0000f3e0: 2020 666f 7220 6e20 696e 2072 616e 6765    for n in range
+0000f3f0: 2831 2c20 6e5f 6d61 782b 3129 3a0a 2020  (1, n_max+1):.  
+0000f400: 2020 2020 2020 666f 7220 6d20 696e 2072        for m in r
+0000f410: 616e 6765 282d 6e2c 206e 2b31 293a 0a20  ange(-n, n+1):. 
+0000f420: 2020 2020 2020 2020 2020 2068 6561 645f             head_
+0000f430: 726f 7720 3d20 6622 7b68 6561 645f 726f  row = f"{head_ro
+0000f440: 777d 7c20 2020 2059 7b6e 7d7b 6d7d 2020  w}|    Y{n}{m}  
+0000f450: 2020 222e 6c6a 7573 7428 3235 290a 2020    ".ljust(25).  
+0000f460: 2020 6865 6164 5f72 6f77 203d 2066 227b    head_row = f"{
+0000f470: 6865 6164 5f72 6f77 7d7c 220a 2020 2020  head_row}|".    
+0000f480: 7072 696e 7428 6865 6164 5f72 6f77 290a  print(head_row).
+0000f490: 2020 2020 2320 5072 696e 7420 7368 6170      # Print shap
+0000f4a0: 6573 2061 7320 726f 7773 0a20 2020 2066  es as rows.    f
+0000f4b0: 6f72 2070 2069 6e20 7261 6e67 6528 312c  or p in range(1,
+0000f4c0: 2070 5f6d 6178 2b31 293a 0a20 2020 2020   p_max+1):.     
+0000f4d0: 2020 2066 6f72 2071 2069 6e20 7261 6e67     for q in rang
+0000f4e0: 6528 2d70 2c20 702b 3129 3a0a 2020 2020  e(-p, p+1):.    
+0000f4f0: 2020 2020 2020 2020 726f 775f 7374 7220          row_str 
+0000f500: 3d20 6622 537b 707d 7b71 7d22 2e6c 6a75  = f"S{p}{q}".lju
+0000f510: 7374 2834 290a 0a20 2020 2020 2020 2020  st(4)..         
+0000f520: 2020 2023 2050 7269 6e74 2065 7863 6974     # Print excit
+0000f530: 6174 696f 6e20 6d6f 6d65 6e74 7320 6173  ation moments as
+0000f540: 2063 6f6c 756d 6e73 0a20 2020 2020 2020   columns.       
+0000f550: 2020 2020 2066 6f72 206e 2069 6e20 7261       for n in ra
+0000f560: 6e67 6528 312c 206e 5f6d 6178 2b31 293a  nge(1, n_max+1):
+0000f570: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000f580: 2066 6f72 206d 2069 6e20 7261 6e67 6528   for m in range(
+0000f590: 2d6e 2c20 6e2b 3129 3a0a 2020 2020 2020  -n, n+1):.      
+0000f5a0: 2020 2020 2020 2020 2020 2020 2020 6365                ce
+0000f5b0: 6c6c 5f73 7472 203d 2022 7c20 220a 0a20  ll_str = "| ".. 
+0000f5c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f5d0: 2020 2023 2050 7269 6e74 206e 6f6e 2d7a     # Print non-z
+0000f5e0: 6572 6f20 7465 726d 7320 666f 7220 6561  ero terms for ea
+0000f5f0: 6368 2063 656c 6c0a 2020 2020 2020 2020  ch cell.        
+0000f600: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+0000f610: 6e70 726d 2069 6e20 7261 6e67 6528 6e70  nprm in range(np
+0000f620: 726d 5f6d 6178 2c20 302c 202d 3129 3a0a  rm_max, 0, -1):.
+0000f630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f640: 2020 2020 2020 2020 6d70 726d 203d 206d          mprm = m
+0000f650: 202b 2071 0a0a 2020 2020 2020 2020 2020   + q..          
+0000f660: 2020 2020 2020 2020 2020 2020 2020 7468                th
+0000f670: 6973 5f58 6920 3d20 6361 6c63 5f58 6928  is_Xi = calc_Xi(
+0000f680: 6e2c 6d2c 702c 712c 6e70 726d 2c6d 7072  n,m,p,q,nprm,mpr
+0000f690: 6d29 0a20 2020 2020 2020 2020 2020 2020  m).             
+0000f6a0: 2020 2020 2020 2020 2020 2069 6620 6162             if ab
+0000f6b0: 7328 7468 6973 5f58 6929 203e 2030 2e30  s(this_Xi) > 0.0
+0000f6c0: 3030 3031 3a0a 2020 2020 2020 2020 2020  0001:.          
+0000f6d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f6e0: 2020 6966 2063 656c 6c5f 7374 7220 213d    if cell_str !=
+0000f6f0: 2022 7c20 223a 0a20 2020 2020 2020 2020   "| ":.         
+0000f700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f710: 2020 2020 2020 2069 6628 696e 7428 7468         if(int(th
+0000f720: 6973 5f58 693c 3029 293a 0a20 2020 2020  is_Xi<0)):.     
+0000f730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f740: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+0000f750: 656c 6c5f 7374 7220 3d20 6622 7b63 656c  ell_str = f"{cel
+0000f760: 6c5f 7374 727d 2d20 220a 2020 2020 2020  l_str}- ".      
+0000f770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f780: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
+0000f790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f7a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f7b0: 2020 2020 6365 6c6c 5f73 7472 203d 2066      cell_str = f
+0000f7c0: 227b 6365 6c6c 5f73 7472 7d2b 2022 0a20  "{cell_str}+ ". 
+0000f7d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f7e0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+0000f7f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000f800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f810: 2069 6628 696e 7428 7468 6973 5f58 693c   if(int(this_Xi<
+0000f820: 3029 293a 0a20 2020 2020 2020 2020 2020  0)):.           
+0000f830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f840: 2020 2020 2020 2020 2063 656c 6c5f 7374           cell_st
+0000f850: 7220 3d20 6622 7b63 656c 6c5f 7374 727d  r = f"{cell_str}
+0000f860: 2d22 0a20 2020 2020 2020 2020 2020 2020  -".             
+0000f870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f880: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+0000f890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f8a0: 2020 2020 2020 2020 2020 2020 2063 656c               cel
+0000f8b0: 6c5f 7374 7220 3d20 6622 7b63 656c 6c5f  l_str = f"{cell_
+0000f8c0: 7374 727d 2022 0a20 2020 2020 2020 2020  str} ".         
+0000f8d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f8e0: 2020 2063 656c 6c5f 7374 7220 3d20 6622     cell_str = f"
+0000f8f0: 7b63 656c 6c5f 7374 727d 7b61 6273 2874  {cell_str}{abs(t
+0000f900: 6869 735f 5869 293a 2e33 667d 597b 6e70  his_Xi):.3f}Y{np
+0000f910: 726d 7d7b 6d70 726d 7d20 222e 6c6a 7573  rm}{mprm} ".ljus
+0000f920: 7428 3133 290a 0a20 2020 2020 2020 2020  t(13)..         
+0000f930: 2020 2020 2020 2020 2020 2072 6f77 5f73             row_s
+0000f940: 7472 203d 2066 227b 726f 775f 7374 727d  tr = f"{row_str}
+0000f950: 7b63 656c 6c5f 7374 727d 222e 6c6a 7573  {cell_str}".ljus
+0000f960: 7428 3235 290a 0a20 2020 2020 2020 2020  t(25)..         
+0000f970: 2020 2072 6f77 5f73 7472 203d 2066 227b     row_str = f"{
+0000f980: 726f 775f 7374 727d 7c22 0a20 2020 2020  row_str}|".     
+0000f990: 2020 2020 2020 2070 7269 6e74 2872 6f77         print(row
+0000f9a0: 5f73 7472 290a 0a20 2020 2072 6574 7572  _str)..    retur
+0000f9b0: 6e0a 0a22 2222 0a54 6865 2072 656d 6169  n..""".The remai
+0000f9c0: 6e69 6e67 2066 756e 6374 696f 6e73 2069  ning functions i
+0000f9d0: 6e20 7468 6973 2062 6c6f 636b 2061 7265  n this block are
+0000f9e0: 2061 6c6c 2073 7465 7073 2061 6e64 2073   all steps and s
+0000f9f0: 7562 7374 6570 7320 696e 2063 616c 6375  ubsteps in calcu
+0000fa00: 6c61 7469 6e67 2058 6964 0a20 2020 2061  lating Xid.    a
+0000fa10: 7320 696e 2065 7175 6174 696f 6e73 2053  s in equations S
+0000fa20: 3931 2d53 3130 3320 6672 6f6d 2074 6865  91-S103 from the
+0000fa30: 2070 6170 6572 2e0a 2020 2020 2222 220a   paper..    """.
+0000fa40: 6465 6620 6361 6c63 5f58 6964 286e 2c6d  def calc_Xid(n,m
+0000fa50: 2c70 2c71 2c6e 7072 6d2c 6d70 726d 2c20  ,p,q,nprm,mprm, 
+0000fa60: 6e70 726d 5f6d 6178 293a 0a20 2020 2074  nprm_max):.    t
+0000fa70: 6869 735f 5869 645f 6e75 6d20 3d20 2020  his_Xid_num =   
+0000fa80: 2020 2020 2063 616c 635f 5869 7728 6e2c       calc_Xiw(n,
+0000fa90: 206d 2c20 702c 2071 2c20 6e70 726d 2c20   m, p, q, nprm, 
+0000faa0: 6d70 726d 2920 2b20 205c 0a20 2020 2020  mprm) +  \.     
+0000fab0: 2020 2020 2020 2020 2020 2020 2020 2058                 X
+0000fac0: 6964 5365 7269 6573 4c6f 7765 7228 6e2c  idSeriesLower(n,
+0000fad0: 206d 2c20 702c 2071 2c20 6e70 726d 2c20   m, p, q, nprm, 
+0000fae0: 6d70 726d 2920 2b20 205c 0a20 2020 2020  mprm) +  \.     
+0000faf0: 2020 2020 2020 2020 2020 2020 2020 2058                 X
+0000fb00: 6964 5365 7269 6573 5570 7065 7228 6e2c  idSeriesUpper(n,
+0000fb10: 206d 2c20 702c 2071 2c20 6e70 726d 2c20   m, p, q, nprm, 
+0000fb20: 6d70 726d 2c20 6e70 726d 5f6d 6178 290a  mprm, nprm_max).
+0000fb30: 2020 2020 6966 2074 6869 735f 5869 645f      if this_Xid_
+0000fb40: 6e75 6d20 213d 2030 3a0a 2020 2020 2020  num != 0:.      
+0000fb50: 2020 5869 6420 3d20 7468 6973 5f58 6964    Xid = this_Xid
+0000fb60: 5f6e 756d 202f 2058 6964 4465 6e6f 6d28  _num / XidDenom(
+0000fb70: 6e70 726d 2c6d 7072 6d2c 6e70 726d 5f6d  nprm,mprm,nprm_m
+0000fb80: 6178 290a 2020 2020 656c 7365 3a0a 2020  ax).    else:.  
+0000fb90: 2020 2020 2020 5869 6420 3d20 7a65 726f        Xid = zero
+0000fba0: 0a20 2020 2072 6574 7572 6e20 5869 640a  .    return Xid.
+0000fbb0: 0a64 6566 2063 616c 635f 5869 286e 2c20  .def calc_Xi(n, 
+0000fbc0: 6d2c 2070 2c20 712c 206e 7072 6d2c 206d  m, p, q, nprm, m
+0000fbd0: 7072 6d29 3a0a 2020 2020 7472 6961 6e67  prm):.    triang
+0000fbe0: 203d 2028 6162 7328 6e20 2d20 7029 203c   = (abs(n - p) <
+0000fbf0: 3d20 6e70 726d 2920 616e 6420 286e 7072  = nprm) and (npr
+0000fc00: 6d20 3c3d 206e 202b 2070 290a 2020 2020  m <= n + p).    
+0000fc10: 6576 656e 203d 2028 6e20 2b20 7020 2b20  even = (n + p + 
+0000fc20: 6e70 726d 2920 2520 3220 3d3d 2030 0a20  nprm) % 2 == 0. 
+0000fc30: 2020 206d 5f6d 6174 6368 203d 2028 6d20     m_match = (m 
+0000fc40: 2b20 7120 3d3d 206d 7072 6d29 0a0a 2020  + q == mprm)..  
+0000fc50: 2020 6966 2074 7269 616e 6720 616e 6420    if triang and 
+0000fc60: 6576 656e 2061 6e64 206d 5f6d 6174 6368  even and m_match
+0000fc70: 3a0a 2020 2020 2020 2020 6e75 203d 2069  :.        nu = i
+0000fc80: 6e74 2828 6e20 2b20 7020 2d20 6e70 726d  nt((n + p - nprm
+0000fc90: 292f 3229 0a20 2020 2020 2020 2063 735f  )/2).        cs_
+0000fca0: 7369 676e 203d 2028 2d31 292a 2a6e 750a  sign = (-1)**nu.
+0000fcb0: 0a20 2020 2020 2020 206b 6170 5f6d 696e  .        kap_min
+0000fcc0: 203d 206d 6178 2830 2c20 322a 6e75 2d28   = max(0, 2*nu-(
+0000fcd0: 6e2b 6d29 2c20 322a 6e75 2d28 702d 7129  n+m), 2*nu-(p-q)
+0000fce0: 290a 2020 2020 2020 2020 6b61 705f 6d61  ).        kap_ma
+0000fcf0: 7820 3d20 6d69 6e28 322a 6e75 2c20 6e2d  x = min(2*nu, n-
+0000fd00: 6d2c 2070 2b71 290a 0a20 2020 2020 2020  m, p+q)..       
+0000fd10: 206e 6f72 6d20 3d20 6e70 2e73 7172 7428   norm = np.sqrt(
+0000fd20: 2832 2a6e 202b 2031 2920 2a20 2832 2a70  (2*n + 1) * (2*p
+0000fd30: 202b 2031 2920 2a20 2832 2a6e 7072 6d20   + 1) * (2*nprm 
+0000fd40: 2b20 3129 202f 2034 202f 206e 702e 7069  + 1) / 4 / np.pi
+0000fd50: 290a 2020 2020 2020 2020 6674 5f73 7172  ).        ft_sqr
+0000fd60: 7420 3d20 6e70 2e73 7172 7428 2066 7428  t = np.sqrt( ft(
+0000fd70: 6e2b 6d29 2a66 7428 6e2d 6d29 2a66 7428  n+m)*ft(n-m)*ft(
+0000fd80: 702b 7129 2a66 7428 702d 7129 2a66 7428  p+q)*ft(p-q)*ft(
+0000fd90: 6e70 726d 2b6d 7072 6d29 2a66 7428 6e70  nprm+mprm)*ft(np
+0000fda0: 726d 2d6d 7072 6d29 2029 0a20 2020 2020  rm-mprm) ).     
+0000fdb0: 2020 2066 745f 6672 6163 203d 2066 7428     ft_frac = ft(
+0000fdc0: 322a 6e75 292f 6674 286e 7529 202a 2066  2*nu)/ft(nu) * f
+0000fdd0: 7428 322a 6e2d 322a 6e75 292f 6674 286e  t(2*n-2*nu)/ft(n
+0000fde0: 2d6e 7529 202a 2066 7428 322a 702d 322a  -nu) * ft(2*p-2*
+0000fdf0: 6e75 292f 6674 2870 2d6e 7529 202a 2066  nu)/ft(p-nu) * f
+0000fe00: 7428 6e70 726d 2b6e 7529 2f66 7428 322a  t(nprm+nu)/ft(2*
+0000fe10: 6e70 726d 2b31 2b32 2a6e 7529 0a0a 2020  nprm+1+2*nu)..  
+0000fe20: 2020 2020 2020 6b61 705f 7375 6d20 3d20        kap_sum = 
+0000fe30: 6e70 2e73 756d 285b 2028 2d31 292a 2a6b  np.sum([ (-1)**k
+0000fe40: 6170 202f 2028 2066 7428 6b61 7029 2a66  ap / ( ft(kap)*f
+0000fe50: 7428 322a 6e75 2d6b 6170 2920 2a20 6674  t(2*nu-kap) * ft
+0000fe60: 286e 2d6d 2d6b 6170 292a 6674 286e 2b6d  (n-m-kap)*ft(n+m
+0000fe70: 2d28 322a 6e75 2d6b 6170 2929 202a 0a20  -(2*nu-kap)) *. 
+0000fe80: 2020 2020 2020 2020 2020 2066 7428 702b             ft(p+
+0000fe90: 712d 6b61 7029 2a66 7428 702d 712d 2832  q-kap)*ft(p-q-(2
+0000fea0: 2a6e 752d 6b61 7029 2920 2920 666f 7220  *nu-kap)) ) for 
+0000feb0: 6b61 7020 696e 2072 616e 6765 286b 6170  kap in range(kap
+0000fec0: 5f6d 696e 2c6b 6170 5f6d 6178 2b31 2920  _min,kap_max+1) 
+0000fed0: 5d29 0a0a 2020 2020 2020 2020 5869 203d  ])..        Xi =
+0000fee0: 2063 735f 7369 676e 202a 206e 6f72 6d20   cs_sign * norm 
+0000fef0: 2a20 6674 5f66 7261 6320 2a20 6674 5f73  * ft_frac * ft_s
+0000ff00: 7172 7420 2a20 6b61 705f 7375 6d0a 2020  qrt * kap_sum.  
+0000ff10: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+0000ff20: 5869 203d 207a 6572 6f0a 0a20 2020 2072  Xi = zero..    r
+0000ff30: 6574 7572 6e20 5869 0a0a 6465 6620 775f  eturn Xi..def w_
+0000ff40: 4d28 6e2c 6d29 3a0a 2020 2020 776d 203d  M(n,m):.    wm =
+0000ff50: 206d 702e 7265 2820 286e 2b31 292a 6d70   mp.re( (n+1)*mp
+0000ff60: 2e73 7172 7428 6e2a 2a32 202d 206d 2a2a  .sqrt(n**2 - m**
+0000ff70: 3229 202f 206d 702e 7371 7274 2828 322a  2) / mp.sqrt((2*
+0000ff80: 6e2d 3129 202a 2028 322a 6e2b 3129 2920  n-1) * (2*n+1)) 
+0000ff90: 290a 2020 2020 7265 7475 726e 2077 6d0a  ).    return wm.
+0000ffa0: 0a64 6566 2077 5f50 286e 2c6d 293a 0a20  .def w_P(n,m):. 
+0000ffb0: 2020 2077 7020 3d20 6e2a 6d70 2e72 6528     wp = n*mp.re(
+0000ffc0: 206d 702e 7371 7274 2828 6e2b 3129 2a2a   mp.sqrt((n+1)**
+0000ffd0: 3220 2d20 6d2a 2a32 2920 2f20 6d70 2e73  2 - m**2) / mp.s
+0000ffe0: 7172 7428 2832 2a6e 2b31 292a 2832 2a6e  qrt((2*n+1)*(2*n
+0000fff0: 2b33 2929 2029 0a20 2020 2072 6574 7572  +3)) ).    retur
+00010000: 6e20 7770 0a0a 6465 6620 6361 6c63 5f58  n wp..def calc_X
+00010010: 6977 286e 2c20 6d2c 2070 2c20 712c 206e  iw(n, m, p, q, n
+00010020: 7072 6d2c 206d 7072 6d29 3a0a 2020 2020  prm, mprm):.    
+00010030: 6d61 6273 203d 2061 6273 286d 290a 2020  mabs = abs(m).  
+00010040: 2020 6d70 6162 7320 3d20 6162 7328 6d70    mpabs = abs(mp
+00010050: 726d 290a 0a20 2020 2077 4d6e 203d 2077  rm)..    wMn = w
+00010060: 5f4d 286e 2c6d 6162 7329 0a20 2020 2077  _M(n,mabs).    w
+00010070: 506e 203d 2077 5f50 286e 2c6d 6162 7329  Pn = w_P(n,mabs)
+00010080: 0a20 2020 2077 4d6e 7020 3d20 775f 4d28  .    wMnp = w_M(
+00010090: 6e70 726d 2c6d 7061 6273 290a 2020 2020  nprm,mpabs).    
+000100a0: 7750 6e70 203d 2077 5f50 286e 7072 6d2c  wPnp = w_P(nprm,
+000100b0: 6d70 6162 7329 0a0a 2020 2020 5869 7720  mpabs)..    Xiw 
+000100c0: 3d20 2077 4d6e 202a 2077 4d6e 7020 2a20  =  wMn * wMnp * 
+000100d0: 6361 6c63 5f58 6928 6e2d 312c 206d 2c20  calc_Xi(n-1, m, 
+000100e0: 702c 2071 2c20 6e70 726d 2d31 2c20 6d70  p, q, nprm-1, mp
+000100f0: 726d 2920 2020 205c 0a20 2020 2020 2020  rm)    \.       
+00010100: 2020 2b20 7750 6e20 2a20 7750 6e70 202a    + wPn * wPnp *
+00010110: 2063 616c 635f 5869 286e 2b31 2c20 6d2c   calc_Xi(n+1, m,
+00010120: 2070 2c20 712c 206e 7072 6d2b 312c 206d   p, q, nprm+1, m
+00010130: 7072 6d29 2020 2020 5c0a 2020 2020 2020  prm)    \.      
+00010140: 2020 202d 2077 4d6e 202a 2077 506e 7020     - wMn * wPnp 
+00010150: 2a20 6361 6c63 5f58 6928 6e2d 312c 206d  * calc_Xi(n-1, m
+00010160: 2c20 702c 2071 2c20 6e70 726d 2b31 2c20  , p, q, nprm+1, 
+00010170: 6d70 726d 2920 2020 205c 0a20 2020 2020  mprm)    \.     
+00010180: 2020 2020 2d20 7750 6e20 2a20 774d 6e70      - wPn * wMnp
+00010190: 202a 2063 616c 635f 5869 286e 2b31 2c20   * calc_Xi(n+1, 
+000101a0: 6d2c 2070 2c20 712c 206e 7072 6d2d 312c  m, p, q, nprm-1,
+000101b0: 206d 7072 6d29 0a0a 2020 2020 7265 7475   mprm)..    retu
+000101c0: 726e 2058 6977 0a0a 6465 6620 465f 4d28  rn Xiw..def F_M(
+000101d0: 6e2c 206d 2c20 7477 6f6b 6170 293a 0a20  n, m, twokap):. 
+000101e0: 2020 2069 6620 6e20 3c20 3320 6f72 2074     if n < 3 or t
+000101f0: 776f 6b61 7020 3e20 6e2d 6162 7328 6d29  wokap > n-abs(m)
+00010200: 2d32 3a0a 2020 2020 2020 2020 7265 7475  -2:.        retu
+00010210: 726e 207a 6572 6f0a 2020 2020 656c 7365  rn zero.    else
+00010220: 3a0a 2020 2020 2020 2020 6e5f 7468 6973  :.        n_this
+00010230: 203d 206e 2d74 776f 6b61 700a 2020 2020   = n-twokap.    
+00010240: 2020 2020 6e5f 646f 776e 203d 206e 2d28      n_down = n-(
+00010250: 7477 6f6b 6170 2b32 290a 2020 2020 2020  twokap+2).      
+00010260: 2020 6e5f 646f 776e 3220 3d20 6e2d 2874    n_down2 = n-(t
+00010270: 776f 6b61 702b 3429 0a20 2020 2020 2020  wokap+4).       
+00010280: 2069 6620 775f 4d28 6e5f 7468 6973 2c6d   if w_M(n_this,m
+00010290: 293d 3d30 206f 7220 775f 5028 6e5f 646f  )==0 or w_P(n_do
+000102a0: 776e 2c6d 293d 3d30 3a0a 2020 2020 2020  wn,m)==0:.      
+000102b0: 2020 2020 2020 7265 7475 726e 207a 6572        return zer
+000102c0: 6f0a 2020 2020 2020 2020 656c 7365 3a0a  o.        else:.
+000102d0: 2020 2020 2020 2020 2020 2020 466d 203d              Fm =
+000102e0: 2077 5f4d 286e 5f74 6869 732c 6d29 2a77   w_M(n_this,m)*w
+000102f0: 5f50 286e 5f64 6f77 6e2c 6d29 202f 2020  _P(n_down,m) /  
+00010300: 2020 5c0a 2020 2020 2020 2020 2020 2020    \.            
+00010310: 2820 775f 4d28 6e5f 646f 776e 2c6d 292a  ( w_M(n_down,m)*
+00010320: 2a32 202b 2077 5f50 286e 5f64 6f77 6e2c  *2 + w_P(n_down,
+00010330: 6d29 2a2a 3220 2d0a 2020 2020 2020 2020  m)**2 -.        
+00010340: 2020 2020 2020 2020 775f 4d28 6e5f 646f          w_M(n_do
+00010350: 776e 2c6d 292a 775f 5028 6e5f 646f 776e  wn,m)*w_P(n_down
+00010360: 322c 6d29 2a46 5f4d 286e 2c6d 2c74 776f  2,m)*F_M(n,m,two
+00010370: 6b61 702b 3229 2029 0a0a 2020 2020 7265  kap+2) )..    re
+00010380: 7475 726e 2046 6d0a 0a64 6566 2046 5f50  turn Fm..def F_P
+00010390: 286e 2c20 6d2c 2074 776f 6b61 702c 206e  (n, m, twokap, n
+000103a0: 7072 6d5f 6d61 7829 3a0a 2020 2020 6966  prm_max):.    if
+000103b0: 2074 776f 6b61 7020 3e20 6e70 726d 5f6d   twokap > nprm_m
+000103c0: 6178 2d6e 3a0a 2020 2020 2020 2020 7265  ax-n:.        re
+000103d0: 7475 726e 207a 6572 6f0a 2020 2020 656c  turn zero.    el
+000103e0: 7365 3a0a 2020 2020 2020 2020 6e5f 7468  se:.        n_th
+000103f0: 6973 203d 206e 2b74 776f 6b61 700a 2020  is = n+twokap.  
+00010400: 2020 2020 2020 6e5f 7570 203d 206e 2b28        n_up = n+(
+00010410: 7477 6f6b 6170 2b32 290a 2020 2020 2020  twokap+2).      
+00010420: 2020 6e5f 7570 3220 3d20 6e2b 2874 776f    n_up2 = n+(two
+00010430: 6b61 702b 3429 0a20 2020 2020 2020 2046  kap+4).        F
+00010440: 7020 3d20 775f 5028 6e5f 7468 6973 2c6d  p = w_P(n_this,m
+00010450: 292a 775f 4d28 6e5f 7570 2c6d 2920 2f20  )*w_M(n_up,m) / 
+00010460: 2020 205c 0a20 2020 2020 2020 2028 2077     \.        ( w
+00010470: 5f4d 286e 5f75 702c 6d29 2a2a 3220 2b20  _M(n_up,m)**2 + 
+00010480: 775f 5028 6e5f 7570 2c6d 292a 2a32 202d  w_P(n_up,m)**2 -
+00010490: 0a20 2020 2020 2020 2020 2020 2077 5f50  .            w_P
+000104a0: 286e 5f75 702c 6d29 2a77 5f4d 286e 5f75  (n_up,m)*w_M(n_u
+000104b0: 7032 2c6d 292a 465f 5028 6e2c 6d2c 7477  p2,m)*F_P(n,m,tw
+000104c0: 6f6b 6170 2b32 2c6e 7072 6d5f 6d61 7829  okap+2,nprm_max)
+000104d0: 2029 0a0a 2020 2020 7265 7475 726e 2046   )..    return F
+000104e0: 700a 0a23 204e 6f74 6520 7468 6174 2061  p..# Note that a
+000104f0: 6c74 686f 7567 6820 7468 6973 2074 6572  lthough this ter
+00010500: 6d20 6973 2063 616c 6c65 6420 5365 7269  m is called Seri
+00010510: 6573 4c6f 7765 722c 2069 7420 636f 6e74  esLower, it cont
+00010520: 6169 6e73 206d 6978 696e 6720 7465 726d  ains mixing term
+00010530: 7320 6672 6f6d 2068 6967 6865 7220 6465  s from higher de
+00010540: 6772 6565 206e 2727 2069 6e74 6f20 7468  gree n'' into th
+00010550: 6520 6c6f 7765 7220 6e27 0a64 6566 2058  e lower n'.def X
+00010560: 6964 5365 7269 6573 4c6f 7765 7228 6e2c  idSeriesLower(n,
+00010570: 206d 2c20 702c 2071 2c20 6e70 726d 2c20   m, p, q, nprm, 
+00010580: 6d70 726d 293a 0a20 2020 2069 6620 6e70  mprm):.    if np
+00010590: 726d 203e 3d20 333a 0a20 2020 2020 2020  rm >= 3:.       
+000105a0: 2067 6d61 785f 6c20 3d20 666c 6f6f 7228   gmax_l = floor(
+000105b0: 286e 7072 6d2d 6162 7328 6d70 726d 2929  (nprm-abs(mprm))
+000105c0: 2f32 290a 2020 2020 656c 7365 3a0a 2020  /2).    else:.  
+000105d0: 2020 2020 2020 676d 6178 5f6c 203d 2030        gmax_l = 0
+000105e0: 0a20 2020 2074 6869 734c 6f77 6572 203d  .    thisLower =
+000105f0: 2030 0a20 2020 2066 6f72 2067 2069 6e20   0.    for g in 
+00010600: 7261 6e67 6528 312c 676d 6178 5f6c 2b31  range(1,gmax_l+1
+00010610: 293a 0a20 2020 2020 2020 2074 6869 7350  ):.        thisP
+00010620: 726f 6420 3d20 310a 2020 2020 2020 2020  rod = 1.        
+00010630: 666f 7220 6b61 7020 696e 2072 616e 6765  for kap in range
+00010640: 2867 293a 0a20 2020 2020 2020 2020 2020  (g):.           
+00010650: 2074 6869 7350 726f 6420 3d20 7468 6973   thisProd = this
+00010660: 5072 6f64 202a 2046 5f4d 286e 7072 6d2c  Prod * F_M(nprm,
+00010670: 6d70 726d 2c32 2a6b 6170 290a 0a20 2020  mprm,2*kap)..   
+00010680: 2020 2020 2074 6869 734c 6f77 6572 203d       thisLower =
+00010690: 2074 6869 734c 6f77 6572 202b 2063 616c   thisLower + cal
+000106a0: 635f 5869 7728 6e2c 206d 2c20 702c 2071  c_Xiw(n, m, p, q
+000106b0: 2c20 6e70 726d 2d32 2a67 2c20 6d70 726d  , nprm-2*g, mprm
+000106c0: 292a 7468 6973 5072 6f64 0a0a 2020 2020  )*thisProd..    
+000106d0: 7365 7269 6573 4c6f 7765 7220 3d20 7468  seriesLower = th
+000106e0: 6973 4c6f 7765 720a 2020 2020 7265 7475  isLower.    retu
+000106f0: 726e 2073 6572 6965 734c 6f77 6572 0a0a  rn seriesLower..
+00010700: 2320 4e6f 7465 2074 6861 7420 616c 7468  # Note that alth
+00010710: 6f75 6768 2074 6869 7320 7465 726d 2069  ough this term i
+00010720: 7320 6361 6c6c 6564 2053 6572 6965 7355  s called SeriesU
+00010730: 7070 6572 2c20 6974 2063 6f6e 7461 696e  pper, it contain
+00010740: 7320 6d69 7869 6e67 2074 6572 6d73 2066  s mixing terms f
+00010750: 726f 6d20 6c6f 7765 7220 6465 6772 6565  rom lower degree
+00010760: 206e 2727 2069 6e74 6f20 7468 6520 6869   n'' into the hi
+00010770: 6768 6572 206e 270a 6465 6620 5869 6453  gher n'.def XidS
+00010780: 6572 6965 7355 7070 6572 286e 2c20 6d2c  eriesUpper(n, m,
+00010790: 2070 2c20 712c 206e 7072 6d2c 206d 7072   p, q, nprm, mpr
+000107a0: 6d2c 206e 7072 6d5f 6d61 7829 3a0a 2020  m, nprm_max):.  
+000107b0: 2020 676d 6178 5f75 203d 2066 6c6f 6f72    gmax_u = floor
+000107c0: 2828 6e70 726d 5f6d 6178 2d6e 7072 6d29  ((nprm_max-nprm)
+000107d0: 2f32 290a 2020 2020 7468 6973 5570 7065  /2).    thisUppe
+000107e0: 7220 3d20 300a 2020 2020 666f 7220 6720  r = 0.    for g 
+000107f0: 696e 2072 616e 6765 2831 2c67 6d61 785f  in range(1,gmax_
+00010800: 752b 3129 3a0a 2020 2020 2020 2020 7468  u+1):.        th
+00010810: 6973 5072 6f64 203d 2031 0a20 2020 2020  isProd = 1.     
+00010820: 2020 2066 6f72 206b 6170 2069 6e20 7261     for kap in ra
+00010830: 6e67 6528 6729 3a0a 2020 2020 2020 2020  nge(g):.        
+00010840: 2020 2020 7468 6973 5072 6f64 203d 2074      thisProd = t
+00010850: 6869 7350 726f 6420 2a20 465f 5028 6e70  hisProd * F_P(np
+00010860: 726d 2c6d 7072 6d2c 322a 6b61 702c 6e70  rm,mprm,2*kap,np
+00010870: 726d 5f6d 6178 290a 0a20 2020 2020 2020  rm_max)..       
+00010880: 2074 6869 7355 7070 6572 203d 2074 6869   thisUpper = thi
+00010890: 7355 7070 6572 202b 2063 616c 635f 5869  sUpper + calc_Xi
+000108a0: 7728 6e2c 206d 2c20 702c 2071 2c20 6e70  w(n, m, p, q, np
+000108b0: 726d 2b32 2a67 2c20 6d70 726d 292a 7468  rm+2*g, mprm)*th
+000108c0: 6973 5072 6f64 0a0a 2020 2020 7365 7269  isProd..    seri
+000108d0: 6573 5570 7065 7220 3d20 7468 6973 5570  esUpper = thisUp
+000108e0: 7065 720a 2020 2020 7265 7475 726e 2073  per.    return s
+000108f0: 6572 6965 7355 7070 6572 0a0a 6465 6620  eriesUpper..def 
+00010900: 5869 6444 656e 6f6d 286e 2c20 6d2c 206e  XidDenom(n, m, n
+00010910: 7072 6d5f 6d61 7829 3a0a 2020 2020 5869  prm_max):.    Xi
+00010920: 6444 656e 6f6d 203d 2077 5f4d 286e 2c6d  dDenom = w_M(n,m
+00010930: 292a 2a32 202b 2077 5f50 286e 2c6d 292a  )**2 + w_P(n,m)*
+00010940: 2a32 202d 2077 5f4d 286e 2c6d 292a 775f  *2 - w_M(n,m)*w_
+00010950: 5028 6e2d 322c 6d29 2a46 5f4d 286e 2c6d  P(n-2,m)*F_M(n,m
+00010960: 2c30 2920 2d20 775f 5028 6e2c 6d29 2a77  ,0) - w_P(n,m)*w
+00010970: 5f4d 286e 2b32 2c6d 292a 465f 5028 6e2c  _M(n+2,m)*F_P(n,
+00010980: 6d2c 302c 6e70 726d 5f6d 6178 290a 2020  m,0,nprm_max).  
+00010990: 2020 7265 7475 726e 2058 6964 4465 6e6f    return XidDeno
+000109a0: 6d0a 0a23 2323 2323 2323 2323 2323 2323  m..#############
+000109b0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000109c0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000109d0: 0a23 202d 2d20 454e 4420 5245 5645 5253  .# -- END REVERS
+000109e0: 4544 206e 2c20 6e27 204e 4f54 4154 494f  ED n, n' NOTATIO
+000109f0: 4e20 2d2d 0a23 2323 2323 2323 2323 2323  N --.###########
+00010a00: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00010a10: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00010a20: 2323 0a0a 2222 220a 6576 616c 5f64 6576  ##..""".eval_dev
+00010a30: 2829 0a20 2020 2045 7661 6c75 6174 6573  ().    Evaluates
+00010a40: 2074 6865 2064 6576 6961 7469 6f6e 2066   the deviation f
+00010a50: 726f 6d20 7370 6865 7269 6361 6c20 7379  rom spherical sy
+00010a60: 6d6d 6574 7279 2061 7320 6120 6675 6e63  mmetry as a func
+00010a70: 7469 6f6e 206f 6620 6c61 742f 6c6f 6e20  tion of lat/lon 
+00010a80: 666f 7220 6120 6769 7665 6e20 6465 6772  for a given degr
+00010a90: 6565 2070 2061 6e64 206f 7264 6572 2071  ee p and order q
+00010aa0: 206f 6620 626f 756e 6461 7279 2073 6861   of boundary sha
+00010ab0: 7065 2e0a 2020 2020 5661 6c75 6573 2066  pe..    Values f
+00010ac0: 6f72 2063 6869 5f70 7120 6172 6520 636f  or chi_pq are co
+00010ad0: 6566 6669 6369 656e 7473 2074 6861 7420  efficients that 
+00010ae0: 6d75 6c74 6970 6c79 2074 6865 2061 7373  multiply the ass
+00010af0: 6f63 6961 7465 6420 6f72 7468 6f6e 6f72  ociated orthonor
+00010b00: 6d61 6c20 7370 6865 7269 6361 6c20 6861  mal spherical ha
+00010b10: 726d 6f6e 6963 2061 6e64 2074 6865 6e0a  rmonic and then.
+00010b20: 2020 2020 6172 6520 6164 6465 6420 746f      are added to
+00010b30: 2074 6865 206e 6f6d 696e 616c 2072 6164   the nominal rad
+00010b40: 6975 732e 2052 6574 7572 6e73 2073 616d  ius. Returns sam
+00010b50: 6520 756e 6974 7320 6173 2069 6e70 7574  e units as input
+00010b60: 2063 6869 5f70 712e 0a20 2020 2055 7361   chi_pq..    Usa
+00010b70: 6765 3a20 6074 6869 735f 6465 7673 6020  ge: `this_devs` 
+00010b80: 3d20 6576 616c 5f64 6576 2860 7060 2c20  = eval_dev(`p`, 
+00010b90: 6071 602c 2060 6368 695f 7071 602c 2060  `q`, `chi_pq`, `
+00010ba0: 6c74 6874 602c 2060 6c70 6869 602c 2060  ltht`, `lphi`, `
+00010bb0: 6c6c 656e 7960 2c20 606c 6c65 6e78 6029  lleny`, `llenx`)
+00010bc0: 0a20 2020 2052 6574 7572 6e73 3a0a 2020  .    Returns:.  
+00010bd0: 2020 2020 2020 7468 6973 5f64 6576 733a        this_devs:
+00010be0: 2066 6c6f 6174 2c20 7368 6170 6528 6c6c   float, shape(ll
+00010bf0: 656e 792c 6c6c 656e 7829 2e20 426f 756e  eny,llenx). Boun
+00010c00: 6461 7279 2073 6861 7065 2064 6576 6961  dary shape devia
+00010c10: 7469 6f6e 7320 6475 6520 746f 2074 6869  tions due to thi
+00010c20: 7320 7061 7274 6963 756c 6172 2070 2c71  s particular p,q
+00010c30: 2063 6f6d 6269 6e61 7469 6f6e 2e0a 2020   combination..  
+00010c40: 2020 5061 7261 6d65 7465 7273 3a0a 2020    Parameters:.  
+00010c50: 2020 2020 2020 703a 2069 6e74 6567 6572        p: integer
+00010c60: 2e20 4465 6772 6565 206f 6620 7368 6170  . Degree of shap
+00010c70: 6520 6861 726d 6f6e 6963 2074 6f20 6265  e harmonic to be
+00010c80: 2065 7661 6c75 6174 6564 2e0a 2020 2020   evaluated..    
+00010c90: 2020 2020 713a 2069 6e74 6567 6572 2e20      q: integer. 
+00010ca0: 4f72 6465 7220 6f66 2073 6861 7065 2068  Order of shape h
+00010cb0: 6172 6d6f 6e69 6320 746f 2062 6520 6576  armonic to be ev
+00010cc0: 616c 7561 7465 642e 0a20 2020 2020 2020  aluated..       
+00010cd0: 2063 6869 5f70 713a 2063 6f6d 706c 6578   chi_pq: complex
+00010ce0: 2e20 436f 6566 6669 6369 656e 7420 666f  . Coefficient fo
+00010cf0: 7220 7370 6865 7269 6361 6c20 6861 726d  r spherical harm
+00010d00: 6f6e 6963 7320 6f66 2064 6567 7265 6520  onics of degree 
+00010d10: 616e 6420 6f72 6465 7220 702c 712c 0a20  and order p,q,. 
+00010d20: 2020 2020 2020 2020 2020 2073 7563 6820             such 
+00010d30: 7468 6174 2072 2874 6865 7461 2c20 7068  that r(theta, ph
+00010d40: 6929 203d 2052 202b 2053 756d 5b63 6869  i) = R + Sum[chi
+00010d50: 5f70 7120 2a20 5970 7128 7468 6574 612c  _pq * Ypq(theta,
+00010d60: 2070 6869 295d 2e0a 2020 2020 2020 2020   phi)]..        
+00010d70: 6c74 6874 3a20 666c 6f61 742c 2073 6861  ltht: float, sha
+00010d80: 7065 286c 6c65 6e79 2920 6f72 2073 6861  pe(lleny) or sha
+00010d90: 7065 286c 3144 292e 204c 6f63 616c 2063  pe(l1D). Local c
+00010da0: 6f70 7920 6f66 2074 6865 7461 2067 7269  opy of theta gri
+00010db0: 6420 7661 6c75 6573 2028 6661 7374 6572  d values (faster
+00010dc0: 2065 7865 6375 7469 6f6e 2074 6861 6e20   execution than 
+00010dd0: 7265 6665 7265 6e63 696e 6720 6120 676c  referencing a gl
+00010de0: 6f62 616c 2076 6172 6961 626c 6529 2e0a  obal variable)..
+00010df0: 2020 2020 2020 2020 6c70 6869 3a20 666c          lphi: fl
+00010e00: 6f61 742c 2073 6861 7065 286c 6c65 6e78  oat, shape(llenx
+00010e10: 2920 6f72 2073 6861 7065 286c 3144 292e  ) or shape(l1D).
+00010e20: 204c 6f63 616c 2063 6f70 7920 6f66 2070   Local copy of p
+00010e30: 6869 2067 7269 6420 7661 6c75 6573 2e0a  hi grid values..
+00010e40: 2020 2020 2222 220a 6465 6620 6576 616c      """.def eval
+00010e50: 5f64 6576 2870 2c20 712c 2063 6869 5f70  _dev(p, q, chi_p
+00010e60: 712c 206c 7468 742c 206c 7068 692c 206f  q, ltht, lphi, o
+00010e70: 7574 5368 6170 6529 3a0a 2020 2020 6966  utShape):.    if
+00010e80: 2063 6869 5f70 7120 3d3d 2030 3a0a 2020   chi_pq == 0:.  
+00010e90: 2020 2020 2020 7468 6973 5f64 6576 7320        this_devs 
+00010ea0: 3d20 6e70 2e7a 6572 6f73 286f 7574 5368  = np.zeros(outSh
+00010eb0: 6170 652c 2064 7479 7065 3d6e 702e 666c  ape, dtype=np.fl
+00010ec0: 6f61 745f 290a 2020 2020 656c 7365 3a0a  oat_).    else:.
+00010ed0: 2020 2020 2020 2020 7468 6973 5f64 6576          this_dev
+00010ee0: 7320 3d20 6e70 2e72 6561 6c28 6368 695f  s = np.real(chi_
+00010ef0: 7071 202a 2073 7068 5f68 6172 6d28 712c  pq * sph_harm(q,
+00010f00: 2070 2c20 6c70 6869 2c20 6c74 6874 2929   p, lphi, ltht))
+00010f10: 0a20 2020 206c 6f67 2e64 6562 7567 2866  .    log.debug(f
+00010f20: 2270 2c71 203d 207b 707d 7b71 7d20 636f  "p,q = {p}{q} co
+00010f30: 6d70 6c65 7465 6422 290a 2020 2020 7265  mpleted").    re
+00010f40: 7475 726e 2074 6869 735f 6465 7673 0a0a  turn this_devs..
+00010f50: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00010f60: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00010f70: 2323 2323 2323 2323 2323 2323 230a 0a22  #############.."
+00010f80: 2222 0a67 6574 5f72 7375 7266 2829 0a20  "".get_rsurf(). 
+00010f90: 2020 2043 616c 6375 6c61 7465 7320 7228     Calculates r(
+00010fa0: 7468 6574 612c 2070 6869 2920 6672 6f6d  theta, phi) from
+00010fb0: 2072 5f6d 6561 6e20 616e 6420 6368 695f   r_mean and chi_
+00010fc0: 7071 2c20 7768 6572 6520 7228 7468 6574  pq, where r(thet
+00010fd0: 612c 2070 6869 2920 3d20 725f 6d65 616e  a, phi) = r_mean
+00010fe0: 202b 2053 756d 5b63 6869 5f70 712a 5970   + Sum[chi_pq*Yp
+00010ff0: 7128 7468 6574 612c 2070 6869 295d 2e0a  q(theta, phi)]..
+00011000: 2020 2020 5573 6167 653a 2067 6574 5f72      Usage: get_r
+00011010: 7375 7266 2860 4269 6e6d 602c 2060 6e5f  surf(`Binm`, `n_
+00011020: 6d61 7860 2c20 6066 7061 7468 3d4e 6f6e  max`, `fpath=Non
+00011030: 6560 2c20 6064 6966 6665 7265 6e63 653d  e`, `difference=
+00011040: 5472 7565 602c 2060 4269 6e6d 5f73 7068  True`, `Binm_sph
+00011050: 3d4e 6f6e 6560 290a 2020 2020 5265 7475  =None`).    Retu
+00011060: 726e 733a 0a20 2020 2020 2020 2073 7572  rns:.        sur
+00011070: 663a 2066 6c6f 6174 2c20 7368 6170 6528  f: float, shape(
+00011080: 6c6c 656e 792c 6c6c 656e 7829 2e20 7228  lleny,llenx). r(
+00011090: 7468 6574 612c 2070 6869 2920 7661 6c75  theta, phi) valu
+000110a0: 6573 2063 6f72 7265 7370 6f6e 6469 6e67  es corresponding
+000110b0: 2074 6f20 7468 6520 696e 7075 7420 6772   to the input gr
+000110c0: 6964 206f 660a 2020 2020 2020 2020 2020  id of.          
+000110d0: 2020 6c74 6874 2061 6e64 206c 7068 6920    ltht and lphi 
+000110e0: 7661 6c75 6573 2e20 5361 6d65 2075 6e69  values. Same uni
+000110f0: 7473 2061 7320 6173 796d 5f73 6861 7065  ts as asym_shape
+00011100: 2061 6e64 2072 5f6d 6561 6e2e 0a20 2020   and r_mean..   
+00011110: 2050 6172 616d 6574 6572 733a 0a20 2020   Parameters:.   
+00011120: 2020 2020 2070 7661 6c73 2c20 7176 616c       pvals, qval
+00011130: 733a 2069 6e74 6567 6572 2c20 7368 6170  s: integer, shap
+00011140: 6528 4e70 7129 2e20 4c69 6e65 6172 2061  e(Npq). Linear a
+00011150: 7272 6179 7320 6f66 2070 6169 7265 6420  rrays of paired 
+00011160: 702c 7120 7661 6c75 6573 2066 6f72 2070  p,q values for p
+00011170: 6172 616c 6c65 6c20 636f 6d70 7574 6174  arallel computat
+00011180: 696f 6e2e 0a20 2020 2020 2020 2061 7379  ion..        asy
+00011190: 6d5f 7368 6170 653a 2063 6f6d 706c 6578  m_shape: complex
+000111a0: 2c20 7368 6170 6528 322c 705f 6d61 782b  , shape(2,p_max+
+000111b0: 312c 705f 6d61 782b 3129 2e20 4162 736f  1,p_max+1). Abso
+000111c0: 6c75 7465 2062 6f75 6e64 6172 7920 6465  lute boundary de
+000111d0: 7669 6174 696f 6e73 2066 6f72 2061 6c6c  viations for all
+000111e0: 2070 2c71 2076 616c 7565 7320 666f 7220   p,q values for 
+000111f0: 7468 650a 2020 2020 2020 2020 2020 2020  the.            
+00011200: 636f 6e73 6964 6572 6564 2073 7572 6661  considered surfa
+00011210: 6365 2e20 556e 6974 7320 6d75 7374 206d  ce. Units must m
+00011220: 6174 6368 2072 5f6d 6561 6e2e 0a20 2020  atch r_mean..   
+00011230: 2020 2020 2072 5f6d 6561 6e3a 2066 6c6f       r_mean: flo
+00011240: 6174 2e20 4d65 616e 2076 616c 7565 206f  at. Mean value o
+00011250: 6620 7261 6469 7573 2066 6f72 2074 6865  f radius for the
+00011260: 2063 6f6e 7369 6465 7265 6420 7375 7266   considered surf
+00011270: 6163 652e 2055 6e69 7473 206d 7573 7420  ace. Units must 
+00011280: 6d61 7463 6820 6173 796d 5f73 6861 7065  match asym_shape
+00011290: 2e0a 2020 2020 2020 2020 6c74 6874 3a20  ..        ltht: 
+000112a0: 666c 6f61 742c 2073 6861 7065 286c 6c65  float, shape(lle
+000112b0: 6e79 292e 204c 6f63 616c 2063 6f70 7920  ny). Local copy 
+000112c0: 6f66 2074 6865 7461 2067 7269 6420 7661  of theta grid va
+000112d0: 6c75 6573 2028 6661 7374 6572 2065 7865  lues (faster exe
+000112e0: 6375 7469 6f6e 2074 6861 6e20 7265 6665  cution than refe
+000112f0: 7265 6e63 696e 6720 6120 676c 6f62 616c  rencing a global
+00011300: 2076 6172 6961 626c 6529 2e0a 2020 2020   variable)..    
+00011310: 2020 2020 6c70 6869 3a20 666c 6f61 742c      lphi: float,
+00011320: 2073 6861 7065 286c 6c65 6e79 292e 204c   shape(lleny). L
+00011330: 6f63 616c 2063 6f70 7920 6f66 2070 6869  ocal copy of phi
+00011340: 2067 7269 6420 7661 6c75 6573 2e0a 2020   grid values..  
+00011350: 2020 2222 220a 6465 6620 6765 745f 7273    """.def get_rs
+00011360: 7572 6628 7076 616c 732c 7176 616c 732c  urf(pvals,qvals,
+00011370: 6173 796d 5f73 6861 7065 2c20 725f 6d65  asym_shape, r_me
+00011380: 616e 2c6c 7468 742c 6c70 6869 2c20 646f  an,ltht,lphi, do
+00011390: 5f70 6172 616c 6c65 6c3d 5472 7565 293a  _parallel=True):
+000113a0: 0a20 2020 204e 7071 203d 206e 702e 7369  .    Npq = np.si
+000113b0: 7a65 2870 7661 6c73 290a 2020 2020 6c6c  ze(pvals).    ll
+000113c0: 656e 7920 3d20 6e70 2e73 697a 6528 6c74  eny = np.size(lt
+000113d0: 6874 290a 2020 2020 6c6c 656e 7820 3d20  ht).    llenx = 
+000113e0: 6e70 2e73 697a 6528 6c70 6869 290a 2020  np.size(lphi).  
+000113f0: 2020 6966 206c 6c65 6e79 203d 3d20 6c6c    if lleny == ll
+00011400: 656e 783a 0a20 2020 2020 2020 2023 2041  enx:.        # A
+00011410: 7373 756d 6520 3144 2061 7272 6179 7320  ssume 1D arrays 
+00011420: 6966 2062 6f74 6820 6c74 6874 2061 6e64  if both ltht and
+00011430: 206c 7068 6920 6172 6520 7361 6d65 206c   lphi are same l
+00011440: 656e 6774 680a 2020 2020 2020 2020 6f75  ength.        ou
+00011450: 7453 6861 7065 203d 2028 6c6c 656e 7929  tShape = (lleny)
+00011460: 0a20 2020 2065 6c73 653a 0a20 2020 2020  .    else:.     
+00011470: 2020 206f 7574 5368 6170 6520 3d20 286c     outShape = (l
+00011480: 6c65 6e79 2c6c 6c65 6e78 290a 2020 2020  leny,llenx).    
+00011490: 2020 2020 6c74 6874 2c20 6c70 6869 203d      ltht, lphi =
+000114a0: 206e 702e 6d65 7368 6772 6964 286c 7468   np.meshgrid(lth
+000114b0: 742c 206c 7068 692c 2069 6e64 6578 696e  t, lphi, indexin
+000114c0: 673d 2769 6a27 290a 2020 2020 6465 7673  g='ij').    devs
+000114d0: 203d 206e 702e 7a65 726f 7328 6f75 7453   = np.zeros(outS
+000114e0: 6861 7065 290a 0a20 2020 206c 696e 5f62  hape)..    lin_b
+000114f0: 645f 7368 6170 6520 3d20 6e70 2e61 7272  d_shape = np.arr
+00011500: 6179 285b 2061 7379 6d5f 7368 6170 655b  ay([ asym_shape[
+00011510: 696e 7428 7176 616c 735b 694e 5d3c 3029  int(qvals[iN]<0)
+00011520: 2c70 7661 6c73 5b69 4e5d 2c61 6273 2871  ,pvals[iN],abs(q
+00011530: 7661 6c73 5b69 4e5d 295d 2066 6f72 2069  vals[iN])] for i
+00011540: 4e20 696e 2072 616e 6765 284e 7071 2920  N in range(Npq) 
+00011550: 5d29 0a0a 2020 2020 6966 2064 6f5f 7061  ])..    if do_pa
+00011560: 7261 6c6c 656c 3a0a 2020 2020 2020 2020  rallel:.        
+00011570: 706f 6f6c 203d 206d 7470 436f 6e74 6578  pool = mtpContex
+00011580: 742e 506f 6f6c 286e 756d 5f63 6f72 6573  t.Pool(num_cores
+00011590: 290a 2020 2020 2020 2020 7061 725f 7265  ).        par_re
+000115a0: 7375 6c74 203d 205b 706f 6f6c 2e61 7070  sult = [pool.app
+000115b0: 6c79 5f61 7379 6e63 2820 6576 616c 5f64  ly_async( eval_d
+000115c0: 6576 2c20 6172 6773 3d28 7076 616c 735b  ev, args=(pvals[
+000115d0: 694e 5d2c 7176 616c 735b 694e 5d2c 6c69  iN],qvals[iN],li
+000115e0: 6e5f 6264 5f73 6861 7065 5b69 4e5d 2c6c  n_bd_shape[iN],l
+000115f0: 7468 742c 6c70 6869 2c6f 7574 5368 6170  tht,lphi,outShap
+00011600: 6529 2029 2066 6f72 2069 4e20 696e 2072  e) ) for iN in r
+00011610: 616e 6765 284e 7071 295d 0a20 2020 2020  ange(Npq)].     
+00011620: 2020 2070 6f6f 6c2e 636c 6f73 6528 290a     pool.close().
+00011630: 2020 2020 2020 2020 706f 6f6c 2e6a 6f69          pool.joi
+00011640: 6e28 290a 0a20 2020 2020 2020 2023 2055  n()..        # U
+00011650: 6e70 6163 6b20 7468 6520 7061 7261 6c6c  npack the parall
+00011660: 656c 2070 726f 6365 7373 696e 6720 7265  el processing re
+00011670: 7375 6c74 7320 616e 6420 7375 6d20 7468  sults and sum th
+00011680: 656d 2074 6f67 6574 6865 720a 2020 2020  em together.    
+00011690: 2020 2020 666f 7220 7265 7320 696e 2070      for res in p
+000116a0: 6172 5f72 6573 756c 743a 0a20 2020 2020  ar_result:.     
+000116b0: 2020 2020 2020 2064 6576 7320 3d20 6465         devs = de
+000116c0: 7673 202b 2072 6573 2e67 6574 2829 0a20  vs + res.get(). 
+000116d0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+000116e0: 2066 6f72 2069 4e20 696e 2072 616e 6765   for iN in range
+000116f0: 284e 7071 293a 0a20 2020 2020 2020 2020  (Npq):.         
+00011700: 2020 2064 6576 7320 3d20 6465 7673 202b     devs = devs +
+00011710: 2065 7661 6c5f 6465 7628 7076 616c 735b   eval_dev(pvals[
+00011720: 694e 5d2c 7176 616c 735b 694e 5d2c 6c69  iN],qvals[iN],li
+00011730: 6e5f 6264 5f73 6861 7065 5b69 4e5d 2c6c  n_bd_shape[iN],l
+00011740: 7468 742c 6c70 6869 2c6f 7574 5368 6170  tht,lphi,outShap
+00011750: 6529 0a0a 2020 2020 6966 2072 5f6d 6561  e)..    if r_mea
+00011760: 6e20 6973 204e 6f6e 653a 0a20 2020 2020  n is None:.     
+00011770: 2020 2072 5f6d 6561 6e20 3d20 6e70 2e61     r_mean = np.a
+00011780: 6273 2861 7379 6d5f 7368 6170 655b 302c  bs(asym_shape[0,
+00011790: 302c 305d 2920 2f20 6e70 2e73 7172 7428  0,0]) / np.sqrt(
+000117a0: 342a 6e70 2e70 6929 0a20 2020 2073 7572  4*np.pi).    sur
+000117b0: 6620 3d20 6465 7673 202b 2072 5f6d 6561  f = devs + r_mea
+000117c0: 6e0a 2020 2020 7265 7475 726e 2073 7572  n.    return sur
+000117d0: 660a 0a23 2323 2323 2323 2323 2323 2323  f..#############
+000117e0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+000117f0: 2323 2323 2323 2323 2323 2323 2323 2323  ################
+00011800: 0a0a 2222 220a 6765 744d 6167 5375 7266  ..""".getMagSurf
+00011810: 2829 0a20 2020 2045 7661 6c75 6174 6573  ().    Evaluates
+00011820: 2074 6865 2069 6e64 7563 6564 206d 6167   the induced mag
+00011830: 6e65 7469 6320 6669 656c 6420 6174 2074  netic field at t
+00011840: 6865 2073 7572 6661 6365 2066 6f72 2061  he surface for a
+00011850: 6c6c 206d 6167 6e65 7469 6320 6d6f 6d65  ll magnetic mome
+00011860: 6e74 7320 4269 6e6d 2e0a 2020 2020 5573  nts Binm..    Us
+00011870: 6167 653a 2060 4278 602c 2060 4279 602c  age: `Bx`, `By`,
+00011880: 2060 427a 6020 3d20 6765 744d 6167 5375   `Bz` = getMagSu
+00011890: 7266 2860 6e76 616c 7360 2c20 606d 7661  rf(`nvals`, `mva
+000118a0: 6c73 602c 2060 4269 6e6d 602c 2060 725f  ls`, `Binm`, `r_
+000118b0: 7468 5f70 6860 2c20 606c 7468 7460 2c20  th_ph`, `ltht`, 
+000118c0: 606c 7068 6960 2c20 606e 6d61 785f 706c  `lphi`, `nmax_pl
+000118d0: 6f74 3d34 602c 2060 5363 686d 6964 743d  ot=4`, `Schmidt=
+000118e0: 4661 6c73 6560 290a 2020 2020 5265 7475  False`).    Retu
+000118f0: 726e 733a 0a20 2020 2020 2020 2042 782c  rns:.        Bx,
+00011900: 4279 2c42 7a20 2865 6163 6829 3a20 636f  By,Bz (each): co
+00011910: 6d70 6c65 782c 2073 6861 7065 286c 6c65  mplex, shape(lle
+00011920: 6e79 2c6c 6c65 6e78 292e 2041 2028 6c6c  ny,llenx). A (ll
+00011930: 656e 792c 6c6c 656e 7829 2061 7272 6179  eny,llenx) array
+00011940: 206f 6620 6669 656c 6420 7661 6c75 6573   of field values
+00011950: 2064 7565 2074 6f20 7468 6520 7061 7274   due to the part
+00011960: 6963 756c 6172 2042 696e 6d20 7661 6c75  icular Binm valu
+00011970: 6573 2070 6173 7365 642e 0a20 2020 2020  es passed..     
+00011980: 2020 2020 2020 2046 6965 6c64 2076 616c         Field val
+00011990: 7565 7320 6361 6e20 6265 206f 6274 6169  ues can be obtai
+000119a0: 6e65 6420 666f 7220 616e 7920 6675 7475  ned for any futu
+000119b0: 7265 2074 696d 6520 6279 206d 756c 7469  re time by multi
+000119c0: 706c 7969 6e67 2065 6163 6820 4269 6e6d  plying each Binm
+000119d0: 5b69 2c3a 2c3a 2c3a 5d20 6279 2074 6865  [i,:,:,:] by the
+000119e0: 2063 6f72 7265 7370 6f6e 6469 6e67 2065   corresponding e
+000119f0: 5e2d 69cf 8974 2066 6163 746f 722e 0a20  ^-i..t factor.. 
+00011a00: 2020 2020 2020 2020 2020 2074 3d30 2069             t=0 i
+00011a10: 7320 6465 6669 6e65 6420 746f 2062 6520  s defined to be 
+00011a20: 7468 6520 4a32 3030 3020 6570 6f63 682e  the J2000 epoch.
+00011a30: 0a20 2020 2050 6172 616d 6574 6572 733a  .    Parameters:
+00011a40: 0a20 2020 2020 2020 206e 7661 6c73 3a20  .        nvals: 
+00011a50: 696e 7465 6765 722c 2073 6861 7065 284e  integer, shape(N
+00011a60: 6e6d 292e 204c 696e 6561 7220 6c69 7374  nm). Linear list
+00011a70: 206f 6620 6d61 676e 6574 6963 206d 6f6d   of magnetic mom
+00011a80: 656e 7420 6465 6772 6565 7320 746f 2062  ent degrees to b
+00011a90: 6520 6576 616c 7561 7465 642e 0a20 2020  e evaluated..   
+00011aa0: 2020 2020 206d 7661 6c73 3a20 696e 7465       mvals: inte
+00011ab0: 6765 722c 2073 6861 7065 284e 6e6d 292e  ger, shape(Nnm).
+00011ac0: 204c 696e 6561 7220 6c69 7374 206f 6620   Linear list of 
+00011ad0: 6d61 676e 6574 6963 206d 6f6d 656e 7420  magnetic moment 
+00011ae0: 6f72 6465 7273 2074 6f20 6265 2065 7661  orders to be eva
+00011af0: 6c75 6174 6564 2c20 636f 7272 6573 706f  luated, correspo
+00011b00: 6e64 696e 6720 746f 206e 7661 6c73 206f  nding to nvals o
+00011b10: 6620 7468 6520 7361 6d65 2069 6e64 6578  f the same index
+00011b20: 2e0a 2020 2020 2020 2020 4269 6e6d 3a20  ..        Binm: 
+00011b30: 636f 6d70 6c65 782c 2073 6861 7065 2832  complex, shape(2
+00011b40: 2c6e 5f6d 6178 2b31 2c6e 5f6d 6178 2b31  ,n_max+1,n_max+1
+00011b50: 2920 4f52 2073 6861 7065 284e 6e6d 293b  ) OR shape(Nnm);
+00011b60: 2069 6620 5363 686d 6964 743d 5472 7565   if Schmidt=True
+00011b70: 2c20 7475 706c 6520 6f66 2028 676e 6d2c  , tuple of (gnm,
+00011b80: 686e 6d29 2e20 4d61 676e 6574 6963 206d  hnm). Magnetic m
+00011b90: 6f6d 656e 7420 6f66 2064 6567 7265 6520  oment of degree 
+00011ba0: 616e 640a 2020 2020 2020 2020 2020 2020  and.            
+00011bb0: 6f72 6465 7220 6e2c 6d20 7468 6174 2063  order n,m that c
+00011bc0: 616e 2062 6520 696e 6465 7865 6420 6279  an be indexed by
+00011bd0: 2074 6865 206d 6174 6368 6564 2065 6e74   the matched ent
+00011be0: 7269 6573 2069 6e20 6e76 616c 7320 616e  ries in nvals an
+00011bf0: 6420 6d76 616c 732e 2055 6e69 7473 206d  d mvals. Units m
+00011c00: 6174 6368 2074 6865 206f 7574 7075 7420  atch the output 
+00011c10: 6669 656c 642e 0a20 2020 2020 2020 2072  field..        r
+00011c20: 5f74 685f 7068 3a20 666c 6f61 742c 2073  _th_ph: float, s
+00011c30: 6861 7065 286c 6c65 6e79 2c6c 6c65 6e78  hape(lleny,llenx
+00011c40: 292e 204d 6573 6867 7269 6420 6172 7261  ). Meshgrid arra
+00011c50: 7920 6f66 2072 2874 6865 7461 2c20 7068  y of r(theta, ph
+00011c60: 6929 2076 616c 7565 7320 636f 7272 6573  i) values corres
+00011c70: 706f 6e64 696e 6720 746f 2074 6865 2066  ponding to the f
+00011c80: 6f6c 6c6f 7769 6e67 2074 6874 2061 6e64  ollowing tht and
+00011c90: 2070 6869 2076 616c 7565 732e 0a20 2020   phi values..   
+00011ca0: 2020 2020 2020 2020 2072 5f74 685f 7068           r_th_ph
+00011cb0: 2068 6173 2075 6e69 7473 206f 6620 525f   has units of R_
+00011cc0: 626f 6479 2c20 692e 652e 2074 6865 2070  body, i.e. the p
+00011cd0: 6879 7369 6361 6c20 7375 7266 6163 6520  hysical surface 
+00011ce0: 6973 2031 2e30 2e0a 2020 2020 2020 2020  is 1.0..        
+00011cf0: 6c74 6874 3a20 666c 6f61 742c 2073 6861  ltht: float, sha
+00011d00: 7065 286c 6c65 6e79 292e 2041 7272 6179  pe(lleny). Array
+00011d10: 206f 6620 7468 6574 6120 7661 6c75 6573   of theta values
+00011d20: 206f 7665 7220 7768 6963 6820 746f 2065   over which to e
+00011d30: 7661 6c75 6174 6520 7468 6520 6669 656c  valuate the fiel
+00011d40: 6420 636f 6d70 6f6e 656e 7473 2e0a 2020  d components..  
+00011d50: 2020 2020 2020 6c70 6869 3a20 666c 6f61        lphi: floa
+00011d60: 742c 2073 6861 7065 286c 6c65 6e78 292e  t, shape(llenx).
+00011d70: 2041 7272 6179 206f 6620 7068 6920 7661   Array of phi va
+00011d80: 6c75 6573 206f 7665 7220 7768 6963 6820  lues over which 
+00011d90: 746f 2065 7661 6c75 6174 6520 7468 6520  to evaluate the 
+00011da0: 6669 656c 6420 636f 6d70 6f6e 656e 7473  field components
+00011db0: 2e0a 2020 2020 2020 2020 6e6d 6178 5f70  ..        nmax_p
+00011dc0: 6c6f 743a 2069 6e74 6567 6572 2028 3429  lot: integer (4)
+00011dd0: 2e20 4d61 7869 6d75 6d20 7661 6c75 6520  . Maximum value 
+00011de0: 6f66 206e 2066 6f72 2065 7661 6c75 6174  of n for evaluat
+00011df0: 696e 6720 6d61 676e 6574 6963 2066 6965  ing magnetic fie
+00011e00: 6c64 732e 2065 7661 6c5f 4269 206d 7573  lds. eval_Bi mus
+00011e10: 7420 6861 7665 2065 6163 6820 6e20 6578  t have each n ex
+00011e20: 706c 6963 6974 6c79 2068 6172 642d 636f  plicitly hard-co
+00011e30: 6465 642c 0a20 2020 2020 2020 2020 2020  ded,.           
+00011e40: 2077 6869 6368 2068 6173 206f 6e6c 7920   which has only 
+00011e50: 6265 656e 2064 6f6e 6520 7570 2074 6f20  been done up to 
+00011e60: 6e3d 3420 6265 6361 7573 6520 6c61 7267  n=4 because larg
+00011e70: 6572 2d64 6567 7265 6520 6d6f 6d65 6e74  er-degree moment
+00011e80: 7320 6172 6520 6578 7065 6374 6564 2074  s are expected t
+00011e90: 6f20 6861 7665 2073 6d61 6c6c 2063 6f6e  o have small con
+00011ea0: 7472 6962 7574 696f 6e73 2061 7420 616c  tributions at al
+00011eb0: 7469 7475 6465 2e0a 2020 2020 2020 2020  titude..        
+00011ec0: 5363 686d 6964 743a 2062 6f6f 6c65 616e  Schmidt: boolean
+00011ed0: 2028 4661 6c73 6529 2e20 5768 6574 6865   (False). Whethe
+00011ee0: 7220 696e 7075 7420 6d61 676e 6574 6963  r input magnetic
+00011ef0: 206d 6f6d 656e 7473 2061 7265 2069 6e20   moments are in 
+00011f00: 5363 686d 6964 7420 7365 6d69 2d6e 6f72  Schmidt semi-nor
+00011f10: 6d61 6c69 7a65 6420 666f 726d 2077 6974  malized form wit
+00011f20: 686f 7574 2043 6f6e 646f 6e2d 5368 6f72  hout Condon-Shor
+00011f30: 746c 6579 0a20 2020 2020 2020 2020 2020  tley.           
+00011f40: 2070 6861 7365 2e20 4966 2046 616c 7365   phase. If False
+00011f50: 2c20 6d6f 6d65 6e74 7320 6d75 7374 2062  , moments must b
+00011f60: 6520 696e 2066 756c 6c79 206e 6f72 6d61  e in fully norma
+00011f70: 6c69 7a65 6420 666f 726d 2077 6974 6820  lized form with 
+00011f80: 7468 6520 436f 6e64 6f6e 2d53 686f 7274  the Condon-Short
+00011f90: 6c65 7920 7068 6173 652e 0a20 2020 2020  ley phase..     
+00011fa0: 2020 2067 6e6d 2c20 686e 6d3a 2063 6f6d     gnm, hnm: com
+00011fb0: 706c 6578 2c20 7368 6170 6528 6e5f 6d61  plex, shape(n_ma
+00011fc0: 782b 312c 6e5f 6d61 782b 3129 2e20 5363  x+1,n_max+1). Sc
+00011fd0: 686d 6964 7420 7365 6d69 2d6e 6f72 6d61  hmidt semi-norma
+00011fe0: 6c69 7a65 6420 6d61 676e 6574 6963 206d  lized magnetic m
+00011ff0: 6f6d 656e 7473 2e20 5061 7373 6564 2061  oments. Passed a
+00012000: 7320 6120 7475 706c 6520 696e 2042 696e  s a tuple in Bin
+00012010: 6d2e 0a20 2020 2022 2222 0a64 6566 2067  m..    """.def g
+00012020: 6574 4d61 6753 7572 6628 6e76 616c 732c  etMagSurf(nvals,
+00012030: 6d76 616c 732c 4269 6e6d 2c20 725f 7468  mvals,Binm, r_th
+00012040: 5f70 682c 6c74 6874 2c6c 7068 692c 206e  _ph,ltht,lphi, n
+00012050: 6d61 785f 706c 6f74 3d31 302c 2053 6368  max_plot=10, Sch
+00012060: 6d69 6474 3d46 616c 7365 2c20 646f 5f70  midt=False, do_p
+00012070: 6172 616c 6c65 6c3d 5472 7565 293a 0a20  arallel=True):. 
+00012080: 2020 2069 6620 6e6d 6178 5f70 6c6f 7420     if nmax_plot 
+00012090: 3e20 3130 3a0a 2020 2020 2020 2020 6e6d  > 10:.        nm
+000120a0: 6178 5f70 6c6f 7420 3d20 3130 0a20 2020  ax_plot = 10.   
+000120b0: 2020 2020 206c 6f67 2e77 6172 6e69 6e67       log.warning
+000120c0: 2866 2245 7661 6c75 6174 696f 6e20 6f66  (f"Evaluation of
+000120d0: 206d 6167 6e65 7469 6320 6669 656c 6473   magnetic fields
+000120e0: 2069 7320 7375 7070 6f72 7465 6420 6f6e   is supported on
+000120f0: 6c79 2075 7020 746f 206e 3d7b 6e6d 6178  ly up to n={nmax
+00012100: 5f70 6c6f 747d 2e20 6e6d 6178 5f70 6c6f  _plot}. nmax_plo
+00012110: 7420 6861 7320 6265 656e 2073 6574 2074  t has been set t
+00012120: 6f20 7b6e 6d61 785f 706c 6f74 7d2e 2229  o {nmax_plot}.")
+00012130: 0a0a 2020 2020 6966 2053 6368 6d69 6474  ..    if Schmidt
+00012140: 3a0a 2020 2020 2020 2020 4e6e 6d20 3d20  :.        Nnm = 
+00012150: 6d69 6e28 2069 6e74 2828 6e6d 6178 5f70  min( int((nmax_p
+00012160: 6c6f 742b 3129 2a28 6e6d 6178 5f70 6c6f  lot+1)*(nmax_plo
+00012170: 742b 3229 2f32 2920 2d20 312c 206e 702e  t+2)/2) - 1, np.
+00012180: 7369 7a65 286e 7661 6c73 2920 290a 2020  size(nvals) ).  
+00012190: 2020 2020 2020 676e 6d2c 2068 6e6d 203d        gnm, hnm =
+000121a0: 2042 696e 6d0a 2020 2020 2020 2020 6966   Binm.        if
+000121b0: 206e 702e 7369 7a65 286e 702e 7368 6170   np.size(np.shap
+000121c0: 6528 676e 6d29 2920 3e20 313a 0a20 2020  e(gnm)) > 1:.   
+000121d0: 2020 2020 2020 2020 206c 696e 5f67 6e6d           lin_gnm
+000121e0: 203d 206e 702e 6172 7261 7928 5b67 6e6d   = np.array([gnm
+000121f0: 5b6e 7661 6c73 5b69 4e5d 2c20 6d76 616c  [nvals[iN], mval
+00012200: 735b 694e 5d5d 2066 6f72 2069 4e20 696e  s[iN]] for iN in
+00012210: 2072 616e 6765 284e 6e6d 295d 290a 2020   range(Nnm)]).  
+00012220: 2020 2020 2020 2020 2020 6c69 6e5f 686e            lin_hn
+00012230: 6d20 3d20 6e70 2e61 7272 6179 285b 686e  m = np.array([hn
+00012240: 6d5b 6e76 616c 735b 694e 5d2c 206d 7661  m[nvals[iN], mva
+00012250: 6c73 5b69 4e5d 5d20 666f 7220 694e 2069  ls[iN]] for iN i
+00012260: 6e20 7261 6e67 6528 4e6e 6d29 5d29 0a20  n range(Nnm)]). 
+00012270: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+00012280: 2020 2020 2020 2020 206c 696e 5f67 6e6d           lin_gnm
+00012290: 203d 2067 6e6d 0a20 2020 2020 2020 2020   = gnm.         
+000122a0: 2020 206c 696e 5f68 6e6d 203d 2068 6e6d     lin_hnm = hnm
+000122b0: 0a20 2020 2065 6c73 653a 0a20 2020 2020  .    else:.     
+000122c0: 2020 204e 6e6d 203d 206d 696e 2828 6e6d     Nnm = min((nm
+000122d0: 6178 5f70 6c6f 7420 2b20 3129 202a 2a20  ax_plot + 1) ** 
+000122e0: 3220 2d20 312c 206e 702e 7369 7a65 286e  2 - 1, np.size(n
+000122f0: 7661 6c73 2929 0a20 2020 2020 2020 2069  vals)).        i
+00012300: 6620 6e70 2e73 697a 6528 6e70 2e73 6861  f np.size(np.sha
+00012310: 7065 2842 696e 6d29 2920 3e20 323a 0a20  pe(Binm)) > 2:. 
+00012320: 2020 2020 2020 2020 2020 206c 696e 5f42             lin_B
+00012330: 696e 6d20 3d20 6e70 2e61 7272 6179 285b  inm = np.array([
+00012340: 2042 696e 6d5b 696e 7428 6d76 616c 735b   Binm[int(mvals[
+00012350: 694e 5d3c 3029 2c6e 7661 6c73 5b69 4e5d  iN]<0),nvals[iN]
+00012360: 2c61 6273 286d 7661 6c73 5b69 4e5d 295d  ,abs(mvals[iN])]
+00012370: 2066 6f72 2069 4e20 696e 2072 616e 6765   for iN in range
+00012380: 284e 6e6d 2920 5d29 0a20 2020 2020 2020  (Nnm) ]).       
+00012390: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+000123a0: 2020 206c 696e 5f42 696e 6d20 3d20 4269     lin_Binm = Bi
+000123b0: 6e6d 0a0a 2020 2020 6c6c 656e 7920 3d20  nm..    lleny = 
+000123c0: 6e70 2e73 697a 6528 6c74 6874 290a 2020  np.size(ltht).  
+000123d0: 2020 6c6c 656e 7820 3d20 6e70 2e73 697a    llenx = np.siz
+000123e0: 6528 6c70 6869 290a 2020 2020 4278 2c20  e(lphi).    Bx, 
+000123f0: 4279 2c20 427a 203d 2028 206e 702e 7a65  By, Bz = ( np.ze
+00012400: 726f 7328 2831 2c6c 6c65 6e79 2a6c 6c65  ros((1,lleny*lle
+00012410: 6e78 292c 2064 7479 7065 3d6e 702e 636f  nx), dtype=np.co
+00012420: 6d70 6c65 785f 2920 666f 7220 5f20 696e  mplex_) for _ in
+00012430: 2072 616e 6765 2833 2920 290a 0a20 2020   range(3) )..   
+00012440: 2023 2049 6620 7765 2070 6173 7320 6120   # If we pass a 
+00012450: 7369 6e67 6c65 2076 616c 7565 2066 6f72  single value for
+00012460: 2072 2874 6865 7461 2c20 7068 6929 203d   r(theta, phi) =
+00012470: 2052 2c20 6576 616c 7561 7465 206f 7665   R, evaluate ove
+00012480: 7220 6120 7370 6865 7265 2077 6974 6820  r a sphere with 
+00012490: 7468 6174 2072 6164 6975 732e 0a20 2020  that radius..   
+000124a0: 2023 204f 7468 6572 7769 7365 2c20 6576   # Otherwise, ev
+000124b0: 616c 7561 7465 202a 6174 2a20 7468 6520  aluate *at* the 
+000124c0: 6173 796d 6d65 7472 6963 2033 4420 7375  asymmetric 3D su
+000124d0: 7266 6163 652e 0a20 2020 2069 6620 6e6f  rface..    if no
+000124e0: 7420 6973 696e 7374 616e 6365 2872 5f74  t isinstance(r_t
+000124f0: 685f 7068 2c20 4974 6572 6162 6c65 293a  h_ph, Iterable):
+00012500: 0a20 2020 2020 2020 2078 203d 206e 702e  .        x = np.
+00012510: 6172 7261 7928 5b20 725f 7468 5f70 682a  array([ r_th_ph*
+00012520: 6e70 2e73 696e 2874 6874 6929 2a6e 702e  np.sin(thti)*np.
+00012530: 636f 7328 7068 6969 2920 666f 7220 7468  cos(phii) for th
+00012540: 7469 2069 6e20 6c74 6874 2066 6f72 2070  ti in ltht for p
+00012550: 6869 6920 696e 206c 7068 6920 5d29 0a20  hii in lphi ]). 
+00012560: 2020 2020 2020 2079 203d 206e 702e 6172         y = np.ar
+00012570: 7261 7928 5b20 725f 7468 5f70 682a 6e70  ray([ r_th_ph*np
+00012580: 2e73 696e 2874 6874 6929 2a6e 702e 7369  .sin(thti)*np.si
+00012590: 6e28 7068 6969 2920 666f 7220 7468 7469  n(phii) for thti
+000125a0: 2069 6e20 6c74 6874 2066 6f72 2070 6869   in ltht for phi
+000125b0: 6920 696e 206c 7068 6920 5d29 0a20 2020  i in lphi ]).   
+000125c0: 2020 2020 207a 203d 206e 702e 6172 7261       z = np.arra
+000125d0: 7928 5b20 725f 7468 5f70 682a 6e70 2e63  y([ r_th_ph*np.c
+000125e0: 6f73 2874 6874 6929 2066 6f72 2074 6874  os(thti) for tht
+000125f0: 6920 696e 206c 7468 7420 666f 7220 5f20  i in ltht for _ 
+00012600: 696e 206c 7068 6920 5d29 0a20 2020 2020  in lphi ]).     
+00012610: 2020 2072 203d 206e 702e 7a65 726f 7328     r = np.zeros(
+00012620: 2831 2c6c 6c65 6e79 2a6c 6c65 6e78 2929  (1,lleny*llenx))
+00012630: 202b 2072 5f74 685f 7068 0a20 2020 2065   + r_th_ph.    e
+00012640: 6c73 653a 0a20 2020 2020 2020 2078 203d  lse:.        x =
+00012650: 206e 702e 6172 7261 7928 5b20 725f 7468   np.array([ r_th
+00012660: 5f70 685b 695f 7468 2c69 5f70 685d 2a6e  _ph[i_th,i_ph]*n
+00012670: 702e 7369 6e28 6c74 6874 5b69 5f74 685d  p.sin(ltht[i_th]
+00012680: 292a 6e70 2e63 6f73 286c 7068 695b 695f  )*np.cos(lphi[i_
+00012690: 7068 5d29 2066 6f72 2069 5f74 6820 696e  ph]) for i_th in
+000126a0: 2072 616e 6765 286c 6c65 6e79 2920 666f   range(lleny) fo
+000126b0: 7220 695f 7068 2069 6e20 7261 6e67 6528  r i_ph in range(
+000126c0: 6c6c 656e 7829 205d 290a 2020 2020 2020  llenx) ]).      
+000126d0: 2020 7920 3d20 6e70 2e61 7272 6179 285b    y = np.array([
+000126e0: 2072 5f74 685f 7068 5b69 5f74 682c 695f   r_th_ph[i_th,i_
+000126f0: 7068 5d2a 6e70 2e73 696e 286c 7468 745b  ph]*np.sin(ltht[
+00012700: 695f 7468 5d29 2a6e 702e 7369 6e28 6c70  i_th])*np.sin(lp
+00012710: 6869 5b69 5f70 685d 2920 666f 7220 695f  hi[i_ph]) for i_
+00012720: 7468 2069 6e20 7261 6e67 6528 6c6c 656e  th in range(llen
+00012730: 7929 2066 6f72 2069 5f70 6820 696e 2072  y) for i_ph in r
+00012740: 616e 6765 286c 6c65 6e78 2920 5d29 0a20  ange(llenx) ]). 
+00012750: 2020 2020 2020 207a 203d 206e 702e 6172         z = np.ar
+00012760: 7261 7928 5b20 725f 7468 5f70 685b 695f  ray([ r_th_ph[i_
+00012770: 7468 2c69 5f70 685d 2a6e 702e 636f 7328  th,i_ph]*np.cos(
+00012780: 6c74 6874 5b69 5f74 685d 2920 666f 7220  ltht[i_th]) for 
+00012790: 695f 7468 2069 6e20 7261 6e67 6528 6c6c  i_th in range(ll
+000127a0: 656e 7929 2066 6f72 2069 5f70 6820 696e  eny) for i_ph in
+000127b0: 2072 616e 6765 286c 6c65 6e78 2920 5d29   range(llenx) ])
+000127c0: 0a20 2020 2020 2020 2072 203d 206e 702e  .        r = np.
+000127d0: 7265 7368 6170 6528 725f 7468 5f70 682c  reshape(r_th_ph,
+000127e0: 2028 312c 6c6c 656e 792a 6c6c 656e 7829   (1,lleny*llenx)
+000127f0: 290a 0a20 2020 2069 6620 646f 5f70 6172  )..    if do_par
+00012800: 616c 6c65 6c3a 0a20 2020 2020 2020 2069  allel:.        i
+00012810: 6620 5363 686d 6964 743a 0a20 2020 2020  f Schmidt:.     
+00012820: 2020 2020 2020 2070 6f6f 6c20 3d20 6d74         pool = mt
+00012830: 7043 6f6e 7465 7874 2e50 6f6f 6c28 6e75  pContext.Pool(nu
+00012840: 6d5f 636f 7265 7329 0a20 2020 2020 2020  m_cores).       
+00012850: 2020 2020 2070 6172 5f72 6573 756c 7420       par_result 
+00012860: 3d20 5b70 6f6f 6c2e 6170 706c 795f 6173  = [pool.apply_as
+00012870: 796e 6328 2065 7661 6c5f 4269 5f53 6368  ync( eval_Bi_Sch
+00012880: 6d69 6474 2c20 6172 6773 3d28 6e76 616c  midt, args=(nval
+00012890: 735b 694e 5d2c 6d76 616c 735b 694e 5d2c  s[iN],mvals[iN],
+000128a0: 6c69 6e5f 676e 6d5b 694e 5d2c 6c69 6e5f  lin_gnm[iN],lin_
+000128b0: 686e 6d5b 694e 5d2c 2078 2c79 2c7a 2c72  hnm[iN], x,y,z,r
+000128c0: 2920 2920 666f 7220 694e 2069 6e20 7261  ) ) for iN in ra
+000128d0: 6e67 6528 4e6e 6d29 5d0a 2020 2020 2020  nge(Nnm)].      
+000128e0: 2020 2020 2020 706f 6f6c 2e63 6c6f 7365        pool.close
+000128f0: 2829 0a20 2020 2020 2020 2020 2020 2070  ().            p
+00012900: 6f6f 6c2e 6a6f 696e 2829 0a20 2020 2020  ool.join().     
+00012910: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00012920: 2020 2020 2070 6f6f 6c20 3d20 6d74 7043       pool = mtpC
+00012930: 6f6e 7465 7874 2e50 6f6f 6c28 6e75 6d5f  ontext.Pool(num_
+00012940: 636f 7265 7329 0a20 2020 2020 2020 2020  cores).         
+00012950: 2020 2070 6172 5f72 6573 756c 7420 3d20     par_result = 
+00012960: 5b70 6f6f 6c2e 6170 706c 795f 6173 796e  [pool.apply_asyn
+00012970: 6328 2065 7661 6c5f 4269 2c20 6172 6773  c( eval_Bi, args
+00012980: 3d28 6e76 616c 735b 694e 5d2c 6d76 616c  =(nvals[iN],mval
+00012990: 735b 694e 5d2c 6c69 6e5f 4269 6e6d 5b69  s[iN],lin_Binm[i
+000129a0: 4e5d 2c20 782c 792c 7a2c 7229 2029 2066  N], x,y,z,r) ) f
+000129b0: 6f72 2069 4e20 696e 2072 616e 6765 284e  or iN in range(N
+000129c0: 6e6d 295d 0a20 2020 2020 2020 2020 2020  nm)].           
+000129d0: 2070 6f6f 6c2e 636c 6f73 6528 290a 2020   pool.close().  
+000129e0: 2020 2020 2020 2020 2020 706f 6f6c 2e6a            pool.j
+000129f0: 6f69 6e28 290a 2020 2020 2020 2020 2320  oin().        # 
+00012a00: 556e 7061 636b 2072 6573 756c 7473 2066  Unpack results f
+00012a10: 726f 6d20 7061 7261 6c6c 656c 2070 726f  rom parallel pro
+00012a20: 6365 7373 696e 6720 616e 6420 7375 6d20  cessing and sum 
+00012a30: 7468 656d 0a20 2020 2020 2020 2066 6f72  them.        for
+00012a40: 2072 6573 2069 6e20 7061 725f 7265 7375   res in par_resu
+00012a50: 6c74 3a0a 2020 2020 2020 2020 2020 2020  lt:.            
+00012a60: 7468 6973 5f42 782c 2074 6869 735f 4279  this_Bx, this_By
+00012a70: 2c20 7468 6973 5f42 7a20 3d20 7265 732e  , this_Bz = res.
+00012a80: 6765 7428 290a 2020 2020 2020 2020 2020  get().          
+00012a90: 2020 4278 203d 2042 7820 2b20 7468 6973    Bx = Bx + this
+00012aa0: 5f42 780a 2020 2020 2020 2020 2020 2020  _Bx.            
+00012ab0: 4279 203d 2042 7920 2b20 7468 6973 5f42  By = By + this_B
+00012ac0: 790a 2020 2020 2020 2020 2020 2020 427a  y.            Bz
+00012ad0: 203d 2042 7a20 2b20 7468 6973 5f42 7a0a   = Bz + this_Bz.
+00012ae0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00012af0: 2020 666f 7220 694e 2069 6e20 7261 6e67    for iN in rang
+00012b00: 6528 4e6e 6d29 3a0a 2020 2020 2020 2020  e(Nnm):.        
+00012b10: 2020 2020 6966 2053 6368 6d69 6474 3a0a      if Schmidt:.
+00012b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012b30: 7468 6973 5f42 782c 2074 6869 735f 4279  this_Bx, this_By
+00012b40: 2c20 7468 6973 5f42 7a20 3d20 6576 616c  , this_Bz = eval
+00012b50: 5f42 695f 5363 686d 6964 7428 6e76 616c  _Bi_Schmidt(nval
+00012b60: 735b 694e 5d2c 206d 7661 6c73 5b69 4e5d  s[iN], mvals[iN]
+00012b70: 2c20 6c69 6e5f 676e 6d5b 694e 5d2c 206c  , lin_gnm[iN], l
+00012b80: 696e 5f68 6e6d 5b69 4e5d 2c20 782c 2079  in_hnm[iN], x, y
+00012b90: 2c20 7a2c 2072 290a 2020 2020 2020 2020  , z, r).        
+00012ba0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00012bb0: 2020 2020 2020 2020 2020 7468 6973 5f42            this_B
+00012bc0: 782c 2074 6869 735f 4279 2c20 7468 6973  x, this_By, this
+00012bd0: 5f42 7a20 3d20 6576 616c 5f42 6928 6e76  _Bz = eval_Bi(nv
+00012be0: 616c 735b 694e 5d2c 6d76 616c 735b 694e  als[iN],mvals[iN
+00012bf0: 5d2c 6c69 6e5f 4269 6e6d 5b69 4e5d 2c20  ],lin_Binm[iN], 
+00012c00: 782c 792c 7a2c 7229 0a20 2020 2020 2020  x,y,z,r).       
+00012c10: 2020 2020 2042 7820 3d20 4278 202b 2074       Bx = Bx + t
+00012c20: 6869 735f 4278 0a20 2020 2020 2020 2020  his_Bx.         
+00012c30: 2020 2042 7920 3d20 4279 202b 2074 6869     By = By + thi
+00012c40: 735f 4279 0a20 2020 2020 2020 2020 2020  s_By.           
+00012c50: 2042 7a20 3d20 427a 202b 2074 6869 735f   Bz = Bz + this_
+00012c60: 427a 0a0a 2020 2020 4278 203d 206e 702e  Bz..    Bx = np.
+00012c70: 7265 7368 6170 6528 4278 2c20 286c 6c65  reshape(Bx, (lle
+00012c80: 6e79 2c6c 6c65 6e78 2929 0a20 2020 2042  ny,llenx)).    B
+00012c90: 7920 3d20 6e70 2e72 6573 6861 7065 2842  y = np.reshape(B
+00012ca0: 792c 2028 6c6c 656e 792c 6c6c 656e 7829  y, (lleny,llenx)
+00012cb0: 290a 2020 2020 427a 203d 206e 702e 7265  ).    Bz = np.re
+00012cc0: 7368 6170 6528 427a 2c20 286c 6c65 6e79  shape(Bz, (lleny
+00012cd0: 2c6c 6c65 6e78 2929 0a20 2020 2072 6574  ,llenx)).    ret
+00012ce0: 7572 6e20 4278 2c20 4279 2c20 427a 0a0a  urn Bx, By, Bz..
+00012cf0: 0a64 6566 206e 6f72 6d34 7069 286e 2c20  .def norm4pi(n, 
+00012d00: 6d29 3a0a 2020 2020 2222 220a 2020 2020  m):.    """.    
+00012d10: 4361 6c63 756c 6174 6520 6e6f 726d 616c  Calculate normal
+00012d20: 697a 6174 696f 6e20 6661 6374 6f72 2066  ization factor f
+00012d30: 6f72 2034 7069 2d6e 6f72 6d61 6c69 7a65  or 4pi-normalize
+00012d40: 6420 7370 6865 7269 6361 6c20 6861 726d  d spherical harm
+00012d50: 6f6e 6963 732e 0a20 2020 2041 7267 733a  onics..    Args:
+00012d60: 0a20 2020 2020 2020 206e 3a20 696e 742e  .        n: int.
+00012d70: 2044 6567 7265 6520 6f66 2073 7068 6572   Degree of spher
+00012d80: 6963 616c 2068 6172 6d6f 6e69 632e 0a20  ical harmonic.. 
+00012d90: 2020 2020 2020 206d 3a20 696e 742e 204f         m: int. O
+00012da0: 7264 6572 206f 6620 7370 6865 7269 6361  rder of spherica
+00012db0: 6c20 6861 726d 6f6e 6963 2e0a 0a20 2020  l harmonic...   
+00012dc0: 2052 6574 7572 6e73 3a0a 2020 2020 2020   Returns:.      
+00012dd0: 2020 6e6f 726d 3a20 666c 6f61 742e 204e    norm: float. N
+00012de0: 6f72 6d61 6c69 7a61 7469 6f6e 2066 6163  ormalization fac
+00012df0: 746f 722c 206e 6f74 2069 6e63 6c75 6469  tor, not includi
+00012e00: 6e67 2061 6e79 2070 6f73 7369 626c 6520  ng any possible 
+00012e10: 436f 6e64 6f6e 2d53 686f 7274 6c65 7920  Condon-Shortley 
+00012e20: 7068 6173 652e 0a20 2020 2022 2222 0a20  phase..    """. 
+00012e30: 2020 206e 6f72 6d20 3d20 6e70 2e73 7172     norm = np.sqr
+00012e40: 7428 322a 6e20 2b20 3129 0a20 2020 2069  t(2*n + 1).    i
+00012e50: 6620 6d20 213d 2030 3a0a 2020 2020 2020  f m != 0:.      
+00012e60: 2020 6e6f 726d 203d 206e 6f72 6d20 2a20    norm = norm * 
+00012e70: 6e70 2e73 7172 7428 3220 2a20 6674 286e  np.sqrt(2 * ft(n
+00012e80: 202d 2061 6273 286d 2929 202f 2066 7428   - abs(m)) / ft(
+00012e90: 6e20 2b20 6162 7328 6d29 2929 0a20 2020  n + abs(m))).   
+00012ea0: 2072 6574 7572 6e20 6e6f 726d 0a0a 0a64   return norm...d
+00012eb0: 6566 2073 7068 6572 6861 726d 3470 6928  ef spherharm4pi(
+00012ec0: 6e2c 206d 2c20 6c74 6874 2c20 6c70 6869  n, m, ltht, lphi
+00012ed0: 293a 0a20 2020 2022 2222 0a20 2020 2044  ):.    """.    D
+00012ee0: 6574 6572 6d69 6e65 7320 7468 6520 3470  etermines the 4p
+00012ef0: 692d 6e6f 726d 616c 697a 6564 2073 7572  i-normalized sur
+00012f00: 6661 6365 2073 7068 6572 6963 616c 2068  face spherical h
+00012f10: 6172 6d6f 6e69 6320 7769 7468 6f75 7420  armonic without 
+00012f20: 7468 6520 436f 6e64 6f6e 2d53 686f 7274  the Condon-Short
+00012f30: 6c65 7920 7068 6173 652e 0a20 2020 2041  ley phase..    A
+00012f40: 7267 733a 0a20 2020 2020 2020 206e 3a20  rgs:.        n: 
+00012f50: 696e 742e 2044 6567 7265 6520 6f66 2073  int. Degree of s
+00012f60: 7068 6572 6963 616c 2068 6172 6d6f 6e69  pherical harmoni
+00012f70: 6320 746f 2065 7661 6c75 6174 652e 0a20  c to evaluate.. 
+00012f80: 2020 2020 2020 206d 3a20 696e 742e 204f         m: int. O
+00012f90: 7264 6572 206f 6620 7370 6865 7269 6361  rder of spherica
+00012fa0: 6c20 6861 726d 6f6e 6963 2074 6f20 6576  l harmonic to ev
+00012fb0: 616c 7561 7465 2e0a 2020 2020 2020 2020  aluate..        
+00012fc0: 6c74 6874 3a20 666c 6f61 742c 2073 6861  ltht: float, sha
+00012fd0: 7065 286c 6c65 6e79 292e 2031 4420 6c69  pe(lleny). 1D li
+00012fe0: 7374 2061 6c6f 6e67 2074 6865 7461 2061  st along theta a
+00012ff0: 7420 7768 6963 6820 746f 2065 7661 6c75  t which to evalu
+00013000: 6174 652e 0a20 2020 2020 2020 206c 7068  ate..        lph
+00013010: 693a 2066 6c6f 6174 2c20 7368 6170 6528  i: float, shape(
+00013020: 6c6c 656e 7829 2e20 3144 206c 6973 7420  llenx). 1D list 
+00013030: 616c 6f6e 6720 7068 6920 6174 2077 6869  along phi at whi
+00013040: 6368 2074 6f20 6576 616c 7561 7465 2e0a  ch to evaluate..
+00013050: 0a20 2020 2052 6574 7572 6e73 3a0a 2020  .    Returns:.  
+00013060: 2020 2020 2020 6353 6e6d 2c20 7353 6e6d        cSnm, sSnm
+00013070: 3a20 666c 6f61 742c 2073 6861 7065 286c  : float, shape(l
+00013080: 6c65 6e79 2c20 6c6c 656e 7829 2e20 5265  leny, llenx). Re
+00013090: 616c 2073 7572 6661 6365 2073 7068 6572  al surface spher
+000130a0: 6963 616c 2068 6172 6d6f 6e69 6373 2069  ical harmonics i
+000130b0: 6e20 3470 6920 6e6f 726d 616c 697a 6174  n 4pi normalizat
+000130c0: 696f 6e0a 2020 2020 2020 2020 2020 2020  ion.            
+000130d0: 666f 7220 696e 7075 7420 6e2c 206d 2e20  for input n, m. 
+000130e0: 6353 6e6d 2069 7320 7468 6520 636f 7320  cSnm is the cos 
+000130f0: 6f66 2074 6573 7365 7261 6c20 7061 7274  of tesseral part
+00013100: 2061 6e64 2073 536e 6d20 6973 2074 6865   and sSnm is the
+00013110: 2073 696e 2070 6172 742e 0a20 2020 2022   sin part..    "
+00013120: 2222 0a20 2020 206e 6f72 6d20 3d20 6e6f  "".    norm = no
+00013130: 726d 3470 6928 6e2c 206d 2920 2a20 282d  rm4pi(n, m) * (-
+00013140: 3129 2a2a 6d20 2023 2053 6369 7079 206c  1)**m  # Scipy l
+00013150: 706d 7620 6675 6e63 7469 6f6e 2028 6c65  pmv function (le
+00013160: 6765 6e70 2920 696e 636c 7564 6573 2043  genp) includes C
+00013170: 6f6e 646f 6e2d 5368 6f72 746c 6579 2070  ondon-Shortley p
+00013180: 6861 7365 3b20 7468 6973 2072 656d 6f76  hase; this remov
+00013190: 6573 2069 742e 0a20 2020 2050 6e6d 203d  es it..    Pnm =
+000131a0: 206e 6f72 6d20 2a20 6c65 6765 6e70 286d   norm * legenp(m
+000131b0: 2c20 6e2c 206e 702e 636f 7328 6c74 6874  , n, np.cos(ltht
+000131c0: 2929 2020 2320 5363 6970 7920 6c70 6d76  ))  # Scipy lpmv
+000131d0: 2061 6c73 6f20 6861 7320 6e20 616e 6420   also has n and 
+000131e0: 6d20 7265 7665 7273 6564 2d2d 6d20 6669  m reversed--m fi
+000131f0: 7273 742e 0a20 2020 2063 6d70 6869 203d  rst..    cmphi =
+00013200: 206e 702e 636f 7328 6d2a 6c70 6869 290a   np.cos(m*lphi).
+00013210: 2020 2020 736d 7068 6920 3d20 6e70 2e73      smphi = np.s
+00013220: 696e 286d 2a6c 7068 6929 0a20 2020 2063  in(m*lphi).    c
+00013230: 536e 6d20 3d20 6e70 2e73 7175 6565 7a65  Snm = np.squeeze
+00013240: 286e 702e 6172 7261 7928 5b63 6d70 6869  (np.array([cmphi
+00013250: 202a 2050 6e6d 6920 666f 7220 506e 6d69   * Pnmi for Pnmi
+00013260: 2069 6e20 506e 6d5d 2929 0a20 2020 2073   in Pnm])).    s
+00013270: 536e 6d20 3d20 6e70 2e73 7175 6565 7a65  Snm = np.squeeze
+00013280: 286e 702e 6172 7261 7928 5b73 6d70 6869  (np.array([smphi
+00013290: 202a 2050 6e6d 6920 666f 7220 506e 6d69   * Pnmi for Pnmi
+000132a0: 2069 6e20 506e 6d5d 2929 0a0a 2020 2020   in Pnm]))..    
+000132b0: 7265 7475 726e 2063 536e 6d20 2b20 7353  return cSnm + sS
+000132c0: 6e6d 0a                                  nm.
```

### Comparing `MoonMag-1.5.2/src/MoonMag/calc_Ganymede_induced.py` & `MoonMag-1.5.3/MoonMag/calc_Ganymede_induced.py`

 * *Files identical despite different names*

### Comparing `MoonMag-1.5.2/src/MoonMag/calc_trajec_induced.py` & `MoonMag-1.5.3/MoonMag/calc_trajec_induced.py`

 * *Files identical despite different names*

### Comparing `MoonMag-1.5.2/src/MoonMag/config.py` & `MoonMag-1.5.3/MoonMag/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,53 +2,62 @@
     and dependent functions.
     Developed in Python 3.8 for "A perturbation method for evaluating the
     magnetic field induced from an arbitrary, asymmetric ocean world 
     analytically" by Styczinski et al.
     DOI: 10.1016/j.icarus.2021.114840
 Author: M. J. Styczinski, mjstyczi@uw.edu """   
 
-import logging
+import logging, shutil
 
 # @@@@@@@@@@@@@@@@@
 #   Main settings
 # @@@@@@@@@@@@@@@@@
 
 ppgc = 540  # Points per great circle (sets longitudinal resolution for plots)
 
 verbose = True
-use_latex = False  # Whether to use Latex in rendering plot text
-relative = True  # Whether to use relative (epsilon/R*chi_pq) or absolute (direct spherical harmonic coefficients) formulation for reading Ypq. Affects which files are needed/read to interpret the asymmetric interior structure.
+use_latex = True  # Whether to use Latex in rendering plot text
+relative = False  # Whether to use relative (epsilon/R*chi_pq) or absolute (direct spherical harmonic coefficients) formulation for reading Ypq. Affects which files are needed/read to interpret the asymmetric interior structure.
 synodic_period_only = False  # Whether to consider only the synodic period for induction
 orbital_time_series = False  # Whether to plot a time series that considers only the orbital period
-sub_planet_vert = True  # Whether to plot a vertical cut at the sub-planetary point (or nearby) for a snapshot in time
+sub_planet_vert = False  # Whether to plot a vertical cut at the sub-planetary point (or nearby) for a snapshot in time
 plot_diffs = True  # Whether to plot magnetic fields as differences arising due to asymmetry
 gif_diff = True  # Whether to plot differences in animation frames or the absolute component
 
 nprm_max_main = 1  # Highest degree in excitation field to use
-eval_radius = 2.0  # Distance (in units of body radii) from body center to use for evaluating B. Overridden for Europa and Enceladus.
+eval_radius = 2  # Distance (in units of body radii) from body center to use for evaluating B. Overridden for Europa and Enceladus.
 
 debug = False  # Special use debug flag
 convert_depth_to_chipq = True  # Prints a file named interior/chi_pq_bodyname.txt for copying over relative harmonic coefficients to degree<p>_shapes_bodyname.txt files. Only used if relative = False.
 output_Schmidt = False  # Record induced moment coefficients in Schmidt semi-normalized form in addition to fully normalized moments. Also reads in and plots fields using this normalization.
 
 # @@@@@@@@@@@@@@@@@@@@@@@@
 #   Calculation settings
 # @@@@@@@@@@@@@@@@@@@@@@@@
 
 do_parallel = True  # Whether to run certain calculations in parallel. Setting to False makes debugging much more straightforward.
 digits_precision = 750  # Number of digits of precision for use in calculations involving Bessel functions. Calculations involve small differences between large numbers when conductivities are very large or very small.
                         # If you encounter divide-by-zero errors, try increasing this number.
 
-eval_datetime = "2000-01-01T11:58:55.816"  # UTC datetime string for the time to evaluate the induced fields (and start animations from) in yyyy-mm-ddThh:mm:mm:ss.sss format
+default_eval_datetime = "2000-01-01T11:58:55.816"  # UTC datetime string for the time to evaluate the induced fields (and start animations from) in yyyy-mm-ddThh:mm:mm:ss.sss format
 
 # The following are only used if synodic_period_only is True:
 loclat = 0  # degrees latitude (IAU) for plotting a time series
 loclon = 0  # degrees longitude (IAU) for plotting a time series
 localt = 0  # km altitude for plotting a time series
 
+# Model option strings
+prevEuropa = 'prev'
+TobieHigh = 'Tobie_high'
+TobieLow = 'Tobie_low'
+CochraneBestFit = 'Cochrane_best'
+CochraneLikely = 'Cochrane_likely'
+DO_LARGE = 'large'
+DO_GIF = 'do_gif'
+
 # @@@@@@@@@@@@@@@@@@@
 #   Plotting params
 # @@@@@@@@@@@@@@@@@@@
 
 t_pts = 200  # Number of points in 1-period time series (or spatial points in vertical cut)
 n_frames = 100  # Number of animation frames to use, spaced evenly throughout one period of oscillation
 vert_start = 1.0  # Units of body radii to start vertical cut
@@ -58,24 +67,31 @@
 vert_cut_lon = 0
 
 # Color and style options
 c = [ "green", "black", "blue" ]
 vc = "brown"
 style1 = "solid"
 style2 = "dashed"
+cMark = "xkcd:grass green"
+cMarkE = "xkcd:forest green"
+szMark = 20
+stMark = 'o'
 
 # Figure formatting defaults
 deft_figsize = (8,4)
 lat_min = -90
 lat_max = 90
 do_360 = False  # Whether to plot from 0 to 360 (True) or from -180 to 180 (False).
 no_title_text = False
 save_vector = False  # Toggle for saving additional vector graphics (pdf)
 pub_override = True  # Use fixed colorbar scale for both Europa models
 clabel_pad = 5  # Whitespace to add adjacent to contour labels
+fig_dpi = 200  # Default dpi to use for raster images when not passed as argument
+fmt = 'pdf'  # Default figure format to use (file extension)
+animFmt = 'png'  # Figure format to force for animations (PDFs can't be easily made into animation frames)
 
 # Colorbar and tick formatting
 cbar_pos = [0.90, 0.18, 0.02, 0.6]
 cbar_adj = 5
 deft_tsize = 16
 deft_ticksize = 14
 
@@ -94,7 +110,12 @@
 printFmt = '[%(levelname)s] %(message)s'
 stream = logging.StreamHandler()
 stream.setFormatter(logging.Formatter(printFmt))
 log.setLevel(logLevel)
 log.addHandler(stream)
 logging.getLogger('matplotlib').setLevel(logging.WARNING)
 logging.getLogger('PIL').setLevel(logging.WARNING)
+
+if use_latex and not shutil.which('latex'):
+    log.warning('A LaTeX installation was not found. LaTeX will not be used for plot labels.')
+    use_latex = False
+
```

### Comparing `MoonMag-1.5.2/src/MoonMag/eval_induced_field.py` & `MoonMag-1.5.3/MoonMag/eval_induced_field.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,17 +19,30 @@
 
 from MoonMag import _excitation
 from MoonMag.config import *
 import MoonMag.symmetry_funcs as sym
 import MoonMag.asymmetry_funcs as asym
 import MoonMag.plotting_funcs as plots
 
-def run_calcs(bname, comp, recalc, plot_field, plot_asym, synodic_only=True,
-              do_large=False, seawater=True, compare_me=False, surface=False, do_gif=False,
-              inp_path=None, inp_Bi_path=None):
+def run_calcs(bname, comp, recalc, plot_field, plot_asym, synodic_only=False,
+              inp_path=None, inp_Bi_path=None, eval_r=None,
+              timePair=None, CAmarks=None, modelOpts=None):
+
+    if eval_r is None:
+        eval_r = eval_radius
+
+    if timePair is not None:
+        eval_datetime = timePair[1]
+    else:
+        eval_datetime = default_eval_datetime
+
+    if modelOpts is None:
+        modelOpts = []
+
+    flyby_opt = ""  # Label for flyby-specific models
 
     absolute = (comp==None)   # Whether to plot the symmetric and asymmetric absolute magnitudes in addition to the desired component
     if comp is None:
         compstr = "_mag"
     else:
         compstr = f"_{comp}"
 
@@ -42,62 +55,61 @@
     # IO file paths
     if inp_path is None:
         inp_path = os.path.join("MoonMag", "interior")
     if inp_Bi_path is None:
         inp_Bi_path = os.path.join("MoonMag", "induced")
 
     # p_max is highest degree in boundary shapes to use
-    # bname_opt and sw_opt are strings to append to filenames to identify special cases
-    sw_opt = ""
+    # bname_opt is a string to append to filenames to identify special cases
+    bname_opt = ""
+    p_max_main = 2
+    Benm_model = None
     if bname == "Enceladus":
         p_max_main = 8
-        bname_opt = ""
-        eval_r = 1.1 # About 25 km altitude
+        eval_r = 1.1  # About 25 km altitude
     elif bname == "Miranda":
         p_max_main = 8
-        if surface:
-            bname_opt = "_surface"
-            eval_r = 1.0
-        else:
-            bname_opt = ""
-            eval_r = eval_radius
     elif bname == "Europa":
-        if compare_me:
+        if prevEuropa in modelOpts:
             p_max_main = 2
-            bname_opt = "_prev"
+            bname_opt = '_prev'
             eval_r = 1.0
-        else:
+            synodic_only = True
+        elif TobieHigh in modelOpts or TobieLow in modelOpts:
             p_max_main = 4
-            bname_opt = "_Tobie"
-            if seawater:
-                sw_opt = "_high"
+            if TobieHigh in modelOpts:
+                bname_opt = '_Tobie_high'
             else:
-                sw_opt = "_low"
-            eval_r = 1.016 # 25 km altitude, the planned CA for some Clipper flybys
-    else:
+                bname_opt = '_Tobie_low'
+            eval_r = 1.016  # 25 km altitude, the planned CA for some Clipper flybys
+    elif bname == "Callisto":
         p_max_main = 2
-        bname_opt = ""
-        eval_r = eval_radius
+        if CochraneBestFit in modelOpts or CochraneLikely in modelOpts:
+            Benm_model = 'Cochrane'
+            if timePair is not None:
+                flyby_opt = timePair[0]
+            if CochraneBestFit in modelOpts:
+                bname_opt = '_inverted'
+            else:
+                bname_opt = '_likely'
 
-    # Override synodic_only setting in the case of previous work comparison
-    if bname == "Europa" and compare_me:
-        synodic_only = True
+    if 'surface' in modelOpts:
+        eval_r = 1.0
 
     # Highest degree of induced moments
     n_max_main = nprm_max_main + p_max_main
 
     # Set time to evaluate magnetic fields
     spiceTLS = 'naif0012.tls'
     spice.furnsh(os.path.join(_excitation, spiceTLS))
 
     #tsec = spice.str2et(dtime.now().isoformat())  # Evaluate as the bodies are right NOW
     #tsec = 0  # Evaluate AT J2000
     tsec = spice.str2et(eval_datetime)
 
-
     # Linear arrays of values to loop over for nprm,mprm,p,q,n,m
     nprmvals = [ nprm for nprm in range(1,nprm_max_main+1) for _    in range(-nprm,nprm+1) ]
     mprmvals = [ mprm for nprm in range(1,nprm_max_main+1) for mprm in range(-nprm,nprm+1) ]
     pvals = [ p for p in range(1,p_max_main+1) for _ in range(-p,p+1) ]
     qvals = [ q for p in range(1,p_max_main+1) for q in range(-p,p+1) ]
     nvals = [ n for n in range(1,n_max_main+1) for _ in range(-n,n+1) ]
     mvals = [ m for n in range(1,n_max_main+1) for m in range(-n,n+1) ]
@@ -121,27 +133,30 @@
         r_io = -1
     elif bname == "Enceladus":
         rscale_moments = 1/252.1/1e3
         rscale_asym = 1/230035.1
         r_io = -2
     elif bname == "Europa":
         r_io = -2
-        if compare_me:
+        if prevEuropa in modelOpts:
             rscale_moments = 1/1560.0/1e3
             rscale_asym = 1/1537500
         else:
             rscale_moments = 1/1561.0/1e3
-            if seawater:
-                rscale_asym = 1/1538503.78421254
+            if TobieHigh in modelOpts or TobieLow in modelOpts:
+                if TobieHigh in modelOpts:
+                    rscale_asym = 1/1538503.78421254
+                else:
+                    rscale_asym = 1/1538489.72081887
             else:
-                rscale_asym = 1/1538489.72081887
+                rscale_asym = 1/(1561 - 30)/1e3
     elif bname == "Miranda":
         rscale_moments = 1/235.8/1e3
         rscale_asym = 1/185989.764241229
-        if bname_opt == "_surface":
+        if "surface" in modelOpts:
             r_io = -2
         else:
             r_io = -3
     elif bname == "Triton":
         rscale_moments = 1/1353.4/1e3
         rscale_asym = 1/1803400
         r_io = -1
@@ -153,33 +168,33 @@
         Xid = asym.get_all_Xid(nprm_max_main, p_max_main, n_max_main, nvals, mvals)
         log.debug("#######   Xid values   #######")
         asym.print_Xid_table(Xid, nprm_max_main, p_max_main, n_max_main)
         log.debug(f"\n#######   Xi values   #######")
         asym.print_Xi_table(nprm_max_main, p_max_main, n_max_main)
 
     if recalc:
-        int_model = os.path.join(inp_path, f"interior_model_asym{bfname}{bname_opt}{sw_opt}.txt")
+        int_model = os.path.join(inp_path, f"interior_model_asym{bfname}{bname_opt}.txt")
         log.debug(f"Using interior model: {int_model}")
 
         r_bds, sigmas, bcdev = np.loadtxt(int_model, skiprows=1, unpack=True, delimiter=',')
         n_bds = np.size(r_bds)
 
         # Read in asymmetric shape information
         eps_scaled = r_bds * bcdev
         if relative:
             single_asym = None
         else:
             single_asym = r_io
         asym_shape, grav_shape = asym.read_shape(n_bds, p_max_main, rscale_asym, bodyname=bname, relative=relative, single_asym=single_asym,
-                                     eps_scaled=eps_scaled, r_bds=r_bds, r_io=r_io, append=bname_opt, convert_depth_to_chipq=convert_depth_to_chipq)
+                                     eps_scaled=eps_scaled, r_bds=r_bds, r_io=r_io, append=bname_opt+flyby_opt, convert_depth_to_chipq=convert_depth_to_chipq)
         r_bds, sigmas, asym_shape = asym.validate(r_bds, sigmas, bcdev, asym_shape, p_max_main)
 
         # Read in Benm info
         if plot_field:
-            peak_periods, Benm, B0 = asym.read_Benm(nprm_max_main, p_max_main, bodyname=bname, synodic=synodic_only, orbital=False)
+            peak_periods, Benm, B0 = asym.read_Benm(nprm_max_main, p_max_main, bodyname=bname, synodic=synodic_only, orbital=False, model=Benm_model)
             peak_omegas = 2*np.pi/(peak_periods*3600)
             if not isinstance(peak_omegas, Iterable):
                 peak_periods = [peak_periods]
                 peak_omegas = [peak_omegas]
             n_peaks = len(peak_omegas)
 
     else:
@@ -225,25 +240,27 @@
     if plot_asym:
         if bname == "Triton" or bname == "Callisto":
             R_surface = -2
             r_io = -1
             descrip = "Ionosphere"
         else:
             R_surface = r_io + 1
-            if do_large:
+            if DO_LARGE in modelOpts:
                 descrip = "Ice shell"
             else:
                 descrip = "Ice--ocean"
-        plots.plotAsym(recalc, do_large, index=r_io, cmp_index=R_surface, r_bds=r_bds, asym_shape=asym_shape, pvals=pvals, qvals=qvals, bodyname=bname, append=bname_opt+sw_opt, descrip=descrip, no_title=no_title_text)
+        plots.plotAsym(recalc, DO_LARGE in modelOpts, index=r_io, cmp_index=R_surface, r_bds=r_bds,
+                       asym_shape=asym_shape, pvals=pvals, qvals=qvals, bodyname=bname,
+                       append=bname_opt+flyby_opt, descrip=descrip, no_title=no_title_text)
 
     if plot_field:
         if recalc:
             # Calculate and print to data files
-            Binm_sph = sym.BiList(r_bds, sigmas, peak_omegas, Benm, nprmvals, mprmvals, rscale_moments, n_max=nprm_max_main, bodyname=bname, append=bname_opt+sw_opt, Schmidt=output_Schmidt)
-            Binm = asym.BiList(r_bds, sigmas, peak_omegas, asym_shape, grav_shape, Benm, rscale_moments, nvals, mvals, p_max_main, nprm_max=nprm_max_main, bodyname=bname, append=bname_opt+sw_opt, Schmidt=output_Schmidt)
+            Binm_sph = sym.BiList(r_bds, sigmas, peak_omegas, Benm, nprmvals, mprmvals, rscale_moments, n_max=nprm_max_main, bodyname=bname, append=bname_opt+flyby_opt, Schmidt=output_Schmidt)
+            Binm = asym.BiList(r_bds, sigmas, peak_omegas, asym_shape, grav_shape, Benm, rscale_moments, nvals, mvals, p_max_main, nprm_max=nprm_max_main, bodyname=bname, append=bname_opt+flyby_opt, Schmidt=output_Schmidt)
             n_peaks = len(peak_omegas)
             if output_Schmidt:
                 nprmvals = [nprm for nprm in range(1, nprm_max_main + 1) for _ in range(0, nprm + 1)]
                 mprmvals = [mprm for nprm in range(1, nprm_max_main + 1) for mprm in range(0, nprm + 1)]
                 nvals = [n for n in range(1, n_max_main + 1) for _ in range(0, n + 1)]
                 mvals = [m for n in range(1, n_max_main + 1) for m in range(0, n + 1)]
                 gnm, hnm = ( np.zeros((n_peaks,n_max_main+1,n_max_main+1), dtype=np.complex_) for _ in range(2) )
@@ -254,25 +271,25 @@
         else:
             if output_Schmidt:
                 nprmvals = [nprm for nprm in range(1, nprm_max_main + 1) for _ in range(0, nprm + 1)]
                 mprmvals = [mprm for nprm in range(1, nprm_max_main + 1) for mprm in range(0, nprm + 1)]
                 nvals = [n for n in range(1, n_max_main + 1) for _ in range(0, n + 1)]
                 mvals = [m for n in range(1, n_max_main + 1) for m in range(0, n + 1)]
                 T_hrs, n_asy, m_asy, lin_gnm_Re, lin_gnm_Im, lin_hnm_Re, lin_hnm_Im = np.loadtxt(
-                    os.path.join(inp_Bi_path, f"{bin_name}ghnm_asym{bname_opt}{sw_opt}.dat"),
+                    os.path.join(inp_Bi_path, f"{bin_name}ghnm_asym{bname_opt}{flyby_opt}.dat"),
                     skiprows=1, unpack=True, delimiter=',')
                 T_hrs_sym, n_sph, m_sph, lin_gnm_sph_Re, lin_gnm_sph_Im, lin_hnm_sph_Re, lin_hnm_sph_Im = np.loadtxt(
-                    os.path.join(inp_Bi_path, f"{bin_name}ghnm_sym{bname_opt}{sw_opt}.dat"),
+                    os.path.join(inp_Bi_path, f"{bin_name}ghnm_sym{bname_opt}{flyby_opt}.dat"),
                     skiprows=1, unpack=True, delimiter=',')
             else:
                 T_hrs, n_asy, m_asy, lin_Binm_Re, lin_Binm_Im = np.loadtxt(
-                    os.path.join(inp_Bi_path, f"{bin_name}Binm_asym{bname_opt}{sw_opt}.dat"),
+                    os.path.join(inp_Bi_path, f"{bin_name}Binm_asym{bname_opt}{flyby_opt}.dat"),
                     skiprows=1, unpack=True, delimiter=',')
                 T_hrs_sym, n_sph, m_sph, lin_Binm_sph_Re, lin_Binm_sph_Im = np.loadtxt(
-                    os.path.join(inp_Bi_path, f"{bin_name}Binm_sym{bname_opt}{sw_opt}.dat"),
+                    os.path.join(inp_Bi_path, f"{bin_name}Binm_sym{bname_opt}{flyby_opt}.dat"),
                     skiprows=1, unpack=True, delimiter=',')
 
             peak_periods = np.unique(T_hrs)
             peak_omegas = 2*np.pi/(peak_periods*3600)
             n_peaks = len(peak_omegas)
             Nnm_asy = int(len(n_asy)/n_peaks)
             peak_periods_sym = np.unique(T_hrs_sym)
@@ -311,15 +328,15 @@
             gnm_rot = gnm * 1.0
             hnm_sph_rot = hnm_sph * 1.0
             hnm_rot = hnm * 1.0
         else:
             Binm_sph_rot = Binm_sph * 1.0
             Binm_rot = Binm * 1.0
 
-        if do_gif:
+        if DO_GIF in modelOpts:
             log.debug(f"Making {n_frames} animation frames.")
             for iT in range(n_frames):
                 iT_str = f"{iT:04}"
                 t_hr = peak_periods[-1] * iT / n_frames
                 tstr = f"{round(t_hr, 1):03}"
                 tframe = tsec + t_hr*3600
                 for i_om in range(n_peaks):
@@ -331,17 +348,18 @@
                     else:
                         Binm_sph_rot[i_om,...] = Binm_sph[i_om,...] * np.exp(-1j * peak_omegas[i_om] * tframe)
                         Binm_rot[i_om,...]     = Binm[i_om,...]     * np.exp(-1j * peak_omegas[i_om] * tframe)
 
                 if output_Schmidt:
                     Binm_rot = (gnm_rot, hnm_rot)
                     Binm_sph_rot = (gnm_sph_rot, hnm_sph_rot)
-                plots.plotMagSurf(n_peaks, Binm_rot, nvals, mvals, do_large, Schmidt=output_Schmidt, r_surf_mean=eval_r, asym_frac=asym_frac,
+                plots.plotMagSurf(n_peaks, Binm_rot, nvals, mvals, DO_LARGE in modelOpts, Schmidt=output_Schmidt, r_surf_mean=eval_r, asym_frac=asym_frac,
                                   pvals=pvals, qvals=qvals, difference=gif_diff, Binm_sph=Binm_sph_rot, nprmvals=nprmvals, mprmvals=mprmvals,
-                                  bodyname=bname, append=bname_opt+sw_opt, fend=iT_str, tstr=tstr, component=comp, absolute=True, no_title=False)
+                                  bodyname=bname, append=bname_opt+flyby_opt, fend=iT_str, tstr=tstr, component=comp,
+                                  absolute=True, no_title=False, marks=CAmarks)
 
             log.info("Animation frames printed to figures/anim_frames/ folder.\n" +
                      "Stack them into a gif with, e.g.:\n" +
                      "convert -delay 15 figures/anim_frames/Miranda_field_asym0*.png -loop 15 figures/anim_Miranda_asym.gif")
         else:
             for i_om in range(n_peaks):
                 if output_Schmidt:
@@ -353,69 +371,71 @@
                     Binm_sph_rot[i_om,...] = Binm_sph[i_om,...] * np.exp(-1j * peak_omegas[i_om] * tsec)
                     Binm_rot[i_om,...]     = Binm[i_om,...]     * np.exp(-1j * peak_omegas[i_om] * tsec)
 
             # Plot symmetric moments/difference
             if output_Schmidt:
                 Binm_rot = (gnm_rot, hnm_rot)
                 Binm_sph_rot = (gnm_sph_rot, hnm_sph_rot)
-            plots.plotMagSurf(n_peaks, Binm_rot, nvals, mvals, do_large, Schmidt=output_Schmidt, r_surf_mean=eval_r, asym_frac=asym_frac,
+            plots.plotMagSurf(n_peaks, Binm_rot, nvals, mvals, DO_LARGE in modelOpts, Schmidt=output_Schmidt, r_surf_mean=eval_r, asym_frac=asym_frac,
                             pvals=pvals, qvals=qvals, difference=plot_diffs, Binm_sph=Binm_sph_rot, nprmvals=nprmvals, mprmvals=mprmvals,
-                            bodyname=bname, append=bname_opt+sw_opt, component=comp, absolute=absolute, no_title=no_title_text)
+                            bodyname=bname, append=bname_opt+flyby_opt, component=comp, absolute=absolute, no_title=no_title_text,
+                            marks=CAmarks)
 
         # Restrict plotting of certain diagnostic plots so we don't get spammed when we only want to do this for special conditions
-        actually_plot_traces = bname == "Europa" and (compare_me or seawater) and comp == "x"
+        actually_plot_traces = bname == "Europa" and comp == "x" \
+                               and (prevEuropa in modelOpts or TobieLow in modelOpts or TobieHigh in modelOpts)
         if (sub_planet_vert and actually_plot_traces) and not output_Schmidt:
             if not recalc:
-                peak_periods, Benm, B0 = asym.read_Benm(nprm_max_main, p_max_main, bodyname=bname, synodic=synodic_only)
-                int_model = os.path.join(inp_path, f"interior_model_asym{bfname}{bname_opt}{sw_opt}.txt")
+                peak_periods, Benm, B0 = asym.read_Benm(nprm_max_main, p_max_main, bodyname=bname, synodic=synodic_only, model=Benm_model)
+                int_model = os.path.join(inp_path, f"interior_model_asym{bfname}{bname_opt}{flyby_opt}.txt")
                 r_bds, sigmas, bcdev = np.loadtxt(int_model, skiprows=1, unpack=True, delimiter=',')
 
             t_cut = vert_cut_hr * 3600
             vert_begin = np.maximum(vert_start, r_bds[-1]*rscale_moments)
             r = np.linspace(vert_begin, vert_stop, t_pts)
             x = r * np.cos(np.radians(vert_cut_lat)) * np.cos(np.radians(vert_cut_lon))
             y = r * np.cos(np.radians(vert_cut_lat)) * np.sin(np.radians(vert_cut_lon))
             z = r * np.sin(np.radians(vert_cut_lat))
             t = np.zeros(t_pts)
             t += t_cut
             plots.calcAndPlotTrajec(x,y,z,r,t, Binm, Benm, peak_omegas, nprm_max_main, n_max_main, nvals, mvals, 
                                     R_body=R, component=comp, difference=True, Binm_sph=Binm_sph, bodyname=bname, 
-                                    append=bname_opt+sw_opt+compstr)
+                                    append=bname_opt+flyby_opt+compstr)
 
         # Plot a time series at the sub-parent-planet point--(0 deg, 0 deg) in IAU coordinates.
         # Only tested for Europa, with no ionosphere.
         if (synodic_only and actually_plot_traces) and not output_Schmidt:
             if not recalc:
                 synodic_period, Benm, B0 = asym.read_Benm(nprm_max_main, p_max_main, bodyname=bname, synodic=True)
                 peak_periods = [synodic_period]
             if not sub_planet_vert:
-                int_model = os.path.join(inp_path, f"interior_model_asym{bfname}{bname_opt}{sw_opt}.txt")
+                int_model = os.path.join(inp_path, f"interior_model_asym{bfname}{bname_opt}{flyby_opt}.txt")
                 r_bds, sigmas, bcdev = np.loadtxt(int_model, skiprows=1, unpack=True, delimiter=',')
 
             r = (localt + R) / R
 
             # Only valid if the evaluation point is outside the conducting region, so that B is subject to the Laplace equation.
             if r*R*1e3/r_bds[-1] >= 0.999:
                 locx = r * np.cos(np.radians(loclat)) * np.cos(np.radians(loclon))
                 locy = r * np.cos(np.radians(loclat)) * np.sin(np.radians(loclon))
                 locz = r * np.sin(np.radians(loclat))
                 loc = [ locx, locy, locz, r ] # Now IAU planetocentric in terms of body radii
                 plots.plotTimeSeries(loc, Binm[0,...], Benm[0,...], tsec, peak_periods[0], nprm_max_main, n_max_main, nvals, mvals,
-                                     n_pts=t_pts, component=comp, Binm_sph=Binm_sph[0,...], bodyname=bname, append=bname_opt+sw_opt+compstr)
+                                     n_pts=t_pts, component=comp, Binm_sph=Binm_sph[0,...], bodyname=bname, append=bname_opt+flyby_opt+compstr)
 
                 if orbital_time_series:
                     if not recalc:
                         n_bds = np.size(r_bds)
                         eps_scaled = r_bds * bcdev
                         if relative:
                             single_asym = None
                         else:
                             single_asym = r_io
                         asym_shape, grav_shape = asym.read_shape(n_bds, p_max_main, rscale_asym, bodyname=bname, relative=relative, single_asym=single_asym,
-                                                     eps_scaled=eps_scaled, r_bds=r_bds, r_io=r_io, append=bname_opt, convert_depth_to_chipq=convert_depth_to_chipq)
+                                                     eps_scaled=eps_scaled, r_bds=r_bds, r_io=r_io, append=bname_opt+flyby_opt, convert_depth_to_chipq=convert_depth_to_chipq)
                         r_bds, sigmas, asym_shape = asym.validate(r_bds, sigmas, bcdev, asym_shape, p_max_main)
 
                     orbital_period, Benm_orbital, B0 = asym.read_Benm(nprm_max_main, p_max_main, bodyname=bname, orbital=True)
                     orbital_omega = 2*np.pi/(orbital_period*3600)
-                    Binm_sph_orbital = sym.BiList(r_bds, sigmas, [orbital_omega], Benm_orbital, nprmvals, mprmvals, rscale_moments, n_max=nprm_max_main, bodyname=bname, append=bname_opt + sw_opt)
-                    Binm_orbital = asym.BiList(r_bds, sigmas, [orbital_omega], asym_shape, grav_shape, Benm_orbital, rscale_moments, nvals, mvals, p_max_main, nprm_max=nprm_max_main, bodyname=bname, append=bname_opt + sw_opt)
-                    plots.plotTimeSeries(loc, Binm_orbital[0, ...], Benm_orbital[0, ...], tsec, orbital_period, nprm_max_main, n_max_main, nvals, mvals, n_pts=t_pts, component=comp, Binm_sph=Binm_sph_orbital[0, ...], bodyname=bname, append=bname_opt+sw_opt+compstr+"_orbital")
+                    Binm_sph_orbital = sym.BiList(r_bds, sigmas, [orbital_omega], Benm_orbital, nprmvals, mprmvals, rscale_moments, n_max=nprm_max_main, bodyname=bname, append=bname_opt+flyby_opt)
+                    Binm_orbital = asym.BiList(r_bds, sigmas, [orbital_omega], asym_shape, grav_shape, Benm_orbital, rscale_moments, nvals, mvals, p_max_main, nprm_max=nprm_max_main, bodyname=bname, append=bname_opt+flyby_opt)
+                    plots.plotTimeSeries(loc, Binm_orbital[0, ...], Benm_orbital[0, ...], tsec, orbital_period, nprm_max_main, n_max_main, nvals, mvals, n_pts=t_pts, component=comp, Binm_sph=Binm_sph_orbital[0, ...], bodyname=bname, append=bname_opt+flyby_opt+compstr+"_orbital")
```

### Comparing `MoonMag-1.5.2/src/MoonMag/excitation/Be1xyz.txt` & `MoonMag-1.5.3/MoonMag/excitation/Be1xyz.txt`

 * *Files identical despite different names*

### Comparing `MoonMag-1.5.2/src/MoonMag/excitation/Be1xyz_Callisto.txt` & `MoonMag-1.5.3/MoonMag/excitation/Be1xyz_Callisto.txt`

 * *Files identical despite different names*

### Comparing `MoonMag-1.5.2/src/MoonMag/excitation/Be1xyz_Europa.txt` & `MoonMag-1.5.3/MoonMag/excitation/Be1xyz_Europa.txt`

 * *Files identical despite different names*

### Comparing `MoonMag-1.5.2/src/MoonMag/excitation/Be1xyz_Miranda.txt` & `MoonMag-1.5.3/MoonMag/excitation/Be1xyz_Miranda.txt`

 * *Files identical despite different names*

### Comparing `MoonMag-1.5.2/src/MoonMag/excitation/Be2xyz.txt` & `MoonMag-1.5.3/MoonMag/excitation/Be2xyz.txt`

 * *Files identical despite different names*

### Comparing `MoonMag-1.5.2/src/MoonMag/field_xyz.py` & `MoonMag-1.5.3/MoonMag/field_xyz.py`

 * *Files identical despite different names*

### Comparing `MoonMag-1.5.2/src/MoonMag/induced/Xid_values_n1_p10_np11.mat` & `MoonMag-1.5.3/MoonMag/induced/Xid_values_n1_p10_np11.mat`

 * *Files identical despite different names*

### Comparing `MoonMag-1.5.2/src/MoonMag/induced/Xid_values_n1_p2_np3.mat` & `MoonMag-1.5.3/MoonMag/induced/Xid_values_n1_p2_np3.mat`

 * *Files identical despite different names*

### Comparing `MoonMag-1.5.2/src/MoonMag/induced/Xid_values_n1_p4_np5.mat` & `MoonMag-1.5.3/MoonMag/induced/Xid_values_n1_p4_np5.mat`

 * *Files identical despite different names*

### Comparing `MoonMag-1.5.2/src/MoonMag/induced/Xid_values_n1_p8_np9.mat` & `MoonMag-1.5.3/MoonMag/induced/Xid_values_n1_p8_np9.mat`

 * *Files identical despite different names*

### Comparing `MoonMag-1.5.2/src/MoonMag/interior/degree1_shapes.txt` & `MoonMag-1.5.3/MoonMag/interior/degree1_shapes.txt`

 * *Files identical despite different names*

### Comparing `MoonMag-1.5.2/src/MoonMag/interior/degree1_shapes_Miranda.txt` & `MoonMag-1.5.3/MoonMag/interior/degree1_shapes_Miranda.txt`

 * *Files identical despite different names*

### Comparing `MoonMag-1.5.2/src/MoonMag/interior/degree2_shapes.txt` & `MoonMag-1.5.3/MoonMag/interior/degree2_shapes.txt`

 * *Files identical despite different names*

### Comparing `MoonMag-1.5.2/src/MoonMag/interior/degree2_shapes_Europa_Tobie.txt` & `MoonMag-1.5.3/MoonMag/interior/degree2_shapes_Europa_Tobie.txt`

 * *Files identical despite different names*

### Comparing `MoonMag-1.5.2/src/MoonMag/interior/degree2_shapes_Miranda.txt` & `MoonMag-1.5.3/MoonMag/interior/degree2_shapes_Miranda.txt`

 * *Files identical despite different names*

### Comparing `MoonMag-1.5.2/src/MoonMag/interior/degree3_shapes.txt` & `MoonMag-1.5.3/MoonMag/interior/degree3_shapes.txt`

 * *Files identical despite different names*

### Comparing `MoonMag-1.5.2/src/MoonMag/interior/degree3_shapes_Miranda.txt` & `MoonMag-1.5.3/MoonMag/interior/degree3_shapes_Miranda.txt`

 * *Files identical despite different names*

### Comparing `MoonMag-1.5.2/src/MoonMag/interior/degree4_shapes.txt` & `MoonMag-1.5.3/MoonMag/interior/degree4_shapes.txt`

 * *Files identical despite different names*

### Comparing `MoonMag-1.5.2/src/MoonMag/interior/degree4_shapes_Europa_Tobie.txt` & `MoonMag-1.5.3/MoonMag/interior/degree4_shapes_Europa_Tobie.txt`

 * *Files identical despite different names*

### Comparing `MoonMag-1.5.2/src/MoonMag/interior/degree4_shapes_Miranda.txt` & `MoonMag-1.5.3/MoonMag/interior/degree4_shapes_Miranda.txt`

 * *Files identical despite different names*

### Comparing `MoonMag-1.5.2/src/MoonMag/interior/degree5_shapes.txt` & `MoonMag-1.5.3/MoonMag/interior/degree5_shapes.txt`

 * *Files identical despite different names*

### Comparing `MoonMag-1.5.2/src/MoonMag/interior/degree5_shapes_Miranda.txt` & `MoonMag-1.5.3/MoonMag/interior/degree5_shapes_Miranda.txt`

 * *Files identical despite different names*

### Comparing `MoonMag-1.5.2/src/MoonMag/interior/degree6_shapes.txt` & `MoonMag-1.5.3/MoonMag/interior/degree6_shapes.txt`

 * *Files identical despite different names*

### Comparing `MoonMag-1.5.2/src/MoonMag/interior/degree6_shapes_Miranda.txt` & `MoonMag-1.5.3/MoonMag/interior/degree6_shapes_Miranda.txt`

 * *Files identical despite different names*

### Comparing `MoonMag-1.5.2/src/MoonMag/interior/degree7_shapes.txt` & `MoonMag-1.5.3/MoonMag/interior/degree7_shapes.txt`

 * *Files identical despite different names*

### Comparing `MoonMag-1.5.2/src/MoonMag/interior/degree7_shapes_Miranda.txt` & `MoonMag-1.5.3/MoonMag/interior/degree7_shapes_Miranda.txt`

 * *Files identical despite different names*

### Comparing `MoonMag-1.5.2/src/MoonMag/interior/degree8_shapes.txt` & `MoonMag-1.5.3/MoonMag/interior/degree8_shapes.txt`

 * *Files identical despite different names*

### Comparing `MoonMag-1.5.2/src/MoonMag/interior/degree8_shapes_Miranda.txt` & `MoonMag-1.5.3/MoonMag/interior/degree8_shapes_Miranda.txt`

 * *Files identical despite different names*

### Comparing `MoonMag-1.5.2/src/MoonMag/interior/depth_chi_pq_shape_Callisto.txt` & `MoonMag-1.5.3/MoonMag/interior/depth_chi_pq_shape_Callisto.txt`

 * *Files identical despite different names*

### Comparing `MoonMag-1.5.2/src/MoonMag/interior/depth_chi_pq_shape_Enceladus.txt` & `MoonMag-1.5.3/MoonMag/interior/depth_chi_pq_shape_Enceladus.txt`

 * *Files identical despite different names*

### Comparing `MoonMag-1.5.2/src/MoonMag/interior/depth_chi_pq_shape_Europa.txt` & `MoonMag-1.5.3/MoonMag/interior/depth_chi_pq_shape_Europa.txt`

 * *Files identical despite different names*

### Comparing `MoonMag-1.5.2/src/MoonMag/interior/depth_chi_pq_shape_Europa_Tobie.txt` & `MoonMag-1.5.3/MoonMag/interior/depth_chi_pq_shape_Europa_Tobie_high.txt`

 * *Files identical despite different names*

### Comparing `MoonMag-1.5.2/src/MoonMag/interior/depth_chi_pq_shape_Miranda.txt` & `MoonMag-1.5.3/MoonMag/interior/depth_chi_pq_shape_Miranda.txt`

 * *Files identical despite different names*

### Comparing `MoonMag-1.5.2/src/MoonMag/interior/depth_chi_pq_shape_Triton.txt` & `MoonMag-1.5.3/MoonMag/interior/depth_chi_pq_shape_Triton.txt`

 * *Files identical despite different names*

### Comparing `MoonMag-1.5.2/src/MoonMag/interior/gravity_Europa_Tobie.txt` & `MoonMag-1.5.3/MoonMag/interior/gravity_Europa_Tobie_high.txt`

 * *Files identical despite different names*

### Comparing `MoonMag-1.5.2/src/MoonMag/interior/interior_model_asym.txt` & `MoonMag-1.5.3/MoonMag/interior/interior_model_asym.txt`

 * *Files identical despite different names*

### Comparing `MoonMag-1.5.2/src/MoonMag/plot_Aes.py` & `MoonMag-1.5.3/MoonMag/plot_Aes.py`

 * *Files identical despite different names*

### Comparing `MoonMag-1.5.2/src/MoonMag/plotting_funcs.py` & `MoonMag-1.5.3/MoonMag/plotting_funcs.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,30 +46,30 @@
         n_latticks = 5
         n_lonticks = 5
         lg_end = "_small"
     else:
         n_latticks = 7
         n_lonticks = 9
         lg_end = ""
-    latticks = np.linspace(lat_min, lat_max, n_latticks, endpoint=True, dtype=np.int)
+    latticks = np.linspace(lat_min, lat_max, n_latticks, endpoint=True, dtype=np.int_)
 
     # Generate lat/lon formatters
     if do_360:
         phi = phi_std
         lon = elon
 
         lon_formatter = tick.FuncFormatter(lambda v, pos: east_formatted(v, EAST=True))
         lon_min = 0
         lon_max = 360
-        lonticks = np.linspace(lon_min, lon_max, n_lonticks, dtype=np.int)
+        lonticks = np.linspace(lon_min, lon_max, n_lonticks, dtype=np.int_)
     else:
         lon_formatter = tick.FuncFormatter(lambda v, pos: east_formatted(v, EAST=False))
         lon_min = -180
         lon_max = 180
-        lonticks = np.linspace(lon_min, lon_max, n_lonticks, dtype=np.int)
+        lonticks = np.linspace(lon_min, lon_max, n_lonticks, dtype=np.int_)
 
     return lon, lat, lon_min, lon_max, tht, phi, lenx, leny, lonticks, latticks, n_lonticks, n_latticks, lon_formatter, lg_end
 
 lat_formatter = tick.FuncFormatter(lambda v, pos: lat_formatted(v))
 con_formatter = tick.FuncFormatter(lambda v, pos:cformat(v))
 
 """
@@ -92,20 +92,22 @@
         fpath: string (None). Optional location to print image file to. Defaults to "figures/".
         bodyname: string (None). Optional body name to include in plot titles and file names.
         append: string(""). Optional string to append to filenames.
         descrip: string ("Ice--ocean"). Description of the asymmetric layer being plotted, for plot titles.
         no_title: boolean (False). If true, print figures without title text.
     """
 def plotAsym(recalc, do_large, index=-2, cmp_index=-1, r_bds=None, asym_shape=None, pvals=None, qvals=None, inpath=None,
-             fpath=None, outFname=None, bodyname=None, append="", descrip="Ice--ocean", no_title=False):
+             fpath=None, outFname=None, bodyname=None, append="", descrip="Ice--ocean", no_title=False, lfig_dpi=None):
     lon, lat, lon_min, lon_max, tht, phi, lenx, leny, lonticks, latticks, n_lonticks, n_latticks, lon_formatter, lg_end = get_latlon(do_large)
     do_cbar = not do_large
 
     if fpath is None:
         fpath = "figures"
+    if lfig_dpi is None:
+        lfig_dpi = fig_dpi
 
     if bodyname is None:
         bfname = ""
         bstr = ""
     else:
         bfname = f"_{bodyname}"
         bstr = f"{bodyname}_"
@@ -207,16 +209,16 @@
     axes.set_xticks([])
     axes.set_yticks([])
     cbar_title = "Layer thickness $(\mathrm{km})$"
     cbar_top = ""
     if do_cbar:
         cbar_ax = fig.add_axes(cbar_pos)
     else:
-        lonticks = np.linspace(lon_min, lon_max, 5, dtype=np.int)
-        latticks = np.linspace(lat_min, lat_max, 5, dtype=np.int)
+        lonticks = np.linspace(lon_min, lon_max, 5, dtype=np.int_)
+        latticks = np.linspace(lat_min, lat_max, 5, dtype=np.int_)
 
     themap = plt.axes()
     fig.subplots_adjust(left=0.07, right=0.88, wspace=0.15, hspace=0.05, top=0.90, bottom=0.07)
 
     # Apply plot formatting
     themap.set_xticks(lonticks)
     themap.set_yticks(latticks)
@@ -241,30 +243,28 @@
         ptitle = f"{descrip} thickness $(\mathrm{{km}})$, $\overline{{D}}={abs(mean_thick):.0f}\,\mathrm{{km}}$"
         tsize = deft_tsize * 1.5
     themap.tick_params(axis='both', which='major', labelsize=tick_size)
     if not no_title:
         fig.suptitle(ptitle, size=tsize)
 
     # Plot the data
-    mesh = plt.pcolormesh(lon_adj, lat, thicks_adj, shading="auto", cmap="PuBu_r")
+    mesh = plt.pcolormesh(lon_adj, lat, thicks_adj, shading="auto", cmap="PuBu_r", rasterized=True)
     cont = plt.contour(lon_adj, lat, thicks_adj, levels=levels, colors="black")
     lbls = plt.clabel(cont, fmt="%1.0f", fontsize=clabel_size, inline_spacing=clabel_pad)
 
     # Finish formatting (as long as we're not making big-label plots)
     if do_cbar:
         cbar = fig.colorbar(mesh, cax=cbar_ax, label=cbar_title, ticks=levels, format="%1.0f")
         cbar.ax.set_title(cbar_top, pad=cbar_adj, size=12)
 
     # Save the figure
     topofig = f"{bstr}asym_contour"
     print_fname = os.path.join(fpath, f"{topofig}{append}{lg_end}")
-    fig.savefig(f"{print_fname}.png", format="png", dpi=300)
-    if not do_large:
-        fig.savefig(f"{print_fname}.pdf", format="pdf")
-    log.info(f"Contour plot for asym bdy saved to: {print_fname}.png")
+    fig.savefig(f"{print_fname}.{fmt}", format=fmt, dpi=lfig_dpi,)
+    log.info(f"Contour plot for asym bdy saved to: {print_fname}.{fmt}")
 
     return
 
 #############################################
 
 # For configuring longitudes from -180 to 180 or 0 to 360.
 def east_formatted(longitude, EAST=True):
@@ -351,34 +351,33 @@
             empty string to use standard labelling; otherwise images will get set up as animation frames.
         tstr: string (""). String to use to describe the frame's timestamp in the image title.
         component: string (None). Optional component to plot instead of magnitude. Accepts 'x', 'y', and 'z'.
         absolute: boolean (False). Optional flag to plot the absolute induced field in addition to differences.
         no_title: boolean (False). If true, print figures without title text.
         outFname: string (None). Optional string with full file path to override other infrastructure for determining output path.
         gnm, hnm: complex, shape(n_max+1,n_max+1). Schmidt semi-normalized magnetic moments. Passed as a tuple in Binm.
+        marks: tuple of 2 arrays, each shape(j). Lat/lon pairs (array 1 is lat, array 2 is lon) in degrees to mark on the plot.
     """
 def plotMagSurf(n_peaks, Binm, nvals, mvals, do_large, Schmidt=False, r_surf_mean=1.0, asym_frac=None, pvals=None, qvals=None,
                 difference=False, Binm_sph=None, nprmvals=None, mprmvals=None, fpath=None, bodyname=None, append="", fend="",
-                tstr="", component=None, absolute=False, no_title=False, outFname=None, fmt=None, title=None, sym_title=None,
-                fig_dpi=None):
+                tstr="", component=None, absolute=False, no_title=False, outFname=None, title=None, sym_title=None,
+                lfig_dpi=None, marks=None):
     lon, lat, lon_min, lon_max, tht, phi, lenx, leny, lonticks, latticks, n_lonticks, n_latticks, lon_formatter, lg_end = get_latlon(do_large)
     do_cbar = not do_large
 
     if Schmidt:
         gnm, hnm = Binm
         if difference:
             gnm_sph, hnm_sph = Binm_sph
 
     if outFname is None:
         if fpath is None:
             fpath = "figures"
-    if fmt is None:
-        fmt = 'png'
-    if fig_dpi is None:
-        fig_dpi = 150
+    if lfig_dpi is None:
+        lfig_dpi = fig_dpi
     if component is None:
         compstr = ""
         comptitlestr = " magnitude"
         substr = "{\mathrm{mag}"
         field_cmap = "afmhot"
     else:
         compstr = component
@@ -609,17 +608,20 @@
     # Generate the plot
 
     if difference:
         plot_cmap = diff_cmap
     else:
         plot_cmap = field_cmap
 
-    mesh = plt.pcolormesh(lon, lat, B_plot, shading="auto", cmap=plot_cmap, vmin=minval, vmax=maxval)
+    mesh = plt.pcolormesh(lon, lat, B_plot, shading="auto", cmap=plot_cmap, vmin=minval, vmax=maxval, rasterized=True)
     cont = plt.contour(lon, lat, B_plot, levels=clevels, colors="black")
     lbls = plt.clabel(cont, fmt=con_formatter, fontsize=clabel_size, inline_spacing=clabel_pad)
+    # Mark points if passed
+    if marks is not None:
+        marked = plt.scatter(marks[1], marks[0], color=cMark, edgecolors=cMarkE, marker=stMark, s=szMark)
 
     # Show colorbar if there's room
     if do_cbar:
         cbar = fig.colorbar(mesh, cax=cbar_ax, label=cbar_title)
         cbar.ax.set_title(cbar_top, pad=cbar_adj, size=12)
 
     # Save the figure
@@ -628,22 +630,22 @@
         sym_topofig = "field_sym"
         asym_topofig = "field_asym"
     else:
         topofig = f"{bodyname}_field_asym{append}{fname_diff}{lg_end}{fend}"
         sym_topofig = f"{bodyname}_field_sym"
         asym_topofig = f"{bodyname}_field_asym"
 
+    lfmt = fmt + ''
     if outFname is None:
-        if fend == "":
-            if not do_large and save_vector:
-                fig.savefig(os.path.join(fpath, f"{topofig}.pdf"), format="pdf")
-        else:
+        if fend != "":
             fpath = os.path.join(fpath, "anim_frames")
-        outFname = os.path.join(fpath, f"{topofig}.{fmt}")
-    fig.savefig(outFname, format=fmt, dpi=fig_dpi)
+            lfmt = animFmt
+
+        outFname = os.path.join(fpath, f"{topofig}.{lfmt}")
+    fig.savefig(outFname, format=lfmt, dpi=lfig_dpi)
     log.info(f"Contour plot for asym field saved to: {outFname}")
 
     # Plot the absolute induced field in addition to a difference
     if (absolute and difference) and fend=="":
         for old_cont in cont.collections:
             old_cont.remove()
         for old_lbls in lbls:
@@ -664,23 +666,25 @@
             abs_cmap = "seismic"
 
         mesh.set_array(asym_plot)
         mesh.set_cmap(abs_cmap)
         mesh.set_clim(minval, maxval)
         cont = plt.contour(lon, lat, asym_plot, colors="black")
         lbls = plt.clabel(cont, fmt=con_formatter, fontsize=clabel_size, inline_spacing=clabel_pad)
+        if marks is not None:
+            marked = plt.scatter(marks[1], marks[0], color=cMark, edgecolors=cMarkE, marker=stMark, s=szMark)
 
         if do_cbar:
             cbar.set_label(abs_cbar_title)
 
         if not no_title:
             fig.suptitle(asym_ptitle, size=tsize)
         print_abs_asym_fname = os.path.join(fpath, f"{asym_topofig}{append}{lg_end}")
-        fig.savefig(f"{print_abs_asym_fname}.png", format="png", dpi=fig_dpi)
-        log.info(f"Contour plot for absolute asym field saved to: {print_abs_asym_fname}.png")
+        fig.savefig(f"{print_abs_asym_fname}.{fmt}", format=fmt, dpi=lfig_dpi)
+        log.info(f"Contour plot for absolute asym field saved to: {print_abs_asym_fname}.{fmt}")
 
         # Plot analogous plot for field from symmetric shape for comparison
         for old_cont in cont.collections:
             old_cont.remove()
         for old_lbls in lbls:
             old_lbls.remove()
         del cont
@@ -695,29 +699,31 @@
         sym_clevels = np.linspace(minval, maxval, 10, endpoint=True)
 
         mesh.set_array(sym_plot)
         mesh.set_cmap(abs_cmap)
         mesh.set_clim(minval,maxval)
         cont = plt.contour(lon, lat, sym_plot, colors="black")
         lbls = plt.clabel(cont, fmt=con_formatter, fontsize=clabel_size, inline_spacing=clabel_pad)
+        if marks is not None:
+            marked = plt.scatter(marks[1], marks[0], color=cMark, edgecolors=cMarkE, marker=stMark, s=szMark)
 
         if do_cbar:
             cbar.set_label(abs_cbar_title)
 
         if not no_title:
             if fend != "":
                 title_tstring = f" at t={tstr} h"
             else:
                 title_tstring = ""
             if sym_title is None:
                 sym_title = f"{sym_ptitle}{title_tstring}"
             fig.suptitle(sym_title, size=tsize)
         print_abs_sym_fname = os.path.join(fpath, f"{sym_topofig}{append}{lg_end}")
-        fig.savefig(f"{print_abs_sym_fname}.png", format="png", dpi=fig_dpi)
-        log.info(f"Contour plot for absolute sym field saved to: {print_abs_sym_fname}.png")
+        fig.savefig(f"{print_abs_sym_fname}.{fmt}", format=fmt, dpi=lfig_dpi)
+        log.info(f"Contour plot for absolute sym field saved to: {print_abs_sym_fname}.{fmt}")
 
     plt.close()
     return
 
 #############################################
 
 
@@ -740,17 +746,20 @@
         component: string (None). Component of magnetic field to plot. Options are None (for magnitude), "x", "y", or "z".
         Binm_sph: complex, shape(2, nprm_max+1, nprm_max+1) OR shape(Nnmprm) (None). Optional induced moments for a spherically symmetric body,
             to plot for comparison purposes.
         bodyname: string (None). Name of the body being modeled for titles and filenames.
         append: string (""). Optional string to append to filenames.
         fpath: string (None). Optional path to figure save location. Passing None defaults to "figures/".  
     """
-def plotTimeSeries(loc, Binm, Benm, t_start, T_hrs, nprm_max, n_max, nvals, mvals, n_pts=200, component=None, Binm_sph=None, bodyname=None, append="", fpath=None):
+def plotTimeSeries(loc, Binm, Benm, t_start, T_hrs, nprm_max, n_max, nvals, mvals, n_pts=200, component=None, Binm_sph=None, bodyname=None, append="", fpath=None,
+                   lfig_dpi=None):
     if fpath is None:
         fpath = "figures"
+    if lfig_dpi is None:
+        lfig_dpi = fig_dpi
 
     T_secs = T_hrs * 3600
     x = loc[0]
     y = loc[1]
     z = loc[2]
     r = loc[3]
     t_s = np.arange(t_start, t_start+T_secs, T_secs/n_pts)
@@ -857,16 +866,15 @@
     axes.plot(t_h, Bplot, color=c[0], label=asym_label)
     if Binm_sph is not None:
         axes.plot(t_h, Bplot_sph, color=c[1], label=sym_label)
         plt.legend(loc="best")
 
     #	Save and close
     fig_fname = os.path.join(fpath, f"{bodyname}_tSeries{append}")
-    fig.savefig(f"{fig_fname}.png", format="png", dpi=200)
-    fig.savefig(f"{fig_fname}.pdf", format="pdf")
+    fig.savefig(f"{fig_fname}.{fmt}", format=fmt, dpi=lfig_dpi)
     plt.close()
     log.info(f"Time series plot saved to file: {fig_fname}")
     return
 
 #############################################
 
 
@@ -890,17 +898,19 @@
         Binm_sph: complex, shape(n_peaks, 2, nprm_max+1, nprm_max+1) OR shape(Nnmprm) (None). Optional induced moments for a spherically symmetric body,
             to plot for comparison purposes. Required if difference == True.
         bodyname: string (None). Name of the body being modeled for titles and filenames.
         net_field: boolean (False). Whether to plot the net magnetic field or just the induced field.
         append: string (""). Optional string to append to filenames.
         fpath: string (None). Optional path to figure save location. Passing None defaults to "figures/".  
     """
-def plotTrajec(t, Bx, By, Bz, Bdat=None, bodyname=None, t_CA=None, append="", fpath=None):
+def plotTrajec(t, Bx, By, Bz, Bdat=None, bodyname=None, t_CA=None, append="", fpath=None, lfig_dpi=None):
     if fpath is None:
         fpath = "figures"
+    if lfig_dpi is None:
+        lfig_dpi = fig_dpi
 
     # Set plot labels
     fig, axes = plt.subplots(3, 1)
 
     fig.suptitle(bodyname + " net magnetic field, IAU coordinates")
     axes[-1].set_xlabel("Measurement time")
     axes[0].set_ylabel("$B_x (\mathrm{nT})$")
@@ -932,18 +942,17 @@
         axes[1].axvline(x=t_CA, color=c[2])
         axes[2].axvline(x=t_CA, color=c[2])
         topYmin, topYmax = axes[0].get_ylim()
         axes[0].text(t_CA, topYmax + (topYmax-topYmin)/20, "CA", ha="center")
 
     # Save and close
     fig_fname = os.path.join(fpath, f"{bodyname}-{append}")
-    fig.savefig(f"{fig_fname}.png", format="png", dpi=200)
-    fig.savefig(f"{fig_fname}.pdf", format="pdf")
+    fig.savefig(f"{fig_fname}.{fmt}", format=fmt, dpi=lfig_dpi)
     plt.close()
-    log.info(f"Trajectory plot saved to file: {fig_fname}.pdf")
+    log.info(f"Trajectory plot saved to file: {fig_fname}.{fmt}")
 
     return
 
 #############################################
 
 
 """
@@ -967,17 +976,19 @@
             to plot for comparison purposes. Required if difference == True.
         bodyname: string (None). Name of the body being modeled for titles and filenames.
         net_field: boolean (False). Whether to plot the net magnetic field or just the induced field.
         append: string (""). Optional string to append to filenames.
         fpath: string (None). Optional path to figure save location. Passing None defaults to "figures/".  
     """
 def calcAndPlotTrajec(x,y,z,r,t, Binm, Benm, peak_omegas, nprm_max, n_max, nvals, mvals, R_body=None, difference=False,
-               component=None, Binm_sph=None, net_field=False, bodyname=None, append="", fpath=None):
+               component=None, Binm_sph=None, net_field=False, bodyname=None, append="", fpath=None, lfig_dpi=None):
     if fpath is None:
         fpath = "figures"
+    if lfig_dpi is None:
+        lfig_dpi = fig_dpi
 
     if n_max > 10:
         n_max = 10
         log.warning(f'Evaluation of magnetic fields is supported only up to n={n_max}. n_max has been set to {n_max}.')
 
     Nnm = (n_max + 1) ** 2 - 1
     Nnmprm = (nprm_max + 1) ** 2 - 1
@@ -1127,18 +1138,17 @@
         axes.plot(plotx, Bplot, color=c[0], label=asym_label)
         if Binm_sph is not None and not difference:
             axes.plot(plotx, Bplot_sph, color=c[1], label=sym_label)
             plt.legend(loc="best")
 
     # Save and close
     fig_fname = os.path.join(fpath, f"{bodyname}{append}")
-    fig.savefig(f"{fig_fname}.png", format="png", dpi=200)
-    fig.savefig(f"{fig_fname}.pdf", format="pdf")
+    fig.savefig(f"{fig_fname}.{fmt}", format=fmt, dpi=lfig_dpi)
     plt.close()
-    log.info(f"Trajectory plot saved to file: {fig_fname}.png")
+    log.info(f"Trajectory plot saved to file: {fig_fname}.{fmt}")
 
     return
 
 #############################################
 
 
 """
@@ -1152,15 +1162,18 @@
         kr: mpc, shape(n_omegas). List of kr values against which to plot.
         n: integer. n value for which A functions have been calculated.
         Aes: mpc, shape(n_omegas). "Excitation" amplitude A_n^e.
         Ats: mpc, shape(n_omegas). "Tangential" amplitude A_n^t.
         Ads: mpc, shape(n_omegas). "Mixing" amplitude A_n'^\star.
         AtAds: mpc, shape(n_omegas). Ats and Ads multiplied together, which should be asymptotic to (1+0i).
     """
-def plotAfunctions(kr, n, Ae_mag, Ae_arg, At_mag, At_arg, Ad_mag, Ad_arg, AtAd_mag, AtAd_arg):
+def plotAfunctions(kr, n, Ae_mag, Ae_arg, At_mag, At_arg, Ad_mag, Ad_arg, AtAd_mag, AtAd_arg, lfig_dpi=None):
+    if lfig_dpi is None:
+        lfig_dpi = fig_dpi
+
     c = ["black", "blue", "brown", "green"]
     style1 = "solid"
     style2 = "dashed"
 
     #	(This is Figure 1 in the paper)
     fig, axes = plt.subplots(1, 1, figsize=(5.5, 4))
 
@@ -1205,24 +1218,26 @@
 
     #	Adjust decoration
     axes.grid()
     axes.ticklabel_format(axis="y", style="sci", scilimits=(0, 0))
 
     #	Save and close
     plt.legend(loc="best")
-    xtn = "png"
-    thefig = os.path.join("figures", f"A_functions.{xtn}")
-    fig.savefig(thefig, format=xtn, dpi=300)
+    thefig = os.path.join("figures", f"A_functions.{fmt}")
+    fig.savefig(thefig, format=fmt, dpi=lfig_dpi)
     plt.close()
     log.info(f"A functions plot printed to: {thefig}")
 
     return
 
 
-def plotAes(T_h, Ae_mag, Ae_arg, Tinterest_h, BeRatio, intModels, n=1, fEnd=""):
+def plotAes(T_h, Ae_mag, Ae_arg, Tinterest_h, BeRatio, intModels, n=1, fEnd="", lfig_dpi=None):
+    if lfig_dpi is None:
+        lfig_dpi = fig_dpi
+
     c = ["blue", "green", "brown", "black", "red"]
     style1 = "solid"
     style2 = "dashed"
 
     fig, axes = plt.subplots(1, 1, figsize=(5.5, 4))
 
     # Set plot labels
@@ -1257,17 +1272,16 @@
 
     # Adjust decoration
     axes.grid()
     axes.ticklabel_format(axis="y", style="sci", scilimits=(0, 0))
 
     # Save and close
     plt.legend(loc="upper right")
-    xtn = "png"
-    thefig = os.path.join("figures", f"A1e{fEnd}.{xtn}")
-    fig.savefig(thefig, format=xtn, dpi=300)
+    thefig = os.path.join("figures", f"A1e{fEnd}.{fmt}")
+    fig.savefig(thefig, format=fmt, dpi=lfig_dpi)
     plt.close()
     log.info(f"Ae plot printed to: {thefig}")
 
     return
 
 #	For secondary axis labels
 def getphase(A):
```

### Comparing `MoonMag-1.5.2/src/MoonMag/reduce_interior_model.py` & `MoonMag-1.5.3/MoonMag/reduce_interior_model.py`

 * *Files identical despite different names*

### Comparing `MoonMag-1.5.2/src/MoonMag/run_all.py` & `MoonMag-1.5.3/MoonMag/run_all.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,14 +4,15 @@
     Developed in Python 3.8 for "A perturbation method for evaluating the
     magnetic field induced from an arbitrary, asymmetric ocean world 
     analytically" by Styczinski et al.
     DOI: 10.1016/j.icarus.2021.114840
 Author: M. J. Styczinski, mjstyczi@uw.edu """
 
 import MoonMag.eval_induced_field as eval
+from MoonMag.config import prevEuropa, TobieHigh, TobieLow, DO_LARGE
 
 def run_all():
     # Each body to include in calculations
     do_Europa = True
     do_Miranda = True
     do_Callisto = True
     do_Triton = True
@@ -26,110 +27,123 @@
     do_fields = True  # Whether to evaluate and plot fields
     do_detailed = True  # Whether to make standard plots (this option is independent from do_large_plots)
     do_large_plots = False  # Whether to make copies with larger print and no colorbars, for cramped spaces
     
     # Uses the following command structure:
     # eval.run_calcs(bname, comp, recalc, plot_field, plot_asym, do_large=False, seawater=False, compare_me=False, do_gif=False)
 
+    opts = []
     if do_Miranda:
         bname = "Miranda"
         print(f" - {bname} - ")
         if do_detailed:
-            eval.run_calcs(bname, None, do_recalc, do_fields, initial_contour, do_large=False)
-            eval.run_calcs(bname, "x", False, do_fields, False, do_large=False)
-            eval.run_calcs(bname, "y", False, do_fields, False, do_large=False)
-            eval.run_calcs(bname, "z", False, do_fields, False, do_large=False)
+            eval.run_calcs(bname, None, do_recalc, do_fields, initial_contour, modelOpts=opts)
+            eval.run_calcs(bname, "x", False, do_fields, False, modelOpts=opts)
+            eval.run_calcs(bname, "y", False, do_fields, False, modelOpts=opts)
+            eval.run_calcs(bname, "z", False, do_fields, False, modelOpts=opts)
 
         if do_large_plots:
-            eval.run_calcs(bname, None, False, do_fields, initial_contour, do_large=True)
-            eval.run_calcs(bname, "x", False, do_fields, False, do_large=True)
-            eval.run_calcs(bname, "y", False, do_fields, False, do_large=True)
-            eval.run_calcs(bname, "z", False, do_fields, False, do_large=True)
+            opts += [DO_LARGE]
+            eval.run_calcs(bname, None, do_recalc and not do_detailed, do_fields, initial_contour, modelOpts=opts)
+            eval.run_calcs(bname, "x", False, do_fields, False, modelOpts=opts)
+            eval.run_calcs(bname, "y", False, do_fields, False, modelOpts=opts)
+            eval.run_calcs(bname, "z", False, do_fields, False, modelOpts=opts)
 
     if do_Europa:
         bname = "Europa"
         print(f" - {bname} Tobie model high salinity (Seawater) - ")
+        opts = [TobieHigh]
         if do_detailed:
-            eval.run_calcs(bname, None, do_recalc, do_fields, initial_contour, seawater=True)
-            eval.run_calcs(bname, "x", False, do_fields, False, seawater=True)
-            eval.run_calcs(bname, "y", False, do_fields, False, seawater=True)
-            eval.run_calcs(bname, "z", False, do_fields, False, seawater=True)
+            eval.run_calcs(bname, None, do_recalc, do_fields, initial_contour, modelOpts=opts)
+            eval.run_calcs(bname, "x", False, do_fields, False, modelOpts=opts)
+            eval.run_calcs(bname, "y", False, do_fields, False, modelOpts=opts)
+            eval.run_calcs(bname, "z", False, do_fields, False, modelOpts=opts)
 
         if do_large_plots:
-            eval.run_calcs(bname, None, False, do_fields, initial_contour, do_large=True, seawater=True)
-            eval.run_calcs(bname, "x", False, do_fields, False, do_large=True, seawater=True)
-            eval.run_calcs(bname, "y", False, do_fields, False, do_large=True, seawater=True)
-            eval.run_calcs(bname, "z", False, do_fields, False, do_large=True, seawater=True)
-    
+            opts += [DO_LARGE]
+            eval.run_calcs(bname, None, do_recalc and not do_detailed, do_fields, initial_contour, modelOpts=opts)
+            eval.run_calcs(bname, "x", False, do_fields, False, modelOpts=opts)
+            eval.run_calcs(bname, "y", False, do_fields, False, modelOpts=opts)
+            eval.run_calcs(bname, "z", False, do_fields, False, modelOpts=opts)
+
         bname = "Europa"
         print(f" - {bname} Tobie model low salinity (10% Seawater) - ")
+        opts = [TobieLow]
         if do_detailed:
-            eval.run_calcs(bname, None, do_recalc, do_fields, initial_contour, seawater=False)
-            eval.run_calcs(bname, "x", False, do_fields, False, seawater=False)
-            eval.run_calcs(bname, "y", False, do_fields, False, seawater=False)
-            eval.run_calcs(bname, "z", False, do_fields, False, seawater=False)
+            eval.run_calcs(bname, None, do_recalc, do_fields, initial_contour, modelOpts=opts)
+            eval.run_calcs(bname, "x", False, do_fields, False, modelOpts=opts)
+            eval.run_calcs(bname, "y", False, do_fields, False, modelOpts=opts)
+            eval.run_calcs(bname, "z", False, do_fields, False, modelOpts=opts)
     
         if do_large_plots:
-            eval.run_calcs(bname, None, False, do_fields, initial_contour, do_large=True, seawater=False)
-            eval.run_calcs(bname, "x", False, do_fields, False, do_large=True, seawater=False)
-            eval.run_calcs(bname, "y", False, do_fields, False, do_large=True, seawater=False)
-            eval.run_calcs(bname, "z", False, do_fields, False, do_large=True, seawater=False)
-    
+            opts += [DO_LARGE]
+            eval.run_calcs(bname, None, do_recalc and not do_detailed, do_fields, initial_contour, modelOpts=opts)
+            eval.run_calcs(bname, "x", False, do_fields, False, modelOpts=opts)
+            eval.run_calcs(bname, "y", False, do_fields, False, modelOpts=opts)
+            eval.run_calcs(bname, "z", False, do_fields, False, modelOpts=opts)
+
         bname = "Europa"
         print(f" - {bname} previous comparison - ")
+        opts = [prevEuropa]
         if do_detailed:
-            eval.run_calcs(bname, None, do_recalc, do_fields, initial_contour, compare_me=True)
-            eval.run_calcs(bname, "x", False, do_fields, False, compare_me=True)
-            eval.run_calcs(bname, "y", False, do_fields, False, compare_me=True)
-            eval.run_calcs(bname, "z", False, do_fields, False, compare_me=True)
+            eval.run_calcs(bname, None, do_recalc, do_fields, initial_contour, modelOpts=opts)
+            eval.run_calcs(bname, "x", False, do_fields, False, modelOpts=opts)
+            eval.run_calcs(bname, "y", False, do_fields, False, modelOpts=opts)
+            eval.run_calcs(bname, "z", False, do_fields, False, modelOpts=opts)
     
         if do_large_plots:
-            eval.run_calcs(bname, None, False, do_fields, initial_contour, do_large=True, compare_me=True)
-            eval.run_calcs(bname, "x", False, do_fields, False, do_large=True, compare_me=True)
-            eval.run_calcs(bname, "y", False, do_fields, False, do_large=True, compare_me=True)
-            eval.run_calcs(bname, "z", False, do_fields, False, do_large=True, compare_me=True)
+            opts += [DO_LARGE]
+            eval.run_calcs(bname, None, do_recalc and not do_detailed, do_fields, initial_contour, modelOpts=opts)
+            eval.run_calcs(bname, "x", False, do_fields, False, modelOpts=opts)
+            eval.run_calcs(bname, "y", False, do_fields, False, modelOpts=opts)
+            eval.run_calcs(bname, "z", False, do_fields, False, modelOpts=opts)
     
     if do_Callisto:
         bname = "Callisto"
         print(f" - {bname} - ")
+        opts = []
         if do_detailed:
-            eval.run_calcs(bname, None, do_recalc, do_fields, initial_contour)
-            eval.run_calcs(bname, "x", False, do_fields, False)
-            eval.run_calcs(bname, "y", False, do_fields, False)
-            eval.run_calcs(bname, "z", False, do_fields, False)
+            eval.run_calcs(bname, None, do_recalc, do_fields, initial_contour, modelOpts=opts)
+            eval.run_calcs(bname, "x", False, do_fields, False, modelOpts=opts)
+            eval.run_calcs(bname, "y", False, do_fields, False, modelOpts=opts)
+            eval.run_calcs(bname, "z", False, do_fields, False, modelOpts=opts)
     
         if do_large_plots:
-            eval.run_calcs(bname, None, False, do_fields, initial_contour, do_large=True)
-            eval.run_calcs(bname, "x", False, do_fields, False, do_large=True)
-            eval.run_calcs(bname, "y", False, do_fields, False, do_large=True)
-            eval.run_calcs(bname, "z", False, do_fields, False, do_large=True)
+            opts += [DO_LARGE]
+            eval.run_calcs(bname, None, do_recalc and not do_detailed, do_fields, initial_contour, modelOpts=opts)
+            eval.run_calcs(bname, "x", False, do_fields, False, modelOpts=opts)
+            eval.run_calcs(bname, "y", False, do_fields, False, modelOpts=opts)
+            eval.run_calcs(bname, "z", False, do_fields, False, modelOpts=opts)
     
     if do_Triton:
         bname = "Triton"
         print(f" - {bname} - ")
+        opts = []
         if do_detailed:
-            eval.run_calcs(bname, None, do_recalc, do_fields, initial_contour)
-            eval.run_calcs(bname, "x", False, do_fields, False)
-            eval.run_calcs(bname, "y", False, do_fields, False)
-            eval.run_calcs(bname, "z", False, do_fields, False)
+            eval.run_calcs(bname, None, do_recalc, do_fields, initial_contour, modelOpts=opts)
+            eval.run_calcs(bname, "x", False, do_fields, False, modelOpts=opts)
+            eval.run_calcs(bname, "y", False, do_fields, False, modelOpts=opts)
+            eval.run_calcs(bname, "z", False, do_fields, False, modelOpts=opts)
     
         if do_large_plots:
-            eval.run_calcs(bname, None, False, do_fields, initial_contour, do_large=True)
-            eval.run_calcs(bname, "x", False, do_fields, False, do_large=True)
-            eval.run_calcs(bname, "y", False, do_fields, False, do_large=True)
-            eval.run_calcs(bname, "z", False, do_fields, False, do_large=True)
+            opts += [DO_LARGE]
+            eval.run_calcs(bname, None, do_recalc and not do_detailed, do_fields, initial_contour, modelOpts=opts)
+            eval.run_calcs(bname, "x", False, do_fields, False, modelOpts=opts)
+            eval.run_calcs(bname, "y", False, do_fields, False, modelOpts=opts)
+            eval.run_calcs(bname, "z", False, do_fields, False, modelOpts=opts)
     
     if make_gifs:
+        opts = [DO_GIF]
         if do_Europa:
-            eval.run_calcs("Europa", gif_comp, False, True, False, seawater=True, do_gif=True)
-            eval.run_calcs("Europa", gif_comp, False, True, False, seawater=False, do_gif=True)
-            eval.run_calcs("Europa", gif_comp, False, True, False, compare_me=True, do_gif=True)
+            eval.run_calcs("Europa", gif_comp, False, True, False, modelOpts=opts+[TobieHigh])
+            eval.run_calcs("Europa", gif_comp, False, True, False, modelOpts=opts+[TobieLow])
+            eval.run_calcs("Europa", gif_comp, False, True, False, modelOpts=opts+[prevEuropa])
         if do_Miranda:
-            eval.run_calcs("Miranda", gif_comp, False, True, False, do_gif=True)
+            eval.run_calcs("Miranda", gif_comp, False, True, False, modelOpts=opts)
         if do_Callisto:
-            eval.run_calcs("Callisto", gif_comp, False, True, False, do_gif=True)
+            eval.run_calcs("Callisto", gif_comp, False, True, False, modelOpts=opts)
         if do_Triton:
-            eval.run_calcs("Triton", gif_comp, False, True, False, do_gif=True)
+            eval.run_calcs("Triton", gif_comp, False, True, False, modelOpts=opts)
 
 
 if __name__ == "__main__":
     run_all()
```

### Comparing `MoonMag-1.5.2/src/MoonMag/symmetry_funcs.py` & `MoonMag-1.5.3/MoonMag/symmetry_funcs.py`

 * *Files identical despite different names*

### Comparing `MoonMag-1.5.2/src/MoonMag/trajec_analysis.py` & `MoonMag-1.5.3/MoonMag/trajec_analysis.py`

 * *Files identical despite different names*

### Comparing `MoonMag-1.5.2/src/MoonMag.egg-info/PKG-INFO` & `MoonMag-1.5.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: MoonMag
-Version: 1.5.2
+Version: 1.5.3
 Summary: Magnetic induction calculations for sounding of icy moons
 Home-page: https://github.com/itsmoosh/MoonMag
 Author: Marshall J. Styczinski
 Author-email: marshall.j.styczinski@jpl.nasa.gov
-Project-URL: Bug Tracker, https://github.com/itsmoosh/MoonMag/issues
+Project-URL: Bug tracker, https://github.com/itsmoosh/MoonMag/issues
 Project-URL: Original publication, https://doi.org/10.1016/j.icarus.2021.114840
-Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # MoonMag
+<img src="misc/MoonMag_logo.png" width=240 title="MoonMag logo"/>
+
 ## Magnetic induction calculations and analysis for sounding of icy moons
 Written in Python 3.8 as supplemental material for "An analytic solution for evaluating the magnetic field induced from an arbitrary, asymmetric ocean world" DOI: [10.1016/j.icarus.2021.114840](https://doi.org/10.1016/j.icarus.2021.114840). For help, please contact M. Styczinski at [marshall.j.styczinski@jpl.nasa.gov](mailto:marshall.j.styczinski@jpl.nasa.gov).
 
 The main repository is mirrored at https://github.com/NASA-Planetary-Science/MoonMag; any pull requests should be submitted to https://github.com/itsmoosh/MoonMag.
 
 ## Acknowledging MoonMag
 Thank you for your interest in MoonMag! Please consider alerting us to your work (marshall.j.styczinski@jpl.nasa.gov). Suggested acknowledgement in publications: "Data used in this work were generated with the open source MoonMag framework hosted on GitHub."
```

### Comparing `MoonMag-1.5.2/src/MoonMag.egg-info/SOURCES.txt` & `MoonMag-1.5.3/MoonMag.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,105 +1,111 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
-setup.cfg
 setup.py
-src/MoonMag/__init__.py
-src/MoonMag/asymmetry_funcs.py
-src/MoonMag/calc_Ganymede_induced.py
-src/MoonMag/calc_trajec_induced.py
-src/MoonMag/config.py
-src/MoonMag/eval_induced_field.py
-src/MoonMag/field_xyz.py
-src/MoonMag/plot_Aes.py
-src/MoonMag/plotting_funcs.py
-src/MoonMag/reduce_interior_model.py
-src/MoonMag/run_all.py
-src/MoonMag/symmetry_funcs.py
-src/MoonMag/trajec_analysis.py
-src/MoonMag.egg-info/PKG-INFO
-src/MoonMag.egg-info/SOURCES.txt
-src/MoonMag.egg-info/dependency_links.txt
-src/MoonMag.egg-info/requires.txt
-src/MoonMag.egg-info/top_level.txt
-src/MoonMag/excitation/Be1xyz.txt
-src/MoonMag/excitation/Be1xyz_Callisto.txt
-src/MoonMag/excitation/Be1xyz_Europa.txt
-src/MoonMag/excitation/Be1xyz_Miranda.txt
-src/MoonMag/excitation/Be1xyz_Triton.txt
-src/MoonMag/excitation/Be2xyz.txt
-src/MoonMag/excitation/orbital_Be1xyz_Callisto.txt
-src/MoonMag/excitation/orbital_Be1xyz_Europa.txt
-src/MoonMag/excitation/orbital_Be1xyz_Miranda.txt
-src/MoonMag/excitation/orbital_Be1xyz_Triton.txt
-src/MoonMag/excitation/synodic_Be1xyz_Callisto.txt
-src/MoonMag/excitation/synodic_Be1xyz_Europa.txt
-src/MoonMag/excitation/synodic_Be1xyz_Miranda.txt
-src/MoonMag/excitation/synodic_Be1xyz_Triton.txt
-src/MoonMag/induced/Xid_values_n1_p10_np11.mat
-src/MoonMag/induced/Xid_values_n1_p2_np3.mat
-src/MoonMag/induced/Xid_values_n1_p4_np5.mat
-src/MoonMag/induced/Xid_values_n1_p8_np9.mat
-src/MoonMag/interior/degree1_shapes.txt
-src/MoonMag/interior/degree1_shapes_Callisto.txt
-src/MoonMag/interior/degree1_shapes_Europa_Tobie.txt
-src/MoonMag/interior/degree1_shapes_Europa_prev.txt
-src/MoonMag/interior/degree1_shapes_Miranda.txt
-src/MoonMag/interior/degree1_shapes_Triton.txt
-src/MoonMag/interior/degree2_shapes.txt
-src/MoonMag/interior/degree2_shapes_Callisto.txt
-src/MoonMag/interior/degree2_shapes_Europa_Tobie.txt
-src/MoonMag/interior/degree2_shapes_Europa_prev.txt
-src/MoonMag/interior/degree2_shapes_Miranda.txt
-src/MoonMag/interior/degree2_shapes_Triton.txt
-src/MoonMag/interior/degree3_shapes.txt
-src/MoonMag/interior/degree3_shapes_Callisto.txt
-src/MoonMag/interior/degree3_shapes_Europa_Tobie.txt
-src/MoonMag/interior/degree3_shapes_Europa_prev.txt
-src/MoonMag/interior/degree3_shapes_Miranda.txt
-src/MoonMag/interior/degree3_shapes_Triton.txt
-src/MoonMag/interior/degree4_shapes.txt
-src/MoonMag/interior/degree4_shapes_Callisto.txt
-src/MoonMag/interior/degree4_shapes_Europa_Tobie.txt
-src/MoonMag/interior/degree4_shapes_Europa_prev.txt
-src/MoonMag/interior/degree4_shapes_Miranda.txt
-src/MoonMag/interior/degree4_shapes_Triton.txt
-src/MoonMag/interior/degree5_shapes.txt
-src/MoonMag/interior/degree5_shapes_Callisto.txt
-src/MoonMag/interior/degree5_shapes_Europa_Tobie.txt
-src/MoonMag/interior/degree5_shapes_Europa_prev.txt
-src/MoonMag/interior/degree5_shapes_Miranda.txt
-src/MoonMag/interior/degree5_shapes_Triton.txt
-src/MoonMag/interior/degree6_shapes.txt
-src/MoonMag/interior/degree6_shapes_Callisto.txt
-src/MoonMag/interior/degree6_shapes_Europa_Tobie.txt
-src/MoonMag/interior/degree6_shapes_Europa_prev.txt
-src/MoonMag/interior/degree6_shapes_Miranda.txt
-src/MoonMag/interior/degree6_shapes_Triton.txt
-src/MoonMag/interior/degree7_shapes.txt
-src/MoonMag/interior/degree7_shapes_Callisto.txt
-src/MoonMag/interior/degree7_shapes_Europa_Tobie.txt
-src/MoonMag/interior/degree7_shapes_Europa_prev.txt
-src/MoonMag/interior/degree7_shapes_Miranda.txt
-src/MoonMag/interior/degree7_shapes_Triton.txt
-src/MoonMag/interior/degree8_shapes.txt
-src/MoonMag/interior/degree8_shapes_Callisto.txt
-src/MoonMag/interior/degree8_shapes_Europa_Tobie.txt
-src/MoonMag/interior/degree8_shapes_Europa_prev.txt
-src/MoonMag/interior/degree8_shapes_Miranda.txt
-src/MoonMag/interior/degree8_shapes_Triton.txt
-src/MoonMag/interior/depth_chi_pq_shape_Callisto.txt
-src/MoonMag/interior/depth_chi_pq_shape_Enceladus.txt
-src/MoonMag/interior/depth_chi_pq_shape_Europa.txt
-src/MoonMag/interior/depth_chi_pq_shape_Europa_Tobie.txt
-src/MoonMag/interior/depth_chi_pq_shape_Miranda.txt
-src/MoonMag/interior/depth_chi_pq_shape_Triton.txt
-src/MoonMag/interior/gravity_Europa_Tobie.txt
-src/MoonMag/interior/interior_model_asym.txt
-src/MoonMag/interior/interior_model_asym_Callisto.txt
-src/MoonMag/interior/interior_model_asym_Enceladus.txt
-src/MoonMag/interior/interior_model_asym_Europa_Tobie_high.txt
-src/MoonMag/interior/interior_model_asym_Europa_Tobie_low.txt
-src/MoonMag/interior/interior_model_asym_Europa_prev.txt
-src/MoonMag/interior/interior_model_asym_Miranda.txt
-src/MoonMag/interior/interior_model_asym_Triton.txt
+MoonMag/__init__.py
+MoonMag/asymmetry_funcs.py
+MoonMag/calc_Ganymede_induced.py
+MoonMag/calc_trajec_induced.py
+MoonMag/config.py
+MoonMag/eval_induced_field.py
+MoonMag/field_xyz.py
+MoonMag/plot_Aes.py
+MoonMag/plotting_funcs.py
+MoonMag/reduce_interior_model.py
+MoonMag/run_all.py
+MoonMag/symmetry_funcs.py
+MoonMag/trajec_analysis.py
+MoonMag.egg-info/PKG-INFO
+MoonMag.egg-info/SOURCES.txt
+MoonMag.egg-info/dependency_links.txt
+MoonMag.egg-info/requires.txt
+MoonMag.egg-info/top_level.txt
+MoonMag/excitation/Be1xyz.txt
+MoonMag/excitation/Be1xyz_Callisto.txt
+MoonMag/excitation/Be1xyz_Europa.txt
+MoonMag/excitation/Be1xyz_Miranda.txt
+MoonMag/excitation/Be1xyz_Triton.txt
+MoonMag/excitation/Be2xyz.txt
+MoonMag/excitation/orbital_Be1xyz_Callisto.txt
+MoonMag/excitation/orbital_Be1xyz_Europa.txt
+MoonMag/excitation/orbital_Be1xyz_Miranda.txt
+MoonMag/excitation/orbital_Be1xyz_Triton.txt
+MoonMag/excitation/synodic_Be1xyz_Callisto.txt
+MoonMag/excitation/synodic_Be1xyz_Europa.txt
+MoonMag/excitation/synodic_Be1xyz_Miranda.txt
+MoonMag/excitation/synodic_Be1xyz_Triton.txt
+MoonMag/induced/Xid_values_n1_p10_np11.mat
+MoonMag/induced/Xid_values_n1_p2_np3.mat
+MoonMag/induced/Xid_values_n1_p4_np5.mat
+MoonMag/induced/Xid_values_n1_p8_np9.mat
+MoonMag/interior/chi_pq_Callisto.txt
+MoonMag/interior/chi_pq_Europa.txt
+MoonMag/interior/chi_pq_Miranda.txt
+MoonMag/interior/chi_pq_Triton.txt
+MoonMag/interior/degree1_shapes.txt
+MoonMag/interior/degree1_shapes_Callisto.txt
+MoonMag/interior/degree1_shapes_Europa_Tobie.txt
+MoonMag/interior/degree1_shapes_Europa_prev.txt
+MoonMag/interior/degree1_shapes_Miranda.txt
+MoonMag/interior/degree1_shapes_Triton.txt
+MoonMag/interior/degree2_shapes.txt
+MoonMag/interior/degree2_shapes_Callisto.txt
+MoonMag/interior/degree2_shapes_Europa_Tobie.txt
+MoonMag/interior/degree2_shapes_Europa_prev.txt
+MoonMag/interior/degree2_shapes_Miranda.txt
+MoonMag/interior/degree2_shapes_Triton.txt
+MoonMag/interior/degree3_shapes.txt
+MoonMag/interior/degree3_shapes_Callisto.txt
+MoonMag/interior/degree3_shapes_Europa_Tobie.txt
+MoonMag/interior/degree3_shapes_Europa_prev.txt
+MoonMag/interior/degree3_shapes_Miranda.txt
+MoonMag/interior/degree3_shapes_Triton.txt
+MoonMag/interior/degree4_shapes.txt
+MoonMag/interior/degree4_shapes_Callisto.txt
+MoonMag/interior/degree4_shapes_Europa_Tobie.txt
+MoonMag/interior/degree4_shapes_Europa_prev.txt
+MoonMag/interior/degree4_shapes_Miranda.txt
+MoonMag/interior/degree4_shapes_Triton.txt
+MoonMag/interior/degree5_shapes.txt
+MoonMag/interior/degree5_shapes_Callisto.txt
+MoonMag/interior/degree5_shapes_Europa_Tobie.txt
+MoonMag/interior/degree5_shapes_Europa_prev.txt
+MoonMag/interior/degree5_shapes_Miranda.txt
+MoonMag/interior/degree5_shapes_Triton.txt
+MoonMag/interior/degree6_shapes.txt
+MoonMag/interior/degree6_shapes_Callisto.txt
+MoonMag/interior/degree6_shapes_Europa_Tobie.txt
+MoonMag/interior/degree6_shapes_Europa_prev.txt
+MoonMag/interior/degree6_shapes_Miranda.txt
+MoonMag/interior/degree6_shapes_Triton.txt
+MoonMag/interior/degree7_shapes.txt
+MoonMag/interior/degree7_shapes_Callisto.txt
+MoonMag/interior/degree7_shapes_Europa_Tobie.txt
+MoonMag/interior/degree7_shapes_Europa_prev.txt
+MoonMag/interior/degree7_shapes_Miranda.txt
+MoonMag/interior/degree7_shapes_Triton.txt
+MoonMag/interior/degree8_shapes.txt
+MoonMag/interior/degree8_shapes_Callisto.txt
+MoonMag/interior/degree8_shapes_Europa_Tobie.txt
+MoonMag/interior/degree8_shapes_Europa_prev.txt
+MoonMag/interior/degree8_shapes_Miranda.txt
+MoonMag/interior/degree8_shapes_Triton.txt
+MoonMag/interior/depth_chi_pq_shape_Callisto.txt
+MoonMag/interior/depth_chi_pq_shape_Enceladus.txt
+MoonMag/interior/depth_chi_pq_shape_Europa.txt
+MoonMag/interior/depth_chi_pq_shape_Europa_Tobie_high.txt
+MoonMag/interior/depth_chi_pq_shape_Europa_Tobie_low.txt
+MoonMag/interior/depth_chi_pq_shape_Europa_prev.txt
+MoonMag/interior/depth_chi_pq_shape_Miranda.txt
+MoonMag/interior/depth_chi_pq_shape_Triton.txt
+MoonMag/interior/gravity_Europa_Tobie_high.txt
+MoonMag/interior/gravity_Europa_Tobie_low.txt
+MoonMag/interior/interior_model_asym.txt
+MoonMag/interior/interior_model_asym_Callisto.txt
+MoonMag/interior/interior_model_asym_Enceladus.txt
+MoonMag/interior/interior_model_asym_Europa_Tobie_high.txt
+MoonMag/interior/interior_model_asym_Europa_Tobie_low.txt
+MoonMag/interior/interior_model_asym_Europa_prev.txt
+MoonMag/interior/interior_model_asym_Miranda.txt
+MoonMag/interior/interior_model_asym_Triton.txt
```

