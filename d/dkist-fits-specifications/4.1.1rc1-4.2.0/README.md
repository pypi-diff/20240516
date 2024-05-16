# Comparing `tmp/dkist_fits_specifications-4.1.1rc1.tar.gz` & `tmp/dkist_fits_specifications-4.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dkist_fits_specifications-4.1.1rc1.tar", last modified: Mon Feb 26 10:31:13 2024, max compression
+gzip compressed data, was "dkist_fits_specifications-4.2.0.tar", last modified: Thu May 16 16:07:22 2024, max compression
```

## Comparing `dkist_fits_specifications-4.1.1rc1.tar` & `dkist_fits_specifications-4.2.0.tar`

### file list

```diff
@@ -1,105 +1,105 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-26 10:31:13.432700 dkist_fits_specifications-4.1.1rc1/
--rw-rw-rw-   0 root         (0) root         (0)     3334 2024-02-26 10:30:55.000000 dkist_fits_specifications-4.1.1rc1/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      676 2024-02-26 10:30:55.000000 dkist_fits_specifications-4.1.1rc1/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)      306 2024-02-26 10:30:55.000000 dkist_fits_specifications-4.1.1rc1/.readthedocs.yml
--rw-rw-rw-   0 root         (0) root         (0)     9637 2024-02-26 10:30:55.000000 dkist_fits_specifications-4.1.1rc1/CHANGELOG.rst
--rw-rw-rw-   0 root         (0) root         (0)       71 2024-02-26 10:30:55.000000 dkist_fits_specifications-4.1.1rc1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     7309 2024-02-26 10:31:13.432700 dkist_fits_specifications-4.1.1rc1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     6270 2024-02-26 10:30:55.000000 dkist_fits_specifications-4.1.1rc1/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     2285 2024-02-26 10:30:55.000000 dkist_fits_specifications-4.1.1rc1/bitbucket-pipelines.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-26 10:31:13.420699 dkist_fits_specifications-4.1.1rc1/changelog/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-26 10:30:55.000000 dkist_fits_specifications-4.1.1rc1/changelog/.gitempty
--rw-rw-rw-   0 root         (0) root         (0)       46 2024-02-26 10:30:55.000000 dkist_fits_specifications-4.1.1rc1/changelog/48.bugfix.rst
--rwxrwxrwx   0 root         (0) root         (0)      642 2024-02-26 10:30:55.000000 dkist_fits_specifications-4.1.1rc1/check_changelog_updated.sh
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-26 10:31:13.420699 dkist_fits_specifications-4.1.1rc1/dkist_fits_specifications/
--rw-rw-rw-   0 root         (0) root         (0)      870 2024-02-26 10:30:55.000000 dkist_fits_specifications-4.1.1rc1/dkist_fits_specifications/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-26 10:30:55.000000 dkist_fits_specifications-4.1.1rc1/dkist_fits_specifications/py.typed
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-26 10:31:13.420699 dkist_fits_specifications-4.1.1rc1/dkist_fits_specifications/spec122/
--rw-rw-rw-   0 root         (0) root         (0)     6204 2024-02-26 10:30:55.000000 dkist_fits_specifications-4.1.1rc1/dkist_fits_specifications/spec122/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-26 10:31:13.424700 dkist_fits_specifications-4.1.1rc1/dkist_fits_specifications/spec122/schemas/
--rw-rw-rw-   0 root         (0) root         (0)      792 2024-02-26 10:30:55.000000 dkist_fits_specifications-4.1.1rc1/dkist_fits_specifications/spec122/schemas/ao.yml
--rw-rw-rw-   0 root         (0) root         (0)     2951 2024-02-26 10:30:55.000000 dkist_fits_specifications-4.1.1rc1/dkist_fits_specifications/spec122/schemas/camera.yml
--rw-rw-rw-   0 root         (0) root         (0)      515 2024-02-26 10:30:55.000000 dkist_fits_specifications-4.1.1rc1/dkist_fits_specifications/spec122/schemas/compression.yml
--rw-rw-rw-   0 root         (0) root         (0)    13916 2024-02-26 10:30:55.000000 dkist_fits_specifications-4.1.1rc1/dkist_fits_specifications/spec122/schemas/cryonirsp.yml
--rw-rw-rw-   0 root         (0) root         (0)     1466 2024-02-26 10:30:55.000000 dkist_fits_specifications-4.1.1rc1/dkist_fits_specifications/spec122/schemas/dkist-dkist.yml
--rw-rw-rw-   0 root         (0) root         (0)     1088 2024-02-26 10:30:55.000000 dkist_fits_specifications-4.1.1rc1/dkist_fits_specifications/spec122/schemas/dkist-id.yml
--rw-rw-rw-   0 root         (0) root         (0)     5667 2024-02-26 10:30:55.000000 dkist_fits_specifications-4.1.1rc1/dkist_fits_specifications/spec122/schemas/dlnirsp.yml
--rw-rw-rw-   0 root         (0) root         (0)     1709 2024-02-26 10:30:55.000000 dkist_fits_specifications-4.1.1rc1/dkist_fits_specifications/spec122/schemas/fits.yml
--rw-rw-rw-   0 root         (0) root         (0)     1934 2024-02-26 10:30:55.000000 dkist_fits_specifications-4.1.1rc1/dkist_fits_specifications/spec122/schemas/pac.yml
--rw-rw-rw-   0 root         (0) root         (0)     2653 2024-02-26 10:30:55.000000 dkist_fits_specifications-4.1.1rc1/dkist_fits_specifications/spec122/schemas/telescope.yml
--rw-rw-rw-   0 root         (0) root         (0)      957 2024-02-26 10:30:55.000000 dkist_fits_specifications-4.1.1rc1/dkist_fits_specifications/spec122/schemas/vbi.yml
--rw-rw-rw-   0 root         (0) root         (0)     3579 2024-02-26 10:30:55.000000 dkist_fits_specifications-4.1.1rc1/dkist_fits_specifications/spec122/schemas/visp.yml
--rw-rw-rw-   0 root         (0) root         (0)     2326 2024-02-26 10:30:55.000000 dkist_fits_specifications-4.1.1rc1/dkist_fits_specifications/spec122/schemas/vtf.yml
--rw-rw-rw-   0 root         (0) root         (0)      776 2024-02-26 10:30:55.000000 dkist_fits_specifications-4.1.1rc1/dkist_fits_specifications/spec122/schemas/wfc.yml
--rw-rw-rw-   0 root         (0) root         (0)      703 2024-02-26 10:30:55.000000 dkist_fits_specifications-4.1.1rc1/dkist_fits_specifications/spec122/schemas/ws.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-26 10:31:13.424700 dkist_fits_specifications-4.1.1rc1/dkist_fits_specifications/spec214/
--rw-rw-rw-   0 root         (0) root         (0)    13981 2024-02-26 10:30:55.000000 dkist_fits_specifications-4.1.1rc1/dkist_fits_specifications/spec214/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3421 2024-02-26 10:30:55.000000 dkist_fits_specifications-4.1.1rc1/dkist_fits_specifications/spec214/level0.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-26 10:31:13.428700 dkist_fits_specifications-4.1.1rc1/dkist_fits_specifications/spec214/schemas/
--rw-rw-rw-   0 root         (0) root         (0)     1973 2024-02-26 10:30:55.000000 dkist_fits_specifications-4.1.1rc1/dkist_fits_specifications/spec214/schemas/ao.yml
--rw-rw-rw-   0 root         (0) root         (0)     5886 2024-02-26 10:30:55.000000 dkist_fits_specifications-4.1.1rc1/dkist_fits_specifications/spec214/schemas/camera.yml
--rw-rw-rw-   0 root         (0) root         (0)     6424 2024-02-26 10:30:55.000000 dkist_fits_specifications-4.1.1rc1/dkist_fits_specifications/spec214/schemas/compression.yml
--rw-rw-rw-   0 root         (0) root         (0)    13579 2024-02-26 10:30:55.000000 dkist_fits_specifications-4.1.1rc1/dkist_fits_specifications/spec214/schemas/cryonirsp.yml
--rw-rw-rw-   0 root         (0) root         (0)     4107 2024-02-26 10:30:55.000000 dkist_fits_specifications-4.1.1rc1/dkist_fits_specifications/spec214/schemas/datacenter.yml
--rw-rw-rw-   0 root         (0) root         (0)     4144 2024-02-26 10:30:55.000000 dkist_fits_specifications-4.1.1rc1/dkist_fits_specifications/spec214/schemas/dataset.yml
--rw-rw-rw-   0 root         (0) root         (0)     2429 2024-02-26 10:30:55.000000 dkist_fits_specifications-4.1.1rc1/dkist_fits_specifications/spec214/schemas/dkist-id.yml
--rw-rw-rw-   0 root         (0) root         (0)     1567 2024-02-26 10:30:55.000000 dkist_fits_specifications-4.1.1rc1/dkist_fits_specifications/spec214/schemas/dkist-op.yml
--rw-rw-rw-   0 root         (0) root         (0)     8355 2024-02-26 10:30:55.000000 dkist_fits_specifications-4.1.1rc1/dkist_fits_specifications/spec214/schemas/dlnirsp.yml
--rw-rw-rw-   0 root         (0) root         (0)     7249 2024-02-26 10:30:55.000000 dkist_fits_specifications-4.1.1rc1/dkist_fits_specifications/spec214/schemas/fits.yml
--rw-rw-rw-   0 root         (0) root         (0)     2381 2024-02-26 10:30:55.000000 dkist_fits_specifications-4.1.1rc1/dkist_fits_specifications/spec214/schemas/pac.yml
--rw-rw-rw-   0 root         (0) root         (0)      778 2024-02-26 10:30:55.000000 dkist_fits_specifications-4.1.1rc1/dkist_fits_specifications/spec214/schemas/stats.yml
--rw-rw-rw-   0 root         (0) root         (0)     7346 2024-02-26 10:30:55.000000 dkist_fits_specifications-4.1.1rc1/dkist_fits_specifications/spec214/schemas/telescope.yml
--rw-rw-rw-   0 root         (0) root         (0)     1907 2024-02-26 10:30:55.000000 dkist_fits_specifications-4.1.1rc1/dkist_fits_specifications/spec214/schemas/vbi.yml
--rw-rw-rw-   0 root         (0) root         (0)     2939 2024-02-26 10:30:55.000000 dkist_fits_specifications-4.1.1rc1/dkist_fits_specifications/spec214/schemas/visp.yml
--rw-rw-rw-   0 root         (0) root         (0)     3660 2024-02-26 10:30:55.000000 dkist_fits_specifications-4.1.1rc1/dkist_fits_specifications/spec214/schemas/vtf.yml
--rw-rw-rw-   0 root         (0) root         (0)     1483 2024-02-26 10:30:55.000000 dkist_fits_specifications-4.1.1rc1/dkist_fits_specifications/spec214/schemas/wfc.yml
--rw-rw-rw-   0 root         (0) root         (0)     1310 2024-02-26 10:30:55.000000 dkist_fits_specifications-4.1.1rc1/dkist_fits_specifications/spec214/schemas/ws.yml
--rw-rw-rw-   0 root         (0) root         (0)     1090 2024-02-26 10:30:55.000000 dkist_fits_specifications-4.1.1rc1/dkist_fits_specifications/spec214/spec214_full_schema.yml
--rw-rw-rw-   0 root         (0) root         (0)      648 2024-02-26 10:30:55.000000 dkist_fits_specifications-4.1.1rc1/dkist_fits_specifications/spec_validation_schema.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-26 10:31:13.428700 dkist_fits_specifications-4.1.1rc1/dkist_fits_specifications/tests/
--rw-rw-rw-   0 root         (0) root         (0)       44 2024-02-26 10:30:55.000000 dkist_fits_specifications-4.1.1rc1/dkist_fits_specifications/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2475 2024-02-26 10:30:55.000000 dkist_fits_specifications-4.1.1rc1/dkist_fits_specifications/tests/test_122.py
--rw-rw-rw-   0 root         (0) root         (0)     8645 2024-02-26 10:30:55.000000 dkist_fits_specifications-4.1.1rc1/dkist_fits_specifications/tests/test_214.py
--rw-rw-rw-   0 root         (0) root         (0)     2842 2024-02-26 10:30:55.000000 dkist_fits_specifications-4.1.1rc1/dkist_fits_specifications/tests/test_expansions.py
--rw-rw-rw-   0 root         (0) root         (0)      744 2024-02-26 10:30:55.000000 dkist_fits_specifications-4.1.1rc1/dkist_fits_specifications/tests/test_level0_214.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-26 10:31:13.428700 dkist_fits_specifications-4.1.1rc1/dkist_fits_specifications/utils/
--rw-rw-rw-   0 root         (0) root         (0)       55 2024-02-26 10:30:55.000000 dkist_fits_specifications-4.1.1rc1/dkist_fits_specifications/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3374 2024-02-26 10:30:55.000000 dkist_fits_specifications-4.1.1rc1/dkist_fits_specifications/utils/formatter.py
--rw-rw-rw-   0 root         (0) root         (0)     1222 2024-02-26 10:30:55.000000 dkist_fits_specifications-4.1.1rc1/dkist_fits_specifications/utils/frozendict.py
--rw-rw-rw-   0 root         (0) root         (0)     2843 2024-02-26 10:30:55.000000 dkist_fits_specifications-4.1.1rc1/dkist_fits_specifications/utils/spec.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-26 10:31:13.428700 dkist_fits_specifications-4.1.1rc1/dkist_fits_specifications/utils/spec_processors/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-26 10:30:55.000000 dkist_fits_specifications-4.1.1rc1/dkist_fits_specifications/utils/spec_processors/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2489 2024-02-26 10:30:55.000000 dkist_fits_specifications-4.1.1rc1/dkist_fits_specifications/utils/spec_processors/expansion.py
--rw-rw-rw-   0 root         (0) root         (0)      933 2024-02-26 10:30:55.000000 dkist_fits_specifications-4.1.1rc1/dkist_fits_specifications/utils/spec_processors/instrument_requiredness.py
--rw-rw-rw-   0 root         (0) root         (0)     4401 2024-02-26 10:30:55.000000 dkist_fits_specifications-4.1.1rc1/dkist_fits_specifications/utils/spec_processors/polarimetric_requiredness.py
--rw-rw-rw-   0 root         (0) root         (0)     1565 2024-02-26 10:30:55.000000 dkist_fits_specifications-4.1.1rc1/dkist_fits_specifications/utils/spec_processors/requiredness_base.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-26 10:31:13.428700 dkist_fits_specifications-4.1.1rc1/dkist_fits_specifications/utils/sphinx/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-26 10:30:55.000000 dkist_fits_specifications-4.1.1rc1/dkist_fits_specifications/utils/sphinx/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8553 2024-02-26 10:30:55.000000 dkist_fits_specifications-4.1.1rc1/dkist_fits_specifications/utils/sphinx/spec_table.py
--rw-rw-rw-   0 root         (0) root         (0)      348 2024-02-26 10:31:13.000000 dkist_fits_specifications-4.1.1rc1/dkist_fits_specifications/version.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-26 10:31:13.432700 dkist_fits_specifications-4.1.1rc1/dkist_fits_specifications.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7309 2024-02-26 10:31:13.000000 dkist_fits_specifications-4.1.1rc1/dkist_fits_specifications.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3707 2024-02-26 10:31:13.000000 dkist_fits_specifications-4.1.1rc1/dkist_fits_specifications.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-02-26 10:31:13.000000 dkist_fits_specifications-4.1.1rc1/dkist_fits_specifications.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-02-26 10:31:13.000000 dkist_fits_specifications-4.1.1rc1/dkist_fits_specifications.egg-info/not-zip-safe
--rw-rw-rw-   0 root         (0) root         (0)      205 2024-02-26 10:31:13.000000 dkist_fits_specifications-4.1.1rc1/dkist_fits_specifications.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       26 2024-02-26 10:31:13.000000 dkist_fits_specifications-4.1.1rc1/dkist_fits_specifications.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-26 10:31:13.432700 dkist_fits_specifications-4.1.1rc1/docs/
--rw-rw-rw-   0 root         (0) root         (0)      634 2024-02-26 10:30:55.000000 dkist_fits_specifications-4.1.1rc1/docs/Makefile
--rw-rw-rw-   0 root         (0) root         (0)      872 2024-02-26 10:30:55.000000 dkist_fits_specifications-4.1.1rc1/docs/conf.py
--rw-rw-rw-   0 root         (0) root         (0)     1092 2024-02-26 10:30:55.000000 dkist_fits_specifications-4.1.1rc1/docs/index.rst
--rw-rw-rw-   0 root         (0) root         (0)     3424 2024-02-26 10:30:55.000000 dkist_fits_specifications-4.1.1rc1/docs/level_one.rst
--rw-rw-rw-   0 root         (0) root         (0)      760 2024-02-26 10:30:55.000000 dkist_fits_specifications-4.1.1rc1/docs/make.bat
--rw-rw-rw-   0 root         (0) root         (0)      382 2024-02-26 10:30:55.000000 dkist_fits_specifications-4.1.1rc1/docs/reference.rst
--rw-rw-rw-   0 root         (0) root         (0)      165 2024-02-26 10:30:55.000000 dkist_fits_specifications-4.1.1rc1/docs/release_history.rst
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-26 10:31:13.432700 dkist_fits_specifications-4.1.1rc1/docs/specs/
--rw-rw-rw-   0 root         (0) root         (0)     1463 2024-02-26 10:30:55.000000 dkist_fits_specifications-4.1.1rc1/docs/specs/spec-122.rst
--rw-rw-rw-   0 root         (0) root         (0)     2668 2024-02-26 10:30:55.000000 dkist_fits_specifications-4.1.1rc1/docs/specs/spec-214.rst
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-02-26 10:31:13.432700 dkist_fits_specifications-4.1.1rc1/licenses/
--rw-rw-rw-   0 root         (0) root         (0)     1480 2024-02-26 10:30:55.000000 dkist_fits_specifications-4.1.1rc1/licenses/LICENSE.rst
--rw-rw-rw-   0 root         (0) root         (0)      372 2024-02-26 10:30:55.000000 dkist_fits_specifications-4.1.1rc1/licenses/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     1659 2024-02-26 10:30:55.000000 dkist_fits_specifications-4.1.1rc1/licenses/TEMPLATE_LICENSE.rst
--rw-rw-rw-   0 root         (0) root         (0)     1437 2024-02-26 10:30:55.000000 dkist_fits_specifications-4.1.1rc1/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     2031 2024-02-26 10:31:13.432700 dkist_fits_specifications-4.1.1rc1/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)      612 2024-02-26 10:30:55.000000 dkist_fits_specifications-4.1.1rc1/setup.py
--rw-rw-rw-   0 root         (0) root         (0)     1327 2024-02-26 10:30:55.000000 dkist_fits_specifications-4.1.1rc1/tox.ini
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-16 16:07:22.358621 dkist_fits_specifications-4.2.0/
+-rw-rw-rw-   0 root         (0) root         (0)     3334 2024-05-16 16:07:05.000000 dkist_fits_specifications-4.2.0/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      676 2024-05-16 16:07:05.000000 dkist_fits_specifications-4.2.0/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      306 2024-05-16 16:07:05.000000 dkist_fits_specifications-4.2.0/.readthedocs.yml
+-rw-rw-rw-   0 root         (0) root         (0)    10489 2024-05-16 16:07:05.000000 dkist_fits_specifications-4.2.0/CHANGELOG.rst
+-rw-rw-rw-   0 root         (0) root         (0)       71 2024-05-16 16:07:05.000000 dkist_fits_specifications-4.2.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     7306 2024-05-16 16:07:22.358621 dkist_fits_specifications-4.2.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     6270 2024-05-16 16:07:05.000000 dkist_fits_specifications-4.2.0/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2285 2024-05-16 16:07:05.000000 dkist_fits_specifications-4.2.0/bitbucket-pipelines.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-16 16:07:22.346621 dkist_fits_specifications-4.2.0/changelog/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-16 16:07:05.000000 dkist_fits_specifications-4.2.0/changelog/.gitempty
+-rwxrwxrwx   0 root         (0) root         (0)      642 2024-05-16 16:07:05.000000 dkist_fits_specifications-4.2.0/check_changelog_updated.sh
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-16 16:07:22.346621 dkist_fits_specifications-4.2.0/dkist_fits_specifications/
+-rw-rw-rw-   0 root         (0) root         (0)      870 2024-05-16 16:07:05.000000 dkist_fits_specifications-4.2.0/dkist_fits_specifications/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-16 16:07:05.000000 dkist_fits_specifications-4.2.0/dkist_fits_specifications/py.typed
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-16 16:07:22.346621 dkist_fits_specifications-4.2.0/dkist_fits_specifications/spec122/
+-rw-rw-rw-   0 root         (0) root         (0)     6204 2024-05-16 16:07:05.000000 dkist_fits_specifications-4.2.0/dkist_fits_specifications/spec122/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-16 16:07:22.350621 dkist_fits_specifications-4.2.0/dkist_fits_specifications/spec122/schemas/
+-rw-rw-rw-   0 root         (0) root         (0)      792 2024-05-16 16:07:05.000000 dkist_fits_specifications-4.2.0/dkist_fits_specifications/spec122/schemas/ao.yml
+-rw-rw-rw-   0 root         (0) root         (0)     3049 2024-05-16 16:07:05.000000 dkist_fits_specifications-4.2.0/dkist_fits_specifications/spec122/schemas/camera.yml
+-rw-rw-rw-   0 root         (0) root         (0)      515 2024-05-16 16:07:05.000000 dkist_fits_specifications-4.2.0/dkist_fits_specifications/spec122/schemas/compression.yml
+-rw-rw-rw-   0 root         (0) root         (0)    13916 2024-05-16 16:07:05.000000 dkist_fits_specifications-4.2.0/dkist_fits_specifications/spec122/schemas/cryonirsp.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1572 2024-05-16 16:07:05.000000 dkist_fits_specifications-4.2.0/dkist_fits_specifications/spec122/schemas/dkist-dkist.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1088 2024-05-16 16:07:05.000000 dkist_fits_specifications-4.2.0/dkist_fits_specifications/spec122/schemas/dkist-id.yml
+-rw-rw-rw-   0 root         (0) root         (0)     5824 2024-05-16 16:07:05.000000 dkist_fits_specifications-4.2.0/dkist_fits_specifications/spec122/schemas/dlnirsp.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1709 2024-05-16 16:07:05.000000 dkist_fits_specifications-4.2.0/dkist_fits_specifications/spec122/schemas/fits.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1934 2024-05-16 16:07:05.000000 dkist_fits_specifications-4.2.0/dkist_fits_specifications/spec122/schemas/pac.yml
+-rw-rw-rw-   0 root         (0) root         (0)     2653 2024-05-16 16:07:05.000000 dkist_fits_specifications-4.2.0/dkist_fits_specifications/spec122/schemas/telescope.yml
+-rw-rw-rw-   0 root         (0) root         (0)      957 2024-05-16 16:07:05.000000 dkist_fits_specifications-4.2.0/dkist_fits_specifications/spec122/schemas/vbi.yml
+-rw-rw-rw-   0 root         (0) root         (0)     3579 2024-05-16 16:07:05.000000 dkist_fits_specifications-4.2.0/dkist_fits_specifications/spec122/schemas/visp.yml
+-rw-rw-rw-   0 root         (0) root         (0)     2326 2024-05-16 16:07:05.000000 dkist_fits_specifications-4.2.0/dkist_fits_specifications/spec122/schemas/vtf.yml
+-rw-rw-rw-   0 root         (0) root         (0)      776 2024-05-16 16:07:05.000000 dkist_fits_specifications-4.2.0/dkist_fits_specifications/spec122/schemas/wfc.yml
+-rw-rw-rw-   0 root         (0) root         (0)      703 2024-05-16 16:07:05.000000 dkist_fits_specifications-4.2.0/dkist_fits_specifications/spec122/schemas/ws.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-16 16:07:22.350621 dkist_fits_specifications-4.2.0/dkist_fits_specifications/spec214/
+-rw-rw-rw-   0 root         (0) root         (0)    13981 2024-05-16 16:07:05.000000 dkist_fits_specifications-4.2.0/dkist_fits_specifications/spec214/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3421 2024-05-16 16:07:05.000000 dkist_fits_specifications-4.2.0/dkist_fits_specifications/spec214/level0.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-16 16:07:22.354621 dkist_fits_specifications-4.2.0/dkist_fits_specifications/spec214/schemas/
+-rw-rw-rw-   0 root         (0) root         (0)     1973 2024-05-16 16:07:05.000000 dkist_fits_specifications-4.2.0/dkist_fits_specifications/spec214/schemas/ao.yml
+-rw-rw-rw-   0 root         (0) root         (0)     5886 2024-05-16 16:07:05.000000 dkist_fits_specifications-4.2.0/dkist_fits_specifications/spec214/schemas/camera.yml
+-rw-rw-rw-   0 root         (0) root         (0)     6424 2024-05-16 16:07:05.000000 dkist_fits_specifications-4.2.0/dkist_fits_specifications/spec214/schemas/compression.yml
+-rw-rw-rw-   0 root         (0) root         (0)    13579 2024-05-16 16:07:05.000000 dkist_fits_specifications-4.2.0/dkist_fits_specifications/spec214/schemas/cryonirsp.yml
+-rw-rw-rw-   0 root         (0) root         (0)     4107 2024-05-16 16:07:05.000000 dkist_fits_specifications-4.2.0/dkist_fits_specifications/spec214/schemas/datacenter.yml
+-rw-rw-rw-   0 root         (0) root         (0)     4144 2024-05-16 16:07:05.000000 dkist_fits_specifications-4.2.0/dkist_fits_specifications/spec214/schemas/dataset.yml
+-rw-rw-rw-   0 root         (0) root         (0)     2429 2024-05-16 16:07:05.000000 dkist_fits_specifications-4.2.0/dkist_fits_specifications/spec214/schemas/dkist-id.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1805 2024-05-16 16:07:05.000000 dkist_fits_specifications-4.2.0/dkist_fits_specifications/spec214/schemas/dkist-op.yml
+-rw-rw-rw-   0 root         (0) root         (0)     9112 2024-05-16 16:07:05.000000 dkist_fits_specifications-4.2.0/dkist_fits_specifications/spec214/schemas/dlnirsp.yml
+-rw-rw-rw-   0 root         (0) root         (0)     7249 2024-05-16 16:07:05.000000 dkist_fits_specifications-4.2.0/dkist_fits_specifications/spec214/schemas/fits.yml
+-rw-rw-rw-   0 root         (0) root         (0)     2381 2024-05-16 16:07:05.000000 dkist_fits_specifications-4.2.0/dkist_fits_specifications/spec214/schemas/pac.yml
+-rw-rw-rw-   0 root         (0) root         (0)      778 2024-05-16 16:07:05.000000 dkist_fits_specifications-4.2.0/dkist_fits_specifications/spec214/schemas/stats.yml
+-rw-rw-rw-   0 root         (0) root         (0)     7346 2024-05-16 16:07:05.000000 dkist_fits_specifications-4.2.0/dkist_fits_specifications/spec214/schemas/telescope.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1907 2024-05-16 16:07:05.000000 dkist_fits_specifications-4.2.0/dkist_fits_specifications/spec214/schemas/vbi.yml
+-rw-rw-rw-   0 root         (0) root         (0)     2939 2024-05-16 16:07:05.000000 dkist_fits_specifications-4.2.0/dkist_fits_specifications/spec214/schemas/visp.yml
+-rw-rw-rw-   0 root         (0) root         (0)     3660 2024-05-16 16:07:05.000000 dkist_fits_specifications-4.2.0/dkist_fits_specifications/spec214/schemas/vtf.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1483 2024-05-16 16:07:05.000000 dkist_fits_specifications-4.2.0/dkist_fits_specifications/spec214/schemas/wfc.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1310 2024-05-16 16:07:05.000000 dkist_fits_specifications-4.2.0/dkist_fits_specifications/spec214/schemas/ws.yml
+-rw-rw-rw-   0 root         (0) root         (0)     1090 2024-05-16 16:07:05.000000 dkist_fits_specifications-4.2.0/dkist_fits_specifications/spec214/spec214_full_schema.yml
+-rw-rw-rw-   0 root         (0) root         (0)      648 2024-05-16 16:07:05.000000 dkist_fits_specifications-4.2.0/dkist_fits_specifications/spec_validation_schema.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-16 16:07:22.354621 dkist_fits_specifications-4.2.0/dkist_fits_specifications/tests/
+-rw-rw-rw-   0 root         (0) root         (0)       44 2024-05-16 16:07:05.000000 dkist_fits_specifications-4.2.0/dkist_fits_specifications/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2475 2024-05-16 16:07:05.000000 dkist_fits_specifications-4.2.0/dkist_fits_specifications/tests/test_122.py
+-rw-rw-rw-   0 root         (0) root         (0)     8645 2024-05-16 16:07:05.000000 dkist_fits_specifications-4.2.0/dkist_fits_specifications/tests/test_214.py
+-rw-rw-rw-   0 root         (0) root         (0)     2842 2024-05-16 16:07:05.000000 dkist_fits_specifications-4.2.0/dkist_fits_specifications/tests/test_expansions.py
+-rw-rw-rw-   0 root         (0) root         (0)     1272 2024-05-16 16:07:05.000000 dkist_fits_specifications-4.2.0/dkist_fits_specifications/tests/test_formatter.py
+-rw-rw-rw-   0 root         (0) root         (0)      744 2024-05-16 16:07:05.000000 dkist_fits_specifications-4.2.0/dkist_fits_specifications/tests/test_level0_214.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-16 16:07:22.354621 dkist_fits_specifications-4.2.0/dkist_fits_specifications/utils/
+-rw-rw-rw-   0 root         (0) root         (0)       55 2024-05-16 16:07:05.000000 dkist_fits_specifications-4.2.0/dkist_fits_specifications/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3374 2024-05-16 16:07:05.000000 dkist_fits_specifications-4.2.0/dkist_fits_specifications/utils/formatter.py
+-rw-rw-rw-   0 root         (0) root         (0)     1222 2024-05-16 16:07:05.000000 dkist_fits_specifications-4.2.0/dkist_fits_specifications/utils/frozendict.py
+-rw-rw-rw-   0 root         (0) root         (0)     2843 2024-05-16 16:07:05.000000 dkist_fits_specifications-4.2.0/dkist_fits_specifications/utils/spec.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-16 16:07:22.354621 dkist_fits_specifications-4.2.0/dkist_fits_specifications/utils/spec_processors/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-16 16:07:05.000000 dkist_fits_specifications-4.2.0/dkist_fits_specifications/utils/spec_processors/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2489 2024-05-16 16:07:05.000000 dkist_fits_specifications-4.2.0/dkist_fits_specifications/utils/spec_processors/expansion.py
+-rw-rw-rw-   0 root         (0) root         (0)      933 2024-05-16 16:07:05.000000 dkist_fits_specifications-4.2.0/dkist_fits_specifications/utils/spec_processors/instrument_requiredness.py
+-rw-rw-rw-   0 root         (0) root         (0)     4401 2024-05-16 16:07:05.000000 dkist_fits_specifications-4.2.0/dkist_fits_specifications/utils/spec_processors/polarimetric_requiredness.py
+-rw-rw-rw-   0 root         (0) root         (0)     1565 2024-05-16 16:07:05.000000 dkist_fits_specifications-4.2.0/dkist_fits_specifications/utils/spec_processors/requiredness_base.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-16 16:07:22.354621 dkist_fits_specifications-4.2.0/dkist_fits_specifications/utils/sphinx/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-16 16:07:05.000000 dkist_fits_specifications-4.2.0/dkist_fits_specifications/utils/sphinx/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8553 2024-05-16 16:07:05.000000 dkist_fits_specifications-4.2.0/dkist_fits_specifications/utils/sphinx/spec_table.py
+-rw-rw-rw-   0 root         (0) root         (0)      345 2024-05-16 16:07:22.000000 dkist_fits_specifications-4.2.0/dkist_fits_specifications/version.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-16 16:07:22.358621 dkist_fits_specifications-4.2.0/dkist_fits_specifications.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7306 2024-05-16 16:07:22.000000 dkist_fits_specifications-4.2.0/dkist_fits_specifications.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3733 2024-05-16 16:07:22.000000 dkist_fits_specifications-4.2.0/dkist_fits_specifications.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-05-16 16:07:22.000000 dkist_fits_specifications-4.2.0/dkist_fits_specifications.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-05-16 16:07:18.000000 dkist_fits_specifications-4.2.0/dkist_fits_specifications.egg-info/not-zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)      205 2024-05-16 16:07:22.000000 dkist_fits_specifications-4.2.0/dkist_fits_specifications.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       26 2024-05-16 16:07:22.000000 dkist_fits_specifications-4.2.0/dkist_fits_specifications.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-16 16:07:22.358621 dkist_fits_specifications-4.2.0/docs/
+-rw-rw-rw-   0 root         (0) root         (0)      634 2024-05-16 16:07:05.000000 dkist_fits_specifications-4.2.0/docs/Makefile
+-rw-rw-rw-   0 root         (0) root         (0)      872 2024-05-16 16:07:05.000000 dkist_fits_specifications-4.2.0/docs/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)     1092 2024-05-16 16:07:05.000000 dkist_fits_specifications-4.2.0/docs/index.rst
+-rw-rw-rw-   0 root         (0) root         (0)     3424 2024-05-16 16:07:05.000000 dkist_fits_specifications-4.2.0/docs/level_one.rst
+-rw-rw-rw-   0 root         (0) root         (0)      760 2024-05-16 16:07:05.000000 dkist_fits_specifications-4.2.0/docs/make.bat
+-rw-rw-rw-   0 root         (0) root         (0)      382 2024-05-16 16:07:05.000000 dkist_fits_specifications-4.2.0/docs/reference.rst
+-rw-rw-rw-   0 root         (0) root         (0)      165 2024-05-16 16:07:05.000000 dkist_fits_specifications-4.2.0/docs/release_history.rst
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-16 16:07:22.358621 dkist_fits_specifications-4.2.0/docs/specs/
+-rw-rw-rw-   0 root         (0) root         (0)     1463 2024-05-16 16:07:05.000000 dkist_fits_specifications-4.2.0/docs/specs/spec-122.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2668 2024-05-16 16:07:05.000000 dkist_fits_specifications-4.2.0/docs/specs/spec-214.rst
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-16 16:07:22.358621 dkist_fits_specifications-4.2.0/licenses/
+-rw-rw-rw-   0 root         (0) root         (0)     1480 2024-05-16 16:07:05.000000 dkist_fits_specifications-4.2.0/licenses/LICENSE.rst
+-rw-rw-rw-   0 root         (0) root         (0)      372 2024-05-16 16:07:05.000000 dkist_fits_specifications-4.2.0/licenses/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1659 2024-05-16 16:07:05.000000 dkist_fits_specifications-4.2.0/licenses/TEMPLATE_LICENSE.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1437 2024-05-16 16:07:05.000000 dkist_fits_specifications-4.2.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     2031 2024-05-16 16:07:22.358621 dkist_fits_specifications-4.2.0/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)      612 2024-05-16 16:07:05.000000 dkist_fits_specifications-4.2.0/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)     1327 2024-05-16 16:07:05.000000 dkist_fits_specifications-4.2.0/tox.ini
```

### Comparing `dkist_fits_specifications-4.1.1rc1/.gitignore` & `dkist_fits_specifications-4.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-4.1.1rc1/.pre-commit-config.yaml` & `dkist_fits_specifications-4.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-4.1.1rc1/CHANGELOG.rst` & `dkist_fits_specifications-4.2.0/CHANGELOG.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,29 @@
+v4.2.0 (2024-05-16)
+===================
+
+Backwards Compatible Changes to the Specification
+-------------------------------------------------
+
+- Updated 214 DL-NIRSP Spec to match the information provided in the 122 DL-NIRSP Spec. (`#49 <https://bitbucket.org/dkistdc/dkist-fits-specifications/pull-requests/49>`__)
+- Revision J:
+  Added DKIST013 to capture status of Lyot stop. Added CAM__043 to indicate
+  whether the frame data was simulated or not. Modified accepted range of values for
+  DLN__026 to allow for the MISI upgrade. (`#49 <https://bitbucket.org/dkistdc/dkist-fits-specifications/pull-requests/49>`__)
+
+
+v4.1.1 (2024-02-26)
+===================
+
+Bug Fixes to the Python API
+---------------------------
+
+- Correctly handle a header which has DEAXES=0. (`#48 <https://bitbucket.org/dkistdc/dkist-fits-specifications/pull-requests/48>`__)
+
+
 v4.1.0 (2024-01-31)
 ===================
 
 Backwards Compatible Changes to the Specification
 -------------------------------------------------
 
 - Add new keyword `SOLARRAD` which contains the value of the solar radius at the time of observation, in arcseconds. (`#44 <https://bitbucket.org/dkistdc/dkist-fits-specifications/pull-requests/44>`__)
