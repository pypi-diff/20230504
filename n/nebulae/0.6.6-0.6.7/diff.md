# Comparing `tmp/nebulae-0.6.6.tar.gz` & `tmp/nebulae-0.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nebulae-0.6.6.tar", last modified: Sat Apr 29 14:57:00 2023, max compression
+gzip compressed data, was "nebulae-0.6.7.tar", last modified: Thu May  4 18:13:54 2023, max compression
```

## Comparing `nebulae-0.6.6.tar` & `nebulae-0.6.7.tar`

### file list

```diff
@@ -1,65 +1,64 @@
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-29 14:57:00.000000 nebulae-0.6.6/
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-29 14:57:00.000000 nebulae-0.6.6/nebulae/
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-29 14:57:00.000000 nebulae-0.6.6/nebulae/fuel/
--rw-r--r--   0 root         (0) staff       (20)     1005 2022-08-20 04:55:27.000000 nebulae-0.6.6/nebulae/fuel/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     9783 2022-08-20 04:52:42.000000 nebulae-0.6.6/nebulae/fuel/generator.py
--rw-r--r--   0 root         (0) staff       (20)    37708 2023-01-30 13:19:41.000000 nebulae-0.6.6/nebulae/fuel/comburant.py
--rw-r--r--   0 root         (0) staff       (20)     7790 2022-11-01 09:29:19.000000 nebulae-0.6.6/nebulae/fuel/tank.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-29 14:57:00.000000 nebulae-0.6.6/nebulae/law/
--rw-r--r--   0 root         (0) staff       (20)      698 2021-09-14 09:32:19.000000 nebulae-0.6.6/nebulae/law/__init__.py
--rw-r--r--   0 root         (0) staff       (20)      928 2020-10-20 09:25:06.000000 nebulae-0.6.6/nebulae/law/constant.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-29 14:57:00.000000 nebulae-0.6.6/nebulae/kit/
--rw-r--r--   0 root         (0) staff       (20)     1362 2023-04-29 13:24:36.000000 nebulae-0.6.6/nebulae/kit/decorator.py
--rw-r--r--   0 root         (0) staff       (20)    25772 2022-11-04 03:44:29.000000 nebulae-0.6.6/nebulae/kit/utility.py
--rw-r--r--   0 root         (0) staff       (20)     1096 2023-04-29 13:24:36.000000 nebulae-0.6.6/nebulae/kit/__init__.py
--rw-r--r--   0 root         (0) staff       (20)      862 2022-07-22 10:10:53.000000 nebulae-0.6.6/nebulae/__init__.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-29 14:57:00.000000 nebulae-0.6.6/nebulae/cockpit/
--rw-r--r--   0 root         (0) staff       (20)     3516 2022-08-06 07:48:20.000000 nebulae-0.6.6/nebulae/cockpit/time_machine.py
--rw-r--r--   0 root         (0) staff       (20)     5219 2022-09-16 14:43:52.000000 nebulae-0.6.6/nebulae/cockpit/multiverse.py
--rw-r--r--   0 root         (0) staff       (20)      843 2022-08-06 09:24:38.000000 nebulae-0.6.6/nebulae/cockpit/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     4251 2022-09-06 15:10:12.000000 nebulae-0.6.6/nebulae/cockpit/engine.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-29 14:57:00.000000 nebulae-0.6.6/nebulae/aerolog/
--rw-r--r--   0 root         (0) staff       (20)     6383 2023-04-29 13:28:54.000000 nebulae-0.6.6/nebulae/aerolog/inspector.py
--rw-r--r--   0 root         (0) staff       (20)      733 2023-04-21 11:05:32.000000 nebulae-0.6.6/nebulae/aerolog/__init__.py
--rw-r--r--   0 root         (0) staff       (20)    14070 2023-04-29 14:54:27.000000 nebulae-0.6.6/nebulae/aerolog/dashboard.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-29 14:57:00.000000 nebulae-0.6.6/nebulae/astro/
--rw-r--r--   0 root         (0) staff       (20)    74885 2023-04-29 13:24:36.000000 nebulae-0.6.6/nebulae/astro/craft.py
--rw-r--r--   0 root         (0) staff       (20)      735 2023-04-27 15:32:39.000000 nebulae-0.6.6/nebulae/astro/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     3187 2023-04-27 15:32:39.000000 nebulae-0.6.6/nebulae/astro/dock.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-29 14:57:00.000000 nebulae-0.6.6/nebulae/astro/hangar/
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-29 14:57:00.000000 nebulae-0.6.6/nebulae/astro/hangar/GAN/
--rw-r--r--   0 root         (0) staff       (20)     1330 2022-10-26 12:11:07.000000 nebulae-0.6.6/nebulae/astro/hangar/GAN/gan.py
--rw-r--r--   0 root         (0) staff       (20)     1489 2020-11-18 08:18:05.000000 nebulae-0.6.6/nebulae/astro/hangar/GAN/wgan.py
--rw-r--r--   0 root         (0) staff       (20)     3571 2020-12-08 10:05:34.000000 nebulae-0.6.6/nebulae/astro/hangar/GAN/infogan.py
--rw-r--r--   0 root         (0) staff       (20)      667 2020-11-18 05:38:52.000000 nebulae-0.6.6/nebulae/astro/hangar/GAN/__init__.py
--rw-r--r--   0 root         (0) staff       (20)    27430 2022-11-19 06:49:17.000000 nebulae-0.6.6/nebulae/astro/hangar/GAN/architect.py
--rw-r--r--   0 root         (0) staff       (20)     1838 2021-02-09 08:51:42.000000 nebulae-0.6.6/nebulae/astro/hangar/GAN/biggan.py
--rw-r--r--   0 root         (0) staff       (20)     1378 2022-10-26 12:57:19.000000 nebulae-0.6.6/nebulae/astro/hangar/GAN/dcgan.py
--rw-r--r--   0 root         (0) staff       (20)     1914 2022-11-19 03:39:59.000000 nebulae-0.6.6/nebulae/astro/hangar/GAN/wgan_div.py
--rw-r--r--   0 root         (0) staff       (20)     1384 2020-11-18 08:16:31.000000 nebulae-0.6.6/nebulae/astro/hangar/GAN/fcgan.py
--rw-r--r--   0 root         (0) staff       (20)     1912 2022-11-19 07:00:35.000000 nebulae-0.6.6/nebulae/astro/hangar/GAN/resgan.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-29 14:57:00.000000 nebulae-0.6.6/nebulae/astro/hangar/Classic/
--rw-r--r--   0 root         (0) staff       (20)     3916 2022-08-20 12:56:43.000000 nebulae-0.6.6/nebulae/astro/hangar/Classic/vgg.py
--rw-r--r--   0 root         (0) staff       (20)      667 2020-11-18 05:38:37.000000 nebulae-0.6.6/nebulae/astro/hangar/Classic/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     4998 2022-11-03 08:01:22.000000 nebulae-0.6.6/nebulae/astro/hangar/Classic/resnet.py
--rw-r--r--   0 root         (0) staff       (20)     1267 2023-02-22 11:57:27.000000 nebulae-0.6.6/nebulae/astro/hangar/__init__.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-29 14:57:00.000000 nebulae-0.6.6/nebulae/astro/hangar/Seq2Seq/
--rw-r--r--   0 root         (0) staff       (20)      667 2021-05-22 03:22:45.000000 nebulae-0.6.6/nebulae/astro/hangar/Seq2Seq/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     6860 2021-06-28 07:36:00.000000 nebulae-0.6.6/nebulae/astro/hangar/Seq2Seq/architect.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-29 14:57:00.000000 nebulae-0.6.6/nebulae/astro/hangar/VAE/
--rw-r--r--   0 root         (0) staff       (20)     1077 2023-01-27 08:47:47.000000 nebulae-0.6.6/nebulae/astro/hangar/VAE/resvae.py
--rw-r--r--   0 root         (0) staff       (20)      666 2022-11-03 11:54:33.000000 nebulae-0.6.6/nebulae/astro/hangar/VAE/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     1091 2022-11-08 12:17:50.000000 nebulae-0.6.6/nebulae/astro/hangar/VAE/dcvae.py
--rw-r--r--   0 root         (0) staff       (20)    21531 2023-02-23 04:46:05.000000 nebulae-0.6.6/nebulae/astro/hangar/VAE/architect.py
--rw-r--r--   0 root         (0) staff       (20)     1813 2023-04-29 14:48:07.000000 nebulae-0.6.6/nebulae/astro/hangar/VAE/vqvae.py
--rw-r--r--   0 root         (0) staff       (20)     1070 2022-11-08 12:17:50.000000 nebulae-0.6.6/nebulae/astro/hangar/VAE/vae.py
--rw-r--r--   0 root         (0) staff       (20)    16636 2023-04-29 14:57:00.000000 nebulae-0.6.6/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)     1073 2018-11-04 13:15:50.000000 nebulae-0.6.6/LICENSE
--rw-r--r--   0 root         (0) staff       (20)    15430 2023-04-29 14:56:45.000000 nebulae-0.6.6/setup.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-04-29 14:57:00.000000 nebulae-0.6.6/nebulae.egg-info/
--rw-r--r--   0 root         (0) staff       (20)    16636 2023-04-29 14:57:00.000000 nebulae-0.6.6/nebulae.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)     1474 2023-04-29 14:57:00.000000 nebulae-0.6.6/nebulae.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) staff       (20)      114 2023-04-29 14:57:00.000000 nebulae-0.6.6/nebulae.egg-info/requires.txt
--rw-r--r--   0 root         (0) staff       (20)        8 2023-04-29 14:57:00.000000 nebulae-0.6.6/nebulae.egg-info/top_level.txt
--rw-r--r--   0 root         (0) staff       (20)        1 2023-04-29 14:57:00.000000 nebulae-0.6.6/nebulae.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) staff       (20)       38 2023-04-29 14:57:00.000000 nebulae-0.6.6/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 18:13:54.452844 nebulae-0.6.7/
+-rw-r--r--   0 root         (0) root         (0)    16769 2023-05-04 18:13:54.452844 nebulae-0.6.7/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 18:13:54.452844 nebulae-0.6.7/nebulae/
+-rw-r--r--   0 root         (0) root         (0)      862 2023-05-01 06:31:06.000000 nebulae-0.6.7/nebulae/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 18:13:54.452844 nebulae-0.6.7/nebulae/aerolog/
+-rw-r--r--   0 root         (0) root         (0)      733 2023-05-01 06:31:06.000000 nebulae-0.6.7/nebulae/aerolog/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14072 2023-05-03 14:06:07.000000 nebulae-0.6.7/nebulae/aerolog/dashboard.py
+-rw-r--r--   0 root         (0) root         (0)     7911 2023-05-03 19:00:43.000000 nebulae-0.6.7/nebulae/aerolog/inspector.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 18:13:54.452844 nebulae-0.6.7/nebulae/astro/
+-rw-r--r--   0 root         (0) root         (0)      735 2023-05-01 06:31:06.000000 nebulae-0.6.7/nebulae/astro/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    76912 2023-05-04 17:23:15.000000 nebulae-0.6.7/nebulae/astro/craft.py
+-rw-r--r--   0 root         (0) root         (0)     3187 2023-05-01 06:31:06.000000 nebulae-0.6.7/nebulae/astro/dock.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 18:13:54.452844 nebulae-0.6.7/nebulae/astro/hangar/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 18:13:54.452844 nebulae-0.6.7/nebulae/astro/hangar/Classic/
+-rw-r--r--   0 root         (0) root         (0)      667 2023-05-01 06:31:07.000000 nebulae-0.6.7/nebulae/astro/hangar/Classic/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4861 2023-05-02 18:30:06.000000 nebulae-0.6.7/nebulae/astro/hangar/Classic/resnet.py
+-rw-r--r--   0 root         (0) root         (0)     3916 2023-05-01 06:31:07.000000 nebulae-0.6.7/nebulae/astro/hangar/Classic/vgg.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 18:13:54.452844 nebulae-0.6.7/nebulae/astro/hangar/GAN/
+-rw-r--r--   0 root         (0) root         (0)      667 2023-05-01 06:31:06.000000 nebulae-0.6.7/nebulae/astro/hangar/GAN/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    27430 2023-05-01 06:31:06.000000 nebulae-0.6.7/nebulae/astro/hangar/GAN/architect.py
+-rw-r--r--   0 root         (0) root         (0)     1838 2023-05-01 06:31:06.000000 nebulae-0.6.7/nebulae/astro/hangar/GAN/biggan.py
+-rw-r--r--   0 root         (0) root         (0)     1378 2023-05-01 06:31:06.000000 nebulae-0.6.7/nebulae/astro/hangar/GAN/dcgan.py
+-rw-r--r--   0 root         (0) root         (0)     1384 2023-05-01 06:31:07.000000 nebulae-0.6.7/nebulae/astro/hangar/GAN/fcgan.py
+-rw-r--r--   0 root         (0) root         (0)     1330 2023-05-01 06:31:06.000000 nebulae-0.6.7/nebulae/astro/hangar/GAN/gan.py
+-rw-r--r--   0 root         (0) root         (0)     3571 2023-05-01 06:31:06.000000 nebulae-0.6.7/nebulae/astro/hangar/GAN/infogan.py
+-rw-r--r--   0 root         (0) root         (0)     1912 2023-05-01 06:31:07.000000 nebulae-0.6.7/nebulae/astro/hangar/GAN/resgan.py
+-rw-r--r--   0 root         (0) root         (0)     1489 2023-05-01 06:31:06.000000 nebulae-0.6.7/nebulae/astro/hangar/GAN/wgan.py
+-rw-r--r--   0 root         (0) root         (0)     1914 2023-05-01 06:31:06.000000 nebulae-0.6.7/nebulae/astro/hangar/GAN/wgan_div.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 18:13:54.452844 nebulae-0.6.7/nebulae/astro/hangar/Seq2Seq/
+-rw-r--r--   0 root         (0) root         (0)      667 2023-05-01 06:31:07.000000 nebulae-0.6.7/nebulae/astro/hangar/Seq2Seq/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6860 2023-05-01 06:31:07.000000 nebulae-0.6.7/nebulae/astro/hangar/Seq2Seq/architect.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 18:13:54.452844 nebulae-0.6.7/nebulae/astro/hangar/VAE/
+-rw-r--r--   0 root         (0) root         (0)      666 2023-05-01 06:31:07.000000 nebulae-0.6.7/nebulae/astro/hangar/VAE/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21531 2023-05-01 06:31:07.000000 nebulae-0.6.7/nebulae/astro/hangar/VAE/architect.py
+-rw-r--r--   0 root         (0) root         (0)     1091 2023-05-01 06:31:07.000000 nebulae-0.6.7/nebulae/astro/hangar/VAE/dcvae.py
+-rw-r--r--   0 root         (0) root         (0)     1077 2023-05-01 06:31:07.000000 nebulae-0.6.7/nebulae/astro/hangar/VAE/resvae.py
+-rw-r--r--   0 root         (0) root         (0)     1070 2023-05-01 06:31:07.000000 nebulae-0.6.7/nebulae/astro/hangar/VAE/vae.py
+-rw-r--r--   0 root         (0) root         (0)     1813 2023-05-01 06:31:07.000000 nebulae-0.6.7/nebulae/astro/hangar/VAE/vqvae.py
+-rw-r--r--   0 root         (0) root         (0)     1267 2023-05-01 06:31:07.000000 nebulae-0.6.7/nebulae/astro/hangar/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 18:13:54.452844 nebulae-0.6.7/nebulae/cockpit/
+-rw-r--r--   0 root         (0) root         (0)      897 2023-05-02 06:11:46.000000 nebulae-0.6.7/nebulae/cockpit/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4543 2023-05-04 16:44:17.000000 nebulae-0.6.7/nebulae/cockpit/engine.py
+-rw-r--r--   0 root         (0) root         (0)     6137 2023-05-04 01:57:25.000000 nebulae-0.6.7/nebulae/cockpit/multiverse.py
+-rw-r--r--   0 root         (0) root         (0)     3516 2023-05-01 06:31:06.000000 nebulae-0.6.7/nebulae/cockpit/time_machine.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 18:13:54.452844 nebulae-0.6.7/nebulae/fuel/
+-rw-r--r--   0 root         (0) root         (0)     1005 2023-05-01 06:31:06.000000 nebulae-0.6.7/nebulae/fuel/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    37708 2023-05-01 06:31:06.000000 nebulae-0.6.7/nebulae/fuel/comburant.py
+-rw-r--r--   0 root         (0) root         (0)     9783 2023-05-01 06:31:06.000000 nebulae-0.6.7/nebulae/fuel/generator.py
+-rw-r--r--   0 root         (0) root         (0)     8160 2023-05-03 13:55:26.000000 nebulae-0.6.7/nebulae/fuel/tank.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 18:13:54.452844 nebulae-0.6.7/nebulae/kit/
+-rw-r--r--   0 root         (0) root         (0)     1096 2023-05-01 06:31:06.000000 nebulae-0.6.7/nebulae/kit/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1362 2023-05-01 06:31:06.000000 nebulae-0.6.7/nebulae/kit/decorator.py
+-rw-r--r--   0 root         (0) root         (0)    25772 2023-05-01 06:31:06.000000 nebulae-0.6.7/nebulae/kit/utility.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 18:13:54.452844 nebulae-0.6.7/nebulae/law/
+-rw-r--r--   0 root         (0) root         (0)      698 2023-05-01 06:31:06.000000 nebulae-0.6.7/nebulae/law/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      928 2023-05-01 06:31:06.000000 nebulae-0.6.7/nebulae/law/constant.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 18:13:54.452844 nebulae-0.6.7/nebulae.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    16769 2023-05-04 18:13:54.000000 nebulae-0.6.7/nebulae.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1466 2023-05-04 18:13:54.000000 nebulae-0.6.7/nebulae.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-04 18:13:54.000000 nebulae-0.6.7/nebulae.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      114 2023-05-04 18:13:54.000000 nebulae-0.6.7/nebulae.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-04 18:13:54.000000 nebulae-0.6.7/nebulae.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-04 18:13:54.452844 nebulae-0.6.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)    15711 2023-05-04 17:27:36.000000 nebulae-0.6.7/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `nebulae-0.6.6/nebulae/fuel/__init__.py` & `nebulae-0.6.7/nebulae/fuel/__init__.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.6/nebulae/fuel/generator.py` & `nebulae-0.6.7/nebulae/fuel/generator.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.6/nebulae/fuel/comburant.py` & `nebulae-0.6.7/nebulae/fuel/comburant.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.6/nebulae/fuel/tank.py` & `nebulae-0.6.7/nebulae/fuel/tank.py`

 * *Files 4% similar despite different names*

