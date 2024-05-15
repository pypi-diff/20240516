# Comparing `tmp/commoncode-31.0.3.tar.gz` & `tmp/commoncode-31.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "commoncode-31.0.3.tar", last modified: Fri Aug 25 20:43:23 2023, max compression
+gzip compressed data, was "commoncode-31.1.0.tar", last modified: Wed May 15 23:25:54 2024, max compression
```

## Comparing `commoncode-31.0.3.tar` & `commoncode-31.1.0.tar`

### file list

```diff
@@ -1,471 +1,471 @@
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.923959 commoncode-31.0.3/
--rw-r--r--   0 runner    (1001) docker     (998)       89 2023-08-25 20:43:12.000000 commoncode-31.0.3/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.859952 commoncode-31.0.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.875954 commoncode-31.0.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (998)      855 2023-08-25 20:43:12.000000 commoncode-31.0.3/.github/workflows/docs-ci.yml
--rw-r--r--   0 runner    (1001) docker     (998)     2023 2023-08-25 20:43:12.000000 commoncode-31.0.3/.github/workflows/pypi-release.yml
--rw-r--r--   0 runner    (1001) docker     (998)      755 2023-08-25 20:43:12.000000 commoncode-31.0.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (998)      525 2023-08-25 20:43:12.000000 commoncode-31.0.3/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (998)      399 2023-08-25 20:43:12.000000 commoncode-31.0.3/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (998)     8756 2023-08-25 20:43:12.000000 commoncode-31.0.3/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (998)     3422 2023-08-25 20:43:12.000000 commoncode-31.0.3/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (998)      218 2023-08-25 20:43:12.000000 commoncode-31.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (998)     1596 2023-08-25 20:43:12.000000 commoncode-31.0.3/Makefile
--rw-r--r--   0 runner    (1001) docker     (998)      312 2023-08-25 20:43:12.000000 commoncode-31.0.3/NOTICE
--rw-r--r--   0 runner    (1001) docker     (998)     1557 2023-08-25 20:43:23.923959 commoncode-31.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (998)      724 2023-08-25 20:43:12.000000 commoncode-31.0.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (998)    11357 2023-08-25 20:43:12.000000 commoncode-31.0.3/apache-2.0.LICENSE
--rw-r--r--   0 runner    (1001) docker     (998)     4474 2023-08-25 20:43:12.000000 commoncode-31.0.3/azure-pipelines.yml
--rw-r--r--   0 runner    (1001) docker     (998)      567 2023-08-25 20:43:12.000000 commoncode-31.0.3/commoncode.ABOUT
--rwxr-xr-x   0 runner    (1001) docker     (998)     6328 2023-08-25 20:43:12.000000 commoncode-31.0.3/configure
--rw-r--r--   0 runner    (1001) docker     (998)     6948 2023-08-25 20:43:12.000000 commoncode-31.0.3/configure.bat
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.875954 commoncode-31.0.3/docs/
--rw-r--r--   0 runner    (1001) docker     (998)      638 2023-08-25 20:43:12.000000 commoncode-31.0.3/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (998)      799 2023-08-25 20:43:12.000000 commoncode-31.0.3/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.875954 commoncode-31.0.3/docs/scripts/
--rw-r--r--   0 runner    (1001) docker     (998)      131 2023-08-25 20:43:12.000000 commoncode-31.0.3/docs/scripts/doc8_style_check.sh
--rw-r--r--   0 runner    (1001) docker     (998)      124 2023-08-25 20:43:12.000000 commoncode-31.0.3/docs/scripts/sphinx_build_link_check.sh
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.875954 commoncode-31.0.3/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.875954 commoncode-31.0.3/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (998)     8022 2023-08-25 20:43:12.000000 commoncode-31.0.3/docs/source/_static/theme_overrides.css
--rw-r--r--   0 runner    (1001) docker     (998)     3397 2023-08-25 20:43:12.000000 commoncode-31.0.3/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.875954 commoncode-31.0.3/docs/source/contribute/
--rw-r--r--   0 runner    (1001) docker     (998)    10245 2023-08-25 20:43:12.000000 commoncode-31.0.3/docs/source/contribute/contrib_doc.rst
--rw-r--r--   0 runner    (1001) docker     (998)      251 2023-08-25 20:43:12.000000 commoncode-31.0.3/docs/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.859952 commoncode-31.0.3/etc/
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.879954 commoncode-31.0.3/etc/ci/
--rw-r--r--   0 runner    (1001) docker     (998)     1700 2023-08-25 20:43:12.000000 commoncode-31.0.3/etc/ci/azure-container-deb.yml
--rw-r--r--   0 runner    (1001) docker     (998)     1753 2023-08-25 20:43:12.000000 commoncode-31.0.3/etc/ci/azure-container-rpm.yml
--rw-r--r--   0 runner    (1001) docker     (998)     1240 2023-08-25 20:43:12.000000 commoncode-31.0.3/etc/ci/azure-posix.yml
--rw-r--r--   0 runner    (1001) docker     (998)     1215 2023-08-25 20:43:12.000000 commoncode-31.0.3/etc/ci/azure-win.yml
--rw-r--r--   0 runner    (1001) docker     (998)      257 2023-08-25 20:43:12.000000 commoncode-31.0.3/etc/ci/install_sudo.sh
--rw-r--r--   0 runner    (1001) docker     (998)     8365 2023-08-25 20:43:12.000000 commoncode-31.0.3/etc/ci/macports-ci
--rw-r--r--   0 runner    (1001) docker     (998)      684 2023-08-25 20:43:12.000000 commoncode-31.0.3/etc/ci/macports-ci.ABOUT
--rw-r--r--   0 runner    (1001) docker     (998)     1022 2023-08-25 20:43:12.000000 commoncode-31.0.3/etc/ci/mit.LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.879954 commoncode-31.0.3/etc/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (998)     3744 2023-08-25 20:43:12.000000 commoncode-31.0.3/etc/scripts/README.rst
--rw-r--r--   0 runner    (1001) docker     (998)     1301 2023-08-25 20:43:12.000000 commoncode-31.0.3/etc/scripts/check_thirdparty.py
--rw-r--r--   0 runner    (1001) docker     (998)     9486 2023-08-25 20:43:12.000000 commoncode-31.0.3/etc/scripts/fetch_thirdparty.py
--rw-r--r--   0 runner    (1001) docker     (998)     9699 2023-08-25 20:43:12.000000 commoncode-31.0.3/etc/scripts/gen_pypi_simple.py
--rw-r--r--   0 runner    (1001) docker     (998)      354 2023-08-25 20:43:12.000000 commoncode-31.0.3/etc/scripts/gen_pypi_simple.py.ABOUT
--rw-r--r--   0 runner    (1001) docker     (998)     2776 2023-08-25 20:43:12.000000 commoncode-31.0.3/etc/scripts/gen_pypi_simple.py.NOTICE
--rw-r--r--   0 runner    (1001) docker     (998)     1715 2023-08-25 20:43:12.000000 commoncode-31.0.3/etc/scripts/gen_requirements.py
--rw-r--r--   0 runner    (1001) docker     (998)     2266 2023-08-25 20:43:12.000000 commoncode-31.0.3/etc/scripts/gen_requirements_dev.py
--rw-r--r--   0 runner    (1001) docker     (998)      101 2023-08-25 20:43:12.000000 commoncode-31.0.3/etc/scripts/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (998)     4497 2023-08-25 20:43:12.000000 commoncode-31.0.3/etc/scripts/test_utils_pip_compatibility_tags.py
--rw-r--r--   0 runner    (1001) docker     (998)      504 2023-08-25 20:43:12.000000 commoncode-31.0.3/etc/scripts/test_utils_pip_compatibility_tags.py.ABOUT
--rw-r--r--   0 runner    (1001) docker     (998)     2839 2023-08-25 20:43:12.000000 commoncode-31.0.3/etc/scripts/test_utils_pypi_supported_tags.py
--rw-r--r--   0 runner    (1001) docker     (998)      773 2023-08-25 20:43:12.000000 commoncode-31.0.3/etc/scripts/test_utils_pypi_supported_tags.py.ABOUT
--rw-r--r--   0 runner    (1001) docker     (998)     6418 2023-08-25 20:43:12.000000 commoncode-31.0.3/etc/scripts/utils_dejacode.py
--rw-r--r--   0 runner    (1001) docker     (998)     6704 2023-08-25 20:43:12.000000 commoncode-31.0.3/etc/scripts/utils_pip_compatibility_tags.py
--rw-r--r--   0 runner    (1001) docker     (998)      494 2023-08-25 20:43:12.000000 commoncode-31.0.3/etc/scripts/utils_pip_compatibility_tags.py.ABOUT
--rw-r--r--   0 runner    (1001) docker     (998)     2850 2023-08-25 20:43:12.000000 commoncode-31.0.3/etc/scripts/utils_pypi_supported_tags.py
--rw-r--r--   0 runner    (1001) docker     (998)      741 2023-08-25 20:43:12.000000 commoncode-31.0.3/etc/scripts/utils_pypi_supported_tags.py.ABOUT
--rw-r--r--   0 runner    (1001) docker     (998)     6152 2023-08-25 20:43:12.000000 commoncode-31.0.3/etc/scripts/utils_requirements.py
--rw-r--r--   0 runner    (1001) docker     (998)    75931 2023-08-25 20:43:12.000000 commoncode-31.0.3/etc/scripts/utils_thirdparty.py
--rw-r--r--   0 runner    (1001) docker     (998)      608 2023-08-25 20:43:12.000000 commoncode-31.0.3/etc/scripts/utils_thirdparty.py.ABOUT
--rw-r--r--   0 runner    (1001) docker     (998)      857 2023-08-25 20:43:12.000000 commoncode-31.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (998)      767 2023-08-25 20:43:12.000000 commoncode-31.0.3/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (998)      245 2023-08-25 20:43:12.000000 commoncode-31.0.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (998)     1302 2023-08-25 20:43:23.923959 commoncode-31.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (998)       92 2023-08-25 20:43:12.000000 commoncode-31.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.859952 commoncode-31.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.883955 commoncode-31.0.3/src/commoncode/
--rw-r--r--   0 runner    (1001) docker     (998)      916 2023-08-25 20:43:12.000000 commoncode-31.0.3/src/commoncode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (998)     3999 2023-08-25 20:43:12.000000 commoncode-31.0.3/src/commoncode/archive.py
--rw-r--r--   0 runner    (1001) docker     (998)    19600 2023-08-25 20:43:12.000000 commoncode-31.0.3/src/commoncode/cliutils.py
--rw-r--r--   0 runner    (1001) docker     (998)     1581 2023-08-25 20:43:12.000000 commoncode-31.0.3/src/commoncode/codec.py
--rw-r--r--   0 runner    (1001) docker     (998)     9516 2023-08-25 20:43:12.000000 commoncode-31.0.3/src/commoncode/command.py
--rw-r--r--   0 runner    (1001) docker     (998)      381 2023-08-25 20:43:12.000000 commoncode-31.0.3/src/commoncode/compat.py
--rw-r--r--   0 runner    (1001) docker     (998)     5480 2023-08-25 20:43:12.000000 commoncode-31.0.3/src/commoncode/datautils.py
--rw-r--r--   0 runner    (1001) docker     (998)     1221 2023-08-25 20:43:12.000000 commoncode-31.0.3/src/commoncode/date.py
--rw-r--r--   0 runner    (1001) docker     (998)      346 2023-08-25 20:43:12.000000 commoncode-31.0.3/src/commoncode/dict_utils.ABOUT
--rw-r--r--   0 runner    (1001) docker     (998)      779 2023-08-25 20:43:12.000000 commoncode-31.0.3/src/commoncode/dict_utils.py
--rw-r--r--   0 runner    (1001) docker     (998)     2148 2023-08-25 20:43:12.000000 commoncode-31.0.3/src/commoncode/fetch.py
--rw-r--r--   0 runner    (1001) docker     (998)     6487 2023-08-25 20:43:12.000000 commoncode-31.0.3/src/commoncode/fileset.py
--rw-r--r--   0 runner    (1001) docker     (998)     6660 2023-08-25 20:43:12.000000 commoncode-31.0.3/src/commoncode/filetype.py
--rw-r--r--   0 runner    (1001) docker     (998)    17123 2023-08-25 20:43:12.000000 commoncode-31.0.3/src/commoncode/fileutils.py
--rw-r--r--   0 runner    (1001) docker     (998)      554 2023-08-25 20:43:12.000000 commoncode-31.0.3/src/commoncode/fileutils.py.ABOUT
--rw-r--r--   0 runner    (1001) docker     (998)     3325 2023-08-25 20:43:12.000000 commoncode-31.0.3/src/commoncode/functional.py
--rw-r--r--   0 runner    (1001) docker     (998)     4967 2023-08-25 20:43:12.000000 commoncode-31.0.3/src/commoncode/hash.py
--rw-r--r--   0 runner    (1001) docker     (998)    11645 2023-08-25 20:43:12.000000 commoncode-31.0.3/src/commoncode/ignore.py
--rw-r--r--   0 runner    (1001) docker     (998)     9167 2023-08-25 20:43:12.000000 commoncode-31.0.3/src/commoncode/paths.py
--rw-r--r--   0 runner    (1001) docker     (998)    32426 2023-08-25 20:43:12.000000 commoncode-31.0.3/src/commoncode/python.LICENSE
--rw-r--r--   0 runner    (1001) docker     (998)    73970 2023-08-25 20:43:12.000000 commoncode-31.0.3/src/commoncode/resource.py
--rw-r--r--   0 runner    (1001) docker     (998)     3699 2023-08-25 20:43:12.000000 commoncode-31.0.3/src/commoncode/system.py
--rw-r--r--   0 runner    (1001) docker     (998)    14225 2023-08-25 20:43:12.000000 commoncode-31.0.3/src/commoncode/testcase.py
--rw-r--r--   0 runner    (1001) docker     (998)     4163 2023-08-25 20:43:12.000000 commoncode-31.0.3/src/commoncode/text.py
--rw-r--r--   0 runner    (1001) docker     (998)     3692 2023-08-25 20:43:12.000000 commoncode-31.0.3/src/commoncode/timeutils.py
--rw-r--r--   0 runner    (1001) docker     (998)     4551 2023-08-25 20:43:12.000000 commoncode-31.0.3/src/commoncode/urn.py
--rw-r--r--   0 runner    (1001) docker     (998)     9995 2023-08-25 20:43:12.000000 commoncode-31.0.3/src/commoncode/version.py
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.887955 commoncode-31.0.3/src/commoncode.egg-info/
--rw-r--r--   0 runner    (1001) docker     (998)     1557 2023-08-25 20:43:23.000000 commoncode-31.0.3/src/commoncode.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (998)    14540 2023-08-25 20:43:23.000000 commoncode-31.0.3/src/commoncode.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (998)        1 2023-08-25 20:43:23.000000 commoncode-31.0.3/src/commoncode.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (998)        1 2023-08-25 20:43:23.000000 commoncode-31.0.3/src/commoncode.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (998)      304 2023-08-25 20:43:23.000000 commoncode-31.0.3/src/commoncode.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (998)       11 2023-08-25 20:43:23.000000 commoncode-31.0.3/src/commoncode.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.887955 commoncode-31.0.3/tests/
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.871954 commoncode-31.0.3/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.859952 commoncode-31.0.3/tests/data/count/
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.859952 commoncode-31.0.3/tests/data/count/filecount/
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.891955 commoncode-31.0.3/tests/data/count/filecount/dir/
--rw-r--r--   0 runner    (1001) docker     (998)        2 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/count/filecount/dir/a.txt
--rw-r--r--   0 runner    (1001) docker     (998)        2 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/count/filecount/dir/b.txt
--rw-r--r--   0 runner    (1001) docker     (998)        2 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/count/filecount/dir/c.txt
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.891955 commoncode-31.0.3/tests/data/count/filecount/dir/sub1/
--rw-r--r--   0 runner    (1001) docker     (998)        2 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/count/filecount/dir/sub1/a.txt
--rw-r--r--   0 runner    (1001) docker     (998)        2 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/count/filecount/dir/sub1/b.txt
--rw-r--r--   0 runner    (1001) docker     (998)        2 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/count/filecount/dir/sub1/c.txt
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.891955 commoncode-31.0.3/tests/data/count/filecount/dir/sub1/subsub/
--rw-r--r--   0 runner    (1001) docker     (998)        2 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/count/filecount/dir/sub1/subsub/a.txt
--rw-r--r--   0 runner    (1001) docker     (998)        2 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/count/filecount/dir/sub1/subsub/b.txt
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.891955 commoncode-31.0.3/tests/data/count/filecount/dir/sub2/
--rw-r--r--   0 runner    (1001) docker     (998)        2 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/count/filecount/dir/sub2/a.txt
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.891955 commoncode-31.0.3/tests/data/date/
--rw-r--r--   0 runner    (1001) docker     (998)      596 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/date/ant-jsch-1.7.0.tar.gz
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.891955 commoncode-31.0.3/tests/data/date/dir/
--rw-r--r--   0 runner    (1001) docker     (998)        2 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/date/dir/a.txt
--rw-r--r--   0 runner    (1001) docker     (998)        2 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/date/dir/b.txt
--rw-r--r--   0 runner    (1001) docker     (998)        2 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/date/dir/c.txt
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.891955 commoncode-31.0.3/tests/data/date/dir/sub1/
--rw-r--r--   0 runner    (1001) docker     (998)        2 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/date/dir/sub1/a.txt
--rw-r--r--   0 runner    (1001) docker     (998)        2 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/date/dir/sub1/b.txt
--rw-r--r--   0 runner    (1001) docker     (998)        2 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/date/dir/sub1/c.txt
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.891955 commoncode-31.0.3/tests/data/date/dir/sub1/subsub/
--rw-r--r--   0 runner    (1001) docker     (998)        2 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/date/dir/sub1/subsub/a.txt
--rw-r--r--   0 runner    (1001) docker     (998)        2 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/date/dir/sub1/subsub/b.txt
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.891955 commoncode-31.0.3/tests/data/date/dir/sub2/
--rw-r--r--   0 runner    (1001) docker     (998)        2 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/date/dir/sub2/a.txt
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.891955 commoncode-31.0.3/tests/data/fileset/
--rw-r--r--   0 runner    (1001) docker     (998)       33 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/fileset/scancodeignore.lst
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.891955 commoncode-31.0.3/tests/data/filetype/
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.863953 commoncode-31.0.3/tests/data/filetype/readwrite/
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.891955 commoncode-31.0.3/tests/data/filetype/readwrite/sub/
--rw-r--r--   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/filetype/readwrite/sub/file
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.891955 commoncode-31.0.3/tests/data/filetype/size/
--rw-r--r--   0 runner    (1001) docker     (998)    12388 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/filetype/size/Image1.eps
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.891955 commoncode-31.0.3/tests/data/filetype/size/exec/
--rw-r--r--   0 runner    (1001) docker     (998)        2 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/filetype/size/exec/1.txt
--rw-r--r--   0 runner    (1001) docker     (998)        2 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/filetype/size/exec/a.bat
--rw-r--r--   0 runner    (1001) docker     (998)        2 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/filetype/size/exec/a.tar
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.891955 commoncode-31.0.3/tests/data/filetype/size/exec/subtxt/
--rw-r--r--   0 runner    (1001) docker     (998)        2 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/filetype/size/exec/subtxt/1.txt
--rw-r--r--   0 runner    (1001) docker     (998)        2 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/filetype/size/exec/subtxt/a.txt
--rw-r--r--   0 runner    (1001) docker     (998)        2 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/filetype/size/exec/subtxt/b.txt
--rw-r--r--   0 runner    (1001) docker     (998)   109056 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/filetype/types.tar
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.863953 commoncode-31.0.3/tests/data/fileutils/
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.895956 commoncode-31.0.3/tests/data/fileutils/basename/
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.895956 commoncode-31.0.3/tests/data/fileutils/basename/a/
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.895956 commoncode-31.0.3/tests/data/fileutils/basename/a/.a/
--rw-r--r--   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/fileutils/basename/a/.a/file
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.895956 commoncode-31.0.3/tests/data/fileutils/basename/a/b/
--rw-r--r--   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/fileutils/basename/a/b/.a
--rw-r--r--   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/fileutils/basename/a/b/.a.b
--rw-r--r--   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/fileutils/basename/a/b/a.tag.gz
--rw-r--r--   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/fileutils/basename/a/f.a
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.895956 commoncode-31.0.3/tests/data/fileutils/basename/f.a/
--rw-r--r--   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/fileutils/basename/f.a/a.c
--rw-r--r--   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/fileutils/basename/tst
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.895956 commoncode-31.0.3/tests/data/fileutils/exec/
--rw-r--r--   0 runner    (1001) docker     (998)        2 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/fileutils/exec/1.txt
--rw-r--r--   0 runner    (1001) docker     (998)        2 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/fileutils/exec/a.bat
--rw-r--r--   0 runner    (1001) docker     (998)        2 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/fileutils/exec/a.tar
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.895956 commoncode-31.0.3/tests/data/fileutils/exec/subtxt/
--rw-r--r--   0 runner    (1001) docker     (998)        2 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/fileutils/exec/subtxt/1.txt
--rw-r--r--   0 runner    (1001) docker     (998)        2 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/fileutils/exec/subtxt/a.txt
--rw-r--r--   0 runner    (1001) docker     (998)        2 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/fileutils/exec/subtxt/b.txt
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.863953 commoncode-31.0.3/tests/data/fileutils/executable/
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.863953 commoncode-31.0.3/tests/data/fileutils/executable/deep1/
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.895956 commoncode-31.0.3/tests/data/fileutils/executable/deep1/deep2/
--rw-r--r--   0 runner    (1001) docker     (998)       73 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/fileutils/executable/deep1/deep2/ctags
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.895956 commoncode-31.0.3/tests/data/fileutils/filetype/
--rw-r--r--   0 runner    (1001) docker     (998)      147 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/fileutils/filetype/a.html
--rw-r--r--   0 runner    (1001) docker     (998)      512 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/fileutils/filetype/stage1
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.895956 commoncode-31.0.3/tests/data/fileutils/perms/
--rw-r--r--   0 runner    (1001) docker     (998)      195 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/fileutils/perms/unreadable.tgz
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.863953 commoncode-31.0.3/tests/data/fileutils/readwrite/
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.895956 commoncode-31.0.3/tests/data/fileutils/readwrite/sub/
--rw-r--r--   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/fileutils/readwrite/sub/file
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.895956 commoncode-31.0.3/tests/data/fileutils/walk/
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.895956 commoncode-31.0.3/tests/data/fileutils/walk/d1/
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.895956 commoncode-31.0.3/tests/data/fileutils/walk/d1/d2/
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.895956 commoncode-31.0.3/tests/data/fileutils/walk/d1/d2/d3/
--rw-r--r--   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/fileutils/walk/d1/d2/d3/f3
--rw-r--r--   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/fileutils/walk/d1/d2/f2
--rw-r--r--   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/fileutils/walk/d1/f1
--rw-r--r--   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/fileutils/walk/f
--rw-r--r--   0 runner    (1001) docker     (998)     1136 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/fileutils/walk/unicode.zip
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.895956 commoncode-31.0.3/tests/data/fileutils/walk_non_utf8/
--rw-r--r--   0 runner    (1001) docker     (998)      506 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/fileutils/walk_non_utf8/non_unicode.tgz
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.863953 commoncode-31.0.3/tests/data/hash/
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.895956 commoncode-31.0.3/tests/data/hash/dir1/
--rw-r--r--   0 runner    (1001) docker     (998)     7859 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/hash/dir1/a.png
--rw-r--r--   0 runner    (1001) docker     (998)        6 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/hash/dir1/a.txt
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.895956 commoncode-31.0.3/tests/data/hash/dir2/
--rw-r--r--   0 runner    (1001) docker     (998)        6 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/hash/dir2/a.txt
--rw-r--r--   0 runner    (1001) docker     (998)       21 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/hash/dir2/dos.txt
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.899956 commoncode-31.0.3/tests/data/hash/sha1-collision/
--rw-r--r--   0 runner    (1001) docker     (998)   422435 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/hash/sha1-collision/shattered-1.pdf
--rw-r--r--   0 runner    (1001) docker     (998)      158 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/hash/sha1-collision/shattered-1.pdf.ABOUT
--rw-r--r--   0 runner    (1001) docker     (998)   422435 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/hash/sha1-collision/shattered-2.pdf
--rw-r--r--   0 runner    (1001) docker     (998)      158 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/hash/sha1-collision/shattered-2.pdf.ABOUT
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.899956 commoncode-31.0.3/tests/data/ignore/
--rw-r--r--   0 runner    (1001) docker     (998)       33 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/ignore/.scancodeignore
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.899956 commoncode-31.0.3/tests/data/ignore/excludes/
--rw-r--r--   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/ignore/excludes/.localized
--rw-r--r--   0 runner    (1001) docker     (998)      225 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/ignore/excludes/eclipse.tgz
--rw-r--r--   0 runner    (1001) docker     (998)      409 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/ignore/excludes/mac.tgz
--rw-r--r--   0 runner    (1001) docker     (998)      163 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/ignore/excludes/msft-vs.tgz
--rw-r--r--   0 runner    (1001) docker     (998)     6296 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/ignore/vcs.tgz
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.871954 commoncode-31.0.3/tests/data/resource/
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.863953 commoncode-31.0.3/tests/data/resource/cache/
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.899956 commoncode-31.0.3/tests/data/resource/cache/package/
--rw-r--r--   0 runner    (1001) docker     (998)     2361 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/cache/package/package.json
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.899956 commoncode-31.0.3/tests/data/resource/cache2/
--rw-r--r--   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/cache2/abc
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.899956 commoncode-31.0.3/tests/data/resource/cache2/dir/
--rw-r--r--   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/cache2/dir/that
--rw-r--r--   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/cache2/dir/this
--rw-r--r--   0 runner    (1001) docker     (998)     2228 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/cache2/et131x.h
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.899956 commoncode-31.0.3/tests/data/resource/cache2/other dir/
--rw-r--r--   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/cache2/other dir/file
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.867953 commoncode-31.0.3/tests/data/resource/client/
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.899956 commoncode-31.0.3/tests/data/resource/client/Images/
--rw-r--r--   0 runner    (1001) docker     (998)        1 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/client/Images/applicationCache.png
--rw-r--r--   0 runner    (1001) docker     (998)        1 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/client/Images/spinner.gif
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.899956 commoncode-31.0.3/tests/data/resource/codebase/
--rw-r--r--   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/codebase/abc
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.899956 commoncode-31.0.3/tests/data/resource/codebase/dir/
--rw-r--r--   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/codebase/dir/that
--rw-r--r--   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/codebase/dir/this
--rw-r--r--   0 runner    (1001) docker     (998)     2228 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/codebase/et131x.h
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.903957 commoncode-31.0.3/tests/data/resource/codebase/other dir/
--rw-r--r--   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/codebase/other dir/file
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.903957 commoncode-31.0.3/tests/data/resource/deeply_nested/
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.903957 commoncode-31.0.3/tests/data/resource/deeply_nested/level1_dir1/
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.903957 commoncode-31.0.3/tests/data/resource/deeply_nested/level1_dir1/level2_dir1/
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.903957 commoncode-31.0.3/tests/data/resource/deeply_nested/level1_dir1/level2_dir1/level3_dir1/
--rw-r--r--   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/deeply_nested/level1_dir1/level2_dir1/level3_dir1/level4_file1
--rw-r--r--   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/deeply_nested/level1_dir1/level2_dir1/level3_file1
--rw-r--r--   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/deeply_nested/level1_dir1/level2_dir1/level3_file2
--rw-r--r--   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/deeply_nested/level1_dir1/level2_file1
--rw-r--r--   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/deeply_nested/level1_dir1/level2_file2
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.903957 commoncode-31.0.3/tests/data/resource/deeply_nested/level1_dir2/
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.903957 commoncode-31.0.3/tests/data/resource/deeply_nested/level1_dir2/level2_dir3/
--rw-r--r--   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/deeply_nested/level1_dir2/level2_dir3/level3_file3
--rw-r--r--   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/deeply_nested/level1_dir2/level2_dir3/level3_file4
--rw-r--r--   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/deeply_nested/level1_dir2/level2_file3
--rw-r--r--   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/deeply_nested/level1_dir2/level2_file4
--rw-r--r--   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/deeply_nested/level1_dir2/level2_file5
--rw-r--r--   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/deeply_nested/level1_file1
--rw-r--r--   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/deeply_nested/level1_file2
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.867953 commoncode-31.0.3/tests/data/resource/dist/
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.903957 commoncode-31.0.3/tests/data/resource/dist/JGroups/
--rw-r--r--   0 runner    (1001) docker     (998)        1 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/dist/JGroups/EULA
--rw-r--r--   0 runner    (1001) docker     (998)        1 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/dist/JGroups/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.903957 commoncode-31.0.3/tests/data/resource/dist/JGroups/src/
--rw-r--r--   0 runner    (1001) docker     (998)        1 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/dist/JGroups/src/RouterStub.java
--rw-r--r--   0 runner    (1001) docker     (998)        1 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/dist/JGroups/src/RouterStubManager.java
--rw-r--r--   0 runner    (1001) docker     (998)        1 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/dist/JGroups/src/S3_PING.java
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.867953 commoncode-31.0.3/tests/data/resource/dist/simple/
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.903957 commoncode-31.0.3/tests/data/resource/dist/simple/META-INF/
--rw-r--r--   0 runner    (1001) docker     (998)        1 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/dist/simple/META-INF/MANIFEST.MF
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.903957 commoncode-31.0.3/tests/data/resource/ignore/
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.903957 commoncode-31.0.3/tests/data/resource/ignore/cvs/
--rw-r--r--   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/ignore/cvs/file2
--rw-r--r--   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/ignore/file1
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.867953 commoncode-31.0.3/tests/data/resource/lcp/
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.903957 commoncode-31.0.3/tests/data/resource/lcp/test1/
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.903957 commoncode-31.0.3/tests/data/resource/lcp/test1/JGroups/
--rw-r--r--   0 runner    (1001) docker     (998)        1 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/lcp/test1/JGroups/EULA
--rw-r--r--   0 runner    (1001) docker     (998)        1 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/lcp/test1/JGroups/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.903957 commoncode-31.0.3/tests/data/resource/lcp/test1/JGroups/licenses/
--rw-r--r--   0 runner    (1001) docker     (998)        1 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/lcp/test1/JGroups/licenses/apache-1.1.txt
--rw-r--r--   0 runner    (1001) docker     (998)        1 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/lcp/test1/JGroups/licenses/lgpl.txt
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.903957 commoncode-31.0.3/tests/data/resource/lcp/test1/JGroups/src/
--rw-r--r--   0 runner    (1001) docker     (998)        1 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/lcp/test1/JGroups/src/RouterStub.java
--rw-r--r--   0 runner    (1001) docker     (998)        1 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/lcp/test1/JGroups/src/RouterStubManager.java
--rw-r--r--   0 runner    (1001) docker     (998)        1 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/lcp/test1/JGroups/src/S3_PING.java
--rw-r--r--   0 runner    (1001) docker     (998)        1 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/lcp/test1/screenshot.png
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.867953 commoncode-31.0.3/tests/data/resource/lcp/test1/simple/
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.907957 commoncode-31.0.3/tests/data/resource/lcp/test1/simple/META-INF/
--rw-r--r--   0 runner    (1001) docker     (998)        1 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/lcp/test1/simple/META-INF/MANIFEST.MF
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.867953 commoncode-31.0.3/tests/data/resource/lcp/test1/simple/org/
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.867953 commoncode-31.0.3/tests/data/resource/lcp/test1/simple/org/jvnet/
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.867953 commoncode-31.0.3/tests/data/resource/lcp/test1/simple/org/jvnet/glassfish/
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.867953 commoncode-31.0.3/tests/data/resource/lcp/test1/simple/org/jvnet/glassfish/comms/
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.907957 commoncode-31.0.3/tests/data/resource/lcp/test1/simple/org/jvnet/glassfish/comms/sipagent/
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.907957 commoncode-31.0.3/tests/data/resource/lcp/test1/simple/org/jvnet/glassfish/comms/sipagent/actions/
--rw-r--r--   0 runner    (1001) docker     (998)        1 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/lcp/test1/simple/org/jvnet/glassfish/comms/sipagent/actions/Bundle.properties
--rw-r--r--   0 runner    (1001) docker     (998)        1 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/lcp/test1/simple/org/jvnet/glassfish/comms/sipagent/actions/SipAgentCookieAction.class
--rw-r--r--   0 runner    (1001) docker     (998)        1 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/lcp/test1/simple/org/jvnet/glassfish/comms/sipagent/actions/bd.png
--rw-r--r--   0 runner    (1001) docker     (998)        1 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/lcp/test1/simple/org/jvnet/glassfish/comms/sipagent/actions/bd24.png
--rw-r--r--   0 runner    (1001) docker     (998)        1 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/lcp/test1/simple/org/jvnet/glassfish/comms/sipagent/org-jvnet-glassfish-comms-sipagent-actions-SipAgentCookieAction.instance
--rw-r--r--   0 runner    (1001) docker     (998)        1 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/lcp/test1/simple/org/jvnet/glassfish/comms/sipagent/org-jvnet-glassfish-comms-sipagent-actions-SipAgentCookieAction_1.instance
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.867953 commoncode-31.0.3/tests/data/resource/lcp/test1/zlib/
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.907957 commoncode-31.0.3/tests/data/resource/lcp/test1/zlib/ada/
--rw-r--r--   0 runner    (1001) docker     (998)        1 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/lcp/test1/zlib/ada/zlib.ads
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.871954 commoncode-31.0.3/tests/data/resource/lcp/test1/zlib/inter/
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.907957 commoncode-31.0.3/tests/data/resource/lcp/test1/zlib/inter/arch/
--rw-r--r--   0 runner    (1001) docker     (998)        1 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/lcp/test1/zlib/inter/arch/zlib.tar.gz
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.907957 commoncode-31.0.3/tests/data/resource/lcp/test1/zlib/inter/dir/
--rw-r--r--   0 runner    (1001) docker     (998)        1 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/lcp/test1/zlib/inter/dir/EULA
--rw-r--r--   0 runner    (1001) docker     (998)        1 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/lcp/test1/zlib/inter/dir/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.907957 commoncode-31.0.3/tests/data/resource/lcp/test1/zlib/inter/dir/licenses/
--rw-r--r--   0 runner    (1001) docker     (998)        1 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/lcp/test1/zlib/inter/dir/licenses/apache-1.1.txt
--rw-r--r--   0 runner    (1001) docker     (998)        1 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/lcp/test1/zlib/inter/dir/licenses/apache-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (998)        1 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/lcp/test1/zlib/inter/dir/licenses/bouncycastle.txt
--rw-r--r--   0 runner    (1001) docker     (998)        1 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/lcp/test1/zlib/inter/dir/licenses/cpl-1.0.txt
--rw-r--r--   0 runner    (1001) docker     (998)        1 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/lcp/test1/zlib/inter/dir/licenses/lgpl.txt
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.907957 commoncode-31.0.3/tests/data/resource/lcp/test1/zlib/inter/dir/src/
--rw-r--r--   0 runner    (1001) docker     (998)        1 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/lcp/test1/zlib/inter/dir/src/FixedMembershipToken.java
--rw-r--r--   0 runner    (1001) docker     (998)        1 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/lcp/test1/zlib/inter/dir/src/GuardedBy.java
--rw-r--r--   0 runner    (1001) docker     (998)        1 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/lcp/test1/zlib/inter/dir/src/ImmutableReference.java
--rw-r--r--   0 runner    (1001) docker     (998)        1 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/lcp/test1/zlib/inter/dir/src/RATE_LIMITER.java
--rw-r--r--   0 runner    (1001) docker     (998)        1 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/lcp/test1/zlib/inter/dir/src/RouterStub.java
--rw-r--r--   0 runner    (1001) docker     (998)        1 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/lcp/test1/zlib/inter/dir/src/RouterStubManager.java
--rw-r--r--   0 runner    (1001) docker     (998)        1 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/lcp/test1/zlib/inter/dir/src/S3_PING.java
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.907957 commoncode-31.0.3/tests/data/resource/lcp/test1/zlib/inter/iostream2/
--rw-r--r--   0 runner    (1001) docker     (998)        1 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/lcp/test1/zlib/inter/iostream2/zstream.h
--rw-r--r--   0 runner    (1001) docker     (998)        1 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/lcp/test1/zlib/inter/iostream2/zstream_test.cpp
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.911958 commoncode-31.0.3/tests/data/resource/lcp/test1/zlib/inter/zlib/
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.911958 commoncode-31.0.3/tests/data/resource/lcp/test1/zlib/inter/zlib/ada/
--rw-r--r--   0 runner    (1001) docker     (998)        1 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/lcp/test1/zlib/inter/zlib/ada/zlib.ads
--rw-r--r--   0 runner    (1001) docker     (998)        1 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/lcp/test1/zlib/inter/zlib/adler32.c
--rw-r--r--   0 runner    (1001) docker     (998)        1 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/lcp/test1/zlib/inter/zlib/deflate.c
--rw-r--r--   0 runner    (1001) docker     (998)        1 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/lcp/test1/zlib/inter/zlib/deflate.h
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.911958 commoncode-31.0.3/tests/data/resource/lcp/test1/zlib/inter/zlib/dotzlib/
--rw-r--r--   0 runner    (1001) docker     (998)        1 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/lcp/test1/zlib/inter/zlib/dotzlib/AssemblyInfo.cs
--rw-r--r--   0 runner    (1001) docker     (998)        1 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/lcp/test1/zlib/inter/zlib/dotzlib/ChecksumImpl.cs
--rw-r--r--   0 runner    (1001) docker     (998)        1 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/lcp/test1/zlib/inter/zlib/dotzlib/LICENSE_1_0.txt
--rw-r--r--   0 runner    (1001) docker     (998)        1 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/lcp/test1/zlib/inter/zlib/dotzlib/readme.txt
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.911958 commoncode-31.0.3/tests/data/resource/lcp/test1/zlib/inter/zlib/gcc_gvmat64/
--rw-r--r--   0 runner    (1001) docker     (998)        1 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/lcp/test1/zlib/inter/zlib/gcc_gvmat64/gvmat64.S
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.911958 commoncode-31.0.3/tests/data/resource/lcp/test1/zlib/inter/zlib/infback9/
--rw-r--r--   0 runner    (1001) docker     (998)        1 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/lcp/test1/zlib/inter/zlib/infback9/infback9.c
--rw-r--r--   0 runner    (1001) docker     (998)        1 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/lcp/test1/zlib/inter/zlib/infback9/infback9.h
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.911958 commoncode-31.0.3/tests/data/resource/lcp/test1/zlib/inter/zlib/iostream2/
--rw-r--r--   0 runner    (1001) docker     (998)        1 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/lcp/test1/zlib/inter/zlib/iostream2/zstream.h
--rw-r--r--   0 runner    (1001) docker     (998)        1 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/lcp/test1/zlib/inter/zlib/iostream2/zstream_test.cpp
--rw-r--r--   0 runner    (1001) docker     (998)        1 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/lcp/test1/zlib/inter/zlib/zlib.h
--rw-r--r--   0 runner    (1001) docker     (998)        1 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/lcp/test1/zlib/inter/zlib/zutil.c
--rw-r--r--   0 runner    (1001) docker     (998)        1 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/lcp/test1/zlib/inter/zlib/zutil.h
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.911958 commoncode-31.0.3/tests/data/resource/resource/
--rw-r--r--   0 runner    (1001) docker     (998)     7194 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/resource/test-extracted-from-to.json
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.911958 commoncode-31.0.3/tests/data/resource/samples/
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.911958 commoncode-31.0.3/tests/data/resource/samples/JGroups/
--rw-r--r--   0 runner    (1001) docker     (998)     8156 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/samples/JGroups/EULA
--rw-r--r--   0 runner    (1001) docker     (998)    26430 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/samples/JGroups/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.915958 commoncode-31.0.3/tests/data/resource/samples/JGroups/licenses/
--rw-r--r--   0 runner    (1001) docker     (998)     2885 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/samples/JGroups/licenses/apache-1.1.txt
--rw-r--r--   0 runner    (1001) docker     (998)    11560 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/samples/JGroups/licenses/apache-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (998)     1186 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/samples/JGroups/licenses/bouncycastle.txt
--rw-r--r--   0 runner    (1001) docker     (998)    11987 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/samples/JGroups/licenses/cpl-1.0.txt
--rw-r--r--   0 runner    (1001) docker     (998)    26934 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/samples/JGroups/licenses/lgpl.txt
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.915958 commoncode-31.0.3/tests/data/resource/samples/JGroups/src/
--rw-r--r--   0 runner    (1001) docker     (998)     5144 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/samples/JGroups/src/FixedMembershipToken.java
--rw-r--r--   0 runner    (1001) docker     (998)      813 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/samples/JGroups/src/GuardedBy.java
--rw-r--r--   0 runner    (1001) docker     (998)     1838 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/samples/JGroups/src/ImmutableReference.java
--rw-r--r--   0 runner    (1001) docker     (998)     3692 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/samples/JGroups/src/RATE_LIMITER.java
--rw-r--r--   0 runner    (1001) docker     (998)     9913 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/samples/JGroups/src/RouterStub.java
--rw-r--r--   0 runner    (1001) docker     (998)     8162 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/samples/JGroups/src/RouterStubManager.java
--rw-r--r--   0 runner    (1001) docker     (998)   122528 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/samples/JGroups/src/S3_PING.java
--rw-r--r--   0 runner    (1001) docker     (998)      236 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/samples/README
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.915958 commoncode-31.0.3/tests/data/resource/samples/arch/
--rw-r--r--   0 runner    (1001) docker     (998)    28103 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/samples/arch/zlib.tar.gz
--rw-r--r--   0 runner    (1001) docker     (998)   622754 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/samples/screenshot.png
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.915958 commoncode-31.0.3/tests/data/resource/samples/zlib/
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.915958 commoncode-31.0.3/tests/data/resource/samples/zlib/ada/
--rw-r--r--   0 runner    (1001) docker     (998)    13594 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/samples/zlib/ada/zlib.ads
--rw-r--r--   0 runner    (1001) docker     (998)     4968 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/samples/zlib/adler32.c
--rw-r--r--   0 runner    (1001) docker     (998)    71476 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/samples/zlib/deflate.c
--rw-r--r--   0 runner    (1001) docker     (998)    12774 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/samples/zlib/deflate.h
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.915958 commoncode-31.0.3/tests/data/resource/samples/zlib/dotzlib/
--rw-r--r--   0 runner    (1001) docker     (998)     2500 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/samples/zlib/dotzlib/AssemblyInfo.cs
--rw-r--r--   0 runner    (1001) docker     (998)     8040 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/samples/zlib/dotzlib/ChecksumImpl.cs
--rw-r--r--   0 runner    (1001) docker     (998)     1359 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/samples/zlib/dotzlib/LICENSE_1_0.txt
--rw-r--r--   0 runner    (1001) docker     (998)     2358 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/samples/zlib/dotzlib/readme.txt
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.915958 commoncode-31.0.3/tests/data/resource/samples/zlib/gcc_gvmat64/
--rw-r--r--   0 runner    (1001) docker     (998)    16413 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/samples/zlib/gcc_gvmat64/gvmat64.S
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.915958 commoncode-31.0.3/tests/data/resource/samples/zlib/infback9/
--rw-r--r--   0 runner    (1001) docker     (998)    21629 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/samples/zlib/infback9/infback9.c
--rw-r--r--   0 runner    (1001) docker     (998)     1594 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/samples/zlib/infback9/infback9.h
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.919958 commoncode-31.0.3/tests/data/resource/samples/zlib/iostream2/
--rw-r--r--   0 runner    (1001) docker     (998)     9283 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/samples/zlib/iostream2/zstream.h
--rw-r--r--   0 runner    (1001) docker     (998)      711 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/samples/zlib/iostream2/zstream_test.cpp
--rw-r--r--   0 runner    (1001) docker     (998)    87883 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/samples/zlib/zlib.h
--rw-r--r--   0 runner    (1001) docker     (998)     7414 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/samples/zlib/zutil.c
--rw-r--r--   0 runner    (1001) docker     (998)     6766 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/samples/zlib/zutil.h
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.919958 commoncode-31.0.3/tests/data/resource/skip_directories_during_walk/
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.919958 commoncode-31.0.3/tests/data/resource/skip_directories_during_walk/skip-this-directory/
--rw-r--r--   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/skip_directories_during_walk/skip-this-directory/this-should-not-be-returned
--rw-r--r--   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/skip_directories_during_walk/this-should-be-returned
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.923959 commoncode-31.0.3/tests/data/resource/virtual_codebase/
--rw-r--r--   0 runner    (1001) docker     (998)     4628 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/virtual_codebase/codebase-for-cache-tests.json
--rw-r--r--   0 runner    (1001) docker     (998)      212 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/virtual_codebase/combine-1.json
--rw-r--r--   0 runner    (1001) docker     (998)      223 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/virtual_codebase/combine-2.json
--rw-r--r--   0 runner    (1001) docker     (998)      836 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/virtual_codebase/combine-expected.json
--rw-r--r--   0 runner    (1001) docker     (998)     1596 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/virtual_codebase/combine-shared-directory-name-1.json
--rw-r--r--   0 runner    (1001) docker     (998)     1598 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/virtual_codebase/combine-shared-directory-name-2.json
--rw-r--r--   0 runner    (1001) docker     (998)      699 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/virtual_codebase/combine-shared-directory-name-expected.json
--rw-r--r--   0 runner    (1001) docker     (998)     5129 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/virtual_codebase/docker-hello-world.json
--rw-r--r--   0 runner    (1001) docker     (998)      670 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/virtual_codebase/et131x.h.json
--rw-r--r--   0 runner    (1001) docker     (998)      714 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/virtual_codebase/fingerprint_attribute.json
--rw-r--r--   0 runner    (1001) docker     (998)      468 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/virtual_codebase/from_file.json
--rw-r--r--   0 runner    (1001) docker     (998)    17547 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/virtual_codebase/full-root-info-many-expected.json
--rw-r--r--   0 runner    (1001) docker     (998)    16812 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/virtual_codebase/full-root-info-many.json
--rw-r--r--   0 runner    (1001) docker     (998)      711 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/virtual_codebase/full-root-info-one-expected.json
--rw-r--r--   0 runner    (1001) docker     (998)     1047 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/virtual_codebase/full-root-info-one.json
--rw-r--r--   0 runner    (1001) docker     (998)    50927 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/virtual_codebase/lcp.json
--rw-r--r--   0 runner    (1001) docker     (998)     5671 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/virtual_codebase/license-scan.json
--rw-r--r--   0 runner    (1001) docker     (998)      608 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/virtual_codebase/node-16-slim.json
--rw-r--r--   0 runner    (1001) docker     (998)      396 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/virtual_codebase/noinfo.json
--rw-r--r--   0 runner    (1001) docker     (998)      121 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/virtual_codebase/only-path.json
--rw-r--r--   0 runner    (1001) docker     (998)      576 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/virtual_codebase/resource.json
--rw-r--r--   0 runner    (1001) docker     (998)      184 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/virtual_codebase/root-is-not-first-resource.json
--rw-r--r--   0 runner    (1001) docker     (998)     8187 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/virtual_codebase/samples-only-findings-expected.json
--rw-r--r--   0 runner    (1001) docker     (998)     4410 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/virtual_codebase/samples-only-findings.json
--rw-r--r--   0 runner    (1001) docker     (998)      298 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/virtual_codebase/stripped-and-skipped-root.json
--rw-r--r--   0 runner    (1001) docker     (998)     3151 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/virtual_codebase/virtual_codebase.json
--rw-r--r--   0 runner    (1001) docker     (998)     6690 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/virtual_codebase/zephyr-binary.json
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.923959 commoncode-31.0.3/tests/data/resource/with_path/
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.923959 commoncode-31.0.3/tests/data/resource/with_path/codebase/
--rw-r--r--   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/with_path/codebase/abc
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.923959 commoncode-31.0.3/tests/data/resource/with_path/codebase/dir/
--rw-r--r--   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/with_path/codebase/dir/that
--rw-r--r--   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/with_path/codebase/dir/this
--rw-r--r--   0 runner    (1001) docker     (998)     2228 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/with_path/codebase/et131x.h
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.923959 commoncode-31.0.3/tests/data/resource/with_path/codebase/other dir/
--rw-r--r--   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/with_path/codebase/other dir/file
--rw-r--r--   0 runner    (1001) docker     (998)      262 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/with_path/codebase-expected.json
--rw-r--r--   0 runner    (1001) docker     (998)      262 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/with_path/virtual-codebase-expected.json
--rw-r--r--   0 runner    (1001) docker     (998)     2205 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/resource/with_path/virtual-codebase.json
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.923959 commoncode-31.0.3/tests/data/saneyaml/
--rw-r--r--   0 runner    (1001) docker     (998)     1829 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/saneyaml/metadata1
--rw-r--r--   0 runner    (1001) docker     (998)     1393 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/saneyaml/metadata1.notag
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.923959 commoncode-31.0.3/tests/data/symlink/
--rw-r--r--   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/symlink/test
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.923959 commoncode-31.0.3/tests/data/symlink/walk/
--rw-r--r--   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/symlink/walk/a
-drwxr-xr-x   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:23.923959 commoncode-31.0.3/tests/data/symlink/walk/dir/
--rw-r--r--   0 runner    (1001) docker     (998)        0 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/data/symlink/walk/dir/b
--rw-r--r--   0 runner    (1001) docker     (998)     5114 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/test_cliutils.py
--rw-r--r--   0 runner    (1001) docker     (998)      878 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/test_cliutils_progressbar.py
--rw-r--r--   0 runner    (1001) docker     (998)     3144 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/test_codec.py
--rw-r--r--   0 runner    (1001) docker     (998)     5946 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/test_command.py
--rw-r--r--   0 runner    (1001) docker     (998)     2065 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/test_date.py
--rw-r--r--   0 runner    (1001) docker     (998)     4130 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/test_fileset.py
--rw-r--r--   0 runner    (1001) docker     (998)     7749 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/test_filetype.py
--rw-r--r--   0 runner    (1001) docker     (998)    39362 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/test_fileutils.py
--rw-r--r--   0 runner    (1001) docker     (998)     1659 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/test_functional.py
--rw-r--r--   0 runner    (1001) docker     (998)     7107 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/test_hash.py
--rw-r--r--   0 runner    (1001) docker     (998)     8215 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/test_ignore.py
--rw-r--r--   0 runner    (1001) docker     (998)    12779 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/test_paths.py
--rw-r--r--   0 runner    (1001) docker     (998)    63974 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/test_resource.py
--rw-r--r--   0 runner    (1001) docker     (998)      917 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/test_saneyaml.py
--rw-r--r--   0 runner    (1001) docker     (998)     1312 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/test_skeleton_codestyle.py
--rw-r--r--   0 runner    (1001) docker     (998)     2946 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/test_text.py
--rw-r--r--   0 runner    (1001) docker     (998)     3671 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/test_timeutils.py
--rw-r--r--   0 runner    (1001) docker     (998)     5784 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/test_urn.py
--rw-r--r--   0 runner    (1001) docker     (998)     8797 2023-08-25 20:43:12.000000 commoncode-31.0.3/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.846425 commoncode-31.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-15 23:25:49.000000 commoncode-31.1.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.774424 commoncode-31.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.794425 commoncode-31.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-05-15 23:25:49.000000 commoncode-31.1.0/.github/workflows/docs-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-05-15 23:25:49.000000 commoncode-31.1.0/.github/workflows/pypi-release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-15 23:25:49.000000 commoncode-31.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-15 23:25:49.000000 commoncode-31.1.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-15 23:25:49.000000 commoncode-31.1.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8900 2024-05-15 23:25:49.000000 commoncode-31.1.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3422 2024-05-15 23:25:49.000000 commoncode-31.1.0/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-15 23:25:49.000000 commoncode-31.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-05-15 23:25:49.000000 commoncode-31.1.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-15 23:25:49.000000 commoncode-31.1.0/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-05-15 23:25:54.846425 commoncode-31.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-05-15 23:25:49.000000 commoncode-31.1.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-15 23:25:49.000000 commoncode-31.1.0/apache-2.0.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4474 2024-05-15 23:25:49.000000 commoncode-31.1.0/azure-pipelines.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-15 23:25:49.000000 commoncode-31.1.0/commoncode.ABOUT
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6328 2024-05-15 23:25:49.000000 commoncode-31.1.0/configure
+-rw-r--r--   0 runner    (1001) docker     (127)     6948 2024-05-15 23:25:49.000000 commoncode-31.1.0/configure.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.794425 commoncode-31.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-15 23:25:49.000000 commoncode-31.1.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-15 23:25:49.000000 commoncode-31.1.0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.794425 commoncode-31.1.0/docs/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-15 23:25:49.000000 commoncode-31.1.0/docs/scripts/doc8_style_check.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-15 23:25:49.000000 commoncode-31.1.0/docs/scripts/sphinx_build_link_check.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.794425 commoncode-31.1.0/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.794425 commoncode-31.1.0/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     8022 2024-05-15 23:25:49.000000 commoncode-31.1.0/docs/source/_static/theme_overrides.css
+-rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-05-15 23:25:49.000000 commoncode-31.1.0/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.794425 commoncode-31.1.0/docs/source/contribute/
+-rw-r--r--   0 runner    (1001) docker     (127)    10245 2024-05-15 23:25:49.000000 commoncode-31.1.0/docs/source/contribute/contrib_doc.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-15 23:25:49.000000 commoncode-31.1.0/docs/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.774424 commoncode-31.1.0/etc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.794425 commoncode-31.1.0/etc/ci/
+-rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-05-15 23:25:49.000000 commoncode-31.1.0/etc/ci/azure-container-deb.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-05-15 23:25:49.000000 commoncode-31.1.0/etc/ci/azure-container-rpm.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-05-15 23:25:49.000000 commoncode-31.1.0/etc/ci/azure-posix.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-05-15 23:25:49.000000 commoncode-31.1.0/etc/ci/azure-win.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-15 23:25:49.000000 commoncode-31.1.0/etc/ci/install_sudo.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     8365 2024-05-15 23:25:49.000000 commoncode-31.1.0/etc/ci/macports-ci
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-15 23:25:49.000000 commoncode-31.1.0/etc/ci/macports-ci.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-15 23:25:49.000000 commoncode-31.1.0/etc/ci/mit.LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.798425 commoncode-31.1.0/etc/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3744 2024-05-15 23:25:49.000000 commoncode-31.1.0/etc/scripts/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-15 23:25:49.000000 commoncode-31.1.0/etc/scripts/check_thirdparty.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9486 2024-05-15 23:25:49.000000 commoncode-31.1.0/etc/scripts/fetch_thirdparty.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9699 2024-05-15 23:25:49.000000 commoncode-31.1.0/etc/scripts/gen_pypi_simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-15 23:25:49.000000 commoncode-31.1.0/etc/scripts/gen_pypi_simple.py.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (127)     2776 2024-05-15 23:25:49.000000 commoncode-31.1.0/etc/scripts/gen_pypi_simple.py.NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-05-15 23:25:49.000000 commoncode-31.1.0/etc/scripts/gen_requirements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-05-15 23:25:49.000000 commoncode-31.1.0/etc/scripts/gen_requirements_dev.py
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-15 23:25:49.000000 commoncode-31.1.0/etc/scripts/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4497 2024-05-15 23:25:49.000000 commoncode-31.1.0/etc/scripts/test_utils_pip_compatibility_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-15 23:25:49.000000 commoncode-31.1.0/etc/scripts/test_utils_pip_compatibility_tags.py.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (127)     2839 2024-05-15 23:25:49.000000 commoncode-31.1.0/etc/scripts/test_utils_pypi_supported_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-15 23:25:49.000000 commoncode-31.1.0/etc/scripts/test_utils_pypi_supported_tags.py.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (127)     6418 2024-05-15 23:25:49.000000 commoncode-31.1.0/etc/scripts/utils_dejacode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6704 2024-05-15 23:25:49.000000 commoncode-31.1.0/etc/scripts/utils_pip_compatibility_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-05-15 23:25:49.000000 commoncode-31.1.0/etc/scripts/utils_pip_compatibility_tags.py.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (127)     2850 2024-05-15 23:25:49.000000 commoncode-31.1.0/etc/scripts/utils_pypi_supported_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-15 23:25:49.000000 commoncode-31.1.0/etc/scripts/utils_pypi_supported_tags.py.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (127)     6152 2024-05-15 23:25:49.000000 commoncode-31.1.0/etc/scripts/utils_requirements.py
+-rw-r--r--   0 runner    (1001) docker     (127)    75931 2024-05-15 23:25:49.000000 commoncode-31.1.0/etc/scripts/utils_thirdparty.py
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-15 23:25:49.000000 commoncode-31.1.0/etc/scripts/utils_thirdparty.py.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-05-15 23:25:49.000000 commoncode-31.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-15 23:25:49.000000 commoncode-31.1.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-15 23:25:49.000000 commoncode-31.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-05-15 23:25:54.850425 commoncode-31.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-15 23:25:49.000000 commoncode-31.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.774424 commoncode-31.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.802425 commoncode-31.1.0/src/commoncode/
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-05-15 23:25:49.000000 commoncode-31.1.0/src/commoncode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3999 2024-05-15 23:25:49.000000 commoncode-31.1.0/src/commoncode/archive.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19600 2024-05-15 23:25:49.000000 commoncode-31.1.0/src/commoncode/cliutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-05-15 23:25:49.000000 commoncode-31.1.0/src/commoncode/codec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9516 2024-05-15 23:25:49.000000 commoncode-31.1.0/src/commoncode/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-05-15 23:25:49.000000 commoncode-31.1.0/src/commoncode/compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5480 2024-05-15 23:25:49.000000 commoncode-31.1.0/src/commoncode/datautils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-15 23:25:49.000000 commoncode-31.1.0/src/commoncode/date.py
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-15 23:25:49.000000 commoncode-31.1.0/src/commoncode/dict_utils.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-05-15 23:25:49.000000 commoncode-31.1.0/src/commoncode/dict_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2148 2024-05-15 23:25:49.000000 commoncode-31.1.0/src/commoncode/fetch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6487 2024-05-15 23:25:49.000000 commoncode-31.1.0/src/commoncode/fileset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6660 2024-05-15 23:25:49.000000 commoncode-31.1.0/src/commoncode/filetype.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17123 2024-05-15 23:25:49.000000 commoncode-31.1.0/src/commoncode/fileutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-15 23:25:49.000000 commoncode-31.1.0/src/commoncode/fileutils.py.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (127)     3325 2024-05-15 23:25:49.000000 commoncode-31.1.0/src/commoncode/functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4967 2024-05-15 23:25:49.000000 commoncode-31.1.0/src/commoncode/hash.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11645 2024-05-15 23:25:49.000000 commoncode-31.1.0/src/commoncode/ignore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9167 2024-05-15 23:25:49.000000 commoncode-31.1.0/src/commoncode/paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32426 2024-05-15 23:25:49.000000 commoncode-31.1.0/src/commoncode/python.LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    73970 2024-05-15 23:25:49.000000 commoncode-31.1.0/src/commoncode/resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4736 2024-05-15 23:25:49.000000 commoncode-31.1.0/src/commoncode/system.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14225 2024-05-15 23:25:49.000000 commoncode-31.1.0/src/commoncode/testcase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4163 2024-05-15 23:25:49.000000 commoncode-31.1.0/src/commoncode/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3692 2024-05-15 23:25:49.000000 commoncode-31.1.0/src/commoncode/timeutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4551 2024-05-15 23:25:49.000000 commoncode-31.1.0/src/commoncode/urn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9995 2024-05-15 23:25:49.000000 commoncode-31.1.0/src/commoncode/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.846425 commoncode-31.1.0/src/commoncode.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-05-15 23:25:54.000000 commoncode-31.1.0/src/commoncode.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14540 2024-05-15 23:25:54.000000 commoncode-31.1.0/src/commoncode.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 23:25:54.000000 commoncode-31.1.0/src/commoncode.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 23:25:54.000000 commoncode-31.1.0/src/commoncode.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-15 23:25:54.000000 commoncode-31.1.0/src/commoncode.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-15 23:25:54.000000 commoncode-31.1.0/src/commoncode.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.806425 commoncode-31.1.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.790424 commoncode-31.1.0/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.774424 commoncode-31.1.0/tests/data/count/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.774424 commoncode-31.1.0/tests/data/count/filecount/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.810425 commoncode-31.1.0/tests/data/count/filecount/dir/
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/count/filecount/dir/a.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/count/filecount/dir/b.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/count/filecount/dir/c.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.810425 commoncode-31.1.0/tests/data/count/filecount/dir/sub1/
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/count/filecount/dir/sub1/a.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/count/filecount/dir/sub1/b.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/count/filecount/dir/sub1/c.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.810425 commoncode-31.1.0/tests/data/count/filecount/dir/sub1/subsub/
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/count/filecount/dir/sub1/subsub/a.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/count/filecount/dir/sub1/subsub/b.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.810425 commoncode-31.1.0/tests/data/count/filecount/dir/sub2/
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/count/filecount/dir/sub2/a.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.810425 commoncode-31.1.0/tests/data/date/
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/date/ant-jsch-1.7.0.tar.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.810425 commoncode-31.1.0/tests/data/date/dir/
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/date/dir/a.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/date/dir/b.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/date/dir/c.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.810425 commoncode-31.1.0/tests/data/date/dir/sub1/
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/date/dir/sub1/a.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/date/dir/sub1/b.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/date/dir/sub1/c.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.810425 commoncode-31.1.0/tests/data/date/dir/sub1/subsub/
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/date/dir/sub1/subsub/a.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/date/dir/sub1/subsub/b.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.810425 commoncode-31.1.0/tests/data/date/dir/sub2/
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/date/dir/sub2/a.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.810425 commoncode-31.1.0/tests/data/fileset/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/fileset/scancodeignore.lst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.810425 commoncode-31.1.0/tests/data/filetype/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.778424 commoncode-31.1.0/tests/data/filetype/readwrite/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.810425 commoncode-31.1.0/tests/data/filetype/readwrite/sub/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/filetype/readwrite/sub/file
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.810425 commoncode-31.1.0/tests/data/filetype/size/
+-rw-r--r--   0 runner    (1001) docker     (127)    12388 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/filetype/size/Image1.eps
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.810425 commoncode-31.1.0/tests/data/filetype/size/exec/
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/filetype/size/exec/1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/filetype/size/exec/a.bat
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/filetype/size/exec/a.tar
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.814425 commoncode-31.1.0/tests/data/filetype/size/exec/subtxt/
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/filetype/size/exec/subtxt/1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/filetype/size/exec/subtxt/a.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/filetype/size/exec/subtxt/b.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   109056 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/filetype/types.tar
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.778424 commoncode-31.1.0/tests/data/fileutils/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.814425 commoncode-31.1.0/tests/data/fileutils/basename/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.814425 commoncode-31.1.0/tests/data/fileutils/basename/a/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.814425 commoncode-31.1.0/tests/data/fileutils/basename/a/.a/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/fileutils/basename/a/.a/file
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.814425 commoncode-31.1.0/tests/data/fileutils/basename/a/b/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/fileutils/basename/a/b/.a
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/fileutils/basename/a/b/.a.b
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/fileutils/basename/a/b/a.tag.gz
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/fileutils/basename/a/f.a
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.814425 commoncode-31.1.0/tests/data/fileutils/basename/f.a/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/fileutils/basename/f.a/a.c
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/fileutils/basename/tst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.814425 commoncode-31.1.0/tests/data/fileutils/exec/
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/fileutils/exec/1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/fileutils/exec/a.bat
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/fileutils/exec/a.tar
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.814425 commoncode-31.1.0/tests/data/fileutils/exec/subtxt/
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/fileutils/exec/subtxt/1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/fileutils/exec/subtxt/a.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/fileutils/exec/subtxt/b.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.778424 commoncode-31.1.0/tests/data/fileutils/executable/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.778424 commoncode-31.1.0/tests/data/fileutils/executable/deep1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.814425 commoncode-31.1.0/tests/data/fileutils/executable/deep1/deep2/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/fileutils/executable/deep1/deep2/ctags
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.814425 commoncode-31.1.0/tests/data/fileutils/filetype/
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/fileutils/filetype/a.html
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/fileutils/filetype/stage1
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.814425 commoncode-31.1.0/tests/data/fileutils/perms/
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/fileutils/perms/unreadable.tgz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.778424 commoncode-31.1.0/tests/data/fileutils/readwrite/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.814425 commoncode-31.1.0/tests/data/fileutils/readwrite/sub/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/fileutils/readwrite/sub/file
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.814425 commoncode-31.1.0/tests/data/fileutils/walk/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.814425 commoncode-31.1.0/tests/data/fileutils/walk/d1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.814425 commoncode-31.1.0/tests/data/fileutils/walk/d1/d2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.814425 commoncode-31.1.0/tests/data/fileutils/walk/d1/d2/d3/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/fileutils/walk/d1/d2/d3/f3
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/fileutils/walk/d1/d2/f2
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/fileutils/walk/d1/f1
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/fileutils/walk/f
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/fileutils/walk/unicode.zip
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.814425 commoncode-31.1.0/tests/data/fileutils/walk_non_utf8/
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/fileutils/walk_non_utf8/non_unicode.tgz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.782425 commoncode-31.1.0/tests/data/hash/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.818425 commoncode-31.1.0/tests/data/hash/dir1/
+-rw-r--r--   0 runner    (1001) docker     (127)     7859 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/hash/dir1/a.png
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/hash/dir1/a.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.818425 commoncode-31.1.0/tests/data/hash/dir2/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/hash/dir2/a.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/hash/dir2/dos.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.818425 commoncode-31.1.0/tests/data/hash/sha1-collision/
+-rw-r--r--   0 runner    (1001) docker     (127)   422435 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/hash/sha1-collision/shattered-1.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/hash/sha1-collision/shattered-1.pdf.ABOUT
+-rw-r--r--   0 runner    (1001) docker     (127)   422435 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/hash/sha1-collision/shattered-2.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/hash/sha1-collision/shattered-2.pdf.ABOUT
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.818425 commoncode-31.1.0/tests/data/ignore/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/ignore/.scancodeignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.818425 commoncode-31.1.0/tests/data/ignore/excludes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/ignore/excludes/.localized
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/ignore/excludes/eclipse.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/ignore/excludes/mac.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/ignore/excludes/msft-vs.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)     6296 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/ignore/vcs.tgz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.790424 commoncode-31.1.0/tests/data/resource/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.782425 commoncode-31.1.0/tests/data/resource/cache/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.818425 commoncode-31.1.0/tests/data/resource/cache/package/
+-rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/cache/package/package.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.818425 commoncode-31.1.0/tests/data/resource/cache2/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/cache2/abc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.818425 commoncode-31.1.0/tests/data/resource/cache2/dir/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/cache2/dir/that
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/cache2/dir/this
+-rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/cache2/et131x.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.818425 commoncode-31.1.0/tests/data/resource/cache2/other dir/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/cache2/other dir/file
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.782425 commoncode-31.1.0/tests/data/resource/client/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.822425 commoncode-31.1.0/tests/data/resource/client/Images/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/client/Images/applicationCache.png
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/client/Images/spinner.gif
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.822425 commoncode-31.1.0/tests/data/resource/codebase/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/codebase/abc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.822425 commoncode-31.1.0/tests/data/resource/codebase/dir/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/codebase/dir/that
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/codebase/dir/this
+-rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/codebase/et131x.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.822425 commoncode-31.1.0/tests/data/resource/codebase/other dir/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/codebase/other dir/file
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.822425 commoncode-31.1.0/tests/data/resource/deeply_nested/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.822425 commoncode-31.1.0/tests/data/resource/deeply_nested/level1_dir1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.822425 commoncode-31.1.0/tests/data/resource/deeply_nested/level1_dir1/level2_dir1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.822425 commoncode-31.1.0/tests/data/resource/deeply_nested/level1_dir1/level2_dir1/level3_dir1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/deeply_nested/level1_dir1/level2_dir1/level3_dir1/level4_file1
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/deeply_nested/level1_dir1/level2_dir1/level3_file1
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/deeply_nested/level1_dir1/level2_dir1/level3_file2
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/deeply_nested/level1_dir1/level2_file1
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/deeply_nested/level1_dir1/level2_file2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.822425 commoncode-31.1.0/tests/data/resource/deeply_nested/level1_dir2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.822425 commoncode-31.1.0/tests/data/resource/deeply_nested/level1_dir2/level2_dir3/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/deeply_nested/level1_dir2/level2_dir3/level3_file3
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/deeply_nested/level1_dir2/level2_dir3/level3_file4
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/deeply_nested/level1_dir2/level2_file3
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/deeply_nested/level1_dir2/level2_file4
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/deeply_nested/level1_dir2/level2_file5
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/deeply_nested/level1_file1
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/deeply_nested/level1_file2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.782425 commoncode-31.1.0/tests/data/resource/dist/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.822425 commoncode-31.1.0/tests/data/resource/dist/JGroups/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/dist/JGroups/EULA
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/dist/JGroups/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.822425 commoncode-31.1.0/tests/data/resource/dist/JGroups/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/dist/JGroups/src/RouterStub.java
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/dist/JGroups/src/RouterStubManager.java
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/dist/JGroups/src/S3_PING.java
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.782425 commoncode-31.1.0/tests/data/resource/dist/simple/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.822425 commoncode-31.1.0/tests/data/resource/dist/simple/META-INF/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/dist/simple/META-INF/MANIFEST.MF
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.822425 commoncode-31.1.0/tests/data/resource/ignore/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.822425 commoncode-31.1.0/tests/data/resource/ignore/cvs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/ignore/cvs/file2
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/ignore/file1
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.782425 commoncode-31.1.0/tests/data/resource/lcp/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.822425 commoncode-31.1.0/tests/data/resource/lcp/test1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.826425 commoncode-31.1.0/tests/data/resource/lcp/test1/JGroups/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/lcp/test1/JGroups/EULA
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/lcp/test1/JGroups/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.826425 commoncode-31.1.0/tests/data/resource/lcp/test1/JGroups/licenses/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/lcp/test1/JGroups/licenses/apache-1.1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/lcp/test1/JGroups/licenses/lgpl.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.826425 commoncode-31.1.0/tests/data/resource/lcp/test1/JGroups/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/lcp/test1/JGroups/src/RouterStub.java
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/lcp/test1/JGroups/src/RouterStubManager.java
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/lcp/test1/JGroups/src/S3_PING.java
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/lcp/test1/screenshot.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.786424 commoncode-31.1.0/tests/data/resource/lcp/test1/simple/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.826425 commoncode-31.1.0/tests/data/resource/lcp/test1/simple/META-INF/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/lcp/test1/simple/META-INF/MANIFEST.MF
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.786424 commoncode-31.1.0/tests/data/resource/lcp/test1/simple/org/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.786424 commoncode-31.1.0/tests/data/resource/lcp/test1/simple/org/jvnet/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.786424 commoncode-31.1.0/tests/data/resource/lcp/test1/simple/org/jvnet/glassfish/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.786424 commoncode-31.1.0/tests/data/resource/lcp/test1/simple/org/jvnet/glassfish/comms/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.826425 commoncode-31.1.0/tests/data/resource/lcp/test1/simple/org/jvnet/glassfish/comms/sipagent/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.826425 commoncode-31.1.0/tests/data/resource/lcp/test1/simple/org/jvnet/glassfish/comms/sipagent/actions/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/lcp/test1/simple/org/jvnet/glassfish/comms/sipagent/actions/Bundle.properties
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/lcp/test1/simple/org/jvnet/glassfish/comms/sipagent/actions/SipAgentCookieAction.class
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/lcp/test1/simple/org/jvnet/glassfish/comms/sipagent/actions/bd.png
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/lcp/test1/simple/org/jvnet/glassfish/comms/sipagent/actions/bd24.png
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/lcp/test1/simple/org/jvnet/glassfish/comms/sipagent/org-jvnet-glassfish-comms-sipagent-actions-SipAgentCookieAction.instance
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/lcp/test1/simple/org/jvnet/glassfish/comms/sipagent/org-jvnet-glassfish-comms-sipagent-actions-SipAgentCookieAction_1.instance
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.786424 commoncode-31.1.0/tests/data/resource/lcp/test1/zlib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.826425 commoncode-31.1.0/tests/data/resource/lcp/test1/zlib/ada/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/lcp/test1/zlib/ada/zlib.ads
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.786424 commoncode-31.1.0/tests/data/resource/lcp/test1/zlib/inter/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.826425 commoncode-31.1.0/tests/data/resource/lcp/test1/zlib/inter/arch/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/lcp/test1/zlib/inter/arch/zlib.tar.gz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.826425 commoncode-31.1.0/tests/data/resource/lcp/test1/zlib/inter/dir/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/lcp/test1/zlib/inter/dir/EULA
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/lcp/test1/zlib/inter/dir/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.826425 commoncode-31.1.0/tests/data/resource/lcp/test1/zlib/inter/dir/licenses/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/lcp/test1/zlib/inter/dir/licenses/apache-1.1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/lcp/test1/zlib/inter/dir/licenses/apache-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/lcp/test1/zlib/inter/dir/licenses/bouncycastle.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/lcp/test1/zlib/inter/dir/licenses/cpl-1.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/lcp/test1/zlib/inter/dir/licenses/lgpl.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.830425 commoncode-31.1.0/tests/data/resource/lcp/test1/zlib/inter/dir/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/lcp/test1/zlib/inter/dir/src/FixedMembershipToken.java
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/lcp/test1/zlib/inter/dir/src/GuardedBy.java
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/lcp/test1/zlib/inter/dir/src/ImmutableReference.java
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/lcp/test1/zlib/inter/dir/src/RATE_LIMITER.java
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/lcp/test1/zlib/inter/dir/src/RouterStub.java
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/lcp/test1/zlib/inter/dir/src/RouterStubManager.java
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/lcp/test1/zlib/inter/dir/src/S3_PING.java
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.830425 commoncode-31.1.0/tests/data/resource/lcp/test1/zlib/inter/iostream2/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/lcp/test1/zlib/inter/iostream2/zstream.h
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/lcp/test1/zlib/inter/iostream2/zstream_test.cpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.830425 commoncode-31.1.0/tests/data/resource/lcp/test1/zlib/inter/zlib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.830425 commoncode-31.1.0/tests/data/resource/lcp/test1/zlib/inter/zlib/ada/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/lcp/test1/zlib/inter/zlib/ada/zlib.ads
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/lcp/test1/zlib/inter/zlib/adler32.c
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/lcp/test1/zlib/inter/zlib/deflate.c
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/lcp/test1/zlib/inter/zlib/deflate.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.830425 commoncode-31.1.0/tests/data/resource/lcp/test1/zlib/inter/zlib/dotzlib/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/lcp/test1/zlib/inter/zlib/dotzlib/AssemblyInfo.cs
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/lcp/test1/zlib/inter/zlib/dotzlib/ChecksumImpl.cs
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/lcp/test1/zlib/inter/zlib/dotzlib/LICENSE_1_0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/lcp/test1/zlib/inter/zlib/dotzlib/readme.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.830425 commoncode-31.1.0/tests/data/resource/lcp/test1/zlib/inter/zlib/gcc_gvmat64/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/lcp/test1/zlib/inter/zlib/gcc_gvmat64/gvmat64.S
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.830425 commoncode-31.1.0/tests/data/resource/lcp/test1/zlib/inter/zlib/infback9/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/lcp/test1/zlib/inter/zlib/infback9/infback9.c
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/lcp/test1/zlib/inter/zlib/infback9/infback9.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.830425 commoncode-31.1.0/tests/data/resource/lcp/test1/zlib/inter/zlib/iostream2/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/lcp/test1/zlib/inter/zlib/iostream2/zstream.h
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/lcp/test1/zlib/inter/zlib/iostream2/zstream_test.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/lcp/test1/zlib/inter/zlib/zlib.h
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/lcp/test1/zlib/inter/zlib/zutil.c
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/lcp/test1/zlib/inter/zlib/zutil.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.830425 commoncode-31.1.0/tests/data/resource/resource/
+-rw-r--r--   0 runner    (1001) docker     (127)     7194 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/resource/test-extracted-from-to.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.830425 commoncode-31.1.0/tests/data/resource/samples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.834425 commoncode-31.1.0/tests/data/resource/samples/JGroups/
+-rw-r--r--   0 runner    (1001) docker     (127)     8156 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/samples/JGroups/EULA
+-rw-r--r--   0 runner    (1001) docker     (127)    26430 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/samples/JGroups/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.834425 commoncode-31.1.0/tests/data/resource/samples/JGroups/licenses/
+-rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/samples/JGroups/licenses/apache-1.1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11560 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/samples/JGroups/licenses/apache-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/samples/JGroups/licenses/bouncycastle.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11987 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/samples/JGroups/licenses/cpl-1.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    26934 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/samples/JGroups/licenses/lgpl.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.834425 commoncode-31.1.0/tests/data/resource/samples/JGroups/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     5144 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/samples/JGroups/src/FixedMembershipToken.java
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/samples/JGroups/src/GuardedBy.java
+-rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/samples/JGroups/src/ImmutableReference.java
+-rw-r--r--   0 runner    (1001) docker     (127)     3692 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/samples/JGroups/src/RATE_LIMITER.java
+-rw-r--r--   0 runner    (1001) docker     (127)     9913 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/samples/JGroups/src/RouterStub.java
+-rw-r--r--   0 runner    (1001) docker     (127)     8162 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/samples/JGroups/src/RouterStubManager.java
+-rw-r--r--   0 runner    (1001) docker     (127)   122528 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/samples/JGroups/src/S3_PING.java
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/samples/README
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.834425 commoncode-31.1.0/tests/data/resource/samples/arch/
+-rw-r--r--   0 runner    (1001) docker     (127)    28103 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/samples/arch/zlib.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (127)   622754 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/samples/screenshot.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.838425 commoncode-31.1.0/tests/data/resource/samples/zlib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.838425 commoncode-31.1.0/tests/data/resource/samples/zlib/ada/
+-rw-r--r--   0 runner    (1001) docker     (127)    13594 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/samples/zlib/ada/zlib.ads
+-rw-r--r--   0 runner    (1001) docker     (127)     4968 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/samples/zlib/adler32.c
+-rw-r--r--   0 runner    (1001) docker     (127)    71476 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/samples/zlib/deflate.c
+-rw-r--r--   0 runner    (1001) docker     (127)    12774 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/samples/zlib/deflate.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.838425 commoncode-31.1.0/tests/data/resource/samples/zlib/dotzlib/
+-rw-r--r--   0 runner    (1001) docker     (127)     2500 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/samples/zlib/dotzlib/AssemblyInfo.cs
+-rw-r--r--   0 runner    (1001) docker     (127)     8040 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/samples/zlib/dotzlib/ChecksumImpl.cs
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/samples/zlib/dotzlib/LICENSE_1_0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/samples/zlib/dotzlib/readme.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.838425 commoncode-31.1.0/tests/data/resource/samples/zlib/gcc_gvmat64/
+-rw-r--r--   0 runner    (1001) docker     (127)    16413 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/samples/zlib/gcc_gvmat64/gvmat64.S
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.838425 commoncode-31.1.0/tests/data/resource/samples/zlib/infback9/
+-rw-r--r--   0 runner    (1001) docker     (127)    21629 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/samples/zlib/infback9/infback9.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/samples/zlib/infback9/infback9.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.838425 commoncode-31.1.0/tests/data/resource/samples/zlib/iostream2/
+-rw-r--r--   0 runner    (1001) docker     (127)     9283 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/samples/zlib/iostream2/zstream.h
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/samples/zlib/iostream2/zstream_test.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    87883 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/samples/zlib/zlib.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7414 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/samples/zlib/zutil.c
+-rw-r--r--   0 runner    (1001) docker     (127)     6766 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/samples/zlib/zutil.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.838425 commoncode-31.1.0/tests/data/resource/skip_directories_during_walk/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.838425 commoncode-31.1.0/tests/data/resource/skip_directories_during_walk/skip-this-directory/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/skip_directories_during_walk/skip-this-directory/this-should-not-be-returned
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/skip_directories_during_walk/this-should-be-returned
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.842425 commoncode-31.1.0/tests/data/resource/virtual_codebase/
+-rw-r--r--   0 runner    (1001) docker     (127)     4628 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/virtual_codebase/codebase-for-cache-tests.json
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/virtual_codebase/combine-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/virtual_codebase/combine-2.json
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/virtual_codebase/combine-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/virtual_codebase/combine-shared-directory-name-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/virtual_codebase/combine-shared-directory-name-2.json
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/virtual_codebase/combine-shared-directory-name-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5129 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/virtual_codebase/docker-hello-world.json
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/virtual_codebase/et131x.h.json
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/virtual_codebase/fingerprint_attribute.json
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/virtual_codebase/from_file.json
+-rw-r--r--   0 runner    (1001) docker     (127)    17547 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/virtual_codebase/full-root-info-many-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)    16812 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/virtual_codebase/full-root-info-many.json
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/virtual_codebase/full-root-info-one-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/virtual_codebase/full-root-info-one.json
+-rw-r--r--   0 runner    (1001) docker     (127)    50927 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/virtual_codebase/lcp.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5671 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/virtual_codebase/license-scan.json
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/virtual_codebase/node-16-slim.json
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/virtual_codebase/noinfo.json
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/virtual_codebase/only-path.json
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/virtual_codebase/resource.json
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/virtual_codebase/root-is-not-first-resource.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8187 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/virtual_codebase/samples-only-findings-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4410 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/virtual_codebase/samples-only-findings.json
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/virtual_codebase/stripped-and-skipped-root.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3151 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/virtual_codebase/virtual_codebase.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6690 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/virtual_codebase/zephyr-binary.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.842425 commoncode-31.1.0/tests/data/resource/with_path/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.842425 commoncode-31.1.0/tests/data/resource/with_path/codebase/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/with_path/codebase/abc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.842425 commoncode-31.1.0/tests/data/resource/with_path/codebase/dir/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/with_path/codebase/dir/that
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/with_path/codebase/dir/this
+-rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/with_path/codebase/et131x.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.842425 commoncode-31.1.0/tests/data/resource/with_path/codebase/other dir/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/with_path/codebase/other dir/file
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/with_path/codebase-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/with_path/virtual-codebase-expected.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/resource/with_path/virtual-codebase.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.846425 commoncode-31.1.0/tests/data/saneyaml/
+-rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/saneyaml/metadata1
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/saneyaml/metadata1.notag
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.846425 commoncode-31.1.0/tests/data/symlink/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/symlink/test
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.846425 commoncode-31.1.0/tests/data/symlink/walk/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/symlink/walk/a
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:54.846425 commoncode-31.1.0/tests/data/symlink/walk/dir/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/data/symlink/walk/dir/b
+-rw-r--r--   0 runner    (1001) docker     (127)     5114 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/test_cliutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/test_cliutils_progressbar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/test_codec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5946 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/test_command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2065 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/test_date.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4130 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/test_fileset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7749 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/test_filetype.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39362 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/test_fileutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/test_functional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7107 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/test_hash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8215 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/test_ignore.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12779 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/test_paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63974 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/test_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/test_saneyaml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/test_skeleton_codestyle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/test_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3671 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/test_timeutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5784 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/test_urn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8797 2024-05-15 23:25:49.000000 commoncode-31.1.0/tests/test_version.py
```

### Comparing `commoncode-31.0.3/.github/workflows/docs-ci.yml` & `commoncode-31.1.0/.github/workflows/docs-ci.yml`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/.github/workflows/pypi-release.yml` & `commoncode-31.1.0/.github/workflows/pypi-release.yml`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/.gitignore` & `commoncode-31.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/.readthedocs.yml` & `commoncode-31.1.0/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/CHANGELOG.rst` & `commoncode-31.1.0/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 Release notes
 =============
 
