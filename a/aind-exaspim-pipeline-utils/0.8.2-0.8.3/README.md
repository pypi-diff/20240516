# Comparing `tmp/aind_exaspim_pipeline_utils-0.8.2.tar.gz` & `tmp/aind_exaspim_pipeline_utils-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aind_exaspim_pipeline_utils-0.8.2.tar", last modified: Wed May  1 22:36:54 2024, max compression
+gzip compressed data, was "aind_exaspim_pipeline_utils-0.8.3.tar", last modified: Thu May 16 03:26:27 2024, max compression
```

## Comparing `aind_exaspim_pipeline_utils-0.8.2.tar` & `aind_exaspim_pipeline_utils-0.8.3.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:36:54.759838 aind_exaspim_pipeline_utils-0.8.2/
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-01 22:36:44.000000 aind_exaspim_pipeline_utils-0.8.2/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:36:54.743838 aind_exaspim_pipeline_utils-0.8.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:36:54.747838 aind_exaspim_pipeline_utils-0.8.2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-01 22:36:44.000000 aind_exaspim_pipeline_utils-0.8.2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-01 22:36:44.000000 aind_exaspim_pipeline_utils-0.8.2/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-01 22:36:44.000000 aind_exaspim_pipeline_utils-0.8.2/.github/ISSUE_TEMPLATE/user-story.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:36:54.747838 aind_exaspim_pipeline_utils-0.8.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-01 22:36:44.000000 aind_exaspim_pipeline_utils-0.8.2/.github/workflows/lint_and_test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-01 22:36:44.000000 aind_exaspim_pipeline_utils-0.8.2/.github/workflows/tag_and_publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-05-01 22:36:44.000000 aind_exaspim_pipeline_utils-0.8.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-01 22:36:44.000000 aind_exaspim_pipeline_utils-0.8.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-01 22:36:44.000000 aind_exaspim_pipeline_utils-0.8.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4947 2024-05-01 22:36:54.759838 aind_exaspim_pipeline_utils-0.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3815 2024-05-01 22:36:44.000000 aind_exaspim_pipeline_utils-0.8.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:36:54.751838 aind_exaspim_pipeline_utils-0.8.2/capsule_scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-01 22:36:44.000000 aind_exaspim_pipeline_utils-0.8.2/capsule_scripts/imagej_postInstall
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-01 22:36:44.000000 aind_exaspim_pipeline_utils-0.8.2/capsule_scripts/imagej_run.sh
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-01 22:36:44.000000 aind_exaspim_pipeline_utils-0.8.2/capsule_scripts/n5tozarr_postInstall
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-01 22:36:44.000000 aind_exaspim_pipeline_utils-0.8.2/capsule_scripts/n5tozarr_run.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:36:54.751838 aind_exaspim_pipeline_utils-0.8.2/doc/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-01 22:36:44.000000 aind_exaspim_pipeline_utils-0.8.2/doc/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-01 22:36:44.000000 aind_exaspim_pipeline_utils-0.8.2/doc/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:36:54.751838 aind_exaspim_pipeline_utils-0.8.2/doc/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:36:54.751838 aind_exaspim_pipeline_utils-0.8.2/doc/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     8733 2024-05-01 22:36:44.000000 aind_exaspim_pipeline_utils-0.8.2/doc/source/_static/dark-logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)   259838 2024-05-01 22:36:44.000000 aind_exaspim_pipeline_utils-0.8.2/doc/source/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)     8712 2024-05-01 22:36:44.000000 aind_exaspim_pipeline_utils-0.8.2/doc/source/_static/light-logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-05-01 22:36:44.000000 aind_exaspim_pipeline_utils-0.8.2/doc/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-05-01 22:36:44.000000 aind_exaspim_pipeline_utils-0.8.2/doc/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-05-01 22:36:44.000000 aind_exaspim_pipeline_utils-0.8.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 22:36:54.759838 aind_exaspim_pipeline_utils-0.8.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-01 22:36:44.000000 aind_exaspim_pipeline_utils-0.8.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:36:54.747838 aind_exaspim_pipeline_utils-0.8.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:36:54.751838 aind_exaspim_pipeline_utils-0.8.2/src/aind_exaspim_pipeline_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-01 22:36:45.000000 aind_exaspim_pipeline_utils-0.8.2/src/aind_exaspim_pipeline_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23467 2024-05-01 22:36:44.000000 aind_exaspim_pipeline_utils-0.8.2/src/aind_exaspim_pipeline_utils/exaspim_manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)     7057 2024-05-01 22:36:44.000000 aind_exaspim_pipeline_utils-0.8.2/src/aind_exaspim_pipeline_utils/imagej_macros.py
--rw-r--r--   0 runner    (1001) docker     (127)    24042 2024-05-01 22:36:44.000000 aind_exaspim_pipeline_utils-0.8.2/src/aind_exaspim_pipeline_utils/imagej_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-05-01 22:36:44.000000 aind_exaspim_pipeline_utils-0.8.2/src/aind_exaspim_pipeline_utils/java_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:36:54.751838 aind_exaspim_pipeline_utils-0.8.2/src/aind_exaspim_pipeline_utils/n5tozarr/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-01 22:36:44.000000 aind_exaspim_pipeline_utils-0.8.2/src/aind_exaspim_pipeline_utils/n5tozarr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18825 2024-05-01 22:36:44.000000 aind_exaspim_pipeline_utils-0.8.2/src/aind_exaspim_pipeline_utils/n5tozarr/n5tozarr_da.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:36:54.755838 aind_exaspim_pipeline_utils-0.8.2/src/aind_exaspim_pipeline_utils/qc/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-01 22:36:44.000000 aind_exaspim_pipeline_utils-0.8.2/src/aind_exaspim_pipeline_utils/qc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3429 2024-05-01 22:36:44.000000 aind_exaspim_pipeline_utils-0.8.2/src/aind_exaspim_pipeline_utils/qc/bigstitcher_log_edge_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     6987 2024-05-01 22:36:44.000000 aind_exaspim_pipeline_utils-0.8.2/src/aind_exaspim_pipeline_utils/qc/create_ng_link.py
--rw-r--r--   0 runner    (1001) docker     (127)     9689 2024-05-01 22:36:44.000000 aind_exaspim_pipeline_utils-0.8.2/src/aind_exaspim_pipeline_utils/qc/ng_ip_visualization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:36:54.755838 aind_exaspim_pipeline_utils-0.8.2/src/aind_exaspim_pipeline_utils/trigger/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-01 22:36:44.000000 aind_exaspim_pipeline_utils-0.8.2/src/aind_exaspim_pipeline_utils/trigger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28034 2024-05-01 22:36:44.000000 aind_exaspim_pipeline_utils-0.8.2/src/aind_exaspim_pipeline_utils/trigger/capsule.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:36:54.755838 aind_exaspim_pipeline_utils-0.8.2/src/aind_exaspim_pipeline_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4947 2024-05-01 22:36:54.000000 aind_exaspim_pipeline_utils-0.8.2/src/aind_exaspim_pipeline_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-05-01 22:36:54.000000 aind_exaspim_pipeline_utils-0.8.2/src/aind_exaspim_pipeline_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 22:36:54.000000 aind_exaspim_pipeline_utils-0.8.2/src/aind_exaspim_pipeline_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-01 22:36:54.000000 aind_exaspim_pipeline_utils-0.8.2/src/aind_exaspim_pipeline_utils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-01 22:36:54.000000 aind_exaspim_pipeline_utils-0.8.2/src/aind_exaspim_pipeline_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-01 22:36:54.000000 aind_exaspim_pipeline_utils-0.8.2/src/aind_exaspim_pipeline_utils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:36:54.755838 aind_exaspim_pipeline_utils-0.8.2/src/aind_trigger_codeocean/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-01 22:36:44.000000 aind_exaspim_pipeline_utils-0.8.2/src/aind_trigger_codeocean/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    51638 2024-05-01 22:36:44.000000 aind_exaspim_pipeline_utils-0.8.2/src/aind_trigger_codeocean/pipelines.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:36:54.755838 aind_exaspim_pipeline_utils-0.8.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-01 22:36:44.000000 aind_exaspim_pipeline_utils-0.8.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-05-01 22:36:44.000000 aind_exaspim_pipeline_utils-0.8.2/tests/test_capsule.py
--rw-r--r--   0 runner    (1001) docker     (127)     5059 2024-05-01 22:36:44.000000 aind_exaspim_pipeline_utils-0.8.2/tests/test_imagej_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-01 22:36:44.000000 aind_exaspim_pipeline_utils-0.8.2/tests/test_n5tozarr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 03:26:27.445949 aind_exaspim_pipeline_utils-0.8.3/
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-16 03:26:17.000000 aind_exaspim_pipeline_utils-0.8.3/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 03:26:27.433949 aind_exaspim_pipeline_utils-0.8.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 03:26:27.437949 aind_exaspim_pipeline_utils-0.8.3/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-16 03:26:17.000000 aind_exaspim_pipeline_utils-0.8.3/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-16 03:26:17.000000 aind_exaspim_pipeline_utils-0.8.3/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-16 03:26:17.000000 aind_exaspim_pipeline_utils-0.8.3/.github/ISSUE_TEMPLATE/user-story.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 03:26:27.437949 aind_exaspim_pipeline_utils-0.8.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-16 03:26:17.000000 aind_exaspim_pipeline_utils-0.8.3/.github/workflows/lint_and_test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-16 03:26:17.000000 aind_exaspim_pipeline_utils-0.8.3/.github/workflows/tag_and_publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-05-16 03:26:17.000000 aind_exaspim_pipeline_utils-0.8.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-16 03:26:17.000000 aind_exaspim_pipeline_utils-0.8.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-16 03:26:17.000000 aind_exaspim_pipeline_utils-0.8.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4947 2024-05-16 03:26:27.445949 aind_exaspim_pipeline_utils-0.8.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3815 2024-05-16 03:26:17.000000 aind_exaspim_pipeline_utils-0.8.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 03:26:27.437949 aind_exaspim_pipeline_utils-0.8.3/capsule_scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-16 03:26:17.000000 aind_exaspim_pipeline_utils-0.8.3/capsule_scripts/imagej_postInstall
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-16 03:26:17.000000 aind_exaspim_pipeline_utils-0.8.3/capsule_scripts/imagej_run.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-16 03:26:17.000000 aind_exaspim_pipeline_utils-0.8.3/capsule_scripts/n5tozarr_postInstall
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-16 03:26:17.000000 aind_exaspim_pipeline_utils-0.8.3/capsule_scripts/n5tozarr_run.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 03:26:27.437949 aind_exaspim_pipeline_utils-0.8.3/doc/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-16 03:26:17.000000 aind_exaspim_pipeline_utils-0.8.3/doc/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-16 03:26:17.000000 aind_exaspim_pipeline_utils-0.8.3/doc/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 03:26:27.437949 aind_exaspim_pipeline_utils-0.8.3/doc/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 03:26:27.437949 aind_exaspim_pipeline_utils-0.8.3/doc/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     8733 2024-05-16 03:26:17.000000 aind_exaspim_pipeline_utils-0.8.3/doc/source/_static/dark-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   259838 2024-05-16 03:26:17.000000 aind_exaspim_pipeline_utils-0.8.3/doc/source/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     8712 2024-05-16 03:26:17.000000 aind_exaspim_pipeline_utils-0.8.3/doc/source/_static/light-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-05-16 03:26:17.000000 aind_exaspim_pipeline_utils-0.8.3/doc/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-05-16 03:26:17.000000 aind_exaspim_pipeline_utils-0.8.3/doc/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2594 2024-05-16 03:26:17.000000 aind_exaspim_pipeline_utils-0.8.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 03:26:27.445949 aind_exaspim_pipeline_utils-0.8.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-16 03:26:17.000000 aind_exaspim_pipeline_utils-0.8.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 03:26:27.433949 aind_exaspim_pipeline_utils-0.8.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 03:26:27.441949 aind_exaspim_pipeline_utils-0.8.3/src/aind_exaspim_pipeline_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-16 03:26:17.000000 aind_exaspim_pipeline_utils-0.8.3/src/aind_exaspim_pipeline_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23464 2024-05-16 03:26:17.000000 aind_exaspim_pipeline_utils-0.8.3/src/aind_exaspim_pipeline_utils/exaspim_manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7057 2024-05-16 03:26:17.000000 aind_exaspim_pipeline_utils-0.8.3/src/aind_exaspim_pipeline_utils/imagej_macros.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24060 2024-05-16 03:26:17.000000 aind_exaspim_pipeline_utils-0.8.3/src/aind_exaspim_pipeline_utils/imagej_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3114 2024-05-16 03:26:17.000000 aind_exaspim_pipeline_utils-0.8.3/src/aind_exaspim_pipeline_utils/java_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 03:26:27.441949 aind_exaspim_pipeline_utils-0.8.3/src/aind_exaspim_pipeline_utils/n5tozarr/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-16 03:26:17.000000 aind_exaspim_pipeline_utils-0.8.3/src/aind_exaspim_pipeline_utils/n5tozarr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18825 2024-05-16 03:26:17.000000 aind_exaspim_pipeline_utils-0.8.3/src/aind_exaspim_pipeline_utils/n5tozarr/n5tozarr_da.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 03:26:27.441949 aind_exaspim_pipeline_utils-0.8.3/src/aind_exaspim_pipeline_utils/qc/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-16 03:26:17.000000 aind_exaspim_pipeline_utils-0.8.3/src/aind_exaspim_pipeline_utils/qc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3516 2024-05-16 03:26:17.000000 aind_exaspim_pipeline_utils-0.8.3/src/aind_exaspim_pipeline_utils/qc/bigstitcher_log_edge_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6987 2024-05-16 03:26:17.000000 aind_exaspim_pipeline_utils-0.8.3/src/aind_exaspim_pipeline_utils/qc/create_ng_link.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9689 2024-05-16 03:26:17.000000 aind_exaspim_pipeline_utils-0.8.3/src/aind_exaspim_pipeline_utils/qc/ng_ip_visualization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 03:26:27.441949 aind_exaspim_pipeline_utils-0.8.3/src/aind_exaspim_pipeline_utils/trigger/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-16 03:26:17.000000 aind_exaspim_pipeline_utils-0.8.3/src/aind_exaspim_pipeline_utils/trigger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28937 2024-05-16 03:26:17.000000 aind_exaspim_pipeline_utils-0.8.3/src/aind_exaspim_pipeline_utils/trigger/capsule.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 03:26:27.445949 aind_exaspim_pipeline_utils-0.8.3/src/aind_exaspim_pipeline_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4947 2024-05-16 03:26:27.000000 aind_exaspim_pipeline_utils-0.8.3/src/aind_exaspim_pipeline_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-05-16 03:26:27.000000 aind_exaspim_pipeline_utils-0.8.3/src/aind_exaspim_pipeline_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 03:26:27.000000 aind_exaspim_pipeline_utils-0.8.3/src/aind_exaspim_pipeline_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-16 03:26:27.000000 aind_exaspim_pipeline_utils-0.8.3/src/aind_exaspim_pipeline_utils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-16 03:26:27.000000 aind_exaspim_pipeline_utils-0.8.3/src/aind_exaspim_pipeline_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-16 03:26:27.000000 aind_exaspim_pipeline_utils-0.8.3/src/aind_exaspim_pipeline_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 03:26:27.441949 aind_exaspim_pipeline_utils-0.8.3/src/aind_trigger_codeocean/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-16 03:26:17.000000 aind_exaspim_pipeline_utils-0.8.3/src/aind_trigger_codeocean/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51638 2024-05-16 03:26:17.000000 aind_exaspim_pipeline_utils-0.8.3/src/aind_trigger_codeocean/pipelines.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 03:26:27.445949 aind_exaspim_pipeline_utils-0.8.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-16 03:26:17.000000 aind_exaspim_pipeline_utils-0.8.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-05-16 03:26:17.000000 aind_exaspim_pipeline_utils-0.8.3/tests/test_capsule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5059 2024-05-16 03:26:17.000000 aind_exaspim_pipeline_utils-0.8.3/tests/test_imagej_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-16 03:26:17.000000 aind_exaspim_pipeline_utils-0.8.3/tests/test_n5tozarr.py
```

### Comparing `aind_exaspim_pipeline_utils-0.8.2/.github/ISSUE_TEMPLATE/bug_report.md` & `aind_exaspim_pipeline_utils-0.8.3/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `aind_exaspim_pipeline_utils-0.8.2/.github/ISSUE_TEMPLATE/feature_request.md` & `aind_exaspim_pipeline_utils-0.8.3/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `aind_exaspim_pipeline_utils-0.8.2/.github/ISSUE_TEMPLATE/user-story.md` & `aind_exaspim_pipeline_utils-0.8.3/.github/ISSUE_TEMPLATE/user-story.md`

 * *Files identical despite different names*

### Comparing `aind_exaspim_pipeline_utils-0.8.2/.github/workflows/lint_and_test.yml` & `aind_exaspim_pipeline_utils-0.8.3/.github/workflows/lint_and_test.yml`

 * *Files identical despite different names*

### Comparing `aind_exaspim_pipeline_utils-0.8.2/.github/workflows/tag_and_publish.yml` & `aind_exaspim_pipeline_utils-0.8.3/.github/workflows/tag_and_publish.yml`

 * *Files identical despite different names*

### Comparing `aind_exaspim_pipeline_utils-0.8.2/.gitignore` & `aind_exaspim_pipeline_utils-0.8.3/.gitignore`

 * *Files identical despite different names*

### Comparing `aind_exaspim_pipeline_utils-0.8.2/LICENSE` & `aind_exaspim_pipeline_utils-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aind_exaspim_pipeline_utils-0.8.2/PKG-INFO` & `aind_exaspim_pipeline_utils-0.8.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aind_exaspim_pipeline_utils
-Version: 0.8.2
+Version: 0.8.3
 Summary: AIND exaSPIM pipeline utilities.
 Author: Allen Institute for Neural Dynamics
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `aind_exaspim_pipeline_utils-0.8.2/README.md` & `aind_exaspim_pipeline_utils-0.8.3/README.md`

 * *Files identical despite different names*

