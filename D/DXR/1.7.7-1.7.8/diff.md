# Comparing `tmp/DXR-1.7.7.tar.gz` & `tmp/DXR-1.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DXR-1.7.7.tar", last modified: Tue Apr 25 10:47:03 2023, max compression
+gzip compressed data, was "DXR-1.7.8.tar", last modified: Thu May  4 13:48:19 2023, max compression
```

## Comparing `DXR-1.7.7.tar` & `DXR-1.7.8.tar`

### file list

```diff
@@ -1,78 +1,80 @@
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-25 10:47:03.497001 DXR-1.7.7/
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-25 10:47:03.409408 DXR-1.7.7/DXR.egg-info/
--rw-r--r--   0 luzhipeng   (501) staff       (20)      181 2023-04-25 10:47:03.000000 DXR-1.7.7/DXR.egg-info/PKG-INFO
--rw-r--r--   0 luzhipeng   (501) staff       (20)     1381 2023-04-25 10:47:03.000000 DXR-1.7.7/DXR.egg-info/SOURCES.txt
--rw-r--r--   0 luzhipeng   (501) staff       (20)        1 2023-04-25 10:47:03.000000 DXR-1.7.7/DXR.egg-info/dependency_links.txt
--rw-r--r--   0 luzhipeng   (501) staff       (20)       40 2023-04-25 10:47:03.000000 DXR-1.7.7/DXR.egg-info/entry_points.txt
--rw-r--r--   0 luzhipeng   (501) staff       (20)      102 2023-04-25 10:47:03.000000 DXR-1.7.7/DXR.egg-info/requires.txt
--rw-r--r--   0 luzhipeng   (501) staff       (20)      122 2023-04-25 10:47:03.000000 DXR-1.7.7/DXR.egg-info/top_level.txt
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-25 10:47:03.411276 DXR-1.7.7/Dxr_Chat/
--rw-r--r--   0 luzhipeng   (501) staff       (20)     7731 2023-04-06 00:37:09.000000 DXR-1.7.7/Dxr_Chat/ChatGPT.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2023-04-06 00:28:21.000000 DXR-1.7.7/Dxr_Chat/__init__.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)      854 2023-04-06 00:28:21.000000 DXR-1.7.7/Dxr_Chat/utils.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-25 10:47:03.413560 DXR-1.7.7/Dxr_bytes/
--rw-r--r--   0 luzhipeng   (501) staff       (20)    34564 2023-01-30 07:47:41.000000 DXR-1.7.7/Dxr_bytes/Dxr_bytes.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)       23 2022-11-20 06:11:57.000000 DXR-1.7.7/Dxr_bytes/__init__.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-25 10:47:03.422153 DXR-1.7.7/Dxr_file/
--rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2023-02-24 03:25:36.000000 DXR-1.7.7/Dxr_file/__init__.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     6042 2023-02-24 03:25:36.000000 DXR-1.7.7/Dxr_file/dxr_file.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     3364 2023-04-24 05:32:08.000000 DXR-1.7.7/Dxr_file/dxr_request.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     2524 2023-04-24 05:49:44.000000 DXR-1.7.7/Dxr_file/dxr_request_ros.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     3427 2023-04-24 05:40:55.000000 DXR-1.7.7/Dxr_file/dxr_requests.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)    20653 2023-02-24 03:25:36.000000 DXR-1.7.7/Dxr_file/dxr_ssh.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-25 10:47:03.442240 DXR-1.7.7/Dxr_grpc/
--rw-r--r--   0 luzhipeng   (501) staff       (20)     4642 2022-12-05 09:42:10.000000 DXR-1.7.7/Dxr_grpc/Datas_pb2.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     2228 2022-12-05 09:45:42.000000 DXR-1.7.7/Dxr_grpc/Datas_pb2_grpc.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     1203 2023-02-15 14:06:08.000000 DXR-1.7.7/Dxr_grpc/audios_pb2.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     2263 2023-02-15 14:14:37.000000 DXR-1.7.7/Dxr_grpc/audios_pb2_grpc.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     2252 2023-02-16 00:43:10.000000 DXR-1.7.7/Dxr_grpc/dxr_grpc_audio_client.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     1141 2023-02-15 14:14:56.000000 DXR-1.7.7/Dxr_grpc/dxr_grpc_audio_server.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     2906 2022-12-05 11:09:41.000000 DXR-1.7.7/Dxr_grpc/dxr_grpc_client.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     1546 2022-12-13 11:26:26.000000 DXR-1.7.7/Dxr_grpc/dxr_grpc_server.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-25 10:47:03.450584 DXR-1.7.7/Dxr_isapi/
--rw-r--r--   0 luzhipeng   (501) staff       (20)      153 2022-12-13 11:34:34.000000 DXR-1.7.7/Dxr_isapi/__init__.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)    29134 2023-04-25 05:13:27.000000 DXR-1.7.7/Dxr_isapi/api.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)      371 2022-12-13 11:34:40.000000 DXR-1.7.7/Dxr_isapi/constants.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     1369 2022-12-13 11:34:43.000000 DXR-1.7.7/Dxr_isapi/error.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     8850 2023-03-13 07:52:33.000000 DXR-1.7.7/Dxr_isapi/ir_client.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-25 10:47:03.454039 DXR-1.7.7/Dxr_log/
--rw-r--r--   0 luzhipeng   (501) staff       (20)       23 2022-11-20 06:11:57.000000 DXR-1.7.7/Dxr_log/__init__.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     3832 2022-11-20 06:11:57.000000 DXR-1.7.7/Dxr_log/log.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-25 10:47:03.461112 DXR-1.7.7/Dxr_mqtt/
--rw-r--r--   0 luzhipeng   (501) staff       (20)       54 2022-11-20 06:11:57.000000 DXR-1.7.7/Dxr_mqtt/__init__.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)       78 2022-11-20 06:11:57.000000 DXR-1.7.7/Dxr_mqtt/dxr_log.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)    14253 2023-04-14 07:14:34.000000 DXR-1.7.7/Dxr_mqtt/dxr_mqtt.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     3433 2022-11-20 06:11:57.000000 DXR-1.7.7/Dxr_mqtt/dxr_mqtt_2.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)    64134 2023-03-08 06:10:00.000000 DXR-1.7.7/Dxr_mqtt/msg.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-25 10:47:03.465935 DXR-1.7.7/Dxr_serial/
--rw-r--r--   0 luzhipeng   (501) staff       (20)     6754 2023-01-30 07:47:41.000000 DXR-1.7.7/Dxr_serial/Dxr_serial.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2022-11-20 06:11:57.000000 DXR-1.7.7/Dxr_serial/__init__.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-25 10:47:03.471959 DXR-1.7.7/Dxr_utils/
--rw-r--r--   0 luzhipeng   (501) staff       (20)       23 2022-11-20 06:11:57.000000 DXR-1.7.7/Dxr_utils/__init__.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     2033 2022-11-20 06:11:57.000000 DXR-1.7.7/Dxr_utils/dxr_ftp.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     3334 2022-11-20 06:11:57.000000 DXR-1.7.7/Dxr_utils/dxr_utils.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)       58 2022-11-20 06:11:57.000000 DXR-1.7.7/Dxr_utils/gvalues.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-25 10:47:03.488099 DXR-1.7.7/Dxr_video/
--rw-r--r--   0 luzhipeng   (501) staff       (20)     3617 2022-11-20 06:11:57.000000 DXR-1.7.7/Dxr_video/Datas_pb2.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     1456 2022-11-20 06:11:57.000000 DXR-1.7.7/Dxr_video/Datas_pb2_grpc.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)    36887 2022-11-20 06:11:57.000000 DXR-1.7.7/Dxr_video/HCNetSDK.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)      731 2022-11-20 06:11:57.000000 DXR-1.7.7/Dxr_video/PlayCtrl.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)       23 2022-11-20 06:11:57.000000 DXR-1.7.7/Dxr_video/__init__.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)      300 2022-11-20 06:11:57.000000 DXR-1.7.7/Dxr_video/global_values.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     8026 2022-11-20 06:11:57.000000 DXR-1.7.7/Dxr_video/test_main.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     2363 2022-11-20 06:11:57.000000 DXR-1.7.7/Dxr_video/video.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     3861 2022-11-20 06:11:57.000000 DXR-1.7.7/Dxr_video/video_hk.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     4806 2022-11-20 06:11:57.000000 DXR-1.7.7/Dxr_video/video_server.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-25 10:47:03.490619 DXR-1.7.7/Dxr_voice/
--rw-r--r--   0 luzhipeng   (501) staff       (20)     2817 2023-03-19 13:53:10.000000 DXR-1.7.7/Dxr_voice/dxr_tts.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2023-03-19 13:53:09.000000 DXR-1.7.7/Dxr_voice/dxr_whisper.py
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-25 10:47:03.492544 DXR-1.7.7/Dxr_yaml/
--rw-r--r--   0 luzhipeng   (501) staff       (20)     6685 2022-12-27 07:21:21.000000 DXR-1.7.7/Dxr_yaml/Dxr_yaml.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2022-11-20 06:11:57.000000 DXR-1.7.7/Dxr_yaml/__init__.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)      181 2023-04-25 10:47:03.496336 DXR-1.7.7/PKG-INFO
--rw-r--r--   0 luzhipeng   (501) staff       (20)    10733 2022-11-20 06:11:57.000000 DXR-1.7.7/README.md
-drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-04-25 10:47:03.494964 DXR-1.7.7/dxr_cli/
--rw-r--r--   0 luzhipeng   (501) staff       (20)       38 2023-04-24 09:19:18.000000 DXR-1.7.7/dxr_cli/__init__.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)     2794 2023-04-25 10:46:49.000000 DXR-1.7.7/dxr_cli/cli.py
--rw-r--r--   0 luzhipeng   (501) staff       (20)       38 2023-04-25 10:47:03.497494 DXR-1.7.7/setup.cfg
--rw-r--r--   0 luzhipeng   (501) staff       (20)      675 2023-04-25 10:46:56.000000 DXR-1.7.7/setup.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-04 13:48:19.921285 DXR-1.7.8/
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-04 13:48:19.837706 DXR-1.7.8/DXR.egg-info/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      181 2023-05-04 13:48:19.000000 DXR-1.7.8/DXR.egg-info/PKG-INFO
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     1417 2023-05-04 13:48:19.000000 DXR-1.7.8/DXR.egg-info/SOURCES.txt
+-rw-r--r--   0 luzhipeng   (501) staff       (20)        1 2023-05-04 13:48:19.000000 DXR-1.7.8/DXR.egg-info/dependency_links.txt
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       40 2023-05-04 13:48:19.000000 DXR-1.7.8/DXR.egg-info/entry_points.txt
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      102 2023-05-04 13:48:19.000000 DXR-1.7.8/DXR.egg-info/requires.txt
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      122 2023-05-04 13:48:19.000000 DXR-1.7.8/DXR.egg-info/top_level.txt
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-04 13:48:19.839496 DXR-1.7.8/Dxr_Chat/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     7782 2023-05-04 13:36:10.000000 DXR-1.7.8/Dxr_Chat/ChatGPT.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2023-04-06 00:28:21.000000 DXR-1.7.8/Dxr_Chat/__init__.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      854 2023-04-06 00:28:21.000000 DXR-1.7.8/Dxr_Chat/utils.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-04 13:48:19.842003 DXR-1.7.8/Dxr_bytes/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    34564 2023-01-30 07:47:41.000000 DXR-1.7.8/Dxr_bytes/Dxr_bytes.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       23 2022-11-20 06:11:57.000000 DXR-1.7.8/Dxr_bytes/__init__.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-04 13:48:19.851444 DXR-1.7.8/Dxr_file/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2023-02-24 03:25:36.000000 DXR-1.7.8/Dxr_file/__init__.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     6042 2023-02-24 03:25:36.000000 DXR-1.7.8/Dxr_file/dxr_file.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     3364 2023-04-24 05:32:08.000000 DXR-1.7.8/Dxr_file/dxr_request.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     2427 2023-04-28 02:39:04.000000 DXR-1.7.8/Dxr_file/dxr_request_ros.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     3427 2023-04-24 05:40:55.000000 DXR-1.7.8/Dxr_file/dxr_requests.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    20653 2023-02-24 03:25:36.000000 DXR-1.7.8/Dxr_file/dxr_ssh.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-04 13:48:19.861397 DXR-1.7.8/Dxr_grpc/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     4642 2022-12-05 09:42:10.000000 DXR-1.7.8/Dxr_grpc/Datas_pb2.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     2228 2022-12-05 09:45:42.000000 DXR-1.7.8/Dxr_grpc/Datas_pb2_grpc.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     1203 2023-02-15 14:06:08.000000 DXR-1.7.8/Dxr_grpc/audios_pb2.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     2263 2023-02-15 14:14:37.000000 DXR-1.7.8/Dxr_grpc/audios_pb2_grpc.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     2252 2023-02-16 00:43:10.000000 DXR-1.7.8/Dxr_grpc/dxr_grpc_audio_client.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     1141 2023-02-15 14:14:56.000000 DXR-1.7.8/Dxr_grpc/dxr_grpc_audio_server.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     2906 2022-12-05 11:09:41.000000 DXR-1.7.8/Dxr_grpc/dxr_grpc_client.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     1546 2022-12-13 11:26:26.000000 DXR-1.7.8/Dxr_grpc/dxr_grpc_server.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-04 13:48:19.870549 DXR-1.7.8/Dxr_isapi/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      153 2022-12-13 11:34:34.000000 DXR-1.7.8/Dxr_isapi/__init__.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    29134 2023-04-25 05:13:27.000000 DXR-1.7.8/Dxr_isapi/api.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      371 2022-12-13 11:34:40.000000 DXR-1.7.8/Dxr_isapi/constants.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     1369 2022-12-13 11:34:43.000000 DXR-1.7.8/Dxr_isapi/error.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     8850 2023-03-13 07:52:33.000000 DXR-1.7.8/Dxr_isapi/ir_client.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-04 13:48:19.875251 DXR-1.7.8/Dxr_log/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       23 2022-11-20 06:11:57.000000 DXR-1.7.8/Dxr_log/__init__.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     3832 2022-11-20 06:11:57.000000 DXR-1.7.8/Dxr_log/log.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-04 13:48:19.883714 DXR-1.7.8/Dxr_mqtt/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       54 2022-11-20 06:11:57.000000 DXR-1.7.8/Dxr_mqtt/__init__.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       78 2022-11-20 06:11:57.000000 DXR-1.7.8/Dxr_mqtt/dxr_log.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    14253 2023-04-14 07:14:34.000000 DXR-1.7.8/Dxr_mqtt/dxr_mqtt.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     3433 2022-11-20 06:11:57.000000 DXR-1.7.8/Dxr_mqtt/dxr_mqtt_2.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    64134 2023-03-08 06:10:00.000000 DXR-1.7.8/Dxr_mqtt/msg.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-04 13:48:19.888503 DXR-1.7.8/Dxr_serial/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     6754 2023-01-30 07:47:41.000000 DXR-1.7.8/Dxr_serial/Dxr_serial.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2022-11-20 06:11:57.000000 DXR-1.7.8/Dxr_serial/__init__.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-04 13:48:19.894154 DXR-1.7.8/Dxr_utils/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       23 2022-11-20 06:11:57.000000 DXR-1.7.8/Dxr_utils/__init__.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     2033 2022-11-20 06:11:57.000000 DXR-1.7.8/Dxr_utils/dxr_ftp.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     3334 2022-11-20 06:11:57.000000 DXR-1.7.8/Dxr_utils/dxr_utils.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       58 2022-11-20 06:11:57.000000 DXR-1.7.8/Dxr_utils/gvalues.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-04 13:48:19.911445 DXR-1.7.8/Dxr_video/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     3617 2022-11-20 06:11:57.000000 DXR-1.7.8/Dxr_video/Datas_pb2.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     1456 2022-11-20 06:11:57.000000 DXR-1.7.8/Dxr_video/Datas_pb2_grpc.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    36887 2022-11-20 06:11:57.000000 DXR-1.7.8/Dxr_video/HCNetSDK.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      731 2022-11-20 06:11:57.000000 DXR-1.7.8/Dxr_video/PlayCtrl.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       23 2022-11-20 06:11:57.000000 DXR-1.7.8/Dxr_video/__init__.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      300 2022-11-20 06:11:57.000000 DXR-1.7.8/Dxr_video/global_values.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     8026 2022-11-20 06:11:57.000000 DXR-1.7.8/Dxr_video/test_main.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     2363 2022-11-20 06:11:57.000000 DXR-1.7.8/Dxr_video/video.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     3861 2022-11-20 06:11:57.000000 DXR-1.7.8/Dxr_video/video_hk.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     4806 2022-11-20 06:11:57.000000 DXR-1.7.8/Dxr_video/video_server.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-04 13:48:19.913441 DXR-1.7.8/Dxr_voice/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     2817 2023-03-19 13:53:10.000000 DXR-1.7.8/Dxr_voice/dxr_tts.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2023-03-19 13:53:09.000000 DXR-1.7.8/Dxr_voice/dxr_whisper.py
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-04 13:48:19.915329 DXR-1.7.8/Dxr_yaml/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     6685 2022-12-27 07:21:21.000000 DXR-1.7.8/Dxr_yaml/Dxr_yaml.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)        0 2022-11-20 06:11:57.000000 DXR-1.7.8/Dxr_yaml/__init__.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      181 2023-05-04 13:48:19.920660 DXR-1.7.8/PKG-INFO
+-rw-r--r--   0 luzhipeng   (501) staff       (20)    10733 2022-11-20 06:11:57.000000 DXR-1.7.8/README.md
+drwxr-xr-x   0 luzhipeng   (501) staff       (20)        0 2023-05-04 13:48:19.919486 DXR-1.7.8/dxr_cli/
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     7782 2023-05-04 13:36:35.000000 DXR-1.7.8/dxr_cli/ChatGPT.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       38 2023-04-24 09:19:18.000000 DXR-1.7.8/dxr_cli/__init__.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)     3340 2023-05-04 13:44:59.000000 DXR-1.7.8/dxr_cli/cli.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      854 2023-05-04 13:36:41.000000 DXR-1.7.8/dxr_cli/utils.py
+-rw-r--r--   0 luzhipeng   (501) staff       (20)       38 2023-05-04 13:48:19.922106 DXR-1.7.8/setup.cfg
+-rw-r--r--   0 luzhipeng   (501) staff       (20)      675 2023-05-04 13:48:08.000000 DXR-1.7.8/setup.py
```

### Comparing `DXR-1.7.7/DXR.egg-info/SOURCES.txt` & `DXR-1.7.8/DXR.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -53,9 +53,11 @@
 Dxr_video/video.py
 Dxr_video/video_hk.py
 Dxr_video/video_server.py
 Dxr_voice/dxr_tts.py
 Dxr_voice/dxr_whisper.py
 Dxr_yaml/Dxr_yaml.py
 Dxr_yaml/__init__.py
