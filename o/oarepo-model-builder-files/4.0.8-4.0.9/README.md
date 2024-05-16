# Comparing `tmp/oarepo-model-builder-files-4.0.8.tar.gz` & `tmp/oarepo-model-builder-files-4.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oarepo-model-builder-files-4.0.8.tar", last modified: Tue Oct 24 08:48:52 2023, max compression
+gzip compressed data, was "oarepo-model-builder-files-4.0.9.tar", last modified: Sun Oct 29 20:49:45 2023, max compression
```

## Comparing `oarepo-model-builder-files-4.0.8.tar` & `oarepo-model-builder-files-4.0.9.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 08:48:52.045152 oarepo-model-builder-files-4.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2023-10-24 08:42:08.000000 oarepo-model-builder-files-4.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2023-10-24 08:48:52.045152 oarepo-model-builder-files-4.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1694 2023-10-24 08:42:08.000000 oarepo-model-builder-files-4.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 08:48:52.033152 oarepo-model-builder-files-4.0.8/oarepo_model_builder_files/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-24 08:42:08.000000 oarepo-model-builder-files-4.0.8/oarepo_model_builder_files/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 08:48:52.033152 oarepo-model-builder-files-4.0.8/oarepo_model_builder_files/builders/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-24 08:42:08.000000 oarepo-model-builder-files-4.0.8/oarepo_model_builder_files/builders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      606 2023-10-24 08:42:08.000000 oarepo-model-builder-files-4.0.8/oarepo_model_builder_files/builders/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 08:48:52.033152 oarepo-model-builder-files-4.0.8/oarepo_model_builder_files/builders/invenio/
--rw-r--r--   0 runner    (1001) docker     (127)      592 2023-10-24 08:42:08.000000 oarepo-model-builder-files-4.0.8/oarepo_model_builder_files/builders/invenio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      200 2023-10-24 08:42:08.000000 oarepo-model-builder-files-4.0.8/oarepo_model_builder_files/builders/invenio/invenio_files_record.py
--rw-r--r--   0 runner    (1001) docker     (127)      235 2023-10-24 08:42:08.000000 oarepo-model-builder-files-4.0.8/oarepo_model_builder_files/builders/invenio/invenio_files_record_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)      226 2023-10-24 08:42:08.000000 oarepo-model-builder-files-4.0.8/oarepo_model_builder_files/builders/invenio/invenio_files_record_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)      239 2023-10-24 08:42:08.000000 oarepo-model-builder-files-4.0.8/oarepo_model_builder_files/builders/invenio/invenio_files_record_service_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 08:48:52.037152 oarepo-model-builder-files-4.0.8/oarepo_model_builder_files/builders/invenio/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      143 2023-10-24 08:42:08.000000 oarepo-model-builder-files-4.0.8/oarepo_model_builder_files/builders/invenio/templates/invenio_files_record.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)      233 2023-10-24 08:42:08.000000 oarepo-model-builder-files-4.0.8/oarepo_model_builder_files/builders/invenio/templates/invenio_files_record_metadata.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)      671 2023-10-24 08:42:08.000000 oarepo-model-builder-files-4.0.8/oarepo_model_builder_files/builders/invenio/templates/invenio_files_record_permissions.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)      260 2023-10-24 08:42:08.000000 oarepo-model-builder-files-4.0.8/oarepo_model_builder_files/builders/invenio/templates/invenio_files_record_service_config.py.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 08:48:52.037152 oarepo-model-builder-files-4.0.8/oarepo_model_builder_files/builders/invenio_parent/
--rw-r--r--   0 runner    (1001) docker     (127)      348 2023-10-24 08:42:08.000000 oarepo-model-builder-files-4.0.8/oarepo_model_builder_files/builders/invenio_parent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      258 2023-10-24 08:42:08.000000 oarepo-model-builder-files-4.0.8/oarepo_model_builder_files/builders/invenio_parent/invenio_files_parent_record.py
--rw-r--r--   0 runner    (1001) docker     (127)      293 2023-10-24 08:42:08.000000 oarepo-model-builder-files-4.0.8/oarepo_model_builder_files/builders/invenio_parent/invenio_files_parent_record_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)      263 2023-10-24 08:42:08.000000 oarepo-model-builder-files-4.0.8/oarepo_model_builder_files/builders/invenio_parent/invenio_files_parent_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 08:48:52.037152 oarepo-model-builder-files-4.0.8/oarepo_model_builder_files/builders/invenio_parent/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      653 2023-10-24 08:42:08.000000 oarepo-model-builder-files-4.0.8/oarepo_model_builder_files/builders/invenio_parent/templates/invenio_files_record.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)      240 2023-10-24 08:42:08.000000 oarepo-model-builder-files-4.0.8/oarepo_model_builder_files/builders/invenio_parent/templates/invenio_files_record_metadata.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)     1721 2023-10-24 08:42:08.000000 oarepo-model-builder-files-4.0.8/oarepo_model_builder_files/builders/invenio_parent/templates/invenio_files_schema.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)      522 2023-10-24 08:42:08.000000 oarepo-model-builder-files-4.0.8/oarepo_model_builder_files/builders/parent_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 08:48:52.037152 oarepo-model-builder-files-4.0.8/oarepo_model_builder_files/builders/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      252 2023-10-24 08:42:08.000000 oarepo-model-builder-files-4.0.8/oarepo_model_builder_files/builders/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      338 2023-10-24 08:42:08.000000 oarepo-model-builder-files-4.0.8/oarepo_model_builder_files/builders/tests/invenio_files_conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      351 2023-10-24 08:42:08.000000 oarepo-model-builder-files-4.0.8/oarepo_model_builder_files/builders/tests/invenio_files_conftest_files.py
--rw-r--r--   0 runner    (1001) docker     (127)      746 2023-10-24 08:42:08.000000 oarepo-model-builder-files-4.0.8/oarepo_model_builder_files/builders/tests/invenio_files_test_file_resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 08:48:52.037152 oarepo-model-builder-files-4.0.8/oarepo_model_builder_files/builders/tests/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      621 2023-10-24 08:42:08.000000 oarepo-model-builder-files-4.0.8/oarepo_model_builder_files/builders/tests/templates/invenio_files_conftest.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)      775 2023-10-24 08:42:08.000000 oarepo-model-builder-files-4.0.8/oarepo_model_builder_files/builders/tests/templates/invenio_files_conftest_files.py.jinja2
--rw-r--r--   0 runner    (1001) docker     (127)    12349 2023-10-24 08:42:08.000000 oarepo-model-builder-files-4.0.8/oarepo_model_builder_files/builders/tests/templates/invenio_files_test_file_resources.py.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 08:48:52.041152 oarepo-model-builder-files-4.0.8/oarepo_model_builder_files/builtin_models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-24 08:42:08.000000 oarepo-model-builder-files-4.0.8/oarepo_model_builder_files/builtin_models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2023-10-24 08:42:08.000000 oarepo-model-builder-files-4.0.8/oarepo_model_builder_files/builtin_models/invenio_files.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 08:48:52.041152 oarepo-model-builder-files-4.0.8/oarepo_model_builder_files/datatypes/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2023-10-24 08:42:08.000000 oarepo-model-builder-files-4.0.8/oarepo_model_builder_files/datatypes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 08:48:52.041152 oarepo-model-builder-files-4.0.8/oarepo_model_builder_files/datatypes/components/
--rw-r--r--   0 runner    (1001) docker     (127)      853 2023-10-24 08:42:08.000000 oarepo-model-builder-files-4.0.8/oarepo_model_builder_files/datatypes/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4630 2023-10-24 08:42:08.000000 oarepo-model-builder-files-4.0.8/oarepo_model_builder_files/datatypes/components/file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 08:48:52.045152 oarepo-model-builder-files-4.0.8/oarepo_model_builder_files/datatypes/components/files_model/
--rw-r--r--   0 runner    (1001) docker     (127)     1403 2023-10-24 08:42:08.000000 oarepo-model-builder-files-4.0.8/oarepo_model_builder_files/datatypes/components/files_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1183 2023-10-24 08:42:08.000000 oarepo-model-builder-files-4.0.8/oarepo_model_builder_files/datatypes/components/files_model/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     1213 2023-10-24 08:42:08.000000 oarepo-model-builder-files-4.0.8/oarepo_model_builder_files/datatypes/components/files_model/ext_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     2084 2023-10-24 08:42:08.000000 oarepo-model-builder-files-4.0.8/oarepo_model_builder_files/datatypes/components/files_model/files_field.py
--rw-r--r--   0 runner    (1001) docker     (127)      918 2023-10-24 08:42:08.000000 oarepo-model-builder-files-4.0.8/oarepo_model_builder_files/datatypes/components/files_model/permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)      923 2023-10-24 08:42:08.000000 oarepo-model-builder-files-4.0.8/oarepo_model_builder_files/datatypes/components/files_model/pid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2023-10-24 08:42:08.000000 oarepo-model-builder-files-4.0.8/oarepo_model_builder_files/datatypes/components/files_model/record.py
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2023-10-24 08:42:08.000000 oarepo-model-builder-files-4.0.8/oarepo_model_builder_files/datatypes/components/files_model/record_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2023-10-24 08:42:08.000000 oarepo-model-builder-files-4.0.8/oarepo_model_builder_files/datatypes/components/files_model/resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     1251 2023-10-24 08:42:08.000000 oarepo-model-builder-files-4.0.8/oarepo_model_builder_files/datatypes/components/files_model/service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2023-10-24 08:42:08.000000 oarepo-model-builder-files-4.0.8/oarepo_model_builder_files/datatypes/components/files_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     1647 2023-10-24 08:42:08.000000 oarepo-model-builder-files-4.0.8/oarepo_model_builder_files/datatypes/components/parent_record.py
--rw-r--r--   0 runner    (1001) docker     (127)      268 2023-10-24 08:42:08.000000 oarepo-model-builder-files-4.0.8/oarepo_model_builder_files/datatypes/components/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      469 2023-10-24 08:42:08.000000 oarepo-model-builder-files-4.0.8/oarepo_model_builder_files/datatypes/file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 08:48:52.045152 oarepo-model-builder-files-4.0.8/oarepo_model_builder_files/profiles/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-24 08:42:08.000000 oarepo-model-builder-files-4.0.8/oarepo_model_builder_files/profiles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2023-10-24 08:42:08.000000 oarepo-model-builder-files-4.0.8/oarepo_model_builder_files/profiles/file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 08:48:52.033152 oarepo-model-builder-files-4.0.8/oarepo_model_builder_files.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2023-10-24 08:48:51.000000 oarepo-model-builder-files-4.0.8/oarepo_model_builder_files.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3763 2023-10-24 08:48:52.000000 oarepo-model-builder-files-4.0.8/oarepo_model_builder_files.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-24 08:48:51.000000 oarepo-model-builder-files-4.0.8/oarepo_model_builder_files.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2246 2023-10-24 08:48:51.000000 oarepo-model-builder-files-4.0.8/oarepo_model_builder_files.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2023-10-24 08:48:51.000000 oarepo-model-builder-files-4.0.8/oarepo_model_builder_files.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2023-10-24 08:48:51.000000 oarepo-model-builder-files-4.0.8/oarepo_model_builder_files.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      102 2023-10-24 08:42:08.000000 oarepo-model-builder-files-4.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     2727 2023-10-24 08:48:52.045152 oarepo-model-builder-files-4.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-24 08:42:08.000000 oarepo-model-builder-files-4.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-29 20:49:45.442696 oarepo-model-builder-files-4.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2023-10-29 20:42:40.000000 oarepo-model-builder-files-4.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2023-10-29 20:49:45.442696 oarepo-model-builder-files-4.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1694 2023-10-29 20:42:40.000000 oarepo-model-builder-files-4.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-29 20:49:45.406696 oarepo-model-builder-files-4.0.9/oarepo_model_builder_files/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-29 20:42:40.000000 oarepo-model-builder-files-4.0.9/oarepo_model_builder_files/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-29 20:49:45.410696 oarepo-model-builder-files-4.0.9/oarepo_model_builder_files/builders/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-29 20:42:40.000000 oarepo-model-builder-files-4.0.9/oarepo_model_builder_files/builders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2023-10-29 20:42:40.000000 oarepo-model-builder-files-4.0.9/oarepo_model_builder_files/builders/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-29 20:49:45.414696 oarepo-model-builder-files-4.0.9/oarepo_model_builder_files/builders/invenio/
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2023-10-29 20:42:40.000000 oarepo-model-builder-files-4.0.9/oarepo_model_builder_files/builders/invenio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2023-10-29 20:42:40.000000 oarepo-model-builder-files-4.0.9/oarepo_model_builder_files/builders/invenio/invenio_files_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2023-10-29 20:42:40.000000 oarepo-model-builder-files-4.0.9/oarepo_model_builder_files/builders/invenio/invenio_files_record_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2023-10-29 20:42:40.000000 oarepo-model-builder-files-4.0.9/oarepo_model_builder_files/builders/invenio/invenio_files_record_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2023-10-29 20:42:40.000000 oarepo-model-builder-files-4.0.9/oarepo_model_builder_files/builders/invenio/invenio_files_record_service_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-29 20:49:45.418696 oarepo-model-builder-files-4.0.9/oarepo_model_builder_files/builders/invenio/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2023-10-29 20:42:40.000000 oarepo-model-builder-files-4.0.9/oarepo_model_builder_files/builders/invenio/templates/invenio_files_record.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2023-10-29 20:42:40.000000 oarepo-model-builder-files-4.0.9/oarepo_model_builder_files/builders/invenio/templates/invenio_files_record_metadata.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2023-10-29 20:42:40.000000 oarepo-model-builder-files-4.0.9/oarepo_model_builder_files/builders/invenio/templates/invenio_files_record_permissions.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2023-10-29 20:42:40.000000 oarepo-model-builder-files-4.0.9/oarepo_model_builder_files/builders/invenio/templates/invenio_files_record_service_config.py.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-29 20:49:45.422696 oarepo-model-builder-files-4.0.9/oarepo_model_builder_files/builders/invenio_parent/
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2023-10-29 20:42:40.000000 oarepo-model-builder-files-4.0.9/oarepo_model_builder_files/builders/invenio_parent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2023-10-29 20:42:40.000000 oarepo-model-builder-files-4.0.9/oarepo_model_builder_files/builders/invenio_parent/invenio_files_parent_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2023-10-29 20:42:40.000000 oarepo-model-builder-files-4.0.9/oarepo_model_builder_files/builders/invenio_parent/invenio_files_parent_record_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2023-10-29 20:42:40.000000 oarepo-model-builder-files-4.0.9/oarepo_model_builder_files/builders/invenio_parent/invenio_files_parent_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-29 20:49:45.422696 oarepo-model-builder-files-4.0.9/oarepo_model_builder_files/builders/invenio_parent/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2023-10-29 20:42:40.000000 oarepo-model-builder-files-4.0.9/oarepo_model_builder_files/builders/invenio_parent/templates/invenio_files_record.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2023-10-29 20:42:40.000000 oarepo-model-builder-files-4.0.9/oarepo_model_builder_files/builders/invenio_parent/templates/invenio_files_record_metadata.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)     1721 2023-10-29 20:42:40.000000 oarepo-model-builder-files-4.0.9/oarepo_model_builder_files/builders/invenio_parent/templates/invenio_files_schema.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2023-10-29 20:42:40.000000 oarepo-model-builder-files-4.0.9/oarepo_model_builder_files/builders/parent_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-29 20:49:45.426696 oarepo-model-builder-files-4.0.9/oarepo_model_builder_files/builders/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2023-10-29 20:42:40.000000 oarepo-model-builder-files-4.0.9/oarepo_model_builder_files/builders/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      338 2023-10-29 20:42:40.000000 oarepo-model-builder-files-4.0.9/oarepo_model_builder_files/builders/tests/invenio_files_conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2023-10-29 20:42:40.000000 oarepo-model-builder-files-4.0.9/oarepo_model_builder_files/builders/tests/invenio_files_conftest_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2023-10-29 20:42:40.000000 oarepo-model-builder-files-4.0.9/oarepo_model_builder_files/builders/tests/invenio_files_test_file_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-29 20:49:45.426696 oarepo-model-builder-files-4.0.9/oarepo_model_builder_files/builders/tests/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2023-10-29 20:42:40.000000 oarepo-model-builder-files-4.0.9/oarepo_model_builder_files/builders/tests/templates/invenio_files_conftest.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2023-10-29 20:42:40.000000 oarepo-model-builder-files-4.0.9/oarepo_model_builder_files/builders/tests/templates/invenio_files_conftest_files.py.jinja2
+-rw-r--r--   0 runner    (1001) docker     (127)    12349 2023-10-29 20:42:40.000000 oarepo-model-builder-files-4.0.9/oarepo_model_builder_files/builders/tests/templates/invenio_files_test_file_resources.py.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-29 20:49:45.426696 oarepo-model-builder-files-4.0.9/oarepo_model_builder_files/builtin_models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-29 20:42:40.000000 oarepo-model-builder-files-4.0.9/oarepo_model_builder_files/builtin_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2023-10-29 20:42:40.000000 oarepo-model-builder-files-4.0.9/oarepo_model_builder_files/builtin_models/invenio_files.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-29 20:49:45.430696 oarepo-model-builder-files-4.0.9/oarepo_model_builder_files/datatypes/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2023-10-29 20:42:40.000000 oarepo-model-builder-files-4.0.9/oarepo_model_builder_files/datatypes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-29 20:49:45.434696 oarepo-model-builder-files-4.0.9/oarepo_model_builder_files/datatypes/components/
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2023-10-29 20:42:40.000000 oarepo-model-builder-files-4.0.9/oarepo_model_builder_files/datatypes/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4675 2023-10-29 20:42:40.000000 oarepo-model-builder-files-4.0.9/oarepo_model_builder_files/datatypes/components/file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-29 20:49:45.438696 oarepo-model-builder-files-4.0.9/oarepo_model_builder_files/datatypes/components/files_model/
+-rw-r--r--   0 runner    (1001) docker     (127)     1403 2023-10-29 20:42:40.000000 oarepo-model-builder-files-4.0.9/oarepo_model_builder_files/datatypes/components/files_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2023-10-29 20:42:40.000000 oarepo-model-builder-files-4.0.9/oarepo_model_builder_files/datatypes/components/files_model/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2023-10-29 20:42:40.000000 oarepo-model-builder-files-4.0.9/oarepo_model_builder_files/datatypes/components/files_model/ext_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1990 2023-10-29 20:42:40.000000 oarepo-model-builder-files-4.0.9/oarepo_model_builder_files/datatypes/components/files_model/files_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2023-10-29 20:42:40.000000 oarepo-model-builder-files-4.0.9/oarepo_model_builder_files/datatypes/components/files_model/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2023-10-29 20:42:40.000000 oarepo-model-builder-files-4.0.9/oarepo_model_builder_files/datatypes/components/files_model/pid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2023-10-29 20:42:40.000000 oarepo-model-builder-files-4.0.9/oarepo_model_builder_files/datatypes/components/files_model/record.py
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2023-10-29 20:42:40.000000 oarepo-model-builder-files-4.0.9/oarepo_model_builder_files/datatypes/components/files_model/record_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1372 2023-10-29 20:42:40.000000 oarepo-model-builder-files-4.0.9/oarepo_model_builder_files/datatypes/components/files_model/resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2023-10-29 20:42:40.000000 oarepo-model-builder-files-4.0.9/oarepo_model_builder_files/datatypes/components/files_model/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2023-10-29 20:42:40.000000 oarepo-model-builder-files-4.0.9/oarepo_model_builder_files/datatypes/components/files_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2023-10-29 20:42:40.000000 oarepo-model-builder-files-4.0.9/oarepo_model_builder_files/datatypes/components/parent_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2023-10-29 20:42:40.000000 oarepo-model-builder-files-4.0.9/oarepo_model_builder_files/datatypes/components/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2023-10-29 20:42:40.000000 oarepo-model-builder-files-4.0.9/oarepo_model_builder_files/datatypes/file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-29 20:49:45.438696 oarepo-model-builder-files-4.0.9/oarepo_model_builder_files/profiles/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-29 20:42:40.000000 oarepo-model-builder-files-4.0.9/oarepo_model_builder_files/profiles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2023-10-29 20:42:40.000000 oarepo-model-builder-files-4.0.9/oarepo_model_builder_files/profiles/file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-29 20:49:45.410696 oarepo-model-builder-files-4.0.9/oarepo_model_builder_files.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2023-10-29 20:49:45.000000 oarepo-model-builder-files-4.0.9/oarepo_model_builder_files.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3763 2023-10-29 20:49:45.000000 oarepo-model-builder-files-4.0.9/oarepo_model_builder_files.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-29 20:49:45.000000 oarepo-model-builder-files-4.0.9/oarepo_model_builder_files.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2246 2023-10-29 20:49:45.000000 oarepo-model-builder-files-4.0.9/oarepo_model_builder_files.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2023-10-29 20:49:45.000000 oarepo-model-builder-files-4.0.9/oarepo_model_builder_files.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2023-10-29 20:49:45.000000 oarepo-model-builder-files-4.0.9/oarepo_model_builder_files.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2023-10-29 20:42:40.000000 oarepo-model-builder-files-4.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     2727 2023-10-29 20:49:45.442696 oarepo-model-builder-files-4.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-29 20:42:40.000000 oarepo-model-builder-files-4.0.9/setup.py
```

### Comparing `oarepo-model-builder-files-4.0.8/PKG-INFO` & `oarepo-model-builder-files-4.0.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-model-builder-files
-Version: 4.0.8
+Version: 4.0.9
 Description-Content-Type: text/markdown
 Requires-Dist: oarepo-model-builder-tests>=4.0.0
 Requires-Dist: oarepo-model-builder>=4.0.0
 
 # OARepo model builder files
 
 Plugin adding support for working with files based on the invenio model. <br>
