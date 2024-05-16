# Comparing `tmp/nwb4fp-0.6.3.1.tar.gz` & `tmp/nwb4fp-0.6.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nwb4fp-0.6.3.1.tar", last modified: Mon May 13 15:01:37 2024, max compression
+gzip compressed data, was "nwb4fp-0.6.3.2.tar", last modified: Thu May 16 11:12:39 2024, max compression
```

## Comparing `nwb4fp-0.6.3.1.tar` & `nwb4fp-0.6.3.2.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 15:01:37.407803 nwb4fp-0.6.3.1/
--rw-rw-rw-   0        0        0     1089 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.1/LICENSE
--rw-rw-rw-   0        0        0     5732 2024-05-13 15:01:37.378800 nwb4fp-0.6.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     6901 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.1/README.md
--rw-rw-rw-   0        0        0       42 2024-05-13 15:01:37.409801 nwb4fp-0.6.3.1/setup.cfg
--rw-rw-rw-   0        0        0      886 2024-05-13 14:58:50.000000 nwb4fp-0.6.3.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-13 15:01:36.712802 nwb4fp-0.6.3.1/src/
-drwxrwxrwx   0        0        0        0 2024-05-13 15:01:36.728802 nwb4fp-0.6.3.1/src/nwb4fp/
-drwxrwxrwx   0        0        0        0 2024-05-13 15:01:36.870807 nwb4fp-0.6.3.1/src/nwb4fp/main/
--rw-rw-rw-   0        0        0        0 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.1/src/nwb4fp/main/__init__.py
--rw-rw-rw-   0        0        0     3593 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.1/src/nwb4fp/main/main_create_nwb.py
-drwxrwxrwx   0        0        0        0 2024-05-13 15:01:37.033805 nwb4fp-0.6.3.1/src/nwb4fp/postprocess/
--rw-rw-rw-   0        0        0    15551 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.1/src/nwb4fp/postprocess/Get_positions.py
--rw-rw-rw-   0        0        0        0 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.1/src/nwb4fp/postprocess/__init__.py
--rw-rw-rw-   0        0        0     1850 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.1/src/nwb4fp/postprocess/add_wfcor.py
--rw-rw-rw-   0        0        0      470 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.1/src/nwb4fp/postprocess/dlc_kinematic.py
--rw-rw-rw-   0        0        0     2485 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.1/src/nwb4fp/postprocess/extract_wf.py
--rw-rw-rw-   0        0        0     1343 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.1/src/nwb4fp/postprocess/get_potential_merge.py
--rw-rw-rw-   0        0        0        0 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.1/src/nwb4fp/postprocess/lfp_channel.py
--rw-rw-rw-   0        0        0    17084 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.1/src/nwb4fp/postprocess/nwbPHYnOPHYS.py
--rw-rw-rw-   0        0        0    14469 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.1/src/nwb4fp/postprocess/quality_metrix.py
-drwxrwxrwx   0        0        0        0 2024-05-13 15:01:36.723804 nwb4fp-0.6.3.1/src/nwb4fp/preprocess/
--rw-rw-rw-   0        0        0        0 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.1/src/nwb4fp/preprocess/__init__.py
--rw-rw-rw-   0        0        0      459 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.1/src/nwb4fp/preprocess/copy_file.py
--rw-rw-rw-   0        0        0      620 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.1/src/nwb4fp/preprocess/down_sample.py
--rw-rw-rw-   0        0        0     8249 2024-05-13 14:58:38.000000 nwb4fp-0.6.3.1/src/nwb4fp/preprocess/down_sample_lfp.py
--rw-rw-rw-   0        0        0     3712 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.1/src/nwb4fp/preprocess/extract_lfp.py
--rw-rw-rw-   0        0        0      148 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.1/src/nwb4fp/preprocess/get_path.py
--rw-rw-rw-   0        0        0     1203 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.1/src/nwb4fp/preprocess/load_data.py
--rw-rw-rw-   0        0        0      244 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.1/src/nwb4fp/preprocess/run_phy.py
-drwxrwxrwx   0        0        0        0 2024-05-13 15:01:36.730803 nwb4fp-0.6.3.1/src/nwb4fp/test/
-drwxrwxrwx   0        0        0        0 2024-05-13 15:01:37.328801 nwb4fp-0.6.3.1/src/nwb4fp/test/run_scripts/
--rw-rw-rw-   0        0        0     1525 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.1/src/nwb4fp/test/run_scripts/readnwb.py
--rw-rw-rw-   0        0        0     1028 2024-05-13 13:05:19.000000 nwb4fp-0.6.3.1/src/nwb4fp/test/run_scripts/readnwb_0283.py
--rw-rw-rw-   0        0        0     1054 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.1/src/nwb4fp/test/run_scripts/readnwb_09PC.py
--rw-rw-rw-   0        0        0     1448 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.1/src/nwb4fp/test/run_scripts/readnwb_09PD.py
--rw-rw-rw-   0        0        0        0 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.1/src/nwb4fp/test/run_scripts/test.py
--rw-rw-rw-   0        0        0     5828 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.1/src/nwb4fp/test/run_scripts/test_lfp.py
-drwxrwxrwx   0        0        0        0 2024-05-13 15:01:36.841806 nwb4fp-0.6.3.1/src/nwb4fp.egg-info/
--rw-rw-rw-   0        0        0     5732 2024-05-13 15:01:36.000000 nwb4fp-0.6.3.1/src/nwb4fp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1143 2024-05-13 15:01:36.000000 nwb4fp-0.6.3.1/src/nwb4fp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 15:01:36.000000 nwb4fp-0.6.3.1/src/nwb4fp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     2885 2024-05-13 15:01:36.000000 nwb4fp-0.6.3.1/src/nwb4fp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-13 15:01:36.000000 nwb4fp-0.6.3.1/src/nwb4fp.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-16 11:12:39.333885 nwb4fp-0.6.3.2/
+-rw-rw-rw-   0        0        0     1089 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.2/LICENSE
+-rw-rw-rw-   0        0        0     5732 2024-05-16 11:12:39.325874 nwb4fp-0.6.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0     6901 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-16 11:12:39.353879 nwb4fp-0.6.3.2/setup.cfg
+-rw-rw-rw-   0        0        0      888 2024-05-16 11:12:25.000000 nwb4fp-0.6.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 11:12:38.885922 nwb4fp-0.6.3.2/src/
+drwxrwxrwx   0        0        0        0 2024-05-16 11:12:38.902888 nwb4fp-0.6.3.2/src/nwb4fp/
+drwxrwxrwx   0        0        0        0 2024-05-16 11:12:38.893896 nwb4fp-0.6.3.2/src/nwb4fp/main/
+-rw-rw-rw-   0        0        0        0 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.2/src/nwb4fp/main/__init__.py
+-rw-rw-rw-   0        0        0     3799 2024-05-16 11:11:30.000000 nwb4fp-0.6.3.2/src/nwb4fp/main/main_create_nwb.py
+drwxrwxrwx   0        0        0        0 2024-05-16 11:12:38.897961 nwb4fp-0.6.3.2/src/nwb4fp/postprocess/
+-rw-rw-rw-   0        0        0    15551 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.2/src/nwb4fp/postprocess/Get_positions.py
+-rw-rw-rw-   0        0        0        0 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.2/src/nwb4fp/postprocess/__init__.py
+-rw-rw-rw-   0        0        0     1845 2024-05-16 11:04:28.000000 nwb4fp-0.6.3.2/src/nwb4fp/postprocess/add_wfcor.py
+-rw-rw-rw-   0        0        0      470 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.2/src/nwb4fp/postprocess/dlc_kinematic.py
+-rw-rw-rw-   0        0        0     2485 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.2/src/nwb4fp/postprocess/extract_wf.py
+-rw-rw-rw-   0        0        0     1343 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.2/src/nwb4fp/postprocess/get_potential_merge.py
+-rw-rw-rw-   0        0        0        0 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.2/src/nwb4fp/postprocess/lfp_channel.py
+-rw-rw-rw-   0        0        0    17084 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.2/src/nwb4fp/postprocess/nwbPHYnOPHYS.py
+-rw-rw-rw-   0        0        0    14469 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.2/src/nwb4fp/postprocess/quality_metrix.py
+drwxrwxrwx   0        0        0        0 2024-05-16 11:12:38.902888 nwb4fp-0.6.3.2/src/nwb4fp/preprocess/
+-rw-rw-rw-   0        0        0        0 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.2/src/nwb4fp/preprocess/__init__.py
+-rw-rw-rw-   0        0        0      459 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.2/src/nwb4fp/preprocess/copy_file.py
+-rw-rw-rw-   0        0        0      620 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.2/src/nwb4fp/preprocess/down_sample.py
+-rw-rw-rw-   0        0        0     8249 2024-05-13 14:58:38.000000 nwb4fp-0.6.3.2/src/nwb4fp/preprocess/down_sample_lfp.py
+-rw-rw-rw-   0        0        0     3712 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.2/src/nwb4fp/preprocess/extract_lfp.py
+-rw-rw-rw-   0        0        0      148 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.2/src/nwb4fp/preprocess/get_path.py
+-rw-rw-rw-   0        0        0     1203 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.2/src/nwb4fp/preprocess/load_data.py
+-rw-rw-rw-   0        0        0      244 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.2/src/nwb4fp/preprocess/run_phy.py
+drwxrwxrwx   0        0        0        0 2024-05-16 11:12:38.908927 nwb4fp-0.6.3.2/src/nwb4fp/test/
+drwxrwxrwx   0        0        0        0 2024-05-16 11:12:38.911945 nwb4fp-0.6.3.2/src/nwb4fp/test/run_scripts/
+-rw-rw-rw-   0        0        0     1525 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.2/src/nwb4fp/test/run_scripts/readnwb.py
+-rw-rw-rw-   0        0        0     1028 2024-05-13 13:05:19.000000 nwb4fp-0.6.3.2/src/nwb4fp/test/run_scripts/readnwb_0283.py
+-rw-rw-rw-   0        0        0     1069 2024-05-16 11:12:05.000000 nwb4fp-0.6.3.2/src/nwb4fp/test/run_scripts/readnwb_09PC.py
+-rw-rw-rw-   0        0        0     1448 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.2/src/nwb4fp/test/run_scripts/readnwb_09PD.py
+-rw-rw-rw-   0        0        0        0 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.2/src/nwb4fp/test/run_scripts/test.py
+-rw-rw-rw-   0        0        0     5828 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.2/src/nwb4fp/test/run_scripts/test_lfp.py
+drwxrwxrwx   0        0        0        0 2024-05-16 11:12:38.885922 nwb4fp-0.6.3.2/src/nwb4fp.egg-info/
+-rw-rw-rw-   0        0        0     5732 2024-05-16 11:12:38.000000 nwb4fp-0.6.3.2/src/nwb4fp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1143 2024-05-16 11:12:38.000000 nwb4fp-0.6.3.2/src/nwb4fp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 11:12:38.000000 nwb4fp-0.6.3.2/src/nwb4fp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     2885 2024-05-16 11:12:38.000000 nwb4fp-0.6.3.2/src/nwb4fp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-16 11:12:38.000000 nwb4fp-0.6.3.2/src/nwb4fp.egg-info/top_level.txt
```

### Comparing `nwb4fp-0.6.3.1/LICENSE` & `nwb4fp-0.6.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.3.1/PKG-INFO` & `nwb4fp-0.6.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nwb4fp
-Version: 0.6.3.1
+Version: 0.6.3.2
 Summary: Description of my package
 Home-page: https://github.com/sachuriga/QuattrocoloLab-nwb4fp
 Author: sachuriga
 Author-email: sachuriga.sachuriga@ntnu.no
 License-File: LICENSE
 Requires-Dist: aiobotocore==2.11.2
 Requires-Dist: aiohttp==3.9.3