```

### Comparing `dkist_fits_specifications-4.1.1rc1/PKG-INFO` & `dkist_fits_specifications-4.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist_fits_specifications
-Version: 4.1.1rc1
+Version: 4.2.0
 Summary: Machine readable FITS specifications for DKIST data.
 Home-page: https://bitbucket.org/dkistdc/dkist-fits-specifications/src/main/
 Author: AURA/NSO
 Author-email: stuart@cadair.com
 License: BSD 3-Clause
 Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
```

### Comparing `dkist_fits_specifications-4.1.1rc1/README.rst` & `dkist_fits_specifications-4.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-4.1.1rc1/bitbucket-pipelines.yml` & `dkist_fits_specifications-4.2.0/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-4.1.1rc1/check_changelog_updated.sh` & `dkist_fits_specifications-4.2.0/check_changelog_updated.sh`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-4.1.1rc1/dkist_fits_specifications/__init__.py` & `dkist_fits_specifications-4.2.0/dkist_fits_specifications/__init__.py`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-4.1.1rc1/dkist_fits_specifications/spec122/__init__.py` & `dkist_fits_specifications-4.2.0/dkist_fits_specifications/spec122/__init__.py`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-4.1.1rc1/dkist_fits_specifications/spec122/schemas/ao.yml` & `dkist_fits_specifications-4.2.0/dkist_fits_specifications/spec122/schemas/ao.yml`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 spec122:
   section: ao
