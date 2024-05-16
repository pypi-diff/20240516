# Comparing `tmp/sitesyncro-0.9.4.tar.gz` & `tmp/sitesyncro-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sitesyncro-0.9.4.tar", last modified: Sat May  4 20:50:15 2024, max compression
+gzip compressed data, was "sitesyncro-0.9.5.tar", last modified: Thu May 16 12:15:58 2024, max compression
```

## Comparing `sitesyncro-0.9.4.tar` & `sitesyncro-0.9.5.tar`

### file list

```diff
@@ -1,29 +1,35 @@
-drwxrwxrwx   0        0        0        0 2024-05-04 20:50:15.609008 sitesyncro-0.9.4/
--rw-rw-rw-   0        0        0    35821 2022-11-10 14:20:31.000000 sitesyncro-0.9.4/LICENSE
--rw-rw-rw-   0        0        0    11296 2024-05-04 20:50:15.609008 sitesyncro-0.9.4/PKG-INFO
--rw-rw-rw-   0        0        0    10362 2024-05-02 21:07:04.000000 sitesyncro-0.9.4/README.md
--rw-rw-rw-   0        0        0       42 2024-05-04 20:50:15.609008 sitesyncro-0.9.4/setup.cfg
--rw-rw-rw-   0        0        0     1712 2024-05-03 18:25:42.000000 sitesyncro-0.9.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-04 20:50:15.418664 sitesyncro-0.9.4/src/
-drwxrwxrwx   0        0        0        0 2024-05-04 20:50:15.468764 sitesyncro-0.9.4/src/sitesyncro/
--rw-rw-rw-   0        0        0    39742 2024-05-04 15:15:10.000000 sitesyncro-0.9.4/src/sitesyncro/Model.py
--rw-rw-rw-   0        0        0    19654 2024-05-02 20:25:50.000000 sitesyncro-0.9.4/src/sitesyncro/Sample.py
--rw-rw-rw-   0        0        0      201 2024-05-03 18:25:30.000000 sitesyncro-0.9.4/src/sitesyncro/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-04 20:50:15.588676 sitesyncro-0.9.4/src/sitesyncro/utils/
--rw-rw-rw-   0        0        0        0 2024-03-20 16:40:04.000000 sitesyncro-0.9.4/src/sitesyncro/utils/__init__.py
--rw-rw-rw-   0        0        0    16964 2024-05-04 12:34:57.000000 sitesyncro-0.9.4/src/sitesyncro/utils/fnc_cluster.py
--rw-rw-rw-   0        0        0     2425 2024-05-02 14:21:12.000000 sitesyncro-0.9.4/src/sitesyncro/utils/fnc_data.py
--rw-rw-rw-   0        0        0     8495 2024-05-02 17:55:24.000000 sitesyncro-0.9.4/src/sitesyncro/utils/fnc_load.py
--rw-rw-rw-   0        0        0     3648 2024-05-04 16:21:26.000000 sitesyncro-0.9.4/src/sitesyncro/utils/fnc_mp.py
--rw-rw-rw-   0        0        0    11396 2024-05-02 14:33:18.000000 sitesyncro-0.9.4/src/sitesyncro/utils/fnc_oxcal.py
--rw-rw-rw-   0        0        0    13621 2024-05-02 17:55:24.000000 sitesyncro-0.9.4/src/sitesyncro/utils/fnc_phase.py
--rw-rw-rw-   0        0        0     5882 2024-05-02 17:55:24.000000 sitesyncro-0.9.4/src/sitesyncro/utils/fnc_plot.py
--rw-rw-rw-   0        0        0     2572 2024-05-02 14:41:27.000000 sitesyncro-0.9.4/src/sitesyncro/utils/fnc_radiocarbon.py
--rw-rw-rw-   0        0        0     8520 2024-05-04 12:47:58.000000 sitesyncro-0.9.4/src/sitesyncro/utils/fnc_simulate.py
--rw-rw-rw-   0        0        0     7720 2024-05-04 12:22:34.000000 sitesyncro-0.9.4/src/sitesyncro/utils/fnc_stat.py
-drwxrwxrwx   0        0        0        0 2024-05-04 20:50:15.598782 sitesyncro-0.9.4/src/sitesyncro.egg-info/
--rw-rw-rw-   0        0        0    11296 2024-05-04 20:50:15.000000 sitesyncro-0.9.4/src/sitesyncro.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      668 2024-05-04 20:50:15.000000 sitesyncro-0.9.4/src/sitesyncro.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-04 20:50:15.000000 sitesyncro-0.9.4/src/sitesyncro.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      133 2024-05-04 20:50:15.000000 sitesyncro-0.9.4/src/sitesyncro.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-04 20:50:15.000000 sitesyncro-0.9.4/src/sitesyncro.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-16 12:15:58.449489 sitesyncro-0.9.5/
+-rw-rw-rw-   0        0        0    35821 2022-11-10 14:20:31.000000 sitesyncro-0.9.5/LICENSE
+-rw-rw-rw-   0        0        0    11779 2024-05-16 12:15:58.433860 sitesyncro-0.9.5/PKG-INFO
+-rw-rw-rw-   0        0        0    10770 2024-05-15 15:34:33.000000 sitesyncro-0.9.5/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-16 12:15:58.449489 sitesyncro-0.9.5/setup.cfg
+-rw-rw-rw-   0        0        0     1968 2024-05-15 06:17:47.000000 sitesyncro-0.9.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 12:15:58.396111 sitesyncro-0.9.5/src/
+drwxrwxrwx   0        0        0        0 2024-05-16 12:15:58.411747 sitesyncro-0.9.5/src/sitesyncro/
+-rw-rw-rw-   0        0        0    38904 2024-05-16 11:41:57.000000 sitesyncro-0.9.5/src/sitesyncro/Model.py
+-rw-rw-rw-   0        0        0    19732 2024-05-15 14:36:11.000000 sitesyncro-0.9.5/src/sitesyncro/Sample.py
+-rw-rw-rw-   0        0        0      202 2024-05-15 08:39:18.000000 sitesyncro-0.9.5/src/sitesyncro/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-16 12:15:58.427354 sitesyncro-0.9.5/src/sitesyncro/mhelpers/
+-rw-rw-rw-   0        0        0    11338 2024-05-16 11:07:38.000000 sitesyncro-0.9.5/src/sitesyncro/mhelpers/MCluster.py
+-rw-rw-rw-   0        0        0     1808 2024-05-16 09:19:33.000000 sitesyncro-0.9.5/src/sitesyncro/mhelpers/MOxCal.py
+-rw-rw-rw-   0        0        0    12885 2024-05-16 11:02:34.000000 sitesyncro-0.9.5/src/sitesyncro/mhelpers/MPhasing.py
+-rw-rw-rw-   0        0        0     6286 2024-05-16 10:24:18.000000 sitesyncro-0.9.5/src/sitesyncro/mhelpers/MPlot.py
+-rw-rw-rw-   0        0        0     3909 2024-05-16 09:31:19.000000 sitesyncro-0.9.5/src/sitesyncro/mhelpers/MRandomization.py
+-rw-rw-rw-   0        0        0        0 2024-03-20 16:40:04.000000 sitesyncro-0.9.5/src/sitesyncro/mhelpers/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-16 12:15:58.433860 sitesyncro-0.9.5/src/sitesyncro/utils/
+-rw-rw-rw-   0        0        0        0 2024-03-20 16:40:04.000000 sitesyncro-0.9.5/src/sitesyncro/utils/__init__.py
+-rw-rw-rw-   0        0        0     5766 2024-05-16 10:31:01.000000 sitesyncro-0.9.5/src/sitesyncro/utils/fnc_cluster.py
+-rw-rw-rw-   0        0        0     2425 2024-05-02 14:21:12.000000 sitesyncro-0.9.5/src/sitesyncro/utils/fnc_data.py
+-rw-rw-rw-   0        0        0     8268 2024-05-16 10:50:52.000000 sitesyncro-0.9.5/src/sitesyncro/utils/fnc_load.py
+-rw-rw-rw-   0        0        0     3689 2024-05-04 21:29:14.000000 sitesyncro-0.9.5/src/sitesyncro/utils/fnc_mp.py
+-rw-rw-rw-   0        0        0     9981 2024-05-16 09:14:45.000000 sitesyncro-0.9.5/src/sitesyncro/utils/fnc_oxcal.py
+-rw-rw-rw-   0        0        0     5593 2024-05-16 10:35:51.000000 sitesyncro-0.9.5/src/sitesyncro/utils/fnc_phase.py
+-rw-rw-rw-   0        0        0     2572 2024-05-02 14:41:27.000000 sitesyncro-0.9.5/src/sitesyncro/utils/fnc_radiocarbon.py
+-rw-rw-rw-   0        0        0     5107 2024-05-16 09:27:30.000000 sitesyncro-0.9.5/src/sitesyncro/utils/fnc_simulate.py
+-rw-rw-rw-   0        0        0     7720 2024-05-04 12:22:34.000000 sitesyncro-0.9.5/src/sitesyncro/utils/fnc_stat.py
+drwxrwxrwx   0        0        0        0 2024-05-16 12:15:58.433860 sitesyncro-0.9.5/src/sitesyncro.egg-info/
+-rw-rw-rw-   0        0        0    11779 2024-05-16 12:15:58.000000 sitesyncro-0.9.5/src/sitesyncro.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      852 2024-05-16 12:15:58.000000 sitesyncro-0.9.5/src/sitesyncro.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 12:15:58.000000 sitesyncro-0.9.5/src/sitesyncro.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      176 2024-05-16 12:15:58.000000 sitesyncro-0.9.5/src/sitesyncro.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-16 12:15:58.000000 sitesyncro-0.9.5/src/sitesyncro.egg-info/top_level.txt
```

### Comparing `sitesyncro-0.9.4/LICENSE` & `sitesyncro-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sitesyncro-0.9.4/PKG-INFO` & `sitesyncro-0.9.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sitesyncro
-Version: 0.9.4
+Version: 0.9.5
 Summary: SiteSyncro - Site-specific chronological modeling and synchronization
 Home-page: https://github.com/demjanp/SiteSyncro
 Author: Peter Demjan
 Author-email: peter.demjan@gmail.com
 Keywords: archaeology,radiocarbon,chronology,stratigraphy
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
@@ -16,22 +16,27 @@
 License-File: LICENSE
 Requires-Dist: numpy<2,>=1.26.4
 Requires-Dist: scipy<2,>=1.13.0
 Requires-Dist: matplotlib<4,>=3.8.4
 Requires-Dist: scikit-learn<2,>=1.4.2
 Requires-Dist: tqdm<5,>=4.66.0
 Requires-Dist: requests<3,>=2.31.0
