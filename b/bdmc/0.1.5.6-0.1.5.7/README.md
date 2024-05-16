# Comparing `tmp/bdmc-0.1.5.6.tar.gz` & `tmp/bdmc-0.1.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bdmc-0.1.5.6.tar", last modified: Tue May 14 11:19:25 2024, max compression
+gzip compressed data, was "bdmc-0.1.5.7.tar", last modified: Thu May 16 13:18:59 2024, max compression
```

## Comparing `bdmc-0.1.5.6.tar` & `bdmc-0.1.5.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     5466 2024-05-14 11:19:06.232864 bdmc-0.1.5.6/README.md
--rw-r--r--   0        0        0      547 2024-05-14 11:19:25.569004 bdmc-0.1.5.6/pyproject.toml
--rw-r--r--   0        0        0      556 2024-05-14 11:19:06.232864 bdmc-0.1.5.6/src/bdmc/__init__.py
--rw-r--r--   0        0        0      419 2024-05-14 11:19:06.232864 bdmc-0.1.5.6/src/bdmc/modules/cmd.py
--rw-r--r--   0        0        0    17701 2024-05-14 11:19:06.232864 bdmc-0.1.5.6/src/bdmc/modules/controller.py
--rw-r--r--   0        0        0     2266 2024-05-14 11:19:06.232864 bdmc-0.1.5.6/src/bdmc/modules/debug.py
--rw-r--r--   0        0        0      574 2024-05-14 11:19:06.232864 bdmc-0.1.5.6/src/bdmc/modules/logger.py
--rw-r--r--   0        0        0     1356 2024-05-14 11:19:06.232864 bdmc-0.1.5.6/src/bdmc/modules/port.py
--rw-r--r--   0        0        0     7529 2024-05-14 11:19:06.232864 bdmc-0.1.5.6/src/bdmc/modules/seriald.py
--rw-r--r--   0        0        0      682 2024-05-14 11:19:06.232864 bdmc-0.1.5.6/tests/find_tests.py
--rw-r--r--   0        0        0     4380 2024-05-14 11:19:06.232864 bdmc-0.1.5.6/tests/test_context.py
--rw-r--r--   0        0        0     1989 2024-05-14 11:19:06.232864 bdmc-0.1.5.6/tests/test_controller.py
--rw-r--r--   0        0        0     5782 1970-01-01 00:00:00.000000 bdmc-0.1.5.6/PKG-INFO
+-rw-r--r--   0        0        0     5466 2024-05-16 13:18:40.790090 bdmc-0.1.5.7/README.md
+-rw-r--r--   0        0        0      547 2024-05-16 13:18:59.334127 bdmc-0.1.5.7/pyproject.toml
+-rw-r--r--   0        0        0      556 2024-05-16 13:18:40.790090 bdmc-0.1.5.7/src/bdmc/__init__.py
+-rw-r--r--   0        0        0      419 2024-05-16 13:18:40.790090 bdmc-0.1.5.7/src/bdmc/modules/cmd.py
+-rw-r--r--   0        0        0    17286 2024-05-16 13:18:40.790090 bdmc-0.1.5.7/src/bdmc/modules/controller.py
+-rw-r--r--   0        0        0     2266 2024-05-16 13:18:40.790090 bdmc-0.1.5.7/src/bdmc/modules/debug.py
+-rw-r--r--   0        0        0      574 2024-05-16 13:18:40.790090 bdmc-0.1.5.7/src/bdmc/modules/logger.py
+-rw-r--r--   0        0        0     1356 2024-05-16 13:18:40.790090 bdmc-0.1.5.7/src/bdmc/modules/port.py
+-rw-r--r--   0        0        0     7529 2024-05-16 13:18:40.790090 bdmc-0.1.5.7/src/bdmc/modules/seriald.py
+-rw-r--r--   0        0        0      682 2024-05-16 13:18:40.794090 bdmc-0.1.5.7/tests/find_tests.py
+-rw-r--r--   0        0        0     4380 2024-05-16 13:18:40.794090 bdmc-0.1.5.7/tests/test_context.py
+-rw-r--r--   0        0        0     1989 2024-05-16 13:18:40.794090 bdmc-0.1.5.7/tests/test_controller.py
+-rw-r--r--   0        0        0     5782 1970-01-01 00:00:00.000000 bdmc-0.1.5.7/PKG-INFO
```

### Comparing `bdmc-0.1.5.6/README.md` & `bdmc-0.1.5.7/README.md`

 * *Files identical despite different names*

### Comparing `bdmc-0.1.5.6/pyproject.toml` & `bdmc-0.1.5.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "bdmc"
-version = "0.1.5.6"
+version = "0.1.5.7"
 description = "An api wrapper lib designed for the uptech BDMC divers"
 authors = [
     { name = "Whth", email = "88489697+Whth@users.noreply.github.com" },
 ]
 dependencies = [
     "pyserial>=3.5",
     "coloredlogs>=15.0.1",
```

### Comparing `bdmc-0.1.5.6/src/bdmc/__init__.py` & `bdmc-0.1.5.7/src/bdmc/__init__.py`

 * *Files identical despite different names*

### Comparing `bdmc-0.1.5.6/src/bdmc/modules/controller.py` & `bdmc-0.1.5.7/src/bdmc/modules/controller.py`

 * *Files 6% similar despite different names*

```diff
@@ -372,18 +372,14 @@
              It should be at least twice as large as the delay_sec parameter to ensure accurate timing.
             - The breaker function is called periodically to check if the delay should be aborted.
             If the breaker function returns True, the delay is aborted and the function returns immediately.
             - If the breaker function returns False, the function continues to check the breaker function until either
             the delay is completed or the breaker function returns True.
             - If the delay is completed before the breaker function returns True, the function returns immediately.
         """
-        if not (delay_sec > check_interval * 2):
-            raise ValueError(
-                f"check_interval must be 2 times greater than delay_sec, while 2 x {check_interval} > {delay_sec}"
-            )
 
         ed_time = time() + delay_sec - check_interval
         # this is to add the first time check, since the timer waits before the check
         if alarm := breaker():
             return self
         while not alarm and time() < ed_time:
             alarm = breaker()
@@ -416,18 +412,15 @@
             - The `check_interval` parameter specifies the interval in seconds between each check.
             It should be at least twice as large as the `delay_sec` parameter to ensure accurate timing.
             - The `breaker` function is called periodically to check if the delay should be aborted.
             If the `breaker` function returns True, the delay is aborted and the function returns immediately.
             - If the `breaker` function returns False, the function continues to check the `breaker` function until
             either the delay is completed or the `breaker` function returns True.
         """
-        if not (delay_sec > check_interval * 2):
-            raise ValueError(
-                f"check_interval must be 2 times greater than delay_sec, while 2 x {check_interval} > {delay_sec}"
-            )
+
         ed_time = time() + delay_sec - check_interval
         # this is to add the first time check, since the timer waits before the check
         if alarm := breaker():
             return alarm
         while not alarm and time() < ed_time:
             alarm = breaker()
             sleep(check_interval)
```

### Comparing `bdmc-0.1.5.6/src/bdmc/modules/debug.py` & `bdmc-0.1.5.7/src/bdmc/modules/debug.py`

 * *Files identical despite different names*

### Comparing `bdmc-0.1.5.6/src/bdmc/modules/logger.py` & `bdmc-0.1.5.7/src/bdmc/modules/logger.py`

 * *Files identical despite different names*

### Comparing `bdmc-0.1.5.6/src/bdmc/modules/port.py` & `bdmc-0.1.5.7/src/bdmc/modules/port.py`

 * *Files identical despite different names*

### Comparing `bdmc-0.1.5.6/src/bdmc/modules/seriald.py` & `bdmc-0.1.5.7/src/bdmc/modules/seriald.py`

 * *Files identical despite different names*

### Comparing `bdmc-0.1.5.6/tests/find_tests.py` & `bdmc-0.1.5.7/tests/find_tests.py`

 * *Files identical despite different names*

### Comparing `bdmc-0.1.5.6/tests/test_context.py` & `bdmc-0.1.5.7/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `bdmc-0.1.5.6/tests/test_controller.py` & `bdmc-0.1.5.7/tests/test_controller.py`

 * *Files identical despite different names*

### Comparing `bdmc-0.1.5.6/PKG-INFO` & `bdmc-0.1.5.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bdmc
-Version: 0.1.5.6
+Version: 0.1.5.7
 Summary: An api wrapper lib designed for the uptech BDMC divers
 Author-Email: Whth <88489697+Whth@users.noreply.github.com>
 License: MIT
 Requires-Python: >=3.11
 Requires-Dist: pyserial>=3.5
 Requires-Dist: coloredlogs>=15.0.1
 Description-Content-Type: text/markdown
```

