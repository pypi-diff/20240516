# Comparing `tmp/dls-dodal-1.8.0.tar.gz` & `tmp/dls-dodal-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dls-dodal-1.8.0.tar", last modified: Wed Dec  6 13:04:03 2023, max compression
+gzip compressed data, was "dls-dodal-1.9.0.tar", last modified: Tue Dec 12 14:00:53 2023, max compression
```

## Comparing `dls-dodal-1.8.0.tar` & `dls-dodal-1.9.0.tar`

### file list

```diff
@@ -1,250 +1,250 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 13:04:03.739488 dls-dodal-1.8.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 13:04:03.703488 dls-dodal-1.8.0/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (127)     2140 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/.devcontainer/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 13:04:03.703488 dls-dodal-1.8.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)     1341 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/.github/CONTRIBUTING.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 13:04:03.703488 dls-dodal-1.8.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      302 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/.github/ISSUE_TEMPLATE/issue_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 13:04:03.699488 dls-dodal-1.8.0/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 13:04:03.703488 dls-dodal-1.8.0/.github/actions/install_requirements/
--rw-r--r--   0 runner    (1001) docker     (127)     2060 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/.github/actions/install_requirements/action.yml
--rw-r--r--   0 runner    (1001) docker     (127)      529 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 13:04:03.707488 dls-dodal-1.8.0/.github/pages/
--rw-r--r--   0 runner    (1001) docker     (127)      237 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/.github/pages/index.html
--rwxr-xr-x   0 runner    (1001) docker     (127)     3025 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/.github/pages/make_switcher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 13:04:03.707488 dls-dodal-1.8.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     6590 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/.github/workflows/code.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1863 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/.github/workflows/docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/.github/workflows/docs_clean.yml
--rw-r--r--   0 runner    (1001) docker     (127)      546 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/.github/workflows/linkcheck.yml
--rw-r--r--   0 runner    (1001) docker     (127)      855 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      805 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 13:04:03.707488 dls-dodal-1.8.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)      248 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (127)      871 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (127)      680 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)      398 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    16254 2023-12-06 13:04:03.739488 dls-dodal-1.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1657 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 13:04:03.707488 dls-dodal-1.8.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     6505 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 13:04:03.707488 dls-dodal-1.8.0/docs/developer/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 13:04:03.707488 dls-dodal-1.8.0/docs/developer/explanations/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 13:04:03.707488 dls-dodal-1.8.0/docs/developer/explanations/decisions/
--rw-r--r--   0 runner    (1001) docker     (127)      506 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/docs/developer/explanations/decisions/0001-record-architecture-decisions.rst
--rw-r--r--   0 runner    (1001) docker     (127)      558 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/docs/developer/explanations/decisions.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 13:04:03.711488 dls-dodal-1.8.0/docs/developer/how-to/
--rw-r--r--   0 runner    (1001) docker     (127)      954 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/docs/developer/how-to/build-docs.rst
--rw-r--r--   0 runner    (1001) docker     (127)       47 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/docs/developer/how-to/contribute.rst
--rw-r--r--   0 runner    (1001) docker     (127)      855 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/docs/developer/how-to/lint.rst
--rw-r--r--   0 runner    (1001) docker     (127)      629 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/docs/developer/how-to/make-release.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2899 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/docs/developer/how-to/move-code.rst
--rw-r--r--   0 runner    (1001) docker     (127)      418 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/docs/developer/how-to/run-tests.rst
--rw-r--r--   0 runner    (1001) docker     (127)      267 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/docs/developer/how-to/static-analysis.rst
--rw-r--r--   0 runner    (1001) docker     (127)      744 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/docs/developer/how-to/update-tools.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/docs/developer/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 13:04:03.711488 dls-dodal-1.8.0/docs/developer/reference/
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/docs/developer/reference/standards.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 13:04:03.711488 dls-dodal-1.8.0/docs/developer/tutorials/
--rw-r--r--   0 runner    (1001) docker     (127)     1362 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/docs/developer/tutorials/dev-install.rst
--rw-r--r--   0 runner    (1001) docker     (127)       65 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/docs/genindex.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 13:04:03.711488 dls-dodal-1.8.0/docs/images/
--rw-r--r--   0 runner    (1001) docker     (127)    99678 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/docs/images/dls-favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)     1750 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/docs/images/dls-logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)      707 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 13:04:03.711488 dls-dodal-1.8.0/docs/user/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 13:04:03.711488 dls-dodal-1.8.0/docs/user/explanations/
--rw-r--r--   0 runner    (1001) docker     (127)      664 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/docs/user/explanations/docs-structure.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 13:04:03.711488 dls-dodal-1.8.0/docs/user/how-to/
--rw-r--r--   0 runner    (1001) docker     (127)      449 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/docs/user/how-to/run-container.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1242 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/docs/user/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 13:04:03.711488 dls-dodal-1.8.0/docs/user/reference/
--rw-r--r--   0 runner    (1001) docker     (127)      252 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/docs/user/reference/api.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 13:04:03.711488 dls-dodal-1.8.0/docs/user/tutorials/
--rw-r--r--   0 runner    (1001) docker     (127)     1807 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/docs/user/tutorials/get_started.rst
--rw-r--r--   0 runner    (1001) docker     (127)      992 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/docs/user/tutorials/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)      336 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/pull_request_template.md
--rw-r--r--   0 runner    (1001) docker     (127)     3643 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-06 13:04:03.739488 dls-dodal-1.8.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 13:04:03.711488 dls-dodal-1.8.0/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 13:04:03.735488 dls-dodal-1.8.0/src/dls_dodal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16254 2023-12-06 13:04:03.000000 dls-dodal-1.8.0/src/dls_dodal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7253 2023-12-06 13:04:03.000000 dls-dodal-1.8.0/src/dls_dodal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-06 13:04:03.000000 dls-dodal-1.8.0/src/dls_dodal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      338 2023-12-06 13:04:03.000000 dls-dodal-1.8.0/src/dls_dodal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2023-12-06 13:04:03.000000 dls-dodal-1.8.0/src/dls_dodal.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 13:04:03.715488 dls-dodal-1.8.0/src/dodal/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/src/dodal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      316 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/src/dodal/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2023-12-06 13:04:03.000000 dls-dodal-1.8.0/src/dodal/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/src/dodal/adsim.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 13:04:03.715488 dls-dodal-1.8.0/src/dodal/beamlines/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/src/dodal/beamlines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3904 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/src/dodal/beamlines/beamline_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10816 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/src/dodal/beamlines/i03.py
--rw-r--r--   0 runner    (1001) docker     (127)    11995 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/src/dodal/beamlines/i04.py
--rw-r--r--   0 runner    (1001) docker     (127)     4749 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/src/dodal/beamlines/i04_1.py
--rw-r--r--   0 runner    (1001) docker     (127)     1388 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/src/dodal/beamlines/i23.py
--rw-r--r--   0 runner    (1001) docker     (127)     4554 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/src/dodal/beamlines/i24.py
--rw-r--r--   0 runner    (1001) docker     (127)      390 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/src/dodal/beamlines/p38.py
--rw-r--r--   0 runner    (1001) docker     (127)      729 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/src/dodal/beamlines/p45.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 13:04:03.723488 dls-dodal-1.8.0/src/dodal/devices/
--rw-r--r--   0 runner    (1001) docker     (127)     1777 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/src/dodal/devices/CTAB.py
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/src/dodal/devices/DCM.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/src/dodal/devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      371 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/src/dodal/devices/adsim.py
--rw-r--r--   0 runner    (1001) docker     (127)      358 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/src/dodal/devices/aperture.py
--rw-r--r--   0 runner    (1001) docker     (127)     5447 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/src/dodal/devices/aperturescatterguard.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 13:04:03.723488 dls-dodal-1.8.0/src/dodal/devices/areadetector/
--rw-r--r--   0 runner    (1001) docker     (127)      240 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/src/dodal/devices/areadetector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3825 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/src/dodal/devices/areadetector/adaravis.py
--rw-r--r--   0 runner    (1001) docker     (127)     1959 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/src/dodal/devices/areadetector/adsim.py
--rw-r--r--   0 runner    (1001) docker     (127)     2576 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/src/dodal/devices/areadetector/adutils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 13:04:03.723488 dls-dodal-1.8.0/src/dodal/devices/areadetector/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)     1706 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/src/dodal/devices/areadetector/plugins/MJPG.py
--rw-r--r--   0 runner    (1001) docker     (127)     5289 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/src/dodal/devices/areadetector/plugins/MXSC.py
--rw-r--r--   0 runner    (1001) docker     (127)     6124 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/src/dodal/devices/attenuator.py
--rw-r--r--   0 runner    (1001) docker     (127)      588 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/src/dodal/devices/backlight.py
--rw-r--r--   0 runner    (1001) docker     (127)      251 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/src/dodal/devices/beamstop.py
--rw-r--r--   0 runner    (1001) docker     (127)      388 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/src/dodal/devices/cryostream.py
--rw-r--r--   0 runner    (1001) docker     (127)     2253 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/src/dodal/devices/det_dim_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1937 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/src/dodal/devices/det_dist_to_beam_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4883 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/src/dodal/devices/detector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/src/dodal/devices/detector_motion.py
--rw-r--r--   0 runner    (1001) docker     (127)    12659 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/src/dodal/devices/eiger.py
--rw-r--r--   0 runner    (1001) docker     (127)     7236 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/src/dodal/devices/eiger_odin.py
--rw-r--r--   0 runner    (1001) docker     (127)    11150 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/src/dodal/devices/fast_grid_scan.py
--rw-r--r--   0 runner    (1001) docker     (127)      194 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/src/dodal/devices/fluorescence_detector_motion.py
--rw-r--r--   0 runner    (1001) docker     (127)      213 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/src/dodal/devices/flux.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 13:04:03.723488 dls-dodal-1.8.0/src/dodal/devices/i03/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/src/dodal/devices/i03/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 13:04:03.723488 dls-dodal-1.8.0/src/dodal/devices/i04/
--rw-r--r--   0 runner    (1001) docker     (127)     3236 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/src/dodal/devices/i04/transfocator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 13:04:03.723488 dls-dodal-1.8.0/src/dodal/devices/i23/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/src/dodal/devices/i23/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      936 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/src/dodal/devices/i23/gonio.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 13:04:03.723488 dls-dodal-1.8.0/src/dodal/devices/i24/
--rw-r--r--   0 runner    (1001) docker     (127)      253 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/src/dodal/devices/i24/I24_detector_motion.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/src/dodal/devices/i24/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1427 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/src/dodal/devices/i24/dual_backlight.py
--rw-r--r--   0 runner    (1001) docker     (127)      569 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/src/dodal/devices/i24/i24_vgonio.py
--rw-r--r--   0 runner    (1001) docker     (127)      223 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/src/dodal/devices/i24/pmac.py
--rw-r--r--   0 runner    (1001) docker     (127)      223 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/src/dodal/devices/ipin.py
--rw-r--r--   0 runner    (1001) docker     (127)      666 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/src/dodal/devices/logging_ophyd_device.py
--rw-r--r--   0 runner    (1001) docker     (127)      265 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/src/dodal/devices/lower_gonio_stages.py
--rw-r--r--   0 runner    (1001) docker     (127)     1262 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/src/dodal/devices/motors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 13:04:03.723488 dls-dodal-1.8.0/src/dodal/devices/oav/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/src/dodal/devices/oav/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5053 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/src/dodal/devices/oav/grid_overlay.py
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/src/dodal/devices/oav/microns_for_zoom_levels.json
--rw-r--r--   0 runner    (1001) docker     (127)    13804 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/src/dodal/devices/oav/oav_calculations.py
--rw-r--r--   0 runner    (1001) docker     (127)     7186 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/src/dodal/devices/oav/oav_detector.py
--rw-r--r--   0 runner    (1001) docker     (127)      753 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/src/dodal/devices/oav/oav_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     3366 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/src/dodal/devices/oav/oav_parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 13:04:03.727488 dls-dodal-1.8.0/src/dodal/devices/oav/pin_image_recognition/
--rw-r--r--   0 runner    (1001) docker     (127)     5877 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/src/dodal/devices/oav/pin_image_recognition/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      902 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/src/dodal/devices/oav/pin_image_recognition/manual_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8823 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/src/dodal/devices/oav/pin_image_recognition/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      999 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/src/dodal/devices/oav/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/src/dodal/devices/p45.py
--rw-r--r--   0 runner    (1001) docker     (127)      193 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/src/dodal/devices/qbpm1.py
--rw-r--r--   0 runner    (1001) docker     (127)      180 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/src/dodal/devices/robot.py
--rw-r--r--   0 runner    (1001) docker     (127)      267 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/src/dodal/devices/s4_slit_gaps.py
--rw-r--r--   0 runner    (1001) docker     (127)      687 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/src/dodal/devices/sample_shutter.py
--rw-r--r--   0 runner    (1001) docker     (127)      184 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/src/dodal/devices/scatterguard.py
--rw-r--r--   0 runner    (1001) docker     (127)      208 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/src/dodal/devices/scintillator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3007 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/src/dodal/devices/smargon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1223 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/src/dodal/devices/status.py
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/src/dodal/devices/synchrotron.py
--rw-r--r--   0 runner    (1001) docker     (127)      926 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/src/dodal/devices/undulator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2748 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/src/dodal/devices/undulator_dcm.py
--rw-r--r--   0 runner    (1001) docker     (127)     4382 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/src/dodal/devices/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1652 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/src/dodal/devices/xbpm_feedback.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 13:04:03.727488 dls-dodal-1.8.0/src/dodal/devices/xspress3_mini/
--rw-r--r--   0 runner    (1001) docker     (127)     3034 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/src/dodal/devices/xspress3_mini/xspress3_mini.py
--rw-r--r--   0 runner    (1001) docker     (127)      810 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/src/dodal/devices/xspress3_mini/xspress3_mini_channel.py
--rw-r--r--   0 runner    (1001) docker     (127)     8155 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/src/dodal/devices/zebra.py
--rw-r--r--   0 runner    (1001) docker     (127)     7212 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/src/dodal/log.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 13:04:03.727488 dls-dodal-1.8.0/src/dodal/parameters/
--rw-r--r--   0 runner    (1001) docker     (127)      145 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/src/dodal/parameters/experiment_parameter_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6682 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/src/dodal/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 13:04:03.727488 dls-dodal-1.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 13:04:03.703488 dls-dodal-1.8.0/tests/beamlines/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 13:04:03.727488 dls-dodal-1.8.0/tests/beamlines/unit_tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3469 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/tests/beamlines/unit_tests/test_beamline_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1708 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/tests/beamlines/unit_tests/test_i03.py
--rw-r--r--   0 runner    (1001) docker     (127)      377 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/tests/beamlines/unit_tests/test_i04.py
--rw-r--r--   0 runner    (1001) docker     (127)      878 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/tests/beamlines/unit_tests/test_i24.py
--rw-r--r--   0 runner    (1001) docker     (127)     1305 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 13:04:03.703488 dls-dodal-1.8.0/tests/devices/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 13:04:03.727488 dls-dodal-1.8.0/tests/devices/i04/
--rw-r--r--   0 runner    (1001) docker     (127)     2062 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/tests/devices/i04/test_transfocator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 13:04:03.731488 dls-dodal-1.8.0/tests/devices/system_tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/tests/devices/system_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5376 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/tests/devices/system_tests/test_aperturescatterguard_system.py
--rw-r--r--   0 runner    (1001) docker     (127)     1215 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/tests/devices/system_tests/test_eiger_system.py
--rw-r--r--   0 runner    (1001) docker     (127)     2645 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/tests/devices/system_tests/test_gridscan_system.py
--rw-r--r--   0 runner    (1001) docker     (127)     1579 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/tests/devices/system_tests/test_oav_system.py
--rw-r--r--   0 runner    (1001) docker     (127)      255 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/tests/devices/system_tests/test_slit_gaps_system.py
--rw-r--r--   0 runner    (1001) docker     (127)      232 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/tests/devices/system_tests/test_smargon_system.py
--rw-r--r--   0 runner    (1001) docker     (127)      293 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/tests/devices/system_tests/test_synchrotron_system.py
--rw-r--r--   0 runner    (1001) docker     (127)      328 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/tests/devices/system_tests/test_undulator_system.py
--rw-r--r--   0 runner    (1001) docker     (127)      664 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/tests/devices/system_tests/test_zebra_system.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 13:04:03.735488 dls-dodal-1.8.0/tests/devices/unit_tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/tests/devices/unit_tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 13:04:03.735488 dls-dodal-1.8.0/tests/devices/unit_tests/i24/
--rw-r--r--   0 runner    (1001) docker     (127)     1413 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/tests/devices/unit_tests/i24/test_dual_backlight.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 13:04:03.735488 dls-dodal-1.8.0/tests/devices/unit_tests/oav/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/tests/devices/unit_tests/oav/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 13:04:03.735488 dls-dodal-1.8.0/tests/devices/unit_tests/oav/image_recognition/
--rw-r--r--   0 runner    (1001) docker     (127)     3015 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/tests/devices/unit_tests/oav/image_recognition/test_pin_tip_detect.py
--rw-r--r--   0 runner    (1001) docker     (127)     5216 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/tests/devices/unit_tests/oav/image_recognition/test_pin_tip_detect_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3778 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/tests/devices/unit_tests/oav/test_oav.py
--rw-r--r--   0 runner    (1001) docker     (127)     1467 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/tests/devices/unit_tests/oav/test_oav_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1821 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/tests/devices/unit_tests/test_OAVCentring.json
--rw-r--r--   0 runner    (1001) docker     (127)      369 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/tests/devices/unit_tests/test_aperture.py
--rw-r--r--   0 runner    (1001) docker     (127)     1788 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/tests/devices/unit_tests/test_aperture_scatterguard.py
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/tests/devices/unit_tests/test_attenuator.py
--rw-r--r--   0 runner    (1001) docker     (127)      939 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/tests/devices/unit_tests/test_backlight.py
--rw-r--r--   0 runner    (1001) docker     (127)     3333 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/tests/devices/unit_tests/test_beam_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1018 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/tests/devices/unit_tests/test_beamline_undulator_to_gap_lookup_table.txt
--rw-r--r--   0 runner    (1001) docker     (127)      426 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/tests/devices/unit_tests/test_det_dim_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1652 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/tests/devices/unit_tests/test_detector.py
--rw-r--r--   0 runner    (1001) docker     (127)      705 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/tests/devices/unit_tests/test_display.configuration
--rw-r--r--   0 runner    (1001) docker     (127)    20458 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/tests/devices/unit_tests/test_eiger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2889 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/tests/devices/unit_tests/test_grid_overlay.py
--rw-r--r--   0 runner    (1001) docker     (127)    10241 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/tests/devices/unit_tests/test_gridscan.py
--rw-r--r--   0 runner    (1001) docker     (127)     1227 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/tests/devices/unit_tests/test_jCameraManZoomLevels.xml
--rw-r--r--   0 runner    (1001) docker     (127)      108 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/tests/devices/unit_tests/test_lookup_table.txt
--rw-r--r--   0 runner    (1001) docker     (127)      108 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/tests/devices/unit_tests/test_lookup_table_2.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/tests/devices/unit_tests/test_motors.py
--rw-r--r--   0 runner    (1001) docker     (127)     4871 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/tests/devices/unit_tests/test_oav.py
--rw-r--r--   0 runner    (1001) docker     (127)     8285 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/tests/devices/unit_tests/test_oav_centring.py
--rw-r--r--   0 runner    (1001) docker     (127)     3607 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/tests/devices/unit_tests/test_odin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4231 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/tests/devices/unit_tests/test_pin_tip_detect.py
--rw-r--r--   0 runner    (1001) docker     (127)      774 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/tests/devices/unit_tests/test_sample_shutter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1940 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/tests/devices/unit_tests/test_smargon.py
--rw-r--r--   0 runner    (1001) docker     (127)      863 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/tests/devices/unit_tests/test_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     4099 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/tests/devices/unit_tests/test_undulator_dcm.py
--rw-r--r--   0 runner    (1001) docker     (127)     3660 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/tests/devices/unit_tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      870 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/tests/devices/unit_tests/test_xbpm_feedback.py
--rw-r--r--   0 runner    (1001) docker     (127)     1665 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/tests/devices/unit_tests/test_xspress3mini.py
--rw-r--r--   0 runner    (1001) docker     (127)     3214 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/tests/devices/unit_tests/test_zebra.py
--rw-r--r--   0 runner    (1001) docker     (127)      493 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/tests/fake_beamline.py
--rw-r--r--   0 runner    (1001) docker     (127)      493 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/tests/fake_beamline_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (127)      493 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/tests/fake_beamline_disordered_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (127)     1259 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/tests/fake_beamline_misbehaving_builtins.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 13:04:03.735488 dls-dodal-1.8.0/tests/system_tests/
--rw-r--r--   0 runner    (1001) docker     (127)      657 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/tests/system_tests/test_i03_system.py
--rw-r--r--   0 runner    (1001) docker     (127)      797 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/tests/system_tests/test_i04_1_system.py
--rw-r--r--   0 runner    (1001) docker     (127)      657 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/tests/system_tests/test_i04_system.py
--rw-r--r--   0 runner    (1001) docker     (127)      899 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/tests/system_tests/test_i23_system.py
--rw-r--r--   0 runner    (1001) docker     (127)      657 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/tests/system_tests/test_i24_system.py
--rw-r--r--   0 runner    (1001) docker     (127)      434 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/tests/system_tests/test_s03_system.py
--rw-r--r--   0 runner    (1001) docker     (127)     2481 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-06 13:04:03.735488 dls-dodal-1.8.0/tests/unit_tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5368 2023-12-06 13:03:55.000000 dls-dodal-1.8.0/tests/unit_tests/test_log.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 14:00:53.652333 dls-dodal-1.9.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 14:00:53.620333 dls-dodal-1.9.0/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (127)     2140 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 14:00:53.620333 dls-dodal-1.9.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/.github/CONTRIBUTING.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 14:00:53.620333 dls-dodal-1.9.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/.github/ISSUE_TEMPLATE/issue_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 14:00:53.616333 dls-dodal-1.9.0/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 14:00:53.620333 dls-dodal-1.9.0/.github/actions/install_requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)     2060 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/.github/actions/install_requirements/action.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 14:00:53.620333 dls-dodal-1.9.0/.github/pages/
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/.github/pages/index.html
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3025 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/.github/pages/make_switcher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 14:00:53.624333 dls-dodal-1.9.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     6590 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/.github/workflows/code.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1863 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/.github/workflows/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/.github/workflows/docs_clean.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/.github/workflows/linkcheck.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 14:00:53.624333 dls-dodal-1.9.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    16247 2023-12-12 14:00:53.652333 dls-dodal-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1657 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 14:00:53.624333 dls-dodal-1.9.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     6505 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 14:00:53.624333 dls-dodal-1.9.0/docs/developer/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 14:00:53.624333 dls-dodal-1.9.0/docs/developer/explanations/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 14:00:53.624333 dls-dodal-1.9.0/docs/developer/explanations/decisions/
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/docs/developer/explanations/decisions/0001-record-architecture-decisions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/docs/developer/explanations/decisions.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 14:00:53.624333 dls-dodal-1.9.0/docs/developer/how-to/
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/docs/developer/how-to/build-docs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/docs/developer/how-to/contribute.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/docs/developer/how-to/lint.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/docs/developer/how-to/make-release.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2899 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/docs/developer/how-to/move-code.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/docs/developer/how-to/run-tests.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/docs/developer/how-to/static-analysis.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/docs/developer/how-to/update-tools.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/docs/developer/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 14:00:53.624333 dls-dodal-1.9.0/docs/developer/reference/
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/docs/developer/reference/standards.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 14:00:53.624333 dls-dodal-1.9.0/docs/developer/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/docs/developer/tutorials/dev-install.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/docs/genindex.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 14:00:53.624333 dls-dodal-1.9.0/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    99678 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/docs/images/dls-favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/docs/images/dls-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 14:00:53.624333 dls-dodal-1.9.0/docs/user/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 14:00:53.624333 dls-dodal-1.9.0/docs/user/explanations/
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/docs/user/explanations/docs-structure.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 14:00:53.628333 dls-dodal-1.9.0/docs/user/how-to/
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/docs/user/how-to/run-container.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1242 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/docs/user/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 14:00:53.628333 dls-dodal-1.9.0/docs/user/reference/
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/docs/user/reference/api.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 14:00:53.628333 dls-dodal-1.9.0/docs/user/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (127)     1807 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/docs/user/tutorials/get_started.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/docs/user/tutorials/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/pull_request_template.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3636 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-12 14:00:53.652333 dls-dodal-1.9.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 14:00:53.628333 dls-dodal-1.9.0/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 14:00:53.652333 dls-dodal-1.9.0/src/dls_dodal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16247 2023-12-12 14:00:53.000000 dls-dodal-1.9.0/src/dls_dodal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7253 2023-12-12 14:00:53.000000 dls-dodal-1.9.0/src/dls_dodal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-12 14:00:53.000000 dls-dodal-1.9.0/src/dls_dodal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2023-12-12 14:00:53.000000 dls-dodal-1.9.0/src/dls_dodal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2023-12-12 14:00:53.000000 dls-dodal-1.9.0/src/dls_dodal.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 14:00:53.628333 dls-dodal-1.9.0/src/dodal/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/src/dodal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/src/dodal/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2023-12-12 14:00:53.000000 dls-dodal-1.9.0/src/dodal/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/src/dodal/adsim.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 14:00:53.628333 dls-dodal-1.9.0/src/dodal/beamlines/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/src/dodal/beamlines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3904 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/src/dodal/beamlines/beamline_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10816 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/src/dodal/beamlines/i03.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11995 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/src/dodal/beamlines/i04.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4749 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/src/dodal/beamlines/i04_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/src/dodal/beamlines/i23.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4554 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/src/dodal/beamlines/i24.py
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/src/dodal/beamlines/p38.py
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/src/dodal/beamlines/p45.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 14:00:53.636333 dls-dodal-1.9.0/src/dodal/devices/
+-rw-r--r--   0 runner    (1001) docker     (127)     1777 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/src/dodal/devices/CTAB.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/src/dodal/devices/DCM.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/src/dodal/devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/src/dodal/devices/adsim.py
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/src/dodal/devices/aperture.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5447 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/src/dodal/devices/aperturescatterguard.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 14:00:53.636333 dls-dodal-1.9.0/src/dodal/devices/areadetector/
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/src/dodal/devices/areadetector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3825 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/src/dodal/devices/areadetector/adaravis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1959 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/src/dodal/devices/areadetector/adsim.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2576 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/src/dodal/devices/areadetector/adutils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 14:00:53.636333 dls-dodal-1.9.0/src/dodal/devices/areadetector/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)     1706 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/src/dodal/devices/areadetector/plugins/MJPG.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5289 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/src/dodal/devices/areadetector/plugins/MXSC.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6124 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/src/dodal/devices/attenuator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/src/dodal/devices/backlight.py
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/src/dodal/devices/beamstop.py
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/src/dodal/devices/cryostream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2253 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/src/dodal/devices/det_dim_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1937 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/src/dodal/devices/det_dist_to_beam_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4883 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/src/dodal/devices/detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/src/dodal/devices/detector_motion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12659 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/src/dodal/devices/eiger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7236 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/src/dodal/devices/eiger_odin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11150 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/src/dodal/devices/fast_grid_scan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/src/dodal/devices/fluorescence_detector_motion.py
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/src/dodal/devices/flux.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 14:00:53.636333 dls-dodal-1.9.0/src/dodal/devices/i03/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/src/dodal/devices/i03/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 14:00:53.636333 dls-dodal-1.9.0/src/dodal/devices/i04/
+-rw-r--r--   0 runner    (1001) docker     (127)     3236 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/src/dodal/devices/i04/transfocator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 14:00:53.636333 dls-dodal-1.9.0/src/dodal/devices/i23/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/src/dodal/devices/i23/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/src/dodal/devices/i23/gonio.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 14:00:53.636333 dls-dodal-1.9.0/src/dodal/devices/i24/
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/src/dodal/devices/i24/I24_detector_motion.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/src/dodal/devices/i24/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1427 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/src/dodal/devices/i24/dual_backlight.py
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/src/dodal/devices/i24/i24_vgonio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/src/dodal/devices/i24/pmac.py
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/src/dodal/devices/ipin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/src/dodal/devices/logging_ophyd_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/src/dodal/devices/lower_gonio_stages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1262 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/src/dodal/devices/motors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 14:00:53.640333 dls-dodal-1.9.0/src/dodal/devices/oav/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/src/dodal/devices/oav/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5053 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/src/dodal/devices/oav/grid_overlay.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/src/dodal/devices/oav/microns_for_zoom_levels.json
+-rw-r--r--   0 runner    (1001) docker     (127)    13804 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/src/dodal/devices/oav/oav_calculations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8143 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/src/dodal/devices/oav/oav_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/src/dodal/devices/oav/oav_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3366 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/src/dodal/devices/oav/oav_parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 14:00:53.640333 dls-dodal-1.9.0/src/dodal/devices/oav/pin_image_recognition/
+-rw-r--r--   0 runner    (1001) docker     (127)     5877 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/src/dodal/devices/oav/pin_image_recognition/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/src/dodal/devices/oav/pin_image_recognition/manual_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8823 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/src/dodal/devices/oav/pin_image_recognition/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/src/dodal/devices/oav/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/src/dodal/devices/p45.py
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/src/dodal/devices/qbpm1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/src/dodal/devices/robot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/src/dodal/devices/s4_slit_gaps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/src/dodal/devices/sample_shutter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/src/dodal/devices/scatterguard.py
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/src/dodal/devices/scintillator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3007 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/src/dodal/devices/smargon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1223 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/src/dodal/devices/status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/src/dodal/devices/synchrotron.py
+-rw-r--r--   0 runner    (1001) docker     (127)      926 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/src/dodal/devices/undulator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2748 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/src/dodal/devices/undulator_dcm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4382 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/src/dodal/devices/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1652 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/src/dodal/devices/xbpm_feedback.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 14:00:53.640333 dls-dodal-1.9.0/src/dodal/devices/xspress3_mini/
+-rw-r--r--   0 runner    (1001) docker     (127)     3034 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/src/dodal/devices/xspress3_mini/xspress3_mini.py
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/src/dodal/devices/xspress3_mini/xspress3_mini_channel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8155 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/src/dodal/devices/zebra.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7212 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/src/dodal/log.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 14:00:53.640333 dls-dodal-1.9.0/src/dodal/parameters/
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/src/dodal/parameters/experiment_parameter_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6682 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/src/dodal/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 14:00:53.640333 dls-dodal-1.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 14:00:53.620333 dls-dodal-1.9.0/tests/beamlines/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 14:00:53.640333 dls-dodal-1.9.0/tests/beamlines/unit_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3469 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/tests/beamlines/unit_tests/test_beamline_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1708 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/tests/beamlines/unit_tests/test_i03.py
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/tests/beamlines/unit_tests/test_i04.py
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/tests/beamlines/unit_tests/test_i24.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 14:00:53.620333 dls-dodal-1.9.0/tests/devices/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 14:00:53.640333 dls-dodal-1.9.0/tests/devices/i04/
+-rw-r--r--   0 runner    (1001) docker     (127)     2062 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/tests/devices/i04/test_transfocator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 14:00:53.644333 dls-dodal-1.9.0/tests/devices/system_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/tests/devices/system_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5376 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/tests/devices/system_tests/test_aperturescatterguard_system.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/tests/devices/system_tests/test_eiger_system.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2645 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/tests/devices/system_tests/test_gridscan_system.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1579 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/tests/devices/system_tests/test_oav_system.py
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/tests/devices/system_tests/test_slit_gaps_system.py
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/tests/devices/system_tests/test_smargon_system.py
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/tests/devices/system_tests/test_synchrotron_system.py
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/tests/devices/system_tests/test_undulator_system.py
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/tests/devices/system_tests/test_zebra_system.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 14:00:53.648333 dls-dodal-1.9.0/tests/devices/unit_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/tests/devices/unit_tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 14:00:53.648333 dls-dodal-1.9.0/tests/devices/unit_tests/i24/
+-rw-r--r--   0 runner    (1001) docker     (127)     1413 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/tests/devices/unit_tests/i24/test_dual_backlight.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 14:00:53.648333 dls-dodal-1.9.0/tests/devices/unit_tests/oav/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/tests/devices/unit_tests/oav/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 14:00:53.648333 dls-dodal-1.9.0/tests/devices/unit_tests/oav/image_recognition/
+-rw-r--r--   0 runner    (1001) docker     (127)     3015 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/tests/devices/unit_tests/oav/image_recognition/test_pin_tip_detect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5216 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/tests/devices/unit_tests/oav/image_recognition/test_pin_tip_detect_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4625 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/tests/devices/unit_tests/oav/test_oav.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1478 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/tests/devices/unit_tests/oav/test_oav_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1821 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/tests/devices/unit_tests/test_OAVCentring.json
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/tests/devices/unit_tests/test_aperture.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8459 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/tests/devices/unit_tests/test_aperture_scatterguard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/tests/devices/unit_tests/test_attenuator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/tests/devices/unit_tests/test_backlight.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3333 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/tests/devices/unit_tests/test_beam_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/tests/devices/unit_tests/test_beamline_undulator_to_gap_lookup_table.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/tests/devices/unit_tests/test_det_dim_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1652 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/tests/devices/unit_tests/test_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/tests/devices/unit_tests/test_display.configuration
+-rw-r--r--   0 runner    (1001) docker     (127)    20458 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/tests/devices/unit_tests/test_eiger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2889 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/tests/devices/unit_tests/test_grid_overlay.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10241 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/tests/devices/unit_tests/test_gridscan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/tests/devices/unit_tests/test_jCameraManZoomLevels.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/tests/devices/unit_tests/test_lookup_table.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/tests/devices/unit_tests/test_lookup_table_2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/tests/devices/unit_tests/test_motors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4871 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/tests/devices/unit_tests/test_oav.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8364 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/tests/devices/unit_tests/test_oav_centring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3607 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/tests/devices/unit_tests/test_odin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4231 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/tests/devices/unit_tests/test_pin_tip_detect.py
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/tests/devices/unit_tests/test_sample_shutter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1940 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/tests/devices/unit_tests/test_smargon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/tests/devices/unit_tests/test_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4099 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/tests/devices/unit_tests/test_undulator_dcm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3660 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/tests/devices/unit_tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/tests/devices/unit_tests/test_xbpm_feedback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/tests/devices/unit_tests/test_xspress3mini.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3214 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/tests/devices/unit_tests/test_zebra.py
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/tests/fake_beamline.py
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/tests/fake_beamline_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/tests/fake_beamline_disordered_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1259 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/tests/fake_beamline_misbehaving_builtins.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 14:00:53.652333 dls-dodal-1.9.0/tests/system_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/tests/system_tests/test_i03_system.py
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/tests/system_tests/test_i04_1_system.py
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/tests/system_tests/test_i04_system.py
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/tests/system_tests/test_i23_system.py
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/tests/system_tests/test_i24_system.py
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/tests/system_tests/test_s03_system.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2481 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 14:00:53.652333 dls-dodal-1.9.0/tests/unit_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5368 2023-12-12 14:00:47.000000 dls-dodal-1.9.0/tests/unit_tests/test_log.py
```

### Comparing `dls-dodal-1.8.0/.devcontainer/devcontainer.json` & `dls-dodal-1.9.0/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/.github/CONTRIBUTING.rst` & `dls-dodal-1.9.0/.github/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/.github/actions/install_requirements/action.yml` & `dls-dodal-1.9.0/.github/actions/install_requirements/action.yml`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/.github/dependabot.yml` & `dls-dodal-1.9.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/.github/pages/make_switcher.py` & `dls-dodal-1.9.0/.github/pages/make_switcher.py`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/.github/workflows/code.yml` & `dls-dodal-1.9.0/.github/workflows/code.yml`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/.github/workflows/docs.yml` & `dls-dodal-1.9.0/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/.github/workflows/docs_clean.yml` & `dls-dodal-1.9.0/.github/workflows/docs_clean.yml`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/.github/workflows/linkcheck.yml` & `dls-dodal-1.9.0/.github/workflows/linkcheck.yml`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/.gitignore` & `dls-dodal-1.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/.pre-commit-config.yaml` & `dls-dodal-1.9.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/.vscode/launch.json` & `dls-dodal-1.9.0/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/.vscode/settings.json` & `dls-dodal-1.9.0/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/Dockerfile` & `dls-dodal-1.9.0/Dockerfile`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/LICENSE` & `dls-dodal-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/PKG-INFO` & `dls-dodal-1.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dls-dodal
-Version: 1.8.0
+Version: 1.9.0
 Summary: Ophyd devices and other utils that could be used across DLS beamlines
 Author-email: Dominic Oram <dominic.oram@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -211,15 +211,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: ophyd
