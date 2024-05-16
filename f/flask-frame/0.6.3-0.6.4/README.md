# Comparing `tmp/flask_frame-0.6.3.tar.gz` & `tmp/flask_frame-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask_frame-0.6.3.tar", last modified: Sun Apr 21 07:07:39 2024, max compression
+gzip compressed data, was "flask_frame-0.6.4.tar", last modified: Thu May 16 02:34:05 2024, max compression
```

## Comparing `flask_frame-0.6.3.tar` & `flask_frame-0.6.4.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxrwxr-x   0 wuhanchu  (1000) wuhanchu  (1000)        0 2024-04-21 07:07:39.573700 flask_frame-0.6.3/
--rwxrwxrwx   0 wuhanchu  (1000) wuhanchu  (1000)     1066 2022-09-27 05:29:11.000000 flask_frame-0.6.3/LICENSE
--rw-rw-r--   0 wuhanchu  (1000) wuhanchu  (1000)      254 2024-04-21 07:07:39.574700 flask_frame-0.6.3/PKG-INFO
--rwxrwxrwx   0 wuhanchu  (1000) wuhanchu  (1000)       78 2024-04-21 07:07:39.574700 flask_frame-0.6.3/setup.cfg
--rwxrwxrwx   0 wuhanchu  (1000) wuhanchu  (1000)      563 2024-04-21 07:06:32.000000 flask_frame-0.6.3/setup.py
-drwxrwxr-x   0 wuhanchu  (1000) wuhanchu  (1000)        0 2024-04-21 07:07:39.568700 flask_frame-0.6.3/src/
-drwxrwxr-x   0 wuhanchu  (1000) wuhanchu  (1000)        0 2024-04-21 07:07:39.569700 flask_frame-0.6.3/src/flask_frame/
--rwxrwxrwx   0 wuhanchu  (1000) wuhanchu  (1000)        0 2022-11-10 06:57:22.000000 flask_frame-0.6.3/src/flask_frame/__init__.py
-drwxrwxr-x   0 wuhanchu  (1000) wuhanchu  (1000)        0 2024-04-21 07:07:39.570700 flask_frame-0.6.3/src/flask_frame/algorithm/
--rwxrwxrwx   0 wuhanchu  (1000) wuhanchu  (1000)        0 2022-11-10 06:57:22.000000 flask_frame-0.6.3/src/flask_frame/algorithm/__init__.py
--rwxrwxrwx   0 wuhanchu  (1000) wuhanchu  (1000)      699 2024-02-21 08:23:16.000000 flask_frame-0.6.3/src/flask_frame/algorithm/text.py
-drwxrwxr-x   0 wuhanchu  (1000) wuhanchu  (1000)        0 2024-04-21 07:07:39.570700 flask_frame-0.6.3/src/flask_frame/annotation/
--rwxrwxrwx   0 wuhanchu  (1000) wuhanchu  (1000)     1985 2024-02-21 08:23:16.000000 flask_frame-0.6.3/src/flask_frame/annotation/__init__.py
-drwxrwxr-x   0 wuhanchu  (1000) wuhanchu  (1000)        0 2024-04-21 07:07:39.570700 flask_frame-0.6.3/src/flask_frame/api/
--rwxrwxrwx   0 wuhanchu  (1000) wuhanchu  (1000)     1032 2024-02-21 08:23:15.000000 flask_frame-0.6.3/src/flask_frame/api/__init__.py
--rwxrwxrwx   0 wuhanchu  (1000) wuhanchu  (1000)     2197 2024-02-21 08:23:15.000000 flask_frame-0.6.3/src/flask_frame/api/exception.py
--rw-r--r--   0 wuhanchu  (1000) wuhanchu  (1000)     3032 2024-04-21 02:44:58.000000 flask_frame-0.6.3/src/flask_frame/api/request.py
--rwxrwxrwx   0 wuhanchu  (1000) wuhanchu  (1000)     7401 2024-02-21 08:23:15.000000 flask_frame-0.6.3/src/flask_frame/api/response.py
--rwxrwxrwx   0 wuhanchu  (1000) wuhanchu  (1000)     3688 2024-02-21 08:23:15.000000 flask_frame-0.6.3/src/flask_frame/app.py
-drwxrwxr-x   0 wuhanchu  (1000) wuhanchu  (1000)        0 2024-04-21 07:07:39.571700 flask_frame-0.6.3/src/flask_frame/extension/
--rwxrwxrwx   0 wuhanchu  (1000) wuhanchu  (1000)      211 2022-11-10 06:57:22.000000 flask_frame-0.6.3/src/flask_frame/extension/__init__.py
-drwxrwxr-x   0 wuhanchu  (1000) wuhanchu  (1000)        0 2024-04-21 07:07:39.571700 flask_frame-0.6.3/src/flask_frame/extension/api_log/
--rwxrwxrwx   0 wuhanchu  (1000) wuhanchu  (1000)     1591 2024-02-21 08:23:16.000000 flask_frame-0.6.3/src/flask_frame/extension/api_log/__init__.py
--rwxrwxrwx   0 wuhanchu  (1000) wuhanchu  (1000)      232 2022-11-10 06:57:22.000000 flask_frame-0.6.3/src/flask_frame/extension/api_log/model.py
--rwxrwxrwx   0 wuhanchu  (1000) wuhanchu  (1000)     3161 2024-02-21 08:23:15.000000 flask_frame-0.6.3/src/flask_frame/extension/celery.py
-drwxrwxr-x   0 wuhanchu  (1000) wuhanchu  (1000)        0 2024-04-21 07:07:39.571700 flask_frame-0.6.3/src/flask_frame/extension/database/
--rwxrwxrwx   0 wuhanchu  (1000) wuhanchu  (1000)    11406 2024-02-21 08:23:16.000000 flask_frame-0.6.3/src/flask_frame/extension/database/__init__.py
--rwxrwxrwx   0 wuhanchu  (1000) wuhanchu  (1000)      221 2022-11-10 06:57:22.000000 flask_frame-0.6.3/src/flask_frame/extension/database/model.py
--rwxrwxrwx   0 wuhanchu  (1000) wuhanchu  (1000)     2712 2022-11-10 06:57:22.000000 flask_frame-0.6.3/src/flask_frame/extension/lock.py
-drwxrwxr-x   0 wuhanchu  (1000) wuhanchu  (1000)        0 2024-04-21 07:07:39.572700 flask_frame-0.6.3/src/flask_frame/extension/loguru/
--rw-r--r--   0 wuhanchu  (1000) wuhanchu  (1000)     3164 2024-02-28 06:00:38.000000 flask_frame-0.6.3/src/flask_frame/extension/loguru/__init__.py
--rwxrwxrwx   0 wuhanchu  (1000) wuhanchu  (1000)      605 2024-02-21 08:23:15.000000 flask_frame-0.6.3/src/flask_frame/extension/loguru/compress.py
--rwxrwxrwx   0 wuhanchu  (1000) wuhanchu  (1000)      401 2022-11-10 06:57:22.000000 flask_frame-0.6.3/src/flask_frame/extension/loguru/macro.py
--rwxrwxrwx   0 wuhanchu  (1000) wuhanchu  (1000)      125 2022-11-10 06:57:22.000000 flask_frame-0.6.3/src/flask_frame/extension/marshmallow.py
--rwxrwxrwx   0 wuhanchu  (1000) wuhanchu  (1000)      963 2024-02-21 08:23:15.000000 flask_frame-0.6.3/src/flask_frame/extension/participle.py
--rwxrwxrwx   0 wuhanchu  (1000) wuhanchu  (1000)     4454 2024-02-21 08:23:15.000000 flask_frame-0.6.3/src/flask_frame/extension/permission.py
-drwxrwxr-x   0 wuhanchu  (1000) wuhanchu  (1000)        0 2024-04-21 07:07:39.572700 flask_frame-0.6.3/src/flask_frame/extension/postgrest/
--rwxrwxrwx   0 wuhanchu  (1000) wuhanchu  (1000)     4355 2024-02-21 08:23:15.000000 flask_frame-0.6.3/src/flask_frame/extension/postgrest/__init__.py
--rwxrwxrwx   0 wuhanchu  (1000) wuhanchu  (1000)    13826 2024-02-21 08:23:16.000000 flask_frame-0.6.3/src/flask_frame/extension/postgrest/sql_generator.py
--rwxrwxrwx   0 wuhanchu  (1000) wuhanchu  (1000)      191 2024-02-21 08:23:15.000000 flask_frame-0.6.3/src/flask_frame/extension/postgrest/util.py
--rwxrwxrwx   0 wuhanchu  (1000) wuhanchu  (1000)     1564 2024-02-21 08:23:15.000000 flask_frame-0.6.3/src/flask_frame/extension/redis.py
--rwxrwxrwx   0 wuhanchu  (1000) wuhanchu  (1000)     1007 2022-11-10 07:44:33.000000 flask_frame-0.6.3/src/flask_frame/extension/sentry.py
-drwxrwxr-x   0 wuhanchu  (1000) wuhanchu  (1000)        0 2024-04-21 07:07:39.572700 flask_frame-0.6.3/src/flask_frame/file/
--rwxrwxrwx   0 wuhanchu  (1000) wuhanchu  (1000)      978 2024-02-21 08:23:15.000000 flask_frame-0.6.3/src/flask_frame/file/__init__.py
--rwxrwxrwx   0 wuhanchu  (1000) wuhanchu  (1000)     1843 2024-02-21 08:23:15.000000 flask_frame-0.6.3/src/flask_frame/file/audio.py
--rwxrwxrwx   0 wuhanchu  (1000) wuhanchu  (1000)      468 2024-02-21 08:23:15.000000 flask_frame-0.6.3/src/flask_frame/file/video.py
--rwxrwxrwx   0 wuhanchu  (1000) wuhanchu  (1000)     1339 2024-02-21 08:23:15.000000 flask_frame-0.6.3/src/flask_frame/permission_context.py
-drwxrwxr-x   0 wuhanchu  (1000) wuhanchu  (1000)        0 2024-04-21 07:07:39.572700 flask_frame-0.6.3/src/flask_frame/schema/
--rwxrwxrwx   0 wuhanchu  (1000) wuhanchu  (1000)      404 2022-11-10 06:57:22.000000 flask_frame-0.6.3/src/flask_frame/schema/__init__.py
-drwxrwxr-x   0 wuhanchu  (1000) wuhanchu  (1000)        0 2024-04-21 07:07:39.572700 flask_frame-0.6.3/src/flask_frame/thread/
--rwxrwxrwx   0 wuhanchu  (1000) wuhanchu  (1000)        0 2022-11-10 06:57:22.000000 flask_frame-0.6.3/src/flask_frame/thread/__init__.py
--rwxrwxrwx   0 wuhanchu  (1000) wuhanchu  (1000)      612 2022-11-10 06:57:22.000000 flask_frame-0.6.3/src/flask_frame/thread/dk_thread_pool.py
--rwxrwxrwx   0 wuhanchu  (1000) wuhanchu  (1000)     1068 2022-11-10 06:57:22.000000 flask_frame-0.6.3/src/flask_frame/thread/my_synchronized.py
-drwxrwxr-x   0 wuhanchu  (1000) wuhanchu  (1000)        0 2024-04-21 07:07:39.573700 flask_frame-0.6.3/src/flask_frame/util/
--rwxrwxrwx   0 wuhanchu  (1000) wuhanchu  (1000)        0 2022-11-10 06:57:22.000000 flask_frame-0.6.3/src/flask_frame/util/__init__.py
--rwxrwxrwx   0 wuhanchu  (1000) wuhanchu  (1000)     4030 2024-02-21 08:23:15.000000 flask_frame-0.6.3/src/flask_frame/util/algorithm.py
--rwxrwxrwx   0 wuhanchu  (1000) wuhanchu  (1000)     4258 2024-02-21 08:23:15.000000 flask_frame-0.6.3/src/flask_frame/util/com_tool.py
--rwxrwxrwx   0 wuhanchu  (1000) wuhanchu  (1000)      609 2024-02-21 08:23:15.000000 flask_frame-0.6.3/src/flask_frame/util/db.py
--rwxrwxrwx   0 wuhanchu  (1000) wuhanchu  (1000)     1525 2024-02-21 08:23:15.000000 flask_frame-0.6.3/src/flask_frame/util/doc.py
--rwxrwxrwx   0 wuhanchu  (1000) wuhanchu  (1000)      356 2024-02-21 08:23:15.000000 flask_frame-0.6.3/src/flask_frame/util/enum.py
--rwxrwxrwx   0 wuhanchu  (1000) wuhanchu  (1000)      637 2024-02-21 08:23:15.000000 flask_frame-0.6.3/src/flask_frame/util/file.py
--rwxrwxrwx   0 wuhanchu  (1000) wuhanchu  (1000)     1615 2024-02-21 08:23:15.000000 flask_frame-0.6.3/src/flask_frame/util/lock.py
--rwxrwxrwx   0 wuhanchu  (1000) wuhanchu  (1000)      546 2024-02-21 08:23:15.000000 flask_frame-0.6.3/src/flask_frame/util/model.py
--rwxrwxrwx   0 wuhanchu  (1000) wuhanchu  (1000)      725 2024-02-21 08:23:15.000000 flask_frame-0.6.3/src/flask_frame/util/obj.py
--rwxrwxrwx   0 wuhanchu  (1000) wuhanchu  (1000)      646 2022-11-10 06:57:22.000000 flask_frame-0.6.3/src/flask_frame/util/param_tool.py
--rwxrwxrwx   0 wuhanchu  (1000) wuhanchu  (1000)      294 2024-02-21 08:23:15.000000 flask_frame-0.6.3/src/flask_frame/util/py_utils.py
--rwxrwxrwx   0 wuhanchu  (1000) wuhanchu  (1000)     3400 2024-02-21 08:23:15.000000 flask_frame-0.6.3/src/flask_frame/util/rsa_tool.py
--rwxrwxrwx   0 wuhanchu  (1000) wuhanchu  (1000)     1296 2022-11-10 06:57:22.000000 flask_frame-0.6.3/src/flask_frame/util/sql_tool.py
--rwxrwxrwx   0 wuhanchu  (1000) wuhanchu  (1000)    13900 2024-02-21 08:23:15.000000 flask_frame-0.6.3/src/flask_frame/util/text.py
--rwxrwxrwx   0 wuhanchu  (1000) wuhanchu  (1000)       24 2022-11-10 06:57:22.000000 flask_frame-0.6.3/src/flask_frame/util/time.py
--rwxrwxrwx   0 wuhanchu  (1000) wuhanchu  (1000)    12352 2024-02-21 08:23:15.000000 flask_frame-0.6.3/src/flask_frame/util/txt_compare.py
--rwxrwxrwx   0 wuhanchu  (1000) wuhanchu  (1000)    12442 2024-02-21 08:23:15.000000 flask_frame-0.6.3/src/flask_frame/util/wav.py
-drwxrwxr-x   0 wuhanchu  (1000) wuhanchu  (1000)        0 2024-04-21 07:07:39.570700 flask_frame-0.6.3/src/flask_frame.egg-info/
--rwxrwxrwx   0 wuhanchu  (1000) wuhanchu  (1000)      254 2024-04-21 07:07:39.000000 flask_frame-0.6.3/src/flask_frame.egg-info/PKG-INFO
--rwxrwxrwx   0 wuhanchu  (1000) wuhanchu  (1000)     2107 2024-04-21 07:07:39.000000 flask_frame-0.6.3/src/flask_frame.egg-info/SOURCES.txt
--rwxrwxrwx   0 wuhanchu  (1000) wuhanchu  (1000)        1 2024-04-21 07:07:39.000000 flask_frame-0.6.3/src/flask_frame.egg-info/dependency_links.txt
--rwxrwxrwx   0 wuhanchu  (1000) wuhanchu  (1000)      536 2024-04-21 07:07:39.000000 flask_frame-0.6.3/src/flask_frame.egg-info/requires.txt
--rwxrwxrwx   0 wuhanchu  (1000) wuhanchu  (1000)       12 2024-04-21 07:07:39.000000 flask_frame-0.6.3/src/flask_frame.egg-info/top_level.txt
+drwxr-xr-x   0 wuhanchu  (1000) wuhanchu  (1000)        0 2024-05-16 02:34:05.812057 flask_frame-0.6.4/
+-rwxrwxrwx   0 wuhanchu  (1000) wuhanchu  (1000)     1066 2022-09-27 05:29:11.000000 flask_frame-0.6.4/LICENSE
+-rw-r--r--   0 wuhanchu  (1000) wuhanchu  (1000)      254 2024-05-16 02:34:05.812057 flask_frame-0.6.4/PKG-INFO
+-rwxrwxrwx   0 wuhanchu  (1000) wuhanchu  (1000)       78 2024-05-16 02:34:05.812057 flask_frame-0.6.4/setup.cfg
+-rwxrwxrwx   0 wuhanchu  (1000) wuhanchu  (1000)      563 2024-05-16 02:32:36.000000 flask_frame-0.6.4/setup.py
+drwxr-xr-x   0 wuhanchu  (1000) wuhanchu  (1000)        0 2024-05-16 02:34:05.807057 flask_frame-0.6.4/src/
+drwxr-xr-x   0 wuhanchu  (1000) wuhanchu  (1000)        0 2024-05-16 02:34:05.808057 flask_frame-0.6.4/src/flask_frame/
+-rwxrwxrwx   0 wuhanchu  (1000) wuhanchu  (1000)        0 2022-11-10 06:57:22.000000 flask_frame-0.6.4/src/flask_frame/__init__.py
+drwxr-xr-x   0 wuhanchu  (1000) wuhanchu  (1000)        0 2024-05-16 02:34:05.808057 flask_frame-0.6.4/src/flask_frame/algorithm/
+-rwxrwxrwx   0 wuhanchu  (1000) wuhanchu  (1000)        0 2022-11-10 06:57:22.000000 flask_frame-0.6.4/src/flask_frame/algorithm/__init__.py
+-rwxrwxrwx   0 wuhanchu  (1000) wuhanchu  (1000)      699 2024-02-21 08:23:16.000000 flask_frame-0.6.4/src/flask_frame/algorithm/text.py
+drwxr-xr-x   0 wuhanchu  (1000) wuhanchu  (1000)        0 2024-05-16 02:34:05.808057 flask_frame-0.6.4/src/flask_frame/annotation/
+-rwxrwxrwx   0 wuhanchu  (1000) wuhanchu  (1000)     1985 2024-02-21 08:23:16.000000 flask_frame-0.6.4/src/flask_frame/annotation/__init__.py
+drwxr-xr-x   0 wuhanchu  (1000) wuhanchu  (1000)        0 2024-05-16 02:34:05.808057 flask_frame-0.6.4/src/flask_frame/api/
+-rwxrwxrwx   0 wuhanchu  (1000) wuhanchu  (1000)     1032 2024-02-21 08:23:15.000000 flask_frame-0.6.4/src/flask_frame/api/__init__.py
+-rwxrwxrwx   0 wuhanchu  (1000) wuhanchu  (1000)     2197 2024-02-21 08:23:15.000000 flask_frame-0.6.4/src/flask_frame/api/exception.py
+-rw-r--r--   0 wuhanchu  (1000) wuhanchu  (1000)     3032 2024-04-21 02:44:58.000000 flask_frame-0.6.4/src/flask_frame/api/request.py
+-rwxrwxrwx   0 wuhanchu  (1000) wuhanchu  (1000)     7401 2024-02-21 08:23:15.000000 flask_frame-0.6.4/src/flask_frame/api/response.py
+-rwxrwxrwx   0 wuhanchu  (1000) wuhanchu  (1000)     3688 2024-02-21 08:23:15.000000 flask_frame-0.6.4/src/flask_frame/app.py
+drwxr-xr-x   0 wuhanchu  (1000) wuhanchu  (1000)        0 2024-05-16 02:34:05.809057 flask_frame-0.6.4/src/flask_frame/extension/
+-rwxrwxrwx   0 wuhanchu  (1000) wuhanchu  (1000)      211 2022-11-10 06:57:22.000000 flask_frame-0.6.4/src/flask_frame/extension/__init__.py
+drwxr-xr-x   0 wuhanchu  (1000) wuhanchu  (1000)        0 2024-05-16 02:34:05.810057 flask_frame-0.6.4/src/flask_frame/extension/api_log/
+-rwxrwxrwx   0 wuhanchu  (1000) wuhanchu  (1000)     1591 2024-02-21 08:23:16.000000 flask_frame-0.6.4/src/flask_frame/extension/api_log/__init__.py
+-rwxrwxrwx   0 wuhanchu  (1000) wuhanchu  (1000)      232 2022-11-10 06:57:22.000000 flask_frame-0.6.4/src/flask_frame/extension/api_log/model.py
+-rwxrwxrwx   0 wuhanchu  (1000) wuhanchu  (1000)     3161 2024-02-21 08:23:15.000000 flask_frame-0.6.4/src/flask_frame/extension/celery.py
+drwxr-xr-x   0 wuhanchu  (1000) wuhanchu  (1000)        0 2024-05-16 02:34:05.810057 flask_frame-0.6.4/src/flask_frame/extension/database/
+-rwxrwxrwx   0 wuhanchu  (1000) wuhanchu  (1000)    11406 2024-02-21 08:23:16.000000 flask_frame-0.6.4/src/flask_frame/extension/database/__init__.py
+-rwxrwxrwx   0 wuhanchu  (1000) wuhanchu  (1000)      221 2022-11-10 06:57:22.000000 flask_frame-0.6.4/src/flask_frame/extension/database/model.py
+-rwxrwxrwx   0 wuhanchu  (1000) wuhanchu  (1000)     2712 2022-11-10 06:57:22.000000 flask_frame-0.6.4/src/flask_frame/extension/lock.py
+drwxr-xr-x   0 wuhanchu  (1000) wuhanchu  (1000)        0 2024-05-16 02:34:05.810057 flask_frame-0.6.4/src/flask_frame/extension/loguru/
+-rw-r--r--   0 wuhanchu  (1000) wuhanchu  (1000)     3164 2024-02-28 06:00:38.000000 flask_frame-0.6.4/src/flask_frame/extension/loguru/__init__.py
+-rwxrwxrwx   0 wuhanchu  (1000) wuhanchu  (1000)      605 2024-02-21 08:23:15.000000 flask_frame-0.6.4/src/flask_frame/extension/loguru/compress.py
+-rwxrwxrwx   0 wuhanchu  (1000) wuhanchu  (1000)      401 2022-11-10 06:57:22.000000 flask_frame-0.6.4/src/flask_frame/extension/loguru/macro.py
+-rwxrwxrwx   0 wuhanchu  (1000) wuhanchu  (1000)      125 2022-11-10 06:57:22.000000 flask_frame-0.6.4/src/flask_frame/extension/marshmallow.py
+-rwxrwxrwx   0 wuhanchu  (1000) wuhanchu  (1000)      963 2024-02-21 08:23:15.000000 flask_frame-0.6.4/src/flask_frame/extension/participle.py
+-rwxrwxrwx   0 wuhanchu  (1000) wuhanchu  (1000)     4454 2024-02-21 08:23:15.000000 flask_frame-0.6.4/src/flask_frame/extension/permission.py
+drwxr-xr-x   0 wuhanchu  (1000) wuhanchu  (1000)        0 2024-05-16 02:34:05.810057 flask_frame-0.6.4/src/flask_frame/extension/postgrest/
+-rwxrwxrwx   0 wuhanchu  (1000) wuhanchu  (1000)     4355 2024-02-21 08:23:15.000000 flask_frame-0.6.4/src/flask_frame/extension/postgrest/__init__.py
+-rwxrwxrwx   0 wuhanchu  (1000) wuhanchu  (1000)    13826 2024-02-21 08:23:16.000000 flask_frame-0.6.4/src/flask_frame/extension/postgrest/sql_generator.py
+-rwxrwxrwx   0 wuhanchu  (1000) wuhanchu  (1000)      191 2024-02-21 08:23:15.000000 flask_frame-0.6.4/src/flask_frame/extension/postgrest/util.py
+-rwxrwxrwx   0 wuhanchu  (1000) wuhanchu  (1000)     1564 2024-02-21 08:23:15.000000 flask_frame-0.6.4/src/flask_frame/extension/redis.py
+-rwxrwxrwx   0 wuhanchu  (1000) wuhanchu  (1000)     1007 2022-11-10 07:44:33.000000 flask_frame-0.6.4/src/flask_frame/extension/sentry.py
+drwxr-xr-x   0 wuhanchu  (1000) wuhanchu  (1000)        0 2024-05-16 02:34:05.810057 flask_frame-0.6.4/src/flask_frame/file/
+-rwxrwxrwx   0 wuhanchu  (1000) wuhanchu  (1000)      978 2024-02-21 08:23:15.000000 flask_frame-0.6.4/src/flask_frame/file/__init__.py
+-rwxrwxrwx   0 wuhanchu  (1000) wuhanchu  (1000)     1843 2024-02-21 08:23:15.000000 flask_frame-0.6.4/src/flask_frame/file/audio.py
+-rwxrwxrwx   0 wuhanchu  (1000) wuhanchu  (1000)      468 2024-02-21 08:23:15.000000 flask_frame-0.6.4/src/flask_frame/file/video.py
+-rwxrwxrwx   0 wuhanchu  (1000) wuhanchu  (1000)     1339 2024-02-21 08:23:15.000000 flask_frame-0.6.4/src/flask_frame/permission_context.py
+drwxr-xr-x   0 wuhanchu  (1000) wuhanchu  (1000)        0 2024-05-16 02:34:05.810057 flask_frame-0.6.4/src/flask_frame/schema/
+-rwxrwxrwx   0 wuhanchu  (1000) wuhanchu  (1000)      404 2022-11-10 06:57:22.000000 flask_frame-0.6.4/src/flask_frame/schema/__init__.py
+drwxr-xr-x   0 wuhanchu  (1000) wuhanchu  (1000)        0 2024-05-16 02:34:05.810057 flask_frame-0.6.4/src/flask_frame/thread/
+-rwxrwxrwx   0 wuhanchu  (1000) wuhanchu  (1000)        0 2022-11-10 06:57:22.000000 flask_frame-0.6.4/src/flask_frame/thread/__init__.py
+-rwxrwxrwx   0 wuhanchu  (1000) wuhanchu  (1000)      612 2022-11-10 06:57:22.000000 flask_frame-0.6.4/src/flask_frame/thread/dk_thread_pool.py
+-rwxrwxrwx   0 wuhanchu  (1000) wuhanchu  (1000)     1068 2022-11-10 06:57:22.000000 flask_frame-0.6.4/src/flask_frame/thread/my_synchronized.py
+drwxr-xr-x   0 wuhanchu  (1000) wuhanchu  (1000)        0 2024-05-16 02:34:05.812057 flask_frame-0.6.4/src/flask_frame/util/
+-rwxrwxrwx   0 wuhanchu  (1000) wuhanchu  (1000)        0 2022-11-10 06:57:22.000000 flask_frame-0.6.4/src/flask_frame/util/__init__.py
+-rwxrwxrwx   0 wuhanchu  (1000) wuhanchu  (1000)     4030 2024-02-21 08:23:15.000000 flask_frame-0.6.4/src/flask_frame/util/algorithm.py
+-rwxrwxrwx   0 wuhanchu  (1000) wuhanchu  (1000)     4258 2024-02-21 08:23:15.000000 flask_frame-0.6.4/src/flask_frame/util/com_tool.py
+-rwxrwxrwx   0 wuhanchu  (1000) wuhanchu  (1000)      609 2024-02-21 08:23:15.000000 flask_frame-0.6.4/src/flask_frame/util/db.py
+-rwxrwxrwx   0 wuhanchu  (1000) wuhanchu  (1000)     1525 2024-02-21 08:23:15.000000 flask_frame-0.6.4/src/flask_frame/util/doc.py
+-rwxrwxrwx   0 wuhanchu  (1000) wuhanchu  (1000)      356 2024-02-21 08:23:15.000000 flask_frame-0.6.4/src/flask_frame/util/enum.py
+-rwxrwxrwx   0 wuhanchu  (1000) wuhanchu  (1000)      637 2024-02-21 08:23:15.000000 flask_frame-0.6.4/src/flask_frame/util/file.py
+-rwxrwxrwx   0 wuhanchu  (1000) wuhanchu  (1000)     1615 2024-02-21 08:23:15.000000 flask_frame-0.6.4/src/flask_frame/util/lock.py
+-rwxrwxrwx   0 wuhanchu  (1000) wuhanchu  (1000)      546 2024-02-21 08:23:15.000000 flask_frame-0.6.4/src/flask_frame/util/model.py
+-rwxrwxrwx   0 wuhanchu  (1000) wuhanchu  (1000)      725 2024-02-21 08:23:15.000000 flask_frame-0.6.4/src/flask_frame/util/obj.py
+-rwxrwxrwx   0 wuhanchu  (1000) wuhanchu  (1000)      646 2022-11-10 06:57:22.000000 flask_frame-0.6.4/src/flask_frame/util/param_tool.py
+-rwxrwxrwx   0 wuhanchu  (1000) wuhanchu  (1000)      294 2024-02-21 08:23:15.000000 flask_frame-0.6.4/src/flask_frame/util/py_utils.py
+-rwxrwxrwx   0 wuhanchu  (1000) wuhanchu  (1000)     3400 2024-02-21 08:23:15.000000 flask_frame-0.6.4/src/flask_frame/util/rsa_tool.py
+-rwxrwxrwx   0 wuhanchu  (1000) wuhanchu  (1000)     1296 2022-11-10 06:57:22.000000 flask_frame-0.6.4/src/flask_frame/util/sql_tool.py
+-rwxrwxrwx   0 wuhanchu  (1000) wuhanchu  (1000)    13900 2024-02-21 08:23:15.000000 flask_frame-0.6.4/src/flask_frame/util/text.py
+-rwxrwxrwx   0 wuhanchu  (1000) wuhanchu  (1000)       24 2022-11-10 06:57:22.000000 flask_frame-0.6.4/src/flask_frame/util/time.py
+-rwxrwxrwx   0 wuhanchu  (1000) wuhanchu  (1000)    12352 2024-02-21 08:23:15.000000 flask_frame-0.6.4/src/flask_frame/util/txt_compare.py
+-rwxrwxrwx   0 wuhanchu  (1000) wuhanchu  (1000)    12442 2024-02-21 08:23:15.000000 flask_frame-0.6.4/src/flask_frame/util/wav.py
+drwxr-xr-x   0 wuhanchu  (1000) wuhanchu  (1000)        0 2024-05-16 02:34:05.808057 flask_frame-0.6.4/src/flask_frame.egg-info/
+-rwxrwxrwx   0 wuhanchu  (1000) wuhanchu  (1000)      254 2024-05-16 02:34:05.000000 flask_frame-0.6.4/src/flask_frame.egg-info/PKG-INFO
+-rwxrwxrwx   0 wuhanchu  (1000) wuhanchu  (1000)     2107 2024-05-16 02:34:05.000000 flask_frame-0.6.4/src/flask_frame.egg-info/SOURCES.txt
+-rwxrwxrwx   0 wuhanchu  (1000) wuhanchu  (1000)        1 2024-05-16 02:34:05.000000 flask_frame-0.6.4/src/flask_frame.egg-info/dependency_links.txt
+-rwxrwxrwx   0 wuhanchu  (1000) wuhanchu  (1000)      536 2024-05-16 02:34:05.000000 flask_frame-0.6.4/src/flask_frame.egg-info/requires.txt
+-rwxrwxrwx   0 wuhanchu  (1000) wuhanchu  (1000)       12 2024-05-16 02:34:05.000000 flask_frame-0.6.4/src/flask_frame.egg-info/top_level.txt
```

### Comparing `flask_frame-0.6.3/LICENSE` & `flask_frame-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `flask_frame-0.6.3/setup.py` & `flask_frame-0.6.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     install_requires = [
         str(requirement)
         for requirement in pkg_resources.parse_requirements(requirements_txt)
     ]
 
 setup(
     name="flask_frame",
-    version="0.6.3",
+    version="0.6.4",
     author="wuhanchu",
     author_email="whcwuhanchu@gmail.com",
     description="基于FLASK快速开发REST接口框架",
     packages=find_packages("src"),
     package_dir={"": "src"},
     install_requires=install_requires,
 )
```

