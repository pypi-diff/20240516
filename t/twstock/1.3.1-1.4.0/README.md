# Comparing `tmp/twstock-1.3.1.tar.gz` & `tmp/twstock-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twstock-1.3.1.tar", last modified: Wed May 15 06:48:25 2019, max compression
+gzip compressed data, was "twstock-1.4.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `twstock-1.3.1.tar` & `twstock-1.4.0.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0       16 2018-03-17 11:26:23.390197 twstock-1.3.1/.codecov.yml
--rw-r--r--   0        0        0     1150 2018-03-17 11:26:23.390197 twstock-1.3.1/.gitignore
--rw-r--r--   0        0        0      343 2019-03-18 10:02:58.213104 twstock-1.3.1/.travis.yml
--rw-r--r--   0        0        0     3209 2018-03-17 11:26:23.390197 twstock-1.3.1/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0      659 2018-03-17 11:26:23.390197 twstock-1.3.1/CONTRIBUTING
--rw-r--r--   0        0        0     1057 2019-03-19 06:12:08.840044 twstock-1.3.1/LICENSE
--rw-r--r--   0        0        0       28 2018-03-17 11:26:23.390197 twstock-1.3.1/MANIFEST.in
--rw-r--r--   0        0        0      171 2019-05-15 06:45:57.459516 twstock-1.3.1/Pipfile
--rw-r--r--   0        0        0     5802 2019-05-15 06:46:03.862762 twstock-1.3.1/README.md
--rw-r--r--   0        0        0      587 2019-03-18 10:02:58.213104 twstock-1.3.1/appveyor.yml
--rw-r--r--   0        0        0      638 2018-03-17 11:26:23.390197 twstock-1.3.1/docs/Makefile
--rw-r--r--   0        0        0     4834 2018-03-17 11:26:23.390197 twstock-1.3.1/docs/conf.py
--rw-r--r--   0        0        0      722 2018-03-17 11:26:23.390197 twstock-1.3.1/docs/contributing.rst
--rw-r--r--   0        0        0     1413 2018-03-17 11:26:23.390197 twstock-1.3.1/docs/index.rst
--rw-r--r--   0        0        0     1088 2019-03-19 06:12:08.843377 twstock-1.3.1/docs/license.rst
--rw-r--r--   0        0        0      811 2018-03-17 11:26:23.390197 twstock-1.3.1/docs/make.bat
--rw-r--r--   0        0        0     1362 2018-03-17 11:26:23.390197 twstock-1.3.1/docs/prepare.rst
--rw-r--r--   0        0        0     9439 2019-03-18 10:25:26.379961 twstock-1.3.1/docs/quickstart.rst
--rw-r--r--   0        0        0     3486 2018-03-17 11:26:23.390197 twstock-1.3.1/docs/reference/analytics.rst
--rw-r--r--   0        0        0      576 2018-03-17 11:26:23.390197 twstock-1.3.1/docs/reference/codes.rst
--rw-r--r--   0        0        0      115 2018-03-17 11:26:23.390197 twstock-1.3.1/docs/reference/index.rst
--rw-r--r--   0        0        0     1953 2018-03-17 11:26:23.390197 twstock-1.3.1/docs/reference/realtime.rst
--rw-r--r--   0        0        0     3535 2018-03-17 11:26:23.390197 twstock-1.3.1/docs/reference/stock.rst
--rwxr-xr-x   0        0        0     1162 2018-03-17 11:26:23.390197 twstock-1.3.1/docs/serve.py
--rw-r--r--   0        0        0      374 2018-03-17 11:26:23.390197 twstock-1.3.1/flit.ini
--rw-r--r--   0        0        0        0 2018-03-17 11:26:23.390197 twstock-1.3.1/test/__init__.py
--rw-r--r--   0        0        0     5464 2018-03-17 11:26:23.393531 twstock-1.3.1/test/test_analytics.py
--rw-r--r--   0        0        0      313 2018-03-17 11:26:23.393531 twstock-1.3.1/test/test_cli.py
--rw-r--r--   0        0        0      925 2018-03-17 11:26:23.393531 twstock-1.3.1/test/test_mock.py
--rw-r--r--   0        0        0     1273 2019-05-13 11:45:43.614802 twstock-1.3.1/test/test_proxy.py
--rw-r--r--   0        0        0     2207 2018-03-17 11:26:23.393531 twstock-1.3.1/test/test_realtime.py
--rw-r--r--   0        0        0     8477 2019-03-18 10:02:58.213104 twstock-1.3.1/test/test_stock.py
--rw-r--r--   0        0        0      348 2019-05-15 06:47:26.778288 twstock-1.3.1/twstock/__init__.py
--rw-r--r--   0        0        0      108 2018-03-17 11:26:23.393531 twstock-1.3.1/twstock/__main__.py
--rw-r--r--   0        0        0     4421 2018-03-17 11:26:23.393531 twstock-1.3.1/twstock/analytics.py
--rw-r--r--   0        0        0      845 2019-03-18 10:45:14.240130 twstock-1.3.1/twstock/cli/__init__.py
--rw-r--r--   0        0        0      767 2018-03-17 11:26:23.393531 twstock-1.3.1/twstock/cli/best_four_point.py
--rw-r--r--   0        0        0       66 2018-03-17 11:26:23.393531 twstock-1.3.1/twstock/cli/realtime.py
--rw-r--r--   0        0        0      393 2018-03-17 11:26:23.393531 twstock-1.3.1/twstock/cli/stock.py
--rw-r--r--   0        0        0       71 2019-03-18 10:02:58.213104 twstock-1.3.1/twstock/codes/__init__.py
--rw-r--r--   0        0        0     1103 2019-03-18 10:02:58.213104 twstock-1.3.1/twstock/codes/codes.py
--rw-r--r--   0        0        0     1852 2019-05-13 11:27:51.209607 twstock-1.3.1/twstock/codes/fetch.py
--rw-r--r--   0        0        0   426337 2019-03-18 10:18:58.816573 twstock-1.3.1/twstock/codes/tpex_equities.csv
--rw-r--r--   0        0        0  1472016 2019-03-18 10:18:58.819906 twstock-1.3.1/twstock/codes/twse_equities.csv
--rw-r--r--   0        0        0     6875 2018-03-17 11:26:23.410197 twstock-1.3.1/twstock/legacy.py
--rw-r--r--   0        0        0     3622 2018-03-17 11:26:23.410197 twstock-1.3.1/twstock/mock/__init__.py
--rw-r--r--   0        0        0     1374 2019-05-13 11:45:43.614802 twstock-1.3.1/twstock/proxy.py
--rw-r--r--   0        0        0     3500 2019-05-13 11:27:51.209607 twstock-1.3.1/twstock/realtime.py
--rw-r--r--   0        0        0     7057 2019-05-15 06:47:10.338514 twstock-1.3.1/twstock/stock.py
--rw-r--r--   0        0        0      720 1970-01-01 00:00:00.000000 twstock-1.3.1/setup.py
--rw-r--r--   0        0        0      197 1970-01-01 00:00:00.000000 twstock-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0       16 2024-05-15 14:30:23.007571 twstock-1.4.0/.codecov.yml
+-rw-r--r--   0        0        0     1709 2024-05-15 14:30:23.007571 twstock-1.4.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0     1095 2024-05-16 03:48:57.139558 twstock-1.4.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     1173 2024-05-15 15:08:21.666683 twstock-1.4.0/.gitignore
+-rw-r--r--   0        0        0     3209 2024-05-15 14:30:23.007571 twstock-1.4.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0      659 2024-05-15 14:30:23.007571 twstock-1.4.0/CONTRIBUTING
+-rw-r--r--   0        0        0     1057 2024-05-16 03:48:57.139558 twstock-1.4.0/LICENSE
+-rw-r--r--   0        0        0       28 2024-05-15 14:30:23.007571 twstock-1.4.0/MANIFEST.in
+-rw-r--r--   0        0        0      171 2024-05-15 14:30:23.007571 twstock-1.4.0/Pipfile
+-rw-r--r--   0        0        0     5635 2024-05-16 03:48:57.139558 twstock-1.4.0/README.md
+-rw-r--r--   0        0        0      638 2024-05-15 14:30:23.007571 twstock-1.4.0/docs/Makefile
+-rw-r--r--   0        0        0     4872 2024-05-16 03:48:57.139558 twstock-1.4.0/docs/conf.py
+-rw-r--r--   0        0        0      722 2024-05-15 14:30:23.007571 twstock-1.4.0/docs/contributing.rst
+-rw-r--r--   0        0        0     1413 2024-05-15 14:30:23.007571 twstock-1.4.0/docs/index.rst
+-rw-r--r--   0        0        0     1088 2024-05-16 03:48:57.139558 twstock-1.4.0/docs/license.rst
+-rw-r--r--   0        0        0      811 2024-05-15 14:30:23.007571 twstock-1.4.0/docs/make.bat
+-rw-r--r--   0        0        0     1362 2024-05-15 14:30:23.007571 twstock-1.4.0/docs/prepare.rst
+-rw-r--r--   0        0        0     9439 2024-05-15 14:30:23.007571 twstock-1.4.0/docs/quickstart.rst
+-rw-r--r--   0        0        0     3486 2024-05-15 14:30:23.007571 twstock-1.4.0/docs/reference/analytics.rst
+-rw-r--r--   0        0        0      576 2024-05-15 14:30:23.007571 twstock-1.4.0/docs/reference/codes.rst
+-rw-r--r--   0        0        0      115 2024-05-15 14:30:23.007571 twstock-1.4.0/docs/reference/index.rst
+-rw-r--r--   0        0        0     1953 2024-05-15 14:30:23.007571 twstock-1.4.0/docs/reference/realtime.rst
+-rw-r--r--   0        0        0     3535 2024-05-15 14:30:23.007571 twstock-1.4.0/docs/reference/stock.rst
+-rwxr-xr-x   0        0        0     1162 2024-05-15 15:08:21.666683 twstock-1.4.0/docs/serve.py
+-rw-r--r--   0        0        0      374 2024-05-15 14:30:23.007571 twstock-1.4.0/flit.ini
+-rw-r--r--   0        0        0      514 2024-05-15 14:32:41.783073 twstock-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-15 14:30:23.007571 twstock-1.4.0/test/__init__.py
+-rw-r--r--   0        0        0     5357 2024-05-15 15:08:21.666683 twstock-1.4.0/test/test_analytics.py
+-rw-r--r--   0        0        0      313 2024-05-15 15:08:21.666683 twstock-1.4.0/test/test_cli.py
+-rw-r--r--   0        0        0     1129 2024-05-16 03:48:57.139558 twstock-1.4.0/test/test_mock.py
+-rw-r--r--   0        0        0     1293 2024-05-15 15:08:21.666683 twstock-1.4.0/test/test_proxy.py
+-rw-r--r--   0        0        0     2219 2024-05-16 03:48:57.142891 twstock-1.4.0/test/test_realtime.py
+-rw-r--r--   0        0        0    10112 2024-05-15 15:08:21.666683 twstock-1.4.0/test/test_stock.py
+-rw-r--r--   0        0        0      348 2024-05-16 03:48:57.142891 twstock-1.4.0/twstock/__init__.py
+-rw-r--r--   0        0        0      108 2024-05-15 15:08:21.666683 twstock-1.4.0/twstock/__main__.py
+-rw-r--r--   0        0        0     4739 2024-05-15 15:08:21.666683 twstock-1.4.0/twstock/analytics.py
+-rw-r--r--   0        0        0      859 2024-05-15 15:08:21.666683 twstock-1.4.0/twstock/cli/__init__.py
+-rw-r--r--   0        0        0      768 2024-05-15 15:08:21.666683 twstock-1.4.0/twstock/cli/best_four_point.py
+-rw-r--r--   0        0        0       66 2024-05-15 14:30:23.010905 twstock-1.4.0/twstock/cli/realtime.py
+-rw-r--r--   0        0        0      393 2024-05-15 15:08:21.666683 twstock-1.4.0/twstock/cli/stock.py
+-rw-r--r--   0        0        0       71 2024-05-15 14:30:23.010905 twstock-1.4.0/twstock/codes/__init__.py
+-rw-r--r--   0        0        0     1074 2024-05-15 15:08:21.666683 twstock-1.4.0/twstock/codes/codes.py
+-rw-r--r--   0        0        0     1829 2024-05-15 15:12:59.113293 twstock-1.4.0/twstock/codes/fetch.py
+-rw-r--r--   0        0        0  1085370 2024-05-16 03:48:57.142891 twstock-1.4.0/twstock/codes/tpex_equities.csv
+-rw-r--r--   0        0        0  3613203 2024-05-16 03:48:57.149558 twstock-1.4.0/twstock/codes/twse_equities.csv
+-rw-r--r--   0        0        0     6865 2024-05-15 15:08:21.670016 twstock-1.4.0/twstock/legacy.py
+-rw-r--r--   0        0        0     3590 2024-05-16 03:48:57.149558 twstock-1.4.0/twstock/mock/__init__.py
+-rw-r--r--   0        0        0     1370 2024-05-15 15:08:21.670016 twstock-1.4.0/twstock/proxy.py
+-rw-r--r--   0        0        0     3557 2024-05-16 02:39:01.933038 twstock-1.4.0/twstock/realtime.py
+-rw-r--r--   0        0        0     6982 2024-05-16 02:39:01.933038 twstock-1.4.0/twstock/stock.py
+-rw-r--r--   0        0        0     6072 1970-01-01 00:00:00.000000 twstock-1.4.0/PKG-INFO
```

### Comparing `twstock-1.3.1/.gitignore` & `twstock-1.4.0/.gitignore`

 * *Files 9% similar despite different names*

```diff
@@ -94,7 +94,11 @@
 
 # mkdocs documentation
 /site
 
 # mypy
 .mypy_cache/
 
