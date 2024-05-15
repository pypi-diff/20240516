# Comparing `tmp/plone.exportimport-1.0.0a3.tar.gz` & `tmp/plone.exportimport-1.0.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone.exportimport-1.0.0a3.tar", last modified: Thu May  2 14:45:00 2024, max compression
+gzip compressed data, was "plone.exportimport-1.0.0a4.tar", last modified: Wed May 15 20:35:17 2024, max compression
```

## Comparing `plone.exportimport-1.0.0a3.tar` & `plone.exportimport-1.0.0a4.tar`

### file list

```diff
@@ -1,229 +1,232 @@
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-02 14:45:00.799834 plone.exportimport-1.0.0a3/
--rw-r--r--   0 ericof     (501) staff       (20)     1381 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/.editorconfig
--rw-r--r--   0 ericof     (501) staff       (20)      538 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/.flake8
--rw-r--r--   0 ericof     (501) staff       (20)      722 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/.gitignore
--rw-r--r--   0 ericof     (501) staff       (20)      828 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/.meta.toml
--rw-r--r--   0 ericof     (501) staff       (20)     2023 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/.pre-commit-config.yaml
--rw-r--r--   0 ericof     (501) staff       (20)     1035 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/CHANGES.md
--rw-r--r--   0 ericof     (501) staff       (20)       95 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/CONTRIBUTING.md
--rw-r--r--   0 ericof     (501) staff       (20)    18092 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/LICENSE
--rw-r--r--   0 ericof     (501) staff       (20)      320 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/MANIFEST.in
--rw-r--r--   0 ericof     (501) staff       (20)     3920 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/Makefile
--rw-r--r--   0 ericof     (501) staff       (20)     2971 2024-05-02 14:45:00.799704 plone.exportimport-1.0.0a3/PKG-INFO
--rw-r--r--   0 ericof     (501) staff       (20)      731 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/README.md
--rw-r--r--   0 ericof     (501) staff       (20)       56 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/constraints.txt
--rw-r--r--   0 ericof     (501) staff       (20)      322 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/dependabot.yml
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-02 14:45:00.778721 plone.exportimport-1.0.0a3/docs/
--rw-r--r--   0 ericof     (501) staff       (20)     7078 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/docs/Makefile
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-02 14:45:00.779230 plone.exportimport-1.0.0a3/docs/_static/
--rw-r--r--   0 ericof     (501) staff       (20)     5430 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/docs/_static/favicon.ico
--rw-r--r--   0 ericof     (501) staff       (20)     3775 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/docs/_static/logo.svg
--rw-r--r--   0 ericof     (501) staff       (20)       30 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/docs/_static/print.css
--rw-r--r--   0 ericof     (501) staff       (20)     7814 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/docs/_static/styles.css
--rw-r--r--   0 ericof     (501) staff       (20)     2813 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/docs/conf.py
--rw-r--r--   0 ericof     (501) staff       (20)     1310 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/docs/develop.md
--rw-r--r--   0 ericof     (501) staff       (20)     3374 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/docs/features.md
--rw-r--r--   0 ericof     (501) staff       (20)      722 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/docs/index.md
--rw-r--r--   0 ericof     (501) staff       (20)     1135 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/docs/installation.md
--rw-r--r--   0 ericof     (501) staff       (20)      158 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/instance.yaml
--rw-r--r--   0 ericof     (501) staff       (20)      251 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/mx.ini
--rw-r--r--   0 ericof     (501) staff       (20)     4747 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/pyproject.toml
--rw-r--r--   0 ericof     (501) staff       (20)     1032 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/requirements-docs.txt
--rw-r--r--   0 ericof     (501) staff       (20)       33 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/requirements.txt
--rw-r--r--   0 ericof     (501) staff       (20)       38 2024-05-02 14:45:00.799871 plone.exportimport-1.0.0a3/setup.cfg
--rw-r--r--   0 ericof     (501) staff       (20)     2834 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/setup.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-02 14:45:00.771354 plone.exportimport-1.0.0a3/src/
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-02 14:45:00.779379 plone.exportimport-1.0.0a3/src/plone/
--rw-r--r--   0 ericof     (501) staff       (20)       56 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/src/plone/__init__.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-02 14:45:00.780956 plone.exportimport-1.0.0a3/src/plone/exportimport/
--rw-r--r--   0 ericof     (501) staff       (20)      130 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/src/plone/exportimport/__init__.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-02 14:45:00.781079 plone.exportimport-1.0.0a3/src/plone/exportimport/cli/
--rw-r--r--   0 ericof     (501) staff       (20)     2651 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/src/plone/exportimport/cli/__init__.py
--rw-r--r--   0 ericof     (501) staff       (20)      667 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/src/plone/exportimport/configure.zcml
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-02 14:45:00.781552 plone.exportimport-1.0.0a3/src/plone/exportimport/deserializers/
--rw-r--r--   0 ericof     (501) staff       (20)        0 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/src/plone/exportimport/deserializers/__init__.py
--rw-r--r--   0 ericof     (501) staff       (20)     1670 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/src/plone/exportimport/deserializers/blob.py
--rw-r--r--   0 ericof     (501) staff       (20)      626 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/src/plone/exportimport/deserializers/blocks.py
--rw-r--r--   0 ericof     (501) staff       (20)      193 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/src/plone/exportimport/deserializers/configure.zcml
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-02 14:45:00.782846 plone.exportimport-1.0.0a3/src/plone/exportimport/exporters/
--rw-r--r--   0 ericof     (501) staff       (20)     2459 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/src/plone/exportimport/exporters/__init__.py
--rw-r--r--   0 ericof     (501) staff       (20)     1979 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/src/plone/exportimport/exporters/base.py
--rw-r--r--   0 ericof     (501) staff       (20)     1933 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/src/plone/exportimport/exporters/configure.zcml
--rw-r--r--   0 ericof     (501) staff       (20)     6123 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/src/plone/exportimport/exporters/content.py
--rw-r--r--   0 ericof     (501) staff       (20)      700 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/src/plone/exportimport/exporters/discussions.py
--rw-r--r--   0 ericof     (501) staff       (20)      651 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/src/plone/exportimport/exporters/portlets.py
--rw-r--r--   0 ericof     (501) staff       (20)      828 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/src/plone/exportimport/exporters/principals.py
--rw-r--r--   0 ericof     (501) staff       (20)      660 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/src/plone/exportimport/exporters/redirects.py
--rw-r--r--   0 ericof     (501) staff       (20)      660 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/src/plone/exportimport/exporters/relations.py
--rw-r--r--   0 ericof     (501) staff       (20)      709 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/src/plone/exportimport/exporters/translations.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-02 14:45:00.784686 plone.exportimport-1.0.0a3/src/plone/exportimport/importers/
--rw-r--r--   0 ericof     (501) staff       (20)     1938 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/src/plone/exportimport/importers/__init__.py
--rw-r--r--   0 ericof     (501) staff       (20)     1946 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/src/plone/exportimport/importers/base.py
--rw-r--r--   0 ericof     (501) staff       (20)     1933 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/src/plone/exportimport/importers/configure.zcml
--rw-r--r--   0 ericof     (501) staff       (20)     5277 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/src/plone/exportimport/importers/content.py
--rw-r--r--   0 ericof     (501) staff       (20)      613 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/src/plone/exportimport/importers/discussions.py
--rw-r--r--   0 ericof     (501) staff       (20)      581 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/src/plone/exportimport/importers/portlets.py
--rw-r--r--   0 ericof     (501) staff       (20)     1355 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/src/plone/exportimport/importers/principals.py
--rw-r--r--   0 ericof     (501) staff       (20)      597 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/src/plone/exportimport/importers/redirects.py
--rw-r--r--   0 ericof     (501) staff       (20)      597 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/src/plone/exportimport/importers/relations.py
--rw-r--r--   0 ericof     (501) staff       (20)      617 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/src/plone/exportimport/importers/translations.py
--rw-r--r--   0 ericof     (501) staff       (20)      568 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/src/plone/exportimport/interfaces.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-02 14:45:00.785608 plone.exportimport-1.0.0a3/src/plone/exportimport/serializers/
--rw-r--r--   0 ericof     (501) staff       (20)        0 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/src/plone/exportimport/serializers/__init__.py
--rw-r--r--   0 ericof     (501) staff       (20)     4118 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/src/plone/exportimport/serializers/blob.py
--rw-r--r--   0 ericof     (501) staff       (20)      611 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/src/plone/exportimport/serializers/blocks.py
--rw-r--r--   0 ericof     (501) staff       (20)      388 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/src/plone/exportimport/serializers/configure.zcml
--rw-r--r--   0 ericof     (501) staff       (20)      498 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/src/plone/exportimport/settings.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-02 14:45:00.785757 plone.exportimport-1.0.0a3/src/plone/exportimport/testing/
--rw-r--r--   0 ericof     (501) staff       (20)      762 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/src/plone/exportimport/testing/__init__.py
--rw-r--r--   0 ericof     (501) staff       (20)     1613 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/src/plone/exportimport/types.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-02 14:45:00.787302 plone.exportimport-1.0.0a3/src/plone/exportimport/utils/
--rw-r--r--   0 ericof     (501) staff       (20)       42 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/src/plone/exportimport/utils/__init__.py
--rw-r--r--   0 ericof     (501) staff       (20)     1747 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/src/plone/exportimport/utils/cli.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-02 14:45:00.788493 plone.exportimport-1.0.0a3/src/plone/exportimport/utils/content/
--rw-r--r--   0 ericof     (501) staff       (20)      825 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/src/plone/exportimport/utils/content/__init__.py
--rw-r--r--   0 ericof     (501) staff       (20)     1359 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/src/plone/exportimport/utils/content/blocks.py
--rw-r--r--   0 ericof     (501) staff       (20)     3005 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/src/plone/exportimport/utils/content/core.py
--rw-r--r--   0 ericof     (501) staff       (20)    10232 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/src/plone/exportimport/utils/content/export_helpers.py
--rw-r--r--   0 ericof     (501) staff       (20)    10119 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/src/plone/exportimport/utils/content/import_helpers.py
--rw-r--r--   0 ericof     (501) staff       (20)     1558 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/src/plone/exportimport/utils/content/revisions.py
--rw-r--r--   0 ericof     (501) staff       (20)      592 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/src/plone/exportimport/utils/dates.py
--rw-r--r--   0 ericof     (501) staff       (20)     5169 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/src/plone/exportimport/utils/discussions.py
--rw-r--r--   0 ericof     (501) staff       (20)      627 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/src/plone/exportimport/utils/path.py
--rw-r--r--   0 ericof     (501) staff       (20)     8820 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/src/plone/exportimport/utils/portlets.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-02 14:45:00.789058 plone.exportimport-1.0.0a3/src/plone/exportimport/utils/principals/
--rw-r--r--   0 ericof     (501) staff       (20)      172 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/src/plone/exportimport/utils/principals/__init__.py
--rw-r--r--   0 ericof     (501) staff       (20)     1741 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/src/plone/exportimport/utils/principals/groups.py
--rw-r--r--   0 ericof     (501) staff       (20)     1184 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/src/plone/exportimport/utils/principals/helpers.py
--rw-r--r--   0 ericof     (501) staff       (20)     4217 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/src/plone/exportimport/utils/principals/members.py
--rw-r--r--   0 ericof     (501) staff       (20)      999 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/src/plone/exportimport/utils/redirects.py
--rw-r--r--   0 ericof     (501) staff       (20)     3567 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/src/plone/exportimport/utils/relations.py
--rw-r--r--   0 ericof     (501) staff       (20)     5259 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/src/plone/exportimport/utils/translations.py
--rw-r--r--   0 ericof     (501) staff       (20)      468 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/src/plone/exportimport/utils/zca.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-02 14:45:00.780354 plone.exportimport-1.0.0a3/src/plone.exportimport.egg-info/
--rw-r--r--   0 ericof     (501) staff       (20)     2971 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/src/plone.exportimport.egg-info/PKG-INFO
--rw-r--r--   0 ericof     (501) staff       (20)     7841 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/src/plone.exportimport.egg-info/SOURCES.txt
--rw-r--r--   0 ericof     (501) staff       (20)        1 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/src/plone.exportimport.egg-info/dependency_links.txt
--rw-r--r--   0 ericof     (501) staff       (20)      165 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/src/plone.exportimport.egg-info/entry_points.txt
--rw-r--r--   0 ericof     (501) staff       (20)        6 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/src/plone.exportimport.egg-info/namespace_packages.txt
--rw-r--r--   0 ericof     (501) staff       (20)        1 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/src/plone.exportimport.egg-info/not-zip-safe
--rw-r--r--   0 ericof     (501) staff       (20)      515 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/src/plone.exportimport.egg-info/requires.txt
--rw-r--r--   0 ericof     (501) staff       (20)        6 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/src/plone.exportimport.egg-info/top_level.txt
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-02 14:45:00.789226 plone.exportimport-1.0.0a3/tests/
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-02 14:45:00.773553 plone.exportimport-1.0.0a3/tests/_resources/
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-02 14:45:00.790094 plone.exportimport-1.0.0a3/tests/_resources/base_import/
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-02 14:45:00.790217 plone.exportimport-1.0.0a3/tests/_resources/base_import/content/
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-02 14:45:00.790342 plone.exportimport-1.0.0a3/tests/_resources/base_import/content/35661c9bb5be42c68f665aa1ed291418/
--rw-r--r--   0 ericof     (501) staff       (20)     1404 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/tests/_resources/base_import/content/35661c9bb5be42c68f665aa1ed291418/data.json
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-02 14:45:00.790466 plone.exportimport-1.0.0a3/tests/_resources/base_import/content/3e0dd7c4b2714eafa1d6fc6a1493f953/
--rw-r--r--   0 ericof     (501) staff       (20)     1135 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/tests/_resources/base_import/content/3e0dd7c4b2714eafa1d6fc6a1493f953/data.json
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-02 14:45:00.790598 plone.exportimport-1.0.0a3/tests/_resources/base_import/content/3e0dd7c4b2714eafa1d6fc6a1493f953/file/
--rw-r--r--   0 ericof     (501) staff       (20)     7903 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/tests/_resources/base_import/content/3e0dd7c4b2714eafa1d6fc6a1493f953/file/plone.pdf
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-02 14:45:00.790763 plone.exportimport-1.0.0a3/tests/_resources/base_import/content/45b0b46f17104a7b8fa7bb94d3dd5bd9/
--rw-r--r--   0 ericof     (501) staff       (20)     1447 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/tests/_resources/base_import/content/45b0b46f17104a7b8fa7bb94d3dd5bd9/data.json
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-02 14:45:00.790888 plone.exportimport-1.0.0a3/tests/_resources/base_import/content/5d77cd5686184ec49ab077017b1fbc3a/
--rw-r--r--   0 ericof     (501) staff       (20)     1638 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/tests/_resources/base_import/content/5d77cd5686184ec49ab077017b1fbc3a/data.json
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-02 14:45:00.791006 plone.exportimport-1.0.0a3/tests/_resources/base_import/content/70844f7bec1843b8ab2796c972c9ebfe/
--rw-r--r--   0 ericof     (501) staff       (20)     1455 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/tests/_resources/base_import/content/70844f7bec1843b8ab2796c972c9ebfe/data.json
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-02 14:45:00.791128 plone.exportimport-1.0.0a3/tests/_resources/base_import/content/7c1393f615c4447c80db0d784390c5b7/
--rw-r--r--   0 ericof     (501) staff       (20)     1903 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/tests/_resources/base_import/content/7c1393f615c4447c80db0d784390c5b7/data.json
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-02 14:45:00.791263 plone.exportimport-1.0.0a3/tests/_resources/base_import/content/7c1393f615c4447c80db0d784390c5b7/image/
--rw-r--r--   0 ericof     (501) staff       (20)    66267 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/tests/_resources/base_import/content/7c1393f615c4447c80db0d784390c5b7/image/brazil-coins.png
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-02 14:45:00.791455 plone.exportimport-1.0.0a3/tests/_resources/base_import/content/90b11c863598495ba699b22ca76b1041/
--rw-r--r--   0 ericof     (501) staff       (20)     1256 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/tests/_resources/base_import/content/90b11c863598495ba699b22ca76b1041/data.json
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-02 14:45:00.791574 plone.exportimport-1.0.0a3/tests/_resources/base_import/content/90b11c863598495ba699b22ca76b1041/image/
--rw-r--r--   0 ericof     (501) staff       (20)    40383 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/tests/_resources/base_import/content/90b11c863598495ba699b22ca76b1041/image/2025.png
--rw-r--r--   0 ericof     (501) staff       (20)     2349 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/tests/_resources/base_import/content/__metadata__.json
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-02 14:45:00.791946 plone.exportimport-1.0.0a3/tests/_resources/base_import/content/e7359727ace64e609b79c4091c38822a/
--rw-r--r--   0 ericof     (501) staff       (20)     3720 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/tests/_resources/base_import/content/e7359727ace64e609b79c4091c38822a/data.json
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-02 14:45:00.792070 plone.exportimport-1.0.0a3/tests/_resources/base_import/content/plone_site_root/
--rw-r--r--   0 ericof     (501) staff       (20)    18437 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/tests/_resources/base_import/content/plone_site_root/data.json
--rw-r--r--   0 ericof     (501) staff       (20)     4827 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/tests/_resources/base_import/discussions.json
--rw-r--r--   0 ericof     (501) staff       (20)     1583 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/tests/_resources/base_import/portlets.json
--rw-r--r--   0 ericof     (501) staff       (20)     1877 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/tests/_resources/base_import/principals.json
--rw-r--r--   0 ericof     (501) staff       (20)        3 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/tests/_resources/base_import/redirects.json
--rw-r--r--   0 ericof     (501) staff       (20)        3 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/tests/_resources/base_import/relations.json
--rw-r--r--   0 ericof     (501) staff       (20)        3 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/tests/_resources/base_import/translations.json
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-02 14:45:00.792223 plone.exportimport-1.0.0a3/tests/_resources/empty_import/
--rw-r--r--   0 ericof     (501) staff       (20)        0 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/tests/_resources/empty_import/.gitkeep
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-02 14:45:00.792820 plone.exportimport-1.0.0a3/tests/_resources/multilingual_import/
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-02 14:45:00.792941 plone.exportimport-1.0.0a3/tests/_resources/multilingual_import/content/
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-02 14:45:00.793093 plone.exportimport-1.0.0a3/tests/_resources/multilingual_import/content/01fbca4cccd448d880959ba93aa8176e/
--rw-r--r--   0 ericof     (501) staff       (20)     1168 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/tests/_resources/multilingual_import/content/01fbca4cccd448d880959ba93aa8176e/data.json
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-02 14:45:00.793217 plone.exportimport-1.0.0a3/tests/_resources/multilingual_import/content/1cbf4ae73c74459485d3fd6cb9714e43/
--rw-r--r--   0 ericof     (501) staff       (20)     1468 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/tests/_resources/multilingual_import/content/1cbf4ae73c74459485d3fd6cb9714e43/data.json
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-02 14:45:00.793347 plone.exportimport-1.0.0a3/tests/_resources/multilingual_import/content/20737423549c43a88488242ec629e087/
--rw-r--r--   0 ericof     (501) staff       (20)     1297 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/tests/_resources/multilingual_import/content/20737423549c43a88488242ec629e087/data.json
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-02 14:45:00.793469 plone.exportimport-1.0.0a3/tests/_resources/multilingual_import/content/2be023c76b3e4e0aa9908c70f19a14df/
--rw-r--r--   0 ericof     (501) staff       (20)     1502 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/tests/_resources/multilingual_import/content/2be023c76b3e4e0aa9908c70f19a14df/data.json
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-02 14:45:00.793588 plone.exportimport-1.0.0a3/tests/_resources/multilingual_import/content/2d099ac593344be7aaf2e4aafbba9065/
--rw-r--r--   0 ericof     (501) staff       (20)     1428 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/tests/_resources/multilingual_import/content/2d099ac593344be7aaf2e4aafbba9065/data.json
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-02 14:45:00.793711 plone.exportimport-1.0.0a3/tests/_resources/multilingual_import/content/3e3d4bf2cac4482f9c03e34b52092f02/
--rw-r--r--   0 ericof     (501) staff       (20)     1177 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/tests/_resources/multilingual_import/content/3e3d4bf2cac4482f9c03e34b52092f02/data.json
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-02 14:45:00.793838 plone.exportimport-1.0.0a3/tests/_resources/multilingual_import/content/496cbe4f17904d6bb9321b23f91dc8cc/
--rw-r--r--   0 ericof     (501) staff       (20)     1463 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/tests/_resources/multilingual_import/content/496cbe4f17904d6bb9321b23f91dc8cc/data.json
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-02 14:45:00.793969 plone.exportimport-1.0.0a3/tests/_resources/multilingual_import/content/59e06b23024a4c4b9d93672fe440e019/
--rw-r--r--   0 ericof     (501) staff       (20)     1295 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/tests/_resources/multilingual_import/content/59e06b23024a4c4b9d93672fe440e019/data.json
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-02 14:45:00.794091 plone.exportimport-1.0.0a3/tests/_resources/multilingual_import/content/5ffe1d0c89c745eaab26df0e71ac82de/
--rw-r--r--   0 ericof     (501) staff       (20)     1419 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/tests/_resources/multilingual_import/content/5ffe1d0c89c745eaab26df0e71ac82de/data.json
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-02 14:45:00.794219 plone.exportimport-1.0.0a3/tests/_resources/multilingual_import/content/6d8a2b38d445462aa19f604b0801a13c/
--rw-r--r--   0 ericof     (501) staff       (20)     1286 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/tests/_resources/multilingual_import/content/6d8a2b38d445462aa19f604b0801a13c/data.json
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-02 14:45:00.794337 plone.exportimport-1.0.0a3/tests/_resources/multilingual_import/content/85a60611c2744e7abe53e3f356df236a/
--rw-r--r--   0 ericof     (501) staff       (20)     1520 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/tests/_resources/multilingual_import/content/85a60611c2744e7abe53e3f356df236a/data.json
--rw-r--r--   0 ericof     (501) staff       (20)     4390 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/tests/_resources/multilingual_import/content/__metadata__.json
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-02 14:45:00.794463 plone.exportimport-1.0.0a3/tests/_resources/multilingual_import/content/b69412b6d0b0438d85b340c13a39fc8c/
--rw-r--r--   0 ericof     (501) staff       (20)     1520 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/tests/_resources/multilingual_import/content/b69412b6d0b0438d85b340c13a39fc8c/data.json
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-02 14:45:00.794586 plone.exportimport-1.0.0a3/tests/_resources/multilingual_import/content/cecc6f7007344d3cbac68f1da4bd084a/
--rw-r--r--   0 ericof     (501) staff       (20)     1502 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/tests/_resources/multilingual_import/content/cecc6f7007344d3cbac68f1da4bd084a/data.json
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-02 14:45:00.794705 plone.exportimport-1.0.0a3/tests/_resources/multilingual_import/content/ddb27456033d4b86a78f3ec783874b63/
--rw-r--r--   0 ericof     (501) staff       (20)     1419 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/tests/_resources/multilingual_import/content/ddb27456033d4b86a78f3ec783874b63/data.json
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-02 14:45:00.794824 plone.exportimport-1.0.0a3/tests/_resources/multilingual_import/content/f40d3a236b464aa487b715adf3c0be92/
--rw-r--r--   0 ericof     (501) staff       (20)     1511 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/tests/_resources/multilingual_import/content/f40d3a236b464aa487b715adf3c0be92/data.json
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-02 14:45:00.794954 plone.exportimport-1.0.0a3/tests/_resources/multilingual_import/content/f9767fbdadf041bd892010d21b290cb5/
--rw-r--r--   0 ericof     (501) staff       (20)     1472 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/tests/_resources/multilingual_import/content/f9767fbdadf041bd892010d21b290cb5/data.json
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-02 14:45:00.795080 plone.exportimport-1.0.0a3/tests/_resources/multilingual_import/content/f98b033fa8ce46f487ca8923ddae7480/
--rw-r--r--   0 ericof     (501) staff       (20)     1173 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/tests/_resources/multilingual_import/content/f98b033fa8ce46f487ca8923ddae7480/data.json
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-02 14:45:00.795199 plone.exportimport-1.0.0a3/tests/_resources/multilingual_import/content/fbcd98e2d1a741e2a90b8f0389203530/
--rw-r--r--   0 ericof     (501) staff       (20)     1529 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/tests/_resources/multilingual_import/content/fbcd98e2d1a741e2a90b8f0389203530/data.json
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-02 14:45:00.795328 plone.exportimport-1.0.0a3/tests/_resources/multilingual_import/content/plone_site_root/
--rw-r--r--   0 ericof     (501) staff       (20)      738 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/tests/_resources/multilingual_import/content/plone_site_root/data.json
--rw-r--r--   0 ericof     (501) staff       (20)     4888 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/tests/_resources/multilingual_import/discussions.json
--rw-r--r--   0 ericof     (501) staff       (20)     1877 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/tests/_resources/multilingual_import/principals.json
--rw-r--r--   0 ericof     (501) staff       (20)       41 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/tests/_resources/multilingual_import/redirects.json
--rw-r--r--   0 ericof     (501) staff       (20)      452 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/tests/_resources/multilingual_import/relations.json
--rw-r--r--   0 ericof     (501) staff       (20)      928 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/tests/_resources/multilingual_import/translations.json
--rw-r--r--   0 ericof     (501) staff       (20)     7068 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/tests/conftest.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-02 14:45:00.796543 plone.exportimport-1.0.0a3/tests/exporters/
--rw-r--r--   0 ericof     (501) staff       (20)      864 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/tests/exporters/conftest.py
--rw-r--r--   0 ericof     (501) staff       (20)     3239 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/tests/exporters/test_exporters.py
--rw-r--r--   0 ericof     (501) staff       (20)     2556 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/tests/exporters/test_exporters_content.py
--rw-r--r--   0 ericof     (501) staff       (20)     1942 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/tests/exporters/test_exporters_discussions.py
--rw-r--r--   0 ericof     (501) staff       (20)     1966 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/tests/exporters/test_exporters_portlets.py
--rw-r--r--   0 ericof     (501) staff       (20)     1303 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/tests/exporters/test_exporters_principals.py
--rw-r--r--   0 ericof     (501) staff       (20)     1294 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/tests/exporters/test_exporters_redirects.py
--rw-r--r--   0 ericof     (501) staff       (20)     1861 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/tests/exporters/test_exporters_relations.py
--rw-r--r--   0 ericof     (501) staff       (20)     1890 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/tests/exporters/test_exporters_translations.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-02 14:45:00.797763 plone.exportimport-1.0.0a3/tests/importers/
--rw-r--r--   0 ericof     (501) staff       (20)      666 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/tests/importers/conftest.py
--rw-r--r--   0 ericof     (501) staff       (20)     1533 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/tests/importers/test_importers.py
--rw-r--r--   0 ericof     (501) staff       (20)     1118 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/tests/importers/test_importers_content.py
--rw-r--r--   0 ericof     (501) staff       (20)     1437 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/tests/importers/test_importers_discussions.py
--rw-r--r--   0 ericof     (501) staff       (20)     1517 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/tests/importers/test_importers_portlets.py
--rw-r--r--   0 ericof     (501) staff       (20)     1434 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/tests/importers/test_importers_principals.py
--rw-r--r--   0 ericof     (501) staff       (20)     1413 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/tests/importers/test_importers_redirects.py
--rw-r--r--   0 ericof     (501) staff       (20)     1413 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/tests/importers/test_importers_relations.py
--rw-r--r--   0 ericof     (501) staff       (20)     1446 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/tests/importers/test_importers_translations.py
-drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-02 14:45:00.799496 plone.exportimport-1.0.0a3/tests/utils/
--rw-r--r--   0 ericof     (501) staff       (20)        0 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/tests/utils/conftest.py
--rw-r--r--   0 ericof     (501) staff       (20)     3700 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/tests/utils/test_utils_content_core.py
--rw-r--r--   0 ericof     (501) staff       (20)     1111 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/tests/utils/test_utils_content_export_helpers.py
--rw-r--r--   0 ericof     (501) staff       (20)      860 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/tests/utils/test_utils_content_revisions.py
--rw-r--r--   0 ericof     (501) staff       (20)     1304 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/tests/utils/test_utils_dates.py
--rw-r--r--   0 ericof     (501) staff       (20)     3688 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/tests/utils/test_utils_discussions.py
--rw-r--r--   0 ericof     (501) staff       (20)     1365 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/tests/utils/test_utils_path.py
--rw-r--r--   0 ericof     (501) staff       (20)     1023 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/tests/utils/test_utils_principals_groups.py
--rw-r--r--   0 ericof     (501) staff       (20)     1184 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/tests/utils/test_utils_principals_members.py
--rw-r--r--   0 ericof     (501) staff       (20)     1252 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/tests/utils/test_utils_redirects.py
--rw-r--r--   0 ericof     (501) staff       (20)     5384 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/tests/utils/test_utils_relations.py
--rw-r--r--   0 ericof     (501) staff       (20)     5186 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/tests/utils/test_utils_translations.py
--rw-r--r--   0 ericof     (501) staff       (20)     4873 2024-05-02 14:45:00.000000 plone.exportimport-1.0.0a3/tox.ini
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-15 20:35:17.322775 plone.exportimport-1.0.0a4/
+-rw-r--r--   0 ericof     (501) staff       (20)     1381 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/.editorconfig
+-rw-r--r--   0 ericof     (501) staff       (20)      538 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/.flake8
+-rw-r--r--   0 ericof     (501) staff       (20)      722 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/.gitignore
+-rw-r--r--   0 ericof     (501) staff       (20)      865 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/.meta.toml
+-rw-r--r--   0 ericof     (501) staff       (20)     2023 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/.pre-commit-config.yaml
+-rw-r--r--   0 ericof     (501) staff       (20)     1376 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/CHANGES.md
+-rw-r--r--   0 ericof     (501) staff       (20)       95 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/CONTRIBUTING.md
+-rw-r--r--   0 ericof     (501) staff       (20)    18092 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/LICENSE
+-rw-r--r--   0 ericof     (501) staff       (20)      320 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/MANIFEST.in
+-rw-r--r--   0 ericof     (501) staff       (20)     3920 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/Makefile
+-rw-r--r--   0 ericof     (501) staff       (20)     3312 2024-05-15 20:35:17.322600 plone.exportimport-1.0.0a4/PKG-INFO
+-rw-r--r--   0 ericof     (501) staff       (20)      731 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/README.md
+-rw-r--r--   0 ericof     (501) staff       (20)       56 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/constraints.txt
+-rw-r--r--   0 ericof     (501) staff       (20)      322 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/dependabot.yml
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-15 20:35:17.301202 plone.exportimport-1.0.0a4/docs/
+-rw-r--r--   0 ericof     (501) staff       (20)     7078 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/docs/Makefile
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-15 20:35:17.301729 plone.exportimport-1.0.0a4/docs/_static/
+-rw-r--r--   0 ericof     (501) staff       (20)     5430 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/docs/_static/favicon.ico
+-rw-r--r--   0 ericof     (501) staff       (20)     3775 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/docs/_static/logo.svg
+-rw-r--r--   0 ericof     (501) staff       (20)       30 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/docs/_static/print.css
+-rw-r--r--   0 ericof     (501) staff       (20)     7814 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/docs/_static/styles.css
+-rw-r--r--   0 ericof     (501) staff       (20)     2813 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/docs/conf.py
+-rw-r--r--   0 ericof     (501) staff       (20)     1310 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/docs/develop.md
+-rw-r--r--   0 ericof     (501) staff       (20)     3374 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/docs/features.md
+-rw-r--r--   0 ericof     (501) staff       (20)      722 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/docs/index.md
+-rw-r--r--   0 ericof     (501) staff       (20)     1135 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/docs/installation.md
+-rw-r--r--   0 ericof     (501) staff       (20)      158 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/instance.yaml
+-rw-r--r--   0 ericof     (501) staff       (20)      251 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/mx.ini
+-rw-r--r--   0 ericof     (501) staff       (20)     4747 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/pyproject.toml
+-rw-r--r--   0 ericof     (501) staff       (20)     1032 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/requirements-docs.txt
+-rw-r--r--   0 ericof     (501) staff       (20)       33 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/requirements.txt
+-rw-r--r--   0 ericof     (501) staff       (20)       38 2024-05-15 20:35:17.322820 plone.exportimport-1.0.0a4/setup.cfg
+-rw-r--r--   0 ericof     (501) staff       (20)     2834 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/setup.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-15 20:35:17.293035 plone.exportimport-1.0.0a4/src/
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-15 20:35:17.301876 plone.exportimport-1.0.0a4/src/plone/
+-rw-r--r--   0 ericof     (501) staff       (20)       56 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/src/plone/__init__.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-15 20:35:17.303752 plone.exportimport-1.0.0a4/src/plone/exportimport/
+-rw-r--r--   0 ericof     (501) staff       (20)      130 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/src/plone/exportimport/__init__.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-15 20:35:17.303894 plone.exportimport-1.0.0a4/src/plone/exportimport/cli/
+-rw-r--r--   0 ericof     (501) staff       (20)     2651 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/src/plone/exportimport/cli/__init__.py
+-rw-r--r--   0 ericof     (501) staff       (20)      667 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/src/plone/exportimport/configure.zcml
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-15 20:35:17.304409 plone.exportimport-1.0.0a4/src/plone/exportimport/deserializers/
+-rw-r--r--   0 ericof     (501) staff       (20)        0 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/src/plone/exportimport/deserializers/__init__.py
+-rw-r--r--   0 ericof     (501) staff       (20)     1670 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/src/plone/exportimport/deserializers/blob.py
+-rw-r--r--   0 ericof     (501) staff       (20)      626 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/src/plone/exportimport/deserializers/blocks.py
+-rw-r--r--   0 ericof     (501) staff       (20)      193 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/src/plone/exportimport/deserializers/configure.zcml
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-15 20:35:17.305782 plone.exportimport-1.0.0a4/src/plone/exportimport/exporters/
+-rw-r--r--   0 ericof     (501) staff       (20)     2459 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/src/plone/exportimport/exporters/__init__.py
+-rw-r--r--   0 ericof     (501) staff       (20)     1979 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/src/plone/exportimport/exporters/base.py
+-rw-r--r--   0 ericof     (501) staff       (20)     1933 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/src/plone/exportimport/exporters/configure.zcml
+-rw-r--r--   0 ericof     (501) staff       (20)     6128 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/src/plone/exportimport/exporters/content.py
+-rw-r--r--   0 ericof     (501) staff       (20)      700 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/src/plone/exportimport/exporters/discussions.py
+-rw-r--r--   0 ericof     (501) staff       (20)      651 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/src/plone/exportimport/exporters/portlets.py
+-rw-r--r--   0 ericof     (501) staff       (20)      828 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/src/plone/exportimport/exporters/principals.py
+-rw-r--r--   0 ericof     (501) staff       (20)      660 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/src/plone/exportimport/exporters/redirects.py
+-rw-r--r--   0 ericof     (501) staff       (20)      660 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/src/plone/exportimport/exporters/relations.py
+-rw-r--r--   0 ericof     (501) staff       (20)      709 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/src/plone/exportimport/exporters/translations.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-15 20:35:17.307100 plone.exportimport-1.0.0a4/src/plone/exportimport/importers/
+-rw-r--r--   0 ericof     (501) staff       (20)     1938 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/src/plone/exportimport/importers/__init__.py
+-rw-r--r--   0 ericof     (501) staff       (20)     2169 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/src/plone/exportimport/importers/base.py
+-rw-r--r--   0 ericof     (501) staff       (20)     1933 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/src/plone/exportimport/importers/configure.zcml
+-rw-r--r--   0 ericof     (501) staff       (20)     5928 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/src/plone/exportimport/importers/content.py
+-rw-r--r--   0 ericof     (501) staff       (20)      613 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/src/plone/exportimport/importers/discussions.py
+-rw-r--r--   0 ericof     (501) staff       (20)      586 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/src/plone/exportimport/importers/portlets.py
+-rw-r--r--   0 ericof     (501) staff       (20)     1355 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/src/plone/exportimport/importers/principals.py
+-rw-r--r--   0 ericof     (501) staff       (20)      597 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/src/plone/exportimport/importers/redirects.py
+-rw-r--r--   0 ericof     (501) staff       (20)      912 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/src/plone/exportimport/importers/relations.py
+-rw-r--r--   0 ericof     (501) staff       (20)      617 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/src/plone/exportimport/importers/translations.py
+-rw-r--r--   0 ericof     (501) staff       (20)      568 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/src/plone/exportimport/interfaces.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-15 20:35:17.307751 plone.exportimport-1.0.0a4/src/plone/exportimport/serializers/
+-rw-r--r--   0 ericof     (501) staff       (20)        0 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/src/plone/exportimport/serializers/__init__.py
+-rw-r--r--   0 ericof     (501) staff       (20)     4118 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/src/plone/exportimport/serializers/blob.py
+-rw-r--r--   0 ericof     (501) staff       (20)      611 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/src/plone/exportimport/serializers/blocks.py
+-rw-r--r--   0 ericof     (501) staff       (20)      500 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/src/plone/exportimport/serializers/configure.zcml
+-rw-r--r--   0 ericof     (501) staff       (20)     3234 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/src/plone/exportimport/serializers/fields.py
+-rw-r--r--   0 ericof     (501) staff       (20)      498 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/src/plone/exportimport/settings.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-15 20:35:17.308020 plone.exportimport-1.0.0a4/src/plone/exportimport/testing/
+-rw-r--r--   0 ericof     (501) staff       (20)      762 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/src/plone/exportimport/testing/__init__.py
+-rw-r--r--   0 ericof     (501) staff       (20)     1613 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/src/plone/exportimport/types.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-15 20:35:17.309391 plone.exportimport-1.0.0a4/src/plone/exportimport/utils/
+-rw-r--r--   0 ericof     (501) staff       (20)       42 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/src/plone/exportimport/utils/__init__.py
+-rw-r--r--   0 ericof     (501) staff       (20)     1747 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/src/plone/exportimport/utils/cli.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-15 20:35:17.310218 plone.exportimport-1.0.0a4/src/plone/exportimport/utils/content/
+-rw-r--r--   0 ericof     (501) staff       (20)      825 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/src/plone/exportimport/utils/content/__init__.py
+-rw-r--r--   0 ericof     (501) staff       (20)     1359 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/src/plone/exportimport/utils/content/blocks.py
+-rw-r--r--   0 ericof     (501) staff       (20)     3005 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/src/plone/exportimport/utils/content/core.py
+-rw-r--r--   0 ericof     (501) staff       (20)    10232 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/src/plone/exportimport/utils/content/export_helpers.py
+-rw-r--r--   0 ericof     (501) staff       (20)    10215 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/src/plone/exportimport/utils/content/import_helpers.py
+-rw-r--r--   0 ericof     (501) staff       (20)     1558 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/src/plone/exportimport/utils/content/revisions.py
+-rw-r--r--   0 ericof     (501) staff       (20)      592 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/src/plone/exportimport/utils/dates.py
+-rw-r--r--   0 ericof     (501) staff       (20)     5169 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/src/plone/exportimport/utils/discussions.py
+-rw-r--r--   0 ericof     (501) staff       (20)      627 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/src/plone/exportimport/utils/path.py
+-rw-r--r--   0 ericof     (501) staff       (20)    10615 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/src/plone/exportimport/utils/portlets.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-15 20:35:17.310761 plone.exportimport-1.0.0a4/src/plone/exportimport/utils/principals/
+-rw-r--r--   0 ericof     (501) staff       (20)      172 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/src/plone/exportimport/utils/principals/__init__.py
+-rw-r--r--   0 ericof     (501) staff       (20)     1808 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/src/plone/exportimport/utils/principals/groups.py
+-rw-r--r--   0 ericof     (501) staff       (20)     1184 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/src/plone/exportimport/utils/principals/helpers.py
+-rw-r--r--   0 ericof     (501) staff       (20)     4217 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/src/plone/exportimport/utils/principals/members.py
+-rw-r--r--   0 ericof     (501) staff       (20)      999 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/src/plone/exportimport/utils/redirects.py
+-rw-r--r--   0 ericof     (501) staff       (20)     3567 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/src/plone/exportimport/utils/relations.py
+-rw-r--r--   0 ericof     (501) staff       (20)     5259 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/src/plone/exportimport/utils/translations.py
+-rw-r--r--   0 ericof     (501) staff       (20)      468 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/src/plone/exportimport/utils/zca.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-15 20:35:17.303025 plone.exportimport-1.0.0a4/src/plone.exportimport.egg-info/
+-rw-r--r--   0 ericof     (501) staff       (20)     3312 2024-05-15 20:35:17.000000 plone.exportimport-1.0.0a4/src/plone.exportimport.egg-info/PKG-INFO
+-rw-r--r--   0 ericof     (501) staff       (20)     7933 2024-05-15 20:35:17.000000 plone.exportimport-1.0.0a4/src/plone.exportimport.egg-info/SOURCES.txt
+-rw-r--r--   0 ericof     (501) staff       (20)        1 2024-05-15 20:35:17.000000 plone.exportimport-1.0.0a4/src/plone.exportimport.egg-info/dependency_links.txt
+-rw-r--r--   0 ericof     (501) staff       (20)      165 2024-05-15 20:35:17.000000 plone.exportimport-1.0.0a4/src/plone.exportimport.egg-info/entry_points.txt
+-rw-r--r--   0 ericof     (501) staff       (20)        6 2024-05-15 20:35:17.000000 plone.exportimport-1.0.0a4/src/plone.exportimport.egg-info/namespace_packages.txt
+-rw-r--r--   0 ericof     (501) staff       (20)        1 2024-05-15 20:35:17.000000 plone.exportimport-1.0.0a4/src/plone.exportimport.egg-info/not-zip-safe
+-rw-r--r--   0 ericof     (501) staff       (20)      515 2024-05-15 20:35:17.000000 plone.exportimport-1.0.0a4/src/plone.exportimport.egg-info/requires.txt
+-rw-r--r--   0 ericof     (501) staff       (20)        6 2024-05-15 20:35:17.000000 plone.exportimport-1.0.0a4/src/plone.exportimport.egg-info/top_level.txt
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-15 20:35:17.310915 plone.exportimport-1.0.0a4/tests/
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-15 20:35:17.297447 plone.exportimport-1.0.0a4/tests/_resources/
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-15 20:35:17.311737 plone.exportimport-1.0.0a4/tests/_resources/base_import/
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-15 20:35:17.311855 plone.exportimport-1.0.0a4/tests/_resources/base_import/content/
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-15 20:35:17.312223 plone.exportimport-1.0.0a4/tests/_resources/base_import/content/35661c9bb5be42c68f665aa1ed291418/
+-rw-r--r--   0 ericof     (501) staff       (20)     1404 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/tests/_resources/base_import/content/35661c9bb5be42c68f665aa1ed291418/data.json
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-15 20:35:17.312417 plone.exportimport-1.0.0a4/tests/_resources/base_import/content/3e0dd7c4b2714eafa1d6fc6a1493f953/
+-rw-r--r--   0 ericof     (501) staff       (20)     1135 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/tests/_resources/base_import/content/3e0dd7c4b2714eafa1d6fc6a1493f953/data.json
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-15 20:35:17.312573 plone.exportimport-1.0.0a4/tests/_resources/base_import/content/3e0dd7c4b2714eafa1d6fc6a1493f953/file/
+-rw-r--r--   0 ericof     (501) staff       (20)     7903 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/tests/_resources/base_import/content/3e0dd7c4b2714eafa1d6fc6a1493f953/file/plone.pdf
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-15 20:35:17.312733 plone.exportimport-1.0.0a4/tests/_resources/base_import/content/45b0b46f17104a7b8fa7bb94d3dd5bd9/
+-rw-r--r--   0 ericof     (501) staff       (20)     1447 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/tests/_resources/base_import/content/45b0b46f17104a7b8fa7bb94d3dd5bd9/data.json
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-15 20:35:17.312876 plone.exportimport-1.0.0a4/tests/_resources/base_import/content/5d77cd5686184ec49ab077017b1fbc3a/
+-rw-r--r--   0 ericof     (501) staff       (20)     1638 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/tests/_resources/base_import/content/5d77cd5686184ec49ab077017b1fbc3a/data.json
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-15 20:35:17.313027 plone.exportimport-1.0.0a4/tests/_resources/base_import/content/70844f7bec1843b8ab2796c972c9ebfe/
+-rw-r--r--   0 ericof     (501) staff       (20)     1455 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/tests/_resources/base_import/content/70844f7bec1843b8ab2796c972c9ebfe/data.json
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-15 20:35:17.313170 plone.exportimport-1.0.0a4/tests/_resources/base_import/content/7c1393f615c4447c80db0d784390c5b7/
+-rw-r--r--   0 ericof     (501) staff       (20)     1903 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/tests/_resources/base_import/content/7c1393f615c4447c80db0d784390c5b7/data.json
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-15 20:35:17.313317 plone.exportimport-1.0.0a4/tests/_resources/base_import/content/7c1393f615c4447c80db0d784390c5b7/image/
+-rw-r--r--   0 ericof     (501) staff       (20)    66267 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/tests/_resources/base_import/content/7c1393f615c4447c80db0d784390c5b7/image/brazil-coins.png
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-15 20:35:17.313550 plone.exportimport-1.0.0a4/tests/_resources/base_import/content/90b11c863598495ba699b22ca76b1041/
+-rw-r--r--   0 ericof     (501) staff       (20)     1256 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/tests/_resources/base_import/content/90b11c863598495ba699b22ca76b1041/data.json
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-15 20:35:17.313820 plone.exportimport-1.0.0a4/tests/_resources/base_import/content/90b11c863598495ba699b22ca76b1041/image/
+-rw-r--r--   0 ericof     (501) staff       (20)    40383 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/tests/_resources/base_import/content/90b11c863598495ba699b22ca76b1041/image/2025.png
+-rw-r--r--   0 ericof     (501) staff       (20)     2349 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/tests/_resources/base_import/content/__metadata__.json
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-15 20:35:17.314007 plone.exportimport-1.0.0a4/tests/_resources/base_import/content/e7359727ace64e609b79c4091c38822a/
+-rw-r--r--   0 ericof     (501) staff       (20)     3720 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/tests/_resources/base_import/content/e7359727ace64e609b79c4091c38822a/data.json
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-15 20:35:17.314157 plone.exportimport-1.0.0a4/tests/_resources/base_import/content/plone_site_root/
+-rw-r--r--   0 ericof     (501) staff       (20)    18437 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/tests/_resources/base_import/content/plone_site_root/data.json
+-rw-r--r--   0 ericof     (501) staff       (20)     4827 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/tests/_resources/base_import/discussions.json
+-rw-r--r--   0 ericof     (501) staff       (20)     1947 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/tests/_resources/base_import/portlets.json
+-rw-r--r--   0 ericof     (501) staff       (20)     1877 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/tests/_resources/base_import/principals.json
+-rw-r--r--   0 ericof     (501) staff       (20)        3 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/tests/_resources/base_import/redirects.json
+-rw-r--r--   0 ericof     (501) staff       (20)        3 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/tests/_resources/base_import/relations.json
+-rw-r--r--   0 ericof     (501) staff       (20)        3 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/tests/_resources/base_import/translations.json
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-15 20:35:17.314316 plone.exportimport-1.0.0a4/tests/_resources/empty_import/
+-rw-r--r--   0 ericof     (501) staff       (20)        0 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/tests/_resources/empty_import/.gitkeep
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-15 20:35:17.315144 plone.exportimport-1.0.0a4/tests/_resources/multilingual_import/
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-15 20:35:17.315289 plone.exportimport-1.0.0a4/tests/_resources/multilingual_import/content/
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-15 20:35:17.315439 plone.exportimport-1.0.0a4/tests/_resources/multilingual_import/content/01fbca4cccd448d880959ba93aa8176e/
+-rw-r--r--   0 ericof     (501) staff       (20)     1168 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/tests/_resources/multilingual_import/content/01fbca4cccd448d880959ba93aa8176e/data.json
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-15 20:35:17.315583 plone.exportimport-1.0.0a4/tests/_resources/multilingual_import/content/1cbf4ae73c74459485d3fd6cb9714e43/
+-rw-r--r--   0 ericof     (501) staff       (20)     1468 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/tests/_resources/multilingual_import/content/1cbf4ae73c74459485d3fd6cb9714e43/data.json
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-15 20:35:17.315739 plone.exportimport-1.0.0a4/tests/_resources/multilingual_import/content/20737423549c43a88488242ec629e087/
+-rw-r--r--   0 ericof     (501) staff       (20)     1297 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/tests/_resources/multilingual_import/content/20737423549c43a88488242ec629e087/data.json
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-15 20:35:17.315884 plone.exportimport-1.0.0a4/tests/_resources/multilingual_import/content/2be023c76b3e4e0aa9908c70f19a14df/
+-rw-r--r--   0 ericof     (501) staff       (20)     1502 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/tests/_resources/multilingual_import/content/2be023c76b3e4e0aa9908c70f19a14df/data.json
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-15 20:35:17.316029 plone.exportimport-1.0.0a4/tests/_resources/multilingual_import/content/2d099ac593344be7aaf2e4aafbba9065/
+-rw-r--r--   0 ericof     (501) staff       (20)     1428 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/tests/_resources/multilingual_import/content/2d099ac593344be7aaf2e4aafbba9065/data.json
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-15 20:35:17.316161 plone.exportimport-1.0.0a4/tests/_resources/multilingual_import/content/3e3d4bf2cac4482f9c03e34b52092f02/
+-rw-r--r--   0 ericof     (501) staff       (20)     1177 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/tests/_resources/multilingual_import/content/3e3d4bf2cac4482f9c03e34b52092f02/data.json
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-15 20:35:17.316300 plone.exportimport-1.0.0a4/tests/_resources/multilingual_import/content/496cbe4f17904d6bb9321b23f91dc8cc/
+-rw-r--r--   0 ericof     (501) staff       (20)     1463 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/tests/_resources/multilingual_import/content/496cbe4f17904d6bb9321b23f91dc8cc/data.json
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-15 20:35:17.316440 plone.exportimport-1.0.0a4/tests/_resources/multilingual_import/content/59e06b23024a4c4b9d93672fe440e019/
+-rw-r--r--   0 ericof     (501) staff       (20)     1295 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/tests/_resources/multilingual_import/content/59e06b23024a4c4b9d93672fe440e019/data.json
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-15 20:35:17.316583 plone.exportimport-1.0.0a4/tests/_resources/multilingual_import/content/5ffe1d0c89c745eaab26df0e71ac82de/
+-rw-r--r--   0 ericof     (501) staff       (20)     1419 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/tests/_resources/multilingual_import/content/5ffe1d0c89c745eaab26df0e71ac82de/data.json
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-15 20:35:17.316720 plone.exportimport-1.0.0a4/tests/_resources/multilingual_import/content/6d8a2b38d445462aa19f604b0801a13c/
+-rw-r--r--   0 ericof     (501) staff       (20)     1286 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/tests/_resources/multilingual_import/content/6d8a2b38d445462aa19f604b0801a13c/data.json
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-15 20:35:17.316850 plone.exportimport-1.0.0a4/tests/_resources/multilingual_import/content/85a60611c2744e7abe53e3f356df236a/
+-rw-r--r--   0 ericof     (501) staff       (20)     1520 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/tests/_resources/multilingual_import/content/85a60611c2744e7abe53e3f356df236a/data.json
+-rw-r--r--   0 ericof     (501) staff       (20)     4390 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/tests/_resources/multilingual_import/content/__metadata__.json
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-15 20:35:17.316987 plone.exportimport-1.0.0a4/tests/_resources/multilingual_import/content/b69412b6d0b0438d85b340c13a39fc8c/
+-rw-r--r--   0 ericof     (501) staff       (20)     1520 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/tests/_resources/multilingual_import/content/b69412b6d0b0438d85b340c13a39fc8c/data.json
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-15 20:35:17.317121 plone.exportimport-1.0.0a4/tests/_resources/multilingual_import/content/cecc6f7007344d3cbac68f1da4bd084a/
+-rw-r--r--   0 ericof     (501) staff       (20)     1502 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/tests/_resources/multilingual_import/content/cecc6f7007344d3cbac68f1da4bd084a/data.json
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-15 20:35:17.317282 plone.exportimport-1.0.0a4/tests/_resources/multilingual_import/content/ddb27456033d4b86a78f3ec783874b63/
+-rw-r--r--   0 ericof     (501) staff       (20)     1419 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/tests/_resources/multilingual_import/content/ddb27456033d4b86a78f3ec783874b63/data.json
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-15 20:35:17.317420 plone.exportimport-1.0.0a4/tests/_resources/multilingual_import/content/f40d3a236b464aa487b715adf3c0be92/
+-rw-r--r--   0 ericof     (501) staff       (20)     1511 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/tests/_resources/multilingual_import/content/f40d3a236b464aa487b715adf3c0be92/data.json
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-15 20:35:17.317557 plone.exportimport-1.0.0a4/tests/_resources/multilingual_import/content/f9767fbdadf041bd892010d21b290cb5/
+-rw-r--r--   0 ericof     (501) staff       (20)     1472 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/tests/_resources/multilingual_import/content/f9767fbdadf041bd892010d21b290cb5/data.json
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-15 20:35:17.317700 plone.exportimport-1.0.0a4/tests/_resources/multilingual_import/content/f98b033fa8ce46f487ca8923ddae7480/
+-rw-r--r--   0 ericof     (501) staff       (20)     1173 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/tests/_resources/multilingual_import/content/f98b033fa8ce46f487ca8923ddae7480/data.json
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-15 20:35:17.317839 plone.exportimport-1.0.0a4/tests/_resources/multilingual_import/content/fbcd98e2d1a741e2a90b8f0389203530/
+-rw-r--r--   0 ericof     (501) staff       (20)     1529 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/tests/_resources/multilingual_import/content/fbcd98e2d1a741e2a90b8f0389203530/data.json
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-15 20:35:17.318225 plone.exportimport-1.0.0a4/tests/_resources/multilingual_import/content/plone_site_root/
+-rw-r--r--   0 ericof     (501) staff       (20)      738 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/tests/_resources/multilingual_import/content/plone_site_root/data.json
+-rw-r--r--   0 ericof     (501) staff       (20)     4888 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/tests/_resources/multilingual_import/discussions.json
+-rw-r--r--   0 ericof     (501) staff       (20)     1877 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/tests/_resources/multilingual_import/principals.json
+-rw-r--r--   0 ericof     (501) staff       (20)       41 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/tests/_resources/multilingual_import/redirects.json
+-rw-r--r--   0 ericof     (501) staff       (20)      452 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/tests/_resources/multilingual_import/relations.json
+-rw-r--r--   0 ericof     (501) staff       (20)      928 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/tests/_resources/multilingual_import/translations.json
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-15 20:35:17.318349 plone.exportimport-1.0.0a4/tests/_resources/portlets_import/
+-rw-r--r--   0 ericof     (501) staff       (20)     1131 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/tests/_resources/portlets_import/portlets.json
+-rw-r--r--   0 ericof     (501) staff       (20)     7216 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/tests/conftest.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-15 20:35:17.319484 plone.exportimport-1.0.0a4/tests/exporters/
+-rw-r--r--   0 ericof     (501) staff       (20)      864 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/tests/exporters/conftest.py
+-rw-r--r--   0 ericof     (501) staff       (20)     3239 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/tests/exporters/test_exporters.py
+-rw-r--r--   0 ericof     (501) staff       (20)     2556 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/tests/exporters/test_exporters_content.py
+-rw-r--r--   0 ericof     (501) staff       (20)     1942 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/tests/exporters/test_exporters_discussions.py
+-rw-r--r--   0 ericof     (501) staff       (20)     1966 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/tests/exporters/test_exporters_portlets.py
+-rw-r--r--   0 ericof     (501) staff       (20)     1303 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/tests/exporters/test_exporters_principals.py
+-rw-r--r--   0 ericof     (501) staff       (20)     1294 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/tests/exporters/test_exporters_redirects.py
+-rw-r--r--   0 ericof     (501) staff       (20)     1861 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/tests/exporters/test_exporters_relations.py
+-rw-r--r--   0 ericof     (501) staff       (20)     1890 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/tests/exporters/test_exporters_translations.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-15 20:35:17.320681 plone.exportimport-1.0.0a4/tests/importers/
+-rw-r--r--   0 ericof     (501) staff       (20)      666 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/tests/importers/conftest.py
+-rw-r--r--   0 ericof     (501) staff       (20)     1533 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/tests/importers/test_importers.py
+-rw-r--r--   0 ericof     (501) staff       (20)     1118 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/tests/importers/test_importers_content.py
+-rw-r--r--   0 ericof     (501) staff       (20)     1437 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/tests/importers/test_importers_discussions.py
+-rw-r--r--   0 ericof     (501) staff       (20)     1815 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/tests/importers/test_importers_portlets.py
+-rw-r--r--   0 ericof     (501) staff       (20)     1434 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/tests/importers/test_importers_principals.py
+-rw-r--r--   0 ericof     (501) staff       (20)     1413 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/tests/importers/test_importers_redirects.py
+-rw-r--r--   0 ericof     (501) staff       (20)     1413 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/tests/importers/test_importers_relations.py
+-rw-r--r--   0 ericof     (501) staff       (20)     1446 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/tests/importers/test_importers_translations.py
+drwxr-xr-x   0 ericof     (501) staff       (20)        0 2024-05-15 20:35:17.322352 plone.exportimport-1.0.0a4/tests/utils/
+-rw-r--r--   0 ericof     (501) staff       (20)        0 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/tests/utils/conftest.py
+-rw-r--r--   0 ericof     (501) staff       (20)     3700 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/tests/utils/test_utils_content_core.py
+-rw-r--r--   0 ericof     (501) staff       (20)     1111 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/tests/utils/test_utils_content_export_helpers.py
+-rw-r--r--   0 ericof     (501) staff       (20)      860 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/tests/utils/test_utils_content_revisions.py
+-rw-r--r--   0 ericof     (501) staff       (20)     1304 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/tests/utils/test_utils_dates.py
+-rw-r--r--   0 ericof     (501) staff       (20)     3688 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/tests/utils/test_utils_discussions.py
+-rw-r--r--   0 ericof     (501) staff       (20)     1365 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/tests/utils/test_utils_path.py
+-rw-r--r--   0 ericof     (501) staff       (20)     1023 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/tests/utils/test_utils_principals_groups.py
+-rw-r--r--   0 ericof     (501) staff       (20)     1184 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/tests/utils/test_utils_principals_members.py
+-rw-r--r--   0 ericof     (501) staff       (20)     1252 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/tests/utils/test_utils_redirects.py
+-rw-r--r--   0 ericof     (501) staff       (20)     5384 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/tests/utils/test_utils_relations.py
+-rw-r--r--   0 ericof     (501) staff       (20)     5186 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/tests/utils/test_utils_translations.py
+-rw-r--r--   0 ericof     (501) staff       (20)     5050 2024-05-15 20:35:16.000000 plone.exportimport-1.0.0a4/tox.ini
```

### Comparing `plone.exportimport-1.0.0a3/.editorconfig` & `plone.exportimport-1.0.0a4/.editorconfig`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a3/.flake8` & `plone.exportimport-1.0.0a4/.flake8`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a3/.gitignore` & `plone.exportimport-1.0.0a4/.gitignore`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a3/.meta.toml` & `plone.exportimport-1.0.0a4/.meta.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Generated from:
 # https://github.com/plone/meta/tree/main/config/default
 # See the inline comments on how to expand/tweak this configuration file
 [meta]
 template = "default"
-commit-id = "fafcd936"
+commit-id = "a58656d9"
 
 [pyproject]
 codespell_skip = "*.min.js"
 codespell_ignores = "vew"
 dependencies_ignores = "['plone.volto', 'zestreleaser.towncrier', 'zest.releaser', 'pytest', 'pytest-cov', 'pytest-plone', 'plone.testing', 'plone.app.testing', 'plone.portlets', 'plone.app.portlets']"
 dependencies_mappings = [
     "Plone = ['Products.CMFPlone', 'Products.CMFCore', 'Products.GenericSetup']",
@@ -16,14 +16,15 @@
 [tox]
 test_runner = "pytest"
 test_path = "/tests"
 use_mxdev = true
 test_deps_additional = ""
 
 [github]
+py_versions = "[\"3.11\", \"3.10\"]"
 jobs = [
     "qa",
     "test",
     "coverage",
     "dependencies",
     "release_ready",
     ]
```

