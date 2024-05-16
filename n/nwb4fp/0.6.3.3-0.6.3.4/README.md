# Comparing `tmp/nwb4fp-0.6.3.3.tar.gz` & `tmp/nwb4fp-0.6.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nwb4fp-0.6.3.3.tar", last modified: Thu May 16 11:24:40 2024, max compression
+gzip compressed data, was "nwb4fp-0.6.3.4.tar", last modified: Thu May 16 11:53:38 2024, max compression
```

## Comparing `nwb4fp-0.6.3.3.tar` & `nwb4fp-0.6.3.4.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 11:24:40.158890 nwb4fp-0.6.3.3/
--rw-rw-rw-   0        0        0     1089 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.3/LICENSE
--rw-rw-rw-   0        0        0     5732 2024-05-16 11:24:40.151898 nwb4fp-0.6.3.3/PKG-INFO
--rw-rw-rw-   0        0        0     6901 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.3/README.md
--rw-rw-rw-   0        0        0       42 2024-05-16 11:24:40.179900 nwb4fp-0.6.3.3/setup.cfg
--rw-rw-rw-   0        0        0      888 2024-05-16 11:19:02.000000 nwb4fp-0.6.3.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-16 11:24:39.329889 nwb4fp-0.6.3.3/src/
-drwxrwxrwx   0        0        0        0 2024-05-16 11:24:39.355879 nwb4fp-0.6.3.3/src/nwb4fp/
-drwxrwxrwx   0        0        0        0 2024-05-16 11:24:39.674881 nwb4fp-0.6.3.3/src/nwb4fp/main/
--rw-rw-rw-   0        0        0        0 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.3/src/nwb4fp/main/__init__.py
--rw-rw-rw-   0        0        0     3799 2024-05-16 11:16:18.000000 nwb4fp-0.6.3.3/src/nwb4fp/main/main_create_nwb.py
-drwxrwxrwx   0        0        0        0 2024-05-16 11:24:39.829888 nwb4fp-0.6.3.3/src/nwb4fp/postprocess/
--rw-rw-rw-   0        0        0    15551 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.3/src/nwb4fp/postprocess/Get_positions.py
--rw-rw-rw-   0        0        0        0 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.3/src/nwb4fp/postprocess/__init__.py
--rw-rw-rw-   0        0        0     1844 2024-05-16 11:18:45.000000 nwb4fp-0.6.3.3/src/nwb4fp/postprocess/add_wfcor.py
--rw-rw-rw-   0        0        0      470 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.3/src/nwb4fp/postprocess/dlc_kinematic.py
--rw-rw-rw-   0        0        0     2485 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.3/src/nwb4fp/postprocess/extract_wf.py
--rw-rw-rw-   0        0        0     1343 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.3/src/nwb4fp/postprocess/get_potential_merge.py
--rw-rw-rw-   0        0        0        0 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.3/src/nwb4fp/postprocess/lfp_channel.py
--rw-rw-rw-   0        0        0    17084 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.3/src/nwb4fp/postprocess/nwbPHYnOPHYS.py
--rw-rw-rw-   0        0        0    14469 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.3/src/nwb4fp/postprocess/quality_metrix.py
-drwxrwxrwx   0        0        0        0 2024-05-16 11:24:39.951902 nwb4fp-0.6.3.3/src/nwb4fp/preprocess/
--rw-rw-rw-   0        0        0        0 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.3/src/nwb4fp/preprocess/__init__.py
--rw-rw-rw-   0        0        0      459 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.3/src/nwb4fp/preprocess/copy_file.py
--rw-rw-rw-   0        0        0      620 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.3/src/nwb4fp/preprocess/down_sample.py
--rw-rw-rw-   0        0        0     8249 2024-05-13 14:58:38.000000 nwb4fp-0.6.3.3/src/nwb4fp/preprocess/down_sample_lfp.py
--rw-rw-rw-   0        0        0     3712 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.3/src/nwb4fp/preprocess/extract_lfp.py
--rw-rw-rw-   0        0        0      148 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.3/src/nwb4fp/preprocess/get_path.py
--rw-rw-rw-   0        0        0     1203 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.3/src/nwb4fp/preprocess/load_data.py
--rw-rw-rw-   0        0        0      244 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.3/src/nwb4fp/preprocess/run_phy.py
-drwxrwxrwx   0        0        0        0 2024-05-16 11:24:39.357893 nwb4fp-0.6.3.3/src/nwb4fp/test/
-drwxrwxrwx   0        0        0        0 2024-05-16 11:24:40.006895 nwb4fp-0.6.3.3/src/nwb4fp/test/run_scripts/
--rw-rw-rw-   0        0        0     1525 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.3/src/nwb4fp/test/run_scripts/readnwb.py
--rw-rw-rw-   0        0        0     1028 2024-05-13 13:05:19.000000 nwb4fp-0.6.3.3/src/nwb4fp/test/run_scripts/readnwb_0283.py
--rw-rw-rw-   0        0        0     1068 2024-05-16 11:17:06.000000 nwb4fp-0.6.3.3/src/nwb4fp/test/run_scripts/readnwb_09PC.py
--rw-rw-rw-   0        0        0     1448 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.3/src/nwb4fp/test/run_scripts/readnwb_09PD.py
--rw-rw-rw-   0        0        0        0 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.3/src/nwb4fp/test/run_scripts/test.py
--rw-rw-rw-   0        0        0     5828 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.3/src/nwb4fp/test/run_scripts/test_lfp.py
-drwxrwxrwx   0        0        0        0 2024-05-16 11:24:39.652881 nwb4fp-0.6.3.3/src/nwb4fp.egg-info/
--rw-rw-rw-   0        0        0     5732 2024-05-16 11:24:39.000000 nwb4fp-0.6.3.3/src/nwb4fp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1143 2024-05-16 11:24:39.000000 nwb4fp-0.6.3.3/src/nwb4fp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 11:24:39.000000 nwb4fp-0.6.3.3/src/nwb4fp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     2885 2024-05-16 11:24:39.000000 nwb4fp-0.6.3.3/src/nwb4fp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-16 11:24:39.000000 nwb4fp-0.6.3.3/src/nwb4fp.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-16 11:53:38.547735 nwb4fp-0.6.3.4/
+-rw-rw-rw-   0        0        0     1089 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.4/LICENSE
+-rw-rw-rw-   0        0        0     5732 2024-05-16 11:53:38.538743 nwb4fp-0.6.3.4/PKG-INFO
+-rw-rw-rw-   0        0        0     6901 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.4/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-16 11:53:38.564743 nwb4fp-0.6.3.4/setup.cfg
+-rw-rw-rw-   0        0        0      888 2024-05-16 11:53:34.000000 nwb4fp-0.6.3.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 11:53:37.836741 nwb4fp-0.6.3.4/src/
+drwxrwxrwx   0        0        0        0 2024-05-16 11:53:37.852752 nwb4fp-0.6.3.4/src/nwb4fp/
+drwxrwxrwx   0        0        0        0 2024-05-16 11:53:37.985744 nwb4fp-0.6.3.4/src/nwb4fp/main/
+-rw-rw-rw-   0        0        0        0 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.4/src/nwb4fp/main/__init__.py
+-rw-rw-rw-   0        0        0     3846 2024-05-16 11:52:07.000000 nwb4fp-0.6.3.4/src/nwb4fp/main/main_create_nwb.py
+drwxrwxrwx   0        0        0        0 2024-05-16 11:53:38.171741 nwb4fp-0.6.3.4/src/nwb4fp/postprocess/
+-rw-rw-rw-   0        0        0    15551 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.4/src/nwb4fp/postprocess/Get_positions.py
+-rw-rw-rw-   0        0        0        0 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.4/src/nwb4fp/postprocess/__init__.py
+-rw-rw-rw-   0        0        0     1844 2024-05-16 11:18:45.000000 nwb4fp-0.6.3.4/src/nwb4fp/postprocess/add_wfcor.py
+-rw-rw-rw-   0        0        0      470 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.4/src/nwb4fp/postprocess/dlc_kinematic.py
+-rw-rw-rw-   0        0        0     2485 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.4/src/nwb4fp/postprocess/extract_wf.py
+-rw-rw-rw-   0        0        0     1343 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.4/src/nwb4fp/postprocess/get_potential_merge.py
+-rw-rw-rw-   0        0        0        0 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.4/src/nwb4fp/postprocess/lfp_channel.py
+-rw-rw-rw-   0        0        0    17284 2024-05-16 11:52:05.000000 nwb4fp-0.6.3.4/src/nwb4fp/postprocess/nwbPHYnOPHYS.py
+-rw-rw-rw-   0        0        0    14469 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.4/src/nwb4fp/postprocess/quality_metrix.py
+drwxrwxrwx   0        0        0        0 2024-05-16 11:53:38.310735 nwb4fp-0.6.3.4/src/nwb4fp/preprocess/
+-rw-rw-rw-   0        0        0        0 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.4/src/nwb4fp/preprocess/__init__.py
+-rw-rw-rw-   0        0        0      459 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.4/src/nwb4fp/preprocess/copy_file.py
+-rw-rw-rw-   0        0        0      620 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.4/src/nwb4fp/preprocess/down_sample.py
+-rw-rw-rw-   0        0        0     8249 2024-05-13 14:58:38.000000 nwb4fp-0.6.3.4/src/nwb4fp/preprocess/down_sample_lfp.py
+-rw-rw-rw-   0        0        0     3712 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.4/src/nwb4fp/preprocess/extract_lfp.py
+-rw-rw-rw-   0        0        0      148 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.4/src/nwb4fp/preprocess/get_path.py
+-rw-rw-rw-   0        0        0     1203 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.4/src/nwb4fp/preprocess/load_data.py
+-rw-rw-rw-   0        0        0      244 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.4/src/nwb4fp/preprocess/run_phy.py
+drwxrwxrwx   0        0        0        0 2024-05-16 11:53:37.854763 nwb4fp-0.6.3.4/src/nwb4fp/test/
+drwxrwxrwx   0        0        0        0 2024-05-16 11:53:38.405740 nwb4fp-0.6.3.4/src/nwb4fp/test/run_scripts/
+-rw-rw-rw-   0        0        0     1525 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.4/src/nwb4fp/test/run_scripts/readnwb.py
+-rw-rw-rw-   0        0        0     1028 2024-05-13 13:05:19.000000 nwb4fp-0.6.3.4/src/nwb4fp/test/run_scripts/readnwb_0283.py
+-rw-rw-rw-   0        0        0     1108 2024-05-16 11:52:09.000000 nwb4fp-0.6.3.4/src/nwb4fp/test/run_scripts/readnwb_09PC.py
+-rw-rw-rw-   0        0        0     1448 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.4/src/nwb4fp/test/run_scripts/readnwb_09PD.py
+-rw-rw-rw-   0        0        0        0 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.4/src/nwb4fp/test/run_scripts/test.py
+-rw-rw-rw-   0        0        0     5828 2024-05-13 12:41:11.000000 nwb4fp-0.6.3.4/src/nwb4fp/test/run_scripts/test_lfp.py
+drwxrwxrwx   0        0        0        0 2024-05-16 11:53:37.963752 nwb4fp-0.6.3.4/src/nwb4fp.egg-info/
+-rw-rw-rw-   0        0        0     5732 2024-05-16 11:53:37.000000 nwb4fp-0.6.3.4/src/nwb4fp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1143 2024-05-16 11:53:37.000000 nwb4fp-0.6.3.4/src/nwb4fp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 11:53:37.000000 nwb4fp-0.6.3.4/src/nwb4fp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     2885 2024-05-16 11:53:37.000000 nwb4fp-0.6.3.4/src/nwb4fp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-16 11:53:37.000000 nwb4fp-0.6.3.4/src/nwb4fp.egg-info/top_level.txt
```

### Comparing `nwb4fp-0.6.3.3/LICENSE` & `nwb4fp-0.6.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.3.3/PKG-INFO` & `nwb4fp-0.6.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nwb4fp
-Version: 0.6.3.3
+Version: 0.6.3.4
 Summary: Description of my package
 Home-page: https://github.com/sachuriga/QuattrocoloLab-nwb4fp
 Author: sachuriga
 Author-email: sachuriga.sachuriga@ntnu.no
 License-File: LICENSE
 Requires-Dist: aiobotocore==2.11.2
 Requires-Dist: aiohttp==3.9.3