```

### Comparing `oarepo-model-builder-files-4.0.8/README.md` & `oarepo-model-builder-files-4.0.9/README.md`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-files-4.0.8/oarepo_model_builder_files/builders/base.py` & `oarepo-model-builder-files-4.0.9/oarepo_model_builder_files/builders/base.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-files-4.0.8/oarepo_model_builder_files/builders/invenio/__init__.py` & `oarepo-model-builder-files-4.0.9/oarepo_model_builder_files/builders/invenio/__init__.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-files-4.0.8/oarepo_model_builder_files/builders/invenio/templates/invenio_files_record_permissions.py.jinja2` & `oarepo-model-builder-files-4.0.9/oarepo_model_builder_files/builders/invenio/templates/invenio_files_record_permissions.py.jinja2`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from invenio_records_resources.services.files.generators import AnyUserIfFileIsLocal
-{{ vars.permissions.imports|generate_import }}
+{{ vars.permissions|imports }}
 
 class {{ vars.permissions|class_header }}:
     # defined in profiles, here just for information
     #
     # can_create_files = [AnyUser(), SystemProcess()]
     # can_set_content_files = [AnyUserIfFileIsLocal(), SystemProcess()]
     # can_get_content_files = [AnyUserIfFileIsLocal(), SystemProcess()]
