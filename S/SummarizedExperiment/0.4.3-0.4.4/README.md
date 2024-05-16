# Comparing `tmp/SummarizedExperiment-0.4.3.tar.gz` & `tmp/summarizedexperiment-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SummarizedExperiment-0.4.3.tar", last modified: Tue Feb 13 21:45:05 2024, max compression
+gzip compressed data, was "summarizedexperiment-0.4.4.tar", last modified: Thu May 16 15:20:47 2024, max compression
```

## Comparing `SummarizedExperiment-0.4.3.tar` & `summarizedexperiment-0.4.4.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 21:45:05.782173 SummarizedExperiment-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-02-13 21:43:54.000000 SummarizedExperiment-0.4.3/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 21:45:05.766174 SummarizedExperiment-0.4.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 21:45:05.770174 SummarizedExperiment-0.4.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-02-13 21:43:54.000000 SummarizedExperiment-0.4.3/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-02-13 21:43:54.000000 SummarizedExperiment-0.4.3/.github/workflows/pypi-test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-02-13 21:43:54.000000 SummarizedExperiment-0.4.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-02-13 21:43:54.000000 SummarizedExperiment-0.4.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-02-13 21:43:54.000000 SummarizedExperiment-0.4.3/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-02-13 21:43:54.000000 SummarizedExperiment-0.4.3/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)     3664 2024-02-13 21:43:54.000000 SummarizedExperiment-0.4.3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)    13646 2024-02-13 21:43:54.000000 SummarizedExperiment-0.4.3/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-02-13 21:43:54.000000 SummarizedExperiment-0.4.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4148 2024-02-13 21:45:05.782173 SummarizedExperiment-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3012 2024-02-13 21:43:54.000000 SummarizedExperiment-0.4.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 21:45:05.774174 SummarizedExperiment-0.4.3/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-02-13 21:43:54.000000 SummarizedExperiment-0.4.3/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 21:45:05.774174 SummarizedExperiment-0.4.3/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-02-13 21:43:54.000000 SummarizedExperiment-0.4.3/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-02-13 21:43:54.000000 SummarizedExperiment-0.4.3/docs/authors.md
--rw-r--r--   0 runner    (1001) docker     (127)     3664 2024-02-13 21:43:54.000000 SummarizedExperiment-0.4.3/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)    10478 2024-02-13 21:43:54.000000 SummarizedExperiment-0.4.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-02-13 21:43:54.000000 SummarizedExperiment-0.4.3/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-02-13 21:43:54.000000 SummarizedExperiment-0.4.3/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-02-13 21:43:54.000000 SummarizedExperiment-0.4.3/docs/license.md
--rw-r--r--   0 runner    (1001) docker     (127)     3012 2024-02-13 21:43:54.000000 SummarizedExperiment-0.4.3/docs/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-02-13 21:43:54.000000 SummarizedExperiment-0.4.3/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     7586 2024-02-13 21:43:54.000000 SummarizedExperiment-0.4.3/docs/tutorial.md
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-02-13 21:43:54.000000 SummarizedExperiment-0.4.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1501 2024-02-13 21:45:05.782173 SummarizedExperiment-0.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-02-13 21:43:54.000000 SummarizedExperiment-0.4.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 21:45:05.766174 SummarizedExperiment-0.4.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 21:45:05.778174 SummarizedExperiment-0.4.3/src/SummarizedExperiment.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4148 2024-02-13 21:45:05.000000 SummarizedExperiment-0.4.3/src/SummarizedExperiment.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-02-13 21:45:05.000000 SummarizedExperiment-0.4.3/src/SummarizedExperiment.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-13 21:45:05.000000 SummarizedExperiment-0.4.3/src/SummarizedExperiment.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-13 21:44:04.000000 SummarizedExperiment-0.4.3/src/SummarizedExperiment.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-02-13 21:45:05.000000 SummarizedExperiment-0.4.3/src/SummarizedExperiment.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-02-13 21:45:05.000000 SummarizedExperiment-0.4.3/src/SummarizedExperiment.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 21:45:05.774174 SummarizedExperiment-0.4.3/src/summarizedexperiment/
--rw-r--r--   0 runner    (1001) docker     (127)    39580 2024-02-13 21:43:54.000000 SummarizedExperiment-0.4.3/src/summarizedexperiment/BaseSE.py
--rw-r--r--   0 runner    (1001) docker     (127)    36198 2024-02-13 21:43:54.000000 SummarizedExperiment-0.4.3/src/summarizedexperiment/RangedSummarizedExperiment.py
--rw-r--r--   0 runner    (1001) docker     (127)     8461 2024-02-13 21:43:54.000000 SummarizedExperiment-0.4.3/src/summarizedexperiment/SummarizedExperiment.py
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-02-13 21:43:54.000000 SummarizedExperiment-0.4.3/src/summarizedexperiment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-02-13 21:43:54.000000 SummarizedExperiment-0.4.3/src/summarizedexperiment/_combineutils.py
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-02-13 21:43:54.000000 SummarizedExperiment-0.4.3/src/summarizedexperiment/_frameutils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-02-13 21:43:54.000000 SummarizedExperiment-0.4.3/src/summarizedexperiment/type_checks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 21:45:05.778174 SummarizedExperiment-0.4.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-02-13 21:43:54.000000 SummarizedExperiment-0.4.3/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 21:45:05.778174 SummarizedExperiment-0.4.3/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)     8414 2024-02-13 21:43:54.000000 SummarizedExperiment-0.4.3/tests/data/summarized_experiments.py
--rw-r--r--   0 runner    (1001) docker     (127)   986863 2024-02-13 21:43:54.000000 SummarizedExperiment-0.4.3/tests/data/tenx.sub.h5
--rw-r--r--   0 runner    (1001) docker     (127)     3277 2024-02-13 21:43:54.000000 SummarizedExperiment-0.4.3/tests/test_RSE.py
--rw-r--r--   0 runner    (1001) docker     (127)     4762 2024-02-13 21:43:54.000000 SummarizedExperiment-0.4.3/tests/test_RSE_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)     5501 2024-02-13 21:43:54.000000 SummarizedExperiment-0.4.3/tests/test_SE.py
--rw-r--r--   0 runner    (1001) docker     (127)     3870 2024-02-13 21:43:54.000000 SummarizedExperiment-0.4.3/tests/test_SE_combine_cols.py
--rw-r--r--   0 runner    (1001) docker     (127)     3609 2024-02-13 21:43:54.000000 SummarizedExperiment-0.4.3/tests/test_SE_combine_rows.py
--rw-r--r--   0 runner    (1001) docker     (127)     2431 2024-02-13 21:43:54.000000 SummarizedExperiment-0.4.3/tests/test_SE_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)     6837 2024-02-13 21:43:54.000000 SummarizedExperiment-0.4.3/tests/test_SE_subset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2241 2024-02-13 21:43:54.000000 SummarizedExperiment-0.4.3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:20:47.640710 summarizedexperiment-0.4.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-16 15:19:39.000000 summarizedexperiment-0.4.4/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:20:47.624710 summarizedexperiment-0.4.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:20:47.628710 summarizedexperiment-0.4.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-05-16 15:19:39.000000 summarizedexperiment-0.4.4/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-16 15:19:39.000000 summarizedexperiment-0.4.4/.github/workflows/pypi-test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-05-16 15:19:39.000000 summarizedexperiment-0.4.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-16 15:19:39.000000 summarizedexperiment-0.4.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-16 15:19:39.000000 summarizedexperiment-0.4.4/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-16 15:19:39.000000 summarizedexperiment-0.4.4/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3664 2024-05-16 15:19:39.000000 summarizedexperiment-0.4.4/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)    13646 2024-05-16 15:19:39.000000 summarizedexperiment-0.4.4/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-16 15:19:39.000000 summarizedexperiment-0.4.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4149 2024-05-16 15:20:47.640710 summarizedexperiment-0.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3012 2024-05-16 15:19:39.000000 summarizedexperiment-0.4.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:20:47.632710 summarizedexperiment-0.4.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-16 15:19:39.000000 summarizedexperiment-0.4.4/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:20:47.632710 summarizedexperiment-0.4.4/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-16 15:19:39.000000 summarizedexperiment-0.4.4/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-16 15:19:39.000000 summarizedexperiment-0.4.4/docs/authors.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3664 2024-05-16 15:19:39.000000 summarizedexperiment-0.4.4/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10478 2024-05-16 15:19:39.000000 summarizedexperiment-0.4.4/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-16 15:19:39.000000 summarizedexperiment-0.4.4/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-05-16 15:19:39.000000 summarizedexperiment-0.4.4/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-16 15:19:39.000000 summarizedexperiment-0.4.4/docs/license.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3012 2024-05-16 15:19:39.000000 summarizedexperiment-0.4.4/docs/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-16 15:19:39.000000 summarizedexperiment-0.4.4/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     7586 2024-05-16 15:19:39.000000 summarizedexperiment-0.4.4/docs/tutorial.md
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-16 15:19:39.000000 summarizedexperiment-0.4.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-05-16 15:20:47.640710 summarizedexperiment-0.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-16 15:19:39.000000 summarizedexperiment-0.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:20:47.624710 summarizedexperiment-0.4.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:20:47.636710 summarizedexperiment-0.4.4/src/SummarizedExperiment.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4149 2024-05-16 15:20:47.000000 summarizedexperiment-0.4.4/src/SummarizedExperiment.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-05-16 15:20:47.000000 summarizedexperiment-0.4.4/src/SummarizedExperiment.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 15:20:47.000000 summarizedexperiment-0.4.4/src/SummarizedExperiment.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 15:19:46.000000 summarizedexperiment-0.4.4/src/SummarizedExperiment.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-16 15:20:47.000000 summarizedexperiment-0.4.4/src/SummarizedExperiment.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-16 15:20:47.000000 summarizedexperiment-0.4.4/src/SummarizedExperiment.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:20:47.632710 summarizedexperiment-0.4.4/src/summarizedexperiment/
+-rw-r--r--   0 runner    (1001) docker     (127)    39877 2024-05-16 15:19:39.000000 summarizedexperiment-0.4.4/src/summarizedexperiment/BaseSE.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36198 2024-05-16 15:19:39.000000 summarizedexperiment-0.4.4/src/summarizedexperiment/RangedSummarizedExperiment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8461 2024-05-16 15:19:39.000000 summarizedexperiment-0.4.4/src/summarizedexperiment/SummarizedExperiment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-05-16 15:19:39.000000 summarizedexperiment-0.4.4/src/summarizedexperiment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-05-16 15:19:39.000000 summarizedexperiment-0.4.4/src/summarizedexperiment/_combineutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-16 15:19:39.000000 summarizedexperiment-0.4.4/src/summarizedexperiment/_frameutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-05-16 15:19:39.000000 summarizedexperiment-0.4.4/src/summarizedexperiment/type_checks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:20:47.636710 summarizedexperiment-0.4.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-16 15:19:39.000000 summarizedexperiment-0.4.4/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:20:47.636710 summarizedexperiment-0.4.4/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     8414 2024-05-16 15:19:39.000000 summarizedexperiment-0.4.4/tests/data/summarized_experiments.py
+-rw-r--r--   0 runner    (1001) docker     (127)   986863 2024-05-16 15:19:39.000000 summarizedexperiment-0.4.4/tests/data/tenx.sub.h5
+-rw-r--r--   0 runner    (1001) docker     (127)     3277 2024-05-16 15:19:39.000000 summarizedexperiment-0.4.4/tests/test_RSE.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4762 2024-05-16 15:19:39.000000 summarizedexperiment-0.4.4/tests/test_RSE_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5501 2024-05-16 15:19:39.000000 summarizedexperiment-0.4.4/tests/test_SE.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3870 2024-05-16 15:19:39.000000 summarizedexperiment-0.4.4/tests/test_SE_combine_cols.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3609 2024-05-16 15:19:39.000000 summarizedexperiment-0.4.4/tests/test_SE_combine_rows.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2431 2024-05-16 15:19:39.000000 summarizedexperiment-0.4.4/tests/test_SE_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6837 2024-05-16 15:19:39.000000 summarizedexperiment-0.4.4/tests/test_SE_subset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2241 2024-05-16 15:19:39.000000 summarizedexperiment-0.4.4/tox.ini
```

### Comparing `SummarizedExperiment-0.4.3/.coveragerc` & `summarizedexperiment-0.4.4/.coveragerc`

 * *Files identical despite different names*

### Comparing `SummarizedExperiment-0.4.3/.github/workflows/pypi-publish.yml` & `summarizedexperiment-0.4.4/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `SummarizedExperiment-0.4.3/.github/workflows/pypi-test.yml` & `summarizedexperiment-0.4.4/.github/workflows/pypi-test.yml`

 * *Files identical despite different names*

