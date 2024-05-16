# Comparing `tmp/nexgen-0.9.2.tar.gz` & `tmp/nexgen-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nexgen-0.9.2.tar", last modified: Thu May  9 14:47:21 2024, max compression
+gzip compressed data, was "nexgen-0.9.3.tar", last modified: Thu May 16 11:48:24 2024, max compression
```

## Comparing `nexgen-0.9.2.tar` & `nexgen-0.9.3.tar`

### file list

```diff
@@ -1,150 +1,150 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:47:21.595804 nexgen-0.9.2/
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-09 14:47:15.000000 nexgen-0.9.2/.bumpversion.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-09 14:47:15.000000 nexgen-0.9.2/.codecov.yml
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-09 14:47:15.000000 nexgen-0.9.2/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:47:21.571804 nexgen-0.9.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:47:21.567804 nexgen-0.9.2/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:47:21.571804 nexgen-0.9.2/.github/actions/install_requirements/
--rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-05-09 14:47:15.000000 nexgen-0.9.2/.github/actions/install_requirements/action.yml
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-09 14:47:15.000000 nexgen-0.9.2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:47:21.575804 nexgen-0.9.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     5196 2024-05-09 14:47:15.000000 nexgen-0.9.2/.github/workflows/code.yml
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-05-09 14:47:15.000000 nexgen-0.9.2/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-09 14:47:15.000000 nexgen-0.9.2/.github/workflows/linkcheck.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-05-09 14:47:15.000000 nexgen-0.9.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-09 14:47:15.000000 nexgen-0.9.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-09 14:47:15.000000 nexgen-0.9.2/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    11948 2024-05-09 14:47:15.000000 nexgen-0.9.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     3952 2024-05-09 14:47:15.000000 nexgen-0.9.2/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-05-09 14:47:15.000000 nexgen-0.9.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-09 14:47:15.000000 nexgen-0.9.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4719 2024-05-09 14:47:21.595804 nexgen-0.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-05-09 14:47:15.000000 nexgen-0.9.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:47:21.575804 nexgen-0.9.2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-09 14:47:15.000000 nexgen-0.9.2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     4274 2024-05-09 14:47:15.000000 nexgen-0.9.2/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-05-09 14:47:15.000000 nexgen-0.9.2/docs/api_beamlines.rst
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-09 14:47:15.000000 nexgen-0.9.2/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6607 2024-05-09 14:47:15.000000 nexgen-0.9.2/docs/beamlines.rst
--rwxr-xr-x   0 runner    (1001) docker     (127)     5119 2024-05-09 14:47:15.000000 nexgen-0.9.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-09 14:47:15.000000 nexgen-0.9.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-09 14:47:15.000000 nexgen-0.9.2/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)     6987 2024-05-09 14:47:15.000000 nexgen-0.9.2/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3570 2024-05-09 14:47:15.000000 nexgen-0.9.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-09 14:47:15.000000 nexgen-0.9.2/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-09 14:47:15.000000 nexgen-0.9.2/requirements_doc.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 14:47:21.595804 nexgen-0.9.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:47:21.567804 nexgen-0.9.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:47:21.575804 nexgen-0.9.2/src/nexgen/
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-09 14:47:15.000000 nexgen-0.9.2/src/nexgen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-09 14:47:15.000000 nexgen-0.9.2/src/nexgen/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:47:21.579804 nexgen-0.9.2/src/nexgen/beamlines/
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-05-09 14:47:15.000000 nexgen-0.9.2/src/nexgen/beamlines/ED_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     8246 2024-05-09 14:47:15.000000 nexgen-0.9.2/src/nexgen/beamlines/ED_singla_nxs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:47:21.579804 nexgen-0.9.2/src/nexgen/beamlines/GDAtools/
--rw-r--r--   0 runner    (1001) docker     (127)     4264 2024-05-09 14:47:15.000000 nexgen-0.9.2/src/nexgen/beamlines/GDAtools/ExtendedRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4967 2024-05-09 14:47:15.000000 nexgen-0.9.2/src/nexgen/beamlines/GDAtools/GDAjson2params.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 14:47:15.000000 nexgen-0.9.2/src/nexgen/beamlines/GDAtools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12195 2024-05-09 14:47:15.000000 nexgen-0.9.2/src/nexgen/beamlines/I19_2_gda_nxs.py
--rw-r--r--   0 runner    (1001) docker     (127)    19350 2024-05-09 14:47:15.000000 nexgen-0.9.2/src/nexgen/beamlines/I19_2_nxs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-09 14:47:15.000000 nexgen-0.9.2/src/nexgen/beamlines/I19_2_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-05-09 14:47:15.000000 nexgen-0.9.2/src/nexgen/beamlines/I24_params.py
--rw-r--r--   0 runner    (1001) docker     (127)    12755 2024-05-09 14:47:15.000000 nexgen-0.9.2/src/nexgen/beamlines/SSX_Eiger_nxs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9040 2024-05-09 14:47:15.000000 nexgen-0.9.2/src/nexgen/beamlines/SSX_Tristan_nxs.py
--rw-r--r--   0 runner    (1001) docker     (127)     7586 2024-05-09 14:47:15.000000 nexgen-0.9.2/src/nexgen/beamlines/SSX_chip.py
--rw-r--r--   0 runner    (1001) docker     (127)     8084 2024-05-09 14:47:15.000000 nexgen-0.9.2/src/nexgen/beamlines/SSX_expt.py
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-09 14:47:15.000000 nexgen-0.9.2/src/nexgen/beamlines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-05-09 14:47:15.000000 nexgen-0.9.2/src/nexgen/beamlines/beamline_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:47:21.583804 nexgen-0.9.2/src/nexgen/command_line/
--rw-r--r--   0 runner    (1001) docker     (127)     6715 2024-05-09 14:47:15.000000 nexgen-0.9.2/src/nexgen/command_line/ED_mrc_to_nexus.py
--rw-r--r--   0 runner    (1001) docker     (127)     7378 2024-05-09 14:47:15.000000 nexgen-0.9.2/src/nexgen/command_line/ED_nexus.py
--rw-r--r--   0 runner    (1001) docker     (127)     8555 2024-05-09 14:47:15.000000 nexgen-0.9.2/src/nexgen/command_line/I19_2_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     5292 2024-05-09 14:47:15.000000 nexgen-0.9.2/src/nexgen/command_line/SSX_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3112 2024-05-09 14:47:15.000000 nexgen-0.9.2/src/nexgen/command_line/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14082 2024-05-09 14:47:15.000000 nexgen-0.9.2/src/nexgen/command_line/cli_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7221 2024-05-09 14:47:15.000000 nexgen-0.9.2/src/nexgen/command_line/copy_nexus.py
--rw-r--r--   0 runner    (1001) docker     (127)    27639 2024-05-09 14:47:15.000000 nexgen-0.9.2/src/nexgen/command_line/nexus_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     8223 2024-05-09 14:47:15.000000 nexgen-0.9.2/src/nexgen/command_line/nxs_phil.py
--rw-r--r--   0 runner    (1001) docker     (127)     4025 2024-05-09 14:47:15.000000 nexgen-0.9.2/src/nexgen/command_line/phil_files_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2570 2024-05-09 14:47:15.000000 nexgen-0.9.2/src/nexgen/log.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:47:21.583804 nexgen-0.9.2/src/nexgen/nxs_copy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 14:47:15.000000 nexgen-0.9.2/src/nexgen/nxs_copy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4784 2024-05-09 14:47:15.000000 nexgen-0.9.2/src/nexgen/nxs_copy/copy_nexus.py
--rw-r--r--   0 runner    (1001) docker     (127)    11945 2024-05-09 14:47:15.000000 nexgen-0.9.2/src/nexgen/nxs_copy/copy_tristan_nexus.py
--rw-r--r--   0 runner    (1001) docker     (127)    11970 2024-05-09 14:47:15.000000 nexgen-0.9.2/src/nexgen/nxs_copy/copy_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:47:21.583804 nexgen-0.9.2/src/nexgen/nxs_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-09 14:47:15.000000 nexgen-0.9.2/src/nexgen/nxs_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-05-09 14:47:15.000000 nexgen-0.9.2/src/nexgen/nxs_utils/axes.py
--rw-r--r--   0 runner    (1001) docker     (127)    12330 2024-05-09 14:47:15.000000 nexgen-0.9.2/src/nexgen/nxs_utils/detector.py
--rw-r--r--   0 runner    (1001) docker     (127)     7147 2024-05-09 14:47:15.000000 nexgen-0.9.2/src/nexgen/nxs_utils/goniometer.py
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-09 14:47:15.000000 nexgen-0.9.2/src/nexgen/nxs_utils/sample.py
--rw-r--r--   0 runner    (1001) docker     (127)     7085 2024-05-09 14:47:15.000000 nexgen-0.9.2/src/nexgen/nxs_utils/scan_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2810 2024-05-09 14:47:15.000000 nexgen-0.9.2/src/nexgen/nxs_utils/source.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:47:21.583804 nexgen-0.9.2/src/nexgen/nxs_write/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 14:47:15.000000 nexgen-0.9.2/src/nexgen/nxs_write/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    36768 2024-05-09 14:47:15.000000 nexgen-0.9.2/src/nexgen/nxs_write/nxclass_writers.py
--rw-r--r--   0 runner    (1001) docker     (127)    22235 2024-05-09 14:47:15.000000 nexgen-0.9.2/src/nexgen/nxs_write/nxmx_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)    11555 2024-05-09 14:47:15.000000 nexgen-0.9.2/src/nexgen/nxs_write/write_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:47:21.587804 nexgen-0.9.2/src/nexgen/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-05-09 14:47:15.000000 nexgen-0.9.2/src/nexgen/templates/DLS_Template.phil
--rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-05-09 14:47:15.000000 nexgen-0.9.2/src/nexgen/templates/ED_Singla.phil
--rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-05-09 14:47:15.000000 nexgen-0.9.2/src/nexgen/templates/I03_Eiger.phil
--rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-05-09 14:47:15.000000 nexgen-0.9.2/src/nexgen/templates/I19-2_Eiger.phil
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-09 14:47:15.000000 nexgen-0.9.2/src/nexgen/templates/I19-2_Tristan.phil
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-09 14:47:15.000000 nexgen-0.9.2/src/nexgen/templates/I24_Eiger.phil
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-05-09 14:47:15.000000 nexgen-0.9.2/src/nexgen/templates/VMXi.phil
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 14:47:15.000000 nexgen-0.9.2/src/nexgen/templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:47:21.587804 nexgen-0.9.2/src/nexgen/tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 14:47:15.000000 nexgen-0.9.2/src/nexgen/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-09 14:47:15.000000 nexgen-0.9.2/src/nexgen/tools/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    10359 2024-05-09 14:47:15.000000 nexgen-0.9.2/src/nexgen/tools/data_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)    10343 2024-05-09 14:47:15.000000 nexgen-0.9.2/src/nexgen/tools/ed_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     9735 2024-05-09 14:47:15.000000 nexgen-0.9.2/src/nexgen/tools/meta_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     9418 2024-05-09 14:47:15.000000 nexgen-0.9.2/src/nexgen/tools/metafile.py
--rw-r--r--   0 runner    (1001) docker     (127)     6758 2024-05-09 14:47:15.000000 nexgen-0.9.2/src/nexgen/tools/mrc_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)    13035 2024-05-09 14:47:15.000000 nexgen-0.9.2/src/nexgen/tools/vds_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     8211 2024-05-09 14:47:15.000000 nexgen-0.9.2/src/nexgen/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:47:21.591804 nexgen-0.9.2/src/nexgen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4719 2024-05-09 14:47:21.000000 nexgen-0.9.2/src/nexgen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3699 2024-05-09 14:47:21.000000 nexgen-0.9.2/src/nexgen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 14:47:21.000000 nexgen-0.9.2/src/nexgen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-09 14:47:21.000000 nexgen-0.9.2/src/nexgen.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-09 14:47:21.000000 nexgen-0.9.2/src/nexgen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-09 14:47:21.000000 nexgen-0.9.2/src/nexgen.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:47:21.587804 nexgen-0.9.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 14:47:15.000000 nexgen-0.9.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:47:21.587804 nexgen-0.9.2/tests/beamlines/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 14:47:15.000000 nexgen-0.9.2/tests/beamlines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4619 2024-05-09 14:47:15.000000 nexgen-0.9.2/tests/beamlines/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-05-09 14:47:15.000000 nexgen-0.9.2/tests/beamlines/test_GDA_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-05-09 14:47:15.000000 nexgen-0.9.2/tests/beamlines/test_SSX_chip.py
--rw-r--r--   0 runner    (1001) docker     (127)     4177 2024-05-09 14:47:15.000000 nexgen-0.9.2/tests/beamlines/test_SSX_expt.py
--rw-r--r--   0 runner    (1001) docker     (127)      742 2024-05-09 14:47:15.000000 nexgen-0.9.2/tests/beamlines/test_SSXwriters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-05-09 14:47:15.000000 nexgen-0.9.2/tests/beamlines/test_beamline_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-09 14:47:15.000000 nexgen-0.9.2/tests/beamlines/test_i19nxs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:47:21.591804 nexgen-0.9.2/tests/cli/
--rw-r--r--   0 runner    (1001) docker     (127)     3231 2024-05-09 14:47:15.000000 nexgen-0.9.2/tests/cli/test_cli_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:47:21.591804 nexgen-0.9.2/tests/nxs_copy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 14:47:15.000000 nexgen-0.9.2/tests/nxs_copy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3744 2024-05-09 14:47:15.000000 nexgen-0.9.2/tests/nxs_copy/test_copy_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:47:21.591804 nexgen-0.9.2/tests/nxs_utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 14:47:15.000000 nexgen-0.9.2/tests/nxs_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-05-09 14:47:15.000000 nexgen-0.9.2/tests/nxs_utils/test_axes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3314 2024-05-09 14:47:15.000000 nexgen-0.9.2/tests/nxs_utils/test_detector.py
--rw-r--r--   0 runner    (1001) docker     (127)     4664 2024-05-09 14:47:15.000000 nexgen-0.9.2/tests/nxs_utils/test_goniometer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4864 2024-05-09 14:47:15.000000 nexgen-0.9.2/tests/nxs_utils/test_scan.py
--rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-05-09 14:47:15.000000 nexgen-0.9.2/tests/nxs_utils/test_source.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:47:21.591804 nexgen-0.9.2/tests/nxs_write/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 14:47:15.000000 nexgen-0.9.2/tests/nxs_write/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-05-09 14:47:15.000000 nexgen-0.9.2/tests/nxs_write/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    17441 2024-05-09 14:47:15.000000 nexgen-0.9.2/tests/nxs_write/test_NXclassWriters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-05-09 14:47:15.000000 nexgen-0.9.2/tests/nxs_write/test_NXmxWriter.py
--rw-r--r--   0 runner    (1001) docker     (127)     4002 2024-05-09 14:47:15.000000 nexgen-0.9.2/tests/nxs_write/test_write_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-09 14:47:15.000000 nexgen-0.9.2/tests/test_log.py
--rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-05-09 14:47:15.000000 nexgen-0.9.2/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-09 14:47:15.000000 nexgen-0.9.2/tests/test_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 14:47:21.591804 nexgen-0.9.2/tests/tools/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 14:47:15.000000 nexgen-0.9.2/tests/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4617 2024-05-09 14:47:15.000000 nexgen-0.9.2/tests/tools/test_VDS_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     4796 2024-05-09 14:47:15.000000 nexgen-0.9.2/tests/tools/test_meta_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     5378 2024-05-09 14:47:15.000000 nexgen-0.9.2/tests/tools/test_tools_for_ED.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:48:24.755029 nexgen-0.9.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-16 11:48:19.000000 nexgen-0.9.3/.bumpversion.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-16 11:48:19.000000 nexgen-0.9.3/.codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-16 11:48:19.000000 nexgen-0.9.3/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:48:24.735029 nexgen-0.9.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:48:24.731029 nexgen-0.9.3/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:48:24.735029 nexgen-0.9.3/.github/actions/install_requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-05-16 11:48:19.000000 nexgen-0.9.3/.github/actions/install_requirements/action.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-16 11:48:19.000000 nexgen-0.9.3/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:48:24.735029 nexgen-0.9.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     5196 2024-05-16 11:48:19.000000 nexgen-0.9.3/.github/workflows/code.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-05-16 11:48:19.000000 nexgen-0.9.3/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-16 11:48:19.000000 nexgen-0.9.3/.github/workflows/linkcheck.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1981 2024-05-16 11:48:19.000000 nexgen-0.9.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-16 11:48:19.000000 nexgen-0.9.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-16 11:48:19.000000 nexgen-0.9.3/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    12245 2024-05-16 11:48:19.000000 nexgen-0.9.3/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3952 2024-05-16 11:48:19.000000 nexgen-0.9.3/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-05-16 11:48:19.000000 nexgen-0.9.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-16 11:48:19.000000 nexgen-0.9.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4719 2024-05-16 11:48:24.755029 nexgen-0.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-05-16 11:48:19.000000 nexgen-0.9.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:48:24.735029 nexgen-0.9.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-16 11:48:19.000000 nexgen-0.9.3/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     4274 2024-05-16 11:48:19.000000 nexgen-0.9.3/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-05-16 11:48:19.000000 nexgen-0.9.3/docs/api_beamlines.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-16 11:48:19.000000 nexgen-0.9.3/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6607 2024-05-16 11:48:19.000000 nexgen-0.9.3/docs/beamlines.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5119 2024-05-16 11:48:19.000000 nexgen-0.9.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-16 11:48:19.000000 nexgen-0.9.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-16 11:48:19.000000 nexgen-0.9.3/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)     6987 2024-05-16 11:48:19.000000 nexgen-0.9.3/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3570 2024-05-16 11:48:19.000000 nexgen-0.9.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-16 11:48:19.000000 nexgen-0.9.3/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-16 11:48:19.000000 nexgen-0.9.3/requirements_doc.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 11:48:24.755029 nexgen-0.9.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:48:24.731029 nexgen-0.9.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:48:24.739029 nexgen-0.9.3/src/nexgen/
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-16 11:48:19.000000 nexgen-0.9.3/src/nexgen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-16 11:48:19.000000 nexgen-0.9.3/src/nexgen/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:48:24.739029 nexgen-0.9.3/src/nexgen/beamlines/
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-05-16 11:48:19.000000 nexgen-0.9.3/src/nexgen/beamlines/ED_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8246 2024-05-16 11:48:19.000000 nexgen-0.9.3/src/nexgen/beamlines/ED_singla_nxs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:48:24.739029 nexgen-0.9.3/src/nexgen/beamlines/GDAtools/
+-rw-r--r--   0 runner    (1001) docker     (127)     4264 2024-05-16 11:48:19.000000 nexgen-0.9.3/src/nexgen/beamlines/GDAtools/ExtendedRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4967 2024-05-16 11:48:19.000000 nexgen-0.9.3/src/nexgen/beamlines/GDAtools/GDAjson2params.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 11:48:19.000000 nexgen-0.9.3/src/nexgen/beamlines/GDAtools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12195 2024-05-16 11:48:19.000000 nexgen-0.9.3/src/nexgen/beamlines/I19_2_gda_nxs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19350 2024-05-16 11:48:19.000000 nexgen-0.9.3/src/nexgen/beamlines/I19_2_nxs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-16 11:48:19.000000 nexgen-0.9.3/src/nexgen/beamlines/I19_2_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-05-16 11:48:19.000000 nexgen-0.9.3/src/nexgen/beamlines/I24_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12755 2024-05-16 11:48:19.000000 nexgen-0.9.3/src/nexgen/beamlines/SSX_Eiger_nxs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9040 2024-05-16 11:48:19.000000 nexgen-0.9.3/src/nexgen/beamlines/SSX_Tristan_nxs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7586 2024-05-16 11:48:19.000000 nexgen-0.9.3/src/nexgen/beamlines/SSX_chip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8084 2024-05-16 11:48:19.000000 nexgen-0.9.3/src/nexgen/beamlines/SSX_expt.py
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-16 11:48:19.000000 nexgen-0.9.3/src/nexgen/beamlines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-05-16 11:48:19.000000 nexgen-0.9.3/src/nexgen/beamlines/beamline_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:48:24.743029 nexgen-0.9.3/src/nexgen/command_line/
+-rw-r--r--   0 runner    (1001) docker     (127)     6715 2024-05-16 11:48:19.000000 nexgen-0.9.3/src/nexgen/command_line/ED_mrc_to_nexus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7378 2024-05-16 11:48:19.000000 nexgen-0.9.3/src/nexgen/command_line/ED_nexus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8555 2024-05-16 11:48:19.000000 nexgen-0.9.3/src/nexgen/command_line/I19_2_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5292 2024-05-16 11:48:19.000000 nexgen-0.9.3/src/nexgen/command_line/SSX_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3112 2024-05-16 11:48:19.000000 nexgen-0.9.3/src/nexgen/command_line/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14082 2024-05-16 11:48:19.000000 nexgen-0.9.3/src/nexgen/command_line/cli_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7221 2024-05-16 11:48:19.000000 nexgen-0.9.3/src/nexgen/command_line/copy_nexus.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27639 2024-05-16 11:48:19.000000 nexgen-0.9.3/src/nexgen/command_line/nexus_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8223 2024-05-16 11:48:19.000000 nexgen-0.9.3/src/nexgen/command_line/nxs_phil.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4025 2024-05-16 11:48:19.000000 nexgen-0.9.3/src/nexgen/command_line/phil_files_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2569 2024-05-16 11:48:19.000000 nexgen-0.9.3/src/nexgen/log.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:48:24.743029 nexgen-0.9.3/src/nexgen/nxs_copy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 11:48:19.000000 nexgen-0.9.3/src/nexgen/nxs_copy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4773 2024-05-16 11:48:19.000000 nexgen-0.9.3/src/nexgen/nxs_copy/copy_nexus.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11945 2024-05-16 11:48:19.000000 nexgen-0.9.3/src/nexgen/nxs_copy/copy_tristan_nexus.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12321 2024-05-16 11:48:19.000000 nexgen-0.9.3/src/nexgen/nxs_copy/copy_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:48:24.743029 nexgen-0.9.3/src/nexgen/nxs_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-16 11:48:19.000000 nexgen-0.9.3/src/nexgen/nxs_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-05-16 11:48:19.000000 nexgen-0.9.3/src/nexgen/nxs_utils/axes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12330 2024-05-16 11:48:19.000000 nexgen-0.9.3/src/nexgen/nxs_utils/detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7147 2024-05-16 11:48:19.000000 nexgen-0.9.3/src/nexgen/nxs_utils/goniometer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-16 11:48:19.000000 nexgen-0.9.3/src/nexgen/nxs_utils/sample.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7053 2024-05-16 11:48:19.000000 nexgen-0.9.3/src/nexgen/nxs_utils/scan_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2810 2024-05-16 11:48:19.000000 nexgen-0.9.3/src/nexgen/nxs_utils/source.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:48:24.747029 nexgen-0.9.3/src/nexgen/nxs_write/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 11:48:19.000000 nexgen-0.9.3/src/nexgen/nxs_write/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33019 2024-05-16 11:48:19.000000 nexgen-0.9.3/src/nexgen/nxs_write/nxclass_writers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22674 2024-05-16 11:48:19.000000 nexgen-0.9.3/src/nexgen/nxs_write/nxmx_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12956 2024-05-16 11:48:19.000000 nexgen-0.9.3/src/nexgen/nxs_write/write_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:48:24.747029 nexgen-0.9.3/src/nexgen/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-05-16 11:48:19.000000 nexgen-0.9.3/src/nexgen/templates/DLS_Template.phil
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-05-16 11:48:19.000000 nexgen-0.9.3/src/nexgen/templates/ED_Singla.phil
+-rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-05-16 11:48:19.000000 nexgen-0.9.3/src/nexgen/templates/I03_Eiger.phil
+-rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-05-16 11:48:19.000000 nexgen-0.9.3/src/nexgen/templates/I19-2_Eiger.phil
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-16 11:48:19.000000 nexgen-0.9.3/src/nexgen/templates/I19-2_Tristan.phil
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-16 11:48:19.000000 nexgen-0.9.3/src/nexgen/templates/I24_Eiger.phil
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-05-16 11:48:19.000000 nexgen-0.9.3/src/nexgen/templates/VMXi.phil
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 11:48:19.000000 nexgen-0.9.3/src/nexgen/templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:48:24.747029 nexgen-0.9.3/src/nexgen/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 11:48:19.000000 nexgen-0.9.3/src/nexgen/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-16 11:48:19.000000 nexgen-0.9.3/src/nexgen/tools/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10359 2024-05-16 11:48:19.000000 nexgen-0.9.3/src/nexgen/tools/data_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10343 2024-05-16 11:48:19.000000 nexgen-0.9.3/src/nexgen/tools/ed_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9751 2024-05-16 11:48:19.000000 nexgen-0.9.3/src/nexgen/tools/meta_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9418 2024-05-16 11:48:19.000000 nexgen-0.9.3/src/nexgen/tools/metafile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6758 2024-05-16 11:48:19.000000 nexgen-0.9.3/src/nexgen/tools/mrc_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13061 2024-05-16 11:48:19.000000 nexgen-0.9.3/src/nexgen/tools/vds_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8211 2024-05-16 11:48:19.000000 nexgen-0.9.3/src/nexgen/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:48:24.751029 nexgen-0.9.3/src/nexgen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4719 2024-05-16 11:48:24.000000 nexgen-0.9.3/src/nexgen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3699 2024-05-16 11:48:24.000000 nexgen-0.9.3/src/nexgen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 11:48:24.000000 nexgen-0.9.3/src/nexgen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-16 11:48:24.000000 nexgen-0.9.3/src/nexgen.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-16 11:48:24.000000 nexgen-0.9.3/src/nexgen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-16 11:48:24.000000 nexgen-0.9.3/src/nexgen.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:48:24.747029 nexgen-0.9.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 11:48:19.000000 nexgen-0.9.3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:48:24.751029 nexgen-0.9.3/tests/beamlines/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 11:48:19.000000 nexgen-0.9.3/tests/beamlines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4619 2024-05-16 11:48:19.000000 nexgen-0.9.3/tests/beamlines/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2545 2024-05-16 11:48:19.000000 nexgen-0.9.3/tests/beamlines/test_GDA_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-05-16 11:48:19.000000 nexgen-0.9.3/tests/beamlines/test_SSX_chip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4177 2024-05-16 11:48:19.000000 nexgen-0.9.3/tests/beamlines/test_SSX_expt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-05-16 11:48:19.000000 nexgen-0.9.3/tests/beamlines/test_SSXwriters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-05-16 11:48:19.000000 nexgen-0.9.3/tests/beamlines/test_beamline_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-16 11:48:19.000000 nexgen-0.9.3/tests/beamlines/test_i19nxs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:48:24.751029 nexgen-0.9.3/tests/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     3231 2024-05-16 11:48:19.000000 nexgen-0.9.3/tests/cli/test_cli_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:48:24.751029 nexgen-0.9.3/tests/nxs_copy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 11:48:19.000000 nexgen-0.9.3/tests/nxs_copy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3744 2024-05-16 11:48:19.000000 nexgen-0.9.3/tests/nxs_copy/test_copy_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:48:24.751029 nexgen-0.9.3/tests/nxs_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 11:48:19.000000 nexgen-0.9.3/tests/nxs_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-05-16 11:48:19.000000 nexgen-0.9.3/tests/nxs_utils/test_axes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3314 2024-05-16 11:48:19.000000 nexgen-0.9.3/tests/nxs_utils/test_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4664 2024-05-16 11:48:19.000000 nexgen-0.9.3/tests/nxs_utils/test_goniometer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4864 2024-05-16 11:48:19.000000 nexgen-0.9.3/tests/nxs_utils/test_scan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-05-16 11:48:19.000000 nexgen-0.9.3/tests/nxs_utils/test_source.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:48:24.751029 nexgen-0.9.3/tests/nxs_write/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 11:48:19.000000 nexgen-0.9.3/tests/nxs_write/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-05-16 11:48:19.000000 nexgen-0.9.3/tests/nxs_write/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18448 2024-05-16 11:48:19.000000 nexgen-0.9.3/tests/nxs_write/test_NXclassWriters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-05-16 11:48:19.000000 nexgen-0.9.3/tests/nxs_write/test_NXmxWriter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4679 2024-05-16 11:48:19.000000 nexgen-0.9.3/tests/nxs_write/test_write_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-05-16 11:48:19.000000 nexgen-0.9.3/tests/test_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-05-16 11:48:19.000000 nexgen-0.9.3/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-16 11:48:19.000000 nexgen-0.9.3/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 11:48:24.751029 nexgen-0.9.3/tests/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 11:48:19.000000 nexgen-0.9.3/tests/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4617 2024-05-16 11:48:19.000000 nexgen-0.9.3/tests/tools/test_VDS_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4796 2024-05-16 11:48:19.000000 nexgen-0.9.3/tests/tools/test_meta_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5378 2024-05-16 11:48:19.000000 nexgen-0.9.3/tests/tools/test_tools_for_ED.py
```

### Comparing `nexgen-0.9.2/.github/actions/install_requirements/action.yml` & `nexgen-0.9.3/.github/actions/install_requirements/action.yml`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.2/.github/dependabot.yml` & `nexgen-0.9.3/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.2/.github/workflows/code.yml` & `nexgen-0.9.3/.github/workflows/code.yml`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.2/.github/workflows/codeql.yml` & `nexgen-0.9.3/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.2/.gitignore` & `nexgen-0.9.3/.gitignore`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.2/.pre-commit-config.yaml` & `nexgen-0.9.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.2/.readthedocs.yaml` & `nexgen-0.9.3/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.2/CHANGELOG.md` & `nexgen-0.9.3/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 # CHANGELOG
 
 
+## 0.9.3
+
+### Changed
+- Non-standard "sample_{phi,omega,...}" groups in NXsample made optional and NXclass now set to NXtransformations instead of NXpositioner.
+- Set level of most logs in the NXclass and Nexus writers to DEBUG.
+- Console logs level set to INFO, DEBUG logs only written to file.
+
 
 ## 0.9.2
 
 ### Changed
 - Temporarily disabled external links in NXdetector and detectorSpecific groups which may have wrong data type in meta file.
 Currently unavailable fields: `serial_number`, `data_collection_date`, `eiger_fw_version`.
 - More CI fixes
```

