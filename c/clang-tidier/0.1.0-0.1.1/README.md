# Comparing `tmp/clang_tidier-0.1.0.tar.gz` & `tmp/clang_tidier-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clang_tidier-0.1.0.tar", last modified: Thu May  9 19:40:33 2024, max compression
+gzip compressed data, was "clang_tidier-0.1.1.tar", last modified: Thu May 16 14:52:32 2024, max compression
```

## Comparing `clang_tidier-0.1.0.tar` & `clang_tidier-0.1.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-05-09 19:40:33.726882 clang_tidier-0.1.0/
--rw-rw-rw-   0        0        0       62 2024-05-09 12:13:25.000000 clang_tidier-0.1.0/CHANGELOG.md
--rw-rw-rw-   0        0        0     1064 2024-01-10 12:56:54.000000 clang_tidier-0.1.0/LICENSE.txt
--rw-rw-rw-   0        0        0     2584 2024-05-09 19:40:33.725881 clang_tidier-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1457 2024-05-09 19:39:23.000000 clang_tidier-0.1.0/README.md
--rw-rw-rw-   0        0        0     2008 2024-05-09 15:35:18.000000 clang_tidier-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-09 19:40:33.726882 clang_tidier-0.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-09 19:40:33.707882 clang_tidier-0.1.0/src/
-drwxrwxrwx   0        0        0        0 2024-05-09 19:40:33.716881 clang_tidier-0.1.0/src/clang_tidier/
--rw-rw-rw-   0        0        0      491 2024-05-09 15:34:59.000000 clang_tidier-0.1.0/src/clang_tidier/__init__.py
--rw-rw-rw-   0        0        0      899 2024-05-09 15:34:59.000000 clang_tidier-0.1.0/src/clang_tidier/colour.py
--rw-rw-rw-   0        0        0    14005 2024-05-09 19:24:21.000000 clang_tidier-0.1.0/src/clang_tidier/main.py
--rw-rw-rw-   0        0        0      873 2024-05-09 15:34:59.000000 clang_tidier-0.1.0/src/clang_tidier/paths.py
--rw-rw-rw-   0        0        0      601 2024-05-09 15:34:59.000000 clang_tidier-0.1.0/src/clang_tidier/version.py
--rw-rw-rw-   0        0        0        6 2024-05-09 14:57:05.000000 clang_tidier-0.1.0/src/clang_tidier/version.txt
-drwxrwxrwx   0        0        0        0 2024-05-09 19:40:33.724883 clang_tidier-0.1.0/src/clang_tidier.egg-info/
--rw-rw-rw-   0        0        0     2584 2024-05-09 19:40:33.000000 clang_tidier-0.1.0/src/clang_tidier.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      519 2024-05-09 19:40:33.000000 clang_tidier-0.1.0/src/clang_tidier.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 19:40:33.000000 clang_tidier-0.1.0/src/clang_tidier.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       84 2024-05-09 19:40:33.000000 clang_tidier-0.1.0/src/clang_tidier.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       21 2024-05-09 19:40:33.000000 clang_tidier-0.1.0/src/clang_tidier.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-09 19:40:33.000000 clang_tidier-0.1.0/src/clang_tidier.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        1 2024-05-09 15:40:44.000000 clang_tidier-0.1.0/src/clang_tidier.egg-info/zip-safe
+drwxrwxrwx   0        0        0        0 2024-05-16 14:52:32.511680 clang_tidier-0.1.1/
+-rw-rw-rw-   0        0        0      176 2024-05-16 14:41:06.000000 clang_tidier-0.1.1/CHANGELOG.md
+-rw-rw-rw-   0        0        0     1064 2024-01-10 12:56:54.000000 clang_tidier-0.1.1/LICENSE.txt
+-rw-rw-rw-   0        0        0     2702 2024-05-16 14:52:32.511680 clang_tidier-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1457 2024-05-09 19:39:23.000000 clang_tidier-0.1.1/README.md
+-rw-rw-rw-   0        0        0     2008 2024-05-09 15:35:18.000000 clang_tidier-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-16 14:52:32.511680 clang_tidier-0.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-16 14:52:32.496992 clang_tidier-0.1.1/src/
+drwxrwxrwx   0        0        0        0 2024-05-16 14:52:32.505118 clang_tidier-0.1.1/src/clang_tidier/
+-rw-rw-rw-   0        0        0      491 2024-05-09 15:34:59.000000 clang_tidier-0.1.1/src/clang_tidier/__init__.py
+-rw-rw-rw-   0        0        0      899 2024-05-09 15:34:59.000000 clang_tidier-0.1.1/src/clang_tidier/colour.py
+-rw-rw-rw-   0        0        0    15661 2024-05-16 14:39:57.000000 clang_tidier-0.1.1/src/clang_tidier/main.py
+-rw-rw-rw-   0        0        0      873 2024-05-09 15:34:59.000000 clang_tidier-0.1.1/src/clang_tidier/paths.py
+-rw-rw-rw-   0        0        0      601 2024-05-09 15:34:59.000000 clang_tidier-0.1.1/src/clang_tidier/version.py
+-rw-rw-rw-   0        0        0        6 2024-05-16 14:40:00.000000 clang_tidier-0.1.1/src/clang_tidier/version.txt
+drwxrwxrwx   0        0        0        0 2024-05-16 14:52:32.511680 clang_tidier-0.1.1/src/clang_tidier.egg-info/
+-rw-rw-rw-   0        0        0     2702 2024-05-16 14:52:32.000000 clang_tidier-0.1.1/src/clang_tidier.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      519 2024-05-16 14:52:32.000000 clang_tidier-0.1.1/src/clang_tidier.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 14:52:32.000000 clang_tidier-0.1.1/src/clang_tidier.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       84 2024-05-16 14:52:32.000000 clang_tidier-0.1.1/src/clang_tidier.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       21 2024-05-16 14:52:32.000000 clang_tidier-0.1.1/src/clang_tidier.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-16 14:52:32.000000 clang_tidier-0.1.1/src/clang_tidier.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        1 2024-05-09 15:40:44.000000 clang_tidier-0.1.1/src/clang_tidier.egg-info/zip-safe
```

### Comparing `clang_tidier-0.1.0/LICENSE.txt` & `clang_tidier-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `clang_tidier-0.1.0/PKG-INFO` & `clang_tidier-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clang-tidier
-Version: 0.1.0
+Version: 0.1.1
 Summary: A simple runner for clang-tidy.
 Author-email: Mark Gillard <mark.gillard@outlook.com.au>
 License: MIT
 Project-URL: Source, https://github.com/marzer/clang-tidier
 Project-URL: Tracker, https://github.com/marzer/clang-tidier/issues
 Project-URL: Funding, https://github.com/sponsors/marzer
 Keywords: c++,clang-tidy
@@ -68,10 +68,14 @@
 | 0                                    | No issues were found   |
 | `N`, where `N` is a positive integer | `N` issues were found  |
 | -1                                   | A fatal error occurred |
 
 
 # Changelog
 
-## v0.1.0
+## v0.1.1 - 2024/05/16
+
+-   Fixed issues with older clang-tidy versions trying to use `--use-color`
+
+## v0.1.0 - 2024/05/09
 
 -   First public release 🎉&#xFE0F;
```