### Comparing `flask_frame-0.6.3/src/flask_frame/algorithm/text.py` & `flask_frame-0.6.4/src/flask_frame/algorithm/text.py`

 * *Files identical despite different names*

### Comparing `flask_frame-0.6.3/src/flask_frame/annotation/__init__.py` & `flask_frame-0.6.4/src/flask_frame/annotation/__init__.py`

 * *Files identical despite different names*

### Comparing `flask_frame-0.6.3/src/flask_frame/api/__init__.py` & `flask_frame-0.6.4/src/flask_frame/api/__init__.py`

 * *Files identical despite different names*

### Comparing `flask_frame-0.6.3/src/flask_frame/api/exception.py` & `flask_frame-0.6.4/src/flask_frame/api/exception.py`

 * *Files identical despite different names*

### Comparing `flask_frame-0.6.3/src/flask_frame/api/request.py` & `flask_frame-0.6.4/src/flask_frame/api/request.py`

 * *Files identical despite different names*

### Comparing `flask_frame-0.6.3/src/flask_frame/api/response.py` & `flask_frame-0.6.4/src/flask_frame/api/response.py`

 * *Files identical despite different names*

### Comparing `flask_frame-0.6.3/src/flask_frame/app.py` & `flask_frame-0.6.4/src/flask_frame/app.py`

 * *Files identical despite different names*

