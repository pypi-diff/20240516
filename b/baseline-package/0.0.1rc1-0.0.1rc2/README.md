# Comparing `tmp/baseline_package-0.0.1rc1.tar.gz` & `tmp/baseline_package-0.0.1rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "baseline_package-0.0.1rc1.tar", last modified: Thu May 16 14:47:36 2024, max compression
+gzip compressed data, was "baseline_package-0.0.1rc2.tar", last modified: Thu May 16 15:08:52 2024, max compression
```

## Comparing `baseline_package-0.0.1rc1.tar` & `baseline_package-0.0.1rc2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 wolf       (501) staff       (20)        0 2024-05-16 14:47:36.740090 baseline_package-0.0.1rc1/
--rw-r--r--   0 wolf       (501) staff       (20)     1118 2024-05-16 14:37:29.000000 baseline_package-0.0.1rc1/LICENSE.md
--rw-r--r--   0 wolf       (501) staff       (20)     3847 2024-05-16 14:47:36.739923 baseline_package-0.0.1rc1/PKG-INFO
--rw-r--r--   0 wolf       (501) staff       (20)     2852 2024-05-16 14:37:29.000000 baseline_package-0.0.1rc1/README.md
-drwxr-xr-x   0 wolf       (501) staff       (20)        0 2024-05-16 14:47:36.736235 baseline_package-0.0.1rc1/baseline_package/
--rw-r--r--   0 wolf       (501) staff       (20)      254 2024-05-16 14:38:40.000000 baseline_package-0.0.1rc1/baseline_package/__init__.py
--rw-r--r--   0 wolf       (501) staff       (20)     2996 2024-05-16 14:45:27.000000 baseline_package-0.0.1rc1/baseline_package/cli.py
--rw-r--r--   0 wolf       (501) staff       (20)      847 2024-05-16 14:38:40.000000 baseline_package-0.0.1rc1/baseline_package/config.py
--rw-r--r--   0 wolf       (501) staff       (20)      533 2024-05-16 14:38:40.000000 baseline_package-0.0.1rc1/baseline_package/constants.py
--rw-r--r--   0 wolf       (501) staff       (20)      461 2024-05-16 14:38:40.000000 baseline_package-0.0.1rc1/baseline_package/exceptions.py
--rw-r--r--   0 wolf       (501) staff       (20)      518 2024-05-16 14:38:40.000000 baseline_package-0.0.1rc1/baseline_package/globals.py
--rw-r--r--   0 wolf       (501) staff       (20)      925 2024-05-16 14:44:54.000000 baseline_package-0.0.1rc1/baseline_package/main.py
--rw-r--r--   0 wolf       (501) staff       (20)     1411 2024-05-16 14:38:40.000000 baseline_package-0.0.1rc1/baseline_package/notify.py
-drwxr-xr-x   0 wolf       (501) staff       (20)        0 2024-05-16 14:47:36.739388 baseline_package-0.0.1rc1/baseline_package.egg-info/
--rw-r--r--   0 wolf       (501) staff       (20)     3847 2024-05-16 14:47:36.000000 baseline_package-0.0.1rc1/baseline_package.egg-info/PKG-INFO
--rw-r--r--   0 wolf       (501) staff       (20)      502 2024-05-16 14:47:36.000000 baseline_package-0.0.1rc1/baseline_package.egg-info/SOURCES.txt
--rw-r--r--   0 wolf       (501) staff       (20)        1 2024-05-16 14:47:36.000000 baseline_package-0.0.1rc1/baseline_package.egg-info/dependency_links.txt
--rw-r--r--   0 wolf       (501) staff       (20)       64 2024-05-16 14:47:36.000000 baseline_package-0.0.1rc1/baseline_package.egg-info/entry_points.txt
--rw-r--r--   0 wolf       (501) staff       (20)       30 2024-05-16 14:47:36.000000 baseline_package-0.0.1rc1/baseline_package.egg-info/requires.txt
--rw-r--r--   0 wolf       (501) staff       (20)       17 2024-05-16 14:47:36.000000 baseline_package-0.0.1rc1/baseline_package.egg-info/top_level.txt
--rw-r--r--   0 wolf       (501) staff       (20)      526 2024-05-16 14:47:36.740805 baseline_package-0.0.1rc1/setup.cfg
--rw-r--r--   0 wolf       (501) staff       (20)     1493 2024-05-16 14:40:43.000000 baseline_package-0.0.1rc1/setup.py
+drwxr-xr-x   0 wolf       (501) staff       (20)        0 2024-05-16 15:08:52.405548 baseline_package-0.0.1rc2/
+-rw-r--r--   0 wolf       (501) staff       (20)     1118 2024-05-16 14:37:29.000000 baseline_package-0.0.1rc2/LICENSE.md
+-rw-r--r--   0 wolf       (501) staff       (20)     3852 2024-05-16 15:08:52.405374 baseline_package-0.0.1rc2/PKG-INFO
+-rw-r--r--   0 wolf       (501) staff       (20)     2852 2024-05-16 14:37:29.000000 baseline_package-0.0.1rc2/README.md
+drwxr-xr-x   0 wolf       (501) staff       (20)        0 2024-05-16 15:08:52.401508 baseline_package-0.0.1rc2/baseline_package/
+-rw-r--r--   0 wolf       (501) staff       (20)      254 2024-05-16 14:38:40.000000 baseline_package-0.0.1rc2/baseline_package/__init__.py
+-rw-r--r--   0 wolf       (501) staff       (20)     2996 2024-05-16 14:45:27.000000 baseline_package-0.0.1rc2/baseline_package/cli.py
+-rw-r--r--   0 wolf       (501) staff       (20)      847 2024-05-16 14:38:40.000000 baseline_package-0.0.1rc2/baseline_package/config.py
+-rw-r--r--   0 wolf       (501) staff       (20)      533 2024-05-16 14:38:40.000000 baseline_package-0.0.1rc2/baseline_package/constants.py
+-rw-r--r--   0 wolf       (501) staff       (20)      461 2024-05-16 14:38:40.000000 baseline_package-0.0.1rc2/baseline_package/exceptions.py
+-rw-r--r--   0 wolf       (501) staff       (20)      518 2024-05-16 14:38:40.000000 baseline_package-0.0.1rc2/baseline_package/globals.py
+-rw-r--r--   0 wolf       (501) staff       (20)      945 2024-05-16 15:00:19.000000 baseline_package-0.0.1rc2/baseline_package/main.py
+-rw-r--r--   0 wolf       (501) staff       (20)     1411 2024-05-16 14:38:40.000000 baseline_package-0.0.1rc2/baseline_package/notify.py
+drwxr-xr-x   0 wolf       (501) staff       (20)        0 2024-05-16 15:08:52.404732 baseline_package-0.0.1rc2/baseline_package.egg-info/
+-rw-r--r--   0 wolf       (501) staff       (20)     3852 2024-05-16 15:08:52.000000 baseline_package-0.0.1rc2/baseline_package.egg-info/PKG-INFO
+-rw-r--r--   0 wolf       (501) staff       (20)      502 2024-05-16 15:08:52.000000 baseline_package-0.0.1rc2/baseline_package.egg-info/SOURCES.txt
+-rw-r--r--   0 wolf       (501) staff       (20)        1 2024-05-16 15:08:52.000000 baseline_package-0.0.1rc2/baseline_package.egg-info/dependency_links.txt
+-rw-r--r--   0 wolf       (501) staff       (20)       64 2024-05-16 15:08:52.000000 baseline_package-0.0.1rc2/baseline_package.egg-info/entry_points.txt
+-rw-r--r--   0 wolf       (501) staff       (20)       35 2024-05-16 15:08:52.000000 baseline_package-0.0.1rc2/baseline_package.egg-info/requires.txt
+-rw-r--r--   0 wolf       (501) staff       (20)       17 2024-05-16 15:08:52.000000 baseline_package-0.0.1rc2/baseline_package.egg-info/top_level.txt
+-rw-r--r--   0 wolf       (501) staff       (20)      526 2024-05-16 15:08:52.406236 baseline_package-0.0.1rc2/setup.cfg
+-rw-r--r--   0 wolf       (501) staff       (20)     1493 2024-05-16 15:08:24.000000 baseline_package-0.0.1rc2/setup.py
```

### Comparing `baseline_package-0.0.1rc1/LICENSE.md` & `baseline_package-0.0.1rc2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `baseline_package-0.0.1rc1/PKG-INFO` & `baseline_package-0.0.1rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baseline-package
-Version: 0.0.1rc1
+Version: 0.0.1rc2
 Summary: A nice description will go here
 Home-page: https://github.com/GreyTeamToolbox/baseline-package
 Author: Wolf Software
 Author-email: pypi@wolfsoftware.com
 Project-URL:  Source, https://github.com/GreyTeamToolbox/baseline-package
 Project-URL:  Tracker, https://github.com/GreyTeamToolbox/baseline-package/issues/
 Project-URL:  Documentation, https://github.com/GreyTeamToolbox/baseline-package
@@ -16,15 +16,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: colorama==0.4.6
-Requires-Dist: pytest==7.4.4
+Requires-Dist: setuptools==69.5.1
 
 <!-- markdownlint-disable -->
 <p align="center">
     <a href="https://github.com/GreyTeamToolbox/">
         <img src="https://cdn.wolfsoftware.com/assets/images/github/organisations/greyteamtoolbox/black-and-white-circle-256.png" alt="GreyTeamToolbox logo" />
     </a>
     <br />
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 2.1 Name: baseline-package Version: 0.0.1rc1 Summary: A nice
+Metadata-Version: 2.1 Name: baseline-package Version: 0.0.1rc2 Summary: A nice
 description will go here Home-page: https://github.com/GreyTeamToolbox/
 baseline-package Author: Wolf Software Author-email: pypi@wolfsoftware.com
 Project-URL: Source, https://github.com/GreyTeamToolbox/baseline-package
 Project-URL: Tracker, https://github.com/GreyTeamToolbox/baseline-package/
 issues/ Project-URL: Documentation, https://github.com/GreyTeamToolbox/
 baseline-package Project-URL: Funding, https://ko-fi.com/wolfsoftware Project-
 URL: Say Thanks!, https://github.com/sponsors/TGWolf Classifier: Environment ::
 Console Classifier: Intended Audience :: Developers Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Classifier: Topic :: Software
 Development Requires-Python: >=3.9 Description-Content-Type: text/markdown
 License-File: LICENSE.md Requires-Dist: colorama==0.4.6 Requires-Dist:
-pytest==7.4.4
+setuptools==69.5.1
                             _[_G_r_e_y_T_e_a_m_T_o_o_l_b_o_x_ _l_o_g_o_]
                     _[_G_i_t_h_u_b_ _B_u_i_l_d_ _S_t_a_t_u_s_]_[_L_i_c_e_n_s_e_]_[_C_r_e_a_t_e_d_]
                   _[_R_e_l_e_a_s_e_]_[_R_e_l_e_a_s_e_d_]_[_C_o_m_m_i_t_s_ _s_i_n_c_e_ _r_e_l_e_a_s_e_]
   _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_C_o_d_e_%_2_0_o_f_%_2_0_C_o_n_d_u_c_t_-_b_l_u_e_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_]
  _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_C_o_n_t_r_i_b_u_t_i_n_g_-_b_l_u_e_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_]_[_h_t_t_p_s_:_/_/
   _i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_R_e_p_o_r_t_%_2_0_S_e_c_u_r_i_t_y_%_2_0_C_o_n_c_e_r_n_-_b_l_u_e_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_]
      _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_G_e_t_%_2_0_S_u_p_p_o_r_t_-_b_l_u_e_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_]
```