```

### Comparing `oarepo-model-builder-files-4.0.8/oarepo_model_builder_files/builders/invenio_parent/templates/invenio_files_record.py.jinja2` & `oarepo-model-builder-files-4.0.9/oarepo_model_builder_files/builders/invenio_parent/templates/invenio_files_record.py.jinja2`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-from invenio_records_resources.records.systemfields import FilesField
 from invenio_records.systemfields import ModelField
 
 {{ vars.record.class|generate_import }}
+{{ vars.files_field.file_class|generate_import }}
+{{ vars.files_field.field_class|generate_import }}
 
 class {{ metadata_record.record.class|base_name }}:
     {% if not vars.files_field.skip %}
-    files = {{ vars.files_field.field_class }}(
-        file_cls={{ vars.files_field.file_class }}{% if vars.files_field.field_args %},
+    files = {{ vars.files_field.field_class|base_name }}(
+        file_cls={{ vars.files_field.file_class|base_name }}{% if vars.files_field.field_args %},
         {{ vars.files_field.field_args|generate_list }}
     {% endif %}
     )
     {% endif %}
 
     bucket_id = ModelField(dump=False)
     bucket = ModelField(dump=False)
```

### Comparing `oarepo-model-builder-files-4.0.8/oarepo_model_builder_files/builders/invenio_parent/templates/invenio_files_schema.py.jinja2` & `oarepo-model-builder-files-4.0.9/oarepo_model_builder_files/builders/invenio_parent/templates/invenio_files_schema.py.jinja2`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-files-4.0.8/oarepo_model_builder_files/builders/parent_builder.py` & `oarepo-model-builder-files-4.0.9/oarepo_model_builder_files/builders/parent_builder.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-files-4.0.8/oarepo_model_builder_files/builders/tests/invenio_files_test_file_resources.py` & `oarepo-model-builder-files-4.0.9/oarepo_model_builder_files/builders/tests/invenio_files_test_file_resources.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-files-4.0.8/oarepo_model_builder_files/builders/tests/templates/invenio_files_conftest.py.jinja2` & `oarepo-model-builder-files-4.0.9/oarepo_model_builder_files/builders/tests/templates/invenio_files_conftest.py.jinja2`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-files-4.0.8/oarepo_model_builder_files/builders/tests/templates/invenio_files_conftest_files.py.jinja2` & `oarepo-model-builder-files-4.0.9/oarepo_model_builder_files/builders/tests/templates/invenio_files_conftest_files.py.jinja2`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-files-4.0.8/oarepo_model_builder_files/builders/tests/templates/invenio_files_test_file_resources.py.jinja2` & `oarepo-model-builder-files-4.0.9/oarepo_model_builder_files/builders/tests/templates/invenio_files_test_file_resources.py.jinja2`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-files-4.0.8/oarepo_model_builder_files/builtin_models/invenio_files.json` & `oarepo-model-builder-files-4.0.9/oarepo_model_builder_files/builtin_models/invenio_files.json`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-files-4.0.8/oarepo_model_builder_files/datatypes/components/__init__.py` & `oarepo-model-builder-files-4.0.9/oarepo_model_builder_files/datatypes/components/__init__.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-files-4.0.8/oarepo_model_builder_files/datatypes/components/file.py` & `oarepo-model-builder-files-4.0.9/oarepo_model_builder_files/datatypes/components/file.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 import marshmallow as ma
 from oarepo_model_builder.datatypes import (
     DataType,
     DataTypeComponent,
-    Import,
     ModelDataType,
     Section,
 )
 from oarepo_model_builder.datatypes.components import DefaultsModelComponent
 from oarepo_model_builder.datatypes.components.model.utils import set_default
 from oarepo_model_builder.datatypes.model import Link
 from oarepo_model_builder.utils.links import url_prefix2link