```

### Comparing `nwb4fp-0.6.3.1/README.md` & `nwb4fp-0.6.3.2/README.md`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.3.1/setup.py` & `nwb4fp-0.6.3.2/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -6,18 +6,19 @@
         with open('requirements.txt', encoding='utf-8-sig') as req:
             return [line.strip() for line in req if line.strip() and not line.startswith('#')]
     except UnicodeDecodeError:
         with open('requirements.txt', encoding='utf-16') as req:
             return [line.strip() for line in req if line.strip() and not line.startswith('#')]
 setup(
     name='nwb4fp',
-    version='0.6.3.1',
+    version='0.6.3.2',
     url='https://github.com/sachuriga/QuattrocoloLab-nwb4fp',
     author='sachuriga',
     author_email='sachuriga.sachuriga@ntnu.no',
     description='Description of my package',
     #packages=find_packages(./src/),    
     install_requires=read_requirements(),
 )
+
 if __name__ == "__main__":
     ## pip list --format=freeze > requirements.txt
     setuptools.setup()
```

### Comparing `nwb4fp-0.6.3.1/src/nwb4fp/main/main_create_nwb.py` & `nwb4fp-0.6.3.2/src/nwb4fp/main/main_create_nwb.py`

 * *Files 8% similar despite different names*