### Comparing `plone.exportimport-1.0.0a3/.pre-commit-config.yaml` & `plone.exportimport-1.0.0a4/.pre-commit-config.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 # See the inline comments on how to expand/tweak this configuration file
 ci:
     autofix_prs: false
     autoupdate_schedule: monthly
 
 repos:
 -   repo: https://github.com/asottile/pyupgrade
-    rev: v3.15.0
+    rev: v3.15.2
     hooks:
     -   id: pyupgrade
         args: [--py38-plus]
 -   repo: https://github.com/pycqa/isort
     rev: 5.13.2
     hooks:
     -   id: isort
 -   repo: https://github.com/psf/black
-    rev: 24.1.1
+    rev: 24.4.2
     hooks:
     -   id: black
 -   repo: https://github.com/collective/zpretty
     rev: 3.1.0
     hooks:
     -   id: zpretty
 
@@ -67,15 +67,15 @@
     -   id: pyroma
 -   repo: https://github.com/mgedmin/check-python-versions
     rev: "0.22.0"
     hooks:
     -   id: check-python-versions
         args: ['--only', 'setup.py,pyproject.toml']
 -   repo: https://github.com/collective/i18ndude
-    rev: "6.1.0"
+    rev: "6.2.0"
     hooks:
     -   id: i18ndude
 
 
 ##
 # Add extra configuration options in .meta.toml:
 #  [pre_commit]
