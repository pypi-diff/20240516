# Comparing `tmp/django_import_export-4.0.2.tar.gz` & `tmp/django_import_export-4.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_import_export-4.0.2.tar", last modified: Mon May 13 18:47:11 2024, max compression
+gzip compressed data, was "django_import_export-4.0.3.tar", last modified: Thu May 16 13:47:07 2024, max compression
```

## Comparing `django_import_export-4.0.2.tar` & `django_import_export-4.0.3.tar`

### file list

```diff
@@ -1,336 +1,344 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.700663 django_import_export-4.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-13 18:47:07.000000 django_import_export-4.0.2/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-13 18:47:07.000000 django_import_export-4.0.2/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-13 18:47:07.000000 django_import_export-4.0.2/.flake8
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-13 18:47:07.000000 django_import_export-4.0.2/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.656663 django_import_export-4.0.2/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-13 18:47:07.000000 django_import_export-4.0.2/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.656663 django_import_export-4.0.2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-13 18:47:07.000000 django_import_export-4.0.2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-13 18:47:07.000000 django_import_export-4.0.2/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-13 18:47:07.000000 django_import_export-4.0.2/.github/ISSUE_TEMPLATE/question.md
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-13 18:47:07.000000 django_import_export-4.0.2/.github/pull_request_template.md
--rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-05-13 18:47:07.000000 django_import_export-4.0.2/.github/stale.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.660663 django_import_export-4.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-13 18:47:07.000000 django_import_export-4.0.2/.github/workflows/pre-commit.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-05-13 18:47:07.000000 django_import_export-4.0.2/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-05-13 18:47:07.000000 django_import_export-4.0.2/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-13 18:47:07.000000 django_import_export-4.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-13 18:47:07.000000 django_import_export-4.0.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-05-13 18:47:07.000000 django_import_export-4.0.2/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3784 2024-05-13 18:47:07.000000 django_import_export-4.0.2/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)     5547 2024-05-13 18:47:07.000000 django_import_export-4.0.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-13 18:47:07.000000 django_import_export-4.0.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-13 18:47:07.000000 django_import_export-4.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-05-13 18:47:07.000000 django_import_export-4.0.2/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     5434 2024-05-13 18:47:11.700663 django_import_export-4.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-05-13 18:47:07.000000 django_import_export-4.0.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-05-13 18:47:07.000000 django_import_export-4.0.2/RELEASE.md
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-13 18:47:07.000000 django_import_export-4.0.2/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.696663 django_import_export-4.0.2/django_import_export.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5434 2024-05-13 18:47:11.000000 django_import_export-4.0.2/django_import_export.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10128 2024-05-13 18:47:11.000000 django_import_export-4.0.2/django_import_export.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 18:47:11.000000 django_import_export-4.0.2/django_import_export.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-13 18:47:11.000000 django_import_export-4.0.2/django_import_export.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-13 18:47:11.000000 django_import_export-4.0.2/django_import_export.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.664662 django_import_export-4.0.2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     5621 2024-05-13 18:47:07.000000 django_import_export-4.0.2/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.644662 django_import_export-4.0.2/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.668663 django_import_export-4.0.2/docs/_static/images/
--rw-r--r--   0 runner    (1001) docker     (127)    21509 2024-05-13 18:47:07.000000 django_import_export-4.0.2/docs/_static/images/change-form-export.png
--rw-r--r--   0 runner    (1001) docker     (127)    28966 2024-05-13 18:47:07.000000 django_import_export-4.0.2/docs/_static/images/custom-export-form.png
--rw-r--r--   0 runner    (1001) docker     (127)    90059 2024-05-13 18:47:07.000000 django_import_export-4.0.2/docs/_static/images/custom-import-form.png
--rw-r--r--   0 runner    (1001) docker     (127)    33092 2024-05-13 18:47:07.000000 django_import_export-4.0.2/docs/_static/images/date-widget-validation-error.png
--rw-r--r--   0 runner    (1001) docker     (127)    30818 2024-05-13 18:47:07.000000 django_import_export-4.0.2/docs/_static/images/django-import-export-change.png
--rw-r--r--   0 runner    (1001) docker     (127)    29191 2024-05-13 18:47:07.000000 django_import_export-4.0.2/docs/_static/images/django-import-export-export-confirm.png
--rw-r--r--   0 runner    (1001) docker     (127)    35696 2024-05-13 18:47:07.000000 django_import_export-4.0.2/docs/_static/images/django-import-export-import-confirm.png
--rw-r--r--   0 runner    (1001) docker     (127)    32366 2024-05-13 18:47:07.000000 django_import_export-4.0.2/docs/_static/images/django-import-export-import.png
--rw-r--r--   0 runner    (1001) docker     (127)     6097 2024-05-13 18:47:07.000000 django_import_export-4.0.2/docs/_static/images/export-button.png
--rw-r--r--   0 runner    (1001) docker     (127)    33710 2024-05-13 18:47:07.000000 django_import_export-4.0.2/docs/_static/images/export_workflow.svg
--rw-r--r--   0 runner    (1001) docker     (127)     6047 2024-05-13 18:47:07.000000 django_import_export-4.0.2/docs/_static/images/import-button.png
--rw-r--r--   0 runner    (1001) docker     (127)    56726 2024-05-13 18:47:07.000000 django_import_export-4.0.2/docs/_static/images/import_workflow.svg
--rw-r--r--   0 runner    (1001) docker     (127)    29758 2024-05-13 18:47:07.000000 django_import_export-4.0.2/docs/_static/images/non-field-specific-validation-error.png
--rw-r--r--   0 runner    (1001) docker     (127)    17197 2024-05-13 18:47:07.000000 django_import_export-4.0.2/docs/_static/images/select-for-export.png
--rw-r--r--   0 runner    (1001) docker     (127)    22107 2024-05-13 18:47:07.000000 django_import_export-4.0.2/docs/admin_integration.rst
--rw-r--r--   0 runner    (1001) docker     (127)    30707 2024-05-13 18:47:07.000000 django_import_export-4.0.2/docs/advanced_usage.rst
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-13 18:47:07.000000 django_import_export-4.0.2/docs/api_admin.rst
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-13 18:47:07.000000 django_import_export-4.0.2/docs/api_exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-13 18:47:07.000000 django_import_export-4.0.2/docs/api_fields.rst
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-13 18:47:07.000000 django_import_export-4.0.2/docs/api_forms.rst
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-13 18:47:07.000000 django_import_export-4.0.2/docs/api_instance_loaders.rst
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-05-13 18:47:07.000000 django_import_export-4.0.2/docs/api_mixins.rst
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-13 18:47:07.000000 django_import_export-4.0.2/docs/api_resources.rst
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-13 18:47:07.000000 django_import_export-4.0.2/docs/api_results.rst
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-13 18:47:07.000000 django_import_export-4.0.2/docs/api_tmp_storages.rst
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-13 18:47:07.000000 django_import_export-4.0.2/docs/api_widgets.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3421 2024-05-13 18:47:07.000000 django_import_export-4.0.2/docs/bulk_import.rst
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-13 18:47:07.000000 django_import_export-4.0.2/docs/celery.rst
--rw-r--r--   0 runner    (1001) docker     (127)    58752 2024-05-13 18:47:07.000000 django_import_export-4.0.2/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-05-13 18:47:07.000000 django_import_export-4.0.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     6284 2024-05-13 18:47:07.000000 django_import_export-4.0.2/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-05-13 18:47:07.000000 django_import_export-4.0.2/docs/export_workflow.rst
--rwxr-xr-x   0 runner    (1001) docker     (127)    10047 2024-05-13 18:47:07.000000 django_import_export-4.0.2/docs/faq.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4748 2024-05-13 18:47:07.000000 django_import_export-4.0.2/docs/getting_started.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.668663 django_import_export-4.0.2/docs/image_src/
--rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-05-13 18:47:07.000000 django_import_export-4.0.2/docs/image_src/export_workflow.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3002 2024-05-13 18:47:07.000000 django_import_export-4.0.2/docs/image_src/import_workflow.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5713 2024-05-13 18:47:07.000000 django_import_export-4.0.2/docs/import_workflow.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-05-13 18:47:07.000000 django_import_export-4.0.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7889 2024-05-13 18:47:07.000000 django_import_export-4.0.2/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5126 2024-05-13 18:47:07.000000 django_import_export-4.0.2/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)    14882 2024-05-13 18:47:07.000000 django_import_export-4.0.2/docs/release_notes.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2662 2024-05-13 18:47:07.000000 django_import_export-4.0.2/docs/testing.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.672663 django_import_export-4.0.2/import_export/
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-13 18:47:11.000000 django_import_export-4.0.2/import_export/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    35711 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)     6467 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/declarative.py
--rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5643 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/fields.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.672663 django_import_export-4.0.2/import_export/formats/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/formats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6018 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/formats/base_formats.py
--rw-r--r--   0 runner    (1001) docker     (127)     9611 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/forms.py
--rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/instance_loaders.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.652662 django_import_export-4.0.2/import_export/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.644662 django_import_export-4.0.2/import_export/locale/ar/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.672663 django_import_export-4.0.2/import_export/locale/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/locale/ar/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5394 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/locale/ar/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.648662 django_import_export-4.0.2/import_export/locale/bg/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.672663 django_import_export-4.0.2/import_export/locale/bg/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/locale/bg/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5626 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/locale/bg/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.648662 django_import_export-4.0.2/import_export/locale/ca/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.672663 django_import_export-4.0.2/import_export/locale/ca/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/locale/ca/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5117 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/locale/ca/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.648662 django_import_export-4.0.2/import_export/locale/cs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.672663 django_import_export-4.0.2/import_export/locale/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/locale/cs/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5187 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/locale/cs/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.648662 django_import_export-4.0.2/import_export/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.672663 django_import_export-4.0.2/import_export/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     2269 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5619 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.648662 django_import_export-4.0.2/import_export/locale/es/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.672663 django_import_export-4.0.2/import_export/locale/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5708 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.648662 django_import_export-4.0.2/import_export/locale/es_AR/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.672663 django_import_export-4.0.2/import_export/locale/es_AR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/locale/es_AR/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5712 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/locale/es_AR/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.648662 django_import_export-4.0.2/import_export/locale/fa/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.672663 django_import_export-4.0.2/import_export/locale/fa/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/locale/fa/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5726 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/locale/fa/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.648662 django_import_export-4.0.2/import_export/locale/fi/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.672663 django_import_export-4.0.2/import_export/locale/fi/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/locale/fi/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5140 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/locale/fi/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.648662 django_import_export-4.0.2/import_export/locale/fr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.676663 django_import_export-4.0.2/import_export/locale/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5108 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.648662 django_import_export-4.0.2/import_export/locale/it/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.676663 django_import_export-4.0.2/import_export/locale/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/locale/it/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5067 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/locale/it/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.648662 django_import_export-4.0.2/import_export/locale/ja/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.676663 django_import_export-4.0.2/import_export/locale/ja/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/locale/ja/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5194 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/locale/ja/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.648662 django_import_export-4.0.2/import_export/locale/ko/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.676663 django_import_export-4.0.2/import_export/locale/ko/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/locale/ko/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5371 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/locale/ko/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.648662 django_import_export-4.0.2/import_export/locale/kz/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.676663 django_import_export-4.0.2/import_export/locale/kz/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/locale/kz/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5913 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/locale/kz/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.648662 django_import_export-4.0.2/import_export/locale/nl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.676663 django_import_export-4.0.2/import_export/locale/nl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/locale/nl/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5456 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/locale/nl/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.648662 django_import_export-4.0.2/import_export/locale/pl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.676663 django_import_export-4.0.2/import_export/locale/pl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/locale/pl/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5280 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/locale/pl/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.648662 django_import_export-4.0.2/import_export/locale/pt_BR/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.676663 django_import_export-4.0.2/import_export/locale/pt_BR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/locale/pt_BR/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5405 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/locale/pt_BR/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.648662 django_import_export-4.0.2/import_export/locale/ru/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.676663 django_import_export-4.0.2/import_export/locale/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     5198 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     7399 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.648662 django_import_export-4.0.2/import_export/locale/sk/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.676663 django_import_export-4.0.2/import_export/locale/sk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/locale/sk/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5113 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/locale/sk/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.652662 django_import_export-4.0.2/import_export/locale/tr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.676663 django_import_export-4.0.2/import_export/locale/tr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/locale/tr/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5465 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/locale/tr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.652662 django_import_export-4.0.2/import_export/locale/zh_Hans/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.676663 django_import_export-4.0.2/import_export/locale/zh_Hans/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/locale/zh_Hans/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (127)     5238 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/locale/zh_Hans/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (127)     8064 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)     6543 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/options.py
--rw-r--r--   0 runner    (1001) docker     (127)    50781 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     8079 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/results.py
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.652662 django_import_export-4.0.2/import_export/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.680663 django_import_export-4.0.2/import_export/static/import_export/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/static/import_export/export.css
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/static/import_export/export_selectable_fields.js
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/static/import_export/guess_format.js
--rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/static/import_export/import.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.652662 django_import_export-4.0.2/import_export/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.652662 django_import_export-4.0.2/import_export/templates/admin/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.680663 django_import_export-4.0.2/import_export/templates/admin/import_export/
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/templates/admin/import_export/base.html
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/templates/admin/import_export/change_form.html
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/templates/admin/import_export/change_list.html
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/templates/admin/import_export/change_list_export.html
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/templates/admin/import_export/change_list_export_item.html
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/templates/admin/import_export/change_list_import.html
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/templates/admin/import_export/change_list_import_export.html
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/templates/admin/import_export/change_list_import_item.html
--rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/templates/admin/import_export/export.html
--rw-r--r--   0 runner    (1001) docker     (127)     6686 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/templates/admin/import_export/import.html
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/templates/admin/import_export/resource_fields_list.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.680663 django_import_export-4.0.2/import_export/templatetags/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/templatetags/import_export_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/tmp_storages.py
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    21446 2024-05-13 18:47:07.000000 django_import_export-4.0.2/import_export/widgets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-05-13 18:47:07.000000 django_import_export-4.0.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.680663 django_import_export-4.0.2/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-13 18:47:07.000000 django_import_export-4.0.2/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-13 18:47:07.000000 django_import_export-4.0.2/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-13 18:47:07.000000 django_import_export-4.0.2/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-05-13 18:47:07.000000 django_import_export-4.0.2/runtests.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      884 2024-05-13 18:47:07.000000 django_import_export-4.0.2/runtests.sh
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 18:47:11.700663 django_import_export-4.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 18:47:07.000000 django_import_export-4.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.680663 django_import_export-4.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/books-sample.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.684663 django_import_export-4.0.2/tests/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3475 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.684663 django_import_export-4.0.2/tests/core/exports/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/exports/authors.csv
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/exports/books-ISO-8859-1.csv
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/exports/books-dos.csv
--rw-r--r--   0 runner    (1001) docker     (127)     9650 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/exports/books-empty-author-email.xlsx
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/exports/books-for-delete.csv
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/exports/books-invalid-date.csv
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/exports/books-mac.csv
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/exports/books-mac.tsv
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/exports/books-no-headers.csv
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/exports/books-unicode.csv
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/exports/books-unicode.tsv
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/exports/books.csv
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/exports/books.json
--rw-r--r--   0 runner    (1001) docker     (127)     5632 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/exports/books.xls
--rw-r--r--   0 runner    (1001) docker     (127)     4886 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/exports/books.xlsx
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/exports/child.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.684663 django_import_export-4.0.2/tests/core/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/fixtures/author.json
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/fixtures/book.json
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/fixtures/category.json
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.688663 django_import_export-4.0.2/tests/core/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     5662 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/migrations/0002_book_published_time.py
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/migrations/0003_withfloatfield.py
--rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/migrations/0004_bookwithchapters.py
--rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/migrations/0005_addparentchild.py
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/migrations/0006_auto_20171130_0147.py
--rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/migrations/0007_auto_20180628_0411.py
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/migrations/0008_auto_20190409_0846.py
--rw-r--r--   0 runner    (1001) docker     (127)     3131 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/migrations/0009_auto_20211111_0807.py
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/migrations/0010_uuidbook.py
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/migrations/0011_uuidcategory_legacybook_alter_uuidbook_id_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/migrations/0012_delete_legacybook.py
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/migrations/0013_alter_author_birthday.py
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/migrations/0014_bookwithchapternumbers.py
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/migrations/0015_withpositiveintegerfields.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5102 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.652662 django_import_export-4.0.2/tests/core/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.688663 django_import_export-4.0.2/tests/core/templates/core/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.688663 django_import_export-4.0.2/tests/core/templates/core/admin/
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/templates/core/admin/change_list.html
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/templates/core/category_list.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.692663 django_import_export-4.0.2/tests/core/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.692663 django_import_export-4.0.2/tests/core/tests/admin_integration/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/tests/admin_integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/tests/admin_integration/mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)     8435 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/tests/admin_integration/test_action_export.py
--rw-r--r--   0 runner    (1001) docker     (127)    20354 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/tests/admin_integration/test_export.py
--rw-r--r--   0 runner    (1001) docker     (127)    40988 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/tests/admin_integration/test_import.py
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/tests/admin_integration/test_views.py
--rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/tests/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     8043 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/tests/test_base_formats.py
--rw-r--r--   0 runner    (1001) docker     (127)     3706 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/tests/test_declarative.py
--rw-r--r--   0 runner    (1001) docker     (127)     5318 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/tests/test_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     7211 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/tests/test_forms.py
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/tests/test_import_export_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/tests/test_instance_loaders.py
--rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/tests/test_invalidrow.py
--rw-r--r--   0 runner    (1001) docker     (127)    11181 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/tests/test_mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)     8133 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/tests/test_model_resource_fields_generate_widgets.py
--rw-r--r--   0 runner    (1001) docker     (127)     4622 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/tests/test_permissions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.692663 django_import_export-4.0.2/tests/core/tests/test_resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/tests/test_resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22130 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/tests/test_resources/test_bulk_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     4295 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/tests/test_resources/test_diffs.py
--rw-r--r--   0 runner    (1001) docker     (127)    15445 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/tests/test_resources/test_import_export.py
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/tests/test_resources/test_misc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.696663 django_import_export-4.0.2/tests/core/tests/test_resources/test_modelresource/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/tests/test_resources/test_modelresource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6300 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/tests/test_resources/test_modelresource/test_data_deletion.py
--rw-r--r--   0 runner    (1001) docker     (127)     4626 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/tests/test_resources/test_modelresource/test_data_handling.py
--rw-r--r--   0 runner    (1001) docker     (127)     5698 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/tests/test_resources/test_modelresource/test_data_import.py
--rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/tests/test_resources/test_modelresource/test_deprecated_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)    13486 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/tests/test_resources/test_modelresource/test_dynamic_customization.py
--rw-r--r--   0 runner    (1001) docker     (127)     6718 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/tests/test_resources/test_modelresource/test_error_handling.py
--rw-r--r--   0 runner    (1001) docker     (127)     2816 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/tests/test_resources/test_modelresource/test_export.py
--rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/tests/test_resources/test_modelresource/test_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     5596 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/tests/test_resources/test_modelresource/test_m2m.py
--rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/tests/test_resources/test_modelresource/test_queryset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/tests/test_resources/test_modelresource/test_relationship.py
--rw-r--r--   0 runner    (1001) docker     (127)     3661 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/tests/test_resources/test_modelresource/test_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/tests/test_resources/test_modelresource/test_resource_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     6083 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/tests/test_resources/test_modelresource/test_resource_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     7346 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/tests/test_resources/test_modelresource/test_resource_postgres.py
--rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/tests/test_resources/test_modelresource/test_resource_setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     4598 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/tests/test_resources/test_modelresource/test_resource_transactions.py
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/tests/test_resources/test_modelresource/test_string_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/tests/test_resources/test_modelresource/test_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/tests/test_resources/test_natural_foreign_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     9679 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/tests/test_resources/test_relationships.py
--rw-r--r--   0 runner    (1001) docker     (127)     4651 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/tests/test_results.py
--rw-r--r--   0 runner    (1001) docker     (127)     5877 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/tests/test_tmp_storages.py
--rw-r--r--   0 runner    (1001) docker     (127)    26689 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/tests/test_widgets.py
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/tests/widget.py
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/core/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.652662 django_import_export-4.0.2/tests/docker/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.696663 django_import_export-4.0.2/tests/docker/db/
--rwxr-xr-x   0 runner    (1001) docker     (127)      146 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/docker/db/init-mysql-db.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      401 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/docker/db/init-postgres-db.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/docker-compose.yml
--rwxr-xr-x   0 runner    (1001) docker     (127)      320 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/manage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:11.696663 django_import_export-4.0.2/tests/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5341 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/scripts/bulk_import.py
--rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tests/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)      985 2024-05-13 18:47:07.000000 django_import_export-4.0.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.546338 django_import_export-4.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-16 13:47:03.000000 django_import_export-4.0.3/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-16 13:47:03.000000 django_import_export-4.0.3/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-16 13:47:03.000000 django_import_export-4.0.3/.flake8
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-16 13:47:03.000000 django_import_export-4.0.3/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.506338 django_import_export-4.0.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-16 13:47:03.000000 django_import_export-4.0.3/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.506338 django_import_export-4.0.3/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-16 13:47:03.000000 django_import_export-4.0.3/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-16 13:47:03.000000 django_import_export-4.0.3/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-16 13:47:03.000000 django_import_export-4.0.3/.github/ISSUE_TEMPLATE/question.md
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-16 13:47:03.000000 django_import_export-4.0.3/.github/pull_request_template.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-05-16 13:47:03.000000 django_import_export-4.0.3/.github/stale.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.506338 django_import_export-4.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-16 13:47:03.000000 django_import_export-4.0.3/.github/workflows/pre-commit.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-05-16 13:47:03.000000 django_import_export-4.0.3/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2784 2024-05-16 13:47:03.000000 django_import_export-4.0.3/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-16 13:47:03.000000 django_import_export-4.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-16 13:47:03.000000 django_import_export-4.0.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-05-16 13:47:03.000000 django_import_export-4.0.3/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3815 2024-05-16 13:47:03.000000 django_import_export-4.0.3/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)     5547 2024-05-16 13:47:03.000000 django_import_export-4.0.3/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-16 13:47:03.000000 django_import_export-4.0.3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-05-16 13:47:03.000000 django_import_export-4.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-05-16 13:47:03.000000 django_import_export-4.0.3/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    11174 2024-05-16 13:47:07.546338 django_import_export-4.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7632 2024-05-16 13:47:03.000000 django_import_export-4.0.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-05-16 13:47:03.000000 django_import_export-4.0.3/RELEASE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-16 13:47:03.000000 django_import_export-4.0.3/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.546338 django_import_export-4.0.3/django_import_export.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11174 2024-05-16 13:47:07.000000 django_import_export-4.0.3/django_import_export.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10470 2024-05-16 13:47:07.000000 django_import_export-4.0.3/django_import_export.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 13:47:07.000000 django_import_export-4.0.3/django_import_export.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-16 13:47:07.000000 django_import_export-4.0.3/django_import_export.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-16 13:47:07.000000 django_import_export-4.0.3/django_import_export.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.510338 django_import_export-4.0.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     5621 2024-05-16 13:47:03.000000 django_import_export-4.0.3/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.494338 django_import_export-4.0.3/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.514338 django_import_export-4.0.3/docs/_static/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    21509 2024-05-16 13:47:03.000000 django_import_export-4.0.3/docs/_static/images/change-form-export.png
+-rw-r--r--   0 runner    (1001) docker     (127)    28966 2024-05-16 13:47:03.000000 django_import_export-4.0.3/docs/_static/images/custom-export-form.png
+-rw-r--r--   0 runner    (1001) docker     (127)    90059 2024-05-16 13:47:03.000000 django_import_export-4.0.3/docs/_static/images/custom-import-form.png
+-rw-r--r--   0 runner    (1001) docker     (127)    33092 2024-05-16 13:47:03.000000 django_import_export-4.0.3/docs/_static/images/date-widget-validation-error.png
+-rw-r--r--   0 runner    (1001) docker     (127)    30818 2024-05-16 13:47:03.000000 django_import_export-4.0.3/docs/_static/images/django-import-export-change.png
+-rw-r--r--   0 runner    (1001) docker     (127)    29191 2024-05-16 13:47:03.000000 django_import_export-4.0.3/docs/_static/images/django-import-export-export-confirm.png
+-rw-r--r--   0 runner    (1001) docker     (127)    35696 2024-05-16 13:47:03.000000 django_import_export-4.0.3/docs/_static/images/django-import-export-import-confirm.png
+-rw-r--r--   0 runner    (1001) docker     (127)    32366 2024-05-16 13:47:03.000000 django_import_export-4.0.3/docs/_static/images/django-import-export-import.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6097 2024-05-16 13:47:03.000000 django_import_export-4.0.3/docs/_static/images/export-button.png
+-rw-r--r--   0 runner    (1001) docker     (127)    33710 2024-05-16 13:47:03.000000 django_import_export-4.0.3/docs/_static/images/export_workflow.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     6047 2024-05-16 13:47:03.000000 django_import_export-4.0.3/docs/_static/images/import-button.png
+-rw-r--r--   0 runner    (1001) docker     (127)    56726 2024-05-16 13:47:03.000000 django_import_export-4.0.3/docs/_static/images/import_workflow.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    29758 2024-05-16 13:47:03.000000 django_import_export-4.0.3/docs/_static/images/non-field-specific-validation-error.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.518338 django_import_export-4.0.3/docs/_static/images/screenshots/
+-rw-r--r--   0 runner    (1001) docker     (127)   445502 2024-05-16 13:47:03.000000 django_import_export-4.0.3/docs/_static/images/screenshots/confirm-import.png
+-rw-r--r--   0 runner    (1001) docker     (127)   311653 2024-05-16 13:47:03.000000 django_import_export-4.0.3/docs/_static/images/screenshots/export-form.png
+-rw-r--r--   0 runner    (1001) docker     (127)   469577 2024-05-16 13:47:03.000000 django_import_export-4.0.3/docs/_static/images/screenshots/export-selected-action.png
+-rw-r--r--   0 runner    (1001) docker     (127)   447473 2024-05-16 13:47:03.000000 django_import_export-4.0.3/docs/_static/images/screenshots/import-complete.png
+-rw-r--r--   0 runner    (1001) docker     (127)   308805 2024-05-16 13:47:03.000000 django_import_export-4.0.3/docs/_static/images/screenshots/import-form.png
+-rw-r--r--   0 runner    (1001) docker     (127)   313540 2024-05-16 13:47:03.000000 django_import_export-4.0.3/docs/_static/images/screenshots/import-update-with-authors.png
+-rw-r--r--   0 runner    (1001) docker     (127)    17197 2024-05-16 13:47:03.000000 django_import_export-4.0.3/docs/_static/images/select-for-export.png
+-rw-r--r--   0 runner    (1001) docker     (127)    22131 2024-05-16 13:47:03.000000 django_import_export-4.0.3/docs/admin_integration.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    32484 2024-05-16 13:47:03.000000 django_import_export-4.0.3/docs/advanced_usage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-16 13:47:03.000000 django_import_export-4.0.3/docs/api_admin.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-16 13:47:03.000000 django_import_export-4.0.3/docs/api_exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-16 13:47:03.000000 django_import_export-4.0.3/docs/api_fields.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-16 13:47:03.000000 django_import_export-4.0.3/docs/api_forms.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-16 13:47:03.000000 django_import_export-4.0.3/docs/api_instance_loaders.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-05-16 13:47:03.000000 django_import_export-4.0.3/docs/api_mixins.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-16 13:47:03.000000 django_import_export-4.0.3/docs/api_resources.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-16 13:47:03.000000 django_import_export-4.0.3/docs/api_results.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-16 13:47:03.000000 django_import_export-4.0.3/docs/api_tmp_storages.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-16 13:47:03.000000 django_import_export-4.0.3/docs/api_widgets.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3421 2024-05-16 13:47:03.000000 django_import_export-4.0.3/docs/bulk_import.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-16 13:47:03.000000 django_import_export-4.0.3/docs/celery.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    59446 2024-05-16 13:47:03.000000 django_import_export-4.0.3/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-05-16 13:47:03.000000 django_import_export-4.0.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6284 2024-05-16 13:47:03.000000 django_import_export-4.0.3/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-05-16 13:47:03.000000 django_import_export-4.0.3/docs/export_workflow.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10518 2024-05-16 13:47:03.000000 django_import_export-4.0.3/docs/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4748 2024-05-16 13:47:03.000000 django_import_export-4.0.3/docs/getting_started.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.518338 django_import_export-4.0.3/docs/image_src/
+-rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-05-16 13:47:03.000000 django_import_export-4.0.3/docs/image_src/export_workflow.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3002 2024-05-16 13:47:03.000000 django_import_export-4.0.3/docs/image_src/import_workflow.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5713 2024-05-16 13:47:03.000000 django_import_export-4.0.3/docs/import_workflow.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-05-16 13:47:03.000000 django_import_export-4.0.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8438 2024-05-16 13:47:03.000000 django_import_export-4.0.3/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5126 2024-05-16 13:47:03.000000 django_import_export-4.0.3/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)    15410 2024-05-16 13:47:03.000000 django_import_export-4.0.3/docs/release_notes.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-05-16 13:47:03.000000 django_import_export-4.0.3/docs/screenshots.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2666 2024-05-16 13:47:03.000000 django_import_export-4.0.3/docs/testing.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.522338 django_import_export-4.0.3/import_export/
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-16 13:47:07.000000 django_import_export-4.0.3/import_export/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35711 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6467 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/declarative.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5643 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/fields.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.522338 django_import_export-4.0.3/import_export/formats/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/formats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6018 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/formats/base_formats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9649 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2089 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/instance_loaders.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.498338 django_import_export-4.0.3/import_export/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.494338 django_import_export-4.0.3/import_export/locale/ar/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.522338 django_import_export-4.0.3/import_export/locale/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5394 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/locale/ar/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.494338 django_import_export-4.0.3/import_export/locale/bg/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.522338 django_import_export-4.0.3/import_export/locale/bg/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/locale/bg/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5626 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/locale/bg/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.498338 django_import_export-4.0.3/import_export/locale/ca/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.522338 django_import_export-4.0.3/import_export/locale/ca/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/locale/ca/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5117 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/locale/ca/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.498338 django_import_export-4.0.3/import_export/locale/cs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.522338 django_import_export-4.0.3/import_export/locale/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/locale/cs/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5187 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/locale/cs/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.498338 django_import_export-4.0.3/import_export/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.522338 django_import_export-4.0.3/import_export/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2269 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5619 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.498338 django_import_export-4.0.3/import_export/locale/es/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.522338 django_import_export-4.0.3/import_export/locale/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5708 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.498338 django_import_export-4.0.3/import_export/locale/es_AR/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.522338 django_import_export-4.0.3/import_export/locale/es_AR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/locale/es_AR/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5712 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/locale/es_AR/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.498338 django_import_export-4.0.3/import_export/locale/fa/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.522338 django_import_export-4.0.3/import_export/locale/fa/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/locale/fa/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5726 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/locale/fa/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.498338 django_import_export-4.0.3/import_export/locale/fi/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.522338 django_import_export-4.0.3/import_export/locale/fi/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/locale/fi/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5140 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/locale/fi/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.498338 django_import_export-4.0.3/import_export/locale/fr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.522338 django_import_export-4.0.3/import_export/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5108 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.498338 django_import_export-4.0.3/import_export/locale/it/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.522338 django_import_export-4.0.3/import_export/locale/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/locale/it/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5067 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/locale/it/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.498338 django_import_export-4.0.3/import_export/locale/ja/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.526338 django_import_export-4.0.3/import_export/locale/ja/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/locale/ja/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5194 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/locale/ja/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.498338 django_import_export-4.0.3/import_export/locale/ko/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.526338 django_import_export-4.0.3/import_export/locale/ko/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/locale/ko/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5371 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/locale/ko/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.498338 django_import_export-4.0.3/import_export/locale/kz/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.526338 django_import_export-4.0.3/import_export/locale/kz/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/locale/kz/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5913 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/locale/kz/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.498338 django_import_export-4.0.3/import_export/locale/nl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.526338 django_import_export-4.0.3/import_export/locale/nl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/locale/nl/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5456 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/locale/nl/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.498338 django_import_export-4.0.3/import_export/locale/pl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.526338 django_import_export-4.0.3/import_export/locale/pl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/locale/pl/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5280 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/locale/pl/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.498338 django_import_export-4.0.3/import_export/locale/pt_BR/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.526338 django_import_export-4.0.3/import_export/locale/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/locale/pt_BR/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5405 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/locale/pt_BR/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.498338 django_import_export-4.0.3/import_export/locale/ru/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.526338 django_import_export-4.0.3/import_export/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     5198 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     7399 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.498338 django_import_export-4.0.3/import_export/locale/sk/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.526338 django_import_export-4.0.3/import_export/locale/sk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/locale/sk/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5113 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/locale/sk/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.498338 django_import_export-4.0.3/import_export/locale/tr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.526338 django_import_export-4.0.3/import_export/locale/tr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/locale/tr/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5465 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/locale/tr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.498338 django_import_export-4.0.3/import_export/locale/zh_Hans/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.526338 django_import_export-4.0.3/import_export/locale/zh_Hans/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/locale/zh_Hans/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     5238 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/locale/zh_Hans/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (127)     9665 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6543 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51173 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8079 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/results.py
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.498338 django_import_export-4.0.3/import_export/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.526338 django_import_export-4.0.3/import_export/static/import_export/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/static/import_export/export.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/static/import_export/export_selectable_fields.js
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/static/import_export/guess_format.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/static/import_export/import.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.498338 django_import_export-4.0.3/import_export/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.498338 django_import_export-4.0.3/import_export/templates/admin/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.530338 django_import_export-4.0.3/import_export/templates/admin/import_export/
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/templates/admin/import_export/base.html
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/templates/admin/import_export/change_form.html
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/templates/admin/import_export/change_list.html
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/templates/admin/import_export/change_list_export.html
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/templates/admin/import_export/change_list_export_item.html
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/templates/admin/import_export/change_list_import.html
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/templates/admin/import_export/change_list_import_export.html
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/templates/admin/import_export/change_list_import_item.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/templates/admin/import_export/export.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6686 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/templates/admin/import_export/import.html
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/templates/admin/import_export/resource_fields_list.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.530338 django_import_export-4.0.3/import_export/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/templatetags/import_export_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/tmp_storages.py
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21446 2024-05-16 13:47:03.000000 django_import_export-4.0.3/import_export/widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2109 2024-05-16 13:47:03.000000 django_import_export-4.0.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.530338 django_import_export-4.0.3/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-16 13:47:03.000000 django_import_export-4.0.3/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-16 13:47:03.000000 django_import_export-4.0.3/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-16 13:47:03.000000 django_import_export-4.0.3/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-05-16 13:47:03.000000 django_import_export-4.0.3/runtests.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      884 2024-05-16 13:47:03.000000 django_import_export-4.0.3/runtests.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 13:47:07.546338 django_import_export-4.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 13:47:03.000000 django_import_export-4.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.530338 django_import_export-4.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/books-sample.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.530338 django_import_export-4.0.3/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3475 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.534338 django_import_export-4.0.3/tests/core/exports/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/exports/authors.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/exports/books-ISO-8859-1.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/exports/books-dos.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     9650 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/exports/books-empty-author-email.xlsx
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/exports/books-for-delete.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/exports/books-invalid-date.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/exports/books-mac.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/exports/books-mac.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/exports/books-no-headers.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/exports/books-unicode.csv
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/exports/books-unicode.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/exports/books.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/exports/books.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5632 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/exports/books.xls
+-rw-r--r--   0 runner    (1001) docker     (127)     4886 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/exports/books.xlsx
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/exports/child.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.534338 django_import_export-4.0.3/tests/core/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/fixtures/author.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/fixtures/book.json
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/fixtures/category.json
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.538338 django_import_export-4.0.3/tests/core/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     5662 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/migrations/0002_book_published_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/migrations/0003_withfloatfield.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/migrations/0004_bookwithchapters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/migrations/0005_addparentchild.py
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/migrations/0006_auto_20171130_0147.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/migrations/0007_auto_20180628_0411.py
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/migrations/0008_auto_20190409_0846.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3131 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/migrations/0009_auto_20211111_0807.py
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/migrations/0010_uuidbook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/migrations/0011_uuidcategory_legacybook_alter_uuidbook_id_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/migrations/0012_delete_legacybook.py
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/migrations/0013_alter_author_birthday.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/migrations/0014_bookwithchapternumbers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/migrations/0015_withpositiveintegerfields.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5102 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.502338 django_import_export-4.0.3/tests/core/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.538338 django_import_export-4.0.3/tests/core/templates/core/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.538338 django_import_export-4.0.3/tests/core/templates/core/admin/
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/templates/core/admin/change_list.html
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/templates/core/category_list.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.538338 django_import_export-4.0.3/tests/core/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.542338 django_import_export-4.0.3/tests/core/tests/admin_integration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/tests/admin_integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/tests/admin_integration/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8435 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/tests/admin_integration/test_action_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20354 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/tests/admin_integration/test_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40988 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/tests/admin_integration/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/tests/admin_integration/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/tests/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8043 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/tests/test_base_formats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3706 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/tests/test_declarative.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5318 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/tests/test_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8776 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/tests/test_forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/tests/test_import_export_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/tests/test_instance_loaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/tests/test_invalidrow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14997 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/tests/test_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8133 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/tests/test_model_resource_fields_generate_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4622 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/tests/test_permissions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.542338 django_import_export-4.0.3/tests/core/tests/test_resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/tests/test_resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22130 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/tests/test_resources/test_bulk_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4295 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/tests/test_resources/test_diffs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16292 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/tests/test_resources/test_import_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/tests/test_resources/test_misc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.546338 django_import_export-4.0.3/tests/core/tests/test_resources/test_modelresource/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/tests/test_resources/test_modelresource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6300 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/tests/test_resources/test_modelresource/test_data_deletion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4626 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/tests/test_resources/test_modelresource/test_data_handling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5698 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/tests/test_resources/test_modelresource/test_data_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/tests/test_resources/test_modelresource/test_deprecated_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13486 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/tests/test_resources/test_modelresource/test_dynamic_customization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6718 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/tests/test_resources/test_modelresource/test_error_handling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2816 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/tests/test_resources/test_modelresource/test_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/tests/test_resources/test_modelresource/test_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5596 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/tests/test_resources/test_modelresource/test_m2m.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/tests/test_resources/test_modelresource/test_queryset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/tests/test_resources/test_modelresource/test_relationship.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3661 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/tests/test_resources/test_modelresource/test_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/tests/test_resources/test_modelresource/test_resource_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6083 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/tests/test_resources/test_modelresource/test_resource_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7346 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/tests/test_resources/test_modelresource/test_resource_postgres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2192 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/tests/test_resources/test_modelresource/test_resource_setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4598 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/tests/test_resources/test_modelresource/test_resource_transactions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/tests/test_resources/test_modelresource/test_string_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/tests/test_resources/test_modelresource/test_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/tests/test_resources/test_natural_foreign_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9679 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/tests/test_resources/test_relationships.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4651 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/tests/test_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5877 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/tests/test_tmp_storages.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26689 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/tests/test_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/tests/widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/core/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.502338 django_import_export-4.0.3/tests/docker/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.546338 django_import_export-4.0.3/tests/docker/db/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      146 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/docker/db/init-mysql-db.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      401 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/docker/db/init-postgres-db.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/docker-compose.yml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      320 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/manage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:07.546338 django_import_export-4.0.3/tests/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5341 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/scripts/bulk_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tests/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-05-16 13:47:03.000000 django_import_export-4.0.3/tox.ini
```

### Comparing `django_import_export-4.0.2/.github/ISSUE_TEMPLATE/bug_report.md` & `django_import_export-4.0.3/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/.github/ISSUE_TEMPLATE/question.md` & `django_import_export-4.0.3/.github/ISSUE_TEMPLATE/question.md`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/.github/stale.yml` & `django_import_export-4.0.3/.github/stale.yml`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/.github/workflows/release.yml` & `django_import_export-4.0.3/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/.github/workflows/test.yml` & `django_import_export-4.0.3/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/AUTHORS` & `django_import_export-4.0.3/AUTHORS`

 * *Files 2% similar despite different names*

```diff
@@ -147,7 +147,8 @@
 * ZibingZhang (Zibing Zhang)
 * Glay00 (Gleb Gorelov)
 * PrashansaChaudhary (Prashansa Chaudhary)
 * Vedang Barhate (bvedang)
 * RobTilton (Robert Tilton)
 * ulliholtgrave
 * mishka251 (Mikhail Belov)
