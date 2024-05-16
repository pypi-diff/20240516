# Comparing `tmp/erlab-2.5.0.tar.gz` & `tmp/erlab-2.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "erlab-2.5.0.tar", last modified: Mon May 13 08:15:48 2024, max compression
+gzip compressed data, was "erlab-2.5.1.tar", last modified: Wed May 15 13:38:01 2024, max compression
```

## Comparing `erlab-2.5.0.tar` & `erlab-2.5.1.tar`

### file list

```diff
@@ -1,186 +1,195 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 08:15:48.800446 erlab-2.5.0/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 08:15:48.756446 erlab-2.5.0/.github/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 08:15:48.760446 erlab-2.5.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 root         (0) root         (0)     2200 2024-05-13 08:15:39.000000 erlab-2.5.0/.github/ISSUE_TEMPLATE/bug-report.yml
--rw-r--r--   0 root         (0) root         (0)      206 2024-05-13 08:15:39.000000 erlab-2.5.0/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 root         (0) root         (0)     1071 2024-05-13 08:15:39.000000 erlab-2.5.0/.github/ISSUE_TEMPLATE/feature-request.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 08:15:48.760446 erlab-2.5.0/.github/workflows/
--rw-r--r--   0 root         (0) root         (0)     1047 2024-05-13 08:15:39.000000 erlab-2.5.0/.github/workflows/pr.yml
--rw-r--r--   0 root         (0) root         (0)     1893 2024-05-13 08:15:39.000000 erlab-2.5.0/.github/workflows/release.yml
--rw-r--r--   0 root         (0) root         (0)     2898 2024-05-13 08:15:39.000000 erlab-2.5.0/.gitignore
--rw-r--r--   0 root         (0) root         (0)     1022 2024-05-13 08:15:39.000000 erlab-2.5.0/.pre-commit-config.yaml
--rw-r--r--   0 root         (0) root         (0)      793 2024-05-13 08:15:39.000000 erlab-2.5.0/.readthedocs.yaml
--rw-r--r--   0 root         (0) root         (0)   126450 2024-05-13 08:15:44.000000 erlab-2.5.0/CHANGELOG.md
--rw-r--r--   0 root         (0) root         (0)    35149 2024-05-13 08:15:39.000000 erlab-2.5.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)    48438 2024-05-13 08:15:48.800446 erlab-2.5.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1473 2024-05-13 08:15:39.000000 erlab-2.5.0/PythonInterface.ipf
--rw-r--r--   0 root         (0) root         (0)     5147 2024-05-13 08:15:39.000000 erlab-2.5.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 08:15:48.760446 erlab-2.5.0/docs/
--rw-r--r--   0 root         (0) root         (0)      638 2024-05-13 08:15:39.000000 erlab-2.5.0/docs/Makefile
--rw-r--r--   0 root         (0) root         (0)      726 2024-05-13 08:15:39.000000 erlab-2.5.0/docs/environment.yml
--rw-r--r--   0 root         (0) root         (0)      804 2024-05-13 08:15:39.000000 erlab-2.5.0/docs/make.bat
--rw-r--r--   0 root         (0) root         (0)       65 2024-05-13 08:15:39.000000 erlab-2.5.0/docs/requirements.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 08:15:48.764446 erlab-2.5.0/docs/source/
--rw-r--r--   0 root         (0) root         (0)       52 2024-05-13 08:15:39.000000 erlab-2.5.0/docs/source/bibliography.rst
--rw-r--r--   0 root         (0) root         (0)    18220 2024-05-13 08:15:39.000000 erlab-2.5.0/docs/source/conf.py
--rw-r--r--   0 root         (0) root         (0)    15203 2024-05-13 08:15:39.000000 erlab-2.5.0/docs/source/contributing.rst
--rw-r--r--   0 root         (0) root         (0)      106 2024-05-13 08:15:39.000000 erlab-2.5.0/docs/source/erlab.accessors.rst
--rw-r--r--   0 root         (0) root         (0)      101 2024-05-13 08:15:39.000000 erlab-2.5.0/docs/source/erlab.analysis.rst
--rw-r--r--   0 root         (0) root         (0)      485 2024-05-13 08:15:39.000000 erlab-2.5.0/docs/source/erlab.constants.rst
--rw-r--r--   0 root         (0) root         (0)      116 2024-05-13 08:15:39.000000 erlab-2.5.0/docs/source/erlab.interactive.rst
--rw-r--r--   0 root         (0) root         (0)       81 2024-05-13 08:15:39.000000 erlab-2.5.0/docs/source/erlab.io.rst
--rw-r--r--   0 root         (0) root         (0)      236 2024-05-13 08:15:39.000000 erlab-2.5.0/docs/source/erlab.lattice.rst
--rw-r--r--   0 root         (0) root         (0)      224 2024-05-13 08:15:39.000000 erlab-2.5.0/docs/source/erlab.parallel.rst
--rw-r--r--   0 root         (0) root         (0)      174 2024-05-13 08:15:39.000000 erlab-2.5.0/docs/source/erlab.plotting.rst
--rw-r--r--   0 root         (0) root         (0)     5039 2024-05-13 08:15:39.000000 erlab-2.5.0/docs/source/getting-started.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 08:15:48.772446 erlab-2.5.0/docs/source/images/
--rw-r--r--   0 root         (0) root         (0)   328062 2024-05-13 08:15:39.000000 erlab-2.5.0/docs/source/images/flowchart_multiple.pdf
--rw-r--r--   0 root         (0) root         (0)   328737 2024-05-13 08:15:39.000000 erlab-2.5.0/docs/source/images/flowchart_single.pdf
--rw-r--r--   0 root         (0) root         (0)   996803 2024-05-13 08:15:39.000000 erlab-2.5.0/docs/source/images/imagetool_dark.png
--rw-r--r--   0 root         (0) root         (0)   966547 2024-05-13 08:15:39.000000 erlab-2.5.0/docs/source/images/imagetool_light.png
--rw-r--r--   0 root         (0) root         (0)   709231 2024-05-13 08:15:39.000000 erlab-2.5.0/docs/source/images/ktool_1_dark.png
--rw-r--r--   0 root         (0) root         (0)   694078 2024-05-13 08:15:39.000000 erlab-2.5.0/docs/source/images/ktool_1_light.png
--rw-r--r--   0 root         (0) root         (0)   703343 2024-05-13 08:15:39.000000 erlab-2.5.0/docs/source/images/ktool_2_dark.png
--rw-r--r--   0 root         (0) root         (0)   686688 2024-05-13 08:15:39.000000 erlab-2.5.0/docs/source/images/ktool_2_light.png
--rw-r--r--   0 root         (0) root         (0)     3119 2024-05-13 08:15:39.000000 erlab-2.5.0/docs/source/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 08:15:48.772446 erlab-2.5.0/docs/source/pyplots/
--rw-r--r--   0 root         (0) root         (0)     2604 2024-05-13 08:15:39.000000 erlab-2.5.0/docs/source/pyplots/norms.py
--rw-r--r--   0 root         (0) root         (0)     1470 2024-05-13 08:15:39.000000 erlab-2.5.0/docs/source/reference.rst
--rw-r--r--   0 root         (0) root         (0)     3099 2024-05-13 08:15:39.000000 erlab-2.5.0/docs/source/refs.bib
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 08:15:48.776446 erlab-2.5.0/docs/source/user-guide/
--rw-r--r--   0 root         (0) root         (0)    42435 2024-05-13 08:15:39.000000 erlab-2.5.0/docs/source/user-guide/curve-fitting.ipynb
--rw-r--r--   0 root         (0) root         (0)     2598 2024-05-13 08:15:39.000000 erlab-2.5.0/docs/source/user-guide/imagetool.rst
--rw-r--r--   0 root         (0) root         (0)     1291 2024-05-13 08:15:39.000000 erlab-2.5.0/docs/source/user-guide/index.rst
--rw-r--r--   0 root         (0) root         (0)    12039 2024-05-13 08:15:39.000000 erlab-2.5.0/docs/source/user-guide/indexing.ipynb
--rw-r--r--   0 root         (0) root         (0)    54817 2024-05-13 08:15:39.000000 erlab-2.5.0/docs/source/user-guide/io.ipynb
--rw-r--r--   0 root         (0) root         (0)    10710 2024-05-13 08:15:39.000000 erlab-2.5.0/docs/source/user-guide/kconv.ipynb
--rw-r--r--   0 root         (0) root         (0)    27572 2024-05-13 08:15:39.000000 erlab-2.5.0/docs/source/user-guide/plotting.ipynb
--rw-r--r--   0 root         (0) root         (0)      455 2024-05-13 08:15:39.000000 erlab-2.5.0/environment.yml
--rw-r--r--   0 root         (0) root         (0)     5369 2024-05-13 08:15:39.000000 erlab-2.5.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)      299 2024-05-13 08:15:39.000000 erlab-2.5.0/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-13 08:15:48.800446 erlab-2.5.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 08:15:48.756446 erlab-2.5.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 08:15:48.776446 erlab-2.5.0/src/erlab/
--rw-r--r--   0 root         (0) root         (0)       60 2024-05-13 08:15:44.000000 erlab-2.5.0/src/erlab/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 08:15:48.780446 erlab-2.5.0/src/erlab/accessors/
--rw-r--r--   0 root         (0) root         (0)      897 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/accessors/__init__.py
--rw-r--r--   0 root         (0) root         (0)    26123 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/accessors/fit.py
--rw-r--r--   0 root         (0) root         (0)    30007 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/accessors/kspace.py
--rw-r--r--   0 root         (0) root         (0)    14898 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/accessors/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 08:15:48.780446 erlab-2.5.0/src/erlab/analysis/
--rw-r--r--   0 root         (0) root         (0)      880 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/analysis/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5322 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/analysis/correlation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 08:15:48.780446 erlab-2.5.0/src/erlab/analysis/fit/
--rw-r--r--   0 root         (0) root         (0)      168 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/analysis/fit/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 08:15:48.780446 erlab-2.5.0/src/erlab/analysis/fit/functions/
--rw-r--r--   0 root         (0) root         (0)      957 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/analysis/fit/functions/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10779 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/analysis/fit/functions/dynamic.py
--rw-r--r--   0 root         (0) root         (0)     9594 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/analysis/fit/functions/general.py
--rw-r--r--   0 root         (0) root         (0)     6905 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/analysis/fit/minuit.py
--rw-r--r--   0 root         (0) root         (0)    12739 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/analysis/fit/models.py
--rw-r--r--   0 root         (0) root         (0)     1112 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/analysis/fit/spline.py
--rw-r--r--   0 root         (0) root         (0)    20223 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/analysis/gold.py
--rw-r--r--   0 root         (0) root         (0)    27520 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/analysis/image.py
--rw-r--r--   0 root         (0) root         (0)    14968 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/analysis/interpolate.py
--rw-r--r--   0 root         (0) root         (0)    10276 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/analysis/kspace.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 08:15:48.784446 erlab-2.5.0/src/erlab/analysis/mask/
--rw-r--r--   0 root         (0) root         (0)     5397 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/analysis/mask/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8505 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/analysis/mask/polygon.py
--rw-r--r--   0 root         (0) root         (0)      878 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/analysis/transform.py
--rw-r--r--   0 root         (0) root         (0)     5443 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/analysis/utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 08:15:48.784446 erlab-2.5.0/src/erlab/characterization/
--rw-r--r--   0 root         (0) root         (0)      232 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/characterization/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2152 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 08:15:48.784446 erlab-2.5.0/src/erlab/interactive/
--rw-r--r--   0 root         (0) root         (0)      526 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/interactive/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14330 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/interactive/bzplot.py
--rw-r--r--   0 root         (0) root         (0)    21371 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/interactive/colors.py
--rw-r--r--   0 root         (0) root         (0)    23024 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/interactive/curvefittingtool.py
--rw-r--r--   0 root         (0) root         (0)    11891 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/interactive/derivative.py
--rw-r--r--   0 root         (0) root         (0)    16300 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/interactive/dtool.ui
--rw-r--r--   0 root         (0) root         (0)    19282 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/interactive/fermiedge.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 08:15:48.784446 erlab-2.5.0/src/erlab/interactive/imagetool/
--rw-r--r--   0 root         (0) root         (0)    20451 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/interactive/imagetool/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 08:15:48.788446 erlab-2.5.0/src/erlab/interactive/imagetool/_deprecated/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/interactive/imagetool/_deprecated/__init__.py
--rw-r--r--   0 root         (0) root         (0)    52053 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/interactive/imagetool/_deprecated/imagetool_mpl.py
--rw-r--r--   0 root         (0) root         (0)   114641 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/interactive/imagetool/_deprecated/imagetool_old.py
--rw-r--r--   0 root         (0) root         (0)    27909 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/interactive/imagetool/controls.py
--rw-r--r--   0 root         (0) root         (0)    57841 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/interactive/imagetool/core.py
--rw-r--r--   0 root         (0) root         (0)    14551 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/interactive/imagetool/fastbinning.py
--rw-r--r--   0 root         (0) root         (0)    25642 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/interactive/imagetool/slicer.py
--rw-r--r--   0 root         (0) root         (0)    15979 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/interactive/kspace.py
--rw-r--r--   0 root         (0) root         (0)    19321 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/interactive/ktool.ui
--rw-r--r--   0 root         (0) root         (0)     2749 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/interactive/masktool.py
--rw-r--r--   0 root         (0) root         (0)    56647 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/interactive/utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 08:15:48.788446 erlab-2.5.0/src/erlab/io/
--rw-r--r--   0 root         (0) root         (0)     2194 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/io/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 08:15:48.788446 erlab-2.5.0/src/erlab/io/characterization/
--rw-r--r--   0 root         (0) root         (0)      170 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/io/characterization/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3058 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/io/characterization/resistance.py
--rw-r--r--   0 root         (0) root         (0)     1981 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/io/characterization/xrd.py
--rw-r--r--   0 root         (0) root         (0)    43727 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/io/dataloader.py
--rw-r--r--   0 root         (0) root         (0)    12313 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/io/exampledata.py
--rw-r--r--   0 root         (0) root         (0)     6998 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/io/igor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 08:15:48.788446 erlab-2.5.0/src/erlab/io/plugins/
--rw-r--r--   0 root         (0) root         (0)      900 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/io/plugins/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3811 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/io/plugins/da30.py
--rw-r--r--   0 root         (0) root         (0)     1142 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/io/plugins/kriss.py
--rw-r--r--   0 root         (0) root         (0)     8166 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/io/plugins/merlin.py
--rw-r--r--   0 root         (0) root         (0)     7667 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/io/plugins/ssrl52.py
--rw-r--r--   0 root         (0) root         (0)     6737 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/io/utilities.py
--rw-r--r--   0 root         (0) root         (0)     2528 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/lattice.py
--rw-r--r--   0 root         (0) root         (0)     1522 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/parallel.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 08:15:48.792446 erlab-2.5.0/src/erlab/plotting/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 08:15:48.792446 erlab-2.5.0/src/erlab/plotting/IgorCT/
--rw-r--r--   0 root         (0) root         (0)     3379 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/plotting/IgorCT/Blue-White.txt
--rw-r--r--   0 root         (0) root         (0)     3456 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/plotting/IgorCT/BlueHot.ibw
--rw-r--r--   0 root         (0) root         (0)     3526 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/plotting/IgorCT/CTBlueWhite.ibw
--rw-r--r--   0 root         (0) root         (0)     3530 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/plotting/IgorCT/CTRainbowLIght.ibw
--rw-r--r--   0 root         (0) root         (0)     3531 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/plotting/IgorCT/CTRedTemperature.ibw
--rw-r--r--   0 root         (0) root         (0)     3456 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/plotting/IgorCT/ColdWarm.ibw
--rw-r--r--   0 root         (0) root         (0)     3456 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/plotting/IgorCT/PlanetEarth.ibw
--rw-r--r--   0 root         (0) root         (0)     1920 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/plotting/IgorCT/ametrine.ibw
--rw-r--r--   0 root         (0) root         (0)     2048 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/plotting/IgorCT/isolum.ibw
--rw-r--r--   0 root         (0) root         (0)     2048 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/plotting/IgorCT/morgenstemning.ibw
--rw-r--r--   0 root         (0) root         (0)     2113 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/plotting/__init__.py
--rw-r--r--   0 root         (0) root         (0)    30641 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/plotting/annotations.py
--rw-r--r--   0 root         (0) root         (0)    18686 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/plotting/atoms.py
--rw-r--r--   0 root         (0) root         (0)     4420 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/plotting/bz.py
--rw-r--r--   0 root         (0) root         (0)    39760 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/plotting/colors.py
--rw-r--r--   0 root         (0) root         (0)     2248 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/plotting/erplot.py
--rw-r--r--   0 root         (0) root         (0)    38515 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/plotting/general.py
--rw-r--r--   0 root         (0) root         (0)     2739 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/plotting/plot3d.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 08:15:48.796446 erlab-2.5.0/src/erlab/plotting/stylelib/
--rw-r--r--   0 root         (0) root         (0)     6839 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/plotting/stylelib/fira.mplstyle
--rw-r--r--   0 root         (0) root         (0)     6826 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/plotting/stylelib/firalight.mplstyle
--rw-r--r--   0 root         (0) root         (0)    14358 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/plotting/stylelib/khan.mplstyle
--rw-r--r--   0 root         (0) root         (0)     9160 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/plotting/stylelib/nature.mplstyle
--rw-r--r--   0 root         (0) root         (0)      630 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/plotting/stylelib/poster.mplstyle
--rw-r--r--   0 root         (0) root         (0)     7023 2024-05-13 08:15:39.000000 erlab-2.5.0/src/erlab/plotting/stylelib/times.mplstyle
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 08:15:48.800446 erlab-2.5.0/src/erlab.egg-info/
--rw-r--r--   0 root         (0) root         (0)    48438 2024-05-13 08:15:48.000000 erlab-2.5.0/src/erlab.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4973 2024-05-13 08:15:48.000000 erlab-2.5.0/src/erlab.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-13 08:15:48.000000 erlab-2.5.0/src/erlab.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      631 2024-05-13 08:15:48.000000 erlab-2.5.0/src/erlab.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2024-05-13 08:15:48.000000 erlab-2.5.0/src/erlab.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 08:15:48.796446 erlab-2.5.0/templates/
--rw-r--r--   0 root         (0) root         (0)     1063 2024-05-13 08:15:39.000000 erlab-2.5.0/templates/.macros.j2
--rw-r--r--   0 root         (0) root         (0)      161 2024-05-13 08:15:39.000000 erlab-2.5.0/templates/.release_notes.md.j2
--rw-r--r--   0 root         (0) root         (0)      423 2024-05-13 08:15:39.000000 erlab-2.5.0/templates/CHANGELOG.md.j2
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 08:15:48.756446 erlab-2.5.0/tests/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 08:15:48.796446 erlab-2.5.0/tests/accessors/
--rw-r--r--   0 root         (0) root         (0)     5785 2024-05-13 08:15:39.000000 erlab-2.5.0/tests/accessors/test_fit.py
--rw-r--r--   0 root         (0) root         (0)     4035 2024-05-13 08:15:39.000000 erlab-2.5.0/tests/accessors/test_kspace.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 08:15:48.796446 erlab-2.5.0/tests/analysis/
--rw-r--r--   0 root         (0) root         (0)     1020 2024-05-13 08:15:39.000000 erlab-2.5.0/tests/analysis/test_fastbinning.py
--rw-r--r--   0 root         (0) root         (0)     4497 2024-05-13 08:15:39.000000 erlab-2.5.0/tests/analysis/test_fit_functions_dynamic.py
--rw-r--r--   0 root         (0) root         (0)     4794 2024-05-13 08:15:39.000000 erlab-2.5.0/tests/analysis/test_fit_functions_general.py
--rw-r--r--   0 root         (0) root         (0)     6035 2024-05-13 08:15:39.000000 erlab-2.5.0/tests/analysis/test_fit_models.py
--rw-r--r--   0 root         (0) root         (0)     5228 2024-05-13 08:15:39.000000 erlab-2.5.0/tests/analysis/test_image.py
--rw-r--r--   0 root         (0) root         (0)     3909 2024-05-13 08:15:39.000000 erlab-2.5.0/tests/analysis/test_image_savgol.py
--rw-r--r--   0 root         (0) root         (0)     3126 2024-05-13 08:15:39.000000 erlab-2.5.0/tests/analysis/test_interpolate.py
--rw-r--r--   0 root         (0) root         (0)     1513 2024-05-13 08:15:39.000000 erlab-2.5.0/tests/analysis/test_kspace.py
--rw-r--r--   0 root         (0) root         (0)      718 2024-05-13 08:15:39.000000 erlab-2.5.0/tests/analysis/test_utilities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-13 08:15:48.800446 erlab-2.5.0/tests/io/
--rw-r--r--   0 root         (0) root         (0)     9385 2024-05-13 08:15:39.000000 erlab-2.5.0/tests/io/test_dataloader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 13:38:01.457206 erlab-2.5.1/
+-rw-r--r--   0 root         (0) root         (0)       99 2024-05-15 13:37:52.000000 erlab-2.5.1/.codecov.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 13:38:01.405206 erlab-2.5.1/.github/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 13:38:01.413206 erlab-2.5.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 root         (0) root         (0)     2200 2024-05-15 13:37:52.000000 erlab-2.5.1/.github/ISSUE_TEMPLATE/bug-report.yml
+-rw-r--r--   0 root         (0) root         (0)      206 2024-05-15 13:37:52.000000 erlab-2.5.1/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 root         (0) root         (0)     1071 2024-05-15 13:37:52.000000 erlab-2.5.1/.github/ISSUE_TEMPLATE/feature-request.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 13:38:01.413206 erlab-2.5.1/.github/workflows/
+-rw-r--r--   0 root         (0) root         (0)     1590 2024-05-15 13:37:52.000000 erlab-2.5.1/.github/workflows/pr.yml
+-rw-r--r--   0 root         (0) root         (0)     2457 2024-05-15 13:37:52.000000 erlab-2.5.1/.github/workflows/release.yml
+-rw-r--r--   0 root         (0) root         (0)     2898 2024-05-15 13:37:52.000000 erlab-2.5.1/.gitignore
+-rw-r--r--   0 root         (0) root         (0)     1022 2024-05-15 13:37:52.000000 erlab-2.5.1/.pre-commit-config.yaml
+-rw-r--r--   0 root         (0) root         (0)      793 2024-05-15 13:37:52.000000 erlab-2.5.1/.readthedocs.yaml
+-rw-r--r--   0 root         (0) root         (0)   126530 2024-05-15 13:37:57.000000 erlab-2.5.1/CHANGELOG.md
+-rw-r--r--   0 root         (0) root         (0)    35149 2024-05-15 13:37:52.000000 erlab-2.5.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    48524 2024-05-15 13:38:01.457206 erlab-2.5.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1473 2024-05-15 13:37:52.000000 erlab-2.5.1/PythonInterface.ipf
+-rw-r--r--   0 root         (0) root         (0)     5147 2024-05-15 13:37:52.000000 erlab-2.5.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 13:38:01.417206 erlab-2.5.1/docs/
+-rw-r--r--   0 root         (0) root         (0)      638 2024-05-15 13:37:52.000000 erlab-2.5.1/docs/Makefile
+-rw-r--r--   0 root         (0) root         (0)      726 2024-05-15 13:37:52.000000 erlab-2.5.1/docs/environment.yml
+-rw-r--r--   0 root         (0) root         (0)      804 2024-05-15 13:37:52.000000 erlab-2.5.1/docs/make.bat
+-rw-r--r--   0 root         (0) root         (0)       65 2024-05-15 13:37:52.000000 erlab-2.5.1/docs/requirements.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 13:38:01.417206 erlab-2.5.1/docs/source/
+-rw-r--r--   0 root         (0) root         (0)       52 2024-05-15 13:37:52.000000 erlab-2.5.1/docs/source/bibliography.rst
+-rw-r--r--   0 root         (0) root         (0)    18220 2024-05-15 13:37:52.000000 erlab-2.5.1/docs/source/conf.py
+-rw-r--r--   0 root         (0) root         (0)    15203 2024-05-15 13:37:52.000000 erlab-2.5.1/docs/source/contributing.rst
+-rw-r--r--   0 root         (0) root         (0)      106 2024-05-15 13:37:52.000000 erlab-2.5.1/docs/source/erlab.accessors.rst
+-rw-r--r--   0 root         (0) root         (0)      101 2024-05-15 13:37:52.000000 erlab-2.5.1/docs/source/erlab.analysis.rst
+-rw-r--r--   0 root         (0) root         (0)      485 2024-05-15 13:37:52.000000 erlab-2.5.1/docs/source/erlab.constants.rst
+-rw-r--r--   0 root         (0) root         (0)      116 2024-05-15 13:37:52.000000 erlab-2.5.1/docs/source/erlab.interactive.rst
+-rw-r--r--   0 root         (0) root         (0)       81 2024-05-15 13:37:52.000000 erlab-2.5.1/docs/source/erlab.io.rst
+-rw-r--r--   0 root         (0) root         (0)      236 2024-05-15 13:37:52.000000 erlab-2.5.1/docs/source/erlab.lattice.rst
+-rw-r--r--   0 root         (0) root         (0)      224 2024-05-15 13:37:52.000000 erlab-2.5.1/docs/source/erlab.parallel.rst
+-rw-r--r--   0 root         (0) root         (0)      174 2024-05-15 13:37:52.000000 erlab-2.5.1/docs/source/erlab.plotting.rst
+-rw-r--r--   0 root         (0) root         (0)     5039 2024-05-15 13:37:52.000000 erlab-2.5.1/docs/source/getting-started.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 13:38:01.425206 erlab-2.5.1/docs/source/images/
+-rw-r--r--   0 root         (0) root         (0)   328062 2024-05-15 13:37:52.000000 erlab-2.5.1/docs/source/images/flowchart_multiple.pdf
+-rw-r--r--   0 root         (0) root         (0)   328737 2024-05-15 13:37:52.000000 erlab-2.5.1/docs/source/images/flowchart_single.pdf
+-rw-r--r--   0 root         (0) root         (0)   996803 2024-05-15 13:37:52.000000 erlab-2.5.1/docs/source/images/imagetool_dark.png
+-rw-r--r--   0 root         (0) root         (0)   966547 2024-05-15 13:37:52.000000 erlab-2.5.1/docs/source/images/imagetool_light.png
+-rw-r--r--   0 root         (0) root         (0)   709231 2024-05-15 13:37:52.000000 erlab-2.5.1/docs/source/images/ktool_1_dark.png
+-rw-r--r--   0 root         (0) root         (0)   694078 2024-05-15 13:37:52.000000 erlab-2.5.1/docs/source/images/ktool_1_light.png
+-rw-r--r--   0 root         (0) root         (0)   703343 2024-05-15 13:37:52.000000 erlab-2.5.1/docs/source/images/ktool_2_dark.png
+-rw-r--r--   0 root         (0) root         (0)   686688 2024-05-15 13:37:52.000000 erlab-2.5.1/docs/source/images/ktool_2_light.png
+-rw-r--r--   0 root         (0) root         (0)     3119 2024-05-15 13:37:52.000000 erlab-2.5.1/docs/source/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 13:38:01.429206 erlab-2.5.1/docs/source/pyplots/
+-rw-r--r--   0 root         (0) root         (0)     2604 2024-05-15 13:37:52.000000 erlab-2.5.1/docs/source/pyplots/norms.py
+-rw-r--r--   0 root         (0) root         (0)     1470 2024-05-15 13:37:52.000000 erlab-2.5.1/docs/source/reference.rst
+-rw-r--r--   0 root         (0) root         (0)     3099 2024-05-15 13:37:52.000000 erlab-2.5.1/docs/source/refs.bib
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 13:38:01.429206 erlab-2.5.1/docs/source/user-guide/
+-rw-r--r--   0 root         (0) root         (0)    42435 2024-05-15 13:37:52.000000 erlab-2.5.1/docs/source/user-guide/curve-fitting.ipynb
+-rw-r--r--   0 root         (0) root         (0)     2598 2024-05-15 13:37:52.000000 erlab-2.5.1/docs/source/user-guide/imagetool.rst
+-rw-r--r--   0 root         (0) root         (0)     1291 2024-05-15 13:37:52.000000 erlab-2.5.1/docs/source/user-guide/index.rst
+-rw-r--r--   0 root         (0) root         (0)    12039 2024-05-15 13:37:52.000000 erlab-2.5.1/docs/source/user-guide/indexing.ipynb
+-rw-r--r--   0 root         (0) root         (0)    54817 2024-05-15 13:37:52.000000 erlab-2.5.1/docs/source/user-guide/io.ipynb
+-rw-r--r--   0 root         (0) root         (0)    10710 2024-05-15 13:37:52.000000 erlab-2.5.1/docs/source/user-guide/kconv.ipynb
+-rw-r--r--   0 root         (0) root         (0)    27572 2024-05-15 13:37:52.000000 erlab-2.5.1/docs/source/user-guide/plotting.ipynb
+-rw-r--r--   0 root         (0) root         (0)      455 2024-05-15 13:37:52.000000 erlab-2.5.1/environment.yml
+-rw-r--r--   0 root         (0) root         (0)     5492 2024-05-15 13:37:52.000000 erlab-2.5.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      299 2024-05-15 13:37:52.000000 erlab-2.5.1/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-15 13:38:01.457206 erlab-2.5.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 13:38:01.409206 erlab-2.5.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 13:38:01.429206 erlab-2.5.1/src/erlab/
+-rw-r--r--   0 root         (0) root         (0)       60 2024-05-15 13:37:57.000000 erlab-2.5.1/src/erlab/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 13:38:01.433206 erlab-2.5.1/src/erlab/accessors/
+-rw-r--r--   0 root         (0) root         (0)      897 2024-05-15 13:37:52.000000 erlab-2.5.1/src/erlab/accessors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    26123 2024-05-15 13:37:52.000000 erlab-2.5.1/src/erlab/accessors/fit.py
+-rw-r--r--   0 root         (0) root         (0)    30007 2024-05-15 13:37:52.000000 erlab-2.5.1/src/erlab/accessors/kspace.py
+-rw-r--r--   0 root         (0) root         (0)    14898 2024-05-15 13:37:52.000000 erlab-2.5.1/src/erlab/accessors/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 13:38:01.433206 erlab-2.5.1/src/erlab/analysis/
+-rw-r--r--   0 root         (0) root         (0)      880 2024-05-15 13:37:52.000000 erlab-2.5.1/src/erlab/analysis/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5322 2024-05-15 13:37:52.000000 erlab-2.5.1/src/erlab/analysis/correlation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 13:38:01.437206 erlab-2.5.1/src/erlab/analysis/fit/
+-rw-r--r--   0 root         (0) root         (0)      168 2024-05-15 13:37:52.000000 erlab-2.5.1/src/erlab/analysis/fit/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 13:38:01.437206 erlab-2.5.1/src/erlab/analysis/fit/functions/
+-rw-r--r--   0 root         (0) root         (0)      957 2024-05-15 13:37:52.000000 erlab-2.5.1/src/erlab/analysis/fit/functions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10779 2024-05-15 13:37:52.000000 erlab-2.5.1/src/erlab/analysis/fit/functions/dynamic.py
+-rw-r--r--   0 root         (0) root         (0)     9594 2024-05-15 13:37:52.000000 erlab-2.5.1/src/erlab/analysis/fit/functions/general.py
+-rw-r--r--   0 root         (0) root         (0)     6905 2024-05-15 13:37:52.000000 erlab-2.5.1/src/erlab/analysis/fit/minuit.py
+-rw-r--r--   0 root         (0) root         (0)    12746 2024-05-15 13:37:52.000000 erlab-2.5.1/src/erlab/analysis/fit/models.py
+-rw-r--r--   0 root         (0) root         (0)     1112 2024-05-15 13:37:52.000000 erlab-2.5.1/src/erlab/analysis/fit/spline.py
+-rw-r--r--   0 root         (0) root         (0)    20223 2024-05-15 13:37:52.000000 erlab-2.5.1/src/erlab/analysis/gold.py
+-rw-r--r--   0 root         (0) root         (0)    27520 2024-05-15 13:37:52.000000 erlab-2.5.1/src/erlab/analysis/image.py
+-rw-r--r--   0 root         (0) root         (0)    14968 2024-05-15 13:37:52.000000 erlab-2.5.1/src/erlab/analysis/interpolate.py
+-rw-r--r--   0 root         (0) root         (0)    10276 2024-05-15 13:37:52.000000 erlab-2.5.1/src/erlab/analysis/kspace.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 13:38:01.437206 erlab-2.5.1/src/erlab/analysis/mask/
+-rw-r--r--   0 root         (0) root         (0)     5397 2024-05-15 13:37:52.000000 erlab-2.5.1/src/erlab/analysis/mask/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8505 2024-05-15 13:37:52.000000 erlab-2.5.1/src/erlab/analysis/mask/polygon.py
+-rw-r--r--   0 root         (0) root         (0)      878 2024-05-15 13:37:52.000000 erlab-2.5.1/src/erlab/analysis/transform.py
+-rw-r--r--   0 root         (0) root         (0)     5443 2024-05-15 13:37:52.000000 erlab-2.5.1/src/erlab/analysis/utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 13:38:01.437206 erlab-2.5.1/src/erlab/characterization/
+-rw-r--r--   0 root         (0) root         (0)      232 2024-05-15 13:37:52.000000 erlab-2.5.1/src/erlab/characterization/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2152 2024-05-15 13:37:52.000000 erlab-2.5.1/src/erlab/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 13:38:01.437206 erlab-2.5.1/src/erlab/interactive/
+-rw-r--r--   0 root         (0) root         (0)      526 2024-05-15 13:37:52.000000 erlab-2.5.1/src/erlab/interactive/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14330 2024-05-15 13:37:52.000000 erlab-2.5.1/src/erlab/interactive/bzplot.py
+-rw-r--r--   0 root         (0) root         (0)    21371 2024-05-15 13:37:52.000000 erlab-2.5.1/src/erlab/interactive/colors.py
+-rw-r--r--   0 root         (0) root         (0)    23024 2024-05-15 13:37:52.000000 erlab-2.5.1/src/erlab/interactive/curvefittingtool.py
+-rw-r--r--   0 root         (0) root         (0)    11891 2024-05-15 13:37:52.000000 erlab-2.5.1/src/erlab/interactive/derivative.py
+-rw-r--r--   0 root         (0) root         (0)    16300 2024-05-15 13:37:52.000000 erlab-2.5.1/src/erlab/interactive/dtool.ui
+-rw-r--r--   0 root         (0) root         (0)    19282 2024-05-15 13:37:52.000000 erlab-2.5.1/src/erlab/interactive/fermiedge.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 13:38:01.441206 erlab-2.5.1/src/erlab/interactive/imagetool/
+-rw-r--r--   0 root         (0) root         (0)    17431 2024-05-15 13:37:52.000000 erlab-2.5.1/src/erlab/interactive/imagetool/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 13:38:01.441206 erlab-2.5.1/src/erlab/interactive/imagetool/_deprecated/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-15 13:37:52.000000 erlab-2.5.1/src/erlab/interactive/imagetool/_deprecated/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    52053 2024-05-15 13:37:52.000000 erlab-2.5.1/src/erlab/interactive/imagetool/_deprecated/imagetool_mpl.py
+-rw-r--r--   0 root         (0) root         (0)   114641 2024-05-15 13:37:52.000000 erlab-2.5.1/src/erlab/interactive/imagetool/_deprecated/imagetool_old.py
+-rw-r--r--   0 root         (0) root         (0)    27909 2024-05-15 13:37:52.000000 erlab-2.5.1/src/erlab/interactive/imagetool/controls.py
+-rw-r--r--   0 root         (0) root         (0)    57841 2024-05-15 13:37:52.000000 erlab-2.5.1/src/erlab/interactive/imagetool/core.py
+-rw-r--r--   0 root         (0) root         (0)    14551 2024-05-15 13:37:52.000000 erlab-2.5.1/src/erlab/interactive/imagetool/fastbinning.py
+-rw-r--r--   0 root         (0) root         (0)    25642 2024-05-15 13:37:52.000000 erlab-2.5.1/src/erlab/interactive/imagetool/slicer.py
+-rw-r--r--   0 root         (0) root         (0)    15979 2024-05-15 13:37:52.000000 erlab-2.5.1/src/erlab/interactive/kspace.py
+-rw-r--r--   0 root         (0) root         (0)    19321 2024-05-15 13:37:52.000000 erlab-2.5.1/src/erlab/interactive/ktool.ui
+-rw-r--r--   0 root         (0) root         (0)     2749 2024-05-15 13:37:52.000000 erlab-2.5.1/src/erlab/interactive/masktool.py
+-rw-r--r--   0 root         (0) root         (0)    56647 2024-05-15 13:37:52.000000 erlab-2.5.1/src/erlab/interactive/utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 13:38:01.441206 erlab-2.5.1/src/erlab/io/
+-rw-r--r--   0 root         (0) root         (0)     2194 2024-05-15 13:37:52.000000 erlab-2.5.1/src/erlab/io/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 13:38:01.445206 erlab-2.5.1/src/erlab/io/characterization/
+-rw-r--r--   0 root         (0) root         (0)      170 2024-05-15 13:37:52.000000 erlab-2.5.1/src/erlab/io/characterization/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3058 2024-05-15 13:37:52.000000 erlab-2.5.1/src/erlab/io/characterization/resistance.py
+-rw-r--r--   0 root         (0) root         (0)     1981 2024-05-15 13:37:52.000000 erlab-2.5.1/src/erlab/io/characterization/xrd.py
+-rw-r--r--   0 root         (0) root         (0)    43727 2024-05-15 13:37:52.000000 erlab-2.5.1/src/erlab/io/dataloader.py
+-rw-r--r--   0 root         (0) root         (0)    12460 2024-05-15 13:37:52.000000 erlab-2.5.1/src/erlab/io/exampledata.py
+-rw-r--r--   0 root         (0) root         (0)     6998 2024-05-15 13:37:52.000000 erlab-2.5.1/src/erlab/io/igor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 13:38:01.445206 erlab-2.5.1/src/erlab/io/plugins/
+-rw-r--r--   0 root         (0) root         (0)      900 2024-05-15 13:37:52.000000 erlab-2.5.1/src/erlab/io/plugins/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3811 2024-05-15 13:37:52.000000 erlab-2.5.1/src/erlab/io/plugins/da30.py
+-rw-r--r--   0 root         (0) root         (0)     1142 2024-05-15 13:37:52.000000 erlab-2.5.1/src/erlab/io/plugins/kriss.py
+-rw-r--r--   0 root         (0) root         (0)     8166 2024-05-15 13:37:52.000000 erlab-2.5.1/src/erlab/io/plugins/merlin.py
+-rw-r--r--   0 root         (0) root         (0)     7667 2024-05-15 13:37:52.000000 erlab-2.5.1/src/erlab/io/plugins/ssrl52.py
+-rw-r--r--   0 root         (0) root         (0)     6737 2024-05-15 13:37:52.000000 erlab-2.5.1/src/erlab/io/utilities.py
+-rw-r--r--   0 root         (0) root         (0)     2528 2024-05-15 13:37:52.000000 erlab-2.5.1/src/erlab/lattice.py
+-rw-r--r--   0 root         (0) root         (0)     1522 2024-05-15 13:37:52.000000 erlab-2.5.1/src/erlab/parallel.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 13:38:01.445206 erlab-2.5.1/src/erlab/plotting/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 13:38:01.449206 erlab-2.5.1/src/erlab/plotting/IgorCT/
+-rw-r--r--   0 root         (0) root         (0)     3379 2024-05-15 13:37:52.000000 erlab-2.5.1/src/erlab/plotting/IgorCT/Blue-White.txt
+-rw-r--r--   0 root         (0) root         (0)     3456 2024-05-15 13:37:52.000000 erlab-2.5.1/src/erlab/plotting/IgorCT/BlueHot.ibw
+-rw-r--r--   0 root         (0) root         (0)     3526 2024-05-15 13:37:52.000000 erlab-2.5.1/src/erlab/plotting/IgorCT/CTBlueWhite.ibw
+-rw-r--r--   0 root         (0) root         (0)     3530 2024-05-15 13:37:52.000000 erlab-2.5.1/src/erlab/plotting/IgorCT/CTRainbowLIght.ibw
+-rw-r--r--   0 root         (0) root         (0)     3531 2024-05-15 13:37:52.000000 erlab-2.5.1/src/erlab/plotting/IgorCT/CTRedTemperature.ibw
+-rw-r--r--   0 root         (0) root         (0)     3456 2024-05-15 13:37:52.000000 erlab-2.5.1/src/erlab/plotting/IgorCT/ColdWarm.ibw
+-rw-r--r--   0 root         (0) root         (0)     3456 2024-05-15 13:37:52.000000 erlab-2.5.1/src/erlab/plotting/IgorCT/PlanetEarth.ibw
+-rw-r--r--   0 root         (0) root         (0)     1920 2024-05-15 13:37:52.000000 erlab-2.5.1/src/erlab/plotting/IgorCT/ametrine.ibw
+-rw-r--r--   0 root         (0) root         (0)     2048 2024-05-15 13:37:52.000000 erlab-2.5.1/src/erlab/plotting/IgorCT/isolum.ibw
+-rw-r--r--   0 root         (0) root         (0)     2048 2024-05-15 13:37:52.000000 erlab-2.5.1/src/erlab/plotting/IgorCT/morgenstemning.ibw
+-rw-r--r--   0 root         (0) root         (0)     2113 2024-05-15 13:37:52.000000 erlab-2.5.1/src/erlab/plotting/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    30586 2024-05-15 13:37:52.000000 erlab-2.5.1/src/erlab/plotting/annotations.py
+-rw-r--r--   0 root         (0) root         (0)    18686 2024-05-15 13:37:52.000000 erlab-2.5.1/src/erlab/plotting/atoms.py
+-rw-r--r--   0 root         (0) root         (0)     4420 2024-05-15 13:37:52.000000 erlab-2.5.1/src/erlab/plotting/bz.py
+-rw-r--r--   0 root         (0) root         (0)    39760 2024-05-15 13:37:52.000000 erlab-2.5.1/src/erlab/plotting/colors.py
+-rw-r--r--   0 root         (0) root         (0)     2248 2024-05-15 13:37:52.000000 erlab-2.5.1/src/erlab/plotting/erplot.py
+-rw-r--r--   0 root         (0) root         (0)    38540 2024-05-15 13:37:52.000000 erlab-2.5.1/src/erlab/plotting/general.py
+-rw-r--r--   0 root         (0) root         (0)     2739 2024-05-15 13:37:52.000000 erlab-2.5.1/src/erlab/plotting/plot3d.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 13:38:01.449206 erlab-2.5.1/src/erlab/plotting/stylelib/
+-rw-r--r--   0 root         (0) root         (0)     6839 2024-05-15 13:37:52.000000 erlab-2.5.1/src/erlab/plotting/stylelib/fira.mplstyle
+-rw-r--r--   0 root         (0) root         (0)     6826 2024-05-15 13:37:52.000000 erlab-2.5.1/src/erlab/plotting/stylelib/firalight.mplstyle
+-rw-r--r--   0 root         (0) root         (0)    14358 2024-05-15 13:37:52.000000 erlab-2.5.1/src/erlab/plotting/stylelib/khan.mplstyle
+-rw-r--r--   0 root         (0) root         (0)     9160 2024-05-15 13:37:52.000000 erlab-2.5.1/src/erlab/plotting/stylelib/nature.mplstyle
+-rw-r--r--   0 root         (0) root         (0)      630 2024-05-15 13:37:52.000000 erlab-2.5.1/src/erlab/plotting/stylelib/poster.mplstyle
+-rw-r--r--   0 root         (0) root         (0)     7023 2024-05-15 13:37:52.000000 erlab-2.5.1/src/erlab/plotting/stylelib/times.mplstyle
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 13:38:01.453206 erlab-2.5.1/src/erlab.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    48524 2024-05-15 13:38:01.000000 erlab-2.5.1/src/erlab.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5139 2024-05-15 13:38:01.000000 erlab-2.5.1/src/erlab.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-15 13:38:01.000000 erlab-2.5.1/src/erlab.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      654 2024-05-15 13:38:01.000000 erlab-2.5.1/src/erlab.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2024-05-15 13:38:01.000000 erlab-2.5.1/src/erlab.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 13:38:01.449206 erlab-2.5.1/templates/
+-rw-r--r--   0 root         (0) root         (0)     1063 2024-05-15 13:37:52.000000 erlab-2.5.1/templates/.macros.j2
+-rw-r--r--   0 root         (0) root         (0)      161 2024-05-15 13:37:52.000000 erlab-2.5.1/templates/.release_notes.md.j2
+-rw-r--r--   0 root         (0) root         (0)      423 2024-05-15 13:37:52.000000 erlab-2.5.1/templates/CHANGELOG.md.j2
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 13:38:01.449206 erlab-2.5.1/tests/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 13:38:01.449206 erlab-2.5.1/tests/accessors/
+-rw-r--r--   0 root         (0) root         (0)     5785 2024-05-15 13:37:52.000000 erlab-2.5.1/tests/accessors/test_fit.py
+-rw-r--r--   0 root         (0) root         (0)     4035 2024-05-15 13:37:52.000000 erlab-2.5.1/tests/accessors/test_kspace.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 13:38:01.453206 erlab-2.5.1/tests/analysis/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 13:38:01.453206 erlab-2.5.1/tests/analysis/fit/
+-rw-r--r--   0 root         (0) root         (0)     4497 2024-05-15 13:37:52.000000 erlab-2.5.1/tests/analysis/fit/test_functions_dynamic.py
+-rw-r--r--   0 root         (0) root         (0)     4794 2024-05-15 13:37:52.000000 erlab-2.5.1/tests/analysis/fit/test_functions_general.py
+-rw-r--r--   0 root         (0) root         (0)     1087 2024-05-15 13:37:52.000000 erlab-2.5.1/tests/analysis/fit/test_minuit.py
+-rw-r--r--   0 root         (0) root         (0)     6035 2024-05-15 13:37:52.000000 erlab-2.5.1/tests/analysis/fit/test_models.py
+-rw-r--r--   0 root         (0) root         (0)     1020 2024-05-15 13:37:52.000000 erlab-2.5.1/tests/analysis/test_fastbinning.py
+-rw-r--r--   0 root         (0) root         (0)     1149 2024-05-15 13:37:52.000000 erlab-2.5.1/tests/analysis/test_gold.py
+-rw-r--r--   0 root         (0) root         (0)     5228 2024-05-15 13:37:52.000000 erlab-2.5.1/tests/analysis/test_image.py
+-rw-r--r--   0 root         (0) root         (0)     3909 2024-05-15 13:37:52.000000 erlab-2.5.1/tests/analysis/test_image_savgol.py
+-rw-r--r--   0 root         (0) root         (0)     3126 2024-05-15 13:37:52.000000 erlab-2.5.1/tests/analysis/test_interpolate.py
+-rw-r--r--   0 root         (0) root         (0)     1513 2024-05-15 13:37:52.000000 erlab-2.5.1/tests/analysis/test_kspace.py
+-rw-r--r--   0 root         (0) root         (0)      718 2024-05-15 13:37:52.000000 erlab-2.5.1/tests/analysis/test_utilities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 13:38:01.453206 erlab-2.5.1/tests/interactive/
+-rw-r--r--   0 root         (0) root         (0)     1749 2024-05-15 13:37:52.000000 erlab-2.5.1/tests/interactive/test_imagetool.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 13:38:01.453206 erlab-2.5.1/tests/io/
+-rw-r--r--   0 root         (0) root         (0)     9385 2024-05-15 13:37:52.000000 erlab-2.5.1/tests/io/test_dataloader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 13:38:01.453206 erlab-2.5.1/tests/plotting/
+-rw-r--r--   0 root         (0) root         (0)     2625 2024-05-15 13:37:52.000000 erlab-2.5.1/tests/plotting/test_general.py
+-rw-r--r--   0 root         (0) root         (0)      295 2024-05-15 13:37:52.000000 erlab-2.5.1/tests/test_constants.py
```

### Comparing `erlab-2.5.0/.github/ISSUE_TEMPLATE/bug-report.yml` & `erlab-2.5.1/.github/ISSUE_TEMPLATE/bug-report.yml`

 * *Files identical despite different names*

### Comparing `erlab-2.5.0/.github/ISSUE_TEMPLATE/feature-request.yml` & `erlab-2.5.1/.github/ISSUE_TEMPLATE/feature-request.yml`

 * *Files identical despite different names*

### Comparing `erlab-2.5.0/.github/workflows/release.yml` & `erlab-2.5.1/.github/workflows/release.yml`

 * *Files 16% similar despite different names*

```diff
@@ -5,38 +5,54 @@
     branches: [ "main" ]
   workflow_dispatch:
 
 jobs:
   test:
     name: Python ${{ matrix.python-version }} tests
     runs-on: ubuntu-latest