### Comparing `flask_frame-0.6.3/src/flask_frame/extension/api_log/__init__.py` & `flask_frame-0.6.4/src/flask_frame/extension/api_log/__init__.py`

 * *Files identical despite different names*

### Comparing `flask_frame-0.6.3/src/flask_frame/extension/celery.py` & `flask_frame-0.6.4/src/flask_frame/extension/celery.py`

 * *Files identical despite different names*

### Comparing `flask_frame-0.6.3/src/flask_frame/extension/database/__init__.py` & `flask_frame-0.6.4/src/flask_frame/extension/database/__init__.py`

 * *Files identical despite different names*

### Comparing `flask_frame-0.6.3/src/flask_frame/extension/lock.py` & `flask_frame-0.6.4/src/flask_frame/extension/lock.py`

 * *Files identical despite different names*

### Comparing `flask_frame-0.6.3/src/flask_frame/extension/loguru/__init__.py` & `flask_frame-0.6.4/src/flask_frame/extension/loguru/__init__.py`

 * *Files identical despite different names*

### Comparing `flask_frame-0.6.3/src/flask_frame/extension/loguru/compress.py` & `flask_frame-0.6.4/src/flask_frame/extension/loguru/compress.py`

 * *Files identical despite different names*

### Comparing `flask_frame-0.6.3/src/flask_frame/extension/participle.py` & `flask_frame-0.6.4/src/flask_frame/extension/participle.py`

 * *Files identical despite different names*