### Comparing `aind_exaspim_pipeline_utils-0.8.2/doc/Makefile` & `aind_exaspim_pipeline_utils-0.8.3/doc/Makefile`

 * *Files identical despite different names*

### Comparing `aind_exaspim_pipeline_utils-0.8.2/doc/make.bat` & `aind_exaspim_pipeline_utils-0.8.3/doc/make.bat`

 * *Files identical despite different names*

### Comparing `aind_exaspim_pipeline_utils-0.8.2/doc/source/_static/dark-logo.svg` & `aind_exaspim_pipeline_utils-0.8.3/doc/source/_static/dark-logo.svg`

 * *Files identical despite different names*

### Comparing `aind_exaspim_pipeline_utils-0.8.2/doc/source/_static/favicon.ico` & `aind_exaspim_pipeline_utils-0.8.3/doc/source/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `aind_exaspim_pipeline_utils-0.8.2/doc/source/_static/light-logo.svg` & `aind_exaspim_pipeline_utils-0.8.3/doc/source/_static/light-logo.svg`

 * *Files identical despite different names*

### Comparing `aind_exaspim_pipeline_utils-0.8.2/doc/source/conf.py` & `aind_exaspim_pipeline_utils-0.8.3/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `aind_exaspim_pipeline_utils-0.8.2/pyproject.toml` & `aind_exaspim_pipeline_utils-0.8.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aind_exaspim_pipeline_utils-0.8.2/src/aind_exaspim_pipeline_utils/exaspim_manifest.py` & `aind_exaspim_pipeline_utils-0.8.3/src/aind_exaspim_pipeline_utils/exaspim_manifest.py`

 * *Files 0% similar despite different names*