```diff
@@ -100,14 +100,15 @@
             else:
                 self._chip = engine.chip[self.rank]
             self._coater = engine.coat
         else:
             self._chip = None
         self._tanks = {}
         self._batch_size = {}
+        self._sampler = {} # only store tanks with shuffling
         self.MPE = {}
 
     def mount(self, tank, batch_size, shuffle=True, in_same_size=True, nworker=-1, prefetch=0, transmit=False):
         # >| get unique id
         tid = '0t' + hex(id(tank))[2:]
         # >| check argument validity
         if tid in self._tanks.keys():
@@ -135,66 +136,74 @@
         else:
             self.MPE[tid] = ceil(len(tank) / (batch_size * self.nworld))
         nworker = cpu_count() if nworker <= 0 else nworker - 1
         if self.rank >= 0:
             from torch.utils.data import distributed as dist
             sampler = dist.DistributedSampler(tank)
             if prefetch < 0:
-                loader = DataLoader(tank, batch_size, shuffle, sampler=sampler, collate_fn=tank.collate,
+                loader = DataLoader(tank, batch_size, sampler=sampler, collate_fn=tank.collate,
                                           drop_last=in_same_size, num_workers=nworker)
             else:
-                loader = DataLoader(tank, batch_size, shuffle, sampler=sampler, collate_fn=tank.collate,
+                loader = DataLoader(tank, batch_size, sampler=sampler, collate_fn=tank.collate,
                                     drop_last=in_same_size, num_workers=nworker, prefetch_factor=prefetch)
+            if shuffle:
+                sampler.set_epoch(0)
+                self._sampler[tid] = sampler
         else:
             if prefetch < 0:
                 loader = DataLoader(tank, batch_size, shuffle, collate_fn=tank.collate,
                                           drop_last=in_same_size, num_workers=nworker)
             else:
                 loader = DataLoader(tank, batch_size, shuffle, collate_fn=tank.collate,
                                     drop_last=in_same_size, num_workers=nworker, prefetch_factor=prefetch)
         # >| prefetch if necessary
         if self._transmit: # no matter how many batches to prefetch on GPU is all the same
-            self._tanks[tid] = [tank, loader, loader.__iter__(), 0, cuda.Stream(device=self._chip)]
+            self._tanks[tid] = [tank, loader, loader.__iter__(), 0, 0, cuda.Stream(device=self._chip)]
             self._prefetch(tid)
         else:
-            self._tanks[tid] = [tank, loader, loader.__iter__(), 0]
+            self._tanks[tid] = [tank, loader, loader.__iter__(), 0, 0]
         return tid
 
     def unmount(self, tid):
         assert tid in self._tanks.keys(), 'NEBULAE ERROR ⨷ this tank is not mounted in the depot.'
         self._tanks.pop(tid)
         self._batch_size.pop(tid)
         self.MPE.pop(tid)
+        if tid in self._sampler.keys():
+            self._sampler.pop(tid)
 
     def _prefetch(self, tid):
         self._fetched_data = self._fetch(tid)
-        with cuda.stream(self._tanks[tid][4]):
+        with cuda.stream(self._tanks[tid][-1]):
             # self._fetched_data = self._fetched_data.cuda(device=self.chip, non_blocking=True)
             if isinstance(self._fetched_data, torch.Tensor):
                 self._fetched_data = self._coater(self._fetched_data, sync=False)
             elif isinstance(self._fetched_data, abc.Mapping):
                 self._fetched_data = {key: self._coater(self._fetched_data[key]) for key in self._fetched_data}
             elif isinstance(self._fetched_data, abc.Sequence):
                 self._fetched_data = [self._coater(fd) for fd in self._fetched_data]
             else:
                 raise TypeError('NEBULAE ERROR ⨷ batchified data should be a tensor, sequence or dictionary but is %s'
                                 % type(self._fetched_data))
 
     def _fetch(self, tid):
-        loader, iterator, counter = self._tanks[tid][1:4]
-        if counter == self.MPE[tid]:
+        loader, iterator, mile, epoch = self._tanks[tid][1:5]
+        if mile == self.MPE[tid]:
             iterator = loader.__iter__()
             self._tanks[tid][2:4] = iterator, 1
+            self._tanks[tid][4] += 1
+            if tid in self._sampler.keys():
+                self._sampler[tid].set_epoch(epoch + 1)
         else:
             self._tanks[tid][3] += 1
         return iterator.__next__()
 
     def _next(self, tid):
         if self._transmit:
-            cuda.current_stream().wait_stream(self._tanks[tid][4])
+            cuda.current_stream().wait_stream(self._tanks[tid][-1])
             fetched_data = self._fetched_data
             self._prefetch(tid)
             return fetched_data
         else:
             return self._fetch(tid)
 
     def next(self, tid=None):
```

