# Comparing `tmp/used_addr_check-0.1.1.tar.gz` & `tmp/used_addr_check-0.1.2.tar.gz`

## Comparing `used_addr_check-0.1.1.tar` & `used_addr_check-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,20 @@
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 used_addr_check-0.1.1/.cspell/custom-dictionary-workspace.txt
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 used_addr_check-0.1.1/.vscode/extensions.json
--rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 used_addr_check-0.1.1/.vscode/settings.json
--rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 used_addr_check-0.1.1/src/used_addr_check/__init__.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 used_addr_check-0.1.1/src/used_addr_check/__main__.py
--rw-r--r--   0        0        0     3223 2020-02-02 00:00:00.000000 used_addr_check-0.1.1/src/used_addr_check/cli.py
--rw-r--r--   0        0        0     2951 2020-02-02 00:00:00.000000 used_addr_check-0.1.1/src/used_addr_check/download_list.py
--rw-r--r--   0        0        0     4854 2020-02-02 00:00:00.000000 used_addr_check-0.1.1/src/used_addr_check/index_create.py
--rw-r--r--   0        0        0     4063 2020-02-02 00:00:00.000000 used_addr_check-0.1.1/src/used_addr_check/index_search.py
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 used_addr_check-0.1.1/src/used_addr_check/index_types.py
--rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 used_addr_check-0.1.1/src/used_addr_check/scan_file.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 used_addr_check-0.1.1/tests/test_1.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 used_addr_check-0.1.1/.gitignore
--rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 used_addr_check-0.1.1/LICENSE
--rw-r--r--   0        0        0     2802 2020-02-02 00:00:00.000000 used_addr_check-0.1.1/README.md
--rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 used_addr_check-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3679 2020-02-02 00:00:00.000000 used_addr_check-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 used_addr_check-0.1.2/.cspell/custom-dictionary-workspace.txt
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 used_addr_check-0.1.2/.vscode/extensions.json
+-rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 used_addr_check-0.1.2/.vscode/settings.json
+-rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 used_addr_check-0.1.2/src/used_addr_check/__init__.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 used_addr_check-0.1.2/src/used_addr_check/__main__.py
+-rw-r--r--   0        0        0     3223 2020-02-02 00:00:00.000000 used_addr_check-0.1.2/src/used_addr_check/cli.py
+-rw-r--r--   0        0        0     2951 2020-02-02 00:00:00.000000 used_addr_check-0.1.2/src/used_addr_check/download_list.py
+-rw-r--r--   0        0        0     4854 2020-02-02 00:00:00.000000 used_addr_check-0.1.2/src/used_addr_check/index_create.py
+-rw-r--r--   0        0        0     4063 2020-02-02 00:00:00.000000 used_addr_check-0.1.2/src/used_addr_check/index_search.py
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 used_addr_check-0.1.2/src/used_addr_check/index_types.py
+-rw-r--r--   0        0        0     4095 2020-02-02 00:00:00.000000 used_addr_check-0.1.2/src/used_addr_check/scan_file.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 used_addr_check-0.1.2/tests/test_1.py
+-rw-r--r--   0        0        0     1949 2020-02-02 00:00:00.000000 used_addr_check-0.1.2/tests/test_scan_file.py
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 used_addr_check-0.1.2/tests/test_data/scan_file_sample_1.txt
+-rw-r--r--   0        0        0     7816 2020-02-02 00:00:00.000000 used_addr_check-0.1.2/tests/test_data/scan_file_sample_2.txt
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 used_addr_check-0.1.2/.gitignore
+-rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 used_addr_check-0.1.2/LICENSE
+-rw-r--r--   0        0        0     2968 2020-02-02 00:00:00.000000 used_addr_check-0.1.2/README.md
+-rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 used_addr_check-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3876 2020-02-02 00:00:00.000000 used_addr_check-0.1.2/PKG-INFO
```

### Comparing `used_addr_check-0.1.1/.vscode/settings.json` & `used_addr_check-0.1.2/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `used_addr_check-0.1.1/src/used_addr_check/cli.py` & `used_addr_check-0.1.2/src/used_addr_check/cli.py`

 * *Files identical despite different names*

### Comparing `used_addr_check-0.1.1/src/used_addr_check/download_list.py` & `used_addr_check-0.1.2/src/used_addr_check/download_list.py`

 * *Files identical despite different names*

### Comparing `used_addr_check-0.1.1/src/used_addr_check/index_create.py` & `used_addr_check-0.1.2/src/used_addr_check/index_create.py`

 * *Files identical despite different names*

### Comparing `used_addr_check-0.1.1/src/used_addr_check/index_search.py` & `used_addr_check-0.1.2/src/used_addr_check/index_search.py`

 * *Files identical despite different names*