### Comparing `nexgen-0.9.2/CONTRIBUTING.rst` & `nexgen-0.9.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.2/LICENSE` & `nexgen-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.2/PKG-INFO` & `nexgen-0.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nexgen
-Version: 0.9.2
+Version: 0.9.3
 Summary: Next Generation Nexus Generator
 License: BSD 3-Clause License
         
         Copyright (c) 2021, Diamond Light Source
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `nexgen-0.9.2/README.rst` & `nexgen-0.9.3/README.rst`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.2/docs/Makefile` & `nexgen-0.9.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.2/docs/api.rst` & `nexgen-0.9.3/docs/api.rst`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.2/docs/api_beamlines.rst` & `nexgen-0.9.3/docs/api_beamlines.rst`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.2/docs/beamlines.rst` & `nexgen-0.9.3/docs/beamlines.rst`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.2/docs/conf.py` & `nexgen-0.9.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.2/docs/make.bat` & `nexgen-0.9.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.2/docs/usage.rst` & `nexgen-0.9.3/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.2/pyproject.toml` & `nexgen-0.9.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=64", "setuptools_scm[toml]>=8.0.1", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nexgen"
-version = "0.9.2"
+version = "0.9.3"
 description = "Next Generation Nexus Generator"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: BSD License",
     "Natural Language :: English",
     "Programming Language :: Python :: 3.10",
```