+dxr_cli/ChatGPT.py
 dxr_cli/__init__.py
-dxr_cli/cli.py
+dxr_cli/cli.py
+dxr_cli/utils.py
```

### Comparing `DXR-1.7.7/Dxr_Chat/ChatGPT.py` & `DXR-1.7.8/Dxr_Chat/ChatGPT.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,14 +37,15 @@
         """
         Initialize Chatbot with API key (from https://platform.openai.com/account/api-keys)
         """
         self.engine = engine or ENGINE
         self.session = requests.Session()
         self.api_key = api_key
         openai.api_key = self.api_key
+        openai.api_base = 'https://api.hypere.app'
         self.proxy = proxy
         if self.proxy:
             proxies = {
                 "http": self.proxy,
                 "https": self.proxy,
             }
             self.session.proxies = proxies
```

### Comparing `DXR-1.7.7/Dxr_Chat/utils.py` & `DXR-1.7.8/Dxr_Chat/utils.py`

 * *Files identical despite different names*

### Comparing `DXR-1.7.7/Dxr_bytes/Dxr_bytes.py` & `DXR-1.7.8/Dxr_bytes/Dxr_bytes.py`

 * *Files identical despite different names*

### Comparing `DXR-1.7.7/Dxr_file/dxr_file.py` & `DXR-1.7.8/Dxr_file/dxr_file.py`

 * *Files identical despite different names*

### Comparing `DXR-1.7.7/Dxr_file/dxr_request.py` & `DXR-1.7.8/Dxr_file/dxr_request.py`

 * *Files identical despite different names*

### Comparing `DXR-1.7.7/Dxr_file/dxr_request_ros.py` & `DXR-1.7.8/Dxr_file/dxr_request_ros.py`

 * *Files 18% similar despite different names*

```diff
@@ -37,29 +37,30 @@
                 f.write(chunk)
                 count += len(chunk)
                 # 每下载1M,调用一次callback函数
                 if count / file_size > 0.01:
                     # 调用callback函数
                     if callback:
                         process += count / file_size
