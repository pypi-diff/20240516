# Comparing `tmp/ebilab-2.6.0.tar.gz` & `tmp/ebilab-2.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ebilab-2.6.0.tar", last modified: Tue May 14 10:08:17 2024, max compression
+gzip compressed data, was "ebilab-2.7.0.tar", last modified: Thu May 16 05:39:49 2024, max compression
```

## Comparing `ebilab-2.6.0.tar` & `ebilab-2.7.0.tar`

### file list

```diff
@@ -1,117 +1,118 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:08:17.729264 ebilab-2.6.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:08:17.709264 ebilab-2.6.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:08:17.713264 ebilab-2.6.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-14 10:08:08.000000 ebilab-2.6.0/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-14 10:08:08.000000 ebilab-2.6.0/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3322 2024-05-14 10:08:08.000000 ebilab-2.6.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-14 10:08:08.000000 ebilab-2.6.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-14 10:08:08.000000 ebilab-2.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-14 10:08:08.000000 ebilab-2.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-14 10:08:08.000000 ebilab-2.6.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-14 10:08:17.729264 ebilab-2.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-05-14 10:08:08.000000 ebilab-2.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:08:17.713264 ebilab-2.6.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-05-14 10:08:08.000000 ebilab-2.6.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-14 10:08:08.000000 ebilab-2.6.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-14 10:08:08.000000 ebilab-2.6.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:08:17.717264 ebilab-2.6.0/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:08:17.717264 ebilab-2.6.0/docs/source/api/
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-14 10:08:08.000000 ebilab-2.6.0/docs/source/api/ebilab.analysis.rst
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-14 10:08:08.000000 ebilab-2.6.0/docs/source/api/ebilab.experiment.devices.rst
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-14 10:08:08.000000 ebilab-2.6.0/docs/source/api/ebilab.experiment.devices.visa.rst
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-14 10:08:08.000000 ebilab-2.6.0/docs/source/api/ebilab.experiment.rst
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-14 10:08:08.000000 ebilab-2.6.0/docs/source/api/ebilab.project.rst
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-14 10:08:08.000000 ebilab-2.6.0/docs/source/api/ebilab.rst
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-14 10:08:08.000000 ebilab-2.6.0/docs/source/api/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4400 2024-05-14 10:08:08.000000 ebilab-2.6.0/docs/source/changelog-v2.0.0-pre.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5476 2024-05-14 10:08:08.000000 ebilab-2.6.0/docs/source/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-05-14 10:08:08.000000 ebilab-2.6.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      853 2024-05-14 10:08:08.000000 ebilab-2.6.0/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-14 10:08:08.000000 ebilab-2.6.0/docs/source/installation.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:08:17.709264 ebilab-2.6.0/docs/source/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:08:17.709264 ebilab-2.6.0/docs/source/locale/en/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:08:17.717264 ebilab-2.6.0/docs/source/locale/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    12691 2024-05-14 10:08:08.000000 ebilab-2.6.0/docs/source/locale/en/LC_MESSAGES/api.po
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-05-14 10:08:08.000000 ebilab-2.6.0/docs/source/locale/en/LC_MESSAGES/changelog.po
--rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-05-14 10:08:08.000000 ebilab-2.6.0/docs/source/locale/en/LC_MESSAGES/index.po
--rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-05-14 10:08:08.000000 ebilab-2.6.0/docs/source/locale/en/LC_MESSAGES/installation.po
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-14 10:08:08.000000 ebilab-2.6.0/docs/source/locale/en/LC_MESSAGES/modules.po
--rw-r--r--   0 runner    (1001) docker     (127)    14754 2024-05-14 10:08:08.000000 ebilab-2.6.0/docs/source/locale/en/LC_MESSAGES/tutorial.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:08:17.721264 ebilab-2.6.0/docs/source/tutorial/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-14 10:08:08.000000 ebilab-2.6.0/docs/source/tutorial/analysis.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5886 2024-05-14 10:08:08.000000 ebilab-2.6.0/docs/source/tutorial/experiment.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-14 10:08:08.000000 ebilab-2.6.0/docs/source/tutorial/experiment_device.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3004 2024-05-14 10:08:08.000000 ebilab-2.6.0/docs/source/tutorial/version.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:08:17.721264 ebilab-2.6.0/ebilab/
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-14 10:08:08.000000 ebilab-2.6.0/ebilab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-14 10:08:08.000000 ebilab-2.6.0/ebilab/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5457 2024-05-14 10:08:08.000000 ebilab-2.6.0/ebilab/_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:08:17.721264 ebilab-2.6.0/ebilab/analysis/
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-14 10:08:08.000000 ebilab-2.6.0/ebilab/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-14 10:08:08.000000 ebilab-2.6.0/ebilab/analysis/_actions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-05-14 10:08:08.000000 ebilab-2.6.0/ebilab/analysis/_preprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)     4967 2024-05-14 10:08:08.000000 ebilab-2.6.0/ebilab/analysis/_process.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:08:17.709264 ebilab-2.6.0/ebilab/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:08:17.721264 ebilab-2.6.0/ebilab/data/project-template/
--rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-05-14 10:08:08.000000 ebilab-2.6.0/ebilab/data/project-template/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:08:17.713264 ebilab-2.6.0/ebilab/data/project-template/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:08:17.721264 ebilab-2.6.0/ebilab/data/project-template/data/input/
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-14 10:08:08.000000 ebilab-2.6.0/ebilab/data/project-template/data/input/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:08:17.721264 ebilab-2.6.0/ebilab/data/project-template/data/original/
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-14 10:08:08.000000 ebilab-2.6.0/ebilab/data/project-template/data/original/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:08:17.721264 ebilab-2.6.0/ebilab/data/project-template/data/output/
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-14 10:08:08.000000 ebilab-2.6.0/ebilab/data/project-template/data/output/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:08:17.725264 ebilab-2.6.0/ebilab/data/project-template/data/plot/
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-14 10:08:08.000000 ebilab-2.6.0/ebilab/data/project-template/data/plot/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 10:08:08.000000 ebilab-2.6.0/ebilab/data/project-template/ebilab.ini
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 10:08:08.000000 ebilab-2.6.0/ebilab/data/project-template/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:08:17.725264 ebilab-2.6.0/ebilab/experiment/
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-14 10:08:08.000000 ebilab-2.6.0/ebilab/experiment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10644 2024-05-14 10:08:08.000000 ebilab-2.6.0/ebilab/experiment/_experiment_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)    22272 2024-05-14 10:08:08.000000 ebilab-2.6.0/ebilab/experiment/_ui_tkinter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:08:17.725264 ebilab-2.6.0/ebilab/experiment/devices/
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-14 10:08:08.000000 ebilab-2.6.0/ebilab/experiment/devices/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:08:17.725264 ebilab-2.6.0/ebilab/experiment/devices/_visa/
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-05-14 10:08:08.000000 ebilab-2.6.0/ebilab/experiment/devices/_visa/A707.py
--rw-r--r--   0 runner    (1001) docker     (127)     2521 2024-05-14 10:08:08.000000 ebilab-2.6.0/ebilab/experiment/devices/_visa/E4980.py
--rw-r--r--   0 runner    (1001) docker     (127)     4002 2024-05-14 10:08:08.000000 ebilab-2.6.0/ebilab/experiment/devices/_visa/K34411A.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 10:08:08.000000 ebilab-2.6.0/ebilab/experiment/devices/_visa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4406 2024-05-14 10:08:08.000000 ebilab-2.6.0/ebilab/experiment/devices/visa.py
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-05-14 10:08:08.000000 ebilab-2.6.0/ebilab/experiment/options.py
--rw-r--r--   0 runner    (1001) docker     (127)    20598 2024-05-14 10:08:08.000000 ebilab-2.6.0/ebilab/icon.ico
--rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-05-14 10:08:08.000000 ebilab-2.6.0/ebilab/project.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:08:17.729264 ebilab-2.6.0/ebilab.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-14 10:08:17.000000 ebilab-2.6.0/ebilab.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-05-14 10:08:17.000000 ebilab-2.6.0/ebilab.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 10:08:17.000000 ebilab-2.6.0/ebilab.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-14 10:08:17.000000 ebilab-2.6.0/ebilab.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-14 10:08:17.000000 ebilab-2.6.0/ebilab.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-14 10:08:17.000000 ebilab-2.6.0/ebilab.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-14 10:08:08.000000 ebilab-2.6.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:08:17.725264 ebilab-2.6.0/sample/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-14 10:08:08.000000 ebilab-2.6.0/sample/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-14 10:08:08.000000 ebilab-2.6.0/sample/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-14 10:08:08.000000 ebilab-2.6.0/sample/cont_r.py
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-14 10:08:08.000000 ebilab-2.6.0/sample/multimeter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2916 2024-05-14 10:08:08.000000 ebilab-2.6.0/sample/random-walk.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:08:17.725264 ebilab-2.6.0/sample/recipes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 10:08:08.000000 ebilab-2.6.0/sample/recipes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-14 10:08:08.000000 ebilab-2.6.0/sample/recipes/do-nothing.py
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-14 10:08:08.000000 ebilab-2.6.0/sample/recipes/raise-error.py
--rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-05-14 10:08:08.000000 ebilab-2.6.0/sample/recipes/random-walk.py
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-14 10:08:08.000000 ebilab-2.6.0/sample/voltage.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 10:08:17.729264 ebilab-2.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-05-14 10:08:08.000000 ebilab-2.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:08:17.725264 ebilab-2.6.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:08:17.729264 ebilab-2.6.0/tests/sample/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:08:17.713264 ebilab-2.6.0/tests/sample/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:08:17.729264 ebilab-2.6.0/tests/sample/data/input/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 10:08:08.000000 ebilab-2.6.0/tests/sample/data/input/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:08:17.729264 ebilab-2.6.0/tests/sample/data/original/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 10:08:08.000000 ebilab-2.6.0/tests/sample/data/original/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:08:17.729264 ebilab-2.6.0/tests/sample/data/output/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 10:08:08.000000 ebilab-2.6.0/tests/sample/data/output/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 10:08:08.000000 ebilab-2.6.0/tests/sample/ebilab.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 10:08:17.729264 ebilab-2.6.0/tests/sample/other_dir/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 10:08:08.000000 ebilab-2.6.0/tests/sample/other_dir/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-14 10:08:08.000000 ebilab-2.6.0/tests/test_paths.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 05:39:49.250562 ebilab-2.7.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 05:39:49.234561 ebilab-2.7.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 05:39:49.238561 ebilab-2.7.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-16 05:39:37.000000 ebilab-2.7.0/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-16 05:39:37.000000 ebilab-2.7.0/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3322 2024-05-16 05:39:37.000000 ebilab-2.7.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-16 05:39:37.000000 ebilab-2.7.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-16 05:39:37.000000 ebilab-2.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-16 05:39:37.000000 ebilab-2.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-16 05:39:37.000000 ebilab-2.7.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-16 05:39:49.250562 ebilab-2.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-05-16 05:39:37.000000 ebilab-2.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 05:39:49.238561 ebilab-2.7.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-05-16 05:39:37.000000 ebilab-2.7.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-16 05:39:37.000000 ebilab-2.7.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-16 05:39:37.000000 ebilab-2.7.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 05:39:49.242561 ebilab-2.7.0/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 05:39:49.242561 ebilab-2.7.0/docs/source/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-16 05:39:37.000000 ebilab-2.7.0/docs/source/api/ebilab.analysis.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-16 05:39:37.000000 ebilab-2.7.0/docs/source/api/ebilab.experiment.devices.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-16 05:39:37.000000 ebilab-2.7.0/docs/source/api/ebilab.experiment.devices.visa.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-16 05:39:37.000000 ebilab-2.7.0/docs/source/api/ebilab.experiment.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-16 05:39:37.000000 ebilab-2.7.0/docs/source/api/ebilab.project.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-16 05:39:37.000000 ebilab-2.7.0/docs/source/api/ebilab.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-16 05:39:37.000000 ebilab-2.7.0/docs/source/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4400 2024-05-16 05:39:37.000000 ebilab-2.7.0/docs/source/changelog-v2.0.0-pre.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7001 2024-05-16 05:39:37.000000 ebilab-2.7.0/docs/source/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-05-16 05:39:37.000000 ebilab-2.7.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-05-16 05:39:37.000000 ebilab-2.7.0/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-16 05:39:37.000000 ebilab-2.7.0/docs/source/installation.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 05:39:49.234561 ebilab-2.7.0/docs/source/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 05:39:49.234561 ebilab-2.7.0/docs/source/locale/en/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 05:39:49.242561 ebilab-2.7.0/docs/source/locale/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    12691 2024-05-16 05:39:37.000000 ebilab-2.7.0/docs/source/locale/en/LC_MESSAGES/api.po
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-05-16 05:39:37.000000 ebilab-2.7.0/docs/source/locale/en/LC_MESSAGES/changelog.po
+-rw-r--r--   0 runner    (1001) docker     (127)     1885 2024-05-16 05:39:37.000000 ebilab-2.7.0/docs/source/locale/en/LC_MESSAGES/index.po
+-rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-05-16 05:39:37.000000 ebilab-2.7.0/docs/source/locale/en/LC_MESSAGES/installation.po
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-16 05:39:37.000000 ebilab-2.7.0/docs/source/locale/en/LC_MESSAGES/modules.po
+-rw-r--r--   0 runner    (1001) docker     (127)    14754 2024-05-16 05:39:37.000000 ebilab-2.7.0/docs/source/locale/en/LC_MESSAGES/tutorial.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 05:39:49.242561 ebilab-2.7.0/docs/source/tutorial/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-16 05:39:37.000000 ebilab-2.7.0/docs/source/tutorial/analysis.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5886 2024-05-16 05:39:37.000000 ebilab-2.7.0/docs/source/tutorial/experiment.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-16 05:39:37.000000 ebilab-2.7.0/docs/source/tutorial/experiment_device.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3818 2024-05-16 05:39:37.000000 ebilab-2.7.0/docs/source/tutorial/version.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 05:39:49.242561 ebilab-2.7.0/ebilab/
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-16 05:39:37.000000 ebilab-2.7.0/ebilab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-16 05:39:37.000000 ebilab-2.7.0/ebilab/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5457 2024-05-16 05:39:37.000000 ebilab-2.7.0/ebilab/_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 05:39:49.246562 ebilab-2.7.0/ebilab/analysis/
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-16 05:39:37.000000 ebilab-2.7.0/ebilab/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-16 05:39:37.000000 ebilab-2.7.0/ebilab/analysis/_actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-05-16 05:39:37.000000 ebilab-2.7.0/ebilab/analysis/_preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4967 2024-05-16 05:39:37.000000 ebilab-2.7.0/ebilab/analysis/_process.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 05:39:49.234561 ebilab-2.7.0/ebilab/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 05:39:49.246562 ebilab-2.7.0/ebilab/data/project-template/
+-rw-r--r--   0 runner    (1001) docker     (127)     3095 2024-05-16 05:39:37.000000 ebilab-2.7.0/ebilab/data/project-template/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 05:39:49.234561 ebilab-2.7.0/ebilab/data/project-template/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 05:39:49.246562 ebilab-2.7.0/ebilab/data/project-template/data/input/
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-16 05:39:37.000000 ebilab-2.7.0/ebilab/data/project-template/data/input/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 05:39:49.246562 ebilab-2.7.0/ebilab/data/project-template/data/original/
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-16 05:39:37.000000 ebilab-2.7.0/ebilab/data/project-template/data/original/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 05:39:49.246562 ebilab-2.7.0/ebilab/data/project-template/data/output/
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-16 05:39:37.000000 ebilab-2.7.0/ebilab/data/project-template/data/output/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 05:39:49.246562 ebilab-2.7.0/ebilab/data/project-template/data/plot/
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-16 05:39:37.000000 ebilab-2.7.0/ebilab/data/project-template/data/plot/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 05:39:37.000000 ebilab-2.7.0/ebilab/data/project-template/ebilab.ini
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 05:39:37.000000 ebilab-2.7.0/ebilab/data/project-template/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 05:39:49.246562 ebilab-2.7.0/ebilab/experiment/
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-16 05:39:37.000000 ebilab-2.7.0/ebilab/experiment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11027 2024-05-16 05:39:37.000000 ebilab-2.7.0/ebilab/experiment/_experiment_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22272 2024-05-16 05:39:37.000000 ebilab-2.7.0/ebilab/experiment/_ui_tkinter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 05:39:49.246562 ebilab-2.7.0/ebilab/experiment/devices/
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-16 05:39:37.000000 ebilab-2.7.0/ebilab/experiment/devices/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 05:39:49.250562 ebilab-2.7.0/ebilab/experiment/devices/_visa/
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-05-16 05:39:37.000000 ebilab-2.7.0/ebilab/experiment/devices/_visa/A707.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2521 2024-05-16 05:39:37.000000 ebilab-2.7.0/ebilab/experiment/devices/_visa/E4980.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4002 2024-05-16 05:39:37.000000 ebilab-2.7.0/ebilab/experiment/devices/_visa/K34411A.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 05:39:37.000000 ebilab-2.7.0/ebilab/experiment/devices/_visa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4406 2024-05-16 05:39:37.000000 ebilab-2.7.0/ebilab/experiment/devices/visa.py
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-05-16 05:39:37.000000 ebilab-2.7.0/ebilab/experiment/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20598 2024-05-16 05:39:37.000000 ebilab-2.7.0/ebilab/icon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     2268 2024-05-16 05:39:37.000000 ebilab-2.7.0/ebilab/project.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 05:39:49.250562 ebilab-2.7.0/ebilab.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-16 05:39:49.000000 ebilab-2.7.0/ebilab.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-05-16 05:39:49.000000 ebilab-2.7.0/ebilab.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 05:39:49.000000 ebilab-2.7.0/ebilab.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-16 05:39:49.000000 ebilab-2.7.0/ebilab.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-16 05:39:49.000000 ebilab-2.7.0/ebilab.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-16 05:39:49.000000 ebilab-2.7.0/ebilab.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-16 05:39:37.000000 ebilab-2.7.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 05:39:49.250562 ebilab-2.7.0/sample/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-16 05:39:37.000000 ebilab-2.7.0/sample/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-16 05:39:37.000000 ebilab-2.7.0/sample/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-16 05:39:37.000000 ebilab-2.7.0/sample/cont_r.py
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-05-16 05:39:37.000000 ebilab-2.7.0/sample/multimeter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2916 2024-05-16 05:39:37.000000 ebilab-2.7.0/sample/random-walk.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 05:39:49.250562 ebilab-2.7.0/sample/recipes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 05:39:37.000000 ebilab-2.7.0/sample/recipes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-16 05:39:37.000000 ebilab-2.7.0/sample/recipes/ctx-sleep.py
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-16 05:39:37.000000 ebilab-2.7.0/sample/recipes/do-nothing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-16 05:39:37.000000 ebilab-2.7.0/sample/recipes/raise-error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-05-16 05:39:37.000000 ebilab-2.7.0/sample/recipes/random-walk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-16 05:39:37.000000 ebilab-2.7.0/sample/voltage.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 05:39:49.250562 ebilab-2.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-05-16 05:39:37.000000 ebilab-2.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 05:39:49.250562 ebilab-2.7.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 05:39:49.250562 ebilab-2.7.0/tests/sample/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 05:39:49.238561 ebilab-2.7.0/tests/sample/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 05:39:49.250562 ebilab-2.7.0/tests/sample/data/input/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 05:39:37.000000 ebilab-2.7.0/tests/sample/data/input/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 05:39:49.250562 ebilab-2.7.0/tests/sample/data/original/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 05:39:37.000000 ebilab-2.7.0/tests/sample/data/original/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 05:39:49.250562 ebilab-2.7.0/tests/sample/data/output/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 05:39:37.000000 ebilab-2.7.0/tests/sample/data/output/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 05:39:37.000000 ebilab-2.7.0/tests/sample/ebilab.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 05:39:49.250562 ebilab-2.7.0/tests/sample/other_dir/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 05:39:37.000000 ebilab-2.7.0/tests/sample/other_dir/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-16 05:39:37.000000 ebilab-2.7.0/tests/test_paths.py
```

### Comparing `ebilab-2.6.0/.gitignore` & `ebilab-2.7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `ebilab-2.6.0/LICENSE` & `ebilab-2.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ebilab-2.6.0/PKG-INFO` & `ebilab-2.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ebilab
-Version: 2.6.0
+Version: 2.7.0
 Summary: Python package for my research
 Home-page: https://ebilab.readthedocs.io/
 Author: Yusuke Ebihara
 Author-email: yusuke@ebihara.me
 Project-URL: GitHub repository, https://github.com/ebiyuu1121/ebilab
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ebilab-2.6.0/README.md` & `ebilab-2.7.0/README.md`

 * *Files identical despite different names*