+Version 31.1.0 - (2024-05-15)
+------------------------------
+
+- Add ``on_macos_arm64`` and ``on_ubuntu_22`` markers to ``commoncode.system``.
+
+
 Version 31.0.3 - (2023-08-25)
 ------------------------------
 
 - Mark our use of MD5 as NOT for security #54
 - Fix VirtualCodebase walk issue when the root directory name is repeated #57
```

### Comparing `commoncode-31.0.3/CODE_OF_CONDUCT.rst` & `commoncode-31.1.0/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/Makefile` & `commoncode-31.1.0/Makefile`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/README.rst` & `commoncode-31.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/apache-2.0.LICENSE` & `commoncode-31.1.0/apache-2.0.LICENSE`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/azure-pipelines.yml` & `commoncode-31.1.0/azure-pipelines.yml`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/commoncode.ABOUT` & `commoncode-31.1.0/commoncode.ABOUT`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/configure` & `commoncode-31.1.0/configure`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/configure.bat` & `commoncode-31.1.0/configure.bat`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/docs/Makefile` & `commoncode-31.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/docs/make.bat` & `commoncode-31.1.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/docs/source/_static/theme_overrides.css` & `commoncode-31.1.0/docs/source/_static/theme_overrides.css`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/docs/source/conf.py` & `commoncode-31.1.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/docs/source/contribute/contrib_doc.rst` & `commoncode-31.1.0/docs/source/contribute/contrib_doc.rst`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/etc/ci/azure-container-deb.yml` & `commoncode-31.1.0/etc/ci/azure-container-deb.yml`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/etc/ci/azure-container-rpm.yml` & `commoncode-31.1.0/etc/ci/azure-container-rpm.yml`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/etc/ci/azure-posix.yml` & `commoncode-31.1.0/etc/ci/azure-posix.yml`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/etc/ci/azure-win.yml` & `commoncode-31.1.0/etc/ci/azure-win.yml`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/etc/ci/macports-ci` & `commoncode-31.1.0/etc/ci/macports-ci`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/etc/ci/macports-ci.ABOUT` & `commoncode-31.1.0/etc/ci/macports-ci.ABOUT`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/etc/ci/mit.LICENSE` & `commoncode-31.1.0/etc/ci/mit.LICENSE`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/etc/scripts/README.rst` & `commoncode-31.1.0/etc/scripts/README.rst`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/etc/scripts/check_thirdparty.py` & `commoncode-31.1.0/etc/scripts/check_thirdparty.py`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/etc/scripts/fetch_thirdparty.py` & `commoncode-31.1.0/etc/scripts/fetch_thirdparty.py`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/etc/scripts/gen_pypi_simple.py` & `commoncode-31.1.0/etc/scripts/gen_pypi_simple.py`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/etc/scripts/gen_pypi_simple.py.NOTICE` & `commoncode-31.1.0/etc/scripts/gen_pypi_simple.py.NOTICE`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/etc/scripts/gen_requirements.py` & `commoncode-31.1.0/etc/scripts/gen_requirements.py`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/etc/scripts/gen_requirements_dev.py` & `commoncode-31.1.0/etc/scripts/gen_requirements_dev.py`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/etc/scripts/test_utils_pip_compatibility_tags.py` & `commoncode-31.1.0/etc/scripts/test_utils_pip_compatibility_tags.py`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/etc/scripts/test_utils_pypi_supported_tags.py` & `commoncode-31.1.0/etc/scripts/test_utils_pypi_supported_tags.py`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/etc/scripts/test_utils_pypi_supported_tags.py.ABOUT` & `commoncode-31.1.0/etc/scripts/test_utils_pypi_supported_tags.py.ABOUT`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/etc/scripts/utils_dejacode.py` & `commoncode-31.1.0/etc/scripts/utils_dejacode.py`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/etc/scripts/utils_pip_compatibility_tags.py` & `commoncode-31.1.0/etc/scripts/utils_pip_compatibility_tags.py`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/etc/scripts/utils_pypi_supported_tags.py` & `commoncode-31.1.0/etc/scripts/utils_pypi_supported_tags.py`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/etc/scripts/utils_pypi_supported_tags.py.ABOUT` & `commoncode-31.1.0/etc/scripts/utils_pypi_supported_tags.py.ABOUT`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/etc/scripts/utils_requirements.py` & `commoncode-31.1.0/etc/scripts/utils_requirements.py`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/etc/scripts/utils_thirdparty.py` & `commoncode-31.1.0/etc/scripts/utils_thirdparty.py`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/etc/scripts/utils_thirdparty.py.ABOUT` & `commoncode-31.1.0/etc/scripts/utils_thirdparty.py.ABOUT`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/pyproject.toml` & `commoncode-31.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/requirements-dev.txt` & `commoncode-31.1.0/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/setup.cfg` & `commoncode-31.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/src/commoncode/__init__.py` & `commoncode-31.1.0/src/commoncode/__init__.py`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/src/commoncode/archive.py` & `commoncode-31.1.0/src/commoncode/archive.py`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/src/commoncode/cliutils.py` & `commoncode-31.1.0/src/commoncode/cliutils.py`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/src/commoncode/codec.py` & `commoncode-31.1.0/src/commoncode/codec.py`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/src/commoncode/command.py` & `commoncode-31.1.0/src/commoncode/command.py`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/src/commoncode/datautils.py` & `commoncode-31.1.0/src/commoncode/datautils.py`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/src/commoncode/date.py` & `commoncode-31.1.0/src/commoncode/date.py`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/src/commoncode/dict_utils.py` & `commoncode-31.1.0/src/commoncode/dict_utils.py`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/src/commoncode/fetch.py` & `commoncode-31.1.0/src/commoncode/fetch.py`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/src/commoncode/fileset.py` & `commoncode-31.1.0/src/commoncode/fileset.py`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/src/commoncode/filetype.py` & `commoncode-31.1.0/src/commoncode/filetype.py`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/src/commoncode/fileutils.py` & `commoncode-31.1.0/src/commoncode/fileutils.py`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/src/commoncode/fileutils.py.ABOUT` & `commoncode-31.1.0/src/commoncode/fileutils.py.ABOUT`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/src/commoncode/functional.py` & `commoncode-31.1.0/src/commoncode/functional.py`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/src/commoncode/hash.py` & `commoncode-31.1.0/src/commoncode/hash.py`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/src/commoncode/ignore.py` & `commoncode-31.1.0/src/commoncode/ignore.py`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/src/commoncode/paths.py` & `commoncode-31.1.0/src/commoncode/paths.py`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/src/commoncode/python.LICENSE` & `commoncode-31.1.0/src/commoncode/python.LICENSE`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/src/commoncode/resource.py` & `commoncode-31.1.0/src/commoncode/resource.py`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/src/commoncode/system.py` & `commoncode-31.1.0/src/commoncode/system.py`

 * *Files 19% similar despite different names*

