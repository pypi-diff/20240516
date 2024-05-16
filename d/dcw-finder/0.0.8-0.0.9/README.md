# Comparing `tmp/dcw-finder-0.0.8.tar.gz` & `tmp/dcw-finder-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcw-finder-0.0.8.tar", last modified: Mon May 13 18:23:14 2024, max compression
+gzip compressed data, was "dcw-finder-0.0.9.tar", last modified: Mon May 13 18:27:42 2024, max compression
```

## Comparing `dcw-finder-0.0.8.tar` & `dcw-finder-0.0.9.tar`

### file list

```diff
@@ -1,26 +1,25 @@
-drwxr-xr-x   0 jrim       (501) staff       (20)        0 2024-05-13 18:23:14.968813 dcw-finder-0.0.8/
--rw-r--r--   0 jrim       (501) staff       (20)      448 2024-05-13 18:23:14.968577 dcw-finder-0.0.8/PKG-INFO
-drwxr-xr-x   0 jrim       (501) staff       (20)        0 2024-05-13 18:23:14.968314 dcw-finder-0.0.8/dcw_finder.egg-info/
--rw-r--r--   0 jrim       (501) staff       (20)      448 2024-05-13 18:23:14.000000 dcw-finder-0.0.8/dcw_finder.egg-info/PKG-INFO
--rw-r--r--   0 jrim       (501) staff       (20)      420 2024-05-13 18:23:14.000000 dcw-finder-0.0.8/dcw_finder.egg-info/SOURCES.txt
--rw-r--r--   0 jrim       (501) staff       (20)        1 2024-05-13 18:23:14.000000 dcw-finder-0.0.8/dcw_finder.egg-info/dependency_links.txt
--rw-r--r--   0 jrim       (501) staff       (20)        1 2024-05-13 17:52:51.000000 dcw-finder-0.0.8/dcw_finder.egg-info/not-zip-safe
--rw-r--r--   0 jrim       (501) staff       (20)        7 2024-05-13 18:23:14.000000 dcw-finder-0.0.8/dcw_finder.egg-info/requires.txt
--rw-r--r--   0 jrim       (501) staff       (20)        4 2024-05-13 18:23:14.000000 dcw-finder-0.0.8/dcw_finder.egg-info/top_level.txt
--rw-r--r--   0 jrim       (501) staff       (20)       38 2024-05-13 18:23:14.968873 dcw-finder-0.0.8/setup.cfg
--rw-r--r--   0 jrim       (501) staff       (20)      650 2024-05-13 18:23:12.000000 dcw-finder-0.0.8/setup.py
-drwxr-xr-x   0 jrim       (501) staff       (20)        0 2024-05-13 18:23:14.968097 dcw-finder-0.0.8/src/
--rw-r--r--   0 jrim       (501) staff       (20)      301 2024-05-13 18:23:08.000000 dcw-finder-0.0.8/src/__init__.py
--rw-r--r--   0 jrim       (501) staff       (20)     7747 2024-05-13 18:17:38.000000 dcw-finder-0.0.8/src/_accessory.py
--rw-r--r--   0 jrim       (501) staff       (20)     7167 2024-05-13 17:40:31.000000 dcw-finder-0.0.8/src/_blast.py
--rw-r--r--   0 jrim       (501) staff       (20)    11475 2024-05-13 18:17:38.000000 dcw-finder-0.0.8/src/_cluster.py
--rw-r--r--   0 jrim       (501) staff       (20)    10160 2024-05-13 18:20:34.000000 dcw-finder-0.0.8/src/_count.py
--rw-r--r--   0 jrim       (501) staff       (20)    16245 2024-05-13 18:19:55.000000 dcw-finder-0.0.8/src/_info.py
--rw-r--r--   0 jrim       (501) staff       (20)     7793 2024-05-13 18:20:55.000000 dcw-finder-0.0.8/src/_parse.py
--rw-r--r--   0 jrim       (501) staff       (20)     2668 2024-05-13 18:17:38.000000 dcw-finder-0.0.8/src/_profile.py
--rw-r--r--   0 jrim       (501) staff       (20)     4207 2024-05-13 17:40:31.000000 dcw-finder-0.0.8/src/_search.py
--rw-r--r--   0 jrim       (501) staff       (20)     4184 2024-05-13 18:17:38.000000 dcw-finder-0.0.8/src/_seqlib.py
--rw-r--r--   0 jrim       (501) staff       (20)     4337 2024-05-13 17:40:31.000000 dcw-finder-0.0.8/src/_target.py
--rw-r--r--   0 jrim       (501) staff       (20)     5582 2024-05-13 17:40:31.000000 dcw-finder-0.0.8/src/_utils.py
--rw-r--r--   0 jrim       (501) staff       (20)     6584 2024-05-13 18:22:56.000000 dcw-finder-0.0.8/src/_visualize.py
--rw-r--r--   0 jrim       (501) staff       (20)     1984 2024-05-13 18:17:38.000000 dcw-finder-0.0.8/src/main.py
+drwxr-xr-x   0 jrim       (501) staff       (20)        0 2024-05-13 18:27:42.979098 dcw-finder-0.0.9/
+-rw-r--r--   0 jrim       (501) staff       (20)      448 2024-05-13 18:27:42.978882 dcw-finder-0.0.9/PKG-INFO
+drwxr-xr-x   0 jrim       (501) staff       (20)        0 2024-05-13 18:27:42.978638 dcw-finder-0.0.9/dcw_finder.egg-info/
+-rw-r--r--   0 jrim       (501) staff       (20)      448 2024-05-13 18:27:42.000000 dcw-finder-0.0.9/dcw_finder.egg-info/PKG-INFO
+-rw-r--r--   0 jrim       (501) staff       (20)      407 2024-05-13 18:27:42.000000 dcw-finder-0.0.9/dcw_finder.egg-info/SOURCES.txt
+-rw-r--r--   0 jrim       (501) staff       (20)        1 2024-05-13 18:27:42.000000 dcw-finder-0.0.9/dcw_finder.egg-info/dependency_links.txt
+-rw-r--r--   0 jrim       (501) staff       (20)        1 2024-05-13 18:27:42.000000 dcw-finder-0.0.9/dcw_finder.egg-info/not-zip-safe
+-rw-r--r--   0 jrim       (501) staff       (20)        7 2024-05-13 18:27:42.000000 dcw-finder-0.0.9/dcw_finder.egg-info/requires.txt
+-rw-r--r--   0 jrim       (501) staff       (20)        4 2024-05-13 18:27:42.000000 dcw-finder-0.0.9/dcw_finder.egg-info/top_level.txt
+-rw-r--r--   0 jrim       (501) staff       (20)       38 2024-05-13 18:27:42.979164 dcw-finder-0.0.9/setup.cfg
+-rw-r--r--   0 jrim       (501) staff       (20)      650 2024-05-13 18:27:37.000000 dcw-finder-0.0.9/setup.py
+drwxr-xr-x   0 jrim       (501) staff       (20)        0 2024-05-13 18:27:42.978431 dcw-finder-0.0.9/src/
+-rw-r--r--   0 jrim       (501) staff       (20)      280 2024-05-13 18:27:32.000000 dcw-finder-0.0.9/src/__init__.py
+-rw-r--r--   0 jrim       (501) staff       (20)     7747 2024-05-13 18:17:38.000000 dcw-finder-0.0.9/src/_accessory.py
+-rw-r--r--   0 jrim       (501) staff       (20)     7167 2024-05-13 17:40:31.000000 dcw-finder-0.0.9/src/_blast.py
+-rw-r--r--   0 jrim       (501) staff       (20)    11475 2024-05-13 18:17:38.000000 dcw-finder-0.0.9/src/_cluster.py
+-rw-r--r--   0 jrim       (501) staff       (20)    10060 2024-05-13 18:26:56.000000 dcw-finder-0.0.9/src/_count.py
+-rw-r--r--   0 jrim       (501) staff       (20)     8060 2024-05-13 18:25:20.000000 dcw-finder-0.0.9/src/_parse.py
+-rw-r--r--   0 jrim       (501) staff       (20)     2668 2024-05-13 18:17:38.000000 dcw-finder-0.0.9/src/_profile.py
+-rw-r--r--   0 jrim       (501) staff       (20)     4207 2024-05-13 17:40:31.000000 dcw-finder-0.0.9/src/_search.py
+-rw-r--r--   0 jrim       (501) staff       (20)     4184 2024-05-13 18:17:38.000000 dcw-finder-0.0.9/src/_seqlib.py
+-rw-r--r--   0 jrim       (501) staff       (20)     4337 2024-05-13 17:40:31.000000 dcw-finder-0.0.9/src/_target.py
+-rw-r--r--   0 jrim       (501) staff       (20)     5582 2024-05-13 17:40:31.000000 dcw-finder-0.0.9/src/_utils.py
+-rw-r--r--   0 jrim       (501) staff       (20)     7008 2024-05-13 18:27:10.000000 dcw-finder-0.0.9/src/_visualize.py
+-rw-r--r--   0 jrim       (501) staff       (20)     1984 2024-05-13 18:17:38.000000 dcw-finder-0.0.9/src/main.py
```

### Comparing `dcw-finder-0.0.8/setup.py` & `dcw-finder-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='dcw-finder',
-    version='0.0.8',
+    version='0.0.9',
     description='Package for detecting dcw gene cluster',
     author='jsrim',
     author_email='comfortindex@naver.com',
     url='https://github.com/jrim42/gene-cluster',
     install_requires=['pandas'],
     packages=find_packages(exclude=[]),
     keywords=[],