```

### Comparing `nwb4fp-0.6.3.3/README.md` & `nwb4fp-0.6.3.4/README.md`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.3.3/setup.py` & `nwb4fp-0.6.3.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
         with open('requirements.txt', encoding='utf-8-sig') as req:
             return [line.strip() for line in req if line.strip() and not line.startswith('#')]
     except UnicodeDecodeError:
         with open('requirements.txt', encoding='utf-16') as req:
             return [line.strip() for line in req if line.strip() and not line.startswith('#')]
 setup(
     name='nwb4fp',
-    version='0.6.3.3',
+    version='0.6.3.4',
     url='https://github.com/sachuriga/QuattrocoloLab-nwb4fp',
     author='sachuriga',
     author_email='sachuriga.sachuriga@ntnu.no',
     description='Description of my package',
     #packages=find_packages(./src/),    
     install_requires=read_requirements(),
 )
```

### Comparing `nwb4fp-0.6.3.3/src/nwb4fp/main/main_create_nwb.py` & `nwb4fp-0.6.3.4/src/nwb4fp/main/main_create_nwb.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,15 +83,16 @@
                 qualitymetrix(file,temp_folder)
             add_wf_cor(fr"{file}_manual")
             nwbPHYnOPHYS(fr"{file}_manual",
                         sex,
                         age,
                         species,
                         vedio_search_directory,
-                        path_to_save_nwbfile = path_save)
+                        path_to_save_nwbfile = path_save,
+                        skip_qmr = skip_qmr) 
             counter += 1
             percent = counter/len(sorted_files)
             #wf4unim(fr"{file}_manual")
             print(f"{percent} % completet!!!!{file}\ncreated new phy folder {file}_manual \ncreated nwb file at {path_save}for {ID} {age} {species}\n\n\n\n")
 
 if __name__== "__main__":
     main()