-
+from oarepo_model_builder.utils.python_name import Import
 
 def get_file_schema():
     from ..file import FileDataType
 
     return FileDataType.validator()
```

### Comparing `oarepo-model-builder-files-4.0.8/oarepo_model_builder_files/datatypes/components/files_model/__init__.py` & `oarepo-model-builder-files-4.0.9/oarepo_model_builder_files/datatypes/components/files_model/__init__.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-files-4.0.8/oarepo_model_builder_files/datatypes/components/files_model/defaults.py` & `oarepo-model-builder-files-4.0.9/oarepo_model_builder_files/datatypes/components/files_model/defaults.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-files-4.0.8/oarepo_model_builder_files/datatypes/components/files_model/ext_resource.py` & `oarepo-model-builder-files-4.0.9/oarepo_model_builder_files/datatypes/components/files_model/ext_resource.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-files-4.0.8/oarepo_model_builder_files/datatypes/components/files_model/files_field.py` & `oarepo-model-builder-files-4.0.9/oarepo_model_builder_files/datatypes/components/files_model/files_field.py`

 * *Files 10% similar despite different names*

```diff
@@ -44,17 +44,16 @@
         )
 
     def before_model_prepare(self, datatype, *, context, **kwargs):
         file_record = datatype.definition["record"]
 
         files_field = set_default(datatype, "files-field", {})
         files_field.setdefault("generate", True)