-  expand: False
+  expand: false
 ---
 AO___001:
   required: false
   comment: '[m] HOAOFriedParameter'
   type: float
 AO___002:
   required: false
   comment: HOAOLockStatus
   type: bool
   values:
-    - True
-    - False
+    - true
+    - false
 AO___003:
   required: false
   comment: '[arcs] HOAOLockOffPointingX'
   type: float
 AO___004:
   required: false
   comment: '[arcs] HOAOLockOffPointingY'
```

### Comparing `dkist_fits_specifications-4.1.1rc1/dkist_fits_specifications/spec122/schemas/camera.yml` & `dkist_fits_specifications-4.2.0/dkist_fits_specifications/spec122/schemas/camera.yml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 spec122:
   section: camera
-  expand: False
+  expand: false
 ---
 CAM__001:
   required: true
   comment: CameraUniqueID
   type: str
 CAM__002:
   required: true
@@ -166,7 +166,13 @@
   required: false
   comment: '[px] HWROI2SizeY'
   type: int
 CAM__042:
   required: false
   comment: FPABitsPerPixel
   type: int
+CAM__043:
+  required: false
+  comment: SimulatedFrameIndicator
+  type: bool
+  values:
+    - false
```

### Comparing `dkist_fits_specifications-4.1.1rc1/dkist_fits_specifications/spec122/schemas/compression.yml` & `dkist_fits_specifications-4.2.0/dkist_fits_specifications/spec122/schemas/compression.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 spec122:
   section: compression
