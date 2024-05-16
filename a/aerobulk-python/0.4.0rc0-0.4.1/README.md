# Comparing `tmp/aerobulk-python-0.4.0rc0.tar.gz` & `tmp/aerobulk-python-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aerobulk-python-0.4.0rc0.tar", last modified: Tue Oct  4 17:13:09 2022, max compression
+gzip compressed data, was "aerobulk-python-0.4.1.tar", last modified: Thu May 16 17:29:35 2024, max compression
```

## Comparing `aerobulk-python-0.4.0rc0.tar` & `aerobulk-python-0.4.1.tar`

### file list

```diff
@@ -1,54 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-04 17:13:09.839970 aerobulk-python-0.4.0rc0/
--rw-r--r--   0 runner    (1001) docker     (121)       41 2022-10-04 17:12:57.000000 aerobulk-python-0.4.0rc0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-04 17:13:09.835970 aerobulk-python-0.4.0rc0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-04 17:13:09.839970 aerobulk-python-0.4.0rc0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     1818 2022-10-04 17:12:57.000000 aerobulk-python-0.4.0rc0/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1232 2022-10-04 17:12:57.000000 aerobulk-python-0.4.0rc0/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (121)      297 2022-10-04 17:12:57.000000 aerobulk-python-0.4.0rc0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      114 2022-10-04 17:12:57.000000 aerobulk-python-0.4.0rc0/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (121)      433 2022-10-04 17:12:57.000000 aerobulk-python-0.4.0rc0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    35121 2022-10-04 17:12:57.000000 aerobulk-python-0.4.0rc0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       34 2022-10-04 17:12:57.000000 aerobulk-python-0.4.0rc0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      726 2022-10-04 17:13:09.839970 aerobulk-python-0.4.0rc0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    12712 2022-10-04 17:12:57.000000 aerobulk-python-0.4.0rc0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-04 17:13:09.839970 aerobulk-python-0.4.0rc0/ci/
--rw-r--r--   0 runner    (1001) docker     (121)      162 2022-10-04 17:12:57.000000 aerobulk-python-0.4.0rc0/ci/environment.yml
--rw-r--r--   0 runner    (1001) docker     (121)      165 2022-10-04 17:13:09.843970 aerobulk-python-0.4.0rc0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     4862 2022-10-04 17:12:57.000000 aerobulk-python-0.4.0rc0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-04 17:13:09.835970 aerobulk-python-0.4.0rc0/source/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-04 17:13:09.839970 aerobulk-python-0.4.0rc0/source/aerobulk/
--rw-r--r--   0 runner    (1001) docker     (121)      210 2022-10-04 17:12:57.000000 aerobulk-python-0.4.0rc0/source/aerobulk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       24 2022-10-04 17:13:09.000000 aerobulk-python-0.4.0rc0/source/aerobulk/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)    13835 2022-10-04 17:12:57.000000 aerobulk-python-0.4.0rc0/source/aerobulk/flux.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-04 17:13:09.839970 aerobulk-python-0.4.0rc0/source/aerobulk_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      726 2022-10-04 17:13:09.000000 aerobulk-python-0.4.0rc0/source/aerobulk_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1517 2022-10-04 17:13:09.000000 aerobulk-python-0.4.0rc0/source/aerobulk_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-04 17:13:09.000000 aerobulk-python-0.4.0rc0/source/aerobulk_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-10-04 17:13:09.000000 aerobulk-python-0.4.0rc0/source/aerobulk_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-10-04 17:13:09.000000 aerobulk-python-0.4.0rc0/source/aerobulk_python.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-04 17:13:09.839970 aerobulk-python-0.4.0rc0/source/fortran/
--rw-r--r--   0 runner    (1001) docker     (121)       58 2022-10-04 17:12:57.000000 aerobulk-python-0.4.0rc0/source/fortran/.f2py_f2cmap
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-04 17:13:09.835970 aerobulk-python-0.4.0rc0/source/fortran/aerobulk/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-04 17:13:09.839970 aerobulk-python-0.4.0rc0/source/fortran/aerobulk/src/
--rw-r--r--   0 runner    (1001) docker     (121)    13313 2022-10-04 17:12:58.000000 aerobulk-python-0.4.0rc0/source/fortran/aerobulk/src/mod_aerobulk.f90
--rw-r--r--   0 runner    (1001) docker     (121)     9464 2022-10-04 17:12:58.000000 aerobulk-python-0.4.0rc0/source/fortran/aerobulk/src/mod_aerobulk_compute.f90
--rw-r--r--   0 runner    (1001) docker     (121)    20785 2022-10-04 17:12:58.000000 aerobulk-python-0.4.0rc0/source/fortran/aerobulk/src/mod_blk_andreas.f90
--rw-r--r--   0 runner    (1001) docker     (121)    23487 2022-10-04 17:12:58.000000 aerobulk-python-0.4.0rc0/source/fortran/aerobulk/src/mod_blk_coare3p0.f90
--rw-r--r--   0 runner    (1001) docker     (121)    24770 2022-10-04 17:12:58.000000 aerobulk-python-0.4.0rc0/source/fortran/aerobulk/src/mod_blk_coare3p6.f90
--rw-r--r--   0 runner    (1001) docker     (121)    30608 2022-10-04 17:12:58.000000 aerobulk-python-0.4.0rc0/source/fortran/aerobulk/src/mod_blk_ecmwf.f90
--rw-r--r--   0 runner    (1001) docker     (121)    21480 2022-10-04 17:12:58.000000 aerobulk-python-0.4.0rc0/source/fortran/aerobulk/src/mod_blk_ncar.f90
--rw-r--r--   0 runner    (1001) docker     (121)     6511 2022-10-04 17:12:58.000000 aerobulk-python-0.4.0rc0/source/fortran/aerobulk/src/mod_blk_neutral_10m.f90
--rw-r--r--   0 runner    (1001) docker     (121)    18607 2022-10-04 17:12:58.000000 aerobulk-python-0.4.0rc0/source/fortran/aerobulk/src/mod_common_coare.f90
--rw-r--r--   0 runner    (1001) docker     (121)    14068 2022-10-04 17:12:58.000000 aerobulk-python-0.4.0rc0/source/fortran/aerobulk/src/mod_const.f90
--rw-r--r--   0 runner    (1001) docker     (121)   104694 2022-10-04 17:12:58.000000 aerobulk-python-0.4.0rc0/source/fortran/aerobulk/src/mod_phymbl.f90
--rw-r--r--   0 runner    (1001) docker     (121)    13064 2022-10-04 17:12:58.000000 aerobulk-python-0.4.0rc0/source/fortran/aerobulk/src/mod_skin_coare.f90
--rw-r--r--   0 runner    (1001) docker     (121)    11478 2022-10-04 17:12:58.000000 aerobulk-python-0.4.0rc0/source/fortran/aerobulk/src/mod_skin_ecmwf.f90
--rw-r--r--   0 runner    (1001) docker     (121)     1373 2022-10-04 17:12:57.000000 aerobulk-python-0.4.0rc0/source/fortran/mod_aerobulk_wrap_noskin.f90
--rw-r--r--   0 runner    (1001) docker     (121)     2353 2022-10-04 17:12:57.000000 aerobulk-python-0.4.0rc0/source/fortran/mod_aerobulk_wrap_noskin.pyf
--rw-r--r--   0 runner    (1001) docker     (121)     1512 2022-10-04 17:12:57.000000 aerobulk-python-0.4.0rc0/source/fortran/mod_aerobulk_wrap_skin.f90
--rw-r--r--   0 runner    (1001) docker     (121)     2580 2022-10-04 17:12:57.000000 aerobulk-python-0.4.0rc0/source/fortran/mod_aerobulk_wrap_skin.pyf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-04 17:13:09.839970 aerobulk-python-0.4.0rc0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     1668 2022-10-04 17:12:57.000000 aerobulk-python-0.4.0rc0/tests/create_test_data.py
--rw-r--r--   0 runner    (1001) docker     (121)     3500 2022-10-04 17:12:57.000000 aerobulk-python-0.4.0rc0/tests/test_flux_np.py
--rw-r--r--   0 runner    (1001) docker     (121)     3022 2022-10-04 17:12:57.000000 aerobulk-python-0.4.0rc0/tests/test_flux_xr.py
--rw-r--r--   0 runner    (1001) docker     (121)     3741 2022-10-04 17:12:57.000000 aerobulk-python-0.4.0rc0/tests/test_fortran.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 17:29:35.527142 aerobulk-python-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-16 17:29:23.000000 aerobulk-python-0.4.1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 17:29:35.519142 aerobulk-python-0.4.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 17:29:35.527142 aerobulk-python-0.4.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-05-16 17:29:23.000000 aerobulk-python-0.4.1/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-05-16 17:29:23.000000 aerobulk-python-0.4.1/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-16 17:29:23.000000 aerobulk-python-0.4.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-16 17:29:23.000000 aerobulk-python-0.4.1/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-16 17:29:23.000000 aerobulk-python-0.4.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-05-16 17:29:23.000000 aerobulk-python-0.4.1/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)    35121 2024-05-16 17:29:23.000000 aerobulk-python-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-16 17:29:23.000000 aerobulk-python-0.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-16 17:29:35.527142 aerobulk-python-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12938 2024-05-16 17:29:23.000000 aerobulk-python-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 17:29:35.527142 aerobulk-python-0.4.1/ci/
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-16 17:29:23.000000 aerobulk-python-0.4.1/ci/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-16 17:29:35.527142 aerobulk-python-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4919 2024-05-16 17:29:23.000000 aerobulk-python-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 17:29:35.523142 aerobulk-python-0.4.1/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 17:29:35.527142 aerobulk-python-0.4.1/source/aerobulk/
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-16 17:29:23.000000 aerobulk-python-0.4.1/source/aerobulk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-16 17:29:35.000000 aerobulk-python-0.4.1/source/aerobulk/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13834 2024-05-16 17:29:23.000000 aerobulk-python-0.4.1/source/aerobulk/flux.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 17:29:35.527142 aerobulk-python-0.4.1/source/aerobulk_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-16 17:29:35.000000 aerobulk-python-0.4.1/source/aerobulk_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-05-16 17:29:35.000000 aerobulk-python-0.4.1/source/aerobulk_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 17:29:35.000000 aerobulk-python-0.4.1/source/aerobulk_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-16 17:29:35.000000 aerobulk-python-0.4.1/source/aerobulk_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-16 17:29:35.000000 aerobulk-python-0.4.1/source/aerobulk_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 17:29:35.527142 aerobulk-python-0.4.1/source/fortran/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-16 17:29:23.000000 aerobulk-python-0.4.1/source/fortran/.f2py_f2cmap
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 17:29:35.519142 aerobulk-python-0.4.1/source/fortran/aerobulk/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 17:29:35.527142 aerobulk-python-0.4.1/source/fortran/aerobulk/src/
+-rw-r--r--   0 runner    (1001) docker     (127)    13313 2024-05-16 17:29:24.000000 aerobulk-python-0.4.1/source/fortran/aerobulk/src/mod_aerobulk.f90
+-rw-r--r--   0 runner    (1001) docker     (127)     9464 2024-05-16 17:29:24.000000 aerobulk-python-0.4.1/source/fortran/aerobulk/src/mod_aerobulk_compute.f90
+-rw-r--r--   0 runner    (1001) docker     (127)    20785 2024-05-16 17:29:24.000000 aerobulk-python-0.4.1/source/fortran/aerobulk/src/mod_blk_andreas.f90
+-rw-r--r--   0 runner    (1001) docker     (127)    23487 2024-05-16 17:29:24.000000 aerobulk-python-0.4.1/source/fortran/aerobulk/src/mod_blk_coare3p0.f90
+-rw-r--r--   0 runner    (1001) docker     (127)    24770 2024-05-16 17:29:24.000000 aerobulk-python-0.4.1/source/fortran/aerobulk/src/mod_blk_coare3p6.f90
+-rw-r--r--   0 runner    (1001) docker     (127)    30608 2024-05-16 17:29:24.000000 aerobulk-python-0.4.1/source/fortran/aerobulk/src/mod_blk_ecmwf.f90
+-rw-r--r--   0 runner    (1001) docker     (127)    21480 2024-05-16 17:29:24.000000 aerobulk-python-0.4.1/source/fortran/aerobulk/src/mod_blk_ncar.f90
+-rw-r--r--   0 runner    (1001) docker     (127)     6511 2024-05-16 17:29:24.000000 aerobulk-python-0.4.1/source/fortran/aerobulk/src/mod_blk_neutral_10m.f90
+-rw-r--r--   0 runner    (1001) docker     (127)    18607 2024-05-16 17:29:24.000000 aerobulk-python-0.4.1/source/fortran/aerobulk/src/mod_common_coare.f90
+-rw-r--r--   0 runner    (1001) docker     (127)    14068 2024-05-16 17:29:24.000000 aerobulk-python-0.4.1/source/fortran/aerobulk/src/mod_const.f90
+-rw-r--r--   0 runner    (1001) docker     (127)   104694 2024-05-16 17:29:24.000000 aerobulk-python-0.4.1/source/fortran/aerobulk/src/mod_phymbl.f90
+-rw-r--r--   0 runner    (1001) docker     (127)    13064 2024-05-16 17:29:24.000000 aerobulk-python-0.4.1/source/fortran/aerobulk/src/mod_skin_coare.f90
+-rw-r--r--   0 runner    (1001) docker     (127)    11478 2024-05-16 17:29:24.000000 aerobulk-python-0.4.1/source/fortran/aerobulk/src/mod_skin_ecmwf.f90
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-16 17:29:23.000000 aerobulk-python-0.4.1/source/fortran/mod_aerobulk_wrap_noskin.f90
+-rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-05-16 17:29:23.000000 aerobulk-python-0.4.1/source/fortran/mod_aerobulk_wrap_noskin.pyf
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-16 17:29:23.000000 aerobulk-python-0.4.1/source/fortran/mod_aerobulk_wrap_skin.f90
+-rw-r--r--   0 runner    (1001) docker     (127)     2580 2024-05-16 17:29:23.000000 aerobulk-python-0.4.1/source/fortran/mod_aerobulk_wrap_skin.pyf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 17:29:35.527142 aerobulk-python-0.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-05-16 17:29:23.000000 aerobulk-python-0.4.1/tests/create_test_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3500 2024-05-16 17:29:23.000000 aerobulk-python-0.4.1/tests/test_flux_np.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3022 2024-05-16 17:29:23.000000 aerobulk-python-0.4.1/tests/test_flux_xr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3741 2024-05-16 17:29:23.000000 aerobulk-python-0.4.1/tests/test_fortran.py
```

### Comparing `aerobulk-python-0.4.0rc0/.github/workflows/ci.yaml` & `aerobulk-python-0.4.1/.github/workflows/ci.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -4,58 +4,54 @@
     branches:
       - "main"
   pull_request:
     branches:
       - "*"
   schedule:
     - cron: "0 13 * * 1"