+# Emacs
+*~
+\#.*\#
+*.\#
```

### Comparing `twstock-1.3.1/CODE_OF_CONDUCT.md` & `twstock-1.4.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `twstock-1.3.1/CONTRIBUTING` & `twstock-1.4.0/CONTRIBUTING`

 * *Files identical despite different names*

### Comparing `twstock-1.3.1/LICENSE` & `twstock-1.4.0/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2017-2019 Louie Lu
+Copyright (c) 2017-2024 Louie Lu
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `twstock-1.3.1/README.md` & `twstock-1.4.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-[![Travis Build
-Status](https://travis-ci.org/mlouielu/twstock.svg?branch=master)](https://travis-ci.org/mlouielu/twstock)
-[![Appveyor Build Status](https://ci.appveyor.com/api/projects/status/d03c5laj01ap7qrt?svg=true)](https://ci.appveyor.com/project/mlouielu/twstock)
+![GitHub Actions Status](https://github.com/mlouielu/twstock/actions/workflows/ci.yml/badge.svg)
 [![Coverage Status](https://coveralls.io/repos/github/mlouielu/twstock/badge.svg?branch=master)](https://coveralls.io/github/mlouielu/twstock?branch=master)
 [![PyPI version](https://badge.fury.io/py/twstock.svg)](https://badge.fury.io/py/twstock)
 [![Documentation Status](https://readthedocs.org/projects/twstock/badge/?version=latest)](http://twstock.readthedocs.io/zh_TW/latest/?badge=latest)
 
 
 有任何問題歡迎透過 [Gitter.im](https://gitter.im/twstock/Lobby) 詢問。
 
@@ -23,16 +21,17 @@
 
 ## Documentation
 
 * [twstock documentation (正體中文)](http://twstock.readthedocs.io/zh_TW/latest)
 
 ## Requirements
 
-* requests
 * Python 3
+* lxml
+* requests
 
 ## Install
 
 By PyPi
 
 ```
 $ python -m pip install --user twstock
@@ -106,19 +105,19 @@
 stock = Stock('2330')                             # 擷取台積電股價
 ma_p = stock.moving_average(stock.price, 5)       # 計算五日均價
 ma_c = stock.moving_average(stock.capacity, 5)    # 計算五日均量
 ma_p_cont = stock.continuous(ma_p)                # 計算五日均價持續天數
 ma_br = stock.ma_bias_ratio(5, 10)                # 計算五日、十日乖離值
 ```
 
-擷取自 2015 年 1 月至今之資料
+擷取自 2024 年 3 月至今之資料
 
 ```python
 stock = Stock('2330')
-stock.fetch_from(2015, 1)
+stock.fetch_from(2024, 3)
 ```
 
 基本資料之使用
 
 ```python
 >>> stock = Stock('2330')
 >>> stock.price
```

### Comparing `twstock-1.3.1/docs/Makefile` & `twstock-1.4.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `twstock-1.3.1/docs/conf.py` & `twstock-1.4.0/docs/conf.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,134 +27,132 @@
 # If your documentation needs a minimal Sphinx version, state it here.
 #
 # needs_sphinx = '1.0'
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
-extensions = ['sphinx.ext.coverage']
+extensions = ["sphinx.ext.coverage"]
 
 # Add any paths that contain templates here, relative to this directory.
-templates_path = ['_templates']
+templates_path = ["_templates"]
 
 # The suffix(es) of source filenames.
 # You can specify multiple suffix as a list of string:
 #
 # source_suffix = ['.rst', '.md']
-source_suffix = '.rst'
+source_suffix = ".rst"
 
 # The master toctree document.
-master_doc = 'index'
+master_doc = "index"
 
 # General information about the project.
-project = 'twstock'
-copyright = '2017, Louie Lu'
-author = 'Louie Lu'
+project = "twstock"
+copyright = "2017-2024, Louie Lu"
+author = "Louie Lu"
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
-version = '1.0'
+version = "1.0"
 # The full version, including alpha/beta/rc tags.
-release = '1.0.1'
+release = "1.0.1"
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
-language = 'zh_TW'
+language = "zh_TW"
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This patterns also effect to html_static_path and html_extra_path
-exclude_patterns = ['_build', 'Thumbs.db', '.DS_Store']
+exclude_patterns = ["_build", "Thumbs.db", ".DS_Store"]
 
 # The name of the Pygments (syntax highlighting) style to use.
-pygments_style = 'sphinx'
+pygments_style = "sphinx"
 
 # If true, `todo` and `todoList` produce output, else they produce nothing.
 todo_include_todos = False
 
 
 # -- Options for HTML output ----------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 #
-html_theme = 'alabaster'
+html_theme = "alabaster"
 
 # Theme options are theme-specific and customize the look and feel of a theme
 # further.  For a list of options available for each theme, see the
 # documentation.
 #
 # html_theme_options = {}
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
-html_static_path = ['_static']
+html_static_path = ["_static"]
 
 
 # -- Options for HTMLHelp output ------------------------------------------
 
 # Output file base name for HTML help builder.
-htmlhelp_basename = 'twstockdoc'
+htmlhelp_basename = "twstockdoc"
 
 
 # -- Options for LaTeX output ---------------------------------------------
 
 latex_elements = {
     # The paper size ('letterpaper' or 'a4paper').
     #
     # 'papersize': 'letterpaper',
-
     # The font size ('10pt', '11pt' or '12pt').
     #
     # 'pointsize': '10pt',
-
     # Additional stuff for the LaTeX preamble.
     #
     # 'preamble': '',
-
     # Latex figure (float) alignment
     #
     # 'figure_align': 'htbp',
 }
 
 # Grouping the document tree into LaTeX files. List of tuples
 # (source start file, target name, title,
 #  author, documentclass [howto, manual, or own class]).
 latex_documents = [
-    (master_doc, 'twstock.tex', 'twstock Documentation',
-     'Louie Lu', 'manual'),
+    (master_doc, "twstock.tex", "twstock Documentation", "Louie Lu", "manual"),
 ]
 
 
 # -- Options for manual page output ---------------------------------------
 
 # One entry per manual page. List of tuples
 # (source start file, name, description, authors, manual section).
-man_pages = [
-    (master_doc, 'twstock', 'twstock Documentation',
-     [author], 1)
-]
+man_pages = [(master_doc, "twstock", "twstock Documentation", [author], 1)]
 
 
 # -- Options for Texinfo output -------------------------------------------
 
 # Grouping the document tree into Texinfo files. List of tuples
 # (source start file, target name, title, author,
 #  dir menu entry, description, category)
 texinfo_documents = [
-    (master_doc, 'twstock', 'twstock Documentation',
-     author, 'twstock', 'One line description of project.',
-     'Miscellaneous'),
+    (
+        master_doc,
+        "twstock",
+        "twstock Documentation",
+        author,
+        "twstock",
+        "One line description of project.",
+        "Miscellaneous",
+    ),
 ]
 
 
-
 html_sidebars = {
-    '**': ['globaltoc.html', 'relations.html', 'sourcelink.html', 'searchbox.html']
+    "**": ["globaltoc.html", "relations.html", "sourcelink.html", "searchbox.html"]
 }
```

