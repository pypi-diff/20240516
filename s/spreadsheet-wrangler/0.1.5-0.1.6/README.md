# Comparing `tmp/spreadsheet_wrangler-0.1.5.tar.gz` & `tmp/spreadsheet_wrangler-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spreadsheet_wrangler-0.1.5.tar", last modified: Tue Dec  5 16:51:25 2023, max compression
+gzip compressed data, was "spreadsheet_wrangler-0.1.6.tar", last modified: Thu May 16 01:13:23 2024, max compression
```

## Comparing `spreadsheet_wrangler-0.1.5.tar` & `spreadsheet_wrangler-0.1.6.tar`

### file list

```diff
@@ -1,34 +1,49 @@
-drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-12-05 16:51:25.234467 spreadsheet_wrangler-0.1.5/
--rw-rw-r--   0 simon     (1000) simon     (1000)     3677 2023-10-28 15:56:47.000000 spreadsheet_wrangler-0.1.5/CONTRIBUTING.rst
--rw-rw-r--   0 simon     (1000) simon     (1000)       89 2023-10-28 15:56:47.000000 spreadsheet_wrangler-0.1.5/HISTORY.rst
--rw-rw-r--   0 simon     (1000) simon     (1000)     1070 2023-10-28 15:56:47.000000 spreadsheet_wrangler-0.1.5/LICENSE
--rw-rw-r--   0 simon     (1000) simon     (1000)      242 2023-10-28 15:56:47.000000 spreadsheet_wrangler-0.1.5/MANIFEST.in
--rw-rw-r--   0 simon     (1000) simon     (1000)     5039 2023-12-05 16:51:25.234467 spreadsheet_wrangler-0.1.5/PKG-INFO
--rw-rw-r--   0 simon     (1000) simon     (1000)     4186 2023-10-23 18:42:52.000000 spreadsheet_wrangler-0.1.5/README.md
-drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-12-05 16:51:25.234467 spreadsheet_wrangler-0.1.5/docs/
--rw-rw-r--   0 simon     (1000) simon     (1000)      621 2023-10-28 15:56:47.000000 spreadsheet_wrangler-0.1.5/docs/Makefile
--rwxrwxr-x   0 simon     (1000) simon     (1000)     4944 2023-10-28 15:56:47.000000 spreadsheet_wrangler-0.1.5/docs/conf.py
--rw-rw-r--   0 simon     (1000) simon     (1000)       33 2023-10-28 15:56:47.000000 spreadsheet_wrangler-0.1.5/docs/contributing.rst
--rw-rw-r--   0 simon     (1000) simon     (1000)       28 2023-10-28 15:56:47.000000 spreadsheet_wrangler-0.1.5/docs/history.rst
--rw-rw-r--   0 simon     (1000) simon     (1000)      306 2023-10-28 15:56:47.000000 spreadsheet_wrangler-0.1.5/docs/index.rst
--rw-rw-r--   0 simon     (1000) simon     (1000)     1214 2023-10-28 15:56:47.000000 spreadsheet_wrangler-0.1.5/docs/installation.rst
--rw-rw-r--   0 simon     (1000) simon     (1000)      818 2023-10-28 15:56:47.000000 spreadsheet_wrangler-0.1.5/docs/make.bat
--rw-rw-r--   0 simon     (1000) simon     (1000)       27 2023-10-28 15:56:47.000000 spreadsheet_wrangler-0.1.5/docs/readme.rst
--rw-rw-r--   0 simon     (1000) simon     (1000)       95 2023-10-28 15:56:47.000000 spreadsheet_wrangler-0.1.5/docs/usage.rst
--rw-rw-r--   0 simon     (1000) simon     (1000)      392 2023-12-05 16:51:25.234467 spreadsheet_wrangler-0.1.5/setup.cfg
--rw-rw-r--   0 simon     (1000) simon     (1000)     1568 2023-10-28 16:05:05.000000 spreadsheet_wrangler-0.1.5/setup.py
-drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-12-05 16:51:25.234467 spreadsheet_wrangler-0.1.5/spreadsheet_wrangler/
--rw-rw-r--   0 simon     (1000) simon     (1000)      185 2023-10-28 16:08:14.000000 spreadsheet_wrangler-0.1.5/spreadsheet_wrangler/__init__.py
--rw-rw-r--   0 simon     (1000) simon     (1000)    11528 2023-10-31 01:03:46.000000 spreadsheet_wrangler-0.1.5/spreadsheet_wrangler/cli.py
--rw-rw-r--   0 simon     (1000) simon     (1000)     9229 2023-10-28 15:58:25.000000 spreadsheet_wrangler-0.1.5/spreadsheet_wrangler/spreadsheet_wrangler.py
-drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-12-05 16:51:25.234467 spreadsheet_wrangler-0.1.5/spreadsheet_wrangler.egg-info/
--rw-rw-r--   0 simon     (1000) simon     (1000)     5039 2023-12-05 16:51:25.000000 spreadsheet_wrangler-0.1.5/spreadsheet_wrangler.egg-info/PKG-INFO
--rw-rw-r--   0 simon     (1000) simon     (1000)      693 2023-12-05 16:51:25.000000 spreadsheet_wrangler-0.1.5/spreadsheet_wrangler.egg-info/SOURCES.txt
--rw-rw-r--   0 simon     (1000) simon     (1000)        1 2023-12-05 16:51:25.000000 spreadsheet_wrangler-0.1.5/spreadsheet_wrangler.egg-info/dependency_links.txt
--rw-rw-r--   0 simon     (1000) simon     (1000)       72 2023-12-05 16:51:25.000000 spreadsheet_wrangler-0.1.5/spreadsheet_wrangler.egg-info/entry_points.txt
--rw-rw-r--   0 simon     (1000) simon     (1000)        1 2023-12-05 16:51:25.000000 spreadsheet_wrangler-0.1.5/spreadsheet_wrangler.egg-info/not-zip-safe
--rw-rw-r--   0 simon     (1000) simon     (1000)       40 2023-12-05 16:51:25.000000 spreadsheet_wrangler-0.1.5/spreadsheet_wrangler.egg-info/requires.txt
--rw-rw-r--   0 simon     (1000) simon     (1000)       21 2023-12-05 16:51:25.000000 spreadsheet_wrangler-0.1.5/spreadsheet_wrangler.egg-info/top_level.txt
-drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2023-12-05 16:51:25.234467 spreadsheet_wrangler-0.1.5/tests/
--rw-rw-r--   0 simon     (1000) simon     (1000)        0 2021-04-30 03:35:54.000000 spreadsheet_wrangler-0.1.5/tests/__init__.py
--rw-rw-r--   0 simon     (1000) simon     (1000)     1955 2021-04-30 03:35:54.000000 spreadsheet_wrangler-0.1.5/tests/test_spreadsheet_wrangler.py
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2024-05-16 01:13:23.796689 spreadsheet_wrangler-0.1.6/
+-rw-rw-r--   0 simon     (1000) simon     (1000)     1799 2021-04-30 03:35:54.000000 spreadsheet_wrangler-0.1.6/.gitignore
+-rw-rw-r--   0 simon     (1000) simon     (1000)     1192 2024-05-16 01:06:31.000000 spreadsheet_wrangler-0.1.6/.pre-commit-config.yaml
+-rw-rw-r--   0 simon     (1000) simon     (1000)     3677 2023-10-28 15:56:47.000000 spreadsheet_wrangler-0.1.6/CONTRIBUTING.rst
+-rw-rw-r--   0 simon     (1000) simon     (1000)       89 2023-10-28 15:56:47.000000 spreadsheet_wrangler-0.1.6/HISTORY.rst
+-rw-rw-r--   0 simon     (1000) simon     (1000)     1069 2024-05-14 13:02:17.000000 spreadsheet_wrangler-0.1.6/LICENSE
+-rw-rw-r--   0 simon     (1000) simon     (1000)      242 2023-10-28 15:56:47.000000 spreadsheet_wrangler-0.1.6/MANIFEST.in
+-rw-rw-r--   0 simon     (1000) simon     (1000)     2300 2024-05-16 00:34:09.000000 spreadsheet_wrangler-0.1.6/Makefile
+-rw-r--r--   0 simon     (1000) simon     (1000)     6123 2024-05-16 01:13:23.796689 spreadsheet_wrangler-0.1.6/PKG-INFO
+-rw-rw-r--   0 simon     (1000) simon     (1000)     4184 2024-05-14 13:02:17.000000 spreadsheet_wrangler-0.1.6/README.md
+-rw-rw-r--   0 simon     (1000) simon     (1000)    84272 2022-11-10 15:18:00.000000 spreadsheet_wrangler-0.1.6/clustered_on_comment_and_footprint.png
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2024-05-16 01:13:23.792689 spreadsheet_wrangler-0.1.6/docs/
+-rw-rw-r--   0 simon     (1000) simon     (1000)      621 2023-10-28 15:56:47.000000 spreadsheet_wrangler-0.1.6/docs/Makefile
+-rwxrwxr-x   0 simon     (1000) simon     (1000)     4944 2023-10-28 15:56:47.000000 spreadsheet_wrangler-0.1.6/docs/conf.py
+-rw-rw-r--   0 simon     (1000) simon     (1000)       33 2023-10-28 15:56:47.000000 spreadsheet_wrangler-0.1.6/docs/contributing.rst
+-rw-rw-r--   0 simon     (1000) simon     (1000)       28 2023-10-28 15:56:47.000000 spreadsheet_wrangler-0.1.6/docs/history.rst
+-rw-rw-r--   0 simon     (1000) simon     (1000)      306 2023-10-28 15:56:47.000000 spreadsheet_wrangler-0.1.6/docs/index.rst
+-rw-rw-r--   0 simon     (1000) simon     (1000)     1214 2023-10-28 15:56:47.000000 spreadsheet_wrangler-0.1.6/docs/installation.rst
+-rw-rw-r--   0 simon     (1000) simon     (1000)      818 2023-10-28 15:56:47.000000 spreadsheet_wrangler-0.1.6/docs/make.bat
+-rw-rw-r--   0 simon     (1000) simon     (1000)       97 2024-05-16 00:38:34.000000 spreadsheet_wrangler-0.1.6/docs/modules.rst
+-rw-rw-r--   0 simon     (1000) simon     (1000)       27 2023-10-28 15:56:47.000000 spreadsheet_wrangler-0.1.6/docs/readme.rst
+-rw-rw-r--   0 simon     (1000) simon     (1000)      587 2024-05-16 00:38:34.000000 spreadsheet_wrangler-0.1.6/docs/spreadsheet_wrangler.rst
+-rw-rw-r--   0 simon     (1000) simon     (1000)       95 2023-10-28 15:56:47.000000 spreadsheet_wrangler-0.1.6/docs/usage.rst
+-rw-rw-r--   0 simon     (1000) simon     (1000)     3873 2024-05-16 01:12:46.000000 spreadsheet_wrangler-0.1.6/pyproject.toml
+-rw-rw-r--   0 simon     (1000) simon     (1000)       47 2024-05-16 00:51:51.000000 spreadsheet_wrangler-0.1.6/requirements.txt
+-rw-rw-r--   0 simon     (1000) simon     (1000)      146 2024-05-14 13:02:17.000000 spreadsheet_wrangler-0.1.6/requirements_dev.txt
+-rw-rw-r--   0 simon     (1000) simon     (1000)      398 2024-05-16 01:13:23.796689 spreadsheet_wrangler-0.1.6/setup.cfg
+-rw-rw-r--   0 simon     (1000) simon     (1000)       61 2024-05-16 00:25:35.000000 spreadsheet_wrangler-0.1.6/setup.py
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2024-05-16 01:13:23.792689 spreadsheet_wrangler-0.1.6/spreadsheet_wrangler/
+-rw-rw-r--   0 simon     (1000) simon     (1000)      292 2023-10-28 15:56:47.000000 spreadsheet_wrangler-0.1.6/spreadsheet_wrangler/.editorconfig
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2024-05-16 01:13:23.796689 spreadsheet_wrangler-0.1.6/spreadsheet_wrangler/.github/
+-rw-rw-r--   0 simon     (1000) simon     (1000)      331 2023-10-28 15:56:47.000000 spreadsheet_wrangler-0.1.6/spreadsheet_wrangler/.github/ISSUE_TEMPLATE.md
+-rw-rw-r--   0 simon     (1000) simon     (1000)     1204 2023-10-28 15:56:47.000000 spreadsheet_wrangler-0.1.6/spreadsheet_wrangler/.gitignore
+-rw-rw-r--   0 simon     (1000) simon     (1000)      696 2023-10-28 15:56:47.000000 spreadsheet_wrangler-0.1.6/spreadsheet_wrangler/.travis.yml
+-rw-rw-r--   0 simon     (1000) simon     (1000)     1330 2024-05-16 01:12:46.000000 spreadsheet_wrangler-0.1.6/spreadsheet_wrangler/__init__.py
+-rw-rw-r--   0 simon     (1000) simon     (1000)    12154 2024-05-16 01:02:46.000000 spreadsheet_wrangler-0.1.6/spreadsheet_wrangler/cli.py
+-rw-rw-r--   0 simon     (1000) simon     (1000)     9368 2024-05-16 01:11:26.000000 spreadsheet_wrangler-0.1.6/spreadsheet_wrangler/spreadsheet_wrangler.py
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2024-05-16 01:13:23.796689 spreadsheet_wrangler-0.1.6/spreadsheet_wrangler.egg-info/
+-rw-r--r--   0 simon     (1000) simon     (1000)     6123 2024-05-16 01:13:23.000000 spreadsheet_wrangler-0.1.6/spreadsheet_wrangler.egg-info/PKG-INFO
+-rw-rw-r--   0 simon     (1000) simon     (1000)     1008 2024-05-16 01:13:23.000000 spreadsheet_wrangler-0.1.6/spreadsheet_wrangler.egg-info/SOURCES.txt
+-rw-rw-r--   0 simon     (1000) simon     (1000)        1 2024-05-16 01:13:23.000000 spreadsheet_wrangler-0.1.6/spreadsheet_wrangler.egg-info/dependency_links.txt
+-rw-rw-r--   0 simon     (1000) simon     (1000)       71 2024-05-16 01:13:23.000000 spreadsheet_wrangler-0.1.6/spreadsheet_wrangler.egg-info/entry_points.txt
+-rw-rw-r--   0 simon     (1000) simon     (1000)       47 2024-05-16 01:13:23.000000 spreadsheet_wrangler-0.1.6/spreadsheet_wrangler.egg-info/requires.txt
+-rw-rw-r--   0 simon     (1000) simon     (1000)       21 2024-05-16 01:13:23.000000 spreadsheet_wrangler-0.1.6/spreadsheet_wrangler.egg-info/top_level.txt
+drwxrwxr-x   0 simon     (1000) simon     (1000)        0 2024-05-16 01:13:23.796689 spreadsheet_wrangler-0.1.6/tests/
+-rw-rw-r--   0 simon     (1000) simon     (1000)        0 2021-04-30 03:35:54.000000 spreadsheet_wrangler-0.1.6/tests/__init__.py
+-rw-rw-r--   0 simon     (1000) simon     (1000)     1786 2024-05-16 00:57:37.000000 spreadsheet_wrangler-0.1.6/tests/test_spreadsheet_wrangler.py
+-rw-rw-r--   0 simon     (1000) simon     (1000)      364 2024-05-16 00:35:31.000000 spreadsheet_wrangler-0.1.6/tox.ini
+-rw-rw-r--   0 simon     (1000) simon     (1000)    42690 2022-11-10 15:00:53.000000 spreadsheet_wrangler-0.1.6/unclustered_bom.png
```

### Comparing `spreadsheet_wrangler-0.1.5/CONTRIBUTING.rst` & `spreadsheet_wrangler-0.1.6/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `spreadsheet_wrangler-0.1.5/LICENSE` & `spreadsheet_wrangler-0.1.6/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -15,8 +15,7 @@
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
-
```

