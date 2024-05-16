# Comparing `tmp/mio-cli-1.3.5.tar.gz` & `tmp/mio-cli-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/homes/dpoulin/git/mio_cli_client/dist/tmpigjiup5a/mio-cli-1.3.5.tar", last modified: Wed Dec 13 22:04:05 2023, max compression
+gzip compressed data, was "/homes/dpoulin/git/mio_cli_client/dist/tmphzu0tw27/mio-cli-1.3.6.tar", last modified: Thu Dec 21 01:52:57 2023, max compression
```

## Comparing `mio-cli-1.3.5.tar` & `mio-cli-1.3.6.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxrwxr-x   0 dpoulin   (1000) dpoulin   (1004)        0 2023-12-13 22:04:04.000000 mio-cli-1.3.5/
-drwxrwxr-x   0 dpoulin   (1000) dpoulin   (1004)        0 2023-12-13 22:04:04.000000 mio-cli-1.3.5/src/
-drwxrwxr-x   0 dpoulin   (1000) dpoulin   (1004)        0 2023-12-13 22:04:04.000000 mio-cli-1.3.5/src/data/
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      207 2023-02-20 21:32:40.000000 mio-cli-1.3.5/src/data/__init__.py
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     4923 2022-06-16 19:18:56.000000 mio-cli-1.3.5/src/data/doxygen-awesome-darkmode-toggle.js
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     1466 2022-06-16 19:18:55.000000 mio-cli-1.3.5/src/data/doxygen-awesome-sidebar-only-darkmode-toggle.css
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     3068 2022-06-16 19:18:55.000000 mio-cli-1.3.5/src/data/doxygen-awesome-sidebar-only.css
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    35619 2022-09-03 16:25:11.000000 mio-cli-1.3.5/src/data/doxygen-awesome.css
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    99962 2022-07-15 15:15:38.000000 mio-cli-1.3.5/src/data/doxygen.awesome.cfg
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    99996 2023-03-13 18:57:01.000000 mio-cli-1.3.5/src/data/doxygen.private.cfg
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    99914 2022-09-02 20:28:49.000000 mio-cli-1.3.5/src/data/doxygen.public.cfg
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      579 2022-09-02 20:15:26.000000 mio-cli-1.3.5/src/data/doxygen_footer.html
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     2172 2022-09-03 03:28:48.000000 mio-cli-1.3.5/src/data/doxygen_header.awesome.html
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     2065 2022-06-16 19:18:55.000000 mio-cli-1.3.5/src/data/doxygen_header.html
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     5792 2023-03-13 18:50:26.000000 mio-cli-1.3.5/src/data/doxygen_layout.xml
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    23854 2022-06-16 19:18:56.000000 mio-cli-1.3.5/src/data/doxygen_stylesheet.css
--rwxrwxr-x   0 dpoulin   (1000) dpoulin   (1004)    40097 2022-06-16 19:18:56.000000 mio-cli-1.3.5/src/data/idv_doxyfilter_sv.pl
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      990 2023-05-16 18:43:16.000000 mio-cli-1.3.5/src/data/mio.toml
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)  8578435 2022-06-16 19:18:56.000000 mio-cli-1.3.5/src/data/plantuml.jar
-drwxrwxr-x   0 dpoulin   (1000) dpoulin   (1004)        0 2023-12-13 22:04:04.000000 mio-cli-1.3.5/src/mio/
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      232 2023-03-23 22:41:29.000000 mio-cli-1.3.5/src/mio/__init__.py
--rwxrwxr-x   0 dpoulin   (1000) dpoulin   (1004)      438 2023-02-20 21:32:40.000000 mio-cli-1.3.5/src/mio/__main__.py
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    49802 2023-09-24 04:09:30.000000 mio-cli-1.3.5/src/mio/cache.py
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     9149 2023-11-28 22:47:56.000000 mio-cli-1.3.5/src/mio/cfg.py
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     4429 2023-04-02 01:47:39.000000 mio-cli-1.3.5/src/mio/clean.py
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    22072 2023-11-28 22:41:48.000000 mio-cli-1.3.5/src/mio/cli.py
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     8094 2023-03-23 09:22:45.000000 mio-cli-1.3.5/src/mio/common.py
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     3767 2023-03-23 21:32:24.000000 mio-cli-1.3.5/src/mio/cov.py
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     1807 2023-02-20 21:32:41.000000 mio-cli-1.3.5/src/mio/doctor.py
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     3975 2023-03-13 19:10:51.000000 mio-cli-1.3.5/src/mio/dox.py
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    92084 2023-12-13 21:23:38.000000 mio-cli-1.3.5/src/mio/eal.py
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    12763 2023-11-28 22:40:29.000000 mio-cli-1.3.5/src/mio/help_text.py
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    10691 2023-03-08 21:25:16.000000 mio-cli-1.3.5/src/mio/init.py
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     8499 2023-03-08 18:46:00.000000 mio-cli-1.3.5/src/mio/install.py
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      424 2023-09-23 23:12:22.000000 mio-cli-1.3.5/src/mio/main.py
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     3278 2023-11-29 02:50:01.000000 mio-cli-1.3.5/src/mio/new.py
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    16616 2023-12-12 03:28:19.000000 mio-cli-1.3.5/src/mio/publish.py
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    35657 2023-11-21 19:42:20.000000 mio-cli-1.3.5/src/mio/regr.py
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    21762 2023-03-27 16:48:51.000000 mio-cli-1.3.5/src/mio/results.py
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    27745 2023-07-24 15:42:50.000000 mio-cli-1.3.5/src/mio/sim.py
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     5416 2023-02-20 21:32:42.000000 mio-cli-1.3.5/src/mio/user.py
-drwxrwxr-x   0 dpoulin   (1000) dpoulin   (1004)        0 2023-12-13 22:04:04.000000 mio-cli-1.3.5/src/mio_cli.egg-info/
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     3900 2023-12-13 22:04:04.000000 mio-cli-1.3.5/src/mio_cli.egg-info/PKG-INFO
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     1838 2023-12-13 22:04:04.000000 mio-cli-1.3.5/src/mio_cli.egg-info/SOURCES.txt
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)        1 2023-12-13 22:04:04.000000 mio-cli-1.3.5/src/mio_cli.egg-info/dependency_links.txt
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)       34 2023-12-13 22:04:04.000000 mio-cli-1.3.5/src/mio_cli.egg-info/entry_points.txt
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)        1 2022-11-30 18:59:49.000000 mio-cli-1.3.5/src/mio_cli.egg-info/not-zip-safe
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      155 2023-12-13 22:04:04.000000 mio-cli-1.3.5/src/mio_cli.egg-info/requires.txt
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)       19 2023-12-13 22:04:04.000000 mio-cli-1.3.5/src/mio_cli.egg-info/top_level.txt
-drwxrwxr-x   0 dpoulin   (1000) dpoulin   (1004)        0 2023-12-13 22:04:04.000000 mio-cli-1.3.5/src/templates/
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     3913 2021-10-06 01:07:11.000000 mio-cli-1.3.5/src/templates/LICENSE_solderpad_v2p1.md
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      207 2023-02-20 21:32:42.000000 mio-cli-1.3.5/src/templates/__init__.py
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     1228 2023-03-08 19:42:25.000000 mio-cli-1.3.5/src/templates/dv_ip.yml
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     3537 2023-04-02 01:43:15.000000 mio-cli-1.3.5/src/templates/interactive_results.html.j2
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      405 2022-12-22 03:35:11.000000 mio-cli-1.3.5/src/templates/mdc.flist.j2
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      412 2022-12-22 03:31:30.000000 mio-cli-1.3.5/src/templates/mdc.mflist.j2
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      285 2023-03-08 19:41:09.000000 mio-cli-1.3.5/src/templates/mio.toml
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)        4 2022-11-22 23:38:10.000000 mio-cli-1.3.5/src/templates/project_gitignore
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      407 2022-12-22 03:35:04.000000 mio-cli-1.3.5/src/templates/qst.flist.j2
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      426 2022-12-22 03:34:06.000000 mio-cli-1.3.5/src/templates/qst.mflist.j2
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     3873 2023-04-02 01:42:37.000000 mio-cli-1.3.5/src/templates/regression_results.html.j2
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      407 2022-12-22 03:34:58.000000 mio-cli-1.3.5/src/templates/riv.flist.j2
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      358 2022-12-22 03:32:40.000000 mio-cli-1.3.5/src/templates/riv.mflist.j2
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      839 2023-03-08 19:42:18.000000 mio-cli-1.3.5/src/templates/rtl_ip.yml
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)       26 2022-11-26 22:28:34.000000 mio-cli-1.3.5/src/templates/sim_gitignore
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      769 2023-03-12 23:53:13.000000 mio-cli-1.3.5/src/templates/ts.yml.j2
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      407 2022-12-22 03:34:52.000000 mio-cli-1.3.5/src/templates/vcs.flist.j2
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      358 2022-12-22 03:32:35.000000 mio-cli-1.3.5/src/templates/vcs.mflist.j2
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      392 2022-12-22 05:03:50.000000 mio-cli-1.3.5/src/templates/viv.flist.j2
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      347 2023-03-28 20:21:55.000000 mio-cli-1.3.5/src/templates/viv.mflist.j2
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      420 2022-12-22 05:08:01.000000 mio-cli-1.3.5/src/templates/viv.prj.j2
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      935 2023-03-08 19:42:00.000000 mio-cli-1.3.5/src/templates/vivado_ip.yml
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      407 2022-12-22 03:34:40.000000 mio-cli-1.3.5/src/templates/xcl.flist.j2
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      358 2022-12-22 03:32:17.000000 mio-cli-1.3.5/src/templates/xcl.mflist.j2
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    35208 2023-02-20 09:54:39.000000 mio-cli-1.3.5/LICENSE
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     3091 2023-06-21 22:37:21.000000 mio-cli-1.3.5/README.md
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      305 2022-07-26 18:06:36.000000 mio-cli-1.3.5/pyproject.toml
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     2148 2023-12-13 22:04:04.000000 mio-cli-1.3.5/setup.cfg
--rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     3900 2023-12-13 22:04:04.000000 mio-cli-1.3.5/PKG-INFO
+drwxrwxr-x   0 dpoulin   (1000) dpoulin   (1004)        0 2023-12-21 01:52:54.000000 mio-cli-1.3.6/
+drwxrwxr-x   0 dpoulin   (1000) dpoulin   (1004)        0 2023-12-21 01:52:54.000000 mio-cli-1.3.6/src/
+drwxrwxr-x   0 dpoulin   (1000) dpoulin   (1004)        0 2023-12-21 01:52:54.000000 mio-cli-1.3.6/src/data/
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      207 2023-02-20 21:32:40.000000 mio-cli-1.3.6/src/data/__init__.py
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     4923 2022-06-16 19:18:56.000000 mio-cli-1.3.6/src/data/doxygen-awesome-darkmode-toggle.js
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     1466 2022-06-16 19:18:55.000000 mio-cli-1.3.6/src/data/doxygen-awesome-sidebar-only-darkmode-toggle.css
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     3068 2022-06-16 19:18:55.000000 mio-cli-1.3.6/src/data/doxygen-awesome-sidebar-only.css
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    35619 2022-09-03 16:25:11.000000 mio-cli-1.3.6/src/data/doxygen-awesome.css
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    99962 2022-07-15 15:15:38.000000 mio-cli-1.3.6/src/data/doxygen.awesome.cfg
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    99996 2023-03-13 18:57:01.000000 mio-cli-1.3.6/src/data/doxygen.private.cfg
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    99914 2022-09-02 20:28:49.000000 mio-cli-1.3.6/src/data/doxygen.public.cfg
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      579 2022-09-02 20:15:26.000000 mio-cli-1.3.6/src/data/doxygen_footer.html
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     2172 2022-09-03 03:28:48.000000 mio-cli-1.3.6/src/data/doxygen_header.awesome.html
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     2065 2022-06-16 19:18:55.000000 mio-cli-1.3.6/src/data/doxygen_header.html
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     5792 2023-03-13 18:50:26.000000 mio-cli-1.3.6/src/data/doxygen_layout.xml
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    23854 2022-06-16 19:18:56.000000 mio-cli-1.3.6/src/data/doxygen_stylesheet.css
+-rwxrwxr-x   0 dpoulin   (1000) dpoulin   (1004)    40097 2022-06-16 19:18:56.000000 mio-cli-1.3.6/src/data/idv_doxyfilter_sv.pl
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      990 2023-05-16 18:43:16.000000 mio-cli-1.3.6/src/data/mio.toml
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)  8578435 2022-06-16 19:18:56.000000 mio-cli-1.3.6/src/data/plantuml.jar
+drwxrwxr-x   0 dpoulin   (1000) dpoulin   (1004)        0 2023-12-21 01:52:54.000000 mio-cli-1.3.6/src/mio/
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      232 2023-03-23 22:41:29.000000 mio-cli-1.3.6/src/mio/__init__.py
+-rwxrwxr-x   0 dpoulin   (1000) dpoulin   (1004)      438 2023-02-20 21:32:40.000000 mio-cli-1.3.6/src/mio/__main__.py
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    49802 2023-09-24 04:09:30.000000 mio-cli-1.3.6/src/mio/cache.py
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     9149 2023-11-28 22:47:56.000000 mio-cli-1.3.6/src/mio/cfg.py
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     4429 2023-04-02 01:47:39.000000 mio-cli-1.3.6/src/mio/clean.py
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    22072 2023-11-28 22:41:48.000000 mio-cli-1.3.6/src/mio/cli.py
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     8094 2023-03-23 09:22:45.000000 mio-cli-1.3.6/src/mio/common.py
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     3767 2023-03-23 21:32:24.000000 mio-cli-1.3.6/src/mio/cov.py
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     1807 2023-02-20 21:32:41.000000 mio-cli-1.3.6/src/mio/doctor.py
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     3975 2023-03-13 19:10:51.000000 mio-cli-1.3.6/src/mio/dox.py
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    92099 2023-12-20 00:50:19.000000 mio-cli-1.3.6/src/mio/eal.py
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    12763 2023-12-19 00:54:08.000000 mio-cli-1.3.6/src/mio/help_text.py
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    10691 2023-03-08 21:25:16.000000 mio-cli-1.3.6/src/mio/init.py
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     8499 2023-03-08 18:46:00.000000 mio-cli-1.3.6/src/mio/install.py
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      424 2023-09-23 23:12:22.000000 mio-cli-1.3.6/src/mio/main.py
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     3278 2023-11-29 02:50:01.000000 mio-cli-1.3.6/src/mio/new.py
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    16616 2023-12-12 03:28:19.000000 mio-cli-1.3.6/src/mio/publish.py
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    35657 2023-11-21 19:42:20.000000 mio-cli-1.3.6/src/mio/regr.py
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    21762 2023-03-27 16:48:51.000000 mio-cli-1.3.6/src/mio/results.py
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    27756 2023-12-20 00:50:33.000000 mio-cli-1.3.6/src/mio/sim.py
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     5416 2023-02-20 21:32:42.000000 mio-cli-1.3.6/src/mio/user.py
+drwxrwxr-x   0 dpoulin   (1000) dpoulin   (1004)        0 2023-12-21 01:52:54.000000 mio-cli-1.3.6/src/mio_cli.egg-info/
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     3900 2023-12-21 01:52:54.000000 mio-cli-1.3.6/src/mio_cli.egg-info/PKG-INFO
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     1838 2023-12-21 01:52:54.000000 mio-cli-1.3.6/src/mio_cli.egg-info/SOURCES.txt
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)        1 2023-12-21 01:52:54.000000 mio-cli-1.3.6/src/mio_cli.egg-info/dependency_links.txt
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)       34 2023-12-21 01:52:54.000000 mio-cli-1.3.6/src/mio_cli.egg-info/entry_points.txt
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)        1 2022-11-30 18:59:49.000000 mio-cli-1.3.6/src/mio_cli.egg-info/not-zip-safe
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      155 2023-12-21 01:52:54.000000 mio-cli-1.3.6/src/mio_cli.egg-info/requires.txt
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)       19 2023-12-21 01:52:54.000000 mio-cli-1.3.6/src/mio_cli.egg-info/top_level.txt
+drwxrwxr-x   0 dpoulin   (1000) dpoulin   (1004)        0 2023-12-21 01:52:54.000000 mio-cli-1.3.6/src/templates/
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     3913 2021-10-06 01:07:11.000000 mio-cli-1.3.6/src/templates/LICENSE_solderpad_v2p1.md
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      207 2023-02-20 21:32:42.000000 mio-cli-1.3.6/src/templates/__init__.py
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     1228 2023-03-08 19:42:25.000000 mio-cli-1.3.6/src/templates/dv_ip.yml
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     3537 2023-04-02 01:43:15.000000 mio-cli-1.3.6/src/templates/interactive_results.html.j2
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      405 2022-12-22 03:35:11.000000 mio-cli-1.3.6/src/templates/mdc.flist.j2
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      412 2022-12-22 03:31:30.000000 mio-cli-1.3.6/src/templates/mdc.mflist.j2
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      285 2023-03-08 19:41:09.000000 mio-cli-1.3.6/src/templates/mio.toml
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)        4 2022-11-22 23:38:10.000000 mio-cli-1.3.6/src/templates/project_gitignore
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      407 2022-12-22 03:35:04.000000 mio-cli-1.3.6/src/templates/qst.flist.j2
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      426 2022-12-22 03:34:06.000000 mio-cli-1.3.6/src/templates/qst.mflist.j2
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     3873 2023-04-02 01:42:37.000000 mio-cli-1.3.6/src/templates/regression_results.html.j2
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      407 2022-12-22 03:34:58.000000 mio-cli-1.3.6/src/templates/riv.flist.j2
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      358 2022-12-22 03:32:40.000000 mio-cli-1.3.6/src/templates/riv.mflist.j2
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      839 2023-03-08 19:42:18.000000 mio-cli-1.3.6/src/templates/rtl_ip.yml
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)       26 2022-11-26 22:28:34.000000 mio-cli-1.3.6/src/templates/sim_gitignore
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      769 2023-03-12 23:53:13.000000 mio-cli-1.3.6/src/templates/ts.yml.j2
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      407 2022-12-22 03:34:52.000000 mio-cli-1.3.6/src/templates/vcs.flist.j2
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      358 2022-12-22 03:32:35.000000 mio-cli-1.3.6/src/templates/vcs.mflist.j2
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      392 2022-12-22 05:03:50.000000 mio-cli-1.3.6/src/templates/viv.flist.j2
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      347 2023-03-28 20:21:55.000000 mio-cli-1.3.6/src/templates/viv.mflist.j2
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      420 2022-12-22 05:08:01.000000 mio-cli-1.3.6/src/templates/viv.prj.j2
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      935 2023-03-08 19:42:00.000000 mio-cli-1.3.6/src/templates/vivado_ip.yml
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      407 2022-12-22 03:34:40.000000 mio-cli-1.3.6/src/templates/xcl.flist.j2
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      358 2022-12-22 03:32:17.000000 mio-cli-1.3.6/src/templates/xcl.mflist.j2
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)    35208 2023-02-20 09:54:39.000000 mio-cli-1.3.6/LICENSE
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     3091 2023-06-21 22:37:21.000000 mio-cli-1.3.6/README.md
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)      305 2022-07-26 18:06:36.000000 mio-cli-1.3.6/pyproject.toml
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     2148 2023-12-21 01:52:54.000000 mio-cli-1.3.6/setup.cfg
+-rw-rw-r--   0 dpoulin   (1000) dpoulin   (1004)     3900 2023-12-21 01:52:54.000000 mio-cli-1.3.6/PKG-INFO
```

### Comparing `mio-cli-1.3.5/src/data/doxygen-awesome-darkmode-toggle.js` & `mio-cli-1.3.6/src/data/doxygen-awesome-darkmode-toggle.js`

 * *Files identical despite different names*

### Comparing `mio-cli-1.3.5/src/data/doxygen-awesome-sidebar-only-darkmode-toggle.css` & `mio-cli-1.3.6/src/data/doxygen-awesome-sidebar-only-darkmode-toggle.css`

 * *Files identical despite different names*

### Comparing `mio-cli-1.3.5/src/data/doxygen-awesome-sidebar-only.css` & `mio-cli-1.3.6/src/data/doxygen-awesome-sidebar-only.css`

 * *Files identical despite different names*

### Comparing `mio-cli-1.3.5/src/data/doxygen-awesome.css` & `mio-cli-1.3.6/src/data/doxygen-awesome.css`

 * *Files identical despite different names*

### Comparing `mio-cli-1.3.5/src/data/doxygen.awesome.cfg` & `mio-cli-1.3.6/src/data/doxygen.awesome.cfg`

 * *Files identical despite different names*

### Comparing `mio-cli-1.3.5/src/data/doxygen.private.cfg` & `mio-cli-1.3.6/src/data/doxygen.private.cfg`

 * *Files identical despite different names*

### Comparing `mio-cli-1.3.5/src/data/doxygen.public.cfg` & `mio-cli-1.3.6/src/data/doxygen.public.cfg`

 * *Files identical despite different names*

### Comparing `mio-cli-1.3.5/src/data/doxygen_footer.html` & `mio-cli-1.3.6/src/data/doxygen_footer.html`

 * *Files identical despite different names*

### Comparing `mio-cli-1.3.5/src/data/doxygen_header.awesome.html` & `mio-cli-1.3.6/src/data/doxygen_header.awesome.html`

 * *Files identical despite different names*

### Comparing `mio-cli-1.3.5/src/data/doxygen_header.html` & `mio-cli-1.3.6/src/data/doxygen_header.html`

 * *Files identical despite different names*

### Comparing `mio-cli-1.3.5/src/data/doxygen_layout.xml` & `mio-cli-1.3.6/src/data/doxygen_layout.xml`

 * *Files identical despite different names*

### Comparing `mio-cli-1.3.5/src/data/doxygen_stylesheet.css` & `mio-cli-1.3.6/src/data/doxygen_stylesheet.css`

 * *Files identical despite different names*

### Comparing `mio-cli-1.3.5/src/data/idv_doxyfilter_sv.pl` & `mio-cli-1.3.6/src/data/idv_doxyfilter_sv.pl`

 * *Files identical despite different names*

### Comparing `mio-cli-1.3.5/src/data/mio.toml` & `mio-cli-1.3.6/src/data/mio.toml`

 * *Files identical despite different names*

### Comparing `mio-cli-1.3.5/src/data/plantuml.jar` & `mio-cli-1.3.6/src/data/plantuml.jar`

 * *Files identical despite different names*

### Comparing `mio-cli-1.3.5/src/mio/cache.py` & `mio-cli-1.3.6/src/mio/cache.py`

 * *Files identical despite different names*

### Comparing `mio-cli-1.3.5/src/mio/cfg.py` & `mio-cli-1.3.6/src/mio/cfg.py`

 * *Files identical despite different names*

### Comparing `mio-cli-1.3.5/src/mio/clean.py` & `mio-cli-1.3.6/src/mio/clean.py`

 * *Files identical despite different names*

### Comparing `mio-cli-1.3.5/src/mio/cli.py` & `mio-cli-1.3.6/src/mio/cli.py`

 * *Files identical despite different names*

### Comparing `mio-cli-1.3.5/src/mio/common.py` & `mio-cli-1.3.6/src/mio/common.py`

 * *Files identical despite different names*

### Comparing `mio-cli-1.3.5/src/mio/cov.py` & `mio-cli-1.3.6/src/mio/cov.py`

 * *Files identical despite different names*

### Comparing `mio-cli-1.3.5/src/mio/doctor.py` & `mio-cli-1.3.6/src/mio/doctor.py`

 * *Files identical despite different names*

### Comparing `mio-cli-1.3.5/src/mio/dox.py` & `mio-cli-1.3.6/src/mio/dox.py`

 * *Files identical despite different names*

### Comparing `mio-cli-1.3.5/src/mio/eal.py` & `mio-cli-1.3.6/src/mio/eal.py`

 * *Files 0% similar despite different names*

```diff
@@ -894,15 +894,15 @@
                     f.close()
                 except Exception as e:
                     common.fatal("Could not create wave capture script at " + wave_capture_script_path + ": " + str(e))
         elif sim_job.simulator == common.simulators_enum.VCS:
             # TODO Implement waves file for vcs
             pass
         elif sim_job.simulator == common.simulators_enum.METRICS:
-            arg_list.append(f"-waves {test_result_dir}.vcd")
+            arg_list.append(f"-waves {test_result_dir}.vcd.gz")
         elif sim_job.simulator == common.simulators_enum.XCELIUM:
             # TODO Implement waves file for xcelium
             pass
         elif sim_job.simulator == common.simulators_enum.QUESTA:
             # TODO Implement waves file for questa
             pass
         elif sim_job.simulator == common.simulators_enum.RIVIERA:
@@ -1013,18 +1013,18 @@
         sim_job.bwrap_commands += launch_eda_bin(cfg.metrics_home + "/mdc", arg_list, wd=cfg.project_dir, output=output, dry_run=sim_job.dry_run)
         common.remove_file(f"{cfg.project_dir}/_downloaded_{mtr_simulation_log_path}")
         common.info("Downloading simulation log ...")
         sim_job.bwrap_commands += launch_eda_bin(cfg.metrics_home + "/mdc", ["download", mtr_simulation_log_path], wd=cfg.project_dir, dry_run=sim_job.dry_run)
         if not sim_job.dry_run:
             common.move_file(f"{cfg.project_dir}/_downloaded_{mtr_simulation_log_path}", simulation_log_path)
             if sim_job.waves:
-                common.remove_file(f"{cfg.project_dir}/_downloaded_{test_result_dir}.vcd")
+                common.remove_file(f"{cfg.project_dir}/_downloaded_{test_result_dir}.vcd.gz")
                 common.info("Downloading simulation waveforms ...")