```diff
@@ -55,26 +55,36 @@
             test_clusterInfo(file,
                              temp_folder,
                              save_path_test,
                              vedio_search_directory,
                              idun_vedio_path)
 
 
-def run_qmnwb(animals,base_data_folder,project_name,file_suffix, sex,age,species,vedio_search_directory,path_save,temp_folder):
+def run_qmnwb(animals,
+              base_data_folder,
+              project_name,
+              file_suffix, 
+              sex,age,species,
+              vedio_search_directory,
+              path_save,temp_folder,
+              skip_qmr: bool = False):
     for indvi in animals:
         ID = indvi
         counter = 0
         #getting sorted files02
         folder_path = fr"{str(base_data_folder)}/Ephys_Recording/{project_name}/{ID}/"
         ##for quality metrix
         sorted_files = load_data(folder_path, file_suffix=fr"{file_suffix}")
 
         for file in sorted_files:
             print(file)
-            qualitymetrix(file,temp_folder)
+            if skip_qmr:
+                pass
+            else:
+                qualitymetrix(file,temp_folder)
             add_wf_cor(fr"{file}_manual")
             nwbPHYnOPHYS(fr"{file}_manual",
                         sex,
                         age,
                         species,
                         vedio_search_directory,
                         path_to_save_nwbfile = path_save)
```