### Comparing `SummarizedExperiment-0.4.3/.gitignore` & `summarizedexperiment-0.4.4/.gitignore`

 * *Files identical despite different names*

### Comparing `SummarizedExperiment-0.4.3/.pre-commit-config.yaml` & `summarizedexperiment-0.4.4/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 exclude: '^docs/conf.py'
 
 repos:
 - repo: https://github.com/pre-commit/pre-commit-hooks
-  rev: v4.5.0
+  rev: v4.6.0
   hooks:
   - id: trailing-whitespace
   - id: check-added-large-files
   - id: check-ast
   - id: check-json
   - id: check-merge-conflict
   - id: check-xml
@@ -22,22 +22,22 @@
   hooks:
     - id: docformatter
       additional_dependencies: [tomli]
       args: [--in-place, --wrap-descriptions=120, --wrap-summaries=120]
       # --config, ./pyproject.toml
 
 - repo: https://github.com/psf/black
-  rev: 24.1.1
+  rev: 24.4.0
   hooks:
   - id: black
     language_version: python3
 
 - repo: https://github.com/astral-sh/ruff-pre-commit
   # Ruff version.
-  rev: v0.2.1
+  rev: v0.3.7
   hooks:
     - id: ruff
       args: [--fix, --exit-non-zero-on-fix]
 
 ## If like to embrace black styles even in the docs:
 # - repo: https://github.com/asottile/blacken-docs
 #   rev: v1.13.0