-        files_field.setdefault("field-class", "FilesField")
-        files_field.setdefault("file-class", base_name(file_record["class"]))
+        files_field.setdefault(
+            "field-class", "invenio_records_resources.records.systemfields.FilesField"
+        )
+        files_field.setdefault("file-class", file_record["class"])
         files_field.setdefault("field-args", ["store=False"])
         files_field.setdefault(
             "imports",
-            [
-                {"import": "invenio_records_resources.records.systemfields.FilesField"},
-                {"import": file_record["class"]},
-            ],
+            [],
         )
```

### Comparing `oarepo-model-builder-files-4.0.8/oarepo_model_builder_files/datatypes/components/files_model/permissions.py` & `oarepo-model-builder-files-4.0.9/oarepo_model_builder_files/datatypes/components/files_model/permissions.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-files-4.0.8/oarepo_model_builder_files/datatypes/components/files_model/pid.py` & `oarepo-model-builder-files-4.0.9/oarepo_model_builder_files/datatypes/components/files_model/pid.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-files-4.0.8/oarepo_model_builder_files/datatypes/components/files_model/record.py` & `oarepo-model-builder-files-4.0.9/oarepo_model_builder_files/datatypes/components/files_model/record.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,12 +12,12 @@
 
     def before_model_prepare(self, datatype, *, context, **kwargs):
         parent_record_datatype = get_metadata_record(datatype, context)
         parent_record_prefix = parent_record_datatype.definition["module"]["prefix"]
 
         record = set_default(datatype, "record", {})
         record.setdefault("class", f"{parent_record_prefix}File")