### Comparing `spreadsheet_wrangler-0.1.5/PKG-INFO` & `spreadsheet_wrangler-0.1.6/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,7 @@
-Metadata-Version: 2.1
-Name: spreadsheet_wrangler
-Version: 0.1.5
-Summary: Spreadsheet editing tools
-Home-page: https://github.com/snhobbs/spreadsheet-wrangler
-Author: Simon Hobbs
-Author-email: simon.hobbs@electrooptical.net
-License: MIT license
-Keywords: spreadsheet_wrangler
-Platform: UNKNOWN
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # spreadsheet-wrangler
 Command line tool for interacting with spreadsheet data
 
 ## Installation
 ### pypi
 ```
 pip install spreadsheet-wrangler
@@ -58,15 +36,15 @@
 
 ### Compare the data in two BOMS
 To compare the available data of two BOMs to compare function of spreadsheet_wrangler should be used. If a BOM was exported
 and needs to be checked against another with questionable history run:
 ```
 spreadsheet_wrangler.py compare --on="ref-des" -l bom.xlsx -r bom_Merged_data_store_On_pn.xlsx
 ```
-This will compare the original BOM with the merged one from the first example. Comparisons are done column by column with rows matched by the value in the column passed with the argument "--on". This should be a unique for each instance of a part (i.e a ref des). 
+This will compare the original BOM with the merged one from the first example. Comparisons are done column by column with rows matched by the value in the column passed with the argument "--on". This should be a unique for each instance of a part (i.e a ref des).
 The shared columns will be checked as well as any passed in with the --columns argument. Discrepancies are printed to screen.
 
 ### Generate a BOM sorted by the type of parts
 BOMs used for ordering, shipping, budgeting, or shipping to a CM are typically ordered by the type of part.
 
 The ordering BOM sorts by reference designator and combines the BOM into unique part types. This can then be used for ordering or quoting. This can be passed to a tool like kicost or used with supplier BOM Managers or the Octopart BOM Manager (recommended).
 
@@ -82,31 +60,19 @@
 spreadsheet_wrangler.py uncluster --column="ref-des" -s bom_unclustered.xlsx
 ```
 This will separate the lines like the original bom.xlsx. This BOM can now be compared using the compare function described above.
 
 NOTE: Note the data in each grouped row is duplicated for each clustered element. This is not necessarily correct if data was dissimilar and lost during the clustering step.
 
 ### Clustering a partially filled in BOM