### Comparing `clang_tidier-0.1.0/README.md` & `clang_tidier-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `clang_tidier-0.1.0/pyproject.toml` & `clang_tidier-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `clang_tidier-0.1.0/src/clang_tidier/colour.py` & `clang_tidier-0.1.1/src/clang_tidier/colour.py`

 * *Files identical despite different names*

### Comparing `clang_tidier-0.1.0/src/clang_tidier/main.py` & `clang_tidier-0.1.1/src/clang_tidier/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,27 +11,29 @@
 import signal
 import subprocess
 import sys
 import misk
 import json
 import os
 import concurrent.futures as futures
+from typing import Tuple
 from io import StringIO
 from pathlib import Path
 
 import colorama
 
 from . import paths
 from .colour import *
 from .version import *
 
 IS_WORKER = False
 STOP = None
 FATAL_ERROR = None
 PROBLEMATIC_FILE_COUNT = None
+ANSI_ESCAPE_CODES = re.compile(r'(?:\x1B[@-_]|[\x80-\x9F])[0-?]*[ -/]*[@-~]')
 
 
 def error(text):
     print(rf"{bright(rf'error:', 'red')} {text}", file=sys.stderr)
 
 
 def sigint_handler(signal, frame):
@@ -44,18 +46,24 @@
 
 def initialize_worker():
     global IS_WORKER
     IS_WORKER = True
     signal.signal(signal.SIGINT, sigint_handler)
 
 