```diff
@@ -67,14 +67,57 @@
 
 
 on_macos_14_or_higher = is_on_macos_14_or_higher()
 
 del is_on_macos_14_or_higher
 
 
+def is_on_macos_arm64():
+    """
+    Return True if the current OS is macOS running on Apple Silicon.
+    """
+    import platform
+    return on_mac and platform.machine() == 'arm64'
+
+
+on_macos_arm64 = is_on_macos_arm64()
+
+del is_on_macos_arm64
+
+
+def get_etc_os_release_info(os_release_path='/etc/os-release'):
+    """
+    Return a dictionary of key-value pairs from /etc/os-release
+    """
+    os_release_data = {}
+    with open(os_release_path) as f:
+        for line in f:
+            split_line = line.split('=')
+            if not split_line:
+                continue
+            k = split_line[0].strip()
+            v = split_line[-1].strip()
+            os_release_data[k] = v
+    return os_release_data
+
+
+def is_on_ubuntu_22():
+    """
+    Return True if the current OS is Ubuntu 22.XX.
+    """
+    if not on_linux:
+        return False
+    os_release_info = get_etc_os_release_info()
+    return os_release_info['ID'] == 'ubuntu' and '22' in os_release_info['VERSION_ID']
+
+on_ubuntu_22 = is_on_ubuntu_22()
+
+del is_on_ubuntu_22
+
+
 def has_case_sensitive_fs():
     """
     Return True if the current FS is case sensitive.
 
     Windows is not case sensitive, and while older macOS HPFS+ were POSIX and
     case sensitive by default, newer macOS use APFS which is no longer case
     sensitive by default.
```