### Comparing `ebilab-2.6.0/docs/Makefile` & `ebilab-2.7.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ebilab-2.6.0/docs/make.bat` & `ebilab-2.7.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ebilab-2.6.0/docs/source/api/ebilab.analysis.rst` & `ebilab-2.7.0/docs/source/api/ebilab.analysis.rst`

 * *Files identical despite different names*

### Comparing `ebilab-2.6.0/docs/source/changelog-v2.0.0-pre.rst` & `ebilab-2.7.0/docs/source/changelog-v2.0.0-pre.rst`

 * *Files identical despite different names*

### Comparing `ebilab-2.6.0/docs/source/changelog.md` & `ebilab-2.7.0/docs/source/changelog.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,28 @@
 更新履歴
 ========
 
+v2.7.0 (May 16, 2024)
+---------------------
+
+### Features
+
+- `ebilab.experiment` にて、 `ctx.sleep` 関数を追加しました。
+    - 実験定義の中で `time.sleep` 関数を用いると、STOPボタンを押してもsleep中は実験が停止できません。そこで、代わりに `ctx.sleep` 関数を用いると、sleep中にSTOPボタンを押しても停止することができます。
+
+## Other
+
+- バージョン更新ポリシーを変更し、semantic versioningにより準拠するようになりました。
+    - 今後、より広報互換性を重視するようになります。
+    - 新しいポリシーは以下の通りです。
+        - a (Major version): 重要で破壊的な変更があった場合に更新されます。
+        - b (Minor version): 新機能の追加や一部機能の仕様な変更など、軽微な変更があった場合に更新されます。
+        - c (Patch version): 新メソッドの追加などの軽微な機能や、バグ修正など機能に変更がない場合に更新されます。ドキュメントに未完成(unstable)と明記されている機能に関しては、パッチバージョンで更新が行なわれることがあります。
+    - minor versionやpatch versionに関しては後方互換性がありますが、バグに依存していた場合や内部機能をハックしていた場合にはその限りではありません。厳密な再現性のためにはバージョンの固定を行ってください。
+
 v2.6.0 (May 14, 2024)
 ---------------------
 
 ### Features
 
 - `ebilab.experiment` にて、実験時にPython例外が発生しても適切に処理するようにしました。
