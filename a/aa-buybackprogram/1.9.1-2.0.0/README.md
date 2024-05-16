# Comparing `tmp/aa-buybackprogram-1.9.1.tar.gz` & `tmp/aa_buybackprogram-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aa-buybackprogram-1.9.1.tar", last modified: Wed Mar 29 15:38:31 2023, max compression
+gzip compressed data, was "aa_buybackprogram-2.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `aa-buybackprogram-1.9.1.tar` & `aa_buybackprogram-2.0.0.tar`

### file list

```diff
@@ -1,108 +1,108 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 15:38:31.013009 aa-buybackprogram-1.9.1/
--rwxrwxrwx   0 root         (0) root         (0)     1070 2022-11-06 14:22:31.000000 aa-buybackprogram-1.9.1/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)      195 2022-11-06 14:22:31.000000 aa-buybackprogram-1.9.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    19555 2023-03-29 15:38:31.013009 aa-buybackprogram-1.9.1/PKG-INFO
--rwxr-xr-x   0 root         (0) root         (0)    18610 2023-03-27 13:16:33.000000 aa-buybackprogram-1.9.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 15:38:31.005009 aa-buybackprogram-1.9.1/aa_buybackprogram.egg-info/
--rw-r--r--   0 root         (0) root         (0)    19555 2023-03-29 15:38:30.000000 aa-buybackprogram-1.9.1/aa_buybackprogram.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3836 2023-03-29 15:38:31.000000 aa-buybackprogram-1.9.1/aa_buybackprogram.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-29 15:38:30.000000 aa-buybackprogram-1.9.1/aa_buybackprogram.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       75 2023-03-29 15:38:30.000000 aa-buybackprogram-1.9.1/aa_buybackprogram.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       24 2023-03-29 15:38:30.000000 aa-buybackprogram-1.9.1/aa_buybackprogram.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 15:38:31.009009 aa-buybackprogram-1.9.1/buybackprogram/
--rwxr-xr-x   0 root         (0) root         (0)      117 2023-03-29 15:14:47.000000 aa-buybackprogram-1.9.1/buybackprogram/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)      965 2023-03-25 14:23:02.000000 aa-buybackprogram-1.9.1/buybackprogram/admin.py
--rwxr-xr-x   0 root         (0) root         (0)     1641 2023-03-27 13:16:33.000000 aa-buybackprogram-1.9.1/buybackprogram/app_settings.py
--rwxrwxrwx   0 root         (0) root         (0)      168 2022-11-06 14:22:31.000000 aa-buybackprogram-1.9.1/buybackprogram/apps.py
--rwxrwxrwx   0 root         (0) root         (0)      936 2022-11-06 14:22:31.000000 aa-buybackprogram-1.9.1/buybackprogram/auth_hooks.py
--rwxrwxrwx   0 root         (0) root         (0)      553 2022-11-06 14:22:31.000000 aa-buybackprogram-1.9.1/buybackprogram/constants.py
--rwxrwxrwx   0 root         (0) root         (0)      553 2022-11-06 14:22:31.000000 aa-buybackprogram-1.9.1/buybackprogram/decorators.py
--rwxr-xr-x   0 root         (0) root         (0)     5699 2023-03-27 13:16:33.000000 aa-buybackprogram-1.9.1/buybackprogram/forms.py
--rwxr-xr-x   0 root         (0) root         (0)    35039 2023-03-29 15:14:47.000000 aa-buybackprogram-1.9.1/buybackprogram/helpers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 15:38:31.009009 aa-buybackprogram-1.9.1/buybackprogram/management/
--rwxrwxrwx   0 root         (0) root         (0)        0 2022-11-06 14:22:31.000000 aa-buybackprogram-1.9.1/buybackprogram/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 15:38:31.009009 aa-buybackprogram-1.9.1/buybackprogram/management/commands/
--rwxrwxrwx   0 root         (0) root         (0)      102 2022-11-06 14:22:31.000000 aa-buybackprogram-1.9.1/buybackprogram/management/commands/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     3519 2023-03-27 13:16:33.000000 aa-buybackprogram-1.9.1/buybackprogram/management/commands/buybackprogram_generate_test_data.py
--rwxr-xr-x   0 root         (0) root         (0)     2179 2023-03-27 13:16:33.000000 aa-buybackprogram-1.9.1/buybackprogram/management/commands/buybackprogram_link_contracts.py
--rwxr-xr-x   0 root         (0) root         (0)     1849 2023-03-27 13:16:33.000000 aa-buybackprogram-1.9.1/buybackprogram/management/commands/buybackprogram_load_data.py
--rwxrwxrwx   0 root         (0) root         (0)     3792 2022-11-06 14:22:31.000000 aa-buybackprogram-1.9.1/buybackprogram/management/commands/buybackprogram_load_prices.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 15:38:31.009009 aa-buybackprogram-1.9.1/buybackprogram/migrations/
--rwxr-xr-x   0 root         (0) root         (0)    23557 2023-03-27 13:16:33.000000 aa-buybackprogram-1.9.1/buybackprogram/migrations/0001_initial.py
--rwxr-xr-x   0 root         (0) root         (0)     1112 2023-03-27 13:16:33.000000 aa-buybackprogram-1.9.1/buybackprogram/migrations/0002_contractnotification.py
--rwxr-xr-x   0 root         (0) root         (0)     1119 2023-03-27 13:16:33.000000 aa-buybackprogram-1.9.1/buybackprogram/migrations/0003_statics_performance_increase.py
--rwxr-xr-x   0 root         (0) root         (0)      709 2023-03-27 13:16:33.000000 aa-buybackprogram-1.9.1/buybackprogram/migrations/0004_auto_20220323_1331.py
--rwxr-xr-x   0 root         (0) root         (0)      744 2023-03-27 13:16:33.000000 aa-buybackprogram-1.9.1/buybackprogram/migrations/0005_program_compression_price_dencity_modifier.py
--rwxr-xr-x   0 root         (0) root         (0)     1334 2023-03-27 13:16:33.000000 aa-buybackprogram-1.9.1/buybackprogram/migrations/0006_program_bonds_npc_price_and_more.py
--rwxr-xr-x   0 root         (0) root         (0)      809 2023-03-27 13:16:33.000000 aa-buybackprogram-1.9.1/buybackprogram/migrations/0007_program_expiration.py
--rwxr-xr-x   0 root         (0) root         (0)     1763 2023-03-27 13:16:33.000000 aa-buybackprogram-1.9.1/buybackprogram/migrations/0008_alter_general_options_alter_program_refining_rate.py
--rw-r--r--   0 root         (0) root         (0)      442 2023-03-27 13:16:33.000000 aa-buybackprogram-1.9.1/buybackprogram/migrations/0009_contract_location_name.py
--rw-r--r--   0 root         (0) root         (0)      568 2023-03-27 13:28:24.000000 aa-buybackprogram-1.9.1/buybackprogram/migrations/0010_contract_no_tracking_alter_tracking_tracking_number.py
--rwxrwxrwx   0 root         (0) root         (0)        0 2022-11-06 14:22:31.000000 aa-buybackprogram-1.9.1/buybackprogram/migrations/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)    48918 2023-03-29 14:56:21.000000 aa-buybackprogram-1.9.1/buybackprogram/models.py
--rwxr-xr-x   0 root         (0) root         (0)     5514 2023-03-27 13:16:33.000000 aa-buybackprogram-1.9.1/buybackprogram/notes.py
--rwxr-xr-x   0 root         (0) root         (0)     6138 2023-03-27 13:16:33.000000 aa-buybackprogram-1.9.1/buybackprogram/notification.py
--rwxrwxrwx   0 root         (0) root         (0)      386 2022-11-06 14:22:31.000000 aa-buybackprogram-1.9.1/buybackprogram/providers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 15:38:31.005009 aa-buybackprogram-1.9.1/buybackprogram/static/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 15:38:31.005009 aa-buybackprogram-1.9.1/buybackprogram/static/buybackprogram/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 15:38:31.009009 aa-buybackprogram-1.9.1/buybackprogram/static/buybackprogram/css/
--rwxr-xr-x   0 root         (0) root         (0)     4582 2022-11-06 17:12:51.000000 aa-buybackprogram-1.9.1/buybackprogram/static/buybackprogram/css/billboards_dark.css
--rwxr-xr-x   0 root         (0) root         (0)     4558 2022-11-06 17:12:51.000000 aa-buybackprogram-1.9.1/buybackprogram/static/buybackprogram/css/billboards_light.css
--rwxr-xr-x   0 root         (0) root         (0)    21820 2022-11-06 17:12:51.000000 aa-buybackprogram-1.9.1/buybackprogram/static/buybackprogram/css/style_dark.css
--rwxrwxrwx   0 root         (0) root         (0)    21655 2022-11-06 14:22:31.000000 aa-buybackprogram-1.9.1/buybackprogram/static/buybackprogram/css/style_light.css
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 15:38:31.009009 aa-buybackprogram-1.9.1/buybackprogram/static/buybackprogram/images/
--rwxr-xr-x   0 root         (0) root         (0)      761 2022-11-06 17:12:51.000000 aa-buybackprogram-1.9.1/buybackprogram/static/buybackprogram/images/help.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 15:38:31.009009 aa-buybackprogram-1.9.1/buybackprogram/static/buybackprogram/js/
--rwxrwxrwx   0 root         (0) root         (0)      412 2022-11-06 14:22:31.000000 aa-buybackprogram-1.9.1/buybackprogram/static/buybackprogram/js/autocomplete.js
--rwxrwxrwx   0 root         (0) root         (0)    37085 2022-11-06 14:22:31.000000 aa-buybackprogram-1.9.1/buybackprogram/static/buybackprogram/js/bootstrap-autocomplete.min.js
--rwxrwxrwx   0 root         (0) root         (0)   947196 2022-11-06 14:22:31.000000 aa-buybackprogram-1.9.1/buybackprogram/swagger.json
--rwxr-xr-x   0 root         (0) root         (0)     7971 2023-03-27 13:16:33.000000 aa-buybackprogram-1.9.1/buybackprogram/tasks.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 15:38:31.005009 aa-buybackprogram-1.9.1/buybackprogram/templates/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 15:38:31.009009 aa-buybackprogram-1.9.1/buybackprogram/templates/buybackprogram/
--rwxrwxrwx   0 root         (0) root         (0)      802 2022-11-06 14:22:31.000000 aa-buybackprogram-1.9.1/buybackprogram/templates/buybackprogram/base.html
--rwxr-xr-x   0 root         (0) root         (0)     6729 2022-11-06 18:09:14.000000 aa-buybackprogram-1.9.1/buybackprogram/templates/buybackprogram/contract_details.html
--rwxr-xr-x   0 root         (0) root         (0)     1218 2022-11-06 17:12:51.000000 aa-buybackprogram-1.9.1/buybackprogram/templates/buybackprogram/faq.html
--rwxrwxrwx   0 root         (0) root         (0)     3099 2022-11-06 14:22:31.000000 aa-buybackprogram-1.9.1/buybackprogram/templates/buybackprogram/index.html
--rwxr-xr-x   0 root         (0) root         (0)     2774 2022-11-06 17:12:51.000000 aa-buybackprogram-1.9.1/buybackprogram/templates/buybackprogram/leaderboards.html
--rwxrwxrwx   0 root         (0) root         (0)     1753 2022-11-06 14:22:31.000000 aa-buybackprogram-1.9.1/buybackprogram/templates/buybackprogram/location_add.html
--rwxrwxrwx   0 root         (0) root         (0)     2838 2022-11-06 14:22:31.000000 aa-buybackprogram-1.9.1/buybackprogram/templates/buybackprogram/menu.html
--rwxrwxrwx   0 root         (0) root         (0)      171 2022-11-06 14:22:31.000000 aa-buybackprogram-1.9.1/buybackprogram/templates/buybackprogram/page.html
--rwxr-xr-x   0 root         (0) root         (0)     7008 2023-03-18 13:02:24.000000 aa-buybackprogram-1.9.1/buybackprogram/templates/buybackprogram/performance.html
--rwxrwxrwx   0 root         (0) root         (0)      584 2022-11-06 14:22:31.000000 aa-buybackprogram-1.9.1/buybackprogram/templates/buybackprogram/program_add.html
--rwxrwxrwx   0 root         (0) root         (0)    16302 2022-11-06 14:22:31.000000 aa-buybackprogram-1.9.1/buybackprogram/templates/buybackprogram/program_calculate.html
--rwxrwxrwx   0 root         (0) root         (0)      861 2022-11-06 14:22:31.000000 aa-buybackprogram-1.9.1/buybackprogram/templates/buybackprogram/program_edit.html
--rwxrwxrwx   0 root         (0) root         (0)     1180 2022-11-06 14:22:31.000000 aa-buybackprogram-1.9.1/buybackprogram/templates/buybackprogram/program_edit_item.html
--rwxr-xr-x   0 root         (0) root         (0)     1188 2022-11-06 17:12:51.000000 aa-buybackprogram-1.9.1/buybackprogram/templates/buybackprogram/program_edit_marketgroup.html
--rwxr-xr-x   0 root         (0) root         (0)     2748 2022-11-06 17:12:51.000000 aa-buybackprogram-1.9.1/buybackprogram/templates/buybackprogram/program_special_taxes.html
--rwxr-xr-x   0 root         (0) root         (0)    11272 2023-03-27 13:28:24.000000 aa-buybackprogram-1.9.1/buybackprogram/templates/buybackprogram/stats.html
--rwxr-xr-x   0 root         (0) root         (0)      669 2022-11-06 17:12:51.000000 aa-buybackprogram-1.9.1/buybackprogram/templates/buybackprogram/user_settings.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 15:38:31.009009 aa-buybackprogram-1.9.1/buybackprogram/templatetags/
--rwxrwxrwx   0 root         (0) root         (0)        0 2022-11-06 14:22:31.000000 aa-buybackprogram-1.9.1/buybackprogram/templatetags/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      430 2022-11-06 14:22:31.000000 aa-buybackprogram-1.9.1/buybackprogram/templatetags/price_formats.py
--rwxr-xr-x   0 root         (0) root         (0)     4618 2023-03-27 13:16:33.000000 aa-buybackprogram-1.9.1/buybackprogram/templatetags/program_settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 15:38:31.009009 aa-buybackprogram-1.9.1/buybackprogram/tests/
--rwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 14:56:21.000000 aa-buybackprogram-1.9.1/buybackprogram/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)      924 2023-03-29 15:14:47.000000 aa-buybackprogram-1.9.1/buybackprogram/tests/test_helpers.py
--rw-r--r--   0 root         (0) root         (0)    10700 2023-03-29 14:56:21.000000 aa-buybackprogram-1.9.1/buybackprogram/tests/test_models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 15:38:31.013009 aa-buybackprogram-1.9.1/buybackprogram/tests/testdata/
--rw-r--r--   0 root         (0) root         (0)      267 2023-03-29 14:56:21.000000 aa-buybackprogram-1.9.1/buybackprogram/tests/testdata/__init__.py
--rw-r--r--   0 root         (0) root         (0)      757 2023-03-29 14:56:21.000000 aa-buybackprogram-1.9.1/buybackprogram/tests/testdata/create_eveuniverse.py
--rw-r--r--   0 root         (0) root         (0)     9166 2023-03-29 14:56:21.000000 aa-buybackprogram-1.9.1/buybackprogram/tests/testdata/factories.py
--rw-r--r--   0 root         (0) root         (0)      412 2023-03-29 14:56:21.000000 aa-buybackprogram-1.9.1/buybackprogram/tests/testdata/load_eveuniverse.py
--rwxrwxrwx   0 root         (0) root         (0)     2765 2022-11-06 14:22:31.000000 aa-buybackprogram-1.9.1/buybackprogram/urls.py
--rwxr-xr-x   0 root         (0) root         (0)     3885 2023-03-27 13:16:33.000000 aa-buybackprogram-1.9.1/buybackprogram/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 15:38:31.013009 aa-buybackprogram-1.9.1/buybackprogram/views/
--rwxrwxrwx   0 root         (0) root         (0)       29 2022-11-06 14:22:31.000000 aa-buybackprogram-1.9.1/buybackprogram/views/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     9148 2023-03-27 13:16:33.000000 aa-buybackprogram-1.9.1/buybackprogram/views/calculate.py
--rwxr-xr-x   0 root         (0) root         (0)     5261 2023-03-27 13:16:33.000000 aa-buybackprogram-1.9.1/buybackprogram/views/common.py
--rwxr-xr-x   0 root         (0) root         (0)     8622 2023-03-27 13:16:33.000000 aa-buybackprogram-1.9.1/buybackprogram/views/programs.py
--rwxr-xr-x   0 root         (0) root         (0)     6579 2023-03-27 13:16:33.000000 aa-buybackprogram-1.9.1/buybackprogram/views/special_taxes.py
--rwxr-xr-x   0 root         (0) root         (0)    23046 2023-03-27 13:28:24.000000 aa-buybackprogram-1.9.1/buybackprogram/views/stats.py
--rwxr-xr-x   0 root         (0) root         (0)      187 2023-03-29 15:38:31.013009 aa-buybackprogram-1.9.1/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)     1647 2023-03-29 14:56:21.000000 aa-buybackprogram-1.9.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-29 15:38:31.013009 aa-buybackprogram-1.9.1/testauth/
--rwxrwxrwx   0 root         (0) root         (0)       46 2022-11-06 14:22:31.000000 aa-buybackprogram-1.9.1/testauth/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)      612 2022-11-06 14:22:31.000000 aa-buybackprogram-1.9.1/testauth/celery.py
--rwxr-xr-x   0 root         (0) root         (0)    10041 2023-03-29 14:56:21.000000 aa-buybackprogram-1.9.1/testauth/settings.py
--rwxr-xr-x   0 root         (0) root         (0)      174 2023-03-25 14:23:02.000000 aa-buybackprogram-1.9.1/testauth/urls.py
--rwxrwxrwx   0 root         (0) root         (0)      397 2022-11-06 14:22:31.000000 aa-buybackprogram-1.9.1/testauth/wsgi.py
+-rwxr-xr-x   0        0        0     1070 2024-05-05 07:48:32.887884 aa_buybackprogram-2.0.0/LICENSE
+-rwxr-xr-x   0        0        0    20467 2024-05-16 14:00:46.096935 aa_buybackprogram-2.0.0/README.md
+-rwxr-xr-x   0        0        0      170 2024-05-16 14:02:47.325610 aa_buybackprogram-2.0.0/buybackprogram/__init__.py
+-rwxr-xr-x   0        0        0     1124 2024-05-16 14:00:46.096935 aa_buybackprogram-2.0.0/buybackprogram/admin.py
+-rwxr-xr-x   0        0        0     1931 2024-05-05 07:48:32.891886 aa_buybackprogram-2.0.0/buybackprogram/app_settings.py
+-rwxr-xr-x   0        0        0      168 2024-05-05 07:48:32.891886 aa_buybackprogram-2.0.0/buybackprogram/apps.py
+-rwxr-xr-x   0        0        0      936 2024-05-16 14:00:46.096935 aa_buybackprogram-2.0.0/buybackprogram/auth_hooks.py
+-rwxr-xr-x   0        0        0      604 2024-05-05 07:48:32.891886 aa_buybackprogram-2.0.0/buybackprogram/constants.py
+-rwxr-xr-x   0        0        0      553 2024-05-05 07:48:32.891886 aa_buybackprogram-2.0.0/buybackprogram/decorators.py
+-rwxr-xr-x   0        0        0     5910 2024-05-16 14:00:46.096935 aa_buybackprogram-2.0.0/buybackprogram/forms.py
+-rwxr-xr-x   0        0        0    38564 2024-05-16 14:00:46.096935 aa_buybackprogram-2.0.0/buybackprogram/helpers.py
+-rwxr-xr-x   0        0        0        0 2024-05-05 07:48:32.891886 aa_buybackprogram-2.0.0/buybackprogram/management/__init__.py
+-rwxr-xr-x   0        0        0      102 2024-05-05 07:48:32.891886 aa_buybackprogram-2.0.0/buybackprogram/management/commands/__init__.py
+-rwxr-xr-x   0        0        0     3519 2024-05-05 07:48:32.891886 aa_buybackprogram-2.0.0/buybackprogram/management/commands/buybackprogram_generate_test_data.py
+-rwxr-xr-x   0        0        0     2179 2024-05-05 07:48:32.891886 aa_buybackprogram-2.0.0/buybackprogram/management/commands/buybackprogram_link_contracts.py
+-rwxr-xr-x   0        0        0      548 2024-05-05 07:48:32.891886 aa_buybackprogram-2.0.0/buybackprogram/management/commands/buybackprogram_load_data.py
+-rwxr-xr-x   0        0        0     4621 2024-05-05 07:48:32.891886 aa_buybackprogram-2.0.0/buybackprogram/management/commands/buybackprogram_load_prices.py
+-rw-r--r--   0        0        0     4975 2024-05-16 14:00:46.096935 aa_buybackprogram-2.0.0/buybackprogram/management/commands/generate_dummy_data.py
+-rwxr-xr-x   0        0        0    23557 2024-05-05 07:48:32.891886 aa_buybackprogram-2.0.0/buybackprogram/migrations/0001_initial.py
+-rwxr-xr-x   0        0        0     1112 2024-05-05 07:48:32.891886 aa_buybackprogram-2.0.0/buybackprogram/migrations/0002_contractnotification.py
+-rwxr-xr-x   0        0        0     1119 2024-05-05 07:48:32.891886 aa_buybackprogram-2.0.0/buybackprogram/migrations/0003_statics_performance_increase.py
+-rwxr-xr-x   0        0        0      709 2024-05-05 07:48:32.891886 aa_buybackprogram-2.0.0/buybackprogram/migrations/0004_auto_20220323_1331.py
+-rwxr-xr-x   0        0        0      744 2024-05-05 07:48:32.891886 aa_buybackprogram-2.0.0/buybackprogram/migrations/0005_program_compression_price_dencity_modifier.py
+-rwxr-xr-x   0        0        0     1334 2024-05-05 07:48:32.891886 aa_buybackprogram-2.0.0/buybackprogram/migrations/0006_program_bonds_npc_price_and_more.py
+-rwxr-xr-x   0        0        0      809 2024-05-05 07:48:32.891886 aa_buybackprogram-2.0.0/buybackprogram/migrations/0007_program_expiration.py
+-rwxr-xr-x   0        0        0     1763 2024-05-05 07:48:32.891886 aa_buybackprogram-2.0.0/buybackprogram/migrations/0008_alter_general_options_alter_program_refining_rate.py
+-rwxr-xr-x   0        0        0      442 2024-05-05 07:48:32.891886 aa_buybackprogram-2.0.0/buybackprogram/migrations/0009_contract_location_name.py
+-rwxr-xr-x   0        0        0      568 2024-05-05 07:48:32.891886 aa_buybackprogram-2.0.0/buybackprogram/migrations/0010_contract_no_tracking_alter_tracking_tracking_number.py
+-rwxr-xr-x   0        0        0     3191 2024-05-05 07:48:32.891886 aa_buybackprogram-2.0.0/buybackprogram/migrations/0011_delete_duplicated_contracts.py
+-rwxr-xr-x   0        0        0      409 2024-05-05 07:48:32.891886 aa_buybackprogram-2.0.0/buybackprogram/migrations/0012_make_contract_id_unique.py
+-rwxr-xr-x   0        0        0      671 2024-05-05 07:48:32.891886 aa_buybackprogram-2.0.0/buybackprogram/migrations/0013_program_discord_show_item_list.py
+-rwxr-xr-x   0        0        0      643 2024-05-16 14:00:46.096935 aa_buybackprogram-2.0.0/buybackprogram/migrations/0014_program_price_type.py
+-rw-r--r--   0        0        0     1106 2024-05-16 14:00:46.096935 aa_buybackprogram-2.0.0/buybackprogram/migrations/0015_faq_contractnotification_header_and_more.py
+-rwxr-xr-x   0        0        0        0 2024-05-05 07:48:32.891886 aa_buybackprogram-2.0.0/buybackprogram/migrations/__init__.py
+-rwxr-xr-x   0        0        0    51801 2024-05-16 14:00:46.096935 aa_buybackprogram-2.0.0/buybackprogram/models.py
+-rwxr-xr-x   0        0        0     5514 2024-05-05 07:48:32.891886 aa_buybackprogram-2.0.0/buybackprogram/notes.py
+-rwxr-xr-x   0        0        0     9387 2024-05-05 07:48:32.891886 aa_buybackprogram-2.0.0/buybackprogram/notification.py
+-rwxr-xr-x   0        0        0      386 2024-05-05 07:48:32.891886 aa_buybackprogram-2.0.0/buybackprogram/providers.py
+-rwxr-xr-x   0        0        0     4582 2024-05-05 07:48:32.891886 aa_buybackprogram-2.0.0/buybackprogram/static/buybackprogram/css/billboards_dark.css
+-rwxr-xr-x   0        0        0     4558 2024-05-05 07:48:32.891886 aa_buybackprogram-2.0.0/buybackprogram/static/buybackprogram/css/billboards_light.css
+-rwxr-xr-x   0        0        0    21820 2024-05-05 07:48:32.891886 aa_buybackprogram-2.0.0/buybackprogram/static/buybackprogram/css/style_dark.css
+-rwxr-xr-x   0        0        0    21763 2024-05-16 14:00:46.100933 aa_buybackprogram-2.0.0/buybackprogram/static/buybackprogram/css/style_light.css
+-rwxr-xr-x   0        0        0      761 2024-05-05 07:48:32.891886 aa_buybackprogram-2.0.0/buybackprogram/static/buybackprogram/images/help.png
+-rwxr-xr-x   0        0        0      412 2024-05-05 07:48:32.891886 aa_buybackprogram-2.0.0/buybackprogram/static/buybackprogram/js/autocomplete.js
+-rwxr-xr-x   0        0        0    37085 2024-05-05 07:48:32.891886 aa_buybackprogram-2.0.0/buybackprogram/static/buybackprogram/js/bootstrap-autocomplete.min.js
+-rwxr-xr-x   0        0        0   947196 2024-05-05 07:48:32.895887 aa_buybackprogram-2.0.0/buybackprogram/swagger.json
+-rwxr-xr-x   0        0        0    19880 2024-05-16 14:00:46.100933 aa_buybackprogram-2.0.0/buybackprogram/tasks.py
+-rwxr-xr-x   0        0        0      718 2024-05-16 14:00:46.100933 aa_buybackprogram-2.0.0/buybackprogram/templates/buybackprogram/base.html
+-rwxr-xr-x   0        0        0      115 2024-05-16 14:00:46.100933 aa_buybackprogram-2.0.0/buybackprogram/templates/buybackprogram/bundles/buybackprogram-css-light.html
+-rwxr-xr-x   0        0        0     2583 2024-05-16 14:00:46.100933 aa_buybackprogram-2.0.0/buybackprogram/templates/buybackprogram/contract_details.html
+-rwxr-xr-x   0        0        0     1667 2024-05-16 14:00:46.100933 aa_buybackprogram-2.0.0/buybackprogram/templates/buybackprogram/faq.html
+-rwxr-xr-x   0        0        0     3356 2024-05-16 14:00:46.100933 aa_buybackprogram-2.0.0/buybackprogram/templates/buybackprogram/index.html
+-rwxr-xr-x   0        0        0     2645 2024-05-16 14:00:46.100933 aa_buybackprogram-2.0.0/buybackprogram/templates/buybackprogram/leaderboards.html
+-rwxr-xr-x   0        0        0     1739 2024-05-16 14:00:46.100933 aa_buybackprogram-2.0.0/buybackprogram/templates/buybackprogram/location_add.html
+-rwxr-xr-x   0        0        0      171 2024-05-06 04:45:55.385577 aa_buybackprogram-2.0.0/buybackprogram/templates/buybackprogram/page.html
+-rw-r--r--   0        0        0      734 2024-05-16 14:00:46.100933 aa_buybackprogram-2.0.0/buybackprogram/templates/buybackprogram/partials/base/menu-management.html
+-rw-r--r--   0        0        0     1478 2024-05-16 14:00:46.100933 aa_buybackprogram-2.0.0/buybackprogram/templates/buybackprogram/partials/base/menu.html
+-rw-r--r--   0        0        0      347 2024-05-16 14:00:46.100933 aa_buybackprogram-2.0.0/buybackprogram/templates/buybackprogram/partials/calculate/accepted_locations.html
+-rw-r--r--   0        0        0      169 2024-05-16 14:00:46.100933 aa_buybackprogram-2.0.0/buybackprogram/templates/buybackprogram/partials/calculate/calculation_success.html
+-rw-r--r--   0        0        0     1784 2024-05-16 14:00:46.100933 aa_buybackprogram-2.0.0/buybackprogram/templates/buybackprogram/partials/calculate/contract_settings.html
+-rw-r--r--   0        0        0     1936 2024-05-16 14:00:46.100933 aa_buybackprogram-2.0.0/buybackprogram/templates/buybackprogram/partials/calculate/invoice.html
+-rw-r--r--   0        0        0    11774 2024-05-16 14:00:46.100933 aa_buybackprogram-2.0.0/buybackprogram/templates/buybackprogram/partials/calculate/item_details.html
+-rwxr-xr-x   0        0        0      325 2024-05-16 14:00:46.100933 aa_buybackprogram-2.0.0/buybackprogram/templates/buybackprogram/partials/details/accepted-locations.html
+-rwxr-xr-x   0        0        0     1245 2024-05-16 14:00:46.100933 aa_buybackprogram-2.0.0/buybackprogram/templates/buybackprogram/partials/details/contract-info.html
+-rwxr-xr-x   0        0        0     1371 2024-05-16 14:00:46.100933 aa_buybackprogram-2.0.0/buybackprogram/templates/buybackprogram/partials/details/invoice.html
+-rwxr-xr-x   0        0        0     1207 2024-05-16 14:00:46.100933 aa_buybackprogram-2.0.0/buybackprogram/templates/buybackprogram/partials/details/tabs/contract-items.html
+-rwxr-xr-x   0        0        0     1359 2024-05-16 14:00:46.100933 aa_buybackprogram-2.0.0/buybackprogram/templates/buybackprogram/partials/details/tabs/original-items.html
+-rwxr-xr-x   0        0        0      702 2024-05-16 14:00:46.100933 aa_buybackprogram-2.0.0/buybackprogram/templates/buybackprogram/partials/details/tabs/tabs-navigation.html
+-rwxr-xr-x   0        0        0      358 2024-05-16 14:00:46.100933 aa_buybackprogram-2.0.0/buybackprogram/templates/buybackprogram/partials/details/warning.html
+-rwxr-xr-x   0        0        0      945 2024-05-16 14:00:46.100933 aa_buybackprogram-2.0.0/buybackprogram/templates/buybackprogram/partials/stats/summary.html
+-rwxr-xr-x   0        0        0     2437 2024-05-16 14:00:46.100933 aa_buybackprogram-2.0.0/buybackprogram/templates/buybackprogram/partials/stats/tabs/finished.html
+-rwxr-xr-x   0        0        0     2423 2024-05-16 14:00:46.100933 aa_buybackprogram-2.0.0/buybackprogram/templates/buybackprogram/partials/stats/tabs/outstanding.html
+-rwxr-xr-x   0        0        0     1089 2024-05-16 14:00:46.100933 aa_buybackprogram-2.0.0/buybackprogram/templates/buybackprogram/partials/stats/tabs/tabs-navigation.html
+-rwxr-xr-x   0        0        0     2296 2024-05-16 14:00:46.100933 aa_buybackprogram-2.0.0/buybackprogram/templates/buybackprogram/partials/stats/tabs/untracked.html
+-rwxr-xr-x   0        0        0      451 2024-05-16 14:00:46.100933 aa_buybackprogram-2.0.0/buybackprogram/templates/buybackprogram/partials/stats/warning.html
+-rwxr-xr-x   0        0        0     7547 2024-05-16 14:00:46.100933 aa_buybackprogram-2.0.0/buybackprogram/templates/buybackprogram/performance.html
+-rwxr-xr-x   0        0        0      660 2024-05-16 14:00:46.100933 aa_buybackprogram-2.0.0/buybackprogram/templates/buybackprogram/program_add.html
+-rwxr-xr-x   0        0        0     3307 2024-05-16 14:00:46.100933 aa_buybackprogram-2.0.0/buybackprogram/templates/buybackprogram/program_calculate.html
+-rwxr-xr-x   0        0        0      929 2024-05-16 14:00:46.100933 aa_buybackprogram-2.0.0/buybackprogram/templates/buybackprogram/program_edit.html
+-rwxr-xr-x   0        0        0     1321 2024-05-16 14:00:46.100933 aa_buybackprogram-2.0.0/buybackprogram/templates/buybackprogram/program_edit_item.html
+-rwxr-xr-x   0        0        0     1335 2024-05-16 14:00:46.100933 aa_buybackprogram-2.0.0/buybackprogram/templates/buybackprogram/program_edit_marketgroup.html
+-rwxr-xr-x   0        0        0     2997 2024-05-16 14:00:46.100933 aa_buybackprogram-2.0.0/buybackprogram/templates/buybackprogram/program_special_taxes.html
+-rwxr-xr-x   0        0        0     1471 2024-05-16 14:00:46.100933 aa_buybackprogram-2.0.0/buybackprogram/templates/buybackprogram/stats.html
+-rwxr-xr-x   0        0        0      669 2024-05-16 14:00:46.100933 aa_buybackprogram-2.0.0/buybackprogram/templates/buybackprogram/user_settings.html
+-rwxr-xr-x   0        0        0        0 2024-05-05 07:48:32.895887 aa_buybackprogram-2.0.0/buybackprogram/templatetags/__init__.py
+-rwxr-xr-x   0        0        0      305 2024-05-16 14:00:46.100933 aa_buybackprogram-2.0.0/buybackprogram/templatetags/bs_tab_color_class.py
+-rwxr-xr-x   0        0        0     1285 2024-05-16 14:00:46.100933 aa_buybackprogram-2.0.0/buybackprogram/templatetags/help_icons.py
+-rwxr-xr-x   0        0        0      430 2024-05-05 07:48:32.895887 aa_buybackprogram-2.0.0/buybackprogram/templatetags/price_formats.py
+-rwxr-xr-x   0        0        0     5705 2024-05-05 07:48:32.895887 aa_buybackprogram-2.0.0/buybackprogram/templatetags/program_settings.py
+-rwxr-xr-x   0        0        0        0 2024-05-05 07:48:32.895887 aa_buybackprogram-2.0.0/buybackprogram/tests/__init__.py
+-rwxr-xr-x   0        0        0     3513 2024-05-05 07:48:32.895887 aa_buybackprogram-2.0.0/buybackprogram/tests/test_data_migrations.py
+-rwxr-xr-x   0        0        0     1003 2024-05-16 14:00:46.100933 aa_buybackprogram-2.0.0/buybackprogram/tests/test_helpers.py
+-rwxr-xr-x   0        0        0    10970 2024-05-05 07:48:32.895887 aa_buybackprogram-2.0.0/buybackprogram/tests/test_models.py
+-rwxr-xr-x   0        0        0      267 2024-05-05 07:48:32.895887 aa_buybackprogram-2.0.0/buybackprogram/tests/testdata/__init__.py
+-rwxr-xr-x   0        0        0      757 2024-05-05 07:48:32.895887 aa_buybackprogram-2.0.0/buybackprogram/tests/testdata/create_eveuniverse.py
+-rwxr-xr-x   0        0        0  1382783 2024-05-05 07:48:32.895887 aa_buybackprogram-2.0.0/buybackprogram/tests/testdata/eveuniverse.json
+-rwxr-xr-x   0        0        0     9124 2024-05-05 07:48:32.895887 aa_buybackprogram-2.0.0/buybackprogram/tests/testdata/factories.py
+-rwxr-xr-x   0        0        0      412 2024-05-05 07:48:32.895887 aa_buybackprogram-2.0.0/buybackprogram/tests/testdata/load_eveuniverse.py
+-rwxr-xr-x   0        0        0     2765 2024-05-10 08:03:30.190327 aa_buybackprogram-2.0.0/buybackprogram/urls.py
+-rwxr-xr-x   0        0        0     3885 2024-05-05 07:48:32.895887 aa_buybackprogram-2.0.0/buybackprogram/utils.py
+-rwxr-xr-x   0        0        0       29 2024-05-05 07:48:32.895887 aa_buybackprogram-2.0.0/buybackprogram/views/__init__.py
+-rwxr-xr-x   0        0        0     8893 2024-05-16 14:00:46.100933 aa_buybackprogram-2.0.0/buybackprogram/views/calculate.py
+-rwxr-xr-x   0        0        0     5348 2024-05-16 14:00:46.100933 aa_buybackprogram-2.0.0/buybackprogram/views/common.py
+-rwxr-xr-x   0        0        0     8622 2024-05-05 07:48:32.895887 aa_buybackprogram-2.0.0/buybackprogram/views/programs.py
+-rwxr-xr-x   0        0        0     6579 2024-05-05 07:48:32.895887 aa_buybackprogram-2.0.0/buybackprogram/views/special_taxes.py
+-rwxr-xr-x   0        0        0    14556 2024-05-16 14:00:46.100933 aa_buybackprogram-2.0.0/buybackprogram/views/stats.py
+-rwxr-xr-x   0        0        0     1424 2024-05-16 14:00:46.100933 aa_buybackprogram-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0    21512 1970-01-01 00:00:00.000000 aa_buybackprogram-2.0.0/PKG-INFO
```

