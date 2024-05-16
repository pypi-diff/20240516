# Comparing `tmp/funcs_aux-0.1.3.tar.gz` & `tmp/funcs_aux-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funcs_aux-0.1.3.tar", last modified: Sat Apr 27 13:32:10 2024, max compression
+gzip compressed data, was "funcs_aux-0.1.4.tar", last modified: Thu May 16 09:01:22 2024, max compression
```

## Comparing `funcs_aux-0.1.3.tar` & `funcs_aux-0.1.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-27 13:32:10.201542 funcs_aux-0.1.3/
--rw-rw-rw-   0        0        0     1180 2023-12-28 13:58:03.000000 funcs_aux-0.1.3/LICENSE
--rw-rw-rw-   0        0        0     1883 2024-04-27 13:32:10.200541 funcs_aux-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0      990 2024-04-27 13:31:41.000000 funcs_aux-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2024-04-27 13:32:10.190369 funcs_aux-0.1.3/funcs_aux/
--rw-rw-rw-   0        0        0      282 2024-03-28 09:55:47.000000 funcs_aux-0.1.3/funcs_aux/__init__.py
--rw-rw-rw-   0        0        0     1894 2024-03-01 08:49:51.000000 funcs_aux-0.1.3/funcs_aux/arrays.py
--rw-rw-rw-   0        0        0     6005 2024-03-28 14:40:09.000000 funcs_aux-0.1.3/funcs_aux/collects.py
--rw-rw-rw-   0        0        0     5211 2024-03-22 14:19:18.000000 funcs_aux-0.1.3/funcs_aux/iterables.py
--rw-rw-rw-   0        0        0     9110 2024-04-27 13:29:45.000000 funcs_aux-0.1.3/funcs_aux/results.py
--rw-rw-rw-   0        0        0     1920 2024-03-01 08:45:13.000000 funcs_aux-0.1.3/funcs_aux/strings.py
-drwxrwxrwx   0        0        0        0 2024-04-27 13:32:10.200541 funcs_aux-0.1.3/funcs_aux.egg-info/
--rw-rw-rw-   0        0        0     1883 2024-04-27 13:32:10.000000 funcs_aux-0.1.3/funcs_aux.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      297 2024-04-27 13:32:10.000000 funcs_aux-0.1.3/funcs_aux.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-27 13:32:10.000000 funcs_aux-0.1.3/funcs_aux.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-04-27 13:32:10.000000 funcs_aux-0.1.3/funcs_aux.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-27 13:32:10.202542 funcs_aux-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0     2184 2024-01-30 14:09:01.000000 funcs_aux-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 09:01:22.971678 funcs_aux-0.1.4/
+-rw-rw-rw-   0        0        0     1180 2023-12-28 13:58:03.000000 funcs_aux-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0     1883 2024-05-16 09:01:22.970678 funcs_aux-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0      990 2024-05-16 09:00:23.000000 funcs_aux-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-16 09:01:22.962048 funcs_aux-0.1.4/funcs_aux/
+-rw-rw-rw-   0        0        0      282 2024-03-28 09:55:47.000000 funcs_aux-0.1.4/funcs_aux/__init__.py
+-rw-rw-rw-   0        0        0     1894 2024-03-01 08:49:51.000000 funcs_aux-0.1.4/funcs_aux/arrays.py
+-rw-rw-rw-   0        0        0     6005 2024-03-28 14:40:09.000000 funcs_aux-0.1.4/funcs_aux/collects.py
+-rw-rw-rw-   0        0        0     5211 2024-03-22 14:19:18.000000 funcs_aux-0.1.4/funcs_aux/iterables.py
+-rw-rw-rw-   0        0        0     9772 2024-05-16 08:59:28.000000 funcs_aux-0.1.4/funcs_aux/results.py
+-rw-rw-rw-   0        0        0     1920 2024-03-01 08:45:13.000000 funcs_aux-0.1.4/funcs_aux/strings.py
+drwxrwxrwx   0        0        0        0 2024-05-16 09:01:22.969617 funcs_aux-0.1.4/funcs_aux.egg-info/
+-rw-rw-rw-   0        0        0     1883 2024-05-16 09:01:22.000000 funcs_aux-0.1.4/funcs_aux.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      297 2024-05-16 09:01:22.000000 funcs_aux-0.1.4/funcs_aux.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 09:01:22.000000 funcs_aux-0.1.4/funcs_aux.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-05-16 09:01:22.000000 funcs_aux-0.1.4/funcs_aux.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-16 09:01:22.971678 funcs_aux-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     2184 2024-01-30 14:09:01.000000 funcs_aux-0.1.4/setup.py
```

### Comparing `funcs_aux-0.1.3/LICENSE` & `funcs_aux-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `funcs_aux-0.1.3/PKG-INFO` & `funcs_aux-0.1.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funcs_aux
-Version: 0.1.3
+Version: 0.1.4
 Summary: useful funcs in one place
 Home-page: https://github.com/centroid457/
 Author: Andrei Starichenko
 Author-email: centroid@mail.ru
 Project-URL: Source, https://github.com/centroid457/funcs_aux
 Keywords: functions,auxiliary,auxiliary funcs,np funcs,collections funcs,strings funcs,result object
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -16,15 +16,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Typing :: Typed
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# funcs_aux (v0.1.3)
+# funcs_aux (v0.1.4)
 
 ## DESCRIPTION_SHORT
 useful funcs in one place
 
 ## DESCRIPTION_LONG
 Now its just a beginning!
 Designed to collect useful funcs in one place!
```