-        record.setdefault("base-classes", ["FileRecord"])
         record.setdefault(
-            "imports", [{"import": "invenio_records_resources.records.api.FileRecord"}]
+            "base-classes", ["invenio_records_resources.records.api.FileRecord"]
         )
+        record.setdefault("imports", [])
         super().before_model_prepare(datatype, context=context, **kwargs)
```

### Comparing `oarepo-model-builder-files-4.0.8/oarepo_model_builder_files/datatypes/components/files_model/resource.py` & `oarepo-model-builder-files-4.0.9/oarepo_model_builder_files/datatypes/components/files_model/resource.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,24 +13,19 @@
     def before_model_prepare(self, datatype, *, context, **kwargs):
         parent_record_datatype = get_metadata_record(datatype, context)
         resource_config = set_default(datatype, "resource-config", {})
         parent_record_url = parent_record_datatype.definition["resource-config"][
             "base-url"
         ]
         resource_config.setdefault("base-url", f"{parent_record_url}<pid_value>")
-        resource_config.setdefault("base-classes", ["FileResourceConfig"])
         resource_config.setdefault(
-            "imports",
-            [{"import": "invenio_records_resources.resources.FileResourceConfig"}],
+            "base-classes", ["invenio_records_resources.resources.FileResourceConfig"]
         )
