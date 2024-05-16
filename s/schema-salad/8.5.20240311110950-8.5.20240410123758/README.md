# Comparing `tmp/schema-salad-8.5.20240311110950.tar.gz` & `tmp/schema-salad-8.5.20240410123758.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "schema-salad-8.5.20240311110950.tar", last modified: Mon Mar 11 11:29:10 2024, max compression
+gzip compressed data, was "schema-salad-8.5.20240410123758.tar", last modified: Wed Apr 10 13:09:16 2024, max compression
```

## Comparing `schema-salad-8.5.20240311110950.tar` & `schema-salad-8.5.20240410123758.tar`

### file list

```diff
@@ -1,508 +1,508 @@
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-03-11 11:29:10.539134 schema-salad-8.5.20240311110950/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-03-11 11:29:10.467133 schema-salad-8.5.20240311110950/.circleci/
--rw-r--r--   0 michael   (1000) michael   (1000)     3363 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/.circleci/config.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      324 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/.coveragerc
--rw-r--r--   0 michael   (1000) michael   (1000)      310 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/.dockerignore
--rw-r--r--   0 michael   (1000) michael   (1000)      377 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/.flake8
--rw-r--r--   0 michael   (1000) michael   (1000)      282 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/.git-blame-ignore-revs
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-03-11 11:29:10.467133 schema-salad-8.5.20240311110950/.github/
--rw-r--r--   0 michael   (1000) michael   (1000)      603 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/.github/dependabot.yml
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-03-11 11:29:10.467133 schema-salad-8.5.20240311110950/.github/workflows/
--rw-r--r--   0 michael   (1000) michael   (1000)     3621 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/.github/workflows/ci-tests.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      835 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     1102 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/.github/workflows/quay-publish.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      169 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/.github/workflows/wheel-prep.sh
--rw-r--r--   0 michael   (1000) michael   (1000)     3726 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/.github/workflows/wheels.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      219 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/.gitignore
--rw-r--r--   0 michael   (1000) michael   (1000)      113 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/.isort.cfg
--rw-r--r--   0 michael   (1000) michael   (1000)      627 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/.mergify.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    21223 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/.pylintrc
--rw-r--r--   0 michael   (1000) michael   (1000)      558 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/.readthedocs.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     1643 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/CONTRIBUTING.md
--rw-r--r--   0 michael   (1000) michael   (1000)    11358 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/LICENSE.txt
--rw-r--r--   0 michael   (1000) michael   (1000)      737 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/MANIFEST.in
--rw-r--r--   0 michael   (1000) michael   (1000)     8105 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/Makefile
--rw-r--r--   0 michael   (1000) michael   (1000)    17485 2024-03-11 11:29:10.539134 schema-salad-8.5.20240311110950/PKG-INFO
--rw-r--r--   0 michael   (1000) michael   (1000)    15769 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/README.rst
--rwxr-xr-x   0 michael   (1000) michael   (1000)      563 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/build-schema_salad-docker.sh
--rw-r--r--   0 michael   (1000) michael   (1000)       21 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/cibw-requirements.txt
--rw-r--r--   0 michael   (1000) michael   (1000)      224 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/dev-requirements.txt
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-03-11 11:29:10.467133 schema-salad-8.5.20240311110950/docs/
--rw-r--r--   0 michael   (1000) michael   (1000)      634 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/docs/Makefile
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-03-11 11:29:10.467133 schema-salad-8.5.20240311110950/docs/_static/
--rw-r--r--   0 michael   (1000) michael   (1000)    15086 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/docs/_static/favicon.ico
--rw-r--r--   0 michael   (1000) michael   (1000)      200 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/docs/cli.rst
--rw-r--r--   0 michael   (1000) michael   (1000)     3418 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/docs/conf.py
--rw-r--r--   0 michael   (1000) michael   (1000)      220 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/docs/index.rst
--rw-r--r--   0 michael   (1000) michael   (1000)      795 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/docs/make.bat
--rw-r--r--   0 michael   (1000) michael   (1000)      656 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/docs/typeshed.rst
--rw-r--r--   0 michael   (1000) michael   (1000)      325 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/lgtm.yml
--rwxr-xr-x   0 michael   (1000) michael   (1000)      819 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/manual_wheel_publish.sh
--rw-r--r--   0 michael   (1000) michael   (1000)      106 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/mypy-requirements.txt
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-03-11 11:29:10.455133 schema-salad-8.5.20240311110950/mypy-stubs/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-03-11 11:29:10.467133 schema-salad-8.5.20240311110950/mypy-stubs/cachecontrol/
--rw-r--r--   0 michael   (1000) michael   (1000)      219 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/mypy-stubs/cachecontrol/__init__.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      226 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/mypy-stubs/cachecontrol/cache.pyi
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-03-11 11:29:10.467133 schema-salad-8.5.20240311110950/mypy-stubs/cachecontrol/caches/
--rw-r--r--   0 michael   (1000) michael   (1000)      273 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/mypy-stubs/cachecontrol/caches/__init__.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      873 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/mypy-stubs/cachecontrol/caches/file_cache.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      169 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/mypy-stubs/cachecontrol/compat.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      470 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/mypy-stubs/cachecontrol/controller.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      532 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/mypy-stubs/cachecontrol/wrapper.pyi
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-03-11 11:29:10.471133 schema-salad-8.5.20240311110950/mypy-stubs/mistune/
--rw-r--r--   0 michael   (1000) michael   (1000)     1354 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/mypy-stubs/mistune/__init__.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     2448 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/mypy-stubs/mistune/block_parser.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     2810 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/mypy-stubs/mistune/core.pyi
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-03-11 11:29:10.471133 schema-salad-8.5.20240311110950/mypy-stubs/mistune/directives/
--rw-r--r--   0 michael   (1000) michael   (1000)      808 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/mypy-stubs/mistune/directives/__init__.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     2365 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/mypy-stubs/mistune/directives/_base.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1027 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/mypy-stubs/mistune/directives/_fenced.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      722 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/mypy-stubs/mistune/directives/_rst.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      751 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/mypy-stubs/mistune/directives/admonition.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      817 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/mypy-stubs/mistune/directives/image.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      679 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/mypy-stubs/mistune/directives/include.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1078 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/mypy-stubs/mistune/directives/toc.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1006 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/mypy-stubs/mistune/helpers.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     2309 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/mypy-stubs/mistune/inline_parser.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      366 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/mypy-stubs/mistune/list_parser.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1291 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/mypy-stubs/mistune/markdown.pyi
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-03-11 11:29:10.471133 schema-salad-8.5.20240311110950/mypy-stubs/mistune/plugins/
--rw-r--r--   0 michael   (1000) michael   (1000)      232 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/mypy-stubs/mistune/plugins/__init__.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)       89 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/mypy-stubs/mistune/plugins/abbr.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)       97 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/mypy-stubs/mistune/plugins/def_list.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)       99 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/mypy-stubs/mistune/plugins/footnotes.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      311 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/mypy-stubs/mistune/plugins/formatting.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      211 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/mypy-stubs/mistune/plugins/math.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      709 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/mypy-stubs/mistune/plugins/ruby.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)       95 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/mypy-stubs/mistune/plugins/speedup.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)       95 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/mypy-stubs/mistune/plugins/spoiler.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      217 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/mypy-stubs/mistune/plugins/table.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      101 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/mypy-stubs/mistune/plugins/task_lists.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)       87 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/mypy-stubs/mistune/plugins/url.pyi
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-03-11 11:29:10.475133 schema-salad-8.5.20240311110950/mypy-stubs/mistune/renderers/
--rw-r--r--   0 michael   (1000) michael   (1000)        0 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/mypy-stubs/mistune/renderers/__init__.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      259 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/mypy-stubs/mistune/renderers/_list.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1756 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/mypy-stubs/mistune/renderers/html.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     2047 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/mypy-stubs/mistune/renderers/markdown.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     2102 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/mypy-stubs/mistune/renderers/rst.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      521 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/mypy-stubs/mistune/toc.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      380 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/mypy-stubs/mistune/util.pyi
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-03-11 11:29:10.475133 schema-salad-8.5.20240311110950/mypy-stubs/rdflib/
--rw-r--r--   0 michael   (1000) michael   (1000)     1292 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/mypy-stubs/rdflib/__init__.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      674 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/mypy-stubs/rdflib/collection.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      231 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/mypy-stubs/rdflib/compare.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      182 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/mypy-stubs/rdflib/exceptions.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     8337 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/mypy-stubs/rdflib/graph.pyi
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-03-11 11:29:10.479133 schema-salad-8.5.20240311110950/mypy-stubs/rdflib/namespace/
--rw-r--r--   0 michael   (1000) michael   (1000)     2010 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/mypy-stubs/rdflib/namespace/_CSVW.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      493 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/mypy-stubs/rdflib/namespace/_DC.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1034 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/mypy-stubs/rdflib/namespace/_DCAT.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     2361 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/mypy-stubs/rdflib/namespace/_DCTERMS.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1109 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/mypy-stubs/rdflib/namespace/_DOAP.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1847 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/mypy-stubs/rdflib/namespace/_FOAF.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     4691 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/mypy-stubs/rdflib/namespace/_ODRL2.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1259 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/mypy-stubs/rdflib/namespace/_ORG.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     2260 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/mypy-stubs/rdflib/namespace/_OWL.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      441 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/mypy-stubs/rdflib/namespace/_PROF.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     4520 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/mypy-stubs/rdflib/namespace/_PROV.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1105 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/mypy-stubs/rdflib/namespace/_QB.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      620 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/mypy-stubs/rdflib/namespace/_RDF.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      519 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/mypy-stubs/rdflib/namespace/_RDFS.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)    41401 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/mypy-stubs/rdflib/namespace/_SDO.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     4965 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/mypy-stubs/rdflib/namespace/_SH.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      943 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/mypy-stubs/rdflib/namespace/_SKOS.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1075 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/mypy-stubs/rdflib/namespace/_SOSA.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      680 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/mypy-stubs/rdflib/namespace/_SSN.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     2462 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/mypy-stubs/rdflib/namespace/_TIME.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      927 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/mypy-stubs/rdflib/namespace/_VOID.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1742 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/mypy-stubs/rdflib/namespace/_XSD.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     2282 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/mypy-stubs/rdflib/namespace/__init__.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      131 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/mypy-stubs/rdflib/parser.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      724 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/mypy-stubs/rdflib/paths.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      893 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/mypy-stubs/rdflib/plugin.pyi
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-03-11 11:29:10.479133 schema-salad-8.5.20240311110950/mypy-stubs/rdflib/plugins/
--rw-r--r--   0 michael   (1000) michael   (1000)      118 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/mypy-stubs/rdflib/plugins/__init__.pyi
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-03-11 11:29:10.479133 schema-salad-8.5.20240311110950/mypy-stubs/rdflib/plugins/parsers/
--rw-r--r--   0 michael   (1000) michael   (1000)      126 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/mypy-stubs/rdflib/plugins/parsers/__init__.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)       34 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/mypy-stubs/rdflib/plugins/parsers/notation3.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1354 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/mypy-stubs/rdflib/query.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1370 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/mypy-stubs/rdflib/resource.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)     1337 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/mypy-stubs/rdflib/term.pyi
--rw-r--r--   0 michael   (1000) michael   (1000)      115 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/mypy-stubs/rdflib/util.pyi
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-03-11 11:29:10.479133 schema-salad-8.5.20240311110950/mypy-stubs/ruamel/
--rw-r--r--   0 michael   (1000) michael   (1000)        0 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/mypy-stubs/ruamel/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)      136 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/mypy.ini
--rw-r--r--   0 michael   (1000) michael   (1000)      949 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/pyproject.toml
--rwxr-xr-x   0 michael   (1000) michael   (1000)     3511 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/release-test.sh
--rw-r--r--   0 michael   (1000) michael   (1000)      210 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/requirements.txt
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-03-11 11:29:10.487133 schema-salad-8.5.20240311110950/schema_salad/
--rw-r--r--   0 michael   (1000) michael   (1000)      395 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)      110 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/__main__.py
--rw-r--r--   0 michael   (1000) michael   (1000)      437 2024-03-11 11:29:10.000000 schema-salad-8.5.20240311110950/schema_salad/_version.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-03-11 11:29:10.487133 schema-salad-8.5.20240311110950/schema_salad/avro/
--rw-r--r--   0 michael   (1000) michael   (1000)    11359 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/avro/LICENSE
--rw-r--r--   0 michael   (1000) michael   (1000)      166 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/avro/NOTICE
--rw-r--r--   0 michael   (1000) michael   (1000)      802 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/avro/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)    29458 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/avro/schema.py
--rw-r--r--   0 michael   (1000) michael   (1000)     8224 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/codegen.py
--rw-r--r--   0 michael   (1000) michael   (1000)     5130 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/codegen_base.py
--rw-r--r--   0 michael   (1000) michael   (1000)    39698 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/cpp_codegen.py
--rw-r--r--   0 michael   (1000) michael   (1000)    11181 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/dlang_codegen.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-03-11 11:29:10.491133 schema-salad-8.5.20240311110950/schema_salad/dotnet/
--rw-r--r--   0 michael   (1000) michael   (1000)       82 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/dotnet/AssemblyInfo.cs
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-03-11 11:29:10.491133 schema-salad-8.5.20240311110950/schema_salad/dotnet/DocFx/
--rw-r--r--   0 michael   (1000) michael   (1000)      445 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/dotnet/DocFx/filterConfig.yml
--rw-r--r--   0 michael   (1000) michael   (1000)       22 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/dotnet/DocFx/index.md
--rw-r--r--   0 michael   (1000) michael   (1000)       71 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/dotnet/DocFx/toc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    11356 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/dotnet/LICENSE
--rw-r--r--   0 michael   (1000) michael   (1000)     1442 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/dotnet/Project.csproj.template
--rw-r--r--   0 michael   (1000) michael   (1000)       40 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/dotnet/README.md
--rw-r--r--   0 michael   (1000) michael   (1000)     1788 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/dotnet/Solution.sln
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-03-11 11:29:10.491133 schema-salad-8.5.20240311110950/schema_salad/dotnet/Test/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-03-11 11:29:10.491133 schema-salad-8.5.20240311110950/schema_salad/dotnet/Test/data/
--rw-r--r--   0 michael   (1000) michael   (1000)        4 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/dotnet/Test/data/test.txt
--rw-r--r--   0 michael   (1000) michael   (1000)      333 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/dotnet/Test/runsettings.xml
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-03-11 11:29:10.491133 schema-salad-8.5.20240311110950/schema_salad/dotnet/Test/src/
--rw-r--r--   0 michael   (1000) michael   (1000)      207 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/dotnet/Test/src/ExampleTests.cs
--rw-r--r--   0 michael   (1000) michael   (1000)     2173 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/dotnet/Test/src/FetcherTests.cs
--rw-r--r--   0 michael   (1000) michael   (1000)     1151 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/dotnet/Test/src/UtilitiesTests.cs
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-03-11 11:29:10.491133 schema-salad-8.5.20240311110950/schema_salad/dotnet/Test/src/loaders/
--rw-r--r--   0 michael   (1000) michael   (1000)     1027 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/dotnet/Test/src/loaders/AnyLoaderTests.cs
--rw-r--r--   0 michael   (1000) michael   (1000)     1321 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/dotnet/Test/src/loaders/ArrayLoaderTests.cs
--rw-r--r--   0 michael   (1000) michael   (1000)     2429 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/dotnet/Test/src/loaders/EnumLoaderTests.cs
--rw-r--r--   0 michael   (1000) michael   (1000)      749 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/dotnet/Test/src/loaders/ExpressionLoaderTests.cs
--rw-r--r--   0 michael   (1000) michael   (1000)     1742 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/dotnet/Test/src/loaders/IdMapLoaderTests.cs
--rw-r--r--   0 michael   (1000) michael   (1000)      766 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/dotnet/Test/src/loaders/NullLoaderTests.cs
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-03-11 11:29:10.491133 schema-salad-8.5.20240311110950/schema_salad/dotnet/Test/src/loaders/PrimtiveLoader/
--rw-r--r--   0 michael   (1000) michael   (1000)     1435 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/dotnet/Test/src/loaders/PrimtiveLoader/PrimitiveLoaderDoubleTests.cs
--rw-r--r--   0 michael   (1000) michael   (1000)     1431 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/dotnet/Test/src/loaders/PrimtiveLoader/PrimitiveLoaderFloatTests.cs
--rw-r--r--   0 michael   (1000) michael   (1000)     1393 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/dotnet/Test/src/loaders/PrimtiveLoader/PrimitiveLoaderIntTests.cs
--rw-r--r--   0 michael   (1000) michael   (1000)     1246 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/dotnet/Test/src/loaders/PrimtiveLoader/PrimitiveLoaderStringTests.cs
--rw-r--r--   0 michael   (1000) michael   (1000)     1087 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/dotnet/Test/src/loaders/UnionLoaderTests.cs
--rw-r--r--   0 michael   (1000) michael   (1000)     1188 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/dotnet/Test.csproj.template
--rw-r--r--   0 michael   (1000) michael   (1000)     1459 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/dotnet/docfx.json
--rw-r--r--   0 michael   (1000) michael   (1000)    11383 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/dotnet/editorconfig
--rw-r--r--   0 michael   (1000) michael   (1000)     6894 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/dotnet/gitignore
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-03-11 11:29:10.495133 schema-salad-8.5.20240311110950/schema_salad/dotnet/util/
--rw-r--r--   0 michael   (1000) michael   (1000)     2262 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/dotnet/util/Fetcher.cs
--rw-r--r--   0 michael   (1000) michael   (1000)      167 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/dotnet/util/LoaderInstances.cs
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-03-11 11:29:10.495133 schema-salad-8.5.20240311110950/schema_salad/dotnet/util/Loaders/
--rw-r--r--   0 michael   (1000) michael   (1000)      338 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/dotnet/util/Loaders/AnyLoader.cs
--rw-r--r--   0 michael   (1000) michael   (1000)     1847 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/dotnet/util/Loaders/ArrayLoader.cs
--rw-r--r--   0 michael   (1000) michael   (1000)      905 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/dotnet/util/Loaders/EnumLoader.cs
--rw-r--r--   0 michael   (1000) michael   (1000)      646 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/dotnet/util/Loaders/ExpressionLoader.cs
--rw-r--r--   0 michael   (1000) michael   (1000)     2168 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/dotnet/util/Loaders/IdMapLoader.cs
--rw-r--r--   0 michael   (1000) michael   (1000)     4481 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/dotnet/util/Loaders/Loader.cs
--rw-r--r--   0 michael   (1000) michael   (1000)     2146 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/dotnet/util/Loaders/MapLoader.cs
--rw-r--r--   0 michael   (1000) michael   (1000)      362 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/dotnet/util/Loaders/NullLoader.cs
--rw-r--r--   0 michael   (1000) michael   (1000)      745 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/dotnet/util/Loaders/PrimitiveLoader.cs
--rw-r--r--   0 michael   (1000) michael   (1000)     1261 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/dotnet/util/Loaders/RecordLoader.cs
--rw-r--r--   0 michael   (1000) michael   (1000)     1674 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/dotnet/util/Loaders/RootLoader.cs
--rw-r--r--   0 michael   (1000) michael   (1000)     3984 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/dotnet/util/Loaders/SecondaryDSLLoader.cs
--rw-r--r--   0 michael   (1000) michael   (1000)     3056 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/dotnet/util/Loaders/TypeDSLLoader.cs
--rw-r--r--   0 michael   (1000) michael   (1000)      908 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/dotnet/util/Loaders/UnionLoader.cs
--rw-r--r--   0 michael   (1000) michael   (1000)     1995 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/dotnet/util/Loaders/UriLoader.cs
--rw-r--r--   0 michael   (1000) michael   (1000)     5665 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/dotnet/util/LoadingOptions.cs
--rw-r--r--   0 michael   (1000) michael   (1000)     4595 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/dotnet/util/Saveable.cs
--rw-r--r--   0 michael   (1000) michael   (1000)     1490 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/dotnet/util/ScalarNodeTypeResolver.cs
--rw-r--r--   0 michael   (1000) michael   (1000)      501 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/dotnet/util/UriExtensions.cs
--rw-r--r--   0 michael   (1000) michael   (1000)     1624 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/dotnet/util/Utilities.cs
--rw-r--r--   0 michael   (1000) michael   (1000)     1913 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/dotnet/util/ValidationException.cs
--rw-r--r--   0 michael   (1000) michael   (1000)      264 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/dotnet/util/Vocabs.cs
--rw-r--r--   0 michael   (1000) michael   (1000)    35889 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/dotnet_codegen.py
--rw-r--r--   0 michael   (1000) michael   (1000)     4176 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/exceptions.py
--rw-r--r--   0 michael   (1000) michael   (1000)     8412 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/fetcher.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-03-11 11:29:10.499133 schema-salad-8.5.20240311110950/schema_salad/java/
--rw-r--r--   0 michael   (1000) michael   (1000)       61 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/java/MANIFEST.MF
--rw-r--r--   0 michael   (1000) michael   (1000)      993 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/java/README.md
--rw-r--r--   0 michael   (1000) michael   (1000)        8 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/java/gitignore
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-03-11 11:29:10.503133 schema-salad-8.5.20240311110950/schema_salad/java/main_utils/
--rw-r--r--   0 michael   (1000) michael   (1000)      335 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/java/main_utils/AnyLoader.java
--rw-r--r--   0 michael   (1000) michael   (1000)     1334 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/java/main_utils/ArrayLoader.java
--rw-r--r--   0 michael   (1000) michael   (1000)      296 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/java/main_utils/ConstantMaps.java
--rw-r--r--   0 michael   (1000) michael   (1000)     1521 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/java/main_utils/DefaultFetcher.java
--rw-r--r--   0 michael   (1000) michael   (1000)      984 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/java/main_utils/EnumLoader.java
--rw-r--r--   0 michael   (1000) michael   (1000)      416 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/java/main_utils/ExpressionLoader.java
--rw-r--r--   0 michael   (1000) michael   (1000)      186 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/java/main_utils/Fetcher.java
--rw-r--r--   0 michael   (1000) michael   (1000)     1697 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/java/main_utils/IdMapLoader.java
--rw-r--r--   0 michael   (1000) michael   (1000)     4613 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/java/main_utils/Loader.java
--rw-r--r--   0 michael   (1000) michael   (1000)      125 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/java/main_utils/LoaderInstances.java
--rw-r--r--   0 michael   (1000) michael   (1000)     3989 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/java/main_utils/LoadingOptions.java
--rw-r--r--   0 michael   (1000) michael   (1000)     2641 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/java/main_utils/LoadingOptionsBuilder.java
--rw-r--r--   0 michael   (1000) michael   (1000)     1747 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/java/main_utils/MapLoader.java
--rw-r--r--   0 michael   (1000) michael   (1000)      332 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/java/main_utils/NullLoader.java
--rw-r--r--   0 michael   (1000) michael   (1000)     1113 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/java/main_utils/OneOrListOf.java
--rw-r--r--   0 michael   (1000) michael   (1000)     1050 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/java/main_utils/OneOrListOfLoader.java
--rw-r--r--   0 michael   (1000) michael   (1000)      543 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/java/main_utils/OptionalLoader.java
--rw-r--r--   0 michael   (1000) michael   (1000)      384 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/java/main_utils/PrimitiveLoader.java
--rw-r--r--   0 michael   (1000) michael   (1000)     1842 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/java/main_utils/RecordLoader.java
--rw-r--r--   0 michael   (1000) michael   (1000)     3734 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/java/main_utils/RootLoader.java
--rw-r--r--   0 michael   (1000) michael   (1000)      180 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/java/main_utils/Saveable.java
--rw-r--r--   0 michael   (1000) michael   (1000)      177 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/java/main_utils/SaveableImpl.java
--rw-r--r--   0 michael   (1000) michael   (1000)     3035 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/java/main_utils/SecondaryFilesDslLoader.java
--rw-r--r--   0 michael   (1000) michael   (1000)     2555 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/java/main_utils/TypeDslLoader.java
--rw-r--r--   0 michael   (1000) michael   (1000)     1053 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/java/main_utils/UnionLoader.java
--rw-r--r--   0 michael   (1000) michael   (1000)     1856 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/java/main_utils/UriLoader.java
--rw-r--r--   0 michael   (1000) michael   (1000)     3293 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/java/main_utils/Uris.java
--rw-r--r--   0 michael   (1000) michael   (1000)     2254 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/java/main_utils/ValidationException.java
--rw-r--r--   0 michael   (1000) michael   (1000)      789 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/java/main_utils/Validator.java
--rw-r--r--   0 michael   (1000) michael   (1000)     1025 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/java/main_utils/YamlUtils.java
--rw-r--r--   0 michael   (1000) michael   (1000)      131 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/java/main_utils/package.html
--rw-r--r--   0 michael   (1000) michael   (1000)      237 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/java/overview.html
--rw-r--r--   0 michael   (1000) michael   (1000)      187 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/java/package.html
--rw-r--r--   0 michael   (1000) michael   (1000)     5467 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/java/pom.xml
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-03-11 11:29:10.503133 schema-salad-8.5.20240311110950/schema_salad/java/test_utils/
--rw-r--r--   0 michael   (1000) michael   (1000)     1347 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/java/test_utils/DefaultFetcherTest.java
--rw-r--r--   0 michael   (1000) michael   (1000)       74 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/java/test_utils/ExamplesTest.java
--rw-r--r--   0 michael   (1000) michael   (1000)     1134 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/java/test_utils/ShortnameTest.java
--rw-r--r--   0 michael   (1000) michael   (1000)      402 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/java/test_utils/YamlUtilsTest.java
--rw-r--r--   0 michael   (1000) michael   (1000)    37505 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/java_codegen.py
--rwxr-xr-x   0 michael   (1000) michael   (1000)     8438 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/jsonld_context.py
--rw-r--r--   0 michael   (1000) michael   (1000)    14890 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/main.py
--rw-r--r--   0 michael   (1000) michael   (1000)    27263 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/makedoc.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-03-11 11:29:10.507134 schema-salad-8.5.20240311110950/schema_salad/metaschema/
--rw-r--r--   0 michael   (1000) michael   (1000)     1327 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/metaschema/field_name.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      171 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/metaschema/field_name_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      283 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/metaschema/field_name_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      171 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/metaschema/field_name_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     2442 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/metaschema/ident_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      493 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/metaschema/ident_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      473 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/metaschema/ident_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      437 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/metaschema/ident_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     3322 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/metaschema/import_include.md
--rw-r--r--   0 michael   (1000) michael   (1000)     1804 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/metaschema/link_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      411 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/metaschema/link_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      264 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/metaschema/link_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      313 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/metaschema/link_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      932 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/metaschema/map_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      183 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/metaschema/map_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      518 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/metaschema/map_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)       90 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/metaschema/map_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    13389 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/metaschema/metaschema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     5908 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/metaschema/metaschema_base.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    13923 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/metaschema/salad.md
--rw-r--r--   0 michael   (1000) michael   (1000)      882 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/metaschema/sfdsl_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      367 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/metaschema/sfdsl_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      289 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/metaschema/sfdsl_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      190 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/metaschema/sfdsl_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     1273 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/metaschema/typedsl_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      394 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/metaschema/typedsl_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      299 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/metaschema/typedsl_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      111 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/metaschema/typedsl_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      846 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/metaschema/vocab_res.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      243 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/metaschema/vocab_res_proc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      345 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/metaschema/vocab_res_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      267 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/metaschema/vocab_res_src.yml
--rw-r--r--   0 michael   (1000) michael   (1000)   278658 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/metaschema.py
--rw-r--r--   0 michael   (1000) michael   (1000)        0 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/py.typed
--rw-r--r--   0 michael   (1000) michael   (1000)    27678 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/python_codegen.py
--rw-r--r--   0 michael   (1000) michael   (1000)    39328 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/python_codegen_support.py
--rw-r--r--   0 michael   (1000) michael   (1000)    47501 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/ref_resolver.py
--rw-r--r--   0 michael   (1000) michael   (1000)    30704 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/schema.py
--rw-r--r--   0 michael   (1000) michael   (1000)     9000 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/sourceline.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-03-11 11:29:10.519134 schema-salad-8.5.20240311110950/schema_salad/tests/
--rw-r--r--   0 michael   (1000) michael   (1000)  2615816 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/EDAM.owl
--rw-r--r--   0 michael   (1000) michael   (1000)      827 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/Process.yml
--rw-r--r--   0 michael   (1000) michael   (1000)        0 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)      125 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/bad_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)       65 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/bad_schema2.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      140 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/basket.yml
--rw-r--r--   0 michael   (1000) michael   (1000)     1267 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/basket_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      590 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/class_field_test.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      452 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/conftest.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-03-11 11:29:10.523134 schema-salad-8.5.20240311110950/schema_salad/tests/cpp_tests/
--rw-r--r--   0 michael   (1000) michael   (1000)    10312 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/cpp_tests/01_single_record.h
--rw-r--r--   0 michael   (1000) michael   (1000)      140 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/cpp_tests/01_single_record.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    11531 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/cpp_tests/02_two_records.h
--rw-r--r--   0 michael   (1000) michael   (1000)      210 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/cpp_tests/02_two_records.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    11693 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/cpp_tests/03_simple_inheritance.h
--rw-r--r--   0 michael   (1000) michael   (1000)      235 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/cpp_tests/03_simple_inheritance.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    11184 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/cpp_tests/04_abstract_inheritance.h
--rw-r--r--   0 michael   (1000) michael   (1000)      252 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/cpp_tests/04_abstract_inheritance.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    13621 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/cpp_tests/05_specialization.h
--rw-r--r--   0 michael   (1000) michael   (1000)      440 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/cpp_tests/05_specialization.yml
--rw-r--r--   0 michael   (1000) michael   (1000)   133826 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/cwl-pre.yml
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-03-11 11:29:10.523134 schema-salad-8.5.20240311110950/schema_salad/tests/docimp/
--rw-r--r--   0 michael   (1000) michael   (1000)      155 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/docimp/d1.yml
--rw-r--r--   0 michael   (1000) michael   (1000)        7 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/docimp/d2.md
--rw-r--r--   0 michael   (1000) michael   (1000)       42 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/docimp/d3.yml
--rw-r--r--   0 michael   (1000) michael   (1000)       42 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/docimp/d4.yml
--rw-r--r--   0 michael   (1000) michael   (1000)       18 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/docimp/d5.md
--rw-r--r--   0 michael   (1000) michael   (1000)      320 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/docimp/dpre.json
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-03-11 11:29:10.523134 schema-salad-8.5.20240311110950/schema_salad/tests/foreign/
--rwxr-xr-x   0 michael   (1000) michael   (1000)      347 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/foreign/foreign_prop1.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      302 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/foreign/foreign_prop2.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      436 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/foreign/foreign_prop3.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      390 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/foreign/foreign_prop4.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      428 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/foreign/foreign_prop5.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      294 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/foreign/foreign_prop6.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      292 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/foreign/foreign_prop7.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      493 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/formattest2.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)       41 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/frag.yml
--rw-r--r--   0 michael   (1000) michael   (1000)       13 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/hello.txt
--rw-r--r--   0 michael   (1000) michael   (1000)       71 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/hellofield.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      946 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/inherited-attributes.yml
--rw-r--r--   0 michael   (1000) michael   (1000)       17 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/inject-id1.yml
--rw-r--r--   0 michael   (1000) michael   (1000)        9 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/inject-id2.yml
--rw-r--r--   0 michael   (1000) michael   (1000)       32 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/inject-id3.yml
--rw-r--r--   0 michael   (1000) michael   (1000)       25 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/list.json
--rw-r--r--   0 michael   (1000) michael   (1000)     1241 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/matcher.py
--rw-r--r--   0 michael   (1000) michael   (1000)      331 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/memory-leak-check.py
--rw-r--r--   0 michael   (1000) michael   (1000)    66980 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/metaschema-pre.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      208 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/missing_step_name.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)       18 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/mixin.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      154 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/multidoc.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      900 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/pt.yml
--rwxr-xr-x   0 michael   (1000) michael   (1000)     1466 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/revtool_bad_schema.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      519 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/test_avro_names.py
--rw-r--r--   0 michael   (1000) michael   (1000)     7519 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/test_cg.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1146 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/test_cli_args.py
--rw-r--r--   0 michael   (1000) michael   (1000)     9903 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/test_codegen_errors.py
--rw-r--r--   0 michael   (1000) michael   (1000)     4428 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/test_cpp_codegen.py
--rw-r--r--   0 michael   (1000) michael   (1000)     2420 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/test_cwl11.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1071 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/test_dlang_codegen.py
--rw-r--r--   0 michael   (1000) michael   (1000)     3366 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/test_dotnet_codegen.py
--rw-r--r--   0 michael   (1000) michael   (1000)    15568 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/test_errors.py
--rw-r--r--   0 michael   (1000) michael   (1000)    20481 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/test_examples.py
--rw-r--r--   0 michael   (1000) michael   (1000)     2650 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/test_fetch.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1603 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/test_fp.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1868 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/test_java_codegen.py
--rw-r--r--   0 michael   (1000) michael   (1000)     9242 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/test_makedoc.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1334 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/test_misc.py
--rw-r--r--   0 michael   (1000) michael   (1000)      818 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/test_pickling.py
--rw-r--r--   0 michael   (1000) michael   (1000)     6218 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/test_print_oneline.py
--rw-r--r--   0 michael   (1000) michael   (1000)     4547 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/test_python_codegen.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-03-11 11:29:10.523134 schema-salad-8.5.20240311110950/schema_salad/tests/test_real_cwl/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-03-11 11:29:10.523134 schema-salad-8.5.20240311110950/schema_salad/tests/test_real_cwl/ICGC-TCGA-PanCancer/
--rw-r--r--   0 michael   (1000) michael   (1000)      227 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/test_real_cwl/ICGC-TCGA-PanCancer/PreprocessedFilesType.yaml
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-03-11 11:29:10.523134 schema-salad-8.5.20240311110950/schema_salad/tests/test_real_cwl/ICGC-TCGA-PanCancer/complete/
--rw-r--r--   0 michael   (1000) michael   (1000)      227 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/test_real_cwl/ICGC-TCGA-PanCancer/complete/PreprocessedFilesType.yaml
--rw-r--r--   0 michael   (1000) michael   (1000)      648 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/test_real_cwl/ICGC-TCGA-PanCancer/complete/clean_vcf.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      666 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/test_real_cwl/ICGC-TCGA-PanCancer/complete/extract_snv.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      783 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/test_real_cwl/ICGC-TCGA-PanCancer/complete/normalize.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      902 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/test_real_cwl/ICGC-TCGA-PanCancer/complete/pass-filter.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      912 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/test_real_cwl/ICGC-TCGA-PanCancer/complete/preprocess_util.js
--rwxr-xr-x   0 michael   (1000) michael   (1000)    12007 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/test_real_cwl/ICGC-TCGA-PanCancer/complete/preprocess_vcf.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     2352 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/test_real_cwl/ICGC-TCGA-PanCancer/complete/vcf_merge.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      148 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/test_real_cwl/ICGC-TCGA-PanCancer/complete/vcf_merge_util.js
--rw-r--r--   0 michael   (1000) michael   (1000)      912 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/test_real_cwl/ICGC-TCGA-PanCancer/preprocess_util.js
--rwxr-xr-x   0 michael   (1000) michael   (1000)    12007 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/test_real_cwl/ICGC-TCGA-PanCancer/preprocess_vcf.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)      148 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/test_real_cwl/ICGC-TCGA-PanCancer/vcf_merge_util.js
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-03-11 11:29:10.527134 schema-salad-8.5.20240311110950/schema_salad/tests/test_real_cwl/bio-cwl-tools/
--rwxr-xr-x   0 michael   (1000) michael   (1000)     4732 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/test_real_cwl/bio-cwl-tools/bamtools_stats.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)     4701 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/test_real_cwl/bio-cwl-tools/bamtools_stats_invalid_schema_ref.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     5757 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/test_real_cwl/bio-cwl-tools/picard_CreateSequenceDictionary.cwl
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-03-11 11:29:10.527134 schema-salad-8.5.20240311110950/schema_salad/tests/test_real_cwl/h3agatk/
--rwxr-xr-x   0 michael   (1000) michael   (1000)     1905 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/test_real_cwl/h3agatk/GATK-Sub-Workflow-h3abionet-snp.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)    10910 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/test_real_cwl/h3agatk/GATK-complete-WES-Workflow-h3abionet.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     1122 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/test_real_cwl/tabs_rna_seq_workflow.cwl
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-03-11 11:29:10.527134 schema-salad-8.5.20240311110950/schema_salad/tests/test_real_cwl/topmed/
--rwxr-xr-x   0 michael   (1000) michael   (1000)     5976 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/test_real_cwl/topmed/topmed_variant_calling_pipeline.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     2231 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/test_real_cwl.py
--rw-r--r--   0 michael   (1000) michael   (1000)     9624 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/test_ref_resolver.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-03-11 11:29:10.535134 schema-salad-8.5.20240311110950/schema_salad/tests/test_schema/
--rw-r--r--   0 michael   (1000) michael   (1000)    19840 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/test_schema/Base.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    36450 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/test_schema/CommandLineTool.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      209 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/test_schema/CommonWorkflowLanguage.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    16131 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/test_schema/Process.yml
--rw-r--r--   0 michael   (1000) michael   (1000)    22914 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/test_schema/Workflow.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      453 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/test_schema/avro_naming.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      529 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/test_schema/avro_naming_base.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      529 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/test_schema/avro_subtype.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      524 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/test_schema/avro_subtype_bad.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      814 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/test_schema/avro_subtype_nested.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      818 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/test_schema/avro_subtype_nested_bad.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      679 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/test_schema/avro_subtype_recursive.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      865 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/test_schema/avro_subtype_union.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      869 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/test_schema/avro_subtype_union_bad.yml
--rw-r--r--   0 michael   (1000) michael   (1000)        1 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/test_schema/concepts.md
--rw-r--r--   0 michael   (1000) michael   (1000)        1 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/test_schema/contrib.md
--rw-r--r--   0 michael   (1000) michael   (1000)      514 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/test_schema/cwltest-schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)        1 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/test_schema/intro.md
--rw-r--r--   0 michael   (1000) michael   (1000)        1 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/test_schema/invocation.md
--rw-r--r--   0 michael   (1000) michael   (1000)     5774 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/test_schema/metaschema_base.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      514 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/test_schema/misc_schema_v1.yml
--rw-r--r--   0 michael   (1000) michael   (1000)      575 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/test_schema/misc_schema_v2.yml
--rw-r--r--   0 michael   (1000) michael   (1000)       54 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/test_schema/no_field_schema.yml
--rw-r--r--   0 michael   (1000) michael   (1000)       70 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/test_schema/one_line_primary_doc.yml
--rwxr-xr-x   0 michael   (1000) michael   (1000)       58 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/test_schema/test1.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      174 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/test_schema/test10.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      164 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/test_schema/test11.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      299 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/test_schema/test12.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      302 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/test_schema/test13.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      208 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/test_schema/test14.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      247 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/test_schema/test15.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      274 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/test_schema/test16.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      238 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/test_schema/test17.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      241 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/test_schema/test18.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      269 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/test_schema/test19.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)       59 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/test_schema/test2.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      115 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/test_schema/test3.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      110 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/test_schema/test4.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      116 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/test_schema/test5.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      100 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/test_schema/test6.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      171 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/test_schema/test7.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      169 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/test_schema/test8.cwl
--rwxr-xr-x   0 michael   (1000) michael   (1000)      168 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/test_schema/test9.cwl
--rw-r--r--   0 michael   (1000) michael   (1000)     1233 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/test_schema.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1536 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/test_schemas_directive.py
--rw-r--r--   0 michael   (1000) michael   (1000)     5593 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/test_subtypes.py
--rw-r--r--   0 michael   (1000) michael   (1000)     3412 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/test_typescript_codegen.py
--rw-r--r--   0 michael   (1000) michael   (1000)     1816 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/tests/util.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-03-11 11:29:10.535134 schema-salad-8.5.20240311110950/schema_salad/typescript/
--rw-r--r--   0 michael   (1000) michael   (1000)     1617 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/typescript/.gitignore
--rw-r--r--   0 michael   (1000) michael   (1000)    11357 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/typescript/LICENSE
--rw-r--r--   0 michael   (1000) michael   (1000)      138 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/typescript/index.ts
--rw-r--r--   0 michael   (1000) michael   (1000)     1082 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/typescript/package.json
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-03-11 11:29:10.535134 schema-salad-8.5.20240311110950/schema_salad/typescript/test/
--rw-r--r--   0 michael   (1000) michael   (1000)      879 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/typescript/test/AnyLoader.spec.ts
--rw-r--r--   0 michael   (1000) michael   (1000)      147 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/typescript/test/ExampleTest.ts
--rw-r--r--   0 michael   (1000) michael   (1000)     3118 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/typescript/test/Fetcher.spec.ts
--rw-r--r--   0 michael   (1000) michael   (1000)     1390 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/typescript/test/IdMap.spec.ts
--rw-r--r--   0 michael   (1000) michael   (1000)     3265 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/typescript/test/Typeguards.spec.ts
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-03-11 11:29:10.535134 schema-salad-8.5.20240311110950/schema_salad/typescript/test/data/
--rw-r--r--   0 michael   (1000) michael   (1000)       70 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/typescript/test/data/hellofield.yml
--rw-r--r--   0 michael   (1000) michael   (1000)        5 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/typescript/test/data/test.txt
--rw-r--r--   0 michael   (1000) michael   (1000)     1418 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/typescript/test/utilities.spec.ts
--rw-r--r--   0 michael   (1000) michael   (1000)      541 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/typescript/tsconfig.json
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-03-11 11:29:10.535134 schema-salad-8.5.20240311110950/schema_salad/typescript/util/
--rw-r--r--   0 michael   (1000) michael   (1000)       60 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/typescript/util/Dict.ts
--rw-r--r--   0 michael   (1000) michael   (1000)     2336 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/typescript/util/Fetcher.ts
--rw-r--r--   0 michael   (1000) michael   (1000)      896 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/typescript/util/Internal.ts
--rw-r--r--   0 michael   (1000) michael   (1000)      296 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/typescript/util/LoaderInstances.ts
--rw-r--r--   0 michael   (1000) michael   (1000)     1915 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/typescript/util/LoadingOptions.ts
--rw-r--r--   0 michael   (1000) michael   (1000)     3536 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/typescript/util/Saveable.ts
--rw-r--r--   0 michael   (1000) michael   (1000)      593 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/typescript/util/Typeguards.ts
--rw-r--r--   0 michael   (1000) michael   (1000)     1406 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/typescript/util/ValidationException.ts
--rw-r--r--   0 michael   (1000) michael   (1000)       74 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/typescript/util/Vocabs.ts
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-03-11 11:29:10.539134 schema-salad-8.5.20240311110950/schema_salad/typescript/util/loaders/
--rw-r--r--   0 michael   (1000) michael   (1000)      345 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/typescript/util/loaders/AnyLoader.ts
--rw-r--r--   0 michael   (1000) michael   (1000)     1085 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/typescript/util/loaders/ArrayLoader.ts
--rw-r--r--   0 michael   (1000) michael   (1000)      481 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/typescript/util/loaders/EnumLoader.ts
--rw-r--r--   0 michael   (1000) michael   (1000)      350 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/typescript/util/loaders/ExpressionLoader.ts
--rw-r--r--   0 michael   (1000) michael   (1000)     1180 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/typescript/util/loaders/IdMapLoader.ts
--rw-r--r--   0 michael   (1000) michael   (1000)     3228 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/typescript/util/loaders/Loader.ts
--rw-r--r--   0 michael   (1000) michael   (1000)     1307 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/typescript/util/loaders/MapLoader.ts
--rw-r--r--   0 michael   (1000) michael   (1000)      497 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/typescript/util/loaders/PrimitiveLoader.ts
--rw-r--r--   0 michael   (1000) michael   (1000)     1086 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/typescript/util/loaders/RecordLoader.ts
--rw-r--r--   0 michael   (1000) michael   (1000)     2508 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/typescript/util/loaders/RootLoader.ts
--rw-r--r--   0 michael   (1000) michael   (1000)     2421 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/typescript/util/loaders/SecondaryDSLLoader.ts
--rw-r--r--   0 michael   (1000) michael   (1000)     1776 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/typescript/util/loaders/TypeDSLLoader.ts
--rw-r--r--   0 michael   (1000) michael   (1000)      865 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/typescript/util/loaders/UnionLoader.ts
--rw-r--r--   0 michael   (1000) michael   (1000)     1276 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/typescript/util/loaders/UriLoader.ts
--rw-r--r--   0 michael   (1000) michael   (1000)    31625 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/typescript_codegen.py
--rw-r--r--   0 michael   (1000) michael   (1000)     4186 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/utils.py
--rw-r--r--   0 michael   (1000) michael   (1000)    15955 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad/validate.py
--rw-r--r--   0 michael   (1000) michael   (1000)      841 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/schema_salad.Dockerfile
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-03-11 11:29:10.539134 schema-salad-8.5.20240311110950/schema_salad.egg-info/
--rw-r--r--   0 michael   (1000) michael   (1000)    17485 2024-03-11 11:29:10.000000 schema-salad-8.5.20240311110950/schema_salad.egg-info/PKG-INFO
--rw-r--r--   0 michael   (1000) michael   (1000)    18361 2024-03-11 11:29:10.000000 schema-salad-8.5.20240311110950/schema_salad.egg-info/SOURCES.txt
--rw-r--r--   0 michael   (1000) michael   (1000)        1 2024-03-11 11:29:10.000000 schema-salad-8.5.20240311110950/schema_salad.egg-info/dependency_links.txt
--rw-r--r--   0 michael   (1000) michael   (1000)      106 2024-03-11 11:29:10.000000 schema-salad-8.5.20240311110950/schema_salad.egg-info/entry_points.txt
--rw-r--r--   0 michael   (1000) michael   (1000)      317 2024-03-11 11:29:10.000000 schema-salad-8.5.20240311110950/schema_salad.egg-info/requires.txt
--rw-r--r--   0 michael   (1000) michael   (1000)       13 2024-03-11 11:29:10.000000 schema-salad-8.5.20240311110950/schema_salad.egg-info/top_level.txt
--rw-r--r--   0 michael   (1000) michael   (1000)        1 2024-03-11 11:17:32.000000 schema-salad-8.5.20240311110950/schema_salad.egg-info/zip-safe
--rw-r--r--   0 michael   (1000) michael   (1000)       95 2024-03-11 11:29:10.539134 schema-salad-8.5.20240311110950/setup.cfg
--rw-r--r--   0 michael   (1000) michael   (1000)     5533 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/setup.py
--rw-r--r--   0 michael   (1000) michael   (1000)       75 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/test-requirements.txt
--rw-r--r--   0 michael   (1000) michael   (1000)     2493 2024-03-11 11:17:12.000000 schema-salad-8.5.20240311110950/tox.ini
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:09:16.052068 schema-salad-8.5.20240410123758/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:09:16.004067 schema-salad-8.5.20240410123758/.circleci/
+-rw-r--r--   0 michael   (1000) michael   (1000)     2908 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/.circleci/config.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      324 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/.coveragerc
+-rw-r--r--   0 michael   (1000) michael   (1000)      310 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/.dockerignore
+-rw-r--r--   0 michael   (1000) michael   (1000)      377 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/.flake8
+-rw-r--r--   0 michael   (1000) michael   (1000)      282 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/.git-blame-ignore-revs
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:09:16.004067 schema-salad-8.5.20240410123758/.github/
+-rw-r--r--   0 michael   (1000) michael   (1000)      603 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/.github/dependabot.yml
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:09:16.004067 schema-salad-8.5.20240410123758/.github/workflows/
+-rw-r--r--   0 michael   (1000) michael   (1000)     3621 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/.github/workflows/ci-tests.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      835 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     1102 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/.github/workflows/quay-publish.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     3961 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/.github/workflows/wheels.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      219 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/.gitignore
+-rw-r--r--   0 michael   (1000) michael   (1000)      113 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/.isort.cfg
+-rw-r--r--   0 michael   (1000) michael   (1000)      627 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/.mergify.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    21223 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/.pylintrc
+-rw-r--r--   0 michael   (1000) michael   (1000)      558 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/.readthedocs.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     1643 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/CONTRIBUTING.md
+-rw-r--r--   0 michael   (1000) michael   (1000)    11358 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/LICENSE.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)      737 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/MANIFEST.in
+-rw-r--r--   0 michael   (1000) michael   (1000)     8105 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/Makefile
+-rw-r--r--   0 michael   (1000) michael   (1000)    17485 2024-04-10 13:09:16.052068 schema-salad-8.5.20240410123758/PKG-INFO
+-rw-r--r--   0 michael   (1000) michael   (1000)    15769 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/README.rst
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      563 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/build-schema_salad-docker.sh
+-rw-r--r--   0 michael   (1000) michael   (1000)       21 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/cibw-requirements.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)      224 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/dev-requirements.txt
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:09:16.004067 schema-salad-8.5.20240410123758/docs/
+-rw-r--r--   0 michael   (1000) michael   (1000)      634 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/docs/Makefile
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:09:16.004067 schema-salad-8.5.20240410123758/docs/_static/
+-rw-r--r--   0 michael   (1000) michael   (1000)    15086 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/docs/_static/favicon.ico
+-rw-r--r--   0 michael   (1000) michael   (1000)      200 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/docs/cli.rst
+-rw-r--r--   0 michael   (1000) michael   (1000)     3418 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/docs/conf.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      220 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/docs/index.rst
+-rw-r--r--   0 michael   (1000) michael   (1000)      795 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/docs/make.bat
+-rw-r--r--   0 michael   (1000) michael   (1000)      656 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/docs/typeshed.rst
+-rw-r--r--   0 michael   (1000) michael   (1000)      325 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/lgtm.yml
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      819 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/manual_wheel_publish.sh
+-rw-r--r--   0 michael   (1000) michael   (1000)      106 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/mypy-requirements.txt
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:09:16.000067 schema-salad-8.5.20240410123758/mypy-stubs/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:09:16.004067 schema-salad-8.5.20240410123758/mypy-stubs/cachecontrol/
+-rw-r--r--   0 michael   (1000) michael   (1000)      219 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/mypy-stubs/cachecontrol/__init__.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      226 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/mypy-stubs/cachecontrol/cache.pyi
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:09:16.004067 schema-salad-8.5.20240410123758/mypy-stubs/cachecontrol/caches/
+-rw-r--r--   0 michael   (1000) michael   (1000)      273 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/mypy-stubs/cachecontrol/caches/__init__.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      873 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/mypy-stubs/cachecontrol/caches/file_cache.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      169 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/mypy-stubs/cachecontrol/compat.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      470 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/mypy-stubs/cachecontrol/controller.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      532 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/mypy-stubs/cachecontrol/wrapper.pyi
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:09:16.008067 schema-salad-8.5.20240410123758/mypy-stubs/mistune/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1354 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/mypy-stubs/mistune/__init__.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     2448 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/mypy-stubs/mistune/block_parser.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     2810 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/mypy-stubs/mistune/core.pyi
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:09:16.008067 schema-salad-8.5.20240410123758/mypy-stubs/mistune/directives/
+-rw-r--r--   0 michael   (1000) michael   (1000)      808 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/mypy-stubs/mistune/directives/__init__.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     2365 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/mypy-stubs/mistune/directives/_base.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1027 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/mypy-stubs/mistune/directives/_fenced.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      722 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/mypy-stubs/mistune/directives/_rst.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      751 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/mypy-stubs/mistune/directives/admonition.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      817 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/mypy-stubs/mistune/directives/image.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      679 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/mypy-stubs/mistune/directives/include.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1078 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/mypy-stubs/mistune/directives/toc.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1006 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/mypy-stubs/mistune/helpers.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     2309 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/mypy-stubs/mistune/inline_parser.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      366 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/mypy-stubs/mistune/list_parser.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1291 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/mypy-stubs/mistune/markdown.pyi
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:09:16.008067 schema-salad-8.5.20240410123758/mypy-stubs/mistune/plugins/
+-rw-r--r--   0 michael   (1000) michael   (1000)      232 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/mypy-stubs/mistune/plugins/__init__.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)       89 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/mypy-stubs/mistune/plugins/abbr.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)       97 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/mypy-stubs/mistune/plugins/def_list.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)       99 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/mypy-stubs/mistune/plugins/footnotes.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      311 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/mypy-stubs/mistune/plugins/formatting.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      211 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/mypy-stubs/mistune/plugins/math.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      709 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/mypy-stubs/mistune/plugins/ruby.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)       95 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/mypy-stubs/mistune/plugins/speedup.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)       95 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/mypy-stubs/mistune/plugins/spoiler.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      217 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/mypy-stubs/mistune/plugins/table.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      101 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/mypy-stubs/mistune/plugins/task_lists.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)       87 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/mypy-stubs/mistune/plugins/url.pyi
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:09:16.008067 schema-salad-8.5.20240410123758/mypy-stubs/mistune/renderers/
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/mypy-stubs/mistune/renderers/__init__.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      259 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/mypy-stubs/mistune/renderers/_list.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1756 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/mypy-stubs/mistune/renderers/html.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     2047 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/mypy-stubs/mistune/renderers/markdown.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     2102 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/mypy-stubs/mistune/renderers/rst.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      521 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/mypy-stubs/mistune/toc.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      380 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/mypy-stubs/mistune/util.pyi
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:09:16.012067 schema-salad-8.5.20240410123758/mypy-stubs/rdflib/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1292 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/mypy-stubs/rdflib/__init__.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      674 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/mypy-stubs/rdflib/collection.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      231 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/mypy-stubs/rdflib/compare.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      182 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/mypy-stubs/rdflib/exceptions.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     8337 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/mypy-stubs/rdflib/graph.pyi
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:09:16.012067 schema-salad-8.5.20240410123758/mypy-stubs/rdflib/namespace/
+-rw-r--r--   0 michael   (1000) michael   (1000)     2010 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/mypy-stubs/rdflib/namespace/_CSVW.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      493 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/mypy-stubs/rdflib/namespace/_DC.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1034 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/mypy-stubs/rdflib/namespace/_DCAT.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     2361 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/mypy-stubs/rdflib/namespace/_DCTERMS.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1109 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/mypy-stubs/rdflib/namespace/_DOAP.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1847 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/mypy-stubs/rdflib/namespace/_FOAF.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     4691 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/mypy-stubs/rdflib/namespace/_ODRL2.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1259 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/mypy-stubs/rdflib/namespace/_ORG.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     2260 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/mypy-stubs/rdflib/namespace/_OWL.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      441 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/mypy-stubs/rdflib/namespace/_PROF.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     4520 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/mypy-stubs/rdflib/namespace/_PROV.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1105 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/mypy-stubs/rdflib/namespace/_QB.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      620 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/mypy-stubs/rdflib/namespace/_RDF.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      519 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/mypy-stubs/rdflib/namespace/_RDFS.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)    41401 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/mypy-stubs/rdflib/namespace/_SDO.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     4965 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/mypy-stubs/rdflib/namespace/_SH.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      943 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/mypy-stubs/rdflib/namespace/_SKOS.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1075 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/mypy-stubs/rdflib/namespace/_SOSA.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      680 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/mypy-stubs/rdflib/namespace/_SSN.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     2462 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/mypy-stubs/rdflib/namespace/_TIME.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      927 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/mypy-stubs/rdflib/namespace/_VOID.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1742 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/mypy-stubs/rdflib/namespace/_XSD.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     2282 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/mypy-stubs/rdflib/namespace/__init__.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      131 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/mypy-stubs/rdflib/parser.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      724 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/mypy-stubs/rdflib/paths.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      893 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/mypy-stubs/rdflib/plugin.pyi
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:09:16.012067 schema-salad-8.5.20240410123758/mypy-stubs/rdflib/plugins/
+-rw-r--r--   0 michael   (1000) michael   (1000)      118 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/mypy-stubs/rdflib/plugins/__init__.pyi
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:09:16.012067 schema-salad-8.5.20240410123758/mypy-stubs/rdflib/plugins/parsers/
+-rw-r--r--   0 michael   (1000) michael   (1000)      126 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/mypy-stubs/rdflib/plugins/parsers/__init__.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)       34 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/mypy-stubs/rdflib/plugins/parsers/notation3.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1354 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/mypy-stubs/rdflib/query.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1370 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/mypy-stubs/rdflib/resource.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)     1337 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/mypy-stubs/rdflib/term.pyi
+-rw-r--r--   0 michael   (1000) michael   (1000)      115 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/mypy-stubs/rdflib/util.pyi
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:09:16.012067 schema-salad-8.5.20240410123758/mypy-stubs/ruamel/
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/mypy-stubs/ruamel/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      136 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/mypy.ini
+-rw-r--r--   0 michael   (1000) michael   (1000)      942 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/pyproject.toml
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     3511 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/release-test.sh
+-rw-r--r--   0 michael   (1000) michael   (1000)      210 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/requirements.txt
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:09:16.016067 schema-salad-8.5.20240410123758/schema_salad/
+-rw-r--r--   0 michael   (1000) michael   (1000)      395 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      110 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/__main__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      437 2024-04-10 13:09:15.000000 schema-salad-8.5.20240410123758/schema_salad/_version.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:09:16.016067 schema-salad-8.5.20240410123758/schema_salad/avro/
+-rw-r--r--   0 michael   (1000) michael   (1000)    11359 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/avro/LICENSE
+-rw-r--r--   0 michael   (1000) michael   (1000)      166 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/avro/NOTICE
+-rw-r--r--   0 michael   (1000) michael   (1000)      802 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/avro/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    29458 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/avro/schema.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     8224 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/codegen.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     5130 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/codegen_base.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    39698 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/cpp_codegen.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    11181 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/dlang_codegen.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:09:16.020068 schema-salad-8.5.20240410123758/schema_salad/dotnet/
+-rw-r--r--   0 michael   (1000) michael   (1000)       82 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/dotnet/AssemblyInfo.cs
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:09:16.020068 schema-salad-8.5.20240410123758/schema_salad/dotnet/DocFx/
+-rw-r--r--   0 michael   (1000) michael   (1000)      445 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/dotnet/DocFx/filterConfig.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)       22 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/dotnet/DocFx/index.md
+-rw-r--r--   0 michael   (1000) michael   (1000)       71 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/dotnet/DocFx/toc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    11356 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/dotnet/LICENSE
+-rw-r--r--   0 michael   (1000) michael   (1000)     1442 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/dotnet/Project.csproj.template
+-rw-r--r--   0 michael   (1000) michael   (1000)       40 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/dotnet/README.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     1788 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/dotnet/Solution.sln
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:09:16.020068 schema-salad-8.5.20240410123758/schema_salad/dotnet/Test/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:09:16.020068 schema-salad-8.5.20240410123758/schema_salad/dotnet/Test/data/
+-rw-r--r--   0 michael   (1000) michael   (1000)        4 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/dotnet/Test/data/test.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)      333 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/dotnet/Test/runsettings.xml
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:09:16.020068 schema-salad-8.5.20240410123758/schema_salad/dotnet/Test/src/
+-rw-r--r--   0 michael   (1000) michael   (1000)      207 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/dotnet/Test/src/ExampleTests.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)     2173 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/dotnet/Test/src/FetcherTests.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)     1151 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/dotnet/Test/src/UtilitiesTests.cs
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:09:16.020068 schema-salad-8.5.20240410123758/schema_salad/dotnet/Test/src/loaders/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1027 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/dotnet/Test/src/loaders/AnyLoaderTests.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)     1321 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/dotnet/Test/src/loaders/ArrayLoaderTests.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)     2429 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/dotnet/Test/src/loaders/EnumLoaderTests.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)      749 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/dotnet/Test/src/loaders/ExpressionLoaderTests.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)     1742 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/dotnet/Test/src/loaders/IdMapLoaderTests.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)      766 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/dotnet/Test/src/loaders/NullLoaderTests.cs
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:09:16.020068 schema-salad-8.5.20240410123758/schema_salad/dotnet/Test/src/loaders/PrimtiveLoader/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1435 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/dotnet/Test/src/loaders/PrimtiveLoader/PrimitiveLoaderDoubleTests.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)     1431 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/dotnet/Test/src/loaders/PrimtiveLoader/PrimitiveLoaderFloatTests.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)     1393 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/dotnet/Test/src/loaders/PrimtiveLoader/PrimitiveLoaderIntTests.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)     1246 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/dotnet/Test/src/loaders/PrimtiveLoader/PrimitiveLoaderStringTests.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)     1087 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/dotnet/Test/src/loaders/UnionLoaderTests.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)     1188 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/dotnet/Test.csproj.template
+-rw-r--r--   0 michael   (1000) michael   (1000)     1459 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/dotnet/docfx.json
+-rw-r--r--   0 michael   (1000) michael   (1000)    11383 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/dotnet/editorconfig
+-rw-r--r--   0 michael   (1000) michael   (1000)     6894 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/dotnet/gitignore
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:09:16.020068 schema-salad-8.5.20240410123758/schema_salad/dotnet/util/
+-rw-r--r--   0 michael   (1000) michael   (1000)     2262 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/dotnet/util/Fetcher.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)      167 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/dotnet/util/LoaderInstances.cs
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:09:16.024067 schema-salad-8.5.20240410123758/schema_salad/dotnet/util/Loaders/
+-rw-r--r--   0 michael   (1000) michael   (1000)      338 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/dotnet/util/Loaders/AnyLoader.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)     1847 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/dotnet/util/Loaders/ArrayLoader.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)      905 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/dotnet/util/Loaders/EnumLoader.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)      646 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/dotnet/util/Loaders/ExpressionLoader.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)     2168 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/dotnet/util/Loaders/IdMapLoader.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)     4481 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/dotnet/util/Loaders/Loader.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)     2146 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/dotnet/util/Loaders/MapLoader.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)      362 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/dotnet/util/Loaders/NullLoader.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)      745 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/dotnet/util/Loaders/PrimitiveLoader.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)     1261 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/dotnet/util/Loaders/RecordLoader.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)     1674 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/dotnet/util/Loaders/RootLoader.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)     3984 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/dotnet/util/Loaders/SecondaryDSLLoader.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)     3056 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/dotnet/util/Loaders/TypeDSLLoader.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)      908 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/dotnet/util/Loaders/UnionLoader.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)     1995 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/dotnet/util/Loaders/UriLoader.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)     5665 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/dotnet/util/LoadingOptions.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)     4595 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/dotnet/util/Saveable.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)     1490 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/dotnet/util/ScalarNodeTypeResolver.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)      501 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/dotnet/util/UriExtensions.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)     1624 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/dotnet/util/Utilities.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)     1913 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/dotnet/util/ValidationException.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)      264 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/dotnet/util/Vocabs.cs
+-rw-r--r--   0 michael   (1000) michael   (1000)    35889 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/dotnet_codegen.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     4176 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/exceptions.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     8412 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/fetcher.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:09:16.024067 schema-salad-8.5.20240410123758/schema_salad/java/
+-rw-r--r--   0 michael   (1000) michael   (1000)       61 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/java/MANIFEST.MF
+-rw-r--r--   0 michael   (1000) michael   (1000)      993 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/java/README.md
+-rw-r--r--   0 michael   (1000) michael   (1000)        8 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/java/gitignore
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:09:16.028068 schema-salad-8.5.20240410123758/schema_salad/java/main_utils/
+-rw-r--r--   0 michael   (1000) michael   (1000)      335 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/java/main_utils/AnyLoader.java
+-rw-r--r--   0 michael   (1000) michael   (1000)     1334 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/java/main_utils/ArrayLoader.java
+-rw-r--r--   0 michael   (1000) michael   (1000)      296 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/java/main_utils/ConstantMaps.java
+-rw-r--r--   0 michael   (1000) michael   (1000)     1521 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/java/main_utils/DefaultFetcher.java
+-rw-r--r--   0 michael   (1000) michael   (1000)      984 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/java/main_utils/EnumLoader.java
+-rw-r--r--   0 michael   (1000) michael   (1000)      416 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/java/main_utils/ExpressionLoader.java
+-rw-r--r--   0 michael   (1000) michael   (1000)      186 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/java/main_utils/Fetcher.java
+-rw-r--r--   0 michael   (1000) michael   (1000)     1697 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/java/main_utils/IdMapLoader.java
+-rw-r--r--   0 michael   (1000) michael   (1000)     4613 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/java/main_utils/Loader.java
+-rw-r--r--   0 michael   (1000) michael   (1000)      125 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/java/main_utils/LoaderInstances.java
+-rw-r--r--   0 michael   (1000) michael   (1000)     3989 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/java/main_utils/LoadingOptions.java
+-rw-r--r--   0 michael   (1000) michael   (1000)     2641 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/java/main_utils/LoadingOptionsBuilder.java
+-rw-r--r--   0 michael   (1000) michael   (1000)     1747 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/java/main_utils/MapLoader.java
+-rw-r--r--   0 michael   (1000) michael   (1000)      332 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/java/main_utils/NullLoader.java
+-rw-r--r--   0 michael   (1000) michael   (1000)     1113 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/java/main_utils/OneOrListOf.java
+-rw-r--r--   0 michael   (1000) michael   (1000)     1050 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/java/main_utils/OneOrListOfLoader.java
+-rw-r--r--   0 michael   (1000) michael   (1000)      543 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/java/main_utils/OptionalLoader.java
+-rw-r--r--   0 michael   (1000) michael   (1000)      384 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/java/main_utils/PrimitiveLoader.java
+-rw-r--r--   0 michael   (1000) michael   (1000)     1842 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/java/main_utils/RecordLoader.java
+-rw-r--r--   0 michael   (1000) michael   (1000)     3734 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/java/main_utils/RootLoader.java
+-rw-r--r--   0 michael   (1000) michael   (1000)      180 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/java/main_utils/Saveable.java
+-rw-r--r--   0 michael   (1000) michael   (1000)      177 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/java/main_utils/SaveableImpl.java
+-rw-r--r--   0 michael   (1000) michael   (1000)     3035 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/java/main_utils/SecondaryFilesDslLoader.java
+-rw-r--r--   0 michael   (1000) michael   (1000)     2555 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/java/main_utils/TypeDslLoader.java
+-rw-r--r--   0 michael   (1000) michael   (1000)     1053 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/java/main_utils/UnionLoader.java
+-rw-r--r--   0 michael   (1000) michael   (1000)     1856 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/java/main_utils/UriLoader.java
+-rw-r--r--   0 michael   (1000) michael   (1000)     3293 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/java/main_utils/Uris.java
+-rw-r--r--   0 michael   (1000) michael   (1000)     2254 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/java/main_utils/ValidationException.java
+-rw-r--r--   0 michael   (1000) michael   (1000)      789 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/java/main_utils/Validator.java
+-rw-r--r--   0 michael   (1000) michael   (1000)     1025 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/java/main_utils/YamlUtils.java
+-rw-r--r--   0 michael   (1000) michael   (1000)      131 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/java/main_utils/package.html
+-rw-r--r--   0 michael   (1000) michael   (1000)      237 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/java/overview.html
+-rw-r--r--   0 michael   (1000) michael   (1000)      187 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/java/package.html
+-rw-r--r--   0 michael   (1000) michael   (1000)     5467 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/java/pom.xml
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:09:16.028068 schema-salad-8.5.20240410123758/schema_salad/java/test_utils/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1347 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/java/test_utils/DefaultFetcherTest.java
+-rw-r--r--   0 michael   (1000) michael   (1000)       74 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/java/test_utils/ExamplesTest.java
+-rw-r--r--   0 michael   (1000) michael   (1000)     1134 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/java/test_utils/ShortnameTest.java
+-rw-r--r--   0 michael   (1000) michael   (1000)      402 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/java/test_utils/YamlUtilsTest.java
+-rw-r--r--   0 michael   (1000) michael   (1000)    37505 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/java_codegen.py
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     8438 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/jsonld_context.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    14890 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/main.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    27263 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/makedoc.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:09:16.032068 schema-salad-8.5.20240410123758/schema_salad/metaschema/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1327 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/metaschema/field_name.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      171 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/metaschema/field_name_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      283 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/metaschema/field_name_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      171 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/metaschema/field_name_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     2442 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/metaschema/ident_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      493 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/metaschema/ident_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      473 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/metaschema/ident_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      437 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/metaschema/ident_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     3322 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/metaschema/import_include.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     1804 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/metaschema/link_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      411 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/metaschema/link_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      264 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/metaschema/link_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      313 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/metaschema/link_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      932 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/metaschema/map_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      183 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/metaschema/map_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      518 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/metaschema/map_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)       90 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/metaschema/map_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    13389 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/metaschema/metaschema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     5908 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/metaschema/metaschema_base.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    13923 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/metaschema/salad.md
+-rw-r--r--   0 michael   (1000) michael   (1000)      882 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/metaschema/sfdsl_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      367 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/metaschema/sfdsl_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      289 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/metaschema/sfdsl_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      190 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/metaschema/sfdsl_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     1273 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/metaschema/typedsl_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      394 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/metaschema/typedsl_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      299 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/metaschema/typedsl_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      111 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/metaschema/typedsl_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      846 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/metaschema/vocab_res.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      243 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/metaschema/vocab_res_proc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      345 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/metaschema/vocab_res_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      267 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/metaschema/vocab_res_src.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)   278658 2024-04-10 12:59:20.000000 schema-salad-8.5.20240410123758/schema_salad/metaschema.py
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/py.typed
+-rw-r--r--   0 michael   (1000) michael   (1000)    27678 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/python_codegen.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    39328 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/python_codegen_support.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    47501 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/ref_resolver.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    30704 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/schema.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     9000 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/sourceline.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:09:16.040068 schema-salad-8.5.20240410123758/schema_salad/tests/
+-rw-r--r--   0 michael   (1000) michael   (1000)  2615816 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/EDAM.owl
+-rw-r--r--   0 michael   (1000) michael   (1000)      827 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/Process.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      125 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/bad_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)       65 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/bad_schema2.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      140 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/basket.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)     1267 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/basket_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      590 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/class_field_test.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      452 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/conftest.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:09:16.040068 schema-salad-8.5.20240410123758/schema_salad/tests/cpp_tests/
+-rw-r--r--   0 michael   (1000) michael   (1000)    10312 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/cpp_tests/01_single_record.h
+-rw-r--r--   0 michael   (1000) michael   (1000)      140 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/cpp_tests/01_single_record.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    11531 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/cpp_tests/02_two_records.h
+-rw-r--r--   0 michael   (1000) michael   (1000)      210 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/cpp_tests/02_two_records.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    11693 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/cpp_tests/03_simple_inheritance.h
+-rw-r--r--   0 michael   (1000) michael   (1000)      235 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/cpp_tests/03_simple_inheritance.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    11184 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/cpp_tests/04_abstract_inheritance.h
+-rw-r--r--   0 michael   (1000) michael   (1000)      252 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/cpp_tests/04_abstract_inheritance.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    13621 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/cpp_tests/05_specialization.h
+-rw-r--r--   0 michael   (1000) michael   (1000)      440 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/cpp_tests/05_specialization.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)   133826 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/cwl-pre.yml
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:09:16.040068 schema-salad-8.5.20240410123758/schema_salad/tests/docimp/
+-rw-r--r--   0 michael   (1000) michael   (1000)      155 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/docimp/d1.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)        7 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/docimp/d2.md
+-rw-r--r--   0 michael   (1000) michael   (1000)       42 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/docimp/d3.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)       42 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/docimp/d4.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)       18 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/docimp/d5.md
+-rw-r--r--   0 michael   (1000) michael   (1000)      320 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/docimp/dpre.json
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:09:16.040068 schema-salad-8.5.20240410123758/schema_salad/tests/foreign/
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      347 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/foreign/foreign_prop1.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      302 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/foreign/foreign_prop2.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      436 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/foreign/foreign_prop3.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      390 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/foreign/foreign_prop4.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      428 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/foreign/foreign_prop5.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      294 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/foreign/foreign_prop6.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      292 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/foreign/foreign_prop7.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      493 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/formattest2.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)       41 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/frag.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)       13 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/hello.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)       71 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/hellofield.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      946 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/inherited-attributes.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)       17 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/inject-id1.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)        9 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/inject-id2.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)       32 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/inject-id3.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)       25 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/list.json
+-rw-r--r--   0 michael   (1000) michael   (1000)     1241 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/matcher.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      331 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/memory-leak-check.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    66980 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/metaschema-pre.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      208 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/missing_step_name.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)       18 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/mixin.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      154 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/multidoc.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      900 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/pt.yml
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     1466 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/revtool_bad_schema.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      519 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/test_avro_names.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     7519 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/test_cg.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1146 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/test_cli_args.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     9903 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/test_codegen_errors.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     4428 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/test_cpp_codegen.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     2420 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/test_cwl11.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1071 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/test_dlang_codegen.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     3366 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/test_dotnet_codegen.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    15568 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/test_errors.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    20481 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/test_examples.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     2650 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/test_fetch.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1603 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/test_fp.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1868 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/test_java_codegen.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     9242 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/test_makedoc.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1334 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/test_misc.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      818 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/test_pickling.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     6218 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/test_print_oneline.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     4547 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/test_python_codegen.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:09:16.040068 schema-salad-8.5.20240410123758/schema_salad/tests/test_real_cwl/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:09:16.040068 schema-salad-8.5.20240410123758/schema_salad/tests/test_real_cwl/ICGC-TCGA-PanCancer/
+-rw-r--r--   0 michael   (1000) michael   (1000)      227 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/test_real_cwl/ICGC-TCGA-PanCancer/PreprocessedFilesType.yaml
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:09:16.040068 schema-salad-8.5.20240410123758/schema_salad/tests/test_real_cwl/ICGC-TCGA-PanCancer/complete/
+-rw-r--r--   0 michael   (1000) michael   (1000)      227 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/test_real_cwl/ICGC-TCGA-PanCancer/complete/PreprocessedFilesType.yaml
+-rw-r--r--   0 michael   (1000) michael   (1000)      648 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/test_real_cwl/ICGC-TCGA-PanCancer/complete/clean_vcf.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      666 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/test_real_cwl/ICGC-TCGA-PanCancer/complete/extract_snv.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      783 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/test_real_cwl/ICGC-TCGA-PanCancer/complete/normalize.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      902 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/test_real_cwl/ICGC-TCGA-PanCancer/complete/pass-filter.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      912 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/test_real_cwl/ICGC-TCGA-PanCancer/complete/preprocess_util.js
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    12007 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/test_real_cwl/ICGC-TCGA-PanCancer/complete/preprocess_vcf.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     2352 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/test_real_cwl/ICGC-TCGA-PanCancer/complete/vcf_merge.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      148 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/test_real_cwl/ICGC-TCGA-PanCancer/complete/vcf_merge_util.js
+-rw-r--r--   0 michael   (1000) michael   (1000)      912 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/test_real_cwl/ICGC-TCGA-PanCancer/preprocess_util.js
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    12007 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/test_real_cwl/ICGC-TCGA-PanCancer/preprocess_vcf.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)      148 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/test_real_cwl/ICGC-TCGA-PanCancer/vcf_merge_util.js
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:09:16.044068 schema-salad-8.5.20240410123758/schema_salad/tests/test_real_cwl/bio-cwl-tools/
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     4732 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/test_real_cwl/bio-cwl-tools/bamtools_stats.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     4701 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/test_real_cwl/bio-cwl-tools/bamtools_stats_invalid_schema_ref.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     5757 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/test_real_cwl/bio-cwl-tools/picard_CreateSequenceDictionary.cwl
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:09:16.044068 schema-salad-8.5.20240410123758/schema_salad/tests/test_real_cwl/h3agatk/
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     1905 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/test_real_cwl/h3agatk/GATK-Sub-Workflow-h3abionet-snp.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)    10910 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/test_real_cwl/h3agatk/GATK-complete-WES-Workflow-h3abionet.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     1122 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/test_real_cwl/tabs_rna_seq_workflow.cwl
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:09:16.044068 schema-salad-8.5.20240410123758/schema_salad/tests/test_real_cwl/topmed/
+-rwxr-xr-x   0 michael   (1000) michael   (1000)     5976 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/test_real_cwl/topmed/topmed_variant_calling_pipeline.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     2231 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/test_real_cwl.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     9624 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/test_ref_resolver.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:09:16.048068 schema-salad-8.5.20240410123758/schema_salad/tests/test_schema/
+-rw-r--r--   0 michael   (1000) michael   (1000)    19840 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/test_schema/Base.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    36450 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/test_schema/CommandLineTool.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      209 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/test_schema/CommonWorkflowLanguage.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    16131 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/test_schema/Process.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)    22914 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/test_schema/Workflow.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      453 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/test_schema/avro_naming.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      529 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/test_schema/avro_naming_base.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      529 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/test_schema/avro_subtype.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      524 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/test_schema/avro_subtype_bad.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      814 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/test_schema/avro_subtype_nested.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      818 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/test_schema/avro_subtype_nested_bad.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      679 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/test_schema/avro_subtype_recursive.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      865 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/test_schema/avro_subtype_union.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      869 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/test_schema/avro_subtype_union_bad.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)        1 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/test_schema/concepts.md
+-rw-r--r--   0 michael   (1000) michael   (1000)        1 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/test_schema/contrib.md
+-rw-r--r--   0 michael   (1000) michael   (1000)      514 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/test_schema/cwltest-schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)        1 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/test_schema/intro.md
+-rw-r--r--   0 michael   (1000) michael   (1000)        1 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/test_schema/invocation.md
+-rw-r--r--   0 michael   (1000) michael   (1000)     5774 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/test_schema/metaschema_base.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      514 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/test_schema/misc_schema_v1.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)      575 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/test_schema/misc_schema_v2.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)       54 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/test_schema/no_field_schema.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)       70 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/test_schema/one_line_primary_doc.yml
+-rwxr-xr-x   0 michael   (1000) michael   (1000)       58 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/test_schema/test1.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      174 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/test_schema/test10.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      164 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/test_schema/test11.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      299 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/test_schema/test12.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      302 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/test_schema/test13.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      208 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/test_schema/test14.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      247 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/test_schema/test15.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      274 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/test_schema/test16.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      238 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/test_schema/test17.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      241 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/test_schema/test18.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      269 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/test_schema/test19.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)       59 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/test_schema/test2.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      115 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/test_schema/test3.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      110 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/test_schema/test4.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      116 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/test_schema/test5.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      100 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/test_schema/test6.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      171 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/test_schema/test7.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      169 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/test_schema/test8.cwl
+-rwxr-xr-x   0 michael   (1000) michael   (1000)      168 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/test_schema/test9.cwl
+-rw-r--r--   0 michael   (1000) michael   (1000)     1233 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/test_schema.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1536 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/test_schemas_directive.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     5593 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/test_subtypes.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     3412 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/test_typescript_codegen.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     1816 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/tests/util.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:09:16.048068 schema-salad-8.5.20240410123758/schema_salad/typescript/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1617 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/typescript/.gitignore
+-rw-r--r--   0 michael   (1000) michael   (1000)    11357 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/typescript/LICENSE
+-rw-r--r--   0 michael   (1000) michael   (1000)      138 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/typescript/index.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)     1082 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/typescript/package.json
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:09:16.048068 schema-salad-8.5.20240410123758/schema_salad/typescript/test/
+-rw-r--r--   0 michael   (1000) michael   (1000)      879 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/typescript/test/AnyLoader.spec.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)      147 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/typescript/test/ExampleTest.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)     3118 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/typescript/test/Fetcher.spec.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)     1390 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/typescript/test/IdMap.spec.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)      949 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/typescript/test/LoadingOptions.spec.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)     3265 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/typescript/test/Typeguards.spec.ts
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:09:16.048068 schema-salad-8.5.20240410123758/schema_salad/typescript/test/data/
+-rw-r--r--   0 michael   (1000) michael   (1000)       70 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/typescript/test/data/hellofield.yml
+-rw-r--r--   0 michael   (1000) michael   (1000)        5 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/typescript/test/data/test.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)     1418 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/typescript/test/utilities.spec.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)      541 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/typescript/tsconfig.json
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:09:16.048068 schema-salad-8.5.20240410123758/schema_salad/typescript/util/
+-rw-r--r--   0 michael   (1000) michael   (1000)       60 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/typescript/util/Dict.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)     2336 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/typescript/util/Fetcher.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)      896 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/typescript/util/Internal.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)      296 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/typescript/util/LoaderInstances.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)     1910 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/typescript/util/LoadingOptions.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)     3536 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/typescript/util/Saveable.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)      593 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/typescript/util/Typeguards.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)     1406 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/typescript/util/ValidationException.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)       74 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/typescript/util/Vocabs.ts
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:09:16.052068 schema-salad-8.5.20240410123758/schema_salad/typescript/util/loaders/
+-rw-r--r--   0 michael   (1000) michael   (1000)      345 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/typescript/util/loaders/AnyLoader.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)     1085 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/typescript/util/loaders/ArrayLoader.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)      481 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/typescript/util/loaders/EnumLoader.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)      350 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/typescript/util/loaders/ExpressionLoader.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)     1180 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/typescript/util/loaders/IdMapLoader.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)     3228 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/typescript/util/loaders/Loader.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)     1307 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/typescript/util/loaders/MapLoader.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)      497 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/typescript/util/loaders/PrimitiveLoader.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)     1086 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/typescript/util/loaders/RecordLoader.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)     2508 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/typescript/util/loaders/RootLoader.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)     2421 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/typescript/util/loaders/SecondaryDSLLoader.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)     1776 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/typescript/util/loaders/TypeDSLLoader.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)      865 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/typescript/util/loaders/UnionLoader.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)     1276 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/typescript/util/loaders/UriLoader.ts
+-rw-r--r--   0 michael   (1000) michael   (1000)    31625 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/typescript_codegen.py
+-rw-r--r--   0 michael   (1000) michael   (1000)     4186 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/utils.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    15955 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad/validate.py
+-rw-r--r--   0 michael   (1000) michael   (1000)      841 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/schema_salad.Dockerfile
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2024-04-10 13:09:16.052068 schema-salad-8.5.20240410123758/schema_salad.egg-info/
+-rw-r--r--   0 michael   (1000) michael   (1000)    17485 2024-04-10 13:09:15.000000 schema-salad-8.5.20240410123758/schema_salad.egg-info/PKG-INFO
+-rw-r--r--   0 michael   (1000) michael   (1000)    18381 2024-04-10 13:09:15.000000 schema-salad-8.5.20240410123758/schema_salad.egg-info/SOURCES.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)        1 2024-04-10 13:09:15.000000 schema-salad-8.5.20240410123758/schema_salad.egg-info/dependency_links.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)      106 2024-04-10 13:09:15.000000 schema-salad-8.5.20240410123758/schema_salad.egg-info/entry_points.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)      317 2024-04-10 13:09:15.000000 schema-salad-8.5.20240410123758/schema_salad.egg-info/requires.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)       13 2024-04-10 13:09:15.000000 schema-salad-8.5.20240410123758/schema_salad.egg-info/top_level.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)        1 2024-04-10 12:59:10.000000 schema-salad-8.5.20240410123758/schema_salad.egg-info/zip-safe
+-rw-r--r--   0 michael   (1000) michael   (1000)       95 2024-04-10 13:09:16.052068 schema-salad-8.5.20240410123758/setup.cfg
+-rw-r--r--   0 michael   (1000) michael   (1000)     5533 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/setup.py
+-rw-r--r--   0 michael   (1000) michael   (1000)       75 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/test-requirements.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)     2493 2024-04-10 12:58:44.000000 schema-salad-8.5.20240410123758/tox.ini
```

### Comparing `schema-salad-8.5.20240311110950/.circleci/config.yml` & `schema-salad-8.5.20240410123758/.circleci/config.yml`

 * *Files 24% similar despite different names*

```diff
@@ -36,37 +36,29 @@
                 git checkout << pipeline.parameters.REF >> || true
                 git pull origin << pipeline.parameters.REF >> || true
       - run:
           name: install cibuildwheel and other build reqs
           command: |
             python3 -m pip install --upgrade pip setuptools setuptools_scm[toml]
             python3 -m pip install -rcibw-requirements.txt