-  expand: False
+  expand: false
 ---
 ZIMAGE:
   required: false
   type: bool
   values:
-    - True
+    - true
 ZCMPTYPE:
   required: false
   type: str
   values:
     - 'RICE_1'
     - 'GZIP_1'
     - 'GZIP_2'
@@ -31,11 +31,11 @@
   required: false
   type: int
   values:
     - 3
 ZNAXIS<n>:
   required: false
   type: int
-  expand: True
+  expand: true
 ZBLANK:
   required: false
   type: int
```

### Comparing `dkist_fits_specifications-4.1.1rc1/dkist_fits_specifications/spec122/schemas/cryonirsp.yml` & `dkist_fits_specifications-4.2.0/dkist_fits_specifications/spec122/schemas/cryonirsp.yml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 spec122:
   section: cryonirsp
-  expand: False
+  expand: false
 ---
 CRSP_001:
   required: false
   instrument_required: CRYO-NIRSP
   comment: ArmID
   type: str
   values:
```

### Comparing `dkist_fits_specifications-4.1.1rc1/dkist_fits_specifications/spec122/schemas/dkist-dkist.yml` & `dkist_fits_specifications-4.2.0/dkist_fits_specifications/spec122/schemas/dkist-dkist.yml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 spec122:
   section: dkist-dkist
-  expand: False
+  expand: false
 ---
 DKIST001:
   required: true
   comment: OCSControl
   type: str
   values:
     - "Auto"
@@ -62,16 +62,16 @@
     - 'Bad'
     - 'Unknown'
 DKIST007:
   required: true
   comment: EngineeringDataFlag
   type: bool
   values:
-    - True
-    - False
+    - true
+    - false
 DKIST008:
   required: true
   comment: DSPSNumberOfRepeats
   type: int
 DKIST009:
   required: true
   comment: DSPSRepeatNumber
@@ -86,7 +86,14 @@
   type: str
   format: isot
 DKIST012:
   required: false
   comment: InstrumentProgramEndTime
   type: str
   format: isot
+DKIST013:
+  required: false
+  comment: LyotStopInBeamStatus
+  type: bool
+  values:
+    - true
+    - false
```

### Comparing `dkist_fits_specifications-4.1.1rc1/dkist_fits_specifications/spec122/schemas/dkist-id.yml` & `dkist_fits_specifications-4.2.0/dkist_fits_specifications/spec122/schemas/dkist-id.yml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 spec122:
   section: dkist-id
-  expand: False
+  expand: false
 ---
 ID___001:
   required: true
   comment: DKISTFITSHeaderVersion
   type: str
   example_values:
     - 'Data Model (SPEC-0122) Revision F'
```

### Comparing `dkist_fits_specifications-4.1.1rc1/dkist_fits_specifications/spec122/schemas/dlnirsp.yml` & `dkist_fits_specifications-4.2.0/dkist_fits_specifications/spec122/schemas/dlnirsp.yml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 spec122:
   section: dlnirsp
-  expand: False
+  expand: false
 ---
 DLN__001:
   required: false
   instrument_required: DL-NIRSP
   comment: ArmID
   type: str
   values:
@@ -150,14 +150,16 @@
   required: false
   instrument_required: DL-NIRSP
   comment: IFUID
   type: str
   values:
     - 'IFU-36'
     - 'IFU-72'
+    - 'MISI-36'
+    - 'MISI-116'
 DLN__027:
   required: false
   instrument_required: DL-NIRSP
   comment: '[mm] IFUPosition'
   type: float
 DLN__028:
   required: false
@@ -167,15 +169,14 @@
   values:
     - 'Single'
     - 'All'
     - 'None'
     - 'Invalid'
 DLN__029:
   required: false
-  instrument_required: DL-NIRSP
   comment: SlitSelection
   type: int
   values:
     - 0
     - 1
     - 2
     - 3
@@ -184,29 +185,28 @@
   required: false
   instrument_required: DL-NIRSP
   comment: '[mm] SlitPosition'
   type: float
 DLN__031:
   required: false
   instrument_required: DL-NIRSP
-  comment: 'MosaicNumRepeat'
+  comment: MosaicNumRepeat
   type: int
 DLN__032:
   required: false
   instrument_required: DL-NIRSP
-  comment: 'CurrentMosaicRepeat'
+  comment: CurrentMosaicRepeat
   type: int
 DLN__033:
   required: false
   instrument_required: DL-NIRSP
-  comment: 'MosaicScanPattern'
+  comment: MosaicScanPattern
   type: str
 DLN__034:
   required: false
-  instrument_required: DL-NIRSP
   comment: NumberOfSpatialStepsX
   type: int
 DLN__035:
   required: false
   instrument_required: DL-NIRSP
   comment: '[urad] StepCenterPositionX'
   type: float
@@ -238,26 +238,35 @@
   comment: CurrentSpatialStepY
   type: int
 DLN__042:
   required: false
   instrument_required: DL-NIRSP
   comment: DitherMode
   type: bool
+  values:
+    - true
+    - false
 DLN__043:
   required: false
+  instrument_required: DL-NIRSP
   comment: '[urad] DitherOffsetX'
   type: float
 DLN__044:
   required: false
+  instrument_required: DL-NIRSP
   comment: '[urad] DitherOffsetY'
   type: float
 DLN__045:
   required: false
+  instrument_required: DL-NIRSP
   comment: DitherCurrentStep
   type: bool
+  values:
+    - true
+    - false
 DLN__046:
   required: false
   comment: CameraSamplingMode
   type: str
   values:
     - 'SubFrame'
     - 'UpTheRamp'
@@ -291,9 +300,10 @@
   type: float
 DLN__054:
   required: false
   comment: CameraFilterID
   type: str
 DLN__055:
   required: false
+  instrument_required: DL-NIRSP
   comment: ModulatorReferenceT0
   type: str
```

### Comparing `dkist_fits_specifications-4.1.1rc1/dkist_fits_specifications/spec122/schemas/fits.yml` & `dkist_fits_specifications-4.2.0/dkist_fits_specifications/spec122/schemas/fits.yml`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 spec122:
   section: fits
-  expand: False
+  expand: false
 ---
 SIMPLE:
   required: false
   type: bool
   values:
-    - True
+    - true
 BITPIX:
   required: true
   type: int
   values:
     - 8
     - 16
     - 32
@@ -21,15 +21,15 @@
   required: true
   type: int
   values:
     - 3
 NAXIS<n>:
   required: true
   type: int
-  expand: True
+  expand: true
 BUNIT:
   required: true
   type: str
   format: 'unit'
 BZERO:
   required: false
   type: float
```

### Comparing `dkist_fits_specifications-4.1.1rc1/dkist_fits_specifications/spec122/schemas/pac.yml` & `dkist_fits_specifications-4.2.0/dkist_fits_specifications/spec122/schemas/pac.yml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 spec122:
   section: pac
-  expand: False
+  expand: false
 ---
 PAC__001:
   required: true
   comment: "Upper GOS shutter"
   type: str
   values:
     - 'open'
```

### Comparing `dkist_fits_specifications-4.1.1rc1/dkist_fits_specifications/spec122/schemas/telescope.yml` & `dkist_fits_specifications-4.2.0/dkist_fits_specifications/spec122/schemas/telescope.yml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 spec122:
   section: telescope
-  expand: False
+  expand: false
 ---
 WCSAXES:
   required: true
   type: int
   values:
     - 3
 WCSAXESA:
@@ -23,88 +23,88 @@
   type: str
   values:
     - 'Helioprojective-cartesian'
     - 'Equatorial equinox J2000'
 CRPIX<n>:
   required: true
   type: float
-  expand: True
+  expand: true
 CRPIX<n>A:
   required: false
   type: float
-  expand: True
+  expand: true
 CRDATE<n>:
   required: false
   type: str
   format: isot
-  expand: True
+  expand: true
 CRDATE<n>A:
   required: false
   type: str
   format: isot
-  expand: True
+  expand: true
 CRVAL<n>:
   required: true
   type: float
-  expand: True
+  expand: true
 CRVAL<n>A:
   required: false
   type: float
-  expand: True
+  expand: true
 CDELT<n>:
   required: true
   type: float
-  expand: True
+  expand: true
 CDELT<n>A:
   required: false
   type: float
-  expand: True
+  expand: true
 CUNIT<n>:
   required: true
   type: str
-  expand: True
+  expand: true
   format: 'unit'
 CUNIT<n>A:
   required: false
   type: str
-  expand: True
+  expand: true
   format: 'unit'
 CTYPE<n>:
   required: true
   type: str
-  expand: True
+  expand: true
 CTYPE<n>A:
   required: false
   type: str
-  expand: True
+  expand: true
 PC<i>_<j>:
   required: true
   type: float
-  expand: True
+  expand: true
 PC<i>_<j>A:
   required: false
   type: float
-  expand: True
+  expand: true
 #not currently in use
 #PVi_m:
 #  required: true
 #  type: float
-#  expand: True
+#  expand: true
 #PVi_mA:
 #  required: false
 # type: float
-#  expand: True
+#  expand: true
 #PSi_m:
 #  required: true
 #  type: float
-#  expand: True
+#  expand: true
 #PSi_mA:
 #  required: false
 #  type: float
-#  expand: True
+#  expand: true
 LONPOLE:
   required: false
   type: float
 LONPOLEA:
   required: false
   type: float
 LATPOLE:
@@ -154,9 +154,9 @@
     - 'coude and tel. azimuth'
     - 'fixed coude table angle'
 WCSVALID:
   required: false
   comment: WCSValidityIndicator
   type: bool
   values:
-    - True
-    - False
+    - true
+    - false
```

### Comparing `dkist_fits_specifications-4.1.1rc1/dkist_fits_specifications/spec122/schemas/vbi.yml` & `dkist_fits_specifications-4.2.0/dkist_fits_specifications/spec122/schemas/vbi.yml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 spec122:
   section: vbi
   instrument_required: VBI
-  expand: False
+  expand: false
 ---
 VBI__001:
   required: false
   comment: '[nm] InterferenceFilterFWHM'
   type: float
 VBI__002:
   required: false
```

### Comparing `dkist_fits_specifications-4.1.1rc1/dkist_fits_specifications/spec122/schemas/visp.yml` & `dkist_fits_specifications-4.2.0/dkist_fits_specifications/spec122/schemas/visp.yml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 spec122:
   section: visp
-  expand: False
+  expand: false
 ---
 VISP_001:
   required: false
   instrument_required: VISP
   comment: ArmID
   type: int
   values:
```

### Comparing `dkist_fits_specifications-4.1.1rc1/dkist_fits_specifications/spec122/schemas/vtf.yml` & `dkist_fits_specifications-4.2.0/dkist_fits_specifications/spec122/schemas/vtf.yml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 spec122:
   section: vtf
-  expand: False
+  expand: false
   instrument_required: VTF
 ---
 VTF__001:
   required: false
   comment: InstrumentMode
   type: str
   values:
```

### Comparing `dkist_fits_specifications-4.1.1rc1/dkist_fits_specifications/spec122/schemas/wfc.yml` & `dkist_fits_specifications-4.2.0/dkist_fits_specifications/spec122/schemas/wfc.yml`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 spec122:
   section: wfc
-  expand: False
+  expand: false
 ---
 WFC__001:
   required: false
   comment: '[nm] FilterFWHM'
   type: float
 WFC__002:
   required: false
   comment: HOAOFrameLockStatus
   type: bool
   example_values:
-    - True
-    - False
+    - true
+    - false
 WFC__003:
   required: false
   comment: HOAOReconstructionMatrixID
   type: str
 WFC__004:
   required: false
   comment: HOAOCtrlLoopPValue
@@ -30,16 +30,16 @@
   comment: '[Hz] HOAOWFSFrameRate'
   type: int
 WFC__007:
   required: false
   comment: TTFrameLockStatus
   type: bool
   example_values:
-    - True
-    - False
+    - true
+    - false
 WFC__008:
   required: false
   comment: TTCtrlLoopPValue
   type: float
 WFC__009:
   required: false
   comment: TTCtrlLoopIValue
```

### Comparing `dkist_fits_specifications-4.1.1rc1/dkist_fits_specifications/spec122/schemas/ws.yml` & `dkist_fits_specifications-4.2.0/dkist_fits_specifications/spec122/schemas/ws.yml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 spec122:
   section: ws
-  expand: False
+  expand: false
 ---
 WS___001:
   required: true
   comment: WeathSource
   type: str
 WS___002:
   required: true
```

### Comparing `dkist_fits_specifications-4.1.1rc1/dkist_fits_specifications/spec214/__init__.py` & `dkist_fits_specifications-4.2.0/dkist_fits_specifications/spec214/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 The 214 schemas are more complex than the 122 ones, as they have more uses, and
 are tightly coupled to the 122 schemas.
 There are three main variants to the 214 schemas:
 
 * The **raw schemas** as saved in the yaml files. Each 214 raw schema can
   reference a 122 schema, from which it can copy the 'type', 'default_value',
   'values', and 'format' fields for keys. A key can be marked as ``copy:
