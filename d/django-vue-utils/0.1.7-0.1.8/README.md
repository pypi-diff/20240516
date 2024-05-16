# Comparing `tmp/django-vue-utils-0.1.7.tar.gz` & `tmp/django-vue-utils-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-vue-utils-0.1.7.tar", last modified: Tue Oct  3 09:29:35 2023, max compression
+gzip compressed data, was "django-vue-utils-0.1.8.tar", last modified: Thu May 16 05:40:10 2024, max compression
```

## Comparing `django-vue-utils-0.1.7.tar` & `django-vue-utils-0.1.8.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-10-03 09:29:35.653299 django-vue-utils-0.1.7/
--rw-rw-r--   0 mike      (1000) mike      (1000)     1080 2023-09-29 13:02:46.000000 django-vue-utils-0.1.7/LICENSE
--rw-rw-r--   0 mike      (1000) mike      (1000)       78 2023-09-29 15:05:56.000000 django-vue-utils-0.1.7/MANIFEST.in
--rw-r--r--   0 mike      (1000) mike      (1000)     2604 2023-10-03 09:29:35.653299 django-vue-utils-0.1.7/PKG-INFO
--rw-rw-r--   0 mike      (1000) mike      (1000)     1718 2023-10-03 09:28:58.000000 django-vue-utils-0.1.7/README.rst
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-10-03 09:29:35.629299 django-vue-utils-0.1.7/django_vue_utilities/
--rw-rw-r--   0 mike      (1000) mike      (1000)        0 2023-09-29 12:46:51.000000 django-vue-utils-0.1.7/django_vue_utilities/__init__.py
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-10-03 09:29:35.629299 django-vue-utils-0.1.7/django_vue_utilities/templatetags/
--rw-rw-r--   0 mike      (1000) mike      (1000)        0 2023-09-29 12:48:08.000000 django-vue-utils-0.1.7/django_vue_utilities/templatetags/__init__.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     1875 2023-09-29 14:57:49.000000 django-vue-utils-0.1.7/django_vue_utilities/templatetags/vue_utils.py
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-10-03 09:29:35.629299 django-vue-utils-0.1.7/django_vue_utilities/tests/
--rw-rw-r--   0 mike      (1000) mike      (1000)     5152 2023-09-29 14:59:12.000000 django-vue-utils-0.1.7/django_vue_utilities/tests/__init__.py
--rw-rw-r--   0 mike      (1000) mike      (1000)      495 2023-09-29 13:57:32.000000 django-vue-utils-0.1.7/django_vue_utilities/tests/settings.py
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-10-03 09:29:35.629299 django-vue-utils-0.1.7/django_vue_utils.egg-info/
--rw-r--r--   0 mike      (1000) mike      (1000)     2604 2023-10-03 09:29:35.000000 django-vue-utils-0.1.7/django_vue_utils.egg-info/PKG-INFO
--rw-rw-r--   0 mike      (1000) mike      (1000)     3127 2023-10-03 09:29:35.000000 django-vue-utils-0.1.7/django_vue_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 mike      (1000) mike      (1000)        1 2023-10-03 09:29:35.000000 django-vue-utils-0.1.7/django_vue_utils.egg-info/dependency_links.txt
--rw-rw-r--   0 mike      (1000) mike      (1000)       12 2023-10-03 09:29:35.000000 django-vue-utils-0.1.7/django_vue_utils.egg-info/requires.txt
--rw-rw-r--   0 mike      (1000) mike      (1000)       21 2023-10-03 09:29:35.000000 django-vue-utils-0.1.7/django_vue_utils.egg-info/top_level.txt
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-10-03 09:29:35.629299 django-vue-utils-0.1.7/docs/
--rw-rw-r--   0 mike      (1000) mike      (1000)     7662 2023-09-29 13:46:30.000000 django-vue-utils-0.1.7/docs/Makefile
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-10-03 09:29:35.625298 django-vue-utils-0.1.7/docs/_build/
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-10-03 09:29:35.633298 django-vue-utils-0.1.7/docs/_build/doctrees/
--rw-rw-r--   0 mike      (1000) mike      (1000)     8998 2023-09-29 13:52:33.000000 django-vue-utils-0.1.7/docs/_build/doctrees/documentation.doctree
--rw-rw-r--   0 mike      (1000) mike      (1000)    62045 2023-09-29 14:34:36.000000 django-vue-utils-0.1.7/docs/_build/doctrees/environment.pickle
--rw-rw-r--   0 mike      (1000) mike      (1000)    14365 2023-09-29 14:34:36.000000 django-vue-utils-0.1.7/docs/_build/doctrees/index.doctree
--rw-rw-r--   0 mike      (1000) mike      (1000)     6074 2023-09-29 13:52:33.000000 django-vue-utils-0.1.7/docs/_build/doctrees/install.doctree
--rw-rw-r--   0 mike      (1000) mike      (1000)     4091 2023-09-29 14:34:36.000000 django-vue-utils-0.1.7/docs/_build/doctrees/settings.doctree
--rw-rw-r--   0 mike      (1000) mike      (1000)     5070 2023-09-29 14:34:36.000000 django-vue-utils-0.1.7/docs/_build/doctrees/tests.doctree
--rw-rw-r--   0 mike      (1000) mike      (1000)     4476 2023-09-29 14:34:36.000000 django-vue-utils-0.1.7/docs/_build/doctrees/usage.doctree
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-10-03 09:29:35.633298 django-vue-utils-0.1.7/docs/_build/html/
--rw-rw-r--   0 mike      (1000) mike      (1000)      230 2023-09-29 14:34:36.000000 django-vue-utils-0.1.7/docs/_build/html/.buildinfo
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-10-03 09:29:35.637298 django-vue-utils-0.1.7/docs/_build/html/_sources/
--rw-rw-r--   0 mike      (1000) mike      (1000)     1122 2023-09-29 13:42:59.000000 django-vue-utils-0.1.7/docs/_build/html/_sources/documentation.rst.txt
--rw-rw-r--   0 mike      (1000) mike      (1000)     1911 2023-09-29 14:34:50.000000 django-vue-utils-0.1.7/docs/_build/html/_sources/index.rst.txt
--rw-rw-r--   0 mike      (1000) mike      (1000)      615 2023-09-29 13:46:02.000000 django-vue-utils-0.1.7/docs/_build/html/_sources/install.rst.txt
--rw-rw-r--   0 mike      (1000) mike      (1000)      310 2023-09-29 14:34:21.000000 django-vue-utils-0.1.7/docs/_build/html/_sources/settings.rst.txt
--rw-rw-r--   0 mike      (1000) mike      (1000)      575 2023-09-29 14:24:07.000000 django-vue-utils-0.1.7/docs/_build/html/_sources/tests.rst.txt
--rw-rw-r--   0 mike      (1000) mike      (1000)      521 2023-09-30 08:51:42.000000 django-vue-utils-0.1.7/docs/_build/html/_sources/usage.rst.txt
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-10-03 09:29:35.637298 django-vue-utils-0.1.7/docs/_build/html/_static/
--rw-rw-r--   0 mike      (1000) mike      (1000)    15094 2023-09-29 14:34:36.000000 django-vue-utils-0.1.7/docs/_build/html/_static/basic.css
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-10-03 09:29:35.637298 django-vue-utils-0.1.7/docs/_build/html/_static/css/
--rw-rw-r--   0 mike      (1000) mike      (1000)     3229 2023-09-29 13:49:19.000000 django-vue-utils-0.1.7/docs/_build/html/_static/css/badge_only.css
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-10-03 09:29:35.649299 django-vue-utils-0.1.7/docs/_build/html/_static/css/fonts/
--rw-rw-r--   0 mike      (1000) mike      (1000)    87624 2023-09-29 13:49:19.000000 django-vue-utils-0.1.7/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff
--rw-rw-r--   0 mike      (1000) mike      (1000)    67312 2023-09-29 13:49:19.000000 django-vue-utils-0.1.7/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff2
--rw-rw-r--   0 mike      (1000) mike      (1000)    86288 2023-09-29 13:49:19.000000 django-vue-utils-0.1.7/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff
--rw-rw-r--   0 mike      (1000) mike      (1000)    66444 2023-09-29 13:49:19.000000 django-vue-utils-0.1.7/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff2
--rw-rw-r--   0 mike      (1000) mike      (1000)   165742 2023-09-29 13:49:19.000000 django-vue-utils-0.1.7/docs/_build/html/_static/css/fonts/fontawesome-webfont.eot
--rw-rw-r--   0 mike      (1000) mike      (1000)   444379 2023-09-29 13:49:19.000000 django-vue-utils-0.1.7/docs/_build/html/_static/css/fonts/fontawesome-webfont.svg
--rw-rw-r--   0 mike      (1000) mike      (1000)   165548 2023-09-29 13:49:19.000000 django-vue-utils-0.1.7/docs/_build/html/_static/css/fonts/fontawesome-webfont.ttf
--rw-rw-r--   0 mike      (1000) mike      (1000)    98024 2023-09-29 13:49:19.000000 django-vue-utils-0.1.7/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff
--rw-rw-r--   0 mike      (1000) mike      (1000)    77160 2023-09-29 13:49:19.000000 django-vue-utils-0.1.7/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff2
--rw-rw-r--   0 mike      (1000) mike      (1000)   323344 2023-09-29 13:49:19.000000 django-vue-utils-0.1.7/docs/_build/html/_static/css/fonts/lato-bold-italic.woff
--rw-rw-r--   0 mike      (1000) mike      (1000)   193308 2023-09-29 13:49:19.000000 django-vue-utils-0.1.7/docs/_build/html/_static/css/fonts/lato-bold-italic.woff2
--rw-rw-r--   0 mike      (1000) mike      (1000)   309728 2023-09-29 13:49:19.000000 django-vue-utils-0.1.7/docs/_build/html/_static/css/fonts/lato-bold.woff
--rw-rw-r--   0 mike      (1000) mike      (1000)   184912 2023-09-29 13:49:19.000000 django-vue-utils-0.1.7/docs/_build/html/_static/css/fonts/lato-bold.woff2
--rw-rw-r--   0 mike      (1000) mike      (1000)   328412 2023-09-29 13:49:19.000000 django-vue-utils-0.1.7/docs/_build/html/_static/css/fonts/lato-normal-italic.woff
--rw-rw-r--   0 mike      (1000) mike      (1000)   195704 2023-09-29 13:49:19.000000 django-vue-utils-0.1.7/docs/_build/html/_static/css/fonts/lato-normal-italic.woff2
--rw-rw-r--   0 mike      (1000) mike      (1000)   309192 2023-09-29 13:49:19.000000 django-vue-utils-0.1.7/docs/_build/html/_static/css/fonts/lato-normal.woff
--rw-rw-r--   0 mike      (1000) mike      (1000)   182708 2023-09-29 13:49:19.000000 django-vue-utils-0.1.7/docs/_build/html/_static/css/fonts/lato-normal.woff2
--rw-rw-r--   0 mike      (1000) mike      (1000)   135314 2023-09-29 13:49:19.000000 django-vue-utils-0.1.7/docs/_build/html/_static/css/theme.css
--rw-rw-r--   0 mike      (1000) mike      (1000)     4472 2023-09-29 13:21:24.000000 django-vue-utils-0.1.7/docs/_build/html/_static/doctools.js
--rw-rw-r--   0 mike      (1000) mike      (1000)      326 2023-09-29 14:34:36.000000 django-vue-utils-0.1.7/docs/_build/html/_static/documentation_options.js
--rw-rw-r--   0 mike      (1000) mike      (1000)      286 2023-09-29 13:21:24.000000 django-vue-utils-0.1.7/docs/_build/html/_static/file.png
-drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2023-10-03 09:29:35.653299 django-vue-utils-0.1.7/docs/_build/html/_static/js/
--rw-rw-r--   0 mike      (1000) mike      (1000)      934 2023-09-29 13:49:19.000000 django-vue-utils-0.1.7/docs/_build/html/_static/js/badge_only.js
--rw-rw-r--   0 mike      (1000) mike      (1000)     4370 2023-09-29 13:49:19.000000 django-vue-utils-0.1.7/docs/_build/html/_static/js/html5shiv-printshiv.min.js
--rw-rw-r--   0 mike      (1000) mike      (1000)     2734 2023-09-29 13:49:19.000000 django-vue-utils-0.1.7/docs/_build/html/_static/js/html5shiv.min.js
--rw-rw-r--   0 mike      (1000) mike      (1000)     5023 2023-09-29 13:49:19.000000 django-vue-utils-0.1.7/docs/_build/html/_static/js/theme.js
--rw-rw-r--   0 mike      (1000) mike      (1000)     4758 2023-09-29 14:34:36.000000 django-vue-utils-0.1.7/docs/_build/html/_static/language_data.js
--rw-rw-r--   0 mike      (1000) mike      (1000)       90 2023-09-29 13:21:24.000000 django-vue-utils-0.1.7/docs/_build/html/_static/minus.png
--rw-rw-r--   0 mike      (1000) mike      (1000)       90 2023-09-29 13:21:24.000000 django-vue-utils-0.1.7/docs/_build/html/_static/plus.png
--rw-rw-r--   0 mike      (1000) mike      (1000)     4929 2023-09-29 14:34:36.000000 django-vue-utils-0.1.7/docs/_build/html/_static/pygments.css
--rw-rw-r--   0 mike      (1000) mike      (1000)    18732 2023-09-29 13:21:24.000000 django-vue-utils-0.1.7/docs/_build/html/_static/searchtools.js
--rw-rw-r--   0 mike      (1000) mike      (1000)     5123 2023-09-29 13:21:24.000000 django-vue-utils-0.1.7/docs/_build/html/_static/sphinx_highlight.js
--rw-rw-r--   0 mike      (1000) mike      (1000)     6762 2023-09-30 12:44:18.000000 django-vue-utils-0.1.7/docs/_build/html/documentation.html
--rw-rw-r--   0 mike      (1000) mike      (1000)     4230 2023-09-29 14:34:36.000000 django-vue-utils-0.1.7/docs/_build/html/genindex.html
--rw-rw-r--   0 mike      (1000) mike      (1000)     8888 2023-09-29 14:34:36.000000 django-vue-utils-0.1.7/docs/_build/html/index.html
--rw-rw-r--   0 mike      (1000) mike      (1000)     6077 2023-09-29 13:52:33.000000 django-vue-utils-0.1.7/docs/_build/html/install.html
--rw-rw-r--   0 mike      (1000) mike      (1000)      384 2023-09-29 14:34:36.000000 django-vue-utils-0.1.7/docs/_build/html/objects.inv
--rw-rw-r--   0 mike      (1000) mike      (1000)     4108 2023-09-29 14:34:36.000000 django-vue-utils-0.1.7/docs/_build/html/py-modindex.html
--rw-rw-r--   0 mike      (1000) mike      (1000)     3941 2023-09-29 14:34:36.000000 django-vue-utils-0.1.7/docs/_build/html/search.html
--rw-rw-r--   0 mike      (1000) mike      (1000)     3766 2023-09-29 14:34:36.000000 django-vue-utils-0.1.7/docs/_build/html/searchindex.js
--rw-rw-r--   0 mike      (1000) mike      (1000)     4170 2023-09-29 14:34:36.000000 django-vue-utils-0.1.7/docs/_build/html/settings.html
--rw-rw-r--   0 mike      (1000) mike      (1000)     5561 2023-09-29 14:34:36.000000 django-vue-utils-0.1.7/docs/_build/html/tests.html
--rw-rw-r--   0 mike      (1000) mike      (1000)     6027 2023-09-29 14:34:36.000000 django-vue-utils-0.1.7/docs/_build/html/usage.html
--rw-rw-r--   0 mike      (1000) mike      (1000)     9340 2023-09-30 12:43:30.000000 django-vue-utils-0.1.7/docs/conf.py
--rw-rw-r--   0 mike      (1000) mike      (1000)     1110 2023-09-30 12:44:00.000000 django-vue-utils-0.1.7/docs/documentation.rst
--rw-rw-r--   0 mike      (1000) mike      (1000)     1841 2023-09-30 12:42:53.000000 django-vue-utils-0.1.7/docs/index.rst
--rw-rw-r--   0 mike      (1000) mike      (1000)      615 2023-09-29 13:46:02.000000 django-vue-utils-0.1.7/docs/install.rst
--rw-rw-r--   0 mike      (1000) mike      (1000)     7752 2023-09-30 12:43:03.000000 django-vue-utils-0.1.7/docs/make.bat
--rw-rw-r--   0 mike      (1000) mike      (1000)      326 2023-09-30 08:49:54.000000 django-vue-utils-0.1.7/docs/settings.rst
--rw-rw-r--   0 mike      (1000) mike      (1000)      571 2023-09-30 12:44:04.000000 django-vue-utils-0.1.7/docs/tests.rst
--rw-rw-r--   0 mike      (1000) mike      (1000)      521 2023-09-30 08:51:45.000000 django-vue-utils-0.1.7/docs/usage.rst
--rw-rw-r--   0 mike      (1000) mike      (1000)      270 2023-09-29 14:23:16.000000 django-vue-utils-0.1.7/manage.py
--rw-rw-r--   0 mike      (1000) mike      (1000)      819 2023-10-03 09:28:58.000000 django-vue-utils-0.1.7/pyproject.toml
--rw-rw-r--   0 mike      (1000) mike      (1000)      716 2023-10-03 09:29:35.653299 django-vue-utils-0.1.7/setup.cfg
--rw-rw-r--   0 mike      (1000) mike      (1000)       39 2023-09-29 13:08:14.000000 django-vue-utils-0.1.7/setup.py
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-05-16 05:40:10.031630 django-vue-utils-0.1.8/
+-rw-rw-r--   0 mike      (1000) mike      (1000)     1080 2023-09-29 13:02:46.000000 django-vue-utils-0.1.8/LICENSE
+-rw-rw-r--   0 mike      (1000) mike      (1000)       78 2023-09-29 15:05:56.000000 django-vue-utils-0.1.8/MANIFEST.in
+-rw-rw-r--   0 mike      (1000) mike      (1000)     2589 2024-05-16 05:40:10.031630 django-vue-utils-0.1.8/PKG-INFO
+-rw-rw-r--   0 mike      (1000) mike      (1000)     1718 2024-05-16 05:39:34.000000 django-vue-utils-0.1.8/README.rst
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-05-16 05:40:10.023629 django-vue-utils-0.1.8/django_vue_utilities/
+-rw-rw-r--   0 mike      (1000) mike      (1000)        0 2023-09-29 12:46:51.000000 django-vue-utils-0.1.8/django_vue_utilities/__init__.py
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-05-16 05:40:10.023629 django-vue-utils-0.1.8/django_vue_utilities/templatetags/
+-rw-rw-r--   0 mike      (1000) mike      (1000)        0 2023-09-29 12:48:08.000000 django-vue-utils-0.1.8/django_vue_utilities/templatetags/__init__.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     1875 2023-09-29 14:57:49.000000 django-vue-utils-0.1.8/django_vue_utilities/templatetags/vue_utils.py
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-05-16 05:40:10.023629 django-vue-utils-0.1.8/django_vue_utilities/tests/
+-rw-rw-r--   0 mike      (1000) mike      (1000)     5152 2023-09-29 14:59:12.000000 django-vue-utils-0.1.8/django_vue_utilities/tests/__init__.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)      495 2023-09-29 13:57:32.000000 django-vue-utils-0.1.8/django_vue_utilities/tests/settings.py
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-05-16 05:40:10.023629 django-vue-utils-0.1.8/django_vue_utils.egg-info/
+-rw-r--r--   0 mike      (1000) mike      (1000)     2589 2024-05-16 05:40:09.000000 django-vue-utils-0.1.8/django_vue_utils.egg-info/PKG-INFO
+-rw-rw-r--   0 mike      (1000) mike      (1000)     3127 2024-05-16 05:40:10.000000 django-vue-utils-0.1.8/django_vue_utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 mike      (1000) mike      (1000)        1 2024-05-16 05:40:09.000000 django-vue-utils-0.1.8/django_vue_utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 mike      (1000) mike      (1000)       12 2024-05-16 05:40:09.000000 django-vue-utils-0.1.8/django_vue_utils.egg-info/requires.txt
+-rw-rw-r--   0 mike      (1000) mike      (1000)       21 2024-05-16 05:40:09.000000 django-vue-utils-0.1.8/django_vue_utils.egg-info/top_level.txt
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-05-16 05:40:10.023629 django-vue-utils-0.1.8/docs/
+-rw-rw-r--   0 mike      (1000) mike      (1000)     7662 2023-09-29 13:46:30.000000 django-vue-utils-0.1.8/docs/Makefile
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-05-16 05:40:10.019629 django-vue-utils-0.1.8/docs/_build/
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-05-16 05:40:10.023629 django-vue-utils-0.1.8/docs/_build/doctrees/
+-rw-rw-r--   0 mike      (1000) mike      (1000)     8998 2023-09-29 13:52:33.000000 django-vue-utils-0.1.8/docs/_build/doctrees/documentation.doctree
+-rw-rw-r--   0 mike      (1000) mike      (1000)    62045 2023-09-29 14:34:36.000000 django-vue-utils-0.1.8/docs/_build/doctrees/environment.pickle
+-rw-rw-r--   0 mike      (1000) mike      (1000)    14365 2023-09-29 14:34:36.000000 django-vue-utils-0.1.8/docs/_build/doctrees/index.doctree
+-rw-rw-r--   0 mike      (1000) mike      (1000)     6074 2023-09-29 13:52:33.000000 django-vue-utils-0.1.8/docs/_build/doctrees/install.doctree
+-rw-rw-r--   0 mike      (1000) mike      (1000)     4091 2023-09-29 14:34:36.000000 django-vue-utils-0.1.8/docs/_build/doctrees/settings.doctree
+-rw-rw-r--   0 mike      (1000) mike      (1000)     5070 2023-09-29 14:34:36.000000 django-vue-utils-0.1.8/docs/_build/doctrees/tests.doctree
+-rw-rw-r--   0 mike      (1000) mike      (1000)     4476 2023-09-29 14:34:36.000000 django-vue-utils-0.1.8/docs/_build/doctrees/usage.doctree
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-05-16 05:40:10.023629 django-vue-utils-0.1.8/docs/_build/html/
+-rw-rw-r--   0 mike      (1000) mike      (1000)      230 2023-09-29 14:34:36.000000 django-vue-utils-0.1.8/docs/_build/html/.buildinfo
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-05-16 05:40:10.023629 django-vue-utils-0.1.8/docs/_build/html/_sources/
+-rw-rw-r--   0 mike      (1000) mike      (1000)     1122 2023-09-29 13:42:59.000000 django-vue-utils-0.1.8/docs/_build/html/_sources/documentation.rst.txt
+-rw-rw-r--   0 mike      (1000) mike      (1000)     1911 2023-09-29 14:34:50.000000 django-vue-utils-0.1.8/docs/_build/html/_sources/index.rst.txt
+-rw-rw-r--   0 mike      (1000) mike      (1000)      615 2023-09-29 13:46:02.000000 django-vue-utils-0.1.8/docs/_build/html/_sources/install.rst.txt
+-rw-rw-r--   0 mike      (1000) mike      (1000)      310 2023-09-29 14:34:21.000000 django-vue-utils-0.1.8/docs/_build/html/_sources/settings.rst.txt
+-rw-rw-r--   0 mike      (1000) mike      (1000)      575 2023-09-29 14:24:07.000000 django-vue-utils-0.1.8/docs/_build/html/_sources/tests.rst.txt
+-rw-rw-r--   0 mike      (1000) mike      (1000)      521 2023-09-30 08:51:42.000000 django-vue-utils-0.1.8/docs/_build/html/_sources/usage.rst.txt
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-05-16 05:40:10.027629 django-vue-utils-0.1.8/docs/_build/html/_static/
+-rw-rw-r--   0 mike      (1000) mike      (1000)    15094 2023-09-29 14:34:36.000000 django-vue-utils-0.1.8/docs/_build/html/_static/basic.css
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-05-16 05:40:10.027629 django-vue-utils-0.1.8/docs/_build/html/_static/css/
+-rw-rw-r--   0 mike      (1000) mike      (1000)     3229 2023-09-29 13:49:19.000000 django-vue-utils-0.1.8/docs/_build/html/_static/css/badge_only.css
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-05-16 05:40:10.027629 django-vue-utils-0.1.8/docs/_build/html/_static/css/fonts/
+-rw-rw-r--   0 mike      (1000) mike      (1000)    87624 2023-09-29 13:49:19.000000 django-vue-utils-0.1.8/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff
+-rw-rw-r--   0 mike      (1000) mike      (1000)    67312 2023-09-29 13:49:19.000000 django-vue-utils-0.1.8/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff2
+-rw-rw-r--   0 mike      (1000) mike      (1000)    86288 2023-09-29 13:49:19.000000 django-vue-utils-0.1.8/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff
+-rw-rw-r--   0 mike      (1000) mike      (1000)    66444 2023-09-29 13:49:19.000000 django-vue-utils-0.1.8/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff2
+-rw-rw-r--   0 mike      (1000) mike      (1000)   165742 2023-09-29 13:49:19.000000 django-vue-utils-0.1.8/docs/_build/html/_static/css/fonts/fontawesome-webfont.eot
+-rw-rw-r--   0 mike      (1000) mike      (1000)   444379 2023-09-29 13:49:19.000000 django-vue-utils-0.1.8/docs/_build/html/_static/css/fonts/fontawesome-webfont.svg
+-rw-rw-r--   0 mike      (1000) mike      (1000)   165548 2023-09-29 13:49:19.000000 django-vue-utils-0.1.8/docs/_build/html/_static/css/fonts/fontawesome-webfont.ttf
+-rw-rw-r--   0 mike      (1000) mike      (1000)    98024 2023-09-29 13:49:19.000000 django-vue-utils-0.1.8/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff
+-rw-rw-r--   0 mike      (1000) mike      (1000)    77160 2023-09-29 13:49:19.000000 django-vue-utils-0.1.8/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff2
+-rw-rw-r--   0 mike      (1000) mike      (1000)   323344 2023-09-29 13:49:19.000000 django-vue-utils-0.1.8/docs/_build/html/_static/css/fonts/lato-bold-italic.woff
+-rw-rw-r--   0 mike      (1000) mike      (1000)   193308 2023-09-29 13:49:19.000000 django-vue-utils-0.1.8/docs/_build/html/_static/css/fonts/lato-bold-italic.woff2
+-rw-rw-r--   0 mike      (1000) mike      (1000)   309728 2023-09-29 13:49:19.000000 django-vue-utils-0.1.8/docs/_build/html/_static/css/fonts/lato-bold.woff
+-rw-rw-r--   0 mike      (1000) mike      (1000)   184912 2023-09-29 13:49:19.000000 django-vue-utils-0.1.8/docs/_build/html/_static/css/fonts/lato-bold.woff2
+-rw-rw-r--   0 mike      (1000) mike      (1000)   328412 2023-09-29 13:49:19.000000 django-vue-utils-0.1.8/docs/_build/html/_static/css/fonts/lato-normal-italic.woff
+-rw-rw-r--   0 mike      (1000) mike      (1000)   195704 2023-09-29 13:49:19.000000 django-vue-utils-0.1.8/docs/_build/html/_static/css/fonts/lato-normal-italic.woff2
+-rw-rw-r--   0 mike      (1000) mike      (1000)   309192 2023-09-29 13:49:19.000000 django-vue-utils-0.1.8/docs/_build/html/_static/css/fonts/lato-normal.woff
+-rw-rw-r--   0 mike      (1000) mike      (1000)   182708 2023-09-29 13:49:19.000000 django-vue-utils-0.1.8/docs/_build/html/_static/css/fonts/lato-normal.woff2
+-rw-rw-r--   0 mike      (1000) mike      (1000)   135314 2023-09-29 13:49:19.000000 django-vue-utils-0.1.8/docs/_build/html/_static/css/theme.css
+-rw-rw-r--   0 mike      (1000) mike      (1000)     4472 2023-09-29 13:21:24.000000 django-vue-utils-0.1.8/docs/_build/html/_static/doctools.js
+-rw-rw-r--   0 mike      (1000) mike      (1000)      326 2023-09-29 14:34:36.000000 django-vue-utils-0.1.8/docs/_build/html/_static/documentation_options.js
+-rw-rw-r--   0 mike      (1000) mike      (1000)      286 2023-09-29 13:21:24.000000 django-vue-utils-0.1.8/docs/_build/html/_static/file.png
+drwxrwxr-x   0 mike      (1000) mike      (1000)        0 2024-05-16 05:40:10.031630 django-vue-utils-0.1.8/docs/_build/html/_static/js/
+-rw-rw-r--   0 mike      (1000) mike      (1000)      934 2023-09-29 13:49:19.000000 django-vue-utils-0.1.8/docs/_build/html/_static/js/badge_only.js
+-rw-rw-r--   0 mike      (1000) mike      (1000)     4370 2023-09-29 13:49:19.000000 django-vue-utils-0.1.8/docs/_build/html/_static/js/html5shiv-printshiv.min.js
+-rw-rw-r--   0 mike      (1000) mike      (1000)     2734 2023-09-29 13:49:19.000000 django-vue-utils-0.1.8/docs/_build/html/_static/js/html5shiv.min.js
+-rw-rw-r--   0 mike      (1000) mike      (1000)     5023 2023-09-29 13:49:19.000000 django-vue-utils-0.1.8/docs/_build/html/_static/js/theme.js
+-rw-rw-r--   0 mike      (1000) mike      (1000)     4758 2023-09-29 14:34:36.000000 django-vue-utils-0.1.8/docs/_build/html/_static/language_data.js
+-rw-rw-r--   0 mike      (1000) mike      (1000)       90 2023-09-29 13:21:24.000000 django-vue-utils-0.1.8/docs/_build/html/_static/minus.png
+-rw-rw-r--   0 mike      (1000) mike      (1000)       90 2023-09-29 13:21:24.000000 django-vue-utils-0.1.8/docs/_build/html/_static/plus.png
+-rw-rw-r--   0 mike      (1000) mike      (1000)     4929 2023-09-29 14:34:36.000000 django-vue-utils-0.1.8/docs/_build/html/_static/pygments.css
+-rw-rw-r--   0 mike      (1000) mike      (1000)    18732 2023-09-29 13:21:24.000000 django-vue-utils-0.1.8/docs/_build/html/_static/searchtools.js
+-rw-rw-r--   0 mike      (1000) mike      (1000)     5123 2023-09-29 13:21:24.000000 django-vue-utils-0.1.8/docs/_build/html/_static/sphinx_highlight.js
+-rw-rw-r--   0 mike      (1000) mike      (1000)     6762 2023-09-30 12:44:18.000000 django-vue-utils-0.1.8/docs/_build/html/documentation.html
+-rw-rw-r--   0 mike      (1000) mike      (1000)     4230 2023-09-29 14:34:36.000000 django-vue-utils-0.1.8/docs/_build/html/genindex.html
+-rw-rw-r--   0 mike      (1000) mike      (1000)     8888 2023-09-29 14:34:36.000000 django-vue-utils-0.1.8/docs/_build/html/index.html
+-rw-rw-r--   0 mike      (1000) mike      (1000)     6077 2023-09-29 13:52:33.000000 django-vue-utils-0.1.8/docs/_build/html/install.html
+-rw-rw-r--   0 mike      (1000) mike      (1000)      384 2023-09-29 14:34:36.000000 django-vue-utils-0.1.8/docs/_build/html/objects.inv
+-rw-rw-r--   0 mike      (1000) mike      (1000)     4108 2023-09-29 14:34:36.000000 django-vue-utils-0.1.8/docs/_build/html/py-modindex.html
+-rw-rw-r--   0 mike      (1000) mike      (1000)     3941 2023-09-29 14:34:36.000000 django-vue-utils-0.1.8/docs/_build/html/search.html
+-rw-rw-r--   0 mike      (1000) mike      (1000)     3766 2023-09-29 14:34:36.000000 django-vue-utils-0.1.8/docs/_build/html/searchindex.js
+-rw-rw-r--   0 mike      (1000) mike      (1000)     4170 2023-09-29 14:34:36.000000 django-vue-utils-0.1.8/docs/_build/html/settings.html
+-rw-rw-r--   0 mike      (1000) mike      (1000)     5561 2023-09-29 14:34:36.000000 django-vue-utils-0.1.8/docs/_build/html/tests.html
+-rw-rw-r--   0 mike      (1000) mike      (1000)     6027 2023-09-29 14:34:36.000000 django-vue-utils-0.1.8/docs/_build/html/usage.html
+-rw-rw-r--   0 mike      (1000) mike      (1000)     9340 2023-09-30 12:43:30.000000 django-vue-utils-0.1.8/docs/conf.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)     1110 2023-09-30 12:44:00.000000 django-vue-utils-0.1.8/docs/documentation.rst
+-rw-rw-r--   0 mike      (1000) mike      (1000)     1841 2023-09-30 12:42:53.000000 django-vue-utils-0.1.8/docs/index.rst
+-rw-rw-r--   0 mike      (1000) mike      (1000)      615 2023-09-29 13:46:02.000000 django-vue-utils-0.1.8/docs/install.rst
+-rw-rw-r--   0 mike      (1000) mike      (1000)     7752 2023-09-30 12:43:03.000000 django-vue-utils-0.1.8/docs/make.bat
+-rw-rw-r--   0 mike      (1000) mike      (1000)      326 2023-09-30 08:49:54.000000 django-vue-utils-0.1.8/docs/settings.rst
+-rw-rw-r--   0 mike      (1000) mike      (1000)      571 2023-09-30 12:44:04.000000 django-vue-utils-0.1.8/docs/tests.rst
+-rw-rw-r--   0 mike      (1000) mike      (1000)      521 2023-09-30 08:51:45.000000 django-vue-utils-0.1.8/docs/usage.rst
+-rw-rw-r--   0 mike      (1000) mike      (1000)      270 2023-09-29 14:23:16.000000 django-vue-utils-0.1.8/manage.py
+-rw-rw-r--   0 mike      (1000) mike      (1000)      827 2024-05-16 05:39:06.000000 django-vue-utils-0.1.8/pyproject.toml
+-rw-rw-r--   0 mike      (1000) mike      (1000)      723 2024-05-16 05:40:10.031630 django-vue-utils-0.1.8/setup.cfg
+-rw-rw-r--   0 mike      (1000) mike      (1000)       39 2023-09-29 13:08:14.000000 django-vue-utils-0.1.8/setup.py
```

### Comparing `django-vue-utils-0.1.7/LICENSE` & `django-vue-utils-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `django-vue-utils-0.1.7/PKG-INFO` & `django-vue-utils-0.1.8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 Metadata-Version: 2.1
 Name: django-vue-utils
-Version: 0.1.7
+Version: 0.1.8
 Summary: Utilities and helpers for integrating Django + Vue
-Home-page: https://github.com/ilikerobots/django-vue-utils
+Home-page: https://github.com/ilikerobots/django-vue-utilities
 Author: Mike Hoolehan
 Author-email: Mike Hoolehan <mike@starheightmedia.com>
 License: MIT
-Project-URL: Homepage, https://github.com/ilikerobots/django-vue-utils
-Project-URL: Bug Tracker, https://github.com/ilikerobots/django-vue-utils/issues
+Project-URL: Homepage, https://github.com/ilikerobots/django-vue-utilities
+Project-URL: Bug Tracker, https://github.com/ilikerobots/django-vue-utilities/issues
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: JavaScript
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
-Requires-Dist: Django>=3.2
 
 ====================
 Django Vue Utilities
 ====================
 
 .. image:: https://badge.fury.io/py/django-vue-utils.svg
     :target: https://badge.fury.io/py/django-vue-utils
@@ -40,15 +39,15 @@
 Quick start
 -----------
 
 Add dependency django-vue-utils
 
 .. code-block:: bash
 
-    pip install django-vue-utils==0.1.7
+    pip install django-vue-utils==0.1.8
 
 Add "django_vue_utilities" to your INSTALLED_APPS setting:
 
 .. code-block:: python
 
     INSTALLED_APPS = [
         ...,
```