-            python3 ./setup.py --version
 
       - run:
           name: pip freeze
           command: |
             python3 -m pip freeze
 
       - run:
           name: list wheels
           command: |
             python3 -m cibuildwheel . --print-build-identifiers
 
       - run:
           name: cibuildwheel
           command: |
-            source .github/workflows/wheel-prep.sh
-            export CIBW_ENVIRONMENT="SCHEMA_SALAD_USE_MYPYC=1 MYPYPATH=/project/mypy-stubs SETUPTOOLS_SCM_PRETEND_VERSION=${SETUPTOOLS_SCM_PRETEND_VERSION}"
             python3 -m cibuildwheel .
-            # "/project" is the project path inside the cibuildwheel container itself
-
-      - run:
-          name: move tests results out of the wheelhouse
-          command: mv wheelhouse/test-results ./
 
       - store_test_results:
           path: test-results/
 
       - store_artifacts:
           path: wheelhouse/
```

### Comparing `schema-salad-8.5.20240311110950/.github/dependabot.yml` & `schema-salad-8.5.20240410123758/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/.github/workflows/ci-tests.yml` & `schema-salad-8.5.20240410123758/.github/workflows/ci-tests.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/.github/workflows/codeql-analysis.yml` & `schema-salad-8.5.20240410123758/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/.github/workflows/quay-publish.yml` & `schema-salad-8.5.20240410123758/.github/workflows/quay-publish.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/.github/workflows/wheels.yml` & `schema-salad-8.5.20240410123758/.github/workflows/wheels.yml`

 * *Files 8% similar despite different names*

```diff
@@ -31,36 +31,23 @@
           fetch-depth: 0  # slow, but gets all the tags
       - uses: actions/checkout@v4
         if: ${{ github.event_name == 'repository_dispatch' }}
         with:
           fetch-depth: 0  # slow, but gets all the tags
           ref: ${{ github.event.client_payload.ref }}
 
