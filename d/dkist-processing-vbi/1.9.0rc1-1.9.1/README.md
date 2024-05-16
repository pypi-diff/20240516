# Comparing `tmp/dkist_processing_vbi-1.9.0rc1.tar.gz` & `tmp/dkist_processing_vbi-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dkist_processing_vbi-1.9.0rc1.tar", last modified: Wed May  8 02:03:52 2024, max compression
+gzip compressed data, was "dkist_processing_vbi-1.9.1.tar", last modified: Thu May  9 21:06:44 2024, max compression
```

## Comparing `dkist_processing_vbi-1.9.0rc1.tar` & `dkist_processing_vbi-1.9.1.tar`

### file list

```diff
@@ -1,90 +1,89 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-08 02:03:52.228695 dkist_processing_vbi-1.9.0rc1/
--rw-rw-rw-   0 root         (0) root         (0)     2410 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      813 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)      306 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/.readthedocs.yml
--rw-rw-rw-   0 root         (0) root         (0)    17271 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/CHANGELOG.rst
--rw-rw-rw-   0 root         (0) root         (0)     6372 2024-05-08 02:03:52.228695 dkist_processing_vbi-1.9.0rc1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     5696 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/README.rst
--rw-rw-rw-   0 root         (0) root         (0)      307 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/SCIENCE_CHANGELOG.rst
--rw-rw-rw-   0 root         (0) root         (0)     5465 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/bitbucket-pipelines.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-08 02:03:52.224695 dkist_processing_vbi-1.9.0rc1/changelog/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/changelog/.gitempty
--rw-rw-rw-   0 root         (0) root         (0)       66 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/changelog/72.feature.rst
--rwxrwxrwx   0 root         (0) root         (0)      642 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/check_changelog_updated.sh
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-08 02:03:52.224695 dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/
--rw-rw-rw-   0 root         (0) root         (0)      348 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-08 02:03:52.224695 dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/models/
--rw-rw-rw-   0 root         (0) root         (0)       12 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3128 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/models/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     1512 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/models/filter.py
--rw-rw-rw-   0 root         (0) root         (0)      747 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/models/tags.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-08 02:03:52.224695 dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/parsers/
--rw-rw-rw-   0 root         (0) root         (0)       12 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/parsers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     7036 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/parsers/mosaic_repeats.py
--rw-rw-rw-   0 root         (0) root         (0)     1616 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/parsers/spatial_step_pattern.py
--rw-rw-rw-   0 root         (0) root         (0)     1209 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/parsers/vbi_l0_fits_access.py
--rw-rw-rw-   0 root         (0) root         (0)      994 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/parsers/vbi_l1_fits_access.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-08 02:03:52.228695 dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/tasks/
--rw-rw-rw-   0 root         (0) root         (0)      488 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/tasks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3040 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/tasks/assemble_movie.py
--rw-rw-rw-   0 root         (0) root         (0)     4320 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/tasks/dark.py
--rw-rw-rw-   0 root         (0) root         (0)     6404 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/tasks/gain.py
--rw-rw-rw-   0 root         (0) root         (0)    14101 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/tasks/make_movie_frames.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-08 02:03:52.228695 dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/tasks/mixin/
--rw-rw-rw-   0 root         (0) root         (0)       12 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/tasks/mixin/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2187 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/tasks/mixin/intermediate_loaders.py
--rw-rw-rw-   0 root         (0) root         (0)     3069 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/tasks/parse.py
--rw-rw-rw-   0 root         (0) root         (0)     2194 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/tasks/process_summit_processed.py
--rw-rw-rw-   0 root         (0) root         (0)     2301 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/tasks/quality_metrics.py
--rw-rw-rw-   0 root         (0) root         (0)     5873 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/tasks/science.py
--rw-rw-rw-   0 root         (0) root         (0)      804 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/tasks/vbi_base.py
--rw-rw-rw-   0 root         (0) root         (0)     5477 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/tasks/write_l1.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-08 02:03:52.228695 dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9879 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/tests/conftest.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-08 02:03:52.228695 dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/tests/local_trial_workflows/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/tests/local_trial_workflows/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9275 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/tests/local_trial_workflows/l0_to_l1.py
--rw-rw-rw-   0 root         (0) root         (0)     2499 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/tests/test_assemble_movie.py
--rw-rw-rw-   0 root         (0) root         (0)     4790 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/tests/test_dark.py
--rw-rw-rw-   0 root         (0) root         (0)     4320 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/tests/test_gain.py
--rw-rw-rw-   0 root         (0) root         (0)     3536 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/tests/test_intermediate_loaders.py
--rw-rw-rw-   0 root         (0) root         (0)    10401 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/tests/test_make_movie_frames.py
--rw-rw-rw-   0 root         (0) root         (0)    13274 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/tests/test_parse_l0.py
--rw-rw-rw-   0 root         (0) root         (0)     5599 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/tests/test_parse_summit.py
--rw-rw-rw-   0 root         (0) root         (0)     8467 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/tests/test_process_summit.py
--rw-rw-rw-   0 root         (0) root         (0)     2497 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/tests/test_quality_metrics.py
--rw-rw-rw-   0 root         (0) root         (0)     6828 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/tests/test_science.py
--rw-rw-rw-   0 root         (0) root         (0)     2571 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/tests/test_spatial_step_pattern.py
--rw-rw-rw-   0 root         (0) root         (0)     1016 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/tests/test_vbi_base.py
--rw-rw-rw-   0 root         (0) root         (0)     4348 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/tests/test_vbi_constants.py
--rw-rw-rw-   0 root         (0) root         (0)      285 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/tests/test_workflows.py
--rw-rw-rw-   0 root         (0) root         (0)     7374 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/tests/test_write_l1.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-08 02:03:52.228695 dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/workflows/
--rw-rw-rw-   0 root         (0) root         (0)       12 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/workflows/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2877 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/workflows/l0_processing.py
--rw-rw-rw-   0 root         (0) root         (0)     2707 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/workflows/summit_data_processing.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-08 02:03:52.224695 dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     6372 2024-05-08 02:03:52.000000 dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2789 2024-05-08 02:03:52.000000 dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-05-08 02:03:52.000000 dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)      822 2024-05-08 02:03:52.000000 dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       21 2024-05-08 02:03:52.000000 dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-08 02:03:52.228695 dkist_processing_vbi-1.9.0rc1/docs/
--rw-rw-rw-   0 root         (0) root         (0)     4598 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)      346 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/docs/changelog.rst
--rw-rw-rw-   0 root         (0) root         (0)     2026 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)      224 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)      655 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/docs/l0_to_l1_vbi_no-speckle.rst
--rw-rw-rw-   0 root         (0) root         (0)      613 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/docs/l0_to_l1_vbi_summit-calibrated.rst
--rw-rw-rw-   0 root         (0) root         (0)     4513 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/docs/make.bat
--rw-rw-rw-   0 root         (0) root         (0)       29 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/docs/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      291 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/docs/requirements_table.rst
--rw-rw-rw-   0 root         (0) root         (0)      300 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/docs/scientific_changelog.rst
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-08 02:03:52.228695 dkist_processing_vbi-1.9.0rc1/licenses/
--rw-rw-rw-   0 root         (0) root         (0)     1462 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/licenses/LICENSE.rst
--rw-rw-rw-   0 root         (0) root         (0)      774 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/pyproject.toml
--rwxrwxrwx   0 root         (0) root         (0)       60 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/science_towncrier.sh
--rw-rw-rw-   0 root         (0) root         (0)     1881 2024-05-08 02:03:52.232695 dkist_processing_vbi-1.9.0rc1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      102 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/setup.py
--rw-rw-rw-   0 root         (0) root         (0)      420 2024-05-08 02:03:45.000000 dkist_processing_vbi-1.9.0rc1/towncrier_science.toml
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-09 21:06:44.154650 dkist_processing_vbi-1.9.1/
+-rw-rw-rw-   0 root         (0) root         (0)     2410 2024-05-09 21:06:37.000000 dkist_processing_vbi-1.9.1/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      813 2024-05-09 21:06:37.000000 dkist_processing_vbi-1.9.1/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      306 2024-05-09 21:06:37.000000 dkist_processing_vbi-1.9.1/.readthedocs.yml
+-rw-rw-rw-   0 root         (0) root         (0)    17640 2024-05-09 21:06:37.000000 dkist_processing_vbi-1.9.1/CHANGELOG.rst
+-rw-rw-rw-   0 root         (0) root         (0)     6369 2024-05-09 21:06:44.154650 dkist_processing_vbi-1.9.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     5696 2024-05-09 21:06:37.000000 dkist_processing_vbi-1.9.1/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)      307 2024-05-09 21:06:37.000000 dkist_processing_vbi-1.9.1/SCIENCE_CHANGELOG.rst
+-rw-rw-rw-   0 root         (0) root         (0)     5465 2024-05-09 21:06:37.000000 dkist_processing_vbi-1.9.1/bitbucket-pipelines.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-09 21:06:44.150650 dkist_processing_vbi-1.9.1/changelog/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-09 21:06:37.000000 dkist_processing_vbi-1.9.1/changelog/.gitempty
+-rwxrwxrwx   0 root         (0) root         (0)      642 2024-05-09 21:06:37.000000 dkist_processing_vbi-1.9.1/check_changelog_updated.sh
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-09 21:06:44.150650 dkist_processing_vbi-1.9.1/dkist_processing_vbi/
+-rw-rw-rw-   0 root         (0) root         (0)      348 2024-05-09 21:06:37.000000 dkist_processing_vbi-1.9.1/dkist_processing_vbi/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-09 21:06:44.150650 dkist_processing_vbi-1.9.1/dkist_processing_vbi/models/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2024-05-09 21:06:37.000000 dkist_processing_vbi-1.9.1/dkist_processing_vbi/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3128 2024-05-09 21:06:37.000000 dkist_processing_vbi-1.9.1/dkist_processing_vbi/models/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     1512 2024-05-09 21:06:37.000000 dkist_processing_vbi-1.9.1/dkist_processing_vbi/models/filter.py
+-rw-rw-rw-   0 root         (0) root         (0)      747 2024-05-09 21:06:37.000000 dkist_processing_vbi-1.9.1/dkist_processing_vbi/models/tags.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-09 21:06:44.150650 dkist_processing_vbi-1.9.1/dkist_processing_vbi/parsers/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2024-05-09 21:06:37.000000 dkist_processing_vbi-1.9.1/dkist_processing_vbi/parsers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     7036 2024-05-09 21:06:37.000000 dkist_processing_vbi-1.9.1/dkist_processing_vbi/parsers/mosaic_repeats.py
+-rw-rw-rw-   0 root         (0) root         (0)     1616 2024-05-09 21:06:37.000000 dkist_processing_vbi-1.9.1/dkist_processing_vbi/parsers/spatial_step_pattern.py
+-rw-rw-rw-   0 root         (0) root         (0)     1209 2024-05-09 21:06:37.000000 dkist_processing_vbi-1.9.1/dkist_processing_vbi/parsers/vbi_l0_fits_access.py
+-rw-rw-rw-   0 root         (0) root         (0)      994 2024-05-09 21:06:37.000000 dkist_processing_vbi-1.9.1/dkist_processing_vbi/parsers/vbi_l1_fits_access.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-09 21:06:44.154650 dkist_processing_vbi-1.9.1/dkist_processing_vbi/tasks/
+-rw-rw-rw-   0 root         (0) root         (0)      488 2024-05-09 21:06:37.000000 dkist_processing_vbi-1.9.1/dkist_processing_vbi/tasks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3040 2024-05-09 21:06:37.000000 dkist_processing_vbi-1.9.1/dkist_processing_vbi/tasks/assemble_movie.py
+-rw-rw-rw-   0 root         (0) root         (0)     4320 2024-05-09 21:06:37.000000 dkist_processing_vbi-1.9.1/dkist_processing_vbi/tasks/dark.py
+-rw-rw-rw-   0 root         (0) root         (0)     6404 2024-05-09 21:06:37.000000 dkist_processing_vbi-1.9.1/dkist_processing_vbi/tasks/gain.py
+-rw-rw-rw-   0 root         (0) root         (0)    14101 2024-05-09 21:06:37.000000 dkist_processing_vbi-1.9.1/dkist_processing_vbi/tasks/make_movie_frames.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-09 21:06:44.154650 dkist_processing_vbi-1.9.1/dkist_processing_vbi/tasks/mixin/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2024-05-09 21:06:37.000000 dkist_processing_vbi-1.9.1/dkist_processing_vbi/tasks/mixin/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2187 2024-05-09 21:06:37.000000 dkist_processing_vbi-1.9.1/dkist_processing_vbi/tasks/mixin/intermediate_loaders.py
+-rw-rw-rw-   0 root         (0) root         (0)     3069 2024-05-09 21:06:37.000000 dkist_processing_vbi-1.9.1/dkist_processing_vbi/tasks/parse.py
+-rw-rw-rw-   0 root         (0) root         (0)     2194 2024-05-09 21:06:37.000000 dkist_processing_vbi-1.9.1/dkist_processing_vbi/tasks/process_summit_processed.py
+-rw-rw-rw-   0 root         (0) root         (0)     2301 2024-05-09 21:06:37.000000 dkist_processing_vbi-1.9.1/dkist_processing_vbi/tasks/quality_metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)     5873 2024-05-09 21:06:37.000000 dkist_processing_vbi-1.9.1/dkist_processing_vbi/tasks/science.py
+-rw-rw-rw-   0 root         (0) root         (0)      804 2024-05-09 21:06:37.000000 dkist_processing_vbi-1.9.1/dkist_processing_vbi/tasks/vbi_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     5477 2024-05-09 21:06:37.000000 dkist_processing_vbi-1.9.1/dkist_processing_vbi/tasks/write_l1.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-09 21:06:44.154650 dkist_processing_vbi-1.9.1/dkist_processing_vbi/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-09 21:06:37.000000 dkist_processing_vbi-1.9.1/dkist_processing_vbi/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9879 2024-05-09 21:06:37.000000 dkist_processing_vbi-1.9.1/dkist_processing_vbi/tests/conftest.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-09 21:06:44.154650 dkist_processing_vbi-1.9.1/dkist_processing_vbi/tests/local_trial_workflows/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-09 21:06:37.000000 dkist_processing_vbi-1.9.1/dkist_processing_vbi/tests/local_trial_workflows/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9275 2024-05-09 21:06:37.000000 dkist_processing_vbi-1.9.1/dkist_processing_vbi/tests/local_trial_workflows/l0_to_l1.py
+-rw-rw-rw-   0 root         (0) root         (0)     2499 2024-05-09 21:06:37.000000 dkist_processing_vbi-1.9.1/dkist_processing_vbi/tests/test_assemble_movie.py
+-rw-rw-rw-   0 root         (0) root         (0)     4790 2024-05-09 21:06:37.000000 dkist_processing_vbi-1.9.1/dkist_processing_vbi/tests/test_dark.py
+-rw-rw-rw-   0 root         (0) root         (0)     4320 2024-05-09 21:06:37.000000 dkist_processing_vbi-1.9.1/dkist_processing_vbi/tests/test_gain.py
+-rw-rw-rw-   0 root         (0) root         (0)     3536 2024-05-09 21:06:37.000000 dkist_processing_vbi-1.9.1/dkist_processing_vbi/tests/test_intermediate_loaders.py
+-rw-rw-rw-   0 root         (0) root         (0)    10401 2024-05-09 21:06:37.000000 dkist_processing_vbi-1.9.1/dkist_processing_vbi/tests/test_make_movie_frames.py
+-rw-rw-rw-   0 root         (0) root         (0)    13274 2024-05-09 21:06:37.000000 dkist_processing_vbi-1.9.1/dkist_processing_vbi/tests/test_parse_l0.py
+-rw-rw-rw-   0 root         (0) root         (0)     5599 2024-05-09 21:06:37.000000 dkist_processing_vbi-1.9.1/dkist_processing_vbi/tests/test_parse_summit.py
+-rw-rw-rw-   0 root         (0) root         (0)     8467 2024-05-09 21:06:37.000000 dkist_processing_vbi-1.9.1/dkist_processing_vbi/tests/test_process_summit.py
+-rw-rw-rw-   0 root         (0) root         (0)     2497 2024-05-09 21:06:37.000000 dkist_processing_vbi-1.9.1/dkist_processing_vbi/tests/test_quality_metrics.py
+-rw-rw-rw-   0 root         (0) root         (0)     6828 2024-05-09 21:06:37.000000 dkist_processing_vbi-1.9.1/dkist_processing_vbi/tests/test_science.py
+-rw-rw-rw-   0 root         (0) root         (0)     2571 2024-05-09 21:06:37.000000 dkist_processing_vbi-1.9.1/dkist_processing_vbi/tests/test_spatial_step_pattern.py
+-rw-rw-rw-   0 root         (0) root         (0)     1016 2024-05-09 21:06:37.000000 dkist_processing_vbi-1.9.1/dkist_processing_vbi/tests/test_vbi_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     4348 2024-05-09 21:06:37.000000 dkist_processing_vbi-1.9.1/dkist_processing_vbi/tests/test_vbi_constants.py
+-rw-rw-rw-   0 root         (0) root         (0)      285 2024-05-09 21:06:37.000000 dkist_processing_vbi-1.9.1/dkist_processing_vbi/tests/test_workflows.py
+-rw-rw-rw-   0 root         (0) root         (0)     7374 2024-05-09 21:06:37.000000 dkist_processing_vbi-1.9.1/dkist_processing_vbi/tests/test_write_l1.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-09 21:06:44.154650 dkist_processing_vbi-1.9.1/dkist_processing_vbi/workflows/
+-rw-rw-rw-   0 root         (0) root         (0)       12 2024-05-09 21:06:37.000000 dkist_processing_vbi-1.9.1/dkist_processing_vbi/workflows/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2877 2024-05-09 21:06:37.000000 dkist_processing_vbi-1.9.1/dkist_processing_vbi/workflows/l0_processing.py
+-rw-rw-rw-   0 root         (0) root         (0)     2707 2024-05-09 21:06:37.000000 dkist_processing_vbi-1.9.1/dkist_processing_vbi/workflows/summit_data_processing.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-09 21:06:44.150650 dkist_processing_vbi-1.9.1/dkist_processing_vbi.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     6369 2024-05-09 21:06:44.000000 dkist_processing_vbi-1.9.1/dkist_processing_vbi.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2764 2024-05-09 21:06:44.000000 dkist_processing_vbi-1.9.1/dkist_processing_vbi.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-05-09 21:06:44.000000 dkist_processing_vbi-1.9.1/dkist_processing_vbi.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)      822 2024-05-09 21:06:44.000000 dkist_processing_vbi-1.9.1/dkist_processing_vbi.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       21 2024-05-09 21:06:44.000000 dkist_processing_vbi-1.9.1/dkist_processing_vbi.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-09 21:06:44.154650 dkist_processing_vbi-1.9.1/docs/
+-rw-rw-rw-   0 root         (0) root         (0)     4598 2024-05-09 21:06:37.000000 dkist_processing_vbi-1.9.1/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)      346 2024-05-09 21:06:37.000000 dkist_processing_vbi-1.9.1/docs/changelog.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2026 2024-05-09 21:06:37.000000 dkist_processing_vbi-1.9.1/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)      224 2024-05-09 21:06:37.000000 dkist_processing_vbi-1.9.1/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)      655 2024-05-09 21:06:37.000000 dkist_processing_vbi-1.9.1/docs/l0_to_l1_vbi_no-speckle.rst
+-rw-rw-rw-   0 root         (0) root         (0)      613 2024-05-09 21:06:37.000000 dkist_processing_vbi-1.9.1/docs/l0_to_l1_vbi_summit-calibrated.rst
+-rw-rw-rw-   0 root         (0) root         (0)     4513 2024-05-09 21:06:37.000000 dkist_processing_vbi-1.9.1/docs/make.bat
+-rw-rw-rw-   0 root         (0) root         (0)       29 2024-05-09 21:06:37.000000 dkist_processing_vbi-1.9.1/docs/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)      291 2024-05-09 21:06:37.000000 dkist_processing_vbi-1.9.1/docs/requirements_table.rst
+-rw-rw-rw-   0 root         (0) root         (0)      300 2024-05-09 21:06:37.000000 dkist_processing_vbi-1.9.1/docs/scientific_changelog.rst
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-09 21:06:44.154650 dkist_processing_vbi-1.9.1/licenses/
+-rw-rw-rw-   0 root         (0) root         (0)     1462 2024-05-09 21:06:37.000000 dkist_processing_vbi-1.9.1/licenses/LICENSE.rst
+-rw-rw-rw-   0 root         (0) root         (0)      774 2024-05-09 21:06:37.000000 dkist_processing_vbi-1.9.1/pyproject.toml
+-rwxrwxrwx   0 root         (0) root         (0)       60 2024-05-09 21:06:37.000000 dkist_processing_vbi-1.9.1/science_towncrier.sh
+-rw-rw-rw-   0 root         (0) root         (0)     1881 2024-05-09 21:06:44.158650 dkist_processing_vbi-1.9.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      102 2024-05-09 21:06:37.000000 dkist_processing_vbi-1.9.1/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)      420 2024-05-09 21:06:37.000000 dkist_processing_vbi-1.9.1/towncrier_science.toml
```

### Comparing `dkist_processing_vbi-1.9.0rc1/.gitignore` & `dkist_processing_vbi-1.9.1/.gitignore`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.9.0rc1/.pre-commit-config.yaml` & `dkist_processing_vbi-1.9.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.9.0rc1/CHANGELOG.rst` & `dkist_processing_vbi-1.9.1/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+v1.9.1 (2024-05-09)
+===================
+
+Misc
+----
+
+- Bumped to common 6.3.2 (`#74 <https://bitbucket.org/dkistdc/dkist-processing-vbi/pull-requests/74>`__)
+
+
+v1.9.0 (2024-05-08)
+===================
+
+Features
+--------
+
+- Add the ability to create a quality report from a trial workflow. (`#72 <https://bitbucket.org/dkistdc/dkist-processing-vbi/pull-requests/72>`__)
+
+
 v1.8.9 (2024-05-02)
 ===================
 
 Misc
 ----
 
 - Rename non-FITS L1 products to better manage namespace. (`#73 <https://bitbucket.org/dkistdc/dkist-processing-vbi/pull-requests/73>`__)