```

### Comparing `ebilab-2.6.0/docs/source/conf.py` & `ebilab-2.7.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `ebilab-2.6.0/docs/source/index.rst` & `ebilab-2.7.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `ebilab-2.6.0/docs/source/installation.rst` & `ebilab-2.7.0/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `ebilab-2.6.0/docs/source/locale/en/LC_MESSAGES/api.po` & `ebilab-2.7.0/docs/source/locale/en/LC_MESSAGES/api.po`

 * *Files identical despite different names*

### Comparing `ebilab-2.6.0/docs/source/locale/en/LC_MESSAGES/changelog.po` & `ebilab-2.7.0/docs/source/locale/en/LC_MESSAGES/changelog.po`

 * *Files identical despite different names*

### Comparing `ebilab-2.6.0/docs/source/locale/en/LC_MESSAGES/index.po` & `ebilab-2.7.0/docs/source/locale/en/LC_MESSAGES/index.po`

 * *Files identical despite different names*

### Comparing `ebilab-2.6.0/docs/source/locale/en/LC_MESSAGES/installation.po` & `ebilab-2.7.0/docs/source/locale/en/LC_MESSAGES/installation.po`

 * *Files identical despite different names*

### Comparing `ebilab-2.6.0/docs/source/locale/en/LC_MESSAGES/modules.po` & `ebilab-2.7.0/docs/source/locale/en/LC_MESSAGES/modules.po`

 * *Files identical despite different names*