### Comparing `flask_frame-0.6.3/src/flask_frame/extension/permission.py` & `flask_frame-0.6.4/src/flask_frame/extension/permission.py`

 * *Files identical despite different names*

### Comparing `flask_frame-0.6.3/src/flask_frame/extension/postgrest/__init__.py` & `flask_frame-0.6.4/src/flask_frame/extension/postgrest/__init__.py`

 * *Files identical despite different names*

### Comparing `flask_frame-0.6.3/src/flask_frame/extension/postgrest/sql_generator.py` & `flask_frame-0.6.4/src/flask_frame/extension/postgrest/sql_generator.py`

 * *Files identical despite different names*

### Comparing `flask_frame-0.6.3/src/flask_frame/extension/redis.py` & `flask_frame-0.6.4/src/flask_frame/extension/redis.py`

 * *Files identical despite different names*

### Comparing `flask_frame-0.6.3/src/flask_frame/extension/sentry.py` & `flask_frame-0.6.4/src/flask_frame/extension/sentry.py`

 * *Files identical despite different names*

### Comparing `flask_frame-0.6.3/src/flask_frame/file/__init__.py` & `flask_frame-0.6.4/src/flask_frame/file/__init__.py`

 * *Files identical despite different names*

### Comparing `flask_frame-0.6.3/src/flask_frame/file/audio.py` & `flask_frame-0.6.4/src/flask_frame/file/audio.py`

 * *Files identical despite different names*