-After exporting a design BOM with each component in it's own line you end up with what I call a design BOM except without the useful fields included. 
+After exporting a design BOM with each component in it's own line you end up with what I call a design BOM except without the useful fields included.
 
 ![unclustered BOM](unclustered_bom.png)
 
 For this I want to cluster based on "Comment" and "Footprint", that is I want all 0603 10K resistors together and not include any other 0603 or 10K parts in the cluster. The command would then be:
 
 ```
 spreadsheet_wrangler.py cluster --spreadsheet BOM-1x2_tester.csv --column "Designator" --on "Comment" --on "Footprint" -o BOM_clustered.xlsx
 ```
 This call turns the above BOM into:
 
 ![clustered on comment and footprint](clustered_on_comment_and_footprint.png)
-
-
-=======
-History
-=======
-
-0.1.4 (2023-10-28)
-------------------
-
-* First release on PyPI.
-
-
```

### Comparing `spreadsheet_wrangler-0.1.5/docs/Makefile` & `spreadsheet_wrangler-0.1.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `spreadsheet_wrangler-0.1.5/docs/conf.py` & `spreadsheet_wrangler-0.1.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `spreadsheet_wrangler-0.1.5/docs/installation.rst` & `spreadsheet_wrangler-0.1.6/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `spreadsheet_wrangler-0.1.5/docs/make.bat` & `spreadsheet_wrangler-0.1.6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `spreadsheet_wrangler-0.1.5/spreadsheet_wrangler/cli.py` & `spreadsheet_wrangler-0.1.6/spreadsheet_wrangler/cli.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,223 +1,372 @@
 """Console script for spreadsheet_wrangler."""
-import sys
+
+import re
+from pathlib import Path
+
 import click
-from . import *
+import pandas as pd
+
+from . import cluster
+from . import compare
+from . import extract_columns_by_pseudonyms
 from . import get_supported_file_formats
+from . import read_file_to_df
+from . import read_pseodonyms
+from . import select_on_value
+from . import uncluster
+from . import write
+
 
 @click.group()
 def gr1():
     pass
 
 
 @click.option("--fout", "-o", type=str, default=None, help="Generatated spreadsheet")
 @click.option("--spreadsheet", "-s", type=str, required=True, help="Main spreadsheet")
-@click.option("--on", type=str, multiple=True, required=True, help="Column to compare value")
+@click.option(
+    "--on", type=str, multiple=True, required=True, help="Column to compare value"
+)
 @click.option("--column", type=str, required=True, help="Column to cluster into array")
-@click.option("--pseudonyms", "-p", type=str, default="", help="Alternative column names in json format")
-@click.option("--format", type=click.Choice(get_supported_file_formats()), default="xlsx", help="Generatated spreadsheet format")
-@gr1.command("cluster", help='''Cluster spreadsheet by column value''')
-def cluster_command(fout, spreadsheet, on, column, pseudonyms, format):
-    pseudonyms=read_pseodonyms(pseudonyms)
+@click.option(
+    "--pseudonyms",
+    "-p",
+    type=str,
+    default="",
+    help="Alternative column names in json format",
+)
+@click.option(
+    "--format",
+    "format_",
+    type=click.Choice(get_supported_file_formats()),
+    default="xlsx",
+    help="Generatated spreadsheet format",
+)
+@gr1.command("cluster", help="""Cluster spreadsheet by column value""")
+def cluster_command(fout, spreadsheet, on, column, pseudonyms, format_):
+    pseudonyms = read_pseodonyms(pseudonyms)
     df = extract_columns_by_pseudonyms(read_file_to_df(spreadsheet), pseudonyms)
     if fout is None:
-        base = os.path.split(os.path.splitext(spreadsheet)[0])[-1]
-        fname = f'{base}_Clustered_On_{column}.{format}'
+        base = Path(spreadsheet).stem
+        fname = f"{base}_Clustered_On_{column}.{format_}"
     else:
         fname = fout
     clustered_df = cluster(df, on, column)
     clustered_df[column] = [",".join(pt) for pt in clustered_df[column]]
     write(clustered_df, fname, index=False)
 
 
 @click.option("--fout", "-o", type=str, default=None, help="Generatated spreadsheet")
 @click.option("--spreadsheet", "-s", type=str, required=True, help="Main spreadsheet")
 @click.option("--column", type=str, required=True, help="Clustered column")
