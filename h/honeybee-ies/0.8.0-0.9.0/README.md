# Comparing `tmp/honeybee-ies-0.8.0.tar.gz` & `tmp/honeybee-ies-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/honeybee-ies-0.8.0.tar", last modified: Sat Nov 25 03:33:34 2023, max compression
+gzip compressed data, was "dist/honeybee-ies-0.9.0.tar", last modified: Mon Dec  4 16:42:09 2023, max compression
```

## Comparing `honeybee-ies-0.8.0.tar` & `honeybee-ies-0.9.0.tar`

### file list

```diff
@@ -1,68 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-25 03:33:34.000000 honeybee-ies-0.8.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-25 03:33:34.000000 honeybee-ies-0.8.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-25 03:33:34.000000 honeybee-ies-0.8.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2817 2023-11-25 03:32:38.000000 honeybee-ies-0.8.0/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2023-11-25 03:32:38.000000 honeybee-ies-0.8.0/.github/workflows/dependency-release.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      167 2023-11-25 03:32:38.000000 honeybee-ies-0.8.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      294 2023-11-25 03:32:38.000000 honeybee-ies-0.8.0/.releaserc.json
--rw-r--r--   0 runner    (1001) docker     (127)      279 2023-11-25 03:32:38.000000 honeybee-ies-0.8.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)      445 2023-11-25 03:32:38.000000 honeybee-ies-0.8.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2023-11-25 03:32:38.000000 honeybee-ies-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2233 2023-11-25 03:33:34.000000 honeybee-ies-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1674 2023-11-25 03:32:38.000000 honeybee-ies-0.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      165 2023-11-25 03:32:38.000000 honeybee-ies-0.8.0/deploy.sh
--rw-r--r--   0 runner    (1001) docker     (127)      262 2023-11-25 03:32:38.000000 honeybee-ies-0.8.0/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-25 03:33:34.000000 honeybee-ies-0.8.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      360 2023-11-25 03:32:38.000000 honeybee-ies-0.8.0/docs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-25 03:33:34.000000 honeybee-ies-0.8.0/docs/_build/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-25 03:32:38.000000 honeybee-ies-0.8.0/docs/_build/.nojekyll
--rw-r--r--   0 runner    (1001) docker     (127)       16 2023-11-25 03:32:38.000000 honeybee-ies-0.8.0/docs/_build/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-25 03:33:34.000000 honeybee-ies-0.8.0/docs/_build/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       16 2023-11-25 03:32:38.000000 honeybee-ies-0.8.0/docs/_build/docs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-25 03:33:34.000000 honeybee-ies-0.8.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     1037 2023-11-25 03:32:38.000000 honeybee-ies-0.8.0/docs/_static/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-25 03:33:34.000000 honeybee-ies-0.8.0/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)     3668 2023-11-25 03:32:38.000000 honeybee-ies-0.8.0/docs/_templates/layout.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-25 03:33:34.000000 honeybee-ies-0.8.0/docs/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2023-11-25 03:32:38.000000 honeybee-ies-0.8.0/docs/cli/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)    21471 2023-11-25 03:32:38.000000 honeybee-ies-0.8.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      387 2023-11-25 03:32:38.000000 honeybee-ies-0.8.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       78 2023-11-25 03:32:38.000000 honeybee-ies-0.8.0/docs/modules.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-25 03:33:34.000000 honeybee-ies-0.8.0/honeybee_ies/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2023-11-25 03:32:38.000000 honeybee-ies-0.8.0/honeybee_ies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       72 2023-11-25 03:32:38.000000 honeybee-ies-0.8.0/honeybee_ies/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      191 2023-11-25 03:32:38.000000 honeybee-ies-0.8.0/honeybee_ies/_extend_honeybee.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-25 03:33:34.000000 honeybee-ies-0.8.0/honeybee_ies/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      389 2023-11-25 03:32:38.000000 honeybee-ies-0.8.0/honeybee_ies/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2765 2023-11-25 03:32:38.000000 honeybee-ies-0.8.0/honeybee_ies/cli/translate.py
--rw-r--r--   0 runner    (1001) docker     (127)    12131 2023-11-25 03:32:38.000000 honeybee-ies-0.8.0/honeybee_ies/reader.py
--rw-r--r--   0 runner    (1001) docker     (127)      994 2023-11-25 03:32:38.000000 honeybee-ies-0.8.0/honeybee_ies/templates.py
--rw-r--r--   0 runner    (1001) docker     (127)    12238 2023-11-25 03:32:38.000000 honeybee-ies-0.8.0/honeybee_ies/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-25 03:33:34.000000 honeybee-ies-0.8.0/honeybee_ies.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2233 2023-11-25 03:33:34.000000 honeybee-ies-0.8.0/honeybee_ies.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2023-11-25 03:33:34.000000 honeybee-ies-0.8.0/honeybee_ies.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-25 03:33:34.000000 honeybee-ies-0.8.0/honeybee_ies.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2023-11-25 03:33:34.000000 honeybee-ies-0.8.0/honeybee_ies.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2023-11-25 03:33:34.000000 honeybee-ies-0.8.0/honeybee_ies.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2023-11-25 03:33:34.000000 honeybee-ies-0.8.0/honeybee_ies.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2023-11-25 03:32:38.000000 honeybee-ies-0.8.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      102 2023-11-25 03:33:34.000000 honeybee-ies-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2023-11-25 03:32:38.000000 honeybee-ies-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-25 03:33:34.000000 honeybee-ies-0.8.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-25 03:33:34.000000 honeybee-ies-0.8.0/tests/assets/
--rw-r--r--   0 runner    (1001) docker     (127)  2630219 2023-11-25 03:32:38.000000 honeybee-ies-0.8.0/tests/assets/lab_building.hbjson
--rw-r--r--   0 runner    (1001) docker     (127)    55839 2023-11-25 03:32:38.000000 honeybee-ies-0.8.0/tests/assets/model_with_holes.hbjson
--rw-r--r--   0 runner    (1001) docker     (127)   134559 2023-11-25 03:32:38.000000 honeybee-ies-0.8.0/tests/assets/multiline_name_test.hbjson
--rw-r--r--   0 runner    (1001) docker     (127)   274009 2023-11-25 03:32:38.000000 honeybee-ies-0.8.0/tests/assets/revit_sample_model.hbjson
--rw-r--r--   0 runner    (1001) docker     (127)     1171 2023-11-25 03:32:38.000000 honeybee-ies-0.8.0/tests/assets/room_underground.gem
--rw-r--r--   0 runner    (1001) docker     (127)    47646 2023-11-25 03:32:38.000000 honeybee-ies-0.8.0/tests/assets/room_with_air_boundary.hbjson
--rw-r--r--   0 runner    (1001) docker     (127)    46729 2023-11-25 03:32:38.000000 honeybee-ies-0.8.0/tests/assets/sample_model_45.hbjson
--rw-r--r--   0 runner    (1001) docker     (127)    42885 2023-11-25 03:32:38.000000 honeybee-ies-0.8.0/tests/assets/shade_with_holes.hbjson
--rw-r--r--   0 runner    (1001) docker     (127)    46189 2023-11-25 03:32:38.000000 honeybee-ies-0.8.0/tests/assets/single_face_shade.hbjson
--rw-r--r--   0 runner    (1001) docker     (127)    49097 2023-11-25 03:32:38.000000 honeybee-ies-0.8.0/tests/assets/topographical_shade.gem
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-25 03:33:34.000000 honeybee-ies-0.8.0/tests/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-25 03:32:38.000000 honeybee-ies-0.8.0/tests/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      547 2023-11-25 03:32:38.000000 honeybee-ies-0.8.0/tests/cli/translate_cli_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      361 2023-11-25 03:32:38.000000 honeybee-ies-0.8.0/tests/extend_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      400 2023-11-25 03:32:38.000000 honeybee-ies-0.8.0/tests/reader_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3601 2023-11-25 03:32:38.000000 honeybee-ies-0.8.0/tests/writer_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 16:42:09.000000 honeybee-ies-0.9.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 16:42:09.000000 honeybee-ies-0.9.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 16:42:09.000000 honeybee-ies-0.9.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2817 2023-12-04 16:41:10.000000 honeybee-ies-0.9.0/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2023-12-04 16:41:10.000000 honeybee-ies-0.9.0/.github/workflows/dependency-release.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2023-12-04 16:41:10.000000 honeybee-ies-0.9.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2023-12-04 16:41:10.000000 honeybee-ies-0.9.0/.releaserc.json
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2023-12-04 16:41:10.000000 honeybee-ies-0.9.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2023-12-04 16:41:10.000000 honeybee-ies-0.9.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2023-12-04 16:41:10.000000 honeybee-ies-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2233 2023-12-04 16:42:09.000000 honeybee-ies-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1674 2023-12-04 16:41:10.000000 honeybee-ies-0.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2023-12-04 16:41:10.000000 honeybee-ies-0.9.0/deploy.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2023-12-04 16:41:10.000000 honeybee-ies-0.9.0/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 16:42:09.000000 honeybee-ies-0.9.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2023-12-04 16:41:10.000000 honeybee-ies-0.9.0/docs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 16:42:09.000000 honeybee-ies-0.9.0/docs/_build/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-04 16:41:10.000000 honeybee-ies-0.9.0/docs/_build/.nojekyll
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2023-12-04 16:41:10.000000 honeybee-ies-0.9.0/docs/_build/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 16:42:09.000000 honeybee-ies-0.9.0/docs/_build/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2023-12-04 16:41:10.000000 honeybee-ies-0.9.0/docs/_build/docs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 16:42:09.000000 honeybee-ies-0.9.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     1037 2023-12-04 16:41:10.000000 honeybee-ies-0.9.0/docs/_static/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 16:42:09.000000 honeybee-ies-0.9.0/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     3668 2023-12-04 16:41:10.000000 honeybee-ies-0.9.0/docs/_templates/layout.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 16:42:09.000000 honeybee-ies-0.9.0/docs/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2023-12-04 16:41:10.000000 honeybee-ies-0.9.0/docs/cli/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    21471 2023-12-04 16:41:10.000000 honeybee-ies-0.9.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2023-12-04 16:41:10.000000 honeybee-ies-0.9.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2023-12-04 16:41:10.000000 honeybee-ies-0.9.0/docs/modules.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 16:42:09.000000 honeybee-ies-0.9.0/honeybee_ies/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2023-12-04 16:41:10.000000 honeybee-ies-0.9.0/honeybee_ies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2023-12-04 16:41:10.000000 honeybee-ies-0.9.0/honeybee_ies/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2023-12-04 16:41:10.000000 honeybee-ies-0.9.0/honeybee_ies/_extend_honeybee.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 16:42:09.000000 honeybee-ies-0.9.0/honeybee_ies/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2023-12-04 16:41:10.000000 honeybee-ies-0.9.0/honeybee_ies/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2765 2023-12-04 16:41:10.000000 honeybee-ies-0.9.0/honeybee_ies/cli/translate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20391 2023-12-04 16:41:10.000000 honeybee-ies-0.9.0/honeybee_ies/reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2023-12-04 16:41:10.000000 honeybee-ies-0.9.0/honeybee_ies/templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12238 2023-12-04 16:41:10.000000 honeybee-ies-0.9.0/honeybee_ies/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 16:42:09.000000 honeybee-ies-0.9.0/honeybee_ies.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2233 2023-12-04 16:42:09.000000 honeybee-ies-0.9.0/honeybee_ies.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2023-12-04 16:42:09.000000 honeybee-ies-0.9.0/honeybee_ies.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-04 16:42:09.000000 honeybee-ies-0.9.0/honeybee_ies.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2023-12-04 16:42:09.000000 honeybee-ies-0.9.0/honeybee_ies.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2023-12-04 16:42:09.000000 honeybee-ies-0.9.0/honeybee_ies.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2023-12-04 16:42:09.000000 honeybee-ies-0.9.0/honeybee_ies.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2023-12-04 16:41:10.000000 honeybee-ies-0.9.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2023-12-04 16:42:09.000000 honeybee-ies-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2023-12-04 16:41:10.000000 honeybee-ies-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 16:42:09.000000 honeybee-ies-0.9.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 16:42:09.000000 honeybee-ies-0.9.0/tests/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)  2630219 2023-12-04 16:41:10.000000 honeybee-ies-0.9.0/tests/assets/lab_building.hbjson
+-rw-r--r--   0 runner    (1001) docker     (127)    55839 2023-12-04 16:41:10.000000 honeybee-ies-0.9.0/tests/assets/model_with_holes.hbjson
+-rw-r--r--   0 runner    (1001) docker     (127)   134559 2023-12-04 16:41:10.000000 honeybee-ies-0.9.0/tests/assets/multiline_name_test.hbjson
+-rw-r--r--   0 runner    (1001) docker     (127)     4039 2023-12-04 16:41:10.000000 honeybee-ies-0.9.0/tests/assets/pv.gem
+-rw-r--r--   0 runner    (1001) docker     (127)   274009 2023-12-04 16:41:10.000000 honeybee-ies-0.9.0/tests/assets/revit_sample_model.hbjson
+-rw-r--r--   0 runner    (1001) docker     (127)     1171 2023-12-04 16:41:10.000000 honeybee-ies-0.9.0/tests/assets/room_underground.gem
+-rw-r--r--   0 runner    (1001) docker     (127)    47646 2023-12-04 16:41:10.000000 honeybee-ies-0.9.0/tests/assets/room_with_air_boundary.hbjson
+-rw-r--r--   0 runner    (1001) docker     (127)    46729 2023-12-04 16:41:10.000000 honeybee-ies-0.9.0/tests/assets/sample_model_45.hbjson
+-rw-r--r--   0 runner    (1001) docker     (127)    42885 2023-12-04 16:41:10.000000 honeybee-ies-0.9.0/tests/assets/shade_with_holes.hbjson
+-rw-r--r--   0 runner    (1001) docker     (127)    46189 2023-12-04 16:41:10.000000 honeybee-ies-0.9.0/tests/assets/single_face_shade.hbjson
+-rw-r--r--   0 runner    (1001) docker     (127)    49097 2023-12-04 16:41:10.000000 honeybee-ies-0.9.0/tests/assets/topographical_shade.gem
+-rw-r--r--   0 runner    (1001) docker     (127)     4312 2023-12-04 16:41:10.000000 honeybee-ies-0.9.0/tests/assets/translucent_shade.gem
+-rw-r--r--   0 runner    (1001) docker     (127)     4715 2023-12-04 16:41:10.000000 honeybee-ies-0.9.0/tests/assets/tree.gem
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 16:42:09.000000 honeybee-ies-0.9.0/tests/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-04 16:41:10.000000 honeybee-ies-0.9.0/tests/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2023-12-04 16:41:10.000000 honeybee-ies-0.9.0/tests/cli/translate_cli_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2023-12-04 16:41:10.000000 honeybee-ies-0.9.0/tests/extend_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2023-12-04 16:41:10.000000 honeybee-ies-0.9.0/tests/reader_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3601 2023-12-04 16:41:10.000000 honeybee-ies-0.9.0/tests/writer_test.py
```

### Comparing `honeybee-ies-0.8.0/.github/workflows/ci.yaml` & `honeybee-ies-0.9.0/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `honeybee-ies-0.8.0/.github/workflows/dependency-release.yaml` & `honeybee-ies-0.9.0/.github/workflows/dependency-release.yaml`

 * *Files identical despite different names*

