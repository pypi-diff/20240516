# Comparing `tmp/aily_code_sdk_core-0.1.0b1.tar.gz` & `tmp/aily_code_sdk_core-0.1.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aily_code_sdk_core-0.1.0b1.tar", last modified: Wed May 15 08:47:56 2024, max compression
+gzip compressed data, was "aily_code_sdk_core-0.1.0b2.tar", last modified: Thu May 16 12:43:16 2024, max compression
```

## Comparing `aily_code_sdk_core-0.1.0b1.tar` & `aily_code_sdk_core-0.1.0b2.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2024-05-15 08:47:56.349769 aily_code_sdk_core-0.1.0b1/
--rw-r--r--   0 bytedance   (501) staff       (20)    10947 2024-05-15 08:04:11.000000 aily_code_sdk_core-0.1.0b1/LICENSE
--rw-r--r--   0 bytedance   (501) staff       (20)    13278 2024-05-15 08:47:56.349253 aily_code_sdk_core-0.1.0b1/PKG-INFO
--rw-r--r--   0 bytedance   (501) staff       (20)      341 2024-05-13 07:52:06.000000 aily_code_sdk_core-0.1.0b1/README.md
--rw-r--r--   0 bytedance   (501) staff       (20)      516 2024-05-15 08:47:45.000000 aily_code_sdk_core-0.1.0b1/pyproject.toml
--rw-r--r--   0 bytedance   (501) staff       (20)       38 2024-05-15 08:47:56.349826 aily_code_sdk_core-0.1.0b1/setup.cfg
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2024-05-15 08:47:56.334827 aily_code_sdk_core-0.1.0b1/src/
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2024-05-15 08:47:56.336905 aily_code_sdk_core-0.1.0b1/src/aily_code_sdk_core/
--rw-r--r--   0 bytedance   (501) staff       (20)        0 2024-05-13 11:55:38.000000 aily_code_sdk_core-0.1.0b1/src/aily_code_sdk_core/__init__.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2024-05-15 08:47:56.338972 aily_code_sdk_core-0.1.0b1/src/aily_code_sdk_core/action/
--rw-r--r--   0 bytedance   (501) staff       (20)       71 2024-05-13 12:16:24.000000 aily_code_sdk_core-0.1.0b1/src/aily_code_sdk_core/action/__init__.py
--rw-r--r--   0 bytedance   (501) staff       (20)     1312 2024-05-13 07:39:09.000000 aily_code_sdk_core-0.1.0b1/src/aily_code_sdk_core/action/call_action.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2024-05-15 08:47:56.339712 aily_code_sdk_core-0.1.0b1/src/aily_code_sdk_core/common/
--rw-r--r--   0 bytedance   (501) staff       (20)     1184 2024-05-13 07:24:36.000000 aily_code_sdk_core-0.1.0b1/src/aily_code_sdk_core/common/context.py
--rw-r--r--   0 bytedance   (501) staff       (20)      335 2024-05-13 07:28:48.000000 aily_code_sdk_core-0.1.0b1/src/aily_code_sdk_core/common/util.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2024-05-15 08:47:56.340483 aily_code_sdk_core-0.1.0b1/src/aily_code_sdk_core/credential/
--rw-r--r--   0 bytedance   (501) staff       (20)       74 2024-05-13 12:16:38.000000 aily_code_sdk_core-0.1.0b1/src/aily_code_sdk_core/credential/__init__.py
--rw-r--r--   0 bytedance   (501) staff       (20)     1559 2024-05-13 07:45:06.000000 aily_code_sdk_core-0.1.0b1/src/aily_code_sdk_core/credential/credential.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2024-05-15 08:47:56.341193 aily_code_sdk_core-0.1.0b1/src/aily_code_sdk_core/env/
--rw-r--r--   0 bytedance   (501) staff       (20)       74 2024-05-13 12:16:47.000000 aily_code_sdk_core-0.1.0b1/src/aily_code_sdk_core/env/__init__.py
--rw-r--r--   0 bytedance   (501) staff       (20)      458 2024-05-15 08:39:46.000000 aily_code_sdk_core-0.1.0b1/src/aily_code_sdk_core/env/get_env_info.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2024-05-15 08:47:56.341640 aily_code_sdk_core-0.1.0b1/src/aily_code_sdk_core/message/
--rw-r--r--   0 bytedance   (501) staff       (20)      752 2024-05-13 12:20:34.000000 aily_code_sdk_core-0.1.0b1/src/aily_code_sdk_core/message/builder.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2024-05-15 08:47:56.348446 aily_code_sdk_core-0.1.0b1/src/aily_code_sdk_core/message/components/
--rw-r--r--   0 bytedance   (501) staff       (20)      682 2024-05-13 12:17:00.000000 aily_code_sdk_core-0.1.0b1/src/aily_code_sdk_core/message/components/__init__.py
--rw-r--r--   0 bytedance   (501) staff       (20)     1840 2024-05-13 12:21:51.000000 aily_code_sdk_core-0.1.0b1/src/aily_code_sdk_core/message/components/base_component.py
--rw-r--r--   0 bytedance   (501) staff       (20)     1556 2024-05-11 04:30:30.000000 aily_code_sdk_core-0.1.0b1/src/aily_code_sdk_core/message/components/button.py
--rw-r--r--   0 bytedance   (501) staff       (20)      288 2024-05-11 03:23:07.000000 aily_code_sdk_core-0.1.0b1/src/aily_code_sdk_core/message/components/chart.py
--rw-r--r--   0 bytedance   (501) staff       (20)      362 2024-05-13 12:22:51.000000 aily_code_sdk_core-0.1.0b1/src/aily_code_sdk_core/message/components/code.py
--rw-r--r--   0 bytedance   (501) staff       (20)      266 2024-05-11 04:39:01.000000 aily_code_sdk_core-0.1.0b1/src/aily_code_sdk_core/message/components/col.py
--rw-r--r--   0 bytedance   (501) staff       (20)      441 2024-05-13 12:21:18.000000 aily_code_sdk_core-0.1.0b1/src/aily_code_sdk_core/message/components/color_text.py
--rw-r--r--   0 bytedance   (501) staff       (20)      934 2024-05-13 12:22:32.000000 aily_code_sdk_core-0.1.0b1/src/aily_code_sdk_core/message/components/data_record.py
--rw-r--r--   0 bytedance   (501) staff       (20)      399 2024-05-13 08:09:19.000000 aily_code_sdk_core-0.1.0b1/src/aily_code_sdk_core/message/components/highlight.py
--rw-r--r--   0 bytedance   (501) staff       (20)      337 2024-05-11 03:23:24.000000 aily_code_sdk_core-0.1.0b1/src/aily_code_sdk_core/message/components/image.py
--rw-r--r--   0 bytedance   (501) staff       (20)      354 2024-05-11 03:23:18.000000 aily_code_sdk_core-0.1.0b1/src/aily_code_sdk_core/message/components/item_list.py
--rw-r--r--   0 bytedance   (501) staff       (20)      559 2024-05-13 12:22:14.000000 aily_code_sdk_core-0.1.0b1/src/aily_code_sdk_core/message/components/link.py
--rw-r--r--   0 bytedance   (501) staff       (20)      365 2024-05-11 03:23:18.000000 aily_code_sdk_core-0.1.0b1/src/aily_code_sdk_core/message/components/mention.py
--rw-r--r--   0 bytedance   (501) staff       (20)      389 2024-05-11 08:11:14.000000 aily_code_sdk_core-0.1.0b1/src/aily_code_sdk_core/message/components/note.py
--rw-r--r--   0 bytedance   (501) staff       (20)      491 2024-05-13 12:02:12.000000 aily_code_sdk_core-0.1.0b1/src/aily_code_sdk_core/message/components/ordered_list.py
--rw-r--r--   0 bytedance   (501) staff       (20)      327 2024-05-11 03:23:18.000000 aily_code_sdk_core-0.1.0b1/src/aily_code_sdk_core/message/components/row.py
--rw-r--r--   0 bytedance   (501) staff       (20)     1055 2024-05-11 03:23:18.000000 aily_code_sdk_core-0.1.0b1/src/aily_code_sdk_core/message/components/table.py
--rw-r--r--   0 bytedance   (501) staff       (20)      587 2024-05-11 03:23:17.000000 aily_code_sdk_core-0.1.0b1/src/aily_code_sdk_core/message/components/title.py
-drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2024-05-15 08:47:56.348862 aily_code_sdk_core-0.1.0b1/src/aily_code_sdk_core.egg-info/
--rw-r--r--   0 bytedance   (501) staff       (20)    13278 2024-05-15 08:47:56.000000 aily_code_sdk_core-0.1.0b1/src/aily_code_sdk_core.egg-info/PKG-INFO
--rw-r--r--   0 bytedance   (501) staff       (20)     1632 2024-05-15 08:47:56.000000 aily_code_sdk_core-0.1.0b1/src/aily_code_sdk_core.egg-info/SOURCES.txt
--rw-r--r--   0 bytedance   (501) staff       (20)        1 2024-05-15 08:47:56.000000 aily_code_sdk_core-0.1.0b1/src/aily_code_sdk_core.egg-info/dependency_links.txt
--rw-r--r--   0 bytedance   (501) staff       (20)       24 2024-05-15 08:47:56.000000 aily_code_sdk_core-0.1.0b1/src/aily_code_sdk_core.egg-info/requires.txt
--rw-r--r--   0 bytedance   (501) staff       (20)       19 2024-05-15 08:47:56.000000 aily_code_sdk_core-0.1.0b1/src/aily_code_sdk_core.egg-info/top_level.txt
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2024-05-16 12:43:16.579367 aily_code_sdk_core-0.1.0b2/
+-rw-r--r--   0 bytedance   (501) staff       (20)    10947 2024-05-15 08:04:11.000000 aily_code_sdk_core-0.1.0b2/LICENSE
+-rw-r--r--   0 bytedance   (501) staff       (20)    13318 2024-05-16 12:43:16.578983 aily_code_sdk_core-0.1.0b2/PKG-INFO
+-rw-r--r--   0 bytedance   (501) staff       (20)      381 2024-05-16 12:43:10.000000 aily_code_sdk_core-0.1.0b2/README.md
+-rw-r--r--   0 bytedance   (501) staff       (20)      516 2024-05-16 12:42:46.000000 aily_code_sdk_core-0.1.0b2/pyproject.toml
+-rw-r--r--   0 bytedance   (501) staff       (20)       38 2024-05-16 12:43:16.579429 aily_code_sdk_core-0.1.0b2/setup.cfg
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2024-05-16 12:43:16.568659 aily_code_sdk_core-0.1.0b2/src/
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2024-05-16 12:43:16.570334 aily_code_sdk_core-0.1.0b2/src/aily_code_sdk_core/
+-rw-r--r--   0 bytedance   (501) staff       (20)        0 2024-05-13 11:55:38.000000 aily_code_sdk_core-0.1.0b2/src/aily_code_sdk_core/__init__.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2024-05-16 12:43:16.571904 aily_code_sdk_core-0.1.0b2/src/aily_code_sdk_core/action/
+-rw-r--r--   0 bytedance   (501) staff       (20)       71 2024-05-13 12:16:24.000000 aily_code_sdk_core-0.1.0b2/src/aily_code_sdk_core/action/__init__.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     1341 2024-05-16 08:25:22.000000 aily_code_sdk_core-0.1.0b2/src/aily_code_sdk_core/action/call_action.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2024-05-16 12:43:16.572406 aily_code_sdk_core-0.1.0b2/src/aily_code_sdk_core/common/
+-rw-r--r--   0 bytedance   (501) staff       (20)     1262 2024-05-16 12:42:13.000000 aily_code_sdk_core-0.1.0b2/src/aily_code_sdk_core/common/context.py
+-rw-r--r--   0 bytedance   (501) staff       (20)      335 2024-05-13 07:28:48.000000 aily_code_sdk_core-0.1.0b2/src/aily_code_sdk_core/common/util.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2024-05-16 12:43:16.572856 aily_code_sdk_core-0.1.0b2/src/aily_code_sdk_core/credential/
+-rw-r--r--   0 bytedance   (501) staff       (20)       74 2024-05-13 12:16:38.000000 aily_code_sdk_core-0.1.0b2/src/aily_code_sdk_core/credential/__init__.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     1593 2024-05-16 08:22:26.000000 aily_code_sdk_core-0.1.0b2/src/aily_code_sdk_core/credential/credential.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2024-05-16 12:43:16.573269 aily_code_sdk_core-0.1.0b2/src/aily_code_sdk_core/env/
+-rw-r--r--   0 bytedance   (501) staff       (20)       74 2024-05-13 12:16:47.000000 aily_code_sdk_core-0.1.0b2/src/aily_code_sdk_core/env/__init__.py
+-rw-r--r--   0 bytedance   (501) staff       (20)      458 2024-05-15 08:39:46.000000 aily_code_sdk_core-0.1.0b2/src/aily_code_sdk_core/env/get_env_info.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2024-05-16 12:43:16.573477 aily_code_sdk_core-0.1.0b2/src/aily_code_sdk_core/message/
+-rw-r--r--   0 bytedance   (501) staff       (20)      752 2024-05-13 12:20:34.000000 aily_code_sdk_core-0.1.0b2/src/aily_code_sdk_core/message/builder.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2024-05-16 12:43:16.578312 aily_code_sdk_core-0.1.0b2/src/aily_code_sdk_core/message/components/
+-rw-r--r--   0 bytedance   (501) staff       (20)      682 2024-05-13 12:17:00.000000 aily_code_sdk_core-0.1.0b2/src/aily_code_sdk_core/message/components/__init__.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     1840 2024-05-13 12:21:51.000000 aily_code_sdk_core-0.1.0b2/src/aily_code_sdk_core/message/components/base_component.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     1556 2024-05-11 04:30:30.000000 aily_code_sdk_core-0.1.0b2/src/aily_code_sdk_core/message/components/button.py
+-rw-r--r--   0 bytedance   (501) staff       (20)      288 2024-05-11 03:23:07.000000 aily_code_sdk_core-0.1.0b2/src/aily_code_sdk_core/message/components/chart.py
+-rw-r--r--   0 bytedance   (501) staff       (20)      362 2024-05-13 12:22:51.000000 aily_code_sdk_core-0.1.0b2/src/aily_code_sdk_core/message/components/code.py
+-rw-r--r--   0 bytedance   (501) staff       (20)      266 2024-05-11 04:39:01.000000 aily_code_sdk_core-0.1.0b2/src/aily_code_sdk_core/message/components/col.py
+-rw-r--r--   0 bytedance   (501) staff       (20)      441 2024-05-13 12:21:18.000000 aily_code_sdk_core-0.1.0b2/src/aily_code_sdk_core/message/components/color_text.py
+-rw-r--r--   0 bytedance   (501) staff       (20)      934 2024-05-13 12:22:32.000000 aily_code_sdk_core-0.1.0b2/src/aily_code_sdk_core/message/components/data_record.py
+-rw-r--r--   0 bytedance   (501) staff       (20)      399 2024-05-13 08:09:19.000000 aily_code_sdk_core-0.1.0b2/src/aily_code_sdk_core/message/components/highlight.py
+-rw-r--r--   0 bytedance   (501) staff       (20)      337 2024-05-11 03:23:24.000000 aily_code_sdk_core-0.1.0b2/src/aily_code_sdk_core/message/components/image.py
+-rw-r--r--   0 bytedance   (501) staff       (20)      354 2024-05-11 03:23:18.000000 aily_code_sdk_core-0.1.0b2/src/aily_code_sdk_core/message/components/item_list.py
+-rw-r--r--   0 bytedance   (501) staff       (20)      559 2024-05-13 12:22:14.000000 aily_code_sdk_core-0.1.0b2/src/aily_code_sdk_core/message/components/link.py
+-rw-r--r--   0 bytedance   (501) staff       (20)      365 2024-05-11 03:23:18.000000 aily_code_sdk_core-0.1.0b2/src/aily_code_sdk_core/message/components/mention.py
+-rw-r--r--   0 bytedance   (501) staff       (20)      389 2024-05-11 08:11:14.000000 aily_code_sdk_core-0.1.0b2/src/aily_code_sdk_core/message/components/note.py
+-rw-r--r--   0 bytedance   (501) staff       (20)      491 2024-05-13 12:02:12.000000 aily_code_sdk_core-0.1.0b2/src/aily_code_sdk_core/message/components/ordered_list.py
+-rw-r--r--   0 bytedance   (501) staff       (20)      327 2024-05-11 03:23:18.000000 aily_code_sdk_core-0.1.0b2/src/aily_code_sdk_core/message/components/row.py
+-rw-r--r--   0 bytedance   (501) staff       (20)     1055 2024-05-11 03:23:18.000000 aily_code_sdk_core-0.1.0b2/src/aily_code_sdk_core/message/components/table.py
+-rw-r--r--   0 bytedance   (501) staff       (20)      587 2024-05-11 03:23:17.000000 aily_code_sdk_core-0.1.0b2/src/aily_code_sdk_core/message/components/title.py
+drwxr-xr-x   0 bytedance   (501) staff       (20)        0 2024-05-16 12:43:16.578608 aily_code_sdk_core-0.1.0b2/src/aily_code_sdk_core.egg-info/
+-rw-r--r--   0 bytedance   (501) staff       (20)    13318 2024-05-16 12:43:16.000000 aily_code_sdk_core-0.1.0b2/src/aily_code_sdk_core.egg-info/PKG-INFO
+-rw-r--r--   0 bytedance   (501) staff       (20)     1632 2024-05-16 12:43:16.000000 aily_code_sdk_core-0.1.0b2/src/aily_code_sdk_core.egg-info/SOURCES.txt
+-rw-r--r--   0 bytedance   (501) staff       (20)        1 2024-05-16 12:43:16.000000 aily_code_sdk_core-0.1.0b2/src/aily_code_sdk_core.egg-info/dependency_links.txt
+-rw-r--r--   0 bytedance   (501) staff       (20)       24 2024-05-16 12:43:16.000000 aily_code_sdk_core-0.1.0b2/src/aily_code_sdk_core.egg-info/requires.txt
+-rw-r--r--   0 bytedance   (501) staff       (20)       19 2024-05-16 12:43:16.000000 aily_code_sdk_core-0.1.0b2/src/aily_code_sdk_core.egg-info/top_level.txt
```

### Comparing `aily_code_sdk_core-0.1.0b1/LICENSE` & `aily_code_sdk_core-0.1.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `aily_code_sdk_core-0.1.0b1/PKG-INFO` & `aily_code_sdk_core-0.1.0b2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aily_code_sdk_core
-Version: 0.1.0b1
+Version: 0.1.0b2
 Summary: Aily Code SDK
 Author-email: "sunlei.h" <sunlei.h@bytedance.com>, "zhaolizi.milo" <zhaolizi.milo@bytedance.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
         TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -221,7 +221,13 @@
 AILY_SDK_LOCAL_DEBUG=true
 AILY_SDK_CLIENT_ID=c_xxx
 AILY_SDK_CLIENT_SECRET=cxxx
 AILY_SDK_DOMAIN=https://ae-openapi.feishu-boe.cn/
 ```
 
 然后通过 `python -m unitest` 命令通过执行单元测试来调试代码。