```

### Comparing `plone.exportimport-1.0.0a3/CHANGES.md` & `plone.exportimport-1.0.0a4/CHANGES.md`

 * *Files 16% similar despite different names*

```diff
@@ -5,14 +5,34 @@
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 -->
 
 <!-- towncrier release notes start -->
 
+## 1.0.0a4 (2024-05-15)
+
+
+### New features:
+
+- Add pre_deserialize_hooks to content import [@pbauer] #22
+
+
+### Bug fixes:
+
+- Reindex members of relations in case that they contain preview_image_links
+  [sneridagh] #13
+- Avoid duplicating portlets registration during import [@ericof] #16
+
+
+### Internal:
+
+- Update plone/meta [@ericof] #20
+
+
 ## 1.0.0a3 (2024-05-02)
 
 
 ### Bug fixes:
 
 - Fix importer by issuing a transaction commit
   [sneridagh] #9
```

### Comparing `plone.exportimport-1.0.0a3/LICENSE` & `plone.exportimport-1.0.0a4/LICENSE`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a3/Makefile` & `plone.exportimport-1.0.0a4/Makefile`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a3/PKG-INFO` & `plone.exportimport-1.0.0a4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.exportimport
-Version: 1.0.0a3
+Version: 1.0.0a4
 Summary: Plone content export / import support
 Home-page: https://plone.org
 Author: Plone Foundation
 Author-email: releasemanager@plone.org
 License: GPL version 2
 Project-URL: Homepage, https://plone.org
 Project-URL: Documentation, https://6.docs.plone.org
