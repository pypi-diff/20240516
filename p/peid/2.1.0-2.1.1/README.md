# Comparing `tmp/peid-2.1.0.tar.gz` & `tmp/peid-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peid-2.1.0.tar", last modified: Sun Jan 21 00:32:37 2024, max compression
+gzip compressed data, was "peid-2.1.1.tar", last modified: Tue Jan 23 20:52:13 2024, max compression
```

## Comparing `peid-2.1.0.tar` & `peid-2.1.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 00:32:37.823169 peid-2.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 00:32:37.815169 peid-2.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 00:32:37.815169 peid-2.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-01-21 00:32:31.000000 peid-2.1.0/.github/workflows/python-package.yml
--rwxr-xr-x   0 runner    (1001) docker     (127)      825 2024-01-21 00:32:31.000000 peid-2.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-01-21 00:32:31.000000 peid-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    45529 2024-01-21 00:32:37.823169 peid-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3768 2024-01-21 00:32:31.000000 peid-2.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 00:32:37.815169 peid-2.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)    93834 2024-01-21 00:32:31.000000 peid-2.1.0/docs/logo.png
--rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-01-21 00:32:31.000000 peid-2.1.0/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (127)        9 2024-01-21 00:32:31.000000 peid-2.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-21 00:32:37.823169 peid-2.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 00:32:37.815169 peid-2.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 00:32:37.815169 peid-2.1.0/src/peid/
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-01-21 00:32:31.000000 peid-2.1.0/src/peid/VERSION.txt
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-01-21 00:32:31.000000 peid-2.1.0/src/peid/__info__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-01-21 00:32:31.000000 peid-2.1.0/src/peid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8233 2024-01-21 00:32:31.000000 peid-2.1.0/src/peid/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 00:32:37.819169 peid-2.1.0/src/peid/db/
--rw-r--r--   0 runner    (1001) docker     (127)  2267682 2024-01-21 00:32:31.000000 peid-2.1.0/src/peid/db/.userdb_txt.json
--rw-r--r--   0 runner    (1001) docker     (127)     9927 2024-01-21 00:32:31.000000 peid-2.1.0/src/peid/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)  1557966 2024-01-21 00:32:31.000000 peid-2.1.0/src/peid/db/userdb.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2970 2024-01-21 00:32:31.000000 peid-2.1.0/src/peid/pe.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-21 00:32:37.823169 peid-2.1.0/src/peid.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    45529 2024-01-21 00:32:37.000000 peid-2.1.0/src/peid.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-01-21 00:32:37.000000 peid-2.1.0/src/peid.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-21 00:32:37.000000 peid-2.1.0/src/peid.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-01-21 00:32:37.000000 peid-2.1.0/src/peid.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-01-21 00:32:37.000000 peid-2.1.0/src/peid.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-01-21 00:32:37.000000 peid-2.1.0/src/peid.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 20:52:13.409696 peid-2.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 20:52:13.401696 peid-2.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 20:52:13.401696 peid-2.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-01-23 20:52:05.000000 peid-2.1.1/.github/workflows/python-package.yml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      825 2024-01-23 20:52:05.000000 peid-2.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-01-23 20:52:05.000000 peid-2.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    45529 2024-01-23 20:52:13.409696 peid-2.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3768 2024-01-23 20:52:06.000000 peid-2.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 20:52:13.401696 peid-2.1.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)    93834 2024-01-23 20:52:05.000000 peid-2.1.1/docs/logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-01-23 20:52:05.000000 peid-2.1.1/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (127)        9 2024-01-23 20:52:05.000000 peid-2.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-23 20:52:13.409696 peid-2.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 20:52:13.401696 peid-2.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 20:52:13.405696 peid-2.1.1/src/peid/
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-01-23 20:52:05.000000 peid-2.1.1/src/peid/VERSION.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-01-23 20:52:05.000000 peid-2.1.1/src/peid/__info__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2861 2024-01-23 20:52:05.000000 peid-2.1.1/src/peid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8207 2024-01-23 20:52:05.000000 peid-2.1.1/src/peid/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 20:52:13.409696 peid-2.1.1/src/peid/db/
+-rw-r--r--   0 runner    (1001) docker     (127)  2267682 2024-01-23 20:52:05.000000 peid-2.1.1/src/peid/db/.userdb_txt.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9927 2024-01-23 20:52:05.000000 peid-2.1.1/src/peid/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1557966 2024-01-23 20:52:05.000000 peid-2.1.1/src/peid/db/userdb.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3449 2024-01-23 20:52:05.000000 peid-2.1.1/src/peid/pe.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-23 20:52:13.409696 peid-2.1.1/src/peid.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    45529 2024-01-23 20:52:13.000000 peid-2.1.1/src/peid.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-01-23 20:52:13.000000 peid-2.1.1/src/peid.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-23 20:52:13.000000 peid-2.1.1/src/peid.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-01-23 20:52:13.000000 peid-2.1.1/src/peid.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-01-23 20:52:13.000000 peid-2.1.1/src/peid.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-01-23 20:52:13.000000 peid-2.1.1/src/peid.egg-info/top_level.txt
```

### Comparing `peid-2.1.0/.github/workflows/python-package.yml` & `peid-2.1.1/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `peid-2.1.0/.gitignore` & `peid-2.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `peid-2.1.0/LICENSE` & `peid-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `peid-2.1.0/PKG-INFO` & `peid-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peid
-Version: 2.1.0
+Version: 2.1.1
 Summary: Python implementation of the Packed Executable iDentifier (PEiD)
 Author-email: Alexandre D'Hondt <alexandre.dhondt@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `peid-2.1.0/README.md` & `peid-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `peid-2.1.0/docs/logo.png` & `peid-2.1.1/docs/logo.png`

 * *Files identical despite different names*