```diff
@@ -342,26 +342,26 @@
         title="group all angles/channels/illums/tiles that belong to the same timepoint as one View, "
         "e.g. for stabilization across time (default: false)",
     )
     label: Optional[str] = Field(
         "beads", title="label of the interest points used for solve if using interest points (e.g. beads)"
     )
     globalOptType: str = Field(
-        "TWO_ROUND_ITERATIVE",
+        "TWO_ROUND_SIMPLE",
         title="global optimization method; ONE_ROUND_SIMPLE, ONE_ROUND_ITERATIVE, TWO_ROUND_SIMPLE or "
         "TWO_ROUND_ITERATIVE. Two round handles unconnected tiles, iterative handles wrong links "
         "(default: ONE_ROUND_SIMPLE)",
     )
     relativeThreshold: float = Field(
-        0.0,
+        3.5,
         title="relative error threshold for iterative solvers, how many times worse than the average error "
         "a link needs to be (default: 3.5)",
     )
     absoluteThreshold: float = Field(
-        0.0, title="absoluted error threshold for iterative solver to drop a link in pixels (default: 7.0)"
+        7.0, title="absoluted error threshold for iterative solver to drop a link in pixels (default: 7.0)"
     )
     maxError: float = Field(5.0, title="max error for the solve (default: 5.0)")
     maxIterations: int = Field(10000, title="max number of iterations for solve (default: 10,000)")
     maxPlateauwidth: int = Field(200, title="max plateau witdth for solve (default: 200)")
     disableFixedViews: bool = Field(False, title="disable fixing of views (see --fixedViews)")
     fixedViews: Optional[List[str]] = Field(
         ["0,7"],
```