```

### Comparing `SummarizedExperiment-0.4.3/CHANGELOG.md` & `summarizedexperiment-0.4.4/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `SummarizedExperiment-0.4.3/CONTRIBUTING.md` & `summarizedexperiment-0.4.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `SummarizedExperiment-0.4.3/LICENSE.txt` & `summarizedexperiment-0.4.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `SummarizedExperiment-0.4.3/PKG-INFO` & `summarizedexperiment-0.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: SummarizedExperiment
-Version: 0.4.3
+Version: 0.4.4
 Summary: Container to represent data from genomic experiments
 Home-page: https://github.com/BiocPy/summarizedexperiment
 Author: jkanche
 Author-email: jayaram.kancherla@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/BiocPy/summarizedexperiment
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 License-File: LICENSE.txt
 Requires-Dist: importlib-metadata; python_version < "3.8"
 Requires-Dist: genomicranges<0.5.0,>=0.4.4
-Requires-Dist: biocframe<0.6.0,>=0.5.4
+Requires-Dist: biocframe<0.6.0,>=0.5.10
 Requires-Dist: biocutils<0.2.0,>=0.1.4
 Provides-Extra: optional
 Requires-Dist: anndata; extra == "optional"
 Requires-Dist: scipy; extra == "optional"
 Requires-Dist: delayedarray; extra == "optional"
 Provides-Extra: testing
 Requires-Dist: setuptools; extra == "testing"
```