### Comparing `honeybee-ies-0.8.0/LICENSE` & `honeybee-ies-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `honeybee-ies-0.8.0/PKG-INFO` & `honeybee-ies-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: honeybee-ies
-Version: 0.8.0
+Version: 0.9.0
 Summary: Honeybee extension for import and export to/from IES-VE
 Home-page: https://github.com/ladybug-tools/honeybee-ies
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 License: AGPL-3.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: Implementation :: CPython
```

### Comparing `honeybee-ies-0.8.0/README.md` & `honeybee-ies-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `honeybee-ies-0.8.0/docs/_static/custom.css` & `honeybee-ies-0.9.0/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `honeybee-ies-0.8.0/docs/_templates/layout.html` & `honeybee-ies-0.9.0/docs/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `honeybee-ies-0.8.0/docs/conf.py` & `honeybee-ies-0.9.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `honeybee-ies-0.8.0/honeybee_ies/cli/translate.py` & `honeybee-ies-0.9.0/honeybee_ies/cli/translate.py`

 * *Files identical despite different names*

### Comparing `honeybee-ies-0.8.0/honeybee_ies/templates.py` & `honeybee-ies-0.9.0/honeybee_ies/templates.py`

 * *Files identical despite different names*

### Comparing `honeybee-ies-0.8.0/honeybee_ies/writer.py` & `honeybee-ies-0.9.0/honeybee_ies/writer.py`

 * *Files identical despite different names*

### Comparing `honeybee-ies-0.8.0/honeybee_ies.egg-info/PKG-INFO` & `honeybee-ies-0.9.0/honeybee_ies.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: honeybee-ies
-Version: 0.8.0
+Version: 0.9.0
 Summary: Honeybee extension for import and export to/from IES-VE
 Home-page: https://github.com/ladybug-tools/honeybee-ies
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 License: AGPL-3.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: Implementation :: CPython
```

### Comparing `honeybee-ies-0.8.0/honeybee_ies.egg-info/SOURCES.txt` & `honeybee-ies-0.9.0/honeybee_ies.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -37,16 +37,19 @@
 honeybee_ies/cli/translate.py
 tests/extend_test.py
 tests/reader_test.py
 tests/writer_test.py
 tests/assets/lab_building.hbjson
 tests/assets/model_with_holes.hbjson
 tests/assets/multiline_name_test.hbjson