### Comparing `flask_frame-0.6.3/src/flask_frame/permission_context.py` & `flask_frame-0.6.4/src/flask_frame/permission_context.py`

 * *Files identical despite different names*

### Comparing `flask_frame-0.6.3/src/flask_frame/thread/dk_thread_pool.py` & `flask_frame-0.6.4/src/flask_frame/thread/dk_thread_pool.py`

 * *Files identical despite different names*

### Comparing `flask_frame-0.6.3/src/flask_frame/thread/my_synchronized.py` & `flask_frame-0.6.4/src/flask_frame/thread/my_synchronized.py`

 * *Files identical despite different names*

### Comparing `flask_frame-0.6.3/src/flask_frame/util/algorithm.py` & `flask_frame-0.6.4/src/flask_frame/util/algorithm.py`

 * *Files identical despite different names*

### Comparing `flask_frame-0.6.3/src/flask_frame/util/com_tool.py` & `flask_frame-0.6.4/src/flask_frame/util/com_tool.py`

 * *Files identical despite different names*

### Comparing `flask_frame-0.6.3/src/flask_frame/util/db.py` & `flask_frame-0.6.4/src/flask_frame/util/db.py`

 * *Files identical despite different names*

### Comparing `flask_frame-0.6.3/src/flask_frame/util/doc.py` & `flask_frame-0.6.4/src/flask_frame/util/doc.py`

 * *Files identical despite different names*