### Comparing `baseline_package-0.0.1rc1/README.md` & `baseline_package-0.0.1rc2/README.md`

 * *Files identical despite different names*

### Comparing `baseline_package-0.0.1rc1/baseline_package/cli.py` & `baseline_package-0.0.1rc2/baseline_package/cli.py`

 * *Files identical despite different names*

### Comparing `baseline_package-0.0.1rc1/baseline_package/config.py` & `baseline_package-0.0.1rc2/baseline_package/config.py`

 * *Files identical despite different names*

### Comparing `baseline_package-0.0.1rc1/baseline_package/constants.py` & `baseline_package-0.0.1rc2/baseline_package/constants.py`

 * *Files identical despite different names*

### Comparing `baseline_package-0.0.1rc1/baseline_package/globals.py` & `baseline_package-0.0.1rc2/baseline_package/globals.py`

 * *Files identical despite different names*

### Comparing `baseline_package-0.0.1rc1/baseline_package/main.py` & `baseline_package-0.0.1rc2/baseline_package/main.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,15 @@
+#!/usr/bin/env python
 """This is the summary line.
 
 This is the further elaboration of the docstring. Within this section,
 you can elaborate further on details as appropriate for the situation.
 Notice that the summary and the elaboration is separated by a blank new
 line.
 """