-Requires-Dist: ophyd-async==0.1.0
+Requires-Dist: ophyd-async
 Requires-Dist: bluesky
 Requires-Dist: pyepics
 Requires-Dist: dataclasses-json
 Requires-Dist: pillow
 Requires-Dist: requests
 Requires-Dist: graypy
 Requires-Dist: pydantic<2.0
```

### Comparing `dls-dodal-1.8.0/README.rst` & `dls-dodal-1.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/docs/conf.py` & `dls-dodal-1.9.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/docs/developer/explanations/decisions.rst` & `dls-dodal-1.9.0/docs/developer/explanations/decisions.rst`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/docs/developer/how-to/build-docs.rst` & `dls-dodal-1.9.0/docs/developer/how-to/build-docs.rst`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/docs/developer/how-to/lint.rst` & `dls-dodal-1.9.0/docs/developer/how-to/lint.rst`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/docs/developer/how-to/make-release.rst` & `dls-dodal-1.9.0/docs/developer/how-to/make-release.rst`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/docs/developer/how-to/move-code.rst` & `dls-dodal-1.9.0/docs/developer/how-to/move-code.rst`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/docs/developer/how-to/update-tools.rst` & `dls-dodal-1.9.0/docs/developer/how-to/update-tools.rst`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/docs/developer/index.rst` & `dls-dodal-1.9.0/docs/developer/index.rst`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/docs/developer/reference/standards.rst` & `dls-dodal-1.9.0/docs/developer/reference/standards.rst`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/docs/developer/tutorials/dev-install.rst` & `dls-dodal-1.9.0/docs/developer/tutorials/dev-install.rst`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/docs/images/dls-favicon.ico` & `dls-dodal-1.9.0/docs/images/dls-favicon.ico`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/docs/images/dls-logo.svg` & `dls-dodal-1.9.0/docs/images/dls-logo.svg`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/docs/index.rst` & `dls-dodal-1.9.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/docs/user/explanations/docs-structure.rst` & `dls-dodal-1.9.0/docs/user/explanations/docs-structure.rst`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/docs/user/index.rst` & `dls-dodal-1.9.0/docs/user/index.rst`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/docs/user/tutorials/get_started.rst` & `dls-dodal-1.9.0/docs/user/tutorials/get_started.rst`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/docs/user/tutorials/installation.rst` & `dls-dodal-1.9.0/docs/user/tutorials/installation.rst`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/pyproject.toml` & `dls-dodal-1.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 description = "Ophyd devices and other utils that could be used across DLS beamlines"
 dependencies = [
     "ophyd",
-    "ophyd-async==0.1.0",
+    "ophyd-async",
     "bluesky",
     "pyepics",
     "dataclasses-json",
     "pillow",
     "requests",
     "graypy",
     "pydantic<2.0",
```