```

### Comparing `nwb4fp-0.6.3.3/src/nwb4fp/postprocess/Get_positions.py` & `nwb4fp-0.6.3.4/src/nwb4fp/postprocess/Get_positions.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.3.3/src/nwb4fp/postprocess/add_wfcor.py` & `nwb4fp-0.6.3.4/src/nwb4fp/postprocess/add_wfcor.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.3.3/src/nwb4fp/postprocess/extract_wf.py` & `nwb4fp-0.6.3.4/src/nwb4fp/postprocess/extract_wf.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.3.3/src/nwb4fp/postprocess/get_potential_merge.py` & `nwb4fp-0.6.3.4/src/nwb4fp/postprocess/get_potential_merge.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.3.3/src/nwb4fp/postprocess/nwbPHYnOPHYS.py` & `nwb4fp-0.6.3.4/src/nwb4fp/postprocess/nwbPHYnOPHYS.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,21 @@
     sex = "F"
     ages = "P60"
     species = "Mus musculus"
     vedio_search_directory = "S:/Sachuriga/Ephys_Vedio/CR_CA1"
     path_to_save_nwbfile = "S:/Sachuriga/nwb"
     nwbPHYnOPHYS(path, sex, ages, species, vedio_search_directory, path_to_save_nwbfile)  # Added missing argument
 
