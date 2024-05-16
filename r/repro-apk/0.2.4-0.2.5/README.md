# Comparing `tmp/repro-apk-0.2.4.tar.gz` & `tmp/repro-apk-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "repro-apk-0.2.4.tar", last modified: Sat Mar  9 01:23:13 2024, max compression
+gzip compressed data, was "repro-apk-0.2.5.tar", last modified: Thu Mar 21 15:40:08 2024, max compression
```

## Comparing `repro-apk-0.2.4.tar` & `repro-apk-0.2.5.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwx------   0 fay       (1000) fay       (1000)        0 2024-03-09 01:23:13.484805 repro-apk-0.2.4/
--rw-------   0 fay       (1000) fay       (1000)       23 2022-11-22 04:03:59.000000 repro-apk-0.2.4/.flake8
--rw-------   0 fay       (1000) fay       (1000)       73 2023-02-12 10:27:38.000000 repro-apk-0.2.4/.gitignore
--rw-------   0 fay       (1000) fay       (1000)      140 2023-02-24 17:05:00.000000 repro-apk-0.2.4/.pylintrc
--rw-------   0 fay       (1000) fay       (1000)    35149 2022-11-22 04:08:35.000000 repro-apk-0.2.4/LICENSE.GPLv3
--rw-------   0 fay       (1000) fay       (1000)      139 2024-03-09 01:21:04.000000 repro-apk-0.2.4/MANIFEST.in
--rw-------   0 fay       (1000) fay       (1000)     8561 2024-03-09 00:53:30.000000 repro-apk-0.2.4/Makefile
--rw-------   0 fay       (1000) fay       (1000)    27617 2024-03-09 01:23:13.484805 repro-apk-0.2.4/PKG-INFO
--rw-------   0 fay       (1000) fay       (1000)    26193 2024-03-09 00:53:30.000000 repro-apk-0.2.4/README.md
--rw-------   0 fay       (1000) fay       (1000)     1213 2024-03-09 01:06:45.000000 repro-apk-0.2.4/changelog.txt
-drwx------   0 fay       (1000) fay       (1000)        0 2024-03-09 01:23:13.484805 repro-apk-0.2.4/repro_apk/
--rw-------   0 fay       (1000) fay       (1000)    13117 2024-03-09 01:05:18.000000 repro-apk-0.2.4/repro_apk/__init__.py
--rwx------   0 fay       (1000) fay       (1000)    14505 2024-03-08 21:41:56.000000 repro-apk-0.2.4/repro_apk/diff_zip_meta.py
--rwx------   0 fay       (1000) fay       (1000)     5546 2023-01-15 20:09:06.000000 repro-apk-0.2.4/repro_apk/dump_arsc.py
--rwx------   0 fay       (1000) fay       (1000)     5536 2023-02-16 18:36:33.000000 repro-apk-0.2.4/repro_apk/dump_axml.py
--rwx------   0 fay       (1000) fay       (1000)    11653 2023-01-15 20:09:06.000000 repro-apk-0.2.4/repro_apk/dump_baseline.py
--rwx------   0 fay       (1000) fay       (1000)     5946 2023-02-19 23:11:34.000000 repro-apk-0.2.4/repro_apk/fix_compresslevel.py
--rwx------   0 fay       (1000) fay       (1000)     6405 2023-02-19 23:16:37.000000 repro-apk-0.2.4/repro_apk/fix_files.py
--rwx------   0 fay       (1000) fay       (1000)     6799 2023-02-24 18:06:03.000000 repro-apk-0.2.4/repro_apk/fix_newlines.py
--rwx------   0 fay       (1000) fay       (1000)     7303 2024-03-07 01:24:01.000000 repro-apk-0.2.4/repro_apk/inplace_fix.py
--rwx------   0 fay       (1000) fay       (1000)     3478 2023-02-19 23:18:24.000000 repro-apk-0.2.4/repro_apk/list_compresslevel.py
--rw-------   0 fay       (1000) fay       (1000)        0 2022-11-22 16:14:18.000000 repro-apk-0.2.4/repro_apk/py.typed
--rwx------   0 fay       (1000) fay       (1000)     5423 2023-02-19 23:18:39.000000 repro-apk-0.2.4/repro_apk/rm_files.py
--rwx------   0 fay       (1000) fay       (1000)     5511 2023-01-15 20:09:06.000000 repro-apk-0.2.4/repro_apk/sort_apk.py
--rwx------   0 fay       (1000) fay       (1000)     7107 2023-02-16 19:13:57.000000 repro-apk-0.2.4/repro_apk/sort_baseline.py
--rwx------   0 fay       (1000) fay       (1000)     7276 2024-03-07 01:24:01.000000 repro-apk-0.2.4/repro_apk/zipalign.py
--rwx------   0 fay       (1000) fay       (1000)    11965 2024-03-06 17:50:34.000000 repro-apk-0.2.4/repro_apk/zipinfo.py
-drwx------   0 fay       (1000) fay       (1000)        0 2024-03-09 01:23:13.484805 repro-apk-0.2.4/repro_apk.egg-info/
--rw-------   0 fay       (1000) fay       (1000)    27617 2024-03-09 01:23:13.000000 repro-apk-0.2.4/repro_apk.egg-info/PKG-INFO
--rw-------   0 fay       (1000) fay       (1000)      688 2024-03-09 01:23:13.000000 repro-apk-0.2.4/repro_apk.egg-info/SOURCES.txt
--rw-------   0 fay       (1000) fay       (1000)        1 2024-03-09 01:23:13.000000 repro-apk-0.2.4/repro_apk.egg-info/dependency_links.txt
--rw-------   0 fay       (1000) fay       (1000)       96 2024-03-09 01:23:13.000000 repro-apk-0.2.4/repro_apk.egg-info/entry_points.txt
--rw-------   0 fay       (1000) fay       (1000)       11 2024-03-09 01:23:13.000000 repro-apk-0.2.4/repro_apk.egg-info/requires.txt
--rw-------   0 fay       (1000) fay       (1000)       10 2024-03-09 01:23:13.000000 repro-apk-0.2.4/repro_apk.egg-info/top_level.txt
--rw-------   0 fay       (1000) fay       (1000)       38 2024-03-09 01:23:13.484805 repro-apk-0.2.4/setup.cfg
--rw-------   0 fay       (1000) fay       (1000)     1967 2024-03-09 01:05:25.000000 repro-apk-0.2.4/setup.py
+drwx------   0 fay       (1000) fay       (1000)        0 2024-03-21 15:40:08.611009 repro-apk-0.2.5/
+-rw-------   0 fay       (1000) fay       (1000)       23 2022-11-22 04:03:59.000000 repro-apk-0.2.5/.flake8
+-rw-------   0 fay       (1000) fay       (1000)       73 2023-02-12 10:27:38.000000 repro-apk-0.2.5/.gitignore
+-rw-------   0 fay       (1000) fay       (1000)      140 2023-02-24 17:05:00.000000 repro-apk-0.2.5/.pylintrc
+-rw-------   0 fay       (1000) fay       (1000)    35149 2022-11-22 04:08:35.000000 repro-apk-0.2.5/LICENSE.GPLv3
+-rw-------   0 fay       (1000) fay       (1000)      139 2024-03-09 01:34:00.000000 repro-apk-0.2.5/MANIFEST.in
+-rw-------   0 fay       (1000) fay       (1000)     8561 2024-03-21 15:33:34.000000 repro-apk-0.2.5/Makefile
+-rw-------   0 fay       (1000) fay       (1000)    29830 2024-03-21 15:40:08.611009 repro-apk-0.2.5/PKG-INFO
+-rw-------   0 fay       (1000) fay       (1000)    28406 2024-03-21 15:33:34.000000 repro-apk-0.2.5/README.md
+-rw-------   0 fay       (1000) fay       (1000)     1248 2024-03-21 15:35:13.000000 repro-apk-0.2.5/changelog.txt
+drwx------   0 fay       (1000) fay       (1000)        0 2024-03-21 15:40:08.611009 repro-apk-0.2.5/repro_apk/
+-rw-------   0 fay       (1000) fay       (1000)    13879 2024-03-21 15:33:55.000000 repro-apk-0.2.5/repro_apk/__init__.py
+-rwx------   0 fay       (1000) fay       (1000)    14505 2024-03-08 21:41:56.000000 repro-apk-0.2.5/repro_apk/diff_zip_meta.py
+-rwx------   0 fay       (1000) fay       (1000)     5546 2023-01-15 20:09:06.000000 repro-apk-0.2.5/repro_apk/dump_arsc.py
+-rwx------   0 fay       (1000) fay       (1000)     5536 2023-02-16 18:36:33.000000 repro-apk-0.2.5/repro_apk/dump_axml.py
+-rwx------   0 fay       (1000) fay       (1000)    11653 2023-01-15 20:09:06.000000 repro-apk-0.2.5/repro_apk/dump_baseline.py
+-rwx------   0 fay       (1000) fay       (1000)     5946 2023-02-19 23:11:34.000000 repro-apk-0.2.5/repro_apk/fix_compresslevel.py
+-rwx------   0 fay       (1000) fay       (1000)     6405 2023-02-19 23:16:37.000000 repro-apk-0.2.5/repro_apk/fix_files.py
+-rwx------   0 fay       (1000) fay       (1000)     6799 2023-02-24 18:06:03.000000 repro-apk-0.2.5/repro_apk/fix_newlines.py
+-rwx------   0 fay       (1000) fay       (1000)     9606 2024-03-21 04:26:01.000000 repro-apk-0.2.5/repro_apk/fix_pg_map_id.py
+-rwx------   0 fay       (1000) fay       (1000)     7324 2024-03-21 04:26:01.000000 repro-apk-0.2.5/repro_apk/inplace_fix.py
+-rwx------   0 fay       (1000) fay       (1000)     3478 2024-03-09 23:18:00.000000 repro-apk-0.2.5/repro_apk/list_compresslevel.py
+-rw-------   0 fay       (1000) fay       (1000)        0 2022-11-22 16:14:18.000000 repro-apk-0.2.5/repro_apk/py.typed
+-rwx------   0 fay       (1000) fay       (1000)     5423 2023-02-19 23:18:39.000000 repro-apk-0.2.5/repro_apk/rm_files.py
+-rwx------   0 fay       (1000) fay       (1000)     5511 2023-01-15 20:09:06.000000 repro-apk-0.2.5/repro_apk/sort_apk.py
+-rwx------   0 fay       (1000) fay       (1000)     7107 2023-02-16 19:13:57.000000 repro-apk-0.2.5/repro_apk/sort_baseline.py
+-rwx------   0 fay       (1000) fay       (1000)     7276 2024-03-07 01:24:01.000000 repro-apk-0.2.5/repro_apk/zipalign.py
+-rwx------   0 fay       (1000) fay       (1000)    11965 2024-03-06 17:50:34.000000 repro-apk-0.2.5/repro_apk/zipinfo.py
+drwx------   0 fay       (1000) fay       (1000)        0 2024-03-21 15:40:08.611009 repro-apk-0.2.5/repro_apk.egg-info/
+-rw-------   0 fay       (1000) fay       (1000)    29830 2024-03-21 15:40:08.000000 repro-apk-0.2.5/repro_apk.egg-info/PKG-INFO
+-rw-------   0 fay       (1000) fay       (1000)      715 2024-03-21 15:40:08.000000 repro-apk-0.2.5/repro_apk.egg-info/SOURCES.txt
+-rw-------   0 fay       (1000) fay       (1000)        1 2024-03-21 15:40:08.000000 repro-apk-0.2.5/repro_apk.egg-info/dependency_links.txt
+-rw-------   0 fay       (1000) fay       (1000)       96 2024-03-21 15:40:08.000000 repro-apk-0.2.5/repro_apk.egg-info/entry_points.txt
+-rw-------   0 fay       (1000) fay       (1000)       11 2024-03-21 15:40:08.000000 repro-apk-0.2.5/repro_apk.egg-info/requires.txt
+-rw-------   0 fay       (1000) fay       (1000)       10 2024-03-21 15:40:08.000000 repro-apk-0.2.5/repro_apk.egg-info/top_level.txt
+-rw-------   0 fay       (1000) fay       (1000)       38 2024-03-21 15:40:08.611009 repro-apk-0.2.5/setup.cfg
+-rw-------   0 fay       (1000) fay       (1000)     1967 2024-03-21 15:34:02.000000 repro-apk-0.2.5/setup.py
```

### Comparing `repro-apk-0.2.4/LICENSE.GPLv3` & `repro-apk-0.2.5/LICENSE.GPLv3`

 * *Files identical despite different names*

### Comparing `repro-apk-0.2.4/Makefile` & `repro-apk-0.2.5/Makefile`

 * *Files identical despite different names*

### Comparing `repro-apk-0.2.4/PKG-INFO` & `repro-apk-0.2.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: repro-apk
-Version: 0.2.4
+Version: 0.2.5
 Summary: scripts to make android apks reproducible
 Home-page: https://github.com/obfusk/reproducible-apk-tools
 Author: FC Stegerman
 Author-email: flx@obfusk.net
 License: GPLv3+
 Keywords: android apk reproducible
 Classifier: Development Status :: 4 - Beta
