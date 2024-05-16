# Comparing `tmp/logfunc-2.6.0.tar.gz` & `tmp/logfunc-2.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logfunc-2.6.0.tar", last modified: Sat May 11 22:51:25 2024, max compression
+gzip compressed data, was "logfunc-2.6.1.tar", last modified: Thu May 16 20:19:15 2024, max compression
```

## Comparing `logfunc-2.6.0.tar` & `logfunc-2.6.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 mym2       (501) staff       (20)        0 2024-05-11 22:51:25.615986 logfunc-2.6.0/
--rw-r--r--   0 mym2       (501) staff       (20)     1068 2023-09-03 19:49:58.000000 logfunc-2.6.0/LICENSE
--rw-r--r--   0 mym2       (501) staff       (20)     8257 2024-05-11 22:51:25.615807 logfunc-2.6.0/PKG-INFO
--rw-r--r--   0 mym2       (501) staff       (20)     5812 2024-05-11 22:50:45.000000 logfunc-2.6.0/README.md
-drwxr-xr-x   0 mym2       (501) staff       (20)        0 2024-05-11 22:51:25.615091 logfunc-2.6.0/logfunc/
--rw-r--r--   0 mym2       (501) staff       (20)       56 2024-05-10 21:20:35.000000 logfunc-2.6.0/logfunc/__init__.py
--rw-r--r--   0 mym2       (501) staff       (20)     2822 2024-05-11 22:21:16.000000 logfunc-2.6.0/logfunc/config.py
--rw-r--r--   0 mym2       (501) staff       (20)       44 2024-05-11 18:23:56.000000 logfunc-2.6.0/logfunc/defaults.py
--rw-r--r--   0 mym2       (501) staff       (20)     6656 2024-05-11 22:48:04.000000 logfunc-2.6.0/logfunc/main.py
--rw-r--r--   0 mym2       (501) staff       (20)      673 2024-02-23 01:13:48.000000 logfunc-2.6.0/logfunc/msgs.py
--rw-r--r--   0 mym2       (501) staff       (20)     3238 2024-05-11 19:27:12.000000 logfunc-2.6.0/logfunc/utils.py
--rw-r--r--   0 mym2       (501) staff       (20)       22 2024-05-11 22:31:27.000000 logfunc-2.6.0/logfunc/version.py
-drwxr-xr-x   0 mym2       (501) staff       (20)        0 2024-05-11 22:51:25.615603 logfunc-2.6.0/logfunc.egg-info/
--rw-r--r--   0 mym2       (501) staff       (20)     8257 2024-05-11 22:51:25.000000 logfunc-2.6.0/logfunc.egg-info/PKG-INFO
--rw-r--r--   0 mym2       (501) staff       (20)      291 2024-05-11 22:51:25.000000 logfunc-2.6.0/logfunc.egg-info/SOURCES.txt
--rw-r--r--   0 mym2       (501) staff       (20)        1 2024-05-11 22:51:25.000000 logfunc-2.6.0/logfunc.egg-info/dependency_links.txt
--rw-r--r--   0 mym2       (501) staff       (20)        8 2024-05-11 22:51:25.000000 logfunc-2.6.0/logfunc.egg-info/top_level.txt
--rw-r--r--   0 mym2       (501) staff       (20)     1217 2024-05-11 22:31:27.000000 logfunc-2.6.0/pyproject.toml
--rw-r--r--   0 mym2       (501) staff       (20)       38 2024-05-11 22:51:25.616028 logfunc-2.6.0/setup.cfg
--rw-r--r--   0 mym2       (501) staff       (20)     1237 2024-05-10 01:40:24.000000 logfunc-2.6.0/setup.py
+drwxr-xr-x   0 mym2       (501) staff       (20)        0 2024-05-16 20:19:15.330566 logfunc-2.6.1/
+-rw-r--r--   0 mym2       (501) staff       (20)     1068 2023-09-03 19:49:58.000000 logfunc-2.6.1/LICENSE
+-rw-r--r--   0 mym2       (501) staff       (20)     8257 2024-05-16 20:19:15.330401 logfunc-2.6.1/PKG-INFO
+-rw-r--r--   0 mym2       (501) staff       (20)     5812 2024-05-11 22:50:45.000000 logfunc-2.6.1/README.md
+drwxr-xr-x   0 mym2       (501) staff       (20)        0 2024-05-16 20:19:15.329483 logfunc-2.6.1/logfunc/
+-rw-r--r--   0 mym2       (501) staff       (20)       56 2024-05-10 21:20:35.000000 logfunc-2.6.1/logfunc/__init__.py
+-rw-r--r--   0 mym2       (501) staff       (20)     2822 2024-05-13 18:48:48.000000 logfunc-2.6.1/logfunc/config.py
+-rw-r--r--   0 mym2       (501) staff       (20)       44 2024-05-11 18:23:56.000000 logfunc-2.6.1/logfunc/defaults.py
+-rw-r--r--   0 mym2       (501) staff       (20)     6656 2024-05-16 19:26:37.000000 logfunc-2.6.1/logfunc/main.py
+-rw-r--r--   0 mym2       (501) staff       (20)      673 2024-02-23 01:13:48.000000 logfunc-2.6.1/logfunc/msgs.py
+-rw-r--r--   0 mym2       (501) staff       (20)     3238 2024-05-11 19:27:12.000000 logfunc-2.6.1/logfunc/utils.py
+-rw-r--r--   0 mym2       (501) staff       (20)       22 2024-05-16 20:18:43.000000 logfunc-2.6.1/logfunc/version.py
+drwxr-xr-x   0 mym2       (501) staff       (20)        0 2024-05-16 20:19:15.330047 logfunc-2.6.1/logfunc.egg-info/
+-rw-r--r--   0 mym2       (501) staff       (20)     8257 2024-05-16 20:19:15.000000 logfunc-2.6.1/logfunc.egg-info/PKG-INFO
+-rw-r--r--   0 mym2       (501) staff       (20)      291 2024-05-16 20:19:15.000000 logfunc-2.6.1/logfunc.egg-info/SOURCES.txt
+-rw-r--r--   0 mym2       (501) staff       (20)        1 2024-05-16 20:19:15.000000 logfunc-2.6.1/logfunc.egg-info/dependency_links.txt
+-rw-r--r--   0 mym2       (501) staff       (20)        8 2024-05-16 20:19:15.000000 logfunc-2.6.1/logfunc.egg-info/top_level.txt
+-rw-r--r--   0 mym2       (501) staff       (20)     1209 2024-05-16 20:18:43.000000 logfunc-2.6.1/pyproject.toml
+-rw-r--r--   0 mym2       (501) staff       (20)       38 2024-05-16 20:19:15.330608 logfunc-2.6.1/setup.cfg
+-rw-r--r--   0 mym2       (501) staff       (20)     1237 2024-05-10 01:40:24.000000 logfunc-2.6.1/setup.py
```

### Comparing `logfunc-2.6.0/LICENSE` & `logfunc-2.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `logfunc-2.6.0/PKG-INFO` & `logfunc-2.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logfunc
-Version: 2.6.0
+Version: 2.6.1
 Summary: An EASY TO USE function decorator for advanced logging of function execution, including arguments, return values, and execution time.
 Home-page: https://github.com/cc-d/logf/
 Author: Cary Carter
 Author-email: Cary Carter <ccarterdev@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Cary Carter
```

