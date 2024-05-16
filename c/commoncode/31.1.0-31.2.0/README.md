# Comparing `tmp/commoncode-31.1.0.tar.gz` & `tmp/commoncode-31.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "commoncode-31.1.0.tar", last modified: Wed May 15 23:25:54 2024, max compression
+gzip compressed data, was "commoncode-31.2.0.tar", last modified: Thu May 16 18:35:30 2024, max compression
```

## Comparing `commoncode-31.1.0.tar` & `commoncode-31.2.0.tar`

### file list

```diff
@@ -1,471 +1,924 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.846425 commoncode-31.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-15 23:25:49.000000 commoncode-31.1.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.774424 commoncode-31.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.794425 commoncode-31.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-05-15 23:25:49.000000 commoncode-31.1.0/.github/workflows/docs-ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-05-15 23:25:49.000000 commoncode-31.1.0/.github/workflows/pypi-release.yml
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-15 23:25:49.000000 commoncode-31.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-15 23:25:49.000000 commoncode-31.1.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-15 23:25:49.000000 commoncode-31.1.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8900 2024-05-15 23:25:49.000000 commoncode-31.1.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3422 2024-05-15 23:25:49.000000 commoncode-31.1.0/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-15 23:25:49.000000 commoncode-31.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-05-15 23:25:49.000000 commoncode-31.1.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-15 23:25:49.000000 commoncode-31.1.0/NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-05-15 23:25:54.846425 commoncode-31.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      724 2024-05-15 23:25:49.000000 commoncode-31.1.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-15 23:25:49.000000 commoncode-31.1.0/apache-2.0.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4474 2024-05-15 23:25:49.000000 commoncode-31.1.0/azure-pipelines.yml
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-15 23:25:49.000000 commoncode-31.1.0/commoncode.ABOUT
--rwxr-xr-x   0 runner    (1001) docker     (127)     6328 2024-05-15 23:25:49.000000 commoncode-31.1.0/configure
--rw-r--r--   0 runner    (1001) docker     (127)     6948 2024-05-15 23:25:49.000000 commoncode-31.1.0/configure.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.794425 commoncode-31.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-15 23:25:49.000000 commoncode-31.1.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-15 23:25:49.000000 commoncode-31.1.0/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.794425 commoncode-31.1.0/docs/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-15 23:25:49.000000 commoncode-31.1.0/docs/scripts/doc8_style_check.sh
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-15 23:25:49.000000 commoncode-31.1.0/docs/scripts/sphinx_build_link_check.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.794425 commoncode-31.1.0/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.794425 commoncode-31.1.0/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     8022 2024-05-15 23:25:49.000000 commoncode-31.1.0/docs/source/_static/theme_overrides.css
--rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-05-15 23:25:49.000000 commoncode-31.1.0/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.794425 commoncode-31.1.0/docs/source/contribute/
--rw-r--r--   0 runner    (1001) docker     (127)    10245 2024-05-15 23:25:49.000000 commoncode-31.1.0/docs/source/contribute/contrib_doc.rst
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-15 23:25:49.000000 commoncode-31.1.0/docs/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.774424 commoncode-31.1.0/etc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.794425 commoncode-31.1.0/etc/ci/
--rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-05-15 23:25:49.000000 commoncode-31.1.0/etc/ci/azure-container-deb.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-05-15 23:25:49.000000 commoncode-31.1.0/etc/ci/azure-container-rpm.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-05-15 23:25:49.000000 commoncode-31.1.0/etc/ci/azure-posix.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-05-15 23:25:49.000000 commoncode-31.1.0/etc/ci/azure-win.yml
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-15 23:25:49.000000 commoncode-31.1.0/etc/ci/install_sudo.sh
--rw-r--r--   0 runner    (1001) docker     (127)     8365 2024-05-15 23:25:49.000000 commoncode-31.1.0/etc/ci/macports-ci
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-15 23:25:49.000000 commoncode-31.1.0/etc/ci/macports-ci.ABOUT
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-15 23:25:49.000000 commoncode-31.1.0/etc/ci/mit.LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.798425 commoncode-31.1.0/etc/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)     3744 2024-05-15 23:25:49.000000 commoncode-31.1.0/etc/scripts/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-15 23:25:49.000000 commoncode-31.1.0/etc/scripts/check_thirdparty.py
--rw-r--r--   0 runner    (1001) docker     (127)     9486 2024-05-15 23:25:49.000000 commoncode-31.1.0/etc/scripts/fetch_thirdparty.py
--rw-r--r--   0 runner    (1001) docker     (127)     9699 2024-05-15 23:25:49.000000 commoncode-31.1.0/etc/scripts/gen_pypi_simple.py
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-15 23:25:49.000000 commoncode-31.1.0/etc/scripts/gen_pypi_simple.py.ABOUT
--rw-r--r--   0 runner    (1001) docker     (127)     2776 2024-05-15 23:25:49.000000 commoncode-31.1.0/etc/scripts/gen_pypi_simple.py.NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-05-15 23:25:49.000000 commoncode-31.1.0/etc/scripts/gen_requirements.py
--rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-05-15 23:25:49.000000 commoncode-31.1.0/etc/scripts/gen_requirements_dev.py
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-15 23:25:49.000000 commoncode-31.1.0/etc/scripts/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4497 2024-05-15 23:25:49.000000 commoncode-31.1.0/etc/scripts/test_utils_pip_compatibility_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-15 23:25:49.000000 commoncode-31.1.0/etc/scripts/test_utils_pip_compatibility_tags.py.ABOUT
--rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-05-15 23:25:49.000000 commoncode-31.1.0/etc/scripts/test_utils_pypi_supported_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-15 23:25:49.000000 commoncode-31.1.0/etc/scripts/test_utils_pypi_supported_tags.py.ABOUT
--rw-r--r--   0 runner    (1001) docker     (127)     6418 2024-05-15 23:25:49.000000 commoncode-31.1.0/etc/scripts/utils_dejacode.py
--rw-r--r--   0 runner    (1001) docker     (127)     6704 2024-05-15 23:25:49.000000 commoncode-31.1.0/etc/scripts/utils_pip_compatibility_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-05-15 23:25:49.000000 commoncode-31.1.0/etc/scripts/utils_pip_compatibility_tags.py.ABOUT
--rw-r--r--   0 runner    (1001) docker     (127)     2850 2024-05-15 23:25:49.000000 commoncode-31.1.0/etc/scripts/utils_pypi_supported_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-15 23:25:49.000000 commoncode-31.1.0/etc/scripts/utils_pypi_supported_tags.py.ABOUT
--rw-r--r--   0 runner    (1001) docker     (127)     6152 2024-05-15 23:25:49.000000 commoncode-31.1.0/etc/scripts/utils_requirements.py
--rw-r--r--   0 runner    (1001) docker     (127)    75931 2024-05-15 23:25:49.000000 commoncode-31.1.0/etc/scripts/utils_thirdparty.py
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-15 23:25:49.000000 commoncode-31.1.0/etc/scripts/utils_thirdparty.py.ABOUT
--rw-r--r--   0 runner    (1001) docker     (127)      857 2024-05-15 23:25:49.000000 commoncode-31.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-15 23:25:49.000000 commoncode-31.1.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-15 23:25:49.000000 commoncode-31.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-05-15 23:25:54.850425 commoncode-31.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-15 23:25:49.000000 commoncode-31.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.774424 commoncode-31.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.802425 commoncode-31.1.0/src/commoncode/
--rw-r--r--   0 runner    (1001) docker     (127)      916 2024-05-15 23:25:49.000000 commoncode-31.1.0/src/commoncode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3999 2024-05-15 23:25:49.000000 commoncode-31.1.0/src/commoncode/archive.py
--rw-r--r--   0 runner    (1001) docker     (127)    19600 2024-05-15 23:25:49.000000 commoncode-31.1.0/src/commoncode/cliutils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-05-15 23:25:49.000000 commoncode-31.1.0/src/commoncode/codec.py
--rw-r--r--   0 runner    (1001) docker     (127)     9516 2024-05-15 23:25:49.000000 commoncode-31.1.0/src/commoncode/command.py
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-05-15 23:25:49.000000 commoncode-31.1.0/src/commoncode/compat.py
--rw-r--r--   0 runner    (1001) docker     (127)     5480 2024-05-15 23:25:49.000000 commoncode-31.1.0/src/commoncode/datautils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-15 23:25:49.000000 commoncode-31.1.0/src/commoncode/date.py
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-15 23:25:49.000000 commoncode-31.1.0/src/commoncode/dict_utils.ABOUT
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-05-15 23:25:49.000000 commoncode-31.1.0/src/commoncode/dict_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2148 2024-05-15 23:25:49.000000 commoncode-31.1.0/src/commoncode/fetch.py
--rw-r--r--   0 runner    (1001) docker     (127)     6487 2024-05-15 23:25:49.000000 commoncode-31.1.0/src/commoncode/fileset.py
--rw-r--r--   0 runner    (1001) docker     (127)     6660 2024-05-15 23:25:49.000000 commoncode-31.1.0/src/commoncode/filetype.py
--rw-r--r--   0 runner    (1001) docker     (127)    17123 2024-05-15 23:25:49.000000 commoncode-31.1.0/src/commoncode/fileutils.py
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-15 23:25:49.000000 commoncode-31.1.0/src/commoncode/fileutils.py.ABOUT
--rw-r--r--   0 runner    (1001) docker     (127)     3325 2024-05-15 23:25:49.000000 commoncode-31.1.0/src/commoncode/functional.py
--rw-r--r--   0 runner    (1001) docker     (127)     4967 2024-05-15 23:25:49.000000 commoncode-31.1.0/src/commoncode/hash.py
--rw-r--r--   0 runner    (1001) docker     (127)    11645 2024-05-15 23:25:49.000000 commoncode-31.1.0/src/commoncode/ignore.py
--rw-r--r--   0 runner    (1001) docker     (127)     9167 2024-05-15 23:25:49.000000 commoncode-31.1.0/src/commoncode/paths.py
--rw-r--r--   0 runner    (1001) docker     (127)    32426 2024-05-15 23:25:49.000000 commoncode-31.1.0/src/commoncode/python.LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    73970 2024-05-15 23:25:49.000000 commoncode-31.1.0/src/commoncode/resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     4736 2024-05-15 23:25:49.000000 commoncode-31.1.0/src/commoncode/system.py
--rw-r--r--   0 runner    (1001) docker     (127)    14225 2024-05-15 23:25:49.000000 commoncode-31.1.0/src/commoncode/testcase.py
--rw-r--r--   0 runner    (1001) docker     (127)     4163 2024-05-15 23:25:49.000000 commoncode-31.1.0/src/commoncode/text.py
--rw-r--r--   0 runner    (1001) docker     (127)     3692 2024-05-15 23:25:49.000000 commoncode-31.1.0/src/commoncode/timeutils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4551 2024-05-15 23:25:49.000000 commoncode-31.1.0/src/commoncode/urn.py
--rw-r--r--   0 runner    (1001) docker     (127)     9995 2024-05-15 23:25:49.000000 commoncode-31.1.0/src/commoncode/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.846425 commoncode-31.1.0/src/commoncode.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-05-15 23:25:54.000000 commoncode-31.1.0/src/commoncode.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14540 2024-05-15 23:25:54.000000 commoncode-31.1.0/src/commoncode.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 23:25:54.000000 commoncode-31.1.0/src/commoncode.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 23:25:54.000000 commoncode-31.1.0/src/commoncode.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-15 23:25:54.000000 commoncode-31.1.0/src/commoncode.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-15 23:25:54.000000 commoncode-31.1.0/src/commoncode.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.806425 commoncode-31.1.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.790424 commoncode-31.1.0/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.774424 commoncode-31.1.0/tests/data/count/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.774424 commoncode-31.1.0/tests/data/count/filecount/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.810425 commoncode-31.1.0/tests/data/count/filecount/dir/
--rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/count/filecount/dir/a.txt
--rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/count/filecount/dir/b.txt
--rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/count/filecount/dir/c.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.810425 commoncode-31.1.0/tests/data/count/filecount/dir/sub1/
--rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/count/filecount/dir/sub1/a.txt
--rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/count/filecount/dir/sub1/b.txt
--rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/count/filecount/dir/sub1/c.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.810425 commoncode-31.1.0/tests/data/count/filecount/dir/sub1/subsub/
--rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/count/filecount/dir/sub1/subsub/a.txt
--rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/count/filecount/dir/sub1/subsub/b.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.810425 commoncode-31.1.0/tests/data/count/filecount/dir/sub2/
--rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/count/filecount/dir/sub2/a.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.810425 commoncode-31.1.0/tests/data/date/
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/date/ant-jsch-1.7.0.tar.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.810425 commoncode-31.1.0/tests/data/date/dir/
--rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/date/dir/a.txt
--rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/date/dir/b.txt
--rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/date/dir/c.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.810425 commoncode-31.1.0/tests/data/date/dir/sub1/
--rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/date/dir/sub1/a.txt
--rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/date/dir/sub1/b.txt
--rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/date/dir/sub1/c.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.810425 commoncode-31.1.0/tests/data/date/dir/sub1/subsub/
--rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/date/dir/sub1/subsub/a.txt
--rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/date/dir/sub1/subsub/b.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.810425 commoncode-31.1.0/tests/data/date/dir/sub2/
--rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/date/dir/sub2/a.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.810425 commoncode-31.1.0/tests/data/fileset/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/fileset/scancodeignore.lst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.810425 commoncode-31.1.0/tests/data/filetype/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.778424 commoncode-31.1.0/tests/data/filetype/readwrite/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.810425 commoncode-31.1.0/tests/data/filetype/readwrite/sub/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/filetype/readwrite/sub/file
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.810425 commoncode-31.1.0/tests/data/filetype/size/
--rw-r--r--   0 runner    (1001) docker     (127)    12388 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/filetype/size/Image1.eps
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.810425 commoncode-31.1.0/tests/data/filetype/size/exec/
--rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/filetype/size/exec/1.txt
--rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/filetype/size/exec/a.bat
--rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/filetype/size/exec/a.tar
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.814425 commoncode-31.1.0/tests/data/filetype/size/exec/subtxt/
--rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/filetype/size/exec/subtxt/1.txt
--rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/filetype/size/exec/subtxt/a.txt
--rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/filetype/size/exec/subtxt/b.txt
--rw-r--r--   0 runner    (1001) docker     (127)   109056 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/filetype/types.tar
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.778424 commoncode-31.1.0/tests/data/fileutils/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.814425 commoncode-31.1.0/tests/data/fileutils/basename/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.814425 commoncode-31.1.0/tests/data/fileutils/basename/a/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.814425 commoncode-31.1.0/tests/data/fileutils/basename/a/.a/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/fileutils/basename/a/.a/file
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.814425 commoncode-31.1.0/tests/data/fileutils/basename/a/b/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/fileutils/basename/a/b/.a
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/fileutils/basename/a/b/.a.b
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/fileutils/basename/a/b/a.tag.gz
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/fileutils/basename/a/f.a
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.814425 commoncode-31.1.0/tests/data/fileutils/basename/f.a/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/fileutils/basename/f.a/a.c
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/fileutils/basename/tst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.814425 commoncode-31.1.0/tests/data/fileutils/exec/
--rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/fileutils/exec/1.txt
--rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/fileutils/exec/a.bat
--rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/fileutils/exec/a.tar
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.814425 commoncode-31.1.0/tests/data/fileutils/exec/subtxt/
--rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/fileutils/exec/subtxt/1.txt
--rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/fileutils/exec/subtxt/a.txt
--rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/fileutils/exec/subtxt/b.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.778424 commoncode-31.1.0/tests/data/fileutils/executable/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.778424 commoncode-31.1.0/tests/data/fileutils/executable/deep1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.814425 commoncode-31.1.0/tests/data/fileutils/executable/deep1/deep2/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/fileutils/executable/deep1/deep2/ctags
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.814425 commoncode-31.1.0/tests/data/fileutils/filetype/
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/fileutils/filetype/a.html
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/fileutils/filetype/stage1
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.814425 commoncode-31.1.0/tests/data/fileutils/perms/
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/fileutils/perms/unreadable.tgz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.778424 commoncode-31.1.0/tests/data/fileutils/readwrite/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.814425 commoncode-31.1.0/tests/data/fileutils/readwrite/sub/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/fileutils/readwrite/sub/file
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.814425 commoncode-31.1.0/tests/data/fileutils/walk/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.814425 commoncode-31.1.0/tests/data/fileutils/walk/d1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.814425 commoncode-31.1.0/tests/data/fileutils/walk/d1/d2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.814425 commoncode-31.1.0/tests/data/fileutils/walk/d1/d2/d3/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/fileutils/walk/d1/d2/d3/f3
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/fileutils/walk/d1/d2/f2
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/fileutils/walk/d1/f1
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/fileutils/walk/f
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/fileutils/walk/unicode.zip
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.814425 commoncode-31.1.0/tests/data/fileutils/walk_non_utf8/
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/fileutils/walk_non_utf8/non_unicode.tgz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.782425 commoncode-31.1.0/tests/data/hash/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.818425 commoncode-31.1.0/tests/data/hash/dir1/
--rw-r--r--   0 runner    (1001) docker     (127)     7859 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/hash/dir1/a.png
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/hash/dir1/a.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.818425 commoncode-31.1.0/tests/data/hash/dir2/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/hash/dir2/a.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/hash/dir2/dos.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.818425 commoncode-31.1.0/tests/data/hash/sha1-collision/
--rw-r--r--   0 runner    (1001) docker     (127)   422435 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/hash/sha1-collision/shattered-1.pdf
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/hash/sha1-collision/shattered-1.pdf.ABOUT
--rw-r--r--   0 runner    (1001) docker     (127)   422435 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/hash/sha1-collision/shattered-2.pdf
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/hash/sha1-collision/shattered-2.pdf.ABOUT
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.818425 commoncode-31.1.0/tests/data/ignore/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/ignore/.scancodeignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.818425 commoncode-31.1.0/tests/data/ignore/excludes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/ignore/excludes/.localized
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/ignore/excludes/eclipse.tgz
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/ignore/excludes/mac.tgz
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/ignore/excludes/msft-vs.tgz
--rw-r--r--   0 runner    (1001) docker     (127)     6296 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/ignore/vcs.tgz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.790424 commoncode-31.1.0/tests/data/resource/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.782425 commoncode-31.1.0/tests/data/resource/cache/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.818425 commoncode-31.1.0/tests/data/resource/cache/package/
--rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/cache/package/package.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.818425 commoncode-31.1.0/tests/data/resource/cache2/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/cache2/abc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.818425 commoncode-31.1.0/tests/data/resource/cache2/dir/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/cache2/dir/that
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/cache2/dir/this
--rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/cache2/et131x.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.818425 commoncode-31.1.0/tests/data/resource/cache2/other dir/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/cache2/other dir/file
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.782425 commoncode-31.1.0/tests/data/resource/client/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.822425 commoncode-31.1.0/tests/data/resource/client/Images/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/client/Images/applicationCache.png
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/client/Images/spinner.gif
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.822425 commoncode-31.1.0/tests/data/resource/codebase/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/codebase/abc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.822425 commoncode-31.1.0/tests/data/resource/codebase/dir/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/codebase/dir/that
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/codebase/dir/this
--rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/codebase/et131x.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.822425 commoncode-31.1.0/tests/data/resource/codebase/other dir/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/codebase/other dir/file
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.822425 commoncode-31.1.0/tests/data/resource/deeply_nested/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.822425 commoncode-31.1.0/tests/data/resource/deeply_nested/level1_dir1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.822425 commoncode-31.1.0/tests/data/resource/deeply_nested/level1_dir1/level2_dir1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.822425 commoncode-31.1.0/tests/data/resource/deeply_nested/level1_dir1/level2_dir1/level3_dir1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/deeply_nested/level1_dir1/level2_dir1/level3_dir1/level4_file1
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/deeply_nested/level1_dir1/level2_dir1/level3_file1
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/deeply_nested/level1_dir1/level2_dir1/level3_file2
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/deeply_nested/level1_dir1/level2_file1
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/deeply_nested/level1_dir1/level2_file2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.822425 commoncode-31.1.0/tests/data/resource/deeply_nested/level1_dir2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.822425 commoncode-31.1.0/tests/data/resource/deeply_nested/level1_dir2/level2_dir3/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/deeply_nested/level1_dir2/level2_dir3/level3_file3
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/deeply_nested/level1_dir2/level2_dir3/level3_file4
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/deeply_nested/level1_dir2/level2_file3
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/deeply_nested/level1_dir2/level2_file4
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/deeply_nested/level1_dir2/level2_file5
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/deeply_nested/level1_file1
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/deeply_nested/level1_file2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.782425 commoncode-31.1.0/tests/data/resource/dist/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.822425 commoncode-31.1.0/tests/data/resource/dist/JGroups/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/dist/JGroups/EULA
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/dist/JGroups/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.822425 commoncode-31.1.0/tests/data/resource/dist/JGroups/src/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/dist/JGroups/src/RouterStub.java
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/dist/JGroups/src/RouterStubManager.java
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/dist/JGroups/src/S3_PING.java
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.782425 commoncode-31.1.0/tests/data/resource/dist/simple/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.822425 commoncode-31.1.0/tests/data/resource/dist/simple/META-INF/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/dist/simple/META-INF/MANIFEST.MF
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.822425 commoncode-31.1.0/tests/data/resource/ignore/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.822425 commoncode-31.1.0/tests/data/resource/ignore/cvs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/ignore/cvs/file2
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/ignore/file1
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.782425 commoncode-31.1.0/tests/data/resource/lcp/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.822425 commoncode-31.1.0/tests/data/resource/lcp/test1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.826425 commoncode-31.1.0/tests/data/resource/lcp/test1/JGroups/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/lcp/test1/JGroups/EULA
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/lcp/test1/JGroups/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.826425 commoncode-31.1.0/tests/data/resource/lcp/test1/JGroups/licenses/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/lcp/test1/JGroups/licenses/apache-1.1.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/lcp/test1/JGroups/licenses/lgpl.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.826425 commoncode-31.1.0/tests/data/resource/lcp/test1/JGroups/src/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/lcp/test1/JGroups/src/RouterStub.java
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/lcp/test1/JGroups/src/RouterStubManager.java
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/lcp/test1/JGroups/src/S3_PING.java
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/lcp/test1/screenshot.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.786424 commoncode-31.1.0/tests/data/resource/lcp/test1/simple/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.826425 commoncode-31.1.0/tests/data/resource/lcp/test1/simple/META-INF/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/lcp/test1/simple/META-INF/MANIFEST.MF
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.786424 commoncode-31.1.0/tests/data/resource/lcp/test1/simple/org/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.786424 commoncode-31.1.0/tests/data/resource/lcp/test1/simple/org/jvnet/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.786424 commoncode-31.1.0/tests/data/resource/lcp/test1/simple/org/jvnet/glassfish/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.786424 commoncode-31.1.0/tests/data/resource/lcp/test1/simple/org/jvnet/glassfish/comms/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.826425 commoncode-31.1.0/tests/data/resource/lcp/test1/simple/org/jvnet/glassfish/comms/sipagent/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.826425 commoncode-31.1.0/tests/data/resource/lcp/test1/simple/org/jvnet/glassfish/comms/sipagent/actions/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/lcp/test1/simple/org/jvnet/glassfish/comms/sipagent/actions/Bundle.properties
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/lcp/test1/simple/org/jvnet/glassfish/comms/sipagent/actions/SipAgentCookieAction.class
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/lcp/test1/simple/org/jvnet/glassfish/comms/sipagent/actions/bd.png
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/lcp/test1/simple/org/jvnet/glassfish/comms/sipagent/actions/bd24.png
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/lcp/test1/simple/org/jvnet/glassfish/comms/sipagent/org-jvnet-glassfish-comms-sipagent-actions-SipAgentCookieAction.instance
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/lcp/test1/simple/org/jvnet/glassfish/comms/sipagent/org-jvnet-glassfish-comms-sipagent-actions-SipAgentCookieAction_1.instance
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.786424 commoncode-31.1.0/tests/data/resource/lcp/test1/zlib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.826425 commoncode-31.1.0/tests/data/resource/lcp/test1/zlib/ada/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/lcp/test1/zlib/ada/zlib.ads
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.786424 commoncode-31.1.0/tests/data/resource/lcp/test1/zlib/inter/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.826425 commoncode-31.1.0/tests/data/resource/lcp/test1/zlib/inter/arch/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/lcp/test1/zlib/inter/arch/zlib.tar.gz
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.826425 commoncode-31.1.0/tests/data/resource/lcp/test1/zlib/inter/dir/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/lcp/test1/zlib/inter/dir/EULA
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/lcp/test1/zlib/inter/dir/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.826425 commoncode-31.1.0/tests/data/resource/lcp/test1/zlib/inter/dir/licenses/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/lcp/test1/zlib/inter/dir/licenses/apache-1.1.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/lcp/test1/zlib/inter/dir/licenses/apache-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/lcp/test1/zlib/inter/dir/licenses/bouncycastle.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/lcp/test1/zlib/inter/dir/licenses/cpl-1.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/lcp/test1/zlib/inter/dir/licenses/lgpl.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.830425 commoncode-31.1.0/tests/data/resource/lcp/test1/zlib/inter/dir/src/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/lcp/test1/zlib/inter/dir/src/FixedMembershipToken.java
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/lcp/test1/zlib/inter/dir/src/GuardedBy.java
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/lcp/test1/zlib/inter/dir/src/ImmutableReference.java
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/lcp/test1/zlib/inter/dir/src/RATE_LIMITER.java
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/lcp/test1/zlib/inter/dir/src/RouterStub.java
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/lcp/test1/zlib/inter/dir/src/RouterStubManager.java
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/lcp/test1/zlib/inter/dir/src/S3_PING.java
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.830425 commoncode-31.1.0/tests/data/resource/lcp/test1/zlib/inter/iostream2/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/lcp/test1/zlib/inter/iostream2/zstream.h
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/lcp/test1/zlib/inter/iostream2/zstream_test.cpp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.830425 commoncode-31.1.0/tests/data/resource/lcp/test1/zlib/inter/zlib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.830425 commoncode-31.1.0/tests/data/resource/lcp/test1/zlib/inter/zlib/ada/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/lcp/test1/zlib/inter/zlib/ada/zlib.ads
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/lcp/test1/zlib/inter/zlib/adler32.c
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/lcp/test1/zlib/inter/zlib/deflate.c
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/lcp/test1/zlib/inter/zlib/deflate.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.830425 commoncode-31.1.0/tests/data/resource/lcp/test1/zlib/inter/zlib/dotzlib/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/lcp/test1/zlib/inter/zlib/dotzlib/AssemblyInfo.cs
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/lcp/test1/zlib/inter/zlib/dotzlib/ChecksumImpl.cs
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/lcp/test1/zlib/inter/zlib/dotzlib/LICENSE_1_0.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/lcp/test1/zlib/inter/zlib/dotzlib/readme.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.830425 commoncode-31.1.0/tests/data/resource/lcp/test1/zlib/inter/zlib/gcc_gvmat64/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/lcp/test1/zlib/inter/zlib/gcc_gvmat64/gvmat64.S
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.830425 commoncode-31.1.0/tests/data/resource/lcp/test1/zlib/inter/zlib/infback9/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/lcp/test1/zlib/inter/zlib/infback9/infback9.c
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/lcp/test1/zlib/inter/zlib/infback9/infback9.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.830425 commoncode-31.1.0/tests/data/resource/lcp/test1/zlib/inter/zlib/iostream2/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/lcp/test1/zlib/inter/zlib/iostream2/zstream.h
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/lcp/test1/zlib/inter/zlib/iostream2/zstream_test.cpp
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/lcp/test1/zlib/inter/zlib/zlib.h
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/lcp/test1/zlib/inter/zlib/zutil.c
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/lcp/test1/zlib/inter/zlib/zutil.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.830425 commoncode-31.1.0/tests/data/resource/resource/
--rw-r--r--   0 runner    (1001) docker     (127)     7194 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/resource/test-extracted-from-to.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.830425 commoncode-31.1.0/tests/data/resource/samples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.834425 commoncode-31.1.0/tests/data/resource/samples/JGroups/
--rw-r--r--   0 runner    (1001) docker     (127)     8156 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/samples/JGroups/EULA
--rw-r--r--   0 runner    (1001) docker     (127)    26430 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/samples/JGroups/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.834425 commoncode-31.1.0/tests/data/resource/samples/JGroups/licenses/
--rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/samples/JGroups/licenses/apache-1.1.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11560 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/samples/JGroups/licenses/apache-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/samples/JGroups/licenses/bouncycastle.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11987 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/samples/JGroups/licenses/cpl-1.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)    26934 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/samples/JGroups/licenses/lgpl.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.834425 commoncode-31.1.0/tests/data/resource/samples/JGroups/src/
--rw-r--r--   0 runner    (1001) docker     (127)     5144 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/samples/JGroups/src/FixedMembershipToken.java
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/samples/JGroups/src/GuardedBy.java
--rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/samples/JGroups/src/ImmutableReference.java
--rw-r--r--   0 runner    (1001) docker     (127)     3692 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/samples/JGroups/src/RATE_LIMITER.java
--rw-r--r--   0 runner    (1001) docker     (127)     9913 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/samples/JGroups/src/RouterStub.java
--rw-r--r--   0 runner    (1001) docker     (127)     8162 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/samples/JGroups/src/RouterStubManager.java
--rw-r--r--   0 runner    (1001) docker     (127)   122528 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/samples/JGroups/src/S3_PING.java
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/samples/README
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.834425 commoncode-31.1.0/tests/data/resource/samples/arch/
--rw-r--r--   0 runner    (1001) docker     (127)    28103 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/samples/arch/zlib.tar.gz
--rw-r--r--   0 runner    (1001) docker     (127)   622754 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/samples/screenshot.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.838425 commoncode-31.1.0/tests/data/resource/samples/zlib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.838425 commoncode-31.1.0/tests/data/resource/samples/zlib/ada/
--rw-r--r--   0 runner    (1001) docker     (127)    13594 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/samples/zlib/ada/zlib.ads
--rw-r--r--   0 runner    (1001) docker     (127)     4968 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/samples/zlib/adler32.c
--rw-r--r--   0 runner    (1001) docker     (127)    71476 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/samples/zlib/deflate.c
--rw-r--r--   0 runner    (1001) docker     (127)    12774 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/samples/zlib/deflate.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.838425 commoncode-31.1.0/tests/data/resource/samples/zlib/dotzlib/
--rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/samples/zlib/dotzlib/AssemblyInfo.cs
--rw-r--r--   0 runner    (1001) docker     (127)     8040 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/samples/zlib/dotzlib/ChecksumImpl.cs
--rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/samples/zlib/dotzlib/LICENSE_1_0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/samples/zlib/dotzlib/readme.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.838425 commoncode-31.1.0/tests/data/resource/samples/zlib/gcc_gvmat64/
--rw-r--r--   0 runner    (1001) docker     (127)    16413 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/samples/zlib/gcc_gvmat64/gvmat64.S
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.838425 commoncode-31.1.0/tests/data/resource/samples/zlib/infback9/
--rw-r--r--   0 runner    (1001) docker     (127)    21629 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/samples/zlib/infback9/infback9.c
--rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/samples/zlib/infback9/infback9.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.838425 commoncode-31.1.0/tests/data/resource/samples/zlib/iostream2/
--rw-r--r--   0 runner    (1001) docker     (127)     9283 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/samples/zlib/iostream2/zstream.h
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/samples/zlib/iostream2/zstream_test.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    87883 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/samples/zlib/zlib.h
--rw-r--r--   0 runner    (1001) docker     (127)     7414 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/samples/zlib/zutil.c
--rw-r--r--   0 runner    (1001) docker     (127)     6766 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/samples/zlib/zutil.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.838425 commoncode-31.1.0/tests/data/resource/skip_directories_during_walk/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.838425 commoncode-31.1.0/tests/data/resource/skip_directories_during_walk/skip-this-directory/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/skip_directories_during_walk/skip-this-directory/this-should-not-be-returned
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/skip_directories_during_walk/this-should-be-returned
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.842425 commoncode-31.1.0/tests/data/resource/virtual_codebase/
--rw-r--r--   0 runner    (1001) docker     (127)     4628 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/virtual_codebase/codebase-for-cache-tests.json
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/virtual_codebase/combine-1.json
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/virtual_codebase/combine-2.json
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/virtual_codebase/combine-expected.json
--rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/virtual_codebase/combine-shared-directory-name-1.json
--rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/virtual_codebase/combine-shared-directory-name-2.json
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/virtual_codebase/combine-shared-directory-name-expected.json
--rw-r--r--   0 runner    (1001) docker     (127)     5129 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/virtual_codebase/docker-hello-world.json
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/virtual_codebase/et131x.h.json
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/virtual_codebase/fingerprint_attribute.json
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/virtual_codebase/from_file.json
--rw-r--r--   0 runner    (1001) docker     (127)    17547 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/virtual_codebase/full-root-info-many-expected.json
--rw-r--r--   0 runner    (1001) docker     (127)    16812 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/virtual_codebase/full-root-info-many.json
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/virtual_codebase/full-root-info-one-expected.json
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/virtual_codebase/full-root-info-one.json
--rw-r--r--   0 runner    (1001) docker     (127)    50927 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/virtual_codebase/lcp.json
--rw-r--r--   0 runner    (1001) docker     (127)     5671 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/virtual_codebase/license-scan.json
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/virtual_codebase/node-16-slim.json
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/virtual_codebase/noinfo.json
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/virtual_codebase/only-path.json
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/virtual_codebase/resource.json
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/virtual_codebase/root-is-not-first-resource.json
--rw-r--r--   0 runner    (1001) docker     (127)     8187 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/virtual_codebase/samples-only-findings-expected.json
--rw-r--r--   0 runner    (1001) docker     (127)     4410 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/virtual_codebase/samples-only-findings.json
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/virtual_codebase/stripped-and-skipped-root.json
--rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/virtual_codebase/virtual_codebase.json
--rw-r--r--   0 runner    (1001) docker     (127)     6690 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/virtual_codebase/zephyr-binary.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.842425 commoncode-31.1.0/tests/data/resource/with_path/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.842425 commoncode-31.1.0/tests/data/resource/with_path/codebase/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/with_path/codebase/abc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.842425 commoncode-31.1.0/tests/data/resource/with_path/codebase/dir/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/with_path/codebase/dir/that
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/with_path/codebase/dir/this
--rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/with_path/codebase/et131x.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.842425 commoncode-31.1.0/tests/data/resource/with_path/codebase/other dir/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/with_path/codebase/other dir/file
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/with_path/codebase-expected.json
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/with_path/virtual-codebase-expected.json
--rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/with_path/virtual-codebase.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.846425 commoncode-31.1.0/tests/data/saneyaml/
--rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/saneyaml/metadata1
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/saneyaml/metadata1.notag
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.846425 commoncode-31.1.0/tests/data/symlink/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/symlink/test
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.846425 commoncode-31.1.0/tests/data/symlink/walk/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/symlink/walk/a
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.846425 commoncode-31.1.0/tests/data/symlink/walk/dir/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/symlink/walk/dir/b
--rw-r--r--   0 runner    (1001) docker     (127)     5114 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/test_cliutils.py
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/test_cliutils_progressbar.py
--rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/test_codec.py
--rw-r--r--   0 runner    (1001) docker     (127)     5946 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/test_command.py
--rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/test_date.py
--rw-r--r--   0 runner    (1001) docker     (127)     4130 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/test_fileset.py
--rw-r--r--   0 runner    (1001) docker     (127)     7749 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/test_filetype.py
--rw-r--r--   0 runner    (1001) docker     (127)    39362 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/test_fileutils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/test_functional.py
--rw-r--r--   0 runner    (1001) docker     (127)     7107 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/test_hash.py
--rw-r--r--   0 runner    (1001) docker     (127)     8215 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/test_ignore.py
--rw-r--r--   0 runner    (1001) docker     (127)    12779 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/test_paths.py
--rw-r--r--   0 runner    (1001) docker     (127)    63974 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/test_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/test_saneyaml.py
--rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/test_skeleton_codestyle.py
--rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/test_text.py
--rw-r--r--   0 runner    (1001) docker     (127)     3671 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/test_timeutils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5784 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/test_urn.py
--rw-r--r--   0 runner    (1001) docker     (127)     8797 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.597894 commoncode-31.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-16 18:35:26.000000 commoncode-31.2.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.473893 commoncode-31.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.493893 commoncode-31.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-05-16 18:35:26.000000 commoncode-31.2.0/.github/workflows/docs-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-05-16 18:35:26.000000 commoncode-31.2.0/.github/workflows/pypi-release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-16 18:35:26.000000 commoncode-31.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-16 18:35:26.000000 commoncode-31.2.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-16 18:35:26.000000 commoncode-31.2.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9049 2024-05-16 18:35:26.000000 commoncode-31.2.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3422 2024-05-16 18:35:26.000000 commoncode-31.2.0/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-16 18:35:26.000000 commoncode-31.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-05-16 18:35:26.000000 commoncode-31.2.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-16 18:35:26.000000 commoncode-31.2.0/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-05-16 18:35:30.597894 commoncode-31.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-05-16 18:35:26.000000 commoncode-31.2.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-16 18:35:26.000000 commoncode-31.2.0/apache-2.0.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4474 2024-05-16 18:35:26.000000 commoncode-31.2.0/azure-pipelines.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-16 18:35:26.000000 commoncode-31.2.0/commoncode.ABOUT
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6328 2024-05-16 18:35:26.000000 commoncode-31.2.0/configure
+-rw-r--r--   0 runner    (1001) docker     (127)     6948 2024-05-16 18:35:26.000000 commoncode-31.2.0/configure.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.497893 commoncode-31.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-16 18:35:26.000000 commoncode-31.2.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-16 18:35:26.000000 commoncode-31.2.0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.497893 commoncode-31.2.0/docs/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-16 18:35:26.000000 commoncode-31.2.0/docs/scripts/doc8_style_check.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-16 18:35:26.000000 commoncode-31.2.0/docs/scripts/sphinx_build_link_check.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.497893 commoncode-31.2.0/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.497893 commoncode-31.2.0/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     8022 2024-05-16 18:35:26.000000 commoncode-31.2.0/docs/source/_static/theme_overrides.css
+-rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-05-16 18:35:26.000000 commoncode-31.2.0/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.497893 commoncode-31.2.0/docs/source/contribute/
+-rw-r--r--   0 runner    (1001) docker     (127)    10245 2024-05-16 18:35:26.000000 commoncode-31.2.0/docs/source/contribute/contrib_doc.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-16 18:35:26.000000 commoncode-31.2.0/docs/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.473893 commoncode-31.2.0/etc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.497893 commoncode-31.2.0/etc/ci/
+-rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-05-16 18:35:26.000000 commoncode-31.2.0/etc/ci/azure-container-deb.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-05-16 18:35:26.000000 commoncode-31.2.0/etc/ci/azure-container-rpm.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-05-16 18:35:26.000000 commoncode-31.2.0/etc/ci/azure-posix.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-05-16 18:35:26.000000 commoncode-31.2.0/etc/ci/azure-win.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-16 18:35:26.000000 commoncode-31.2.0/etc/ci/install_sudo.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     8365 2024-05-16 18:35:26.000000 commoncode-31.2.0/etc/ci/macports-ci
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-16 18:35:26.000000 commoncode-31.2.0/etc/ci/macports-ci.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-16 18:35:26.000000 commoncode-31.2.0/etc/ci/mit.LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.501893 commoncode-31.2.0/etc/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3744 2024-05-16 18:35:26.000000 commoncode-31.2.0/etc/scripts/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-16 18:35:26.000000 commoncode-31.2.0/etc/scripts/check_thirdparty.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9486 2024-05-16 18:35:26.000000 commoncode-31.2.0/etc/scripts/fetch_thirdparty.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9699 2024-05-16 18:35:26.000000 commoncode-31.2.0/etc/scripts/gen_pypi_simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-16 18:35:26.000000 commoncode-31.2.0/etc/scripts/gen_pypi_simple.py.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (127)     2776 2024-05-16 18:35:26.000000 commoncode-31.2.0/etc/scripts/gen_pypi_simple.py.NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-05-16 18:35:26.000000 commoncode-31.2.0/etc/scripts/gen_requirements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-05-16 18:35:26.000000 commoncode-31.2.0/etc/scripts/gen_requirements_dev.py
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-16 18:35:26.000000 commoncode-31.2.0/etc/scripts/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4497 2024-05-16 18:35:26.000000 commoncode-31.2.0/etc/scripts/test_utils_pip_compatibility_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-16 18:35:26.000000 commoncode-31.2.0/etc/scripts/test_utils_pip_compatibility_tags.py.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-05-16 18:35:26.000000 commoncode-31.2.0/etc/scripts/test_utils_pypi_supported_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-16 18:35:26.000000 commoncode-31.2.0/etc/scripts/test_utils_pypi_supported_tags.py.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (127)     6418 2024-05-16 18:35:26.000000 commoncode-31.2.0/etc/scripts/utils_dejacode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6704 2024-05-16 18:35:26.000000 commoncode-31.2.0/etc/scripts/utils_pip_compatibility_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-05-16 18:35:26.000000 commoncode-31.2.0/etc/scripts/utils_pip_compatibility_tags.py.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (127)     2850 2024-05-16 18:35:26.000000 commoncode-31.2.0/etc/scripts/utils_pypi_supported_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-16 18:35:26.000000 commoncode-31.2.0/etc/scripts/utils_pypi_supported_tags.py.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (127)     6152 2024-05-16 18:35:26.000000 commoncode-31.2.0/etc/scripts/utils_requirements.py
+-rw-r--r--   0 runner    (1001) docker     (127)    75931 2024-05-16 18:35:26.000000 commoncode-31.2.0/etc/scripts/utils_thirdparty.py
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-16 18:35:26.000000 commoncode-31.2.0/etc/scripts/utils_thirdparty.py.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-05-16 18:35:26.000000 commoncode-31.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-16 18:35:26.000000 commoncode-31.2.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-16 18:35:26.000000 commoncode-31.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-05-16 18:35:30.597894 commoncode-31.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-16 18:35:26.000000 commoncode-31.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.473893 commoncode-31.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.505893 commoncode-31.2.0/src/commoncode/
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-05-16 18:35:26.000000 commoncode-31.2.0/src/commoncode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3999 2024-05-16 18:35:26.000000 commoncode-31.2.0/src/commoncode/archive.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19600 2024-05-16 18:35:26.000000 commoncode-31.2.0/src/commoncode/cliutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-05-16 18:35:26.000000 commoncode-31.2.0/src/commoncode/codec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9516 2024-05-16 18:35:26.000000 commoncode-31.2.0/src/commoncode/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-05-16 18:35:26.000000 commoncode-31.2.0/src/commoncode/compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5480 2024-05-16 18:35:26.000000 commoncode-31.2.0/src/commoncode/datautils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-16 18:35:26.000000 commoncode-31.2.0/src/commoncode/date.py
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-16 18:35:26.000000 commoncode-31.2.0/src/commoncode/dict_utils.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-05-16 18:35:26.000000 commoncode-31.2.0/src/commoncode/dict_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-05-16 18:35:26.000000 commoncode-31.2.0/src/commoncode/distro.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2148 2024-05-16 18:35:26.000000 commoncode-31.2.0/src/commoncode/fetch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6487 2024-05-16 18:35:26.000000 commoncode-31.2.0/src/commoncode/fileset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6660 2024-05-16 18:35:26.000000 commoncode-31.2.0/src/commoncode/filetype.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17123 2024-05-16 18:35:26.000000 commoncode-31.2.0/src/commoncode/fileutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-16 18:35:26.000000 commoncode-31.2.0/src/commoncode/fileutils.py.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (127)     3325 2024-05-16 18:35:26.000000 commoncode-31.2.0/src/commoncode/functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4967 2024-05-16 18:35:26.000000 commoncode-31.2.0/src/commoncode/hash.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11645 2024-05-16 18:35:26.000000 commoncode-31.2.0/src/commoncode/ignore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9167 2024-05-16 18:35:26.000000 commoncode-31.2.0/src/commoncode/paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32426 2024-05-16 18:35:26.000000 commoncode-31.2.0/src/commoncode/python.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    73970 2024-05-16 18:35:26.000000 commoncode-31.2.0/src/commoncode/resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4736 2024-05-16 18:35:26.000000 commoncode-31.2.0/src/commoncode/system.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14225 2024-05-16 18:35:26.000000 commoncode-31.2.0/src/commoncode/testcase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4163 2024-05-16 18:35:26.000000 commoncode-31.2.0/src/commoncode/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3692 2024-05-16 18:35:26.000000 commoncode-31.2.0/src/commoncode/timeutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4551 2024-05-16 18:35:26.000000 commoncode-31.2.0/src/commoncode/urn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9995 2024-05-16 18:35:26.000000 commoncode-31.2.0/src/commoncode/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.593894 commoncode-31.2.0/src/commoncode.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-05-16 18:35:30.000000 commoncode-31.2.0/src/commoncode.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    38667 2024-05-16 18:35:30.000000 commoncode-31.2.0/src/commoncode.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 18:35:30.000000 commoncode-31.2.0/src/commoncode.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 18:35:30.000000 commoncode-31.2.0/src/commoncode.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-16 18:35:30.000000 commoncode-31.2.0/src/commoncode.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-16 18:35:30.000000 commoncode-31.2.0/src/commoncode.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.509893 commoncode-31.2.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.493893 commoncode-31.2.0/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.473893 commoncode-31.2.0/tests/data/count/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.473893 commoncode-31.2.0/tests/data/count/filecount/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.509893 commoncode-31.2.0/tests/data/count/filecount/dir/
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/count/filecount/dir/a.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/count/filecount/dir/b.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/count/filecount/dir/c.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.509893 commoncode-31.2.0/tests/data/count/filecount/dir/sub1/
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/count/filecount/dir/sub1/a.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/count/filecount/dir/sub1/b.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/count/filecount/dir/sub1/c.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.509893 commoncode-31.2.0/tests/data/count/filecount/dir/sub1/subsub/
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/count/filecount/dir/sub1/subsub/a.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/count/filecount/dir/sub1/subsub/b.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.509893 commoncode-31.2.0/tests/data/count/filecount/dir/sub2/
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/count/filecount/dir/sub2/a.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.509893 commoncode-31.2.0/tests/data/date/
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/date/ant-jsch-1.7.0.tar.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.509893 commoncode-31.2.0/tests/data/date/dir/
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/date/dir/a.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/date/dir/b.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/date/dir/c.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.509893 commoncode-31.2.0/tests/data/date/dir/sub1/
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/date/dir/sub1/a.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/date/dir/sub1/b.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/date/dir/sub1/c.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.509893 commoncode-31.2.0/tests/data/date/dir/sub1/subsub/
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/date/dir/sub1/subsub/a.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/date/dir/sub1/subsub/b.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.509893 commoncode-31.2.0/tests/data/date/dir/sub2/
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/date/dir/sub2/a.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.513893 commoncode-31.2.0/tests/data/distro/
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/README-chef.md
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/README-nate.md
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/README-zoo.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/apache-2.0.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7048 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/cc0-1.0.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/mit.LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.481893 commoncode-31.2.0/tests/data/distro/os-release/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.513893 commoncode-31.2.0/tests/data/distro/os-release/alpine/
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/alpine/alpine-3.8.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/alpine/alpine-3.8.txt-expected.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.513893 commoncode-31.2.0/tests/data/distro/os-release/amazon/
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/amazon/amazon-2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/amazon/amazon-2.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/amazon/amazon-2018.03.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/amazon/amazon-2018.03.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/amazon/amzon-2016.09.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/amazon/amzon-2016.09.txt-expected.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.513893 commoncode-31.2.0/tests/data/distro/os-release/antergos/
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/antergos/antergos.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/antergos/antergos.txt-expected.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.513893 commoncode-31.2.0/tests/data/distro/os-release/arch/
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/arch/arch-arm-new.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/arch/arch-arm-new.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/arch/arch-arm.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/arch/arch-arm.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/arch/arch-mini.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/arch/arch-mini.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/arch/arch.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/arch/arch.txt-expected.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.513893 commoncode-31.2.0/tests/data/distro/os-release/artix/
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/artix/artix.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/artix/artix.txt-expected.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.513893 commoncode-31.2.0/tests/data/distro/os-release/centos/
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/centos/centos-7.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/centos/centos-7.txt-expected.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.513893 commoncode-31.2.0/tests/data/distro/os-release/clearlinux/
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/clearlinux/clearlinux-1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/clearlinux/clearlinux-1.txt-expected.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.513893 commoncode-31.2.0/tests/data/distro/os-release/clearos/
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/clearos/clearos-7.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/clearos/clearos-7.txt-expected.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.517893 commoncode-31.2.0/tests/data/distro/os-release/coreos/
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/coreos/coreos-1185.3.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/coreos/coreos-1185.3.0.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/coreos/coreos-1235.6.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/coreos/coreos-1235.6.0.txt-expected.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.517893 commoncode-31.2.0/tests/data/distro/os-release/cumulus/
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/cumulus/cumulus-3.7.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/cumulus/cumulus-3.7.txt-expected.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.517893 commoncode-31.2.0/tests/data/distro/os-release/debian/
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/debian/debian-10.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/debian/debian-10.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/debian/debian-11.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/debian/debian-11.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/debian/debian-7.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/debian/debian-8.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/debian/debian-9.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/debian/debian-sid.txt-expected.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.517893 commoncode-31.2.0/tests/data/distro/os-release/distroless/
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/distroless/distroless-debian10.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/distroless/distroless-debian10.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/distroless/distroless-debian11.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/distroless/distroless-debian11.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/distroless/distroless-debian9.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/distroless/distroless-debian9.txt-expected.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.517893 commoncode-31.2.0/tests/data/distro/os-release/elementary/
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/elementary/elementary-0.4.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/elementary/elementary-0.4.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/elementary/elementary-5.1.7.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/elementary/elementary-5.1.7.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/elementary/elementary-5.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/elementary/elementary-5.txt-expected.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.517893 commoncode-31.2.0/tests/data/distro/os-release/endless/
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/endless/endless-3.2.2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/endless/endless-3.2.2.txt-expected.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.533893 commoncode-31.2.0/tests/data/distro/os-release/fedora/
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/fedora/fedora-17.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/fedora/fedora-17.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/fedora/fedora-18.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/fedora/fedora-18.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/fedora/fedora-20.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/fedora/fedora-20.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/fedora/fedora-21.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/fedora/fedora-21.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/fedora/fedora-22-server.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/fedora/fedora-22-server.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/fedora/fedora-22-workstation.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/fedora/fedora-22-workstation.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/fedora/fedora-22.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/fedora/fedora-22.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/fedora/fedora-23-server.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/fedora/fedora-23-server.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/fedora/fedora-23-workstation.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/fedora/fedora-23.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/fedora/fedora-23.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/fedora/fedora-24-server.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/fedora/fedora-24-server.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/fedora/fedora-24-workstation.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/fedora/fedora-24.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/fedora/fedora-24.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/fedora/fedora-25-server.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/fedora/fedora-25-server.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/fedora/fedora-25-workstation.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/fedora/fedora-25-workstation.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/fedora/fedora-25.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/fedora/fedora-25.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/fedora/fedora-26-modular.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/fedora/fedora-26-modular.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/fedora/fedora-26-server.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/fedora/fedora-26-server.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/fedora/fedora-26-workstation.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/fedora/fedora-26-workstation.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/fedora/fedora-26.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/fedora/fedora-26.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/fedora/fedora-27-server.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/fedora/fedora-27-server.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/fedora/fedora-27-workstation.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/fedora/fedora-27-workstation.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/fedora/fedora-27.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/fedora/fedora-27.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/fedora/fedora-28-server.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      725 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/fedora/fedora-28-server.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/fedora/fedora-28-workstation.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/fedora/fedora-28-workstation.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/fedora/fedora-28.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/fedora/fedora-28.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/fedora/fedora-29-container.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/fedora/fedora-29-container.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/fedora/fedora-29-server.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/fedora/fedora-29-server.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/fedora/fedora-29-workstation.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/fedora/fedora-29-workstation.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/fedora/fedora-29.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/fedora/fedora-29.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/fedora/fedora-30-container.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/fedora/fedora-30-container.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/fedora/fedora-30-server.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/fedora/fedora-30-server.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/fedora/fedora-30-workstation.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/fedora/fedora-30-workstation.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/fedora/fedora-30.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/fedora/fedora-30.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/fedora/fedora-31-container.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/fedora/fedora-31-container.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/fedora/fedora-31-server.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/fedora/fedora-31-server.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/fedora/fedora-31-workstation.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/fedora/fedora-31-workstation.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/fedora/fedora-31.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/fedora/fedora-31.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/fedora/fedora-32-container.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/fedora/fedora-32-container.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/fedora/fedora-32-server.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/fedora/fedora-32-server.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/fedora/fedora-32-workstation.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/fedora/fedora-32-workstation.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/fedora/fedora-32.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/fedora/fedora-32.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/fedora/fedora-33-cinnamon.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/fedora/fedora-33-cinnamon.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/fedora/fedora-33-container.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/fedora/fedora-33-container.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/fedora/fedora-33-kde.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/fedora/fedora-33-kde.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/fedora/fedora-33-matecompiz.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/fedora/fedora-33-matecompiz.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/fedora/fedora-33-server.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/fedora/fedora-33-server.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/fedora/fedora-33-soas.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/fedora/fedora-33-soas.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/fedora/fedora-33-workstation.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/fedora/fedora-33-workstation.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/fedora/fedora-33-xfce.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/fedora/fedora-33-xfce.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/fedora/fedora-33.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/fedora/fedora-33.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/fedora/fedora-34-container.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/fedora/fedora-34-container.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/fedora/fedora-34-kde.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/fedora/fedora-34-kde.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/fedora/fedora-34-matecompiz.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/fedora/fedora-34-matecompiz.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/fedora/fedora-34-server.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/fedora/fedora-34-server.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/fedora/fedora-34-soas.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/fedora/fedora-34-soas.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/fedora/fedora-34-workstation.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/fedora/fedora-34-workstation.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/fedora/fedora-34-xfce.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/fedora/fedora-34-xfce.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/fedora/fedora-34.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/fedora/fedora-34.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/fedora/fedora-35.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/fedora/fedora-35.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/fedora/fedora-36-pre.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/fedora/fedora-36-pre.txt-expected.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.537893 commoncode-31.2.0/tests/data/distro/os-release/galliumos/
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/galliumos/galliumos-2.1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/galliumos/galliumos-2.1.txt-expected.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.537893 commoncode-31.2.0/tests/data/distro/os-release/gentoo/
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/gentoo/gentoo-new.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/gentoo/gentoo-new.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/gentoo/gentoo.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/gentoo/gentoo.txt-expected.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.537893 commoncode-31.2.0/tests/data/distro/os-release/ios/
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/ios/ios-xr-6.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/ios/ios-xr-6.txt-expected.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.537893 commoncode-31.2.0/tests/data/distro/os-release/kali/
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/kali/kali-2018.4.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/kali/kali-2018.4.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/kali/kali-2019.2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/kali/kali-2019.2.txt-expected.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.537893 commoncode-31.2.0/tests/data/distro/os-release/kaos/
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/kaos/kaos.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/kaos/kaos.txt-expected.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.537893 commoncode-31.2.0/tests/data/distro/os-release/kdeneon/
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/kdeneon/kdeneon-5.9.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/kdeneon/kdeneon-5.9.txt-expected.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.537893 commoncode-31.2.0/tests/data/distro/os-release/korora/
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/korora/korora-24.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/korora/korora-24.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/korora/korora-26.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/korora/korora-26.txt-expected.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.537893 commoncode-31.2.0/tests/data/distro/os-release/linuxmint/
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/linuxmint/linuxmint-17.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/linuxmint/linuxmint-18.1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/linuxmint/linuxmint-18.1.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/linuxmint/linuxmint-18.2.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/linuxmint/linuxmint-19.txt-expected.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.537893 commoncode-31.2.0/tests/data/distro/os-release/lirios/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/lirios/lirios.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/lirios/lirios.txt-expected.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.541893 commoncode-31.2.0/tests/data/distro/os-release/mageia/
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/mageia/mageia-6.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/mageia/mageia-6.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/mageia/mageia-7.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/mageia/mageia-7.txt-expected.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.541893 commoncode-31.2.0/tests/data/distro/os-release/manjaro/
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/manjaro/manjaro-new.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/manjaro/manjaro-new.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/manjaro/manjaro.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/manjaro/manjaro.txt-expected.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.541893 commoncode-31.2.0/tests/data/distro/os-release/mx-linux/
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/mx-linux/mx-linux.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/mx-linux/mx-linux.txt-expected.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.541893 commoncode-31.2.0/tests/data/distro/os-release/nexus/
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/nexus/nexus-7.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/nexus/nexus-7.txt-expected.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.541893 commoncode-31.2.0/tests/data/distro/os-release/nixos/
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/nixos/nixos.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/nixos/nixos.txt-expected.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.541893 commoncode-31.2.0/tests/data/distro/os-release/opensuse/
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/opensuse/opensuse-13.2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/opensuse/opensuse-13.2.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/opensuse/opensuse-2015.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/opensuse/opensuse-2015.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/opensuse/opensuse-leap-42.1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/opensuse/opensuse-leap-42.1.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/opensuse/opensuse-leap-42.3.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/opensuse/opensuse-leap-42.3.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/opensuse/opensuseleap-15.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/opensuse/opensuseleap-15.0.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/opensuse/opensuseleap-15.1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/opensuse/opensuseleap-15.1.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/opensuse/tumbleweed-2017-0726.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/opensuse/tumbleweed-2017-0726.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/opensuse/tumbleweed-2020-05.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/opensuse/tumbleweed-2020-05.txt-expected.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.545893 commoncode-31.2.0/tests/data/distro/os-release/oraclelinux/
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/oraclelinux/ol-7.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/oraclelinux/ol-7.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/oraclelinux/ol-8.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/oraclelinux/ol-8.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/oraclelinux/oraclelinux-7.6.txt-expected.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.545893 commoncode-31.2.0/tests/data/distro/os-release/peppermintos/
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/peppermintos/peppermintos-7.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/peppermintos/peppermintos-7.txt-expected.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.545893 commoncode-31.2.0/tests/data/distro/os-release/photon/
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/photon/photon-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/photon/photon-4.0.txt-expected.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.545893 commoncode-31.2.0/tests/data/distro/os-release/pop-os/
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/pop-os/pop-os-17.04.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/pop-os/pop-os-17.04.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/pop-os/pop-os-20.04.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/pop-os/pop-os-20.04.txt-expected.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.545893 commoncode-31.2.0/tests/data/distro/os-release/rancheros/
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/rancheros/rancheros-1.4.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/rancheros/rancheros-1.4.txt-expected.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.545893 commoncode-31.2.0/tests/data/distro/os-release/raspbian/
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/raspbian/raspbian-10.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/raspbian/raspbian-10.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/raspbian/raspbian-8.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/raspbian/raspbian-8.txt-expected.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.549893 commoncode-31.2.0/tests/data/distro/os-release/redhat/
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/redhat/rhel-8_0-ga.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/redhat/rhel-8_0-ga.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/redhat/rhel7_2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/redhat/rhel7_2.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/redhat/rhel7_3.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/redhat/rhel7_3.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/redhat/rhel7_4.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/redhat/rhel7_4.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/redhat/rhel7_5.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/redhat/rhel7_5.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/redhat/rhel7_6.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/redhat/rhel7_6.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/redhat/rhel7_7.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/redhat/rhel7_7.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/redhat/rhel8_0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/redhat/rhel8_0.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/redhat/rhel8_1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/redhat/rhel8_1.txt-expected.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.549893 commoncode-31.2.0/tests/data/distro/os-release/redhat-ubi/
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/redhat-ubi/rhel8_5-ubi.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/redhat-ubi/rhel8_5-ubi.txt-expected.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.549893 commoncode-31.2.0/tests/data/distro/os-release/rocky/
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/rocky/rocky-8.4.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/rocky/rocky-8.4.txt-expected.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.549893 commoncode-31.2.0/tests/data/distro/os-release/scientificlinux/
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/scientificlinux/scientific-7.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/scientificlinux/scientific-7.0.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/scientificlinux/scientific-7.1.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/scientificlinux/scientific-7.2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/scientificlinux/scientific-7.2.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/scientificlinux/scientific-7.3.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/scientificlinux/scientific-7.3.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/scientificlinux/scientific-7.4.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/scientificlinux/scientific-7.4.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/scientificlinux/scientific-7.5.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/scientificlinux/scientific-7.5.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/scientificlinux/scientific-7.6.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/scientificlinux/scientific-7.6.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/scientificlinux/scientific-7.7.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/scientificlinux/scientific-7.7.txt-expected.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.549893 commoncode-31.2.0/tests/data/distro/os-release/sharklinux/
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/sharklinux/sharklinux-CR.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/sharklinux/sharklinux-CR.txt-expected.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.553893 commoncode-31.2.0/tests/data/distro/os-release/slackware/
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/slackware/slackware-14.1
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/slackware/slackware-14.1-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/slackware/slackware-14.2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/slackware/slackware-14.2.txt-expected.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.553893 commoncode-31.2.0/tests/data/distro/os-release/sled/
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/sled/sled-12.3.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/sled/sled-12.3.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/sled/sled-15.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/sled/sled-15.txt-expected.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.557893 commoncode-31.2.0/tests/data/distro/os-release/sles/
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/sles/sles11_4.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/sles/sles11_4.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/sles/sles12.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/sles/sles12.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/sles/sles12_1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/sles/sles12_1.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/sles/sles12_2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/sles/sles12_2.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/sles/sles12_3.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/sles/sles12_3.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/sles/sles12_4.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/sles/sles12_4.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/sles/sles12_5.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/sles/sles12_5.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/sles/sles15_0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/sles/sles15_0.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/sles/sles15_1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/sles/sles15_1.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/sles/sles4sap12_0_1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/sles/sles4sap12_0_1.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/sles/sles4sap12_1_0_1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/sles/sles4sap12_1_0_1.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/sles/sles4sap12_2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/sles/sles4sap12_2.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/sles/sles4sap12_3.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/sles/sles4sap12_3.txt-expected.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.557893 commoncode-31.2.0/tests/data/distro/os-release/solus/
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/solus/solus.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/solus/solus.txt-expected.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.565894 commoncode-31.2.0/tests/data/distro/os-release/ubuntu/
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/ubuntu/kylin-16.04.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/ubuntu/ubuntu-12.04.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/ubuntu/ubuntu-12.10.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/ubuntu/ubuntu-12.10.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/ubuntu/ubuntu-13.04.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/ubuntu/ubuntu-13.04.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/ubuntu/ubuntu-13.10.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/ubuntu/ubuntu-13.10.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/ubuntu/ubuntu-14.04-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/ubuntu/ubuntu-14.04.5.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/ubuntu/ubuntu-14.04.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/ubuntu/ubuntu-14.10.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/ubuntu/ubuntu-14.10.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/ubuntu/ubuntu-15.04.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/ubuntu/ubuntu-15.04.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/ubuntu/ubuntu-15.10.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/ubuntu/ubuntu-15.10.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/ubuntu/ubuntu-16.04.5.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/ubuntu/ubuntu-16.04.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/ubuntu/ubuntu-16.10.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/ubuntu/ubuntu-16.10.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/ubuntu/ubuntu-17.04.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/ubuntu/ubuntu-17.04.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/ubuntu/ubuntu-17.10.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/ubuntu/ubuntu-17.10.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/ubuntu/ubuntu-18.04.5.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/ubuntu/ubuntu-18.04.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/ubuntu/ubuntu-18.10.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/ubuntu/ubuntu-18.10.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/ubuntu/ubuntu-19.04.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/ubuntu/ubuntu-19.04.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/ubuntu/ubuntu-19.10.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/ubuntu/ubuntu-19.10.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/ubuntu/ubuntu-20.04.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/ubuntu/ubuntu-20.04.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/ubuntu/ubuntu-20.10.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/ubuntu/ubuntu-20.10.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/ubuntu/ubuntu-21.04.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/ubuntu/ubuntu-21.04.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/ubuntu/ubuntu-21.10.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/ubuntu/ubuntu-21.10.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/ubuntu/ubuntu-artful.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/ubuntu/ubuntu-cosmic.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/ubuntu/ubuntu-disco.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/ubuntu/ubuntu-eoan.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/ubuntu/ubuntu-focal.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/ubuntu/ubuntu-groovy.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/ubuntu/ubuntu-hirsute.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/ubuntu/ubuntu-impish.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/ubuntu/ubuntu-quantal.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/ubuntu/ubuntu-raring.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/ubuntu/ubuntu-saucy.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/ubuntu/ubuntu-utopic.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/ubuntu/ubuntu-vivid.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/ubuntu/ubuntu-wily.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/ubuntu/ubuntu-yakkety.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/ubuntu/ubuntu-zesty.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.565894 commoncode-31.2.0/tests/data/distro/os-release/xbian/
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/xbian/xbian.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/xbian/xbian.txt-expected.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.565894 commoncode-31.2.0/tests/data/distro/os-release/xcp/
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/xcp/xcp-7.5.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/xcp/xcp-7.5.0.txt-expected.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.565894 commoncode-31.2.0/tests/data/distro/os-release/xenserver/
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/xenserver/xenserver-7.6.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/xenserver/xenserver-7.6.txt-expected.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.565894 commoncode-31.2.0/tests/data/distro/os-release/zorinos/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/zorinos/zorinos-12.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release/zorinos/zorinos-12.txt-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release-chef.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release-nate.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/distro/os-release-zoo.ABOUT
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.565894 commoncode-31.2.0/tests/data/fileset/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/fileset/scancodeignore.lst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.565894 commoncode-31.2.0/tests/data/filetype/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.481893 commoncode-31.2.0/tests/data/filetype/readwrite/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.565894 commoncode-31.2.0/tests/data/filetype/readwrite/sub/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/filetype/readwrite/sub/file
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.565894 commoncode-31.2.0/tests/data/filetype/size/
+-rw-r--r--   0 runner    (1001) docker     (127)    12388 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/filetype/size/Image1.eps
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.565894 commoncode-31.2.0/tests/data/filetype/size/exec/
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/filetype/size/exec/1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/filetype/size/exec/a.bat
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/filetype/size/exec/a.tar
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.565894 commoncode-31.2.0/tests/data/filetype/size/exec/subtxt/
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/filetype/size/exec/subtxt/1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/filetype/size/exec/subtxt/a.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/filetype/size/exec/subtxt/b.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   109056 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/filetype/types.tar
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.485893 commoncode-31.2.0/tests/data/fileutils/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.565894 commoncode-31.2.0/tests/data/fileutils/basename/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.565894 commoncode-31.2.0/tests/data/fileutils/basename/a/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.565894 commoncode-31.2.0/tests/data/fileutils/basename/a/.a/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/fileutils/basename/a/.a/file
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.565894 commoncode-31.2.0/tests/data/fileutils/basename/a/b/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/fileutils/basename/a/b/.a
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/fileutils/basename/a/b/.a.b
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/fileutils/basename/a/b/a.tag.gz
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/fileutils/basename/a/f.a
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.565894 commoncode-31.2.0/tests/data/fileutils/basename/f.a/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/fileutils/basename/f.a/a.c
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/fileutils/basename/tst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.565894 commoncode-31.2.0/tests/data/fileutils/exec/
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/fileutils/exec/1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/fileutils/exec/a.bat
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/fileutils/exec/a.tar
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.569893 commoncode-31.2.0/tests/data/fileutils/exec/subtxt/
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/fileutils/exec/subtxt/1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/fileutils/exec/subtxt/a.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/fileutils/exec/subtxt/b.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.481893 commoncode-31.2.0/tests/data/fileutils/executable/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.481893 commoncode-31.2.0/tests/data/fileutils/executable/deep1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.569893 commoncode-31.2.0/tests/data/fileutils/executable/deep1/deep2/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/fileutils/executable/deep1/deep2/ctags
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.569893 commoncode-31.2.0/tests/data/fileutils/filetype/
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/fileutils/filetype/a.html
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/fileutils/filetype/stage1
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.569893 commoncode-31.2.0/tests/data/fileutils/perms/
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/fileutils/perms/unreadable.tgz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.485893 commoncode-31.2.0/tests/data/fileutils/readwrite/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.569893 commoncode-31.2.0/tests/data/fileutils/readwrite/sub/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/fileutils/readwrite/sub/file
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.569893 commoncode-31.2.0/tests/data/fileutils/walk/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.569893 commoncode-31.2.0/tests/data/fileutils/walk/d1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.569893 commoncode-31.2.0/tests/data/fileutils/walk/d1/d2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.569893 commoncode-31.2.0/tests/data/fileutils/walk/d1/d2/d3/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/fileutils/walk/d1/d2/d3/f3
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/fileutils/walk/d1/d2/f2
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/fileutils/walk/d1/f1
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/fileutils/walk/f
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/fileutils/walk/unicode.zip
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.569893 commoncode-31.2.0/tests/data/fileutils/walk_non_utf8/
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/fileutils/walk_non_utf8/non_unicode.tgz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.485893 commoncode-31.2.0/tests/data/hash/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.569893 commoncode-31.2.0/tests/data/hash/dir1/
+-rw-r--r--   0 runner    (1001) docker     (127)     7859 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/hash/dir1/a.png
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/hash/dir1/a.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.569893 commoncode-31.2.0/tests/data/hash/dir2/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/hash/dir2/a.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/hash/dir2/dos.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.569893 commoncode-31.2.0/tests/data/hash/sha1-collision/
+-rw-r--r--   0 runner    (1001) docker     (127)   422435 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/hash/sha1-collision/shattered-1.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/hash/sha1-collision/shattered-1.pdf.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (127)   422435 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/hash/sha1-collision/shattered-2.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/hash/sha1-collision/shattered-2.pdf.ABOUT
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.569893 commoncode-31.2.0/tests/data/ignore/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/ignore/.scancodeignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.573894 commoncode-31.2.0/tests/data/ignore/excludes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/ignore/excludes/.localized
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/ignore/excludes/eclipse.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/ignore/excludes/mac.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/ignore/excludes/msft-vs.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)     6296 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/ignore/vcs.tgz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.493893 commoncode-31.2.0/tests/data/resource/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.485893 commoncode-31.2.0/tests/data/resource/cache/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.573894 commoncode-31.2.0/tests/data/resource/cache/package/
+-rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/cache/package/package.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.573894 commoncode-31.2.0/tests/data/resource/cache2/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/cache2/abc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.573894 commoncode-31.2.0/tests/data/resource/cache2/dir/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/cache2/dir/that
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/cache2/dir/this
+-rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/cache2/et131x.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.573894 commoncode-31.2.0/tests/data/resource/cache2/other dir/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/cache2/other dir/file
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.485893 commoncode-31.2.0/tests/data/resource/client/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.573894 commoncode-31.2.0/tests/data/resource/client/Images/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/client/Images/applicationCache.png
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/client/Images/spinner.gif
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.573894 commoncode-31.2.0/tests/data/resource/codebase/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/codebase/abc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.573894 commoncode-31.2.0/tests/data/resource/codebase/dir/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/codebase/dir/that
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/codebase/dir/this
+-rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/codebase/et131x.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.573894 commoncode-31.2.0/tests/data/resource/codebase/other dir/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/codebase/other dir/file
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.573894 commoncode-31.2.0/tests/data/resource/deeply_nested/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.573894 commoncode-31.2.0/tests/data/resource/deeply_nested/level1_dir1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.573894 commoncode-31.2.0/tests/data/resource/deeply_nested/level1_dir1/level2_dir1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.573894 commoncode-31.2.0/tests/data/resource/deeply_nested/level1_dir1/level2_dir1/level3_dir1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/deeply_nested/level1_dir1/level2_dir1/level3_dir1/level4_file1
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/deeply_nested/level1_dir1/level2_dir1/level3_file1
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/deeply_nested/level1_dir1/level2_dir1/level3_file2
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/deeply_nested/level1_dir1/level2_file1
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/deeply_nested/level1_dir1/level2_file2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.573894 commoncode-31.2.0/tests/data/resource/deeply_nested/level1_dir2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.573894 commoncode-31.2.0/tests/data/resource/deeply_nested/level1_dir2/level2_dir3/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/deeply_nested/level1_dir2/level2_dir3/level3_file3
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/deeply_nested/level1_dir2/level2_dir3/level3_file4
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/deeply_nested/level1_dir2/level2_file3
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/deeply_nested/level1_dir2/level2_file4
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/deeply_nested/level1_dir2/level2_file5
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/deeply_nested/level1_file1
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/deeply_nested/level1_file2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.485893 commoncode-31.2.0/tests/data/resource/dist/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.573894 commoncode-31.2.0/tests/data/resource/dist/JGroups/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/dist/JGroups/EULA
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/dist/JGroups/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.577894 commoncode-31.2.0/tests/data/resource/dist/JGroups/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/dist/JGroups/src/RouterStub.java
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/dist/JGroups/src/RouterStubManager.java
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/dist/JGroups/src/S3_PING.java
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.485893 commoncode-31.2.0/tests/data/resource/dist/simple/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.577894 commoncode-31.2.0/tests/data/resource/dist/simple/META-INF/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/dist/simple/META-INF/MANIFEST.MF
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.577894 commoncode-31.2.0/tests/data/resource/ignore/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.577894 commoncode-31.2.0/tests/data/resource/ignore/cvs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/ignore/cvs/file2
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/ignore/file1
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.485893 commoncode-31.2.0/tests/data/resource/lcp/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.577894 commoncode-31.2.0/tests/data/resource/lcp/test1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.577894 commoncode-31.2.0/tests/data/resource/lcp/test1/JGroups/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/lcp/test1/JGroups/EULA
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/lcp/test1/JGroups/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.577894 commoncode-31.2.0/tests/data/resource/lcp/test1/JGroups/licenses/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/lcp/test1/JGroups/licenses/apache-1.1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/lcp/test1/JGroups/licenses/lgpl.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.577894 commoncode-31.2.0/tests/data/resource/lcp/test1/JGroups/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/lcp/test1/JGroups/src/RouterStub.java
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/lcp/test1/JGroups/src/RouterStubManager.java
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/lcp/test1/JGroups/src/S3_PING.java
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/lcp/test1/screenshot.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.489893 commoncode-31.2.0/tests/data/resource/lcp/test1/simple/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.577894 commoncode-31.2.0/tests/data/resource/lcp/test1/simple/META-INF/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/lcp/test1/simple/META-INF/MANIFEST.MF
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.489893 commoncode-31.2.0/tests/data/resource/lcp/test1/simple/org/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.489893 commoncode-31.2.0/tests/data/resource/lcp/test1/simple/org/jvnet/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.489893 commoncode-31.2.0/tests/data/resource/lcp/test1/simple/org/jvnet/glassfish/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.489893 commoncode-31.2.0/tests/data/resource/lcp/test1/simple/org/jvnet/glassfish/comms/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.577894 commoncode-31.2.0/tests/data/resource/lcp/test1/simple/org/jvnet/glassfish/comms/sipagent/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.577894 commoncode-31.2.0/tests/data/resource/lcp/test1/simple/org/jvnet/glassfish/comms/sipagent/actions/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/lcp/test1/simple/org/jvnet/glassfish/comms/sipagent/actions/Bundle.properties
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/lcp/test1/simple/org/jvnet/glassfish/comms/sipagent/actions/SipAgentCookieAction.class
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/lcp/test1/simple/org/jvnet/glassfish/comms/sipagent/actions/bd.png
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/lcp/test1/simple/org/jvnet/glassfish/comms/sipagent/actions/bd24.png
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/lcp/test1/simple/org/jvnet/glassfish/comms/sipagent/org-jvnet-glassfish-comms-sipagent-actions-SipAgentCookieAction.instance
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/lcp/test1/simple/org/jvnet/glassfish/comms/sipagent/org-jvnet-glassfish-comms-sipagent-actions-SipAgentCookieAction_1.instance
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.489893 commoncode-31.2.0/tests/data/resource/lcp/test1/zlib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.577894 commoncode-31.2.0/tests/data/resource/lcp/test1/zlib/ada/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/lcp/test1/zlib/ada/zlib.ads
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.489893 commoncode-31.2.0/tests/data/resource/lcp/test1/zlib/inter/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.577894 commoncode-31.2.0/tests/data/resource/lcp/test1/zlib/inter/arch/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/lcp/test1/zlib/inter/arch/zlib.tar.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.577894 commoncode-31.2.0/tests/data/resource/lcp/test1/zlib/inter/dir/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/lcp/test1/zlib/inter/dir/EULA
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/lcp/test1/zlib/inter/dir/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.577894 commoncode-31.2.0/tests/data/resource/lcp/test1/zlib/inter/dir/licenses/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/lcp/test1/zlib/inter/dir/licenses/apache-1.1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/lcp/test1/zlib/inter/dir/licenses/apache-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/lcp/test1/zlib/inter/dir/licenses/bouncycastle.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/lcp/test1/zlib/inter/dir/licenses/cpl-1.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/lcp/test1/zlib/inter/dir/licenses/lgpl.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.581894 commoncode-31.2.0/tests/data/resource/lcp/test1/zlib/inter/dir/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/lcp/test1/zlib/inter/dir/src/FixedMembershipToken.java
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/lcp/test1/zlib/inter/dir/src/GuardedBy.java
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/lcp/test1/zlib/inter/dir/src/ImmutableReference.java
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/lcp/test1/zlib/inter/dir/src/RATE_LIMITER.java
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/lcp/test1/zlib/inter/dir/src/RouterStub.java
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/lcp/test1/zlib/inter/dir/src/RouterStubManager.java
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/lcp/test1/zlib/inter/dir/src/S3_PING.java
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.581894 commoncode-31.2.0/tests/data/resource/lcp/test1/zlib/inter/iostream2/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/lcp/test1/zlib/inter/iostream2/zstream.h
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/lcp/test1/zlib/inter/iostream2/zstream_test.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.581894 commoncode-31.2.0/tests/data/resource/lcp/test1/zlib/inter/zlib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.581894 commoncode-31.2.0/tests/data/resource/lcp/test1/zlib/inter/zlib/ada/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/lcp/test1/zlib/inter/zlib/ada/zlib.ads
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/lcp/test1/zlib/inter/zlib/adler32.c
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/lcp/test1/zlib/inter/zlib/deflate.c
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/lcp/test1/zlib/inter/zlib/deflate.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.581894 commoncode-31.2.0/tests/data/resource/lcp/test1/zlib/inter/zlib/dotzlib/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/lcp/test1/zlib/inter/zlib/dotzlib/AssemblyInfo.cs
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/lcp/test1/zlib/inter/zlib/dotzlib/ChecksumImpl.cs
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/lcp/test1/zlib/inter/zlib/dotzlib/LICENSE_1_0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/lcp/test1/zlib/inter/zlib/dotzlib/readme.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.581894 commoncode-31.2.0/tests/data/resource/lcp/test1/zlib/inter/zlib/gcc_gvmat64/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/lcp/test1/zlib/inter/zlib/gcc_gvmat64/gvmat64.S
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.581894 commoncode-31.2.0/tests/data/resource/lcp/test1/zlib/inter/zlib/infback9/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/lcp/test1/zlib/inter/zlib/infback9/infback9.c
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/lcp/test1/zlib/inter/zlib/infback9/infback9.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.581894 commoncode-31.2.0/tests/data/resource/lcp/test1/zlib/inter/zlib/iostream2/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/lcp/test1/zlib/inter/zlib/iostream2/zstream.h
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/lcp/test1/zlib/inter/zlib/iostream2/zstream_test.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/lcp/test1/zlib/inter/zlib/zlib.h
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/lcp/test1/zlib/inter/zlib/zutil.c
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/lcp/test1/zlib/inter/zlib/zutil.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.581894 commoncode-31.2.0/tests/data/resource/resource/
+-rw-r--r--   0 runner    (1001) docker     (127)     7194 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/resource/test-extracted-from-to.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.581894 commoncode-31.2.0/tests/data/resource/samples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.585893 commoncode-31.2.0/tests/data/resource/samples/JGroups/
+-rw-r--r--   0 runner    (1001) docker     (127)     8156 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/samples/JGroups/EULA
+-rw-r--r--   0 runner    (1001) docker     (127)    26430 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/samples/JGroups/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.585893 commoncode-31.2.0/tests/data/resource/samples/JGroups/licenses/
+-rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/samples/JGroups/licenses/apache-1.1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11560 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/samples/JGroups/licenses/apache-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/samples/JGroups/licenses/bouncycastle.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11987 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/samples/JGroups/licenses/cpl-1.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    26934 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/samples/JGroups/licenses/lgpl.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.585893 commoncode-31.2.0/tests/data/resource/samples/JGroups/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     5144 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/samples/JGroups/src/FixedMembershipToken.java
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/samples/JGroups/src/GuardedBy.java
+-rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/samples/JGroups/src/ImmutableReference.java
+-rw-r--r--   0 runner    (1001) docker     (127)     3692 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/samples/JGroups/src/RATE_LIMITER.java
+-rw-r--r--   0 runner    (1001) docker     (127)     9913 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/samples/JGroups/src/RouterStub.java
+-rw-r--r--   0 runner    (1001) docker     (127)     8162 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/samples/JGroups/src/RouterStubManager.java
+-rw-r--r--   0 runner    (1001) docker     (127)   122528 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/samples/JGroups/src/S3_PING.java
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/samples/README
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.585893 commoncode-31.2.0/tests/data/resource/samples/arch/
+-rw-r--r--   0 runner    (1001) docker     (127)    28103 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/samples/arch/zlib.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (127)   622754 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/samples/screenshot.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.585893 commoncode-31.2.0/tests/data/resource/samples/zlib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.585893 commoncode-31.2.0/tests/data/resource/samples/zlib/ada/
+-rw-r--r--   0 runner    (1001) docker     (127)    13594 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/samples/zlib/ada/zlib.ads
+-rw-r--r--   0 runner    (1001) docker     (127)     4968 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/samples/zlib/adler32.c
+-rw-r--r--   0 runner    (1001) docker     (127)    71476 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/samples/zlib/deflate.c
+-rw-r--r--   0 runner    (1001) docker     (127)    12774 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/samples/zlib/deflate.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.585893 commoncode-31.2.0/tests/data/resource/samples/zlib/dotzlib/
+-rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/samples/zlib/dotzlib/AssemblyInfo.cs
+-rw-r--r--   0 runner    (1001) docker     (127)     8040 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/samples/zlib/dotzlib/ChecksumImpl.cs
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/samples/zlib/dotzlib/LICENSE_1_0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/samples/zlib/dotzlib/readme.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.589894 commoncode-31.2.0/tests/data/resource/samples/zlib/gcc_gvmat64/
+-rw-r--r--   0 runner    (1001) docker     (127)    16413 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/samples/zlib/gcc_gvmat64/gvmat64.S
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.589894 commoncode-31.2.0/tests/data/resource/samples/zlib/infback9/
+-rw-r--r--   0 runner    (1001) docker     (127)    21629 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/samples/zlib/infback9/infback9.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/samples/zlib/infback9/infback9.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.589894 commoncode-31.2.0/tests/data/resource/samples/zlib/iostream2/
+-rw-r--r--   0 runner    (1001) docker     (127)     9283 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/samples/zlib/iostream2/zstream.h
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/samples/zlib/iostream2/zstream_test.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    87883 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/samples/zlib/zlib.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7414 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/samples/zlib/zutil.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6766 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/samples/zlib/zutil.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.589894 commoncode-31.2.0/tests/data/resource/skip_directories_during_walk/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.589894 commoncode-31.2.0/tests/data/resource/skip_directories_during_walk/skip-this-directory/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/skip_directories_during_walk/skip-this-directory/this-should-not-be-returned
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/skip_directories_during_walk/this-should-be-returned
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.593894 commoncode-31.2.0/tests/data/resource/virtual_codebase/
+-rw-r--r--   0 runner    (1001) docker     (127)     4628 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/virtual_codebase/codebase-for-cache-tests.json
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/virtual_codebase/combine-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/virtual_codebase/combine-2.json
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/virtual_codebase/combine-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/virtual_codebase/combine-shared-directory-name-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/virtual_codebase/combine-shared-directory-name-2.json
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/virtual_codebase/combine-shared-directory-name-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5129 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/virtual_codebase/docker-hello-world.json
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/virtual_codebase/et131x.h.json
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/virtual_codebase/fingerprint_attribute.json
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/virtual_codebase/from_file.json
+-rw-r--r--   0 runner    (1001) docker     (127)    17547 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/virtual_codebase/full-root-info-many-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)    16812 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/virtual_codebase/full-root-info-many.json
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/virtual_codebase/full-root-info-one-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/virtual_codebase/full-root-info-one.json
+-rw-r--r--   0 runner    (1001) docker     (127)    50927 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/virtual_codebase/lcp.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5671 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/virtual_codebase/license-scan.json
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/virtual_codebase/node-16-slim.json
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/virtual_codebase/noinfo.json
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/virtual_codebase/only-path.json
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/virtual_codebase/resource.json
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/virtual_codebase/root-is-not-first-resource.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8187 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/virtual_codebase/samples-only-findings-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4410 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/virtual_codebase/samples-only-findings.json
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/virtual_codebase/stripped-and-skipped-root.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/virtual_codebase/virtual_codebase.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6690 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/virtual_codebase/zephyr-binary.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.593894 commoncode-31.2.0/tests/data/resource/with_path/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.593894 commoncode-31.2.0/tests/data/resource/with_path/codebase/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/with_path/codebase/abc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.593894 commoncode-31.2.0/tests/data/resource/with_path/codebase/dir/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/with_path/codebase/dir/that
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/with_path/codebase/dir/this
+-rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/with_path/codebase/et131x.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.593894 commoncode-31.2.0/tests/data/resource/with_path/codebase/other dir/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/with_path/codebase/other dir/file
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/with_path/codebase-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/with_path/virtual-codebase-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/resource/with_path/virtual-codebase.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.593894 commoncode-31.2.0/tests/data/saneyaml/
+-rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/saneyaml/metadata1
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/saneyaml/metadata1.notag
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.593894 commoncode-31.2.0/tests/data/symlink/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/symlink/test
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.593894 commoncode-31.2.0/tests/data/symlink/walk/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/symlink/walk/a
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:30.593894 commoncode-31.2.0/tests/data/symlink/walk/dir/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/data/symlink/walk/dir/b
+-rw-r--r--   0 runner    (1001) docker     (127)     5114 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/test_cliutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/test_cliutils_progressbar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/test_codec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5946 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/test_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/test_date.py
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/test_distro.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4130 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/test_fileset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7749 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/test_filetype.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39362 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/test_fileutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/test_functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7107 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/test_hash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8215 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/test_ignore.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12779 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/test_paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63974 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/test_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/test_saneyaml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/test_skeleton_codestyle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/test_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3671 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/test_timeutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5784 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/test_urn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8797 2024-05-16 18:35:26.000000 commoncode-31.2.0/tests/test_version.py
```

### Comparing `commoncode-31.1.0/.github/workflows/docs-ci.yml` & `commoncode-31.2.0/.github/workflows/docs-ci.yml`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/.github/workflows/pypi-release.yml` & `commoncode-31.2.0/.github/workflows/pypi-release.yml`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/.gitignore` & `commoncode-31.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/.readthedocs.yml` & `commoncode-31.2.0/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/CHANGELOG.rst` & `commoncode-31.2.0/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 Release notes
 =============
 