### Comparing `twstock-1.3.1/docs/contributing.rst` & `twstock-1.4.0/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `twstock-1.3.1/docs/index.rst` & `twstock-1.4.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `twstock-1.3.1/docs/license.rst` & `twstock-1.4.0/docs/license.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 LICENSE
 ---------------------
 
-Copyright (c) 2017-2019 Louie Lu
+Copyright (c) 2017-2024 Louie Lu
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `twstock-1.3.1/docs/make.bat` & `twstock-1.4.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `twstock-1.3.1/docs/prepare.rst` & `twstock-1.4.0/docs/prepare.rst`

 * *Files identical despite different names*

### Comparing `twstock-1.3.1/docs/quickstart.rst` & `twstock-1.4.0/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `twstock-1.3.1/docs/reference/analytics.rst` & `twstock-1.4.0/docs/reference/analytics.rst`

 * *Files identical despite different names*

### Comparing `twstock-1.3.1/docs/reference/codes.rst` & `twstock-1.4.0/docs/reference/codes.rst`

 * *Files identical despite different names*

### Comparing `twstock-1.3.1/docs/reference/realtime.rst` & `twstock-1.4.0/docs/reference/realtime.rst`

 * *Files identical despite different names*

### Comparing `twstock-1.3.1/docs/reference/stock.rst` & `twstock-1.4.0/docs/reference/stock.rst`

 * *Files identical despite different names*

