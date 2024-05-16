# Comparing `tmp/deciphon-0.9.3.tar.gz` & `tmp/deciphon-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deciphon-0.9.3.tar", max compression
+gzip compressed data, was "deciphon-0.9.4.tar", max compression
```

## Comparing `deciphon-0.9.3.tar` & `deciphon-0.9.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1063 2023-08-10 11:58:47.998458 deciphon-0.9.3/LICENSE
--rw-r--r--   0        0        0     2996 2023-08-10 11:58:47.998458 deciphon-0.9.3/README.md
--rw-r--r--   0        0        0        0 2023-08-10 11:58:47.998458 deciphon-0.9.3/deciphon/__init__.py
--rw-r--r--   0        0        0      483 2023-08-10 11:58:47.998458 deciphon-0.9.3/deciphon/catch_validation.py
--rw-r--r--   0        0        0     4945 2023-08-10 11:58:47.998458 deciphon-0.9.3/deciphon/cli.py
--rw-r--r--   0        0        0      430 2023-08-10 11:58:47.998458 deciphon-0.9.3/deciphon/filetype.py
--rw-r--r--   0        0        0      248 2023-08-10 11:58:47.998458 deciphon-0.9.3/deciphon/gencode.py
--rw-r--r--   0        0        0      680 2023-08-10 11:58:47.998458 deciphon-0.9.3/deciphon/h3daemon.py
--rw-r--r--   0        0        0      213 2023-08-10 11:58:47.998458 deciphon-0.9.3/deciphon/hmmer_press.py
--rw-r--r--   0        0        0      775 2023-08-10 11:58:47.998458 deciphon-0.9.3/deciphon/models.py
--rw-r--r--   0        0        0       72 2023-08-10 11:58:47.998458 deciphon-0.9.3/deciphon/path_like.py
--rw-r--r--   0        0        0      522 2023-08-10 11:58:47.998458 deciphon-0.9.3/deciphon/percent.py
--rw-r--r--   0        0        0     1414 2023-08-10 11:58:47.998458 deciphon-0.9.3/deciphon/seq_file.py
--rw-r--r--   0        0        0      670 2023-08-10 11:58:47.998458 deciphon-0.9.3/deciphon/service_exit.py
--rw-r--r--   0        0        0      663 2023-08-10 11:58:47.998458 deciphon-0.9.3/pyproject.toml
--rw-r--r--   0        0        0     3863 1970-01-01 00:00:00.000000 deciphon-0.9.3/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-08-15 10:38:08.178797 deciphon-0.9.4/LICENSE
+-rw-r--r--   0        0        0     2996 2023-08-15 10:38:08.178797 deciphon-0.9.4/README.md
+-rw-r--r--   0        0        0        0 2023-08-15 10:38:08.178797 deciphon-0.9.4/deciphon/__init__.py
+-rw-r--r--   0        0        0      483 2023-08-15 10:38:08.178797 deciphon-0.9.4/deciphon/catch_validation.py
+-rw-r--r--   0        0        0     4928 2023-08-15 10:38:08.178797 deciphon-0.9.4/deciphon/cli.py
+-rw-r--r--   0        0        0      430 2023-08-15 10:38:08.178797 deciphon-0.9.4/deciphon/filetype.py
+-rw-r--r--   0        0        0      248 2023-08-15 10:38:08.178797 deciphon-0.9.4/deciphon/gencode.py
+-rw-r--r--   0        0        0      678 2023-08-15 10:38:08.178797 deciphon-0.9.4/deciphon/h3daemon.py
+-rw-r--r--   0        0        0      213 2023-08-15 10:38:08.178797 deciphon-0.9.4/deciphon/hmmer_press.py
+-rw-r--r--   0        0        0      775 2023-08-15 10:38:08.178797 deciphon-0.9.4/deciphon/models.py
+-rw-r--r--   0        0        0       72 2023-08-15 10:38:08.178797 deciphon-0.9.4/deciphon/path_like.py
+-rw-r--r--   0        0        0      522 2023-08-15 10:38:08.178797 deciphon-0.9.4/deciphon/percent.py
+-rw-r--r--   0        0        0     1414 2023-08-15 10:38:08.178797 deciphon-0.9.4/deciphon/seq_file.py
+-rw-r--r--   0        0        0      670 2023-08-15 10:38:08.178797 deciphon-0.9.4/deciphon/service_exit.py
+-rw-r--r--   0        0        0      709 2023-08-15 10:38:08.178797 deciphon-0.9.4/pyproject.toml
+-rw-r--r--   0        0        0     3863 1970-01-01 00:00:00.000000 deciphon-0.9.4/PKG-INFO
```

### Comparing `deciphon-0.9.3/LICENSE` & `deciphon-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `deciphon-0.9.3/README.md` & `deciphon-0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `deciphon-0.9.3/deciphon/cli.py` & `deciphon-0.9.4/deciphon/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 from __future__ import annotations
 
 import importlib.metadata
 from pathlib import Path
 from subprocess import DEVNULL
 from typing import Optional
 