### Comparing `funcs_aux-0.1.3/README.md` & `funcs_aux-0.1.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# funcs_aux (v0.1.3)
+# funcs_aux (v0.1.4)
 
 ## DESCRIPTION_SHORT
 useful funcs in one place
 
 ## DESCRIPTION_LONG
 Now its just a beginning!
 Designed to collect useful funcs in one place!
```

### Comparing `funcs_aux-0.1.3/funcs_aux/arrays.py` & `funcs_aux-0.1.4/funcs_aux/arrays.py`

 * *Files identical despite different names*

### Comparing `funcs_aux-0.1.3/funcs_aux/collects.py` & `funcs_aux-0.1.4/funcs_aux/collects.py`

 * *Files identical despite different names*

### Comparing `funcs_aux-0.1.3/funcs_aux/iterables.py` & `funcs_aux-0.1.4/funcs_aux/iterables.py`

 * *Files identical despite different names*

### Comparing `funcs_aux-0.1.3/funcs_aux/results.py` & `funcs_aux-0.1.4/funcs_aux/results.py`

 * *Files 4% similar despite different names*

```diff
@@ -151,15 +151,15 @@
     def func():
         return Cls.hello5  # this is OK!!!!
 
     # func()      # AttributeError: type object 'Cls' has no attribute 'hello5'
 
 
 # =====================================================================================================================
-class _ResultExpect_Base:
+class ResultExpect_Base:    # dont hide it cause of need ability to detect both of ResultExpect_Step/Chain
     TITLE: Optional[str] = None
 
     ARGS: TYPE__ARGS = None
     KWARGS: TYPE__KWARGS = None
 
     # markers for CHAIN -----------------------
     CHAIN__USE_RESULT: bool = True
@@ -169,42 +169,54 @@
     STEP__RESULT: Optional[bool] = None
     STEP__EXX: Optional[bool] = None
 
     STEP__INDEX: int = None
 
     def __init__(
             self,
-            # _ResultExpect_Base ---------------------
+            # ResultExpect_Base ---------------------
             title: Optional[str] = None,
 
             args: TYPE__ARGS = None,
             kwargs: TYPE__KWARGS = None,
 
             chain__use_result: bool = True,
             chain__stop_on_fail: bool = True,
     ):
-        # _ResultExpect_Base ---------------------
+        # ResultExpect_Base ---------------------
         self.TITLE = title
 
         self.ARGS = args or ()
         self.KWARGS = kwargs or {}
 
         self.CHAIN__USE_RESULT = chain__use_result
         self.CHAIN__STOP_ON_FAIL = chain__stop_on_fail
 
     def __call__(self, *args, **kwargs) -> Self:
         return self.run(*args, **kwargs)
 
+    def __bool__(self):
+        return self.STEP__RESULT
+
+    def __str__(self) -> str:
+        return "\n".join(self.MSGS)
+
     @property
     def MSG(self) -> str:
-        result = f"ResultExpect[result={self.STEP__RESULT}/title={self.TITLE or ''}/index={self.STEP__INDEX}]"
+        result = f"ResultExpect[index={self.STEP__INDEX}/result={self.STEP__RESULT}//title={self.TITLE}]"
         return result
 
+    @property
+    def MSGS(self) -> list[str]:
+        """here it is useful to keep universal access to MSGS both to STEP/CHAIN
+        """
+        return [self.MSG, ]
+
     def _result__clear(self) -> None:
-        self.STEP__RESULT = False
+        self.STEP__RESULT = None
         self.STEP__EXX = None
 
     def run(self, *args, **kwargs) -> bool:
         self._result__clear()
 
         if args:
             self.ARGS = args
@@ -220,15 +232,16 @@
         print(self.MSG)
         return self.STEP__RESULT
 
     def _run__wrapped(self) -> Union[bool, NoReturn]:
         pass
 
 
-class ResultExpect_Step(_ResultExpect_Base):
+# =====================================================================================================================
+class ResultExpect_Step(ResultExpect_Base):
     # SETTINGS --------------------------------
     VALUE: Union[Any, Callable]
     VALUE_AS_FUNC: bool = True
     VALUE_UNDER_FUNC: TYPE__FUNC_UNDER_VALUE = None
     VALUE_EXPECTED: Union[bool, Any] = True
 
     def __init__(
@@ -261,17 +274,17 @@
         result = value == self.VALUE_EXPECTED
 
         # FINISH --------------------------------------------------------------
         return result
 
 
 # =====================================================================================================================
-class ResultExpect_Chain(_ResultExpect_Base):
+class ResultExpect_Chain(ResultExpect_Base):
     # SETTINGS --------------------------------
-    CHAINS: List[Union[_ResultExpect_Base]] = None
+    CHAINS: List[Union[ResultExpect_Base]] = None
 
     # AUX --------------------------------
     STEP__INDEX: int = -1
 
     def __init__(
             self,
             chains: List[Union[ResultExpect_Step, Self]],
@@ -282,24 +295,31 @@
         self.CHAINS = chains
 
     def _run__wrapped(self) -> bool:
         self.STEP__INDEX = -1
         result = True
         for step in self.CHAINS:
             self.STEP__INDEX += 1
-            if isinstance(step, _ResultExpect_Base):
+            if isinstance(step, ResultExpect_Base):
                 step.STEP__INDEX = self.STEP__INDEX
                 step.run(*self.ARGS, **self.KWARGS)
 
                 if step.CHAIN__USE_RESULT:
                     result &= bool(step.STEP__RESULT)
 
                 if not step.STEP__RESULT and step.CHAIN__STOP_ON_FAIL:
                     break
         return result
 
     @property
     def CHAINS_COUNT(self) -> int:
         return len(self.CHAINS or [])
 
+    @property
+    def MSGS(self) -> list[str]:
+        result = []
+        for step in self.CHAINS:
+            result.append(step.MSG)
+        return result
+
 
 # =====================================================================================================================
```

### Comparing `funcs_aux-0.1.3/funcs_aux/strings.py` & `funcs_aux-0.1.4/funcs_aux/strings.py`

 * *Files identical despite different names*

### Comparing `funcs_aux-0.1.3/funcs_aux.egg-info/PKG-INFO` & `funcs_aux-0.1.4/funcs_aux.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funcs_aux
-Version: 0.1.3
+Version: 0.1.4
 Summary: useful funcs in one place
 Home-page: https://github.com/centroid457/
 Author: Andrei Starichenko
 Author-email: centroid@mail.ru
 Project-URL: Source, https://github.com/centroid457/funcs_aux
 Keywords: functions,auxiliary,auxiliary funcs,np funcs,collections funcs,strings funcs,result object
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -16,15 +16,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Typing :: Typed
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# funcs_aux (v0.1.3)
+# funcs_aux (v0.1.4)
 
 ## DESCRIPTION_SHORT
 useful funcs in one place
 
 ## DESCRIPTION_LONG
 Now its just a beginning!
 Designed to collect useful funcs in one place!
```

### Comparing `funcs_aux-0.1.3/setup.py` & `funcs_aux-0.1.4/setup.py`

 * *Files identical despite different names*