### Comparing `twstock-1.3.1/docs/serve.py` & `twstock-1.4.0/docs/serve.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 #!/usr/bin/env python3
-'''
+"""
 Small wsgiref based web server. Takes a path to serve from and an
 optional port number (defaults to 8000), then tries to serve files.
 Mime types are guessed from the file names, 404 errors are raised
 if the file is not found. Used for the make serve target in Doc.
-'''
+"""
 import sys
 import os
 import mimetypes
 from wsgiref import simple_server, util
 
-def app(environ, respond):
 
-    fn = os.path.join(path, environ['PATH_INFO'][1:])
-    if '.' not in fn.split(os.path.sep)[-1]:
-        fn = os.path.join(fn, 'index.html')
+def app(environ, respond):
+    fn = os.path.join(path, environ["PATH_INFO"][1:])
+    if "." not in fn.split(os.path.sep)[-1]:
+        fn = os.path.join(fn, "index.html")
     type = mimetypes.guess_type(fn)[0]
 
     if os.path.exists(fn):
-        respond('200 OK', [('Content-Type', type)])
+        respond("200 OK", [("Content-Type", type)])
         return util.FileWrapper(open(fn, "rb"))
     else:
-        respond('404 Not Found', [('Content-Type', 'text/plain')])
-        return [b'not found']
+        respond("404 Not Found", [("Content-Type", "text/plain")])
+        return [b"not found"]
 
-if __name__ == '__main__':
+
+if __name__ == "__main__":
     path = sys.argv[1]
     port = int(sys.argv[2]) if len(sys.argv) > 2 else 8000
-    httpd = simple_server.make_server('', port, app)
+    httpd = simple_server.make_server("", port, app)
     print("Serving {} on port {}, control-C to stop".format(path, port))
     try:
         httpd.serve_forever()
     except KeyboardInterrupt:
         print("\b\bShutting down.")
-
```

### Comparing `twstock-1.3.1/test/test_analytics.py` & `twstock-1.4.0/test/test_analytics.py`

 * *Files 5% similar despite different names*

```diff
@@ -81,15 +81,15 @@
         ng_result = self.ng.ma_bias_ratio_pivot(data, 5, True)
         self.assertEqual(legacy_result, ng_result)
 
 
 class BestFourPointTest(unittest.TestCase):
     @classmethod
     def setUpClass(self):
-        self.stock = stock.Stock('2330')
+        self.stock = stock.Stock("2330")
         self.stock.fetch(2015, 5)
         self.legacy = legacy.LegacyBestFourPoint(self.stock)
         self.ng = analytics.BestFourPoint(self.stock)
 
     def test_bias_ratio(self):
         self.assertEqual(self.ng.bias_ratio(), self.legacy.bias_ratio())
         self.assertEqual(self.ng.bias_ratio(True), self.legacy.bias_ratio(True))
@@ -115,31 +115,28 @@
     def test_best_sell_3(self):
         self.assertEqual(self.ng.best_sell_3(), self.legacy.best_sell_3())
 
     def test_best_sell_4(self):
         self.assertEqual(self.ng.best_sell_4(), self.legacy.best_sell_4())
 
     def test_best_four_point_to_buy(self):
-        self.assertEqual(self.ng.best_four_point_to_buy(),
-                         self.legacy.best_four_point_to_buy())
+        self.assertEqual(
+            self.ng.best_four_point_to_buy(), self.legacy.best_four_point_to_buy()
+        )
 
     def test_best_four_point_to_sell(self):
-        self.assertEqual(self.ng.best_four_point_to_sell(),
-                         self.legacy.best_four_point_to_sell())
+        self.assertEqual(
+            self.ng.best_four_point_to_sell(), self.legacy.best_four_point_to_sell()
+        )
 
     def test_best_four_point(self):
         self.stock.fetch(2014, 5)
-        self.assertEqual(self.ng.best_four_point(),
-                         self.legacy.best_four_point())
+        self.assertEqual(self.ng.best_four_point(), self.legacy.best_four_point())
 
         self.stock.fetch(2015, 5)
-        self.assertEqual(self.ng.best_four_point(),
-                         self.legacy.best_four_point())
+        self.assertEqual(self.ng.best_four_point(), self.legacy.best_four_point())
 
         self.stock.fetch(2016, 5)
-        self.assertEqual(self.ng.best_four_point(),
-                         self.legacy.best_four_point())
+        self.assertEqual(self.ng.best_four_point(), self.legacy.best_four_point())
 
         self.stock.fetch(2017, 5)
-        self.assertEqual(self.ng.best_four_point(),
-                         self.legacy.best_four_point())
-
+        self.assertEqual(self.ng.best_four_point(), self.legacy.best_four_point())
```

### Comparing `twstock-1.3.1/test/test_proxy.py` & `twstock-1.4.0/test/test_proxy.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,41 +2,41 @@
 
 from twstock.proxy import get_proxies, configure_proxy_provider, reset_proxy_provider
 from twstock.proxy import SingleProxyProvider
 from twstock.proxy import RoundRobinProxiesProvider
 
 
 class ProxyProviderTest(unittest.TestCase):
-
     def setUp(self):
         reset_proxy_provider()
 
     def tearDown(self):
         reset_proxy_provider()
 
     def test_configure(self):
         # default values are empty
         self.assertDictEqual({}, get_proxies())
 
         # configure fake proxy
-        configure_proxy_provider(SingleProxyProvider(dict(http="http-proxy", https="https-proxy")))
-        self.assertEqual("http-proxy", get_proxies()['http'])
-        self.assertEqual("https-proxy", get_proxies()['https'])
+        configure_proxy_provider(
+            SingleProxyProvider(dict(http="http-proxy", https="https-proxy"))
+        )
+        self.assertEqual("http-proxy", get_proxies()["http"])
+        self.assertEqual("https-proxy", get_proxies()["https"])
 
         # reset proxy
         reset_proxy_provider()
         self.assertDictEqual({}, get_proxies())
 
-
     def test_rr_proxies_provider(self):
-        proxies = ['a', 'b', 'c']
+        proxies = ["a", "b", "c"]
         rr_provider = RoundRobinProxiesProvider(proxies)
 
         for _ in range(3):
             for p in proxies:
                 self.assertEqual(rr_provider.get_proxy(), p)
 
-        proxies = ['d', 'e', 'f']
+        proxies = ["d", "e", "f"]
         rr_provider.proxies = proxies
         for _ in range(3):
             for p in proxies:
                 self.assertEqual(rr_provider.get_proxy(), p)
```

### Comparing `twstock-1.3.1/test/test_realtime.py` & `twstock-1.4.0/test/test_realtime.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,68 +4,70 @@
 import twstock
 from twstock import realtime
 
 
 class RealtimeTest(unittest.TestCase):
     def test_realtime_field(self):
         self.assertCountEqual(
-            realtime.get_raw('2330').keys(),
-            twstock.mock.get_stock_info('2330').keys())
+            realtime.get_raw("2330").keys(), twstock.mock.get_stock_info("2330").keys()
+        )
 
     def test_realtime_get_raw(self):
-        self.assertIn('msgArray', realtime.get_raw('2330'))
+        self.assertIn("msgArray", realtime.get_raw("2330"))
 
     def test_realtime_get_blank(self):
-        stock = realtime.get('')
+        stock = realtime.get("")
 
-        self.assertFalse(stock['success'])
-        self.assertIn('rtmessage', stock)
-        self.assertIn('rtcode', stock)
+        self.assertFalse(stock["success"])
+        self.assertIn("rtmessage", stock)
+        self.assertIn("rtcode", stock)
 
     def test_realtime_get_bad_id(self):
-        stock = realtime.get('9999')
+        stock = realtime.get("9999")
 
-        self.assertFalse(stock['success'])
-        self.assertIn('rtmessage', stock)
-        self.assertIn('rtcode', stock)
+        self.assertFalse(stock["success"])
+        self.assertIn("rtmessage", stock)
+        self.assertIn("rtcode", stock)
 
-        stock = realtime.get(['9999', '8888'])
+        stock = realtime.get(["9999", "8888"])
 
-        self.assertFalse(stock['success'])
-        self.assertIn('rtmessage', stock)
-        self.assertIn('rtcode', stock)
+        self.assertFalse(stock["success"])
+        self.assertIn("rtmessage", stock)
+        self.assertIn("rtcode", stock)
 
     def test_realtime_get_tpex_id(self):
-        stock = realtime.get('6223')
+        stock = realtime.get("6223")
 
-        self.assertTrue(stock['success'])
-        self.assertEqual(stock['info']['code'], '6223')
+        self.assertTrue(stock["success"])
+        self.assertEqual(stock["info"]["code"], "6223")
 
 
 class MockRealtimeTest(unittest.TestCase):
     @classmethod
     def setUpClass(cls):
         realtime.mock = True
 
     @classmethod
     def tearDownClass(cls):
         realtime.mock = False
 
     def test_mock_one_stock_id(self):
-        s = realtime.get('2330')
+        s = realtime.get("2330")
 
-        self.assertTrue(s['success'])
-        self.assertEqual(s['info']['code'], '2330')
-        self.assertEqual(s['realtime']['latest_trade_price'], '214.50')
-        self.assertEqual(s['realtime']['best_bid_price'],
-                         ['214.00', '213.50', '213.00', '212.50', '212.00'])
+        self.assertTrue(s["success"])
+        self.assertEqual(s["info"]["code"], "2330")
+        self.assertEqual(s["realtime"]["latest_trade_price"], "-")
+        self.assertEqual(
+            s["realtime"]["best_bid_price"],
+            ["848.0000", "847.0000", "846.0000", "845.0000", "844.0000"],
+        )
 
-    @unittest.skip('Dont want to fix this, is about the code in realtime')
+    @unittest.skip("Dont want to fix this, is about the code in realtime")
     def test_mock_multiple_stock_id(self):
-        s = realtime.get(['2330', '2337'])
+        s = realtime.get(["2330", "2337"])
 
-        self.assertTrue(s['success'])
-        self.assertCountEqual(s.keys(), ['2330', '2337', 'success'])
-        self.assertTrue(s['2330']['success'])
-        self.assertEqual(s['2330']['info']['code'], '2330')
-        self.assertEqual(s['2330']['realtime']['latest_trade_price'], '214.50')
-        self.assertTrue(s['2337']['success'])
+        self.assertTrue(s["success"])
+        self.assertCountEqual(s.keys(), ["2330", "2337", "success"])
+        self.assertTrue(s["2330"]["success"])
+        self.assertEqual(s["2330"]["info"]["code"], "2330")
+        self.assertEqual(s["2330"]["realtime"]["latest_trade_price"], "214.50")
+        self.assertTrue(s["2337"]["success"])
```

### Comparing `twstock-1.3.1/test/test_stock.py` & `twstock-1.4.0/test/test_stock.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,53 @@
 import datetime
 import unittest
 from twstock import stock
 
 
 class FetcherTest(object):
     def test_convert_date(self):
-        date = '106/05/01'
+        date = "106/05/01"
         cv_date = self.fetcher._convert_date(date)
-        self.assertEqual(cv_date, '2017/05/01')
+        self.assertEqual(cv_date, "2017/05/01")
 
     def test_make_datatuple(self):
-        data = ['106/05/02', '45,851,963', '9,053,856,108', '198.50',
-                '199.00', '195.50', '196.50', '+2.00', '15,718']
+        data = [
+            "106/05/02",
+            "45,851,963",
+            "9,053,856,108",
+            "198.50",
+            "199.00",
+            "195.50",
+            "196.50",
+            "+2.00",
+            "15,718",
+        ]
         dt = self.fetcher._make_datatuple(data)
         self.assertEqual(dt.date, datetime.datetime(2017, 5, 2))
         self.assertEqual(dt.capacity, 45851963)
         self.assertEqual(dt.turnover, 9053856108)
         self.assertEqual(dt.open, 198.5)
         self.assertEqual(dt.high, 199.0)
         self.assertEqual(dt.low, 195.5)
         self.assertEqual(dt.close, 196.5)
         self.assertEqual(dt.change, 2.0)
         self.assertEqual(dt.transaction, 15718)
 
     def test_make_datatuple_without_prices(self):
-        data = ['106/05/02', '45,851,963', '9,053,856,108', '--',
-                '--', '--', '--', ' 0.00', '15,718']
+        data = [
+            "106/05/02",
+            "45,851,963",
+            "9,053,856,108",
+            "--",
+            "--",
+            "--",
+            "--",
+            " 0.00",
+            "15,718",
+        ]
         dt = self.fetcher._make_datatuple(data)
         self.assertEqual(dt.date, datetime.datetime(2017, 5, 2))
         self.assertEqual(dt.capacity, 45851963)
         self.assertEqual(dt.turnover, 9053856108)
         self.assertEqual(dt.open, None)
         self.assertEqual(dt.high, None)
         self.assertEqual(dt.low, None)
@@ -42,44 +60,71 @@
     fetcher = stock.TWSEFetcher()
 
 
 class TPEXFetcherTest(unittest.TestCase, FetcherTest):
     fetcher = stock.TPEXFetcher()
 
     def test_make_datatuple(self):
-        data = ['106/05/02', '45,851', '9,053,856', '198.50',
-                '199.00', '195.50', '196.50', '2.00', '15,718']
+        data = [
+            "106/05/02",
+            "45,851",
+            "9,053,856",
+            "198.50",
+            "199.00",
+            "195.50",
+            "196.50",
+            "2.00",
+            "15,718",
+        ]
         dt = self.fetcher._make_datatuple(data)
         self.assertEqual(dt.date, datetime.datetime(2017, 5, 2))
         self.assertEqual(dt.capacity, 45851000)
         self.assertEqual(dt.turnover, 9053856000)
         self.assertEqual(dt.open, 198.5)
         self.assertEqual(dt.high, 199.0)
         self.assertEqual(dt.low, 195.5)
         self.assertEqual(dt.close, 196.5)
         self.assertEqual(dt.change, 2.0)
         self.assertEqual(dt.transaction, 15718)
 
     def test_make_datatuple_without_prices(self):
-        data = ['106/05/02', '45,851', '9,053,856', '--',
-                '--', '--', '--', '0.00', '15,718']
+        data = [
+            "106/05/02",
+            "45,851",
+            "9,053,856",
+            "--",
+            "--",
+            "--",
+            "--",
+            "0.00",
+            "15,718",
+        ]
         dt = self.fetcher._make_datatuple(data)
         self.assertEqual(dt.date, datetime.datetime(2017, 5, 2))
         self.assertEqual(dt.capacity, 45851000)
         self.assertEqual(dt.turnover, 9053856000)
         self.assertEqual(dt.open, None)
         self.assertEqual(dt.high, None)
         self.assertEqual(dt.low, None)
         self.assertEqual(dt.close, None)
         self.assertEqual(dt.change, 0.0)
         self.assertEqual(dt.transaction, 15718)
 
     def test_make_datatuple_with_asterisk(self):
-        data = ['106/05/02＊', '45,851', '9,053,856', '198.50',
-                '199.00', '195.50', '196.50', '2.00', '15,718']
+        data = [
+            "106/05/02＊",
+            "45,851",
+            "9,053,856",
+            "198.50",
+            "199.00",
+            "195.50",
+            "196.50",
+            "2.00",
+            "15,718",
+        ]
         dt = self.fetcher._make_datatuple(data)
         self.assertEqual(dt.date, datetime.datetime(2017, 5, 2))
         self.assertEqual(dt.capacity, 45851000)
         self.assertEqual(dt.turnover, 9053856000)
         self.assertEqual(dt.open, 198.5)
         self.assertEqual(dt.high, 199.0)
         self.assertEqual(dt.low, 195.5)
@@ -144,56 +189,138 @@
         self.assertEqual(len(self.stk.transaction), len(self.stk.data))
         self.assertEqual(self.stk.transaction, [d.transaction for d in self.stk.data])
 
 
 class TWSEStockTest(unittest.TestCase, StockTest):
     @classmethod
     def setUpClass(cls):
-        cls.stk = stock.Stock('2330')
+        cls.stk = stock.Stock("2330")
 
     def test_price(self):
         self.stk.fetch(2015, 5)
         self.assertIsInstance(self.stk.price, list)
         self.assertEqual(len(self.stk.price), len(self.stk.data))
         self.assertEqual(self.stk.price, [d.close for d in self.stk.data])
-        self.assertEqual(self.stk.price,
-                         [147.5, 147.0, 147.5, 146.5, 146.5, 148.5, 147.5,
-                          148.0, 146.0, 146.5, 146.5, 146.5, 146.5, 145.5,
-                          145.5, 147.5, 146.5, 145.0, 147.0, 146.0])
+        self.assertEqual(
+            self.stk.price,
+            [
+                147.5,
+                147.0,
+                147.5,
+                146.5,
+                146.5,
+                148.5,
+                147.5,
+                148.0,
+                146.0,
+                146.5,
+                146.5,
+                146.5,
+                146.5,
+                145.5,
+                145.5,
+                147.5,
+                146.5,
+                145.0,
+                147.0,
+                146.0,
+            ],
+        )
 
     def test_capacity(self):
         self.stk.fetch(2015, 5)
         self.assertIsInstance(self.stk.capacity, list)
         self.assertEqual(len(self.stk.capacity), len(self.stk.data))
         self.assertEqual(self.stk.capacity, [d.capacity for d in self.stk.data])
-        self.assertEqual(self.stk.capacity,
-                         [30868640, 27789400, 18824208, 21908150, 20035646,
-                          20402529, 24956498, 19437537, 39888654, 24831890,
-                          26212375, 26321396, 26984912, 41286686, 22103852,
-                          16323218, 16069726, 24257941, 36704395, 61983862])
+        self.assertEqual(
+            self.stk.capacity,
+            [
+                30868640,
+                27789400,
+                18824208,
+                21908150,
+                20035646,
+                20402529,
+                24956498,
+                19437537,
+                39888654,
+                24831890,
+                26212375,
+                26321396,
+                26984912,
+                41286686,
+                22103852,
+                16323218,
+                16069726,
+                24257941,
+                36704395,
+                61983862,
+            ],
+        )
 
 
 class TPEXStockTest(unittest.TestCase, StockTest):
     @classmethod
     def setUpClass(cls):
-        cls.stk = stock.Stock('6223')
+        cls.stk = stock.Stock("6223")
 
     def test_price(self):
         self.stk.fetch(2015, 5)
         self.assertIsInstance(self.stk.price, list)
         self.assertEqual(len(self.stk.price), len(self.stk.data))
         self.assertEqual(self.stk.price, [d.close for d in self.stk.data])
-        self.assertEqual(self.stk.price,
-                         [91.4, 91.8, 91.8, 93.5, 91.0, 84.7, 84.0, 85.8, 87.1,
-                          86.1, 83.9, 84.5, 86.7, 86.3, 86.0, 86.2, 91.1, 90.9,
-                          91.7, 90.4])
+        self.assertEqual(
+            self.stk.price,
+            [
+                91.4,
+                91.8,
+                91.8,
+                93.5,
+                91.0,
+                84.7,
+                84.0,
+                85.8,
+                87.1,
+                86.1,
+                83.9,
+                84.5,
+                86.7,
+                86.3,
+                86.0,
+                86.2,
+                91.1,
+                90.9,
+                91.7,
+                90.4,
+            ],
+        )
 
     def test_capacity(self):
         self.stk.fetch(2015, 5)
         self.assertIsInstance(self.stk.capacity, list)
         self.assertEqual(len(self.stk.capacity), len(self.stk.data))
         self.assertEqual(self.stk.capacity, [d.capacity for d in self.stk.data])
-        self.assertEqual(self.stk.capacity,
-                         [374000, 474000, 468000, 1257000, 1079000, 3400000,
-                          3424000, 1078000, 1433000, 891000, 1202000, 1008000,
-                          999000, 488000, 706000, 231000, 1890000, 782000,
-                          1214000, 583000])
+        self.assertEqual(
+            self.stk.capacity,
+            [
+                374000,
+                474000,
+                468000,
+                1257000,
+                1079000,
+                3400000,
+                3424000,
+                1078000,
+                1433000,
+                891000,
+                1202000,
+                1008000,
+                999000,
+                488000,
+                706000,
+                231000,
+                1890000,
+                782000,
+                1214000,
+                583000,
+            ],
+        )
```

### Comparing `twstock-1.3.1/twstock/analytics.py` & `twstock-1.4.0/twstock/analytics.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # -*- coding: utf-8 -*-
 
 
 class Analytics(object):
-
     def continuous(self, data):
         diff = [1 if data[-i] > data[-i - 1] else -1 for i in range(1, len(data))]
         cont = 0
         for v in diff:
             if v == diff[0]:
                 cont += 1
             else:
@@ -21,106 +20,137 @@
             data.pop()
         return result[::-1]
 
     def ma_bias_ratio(self, day1, day2):
         """Calculate moving average bias ratio"""
         data1 = self.moving_average(self.price, day1)
         data2 = self.moving_average(self.price, day2)
-        result = [data1[-i] - data2[-i] for i in range(1, min(len(data1), len(data2)) + 1)]
+        result = [
+            data1[-i] - data2[-i] for i in range(1, min(len(data1), len(data2)) + 1)
+        ]
 
         return result[::-1]
 
     def ma_bias_ratio_pivot(self, data, sample_size=5, position=False):
         """Calculate pivot point"""
         sample = data[-sample_size:]
 
         if position is True:
             check_value = max(sample)
             pre_check_value = max(sample) > 0
         elif position is False:
             check_value = min(sample)
             pre_check_value = max(sample) < 0
 
-        return ((sample_size - sample.index(check_value) < 4 and
-                 sample.index(check_value) != sample_size - 1 and pre_check_value),
-                sample_size - sample.index(check_value) - 1,
-                check_value)
+        return (
+            (
+                sample_size - sample.index(check_value) < 4
+                and sample.index(check_value) != sample_size - 1
+                and pre_check_value
+            ),
+            sample_size - sample.index(check_value) - 1,
+            check_value,
+        )
 
 
 class BestFourPoint(object):
-    BEST_BUY_WHY = ['量大收紅', '量縮價不跌', '三日均價由下往上', '三日均價大於六日均價']
-    BEST_SELL_WHY = ['量大收黑', '量縮價跌', '三日均價由上往下', '三日均價小於六日均價']
+    BEST_BUY_WHY = ["量大收紅", "量縮價不跌", "三日均價由下往上", "三日均價大於六日均價"]
+    BEST_SELL_WHY = ["量大收黑", "量縮價跌", "三日均價由上往下", "三日均價小於六日均價"]
 
     def __init__(self, stock):
         self.stock = stock
 
     def bias_ratio(self, position=False):
         return self.stock.ma_bias_ratio_pivot(
-            self.stock.ma_bias_ratio(3, 6),
-            position=position)
+            self.stock.ma_bias_ratio(3, 6), position=position
+        )
 
     def plus_bias_ratio(self):
         return self.bias_ratio(True)
 
     def mins_bias_ratio(self):
         return self.bias_ratio(False)
 
     def best_buy_1(self):
-        return (self.stock.capacity[-1] > self.stock.capacity[-2] and
-                self.stock.price[-1] > self.stock.open[-1])
+        return (
+            self.stock.capacity[-1] > self.stock.capacity[-2]
+            and self.stock.price[-1] > self.stock.open[-1]
+        )
 
     def best_buy_2(self):
-        return (self.stock.capacity[-1] < self.stock.capacity[-2] and
-                self.stock.price[-1] > self.stock.open[-2])
+        return (
+            self.stock.capacity[-1] < self.stock.capacity[-2]
+            and self.stock.price[-1] > self.stock.open[-2]
+        )
 
     def best_buy_3(self):
-        return self.stock.continuous(self.stock.moving_average(self.stock.price, 3)) == 1
+        return (
+            self.stock.continuous(self.stock.moving_average(self.stock.price, 3)) == 1
+        )
 
     def best_buy_4(self):
-        return (self.stock.moving_average(self.stock.price, 3)[-1] >
-                self.stock.moving_average(self.stock.price, 6)[-1])
+        return (
+            self.stock.moving_average(self.stock.price, 3)[-1]
+            > self.stock.moving_average(self.stock.price, 6)[-1]
+        )
 
     def best_sell_1(self):
-        return (self.stock.capacity[-1] > self.stock.capacity[-2] and
-                self.stock.price[-1] < self.stock.open[-1])
+        return (
+            self.stock.capacity[-1] > self.stock.capacity[-2]
+            and self.stock.price[-1] < self.stock.open[-1]
+        )
 
     def best_sell_2(self):
-        return (self.stock.capacity[-1] < self.stock.capacity[-2] and
-                self.stock.price[-1] < self.stock.open[-2])
+        return (
+            self.stock.capacity[-1] < self.stock.capacity[-2]
+            and self.stock.price[-1] < self.stock.open[-2]
+        )
 
     def best_sell_3(self):
-        return self.stock.continuous(self.stock.moving_average(self.stock.price, 3)) == -1
+        return (
+            self.stock.continuous(self.stock.moving_average(self.stock.price, 3)) == -1
+        )
 
     def best_sell_4(self):
-        return (self.stock.moving_average(self.stock.price, 3)[-1] <
-                self.stock.moving_average(self.stock.price, 6)[-1])
+        return (
+            self.stock.moving_average(self.stock.price, 3)[-1]
+            < self.stock.moving_average(self.stock.price, 6)[-1]
+        )
 
     def best_four_point_to_buy(self):
         result = []
-        check = [self.best_buy_1(), self.best_buy_2(),
-                 self.best_buy_3(), self.best_buy_4()]
+        check = [
+            self.best_buy_1(),
+            self.best_buy_2(),
+            self.best_buy_3(),
+            self.best_buy_4(),
+        ]
         if self.mins_bias_ratio() and any(check):
             for index, v in enumerate(check):
                 if v:
                     result.append(self.BEST_BUY_WHY[index])
         else:
             return False
-        return ', '.join(result)
+        return ", ".join(result)
 
     def best_four_point_to_sell(self):
         result = []
-        check = [self.best_sell_1(), self.best_sell_2(),
-                 self.best_sell_3(), self.best_sell_4()]
+        check = [
+            self.best_sell_1(),
+            self.best_sell_2(),
+            self.best_sell_3(),
+            self.best_sell_4(),
+        ]
         if self.plus_bias_ratio() and any(check):
             for index, v in enumerate(check):
                 if v:
                     result.append(self.BEST_SELL_WHY[index])
         else:
             return False
-        return ', '.join(result)
+        return ", ".join(result)
 
     def best_four_point(self):
         buy = self.best_four_point_to_buy()
         sell = self.best_four_point_to_sell()
         if buy:
             return (True, buy)
         elif sell:
```

### Comparing `twstock-1.3.1/twstock/cli/__init__.py` & `twstock-1.4.0/twstock/cli/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,25 +5,27 @@
 from twstock.cli import stock
 from twstock.cli import realtime
 
 
 def run():
     parser = argparse.ArgumentParser()
 
-    parser.add_argument('-b', '--bfp', nargs='+')
-    parser.add_argument('-s', '--stock', nargs='+')
-    parser.add_argument('-r', '--realtime', nargs='+')
-    parser.add_argument('-U', '--upgrade-codes', action='store_true', help='Update entites codes')
+    parser.add_argument("-b", "--bfp", nargs="+")
+    parser.add_argument("-s", "--stock", nargs="+")
+    parser.add_argument("-r", "--realtime", nargs="+")
+    parser.add_argument(
+        "-U", "--upgrade-codes", action="store_true", help="Update entites codes"
+    )
     args = parser.parse_args()
 
     if args.bfp:
         best_four_point.run(args.bfp)
     elif args.stock:
         stock.run(args.stock)
     elif args.realtime:
         realtime.run(args.realtime)
     elif args.upgrade_codes:
-        print('Start to update codes')
+        print("Start to update codes")
         __update_codes()
-        print('Done!')
+        print("Done!")
     else:
         parser.print_help()
```

### Comparing `twstock-1.3.1/twstock/cli/best_four_point.py` & `twstock-1.4.0/twstock/cli/best_four_point.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,24 +2,25 @@
 
 import io
 import sys
 import twstock
 
 # XXX: Repalce sys.stdout prevent Windows UnicodeEncodeError on cmd.exe
 stdout = io.TextIOWrapper(
-    getattr(sys.stdout, 'buffer', sys.stdout), encoding='utf-8', errors='replace')
+    getattr(sys.stdout, "buffer", sys.stdout), encoding="utf-8", errors="replace"
+)
 
 
 def run(argv):
-    print('四大買賣點判斷 Best Four Point', file=stdout)
-    print('------------------------------', file=stdout)
+    print("四大買賣點判斷 Best Four Point", file=stdout)
+    print("------------------------------", file=stdout)
     for sid in argv:
         bfp = twstock.BestFourPoint(twstock.Stock(sid))
         bfp = bfp.best_four_point()
-        print('%s: ' % (sid), end='', file=stdout)
+        print("%s: " % (sid), end="", file=stdout)
         if bfp:
             if bfp[0]:
-                print('Buy  ', bfp[1], file=stdout)
+                print("Buy  ", bfp[1], file=stdout)
             else:
-                print('Sell ', bfp[1], file=stdout)
+                print("Sell ", bfp[1], file=stdout)
         else:
             print("Don't touch", file=stdout)
```

### Comparing `twstock-1.3.1/twstock/codes/fetch.py` & `twstock-1.4.0/twstock/codes/fetch.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,56 +11,59 @@
 from collections import namedtuple
 
 import requests
 from lxml import etree
 
 from twstock.proxy import get_proxies
 
-TWSE_EQUITIES_URL = 'http://isin.twse.com.tw/isin/C_public.jsp?strMode=2'
-TPEX_EQUITIES_URL = 'http://isin.twse.com.tw/isin/C_public.jsp?strMode=4'
-ROW = namedtuple('Row', ['type', 'code', 'name', 'ISIN', 'start',
-                         'market', 'group', 'CFI'])
+TWSE_EQUITIES_URL = "https://isin.twse.com.tw/isin/C_public.jsp?strMode=2"
+TPEX_EQUITIES_URL = "https://isin.twse.com.tw/isin/C_public.jsp?strMode=4"
+ROW = namedtuple(
+    "Row", ["type", "code", "name", "ISIN", "start", "market", "group", "CFI"]
+)
 
 
 def make_row_tuple(typ, row):
-    code, name = row[1].split('\u3000')
-    return ROW(typ, code, name, *row[2: -1])
+    code, name = row[1].split("\u3000")
+    return ROW(typ, code, name, *row[2:-1])
 
 
 def fetch_data(url):
     r = requests.get(url, proxies=get_proxies())
     root = etree.HTML(r.text)
-    trs = root.xpath('//tr')[1:]
+    trs = root.xpath("//tr")[1:]
 
     result = []
-    typ = ''
+    typ = ""
     for tr in trs:
         tr = list(map(lambda x: x.text, tr.iter()))
         if len(tr) == 4:
             # This is type
-            typ = tr[2].strip(' ')
+            typ = tr[2].strip(" ")
         else:
             # This is the row data
             result.append(make_row_tuple(typ, tr))
     return result
 
 
 def to_csv(url, path):
     data = fetch_data(url)
-    with open(path, 'w', newline='', encoding='utf_8') as csvfile:
-        writer = csv.writer(csvfile,
-                            delimiter=',', quotechar='"', quoting=csv.QUOTE_MINIMAL)
+    with open(path, "w", newline="", encoding="utf_8") as csvfile:
+        writer = csv.writer(
+            csvfile, delimiter=",", quotechar='"', quoting=csv.QUOTE_MINIMAL
+        )
         writer.writerow(data[0]._fields)
         for d in data:
             writer.writerow([_ for _ in d])
 
 
 def __update_codes():
     def get_directory():
         return os.path.dirname(os.path.abspath(__file__))
-    to_csv(TWSE_EQUITIES_URL, os.path.join(get_directory(), 'twse_equities.csv'))
-    to_csv(TPEX_EQUITIES_URL, os.path.join(get_directory(), 'tpex_equities.csv'))
 
+    to_csv(TWSE_EQUITIES_URL, os.path.join(get_directory(), "twse_equities.csv"))
+    to_csv(TPEX_EQUITIES_URL, os.path.join(get_directory(), "tpex_equities.csv"))
 
-if __name__ == '__main__':
-    to_csv(TWSE_EQUITIES_URL, 'twse_equities.csv')
-    to_csv(TPEX_EQUITIES_URL, 'tpex_equities.csv')
+
+if __name__ == "__main__":
+    to_csv(TWSE_EQUITIES_URL, "twse_equities.csv")
+    to_csv(TPEX_EQUITIES_URL, "tpex_equities.csv")
```

### Comparing `twstock-1.3.1/twstock/legacy.py` & `twstock-1.4.0/twstock/legacy.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # -*- coding: utf-8 -*-
 
 
 class LegacyAnalytics(object):
     """Legacy analytics from toomore/grs"""
 
     def cal_continue(self, list_data):
-        """ 計算持續天數
+        """計算持續天數
 
-            :rtype: int
-            :returns: 向量數值：正數向上、負數向下。
+        :rtype: int
+        :returns: 向量數值：正數向上、負數向下。
         """
         diff_data = []
         for i in range(1, len(list_data)):
             if list_data[-i] > list_data[-i - 1]:
                 diff_data.append(1)
             else:
                 diff_data.append(-1)
