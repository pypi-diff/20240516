# Comparing `tmp/flowchat-1.2.4.tar.gz` & `tmp/flowchat-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flowchat-1.2.4.tar", last modified: Thu May 16 17:28:13 2024, max compression
+gzip compressed data, was "flowchat-1.2.5.tar", last modified: Thu May 16 17:40:58 2024, max compression
```

## Comparing `flowchat-1.2.4.tar` & `flowchat-1.2.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 flatypus   (501) staff       (20)        0 2024-05-16 17:28:13.639593 flowchat-1.2.4/
--rw-r--r--   0 flatypus   (501) staff       (20)     1068 2024-03-05 00:02:48.000000 flowchat-1.2.4/LICENSE
--rw-r--r--   0 flatypus   (501) staff       (20)     7640 2024-05-16 17:28:13.639333 flowchat-1.2.4/PKG-INFO
--rw-r--r--   0 flatypus   (501) staff       (20)     6705 2024-04-14 20:10:37.000000 flowchat-1.2.4/README.md
-drwxr-xr-x   0 flatypus   (501) staff       (20)        0 2024-05-16 17:28:13.635906 flowchat-1.2.4/flowchat/
--rw-r--r--   0 flatypus   (501) staff       (20)       81 2024-04-16 03:29:58.000000 flowchat-1.2.4/flowchat/__init__.py
--rw-r--r--   0 flatypus   (501) staff       (20)      590 2024-03-08 00:59:53.000000 flowchat-1.2.4/flowchat/autodedent.py
--rw-r--r--   0 flatypus   (501) staff       (20)    11642 2024-05-16 17:25:48.000000 flowchat-1.2.4/flowchat/chain.py
-drwxr-xr-x   0 flatypus   (501) staff       (20)        0 2024-05-16 17:28:13.637094 flowchat-1.2.4/flowchat/private/
--rw-r--r--   0 flatypus   (501) staff       (20)        0 2023-11-08 02:00:20.000000 flowchat-1.2.4/flowchat/private/__init__.py
--rw-r--r--   0 flatypus   (501) staff       (20)      752 2024-05-16 17:27:36.000000 flowchat-1.2.4/flowchat/private/_private_helpers.py
--rw-r--r--   0 flatypus   (501) staff       (20)     2098 2024-05-16 17:23:53.000000 flowchat-1.2.4/flowchat/types.py
-drwxr-xr-x   0 flatypus   (501) staff       (20)        0 2024-05-16 17:28:13.638992 flowchat-1.2.4/flowchat.egg-info/
--rw-r--r--   0 flatypus   (501) staff       (20)     7640 2024-05-16 17:28:13.000000 flowchat-1.2.4/flowchat.egg-info/PKG-INFO
--rw-r--r--   0 flatypus   (501) staff       (20)      455 2024-05-16 17:28:13.000000 flowchat-1.2.4/flowchat.egg-info/SOURCES.txt
--rw-r--r--   0 flatypus   (501) staff       (20)        1 2024-05-16 17:28:13.000000 flowchat-1.2.4/flowchat.egg-info/dependency_links.txt
--rw-r--r--   0 flatypus   (501) staff       (20)       23 2024-05-16 17:28:13.000000 flowchat-1.2.4/flowchat.egg-info/requires.txt
--rw-r--r--   0 flatypus   (501) staff       (20)        9 2024-05-16 17:28:13.000000 flowchat-1.2.4/flowchat.egg-info/top_level.txt
--rw-r--r--   0 flatypus   (501) staff       (20)      153 2023-11-25 09:49:08.000000 flowchat-1.2.4/pyproject.toml
--rw-r--r--   0 flatypus   (501) staff       (20)       38 2024-05-16 17:28:13.639639 flowchat-1.2.4/setup.cfg
--rw-r--r--   0 flatypus   (501) staff       (20)     1379 2024-05-16 17:28:05.000000 flowchat-1.2.4/setup.py
-drwxr-xr-x   0 flatypus   (501) staff       (20)        0 2024-05-16 17:28:13.638708 flowchat-1.2.4/tests/
--rw-r--r--   0 flatypus   (501) staff       (20)     2041 2023-11-25 09:35:06.000000 flowchat-1.2.4/tests/test_autodedent.py
--rw-r--r--   0 flatypus   (501) staff       (20)     4250 2024-04-16 02:44:31.000000 flowchat-1.2.4/tests/test_chaining.py
--rw-r--r--   0 flatypus   (501) staff       (20)     1344 2023-11-25 07:32:30.000000 flowchat-1.2.4/tests/test_config.py
--rw-r--r--   0 flatypus   (501) staff       (20)     4765 2024-04-16 02:44:31.000000 flowchat-1.2.4/tests/test_pull.py
--rw-r--r--   0 flatypus   (501) staff       (20)     1214 2023-11-25 10:45:06.000000 flowchat-1.2.4/tests/test_stream.py
+drwxr-xr-x   0 flatypus   (501) staff       (20)        0 2024-05-16 17:40:58.108920 flowchat-1.2.5/
+-rw-r--r--   0 flatypus   (501) staff       (20)     1068 2024-03-05 00:02:48.000000 flowchat-1.2.5/LICENSE
+-rw-r--r--   0 flatypus   (501) staff       (20)     7640 2024-05-16 17:40:58.108699 flowchat-1.2.5/PKG-INFO
+-rw-r--r--   0 flatypus   (501) staff       (20)     6705 2024-04-14 20:10:37.000000 flowchat-1.2.5/README.md
+drwxr-xr-x   0 flatypus   (501) staff       (20)        0 2024-05-16 17:40:58.105436 flowchat-1.2.5/flowchat/
+-rw-r--r--   0 flatypus   (501) staff       (20)       81 2024-04-16 03:29:58.000000 flowchat-1.2.5/flowchat/__init__.py
+-rw-r--r--   0 flatypus   (501) staff       (20)      590 2024-03-08 00:59:53.000000 flowchat-1.2.5/flowchat/autodedent.py
+-rw-r--r--   0 flatypus   (501) staff       (20)    11642 2024-05-16 17:25:48.000000 flowchat-1.2.5/flowchat/chain.py
+drwxr-xr-x   0 flatypus   (501) staff       (20)        0 2024-05-16 17:40:58.106521 flowchat-1.2.5/flowchat/private/
+-rw-r--r--   0 flatypus   (501) staff       (20)        0 2023-11-08 02:00:20.000000 flowchat-1.2.5/flowchat/private/__init__.py
+-rw-r--r--   0 flatypus   (501) staff       (20)      752 2024-05-16 17:27:36.000000 flowchat-1.2.5/flowchat/private/_private_helpers.py
+-rw-r--r--   0 flatypus   (501) staff       (20)     2084 2024-05-16 17:40:37.000000 flowchat-1.2.5/flowchat/types.py
+drwxr-xr-x   0 flatypus   (501) staff       (20)        0 2024-05-16 17:40:58.108311 flowchat-1.2.5/flowchat.egg-info/
+-rw-r--r--   0 flatypus   (501) staff       (20)     7640 2024-05-16 17:40:58.000000 flowchat-1.2.5/flowchat.egg-info/PKG-INFO
+-rw-r--r--   0 flatypus   (501) staff       (20)      455 2024-05-16 17:40:58.000000 flowchat-1.2.5/flowchat.egg-info/SOURCES.txt
+-rw-r--r--   0 flatypus   (501) staff       (20)        1 2024-05-16 17:40:58.000000 flowchat-1.2.5/flowchat.egg-info/dependency_links.txt
+-rw-r--r--   0 flatypus   (501) staff       (20)       23 2024-05-16 17:40:58.000000 flowchat-1.2.5/flowchat.egg-info/requires.txt
+-rw-r--r--   0 flatypus   (501) staff       (20)        9 2024-05-16 17:40:58.000000 flowchat-1.2.5/flowchat.egg-info/top_level.txt
+-rw-r--r--   0 flatypus   (501) staff       (20)      153 2023-11-25 09:49:08.000000 flowchat-1.2.5/pyproject.toml
+-rw-r--r--   0 flatypus   (501) staff       (20)       38 2024-05-16 17:40:58.108964 flowchat-1.2.5/setup.cfg
+-rw-r--r--   0 flatypus   (501) staff       (20)     1379 2024-05-16 17:40:44.000000 flowchat-1.2.5/setup.py
+drwxr-xr-x   0 flatypus   (501) staff       (20)        0 2024-05-16 17:40:58.107960 flowchat-1.2.5/tests/
+-rw-r--r--   0 flatypus   (501) staff       (20)     2041 2023-11-25 09:35:06.000000 flowchat-1.2.5/tests/test_autodedent.py
+-rw-r--r--   0 flatypus   (501) staff       (20)     4250 2024-04-16 02:44:31.000000 flowchat-1.2.5/tests/test_chaining.py
+-rw-r--r--   0 flatypus   (501) staff       (20)     1344 2023-11-25 07:32:30.000000 flowchat-1.2.5/tests/test_config.py
+-rw-r--r--   0 flatypus   (501) staff       (20)     4765 2024-04-16 02:44:31.000000 flowchat-1.2.5/tests/test_pull.py
+-rw-r--r--   0 flatypus   (501) staff       (20)     1214 2023-11-25 10:45:06.000000 flowchat-1.2.5/tests/test_stream.py
```

### Comparing `flowchat-1.2.4/LICENSE` & `flowchat-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `flowchat-1.2.4/PKG-INFO` & `flowchat-1.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flowchat
-Version: 1.2.4
+Version: 1.2.5
 Summary: Streamlining the process of multi-prompting LLMs with chains
 Home-page: https://github.com/flatypus/flowchat
 Author: Hinson Chan
 Author-email: <yhc3141@gmail.com>
 Maintainer: Hinson Chan
 Maintainer-email: <yhc3141@gmail.com>
 License: MIT
```