### Comparing `SummarizedExperiment-0.4.3/README.md` & `summarizedexperiment-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `SummarizedExperiment-0.4.3/docs/Makefile` & `summarizedexperiment-0.4.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `SummarizedExperiment-0.4.3/docs/changelog.md` & `summarizedexperiment-0.4.4/docs/changelog.md`

 * *Files identical despite different names*

### Comparing `SummarizedExperiment-0.4.3/docs/conf.py` & `summarizedexperiment-0.4.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `SummarizedExperiment-0.4.3/docs/index.md` & `summarizedexperiment-0.4.4/docs/index.md`

 * *Files identical despite different names*

### Comparing `SummarizedExperiment-0.4.3/docs/readme.md` & `summarizedexperiment-0.4.4/docs/readme.md`

 * *Files identical despite different names*

### Comparing `SummarizedExperiment-0.4.3/docs/tutorial.md` & `summarizedexperiment-0.4.4/docs/tutorial.md`

 * *Files identical despite different names*

### Comparing `SummarizedExperiment-0.4.3/pyproject.toml` & `summarizedexperiment-0.4.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `SummarizedExperiment-0.4.3/setup.cfg` & `summarizedexperiment-0.4.4/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 include_package_data = True
 package_dir = 
 	=src
 python_requires = >=3.8
 install_requires = 
 	importlib-metadata; python_version<"3.8"
 	genomicranges>=0.4.4,<0.5.0