+        resource_config.setdefault("imports", [])
         resource = set_default(datatype, "resource", {})
-        resource.setdefault("base-classes", ["FileResource"])
         resource.setdefault(
-            "imports",
-            [
-                {
-                    "import": "invenio_records_resources.resources.files.resource.FileResource"
-                }
-            ],
+            "base-classes",
+            ["invenio_records_resources.resources.files.resource.FileResource"],
         )
+        resource.setdefault("imports", [])
 
         super().before_model_prepare(datatype, context=context, **kwargs)
```

### Comparing `oarepo-model-builder-files-4.0.8/oarepo_model_builder_files/datatypes/components/files_model/service.py` & `oarepo-model-builder-files-4.0.9/oarepo_model_builder_files/datatypes/components/files_model/service.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,25 +7,21 @@
 class FilesServiceModelComponent(ServiceModelComponent):
     eligible_datatypes = [FileDataType]
     dependency_remap = ServiceModelComponent
 
     def before_model_prepare(self, datatype, *, context, **kwargs):
         service_config = set_default(datatype, "service-config", {})
         service_config.setdefault(
-            "base-classes", ["PermissionsPresetsConfigMixin", "FileServiceConfig"]
-        )
-        service_config.setdefault(
-            "imports",
+            "base-classes",
             [
-                {"import": "invenio_records_resources.services.FileServiceConfig"},
-                {
-                    "import": "oarepo_runtime.config.service.PermissionsPresetsConfigMixin"
-                },
+                "oarepo_runtime.config.service.PermissionsPresetsConfigMixin",
+                "invenio_records_resources.services.FileServiceConfig",
             ],
         )