+Version 31.2.0 - (2024-05-16)
+-----------------------------
+
+- Add ``commoncode.distro.os_release_parser`` from container-inspector to commoncode.
+
+
 Version 31.1.0 - (2024-05-15)
 ------------------------------
 
 - Add ``on_macos_arm64`` and ``on_ubuntu_22`` markers to ``commoncode.system``.
 
 
 Version 31.0.3 - (2023-08-25)
```

### Comparing `commoncode-31.1.0/CODE_OF_CONDUCT.rst` & `commoncode-31.2.0/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/Makefile` & `commoncode-31.2.0/Makefile`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/PKG-INFO` & `commoncode-31.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: commoncode
-Version: 31.1.0
+Version: 31.2.0
 Summary: Set of common utilities, originally split from ScanCode
 Home-page: https://github.com/nexB/commoncode
 Author: nexB. Inc. and others
 Author-email: info@aboutcode.org
 License: Apache-2.0
 Keywords: utilities,scancode-toolkit
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `commoncode-31.1.0/README.rst` & `commoncode-31.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/apache-2.0.LICENSE` & `commoncode-31.2.0/apache-2.0.LICENSE`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/azure-pipelines.yml` & `commoncode-31.2.0/azure-pipelines.yml`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/commoncode.ABOUT` & `commoncode-31.2.0/commoncode.ABOUT`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/configure` & `commoncode-31.2.0/configure`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/configure.bat` & `commoncode-31.2.0/configure.bat`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/docs/Makefile` & `commoncode-31.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/docs/make.bat` & `commoncode-31.2.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/docs/source/_static/theme_overrides.css` & `commoncode-31.2.0/docs/source/_static/theme_overrides.css`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/docs/source/conf.py` & `commoncode-31.2.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/docs/source/contribute/contrib_doc.rst` & `commoncode-31.2.0/docs/source/contribute/contrib_doc.rst`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/etc/ci/azure-container-deb.yml` & `commoncode-31.2.0/etc/ci/azure-container-deb.yml`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/etc/ci/azure-container-rpm.yml` & `commoncode-31.2.0/etc/ci/azure-container-rpm.yml`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/etc/ci/azure-posix.yml` & `commoncode-31.2.0/etc/ci/azure-posix.yml`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/etc/ci/azure-win.yml` & `commoncode-31.2.0/etc/ci/azure-win.yml`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/etc/ci/macports-ci` & `commoncode-31.2.0/etc/ci/macports-ci`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/etc/ci/macports-ci.ABOUT` & `commoncode-31.2.0/etc/ci/macports-ci.ABOUT`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/etc/ci/mit.LICENSE` & `commoncode-31.2.0/etc/ci/mit.LICENSE`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/etc/scripts/README.rst` & `commoncode-31.2.0/etc/scripts/README.rst`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/etc/scripts/check_thirdparty.py` & `commoncode-31.2.0/etc/scripts/check_thirdparty.py`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/etc/scripts/fetch_thirdparty.py` & `commoncode-31.2.0/etc/scripts/fetch_thirdparty.py`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/etc/scripts/gen_pypi_simple.py` & `commoncode-31.2.0/etc/scripts/gen_pypi_simple.py`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/etc/scripts/gen_pypi_simple.py.NOTICE` & `commoncode-31.2.0/etc/scripts/gen_pypi_simple.py.NOTICE`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/etc/scripts/gen_requirements.py` & `commoncode-31.2.0/etc/scripts/gen_requirements.py`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/etc/scripts/gen_requirements_dev.py` & `commoncode-31.2.0/etc/scripts/gen_requirements_dev.py`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/etc/scripts/test_utils_pip_compatibility_tags.py` & `commoncode-31.2.0/etc/scripts/test_utils_pip_compatibility_tags.py`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/etc/scripts/test_utils_pypi_supported_tags.py` & `commoncode-31.2.0/etc/scripts/test_utils_pypi_supported_tags.py`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/etc/scripts/test_utils_pypi_supported_tags.py.ABOUT` & `commoncode-31.2.0/etc/scripts/test_utils_pypi_supported_tags.py.ABOUT`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/etc/scripts/utils_dejacode.py` & `commoncode-31.2.0/etc/scripts/utils_dejacode.py`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/etc/scripts/utils_pip_compatibility_tags.py` & `commoncode-31.2.0/etc/scripts/utils_pip_compatibility_tags.py`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/etc/scripts/utils_pypi_supported_tags.py` & `commoncode-31.2.0/etc/scripts/utils_pypi_supported_tags.py`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/etc/scripts/utils_pypi_supported_tags.py.ABOUT` & `commoncode-31.2.0/etc/scripts/utils_pypi_supported_tags.py.ABOUT`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/etc/scripts/utils_requirements.py` & `commoncode-31.2.0/etc/scripts/utils_requirements.py`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/etc/scripts/utils_thirdparty.py` & `commoncode-31.2.0/etc/scripts/utils_thirdparty.py`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/etc/scripts/utils_thirdparty.py.ABOUT` & `commoncode-31.2.0/etc/scripts/utils_thirdparty.py.ABOUT`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/pyproject.toml` & `commoncode-31.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/requirements-dev.txt` & `commoncode-31.2.0/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/setup.cfg` & `commoncode-31.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/src/commoncode/__init__.py` & `commoncode-31.2.0/src/commoncode/__init__.py`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/src/commoncode/archive.py` & `commoncode-31.2.0/src/commoncode/archive.py`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/src/commoncode/cliutils.py` & `commoncode-31.2.0/src/commoncode/cliutils.py`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/src/commoncode/codec.py` & `commoncode-31.2.0/src/commoncode/codec.py`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/src/commoncode/command.py` & `commoncode-31.2.0/src/commoncode/command.py`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/src/commoncode/datautils.py` & `commoncode-31.2.0/src/commoncode/datautils.py`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/src/commoncode/date.py` & `commoncode-31.2.0/src/commoncode/date.py`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/src/commoncode/dict_utils.py` & `commoncode-31.2.0/src/commoncode/dict_utils.py`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/src/commoncode/fetch.py` & `commoncode-31.2.0/src/commoncode/fetch.py`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/src/commoncode/fileset.py` & `commoncode-31.2.0/src/commoncode/fileset.py`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/src/commoncode/filetype.py` & `commoncode-31.2.0/src/commoncode/filetype.py`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/src/commoncode/fileutils.py` & `commoncode-31.2.0/src/commoncode/fileutils.py`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/src/commoncode/fileutils.py.ABOUT` & `commoncode-31.2.0/src/commoncode/fileutils.py.ABOUT`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/src/commoncode/functional.py` & `commoncode-31.2.0/src/commoncode/functional.py`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/src/commoncode/hash.py` & `commoncode-31.2.0/src/commoncode/hash.py`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/src/commoncode/ignore.py` & `commoncode-31.2.0/src/commoncode/ignore.py`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/src/commoncode/paths.py` & `commoncode-31.2.0/src/commoncode/paths.py`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/src/commoncode/python.LICENSE` & `commoncode-31.2.0/src/commoncode/python.LICENSE`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/src/commoncode/resource.py` & `commoncode-31.2.0/src/commoncode/resource.py`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/src/commoncode/system.py` & `commoncode-31.2.0/src/commoncode/system.py`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/src/commoncode/testcase.py` & `commoncode-31.2.0/src/commoncode/testcase.py`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/src/commoncode/text.py` & `commoncode-31.2.0/src/commoncode/text.py`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/src/commoncode/timeutils.py` & `commoncode-31.2.0/src/commoncode/timeutils.py`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/src/commoncode/urn.py` & `commoncode-31.2.0/src/commoncode/urn.py`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/src/commoncode/version.py` & `commoncode-31.2.0/src/commoncode/version.py`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/src/commoncode.egg-info/PKG-INFO` & `commoncode-31.2.0/src/commoncode.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: commoncode
-Version: 31.1.0
+Version: 31.2.0
 Summary: Set of common utilities, originally split from ScanCode
 Home-page: https://github.com/nexB/commoncode
 Author: nexB. Inc. and others
 Author-email: info@aboutcode.org
 License: Apache-2.0
 Keywords: utilities,scancode-toolkit
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `commoncode-31.1.0/tests/data/date/ant-jsch-1.7.0.tar.gz` & `commoncode-31.2.0/tests/data/date/ant-jsch-1.7.0.tar.gz`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/tests/data/filetype/size/Image1.eps` & `commoncode-31.2.0/tests/data/filetype/size/Image1.eps`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/tests/data/filetype/types.tar` & `commoncode-31.2.0/tests/data/filetype/types.tar`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/tests/data/fileutils/filetype/stage1` & `commoncode-31.2.0/tests/data/fileutils/filetype/stage1`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/tests/data/fileutils/walk/unicode.zip` & `commoncode-31.2.0/tests/data/fileutils/walk/unicode.zip`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/tests/data/hash/dir1/a.png` & `commoncode-31.2.0/tests/data/hash/dir1/a.png`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/tests/data/hash/sha1-collision/shattered-1.pdf` & `commoncode-31.2.0/tests/data/hash/sha1-collision/shattered-1.pdf`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/tests/data/hash/sha1-collision/shattered-2.pdf` & `commoncode-31.2.0/tests/data/hash/sha1-collision/shattered-2.pdf`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/tests/data/ignore/vcs.tgz` & `commoncode-31.2.0/tests/data/ignore/vcs.tgz`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/tests/data/resource/cache/package/package.json` & `commoncode-31.2.0/tests/data/resource/cache/package/package.json`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/tests/data/resource/cache2/et131x.h` & `commoncode-31.2.0/tests/data/resource/cache2/et131x.h`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/tests/data/resource/codebase/et131x.h` & `commoncode-31.2.0/tests/data/resource/codebase/et131x.h`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/tests/data/resource/resource/test-extracted-from-to.json` & `commoncode-31.2.0/tests/data/resource/resource/test-extracted-from-to.json`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/tests/data/resource/samples/JGroups/EULA` & `commoncode-31.2.0/tests/data/resource/samples/JGroups/EULA`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/tests/data/resource/samples/JGroups/LICENSE` & `commoncode-31.2.0/tests/data/resource/samples/JGroups/LICENSE`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/tests/data/resource/samples/JGroups/licenses/apache-1.1.txt` & `commoncode-31.2.0/tests/data/resource/samples/JGroups/licenses/apache-1.1.txt`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/tests/data/resource/samples/JGroups/licenses/apache-2.0.txt` & `commoncode-31.2.0/tests/data/resource/samples/JGroups/licenses/apache-2.0.txt`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/tests/data/resource/samples/JGroups/licenses/bouncycastle.txt` & `commoncode-31.2.0/tests/data/resource/samples/JGroups/licenses/bouncycastle.txt`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/tests/data/resource/samples/JGroups/licenses/cpl-1.0.txt` & `commoncode-31.2.0/tests/data/resource/samples/JGroups/licenses/cpl-1.0.txt`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/tests/data/resource/samples/JGroups/licenses/lgpl.txt` & `commoncode-31.2.0/tests/data/resource/samples/JGroups/licenses/lgpl.txt`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/tests/data/resource/samples/JGroups/src/FixedMembershipToken.java` & `commoncode-31.2.0/tests/data/resource/samples/JGroups/src/FixedMembershipToken.java`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/tests/data/resource/samples/JGroups/src/GuardedBy.java` & `commoncode-31.2.0/tests/data/resource/samples/JGroups/src/GuardedBy.java`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/tests/data/resource/samples/JGroups/src/ImmutableReference.java` & `commoncode-31.2.0/tests/data/resource/samples/JGroups/src/ImmutableReference.java`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/tests/data/resource/samples/JGroups/src/RATE_LIMITER.java` & `commoncode-31.2.0/tests/data/resource/samples/JGroups/src/RATE_LIMITER.java`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/tests/data/resource/samples/JGroups/src/RouterStub.java` & `commoncode-31.2.0/tests/data/resource/samples/JGroups/src/RouterStub.java`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/tests/data/resource/samples/JGroups/src/RouterStubManager.java` & `commoncode-31.2.0/tests/data/resource/samples/JGroups/src/RouterStubManager.java`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/tests/data/resource/samples/JGroups/src/S3_PING.java` & `commoncode-31.2.0/tests/data/resource/samples/JGroups/src/S3_PING.java`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/tests/data/resource/samples/arch/zlib.tar.gz` & `commoncode-31.2.0/tests/data/resource/samples/arch/zlib.tar.gz`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/tests/data/resource/samples/screenshot.png` & `commoncode-31.2.0/tests/data/resource/samples/screenshot.png`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/tests/data/resource/samples/zlib/ada/zlib.ads` & `commoncode-31.2.0/tests/data/resource/samples/zlib/ada/zlib.ads`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/tests/data/resource/samples/zlib/adler32.c` & `commoncode-31.2.0/tests/data/resource/samples/zlib/adler32.c`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/tests/data/resource/samples/zlib/deflate.c` & `commoncode-31.2.0/tests/data/resource/samples/zlib/deflate.c`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/tests/data/resource/samples/zlib/deflate.h` & `commoncode-31.2.0/tests/data/resource/samples/zlib/deflate.h`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/tests/data/resource/samples/zlib/dotzlib/AssemblyInfo.cs` & `commoncode-31.2.0/tests/data/resource/samples/zlib/dotzlib/AssemblyInfo.cs`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/tests/data/resource/samples/zlib/dotzlib/ChecksumImpl.cs` & `commoncode-31.2.0/tests/data/resource/samples/zlib/dotzlib/ChecksumImpl.cs`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/tests/data/resource/samples/zlib/dotzlib/LICENSE_1_0.txt` & `commoncode-31.2.0/tests/data/resource/samples/zlib/dotzlib/LICENSE_1_0.txt`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/tests/data/resource/samples/zlib/dotzlib/readme.txt` & `commoncode-31.2.0/tests/data/resource/samples/zlib/dotzlib/readme.txt`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/tests/data/resource/samples/zlib/gcc_gvmat64/gvmat64.S` & `commoncode-31.2.0/tests/data/resource/samples/zlib/gcc_gvmat64/gvmat64.S`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/tests/data/resource/samples/zlib/infback9/infback9.c` & `commoncode-31.2.0/tests/data/resource/samples/zlib/infback9/infback9.c`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/tests/data/resource/samples/zlib/infback9/infback9.h` & `commoncode-31.2.0/tests/data/resource/samples/zlib/infback9/infback9.h`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/tests/data/resource/samples/zlib/iostream2/zstream.h` & `commoncode-31.2.0/tests/data/resource/samples/zlib/iostream2/zstream.h`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/tests/data/resource/samples/zlib/iostream2/zstream_test.cpp` & `commoncode-31.2.0/tests/data/resource/samples/zlib/iostream2/zstream_test.cpp`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/tests/data/resource/samples/zlib/zlib.h` & `commoncode-31.2.0/tests/data/resource/samples/zlib/zlib.h`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/tests/data/resource/samples/zlib/zutil.c` & `commoncode-31.2.0/tests/data/resource/samples/zlib/zutil.c`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/tests/data/resource/samples/zlib/zutil.h` & `commoncode-31.2.0/tests/data/resource/samples/zlib/zutil.h`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/tests/data/resource/virtual_codebase/codebase-for-cache-tests.json` & `commoncode-31.2.0/tests/data/resource/virtual_codebase/codebase-for-cache-tests.json`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/tests/data/resource/virtual_codebase/combine-expected.json` & `commoncode-31.2.0/tests/data/resource/virtual_codebase/combine-expected.json`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/tests/data/resource/virtual_codebase/combine-shared-directory-name-1.json` & `commoncode-31.2.0/tests/data/resource/virtual_codebase/combine-shared-directory-name-1.json`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/tests/data/resource/virtual_codebase/combine-shared-directory-name-2.json` & `commoncode-31.2.0/tests/data/resource/virtual_codebase/combine-shared-directory-name-2.json`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/tests/data/resource/virtual_codebase/combine-shared-directory-name-expected.json` & `commoncode-31.2.0/tests/data/resource/virtual_codebase/combine-shared-directory-name-expected.json`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/tests/data/resource/virtual_codebase/docker-hello-world.json` & `commoncode-31.2.0/tests/data/resource/virtual_codebase/docker-hello-world.json`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/tests/data/resource/virtual_codebase/et131x.h.json` & `commoncode-31.2.0/tests/data/resource/virtual_codebase/et131x.h.json`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/tests/data/resource/virtual_codebase/fingerprint_attribute.json` & `commoncode-31.2.0/tests/data/resource/virtual_codebase/fingerprint_attribute.json`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/tests/data/resource/virtual_codebase/full-root-info-many-expected.json` & `commoncode-31.2.0/tests/data/resource/virtual_codebase/full-root-info-many-expected.json`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/tests/data/resource/virtual_codebase/full-root-info-many.json` & `commoncode-31.2.0/tests/data/resource/virtual_codebase/full-root-info-many.json`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/tests/data/resource/virtual_codebase/full-root-info-one-expected.json` & `commoncode-31.2.0/tests/data/resource/virtual_codebase/full-root-info-one-expected.json`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/tests/data/resource/virtual_codebase/full-root-info-one.json` & `commoncode-31.2.0/tests/data/resource/virtual_codebase/full-root-info-one.json`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/tests/data/resource/virtual_codebase/lcp.json` & `commoncode-31.2.0/tests/data/resource/virtual_codebase/lcp.json`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/tests/data/resource/virtual_codebase/license-scan.json` & `commoncode-31.2.0/tests/data/resource/virtual_codebase/license-scan.json`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/tests/data/resource/virtual_codebase/node-16-slim.json` & `commoncode-31.2.0/tests/data/resource/virtual_codebase/node-16-slim.json`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/tests/data/resource/virtual_codebase/resource.json` & `commoncode-31.2.0/tests/data/resource/virtual_codebase/resource.json`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/tests/data/resource/virtual_codebase/samples-only-findings-expected.json` & `commoncode-31.2.0/tests/data/resource/virtual_codebase/samples-only-findings-expected.json`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/tests/data/resource/virtual_codebase/samples-only-findings.json` & `commoncode-31.2.0/tests/data/resource/virtual_codebase/samples-only-findings.json`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/tests/data/resource/virtual_codebase/virtual_codebase.json` & `commoncode-31.2.0/tests/data/resource/virtual_codebase/virtual_codebase.json`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/tests/data/resource/virtual_codebase/zephyr-binary.json` & `commoncode-31.2.0/tests/data/resource/virtual_codebase/zephyr-binary.json`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/tests/data/resource/with_path/codebase/et131x.h` & `commoncode-31.2.0/tests/data/resource/with_path/codebase/et131x.h`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/tests/data/resource/with_path/virtual-codebase.json` & `commoncode-31.2.0/tests/data/resource/with_path/virtual-codebase.json`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/tests/data/saneyaml/metadata1` & `commoncode-31.2.0/tests/data/saneyaml/metadata1`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/tests/data/saneyaml/metadata1.notag` & `commoncode-31.2.0/tests/data/saneyaml/metadata1.notag`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/tests/test_cliutils.py` & `commoncode-31.2.0/tests/test_cliutils.py`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/tests/test_cliutils_progressbar.py` & `commoncode-31.2.0/tests/test_cliutils_progressbar.py`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/tests/test_codec.py` & `commoncode-31.2.0/tests/test_codec.py`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/tests/test_command.py` & `commoncode-31.2.0/tests/test_command.py`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/tests/test_date.py` & `commoncode-31.2.0/tests/test_date.py`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/tests/test_fileset.py` & `commoncode-31.2.0/tests/test_fileset.py`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/tests/test_filetype.py` & `commoncode-31.2.0/tests/test_filetype.py`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/tests/test_fileutils.py` & `commoncode-31.2.0/tests/test_fileutils.py`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/tests/test_functional.py` & `commoncode-31.2.0/tests/test_functional.py`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/tests/test_hash.py` & `commoncode-31.2.0/tests/test_hash.py`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/tests/test_ignore.py` & `commoncode-31.2.0/tests/test_ignore.py`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/tests/test_paths.py` & `commoncode-31.2.0/tests/test_paths.py`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/tests/test_resource.py` & `commoncode-31.2.0/tests/test_resource.py`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/tests/test_saneyaml.py` & `commoncode-31.2.0/tests/test_saneyaml.py`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/tests/test_skeleton_codestyle.py` & `commoncode-31.2.0/tests/test_skeleton_codestyle.py`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/tests/test_text.py` & `commoncode-31.2.0/tests/test_text.py`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/tests/test_timeutils.py` & `commoncode-31.2.0/tests/test_timeutils.py`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/tests/test_urn.py` & `commoncode-31.2.0/tests/test_urn.py`

 * *Files identical despite different names*

### Comparing `commoncode-31.1.0/tests/test_version.py` & `commoncode-31.2.0/tests/test_version.py`

 * *Files identical despite different names*