+
+### Build
+
+```bash
+python -m build
+```
```

### Comparing `aily_code_sdk_core-0.1.0b1/pyproject.toml` & `aily_code_sdk_core-0.1.0b2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "aily_code_sdk_core"
-version = "0.1.0-beta.1"
+version = "0.1.0-beta.2"
 authors = [
   { name="sunlei.h", email="sunlei.h@bytedance.com" },
   { name="zhaolizi.milo", email="zhaolizi.milo@bytedance.com" },
 ]
 description = "Aily Code SDK"
 readme = "README.md"
 license = { file = "LICENSE" }
```

### Comparing `aily_code_sdk_core-0.1.0b1/src/aily_code_sdk_core/action/call_action.py` & `aily_code_sdk_core-0.1.0b2/src/aily_code_sdk_core/action/call_action.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,19 @@
 
 defaultOptions = {
     "timeout": 60 * 1000 * 5,
     "retry_times": 0,
 }
 
 
-def call_action(action_api_name: str, action_data: dict, options: dict = {}) -> dict:
+def call_action(
+    action_api_name: str,
+    action_data: dict,
+    options: dict = {},
+) -> dict:
     credential = AppCredential()
     token = credential.get_token()
     domain = get_domain()
 
     if not token:
         raise Exception('get token failed')
 