### Comparing `peid-2.1.0/pyproject.toml` & `peid-2.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `peid-2.1.0/src/peid/__info__.py` & `peid-2.1.1/src/peid/__info__.py`

 * *Files identical despite different names*

### Comparing `peid-2.1.0/src/peid/__init__.py` & `peid-2.1.1/src/peid/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -57,11 +57,13 @@
     
     :param path:    path to the executable file(s)
     :param db:      path to the database
     :param ep_only: consider only entry point signatures
     :return:        return the matching packers
     """
     db, results = SignaturesTree(db, logger=logger), []
+    if logger:
+        logger.debug(f"ep_only={ep_only}, sec_start_only={sec_start_only}, match_all={match_all}")
     for path in paths:
         results.append((path, db.match(path, ep_only, sec_start_only, match_all)))
     return results
```

### Comparing `peid-2.1.0/src/peid/__main__.py` & `peid-2.1.1/src/peid/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,17 +16,16 @@
     examples = "usage examples:\n- " + "\n- ".join(examples)
     return ArgumentParser(description=descr, epilog=examples, formatter_class=RawTextHelpFormatter, add_help=False)
 
 
 def _setup(parser):
     args = parser.parse_args()
     if hasattr(args, "verbose"):
-        logging.basicConfig()
+        logging.basicConfig(level=[logging.INFO, logging.DEBUG][args.verbose])
         args.logger = logging.getLogger("peid")
-        args.logger.setLevel([logging.INFO, logging.DEBUG][args.verbose])
     return args
 
 
 def valid_file(path):
     if not exists(path):
         raise ValueError("input file does not exist")
     return path
@@ -51,20 +50,20 @@
                      help="path to the custom database of signatures (default: None ; use the embedded DB)")
     grp = opt.add_mutually_exclusive_group()
     grp.add_argument("-e", "--ep-only", action="store_false",
                      help="only consider signatures from entry point (default: True)")
     opt.add_argument("-m", "--match-once", action="store_true", help="match only one signature")
     grp.add_argument("-s", "--section-start-only", dest="sec_start_only", action="store_true",
                      help="consider only signatures from section starts (default: False)")
-    opt.add_argument("-v", "--version", action="store_true", help="include the version in the result")
+    opt.add_argument("--version", action="store_true", help="include the version in the result")
     extra = parser.add_argument_group("extra arguments")
     extra.add_argument("-b", "--benchmark", action="store_true",
                        help="enable benchmarking, output in seconds (default: False)")
     extra.add_argument("-h", "--help", action="help", help="show this help message and exit")
-    extra.add_argument("--verbose", action="store_true", help="display debug information (default: False)")
+    extra.add_argument("-v", "--verbose", action="store_true", help="display debug information (default: False)")
     args = _setup(parser)
     # execute the tool
     if args.benchmark:
         t1 = perf_counter()
     results = identify_packer(*args.path, db=args.db, ep_only=args.ep_only, sec_start_only=args.sec_start_only,
                               match_all=not args.match_once, logger=args.logger)
     for pe, r in results:
```

### Comparing `peid-2.1.0/src/peid/db/.userdb_txt.json` & `peid-2.1.1/src/peid/db/.userdb_txt.json`

 * *Files identical despite different names*

### Comparing `peid-2.1.0/src/peid/db/__init__.py` & `peid-2.1.1/src/peid/db/__init__.py`

 * *Files identical despite different names*

### Comparing `peid-2.1.0/src/peid/db/userdb.txt` & `peid-2.1.1/src/peid/db/userdb.txt`

 * *Files identical despite different names*

### Comparing `peid-2.1.0/src/peid/pe.py` & `peid-2.1.1/src/peid/pe.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,21 @@
 # -*- coding: UTF-8 -*-
+import builtins
 from functools import lru_cache, wraps
 from os.path import getsize
 
 
 __all__ = ["PE"]
 
 
+class MalformedPE(ValueError):
+    __module__ = "builtins"
+builtins.MalformedPE = MalformedPE
+
+
 class PE:
     def __init__(self, path, logger=None):
         self.path, self.size, self.logger = path, getsize(path), logger
         self.__fd = f = open(path, "rb")
         # check MZ signature
         if f.read(2) != b"MZ":
             raise OSError("Invalid MZ signature")
@@ -57,17 +63,25 @@
             yield r
     
     @property
     def entrypoint_offset(self):
         # EP is at byte 40 of the PE header (when image file)
         self.__fd.seek(self.pe_offset + 40)
         ep = int.from_bytes(self.__fd.read(4), "little")
+        if self.logger:
+            self.logger.debug(f"Entry point: 0x{ep:08x}")
         for vsize, vaddr, rsize, raddr in self.itersections():
-            if vaddr <= ep < vaddr + rsize:
-                return raddr + ep - vaddr
+            if vaddr <= ep < vaddr + vsize:
+                o = raddr + ep - vaddr
+                if self.logger:
+                    self.logger.debug(f"Entry point offset: {o}")
+                return o
+        self.__fd.seek(0)
+        c = self.__fd.read()
+        raise MalformedPE(f"Entry point (0x{ep:08x}) offset is outside sections (file size: 0x{len(c):08x})")
     
     @property
     def sections_offsets(self):
         f = self.__fd
         # Section Headers Table starts after the Optional Header
         start = self.pe_offset + 24 + self.size_of_opt_header
         f.seek(start)
```

### Comparing `peid-2.1.0/src/peid.egg-info/PKG-INFO` & `peid-2.1.1/src/peid.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peid
-Version: 2.1.0
+Version: 2.1.1
 Summary: Python implementation of the Packed Executable iDentifier (PEiD)
 Author-email: Alexandre D'Hondt <alexandre.dhondt@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