### Comparing `ebilab-2.6.0/docs/source/locale/en/LC_MESSAGES/tutorial.po` & `ebilab-2.7.0/docs/source/locale/en/LC_MESSAGES/tutorial.po`

 * *Files identical despite different names*

### Comparing `ebilab-2.6.0/docs/source/tutorial/analysis.rst` & `ebilab-2.7.0/docs/source/tutorial/analysis.rst`

 * *Files identical despite different names*

### Comparing `ebilab-2.6.0/docs/source/tutorial/experiment.rst` & `ebilab-2.7.0/docs/source/tutorial/experiment.rst`

 * *Files identical despite different names*

### Comparing `ebilab-2.6.0/docs/source/tutorial/experiment_device.rst` & `ebilab-2.7.0/docs/source/tutorial/experiment_device.rst`

 * *Files identical despite different names*

### Comparing `ebilab-2.6.0/docs/source/tutorial/version.rst` & `ebilab-2.7.0/docs/source/tutorial/version.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,24 +1,34 @@
 ####################
 バージョンについて
 ####################
 
 このライブラリは随時アップデートしています。
-バージョンは :code:`a.b.c` の形式で定義され、以下のポリシーで更新されます。
+バージョンは :code:`a.b.c` の形式で定義され、v2.7.0以降は以下のポリシーで更新されます。
+
+* a (Major version): メソッドの仕様変更や機能の削除など、破壊的な変更があった場合に更新されます。
+* b (Minor version): 新機能の追加や非公開APIの変更の際に更新されます。
+* c (Patch version): バグ修正や非公開APIの変更など、機能に変更がない修正の際に更新されます。
+
+なお、ドキュメントに未完成(unstable)と明記されている機能に関しては、パッチバージョンで更新が行なわれることがあります。
+
+v2.6.0以前は以下のポリシーで更新されました。
 
 * a (Major version): 重要で破壊的な変更があった場合に更新されます。
 * b (Minor version): 新機能の追加や一部機能の仕様な変更など、軽微な変更があった場合に更新されます。
 * c (Patch version): 新メソッドの追加などの軽微な機能や、バグ修正など機能に変更がない場合に更新されます。ドキュメントに未完成(unstable)と明記されている機能に関しては、パッチバージョンで更新が行なわれることがあります。
 
 ****************************************
 実験の再現性のために
 ****************************************
 
 :code:`ebilab` のバージョンを更新した場合、過去の実験コードの動作が変化し、実験を再現できなくなる可能性があります。それを防止するには、何らかの方法でバージョンを固定することを推奨します。
 