### Comparing `dls-dodal-1.8.0/src/dls_dodal.egg-info/PKG-INFO` & `dls-dodal-1.9.0/src/dls_dodal.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dls-dodal
-Version: 1.8.0
+Version: 1.9.0
 Summary: Ophyd devices and other utils that could be used across DLS beamlines
 Author-email: Dominic Oram <dominic.oram@diamond.ac.uk>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -211,15 +211,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: ophyd
-Requires-Dist: ophyd-async==0.1.0
+Requires-Dist: ophyd-async
 Requires-Dist: bluesky
 Requires-Dist: pyepics
 Requires-Dist: dataclasses-json
 Requires-Dist: pillow
 Requires-Dist: requests
 Requires-Dist: graypy
 Requires-Dist: pydantic<2.0
```

### Comparing `dls-dodal-1.8.0/src/dls_dodal.egg-info/SOURCES.txt` & `dls-dodal-1.9.0/src/dls_dodal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/src/dodal/beamlines/beamline_utils.py` & `dls-dodal-1.9.0/src/dodal/beamlines/beamline_utils.py`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/src/dodal/beamlines/i03.py` & `dls-dodal-1.9.0/src/dodal/beamlines/i03.py`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/src/dodal/beamlines/i04.py` & `dls-dodal-1.9.0/src/dodal/beamlines/i04.py`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/src/dodal/beamlines/i04_1.py` & `dls-dodal-1.9.0/src/dodal/beamlines/i04_1.py`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/src/dodal/beamlines/i23.py` & `dls-dodal-1.9.0/src/dodal/beamlines/i23.py`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/src/dodal/beamlines/i24.py` & `dls-dodal-1.9.0/src/dodal/beamlines/i24.py`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/src/dodal/beamlines/p45.py` & `dls-dodal-1.9.0/src/dodal/beamlines/p45.py`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/src/dodal/devices/CTAB.py` & `dls-dodal-1.9.0/src/dodal/devices/CTAB.py`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/src/dodal/devices/DCM.py` & `dls-dodal-1.9.0/src/dodal/devices/DCM.py`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/src/dodal/devices/aperturescatterguard.py` & `dls-dodal-1.9.0/src/dodal/devices/aperturescatterguard.py`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/src/dodal/devices/areadetector/adaravis.py` & `dls-dodal-1.9.0/src/dodal/devices/areadetector/adaravis.py`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/src/dodal/devices/areadetector/adsim.py` & `dls-dodal-1.9.0/src/dodal/devices/areadetector/adsim.py`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/src/dodal/devices/areadetector/adutils.py` & `dls-dodal-1.9.0/src/dodal/devices/areadetector/adutils.py`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/src/dodal/devices/areadetector/plugins/MJPG.py` & `dls-dodal-1.9.0/src/dodal/devices/areadetector/plugins/MJPG.py`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/src/dodal/devices/areadetector/plugins/MXSC.py` & `dls-dodal-1.9.0/src/dodal/devices/areadetector/plugins/MXSC.py`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/src/dodal/devices/attenuator.py` & `dls-dodal-1.9.0/src/dodal/devices/attenuator.py`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/src/dodal/devices/backlight.py` & `dls-dodal-1.9.0/src/dodal/devices/backlight.py`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/src/dodal/devices/det_dim_constants.py` & `dls-dodal-1.9.0/src/dodal/devices/det_dim_constants.py`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/src/dodal/devices/det_dist_to_beam_converter.py` & `dls-dodal-1.9.0/src/dodal/devices/det_dist_to_beam_converter.py`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/src/dodal/devices/detector.py` & `dls-dodal-1.9.0/src/dodal/devices/detector.py`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/src/dodal/devices/detector_motion.py` & `dls-dodal-1.9.0/src/dodal/devices/detector_motion.py`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/src/dodal/devices/eiger.py` & `dls-dodal-1.9.0/src/dodal/devices/eiger.py`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/src/dodal/devices/eiger_odin.py` & `dls-dodal-1.9.0/src/dodal/devices/eiger_odin.py`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/src/dodal/devices/fast_grid_scan.py` & `dls-dodal-1.9.0/src/dodal/devices/fast_grid_scan.py`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/src/dodal/devices/i04/transfocator.py` & `dls-dodal-1.9.0/src/dodal/devices/i04/transfocator.py`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/src/dodal/devices/i23/gonio.py` & `dls-dodal-1.9.0/src/dodal/devices/i23/gonio.py`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/src/dodal/devices/i24/dual_backlight.py` & `dls-dodal-1.9.0/src/dodal/devices/i24/dual_backlight.py`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/src/dodal/devices/i24/i24_vgonio.py` & `dls-dodal-1.9.0/src/dodal/devices/i24/i24_vgonio.py`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/src/dodal/devices/logging_ophyd_device.py` & `dls-dodal-1.9.0/src/dodal/devices/logging_ophyd_device.py`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/src/dodal/devices/motors.py` & `dls-dodal-1.9.0/src/dodal/devices/motors.py`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/src/dodal/devices/oav/grid_overlay.py` & `dls-dodal-1.9.0/src/dodal/devices/oav/grid_overlay.py`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/src/dodal/devices/oav/microns_for_zoom_levels.json` & `dls-dodal-1.9.0/src/dodal/devices/oav/microns_for_zoom_levels.json`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/src/dodal/devices/oav/oav_calculations.py` & `dls-dodal-1.9.0/src/dodal/devices/oav/oav_calculations.py`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/src/dodal/devices/oav/oav_detector.py` & `dls-dodal-1.9.0/src/dodal/devices/oav/oav_detector.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import xml.etree.cElementTree as et
+from functools import partial
 from typing import Tuple
 
 from ophyd import ADComponent as ADC
 from ophyd import (
     AreaDetector,
     CamBase,
     Component,
@@ -20,14 +21,20 @@
 from dodal.devices.oav.grid_overlay import SnapshotWithGrid
 from dodal.devices.oav.oav_errors import (
     OAVError_BeamPositionNotFound,
     OAVError_ZoomLevelNotFound,
 )
 from dodal.log import LOGGER
 
+# GDA corrently assumes this aspect ratio for the OAV window size.
+# For some beamline this doesn't affect anything as the actual OAV aspect ratio
+# matches. Others need to take it into account to rescale the values stored in
+# the configuration files.
+DEFAULT_OAV_WINDOW = (1024, 768)
+
 
 class ZoomController(Device):
     """
     Device to control the zoom level. This should be set like
         o = OAV(name="oav")
         oav.zoom_controller.set("1.0x")
 
@@ -87,43 +94,56 @@
         self,
         zoom_params_file,
         display_config,
     ):
         self.zoom_params_file: str = zoom_params_file
         self.display_config: str = display_config
 
-    def update_on_zoom(self, value, *args, **kwargs):
+    def update_on_zoom(self, value, xsize, ysize, *args, **kwargs):
+        xsize, ysize = int(xsize), int(ysize)
         if isinstance(value, str) and value.endswith("x"):
             value = value.strip("x")
         zoom = float(value)
-        self.load_microns_per_pixel(zoom)
-        self.beam_centre_i, self.beam_centre_j = self.get_beam_position_from_zoom(zoom)
+        self.load_microns_per_pixel(zoom, xsize, ysize)
+        self.beam_centre_i, self.beam_centre_j = self.get_beam_position_from_zoom(
+            zoom, xsize, ysize
+        )
 
-    def load_microns_per_pixel(self, zoom: float):
+    def load_microns_per_pixel(self, zoom: float, xsize: int, ysize: int):
         """
         Loads the microns per x pixel and y pixel for a given zoom level. These are
         currently generated by GDA, though hyperion could generate them in future.
         """
         tree = et.parse(self.zoom_params_file)
         self.micronsPerXPixel = self.micronsPerYPixel = None
         root = tree.getroot()
         levels = root.findall(".//zoomLevel")
         for node in levels:
             if float(node.find("level").text) == zoom:
-                self.micronsPerXPixel = float(node.find("micronsPerXPixel").text)
-                self.micronsPerYPixel = float(node.find("micronsPerYPixel").text)
+                self.micronsPerXPixel = (
+                    float(node.find("micronsPerXPixel").text)
+                    * DEFAULT_OAV_WINDOW[0]
+                    / xsize
+                )
+                self.micronsPerYPixel = (
+                    float(node.find("micronsPerYPixel").text)
+                    * DEFAULT_OAV_WINDOW[1]
+                    / ysize
+                )
         if self.micronsPerXPixel is None or self.micronsPerYPixel is None:
             raise OAVError_ZoomLevelNotFound(
                 f"""
                 Could not find the micronsPer[X,Y]Pixel parameters in
                 {self.zoom_params_file} for zoom level {zoom}.
                 """
             )
 
-    def get_beam_position_from_zoom(self, zoom: float) -> Tuple[int, int]:
+    def get_beam_position_from_zoom(
+        self, zoom: float, xsize: int, ysize: int
+    ) -> Tuple[int, int]:
         """
         Extracts the beam location in pixels `xCentre` `yCentre`, for a requested zoom \
         level. The beam location is manually inputted by the beamline operator on GDA \
         by clicking where on screen a scintillator lights up, and stored in the \
         display.configuration file.
         """
         crosshair_x_line = None
@@ -137,18 +157,22 @@
                     break
 
         if crosshair_x_line is None or crosshair_y_line is None:
             raise OAVError_BeamPositionNotFound(
                 f"Could not extract beam position at zoom level {zoom}"
             )
 
-        beam_centre_i = int(crosshair_x_line.split(" = ")[1])
-        beam_centre_j = int(crosshair_y_line.split(" = ")[1])
+        beam_centre_i = (
+            int(crosshair_x_line.split(" = ")[1]) * xsize / DEFAULT_OAV_WINDOW[0]
+        )
+        beam_centre_j = (
+            int(crosshair_y_line.split(" = ")[1]) * ysize / DEFAULT_OAV_WINDOW[1]
+        )
         LOGGER.info(f"Beam centre: {beam_centre_i, beam_centre_j}")
-        return beam_centre_i, beam_centre_j
+        return int(beam_centre_i), int(beam_centre_j)
 
     def calculate_beam_distance(
         self, horizontal_pixels: int, vertical_pixels: int
     ) -> Tuple[int, int]:
         """
         Calculates the distance between the beam centre and the given (horizontal, vertical).
 
@@ -179,9 +203,13 @@
 
     def __init__(self, *args, params: OAVConfigParams, **kwargs):
         super().__init__(*args, **kwargs)
         self.parameters = params
 
     def wait_for_connection(self, all_signals=False, timeout=2):
         connected = super().wait_for_connection(all_signals, timeout)
-        self.zoom_controller.level.subscribe(self.parameters.update_on_zoom)
+        x = self.snapshot.x_size.get()
+        y = self.snapshot.y_size.get()
+
+        cb = partial(self.parameters.update_on_zoom, xsize=x, ysize=y)
+        self.zoom_controller.level.subscribe(cb)
         return connected
```

