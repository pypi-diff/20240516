# Comparing `tmp/prmllab-0.1.tar.gz` & `tmp/prmllab-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prmllab-0.1.tar", last modified: Wed May 15 16:22:12 2024, max compression
+gzip compressed data, was "prmllab-0.2.tar", last modified: Wed May 15 17:22:38 2024, max compression
```

## Comparing `prmllab-0.1.tar` & `prmllab-0.2.tar`

### file list

```diff
@@ -1,12 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 16:22:12.589358 prmllab-0.1/
--rw-rw-rw-   0        0        0       52 2024-05-15 16:22:12.585026 prmllab-0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-15 16:22:12.462443 prmllab-0.1/prmllab/
--rw-rw-rw-   0        0        0        0 2024-05-15 15:55:27.000000 prmllab-0.1/prmllab/__init__.py
--rw-rw-rw-   0        0        0      834 2024-05-15 15:57:22.000000 prmllab-0.1/prmllab/functions.py
-drwxrwxrwx   0        0        0        0 2024-05-15 16:22:12.581706 prmllab-0.1/prmllab.egg-info/
--rw-rw-rw-   0        0        0       52 2024-05-15 16:22:12.000000 prmllab-0.1/prmllab.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      173 2024-05-15 16:22:12.000000 prmllab-0.1/prmllab.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 16:22:12.000000 prmllab-0.1/prmllab.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-05-15 16:22:12.000000 prmllab-0.1/prmllab.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-15 16:22:12.589358 prmllab-0.1/setup.cfg
--rw-rw-rw-   0        0        0      217 2024-05-15 16:21:58.000000 prmllab-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 17:22:38.190824 prmllab-0.2/
+-rw-rw-rw-   0        0        0       52 2024-05-15 17:22:38.186820 prmllab-0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-15 17:22:38.133993 prmllab-0.2/prmllab/
+-rw-rw-rw-   0        0        0   172797 2024-05-15 14:12:04.000000 prmllab-0.2/prmllab/Bagging.ipynb
+-rw-rw-rw-   0        0        0   263198 2024-05-15 14:29:44.000000 prmllab-0.2/prmllab/Regression.ipynb
+-rw-rw-rw-   0        0        0        0 2024-05-15 15:55:27.000000 prmllab-0.2/prmllab/__init__.py
+-rw-rw-rw-   0        0        0      834 2024-05-15 15:57:22.000000 prmllab-0.2/prmllab/functions.py
+-rw-rw-rw-   0        0        0   198851 2024-05-15 14:36:22.000000 prmllab-0.2/prmllab/kmeans.ipynb
+-rw-rw-rw-   0        0        0   187775 2024-05-15 14:37:14.000000 prmllab-0.2/prmllab/mlp.ipynb
+-rw-rw-rw-   0        0        0     2547 2024-05-15 14:37:28.000000 prmllab-0.2/prmllab/naive.ipynb
+-rw-rw-rw-   0        0        0   532184 2024-05-15 16:12:36.000000 prmllab-0.2/prmllab/prml.zip
+drwxrwxrwx   0        0        0        0 2024-05-15 17:22:38.183269 prmllab-0.2/prmllab.egg-info/
+-rw-rw-rw-   0        0        0       52 2024-05-15 17:22:37.000000 prmllab-0.2/prmllab.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      296 2024-05-15 17:22:37.000000 prmllab-0.2/prmllab.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 17:22:37.000000 prmllab-0.2/prmllab.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-05-15 17:22:37.000000 prmllab-0.2/prmllab.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-15 17:22:38.191822 prmllab-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      216 2024-05-15 17:22:30.000000 prmllab-0.2/setup.py
```

### Comparing `prmllab-0.1/prmllab/functions.py` & `prmllab-0.2/prmllab/functions.py`

 * *Files identical despite different names*