@@ -57,14 +57,34 @@
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 -->
 
 <!-- towncrier release notes start -->
 
+## 1.0.0a4 (2024-05-15)
+
+
+### New features:
+
+- Add pre_deserialize_hooks to content import [@pbauer] #22
+
+
+### Bug fixes:
+
+- Reindex members of relations in case that they contain preview_image_links
+  [sneridagh] #13
+- Avoid duplicating portlets registration during import [@ericof] #16
+
+
+### Internal:
+
+- Update plone/meta [@ericof] #20
+
+
 ## 1.0.0a3 (2024-05-02)
 
 
 ### Bug fixes:
 
 - Fix importer by issuing a transaction commit
   [sneridagh] #9
```

### Comparing `plone.exportimport-1.0.0a3/README.md` & `plone.exportimport-1.0.0a4/README.md`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a3/docs/Makefile` & `plone.exportimport-1.0.0a4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a3/docs/_static/favicon.ico` & `plone.exportimport-1.0.0a4/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a3/docs/_static/logo.svg` & `plone.exportimport-1.0.0a4/docs/_static/logo.svg`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a3/docs/_static/styles.css` & `plone.exportimport-1.0.0a4/docs/_static/styles.css`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a3/docs/conf.py` & `plone.exportimport-1.0.0a4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a3/docs/develop.md` & `plone.exportimport-1.0.0a4/docs/develop.md`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a3/docs/features.md` & `plone.exportimport-1.0.0a4/docs/features.md`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a3/docs/index.md` & `plone.exportimport-1.0.0a4/docs/index.md`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a3/docs/installation.md` & `plone.exportimport-1.0.0a4/docs/installation.md`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a3/pyproject.toml` & `plone.exportimport-1.0.0a4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a3/requirements-docs.txt` & `plone.exportimport-1.0.0a4/requirements-docs.txt`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a3/setup.py` & `plone.exportimport-1.0.0a4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 long_description = f"""
 {Path("README.md").read_text()}\n
 {Path("CHANGES.md").read_text()}\n
 """
 
 setup(
     name="plone.exportimport",
-    version="1.0.0a3",
+    version="1.0.0a4",
     description="Plone content export / import support",
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Environment :: Web Environment",
         "Framework :: Plone",
```

### Comparing `plone.exportimport-1.0.0a3/src/plone/exportimport/cli/__init__.py` & `plone.exportimport-1.0.0a4/src/plone/exportimport/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a3/src/plone/exportimport/configure.zcml` & `plone.exportimport-1.0.0a4/src/plone/exportimport/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a3/src/plone/exportimport/deserializers/blob.py` & `plone.exportimport-1.0.0a4/src/plone/exportimport/deserializers/blob.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a3/src/plone/exportimport/deserializers/blocks.py` & `plone.exportimport-1.0.0a4/src/plone/exportimport/deserializers/blocks.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a3/src/plone/exportimport/exporters/__init__.py` & `plone.exportimport-1.0.0a4/src/plone/exportimport/exporters/__init__.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a3/src/plone/exportimport/exporters/base.py` & `plone.exportimport-1.0.0a4/src/plone/exportimport/exporters/base.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a3/src/plone/exportimport/exporters/configure.zcml` & `plone.exportimport-1.0.0a4/src/plone/exportimport/exporters/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a3/src/plone/exportimport/exporters/content.py` & `plone.exportimport-1.0.0a4/src/plone/exportimport/exporters/content.py`

 * *Files 1% similar despite different names*

```diff
@@ -95,15 +95,15 @@
                 data.update(additional)
 
         # Apply data hooks
         for func in self.data_hooks:
             logger.debug(
                 f"{config.logger_prefix} Running data hook {func.__name__} on payload"
             )
-            data = func(data, config)
+            data = func(data, obj, config)
 
         # Cleanup data
         for cleaner in content_utils.cleaners():
             logger.debug(
                 f"{config.logger_prefix} Running {cleaner.name} on serialized data"
             )
             data = cleaner.func(data, config)
```

### Comparing `plone.exportimport-1.0.0a3/src/plone/exportimport/exporters/discussions.py` & `plone.exportimport-1.0.0a4/src/plone/exportimport/exporters/discussions.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a3/src/plone/exportimport/exporters/portlets.py` & `plone.exportimport-1.0.0a4/src/plone/exportimport/exporters/portlets.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a3/src/plone/exportimport/exporters/principals.py` & `plone.exportimport-1.0.0a4/src/plone/exportimport/exporters/principals.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a3/src/plone/exportimport/exporters/redirects.py` & `plone.exportimport-1.0.0a4/src/plone/exportimport/exporters/redirects.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a3/src/plone/exportimport/exporters/relations.py` & `plone.exportimport-1.0.0a4/src/plone/exportimport/exporters/relations.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a3/src/plone/exportimport/exporters/translations.py` & `plone.exportimport-1.0.0a4/src/plone/exportimport/exporters/translations.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a3/src/plone/exportimport/importers/__init__.py` & `plone.exportimport-1.0.0a4/src/plone/exportimport/importers/__init__.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a3/src/plone/exportimport/importers/base.py` & `plone.exportimport-1.0.0a4/src/plone/exportimport/importers/base.py`

 * *Files 15% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 class BaseImporter:
     name: str
     base_path: Path
     site: PloneSite
     errors: list = None
     request: types.HTTPRequest = None
     data_hooks: List[Callable] = None
+    pre_deserialize_hooks: List[Callable] = None
     obj_hooks: List[Callable] = None
 
     def __init__(
         self,
         site: PloneSite,
     ):
         self.request = getRequest()
@@ -50,17 +51,21 @@
         """Deserialize objects."""
         return ""
 
     def import_data(
         self,
         base_path: Path,
         data_hooks: List[Callable] = None,
+        pre_deserialize_hooks: List[Callable] = None,
         obj_hooks: List[Callable] = None,
     ) -> str:
         """Import data into a Plone site."""
         if not base_path.exists():
             return f"{self.__class__.__name__}: Import path does not exist"
         self.base_path = base_path
-        self.data_hooks = data_hooks if data_hooks else []
-        self.obj_hooks = obj_hooks if obj_hooks else []
+        self.data_hooks = self.data_hooks or data_hooks or []
+        pre_deserialize_hooks = (
+            self.pre_deserialize_hooks or pre_deserialize_hooks or []
+        )
+        self.obj_hooks = self.obj_hooks or obj_hooks or []
         report = self.do_import()
         return report
```

### Comparing `plone.exportimport-1.0.0a3/src/plone/exportimport/importers/configure.zcml` & `plone.exportimport-1.0.0a4/src/plone/exportimport/importers/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a3/src/plone/exportimport/importers/content.py` & `plone.exportimport-1.0.0a4/src/plone/exportimport/importers/content.py`

 * *Files 8% similar despite different names*

```diff
@@ -69,14 +69,22 @@
                 f"{config.logger_prefix} Running data hook {func.__name__} on payload"
             )
             item = func(item, config)
 
         # Get or Create object instance
         new = content_utils.get_obj_instance(item, config)
 
+        # Apply pre_deserialize hooks
+        pre_deserialize_hooks = self.pre_deserialize_hooks or []
+        for func in pre_deserialize_hooks:
+            logger.debug(
+                f"{config.logger_prefix} Running pre_deserialize hook {func.__name__} on payload"
+            )
+            item, new = func(item, new)
+
         # Deserialize
         new = self.deserialize(data=item, obj=new, config=config)
 
         # Updaters
         for updater in content_utils.updaters():
             logger.debug(f"{config.logger_prefix} Running {updater.name} for {new}")
             new = updater.func(item, new)
@@ -122,19 +130,31 @@
             content_utils.recatalog_uids(modified, idxs=idxs)
         return f"{self.__class__.__name__}: Imported {len(objs)} objects"
 
     def import_data(
         self,
         base_path: Path,
         data_hooks: List[Callable] = None,
+        pre_deserialize_hooks: List[Callable] = None,
         obj_hooks: List[Callable] = None,
     ) -> str:
         """Import content into a site."""
         base_path = base_path / self.name
         self.request[settings.IMPORT_PATH_KEY] = base_path
         metadata_path = base_path / "__metadata__.json"
         metadata = self._read(metadata_path)
         if metadata is None:
             return f"{self.__class__.__name__}: No data to import"
         self.metadata = types.ExportImportMetadata(**self._read(metadata_path))
         self.languages = content_utils.get_portal_languages()
-        return super().import_data(base_path, data_hooks, obj_hooks)
+        self.start()
+        result = super().import_data(
+            base_path, data_hooks, pre_deserialize_hooks, obj_hooks
+        )
+        self.finish()
+        return result
+
+    def start(self):
+        """Hook to do something before import starts."""
+
+    def finish(self):
+        """Hook to do something after import finishes."""
```

### Comparing `plone.exportimport-1.0.0a3/src/plone/exportimport/importers/discussions.py` & `plone.exportimport-1.0.0a4/src/plone/exportimport/importers/discussions.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a3/src/plone/exportimport/importers/portlets.py` & `plone.exportimport-1.0.0a4/src/plone/exportimport/importers/portlets.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,8 +9,8 @@
     def do_import(self) -> dict:
         """Import portlets into a Plone Site."""
         data = self._read()
         if data is None:
             return f"{self.__class__.__name__}: No data to import"
         logger.debug(f"- Portlets: Read {len(data)} from {self.filepath}")
         count = utils.set_portlets(data)
-        return f"{self.__class__.__name__}: Imported {count} portlets"
+        return f"{self.__class__.__name__}: Imported {count} registrations"
```

### Comparing `plone.exportimport-1.0.0a3/src/plone/exportimport/importers/principals.py` & `plone.exportimport-1.0.0a4/src/plone/exportimport/importers/principals.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a3/src/plone/exportimport/importers/redirects.py` & `plone.exportimport-1.0.0a4/src/plone/exportimport/importers/redirects.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a3/src/plone/exportimport/importers/translations.py` & `plone.exportimport-1.0.0a4/src/plone/exportimport/importers/translations.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a3/src/plone/exportimport/interfaces.py` & `plone.exportimport-1.0.0a4/src/plone/exportimport/interfaces.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a3/src/plone/exportimport/serializers/blob.py` & `plone.exportimport-1.0.0a4/src/plone/exportimport/serializers/blob.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a3/src/plone/exportimport/serializers/blocks.py` & `plone.exportimport-1.0.0a4/src/plone/exportimport/serializers/blocks.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a3/src/plone/exportimport/testing/__init__.py` & `plone.exportimport-1.0.0a4/src/plone/exportimport/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a3/src/plone/exportimport/types.py` & `plone.exportimport-1.0.0a4/src/plone/exportimport/types.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a3/src/plone/exportimport/utils/cli.py` & `plone.exportimport-1.0.0a4/src/plone/exportimport/utils/cli.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a3/src/plone/exportimport/utils/content/__init__.py` & `plone.exportimport-1.0.0a4/src/plone/exportimport/utils/content/__init__.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a3/src/plone/exportimport/utils/content/blocks.py` & `plone.exportimport-1.0.0a4/src/plone/exportimport/utils/content/blocks.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a3/src/plone/exportimport/utils/content/core.py` & `plone.exportimport-1.0.0a4/src/plone/exportimport/utils/content/core.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a3/src/plone/exportimport/utils/content/export_helpers.py` & `plone.exportimport-1.0.0a4/src/plone/exportimport/utils/content/export_helpers.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a3/src/plone/exportimport/utils/content/import_helpers.py` & `plone.exportimport-1.0.0a4/src/plone/exportimport/utils/content/import_helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,15 +109,18 @@
     container = get_parent_from_item(item)
     # Check if we will update an item
     update_existing = item["id"] in container
     if update_existing:
         new = container[item["id"]]
         logger.debug(f"{config.logger_prefix} Will update {new}")
     else:
-        new = unrestricted_construct_instance(item["@type"], container, item["id"])
+        factory_kwargs = item.get("factory_kwargs", {})
+        new = unrestricted_construct_instance(
+            item["@type"], container, item["id"], **factory_kwargs
+        )
         logger.debug(f"{config.logger_prefix} Created {new}")
     return new
 
 
 def update_uid(item: dict, obj: DexterityContent) -> DexterityContent:
     """Set UID from data on the new object."""
     uuid = item.get("UID")
```

### Comparing `plone.exportimport-1.0.0a3/src/plone/exportimport/utils/content/revisions.py` & `plone.exportimport-1.0.0a4/src/plone/exportimport/utils/content/revisions.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a3/src/plone/exportimport/utils/dates.py` & `plone.exportimport-1.0.0a4/src/plone/exportimport/utils/dates.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a3/src/plone/exportimport/utils/discussions.py` & `plone.exportimport-1.0.0a4/src/plone/exportimport/utils/discussions.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a3/src/plone/exportimport/utils/path.py` & `plone.exportimport-1.0.0a4/src/plone/exportimport/utils/path.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a3/src/plone/exportimport/utils/portlets.py` & `plone.exportimport-1.0.0a4/src/plone/exportimport/utils/portlets.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,69 +1,90 @@
+from collections import defaultdict
 from plone import api
 from plone.app.portlets.interfaces import IPortletTypeInterface
 from plone.app.textfield.value import RichTextValue
+from plone.dexterity.content import DexterityContent
 from plone.exportimport import logger
 from plone.exportimport.settings import SITE_ROOT_UID
 from plone.portlets.constants import CONTENT_TYPE_CATEGORY
 from plone.portlets.constants import CONTEXT_CATEGORY
 from plone.portlets.constants import GROUP_CATEGORY
 from plone.portlets.constants import USER_CATEGORY
 from plone.portlets.interfaces import ILocalPortletAssignmentManager
 from plone.portlets.interfaces import IPortletAssignmentMapping
 from plone.portlets.interfaces import IPortletAssignmentSettings
 from plone.portlets.interfaces import IPortletManager
 from plone.restapi.interfaces import IFieldDeserializer
 from plone.restapi.serializer.converters import json_compatible
-from plone.uuid.interfaces import IUUID
+from typing import List
+from typing import Optional
+from typing import Union
 from z3c.relationfield import RelationValue
 from zope.component import getUtilitiesFor
 from zope.component import getUtility
 from zope.component import queryMultiAdapter
 from zope.component import queryUtility
 from zope.component.interfaces import IFactory
 from zope.container.interfaces import INameChooser
 from zope.globalrequest import getRequest
 from zope.interface import providedBy
 
 
-def get_portlets():
+def portlets_in_context(
+    context: DexterityContent, uid: Optional[str] = None
+) -> Union[dict, None]:
+    """Collect portlet registrations in a context."""
+    result = {}
+    uid = uid if uid else api.content.get_uuid(context, None)
+    if not uid:
+        return
+
+    portlets = export_local_portlets(context)
+    if portlets:
+        result["portlets"] = portlets
+    blacklist = export_portlets_blacklist(context)
+    if blacklist:
+        result["blacklist_status"] = blacklist
+    if result:
+        result.update(
+            {
+                "@id": context.absolute_url(),
+                "UID": uid,
+            }
+        )
+    return result
+
+
+def get_portlets() -> List[dict]:
+    """Return a list of all portlet assignments on the site."""
     results = []
     portal = api.portal.get()
     portal_uid = portal.UID()
 
     def collect_portlets(obj, path):
-        uid = IUUID(obj, None)
+        try:
+            uid = api.content.get_uuid(obj)
+        except TypeError:
+            uid = None
         if not uid:
             return
         if uid == portal_uid:
             uid = SITE_ROOT_UID
-
-        result = {}
-        portlets = export_local_portlets(obj)
-        if portlets:
-            result["portlets"] = portlets
-        blacklist = export_portlets_blacklist(obj)
-        if blacklist:
-            result["blacklist_status"] = blacklist
+        result = portlets_in_context(obj, uid)
         if result:
-            result.update(
-                {
-                    "@id": obj.absolute_url(),
-                    "UID": uid,
-                }
-            )
             results.append(result)
 
     portal.ZopeFindAndApply(portal, search_sub=True, apply_func=collect_portlets)
     collect_portlets(portal, portal_uid)
     return results
 
 
-def export_local_portlets(obj):
-    """Serialize portlets for one content object
+def export_local_portlets(obj: DexterityContent) -> dict:
+    """Serialize portlets for one content object.
+
     Code mostly taken from https://github.com/plone/plone.restapi/pull/669
     """
     portlets_schemata = {
         iface: name for name, iface in getUtilitiesFor(IPortletTypeInterface)
     }
     items = {}
     for manager_name, manager in getUtilitiesFor(IPortletManager):
@@ -103,15 +124,16 @@
                     "visible": settings.get("visible", True),
                     "assignment": values,
                 }
             )
     return items
 
 
-def export_portlets_blacklist(obj):
+def export_portlets_blacklist(obj: DexterityContent) -> List[dict]:
+    """Export portlets blacklist for one content object."""
     results = []
     for manager_name, manager in getUtilitiesFor(IPortletManager):
         assignable = queryMultiAdapter((obj, manager), ILocalPortletAssignmentManager)
         if assignable is None:
             continue
         for category in (
             USER_CATEGORY,
@@ -129,46 +151,73 @@
             if obj_results:
                 obj_results["manager"] = manager_name
                 obj_results["category"] = category
                 results.append(obj_results)
     return results
 
 
-def set_portlets(data):
+def _filter_portlets_registrations(base: dict, registrations: dict) -> dict:
+    """Filter new registration with the current registered portlets."""
+    results = defaultdict(dict)
+    key = "portlets"
+    current = base.get(key, {})
+    to_register = registrations.get(key, {})
+    for manager_id, assignments in to_register.items():
+        if manager_id not in current:
+            results[manager_id] = assignments
+            continue
+        manager = current[manager_id]
+        for assignment in assignments:
+            new_assignments = []
+            if assignment in manager:
+                continue
+            new_assignments.append(assignment)
+        if new_assignments:
+            results[manager_id] = new_assignments
+    return results
+
+
+def set_portlets(data: list) -> int:
+    """Set portlets for context."""
     results = 0
     for item in data:
-        obj = api.content.get(UID=item["UID"])
+        item_uid = item["UID"]
+        obj = api.content.get(UID=item_uid)
         if not obj:
-            if item["UID"] == SITE_ROOT_UID:
+            if item_uid == SITE_ROOT_UID:
                 obj = api.portal.get()
             else:
                 logger.info(
                     f"Could not find object to set portlet on UUID: {item['UID']}"
                 )
                 continue
-        registered_portlets = import_local_portlets(obj, item)
-        results += registered_portlets
+        existing_registrations = portlets_in_context(obj, item_uid)
+        new_registrations = _filter_portlets_registrations(existing_registrations, item)
+        if new_registrations:
+            registered_portlets = import_local_portlets(obj, item)
+            results += registered_portlets
     return results
 
 
-def import_local_portlets(obj, item):
-    """Register portlets from one object
+def import_local_portlets(obj: DexterityContent, item: dict) -> int:
+    """Register portlets from one object.
+
     Code adapted from plone.app.portlets.exportimport.portlets.PortletsXMLAdapter
     """
     site = api.portal.get()
     request = getRequest()
     results = 0
+
     for manager_name, portlets in item.get("portlets", {}).items():
         manager = queryUtility(IPortletManager, manager_name)
         if not manager:
             logger.info(f"No portlet manager {manager_name}")
             continue
         mapping = queryMultiAdapter((obj, manager), IPortletAssignmentMapping)
         namechooser = INameChooser(mapping)
-
         for portlet_data in portlets:
             # 1. Create the assignment
             assignment_data = portlet_data["assignment"]
             portlet_type = portlet_data["type"]
             portlet_factory = queryUtility(IFactory, name=portlet_type)
             if not portlet_factory:
                 logger.info(f"No factory for portlet {portlet_type}")
@@ -212,21 +261,22 @@
 
             logger.info(
                 f"Added {portlet_type} '{name}' to {manager_name} of {obj.absolute_url()}"
             )
             results += 1
 
     for blacklist_status in item.get("blacklist_status", []):
-        status = blacklist_status["status"]
+        status: bool = blacklist_status["status"].lower() == "block"
         manager_name = blacklist_status["manager"]
         category = blacklist_status["category"]
         manager = queryUtility(IPortletManager, manager_name)
         if not manager:
             logger.info(f"No portlet manager {manager_name}")
             continue
         assignable = queryMultiAdapter((obj, manager), ILocalPortletAssignmentManager)
-        if status.lower() == "block":
-            assignable.setBlacklistStatus(category, True)
-        elif status.lower() == "show":
-            assignable.setBlacklistStatus(category, False)
+        assignable.setBlacklistStatus(category, status)
+        logger.info(
+            f"Added blacklist entry {category} ({status}) to {manager_name} of {obj.absolute_url()}"
+        )
+        results += 1
 
     return results
```

### Comparing `plone.exportimport-1.0.0a3/src/plone/exportimport/utils/principals/groups.py` & `plone.exportimport-1.0.0a4/src/plone/exportimport/utils/principals/groups.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,14 +35,16 @@
             group = api.group.create(
                 groupname=groupid,
                 title=item["title"],
                 description=item["description"],
                 roles=item["roles"],
             )
             groups.append(group)
+        else:
+            group = api.group.get(groupname=groupid)
         # add all principals, even if they are not stored in plone (e.g. LDAP)
         for principal in principals:
             try:
                 api.group.add_user(group=group, username=principal)
             except api.exc.UserNotFoundError:
                 pass
     return groups
```

### Comparing `plone.exportimport-1.0.0a3/src/plone/exportimport/utils/principals/helpers.py` & `plone.exportimport-1.0.0a4/src/plone/exportimport/utils/principals/helpers.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a3/src/plone/exportimport/utils/principals/members.py` & `plone.exportimport-1.0.0a4/src/plone/exportimport/utils/principals/members.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a3/src/plone/exportimport/utils/redirects.py` & `plone.exportimport-1.0.0a4/src/plone/exportimport/utils/redirects.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a3/src/plone/exportimport/utils/relations.py` & `plone.exportimport-1.0.0a4/src/plone/exportimport/utils/relations.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a3/src/plone/exportimport/utils/translations.py` & `plone.exportimport-1.0.0a4/src/plone/exportimport/utils/translations.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a3/src/plone.exportimport.egg-info/PKG-INFO` & `plone.exportimport-1.0.0a4/src/plone.exportimport.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.exportimport
-Version: 1.0.0a3
+Version: 1.0.0a4
 Summary: Plone content export / import support
 Home-page: https://plone.org
 Author: Plone Foundation
 Author-email: releasemanager@plone.org
 License: GPL version 2
 Project-URL: Homepage, https://plone.org
 Project-URL: Documentation, https://6.docs.plone.org
@@ -57,14 +57,34 @@
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 -->
 
 <!-- towncrier release notes start -->
 
+## 1.0.0a4 (2024-05-15)
+
+
+### New features:
+
+- Add pre_deserialize_hooks to content import [@pbauer] #22
+
+
+### Bug fixes:
+
+- Reindex members of relations in case that they contain preview_image_links
+  [sneridagh] #13
+- Avoid duplicating portlets registration during import [@ericof] #16
+
+
+### Internal:
+
+- Update plone/meta [@ericof] #20
+
+
 ## 1.0.0a3 (2024-05-02)
 
 
 ### Bug fixes:
 
 - Fix importer by issuing a transaction commit
   [sneridagh] #9
```

### Comparing `plone.exportimport-1.0.0a3/src/plone.exportimport.egg-info/SOURCES.txt` & `plone.exportimport-1.0.0a4/src/plone.exportimport.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -67,14 +67,15 @@
 src/plone/exportimport/importers/redirects.py
 src/plone/exportimport/importers/relations.py
 src/plone/exportimport/importers/translations.py
 src/plone/exportimport/serializers/__init__.py
 src/plone/exportimport/serializers/blob.py
 src/plone/exportimport/serializers/blocks.py
 src/plone/exportimport/serializers/configure.zcml
+src/plone/exportimport/serializers/fields.py
 src/plone/exportimport/testing/__init__.py
 src/plone/exportimport/utils/__init__.py
 src/plone/exportimport/utils/cli.py
 src/plone/exportimport/utils/dates.py
 src/plone/exportimport/utils/discussions.py
 src/plone/exportimport/utils/path.py
 src/plone/exportimport/utils/portlets.py
@@ -134,14 +135,15 @@
 tests/_resources/multilingual_import/content/cecc6f7007344d3cbac68f1da4bd084a/data.json
 tests/_resources/multilingual_import/content/ddb27456033d4b86a78f3ec783874b63/data.json
 tests/_resources/multilingual_import/content/f40d3a236b464aa487b715adf3c0be92/data.json
 tests/_resources/multilingual_import/content/f9767fbdadf041bd892010d21b290cb5/data.json
 tests/_resources/multilingual_import/content/f98b033fa8ce46f487ca8923ddae7480/data.json
 tests/_resources/multilingual_import/content/fbcd98e2d1a741e2a90b8f0389203530/data.json
 tests/_resources/multilingual_import/content/plone_site_root/data.json
+tests/_resources/portlets_import/portlets.json
 tests/exporters/conftest.py
 tests/exporters/test_exporters.py
 tests/exporters/test_exporters_content.py
 tests/exporters/test_exporters_discussions.py
 tests/exporters/test_exporters_portlets.py
 tests/exporters/test_exporters_principals.py
 tests/exporters/test_exporters_redirects.py
```

### Comparing `plone.exportimport-1.0.0a3/src/plone.exportimport.egg-info/requires.txt` & `plone.exportimport-1.0.0a4/src/plone.exportimport.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a3/tests/_resources/base_import/content/35661c9bb5be42c68f665aa1ed291418/data.json` & `plone.exportimport-1.0.0a4/tests/_resources/base_import/content/35661c9bb5be42c68f665aa1ed291418/data.json`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a3/tests/_resources/base_import/content/3e0dd7c4b2714eafa1d6fc6a1493f953/data.json` & `plone.exportimport-1.0.0a4/tests/_resources/base_import/content/3e0dd7c4b2714eafa1d6fc6a1493f953/data.json`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a3/tests/_resources/base_import/content/3e0dd7c4b2714eafa1d6fc6a1493f953/file/plone.pdf` & `plone.exportimport-1.0.0a4/tests/_resources/base_import/content/3e0dd7c4b2714eafa1d6fc6a1493f953/file/plone.pdf`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a3/tests/_resources/base_import/content/45b0b46f17104a7b8fa7bb94d3dd5bd9/data.json` & `plone.exportimport-1.0.0a4/tests/_resources/base_import/content/45b0b46f17104a7b8fa7bb94d3dd5bd9/data.json`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a3/tests/_resources/base_import/content/5d77cd5686184ec49ab077017b1fbc3a/data.json` & `plone.exportimport-1.0.0a4/tests/_resources/base_import/content/5d77cd5686184ec49ab077017b1fbc3a/data.json`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a3/tests/_resources/base_import/content/70844f7bec1843b8ab2796c972c9ebfe/data.json` & `plone.exportimport-1.0.0a4/tests/_resources/base_import/content/70844f7bec1843b8ab2796c972c9ebfe/data.json`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a3/tests/_resources/base_import/content/7c1393f615c4447c80db0d784390c5b7/data.json` & `plone.exportimport-1.0.0a4/tests/_resources/base_import/content/7c1393f615c4447c80db0d784390c5b7/data.json`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a3/tests/_resources/base_import/content/7c1393f615c4447c80db0d784390c5b7/image/brazil-coins.png` & `plone.exportimport-1.0.0a4/tests/_resources/base_import/content/7c1393f615c4447c80db0d784390c5b7/image/brazil-coins.png`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a3/tests/_resources/base_import/content/90b11c863598495ba699b22ca76b1041/data.json` & `plone.exportimport-1.0.0a4/tests/_resources/base_import/content/90b11c863598495ba699b22ca76b1041/data.json`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a3/tests/_resources/base_import/content/90b11c863598495ba699b22ca76b1041/image/2025.png` & `plone.exportimport-1.0.0a4/tests/_resources/base_import/content/90b11c863598495ba699b22ca76b1041/image/2025.png`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a3/tests/_resources/base_import/content/__metadata__.json` & `plone.exportimport-1.0.0a4/tests/_resources/base_import/content/__metadata__.json`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a3/tests/_resources/base_import/content/e7359727ace64e609b79c4091c38822a/data.json` & `plone.exportimport-1.0.0a4/tests/_resources/base_import/content/e7359727ace64e609b79c4091c38822a/data.json`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a3/tests/_resources/base_import/content/plone_site_root/data.json` & `plone.exportimport-1.0.0a4/tests/_resources/base_import/content/plone_site_root/data.json`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a3/tests/_resources/base_import/discussions.json` & `plone.exportimport-1.0.0a4/tests/_resources/base_import/discussions.json`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a3/tests/_resources/base_import/portlets.json` & `plone.exportimport-1.0.0a4/tests/_resources/portlets_import/portlets.json`

 * *Files 19% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6560570987654322%*

 * *Differences: {'0': "{'portlets': {'plone.leftcolumn': {1: {'assignment': {'name': 'My Other Navigation', "*

 * *      "'no_icons': True}}, insert: [(0, OrderedDict([('assignment', OrderedDict([('bottomLevel', "*

 * *      "0), ('currentFolderOnly', False), ('includeTop', False), ('name', 'My Navigation'), "*

 * *      "('no_icons', True), ('no_thumbs', False), ('root_uid', None), ('thumb_scale', None), "*

 * *      "('topLevel', 1)])), ('type', 'portlets.Navigation'), ('visible', True)]))]}, delete: "*

 * *      "['plone.footerportlets', 'plone […]*

```diff
@@ -1,67 +1,47 @@
 [
     {
         "@id": "http://localhost:8080/Plone",
         "UID": "plone_site_root",
+        "blacklist_status": [
+            {
+                "category": "context",
+                "manager": "plone.rightcolumn",
+                "status": "block"
+            }
+        ],
         "portlets": {
-            "plone.footerportlets": [
-                {
-                    "assignment": {
-                        "macro": "",
-                        "template": "@@footer"
-                    },
-                    "type": "portlets.Classic",
-                    "visible": true
-                },
-                {
-                    "assignment": {
-                        "category": "site_actions",
-                        "default_icon": "action_icon.png",
-                        "ptitle": "site_actions",
-                        "show_icons": false,
-                        "show_title": false
-                    },
-                    "type": "portlets.Actions",
-                    "visible": true
-                },
-                {
-                    "assignment": {
-                        "macro": "",
-                        "template": "colophon"
-                    },
-                    "type": "portlets.Classic",
-                    "visible": true
-                }
-            ],
             "plone.leftcolumn": [
                 {
                     "assignment": {
                         "bottomLevel": 0,
                         "currentFolderOnly": false,
                         "includeTop": false,
-                        "name": "",
-                        "no_icons": false,
+                        "name": "My Navigation",
+                        "no_icons": true,
                         "no_thumbs": false,
                         "root_uid": null,
                         "thumb_scale": null,
                         "topLevel": 1
                     },
                     "type": "portlets.Navigation",
                     "visible": true
-                }
-            ],
-            "plone.rightcolumn": [
+                },
                 {
                     "assignment": {
-                        "count": 5,
+                        "bottomLevel": 0,
+                        "currentFolderOnly": false,
+                        "includeTop": false,
+                        "name": "My Other Navigation",
+                        "no_icons": true,
                         "no_thumbs": false,
-                        "search_base_uid": null,
-                        "state": null,
-                        "thumb_scale": null
+                        "root_uid": null,
+                        "thumb_scale": null,
+                        "topLevel": 1
                     },
-                    "type": "portlets.Events",
+                    "type": "portlets.Navigation",
                     "visible": true
                 }
             ]
         }
     }
 ]