+        service_config.setdefault("imports", [])
 
         service = set_default(datatype, "service", {})
-        service.setdefault("base-classes", ["FileService"])
         service.setdefault(
-            "imports", [{"import": "invenio_records_resources.services.FileService"}]
+            "base-classes", ["invenio_records_resources.services.FileService"]
         )
+        service.setdefault("imports", [])
         super().before_model_prepare(datatype, context=context, **kwargs)
```

### Comparing `oarepo-model-builder-files-4.0.8/oarepo_model_builder_files/datatypes/components/files_tests.py` & `oarepo-model-builder-files-4.0.9/oarepo_model_builder_files/datatypes/components/files_tests.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-files-4.0.8/oarepo_model_builder_files/profiles/file.py` & `oarepo-model-builder-files-4.0.9/oarepo_model_builder_files/profiles/file.py`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-files-4.0.8/oarepo_model_builder_files.egg-info/PKG-INFO` & `oarepo-model-builder-files-4.0.9/oarepo_model_builder_files.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-model-builder-files
-Version: 4.0.8
+Version: 4.0.9
 Description-Content-Type: text/markdown
 Requires-Dist: oarepo-model-builder-tests>=4.0.0
 Requires-Dist: oarepo-model-builder>=4.0.0
 
 # OARepo model builder files
 
 Plugin adding support for working with files based on the invenio model. <br>
```

### Comparing `oarepo-model-builder-files-4.0.8/oarepo_model_builder_files.egg-info/SOURCES.txt` & `oarepo-model-builder-files-4.0.9/oarepo_model_builder_files.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-files-4.0.8/oarepo_model_builder_files.egg-info/entry_points.txt` & `oarepo-model-builder-files-4.0.9/oarepo_model_builder_files.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-files-4.0.8/setup.cfg` & `oarepo-model-builder-files-4.0.9/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = oarepo-model-builder-files
-version = 4.0.8
+version = 4.0.9
 description = 
 authors = Ronald Krist <krist@cesnet.cz>
 readme = README.md
 long_description = file:README.md
 long_description_content_type = text/markdown
 
 [options]
```