-                        threading.Thread(target=callback, args=(round(process * 100, 2), file_name)).start()
+                        # threading.Thread(target=callback, args=(round(process * 100, 2), file_name)).start()
+                        callback(round(process * 100, 2), file_name)
                     count = 0
-        threading.Thread(target=callback, args=(100, file_name)).start()
+        # threading.Thread(target=callback, args=(100, file_name)).start()
+        callback(100, file_name)
                     
     print('下载完成')
     return True
     
 def callback(process, filename):
     # 使用锁来确保线程安全
     with threading.Lock():
         print(process, filename)
     
     
 if __name__ == '__main__':
     remote_path = '/root/nav_ws/src/lidar_localization/Localization/data/latest/finalCloud.pcd'
     local_path = './'
-    ip = '10.10.11.10'
+    ip = '10.10.9.254'
     user_name = 'root'
-    password = '123456'
+    password = '0'
     port = 5000
     res = ssh_download_file(remote_path, local_path, ip, user_name, password, port, callback)
-    threading.Thread(target=ssh_download_file, args=(os.path.join('/root/nav_ws/src/lidar_localization/Localization/data/latest/', ''), local_path, ip, user_name, password, port, callback)).start()
```

### Comparing `DXR-1.7.7/Dxr_file/dxr_requests.py` & `DXR-1.7.8/Dxr_file/dxr_requests.py`

 * *Files identical despite different names*

### Comparing `DXR-1.7.7/Dxr_file/dxr_ssh.py` & `DXR-1.7.8/Dxr_file/dxr_ssh.py`

 * *Files identical despite different names*

### Comparing `DXR-1.7.7/Dxr_grpc/Datas_pb2.py` & `DXR-1.7.8/Dxr_grpc/Datas_pb2.py`

 * *Files identical despite different names*

### Comparing `DXR-1.7.7/Dxr_grpc/Datas_pb2_grpc.py` & `DXR-1.7.8/Dxr_grpc/Datas_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `DXR-1.7.7/Dxr_grpc/audios_pb2.py` & `DXR-1.7.8/Dxr_grpc/audios_pb2.py`

 * *Files identical despite different names*