-def clean_clang_tidy_output(s):
+def clean_clang_tidy_output(s: str):
     if s is None:
         return ''
 
+    # fix windows nonsense
+    s = str(s).replace("\r\n", "\n")
+
+    # strip away ansi nonsense
+    s = ANSI_ESCAPE_CODES.sub('', s)
+
     # strip "XXXXXX warnings/errors generated."
     s = re.sub(r'[0-9]+ (?:warning|error)s? (?:and [0-9]+ (?:warning|error)s? )?generated[.]?', r'', s)
 
     # strip "error while processing XXXXXXX"
     s = re.sub(r'[Ee]rror while processing [./a-zA-Z0-9_+-]+[.]', r'', s)
 
     return s.strip()
@@ -84,35 +92,37 @@
     relative_to = misk.coerce_path(relative_to).resolve()
     try:
         return Path(os.path.relpath(str(p), str(relative_to)))
     except:
         return p
 
 
-def worker(clang_tidy, compile_db: Path, werror: bool, src_file: Path):
+def worker(
+    clang_tidy_exe: str, clang_tidy_version: Tuple[int, int, int], compile_db: Path, werror: bool, src_file: Path
+):
     global STOP
     global FATAL_ERROR
     global PROBLEMATIC_FILE_COUNT
     if STOP.is_set():
         return
 
     assert src_file is not None
     try:
         src_file = misk.coerce_path(src_file).resolve()
 
         proc = subprocess.run(
             [
-                clang_tidy,
+                clang_tidy_exe,
                 rf'-p={compile_db}',
                 '--quiet',
                 '--warnings-as-errors=-*',  # none
-                '--use-color=false',
                 '--extra-arg=-D__clang_tidy__',
-                src_file,
-            ],
+            ]
+            + (['--use-color=false'] if clang_tidy_version[0] >= 12 else [])
+            + [src_file],
             cwd=str(Path.cwd()),
             encoding='utf-8',
             capture_output=True,
             check=False,
         )
 
         def find_error(s):
@@ -277,24 +287,51 @@
     for filter in args.exclude:
         sources = [s for s in sources if not re.search(filter, str(s))]
     if not sources:
         print("no work to do.")
         return 0
 
     # detect clang-tidy
-    clang_tidy = 'clang-tidy'
+    clang_tidy_exe = 'clang-tidy'
+    clang_tidy_label = clang_tidy_exe
+    clang_tidy_version = (0, 0, 0)
     if not shutil.which('clang-tidy'):
-        clang_tidy = None
+        clang_tidy_exe = None
         for i in range(20, 6, -1):
             if shutil.which(rf'clang-tidy-{i}'):
-                clang_tidy = rf'clang-tidy-{i}'
+                clang_tidy_exe = rf'clang-tidy-{i}'
+                clang_tidy_label = clang_tidy_exe
+                clang_tidy_version = (i, 0, 0)
                 break
-    if clang_tidy is None:
+    if clang_tidy_exe is None:
         return rf"could not detect {bright('clang-tidy')}"
 