### Comparing `flowchat-1.2.4/README.md` & `flowchat-1.2.5/README.md`

 * *Files identical despite different names*

### Comparing `flowchat-1.2.4/flowchat/autodedent.py` & `flowchat-1.2.5/flowchat/autodedent.py`

 * *Files identical despite different names*

### Comparing `flowchat-1.2.4/flowchat/chain.py` & `flowchat-1.2.5/flowchat/chain.py`

 * *Files identical despite different names*

### Comparing `flowchat-1.2.4/flowchat/private/_private_helpers.py` & `flowchat-1.2.5/flowchat/private/_private_helpers.py`

 * *Files identical despite different names*

### Comparing `flowchat-1.2.4/flowchat/types.py` & `flowchat-1.2.5/flowchat/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     'function': ToolChoiceFunction
 })
 
 
 class RequestParams(TypedDict, total=False):
     model: NotRequired[str]
     frequency_penalty: NotRequired[Union[float, int]]
-    logit_bias: NotRequired[Dict[str, Union[float, int]]]
+    logit_bias: NotRequired[Dict[Any, Any]]
     logprobs: NotRequired[bool]
     top_logprobs: NotRequired[int]
     max_tokens: NotRequired[Union[float, int]]
     n: NotRequired[Union[float, int]]
     presence_penalty: NotRequired[Union[float, int]]
     response_format: NotRequired[ResponseFormat]
     seed: NotRequired[int]