### Comparing `DXR-1.7.7/Dxr_grpc/audios_pb2_grpc.py` & `DXR-1.7.8/Dxr_grpc/audios_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `DXR-1.7.7/Dxr_grpc/dxr_grpc_audio_client.py` & `DXR-1.7.8/Dxr_grpc/dxr_grpc_audio_client.py`

 * *Files identical despite different names*

### Comparing `DXR-1.7.7/Dxr_grpc/dxr_grpc_audio_server.py` & `DXR-1.7.8/Dxr_grpc/dxr_grpc_audio_server.py`

 * *Files identical despite different names*

### Comparing `DXR-1.7.7/Dxr_grpc/dxr_grpc_client.py` & `DXR-1.7.8/Dxr_grpc/dxr_grpc_client.py`

 * *Files identical despite different names*

### Comparing `DXR-1.7.7/Dxr_grpc/dxr_grpc_server.py` & `DXR-1.7.8/Dxr_grpc/dxr_grpc_server.py`

 * *Files identical despite different names*

### Comparing `DXR-1.7.7/Dxr_isapi/api.py` & `DXR-1.7.8/Dxr_isapi/api.py`

 * *Files identical despite different names*

### Comparing `DXR-1.7.7/Dxr_isapi/error.py` & `DXR-1.7.8/Dxr_isapi/error.py`

 * *Files identical despite different names*