+minor versionやpatch versionに関しては後方互換性がありますが、バグに依存していた場合や内部機能をハックしていた場合にはその限りではありません。
+
 代表的なものとしては :code:`venv` や :code:`pipenv` などが挙げられます。
 
 .. 一方で、そのようなツールの使用に慣れていない場合や、たった1ファイルのスクリプトなど仮想環境を導入するのが煩雑だと感じる場合もあるでしょう。
 .. その場合では、 :py:func:`assert_ebilab_version() <ebilab.assert_ebilab_version>` 関数を用いて簡易的にバージョンのチェックを行なうことができます。
 
 .. 例えば、以下のようなコードを実験コードの最上部に記述してください。
```

### Comparing `ebilab-2.6.0/ebilab/__init__.py` & `ebilab-2.7.0/ebilab/__init__.py`

 * *Files identical despite different names*

### Comparing `ebilab-2.6.0/ebilab/_cli.py` & `ebilab-2.7.0/ebilab/_cli.py`

 * *Files identical despite different names*

### Comparing `ebilab-2.6.0/ebilab/analysis/_actions.py` & `ebilab-2.7.0/ebilab/analysis/_actions.py`

 * *Files identical despite different names*

### Comparing `ebilab-2.6.0/ebilab/analysis/_preprocess.py` & `ebilab-2.7.0/ebilab/analysis/_preprocess.py`

 * *Files identical despite different names*

### Comparing `ebilab-2.6.0/ebilab/analysis/_process.py` & `ebilab-2.7.0/ebilab/analysis/_process.py`

 * *Files identical despite different names*

### Comparing `ebilab-2.6.0/ebilab/data/project-template/.gitignore` & `ebilab-2.7.0/ebilab/data/project-template/.gitignore`

 * *Files identical despite different names*

### Comparing `ebilab-2.6.0/ebilab/experiment/_experiment_controller.py` & `ebilab-2.7.0/ebilab/experiment/_experiment_controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,30 @@
 
     @property
     def options(self) -> dict:
         return self._delegate.experiment_ctx_delegate_get_options()
 
     def loop(self) -> None:
         self._delegate.experiment_ctx_delegate_loop()