@@ -21,191 +21,204 @@
             if value == diff_data[0]:
                 cont += 1
             else:
                 break
         return cont * diff_data[0]
 
     def moving_average(self, data, days):
-        """ 計算移動平均數
+        """計算移動平均數
 
-            :rtype: 序列 舊→新
+        :rtype: 序列 舊→新
         """
         result = []
         data = data[:]
         for dummy in range(len(data) - int(days) + 1):
             result.append(round(sum(data[-days:]) / days, 2))
             data.pop()
         result.reverse()
         return result
 
     def ma_bias_ratio(self, date1, date2, data):
-        """ 計算乖離率（均價）
-            date1 - date2
+        """計算乖離率（均價）
+        date1 - date2
 
-            :param int data1: n 日
-            :param int data2: m 日
-            :rtype: 序列 舊→新
+        :param int data1: n 日
+        :param int data2: m 日
+        :rtype: 序列 舊→新
         """
         data1 = self.moving_average(data, date1)
         data2 = self.moving_average(data, date2)
         cal_list = []
         for i in range(1, min(len(data1), len(data2)) + 1):
             cal_list.append(data1[-i] - data2[-i])
         cal_list.reverse()
         return cal_list
 
-    def ma_bias_ratio_point(cls, data, sample=5,
-                            positive_or_negative=False):
+    def ma_bias_ratio_point(cls, data, sample=5, positive_or_negative=False):
         """判斷轉折點位置
 
-           :param list data: 計算資料
-           :param int sample: 計算的區間樣本數量
-           :param bool positive_or_negative: 正乖離 為 True，負乖離 為 False
-           :rtype: tuple
-           :returns: (True or False, 第幾個轉折日, 轉折點值)
+        :param list data: 計算資料
+        :param int sample: 計算的區間樣本數量
+        :param bool positive_or_negative: 正乖離 為 True，負乖離 為 False
+        :rtype: tuple
+        :returns: (True or False, 第幾個轉折日, 轉折點值)
         """
         sample_data = data[-sample:]
         if positive_or_negative:  # 正
             ckvalue = max(sample_data)  # 尋找最大值
             preckvalue = max(sample_data) > 0  # 區間最大值必須為正
         else:
             ckvalue = min(sample_data)  # 尋找最小值
             preckvalue = max(sample_data) < 0  # 區間最大值必須為負