### Comparing `DXR-1.7.7/Dxr_isapi/ir_client.py` & `DXR-1.7.8/Dxr_isapi/ir_client.py`

 * *Files identical despite different names*

### Comparing `DXR-1.7.7/Dxr_log/log.py` & `DXR-1.7.8/Dxr_log/log.py`

 * *Files identical despite different names*

### Comparing `DXR-1.7.7/Dxr_mqtt/dxr_mqtt.py` & `DXR-1.7.8/Dxr_mqtt/dxr_mqtt.py`

 * *Files identical despite different names*

### Comparing `DXR-1.7.7/Dxr_mqtt/dxr_mqtt_2.py` & `DXR-1.7.8/Dxr_mqtt/dxr_mqtt_2.py`

 * *Files identical despite different names*

### Comparing `DXR-1.7.7/Dxr_mqtt/msg.py` & `DXR-1.7.8/Dxr_mqtt/msg.py`

 * *Files identical despite different names*

### Comparing `DXR-1.7.7/Dxr_serial/Dxr_serial.py` & `DXR-1.7.8/Dxr_serial/Dxr_serial.py`

 * *Files identical despite different names*

### Comparing `DXR-1.7.7/Dxr_utils/dxr_ftp.py` & `DXR-1.7.8/Dxr_utils/dxr_ftp.py`

 * *Files identical despite different names*