-@click.option("--pseudonyms", "-p", type=str, default="", help="Alternative column names in json format")
-@click.option("--format", type=click.Choice(get_supported_file_formats()), default="xlsx", help="Generatated spreadsheet format")
-@gr1.command("uncluster", help='''Uncluster spreadsheet by column value''')
-def uncluster_command(fout, spreadsheet, column, pseudonyms, format):
-    pseudonyms=read_pseodonyms(pseudonyms)
+@click.option(
+    "--pseudonyms",
+    "-p",
+    type=str,
+    default="",
+    help="Alternative column names in json format",
+)
+@click.option(
+    "--format",
+    "format_",
+    type=click.Choice(get_supported_file_formats()),
+    default="xlsx",
+    help="Generatated spreadsheet format",
+)
+@gr1.command("uncluster", help="""Uncluster spreadsheet by column value""")
+def uncluster_command(fout, spreadsheet, column, pseudonyms, format_):
+    pseudonyms = read_pseodonyms(pseudonyms)
     df = extract_columns_by_pseudonyms(read_file_to_df(spreadsheet), pseudonyms)
     if fout is None:
-        base = os.path.split(os.path.splitext(spreadsheet)[0])[-1]
-        fname = f'{base}_Unclustered_On_{column}.{format}'
+        base = Path(spreadsheet).stem
+        fname = f"{base}_Unclustered_On_{column}.{format_}"
     else:
         fname = fout
     write(uncluster(df, column), fname, index=False)
 
 
 @click.option("--fout", "-o", type=str, default=None, help="Generatated spreadsheet")
-@click.option("-l", type=str, required=True, help="Left merge")
-@click.option("-r", type=str, required=True, help="Right merge")
+@click.option("--left", "-l", type=str, required=True, help="Left merge")
+@click.option("--right", "-r", type=str, required=True, help="Right merge")
 @click.option("--on", type=str, required=True, help="Column to merge on")
-@click.option("--method", default="left", type=click.Choice(["left", "right", "outer", "inner"]), help="Column to merge on")
-@click.option("--pseudonyms", "-p", type=str, default="", help="Alternative column names in json format")
-@click.option("--format", type=click.Choice(get_supported_file_formats()), default="xlsx", help="Generatated spreadsheet format")
-@gr1.command(help='''Merge two spreadsheets on the given column''')
-def merge(fout, l, r, on, method, pseudonyms, format):
-    pseudonyms=read_pseodonyms(pseudonyms)
-    left = extract_columns_by_pseudonyms(read_file_to_df(l), pseudonyms)
-    right = extract_columns_by_pseudonyms(read_file_to_df(r), pseudonyms)
-    df = left.merge(right, on=on, how=method) # include all DNPs, unknown parts won't cause an error
-    fname_l = os.path.split(os.path.splitext(l)[0])[-1]
-    fname_r = os.path.split(os.path.splitext(r)[0])[-1]
-    if fout is None:
-        fname = f'{fname_l}_Merged{fname_r}_On_{on}.{format}'
-    else:
-        fname = fout
+@click.option(
+    "--method",
+    default="left",
+    type=click.Choice(["left", "right", "outer", "inner"]),
+    help="Column to merge on",
+)
+@click.option(
+    "--pseudonyms",
+    "-p",
+    type=str,
+    default="",
+    help="Alternative column names in json format",
+)
+@click.option(
+    "--format",
+    "format_",
+    type=click.Choice(get_supported_file_formats()),
+    default="xlsx",
+    help="Generatated spreadsheet format",
+)
+@gr1.command(help="""Merge two spreadsheets on the given column""")
+def merge(fout, left, right, on, method, pseudonyms, format_):
+    pseudonyms = read_pseodonyms(pseudonyms)
+    left_df = extract_columns_by_pseudonyms(read_file_to_df(left), pseudonyms)
+    right_df = extract_columns_by_pseudonyms(read_file_to_df(right), pseudonyms)
+    df = left_df.merge(
+        right_df, on=on, how=method
+    )  # include all DNPs, unknown parts won't cause an error
+    fname_l = Path(left).stem
+    fname_r = Path(right).stem
+    fname = f"{fname_l}_Merged{fname_r}_On_{on}.{format_}" if fout is None else fout
     write(df, fname, index=False)
 
 
-@click.option("-l", type=str, required=True, help="First spreadsheet")
-@click.option("-r", type=str, required=True, help="Second spreadsheet")
+@click.option("--left", "-l", type=str, required=True, help="First spreadsheet")
+@click.option("--right", "-r", type=str, required=True, help="Second spreadsheet")
 @click.option("--on", type=str, default=None, help="Column to compare on")
-@click.option("--columns", "-c", multiple=True, type=str, default=None, help="Columns to check, leave blank to check all with same name")
-@click.option("--pseudonyms", "-p", type=str, default="", help="Alternative column names in json format")
-@gr1.command("compare", help="Compares the given columns, passes if all given columns exist in both files and values are the same")
-def compare_command(l, r, on, columns, pseudonyms):
-    pseudonyms=read_pseodonyms(pseudonyms)
-    left = extract_columns_by_pseudonyms(read_file_to_df(l), pseudonyms)
-    right = extract_columns_by_pseudonyms(read_file_to_df(r), pseudonyms)
+@click.option(
+    "--columns",
+    "-c",
+    multiple=True,
+    type=str,
+    default=None,
+    help="Columns to check, leave blank to check all with same name",
+)
+@click.option(
+    "--pseudonyms",
+    "-p",
+    type=str,
+    default="",
+    help="Alternative column names in json format",
+)
+@gr1.command(
+    "compare",
+    help="Compares the given columns, passes if all given columns exist in both files and values are the same",
+)
+def compare_command(left, right, on, columns, pseudonyms):
+    pseudonyms = read_pseodonyms(pseudonyms)
+    left_df = extract_columns_by_pseudonyms(read_file_to_df(left), pseudonyms)
+    right_df = extract_columns_by_pseudonyms(read_file_to_df(right), pseudonyms)
     if columns is None:
-        columns = set(left.columns).intersection(set(right.columns))
+        columns = set(left_df.columns).intersection(set(right_df.columns))
 
-    errors = compare(left, right, columns, on)
-    print("Comparing columns:", columns)
-    for _, row in pd.DataFrame(errors).iterrows():
-        print("[{}:{}] Comparison Failure: {}".format(row["column"], row["line"], row["description"]))
+    errors = compare(left_df, right_df, columns, on)
+    for _, _row in pd.DataFrame(errors).iterrows():
+        pass
 
 
 @click.option("--fin", "-i", type=str, required=True, help="Input spreadsheet")
 @click.option("--fout", "-o", type=str, default=None, help="Generatated spreadsheet")
 @click.option("--value", type=str, required=True, help="Value to select")
 @click.option("--column", "-c", type=str, required=True, help="Column to filter on")