-  True`` to indicate that the schema **and** the value should be the same in
+  true`` to indicate that the schema **and** the value should be the same in
   214 as 122, or it can be marked as ``copy: 'schema'`` to indicate that just
   the schema is the same for that key, but the value will be regenerated.
 * The **full schemas**. The full schemas are processed to merge the values in
   the schema header, and any values from the corresponding 122 schema. These
   schemas contain a lot more fields than the 122 schemas do, as these schemas
   are also used to generate documentation describing the specification.
 * The **validation schema**. These schemas (returned by `.load_processed_spec214`) are
```

### Comparing `dkist_fits_specifications-4.1.1rc1/dkist_fits_specifications/spec214/level0.py` & `dkist_fits_specifications-4.2.0/dkist_fits_specifications/spec214/level0.py`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-4.1.1rc1/dkist_fits_specifications/spec214/schemas/ao.yml` & `dkist_fits_specifications-4.2.0/dkist_fits_specifications/spec214/schemas/ao.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 spec214:
   section_122: ao
-  copy: True
+  copy: true
   required: false
-  expand: False
-  expected: True
+  expand: false
+  expected: true
   title: Adaptive Optics
   summary: Keys describing aspects of the adaptive optics system.
 ---
 ATMOS_R0:
   rename: "AO___001"
   description: "Value of Fried's parameter at start of data acquisition."
   units: m
 AO_LOCK:
   rename: "AO___002"
   description: "Lock status of HOAO during data acquisition.
-                False: HOAO was unlocked for some duration of data acquisition
-                True: HOAO was locked for the complete duration of data acquisition"
+                false: HOAO was unlocked for some duration of data acquisition
+                true: HOAO was locked for the complete duration of data acquisition"
   units: null
 AO_LOCKX:
   rename: "AO___003"
   description: "Current Lockpoint offpointing in X of the HOAO WFS in arcseconds relative to WFC Context Viewer defined telescope boresight"
   units: arcsec
 AO_LOCKY:
   rename: "AO___004"
```

### Comparing `dkist_fits_specifications-4.1.1rc1/dkist_fits_specifications/spec214/schemas/camera.yml` & `dkist_fits_specifications-4.2.0/dkist_fits_specifications/spec214/schemas/camera.yml`

 * *Files 12% similar despite different names*

```diff
@@ -1,108 +1,108 @@
 spec214:
   section_122: camera
-  copy: True
+  copy: true
   required: false
   units: null
-  expand: False
+  expand: false
   title: Camera
   summary: Keys describing modes and operation of the camera(s) used.
 ---
 CAM_ID:
   rename: "CAM__001"
   description: "Unique ID of camera used to acquire the data"
-  required: True
+  required: true
 CAMERA:
   rename: "CAM__002"
-  required: True
+  required: true
   description: "Human readable name of camera used to acquire the data"
 BITDEPTH:
   rename: "CAM__003"
   description: "Number of bits used internally by the camera sensor to digitize the measured photo-electrons"
-  required: True
+  required: true
 XPOSURE:
   rename: "CAM__004"
-  required: True
+  required: true
   description: "Total duration of exposure to photons, in milliseconds, that resulted in this FPA"
   units: ms
 TEXPOSUR:
   rename: "CAM__005"
-  required: True
+  required: true
   description: "Duration of photosensitive sensor exposure to photons, in milliseconds, per single sensor read-out."
   units: ms
-  expected: True
+  expected: true
 CAM_FPS:
   rename: "CAM__006"
   description: "Camera exposure rate"
-  required: True
+  required: true
   units: Hz
 CHIPDIM1:
   rename: "CAM__007"
   description: "Number of photosensitive pixels on the camera sensor, in X direction"
-  required: True
+  required: true
   units: pix
 CHIPDIM2:
   rename: "CAM__008"
   description: "Number of photosensitive pixels on the camera sensor, in Y direction"
-  required: True
+  required: true
   units: pix
 HWBIN1:
   rename: "CAM__009"
   description: "Value describing the binning performed in hardware in pixels, in X direction
                 Equals 1 if disabled"
   units: pix
   expand: true
-  required: True
+  required: true
 HWBIN2:
   rename: "CAM__010"
   description: "Value describing the binning performed in hardware in pixels, in Y direction
                 Equals 1 if disabled"
   units: pix
-  required: True
+  required: true
 SWBIN1:
   rename: "CAM__011"
   description: "Binning performed by software in pixels, after hardware binning, in pixels, in X direction
                 Equals 1 if disabled"
   units: pix
-  required: True
+  required: true
 SWBIN2:
   rename: "CAM__012"
   description: "Binning performed by software in pixels, after hardware binning, in pixels, in Y direction
                 Equals 1 if disabled"
   units: pix
-  required: True
+  required: true
 NSUMEXP:
   rename: "CAM__014"
   required: true
   description: "Number of raw frames that contributed to the FPA"
 SWNROI:
   rename: "CAM__016"
   description: "Number of Software Regions of Interest set
                 Default: 1, value ≥ 1"
-  required: True
+  required: true
 SWROI1OX:
   rename: "CAM__017"
   description: "Software Region Of Interest 1 X - Origin coordinate in pixels"
   units: pix
-  required: True
+  required: true
 SWROI1OY:
   rename: "CAM__018"
   description: "Software Region Of Interest 1 Y - Origin coordinate in pixels"
   units: pix
-  required: True
+  required: true
 SWROI1SX:
   rename: "CAM__019"
   description: "Software Region Of Interest 1 X - Size in pixels"
   units: pix
-  required: True
+  required: true
 SWROI1SY:
   rename: "CAM__020"
   description: "Software Region Of Interest 1 Y - Size in pixels"
   units: pix
-  required: True
+  required: true
 SWROI2OX:
   rename: "CAM__021"
   description: "Software Region Of Interest 2 X - Origin coordinate in pixels"
   units: pix
 SWROI2OY:
   rename: "CAM__022"
   description: "Software Region Of Interest 2 Y - Origin coordinate in pixels"
@@ -147,35 +147,35 @@
   rename: "CAM__032"
   description: "Software Region Of Interest 4 Y - Size in pixels"
   units: pix
 HWNROI:
   rename: "CAM__033"
   description: "Number of Hardware Regions of Interest set
                 Default: 1, value ≥ 1"
-  required: True
+  required: true
 HWROI1OX:
   rename: "CAM__034"
   description: "Hardware Region Of Interest 1 X - Origin coordinate in pixels"
   units: pix
-  required: True
+  required: true
 HWROI1OY:
   rename: "CAM__035"
   description: "Hardware Region Of Interest 1 Y - Origin coordinate in pixels"
   units: pix
-  required: True
+  required: true
 HWROI1SX:
   rename: "CAM__036"
   description: "Hardware Region Of Interest 1 X - Size in pixels"
   units: pix
-  required: True
+  required: true
 HWROI1SY:
   rename: "CAM__037"
   description: "Hardware Region Of Interest 1 Y - Size in pixels"
   units: pix
-  required: True
+  required: true
 HWROI2OX:
   rename: "CAM__038"
   description: "Hardware Region Of Interest 2 X - Origin coordinate in pixels"
   units: pix
 HWROI2OY:
   rename: "CAM__039"
   description: "Hardware Region Of Interest 2 Y - Origin coordinate in pixels"
```

### Comparing `dkist_fits_specifications-4.1.1rc1/dkist_fits_specifications/spec214/schemas/compression.yml` & `dkist_fits_specifications-4.2.0/dkist_fits_specifications/spec214/schemas/compression.yml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 spec214:
   section_122: compression
-  copy: False
+  copy: false
   required: false
   units: null
-  expand: False
+  expand: false
   fitsreference: "10.1: Tiled image compression"
   title: Compression
   summary: Keys added when the data is RICE compressed as described in FITS 4.0 Section 10.
   long_description: |
     This table contains the keys describing tiled image compression.
 
     Also included in this table are the keys used to describe a FITS binary table, as these are only used in DKIST data when using tiled image compression.
@@ -37,22 +37,22 @@
 ZNAXIS:
   description: "Mandatory keyword. Value depends on keyword position in file, i.e. whether the keyword is located in the primary HDU, or an extension HDU.
    Generally, the value field shall contain a non-negative integer no greater than 999 representing the number of axes in the associated data array. A value of zero signifies that no data follow the header in the HDU."
   copy: true
 ZNAXIS<n>:
   description: "ZNAXISn keywords. The ZNAXISn keywords must be present for all values n = 1, ..., ZNAXIS, in increasing order of n, and for no other values of n. The value field of this indexed keyword shall contain a non-negative integer representing the number of elements along axis n of a data array. A value of zero for any of the ZNAXISn signifies that no data follow the header in the HDU (however, the random groups structure has ZNAXIS1 = 0, but will have data following the header if the other ZNAXISn keywords are non-zero). If ZNAXIS is equal to 0, there shall not be any ZNAXISn keywords."
   copy: true
-  expand: True
+  expand: true
 ZTILE<n>:
   description: "This keyword shall contain a positive integer representing the number of pixels along axis n of the compression tiles. Each tile of pixels is compressed separately and stored in a row of a variable-length vector column in the binary table. The size of each image dimension (given by ZNAXISn) is not required to be an integer multiple of ZTILEn, and if it is not, then the last tile along that dimension of the image will contain fewer image pixels than the other tiles.
                 If the ZTILEn keywords are not present then the default ’row by row’ tiling will be assumed such that ZTILE1 = ZNAXIS1, and the value of all the other ZTILEn keywords equals 1.
                 The compressed image tiles are stored in the binary table in the same order that the first pixel in each tile appears in the FITS image; the tile containing the first pixel in the image appears in the first row of the table, and the tile containing the last pixel in the image appears in the last row of the binary table."
   type: int
   units: pix
-  expand: True
+  expand: true
 ZHECKSUM:
   description: "The value field of this keyword must contain the original CHECKSUM keyword in the uncompressed image."
   type: str
 ZDATASUM:
   description: "The value field of this keyword must contain the original DATASUM keyword in the uncompressed image."
   type: str
 ZSIMPLE:
@@ -67,19 +67,19 @@
 # parameters".
 # In practice for RICE compression it seems to be equal to ZNAXIS, but the
 # specifications repo expands the schema to match the highest number in all the
 # ZVAL keys
 ZNAME<z>:
   description: "This is a keyword with ZVALz. This pair of optional array keywords supply the compression block size and the pixels per block, respectively."
   type: str
-  expand: True
+  expand: true
 ZVAL<z>:
   description: "This is a keyword with ZNAMEz. This pair of optional array keywords supply the pixels per block and the compression block size, respectively. Possible values: 1, 2, 4, or 8."
   type: int
-  expand: True
+  expand: true
 
 # FITS Binary Table keys
 # Included here and not in the fits table to make it clear we only use these for compressed data.
 TFIELDS:
   description: "The value field shall contain a non-negative integer representing the number of fields in each row."
   fitsreference: "7.3: Binary Table Extension"
   type: int
```

### Comparing `dkist_fits_specifications-4.1.1rc1/dkist_fits_specifications/spec214/schemas/cryonirsp.yml` & `dkist_fits_specifications-4.2.0/dkist_fits_specifications/spec214/schemas/cryonirsp.yml`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 spec214:
   section_122: cryonirsp
-  copy: True
+  copy: true
   required: false
-  expand: False
+  expand: false
   units: null
   description: ""
   title: Cryo-NIRSP Instrument
   summary: Keys specific to the operation of the Cryo-NIRSP instrument.
 ---
 CNARMID:
   rename: "CRSP_001"
@@ -385,13 +385,13 @@
   rename: "CRSP_113"
 CNL3TOTN:
   rename: "CRSP_114"
 CNNMAPS:
   description: "Number of map scans"
   comment: TotalMapScans
   type: int
-  copy: False
+  copy: false
 CNMAP:
   description: "Number of the current map scan"
   comment: CurrentMapScan
   type: int
-  copy: False
+  copy: false
```

### Comparing `dkist_fits_specifications-4.1.1rc1/dkist_fits_specifications/spec214/schemas/datacenter.yml` & `dkist_fits_specifications-4.2.0/dkist_fits_specifications/spec214/schemas/datacenter.yml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 spec214:
   section_122: null
-  copy: False
+  copy: false
   required: true
   units: null
-  expand: False
+  expand: false
   title: Datacenter
   summary: Keys generated by the DKIST data center to describe processing performed, archiving or extra metadata.
 ---
 DSETID:
   description: "Unique ID of the dataset to which the frame belongs."
   type: str
 POINT_ID:
```

### Comparing `dkist_fits_specifications-4.1.1rc1/dkist_fits_specifications/spec214/schemas/dataset.yml` & `dkist_fits_specifications-4.2.0/dkist_fits_specifications/spec214/schemas/dataset.yml`

 * *Files 6% similar despite different names*

```diff
@@ -1,63 +1,63 @@
 spec214:
   section_122: null
-  copy: False
+  copy: false
   required: true
   units: null
-  expand: False
+  expand: false
   title: Dataset
   summary: Keys describing the dataset that this FITS file forms a part of.
   long_description: |
     Each dataset has a given number of axes ``DNAXIS``, ``DAAXES`` of which are contained in the array in a given FITS file, ``DEAXES`` of which are "striped" along all the FITS files that comprise the dataset.
     The keys in this table give information about all the dataset axes, both inside and outside of the array in a given FITS file.
 ---
 DNAXIS:
   description: "The number of axes in the dataset. Normally between three and five, depending on instrument mode."
   type: int
 DNAXIS<d>:
   description: "The length of the nth dataset axis. The length of the axes contained in the FITS file will also be stored in the NAXISn key, but will be duplicated here for clarity."
   type: int
   units: pix
