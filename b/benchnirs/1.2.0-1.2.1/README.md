# Comparing `tmp/benchnirs-1.2.0.tar.gz` & `tmp/benchnirs-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "benchnirs-1.2.0.tar", last modified: Tue May 14 13:39:38 2024, max compression
+gzip compressed data, was "benchnirs-1.2.1.tar", last modified: Thu May 16 08:09:33 2024, max compression
```

## Comparing `benchnirs-1.2.0.tar` & `benchnirs-1.2.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 13:39:38.836725 benchnirs-1.2.0/
--rw-rw-rw-   0 root         (0) root         (0)    35083 2024-05-14 13:39:29.000000 benchnirs-1.2.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)    11603 2024-05-14 13:39:38.836725 benchnirs-1.2.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    11064 2024-05-14 13:39:29.000000 benchnirs-1.2.0/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-14 13:39:38.836725 benchnirs-1.2.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      980 2024-05-14 13:39:29.000000 benchnirs-1.2.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 13:39:38.833725 benchnirs-1.2.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 13:39:38.835725 benchnirs-1.2.0/src/benchnirs/
--rw-rw-rw-   0 root         (0) root         (0)      224 2024-05-14 13:39:29.000000 benchnirs-1.2.0/src/benchnirs/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    48933 2024-05-14 13:39:29.000000 benchnirs-1.2.0/src/benchnirs/learn.py
--rw-rw-rw-   0 root         (0) root         (0)    25059 2024-05-14 13:39:29.000000 benchnirs-1.2.0/src/benchnirs/load.py
--rw-rw-rw-   0 root         (0) root         (0)     2822 2024-05-14 13:39:29.000000 benchnirs-1.2.0/src/benchnirs/process.py
--rw-rw-rw-   0 root         (0) root         (0)     3946 2024-05-14 13:39:29.000000 benchnirs-1.2.0/src/benchnirs/viz.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-14 13:39:38.836725 benchnirs-1.2.0/src/benchnirs.egg-info/
--rw-r--r--   0 root         (0) root         (0)    11603 2024-05-14 13:39:38.000000 benchnirs-1.2.0/src/benchnirs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      327 2024-05-14 13:39:38.000000 benchnirs-1.2.0/src/benchnirs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-14 13:39:38.000000 benchnirs-1.2.0/src/benchnirs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       71 2024-05-14 13:39:38.000000 benchnirs-1.2.0/src/benchnirs.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2024-05-14 13:39:38.000000 benchnirs-1.2.0/src/benchnirs.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 08:09:33.128163 benchnirs-1.2.1/
+-rw-rw-rw-   0 root         (0) root         (0)    35083 2024-05-16 08:09:24.000000 benchnirs-1.2.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    11736 2024-05-16 08:09:33.128163 benchnirs-1.2.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    11197 2024-05-16 08:09:24.000000 benchnirs-1.2.1/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-16 08:09:33.128163 benchnirs-1.2.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      980 2024-05-16 08:09:24.000000 benchnirs-1.2.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 08:09:33.124163 benchnirs-1.2.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 08:09:33.126163 benchnirs-1.2.1/src/benchnirs/
+-rw-rw-rw-   0 root         (0) root         (0)      224 2024-05-16 08:09:24.000000 benchnirs-1.2.1/src/benchnirs/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    48933 2024-05-16 08:09:24.000000 benchnirs-1.2.1/src/benchnirs/learn.py
+-rw-rw-rw-   0 root         (0) root         (0)    25059 2024-05-16 08:09:24.000000 benchnirs-1.2.1/src/benchnirs/load.py
+-rw-rw-rw-   0 root         (0) root         (0)     2822 2024-05-16 08:09:24.000000 benchnirs-1.2.1/src/benchnirs/process.py
+-rw-rw-rw-   0 root         (0) root         (0)     3946 2024-05-16 08:09:24.000000 benchnirs-1.2.1/src/benchnirs/viz.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 08:09:33.127163 benchnirs-1.2.1/src/benchnirs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    11736 2024-05-16 08:09:33.000000 benchnirs-1.2.1/src/benchnirs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      327 2024-05-16 08:09:33.000000 benchnirs-1.2.1/src/benchnirs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-16 08:09:33.000000 benchnirs-1.2.1/src/benchnirs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       71 2024-05-16 08:09:33.000000 benchnirs-1.2.1/src/benchnirs.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2024-05-16 08:09:33.000000 benchnirs-1.2.1/src/benchnirs.egg-info/top_level.txt
```

### Comparing `benchnirs-1.2.0/LICENSE` & `benchnirs-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `benchnirs-1.2.0/PKG-INFO` & `benchnirs-1.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: benchnirs
-Version: 1.2.0
+Version: 1.2.1
 Summary: Benchmarking framework for machine learning with fNIRS
 Home-page: https://gitlab.com/HanBnrd/benchnirs
 Author: Johann Benerradi
 Author-email: johann.benerradi@gmail.com
 License: GNU GPLv3+
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -66,52 +66,46 @@
 - [scikit-learn 0.24](https://scikit-learn.org/stable/install.html)
 - [scipy 1.8](https://scipy.org/install/)
 - [seaborn 0.11](https://seaborn.pydata.org/installing.html)
 - [statsmodels 0.12.2](https://www.statsmodels.org/dev/install.html)
 - [torch 1.5](https://pytorch.org/get-started/locally/)
 
 
+## Setting up *BenchNIRS*
+1. Download and install Python 3.8 or greater, for example with [Miniconda](https://docs.conda.io/projects/miniconda/en/latest/index.html).
+
+2. To install the package with *pip* (cf. [PyPI](https://pypi.org/project/benchnirs/)), open a terminal (eg. Anaconda Prompt) and type:
+```bash
+pip install benchnirs
+```
+> Alternatively to install from source, download and unzip the [repository](https://gitlab.com/HanBnrd/benchnirs/-/archive/main/benchnirs-main.zip).
+> Then, in a terminal or command prompt (eg. Anaconda Prompt), navigate to the directory containing the `requirements.txt` file and run:
+> ```bash
+> python -m pip install -r requirements.txt -f https://download.pytorch.org/whl/torch_stable.html
+> ```
+
+3. Download the datasets (see below).
+
+
 ## Downloading the datasets
 - *Herff et al. 2014* (n-back task): you can download the dataset by making a request [here](http://www.csl.uni-bremen.de/CorpusData/download.php?crps=fNIRS). In the examples, the unzipped folder has been renamed to *dataset_herff_2014* for convenience.
 - *Shin et al. 2018* (n-back and word generation tasks): you can download the dataset [here](http://doc.ml.tu-berlin.de/simultaneous_EEG_NIRS/NIRS/NIRS_01-26_MATLAB.zip). In the examples, the unzipped folder has been renamed to *dataset_shin_2018* for convenience.
 - *Shin et al. 2016* (mental arithmetic task): you can download the dataset by filling the form [here](http://doc.ml.tu-berlin.de/hBCI). Then click on *NIRS_01-29* to download the fNIRS data. In the examples, the unzipped folder has been renamed to *dataset_shin_2016* for convenience.
 - *Bak et al. 2019* (motor execution task): you can download the dataset [here](https://figshare.com/ndownloader/files/18069143). In the examples, the unzipped folder has been renamed to *dataset_bak_2019* for convenience.
 
 
-## Setup
-Download and install Python 3.8 or greater, for example with [Miniconda](https://docs.conda.io/projects/miniconda/en/latest/index.html).
-
-Download and unzip the [*BenchNIRS* repository](https://gitlab.com/HanBnrd/benchnirs/-/archive/main/benchnirs-main.zip).
-
-In a terminal or command prompt (eg. Anaconda Prompt), navigate to the directory containing the `requirements.txt` file and run:
+## Keeping *BenchNIRS* up to date
+To update *BenchNIRS* to the latest version with *pip*, open a terminal (eg. Anaconda Prompt) and type:
 ```bash