-@click.option("--blank-defaults", is_flag=True, help="Include unmatched rows with no value in column")
-@click.option("--pseudonyms", "-p", type=str, default="", help="Alternative column names in json format")
-@click.option("--format", type=click.Choice(get_supported_file_formats()), default="xlsx", help="Generatated spreadsheet format")
-@gr1.command("filter", help="Compares the given columns, selects the row if all given columns exist in both files and values are the same")
-def filter_command(fin, fout, value, column, blank_defaults, pseudonyms, format):
+@click.option(
+    "--blank-defaults",
+    is_flag=True,
+    help="Include unmatched rows with no value in column",
+)
+@click.option(
+    "--pseudonyms",
+    "-p",
+    type=str,
+    default="",
+    help="Alternative column names in json format",
+)
+@click.option(
+    "--format",
+    "format_",
+    type=click.Choice(get_supported_file_formats()),
+    default="xlsx",
+    help="Generatated spreadsheet format",
+)
+@gr1.command(
+    "filter",
+    help="Compares the given columns, selects the row if all given columns exist in both files and values are the same",
+)
+def filter_command(fin, fout, value, column, blank_defaults, pseudonyms, format_):
     pseudonyms = read_pseodonyms(pseudonyms)
     df = extract_columns_by_pseudonyms(read_file_to_df(fin), pseudonyms)
-    filtered_df = select_on_value(df, column=column, value=value, blank_defaults=blank_defaults)
+    filtered_df = select_on_value(
+        df, column=column, value=value, blank_defaults=blank_defaults
+    )
     if fout is None:
-        base = os.path.split(os.path.splitext(fin)[0])[-1]
-        fname = f'{base}_Filtered_On_{column}_by_{value}.{format}'
+        base = Path(fin).stem
+        fname = f"{base}_Filtered_On_{column}_by_{value}.{format_}"
     else:
         fname = fout
     write(filtered_df, fname, index=False)
 
 
 @click.option("--fin", "-i", type=str, required=True, help="Input spreadsheet")
 @click.option("--fout", "-o", type=str, default=None, help="Generatated spreadsheet")
-@click.option("--pseudonyms", "-p", type=str, default="", help="Alternative column names in json format")
-@click.option("--format", type=click.Choice(get_supported_file_formats()), default="xlsx", help="Generatated spreadsheet format")
-@gr1.command("translate", help="Compares the given columns, passes if all given columns exist in both files and values are the same")
-def translate_command(fin, fout, pseudonyms, format):
+@click.option(
+    "--pseudonyms",
+    "-p",
+    type=str,
+    default="",
+    help="Alternative column names in json format",
+)
+@click.option(
+    "--format",
+    "format_",
+    type=click.Choice(get_supported_file_formats()),
+    default="xlsx",
+    help="Generatated spreadsheet format",
+)
+@gr1.command(
+    "translate",
+    help="Compares the given columns, passes if all given columns exist in both files and values are the same",
+)
+def translate_command(fin, fout, pseudonyms, format_):
     pseudonyms = read_pseodonyms(pseudonyms)
     df = extract_columns_by_pseudonyms(read_file_to_df(fin), pseudonyms)
 
     if fout is None:
-        base = os.path.split(os.path.splitext(fin)[0])[-1]
-        if format is not None:
-            fout = f"{base}.{format}"
-        else:
-            fout = fin
+        base = Path(fin).stem
+        fout = f"{base}.{format_}" if format_ is not None else fin
 
     write(df, fout, index=False)
 
 
 @click.option("--fin", "-i", type=str, required=True, help="Input spreadsheet")
 @click.option("--fout", "-o", type=str, default=None, help="Generatated spreadsheet")
 @gr1.command("to_md", help="Generate a markdown table")
 def to_md(fin, fout):
     df = read_file_to_df(fin)
-    with open(fout, "w") as f:
+    with Path(fout).open("w") as f:
         f.write(df.to_markdown())
 
+
 @click.option("--fin", "-i", type=str, required=True, help="Input spreadsheet")
 @click.option("--fout", "-o", type=str, default=None, help="Generatated spreadsheet")
-@click.option("--column", "-c", type=str, required=True, help="Column to use as primary value")
+@click.option(
+    "--column", "-c", type=str, required=True, help="Column to use as primary value"
+)
 @click.option("--delimiter", "-d", type=str, required=True, help="Current delimiter")
 @click.option("--new-delimiter", "-n", type=str, required=True, help="New delimiter")
-@click.option("--pseudonyms", "-p", type=str, default="", help="Alternative column names in json format")
-@click.option("--format", type=click.Choice(get_supported_file_formats()), default="xlsx", help="Generatated spreadsheet format")
-@gr1.command("delimiter", help="Replace a delimiter with a new one, ex. replace tabs with commas")
-def delimiter_command(fin, fout, column, delimiter, new_delimiter, pseudonyms, format):
+@click.option(
+    "--pseudonyms",
+    "-p",
+    type=str,
+    default="",
+    help="Alternative column names in json format",
+)
+@click.option(
+    "--format",
+    "format_",
+    type=click.Choice(get_supported_file_formats()),
+    default="xlsx",
+    help="Generatated spreadsheet format",
+)
+@gr1.command(
+    "delimiter", help="Replace a delimiter with a new one, ex. replace tabs with commas"
+)
+def delimiter_command(fin, fout, column, delimiter, new_delimiter, pseudonyms, format_):
     pseudonyms = read_pseodonyms(pseudonyms)
     df = extract_columns_by_pseudonyms(read_file_to_df(fin), pseudonyms)
     col = []
     for _, line in df.iterrows():
         col.append(new_delimiter.join(line[column].split(delimiter)))
     df[column] = col
 
     if fout is None:
-        base = os.path.split(os.path.splitext(fin)[0])[-1]
-        fname = f'{base}_Delimiter_replaced_{column}.{format}'
+        base = Path(fin).stem
+        fname = f"{base}_Delimiter_replaced_{column}.{format_}"
     else:
         fname = fout
 
-    write(df, fout, index=False)
+    write(df, fname, index=False)
 
 
 @click.option("--fin", "-i", type=str, required=True, help="Input spreadsheet")
 @click.option("--fout", "-o", type=str, default=None, help="Generatated spreadsheet")
-@click.option("--column", "-c", type=str, required=True, help="Column to use as primary value")
+@click.option(
+    "--column", "-c", type=str, required=True, help="Column to use as primary value"
+)
 @click.option("--delimiter", "-d", type=str, required=True, help="Current delimiter")
-@click.option("--pseudonyms", "-p", type=str, default="", help="Alternative column names in json format")
-@click.option("--regex", "-r", type=str, default="(\(?\+?[0-9]*\)?)?[0-9_\- \(\)]", help="Regex expression to sort by, defaults to taking the first number")
-@click.option("--format", type=click.Choice(get_supported_file_formats()), default="xlsx", help="Generatated spreadsheet format")
+@click.option(
+    "--pseudonyms",
+    "-p",
+    type=str,
+    default="",
+    help="Alternative column names in json format",
+)
+@click.option(
+    "--regex",
+    "-r",
+    type=str,
+    default=r"(\(?\+?[0-9]*\)?)?[0-9_\- \(\)]",
+    help="Regex expression to sort by, defaults to taking the first number",
+)
+@click.option(
+    "--format",
+    "format_",
+    type=click.Choice(get_supported_file_formats()),
+    default="xlsx",
+    help="Generatated spreadsheet format",
+)
 @gr1.command("sort-column", help="")
-def sort_lines_in_column(fin, fout, column, delimiter, pseudonyms, regex, format):
-    '''Break a line by delimiter, sort by number if found otherwise by string'''
+def sort_lines_in_column(fin, fout, column, delimiter, pseudonyms, regex, format_):
+    """Break a line by delimiter, sort by number if found otherwise by string"""
     pseudonyms = read_pseodonyms(pseudonyms)
     df = extract_columns_by_pseudonyms(read_file_to_df(fin), pseudonyms)
     col = []
     regex_compiled = re.compile(regex)
     for _, line in df.iterrows():
         entries = line[column].split(delimiter)
         try:
             try:
-                sorted_list = sorted(entries, key=lambda x: int(regex_compiled.search(x).group()))
+                sorted_list = sorted(
+                    entries, key=lambda x: int(regex_compiled.search(x).group())
+                )
             except ValueError:
-                sorted_list = sorted(entries, key=lambda x: regex_compiled.search(x).group())
+                sorted_list = sorted(
+                    entries, key=lambda x: regex_compiled.search(x).group()
+                )
         except TypeError:
             sorted_list = sorted(entries)
         entry = delimiter.join(sorted_list)
         col.append(entry)
     df[column] = col
     if fout is None:
-        base = os.path.split(os.path.splitext(fin)[0])[-1]
-        fname = f'{base}_Sorted_{column}.{format}'
+        base = Path(fin).stem
+        fname = f"{base}_Sorted_{column}.{format_}"
     else:
         fname = fout
-    write(df, fout, index=False)
+    write(df, fname, index=False)
 
 
 @click.option("--fin", "-i", type=str, required=True, help="Input spreadsheet")
 @click.option("--fout", "-o", type=str, default=None, help="Generatated spreadsheet")
 @click.option("--page", type=str, required=True, help="Page name to export")
-@click.option("--format", type=click.Choice(get_supported_file_formats()), default="xlsx", help="Generatated spreadsheet format")
+@click.option(
+    "--format",
+    "format_",
+    type=click.Choice(get_supported_file_formats()),
+    default="xlsx",
+    help="Generatated spreadsheet format",
+)
 @gr1.command("export-sheet", help="Export a single sheet of a spreadsheet")
-def export_sheet(fin, fout, page, format):
-    '''Export a single sheet of a spreadsheet'''
-    path, ext = os.path.splitext(fin)
-    _, base = os.path.split(path)
+def export_sheet(fin, fout, page, format_):
+    """Export a single sheet of a spreadsheet"""
+    path = Path(fin)
+    base = path.stem
 
+    fname = fout
     if fout is None:
-        fname = f'{base}{page}.{format}'
-    else:
-        fname = fout
+        fname = f"{base}{page}.{format_}"
 
-    if ext.lower() == "csv":  # no pages for a csv
+    if path.suffix.lower() == ".csv":  # no pages for a csv
         df = read_file_to_df(fin)
     else:
-        df = pandas.read_excel(fin, sheet_name=page)
+        df = pd.read_excel(fin, sheet_name=page)
 
-    write(df, fout, index=False)
+    write(df, fname, index=False)
 
 
 def main():
     gr1()
 
 
 if __name__ == "__main__":
```

### Comparing `spreadsheet_wrangler-0.1.5/spreadsheet_wrangler/spreadsheet_wrangler.py` & `spreadsheet_wrangler-0.1.6/spreadsheet_wrangler/spreadsheet_wrangler.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,275 +1,289 @@
-'''
+"""
 spreadsheet_wrangler.py
-'''
-import pandas as pd  # type: ignore
-import csv
-import os
-import numpy as np # type: ignore
-import copy
+"""
+
 import ast
+import copy
+import csv
 import json
 import re
-#from pandas_ods_reader import read_ods
+from pathlib import Path
+
+import numpy as np  # type: ignore
+import pandas as pd  # type: ignore
+
+# from pandas_ods_reader import read_ods
 import pyexcel_ods3
-pandas = pd
 
 
 def read_pseodonyms(string: str) -> dict:
     if len(string.strip()) == 0:
         return {}
     return json.loads(string)
 
 
 def make_unique(df: pd.DataFrame, column: str, prefer_column=None):
-    '''Remove the values that are duplicates, prefer the rows with a value.
+    """Remove the values that are duplicates, prefer the rows with a value.
     column is the unique value column, prefer_column is the one to look at the longest argument of
 
     column: column to remove duplicates
     perfer_column: If there are duplicate rows then the row with the
     longest value of this value is kept
-    '''
+    """
 
     not_unique_values = [val for val in df[column] if list(df[column]).count(val) > 1]
     for value in not_unique_values:
-        print(value)
         while list(df[column]).count(value) > 1:
             drop_rows = []
             if prefer_column is None:
-                for i, row in df[df[column] == value].iterrows():
+                for i, _ in df[df[column] == value].iterrows():
                     drop_rows.append(i)
-                drop_rows.pop() # keep last row
+                drop_rows.pop()  # keep last row
             else:
-                print(value)
                 matching = df[df[column] == value][prefer_column]
                 min_length = min([str(pt) for pt in matching])
                 for i, row in df[df[column] == value].iterrows():
                     if len(str(row[prefer_column])) == min_length:
                         drop_rows.append(i)
-            df.drop(df.index[drop_rows], inplace=True)
+            df = df.drop(df.index[drop_rows])
     return df
 
 
 def extract_columns_by_pseudonyms(df: pd.DataFrame, column_names: dict) -> pd.DataFrame:
-    '''Finds knowns pseudonyms for columns and includes names them correctly for passing as argument'''
+    """Finds knowns pseudonyms for columns and includes names them correctly for passing as argument"""
     for name in df.columns:
         for column, names in column_names.items():
-            if name.lower() in [pt.lower() for pt in names] or name.lower() == column.lower():
-                df.rename(columns={name: column}, inplace=True)
+            if (
+                name.lower() in [pt.lower() for pt in names]
+                or name.lower() == column.lower()
+            ):
+                df = df.rename(columns={name: column})
     return df
 
 
 def read_csv_to_df(fname: str, **kwargs) -> pd.DataFrame:
     # Use automatic dialect detection by setting sep to None and engine to python
-    #try sniffing
+    # try sniffing
     try:
         # Use automatic dialect detection by setting sep to None and engine to python
-        kwargs["sep"]=None
-        kwargs["delimiter"]=None
-        df = pd.read_csv(fname, engine='python', **kwargs)
-        return df
-    except Exception as e:
-        print(e)
+        kwargs["sep"] = None
+        kwargs["delimiter"] = None
+        return pd.read_csv(fname, engine="python", **kwargs)
+    except Exception:
         pass
     try:
-        kwargs["sep"]=','
-        df = pd.read_csv(fname, **kwargs)
-        return df
-    except Exception as e:
-        print(e)
+        kwargs["sep"] = ","
+        return pd.read_csv(fname, **kwargs)
+    except Exception:
         pass
     try:
-        kwargs["sep"]=';'
-        df = pd.read_csv(fname, **kwargs)
-        return df
-    except Exception as e:
+        kwargs["sep"] = ";"
+        return pd.read_csv(fname, **kwargs)
+    except Exception:
         raise
 
 
-def read_ods_format_to_df(fname, **kwargs):
+def read_ods_format_to_df(fname: str, **kwargs) -> pd.DataFrame:
     data = pyexcel_ods3.get_data(fname, **kwargs)
     ave_line_length = np.mean([len(line) for line in data])
-    data_lines = []
-    for line in data:
-        if len(line) >= ave_line_length: # assume this is the data
-            data_lines.append(line)
+    data_lines = [
+        line for line in data if len(line) >= ave_line_length
+    ]  # assume this is the data
     header = data_lines[0]
     data_lines = data_lines[1:]
-    df_dict = dict([(column, []) for column in header])
+    df_dict = {column: [] for column in header}
     for line in data_lines:
-        for column, pt in zip(df_dict.keys(), line):
+        for column, pt in zip(df_dict.keys(), line, strict=False):
             df_dict[column].append(pt)
-    df = pd.DataFrame(df_dict)
-    return df
+    return pd.DataFrame(df_dict)
 
 
 def get_supported_file_types_df():
-    '''
+    """
     Installed readers
-    '''
+    """
     return [
-        {'title': 'text',
-         'kwargs': dict(
-                header=0, skipinitialspace=True,
-                index_col=None, comment="#", quotechar='"',
-                quoting=csv.QUOTE_MINIMAL, engine="python",
-                skip_blank_lines=True
-            ),
-         'extensions': ('csv', 'txt'),
-         'writedf': pandas.DataFrame.to_csv,
-         'readf': read_csv_to_df},
-        {'title': 'excel',
-         'kwargs': dict(sheet_name=0, header=0, skiprows=0),
-         'extensions': ("xls", "xlsx", "xlsm","xlsb"),
-         'writedf': pandas.DataFrame.to_excel,
-         'readf': pd.read_excel},
-        {'title': 'ods',
-         'kwargs': dict(sheet_name=0, header=0, skiprows=0),
-         'extensions': ("ods", "odt", "odf"),
-         'writedf': None,
-         'readf': read_ods_format_to_df}
+        {
+            "title": "text",
+            "kwargs": {
+                "header": 0,
+                "skipinitialspace": True,
+                "index_col": None,
+                "comment": "#",
+                "quotechar": '"',
+                "quoting": csv.QUOTE_MINIMAL,
+                "engine": "python",
+                "skip_blank_lines": True,
+            },
+            "extensions": ("csv", "txt"),
+            "writedf": pd.DataFrame.to_csv,
+            "readf": read_csv_to_df,
+        },
+        {
+            "title": "excel",
+            "kwargs": {"sheet_name": 0, "header": 0, "skiprows": 0},
+            "extensions": ("xls", "xlsx", "xlsm", "xlsb"),
+            "writedf": pd.DataFrame.to_excel,
+            "readf": pd.read_excel,
+        },
+        {
+            "title": "ods",
+            "kwargs": {"sheet_name": 0, "header": 0, "skiprows": 0},
+            "extensions": ("ods", "odt", "odf"),
+            "writedf": None,
+            "readf": read_ods_format_to_df,
+        },
     ]
 
 