### Comparing `nebulae-0.6.6/nebulae/law/__init__.py` & `nebulae-0.6.7/nebulae/law/__init__.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.6/nebulae/law/constant.py` & `nebulae-0.6.7/nebulae/law/constant.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.6/nebulae/kit/decorator.py` & `nebulae-0.6.7/nebulae/kit/decorator.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.6/nebulae/kit/utility.py` & `nebulae-0.6.7/nebulae/kit/utility.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.6/nebulae/kit/__init__.py` & `nebulae-0.6.7/nebulae/kit/__init__.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.6/nebulae/__init__.py` & `nebulae-0.6.7/nebulae/__init__.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.6/nebulae/cockpit/time_machine.py` & `nebulae-0.6.7/nebulae/cockpit/time_machine.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.6/nebulae/cockpit/multiverse.py` & `nebulae-0.6.7/nebulae/cockpit/multiverse.py`

 * *Files 22% similar despite different names*

```diff
@@ -20,45 +20,67 @@
          `\--\_    -. ___ .-    _/--/‘
    ===========  \__  NOBUG  __/  ===========
 
 '''
 # -*- coding:utf-8 -*-
 import torch
 import os
-import multiprocessing as mp
+# import multiprocessing as mp
+import torch.multiprocessing as mp
 from ..kit.utility import ver2num
 
 if ver2num(torch.__version__) >= ver2num('1.6.0'):
     is_new_version = True
 else:
     is_new_version = False
 
 if is_new_version:
     class DDP(torch.nn.parallel.DistributedDataParallel):
-        def __init__(self, module, device_ids, output_device):
+        def __init__(self, module, device_ids, output_device, check_unused=False):
             super(DDP, self).__init__(module, device_ids=device_ids, output_device=output_device,
-                                      find_unused_parameters=True)
+                                      find_unused_parameters=check_unused)
 
         def __getattr__(self, name: str):
             if '_parameters' in self.__dict__:
                 _parameters = self.__dict__['_parameters']
                 if name in _parameters:
                     return _parameters[name]
             if '_buffers' in self.__dict__:
                 _buffers = self.__dict__['_buffers']
                 if name in _buffers:
                     return _buffers[name]
             if '_modules' in self.__dict__:
                 modules = self.__dict__['_modules']
                 if name in modules:
                     return modules[name]
-            if hasattr(self, 'module'):
-                if hasattr(self.module, name):
-                    return getattr(self.module, name)
+            
             raise AttributeError("'{}' object has no attribute '{}'".format(type(self).__name__, name))
+
+        def on(self):
+            self.module.on()
+
+        def off(self):
+            self.module.off()
+
+        def update(self):
+            self.module.update()
+
+        def gear(self, gr):
+            self.module = self.module.gear(gr)
+            return self
+
+        def vars(self):
+            return self.module.vars()
+
+        def weights(self):
+            return self.module.weighs()
+
+        @property
+        def fns(self):
+            return self.module.__fns
 else:
     try:
         from apex import parallel
     except ImportError:
         from torch.nn import parallel
         print('NEBULAE WARNING ◘ The PyTorch version is lower than 1.6 which may cause abnormal BNs in distributed manner.')
     class DDP(parallel.DistributedDataParallel):
@@ -94,44 +116,51 @@
 
     def __init__(self, universe, nworld=1):
         self.universe = universe
         self.nworld = nworld
         self.rank = -1
         self.env = os.environ.copy()
         self.env["MASTER_ADDR"] = '127.0.0.1'
-        self.env["MASTER_PORT"] = '29500'
+        self.env["MASTER_PORT"] = '12345'
         self.env["WORLD_SIZE"] = str(nworld)
-        self.env["OMP_NUM_THREADS"] = '1'
+        # self.env["OMP_NUM_THREADS"] = '1'
+
+    def cleanup(self):
+        torch.distributed.destroy_process_group()
 
     def __call__(self, *args, **kwargs):
         # mp.set_start_method('spawn')
         ps = []
         for r in range(self.nworld):
             self.rank = r
             self.env['RANK'] = str(r)
             self.env['LOCAL_RANK'] = str(r)
             p = mp.Process(target=self.universe, args=(self,)+args, kwargs=kwargs)
             p.start()
             ps.append(p)
         for p in ps:
             p.join()
 
-    def init(self):
+        # mp.spawn(self.universe, args=(self,)+args, nprocs=self.nworld)
+
+    def init(self):#, rank):
+        # os.environ['RANK'] = str(rank)
         for k, v in self.env.items():
             os.environ[k] = v
+        rank = int(os.environ['RANK'])
+        torch.distributed.init_process_group(backend="nccl", rank=rank, world_size=self.nworld)
 
     def _sync(self, model):
+        rank = int(os.environ['RANK'])
         scope = model.scope
         if is_new_version:
             model = torch.nn.SyncBatchNorm.convert_sync_batchnorm(model)
-            model = model.to(torch.device('cuda:%d' % self.rank))
-            model = DDP(model, device_ids=[self.rank], output_device=self.rank)
+            model = DDP(model, device_ids=[rank], output_device=rank)
         else:
             model = parallel.convert_syncbn_model(model)
-            model = model.to(torch.device('cuda:%d' % self.rank))
             model = DDP(model, delay_allreduce=True)
 
         model.scope = scope
         return model
 
     def sync(self, models):
         if not isinstance(models, (list, tuple)):
@@ -139,13 +168,22 @@
 
         synced_md = []
         for m in models:
             synced_md.append(self._sync(m))
 
         return tuple(synced_md)
 
-    def reduce(self, tensor, aggregate=False):
+    def _reduce(self, tensor, aggregate=False):
         rt = tensor.clone()
         torch.distributed.all_reduce(rt, op=torch.distributed.ReduceOp.SUM)
         if not aggregate:
             rt /= self.nworld
-        return rt
+        return rt
+
+    def reduce(self, tensors, aggregate=False):
+        if not isinstance(tensors, (list, tuple)):
+            return self._reduce(tensors)
+
+        reduced_ts = []
+        for t in tensors:
+            reduced_ts.append(self._reduce(t))
+        return tuple(reduced_ts)
```

### Comparing `nebulae-0.6.6/nebulae/cockpit/__init__.py` & `nebulae-0.6.7/nebulae/cockpit/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,13 +18,13 @@
          ,--- /   ___\<|>/___   \ ---,
          | |:    \    \ /    /    :| |
          `\--\_    -. ___ .-    _/--/‘
    ===========  \__  NOBUG  __/  ===========
    
 '''
 # -*- coding:utf-8 -*-