### Comparing `dls-dodal-1.8.0/src/dodal/devices/oav/oav_errors.py` & `dls-dodal-1.9.0/src/dodal/devices/oav/oav_errors.py`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/src/dodal/devices/oav/oav_parameters.py` & `dls-dodal-1.9.0/src/dodal/devices/oav/oav_parameters.py`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/src/dodal/devices/oav/pin_image_recognition/__init__.py` & `dls-dodal-1.9.0/src/dodal/devices/oav/pin_image_recognition/__init__.py`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/src/dodal/devices/oav/pin_image_recognition/manual_test.py` & `dls-dodal-1.9.0/src/dodal/devices/oav/pin_image_recognition/manual_test.py`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/src/dodal/devices/oav/pin_image_recognition/utils.py` & `dls-dodal-1.9.0/src/dodal/devices/oav/pin_image_recognition/utils.py`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/src/dodal/devices/oav/utils.py` & `dls-dodal-1.9.0/src/dodal/devices/oav/utils.py`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/src/dodal/devices/p45.py` & `dls-dodal-1.9.0/src/dodal/devices/p45.py`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/src/dodal/devices/sample_shutter.py` & `dls-dodal-1.9.0/src/dodal/devices/sample_shutter.py`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/src/dodal/devices/smargon.py` & `dls-dodal-1.9.0/src/dodal/devices/smargon.py`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/src/dodal/devices/status.py` & `dls-dodal-1.9.0/src/dodal/devices/status.py`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/src/dodal/devices/synchrotron.py` & `dls-dodal-1.9.0/src/dodal/devices/synchrotron.py`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/src/dodal/devices/undulator.py` & `dls-dodal-1.9.0/src/dodal/devices/undulator.py`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/src/dodal/devices/undulator_dcm.py` & `dls-dodal-1.9.0/src/dodal/devices/undulator_dcm.py`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/src/dodal/devices/utils.py` & `dls-dodal-1.9.0/src/dodal/devices/utils.py`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/src/dodal/devices/xbpm_feedback.py` & `dls-dodal-1.9.0/src/dodal/devices/xbpm_feedback.py`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/src/dodal/devices/xspress3_mini/xspress3_mini.py` & `dls-dodal-1.9.0/src/dodal/devices/xspress3_mini/xspress3_mini.py`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/src/dodal/devices/xspress3_mini/xspress3_mini_channel.py` & `dls-dodal-1.9.0/src/dodal/devices/xspress3_mini/xspress3_mini_channel.py`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/src/dodal/devices/zebra.py` & `dls-dodal-1.9.0/src/dodal/devices/zebra.py`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/src/dodal/log.py` & `dls-dodal-1.9.0/src/dodal/log.py`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/src/dodal/utils.py` & `dls-dodal-1.9.0/src/dodal/utils.py`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/tests/beamlines/unit_tests/test_beamline_utils.py` & `dls-dodal-1.9.0/tests/beamlines/unit_tests/test_beamline_utils.py`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/tests/beamlines/unit_tests/test_i03.py` & `dls-dodal-1.9.0/tests/beamlines/unit_tests/test_i03.py`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/tests/beamlines/unit_tests/test_i24.py` & `dls-dodal-1.9.0/tests/beamlines/unit_tests/test_i24.py`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/tests/conftest.py` & `dls-dodal-1.9.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/tests/devices/i04/test_transfocator.py` & `dls-dodal-1.9.0/tests/devices/i04/test_transfocator.py`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/tests/devices/system_tests/test_aperturescatterguard_system.py` & `dls-dodal-1.9.0/tests/devices/system_tests/test_aperturescatterguard_system.py`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/tests/devices/system_tests/test_eiger_system.py` & `dls-dodal-1.9.0/tests/devices/system_tests/test_eiger_system.py`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/tests/devices/system_tests/test_gridscan_system.py` & `dls-dodal-1.9.0/tests/devices/system_tests/test_gridscan_system.py`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/tests/devices/system_tests/test_oav_system.py` & `dls-dodal-1.9.0/tests/devices/system_tests/test_oav_system.py`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/tests/devices/system_tests/test_zebra_system.py` & `dls-dodal-1.9.0/tests/devices/system_tests/test_zebra_system.py`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/tests/devices/unit_tests/i24/test_dual_backlight.py` & `dls-dodal-1.9.0/tests/devices/unit_tests/i24/test_dual_backlight.py`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/tests/devices/unit_tests/oav/image_recognition/test_pin_tip_detect.py` & `dls-dodal-1.9.0/tests/devices/unit_tests/oav/image_recognition/test_pin_tip_detect.py`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/tests/devices/unit_tests/oav/image_recognition/test_pin_tip_detect_utils.py` & `dls-dodal-1.9.0/tests/devices/unit_tests/oav/image_recognition/test_pin_tip_detect_utils.py`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/tests/devices/unit_tests/oav/test_oav.py` & `dls-dodal-1.9.0/tests/devices/unit_tests/oav/test_oav.py`

 * *Files 23% similar despite different names*