@@ -27,15 +31,15 @@
             'options': json.dumps({
                 **defaultOptions,
                 **options,
             }),
         },
     }
 
-    path = f'/ai/v1/connector_action/namespaces/{credential.namespace}/execute_action'
+    path = f'/ai/v1/connector_action/namespaces/{credential.namespace}/execute_action'  # noqa: E501
     url = urljoin(domain, path)
     res = http.post(url, json=req)
 
     if res.status_code != 200:
         raise Exception(f'call action failed: {res.text}')
 
     data = res.json()
```

### Comparing `aily_code_sdk_core-0.1.0b1/src/aily_code_sdk_core/common/context.py` & `aily_code_sdk_core-0.1.0b2/src/aily_code_sdk_core/common/context.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 import contextvars
 import os
 
 NodeClsKey = "x-apaas-node-cls"
+
 CtxVar = contextvars.ContextVar(NodeClsKey)
 
+try:
+    from _sys import CtxVar  # type: ignore
+except Exception:
+    pass
+
 
 def Ctx():
     return contextvars.copy_context()
 
 
 def get_ctx():
     try:
```

### Comparing `aily_code_sdk_core-0.1.0b1/src/aily_code_sdk_core/credential/credential.py` & `aily_code_sdk_core-0.1.0b2/src/aily_code_sdk_core/credential/credential.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,16 @@
     def __init__(self):
         self.expire_time = 0
         self.tenant_info = None
         self.id = get_client_id()
         self.secret = get_client_secret()
 
     def get_token(self):