-  expand: True
+  expand: true
 DTYPE<d>:
   description: "The physical type of the nth axis in the dataset"
   type: str
   values:
     - 'SPATIAL'
     - 'SPECTRAL'
     - 'TEMPORAL'
     - 'STOKES'
-  expand: True
+  expand: true
 DPNAME<d>:
   description: "The name of the nth pixel axis. This is a description of the axis in pixel units. For example it might be 'slit position' or 'scan number'. This is to aid identification of the axes based on the operation of the instrument rather than the world coordinate of that axes."
   type: str
-  expand: True
+  expand: true
 DWNAME<d>:
   type: str
   description: "The name of the nth world coordinate axis. This is the description of the world coordinate corresponding to the nth pixel axis. For example this might be 'helioprojective longitude' or 'wavelength'."
-  expand: True
+  expand: true
 DUNIT<d>:
   type: str
   description: "The unit of the nth world coordinate axis. This should follow the same specification as the FITS standard key CUNITn, and will duplicate the values in CUNITn for the dataset axes which are in the FITS array."
-  expand: True
+  expand: true
   format: 'unit'
 DAAXES:
   type: int
   description: "The number of dataset axes which are contained in the FITS array. This should also equal the number of non-unity length axes in the FITS array. This is included to facilitate the correct encoding of slit-spectrograph frames, which while they are stored as two dimensional arrays have three world coordinate axes (two spatial dimensions for one spatial array axis). FITS-WCS requires the number of pixel and world axes to match, so an extra length unity dimension is added in this situation."
 DEAXES:
   type: int
   description: "The number of dataset pixel axes not present in the FITS array. This is included as it prevents needing to calculate this number by doing DNAXIS - DAAXES."
 DINDEX<k>:
   type: int
   description: "The k index is the range of values between DAAXES + 1 and DAAXES + DEAXES + 1, i.e. the indices of the dataset axes not in the FITS array. This number gives the position of the current frame in the axes of the dataset that are not contained within the array in the FITS file."
   units: pix
-  expand: True
+  expand: true
 LINEWAV:
   section_122: "fits"
-  copy: True
+  copy: true
   rename: "WAVELNTH"
   description: "The central wavelength being observed. This could be the center of a filter or the center of a wavelength range. It should be the same for all frames in a dataset."
 FRAMEWAV:
   type: float
   required: false
   description: "The wavelength observed by this frame. Used when a frame is a narrowband observation observed at a single wavelength. For instance one frame in a sequence of frames scanning a line."
   units: nm
```

### Comparing `dkist_fits_specifications-4.1.1rc1/dkist_fits_specifications/spec214/schemas/dkist-id.yml` & `dkist_fits_specifications-4.2.0/dkist_fits_specifications/spec214/schemas/dkist-id.yml`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 spec214:
   section_122: dkist-id
-  copy: True
+  copy: true
   required: true
   units: null
-  expand: False
+  expand: false
   title: DKIST ID
   summary: Unique identifiers for this FITS file and the observation that created the data.
 ---
 FILE_ID:
   rename: "ID___002"
   description: "Unique ID of this FITS file."
 DKISTVER:
@@ -36,25 +36,25 @@
   required: false
 NPROPOS:
   description: "Number of proposals that contributed to the input data used to make this output. Must be > 0."
   required: false
   type: int
   values_range:
     - 1
-  copy: False
+  copy: false
 PROPID<rr>:
   description: "One of the NPROPOS proposal IDs that contributed input data to make this output. 1 <= rr <= NPROPOS"
   required: false
   type: str
-  copy: False
+  copy: false
 NEXPERS:
   description: "Number of experiments that contributed to the input data used to make this output. Must be > 0."
   required: false
   type: int
   values_range:
     - 1
-  copy: False
+  copy: false
 EXPRID<ee>:
   description: "One of the NEXPERS experiment IDs that contributed input data to make this output. 1 <= ee <= NEXPERS"
   required: false
   type: str
-  copy: False
+  copy: false
```

### Comparing `dkist_fits_specifications-4.1.1rc1/dkist_fits_specifications/spec214/schemas/dkist-op.yml` & `dkist_fits_specifications-4.2.0/dkist_fits_specifications/spec214/schemas/dkist-op.yml`

 * *Files 9% similar despite different names*

```diff
@@ -1,43 +1,48 @@
 spec214:
   section_122: dkist-dkist
-  copy: True
+  copy: true
   required: false
   units: null
-  expand: False
+  expand: false
   title: DKIST Operations
   summary: Information about this configuration or operations of the facility when generating this data.
 ---
 OCS_CTRL:
   rename: "DKIST001"
   description: "Control mode the telescope was operated in:
                 ‘Auto’: Data were acquired as part of a regular, automatic execution of an Observing Program
                 ‘Manual’: Data were acquired executing either a part of an or a complete Observing Program manually."
-  required: True
+  required: true
 FIDO_CFG:
   rename: "DKIST005"
   description: "The DKIST FIDO configuration in the following format:
                 [M9aStatus,CL2,CL2a,CL3,CL3a,CL4]"
-  required: True
+  required: true
 DSHEALTH:
   rename: "DKIST006"
   description: "Worst health status of the data source (e.g. instrument arm) during data acquisition
                 Good, Ill, Bad, Unknown"
-  required: True
+  required: true
 DSPSREPS:
   rename: "DKIST008"
   description: " Number of repeated DataSetParameterSequences within an InstrumentProgram."
-  required: True
+  required: true
 DSPSNUM:
   rename: "DKIST009"
   description: "Number describing the current repetition of the DataSetParameterSequence within an InstrumentProgram."
-  required: True
+  required: true
 LIGHTLVL:
   rename: "DKIST010"
   description: "Value of the telescope light level at start of data acquisition."
   units: adu
-  required: True
+  required: true
 IPTASK:
   rename: "DKIST004"
   description: "Instrument Program Task addressed by the Instrument Program that led to the acquisition of this data"
   required: true
   level0_only: true
+LYOTSTAT:
+  rename: "DKIST013"
+  description: "Value indicating the status of the Lyot Stop in the DKIST science beam.
+                true if the Lyot stop was in the beam when the frame was acquired; false otherwise."
+  required: false
```

### Comparing `dkist_fits_specifications-4.1.1rc1/dkist_fits_specifications/spec214/schemas/dlnirsp.yml` & `dkist_fits_specifications-4.2.0/dkist_fits_specifications/spec214/schemas/dlnirsp.yml`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,42 @@
 spec214:
   section_122: dlnirsp
-  copy: True
+  copy: true
   required: false
   units: null
-  expand: False
+  expand: false
   title: DL-NIRSP Instrument
   summary: Keys specific to the operation of the DL-NIRSP instrument.
 ---
 DLARMID:
   rename: "DLN__001"
   description: "Identifier for DL-NIRSP arm that generated the data"
 DLARMPS:
   rename: "DLN__002"
   description: "Position of the arm linear stage."
-  units: deg
+  units: mm
 DLARMFC:
   rename: "DLN__003"
   description: "Position of the camera focus stage."
   units: mm
 DLFILT:
   rename: "DLN__004"
   description: "Unique ID of the filter in use"
+DLWAV:
+  rename: "DLN__005"
+  description: "Central wavelength of the filter in use"
+  units: nm
 DLFWHM:
   rename: "DLN__006"
   description: "Full Width at Half Maximum spectral transmission at the current filter in use"
   units: nm
+DLFLTPOS:
+  rename: "DLN__007"
+  description: "Position of the filter wheel rotation stage"
+  units: deg
 DLPOLMD:
   rename: "DLN__008"
   description: "Polarimeter Mode with which these data were acquired"
 DLMODID:
   rename: "DLN__009"
   description: "Unique identifier of the modulator."
 DLMOD:
@@ -37,76 +45,87 @@
 DLMODRT:
   rename: "DLN__011"
   description: "Rate at which modulation states are acquired."
   units: Hz
 DLMODN:
   rename: "DLN__012"
   description: "Integer number identifier corresponding to the particular state defined by the position of the modulator at its reference time"
+  level0_only: true
 DLMDANG:
   rename: "DLN__013"
   description: "Modulator angle corresponding to the modulation state at the reference time."
   units: deg
+  level0_only: true
 DLNUMST:
   rename: "DLN__014"
   description: "Number of states to be acquired during a modulation cycle:
                 NumberOfStates ≥ 1. It is required that there be a one-to-one sequential mapping from modulator states to CSS accumulators."
 DLSTNUM:
   rename: "DLN__015"
   description: "Number of the current modulation state:
                 1 ≤ CurrentStateNumber ≤ NumberOfStates"
+  level0_only: true
 DLGRTID:
   rename: "DLN__016"
   description: "Unique identifier of the grating in use."
 DLGRTCN:
   rename: "DLN__017"
-  description: "Grating constant."
+  description: "Grating constant, in lines per mm."
   units: 1/mm
 DLGRTBA:
   rename: "DLN__018"
   description: "Grating blaze angle."
   units: deg
 DLGRTAN:
   rename: "DLN__019"
   description: "Grating angle with respect to incident beam."
   units: deg
 DLNDATAC:
   rename: "DLN__020"
   description: "The number of data cycles that should occur for each mosaic tile. A data cycle can be a single or multiple modulation states. A modulation cycle is defined in discrete sampling by the collection of state values. In continuous sampling, it is defined as one half-rotation of the modulator."
+DLCURDAT:
+  rename: "DLN__021"
+  description: "The index of the current data cycle at this mosaic tile position."
+  level0_only: true
 DLCOADD:
   rename: "DLN__022"
   description: "Defines how data were coadded by the detector. Values are defined as follows:
                 State: All coadded exposures for a single state are acquired prior to progressing to the next modulation state (discrete modulation). Equivalent states are coadded.
                 Sequence: The full modulation sequence for a half rotation is cycled through a number of times equivalent to the number of accumulations.
                 Half-rotation: States of the first half rotation are coadded with comparable states of the second half rotation.
                 None: All exposures are saved without coadding."
 DLFRATIO:
   rename: "DLN__023"
   description: "Configuration of the DL-NIRSP Feed Optics"
 DLF4POS:
   rename: "DLN__024"
   description: "Position of the Feed Optics fold mirror 4 stage which selects the focal ratio."
+  units: deg
 DLF1POS:
   rename: "DLN__025"
   description: "Position of the Feed Optics f/62 mirror 1 stage which selects the focal ratio."
+  units: mm
 DLIFU:
   rename: "DLN__026"
-  description: "BiFOIS-IFU that was used for this observation"
+  description: "Value indicating IFU that was used for this observation"
 DLIFUPOS:
   rename: "DLN__027"
   description: "Position of the IFU stage"
+  units: mm
 DLSLITMD:
   rename: "DLN__028"
   description: "Value indicating whether DL-NIRSP was operated in single, multi-slit, or dark configuration"
 DLSLIT:
   rename: "DLN__029"
   description: "Identifier of the slit used when DL-NIRSP is operated in single slit mode.
                 Keyword not present, if not used"
 DLSLITPS:
   rename: "DLN__030"
   description: "Position of the slit mask stage"
+  units: mm
 DLMOSNRP:
   rename: "DLN__031"
   description: "Total number of times the mosaic pattern is to repeat."
 DLCURMOS:
   rename: "DLN__032"
   description: "Index of the current repeat of the mosaic."
 DLMSPAT:
@@ -115,49 +134,52 @@
 DLNSSTPX:
   rename: "DLN__034"
   description: "Number of mosaic steps in horizontal direction belonging to the scanned FieldOfView.
                 Keyword not present, if not used"
 DLSTPCPX:
   rename: "DLN__035"
   description: "Angular position of the center position in the horizontal direction of the field scan given in units of the field scanning mirror motorized stage. Default position will be a property updated when the instrument is co-aligned with other instruments using a GOS target."
-  units: deg
+  units: urad
 DLSTPX:
   rename: "DLN__036"
   description: "Angular step size in the horizontal direction given in units of the field scanning mirror motorized stage. Default value will be calculated according to IFU, slits, and feed optics selection."
-  units: deg
+  units: urad
 DLCSTPX:
   rename: "DLN__037"
   description: "Current image position in horizontal direction belonging to the scanned FieldOfView.
                 1 ≤ CurrentSpatialStepX ≤ NumberofSpatialStepsX
                 Keyword not present, if not used"
 DLNSSTPY:
   rename: "DLN__038"
-  description: "Number of images in vertical direction belonging to the scanned FieldOfView.
+  description: "Value indicating the number of images in vertical direction belonging to the scanned FieldOfView.
                 Keyword not present, if not used"
 DLSTPCPY:
   rename: "DLN__039"
   description: "Angular position of the center position in the vertical direction of the field scan given in units of the field scanning mirror motorized stage. Default position will be a property updated when the instrument is co-aligned with other instruments using a GOS target."
+  units: urad
 DLSTPY:
   rename: "DLN__040"
   description: "Angular step size in the vertical direction given in units of the field scanning mirror motorized stage. Default value will be calculated according to IFU, slits, and feed optics selection."