```diff
@@ -17,14 +17,17 @@
 @pytest.fixture
 def oav() -> OAV:
     oav_params = OAVConfigParams(ZOOM_LEVELS_XML, DISPLAY_CONFIGURATION)
     oav: OAV = instantiate_fake_device(OAV, params=oav_params)
     oav.proc.port_name.sim_put("proc")
     oav.cam.port_name.sim_put("CAM")
 
+    oav.snapshot.x_size.sim_put("1024")
+    oav.snapshot.y_size.sim_put("768")
+
     oav.zoom_controller.zrst.set("1.0x")
     oav.zoom_controller.onst.set("2.0x")
     oav.zoom_controller.twst.set("3.0x")
     oav.zoom_controller.thst.set("5.0x")
     oav.zoom_controller.frst.set("7.0x")
     oav.zoom_controller.fvst.set("9.0x")
 
@@ -60,15 +63,15 @@
 
     assert mxsc_status in full_status
     assert mjpg_status in full_status
 
 
 def test_load_microns_per_pixel_entry_not_found(oav: OAV):
     with pytest.raises(OAVError_ZoomLevelNotFound):
-        oav.parameters.load_microns_per_pixel(0.000001)
+        oav.parameters.load_microns_per_pixel(0.000001, 0, 0)
 
 
 @pytest.mark.parametrize(
     "zoom_level,expected_microns_x,expected_microns_y",
     [
         ("1.0x", 2.87, 2.87),
         ("2.5", 2.31, 2.31),
@@ -77,26 +80,30 @@
     ],
 )
 def test_get_micronsperpixel_from_oav(
     zoom_level, expected_microns_x, expected_microns_y, oav: OAV
 ):
     oav.zoom_controller.level.sim_put(zoom_level)
 
-    assert oav.parameters.micronsPerXPixel == expected_microns_x
-    assert oav.parameters.micronsPerYPixel == expected_microns_y
+    assert oav.parameters.micronsPerXPixel == pytest.approx(
+        expected_microns_x, abs=1e-2
+    )
+    assert oav.parameters.micronsPerYPixel == pytest.approx(
+        expected_microns_y, abs=1e-2
+    )
 
 
 def test_beam_position_not_found_for_wrong_entry(oav: OAV):
     with pytest.raises(OAVError_BeamPositionNotFound):
-        oav.parameters.get_beam_position_from_zoom(2.0)
+        oav.parameters.get_beam_position_from_zoom(2.0, 0, 0)
 
 
 def test_get_beam_position(oav: OAV):
     expected_beam_position = (493, 355)
-    beam_position = oav.parameters.get_beam_position_from_zoom(2.5)
+    beam_position = oav.parameters.get_beam_position_from_zoom(2.5, 1024, 768)
 
     assert beam_position[0] == expected_beam_position[0]
     assert beam_position[1] == expected_beam_position[1]
 
 
 @pytest.mark.parametrize(
     "zoom_level,expected_xCentre,expected_yCentre",
@@ -110,14 +117,36 @@
 ):
     oav.zoom_controller.level.sim_put(zoom_level)
 
     assert oav.parameters.beam_centre_i == expected_xCentre
     assert oav.parameters.beam_centre_j == expected_yCentre
 
 
+def test_extract_rescaled_micronsperpixel(oav: OAV):
+    oav.snapshot.x_size.sim_put("1292")
+    oav.snapshot.y_size.sim_put("964")
+    oav.wait_for_connection()
+
+    oav.zoom_controller.level.sim_put("1.0")
+
+    assert oav.parameters.micronsPerXPixel == pytest.approx(2.27, abs=1e-2)
+    assert oav.parameters.micronsPerYPixel == pytest.approx(2.28, abs=1e-2)
+
+
+def test_extract_rescaled_beam_position(oav: OAV):
+    oav.snapshot.x_size.sim_put("1292")
+    oav.snapshot.y_size.sim_put("964")
+    oav.wait_for_connection()
+
+    oav.zoom_controller.level.sim_put("1.0")
+
+    assert oav.parameters.beam_centre_i == 601
+    assert oav.parameters.beam_centre_j == 450
+
+
 @pytest.mark.parametrize(
     "h, v, expected_x, expected_y",
     [
         (54, 100, 517 - 54, 350 - 100),
         (0, 0, 517, 350),
         (500, 500, 517 - 500, 350 - 500),
     ],
```