-def nwbPHYnOPHYS(path,sex,ages,species,vedio_search_directory,path_to_save_nwbfile):
+def nwbPHYnOPHYS(path,
+                 sex,
+                 ages,
+                 species,
+                 vedio_search_directory,
+                 path_to_save_nwbfile,
+                 skip_qmr: bool = False):
 
     if path.endswith("phy_k_manual"):
         num2cal = int(41)
     elif path.endswith("phy_k"):
         num2cal = int(35)
 
     temp = path[0 - num2cal:]
@@ -156,16 +162,19 @@
                         folder_path = fr"{ECEPHY_DATA_PATH}/Record Node 102"
                         timestemp = np.load(fr'{folder_path}/experiment1/recording1/continuous/OE_FPGA_Acquisition_Board-101.Rhythm Data/sample_numbers.npy')
                     except FileNotFoundError:
                         folder_path = fr"{ECEPHY_DATA_PATH}/Record Node 101"
                         timestemp = np.load(fr'{folder_path}/experiment1/recording1/continuous/OE_FPGA_Acquisition_Board-100.Rhythm Data/sample_numbers.npy')
         
         print(folder_path)
-        time_spk = timestemp[sample_num]
-        np.save(fr"{folder1_path}/spike_times.npy",time_spk)
+        if skip_qmr:
+            pass
+        else:
+            time_spk = timestemp[sample_num]
+            np.save(fr"{folder1_path}/spike_times.npy",time_spk)
         interface_phy = PhySortingInterface(folder_path=folder1_path, verbose=False)
         # For data provenance we add the time zone information to the conversionSS
         converter = ConverterPipe(data_interfaces=[interface_phy], verbose=False)    
         metadata = converter.get_metadata()
         session_start_time = datetime.now(tzlocal())
         metadata["NWBFile"].update(session_start_time=session_start_time)