### Comparing `aa-buybackprogram-1.9.1/LICENSE` & `aa_buybackprogram-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aa-buybackprogram-1.9.1/PKG-INFO` & `aa_buybackprogram-2.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,49 +1,46 @@
 Metadata-Version: 2.1
 Name: aa-buybackprogram
-Version: 1.9.1
-Summary: Buyback program plugin app for Alliance Auth
-Home-page: https://gitlab.com/paulipa/allianceauth-buyback-program
-Author: Ikarus Cesaille
-Author-email: contact@eve-linknet.com
-License: MIT
+Version: 2.0.0
+Summary: Buyback program plugin app for Alliance Auth.
+Author-email: Ikarus Cesaille <contact@eve-linknet.com>
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 3.1
+Classifier: Framework :: Django :: 4.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
-Requires-Python: ~=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
+Requires-Dist: allianceauth-app-utils>=1.18.0
+Requires-Dist: allianceauth<5.0.0,>=4
+Requires-Dist: django-eveuniverse>=1.0.0
+Project-URL: Homepage, https://gitlab.com/paulipa/allianceauth-buyback-program
 
 # Buyback Program
 
-An Alliance Auth app for creating buyback programs and to allow users calculate prices for buyback contracts.
+An Alliance Auth app for creating buyback programs and to allow users calculate prices for buyback contracts. Designed to be very transparent for the user and fast to use for the managers.
 
 [![pipeline](https://gitlab.com/paulipa/allianceauth-buyback-program/badges/master/pipeline.svg)](https://gitlab.com/paulipa/allianceauth-buyback-program/-/commits/master)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![chat](https://img.shields.io/discord/790364535294132234)](https://discord.gg/zmh52wnfvM)
 
 ## Contents
+
 - [Images](#images)
 - [Features](#features)
-- [Requirements](#requirements)
 - [Installation](#installation)
-- [Setup](#setup)
-- [Permissions](#permissions)
-- [Settings](#settings)
 - [Program Settings](#program-settings)
 - [Change Log](CHANGELOG.md)
 
 ## Images
 
 ![buyback_programs](/uploads/5ed1638501915e936d2e8177f4580da1/buyback_programs.png)
 ![item_details](/uploads/d124c70b15b36490c79b907fa25f768d/item_details.png)
@@ -52,289 +49,357 @@
 
 ## Features
 
 - Multiple programs with their own settings
 - Multiple owners
 - Supports corporation and character owners
 - Flexible program settings:
-	- Allow all items
-	- Allow only spesific items
-	- Custom location names
-	- Global program tax
-	- Item specified tax
-	- Hauling fuel cost
-	- Dynamic low price density tax
-	- NPC price for NPC buy orders
+  - Allow all items
+  - Allow only specific items
+  - Custom location names
+  - Global program tax
+  - Item specified tax
+  - Hauling fuel cost
+  - Dynamic low price density tax
+  - NPC price for NPC buy orders
 - Best price variant for ore:
-	- Supports raw, compressed, refined and any combination of the 3.
-	- Will calculate price by the best available pricing method
+  - Supports raw, compressed, refined and any combination of the 3.
+  - Will calculate price by the best available pricing method
 - Allow / disallow unpacked items
 - Restrict program to:
-	- States
-	- Groups
-	- Open for everyone
+  - States
+  - Groups
+  - Open for everyone
 - Personal buyback static tracking for:
-	- Outstanding contracts
-	- Finished contracts
+  - Outstanding contracts
+  - Finished contracts
 - Program tracking for owners:
-	- Outstanding contracts
-	- Total bought value
+  - Outstanding contracts
+  - Total bought value
 - Contract abuse checker and notifications
-	- Check if items do not match the calcualted contract
-	- Check if price does not match the calculated contract
-	- Check if contract is made at wrong location
-	- Check if contract is made incorrectly to corporation or character
-	- Check extra characters in contract title
-	- Check if contract contains donations
+  - Check if items do not match the calculated contract
+  - Check if price does not match the calculated contract
+  - Check if contract is made at wrong location
+  - Check if contract is made incorrectly to corporation or character
+  - Check extra characters in contract title
+  - Check if contract contains donations
+  - Check for scam contracts mimicing buyback contracts
 - Contract tracking history
 - Supports base price sources from:
-	- [Fuzzwork API](https://market.fuzzwork.co.uk/api/)
-	- [Janice API](https://janice.e-351.com/api/rest/docs/index.html)
+  - [Fuzzwork API](https://market.fuzzwork.co.uk/api/)
+  - [Janice API](https://janice.e-351.com/api/rest/docs/index.html)
+  - Use buy, sell or split price as source
+  - Use 5% top average or instant prices for source
 - Supports discord notifications
-	- Notifications for accepted contracts
-	- Notifications for new contracts
-	- For [aa-discordbot](https://github.com/pvyParts/allianceauth-discordbot)
-	- For [discordproxy](https://gitlab.com/ErikKalkoken/discordproxy)
+  - Notifications for accepted contracts
+  - Notifications for new contracts
+  - For [aa-discordbot](https://github.com/pvyParts/allianceauth-discordbot)
+  - For [discordproxy](https://gitlab.com/ErikKalkoken/discordproxy)
+
+## Installation
 
-## Step 1 - Prerequisites
+### Step 1 - Prerequisites
 
 1. Buyback program is a plugin for Alliance Auth. If you don't have Alliance Auth running already, please install it first before proceeding. (see the official [AA installation guide](https://allianceauth.readthedocs.io/en/latest/installation/auth/allianceauth/) for details)
 1. Buyback program needs the app [django-eveuniverse](https://gitlab.com/ErikKalkoken/django-eveuniverse) to function. Please make sure it is installed, before before continuing.
 
-## Step 2 - Install App
+### Step 2 - Install App
 
 1. Activate your venv ```source /home/allianceserver/venv/auth/bin/activate```
 1. Install the plugin ```pip install aa-buybackprogram```
 1. Add ```'buybackprogram',``` into your settings/local.py installed apps section
 1. Run migrations ```python manage.py migrate```
 1. Collect static files ```python manage.py collectstatic```
 1. Reload supervisor
 
-## Step 3 - Update EVE Online API Application
+### Step 3 - Update EVE Online API Application
+
 Update the Eve Online API app used for authentication in your AA installation to include the following scopes:
+
 - `esi-contracts.read_character_contracts.v1`
 - `esi-contracts.read_corporation_contracts.v1`
 - `esi-universe.read_structures.v1`
 
-## Step 4 - Data Preload
+### Step 4 - Data Preload
 
-Buybackprogram requires a lot of data to function as it is designed to allow your clients to sell you any items that exsist in EVE. For this reason pre-loading all the date will take a while.
+Buybackprogram requires a lot of data to function as it is designed to allow your clients to sell you any items that exists in EVE. For this reason pre-loading all the date will take a while. Data pre-loading is used to decrease the amount of API calls made to type and price fetches.
 
-### Preload Load Type Data
+#### Preload Load Type Data
 
 To load type data run the command ```python manage.py buybackprogram_load_data```. This will start the preload of all `EveType`, `SolarSystem`, `EveMarketGroup` and `EveTypeMaterial` objects.
 
-You can follow the progress of the load from your auth da
+You can follow the progress of the load from your auth dashboard. This task can spike up easily over 100.000 tasks at a time so it is very normal that the queue grows very large while running this task.
 
 > :warning: You will need to wait for the type data to load up before you can start to use the plugin. Trying to adjust program settings while the required data has not been yet loaded may result in failure of adjusting the settings.
 
-### Preload Price Data
+#### Preload Price Data
 
 After you have preloaded the type data you can preload price data into the database. Price data preloading is not mandatory but will speed up the first buyback calculations.
 
-> :information_source: If price information is not found for items when the prices are calcualted the first time the prices for that item will be fetched during the calculation process. This will increase the calculation time for the contract.
+> :information_source: If price information is not found for items when the prices are calculated the first time the prices for that item will be fetched during the calculation process. This will increase the calculation time for the contract.
 
 To preload price data run ```python manage.py buybackprogram_load_prices```
 
-## Step 5 - Configure Auth settings
+### Step 5 - Configure Auth settings
 
 Buyback program requires a few periodic tasks to operate and update its data.
 
-Buybackprogram is designed to use localy stored prices to speed up the price calculations. It is important that you have the price update task in your periodic tasks so that your prices will update.
+Buybackprogram is designed to use locally stored prices to speed up the price calculations. It is important that you have the price update task in your periodic tasks so that your prices will update.
 
-By adding the following lines in your `local.py` setting file the progral will update the stored item prices at midnight. This same task is also responsible for maintenance tasks such as removing unlinked tracking objects. It will also check for any new contracts and update the statistics page with them every 15 minutes:
+By adding the following lines in your `local.py` setting file the program will update the stored item prices at midnight. This same task is also responsible for maintenance tasks such as removing unlinked tracking objects. It will also check for any new contracts and update the statistics page with them every 30 minutes:
 
-```
-# Buybackprogram price updates
+```python
+# Buybackprogram price updates, updates prices at midnight
 CELERYBEAT_SCHEDULE['buybackprogram_update_all_prices'] = {
     'task': 'buybackprogram.tasks.update_all_prices',
     'schedule': crontab(minute=0, hour='0'),
 }
 
-# Buybackprogram contract updates
+# Buybackprogram contract updates, updates contracts every 30 minutes
 CELERYBEAT_SCHEDULE['buybackprogram_update_all_contracts'] = {
     'task': 'buybackprogram.tasks.update_all_contracts',
-    'schedule': crontab(minute='*/15'),
+    'schedule': crontab(minute='*/30'),
+}
+
+# Buybackprogram program performance updates, updates performance at midnight
+CELERYBEAT_SCHEDULE['buybackprogram_update_program_performance'] = {
+    'task': 'buybackprogram.tasks.update_program_performance',
+    'schedule': crontab(minute=0, hour='0'),
 }
 ```
 
-**Additional settings**
+#### Additional settings
+
 You may change the following settings by adding the lines in your `local.py` setting files
 
-Name | Description | Default
--- | -- | --
-BUYBACKPROGRAM_TRACKING_PREFILL | This is the prefill tag you will have on the tracking description for your contracts | aa-bbp.
-BUYBACKPROGRAM_PRICE_SOURCE_ID | Station ID for fetching base prices. Supports IDs listed on [Fuzzworks API](https://market.fuzzwork.co.uk/api/). Does not work with Janice API!| 60003760
-BUYBACKPROGRAM_PRICE_SOURCE_NAME | Display name of your price source. Has no effect on the actual price fetch which uses the ID. | Jita
+Name | Description | Default | Options
+-- | -- | -- | --
+BUYBACKPROGRAM_TRACKING_PREFILL | This is the prefill tag you will have on the tracking description for your contracts | aa-bbp. | Free text input
+BUYBACKPROGRAM_PRICE_SOURCE_ID | Station ID for fetching base prices. Supports IDs listed on [Fuzzwork API](https://market.fuzzwork.co.uk/api/). Does not work with Janice API!| 60003760 | See ID list
+BUYBACKPROGRAM_PRICE_SOURCE_NAME | Display name of your price source. Has no effect on the actual price fetch which uses the ID. | Jita | Free text input
 BUYBACKPROGRAM_PRICE_AGE_WARNING_LIMIT | Limit in hours when an item price is considered as outdated | 48
-BUYBACKPROGRAM_PRICE_METHOD | By default Fuzzwork API will be used for pricing, if this is set to "Janice" then the Janice API will be used. | Fuzzwork
-BUYBACKPROGRAM_PRICE_JANICE_API_KEY | The API key to access Janice API. |
-BUYBACKPROGRAM_UNUSED_TRACKING_PURGE_LIMIT | Time limit to remove unlinked tracking objects from the database. Set to 0 to never purge any tracking objects. | 48 hours
-BUYBACKPROGRAM_TRACK_PREFILL_CONTRACTS | Determines if we will track and store contracts that starts with the prefill phrase but do not have any actual tracking hits in database | True
+BUYBACKPROGRAM_PRICE_METHOD | By default Fuzzwork API will be used for pricing, if this is set to "Janice" then the Janice API will be used. | Fuzzwork | `Fuzzwork`, `Janice`
+BUYBACKPROGRAM_PRICE_INSTANT_PRICES | On default we use top 5% average prices. Set to `true` to change to instant prices | False | `False`, `True`
+BUYBACKPROGRAM_PRICE_JANICE_API_KEY | The API key to access Janice API. | `null` | `G9KwKq3465588VPd6747t95Zh94q3W2E`
+BUYBACKPROGRAM_UNUSED_TRACKING_PURGE_LIMIT | Time limit to remove unlinked tracking objects from the database. Set to 0 to never purge any tracking objects. | 48 | Any number in hours
+BUYBACKPROGRAM_TRACK_PREFILL_CONTRACTS | Determines if we will track and store contracts that starts with the prefill phrase but do not have any actual tracking hits in database | True | `True`, `False`
 
 Note: If you change your price source for an old install you need to wait for the price update task to run or manually run it to update your current database prices.
 
-Note: Using Janice API, Jita 4-4 prices will be used with the top 5% average price of the 5 day median price for buy and sell orders.
+Note: Using Janice API, Jita 4-4 prices will be used with the top 5% average price of the 5 day median price for buy and sell orders. No other price sources can be used with Janice
+
+### Step 6 - Adjust Permissions
 
-## Step 6 - Adjust Permissions
 Overview of all permissions in this program. Note that all permissions are in the "general" section.
 
 Name | Purpose | Example Target Audience
 -- | -- | --
 basic_access | Can access this app and see own statics. Can use buyback programs that are allowed by the buyback restriction rules. | Member State
 manage_programs | Can create new locations and buyback programs and manage their own buyback programs. Can see own buyback programs statics. | Buyback managers
 see_leaderboard | Can see the leaderboard stats for the programs that are visible for the user | Member State
 see_performance | Can see the performance stats for the programs that are visible to the user | Member / Managers
 see_all_statics | Can see all statistics in all buyback programs | Leadership
 
-## Step 7 - Program Setup
+### Step 7 - Program Setup
+
 After you have preloaded all the needed data you can start to setup programs.
 
 Each user with `manage_programs` permission is able to setup their own buyback programs.
 
-### Managers
+#### Managers
+
 Each buyback program is operated by a manager. To add a new manager click on the `setup manager` button.
 
-### Locations
+#### Locations
+
 Each buyback program operates at a location that is constructed of `SolarSystem` and a `Custom name` and an optional `Structure ID`. To add a new location click on the `add location` button on the buyback page.
 
-**Solar System & Name**
-Find a solar system by typing in the solar system box. Then determine a name for the structure. Most often you want to use the actual ingame name of the structure so that people are able to identify the location.
+##### Solar System & Name
+
+Find a solar system by typing in the solar system box. Then determine a name for the structure. Most often you want to use the actual in-game name of the structure so that people are able to identify the location.
+
+The solar system name will indicate your sellers where the program contract structure is located. The name will describe the structure name in where the contracts should be created and most often should be identical to the actual structure name in-game.
 
-The solarsytem name will indicate your sellers where the program contract structure is located. The name will describe the structure name in where the contracts should be created and most often should be identical to the actual structure name ingame.
+##### Structure ID
 
-**Structure ID**
 Structure ID is optional and will enable contract location tracking in the program statistics page. If a program location has been given a structure ID the statistics page will display a warning if the user has made the actual contract from some other structure than the one that was determined in the buyback program.
 
-The easiest way to find the actual structure id is to link the structure name into any chat box and post the structure name into the chat. This can be dont in any channel or the structure name can be also copied from any MOTDs.
+The easiest way to find the actual structure id is to link the structure name into any chat box and post the structure name into the chat. This can be done in any channel or the structure name can be also copied from any MOTDs.
 
 After you have posted the structure name in the chat right click it and press copy. You can now paste the structure into notepad or any other text editor and your output should look like this:
-```
+
+```plain
 [17:37:54] Ikarus Cesaille > <url=showinfo:35826//1037962518481>Oisio - LinkNet Central Station</url> `
 ```
+
 The unique structure ID for your structure is then `1037962518481`. Adding the ID to the location ID field will check if the contract creation location matches this ID.
 
-## Step 8 - Create Program
+### Step 8 - Create Program
+
 Once you have created a location and added at least one manager you can setup the actual program. Click on the `create program` button to create a new program.
 
-### Program settings
+#### Program settings
 
 Each program can be customized based on your needs. When setting up select the settings you wish to use.
 
-#### Owner
+##### Name/Description
+
+A display name for your program
+
+##### Manager
+
 This is the character or the characters corporation which will be used as the assign to target for buyback contracts at this location. To add more owners use the `add manager` button. You can only see your own characters.
 
-#### Is Corporation
+##### Is Corporation
+
 If you wish that the contracts are assigned to the owners corporation instead of the character tick this box.
 
-#### Tax
+##### Location
+
+The location where contracts should be created at. Only these locations are accepted
+
+##### Expiration
+
+Expiration time the contracts should bet set to.
+
+##### Price type
+
+You can select what price type is used as the base price for your calculations. You can select from either buy, sell or split prices.
+
+##### Default tax
+
 This is a general tax which is applied on all items in this program. If you wish to not allow all items in this program you can leave this to 0.
 
-General tax is applied on all items sold via the buyback. You can add additional taxes on individual items or ban them from beeing accepted to the program once you have created the program.
+General tax is applied on all items sold via the buyback. You can add additional taxes on individual items or ban them from being accepted to the program once you have created the program.
+
+##### Hauling fuel cost
 
-#### Hauling fuel cost
 You can add a fuel cost expense that is applied on each item sold via this program based on the volume of the item.
 
 > :information_source: This setting is aimed more to null sec buyback programs to make it easier to calculate your taxes and display your members the expenses you have when selling.
 
-#### Price density modifier
+##### Price density modifier
+
 You can use a price density modifier which will add a additional tax on items with low price per volume ratio such as T1 ships.
 
 > :information_source: This setting is aimer more at high sec buyback programs.
 
-#### Compressable price density modifier
-You can select to ignore price density calculations for items that can be compressed. This is helpful when the compressed variants do not have proper buy orders in Jita. If you set this to True then the compressable item density will be calculated based on the isk / volume of the compression variant of the sold item.
+##### Compressible price density modifier
+
+You can select to ignore price density calculations for items that can be compressed. This is helpful when the compressed variants do not have proper buy orders in Jita. If you set this to True then the compressible item density will be calculated based on the isk / volume of the compression variant of the sold item.
+
+##### Price density threshold
 
-#### Price density threshold
 This is the lowest isk/m^3 ratio for items that are accepted to the program without the price density tax. Finding your own limits depends on your logistical department.
 
 For example: Tritanium is 500 ISK/m³ @ 5 ISK per unit price. PLEX is 14,5Trillion ISK/m³ @2.9M per unit price.
 
-#### Price density tax
+##### Price density tax
+
 This is the tax which will be applied to items with a price density below the price density threshold
 
 > :warning: You should avoid using both the hauling fuel cost and the price density modifier at the same time as their function is fairly similar.
 
-#### Allow all items
+##### Allow all items
+
 If you wish to allow any types of items to be sold via this program keep this box ticker.
 
-You can determine individual increased taxes or ban items from beeing accepted to this program after creating the program.
+You can determine individual increased taxes or ban items from being accepted to this program after creating the program.
 
 If you do not want to accept all items you can set this box to False. By doing this you will need to set up a tax for each item you wish to accept into the program individually.
 
-### Ore settings
+#### Ore settings
+
 Ore type items such as asteroid, moon goo and ice have additional pricing methods you can use. You can use a mix of any of the three pricing models.
 
 > :information_source: When using more than one pricing model the best price will be used as the buy value.
 
-#### Use Refined value
+##### Use Refined value
+
 If you wish to calculate ore buyback value based on the mineral values tick this box.
 
-#### Use compressed value
+##### Use compressed value
+
 If you want to use compressed value as a pricing method tick this box.
 
-#### Use raw ore value
+##### Use raw ore value
+
 If you want to use raw ore value as a pricing method you can tick this box. Note that some ores such as Kernite and Moon Goo do not represent the real mineral value of the ores.
 
 You can also individually ban raw ore types from the program. If you have an other option than the raw ore value selected the price will be calculated based on the other pricing models.
 
-#### Allow unpacked items
+##### Allow unpacked items
+
 Most often you want to buy only items that are packed. This will ensure that people do not sell items such as broken ammo crystals for you.
 
-#### Refining rate
+##### Refining rate
+
 The refining rate is used in combination with the use refined value option.
 
-### Blue loot npc price
+#### Blue loot npc price
+
 If you cant to use NPC buy order prices for blue loot (Sleeper loot) instead of Jita prices check this box. NPC price for these items will always be used even when Jita price would be higher.
 
-### Red loot npc price
+#### Red loot npc price
+
 If you cant to use NPC buy order prices for red loot (Triglavian loot) instead of Jita prices check this box. NPC price for these items will always be used even when Jita price would be higher.
 
-### Restrctions
-You can restict the visibnility of the buyback programs to groups and states with the restriction options.
+#### Restrictions
+
+You can restrict the visibility of the buyback programs to groups and states with the restriction options.
 
 If no options are selected the program will be visible for everyone with the `basic_access` role.
 
 > :no_entry: Do not mix group and state restrictions as this may lead into logic error. If you need to mix then create a separate programs for them.
 
-### Discord DM messages
+#### Discord DM messages
+
 If you want to receive messages over discord for every new contract you can tick this box.
 
 > :information_source: Requires the [aa-discordbot plugin](https://github.com/pvyParts/allianceauth-discordbot) or [discordproxy app](https://gitlab.com/ErikKalkoken/discordproxy) to work
 
-### Discord channel messages
+#### Show list of items on discord message
+
+This option will determine if a list of all contract items is added into the discord message description field. If you are accepting all items the list may become very long. If set to false will show a link to the tracking page instead.
+
+#### Discord channel messages
+
 You can send notifications about new contracts directly into the discord channel which is linked to AUTH,
 
 > :information_source: Requires the [aa-discordbot plugin](https://github.com/pvyParts/allianceauth-discordbot) or [discordproxy app](https://gitlab.com/ErikKalkoken/discordproxy) to work
 
-## Step 9 - Special Taxes
+### Step 9 - Special Taxes
+
 You can modify individual item settings or allow items for a program that has set `allow all items = False` via the `special taxes` menu for each program.
 
-Set a item specific tax for each item. The tax wil be applied on top of the default tax for the program. You can also disallow an item from beeing accepted in the contract completely.
+Set a item specific tax for each item. The tax wil be applied on top of the default tax for the program. You can also disallow an item from being accepted in the contract completely.
 
 > :information_source: The item specific tax can also be a negative value allowing you to decrease taxes on certain items.
 
 To adjust individual item taxes inside a program click on the `Special taxes` button next to your program.
 
-You can either add items one by one with the `add item` button or add all items that belongs to a market group and every subchild market group of that group with `add market group`
+You can either add items one by one with the `add item` button or add all items that belongs to a market group and every sub-child market group of that group with `add market group`
 
 You can edit an item on the taxation table simply by adding it again. To delete the item press the delete button next to it or to delete all items in the program click on the delete all items button.
 
-**Market Groups**
+#### Market Groups
+
 When you add an market group each item inside that market group, the child of the market group and the child of the child group will be added to the item taxes (3 steps down)
 
-The easiest way to check which items are under which market group is to open the market window ingame or third party programs such as [https://evemarketer.com/](https://evemarketer.com/)
+The easiest way to check which items are under which market group is to open the market window in-game or third party programs such as [https://evemarketer.com/](https://evemarketer.com/)
 
 Example:
 
 Market group `Minerals` is the bottom market group that includes the standard minerals. Adding this market group to the taxation will add 8 items to the taxes (Tritanium, Pyerite etc.)
 
-Market group `Standard ores` is a parent gategory and there are no direct items under this category. However this category has child categories such as Veldsar, Jaspet, Scordite which each includes multiple variations of the ores. Adding the `Standard ores` category will add each ore type to the special tax section.
+Market group `Standard ores` is a parent category and there are no direct items under this category. However this category has child categories such as Veldspar, Jaspet, Scordite which each includes multiple variations of the ores. Adding the `Standard ores` category will add each ore type to the special tax section.
+
+#### Most Common Groups
 
-**Most Common Groups**
 Name | Includes | Items
 -- | --
 Standard Ores | Normal ores from belts and anomalies | Veldspar, Hedbergite, Compressed Arkonor ...
 Moon Ores | Ores from moon mining | Cobaltite, Loparite, Pollucite
 Ice Ores | Ores from ice mining | Blue Ice, Dark Glitter, Compressed Blue Ice ....
 Minerals | Contains materials for refining Standard Ore | Tritanium, Pyerite ....
 Salvage Materials | Salvage from loot | Armor Plates, Trigger Unit, Ancient Radar Decorrelator ...
+
```

### Comparing `aa-buybackprogram-1.9.1/README.md` & `aa_buybackprogram-2.0.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 # Buyback Program
 
-An Alliance Auth app for creating buyback programs and to allow users calculate prices for buyback contracts.
+An Alliance Auth app for creating buyback programs and to allow users calculate prices for buyback contracts. Designed to be very transparent for the user and fast to use for the managers.
 
 [![pipeline](https://gitlab.com/paulipa/allianceauth-buyback-program/badges/master/pipeline.svg)](https://gitlab.com/paulipa/allianceauth-buyback-program/-/commits/master)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![chat](https://img.shields.io/discord/790364535294132234)](https://discord.gg/zmh52wnfvM)
 
 ## Contents
+
 - [Images](#images)
 - [Features](#features)
-- [Requirements](#requirements)
 - [Installation](#installation)
-- [Setup](#setup)
-- [Permissions](#permissions)
-- [Settings](#settings)
 - [Program Settings](#program-settings)
 - [Change Log](CHANGELOG.md)
 
 ## Images
 
 ![buyback_programs](/uploads/5ed1638501915e936d2e8177f4580da1/buyback_programs.png)
 ![item_details](/uploads/d124c70b15b36490c79b907fa25f768d/item_details.png)
@@ -27,289 +24,356 @@
 
 ## Features
 
 - Multiple programs with their own settings
 - Multiple owners
 - Supports corporation and character owners
 - Flexible program settings:
-	- Allow all items
-	- Allow only spesific items
-	- Custom location names
-	- Global program tax
-	- Item specified tax
-	- Hauling fuel cost
-	- Dynamic low price density tax
-	- NPC price for NPC buy orders
+  - Allow all items
+  - Allow only specific items
+  - Custom location names
+  - Global program tax
+  - Item specified tax
+  - Hauling fuel cost
+  - Dynamic low price density tax
+  - NPC price for NPC buy orders
 - Best price variant for ore:
-	- Supports raw, compressed, refined and any combination of the 3.
-	- Will calculate price by the best available pricing method
+  - Supports raw, compressed, refined and any combination of the 3.
+  - Will calculate price by the best available pricing method
 - Allow / disallow unpacked items
 - Restrict program to:
-	- States
-	- Groups
-	- Open for everyone
+  - States
+  - Groups
+  - Open for everyone
 - Personal buyback static tracking for:
-	- Outstanding contracts
-	- Finished contracts
+  - Outstanding contracts
+  - Finished contracts
 - Program tracking for owners:
-	- Outstanding contracts
-	- Total bought value
+  - Outstanding contracts
+  - Total bought value
 - Contract abuse checker and notifications
-	- Check if items do not match the calcualted contract
-	- Check if price does not match the calculated contract
-	- Check if contract is made at wrong location
-	- Check if contract is made incorrectly to corporation or character
-	- Check extra characters in contract title
-	- Check if contract contains donations
+  - Check if items do not match the calculated contract
+  - Check if price does not match the calculated contract
+  - Check if contract is made at wrong location
+  - Check if contract is made incorrectly to corporation or character
+  - Check extra characters in contract title
+  - Check if contract contains donations
+  - Check for scam contracts mimicing buyback contracts
 - Contract tracking history
 - Supports base price sources from:
-	- [Fuzzwork API](https://market.fuzzwork.co.uk/api/)
-	- [Janice API](https://janice.e-351.com/api/rest/docs/index.html)
+  - [Fuzzwork API](https://market.fuzzwork.co.uk/api/)
+  - [Janice API](https://janice.e-351.com/api/rest/docs/index.html)
+  - Use buy, sell or split price as source
+  - Use 5% top average or instant prices for source
 - Supports discord notifications
-	- Notifications for accepted contracts
-	- Notifications for new contracts
-	- For [aa-discordbot](https://github.com/pvyParts/allianceauth-discordbot)
-	- For [discordproxy](https://gitlab.com/ErikKalkoken/discordproxy)
+  - Notifications for accepted contracts
+  - Notifications for new contracts
+  - For [aa-discordbot](https://github.com/pvyParts/allianceauth-discordbot)
+  - For [discordproxy](https://gitlab.com/ErikKalkoken/discordproxy)
+
+## Installation
 
-## Step 1 - Prerequisites
+### Step 1 - Prerequisites
 
 1. Buyback program is a plugin for Alliance Auth. If you don't have Alliance Auth running already, please install it first before proceeding. (see the official [AA installation guide](https://allianceauth.readthedocs.io/en/latest/installation/auth/allianceauth/) for details)
 1. Buyback program needs the app [django-eveuniverse](https://gitlab.com/ErikKalkoken/django-eveuniverse) to function. Please make sure it is installed, before before continuing.
 
-## Step 2 - Install App
+### Step 2 - Install App
 
 1. Activate your venv ```source /home/allianceserver/venv/auth/bin/activate```
 1. Install the plugin ```pip install aa-buybackprogram```
 1. Add ```'buybackprogram',``` into your settings/local.py installed apps section
 1. Run migrations ```python manage.py migrate```
 1. Collect static files ```python manage.py collectstatic```
 1. Reload supervisor
 
-## Step 3 - Update EVE Online API Application
+### Step 3 - Update EVE Online API Application
+
 Update the Eve Online API app used for authentication in your AA installation to include the following scopes:
+
 - `esi-contracts.read_character_contracts.v1`
 - `esi-contracts.read_corporation_contracts.v1`
 - `esi-universe.read_structures.v1`
 
-## Step 4 - Data Preload
+### Step 4 - Data Preload
 
-Buybackprogram requires a lot of data to function as it is designed to allow your clients to sell you any items that exsist in EVE. For this reason pre-loading all the date will take a while.
+Buybackprogram requires a lot of data to function as it is designed to allow your clients to sell you any items that exists in EVE. For this reason pre-loading all the date will take a while. Data pre-loading is used to decrease the amount of API calls made to type and price fetches.
 
-### Preload Load Type Data
+#### Preload Load Type Data
 
 To load type data run the command ```python manage.py buybackprogram_load_data```. This will start the preload of all `EveType`, `SolarSystem`, `EveMarketGroup` and `EveTypeMaterial` objects.
 
-You can follow the progress of the load from your auth da
+You can follow the progress of the load from your auth dashboard. This task can spike up easily over 100.000 tasks at a time so it is very normal that the queue grows very large while running this task.
 
 > :warning: You will need to wait for the type data to load up before you can start to use the plugin. Trying to adjust program settings while the required data has not been yet loaded may result in failure of adjusting the settings.
 
-### Preload Price Data
+#### Preload Price Data
 
 After you have preloaded the type data you can preload price data into the database. Price data preloading is not mandatory but will speed up the first buyback calculations.
 
-> :information_source: If price information is not found for items when the prices are calcualted the first time the prices for that item will be fetched during the calculation process. This will increase the calculation time for the contract.
+> :information_source: If price information is not found for items when the prices are calculated the first time the prices for that item will be fetched during the calculation process. This will increase the calculation time for the contract.
 
 To preload price data run ```python manage.py buybackprogram_load_prices```
 
-## Step 5 - Configure Auth settings
+### Step 5 - Configure Auth settings
 
 Buyback program requires a few periodic tasks to operate and update its data.
 
-Buybackprogram is designed to use localy stored prices to speed up the price calculations. It is important that you have the price update task in your periodic tasks so that your prices will update.
+Buybackprogram is designed to use locally stored prices to speed up the price calculations. It is important that you have the price update task in your periodic tasks so that your prices will update.
 
-By adding the following lines in your `local.py` setting file the progral will update the stored item prices at midnight. This same task is also responsible for maintenance tasks such as removing unlinked tracking objects. It will also check for any new contracts and update the statistics page with them every 15 minutes:
+By adding the following lines in your `local.py` setting file the program will update the stored item prices at midnight. This same task is also responsible for maintenance tasks such as removing unlinked tracking objects. It will also check for any new contracts and update the statistics page with them every 30 minutes:
 
-```
-# Buybackprogram price updates
+```python
+# Buybackprogram price updates, updates prices at midnight
 CELERYBEAT_SCHEDULE['buybackprogram_update_all_prices'] = {
     'task': 'buybackprogram.tasks.update_all_prices',
     'schedule': crontab(minute=0, hour='0'),
 }
 
-# Buybackprogram contract updates
+# Buybackprogram contract updates, updates contracts every 30 minutes
 CELERYBEAT_SCHEDULE['buybackprogram_update_all_contracts'] = {
     'task': 'buybackprogram.tasks.update_all_contracts',
-    'schedule': crontab(minute='*/15'),
+    'schedule': crontab(minute='*/30'),
+}
+
+# Buybackprogram program performance updates, updates performance at midnight
+CELERYBEAT_SCHEDULE['buybackprogram_update_program_performance'] = {
+    'task': 'buybackprogram.tasks.update_program_performance',
+    'schedule': crontab(minute=0, hour='0'),
 }
 ```
 
-**Additional settings**
+#### Additional settings
+
 You may change the following settings by adding the lines in your `local.py` setting files
 
-Name | Description | Default
--- | -- | --
-BUYBACKPROGRAM_TRACKING_PREFILL | This is the prefill tag you will have on the tracking description for your contracts | aa-bbp.
-BUYBACKPROGRAM_PRICE_SOURCE_ID | Station ID for fetching base prices. Supports IDs listed on [Fuzzworks API](https://market.fuzzwork.co.uk/api/). Does not work with Janice API!| 60003760
-BUYBACKPROGRAM_PRICE_SOURCE_NAME | Display name of your price source. Has no effect on the actual price fetch which uses the ID. | Jita
+Name | Description | Default | Options
+-- | -- | -- | --
+BUYBACKPROGRAM_TRACKING_PREFILL | This is the prefill tag you will have on the tracking description for your contracts | aa-bbp. | Free text input
+BUYBACKPROGRAM_PRICE_SOURCE_ID | Station ID for fetching base prices. Supports IDs listed on [Fuzzwork API](https://market.fuzzwork.co.uk/api/). Does not work with Janice API!| 60003760 | See ID list
+BUYBACKPROGRAM_PRICE_SOURCE_NAME | Display name of your price source. Has no effect on the actual price fetch which uses the ID. | Jita | Free text input
 BUYBACKPROGRAM_PRICE_AGE_WARNING_LIMIT | Limit in hours when an item price is considered as outdated | 48
-BUYBACKPROGRAM_PRICE_METHOD | By default Fuzzwork API will be used for pricing, if this is set to "Janice" then the Janice API will be used. | Fuzzwork
-BUYBACKPROGRAM_PRICE_JANICE_API_KEY | The API key to access Janice API. |
-BUYBACKPROGRAM_UNUSED_TRACKING_PURGE_LIMIT | Time limit to remove unlinked tracking objects from the database. Set to 0 to never purge any tracking objects. | 48 hours
-BUYBACKPROGRAM_TRACK_PREFILL_CONTRACTS | Determines if we will track and store contracts that starts with the prefill phrase but do not have any actual tracking hits in database | True
+BUYBACKPROGRAM_PRICE_METHOD | By default Fuzzwork API will be used for pricing, if this is set to "Janice" then the Janice API will be used. | Fuzzwork | `Fuzzwork`, `Janice`
+BUYBACKPROGRAM_PRICE_INSTANT_PRICES | On default we use top 5% average prices. Set to `true` to change to instant prices | False | `False`, `True`
+BUYBACKPROGRAM_PRICE_JANICE_API_KEY | The API key to access Janice API. | `null` | `G9KwKq3465588VPd6747t95Zh94q3W2E`
+BUYBACKPROGRAM_UNUSED_TRACKING_PURGE_LIMIT | Time limit to remove unlinked tracking objects from the database. Set to 0 to never purge any tracking objects. | 48 | Any number in hours
+BUYBACKPROGRAM_TRACK_PREFILL_CONTRACTS | Determines if we will track and store contracts that starts with the prefill phrase but do not have any actual tracking hits in database | True | `True`, `False`
 
 Note: If you change your price source for an old install you need to wait for the price update task to run or manually run it to update your current database prices.
 
-Note: Using Janice API, Jita 4-4 prices will be used with the top 5% average price of the 5 day median price for buy and sell orders.
+Note: Using Janice API, Jita 4-4 prices will be used with the top 5% average price of the 5 day median price for buy and sell orders. No other price sources can be used with Janice
+
+### Step 6 - Adjust Permissions
 
-## Step 6 - Adjust Permissions
 Overview of all permissions in this program. Note that all permissions are in the "general" section.
 
 Name | Purpose | Example Target Audience
 -- | -- | --
 basic_access | Can access this app and see own statics. Can use buyback programs that are allowed by the buyback restriction rules. | Member State
 manage_programs | Can create new locations and buyback programs and manage their own buyback programs. Can see own buyback programs statics. | Buyback managers
 see_leaderboard | Can see the leaderboard stats for the programs that are visible for the user | Member State
 see_performance | Can see the performance stats for the programs that are visible to the user | Member / Managers
 see_all_statics | Can see all statistics in all buyback programs | Leadership
 
-## Step 7 - Program Setup
+### Step 7 - Program Setup
+
 After you have preloaded all the needed data you can start to setup programs.
 
 Each user with `manage_programs` permission is able to setup their own buyback programs.
 
-### Managers
+#### Managers
+
 Each buyback program is operated by a manager. To add a new manager click on the `setup manager` button.
 
-### Locations
+#### Locations
+
 Each buyback program operates at a location that is constructed of `SolarSystem` and a `Custom name` and an optional `Structure ID`. To add a new location click on the `add location` button on the buyback page.
 
-**Solar System & Name**
-Find a solar system by typing in the solar system box. Then determine a name for the structure. Most often you want to use the actual ingame name of the structure so that people are able to identify the location.
+##### Solar System & Name
 
-The solarsytem name will indicate your sellers where the program contract structure is located. The name will describe the structure name in where the contracts should be created and most often should be identical to the actual structure name ingame.
+Find a solar system by typing in the solar system box. Then determine a name for the structure. Most often you want to use the actual in-game name of the structure so that people are able to identify the location.
+
+The solar system name will indicate your sellers where the program contract structure is located. The name will describe the structure name in where the contracts should be created and most often should be identical to the actual structure name in-game.
+
+##### Structure ID
 
-**Structure ID**
 Structure ID is optional and will enable contract location tracking in the program statistics page. If a program location has been given a structure ID the statistics page will display a warning if the user has made the actual contract from some other structure than the one that was determined in the buyback program.
 
-The easiest way to find the actual structure id is to link the structure name into any chat box and post the structure name into the chat. This can be dont in any channel or the structure name can be also copied from any MOTDs.
+The easiest way to find the actual structure id is to link the structure name into any chat box and post the structure name into the chat. This can be done in any channel or the structure name can be also copied from any MOTDs.
 
 After you have posted the structure name in the chat right click it and press copy. You can now paste the structure into notepad or any other text editor and your output should look like this:
-```
+
+```plain
 [17:37:54] Ikarus Cesaille > <url=showinfo:35826//1037962518481>Oisio - LinkNet Central Station</url> `
 ```
+
 The unique structure ID for your structure is then `1037962518481`. Adding the ID to the location ID field will check if the contract creation location matches this ID.
 
-## Step 8 - Create Program
+### Step 8 - Create Program
+
 Once you have created a location and added at least one manager you can setup the actual program. Click on the `create program` button to create a new program.
 
-### Program settings
+#### Program settings
 
 Each program can be customized based on your needs. When setting up select the settings you wish to use.
 
-#### Owner
+##### Name/Description
+
+A display name for your program
+
+##### Manager
+
 This is the character or the characters corporation which will be used as the assign to target for buyback contracts at this location. To add more owners use the `add manager` button. You can only see your own characters.
 
-#### Is Corporation
+##### Is Corporation
+
 If you wish that the contracts are assigned to the owners corporation instead of the character tick this box.
 
-#### Tax
+##### Location
+
+The location where contracts should be created at. Only these locations are accepted
+
+##### Expiration
+
+Expiration time the contracts should bet set to.
+
+##### Price type
+
+You can select what price type is used as the base price for your calculations. You can select from either buy, sell or split prices.
+
+##### Default tax
+
 This is a general tax which is applied on all items in this program. If you wish to not allow all items in this program you can leave this to 0.
 
-General tax is applied on all items sold via the buyback. You can add additional taxes on individual items or ban them from beeing accepted to the program once you have created the program.
+General tax is applied on all items sold via the buyback. You can add additional taxes on individual items or ban them from being accepted to the program once you have created the program.
+
+##### Hauling fuel cost
 
-#### Hauling fuel cost
 You can add a fuel cost expense that is applied on each item sold via this program based on the volume of the item.
 
 > :information_source: This setting is aimed more to null sec buyback programs to make it easier to calculate your taxes and display your members the expenses you have when selling.
 
-#### Price density modifier
+##### Price density modifier
+
 You can use a price density modifier which will add a additional tax on items with low price per volume ratio such as T1 ships.
 
 > :information_source: This setting is aimer more at high sec buyback programs.
 
-#### Compressable price density modifier
-You can select to ignore price density calculations for items that can be compressed. This is helpful when the compressed variants do not have proper buy orders in Jita. If you set this to True then the compressable item density will be calculated based on the isk / volume of the compression variant of the sold item.
+##### Compressible price density modifier
+
+You can select to ignore price density calculations for items that can be compressed. This is helpful when the compressed variants do not have proper buy orders in Jita. If you set this to True then the compressible item density will be calculated based on the isk / volume of the compression variant of the sold item.
+
+##### Price density threshold
 
-#### Price density threshold
 This is the lowest isk/m^3 ratio for items that are accepted to the program without the price density tax. Finding your own limits depends on your logistical department.
 
 For example: Tritanium is 500 ISK/m³ @ 5 ISK per unit price. PLEX is 14,5Trillion ISK/m³ @2.9M per unit price.
 
-#### Price density tax
+##### Price density tax
+
 This is the tax which will be applied to items with a price density below the price density threshold
 
 > :warning: You should avoid using both the hauling fuel cost and the price density modifier at the same time as their function is fairly similar.
 
-#### Allow all items
+##### Allow all items
+
 If you wish to allow any types of items to be sold via this program keep this box ticker.
 
-You can determine individual increased taxes or ban items from beeing accepted to this program after creating the program.
+You can determine individual increased taxes or ban items from being accepted to this program after creating the program.
 
 If you do not want to accept all items you can set this box to False. By doing this you will need to set up a tax for each item you wish to accept into the program individually.
 
-### Ore settings
+#### Ore settings
+
 Ore type items such as asteroid, moon goo and ice have additional pricing methods you can use. You can use a mix of any of the three pricing models.
 
 > :information_source: When using more than one pricing model the best price will be used as the buy value.
 
-#### Use Refined value
+##### Use Refined value
+
 If you wish to calculate ore buyback value based on the mineral values tick this box.
 
-#### Use compressed value
+##### Use compressed value
+
 If you want to use compressed value as a pricing method tick this box.
 
-#### Use raw ore value
+##### Use raw ore value
+
 If you want to use raw ore value as a pricing method you can tick this box. Note that some ores such as Kernite and Moon Goo do not represent the real mineral value of the ores.
 
 You can also individually ban raw ore types from the program. If you have an other option than the raw ore value selected the price will be calculated based on the other pricing models.
 
-#### Allow unpacked items
+##### Allow unpacked items
+
 Most often you want to buy only items that are packed. This will ensure that people do not sell items such as broken ammo crystals for you.
 
-#### Refining rate
+##### Refining rate
+
 The refining rate is used in combination with the use refined value option.
 
-### Blue loot npc price
+#### Blue loot npc price
+
 If you cant to use NPC buy order prices for blue loot (Sleeper loot) instead of Jita prices check this box. NPC price for these items will always be used even when Jita price would be higher.
 
-### Red loot npc price
+#### Red loot npc price
+
 If you cant to use NPC buy order prices for red loot (Triglavian loot) instead of Jita prices check this box. NPC price for these items will always be used even when Jita price would be higher.
 
-### Restrctions
-You can restict the visibnility of the buyback programs to groups and states with the restriction options.
+#### Restrictions
+
+You can restrict the visibility of the buyback programs to groups and states with the restriction options.
 
 If no options are selected the program will be visible for everyone with the `basic_access` role.
 
 > :no_entry: Do not mix group and state restrictions as this may lead into logic error. If you need to mix then create a separate programs for them.
 
-### Discord DM messages
+#### Discord DM messages
+
 If you want to receive messages over discord for every new contract you can tick this box.
 
 > :information_source: Requires the [aa-discordbot plugin](https://github.com/pvyParts/allianceauth-discordbot) or [discordproxy app](https://gitlab.com/ErikKalkoken/discordproxy) to work
 
-### Discord channel messages
+#### Show list of items on discord message
+
+This option will determine if a list of all contract items is added into the discord message description field. If you are accepting all items the list may become very long. If set to false will show a link to the tracking page instead.
+
+#### Discord channel messages
+
 You can send notifications about new contracts directly into the discord channel which is linked to AUTH,
 
 > :information_source: Requires the [aa-discordbot plugin](https://github.com/pvyParts/allianceauth-discordbot) or [discordproxy app](https://gitlab.com/ErikKalkoken/discordproxy) to work
 
-## Step 9 - Special Taxes
+### Step 9 - Special Taxes
+
 You can modify individual item settings or allow items for a program that has set `allow all items = False` via the `special taxes` menu for each program.
 
-Set a item specific tax for each item. The tax wil be applied on top of the default tax for the program. You can also disallow an item from beeing accepted in the contract completely.
+Set a item specific tax for each item. The tax wil be applied on top of the default tax for the program. You can also disallow an item from being accepted in the contract completely.
 
 > :information_source: The item specific tax can also be a negative value allowing you to decrease taxes on certain items.
 
 To adjust individual item taxes inside a program click on the `Special taxes` button next to your program.
 
-You can either add items one by one with the `add item` button or add all items that belongs to a market group and every subchild market group of that group with `add market group`
+You can either add items one by one with the `add item` button or add all items that belongs to a market group and every sub-child market group of that group with `add market group`
 
 You can edit an item on the taxation table simply by adding it again. To delete the item press the delete button next to it or to delete all items in the program click on the delete all items button.
 
-**Market Groups**
+#### Market Groups
+
 When you add an market group each item inside that market group, the child of the market group and the child of the child group will be added to the item taxes (3 steps down)
 
-The easiest way to check which items are under which market group is to open the market window ingame or third party programs such as [https://evemarketer.com/](https://evemarketer.com/)
+The easiest way to check which items are under which market group is to open the market window in-game or third party programs such as [https://evemarketer.com/](https://evemarketer.com/)
 
 Example:
 
 Market group `Minerals` is the bottom market group that includes the standard minerals. Adding this market group to the taxation will add 8 items to the taxes (Tritanium, Pyerite etc.)
 
-Market group `Standard ores` is a parent gategory and there are no direct items under this category. However this category has child categories such as Veldsar, Jaspet, Scordite which each includes multiple variations of the ores. Adding the `Standard ores` category will add each ore type to the special tax section.
+Market group `Standard ores` is a parent category and there are no direct items under this category. However this category has child categories such as Veldspar, Jaspet, Scordite which each includes multiple variations of the ores. Adding the `Standard ores` category will add each ore type to the special tax section.
+
+#### Most Common Groups
 
-**Most Common Groups**
 Name | Includes | Items
 -- | --
 Standard Ores | Normal ores from belts and anomalies | Veldspar, Hedbergite, Compressed Arkonor ...
 Moon Ores | Ores from moon mining | Cobaltite, Loparite, Pollucite
 Ice Ores | Ores from ice mining | Blue Ice, Dark Glitter, Compressed Blue Ice ....
 Minerals | Contains materials for refining Standard Ore | Tritanium, Pyerite ....
 Salvage Materials | Salvage from loot | Armor Plates, Trigger Unit, Ancient Radar Decorrelator ...
```

### Comparing `aa-buybackprogram-1.9.1/buybackprogram/admin.py` & `aa_buybackprogram-2.0.0/buybackprogram/admin.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from django.contrib import admin
 
-from .models import Contract, Location, Owner, Program
+from .models import Contract, Faq, Location, Owner, Program
 
 # Register your models here.
 
 
 class ProgramAdmin(admin.ModelAdmin):
     model = Program
 
@@ -32,14 +32,25 @@
         else:
             return None
 
     _location.short_description = "Location"
     _location.admin_order_field = "location__name"
 
 
+class FaqAdmin(admin.ModelAdmin):
+    model = Program
+
+    list_display = (
+        "header",
+        "body",
+    )
+
+
 admin.site.register(Program, ProgramAdmin)
 
 admin.site.register(Owner)
 
 admin.site.register(Contract)
 
 admin.site.register(Location)
+
+admin.site.register(Faq, FaqAdmin)
```

### Comparing `aa-buybackprogram-1.9.1/buybackprogram/app_settings.py` & `aa_buybackprogram-2.0.0/buybackprogram/app_settings.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,25 @@
+import re
+
 from django.conf import settings
 
 from .utils import clean_setting
 
 # put your app settings here
 
 
-EXAMPLE_SETTING_ONE = getattr(settings, "EXAMPLE_SETTING_ONE", None)
+def get_site_url():  # regex sso url
+    regex = r"^(.+)\/s.+"
+    matches = re.finditer(regex, settings.ESI_SSO_CALLBACK_URL, re.MULTILINE)
+    url = "http://"
+
+    for m in matches:
+        url = m.groups()[0]  # first match
+
+    return url
 
 
 # Hard timeout for tasks in seconds to reduce task accumulation during outages
 BUYBACKPROGRAM_TASKS_TIME_LIMIT = clean_setting("BUYBACKPROGRAM_TASKS_TIME_LIMIT", 7200)
 
 # Warning limit for Jita price updates if prices have not been updated
 BUYBACKPROGRAM_PRICE_AGE_WARNING_LIMIT = clean_setting(
@@ -34,14 +44,18 @@
     "BUYBACKPROGRAM_PRICE_SOURCE_ID", 60003760
 )
 
 BUYBACKPROGRAM_PRICE_SOURCE_NAME = clean_setting(
     "BUYBACKPROGRAM_PRICE_SOURCE_NAME", "Jita"
 )
 
+BUYBACKPROGRAM_PRICE_INSTANT_PRICES = clean_setting(
+    "BUYBACKPROGRAM_PRICE_INSTANT_PRICES", False
+)
+
 BUYBACKPROGRAM_PRICE_METHOD = clean_setting("BUYBACKPROGRAM_PRICE_METHOD", "Fuzzwork")
 
 BUYBACKPROGRAM_PRICE_JANICE_API_KEY = clean_setting(
     "BUYBACKPROGRAM_PRICE_JANICE_API_KEY", ""
 )
```

### Comparing `aa-buybackprogram-1.9.1/buybackprogram/auth_hooks.py` & `aa_buybackprogram-2.0.0/buybackprogram/auth_hooks.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     """This class ensures only authorized users will see the menu entry"""
 
     def __init__(self):
         # setup menu entry for sidebar
         MenuItemHook.__init__(
             self,
             _("Buyback Program"),
-            "fas fa-cube fa-fw",
+            "fa-solid fa-store",
             "buybackprogram:index",
             navactive=["buybackprogram:"],
         )
 
     def render(self, request):
         if request.user.has_perm("buybackprogram.basic_access"):
             return MenuItemHook.render(self, request)
```

### Comparing `aa-buybackprogram-1.9.1/buybackprogram/decorators.py` & `aa_buybackprogram-2.0.0/buybackprogram/decorators.py`

 * *Files identical despite different names*

### Comparing `aa-buybackprogram-1.9.1/buybackprogram/forms.py` & `aa_buybackprogram-2.0.0/buybackprogram/forms.py`

 * *Files 2% similar despite different names*

```diff
@@ -127,14 +127,19 @@
     )
     donation = forms.IntegerField(
         label="Donation %",
         initial=0,
         help_text="You can set a optional donation percentage on your contract",
         validators=[MaxValueValidator(100), MinValueValidator(0)],
     )
+    additional_notes = forms.CharField(
+        label="Additional Notes",
+        help_text="You can set additional notes for your contract in here",
+        required=False,  # Make sure it's not required
+    )
 
 
 class UserSettingsForm(forms.ModelForm):
     """
     User settings form
     """
```

### Comparing `aa-buybackprogram-1.9.1/buybackprogram/helpers.py` & `aa_buybackprogram-2.0.0/buybackprogram/helpers.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,21 @@
+import statistics
 import uuid
 
 import requests
 
 from django.db import Error
 from django.utils import timezone
 from eveuniverse.models import EveMarketPrice, EveType, EveTypeMaterial
 
 from allianceauth.services.hooks import get_extension_logger
 
 from buybackprogram.app_settings import (
     BUYBACKPROGRAM_PRICE_AGE_WARNING_LIMIT,
+    BUYBACKPROGRAM_PRICE_INSTANT_PRICES,
     BUYBACKPROGRAM_PRICE_JANICE_API_KEY,
     BUYBACKPROGRAM_PRICE_METHOD,
     BUYBACKPROGRAM_PRICE_SOURCE_ID,
     BUYBACKPROGRAM_TRACKING_PREFILL,
 )
 from buybackprogram.constants import (
     BLUE_LOOT_TYPE_IDS,
@@ -82,30 +84,38 @@
                 },
             )
 
             items_fuzzwork = response_fuzzwork.json()
 
             buy = int(float(items_fuzzwork[str(item_id)]["buy"]["max"]))
             sell = int(float(items_fuzzwork[str(item_id)]["sell"]["min"]))
+            buy_average = int(float(items_fuzzwork[str(item_id)]["buy"]["percentile"]))
+            sell_average = int(
+                float(items_fuzzwork[str(item_id)]["sell"]["percentile"])
+            )
 
         elif BUYBACKPROGRAM_PRICE_METHOD == "Janice":
             if valid_janice_api_key():
                 response_janice = requests.get(
                     f"https://janice.e-351.com/api/rest/v2/pricer/{item_id}",
                     headers={
                         "Content-Type": "text/plain",
                         "X-ApiKey": BUYBACKPROGRAM_PRICE_JANICE_API_KEY,
                         "accept": "application/json",
                     },
                 )
 
                 item_janice = response_janice.json()
 
-                buy = int(float(item_janice["top5AveragePrices"]["buyPrice5DayMedian"]))
-                sell = int(
+                buy = int(float(item_janice["immediatePrices"]["buyPrice5DayMedian"]))
+                sell = int(float(item_janice["immediatePrices"]["sellPrice5DayMedian"]))
+                buy_average = int(
+                    float(item_janice["top5AveragePrices"]["buyPrice5DayMedian"])
+                )
+                sell_average = int(
                     float(item_janice["top5AveragePrices"]["sellPrice5DayMedian"])
                 )
             else:
                 logger.error(
                     "Price setup failed for Janice, invalid API key! Provide a working key or change price source to Fuzzwork"
                 )
 
@@ -114,17 +124,30 @@
 
         else:
             raise f"Unknown pricing method: {BUYBACKPROGRAM_PRICE_METHOD}"
 
         updated = timezone.now()
 
         try:
-            price = ItemPrices.objects.create(
-                eve_type_id=item_id, buy=buy, sell=sell, updated=updated
+            # Check what prices we should use either instant prices or top 5% percentile
+            logger.debug(
+                "Price type instant price is set to %s"
+                % BUYBACKPROGRAM_PRICE_INSTANT_PRICES
             )
+            if not BUYBACKPROGRAM_PRICE_INSTANT_PRICES:
+                price = ItemPrices.objects.create(
+                    eve_type_id=item_id,
+                    buy=buy_average,
+                    sell=sell_average,
+                    updated=updated,
+                )
+            else:
+                price = ItemPrices.objects.create(
+                    eve_type_id=item_id, buy=buy, sell=sell, updated=updated
+                )
 
             return price
         except Error as e:
             logger.error("Error updating prices: %s" % e)
 
 
 def get_npc_price(item_id):
@@ -435,15 +458,27 @@
     compression_raw_value = False
 
     # RAW VARIANT VALUES
     if item_prices["raw_prices"] and item_prices["raw_prices"]["raw_price_used"]:
         quantity = item_prices["raw_prices"]["quantity"]
         sell = item_prices["raw_prices"]["sell"]
         buy = item_prices["raw_prices"]["buy"]
-        price = buy
+        split = statistics.median([sell, buy])
+
+        # Determine what price type we should use
+        if program.price_type == "Buy":
+            price = buy
+        elif program.price_type == "Sell":
+            price = sell
+        elif program.price_type == "Split":
+            price = split
+
+        logger.debug(
+            "Using price value type '%s' with value %s" % (program.price_type, price)
+        )
 
         if not item_type.volume <= 0:
             price_dencity = price / item_type.volume
         else:
             price_dencity = False
         price_dencity_tax = get_price_dencity_tax(
             program, price, item_type.volume, quantity, is_ore(item_type.eve_group.id)
@@ -563,15 +598,32 @@
 
         for material in item_prices["material_prices"]:
             materials = EveType.objects.filter(id=material["id"]).first()
 
             quantity = material["quantity"]
             sell = material["sell"]
             buy = material["buy"]
-            price = buy
+            split = statistics.median([sell, buy])
+
+            # Determine what price type we should use
+            if program.price_type == "Buy":
+                price = buy
+                logger.debug(
+                    "Using price type '%s' with value %s" % (program.price_type, price)
+                )
+            elif program.price_type == "Sell":
+                price = sell
+                logger.debug(
+                    "Using price type '%s' with value %s" % (program.price_type, price)
+                )
+            elif program.price_type == "Split":
+                price = split
+                logger.debug(
+                    "Using price type '%s' with value %s" % (program.price_type, price)
+                )
             program_tax = program.tax
             refining_rate = float(program.refining_rate) / 100
             tax_multiplier = (100 - (program_tax + item_tax + price_dencity_tax)) / 100
 
             raw_value = quantity * refining_rate * price
             value = raw_value * tax_multiplier
 
@@ -624,15 +676,32 @@
         compressed_version = EveType.objects.filter(
             id=item_prices["compression_prices"]["id"]
         ).first()
 
         quantity = item_prices["compression_prices"]["quantity"]
         buy = item_prices["compression_prices"]["buy"]
         sell = item_prices["compression_prices"]["sell"]
-        price = buy
+        split = statistics.median([sell, buy])
+
+        # Determine what price type we should use
+        if program.price_type == "Buy":
+            price = buy
+            logger.debug(
+                "Using price type '%s' with value %s" % (program.price_type, price)
+            )
+        elif program.price_type == "Sell":
+            price = sell
+            logger.debug(
+                "Using price type '%s' with value %s" % (program.price_type, price)
+            )
+        elif program.price_type == "Split":
+            price = split
+            logger.debug(
+                "Using price type '%s' with value %s" % (program.price_type, price)
+            )
         price_dencity = price / compressed_version.volume
 
         logger.debug("Getting price density for compressed variant")
 
         price_dencity_tax = get_price_dencity_tax(
             program,
             price,
@@ -686,15 +755,32 @@
     logger.debug("Values: Item compressed unit value is %s" % compressed["unit_value"])
 
     # Get value for NPC price
     if item_prices["npc_prices"]:
         quantity = item_prices["npc_prices"]["quantity"]
         sell = item_prices["npc_prices"]["sell"]
         buy = item_prices["npc_prices"]["buy"]
-        price = buy
+        split = statistics.median([sell, buy])
+
+        # Determine what price type we should use
+        if program.price_type == "Buy":
+            price = buy
+            logger.debug(
+                "Using price type '%s' with value %s" % (program.price_type, price)
+            )
+        elif program.price_type == "Sell":
+            price = sell
+            logger.debug(
+                "Using price type '%s' with value %s" % (program.price_type, price)
+            )
+        elif program.price_type == "Split":
+            price = split
+            logger.debug(
+                "Using price type '%s' with value %s" % (program.price_type, price)
+            )
 
         if not item_type.volume <= 0:
             price_dencity = price / item_type.volume
         else:
             price_dencity = False
         price_dencity_tax = get_price_dencity_tax(
             program, price, item_type.volume, quantity, is_ore(item_type.eve_group.id)
@@ -989,15 +1075,15 @@
         "buy_value": False,
     }
 
     return values
 
 
 def get_tracking_number(
-    user, program, form_donation, buyback_data, contract_price_data
+    user, program, form_donation, buyback_data, contract_price_data, additional_notes
 ):
     try:
         last_id = Tracking.objects.last().id
     except AttributeError:
         last_id = 0
 
     tracking_number = (
@@ -1019,14 +1105,15 @@
         value=contract_price_data["total_all_items_raw"],
         taxes=contract_price_data["total_tax_amount"],
         hauling_cost=contract_price_data["total_hauling_cost"],
         donation=contract_price_data["total_donation_amount"],
         net_price=round(contract_price_data["contract_net_total"]),
         tracking_number=tracking_number,
         created_at=timezone.now(),
+        additional_notes=additional_notes,
     )
 
     tracking.save()
 
     objs = []
 
     for item in buyback_data:
```

### Comparing `aa-buybackprogram-1.9.1/buybackprogram/management/commands/buybackprogram_generate_test_data.py` & `aa_buybackprogram-2.0.0/buybackprogram/management/commands/buybackprogram_generate_test_data.py`

 * *Files identical despite different names*

### Comparing `aa-buybackprogram-1.9.1/buybackprogram/management/commands/buybackprogram_link_contracts.py` & `aa_buybackprogram-2.0.0/buybackprogram/management/commands/buybackprogram_link_contracts.py`

 * *Files identical despite different names*

### Comparing `aa-buybackprogram-1.9.1/buybackprogram/management/commands/buybackprogram_load_prices.py` & `aa_buybackprogram-2.0.0/buybackprogram/management/commands/buybackprogram_load_prices.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from django.db import IntegrityError
 from django.utils import timezone
 from eveuniverse.models import EveMarketPrice, EveType
 
 from allianceauth.services.hooks import get_extension_logger
 
 from buybackprogram.app_settings import (
+    BUYBACKPROGRAM_PRICE_INSTANT_PRICES,
     BUYBACKPROGRAM_PRICE_METHOD,
     BUYBACKPROGRAM_PRICE_SOURCE_ID,
     BUYBACKPROGRAM_PRICE_SOURCE_NAME,
 )
 from buybackprogram.models import ItemPrices
 from buybackprogram.tasks import get_bulk_prices, valid_janice_api_key
 
@@ -28,26 +29,32 @@
         api_up = True
 
         # Get all type ids
         typeids = EveType.objects.values_list("id", flat=True).filter(published=True)
 
         if BUYBACKPROGRAM_PRICE_METHOD == "Fuzzwork":
             print(
-                "Price setup starting for %s items from Fuzzworks API from station id %s (%s), this may take up to 30 seconds..."
+                "Price setup starting for %s items from Fuzzworks API from station id %s (%s). Use instant prices instead of average is set to %s, this may take up to 30 seconds..."
                 % (
                     len(typeids),
                     BUYBACKPROGRAM_PRICE_SOURCE_ID,
                     BUYBACKPROGRAM_PRICE_SOURCE_NAME,
+                    BUYBACKPROGRAM_PRICE_INSTANT_PRICES,
                 )
             )
         elif BUYBACKPROGRAM_PRICE_METHOD == "Janice":
             if valid_janice_api_key():
                 print(
-                    "Price setup starting for %s items from Janice API for Jita 4-4, this may take up to 30 seconds..."
-                    % (len(typeids))
+                    "Price setup starting for %s items from Janice API from station id %s (%s). Use instant prices instead of average is set to %s, this may take up to 30 seconds..."
+                    % (
+                        len(typeids),
+                        BUYBACKPROGRAM_PRICE_SOURCE_ID,
+                        BUYBACKPROGRAM_PRICE_SOURCE_NAME,
+                        BUYBACKPROGRAM_PRICE_INSTANT_PRICES,
+                    )
                 )
             else:
                 print(
                     "\033[91mPrice setup failed for Janice, invalid API key! Provide a working key or change price source to Fuzzwork\033[91m\033[0m"
                 )
 
                 api_up = False
@@ -70,20 +77,28 @@
             market_data.update(get_bulk_prices(type_ids))
 
             objs = []
 
             for key, value in market_data.items():
                 item_count += 1
 
-                item = ItemPrices(
-                    eve_type_id=key,
-                    buy=int(float(value["buy"]["max"])),
-                    sell=int(float(value["sell"]["min"])),
-                    updated=timezone.now(),
-                )
+                if not BUYBACKPROGRAM_PRICE_INSTANT_PRICES:
+                    item = ItemPrices(
+                        eve_type_id=key,
+                        buy=int(float(value["buy"]["percentile"])),
+                        sell=int(float(value["sell"]["percentile"])),
+                        updated=timezone.now(),
+                    )
+                else:
+                    item = ItemPrices(
+                        eve_type_id=key,
+                        buy=int(float(value["buy"]["max"])),
+                        sell=int(float(value["sell"]["min"])),
+                        updated=timezone.now(),
+                    )
 
                 objs.append(item)
             try:
                 ItemPrices.objects.bulk_create(objs)
 
                 print("Succesfully setup %s prices." % item_count)
             except IntegrityError:
```

### Comparing `aa-buybackprogram-1.9.1/buybackprogram/migrations/0001_initial.py` & `aa_buybackprogram-2.0.0/buybackprogram/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `aa-buybackprogram-1.9.1/buybackprogram/migrations/0002_contractnotification.py` & `aa_buybackprogram-2.0.0/buybackprogram/migrations/0002_contractnotification.py`

 * *Files identical despite different names*

### Comparing `aa-buybackprogram-1.9.1/buybackprogram/migrations/0003_statics_performance_increase.py` & `aa_buybackprogram-2.0.0/buybackprogram/migrations/0003_statics_performance_increase.py`

 * *Files identical despite different names*

### Comparing `aa-buybackprogram-1.9.1/buybackprogram/migrations/0004_auto_20220323_1331.py` & `aa_buybackprogram-2.0.0/buybackprogram/migrations/0004_auto_20220323_1331.py`

 * *Files identical despite different names*

### Comparing `aa-buybackprogram-1.9.1/buybackprogram/migrations/0005_program_compression_price_dencity_modifier.py` & `aa_buybackprogram-2.0.0/buybackprogram/migrations/0005_program_compression_price_dencity_modifier.py`

 * *Files identical despite different names*

### Comparing `aa-buybackprogram-1.9.1/buybackprogram/migrations/0006_program_bonds_npc_price_and_more.py` & `aa_buybackprogram-2.0.0/buybackprogram/migrations/0006_program_bonds_npc_price_and_more.py`

 * *Files identical despite different names*

### Comparing `aa-buybackprogram-1.9.1/buybackprogram/migrations/0007_program_expiration.py` & `aa_buybackprogram-2.0.0/buybackprogram/migrations/0007_program_expiration.py`

 * *Files identical despite different names*

### Comparing `aa-buybackprogram-1.9.1/buybackprogram/migrations/0008_alter_general_options_alter_program_refining_rate.py` & `aa_buybackprogram-2.0.0/buybackprogram/migrations/0008_alter_general_options_alter_program_refining_rate.py`

 * *Files identical despite different names*

### Comparing `aa-buybackprogram-1.9.1/buybackprogram/migrations/0010_contract_no_tracking_alter_tracking_tracking_number.py` & `aa_buybackprogram-2.0.0/buybackprogram/migrations/0010_contract_no_tracking_alter_tracking_tracking_number.py`

 * *Files identical despite different names*

### Comparing `aa-buybackprogram-1.9.1/buybackprogram/models.py` & `aa_buybackprogram-2.0.0/buybackprogram/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,18 +19,18 @@
 
 from buybackprogram.notification import (
     send_message_to_discord_channel,
     send_user_notification,
 )
 
 from .app_settings import (
-    BUYBACKPROGRAM_TRACKING_PREFILL,
     BUYBACKPROGRAM_TRACK_PREFILL_CONTRACTS,
+    BUYBACKPROGRAM_TRACKING_PREFILL,
+    get_site_url,
 )
-
 from .decorators import fetch_token_for_owner
 from .providers import esi
 
 logger = get_extension_logger(__name__)
 
 
 def get_sentinel_user():
@@ -117,14 +117,15 @@
         # Get all contracts for owner corporation
         corporation_contracts = self._fetch_corporation_contracts()
 
         logger.debug("Got %s corporation contracts" % len(corporation_contracts))
 
         # Merge all contracts into a single list
         all_contracts = contracts + corporation_contracts
+        tracked_contrats = list()
 
         logger.debug("Total contracts received: %s" % len(all_contracts))
 
         # Get all tracking objects from the database
         tracking_numbers = Tracking.objects.all()
 
         logger.debug("Got %s tracking numbers from database" % len(tracking_numbers))
@@ -135,22 +136,34 @@
             if tracking.program:
                 # Start checking if we find any matches from our ESI contracts
                 for contract in all_contracts:
                     # Only get contracts with the correct prefill ticker
                     if tracking.tracking_number in contract["title"]:
                         self._process_contract(contract, tracking, token)
 
+                        tracked_contrats.append(contract)
+
                         break  # If we have found a match from our ESI contracts wi will stop looping on the contract
 
         # Check for possible scam contracts that are pretending to be buyback contracts
 
         if BUYBACKPROGRAM_TRACK_PREFILL_CONTRACTS:
             logger.debug("Starting untracked contracts check")
 
-            for contract in all_contracts:
+            # Check what contracts we already have processed earlier
+            untracked_contracts = [
+                x for x in all_contracts if x not in tracked_contrats
+            ]
+
+            logger.debug(
+                "Found %s untracked contracts out of %s"
+                % (len(untracked_contracts), len(all_contracts))
+            )
+
+            for contract in untracked_contracts:
                 if BUYBACKPROGRAM_TRACKING_PREFILL in contract["title"]:
                     try:
                         tracking = Tracking.objects.get(
                             tracking_number__contains=contract["title"]
                         )
                         logger.debug(
                             "Contract %s already tracked, passing"
@@ -297,28 +310,35 @@
                 corporations = CharacterOwnership.objects.filter(
                     user=tracking.program.owner.user
                 ).values_list("character__corporation_id", flat=True)
 
                 logger.debug("Got corporations for contract owner: %s" % corporations)
 
                 objs = []
+                items = []
 
                 # Prepare objects for bulk create
                 for item in contract_items:
                     cont = Contract.objects.get(contract_id=contract["contract_id"])
                     itm, _ = EveType.objects.get_or_create_esi(id=item["type_id"])
 
                     contract_item = ContractItem(
                         contract=cont,
                         eve_type=itm,
                         quantity=item["quantity"],
                     )
 
                     objs.append(contract_item)
 
+                    items.append(
+                        str(EveType.objects.get(id=item["type_id"]))
+                        + " x "
+                        + str(item["quantity"])
+                    )
+
                 try:
                     ContractItem.objects.bulk_create(objs)
                     logger.debug(
                         "Succesfully added %s items for contract %s into database"
                         % (len(objs), contract["contract_id"])
                     )
                 except Error as e:
@@ -342,33 +362,58 @@
                 notifications = ContractNotification.objects.filter(
                     contract__contract_id=contract["contract_id"]
                 )
 
                 notes = str()
 
                 if notifications:
-                    notes += "\n\n**Notes**:\n"
                     for note in notifications:
                         notes += str(note.message)
                         notes += "\n\n"
 
+                logger.debug("Contract contains %s" % "\n".join(items))
+
+                # Check if the program wants to display the item list
+                if tracking.program.discord_show_item_list:
+                    contract_item_list = "\n".join(items)
+                else:
+                    contract_item_list = ""
+
+                contract_url = (
+                    get_site_url()
+                    + "/buybackprogram/tracking/"
+                    + tracking.tracking_number
+                )
+
+                # Limit contract items to fit into embed limitations
+                if (
+                    len(contract_item_list) > 2000
+                    or not tracking.program.discord_show_item_list
+                ):
+                    contract_item_list = (
+                        contract_item_list
+                        + "\n[See all contract items ...]("
+                        + contract_url
+                        + ")"
+                    )
+
                 user_message = {
-                    "title": "New buyback contract assigned",
-                    "description": "A new contract with tracking number {0} has been assigned to buyback program {1}.{2}".format(
-                        tracking.tracking_number,
-                        tracking.program.name,
-                        notes,
+                    "contract": obj,
+                    "contract_items": contract_item_list,
+                    "tracking": tracking,
+                    "notes": notes,
+                    "title": "New buyback contract assigned for program {0}".format(
+                        tracking.program.name
                     ),
                     "color": 0x5BC0DE,
                     "value": intcomma(int(contract["price"])),
                     "assigned_to": assigned_to,
                     "assigned_from": EveEntity.objects.resolve_name(
                         contract["issuer_id"]
                     ),
-                    "footer": "Hint: You can disable these notifications from your program settings",
                 }
 
                 # If tracking is active and we should send a message for our users
                 if tracking.program.discord_dm_notification:
                     send_user_notification(
                         user=self.user,
                         level="success",
@@ -433,36 +478,32 @@
                         status = contract["status"]
 
                     notifications = ContractNotification.objects.filter(
                         contract__contract_id=contract["contract_id"]
                     )
 
                     notes = str()
+                    items = []
 
                     if notifications:
-                        notes += "\n\n**Notes**:\n"
                         for note in notifications:
                             notes += str(note.message)
                             notes += "\n\n"
 
                     user_message = {
-                        "title": "Buyback contract {0}".format(status),
-                        "description": "Your outstanding buyback contract {0} has been {1} by {2}.{3}".format(
-                            tracking.tracking_number,
-                            status,
-                            self.character.character,
-                            notes,
-                        ),
+                        "contract": obj,
+                        "tracking": tracking,
+                        "title": "Your buyback contract has been {0}".format(status),
                         "color": color,
+                        "notes": notes,
                         "value": intcomma(int(contract["price"])),
                         "assigned_to": assigned_to,
                         "assigned_from": EveEntity.objects.resolve_name(
                             contract["issuer_id"]
                         ),
-                        "footer": "Hint: You can disable these notifications from your buybackprogram settings",
                     }
 
                     send_user_notification(
                         user=tracking.issuer_user,
                         level=level,
                         message=user_message,
                     )
@@ -701,14 +742,15 @@
         # List for all notes
         notes = []
 
         note = ContractNotification(
             contract=contract,
             icon="fa-theater-masks",
             color="red",
+            header="Suspicious Contract",
             message="Contract has no tracking object but is has a buyback prefill text! Possibly a scam contract.",
         )
 
         notes.append(note)
 
         try:
             ContractNotification.objects.bulk_create(notes)
@@ -758,93 +800,111 @@
         logger.debug("Got contract items: %s" % (contract_items))
 
         if tracking_items != contract_items:
             note = ContractNotification(
                 contract=contract,
                 icon="fa-unlink",
                 color="red",
+                header="Item missmatch",
                 message="Tracked items do not match the actual items in the contract. See details for more info.",
             )
 
             notes.append(note)
 
         # If our tracked price is different than the actual contract price
         if tracking.net_price >= 0 and tracking.net_price != contract.price:
             # If contract price is bellow tracked price
             if contract.price > tracking.net_price:
                 note = ContractNotification(
                     contract=contract,
                     icon="fa-dollar-sign",
                     color="red",
+                    header="High ask price",
                     message="Ask price is above the calculated price for this contract",
                 )
 
                 notes.append(note)
 
             else:
                 note = ContractNotification(
                     contract=contract,
                     icon="fa-dollar-sign",
                     color="orange",
+                    header="low ask price",
                     message="Ask price is bellow the calculated price for this contract",
                 )
 
                 notes.append(note)
 
         if structure_id and contract.start_location_id not in structure_id:
             note = ContractNotification(
                 contract=contract,
                 icon="fa-compass",
                 color="red",
+                header="Location missmatch",
                 message="Contract location does not match program location",
             )
 
             notes.append(note)
 
         if contract.assignee_id in corporations and not tracking.program.is_corporation:
             note = ContractNotification(
                 contract=contract,
                 icon="fa-home",
                 color="orange",
+                header="Receiver missmatch",
                 message="Contract is made for corporation while it should be made directly to the program managers character",
             )
 
             notes.append(note)
 
         if contract.assignee_id not in corporations and tracking.program.is_corporation:
             note = ContractNotification(
                 contract=contract,
                 icon="fa-user",
                 color="orange",
+                header="Receiver missmatch",
                 message="Contract is made for the program managers character while it should be made to the managers corporation",
             )
 
             notes.append(note)
 
         if not tracking.tracking_number == contract.title:
             note = ContractNotification(
                 contract=contract,
                 icon="fa-exclamation",
                 color="orange",
+                header="Title variation",
                 message="Contract description contains extra characterse besides the tracking number. The description should be: '%s', instead it is: '%s'"
                 % (tracking.tracking_number, contract.title),
             )
 
             notes.append(note)
 
         if tracking.donation:
             note = ContractNotification(
                 contract=contract,
                 icon="fa-hand-holding-usd",
                 color="green",
+                header="Donation",
                 message="Contact contains a donation",
             )
 
             notes.append(note)
 
+        if tracking.additional_notes:
+            note = ContractNotification(
+                contract=contract,
+                icon="fa-message",
+                header="Additional notes",
+                message="Extra notes provided by the seller",
+            )
+
+            notes.append(note)
+
         try:
             ContractNotification.objects.bulk_create(notes)
 
             logger.debug(
                 "Succesfully added items for contract %s into database"
                 % contract.contract_id
             )
@@ -970,14 +1030,19 @@
     class Expiration(models.TextChoices):
         DAY1 = "1 Day", _("1 Day")
         DAY3 = "3 Days", _("3 Days")
         WEEK1 = "1 Week", _("1 Week")
         WEEK2 = "2 Weeks", _("2 Weeks")
         WEEK4 = "4 Weeks", _("4 Weeks")
 
+    class PriceType(models.TextChoices):
+        BUY = "Buy", _("Buy")
+        SELL = "Sell", _("Sell")
+        SPLIT = "Split", _("Split")
+
     name = models.CharField(
         verbose_name="Name/description",
         max_length=64,
         help_text="A name or a description for this program",
         blank=True,
         default="",
     )
@@ -1004,14 +1069,21 @@
     expiration = models.CharField(
         max_length=7,
         choices=Expiration.choices,
         default=Expiration.WEEK2,
         help_text="Expiration time the contracts should bet set to.",
     )
 
+    price_type = models.CharField(
+        max_length=7,
+        choices=PriceType.choices,
+        default=PriceType.BUY,
+        help_text="What prices should we use as the source for prices. Default: Buy",
+    )
+
     tax = models.IntegerField(
         verbose_name="Default tax",
         default=0,
         blank=False,
         null=False,
         help_text="A default tax rate in this program that is applied on all items.",
         validators=[MaxValueValidator(100), MinValueValidator(0)],
@@ -1128,14 +1200,20 @@
 
     discord_dm_notification = models.BooleanField(
         verbose_name="Discord direct messages for new contracts",
         default=False,
         help_text="Check if you want to receive a direct message notification each time a new contract is created. <b>Requires aa-discordbot app or discordproxy app to work</b>",
     )
 
+    discord_show_item_list = models.BooleanField(
+        verbose_name="Show list of items on discord message",
+        default=False,
+        help_text="Determines if you want to show the contract items in the discord messages. This applies to both webhooks and direct messages.",
+    )
+
     discord_channel_notification = models.CharField(
         verbose_name="Discord webhook for notifications",
         max_length=256,
         null=True,
         blank=True,
         help_text="Discord webhook to send contract notifications to.",
     )
@@ -1210,30 +1288,31 @@
     sell = models.BigIntegerField()
     updated = models.DateTimeField()
 
 
 class Contract(models.Model):
     assignee_id = models.IntegerField()
     availability = models.CharField(max_length=20)
-    contract_id = models.IntegerField()
+    contract_id = models.IntegerField(unique=True)
     date_completed = models.DateTimeField(null=True)
     date_expired = models.DateTimeField(null=True)
     date_issued = models.DateTimeField()
     for_corporation = models.BooleanField()
     issuer_corporation_id = models.IntegerField()
     issuer_id = models.IntegerField()
     start_location_id = models.BigIntegerField(null=True)
     location_name = models.CharField(max_length=128, null=True)
     price = models.BigIntegerField()
     status = models.CharField(max_length=30)
     title = models.CharField(max_length=128)
     volume = models.BigIntegerField()
-    no_tracking = models.BooleanField(
-        default=False,
-    )
+    no_tracking = models.BooleanField(default=False)
+
+    def __str__(self) -> str:
+        return str(self.contract_id)
 
 
 class ContractItem(models.Model):
     contract = models.ForeignKey(
         Contract,
         on_delete=models.deletion.CASCADE,
         help_text="What contract do these items belong to",
@@ -1258,14 +1337,20 @@
         max_length=64,
     )
 
     color = models.CharField(
         max_length=32,
     )
 
+    header = models.CharField(
+        max_length=1024,
+        null=True,
+        blank=True,
+    )
+
     message = models.CharField(
         max_length=1024,
     )
 
 
 class Tracking(models.Model):
     program = models.ForeignKey(
@@ -1288,14 +1373,15 @@
     value = models.BigIntegerField(null=False)
     taxes = models.BigIntegerField(null=False)
     hauling_cost = models.BigIntegerField(null=False)
     donation = models.BigIntegerField(null=True, blank=True)
     net_price = models.BigIntegerField(null=False)
     tracking_number = models.CharField(max_length=32)
     created_at = models.DateTimeField(null=True, blank=True)
+    additional_notes = models.TextField(null=True, blank=True)
 
 
 class TrackingItem(models.Model):
     tracking = models.ForeignKey(
         Tracking,
         on_delete=models.deletion.CASCADE,
         help_text="What tracking do these items belong to",
@@ -1334,7 +1420,15 @@
         """
         Meta definitions
         """
 
         default_permissions = ()
         verbose_name = _("User Settings")
         verbose_name_plural = _("User Settings")
+
+
+class Faq(models.Model):
+    header = models.CharField(
+        max_length=1024,
+    )
+
+    body = models.TextField()
```

### Comparing `aa-buybackprogram-1.9.1/buybackprogram/notes.py` & `aa_buybackprogram-2.0.0/buybackprogram/notes.py`

 * *Files identical despite different names*

### Comparing `aa-buybackprogram-1.9.1/buybackprogram/static/buybackprogram/css/billboards_dark.css` & `aa_buybackprogram-2.0.0/buybackprogram/static/buybackprogram/css/billboards_dark.css`

 * *Files identical despite different names*

### Comparing `aa-buybackprogram-1.9.1/buybackprogram/static/buybackprogram/css/billboards_light.css` & `aa_buybackprogram-2.0.0/buybackprogram/static/buybackprogram/css/billboards_light.css`

 * *Files identical despite different names*

### Comparing `aa-buybackprogram-1.9.1/buybackprogram/static/buybackprogram/css/style_dark.css` & `aa_buybackprogram-2.0.0/buybackprogram/static/buybackprogram/css/style_dark.css`

 * *Files identical despite different names*

### Comparing `aa-buybackprogram-1.9.1/buybackprogram/static/buybackprogram/css/style_light.css` & `aa_buybackprogram-2.0.0/buybackprogram/static/buybackprogram/css/style_light.css`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,18 @@
-.allianceauth-buyback-program-plugin .buy-value-True{
-	color: green !important;
+.allianceauth-buyback-program-plugin .no-border{
+  border:0;
+
+}
+
+.allianceauth-buyback-program-plugin tr.no-border td {
+  border: 0;
+}
+
+.allianceauth-buyback-program-plugin{
+	margin:10px;
 
 }
 
 .allianceauth-buyback-program-plugin .tooltip {
   position: relative;
   display: inline-block;
   border-bottom: 1px dotted black;
```

### Comparing `aa-buybackprogram-1.9.1/buybackprogram/static/buybackprogram/images/help.png` & `aa_buybackprogram-2.0.0/buybackprogram/static/buybackprogram/images/help.png`

 * *Files identical despite different names*

### Comparing `aa-buybackprogram-1.9.1/buybackprogram/static/buybackprogram/js/bootstrap-autocomplete.min.js` & `aa_buybackprogram-2.0.0/buybackprogram/static/buybackprogram/js/bootstrap-autocomplete.min.js`

 * *Files identical despite different names*

### Comparing `aa-buybackprogram-1.9.1/buybackprogram/swagger.json` & `aa_buybackprogram-2.0.0/buybackprogram/swagger.json`

 * *Files identical despite different names*

### Comparing `aa-buybackprogram-1.9.1/buybackprogram/templates/buybackprogram/base.html` & `aa_buybackprogram-2.0.0/buybackprogram/templates/buybackprogram/program_add.html`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,27 @@
-{% extends 'allianceauth/base.html' %}
+{% extends 'buybackprogram/page.html' %}
 {% load i18n %}
-{% load static %}
-{% block extra_css %}
-    {% if NIGHT_MODE %}
-        <link rel="stylesheet" type="text/css" href="{% static 'buybackprogram/css/style_dark.css' %}">
-        {% else %}
-        <link rel="stylesheet" type="text/css" href="{% static 'buybackprogram/css/style_light.css' %}">
-    {% endif %}
-{% endblock extra_css %}
+{% load humanize %}
+{% load bootstrap %}
+
+{% block body %}
+<div class="card">
+  <h5 class="card-header">{% trans "Create New Program" %}</h5>
+  <div class="card-body">
+      <form class="form" action="{{ url }}" method="POST">
+      {% csrf_token %}
+      {{ form|bootstrap }}
+      <button type="submit" class="btn btn-primary">{% trans "Create program" %}</button>
+    </form>
+  </div>
+</div>
+{% endblock %}
 
-{% block page_title %}{% translate "buybackprogram" %}{% endblock %}
+{% block extra_javascript %}
+{% endblock %}
+
+{% block extra_css %}
+{% include "buybackprogram/bundles/buybackprogram-css-light.html" %}
+{% endblock %}
 
-{% block content %}
-    <div class="allianceauth-buyback-program-plugin">
-        <div class="col-lg-12 container">
-            <h1 class="page-header text-center">{% translate "Buyback Program" %}</h1>
-            {% include 'buybackprogram/menu.html' %}
-            {% block details %}{% endblock %}
-        </div>
-    </div>
+{% block extra_script %}
 {% endblock %}
```

### Comparing `aa-buybackprogram-1.9.1/buybackprogram/templates/buybackprogram/faq.html` & `aa_buybackprogram-2.0.0/buybackprogram/templates/buybackprogram/location_add.html`

 * *Files 26% similar despite different names*

```diff
@@ -1,37 +1,48 @@
 {% extends 'buybackprogram/page.html' %}
 {% load i18n %}
 {% load humanize %}
 {% load bootstrap %}
 {% load static %}
 
 {% block body %}
-<div class="panel-heading">
-  <h2 class="panel-title">Frequently Asked Questions</h2>
-</div>
-<div class="panel-body" style="min-height: 100px;">
-  <div>
-    <h3>Where can I sell my items?</h3>
-    <p>Each program has a system and a structure mentioned on the program page. The manager for this program will most likely only accept items if the contract has been created at this exact location.</p>
-
-    <h3>How can I sell my items?</h3>
-    <ul>
-      <li>Have your items at the program location</li>
-      <li>Click <b>Use</b> on the program you wish to use</li>
-      <li>Copy paste your items from your inventory into the calculator</li>
-      <li>Follow the settings given by the calculator when creating the contract</li>
-    </ul>
-
-    <h3>How can I disable discord notifications for my contracts?</h3>
-    <p>You can disable notifications about your contracts via the <a href="user_settings_edit">My Settings</a> page</p>
+<div class="card">
+  <div class="card-body">
+      <form class="form" action="{% url 'buybackprogram:location_add' %}" method="POST">
+        {% csrf_token %}
+        {{ form|bootstrap }}
+        <button type="submit" class="btn btn-primary">{% trans "Add location" %}</button>
+      </form>
+      <table id="locations" style="margin: 20px auto;" class="table table-striped table-condensed">
+      <thead>
+        <th>{% trans "Solar System" %}</th>
+        <th style="text-align: center;">{% trans "Name" %}</th>
+        <th style="text-align: center;">{% trans "Structure ID" %}</th>
+      </thead>
+      <tbody>
+        {% for location in locations %}
+          {% if location.owner.user == request.user %}
+            <tr>
+              <td>{{location.eve_solar_system.name}}</td>
+              <td style="text-align: center;">{{location.name}}</td>
+              <td style="text-align: center;">{{location.structure_id}}</td>
+              <td><a class="btn btn-sm btn-danger" href="{% url 'buybackprogram:location_remove' location_pk=location.id %}">{% trans "Delete" %}</a></td>
+            </tr>
+          {% endif %}
+        {% endfor %}
+      </tbody>
+    </table>
   </div>
 </div>
 {% endblock %}
 
 {% block extra_javascript %}
+<script type="text/javascript" src="{% static 'buybackprogram/js/bootstrap-autocomplete.min.js' %}"></script>
+<script type="text/javascript" src="{% static 'buybackprogram/js/autocomplete.js' %}"></script>
 {% endblock %}
 
 {% block extra_css %}
+{% include "buybackprogram/bundles/buybackprogram-css-light.html" %}
 {% endblock %}
 
 {% block extra_script %}
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,16 +1,10 @@
 {% extends 'buybackprogram/page.html' %} {% load i18n %} {% load humanize %} {%
 load bootstrap %} {% load static %} {% block body %}
-********** FFrreeqquueennttllyy AAsskkeedd QQuueessttiioonnss **********
-******** WWhheerree ccaann II sseellll mmyy iitteemmss?? ********
-Each program has a system and a structure mentioned on the program page. The
-manager for this program will most likely only accept items if the contract has
-been created at this exact location.
-******** HHooww ccaann II sseellll mmyy iitteemmss?? ********
-    * Have your items at the program location
-    * Click UUssee on the program you wish to use
-    * Copy paste your items from your inventory into the calculator
-    * Follow the settings given by the calculator when creating the contract
-******** HHooww ccaann II ddiissaabbllee ddiissccoorrdd nnoottiiffiiccaattiioonnss ffoorr mmyy ccoonnttrraaccttss?? ********
-You can disable notifications about your contracts via the _M_y_ _S_e_t_t_i_n_g_s page
-{% endblock %} {% block extra_javascript %} {% endblock %} {% block extra_css
-%} {% endblock %} {% block extra_script %} {% endblock %}
+{% csrf_token %} {{ form|bootstrap }} {% trans "Add location" %}
+{                                        {                    {             _{_%_ _t_r_a_n_s
+{location.eve_solar_system.name}} {location.name}} {location.structure_id}} _"_D_e_l_e_t_e_"
+                                                                            _%_}
+{% endblock %} {% block extra_javascript %}
+{% endblock %} {% block extra_css %} {% include "buybackprogram/bundles/
+buybackprogram-css-light.html" %} {% endblock %} {% block extra_script %} {%
+endblock %}
```

### Comparing `aa-buybackprogram-1.9.1/buybackprogram/templates/buybackprogram/index.html` & `aa_buybackprogram-2.0.0/buybackprogram/templates/buybackprogram/index.html`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,26 @@
 {% extends 'buybackprogram/base.html' %}
 {% load i18n %}
 {% load humanize %}
+{% load static %}
 {% load program_settings %}
 
+{% block extra_css %}
+
+{% include "buybackprogram/bundles/buybackprogram-css-light.html" %}
+
+{% endblock extra_css %}
+
 {% block details %}
 
-<div class="table-responsive">
-    <table style="width: 100%; margin: auto;" class="table table-striped table-condensed">
+<div class="card">
+    <div class="card-header">
+        {% trans "Buyback Programs" %}
+    </div>
+    <table style="width: 100%; margin: auto;" class="table table-striped table-hover no-footer w-100">
         <thead>
             <tr>
                 <th>{% trans "Name" %}</th>
                 <th>{% trans "Location(s)" %}</th>
                 <th>{% trans "Tax" %}</th>
                 <th>{% trans "Manager" %}</th>
                 <th>{% trans "Settings" %}</th>
@@ -41,44 +51,41 @@
                     {% endfor %}
 
                 </td>
 
 
                 <td class="text-center">
                     <a class="btn btn-success btn-sm" href="{% url 'buybackprogram:program_calculate' program_pk=program.id %}">
-                        Use
+                        {% trans "Use" %}
                     </a>
 
                     {% if perms.buybackprogram.see_leaderboard %}
-                        <a class="btn btn-sm btn-info" href="{% url 'buybackprogram:program_leaderboard' program_pk=program.id %}">Leaderboard</a>
+                        <a class="btn btn-sm btn-info" href="{% url 'buybackprogram:program_leaderboard' program_pk=program.id %}">{% trans "Leaderboard" %}</a>
                     {% endif %}
 
                     {% if program.owner.user == request.user or perms.buybackprogram.see_performance %}
-                        <a class="btn btn-sm btn-info" href="{% url 'buybackprogram:program_performance' program_pk=program.id %}">Performance</a>
+                        <a class="btn btn-sm btn-info" href="{% url 'buybackprogram:program_performance' program_pk=program.id %}">{% trans "Performance" %}</a>
                     {% endif %}
 
-                    <a class="btn btn-sm btn-warning" href="{% url 'buybackprogram:program_special_taxes' program_pk=program.id %}">Special taxes</a>
+                    <a class="btn btn-sm btn-warning" href="{% url 'buybackprogram:program_special_taxes' program_pk=program.id %}">{% trans "Special taxes" %}</a>
 
                     {% if perms.buybackprogram.manage_programs and program.owner.user == request.user %}
-                        <a class="btn btn-sm btn-warning" href="{% url 'buybackprogram:program_edit' program_pk=program.id %}">Edit program</a>
+                        <a class="btn btn-sm btn-warning" href="{% url 'buybackprogram:program_edit' program_pk=program.id %}">{% trans "Edit program" %}</a>
                         <a class="btn btn-danger btn-sm" href="{% url 'buybackprogram:program_remove' program_pk=program.id %}">
-                        Delete
+                        {% trans "Delete" %}
                     </a>
                     {% endif %}
 
                 </td>
             </tr>
             {% endfor %}
         </tbody>
     </table>
-</div>
 
-{% endblock %}
 
-{% block extra_javascript %}
 {% endblock %}
 
-{% block extra_css %}
+{% block extra_javascript %}
 {% endblock %}
 
 {% block extra_script %}
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,18 +1,23 @@
 {% extends 'buybackprogram/base.html' %} {% load i18n %} {% load humanize %} {%
-load program_settings %} {% block details %}
+load static %} {% load program_settings %} {% block extra_css %} {% include
+"buybackprogram/bundles/buybackprogram-css-light.html" %} {% endblock extra_css
+%} {% block details %}
+{% trans "Buyback Programs" %}
 {{%% ttrraannss     {{%% ttrraannss ""LLooccaattiioonn((ss))"" %%}}         {{%% ttrraannss    {{%% ttrraannss ""MMaannaaggeerr"" %%}}     {{%% ttrraannss ""SSeettttiinnggss"" %%}}            {{%% ttrraannss ""AAccttiioonnss"" %%}}
 ""NNaammee"" %%}}                                      ""TTaaxx"" %%}}
-                                                                                                                                               _U_s_e_ {% if
+                                                                                                                                               _{_%_ _t_r_a_n_s_ _"_U_s_e_"_ _%_}_ {% if
                                                                                                                                                perms.buybackprogram.see_leaderboard
-                                                                                                                                               %} _L_e_a_d_e_r_b_o_a_r_d {% endif %} {% if
-             {% for location in                                                                                                                program.owner.user == request.user
-{            program.location.all %}           {           {                         {                                 {% for setting in       or
-{            {                                 {           {                         {                                 program|program_setting perms.buybackprogram.see_performance
-program.name {location.location_display_name}} program.tax program.owner.corporation program.owner.character.character %} {% endfor %}         %} _P_e_r_f_o_r_m_a_n_c_e {% endif %} _S_p_e_c_i_a_l
-}}           {% endfor %}                      }} %        }}                        }}                                                        _t_a_x_e_s {% if
+                                                                                                                                               %} _{_%_ _t_r_a_n_s_ _"_L_e_a_d_e_r_b_o_a_r_d_"_ _%_} {%
+                                                                                                                                               endif %} {% if program.owner.user ==
+             {% for location in                                                                                                                request.user or
+{            program.location.all %}           {           {                         {                                 {% for setting in       perms.buybackprogram.see_performance
+{            {                                 {           {                         {                                 program|program_setting %} _{_%_ _t_r_a_n_s_ _"_P_e_r_f_o_r_m_a_n_c_e_"_ _%_} {%
+program.name {location.location_display_name}} program.tax program.owner.corporation program.owner.character.character %} {% endfor %}         endif %} _{_%_ _t_r_a_n_s_ _"_S_p_e_c_i_a_l_ _t_a_x_e_s_"_ _%_}
+}}           {% endfor %}                      }} %        }}                        }}                                                        {% if
                                                                                                                                                perms.buybackprogram.manage_programs
                                                                                                                                                and program.owner.user ==
-                                                                                                                                               request.user %} _E_d_i_t_ _p_r_o_g_r_a_m _D_e_l_e_t_e_ 
-                                                                                                                                               {% endif %}
-{% endblock %} {% block extra_javascript %} {% endblock %} {% block extra_css
-%} {% endblock %} {% block extra_script %} {% endblock %}
+                                                                                                                                               request.user %} _{_%_ _t_r_a_n_s_ _"_E_d_i_t
+                                                                                                                                               _p_r_o_g_r_a_m_"_ _%_} _{_%_ _t_r_a_n_s_ _"_D_e_l_e_t_e_"_ _%_}_ {%
+                                                                                                                                               endif %}
+{% endblock %} {% block extra_javascript %} {% endblock %} {% block
+extra_script %} {% endblock %}
```

### Comparing `aa-buybackprogram-1.9.1/buybackprogram/templates/buybackprogram/leaderboards.html` & `aa_buybackprogram-2.0.0/buybackprogram/templates/buybackprogram/leaderboards.html`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 {% extends 'buybackprogram/page.html' %}
 {% load i18n %}
 {% load humanize %}
 {% load bootstrap %}
 {% load static %}
 
 {% block body %}
-<div class="panel-heading">
-  <h3 class="panel-title">Buyback Leaderboards</h3>
-</div>
-<div class="panel-body" style="min-height: 100px;">
+{% load i18n %}
+<div class="card">
+	<div class="card-header">
+    {% trans "Leaderboard for:" %} {{program.name}}
+  </div>
   <div class='row'>
     <div class='col-md-1'>
 	    <button class="btn btn-default" onclick="prior()"><span class="glyphicon glyphicon-chevron-left" aria-hidden="true"></span></button>
     </div>
     <div class='col-md-7 col-md-offset-3'>
-	    <h3>Month: <span id="month"></span></h3>
+	    <h3>{% trans "Month:" %} <span id="month"></span></h3>
     </div>
     <div class='col-md-1'>
 	    <button class="btn btn-default" onclick="next()"><span class="glyphicon glyphicon-chevron-right" aria-hidden="true"></span></button>
     </div>
   </div>
   <div class='row'>
     <div class='col-md-12'>
-	    <table id="leaderboard" class="table table-striped"><thead><tr><th>Name</th><th>Contract Total (ISK)</th><th>Donation Total (ISK)</th></tr></thead>
+	    <table id="leaderboard" class="table table-striped"><thead><tr><th>{% trans "Name" %}</th><th>{% trans "Contract Total (ISK)" %}</th><th>{% trans "Donation Total (ISK)" %}</th></tr></thead>
 		    <tbody id="data"></tbody>
 	    </table>
     </div>
   </div>
 </div>
 {% endblock %}
 
@@ -81,16 +82,12 @@
 {% endautoescape %}
 </script>
 {% endblock %}
 
 {% block extra_css %}
 <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/billboard.js/3.5.1/billboard.min.css" integrity="sha512-RMOXiaUbYERixbCxwbAyhJcq/KDpbXMZGLLUbexHB5JWdXsZONmsv2tLycOcTnAGCDZ9qPGG5pbd6bnL8YRhSw==" crossorigin="anonymous" referrerpolicy="no-referrer" />
 
-{% if NIGHT_MODE %}
-	<link rel="stylesheet" type="text/css" href="{% static 'buybackprogram/css/style_dark.css' %}">
-{% else %}
-	<link rel="stylesheet" type="text/css" href="{% static 'buybackprogram/css/style_light.css' %}">
-{% endif %}
+{% include "buybackprogram/bundles/buybackprogram-css-light.html" %}
 {% endblock %}
 
 {% block extra_script %}
 {% endblock %}
```

### Comparing `aa-buybackprogram-1.9.1/buybackprogram/templates/buybackprogram/program_add.html` & `aa_buybackprogram-2.0.0/buybackprogram/templates/buybackprogram/user_settings.html`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 {% extends 'buybackprogram/page.html' %}
 {% load i18n %}
 {% load humanize %}
 {% load bootstrap %}
+{% load static %}
 
 {% block body %}
-<div class="panel-heading">
-  <h3 class="panel-title">Create new program</h3>
-</div>
-<div class="panel-body" style="min-height: 100px;">
-  <form class="form" action="{{ url }}" method="POST">
-    {% csrf_token %}
-    {{ form|bootstrap }}
-    <button type="submit" class="btn btn-primary">Create program</button>
-  </form>
+<div class="card text-center">
+  <div class="card-header">
+    {% trans "Buyback user settings" %}
+  </div>
+  <div class="card-body">
+    <form class="form" action="{% url 'buybackprogram:user_settings_edit' %}" method="POST">
+      {% csrf_token %}
+      {{ form|bootstrap }}
+      <button type="submit" class="btn btn-primary">{% trans "Update Settings" %}</button>
+    </form>
+  </div>
 </div>
 {% endblock %}
 
 {% block extra_javascript %}
 {% endblock %}
 
 {% block extra_css %}
```

### Comparing `aa-buybackprogram-1.9.1/buybackprogram/templates/buybackprogram/program_edit_item.html` & `aa_buybackprogram-2.0.0/buybackprogram/templates/buybackprogram/program_edit.html`

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,33 @@
 {% extends 'buybackprogram/page.html' %}
 {% load i18n %}
 {% load humanize %}
 {% load bootstrap %}
 {% load static %}
 
 {% block body %}
-<div class="panel-heading">
-  <h3 class="panel-title">Program Special Taxes</h3>
-</div>
-<div class="panel-body" style="min-height: 100px;">
-  {% if perms.buybackprogram.manage_programs and program.owner.user == request.user %}
-  <div>
-    <form class="form" action="{% url 'buybackprogram:program_edit_item' program_pk=program.id %}" method="POST">
+<div class="card">
+  <div class="card-header">
+    Featured
+  </div>
+  <div class="card-body">
+    <form class="form" action="{% url 'buybackprogram:program_edit' program_pk=program.id %}" method="POST">
       {% csrf_token %}
       {{ form|bootstrap }}
-      <button type="submit" class="btn btn-primary">Add item</button>
+      <button type="submit" class="btn btn-primary">{% trans "Edit Program" %}</button>
     </form>
-    <a class="btn btn-default navbar-btn btn-warning" href="{% url 'buybackprogram:program_special_taxes' program_pk=program.id %}"><i class="fas fa-long-arrow-alt-left">Item taxes</i></a>
   </div>
-  {% endif %}
-
 </div>
 {% endblock %}
 
 {% block extra_javascript %}
-<script type="text/javascript" src="{% static 'buybackprogram/js/bootstrap-autocomplete.min.js' %}"></script>
-<script type="text/javascript" src="{% static 'buybackprogram/js/autocomplete.js' %}"></script>
+  <script type="text/javascript" src="{% static 'buybackprogram/js/bootstrap-autocomplete.min.js' %}"></script>
+  <script type="text/javascript" src="{% static 'buybackprogram/js/autocomplete.js' %}"></script>
+</div>
 {% endblock %}
 
 {% block extra_css %}
+{% include "buybackprogram/bundles/buybackprogram-css-light.html" %}
 {% endblock %}
 
 {% block extra_script %}
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,11 +1,8 @@
 {% extends 'buybackprogram/page.html' %} {% load i18n %} {% load humanize %} {%
 load bootstrap %} {% load static %} {% block body %}
-******** PPrrooggrraamm SSppeecciiaall TTaaxxeess ********
-{% if perms.buybackprogram.manage_programs and program.owner.user ==
-request.user %}
-{% csrf_token %} {{ form|bootstrap }} Add item
-_I_t_e_m_ _t_a_x_e_s
-{% endif %}
+Featured
+{% csrf_token %} {{ form|bootstrap }} {% trans "Edit Program" %}
 {% endblock %} {% block extra_javascript %}
-{% endblock %} {% block extra_css %} {% endblock %} {% block extra_script %} {%
+{% endblock %} {% block extra_css %} {% include "buybackprogram/bundles/
+buybackprogram-css-light.html" %} {% endblock %} {% block extra_script %} {%
 endblock %}
```

### Comparing `aa-buybackprogram-1.9.1/buybackprogram/templates/buybackprogram/program_edit_marketgroup.html` & `aa_buybackprogram-2.0.0/buybackprogram/templates/buybackprogram/program_edit_item.html`

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 {% extends 'buybackprogram/page.html' %}
 {% load i18n %}
 {% load humanize %}
 {% load bootstrap %}
 {% load static %}
 
 {% block body %}
-<div class="panel-heading">
-  <h3 class="panel-title">Program Special Taxes</h3>
-</div>
-<div class="panel-body" style="min-height: 100px;">
-  {% if perms.buybackprogram.manage_programs and program.owner.user == request.user %}
-  <div>
-    <form class="form" action="{% url 'buybackprogram:program_edit_marketgroup' program_pk=program.id %}" method="POST">
-      {% csrf_token %}
-      {{ form|bootstrap }}
-      <button type="submit" class="btn btn-primary">Add items</button>
-    </form>
-    <a class="btn btn-default navbar-btn btn-warning" href="{% url 'buybackprogram:program_special_taxes' program_pk=program.id %}"><i class="fas fa-long-arrow-alt-left">Item taxes</i></a>
+<div class="card">
+  <h5 class="card-header">{% trans "Add Special Item Tax to Program" %}</h5>
+  <div class="card-body">
+    {% if perms.buybackprogram.manage_programs and program.owner.user == request.user %}
+      <form class="form" action="{% url 'buybackprogram:program_edit_item' program_pk=program.id %}" method="POST">
+        {% csrf_token %}
+        {{ form|bootstrap }}
+        <button type="submit" class="btn btn-primary">{% trans "Add item" %}</button>
+      </form>
+    {% endif %}
+  </div>
+  <div class="card-footer text-muted">
+    <a class="btn btn-default navbar-btn btn-warning" href="{% url 'buybackprogram:program_special_taxes' program_pk=program.id %}"><i class="fas fa-long-arrow-alt-left"></i> {% trans "Back to item taxes" %}</a>
   </div>
-  {% endif %}
-
 </div>
 {% endblock %}
 
 {% block extra_javascript %}
 <script type="text/javascript" src="{% static 'buybackprogram/js/bootstrap-autocomplete.min.js' %}"></script>
 <script type="text/javascript" src="{% static 'buybackprogram/js/autocomplete.js' %}"></script>
 {% endblock %}
 
 {% block extra_css %}
+{% include "buybackprogram/bundles/buybackprogram-css-light.html" %}
 {% endblock %}
 
 {% block extra_script %}
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,11 +1,12 @@
 {% extends 'buybackprogram/page.html' %} {% load i18n %} {% load humanize %} {%
 load bootstrap %} {% load static %} {% block body %}
-******** PPrrooggrraamm SSppeecciiaall TTaaxxeess ********
+**** {{%% ttrraannss ""AAdddd SSppeecciiaall IItteemm TTaaxx ttoo PPrrooggrraamm"" %%}} ****
 {% if perms.buybackprogram.manage_programs and program.owner.user ==
 request.user %}
-{% csrf_token %} {{ form|bootstrap }} Add items
-_I_t_e_m_ _t_a_x_e_s
+{% csrf_token %} {{ form|bootstrap }} {% trans "Add item" %}
 {% endif %}
+_{_%_ _t_r_a_n_s_ _"_B_a_c_k_ _t_o_ _i_t_e_m_ _t_a_x_e_s_"_ _%_}
 {% endblock %} {% block extra_javascript %}
-{% endblock %} {% block extra_css %} {% endblock %} {% block extra_script %} {%
+{% endblock %} {% block extra_css %} {% include "buybackprogram/bundles/
+buybackprogram-css-light.html" %} {% endblock %} {% block extra_script %} {%
 endblock %}
```

### Comparing `aa-buybackprogram-1.9.1/buybackprogram/templates/buybackprogram/program_special_taxes.html` & `aa_buybackprogram-2.0.0/buybackprogram/templates/buybackprogram/program_special_taxes.html`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 {% extends 'buybackprogram/page.html' %}
 {% load i18n %}
 {% load humanize %}
 {% load bootstrap %}
 {% load static %}
 
 {% block body %}
-<div class="panel-heading">
-  <h3 class="panel-title">Program Special Taxes</h3>
-</div>
-<div class="panel-body" style="min-height: 100px;">
-  {% if perms.buybackprogram.manage_programs and program.owner.user == request.user %}
-    <a class="btn btn-sm btn-warning" href="{% url 'buybackprogram:program_edit_item' program_pk=program.id %}"><i class="fas fa-plus">Add item</i></a>
-    <a class="btn btn-sm btn-warning" href="{% url 'buybackprogram:program_edit_marketgroup' program_pk=program.id %}"><i class="fas fa-plus">Add market group</i></a>
-    <a class="btn btn-sm btn-danger" href="{% url 'buybackprogram:program_item_remove_all' program_pk=program.id %}"><i class="fas fa-trash">Deleta all items</i></a>
+<div class="card">
+  <div class="card-header">
+    {% trans "Program Special Taxes" %}
+  </div>
+  <div class="card-body">
+    {% if perms.buybackprogram.manage_programs and program.owner.user == request.user %}
+    <a class="btn btn-sm btn-warning" href="{% url 'buybackprogram:program_edit_item' program_pk=program.id %}"><i class="fas fa-plus"></i> {% trans "Add item" %}</a>
+    <a class="btn btn-sm btn-warning" href="{% url 'buybackprogram:program_edit_marketgroup' program_pk=program.id %}"><i class="fas fa-plus"></i> {% trans "Add market group" %}</a>
+    <a class="btn btn-sm btn-danger" href="{% url 'buybackprogram:program_item_remove_all' program_pk=program.id %}"><i class="fas fa-trash"></i> {% trans "Deleta all items" %}</a>
   {% endif %}
-  <div class="table-responsive" style="margin: 20px 0;">
-    <table id="program_items" style="margin: 20px auto;" class="table table-striped table-condensed">
+    <p style="margin-top:5px;">{% trans "This section shows all special item taxes applied to this program. Taxes may either be additional taxes or discounts." %}</p>
+    <table id="program_items" class="table table-striped table-hover no-footer w-100">
       <thead>
         <th>Name</th>
-        <th style="text-align: center;">Tax adjustment</th>
-        <th style="text-align: center;">Total tax</th>
-        <th style="text-align: center;">Is allowed</th>
+        <th style="text-align: center;">{% trans "Tax adjustment" %}</th>
+        <th style="text-align: center;">{% trans "Total tax" %}</th>
+        <th style="text-align: center;">{% trans "Is allowed" %}</th>
         {% if perms.buybackprogram.manage_programs and program.owner.user == request.user %}
-          <th style="text-align: center;">Actions</th>
+          <th style="text-align: center;">{% trans "Actions" %}</th>
         {% endif %}
       </thead>
       <tbody>
         {% for item in program_items %}
           <tr>
             <td>{{item.item_type.name}}</td>
             <td style="text-align: center;">{{item.item_tax}} %</td>
@@ -53,11 +54,12 @@
 
 {% block extra_javascript %}
 <script type="text/javascript" src="{% static 'buybackprogram/js/bootstrap-autocomplete.min.js' %}"></script>
 <script type="text/javascript" src="{% static 'buybackprogram/js/autocomplete.js' %}"></script>
 {% endblock %}
 
 {% block extra_css %}
+{% include "buybackprogram/bundles/buybackprogram-css-light.html" %}
 {% endblock %}
 
 {% block extra_script %}
 {% endblock %}
```

#### html2text {}

```diff
@@ -1,10 +1,19 @@
 {% extends 'buybackprogram/page.html' %} {% load i18n %} {% load humanize %} {%
 load bootstrap %} {% load static %} {% block body %}
-******** PPrrooggrraamm SSppeecciiaall TTaaxxeess ********
+{% trans "Program Special Taxes" %}
 {% if perms.buybackprogram.manage_programs and program.owner.user ==
-request.user %} _A_d_d_ _i_t_e_m _A_d_d_ _m_a_r_k_e_t_ _g_r_o_u_p _D_e_l_e_t_a_ _a_l_l_ _i_t_e_m_s {% endif %}
+request.user %}
+_{_%_ _t_r_a_n_s_ _"_A_d_d_ _i_t_e_m_"_ _%_}
+
+_{_%_ _t_r_a_n_s_ _"_A_d_d_ _m_a_r_k_e_t_ _g_r_o_u_p_"_ _%_}
+
+_{_%_ _t_r_a_n_s_ _"_D_e_l_e_t_a_ _a_l_l_ _i_t_e_m_s_"_ _%_}
+ {% endif %}
+{% trans "This section shows all special item taxes applied to this program.
+Taxes may either be additional taxes or discounts." %}
 {{item.item_type.name}} {{item.item_tax}} % {{item.item_tax|add:   _D_e_l_e_t_e
                                               program.tax }} %
 {% endblock %} {% block extra_javascript %}
-{% endblock %} {% block extra_css %} {% endblock %} {% block extra_script %} {%
+{% endblock %} {% block extra_css %} {% include "buybackprogram/bundles/
+buybackprogram-css-light.html" %} {% endblock %} {% block extra_script %} {%
 endblock %}
```

### Comparing `aa-buybackprogram-1.9.1/buybackprogram/tests/test_helpers.py` & `aa_buybackprogram-2.0.0/buybackprogram/tests/test_helpers.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,21 +8,24 @@
 
 class TestHelpers(TestCase):
     def test_should_create_tracking_when_first(self):
         # given
         load_eveuniverse()
         user = UserIssuerFactory()
         program = ProgramFactory()
+        additional_notes = "Test note"
         contract_net_prices = {
             "total_all_items_raw": 1,
             "total_all_items": 1,
             "total_tax_amount": 1,
             "total_donation_amount": 1,
             "hauling_cost": 0,
             "total_hauling_cost": 0,
             "contract_net_total": 1,
         }
         # when
-        tracking = get_tracking_number(user, program, None, [], contract_net_prices)
+        tracking = get_tracking_number(
+            user, program, None, [], contract_net_prices, additional_notes
+        )
         # then
         self.assertEqual(tracking.program, program)
         self.assertEqual(tracking.issuer_user, user)
```

### Comparing `aa-buybackprogram-1.9.1/buybackprogram/tests/test_models.py` & `aa_buybackprogram-2.0.0/buybackprogram/tests/test_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from unittest.mock import patch
 
+from django.db import IntegrityError
 from django.test import TestCase
 from eveuniverse.models import EveType
 
 from app_utils.esi import EsiStatus
 from app_utils.esi_testing import EsiClientStub, EsiEndpoint
 from app_utils.testing import NoSocketsTestCase
 
@@ -280,14 +281,21 @@
 class TestContracts(TestCase):
     def test_should_have_str_method(self):
         # given
         obj = ContractFactory()
         # when/then
         self.assertIsInstance(str(obj), str)
 
+    def test_contract_id_should_be_unique(self):
+        # given
+        contract = ContractFactory()
+        # when/then
+        with self.assertRaises(IntegrityError):
+            ContractFactory(contract_id=contract.contract_id)
+
 
 class TestContractItems(TestCase):
     @classmethod
     def setUpClass(cls) -> None:
         super().setUpClass()
         load_eveuniverse()
```

### Comparing `aa-buybackprogram-1.9.1/buybackprogram/tests/testdata/create_eveuniverse.py` & `aa_buybackprogram-2.0.0/buybackprogram/tests/testdata/create_eveuniverse.py`

 * *Files identical despite different names*

### Comparing `aa-buybackprogram-1.9.1/buybackprogram/tests/testdata/factories.py` & `aa_buybackprogram-2.0.0/buybackprogram/tests/testdata/factories.py`

 * *Files 10% similar despite different names*

```diff
@@ -182,38 +182,38 @@
         return obj
 
 
 class ContractFactory(factory.django.DjangoModelFactory):
     class Meta:
         model = Contract
 
-    assignee_id = factory.fuzzy.FuzzyInteger(90_000, 99_000)
+    assignee_id = factory.Sequence(lambda n: 90_000 + n)
     availability = "public"
-    contract_id = factory.fuzzy.FuzzyInteger(1_000_000_000, 2_000_000_000)
+    contract_id = factory.Sequence(lambda n: 1_000_000_000 + n)
     date_issued = factory.fuzzy.FuzzyDateTime(now() - dt.timedelta(days=3))
     for_corporation = False
-    issuer_corporation_id = factory.fuzzy.FuzzyInteger(90_000, 99_000)
-    issuer_id = factory.fuzzy.FuzzyInteger(90_000, 99_000)
+    issuer_corporation_id = factory.Sequence(lambda n: 99_000 + n)
+    issuer_id = factory.Sequence(lambda n: 95_000 + n)
     price = factory.fuzzy.FuzzyInteger(90_000, 99_000)
     status = "outstanding"
     title = factory.Faker("sentence")
     volume = factory.fuzzy.FuzzyInteger(10, 320)
 
 
 class EsiContractFactory(factory.DictFactory):
     """Contract dictionary returned from ESI endpoint."""
 
     # acceptor_id
-    assignee_id = factory.fuzzy.FuzzyInteger(90_000, 99_000)
+    assignee_id = factory.Sequence(lambda n: 90_000 + n)
     availability = "public"
-    contract_id = factory.fuzzy.FuzzyInteger(1_000_000_000, 2_000_000_000)
+    contract_id = factory.Sequence(lambda n: 1_000_000_000 + n)
     date_issued = factory.fuzzy.FuzzyDateTime(now() - dt.timedelta(days=3))
     for_corporation = False
-    issuer_corporation_id = factory.fuzzy.FuzzyInteger(90_000, 99_000)
-    issuer_id = factory.fuzzy.FuzzyInteger(90_000, 99_000)
+    issuer_corporation_id = factory.Sequence(lambda n: 99_000 + n)
+    issuer_id = factory.Sequence(lambda n: 95_000 + n)
     price = factory.fuzzy.FuzzyInteger(90_000, 99_000)
     status = "outstanding"
     start_location_id = 60003760
     title = factory.Faker("sentence")
     type = "item_exchange"
     volume = factory.fuzzy.FuzzyInteger(10, 320)
 
@@ -230,15 +230,15 @@
 
 class EsiContractItemFactory(factory.DictFactory):
     """Contract item dictionary returned from ESI endpoint."""
 
     is_included = True
     is_singleton = False
     quantity = factory.fuzzy.FuzzyInteger(1, 999)
-    record_id = factory.Sequence(lambda n: n)
+    record_id = factory.Sequence(lambda n: 1 + n)
 
     @factory.lazy_attribute
     def type_id(self):
         id = random_eve_type_id()
         if not id:
             raise RuntimeError("No EveType found for EsiContractItemFactory.")
         return id
```

### Comparing `aa-buybackprogram-1.9.1/buybackprogram/urls.py` & `aa_buybackprogram-2.0.0/buybackprogram/urls.py`

 * *Files identical despite different names*

### Comparing `aa-buybackprogram-1.9.1/buybackprogram/utils.py` & `aa_buybackprogram-2.0.0/buybackprogram/utils.py`

 * *Files identical despite different names*

### Comparing `aa-buybackprogram-1.9.1/buybackprogram/views/calculate.py` & `aa_buybackprogram-2.0.0/buybackprogram/views/calculate.py`

 * *Files 19% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 
 @login_required
 @permission_required("buybackprogram.basic_access")
 def program_calculate(request, program_pk):
     program = Program.objects.filter(pk=program_pk).first()
 
     buyback_data = []
+    additional_notes = False
 
     form_donation = False
 
     if program is None:
         return redirect("buybackprogram:index")
 
     if request.method != "POST":
@@ -38,14 +39,17 @@
 
     else:
         form = CalculatorForm(request.POST)
 
         if form.is_valid():
             form_items = form.cleaned_data["items"]
             form_donation = form.cleaned_data["donation"]
+            additional_notes = form.cleaned_data[
+                "additional_notes"
+            ]  # Capture additional notes
 
             # If we have an ingame copy paste
             if "\t" in form_items:
                 # Split items by rows
                 for item in form_items.split("\n"):
                     item_accepted = True
                     notes = []
@@ -102,21 +106,15 @@
                             notes.append(note)
 
                     # Icons view
                     elif len(parts) == 2:
                         # Get item quantity.
                         if not parts[1] == "\r":
                             # Get quantities and format the different localization imputs
-                            quantity = int(
-                                parts[1]
-                                .replace(" ", "")
-                                .replace(".", "")
-                                .replace(",", "")
-                                .replace("\xa0", "")
-                            )
+                            quantity = int("".join(filter(str.isdigit, parts[1])))
 
                         elif program.allow_unpacked_items:
                             quantity = 1
 
                         else:
                             quantity = 1
                             item_accepted = False
@@ -131,21 +129,15 @@
                             notes.append(note)
 
                     # Detail view
                     else:
                         # Get item quantity.
                         if parts[1]:
                             # Get quantities and format the different localization imputs
-                            quantity = int(
-                                parts[1]
-                                .replace(" ", "")
-                                .replace(".", "")
-                                .replace(",", "")
-                                .replace("\xa0", "")
-                            )
+                            quantity = int("".join(filter(str.isdigit, parts[1])))
 
                         elif program.allow_unpacked_items:
                             quantity = 1
 
                         else:
                             quantity = 1
                             item_accepted = False
@@ -218,15 +210,20 @@
     logger.debug(
         "Calculated contract net total is %s"
         % contract_price_data["contract_net_total"]
     )
 
     # Get item values after other expenses and the total value for the contract
     tracking = get_tracking_number(
-        request.user, program, form_donation, buyback_data, contract_price_data
+        request.user,
+        program,
+        form_donation,
+        buyback_data,
+        contract_price_data,
+        additional_notes,
     )
 
     context = {
         "program": program,
         "form": form,
         "donation": form_donation,
         "buyback_data": buyback_data,
```

### Comparing `aa-buybackprogram-1.9.1/buybackprogram/views/common.py` & `aa_buybackprogram-2.0.0/buybackprogram/views/common.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from django.shortcuts import redirect, render
 from django.utils.html import format_html
 from eveuniverse.models import EveMarketGroup, EveSolarSystem, EveType
 
 from allianceauth.services.hooks import get_extension_logger
 
 from buybackprogram.forms import UserSettingsForm
-from buybackprogram.models import Program, UserSettings
+from buybackprogram.models import Faq, Program, UserSettings
 from buybackprogram.utils import messages_plus
 
 logger = get_extension_logger(__name__)
 
 
 @login_required
 @permission_required("buybackprogram.basic_access")
@@ -55,15 +55,21 @@
 
     return render(request, "buybackprogram/index.html", context)
 
 
 @login_required
 @permission_required("buybackprogram.basic_access")
 def faq(request):
-    return render(request, "buybackprogram/faq.html")
+    faq = Faq.objects.all()
+
+    context = {
+        "faqs": faq,
+    }
+
+    return render(request, "buybackprogram/faq.html", context)
 
 
 @login_required
 @permission_required("buybackprogram.manage_programs")
 def item_autocomplete(request):
     items = EveType.objects.filter(published=True).exclude(
         eve_group__eve_category__id=9
```

### Comparing `aa-buybackprogram-1.9.1/buybackprogram/views/programs.py` & `aa_buybackprogram-2.0.0/buybackprogram/views/programs.py`

 * *Files identical despite different names*

### Comparing `aa-buybackprogram-1.9.1/buybackprogram/views/special_taxes.py` & `aa_buybackprogram-2.0.0/buybackprogram/views/special_taxes.py`

 * *Files identical despite different names*

### Comparing `aa-buybackprogram-1.9.1/buybackprogram/views/stats.py` & `aa_buybackprogram-2.0.0/buybackprogram/views/stats.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,46 +1,47 @@
 import json
+import os
 from datetime import datetime
 
+from django.conf import settings
 from django.contrib.auth.decorators import login_required, permission_required
 from django.db.models import Q
 from django.shortcuts import render
 from django.utils import timezone
 from eveuniverse.models import EveEntity
 
 from allianceauth.authentication.models import CharacterOwnership
 from allianceauth.services.hooks import get_extension_logger
 
+from buybackprogram.app_settings import BUYBACKPROGRAM_TRACK_PREFILL_CONTRACTS
 from buybackprogram.notes import (
     note_missing_from_contract,
     note_missing_from_tracking,
     note_quantity_missing_from_contract,
     note_quantity_missing_from_tracking,
 )
 
 from ..models import (
     Contract,
     ContractItem,
     ContractNotification,
+    Program,
     Tracking,
     TrackingItem,
 )
 
-from buybackprogram.app_settings import (
-    BUYBACKPROGRAM_TRACK_PREFILL_CONTRACTS,
-)
-
 logger = get_extension_logger(__name__)
 
 
 @login_required
 @permission_required("buybackprogram.basic_access")
 def my_stats(request):
     # List for valid contracts to be displayed
     valid_contracts = []
+    contract_notes = []
 
     # Tracker values
     values = {
         "outstanding": 0,
         "finished": 0,
         "outstanding_count": 0,
         "finished_count": 0,
@@ -82,27 +83,31 @@
         # Get the name for the assignee
         tracking.contract.assignee_name = EveEntity.objects.resolve_name(
             tracking.contract.assignee_id
         )
 
         # Add contract to the valid contract list
         valid_contracts.append(tracking)
+        contract_notes.append(tracking.contract.notes)
 
     context = {
         "contracts": valid_contracts,
+        "contract_notes": contract_notes,
         "values": values,
         "mine": True,
     }
 
     return render(request, "buybackprogram/stats.html", context)
 
 
 @login_required
 @permission_required("buybackprogram.basic_access")
 def leaderboard(request, program_pk):
+    program = Program.objects.get(pk=program_pk)
+
     # Tracker values
     monthstats = {
         "users": {},  # monthly stats per user
         "userinfo": {},  # profile information per user
         "months": None,  # all months
     }
     # Get all tracking objects that have a linked contract to them for the user
@@ -135,255 +140,30 @@
                     "name": EveEntity.objects.resolve_name(user),
                     "pic": f"https://images.evetech.net/characters/{user}/portrait?size=32",
                 }
 
     monthstats["months"] = sorted(list(monthstats["users"].keys()))
     context = {
         "stats": json.dumps(monthstats),
+        "program": program,
     }
 
     return render(request, "buybackprogram/leaderboards.html", context)
 
 
 @login_required
 @permission_required("buybackprogram.manage_programs")
 def program_performance(request, program_pk):
-    firstbench = datetime.now()
-    lastbench = datetime.now()
-    # Tracker values
-    monthstats = {
-        "status": {},
-        "overall": {"all": {}},
-        "items": {},
-        "categories": {},
-        "donations": {"all": {}},
-    }
-    allmonths = set()
-
-    # Category to Item mapping
-    category2items = {}
-
-    # Export data
-    dumpdata = [
-        [
-            "Contract ID",
-            "Date Issued",
-            "Date Finished",
-            "User ID",
-            "Total ISK",
-            "Object Cateogry",
-            "Object ID",
-            "Object Name",
-            "Object Quant",
-            "Object ISK",
-        ]
-    ]
-
-    # Get all tracking objects that have a linked contract to them for the user
-    tracking_numbers = (
-        Tracking.objects.filter(program_id=program_pk)
-        .filter(contract__isnull=False)
-        .prefetch_related("contract")
-    )
-
-    logger.debug(
-        "Performance bench: %.2f" % (datetime.now() - lastbench).total_seconds()
-    )
-    lastbench = datetime.now()
-    # Loop all tracking objects
-    for tracking in tracking_numbers:
-        month = datetime.strftime(tracking.contract.date_issued, "%Y-%m") + "-15"
-        allmonths.add(month)
-
-        if month not in monthstats["status"]:
-            monthstats["status"][
-                month
-            ] = {}  # status of all contracts issued during a given month
-
-        # Gather stats on all contracts' statuses
-        if tracking.contract.status not in monthstats["status"][month]:
-            monthstats["status"][month][tracking.contract.status] = 0
-        monthstats["status"][month][tracking.contract.status] += 1
-
-        # For finished contracts, gather more data
-        if tracking.contract.status == "finished":
-            # "overall": {"all": {"isk": {}, "q": {}, }
-            if month not in monthstats["overall"]["all"]:
-                monthstats["overall"]["all"][month] = [0, 0]  # isk, q
-                monthstats["donations"]["all"][month] = [0, 0]  # isk, q
-
-            monthstats["overall"]["all"][month][0] += tracking.contract.price
-            monthstats["overall"]["all"][month][1] += 1
-
-            monthstats["donations"]["all"][month][0] += tracking.donation
-            if tracking.donation > 0:
-                monthstats["donations"]["all"][month][1] += 1
-
-            logger.debug(
-                "Performance loop bench: %.2f"
-                % (datetime.now() - lastbench).total_seconds()
-            )
-            lastbench = datetime.now()
-            # Collect ISK data per items
-            tracking_items = TrackingItem.objects.filter(tracking=tracking)
-            for item in tracking_items:
-                if item.eve_type.name not in monthstats["items"]:
-                    monthstats["items"][item.eve_type.name] = {}
-                if month not in monthstats["items"][item.eve_type.name]:
-                    monthstats["items"][item.eve_type.name][month] = [0, 0]
-                monthstats["items"][item.eve_type.name][month][0] += item.buy_value
-                monthstats["items"][item.eve_type.name][month][1] += item.quantity
-                # cache[tracking.contract.issuer_id] = EveEntity.objects.resolve_name(tracking.contract.issuer_id)
-
-                # Collect item category data
-                catid = item.eve_type.eve_group.name
-                if catid not in category2items:
-                    category2items[catid] = set()
-                category2items[catid].add(item.eve_type.name)
-
-                if catid not in monthstats["categories"]:
-                    monthstats["categories"][catid] = {}
-                if month not in monthstats["categories"][catid]:
-                    monthstats["categories"][catid][month] = [0, 0]
-                monthstats["categories"][catid][month][0] += item.buy_value
-                monthstats["categories"][catid][month][1] += item.quantity
-
-                # Collect data for export
-                dumpdata.append(
-                    [
-                        tracking.id,
-                        datetime.strftime(
-                            tracking.contract.date_issued, "%Y-%m-%d %H:%M:%S"
-                        ),
-                        datetime.strftime(
-                            tracking.contract.date_completed, "%Y-%m-%d %H:%M:%S"
-                        ),
-                        tracking.contract.issuer_id,
-                        tracking.contract.price,
-                        item.eve_type.eve_group.name,
-                        item.eve_type.id,
-                        item.eve_type.name,
-                        item.quantity,
-                        item.buy_value,
-                    ]
-                )
-
-    logger.debug(
-        "Performance exit loop bench: %.2f"
-        % (datetime.now() - lastbench).total_seconds()
-    )
-    lastbench = datetime.now()
-    # Reformat data so that it is easier to use billboard.js
-    allmonths = sorted(list(allmonths))
-
-    scaling = {}
-    hscaling = {}
-    for strata in ("overall", "items", "categories", "donations"):
-        scaling[strata] = []
-        for yi in monthstats[strata].keys():
-            scaling[strata] += [
-                monthstats[strata][yi][x][0] for x in monthstats[strata][yi].keys()
-            ]
-        if len(scaling[strata]) == 0:
-            scaling[strata] = 1
-        else:
-            scaling[strata] = sum(scaling[strata]) / len(scaling[strata])
-        for s, h in ((1e9, "Billions"), (1e6, "Millions")):
-            if scaling[strata] > s:
-                scaling[strata] = s
-                hscaling[strata] = h
-                break
-        if scaling[strata] < 1e6:
-            scaling[strata] = 1
-            hscaling[strata] = ""
-
-    # Always set donations to be the same scale as overall since they are plotted together.
-    scaling["donations"] = scaling["overall"]
-    hscaling["donations"] = hscaling["overall"]
-
-    for strata in ("overall", "items", "categories", "donations"):
-        for yi in monthstats[strata].keys():
-            y = [[yi], [yi]]
-            # Overall ISK
-            if strata == "overall":
-                y = [["Bought"], ["Contract count"]]
-            # Donation ISK
-            if strata == "donations":
-                y = [["Donations"], ["Donation count"]]
-
-            for m in allmonths:
-                if m not in (monthstats[strata][yi]):
-                    monthstats[strata][yi][m] = [0, 0]
-                y[0].append(round(monthstats[strata][yi][m][0] / scaling[strata], 3))
-                y[1].append(monthstats[strata][yi][m][1])
-            monthstats[strata][yi] = y
-    monthstats["x"] = ["x"] + allmonths
-
-    for cat in category2items:
-        category2items[cat] = list(category2items[cat])
-
-    # Break down of categories by last three months:
-    lastthree = {}
-    for yi in monthstats["categories"].keys():
-        calc = monthstats["categories"][yi][0].copy()
-        calc.pop(0)
-        lastthree[yi] = sum(calc[-3:])
-
-    if len(lastthree.keys()) > 10:
-        th = lastthree[sorted(lastthree.keys(), key=lambda x: -lastthree[x])[10]]
-        lastthree["Other"] = 0
-        for k in list(lastthree.keys()):
-            if k != "Other" and lastthree[k] <= th:
-                lastthree["Other"] += lastthree[k]
-                del lastthree[k]
-
-        monthstats["categories"]["Other"] = None
-        for k in list(monthstats["categories"].keys()):
-            if k not in lastthree:
-                if monthstats["categories"]["Other"] is None:
-                    monthstats["categories"]["Other"] = monthstats["categories"][k]
-                else:
-                    monthstats["categories"]["Other"][0][1:] = [
-                        sum(x)
-                        for x in zip(
-                            monthstats["categories"]["Other"][0][1:],
-                            monthstats["categories"][k][0][1:],
-                        )
-                    ]
-                    monthstats["categories"]["Other"][1][1:] = [
-                        sum(x)
-                        for x in zip(
-                            monthstats["categories"]["Other"][1][1:],
-                            monthstats["categories"][k][1][1:],
-                        )
-                    ]
-                del monthstats["categories"][k]
-        monthstats["categories"]["Other"][0][0] = "Other"
-        monthstats["categories"]["Other"][1][0] = "Other"
-
-    lastthree = list(lastthree.items())
-
-    # Sanitize CSV data
-    for i in range(len(dumpdata)):
-        for j in range(len(dumpdata[i])):
-            dumpdata[i][j] = str(dumpdata[i][j]).replace(",", " ")
-
-    context = {
-        "stats": json.dumps(monthstats),
-        "lastthree": json.dumps(lastthree),
-        "categories": json.dumps(category2items),
-        "export": json.dumps(dumpdata),
-        "hscaling": json.dumps(hscaling),
-    }
-    logger.debug(
-        "Performance finished: %.2f" % (datetime.now() - lastbench).total_seconds()
-    )
-    logger.debug(
-        "Performance total: %.2f" % (datetime.now() - firstbench).total_seconds()
-    )
+    static_path = os.path.join(settings.STATIC_ROOT, "buybackprogram/performance_data")
+    filename = f"program_performance_{program_pk}.json"
+    file_path = os.path.join(static_path, filename)
+
+    if os.path.exists(file_path):
+        with open(file_path, "r") as file:
+            context = json.load(file)
 
     return render(request, "buybackprogram/performance.html", context)
 
 
 @login_required
 @permission_required("buybackprogram.manage_programs")
 def program_stats(request):
```