+* jhthompson (Jeremy Thompson)
```

### Comparing `django_import_export-4.0.2/CODE_OF_CONDUCT.md` & `django_import_export-4.0.3/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/LICENSE` & `django_import_export-4.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/Makefile` & `django_import_export-4.0.3/Makefile`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 .PHONY: clean-pyc clean-build docs help
 .PHONY: lint test coverage test-codecov
 .DEFAULT_GOAL := help
-RUN_TEST_COMMAND=PYTHONPATH=".:tests:${PYTHONPATH}" django-admin test core --settings=settings
+RUN_TEST_COMMAND=PYTHONPATH=".:tests:${PYTHONPATH}" python -W error -m django test core --settings=settings
 help:
 	@grep '^[a-zA-Z]' $(MAKEFILE_LIST) | sort | awk -F ':.*?## ' 'NF==2 {printf "\033[36m  %-25s\033[0m %s\n", $$1, $$2}'
 
 clean: clean-build clean-pyc clean-tests
 
 clean-build: ## remove build artifacts
 	rm -fr build/
```

### Comparing `django_import_export-4.0.2/RELEASE.md` & `django_import_export-4.0.3/RELEASE.md`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/django_import_export.egg-info/SOURCES.txt` & `django_import_export-4.0.3/django_import_export.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -54,14 +54,15 @@
 docs/faq.rst
 docs/getting_started.rst
 docs/import_workflow.rst
 docs/index.rst
 docs/installation.rst
 docs/make.bat
 docs/release_notes.rst