-	biocframe>=0.5.4,<0.6.0
+	biocframe>=0.5.10,<0.6.0
 	biocutils>=0.1.4,<0.2.0
 
 [options.packages.find]
 where = src
 exclude = 
 	tests
```

### Comparing `SummarizedExperiment-0.4.3/setup.py` & `summarizedexperiment-0.4.4/setup.py`

 * *Files identical despite different names*

### Comparing `SummarizedExperiment-0.4.3/src/SummarizedExperiment.egg-info/PKG-INFO` & `summarizedexperiment-0.4.4/src/SummarizedExperiment.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: SummarizedExperiment
-Version: 0.4.3
+Version: 0.4.4
 Summary: Container to represent data from genomic experiments
 Home-page: https://github.com/BiocPy/summarizedexperiment
 Author: jkanche
 Author-email: jayaram.kancherla@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/BiocPy/summarizedexperiment
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 License-File: LICENSE.txt
 Requires-Dist: importlib-metadata; python_version < "3.8"
 Requires-Dist: genomicranges<0.5.0,>=0.4.4
-Requires-Dist: biocframe<0.6.0,>=0.5.4
+Requires-Dist: biocframe<0.6.0,>=0.5.10
 Requires-Dist: biocutils<0.2.0,>=0.1.4
 Provides-Extra: optional
 Requires-Dist: anndata; extra == "optional"
 Requires-Dist: scipy; extra == "optional"
 Requires-Dist: delayedarray; extra == "optional"
 Provides-Extra: testing
 Requires-Dist: setuptools; extra == "testing"