### Comparing `nwb4fp-0.6.3.1/src/nwb4fp/postprocess/Get_positions.py` & `nwb4fp-0.6.3.2/src/nwb4fp/postprocess/Get_positions.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.3.1/src/nwb4fp/postprocess/add_wfcor.py` & `nwb4fp-0.6.3.2/src/nwb4fp/postprocess/add_wfcor.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
     path_cluster_group = Path(fr"{path}/cluster_group.tsv")
     path_cluster_metrix = Path(fr"{path}/waveformsfm/extensions/quality_metrics/metrics.csv")
     path_templates = Path(fr"{path}/waveformsfm/extensions/templates_metrics/metrics.csv")
     path_ulocation = Path(fr"{path}/waveformsfm/extensions/unit_locations/unit_locations.npy")
     df0 = pd.read_csv(path_cluster_group, index_col=0, sep='\t')
     df11 = pd.read_csv(path_cluster_metrix)
-    df111 = pd.read_csv(path_cluster_metrix)
+    df111 = pd.read_csv(path_templates)
     
     df1 = pd.merge(df11, df111,left_index=True,right_index=True)
     df2 = pd.DataFrame(np.load(path_ulocation),columns=['x', 'y','z'])
     df3 = pd.merge(df0, df1,left_index=True,right_index=True)
     df4 = pd.merge(df3, df2,left_index=True,right_index=True)
 
     # List all files in the current directory