```

### Comparing `dkist_processing_vbi-1.9.0rc1/PKG-INFO` & `dkist_processing_vbi-1.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist_processing_vbi
-Version: 1.9.0rc1
+Version: 1.9.1
 Summary: Code that is used by the DKIST Science Data Processing Airflow pipelines to process VBI data.
 Home-page: https://bitbucket.org/dkistdc/dkist-processing-vbi/src/main/
 Author: NSO / AURA
 Author-email: "dkistdc@nso.edu"
 License: MIT
 Project-URL: Documentation, https://docs.dkist.nso.edu/projects/vbi
 Classifier: Programming Language :: Python
```

### Comparing `dkist_processing_vbi-1.9.0rc1/README.rst` & `dkist_processing_vbi-1.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.9.0rc1/bitbucket-pipelines.yml` & `dkist_processing_vbi-1.9.1/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.9.0rc1/check_changelog_updated.sh` & `dkist_processing_vbi-1.9.1/check_changelog_updated.sh`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/models/constants.py` & `dkist_processing_vbi-1.9.1/dkist_processing_vbi/models/constants.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/models/filter.py` & `dkist_processing_vbi-1.9.1/dkist_processing_vbi/models/filter.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/models/tags.py` & `dkist_processing_vbi-1.9.1/dkist_processing_vbi/models/tags.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/parsers/mosaic_repeats.py` & `dkist_processing_vbi-1.9.1/dkist_processing_vbi/parsers/mosaic_repeats.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/parsers/spatial_step_pattern.py` & `dkist_processing_vbi-1.9.1/dkist_processing_vbi/parsers/spatial_step_pattern.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/parsers/vbi_l0_fits_access.py` & `dkist_processing_vbi-1.9.1/dkist_processing_vbi/parsers/vbi_l0_fits_access.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/parsers/vbi_l1_fits_access.py` & `dkist_processing_vbi-1.9.1/dkist_processing_vbi/parsers/vbi_l1_fits_access.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/tasks/assemble_movie.py` & `dkist_processing_vbi-1.9.1/dkist_processing_vbi/tasks/assemble_movie.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/tasks/dark.py` & `dkist_processing_vbi-1.9.1/dkist_processing_vbi/tasks/dark.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/tasks/gain.py` & `dkist_processing_vbi-1.9.1/dkist_processing_vbi/tasks/gain.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/tasks/make_movie_frames.py` & `dkist_processing_vbi-1.9.1/dkist_processing_vbi/tasks/make_movie_frames.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/tasks/mixin/intermediate_loaders.py` & `dkist_processing_vbi-1.9.1/dkist_processing_vbi/tasks/mixin/intermediate_loaders.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/tasks/parse.py` & `dkist_processing_vbi-1.9.1/dkist_processing_vbi/tasks/parse.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/tasks/process_summit_processed.py` & `dkist_processing_vbi-1.9.1/dkist_processing_vbi/tasks/process_summit_processed.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/tasks/quality_metrics.py` & `dkist_processing_vbi-1.9.1/dkist_processing_vbi/tasks/quality_metrics.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/tasks/science.py` & `dkist_processing_vbi-1.9.1/dkist_processing_vbi/tasks/science.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/tasks/vbi_base.py` & `dkist_processing_vbi-1.9.1/dkist_processing_vbi/tasks/vbi_base.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/tasks/write_l1.py` & `dkist_processing_vbi-1.9.1/dkist_processing_vbi/tasks/write_l1.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/tests/conftest.py` & `dkist_processing_vbi-1.9.1/dkist_processing_vbi/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/tests/local_trial_workflows/l0_to_l1.py` & `dkist_processing_vbi-1.9.1/dkist_processing_vbi/tests/local_trial_workflows/l0_to_l1.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/tests/test_assemble_movie.py` & `dkist_processing_vbi-1.9.1/dkist_processing_vbi/tests/test_assemble_movie.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/tests/test_dark.py` & `dkist_processing_vbi-1.9.1/dkist_processing_vbi/tests/test_dark.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/tests/test_gain.py` & `dkist_processing_vbi-1.9.1/dkist_processing_vbi/tests/test_gain.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/tests/test_intermediate_loaders.py` & `dkist_processing_vbi-1.9.1/dkist_processing_vbi/tests/test_intermediate_loaders.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/tests/test_make_movie_frames.py` & `dkist_processing_vbi-1.9.1/dkist_processing_vbi/tests/test_make_movie_frames.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/tests/test_parse_l0.py` & `dkist_processing_vbi-1.9.1/dkist_processing_vbi/tests/test_parse_l0.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/tests/test_parse_summit.py` & `dkist_processing_vbi-1.9.1/dkist_processing_vbi/tests/test_parse_summit.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/tests/test_process_summit.py` & `dkist_processing_vbi-1.9.1/dkist_processing_vbi/tests/test_process_summit.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/tests/test_quality_metrics.py` & `dkist_processing_vbi-1.9.1/dkist_processing_vbi/tests/test_quality_metrics.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/tests/test_science.py` & `dkist_processing_vbi-1.9.1/dkist_processing_vbi/tests/test_science.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/tests/test_spatial_step_pattern.py` & `dkist_processing_vbi-1.9.1/dkist_processing_vbi/tests/test_spatial_step_pattern.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/tests/test_vbi_base.py` & `dkist_processing_vbi-1.9.1/dkist_processing_vbi/tests/test_vbi_base.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/tests/test_vbi_constants.py` & `dkist_processing_vbi-1.9.1/dkist_processing_vbi/tests/test_vbi_constants.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/tests/test_write_l1.py` & `dkist_processing_vbi-1.9.1/dkist_processing_vbi/tests/test_write_l1.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/workflows/l0_processing.py` & `dkist_processing_vbi-1.9.1/dkist_processing_vbi/workflows/l0_processing.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi/workflows/summit_data_processing.py` & `dkist_processing_vbi-1.9.1/dkist_processing_vbi/workflows/summit_data_processing.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi.egg-info/PKG-INFO` & `dkist_processing_vbi-1.9.1/dkist_processing_vbi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist-processing-vbi
-Version: 1.9.0rc1
+Version: 1.9.1
 Summary: Code that is used by the DKIST Science Data Processing Airflow pipelines to process VBI data.
 Home-page: https://bitbucket.org/dkistdc/dkist-processing-vbi/src/main/
 Author: NSO / AURA
 Author-email: "dkistdc@nso.edu"
 License: MIT
 Project-URL: Documentation, https://docs.dkist.nso.edu/projects/vbi
 Classifier: Programming Language :: Python
```