### Comparing `aind_exaspim_pipeline_utils-0.8.2/src/aind_exaspim_pipeline_utils/imagej_macros.py` & `aind_exaspim_pipeline_utils-0.8.3/src/aind_exaspim_pipeline_utils/imagej_macros.py`

 * *Files identical despite different names*

### Comparing `aind_exaspim_pipeline_utils-0.8.2/src/aind_exaspim_pipeline_utils/imagej_wrapper.py` & `aind_exaspim_pipeline_utils-0.8.3/src/aind_exaspim_pipeline_utils/imagej_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -447,15 +447,15 @@
     # Read the log file
     with open("../results/edge_connectivity_report.txt", "w") as f_report:
         for i in range(num_registrations):
             print(f"Edge dis-connectivity based on ip_registration{i:d}.log (running order):", file=f_report)
             with open(f"../results/ip_registration{i:d}.log", "r") as f:
                 lines = f.readlines()
             # Extract the tile pair numbers from failed RANSAC correspondence finding log messages
-            blocks = bigstitcher_log_edge_analysis.get_unfitted_tile_pairs(lines)
+            blocks = bigstitcher_log_edge_analysis.get_unfitted_tile_pairs(lines, multiblock=False)
             # Create a visualization of the failed edges
             # Write the visualization to a file
             bigstitcher_log_edge_analysis.print_visualization(blocks, file=f_report)
 
 
 def imagej_do_registrations(pipeline_manifest: ExaspimProcessingPipeline,
                             args: dict, logger: logging.Logger,
```

### Comparing `aind_exaspim_pipeline_utils-0.8.2/src/aind_exaspim_pipeline_utils/java_utils.py` & `aind_exaspim_pipeline_utils-0.8.3/src/aind_exaspim_pipeline_utils/java_utils.py`

 * *Files identical despite different names*

### Comparing `aind_exaspim_pipeline_utils-0.8.2/src/aind_exaspim_pipeline_utils/n5tozarr/n5tozarr_da.py` & `aind_exaspim_pipeline_utils-0.8.3/src/aind_exaspim_pipeline_utils/n5tozarr/n5tozarr_da.py`

 * *Files identical despite different names*

### Comparing `aind_exaspim_pipeline_utils-0.8.2/src/aind_exaspim_pipeline_utils/qc/bigstitcher_log_edge_analysis.py` & `aind_exaspim_pipeline_utils-0.8.3/src/aind_exaspim_pipeline_utils/qc/bigstitcher_log_edge_analysis.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 """Utility functions to search for unfitted tile edges in bigstitcher log output"""
 import re
 import sys
 from typing import Iterable, List, Tuple
 import numpy as np
 
 
-def get_unfitted_tile_pairs(lines: Iterable[str]) -> List[List[Tuple[int, int]]]:  # pragma: no cover
+def get_unfitted_tile_pairs(
+    lines: Iterable[str], multiblock: bool = True
+) -> List[List[Tuple[int, int]]]:  # pragma: no cover
     """Extract tile pair numbers from log lines of failed RANSAC correspondence
     finding.
 
     Extract the tile number pairs from failed RANSAC correspondence finding log messages. The
     results are grouped in blocks based on the RANSAC log messages, i.e. we assume that
     each registration round has the RANSAC related lines in consecutive lines in the input.
     Each non-RANSAC log line starts a new output block.
@@ -30,23 +32,24 @@
     blocks = []
     pairs = []
     for line in lines:
         line = line.strip()
         # RANSAC result lines
         m = re.match(".*\\[TP=(\\d+) ViewId=(\\d+) >>> TP=(\\d+) ViewId=(\\d+)\\]: (\\w+)", line)
         if m:
-            if m.group(5) == "NO" or m.group(5) == "Not":  # Failed RANSAC
+            if m.group(5) == "NO" or m.group(5) == "Not" or m.group(5) == "Model":  # Failed RANSAC
                 a = int(m.group(4))
                 b = int(m.group(2))
             else:
                 # Successful RANSAC line
                 continue
         else:
             # Non-RANSAC line
-            newblock = True
+            if multiblock:
+                newblock = True
             continue
         if b < a:
             a, b = b, a
         if b - a in (1, 3):
             # Failed edge
             if newblock:
                 if pairs:
```

### Comparing `aind_exaspim_pipeline_utils-0.8.2/src/aind_exaspim_pipeline_utils/qc/create_ng_link.py` & `aind_exaspim_pipeline_utils-0.8.3/src/aind_exaspim_pipeline_utils/qc/create_ng_link.py`

 * *Files identical despite different names*

### Comparing `aind_exaspim_pipeline_utils-0.8.2/src/aind_exaspim_pipeline_utils/qc/ng_ip_visualization.py` & `aind_exaspim_pipeline_utils-0.8.3/src/aind_exaspim_pipeline_utils/qc/ng_ip_visualization.py`

 * *Files identical despite different names*

### Comparing `aind_exaspim_pipeline_utils-0.8.2/src/aind_exaspim_pipeline_utils/trigger/capsule.py` & `aind_exaspim_pipeline_utils-0.8.3/src/aind_exaspim_pipeline_utils/trigger/capsule.py`

 * *Files 2% similar despite different names*

```diff
@@ -548,24 +548,41 @@
 
 def create_and_upload_emr_config(args, manifest: ExaspimProcessingPipeline):  # pragma: no cover
     """Create EMR command line parameters for the fusion of the present alignment run."""
     config = (
         f'["-x", "{args.alignment_output_uri}'
         f'bigstitcher_emr_{manifest.subject_id}_{manifest.pipeline_suffix}_0.xml",\n'
         f'"--outS3Bucket", "{args.fusion_output_bucket}", '
-        f'"-o", "/{args.fusion_output_prefix}/fused.n5",\n'
+        f'"-o", "{args.fusion_output_prefix}/fused.n5",\n'
         f'"--bdv", "0,0", '
         f'"--xmlout", "s3://{args.fusion_output_bucket}/{args.fusion_output_prefix}/fused.xml", '
         '"--storage", "N5", "--UINT16", "--minIntensity=0", '
         '"--maxIntensity=65535", "--preserveAnisotropy" ]\n'
     )
-    with open("../results/emr_fusion_config.txt", "w") as f:
+    with open("../results/emr_fusion_config_ijwrap.txt", "w") as f:
         f.write(config)
     logger.info("Uploading emr_fusion_config.txt to bucket {}".format(args.manifest_bucket_name))
     s3 = boto3.client("s3")  # Authentication should be available in the environment
+    object_name = "/".join((args.manifest_path, "emr_fusion_config_ijwrap.txt"))
+    s3.upload_file("../results/emr_fusion_config_ijwrap.txt", args.manifest_bucket_name, object_name)
+
+    # For the directS3 version which should be now the default
+    config = (
+        f'["-x", "{args.alignment_output_uri}'
+        f'bigstitcher.xml",\n'
+        f'"--outS3Bucket", "{args.fusion_output_bucket}", '
+        f'"-o", "{args.fusion_output_prefix}/fused.n5",\n'
+        f'"--bdv", "0,0", '
+        f'"--xmlout", "s3://{args.fusion_output_bucket}/{args.fusion_output_prefix}/fused.xml", '
+        '"--storage", "N5", "--UINT16", "--minIntensity=0", '
+        '"--maxIntensity=65535", "--preserveAnisotropy" ]\n'
+    )
+    with open("../results/emr_fusion_config.txt", "w") as f:
+        f.write(config)
+    logger.info("Uploading emr_fusion_config.txt to bucket {}".format(args.manifest_bucket_name))
     object_name = "/".join((args.manifest_path, "emr_fusion_config.txt"))
     s3.upload_file("../results/emr_fusion_config.txt", args.manifest_bucket_name, object_name)
 
 
 def upload_manifest(args, manifest: ExaspimProcessingPipeline):  # pragma: no cover
     """Write out the given manifest as a json file and upload to S3"""
     s3 = boto3.client("s3")  # Authentication should be available in the environment
```

### Comparing `aind_exaspim_pipeline_utils-0.8.2/src/aind_exaspim_pipeline_utils.egg-info/PKG-INFO` & `aind_exaspim_pipeline_utils-0.8.3/src/aind_exaspim_pipeline_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aind_exaspim_pipeline_utils
-Version: 0.8.2
+Version: 0.8.3
 Summary: AIND exaSPIM pipeline utilities.
 Author: Allen Institute for Neural Dynamics
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `aind_exaspim_pipeline_utils-0.8.2/src/aind_exaspim_pipeline_utils.egg-info/SOURCES.txt` & `aind_exaspim_pipeline_utils-0.8.3/src/aind_exaspim_pipeline_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aind_exaspim_pipeline_utils-0.8.2/src/aind_exaspim_pipeline_utils.egg-info/entry_points.txt` & `aind_exaspim_pipeline_utils-0.8.3/src/aind_exaspim_pipeline_utils.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `aind_exaspim_pipeline_utils-0.8.2/src/aind_trigger_codeocean/pipelines.py` & `aind_exaspim_pipeline_utils-0.8.3/src/aind_trigger_codeocean/pipelines.py`

 * *Files identical despite different names*

### Comparing `aind_exaspim_pipeline_utils-0.8.2/tests/test_capsule.py` & `aind_exaspim_pipeline_utils-0.8.3/tests/test_capsule.py`

 * *Files identical despite different names*

### Comparing `aind_exaspim_pipeline_utils-0.8.2/tests/test_imagej_wrapper.py` & `aind_exaspim_pipeline_utils-0.8.3/tests/test_imagej_wrapper.py`

 * *Files identical despite different names*

### Comparing `aind_exaspim_pipeline_utils-0.8.2/tests/test_n5tozarr.py` & `aind_exaspim_pipeline_utils-0.8.3/tests/test_n5tozarr.py`

 * *Files identical despite different names*