-from deciphon_core.hmmfile import HMMFile
 from deciphon_core.press import PressContext
 from deciphon_core.scan import Scan
 from deciphon_core.scan_params import ScanParams
-from deciphon_core.snapfile import NewSnapFile
+from deciphon_core.schema import Gencode, HMMFile, NewSnapFile
 from deciphon_snap.read_snap import read_snap
 from deciphon_snap.view import view_alignments
 from rich.progress import track
 from typer import Argument, BadParameter, Exit, Option, Typer, echo
 
 from deciphon.catch_validation import catch_validation
 from deciphon.gencode import gencodes
@@ -71,15 +70,15 @@
     """
     with service_exit(), catch_validation():
         hmm = HMMFile(path=hmmfile)
 
         if force and hmm.path.with_suffix(".dcp"):
             hmm.path.with_suffix(".dcp").unlink()
 
-        with PressContext(hmm, gencode=gencode, epsilon=epsilon) as press:
+        with PressContext(hmm, gencode=Gencode(gencode), epsilon=epsilon) as press:
             for x in track([press] * press.nproteins, "Pressing", disable=not progress):
                 x.next()
             hmmer_press(hmm.path)
 
         file_dcp = hmm.path.with_suffix(".dcp")
         file_h3m = hmm.path.with_suffix(".h3m")
         file_h3i = hmm.path.with_suffix(".h3i")
```

### Comparing `deciphon-0.9.3/deciphon/h3daemon.py` & `deciphon-0.9.4/deciphon/h3daemon.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,11 @@
+from deciphon_core.schema import HMMFile
 from h3daemon.hmmfile import HMMFile as H3File
 from h3daemon.sched import SchedContext
 
-from deciphon_core.hmmfile import HMMFile
-
 __all__ = ["H3Daemon"]
 
 
 class H3Daemon:
     def __init__(self, hmmfile: HMMFile, stdout=None, stderr=None) -> None:
         self._hmmfile = hmmfile
         h3file = H3File(hmmfile.path)
```

### Comparing `deciphon-0.9.3/deciphon/models.py` & `deciphon-0.9.4/deciphon/models.py`

 * *Files identical despite different names*

### Comparing `deciphon-0.9.3/deciphon/percent.py` & `deciphon-0.9.4/deciphon/percent.py`

 * *Files identical despite different names*

### Comparing `deciphon-0.9.3/deciphon/seq_file.py` & `deciphon-0.9.4/deciphon/seq_file.py`

 * *Files identical despite different names*

### Comparing `deciphon-0.9.3/deciphon/service_exit.py` & `deciphon-0.9.4/deciphon/service_exit.py`

 * *Files identical despite different names*

### Comparing `deciphon-0.9.3/pyproject.toml` & `deciphon-0.9.4/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "deciphon"
-version = "0.9.3"
+version = "0.9.4"
 description = "Individually annotate long, error-prone nucleotide sequences into proteins"
 authors = ["Danilo Horta <horta@ebi.ac.uk>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "deciphon" }]
 
 [tool.poetry.dependencies]
@@ -19,13 +19,16 @@
 pydantic = "^2"
 typer = "^0"
 rich = "^13"
 
 [tool.poetry.group.dev.dependencies]
 pytest = ">=7.3.2"
 
-[build-system]
-requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
+[tool.pytest.ini_options]
+pythonpath = ["."]
 
 [tool.poetry.scripts]
 deci = 'deciphon.cli:app'
+
+[build-system]
+requires = ["poetry-core"]
+build-backend = "poetry.core.masonry.api"
```

### Comparing `deciphon-0.9.3/PKG-INFO` & `deciphon-0.9.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deciphon
-Version: 0.9.3
+Version: 0.9.4
 Summary: Individually annotate long, error-prone nucleotide sequences into proteins
 License: MIT
 Author: Danilo Horta
 Author-email: horta@ebi.ac.uk
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