-from .engine import Engine, CPU, GPU
+from .engine import Engine, CPU, GPU, DYNAMIC, STATIC, FIXED
 from .time_machine import TimeMachine
 from .multiverse import Multiverse
 
 
-__all__ = ('Engine', 'TimeMachine', 'Multiverse', 'CPU', 'GPU')
+__all__ = ('Engine', 'TimeMachine', 'Multiverse', 'CPU', 'GPU', 'DYNAMIC', 'STATIC', 'FIXED')
```

### Comparing `nebulae-0.6.6/nebulae/cockpit/engine.py` & `nebulae-0.6.7/nebulae/cockpit/engine.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,33 +20,41 @@
          `\--\_    -. ___ .-    _/--/‘
    ===========  \__  NOBUG  __/  ===========
    
 '''
 # -*- coding:utf-8 -*-
 import os
 import torch
-from ..kit.utility import GPUtil
+from ..kit.utility import GPUtil, ver2num
 
 CPU = 0
 GPU = 1
 
+DYNAMIC = 20
+STATIC = 21
+FIXED = 22
+
 
 class Engine(object):
     '''
     Param:
     device: CPU or GPU
     available_gpus
     gpu_mem_fraction
     if_conserve
     least_mem
     '''
-    def __init__(self, device=GPU, ngpu=1, least_mem=2048, avail_gpus=(), multi_piston=False):
+    def __init__(self, device=GPU, ngpu=1, least_mem=2048, avail_gpus=(), multi_piston=False, gearbox=DYNAMIC):
         self.rank = int(os.environ.get('RANK', -1))
         self.device = device
         self.multi_piston = multi_piston
+        if gearbox in (STATIC, FIXED) and ver2num(torch.__version__) < ver2num('2.0'):
+            print('NEBULAE WARNING ◘ The PyTorch version is lower than 2.0, hence the gearbox will be DYNAMIC as default.')
+            gearbox = DYNAMIC
+        self.gearbox = gearbox
         # look for available gpu devices
         if self.device == GPU:
             if len(avail_gpus) == 0:
                 gputil = GPUtil()
                 gpus = gputil.available(ngpu, least_mem)
             else:
                 gpus = avail_gpus
@@ -57,26 +65,26 @@
             # set environment variable
             os.environ['CUDA_VISIBLE_DEVICES'] = str_gpus
             self.chip = [torch.device('cuda:%d'%i) for i in range(ngpu)]
             # setup multi-gpu environment
             if self.rank>=0:
                 torch.backends.cudnn.benchmark = True
                 torch.cuda.set_device(self.rank)
-                torch.distributed.init_process_group(backend='nccl', init_method='env://')
             if self.rank<=0:
                 print('+' + 20 * '-' + '+')
                 print('| Reside in Devices: |')
                 print('+' + 70 * '-' + '+')
                 for g in gpus:
                     print('| \033[1;36mGPU {:<2d}\033[0m | {:<25s} | {:>5d} MiB free out of {:<5d} MiB |'.format(
                         g[0], g[1], g[3], g[2]
                     ))
                     print('+' + 70 * '-' + '+')
         elif self.device == CPU:
             assert self.rank<0
+            self.chip = [torch.device('cpu')]
             print('+' + (24 * '-') + '+')
             print('| Reside in Devices: \033[1;36mCPU\033[0m |')
             print('+' + (24 * '-') + '+')
         else:
             raise KeyError('NEBULAE ERROR ⨷ given device should be either cpu or gpu.')
 
         ###################################
```

### Comparing `nebulae-0.6.6/nebulae/aerolog/inspector.py` & `nebulae-0.6.7/nebulae/aerolog/inspector.py`

 * *Files 15% similar despite different names*