+docs/screenshots.rst
 docs/testing.rst
 docs/_static/images/change-form-export.png
 docs/_static/images/custom-export-form.png
 docs/_static/images/custom-import-form.png
 docs/_static/images/date-widget-validation-error.png
 docs/_static/images/django-import-export-change.png
 docs/_static/images/django-import-export-export-confirm.png
@@ -69,14 +70,20 @@
 docs/_static/images/django-import-export-import.png
 docs/_static/images/export-button.png
 docs/_static/images/export_workflow.svg
 docs/_static/images/import-button.png
 docs/_static/images/import_workflow.svg
 docs/_static/images/non-field-specific-validation-error.png
 docs/_static/images/select-for-export.png
+docs/_static/images/screenshots/confirm-import.png
+docs/_static/images/screenshots/export-form.png
+docs/_static/images/screenshots/export-selected-action.png
+docs/_static/images/screenshots/import-complete.png
+docs/_static/images/screenshots/import-form.png
+docs/_static/images/screenshots/import-update-with-authors.png
 docs/image_src/export_workflow.txt
 docs/image_src/import_workflow.txt
 import_export/__init__.py
 import_export/_version.py
 import_export/admin.py
 import_export/declarative.py
 import_export/exceptions.py
```

### Comparing `django_import_export-4.0.2/docs/Makefile` & `django_import_export-4.0.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/docs/_static/images/change-form-export.png` & `django_import_export-4.0.3/docs/_static/images/change-form-export.png`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/docs/_static/images/custom-export-form.png` & `django_import_export-4.0.3/docs/_static/images/custom-export-form.png`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/docs/_static/images/custom-import-form.png` & `django_import_export-4.0.3/docs/_static/images/custom-import-form.png`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/docs/_static/images/date-widget-validation-error.png` & `django_import_export-4.0.3/docs/_static/images/date-widget-validation-error.png`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/docs/_static/images/django-import-export-change.png` & `django_import_export-4.0.3/docs/_static/images/django-import-export-change.png`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/docs/_static/images/django-import-export-export-confirm.png` & `django_import_export-4.0.3/docs/_static/images/django-import-export-export-confirm.png`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/docs/_static/images/django-import-export-import-confirm.png` & `django_import_export-4.0.3/docs/_static/images/django-import-export-import-confirm.png`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/docs/_static/images/django-import-export-import.png` & `django_import_export-4.0.3/docs/_static/images/django-import-export-import.png`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/docs/_static/images/export-button.png` & `django_import_export-4.0.3/docs/_static/images/export-button.png`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/docs/_static/images/export_workflow.svg` & `django_import_export-4.0.3/docs/_static/images/export_workflow.svg`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/docs/_static/images/import-button.png` & `django_import_export-4.0.3/docs/_static/images/import-button.png`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/docs/_static/images/import_workflow.svg` & `django_import_export-4.0.3/docs/_static/images/import_workflow.svg`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/docs/_static/images/non-field-specific-validation-error.png` & `django_import_export-4.0.3/docs/_static/images/non-field-specific-validation-error.png`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/docs/_static/images/select-for-export.png` & `django_import_export-4.0.3/docs/_static/images/select-for-export.png`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/docs/admin_integration.rst` & `django_import_export-4.0.3/docs/admin_integration.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+.. _admin-integration:
+
 =================
 Admin integration
 =================
 
 One of the main features of import-export is the support for integration with the
 `Django Admin site <https://docs.djangoproject.com/en/stable/ref/contrib/admin/>`_.
 This provides a convenient interface for importing and exporting Django objects.