### Comparing `used_addr_check-0.1.1/.gitignore` & `used_addr_check-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `used_addr_check-0.1.1/LICENSE` & `used_addr_check-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `used_addr_check-0.1.1/README.md` & `used_addr_check-0.1.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -11,26 +11,32 @@
 * CLI and library options
 * Generates a binary search tree index from the text file, and then uses that to search for the address.
 
 ## Getting Started
 
 This project depends on the large address list being downloaded and extracted.
 
-1. Download the zipped text file of used addresses, where each line is a used Bitcoin address.
-
 ```bash
+# Download the zipped text file of used addresses, where each line is a used Bitcoin address.
 wget http://alladdresses.loyce.club/all_Bitcoin_addresses_ever_used_sorted.txt.gz
+
+# Extract the file
+gunzip -d ./all_Bitcoin_addresses_ever_used_sorted.txt.gz --stdout | pv > all_Bitcoin_addresses_ever_used_sorted.txt
 ```
 
-2. Extract the file:
+Optionally, if you intend to use the `scan_file` subcommand, install `ripgrep`
+from optimal performance:
 
 ```bash
-gunzip -d ./all_Bitcoin_addresses_ever_used_sorted.txt.gz --stdout | pv > all_Bitcoin_addresses_ever_used_sorted.txt
+# first, install cargo/rust
+# then, run:
+cargo install ripgrep
 ```
 
+
 ## Usage - CLI
 
 ```bash
 pip install used_addr_check
 
 # download and extract the required file:
 wget http://alladdresses.loyce.club/all_Bitcoin_addresses_ever_used_sorted.txt.gz
```

### Comparing `used_addr_check-0.1.1/pyproject.toml` & `used_addr_check-0.1.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "used_addr_check"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
     { name="RecRanger", email="RecRanger+package@proton.me" },
 ]
 description = "A tool to efficiently check if a Bitcoin Address has ever been used before"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
@@ -19,14 +19,15 @@
 dependencies = [
     "backoff~=2.2.1",
     "loguru~=0.7.2",
     "orjson~=3.10.1",
     "polars~=0.20.23",
     "requests~=2.31.0",
     "tqdm~=4.66.2",
+    "ripgrepy~=2.0.0",
 ]
 
 [project.optional-dependencies]
 dev = [
     "black~=24.4.2",
     "flake8~=7.0.0",
 ]
```

### Comparing `used_addr_check-0.1.1/PKG-INFO` & `used_addr_check-0.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.3
 Name: used_addr_check
-Version: 0.1.1
+Version: 0.1.2
 Summary: A tool to efficiently check if a Bitcoin Address has ever been used before
 Project-URL: Homepage, https://github.com/RecRanger/used-addr-check
 Project-URL: Issues, https://github.com/RecRanger/used-addr-check/issues
 Author-email: RecRanger <RecRanger+package@proton.me>
 License-File: LICENSE
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Requires-Dist: backoff~=2.2.1
 Requires-Dist: loguru~=0.7.2
 Requires-Dist: orjson~=3.10.1
 Requires-Dist: polars~=0.20.23
 Requires-Dist: requests~=2.31.0
+Requires-Dist: ripgrepy~=2.0.0
 Requires-Dist: tqdm~=4.66.2
 Provides-Extra: dev
 Requires-Dist: black~=24.4.2; extra == 'dev'
 Requires-Dist: flake8~=7.0.0; extra == 'dev'
 Provides-Extra: test
 Requires-Dist: pytest~=8.2.0; extra == 'test'
 Description-Content-Type: text/markdown
@@ -35,26 +36,32 @@
 * CLI and library options
 * Generates a binary search tree index from the text file, and then uses that to search for the address.
 
 ## Getting Started
 
 This project depends on the large address list being downloaded and extracted.
 
-1. Download the zipped text file of used addresses, where each line is a used Bitcoin address.
-
 ```bash
+# Download the zipped text file of used addresses, where each line is a used Bitcoin address.
 wget http://alladdresses.loyce.club/all_Bitcoin_addresses_ever_used_sorted.txt.gz
+
+# Extract the file
+gunzip -d ./all_Bitcoin_addresses_ever_used_sorted.txt.gz --stdout | pv > all_Bitcoin_addresses_ever_used_sorted.txt
 ```
 
-2. Extract the file:
+Optionally, if you intend to use the `scan_file` subcommand, install `ripgrep`
+from optimal performance:
 
 ```bash
-gunzip -d ./all_Bitcoin_addresses_ever_used_sorted.txt.gz --stdout | pv > all_Bitcoin_addresses_ever_used_sorted.txt
+# first, install cargo/rust
+# then, run:
+cargo install ripgrep
 ```
 
+
 ## Usage - CLI
 
 ```bash
 pip install used_addr_check
 
 # download and extract the required file:
 wget http://alladdresses.loyce.club/all_Bitcoin_addresses_ever_used_sorted.txt.gz
```