-                sim_job.bwrap_commands += launch_eda_bin(cfg.metrics_home + "/mdc", ["download", f"{test_result_dir}.vcd"], wd=cfg.project_dir, dry_run=sim_job.dry_run)
-                common.move_file(f"{cfg.project_dir}/_downloaded_{test_result_dir}.vcd", f"{tests_results_path}/waves.vcd")
+                sim_job.bwrap_commands += launch_eda_bin(cfg.metrics_home + "/mdc", ["download", f"{test_result_dir}.vcd.gz"], wd=cfg.project_dir, dry_run=sim_job.dry_run)
+                common.move_file(f"{cfg.project_dir}/_downloaded_{test_result_dir}.vcd.gz", f"{tests_results_path}/waves.vcd.gz")
             common.remove_file(f"{cfg.project_dir}/_downloaded_prism.data")
             common.info("Downloading simulation data ...")
             sim_job.bwrap_commands += launch_eda_bin(cfg.metrics_home + "/mdc", ["download", prism_data_path], wd=cfg.project_dir, dry_run=sim_job.dry_run)
             common.move_file(prism_data_downloaded_path, f"{tests_results_path}/prism.data")
             download_uvmx_logs_mdc(sim_job, mdc_tests_results_path, tests_results_path)
         
     elif sim_job.simulator == common.simulators_enum.XCELIUM:
```

### Comparing `mio-cli-1.3.5/src/mio/help_text.py` & `mio-cli-1.3.6/src/mio/help_text.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Copyright 2021-2023 Datum Technology Corporation
 # SPDX-License-Identifier: GPL-3.0
 ########################################################################################################################
 
 
-version = "1.3.5"
+version = "1.3.6"
 version_text = f"Moore.io CLI Client v{version}"
 
 
 
 main_help_text = f"""
                                  Moore.io (`mio`) Command Line Interface (CLI) - v{version}
                                       User Manual: https://mio-cli.readthedocs.io/
```

### Comparing `mio-cli-1.3.5/src/mio/init.py` & `mio-cli-1.3.6/src/mio/init.py`

 * *Files identical despite different names*

### Comparing `mio-cli-1.3.5/src/mio/install.py` & `mio-cli-1.3.6/src/mio/install.py`

 * *Files identical despite different names*

### Comparing `mio-cli-1.3.5/src/mio/new.py` & `mio-cli-1.3.6/src/mio/new.py`

 * *Files identical despite different names*

### Comparing `mio-cli-1.3.5/src/mio/publish.py` & `mio-cli-1.3.6/src/mio/publish.py`

 * *Files identical despite different names*

### Comparing `mio-cli-1.3.5/src/mio/regr.py` & `mio-cli-1.3.6/src/mio/regr.py`

 * *Files identical despite different names*

### Comparing `mio-cli-1.3.5/src/mio/results.py` & `mio-cli-1.3.6/src/mio/results.py`

 * *Files identical despite different names*

### Comparing `mio-cli-1.3.5/src/mio/sim.py` & `mio-cli-1.3.6/src/mio/sim.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 import tarfile
 
 
 
 
 bwrap_ignore_list = [
     "xsim.dir", ".str", ".Xil", ".jou", ".log", ".wdb", ".vcd", ".log", ".sdb", ".rlx", ".pb", ".o", ".png", ".jpg",
-    ".svg", ".vsdx", ".docx", ".xlsx", ".pptx", ".md", "sync", "workspace"
+    ".svg", ".vsdx", ".docx", ".xlsx", ".pptx", ".md", "sync", "workspace", ".fst"
 ]
 
 bwrap_ignore_dirs = [ ".git", ".svn" ]
 
 regex_define_pattern  = "\+define\+((?:\w|_|\d)+)(?:\=((?:\w|_|\d)+))?"
 regex_plusarg_pattern = "\+((?:\w|_|\d)+)(?:\=((?:\w|_|\d)+))?"
 seconds_waited = 0
@@ -571,15 +571,15 @@
     common.info("************************************************************************************************************************")
     if (sim_job.waves):
         if sim_job.simulator == common.simulators_enum.VIVADO:
             common.info("* Waveforms: $MIO_VIVADO_HOME/xsim -gui " + results_path + "/waves.wdb &")
         elif sim_job.simulator == common.simulators_enum.VCS:
             common.info("* Waveforms: $MIO_VCS_HOME/dve -gui " + results_path + "/waves.wdb &")
         elif sim_job.simulator == common.simulators_enum.METRICS:
-            common.info(f"* Waveforms: gtkwave {results_path}/waves.vcd &")
+            common.info(f"* Waveforms: gtkwave {results_path}/waves.vcd.gz &")
         elif sim_job.simulator == common.simulators_enum.XCELIUM:
             common.info("* Waveforms: $MIO_XCELIUM_HOME/simvision -gui " + results_path + "/waves.wdb &")
         elif sim_job.simulator == common.simulators_enum.QUESTA:
             common.info("* Waveforms: $MIO_QUESTA_HOME/visualizer -gui " + results_path + "/waves.wdb &")
         elif sim_job.simulator == common.simulators_enum.RIVIERA:
             common.info("* Waveforms: $MIO_RIVIERA_HOME/??? -gui " + results_path + "/waves.wdb &")
         common.info("")
```

### Comparing `mio-cli-1.3.5/src/mio/user.py` & `mio-cli-1.3.6/src/mio/user.py`

 * *Files identical despite different names*

### Comparing `mio-cli-1.3.5/src/mio_cli.egg-info/PKG-INFO` & `mio-cli-1.3.6/src/mio_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mio-cli
-Version: 1.3.5
+Version: 1.3.6
 Summary: The Moore.io Command Line Interface (CLI) Client is a toolchain for front-end engineering of FPGA/ASIC projects.
 Home-page: https://datum-technology-corporation.github.io/mio_cli_client/
 Author: Datum Technology Corporation
 Author-email: mio@datumtc.ca
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/Datum-Technology-Corporation/mio_cli_client/issues
 Keywords: SystemVerilog,UVM,DV,verilog,VHDL,hdl,rtl,synthesis,FPGA,simulation,Xilinx,Altera
```

### Comparing `mio-cli-1.3.5/src/mio_cli.egg-info/SOURCES.txt` & `mio-cli-1.3.6/src/mio_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mio-cli-1.3.5/src/templates/LICENSE_solderpad_v2p1.md` & `mio-cli-1.3.6/src/templates/LICENSE_solderpad_v2p1.md`

 * *Files identical despite different names*

### Comparing `mio-cli-1.3.5/src/templates/dv_ip.yml` & `mio-cli-1.3.6/src/templates/dv_ip.yml`

 * *Files identical despite different names*

### Comparing `mio-cli-1.3.5/src/templates/interactive_results.html.j2` & `mio-cli-1.3.6/src/templates/interactive_results.html.j2`

 * *Files identical despite different names*

### Comparing `mio-cli-1.3.5/src/templates/regression_results.html.j2` & `mio-cli-1.3.6/src/templates/regression_results.html.j2`

 * *Files identical despite different names*

### Comparing `mio-cli-1.3.5/src/templates/rtl_ip.yml` & `mio-cli-1.3.6/src/templates/rtl_ip.yml`

 * *Files identical despite different names*

### Comparing `mio-cli-1.3.5/src/templates/ts.yml.j2` & `mio-cli-1.3.6/src/templates/ts.yml.j2`

 * *Files identical despite different names*

### Comparing `mio-cli-1.3.5/src/templates/vivado_ip.yml` & `mio-cli-1.3.6/src/templates/vivado_ip.yml`

 * *Files identical despite different names*

### Comparing `mio-cli-1.3.5/LICENSE` & `mio-cli-1.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mio-cli-1.3.5/README.md` & `mio-cli-1.3.6/README.md`

 * *Files identical despite different names*

### Comparing `mio-cli-1.3.5/setup.cfg` & `mio-cli-1.3.6/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = mio-cli
-version = 1.3.5
+version = 1.3.6
 author = Datum Technology Corporation
 author_email = mio@datumtc.ca
 description = The Moore.io Command Line Interface (CLI) Client is a toolchain for front-end engineering of FPGA/ASIC projects.
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = SystemVerilog, UVM, DV, verilog, VHDL, hdl, rtl, synthesis, FPGA, simulation, Xilinx, Altera
 url = https://datum-technology-corporation.github.io/mio_cli_client/
```

### Comparing `mio-cli-1.3.5/PKG-INFO` & `mio-cli-1.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mio-cli
-Version: 1.3.5
+Version: 1.3.6
 Summary: The Moore.io Command Line Interface (CLI) Client is a toolchain for front-end engineering of FPGA/ASIC projects.
 Home-page: https://datum-technology-corporation.github.io/mio_cli_client/
 Author: Datum Technology Corporation
 Author-email: mio@datumtc.ca
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/Datum-Technology-Corporation/mio_cli_client/issues
 Keywords: SystemVerilog,UVM,DV,verilog,VHDL,hdl,rtl,synthesis,FPGA,simulation,Xilinx,Altera
```