### Comparing `flask_frame-0.6.3/src/flask_frame/util/file.py` & `flask_frame-0.6.4/src/flask_frame/util/file.py`

 * *Files identical despite different names*

### Comparing `flask_frame-0.6.3/src/flask_frame/util/lock.py` & `flask_frame-0.6.4/src/flask_frame/util/lock.py`

 * *Files identical despite different names*

### Comparing `flask_frame-0.6.3/src/flask_frame/util/model.py` & `flask_frame-0.6.4/src/flask_frame/util/model.py`

 * *Files identical despite different names*

### Comparing `flask_frame-0.6.3/src/flask_frame/util/obj.py` & `flask_frame-0.6.4/src/flask_frame/util/obj.py`

 * *Files identical despite different names*

### Comparing `flask_frame-0.6.3/src/flask_frame/util/param_tool.py` & `flask_frame-0.6.4/src/flask_frame/util/param_tool.py`

 * *Files identical despite different names*

### Comparing `flask_frame-0.6.3/src/flask_frame/util/rsa_tool.py` & `flask_frame-0.6.4/src/flask_frame/util/rsa_tool.py`

 * *Files identical despite different names*

### Comparing `flask_frame-0.6.3/src/flask_frame/util/sql_tool.py` & `flask_frame-0.6.4/src/flask_frame/util/sql_tool.py`

 * *Files identical despite different names*