```

### Comparing `django_import_export-4.0.2/docs/advanced_usage.rst` & `django_import_export-4.0.3/docs/advanced_usage.rst`

 * *Files 6% similar despite different names*

```diff
@@ -573,14 +573,56 @@
 
 .. note::
 
     If setting ``import_id_fields``, you must ensure that the data can uniquely identify a single row.  If the chosen
     field(s) select more than one row, then a ``MultipleObjectsReturned`` exception will be raised.  If no row is
     identified, then ``DoesNotExist`` exception will be raised.
 
+.. _dynamic_fields:
+
+Using 'dynamic fields' to identify existing instances
+-----------------------------------------------------
+
+There are some use-cases where a field defined in ``import_id_fields`` is not present in the dataset.  An example of
+this would be dynamic fields, where a field is generated from other data and then used as an identifier.  For example::
+
+    class BookResource(resources.ModelResource):
+
+        def before_import_row(self, row, **kwargs):
+            # generate a value for an existing field, based on another field
+            row["hash_id"] = hashlib.sha256(row["name"].encode()).hexdigest()
+
+        class Meta:
+            model = Book
+            # A 'dynamic field' - i.e. is used to identify existing rows
+            # but is not present in the dataset
+            import_id_fields = ("hash_id",)
+
+In the above example, a dynamic field called *hash_id* is generated and added to the dataset.  In this example, an
+error will be raised because *hash_id* is not present in the dataset.  To resolve this, update the dataset before
+import to add the dynamic field as a header::
+
+    class BookResource(resources.ModelResource):
+
+        def before_import(self, dataset, **kwargs):
+            # mimic a 'dynamic field' - i.e. append field which exists on
+            # Book model, but not in dataset
+            dataset.headers.append("hash_id")
+            super().before_import(dataset, **kwargs)
+
+        def before_import_row(self, row, **kwargs):
+            row["hash_id"] = hashlib.sha256(row["name"].encode()).hexdigest()
+
+        class Meta:
+            model = Book
+            # A 'dynamic field' - i.e. is used to identify existing rows
+            # but is not present in the dataset
+            import_id_fields = ("hash_id",)
+
+
 Access instances after import
 =============================
 
 Access instance summary data
 ----------------------------
 
 The instance pk and representation (i.e. output from ``repr()``) can be accessed after import::