-python -m pip install -r requirements.txt -f https://download.pytorch.org/whl/torch_stable.html
+pip install --upgrade benchnirs
 ```
 
-> Alternatively, the *BenchNIRS* library containing the core functions (without main scripts) is available on [PyPI](https://pypi.org/project/benchnirs/) and can be installed using `pip`:
-> ```bash
-> pip install benchnirs
-> ```
-> and updated to the newest version with:
-> ```bash
-> pip install --upgrade benchnirs
-> ```
-
-
-## Running main scripts
-- [`generalised.py`](https://gitlab.com/HanBnrd/benchnirs/-/blob/main/src/generalised.py) compares the 6 models (LDA, SVC, kNN, ANN, CNN and LSTM) on the 5 datasets with a generalised approach (testing with unseen subjects)
-- [`dataset_size.py`](https://gitlab.com/HanBnrd/benchnirs/-/blob/main/src/dataset_size.py) reproduces `generalised.py` but with a range of different dataset sizes (50% to 100% of dataset) to study the influence of this parameter on the classification accuracy
-- [`window_size.py`](https://gitlab.com/HanBnrd/benchnirs/-/blob/main/src/window_size.py) reproduces `generalised.py` but with only the 4 models using feature extraction (LDA, SVC, kNN and ANN) and with a range of different window sizes (2 to 10 seconds) to study the influence of this parameter on the classification accuracy
-- [`sliding_window.py`](https://gitlab.com/HanBnrd/benchnirs/-/blob/main/src/sliding_window.py) reproduces `generalised.py` but with only the 4 models using feature extraction (LDA, SVC, kNN and ANN) and with a 2-second sliding window on the 10-second epochs
-- [`personalised.py`](https://gitlab.com/HanBnrd/benchnirs/-/blob/main/src/personalised.py) compares the 6 models (LDA, SVC, kNN, ANN, CNN and LSTM) on the 5 datasets with a personalised approach (training and testing with each subject individually)
-- [`visualisation.py`](https://gitlab.com/HanBnrd/benchnirs/-/blob/main/src/visualisation.py) enables to visualise the data from the datasets with various signal processing
-
 
 ## Example
-An example script showing how to use the framework with a custom deep learning model can be found [here](https://hanbnrd.gitlab.io/benchnirs/example.html).
+A full example script showing how to use the framework with a custom deep learning model can be found [here](https://hanbnrd.gitlab.io/benchnirs/example.html).
 
 
 ## Simple use case
 *BenchNIRS* enables to evaluate your model in Python with simplicity on an open access dataset supported:
 ```python
 import benchnirs as bn
 