### Comparing `nexgen-0.9.2/src/nexgen/beamlines/ED_params.py` & `nexgen-0.9.3/src/nexgen/beamlines/ED_params.py`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.2/src/nexgen/beamlines/ED_singla_nxs.py` & `nexgen-0.9.3/src/nexgen/beamlines/ED_singla_nxs.py`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.2/src/nexgen/beamlines/GDAtools/ExtendedRequest.py` & `nexgen-0.9.3/src/nexgen/beamlines/GDAtools/ExtendedRequest.py`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.2/src/nexgen/beamlines/GDAtools/GDAjson2params.py` & `nexgen-0.9.3/src/nexgen/beamlines/GDAtools/GDAjson2params.py`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.2/src/nexgen/beamlines/I19_2_gda_nxs.py` & `nexgen-0.9.3/src/nexgen/beamlines/I19_2_gda_nxs.py`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.2/src/nexgen/beamlines/I19_2_nxs.py` & `nexgen-0.9.3/src/nexgen/beamlines/I19_2_nxs.py`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.2/src/nexgen/beamlines/I19_2_params.py` & `nexgen-0.9.3/src/nexgen/beamlines/I19_2_params.py`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.2/src/nexgen/beamlines/I24_params.py` & `nexgen-0.9.3/src/nexgen/beamlines/I24_params.py`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.2/src/nexgen/beamlines/SSX_Eiger_nxs.py` & `nexgen-0.9.3/src/nexgen/beamlines/SSX_Eiger_nxs.py`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.2/src/nexgen/beamlines/SSX_Tristan_nxs.py` & `nexgen-0.9.3/src/nexgen/beamlines/SSX_Tristan_nxs.py`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.2/src/nexgen/beamlines/SSX_chip.py` & `nexgen-0.9.3/src/nexgen/beamlines/SSX_chip.py`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.2/src/nexgen/beamlines/SSX_expt.py` & `nexgen-0.9.3/src/nexgen/beamlines/SSX_expt.py`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.2/src/nexgen/beamlines/beamline_utils.py` & `nexgen-0.9.3/src/nexgen/beamlines/beamline_utils.py`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.2/src/nexgen/command_line/ED_mrc_to_nexus.py` & `nexgen-0.9.3/src/nexgen/command_line/ED_mrc_to_nexus.py`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.2/src/nexgen/command_line/ED_nexus.py` & `nexgen-0.9.3/src/nexgen/command_line/ED_nexus.py`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.2/src/nexgen/command_line/I19_2_cli.py` & `nexgen-0.9.3/src/nexgen/command_line/I19_2_cli.py`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.2/src/nexgen/command_line/SSX_cli.py` & `nexgen-0.9.3/src/nexgen/command_line/SSX_cli.py`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.2/src/nexgen/command_line/__init__.py` & `nexgen-0.9.3/src/nexgen/command_line/__init__.py`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.2/src/nexgen/command_line/cli_utils.py` & `nexgen-0.9.3/src/nexgen/command_line/cli_utils.py`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.2/src/nexgen/command_line/copy_nexus.py` & `nexgen-0.9.3/src/nexgen/command_line/copy_nexus.py`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.2/src/nexgen/command_line/nexus_generator.py` & `nexgen-0.9.3/src/nexgen/command_line/nexus_generator.py`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.2/src/nexgen/command_line/nxs_phil.py` & `nexgen-0.9.3/src/nexgen/command_line/nxs_phil.py`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.2/src/nexgen/command_line/phil_files_cli.py` & `nexgen-0.9.3/src/nexgen/command_line/phil_files_cli.py`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.2/src/nexgen/log.py` & `nexgen-0.9.3/src/nexgen/log.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
         "default": {
             "class": "logging.Formatter",
             "format": "%(levelname)s - %(message)s",
         }
     },
     "handlers": {
         "console": {
-            "level": "DEBUG",
+            "level": "INFO",
             "class": "logging.StreamHandler",
             "formatter": "default",
             "stream": "ext://sys.stdout",
         }
     },
     "loggers": {
         "nexgen": {
```

### Comparing `nexgen-0.9.2/src/nexgen/nxs_copy/copy_nexus.py` & `nexgen-0.9.3/src/nexgen/nxs_copy/copy_nexus.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,29 +36,27 @@
     Returns:
         nxs_filename (str): Filename of new NeXus file.
     """
     copy_logger.info("Copying NeXus file for image dataset ...")
     data_file = [Path(d).expanduser().resolve() for d in data_file]
     original_nexus = Path(original_nexus).expanduser().resolve()
     nxs_filename = get_nexus_filename(data_file[0], copy=True)
-    copy_logger.info(f"New NeXus file name: {nxs_filename}")
-    with h5py.File(original_nexus, "r") as nxs_in, h5py.File(
-        nxs_filename, "x"
-    ) as nxs_out:
+    copy_logger.debug(f"New NeXus file name: {nxs_filename}")
+    with h5py.File(original_nexus, "r") as nxs_in, h5py.File(nxs_filename, "x") as nxs_out:
         if simple_copy is True:
             # Copy the whole tree
             get_nexus_tree(nxs_in, nxs_out, skip=False)
         else:
             copy_logger.warning(
                 f"The following NX base classes will not be copied: {skip_group}"
             )
             nxs_out.attrs["default"] = "entry"
             # Copy the whole tree except for nxdata and whatever other group was passed.
             nxentry = get_nexus_tree(nxs_in, nxs_out, skip=True, skip_obj=skip_group)
-            copy_logger.info(f"Re write NXdata with link to {data_file[0]}.")
+            copy_logger.debug(f"Re write NXdata with link to {data_file[0]}.")
             if "NXdata" in skip_group:  # it always is...
                 # Create nxdata group
                 nxdata = nxentry.create_group("data")
                 # Find and copy only scan axis information
                 for k in nxs_in["entry/data"].keys():
                     if "depends_on" in nxs_in["entry/data"][k].attrs.keys():
                         ax = k
@@ -89,15 +87,15 @@
     Returns:
         nxs_filename (str): Filename of new NeXus file.
     """
     copy_logger.info("Copying NeXus file for events dataset ...")
     data_file = [Path(d).expanduser().resolve() for d in data_file]
     original_nexus = Path(original_nexus).expanduser().resolve()
     nxs_filename = get_nexus_filename(data_file[0], copy=True)
-    copy_logger.info(f"New NeXus file name: {nxs_filename}")
+    copy_logger.debug(f"New NeXus file name: {nxs_filename}")
     with h5py.File(original_nexus, "r") as nxs_in, h5py.File(
         nxs_filename, "x"
     ) as nxs_out:
         nxs_out.attrs["default"] = "entry"
         # Copy the whole tree except for nxdata
         nxentry = get_nexus_tree(nxs_in, nxs_out)
         # Create nxdata group
```

### Comparing `nexgen-0.9.2/src/nexgen/nxs_copy/copy_tristan_nexus.py` & `nexgen-0.9.3/src/nexgen/nxs_copy/copy_tristan_nexus.py`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.2/src/nexgen/nxs_copy/copy_utils.py` & `nexgen-0.9.3/src/nexgen/nxs_copy/copy_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -129,25 +129,33 @@
     Args:
         nxsample (h5py.Group): NXsample group of NeXus file to be modified.
         nxdata (h5py.Group): NXdata group of NeXus file to be modified.
         ax (str): Name of scan_axis.
         ax_range (ArrayLike): Scan points. If passed, axis_increment_set and axis_end will also be written.\
             Defaults to None
     """
-    del nxsample["transformations/" + ax]
-    nxsample["transformations/" + ax] = nxdata[ax]
-    name = (
-        "sample_" + ax + "/" + ax if "sam" not in ax else "sample_" + ax[-1] + "/" + ax
-    )
-    del nxsample[name]
-    nxsample[name] = nxdata[ax]
+    del nxsample[f"transformations/{ax}"]
+    nxsample[f"transformations/{ax}"] = nxdata[ax]
+    grp_name = f"sample_{ax}" if "sam" not in ax else f"sample_{ax[-1]}"
+    old_exists = grp_name in list(nxsample.keys())
+    if old_exists:
+        del nxsample[grp_name]
+        nxsample[f"{grp_name}/{ax}"] = nxdata[ax]
     if ax_range is not None and "sam" not in ax:
         increment = round(ax_range[1] - ax_range[0], 3)
-        nxsample["sample_" + ax].create_dataset(ax + "_increment_set", data=increment)
-        nxsample["sample_" + ax].create_dataset(ax + "_end", data=ax_range + increment)
+        end = ax_range + increment
+        nxsample["transformations"].create_dataset(
+            f"{ax}_increment_set", data=increment
+        )
+        nxsample["transformations"].create_dataset(f"{ax}_end", data=end)
+        if old_exists:
+            nxsample[f"{grp_name}/{ax}_increment_set"] = nxsample[
+                f"transformations/{ax}_increment_set"
+            ]
+            nxsample[f"{grp_name}/{ax}_end"] = nxsample[f"transformations/{ax}_end"]
 
 
 def check_and_fix_det_axis(nxs_in: h5py.File):
     det_z_grp = nxs_in["/entry/instrument/detector/transformations/detector_z"]
     det_z = det_z_grp["det_z"]
     if isinstance(det_z[()], bytes) or isinstance(det_z[()], str):
         det_z_attrs = {}
```

### Comparing `nexgen-0.9.2/src/nexgen/nxs_utils/__init__.py` & `nexgen-0.9.3/src/nexgen/nxs_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.2/src/nexgen/nxs_utils/axes.py` & `nexgen-0.9.3/src/nexgen/nxs_utils/axes.py`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.2/src/nexgen/nxs_utils/detector.py` & `nexgen-0.9.3/src/nexgen/nxs_utils/detector.py`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.2/src/nexgen/nxs_utils/goniometer.py` & `nexgen-0.9.3/src/nexgen/nxs_utils/goniometer.py`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.2/src/nexgen/nxs_utils/scan_utils.py` & `nexgen-0.9.3/src/nexgen/nxs_utils/scan_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,19 +9,17 @@
 from enum import IntEnum
 from typing import Dict, List
 
 from numpy.typing import ArrayLike
 from scanspec.core import Path as ScanPath
 from scanspec.specs import Line
 
-from .. import log
 from .axes import Axis
 
 scan_logger = logging.getLogger("nexgen.ScanUtils")
-log.config()
 
 # Some options for grid scans
 GridScanOptions = namedtuple("GridScanOptions", ("axes_order", "snaked"))
 GridScanOptions.__doc__ = "Options for defining a grid scan"
 GridScanOptions.axes_order.__doc__ = "List of axes in order of (fast, slow)."
 GridScanOptions.snaked.__doc__ = "Boolean to say whether it's a snaked scan."
```

### Comparing `nexgen-0.9.2/src/nexgen/nxs_utils/source.py` & `nexgen-0.9.3/src/nexgen/nxs_utils/source.py`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.2/src/nexgen/nxs_write/nxclass_writers.py` & `nexgen-0.9.3/src/nexgen/nxs_write/nxclass_writers.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,14 +27,15 @@
     get_iso_timestamp,
     units_of_length,
     units_of_time,
     ureg,
 )
 from .write_utils import (
     TSdset,
+    add_sample_axis_groups,
     calculate_origin,
     create_attributes,
     mask_and_flatfield_writer,
     mask_and_flatfield_writer_for_event_data,
     set_dependency,
 )
 
@@ -69,46 +70,39 @@
     return nxentry
 
 
 # NXdata writer
 def write_NXdata(
     nxsfile: h5py.File,
     datafiles: List[Path],
-    goniometer_axes: List[Axis],
     data_type: str,
-    osc_scan: Dict[str, ArrayLike],
-    transl_scan: Dict[str, ArrayLike] = None,
+    osc_axis: str = "omega",
     entry_key: str = "data",
 ):
     """
     Write NXdata group at /entry/data.
 
     Args:
         nxsfile (h5py.File): NeXus file handle.
         datafiles (List[Path]): List of Path objects pointing to HDF5 data files.
-        goniometer_axes (List[Axis]): List of goniometer axes.
         data_type (str): Images or events.
-        osc_scan (Dict[str, ArrayLike]): Rotation scan. If writing events, this is just a (start, end) tuple.
-        transl_scan (Dict[str, ArrayLike], optional): Scan along the xy axes at sample. Defaults to None.
+        osc_scan (str, optional): Rotation scan axis name. Defaults to omega.
         entry_key (str): Entry key to create the external links to the data files. Defaults to data.
 
     Raises:
         OSError: If no data is passed.
-        ValueError: If the data typs is neither "images" nor "events".
+        ValueError: If the data type is neither "images" nor "events".
     """
-    NXclass_logger.info("Start writing NXdata.")
+    NXclass_logger.debug("Start writing NXdata.")
     # Check that a valid datafile_list has been passed.
     if len(datafiles) == 0:
         raise OSError(
             "No HDF5 data filenames have been found. Please pass at least one."
         )
 
-    # This assumes that a rotation scan is always passed
-    osc_axis, osc_range = list(osc_scan.items())[0]
-
     # Create NXdata group, unless it already exists, in which case just open it.
     nxdata = nxsfile.require_group("/entry/data")
     create_attributes(
         nxdata,
         ("NX_class", "axes", "signal", osc_axis + "_indices"),
         (
             "NXdata",
@@ -145,206 +139,140 @@
         else:
             nxdata["meta_file"] = h5py.ExternalLink(meta[0].name, "/")
     else:
         raise ValueError(
             "Unknown data type. Please pass one value for data_type from : [images, events]"
         )
 
-    # Write rotation axis dataset
-    ax = nxdata.create_dataset(osc_axis, data=osc_range)
-    idx = [n for n, ax in enumerate(goniometer_axes) if ax.name == osc_axis][0]
-    dep = set_dependency(
-        goniometer_axes[idx].depends, path="/entry/sample/transformations/"
-    )
 
-    # Write attributes for axis
+# NXtransformations
+def write_NXtransformations(
+    parent_group: h5py.Group,
+    axes: List[Axis],
+    scan: Optional[Dict[str, ArrayLike]] = None,
+    collection_type: str = "images",
+):
+    """Write NXtransformations group.
+
+    This group coulld be written either in /entry/sample/ for the goniometer or in \
+    /entry/instrument/detector for the detector axes. In the latter case, the scan \
+    should always be None.
+
+    Args:
+        parent_group (h5py.Group): Handle to HDF5 group where NXtransformations \
+            should be written.
+        axes (List[Axis]): List of Axes to write to the NXtransformations group.
+        scan (Optional[Dict[str, ArrayLike]], optional): All the scan axes, both \
+            rotation and translation. Defaults to None.
+        collection_type (str, optional): Collection type, could be images or \
+            events. Defaults to "images".
+    """
+    NXclass_logger.debug(f"Start writing NXtransformations group in {parent_group}.")
+    nxtransformations = parent_group.require_group("transformations")
     create_attributes(
-        ax,
-        ("depends_on", "transformation_type", "units", "vector"),
-        (
-            dep,
-            goniometer_axes[idx].transformation_type,
-            goniometer_axes[idx].units,
-            goniometer_axes[idx].vector,
-        ),
+        nxtransformations,
+        ("NX_class",),
+        ("NXtransformations",),
     )
 
-    # If present, add linear/grid scan details
-    if transl_scan:
-        for k, v in transl_scan.items():
-            ax_dset = nxdata.create_dataset(k, data=v)
-            ax_idx = [n for n, ax in enumerate(goniometer_axes) if ax.name == k][0]
-            ax_dep = set_dependency(
-                goniometer_axes[ax_idx].depends, path="/entry/sample/transformations/"
-            )
-            create_attributes(
-                ax_dset,
-                ("depends_on", "transformation_type", "units", "vector"),
-                (
-                    ax_dep,
-                    goniometer_axes[ax_idx].transformation_type,
-                    goniometer_axes[ax_idx].units,
-                    goniometer_axes[ax_idx].vector,
-                ),
-            )
+    for ax in axes:
+        # Dataset
+        data = (
+            scan[ax.name]
+            if scan and ax.name in scan.keys()
+            else np.array([ax.start_pos])
+        )
+        # Dependency
+        ax_dep = set_dependency(ax.depends, path=nxtransformations.name)
+
+        nxax = nxtransformations.create_dataset(ax.name, data=data)
+        create_attributes(
+            nxax,
+            ("depends_on", "transformation_type", "units", "vector"),
+            (ax_dep, ax.transformation_type, ax.units, ax.vector),
+        )
+
+        # Write _increment_set and _end for rotation axis
+        if scan and collection_type == "images":
+            if ax.name in scan.keys() and ax.transformation_type == "rotation":
+                NXclass_logger.debug(
+                    f"Adding increment_set and end for axis {ax.name}."
+                )
+                nxtransformations.create_dataset(
+                    f"{ax.name}_increment_set", data=ax.increment
+                )
+                increment_set = np.repeat(ax.increment, len(scan[ax.name]))
+                ax_end = scan[ax.name] + increment_set
+                nxtransformations.create_dataset(f"{ax.name}_end", data=ax_end)
 
 
 # NXsample
 def write_NXsample(
     nxsfile: h5py.File,
     goniometer_axes: List[Axis],
     data_type: str,
     osc_scan: Dict[str, ArrayLike],
     transl_scan: Dict[str, ArrayLike] = None,
     sample_depends_on: str = None,
     sample_details: Dict[str, Any] = None,
+    add_nonstandard_fields: bool = True,
 ):
     """
     Write NXsample group at /entry/sample.
 
     Args:
         nxsfile (h5py.File): NeXus file handle.
         goniometer_axes (List[Axis]): List of goniometer axes.
         data_type (str): Images or events.
         osc_scan (Dict[str, ArrayLike]): Rotation scan. If writing events, this is just a (start, end) tuple.
         transl_scan (Dict[str, ArrayLike], optional): Scan along the xy axes at sample. Defaults to None.
-        sample_depends_on (str, optional): Axis on which the sample depends on. If absent, the depends_on field will be set to the last axis listed in the goniometer. Defaults to None.
+        sample_depends_on (str, optional): Axis on which the sample depends on. If absent, the depends_on field \
+            will be set to the last axis listed in the goniometer. Defaults to None.
         sample_details (Dict[str, Any], optional): General information about the sample, eg. name, temperature.
+        add_nonstandard_fields (bool, optional): Choose whether to add the old "sample_{x,phi,...}/{x,phi,...}" to the group. \
+            These fields are non-standard but may be needed for processing to run. Defaults to True.
     """
-    NXclass_logger.info("Start writing NXsample and NXtransformations.")
+    NXclass_logger.debug("Start writing NXsample.")
     # Create NXsample group, unless it already exists, in which case just open it.
     nxsample = nxsfile.require_group("/entry/sample")
     create_attributes(
         nxsample,
         ("NX_class",),
         ("NXsample",),
     )
 
-    # Create NXtransformations group: /entry/sample/transformations
-    nxtransformations = nxsample.require_group("transformations")
-    create_attributes(
-        nxtransformations,
-        ("NX_class",),
-        ("NXtransformations",),
-    )
+    # Merge the scan dictionaries
+    full_scan = osc_scan if transl_scan is None else osc_scan | transl_scan
 
-    # Get rotation details
-    osc_axis, osc_range = list(osc_scan.items())[0]
+    # Create NXtransformations group: /entry/sample/transformations
+    write_NXtransformations(nxsample, goniometer_axes, full_scan, data_type)
+    if add_nonstandard_fields:
+        add_sample_axis_groups(nxsample, goniometer_axes)
 
     # Save sample depends_on
     if sample_depends_on:
         nxsample.create_dataset(
             "depends_on",
-            data=set_dependency(sample_depends_on, path=nxtransformations.name),
+            data=set_dependency(
+                sample_depends_on, path=nxsample["transformations"].name
+            ),
         )
     else:
         nxsample.create_dataset(
             "depends_on",
-            data=set_dependency(goniometer_axes[-1].name, path=nxtransformations.name),
+            data=set_dependency(
+                goniometer_axes[-1].name, path=nxsample["transformations"].name
+            ),
         )
 
-    # Get xy details if passed
-    scan_axes = []
-    if transl_scan:
-        for k in transl_scan.keys():
-            scan_axes.append(k)
-
-    # Create sample_{axisname} groups
-    for idx, ax in enumerate(goniometer_axes):
-        axis_name = ax.name
-        grp_name = (
-            f"sample_{axis_name[-1]}" if "sam_" in axis_name else f"sample_{axis_name}"
-        )
-        nxsample_ax = nxsample.create_group(grp_name)
-        create_attributes(nxsample_ax, ("NX_class",), ("NXpositioner",))
-        if axis_name == osc_axis:
-            # If we're dealing with the scan axis
-            if (
-                "data" in nxsfile["/entry"].keys()
-                and axis_name in nxsfile["/entry/data"].keys()
-            ):
-                nxsample_ax[axis_name] = nxsfile[nxsfile["/entry/data"][axis_name].name]
-                nxtransformations[axis_name] = nxsfile[
-                    nxsfile["/entry/data"][axis_name].name
-                ]
-            else:
-                nxax = nxsample_ax.create_dataset(axis_name, data=osc_range)
-                _dep = set_dependency(
-                    goniometer_axes[idx].depends, path="/entry/sample/transformations/"
-                )
-                create_attributes(
-                    nxax,
-                    ("depends_on", "transformation_type", "units", "vector"),
-                    (
-                        _dep,
-                        goniometer_axes[idx].transformation_type,
-                        goniometer_axes[idx].units,
-                        goniometer_axes[idx].vector,
-                    ),
-                )
-                nxtransformations[axis_name] = nxsfile[nxax.name]
-            # Write {axisname}_increment_set and {axis_name}_end datasets
-            if data_type == "images":
-                increment_set = np.repeat(
-                    goniometer_axes[idx].increment, len(osc_range)
-                )
-                nxsample_ax.create_dataset(
-                    axis_name + "_increment_set",
-                    data=goniometer_axes[idx].increment,
-                )  # increment_set
-                nxsample_ax.create_dataset(
-                    axis_name + "_end", data=osc_range + increment_set
-                )
-        elif axis_name in scan_axes:
-            # For translations
-            if (
-                "data" in nxsfile["/entry"].keys()
-                and axis_name in nxsfile["/entry/data"].keys()
-            ):
-                nxsample_ax[axis_name] = nxsfile[nxsfile["/entry/data"][axis_name].name]
-                nxtransformations[axis_name] = nxsfile[
-                    nxsfile["/entry/data"][axis_name].name
-                ]
-            else:
-                nxax = nxsample_ax.create_dataset(
-                    axis_name, data=transl_scan[axis_name]
-                )
-                _dep = set_dependency(
-                    goniometer_axes[idx].depends, path="/entry/sample/transformations/"
-                )
-                create_attributes(
-                    nxax,
-                    ("depends_on", "transformation_type", "units", "vector"),
-                    (
-                        _dep,
-                        goniometer_axes[idx].transformation_type,
-                        goniometer_axes[idx].units,
-                        goniometer_axes[idx].vector,
-                    ),
-                )
-                nxtransformations[axis_name] = nxsfile[nxax.name]
-        else:
-            # For all other axes
-            nxax = nxsample_ax.create_dataset(
-                axis_name, data=np.array([goniometer_axes[idx].start_pos])
-            )
-            _dep = set_dependency(
-                goniometer_axes[idx].depends, path="/entry/sample/transformations/"
-            )
-            create_attributes(
-                nxax,
-                ("depends_on", "transformation_type", "units", "vector"),
-                (
-                    _dep,
-                    goniometer_axes[idx].transformation_type,
-                    goniometer_axes[idx].units,
-                    goniometer_axes[idx].vector,
-                ),
-            )
-            nxtransformations[axis_name] = nxsfile[nxax.name]
+    # Add scan axes datasets to NXdata
+    nxdata = nxsfile.require_group("/entry/data")
+    for ax in goniometer_axes:
+        if ax.name in full_scan.keys():
+            nxdata[ax.name] = nxsfile[f"/entry/sample/transformations/{ax.name}"]
 
     # Look for nxbeam in file, if it's there make link
     try:
         nxsample["beam"] = nxsfile["/entry/instrument/beam"]
     except KeyError:
         NXclass_logger.debug(
             "No NXbeam group found elsewhere in the NeXus file." "No link written."
@@ -372,38 +300,38 @@
         nxsfile (h5py.File): NeXus file handle.
         beam (Dict):Dictionary with beam information, mainly wavelength and flux.
         attenuator (Dict): Dictionary containing transmission.
         source (Source): Source definition, containing the facility information.
         reset_instrument_name (bool, optional): If True, a string with the name of the \
             instrument used. Otherwise, it will be set to 'DIAMOND BEAMLINE Ixx'. Defaults to False.
     """
-    NXclass_logger.info("Start writing NXinstrument.")
+    NXclass_logger.debug("Start writing NXinstrument.")
     # Create NXinstrument group, unless it already exists, in which case just open it.
     nxinstrument = nxsfile.require_group("/entry/instrument")
     create_attributes(
         nxinstrument,
         ("NX_class",),
         ("NXinstrument",),
     )
 
     # Write /name field and relative attribute
-    NXclass_logger.info(f"{source.short_name} {source.beamline}")
+    NXclass_logger.debug(f"{source.short_name} {source.beamline}")
     name_str = (
         source.set_instrument_name()
         if reset_instrument_name
         else f"DIAMOND BEAMLINE {source.beamline}"
     )
     nxinstrument.create_dataset("name", data=np.string_(name_str))
     create_attributes(
         nxinstrument["name"],
         ("short_name",),
         (f"{source.short_name} {source.beamline}",),
     )
 
-    NXclass_logger.info("Write NXattenuator and NXbeam.")
+    NXclass_logger.debug("Write NXattenuator and NXbeam.")
     # Write NXattenuator group: entry/instrument/attenuator
     nxatt = nxinstrument.require_group("attenuator")
     create_attributes(nxatt, ("NX_class",), ("NXattenuator",))
     if attenuator.transmission:
         nxatt.create_dataset(
             "attenuator_transmission",
             data=attenuator.transmission,
@@ -424,15 +352,15 @@
     """
     Write NXsource group /in entry/source.
 
     Args:
         nxsfile (h5py.File): NeXus file handle.
         source (Source): Source definition, containing the facility information.
     """
-    NXclass_logger.info("Start writing NXsource.")
+    NXclass_logger.debug("Start writing NXsource.")
     nxsource = nxsfile.require_group("/entry/source")
     create_attributes(
         nxsource,
         ("NX_class",),
         ("NXsource",),
     )
 
@@ -455,15 +383,15 @@
 
     Args:
         nxsfile (h5py.File): NeXus file handle.
         detector (Detector): Detector definition.
         num_images (int, optional): Total number of images in collections. Defaults to None
         meta (Path, optional): Path to _meta.h5 file. Defaults to None.
     """
-    NXclass_logger.info("Start writing NXdetector.")
+    NXclass_logger.debug("Start writing NXdetector.")
     # Create NXdetector group, unless it already exists, in which case just open it.
     nxdetector = nxsfile.require_group("/entry/instrument/detector")
     create_attributes(
         nxdetector,
         ("NX_class",),
         ("NXdetector",),
     )
@@ -477,15 +405,15 @@
     )
 
     collection_mode = detector.get_detector_mode()
 
     # If there is a meta file, a lot of information will be linked instead of copied
     if isinstance(detector.detector_params, EigerDetector):
         if meta:
-            NXclass_logger.info(f"Found metadata in {meta.as_posix()} file.")
+            NXclass_logger.debug(f"Found metadata in {meta.as_posix()} file.")
             meta_link = (
                 meta.name
                 if meta.parent == Path(nxsfile.filename).parent
                 else meta.as_posix()
             )
             for k, v in detector.detector_params.constants.items():
                 if k in [
@@ -500,15 +428,15 @@
                     # TODO re-enable eiger_fw_version, date & serial_number
                     # see https://github.com/DiamondLightSource/nexgen/issues/236
                     continue
                 nxdetector[k] = h5py.ExternalLink(meta_link, v)
         else:
             NXclass_logger.warning(
                 """
-                Meta file for Eiger detector hasn't been specified.
+                Meta file for Eiger detector hasn't been specified or found.
                 No links will be written. Pixel mask and flatfield information missing.
                 """
             )
     else:
         # If it's an eiger mask and flatfield will be in the links along with other info.
         # If it isn't, the mask and flatfield info still needs to go in
         NXclass_logger.info("Gathering and writing pixel_mask and flatfield to file.")
@@ -598,65 +526,45 @@
 
     # Write_NXcollection
     write_NXcollection(
         nxdetector, detector.detector_params, collection_mode, num_images, meta
     )
 
     # Write NXtransformations: entry/instrument/detector/transformations/detector_z and two_theta
-    nxtransformations = nxdetector.require_group("transformations")
-    create_attributes(nxtransformations, ("NX_class",), ("NXtransformations",))
-
-    # Create groups for detector_z and any other detector axis (eg. two_theta) if present
-    # This assumes that the detector axes are fixed.
-    for idx, ax in enumerate(detector.detector_axes):
-        if ax.name == "det_z":
-            grp_name = "detector_z"
-            dist = units_of_length(str(detector.detector_axes[idx].start_pos) + "mm")
-        else:
-            grp_name = ax.name
-
-        # It shouldn't be too much of an issue but just in case ...
-        if detector.detector_axes[idx].depends == "det_z":
-            grp_dep = "detector_z"
-        else:
-            grp_dep = detector.detector_axes[idx].depends
-        _dep = set_dependency(
-            detector.detector_axes[idx].depends,
-            nxtransformations.name + f"/{grp_dep}/",
-        )
-
-        nxgrp_ax = nxtransformations.create_group(grp_name)
-        create_attributes(nxgrp_ax, ("NX_class",), ("NXpositioner",))
-        nxdet_ax = nxgrp_ax.create_dataset(
-            ax.name, data=np.array([detector.detector_axes[idx].start_pos])
-        )
-        create_attributes(
-            nxdet_ax,
-            ("depends_on", "transformation_type", "units", "vector"),
-            (
-                _dep,
-                detector.detector_axes[idx].transformation_type,
-                detector.detector_axes[idx].units,
-                detector.detector_axes[idx].vector,
-            ),
-        )
-        if ax.name == detector.detector_axes[-1].name:
-            # Detector depends_on
-            nxdetector.create_dataset(
-                "depends_on",
-                data=set_dependency(ax.name, path=nxgrp_ax.name),
-            )
+    write_NXtransformations(nxdetector, detector.detector_axes)
+    # NXdetector depends on the last (often only) axis in the list
+    det_dep = set_dependency(
+        detector.detector_axes[-1].name,
+        path="/entry/instrument/detector/transformations",
+    )
+    nxdetector.create_dataset("depends_on", data=det_dep)
+
+    # Just a det_z check
+    if "det_z" not in list(nxdetector["transformations"].keys()):
+        NXclass_logger.error("No det_z field in nexus file.")
+        return
 
-    # Write a soft link for detector_z
-    if "detector_z" in list(nxtransformations.keys()):
-        nxdetector["detector_z"] = nxsfile[
-            "/entry/instrument/detector/transformations/detector_z"
-        ]
+    # Write a soft link for detector_z, workaround for autoPROC
+    # TODO see https://github.com/DiamondLightSource/nexgen/issues/140
+    nxdetector.create_group("detector_z")
+    create_attributes(
+        nxdetector["detector_z"],
+        ("NX_class",),
+        ("NXtransformations",),  # NXtransformations instead of NXpositioner. TOBETESTED
+    )
+    nxdetector["detector_z/det_z"] = nxsfile[
+        "/entry/instrument/detector/transformations/det_z"
+    ]
 
     # Detector distance
+    det_z_idx = [
+        n for n, ax in enumerate(detector.detector_axes) if ax.name == "det_z"
+    ][0]
+    dist = units_of_length(str(detector.detector_axes[det_z_idx].start_pos) + "mm")
+
     nxdetector.create_dataset("distance", data=dist.to("m").magnitude)
     create_attributes(
         nxdetector["distance"], ("units",), (format(dist.to("m").units, "~"))
     )
 
 
 # NXdetector_module writer
@@ -673,15 +581,15 @@
     Args:
         nxsfile (h5py.File): NeXus file handle.
         module (Dict): Dictionary containing the detector module information: fast and slow axes, how many modules.
         image_size (List | Tuple): Size of the detector, in pixels, passed in the order (slow, fast) axis.
         pixel_size (List | Tuple): Size of the single pixels in fast and slow direction, in mm.
         beam_center (Optional[List | Tuple], optional): Beam center position, needed only if origin needs to be calculated. Defaults to None.
     """
-    NXclass_logger.info("Start writing NXdetector_module.")
+    NXclass_logger.debug("Start writing NXdetector_module.")
     # Create NXdetector_module group, unless it already exists, in which case just open it.
     nxmodule = nxsfile.require_group("/entry/instrument/detector/module")
     create_attributes(
         nxmodule,
         ("NX_class",),
         ("NXdetector_module",),
     )
@@ -708,15 +616,15 @@
             "offset",
             "offset_units",
             "transformation_type",
             "units",
             "vector",
         ),
         (
-            "/entry/instrument/detector/transformations/detector_z/det_z",
+            "/entry/instrument/detector/transformations/det_z",
             offsets[0],
             "mm",
             "translation",
             format(x_pix.units, "~"),
             fast_axis,
         ),
     )
@@ -772,15 +680,15 @@
                 "offset",
                 "offset_units",
                 "transformation_type",
                 "units",
                 "vector",
             ),
             (
-                "/entry/instrument/detector/transformations/detector_z/det_z",
+                "/entry/instrument/detector/transformations/det_z",
                 [0, 0, 0],
                 "mm",
                 "translation",
                 format(x_pix.units, "~"),
                 origin,
             ),
         )
@@ -805,15 +713,15 @@
     Args:
         nxdetector (h5py.Group): HDF5 NXdetector group handle.
         detector_params (DetectorType): Parameters specific to the detector in use.
         collection_mode (str, optional): Data type collected by detector. Defaults to "images".
         num_images (int, optional): Total number of images collected. Defaults to None.
         meta (Path, optional): Path to _meta.h5 file. Defaults to None.
     """
-    NXclass_logger.info("Start writing detectorSpecific group as NXcollection.")
+    NXclass_logger.debug("Start writing detectorSpecific group as NXcollection.")
     # Create detectorSpecific group
     grp = nxdetector.require_group("detectorSpecific")
     grp.create_dataset(
         "x_pixels", data=detector_params.image_size[1], dtype=np.uint32
     )  # fast axis
     grp.create_dataset(
         "y_pixels", data=detector_params.image_size[0], dtype=np.uint32
@@ -900,30 +808,30 @@
     Write any additional information as a NXnote class in a specified location in the NeXus file.
 
     Args:
         nxsfile (h5py.File): NeXus file handle.
         loc (str): Location inside the NeXus file to write NXnote group.
         info (Dict): Dictionary of datasets to be written to NXnote.
     """
-    NXclass_logger.info("Start writing NXnote.")
+    NXclass_logger.debug("Start writing NXnote.")
     # Create the NXnote group in the specified location
     nxnote = nxsfile.require_group(loc)
     create_attributes(
         nxnote,
         ("NX_class",),
         ("NXnote",),
     )
 
     # Write datasets
     for k, v in info.items():
         if v:  # Just in case one value is not recorded and set as None
             if isinstance(v, str):
                 v = np.string_(v)
             nxnote.create_dataset(k, data=v)
-            NXclass_logger.info(f"{k} dataset written in {loc}.")
+            NXclass_logger.debug(f"{k} dataset written in {loc}.")
 
 
 def write_NXcoordinate_system_set(
     nxsfile: h5py.File,
     convention: str,
     base_vectors: Dict[str, Axis],
     origin: List | Tuple | ArrayLike,
@@ -964,15 +872,15 @@
     )
 
     # Needs at least: 3 base vectors, depends_on ("." probably?), origin
     transf.create_dataset("depends_on", data=np.string_("."))  # To be checked
     transf.create_dataset("origin", data=origin)
 
     # Base vectors
-    NXclass_logger.info(
+    NXclass_logger.debug(
         "Base vectors: \n"
         f"x: {base_vectors['x'].vector} \n"
         f"y: {base_vectors['y'].vector} \n"
         f"z: {base_vectors['z'].vector} \n"
     )
     idx = 0
     for k, v in base_vectors.items():
```

### Comparing `nexgen-0.9.2/src/nexgen/nxs_write/nxmx_writer.py` & `nexgen-0.9.3/src/nexgen/nxs_write/nxmx_writer.py`

 * *Files 4% similar despite different names*

```diff
@@ -128,23 +128,24 @@
             notes (Dict): Dictionary of (key, value) pairs where key represents the \
                 dataset name and value its data.
             loc (str, optional): Location in the NeXus file to save metadata. \
                 Defaults to "/entry/notes".
         """
         with h5py.File(self.filename, "r+") as nxs:
             write_NXnote(nxs, loc, notes)
-        nxmx_logger.info(f"Notes saved in {loc}.")
+        nxmx_logger.debug(f"Notes saved in {loc}.")
 
     def write(
         self,
         image_datafiles: List | None = None,
         image_filename: str | None = None,
         start_time: datetime | str | None = None,
         est_end_time: datetime | str | None = None,
         write_mode: str = "x",
+        add_non_standard: bool = True,
     ):
         """Write the NXmx format NeXus file.
 
         This function calls the writers for the main NXclass objects.
 
         Args:
             image_datafiles (List | None, optional): List of image data files. If not passed, \
@@ -155,14 +156,16 @@
                 Defaults to None.
             start_time (datetime | str, optional): Collection start time if available, in the \
                 format "%Y-%m-%dT%H:%M:%SZ".Defaults to None.
             est_end_time (datetime | str, optional): Collection estimated end time if available, \
                 in the format "%Y-%m-%dT%H:%M:%SZ". Defaults to None.
             write_mode (str, optional): String indicating writing mode for the output NeXus file. \
                 Accepts any valid h5py file opening mode. Defaults to "x".
+            add_non_standard (bool, optional): Flag if non-standard NXsample fields should be added \
+                for processing to work. Defaults to True, will change in the future.
         """
         metafile = self._get_meta_file(image_filename)
         if metafile:
             nxmx_logger.debug(f"Metafile name: {metafile.as_posix()}.")
 
         datafiles = (
             image_datafiles
@@ -188,18 +191,16 @@
             if est_end_time:
                 write_NXdatetime(nxs, est_end_time, "end_time_estimated")
 
             # NXdata: entry/data
             write_NXdata(
                 nxs,
                 datafiles,
-                self.goniometer.axes_list,
                 "images",
-                osc,
-                transl,
+                list(osc.keys())[0],
             )
 
             # NXinstrument: entry/instrument
             write_NXinstrument(
                 nxs,
                 self.beam,
                 self.attenuator,
@@ -230,14 +231,15 @@
             write_NXsample(
                 nxs,
                 self.goniometer.axes_list,
                 "images",
                 osc,
                 transl,
                 sample_depends_on=None,  # TODO
+                add_nonstandard_fields=add_non_standard,
             )
 
     def write_vds(
         self,
         vds_offset: int = 0,
         vds_shape: Tuple[int, int, int] = None,
         vds_dtype: DTypeLike = np.uint16,
@@ -267,15 +269,15 @@
                     *vds_shape[1:],
                 )
                 nxmx_logger.warning(
                     "The number of scan points doesn't match the calculated vds_shape. \
                     Resetting it to match the number of frames indicated by the scan."
                 )
 
-        nxmx_logger.info(f"VDS shape set to {vds_shape}.")
+        nxmx_logger.debug(f"VDS shape set to {vds_shape}.")
 
         with h5py.File(self.filename, "r+") as nxs:
             if "jungfrau" in self.detector.detector_params.description.lower():
                 jungfrau_vds_writer(
                     nxs,
                     (self.tot_num_imgs, *self.detector.detector_params.image_size),
                     data_type=vds_dtype,
@@ -328,24 +330,27 @@
         )
         self.end_pos = axis_end_position
 
     def write(
         self,
         start_time: datetime | str | None = None,
         write_mode: str = "x",
+        add_non_standard: bool = False,
     ):
         """Write a NXmx-like NeXus file for event mode data collections.
 
         This method overrides the write() method of NXmxFileWriter, from which thsi class inherits.
 
         Args:
             start_time (datetime | str, optional): Collection estimated end time if available, in the format "%Y-%m-%dT%H:%M:%SZ".\
                 Defaults to None.
             write_mode (str, optional): String indicating writing mode for the output NeXus file. Accepts any valid \
                 h5py file opening mode. Defaults to "x".
+            add_non_standard (bool, optional): Flag if non-standard NXsample fields should be added \
+                for processing to work. Defaults to False.
         """
         # Get metafile
         # No data files, just link to meta
         metafile = super()._get_meta_file()
 
         module = self.detector.get_module_info()
 
@@ -361,17 +366,16 @@
             if start_time:
                 write_NXdatetime(nxs, start_time, "start_time")
 
             # NXdata: entry/data
             write_NXdata(
                 nxs,
                 [metafile],
-                self.goniometer.axes_list,
                 "events",
-                osc,
+                list(osc.keys())[0],
             )
 
             # NXinstrument: entry/instrument
             write_NXinstrument(
                 nxs,
                 self.beam,
                 self.attenuator,
@@ -400,14 +404,15 @@
             # NXsample: entry/sample
             write_NXsample(
                 nxs,
                 self.goniometer.axes_list,
                 "events",
                 osc,
                 sample_depends_on=None,  # TODO
+                add_nonstandard_fields=add_non_standard,
             )
 
 
 class EDNXmxFileWriter(NXmxFileWriter):
     """A class to generate NXmx-like NeXus files for electron diffraction.
 
     Requires an additional argument:
@@ -520,17 +525,16 @@
                 est_end = calculate_estimated_end_time(start_time, tot_exp_time)
                 write_NXdatetime(nxs, est_end, "end_time_estimated")
 
             # NXdata: entry/data
             write_NXdata(
                 nxs,
                 datafiles,
-                self.goniometer.axes_list,
                 "images",
-                osc,
+                list(osc.keys())[0],
                 entry_key=data_entry_key,
             )
 
             # NXinstrument: entry/instrument
             write_NXinstrument(
                 nxs,
                 self.beam,
@@ -583,15 +587,15 @@
             writer_type (str, optional): Type of vds required. Defaults to "dataset".
             data_entry_key (str, optional): Dataset entry key in datafiles. Defaults to "/entry/data/data".
             datafiles ((List | None, optional): List of image data files. If not passed, the program will look for \
                 files with the stem_######.h5 in the target directory. Defaults to None.
         """
         with h5py.File(self.filename, "r+") as nxs:
             if writer_type == "dataset":
-                nxmx_logger.info(
+                nxmx_logger.debug(
                     "Writing vds dataset as /entry/data/data in nexus file."
                 )
                 image_vds_writer(
                     nxs,
                     (self.tot_num_imgs, *self.detector.detector_params.image_size),
                     data_type=vds_dtype,
                     entry_key=data_entry_key,
```

### Comparing `nexgen-0.9.2/src/nexgen/nxs_write/write_utils.py` & `nexgen-0.9.3/src/nexgen/nxs_write/write_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,46 +11,52 @@
 from typing import List, Literal, Tuple
 
 import h5py  # isort: skip
 import numpy as np
 from hdf5plugin import Bitshuffle, Blosc
 from numpy.typing import ArrayLike
 
+from ..nxs_utils import Axis
+
 # Logger
 NXclassUtils_logger = logging.getLogger("nexgen.NXclass_writers.utils")
 NXclassUtils_logger.setLevel(logging.DEBUG)
 
 # Define Timestamp dataset names
 TSdset = Literal["start_time", "end_time", "end_time_estimated"]
 
 
 def create_attributes(nxs_obj: h5py.Group | h5py.Dataset, names: Tuple, values: Tuple):
     """
     Create or overwrite attributes with additional metadata information.
 
     Args:
-        nxs_obj (h5py.Group | h5py.Dataset): NeXus object to which the attributes should be attached.
+        nxs_obj (h5py.Group | h5py.Dataset): NeXus object to which the \
+            attributes should be attached.
         names (Tuple): The names of the new attributes.
         values (Tuple): The attribute values asociated to the names.
     """
     for n, v in zip(names, values):
         if isinstance(v, str):
             # If a string, convert to numpy.string_
             v = np.string_(v)
         h5py.AttributeManager.create(nxs_obj, name=n, data=v)
 
 
 def set_dependency(dep_info: str, path: str = None):
     """
     Define value for "depends_on" attribute.
-    If the attribute points to the head of the dependency chain, simply pass "." for dep_info.
+    If the attribute points to the head of the dependency chain, simply pass \
+        "." for dep_info.
 
     Args:
-        dep_info (str): The name of the transformation upon which the current one depends on.
-        path (str): Where the transformation is. Set to None, if passed it points to location in the NeXus tree.
+        dep_info (str): The name of the transformation upon which the current \
+            one depends on.
+        path (str): Where the transformation is. Set to None, if passed it \
+            points to location in the NeXus tree.
     Returns:
         The value to be passed to the attribute "depends_on"
     """
     if dep_info == ".":
         return np.string_(".")
     if path:
         if path.endswith("/") is False:
@@ -66,31 +72,37 @@
     fast_axis_vector: Tuple,
     slow_axis_vector: Tuple,
     mode: str = "1",
 ) -> Tuple[List, float]:
     """
     Calculate the offset of the detector.
 
-    This function returns the detector origin array, which is saved as the vector attribute of the module_offset field.
-    The value to set the module_offset to is also returned: the magnitude of the displacement if the vector is normalized, 1.0 otherwise
-    Assumes that fast and slow axis vectors have already been converted to mcstas if needed.
+    This function returns the detector origin array, which is saved as the \
+        vector attribute of the module_offset field.
+    The value to set the module_offset to is also returned: the magnitude of \
+        the displacement if the vector is normalized, 1.0 otherwise
+    Assumes that fast and slow axis vectors have already been converted to \
+        mcstas if needed.
 
     Args:
         beam_center_fs (List | Tuple): Beam center position in fast and slow direction.
         fs_pixel_size (List | Tuple): Pixel size in fast and slow direction, in m.
         fast_axis_vector (Tuple): Fast axis vector.
         slow_axis_vector (Tuple): Slow axis vector.
         mode (str, optional): Decide how origin should be calculated.
-                            If set to "1" the displacement vector is un-normalized and the offset value set to 1.0.
-                            If set to "2" the displacement is normalized and the offset value is set to the magnitude of the displacement.
-                            Defaults to "1".
+            If set to "1" the displacement vector is un-normalized \
+                and the offset value set to 1.0.
+            If set to "2" the displacement is normalized and the \
+                offset value is set to the magnitude of the displacement.
+            Defaults to "1".
 
     Returns:
         det_origin (List): Displacement of beam center, vector attribute of module_offset.
-        offset_val (float): Value to assign to module_offset, depending whether det_origin is normalized or not.
+        offset_val (float): Value to assign to module_offset, depending whether \
+            det_origin is normalized or not.
     """
     # what was calculate module_offset
     x_scaled = beam_center_fs[0] * fs_pixel_size[0]
     y_scaled = beam_center_fs[1] * fs_pixel_size[1]
     # Detector origin
     det_origin = x_scaled * np.array(fast_axis_vector) + y_scaled * np.array(
         slow_axis_vector
@@ -105,15 +117,16 @@
 
 def find_number_of_images(datafile_list: List[Path], entry_key: str = "data") -> int:
     """
     Calculate total number of images when there's more than one input HDF5 file.
 
     Args:
         datafile_list (List[Path]): List of paths to the input image files.
-        entry_key (str):    Key for the location of the images inside the data files. Defaults to "data".
+        entry_key (str):    Key for the location of the images inside the \
+            data files. Defaults to "data".
 
     Returns:
         num_images (int): Total number of images.
     """
     num_images = 0
     for filename in datafile_list:
         with h5py.File(filename, "r") as f:
@@ -136,25 +149,26 @@
 
 def mask_and_flatfield_writer(
     nxdet_grp: h5py.Group,
     dset_name: str,
     dset_data: str | ArrayLike,
     applied_val: bool,
 ):
-    """ Utility function to write mask or flatfield to NXdetector group for image data when not \
-    already linked to the _meta.h5 file.
-    If the pixel_mask/flatfield data is passed as a string, it will be assumed to be a file path and \
-    the writer will try to set up an external link to it.
+    """ Utility function to write mask or flatfield to NXdetector group for \
+        image data when not already linked to the _meta.h5 file.
+    If the pixel_mask/flatfield data is passed as a string, it will be assumed \
+        to be a file path and the writer will try to set up an external link to it.
 
     Args:
         nxdet_grp (h5py.Group): Handle to HDF5 NXdetector group.
         dset_name (str): Name of the new field/dataset to be written.
-        dset_data (str | ArrayLike): Dataset data to be written in the field. Can be a string or an \
-        array-like dataset. If the data type is a numpy ndarray, it will be compressed before writing.
-        applied_val (bool): Value to write to the `{flatfield,pixel_mask}_applied` fields.
+        dset_data (str | ArrayLike): Dataset data to be written in the field. \
+            Can be a string or an array-like dataset. \
+            If the data type is a numpy ndarray, it will be compressed before writing.
+        applied_val (bool): Value to write to `{flatfield,pixel_mask}_applied` fields.
     """
     if dset_data is None:
         NXclassUtils_logger.warning(
             f"""
             No copy of the {dset_name} has been found, either as a file or dataset.
             Fields {dset_name} and {dset_name}_applied will not be written to file.
             """
@@ -200,20 +214,22 @@
     if dset_data_file is None:
         NXclassUtils_logger.warning(
             f"No {dset_name} data file passed; {dset_name} won't be written."
         )
         return
 
     nxdet_grp.create_dataset(f"{dset_name}_applied", data=applied_val)
-    NXclassUtils_logger.info(f"Looking for file {dset_data_file} in {wdir.as_posix()}.")
+    NXclassUtils_logger.debug(
+        f"Looking for file {dset_data_file} in {wdir.as_posix()}."
+    )
     filename = [
         wdir / dset_data_file for f in wdir.iterdir() if dset_data_file == f.name
     ]
     if filename:
-        NXclassUtils_logger.info(f"File {dset_name} found in working directory.")
+        NXclassUtils_logger.debug(f"File {dset_name} found in working directory.")
         write_compressed_copy(
             nxdet_grp,
             dset_name,
             filename=filename[0],
             filter_choice="blosc",
             dset_key="image",
         )
@@ -235,42 +251,50 @@
     data: ArrayLike = None,
     filename: Path | str = None,
     filter_choice: str = "bitshuffle",
     dset_key: str = "image",
     **kwargs,
 ):
     """
-    Write a compressed copy of some dataset in the desired HDF5 group, using the filter of choice with lz4 compression. Available filters \
-    at this time include "Blosc" and "Bitshuffle" (default).
-    The main application for this function in nexgen is to write a compressed copy of a pixel mask or a flatfield file/dataset \
-    directly into the NXdetector group of a NXmx NeXus file.
-    The data and filename arguments are mutually exclusive as only one of them can be used as input.
-    If a filename is passed, it is also required to pass the key for the relevant dataset to be copied. Failure to do so will result \
-    in nothing being written to the NeXus file.
+    Write a compressed copy of some dataset in the desired HDF5 group, using \
+        the filter of choice with lz4 compression. Available filters at this \
+        time include "Blosc" and "Bitshuffle" (default).
+    The main application for this function in nexgen is to write a compressed \
+        copy of a pixel mask or a flatfield file/dataset directly into the \
+        NXdetector group of a NXmx NeXus file.
+    The data and filename arguments are mutually exclusive as only one of them \
+        can be used as input.
+    If a filename is passed, it is also required to pass the key for the \
+        relevant dataset to be copied. Failure to do so will result in nothing being \
+        written to the NeXus file.
 
     Args:
         nxgroup (h5py.Group): Handle to HDF5 group.
         dset_name (str): Name of the new dataset to be written.
         data (ArrayLike, optional): Dataset to be compressed. Defaults to None.
-        filename (Path | str, optional): Filename containing the dataset to be compressed into the NeXus file. Defaults to None.
-        filter_choice (str, optional): Filter to be used for compression. Either blosc or bitshuffle. Defaults to bitshuffle.
-        dset_key (str, optional): Dataset name inside the passed file. Defaults to "image".
+        filename (Path | str, optional): Filename containing the dataset to be \
+            compressed into the NeXus file. Defaults to None.
+        filter_choice (str, optional): Filter to be used for compression. \
+            Either blosc or bitshuffle. Defaults to bitshuffle.
+        dset_key (str, optional): Dataset name inside the passed file. \
+            Defaults to "image".
 
     Keyword Args:
-        block_size (int, optional): Number of elements per block, it needs to be divisible by 8. Needed for Bitshuffle filter. \
-            Defaults to 0.
+        block_size (int, optional): Number of elements per block, it needs to \
+            be divisible by 8. Needed for Bitshuffle filter. Defaults to 0.
 
     Raises:
         ValueError: If both a dataset and a filename have been passed to the function.
     """
     if data is not None and filename is not None:
         raise ValueError(
             "The dset and filename arguments are mutually exclusive."
             "Please pass only the one from which the data should be copied."
         )
+
     if filename and not dset_key:
         NXclassUtils_logger.warning(
             f"Missing key to find the dataset to be copied inside {filename}. {dset_name} will not be written into the NeXus file."
         )
         return
 
     if filename:
@@ -292,7 +316,31 @@
         NXclassUtils_logger.warning(
             "Unknown filter choice, no dataset will be written."
         )
         return
     NXclassUtils_logger.info(
         f"A compressed copy of the {dset_name} has been written into the NeXus file."
     )
+
+
+def add_sample_axis_groups(nxsample: h5py.Group, axis_list: List[Axis]):
+    """
+    Add non-standard "sample_{phi,omega,...}" groups to NXsample. These may be needed for \
+    some autoprocessing tools to work correctly.
+
+    Args:
+        nxsample (h5py.Group): NeXus NXsample group.
+        axis_list (List[Axis]): List of goniometer axes.
+    """
+    NXclassUtils_logger.debug("Add non-standard fields for autoPROC to work.")
+    nxtransf = nxsample["transformations"]
+    for ax in axis_list:
+        grp_name = f"sample_{ax.name[-1]}" if "sam" in ax.name else f"sample_{ax.name}"
+        nx_ax = nxsample.require_group(grp_name)
+        # NOTE: NX_class here set to NXtransformations instead of NXpositioner
+        # One step closer to standard.  TO BE TESTED
+        create_attributes(nx_ax, ("NX_class",), ("NXtransformations",))
+        nx_ax[ax.name] = nxtransf[ax.name]
+        if f"{ax.name}_end" in nxtransf.keys():
+            nx_ax[f"{ax.name}_end"] = nxtransf[f"{ax.name}_end"]
+        if f"{ax.name}_increment_set" in nxtransf.keys():
+            nx_ax[f"{ax.name}_increment_set"] = nxtransf[f"{ax.name}_increment_set"]
```

### Comparing `nexgen-0.9.2/src/nexgen/templates/DLS_Template.phil` & `nexgen-0.9.3/src/nexgen/templates/DLS_Template.phil`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.2/src/nexgen/templates/ED_Singla.phil` & `nexgen-0.9.3/src/nexgen/templates/ED_Singla.phil`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.2/src/nexgen/templates/I03_Eiger.phil` & `nexgen-0.9.3/src/nexgen/templates/I03_Eiger.phil`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.2/src/nexgen/templates/I19-2_Eiger.phil` & `nexgen-0.9.3/src/nexgen/templates/I19-2_Eiger.phil`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.2/src/nexgen/templates/I19-2_Tristan.phil` & `nexgen-0.9.3/src/nexgen/templates/I19-2_Tristan.phil`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.2/src/nexgen/templates/I24_Eiger.phil` & `nexgen-0.9.3/src/nexgen/templates/I24_Eiger.phil`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.2/src/nexgen/templates/VMXi.phil` & `nexgen-0.9.3/src/nexgen/templates/VMXi.phil`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.2/src/nexgen/tools/constants.py` & `nexgen-0.9.3/src/nexgen/tools/constants.py`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.2/src/nexgen/tools/data_writer.py` & `nexgen-0.9.3/src/nexgen/tools/data_writer.py`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.2/src/nexgen/tools/ed_tools.py` & `nexgen-0.9.3/src/nexgen/tools/ed_tools.py`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.2/src/nexgen/tools/meta_reader.py` & `nexgen-0.9.3/src/nexgen/tools/meta_reader.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     Raises:
         ValueError: If an invalid detector description is passed. Allowed detectors for this function: Eiger.
     """
     if "eiger" in name.lower():
         meta = DectrisMetafile(meta_file)
         wl = meta.get_wavelength()
         if wl is None:
-            overwrite_logger.info("No wavelength information found in meta file.")
+            overwrite_logger.warning("No wavelength information found in meta file.")
             return
     else:
         raise ValueError("Unknown detector: please pass a valid detector description.")
     # If value exists, overwrite. Otherwise, create.
     overwrite_logger.warning("Wavelength will be overwritten.")
     overwrite_logger.info(f"Value for wavelength found in meta file: {wl}")
     if isinstance(beam, dict):
@@ -86,22 +86,22 @@
         overwrite_logger.info(
             "Found meta_version located at: %s " % new_values["meta_version"]
         )
     elif "eiger" in detector_name:
         meta = DectrisMetafile(meta_file)
         overwrite_logger.info("Looking through meta file for Eiger detector.")
         if meta.hasMask is True:
-            overwrite_logger.info("Mask has been located in meta file")
+            overwrite_logger.debug("Mask has been located in meta file")
             mask_info = meta.find_mask()
             new_values["pixel_mask"] = mask_info[0]
             new_values["pixel_mask_applied"] = mask_info[1]
             link_list[0].append("pixel_mask")
             link_list[0].append("pixel_mask_applied")
         if meta.hasFlatfield is True:
-            overwrite_logger.info("Flatfield has been located in meta file")
+            overwrite_logger.debug("Flatfield has been located in meta file")
             flatfield_info = meta.find_flatfield()
             new_values["flatfield"] = flatfield_info[0]
             new_values["flatfield_applied"] = flatfield_info[1]
             link_list[0].append("flatfield")
             link_list[0].append("flatfield_applied")
         if meta.hasDectrisGroup is True:
             new_values["software_version"] = meta.find_software_version()
@@ -116,37 +116,37 @@
             link_list[1].append("software_version")
             pix = meta.get_pixel_size()
             new_values["pixel_size"] = [
                 units_of_length(pix[0]),
                 units_of_length(pix[1]),
             ]
             overwrite_logger.warning("Pixel_size will be overwritten.")
-            overwrite_logger.info(
+            overwrite_logger.debug(
                 f"Values for x and y pixel size found in meta file: {pix[0]}, {pix[1]}"
             )
             new_values["beam_center"] = meta.get_beam_center()
             overwrite_logger.warning("Beam_center will be overwritten.")
-            overwrite_logger.info(
+            overwrite_logger.debug(
                 f"Values for x and y beam center position found in meta file: "
                 f"{new_values['beam_center']}"
             )
             sensor_info = meta.get_sensor_information()
             new_values["sensor_material"] = sensor_info[0]
             overwrite_logger.warning("Sensor material will be overwritten.")
-            overwrite_logger.info(
+            overwrite_logger.debug(
                 f"Value for sensor material found in meta file: {sensor_info[0]}"
             )
             new_values["sensor_thickness"] = units_of_length(sensor_info[1])
             overwrite_logger.warning("Sensor thickness will be overwritten.")
-            overwrite_logger.info(
+            overwrite_logger.debug(
                 f"Value for sensor thickness found in meta file: {sensor_info[1]}"
             )
             new_values["overload"] = meta.get_saturation_value()
             overwrite_logger.warning("Saturation value (overload) will be overwritten.")
-            overwrite_logger.info(
+            overwrite_logger.debug(
                 f"Value for overload found in meta file: {new_values['overload']}"
             )
     else:
         overwrite_logger.warning("Unknown detector, exit.")
         raise ValueError("Unknown detector: please pass a valid detector description.")
 
     if ignore:
@@ -173,19 +173,19 @@
 
     Args:
         meta_file (DectrisMetafile): Handle to Dectris-shaped meta.h5 file.
 
     Returns:
         DTypeLike: Data type as np.uint##.
     """
-    overwrite_logger.info("Define dtype for VDS creating from bit_depth_image.")
+    overwrite_logger.debug("Define dtype for VDS creating from bit_depth_image.")
     # meta = DectrisMetafile(meta_file)
 
     nbits = meta_file.get_bit_depth_image()
-    overwrite_logger.info(f"Found value for bit_depth_image: {nbits}.")
+    overwrite_logger.debug(f"Found value for bit_depth_image: {nbits}.")
     if nbits == 32:
         return np.uint32
     elif nbits == 8:
         return np.uint8
     else:
         return np.uint16
 
@@ -202,15 +202,15 @@
         meta_file (DectrisMetafile): Handle to Dectris-shaped meta.h5 file.
         axes_list (List[Axis]): List of axes to look up and eventually update.
         osc_axis (str | None, optional): If passed, the number of images corresponding to the osc_axis \
             will be updated too. Defaults to None.
         use_config (bool, optional): If passed read from config dataset in meta file instead of _dectris\
             group. Defaults to False.
     """
-    overwrite_logger.info("Updating axes list with values saved to _dectris group.")
+    overwrite_logger.debug("Updating axes list with values saved to _dectris group.")
     if meta_file.hasDectrisGroup is False:
         overwrite_logger.warning(
             "No Dectris group in meta file. No values will be updated."
         )
         return
 
     if use_config is True and meta_file.hasConfig is True:
@@ -218,20 +218,20 @@
     else:
         config = meta_file.read_dectris_config()
     num = meta_file.get_full_number_of_images()
 
     for ax in axes_list:
         if f"{ax.name}_start" in config.keys():
             ax.start_pos = config[f"{ax.name}_start"]
-            overwrite_logger.info(f"Start value for axis {ax.name}: {ax.start_pos}.")
+            overwrite_logger.debug(f"Start value for axis {ax.name}: {ax.start_pos}.")
             if f"{ax.name}_increment" in config.keys():
                 ax.increment = config[f"{ax.name}_increment"]
-                overwrite_logger.info(
+                overwrite_logger.debug(
                     f"Increment value for axis {ax.name}: {ax.increment}."
                 )
         if osc_axis and ax.name == osc_axis:
             ax.num_steps = num
 
         if ax.name == "det_z":
             dist = units_of_length(meta_file.get_detector_distance())
             ax.start_pos = dist.to("mm").magnitude
-            overwrite_logger.info(f"Start value for axis {ax.name}: {ax.start_pos}.")
+            overwrite_logger.debug(f"Start value for axis {ax.name}: {ax.start_pos}.")
```

### Comparing `nexgen-0.9.2/src/nexgen/tools/metafile.py` & `nexgen-0.9.3/src/nexgen/tools/metafile.py`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.2/src/nexgen/tools/mrc_tools.py` & `nexgen-0.9.3/src/nexgen/tools/mrc_tools.py`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.2/src/nexgen/tools/vds_tools.py` & `nexgen-0.9.3/src/nexgen/tools/vds_tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,15 +126,15 @@
     if not isinstance(start_idx, int):
         vds_logger.warning("VDS start index not passed as int, will attempt to cast")
 
     if vds_shape and not isinstance(vds_shape[0], int):
         vds_logger.warning("VDS start index not passed as int, will attempt to cast")
 
     if vds_shape is None:
-        vds_logger.info(
+        vds_logger.debug(
             "VDS shape not chosen, it will be calculated from the full data shape and the chosen start index."
         )
         vds_shape = (data_shape[0] - start_idx, *data_shape[1:])
 
     full_frames = int(data_shape[0])
     end_cut_frames = int(full_frames - vds_shape[0]) - int(start_idx)
 
@@ -207,15 +207,15 @@
         full_data_shape (Tuple | List): Shape of the full dataset, usually defined as (num_frames, *image_size).
         start_index(int): The start point for the source data. Defaults to 0.
         vds_shape(Tuple, optional): Desired shape of the VDS, usually defined as (num_frames, *image_size). \
             The number of frames must be smaller or equal to the one in full_data_shape. Defaults to None.
         data_type (DTypeLike, optional): The type of the input data. Defaults to np.uint16.
         entry_key (str, optional): Entry key for the Virtual DataSet name. Defaults to data.
     """
-    vds_logger.info("Start creating VDS ...")
+    vds_logger.debug("Start creating VDS ...")
     # Where the vds will go
     nxdata = nxsfile["/entry/data"]
     dset_names = find_datasets_in_file(nxdata)
 
     vds_shape = (
         tuple(vds_shape)
         if vds_shape is not None
@@ -237,15 +237,15 @@
     else:
         datasets = split_datasets(dset_names, full_data_shape, start_index, vds_shape)
 
     layout = create_virtual_layout(datasets, data_type)
 
     # Writea Virtual Dataset in NeXus file
     nxdata.create_virtual_dataset(entry_key, layout, fillvalue=-1)
-    vds_logger.info("VDS written to NeXus file.")
+    vds_logger.debug("VDS correctly written to NeXus file.")
 
 
 def jungfrau_vds_writer(
     nxsfile: h5py.File,
     vds_shape: Tuple | List,
     data_type: DTypeLike = np.uint16,
     source_dsets: List[str] | None = None,
@@ -291,15 +291,15 @@
     Args:
         nxsfile (h5py.File): NeXus file being written.
         datafiles (List[Path]): List of paths to source files.
         data_shape (Tuple | List): Shape of the dataset, usually defined as (num_frames, *image_size).
         data_type (DTypeLike, optional): Dtype. Defaults to np.uint16.
         entry_key (str): Entry key for the Virtual DataSet name. Defaults to data.
     """
-    vds_logger.info("Start creating VDS ...")
+    vds_logger.debug("Start creating VDS file ...")
     # Where the vds will go
     nxdata = nxsfile["/entry/data"]
     # entry_key = "data"
 
     # For every source dataset define its shape and number of frames
     # Once again, it is assumed that the maximum number of frames per dataset is 1000
     frames = (data_shape[0] // 1000) * [1000] + [data_shape[0] % 1000]
@@ -319,15 +319,15 @@
     # Create a _vds.h5 file and add link to nexus file
     s = Path(nxsfile.filename).expanduser().resolve()
     vds_filename = s.parent / f"{s.stem}_vds.h5"
     del s
     with h5py.File(vds_filename, "w") as vds:
         vds.create_virtual_dataset("data", layout, fillvalue=-1)
     nxdata["data"] = h5py.ExternalLink(vds_filename.name, "data")
-    vds_logger.info(f"{vds_filename} written and link added to NeXus file.")
+    vds_logger.debug(f"{vds_filename} written and link added to NeXus file.")
 
 
 def clean_unused_links(
     nxsfile: h5py.File,
     vds_shape: Tuple | List,
     start_index: int = 0,
 ):
@@ -335,29 +335,29 @@
     Remove links to external data not used in VDS.
 
     Args:
         nxsfile (h5py.File): Handle to NeXus file being written.
         vds_shape (Tuple | List): Actual shape of the VDS dataset, usually defined as (num_frames, *image_size).
         start_index(int): The start point for the source data. Defaults to 0.
     """
-    vds_logger.info("Cleaning links unused in VDS ...")
+    vds_logger.debug("Cleaning links unused in VDS ...")
     # Location of the VDS
     nxdata = nxsfile["/entry/data"]
     dataset_names = find_datasets_in_file(nxdata)
     if len(dataset_names) == 1:
-        vds_logger.info("Only one linked file, no need to remove it.")
+        vds_logger.debug("Only one linked file, no need to remove it.")
         return
     datasets = [nxdata[name] for name in dataset_names]
     dataset_lengths = [d.shape[0] for d in datasets]
     if sum(dataset_lengths) == vds_shape[0]:
-        vds_logger.info("All links are used in VDS, no need to remove any.")
+        vds_logger.debug("All links are used in VDS, no need to remove any.")
         return
     for i, _ in enumerate(datasets):
         # unlink datasets before the start of VDS
         if sum(dataset_lengths[0 : i + 1]) < start_index:
-            vds_logger.info(f"Removing {dataset_names[i]} link.")
+            vds_logger.debug(f"Removing {dataset_names[i]} link.")
             del nxdata[dataset_names[i]]
         # unlink datasets after the end of VDS
         if sum(dataset_lengths[0:i]) > start_index + vds_shape[0]:
-            vds_logger.info(f"Removing {dataset_names[i]} link.")
+            vds_logger.debug(f"Removing {dataset_names[i]} link.")
             del nxdata[dataset_names[i]]
-    vds_logger.info("Links unused in VDS removed from NeXus file.")
+    vds_logger.debug("Links unused in VDS removed from NeXus file.")
```

### Comparing `nexgen-0.9.2/src/nexgen/utils.py` & `nexgen-0.9.3/src/nexgen/utils.py`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.2/src/nexgen.egg-info/PKG-INFO` & `nexgen-0.9.3/src/nexgen.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nexgen
-Version: 0.9.2
+Version: 0.9.3
 Summary: Next Generation Nexus Generator
 License: BSD 3-Clause License
         
         Copyright (c) 2021, Diamond Light Source
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `nexgen-0.9.2/src/nexgen.egg-info/SOURCES.txt` & `nexgen-0.9.3/src/nexgen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.2/tests/beamlines/conftest.py` & `nexgen-0.9.3/tests/beamlines/conftest.py`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.2/tests/beamlines/test_GDA_tools.py` & `nexgen-0.9.3/tests/beamlines/test_GDA_tools.py`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.2/tests/beamlines/test_SSX_chip.py` & `nexgen-0.9.3/tests/beamlines/test_SSX_chip.py`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.2/tests/beamlines/test_SSX_expt.py` & `nexgen-0.9.3/tests/beamlines/test_SSX_expt.py`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.2/tests/beamlines/test_SSXwriters.py` & `nexgen-0.9.3/tests/beamlines/test_SSXwriters.py`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.2/tests/beamlines/test_beamline_utils.py` & `nexgen-0.9.3/tests/beamlines/test_beamline_utils.py`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.2/tests/beamlines/test_i19nxs.py` & `nexgen-0.9.3/tests/beamlines/test_i19nxs.py`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.2/tests/cli/test_cli_utils.py` & `nexgen-0.9.3/tests/cli/test_cli_utils.py`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.2/tests/nxs_copy/test_copy_tools.py` & `nexgen-0.9.3/tests/nxs_copy/test_copy_tools.py`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.2/tests/nxs_utils/test_axes.py` & `nexgen-0.9.3/tests/nxs_utils/test_axes.py`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.2/tests/nxs_utils/test_detector.py` & `nexgen-0.9.3/tests/nxs_utils/test_detector.py`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.2/tests/nxs_utils/test_goniometer.py` & `nexgen-0.9.3/tests/nxs_utils/test_goniometer.py`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.2/tests/nxs_utils/test_scan.py` & `nexgen-0.9.3/tests/nxs_utils/test_scan.py`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.2/tests/nxs_utils/test_source.py` & `nexgen-0.9.3/tests/nxs_utils/test_source.py`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.2/tests/nxs_write/conftest.py` & `nexgen-0.9.3/tests/nxs_write/conftest.py`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.2/tests/nxs_write/test_NXclassWriters.py` & `nexgen-0.9.3/tests/nxs_write/test_NXclassWriters.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,23 +23,24 @@
     write_NXdetector,
     write_NXdetector_module,
     write_NXentry,
     write_NXinstrument,
     write_NXnote,
     write_NXsample,
     write_NXsource,
+    write_NXtransformations,
 )
 
 test_module = {"fast_axis": [1, 0, 0], "slow_axis": [0, 1, 0]}
 
 
 def test_given_no_data_files_when_write_NXdata_then_assert_error():
     mock_hdf5_file = MagicMock()
     with pytest.raises(OSError):
-        write_NXdata(mock_hdf5_file, [], [], "", "", [])
+        write_NXdata(mock_hdf5_file, [], "")
 
 
 def test_write_NXentry(dummy_nexus_file):
     entry = write_NXentry(dummy_nexus_file)
 
     assert dummy_nexus_file["/entry/"].attrs["NX_class"] == b"NXentry"
     assert dummy_nexus_file["/entry/"].attrs["default"] == b"data"
@@ -60,146 +61,140 @@
 def test_write_NXSource_with_probe(dummy_nexus_file, mock_source):
     mock_source.probe = "electron"
     write_NXsource(dummy_nexus_file, mock_source)
 
     assert dummy_nexus_file["/entry/source/probe"][()] == b"electron"
 
 
-def test_given_no_data_type_specified_when_write_NXdata_then_exception_raised(
+def test_write_NXtransformations_for_detector_axes(dummy_nexus_file):
+    det_axes = [
+        Axis("two_theta", ".", "rotation", (0, 0, -1), start_pos=90),
+        Axis("det_z", "Two_theta", "translation", (0, 0, 1), start_pos=500),
+    ]
+    nxdet = dummy_nexus_file.require_group("/entry/instrument/detector/")
+    write_NXtransformations(nxdet, det_axes)
+
+    assert "transformations" in nxdet.keys()
+    assert (
+        "det_z" in nxdet["transformations"].keys()
+        and "two_theta" in nxdet["transformations"].keys()
+    )
+    assert_array_equal(nxdet["transformations/det_z"][()], 500)
+    assert_array_equal(nxdet["transformations/two_theta"][()], 90)
+
+
+def test_write_NXtransformations_for_sample_with_rotation_scan(
     dummy_nexus_file, mock_goniometer
 ):
+    nxsample = dummy_nexus_file.require_group("/entry/sample/")
+    write_NXtransformations(nxsample, mock_goniometer.axes_list, mock_goniometer.scan)
+
+    assert "transformations" in nxsample.keys()
+    assert_array_equal(nxsample["transformations/omega"][()], np.arange(0, 90, 1))
+    assert (
+        "omega_increment_set" in nxsample["transformations"].keys()
+        and "omega_end" in nxsample["transformations"].keys()
+    )
+    assert_array_equal(nxsample["transformations/sam_z"][()], 0.0)
+
+
+def test_write_NXtransformations_for_sample_for_events(dummy_nexus_file):
+    axes_list = [Axis("phi", ".", "rotation", (0, 0, -1), start_pos=10)]
+    test_scan = {"phi": (10, 12)}
+    test_gonio = Goniometer(axes_list, test_scan)
+    nxsample = dummy_nexus_file.require_group("/entry/sample/")
+    write_NXtransformations(nxsample, test_gonio.axes_list, test_gonio.scan, "events")
+
+    assert "phi_end" not in nxsample["transformations"].keys()
+    assert_array_equal(nxsample["transformations/phi"], test_scan["phi"])
+
+
+def test_given_no_data_type_specified_when_write_NXdata_then_exception_raised(
+    dummy_nexus_file,
+):
     with pytest.raises(ValueError):
         write_NXdata(
             dummy_nexus_file,
             [Path("tmp")],
-            mock_goniometer.axes_list,
             "",
-            mock_goniometer.scan,
         )
 
 
-def test_given_one_data_file_when_write_NXdata_then_data_in_file(
-    dummy_nexus_file, mock_goniometer
-):
+def test_given_one_data_file_when_write_NXdata_then_data_in_file(dummy_nexus_file):
     write_NXdata(
         dummy_nexus_file,
         [Path("tmp")],
-        mock_goniometer.axes_list,
         "images",
-        mock_goniometer.scan,
+        "omega",
     )
     assert dummy_nexus_file["/entry/data"].attrs["NX_class"] == b"NXdata"
+    assert dummy_nexus_file["/entry/data"].attrs["axes"] == b"omega"
+    assert dummy_nexus_file["/entry/data"].attrs["omega_indices"] == [0]
     assert "data_000001" in dummy_nexus_file["/entry/data"]
 
 
-def test_given_scan_axis_when_write_NXdata_then_axis_in_data_entry_with_correct_data_and_attributes(
-    dummy_nexus_file, mock_goniometer
-):
-    test_axis = "omega"
-    test_scan_range = np.arange(0, 90, 1)
-    axis_entry = f"/entry/data/{test_axis}"
-
-    write_NXdata(
-        dummy_nexus_file,
-        [Path("tmp")],
-        mock_goniometer.axes_list,
-        "images",
-        mock_goniometer.scan,
-    )
-
-    assert test_axis in dummy_nexus_file["/entry/data"]
-    assert_array_equal(test_scan_range, dummy_nexus_file[axis_entry][:])
-    assert dummy_nexus_file[axis_entry].attrs["depends_on"] == b"."
-    assert dummy_nexus_file[axis_entry].attrs["transformation_type"] == b"rotation"
-    assert dummy_nexus_file[axis_entry].attrs["units"] == b"deg"
-    assert_array_equal(dummy_nexus_file[axis_entry].attrs["vector"][:], [-1.0, 0.0, 0])
-
-
-def test_given_scan_axis_when_write_NXsample_then_scan_axis_data_copied_from_data_group_as_well_as_increment_set_and_end(
+def test_given_scan_axis_when_write_NXsample_then_scan_axis_data_written_and_link_to_NXdata_created(
     dummy_nexus_file, mock_goniometer
 ):
     test_axis = "omega"
     test_scan_range = [0, 1, 2]
-    axis_entry = f"/entry/sample/sample_{test_axis}/{test_axis}"
+    axis_entry = f"/entry/sample/transformations/{test_axis}"
     osc_scan = {test_axis: test_scan_range}
 
-    # Doing this to write the scan axis data into the data group
-    write_NXdata(
-        dummy_nexus_file,
-        [Path("tmp")],
-        mock_goniometer.axes_list,
-        "images",
-        osc_scan,
-    )
-
     write_NXsample(
         dummy_nexus_file,
         mock_goniometer.axes_list,
         "images",
         osc_scan,
     )
 
-    assert f"sample_{test_axis}" in dummy_nexus_file["/entry/sample"]
+    assert "transformations" in dummy_nexus_file["/entry/sample"]
     assert_array_equal(test_scan_range, dummy_nexus_file[axis_entry][:])
     assert dummy_nexus_file[axis_entry].attrs["depends_on"] == b"."
     assert dummy_nexus_file[axis_entry].attrs["transformation_type"] == b"rotation"
     assert dummy_nexus_file[axis_entry].attrs["units"] == b"deg"
     assert_array_equal(dummy_nexus_file[axis_entry].attrs["vector"][:], [-1, 0, 0])
     assert_array_equal(dummy_nexus_file[axis_entry + "_increment_set"][()], 1)
     # assert_array_equal(dummy_nexus_file[axis_entry + "_increment_set"][:], [1] * 3)
     assert dummy_nexus_file[axis_entry + "_end"][1] == 2
+    assert f"{test_axis}" in dummy_nexus_file["/entry/data"]
 
 
-def test_given_reverse_rotation_scan_increment_set_and_axis_end_written_correctly(
+def test_given_reverse_rotation_scan_increment_set_and_axis_end_written_correctly_and_old_fields_not_added(
     dummy_nexus_file,
 ):
     test_axis = Axis("phi", ".", TransformationType.ROTATION, (0, 0, -1))
     test_rw_scan = {"phi": np.arange(10, 8, -0.5)}
     test_gonio = Goniometer([test_axis], test_rw_scan)
 
-    # Doing this to write the scan axis data into the data group
-    write_NXdata(
-        dummy_nexus_file,
-        [Path("tmp")],
-        test_gonio.axes_list,
-        "images",
-        test_gonio.scan,
-    )
-
     write_NXsample(
         dummy_nexus_file,
         test_gonio.axes_list,
         "images",
         test_rw_scan,
         sample_depends_on=test_axis.name,
+        add_nonstandard_fields=False,
     )
 
-    axis_entry = f"/entry/sample/sample_{test_axis.name}/{test_axis.name}"
+    axis_entry = f"/entry/sample/transformations/{test_axis.name}"
 
     assert_array_equal(dummy_nexus_file[axis_entry][()], [10.0, 9.5, 9.0, 8.5])
     assert_array_equal(dummy_nexus_file[axis_entry + "_increment_set"][()], -0.5)
     assert_array_equal(dummy_nexus_file[axis_entry + "_end"][()], [9.5, 9.0, 8.5, 8.0])
 
+    assert "sample_phi" not in dummy_nexus_file["/entry/sample"].keys()
+
 
 def test_sample_depends_on_written_correctly_in_NXsample(
     dummy_nexus_file, mock_goniometer
 ):
     test_axis = "omega"
     test_scan_range = [0, 1, 2]
     osc_scan = {test_axis: test_scan_range}
 
-    # Doing this to write the scan axis data into the data group
-    write_NXdata(
-        dummy_nexus_file,
-        [Path("tmp")],
-        mock_goniometer.axes_list,
-        "images",
-        mock_goniometer.scan,
-    )
-
     write_NXsample(
         dummy_nexus_file,
         mock_goniometer.axes_list,
         "images",
         osc_scan,
         sample_depends_on=test_axis,
     )
@@ -217,50 +212,63 @@
 ):
     test_axis = "omega"
     test_scan_range = [0, 1, 2]
     osc_scan = {test_axis: test_scan_range}
 
     test_depends = f"/entry/sample/transformations/{mock_goniometer.axes_list[-1].name}"
 
-    # Doing this to write the scan axis data into the data group
-    write_NXdata(
+    write_NXsample(
         dummy_nexus_file,
-        [Path("tmp")],
         mock_goniometer.axes_list,
         "images",
-        mock_goniometer.scan,
+        osc_scan,
     )
 
+    assert "depends_on" in dummy_nexus_file["/entry/sample"]
+    assert dummy_nexus_file["/entry/sample/depends_on"][()] == test_depends.encode()
+
+
+def test_old_sample_groups_added_correctly_to_NXsample_for_rotation_scan(
+    dummy_nexus_file,
+):
+    test_axes = [
+        Axis("phi", ".", TransformationType.ROTATION, (0, 0, -1)),
+        Axis("sam_z", "phi", TransformationType.TRANSLATION, (0, 0, 1)),
+    ]
+    test_scan = {"phi": np.arange(0, 1, 0.1)}
+    test_gonio = Goniometer(test_axes, test_scan)
+
     write_NXsample(
         dummy_nexus_file,
-        mock_goniometer.axes_list,
+        test_gonio.axes_list,
         "images",
-        osc_scan,
+        test_scan,
+        sample_depends_on=test_axes[0].name,
     )
 
-    assert "depends_on" in dummy_nexus_file["/entry/sample"]
-    assert dummy_nexus_file["/entry/sample/depends_on"][()] == test_depends.encode()
+    sample_path = "/entry/sample/"
+
+    assert "sample_phi" in dummy_nexus_file[sample_path].keys()
+    assert (
+        "sample_z" in dummy_nexus_file[sample_path].keys()
+        and "sam_z" in dummy_nexus_file[sample_path]["sample_z"].keys()
+    )
+    assert_array_equal(
+        dummy_nexus_file[sample_path]["transformations/phi"],
+        dummy_nexus_file[sample_path]["sample_phi/phi"][()],
+    )
 
 
 def test_sample_details_in_NXsample(dummy_nexus_file, mock_goniometer):
 
     test_details = {"name": b"test_sample", "temperature": "25C"}
     test_axis = "omega"
     test_scan_range = [0, 1, 2]
     osc_scan = {test_axis: test_scan_range}
 
-    # Doing this to write the scan axis data into the data group
-    write_NXdata(
-        dummy_nexus_file,
-        [Path("tmp")],
-        mock_goniometer.axes_list,
-        "images",
-        mock_goniometer.scan,
-    )
-
     write_NXsample(
         dummy_nexus_file,
         mock_goniometer.axes_list,
         "images",
         osc_scan,
         sample_details=test_details,
     )
@@ -428,16 +436,16 @@
     assert dummy_nexus_file[det + "x_pixel_size"].attrs["units"] == b"m"
 
     # Check no mask
     assert "pixel_mask" not in list(dummy_nexus_file[det].keys())
 
     # Check detector axis and distance
     tr = det + "transformations/"
-    assert "detector_z" in list(dummy_nexus_file[tr].keys())
-    axis_entry = tr + "detector_z/det_z"
+    assert "det_z" in list(dummy_nexus_file[tr].keys())
+    axis_entry = tr + "det_z"
     assert_array_equal(
         mock_eiger.detector_axes[0].start_pos, dummy_nexus_file[axis_entry][()]
     )
     assert dummy_nexus_file[axis_entry].attrs["depends_on"] == b"."
     assert dummy_nexus_file[axis_entry].attrs["transformation_type"] == b"translation"
     assert dummy_nexus_file[axis_entry].attrs["units"] == b"mm"
     assert_array_equal(
@@ -449,14 +457,15 @@
     assert_array_equal(
         dummy_nexus_file[det + "distance"], mock_eiger.detector_axes[0].start_pos / 1000
     )
     assert dummy_nexus_file[det + "distance"].attrs["units"] == b"m"
 
     # Check that detector_z has also been written in /detector
     assert "detector_z" in list(dummy_nexus_file[det].keys())
+    assert "det_z" in list(dummy_nexus_file[det + "detector_z"].keys())
 
 
 @patch("nexgen.nxs_write.nxclass_writers.write_NXcollection")
 def test_write_NXdetector_for_eiger_images_with_meta_file(
     mock_nxcoll_writer,
     dummy_nexus_file,
     dummy_eiger_meta_file,
```

### Comparing `nexgen-0.9.2/tests/nxs_write/test_NXmxWriter.py` & `nexgen-0.9.3/tests/nxs_write/test_NXmxWriter.py`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.2/tests/nxs_write/test_write_utils.py` & `nexgen-0.9.3/tests/nxs_write/test_write_utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from datetime import datetime
 from pathlib import Path
 from unittest.mock import patch
 
 import numpy as np
 import pytest
 
+from nexgen.nxs_write.nxclass_writers import write_NXtransformations
 from nexgen.nxs_write.write_utils import (
+    add_sample_axis_groups,
     calculate_estimated_end_time,
     calculate_origin,
     create_attributes,
     find_number_of_images,
     mask_and_flatfield_writer,
     mask_and_flatfield_writer_for_event_data,
     set_dependency,
@@ -118,7 +120,20 @@
     assert est_end_time == "2023-11-15T10:30:52Z"
 
 
 def test_calculate_estimated_end_time_from_datetime():
     timestamp = datetime.strptime("2023-11-15T10:30:42", "%Y-%m-%dT%H:%M:%S")
     est_end_time = calculate_estimated_end_time(timestamp, 20)
     assert est_end_time == "2023-11-15T10:31:02Z"
+
+
+def test_add_non_standard_fields_to_NXsample(dummy_nexus_file, mock_goniometer):
+    nxsample_path = "/entry/sample"
+    nxsample = dummy_nexus_file.require_group(nxsample_path)
+    write_NXtransformations(nxsample, mock_goniometer.axes_list, mock_goniometer.scan)
+    add_sample_axis_groups(nxsample, mock_goniometer.axes_list)
+
+    assert "sample_omega" in list(dummy_nexus_file[nxsample_path].keys())
+    assert "sample_z" in list(dummy_nexus_file[nxsample_path].keys())
+    assert "omega_increment_set" in list(
+        dummy_nexus_file[nxsample_path]["sample_omega"]
+    )
```

### Comparing `nexgen-0.9.2/tests/test_log.py` & `nexgen-0.9.3/tests/test_log.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     logger = logging.getLogger("nexgen")
     yield logger
 
 
 def test_basic_logging_config(dummy_logger):
     assert dummy_logger.hasHandlers() is True
     assert len(dummy_logger.handlers) == 1
-    assert dummy_logger.handlers[0].level == logging.DEBUG
+    assert dummy_logger.handlers[0].level == logging.INFO
 
 
 def test_logging_config_with_filehandler(dummy_logger):
     logfile = MagicMock()
     log.config(logfile, delayed=True)
     assert len(dummy_logger.handlers) == 2
     assert dummy_logger.handlers[1].level == logging.DEBUG
```

### Comparing `nexgen-0.9.2/tests/test_utils.py` & `nexgen-0.9.3/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.2/tests/test_version.py` & `nexgen-0.9.3/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.2/tests/tools/test_VDS_tools.py` & `nexgen-0.9.3/tests/tools/test_VDS_tools.py`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.2/tests/tools/test_meta_tools.py` & `nexgen-0.9.3/tests/tools/test_meta_tools.py`

 * *Files identical despite different names*

### Comparing `nexgen-0.9.2/tests/tools/test_tools_for_ED.py` & `nexgen-0.9.3/tests/tools/test_tools_for_ED.py`

 * *Files identical despite different names*