+  workflow_dispatch:
+
+concurrency:
+  group: ${{ github.workflow }}-${{ github.ref }}
+  cancel-in-progress: true
 
 jobs:
   build:
     name: Build (${{ matrix.python-version }} | ${{ matrix.os }})
+    if: github.repository == 'xgcm/aerobulk-python'
     runs-on: ${{ matrix.os }}
     timeout-minutes: 30
     defaults:
       run:
         shell: bash -l {0}
     strategy:
       fail-fast: false
       matrix:
         os: ["ubuntu-latest"]
-        python-version: ["3.8", "3.9", "3.10"]
+        python-version: ["3.8", "3.9", "3.10", "3.11"]
     steps:
       - uses: actions/checkout@v3
         with:
           submodules: recursive
-      - name: Cache conda
-        uses: actions/cache@v3.0.1
-        env:
-          # Increase this value to reset cache if ci/environment.yml has not changed
-          CACHE_NUMBER: 0
-        with:
-          path: ~/conda_pkgs_dir
-          key: ${{ runner.os }}-conda-${{ env.CACHE_NUMBER }}-${{ hashFiles('ci/environment.yml') }}
-      - uses: conda-incubator/setup-miniconda@v2
+      - name: Create conda environment
+        uses: mamba-org/provision-with-micromamba@main
         with:
-          channels: conda-forge
-          mamba-version: '*'
-          channel-priority: strict
-          activate-environment: test_env_aerobulk_python # Defined in ci/environment.yml
-          auto-update-conda: false
-          python-version: ${{ matrix.python-version }}
+          cache-downloads: true
+          micromamba-version: 'latest'
           environment-file: ci/environment.yml
-          use-only-tar-bz2: true # IMPORTANT: This needs to be set for caching to work properly!
-      - name: Set up conda environment
+          extra-specs: |
+            python=${{ matrix.python-version }}
+      - name: Install aerobulk-python
         run: |
           python -m pip install -e . --no-deps
           conda list
       - name: Run Tests
         run: |
           pytest -vv --cov=./ --cov-report=xml
       - name: Upload code coverage to Codecov
-        uses: codecov/codecov-action@v3.1.0
+        uses: codecov/codecov-action@v3.1.1
         with:
           file: ./coverage.xml
           flags: unittests
           env_vars: OS,PYTHON
           name: codecov-umbrella
           fail_ci_if_error: false
```

### Comparing `aerobulk-python-0.4.0rc0/.github/workflows/publish.yml` & `aerobulk-python-0.4.1/.github/workflows/publish.yml`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     steps:
       - uses: actions/checkout@v3
         with:
           submodules: recursive
       - name: Set up Python
         uses: actions/setup-python@v3
         with:
-          python-version: '3.x'
+          python-version: '3.11'
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           pip install numpy setuptools setuptools-scm wheel twine
       - name: Build tarball
         run: python setup.py sdist
       - name: Check dist
```