```

### Comparing `nwb4fp-0.6.3.1/src/nwb4fp/postprocess/extract_wf.py` & `nwb4fp-0.6.3.2/src/nwb4fp/postprocess/extract_wf.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.3.1/src/nwb4fp/postprocess/get_potential_merge.py` & `nwb4fp-0.6.3.2/src/nwb4fp/postprocess/get_potential_merge.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.3.1/src/nwb4fp/postprocess/nwbPHYnOPHYS.py` & `nwb4fp-0.6.3.2/src/nwb4fp/postprocess/nwbPHYnOPHYS.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.3.1/src/nwb4fp/postprocess/quality_metrix.py` & `nwb4fp-0.6.3.2/src/nwb4fp/postprocess/quality_metrix.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.3.1/src/nwb4fp/preprocess/down_sample.py` & `nwb4fp-0.6.3.2/src/nwb4fp/preprocess/down_sample.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.3.1/src/nwb4fp/preprocess/down_sample_lfp.py` & `nwb4fp-0.6.3.2/src/nwb4fp/preprocess/down_sample_lfp.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.3.1/src/nwb4fp/preprocess/extract_lfp.py` & `nwb4fp-0.6.3.2/src/nwb4fp/preprocess/extract_lfp.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.3.1/src/nwb4fp/preprocess/load_data.py` & `nwb4fp-0.6.3.2/src/nwb4fp/preprocess/load_data.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.3.1/src/nwb4fp/test/run_scripts/readnwb.py` & `nwb4fp-0.6.3.2/src/nwb4fp/test/run_scripts/readnwb.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.3.1/src/nwb4fp/test/run_scripts/readnwb_0283.py` & `nwb4fp-0.6.3.2/src/nwb4fp/test/run_scripts/readnwb_0283.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.3.1/src/nwb4fp/test/run_scripts/readnwb_09PC.py` & `nwb4fp-0.6.3.2/src/nwb4fp/test/run_scripts/readnwb_09PC.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 def main():
     import os
     import sys
     base_path = Path("Q:/Sachuriga/Sachuriga_Python")
     base_data_folder = Path("S:/Sachuriga/")
     sex = "F"
-    animals = ["65588", "65409", "65410","65935"] 
+    animals = ["65935","65283"] 
     age = "P45+"
     project_name = "CR_CA1"
     species = "Mus musculus"
     vedio_search_directory = base_data_folder/fr"Ephys_Vedio/CR_CA1/"
     path_save = base_data_folder/fr"nwb"
     temp_folder = Path(fr'C:/temp_waveform/{project_name}')
     save_path_test=(r"S:\Sachuriga/Ephys_Recording/4nwb_check.csv")
@@ -24,11 +24,13 @@
               project_name,
               file_suffix,
               sex,
               age,
               species,
               vedio_search_directory,
               path_save,
-              temp_folder)
+              temp_folder,
+              skip_qmr=True,)
+
     
 if __name__ == "__main__":
     main()
```

### Comparing `nwb4fp-0.6.3.1/src/nwb4fp/test/run_scripts/readnwb_09PD.py` & `nwb4fp-0.6.3.2/src/nwb4fp/test/run_scripts/readnwb_09PD.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.3.1/src/nwb4fp/test/run_scripts/test_lfp.py` & `nwb4fp-0.6.3.2/src/nwb4fp/test/run_scripts/test_lfp.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.3.1/src/nwb4fp.egg-info/PKG-INFO` & `nwb4fp-0.6.3.2/src/nwb4fp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nwb4fp
-Version: 0.6.3.1
+Version: 0.6.3.2
 Summary: Description of my package
 Home-page: https://github.com/sachuriga/QuattrocoloLab-nwb4fp
 Author: sachuriga
 Author-email: sachuriga.sachuriga@ntnu.no
 License-File: LICENSE
 Requires-Dist: aiobotocore==2.11.2
 Requires-Dist: aiohttp==3.9.3
```

### Comparing `nwb4fp-0.6.3.1/src/nwb4fp.egg-info/SOURCES.txt` & `nwb4fp-0.6.3.2/src/nwb4fp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.3.1/src/nwb4fp.egg-info/requires.txt` & `nwb4fp-0.6.3.2/src/nwb4fp.egg-info/requires.txt`

 * *Files identical despite different names*