+    env:
+      DISPLAY: ':99.0'
     strategy:
       matrix:
         python-version: ["3.11", "3.12"]
 
     steps:
       - uses: actions/checkout@v4
         with:
           fetch-depth: 0
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python-version }}
 
+      - uses: tlambert03/setup-qt-libs@v1
+      - name: Setup for Qt testing
+        run: |
+          /sbin/start-stop-daemon --start --quiet --pidfile /tmp/custom_xvfb_99.pid --make-pidfile --background --exec /usr/bin/Xvfb -- :99 -screen 0 1920x1200x24 -ac +extension GLX
+
       - name: Install pytest and dependencies
         run: |
-          sudo apt update && sudo apt install -y libegl1-mesa-dev
           python -m pip install --upgrade pip
-          python -m pip install -r requirements.txt
-          python -m pip install -v . pytest pytest-xdist
-
+          python -m pip install -v .[complete] pyqt6
 
       - name: Test with pytest
+        if: matrix.python-version != '3.12'
         run: |
-          pytest -v -n auto
+          pytest -v
+
+      - name: Test with pytest with coverage
+        if: matrix.python-version == '3.12'
+        run: |
+          pytest --cov erlab --cov-report xml -v
+
+      - name: Upload coverage to Codecov
+        if: matrix.python-version == '3.12'
+        uses: codecov/codecov-action@v4.0.1
+        with:
+          token: ${{ secrets.CODECOV_TOKEN }}
 
   release:
     name: Release
     runs-on: ubuntu-latest
     concurrency: push
     needs: test
     environment:
```

### Comparing `erlab-2.5.0/.gitignore` & `erlab-2.5.1/.gitignore`

 * *Files identical despite different names*

### Comparing `erlab-2.5.0/.pre-commit-config.yaml` & `erlab-2.5.1/.pre-commit-config.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -27,14 +27,14 @@
       - id: check-merge-conflict
       - id: mixed-line-ending
       - id: check-ast
 
   # Lint and format with ruff
   - repo: https://github.com/astral-sh/ruff-pre-commit
     # Ruff version.
-    rev: v0.4.3
+    rev: v0.4.4
     hooks:
       # Run the linter.
       - id: ruff
         args: [ --fix ]
       # Run the formatter.
       - id: ruff-format
```

### Comparing `erlab-2.5.0/.readthedocs.yaml` & `erlab-2.5.1/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `erlab-2.5.0/CHANGELOG.md` & `erlab-2.5.1/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,52 @@
 # CHANGELOG
 
 
 
+## v2.5.1 (2024-05-15)
+
+### Chore
+
+* exclude merge commits from semantic release ([`9179cab`](https://github.com/kmnhan/erlabpy/commit/9179cab62a299b65992ed2621d9618bf7a9f35ee))
+
+* (**deps**) add dask to optional dependencies ([`cdc90dd`](https://github.com/kmnhan/erlabpy/commit/cdc90dd785f8f7d32443e521e89b415a7575303a))
+
+* add coverage configuration ([`9c1e6a5`](https://github.com/kmnhan/erlabpy/commit/9c1e6a5365922303e0119e9f07604ba6d89b539c))
+
+### Ci
+
+* (**github**) ci changes for testing and coverage ([`67550d6`](https://github.com/kmnhan/erlabpy/commit/67550d6ebbf6423052b22bc5224ad331d824d502))
+
+  Parallelized tests for `gold.poly`, setup Qt testing, and added `.codecov.yml` config file.
+
+* (**github**) update codecov script ([`5cab279`](https://github.com/kmnhan/erlabpy/commit/5cab2796d588bc40fc74f8cd130a1efad3b76b37))
+
+* (**github**) update test script ([`7dbb384`](https://github.com/kmnhan/erlabpy/commit/7dbb384caa461992690893017cacb4bd72273149))
+
+* (**pre-commit**) pre-commit autoupdate (#34) ([`acf3dc5`](https://github.com/kmnhan/erlabpy/commit/acf3dc5f4e7987619d8a9be53ad7717f17d12fec))
+
+### Fix
+
+* (**plotting**) fixes #35 ([`a67be68`](https://github.com/kmnhan/erlabpy/commit/a67be6869c2d25780f8a56794aad0386379202dd))
+
+  Gradient fill disappears upon adding labels
+
+* (**fit.models**) wrong StepEdgeModel guess with DataArray input ([`6778c8d`](https://github.com/kmnhan/erlabpy/commit/6778c8dd2c048b0cab67c6d3668b25b3f79a71da))
+
+### Refactor
+
+* (**plotting**) code cleanup ([`aef10e4`](https://github.com/kmnhan/erlabpy/commit/aef10e472a3ebc935711253e91124cfd87beb9cc))
+
+### Test
+
+* fix tests for interactive ([`57403f7`](https://github.com/kmnhan/erlabpy/commit/57403f70f61500e248d57584962c1a0df3a2defc))
+
+* add tests for analysis.gold ([`61d4d36`](https://github.com/kmnhan/erlabpy/commit/61d4d36fb3f858ae9d096f2c8b3f9d090d8905ff))
+
+
 ## v2.5.0 (2024-05-13)
 
 ### Chore
 
 * (**deps**) unpin PyQt6 ([`55a8ce5`](https://github.com/kmnhan/erlabpy/commit/55a8ce5e0c74c38c22a44f4f385c5ee87ee5fdcb))
 
 ### Ci
@@ -37,35 +78,25 @@
 
 * (**interactive**) improve formatting for code copied to clipboard ([`d8b6d91`](https://github.com/kmnhan/erlabpy/commit/d8b6d91a4d2688486886f2464426935fdf8cabc2))
 
 ### Refactor
 
 * (**plotting**) update `clean_labels` to use `Axes.label_outer` ([`0c64756`](https://github.com/kmnhan/erlabpy/commit/0c647564c6027f5b60f9ff288f13019e0e5933b6))
 
-### Unknown
-
-* Merge pull request #33 from kmnhan/dev-2.5 ([`dc9a9a8`](https://github.com/kmnhan/erlabpy/commit/dc9a9a84a6c1e5424d6994ce02a678b6a0a30db2))
-
-  2.5 Update
-
 
 ## v2.4.2 (2024-05-07)
 
 ### Fix
 
 * (**ktool**) resolve ktool initialization problem, closes #32 ([`e88a58e`](https://github.com/kmnhan/erlabpy/commit/e88a58e6aaed326af1a68aa33322d6ea9f0e800d))
 
 * (**itool**) disable flag checking for non-numpy arrays ([`da6eb1d`](https://github.com/kmnhan/erlabpy/commit/da6eb1db9e81d51b52d4b361de938bcf7ba45e68))
 
 ### Unknown
 
-* Merge pull request #31 from kmnhan/pre-commit-ci-update-config ([`e3a4a9f`](https://github.com/kmnhan/erlabpy/commit/e3a4a9f6bda7a21d824ecfc0d70e2e1419898cbf))
-
-  [pre-commit.ci] pre-commit autoupdate
-
 * [pre-commit.ci] pre-commit autoupdate ([`ec62bea`](https://github.com/kmnhan/erlabpy/commit/ec62bea6af2b4074f77ef11a2ddf82b7b7a4db33))
 
   updates:
   - [github.com/astral-sh/ruff-pre-commit: v0.4.2 → v0.4.3](https://github.com/astral-sh/ruff-pre-commit/compare/v0.4.2...v0.4.3)
 
 
 ## v2.4.1 (2024-05-03)
@@ -127,22 +158,14 @@
 
 ### Style
 
 * remove % formatting ([`ae18a34`](https://github.com/kmnhan/erlabpy/commit/ae18a341f36542c2f39d72b0dd975dbe640c7e24))
 
 ### Unknown
 
-* Merge pull request #30 from kmnhan/pre-commit-ci-update-config ([`a550367`](https://github.com/kmnhan/erlabpy/commit/a5503679cf4c432a6c01cc4c0715c21d77136a8b))
-
-  [pre-commit.ci] pre-commit autoupdate
-
-* Merge pull request #28 from kmnhan/dev-2.4 ([`5d1f8fc`](https://github.com/kmnhan/erlabpy/commit/5d1f8fc840a7a807c35b0915ac572fa3ec2bfb49))
-
-  2.4 Release
-
 * [pre-commit.ci] pre-commit autoupdate ([`3c351cc`](https://github.com/kmnhan/erlabpy/commit/3c351cc255dc31010b2c5fab2d134531f00a4dac))
 
   updates:
   - [github.com/astral-sh/ruff-pre-commit: v0.4.1 → v0.4.2](https://github.com/astral-sh/ruff-pre-commit/compare/v0.4.1...v0.4.2)
 
 
 ## v2.3.2 (2024-04-25)
@@ -157,20 +180,14 @@
 
   Also fixes a bug where interactive summary plots were duplicated
 
 * (**io**) data loader related fixes ([`da08e90`](https://github.com/kmnhan/erlabpy/commit/da08e9076e59895b35c393c8e2556c3592adf4a5))
 
   DA30 dataloader now preserves case for attribute names from zip files. Post processing for datasets now works properly
 
-### Unknown
-
-* Merge pull request #24 from kmnhan/pre-commit-ci-update-config ([`bee9e5a`](https://github.com/kmnhan/erlabpy/commit/bee9e5acc7686f03497505cee0f4b533aa85cea2))
-
-  [pre-commit.ci] pre-commit autoupdate
-
 
 ## v2.3.1 (2024-04-25)
 
 ### Chore
 
 * (**deps**) make `iminuit` and `superqt` optional ([`1bbcc24`](https://github.com/kmnhan/erlabpy/commit/1bbcc24268312f8c285df0774e1e5d5c8c775650))
 
@@ -194,16 +211,14 @@
 
 ### Style
 
 * add mypy compatible type hints ([`c97724d`](https://github.com/kmnhan/erlabpy/commit/c97724dcd9095a3cdc1842e5afb1f29b3c472c45))
 
 ### Unknown
 
-* Merge pull request #26 from kmnhan/dev ([`85a60b3`](https://github.com/kmnhan/erlabpy/commit/85a60b37c29aca93db97004f776e8dcdd3d38666))
-
 * Merge branch &#39;main&#39; into dev ([`184afb0`](https://github.com/kmnhan/erlabpy/commit/184afb023dc704b4ab6ffe8ef5c098c19ca19084))
 
 * [pre-commit.ci] pre-commit autoupdate ([`43bfbab`](https://github.com/kmnhan/erlabpy/commit/43bfbabc93720a3afb232a75de05d43aa2567ace))
 
   updates:
   - [github.com/astral-sh/ruff-pre-commit: v0.3.7 → v0.4.1](https://github.com/astral-sh/ruff-pre-commit/compare/v0.3.7...v0.4.1)
 
@@ -302,26 +317,16 @@
 
   Calling from utilities will now raise a DeprecationWarning. The erlab.analysis namespace is unchanged, so the affect will be minimal.
 
 * qsel now raises a warning upon scalar indexing outside coordinate bounds ([`d6ed628`](https://github.com/kmnhan/erlabpy/commit/d6ed628111be8ac594d3a1b83cc2785a31e3f06e))
 
 ### Unknown
 
-* Merge pull request #23 from kmnhan/dev ([`4514a23`](https://github.com/kmnhan/erlabpy/commit/4514a234716e86c77329b48ff8615df193731514))
-
-  Added new interface for fitting, see #22 for discussions.
-  Made loader argument optional for `erlab.io.loader_context` so it can be used to just change the data directory.
-  Momentum conversion has been rewritten using `xarray.apply_ufunc`, and is now dask-compatible. It also automatically determines the current energy axis (kinetic or binding).
-
 * Merge remote-tracking branch &#39;origin/main&#39; into dev ([`fd8e1ad`](https://github.com/kmnhan/erlabpy/commit/fd8e1ad14b345664289810c4c8a605df6b299c3a))
 
-* Merge pull request #20 from kmnhan/pre-commit-ci-update-config ([`f1b965e`](https://github.com/kmnhan/erlabpy/commit/f1b965e84f79d6976ee1cabf692847fe25f58306))
-
-  [pre-commit.ci] pre-commit autoupdate
-
 * [pre-commit.ci] pre-commit autoupdate ([`7e3a89e`](https://github.com/kmnhan/erlabpy/commit/7e3a89e22bb5491f7d4a2bcb21f5a7baeead8773))
 
   updates:
   - [github.com/astral-sh/ruff-pre-commit: v0.3.5 → v0.3.7](https://github.com/astral-sh/ruff-pre-commit/compare/v0.3.5...v0.3.7)
 
 
 ## v2.2.2 (2024-04-15)
```