-def get_supported_file_formats():
-    '''
+def get_supported_file_formats() -> tuple[str]:
+    """
     returns collection of all the supported extensions
-    '''
+    """
     extensions = []
     for entry in get_supported_file_types_df():
         extensions.extend(entry["extensions"])
     return tuple(extensions)
 
 
-def write(df: pandas.DataFrame, fname: str, **kwargs) -> None:
-    base, ext = os.path.splitext(fname)
+def write(df: pd.DataFrame, fname: str, **kwargs) -> None:
+    ext = Path(fname).suffix.strip(".").lower()
     types = get_supported_file_types_df()
     writer = None
     for value in types:
-        if ext.strip('.').lower() in value["extensions"]:
+        if ext in value["extensions"]:
             writer = value["writedf"]
+            break
 
+    assert writer
     writer(df, fname, **kwargs)
 
 
 def read_file_to_df(fname: str, **kwargs) -> pd.DataFrame:
-    '''
+    """
     Cycle through extensions, use the reader object to call
-    '''
-    name, ext = os.path.splitext(fname)
-    ext = ext.strip('.')
-    ext = ext.lower()
+    """
+    ext = Path(fname).suffix.strip(".").lower()
     df = None
     found = False
     for reader in get_supported_file_types_df():
         if ext in reader["extensions"]:
             found = True
             if kwargs is None:
                 kwargs = reader["kwargs"]
             df = reader["readf"](fname, **kwargs)
             break
     if not found:
-        raise UserWarning(f"Extension {ext} unsupported")
+        msg = f"Extension {ext} unsupported"
+        raise UserWarning(msg)
     return pd.DataFrame(df)
 
 
 def uncluster_ast(df: pd.DataFrame, grouped_column: str) -> pd.DataFrame:
     formated_df = df[df[grouped_column] != np.nan]
     expanded_rows = []
     for _, row in formated_df.iterrows():
         group = ast.literal_eval(row[grouped_column])
         for item in group:
             row[grouped_column] = item
             expanded_rows.append(copy.deepcopy(row))
-    expanded_df = pd.DataFrame(expanded_rows)
-    return expanded_df
+    return pd.DataFrame(expanded_rows)
 
 
-def uncluster_regex(df: pd.DataFrame, grouped_column: str, expression: str = "[A-z]+[0-9]+") -> pd.DataFrame:
+def uncluster_regex(
+    df: pd.DataFrame, grouped_column: str, expression: str = "[A-z]+[0-9]+"
+) -> pd.DataFrame:
     formated_df = df[df[grouped_column] != np.nan]
     expanded_rows = []
     ref_regex = re.compile(expression)
     for _, row in formated_df.iterrows():
         refs = row[grouped_column]
-        if type(refs) != str:
+        if not isinstance(refs, str):
             continue
         for ref in ref_regex.findall(refs):
             row[grouped_column] = ref
             expanded_rows.append(copy.deepcopy(row))
-    expanded_df = pd.DataFrame(expanded_rows)
-    return expanded_df
+    return pd.DataFrame(expanded_rows)
 
 
 def uncluster(df: pd.DataFrame, grouped_column: str) -> pd.DataFrame:
     return uncluster_regex(df, grouped_column)
 
 
 def cluster(df: pd.DataFrame, on: list, column: str) -> pd.DataFrame:
-    '''ref-des will not be a tuple of all the matching lines, the rest of the line is taken to be the first in the file and carried forward'''
+    """ref-des will not be a tuple of all the matching lines, the rest of the line is taken to be the first in the file and carried forward"""
     for pt in on:
         if pt not in df.columns:
-            raise KeyError(f"column {pt} or pseudonym not found")
+            msg = f"column {pt} or pseudonym not found"
+            raise KeyError(msg)
     if column not in df.columns:
-        raise KeyError(f"column {column} or pseudonym not found")
+        msg = f"column {column} or pseudonym not found"
+        raise KeyError(msg)
 
-    grouped = df.groupby(by=list(on))  #  IMPORTANT: This has to be a list as a tuple is interpreted as a single key.
-    drop : list = []
-    clustered : list = []
-    rows : list = []
+    grouped = df.groupby(
+        by=list(on)
+    )  #  IMPORTANT: This has to be a list as a tuple is interpreted as a single key.
+    clustered: list = []
+    rows: list = []
 
     for _, group in grouped:
         cluster_entries = []
-        for i, row in group.iterrows():
+        for _i, row in group.iterrows():
             cluster_entries.append(row[column])
         copy_row = copy.deepcopy(row)
         rows.append(copy_row)
         clustered.append(tuple(cluster_entries))
 
     df = pd.DataFrame(rows)
     index = df.columns.get_indexer_for([column])[0]
-    df.drop(columns=[column], inplace=True)
+    df = df.drop(columns=[column])
     df.insert(int(index), column=column, value=clustered)
     return df
 
 
 def compare(left: pd.DataFrame, right: pd.DataFrame, columns: str, on: str) -> dict:
     errors: dict = {"line": [], "column": [], "description": []}
     for pt in list(left[on]) + list(right[on]):
         matching_rows_left = left[left[on] == pt]
         matching_rows_right = right[right[on] == pt]
         for column in columns:
-            for lc, rc in zip(matching_rows_left[column], matching_rows_right[column]):
+            for lc, rc in zip(
+                matching_rows_left[column], matching_rows_right[column], strict=False
+            ):
                 if lc != rc:
                     # filter out nan
                     if lc is np.nan and rc is np.nan:
                         continue
                     errors["line"].append(pt)
                     errors["column"].append(column)
-                    errors["description"].append("{} ({}) != {} ({})".format(lc, type(lc), rc, type(rc)))
+                    errors["description"].append(
+                        f"{lc} ({type(lc)}) != {rc} ({type(rc)})"
+                    )
     return errors
 
 
 def select_on_value(df: pd.DataFrame, value, column: str, blank_defaults: bool):
-    '''
+    """
     Selects all rows that match the value in the given column
-    '''
-    match = [str(pt).lower()==str(value).lower() for pt in df[column]]
+    """
+    match = [str(pt).lower() == str(value).lower() for pt in df[column]]
     if blank_defaults:
         filtered_df = df.loc[(match) | (df[column].isnull())]
     else:
         filtered_df = df.loc[(match)]
     return filtered_df
 
 