```

### Comparing `SummarizedExperiment-0.4.3/src/SummarizedExperiment.egg-info/SOURCES.txt` & `summarizedexperiment-0.4.4/src/SummarizedExperiment.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SummarizedExperiment-0.4.3/src/summarizedexperiment/BaseSE.py` & `summarizedexperiment-0.4.4/src/summarizedexperiment/BaseSE.py`

 * *Files 0% similar despite different names*

```diff
@@ -1178,36 +1178,42 @@
 
         Returns:
             An ``AnnData`` representation of the experiment.
         """
         from anndata import AnnData
         from delayedarray import (
             DelayedArray,
-            to_scipy_sparse_matrix,
-            to_dense_array,
             is_sparse,
+            to_dense_array,
+            to_scipy_sparse_matrix,
         )
 
         layers = OrderedDict()
         for asy, mat in self.assays.items():
             if isinstance(mat, DelayedArray) or issubclass(type(mat), DelayedArray):
                 if is_sparse(mat):
+                    warnings.warn(
+                        "Converting delayedarray into sparse, may require more memory",
+                        RuntimeWarning,
+                    )
+
                     mat = to_scipy_sparse_matrix(mat)
                 else:
+                    warnings.warn(
+                        "Converting delayedarray into dense, may require more memory",
+                        RuntimeWarning,
+                    )
                     mat = to_dense_array(mat)
 
             layers[asy] = mat.transpose()
 
         trows = self._rows.to_pandas()
         if self._row_names is not None:
             trows.index = self._row_names
 
-        if trows.empty:
-            trows.index = range(self._shape[0])
-
         tcols = self._cols.to_pandas()
         if self._column_names is not None:
             tcols.index = self._column_names
 
         if tcols.empty:
             tcols.index = range(self._shape[1])
```

### Comparing `SummarizedExperiment-0.4.3/src/summarizedexperiment/RangedSummarizedExperiment.py` & `summarizedexperiment-0.4.4/src/summarizedexperiment/RangedSummarizedExperiment.py`

 * *Files identical despite different names*

### Comparing `SummarizedExperiment-0.4.3/src/summarizedexperiment/SummarizedExperiment.py` & `summarizedexperiment-0.4.4/src/summarizedexperiment/SummarizedExperiment.py`

 * *Files identical despite different names*

### Comparing `SummarizedExperiment-0.4.3/src/summarizedexperiment/__init__.py` & `summarizedexperiment-0.4.4/src/summarizedexperiment/__init__.py`

 * *Files identical despite different names*

### Comparing `SummarizedExperiment-0.4.3/src/summarizedexperiment/_combineutils.py` & `summarizedexperiment-0.4.4/src/summarizedexperiment/_combineutils.py`

 * *Files identical despite different names*

### Comparing `SummarizedExperiment-0.4.3/src/summarizedexperiment/_frameutils.py` & `summarizedexperiment-0.4.4/src/summarizedexperiment/_frameutils.py`

 * *Files identical despite different names*

### Comparing `SummarizedExperiment-0.4.3/src/summarizedexperiment/type_checks.py` & `summarizedexperiment-0.4.4/src/summarizedexperiment/type_checks.py`

 * *Files identical despite different names*

### Comparing `SummarizedExperiment-0.4.3/tests/data/summarized_experiments.py` & `summarizedexperiment-0.4.4/tests/data/summarized_experiments.py`

 * *Files identical despite different names*

### Comparing `SummarizedExperiment-0.4.3/tests/data/tenx.sub.h5` & `summarizedexperiment-0.4.4/tests/data/tenx.sub.h5`

 * *Files identical despite different names*

### Comparing `SummarizedExperiment-0.4.3/tests/test_RSE.py` & `summarizedexperiment-0.4.4/tests/test_RSE.py`

 * *Files identical despite different names*

### Comparing `SummarizedExperiment-0.4.3/tests/test_RSE_methods.py` & `summarizedexperiment-0.4.4/tests/test_RSE_methods.py`

 * *Files identical despite different names*

### Comparing `SummarizedExperiment-0.4.3/tests/test_SE.py` & `summarizedexperiment-0.4.4/tests/test_SE.py`

 * *Files identical despite different names*

### Comparing `SummarizedExperiment-0.4.3/tests/test_SE_combine_cols.py` & `summarizedexperiment-0.4.4/tests/test_SE_combine_cols.py`

 * *Files identical despite different names*

### Comparing `SummarizedExperiment-0.4.3/tests/test_SE_combine_rows.py` & `summarizedexperiment-0.4.4/tests/test_SE_combine_rows.py`

 * *Files identical despite different names*

### Comparing `SummarizedExperiment-0.4.3/tests/test_SE_methods.py` & `summarizedexperiment-0.4.4/tests/test_SE_methods.py`

 * *Files identical despite different names*

### Comparing `SummarizedExperiment-0.4.3/tests/test_SE_subset.py` & `summarizedexperiment-0.4.4/tests/test_SE_subset.py`

 * *Files identical despite different names*

### Comparing `SummarizedExperiment-0.4.3/tox.ini` & `summarizedexperiment-0.4.4/tox.ini`

 * *Files identical despite different names*