### Comparing `logfunc-2.6.0/README.md` & `logfunc-2.6.1/README.md`

 * *Files identical despite different names*

### Comparing `logfunc-2.6.0/logfunc/config.py` & `logfunc-2.6.1/logfunc/config.py`

 * *Files identical despite different names*

### Comparing `logfunc-2.6.0/logfunc/main.py` & `logfunc-2.6.1/logfunc/main.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -157,15 +157,14 @@
     if cfg.level is not None and cfg.logf_log_level is not None:
         if loglevel_int(cfg.level) < loglevel_int(cfg.logf_log_level):
             return
 
     logmsg = MSG_FORMATS.enter.format(func_name=func_name, args_str=args_str)
 
     if id is not None:
-
         logmsg = logmsg.replace('()', '()[%s]' % id, 1)
 
     if cfg.use_print:
         print(logmsg)
     else:
         handle_log(
             logmsg, cfg.level, cfg.use_logger, log_stack_info=cfg.log_stack
@@ -188,14 +187,15 @@
     logmsg = msgs.exit_msg(
         cfg.single,
         func_name,
         end_time,
         args_str,
         trunc_str(result, cfg.max_str) if cfg.log_return else '',
     )
+
     if id is not None:
         logmsg = logmsg.replace('()', '()[%s]' % id, 1)
 
     if cfg.use_print:
         print(logmsg)
     else:
         handle_log(
```

### Comparing `logfunc-2.6.0/logfunc/msgs.py` & `logfunc-2.6.1/logfunc/msgs.py`

 * *Files identical despite different names*

### Comparing `logfunc-2.6.0/logfunc/utils.py` & `logfunc-2.6.1/logfunc/utils.py`

 * *Files identical despite different names*

### Comparing `logfunc-2.6.0/logfunc.egg-info/PKG-INFO` & `logfunc-2.6.1/logfunc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logfunc
-Version: 2.6.0
+Version: 2.6.1
 Summary: An EASY TO USE function decorator for advanced logging of function execution, including arguments, return values, and execution time.
 Home-page: https://github.com/cc-d/logf/
 Author: Cary Carter
 Author-email: Cary Carter <ccarterdev@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Cary Carter
```

### Comparing `logfunc-2.6.0/pyproject.toml` & `logfunc-2.6.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
-requires = ["setuptools>=40.6.0", "wheel"]
+requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "logfunc"
-version = '2.6.0'
+version = '2.6.1'
 description = "An EASY TO USE function decorator for advanced logging of function execution, including arguments, return values, and execution time."
 authors = [{name = "Cary Carter", email = "ccarterdev@gmail.com"}]
 license = {file = "LICENSE"}
 readme = "README.md"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
```

### Comparing `logfunc-2.6.0/setup.py` & `logfunc-2.6.1/setup.py`

 * *Files identical despite different names*