+tests/assets/pv.gem
 tests/assets/revit_sample_model.hbjson
 tests/assets/room_underground.gem
 tests/assets/room_with_air_boundary.hbjson
 tests/assets/sample_model_45.hbjson
 tests/assets/shade_with_holes.hbjson
 tests/assets/single_face_shade.hbjson
 tests/assets/topographical_shade.gem
+tests/assets/translucent_shade.gem
+tests/assets/tree.gem
 tests/cli/__init__.py
 tests/cli/translate_cli_test.py
```

### Comparing `honeybee-ies-0.8.0/setup.py` & `honeybee-ies-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `honeybee-ies-0.8.0/tests/assets/lab_building.hbjson` & `honeybee-ies-0.9.0/tests/assets/lab_building.hbjson`

 * *Files identical despite different names*

### Comparing `honeybee-ies-0.8.0/tests/assets/model_with_holes.hbjson` & `honeybee-ies-0.9.0/tests/assets/model_with_holes.hbjson`

 * *Files identical despite different names*

### Comparing `honeybee-ies-0.8.0/tests/assets/multiline_name_test.hbjson` & `honeybee-ies-0.9.0/tests/assets/multiline_name_test.hbjson`

 * *Files identical despite different names*

### Comparing `honeybee-ies-0.8.0/tests/assets/revit_sample_model.hbjson` & `honeybee-ies-0.9.0/tests/assets/revit_sample_model.hbjson`

 * *Files identical despite different names*

