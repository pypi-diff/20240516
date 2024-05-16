# Comparing `tmp/lk_logger-5.7.0-py3-none-any.whl.zip` & `tmp/lk_logger-5.7.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,30 +1,30 @@
-Zip file size: 42362 bytes, number of entries: 28
--rw-r--r--  2.0 fat      680 b- defN 80-Jan-01 00:00 lk_logger/__init__.py
+Zip file size: 42425 bytes, number of entries: 28
+-rw-r--r--  2.0 fat      955 b- defN 80-Jan-01 00:00 lk_logger/__init__.py
 -rw-r--r--  2.0 fat       34 b- defN 80-Jan-01 00:00 lk_logger/cache/__init__.py
 -rw-r--r--  2.0 fat     6970 b- defN 80-Jan-01 00:00 lk_logger/cache/cache.py
 -rw-r--r--  2.0 fat        0 b- defN 80-Jan-01 00:00 lk_logger/cache/frame.py
 -rw-r--r--  2.0 fat     1875 b- defN 80-Jan-01 00:00 lk_logger/cache/legacy.py
 -rw-r--r--  2.0 fat      762 b- defN 80-Jan-01 00:00 lk_logger/cache/util.py
 -rw-r--r--  2.0 fat     5815 b- defN 80-Jan-01 00:00 lk_logger/config.py
--rw-r--r--  2.0 fat     1169 b- defN 80-Jan-01 00:00 lk_logger/console.py
+-rw-r--r--  2.0 fat     1267 b- defN 80-Jan-01 00:00 lk_logger/console.py
 -rw-r--r--  2.0 fat     4988 b- defN 80-Jan-01 00:00 lk_logger/control.py
 -rw-r--r--  2.0 fat     8992 b- defN 80-Jan-01 00:00 lk_logger/frame_info.py
 -rw-r--r--  2.0 fat    13871 b- defN 80-Jan-01 00:00 lk_logger/logger.py
 -rw-r--r--  2.0 fat    10376 b- defN 80-Jan-01 00:00 lk_logger/markup.py
 -rw-r--r--  2.0 fat    11434 b- defN 80-Jan-01 00:00 lk_logger/message_builder.py
 -rw-r--r--  2.0 fat    11258 b- defN 80-Jan-01 00:00 lk_logger/message_formatter.py
 -rw-r--r--  2.0 fat     4034 b- defN 80-Jan-01 00:00 lk_logger/path_helper.py
--rw-r--r--  2.0 fat     2658 b- defN 80-Jan-01 00:00 lk_logger/pipeline.py
+-rw-r--r--  2.0 fat     2543 b- defN 80-Jan-01 00:00 lk_logger/pipeline.py
 -rw-r--r--  2.0 fat     2690 b- defN 80-Jan-01 00:00 lk_logger/printer.py
 -rw-r--r--  2.0 fat       73 b- defN 80-Jan-01 00:00 lk_logger/scanner/__init__.py
 -rw-r--r--  2.0 fat     6407 b- defN 80-Jan-01 00:00 lk_logger/scanner/analyser.py
 -rw-r--r--  2.0 fat     1164 b- defN 80-Jan-01 00:00 lk_logger/scanner/const.py
 -rw-r--r--  2.0 fat     1780 b- defN 80-Jan-01 00:00 lk_logger/scanner/exceptions.py
 -rw-r--r--  2.0 fat     9728 b- defN 80-Jan-01 00:00 lk_logger/scanner/scanner.py
 -rw-r--r--  2.0 fat     3306 b- defN 80-Jan-01 00:00 lk_logger/scanner/symbols.py
 -rw-r--r--  2.0 fat    19638 b- defN 80-Jan-01 00:00 lk_logger/scanner/text_scanner.py
 -rw-r--r--  2.0 fat      517 b- defN 80-Jan-01 00:00 lk_logger/scanner/typehint.py
--rw-r--r--  2.0 fat     4952 b- defN 80-Jan-01 00:00 lk_logger-5.7.0.dist-info/METADATA
--rw-r--r--  2.0 fat       88 b- defN 80-Jan-01 00:00 lk_logger-5.7.0.dist-info/WHEEL
-?rw-r--r--  2.0 fat     2252 b- defN 16-Jan-01 00:00 lk_logger-5.7.0.dist-info/RECORD
-28 files, 137511 bytes uncompressed, 38778 bytes compressed:  71.8%
+-rw-r--r--  2.0 fat     4952 b- defN 80-Jan-01 00:00 lk_logger-5.7.1.dist-info/METADATA
+-rw-r--r--  2.0 fat       88 b- defN 80-Jan-01 00:00 lk_logger-5.7.1.dist-info/WHEEL
+?rw-r--r--  2.0 fat     2252 b- defN 16-Jan-01 00:00 lk_logger-5.7.1.dist-info/RECORD
+28 files, 137769 bytes uncompressed, 38841 bytes compressed:  71.8%
```

## zipnote {}

```diff
@@ -69,17 +69,17 @@
 
 Filename: lk_logger/scanner/text_scanner.py
 Comment: 
 
 Filename: lk_logger/scanner/typehint.py
 Comment: 
 