```

### Comparing `plone.exportimport-1.0.0a3/tests/_resources/base_import/principals.json` & `plone.exportimport-1.0.0a4/tests/_resources/base_import/principals.json`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a3/tests/_resources/multilingual_import/content/01fbca4cccd448d880959ba93aa8176e/data.json` & `plone.exportimport-1.0.0a4/tests/_resources/multilingual_import/content/01fbca4cccd448d880959ba93aa8176e/data.json`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a3/tests/_resources/multilingual_import/content/1cbf4ae73c74459485d3fd6cb9714e43/data.json` & `plone.exportimport-1.0.0a4/tests/_resources/multilingual_import/content/1cbf4ae73c74459485d3fd6cb9714e43/data.json`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a3/tests/_resources/multilingual_import/content/20737423549c43a88488242ec629e087/data.json` & `plone.exportimport-1.0.0a4/tests/_resources/multilingual_import/content/20737423549c43a88488242ec629e087/data.json`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a3/tests/_resources/multilingual_import/content/2be023c76b3e4e0aa9908c70f19a14df/data.json` & `plone.exportimport-1.0.0a4/tests/_resources/multilingual_import/content/2be023c76b3e4e0aa9908c70f19a14df/data.json`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a3/tests/_resources/multilingual_import/content/2d099ac593344be7aaf2e4aafbba9065/data.json` & `plone.exportimport-1.0.0a4/tests/_resources/multilingual_import/content/2d099ac593344be7aaf2e4aafbba9065/data.json`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a3/tests/_resources/multilingual_import/content/3e3d4bf2cac4482f9c03e34b52092f02/data.json` & `plone.exportimport-1.0.0a4/tests/_resources/multilingual_import/content/3e3d4bf2cac4482f9c03e34b52092f02/data.json`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a3/tests/_resources/multilingual_import/content/496cbe4f17904d6bb9321b23f91dc8cc/data.json` & `plone.exportimport-1.0.0a4/tests/_resources/multilingual_import/content/496cbe4f17904d6bb9321b23f91dc8cc/data.json`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a3/tests/_resources/multilingual_import/content/59e06b23024a4c4b9d93672fe440e019/data.json` & `plone.exportimport-1.0.0a4/tests/_resources/multilingual_import/content/59e06b23024a4c4b9d93672fe440e019/data.json`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a3/tests/_resources/multilingual_import/content/5ffe1d0c89c745eaab26df0e71ac82de/data.json` & `plone.exportimport-1.0.0a4/tests/_resources/multilingual_import/content/5ffe1d0c89c745eaab26df0e71ac82de/data.json`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a3/tests/_resources/multilingual_import/content/6d8a2b38d445462aa19f604b0801a13c/data.json` & `plone.exportimport-1.0.0a4/tests/_resources/multilingual_import/content/6d8a2b38d445462aa19f604b0801a13c/data.json`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a3/tests/_resources/multilingual_import/content/85a60611c2744e7abe53e3f356df236a/data.json` & `plone.exportimport-1.0.0a4/tests/_resources/multilingual_import/content/85a60611c2744e7abe53e3f356df236a/data.json`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a3/tests/_resources/multilingual_import/content/__metadata__.json` & `plone.exportimport-1.0.0a4/tests/_resources/multilingual_import/content/__metadata__.json`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a3/tests/_resources/multilingual_import/content/b69412b6d0b0438d85b340c13a39fc8c/data.json` & `plone.exportimport-1.0.0a4/tests/_resources/multilingual_import/content/b69412b6d0b0438d85b340c13a39fc8c/data.json`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a3/tests/_resources/multilingual_import/content/cecc6f7007344d3cbac68f1da4bd084a/data.json` & `plone.exportimport-1.0.0a4/tests/_resources/multilingual_import/content/cecc6f7007344d3cbac68f1da4bd084a/data.json`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a3/tests/_resources/multilingual_import/content/ddb27456033d4b86a78f3ec783874b63/data.json` & `plone.exportimport-1.0.0a4/tests/_resources/multilingual_import/content/ddb27456033d4b86a78f3ec783874b63/data.json`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a3/tests/_resources/multilingual_import/content/f40d3a236b464aa487b715adf3c0be92/data.json` & `plone.exportimport-1.0.0a4/tests/_resources/multilingual_import/content/f40d3a236b464aa487b715adf3c0be92/data.json`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a3/tests/_resources/multilingual_import/content/f9767fbdadf041bd892010d21b290cb5/data.json` & `plone.exportimport-1.0.0a4/tests/_resources/multilingual_import/content/f9767fbdadf041bd892010d21b290cb5/data.json`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a3/tests/_resources/multilingual_import/content/f98b033fa8ce46f487ca8923ddae7480/data.json` & `plone.exportimport-1.0.0a4/tests/_resources/multilingual_import/content/f98b033fa8ce46f487ca8923ddae7480/data.json`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a3/tests/_resources/multilingual_import/content/fbcd98e2d1a741e2a90b8f0389203530/data.json` & `plone.exportimport-1.0.0a4/tests/_resources/multilingual_import/content/fbcd98e2d1a741e2a90b8f0389203530/data.json`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a3/tests/_resources/multilingual_import/content/plone_site_root/data.json` & `plone.exportimport-1.0.0a4/tests/_resources/multilingual_import/content/plone_site_root/data.json`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a3/tests/_resources/multilingual_import/discussions.json` & `plone.exportimport-1.0.0a4/tests/_resources/multilingual_import/discussions.json`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a3/tests/_resources/multilingual_import/principals.json` & `plone.exportimport-1.0.0a4/tests/_resources/multilingual_import/principals.json`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a3/tests/_resources/multilingual_import/translations.json` & `plone.exportimport-1.0.0a4/tests/_resources/multilingual_import/translations.json`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a3/tests/conftest.py` & `plone.exportimport-1.0.0a4/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,20 @@
 @pytest.fixture()
 def base_import_path():
     """Base content import Path."""
     return Path(__file__).parent / "_resources" / "base_import"
 
 
 @pytest.fixture()