```

### Comparing `nwb4fp-0.6.3.3/src/nwb4fp/postprocess/quality_metrix.py` & `nwb4fp-0.6.3.4/src/nwb4fp/postprocess/quality_metrix.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.3.3/src/nwb4fp/preprocess/down_sample.py` & `nwb4fp-0.6.3.4/src/nwb4fp/preprocess/down_sample.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.3.3/src/nwb4fp/preprocess/down_sample_lfp.py` & `nwb4fp-0.6.3.4/src/nwb4fp/preprocess/down_sample_lfp.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.3.3/src/nwb4fp/preprocess/extract_lfp.py` & `nwb4fp-0.6.3.4/src/nwb4fp/preprocess/extract_lfp.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.3.3/src/nwb4fp/preprocess/load_data.py` & `nwb4fp-0.6.3.4/src/nwb4fp/preprocess/load_data.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.3.3/src/nwb4fp/test/run_scripts/readnwb.py` & `nwb4fp-0.6.3.4/src/nwb4fp/test/run_scripts/readnwb.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.3.3/src/nwb4fp/test/run_scripts/readnwb_0283.py` & `nwb4fp-0.6.3.4/src/nwb4fp/test/run_scripts/readnwb_0283.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.3.3/src/nwb4fp/test/run_scripts/readnwb_09PC.py` & `nwb4fp-0.6.3.4/src/nwb4fp/test/run_scripts/readnwb_09PC.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 def main():
     import os
     import sys
     base_path = Path("Q:/Sachuriga/Sachuriga_Python")
     base_data_folder = Path("S:/Sachuriga/")
     sex = "F"
-    animals = ["65935","65283"] 
+    animals = ["65091","65165","65283","65409","65410","65588","65935"] 
     age = "P45+"
     project_name = "CR_CA1"
     species = "Mus musculus"
     vedio_search_directory = base_data_folder/fr"Ephys_Vedio/CR_CA1/"
     path_save = base_data_folder/fr"nwb"
     temp_folder = Path(fr'C:/temp_waveform/{project_name}')
     save_path_test=(r"S:\Sachuriga/Ephys_Recording/4nwb_check.csv")
```

### Comparing `nwb4fp-0.6.3.3/src/nwb4fp/test/run_scripts/readnwb_09PD.py` & `nwb4fp-0.6.3.4/src/nwb4fp/test/run_scripts/readnwb_09PD.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.3.3/src/nwb4fp/test/run_scripts/test_lfp.py` & `nwb4fp-0.6.3.4/src/nwb4fp/test/run_scripts/test_lfp.py`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.3.3/src/nwb4fp.egg-info/PKG-INFO` & `nwb4fp-0.6.3.4/src/nwb4fp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nwb4fp
-Version: 0.6.3.3
+Version: 0.6.3.4
 Summary: Description of my package
 Home-page: https://github.com/sachuriga/QuattrocoloLab-nwb4fp
 Author: sachuriga
 Author-email: sachuriga.sachuriga@ntnu.no
 License-File: LICENSE
 Requires-Dist: aiobotocore==2.11.2
 Requires-Dist: aiohttp==3.9.3
```

### Comparing `nwb4fp-0.6.3.3/src/nwb4fp.egg-info/SOURCES.txt` & `nwb4fp-0.6.3.4/src/nwb4fp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nwb4fp-0.6.3.3/src/nwb4fp.egg-info/requires.txt` & `nwb4fp-0.6.3.4/src/nwb4fp.egg-info/requires.txt`

 * *Files identical despite different names*