### Comparing `erlab-2.5.0/LICENSE` & `erlab-2.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `erlab-2.5.0/PKG-INFO` & `erlab-2.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: erlab
-Version: 2.5.0
+Version: 2.5.1
 Summary: Python package for ARPES data analysis and visualization.
 Author-email: Kimoon Han <khan@kaist.ac.kr>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -720,18 +720,20 @@
 Requires-Dist: ipywidgets; extra == "viz"
 Provides-Extra: perf
 Requires-Dist: numbagg>=0.8.1; extra == "perf"
 Requires-Dist: bottleneck>=1.3.8; extra == "perf"
 Provides-Extra: misc
 Requires-Dist: iminuit>=2.25.2; extra == "misc"
 Requires-Dist: csaps>=1.1.0; extra == "misc"
+Requires-Dist: dask>=2024.4.1; extra == "misc"
 Provides-Extra: dev
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
-Requires-Dist: pytest-xdist; extra == "dev"
+Requires-Dist: pytest-cov; extra == "dev"
+Requires-Dist: pytest-qt; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: python-semantic-release; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Provides-Extra: docs
 Requires-Dist: sphinx; extra == "docs"
 Requires-Dist: sphinx-autodoc-typehints; extra == "docs"
 Requires-Dist: sphinx-copybutton; extra == "docs"