+    # query the actual version
+    try:
+        clang_tidy_version_output = clean_clang_tidy_output(
+            subprocess.run(
+                [clang_tidy_exe, '--version'], cwd=str(Path.cwd()), encoding='utf-8', capture_output=True
+            ).stdout
+        )
+        clang_tidy_version_output = re.search(
+            r'\b[vV]?([0-9]+?)[.]([0-9]+?)(?:[.]([0-9]+?))?\b', clang_tidy_version_output
+        )
+        if clang_tidy_version_output is not None:
+            clang_tidy_version = (
+                int(clang_tidy_version_output[1]),
+                int(clang_tidy_version_output[2]),
+                int(clang_tidy_version_output[3]) if clang_tidy_version_output[3] is not None else 0,
+            )
+            print(
+                rf"detected {bright(rf'clang-tidy v{clang_tidy_version[0]}.{clang_tidy_version[1]}.{clang_tidy_version[2]}')}"
+            )
+            clang_tidy_label = rf'clang-tidy-{clang_tidy_version[0]}'
+    except:
+        pass  # a failure here doesn't really matter, it's just for finer-grained version checking
+
     # detect git + filter out gitignored files
     if find_upwards(".git", files=False, directories=True, start_dir=args.compile_db.parent) is not None:
         if shutil.which('git') is not None:
             gitignored_sources = set()
             for source in sources:
                 if (
                     subprocess.run(
@@ -321,19 +358,22 @@
     # run clang-tidy on each file
     global STOP
     global FATAL_ERROR
     global PROBLEMATIC_FILE_COUNT
     STOP = multiprocessing.Event()
     FATAL_ERROR = multiprocessing.Event()
     PROBLEMATIC_FILE_COUNT = multiprocessing.Value('i', 0)
-    print(rf'running {bright(clang_tidy)} on {len(sources)} file{"s" if len(sources) > 1 else ""}')
+    print(rf'running {bright(clang_tidy_label)} on {len(sources)} file{"s" if len(sources) > 1 else ""}')
     with futures.ProcessPoolExecutor(
         max_workers=max(min(os.cpu_count(), len(sources), args.threads), 1), initializer=initialize_worker
     ) as executor:
-        jobs = [executor.submit(worker, clang_tidy, args.compile_db, args.werror, f) for f in sources]
+        jobs = [
+            executor.submit(worker, clang_tidy_exe, clang_tidy_version, args.compile_db, args.werror, f)
+            for f in sources
+        ]
         for future in futures.as_completed(jobs):
             if STOP.is_set():
                 future.cancel()
                 continue
             try:
                 future.result()
             except Exception as exc:
@@ -347,15 +387,15 @@
                     FATAL_ERROR.set()
                     raise
 
     if FATAL_ERROR.is_set():
         return r'An error occurred.'
     with PROBLEMATIC_FILE_COUNT.get_lock():
         if PROBLEMATIC_FILE_COUNT.value:
-            print(rf'{bright(clang_tidy)} found problems in {PROBLEMATIC_FILE_COUNT.value} file(s).')
+            print(rf'{bright(clang_tidy_label)} found problems in {PROBLEMATIC_FILE_COUNT.value} file(s).')
             return int(PROBLEMATIC_FILE_COUNT.value)
     return 0
 
 
 def main():
     signal.signal(signal.SIGINT, sigint_handler)
     colorama.init()
```

### Comparing `clang_tidier-0.1.0/src/clang_tidier/paths.py` & `clang_tidier-0.1.1/src/clang_tidier/paths.py`

 * *Files identical despite different names*

### Comparing `clang_tidier-0.1.0/src/clang_tidier/version.py` & `clang_tidier-0.1.1/src/clang_tidier/version.py`

 * *Files identical despite different names*

### Comparing `clang_tidier-0.1.0/src/clang_tidier.egg-info/PKG-INFO` & `clang_tidier-0.1.1/src/clang_tidier.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clang-tidier
-Version: 0.1.0
+Version: 0.1.1
 Summary: A simple runner for clang-tidy.
 Author-email: Mark Gillard <mark.gillard@outlook.com.au>
 License: MIT
 Project-URL: Source, https://github.com/marzer/clang-tidier
 Project-URL: Tracker, https://github.com/marzer/clang-tidier/issues
 Project-URL: Funding, https://github.com/sponsors/marzer
 Keywords: c++,clang-tidy
@@ -68,10 +68,14 @@
 | 0                                    | No issues were found   |
 | `N`, where `N` is a positive integer | `N` issues were found  |
 | -1                                   | A fatal error occurred |
 
 
 # Changelog
 
-## v0.1.0
+## v0.1.1 - 2024/05/16
+
+-   Fixed issues with older clang-tidy versions trying to use `--use-color`
+
+## v0.1.0 - 2024/05/09
 
 -   First public release 🎉&#xFE0F;
```

### Comparing `clang_tidier-0.1.0/src/clang_tidier.egg-info/SOURCES.txt` & `clang_tidier-0.1.1/src/clang_tidier.egg-info/SOURCES.txt`

 * *Files identical despite different names*