-        return (sample - sample_data.index(ckvalue) < 4 and \
-                sample_data.index(ckvalue) != sample - 1 and preckvalue,
-                sample - sample_data.index(ckvalue) - 1,
-                ckvalue)
+        return (
+            sample - sample_data.index(ckvalue) < 4
+            and sample_data.index(ckvalue) != sample - 1
+            and preckvalue,
+            sample - sample_data.index(ckvalue) - 1,
+            ckvalue,
+        )
 
 
 class LegacyBestFourPoint(object):
-    """ 四大買點組合
+    """四大買點組合
 
-        :param grs.Stock data: 個股資料
+    :param grs.Stock data: 個股資料
     """
+
     def __init__(self, data):
         self.data = data
 
     def bias_ratio(self, position=False):
-        """ 判斷乖離
+        """判斷乖離
 
-            :param bool positive_or_negative: 正乖離 為 True，負乖離 為 False
+        :param bool positive_or_negative: 正乖離 為 True，負乖離 為 False
         """
         return self.data.ma_bias_ratio_pivot(
-                   self.data.ma_bias_ratio(3, 6),
-                   position=position)
+            self.data.ma_bias_ratio(3, 6), position=position
+        )
 
     def check_plus_bias_ratio(self):
-        """ 正乖離扣至最大 """
+        """正乖離扣至最大"""
         return self.bias_ratio(True)
 
     def check_mins_bias_ratio(self):