@@ -119,29 +113,38 @@
 data = bn.process_epochs(epochs['0-back', '2-back', '3-back'])
 results = bn.deep_learn(*data, my_model)
 
 print(results)
 ```
 
 
+## Running main scripts
+- [`generalised.py`](https://gitlab.com/HanBnrd/benchnirs/-/blob/main/src/generalised.py) compares the 6 models (LDA, SVC, kNN, ANN, CNN and LSTM) on the 5 datasets with a generalised approach (testing with unseen subjects)
+- [`dataset_size.py`](https://gitlab.com/HanBnrd/benchnirs/-/blob/main/src/dataset_size.py) reproduces `generalised.py` but with a range of different dataset sizes (50% to 100% of dataset) to study the influence of this parameter on the classification accuracy
+- [`window_size.py`](https://gitlab.com/HanBnrd/benchnirs/-/blob/main/src/window_size.py) reproduces `generalised.py` but with only the 4 models using feature extraction (LDA, SVC, kNN and ANN) and with a range of different window sizes (2 to 10 seconds) to study the influence of this parameter on the classification accuracy
+- [`sliding_window.py`](https://gitlab.com/HanBnrd/benchnirs/-/blob/main/src/sliding_window.py) reproduces `generalised.py` but with only the 4 models using feature extraction (LDA, SVC, kNN and ANN) and with a 2-second sliding window on the 10-second epochs
+- [`personalised.py`](https://gitlab.com/HanBnrd/benchnirs/-/blob/main/src/personalised.py) compares the 6 models (LDA, SVC, kNN, ANN, CNN and LSTM) on the 5 datasets with a personalised approach (training and testing with each subject individually)
+- [`visualisation.py`](https://gitlab.com/HanBnrd/benchnirs/-/blob/main/src/visualisation.py) enables to visualise the data from the datasets with various signal processing
+
+
 ## Extra scripts: n-back tailored
 - `tailored_generalised.py` compares the 6 models (LDA, SVC, kNN, ANN, CNN and LSTM) on the 2 n-back datasets with a generalised approach (testing with unseen subjects)
 - `tailored_window_size.py` reproduces `tailored_generalised.py` but with only 5 models (LDA, SVC, kNN, ANN and LSTM) and with a range of different window sizes (5 to 40 seconds) to study the influence of this parameter on the classification accuracy
 - `tailored_shin_nb.py` optimises and evaluates a tailored CNN on the *Shin et al. 2018* n-back dataset with a generalised approach (testing with unseen subjects)
 
 
 ## Extra scripts: transfer learning
 - `transfer.py` optimises and evaluates a transfer learning model (pretext self-supervised representation learning task with unlabelled and labelled data using a CED, downstream supervised n-back classification task with labelled data) on the *Shin et al. 2018* n-back dataset with a generalised approach (testing with unseen subjects)
 - `transfer_no_unlab.py` reproduces `transfer.py` but with only labelled data for the pretext task.
 
 
 ## Contributing to the repository
 Contributions from the community to this repository are highly appreciated. We are mainly interested in contributions to:
 - improving the recommendation checklist
-- adding support for new **open access datasets**
+- adding support for new open access datasets
 - adding support for new machine learning models
 - adding more fNIRS signal processing techniques
 - improving the documentation
 - tracking bugs
 
 Contributions are encouraged under the form of [issues](https://gitlab.com/HanBnrd/benchnirs/-/issues) (for reporting bugs or requesting new features) and [merge requests](https://gitlab.com/HanBnrd/benchnirs/-/merge_requests) (for fixing bugs and implementing new features).
 Please refer to [this tutorial](https://docs.gitlab.com/ee/user/project/repository/forking_workflow.html) for creating merge requests from a fork of the repository.
```