-  units: deg
+  units: urad
 DLCSTPY:
   rename: "DLN__041"
   description: "Value indicating the current image position in vertical direction belonging to the scanned FieldOfView.
                 1 ≤ CurrentSpatialStepY ≤ NumberOfSpatialStepsY
                 Keyword not present, if not used"
 DLDMODE:
   rename: "DLN__042"
   description: "Boolean indicating whether the DL-NIRSP dithering mode was activated or not. When enabled, a sub-unit field shift is used between successive completed FieldSamples"
 DLDOFFX:
   rename: "DLN__043"
-  description: "Offset of the dithered position in the X direction. Keyword not present if DitherMode is False."
+  description: "Offset of the dithered position in the X direction. Keyword not present if DitherMode is false."
+  units: urad
 DLDOFFY:
   rename: "DLN__044"
-  description: "Offset of the dithered position in the Y direction. Keyword not present if DitherMode is False."
+  description: "Offset of the dithered position in the Y direction. Keyword not present if DitherMode is false."
+  units: urad
 DLCURSTP:
   rename: "DLN__045"
   description: "An integer to indicate whether this spatial step corresponds to the dithered position. Keyword not present if DitherMode is false."
 DLCAMSMD:
   rename: "DLN__046"
   description: "A keyword for H2RGs only. Distinguishes whether the camera was operating in sub- frame time integration."
 DLCAMSSQ:
@@ -168,14 +190,15 @@
   description: "A Keyword for H2RGs only. The number of science frames acquired per ramp, in the '1 line 2 read' example, the number of science frames would be 2."
 DLCAMNS:
   rename: "DLN__049"
   description: "A keyword for H2RGs only. The total number of frames in a read sequence, including bias or calibration frames, acquired per ramp."
 DLCAMCUR:
   rename: "DLN__050"
   description: "A keyword for H2RGs only. The index of the sample in a read sequence."
+  level0_only: true
 DLCAMOFF:
   rename: "DLN__051"
   description: "A keyword for H2RGs only. How long (average) after the trigger does the exposure start"
   units: ms
 DLCAMTIM:
   rename: "DLN__052"
   description: "A keyword for H2RGs only. How long (average) between exposure starts"
@@ -183,7 +206,12 @@
 DLARTEMP:
   rename: "DLN__053"
   description: "A keyword for H2RGs only. Most recent temperature of the detector array in Kelvin."
   units: K
 DLCAMFID:
   rename: "DLN__054"
   description: "A keyword for H2RGs only. Identifier for the camera cold filter or prefilter."
+DLMODT0:
+  rename: "DLN__055"
+  description: "UTC Data/Time of the modulator reference time, T0, in the form:
+                YYYY-MM-DDThh:mm:ss.sss[…]
+                Accuracy at minimum to [ms]"
```

### Comparing `dkist_fits_specifications-4.1.1rc1/dkist_fits_specifications/spec214/schemas/fits.yml` & `dkist_fits_specifications-4.2.0/dkist_fits_specifications/spec214/schemas/fits.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 spec214:
   section_122: fits
-  copy: True
+  copy: true
   required: true
   units: null
-  expand: False
+  expand: false
   title: FITS
   summary: Keys mandated or described by the FITS 4.0 standard.
 ---
 SIMPLE:
   description: "Mandatory FITS keyword when in the primary HDU."
   required: false
   fitsreference: "4.4.1.1: Primary header"
@@ -21,15 +21,15 @@
   type: int
   copy: false  # We don't copy this because it's always 3 in 122
 NAXIS<n>:
   description: "The value field of this indexed keyword shall contain a non-negative integer representing the number of elements along axis n of a data array. A value of zero for any of the NAXISn keywords signifies that no data follow the header in the HDU (however, the random groups structure has NAXIS1 = 0, but will have data following the header if the other NAXISn keywords are non-zero). If NAXIS is equal to 0, there shall not be any NAXISn keywords."
   fitsreference: "4.4.1.1: Primary header"
   units: pix
   copy: "schema"
-  expand: True
+  expand: true
 BUNIT:
   description: "The physical unit of the data values after application of BZERO and BSCALE (physical_value in BUNIT = BZERO + BSCALE × array_value.)"
   fitsreference: "4.4.2.5: Keywords that describe arrays"
   copy: "schema"
 BTYPE:
   description: "Description of what the data array represents."
   copy: false
@@ -62,29 +62,29 @@
   fitsreference: "4.4.2.2: Keywords describing observations"
   rename: 'DATE-OBS'
 DATE-END:
   description: "End date and time of light exposure for the frame."
   fitsreference: "4.4.2.2: Keywords describing observations"
   type: str
   format: isot
-  copy: False
+  copy: false
 TELAPSE:
   copy: false
   description: "TELAPSE = DATE-END - DATE-BEG. Not always equal to the exposure time as multiple exposures could be combined."
   type: float
   units: s
 DATE-AVG:
   description: "Date/Time of the midpoint of the frame. (DATE-END - DATE_BEG) / 2"
   fitsreference: "4.4.2.2: Keywords describing observations"
   copy: false
   type: str
   format: isot
 TIMESYS:
   description: "Time scale of the time related keywords."
-  copy: False
+  copy: false
   type: str
   required: false
   values:
     - 'UTC'
 ORIGIN:
   description: "The organization or institution responsible for creating the FITS file."
   fitsreference: "4.4.2.1: General descriptive keywords"
```

### Comparing `dkist_fits_specifications-4.1.1rc1/dkist_fits_specifications/spec214/schemas/pac.yml` & `dkist_fits_specifications-4.2.0/dkist_fits_specifications/spec214/schemas/pac.yml`

 * *Files 4% similar despite different names*

```diff
@@ -1,82 +1,82 @@
 spec214:
   section_122: pac
-  copy: True
+  copy: true
   required: false
   units: null
-  expand: False
+  expand: false
   title: Polarization Analysis and Calibration
   summary: Keys describing the configuration of the Gregorian Optical System (GOS)
 ---
 GOS_STAT:
   rename: "PAC__001"
   description: "Status of the upper GOS
                 shutter."
-  required: True
+  required: true
 LVL3STAT:
   rename: "PAC__002"
   description: "Status of Level 3 in the GOS."
-  required: True
+  required: true
 LAMPSTAT:
   rename: "PAC__003"
   description: "Status of the GOS Level 3 Lamp."
-  required: True
+  required: true
 LVL2STAT:
   rename: "PAC__004"
   description: "Status of Level 2 in the
                 GOS."
-  required: True
+  required: true
 POLANGLE:
   rename: "PAC__005"
   description: "Polarizer angle, if in the beam (values shown below are relative to those of LVL2STAT)"
   units: deg
-  required: True
+  required: true
 LVL1STAT:
   rename: "PAC__006"
   description: "Status of Level 1 in the
                 GOS."
-  required: True
+  required: true
 RETANGLE:
   rename: "PAC__007"
   description: "Retarder angle, if in the beam (values shown below are relative to those of LVL1STAT)"
   units: deg
-  required: True
+  required: true
 LVL0STAT:
   rename: "PAC__008"
   description: "Status of Level 0 in the GOS.
                 FieldStop (2.8arcmin), FieldStop (5arcmin), DarkShutter, Pinhole (large), Pinhole (small), Pinhole (inverse), Occulter (2.8arcmin), Occulter (5arcmin), NonRedArray, LineGrid, AFResTarget, ReflSphere, Undefined"
-  required: True
+  required: true
 APERTURE:
   rename: "PAC__009"
   description: "Current Aperture property, if in the beam (values shown below are relative to those of LVL0STAT)
                 2.8arcmin, 5arcmin, 1.7arcsec, 0.2arcsec, 0.3arcsec, (tracking, non-tracking), (tracking, non-tracking), None, 0.5mm, None"
-  required: True
+  required: true
 LGOSSTAT:
   rename: "PAC__010"
   description: "Status of the lower GOS shutter."
-  required: True
+  required: true
 GOS_TEMP:
   rename: "PAC__011"
   description: "Temperature of the optics in the GOS."
-  required: True
+  required: true
   units: C
 POL_NOIS:
   description: "RMS noise of the scan"
   type: float
   copy: false
-  polarimetric_required: True
+  polarimetric_required: true
 POL_SENS:
   description: "Estimate of the polarization sensitivity of the scan. This is measured by finding the smallest signal measured within the scan"
   type: float
   units: adu
   copy: false
-  polarimetric_required: True
+  polarimetric_required: true
 STOKES:
   description: "Stokes parameter"
   type: str
   copy: false
-  required: True
+  required: true
   values:
     - 'I'
     - 'Q'
     - 'U'
     - 'V'
```

### Comparing `dkist_fits_specifications-4.1.1rc1/dkist_fits_specifications/spec214/schemas/stats.yml` & `dkist_fits_specifications-4.2.0/dkist_fits_specifications/spec214/schemas/stats.yml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 spec214:
   section_122: null
-  copy: False
+  copy: false
   required: false
   expected: true
   units: 'dimensionless'
-  expand: False
+  expand: false
   title: Statistics
   summary: Statistical information about the data array contained in this FITS file.
 ---
 DATAMIN:
   description: "The minimum data value."
   type: float
 DATAMAX:
```

### Comparing `dkist_fits_specifications-4.1.1rc1/dkist_fits_specifications/spec214/schemas/telescope.yml` & `dkist_fits_specifications-4.2.0/dkist_fits_specifications/spec214/schemas/telescope.yml`

 * *Files 3% similar despite different names*

```diff
@@ -1,118 +1,118 @@
 spec214:
   section_122: telescope
-  copy: True
+  copy: true
   units: null
-  expand: False
+  expand: false
   title: Telescope
   summary: Keys describing the pointing and operation of the telescope. Including the FITS WCS keys describing the world coordinates of the array.
 ---
 WCSAXES:
   description: "Number of axes in the Helioprojective Cartesian WCS description. The value of WCSAXES may exceed the number of pixel axes for the HDU. (see also Pence et al. 2010)."
   required: true
   type: int
-  copy: False
+  copy: false
   values:
     - 2
     - 3
 WCSAXESA:
   description: "Same as WCSAXES but for an Equatorial WCS description."
   required: false
   type: int
-  copy: False
+  copy: false
   values:
     - 2
     - 3
 WCSNAME:
   description: "Helioprojective Cartesian"
   required: true
 WCSNAMEA:
   description: "Equatorial"
   required: false
 CRPIX<n>:
   description: "The value field shall contain a floating point number, identifying the location of a reference point along axis n of the Helioprojective coordinate system, in units of the axis index. This value is based upon a counter that runs from 1 to NAXISn with an increment of 1 per pixel. The reference point value need not be that for the center of a pixel nor lie within the actual data array. Use comments to indicate the location of the index point relative to the pixel. DKIST pointing data will be relative to the boresight of the telescope defined by the WFC Context Viewer that will center an image of the GOS pinhole on its detector using a 10 nm wavelength band centered on 525 nm. The same pinhole image will be used by all instruments as reference for determining the pointing of the instrument in relation to the WFC Context Viewer."
   required: true
   units: pix
-  expand: True
+  expand: true
 CRPIX<n>A:
   description: "Same as CRPIXn but for an Equatorial coordinate system."
   required: false
   units: pix
-  expand: True
+  expand: true
 CRDATE<n>:
   description: "Date of last update of CRPIXn and CDELTn value
                 The value will get updated upon realignment of the data source with the WFC Context Viewer (see CRPIXn)"
   required: false
-  expand: True
+  expand: true
 CRDATE<n>A:
   description: "Same as CRDATEn but for CRPIXnA and CDELTnA."
   required: false
-  expand: True
+  expand: true
 CRVAL<n>:
   description: "The value field shall contain a floating point number, giving the value of the coordinate specified by the CTYPEn keyword at the reference point CRPIXn.
                 DKIST values for this entry will be determined at the wavelength of the WFC Context Viewer, which covers a band of 10 nm centered on 525 nm. The value will not be corrected for differential refraction of Earth's atmosphere."
   required: true
-  expand: True
+  expand: true
 CRVAL<n>A:
   description: "Same as CRVALn but for CTYPEnA and CRPIXnA."
   required: false
-  expand: True
+  expand: true
 CDELT<n>:
   description: "Pixel scale of the world coordinate at the reference point along axis n of the Helioprojective coordinate system. This value must not be zero."
   required: true
-  expand: True
+  expand: true
 CDELT<n>A:
   description: "Same as CDELTn but for an Equatorial coordinate system"
   required: false
-  expand: True
+  expand: true
 CUNIT<n>:
   description: "The unit of the value contained in CDELTn"
   required: true
-  expand: True
+  expand: true
 CUNIT<n>A:
   description: "The unit of the value contained in CDELTnA"
   required: false
-  expand: True
+  expand: true
 CTYPE<n>:
   description: "A string value labeling axis n of the Helioprojective Coordinate system."
   required: true
-  expand: True
+  expand: true
 CTYPE<n>A:
   description: "Same as CTYPEn but for an Equatorial coordinate system."
   required: false
-  expand: True
+  expand: true
 PC<i>_<j>:
   description: "Linear transformation matrix used with the Helioprojective coordinate system"
   required: true
-  expand: True
+  expand: true
 PC<i>_<j>A:
   description: "Linear transformation matrix used with the Equatorial coordinate system"
   required: false
-  expand: True
+  expand: true
 #not currently in use
 #PVi_m:
 #  description: ''
 #  required: true
 #  type: float
-#  expand: True
+#  expand: true
 #PVi_mA:
 #  description: ''
 # required: false
 #  type: float
-#  expand: True
+#  expand: true
 #PSi_m:
 #  description: ''
 #  required: true
 #  type: float