```

### Comparing `dcw-finder-0.0.8/src/_accessory.py` & `dcw-finder-0.0.9/src/_accessory.py`

 * *Files identical despite different names*

### Comparing `dcw-finder-0.0.8/src/_blast.py` & `dcw-finder-0.0.9/src/_blast.py`

 * *Files identical despite different names*

### Comparing `dcw-finder-0.0.8/src/_cluster.py` & `dcw-finder-0.0.9/src/_cluster.py`

 * *Files identical despite different names*

### Comparing `dcw-finder-0.0.8/src/_count.py` & `dcw-finder-0.0.9/src/_count.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,16 +8,18 @@
 '''
 
 import os
 import pandas as pd
 import sys
 import time
 
-sys.path.append('./info/')
-from _info import target_list
+target_names = [
+  "MraZ", "MraW", "FtsL", "FtsI", "MurE", "MurF", "MraY", "MurD", "FtsW", 
+  "MurG", "MurC", "MurB", "MurA", "DdlB", "FtsQ", "FtsA", "FtsZ"
+]
 
 from ._visualize import visualize_heatmap
 from ._visualize import visualize_freq
 
 #===============================================================================
 def count_blastp_result(project_info):
     output_dir = project_info['output']
@@ -89,18 +91,14 @@
     output_dir = project_info['output']
 
     all_directories = [d for d in os.listdir(input_dir) if os.path.isdir(os.path.join(input_dir, d))]
     all_directories = [d for d in all_directories if d != 'output' and not d.startswith('output/')]
 
     start_time = time.time()
 
-    target_names = []
-    for target in target_list:
-        target_names.append(target['protein'])
-
     target_cnt_list_1 = []
     for genus in all_directories:
         genus_df_list = []
         for accession in os.listdir(os.path.join(input_dir, genus)):
             if not "GC" in accession:
                 continue
             file_path = f"{input_dir}/{genus}/{accession}/target_seq.tsv"
@@ -206,18 +204,14 @@
     seq_lib['Prediction'] = seq_lib['Prediction'] + '-' + seq_lib['no'].astype(str)
     seq_lib.drop(['no', 'Total'], axis=1, inplace=True)
 
     genus_rep = seq_lib.copy()
 
     start_time = time.time()
 
-    target_names = []
-    for target in target_list:
-        target_names.append(target['protein'])
-
     for genus in all_directories:
         for accession in os.listdir(os.path.join(input_dir, genus)):
             if not "GC" in accession:
                 continue
             file_path = f"{input_dir}/{genus}/{accession}/target_seq.tsv"
         
             data_df = pd.read_csv(file_path, sep='\t', comment='#')
```

### Comparing `dcw-finder-0.0.8/src/_parse.py` & `dcw-finder-0.0.9/src/_parse.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,24 +5,38 @@
     └── merge_gbff_gff  ˑˑˑˑˑˑ  to merge parsed genome data (gbff + gff).
 
 '''
  
 import os
 import time
 