-      # Used to host cibuildwheel
-      - uses: actions/setup-python@v5
-
       # - name: Set up QEMU
       #   if: runner.os == 'Linux'
       #   uses: docker/setup-qemu-action@v2
       #   with:
       #     platforms: all
 
-      - name: Install cibuildwheel
-        run: python -m pip install -rcibw-requirements.txt
-
-      - name: set version
-        run: pip install setuptools_scm[toml] wheel && python setup.py --version
-
       - name: Build wheels
-        run: |
-          source .github/workflows/wheel-prep.sh
-          export CIBW_ENVIRONMENT="SCHEMA_SALAD_USE_MYPYC=1 MYPYPATH=/project/mypy-stubs SETUPTOOLS_SCM_PRETEND_VERSION=${SETUPTOOLS_SCM_PRETEND_VERSION}"
-          python -m cibuildwheel --output-dir wheelhouse
+        uses: pypa/cibuildwheel@v2.17.0
         env:
-          CIBW_ARCHS_MACOS: x86_64 arm64
           CIBW_BUILD: ${{ matrix.build }}
           CIBW_MANYLINUX_X86_64_IMAGE: quay.io/pypa/${{ matrix.image }}
           CIBW_MUSLLINUX_X86_64_IMAGE: quay.io/pypa/${{ matrix.image }}
           # configure cibuildwheel to build native 64-bit archs ('auto64'), and some
           # emulated ones
           # Linux arm64 wheels are built on circleci
           CIBW_ARCHS_LINUX: auto64 # ppc64le s390x