### Comparing `benchnirs-1.2.0/README.md` & `benchnirs-1.2.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -50,52 +50,46 @@
 - [scikit-learn 0.24](https://scikit-learn.org/stable/install.html)
 - [scipy 1.8](https://scipy.org/install/)
 - [seaborn 0.11](https://seaborn.pydata.org/installing.html)
 - [statsmodels 0.12.2](https://www.statsmodels.org/dev/install.html)
 - [torch 1.5](https://pytorch.org/get-started/locally/)
 
 
+## Setting up *BenchNIRS*
+1. Download and install Python 3.8 or greater, for example with [Miniconda](https://docs.conda.io/projects/miniconda/en/latest/index.html).
+
+2. To install the package with *pip* (cf. [PyPI](https://pypi.org/project/benchnirs/)), open a terminal (eg. Anaconda Prompt) and type:
+```bash
+pip install benchnirs
+```
+> Alternatively to install from source, download and unzip the [repository](https://gitlab.com/HanBnrd/benchnirs/-/archive/main/benchnirs-main.zip).
+> Then, in a terminal or command prompt (eg. Anaconda Prompt), navigate to the directory containing the `requirements.txt` file and run:
+> ```bash
+> python -m pip install -r requirements.txt -f https://download.pytorch.org/whl/torch_stable.html
+> ```
+
+3. Download the datasets (see below).
+
+
 ## Downloading the datasets
 - *Herff et al. 2014* (n-back task): you can download the dataset by making a request [here](http://www.csl.uni-bremen.de/CorpusData/download.php?crps=fNIRS). In the examples, the unzipped folder has been renamed to *dataset_herff_2014* for convenience.
 - *Shin et al. 2018* (n-back and word generation tasks): you can download the dataset [here](http://doc.ml.tu-berlin.de/simultaneous_EEG_NIRS/NIRS/NIRS_01-26_MATLAB.zip). In the examples, the unzipped folder has been renamed to *dataset_shin_2018* for convenience.
 - *Shin et al. 2016* (mental arithmetic task): you can download the dataset by filling the form [here](http://doc.ml.tu-berlin.de/hBCI). Then click on *NIRS_01-29* to download the fNIRS data. In the examples, the unzipped folder has been renamed to *dataset_shin_2016* for convenience.
 - *Bak et al. 2019* (motor execution task): you can download the dataset [here](https://figshare.com/ndownloader/files/18069143). In the examples, the unzipped folder has been renamed to *dataset_bak_2019* for convenience.
 
 
-## Setup
-Download and install Python 3.8 or greater, for example with [Miniconda](https://docs.conda.io/projects/miniconda/en/latest/index.html).
-
-Download and unzip the [*BenchNIRS* repository](https://gitlab.com/HanBnrd/benchnirs/-/archive/main/benchnirs-main.zip).
-
-In a terminal or command prompt (eg. Anaconda Prompt), navigate to the directory containing the `requirements.txt` file and run:
+## Keeping *BenchNIRS* up to date
+To update *BenchNIRS* to the latest version with *pip*, open a terminal (eg. Anaconda Prompt) and type:
 ```bash
-python -m pip install -r requirements.txt -f https://download.pytorch.org/whl/torch_stable.html
+pip install --upgrade benchnirs
 ```
 
-> Alternatively, the *BenchNIRS* library containing the core functions (without main scripts) is available on [PyPI](https://pypi.org/project/benchnirs/) and can be installed using `pip`:
-> ```bash
-> pip install benchnirs
-> ```
-> and updated to the newest version with:
-> ```bash
-> pip install --upgrade benchnirs
-> ```
-
-
-## Running main scripts
-- [`generalised.py`](https://gitlab.com/HanBnrd/benchnirs/-/blob/main/src/generalised.py) compares the 6 models (LDA, SVC, kNN, ANN, CNN and LSTM) on the 5 datasets with a generalised approach (testing with unseen subjects)
-- [`dataset_size.py`](https://gitlab.com/HanBnrd/benchnirs/-/blob/main/src/dataset_size.py) reproduces `generalised.py` but with a range of different dataset sizes (50% to 100% of dataset) to study the influence of this parameter on the classification accuracy
-- [`window_size.py`](https://gitlab.com/HanBnrd/benchnirs/-/blob/main/src/window_size.py) reproduces `generalised.py` but with only the 4 models using feature extraction (LDA, SVC, kNN and ANN) and with a range of different window sizes (2 to 10 seconds) to study the influence of this parameter on the classification accuracy
-- [`sliding_window.py`](https://gitlab.com/HanBnrd/benchnirs/-/blob/main/src/sliding_window.py) reproduces `generalised.py` but with only the 4 models using feature extraction (LDA, SVC, kNN and ANN) and with a 2-second sliding window on the 10-second epochs
-- [`personalised.py`](https://gitlab.com/HanBnrd/benchnirs/-/blob/main/src/personalised.py) compares the 6 models (LDA, SVC, kNN, ANN, CNN and LSTM) on the 5 datasets with a personalised approach (training and testing with each subject individually)
-- [`visualisation.py`](https://gitlab.com/HanBnrd/benchnirs/-/blob/main/src/visualisation.py) enables to visualise the data from the datasets with various signal processing
-
 
 ## Example
-An example script showing how to use the framework with a custom deep learning model can be found [here](https://hanbnrd.gitlab.io/benchnirs/example.html).
+A full example script showing how to use the framework with a custom deep learning model can be found [here](https://hanbnrd.gitlab.io/benchnirs/example.html).
 
 
 ## Simple use case
 *BenchNIRS* enables to evaluate your model in Python with simplicity on an open access dataset supported:
 ```python
 import benchnirs as bn
 
@@ -103,29 +97,38 @@
 data = bn.process_epochs(epochs['0-back', '2-back', '3-back'])
 results = bn.deep_learn(*data, my_model)
 
 print(results)
 ```
 
 
+## Running main scripts
+- [`generalised.py`](https://gitlab.com/HanBnrd/benchnirs/-/blob/main/src/generalised.py) compares the 6 models (LDA, SVC, kNN, ANN, CNN and LSTM) on the 5 datasets with a generalised approach (testing with unseen subjects)
+- [`dataset_size.py`](https://gitlab.com/HanBnrd/benchnirs/-/blob/main/src/dataset_size.py) reproduces `generalised.py` but with a range of different dataset sizes (50% to 100% of dataset) to study the influence of this parameter on the classification accuracy
+- [`window_size.py`](https://gitlab.com/HanBnrd/benchnirs/-/blob/main/src/window_size.py) reproduces `generalised.py` but with only the 4 models using feature extraction (LDA, SVC, kNN and ANN) and with a range of different window sizes (2 to 10 seconds) to study the influence of this parameter on the classification accuracy
+- [`sliding_window.py`](https://gitlab.com/HanBnrd/benchnirs/-/blob/main/src/sliding_window.py) reproduces `generalised.py` but with only the 4 models using feature extraction (LDA, SVC, kNN and ANN) and with a 2-second sliding window on the 10-second epochs
+- [`personalised.py`](https://gitlab.com/HanBnrd/benchnirs/-/blob/main/src/personalised.py) compares the 6 models (LDA, SVC, kNN, ANN, CNN and LSTM) on the 5 datasets with a personalised approach (training and testing with each subject individually)
+- [`visualisation.py`](https://gitlab.com/HanBnrd/benchnirs/-/blob/main/src/visualisation.py) enables to visualise the data from the datasets with various signal processing
+
+
 ## Extra scripts: n-back tailored
 - `tailored_generalised.py` compares the 6 models (LDA, SVC, kNN, ANN, CNN and LSTM) on the 2 n-back datasets with a generalised approach (testing with unseen subjects)
 - `tailored_window_size.py` reproduces `tailored_generalised.py` but with only 5 models (LDA, SVC, kNN, ANN and LSTM) and with a range of different window sizes (5 to 40 seconds) to study the influence of this parameter on the classification accuracy
 - `tailored_shin_nb.py` optimises and evaluates a tailored CNN on the *Shin et al. 2018* n-back dataset with a generalised approach (testing with unseen subjects)
 
 
 ## Extra scripts: transfer learning
 - `transfer.py` optimises and evaluates a transfer learning model (pretext self-supervised representation learning task with unlabelled and labelled data using a CED, downstream supervised n-back classification task with labelled data) on the *Shin et al. 2018* n-back dataset with a generalised approach (testing with unseen subjects)
 - `transfer_no_unlab.py` reproduces `transfer.py` but with only labelled data for the pretext task.
 
 
 ## Contributing to the repository
 Contributions from the community to this repository are highly appreciated. We are mainly interested in contributions to:
 - improving the recommendation checklist
-- adding support for new **open access datasets**
+- adding support for new open access datasets
 - adding support for new machine learning models
 - adding more fNIRS signal processing techniques
 - improving the documentation
 - tracking bugs
 
 Contributions are encouraged under the form of [issues](https://gitlab.com/HanBnrd/benchnirs/-/issues) (for reporting bugs or requesting new features) and [merge requests](https://gitlab.com/HanBnrd/benchnirs/-/merge_requests) (for fixing bugs and implementing new features).
 Please refer to [this tutorial](https://docs.gitlab.com/ee/user/project/repository/forking_workflow.html) for creating merge requests from a fork of the repository.
```

### Comparing `benchnirs-1.2.0/setup.py` & `benchnirs-1.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="benchnirs",
-    version="1.2.0",
+    version="1.2.1",
     author="Johann Benerradi",
     author_email="johann.benerradi@gmail.com",
     description="Benchmarking framework for machine learning with fNIRS",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.com/HanBnrd/benchnirs",
     license='GNU GPLv3+',
```

### Comparing `benchnirs-1.2.0/src/benchnirs/learn.py` & `benchnirs-1.2.1/src/benchnirs/learn.py`

 * *Files identical despite different names*

### Comparing `benchnirs-1.2.0/src/benchnirs/load.py` & `benchnirs-1.2.1/src/benchnirs/load.py`

 * *Files identical despite different names*

### Comparing `benchnirs-1.2.0/src/benchnirs/process.py` & `benchnirs-1.2.1/src/benchnirs/process.py`

 * *Files identical despite different names*

### Comparing `benchnirs-1.2.0/src/benchnirs/viz.py` & `benchnirs-1.2.1/src/benchnirs/viz.py`

 * *Files identical despite different names*

### Comparing `benchnirs-1.2.0/src/benchnirs.egg-info/PKG-INFO` & `benchnirs-1.2.1/src/benchnirs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: benchnirs
-Version: 1.2.0
+Version: 1.2.1
 Summary: Benchmarking framework for machine learning with fNIRS
 Home-page: https://gitlab.com/HanBnrd/benchnirs
 Author: Johann Benerradi
 Author-email: johann.benerradi@gmail.com
 License: GNU GPLv3+
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -66,52 +66,46 @@
 - [scikit-learn 0.24](https://scikit-learn.org/stable/install.html)
 - [scipy 1.8](https://scipy.org/install/)
 - [seaborn 0.11](https://seaborn.pydata.org/installing.html)
 - [statsmodels 0.12.2](https://www.statsmodels.org/dev/install.html)
 - [torch 1.5](https://pytorch.org/get-started/locally/)
 
 
+## Setting up *BenchNIRS*
+1. Download and install Python 3.8 or greater, for example with [Miniconda](https://docs.conda.io/projects/miniconda/en/latest/index.html).
+
+2. To install the package with *pip* (cf. [PyPI](https://pypi.org/project/benchnirs/)), open a terminal (eg. Anaconda Prompt) and type:
+```bash
+pip install benchnirs
+```
+> Alternatively to install from source, download and unzip the [repository](https://gitlab.com/HanBnrd/benchnirs/-/archive/main/benchnirs-main.zip).
+> Then, in a terminal or command prompt (eg. Anaconda Prompt), navigate to the directory containing the `requirements.txt` file and run:
+> ```bash
+> python -m pip install -r requirements.txt -f https://download.pytorch.org/whl/torch_stable.html
+> ```
+
+3. Download the datasets (see below).
+
+
 ## Downloading the datasets
 - *Herff et al. 2014* (n-back task): you can download the dataset by making a request [here](http://www.csl.uni-bremen.de/CorpusData/download.php?crps=fNIRS). In the examples, the unzipped folder has been renamed to *dataset_herff_2014* for convenience.
 - *Shin et al. 2018* (n-back and word generation tasks): you can download the dataset [here](http://doc.ml.tu-berlin.de/simultaneous_EEG_NIRS/NIRS/NIRS_01-26_MATLAB.zip). In the examples, the unzipped folder has been renamed to *dataset_shin_2018* for convenience.
 - *Shin et al. 2016* (mental arithmetic task): you can download the dataset by filling the form [here](http://doc.ml.tu-berlin.de/hBCI). Then click on *NIRS_01-29* to download the fNIRS data. In the examples, the unzipped folder has been renamed to *dataset_shin_2016* for convenience.
 - *Bak et al. 2019* (motor execution task): you can download the dataset [here](https://figshare.com/ndownloader/files/18069143). In the examples, the unzipped folder has been renamed to *dataset_bak_2019* for convenience.
 
 
-## Setup
-Download and install Python 3.8 or greater, for example with [Miniconda](https://docs.conda.io/projects/miniconda/en/latest/index.html).
-
-Download and unzip the [*BenchNIRS* repository](https://gitlab.com/HanBnrd/benchnirs/-/archive/main/benchnirs-main.zip).
-
-In a terminal or command prompt (eg. Anaconda Prompt), navigate to the directory containing the `requirements.txt` file and run:
+## Keeping *BenchNIRS* up to date
+To update *BenchNIRS* to the latest version with *pip*, open a terminal (eg. Anaconda Prompt) and type:
 ```bash
-python -m pip install -r requirements.txt -f https://download.pytorch.org/whl/torch_stable.html
+pip install --upgrade benchnirs
 ```
 
-> Alternatively, the *BenchNIRS* library containing the core functions (without main scripts) is available on [PyPI](https://pypi.org/project/benchnirs/) and can be installed using `pip`:
-> ```bash
-> pip install benchnirs
-> ```
-> and updated to the newest version with:
-> ```bash
-> pip install --upgrade benchnirs
-> ```
-
-
-## Running main scripts
-- [`generalised.py`](https://gitlab.com/HanBnrd/benchnirs/-/blob/main/src/generalised.py) compares the 6 models (LDA, SVC, kNN, ANN, CNN and LSTM) on the 5 datasets with a generalised approach (testing with unseen subjects)
-- [`dataset_size.py`](https://gitlab.com/HanBnrd/benchnirs/-/blob/main/src/dataset_size.py) reproduces `generalised.py` but with a range of different dataset sizes (50% to 100% of dataset) to study the influence of this parameter on the classification accuracy
-- [`window_size.py`](https://gitlab.com/HanBnrd/benchnirs/-/blob/main/src/window_size.py) reproduces `generalised.py` but with only the 4 models using feature extraction (LDA, SVC, kNN and ANN) and with a range of different window sizes (2 to 10 seconds) to study the influence of this parameter on the classification accuracy
-- [`sliding_window.py`](https://gitlab.com/HanBnrd/benchnirs/-/blob/main/src/sliding_window.py) reproduces `generalised.py` but with only the 4 models using feature extraction (LDA, SVC, kNN and ANN) and with a 2-second sliding window on the 10-second epochs
-- [`personalised.py`](https://gitlab.com/HanBnrd/benchnirs/-/blob/main/src/personalised.py) compares the 6 models (LDA, SVC, kNN, ANN, CNN and LSTM) on the 5 datasets with a personalised approach (training and testing with each subject individually)
-- [`visualisation.py`](https://gitlab.com/HanBnrd/benchnirs/-/blob/main/src/visualisation.py) enables to visualise the data from the datasets with various signal processing
-
 
 ## Example
-An example script showing how to use the framework with a custom deep learning model can be found [here](https://hanbnrd.gitlab.io/benchnirs/example.html).
+A full example script showing how to use the framework with a custom deep learning model can be found [here](https://hanbnrd.gitlab.io/benchnirs/example.html).
 
 
 ## Simple use case
 *BenchNIRS* enables to evaluate your model in Python with simplicity on an open access dataset supported:
 ```python
 import benchnirs as bn
 
@@ -119,29 +113,38 @@
 data = bn.process_epochs(epochs['0-back', '2-back', '3-back'])
 results = bn.deep_learn(*data, my_model)
 
 print(results)
 ```
 
 
+## Running main scripts
+- [`generalised.py`](https://gitlab.com/HanBnrd/benchnirs/-/blob/main/src/generalised.py) compares the 6 models (LDA, SVC, kNN, ANN, CNN and LSTM) on the 5 datasets with a generalised approach (testing with unseen subjects)
+- [`dataset_size.py`](https://gitlab.com/HanBnrd/benchnirs/-/blob/main/src/dataset_size.py) reproduces `generalised.py` but with a range of different dataset sizes (50% to 100% of dataset) to study the influence of this parameter on the classification accuracy
+- [`window_size.py`](https://gitlab.com/HanBnrd/benchnirs/-/blob/main/src/window_size.py) reproduces `generalised.py` but with only the 4 models using feature extraction (LDA, SVC, kNN and ANN) and with a range of different window sizes (2 to 10 seconds) to study the influence of this parameter on the classification accuracy
+- [`sliding_window.py`](https://gitlab.com/HanBnrd/benchnirs/-/blob/main/src/sliding_window.py) reproduces `generalised.py` but with only the 4 models using feature extraction (LDA, SVC, kNN and ANN) and with a 2-second sliding window on the 10-second epochs
+- [`personalised.py`](https://gitlab.com/HanBnrd/benchnirs/-/blob/main/src/personalised.py) compares the 6 models (LDA, SVC, kNN, ANN, CNN and LSTM) on the 5 datasets with a personalised approach (training and testing with each subject individually)
+- [`visualisation.py`](https://gitlab.com/HanBnrd/benchnirs/-/blob/main/src/visualisation.py) enables to visualise the data from the datasets with various signal processing
+
+
 ## Extra scripts: n-back tailored
 - `tailored_generalised.py` compares the 6 models (LDA, SVC, kNN, ANN, CNN and LSTM) on the 2 n-back datasets with a generalised approach (testing with unseen subjects)
 - `tailored_window_size.py` reproduces `tailored_generalised.py` but with only 5 models (LDA, SVC, kNN, ANN and LSTM) and with a range of different window sizes (5 to 40 seconds) to study the influence of this parameter on the classification accuracy
 - `tailored_shin_nb.py` optimises and evaluates a tailored CNN on the *Shin et al. 2018* n-back dataset with a generalised approach (testing with unseen subjects)
 
 
 ## Extra scripts: transfer learning
 - `transfer.py` optimises and evaluates a transfer learning model (pretext self-supervised representation learning task with unlabelled and labelled data using a CED, downstream supervised n-back classification task with labelled data) on the *Shin et al. 2018* n-back dataset with a generalised approach (testing with unseen subjects)
 - `transfer_no_unlab.py` reproduces `transfer.py` but with only labelled data for the pretext task.
 
 
 ## Contributing to the repository
 Contributions from the community to this repository are highly appreciated. We are mainly interested in contributions to:
 - improving the recommendation checklist
-- adding support for new **open access datasets**
+- adding support for new open access datasets
 - adding support for new machine learning models
 - adding more fNIRS signal processing techniques
 - improving the documentation
 - tracking bugs
 
 Contributions are encouraged under the form of [issues](https://gitlab.com/HanBnrd/benchnirs/-/issues) (for reporting bugs or requesting new features) and [merge requests](https://gitlab.com/HanBnrd/benchnirs/-/merge_requests) (for fixing bugs and implementing new features).
 Please refer to [this tutorial](https://docs.gitlab.com/ee/user/project/repository/forking_workflow.html) for creating merge requests from a fork of the repository.
```