@@ -54,14 +54,15 @@
 -->
 
 # reproducible-apk-tools
 
 [`fix-compresslevel.py`](#fix-compresslevelpy),
 [`fix-files.py`](#fix-filespy),
 [`fix-newlines.py`](#fix-newlinespy),
+[`fix-pg-map-id.py`](#fix-pg-map-idpy),
 [`rm-files.py`](#rm-filespy),
 [`sort-apk.py`](#sort-apkpy),
 [`sort-baseline.py`](#sort-baselinepy),
 [`zipalign.py`](#zipalignpy);
 
 [`diff-zip-meta.py`](#diff-zip-metapy),
 [`dump-arsc.py`](#dump-arscpy),
@@ -170,14 +171,65 @@
 ```
 
 NB: this builds a new ZIP file, preserving most ZIP metadata (and recompressing
 using the same compression level) but not everything: e.g. copying the existing
 local header extra fields which contain padding for alignment is not supported
 by Python's `ZipFile`, which is why `zipalign` is usually needed.
 
+### fix-pg-map-id.py
+
+Replace non-deterministic R8 `pg-map-id` in `classes.dex` (and `classes2.dex`
+etc. when present) and update checksums, also in `baseline.prof`.
+
+```bash
+$ fix-pg-map-id.py --help
+usage: fix-pg-map-id.py [-h] INPUT_DIR_OR_APK OUTPUT_DIR_OR_APK PG_MAP_ID
+[...]
+$ apksigcopier compare signed.apk --unsigned unsigned.apk
+DOES NOT VERIFY
+[...]
+$ diff -Naur <( unzip -p signed.apk classes.dex | xxd ) <( unzip -p unsigned.apk classes.dex | xxd )
+[...]
+-00000000: 6465 780a 3033 3500 829f 202e c800 6ecc  dex.035... ...n.
+-00000010: c15c 0a17 3737 73fc 982e 34db 6239 bc52  .\..77s...4.b9.R
++00000000: 6465 780a 3033 3500 d89f 1795 f719 4d94  dex.035.......M.
++00000010: 8358 2526 2850 f9e5 ad3d e772 c82e 4f02  .X%&(P...=.r..O.
+[...]
+ 005f1010: 2d61 7069 223a 3233 2c22 7067 2d6d 6170  -api":23,"pg-map
+-005f1020: 2d69 6422 3a22 3261 3939 3764 3322 2c22  -id":"2a997d3","
++005f1020: 2d69 6422 3a22 6565 3436 3531 3322 2c22  -id":"ee46513","
+[...]
+$ fix-pg-map-id.py unsigned.apk fixed.apk 2a997d3
+reading 'assets/dexopt/baseline.prof'...
+reading 'classes.dex'...
+reading 'classes2.dex'...
+fixing 'classes.dex'...
+dex version=035
+fixing pg-map-id: b'ee46513' -> b'2a997d3'
+fixing signature: f7194d94835825262850f9e5ad3de772c82e4f02 -> c8006eccc15c0a17373773fc982e34db6239bc52
+fixing checksum: 0x95179fd8 -> 0x2e209f82
+fixing 'classes2.dex'...
+dex version=035
+(not modified)
+fixing 'assets/dexopt/baseline.prof'...
+prof version=010 P
+fixing 'classes.dex' checksum: 0x95d40f72 -> 0x50191ba4
+writing 'assets/dexopt/baseline.prof'...
+writing 'classes.dex'...
+writing 'classes2.dex'...
+$ zipalign -f 4 fixed.apk fixed-aligned.apk
+$ apksigcopier compare signed.apk --unsigned fixed-aligned.apk && echo OK
+OK
+```
+
+NB: this builds a new ZIP file, preserving most ZIP metadata (and recompressing
+using the same compression level) but not everything: e.g. copying the existing
+local header extra fields which contain padding for alignment is not supported
+by Python's `ZipFile`, which is why `zipalign` is usually needed.
+
 ### rm-files.py
 
 Remove entries from ZIP file.
 
 Specify which files to remove by providing at least one fnmatch-style pattern,
 e.g. `'META-INF/MANIFEST.MF'`.
 
@@ -673,14 +725,16 @@
 $ repro-apk dump-axml --apk some.apk res/foo.xml
 $ repro-apk dump-baseline baseline.prof
 $ repro-apk dump-baseline baseline.profm
 $ repro-apk dump-baseline --apk some.apk
 $ repro-apk fix-compresslevel unsigned.apk fixed.apk 6 assets/foo/bar.js
 $ repro-apk fix-files unsigned.apk fixed.apk unix2dos 'META-INF/services/*'
 $ repro-apk fix-newlines unsigned.apk fixed.apk 'META-INF/services/*'
+$ repro-apk fix-pg-map-id unsigned.apk fixed.apk da39a3e
+$ repro-apk fix-pg-map-id input-dir output-dir da39a3e
 $ repro-apk list-compresslevel some.apk
 $ repro-apk rm-files some.apk fixed.apk META-INF/MANIFEST.IN
 $ repro-apk sort-apk unsigned.apk sorted.apk
 $ repro-apk sort-baseline baseline.profm baseline-sorted.profm
 $ repro-apk sort-baseline --apk unsigned.apk sorted-baseline.apk
 $ repro-apk zipalign fixed.apk fixed-aligned-py.apk
 $ repro-apk zipinfo -e some.apk
@@ -694,14 +748,15 @@
 $ repro-apk diff-zip-meta --help
 $ repro-apk dump-arsc --help
 $ repro-apk dump-axml --help
 $ repro-apk dump-baseline --help
 $ repro-apk fix-compresslevel --help
 $ repro-apk fix-files --help
 $ repro-apk fix-newlines --help
+$ repro-apk fix-pg-map-id --help
 $ repro-apk list-compresslevel --help
 $ repro-apk rm-files --help
 $ repro-apk sort-apk --help
 $ repro-apk sort-baseline --help
 $ repro-apk zipalign --help
 $ repro-apk zipinfo --help
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: repro-apk Version: 0.2.4 Summary: scripts to make
+Metadata-Version: 2.1 Name: repro-apk Version: 0.2.5 Summary: scripts to make
 android apks reproducible Home-page: https://github.com/obfusk/reproducible-
 apk-tools Author: FC Stegerman Author-email: flx@obfusk.net License: GPLv3+
 Keywords: android apk reproducible Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology Classifier: Intended
 Audience :: System Administrators Classifier: Intended Audience ::
 Telecommunications Industry Classifier: License :: OSI Approved :: GNU General
@@ -23,30 +23,31 @@
 //pypi.python.org/pypi/repro-apk) [![Python Versions](https://img.shields.io/
 pypi/pyversions/repro-apk.svg)](https://pypi.python.org/pypi/repro-apk) [![CI]
 (https://github.com/obfusk/reproducible-apk-tools/workflows/CI/badge.svg)]
 (https://github.com/obfusk/reproducible-apk-tools/actions?query=workflow%3ACI)
 [![GPLv3+](https://img.shields.io/badge/license-GPLv3+-blue.svg)](https://
 www.gnu.org/licenses/gpl-3.0.html) # reproducible-apk-tools [`fix-
 compresslevel.py`](#fix-compresslevelpy), [`fix-files.py`](#fix-filespy),
-[`fix-newlines.py`](#fix-newlinespy), [`rm-files.py`](#rm-filespy), [`sort-
-apk.py`](#sort-apkpy), [`sort-baseline.py`](#sort-baselinepy), [`zipalign.py`]
-(#zipalignpy); [`diff-zip-meta.py`](#diff-zip-metapy), [`dump-arsc.py`](#dump-
-arscpy), [`dump-axml.py`](#dump-axmlpy), [`dump-baseline.py`](#dump-
-baselinepy), [`list-compresslevel.py`](#list-compresslevelpy), [`zipinfo.py`]
-(#zipinfopy); [`inplace-fix.py`](#inplace-fixpy). ## scripts to make android
-apks reproducible `reproducible-apk-tools` is a collection of scripts
-(available as subcommands of the `repro-apk` command) to help make APKs
-reproducible (e.g. by changing line endings from LF to CRLF), or find out why
-they are not (e.g. by comparing ZIP file metadata, or dumping `baseline.prof`
-files). ### fix-compresslevel.py Recompress with different compression level.
-Specify which files to change by providing at least one fnmatch-style pattern,
-e.g. `'assets/foo/*.bar'`. If two APKs have identical contents but some ZIP
-entries are compressed with a different compression level, thus making the APKs
-not bit-by-bit identical, this script may help. ```bash $ fix-compresslevel.py
---help usage: fix-compresslevel.py [-h] [-v] INPUT_APK OUTPUT_APK COMPRESSLEVEL
+[`fix-newlines.py`](#fix-newlinespy), [`fix-pg-map-id.py`](#fix-pg-map-idpy),
+[`rm-files.py`](#rm-filespy), [`sort-apk.py`](#sort-apkpy), [`sort-
+baseline.py`](#sort-baselinepy), [`zipalign.py`](#zipalignpy); [`diff-zip-
+meta.py`](#diff-zip-metapy), [`dump-arsc.py`](#dump-arscpy), [`dump-axml.py`]
+(#dump-axmlpy), [`dump-baseline.py`](#dump-baselinepy), [`list-
+compresslevel.py`](#list-compresslevelpy), [`zipinfo.py`](#zipinfopy);
+[`inplace-fix.py`](#inplace-fixpy). ## scripts to make android apks
+reproducible `reproducible-apk-tools` is a collection of scripts (available as
+subcommands of the `repro-apk` command) to help make APKs reproducible (e.g. by
+changing line endings from LF to CRLF), or find out why they are not (e.g. by
+comparing ZIP file metadata, or dumping `baseline.prof` files). ### fix-
+compresslevel.py Recompress with different compression level. Specify which
+files to change by providing at least one fnmatch-style pattern, e.g. `'assets/
+foo/*.bar'`. If two APKs have identical contents but some ZIP entries are
+compressed with a different compression level, thus making the APKs not bit-by-
+bit identical, this script may help. ```bash $ fix-compresslevel.py --help
+usage: fix-compresslevel.py [-h] [-v] INPUT_APK OUTPUT_APK COMPRESSLEVEL
 PATTERN [PATTERN ...] [...] $ apksigcopier compare signed.apk --unsigned
 unsigned.apk DOES NOT VERIFY [...] $ fix-compresslevel.py unsigned.apk
 fixed.apk 6 assets/foo/bar.js fixing 'assets/foo/bar.js'... $ zipalign -f 4
 fixed.apk fixed-aligned.apk $ apksigcopier compare signed.apk --unsigned fixed-
 aligned.apk && echo OK OK ``` NB: this builds a new ZIP file, preserving most
 ZIP metadata (and recompressing entries not matching the pattern using the same
 compression level as in the original APK) but not everything: e.g. copying the
@@ -79,14 +80,41 @@
 fix-newlines.py unsigned.apk fixed.apk 'META-INF/services/*' fixing 'META-INF/
 services/foo'... fixing 'META-INF/services/bar'... $ zipalign -f 4 fixed.apk
 fixed-aligned.apk $ apksigcopier compare signed.apk --unsigned fixed-
 aligned.apk && echo OK OK ``` NB: this builds a new ZIP file, preserving most
 ZIP metadata (and recompressing using the same compression level) but not
 everything: e.g. copying the existing local header extra fields which contain
 padding for alignment is not supported by Python's `ZipFile`, which is why
+`zipalign` is usually needed. ### fix-pg-map-id.py Replace non-deterministic R8
+`pg-map-id` in `classes.dex` (and `classes2.dex` etc. when present) and update
+checksums, also in `baseline.prof`. ```bash $ fix-pg-map-id.py --help usage:
+fix-pg-map-id.py [-h] INPUT_DIR_OR_APK OUTPUT_DIR_OR_APK PG_MAP_ID [...] $
+apksigcopier compare signed.apk --unsigned unsigned.apk DOES NOT VERIFY [...] $
+diff -Naur <( unzip -p signed.apk classes.dex | xxd ) <( unzip -p unsigned.apk
+classes.dex | xxd ) [...] -00000000: 6465 780a 3033 3500 829f 202e c800 6ecc
+dex.035... ...n. -00000010: c15c 0a17 3737 73fc 982e 34db 6239 bc52
+.\..77s...4.b9.R +00000000: 6465 780a 3033 3500 d89f 1795 f719 4d94
+dex.035.......M. +00000010: 8358 2526 2850 f9e5 ad3d e772 c82e 4f02 .X%&
+(P...=.r..O. [...] 005f1010: 2d61 7069 223a 3233 2c22 7067 2d6d 6170 -api":
+23,"pg-map -005f1020: 2d69 6422 3a22 3261 3939 3764 3322 2c22 -id":"2a997d3","
++005f1020: 2d69 6422 3a22 6565 3436 3531 3322 2c22 -id":"ee46513"," [...] $
+fix-pg-map-id.py unsigned.apk fixed.apk 2a997d3 reading 'assets/dexopt/
+baseline.prof'... reading 'classes.dex'... reading 'classes2.dex'... fixing
+'classes.dex'... dex version=035 fixing pg-map-id: b'ee46513' -> b'2a997d3'
+fixing signature: f7194d94835825262850f9e5ad3de772c82e4f02 -
+> c8006eccc15c0a17373773fc982e34db6239bc52 fixing checksum: 0x95179fd8 -
+> 0x2e209f82 fixing 'classes2.dex'... dex version=035 (not modified) fixing
+'assets/dexopt/baseline.prof'... prof version=010 P fixing 'classes.dex'
+checksum: 0x95d40f72 -> 0x50191ba4 writing 'assets/dexopt/baseline.prof'...
+writing 'classes.dex'... writing 'classes2.dex'... $ zipalign -f 4 fixed.apk
+fixed-aligned.apk $ apksigcopier compare signed.apk --unsigned fixed-
+aligned.apk && echo OK OK ``` NB: this builds a new ZIP file, preserving most
+ZIP metadata (and recompressing using the same compression level) but not
+everything: e.g. copying the existing local header extra fields which contain
+padding for alignment is not supported by Python's `ZipFile`, which is why
 `zipalign` is usually needed. ### rm-files.py Remove entries from ZIP file.
 Specify which files to remove by providing at least one fnmatch-style pattern,
 e.g. `'META-INF/MANIFEST.MF'`. ```bash $ rm-files.py --help usage: rm-files.py
 [-h] [-v] INPUT_APK OUTPUT_APK PATTERN [PATTERN ...] [...] $ rm-files.py
 some.apk fixed.apk META-INF/MANIFEST.IN skipping 'META-INF/MANIFEST.IN'... $
 zipalign -f 4 fixed.apk fixed-aligned.apk ``` NB: this builds a new ZIP file,
 preserving most ZIP metadata (and recompressing using the same compression
@@ -305,23 +333,25 @@
 repro-apk diff-zip-meta a.apk c.apk --no-offsets --no-ordering $ repro-apk
 dump-arsc resources.arsc $ repro-apk dump-arsc --apk some.apk $ repro-apk dump-
 axml foo.xml $ repro-apk dump-axml --apk some.apk res/foo.xml $ repro-apk dump-
 baseline baseline.prof $ repro-apk dump-baseline baseline.profm $ repro-apk
 dump-baseline --apk some.apk $ repro-apk fix-compresslevel unsigned.apk
 fixed.apk 6 assets/foo/bar.js $ repro-apk fix-files unsigned.apk fixed.apk
 unix2dos 'META-INF/services/*' $ repro-apk fix-newlines unsigned.apk fixed.apk
-'META-INF/services/*' $ repro-apk list-compresslevel some.apk $ repro-apk rm-
-files some.apk fixed.apk META-INF/MANIFEST.IN $ repro-apk sort-apk unsigned.apk
-sorted.apk $ repro-apk sort-baseline baseline.profm baseline-sorted.profm $
-repro-apk sort-baseline --apk unsigned.apk sorted-baseline.apk $ repro-apk
-zipalign fixed.apk fixed-aligned-py.apk $ repro-apk zipinfo -e some.apk $
-repro-apk zipinfo -l some.apk ``` ### Help ```bash $ repro-apk --help $ repro-
-apk diff-zip-meta --help $ repro-apk dump-arsc --help $ repro-apk dump-axml --
-help $ repro-apk dump-baseline --help $ repro-apk fix-compresslevel --help $
-repro-apk fix-files --help $ repro-apk fix-newlines --help $ repro-apk list-
+'META-INF/services/*' $ repro-apk fix-pg-map-id unsigned.apk fixed.apk da39a3e
+$ repro-apk fix-pg-map-id input-dir output-dir da39a3e $ repro-apk list-
+compresslevel some.apk $ repro-apk rm-files some.apk fixed.apk META-INF/
+MANIFEST.IN $ repro-apk sort-apk unsigned.apk sorted.apk $ repro-apk sort-
+baseline baseline.profm baseline-sorted.profm $ repro-apk sort-baseline --apk
+unsigned.apk sorted-baseline.apk $ repro-apk zipalign fixed.apk fixed-aligned-
+py.apk $ repro-apk zipinfo -e some.apk $ repro-apk zipinfo -l some.apk ``` ###
+Help ```bash $ repro-apk --help $ repro-apk diff-zip-meta --help $ repro-apk
+dump-arsc --help $ repro-apk dump-axml --help $ repro-apk dump-baseline --help
+$ repro-apk fix-compresslevel --help $ repro-apk fix-files --help $ repro-apk
+fix-newlines --help $ repro-apk fix-pg-map-id --help $ repro-apk list-
 compresslevel --help $ repro-apk rm-files --help $ repro-apk sort-apk --help $
 repro-apk sort-baseline --help $ repro-apk zipalign --help $ repro-apk zipinfo
 --help ``` ## Installing ### Using pip ```bash $ pip install repro-apk ``` NB:
 depending on your system you may need to use e.g. `pip3 --user` instead of just
 `pip`. ### From git NB: this installs the latest development version, not the
 latest release. ```bash $ git clone https://github.com/obfusk/reproducible-apk-
 tools.git $ cd reproducible-apk-tools $ pip install -e . ``` NB: you may need
```

### Comparing `repro-apk-0.2.4/README.md` & `repro-apk-0.2.5/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 -->
 
 # reproducible-apk-tools
 
 [`fix-compresslevel.py`](#fix-compresslevelpy),
 [`fix-files.py`](#fix-filespy),
 [`fix-newlines.py`](#fix-newlinespy),
+[`fix-pg-map-id.py`](#fix-pg-map-idpy),
 [`rm-files.py`](#rm-filespy),
 [`sort-apk.py`](#sort-apkpy),
 [`sort-baseline.py`](#sort-baselinepy),
 [`zipalign.py`](#zipalignpy);
 
 [`diff-zip-meta.py`](#diff-zip-metapy),
 [`dump-arsc.py`](#dump-arscpy),
@@ -136,14 +137,65 @@
 ```
 
 NB: this builds a new ZIP file, preserving most ZIP metadata (and recompressing
 using the same compression level) but not everything: e.g. copying the existing
 local header extra fields which contain padding for alignment is not supported
 by Python's `ZipFile`, which is why `zipalign` is usually needed.
 
+### fix-pg-map-id.py
+
+Replace non-deterministic R8 `pg-map-id` in `classes.dex` (and `classes2.dex`
+etc. when present) and update checksums, also in `baseline.prof`.
+
+```bash
+$ fix-pg-map-id.py --help
+usage: fix-pg-map-id.py [-h] INPUT_DIR_OR_APK OUTPUT_DIR_OR_APK PG_MAP_ID
+[...]
+$ apksigcopier compare signed.apk --unsigned unsigned.apk
+DOES NOT VERIFY
+[...]
+$ diff -Naur <( unzip -p signed.apk classes.dex | xxd ) <( unzip -p unsigned.apk classes.dex | xxd )
+[...]
+-00000000: 6465 780a 3033 3500 829f 202e c800 6ecc  dex.035... ...n.
+-00000010: c15c 0a17 3737 73fc 982e 34db 6239 bc52  .\..77s...4.b9.R
++00000000: 6465 780a 3033 3500 d89f 1795 f719 4d94  dex.035.......M.
++00000010: 8358 2526 2850 f9e5 ad3d e772 c82e 4f02  .X%&(P...=.r..O.
+[...]
+ 005f1010: 2d61 7069 223a 3233 2c22 7067 2d6d 6170  -api":23,"pg-map
+-005f1020: 2d69 6422 3a22 3261 3939 3764 3322 2c22  -id":"2a997d3","
++005f1020: 2d69 6422 3a22 6565 3436 3531 3322 2c22  -id":"ee46513","
+[...]
+$ fix-pg-map-id.py unsigned.apk fixed.apk 2a997d3
+reading 'assets/dexopt/baseline.prof'...
+reading 'classes.dex'...
+reading 'classes2.dex'...
+fixing 'classes.dex'...
+dex version=035
+fixing pg-map-id: b'ee46513' -> b'2a997d3'
+fixing signature: f7194d94835825262850f9e5ad3de772c82e4f02 -> c8006eccc15c0a17373773fc982e34db6239bc52
+fixing checksum: 0x95179fd8 -> 0x2e209f82
+fixing 'classes2.dex'...
+dex version=035
+(not modified)
+fixing 'assets/dexopt/baseline.prof'...
+prof version=010 P
+fixing 'classes.dex' checksum: 0x95d40f72 -> 0x50191ba4
+writing 'assets/dexopt/baseline.prof'...
+writing 'classes.dex'...
+writing 'classes2.dex'...
+$ zipalign -f 4 fixed.apk fixed-aligned.apk
+$ apksigcopier compare signed.apk --unsigned fixed-aligned.apk && echo OK
+OK
+```
+
+NB: this builds a new ZIP file, preserving most ZIP metadata (and recompressing
+using the same compression level) but not everything: e.g. copying the existing
+local header extra fields which contain padding for alignment is not supported
+by Python's `ZipFile`, which is why `zipalign` is usually needed.
+
 ### rm-files.py
 
 Remove entries from ZIP file.
 
 Specify which files to remove by providing at least one fnmatch-style pattern,
 e.g. `'META-INF/MANIFEST.MF'`.
 
@@ -639,14 +691,16 @@
 $ repro-apk dump-axml --apk some.apk res/foo.xml
 $ repro-apk dump-baseline baseline.prof
 $ repro-apk dump-baseline baseline.profm
 $ repro-apk dump-baseline --apk some.apk
 $ repro-apk fix-compresslevel unsigned.apk fixed.apk 6 assets/foo/bar.js
 $ repro-apk fix-files unsigned.apk fixed.apk unix2dos 'META-INF/services/*'
 $ repro-apk fix-newlines unsigned.apk fixed.apk 'META-INF/services/*'
+$ repro-apk fix-pg-map-id unsigned.apk fixed.apk da39a3e
+$ repro-apk fix-pg-map-id input-dir output-dir da39a3e
 $ repro-apk list-compresslevel some.apk
 $ repro-apk rm-files some.apk fixed.apk META-INF/MANIFEST.IN
 $ repro-apk sort-apk unsigned.apk sorted.apk
 $ repro-apk sort-baseline baseline.profm baseline-sorted.profm
 $ repro-apk sort-baseline --apk unsigned.apk sorted-baseline.apk
 $ repro-apk zipalign fixed.apk fixed-aligned-py.apk
 $ repro-apk zipinfo -e some.apk
@@ -660,14 +714,15 @@
 $ repro-apk diff-zip-meta --help
 $ repro-apk dump-arsc --help
 $ repro-apk dump-axml --help
 $ repro-apk dump-baseline --help
 $ repro-apk fix-compresslevel --help
 $ repro-apk fix-files --help
 $ repro-apk fix-newlines --help
+$ repro-apk fix-pg-map-id --help
 $ repro-apk list-compresslevel --help
 $ repro-apk rm-files --help
 $ repro-apk sort-apk --help
 $ repro-apk sort-baseline --help
 $ repro-apk zipalign --help
 $ repro-apk zipinfo --help
 ```
```

#### html2text {}

```diff
@@ -4,30 +4,31 @@
 //pypi.python.org/pypi/repro-apk) [![Python Versions](https://img.shields.io/
 pypi/pyversions/repro-apk.svg)](https://pypi.python.org/pypi/repro-apk) [![CI]
 (https://github.com/obfusk/reproducible-apk-tools/workflows/CI/badge.svg)]
 (https://github.com/obfusk/reproducible-apk-tools/actions?query=workflow%3ACI)
 [![GPLv3+](https://img.shields.io/badge/license-GPLv3+-blue.svg)](https://
 www.gnu.org/licenses/gpl-3.0.html) # reproducible-apk-tools [`fix-
 compresslevel.py`](#fix-compresslevelpy), [`fix-files.py`](#fix-filespy),
-[`fix-newlines.py`](#fix-newlinespy), [`rm-files.py`](#rm-filespy), [`sort-
-apk.py`](#sort-apkpy), [`sort-baseline.py`](#sort-baselinepy), [`zipalign.py`]
-(#zipalignpy); [`diff-zip-meta.py`](#diff-zip-metapy), [`dump-arsc.py`](#dump-
-arscpy), [`dump-axml.py`](#dump-axmlpy), [`dump-baseline.py`](#dump-
-baselinepy), [`list-compresslevel.py`](#list-compresslevelpy), [`zipinfo.py`]
-(#zipinfopy); [`inplace-fix.py`](#inplace-fixpy). ## scripts to make android
-apks reproducible `reproducible-apk-tools` is a collection of scripts
-(available as subcommands of the `repro-apk` command) to help make APKs
-reproducible (e.g. by changing line endings from LF to CRLF), or find out why
-they are not (e.g. by comparing ZIP file metadata, or dumping `baseline.prof`
-files). ### fix-compresslevel.py Recompress with different compression level.
-Specify which files to change by providing at least one fnmatch-style pattern,
-e.g. `'assets/foo/*.bar'`. If two APKs have identical contents but some ZIP
-entries are compressed with a different compression level, thus making the APKs
-not bit-by-bit identical, this script may help. ```bash $ fix-compresslevel.py
---help usage: fix-compresslevel.py [-h] [-v] INPUT_APK OUTPUT_APK COMPRESSLEVEL
+[`fix-newlines.py`](#fix-newlinespy), [`fix-pg-map-id.py`](#fix-pg-map-idpy),
+[`rm-files.py`](#rm-filespy), [`sort-apk.py`](#sort-apkpy), [`sort-
+baseline.py`](#sort-baselinepy), [`zipalign.py`](#zipalignpy); [`diff-zip-
+meta.py`](#diff-zip-metapy), [`dump-arsc.py`](#dump-arscpy), [`dump-axml.py`]
+(#dump-axmlpy), [`dump-baseline.py`](#dump-baselinepy), [`list-
+compresslevel.py`](#list-compresslevelpy), [`zipinfo.py`](#zipinfopy);
+[`inplace-fix.py`](#inplace-fixpy). ## scripts to make android apks
+reproducible `reproducible-apk-tools` is a collection of scripts (available as
+subcommands of the `repro-apk` command) to help make APKs reproducible (e.g. by
+changing line endings from LF to CRLF), or find out why they are not (e.g. by
+comparing ZIP file metadata, or dumping `baseline.prof` files). ### fix-
+compresslevel.py Recompress with different compression level. Specify which
+files to change by providing at least one fnmatch-style pattern, e.g. `'assets/
+foo/*.bar'`. If two APKs have identical contents but some ZIP entries are
+compressed with a different compression level, thus making the APKs not bit-by-
+bit identical, this script may help. ```bash $ fix-compresslevel.py --help
+usage: fix-compresslevel.py [-h] [-v] INPUT_APK OUTPUT_APK COMPRESSLEVEL
 PATTERN [PATTERN ...] [...] $ apksigcopier compare signed.apk --unsigned
 unsigned.apk DOES NOT VERIFY [...] $ fix-compresslevel.py unsigned.apk
 fixed.apk 6 assets/foo/bar.js fixing 'assets/foo/bar.js'... $ zipalign -f 4
 fixed.apk fixed-aligned.apk $ apksigcopier compare signed.apk --unsigned fixed-
 aligned.apk && echo OK OK ``` NB: this builds a new ZIP file, preserving most
 ZIP metadata (and recompressing entries not matching the pattern using the same
 compression level as in the original APK) but not everything: e.g. copying the
@@ -60,14 +61,41 @@
 fix-newlines.py unsigned.apk fixed.apk 'META-INF/services/*' fixing 'META-INF/
 services/foo'... fixing 'META-INF/services/bar'... $ zipalign -f 4 fixed.apk
 fixed-aligned.apk $ apksigcopier compare signed.apk --unsigned fixed-
 aligned.apk && echo OK OK ``` NB: this builds a new ZIP file, preserving most
 ZIP metadata (and recompressing using the same compression level) but not
 everything: e.g. copying the existing local header extra fields which contain
 padding for alignment is not supported by Python's `ZipFile`, which is why
+`zipalign` is usually needed. ### fix-pg-map-id.py Replace non-deterministic R8
+`pg-map-id` in `classes.dex` (and `classes2.dex` etc. when present) and update
+checksums, also in `baseline.prof`. ```bash $ fix-pg-map-id.py --help usage:
+fix-pg-map-id.py [-h] INPUT_DIR_OR_APK OUTPUT_DIR_OR_APK PG_MAP_ID [...] $
+apksigcopier compare signed.apk --unsigned unsigned.apk DOES NOT VERIFY [...] $
+diff -Naur <( unzip -p signed.apk classes.dex | xxd ) <( unzip -p unsigned.apk
+classes.dex | xxd ) [...] -00000000: 6465 780a 3033 3500 829f 202e c800 6ecc
+dex.035... ...n. -00000010: c15c 0a17 3737 73fc 982e 34db 6239 bc52
+.\..77s...4.b9.R +00000000: 6465 780a 3033 3500 d89f 1795 f719 4d94
+dex.035.......M. +00000010: 8358 2526 2850 f9e5 ad3d e772 c82e 4f02 .X%&
+(P...=.r..O. [...] 005f1010: 2d61 7069 223a 3233 2c22 7067 2d6d 6170 -api":
+23,"pg-map -005f1020: 2d69 6422 3a22 3261 3939 3764 3322 2c22 -id":"2a997d3","
++005f1020: 2d69 6422 3a22 6565 3436 3531 3322 2c22 -id":"ee46513"," [...] $
+fix-pg-map-id.py unsigned.apk fixed.apk 2a997d3 reading 'assets/dexopt/
+baseline.prof'... reading 'classes.dex'... reading 'classes2.dex'... fixing
+'classes.dex'... dex version=035 fixing pg-map-id: b'ee46513' -> b'2a997d3'
+fixing signature: f7194d94835825262850f9e5ad3de772c82e4f02 -
+> c8006eccc15c0a17373773fc982e34db6239bc52 fixing checksum: 0x95179fd8 -
+> 0x2e209f82 fixing 'classes2.dex'... dex version=035 (not modified) fixing
+'assets/dexopt/baseline.prof'... prof version=010 P fixing 'classes.dex'
+checksum: 0x95d40f72 -> 0x50191ba4 writing 'assets/dexopt/baseline.prof'...
+writing 'classes.dex'... writing 'classes2.dex'... $ zipalign -f 4 fixed.apk
+fixed-aligned.apk $ apksigcopier compare signed.apk --unsigned fixed-
+aligned.apk && echo OK OK ``` NB: this builds a new ZIP file, preserving most
+ZIP metadata (and recompressing using the same compression level) but not
+everything: e.g. copying the existing local header extra fields which contain
+padding for alignment is not supported by Python's `ZipFile`, which is why
 `zipalign` is usually needed. ### rm-files.py Remove entries from ZIP file.
 Specify which files to remove by providing at least one fnmatch-style pattern,
 e.g. `'META-INF/MANIFEST.MF'`. ```bash $ rm-files.py --help usage: rm-files.py
 [-h] [-v] INPUT_APK OUTPUT_APK PATTERN [PATTERN ...] [...] $ rm-files.py
 some.apk fixed.apk META-INF/MANIFEST.IN skipping 'META-INF/MANIFEST.IN'... $
 zipalign -f 4 fixed.apk fixed-aligned.apk ``` NB: this builds a new ZIP file,
 preserving most ZIP metadata (and recompressing using the same compression
@@ -286,23 +314,25 @@
 repro-apk diff-zip-meta a.apk c.apk --no-offsets --no-ordering $ repro-apk
 dump-arsc resources.arsc $ repro-apk dump-arsc --apk some.apk $ repro-apk dump-
 axml foo.xml $ repro-apk dump-axml --apk some.apk res/foo.xml $ repro-apk dump-
 baseline baseline.prof $ repro-apk dump-baseline baseline.profm $ repro-apk
 dump-baseline --apk some.apk $ repro-apk fix-compresslevel unsigned.apk
 fixed.apk 6 assets/foo/bar.js $ repro-apk fix-files unsigned.apk fixed.apk
 unix2dos 'META-INF/services/*' $ repro-apk fix-newlines unsigned.apk fixed.apk
-'META-INF/services/*' $ repro-apk list-compresslevel some.apk $ repro-apk rm-
-files some.apk fixed.apk META-INF/MANIFEST.IN $ repro-apk sort-apk unsigned.apk
-sorted.apk $ repro-apk sort-baseline baseline.profm baseline-sorted.profm $
-repro-apk sort-baseline --apk unsigned.apk sorted-baseline.apk $ repro-apk
-zipalign fixed.apk fixed-aligned-py.apk $ repro-apk zipinfo -e some.apk $
-repro-apk zipinfo -l some.apk ``` ### Help ```bash $ repro-apk --help $ repro-
-apk diff-zip-meta --help $ repro-apk dump-arsc --help $ repro-apk dump-axml --
-help $ repro-apk dump-baseline --help $ repro-apk fix-compresslevel --help $
-repro-apk fix-files --help $ repro-apk fix-newlines --help $ repro-apk list-
+'META-INF/services/*' $ repro-apk fix-pg-map-id unsigned.apk fixed.apk da39a3e
+$ repro-apk fix-pg-map-id input-dir output-dir da39a3e $ repro-apk list-
+compresslevel some.apk $ repro-apk rm-files some.apk fixed.apk META-INF/
+MANIFEST.IN $ repro-apk sort-apk unsigned.apk sorted.apk $ repro-apk sort-
+baseline baseline.profm baseline-sorted.profm $ repro-apk sort-baseline --apk
+unsigned.apk sorted-baseline.apk $ repro-apk zipalign fixed.apk fixed-aligned-
+py.apk $ repro-apk zipinfo -e some.apk $ repro-apk zipinfo -l some.apk ``` ###
+Help ```bash $ repro-apk --help $ repro-apk diff-zip-meta --help $ repro-apk
+dump-arsc --help $ repro-apk dump-axml --help $ repro-apk dump-baseline --help
+$ repro-apk fix-compresslevel --help $ repro-apk fix-files --help $ repro-apk
+fix-newlines --help $ repro-apk fix-pg-map-id --help $ repro-apk list-
 compresslevel --help $ repro-apk rm-files --help $ repro-apk sort-apk --help $
 repro-apk sort-baseline --help $ repro-apk zipalign --help $ repro-apk zipinfo
 --help ``` ## Installing ### Using pip ```bash $ pip install repro-apk ``` NB:
 depending on your system you may need to use e.g. `pip3 --user` instead of just
 `pip`. ### From git NB: this installs the latest development version, not the
 latest release. ```bash $ git clone https://github.com/obfusk/reproducible-apk-
 tools.git $ cd reproducible-apk-tools $ pip install -e . ``` NB: you may need
```

### Comparing `repro-apk-0.2.4/changelog.txt` & `repro-apk-0.2.5/changelog.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+v0.2.5
+
+• add fix-pg-map-id.py.
+
 v0.2.4
 
 • add rm-files.py & fix-files.py.
 • add zipalign.py (w/ -P/--page-size support).
 • inplace-fix.py: --page-align, --page-size; use zipalign.py (fallback & --internal).
 • diff-zip-meta.py: diff extra time [#17], show CRC etc. as hex, show byte diff sizes.
 • zipinfo.py: add --sort-by-offset.
```

### Comparing `repro-apk-0.2.4/repro_apk/__init__.py` & `repro-apk-0.2.5/repro_apk/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,44 +1,47 @@
 #!/usr/bin/python3
 # encoding: utf-8
 # SPDX-FileCopyrightText: 2024 FC (Fay) Stegerman <flx@obfusk.net>
 # SPDX-License-Identifier: GPL-3.0-or-later
 
+import os
 import sys
 import zipfile
 
 from typing import Optional, Tuple
 
 from . import diff_zip_meta as _diff_zip_meta
 from . import dump_arsc as _dump_arsc
 from . import dump_axml as _dump_axml
 from . import dump_baseline as _dump_baseline
 from . import fix_compresslevel as _fix_compresslevel
 from . import fix_files as _fix_files
 from . import fix_newlines as _fix_newlines
+from . import fix_pg_map_id as _fix_pg_map_id
 from . import list_compresslevel as _list_compresslevel
 from . import rm_files as _rm_files
 from . import sort_apk as _sort_apk
 from . import sort_baseline as _sort_baseline
 from . import zipalign as _zipalign
 from . import zipinfo as _zipinfo
 
 import click
 
-__version__ = "0.2.4"
+__version__ = "0.2.5"
 NAME = "repro-apk"
 
 ERRORS = (
     _diff_zip_meta.Error,
     _dump_arsc.Error,
     _dump_axml.Error,
     _dump_baseline.Error,
     _fix_compresslevel.Error,
     _fix_files.Error,
     _fix_newlines.Error,
+    _fix_pg_map_id.Error,
     _list_compresslevel.Error,
     _rm_files.Error,
     _sort_apk.Error,
     _sort_baseline.Error,
     _zipalign.Error,
     _zipinfo.Error,
     zipfile.BadZipFile,
@@ -163,14 +166,27 @@
     def fix_newlines(input_apk: str, output_apk: str, patterns: Tuple[str, ...],
                      from_crlf: bool, verbose: bool) -> None:
         replace = ("\r\n", "\n") if from_crlf else ("\n", "\r\n")
         _fix_newlines.fix_newlines(input_apk, output_apk, *patterns,
                                    replace=replace, verbose=verbose)
 
     @cli.command(help="""
+        Replace non-deterministic R8 pg-map-id in classes{,N}.dex and update
+        checksums, also in baseline.prof.
+    """)
+    @click.argument("input_dir_or_apk", type=click.Path(exists=True, dir_okay=True))
+    @click.argument("output_dir_or_apk", type=click.Path(dir_okay=True))
+    @click.argument("pg_map_id")
+    def fix_pg_map_id(input_dir_or_apk: str, output_dir_or_apk: str, pg_map_id: str) -> None:
+        if os.path.isdir(input_dir_or_apk):
+            _fix_pg_map_id.fix_pg_map_id(input_dir_or_apk, output_dir_or_apk, pg_map_id)
+        else:
+            _fix_pg_map_id.fix_pg_map_id_apk(input_dir_or_apk, output_dir_or_apk, pg_map_id)
+
+    @cli.command(help="""
         List ZIP entries with compression level.
 
         You can optionally specify which files to list by providing one or more
         fnmatch-style patterns, e.g. 'assets/foo/*.bar'.
     """)
     @click.argument("apk", type=click.Path(exists=True, dir_okay=False))
     @click.argument("patterns", metavar="[PATTERN...]", nargs=-1)
```

### Comparing `repro-apk-0.2.4/repro_apk/diff_zip_meta.py` & `repro-apk-0.2.5/repro_apk/diff_zip_meta.py`

 * *Files identical despite different names*

### Comparing `repro-apk-0.2.4/repro_apk/dump_arsc.py` & `repro-apk-0.2.5/repro_apk/dump_arsc.py`

 * *Files identical despite different names*

### Comparing `repro-apk-0.2.4/repro_apk/dump_axml.py` & `repro-apk-0.2.5/repro_apk/dump_axml.py`

 * *Files identical despite different names*

### Comparing `repro-apk-0.2.4/repro_apk/dump_baseline.py` & `repro-apk-0.2.5/repro_apk/dump_baseline.py`

 * *Files identical despite different names*

### Comparing `repro-apk-0.2.4/repro_apk/fix_compresslevel.py` & `repro-apk-0.2.5/repro_apk/fix_compresslevel.py`

 * *Files identical despite different names*

### Comparing `repro-apk-0.2.4/repro_apk/fix_files.py` & `repro-apk-0.2.5/repro_apk/fix_files.py`

 * *Files identical despite different names*

### Comparing `repro-apk-0.2.4/repro_apk/fix_newlines.py` & `repro-apk-0.2.5/repro_apk/fix_newlines.py`

 * *Files identical despite different names*

### Comparing `repro-apk-0.2.4/repro_apk/inplace_fix.py` & `repro-apk-0.2.5/repro_apk/inplace_fix.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 
 from typing import Optional, Tuple
 
 COMMANDS = (
     "fix-compresslevel",
     "fix-files",
     "fix-newlines",
+    "fix-pg-map-id",
     "rm-files",
     "sort-apk",
     "sort-baseline",
 )
 
 BUILD_TOOLS_WITH_BROKEN_ZIPALIGN = ("31.0.0", "32.0.0")
 BUILD_TOOLS_WITH_PAGE_SIZE_FROM = "35.0.0-rc1"
```

### Comparing `repro-apk-0.2.4/repro_apk/list_compresslevel.py` & `repro-apk-0.2.5/repro_apk/list_compresslevel.py`

 * *Files identical despite different names*

### Comparing `repro-apk-0.2.4/repro_apk/rm_files.py` & `repro-apk-0.2.5/repro_apk/rm_files.py`

 * *Files identical despite different names*

### Comparing `repro-apk-0.2.4/repro_apk/sort_apk.py` & `repro-apk-0.2.5/repro_apk/sort_apk.py`

 * *Files identical despite different names*

### Comparing `repro-apk-0.2.4/repro_apk/sort_baseline.py` & `repro-apk-0.2.5/repro_apk/sort_baseline.py`

 * *Files identical despite different names*

### Comparing `repro-apk-0.2.4/repro_apk/zipalign.py` & `repro-apk-0.2.5/repro_apk/zipalign.py`

 * *Files identical despite different names*

### Comparing `repro-apk-0.2.4/repro_apk/zipinfo.py` & `repro-apk-0.2.5/repro_apk/zipinfo.py`

 * *Files identical despite different names*

### Comparing `repro-apk-0.2.4/repro_apk.egg-info/PKG-INFO` & `repro-apk-0.2.5/repro_apk.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: repro-apk
-Version: 0.2.4
+Version: 0.2.5
 Summary: scripts to make android apks reproducible
 Home-page: https://github.com/obfusk/reproducible-apk-tools
 Author: FC Stegerman
 Author-email: flx@obfusk.net
 License: GPLv3+
 Keywords: android apk reproducible
 Classifier: Development Status :: 4 - Beta
@@ -54,14 +54,15 @@
 -->
 
 # reproducible-apk-tools
 
 [`fix-compresslevel.py`](#fix-compresslevelpy),
 [`fix-files.py`](#fix-filespy),
 [`fix-newlines.py`](#fix-newlinespy),
+[`fix-pg-map-id.py`](#fix-pg-map-idpy),
 [`rm-files.py`](#rm-filespy),
 [`sort-apk.py`](#sort-apkpy),
 [`sort-baseline.py`](#sort-baselinepy),
 [`zipalign.py`](#zipalignpy);
 
 [`diff-zip-meta.py`](#diff-zip-metapy),
 [`dump-arsc.py`](#dump-arscpy),
@@ -170,14 +171,65 @@
 ```
 
 NB: this builds a new ZIP file, preserving most ZIP metadata (and recompressing
 using the same compression level) but not everything: e.g. copying the existing
 local header extra fields which contain padding for alignment is not supported
 by Python's `ZipFile`, which is why `zipalign` is usually needed.
 
+### fix-pg-map-id.py
+
+Replace non-deterministic R8 `pg-map-id` in `classes.dex` (and `classes2.dex`
+etc. when present) and update checksums, also in `baseline.prof`.
+
+```bash
+$ fix-pg-map-id.py --help
+usage: fix-pg-map-id.py [-h] INPUT_DIR_OR_APK OUTPUT_DIR_OR_APK PG_MAP_ID
+[...]
+$ apksigcopier compare signed.apk --unsigned unsigned.apk
+DOES NOT VERIFY
+[...]
+$ diff -Naur <( unzip -p signed.apk classes.dex | xxd ) <( unzip -p unsigned.apk classes.dex | xxd )
+[...]
+-00000000: 6465 780a 3033 3500 829f 202e c800 6ecc  dex.035... ...n.
+-00000010: c15c 0a17 3737 73fc 982e 34db 6239 bc52  .\..77s...4.b9.R
++00000000: 6465 780a 3033 3500 d89f 1795 f719 4d94  dex.035.......M.
++00000010: 8358 2526 2850 f9e5 ad3d e772 c82e 4f02  .X%&(P...=.r..O.
+[...]
+ 005f1010: 2d61 7069 223a 3233 2c22 7067 2d6d 6170  -api":23,"pg-map
+-005f1020: 2d69 6422 3a22 3261 3939 3764 3322 2c22  -id":"2a997d3","
++005f1020: 2d69 6422 3a22 6565 3436 3531 3322 2c22  -id":"ee46513","
+[...]
+$ fix-pg-map-id.py unsigned.apk fixed.apk 2a997d3
+reading 'assets/dexopt/baseline.prof'...
+reading 'classes.dex'...
+reading 'classes2.dex'...
+fixing 'classes.dex'...
+dex version=035
+fixing pg-map-id: b'ee46513' -> b'2a997d3'
+fixing signature: f7194d94835825262850f9e5ad3de772c82e4f02 -> c8006eccc15c0a17373773fc982e34db6239bc52
+fixing checksum: 0x95179fd8 -> 0x2e209f82
+fixing 'classes2.dex'...
+dex version=035
+(not modified)
+fixing 'assets/dexopt/baseline.prof'...
+prof version=010 P
+fixing 'classes.dex' checksum: 0x95d40f72 -> 0x50191ba4
+writing 'assets/dexopt/baseline.prof'...
+writing 'classes.dex'...
+writing 'classes2.dex'...
+$ zipalign -f 4 fixed.apk fixed-aligned.apk
+$ apksigcopier compare signed.apk --unsigned fixed-aligned.apk && echo OK
+OK
+```
+
+NB: this builds a new ZIP file, preserving most ZIP metadata (and recompressing
+using the same compression level) but not everything: e.g. copying the existing
+local header extra fields which contain padding for alignment is not supported
+by Python's `ZipFile`, which is why `zipalign` is usually needed.
+
 ### rm-files.py
 
 Remove entries from ZIP file.
 
 Specify which files to remove by providing at least one fnmatch-style pattern,
 e.g. `'META-INF/MANIFEST.MF'`.
 
@@ -673,14 +725,16 @@
 $ repro-apk dump-axml --apk some.apk res/foo.xml
 $ repro-apk dump-baseline baseline.prof
 $ repro-apk dump-baseline baseline.profm
 $ repro-apk dump-baseline --apk some.apk
 $ repro-apk fix-compresslevel unsigned.apk fixed.apk 6 assets/foo/bar.js
 $ repro-apk fix-files unsigned.apk fixed.apk unix2dos 'META-INF/services/*'
 $ repro-apk fix-newlines unsigned.apk fixed.apk 'META-INF/services/*'
+$ repro-apk fix-pg-map-id unsigned.apk fixed.apk da39a3e
+$ repro-apk fix-pg-map-id input-dir output-dir da39a3e
 $ repro-apk list-compresslevel some.apk
 $ repro-apk rm-files some.apk fixed.apk META-INF/MANIFEST.IN
 $ repro-apk sort-apk unsigned.apk sorted.apk
 $ repro-apk sort-baseline baseline.profm baseline-sorted.profm
 $ repro-apk sort-baseline --apk unsigned.apk sorted-baseline.apk
 $ repro-apk zipalign fixed.apk fixed-aligned-py.apk
 $ repro-apk zipinfo -e some.apk
@@ -694,14 +748,15 @@
 $ repro-apk diff-zip-meta --help
 $ repro-apk dump-arsc --help
 $ repro-apk dump-axml --help
 $ repro-apk dump-baseline --help
 $ repro-apk fix-compresslevel --help
 $ repro-apk fix-files --help
 $ repro-apk fix-newlines --help
+$ repro-apk fix-pg-map-id --help
 $ repro-apk list-compresslevel --help
 $ repro-apk rm-files --help
 $ repro-apk sort-apk --help
 $ repro-apk sort-baseline --help
 $ repro-apk zipalign --help
 $ repro-apk zipinfo --help
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: repro-apk Version: 0.2.4 Summary: scripts to make
+Metadata-Version: 2.1 Name: repro-apk Version: 0.2.5 Summary: scripts to make
 android apks reproducible Home-page: https://github.com/obfusk/reproducible-
 apk-tools Author: FC Stegerman Author-email: flx@obfusk.net License: GPLv3+
 Keywords: android apk reproducible Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology Classifier: Intended
 Audience :: System Administrators Classifier: Intended Audience ::
 Telecommunications Industry Classifier: License :: OSI Approved :: GNU General
@@ -23,30 +23,31 @@
 //pypi.python.org/pypi/repro-apk) [![Python Versions](https://img.shields.io/
 pypi/pyversions/repro-apk.svg)](https://pypi.python.org/pypi/repro-apk) [![CI]
 (https://github.com/obfusk/reproducible-apk-tools/workflows/CI/badge.svg)]
 (https://github.com/obfusk/reproducible-apk-tools/actions?query=workflow%3ACI)
 [![GPLv3+](https://img.shields.io/badge/license-GPLv3+-blue.svg)](https://
 www.gnu.org/licenses/gpl-3.0.html) # reproducible-apk-tools [`fix-
 compresslevel.py`](#fix-compresslevelpy), [`fix-files.py`](#fix-filespy),
-[`fix-newlines.py`](#fix-newlinespy), [`rm-files.py`](#rm-filespy), [`sort-
-apk.py`](#sort-apkpy), [`sort-baseline.py`](#sort-baselinepy), [`zipalign.py`]
-(#zipalignpy); [`diff-zip-meta.py`](#diff-zip-metapy), [`dump-arsc.py`](#dump-
-arscpy), [`dump-axml.py`](#dump-axmlpy), [`dump-baseline.py`](#dump-
-baselinepy), [`list-compresslevel.py`](#list-compresslevelpy), [`zipinfo.py`]
-(#zipinfopy); [`inplace-fix.py`](#inplace-fixpy). ## scripts to make android
-apks reproducible `reproducible-apk-tools` is a collection of scripts
-(available as subcommands of the `repro-apk` command) to help make APKs
-reproducible (e.g. by changing line endings from LF to CRLF), or find out why
-they are not (e.g. by comparing ZIP file metadata, or dumping `baseline.prof`
-files). ### fix-compresslevel.py Recompress with different compression level.
-Specify which files to change by providing at least one fnmatch-style pattern,
-e.g. `'assets/foo/*.bar'`. If two APKs have identical contents but some ZIP
-entries are compressed with a different compression level, thus making the APKs
-not bit-by-bit identical, this script may help. ```bash $ fix-compresslevel.py
---help usage: fix-compresslevel.py [-h] [-v] INPUT_APK OUTPUT_APK COMPRESSLEVEL
+[`fix-newlines.py`](#fix-newlinespy), [`fix-pg-map-id.py`](#fix-pg-map-idpy),
+[`rm-files.py`](#rm-filespy), [`sort-apk.py`](#sort-apkpy), [`sort-
+baseline.py`](#sort-baselinepy), [`zipalign.py`](#zipalignpy); [`diff-zip-
+meta.py`](#diff-zip-metapy), [`dump-arsc.py`](#dump-arscpy), [`dump-axml.py`]
+(#dump-axmlpy), [`dump-baseline.py`](#dump-baselinepy), [`list-
+compresslevel.py`](#list-compresslevelpy), [`zipinfo.py`](#zipinfopy);
+[`inplace-fix.py`](#inplace-fixpy). ## scripts to make android apks
+reproducible `reproducible-apk-tools` is a collection of scripts (available as
+subcommands of the `repro-apk` command) to help make APKs reproducible (e.g. by
+changing line endings from LF to CRLF), or find out why they are not (e.g. by
+comparing ZIP file metadata, or dumping `baseline.prof` files). ### fix-
+compresslevel.py Recompress with different compression level. Specify which
+files to change by providing at least one fnmatch-style pattern, e.g. `'assets/
+foo/*.bar'`. If two APKs have identical contents but some ZIP entries are
+compressed with a different compression level, thus making the APKs not bit-by-
+bit identical, this script may help. ```bash $ fix-compresslevel.py --help
+usage: fix-compresslevel.py [-h] [-v] INPUT_APK OUTPUT_APK COMPRESSLEVEL
 PATTERN [PATTERN ...] [...] $ apksigcopier compare signed.apk --unsigned
 unsigned.apk DOES NOT VERIFY [...] $ fix-compresslevel.py unsigned.apk
 fixed.apk 6 assets/foo/bar.js fixing 'assets/foo/bar.js'... $ zipalign -f 4
 fixed.apk fixed-aligned.apk $ apksigcopier compare signed.apk --unsigned fixed-
 aligned.apk && echo OK OK ``` NB: this builds a new ZIP file, preserving most
 ZIP metadata (and recompressing entries not matching the pattern using the same
 compression level as in the original APK) but not everything: e.g. copying the
@@ -79,14 +80,41 @@
 fix-newlines.py unsigned.apk fixed.apk 'META-INF/services/*' fixing 'META-INF/
 services/foo'... fixing 'META-INF/services/bar'... $ zipalign -f 4 fixed.apk
 fixed-aligned.apk $ apksigcopier compare signed.apk --unsigned fixed-
 aligned.apk && echo OK OK ``` NB: this builds a new ZIP file, preserving most
 ZIP metadata (and recompressing using the same compression level) but not
 everything: e.g. copying the existing local header extra fields which contain
 padding for alignment is not supported by Python's `ZipFile`, which is why
+`zipalign` is usually needed. ### fix-pg-map-id.py Replace non-deterministic R8
+`pg-map-id` in `classes.dex` (and `classes2.dex` etc. when present) and update
+checksums, also in `baseline.prof`. ```bash $ fix-pg-map-id.py --help usage:
+fix-pg-map-id.py [-h] INPUT_DIR_OR_APK OUTPUT_DIR_OR_APK PG_MAP_ID [...] $
+apksigcopier compare signed.apk --unsigned unsigned.apk DOES NOT VERIFY [...] $
+diff -Naur <( unzip -p signed.apk classes.dex | xxd ) <( unzip -p unsigned.apk
+classes.dex | xxd ) [...] -00000000: 6465 780a 3033 3500 829f 202e c800 6ecc
+dex.035... ...n. -00000010: c15c 0a17 3737 73fc 982e 34db 6239 bc52
+.\..77s...4.b9.R +00000000: 6465 780a 3033 3500 d89f 1795 f719 4d94
+dex.035.......M. +00000010: 8358 2526 2850 f9e5 ad3d e772 c82e 4f02 .X%&
+(P...=.r..O. [...] 005f1010: 2d61 7069 223a 3233 2c22 7067 2d6d 6170 -api":
+23,"pg-map -005f1020: 2d69 6422 3a22 3261 3939 3764 3322 2c22 -id":"2a997d3","
++005f1020: 2d69 6422 3a22 6565 3436 3531 3322 2c22 -id":"ee46513"," [...] $
+fix-pg-map-id.py unsigned.apk fixed.apk 2a997d3 reading 'assets/dexopt/
+baseline.prof'... reading 'classes.dex'... reading 'classes2.dex'... fixing
+'classes.dex'... dex version=035 fixing pg-map-id: b'ee46513' -> b'2a997d3'
+fixing signature: f7194d94835825262850f9e5ad3de772c82e4f02 -
+> c8006eccc15c0a17373773fc982e34db6239bc52 fixing checksum: 0x95179fd8 -
+> 0x2e209f82 fixing 'classes2.dex'... dex version=035 (not modified) fixing
+'assets/dexopt/baseline.prof'... prof version=010 P fixing 'classes.dex'
+checksum: 0x95d40f72 -> 0x50191ba4 writing 'assets/dexopt/baseline.prof'...
+writing 'classes.dex'... writing 'classes2.dex'... $ zipalign -f 4 fixed.apk
+fixed-aligned.apk $ apksigcopier compare signed.apk --unsigned fixed-
+aligned.apk && echo OK OK ``` NB: this builds a new ZIP file, preserving most
+ZIP metadata (and recompressing using the same compression level) but not
+everything: e.g. copying the existing local header extra fields which contain
+padding for alignment is not supported by Python's `ZipFile`, which is why
 `zipalign` is usually needed. ### rm-files.py Remove entries from ZIP file.
 Specify which files to remove by providing at least one fnmatch-style pattern,
 e.g. `'META-INF/MANIFEST.MF'`. ```bash $ rm-files.py --help usage: rm-files.py
 [-h] [-v] INPUT_APK OUTPUT_APK PATTERN [PATTERN ...] [...] $ rm-files.py
 some.apk fixed.apk META-INF/MANIFEST.IN skipping 'META-INF/MANIFEST.IN'... $
 zipalign -f 4 fixed.apk fixed-aligned.apk ``` NB: this builds a new ZIP file,
 preserving most ZIP metadata (and recompressing using the same compression
@@ -305,23 +333,25 @@
 repro-apk diff-zip-meta a.apk c.apk --no-offsets --no-ordering $ repro-apk
 dump-arsc resources.arsc $ repro-apk dump-arsc --apk some.apk $ repro-apk dump-
 axml foo.xml $ repro-apk dump-axml --apk some.apk res/foo.xml $ repro-apk dump-
 baseline baseline.prof $ repro-apk dump-baseline baseline.profm $ repro-apk
 dump-baseline --apk some.apk $ repro-apk fix-compresslevel unsigned.apk
 fixed.apk 6 assets/foo/bar.js $ repro-apk fix-files unsigned.apk fixed.apk
 unix2dos 'META-INF/services/*' $ repro-apk fix-newlines unsigned.apk fixed.apk
-'META-INF/services/*' $ repro-apk list-compresslevel some.apk $ repro-apk rm-
-files some.apk fixed.apk META-INF/MANIFEST.IN $ repro-apk sort-apk unsigned.apk
-sorted.apk $ repro-apk sort-baseline baseline.profm baseline-sorted.profm $
-repro-apk sort-baseline --apk unsigned.apk sorted-baseline.apk $ repro-apk
-zipalign fixed.apk fixed-aligned-py.apk $ repro-apk zipinfo -e some.apk $
-repro-apk zipinfo -l some.apk ``` ### Help ```bash $ repro-apk --help $ repro-
-apk diff-zip-meta --help $ repro-apk dump-arsc --help $ repro-apk dump-axml --
-help $ repro-apk dump-baseline --help $ repro-apk fix-compresslevel --help $
-repro-apk fix-files --help $ repro-apk fix-newlines --help $ repro-apk list-
+'META-INF/services/*' $ repro-apk fix-pg-map-id unsigned.apk fixed.apk da39a3e
+$ repro-apk fix-pg-map-id input-dir output-dir da39a3e $ repro-apk list-
+compresslevel some.apk $ repro-apk rm-files some.apk fixed.apk META-INF/
+MANIFEST.IN $ repro-apk sort-apk unsigned.apk sorted.apk $ repro-apk sort-
+baseline baseline.profm baseline-sorted.profm $ repro-apk sort-baseline --apk
+unsigned.apk sorted-baseline.apk $ repro-apk zipalign fixed.apk fixed-aligned-
+py.apk $ repro-apk zipinfo -e some.apk $ repro-apk zipinfo -l some.apk ``` ###
+Help ```bash $ repro-apk --help $ repro-apk diff-zip-meta --help $ repro-apk
+dump-arsc --help $ repro-apk dump-axml --help $ repro-apk dump-baseline --help
+$ repro-apk fix-compresslevel --help $ repro-apk fix-files --help $ repro-apk
+fix-newlines --help $ repro-apk fix-pg-map-id --help $ repro-apk list-
 compresslevel --help $ repro-apk rm-files --help $ repro-apk sort-apk --help $
 repro-apk sort-baseline --help $ repro-apk zipalign --help $ repro-apk zipinfo
 --help ``` ## Installing ### Using pip ```bash $ pip install repro-apk ``` NB:
 depending on your system you may need to use e.g. `pip3 --user` instead of just
 `pip`. ### From git NB: this installs the latest development version, not the
 latest release. ```bash $ git clone https://github.com/obfusk/reproducible-apk-
 tools.git $ cd reproducible-apk-tools $ pip install -e . ``` NB: you may need
```

### Comparing `repro-apk-0.2.4/repro_apk.egg-info/SOURCES.txt` & `repro-apk-0.2.5/repro_apk.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 repro_apk/diff_zip_meta.py
 repro_apk/dump_arsc.py
 repro_apk/dump_axml.py
 repro_apk/dump_baseline.py
 repro_apk/fix_compresslevel.py
 repro_apk/fix_files.py
 repro_apk/fix_newlines.py
+repro_apk/fix_pg_map_id.py
 repro_apk/inplace_fix.py
 repro_apk/list_compresslevel.py
 repro_apk/py.typed
 repro_apk/rm_files.py
 repro_apk/sort_apk.py
 repro_apk/sort_baseline.py
 repro_apk/zipalign.py
```

### Comparing `repro-apk-0.2.4/setup.py` & `repro-apk-0.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from pathlib import Path
 import setuptools
 
-__version__ = "0.2.4"
+__version__ = "0.2.5"
 
 info = Path(__file__).with_name("README.md").read_text(encoding="utf8")
 
 setuptools.setup(
     name="repro-apk",
     url="https://github.com/obfusk/reproducible-apk-tools",
     description="scripts to make android apks reproducible",
```