#### html2text {}

```diff
@@ -1,28 +1,29 @@
-Metadata-Version: 2.1 Name: django-vue-utils Version: 0.1.7 Summary: Utilities
+Metadata-Version: 2.1 Name: django-vue-utils Version: 0.1.8 Summary: Utilities
 and helpers for integrating Django + Vue Home-page: https://github.com/
-ilikerobots/django-vue-utils Author: Mike Hoolehan Author-email: Mike Hoolehan
+ilikerobots/django-vue-utilities Author: Mike Hoolehan Author-email: Mike
+Hoolehan
 starheightmedia.com> License: MIT Project-URL: Homepage, https://github.com/
-ilikerobots/django-vue-utils Project-URL: Bug Tracker, https://github.com/
-ilikerobots/django-vue-utils/issues Classifier: Environment :: Web Environment
-Classifier: Framework :: Django Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
-:: OS Independent Classifier: Programming Language :: Python Classifier:
-Programming Language :: Python :: 3 Classifier: Programming Language ::
-JavaScript Requires-Python: >=3.7 Description-Content-Type: text/x-rst License-
-File: LICENSE Requires-Dist: Django>=3.2 ==================== Django Vue
-Utilities ==================== .. image:: https://badge.fury.io/py/django-vue-
-utils.svg :target: https://badge.fury.io/py/django-vue-utils Provides helpers
-and utilities for integrating with a Vue front-end, as described in the article
+ilikerobots/django-vue-utilities Project-URL: Bug Tracker, https://github.com/
+ilikerobots/django-vue-utilities/issues Classifier: Environment :: Web
+Environment Classifier: Framework :: Django Classifier: Intended Audience ::
+Developers Classifier: License :: OSI Approved :: MIT License Classifier:
+Operating System :: OS Independent Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3 Classifier: Programming
+Language :: JavaScript Requires-Python: >=3.7 Description-Content-Type: text/x-
+rst License-File: LICENSE ==================== Django Vue Utilities
+==================== .. image:: https://badge.fury.io/py/django-vue-utils.svg :
+target: https://badge.fury.io/py/django-vue-utils Provides helpers and
+utilities for integrating with a Vue front-end, as described in the article
 `Django + Vue + Vite: REST Not Required`_ and in `Cookiecutter Vue + Django`_
 .. _Django + Vue + Vite\: Rest Not Required: https://medium.com/@ilikerobots/
 django-vue-vite-rest-not-required-ca63cfa558fd .. _Cookiecutter Vue + Django:
 https://github.com/ilikerobots/cookiecutter-vue-django Quick start ----------
 - Add dependency django-vue-utils .. code-block:: bash pip install django-vue-
-utils==0.1.7 Add "django_vue_utilities" to your INSTALLED_APPS setting: ..
+utils==0.1.8 Add "django_vue_utilities" to your INSTALLED_APPS setting: ..
 code-block:: python INSTALLED_APPS = [ ..., "django_vue_utilities", ] Settings
 -------- Tailor the following settings to your Vue front-end. The defaults are
 provided below. .. code-block:: python VUE_FRONTEND_USE_TYPESCRIPT = False
 VUE_FRONTEND_USE_DEV_SERVER = settings.DEBUG VUE_FRONTEND_DEV_SERVER_URL =
 'http://localhost:5173' VUE_FRONTEND_DEV_SERVER_PATH = 'src'
 VUE_FRONTEND_STATIC_PATH = 'vue' Usage ----- .. code-block:: django {% extends
 "base.html" %} {% load vue_utils %} {% block extra_js %} {# Import entrypoint
```