```

### Comparing `erlab-2.5.0/PythonInterface.ipf` & `erlab-2.5.1/PythonInterface.ipf`

 * *Files identical despite different names*

### Comparing `erlab-2.5.0/README.md` & `erlab-2.5.1/README.md`

 * *Files identical despite different names*

### Comparing `erlab-2.5.0/docs/Makefile` & `erlab-2.5.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `erlab-2.5.0/docs/environment.yml` & `erlab-2.5.1/docs/environment.yml`

 * *Files identical despite different names*

### Comparing `erlab-2.5.0/docs/make.bat` & `erlab-2.5.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `erlab-2.5.0/docs/source/conf.py` & `erlab-2.5.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.0/docs/source/contributing.rst` & `erlab-2.5.1/docs/source/contributing.rst`

 * *Files identical despite different names*

### Comparing `erlab-2.5.0/docs/source/getting-started.rst` & `erlab-2.5.1/docs/source/getting-started.rst`

 * *Files identical despite different names*

### Comparing `erlab-2.5.0/docs/source/images/flowchart_multiple.pdf` & `erlab-2.5.1/docs/source/images/flowchart_multiple.pdf`

 * *Files identical despite different names*

### Comparing `erlab-2.5.0/docs/source/images/flowchart_single.pdf` & `erlab-2.5.1/docs/source/images/flowchart_single.pdf`

 * *Files identical despite different names*