```

### Comparing `django_import_export-4.0.2/docs/api_mixins.rst` & `django_import_export-4.0.3/docs/api_mixins.rst`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/docs/api_widgets.rst` & `django_import_export-4.0.3/docs/api_widgets.rst`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/docs/bulk_import.rst` & `django_import_export-4.0.3/docs/bulk_import.rst`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/docs/changelog.rst` & `django_import_export-4.0.3/docs/changelog.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,23 @@
 Changelog
 =========
 
 .. warning::
 
     Version 4 introduces breaking changes.  Please refer to :doc:`release notes<release_notes>`.
 
+4.0.3 (2024-05-16)
+------------------
+
+- Support widgets with CSS and JS media in ImportForm (`1807 <https://github.com/django-import-export/django-import-export/pull/1807>`_)
+- Documentation updates (`1833 <https://github.com/django-import-export/django-import-export/pull/1833>`_)
+- Clarified documentation when importing with ``import_id_fields``  (`1836 <https://github.com/django-import-export/django-import-export/pull/1836>`_)
+- re-add ``resource_class`` deprecation warning (`1837 <https://github.com/django-import-export/django-import-export/pull/1837>`_)
+- fixed Arabic translation for 'import' word (`1838 <https://github.com/django-import-export/django-import-export/pull/1838>`_)
+
 4.0.2 (2024-05-13)
 ------------------
 
 - fix export with custom column name (`1821 <https://github.com/django-import-export/django-import-export/pull/1821>`_)
 - fix allow ``column_name`` to be declared in ``fields`` list (`1822 <https://github.com/django-import-export/django-import-export/pull/1822>`_)
 - fix clash between ``key_is_id`` and ``use_natural_foreign_keys`` (`1824 <https://github.com/django-import-export/django-import-export/pull/1824>`_)
 - remove unreachable code (`1825 <https://github.com/django-import-export/django-import-export/pull/1825>`_)
```

### Comparing `django_import_export-4.0.2/docs/conf.py` & `django_import_export-4.0.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/docs/contributing.rst` & `django_import_export-4.0.3/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/docs/export_workflow.rst` & `django_import_export-4.0.3/docs/export_workflow.rst`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/docs/faq.rst` & `django_import_export-4.0.3/docs/faq.rst`

 * *Files 4% similar despite different names*

```diff
@@ -13,40 +13,44 @@
 
 We welcome contributions from the community.
 
 You can help in the following ways:
 
 * Reporting bugs or issues.
 
-* Answering questions which arise on Stack Overflow or as Github issues.
+* Answering questions which arise on `Stack Overflow <https://stackoverflow.com/questions/tagged/django-import-export/>`_ or as Github issues.
 
 * Providing translations for UI text.
 
 * Suggesting features or changes.
 
 We encourage you to read the :doc:`contributing guidelines <contributing>`.
 
 .. _common_issues:
 
 Common issues
 =============
 
-FieldError on import
---------------------
+.. _import_id_fields_error_on_import:
+
+``import_id_fields`` error on import
+------------------------------------
 
 The following error message can be seen on import:
 
   *The following fields are declared in 'import_id_fields' but are not present in the resource*
 
 This indicates that the Resource has not been configured correctly, and the import logic fails.  Specifically,
 the import process is attempting to use either the defined or default values for
 :attr:`~import_export.options.ResourceOptions.import_id_fields` and no matching field has been detected in the resource
-fields.
+fields. See :ref:`advanced_usage:Create or update model instances`.
 
-See :ref:`advanced_usage:Create or update model instances`.
+In cases where you are deliberately using generated fields in ``import_id_fields`` and these fields are not present in
+the dataset, then you need to modify the resource definition to accommodate this.
+See :ref:`dynamic_fields`.
 
 How to handle double-save from Signals
 --------------------------------------
 
 This issue can apply if you have implemented post-save :ref:`advanced_usage:signals`, and you are using the import workflow in the Admin
 interface.  You will find that the post-save signal is called twice for each instance.  The reason for this is that
 the model ``save()`` method is called twice: once for the 'confirm' step and once for the 'import' step.  The call
@@ -163,16 +167,15 @@
 
 See :ref:`advanced_usage:Creating non existent relations`.
 
 How to handle large file uploads
 ---------------------------------
 
 If uploading large files, you may encounter time-outs.
-See :ref:`Celery:Using celery to perform imports` and :ref:`bulk_import:Bulk imports`.
-
+See :ref:`Using celery<celery>` and :ref:`bulk_import:Bulk imports`.
 
 How to use field other than `id` in Foreign Key lookup
 ------------------------------------------------------
 
 See :ref:`advanced_usage:Foreign key relations`.
 
 ``RelatedObjectDoesNotExist`` exception during import
@@ -235,7 +238,12 @@
       for i, h in enumerate(headers):
           if h == 'name':
             headers[i] = "NEW COLUMN NAME"
       return headers
 
     class Meta:
       model = Book
+
+How to configure logging
+------------------------
+
+Refer to :ref:`logging configuration<logging>` for more information.
```

### Comparing `django_import_export-4.0.2/docs/getting_started.rst` & `django_import_export-4.0.3/docs/getting_started.rst`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/docs/image_src/export_workflow.txt` & `django_import_export-4.0.3/docs/image_src/export_workflow.txt`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/docs/image_src/import_workflow.txt` & `django_import_export-4.0.3/docs/image_src/import_workflow.txt`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/docs/import_workflow.rst` & `django_import_export-4.0.3/docs/import_workflow.rst`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/docs/index.rst` & `django_import_export-4.0.3/docs/index.rst`

 * *Files 10% similar despite different names*

```diff
@@ -41,14 +41,15 @@
    admin_integration
    import_workflow
    export_workflow
    bulk_import
    celery
    testing
    faq
+   screenshots
    release_notes
    changelog
 
 .. toctree::
    :maxdepth: 2
    :caption: API documentation
```

### Comparing `django_import_export-4.0.2/docs/installation.rst` & `django_import_export-4.0.3/docs/installation.rst`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 `tablib documentation <https://tablib.readthedocs.io/en/stable/formats.html>`_.
 
 Alternatively, you can install the git repository directly to obtain the
 development version::
 
   pip install -e git+https://github.com/django-import-export/django-import-export.git#egg=django-import-export
 