-        """ 負乖離扣至最大 """
+        """負乖離扣至最大"""
         return self.bias_ratio()
 
     ##### 四大買點 #####
     def best_buy_1(self):
-        """量大收紅
-        """
-        result = self.data.capacity[-1] > self.data.capacity[-2] and \
-                 self.data.price[-1] > self.data.open[-1]
+        """量大收紅"""
+        result = (
+            self.data.capacity[-1] > self.data.capacity[-2]
+            and self.data.price[-1] > self.data.open[-1]
+        )
         return result
 
     def best_buy_2(self):
-        """量縮價不跌
-        """
-        result = self.data.capacity[-1] < self.data.capacity[-2] and \
-                 self.data.price[-1] > self.data.price[-2]
+        """量縮價不跌"""
+        result = (
+            self.data.capacity[-1] < self.data.capacity[-2]
+            and self.data.price[-1] > self.data.price[-2]
+        )
         return result
 
     def best_buy_3(self):
-        """三日均價由下往上
-        """
+        """三日均價由下往上"""
         return self.data.continuous(self.data.moving_average(self.data.price, 3)) == 1
 
     def best_buy_4(self):
-        """三日均價大於六日均價
-        """
-        return self.data.moving_average(self.data.price, 3)[-1] > \
-               self.data.moving_average(self.data.price, 6)[-1]
+        """三日均價大於六日均價"""
+        return (
+            self.data.moving_average(self.data.price, 3)[-1]
+            > self.data.moving_average(self.data.price, 6)[-1]
+        )
 
     ##### 四大賣點 #####
     def best_sell_1(self):
-        """量大收黑
-        """
-        result = self.data.capacity[-1] > self.data.capacity[-2] and \
-                 self.data.price[-1] < self.data.open[-1]
+        """量大收黑"""
+        result = (
+            self.data.capacity[-1] > self.data.capacity[-2]
+            and self.data.price[-1] < self.data.open[-1]
+        )
         return result
 
     def best_sell_2(self):
-        """量縮價跌
-        """
-        result = self.data.capacity[-1] < self.data.capacity[-2] and \
-                 self.data.price[-1] < self.data.price[-2]
+        """量縮價跌"""
+        result = (
+            self.data.capacity[-1] < self.data.capacity[-2]
+            and self.data.price[-1] < self.data.price[-2]
+        )
         return result
 
     def best_sell_3(self):
-        """三日均價由上往下
-        """
+        """三日均價由上往下"""
         return self.data.continuous(self.data.moving_average(self.data.price, 3)) == -1
 
     def best_sell_4(self):
-        """三日均價小於六日均價
-        """
-        return self.data.moving_average(self.data.price, 3)[-1] < \
-               self.data.moving_average(self.data.price, 6)[-1]
+        """三日均價小於六日均價"""
+        return (
+            self.data.moving_average(self.data.price, 3)[-1]
+            < self.data.moving_average(self.data.price, 6)[-1]
+        )
 
     def best_four_point_to_buy(self):
-        """ 判斷是否為四大買點
+        """判斷是否為四大買點
 
-            :rtype: str or False
+        :rtype: str or False
         """
         result = []
-        if self.check_mins_bias_ratio() and \
-            (self.best_buy_1() or self.best_buy_2() or self.best_buy_3() or \
-             self.best_buy_4()):
+        if self.check_mins_bias_ratio() and (
+            self.best_buy_1()
+            or self.best_buy_2()
+            or self.best_buy_3()
+            or self.best_buy_4()
+        ):
             if self.best_buy_1():
                 result.append(self.best_buy_1.__doc__.strip())
             if self.best_buy_2():
                 result.append(self.best_buy_2.__doc__.strip())
             if self.best_buy_3():
                 result.append(self.best_buy_3.__doc__.strip())
             if self.best_buy_4():
                 result.append(self.best_buy_4.__doc__.strip())
-            result = ', '.join(result)
+            result = ", ".join(result)
         else:
             result = False
         return result
 
     def best_four_point_to_sell(self):
-        """ 判斷是否為四大賣點
+        """判斷是否為四大賣點
 
-            :rtype: str or False
+        :rtype: str or False
         """
         result = []
-        if self.check_plus_bias_ratio() and \
-            (self.best_sell_1() or self.best_sell_2() or self.best_sell_3() or \
-             self.best_sell_4()):
+        if self.check_plus_bias_ratio() and (
+            self.best_sell_1()
+            or self.best_sell_2()
+            or self.best_sell_3()
+            or self.best_sell_4()
+        ):
             if self.best_sell_1():
                 result.append(self.best_sell_1.__doc__.strip())
             if self.best_sell_2():
                 result.append(self.best_sell_2.__doc__.strip())
             if self.best_sell_3():
                 result.append(self.best_sell_3.__doc__.strip())
             if self.best_sell_4():
                 result.append(self.best_sell_4.__doc__.strip())
-            result = ', '.join(result)
+            result = ", ".join(result)
         else:
             result = False
         return result
 
     def best_four_point(self):
-        """ 判斷買點或賣點
+        """判斷買點或賣點
 