### Comparing `erlab-2.5.0/docs/source/images/imagetool_dark.png` & `erlab-2.5.1/docs/source/images/imagetool_dark.png`

 * *Files identical despite different names*

### Comparing `erlab-2.5.0/docs/source/images/imagetool_light.png` & `erlab-2.5.1/docs/source/images/imagetool_light.png`

 * *Files identical despite different names*

### Comparing `erlab-2.5.0/docs/source/images/ktool_1_dark.png` & `erlab-2.5.1/docs/source/images/ktool_1_dark.png`

 * *Files identical despite different names*

### Comparing `erlab-2.5.0/docs/source/images/ktool_1_light.png` & `erlab-2.5.1/docs/source/images/ktool_1_light.png`

 * *Files identical despite different names*

### Comparing `erlab-2.5.0/docs/source/images/ktool_2_dark.png` & `erlab-2.5.1/docs/source/images/ktool_2_dark.png`

 * *Files identical despite different names*

### Comparing `erlab-2.5.0/docs/source/images/ktool_2_light.png` & `erlab-2.5.1/docs/source/images/ktool_2_light.png`

 * *Files identical despite different names*

### Comparing `erlab-2.5.0/docs/source/index.rst` & `erlab-2.5.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `erlab-2.5.0/docs/source/pyplots/norms.py` & `erlab-2.5.1/docs/source/pyplots/norms.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.0/docs/source/reference.rst` & `erlab-2.5.1/docs/source/reference.rst`

 * *Files identical despite different names*

### Comparing `erlab-2.5.0/docs/source/refs.bib` & `erlab-2.5.1/docs/source/refs.bib`

 * *Files identical despite different names*

### Comparing `erlab-2.5.0/docs/source/user-guide/curve-fitting.ipynb` & `erlab-2.5.1/docs/source/user-guide/curve-fitting.ipynb`

 * *Files identical despite different names*

### Comparing `erlab-2.5.0/docs/source/user-guide/imagetool.rst` & `erlab-2.5.1/docs/source/user-guide/imagetool.rst`

 * *Files identical despite different names*

### Comparing `erlab-2.5.0/docs/source/user-guide/index.rst` & `erlab-2.5.1/docs/source/user-guide/index.rst`

 * *Files identical despite different names*

### Comparing `erlab-2.5.0/docs/source/user-guide/indexing.ipynb` & `erlab-2.5.1/docs/source/user-guide/indexing.ipynb`

 * *Files identical despite different names*

### Comparing `erlab-2.5.0/docs/source/user-guide/io.ipynb` & `erlab-2.5.1/docs/source/user-guide/io.ipynb`

 * *Files identical despite different names*

### Comparing `erlab-2.5.0/docs/source/user-guide/kconv.ipynb` & `erlab-2.5.1/docs/source/user-guide/kconv.ipynb`

 * *Files identical despite different names*

### Comparing `erlab-2.5.0/docs/source/user-guide/plotting.ipynb` & `erlab-2.5.1/docs/source/user-guide/plotting.ipynb`

 * *Files identical despite different names*

### Comparing `erlab-2.5.0/pyproject.toml` & `erlab-2.5.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -40,19 +40,20 @@
     "xarray>=2024.02.0",
 ]
 
 [project.optional-dependencies]
 complete = ["erlab[viz,perf,misc,dev]"]
 viz = ["cmasher", "cmocean", "colorcet", "hvplot", "ipywidgets"]
 perf = ["numbagg>=0.8.1", "bottleneck>=1.3.8"]