@@ -80,39 +67,62 @@
           fetch-depth: 0  # slow, but gets all the tags
       - uses: actions/checkout@v4
         if: ${{ github.event_name == 'repository_dispatch' }}
         with:
           fetch-depth: 0  # slow, but gets all the tags
           ref: ${{ github.event.client_payload.ref }}
 
-      - name: set version
-        run: pip install setuptools_scm[toml] wheel && python setup.py --version
-
       - name: Build sdist
         run: pipx run build --sdist
 
       - uses: actions/upload-artifact@v4
         with:
           name: artifact-source
           path: dist/*.tar.gz
 
+  build_wheels_macos:
+    name: Build wheels on ${{ matrix.os }}
+    runs-on: ${{ matrix.os }}
+    strategy:
+      matrix:
+        # macos-13 is an intel runner, macos-14 is apple silicon
+        os: [macos-13, macos-14]
+    steps:
+      - uses: actions/checkout@v4
+        if: ${{ github.event_name != 'repository_dispatch' }}
+        with:
+          fetch-depth: 0  # slow, but gets all the tags
+      - uses: actions/checkout@v4
+        if: ${{ github.event_name == 'repository_dispatch' }}
+        with:
+          fetch-depth: 0  # slow, but gets all the tags
+          ref: ${{ github.event.client_payload.ref }}
+
+      - name: Build wheels
+        uses: pypa/cibuildwheel@v2.17.0
+
+      - uses: actions/upload-artifact@v4
+        with:
+          name: artifact-${{ matrix.os }}-${{ strategy.job-index }}
+          path: ./wheelhouse/*.whl
+
   upload_pypi:
     needs: [build_wheels, build_sdist]
     runs-on: ubuntu-latest
     environment: pypi
     permissions:
       id-token: write
-    if: github.event_name == 'release' && github.event.action == 'published'
+    if: (github.event_name == 'release' && github.event.action == 'published') || (github.event_name == 'repository_dispatch' && github.event.client_payload.publish_wheel == true)
     steps:
       - uses: actions/download-artifact@v4
         with:
           # unpacks default artifact into dist/
-          # if `name: artifact` is omitted, the action will create extra parent dir
           pattern: artifact-*
+          merge-multiple: true
           path: dist
 
       - uses: pypa/gh-action-pypi-publish@release/v1
         with:
           # To test: repository-url: https://test.pypi.org/legacy/
           user: __token__
           password: ${{ secrets.PYPI_API_TOKEN }}
-          skip_existing: true
+          skip-existing: true
```

### Comparing `schema-salad-8.5.20240311110950/.mergify.yml` & `schema-salad-8.5.20240410123758/.mergify.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/.pylintrc` & `schema-salad-8.5.20240410123758/.pylintrc`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/.readthedocs.yml` & `schema-salad-8.5.20240410123758/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/CONTRIBUTING.md` & `schema-salad-8.5.20240410123758/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/LICENSE.txt` & `schema-salad-8.5.20240410123758/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/MANIFEST.in` & `schema-salad-8.5.20240410123758/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/Makefile` & `schema-salad-8.5.20240410123758/Makefile`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/PKG-INFO` & `schema-salad-8.5.20240410123758/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schema-salad
-Version: 8.5.20240311110950
+Version: 8.5.20240410123758
 Summary: Schema Annotations for Linked Avro Data (SALAD)
 Home-page: https://schema-salad.readthedocs.io/
 Download-URL: https://github.com/common-workflow-language/schema_salad/releases
 Author: Common workflow language working group
 Author-email: common-workflow-language@googlegroups.com
 License: Apache 2.0
 Classifier: Environment :: Console
```

### Comparing `schema-salad-8.5.20240311110950/README.rst` & `schema-salad-8.5.20240410123758/README.rst`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/build-schema_salad-docker.sh` & `schema-salad-8.5.20240410123758/build-schema_salad-docker.sh`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/docs/Makefile` & `schema-salad-8.5.20240410123758/docs/Makefile`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/docs/_static/favicon.ico` & `schema-salad-8.5.20240410123758/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/docs/conf.py` & `schema-salad-8.5.20240410123758/docs/conf.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/docs/make.bat` & `schema-salad-8.5.20240410123758/docs/make.bat`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/docs/typeshed.rst` & `schema-salad-8.5.20240410123758/docs/typeshed.rst`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/manual_wheel_publish.sh` & `schema-salad-8.5.20240410123758/manual_wheel_publish.sh`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/mypy-stubs/cachecontrol/caches/file_cache.pyi` & `schema-salad-8.5.20240410123758/mypy-stubs/cachecontrol/caches/file_cache.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/mypy-stubs/cachecontrol/wrapper.pyi` & `schema-salad-8.5.20240410123758/mypy-stubs/cachecontrol/wrapper.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/mypy-stubs/mistune/__init__.pyi` & `schema-salad-8.5.20240410123758/mypy-stubs/mistune/__init__.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/mypy-stubs/mistune/block_parser.pyi` & `schema-salad-8.5.20240410123758/mypy-stubs/mistune/block_parser.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/mypy-stubs/mistune/core.pyi` & `schema-salad-8.5.20240410123758/mypy-stubs/mistune/core.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/mypy-stubs/mistune/directives/__init__.pyi` & `schema-salad-8.5.20240410123758/mypy-stubs/mistune/directives/__init__.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/mypy-stubs/mistune/directives/_base.pyi` & `schema-salad-8.5.20240410123758/mypy-stubs/mistune/directives/_base.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/mypy-stubs/mistune/directives/_fenced.pyi` & `schema-salad-8.5.20240410123758/mypy-stubs/mistune/directives/_fenced.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/mypy-stubs/mistune/directives/_rst.pyi` & `schema-salad-8.5.20240410123758/mypy-stubs/mistune/directives/_rst.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/mypy-stubs/mistune/directives/admonition.pyi` & `schema-salad-8.5.20240410123758/mypy-stubs/mistune/directives/admonition.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/mypy-stubs/mistune/directives/image.pyi` & `schema-salad-8.5.20240410123758/mypy-stubs/mistune/directives/image.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/mypy-stubs/mistune/directives/include.pyi` & `schema-salad-8.5.20240410123758/mypy-stubs/mistune/directives/include.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/mypy-stubs/mistune/directives/toc.pyi` & `schema-salad-8.5.20240410123758/mypy-stubs/mistune/directives/toc.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/mypy-stubs/mistune/helpers.pyi` & `schema-salad-8.5.20240410123758/mypy-stubs/mistune/helpers.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/mypy-stubs/mistune/inline_parser.pyi` & `schema-salad-8.5.20240410123758/mypy-stubs/mistune/inline_parser.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/mypy-stubs/mistune/markdown.pyi` & `schema-salad-8.5.20240410123758/mypy-stubs/mistune/markdown.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/mypy-stubs/mistune/plugins/ruby.pyi` & `schema-salad-8.5.20240410123758/mypy-stubs/mistune/plugins/ruby.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/mypy-stubs/mistune/renderers/html.pyi` & `schema-salad-8.5.20240410123758/mypy-stubs/mistune/renderers/html.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/mypy-stubs/mistune/renderers/markdown.pyi` & `schema-salad-8.5.20240410123758/mypy-stubs/mistune/renderers/markdown.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/mypy-stubs/mistune/renderers/rst.pyi` & `schema-salad-8.5.20240410123758/mypy-stubs/mistune/renderers/rst.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/mypy-stubs/mistune/toc.pyi` & `schema-salad-8.5.20240410123758/mypy-stubs/mistune/toc.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/mypy-stubs/rdflib/__init__.pyi` & `schema-salad-8.5.20240410123758/mypy-stubs/rdflib/__init__.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/mypy-stubs/rdflib/collection.pyi` & `schema-salad-8.5.20240410123758/mypy-stubs/rdflib/collection.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/mypy-stubs/rdflib/graph.pyi` & `schema-salad-8.5.20240410123758/mypy-stubs/rdflib/graph.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/mypy-stubs/rdflib/namespace/_CSVW.pyi` & `schema-salad-8.5.20240410123758/mypy-stubs/rdflib/namespace/_CSVW.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/mypy-stubs/rdflib/namespace/_DCAT.pyi` & `schema-salad-8.5.20240410123758/mypy-stubs/rdflib/namespace/_DCAT.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/mypy-stubs/rdflib/namespace/_DCTERMS.pyi` & `schema-salad-8.5.20240410123758/mypy-stubs/rdflib/namespace/_DCTERMS.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/mypy-stubs/rdflib/namespace/_DOAP.pyi` & `schema-salad-8.5.20240410123758/mypy-stubs/rdflib/namespace/_DOAP.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/mypy-stubs/rdflib/namespace/_FOAF.pyi` & `schema-salad-8.5.20240410123758/mypy-stubs/rdflib/namespace/_FOAF.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/mypy-stubs/rdflib/namespace/_ODRL2.pyi` & `schema-salad-8.5.20240410123758/mypy-stubs/rdflib/namespace/_ODRL2.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/mypy-stubs/rdflib/namespace/_ORG.pyi` & `schema-salad-8.5.20240410123758/mypy-stubs/rdflib/namespace/_ORG.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/mypy-stubs/rdflib/namespace/_OWL.pyi` & `schema-salad-8.5.20240410123758/mypy-stubs/rdflib/namespace/_OWL.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/mypy-stubs/rdflib/namespace/_PROV.pyi` & `schema-salad-8.5.20240410123758/mypy-stubs/rdflib/namespace/_PROV.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/mypy-stubs/rdflib/namespace/_QB.pyi` & `schema-salad-8.5.20240410123758/mypy-stubs/rdflib/namespace/_QB.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/mypy-stubs/rdflib/namespace/_RDF.pyi` & `schema-salad-8.5.20240410123758/mypy-stubs/rdflib/namespace/_RDF.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/mypy-stubs/rdflib/namespace/_RDFS.pyi` & `schema-salad-8.5.20240410123758/mypy-stubs/rdflib/namespace/_RDFS.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/mypy-stubs/rdflib/namespace/_SDO.pyi` & `schema-salad-8.5.20240410123758/mypy-stubs/rdflib/namespace/_SDO.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/mypy-stubs/rdflib/namespace/_SH.pyi` & `schema-salad-8.5.20240410123758/mypy-stubs/rdflib/namespace/_SH.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/mypy-stubs/rdflib/namespace/_SKOS.pyi` & `schema-salad-8.5.20240410123758/mypy-stubs/rdflib/namespace/_SKOS.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/mypy-stubs/rdflib/namespace/_SOSA.pyi` & `schema-salad-8.5.20240410123758/mypy-stubs/rdflib/namespace/_SOSA.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/mypy-stubs/rdflib/namespace/_SSN.pyi` & `schema-salad-8.5.20240410123758/mypy-stubs/rdflib/namespace/_SSN.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/mypy-stubs/rdflib/namespace/_TIME.pyi` & `schema-salad-8.5.20240410123758/mypy-stubs/rdflib/namespace/_TIME.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/mypy-stubs/rdflib/namespace/_VOID.pyi` & `schema-salad-8.5.20240410123758/mypy-stubs/rdflib/namespace/_VOID.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/mypy-stubs/rdflib/namespace/_XSD.pyi` & `schema-salad-8.5.20240410123758/mypy-stubs/rdflib/namespace/_XSD.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/mypy-stubs/rdflib/namespace/__init__.pyi` & `schema-salad-8.5.20240410123758/mypy-stubs/rdflib/namespace/__init__.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/mypy-stubs/rdflib/paths.pyi` & `schema-salad-8.5.20240410123758/mypy-stubs/rdflib/paths.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/mypy-stubs/rdflib/plugin.pyi` & `schema-salad-8.5.20240410123758/mypy-stubs/rdflib/plugin.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/mypy-stubs/rdflib/query.pyi` & `schema-salad-8.5.20240410123758/mypy-stubs/rdflib/query.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/mypy-stubs/rdflib/resource.pyi` & `schema-salad-8.5.20240410123758/mypy-stubs/rdflib/resource.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/mypy-stubs/rdflib/term.pyi` & `schema-salad-8.5.20240410123758/mypy-stubs/rdflib/term.pyi`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/pyproject.toml` & `schema-salad-8.5.20240410123758/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -12,18 +12,18 @@
 ]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools_scm]
 write_to = "schema_salad/_version.py"
 
 [tool.cibuildwheel]
-before-build = "python -m pip install -r requirements.txt -r mypy-requirements.txt"
-test-command = "python -m pytest -n 2 --junitxml=/output/test-results/junit_$(python -V | awk '{print $2}')_${AUDITWHEEL_PLAT}.xml --pyargs schema_salad"
+test-command = "python -m pytest -n 2 --junitxml={project}/test-results/junit_$(python -V | awk '{print $2}')_${AUDITWHEEL_PLAT}.xml --pyargs schema_salad"
 test-requires = "-r test-requirements.txt"
 test-extras = "pycodegen"
 skip = "pp*"
 #      ^ skip building wheels on PyPy (any version)
 build-verbosity = "1"
+environment = { SCHEMA_SALAD_USE_MYPYC="1", MYPYPATH="$(pwd)/mypy-stubs" }
 
 [tool.black]
 line-length = 100
 target-version = [ "py38" ]
```

### Comparing `schema-salad-8.5.20240311110950/release-test.sh` & `schema-salad-8.5.20240410123758/release-test.sh`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/avro/LICENSE` & `schema-salad-8.5.20240410123758/schema_salad/avro/LICENSE`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/avro/__init__.py` & `schema-salad-8.5.20240410123758/schema_salad/avro/__init__.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/avro/schema.py` & `schema-salad-8.5.20240410123758/schema_salad/avro/schema.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/codegen.py` & `schema-salad-8.5.20240410123758/schema_salad/codegen.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/codegen_base.py` & `schema-salad-8.5.20240410123758/schema_salad/codegen_base.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/cpp_codegen.py` & `schema-salad-8.5.20240410123758/schema_salad/cpp_codegen.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/dlang_codegen.py` & `schema-salad-8.5.20240410123758/schema_salad/dlang_codegen.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/dotnet/LICENSE` & `schema-salad-8.5.20240410123758/schema_salad/dotnet/LICENSE`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/dotnet/Project.csproj.template` & `schema-salad-8.5.20240410123758/schema_salad/dotnet/Project.csproj.template`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/dotnet/Solution.sln` & `schema-salad-8.5.20240410123758/schema_salad/dotnet/Solution.sln`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/dotnet/Test/src/FetcherTests.cs` & `schema-salad-8.5.20240410123758/schema_salad/dotnet/Test/src/FetcherTests.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/dotnet/Test/src/UtilitiesTests.cs` & `schema-salad-8.5.20240410123758/schema_salad/dotnet/Test/src/UtilitiesTests.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/dotnet/Test/src/loaders/AnyLoaderTests.cs` & `schema-salad-8.5.20240410123758/schema_salad/dotnet/Test/src/loaders/AnyLoaderTests.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/dotnet/Test/src/loaders/ArrayLoaderTests.cs` & `schema-salad-8.5.20240410123758/schema_salad/dotnet/Test/src/loaders/ArrayLoaderTests.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/dotnet/Test/src/loaders/EnumLoaderTests.cs` & `schema-salad-8.5.20240410123758/schema_salad/dotnet/Test/src/loaders/EnumLoaderTests.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/dotnet/Test/src/loaders/ExpressionLoaderTests.cs` & `schema-salad-8.5.20240410123758/schema_salad/dotnet/Test/src/loaders/ExpressionLoaderTests.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/dotnet/Test/src/loaders/IdMapLoaderTests.cs` & `schema-salad-8.5.20240410123758/schema_salad/dotnet/Test/src/loaders/IdMapLoaderTests.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/dotnet/Test/src/loaders/NullLoaderTests.cs` & `schema-salad-8.5.20240410123758/schema_salad/dotnet/Test/src/loaders/NullLoaderTests.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/dotnet/Test/src/loaders/PrimtiveLoader/PrimitiveLoaderDoubleTests.cs` & `schema-salad-8.5.20240410123758/schema_salad/dotnet/Test/src/loaders/PrimtiveLoader/PrimitiveLoaderDoubleTests.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/dotnet/Test/src/loaders/PrimtiveLoader/PrimitiveLoaderFloatTests.cs` & `schema-salad-8.5.20240410123758/schema_salad/dotnet/Test/src/loaders/PrimtiveLoader/PrimitiveLoaderFloatTests.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/dotnet/Test/src/loaders/PrimtiveLoader/PrimitiveLoaderIntTests.cs` & `schema-salad-8.5.20240410123758/schema_salad/dotnet/Test/src/loaders/PrimtiveLoader/PrimitiveLoaderIntTests.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/dotnet/Test/src/loaders/PrimtiveLoader/PrimitiveLoaderStringTests.cs` & `schema-salad-8.5.20240410123758/schema_salad/dotnet/Test/src/loaders/PrimtiveLoader/PrimitiveLoaderStringTests.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/dotnet/Test/src/loaders/UnionLoaderTests.cs` & `schema-salad-8.5.20240410123758/schema_salad/dotnet/Test/src/loaders/UnionLoaderTests.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/dotnet/Test.csproj.template` & `schema-salad-8.5.20240410123758/schema_salad/dotnet/Test.csproj.template`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/dotnet/docfx.json` & `schema-salad-8.5.20240410123758/schema_salad/dotnet/docfx.json`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/dotnet/editorconfig` & `schema-salad-8.5.20240410123758/schema_salad/dotnet/editorconfig`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/dotnet/gitignore` & `schema-salad-8.5.20240410123758/schema_salad/dotnet/gitignore`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/dotnet/util/Fetcher.cs` & `schema-salad-8.5.20240410123758/schema_salad/dotnet/util/Fetcher.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/dotnet/util/Loaders/ArrayLoader.cs` & `schema-salad-8.5.20240410123758/schema_salad/dotnet/util/Loaders/ArrayLoader.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/dotnet/util/Loaders/EnumLoader.cs` & `schema-salad-8.5.20240410123758/schema_salad/dotnet/util/Loaders/EnumLoader.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/dotnet/util/Loaders/ExpressionLoader.cs` & `schema-salad-8.5.20240410123758/schema_salad/dotnet/util/Loaders/ExpressionLoader.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/dotnet/util/Loaders/IdMapLoader.cs` & `schema-salad-8.5.20240410123758/schema_salad/dotnet/util/Loaders/IdMapLoader.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/dotnet/util/Loaders/Loader.cs` & `schema-salad-8.5.20240410123758/schema_salad/dotnet/util/Loaders/Loader.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/dotnet/util/Loaders/MapLoader.cs` & `schema-salad-8.5.20240410123758/schema_salad/dotnet/util/Loaders/MapLoader.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/dotnet/util/Loaders/PrimitiveLoader.cs` & `schema-salad-8.5.20240410123758/schema_salad/dotnet/util/Loaders/PrimitiveLoader.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/dotnet/util/Loaders/RecordLoader.cs` & `schema-salad-8.5.20240410123758/schema_salad/dotnet/util/Loaders/RecordLoader.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/dotnet/util/Loaders/RootLoader.cs` & `schema-salad-8.5.20240410123758/schema_salad/dotnet/util/Loaders/RootLoader.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/dotnet/util/Loaders/SecondaryDSLLoader.cs` & `schema-salad-8.5.20240410123758/schema_salad/dotnet/util/Loaders/SecondaryDSLLoader.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/dotnet/util/Loaders/TypeDSLLoader.cs` & `schema-salad-8.5.20240410123758/schema_salad/dotnet/util/Loaders/TypeDSLLoader.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/dotnet/util/Loaders/UnionLoader.cs` & `schema-salad-8.5.20240410123758/schema_salad/dotnet/util/Loaders/UnionLoader.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/dotnet/util/Loaders/UriLoader.cs` & `schema-salad-8.5.20240410123758/schema_salad/dotnet/util/Loaders/UriLoader.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/dotnet/util/LoadingOptions.cs` & `schema-salad-8.5.20240410123758/schema_salad/dotnet/util/LoadingOptions.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/dotnet/util/Saveable.cs` & `schema-salad-8.5.20240410123758/schema_salad/dotnet/util/Saveable.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/dotnet/util/ScalarNodeTypeResolver.cs` & `schema-salad-8.5.20240410123758/schema_salad/dotnet/util/ScalarNodeTypeResolver.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/dotnet/util/Utilities.cs` & `schema-salad-8.5.20240410123758/schema_salad/dotnet/util/Utilities.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/dotnet/util/ValidationException.cs` & `schema-salad-8.5.20240410123758/schema_salad/dotnet/util/ValidationException.cs`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/dotnet_codegen.py` & `schema-salad-8.5.20240410123758/schema_salad/dotnet_codegen.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/exceptions.py` & `schema-salad-8.5.20240410123758/schema_salad/exceptions.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/fetcher.py` & `schema-salad-8.5.20240410123758/schema_salad/fetcher.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/java/README.md` & `schema-salad-8.5.20240410123758/schema_salad/java/README.md`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/java/main_utils/ArrayLoader.java` & `schema-salad-8.5.20240410123758/schema_salad/java/main_utils/ArrayLoader.java`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/java/main_utils/DefaultFetcher.java` & `schema-salad-8.5.20240410123758/schema_salad/java/main_utils/DefaultFetcher.java`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/java/main_utils/EnumLoader.java` & `schema-salad-8.5.20240410123758/schema_salad/java/main_utils/EnumLoader.java`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/java/main_utils/IdMapLoader.java` & `schema-salad-8.5.20240410123758/schema_salad/java/main_utils/IdMapLoader.java`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/java/main_utils/Loader.java` & `schema-salad-8.5.20240410123758/schema_salad/java/main_utils/Loader.java`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/java/main_utils/LoadingOptions.java` & `schema-salad-8.5.20240410123758/schema_salad/java/main_utils/LoadingOptions.java`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/java/main_utils/LoadingOptionsBuilder.java` & `schema-salad-8.5.20240410123758/schema_salad/java/main_utils/LoadingOptionsBuilder.java`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/java/main_utils/MapLoader.java` & `schema-salad-8.5.20240410123758/schema_salad/java/main_utils/MapLoader.java`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/java/main_utils/OneOrListOf.java` & `schema-salad-8.5.20240410123758/schema_salad/java/main_utils/OneOrListOf.java`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/java/main_utils/OneOrListOfLoader.java` & `schema-salad-8.5.20240410123758/schema_salad/java/main_utils/OneOrListOfLoader.java`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/java/main_utils/OptionalLoader.java` & `schema-salad-8.5.20240410123758/schema_salad/java/main_utils/OptionalLoader.java`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/java/main_utils/RecordLoader.java` & `schema-salad-8.5.20240410123758/schema_salad/java/main_utils/RecordLoader.java`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/java/main_utils/RootLoader.java` & `schema-salad-8.5.20240410123758/schema_salad/java/main_utils/RootLoader.java`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/java/main_utils/SecondaryFilesDslLoader.java` & `schema-salad-8.5.20240410123758/schema_salad/java/main_utils/SecondaryFilesDslLoader.java`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/java/main_utils/TypeDslLoader.java` & `schema-salad-8.5.20240410123758/schema_salad/java/main_utils/TypeDslLoader.java`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/java/main_utils/UnionLoader.java` & `schema-salad-8.5.20240410123758/schema_salad/java/main_utils/UnionLoader.java`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/java/main_utils/UriLoader.java` & `schema-salad-8.5.20240410123758/schema_salad/java/main_utils/UriLoader.java`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/java/main_utils/Uris.java` & `schema-salad-8.5.20240410123758/schema_salad/java/main_utils/Uris.java`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/java/main_utils/ValidationException.java` & `schema-salad-8.5.20240410123758/schema_salad/java/main_utils/ValidationException.java`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/java/main_utils/Validator.java` & `schema-salad-8.5.20240410123758/schema_salad/java/main_utils/Validator.java`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/java/main_utils/YamlUtils.java` & `schema-salad-8.5.20240410123758/schema_salad/java/main_utils/YamlUtils.java`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/java/pom.xml` & `schema-salad-8.5.20240410123758/schema_salad/java/pom.xml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/java/test_utils/DefaultFetcherTest.java` & `schema-salad-8.5.20240410123758/schema_salad/java/test_utils/DefaultFetcherTest.java`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/java/test_utils/ShortnameTest.java` & `schema-salad-8.5.20240410123758/schema_salad/java/test_utils/ShortnameTest.java`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/java_codegen.py` & `schema-salad-8.5.20240410123758/schema_salad/java_codegen.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/jsonld_context.py` & `schema-salad-8.5.20240410123758/schema_salad/jsonld_context.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/main.py` & `schema-salad-8.5.20240410123758/schema_salad/main.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/makedoc.py` & `schema-salad-8.5.20240410123758/schema_salad/makedoc.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/metaschema/field_name.yml` & `schema-salad-8.5.20240410123758/schema_salad/metaschema/field_name.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/metaschema/ident_res.yml` & `schema-salad-8.5.20240410123758/schema_salad/metaschema/ident_res.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/metaschema/import_include.md` & `schema-salad-8.5.20240410123758/schema_salad/metaschema/import_include.md`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/metaschema/link_res.yml` & `schema-salad-8.5.20240410123758/schema_salad/metaschema/link_res.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/metaschema/map_res.yml` & `schema-salad-8.5.20240410123758/schema_salad/metaschema/map_res.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/metaschema/map_res_schema.yml` & `schema-salad-8.5.20240410123758/schema_salad/metaschema/map_res_schema.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/metaschema/metaschema.yml` & `schema-salad-8.5.20240410123758/schema_salad/metaschema/metaschema.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/metaschema/metaschema_base.yml` & `schema-salad-8.5.20240410123758/schema_salad/metaschema/metaschema_base.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/metaschema/salad.md` & `schema-salad-8.5.20240410123758/schema_salad/metaschema/salad.md`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/metaschema/sfdsl_res.yml` & `schema-salad-8.5.20240410123758/schema_salad/metaschema/sfdsl_res.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/metaschema/typedsl_res.yml` & `schema-salad-8.5.20240410123758/schema_salad/metaschema/typedsl_res.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/metaschema/vocab_res.yml` & `schema-salad-8.5.20240410123758/schema_salad/metaschema/vocab_res.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/metaschema.py` & `schema-salad-8.5.20240410123758/schema_salad/metaschema.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/python_codegen.py` & `schema-salad-8.5.20240410123758/schema_salad/python_codegen.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/python_codegen_support.py` & `schema-salad-8.5.20240410123758/schema_salad/python_codegen_support.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/ref_resolver.py` & `schema-salad-8.5.20240410123758/schema_salad/ref_resolver.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/schema.py` & `schema-salad-8.5.20240410123758/schema_salad/schema.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/sourceline.py` & `schema-salad-8.5.20240410123758/schema_salad/sourceline.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/tests/EDAM.owl` & `schema-salad-8.5.20240410123758/schema_salad/tests/EDAM.owl`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/tests/Process.yml` & `schema-salad-8.5.20240410123758/schema_salad/tests/Process.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/tests/basket_schema.yml` & `schema-salad-8.5.20240410123758/schema_salad/tests/basket_schema.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/tests/class_field_test.yml` & `schema-salad-8.5.20240410123758/schema_salad/tests/class_field_test.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/tests/cpp_tests/01_single_record.h` & `schema-salad-8.5.20240410123758/schema_salad/tests/cpp_tests/01_single_record.h`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/tests/cpp_tests/02_two_records.h` & `schema-salad-8.5.20240410123758/schema_salad/tests/cpp_tests/02_two_records.h`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/tests/cpp_tests/03_simple_inheritance.h` & `schema-salad-8.5.20240410123758/schema_salad/tests/cpp_tests/03_simple_inheritance.h`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/tests/cpp_tests/04_abstract_inheritance.h` & `schema-salad-8.5.20240410123758/schema_salad/tests/cpp_tests/04_abstract_inheritance.h`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/tests/cpp_tests/05_specialization.h` & `schema-salad-8.5.20240410123758/schema_salad/tests/cpp_tests/05_specialization.h`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/tests/cwl-pre.yml` & `schema-salad-8.5.20240410123758/schema_salad/tests/cwl-pre.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/tests/inherited-attributes.yml` & `schema-salad-8.5.20240410123758/schema_salad/tests/inherited-attributes.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/tests/matcher.py` & `schema-salad-8.5.20240410123758/schema_salad/tests/matcher.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/tests/metaschema-pre.yml` & `schema-salad-8.5.20240410123758/schema_salad/tests/metaschema-pre.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/tests/pt.yml` & `schema-salad-8.5.20240410123758/schema_salad/tests/pt.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/tests/revtool_bad_schema.cwl` & `schema-salad-8.5.20240410123758/schema_salad/tests/revtool_bad_schema.cwl`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/tests/test_avro_names.py` & `schema-salad-8.5.20240410123758/schema_salad/tests/test_avro_names.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/tests/test_cg.py` & `schema-salad-8.5.20240410123758/schema_salad/tests/test_cg.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/tests/test_cli_args.py` & `schema-salad-8.5.20240410123758/schema_salad/tests/test_cli_args.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/tests/test_codegen_errors.py` & `schema-salad-8.5.20240410123758/schema_salad/tests/test_codegen_errors.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/tests/test_cpp_codegen.py` & `schema-salad-8.5.20240410123758/schema_salad/tests/test_cpp_codegen.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/tests/test_cwl11.py` & `schema-salad-8.5.20240410123758/schema_salad/tests/test_cwl11.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/tests/test_dlang_codegen.py` & `schema-salad-8.5.20240410123758/schema_salad/tests/test_dlang_codegen.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/tests/test_dotnet_codegen.py` & `schema-salad-8.5.20240410123758/schema_salad/tests/test_dotnet_codegen.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/tests/test_errors.py` & `schema-salad-8.5.20240410123758/schema_salad/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/tests/test_examples.py` & `schema-salad-8.5.20240410123758/schema_salad/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/tests/test_fetch.py` & `schema-salad-8.5.20240410123758/schema_salad/tests/test_fetch.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/tests/test_fp.py` & `schema-salad-8.5.20240410123758/schema_salad/tests/test_fp.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/tests/test_java_codegen.py` & `schema-salad-8.5.20240410123758/schema_salad/tests/test_java_codegen.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/tests/test_makedoc.py` & `schema-salad-8.5.20240410123758/schema_salad/tests/test_makedoc.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/tests/test_misc.py` & `schema-salad-8.5.20240410123758/schema_salad/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/tests/test_pickling.py` & `schema-salad-8.5.20240410123758/schema_salad/tests/test_pickling.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/tests/test_print_oneline.py` & `schema-salad-8.5.20240410123758/schema_salad/tests/test_print_oneline.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/tests/test_python_codegen.py` & `schema-salad-8.5.20240410123758/schema_salad/tests/test_python_codegen.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/tests/test_real_cwl/ICGC-TCGA-PanCancer/complete/clean_vcf.cwl` & `schema-salad-8.5.20240410123758/schema_salad/tests/test_real_cwl/ICGC-TCGA-PanCancer/complete/clean_vcf.cwl`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/tests/test_real_cwl/ICGC-TCGA-PanCancer/complete/extract_snv.cwl` & `schema-salad-8.5.20240410123758/schema_salad/tests/test_real_cwl/ICGC-TCGA-PanCancer/complete/extract_snv.cwl`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/tests/test_real_cwl/ICGC-TCGA-PanCancer/complete/normalize.cwl` & `schema-salad-8.5.20240410123758/schema_salad/tests/test_real_cwl/ICGC-TCGA-PanCancer/complete/normalize.cwl`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/tests/test_real_cwl/ICGC-TCGA-PanCancer/complete/pass-filter.cwl` & `schema-salad-8.5.20240410123758/schema_salad/tests/test_real_cwl/ICGC-TCGA-PanCancer/complete/pass-filter.cwl`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/tests/test_real_cwl/ICGC-TCGA-PanCancer/complete/preprocess_util.js` & `schema-salad-8.5.20240410123758/schema_salad/tests/test_real_cwl/ICGC-TCGA-PanCancer/complete/preprocess_util.js`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/tests/test_real_cwl/ICGC-TCGA-PanCancer/complete/preprocess_vcf.cwl` & `schema-salad-8.5.20240410123758/schema_salad/tests/test_real_cwl/ICGC-TCGA-PanCancer/complete/preprocess_vcf.cwl`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/tests/test_real_cwl/ICGC-TCGA-PanCancer/complete/vcf_merge.cwl` & `schema-salad-8.5.20240410123758/schema_salad/tests/test_real_cwl/ICGC-TCGA-PanCancer/complete/vcf_merge.cwl`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/tests/test_real_cwl/ICGC-TCGA-PanCancer/preprocess_util.js` & `schema-salad-8.5.20240410123758/schema_salad/tests/test_real_cwl/ICGC-TCGA-PanCancer/preprocess_util.js`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/tests/test_real_cwl/ICGC-TCGA-PanCancer/preprocess_vcf.cwl` & `schema-salad-8.5.20240410123758/schema_salad/tests/test_real_cwl/ICGC-TCGA-PanCancer/preprocess_vcf.cwl`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/tests/test_real_cwl/bio-cwl-tools/bamtools_stats.cwl` & `schema-salad-8.5.20240410123758/schema_salad/tests/test_real_cwl/bio-cwl-tools/bamtools_stats.cwl`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/tests/test_real_cwl/bio-cwl-tools/bamtools_stats_invalid_schema_ref.cwl` & `schema-salad-8.5.20240410123758/schema_salad/tests/test_real_cwl/bio-cwl-tools/bamtools_stats_invalid_schema_ref.cwl`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/tests/test_real_cwl/bio-cwl-tools/picard_CreateSequenceDictionary.cwl` & `schema-salad-8.5.20240410123758/schema_salad/tests/test_real_cwl/bio-cwl-tools/picard_CreateSequenceDictionary.cwl`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/tests/test_real_cwl/h3agatk/GATK-Sub-Workflow-h3abionet-snp.cwl` & `schema-salad-8.5.20240410123758/schema_salad/tests/test_real_cwl/h3agatk/GATK-Sub-Workflow-h3abionet-snp.cwl`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/tests/test_real_cwl/h3agatk/GATK-complete-WES-Workflow-h3abionet.cwl` & `schema-salad-8.5.20240410123758/schema_salad/tests/test_real_cwl/h3agatk/GATK-complete-WES-Workflow-h3abionet.cwl`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/tests/test_real_cwl/tabs_rna_seq_workflow.cwl` & `schema-salad-8.5.20240410123758/schema_salad/tests/test_real_cwl/tabs_rna_seq_workflow.cwl`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/tests/test_real_cwl/topmed/topmed_variant_calling_pipeline.cwl` & `schema-salad-8.5.20240410123758/schema_salad/tests/test_real_cwl/topmed/topmed_variant_calling_pipeline.cwl`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/tests/test_real_cwl.py` & `schema-salad-8.5.20240410123758/schema_salad/tests/test_real_cwl.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/tests/test_ref_resolver.py` & `schema-salad-8.5.20240410123758/schema_salad/tests/test_ref_resolver.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/tests/test_schema/Base.yml` & `schema-salad-8.5.20240410123758/schema_salad/tests/test_schema/Base.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/tests/test_schema/CommandLineTool.yml` & `schema-salad-8.5.20240410123758/schema_salad/tests/test_schema/CommandLineTool.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/tests/test_schema/Process.yml` & `schema-salad-8.5.20240410123758/schema_salad/tests/test_schema/Process.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/tests/test_schema/Workflow.yml` & `schema-salad-8.5.20240410123758/schema_salad/tests/test_schema/Workflow.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/tests/test_schema/avro_naming_base.yml` & `schema-salad-8.5.20240410123758/schema_salad/tests/test_schema/avro_naming_base.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/tests/test_schema/avro_subtype.yml` & `schema-salad-8.5.20240410123758/schema_salad/tests/test_schema/avro_subtype.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/tests/test_schema/avro_subtype_bad.yml` & `schema-salad-8.5.20240410123758/schema_salad/tests/test_schema/avro_subtype_bad.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/tests/test_schema/avro_subtype_nested.yml` & `schema-salad-8.5.20240410123758/schema_salad/tests/test_schema/avro_subtype_nested.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/tests/test_schema/avro_subtype_nested_bad.yml` & `schema-salad-8.5.20240410123758/schema_salad/tests/test_schema/avro_subtype_nested_bad.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/tests/test_schema/avro_subtype_recursive.yml` & `schema-salad-8.5.20240410123758/schema_salad/tests/test_schema/avro_subtype_recursive.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/tests/test_schema/avro_subtype_union.yml` & `schema-salad-8.5.20240410123758/schema_salad/tests/test_schema/avro_subtype_union.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/tests/test_schema/avro_subtype_union_bad.yml` & `schema-salad-8.5.20240410123758/schema_salad/tests/test_schema/avro_subtype_union_bad.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/tests/test_schema/cwltest-schema.yml` & `schema-salad-8.5.20240410123758/schema_salad/tests/test_schema/cwltest-schema.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/tests/test_schema/metaschema_base.yml` & `schema-salad-8.5.20240410123758/schema_salad/tests/test_schema/metaschema_base.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/tests/test_schema/misc_schema_v1.yml` & `schema-salad-8.5.20240410123758/schema_salad/tests/test_schema/misc_schema_v1.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/tests/test_schema/misc_schema_v2.yml` & `schema-salad-8.5.20240410123758/schema_salad/tests/test_schema/misc_schema_v2.yml`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/tests/test_schema.py` & `schema-salad-8.5.20240410123758/schema_salad/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/tests/test_schemas_directive.py` & `schema-salad-8.5.20240410123758/schema_salad/tests/test_schemas_directive.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/tests/test_subtypes.py` & `schema-salad-8.5.20240410123758/schema_salad/tests/test_subtypes.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/tests/test_typescript_codegen.py` & `schema-salad-8.5.20240410123758/schema_salad/tests/test_typescript_codegen.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/tests/util.py` & `schema-salad-8.5.20240410123758/schema_salad/tests/util.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/typescript/.gitignore` & `schema-salad-8.5.20240410123758/schema_salad/typescript/.gitignore`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/typescript/LICENSE` & `schema-salad-8.5.20240410123758/schema_salad/typescript/LICENSE`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/typescript/package.json` & `schema-salad-8.5.20240410123758/schema_salad/typescript/package.json`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/typescript/test/AnyLoader.spec.ts` & `schema-salad-8.5.20240410123758/schema_salad/typescript/test/AnyLoader.spec.ts`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/typescript/test/Fetcher.spec.ts` & `schema-salad-8.5.20240410123758/schema_salad/typescript/test/Fetcher.spec.ts`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/typescript/test/IdMap.spec.ts` & `schema-salad-8.5.20240410123758/schema_salad/typescript/test/IdMap.spec.ts`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/typescript/test/Typeguards.spec.ts` & `schema-salad-8.5.20240410123758/schema_salad/typescript/test/Typeguards.spec.ts`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/typescript/test/utilities.spec.ts` & `schema-salad-8.5.20240410123758/schema_salad/typescript/test/utilities.spec.ts`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/typescript/tsconfig.json` & `schema-salad-8.5.20240410123758/schema_salad/typescript/tsconfig.json`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/typescript/util/Fetcher.ts` & `schema-salad-8.5.20240410123758/schema_salad/typescript/util/Fetcher.ts`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/typescript/util/Internal.ts` & `schema-salad-8.5.20240410123758/schema_salad/typescript/util/Internal.ts`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/typescript/util/LoadingOptions.ts` & `schema-salad-8.5.20240410123758/schema_salad/typescript/util/LoadingOptions.ts`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     this.container = container
     this.schemas = schemas
     this.originalDoc = originalDoc
 
     if (copyFrom != null) {
       this.idx = copyFrom.idx
       if (fetcher === undefined) {
-        this.fetcher = copyFrom.fetcher
+        fetcher = copyFrom.fetcher
       }
       if (fileUri === undefined) {
         this.fileUri = copyFrom.fileUri
       }
       if (namespaces === undefined) {
         this.namespaces = copyFrom.namespaces
       }
```

### Comparing `schema-salad-8.5.20240311110950/schema_salad/typescript/util/Saveable.ts` & `schema-salad-8.5.20240410123758/schema_salad/typescript/util/Saveable.ts`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/typescript/util/Typeguards.ts` & `schema-salad-8.5.20240410123758/schema_salad/typescript/util/Typeguards.ts`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/typescript/util/ValidationException.ts` & `schema-salad-8.5.20240410123758/schema_salad/typescript/util/ValidationException.ts`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/typescript/util/loaders/ArrayLoader.ts` & `schema-salad-8.5.20240410123758/schema_salad/typescript/util/loaders/ArrayLoader.ts`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/typescript/util/loaders/IdMapLoader.ts` & `schema-salad-8.5.20240410123758/schema_salad/typescript/util/loaders/IdMapLoader.ts`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/typescript/util/loaders/Loader.ts` & `schema-salad-8.5.20240410123758/schema_salad/typescript/util/loaders/Loader.ts`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/typescript/util/loaders/MapLoader.ts` & `schema-salad-8.5.20240410123758/schema_salad/typescript/util/loaders/MapLoader.ts`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/typescript/util/loaders/RecordLoader.ts` & `schema-salad-8.5.20240410123758/schema_salad/typescript/util/loaders/RecordLoader.ts`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/typescript/util/loaders/RootLoader.ts` & `schema-salad-8.5.20240410123758/schema_salad/typescript/util/loaders/RootLoader.ts`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/typescript/util/loaders/SecondaryDSLLoader.ts` & `schema-salad-8.5.20240410123758/schema_salad/typescript/util/loaders/SecondaryDSLLoader.ts`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/typescript/util/loaders/TypeDSLLoader.ts` & `schema-salad-8.5.20240410123758/schema_salad/typescript/util/loaders/TypeDSLLoader.ts`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/typescript/util/loaders/UnionLoader.ts` & `schema-salad-8.5.20240410123758/schema_salad/typescript/util/loaders/UnionLoader.ts`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/typescript/util/loaders/UriLoader.ts` & `schema-salad-8.5.20240410123758/schema_salad/typescript/util/loaders/UriLoader.ts`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/typescript_codegen.py` & `schema-salad-8.5.20240410123758/schema_salad/typescript_codegen.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/utils.py` & `schema-salad-8.5.20240410123758/schema_salad/utils.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad/validate.py` & `schema-salad-8.5.20240410123758/schema_salad/validate.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad.Dockerfile` & `schema-salad-8.5.20240410123758/schema_salad.Dockerfile`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/schema_salad.egg-info/PKG-INFO` & `schema-salad-8.5.20240410123758/schema_salad.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schema-salad
-Version: 8.5.20240311110950
+Version: 8.5.20240410123758
 Summary: Schema Annotations for Linked Avro Data (SALAD)
 Home-page: https://schema-salad.readthedocs.io/
 Download-URL: https://github.com/common-workflow-language/schema_salad/releases
 Author: Common workflow language working group
 Author-email: common-workflow-language@googlegroups.com
 License: Apache 2.0
 Classifier: Environment :: Console
```

### Comparing `schema-salad-8.5.20240311110950/schema_salad.egg-info/SOURCES.txt` & `schema-salad-8.5.20240410123758/schema_salad.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,14 @@
 test-requirements.txt
 tox.ini
 .circleci/config.yml
 .github/dependabot.yml
 .github/workflows/ci-tests.yml
 .github/workflows/codeql-analysis.yml
 .github/workflows/quay-publish.yml
-.github/workflows/wheel-prep.sh
 .github/workflows/wheels.yml
 docs/Makefile
 docs/cli.rst
 docs/conf.py
 docs/index.rst
 docs/make.bat
 docs/typeshed.rst
@@ -424,14 +423,15 @@
 schema_salad/typescript/index.ts
 schema_salad/typescript/package.json
 schema_salad/typescript/tsconfig.json
 schema_salad/typescript/test/AnyLoader.spec.ts
 schema_salad/typescript/test/ExampleTest.ts
 schema_salad/typescript/test/Fetcher.spec.ts
 schema_salad/typescript/test/IdMap.spec.ts
+schema_salad/typescript/test/LoadingOptions.spec.ts
 schema_salad/typescript/test/Typeguards.spec.ts
 schema_salad/typescript/test/utilities.spec.ts
 schema_salad/typescript/test/data/hellofield.yml
 schema_salad/typescript/test/data/test.txt
 schema_salad/typescript/util/Dict.ts
 schema_salad/typescript/util/Fetcher.ts
 schema_salad/typescript/util/Internal.ts
```

### Comparing `schema-salad-8.5.20240311110950/setup.py` & `schema-salad-8.5.20240410123758/setup.py`

 * *Files identical despite different names*

### Comparing `schema-salad-8.5.20240311110950/tox.ini` & `schema-salad-8.5.20240410123758/tox.ini`

 * *Files identical despite different names*