-        if self.expire_time - datetime.now().timestamp() > AppTokenRefreshTime and self.token:
+        remain_time = self.expire_time - datetime.now().timestamp()
+        if remain_time > AppTokenRefreshTime and self.token:
             return self.token
         self.fetch_token()
         return self.token
 
     def get_tenant_info(self):
         if not self or not self.id or not self.secret:
             self.id = get_client_id()
```

### Comparing `aily_code_sdk_core-0.1.0b1/src/aily_code_sdk_core/message/builder.py` & `aily_code_sdk_core-0.1.0b2/src/aily_code_sdk_core/message/builder.py`

 * *Files identical despite different names*

### Comparing `aily_code_sdk_core-0.1.0b1/src/aily_code_sdk_core/message/components/__init__.py` & `aily_code_sdk_core-0.1.0b2/src/aily_code_sdk_core/message/components/__init__.py`

 * *Files identical despite different names*

### Comparing `aily_code_sdk_core-0.1.0b1/src/aily_code_sdk_core/message/components/base_component.py` & `aily_code_sdk_core-0.1.0b2/src/aily_code_sdk_core/message/components/base_component.py`

 * *Files identical despite different names*

### Comparing `aily_code_sdk_core-0.1.0b1/src/aily_code_sdk_core/message/components/button.py` & `aily_code_sdk_core-0.1.0b2/src/aily_code_sdk_core/message/components/button.py`

 * *Files identical despite different names*

### Comparing `aily_code_sdk_core-0.1.0b1/src/aily_code_sdk_core/message/components/data_record.py` & `aily_code_sdk_core-0.1.0b2/src/aily_code_sdk_core/message/components/data_record.py`

 * *Files identical despite different names*

### Comparing `aily_code_sdk_core-0.1.0b1/src/aily_code_sdk_core/message/components/link.py` & `aily_code_sdk_core-0.1.0b2/src/aily_code_sdk_core/message/components/link.py`

 * *Files identical despite different names*

### Comparing `aily_code_sdk_core-0.1.0b1/src/aily_code_sdk_core/message/components/table.py` & `aily_code_sdk_core-0.1.0b2/src/aily_code_sdk_core/message/components/table.py`

 * *Files identical despite different names*

### Comparing `aily_code_sdk_core-0.1.0b1/src/aily_code_sdk_core/message/components/title.py` & `aily_code_sdk_core-0.1.0b2/src/aily_code_sdk_core/message/components/title.py`

 * *Files identical despite different names*

### Comparing `aily_code_sdk_core-0.1.0b1/src/aily_code_sdk_core.egg-info/PKG-INFO` & `aily_code_sdk_core-0.1.0b2/src/aily_code_sdk_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aily_code_sdk_core
-Version: 0.1.0b1
+Version: 0.1.0b2
 Summary: Aily Code SDK
 Author-email: "sunlei.h" <sunlei.h@bytedance.com>, "zhaolizi.milo" <zhaolizi.milo@bytedance.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
         TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -221,7 +221,13 @@
 AILY_SDK_LOCAL_DEBUG=true
 AILY_SDK_CLIENT_ID=c_xxx
 AILY_SDK_CLIENT_SECRET=cxxx
 AILY_SDK_DOMAIN=https://ae-openapi.feishu-boe.cn/
 ```
 
 然后通过 `python -m unitest` 命令通过执行单元测试来调试代码。
+
+### Build
+
+```bash
+python -m build
+```
```

### Comparing `aily_code_sdk_core-0.1.0b1/src/aily_code_sdk_core.egg-info/SOURCES.txt` & `aily_code_sdk_core-0.1.0b2/src/aily_code_sdk_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