### Comparing `dls-dodal-1.8.0/tests/devices/unit_tests/oav/test_oav_parameters.py` & `dls-dodal-1.9.0/tests/devices/unit_tests/oav/test_oav_parameters.py`

 * *Files 7% similar despite different names*

```diff
@@ -35,13 +35,13 @@
 
 
 def test_given_context_and_microns_per_pixel_get_max_tip_distance_in_pixels(
     mock_parameters: OAVParameters,
 ):
     zoom_level = mock_parameters.zoom
     config_params = OAVConfigParams(ZOOM_LEVELS_XML, DISPLAY_CONFIGURATION)
-    config_params.update_on_zoom(str(zoom_level))
+    config_params.update_on_zoom(str(zoom_level), 1024, 768)
 
     assert mock_parameters.max_tip_distance == 300
     assert mock_parameters.get_max_tip_distance_in_pixels(
         config_params.micronsPerXPixel
     ) == pytest.approx(189.873, abs=1e-3)
```

### Comparing `dls-dodal-1.8.0/tests/devices/unit_tests/test_OAVCentring.json` & `dls-dodal-1.9.0/tests/devices/unit_tests/test_OAVCentring.json`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/tests/devices/unit_tests/test_attenuator.py` & `dls-dodal-1.9.0/tests/devices/unit_tests/test_attenuator.py`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/tests/devices/unit_tests/test_backlight.py` & `dls-dodal-1.9.0/tests/devices/unit_tests/test_backlight.py`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/tests/devices/unit_tests/test_beam_converter.py` & `dls-dodal-1.9.0/tests/devices/unit_tests/test_beam_converter.py`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/tests/devices/unit_tests/test_beamline_undulator_to_gap_lookup_table.txt` & `dls-dodal-1.9.0/tests/devices/unit_tests/test_beamline_undulator_to_gap_lookup_table.txt`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/tests/devices/unit_tests/test_detector.py` & `dls-dodal-1.9.0/tests/devices/unit_tests/test_detector.py`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/tests/devices/unit_tests/test_display.configuration` & `dls-dodal-1.9.0/tests/devices/unit_tests/test_display.configuration`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/tests/devices/unit_tests/test_eiger.py` & `dls-dodal-1.9.0/tests/devices/unit_tests/test_eiger.py`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/tests/devices/unit_tests/test_grid_overlay.py` & `dls-dodal-1.9.0/tests/devices/unit_tests/test_grid_overlay.py`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/tests/devices/unit_tests/test_gridscan.py` & `dls-dodal-1.9.0/tests/devices/unit_tests/test_gridscan.py`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/tests/devices/unit_tests/test_jCameraManZoomLevels.xml` & `dls-dodal-1.9.0/tests/devices/unit_tests/test_jCameraManZoomLevels.xml`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/tests/devices/unit_tests/test_motors.py` & `dls-dodal-1.9.0/tests/devices/unit_tests/test_motors.py`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/tests/devices/unit_tests/test_oav.py` & `dls-dodal-1.9.0/tests/devices/unit_tests/test_oav.py`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/tests/devices/unit_tests/test_oav_centring.py` & `dls-dodal-1.9.0/tests/devices/unit_tests/test_oav_centring.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,14 +36,16 @@
 
 @pytest.fixture
 def mock_oav():
     oav_params = OAVConfigParams(ZOOM_LEVELS_XML, DISPLAY_CONFIGURATION)
     oav: OAV = make_fake_device(OAV)(
         name="oav", prefix="a fake beamline", params=oav_params
     )