-import sys
-sys.path.append("./info/")
-from _info import gbff_key_setting
-
 import pandas as pd
 pd.set_option('display.max_rows', None)
 pd.set_option('display.max_columns', None)
 pd.set_option('display.expand_frame_repr', False)
 pd.set_option('display.max_colwidth', None)
 
+gbff_key_setting = {
+  "gene": True,
+  "locus_tag": False,
+  "EC_number": True,
+  "inference": False,
+  "GO_function": False,
+  "GO_process": False,
+  "note": False,
+  "codon_start": False,
+  "transl_table": False,
+  "product": True,
+  "protein_id": True,
+  "translation": True,
+  "position": False,
+  "db_xref": False,
+  "pseudo": False
+}
+
 #===== parse_genome =================================================================
 def parse_genome(base_info):
     print("<< parsing genome data...")
     base_dir_path = base_info['input']
     base_dir_len = base_info['input_len']
     all_directories = [d for d in os.listdir(base_dir_path) if os.path.isdir(os.path.join(base_dir_path, d))]
     all_directories = [d for d in all_directories if d != 'output' and not d.startswith('output/')]
```

### Comparing `dcw-finder-0.0.8/src/_profile.py` & `dcw-finder-0.0.9/src/_profile.py`

 * *Files identical despite different names*

### Comparing `dcw-finder-0.0.8/src/_search.py` & `dcw-finder-0.0.9/src/_search.py`

 * *Files identical despite different names*

### Comparing `dcw-finder-0.0.8/src/_seqlib.py` & `dcw-finder-0.0.9/src/_seqlib.py`

 * *Files identical despite different names*

### Comparing `dcw-finder-0.0.8/src/_target.py` & `dcw-finder-0.0.9/src/_target.py`

 * *Files identical despite different names*

### Comparing `dcw-finder-0.0.8/src/_utils.py` & `dcw-finder-0.0.9/src/_utils.py`

 * *Files identical despite different names*

### Comparing `dcw-finder-0.0.8/src/_visualize.py` & `dcw-finder-0.0.9/src/_visualize.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,35 @@
 import pandas as pd
 import numpy as np
 import matplotlib.pyplot as plt
 import matplotlib.patches as mpatches
 from matplotlib.font_manager import FontProperties
 from matplotlib.colors import LinearSegmentedColormap
 
-from _info import target_color
+target_color = {
+    "MraZ": "#8ED3C7",
+    "MraW": "#F99FB5",
+    "FtsL": "#2A9D8F",
+    "FtsI": "#BEBADB",
+    "MurE": "#FB7F72",
+    "MurF": "#81B1D3",
+    "MraY": "#FDB364",
+    "MurD": "#B2DE68",
+    "FtsW": "#E4B7CD",
+    "MurG": "#B6C8FE",
+    "MurC": "#BD7FBB",
+    "MurB": "#CDEBC3",
+    "MurA": "#DFC27C",
+    "DdlB": "#C7E8FA",
+    "FtsQ": "#A95C68",
+    "FtsA": "#FCBBA2",
+    "FtsZ": "#F7DA84",
+    "blank": "#F0F0F0",
+    "etc": "#C0C0C0"
+}
 
 #------------------------------------------------------------
 def visualize_cluster_type(output_dir, df):
   x = np.arange(len(df))
   width = 0.3
 
   fig, ax = plt.subplots(figsize=(42, 6))
```

### Comparing `dcw-finder-0.0.8/src/main.py` & `dcw-finder-0.0.9/src/main.py`

 * *Files identical despite different names*