-            :rtype: tuple
-            :returns: (bool, str)
+        :rtype: tuple
+        :returns: (bool, str)
         """
         buy = self.best_four_point_to_buy()
         sell = self.best_four_point_to_sell()
 
         if buy:
             return True, buy
         elif sell:
```

### Comparing `twstock-1.3.1/twstock/mock/__init__.py` & `twstock-1.4.0/twstock/mock/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,76 +1,32 @@
 # -*- coding: utf-8 -*-
 
 import json
 
 
-TSE_2330_TW = ["""
-{"msgArray": [{"ts": "0", "tk0": "2330.tw_tse_20170724_B_9999778918", "tk1":
-"2330.tw_tse_20170724_B_9999777950", "tlong": "1500860849000", "f":
-"853_1193_972_1209_817_", "ex": "tse", "g": "1221_1530_817_1038_1193_", "d":
-"20170724", "it": "12", "b": "214.00_213.50_213.00_212.50_212.00_", "c":
-"2330", "mt": "264564", "a": "214.50_215.00_215.50_216.00_216.50_", "n":
-"\u53f0\u7a4d\u96fb", "o": "213.50", "l": "213.00", "h": "214.50", "ip": "0",
-"i": "24", "w": "193.00", "v": "5094", "u": "235.00", "t": "09:47:29", "s":
-"1", "pz": "213.50", "tv": "1", "p": "0", "nf":
-"\u53f0\u7063\u7a4d\u9ad4\u96fb\u8def\u88fd\u9020\u80a1\u4efd\u6709\u9650\u516c\u53f8",
-"ch": "2330.tw",
-"z": "214.50", "y": "214.00", "ps": "1323"}], "userDelay": 5000, "rtmessage":
-"OK", "referer": "", "queryTime": {"sysTime": "09:47:30", "sessionLatestTime":
--1, "sysDate": "20170724", "sessionKey": "tse_2330.tw_20170724|",
-"sessionFromTime": -1, "stockInfoItem": 2065, "showChart": false,
-"sessionStr": "UserSession", "stockInfo": 204322}, "rtcode": "0000"}
-""", """
-{"msgArray": [{"ts": "0", "tk0": "2330.tw_tse_20170724_B_9999766224", "tk1":
-"2330.tw_tse_20170724_B_9999765954", "tlong": "1500861105000", "f":
-"1059_1079_1014_1229_907_", "ex": "tse", "g": "1455_1598_797_1019_1134_", "d":
-"20170724", "it": "12", "b": "214.00_213.50_213.00_212.50_212.00_", "c":
-"2330", "mt": "778472", "a": "214.50_215.00_215.50_216.00_216.50_", "n":
-"\u53f0\u7a4d\u96fb", "o": "213.50", "l": "213.00", "h": "214.50", "ip": "0",
-"i": "24", "w": "193.00", "v": "5217", "u": "235.00", "t": "09:51:45", "s":
-"0", "pz": "213.50", "tv": "1", "p": "0", "nf":
-"\u53f0\u7063\u7a4d\u9ad4\u96fb\u8def\u88fd\u9020\u80a1\u4efd\u6709\u9650\u516c\u53f8",
-"ch": "2330.tw",
-"z": "214.50", "y": "214.00", "ps": "1323"}], "userDelay": 5000, "rtmessage":
-"OK", "referer": "", "queryTime": {"sysTime": "09:51:48", "sessionLatestTime":
--1, "sysDate": "20170724", "sessionKey": "tse_2330.tw_20170724|",
-"sessionFromTime": -1, "stockInfoItem": 2055, "showChart": false,
-"sessionStr": "UserSession", "stockInfo": 130895}, "rtcode": "0000"}
-""", """
-{"msgArray": [{"ts": "0", "tk0": "2330.tw_tse_20170724_B_9999760446", "tk1":
-"2330.tw_tse_20170724_B_9999759382", "tlong": "1500861243000", "f":
-"1034_1028_1009_1253_933_", "ex": "tse", "g": "1466_1625_798_987_1117_", "d":
-"20170724", "it": "12", "b": "214.00_213.50_213.00_212.50_212.00_", "c":
-"2330", "mt": "962863", "a": "214.50_215.00_215.50_216.00_216.50_", "n":
-"\u53f0\u7a4d\u96fb", "o": "213.50", "l": "213.00", "h": "214.50", "ip": "0",
-"i": "24", "w": "193.00", "v": "5268", "u": "235.00", "t": "09:54:03", "s":
-"0", "pz": "213.50", "tv": "3", "p": "0", "nf":
-"\u53f0\u7063\u7a4d\u9ad4\u96fb\u8def\u88fd\u9020\u80a1\u4efd\u6709\u9650\u516c\u53f8",
-"ch": "2330.tw",
-"z": "214.00", "y": "214.00", "ps": "1323"}], "userDelay": 5000, "rtmessage":
-"OK", "referer": "", "queryTime": {"sysTime": "09:54:10", "sessionLatestTime":
--1, "sysDate": "20170724", "sessionKey": "tse_2330.tw_20170724|",
-"sessionFromTime": -1, "stockInfoItem": 1602, "showChart": false,
-"sessionStr": "UserSession", "stockInfo": 119518}, "rtcode": "0000"}
-"""]
+TSE_2330_TW = [
+    """{"msgArray": [{"tv": "-", "ps": "-", "pz": "-", "bp": "0", "a": "849.0000_850.0000_851.0000_852.0000_853.0000_", "b": "848.0000_847.0000_846.0000_845.0000_844.0000_", "c": "2330", "d": "20240516", "ch": "2330.tw", "tlong": "1715827494000", "f": "170_372_260_647_514_", "ip": "0", "g": "6_50_126_107_255_", "mt": "692836", "h": "856.0000", "i": "24", "it": "12", "l": "844.0000", "n": "\\u53f0\\u7a4d\\u96fb", "o": "852.0000", "p": "0", "ex": "tse", "s": "-", "t": "10:44:54", "u": "922.0000", "v": "23350", "w": "756.0000", "nf": "\\u53f0\\u7063\\u7a4d\\u9ad4\\u96fb\\u8def\\u88fd\\u9020\\u80a1\\u4efd\\u6709\\u9650\\u516c\\u53f8", "y": "839.0000", "z": "-", "ts": "0"}], "referer": "", "userDelay": 5000, "rtcode": "0000", "queryTime": {"sysDate": "20240516", "stockInfoItem": 2300, "stockInfo": 1107969, "sessionStr": "UserSession", "sysTime": "10:45:02", "showChart": false, "sessionFromTime": 1715827477731, "sessionLatestTime": 1715827477731}, "rtmessage": "OK", "exKey": "if_tse_2330.tw_zh-tw.null", "cachedAlive": 41360}""",
+    """{"msgArray": [{"tv": "-", "ps": "-", "pz": "-", "bp": "0", "a": "848.0000_849.0000_850.0000_851.0000_852.0000_", "b": "847.0000_846.0000_845.0000_844.0000_843.0000_", "c": "2330", "d": "20240516", "ch": "2330.tw", "tlong": "1715827560000", "f": "53_157_370_261_945_", "ip": "0", "g": "42_124_116_271_187_", "mt": "826330", "h": "856.0000", "i": "24", "it": "12", "l": "844.0000", "n": "\\u53f0\\u7a4d\\u96fb", "o": "852.0000", "p": "0", "ex": "tse", "s": "-", "t": "10:46:00", "u": "922.0000", "v": "23384", "w": "756.0000", "nf": "\\u53f0\\u7063\\u7a4d\\u9ad4\\u96fb\\u8def\\u88fd\\u9020\\u80a1\\u4efd\\u6709\\u9650\\u516c\\u53f8", "y": "839.0000", "z": "-", "ts": "0"}], "referer": "", "userDelay": 5000, "rtcode": "0000", "queryTime": {"sysDate": "20240516", "stockInfoItem": 762, "stockInfo": 270448, "sessionStr": "UserSession", "sysTime": "10:46:02", "showChart": false, "sessionFromTime": 1715827446503, "sessionLatestTime": 1715827446503}, "rtmessage": "OK", "exKey": "if_tse_2330.tw_zh-tw.null", "cachedAlive": 17846}""",
+    """{"msgArray": [{"tv": "-", "ps": "-", "pz": "-", "bp": "0", "a": "848.0000_849.0000_850.0000_851.0000_852.0000_", "b": "847.0000_846.0000_845.0000_844.0000_843.0000_", "c": "2330", "d": "20240516", "ch": "2330.tw", "tlong": "1715827579000", "f": "64_157_371_261_947_", "ip": "0", "g": "40_124_118_270_185_", "mt": "655374", "h": "856.0000", "i": "24", "it": "12", "l": "844.0000", "n": "\\u53f0\\u7a4d\\u96fb", "o": "852.0000", "p": "0", "ex": "tse", "s": "-", "t": "10:46:19", "u": "922.0000", "v": "23388", "w": "756.0000", "nf": "\\u53f0\\u7063\\u7a4d\\u9ad4\\u96fb\\u8def\\u88fd\\u9020\\u80a1\\u4efd\\u6709\\u9650\\u516c\\u53f8", "y": "839.0000", "z": "-", "ts": "0"}], "referer": "", "userDelay": 5000, "rtcode": "0000", "queryTime": {"sysDate": "20240516", "stockInfoItem": 2216, "stockInfo": 506844, "sessionStr": "UserSession", "sysTime": "10:46:25", "showChart": false, "sessionFromTime": -1, "sessionLatestTime": -1}, "rtmessage": "OK", "exKey": "if_tse_2330.tw_zh-tw.null", "cachedAlive": 21231}""",
+]
 
 
 stock_list = {
-    '2330': TSE_2330_TW,
+    "2330": TSE_2330_TW,
 }
 
 
 def get_stock_info(stock_id, index=0):
     return json.loads(stock_list[stock_id][index])
 
 
 def get_stocks_info(stocks):
-    data = json.loads(stock_list['2330'][0])
+    data = json.loads(stock_list["2330"][0])
     for _ in range(len(stocks)):
-        data['msgArray'].append(data['msgArray'][0])
+        data["msgArray"].append(data["msgArray"][0])
     return data
 
+
 def get(stocks):
     if isinstance(stocks, list):
         return get_stocks_info(stocks)
     return get_stock_info(stocks)
-
```

### Comparing `twstock-1.3.1/twstock/proxy.py` & `twstock-1.4.0/twstock/proxy.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,18 +30,18 @@
     @property
     def proxies(self):
         return self._proxies
 
     @proxies.setter
     def proxies(self, proxies: list):
         if not isinstance(proxies, list):
-            raise ValueError('Proxies only accept list')
+            raise ValueError("Proxies only accept list")
 
         self._proxies = proxies
-        self._proxies_cycle = cycle(proxies)    
+        self._proxies_cycle = cycle(proxies)
 
     def get_proxy(self):
         return next(self._proxies_cycle)
 
 
 _provider_instance = NoProxyProvier()
```