-#  expand: True
+#  expand: true
 #PSi_mA:
 #  description: ''
 #  required: false
 #  type: float
-#  expand: True
+#  expand: true
 LONPOLE:
   description: "Native longitude of the celestial pole in Helioprojective coordinate system"
   required: false
   units: deg
 LONPOLEA:
   description: "Native longitude of the celestial pole in Equatorial coordinate system"
   required: false
@@ -226,15 +226,15 @@
   required: false
 MINDEX2:
   description: "Position of this tile on the second axis of a mosaic"
   type: int
   copy: false
   required: false
 WCSVALID:
-  description: "In instances when the computation of WCI data fails (e.g. for the task 'Dark'), this flag wil be set to False. Default: True"
+  description: "In instances when the computation of WCI data fails (e.g. for the task 'Dark'), this flag wil be set to false. Default: true"
   copy: true
   required: false
 SOLARRAD:
   description: "The solar radius at the time of observation, in arcseconds."
   type: float
   units: arcsec
   required: false
```

### Comparing `dkist_fits_specifications-4.1.1rc1/dkist_fits_specifications/spec214/schemas/vbi.yml` & `dkist_fits_specifications-4.2.0/dkist_fits_specifications/spec214/schemas/vbi.yml`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 spec214:
   section_122: vbi
-  copy: True
+  copy: true
   required: false
   units: null
-  expand: False
+  expand: false
   title: VBI Instrument
   summary: Keys specific to the operation of the VBI instrument.
 ---
 VBIFWHM:
   rename: "VBI__001"
   description: "Full Width at Half Maximum spectral transmission."
   units: nm
@@ -41,13 +41,13 @@
 VBIFRIED:
   rename: "VBI__009"
   description: "Value indicating the Fried parameter per field. Value equals -1 if speckle reconstruction is not enabled, or if speckle reconstruction is enabled but no r0 is available."
 VBINMOSC:
   description: "Total number of mosaic repeats in dataset."
   instrument_required: VBI
   type: int
-  copy: False
+  copy: false
 VBICMOSC:
   description: "Current mosaic repeat."
   instrument_required: VBI
   type: int
-  copy: False
+  copy: false
```

### Comparing `dkist_fits_specifications-4.1.1rc1/dkist_fits_specifications/spec214/schemas/visp.yml` & `dkist_fits_specifications-4.2.0/dkist_fits_specifications/spec214/schemas/visp.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 spec214:
   section_122: visp
-  copy: True
+  copy: true
   required: false
   units: null
-  expand: False
+  expand: false
   title: VISP Instrument
   summary: Keys specific to the operation of the VISP instrument.
 ---
 VSPARMID:
   rename: "VISP_001"
   description: "Identifier for ViSP arm that generated the data:"
 VSPARMPS:
@@ -98,13 +98,13 @@
   rename: "VISP_023"
   description: "Position of the slit selector stage."
   units: mm
 VSPNMAPS:
   description: "Number of map scans"
   comment: TotalMapScans
   type: int
-  copy: False
+  copy: false
 VSPMAP:
   description: "Number of the current map scan"
   comment: CurrentMapScan
   type: int
-  copy: False
+  copy: false
```

### Comparing `dkist_fits_specifications-4.1.1rc1/dkist_fits_specifications/spec214/schemas/vtf.yml` & `dkist_fits_specifications-4.2.0/dkist_fits_specifications/spec214/schemas/vtf.yml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 spec214:
   section_122: vtf
-  copy: True
+  copy: true
   required: false
   units: null
-  expand: False
+  expand: false
   title: VTF Instrument
   summary: Keys specific to the operation of the VTF instrument.
 ---
 VTFINSTM:
   rename: "VTF__001"
   description: "Indicates the current operating mode of the VTF:
                 Spectropolarimetric Imaging SI,
```

### Comparing `dkist_fits_specifications-4.1.1rc1/dkist_fits_specifications/spec214/schemas/wfc.yml` & `dkist_fits_specifications-4.2.0/dkist_fits_specifications/spec214/schemas/wfc.yml`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 spec214:
   section_122: wfc
-  copy: True
+  copy: true
   required: false
   units: null
-  expand: False
+  expand: false
   expected: true
   title: Wavefront Correction
   summary: Keys describing the operation of the wavefront correction system.
 ---
 FLTFWHM:
   rename: "WFC__001"
   description: "Full Width at Half Maximum spectral transmission at the current prefilter central wavelength."
```

### Comparing `dkist_fits_specifications-4.1.1rc1/dkist_fits_specifications/spec214/schemas/ws.yml` & `dkist_fits_specifications-4.2.0/dkist_fits_specifications/spec214/schemas/ws.yml`

 * *Files 14% similar despite different names*

```diff
@@ -1,52 +1,52 @@
 spec214:
   section_122: ws
-  copy: True
+  copy: true
   required: false
-  expand: False
+  expand: false
   title: Weather Station
   summary: Keys describing information reported by the weather station at the facility during this observation.
 ---
 WSSOURCE:
   rename: "WS___001"
   description: "Name of the source of these weather data"
   units: null
-  required: True
+  required: true
 WIND_SPD:
   rename: "WS___002"
   description: "DKIST Local Outside Wind Speed"
   units: m/s
-  required: True
+  required: true
 WIND_DIR:
   rename: "WS___003"
   description: "DKIST Local Outside Wind Direction
                 North: 0 deg
                 East: 90 deg
                 South: 180 deg
                 West: 270 deg"
   units: deg
-  required: True
+  required: true
 WS_TEMP:
   rename: "WS___004"
   description: "DKIST Local Outside Tempertature"
   units: C
-  required: True
+  required: true
 WS_HUMID:
   rename: "WS___005"
   description: "DKIST Local Outside Relative Humidity"
   units: '%'
-  required: True
+  required: true
 WS_DEWPT:
   rename: "WS___006"
   description: "DKIST Local Outside Dew Point"
   units: C
-  required: True
+  required: true
 WS_PRESS:
   rename: "WS___007"
   description: "DKIST Local Outside Barometric Pressure"
   units: hPa
-  required: True
+  required: true
 SKYBRIGT:
   rename: "WS___008"
   description: "DKIST Local Outside Sky Brightness in PPM of the disk center intensity. Value is -1.0 if no data available"
   units: null
-  required: True
+  required: true
```

### Comparing `dkist_fits_specifications-4.1.1rc1/dkist_fits_specifications/spec214/spec214_full_schema.yml` & `dkist_fits_specifications-4.2.0/dkist_fits_specifications/spec214/spec214_full_schema.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-4.1.1rc1/dkist_fits_specifications/spec_validation_schema.yml` & `dkist_fits_specifications-4.2.0/dkist_fits_specifications/spec_validation_schema.yml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-4.1.1rc1/dkist_fits_specifications/tests/test_122.py` & `dkist_fits_specifications-4.2.0/dkist_fits_specifications/tests/test_122.py`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-4.1.1rc1/dkist_fits_specifications/tests/test_214.py` & `dkist_fits_specifications-4.2.0/dkist_fits_specifications/tests/test_214.py`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-4.1.1rc1/dkist_fits_specifications/tests/test_expansions.py` & `dkist_fits_specifications-4.2.0/dkist_fits_specifications/tests/test_expansions.py`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-4.1.1rc1/dkist_fits_specifications/tests/test_level0_214.py` & `dkist_fits_specifications-4.2.0/dkist_fits_specifications/tests/test_level0_214.py`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-4.1.1rc1/dkist_fits_specifications/utils/formatter.py` & `dkist_fits_specifications-4.2.0/dkist_fits_specifications/utils/formatter.py`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-4.1.1rc1/dkist_fits_specifications/utils/frozendict.py` & `dkist_fits_specifications-4.2.0/dkist_fits_specifications/utils/frozendict.py`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-4.1.1rc1/dkist_fits_specifications/utils/spec.py` & `dkist_fits_specifications-4.2.0/dkist_fits_specifications/utils/spec.py`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-4.1.1rc1/dkist_fits_specifications/utils/spec_processors/expansion.py` & `dkist_fits_specifications-4.2.0/dkist_fits_specifications/utils/spec_processors/expansion.py`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-4.1.1rc1/dkist_fits_specifications/utils/spec_processors/instrument_requiredness.py` & `dkist_fits_specifications-4.2.0/dkist_fits_specifications/utils/spec_processors/instrument_requiredness.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,9 +17,9 @@
 
     def __init__(self, header: dict[str, Any]):
         super().__init__(header=header)
         self.instrument = self.header.get("INSTRUME", _NOT_A_DKIST_INSTRUMENT).casefold()
 
     def check_requiredness(self, spec_fields: frozendict[str, Any]) -> bool:
         """Check if the required instrument matches the instrument in the header."""
-        # "False" is importantly different than _NOT_A_DKIST_INSTRUMENT
-        return spec_fields.get("instrument_required", "False").casefold() == self.instrument
+        # "false" is importantly different than _NOT_A_DKIST_INSTRUMENT
+        return spec_fields.get("instrument_required", "false").casefold() == self.instrument
```

### Comparing `dkist_fits_specifications-4.1.1rc1/dkist_fits_specifications/utils/spec_processors/polarimetric_requiredness.py` & `dkist_fits_specifications-4.2.0/dkist_fits_specifications/utils/spec_processors/polarimetric_requiredness.py`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-4.1.1rc1/dkist_fits_specifications/utils/spec_processors/requiredness_base.py` & `dkist_fits_specifications-4.2.0/dkist_fits_specifications/utils/spec_processors/requiredness_base.py`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-4.1.1rc1/dkist_fits_specifications/utils/sphinx/spec_table.py` & `dkist_fits_specifications-4.2.0/dkist_fits_specifications/utils/sphinx/spec_table.py`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-4.1.1rc1/dkist_fits_specifications.egg-info/PKG-INFO` & `dkist_fits_specifications-4.2.0/dkist_fits_specifications.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dkist_fits_specifications
-Version: 4.1.1rc1
+Version: 4.2.0
 Summary: Machine readable FITS specifications for DKIST data.
 Home-page: https://bitbucket.org/dkistdc/dkist-fits-specifications/src/main/
 Author: AURA/NSO
 Author-email: stuart@cadair.com
 License: BSD 3-Clause
 Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
```

### Comparing `dkist_fits_specifications-4.1.1rc1/dkist_fits_specifications.egg-info/SOURCES.txt` & `dkist_fits_specifications-4.2.0/dkist_fits_specifications.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 bitbucket-pipelines.yml
 check_changelog_updated.sh
 pyproject.toml
 setup.cfg
 setup.py
 tox.ini
 changelog/.gitempty
-changelog/48.bugfix.rst
 dkist_fits_specifications/__init__.py
 dkist_fits_specifications/py.typed
 dkist_fits_specifications/spec_validation_schema.yml
 dkist_fits_specifications/version.py
 dkist_fits_specifications.egg-info/PKG-INFO
 dkist_fits_specifications.egg-info/SOURCES.txt
 dkist_fits_specifications.egg-info/dependency_links.txt
@@ -59,14 +58,15 @@
 dkist_fits_specifications/spec214/schemas/vtf.yml
 dkist_fits_specifications/spec214/schemas/wfc.yml
 dkist_fits_specifications/spec214/schemas/ws.yml
 dkist_fits_specifications/tests/__init__.py
 dkist_fits_specifications/tests/test_122.py
 dkist_fits_specifications/tests/test_214.py
 dkist_fits_specifications/tests/test_expansions.py
+dkist_fits_specifications/tests/test_formatter.py
 dkist_fits_specifications/tests/test_level0_214.py
 dkist_fits_specifications/utils/__init__.py
 dkist_fits_specifications/utils/formatter.py
 dkist_fits_specifications/utils/frozendict.py
 dkist_fits_specifications/utils/spec.py
 dkist_fits_specifications/utils/spec_processors/__init__.py
 dkist_fits_specifications/utils/spec_processors/expansion.py
```

### Comparing `dkist_fits_specifications-4.1.1rc1/docs/Makefile` & `dkist_fits_specifications-4.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-4.1.1rc1/docs/conf.py` & `dkist_fits_specifications-4.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-4.1.1rc1/docs/index.rst` & `dkist_fits_specifications-4.2.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-4.1.1rc1/docs/level_one.rst` & `dkist_fits_specifications-4.2.0/docs/level_one.rst`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-4.1.1rc1/docs/make.bat` & `dkist_fits_specifications-4.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-4.1.1rc1/docs/specs/spec-122.rst` & `dkist_fits_specifications-4.2.0/docs/specs/spec-122.rst`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-4.1.1rc1/docs/specs/spec-214.rst` & `dkist_fits_specifications-4.2.0/docs/specs/spec-214.rst`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-4.1.1rc1/licenses/LICENSE.rst` & `dkist_fits_specifications-4.2.0/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-4.1.1rc1/licenses/TEMPLATE_LICENSE.rst` & `dkist_fits_specifications-4.2.0/licenses/TEMPLATE_LICENSE.rst`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-4.1.1rc1/pyproject.toml` & `dkist_fits_specifications-4.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-4.1.1rc1/setup.cfg` & `dkist_fits_specifications-4.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-4.1.1rc1/setup.py` & `dkist_fits_specifications-4.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `dkist_fits_specifications-4.1.1rc1/tox.ini` & `dkist_fits_specifications-4.2.0/tox.ini`

 * *Files identical despite different names*