### Comparing `django-vue-utils-0.1.7/README.rst` & `django-vue-utils-0.1.8/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 Quick start
 -----------
 
 Add dependency django-vue-utils
 
 .. code-block:: bash
 
-    pip install django-vue-utils==0.1.7
+    pip install django-vue-utils==0.1.8
 
 Add "django_vue_utilities" to your INSTALLED_APPS setting:
 
 .. code-block:: python
 
     INSTALLED_APPS = [
         ...,
```

#### html2text {}

```diff
@@ -2,15 +2,15 @@
 https://badge.fury.io/py/django-vue-utils.svg :target: https://badge.fury.io/
 py/django-vue-utils Provides helpers and utilities for integrating with a Vue
 front-end, as described in the article `Django + Vue + Vite: REST Not
 Required`_ and in `Cookiecutter Vue + Django`_ .. _Django + Vue + Vite\: Rest
 Not Required: https://medium.com/@ilikerobots/django-vue-vite-rest-not-
 required-ca63cfa558fd .. _Cookiecutter Vue + Django: https://github.com/
 ilikerobots/cookiecutter-vue-django Quick start ----------- Add dependency
-django-vue-utils .. code-block:: bash pip install django-vue-utils==0.1.7 Add
+django-vue-utils .. code-block:: bash pip install django-vue-utils==0.1.8 Add
 "django_vue_utilities" to your INSTALLED_APPS setting: .. code-block:: python
 INSTALLED_APPS = [ ..., "django_vue_utilities", ] Settings -------- Tailor the
 following settings to your Vue front-end. The defaults are provided below. ..
 code-block:: python VUE_FRONTEND_USE_TYPESCRIPT = False
 VUE_FRONTEND_USE_DEV_SERVER = settings.DEBUG VUE_FRONTEND_DEV_SERVER_URL =
 'http://localhost:5173' VUE_FRONTEND_DEV_SERVER_PATH = 'src'
 VUE_FRONTEND_STATIC_PATH = 'vue' Usage ----- .. code-block:: django {% extends
```

### Comparing `django-vue-utils-0.1.7/django_vue_utilities/templatetags/vue_utils.py` & `django-vue-utils-0.1.8/django_vue_utilities/templatetags/vue_utils.py`

 * *Files identical despite different names*

### Comparing `django-vue-utils-0.1.7/django_vue_utilities/tests/__init__.py` & `django-vue-utils-0.1.8/django_vue_utilities/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `django-vue-utils-0.1.7/django_vue_utils.egg-info/PKG-INFO` & `django-vue-utils-0.1.8/django_vue_utils.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 Metadata-Version: 2.1
 Name: django-vue-utils
-Version: 0.1.7
+Version: 0.1.8
 Summary: Utilities and helpers for integrating Django + Vue
-Home-page: https://github.com/ilikerobots/django-vue-utils
+Home-page: https://github.com/ilikerobots/django-vue-utilities
 Author: Mike Hoolehan
 Author-email: Mike Hoolehan <mike@starheightmedia.com>
 License: MIT
-Project-URL: Homepage, https://github.com/ilikerobots/django-vue-utils
-Project-URL: Bug Tracker, https://github.com/ilikerobots/django-vue-utils/issues
+Project-URL: Homepage, https://github.com/ilikerobots/django-vue-utilities
+Project-URL: Bug Tracker, https://github.com/ilikerobots/django-vue-utilities/issues
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: JavaScript
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
-Requires-Dist: Django>=3.2
 
 ====================
 Django Vue Utilities
 ====================
 
 .. image:: https://badge.fury.io/py/django-vue-utils.svg
     :target: https://badge.fury.io/py/django-vue-utils
@@ -40,15 +39,15 @@
 Quick start
 -----------
 
 Add dependency django-vue-utils
 
 .. code-block:: bash
 
-    pip install django-vue-utils==0.1.7
+    pip install django-vue-utils==0.1.8
 
 Add "django_vue_utilities" to your INSTALLED_APPS setting:
 
 .. code-block:: python
 
     INSTALLED_APPS = [
         ...,
```

#### html2text {}

```diff
@@ -1,28 +1,29 @@
-Metadata-Version: 2.1 Name: django-vue-utils Version: 0.1.7 Summary: Utilities
+Metadata-Version: 2.1 Name: django-vue-utils Version: 0.1.8 Summary: Utilities
 and helpers for integrating Django + Vue Home-page: https://github.com/
-ilikerobots/django-vue-utils Author: Mike Hoolehan Author-email: Mike Hoolehan
+ilikerobots/django-vue-utilities Author: Mike Hoolehan Author-email: Mike
+Hoolehan
 starheightmedia.com> License: MIT Project-URL: Homepage, https://github.com/
-ilikerobots/django-vue-utils Project-URL: Bug Tracker, https://github.com/
-ilikerobots/django-vue-utils/issues Classifier: Environment :: Web Environment
-Classifier: Framework :: Django Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
-:: OS Independent Classifier: Programming Language :: Python Classifier:
-Programming Language :: Python :: 3 Classifier: Programming Language ::
-JavaScript Requires-Python: >=3.7 Description-Content-Type: text/x-rst License-
-File: LICENSE Requires-Dist: Django>=3.2 ==================== Django Vue
-Utilities ==================== .. image:: https://badge.fury.io/py/django-vue-
-utils.svg :target: https://badge.fury.io/py/django-vue-utils Provides helpers
-and utilities for integrating with a Vue front-end, as described in the article
+ilikerobots/django-vue-utilities Project-URL: Bug Tracker, https://github.com/
+ilikerobots/django-vue-utilities/issues Classifier: Environment :: Web
+Environment Classifier: Framework :: Django Classifier: Intended Audience ::
+Developers Classifier: License :: OSI Approved :: MIT License Classifier:
+Operating System :: OS Independent Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3 Classifier: Programming
+Language :: JavaScript Requires-Python: >=3.7 Description-Content-Type: text/x-
+rst License-File: LICENSE ==================== Django Vue Utilities
+==================== .. image:: https://badge.fury.io/py/django-vue-utils.svg :
+target: https://badge.fury.io/py/django-vue-utils Provides helpers and
+utilities for integrating with a Vue front-end, as described in the article
 `Django + Vue + Vite: REST Not Required`_ and in `Cookiecutter Vue + Django`_
 .. _Django + Vue + Vite\: Rest Not Required: https://medium.com/@ilikerobots/
 django-vue-vite-rest-not-required-ca63cfa558fd .. _Cookiecutter Vue + Django:
 https://github.com/ilikerobots/cookiecutter-vue-django Quick start ----------
 - Add dependency django-vue-utils .. code-block:: bash pip install django-vue-
-utils==0.1.7 Add "django_vue_utilities" to your INSTALLED_APPS setting: ..
+utils==0.1.8 Add "django_vue_utilities" to your INSTALLED_APPS setting: ..
 code-block:: python INSTALLED_APPS = [ ..., "django_vue_utilities", ] Settings
 -------- Tailor the following settings to your Vue front-end. The defaults are
 provided below. .. code-block:: python VUE_FRONTEND_USE_TYPESCRIPT = False
 VUE_FRONTEND_USE_DEV_SERVER = settings.DEBUG VUE_FRONTEND_DEV_SERVER_URL =
 'http://localhost:5173' VUE_FRONTEND_DEV_SERVER_PATH = 'src'
 VUE_FRONTEND_STATIC_PATH = 'vue' Usage ----- .. code-block:: django {% extends
 "base.html" %} {% load vue_utils %} {% block extra_js %} {# Import entrypoint
```

### Comparing `django-vue-utils-0.1.7/django_vue_utils.egg-info/SOURCES.txt` & `django-vue-utils-0.1.8/django_vue_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-vue-utils-0.1.7/docs/Makefile` & `django-vue-utils-0.1.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django-vue-utils-0.1.7/docs/_build/doctrees/documentation.doctree` & `django-vue-utils-0.1.8/docs/_build/doctrees/documentation.doctree`

 * *Files identical despite different names*

### Comparing `django-vue-utils-0.1.7/docs/_build/doctrees/environment.pickle` & `django-vue-utils-0.1.8/docs/_build/doctrees/environment.pickle`

 * *Files identical despite different names*

### Comparing `django-vue-utils-0.1.7/docs/_build/doctrees/index.doctree` & `django-vue-utils-0.1.8/docs/_build/doctrees/index.doctree`

 * *Files identical despite different names*

### Comparing `django-vue-utils-0.1.7/docs/_build/doctrees/install.doctree` & `django-vue-utils-0.1.8/docs/_build/doctrees/install.doctree`

 * *Files identical despite different names*

### Comparing `django-vue-utils-0.1.7/docs/_build/doctrees/settings.doctree` & `django-vue-utils-0.1.8/docs/_build/doctrees/settings.doctree`

 * *Files identical despite different names*

### Comparing `django-vue-utils-0.1.7/docs/_build/doctrees/tests.doctree` & `django-vue-utils-0.1.8/docs/_build/doctrees/tests.doctree`

 * *Files identical despite different names*

### Comparing `django-vue-utils-0.1.7/docs/_build/doctrees/usage.doctree` & `django-vue-utils-0.1.8/docs/_build/doctrees/usage.doctree`

 * *Files identical despite different names*

### Comparing `django-vue-utils-0.1.7/docs/_build/html/_sources/documentation.rst.txt` & `django-vue-utils-0.1.8/docs/_build/html/_sources/documentation.rst.txt`

 * *Files identical despite different names*

### Comparing `django-vue-utils-0.1.7/docs/_build/html/_sources/index.rst.txt` & `django-vue-utils-0.1.8/docs/_build/html/_sources/index.rst.txt`

 * *Files identical despite different names*

### Comparing `django-vue-utils-0.1.7/docs/_build/html/_sources/install.rst.txt` & `django-vue-utils-0.1.8/docs/_build/html/_sources/install.rst.txt`

 * *Files identical despite different names*

### Comparing `django-vue-utils-0.1.7/docs/_build/html/_sources/tests.rst.txt` & `django-vue-utils-0.1.8/docs/_build/html/_sources/tests.rst.txt`

 * *Files identical despite different names*

### Comparing `django-vue-utils-0.1.7/docs/_build/html/_sources/usage.rst.txt` & `django-vue-utils-0.1.8/docs/_build/html/_sources/usage.rst.txt`

 * *Files identical despite different names*

### Comparing `django-vue-utils-0.1.7/docs/_build/html/_static/basic.css` & `django-vue-utils-0.1.8/docs/_build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `django-vue-utils-0.1.7/docs/_build/html/_static/css/badge_only.css` & `django-vue-utils-0.1.8/docs/_build/html/_static/css/badge_only.css`

 * *Files identical despite different names*

### Comparing `django-vue-utils-0.1.7/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff` & `django-vue-utils-0.1.8/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff`

 * *Files identical despite different names*

### Comparing `django-vue-utils-0.1.7/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff2` & `django-vue-utils-0.1.8/docs/_build/html/_static/css/fonts/Roboto-Slab-Bold.woff2`

 * *Files identical despite different names*

### Comparing `django-vue-utils-0.1.7/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff` & `django-vue-utils-0.1.8/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff`

 * *Files identical despite different names*

### Comparing `django-vue-utils-0.1.7/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff2` & `django-vue-utils-0.1.8/docs/_build/html/_static/css/fonts/Roboto-Slab-Regular.woff2`

 * *Files identical despite different names*

### Comparing `django-vue-utils-0.1.7/docs/_build/html/_static/css/fonts/fontawesome-webfont.eot` & `django-vue-utils-0.1.8/docs/_build/html/_static/css/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `django-vue-utils-0.1.7/docs/_build/html/_static/css/fonts/fontawesome-webfont.svg` & `django-vue-utils-0.1.8/docs/_build/html/_static/css/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `django-vue-utils-0.1.7/docs/_build/html/_static/css/fonts/fontawesome-webfont.ttf` & `django-vue-utils-0.1.8/docs/_build/html/_static/css/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `django-vue-utils-0.1.7/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff` & `django-vue-utils-0.1.8/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `django-vue-utils-0.1.7/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff2` & `django-vue-utils-0.1.8/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `django-vue-utils-0.1.7/docs/_build/html/_static/css/fonts/lato-bold-italic.woff` & `django-vue-utils-0.1.8/docs/_build/html/_static/css/fonts/lato-bold-italic.woff`

 * *Files identical despite different names*

### Comparing `django-vue-utils-0.1.7/docs/_build/html/_static/css/fonts/lato-bold-italic.woff2` & `django-vue-utils-0.1.8/docs/_build/html/_static/css/fonts/lato-bold-italic.woff2`

 * *Files identical despite different names*

### Comparing `django-vue-utils-0.1.7/docs/_build/html/_static/css/fonts/lato-bold.woff` & `django-vue-utils-0.1.8/docs/_build/html/_static/css/fonts/lato-bold.woff`

 * *Files identical despite different names*

### Comparing `django-vue-utils-0.1.7/docs/_build/html/_static/css/fonts/lato-bold.woff2` & `django-vue-utils-0.1.8/docs/_build/html/_static/css/fonts/lato-bold.woff2`

 * *Files identical despite different names*

### Comparing `django-vue-utils-0.1.7/docs/_build/html/_static/css/fonts/lato-normal-italic.woff` & `django-vue-utils-0.1.8/docs/_build/html/_static/css/fonts/lato-normal-italic.woff`

 * *Files identical despite different names*

### Comparing `django-vue-utils-0.1.7/docs/_build/html/_static/css/fonts/lato-normal-italic.woff2` & `django-vue-utils-0.1.8/docs/_build/html/_static/css/fonts/lato-normal-italic.woff2`

 * *Files identical despite different names*

### Comparing `django-vue-utils-0.1.7/docs/_build/html/_static/css/fonts/lato-normal.woff` & `django-vue-utils-0.1.8/docs/_build/html/_static/css/fonts/lato-normal.woff`

 * *Files identical despite different names*

### Comparing `django-vue-utils-0.1.7/docs/_build/html/_static/css/fonts/lato-normal.woff2` & `django-vue-utils-0.1.8/docs/_build/html/_static/css/fonts/lato-normal.woff2`

 * *Files identical despite different names*

### Comparing `django-vue-utils-0.1.7/docs/_build/html/_static/css/theme.css` & `django-vue-utils-0.1.8/docs/_build/html/_static/css/theme.css`

 * *Files identical despite different names*

### Comparing `django-vue-utils-0.1.7/docs/_build/html/_static/doctools.js` & `django-vue-utils-0.1.8/docs/_build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `django-vue-utils-0.1.7/docs/_build/html/_static/js/badge_only.js` & `django-vue-utils-0.1.8/docs/_build/html/_static/js/badge_only.js`

 * *Files identical despite different names*

### Comparing `django-vue-utils-0.1.7/docs/_build/html/_static/js/html5shiv-printshiv.min.js` & `django-vue-utils-0.1.8/docs/_build/html/_static/js/html5shiv-printshiv.min.js`

 * *Files identical despite different names*

### Comparing `django-vue-utils-0.1.7/docs/_build/html/_static/js/html5shiv.min.js` & `django-vue-utils-0.1.8/docs/_build/html/_static/js/html5shiv.min.js`

 * *Files identical despite different names*

### Comparing `django-vue-utils-0.1.7/docs/_build/html/_static/js/theme.js` & `django-vue-utils-0.1.8/docs/_build/html/_static/js/theme.js`

 * *Files identical despite different names*

### Comparing `django-vue-utils-0.1.7/docs/_build/html/_static/language_data.js` & `django-vue-utils-0.1.8/docs/_build/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `django-vue-utils-0.1.7/docs/_build/html/_static/pygments.css` & `django-vue-utils-0.1.8/docs/_build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `django-vue-utils-0.1.7/docs/_build/html/_static/searchtools.js` & `django-vue-utils-0.1.8/docs/_build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `django-vue-utils-0.1.7/docs/_build/html/_static/sphinx_highlight.js` & `django-vue-utils-0.1.8/docs/_build/html/_static/sphinx_highlight.js`

 * *Files identical despite different names*

### Comparing `django-vue-utils-0.1.7/docs/_build/html/documentation.html` & `django-vue-utils-0.1.8/docs/_build/html/documentation.html`

 * *Files identical despite different names*

### Comparing `django-vue-utils-0.1.7/docs/_build/html/genindex.html` & `django-vue-utils-0.1.8/docs/_build/html/genindex.html`

 * *Files identical despite different names*

### Comparing `django-vue-utils-0.1.7/docs/_build/html/index.html` & `django-vue-utils-0.1.8/docs/_build/html/index.html`

 * *Files identical despite different names*

### Comparing `django-vue-utils-0.1.7/docs/_build/html/install.html` & `django-vue-utils-0.1.8/docs/_build/html/install.html`

 * *Files identical despite different names*

### Comparing `django-vue-utils-0.1.7/docs/_build/html/py-modindex.html` & `django-vue-utils-0.1.8/docs/_build/html/py-modindex.html`

 * *Files identical despite different names*

### Comparing `django-vue-utils-0.1.7/docs/_build/html/search.html` & `django-vue-utils-0.1.8/docs/_build/html/search.html`

 * *Files identical despite different names*

### Comparing `django-vue-utils-0.1.7/docs/_build/html/searchindex.js` & `django-vue-utils-0.1.8/docs/_build/html/searchindex.js`

 * *Files identical despite different names*

### Comparing `django-vue-utils-0.1.7/docs/_build/html/settings.html` & `django-vue-utils-0.1.8/docs/_build/html/settings.html`

 * *Files identical despite different names*

### Comparing `django-vue-utils-0.1.7/docs/_build/html/tests.html` & `django-vue-utils-0.1.8/docs/_build/html/tests.html`

 * *Files identical despite different names*

### Comparing `django-vue-utils-0.1.7/docs/_build/html/usage.html` & `django-vue-utils-0.1.8/docs/_build/html/usage.html`

 * *Files identical despite different names*

### Comparing `django-vue-utils-0.1.7/docs/conf.py` & `django-vue-utils-0.1.8/docs/conf.py`

 * *Files identical despite different names*

### Comparing `django-vue-utils-0.1.7/docs/documentation.rst` & `django-vue-utils-0.1.8/docs/documentation.rst`

 * *Files identical despite different names*

### Comparing `django-vue-utils-0.1.7/docs/index.rst` & `django-vue-utils-0.1.8/docs/index.rst`

 * *Files identical despite different names*

### Comparing `django-vue-utils-0.1.7/docs/install.rst` & `django-vue-utils-0.1.8/docs/install.rst`

 * *Files identical despite different names*

### Comparing `django-vue-utils-0.1.7/docs/make.bat` & `django-vue-utils-0.1.8/docs/make.bat`

 * *Files identical despite different names*

### Comparing `django-vue-utils-0.1.7/docs/tests.rst` & `django-vue-utils-0.1.8/docs/tests.rst`

 * *Files identical despite different names*

### Comparing `django-vue-utils-0.1.7/docs/usage.rst` & `django-vue-utils-0.1.8/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `django-vue-utils-0.1.7/pyproject.toml` & `django-vue-utils-0.1.8/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['setuptools>=40.8.0']
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = "django-vue-utils"
-version = "0.1.7"
+version = "0.1.8"
 authors = [
   { name="Mike Hoolehan", email="mike@starheightmedia.com" },
 ]
 description = "Utilities and helpers for integrating Django + Vue"
 readme = "README.rst"
 requires-python = ">=3.7"
 classifiers = [
@@ -19,9 +19,9 @@
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: JavaScript",
 ]
 
 [project.urls]
-"Homepage" = "https://github.com/ilikerobots/django-vue-utils"
-"Bug Tracker" = "https://github.com/ilikerobots/django-vue-utils/issues"
+"Homepage" = "https://github.com/ilikerobots/django-vue-utilities"
+"Bug Tracker" = "https://github.com/ilikerobots/django-vue-utilities/issues"
```

### Comparing `django-vue-utils-0.1.7/setup.cfg` & `django-vue-utils-0.1.8/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [metadata]
 name = django-vue-utils
-sion = 0.1.7
+version = 0.1.8
 description = Utilities and helpers for integrating Django + Vue
 long_description = file: README.rst
-url = https://github.com/ilikerobots/django-vue-utils
+url = https://github.com/ilikerobots/django-vue-utilities
 author = Mike Hoolehan
 author_email = mike@starheightmedia.com
 license = MIT
 classifiers = 
 	Environment :: Web Environment
 	Framework :: Django
 	Intended Audience :: Developers
```