### Comparing `DXR-1.7.7/Dxr_utils/dxr_utils.py` & `DXR-1.7.8/Dxr_utils/dxr_utils.py`

 * *Files identical despite different names*

### Comparing `DXR-1.7.7/Dxr_video/Datas_pb2.py` & `DXR-1.7.8/Dxr_video/Datas_pb2.py`

 * *Files identical despite different names*

### Comparing `DXR-1.7.7/Dxr_video/Datas_pb2_grpc.py` & `DXR-1.7.8/Dxr_video/Datas_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `DXR-1.7.7/Dxr_video/HCNetSDK.py` & `DXR-1.7.8/Dxr_video/HCNetSDK.py`

 * *Files identical despite different names*

### Comparing `DXR-1.7.7/Dxr_video/PlayCtrl.py` & `DXR-1.7.8/Dxr_video/PlayCtrl.py`

 * *Files identical despite different names*

### Comparing `DXR-1.7.7/Dxr_video/test_main.py` & `DXR-1.7.8/Dxr_video/test_main.py`

 * *Files identical despite different names*

### Comparing `DXR-1.7.7/Dxr_video/video.py` & `DXR-1.7.8/Dxr_video/video.py`

 * *Files identical despite different names*

### Comparing `DXR-1.7.7/Dxr_video/video_hk.py` & `DXR-1.7.8/Dxr_video/video_hk.py`

 * *Files identical despite different names*