### Comparing `dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi.egg-info/SOURCES.txt` & `dkist_processing_vbi-1.9.1/dkist_processing_vbi.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 check_changelog_updated.sh
 pyproject.toml
 science_towncrier.sh
 setup.cfg
 setup.py
 towncrier_science.toml
 changelog/.gitempty
-changelog/72.feature.rst
 dkist_processing_vbi/__init__.py
 dkist_processing_vbi.egg-info/PKG-INFO
 dkist_processing_vbi.egg-info/SOURCES.txt
 dkist_processing_vbi.egg-info/dependency_links.txt
 dkist_processing_vbi.egg-info/requires.txt
 dkist_processing_vbi.egg-info/top_level.txt
 dkist_processing_vbi/models/__init__.py
```

### Comparing `dkist_processing_vbi-1.9.0rc1/dkist_processing_vbi.egg-info/requires.txt` & `dkist_processing_vbi-1.9.1/dkist_processing_vbi.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-dkist-processing-common==6.2.2
+dkist-processing-common==6.2.3
 dkist-processing-math==2.1.0
 dkist-header-validator==5.1.0
 dkist-fits-specifications==4.1.1
 astropy==5.3.0
 numpy==1.24.3
 sunpy==5.0.0
 scipy==1.11.0
```

### Comparing `dkist_processing_vbi-1.9.0rc1/docs/Makefile` & `dkist_processing_vbi-1.9.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.9.0rc1/docs/conf.py` & `dkist_processing_vbi-1.9.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.9.0rc1/docs/l0_to_l1_vbi_no-speckle.rst` & `dkist_processing_vbi-1.9.1/docs/l0_to_l1_vbi_no-speckle.rst`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.9.0rc1/docs/l0_to_l1_vbi_summit-calibrated.rst` & `dkist_processing_vbi-1.9.1/docs/l0_to_l1_vbi_summit-calibrated.rst`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.9.0rc1/docs/make.bat` & `dkist_processing_vbi-1.9.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.9.0rc1/licenses/LICENSE.rst` & `dkist_processing_vbi-1.9.1/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.9.0rc1/pyproject.toml` & `dkist_processing_vbi-1.9.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dkist_processing_vbi-1.9.0rc1/setup.cfg` & `dkist_processing_vbi-1.9.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 [options]
 python_requires = >=3.11
 setup_requires = setuptools_scm
 packages = find:
 include_package_data = True
 install_requires = 
-	dkist-processing-common == 6.2.2
+	dkist-processing-common == 6.2.3
 	dkist-processing-math == 2.1.0
 	dkist-header-validator == 5.1.0
 	dkist-fits-specifications == 4.1.1
 	astropy == 5.3.0
 	numpy == 1.24.3
 	sunpy == 5.0.0
 	scipy == 1.11.0
```