+def portlets_import_path():
+    """Portlets import Path."""
+    return Path(__file__).parent / "_resources" / "portlets_import"
+
+
+@pytest.fixture()
 def multilingual_import_path():
     """Multilingual content import path."""
     return Path(__file__).parent / "_resources" / "multilingual_import"
 
 
 @pytest.fixture()
 def empty_import_path():
```

### Comparing `plone.exportimport-1.0.0a3/tests/exporters/conftest.py` & `plone.exportimport-1.0.0a4/tests/exporters/conftest.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a3/tests/exporters/test_exporters.py` & `plone.exportimport-1.0.0a4/tests/exporters/test_exporters.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a3/tests/exporters/test_exporters_content.py` & `plone.exportimport-1.0.0a4/tests/exporters/test_exporters_content.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a3/tests/exporters/test_exporters_discussions.py` & `plone.exportimport-1.0.0a4/tests/exporters/test_exporters_discussions.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a3/tests/exporters/test_exporters_portlets.py` & `plone.exportimport-1.0.0a4/tests/exporters/test_exporters_portlets.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a3/tests/exporters/test_exporters_principals.py` & `plone.exportimport-1.0.0a4/tests/exporters/test_exporters_principals.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a3/tests/exporters/test_exporters_redirects.py` & `plone.exportimport-1.0.0a4/tests/exporters/test_exporters_redirects.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a3/tests/exporters/test_exporters_relations.py` & `plone.exportimport-1.0.0a4/tests/exporters/test_exporters_relations.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a3/tests/exporters/test_exporters_translations.py` & `plone.exportimport-1.0.0a4/tests/exporters/test_exporters_translations.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a3/tests/importers/conftest.py` & `plone.exportimport-1.0.0a4/tests/importers/conftest.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a3/tests/importers/test_importers.py` & `plone.exportimport-1.0.0a4/tests/importers/test_importers.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a3/tests/importers/test_importers_content.py` & `plone.exportimport-1.0.0a4/tests/importers/test_importers_content.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a3/tests/importers/test_importers_discussions.py` & `plone.exportimport-1.0.0a4/tests/importers/test_importers_discussions.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a3/tests/importers/test_importers_portlets.py` & `plone.exportimport-1.0.0a4/tests/importers/test_importers_portlets.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,19 +21,25 @@
 
     def test_adapter_is_registered(self):
         adapter = getAdapter(
             self.portal, interfaces.INamedImporter, "plone.importer.portlets"
         )
         assert isinstance(adapter, portlets.PortletsImporter)
 