-Requires-Dist: networkx<4,>=3.3.0
+Requires-Dist: networkx<4,>=2.8.0
+Requires-Dist: sphinx<7.4,>=7.3.7
+Requires-Dist: myst-parser<3.1,>=3.0.1
 
 # SiteSyncro
 Site-specific chronological modeling and synchronization
 
 Created on 10.4.2024
 
-<details>
+Project homepage: [https://github.com/demjanp/SiteSyncro](https://github.com/demjanp/SiteSyncro)
+
+Documentation: [https://sitesyncro.readthedocs.io](https://sitesyncro.readthedocs.io)
+
 <summary>Table of Contents</summary>
 
 1. [About SiteSyncro](#about)
 2. [Installation](#installation)
 3. [Usage](#usage)
    * [Input File Format](#input_file)
    * [Model Class](#model_class)
@@ -39,16 +44,14 @@
 4. [Developer Notes](#developer)
 	* [Preparing the Virtual Environment](#venv)
 	* [Building a Windows Executable](#build)
 5. [Contact](#contact)
 6. [Acknowledgements](#acknowledgements)
 7. [License](#license)
 
-</details>
-
 ## About SiteSyncro <a name="about"></a>
 SiteSyncro is a Python-based tool designed for site-specific chronological modeling and synchronization based on radiocarbon dates from stratigraphically and/or spatially linked archaeological contexts. It uses the [OxCal](https://c14.arch.ox.ac.uk/oxcal.html) program for bayesian modelling and a method of temporal clustering of the modelled C-14 dates to determine whether they represent separate events, or phases in time.
  
 The input data represent radiocarbon dates and their stratigraphic relations. Here is a brief overview of the processing workflow:
 1. Bayesian modeling of distributions of the C-14 dates based on stratigraphic constrains using the [OxCal](https://c14.arch.ox.ac.uk/oxcal.html) program.
 2. Randomization testing of the null hypothesis that the observed C-14 dates represent a normal / uniform distribution
 3. Temporal clustering of the modelled C-14 dates. All possible clusterings are produced and tested for randomness. The optimal number of clusters is selected for further analyses.
@@ -72,15 +75,15 @@
 See [Model Class](#model_class) on usage tips.
 
 SiteSyncro requires [OxCal](https://c14.arch.ox.ac.uk/oxcal.html) to be installed in its default location. The program is not included in the SiteSyncro package and must be installed separately. OxCal should be downloaded and installed automatically when running SiteSyncro for the first time. You can also download OxCal manually from the [OxCal website](https://c14.arch.ox.ac.uk/OxCalDistribution.zip) and unzip it in the SiteSyncro folder.
 
 ## Usage <a name="usage"></a>
 
 ### Running the Script
-To use SiteSyncro, you need to run the [process.py](bin/process.py) or `sitesyncro.exe` script. This script accepts several command-line arguments. Here's a basic example of how to run the script:
+To use SiteSyncro, you need to run the [process.py](https://github.com/demjanp/SiteSyncro/blob/main/bin/process.py) or `sitesyncro.exe` script. This script accepts several command-line arguments. Here's a basic example of how to run the script:
 ```
 python process.py -input data_sample.csv
 ```
 or
 ```
 sitesyncro.exe -input data_sample.csv
 ```
@@ -113,21 +116,21 @@
 ### Input File Format <a name="input_file"></a>
 The input file name must be a semicolon-separated CSV file with the following 10 columns: 
 1. Sample: Sample ID (required, unique identifier)
 2. Context: Context ID (required)
 3. Excavation Area: Excavation area ID (required)
 4. C-14 Age: Radiocarbon age in years BP (required)
 5. Uncertainty: Uncertainty of the radiocarbon age in C-14 years (required)
-6. Phase: Phase of the sample (lower = older) (optional)
+6. Excavation Area Phase: Phase of the sample (format: '1' or '1a' or '1-2' or '1a-b' or '1a-2b', higher = earlier (older) phase) (optional)
 7. Earlier-Than: List of contexts that the sample is earlier (older) than (optional)
 8. Long-Lived: Flag indicating whether the sample is long-lived (e.g. old wood)(required, 1 or 0)
 9. Redeposited: Flag indicating whether the sample could be redeposited from a different context (required, 1 or 0)
 10. Outlier: Flag indicating whether the sample is an outlier and should not be used for modeling (required, 1 or 0)
 
-See [data_sample.csv](data_sample.csv) for an example of the input file format.
+See [data_sample.csv](https://github.com/demjanp/SiteSyncro/blob/main/data_sample.csv) for an example of the input file format.
 
 ### Model Class <a name="model_class"></a>
 All functions regarding modeling are encapsulated in the `Model` class. Here is a basic example of how to use it:
 
 ```python
 from sitesyncro import Model
 
@@ -166,15 +169,15 @@
 
 ```python
 from sitesyncro import Sample
 
 if __name__ == '__main__':
 	
 	# Initialize the Sample object
-	sample = Sample('Sample1', 1000, 50, phase = 1, earlier_than = ['Sample2'], long_lived = 1)
+	sample = Sample('Sample1', 1000, 50, excavation_area_phase = 1, earlier_than = ['Sample2'], long_lived = 1)
 	
 	# Print the sample data
 	print(sample)
 ```
 
 See [Sample Class](https://sitesyncro.readthedocs.io/en/latest/sample.html) documentation for more information.
 
@@ -237,8 +240,8 @@
 * [Requests](https://requests.readthedocs.io/)
 * [Scikit-learn](https://scikit-learn.org/)
 * [SciPy](https://scipy.org/)
 * [tqdm](https://tqdm.github.io/)
 
 ## License <a name="license"></a>
 
-This code is licensed under the [GNU GENERAL PUBLIC LICENSE](https://www.gnu.org/licenses/gpl-3.0.en.html) - see the [LICENSE](LICENSE) file for details
+This code is licensed under the [GNU GENERAL PUBLIC LICENSE](https://www.gnu.org/licenses/gpl-3.0.en.html) - see the [LICENSE](https://github.com/demjanp/SiteSyncro/blob/main/LICENSE) file for details
```

### Comparing `sitesyncro-0.9.4/README.md` & `sitesyncro-0.9.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 # SiteSyncro
 Site-specific chronological modeling and synchronization
 
 Created on 10.4.2024
 
-<details>
+Project homepage: [https://github.com/demjanp/SiteSyncro](https://github.com/demjanp/SiteSyncro)
+
+Documentation: [https://sitesyncro.readthedocs.io](https://sitesyncro.readthedocs.io)
+
 <summary>Table of Contents</summary>
 
 1. [About SiteSyncro](#about)
 2. [Installation](#installation)
 3. [Usage](#usage)
    * [Input File Format](#input_file)
    * [Model Class](#model_class)
@@ -15,16 +18,14 @@
 4. [Developer Notes](#developer)
 	* [Preparing the Virtual Environment](#venv)
 	* [Building a Windows Executable](#build)
 5. [Contact](#contact)
 6. [Acknowledgements](#acknowledgements)
 7. [License](#license)
 
-</details>
-
 ## About SiteSyncro <a name="about"></a>
 SiteSyncro is a Python-based tool designed for site-specific chronological modeling and synchronization based on radiocarbon dates from stratigraphically and/or spatially linked archaeological contexts. It uses the [OxCal](https://c14.arch.ox.ac.uk/oxcal.html) program for bayesian modelling and a method of temporal clustering of the modelled C-14 dates to determine whether they represent separate events, or phases in time.
  
 The input data represent radiocarbon dates and their stratigraphic relations. Here is a brief overview of the processing workflow:
 1. Bayesian modeling of distributions of the C-14 dates based on stratigraphic constrains using the [OxCal](https://c14.arch.ox.ac.uk/oxcal.html) program.
 2. Randomization testing of the null hypothesis that the observed C-14 dates represent a normal / uniform distribution
 3. Temporal clustering of the modelled C-14 dates. All possible clusterings are produced and tested for randomness. The optimal number of clusters is selected for further analyses.
@@ -48,15 +49,15 @@
 See [Model Class](#model_class) on usage tips.
 
 SiteSyncro requires [OxCal](https://c14.arch.ox.ac.uk/oxcal.html) to be installed in its default location. The program is not included in the SiteSyncro package and must be installed separately. OxCal should be downloaded and installed automatically when running SiteSyncro for the first time. You can also download OxCal manually from the [OxCal website](https://c14.arch.ox.ac.uk/OxCalDistribution.zip) and unzip it in the SiteSyncro folder.
 
 ## Usage <a name="usage"></a>
 
 ### Running the Script
-To use SiteSyncro, you need to run the [process.py](bin/process.py) or `sitesyncro.exe` script. This script accepts several command-line arguments. Here's a basic example of how to run the script:
+To use SiteSyncro, you need to run the [process.py](https://github.com/demjanp/SiteSyncro/blob/main/bin/process.py) or `sitesyncro.exe` script. This script accepts several command-line arguments. Here's a basic example of how to run the script:
 ```
 python process.py -input data_sample.csv
 ```
 or
 ```
 sitesyncro.exe -input data_sample.csv
 ```
@@ -89,21 +90,21 @@
 ### Input File Format <a name="input_file"></a>
 The input file name must be a semicolon-separated CSV file with the following 10 columns: 
 1. Sample: Sample ID (required, unique identifier)
 2. Context: Context ID (required)
 3. Excavation Area: Excavation area ID (required)
 4. C-14 Age: Radiocarbon age in years BP (required)
 5. Uncertainty: Uncertainty of the radiocarbon age in C-14 years (required)
-6. Phase: Phase of the sample (lower = older) (optional)
+6. Excavation Area Phase: Phase of the sample (format: '1' or '1a' or '1-2' or '1a-b' or '1a-2b', higher = earlier (older) phase) (optional)
 7. Earlier-Than: List of contexts that the sample is earlier (older) than (optional)
 8. Long-Lived: Flag indicating whether the sample is long-lived (e.g. old wood)(required, 1 or 0)
 9. Redeposited: Flag indicating whether the sample could be redeposited from a different context (required, 1 or 0)
 10. Outlier: Flag indicating whether the sample is an outlier and should not be used for modeling (required, 1 or 0)
 
-See [data_sample.csv](data_sample.csv) for an example of the input file format.
+See [data_sample.csv](https://github.com/demjanp/SiteSyncro/blob/main/data_sample.csv) for an example of the input file format.
 
 ### Model Class <a name="model_class"></a>
 All functions regarding modeling are encapsulated in the `Model` class. Here is a basic example of how to use it:
 
 ```python
 from sitesyncro import Model
 
@@ -142,15 +143,15 @@
 
 ```python
 from sitesyncro import Sample
 
 if __name__ == '__main__':
 	
 	# Initialize the Sample object
-	sample = Sample('Sample1', 1000, 50, phase = 1, earlier_than = ['Sample2'], long_lived = 1)
+	sample = Sample('Sample1', 1000, 50, excavation_area_phase = 1, earlier_than = ['Sample2'], long_lived = 1)
 	
 	# Print the sample data
 	print(sample)
 ```
 
 See [Sample Class](https://sitesyncro.readthedocs.io/en/latest/sample.html) documentation for more information.
 
@@ -213,8 +214,8 @@
 * [Requests](https://requests.readthedocs.io/)
 * [Scikit-learn](https://scikit-learn.org/)
 * [SciPy](https://scipy.org/)
 * [tqdm](https://tqdm.github.io/)
 
 ## License <a name="license"></a>
 
-This code is licensed under the [GNU GENERAL PUBLIC LICENSE](https://www.gnu.org/licenses/gpl-3.0.en.html) - see the [LICENSE](LICENSE) file for details
+This code is licensed under the [GNU GENERAL PUBLIC LICENSE](https://www.gnu.org/licenses/gpl-3.0.en.html) - see the [LICENSE](https://github.com/demjanp/SiteSyncro/blob/main/LICENSE) file for details
```

### Comparing `sitesyncro-0.9.4/src/sitesyncro/Model.py` & `sitesyncro-0.9.5/src/sitesyncro/Model.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,23 +5,25 @@
 import subprocess
 from collections import defaultdict
 from typing import List, Dict, Any
 
 import numpy as np
 
 from sitesyncro.Sample import Sample
-from sitesyncro.utils.fnc_cluster import (proc_clustering)
+
+from sitesyncro.mhelpers.MPhasing import MPhasing
+from sitesyncro.mhelpers.MOxCal import MOxCal
+from sitesyncro.mhelpers.MRandomization import MRandomization
+from sitesyncro.mhelpers.MCluster import MCluster
+from sitesyncro.mhelpers.MPlot import MPlot
+
 from sitesyncro.utils.fnc_data import (dict_keys_to_int, dict_np_to_list)
 from sitesyncro.utils.fnc_load import (load_data)
-from sitesyncro.utils.fnc_oxcal import (download_oxcal, gen_oxcal_model, load_oxcal_data, get_distributions)
-from sitesyncro.utils.fnc_phase import (create_earlier_than_matrix, get_groups_and_phases, find_dating_outliers,
-										update_earlier_than_by_clustering, update_earlier_than_by_dating)
-from sitesyncro.utils.fnc_plot import (plot_randomized, plot_clusters, save_results_csv, save_outliers)
+from sitesyncro.utils.fnc_oxcal import (download_oxcal, load_oxcal_data, get_distributions)
 from sitesyncro.utils.fnc_radiocarbon import (get_curve)
-from sitesyncro.utils.fnc_simulate import (test_distributions)
 
 
 class Model(object):
 	"""
 	A class representing a Bayesian model of dated samples interconnected by stratigraphic relationships.
 
 	:param directory: Working directory for model data (default is "model").
@@ -34,15 +36,18 @@
 	:type curve_name: str
 
 	:param phase_model: OxCal phase model type. Can be 'sequence', 'contiguous', 'overlapping', or 'none' (default is "sequence").
 	:type phase_model: str
 
 	:param cluster_n: Number of clusters to form (-1 = automatic; default is -1).
 	:type cluster_n: int
-
+	
+	:param cluster_selection: The method used to select the optimal number of clusters. Can be 'silhouette' or 'mcst' (default is 'silhouette').
+	:type cluster_selection: str
+	
 	:param min_years_per_cluster: The minimum number of years per cluster.
 	:type min_years_per_cluster: int
 
 	:param uniform: Flag indicating whether to use uniform randomization (default is False).
 	:type uniform: bool
 
 	:param p_value: The P-value for statistical tests (default is 0.05).
@@ -68,14 +73,15 @@
 		
 		defaults = dict(
 			directory='model',
 			samples=[],
 			curve_name='intcal20.14c',
 			phase_model='sequence',
 			cluster_n=-1,
+			cluster_selection='silhouette',
 			min_years_per_cluster=25,
 			uniform=False,
 			p_value=0.05,
 			uncertainty_base=15,
 			npass=100,
 			convergence=0.99,
 			oxcal_url='https://c14.arch.ox.ac.uk/OxCalDistribution.zip',
@@ -117,22 +123,29 @@
 		# Convert samples to dict
 		kwargs['samples'] = dict([(sample.name, sample) for sample in kwargs['samples']])
 		
 		self._data.update(kwargs)
 		
 		# Create model directory if needed
 		self._data['directory'] = self._create_dir(self.directory, overwrite)
+		
+		self._mphasing = MPhasing(self)
+		self._moxcal = MOxCal(self)
+		self._mrandomization = MRandomization(self)
+		self._mcluster = MCluster(self)
+		self._mplot = MPlot(self)
 	
 	def _assigned(self) -> Dict[str, Any]:
 		return dict(
 			directory=None,
 			samples=None,
 			curve_name=None,
 			phase_model=None,
 			cluster_n=None,
+			cluster_selection=None,
 			min_years_per_cluster=None,
 			uniform=None,
 			p_value=None,
 			uncertainty_base=None,
 			npass=None,
 			convergence=None,
 			oxcal_url=None,
@@ -191,28 +204,19 @@
 	# Assigned properties
 	
 	@property
 	def directory(self) -> str:
 		"""
 		The directory where the model data is stored.
 		
-		Returns:
-			str: The directory path as a string.
-		"""
-		return self._data['directory']
-	@property
-	def directory(self) -> str:
-		"""
-		Represents the directory where the model data is stored.
-
 		:return: The directory where the model data is stored.
 		:rtype: str
 		"""
-		
 		return self._data['directory']
+	
 	@property
 	def samples(self) -> Dict[str, Sample]:
 		"""
 		A dictionary of samples associated with the model.
 		
 		:return: A dictionary where the keys are the sample names and the values are Sample objects.
 		:rtype: Dict[str, Sample]
@@ -248,14 +252,24 @@
 		
 		:return: The number of clusters to form.
 		:rtype: int
 		"""
 		return self._data['cluster_n']
 	
 	@property
+	def cluster_selection(self) -> str:
+		"""
+		The method used to select the optimal number of clusters.
+		
+		:return: The method used to select the optimal number of clusters. Can be 'silhouette' or 'mcst'.
+		:rtype: str
+		"""
+		return self._data['cluster_selection']
+	
+	@property
 	def min_years_per_cluster(self) -> int:
 		"""
 		The minimum number of years per cluster.
 		
 		:return: The minimum number of years per cluster.
 		:rtype: int
 		"""
@@ -320,30 +334,30 @@
 		:rtype: str
 		"""
 		return self._data['oxcal_url']
 	
 	# Calculated properties
 	
 	@property
-	def years(self) -> np.ndarray:
+	def years(self) -> np.ndarray or None:
 		"""
 		Calendar years BP corresponding to the probability distributions.
 
 		:return: An array of calendar years.
 		:rtype: np.ndarray
 		"""
 		if self._data['years'] is None:
 			if self.curve is not None:
 				self._data['years'] = self.curve[:, 0]
 			else:
 				return None
 		return self._data['years'].copy()
 	
 	@property
-	def curve(self) -> np.ndarray:
+	def curve(self) -> np.ndarray or None:
 		"""
 		Radiocarbon calibration curve.
 
 		2D array containing the calibration curve data. Each row represents a calendar year BP, C-14 year, and uncertainty.
 		
 		:return: An array of the calibration curve.
 		:rtype: np.ndarray
@@ -630,15 +644,15 @@
 		:return: None
 		"""
 		
 		def _from_arguments(name: str, age: float, uncertainty: float,
 							date_type: str = 'R', long_lived: bool = False, redeposited: bool = False,
 							outlier: bool = False, context: bool = None,
 							area: str = None,
-							excavation_area_phase: float = None,
+							excavation_area_phase: str = None,
 							earlier_than: List[str] = [],
 							):
 			self._data['samples'][name] = Sample(
 				name, age, uncertainty, date_type, long_lived, redeposited, outlier,
 				context, area, excavation_area_phase, earlier_than, self.curve
 			)
 			self._data['samples'][name].calibrate(self.curve)
@@ -705,14 +719,15 @@
 		
 		model = Model(
 			directory = directory,
 			samples = [self.samples[name].copy() for name in self.samples],
 			curve_name = self.curve_name,
 			phase_model = self.phase_model,
 			cluster_n = self.cluster_n,
+			cluster_selection = self.cluster_selection,
 			min_years_per_cluster = self.min_years_per_cluster,
 			uniform = self.uniform,
 			p_value = self.p_value,
 			uncertainty_base = self.uncertainty_base,
 			npass = self.npass,
 			convergence = self.convergence,
 			oxcal_url = self.oxcal_url
@@ -780,45 +795,39 @@
 		self._data = data
 		self._data['directory'] = directory
 		return True
 	
 	def import_csv(self, fname: str) -> None:
 		"""
 		Loads sample data from a CSV file.
-
+		
 		The file should be in the following format:
 		- Each line represents a data record.
 		- Data fields are separated by semicolons.
 		- The first line is a header and is skipped.
-		- Each line should have 10 fields: Sample, Context, Area, C14 Age, Uncertainty, Phase, Earlier-Than, Long-Lived, Redeposited, Outlier.
-		- The fields are processed as follows:
-			- Sample, Context, and Area are stripped of leading and trailing whitespace.
-			- C14 Age and Uncertainty are converted to floats.
-			- Phase is converted to a float if possible, otherwise it is set to None.
-			- Earlier-Than is split on commas and stripped of leading and trailing whitespace. If it is empty, it is set to an empty list.
-			- Long-Lived, Redeposited, and Outlier are converted to integers and then to booleans.
-
+		- Each line should have 10 fields: Sample, Context, Area, C14 Age, Uncertainty, Excavation Area Phase, Earlier-Than, Long-Lived, Redeposited, Outlier.
+		
 		:param fname: The file path of the CSV file to be imported.
 		:type fname: str
 		:raises ValueError: If the input file does not exist or is not formatted correctly.
 		:return: None
 		"""
 		
 		# Check if the input file exists
 		if not os.path.isfile(fname):
 			raise ValueError("Input file %s not found" % fname)
 		
-		samples, contexts, context_area, long_lived, redeposited, outlier, r_dates, context_phase, earlier_than = load_data(
+		samples, contexts, context_area, long_lived, redeposited, outlier, r_dates, context_eap, earlier_than = load_data(
 			fname)
 		self._data['samples'] = {}
 		for name in samples:
 			age, uncertainty = r_dates[name]
 			self.add_sample(
 				name, age, uncertainty, 'R', long_lived[name], redeposited[name], outlier[name], contexts[name],
-				context_area[contexts[name]], context_phase[contexts[name]], earlier_than[name]
+				context_area[contexts[name]], context_eap[contexts[name]], earlier_than[name]
 			)
 	
 	def plot_randomized(self, fname: str = None, show: bool = False) -> str:
 		"""
 		Plots the results of the randomization test.
 
 		The plot can either be saved to a file or displayed.
@@ -839,15 +848,15 @@
 			print("\nNo randomization data to plot")
 			return None
 		
 		# Determine the file path for the plot
 		if fname is None:
 			fname = os.path.join(self.directory, "randomized.pdf")
 		
-		plot_randomized(self, fname, show)
+		self._mplot.plot_randomized(fname, show)
 		return fname
 	
 	def plot_clusters(self, fname: str = None, show: bool = False) -> str:
 		"""
 		Plots the clustering results.
 
 		The plot can either be saved to a file or displayed.
@@ -865,15 +874,15 @@
 			return None
 		
 		# Determine the file path for the plot
 		if fname is None:
 			fname = os.path.join(self.directory, "silhouette.pdf")
 		
 		# Plot the clustering data
-		plot_clusters(self, fname, show)
+		self._mplot.plot_clusters(fname, show)
 		return fname
 	
 	def save_csv(self, fcsv: str = None) -> str:
 		"""
 		Saves the results to a CSV file.
 
 		:param fcsv: The file path for the CSV file. If None, a default file name and path are used. Defaults to None.
@@ -888,15 +897,15 @@
 			return None
 		
 		# Determine the file path for the CSV file
 		if fcsv is None:
 			fcsv = os.path.join(self.directory, "results.csv")
 		
 		# Save the results to the CSV file
-		save_results_csv(self, fcsv)
+		self._mplot.save_results_csv(fcsv)
 		return fcsv
 	
 	def save_outliers(self, fname: str = None) -> str:
 		"""
 		Saves a list of outliers to a text file.
 
 		:param fname: The file name to save the outliers to. If None, a default file name is used. Defaults to None.
@@ -904,15 +913,15 @@
 		:return: The file name the outliers were saved to.
 		:rtype: str
 		"""
 		
 		if fname is None:
 			fname = os.path.join(self.directory, "outliers.txt")
 		
-		save_outliers(self, fname)
+		self._mplot.save_outliers(fname)
 		return fname
 	
 	def to_oxcal(self, fname: str = None) -> str:
 		"""
 		Exports the model to an OxCal file.
 
 		Generates an OxCal file from the current model. The OxCal file can be used for further analysis in the OxCal software.
@@ -928,16 +937,16 @@
 		if not self.has_data:
 			print("\nNo data available")
 			return None
 		
 		if fname is None:
 			fname = os.path.join(self.directory, "model.oxcal")
 		
-		txt = gen_oxcal_model(self)
-		with open(fname, "w") as file:
+		txt = self._moxcal.gen_oxcal_model()
+		with open(fname, "w", encoding="utf-8") as file:
 			file.write(txt)
 		return fname
 	
 	def load_oxcal_data(self) -> None:
 		"""
 		Loads the OxCal data associated with the model.
 
@@ -991,15 +1000,15 @@
 			reset_assigned: {parameter: [old value, new value], ...}; parameters and their values that have been updated;
 			reset_calculated: {attribute, ...}; calculated attributes that have been reset
 		:rtype: (Dict[str, List], set)
 		"""
 		
 		assigned_full = ['samples', 'curve_name', 'phase_model']
 		assigned_randomization = ['uniform', 'p_value', 'uncertainty_base', 'npass', 'convergence']
-		assigned_clustering = ['cluster_n', 'min_years_per_cluster']
+		assigned_clustering = ['cluster_n', 'cluster_selection', 'min_years_per_cluster']
 		
 		def _get_n_samples(value):
 			if isinstance(value, dict):
 				return len(value)
 			return 0
 		
 		reset_assigned = {}
@@ -1067,50 +1076,28 @@
 		:type by_clusters: bool, optional
 		:param by_dates: If True, update the phasing by comparing sample dates. Defaults to False.
 		:type by_dates: bool, optional
 		:return: True if phasing has changed, False otherwise.
 		:rtype: bool
 		"""
 		
-		earlier_than, samples = create_earlier_than_matrix(self)
-		if by_clusters and self.is_clustered:
-			earlier_than = update_earlier_than_by_clustering(self, earlier_than, samples)
-		
-		if by_dates and self.is_modeled:
-			earlier_than = update_earlier_than_by_dating(self, earlier_than, samples)
-		
-		groups_phases = get_groups_and_phases(earlier_than, samples)
-		# groups_phases = {sample: [group, phase], ...}
-		for name in self.samples:
-			if name in groups_phases:
-				group, phase = groups_phases[name]
-				self.samples[name].set_group(group)
-				self.samples[name].set_phase(phase)
-			else:
-				self.samples[name].set_group(None)
-				self.samples[name].set_phase(None)
-		
-		earlier_than_1, samples_1 = create_earlier_than_matrix(self)
-		if not ((earlier_than.shape == earlier_than.shape) and np.allclose(earlier_than, earlier_than_1) and (
-				samples == samples_1)):
-			return True
-		return False
+		return self._mphasing.process(by_clusters, by_dates)
 	
 	def process_outliers(self) -> None:
 		"""
 		Identifies and marks dating outliers among the samples in the model.
 
 		Finds dating outliers among the samples which need to be removed for the model to be valid.
 		The outliers are identified based on conflicts between their dating ranges and stratigraphic relationships with other samples.
 		The identified outliers can be retrieved via the attributes Model.outliers and Model.outlier_candidates.
 
 		:return: None
 		"""
 		
-		outliers, self._data['outlier_candidates'] = find_dating_outliers(self)
+		outliers, self._data['outlier_candidates'] = self._mphasing.find_dating_outliers()
 		for name in outliers:
 			self.samples[name].set_outlier(True)
 	
 	def process_dates(self) -> None:
 		"""
 		Calculates the posterior probabilities of sample dates based on phasing using Bayesian modeling in OxCal.
 
@@ -1141,15 +1128,15 @@
 		:type max_cpus: int, optional
 		:param max_queue_size: Maximum queue size for parallel processing. If -1, the queue size is unlimited. Defaults to -1.
 		:type max_queue_size: int, optional
 		:return: None
 		"""
 		
 		self._data['summed'], self._data['random_lower'], self._data['random_upper'], self._data[
-			'random_p'] = test_distributions(self, max_cpus=max_cpus, max_queue_size=max_queue_size)
+			'random_p'] = self._mrandomization.test_distributions(max_cpus=max_cpus, max_queue_size=max_queue_size)
 	
 	def process_clustering(self, max_cpus=-1, max_queue_size=-1) -> None:
 		"""
 		Performs clustering on the sample dates.
 
 		Clusters the sample dates and uses randomization testing to find the optimal clustering solution.
 		
@@ -1157,15 +1144,15 @@
 		:type max_cpus: int, optional
 		:param max_queue_size: Maximum queue size for parallel processing. If -1, the queue size is unlimited. Defaults to -1.
 		:type max_queue_size: int, optional
 		:return: None
 		"""
 		
 		self._data['clusters'], self._data['cluster_means'], self._data['cluster_sils'], self._data['cluster_ps'], \
-			self._data['cluster_opt_n'] = proc_clustering(self, max_cpus=max_cpus, max_queue_size=max_queue_size)
+			self._data['cluster_opt_n'] = self._mcluster.process(max_cpus=max_cpus, max_queue_size=max_queue_size)
 	
 	def process(self, by_clusters: bool = False, by_dates: bool = False, max_cpus: int = -1, max_queue_size: int = -1,
 				save: bool = False) -> None:
 		# Process the complete model
 		# by_clusters: if True, update the phasing by clustering sample dates
 		# by_dates: if True, update the phasing by comparing sample dates
 		"""
@@ -1216,7 +1203,8 @@
 				self.save(zipped=True)
 		if by_clusters:
 			if self.process_phasing(by_clusters=True):
 				print("\nUpdating phasing by clustering\n")
 				self.process_dates()
 				if save:
 					self.save(zipped=True)
+
```

### Comparing `sitesyncro-0.9.4/src/sitesyncro/Sample.py` & `sitesyncro-0.9.5/src/sitesyncro/Sample.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,18 +39,18 @@
 	
 	:param context: Name of the context where sample was found
 	:type context: str, optional
 	
 	:param area: Excavation area
 	:type area: str, optional
 	
-	:param excavation_area_phase: Chronological phase of the context within the excavation area (integer, lower = earlier (older) phase)
-	:type excavation_area_phase: float, optional
+	:param excavation_area_phase: Chronological phase of the context within the excavation area (format: "1" or "1a" or "1-2" or "1a-b" or "1a-2b", higher = earlier (older) phase)
+	:type excavation_area_phase: str, optional
 	
-	:param earlier_than: List of names of samples which are stratigraphically later (younger) than this sample
+	:param earlier_than: List of names of samples which are stratigraphically earlier (older) than this sample
 	:type earlier_than: List[str], optional
 	
 	:param curve: Radiocarbon calibration curve in format `np.array([[calendar year BP, C-14 year, uncertainty], ...])`
 	:type curve: np.ndarray, optional
 	"""
 	
 	def __init__(self, *args, **kwargs):
@@ -60,15 +60,15 @@
 		def _from_arguments(name: str, age: float, uncertainty: float,
 							date_type: str = 'R',
 							long_lived: bool = False,
 							redeposited: bool = False,
 							outlier: bool = False,
 							context: str = None,
 							area: str = None,
-							excavation_area_phase: float = None,
+							excavation_area_phase: str = None,
 							earlier_than: List[str] = [],
 							curve: np.ndarray = None,
 							) -> None:
 			
 			if date_type not in ['R', 'U']:
 				raise Exception("Invalid date type specified: %s (must be 'R' or 'U')" % (date_type))
 			
@@ -220,30 +220,30 @@
 		:return: The name of the excavation area where the sample was found or None if it's not set.
 		:rtype: str or None
 		"""
 		
 		return self._data['area']
 	
 	@property
-	def excavation_area_phase(self) -> float or None:
+	def excavation_area_phase(self) -> str or None:
 		"""
 		The chronological phase of the context within the excavation area.
 		
-		:return: The chronological phase of the context within the excavation area (integer, lower = earlier (older) phase) or None if it's not set.
-		:rtype: float or None
+		:return: The chronological phase of the context within the excavation area (format: "1" or "1a" or "1-2" or "1a-b" or "1a-2b", higher = earlier (older) phase) or None if it's not set.
+		:rtype: str or None
 		"""
 		
 		return self._data['excavation_area_phase']
 	
 	@property
 	def earlier_than(self) -> List[str] or None:
 		"""
-		List of names of samples which are stratigraphically later (younger) than this sample.
+		List of names of samples which are stratigraphically earlier (older) than this sample.
 
-		:return: List of names of samples which are stratigraphically later (younger) than this sample or None if it's not set.
+		:return: List of names of samples which are stratigraphically earlier (older) than this sample or None if it's not set.
 		:rtype: List[str] or None
 		"""
 		
 		if self._data['earlier_than'] is None:
 			return None
 		return copy.copy(self._data['earlier_than'])
```

### Comparing `sitesyncro-0.9.4/src/sitesyncro/utils/fnc_data.py` & `sitesyncro-0.9.5/src/sitesyncro/utils/fnc_data.py`

 * *Files identical despite different names*

### Comparing `sitesyncro-0.9.4/src/sitesyncro/utils/fnc_load.py` & `sitesyncro-0.9.5/src/sitesyncro/utils/fnc_load.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,80 +1,75 @@
 import os
 from collections import defaultdict
 from typing import List, Dict, Any
 
+from sitesyncro.utils.fnc_phase import (eap_to_int)
+
 
 def load_input(fname: str) -> List[Dict[str, Any]]:
 	"""
 	Load input data from a file.
 
 	This function reads a file line by line, parses each line into a dictionary, and appends the dictionary to a list.
 	The file should be in the following format:
 	- Each line represents a data record.
 	- Data fields are separated by semicolons.
 	- The first line is a header and is skipped.
-	- Each line should have 10 fields: Sample, Context, Area, C14 Age, Uncertainty, Phase, Earlier-Than, Long-Lived, Redeposited, Outlier.
-	- The fields are processed as follows:
-		- Sample, Context, and Area are stripped of leading and trailing whitespace.
-		- C14 Age and Uncertainty are converted to floats.
-		- Phase is converted to a float if possible, otherwise it is set to None.
-		- Earlier-Than is split on commas and stripped of leading and trailing whitespace. If it is empty, it is set to an empty list.
-		- Long-Lived, Redeposited, and Outlier are converted to integers and then to booleans.
-
+	- Each line should have 10 fields: Sample, Context, Area, C14 Age, Uncertainty, Excavation Area Phase, Earlier-Than, Long-Lived, Redeposited, Outlier.
+	
 	Parameters:
 	fname (str): The name of the file to load.
 
 	Returns:
 	A list of dictionaries representing the data records in the file.
 
 	Raises:
 	Exception: If a line does not have exactly 10 fields, or if a field cannot be converted to the required type, an exception is raised.
 	"""
 	data = []
-	with open(fname, "r") as file:
+	with open(fname, "r", encoding="utf-8") as file:
 		next(file)  # Skip header
 		for line in file:
 			line = line.strip()
 			if line:
 				elements = line.split(";")
 				if len(elements) != 10:
 					raise Exception(f"Incorrect data format in line: {line}")
-				sample, context, area, age, uncertainty, phase, earlier_than, long_lived, redeposited, outlier = elements
+				elements = [val.strip() for val in elements]
+				sample, context, area, age, uncertainty, eap, earlier_than, long_lived, redeposited, outlier = elements
 				try:
-					age = float(age.strip())
-					uncertainty = float(uncertainty.strip())
-					long_lived = int(long_lived.strip())
-					redeposited = int(redeposited.strip())
-					outlier = int(outlier.strip())
+					age = float(age)
+					uncertainty = float(uncertainty)
+					long_lived = int(long_lived) if long_lived else 0
+					redeposited = int(redeposited) if redeposited else 0
+					outlier = int(outlier) if outlier else 0
 				except ValueError:
 					raise Exception(f"Incorrect data format in line: {line}")
-				phase = phase.strip()
-				try:
-					phase = float(phase)
-				except:
-					phase = None
+				# EAP should be in format "1" or "1a" or "1-2" or "1a-b" or "1a-2b"
+				if not eap:
+					eap = None
+				elif eap_to_int(eap) is None:
+					raise Exception(f"Incorrect EAP format in line: {line}")
+				
 				# split comma-separated values from earlier_than
-				earlier_than = earlier_than.strip()
 				if earlier_than:
 					earlier_than = [val.strip() for val in earlier_than.split(",")]
 				else:
 					earlier_than = []
-				context = context.strip()
 				if not context:
 					context = None
-				area = area.strip()
 				if not area:
 					area = None
 				data.append({
-					"Sample": sample.strip(),
+					"Sample": sample,
 					"Context": context,
 					"Area": area,
 					"C14 Age": age,
 					"Uncertainty": uncertainty,
-					"Phase": phase,
+					"EAP": eap,
 					"Earlier-Than": earlier_than,
 					"Long-Lived": long_lived,
 					"Redeposited": redeposited,
 					"Outlier": outlier,
 				})
 	return data
 
@@ -138,20 +133,22 @@
 def get_c14_dates(data: List[Dict[str, Any]]) -> Dict[str, Any]:
 	r_dates = {}
 	for line in data:
 		r_dates[line["Sample"]] = (line["C14 Age"], line["Uncertainty"])
 	return r_dates
 
 
-def get_context_phase(data: List[Dict[str, Any]]) -> Dict[str, float]:
-	# Create a dictionary of contexts and their phases
-	context_phase = {}
-	for line in data:
-		context_phase[line["Context"]] = line["Phase"]
-	return context_phase
+def get_context_eap(data: List[Dict[str, Any]]) -> Dict[str, str]:
+	# Create a dictionary of contexts and their excavation area phases
+	context_eap = {}
+	for line in data:
+		context = line["Context"]
+		if (context not in context_eap) or (context_eap[context] is None):
+			context_eap[context] = line["EAP"]
+	return context_eap
 
 
 def get_earlier_than_relations(data: List[Dict[str, Any]], context_samples: Dict[str, List[str]]) -> Dict[
 	str, List[str]]:
 	earlier_than_rel = defaultdict(list)
 	for line in data:
 		sample1 = line["Sample"]
@@ -205,43 +202,43 @@
 
 	This function reads a file, processes the data, and returns it in a structured format.
 
 	Parameters:
 	fname (str): The name of the file to load.
 
 	Returns:
-	(samples, contexts, context_area, long_lived, redeposited, outlier, r_dates, context_phase, earlier_than_rel):
+	(samples, contexts, context_area, long_lived, redeposited, outlier, r_dates, context_eap, earlier_than_rel):
 		- samples = [sample, ...]
 		- contexts = {sample: context, ...}
 		- context_area = {context: area, ...}
 		- long_lived = {sample: True/False, ...}
 		- redeposited = {sample: True/False, ...}
 		- outlier = {sample: True/False, ...}
 		- r_dates = {sample: (age, uncertainty), ...}
-		- context_phase = {context: phase, ...}
+		- context_eap = {context: eap, ...}
 		- earlier_than_rel = {sample: [sample, ...], ...}
 	"""
 	
 	data = load_input(fname)
 	samples, context_samples, context_area, areas = get_samples_contexts_and_areas(data)
 	long_lived = get_long_lived(data)
 	redeposited = get_redeposited(data)
 	outlier = get_outlier(data)
 	r_dates = get_c14_dates(data)
-	context_phase = get_context_phase(data)
+	context_eap = get_context_eap(data)
 	earlier_than_rel = get_earlier_than_relations(data, context_samples)
 	
 	contexts = {}
 	for context in context_samples:
 		for sample in context_samples[context]:
 			contexts[sample] = context
 		if context not in context_area:
 			context_area[context] = None
-		if context not in context_phase:
-			context_phase[context] = None
+		if context not in context_eap:
+			context_eap[context] = None
 	
 	for sample in samples:
 		if sample not in contexts:
 			contexts[sample] = None
 		if sample not in long_lived:
 			long_lived[sample] = False
 		if sample not in redeposited:
@@ -249,8 +246,8 @@
 		if sample not in outlier:
 			outlier[sample] = False
 		if sample not in r_dates:
 			r_dates[sample] = (None, None)
 		if sample not in earlier_than_rel:
 			earlier_than_rel[sample] = []
 	
-	return samples, contexts, context_area, long_lived, redeposited, outlier, r_dates, context_phase, earlier_than_rel
+	return samples, contexts, context_area, long_lived, redeposited, outlier, r_dates, context_eap, earlier_than_rel
```

### Comparing `sitesyncro-0.9.4/src/sitesyncro/utils/fnc_mp.py` & `sitesyncro-0.9.5/src/sitesyncro/utils/fnc_mp.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,20 @@
+from queue import Empty as QueueEmpty
 import multiprocessing as mp
 import threading
 import time
 
 from typing import Union, Generator, Callable
 
 
 def _worker(worker_fnc: Callable, params_mp: mp.Queue, collect_mp: mp.Queue, max_queue_size: int, args: list) -> None:
 	while True:
 		try:
 			params = params_mp.get(timeout=10)
-		except mp.Empty:
+		except QueueEmpty:
 			return
 		except:
 			time.sleep(0.01)
 			continue
 		
 		while collect_mp.qsize() > max_queue_size:
 			time.sleep(0.01)
```

### Comparing `sitesyncro-0.9.4/src/sitesyncro/utils/fnc_oxcal.py` & `sitesyncro-0.9.5/src/sitesyncro/utils/fnc_oxcal.py`

 * *Files 6% similar despite different names*

```diff
@@ -178,65 +178,14 @@
 		txt += '''
 		Label("%s-%d");
 		%s
 		''' % (name, phase, data[phase])
 	return txt
 
 
-def gen_oxcal_model(model: object) -> str:
-	"""
-	Generate an OxCal model string.
-
-	This function generates an OxCal model string based on the provided model object.
-
-	Parameters:
-	model (Model): The Model object.
-
-	Returns:
-	str: The generated OxCal model string.
-
-	Raises:
-	Exception: If an invalid phase model is specified.
-	"""
-	model_fncs = {
-		'sequence': gen_sequence,
-		'contiguous': gen_contiguous,
-		'overlapping': gen_overlapping,
-		'none': gen_none,
-	}
-	if model.phase_model not in model_fncs:
-		raise Exception("Invalid model specified: %s" % (model.phase_model))
-	
-	txt = ''
-	groups = model.groups
-	for group in groups:
-		data = defaultdict(list)
-		for name in groups[group]:
-			data[model.samples[name].phase].append(model.samples[name])
-		data = dict(data)
-		for phase in data:
-			data_phase = sorted(data[phase], key=lambda sample: sum(sample.get_range()))
-			data[phase] = "\n".join([sample.to_oxcal() for sample in data_phase])
-		txt += model_fncs[model.phase_model]("Gr.%d" % (group), data)
-	
-	txt = '''
-Curve("%s","%s");
-Plot()
-{
-	Outlier_Model("Charcoal",Exp(1,-10,0),U(0,3),"t");
-	Outlier_Model("General",T(5),U(0,4),"t");
-	%s
-};
-	''' % (model.curve_name, model.curve_name, txt)
-	
-	# Replace non-ASCII characters with their closest ASCII equivalent
-	txt = ''.join(c for c in unicodedata.normalize('NFKD', txt) if unicodedata.category(c) != 'Mn')
-	return txt
-
-
 def load_oxcal_data(fname: str) -> Dict:
 	"""
 	Load OxCal data from a file.
 
 	This function loads OxCal data from a specified file.
 
 	Parameters:
@@ -262,15 +211,15 @@
 		# Recursively process the modified string
 		return replace_colons_in_braces(s)
 	
 	def read_js_file(file_path):
 		
 		data = {}
 		
-		with (open(file_path, 'r') as file):
+		with (open(file_path, 'r', encoding='utf-8') as file):
 			for line in file:
 				if line.startswith('if('):
 					continue
 				
 				# Replace last character of line with a comma
 				line = line[:-2] + ',' + line[-1]
```

### Comparing `sitesyncro-0.9.4/src/sitesyncro/utils/fnc_plot.py` & `sitesyncro-0.9.5/src/sitesyncro/mhelpers/MPlot.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,178 +1,183 @@
+import codecs
 import numpy as np
 from matplotlib import pyplot
 
-
-def plot_randomized(model: object, fname: str, show: bool = False) -> None:
-	"""
-	Plots the randomization test results.
-
-	Parameters:
-	model (Model): The Model object containing the samples.
-	fname (str): The filename where the plot will be saved.
-	show (bool): If True, the plot will be displayed. Default is False.
-
-	Returns:
-	None
+class MPlot(object):
 	"""
+	A class implementing results plotting functionality
 	
-	if model.random_p < model.p_value:
-		null_hypothesis_txt = "Dates are not %s distributed." % ("uniformly" if model.uniform else "normally")
-	else:
-		null_hypothesis_txt = "Dates are %s distributed." % ("uniformly" if model.uniform else "normally")
-	
-	perc_lower = (model.p_value * 100) / 2
-	perc_upper = 100 - perc_lower
-	
-	fig = pyplot.figure(figsize=(15, 4))
-	pyplot.fill_between(model.years - 1950, model.random_lower, model.random_upper, color="lightgrey",
-	                    label="%0.2f%% of randomized dates" % (perc_upper - perc_lower))
-	pyplot.plot(model.years - 1950, model.summed, color="k", label="Observed dates")
-	idxs = np.where(model.random_upper > 0)[0]
-	idx1, idx2 = idxs.min(), idxs.max()
-	pyplot.xlim(model.years[int(idx1)] - 1950, model.years[int(idx2)] - 1950)
-	pyplot.gca().invert_xaxis()
-	pyplot.xlabel("Calendar age (yrs BC)")
-	pyplot.ylabel("Summed p")
-	pyplot.annotate("p: %0.5f\n%s" % (model.random_p, null_hypothesis_txt), xy=(0.05, 0.95), xycoords="axes fraction",
-	                fontsize=12, horizontalalignment="left", verticalalignment="top")
-	pyplot.legend()
-	pyplot.tight_layout()
-	pyplot.savefig(fname)
-	if show:
-		pyplot.show()
-	pyplot.close()
-
-
-def plot_clusters(model: object, fname: str, show: bool = False) -> None:
-	"""
-	Plots Silhouette and p-value for solutions with different numbers of clusters.
-
-	Parameters:
-	model (Model): The Model object containing the samples.
-	fname (str): The filename where the plot will be saved.
-	show (bool): If True, the plot will be displayed. Default is False.
-
-	Returns:
-	None
+	:param model: The parent Model object
+	:type model: Model
 	"""
-	
-	clu_ns = np.array(sorted(list(model.clusters.keys())), dtype=int)
-	ps_plot = np.array([model.cluster_ps[clu_n] for clu_n in clu_ns])
-	sils_plot = np.array([model.cluster_sils[clu_n] for clu_n in clu_ns])
-	
-	color1 = "#414487"
-	color2 = "#7AD151"
-	color3 = "#FDE725"
-	
-	fig, ax1 = pyplot.subplots()
-	
-	ax1.set_xlabel("Clusters")
-	ax1.set_ylabel("Mean Silhouette Coefficient", color=color1)
-	ax1.plot(clu_ns, sils_plot, color=color1)
-	ax1.plot(clu_ns, sils_plot, ".", color=color1)
-	ax1.tick_params(axis="y", labelcolor=color1)
-	
-	ax2 = ax1.twinx()
-	ax2.set_ylabel("p", color=color2)
-	ax2.plot(clu_ns, ps_plot, color=color2)
-	ax2.plot(clu_ns, ps_plot, ".", color=color2)
-	if model.cluster_opt_n is not None:
-		ax2.plot([model.cluster_opt_n, model.cluster_opt_n], [0, max(ps_plot.max(), sils_plot.max())], color=color3,
-		         linewidth=0.7, label="Optimal no. of clusters")
-	if model.p_value is not None:
-		ax2.plot([clu_ns[0], clu_ns[-1]], [model.p_value, model.p_value], "--", color=color2, linewidth=0.7)
-		ax2.annotate("p = %0.3f" % (model.p_value), xy=(clu_ns.mean(), model.p_value), xytext=(0, -3),
-		             textcoords="offset pixels", va="top", ha="center", color=color2)
-	ax2.tick_params(axis="y", labelcolor=color2)
-	
-	pyplot.xticks(clu_ns, clu_ns)
-	pyplot.legend()
-	
-	fig.tight_layout()
-	pyplot.savefig(fname)
-	if show:
-		pyplot.show()
-	pyplot.close()
-
-
-def save_outliers(model: object, fname: str) -> None:
-	"""
-	Saves the outliers and outlier candidates to a file.
-
-	Parameters:
-	model (Model): The Model object containing the samples.
-	fname (str): The filename where the outliers will be saved.
-
-	Returns:
-	None
-	"""
-	txt = "Eliminated outliers:\n"
-	outliers = model.outliers
-	if outliers:
-		txt += "%s\n" % (", ".join(outliers))
-	else:
-		txt += "None\n"
-	txt += "\nOutlier candidates:\n"
-	candidates = model.outlier_candidates
-	if candidates:
-		txt += "%s\n" % (", ".join(candidates))
-	else:
-		txt += "None\n"
-	
-	with open(fname, "w") as file:
-		file.write(txt)
-
-
-def save_results_csv(model: object, fcsv: str) -> None:
-	"""
-	Saves the results to a CSV file.
-
-	Parameters:
-	model (Model): The Model object containing the samples.
-	fcsv (str): The filename where the results will be saved.
-
-	Returns:
-	None
-	"""
-	
-	def _format_year(value):
+	def __init__(self, model: 'Model'):
 		
-		if value is None:
-			return "None"
-		return "%0.2f" % (-(value - 1950))
-	
-	samples = list(model.samples.keys())
-	
-	def _sum_range(rng):
-		if None in rng:
-			return -1
-		return sum(rng)
+		self.model = model
 	
-	samples = sorted(samples, key=lambda name: [
-		model.samples[name].group,
-		model.samples[name].phase,
-		_sum_range(model.samples[name].likelihood_range)
-	])
-	
-	cluster = dict([(name, None) for name in samples])
-	if model.is_clustered:
-		m_clusters = model.clusters[model.cluster_opt_n]
-		for clu in m_clusters:
-			for name in m_clusters[clu]:
-				cluster[name] = clu
+	def plot_randomized(self, fname: str, show: bool = False) -> None:
+		"""
+		Plots the randomization test results.
+
+		Parameters:
+		fname (str): The filename where the plot will be saved.
+		show (bool): If True, the plot will be displayed. Default is False.
+
+		Returns:
+		None
+		"""
+		
+		if self.model.random_p < self.model.p_value:
+			null_hypothesis_txt = "Dates are not %s distributed." % ("uniformly" if self.model.uniform else "normally")
+		else:
+			null_hypothesis_txt = "Dates are %s distributed." % ("uniformly" if self.model.uniform else "normally")
+		
+		perc_lower = (self.model.p_value * 100) / 2
+		perc_upper = 100 - perc_lower
+		
+		fig = pyplot.figure(figsize=(15, 4))
+		pyplot.fill_between(self.model.years - 1950, self.model.random_lower, self.model.random_upper, color="lightgrey",
+							label="%0.2f%% of randomized dates" % (perc_upper - perc_lower))
+		pyplot.plot(self.model.years - 1950, self.model.summed, color="k", label="Observed dates")
+		idxs = np.where(self.model.random_upper > 0)[0]
+		idx1, idx2 = idxs.min(), idxs.max()
+		pyplot.xlim(self.model.years[int(idx1)] - 1950, self.model.years[int(idx2)] - 1950)
+		pyplot.gca().invert_xaxis()
+		pyplot.xlabel("Calendar age (yrs BC)")
+		pyplot.ylabel("Summed p")
+		pyplot.annotate("p: %0.5f\n%s" % (self.model.random_p, null_hypothesis_txt), xy=(0.05, 0.95), xycoords="axes fraction",
+						fontsize=12, horizontalalignment="left", verticalalignment="top")
+		pyplot.legend()
+		pyplot.tight_layout()
+		pyplot.savefig(fname)
+		if show:
+			pyplot.show()
+		pyplot.close()
+	
+	def plot_clusters(self, fname: str, show: bool = False) -> None:
+		"""
+		Plots Silhouette and p-value for solutions with different numbers of clusters.
+
+		Parameters:
+		fname (str): The filename where the plot will be saved.
+		show (bool): If True, the plot will be displayed. Default is False.
+
+		Returns:
+		None
+		"""
+		
+		clu_ns = np.array(sorted(list(self.model.clusters.keys())), dtype=int)
+		ps_plot = np.array([self.model.cluster_ps[clu_n] for clu_n in clu_ns])
+		sils_plot = np.array([self.model.cluster_sils[clu_n] for clu_n in clu_ns])
+		
+		color1 = "#414487"
+		color2 = "#7AD151"
+		color3 = "#FDE725"
+		
+		fig, ax1 = pyplot.subplots()
+		
+		ax1.set_xlabel("Clusters")
+		ax1.set_ylabel("Mean Silhouette Coefficient", color=color1)
+		ax1.plot(clu_ns, sils_plot, color=color1)
+		ax1.plot(clu_ns, sils_plot, ".", color=color1)
+		ax1.tick_params(axis="y", labelcolor=color1)
+		
+		ax2 = ax1.twinx()
+		ax2.set_ylabel("p", color=color2)
+		ax2.plot(clu_ns, ps_plot, color=color2)
+		ax2.plot(clu_ns, ps_plot, ".", color=color2)
+		if self.model.cluster_opt_n is not None:
+			ax2.plot([self.model.cluster_opt_n, self.model.cluster_opt_n], [0, max(ps_plot.max(), sils_plot.max())], color=color3,
+					 linewidth=0.7, label="Optimal no. of clusters")
+		if self.model.p_value is not None:
+			ax2.plot([clu_ns[0], clu_ns[-1]], [self.model.p_value, self.model.p_value], "--", color=color2, linewidth=0.7)
+			ax2.annotate("p = %0.3f" % (self.model.p_value), xy=(clu_ns.mean(), self.model.p_value), xytext=(0, -3),
+						 textcoords="offset pixels", va="top", ha="center", color=color2)
+		ax2.tick_params(axis="y", labelcolor=color2)
+		
+		pyplot.xticks(clu_ns, clu_ns)
+		pyplot.legend()
+		
+		fig.tight_layout()
+		pyplot.savefig(fname)
+		if show:
+			pyplot.show()
+		pyplot.close()
+	
+	def save_outliers(self, fname: str) -> None:
+		"""
+		Saves the outliers and outlier candidates to a file.
+
+		Parameters:
+		fname (str): The filename where the outliers will be saved.
+
+		Returns:
+		None
+		"""
+		txt = "Eliminated outliers:\n"
+		outliers = self.model.outliers
+		if outliers:
+			txt += "%s\n" % (", ".join(outliers))
+		else:
+			txt += "None\n"
+		txt += "\nOutlier candidates:\n"
+		candidates = self.model.outlier_candidates
+		if candidates:
+			txt += "%s\n" % (", ".join(candidates))
+		else:
+			txt += "None\n"
+		
+		with open(fname, "w", encoding="utf-8") as file:
+			file.write(txt)
 	
-	with open(fcsv, "w") as file:
-		file.write(
-			"Name;Context;Area;C-14 Date;C-14 Uncertainty;Long-Lived;Redeposited;Outlier;Group;Phase;Cluster;Unmodeled From (CE);Unmodeled To (CE);Modeled From (CE);Modeled To (CE)\n")
-		for name in samples:
-			likelihood_min, likelihood_max = model.samples[name].likelihood_range
-			posterior_min, posterior_max = model.samples[name].posterior_range
-			file.write('''"%s";"%s";"%s";%0.2f;%0.2f;%s;%s;%s;%s;%s;%s;%s;%s;%s;%s\n''' % (
-				name, model.samples[name].context, model.samples[name].area,
-				model.samples[name].age, model.samples[name].uncertainty,
-				int(model.samples[name].long_lived), int(model.samples[name].redeposited),
-				int(model.samples[name].outlier),
-				model.samples[name].group, model.samples[name].phase, cluster[name],
-				_format_year(likelihood_min), _format_year(likelihood_max),
-				_format_year(posterior_min), _format_year(posterior_max)
-			))
+	def save_results_csv(self, fcsv: str) -> None:
+		"""
+		Saves the results to a CSV file.
+
+		Parameters:
+		fcsv (str): The filename where the results will be saved.
+
+		Returns:
+		None
+		"""
+		
+		def _format_year(value):
+			
+			if value is None:
+				return "None"
+			return "%0.2f" % (-(value - 1950))
+		
+		samples = list(self.model.samples.keys())
+		
+		def _sum_range(rng):
+			if None in rng:
+				return -1
+			return sum(rng)
+		
+		samples = sorted(samples, key=lambda name: [
+			self.model.samples[name].group,
+			self.model.samples[name].phase,
+			_sum_range(self.model.samples[name].likelihood_range)
+		])
+		
+		cluster = dict([(name, None) for name in samples])
+		if self.model.is_clustered:
+			m_clusters = self.model.clusters[self.model.cluster_opt_n]
+			for clu in m_clusters:
+				for name in m_clusters[clu]:
+					cluster[name] = clu
+		
+		with codecs.open(fcsv, "w", encoding="utf-8-sig") as file:
+			file.write(
+				"Name;Context;Area;C-14 Date;C-14 Uncertainty;Long-Lived;Redeposited;Outlier;EAP;Group;Phase;Cluster;Unmodeled From (CE);Unmodeled To (CE);Modeled From (CE);Modeled To (CE)\n")
+			for name in samples:
+				likelihood_min, likelihood_max = self.model.samples[name].likelihood_range
+				posterior_min, posterior_max = self.model.samples[name].posterior_range
+				file.write('''"%s";"%s";"%s";%0.2f;%0.2f;%s;%s;%s;%s;%s;%s;%s;%s;%s;%s;%s\n''' % (
+					name, self.model.samples[name].context, self.model.samples[name].area,
+					self.model.samples[name].age, self.model.samples[name].uncertainty,
+					int(self.model.samples[name].long_lived), int(self.model.samples[name].redeposited),
+					int(self.model.samples[name].outlier), self.model.samples[name].excavation_area_phase,
+					self.model.samples[name].group, self.model.samples[name].phase, cluster[name],
+					_format_year(likelihood_min), _format_year(likelihood_max),
+					_format_year(posterior_min), _format_year(posterior_max)
+				))
+
```

### Comparing `sitesyncro-0.9.4/src/sitesyncro/utils/fnc_radiocarbon.py` & `sitesyncro-0.9.5/src/sitesyncro/utils/fnc_radiocarbon.py`

 * *Files identical despite different names*

### Comparing `sitesyncro-0.9.4/src/sitesyncro/utils/fnc_stat.py` & `sitesyncro-0.9.5/src/sitesyncro/utils/fnc_stat.py`

 * *Files identical despite different names*

### Comparing `sitesyncro-0.9.4/src/sitesyncro.egg-info/PKG-INFO` & `sitesyncro-0.9.5/src/sitesyncro.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sitesyncro
-Version: 0.9.4
+Version: 0.9.5
 Summary: SiteSyncro - Site-specific chronological modeling and synchronization
 Home-page: https://github.com/demjanp/SiteSyncro
 Author: Peter Demjan
 Author-email: peter.demjan@gmail.com
 Keywords: archaeology,radiocarbon,chronology,stratigraphy
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
@@ -16,22 +16,27 @@
 License-File: LICENSE
 Requires-Dist: numpy<2,>=1.26.4
 Requires-Dist: scipy<2,>=1.13.0
 Requires-Dist: matplotlib<4,>=3.8.4
 Requires-Dist: scikit-learn<2,>=1.4.2
 Requires-Dist: tqdm<5,>=4.66.0
 Requires-Dist: requests<3,>=2.31.0
-Requires-Dist: networkx<4,>=3.3.0
+Requires-Dist: networkx<4,>=2.8.0
+Requires-Dist: sphinx<7.4,>=7.3.7
+Requires-Dist: myst-parser<3.1,>=3.0.1
 
 # SiteSyncro
 Site-specific chronological modeling and synchronization
 
 Created on 10.4.2024
 
-<details>
+Project homepage: [https://github.com/demjanp/SiteSyncro](https://github.com/demjanp/SiteSyncro)
+
+Documentation: [https://sitesyncro.readthedocs.io](https://sitesyncro.readthedocs.io)
+
 <summary>Table of Contents</summary>
 
 1. [About SiteSyncro](#about)
 2. [Installation](#installation)
 3. [Usage](#usage)
    * [Input File Format](#input_file)
    * [Model Class](#model_class)
@@ -39,16 +44,14 @@
 4. [Developer Notes](#developer)
 	* [Preparing the Virtual Environment](#venv)
 	* [Building a Windows Executable](#build)
 5. [Contact](#contact)
 6. [Acknowledgements](#acknowledgements)
 7. [License](#license)
 
-</details>
-
 ## About SiteSyncro <a name="about"></a>
 SiteSyncro is a Python-based tool designed for site-specific chronological modeling and synchronization based on radiocarbon dates from stratigraphically and/or spatially linked archaeological contexts. It uses the [OxCal](https://c14.arch.ox.ac.uk/oxcal.html) program for bayesian modelling and a method of temporal clustering of the modelled C-14 dates to determine whether they represent separate events, or phases in time.
  
 The input data represent radiocarbon dates and their stratigraphic relations. Here is a brief overview of the processing workflow:
 1. Bayesian modeling of distributions of the C-14 dates based on stratigraphic constrains using the [OxCal](https://c14.arch.ox.ac.uk/oxcal.html) program.
 2. Randomization testing of the null hypothesis that the observed C-14 dates represent a normal / uniform distribution
 3. Temporal clustering of the modelled C-14 dates. All possible clusterings are produced and tested for randomness. The optimal number of clusters is selected for further analyses.
@@ -72,15 +75,15 @@
 See [Model Class](#model_class) on usage tips.
 
 SiteSyncro requires [OxCal](https://c14.arch.ox.ac.uk/oxcal.html) to be installed in its default location. The program is not included in the SiteSyncro package and must be installed separately. OxCal should be downloaded and installed automatically when running SiteSyncro for the first time. You can also download OxCal manually from the [OxCal website](https://c14.arch.ox.ac.uk/OxCalDistribution.zip) and unzip it in the SiteSyncro folder.
 
 ## Usage <a name="usage"></a>
 
 ### Running the Script
-To use SiteSyncro, you need to run the [process.py](bin/process.py) or `sitesyncro.exe` script. This script accepts several command-line arguments. Here's a basic example of how to run the script:
+To use SiteSyncro, you need to run the [process.py](https://github.com/demjanp/SiteSyncro/blob/main/bin/process.py) or `sitesyncro.exe` script. This script accepts several command-line arguments. Here's a basic example of how to run the script:
 ```
 python process.py -input data_sample.csv
 ```
 or
 ```
 sitesyncro.exe -input data_sample.csv
 ```
@@ -113,21 +116,21 @@
 ### Input File Format <a name="input_file"></a>
 The input file name must be a semicolon-separated CSV file with the following 10 columns: 
 1. Sample: Sample ID (required, unique identifier)
 2. Context: Context ID (required)
 3. Excavation Area: Excavation area ID (required)
 4. C-14 Age: Radiocarbon age in years BP (required)
 5. Uncertainty: Uncertainty of the radiocarbon age in C-14 years (required)
-6. Phase: Phase of the sample (lower = older) (optional)
+6. Excavation Area Phase: Phase of the sample (format: '1' or '1a' or '1-2' or '1a-b' or '1a-2b', higher = earlier (older) phase) (optional)
 7. Earlier-Than: List of contexts that the sample is earlier (older) than (optional)
 8. Long-Lived: Flag indicating whether the sample is long-lived (e.g. old wood)(required, 1 or 0)
 9. Redeposited: Flag indicating whether the sample could be redeposited from a different context (required, 1 or 0)
 10. Outlier: Flag indicating whether the sample is an outlier and should not be used for modeling (required, 1 or 0)
 
-See [data_sample.csv](data_sample.csv) for an example of the input file format.
+See [data_sample.csv](https://github.com/demjanp/SiteSyncro/blob/main/data_sample.csv) for an example of the input file format.
 
 ### Model Class <a name="model_class"></a>
 All functions regarding modeling are encapsulated in the `Model` class. Here is a basic example of how to use it:
 
 ```python
 from sitesyncro import Model
 
@@ -166,15 +169,15 @@
 
 ```python
 from sitesyncro import Sample
 
 if __name__ == '__main__':
 	
 	# Initialize the Sample object
-	sample = Sample('Sample1', 1000, 50, phase = 1, earlier_than = ['Sample2'], long_lived = 1)
+	sample = Sample('Sample1', 1000, 50, excavation_area_phase = 1, earlier_than = ['Sample2'], long_lived = 1)
 	
 	# Print the sample data
 	print(sample)
 ```
 
 See [Sample Class](https://sitesyncro.readthedocs.io/en/latest/sample.html) documentation for more information.
 
@@ -237,8 +240,8 @@
 * [Requests](https://requests.readthedocs.io/)
 * [Scikit-learn](https://scikit-learn.org/)
 * [SciPy](https://scipy.org/)
 * [tqdm](https://tqdm.github.io/)
 
 ## License <a name="license"></a>
 
-This code is licensed under the [GNU GENERAL PUBLIC LICENSE](https://www.gnu.org/licenses/gpl-3.0.en.html) - see the [LICENSE](LICENSE) file for details
+This code is licensed under the [GNU GENERAL PUBLIC LICENSE](https://www.gnu.org/licenses/gpl-3.0.en.html) - see the [LICENSE](https://github.com/demjanp/SiteSyncro/blob/main/LICENSE) file for details
```

### Comparing `sitesyncro-0.9.4/src/sitesyncro.egg-info/SOURCES.txt` & `sitesyncro-0.9.5/src/sitesyncro.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -5,18 +5,23 @@
 src/sitesyncro/Sample.py
 src/sitesyncro/__init__.py
 src/sitesyncro.egg-info/PKG-INFO
 src/sitesyncro.egg-info/SOURCES.txt
 src/sitesyncro.egg-info/dependency_links.txt
 src/sitesyncro.egg-info/requires.txt
 src/sitesyncro.egg-info/top_level.txt
+src/sitesyncro/mhelpers/MCluster.py
+src/sitesyncro/mhelpers/MOxCal.py
+src/sitesyncro/mhelpers/MPhasing.py
+src/sitesyncro/mhelpers/MPlot.py
+src/sitesyncro/mhelpers/MRandomization.py
+src/sitesyncro/mhelpers/__init__.py
 src/sitesyncro/utils/__init__.py
 src/sitesyncro/utils/fnc_cluster.py
 src/sitesyncro/utils/fnc_data.py
 src/sitesyncro/utils/fnc_load.py
 src/sitesyncro/utils/fnc_mp.py
 src/sitesyncro/utils/fnc_oxcal.py
 src/sitesyncro/utils/fnc_phase.py
-src/sitesyncro/utils/fnc_plot.py
 src/sitesyncro/utils/fnc_radiocarbon.py
 src/sitesyncro/utils/fnc_simulate.py
 src/sitesyncro/utils/fnc_stat.py
```