-Filename: lk_logger-5.7.0.dist-info/METADATA
+Filename: lk_logger-5.7.1.dist-info/METADATA
 Comment: 
 
-Filename: lk_logger-5.7.0.dist-info/WHEEL
+Filename: lk_logger-5.7.1.dist-info/WHEEL
 Comment: 
 
-Filename: lk_logger-5.7.0.dist-info/RECORD
+Filename: lk_logger-5.7.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## lk_logger/__init__.py

```diff
@@ -12,15 +12,26 @@
 from .frame_info import FrameInfo
 from .logger import logger
 from .pipeline import pipeline
 from .printer import bprint
 from .printer import parallel_printing
 
 
-# def __init() -> None:
-#     import traceback
-#     pipeline.add(traceback, bprint)
-#     setup(quiet=True)
-#
-#
-# __init()
-__version__ = '5.7.0'
+def __init() -> None:
+    # import traceback
+    # pipeline.add(traceback, bprint)
+    # setup(quiet=True)
+    
+    # from .printer import dprint
+    # dprint(f'{__IPYTHON__=}')
+    try:
+        __IPYTHON__  # noqa
+    except NameError:
+        pass
+    else:
+        import IPython
+        pipeline.add(IPython, bprint, scope=True)
+        # pipeline.add('[ipython]', bprint)
+
+
+__init()
+__version__ = '5.7.1'
```

## lk_logger/console.py

```diff
@@ -21,13 +21,17 @@
         #   if width longer than default, use single line style; otherwise
         #   split sourcemap and message into different lines.
         pass
     
     def print(self, *objects: Any, soft_wrap: bool = True, **kwargs) -> None:
         from .message_builder import MessageStruct
         if len(objects) == 1 and isinstance(objects[0], MessageStruct):
-            super().print(objects[0].text, soft_wrap=soft_wrap, **kwargs)
+            super().print(
+                objects[0].text, overflow='fold', soft_wrap=soft_wrap, **kwargs
+            )
         else:
-            super().print(*objects, soft_wrap=soft_wrap, **kwargs)
+            super().print(
+                *objects, overflow='fold', soft_wrap=soft_wrap, **kwargs
+            )
 
 
 console = Console()
```

## lk_logger/pipeline.py

```diff
@@ -1,16 +1,14 @@
-from __future__ import annotations
-
 import typing as t
 from os import name as _os_name
 from os.path import abspath
 from os.path import dirname
 
-from .printer import bprint
-# from .printer import dprint
+from .printer import non_print
+from .printer import std_print
 
 
 class T:
     PrintFunc = t.Optional[t.Callable]
     Cache = t.Dict[str, PrintFunc]
     PipeLines = t.NamedTuple('PipeLines2', (
         ('abspath', t.Dict[str, PrintFunc]),
@@ -23,39 +21,41 @@
     '''
 
 
 class Pipeline:
     _cache: T.Cache
     _lines: T.PipeLines
     
-    def __init__(self):
+    def __init__(self) -> None:
         self._cache = {}
         self._lines = T.PipeLines({}, {})
     
     def dump_list(self) -> t.List[str]:
         return list(self._lines.abspath.keys())
     
-    def add(self,
-            x: t.Union[str, object],
-            prt: t.Optional[t.Callable] = bprint,
-            scope=False) -> None:
+    def add(
+        self,
+        x: t.Union[str, object],
+        prt: t.Optional[t.Callable] = std_print,
+        scope: bool = False
+    ) -> None:
         if isinstance(x, str):
             if x.startswith('['):
                 path = x
             else:
                 path = _normpath(x)
         else:
             # x is a package or a module
             # dprint(x, x.__file__)
             path = _normpath(x.__file__)
             if scope:
                 path = dirname(path)
         # dprint('add path to pipeline', path)
         if prt is None:
-            prt = _mute_print
+            prt = non_print
         if path.startswith('['):
             self._lines.libname[path] = prt
         else:
             self._lines.abspath[path] = prt
         self._cache[path] = prt
     
     def get(self, path: str) -> T.PrintFunc:
@@ -73,25 +73,18 @@
                 self._cache[path] = prt
                 # dprint('use custom print', path)
                 return prt
         self._cache[path] = None
         return None
 
 
-class _MutePrint:
-    def __call__(self, *_, **__):
-        pass
-
-
-_mute_print = _MutePrint()
-
-_is_win = _os_name == 'nt'
+_IS_WIN = _os_name == 'nt'
 
 
 def _normpath(path: str) -> str:
     path = abspath(path)
-    if _is_win:
+    if _IS_WIN:
         path = path.replace('\\', '/')
     return path
 
 
 pipeline = Pipeline()
```

## Comparing `lk_logger-5.7.0.dist-info/METADATA` & `lk_logger-5.7.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lk-logger
-Version: 5.7.0
+Version: 5.7.1
 Summary: Python print with source and varnames.
 Home-page: https://github.com/likianta/lk-logger
 License: MIT
 Author: Likianta
 Author-email: likianta@foxmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