```diff
@@ -19,21 +19,27 @@
          | |:    \    \ /    /    :| |
          `\--\_    -. ___ .-    _/--/‘
    ===========  \__  NOBUG  __/  ===========
    
 '''
 # -*- coding:utf-8 -*-
 from ..astro import fn
+from ..kit import ver2num
+from ..astro.craft import DP
+from ..cockpit.multiverse import DDP
+
 from graphviz import Digraph
 import os
+import sys
 import torch
+from ptflops.pytorch_engine import add_flops_counting_methods
 
 class Inspector(object):
 
-    def __init__(self, export_path='./viz', verbose=True, hidden=(), onnx_ver=9):
+    def __init__(self, export_path='./craft', verbose=True, hidden=(), onnx_ver=-1):
         self.export_path = export_path
         self.verbose = verbose
         self.hidden = hidden
         self.onnx_ver = onnx_ver
         self.layout = Digraph(comment='The Space Craft', format='jpg')
         self.layout.attr('node', shape='doublecircle')
         self.seen = []
@@ -41,18 +47,23 @@
         self.shapes = {}
 
     def paint(self, archit, *dummy_args, **dummy_kwargs):
         rank = int(os.environ.get('RANK', -1))
         if rank > 0:
             return
 
+        if isinstance(archit, (DP, DDP)):
+            archit = archit.module
+        if ver2num(torch.__version__) >= ver2num('2.0') and isinstance(archit, torch._dynamo.OptimizedModule):
+            self.archit = archit._orig_mod
+        else:
+            self.archit = archit
         _ = archit(*dummy_args, **dummy_kwargs)
-        self.archit = archit
         print('+' + 77 * '-' + '+')
-        for f in archit.fns:
+        for f in self.archit.fns:
             self._parse(f)
         self.layout.render(self.export_path, view=False, format='png')
         os.remove(self.export_path)
 
     def _parse(self, f):
         sym = f.symbol
         comp = f.comp
@@ -112,44 +123,71 @@
                         self.seen.append(pivot.name)
                     if pivot.name not in self.displayed:
                         self.displayed.append(pivot.name)
                     for node in nodes:
                         self.layout.edge(node.name, pivot.name, label=self.shapes[node.name])
                     return pivot
 
-    def dissect(self, *dummy_args, **dummy_kwargs):
+    def _get_flops(self, archit, *dummy_args, **dummy_kwargs):
+        flops_model = add_flops_counting_methods(archit)
+        flops_model.eval()
+        flops_model.start_flops_count(ost=sys.stdout, verbose=False, ignore_list=[])
+
+        _ = flops_model(*dummy_args, **dummy_kwargs)
+
+        flops_count, params_count = flops_model.compute_average_flops_cost()
+        flops_model.stop_flops_count()
+
+        return flops_count
+
+    def dissect(self, archit, *dummy_args, **dummy_kwargs):
         rank = int(os.environ.get('RANK', -1))
         if rank > 0:
             return
-        # TODO: draw architectures
+        
+        if isinstance(archit, (DP, DDP)):
+            archit = archit.module
+        if ver2num(torch.__version__) >= ver2num('2.0') and isinstance(archit, torch._dynamo.OptimizedModule):
+            archit = archit._orig_mod
 
         nbytes = {torch.int8: 1, torch.int64: 8, torch.float16: 2, torch.float32: 4, torch.float64: 8}
-        parambytes = sum([p.numel() * nbytes[p.dtype] for p in self.vars()])
+        parambytes = sum([p.numel() for p in archit.vars()])
         if parambytes<1024:
-            parambytes = '%6d B  ' % parambytes
+            parambytes = '%6d  ' % parambytes
         elif parambytes<1048576:
-            parambytes = '%6.2f KB ' % (parambytes / 1024)
+            parambytes = '%6.2f K' % (parambytes / 1024)
         elif parambytes<1073741824:
-            parambytes = '%6.2f MiB' % (parambytes / 1048576)
+            parambytes = '%6.2f M' % (parambytes / 1048576)
+        else:
+            parambytes = '%6.2f B' % (parambytes / 1073741824)
+
+        membytes = sum([p.numel() * nbytes[p.dtype] for p in archit.vars()])
+        if membytes<1024:
+            membytes = '%6d B  ' % membytes
+        elif membytes<1048576:
+            membytes = '%6.2f KB ' % (membytes / 1024)
+        elif membytes<1073741824:
+            membytes = '%6.2f MiB' % (membytes / 1048576)
         else:
-            parambytes = '%6.2f GB ' % (parambytes / 1073741824)
+            membytes = '%6.2f GB ' % (membytes / 1073741824)
 
-        flops = self._get_flops(*dummy_args, **dummy_kwargs)
+        flops = self._get_flops(archit, *dummy_args, **dummy_kwargs)
 
         if flops<1024:
             flops = '%6d  ' % flops
         elif flops<1048576:
             flops = '%6.2f K' % (flops / 1024)
         elif flops<1073741824:
             flops = '%6.2f M' % (flops / 1048576)
         elif flops<1099511627776:
             flops = '%6.2f G' % (flops / 1073741824)
         else:
             flops = '%6.2f T' % (flops / 1099511627776)
-        print('+' + (len(self.scope) + 46) * '-' + '+')
-        print('| Craft-%s weighs \033[1;32m%s\033[0m with \033[1;32m%s\033[0m FLOPS |' % (self.scope, parambytes, flops))
-        print('+' + (len(self.scope) + 46) * '-' + '+')
+        print('+' + (len(archit.scope) + 66) * '-' + '+')
+        print('| Craft-%s weighs \033[1;32m%s\033[0m with \033[1;32m%s\033[0m FLOPS and \033[1;32m%s\033[0m params |' \
+                % (archit.scope, membytes, flops, parambytes))
+        print('+' + (len(archit.scope) + 66) * '-' + '+')
 
         # convert to onnx
-        if self.verbose:
+        if self.onnx_ver > 0:
             dummies = dummy_args + tuple(dummy_kwargs.values())
-            torch.onnx.export(self, dummies, self.export_path, opset_version=self.onnx_ver)
+            torch.onnx.export(archit, dummies, self.export_path+'.onnx', opset_version=self.onnx_ver)
```

### Comparing `nebulae-0.6.6/nebulae/aerolog/__init__.py` & `nebulae-0.6.7/nebulae/aerolog/__init__.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.6/nebulae/aerolog/dashboard.py` & `nebulae-0.6.7/nebulae/aerolog/dashboard.py`

 * *Files 1% similar despite different names*

```diff
@@ -207,15 +207,15 @@
             print('+' + (len(display) - 3 - cnt * 11) * '-' + '+' + 30 * ' ')
             print(display)
             print('+' + (len(display) - 3 - cnt * 11) * '-' + '+' + 30 * ' ')
             self.time = time.time()
 
     def read(self, entry, stage, epoch=-1):
         if self.rank>0:
-            return
+            return 0
         assert epoch!=0, 'NEBULAE ERROR ⨷ epoch starts from 1.'
         epoch = epoch-1 if epoch>0 else epoch
         return self.gauge_epoch[stage + ':' + entry][epoch]
 
     def record(self, entry, stage, value):
         if self.rank>0:
             return
```

### Comparing `nebulae-0.6.6/nebulae/astro/craft.py` & `nebulae-0.6.7/nebulae/astro/craft.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,21 +18,20 @@
          ,--- /   ___\<|>/___   \ ---,
          | |:    \    \ /    /    :| |
          `\--\_    -. ___ .-    _/--/‘
    ===========  \__  NOBUG  __/  ===========
 
 '''
 # -*- coding:utf-8 -*-
+import os
 from math import ceil, sqrt
 from functools import partial
-import sys
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
-from ptflops.pytorch_engine import add_flops_counting_methods
 from ..cockpit.engine import Engine
 from ..cockpit import CPU, GPU
 from ..kit import ver2num
 
 __all__ = ('Rudder', 'Prober', 'Nozzle',
            'NEAREST', 'LINEAR', 'CUBIC', 'AREA',
            'CONSTANT', 'REFLECT', 'REPLICATE',
@@ -64,14 +63,20 @@
              {LINEAR: 'trilinear', AREA: 'area'})
 
 CONSTANT = 10
 REFLECT = 11
 REPLICATE = 12
 PT_PAD = {CONSTANT: 'constant', REFLECT: 'reflect', REPLICATE: 'replicate'}
 
+DYNAMIC = 20
+STATIC = 21
+FIXED = 22
+
+PT_VER = ver2num(torch.__version__)
+
 
 class DP(nn.DataParallel):
     def __init__(self, module):
         super(DP, self).__init__(module)
 
     def __getattr__(self, name: str):
         if '_parameters' in self.__dict__:
@@ -110,14 +115,21 @@
     def gear(self, gr):
         if isinstance(gr, bool):
             if gr:
                 self.train()
             else:
                 self.eval()
         elif isinstance(gr, Engine):
+            if gr.gearbox == STATIC:
+                torch.set_float32_matmul_precision('high')
+                self = torch.compile(self, dynamics=True)
+            elif gr.gearbox == FIXED:
+                torch.set_float32_matmul_precision('high')
+                self = torch.compile(self)
+
             if gr.device == GPU:
                 if gr.rank < 0:
                     if gr.multi_piston:
                         self = DP(self) # [self] is not this object anymore, but we'll receive it outside
                     self.cuda()
                 else:
                     self.to(gr.chip[gr.rank])
@@ -129,26 +141,14 @@
 
     def vars(self):
         return self.parameters()
 
     def weights(self):
         raise Exception('NEBULAE ERROR ⨷ only a few crafts have weights.')
 