-        
+
+    def sleep(self, sleep_time: float) -> None:
+        """
+        Cancelable sleep
+        You should use ctx.sleep instead of time.sleep
+
+        Args:
+            sleep_time (float): Time to sleep
+        """
+        target = time.time() + sleep_time
+        while target - time.time() > 1.0:
+            time.sleep(1)
+            self.loop()
+
+        time.sleep(target - time.time())
+ 
 @dataclasses.dataclass
 class PlotterContext:
     plotter_options: dict
     protocol_options: dict
 
 class ExperimentPlotter(metaclass=abc.ABCMeta):
     fig: plt.Figure
```

### Comparing `ebilab-2.6.0/ebilab/experiment/_ui_tkinter.py` & `ebilab-2.7.0/ebilab/experiment/_ui_tkinter.py`

 * *Files identical despite different names*

### Comparing `ebilab-2.6.0/ebilab/experiment/devices/_visa/A707.py` & `ebilab-2.7.0/ebilab/experiment/devices/_visa/A707.py`

 * *Files identical despite different names*

### Comparing `ebilab-2.6.0/ebilab/experiment/devices/_visa/E4980.py` & `ebilab-2.7.0/ebilab/experiment/devices/_visa/E4980.py`

 * *Files identical despite different names*

### Comparing `ebilab-2.6.0/ebilab/experiment/devices/_visa/K34411A.py` & `ebilab-2.7.0/ebilab/experiment/devices/_visa/K34411A.py`

 * *Files identical despite different names*

### Comparing `ebilab-2.6.0/ebilab/experiment/devices/visa.py` & `ebilab-2.7.0/ebilab/experiment/devices/visa.py`

 * *Files identical despite different names*

### Comparing `ebilab-2.6.0/ebilab/experiment/options.py` & `ebilab-2.7.0/ebilab/experiment/options.py`

 * *Files identical despite different names*

### Comparing `ebilab-2.6.0/ebilab/icon.ico` & `ebilab-2.7.0/ebilab/icon.ico`

 * *Files identical despite different names*

### Comparing `ebilab-2.6.0/ebilab/project.py` & `ebilab-2.7.0/ebilab/project.py`

 * *Files identical despite different names*

### Comparing `ebilab-2.6.0/ebilab.egg-info/PKG-INFO` & `ebilab-2.7.0/ebilab.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ebilab
-Version: 2.6.0
+Version: 2.7.0
 Summary: Python package for my research
 Home-page: https://ebilab.readthedocs.io/
 Author: Yusuke Ebihara
 Author-email: yusuke@ebihara.me
 Project-URL: GitHub repository, https://github.com/ebiyuu1121/ebilab
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ebilab-2.6.0/ebilab.egg-info/SOURCES.txt` & `ebilab-2.7.0/ebilab.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -68,14 +68,15 @@
 sample/.gitignore
 sample/README.md
 sample/cont_r.py
 sample/multimeter.py
 sample/random-walk.py
 sample/voltage.py
 sample/recipes/__init__.py
+sample/recipes/ctx-sleep.py
 sample/recipes/do-nothing.py
 sample/recipes/raise-error.py
 sample/recipes/random-walk.py
 tests/test_paths.py
 tests/sample/ebilab.ini
 tests/sample/data/input/.gitkeep
 tests/sample/data/original/.gitkeep
```

### Comparing `ebilab-2.6.0/sample/cont_r.py` & `ebilab-2.7.0/sample/cont_r.py`

 * *Files identical despite different names*

### Comparing `ebilab-2.6.0/sample/random-walk.py` & `ebilab-2.7.0/sample/random-walk.py`

 * *Files identical despite different names*

### Comparing `ebilab-2.6.0/sample/recipes/random-walk.py` & `ebilab-2.7.0/sample/recipes/random-walk.py`

 * *Files identical despite different names*

### Comparing `ebilab-2.6.0/sample/voltage.py` & `ebilab-2.7.0/sample/voltage.py`

 * *Files identical despite different names*

### Comparing `ebilab-2.6.0/setup.py` & `ebilab-2.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `ebilab-2.6.0/tests/test_paths.py` & `ebilab-2.7.0/tests/test_paths.py`

 * *Files identical despite different names*