## Comparing `lk_logger-5.7.0.dist-info/RECORD` & `lk_logger-5.7.1.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-lk_logger/__init__.py,sha256=x7IpyoD9eNBYN6b45Nea9Rl--gf5nt1JfOBmpDUU6ZE,680
+lk_logger/__init__.py,sha256=U_xd3o1OGBfzqsZ397z3wc-wSGqssnn4SAduPlWyxVw,955
 lk_logger/cache/__init__.py,sha256=jkWi40WfmTt3Akv3YKjJHI6gxPqzXwpFmdF4bIJ-SUs,34
 lk_logger/cache/cache.py,sha256=b2zusDBHjbAVtoP8CdBedPvkujVjNosUNlsUiCPSJeY,6970
 lk_logger/cache/frame.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 lk_logger/cache/legacy.py,sha256=kuQrFzJGuTd_NQWrO5Vp6b-Da3X73w60Ae2LxVP3Xb8,1875
 lk_logger/cache/util.py,sha256=6qtnnIhdrKTqyP4Elxd1d3OnkTFROzxAGWYz3c4smDk,762
 lk_logger/config.py,sha256=jIB5tc1Eqke8_TGrCiropibesY5dBvyHzur_FtKOYdA,5815
-lk_logger/console.py,sha256=2iDM02xilIILLhjhf7zyp8pYb-SwokCs2HY54EtFsnE,1169
+lk_logger/console.py,sha256=xV0C65Bv4BZ7R7mQgDZNjhmZdV3d0Y5w_n4WP1aAQHE,1267
 lk_logger/control.py,sha256=60G6mzfj7TH6BL07BTzz5ShrzhbUXJpTcZYt2_fvVSE,4988
 lk_logger/frame_info.py,sha256=MFeZoRq8ou5-5m77N40xOO3ADOxNMdWRcn4-EUouQqA,8992
 lk_logger/logger.py,sha256=EMLUj3h6C5d4Vj423GBhB5lvGAdLTt_pA1ebvq2GBD0,13871
 lk_logger/markup.py,sha256=WkIaQIRDwUyYZFY-Jn22qc-Ig7fJyx6V6jYawZcnnYQ,10376
 lk_logger/message_builder.py,sha256=--BtpkikTZXdEbZm1_-dJSxhAiE1E20GWpIIgSm5Nzc,11434
 lk_logger/message_formatter.py,sha256=lpv_rB616EmHLqYaYt7SirNIndvAdbPD9H1ZWrLthbQ,11258
 lk_logger/path_helper.py,sha256=LAZOe5XK_51I0YPA6rUuY0_DKtaMtHyz52xcHqRbxY0,4034
-lk_logger/pipeline.py,sha256=qhgbvYUYLot6aCNMiRZRTtWrXrwWlh1y49uLrGQui9w,2658
+lk_logger/pipeline.py,sha256=V6gWLV_qhb1TNteLqugQ__qWEWPmxYQAj4hVYxX8Yyo,2543
 lk_logger/printer.py,sha256=X9baNbtuLRLK3R43CNbcyvJTA7e6cyXa2b_zDXuNxTQ,2690
 lk_logger/scanner/__init__.py,sha256=2b0jy5SdPwiVQSV9kL_3Vd4AkbKrRp7npAUWC3Hbyek,73
 lk_logger/scanner/analyser.py,sha256=y3HuYB2DJ4ixwww4c9o6Jq6mPc2eqz88w5Cf84_Pf6E,6407
 lk_logger/scanner/const.py,sha256=npj77J2VntzHArQOaIUIj9IeRQi9hH33_lo2XYLlg-s,1164
 lk_logger/scanner/exceptions.py,sha256=G1wpgEIzTLLrD6Q_m0qGD85v5KnlPm3CV1ZxgvGCVd8,1780
 lk_logger/scanner/scanner.py,sha256=I9tf-ELQOLgZxWM5YNCEP5FvW5JkmIhfVEdhezXGz4M,9728
 lk_logger/scanner/symbols.py,sha256=FhLqVbYRG-a72ZoVgriP4FKmAhweyeyh02IkiLymT2I,3306
 lk_logger/scanner/text_scanner.py,sha256=84ese30Bh-H1ZVxT0jcNhsTwM1nLDkZOrUO1LSdjV6k,19638
 lk_logger/scanner/typehint.py,sha256=CdX-02JvaI8PkEHgTN279e081njEAfNOHaxPXCQkguc,517
-lk_logger-5.7.0.dist-info/METADATA,sha256=9YTOj4QYufaG4jH1fFL7a5xZC1_bNyMjfBeeYZj3K74,4952
-lk_logger-5.7.0.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
-lk_logger-5.7.0.dist-info/RECORD,,
+lk_logger-5.7.1.dist-info/METADATA,sha256=_DiYe02jr9mhg4rCqzwu7eyjsLrNxfuC0Bo3zfmPKxE,4952
+lk_logger-5.7.1.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
+lk_logger-5.7.1.dist-info/RECORD,,
```