-    def _get_flops(self, *dummy_args, **dummy_kwargs):
-        flops_model = add_flops_counting_methods(self)
-        flops_model.eval()
-        flops_model.start_flops_count(ost=sys.stdout, verbose=False, ignore_list=[])
-
-        _ = flops_model(*dummy_args, **dummy_kwargs)
-
-        flops_count, params_count = flops_model.compute_average_flops_cost()
-        flops_model.stop_flops_count()
-
-        return flops_count
-
     def formulate(self, *fns):
         for f in fns:
             self.__fns.append(f)
 
     @property
     def fns(self):
         return self.__fns
@@ -601,77 +601,113 @@
         return x
 
 
 
 # ---------------------------------- Manipulation ------------------------------------ #
 
 class EMA(Craft):
-    def __init__(self, hull, decay_fn=lambda x: 0.9, scope='EMA'):
+    def __init__(self, hull, decay_fn=lambda x: 0.9, on_device=False, scope='EMA'):
         super(EMA, self).__init__(scope)
         self.counter = 0
         self.decay_fn = decay_fn
-        self.hull = hull
+        self.on_device = on_device
+        self._rank = int(os.environ.get('RANK', -1))
+        self['hull'] = hull
         self.swapped = False # whether have swapped to its shadow
 
         # initialize shadow as hull itself
         self.shadow = {}
-        hull_params = self.hull.state_dict()
+        hull_params = hull.state_dict()
+        # note that params have not been to GPU even cuda is enabled
         for k, v in hull_params.items():
-            self.shadow[k] = v.clone().detach()
+            self.shadow[k] = v.clone().detach()           
+    
+    def gear(self, gr):
+        if isinstance(gr, torch.device):
+            self.hull.to(gr)
+            self.hull_dev = gr
+        else:
+            self.hull = self.hull.gear(gr)
+            if isinstance(gr, Engine):
+                self.hull_dev = gr.chip[0] # update only take places on main device
+                if self.on_device:
+                    self.shadow_dev = self.hull_dev
+                else:
+                    self.shadow_dev = torch.device('cpu')
+        for k in self.shadow.keys():
+            self.shadow[k] = self.shadow[k].to(self.shadow_dev)
+        return self
+
+    def vars(self):
+        return self.hull.vars()
+
+    def weights(self):
+        return self.hull.weighs()
+
+    @property
+    def fns(self):
+        return self.hull.__fns
+    
+    def __getattr__(self, name: str): # only be invoked when getattr failed.
+        # EMA is basically a wrapper of model i.e. self.hull,
+        # hence we add the following lines to make sure the
+        # attributes in the model is accessible.
+        hull = self['hull']
+        if name == 'hull':
+            return hull
+        if hasattr(hull, name):
+            return getattr(hull, name)
 
-    def __getattr__(self, name: str):
         if '_parameters' in self.__dict__:
             _parameters = self.__dict__['_parameters']
             if name in _parameters:
                 return _parameters[name]
         if '_buffers' in self.__dict__:
             _buffers = self.__dict__['_buffers']
             if name in _buffers:
                 return _buffers[name]
         if '_modules' in self.__dict__:
             modules = self.__dict__['_modules']
             if name in modules:
                 return modules[name]
-        # EMA is basically a wrapper of model i.e. self.hull,
-        # hence we add the following lines to make sure the
-        # attributes in the model is accessible.
-        if hasattr(self, 'hull'):
-            if hasattr(self.hull, name):
-                return getattr(self.hull, name)
+        
         raise AttributeError("'{}' object has no attribute '{}'".format(type(self).__name__, name))
 
     def _swap(self):
-        with torch.no_grad():
-            hull_params = self.hull.state_dict()
-            for key in self.shadow.keys():
-                # h' = h+s
-                hull_params[key].add_(self.shadow[key])
-                # s' = h'-s = h
-                self.shadow[key].data.copy_(hull_params[key].cpu().data - self.shadow[key].data)
-                # h' = h'-s' = s
-                hull_params[key].sub_(self.shadow[key])
+        if self._rank <= 0:
+            with torch.no_grad():
+                hull_params = self.hull.state_dict()
+                for key in self.shadow.keys():
+                    # h' = h+s
+                    hull_params[key].add_(self.shadow[key].to(self.hull_dev))
+                    # s' = h'-s = h
+                    self.shadow[key].data.copy_(hull_params[key].to(self.shadow_dev).data - self.shadow[key].data)
+                    # h' = h'-s' = s
+                    hull_params[key].sub_(self.shadow[key].to(self.hull_dev))
         self.swapped = not self.swapped
 
     # >| turn on shadow to evalute
     def on(self):
         if not self.swapped:
             self._swap()
 
     # >| turn off shadow for training network weights
     def off(self):
         if self.swapped:
             self._swap()
 
     def update(self):
+        if self._rank > 0:
+            return
         self.counter += 1 # count calling times
         decay = self.decay_fn(self.counter)
         with torch.no_grad():
             hull_params = self.hull.state_dict()
             for key in hull_params.keys():
-                self.shadow[key].data.copy_(hull_params[key].data * (1 - decay) + self.shadow[key].data * decay)
+                self.shadow[key].data.copy_(hull_params[key].to(self.shadow_dev).data * (1 - decay) + self.shadow[key].data * decay)
 
     def run(self, *args, **kwargs):
         return self.hull(*args, **kwargs)
 
 
 
 class Retroact(Craft):
@@ -1220,15 +1256,15 @@
 
 
 
 class SurPix(Craft):
     def __init__(self, scale: tuple, scope='SURPIX'):
         super(SurPix, self).__init__(scope)
         assert len(scale)==2 and scale[0]==scale[1]
-        if ver2num(torch.__version__) < ver2num('1.8.0'):
+        if PT_VER < ver2num('1.8.0'):
             def rearrange(x):
                 S = scale[0]
                 C, H, W = x.shape[-3:]
                 _C = C * S ** 2
                 _H = H // S
                 _W = W // S
                 d = x.dim()
@@ -1702,15 +1738,15 @@
         #   SmoothL1  = l - 1/2                , otherwise
         #   Huber     = l**2 / 2               , when l < delta
         #   Huber     = l*delta - (delta**2)/2 , otherwise
         #|> set l' = l/delta
         #   SmoothL1' = l**2 / (2 * delta**2) = Huber / delta**2 , when l < delta
         #   SmoothL1' = l/delta - 1/2         = Huber / delta**2 , otherwise
         super(Huber, self).__init__(scope)
-        if ver2num(torch.__version__) >= ver2num('1.9.0'):
+        if PT_VER >= ver2num('1.9.0'):
             self._fit_closely = False
             self.cost = nn.HuberLoss(delta=delta)
         else:
             self._fit_closely = True
             self.delta = delta
             self.cost = nn.SmoothL1Loss()
 
@@ -1912,17 +1948,21 @@
 
 
 
 # ------------------------------------ Optimizer ------------------------------------ #
 
 class WarmUpWrapper():
     def __init__(self, warmup, scheduler):
+        if PT_VER >= ver2num('2.0'):
+            scheduler_base = torch.optim.lr_scheduler.LRScheduler
+        else:
+            scheduler_base = torch.optim.lr_scheduler._LRScheduler
         self.warmup = warmup
         self.mile = -1
-        if isinstance(scheduler, torch.optim.lr_scheduler._LRScheduler):
+        if issubclass(type(scheduler), scheduler_base):
             self.scheduler = scheduler
             self.optz = scheduler.optimizer
         else:
             self.scheduler = None
             self.optz = scheduler
         self.lr = self.optz.defaults['lr']
         for group in self.optz.param_groups:
@@ -1990,31 +2030,39 @@
     def __call__(self, optimizer):
         lr_update = lambda x: self.dampen ** (x - 1)
         return torch.optim.lr_scheduler.CyclicLR(optimizer, optimizer.defaults['lr'] / 2, optimizer.defaults['lr'],
                                                  step_size_up=self.period // 2, scale_fn=lr_update, scale_mode='cycle')
 
 
 
+try:
+    from torch._dynamo import OptimizedModule
+    compiled_mod = OptimizedModule
+except ImportError:
+    compiled_mod = str # whatever
+
 class Momentum(Craft):
     def __init__(self, hull, lr, mmnt=0.9, wd=0, lr_decay=None, warmup=0,
                  grad_limit=-1, grad_accum=1, update_scope=None, scope='MOMENTUM'):
         super(Momentum, self).__init__(scope)
+        if PT_VER >= ver2num('2.0') and isinstance(hull, compiled_mod):
+            hull = hull._orig_mod
         # select parameters await updating
         if update_scope is None:
-            update_var = hull.parameters()
+            update_var = hull.vars()
         else:
             if isinstance(update_scope, str):
                 update_scope = [update_scope]
             update_var = []
             for us in update_scope:
                 paths = us.split('/')
                 craft = hull
                 for p in paths:
                     craft = getattr(craft, p)
-                update_var.append(craft.parameters())
+                update_var.append(craft.vars())
 
         self.grad_accum = grad_accum
         self.cnt = 0
         if grad_limit>0:
             nn.utils.clip_grad_value_(update_var, grad_limit)
         self.optz = torch.optim.SGD(update_var, lr=lr, momentum=mmnt, weight_decay=wd)
         if lr_decay is None:
@@ -2038,27 +2086,29 @@
 
 
 
 class Nesterov(Craft):
     def __init__(self, hull, lr, mmnt=0.9, wd=0, lr_decay=None, warmup=0,
                  grad_limit=-1, grad_accum=1, update_scope=None, scope='NESTEROV'):
         super(Nesterov, self).__init__(scope)
+        if PT_VER >= ver2num('2.0') and isinstance(hull, compiled_mod):
+            hull = hull._orig_mod
         # select parameters await updating
         if update_scope is None:
-            update_var = hull.parameters()
+            update_var = hull.vars()
         else:
             if isinstance(update_scope, str):
                 update_scope = [update_scope]
             update_var = []
             for us in update_scope:
                 paths = us.split('/')
                 craft = hull
                 for p in paths:
                     craft = getattr(craft, p)
-                update_var.append(craft.parameters())
+                update_var.append(craft.vars())
 
         self.grad_accum = grad_accum
         self.cnt = 0
         if grad_limit > 0:
             nn.utils.clip_grad_value_(update_var, grad_limit)
         self.optz = torch.optim.SGD(update_var, lr=lr, momentum=mmnt, weight_decay=wd, nesterov=True)
         if lr_decay is None:
@@ -2082,27 +2132,29 @@
 
 
 
 class RMSProp(Craft):
     def __init__(self, hull, lr, mmnt=0., wd=0, lr_decay=None, warmup=0,
                  grad_limit=-1, grad_accum=1, update_scope=None, scope='RMSPROP'):
         super(RMSProp, self).__init__(scope)
+        if PT_VER >= ver2num('2.0') and isinstance(hull, compiled_mod):
+            hull = hull._orig_mod
         # select parameters await updating
         if update_scope is None:
-            update_var = hull.parameters()
+            update_var = hull.vars()
         else:
             if isinstance(update_scope, str):
                 update_scope = [update_scope]
             update_var = []
             for us in update_scope:
                 paths = us.split('/')
                 craft = hull
                 for p in paths:
                     craft = getattr(craft, p)
-                update_var.append(craft.parameters())
+                update_var.append(craft.vars())
 
         self.grad_accum = grad_accum
         self.cnt = 0
         if grad_limit > 0:
             nn.utils.clip_grad_value_(update_var, grad_limit)
         self.optz = torch.optim.RMSprop(update_var, lr=lr, momentum=mmnt, weight_decay=wd)
         if lr_decay is None:
@@ -2126,27 +2178,29 @@
 
 
 
 class Adam(Craft):
     def __init__(self, hull, lr, mmnt1=0.9, mmnt2=0.999, wd=0, lr_decay=None, warmup=0,
                  grad_limit=-1, grad_accum=1, update_scope=None, scope='ADAM'):
         super(Adam, self).__init__(scope)
+        if PT_VER >= ver2num('2.0') and isinstance(hull, compiled_mod):
+            hull = hull._orig_mod
         # select parameters await updating
         if update_scope is None:
-            update_var = hull.parameters()
+            update_var = hull.vars()
         else:
             if isinstance(update_scope, str):
                 update_scope = [update_scope]
             update_var = []
             for us in update_scope:
                 paths = us.split('/')
                 craft = hull
                 for p in paths:
                     craft = getattr(craft, p)
-                update_var.append(craft.parameters())
+                update_var.append(craft.vars())
 
         self.grad_accum = grad_accum
         self.cnt = 0
         if grad_limit > 0:
             nn.utils.clip_grad_value_(update_var, grad_limit)
         self.optz = torch.optim.Adam(update_var, lr=lr, betas=(mmnt1, mmnt2), weight_decay=wd)
         if lr_decay is None:
@@ -2169,27 +2223,29 @@
                 self.lr_decay.step()
 
 
 class AdamW(Craft):
     def __init__(self, hull, lr, mmnt1=0.9, mmnt2=0.999, wd=0, lr_decay=None, warmup=0,
                  grad_limit=-1, grad_accum=1, update_scope=None, scope='ADAMW'):
         super(AdamW, self).__init__(scope)
+        if PT_VER >= ver2num('2.0') and isinstance(hull, compiled_mod):
+            hull = hull._orig_mod
         # select parameters await updating
         if update_scope is None:
-            update_var = hull.parameters()
+            update_var = hull.vars()
         else:
             if isinstance(update_scope, str):
                 update_scope = [update_scope]
             update_var = []
             for us in update_scope:
                 paths = us.split('/')
                 craft = hull
                 for p in paths:
                     craft = getattr(craft, p)
-                update_var.append(craft.parameters())
+                update_var.append(craft.vars())
 
         self.grad_accum = grad_accum
         self.cnt = 0
         if grad_limit > 0:
             nn.utils.clip_grad_value_(update_var, grad_limit)
         self.optz = torch.optim.AdamW(update_var, lr=lr, betas=(mmnt1, mmnt2), weight_decay=wd)
         if lr_decay is None:
@@ -2275,27 +2331,29 @@
 
 
 
 class Lion(Craft):
     def __init__(self, hull, lr, mmnt1=0.9, mmnt2=0.99, wd=0, lr_decay=None, warmup=0,
                  grad_limit=-1, grad_accum=1, update_scope=None, scope='LION'):
         super(Lion, self).__init__(scope)
+        if PT_VER >= ver2num('2.0') and isinstance(hull, compiled_mod):
+            hull = hull._orig_mod
         # select parameters await updating
         if update_scope is None:
-            update_var = hull.parameters()
+            update_var = hull.vars()
         else:
             if isinstance(update_scope, str):
                 update_scope = [update_scope]
             update_var = []
             for us in update_scope:
                 paths = us.split('/')
                 craft = hull
                 for p in paths:
                     craft = getattr(craft, p)
-                update_var.append(craft.parameters())
+                update_var.append(craft.vars())
 
         self.grad_accum = grad_accum
         self.cnt = 0
         if grad_limit > 0:
             nn.utils.clip_grad_value_(update_var, grad_limit)
         self.optz = _Lion(update_var, lr=lr, betas=(mmnt1, mmnt2), weight_decay=wd)
         if lr_decay is None:
@@ -2416,27 +2474,29 @@
 
 
 
 class Lamb(Craft):
     def __init__(self, hull, lr, mmnt1=0.9, mmnt2=0.999, wd=0, lr_decay=None, warmup=0,
                  grad_limit=-1, grad_accum=1, update_scope=None, scope='LION'):
         super(Lamb, self).__init__(scope)
+        if PT_VER >= ver2num('2.0') and isinstance(hull, compiled_mod):
+            hull = hull._orig_mod
         # select parameters await updating
         if update_scope is None:
-            update_var = hull.parameters()
+            update_var = hull.vars()
         else:
             if isinstance(update_scope, str):
                 update_scope = [update_scope]
             update_var = []
             for us in update_scope:
                 paths = us.split('/')
                 craft = hull
                 for p in paths:
                     craft = getattr(craft, p)
-                update_var.append(craft.parameters())
+                update_var.append(craft.vars())
 
         self.grad_accum = grad_accum
         self.cnt = 0
         if grad_limit > 0:
             nn.utils.clip_grad_value_(update_var, grad_limit)
         self.optz = _Lamb(update_var, lr=lr, betas=(mmnt1, mmnt2), weight_decay=wd)
         if lr_decay is None:
```

### Comparing `nebulae-0.6.6/nebulae/astro/__init__.py` & `nebulae-0.6.7/nebulae/astro/__init__.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.6/nebulae/astro/dock.py` & `nebulae-0.6.7/nebulae/astro/dock.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.6/nebulae/astro/hangar/GAN/gan.py` & `nebulae-0.6.7/nebulae/astro/hangar/GAN/gan.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.6/nebulae/astro/hangar/GAN/wgan.py` & `nebulae-0.6.7/nebulae/astro/hangar/GAN/wgan.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.6/nebulae/astro/hangar/GAN/infogan.py` & `nebulae-0.6.7/nebulae/astro/hangar/GAN/infogan.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.6/nebulae/astro/hangar/GAN/__init__.py` & `nebulae-0.6.7/nebulae/astro/hangar/Classic/__init__.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.6/nebulae/astro/hangar/GAN/architect.py` & `nebulae-0.6.7/nebulae/astro/hangar/GAN/architect.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.6/nebulae/astro/hangar/GAN/biggan.py` & `nebulae-0.6.7/nebulae/astro/hangar/GAN/biggan.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.6/nebulae/astro/hangar/GAN/dcgan.py` & `nebulae-0.6.7/nebulae/astro/hangar/GAN/dcgan.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.6/nebulae/astro/hangar/GAN/wgan_div.py` & `nebulae-0.6.7/nebulae/astro/hangar/GAN/wgan_div.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.6/nebulae/astro/hangar/GAN/fcgan.py` & `nebulae-0.6.7/nebulae/astro/hangar/GAN/fcgan.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.6/nebulae/astro/hangar/GAN/resgan.py` & `nebulae-0.6.7/nebulae/astro/hangar/GAN/resgan.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.6/nebulae/astro/hangar/Classic/vgg.py` & `nebulae-0.6.7/nebulae/astro/hangar/Classic/vgg.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.6/nebulae/astro/hangar/Classic/__init__.py` & `nebulae-0.6.7/nebulae/astro/hangar/GAN/__init__.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.6/nebulae/astro/hangar/Classic/resnet.py` & `nebulae-0.6.7/nebulae/astro/hangar/Classic/resnet.py`

 * *Files 5% similar despite different names*

```diff
@@ -57,17 +57,17 @@
         y = self.bn_2(y)
         y = self.relu(y)
 
         y = self.conv_3(y)
         y = self.bn_3(y)
 
         if self.dsample:
-            self['identity'] = self.ds_bn(self.ds_conv(x))
+            x = self.ds_bn(self.ds_conv(x))
 
-        y += self['identity']
+        y += x
         y = self.relu(y)
 
         return y
 
 
 class ResBlock(Craft):
     def __init__(self, in_shape, nchs, nblock, stride=1, width_multp=4, scope='RESBLOCK'):
@@ -116,52 +116,53 @@
             ichs *= 4 if i==0 else 2
             nchs *= 2
 
         self.gap = dock.AvgPool((-1, -1))
 
     def run(self, x):
         self['input'] = x
-        y = self.conv_0(self['input'])
+        y = self.conv_0(x)
         y = self.bn_0(y)
         y = self.relu(y)
         y = self.mpool(y)
 
         for i in range(len(self.nblocks)):
             blk = getattr(self, 'layer_%d'%i)
             y = blk(y)
 
-        self['out'] = self.gap(y)
-        return self['out']
+        y = self.gap(y)
+        return y
 
 
 
 class Resnet_V2_50(Craft):
     def __init__(self, in_shape, scope='RESNET_V2_50'):
         super(Resnet_V2_50, self).__init__(scope)
         self.backbone = Resnet_V2(in_shape, [3, 4, 6, 3])
 
     def run(self, x):
-        self['input'] = x
-        self['out'] = self.backbone(self['input'])
-        return self['out']
+        self['in'] = x
+        y = self.backbone(x)
+        self['out'] = y
+        return y
 
 
 class Resnet_V2_101(Craft):
     def __init__(self, in_shape, scope='RESNET_V2_101'):
         super(Resnet_V2_101, self).__init__(scope)
         self.backbone = Resnet_V2(in_shape, [3, 4, 23, 3])
 
     def run(self, x):
         self['input'] = x
-        self['out'] = self.backbone(self['input'])
-        return self['out']
+        y = self.backbone(x)
+        return y
 
 
 class Resnet_V2_152(Craft):
     def __init__(self, in_shape, scope='RESNET_V2_152'):
         super(Resnet_V2_152, self).__init__(scope)
         self.backbone = Resnet_V2(in_shape, [3, 8, 36, 3])
 
     def run(self, x):
         self['input'] = x
-        self['out'] = self.backbone(self['input'])
-        return self['out']
+        y = self.backbone(x)
+        return y
```

### Comparing `nebulae-0.6.6/nebulae/astro/hangar/__init__.py` & `nebulae-0.6.7/nebulae/astro/hangar/__init__.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.6/nebulae/astro/hangar/Seq2Seq/__init__.py` & `nebulae-0.6.7/nebulae/astro/hangar/Seq2Seq/__init__.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.6/nebulae/astro/hangar/Seq2Seq/architect.py` & `nebulae-0.6.7/nebulae/astro/hangar/Seq2Seq/architect.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.6/nebulae/astro/hangar/VAE/resvae.py` & `nebulae-0.6.7/nebulae/astro/hangar/VAE/resvae.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.6/nebulae/astro/hangar/VAE/__init__.py` & `nebulae-0.6.7/nebulae/astro/hangar/VAE/__init__.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.6/nebulae/astro/hangar/VAE/dcvae.py` & `nebulae-0.6.7/nebulae/astro/hangar/VAE/dcvae.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.6/nebulae/astro/hangar/VAE/architect.py` & `nebulae-0.6.7/nebulae/astro/hangar/VAE/architect.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.6/nebulae/astro/hangar/VAE/vqvae.py` & `nebulae-0.6.7/nebulae/astro/hangar/VAE/vqvae.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.6/nebulae/astro/hangar/VAE/vae.py` & `nebulae-0.6.7/nebulae/astro/hangar/VAE/vae.py`

 * *Files identical despite different names*

### Comparing `nebulae-0.6.6/PKG-INFO` & `nebulae-0.6.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: nebulae
-Version: 0.6.6
-Summary: A novel and simple framework based on prevalent DL frameworks and other image processing libs. v0.6.6: add in_loop and last_for args in DashBoard.gauge().
+Version: 0.6.7
+Summary: A novel and simple framework based on prevalent DL frameworks and other image processing libs. v0.6.7: fix bugs of device allocation and attribute getter in EMA; add on_device argument in EMA for faster update with higher memory occupied; add gearbox argument in Engine to apply Module.compile() in PyTorch 2.
 Home-page: https://github.com/
 Author: Seria
 Author-email: zzqsummerai@yeah.net
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 # Nebulae Brochure
 
 **A novel and simple framework based on concurrent mainstream frameworks and other image processing libraries. It is convenient to deploy almost every module independently.**
 
 ------
```

### Comparing `nebulae-0.6.6/setup.py` & `nebulae-0.6.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,19 +26,22 @@
 import setuptools
 
 with open("Nebulae_Brochure.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="nebulae",
-    version="0.6.6",
+    version="0.6.7",
     author="Seria",
     author_email="zzqsummerai@yeah.net",
     description="A novel and simple framework based on prevalent DL frameworks and other image processing libs."
-                + " v0.6.6: add in_loop and last_for args in DashBoard.gauge().",
+                + " v0.6.7: fix bugs of device allocation and attribute getter in EMA;"
+                + " add on_device argument in EMA for faster update with higher memory occupied;"
+                + " add gearbox argument in Engine to apply Module.compile() in PyTorch 2.",
+                # + " v0.6.6: add in_loop and last_for args in DashBoard.gauge().",
                 # + " v0.6.5: remove ControlPanel; add in_loop and last_for args in DashBoard.gauge;"
                 # + " add Lamb optimizer; replace BluePrint module with Inspector.",
                 # + " v0.6.4: DashBoard.log() now plots curves only by metrics;"
                 # + " add Scatter, Gather, Tile, Argmax, Argmin in dock; add Lion and delete AdaBelief in optimizers.",
                 # + " v0.6.3: OHEM loss supports an additional mask as input.",
                 # + " v0.6.2: change plot tools from matplotlib to seaborn;"
                 # + " make Pooling modules compatible with symmetric padding;"
```

### Comparing `nebulae-0.6.6/nebulae.egg-info/PKG-INFO` & `nebulae-0.6.7/nebulae.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: nebulae
-Version: 0.6.6
-Summary: A novel and simple framework based on prevalent DL frameworks and other image processing libs. v0.6.6: add in_loop and last_for args in DashBoard.gauge().
+Version: 0.6.7
+Summary: A novel and simple framework based on prevalent DL frameworks and other image processing libs. v0.6.7: fix bugs of device allocation and attribute getter in EMA; add on_device argument in EMA for faster update with higher memory occupied; add gearbox argument in Engine to apply Module.compile() in PyTorch 2.
 Home-page: https://github.com/
 Author: Seria
 Author-email: zzqsummerai@yeah.net
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 # Nebulae Brochure
 
 **A novel and simple framework based on concurrent mainstream frameworks and other image processing libraries. It is convenient to deploy almost every module independently.**
 
 ------
```

### Comparing `nebulae-0.6.6/nebulae.egg-info/SOURCES.txt` & `nebulae-0.6.7/nebulae.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-LICENSE
 setup.py
 nebulae/__init__.py
 nebulae.egg-info/PKG-INFO
 nebulae.egg-info/SOURCES.txt
 nebulae.egg-info/dependency_links.txt
 nebulae.egg-info/requires.txt
 nebulae.egg-info/top_level.txt
```