```

### Comparing `flowchat-1.2.4/flowchat.egg-info/PKG-INFO` & `flowchat-1.2.5/flowchat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flowchat
-Version: 1.2.4
+Version: 1.2.5
 Summary: Streamlining the process of multi-prompting LLMs with chains
 Home-page: https://github.com/flatypus/flowchat
 Author: Hinson Chan
 Author-email: <yhc3141@gmail.com>
 Maintainer: Hinson Chan
 Maintainer-email: <yhc3141@gmail.com>
 License: MIT
```

### Comparing `flowchat-1.2.4/setup.py` & `flowchat-1.2.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
-VERSION = '1.2.4'
+VERSION = '1.2.5'
 DESCRIPTION = 'Streamlining the process of multi-prompting LLMs with chains'
 
 setup(
     name="flowchat",
     version=VERSION,
     author="Hinson Chan",
     author_email="<yhc3141@gmail.com>",
```

### Comparing `flowchat-1.2.4/tests/test_autodedent.py` & `flowchat-1.2.5/tests/test_autodedent.py`

 * *Files identical despite different names*

### Comparing `flowchat-1.2.4/tests/test_chaining.py` & `flowchat-1.2.5/tests/test_chaining.py`

 * *Files identical despite different names*

### Comparing `flowchat-1.2.4/tests/test_config.py` & `flowchat-1.2.5/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `flowchat-1.2.4/tests/test_pull.py` & `flowchat-1.2.5/tests/test_pull.py`

 * *Files identical despite different names*

### Comparing `flowchat-1.2.4/tests/test_stream.py` & `flowchat-1.2.5/tests/test_stream.py`

 * *Files identical despite different names*