### Comparing `aerobulk-python-0.4.0rc0/LICENSE` & `aerobulk-python-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aerobulk-python-0.4.0rc0/PKG-INFO` & `aerobulk-python-0.4.1/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: aerobulk-python
-Version: 0.4.0rc0
+Version: 0.4.1
 Summary: General Circulation Model Postprocessing with xarray
 Home-page: https://github.com/xgcm/aerobulk-python
 Author: aerobulk-python Developers
 Author-email: julius@ldeo.columbia.edu
 License: GPLv3
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.8
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8, <3.12
 License-File: LICENSE
```

### Comparing `aerobulk-python-0.4.0rc0/README.md` & `aerobulk-python-0.4.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,22 @@
 [![pre-commit.ci status](https://results.pre-commit.ci/badge/github/xgcm/aerobulk-python/main.svg)](https://results.pre-commit.ci/latest/github/xgcm/aerobulk-python/main)
 
 # aerobulk-python
 A python wrapper for aerobulk (https://github.com/brodeau/aerobulk)
 
 ## Installation
+Due to the heavy dependencies in this package we recommend installing the package from conda-forge with mamba/conda
+
+```
+mamba install -c conda-forge aerobulk-python
+```
+or
+```
+conda install -c conda-forge aerobulk-python
+```
 
 ## aerobulk-python developer guide
 
 These are the steps to install and develop the package locally
 
 1. Set up a development environment.
 ```
```

### Comparing `aerobulk-python-0.4.0rc0/setup.py` & `aerobulk-python-0.4.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,17 +97,18 @@
         "Intended Audience :: Science/Research",
         "Topic :: Scientific/Engineering",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
     install_requires=install_requires,
-    python_requires=">=3.8",
+    python_requires=">=3.8, <3.12",
     # long_description=long_description,
     # long_description_content_type="text/x-rst",
     setup_requires="setuptools_scm",
     use_scm_version={
         "write_to": "source/aerobulk/_version.py",
         "write_to_template": '__version__ = "{version}"',
         "tag_regex": r"^(?P<prefix>v)?(?P<version>[^\+]+)(?P<suffix>.*)?$",
```

### Comparing `aerobulk-python-0.4.0rc0/source/aerobulk/flux.py` & `aerobulk-python-0.4.1/source/aerobulk/flux.py`

 * *Files 0% similar despite different names*

```diff
@@ -314,15 +314,14 @@
     slp=101000.0,
     algo="coare3p0",
     zt=2,
     zu=10,
     niter=6,
     input_range_check=True,
 ):
-
     """xarray wrapper for aerobulk with skin correction.
 
     Warnings
     --------
     !ATTENTION If input not provided in the units shown in [] below the code will crash.
     !ATTENTION Missing values taken from NaN values in sst field. No input variables may have NaN values that are not reflected in the sst.
```

### Comparing `aerobulk-python-0.4.0rc0/source/aerobulk_python.egg-info/PKG-INFO` & `aerobulk-python-0.4.1/source/aerobulk_python.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: aerobulk-python
-Version: 0.4.0rc0
+Version: 0.4.1
 Summary: General Circulation Model Postprocessing with xarray
 Home-page: https://github.com/xgcm/aerobulk-python
 Author: aerobulk-python Developers
 Author-email: julius@ldeo.columbia.edu
 License: GPLv3
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.8
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8, <3.12
 License-File: LICENSE
```

### Comparing `aerobulk-python-0.4.0rc0/source/aerobulk_python.egg-info/SOURCES.txt` & `aerobulk-python-0.4.1/source/aerobulk_python.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 .gitattributes
 .gitignore
 .gitmodules
 .pre-commit-config.yaml
+CITATION.cff
 LICENSE
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
 ./source/fortran/mod_aerobulk_wrap_noskin.f90
 ./source/fortran/mod_aerobulk_wrap_skin.f90
```

### Comparing `aerobulk-python-0.4.0rc0/source/fortran/aerobulk/src/mod_aerobulk.f90` & `aerobulk-python-0.4.1/source/fortran/aerobulk/src/mod_aerobulk.f90`

 * *Files identical despite different names*

### Comparing `aerobulk-python-0.4.0rc0/source/fortran/aerobulk/src/mod_aerobulk_compute.f90` & `aerobulk-python-0.4.1/source/fortran/aerobulk/src/mod_aerobulk_compute.f90`

 * *Files identical despite different names*

### Comparing `aerobulk-python-0.4.0rc0/source/fortran/aerobulk/src/mod_blk_andreas.f90` & `aerobulk-python-0.4.1/source/fortran/aerobulk/src/mod_blk_andreas.f90`

 * *Files identical despite different names*

### Comparing `aerobulk-python-0.4.0rc0/source/fortran/aerobulk/src/mod_blk_coare3p0.f90` & `aerobulk-python-0.4.1/source/fortran/aerobulk/src/mod_blk_coare3p0.f90`

 * *Files identical despite different names*

### Comparing `aerobulk-python-0.4.0rc0/source/fortran/aerobulk/src/mod_blk_coare3p6.f90` & `aerobulk-python-0.4.1/source/fortran/aerobulk/src/mod_blk_coare3p6.f90`

 * *Files identical despite different names*

### Comparing `aerobulk-python-0.4.0rc0/source/fortran/aerobulk/src/mod_blk_ecmwf.f90` & `aerobulk-python-0.4.1/source/fortran/aerobulk/src/mod_blk_ecmwf.f90`

 * *Files identical despite different names*

### Comparing `aerobulk-python-0.4.0rc0/source/fortran/aerobulk/src/mod_blk_ncar.f90` & `aerobulk-python-0.4.1/source/fortran/aerobulk/src/mod_blk_ncar.f90`

 * *Files identical despite different names*

### Comparing `aerobulk-python-0.4.0rc0/source/fortran/aerobulk/src/mod_blk_neutral_10m.f90` & `aerobulk-python-0.4.1/source/fortran/aerobulk/src/mod_blk_neutral_10m.f90`

 * *Files identical despite different names*

### Comparing `aerobulk-python-0.4.0rc0/source/fortran/aerobulk/src/mod_common_coare.f90` & `aerobulk-python-0.4.1/source/fortran/aerobulk/src/mod_common_coare.f90`

 * *Files identical despite different names*

### Comparing `aerobulk-python-0.4.0rc0/source/fortran/aerobulk/src/mod_const.f90` & `aerobulk-python-0.4.1/source/fortran/aerobulk/src/mod_const.f90`

 * *Files identical despite different names*

### Comparing `aerobulk-python-0.4.0rc0/source/fortran/aerobulk/src/mod_phymbl.f90` & `aerobulk-python-0.4.1/source/fortran/aerobulk/src/mod_phymbl.f90`

 * *Files identical despite different names*

### Comparing `aerobulk-python-0.4.0rc0/source/fortran/aerobulk/src/mod_skin_coare.f90` & `aerobulk-python-0.4.1/source/fortran/aerobulk/src/mod_skin_coare.f90`

 * *Files identical despite different names*

### Comparing `aerobulk-python-0.4.0rc0/source/fortran/aerobulk/src/mod_skin_ecmwf.f90` & `aerobulk-python-0.4.1/source/fortran/aerobulk/src/mod_skin_ecmwf.f90`

 * *Files identical despite different names*

### Comparing `aerobulk-python-0.4.0rc0/source/fortran/mod_aerobulk_wrap_noskin.f90` & `aerobulk-python-0.4.1/source/fortran/mod_aerobulk_wrap_noskin.f90`

 * *Files identical despite different names*

### Comparing `aerobulk-python-0.4.0rc0/source/fortran/mod_aerobulk_wrap_noskin.pyf` & `aerobulk-python-0.4.1/source/fortran/mod_aerobulk_wrap_noskin.pyf`

 * *Files identical despite different names*

### Comparing `aerobulk-python-0.4.0rc0/source/fortran/mod_aerobulk_wrap_skin.f90` & `aerobulk-python-0.4.1/source/fortran/mod_aerobulk_wrap_skin.f90`

 * *Files identical despite different names*

### Comparing `aerobulk-python-0.4.0rc0/source/fortran/mod_aerobulk_wrap_skin.pyf` & `aerobulk-python-0.4.1/source/fortran/mod_aerobulk_wrap_skin.pyf`

 * *Files identical despite different names*

### Comparing `aerobulk-python-0.4.0rc0/tests/create_test_data.py` & `aerobulk-python-0.4.1/tests/create_test_data.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,17 +32,17 @@
         # adds random noise scaled by a percentage of the value
         randomize_factor = 0.001
         randomize_range = value * randomize_factor
         noise = np.random.rand(*shape) * randomize_range
         arr = arr + noise
 
         if land_mask:
-            arr[
-                multi_indices[0], multi_indices[1], :
-            ] = np.nan  # add NaNs to mimic land mask
+            arr[multi_indices[0], multi_indices[1], :] = (
+                np.nan
+            )  # add NaNs to mimic land mask
         if use_xr:
             arr = xr.DataArray(arr)
             if chunks:
                 arr = arr.chunk(chunks)
         return arr
 
     if skin_correction:
```

### Comparing `aerobulk-python-0.4.0rc0/tests/test_flux_np.py` & `aerobulk-python-0.4.1/tests/test_flux_np.py`

 * *Files identical despite different names*

### Comparing `aerobulk-python-0.4.0rc0/tests/test_flux_xr.py` & `aerobulk-python-0.4.1/tests/test_flux_xr.py`

 * *Files identical despite different names*

### Comparing `aerobulk-python-0.4.0rc0/tests/test_fortran.py` & `aerobulk-python-0.4.1/tests/test_fortran.py`

 * *Files identical despite different names*