-    def test_output_is_str(self, base_import_path):
+    def test_only_default_portlets_to_import(self, base_import_path):
         importer = self.importer
         result = importer.import_data(base_path=base_import_path)
         assert isinstance(result, str)
-        assert result == "PortletsImporter: Imported 5 portlets"
+        assert result == "PortletsImporter: Imported 0 registrations"
+
+    def test_additional_portlets(self, portlets_import_path):
+        importer = self.importer
+        result = importer.import_data(base_path=portlets_import_path)
+        assert isinstance(result, str)
+        assert result == "PortletsImporter: Imported 3 registrations"
 
     def test_empty_import_path(self, empty_import_path):
         importer = self.importer
         result = importer.import_data(base_path=empty_import_path)
         assert isinstance(result, str)
         assert result == "PortletsImporter: No data to import"
```

### Comparing `plone.exportimport-1.0.0a3/tests/importers/test_importers_principals.py` & `plone.exportimport-1.0.0a4/tests/importers/test_importers_principals.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a3/tests/importers/test_importers_redirects.py` & `plone.exportimport-1.0.0a4/tests/importers/test_importers_redirects.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a3/tests/importers/test_importers_relations.py` & `plone.exportimport-1.0.0a4/tests/importers/test_importers_relations.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a3/tests/importers/test_importers_translations.py` & `plone.exportimport-1.0.0a4/tests/importers/test_importers_translations.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a3/tests/utils/test_utils_content_core.py` & `plone.exportimport-1.0.0a4/tests/utils/test_utils_content_core.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a3/tests/utils/test_utils_content_export_helpers.py` & `plone.exportimport-1.0.0a4/tests/utils/test_utils_content_export_helpers.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a3/tests/utils/test_utils_content_revisions.py` & `plone.exportimport-1.0.0a4/tests/utils/test_utils_content_revisions.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a3/tests/utils/test_utils_dates.py` & `plone.exportimport-1.0.0a4/tests/utils/test_utils_dates.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a3/tests/utils/test_utils_discussions.py` & `plone.exportimport-1.0.0a4/tests/utils/test_utils_discussions.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a3/tests/utils/test_utils_path.py` & `plone.exportimport-1.0.0a4/tests/utils/test_utils_path.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a3/tests/utils/test_utils_principals_groups.py` & `plone.exportimport-1.0.0a4/tests/utils/test_utils_principals_groups.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a3/tests/utils/test_utils_principals_members.py` & `plone.exportimport-1.0.0a4/tests/utils/test_utils_principals_members.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a3/tests/utils/test_utils_redirects.py` & `plone.exportimport-1.0.0a4/tests/utils/test_utils_redirects.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a3/tests/utils/test_utils_relations.py` & `plone.exportimport-1.0.0a4/tests/utils/test_utils_relations.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a3/tests/utils/test_utils_translations.py` & `plone.exportimport-1.0.0a4/tests/utils/test_utils_translations.py`

 * *Files identical despite different names*

### Comparing `plone.exportimport-1.0.0a3/tox.ini` & `plone.exportimport-1.0.0a4/tox.ini`

 * *Files 2% similar despite different names*

```diff
@@ -182,14 +182,17 @@
     python -m build --sdist
     twine check dist/*
 
 [testenv:circular]
 description = ensure there are no cyclic dependencies
 use_develop = true
 skip_install = false
+# Here we must always constrain the package deps to what is already installed,
+# otherwise we simply get the latest from PyPI, which may not work.
+constrain_package_deps = true
 set_env =
 
 ##
 # Specify extra test environment variables in .meta.toml:
 #  [tox]
 #  test_environment_variables = """
 #      PIP_EXTRA_INDEX_URL=https://my-pypi.my-server.com/
```