### Comparing `commoncode-31.0.3/src/commoncode/testcase.py` & `commoncode-31.1.0/src/commoncode/testcase.py`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/src/commoncode/text.py` & `commoncode-31.1.0/src/commoncode/text.py`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/src/commoncode/timeutils.py` & `commoncode-31.1.0/src/commoncode/timeutils.py`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/src/commoncode/urn.py` & `commoncode-31.1.0/src/commoncode/urn.py`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/src/commoncode/version.py` & `commoncode-31.1.0/src/commoncode/version.py`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/src/commoncode.egg-info/SOURCES.txt` & `commoncode-31.1.0/src/commoncode.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/tests/data/date/ant-jsch-1.7.0.tar.gz` & `commoncode-31.1.0/tests/data/date/ant-jsch-1.7.0.tar.gz`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/tests/data/filetype/size/Image1.eps` & `commoncode-31.1.0/tests/data/filetype/size/Image1.eps`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/tests/data/filetype/types.tar` & `commoncode-31.1.0/tests/data/filetype/types.tar`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/tests/data/fileutils/filetype/stage1` & `commoncode-31.1.0/tests/data/fileutils/filetype/stage1`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/tests/data/fileutils/walk/unicode.zip` & `commoncode-31.1.0/tests/data/fileutils/walk/unicode.zip`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/tests/data/hash/dir1/a.png` & `commoncode-31.1.0/tests/data/hash/dir1/a.png`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/tests/data/hash/sha1-collision/shattered-1.pdf` & `commoncode-31.1.0/tests/data/hash/sha1-collision/shattered-1.pdf`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/tests/data/hash/sha1-collision/shattered-2.pdf` & `commoncode-31.1.0/tests/data/hash/sha1-collision/shattered-2.pdf`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/tests/data/ignore/vcs.tgz` & `commoncode-31.1.0/tests/data/ignore/vcs.tgz`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/tests/data/resource/cache/package/package.json` & `commoncode-31.1.0/tests/data/resource/cache/package/package.json`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/tests/data/resource/cache2/et131x.h` & `commoncode-31.1.0/tests/data/resource/cache2/et131x.h`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/tests/data/resource/codebase/et131x.h` & `commoncode-31.1.0/tests/data/resource/codebase/et131x.h`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/tests/data/resource/resource/test-extracted-from-to.json` & `commoncode-31.1.0/tests/data/resource/resource/test-extracted-from-to.json`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/tests/data/resource/samples/JGroups/EULA` & `commoncode-31.1.0/tests/data/resource/samples/JGroups/EULA`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/tests/data/resource/samples/JGroups/LICENSE` & `commoncode-31.1.0/tests/data/resource/samples/JGroups/LICENSE`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/tests/data/resource/samples/JGroups/licenses/apache-1.1.txt` & `commoncode-31.1.0/tests/data/resource/samples/JGroups/licenses/apache-1.1.txt`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/tests/data/resource/samples/JGroups/licenses/apache-2.0.txt` & `commoncode-31.1.0/tests/data/resource/samples/JGroups/licenses/apache-2.0.txt`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/tests/data/resource/samples/JGroups/licenses/bouncycastle.txt` & `commoncode-31.1.0/tests/data/resource/samples/JGroups/licenses/bouncycastle.txt`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/tests/data/resource/samples/JGroups/licenses/cpl-1.0.txt` & `commoncode-31.1.0/tests/data/resource/samples/JGroups/licenses/cpl-1.0.txt`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/tests/data/resource/samples/JGroups/licenses/lgpl.txt` & `commoncode-31.1.0/tests/data/resource/samples/JGroups/licenses/lgpl.txt`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/tests/data/resource/samples/JGroups/src/FixedMembershipToken.java` & `commoncode-31.1.0/tests/data/resource/samples/JGroups/src/FixedMembershipToken.java`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/tests/data/resource/samples/JGroups/src/GuardedBy.java` & `commoncode-31.1.0/tests/data/resource/samples/JGroups/src/GuardedBy.java`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/tests/data/resource/samples/JGroups/src/ImmutableReference.java` & `commoncode-31.1.0/tests/data/resource/samples/JGroups/src/ImmutableReference.java`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/tests/data/resource/samples/JGroups/src/RATE_LIMITER.java` & `commoncode-31.1.0/tests/data/resource/samples/JGroups/src/RATE_LIMITER.java`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/tests/data/resource/samples/JGroups/src/RouterStub.java` & `commoncode-31.1.0/tests/data/resource/samples/JGroups/src/RouterStub.java`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/tests/data/resource/samples/JGroups/src/RouterStubManager.java` & `commoncode-31.1.0/tests/data/resource/samples/JGroups/src/RouterStubManager.java`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/tests/data/resource/samples/JGroups/src/S3_PING.java` & `commoncode-31.1.0/tests/data/resource/samples/JGroups/src/S3_PING.java`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/tests/data/resource/samples/arch/zlib.tar.gz` & `commoncode-31.1.0/tests/data/resource/samples/arch/zlib.tar.gz`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/tests/data/resource/samples/screenshot.png` & `commoncode-31.1.0/tests/data/resource/samples/screenshot.png`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/tests/data/resource/samples/zlib/ada/zlib.ads` & `commoncode-31.1.0/tests/data/resource/samples/zlib/ada/zlib.ads`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/tests/data/resource/samples/zlib/adler32.c` & `commoncode-31.1.0/tests/data/resource/samples/zlib/adler32.c`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/tests/data/resource/samples/zlib/deflate.c` & `commoncode-31.1.0/tests/data/resource/samples/zlib/deflate.c`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/tests/data/resource/samples/zlib/deflate.h` & `commoncode-31.1.0/tests/data/resource/samples/zlib/deflate.h`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/tests/data/resource/samples/zlib/dotzlib/AssemblyInfo.cs` & `commoncode-31.1.0/tests/data/resource/samples/zlib/dotzlib/AssemblyInfo.cs`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/tests/data/resource/samples/zlib/dotzlib/ChecksumImpl.cs` & `commoncode-31.1.0/tests/data/resource/samples/zlib/dotzlib/ChecksumImpl.cs`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/tests/data/resource/samples/zlib/dotzlib/LICENSE_1_0.txt` & `commoncode-31.1.0/tests/data/resource/samples/zlib/dotzlib/LICENSE_1_0.txt`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/tests/data/resource/samples/zlib/dotzlib/readme.txt` & `commoncode-31.1.0/tests/data/resource/samples/zlib/dotzlib/readme.txt`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/tests/data/resource/samples/zlib/gcc_gvmat64/gvmat64.S` & `commoncode-31.1.0/tests/data/resource/samples/zlib/gcc_gvmat64/gvmat64.S`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/tests/data/resource/samples/zlib/infback9/infback9.c` & `commoncode-31.1.0/tests/data/resource/samples/zlib/infback9/infback9.c`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/tests/data/resource/samples/zlib/infback9/infback9.h` & `commoncode-31.1.0/tests/data/resource/samples/zlib/infback9/infback9.h`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/tests/data/resource/samples/zlib/iostream2/zstream.h` & `commoncode-31.1.0/tests/data/resource/samples/zlib/iostream2/zstream.h`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/tests/data/resource/samples/zlib/iostream2/zstream_test.cpp` & `commoncode-31.1.0/tests/data/resource/samples/zlib/iostream2/zstream_test.cpp`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/tests/data/resource/samples/zlib/zlib.h` & `commoncode-31.1.0/tests/data/resource/samples/zlib/zlib.h`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/tests/data/resource/samples/zlib/zutil.c` & `commoncode-31.1.0/tests/data/resource/samples/zlib/zutil.c`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/tests/data/resource/samples/zlib/zutil.h` & `commoncode-31.1.0/tests/data/resource/samples/zlib/zutil.h`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/tests/data/resource/virtual_codebase/codebase-for-cache-tests.json` & `commoncode-31.1.0/tests/data/resource/virtual_codebase/codebase-for-cache-tests.json`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/tests/data/resource/virtual_codebase/combine-expected.json` & `commoncode-31.1.0/tests/data/resource/virtual_codebase/combine-expected.json`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/tests/data/resource/virtual_codebase/combine-shared-directory-name-1.json` & `commoncode-31.1.0/tests/data/resource/virtual_codebase/combine-shared-directory-name-1.json`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/tests/data/resource/virtual_codebase/combine-shared-directory-name-2.json` & `commoncode-31.1.0/tests/data/resource/virtual_codebase/combine-shared-directory-name-2.json`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/tests/data/resource/virtual_codebase/combine-shared-directory-name-expected.json` & `commoncode-31.1.0/tests/data/resource/virtual_codebase/combine-shared-directory-name-expected.json`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/tests/data/resource/virtual_codebase/docker-hello-world.json` & `commoncode-31.1.0/tests/data/resource/virtual_codebase/docker-hello-world.json`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/tests/data/resource/virtual_codebase/et131x.h.json` & `commoncode-31.1.0/tests/data/resource/virtual_codebase/et131x.h.json`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/tests/data/resource/virtual_codebase/fingerprint_attribute.json` & `commoncode-31.1.0/tests/data/resource/virtual_codebase/fingerprint_attribute.json`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/tests/data/resource/virtual_codebase/full-root-info-many-expected.json` & `commoncode-31.1.0/tests/data/resource/virtual_codebase/full-root-info-many-expected.json`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/tests/data/resource/virtual_codebase/full-root-info-many.json` & `commoncode-31.1.0/tests/data/resource/virtual_codebase/full-root-info-many.json`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/tests/data/resource/virtual_codebase/full-root-info-one-expected.json` & `commoncode-31.1.0/tests/data/resource/virtual_codebase/full-root-info-one-expected.json`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/tests/data/resource/virtual_codebase/full-root-info-one.json` & `commoncode-31.1.0/tests/data/resource/virtual_codebase/full-root-info-one.json`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/tests/data/resource/virtual_codebase/lcp.json` & `commoncode-31.1.0/tests/data/resource/virtual_codebase/lcp.json`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/tests/data/resource/virtual_codebase/license-scan.json` & `commoncode-31.1.0/tests/data/resource/virtual_codebase/license-scan.json`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/tests/data/resource/virtual_codebase/node-16-slim.json` & `commoncode-31.1.0/tests/data/resource/virtual_codebase/node-16-slim.json`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/tests/data/resource/virtual_codebase/resource.json` & `commoncode-31.1.0/tests/data/resource/virtual_codebase/resource.json`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/tests/data/resource/virtual_codebase/samples-only-findings-expected.json` & `commoncode-31.1.0/tests/data/resource/virtual_codebase/samples-only-findings-expected.json`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/tests/data/resource/virtual_codebase/samples-only-findings.json` & `commoncode-31.1.0/tests/data/resource/virtual_codebase/samples-only-findings.json`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/tests/data/resource/virtual_codebase/virtual_codebase.json` & `commoncode-31.1.0/tests/data/resource/virtual_codebase/virtual_codebase.json`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/tests/data/resource/virtual_codebase/zephyr-binary.json` & `commoncode-31.1.0/tests/data/resource/virtual_codebase/zephyr-binary.json`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/tests/data/resource/with_path/codebase/et131x.h` & `commoncode-31.1.0/tests/data/resource/with_path/codebase/et131x.h`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/tests/data/resource/with_path/virtual-codebase.json` & `commoncode-31.1.0/tests/data/resource/with_path/virtual-codebase.json`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/tests/data/saneyaml/metadata1` & `commoncode-31.1.0/tests/data/saneyaml/metadata1`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/tests/data/saneyaml/metadata1.notag` & `commoncode-31.1.0/tests/data/saneyaml/metadata1.notag`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/tests/test_cliutils.py` & `commoncode-31.1.0/tests/test_cliutils.py`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/tests/test_cliutils_progressbar.py` & `commoncode-31.1.0/tests/test_cliutils_progressbar.py`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/tests/test_codec.py` & `commoncode-31.1.0/tests/test_codec.py`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/tests/test_command.py` & `commoncode-31.1.0/tests/test_command.py`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/tests/test_date.py` & `commoncode-31.1.0/tests/test_date.py`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/tests/test_fileset.py` & `commoncode-31.1.0/tests/test_fileset.py`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/tests/test_filetype.py` & `commoncode-31.1.0/tests/test_filetype.py`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/tests/test_fileutils.py` & `commoncode-31.1.0/tests/test_fileutils.py`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/tests/test_functional.py` & `commoncode-31.1.0/tests/test_functional.py`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/tests/test_hash.py` & `commoncode-31.1.0/tests/test_hash.py`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/tests/test_ignore.py` & `commoncode-31.1.0/tests/test_ignore.py`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/tests/test_paths.py` & `commoncode-31.1.0/tests/test_paths.py`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/tests/test_resource.py` & `commoncode-31.1.0/tests/test_resource.py`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/tests/test_saneyaml.py` & `commoncode-31.1.0/tests/test_saneyaml.py`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/tests/test_skeleton_codestyle.py` & `commoncode-31.1.0/tests/test_skeleton_codestyle.py`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/tests/test_text.py` & `commoncode-31.1.0/tests/test_text.py`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/tests/test_timeutils.py` & `commoncode-31.1.0/tests/test_timeutils.py`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/tests/test_urn.py` & `commoncode-31.1.0/tests/test_urn.py`

 * *Files identical despite different names*

### Comparing `commoncode-31.0.3/tests/test_version.py` & `commoncode-31.1.0/tests/test_version.py`

 * *Files identical despite different names*