-misc = ["iminuit>=2.25.2", "csaps>=1.1.0"]
+misc = ["iminuit>=2.25.2", "csaps>=1.1.0", "dask>=2024.4.1"]
 dev = [
     "mypy",
     "pre-commit",
-    "pytest-xdist",
+    "pytest-cov",
+    "pytest-qt",
     "pytest",
     "python-semantic-release",
     "ruff",
 ]
 docs = [
     "sphinx",
     "sphinx-autodoc-typehints",
@@ -92,15 +93,15 @@
 match = "(main|master)"
 prerelease_token = "rc"
 prerelease = false
 
 [tool.semantic_release.changelog]
 template_dir = "templates"
 changelog_file = "CHANGELOG.md"
-exclude_commit_patterns = []
+exclude_commit_patterns = ["^Merge pull request #.*"]
 
 [tool.semantic_release.commit_author]
 env = "GIT_COMMIT_AUTHOR"
 default = "semantic-release <semantic-release>"
 
 [tool.semantic_release.commit_parser_options]
 allowed_tags = [
@@ -210,14 +211,18 @@
 profile = "black"
 
 [tool.pytest.ini_options]
 addopts = ["--import-mode=importlib"]
 pythonpath = "src"
 testpaths = "tests"
 
+[tool.coverage.run]
+source = ["src"]
+omit = ["*/_deprecated/*"]
+
 [tool.mypy]
 plugins = ["numpy.typing.mypy_plugin"]
 warn_unused_configs = true
 warn_redundant_casts = true
 warn_unused_ignores = true
 allow_redefinition = true
 check_untyped_defs = false
```

### Comparing `erlab-2.5.0/src/erlab/accessors/__init__.py` & `erlab-2.5.1/src/erlab/accessors/__init__.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.0/src/erlab/accessors/fit.py` & `erlab-2.5.1/src/erlab/accessors/fit.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.0/src/erlab/accessors/kspace.py` & `erlab-2.5.1/src/erlab/accessors/kspace.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.0/src/erlab/accessors/utils.py` & `erlab-2.5.1/src/erlab/accessors/utils.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.0/src/erlab/analysis/__init__.py` & `erlab-2.5.1/src/erlab/analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.0/src/erlab/analysis/correlation.py` & `erlab-2.5.1/src/erlab/analysis/correlation.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.0/src/erlab/analysis/fit/functions/__init__.py` & `erlab-2.5.1/src/erlab/analysis/fit/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.0/src/erlab/analysis/fit/functions/dynamic.py` & `erlab-2.5.1/src/erlab/analysis/fit/functions/dynamic.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.0/src/erlab/analysis/fit/functions/general.py` & `erlab-2.5.1/src/erlab/analysis/fit/functions/general.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.0/src/erlab/analysis/fit/minuit.py` & `erlab-2.5.1/src/erlab/analysis/fit/minuit.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.0/src/erlab/analysis/fit/models.py` & `erlab-2.5.1/src/erlab/analysis/fit/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -188,15 +188,15 @@
 
         len_fit = max(round(len(x) * 0.05), 10)
         dos0, dos1, back0, back1 = fit_edges_linear(x, data, len_fit)
         efermi = x[
             np.argmin(np.gradient(scipy.ndimage.gaussian_filter1d(data, 0.2 * len(x))))
         ]
 
-        pars[f"{self.prefix}center"].set(value=efermi)
+        pars[f"{self.prefix}center"].set(value=float(efermi))
         pars[f"{self.prefix}back0"].set(value=back0)
         pars[f"{self.prefix}back1"].set(value=back1)
         pars[f"{self.prefix}dos0"].set(value=dos0)
         pars[f"{self.prefix}dos1"].set(value=dos1)
         pars[f"{self.prefix}sigma"].set(value=0.02)
 
         return lmfit.models.update_param_vals(pars, self.prefix, **kwargs)
```

### Comparing `erlab-2.5.0/src/erlab/analysis/fit/spline.py` & `erlab-2.5.1/src/erlab/analysis/fit/spline.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.0/src/erlab/analysis/gold.py` & `erlab-2.5.1/src/erlab/analysis/gold.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.0/src/erlab/analysis/image.py` & `erlab-2.5.1/src/erlab/analysis/image.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.0/src/erlab/analysis/interpolate.py` & `erlab-2.5.1/src/erlab/analysis/interpolate.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.0/src/erlab/analysis/kspace.py` & `erlab-2.5.1/src/erlab/analysis/kspace.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.0/src/erlab/analysis/mask/__init__.py` & `erlab-2.5.1/src/erlab/analysis/mask/__init__.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.0/src/erlab/analysis/mask/polygon.py` & `erlab-2.5.1/src/erlab/analysis/mask/polygon.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.0/src/erlab/analysis/transform.py` & `erlab-2.5.1/src/erlab/analysis/transform.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.0/src/erlab/analysis/utilities.py` & `erlab-2.5.1/src/erlab/analysis/utilities.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.0/src/erlab/constants.py` & `erlab-2.5.1/src/erlab/constants.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.0/src/erlab/interactive/__init__.py` & `erlab-2.5.1/src/erlab/interactive/__init__.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.0/src/erlab/interactive/bzplot.py` & `erlab-2.5.1/src/erlab/interactive/bzplot.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.0/src/erlab/interactive/colors.py` & `erlab-2.5.1/src/erlab/interactive/colors.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.0/src/erlab/interactive/curvefittingtool.py` & `erlab-2.5.1/src/erlab/interactive/curvefittingtool.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.0/src/erlab/interactive/derivative.py` & `erlab-2.5.1/src/erlab/interactive/derivative.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.0/src/erlab/interactive/dtool.ui` & `erlab-2.5.1/src/erlab/interactive/dtool.ui`

 * *Files identical despite different names*

### Comparing `erlab-2.5.0/src/erlab/interactive/fermiedge.py` & `erlab-2.5.1/src/erlab/interactive/fermiedge.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.0/src/erlab/interactive/imagetool/__init__.py` & `erlab-2.5.1/src/erlab/interactive/imagetool/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -139,14 +139,16 @@
 
     if execute:
         qapp.exec()
         del itool_list
         gc.collect()
 
         return None
+    if len(itool_list) == 1:
+        return itool_list[0]
     return itool_list
 
 
 class BaseImageTool(QtWidgets.QMainWindow):
     def __init__(self, data=None, parent=None, **kwargs):
         super().__init__(parent=parent)
         self.slicer_area = ImageSlicerArea(self, data, **kwargs)
@@ -474,101 +476,7 @@
         dialog.setNameFilters(valid_savers.keys())
         dialog.setDirectory(f"{self.slicer_area._data.name}.h5")
         # dialog.setOption(QtWidgets.QFileDialog.Option.DontUseNativeDialog)
         if dialog.exec():
             files = dialog.selectedFiles()
             fn, kargs = valid_savers[dialog.selectedNameFilter()]
             fn(self.slicer_area._data, files[0], **kargs)
-
-
-if __name__ == "__main__":
-    # import gc
-    # import linecache
-    # import tracemalloc
-
-    # def display_top(snapshot: tracemalloc.Snapshot, limit=10):
-    #     snapshot = snapshot.filter_traces(
-    #         (
-    #             tracemalloc.Filter(False, "<frozen importlib._bootstrap>"),
-    #             tracemalloc.Filter(False, "<unknown>"),
-    #         )
-    #     )
-    #     top_stats = snapshot.statistics("traceback")
-
-    #     print(f"\nTop {limit} lines")
-    #     for index, stat in enumerate(top_stats[:limit], 1):
-    #         frame = stat.traceback[0]
-    #         print(
-    #             f"#{index} {stat.traceback.total_nframe}: "
-    #             f"{frame.filename}:{frame.lineno}: {stat.size/1024:.1f} KiB"
-    #         )
-    #         line = linecache.getline(frame.filename, frame.lineno).strip()
-    #         if line:
-    #             print("    %s" % line)
-
-    #     other = top_stats[limit:]
-    #     if other:
-    #         size = sum(stat.size for stat in other)
-    #         print(f"{len(other)} other: {size/1024:.1f} KiB")
-    #     total = sum(stat.size for stat in top_stats)
-    #     print(f"Total allocated size: {total/1024:.1f} KiB")
-
-    # while True:
-    #     try:
-    #         idx = int(input("Index: "))
-    #         stat = top_stats[idx - 1]
-    #     except (IndexError, ValueError):
-    #         break
-    #     print("%s memory blocks: %.1f KiB" % (stat.count, stat.size / 1024))
-    #     for line in stat.traceback.format():
-    #         print(line)
-
-    # tracemalloc.start()
-    data = xr.load_dataarray(
-        #     # "~/Documents/ERLab/TiSe2/kxy10.nc",
-        #     # "~/Documents/ERLab/TiSe2/221213_SSRL_BL5-2/fullmap_kconv_.h5",
-        "~/Documents/ERLab/CsV3Sb5/2021_Dec_ALS_CV3Sb5/Data/cvs_kxy_small.nc",
-        # "~/Documents/ERLab/CsV3Sb5/2021_Dec_ALS_CV3Sb5/Data/cvs_kxy.nc",
-        # "~/Documents/ERLab/TiSe2/220410_ALS_BL4/map_mm_4d_.nc",
-        # engine="h5netcdf",
-    )
-
-    # win = itool(data, bench=True)
-    # win = itool(data)
-    # del data
-
-    # gc.collect()
-    # data = xr.load_dataarray(
-    #     "~/Documents/ERLab/CsV3Sb5/2021_Dec_ALS_CV3Sb5/Data/cvs_kxy.nc",
-    #     engine="h5netcdf",
-    # )
-
-    # from erlab.io.exampledata import generate_data
-
-    # data = generate_data()
-
-    # win = itool([data, data], link=True, link_colors=False)
-    # win = itool(data.sel(eV=0, method='nearest'))
-    win = itool(data)
-
-    # snapshot = tracemalloc.take_snapshot()
-    # print(
-    #     *[
-    #         f"{n} {m * 2**-20:.2f} MB\t"
-    #         for n, m in zip(("Current", "Max"), tracemalloc.get_traced_memory())
-    #     ],
-    #     sep="",
-    # )
-    # tracemalloc.stop()
-    # display_top(snapshot)
-    # print(win.array_slicer._nanmeancalls)
-
-    # qapp: QtWidgets.QApplication = QtWidgets.QApplication.instance()
-    # if not qapp:
-    #     qapp = QtWidgets.QApplication(sys.argv)
-    # qapp.setStyle("Fusion")
-    # import numpy as np
-    # win = ImageTool(np.ones((2,2)))
-    # win.show()
-    # win.raise_()
-    # win.activateWindow()
-    # qapp.exec()
```

### Comparing `erlab-2.5.0/src/erlab/interactive/imagetool/_deprecated/imagetool_mpl.py` & `erlab-2.5.1/src/erlab/interactive/imagetool/_deprecated/imagetool_mpl.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.0/src/erlab/interactive/imagetool/_deprecated/imagetool_old.py` & `erlab-2.5.1/src/erlab/interactive/imagetool/_deprecated/imagetool_old.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.0/src/erlab/interactive/imagetool/controls.py` & `erlab-2.5.1/src/erlab/interactive/imagetool/controls.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.0/src/erlab/interactive/imagetool/core.py` & `erlab-2.5.1/src/erlab/interactive/imagetool/core.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.0/src/erlab/interactive/imagetool/fastbinning.py` & `erlab-2.5.1/src/erlab/interactive/imagetool/fastbinning.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.0/src/erlab/interactive/imagetool/slicer.py` & `erlab-2.5.1/src/erlab/interactive/imagetool/slicer.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.0/src/erlab/interactive/kspace.py` & `erlab-2.5.1/src/erlab/interactive/kspace.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.0/src/erlab/interactive/ktool.ui` & `erlab-2.5.1/src/erlab/interactive/ktool.ui`

 * *Files identical despite different names*

### Comparing `erlab-2.5.0/src/erlab/interactive/masktool.py` & `erlab-2.5.1/src/erlab/interactive/masktool.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.0/src/erlab/interactive/utilities.py` & `erlab-2.5.1/src/erlab/interactive/utilities.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.0/src/erlab/io/__init__.py` & `erlab-2.5.1/src/erlab/io/__init__.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.0/src/erlab/io/characterization/resistance.py` & `erlab-2.5.1/src/erlab/io/characterization/resistance.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.0/src/erlab/io/characterization/xrd.py` & `erlab-2.5.1/src/erlab/io/characterization/xrd.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.0/src/erlab/io/dataloader.py` & `erlab-2.5.1/src/erlab/io/dataloader.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.0/src/erlab/io/exampledata.py` & `erlab-2.5.1/src/erlab/io/exampledata.py`

 * *Files 3% similar despite different names*

```diff
@@ -307,14 +307,16 @@
     angres: float = 0.1,
     edge_coeffs: Sequence[float] = (0.04, 1e-5, -3e-4),
     background_coeffs: Sequence[float] = (1.0, 0.0, -2e-3),
     count: int = 1000000,
     noise: bool = True,
     seed: int | None = None,
     ccd_sigma: float = 0.6,
+    nx: int = 200,
+    ny: int = 300,
 ) -> xr.DataArray:
     """
     Generate a curved Fermi edge with a linear density of states.
 
     Parameters
     ----------
     a
@@ -340,23 +342,27 @@
     noise
         Flag indicating whether to add noise to the spectrum. Default is True.
     seed
         Seed for the random number generator for the noise. Default is None.
     ccd_sigma
         Standard deviation of the Gaussian filter applied to the spectrum. Default is
         0.6.
+    nx
+        Number of angle points. Default is 200.
+    ny
+        Number of energy points. Default is 300.
 
     Returns
     -------
     data : xarray.DataArray
         Simulated gold edge spectrum.
 
     """
-    alpha = np.linspace(-15, 15, 200)
-    eV = np.linspace(-1.3, 0.3, 300)
+    alpha = np.linspace(-15, 15, nx)
+    eV = np.linspace(-1.3, 0.3, ny)
 
     alpha = xr.DataArray(alpha, dims="alpha", coords={"alpha": alpha})
     eV = xr.DataArray(eV, dims="eV", coords={"eV": eV})
 
     center = np.polynomial.polynomial.polyval(alpha, edge_coeffs)
 
     data = (b - c + a * eV) / (
```

### Comparing `erlab-2.5.0/src/erlab/io/igor.py` & `erlab-2.5.1/src/erlab/io/igor.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.0/src/erlab/io/plugins/__init__.py` & `erlab-2.5.1/src/erlab/io/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.0/src/erlab/io/plugins/da30.py` & `erlab-2.5.1/src/erlab/io/plugins/da30.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.0/src/erlab/io/plugins/kriss.py` & `erlab-2.5.1/src/erlab/io/plugins/kriss.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.0/src/erlab/io/plugins/merlin.py` & `erlab-2.5.1/src/erlab/io/plugins/merlin.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.0/src/erlab/io/plugins/ssrl52.py` & `erlab-2.5.1/src/erlab/io/plugins/ssrl52.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.0/src/erlab/io/utilities.py` & `erlab-2.5.1/src/erlab/io/utilities.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.0/src/erlab/lattice.py` & `erlab-2.5.1/src/erlab/lattice.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.0/src/erlab/parallel.py` & `erlab-2.5.1/src/erlab/parallel.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.0/src/erlab/plotting/IgorCT/Blue-White.txt` & `erlab-2.5.1/src/erlab/plotting/IgorCT/Blue-White.txt`

 * *Files identical despite different names*

### Comparing `erlab-2.5.0/src/erlab/plotting/IgorCT/BlueHot.ibw` & `erlab-2.5.1/src/erlab/plotting/IgorCT/BlueHot.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.5.0/src/erlab/plotting/IgorCT/CTBlueWhite.ibw` & `erlab-2.5.1/src/erlab/plotting/IgorCT/CTBlueWhite.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.5.0/src/erlab/plotting/IgorCT/CTRainbowLIght.ibw` & `erlab-2.5.1/src/erlab/plotting/IgorCT/CTRainbowLIght.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.5.0/src/erlab/plotting/IgorCT/CTRedTemperature.ibw` & `erlab-2.5.1/src/erlab/plotting/IgorCT/CTRedTemperature.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.5.0/src/erlab/plotting/IgorCT/ColdWarm.ibw` & `erlab-2.5.1/src/erlab/plotting/IgorCT/ColdWarm.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.5.0/src/erlab/plotting/IgorCT/PlanetEarth.ibw` & `erlab-2.5.1/src/erlab/plotting/IgorCT/PlanetEarth.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.5.0/src/erlab/plotting/IgorCT/ametrine.ibw` & `erlab-2.5.1/src/erlab/plotting/IgorCT/ametrine.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.5.0/src/erlab/plotting/IgorCT/isolum.ibw` & `erlab-2.5.1/src/erlab/plotting/IgorCT/isolum.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.5.0/src/erlab/plotting/IgorCT/morgenstemning.ibw` & `erlab-2.5.1/src/erlab/plotting/IgorCT/morgenstemning.ibw`

 * *Files identical despite different names*

### Comparing `erlab-2.5.0/src/erlab/plotting/__init__.py` & `erlab-2.5.1/src/erlab/plotting/__init__.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.0/src/erlab/plotting/annotations.py` & `erlab-2.5.1/src/erlab/plotting/annotations.py`

 * *Files 2% similar despite different names*

```diff
@@ -495,39 +495,39 @@
     else:
         value_arr = np.array(values).flatten(order=order)
         if not (axlist.size == value_arr.size):
             raise IndexError(
                 "The number of given values must match the number of given axes."
             )
 
-    for i in range(len(axlist)):
-        bbox_to_anchor = axlist[i].bbox
+    for i, ax in enumerate(axlist):
         if fontsize is None:
-            if isinstance(axlist[i], matplotlib.figure.Figure):
+            if isinstance(ax, matplotlib.figure.Figure):
                 fontsize = "large"
             else:
                 fontsize = "medium"
 
-        bbox_transform = matplotlib.transforms.ScaledTranslation(
-            offset[0] / 72, offset[1] / 72, axlist[i].get_figure().dpi_scale_trans
-        )
         label_str = _alph_label(value_arr[i], prefix, suffix, numeric, capital)
-        with plt.rc_context({"text.color": axes_textcolor(axlist[i])}):
+        with plt.rc_context({"text.color": axes_textcolor(ax)}):
             at = matplotlib.offsetbox.AnchoredText(
                 label_str,
                 loc=loc,
                 frameon=False,
                 pad=0,
                 borderpad=0.5,
                 prop=dict(fontsize=fontsize, **kwargs),
-                bbox_to_anchor=bbox_to_anchor,
-                bbox_transform=bbox_transform,
+                bbox_to_anchor=ax.bbox,
+                bbox_transform=matplotlib.transforms.ScaledTranslation(
+                    offset[0] / 72,
+                    offset[1] / 72,
+                    ax.get_figure().dpi_scale_trans,
+                ),
                 clip_on=False,
             )
-        axlist[i].add_artist(at)
+        ax.add_artist(at)
 
 
 def label_subplots_nature(
     axes: matplotlib.axes.Axes | Sequence[matplotlib.axes.Axes],
     values: Sequence[int | str] | None = None,
     startfrom: int = 1,
     order: Literal["C", "F", "A", "K"] = "C",
```

### Comparing `erlab-2.5.0/src/erlab/plotting/atoms.py` & `erlab-2.5.1/src/erlab/plotting/atoms.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.0/src/erlab/plotting/bz.py` & `erlab-2.5.1/src/erlab/plotting/bz.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.0/src/erlab/plotting/colors.py` & `erlab-2.5.1/src/erlab/plotting/colors.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.0/src/erlab/plotting/erplot.py` & `erlab-2.5.1/src/erlab/plotting/erplot.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.0/src/erlab/plotting/general.py` & `erlab-2.5.1/src/erlab/plotting/general.py`

 * *Files 1% similar despite different names*

```diff
@@ -695,22 +695,25 @@
     )
     ax.add_patch(patch)
 
     im = matplotlib.image.AxesImage(
         ax, cmap=cmap, interpolation="bicubic", origin="lower", zorder=0, **kwargs
     )
     im.use_sticky_edges = False  # type: ignore[attr-defined]
-    ax.add_artist(im)
+
     if transpose:
         im.set_data(np.linspace(0, 1, 1024).reshape(1024, 1).T)
     else:
         im.set_data(np.linspace(0, 1, 1024).reshape(1024, 1))
+
     # with autoscale_off(ax):
     im.set_extent((min(xn), max(xn), min(yn), max(yn)))
     im.set_clip_path(patch)
+    im.autoscale_None()
+    ax.add_image(im)
 
     return im
 
 
 def plot_slices(
     maps: xr.DataArray | Sequence[xr.DataArray],
     figsize: tuple[float, float] | None = None,
```

### Comparing `erlab-2.5.0/src/erlab/plotting/plot3d.py` & `erlab-2.5.1/src/erlab/plotting/plot3d.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.0/src/erlab/plotting/stylelib/fira.mplstyle` & `erlab-2.5.1/src/erlab/plotting/stylelib/fira.mplstyle`

 * *Files identical despite different names*

### Comparing `erlab-2.5.0/src/erlab/plotting/stylelib/firalight.mplstyle` & `erlab-2.5.1/src/erlab/plotting/stylelib/firalight.mplstyle`

 * *Files identical despite different names*

### Comparing `erlab-2.5.0/src/erlab/plotting/stylelib/khan.mplstyle` & `erlab-2.5.1/src/erlab/plotting/stylelib/khan.mplstyle`

 * *Files identical despite different names*

### Comparing `erlab-2.5.0/src/erlab/plotting/stylelib/nature.mplstyle` & `erlab-2.5.1/src/erlab/plotting/stylelib/nature.mplstyle`

 * *Files identical despite different names*

### Comparing `erlab-2.5.0/src/erlab/plotting/stylelib/poster.mplstyle` & `erlab-2.5.1/src/erlab/plotting/stylelib/poster.mplstyle`

 * *Files identical despite different names*

### Comparing `erlab-2.5.0/src/erlab/plotting/stylelib/times.mplstyle` & `erlab-2.5.1/src/erlab/plotting/stylelib/times.mplstyle`

 * *Files identical despite different names*

### Comparing `erlab-2.5.0/src/erlab.egg-info/PKG-INFO` & `erlab-2.5.1/src/erlab.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: erlab
-Version: 2.5.0
+Version: 2.5.1
 Summary: Python package for ARPES data analysis and visualization.
 Author-email: Kimoon Han <khan@kaist.ac.kr>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -720,18 +720,20 @@
 Requires-Dist: ipywidgets; extra == "viz"
 Provides-Extra: perf
 Requires-Dist: numbagg>=0.8.1; extra == "perf"
 Requires-Dist: bottleneck>=1.3.8; extra == "perf"
 Provides-Extra: misc
 Requires-Dist: iminuit>=2.25.2; extra == "misc"
 Requires-Dist: csaps>=1.1.0; extra == "misc"
+Requires-Dist: dask>=2024.4.1; extra == "misc"
 Provides-Extra: dev
 Requires-Dist: mypy; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
-Requires-Dist: pytest-xdist; extra == "dev"
+Requires-Dist: pytest-cov; extra == "dev"
+Requires-Dist: pytest-qt; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: python-semantic-release; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Provides-Extra: docs
 Requires-Dist: sphinx; extra == "docs"
 Requires-Dist: sphinx-autodoc-typehints; extra == "docs"
 Requires-Dist: sphinx-copybutton; extra == "docs"
```

### Comparing `erlab-2.5.0/src/erlab.egg-info/SOURCES.txt` & `erlab-2.5.1/src/erlab.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+.codecov.yml
 .gitignore
 .pre-commit-config.yaml
 .readthedocs.yaml
 CHANGELOG.md
 LICENSE
 PythonInterface.ipf
 README.md
@@ -134,19 +135,24 @@
 src/erlab/plotting/stylelib/khan.mplstyle
 src/erlab/plotting/stylelib/nature.mplstyle
 src/erlab/plotting/stylelib/poster.mplstyle
 src/erlab/plotting/stylelib/times.mplstyle
 templates/.macros.j2
 templates/.release_notes.md.j2
 templates/CHANGELOG.md.j2
+tests/test_constants.py
 tests/accessors/test_fit.py
 tests/accessors/test_kspace.py
 tests/analysis/test_fastbinning.py
-tests/analysis/test_fit_functions_dynamic.py
-tests/analysis/test_fit_functions_general.py
-tests/analysis/test_fit_models.py
+tests/analysis/test_gold.py
 tests/analysis/test_image.py
 tests/analysis/test_image_savgol.py
 tests/analysis/test_interpolate.py
 tests/analysis/test_kspace.py
 tests/analysis/test_utilities.py
-tests/io/test_dataloader.py
+tests/analysis/fit/test_functions_dynamic.py
+tests/analysis/fit/test_functions_general.py
+tests/analysis/fit/test_minuit.py
+tests/analysis/fit/test_models.py
+tests/interactive/test_imagetool.py
+tests/io/test_dataloader.py
+tests/plotting/test_general.py
```

### Comparing `erlab-2.5.0/src/erlab.egg-info/requires.txt` & `erlab-2.5.1/src/erlab.egg-info/requires.txt`

 * *Files 14% similar despite different names*

```diff
@@ -17,15 +17,16 @@
 
 [complete]
 erlab[dev,misc,perf,viz]
 
 [dev]
 mypy
 pre-commit
-pytest-xdist
+pytest-cov
+pytest-qt
 pytest
 python-semantic-release
 ruff
 
 [docs]
 sphinx
 sphinx-autodoc-typehints
@@ -36,14 +37,15 @@
 nbsphinx
 furo
 sphinx-design
 
 [misc]
 iminuit>=2.25.2
 csaps>=1.1.0
+dask>=2024.4.1
 
 [perf]
 numbagg>=0.8.1
 bottleneck>=1.3.8
 
 [viz]
 cmasher
```

### Comparing `erlab-2.5.0/templates/.macros.j2` & `erlab-2.5.1/templates/.macros.j2`

 * *Files identical despite different names*

### Comparing `erlab-2.5.0/tests/accessors/test_fit.py` & `erlab-2.5.1/tests/accessors/test_fit.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.0/tests/accessors/test_kspace.py` & `erlab-2.5.1/tests/accessors/test_kspace.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.0/tests/analysis/test_fastbinning.py` & `erlab-2.5.1/tests/analysis/test_fastbinning.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.0/tests/analysis/test_fit_functions_dynamic.py` & `erlab-2.5.1/tests/analysis/fit/test_functions_dynamic.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.0/tests/analysis/test_fit_functions_general.py` & `erlab-2.5.1/tests/analysis/fit/test_functions_general.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.0/tests/analysis/test_fit_models.py` & `erlab-2.5.1/tests/analysis/fit/test_models.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.0/tests/analysis/test_image.py` & `erlab-2.5.1/tests/analysis/test_image.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.0/tests/analysis/test_image_savgol.py` & `erlab-2.5.1/tests/analysis/test_image_savgol.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.0/tests/analysis/test_interpolate.py` & `erlab-2.5.1/tests/analysis/test_interpolate.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.0/tests/analysis/test_kspace.py` & `erlab-2.5.1/tests/analysis/test_kspace.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.0/tests/analysis/test_utilities.py` & `erlab-2.5.1/tests/analysis/test_utilities.py`

 * *Files identical despite different names*

### Comparing `erlab-2.5.0/tests/io/test_dataloader.py` & `erlab-2.5.1/tests/io/test_dataloader.py`

 * *Files identical despite different names*