+    oav.snapshot.x_size.sim_put("1024")
+    oav.snapshot.y_size.sim_put("768")
     oav.wait_for_connection()
     return oav
 
 
 @pytest.fixture
 def mock_parameters():
     return OAVParameters(
```

### Comparing `dls-dodal-1.8.0/tests/devices/unit_tests/test_odin.py` & `dls-dodal-1.9.0/tests/devices/unit_tests/test_odin.py`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/tests/devices/unit_tests/test_pin_tip_detect.py` & `dls-dodal-1.9.0/tests/devices/unit_tests/test_pin_tip_detect.py`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/tests/devices/unit_tests/test_sample_shutter.py` & `dls-dodal-1.9.0/tests/devices/unit_tests/test_sample_shutter.py`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/tests/devices/unit_tests/test_smargon.py` & `dls-dodal-1.9.0/tests/devices/unit_tests/test_smargon.py`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/tests/devices/unit_tests/test_status.py` & `dls-dodal-1.9.0/tests/devices/unit_tests/test_status.py`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/tests/devices/unit_tests/test_undulator_dcm.py` & `dls-dodal-1.9.0/tests/devices/unit_tests/test_undulator_dcm.py`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/tests/devices/unit_tests/test_utils.py` & `dls-dodal-1.9.0/tests/devices/unit_tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/tests/devices/unit_tests/test_xbpm_feedback.py` & `dls-dodal-1.9.0/tests/devices/unit_tests/test_xbpm_feedback.py`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/tests/devices/unit_tests/test_xspress3mini.py` & `dls-dodal-1.9.0/tests/devices/unit_tests/test_xspress3mini.py`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/tests/devices/unit_tests/test_zebra.py` & `dls-dodal-1.9.0/tests/devices/unit_tests/test_zebra.py`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/tests/fake_beamline_misbehaving_builtins.py` & `dls-dodal-1.9.0/tests/fake_beamline_misbehaving_builtins.py`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/tests/system_tests/test_i03_system.py` & `dls-dodal-1.9.0/tests/system_tests/test_i03_system.py`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/tests/system_tests/test_i04_1_system.py` & `dls-dodal-1.9.0/tests/system_tests/test_i04_1_system.py`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/tests/system_tests/test_i04_system.py` & `dls-dodal-1.9.0/tests/system_tests/test_i04_system.py`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/tests/system_tests/test_i23_system.py` & `dls-dodal-1.9.0/tests/system_tests/test_i23_system.py`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/tests/system_tests/test_i24_system.py` & `dls-dodal-1.9.0/tests/system_tests/test_i24_system.py`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/tests/test_utils.py` & `dls-dodal-1.9.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `dls-dodal-1.8.0/tests/unit_tests/test_log.py` & `dls-dodal-1.9.0/tests/unit_tests/test_log.py`

 * *Files identical despite different names*