### Comparing `DXR-1.7.7/Dxr_video/video_server.py` & `DXR-1.7.8/Dxr_video/video_server.py`

 * *Files identical despite different names*

### Comparing `DXR-1.7.7/Dxr_voice/dxr_tts.py` & `DXR-1.7.8/Dxr_voice/dxr_tts.py`

 * *Files identical despite different names*

### Comparing `DXR-1.7.7/Dxr_yaml/Dxr_yaml.py` & `DXR-1.7.8/Dxr_yaml/Dxr_yaml.py`

 * *Files identical despite different names*

### Comparing `DXR-1.7.7/README.md` & `DXR-1.7.8/README.md`

 * *Files identical despite different names*

### Comparing `DXR-1.7.7/dxr_cli/cli.py` & `DXR-1.7.8/dxr_cli/cli.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 import click
 
 import requests
+from .ChatGPT import Chatbot
+import os
+import sys
+sys.stdin.reconfigure(encoding='utf-8')
 
 @click.command()
 def hello():
     """Say hello"""
     click.echo('Hello, world!')
 
 @click.group()
@@ -88,21 +92,36 @@
             click.echo('Run this script?')
             if click.confirm('Continue?'):
                 os.system(bash_script)
                 break
             step = 2
         
     
+@click.command()
+def chat():
+    """Chat with GPT-3"""
+    api_key = os.environ.get("OPENAI_API_KEY", 'fg-67UDB6GEL04J4WN0UN7HNWHQM76L2IOH6DXXCW3A')
+    bot = Chatbot(api_key)
+    while True:
+        text = input("You: ")
+        if text.strip() == "exit":
+            break
+        response = bot.ask_stream(text)
+        print("ChatGPT: ", end="")
+        for r in response:
+            print(r, end="", flush=True)
+        print()
     
     
    
     
 
 
 def main():
     print("Hello world!")
 
 dxr.add_command(hello)
 dxr.add_command(bash)
+dxr.add_command(chat)
 
 if __name__ == '__main__':
     dxr()
```

### Comparing `DXR-1.7.7/setup.py` & `DXR-1.7.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='DXR',
-    version='1.7.7',
+    version='1.7.8',
     packages=['Dxr_mqtt', 'Dxr_log', 'Dxr_bytes', 'Dxr_utils', 'Dxr_video', 'Dxr_serial', 'Dxr_yaml', 'Dxr_file', 'Dxr_grpc', 'Dxr_isapi', 'Dxr_voice', 'Dxr_Chat', 'dxr_cli'],
     install_requires=['paho-mqtt', 'pyyaml', 'pyserial', 'loguru','tabulate', 'pymysql', 'sqlalchemy', 'oss2', 'imagezmq', 'simplejpeg', 'pexpect', 'aiortsp'],
     author='luzhipeng',
     author_email='402087139@qq.com',
     license='MIT',
     url='http://pycn.me',
     description='DXR is a python library for DXR_mqtt',
```