-
 import sys
 
 from .cli import run
 from .notify import system
 
 
 def main() -> None:
@@ -18,15 +18,14 @@
 
     This function serves as the entry point of the script. It is responsible
     for invoking the `process_arguments` function, which handles the processing
     of command-line arguments. The `main` function does not take any parameters
     and does not return any value. It ensures that the script's functionality
     is triggered correctly when the script is executed.
     """
-
     try:
         run()
     except KeyboardInterrupt:
         system("\n[*] Exiting Program\n")
         sys.exit(1)
```

### Comparing `baseline_package-0.0.1rc1/baseline_package/notify.py` & `baseline_package-0.0.1rc2/baseline_package/notify.py`

 * *Files identical despite different names*

### Comparing `baseline_package-0.0.1rc1/baseline_package.egg-info/PKG-INFO` & `baseline_package-0.0.1rc2/baseline_package.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baseline-package
-Version: 0.0.1rc1
+Version: 0.0.1rc2
 Summary: A nice description will go here
 Home-page: https://github.com/GreyTeamToolbox/baseline-package
 Author: Wolf Software
 Author-email: pypi@wolfsoftware.com
 Project-URL:  Source, https://github.com/GreyTeamToolbox/baseline-package
 Project-URL:  Tracker, https://github.com/GreyTeamToolbox/baseline-package/issues/
 Project-URL:  Documentation, https://github.com/GreyTeamToolbox/baseline-package
@@ -16,15 +16,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: colorama==0.4.6
-Requires-Dist: pytest==7.4.4
+Requires-Dist: setuptools==69.5.1
 
 <!-- markdownlint-disable -->
 <p align="center">
     <a href="https://github.com/GreyTeamToolbox/">
         <img src="https://cdn.wolfsoftware.com/assets/images/github/organisations/greyteamtoolbox/black-and-white-circle-256.png" alt="GreyTeamToolbox logo" />
     </a>
     <br />
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 2.1 Name: baseline-package Version: 0.0.1rc1 Summary: A nice
+Metadata-Version: 2.1 Name: baseline-package Version: 0.0.1rc2 Summary: A nice
 description will go here Home-page: https://github.com/GreyTeamToolbox/
 baseline-package Author: Wolf Software Author-email: pypi@wolfsoftware.com
 Project-URL: Source, https://github.com/GreyTeamToolbox/baseline-package
 Project-URL: Tracker, https://github.com/GreyTeamToolbox/baseline-package/
 issues/ Project-URL: Documentation, https://github.com/GreyTeamToolbox/
 baseline-package Project-URL: Funding, https://ko-fi.com/wolfsoftware Project-
 URL: Say Thanks!, https://github.com/sponsors/TGWolf Classifier: Environment ::
 Console Classifier: Intended Audience :: Developers Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Classifier: Topic :: Software
 Development Requires-Python: >=3.9 Description-Content-Type: text/markdown
 License-File: LICENSE.md Requires-Dist: colorama==0.4.6 Requires-Dist:
-pytest==7.4.4
+setuptools==69.5.1
                             _[_G_r_e_y_T_e_a_m_T_o_o_l_b_o_x_ _l_o_g_o_]
                     _[_G_i_t_h_u_b_ _B_u_i_l_d_ _S_t_a_t_u_s_]_[_L_i_c_e_n_s_e_]_[_C_r_e_a_t_e_d_]
                   _[_R_e_l_e_a_s_e_]_[_R_e_l_e_a_s_e_d_]_[_C_o_m_m_i_t_s_ _s_i_n_c_e_ _r_e_l_e_a_s_e_]
   _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_C_o_d_e_%_2_0_o_f_%_2_0_C_o_n_d_u_c_t_-_b_l_u_e_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_]
  _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_C_o_n_t_r_i_b_u_t_i_n_g_-_b_l_u_e_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_]_[_h_t_t_p_s_:_/_/
   _i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_R_e_p_o_r_t_%_2_0_S_e_c_u_r_i_t_y_%_2_0_C_o_n_c_e_r_n_-_b_l_u_e_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_]
      _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_G_e_t_%_2_0_S_u_p_p_o_r_t_-_b_l_u_e_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_]
```

### Comparing `baseline_package-0.0.1rc1/setup.cfg` & `baseline_package-0.0.1rc2/setup.cfg`

 * *Files identical despite different names*

### Comparing `baseline_package-0.0.1rc1/setup.py` & `baseline_package-0.0.1rc2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     required: list[str] = f.read().splitlines()
 
 with open("README.md", 'r', encoding='UTF-8') as f:
     long_description: str = f.read()
 
 setup(
     name='baseline-package',
-    version='0.0.1rc1',
+    version='0.0.1rc2',
     packages=find_packages(),
     entry_points={
         'console_scripts': [
             'baseline-package=baseline_package.main:main',
         ],
     },
     author='Wolf Software',
```