### Comparing `honeybee-ies-0.8.0/tests/assets/room_underground.gem` & `honeybee-ies-0.9.0/tests/assets/room_underground.gem`

 * *Files identical despite different names*

### Comparing `honeybee-ies-0.8.0/tests/assets/room_with_air_boundary.hbjson` & `honeybee-ies-0.9.0/tests/assets/room_with_air_boundary.hbjson`

 * *Files identical despite different names*

### Comparing `honeybee-ies-0.8.0/tests/assets/sample_model_45.hbjson` & `honeybee-ies-0.9.0/tests/assets/sample_model_45.hbjson`

 * *Files identical despite different names*

### Comparing `honeybee-ies-0.8.0/tests/assets/shade_with_holes.hbjson` & `honeybee-ies-0.9.0/tests/assets/shade_with_holes.hbjson`

 * *Files identical despite different names*

### Comparing `honeybee-ies-0.8.0/tests/assets/single_face_shade.hbjson` & `honeybee-ies-0.9.0/tests/assets/single_face_shade.hbjson`

 * *Files identical despite different names*

### Comparing `honeybee-ies-0.8.0/tests/assets/topographical_shade.gem` & `honeybee-ies-0.9.0/tests/assets/topographical_shade.gem`

 * *Files identical despite different names*

### Comparing `honeybee-ies-0.8.0/tests/cli/translate_cli_test.py` & `honeybee-ies-0.9.0/tests/cli/translate_cli_test.py`

 * *Files identical despite different names*

### Comparing `honeybee-ies-0.8.0/tests/writer_test.py` & `honeybee-ies-0.9.0/tests/writer_test.py`

 * *Files identical despite different names*