-def get_unique(df: pd.DataFrame, column: str, blank_defaults: bool) -> pd.DataFrame:
-    '''
-    Selects only unique lines matching the column, value
-    '''
-    return make_unique(filtered_df, column=column, prefer_column=on)
+# def get_unique(df: pd.DataFrame, column: str, blank_defaults: bool) -> pd.DataFrame:
+#    """
+#    Selects only unique lines matching the column, value
+#    """
+#    return make_unique(df, column=column, prefer_column=on)
 
 
-def filter_df(df: pd.DataFrame, on: str, value, column: str, blank_defaults: bool) -> pd.DataFrame:
-    '''
+def filter_df(
+    df: pd.DataFrame, on: str, value, column: str, blank_defaults: bool
+) -> pd.DataFrame:
+    """
     Returns the rows that both match
-    '''
-    pass
-
+    """
```

### Comparing `spreadsheet_wrangler-0.1.5/spreadsheet_wrangler.egg-info/PKG-INFO` & `spreadsheet_wrangler-0.1.6/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,46 @@
 Metadata-Version: 2.1
-Name: spreadsheet-wrangler
-Version: 0.1.5
-Summary: Spreadsheet editing tools
-Home-page: https://github.com/snhobbs/spreadsheet-wrangler
-Author: Simon Hobbs
-Author-email: simon.hobbs@electrooptical.net
-License: MIT license
-Keywords: spreadsheet_wrangler
-Platform: UNKNOWN
+Name: spreadsheet_wrangler
+Version: 0.1.6
+Summary: Place components in a kicad file programmatically.
+Author-email: Simon Hobbs <simon.hobbs@electrooptical.net>
+License: MIT License
+        
+        Copyright (c) 2023, Simon Hobbs
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: github, https://github.com/snhobbs/spreadsheet-wrangler.git
+Keywords: spreadsheet_wrangler,kicad,python,eda,electronics,pcb,manufacturing
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.6
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: click>=7.0.0
+Requires-Dist: pandas>=2.0.0
+Requires-Dist: pyexcel-ods3>=0.6.0
 
 # spreadsheet-wrangler
 Command line tool for interacting with spreadsheet data
 
 ## Installation
 ### pypi
 ```
@@ -58,15 +76,15 @@
 
 ### Compare the data in two BOMS
 To compare the available data of two BOMs to compare function of spreadsheet_wrangler should be used. If a BOM was exported
 and needs to be checked against another with questionable history run:
 ```
 spreadsheet_wrangler.py compare --on="ref-des" -l bom.xlsx -r bom_Merged_data_store_On_pn.xlsx
 ```
-This will compare the original BOM with the merged one from the first example. Comparisons are done column by column with rows matched by the value in the column passed with the argument "--on". This should be a unique for each instance of a part (i.e a ref des). 
+This will compare the original BOM with the merged one from the first example. Comparisons are done column by column with rows matched by the value in the column passed with the argument "--on". This should be a unique for each instance of a part (i.e a ref des).
 The shared columns will be checked as well as any passed in with the --columns argument. Discrepancies are printed to screen.
 
 ### Generate a BOM sorted by the type of parts
 BOMs used for ordering, shipping, budgeting, or shipping to a CM are typically ordered by the type of part.
 
 The ordering BOM sorts by reference designator and combines the BOM into unique part types. This can then be used for ordering or quoting. This can be passed to a tool like kicost or used with supplier BOM Managers or the Octopart BOM Manager (recommended).
 
@@ -82,31 +100,19 @@
 spreadsheet_wrangler.py uncluster --column="ref-des" -s bom_unclustered.xlsx
 ```
 This will separate the lines like the original bom.xlsx. This BOM can now be compared using the compare function described above.
 
 NOTE: Note the data in each grouped row is duplicated for each clustered element. This is not necessarily correct if data was dissimilar and lost during the clustering step.
 
 ### Clustering a partially filled in BOM
-After exporting a design BOM with each component in it's own line you end up with what I call a design BOM except without the useful fields included. 
+After exporting a design BOM with each component in it's own line you end up with what I call a design BOM except without the useful fields included.
 
 ![unclustered BOM](unclustered_bom.png)
 
 For this I want to cluster based on "Comment" and "Footprint", that is I want all 0603 10K resistors together and not include any other 0603 or 10K parts in the cluster. The command would then be:
 
 ```
 spreadsheet_wrangler.py cluster --spreadsheet BOM-1x2_tester.csv --column "Designator" --on "Comment" --on "Footprint" -o BOM_clustered.xlsx
 ```
 This call turns the above BOM into:
 
 ![clustered on comment and footprint](clustered_on_comment_and_footprint.png)
-
-
-=======
-History
-=======
-
-0.1.4 (2023-10-28)
-------------------
-
-* First release on PyPI.
-
-
```

### Comparing `spreadsheet_wrangler-0.1.5/spreadsheet_wrangler.egg-info/SOURCES.txt` & `spreadsheet_wrangler-0.1.6/spreadsheet_wrangler.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,42 @@
+.gitignore
+.pre-commit-config.yaml
 CONTRIBUTING.rst
 HISTORY.rst
 LICENSE
 MANIFEST.in
+Makefile
 README.md
+clustered_on_comment_and_footprint.png
+pyproject.toml
+requirements.txt
+requirements_dev.txt
 setup.cfg
 setup.py
+tox.ini
+unclustered_bom.png
 docs/Makefile
 docs/conf.py
 docs/contributing.rst
 docs/history.rst
 docs/index.rst
 docs/installation.rst
 docs/make.bat
+docs/modules.rst
 docs/readme.rst
+docs/spreadsheet_wrangler.rst
 docs/usage.rst
+spreadsheet_wrangler/.editorconfig
+spreadsheet_wrangler/.gitignore
+spreadsheet_wrangler/.travis.yml
 spreadsheet_wrangler/__init__.py
 spreadsheet_wrangler/cli.py
 spreadsheet_wrangler/spreadsheet_wrangler.py
 spreadsheet_wrangler.egg-info/PKG-INFO
 spreadsheet_wrangler.egg-info/SOURCES.txt
 spreadsheet_wrangler.egg-info/dependency_links.txt
 spreadsheet_wrangler.egg-info/entry_points.txt
-spreadsheet_wrangler.egg-info/not-zip-safe
 spreadsheet_wrangler.egg-info/requires.txt
 spreadsheet_wrangler.egg-info/top_level.txt
+spreadsheet_wrangler/.github/ISSUE_TEMPLATE.md
 tests/__init__.py
 tests/test_spreadsheet_wrangler.py
```