### Comparing `flask_frame-0.6.3/src/flask_frame/util/text.py` & `flask_frame-0.6.4/src/flask_frame/util/text.py`

 * *Files identical despite different names*

### Comparing `flask_frame-0.6.3/src/flask_frame/util/txt_compare.py` & `flask_frame-0.6.4/src/flask_frame/util/txt_compare.py`

 * *Files identical despite different names*

### Comparing `flask_frame-0.6.3/src/flask_frame/util/wav.py` & `flask_frame-0.6.4/src/flask_frame/util/wav.py`

 * *Files identical despite different names*

### Comparing `flask_frame-0.6.3/src/flask_frame.egg-info/SOURCES.txt` & `flask_frame-0.6.4/src/flask_frame.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flask_frame-0.6.3/src/flask_frame.egg-info/requires.txt` & `flask_frame-0.6.4/src/flask_frame.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,14 @@
 eventlet==0.31.0
 pandas~=1.3.3
 filetype~=1.0.7
 pyinstrument~=4.4.0
 psutil~=5.7.0
 rsa~=4.0
 sentry-sdk[flask]==1.10.1
-numpy~=1.21.2
+numpy~=1.24.4
 gevent==21.8.0
 flask-marshmallow~=0.14.0
 pydevd-pycharm~=202.6397.94
 cn2an~=0.5.11
 chardet~=3.0.4
 tenacity==8.0.1
```