-Now, you're good to go, unless you want to use import_export from the
+Now, you're good to go, unless you want to use import-export from the
 admin as well. In this case, you need to add it to your ``INSTALLED_APPS`` and
 let Django collect its static files.
 
 .. code-block:: python
 
     # settings.py
     INSTALLED_APPS = (
@@ -235,7 +235,29 @@
     ./manage.py createsuperuser
     ./manage.py loaddata author.json category.json book.json
     ./manage.py runserver
 
 Go to http://127.0.0.1:8000
 
 For example import files, see :ref:`getting_started:Test data`.
+
+.. _logging:
+
+Configure logging
+=================
+
+You can adjust the log level to see output as required.
+This is an example configuration to be placed in your application settings::
+
+    LOGGING = {
+        "handlers": {
+            "console": {"level": "DEBUG", "class": "logging.StreamHandler"},
+        },
+        "loggers": {
+            "django.db.backends": {"level": "INFO", "handlers": ["console"]},
+            "import_export": {
+                "handlers": ["console"],
+                "level": "INFO",
+            },
+        },
+    }
+
```

### Comparing `django_import_export-4.0.2/docs/make.bat` & `django_import_export-4.0.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/docs/release_notes.rst` & `django_import_export-4.0.3/docs/release_notes.rst`

 * *Files 2% similar despite different names*

```diff
@@ -65,14 +65,23 @@
 ------------
 
 If the ``raise_errors`` parameter of :meth:`~import_export.resources.Resource.import_data` is ``True``, then an instance
 of :class:`~import_export.exceptions.ImportError` is raised.  This exception wraps the underlying exception.
 
 See `this PR <https://github.com/django-import-export/django-import-export/issues/1729>`_.
 
+Check ``import_id_fields``
+--------------------------
+
+Prior to v4 we had numerous issues where users were confused when imports failed due to declared ``import_id_fields``
+not being present in the dataset.  We added functionality in v4 to check for this and to raise a clearer error message.
+
+In some use-cases, it is a requirement that ``import_id_fields`` are not in the dataset, and are generated dynamically.
+If this affects your implementation, start with the documentation :ref:`here<import_id_fields_error_on_import>`.
+
 Deprecations
 ============
 
 * The ``obj`` param passed to :meth:`~import_export.widgets.Widget.render` is deprecated.
   The :meth:`~import_export.widgets.Widget.render` method should not need to have a reference to
   model instance.
   The call to :meth:`~import_export.widgets.Widget.render` from :meth:`~import_export.fields.Field.export` has been removed.
```

### Comparing `django_import_export-4.0.2/docs/testing.rst` & `django_import_export-4.0.3/docs/testing.rst`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 
   # pass 'create', 'update' or 'delete' to run the single test
   ./manage.py runscript bulk_import --script-args create
 
 Enable logging
 ^^^^^^^^^^^^^^
 
-You can see console debug logging by updating the ``LOGGING`` block in `settings.py`::
+You can see console SQL debug logging by updating the ``LOGGING`` block in `settings.py`::
 
     LOGGING = {
         "version": 1,
         "handlers": {"console": {"class": "logging.StreamHandler"}},
         "root": {
             "handlers": ["console"],
         },
```

### Comparing `django_import_export-4.0.2/import_export/admin.py` & `django_import_export-4.0.3/import_export/admin.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/import_export/declarative.py` & `django_import_export-4.0.3/import_export/declarative.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/import_export/exceptions.py` & `django_import_export-4.0.3/import_export/exceptions.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/import_export/fields.py` & `django_import_export-4.0.3/import_export/fields.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/import_export/formats/base_formats.py` & `django_import_export-4.0.3/import_export/formats/base_formats.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/import_export/forms.py` & `django_import_export-4.0.3/import_export/forms.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,16 +66,17 @@
         super().__init__(formats, resources, **kwargs)
         if len(formats) > 1:
             self.fields["import_file"].widget.attrs["class"] = "guess_format"
             self.fields["format"].widget.attrs["class"] = "guess_format"
 
     @property
     def media(self):
+        media = super().media
         extra = "" if settings.DEBUG else ".min"
-        return forms.Media(
+        return media + forms.Media(
             js=(
                 f"admin/js/vendor/jquery/jquery{extra}.js",
                 "admin/js/jquery.init.js",
                 "import_export/guess_format.js",
             )
         )
```

### Comparing `django_import_export-4.0.2/import_export/instance_loaders.py` & `django_import_export-4.0.3/import_export/instance_loaders.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/import_export/locale/ar/LC_MESSAGES/django.mo` & `django_import_export-4.0.3/import_export/locale/ar/LC_MESSAGES/django.mo`

 * *Files 2% similar despite different names*

#### msgunfmt {}

```diff
@@ -40,15 +40,15 @@
 msgid "Format"
 msgstr "تنسيق"
 
 msgid "Home"
 msgstr "الرئيسية"
 
 msgid "Import"
-msgstr "إستبراد"
+msgstr "إستيراد"
 
 msgid "Line number"
 msgstr "رقم الصطر"
 
 msgid "New"
 msgstr "جديد"
```

### Comparing `django_import_export-4.0.2/import_export/locale/ar/LC_MESSAGES/django.po` & `django_import_export-4.0.3/import_export/locale/ar/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 "%(exc_name)s encountered while trying to read file. Ensure you have chosen "
 "the correct format for the file."
 msgstr ""
 
 #: admin.py:539 templates/admin/import_export/change_list_import_item.html:5
 #: templates/admin/import_export/import.html:19
 msgid "Import"
-msgstr "إستبراد"
+msgstr "إستيراد"
 
 #: admin.py:785 templates/admin/import_export/change_form.html:8
 #: templates/admin/import_export/change_list_export_item.html:5
 #: templates/admin/import_export/export.html:12
 msgid "Export"
 msgstr "تصدير"
```

### Comparing `django_import_export-4.0.2/import_export/locale/bg/LC_MESSAGES/django.mo` & `django_import_export-4.0.3/import_export/locale/bg/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/import_export/locale/bg/LC_MESSAGES/django.po` & `django_import_export-4.0.3/import_export/locale/bg/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/import_export/locale/ca/LC_MESSAGES/django.mo` & `django_import_export-4.0.3/import_export/locale/ca/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/import_export/locale/ca/LC_MESSAGES/django.po` & `django_import_export-4.0.3/import_export/locale/ca/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/import_export/locale/cs/LC_MESSAGES/django.mo` & `django_import_export-4.0.3/import_export/locale/cs/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/import_export/locale/cs/LC_MESSAGES/django.po` & `django_import_export-4.0.3/import_export/locale/cs/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/import_export/locale/de/LC_MESSAGES/django.mo` & `django_import_export-4.0.3/import_export/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/import_export/locale/de/LC_MESSAGES/django.po` & `django_import_export-4.0.3/import_export/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/import_export/locale/es/LC_MESSAGES/django.mo` & `django_import_export-4.0.3/import_export/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/import_export/locale/es/LC_MESSAGES/django.po` & `django_import_export-4.0.3/import_export/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/import_export/locale/es_AR/LC_MESSAGES/django.mo` & `django_import_export-4.0.3/import_export/locale/es_AR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/import_export/locale/es_AR/LC_MESSAGES/django.po` & `django_import_export-4.0.3/import_export/locale/es_AR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/import_export/locale/fa/LC_MESSAGES/django.mo` & `django_import_export-4.0.3/import_export/locale/fa/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/import_export/locale/fa/LC_MESSAGES/django.po` & `django_import_export-4.0.3/import_export/locale/fa/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/import_export/locale/fi/LC_MESSAGES/django.mo` & `django_import_export-4.0.3/import_export/locale/fi/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/import_export/locale/fi/LC_MESSAGES/django.po` & `django_import_export-4.0.3/import_export/locale/fi/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/import_export/locale/fr/LC_MESSAGES/django.mo` & `django_import_export-4.0.3/import_export/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/import_export/locale/fr/LC_MESSAGES/django.po` & `django_import_export-4.0.3/import_export/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/import_export/locale/it/LC_MESSAGES/django.mo` & `django_import_export-4.0.3/import_export/locale/it/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/import_export/locale/it/LC_MESSAGES/django.po` & `django_import_export-4.0.3/import_export/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/import_export/locale/ja/LC_MESSAGES/django.mo` & `django_import_export-4.0.3/import_export/locale/ja/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/import_export/locale/ja/LC_MESSAGES/django.po` & `django_import_export-4.0.3/import_export/locale/ja/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/import_export/locale/ko/LC_MESSAGES/django.mo` & `django_import_export-4.0.3/import_export/locale/ko/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/import_export/locale/ko/LC_MESSAGES/django.po` & `django_import_export-4.0.3/import_export/locale/ko/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/import_export/locale/kz/LC_MESSAGES/django.mo` & `django_import_export-4.0.3/import_export/locale/kz/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/import_export/locale/kz/LC_MESSAGES/django.po` & `django_import_export-4.0.3/import_export/locale/kz/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/import_export/locale/nl/LC_MESSAGES/django.mo` & `django_import_export-4.0.3/import_export/locale/nl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/import_export/locale/nl/LC_MESSAGES/django.po` & `django_import_export-4.0.3/import_export/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/import_export/locale/pl/LC_MESSAGES/django.mo` & `django_import_export-4.0.3/import_export/locale/pl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/import_export/locale/pl/LC_MESSAGES/django.po` & `django_import_export-4.0.3/import_export/locale/pl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/import_export/locale/pt_BR/LC_MESSAGES/django.mo` & `django_import_export-4.0.3/import_export/locale/pt_BR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/import_export/locale/pt_BR/LC_MESSAGES/django.po` & `django_import_export-4.0.3/import_export/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/import_export/locale/ru/LC_MESSAGES/django.mo` & `django_import_export-4.0.3/import_export/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/import_export/locale/ru/LC_MESSAGES/django.po` & `django_import_export-4.0.3/import_export/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/import_export/locale/sk/LC_MESSAGES/django.mo` & `django_import_export-4.0.3/import_export/locale/sk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/import_export/locale/sk/LC_MESSAGES/django.po` & `django_import_export-4.0.3/import_export/locale/sk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/import_export/locale/tr/LC_MESSAGES/django.mo` & `django_import_export-4.0.3/import_export/locale/tr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/import_export/locale/tr/LC_MESSAGES/django.po` & `django_import_export-4.0.3/import_export/locale/tr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/import_export/locale/zh_Hans/LC_MESSAGES/django.mo` & `django_import_export-4.0.3/import_export/locale/zh_Hans/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/import_export/locale/zh_Hans/LC_MESSAGES/django.po` & `django_import_export-4.0.3/import_export/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/import_export/mixins.py` & `django_import_export-4.0.3/import_export/mixins.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import logging
+import warnings
 from warnings import warn
 
 from django.conf import settings
 from django.http import HttpResponse
 from django.utils.timezone import now
 from django.views.generic.edit import FormView
 
@@ -16,14 +17,15 @@
 
 class BaseImportExportMixin:
     """
     Base mixin for functionality related to importing and exporting via the Admin
     interface.
     """
 
+    resource_class = None
     resource_classes = []
 
     @property
     def formats(self):
         return getattr(settings, "IMPORT_EXPORT_FORMATS", base_formats.DEFAULT_FORMATS)
 
     @property
@@ -43,19 +45,38 @@
 
     def get_resource_classes(self, request):
         """
         Return subscriptable type (list, tuple, ...) containing resource classes
         :param request: The request object.
         :returns: The Resource classes.
         """
-        if not self.resource_classes:
+        if self.resource_classes and self.resource_class:
+            raise Exception(
+                "Only one of 'resource_class' and 'resource_classes' can be set"
+            )
+        if hasattr(self, "get_resource_class"):
+            warnings.warn(
+                "The 'get_resource_class()' method has been deprecated. "
+                "Please implement the new 'get_resource_classes()' method",
+                DeprecationWarning,
+            )
+            return [self.get_resource_class()]
+        if self.resource_class:
+            warnings.warn(
+                "The 'resource_class' field has been deprecated. "
+                "Please implement the new 'resource_classes' field",
+                DeprecationWarning,
+            )
+        if not self.resource_classes and not self.resource_class:
             return [modelresource_factory(self.model)]
-        return self.resource_classes
+        if self.resource_classes:
+            return self.resource_classes
+        return [self.resource_class]
 
-    def get_resource_kwargs(self, request, **kwargs):
+    def get_resource_kwargs(self, request, *args, **kwargs):
         """
         Return the kwargs which are to be passed to the Resource constructor.
         Can be overridden to provide additional kwarg params.
 
         :param request: The request object.
         :param kwargs: Keyword arguments.
         :returns: The Resource kwargs (by default, is the kwargs passed).
@@ -80,14 +101,21 @@
 
 class BaseImportMixin(BaseImportExportMixin):
     def get_import_resource_classes(self, request):
         """
         :param request: The request object.
         Returns ResourceClass subscriptable (list, tuple, ...) to use for import.
         """
+        if hasattr(self, "get_import_resource_class"):
+            warnings.warn(
+                "The 'get_import_resource_class()' method has been deprecated. "
+                "Please implement the new 'get_import_resource_classes()' method",
+                DeprecationWarning,
+            )
+            return [self.get_import_resource_class()]
         resource_classes = self.get_resource_classes(request)
         self.check_resource_classes(resource_classes)
         return resource_classes
 
     def get_import_formats(self):
         """
         Returns available import formats.
@@ -125,14 +153,21 @@
 
     def get_export_resource_classes(self, request):
         """
         Returns ResourceClass subscriptable (list, tuple, ...) to use for export.
         :param request: The request object.
         :returns: The Resource classes.
         """
+        if hasattr(self, "get_export_resource_class"):
+            warnings.warn(
+                "The 'get_export_resource_class()' method has been deprecated. "
+                "Please implement the new 'get_export_resource_classes()' method",
+                DeprecationWarning,
+            )
+            return [self.get_export_resource_class()]
         resource_classes = self.get_resource_classes(request)
         self.check_resource_classes(resource_classes)
         return resource_classes
 
     def choose_export_resource_class(self, form, request):
         """
         Identify which class should be used for export
```

### Comparing `django_import_export-4.0.2/import_export/options.py` & `django_import_export-4.0.3/import_export/options.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/import_export/resources.py` & `django_import_export-4.0.3/import_export/resources.py`

 * *Files 0% similar despite different names*

```diff
@@ -1149,14 +1149,21 @@
     def _is_using_transactions(self, kwargs):
         return kwargs.get("using_transactions", False)
 
     def _is_dry_run(self, kwargs):
         return kwargs.get("dry_run", False)
 
     def _check_import_id_fields(self, headers):
+        """
+        Provides a safety check with a meaningful error message for cases where
+        the ``import_id_fields`` declaration contains a field which is not in the
+        dataset.  For most use-cases this is an error, so we detect and raise.
+        There are conditions, such as 'dynamic fields' where this does not apply.
+        See issue 1834 for more information.
+        """
         import_id_fields = list()
         missing_fields = list()
         missing_headers = list()
 
         if self.get_import_id_fields() == ["id"]:
             # this is the default case, so ok if not present
             return
```

### Comparing `django_import_export-4.0.2/import_export/results.py` & `django_import_export-4.0.3/import_export/results.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/import_export/static/import_export/export_selectable_fields.js` & `django_import_export-4.0.3/import_export/static/import_export/export_selectable_fields.js`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/import_export/static/import_export/guess_format.js` & `django_import_export-4.0.3/import_export/static/import_export/guess_format.js`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/import_export/static/import_export/import.css` & `django_import_export-4.0.3/import_export/static/import_export/import.css`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/import_export/templates/admin/import_export/base.html` & `django_import_export-4.0.3/import_export/templates/admin/import_export/base.html`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/import_export/templates/admin/import_export/export.html` & `django_import_export-4.0.3/import_export/templates/admin/import_export/export.html`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/import_export/templates/admin/import_export/import.html` & `django_import_export-4.0.3/import_export/templates/admin/import_export/import.html`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/import_export/templates/admin/import_export/resource_fields_list.html` & `django_import_export-4.0.3/import_export/templates/admin/import_export/resource_fields_list.html`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/import_export/tmp_storages.py` & `django_import_export-4.0.3/import_export/tmp_storages.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/import_export/utils.py` & `django_import_export-4.0.3/import_export/utils.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/import_export/widgets.py` & `django_import_export-4.0.3/import_export/widgets.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/pyproject.toml` & `django_import_export-4.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/runtests.py` & `django_import_export-4.0.3/runtests.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/runtests.sh` & `django_import_export-4.0.3/runtests.sh`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/tests/core/admin.py` & `django_import_export-4.0.3/tests/core/admin.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/tests/core/exports/books-empty-author-email.xlsx` & `django_import_export-4.0.3/tests/core/exports/books-empty-author-email.xlsx`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/tests/core/exports/books.json` & `django_import_export-4.0.3/tests/core/exports/books.json`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/tests/core/exports/books.xls` & `django_import_export-4.0.3/tests/core/exports/books.xls`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/tests/core/exports/books.xlsx` & `django_import_export-4.0.3/tests/core/exports/books.xlsx`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/tests/core/fixtures/book.json` & `django_import_export-4.0.3/tests/core/fixtures/book.json`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/tests/core/forms.py` & `django_import_export-4.0.3/tests/core/forms.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/tests/core/migrations/0001_initial.py` & `django_import_export-4.0.3/tests/core/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/tests/core/migrations/0003_withfloatfield.py` & `django_import_export-4.0.3/tests/core/migrations/0003_withfloatfield.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/tests/core/migrations/0004_bookwithchapters.py` & `django_import_export-4.0.3/tests/core/migrations/0004_bookwithchapters.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/tests/core/migrations/0005_addparentchild.py` & `django_import_export-4.0.3/tests/core/migrations/0005_addparentchild.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/tests/core/migrations/0007_auto_20180628_0411.py` & `django_import_export-4.0.3/tests/core/migrations/0007_auto_20180628_0411.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/tests/core/migrations/0008_auto_20190409_0846.py` & `django_import_export-4.0.3/tests/core/migrations/0008_auto_20190409_0846.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/tests/core/migrations/0009_auto_20211111_0807.py` & `django_import_export-4.0.3/tests/core/migrations/0009_auto_20211111_0807.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/tests/core/migrations/0010_uuidbook.py` & `django_import_export-4.0.3/tests/core/migrations/0010_uuidbook.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/tests/core/migrations/0011_uuidcategory_legacybook_alter_uuidbook_id_and_more.py` & `django_import_export-4.0.3/tests/core/migrations/0011_uuidcategory_legacybook_alter_uuidbook_id_and_more.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/tests/core/migrations/0014_bookwithchapternumbers.py` & `django_import_export-4.0.3/tests/core/migrations/0014_bookwithchapternumbers.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/tests/core/migrations/0015_withpositiveintegerfields.py` & `django_import_export-4.0.3/tests/core/migrations/0015_withpositiveintegerfields.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/tests/core/models.py` & `django_import_export-4.0.3/tests/core/models.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/tests/core/tests/admin_integration/mixins.py` & `django_import_export-4.0.3/tests/core/tests/admin_integration/mixins.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/tests/core/tests/admin_integration/test_action_export.py` & `django_import_export-4.0.3/tests/core/tests/admin_integration/test_action_export.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/tests/core/tests/admin_integration/test_export.py` & `django_import_export-4.0.3/tests/core/tests/admin_integration/test_export.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/tests/core/tests/admin_integration/test_import.py` & `django_import_export-4.0.3/tests/core/tests/admin_integration/test_import.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/tests/core/tests/admin_integration/test_views.py` & `django_import_export-4.0.3/tests/core/tests/admin_integration/test_views.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/tests/core/tests/resources.py` & `django_import_export-4.0.3/tests/core/tests/resources.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/tests/core/tests/test_base_formats.py` & `django_import_export-4.0.3/tests/core/tests/test_base_formats.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/tests/core/tests/test_declarative.py` & `django_import_export-4.0.3/tests/core/tests/test_declarative.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/tests/core/tests/test_fields.py` & `django_import_export-4.0.3/tests/core/tests/test_fields.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/tests/core/tests/test_forms.py` & `django_import_export-4.0.3/tests/core/tests/test_forms.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import django.forms
+from core.models import Author
 from django.test import TestCase
 
 from import_export import forms, resources
 from import_export.formats.base_formats import CSV
 
 from .resources import BookResource, BookResourceWithStoreInstance
 
@@ -29,14 +30,67 @@
         form = forms.ImportExportFormBase([CSV], resource_list)
         self.assertEqual(
             form.fields["resource"].choices,
             [(0, "ModelResource"), (1, "My super resource")],
         )
 
 
+class ImportFormMediaTest(TestCase):
+    def test_import_form_media(self):
+        form = forms.ImportForm([CSV], [MyResource])
+        media = form.media
+        self.assertEqual(
+            media._css,
+            {},
+        )
+        self.assertEqual(
+            media._js,
+            [
+                "admin/js/vendor/jquery/jquery.min.js",
+                "admin/js/jquery.init.js",
+                "import_export/guess_format.js",
+            ],
+        )
+
+    def test_import_form_and_custom_widget_media(self):
+        class TestMediaWidget(django.forms.TextInput):
+            """Dummy test widget with associated CSS and JS media."""
+
+            class Media:
+                css = {
+                    "all": ["test.css"],
+                }
+                js = ["test.js"]
+
+        class CustomImportForm(forms.ImportForm):
+            """Dummy custom import form with a custom widget."""
+
+            author = django.forms.ModelChoiceField(
+                queryset=Author.objects.none(),
+                required=True,
+                widget=TestMediaWidget,
+            )
+
+        form = CustomImportForm([CSV], [MyResource])
+        media = form.media
+        self.assertEqual(
+            media._css,
+            {"all": ["test.css"]},
+        )
+        self.assertEqual(
+            media._js,
+            [
+                "test.js",
+                "admin/js/vendor/jquery/jquery.min.js",
+                "admin/js/jquery.init.js",
+                "import_export/guess_format.js",
+            ],
+        )
+
+
 class SelectableFieldsExportFormTest(TestCase):
     @classmethod
     def setUpTestData(cls) -> None:
         cls.resources = (BookResource, BookResourceWithStoreInstance)
         cls.form = forms.SelectableFieldsExportForm(
             formats=(CSV,),
             resources=cls.resources,
```

### Comparing `django_import_export-4.0.2/tests/core/tests/test_instance_loaders.py` & `django_import_export-4.0.3/tests/core/tests/test_instance_loaders.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/tests/core/tests/test_invalidrow.py` & `django_import_export-4.0.3/tests/core/tests/test_invalidrow.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/tests/core/tests/test_mixins.py` & `django_import_export-4.0.3/tests/core/tests/test_mixins.py`

 * *Files 22% similar despite different names*

```diff
@@ -178,14 +178,70 @@
         self.assertEqual(1, admin.call_count)
 
     def test_get_export_resource_kwargs_calls_self_get_resource_kwargs(self):
         admin = self.BaseExportModelAdminTest()
         admin.get_export_resource_kwargs(self.request)
         self.assertEqual(1, admin.call_count)
 
+    class BaseModelResourceClassTest(mixins.BaseImportMixin, mixins.BaseExportMixin):
+        resource_class = resources.Resource
+        export_call_count = 0
+        import_call_count = 0
+
+        def get_export_resource_class(self):
+            self.export_call_count += 1
+
+        def get_import_resource_class(self):
+            self.import_call_count += 1
+
+    def test_deprecated_resource_class_raises_warning(self):
+        """Test that the mixin throws error if user didn't
+        migrate to resource_classes"""
+        admin = self.BaseModelResourceClassTest()
+        with self.assertWarnsRegex(
+            DeprecationWarning,
+            r"^The 'get_export_resource_class\(\)' method has been deprecated. "
+            r"Please implement the new 'get_export_resource_classes\(\)' method$",
+        ):
+            admin.get_export_resource_classes(self.request)
+
+        with self.assertWarnsRegex(
+            DeprecationWarning,
+            r"^The 'get_import_resource_class\(\)' method has been deprecated. "
+            r"Please implement the new 'get_import_resource_classes\(\)' method$",
+        ):
+            admin.get_import_resource_classes(self.request)
+
+        with self.assertWarnsRegex(
+            DeprecationWarning,
+            r"^The 'resource_class' field has been deprecated. "
+            r"Please implement the new 'resource_classes' field$",
+        ):
+            self.assertEqual(
+                admin.get_resource_classes(self.request), [resources.Resource]
+            )
+
+        self.assertEqual(1, admin.export_call_count)
+        self.assertEqual(1, admin.import_call_count)
+
+    class BaseModelGetExportResourceClassTest(mixins.BaseExportMixin):
+        def get_resource_class(self):
+            pass
+
+    def test_deprecated_get_resource_class_raises_warning(self):
+        """Test that the mixin throws error if user
+        didn't migrate to resource_classes"""
+        admin = self.BaseModelGetExportResourceClassTest()
+        with self.assertWarnsRegex(
+            DeprecationWarning,
+            r"^The 'get_resource_class\(\)' method has been deprecated. "
+            r"Please implement the new 'get_resource_classes\(\)' method$",
+        ):
+            admin.get_resource_classes(self.request)
+
     class BaseModelAdminFaultyResourceClassesTest(mixins.BaseExportMixin):
         resource_classes = resources.Resource
 
     def test_faulty_resource_class_raises_exception(self):
         """Test fallback mechanism to old get_export_resource_class() method"""
         admin = self.BaseModelAdminFaultyResourceClassesTest()
         with self.assertRaisesRegex(
@@ -195,14 +251,22 @@
 
     class BaseModelAdminBothResourceTest(mixins.BaseExportMixin):
         call_count = 0
 
         resource_class = resources.Resource
         resource_classes = [resources.Resource]
 
+    def test_both_resource_class_raises_exception(self):
+        """Test fallback mechanism to old get_export_resource_class() method"""
+        admin = self.BaseModelAdminBothResourceTest()
+        with self.assertRaisesRegex(
+            Exception, "Only one of 'resource_class' and 'resource_classes' can be set"
+        ):
+            admin.get_export_resource_classes(self.request)
+
     class BaseModelExportChooseTest(mixins.BaseExportMixin):
         resource_classes = [resources.Resource, FooResource]
 
     @mock.patch("import_export.admin.SelectableFieldsExportForm")
     def test_choose_export_resource_class(self, form):
         """Test choose_export_resource_class() method"""
         admin = self.BaseModelExportChooseTest()
@@ -227,14 +291,42 @@
             admin.choose_import_resource_class(form, request),
             resources.Resource,
         )
 
         form.cleaned_data = {"resource": 1}
         self.assertEqual(admin.choose_import_resource_class(form, request), FooResource)
 
+    class BaseModelResourceClassOldTest(mixins.BaseImportMixin, mixins.BaseExportMixin):
+        def get_resource_class(self):
+            return FooResource
+
+    def test_get_resource_class_old(self):
+        """
+        Test that if only the old get_resource_class() method is defined,
+        the get_export_resource_classes() and get_import_resource_classes()
+        still return list of resources.
+        """
+        admin = self.BaseModelResourceClassOldTest()
+        with self.assertWarnsRegex(
+            DeprecationWarning,
+            r"^The 'get_resource_class\(\)' method has been deprecated. "
+            r"Please implement the new 'get_resource_classes\(\)' method$",
+        ):
+            self.assertEqual(
+                admin.get_export_resource_classes(self.request), [FooResource]
+            )
+        with self.assertWarnsRegex(
+            DeprecationWarning,
+            r"^The 'get_resource_class\(\)' method has been deprecated. "
+            r"Please implement the new 'get_resource_classes\(\)' method$",
+        ):
+            self.assertEqual(
+                admin.get_import_resource_classes(self.request), [FooResource]
+            )
+
 
 class BaseExportMixinTest(TestCase):
     class TestBaseExportMixin(mixins.BaseExportMixin):
         def get_export_resource_kwargs(self, request, **kwargs):
             self.kwargs = kwargs
             return super().get_resource_kwargs(request, **kwargs)
```

### Comparing `django_import_export-4.0.2/tests/core/tests/test_model_resource_fields_generate_widgets.py` & `django_import_export-4.0.3/tests/core/tests/test_model_resource_fields_generate_widgets.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/tests/core/tests/test_permissions.py` & `django_import_export-4.0.3/tests/core/tests/test_permissions.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/tests/core/tests/test_resources/test_bulk_operations.py` & `django_import_export-4.0.3/tests/core/tests/test_resources/test_bulk_operations.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/tests/core/tests/test_resources/test_diffs.py` & `django_import_export-4.0.3/tests/core/tests/test_resources/test_diffs.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/tests/core/tests/test_resources/test_import_export.py` & `django_import_export-4.0.3/tests/core/tests/test_resources/test_import_export.py`

 * *Files 3% similar despite different names*

```diff
@@ -326,14 +326,35 @@
             self.resource.import_data(dataset, raise_errors=True)
         self.assertEqual(
             "The following fields are declared in 'import_id_fields' "
             "but are not present in the file headers: id, author_email",
             str(e.exception),
         )
 
+    def test_dynamic_import_id_fields(self):
+        # issue 1834
+        class BookResource(resources.ModelResource):
+            def before_import(self, dataset, **kwargs):
+                # mimic a 'dynamic field' - i.e. append field which exists on
+                # Book model, but not in dataset
+                dataset.headers.append("price")
+                super().before_import(dataset, **kwargs)
+
+            class Meta:
+                model = Book
+                import_id_fields = ("price",)
+
+        self.resource = BookResource()
+        dataset = tablib.Dataset(
+            *[(self.book.pk, "Goldeneye", "ian.fleming@example.com")],
+            headers=["id", "name", "author_email"],
+        )
+        self.resource.import_data(dataset, raise_errors=True)
+        self.assertEqual("Goldeneye", Book.objects.latest("id").name)
+
 
 class ImportWithMissingFields(TestCase):
     # issue 1517
 
     @patch("import_export.resources.logger")
     @patch("import_export.fields.Field.save")
     def test_import_with_missing_instance_attribute(self, mock_field_save, mock_logger):
```

### Comparing `django_import_export-4.0.2/tests/core/tests/test_resources/test_misc.py` & `django_import_export-4.0.3/tests/core/tests/test_resources/test_misc.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/tests/core/tests/test_resources/test_modelresource/test_data_deletion.py` & `django_import_export-4.0.3/tests/core/tests/test_resources/test_modelresource/test_data_deletion.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/tests/core/tests/test_resources/test_modelresource/test_data_handling.py` & `django_import_export-4.0.3/tests/core/tests/test_resources/test_modelresource/test_data_handling.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/tests/core/tests/test_resources/test_modelresource/test_data_import.py` & `django_import_export-4.0.3/tests/core/tests/test_resources/test_modelresource/test_data_import.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/tests/core/tests/test_resources/test_modelresource/test_deprecated_fields.py` & `django_import_export-4.0.3/tests/core/tests/test_resources/test_modelresource/test_deprecated_fields.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/tests/core/tests/test_resources/test_modelresource/test_dynamic_customization.py` & `django_import_export-4.0.3/tests/core/tests/test_resources/test_modelresource/test_dynamic_customization.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/tests/core/tests/test_resources/test_modelresource/test_error_handling.py` & `django_import_export-4.0.3/tests/core/tests/test_resources/test_modelresource/test_error_handling.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/tests/core/tests/test_resources/test_modelresource/test_export.py` & `django_import_export-4.0.3/tests/core/tests/test_resources/test_modelresource/test_export.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/tests/core/tests/test_resources/test_modelresource/test_fields.py` & `django_import_export-4.0.3/tests/core/tests/test_resources/test_modelresource/test_fields.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/tests/core/tests/test_resources/test_modelresource/test_m2m.py` & `django_import_export-4.0.3/tests/core/tests/test_resources/test_modelresource/test_m2m.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/tests/core/tests/test_resources/test_modelresource/test_queryset.py` & `django_import_export-4.0.3/tests/core/tests/test_resources/test_modelresource/test_queryset.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/tests/core/tests/test_resources/test_modelresource/test_relationship.py` & `django_import_export-4.0.3/tests/core/tests/test_resources/test_modelresource/test_relationship.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/tests/core/tests/test_resources/test_modelresource/test_resource.py` & `django_import_export-4.0.3/tests/core/tests/test_resources/test_modelresource/test_resource.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/tests/core/tests/test_resources/test_modelresource/test_resource_fields.py` & `django_import_export-4.0.3/tests/core/tests/test_resources/test_modelresource/test_resource_fields.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/tests/core/tests/test_resources/test_modelresource/test_resource_postgres.py` & `django_import_export-4.0.3/tests/core/tests/test_resources/test_modelresource/test_resource_postgres.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/tests/core/tests/test_resources/test_modelresource/test_resource_setup.py` & `django_import_export-4.0.3/tests/core/tests/test_resources/test_modelresource/test_resource_setup.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/tests/core/tests/test_resources/test_modelresource/test_resource_transactions.py` & `django_import_export-4.0.3/tests/core/tests/test_resources/test_modelresource/test_resource_transactions.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/tests/core/tests/test_resources/test_modelresource/test_widget.py` & `django_import_export-4.0.3/tests/core/tests/test_resources/test_modelresource/test_widget.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/tests/core/tests/test_resources/test_natural_foreign_key.py` & `django_import_export-4.0.3/tests/core/tests/test_resources/test_natural_foreign_key.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/tests/core/tests/test_resources/test_relationships.py` & `django_import_export-4.0.3/tests/core/tests/test_resources/test_relationships.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/tests/core/tests/test_results.py` & `django_import_export-4.0.3/tests/core/tests/test_results.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/tests/core/tests/test_tmp_storages.py` & `django_import_export-4.0.3/tests/core/tests/test_tmp_storages.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/tests/core/tests/test_widgets.py` & `django_import_export-4.0.3/tests/core/tests/test_widgets.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/tests/docker-compose.yml` & `django_import_export-4.0.3/tests/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/tests/scripts/bulk_import.py` & `django_import_export-4.0.3/tests/scripts/bulk_import.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/tests/settings.py` & `django_import_export-4.0.3/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django_import_export-4.0.2/tox.ini` & `django_import_export-4.0.3/tox.ini`

 * *Files identical despite different names*

