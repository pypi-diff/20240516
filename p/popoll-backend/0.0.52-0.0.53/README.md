# Comparing `tmp/popoll_backend-0.0.52.tar.gz` & `tmp/popoll_backend-0.0.53.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "popoll_backend-0.0.52.tar", last modified: Wed May 15 21:15:04 2024, max compression
+gzip compressed data, was "popoll_backend-0.0.53.tar", last modified: Thu May 16 21:56:04 2024, max compression
```

## Comparing `popoll_backend-0.0.52.tar` & `popoll_backend-0.0.53.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 21:15:04.984267 popoll_backend-0.0.52/
--rw-r--r--   0 root         (0) root         (0)      618 2024-05-15 21:15:04.984267 popoll_backend-0.0.52/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)       16 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 21:15:04.970267 popoll_backend-0.0.52/popoll_backend/
--rw-rw-rw-   0 root         (0) root         (0)     6871 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/popoll_backend/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 21:15:04.971267 popoll_backend-0.0.52/popoll_backend/model/
--rw-rw-rw-   0 root         (0) root         (0)      257 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/popoll_backend/model/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 21:15:04.973267 popoll_backend-0.0.52/popoll_backend/model/db/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/popoll_backend/model/db/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      683 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/popoll_backend/model/db/answer.py
--rw-rw-rw-   0 root         (0) root         (0)      664 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/popoll_backend/model/db/date.py
--rw-rw-rw-   0 root         (0) root         (0)      394 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/popoll_backend/model/db/instrument.py
--rw-rw-rw-   0 root         (0) root         (0)      371 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/popoll_backend/model/db/option.py
--rw-rw-rw-   0 root         (0) root         (0)      549 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/popoll_backend/model/db/session.py
--rw-rw-rw-   0 root         (0) root         (0)      405 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/popoll_backend/model/db/user.py
--rw-rw-rw-   0 root         (0) root         (0)      666 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/popoll_backend/model/db/user_instruments.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 21:15:04.975267 popoll_backend-0.0.52/popoll_backend/model/payload/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/popoll_backend/model/payload/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2408 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/popoll_backend/model/payload/date_payload.py
--rw-rw-rw-   0 root         (0) root         (0)      286 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/popoll_backend/model/payload/dates_payload.py
--rw-rw-rw-   0 root         (0) root         (0)      730 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/popoll_backend/model/payload/history.py
--rw-rw-rw-   0 root         (0) root         (0)      141 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/popoll_backend/model/payload/id_payload.py
--rw-rw-rw-   0 root         (0) root         (0)      276 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/popoll_backend/model/payload/instruments_payload.py
--rw-rw-rw-   0 root         (0) root         (0)      711 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/popoll_backend/model/payload/user.py
--rw-rw-rw-   0 root         (0) root         (0)      957 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/popoll_backend/model/payload/user_payload.py
--rw-rw-rw-   0 root         (0) root         (0)      229 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/popoll_backend/model/payload/users_payload.py
--rw-rw-rw-   0 root         (0) root         (0)      250 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/popoll_backend/model/payload/users_payload_details.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 21:15:04.979267 popoll_backend-0.0.52/popoll_backend/query/
--rw-rw-rw-   0 root         (0) root         (0)     2121 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/popoll_backend/query/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1029 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/popoll_backend/query/create_answer.py
--rw-rw-rw-   0 root         (0) root         (0)      861 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/popoll_backend/query/create_date.py
--rw-rw-rw-   0 root         (0) root         (0)      636 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/popoll_backend/query/create_instrument.py
--rw-rw-rw-   0 root         (0) root         (0)     1624 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/popoll_backend/query/create_poll.py
--rw-rw-rw-   0 root         (0) root         (0)      789 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/popoll_backend/query/create_session.py
--rw-rw-rw-   0 root         (0) root         (0)     1349 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/popoll_backend/query/create_user.py
--rw-rw-rw-   0 root         (0) root         (0)      527 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/popoll_backend/query/delete_answer.py
--rw-rw-rw-   0 root         (0) root         (0)      523 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/popoll_backend/query/delete_date.py
--rw-rw-rw-   0 root         (0) root         (0)      523 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/popoll_backend/query/delete_user.py
--rw-rw-rw-   0 root         (0) root         (0)      535 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/popoll_backend/query/get_answer.py
--rw-rw-rw-   0 root         (0) root         (0)     1796 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/popoll_backend/query/get_date.py
--rw-rw-rw-   0 root         (0) root         (0)      630 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/popoll_backend/query/get_dates.py
--rw-rw-rw-   0 root         (0) root         (0)      686 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/popoll_backend/query/get_instruments.py
--rw-rw-rw-   0 root         (0) root         (0)      486 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/popoll_backend/query/get_poll.py
--rw-rw-rw-   0 root         (0) root         (0)      860 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/popoll_backend/query/get_search_answer.py
--rw-rw-rw-   0 root         (0) root         (0)      780 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/popoll_backend/query/get_session.py
--rw-rw-rw-   0 root         (0) root         (0)     1968 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/popoll_backend/query/get_user.py
--rw-rw-rw-   0 root         (0) root         (0)     1563 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/popoll_backend/query/get_users.py
--rw-rw-rw-   0 root         (0) root         (0)      732 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/popoll_backend/query/update_answer.py
--rw-rw-rw-   0 root         (0) root         (0)      858 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/popoll_backend/query/update_date.py
--rw-rw-rw-   0 root         (0) root         (0)      609 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/popoll_backend/query/update_poll.py
--rw-rw-rw-   0 root         (0) root         (0)     1415 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/popoll_backend/query/update_user.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 21:15:04.984267 popoll_backend-0.0.52/popoll_backend.egg-info/
--rw-r--r--   0 root         (0) root         (0)      618 2024-05-15 21:15:04.000000 popoll_backend-0.0.52/popoll_backend.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2538 2024-05-15 21:15:04.000000 popoll_backend-0.0.52/popoll_backend.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-15 21:15:04.000000 popoll_backend-0.0.52/popoll_backend.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       51 2024-05-15 21:15:04.000000 popoll_backend-0.0.52/popoll_backend.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2024-05-15 21:15:04.000000 popoll_backend-0.0.52/popoll_backend.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      845 2024-05-15 21:14:59.000000 popoll_backend-0.0.52/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-15 21:15:04.984267 popoll_backend-0.0.52/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 21:15:04.983267 popoll_backend-0.0.52/tests/
--rw-rw-rw-   0 root         (0) root         (0)      536 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/tests/test_01_db_creation.py
--rw-rw-rw-   0 root         (0) root         (0)     1256 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/tests/test_02_simple_adds.py
--rw-rw-rw-   0 root         (0) root         (0)     1232 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/tests/test_03_no_duplicates.py
--rw-rw-rw-   0 root         (0) root         (0)     1653 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/tests/test_04_update_user_entry.py
--rw-rw-rw-   0 root         (0) root         (0)     1836 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/tests/test_05_update_date_entry.py
--rw-rw-rw-   0 root         (0) root         (0)     1186 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/tests/test_06_update_answer_entry.py
--rw-rw-rw-   0 root         (0) root         (0)      748 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/tests/test_07_delete_user_entry.py
--rw-rw-rw-   0 root         (0) root         (0)     1784 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/tests/test_08_delete_date_entry.py
--rw-rw-rw-   0 root         (0) root         (0)     2283 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/tests/test_09_delete_user_date_entries.py
--rw-rw-rw-   0 root         (0) root         (0)     1333 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/tests/test_10_get_users.py
--rw-rw-rw-   0 root         (0) root         (0)      628 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/tests/test_11_get_users_sort_name.py
--rw-rw-rw-   0 root         (0) root         (0)     1203 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/tests/test_12_get_dates_sort_dateTime.py
--rw-rw-rw-   0 root         (0) root         (0)     2887 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/tests/test_13_history.py
--rw-rw-rw-   0 root         (0) root         (0)     2122 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/tests/test_14_get_answers_user.py
--rw-rw-rw-   0 root         (0) root         (0)     2388 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/tests/test_15_multi_instruments.py
--rw-rw-rw-   0 root         (0) root         (0)     5130 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/tests/test_16_get_date.py
--rw-rw-rw-   0 root         (0) root         (0)      478 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/tests/test_17_get_instruments.py
--rw-rw-rw-   0 root         (0) root         (0)      444 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/tests/test_18_post_instrument.py
--rw-rw-rw-   0 root         (0) root         (0)      435 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/tests/test_19_delete_database.py
--rw-rw-rw-   0 root         (0) root         (0)      537 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/tests/test_20_add_answer_no_dupe.py
--rw-rw-rw-   0 root         (0) root         (0)      833 2024-05-15 21:14:45.000000 popoll_backend-0.0.52/tests/test_21_get_dates.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 21:56:04.755149 popoll_backend-0.0.53/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-16 21:56:04.755149 popoll_backend-0.0.53/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)       16 2024-05-16 21:55:44.000000 popoll_backend-0.0.53/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 21:56:04.740149 popoll_backend-0.0.53/popoll_backend/
+-rw-rw-rw-   0 root         (0) root         (0)     6971 2024-05-16 21:55:44.000000 popoll_backend-0.0.53/popoll_backend/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 21:56:04.741149 popoll_backend-0.0.53/popoll_backend/model/
+-rw-rw-rw-   0 root         (0) root         (0)      257 2024-05-16 21:55:44.000000 popoll_backend-0.0.53/popoll_backend/model/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 21:56:04.743149 popoll_backend-0.0.53/popoll_backend/model/db/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-16 21:55:44.000000 popoll_backend-0.0.53/popoll_backend/model/db/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      683 2024-05-16 21:55:44.000000 popoll_backend-0.0.53/popoll_backend/model/db/answer.py
+-rw-rw-rw-   0 root         (0) root         (0)      798 2024-05-16 21:55:44.000000 popoll_backend-0.0.53/popoll_backend/model/db/date.py
+-rw-rw-rw-   0 root         (0) root         (0)      394 2024-05-16 21:55:44.000000 popoll_backend-0.0.53/popoll_backend/model/db/instrument.py
+-rw-rw-rw-   0 root         (0) root         (0)      371 2024-05-16 21:55:44.000000 popoll_backend-0.0.53/popoll_backend/model/db/option.py
+-rw-rw-rw-   0 root         (0) root         (0)      549 2024-05-16 21:55:44.000000 popoll_backend-0.0.53/popoll_backend/model/db/session.py
+-rw-rw-rw-   0 root         (0) root         (0)      405 2024-05-16 21:55:44.000000 popoll_backend-0.0.53/popoll_backend/model/db/user.py
+-rw-rw-rw-   0 root         (0) root         (0)      666 2024-05-16 21:55:44.000000 popoll_backend-0.0.53/popoll_backend/model/db/user_instruments.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 21:56:04.745149 popoll_backend-0.0.53/popoll_backend/model/payload/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-16 21:55:44.000000 popoll_backend-0.0.53/popoll_backend/model/payload/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2408 2024-05-16 21:55:44.000000 popoll_backend-0.0.53/popoll_backend/model/payload/date_payload.py
+-rw-rw-rw-   0 root         (0) root         (0)      286 2024-05-16 21:55:44.000000 popoll_backend-0.0.53/popoll_backend/model/payload/dates_payload.py
+-rw-rw-rw-   0 root         (0) root         (0)      730 2024-05-16 21:55:44.000000 popoll_backend-0.0.53/popoll_backend/model/payload/history.py
+-rw-rw-rw-   0 root         (0) root         (0)      141 2024-05-16 21:55:44.000000 popoll_backend-0.0.53/popoll_backend/model/payload/id_payload.py
+-rw-rw-rw-   0 root         (0) root         (0)      276 2024-05-16 21:55:44.000000 popoll_backend-0.0.53/popoll_backend/model/payload/instruments_payload.py
+-rw-rw-rw-   0 root         (0) root         (0)      711 2024-05-16 21:55:44.000000 popoll_backend-0.0.53/popoll_backend/model/payload/user.py
+-rw-rw-rw-   0 root         (0) root         (0)      957 2024-05-16 21:55:44.000000 popoll_backend-0.0.53/popoll_backend/model/payload/user_payload.py
+-rw-rw-rw-   0 root         (0) root         (0)      229 2024-05-16 21:55:44.000000 popoll_backend-0.0.53/popoll_backend/model/payload/users_payload.py
+-rw-rw-rw-   0 root         (0) root         (0)      250 2024-05-16 21:55:44.000000 popoll_backend-0.0.53/popoll_backend/model/payload/users_payload_details.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 21:56:04.750149 popoll_backend-0.0.53/popoll_backend/query/
+-rw-rw-rw-   0 root         (0) root         (0)     2121 2024-05-16 21:55:44.000000 popoll_backend-0.0.53/popoll_backend/query/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1029 2024-05-16 21:55:44.000000 popoll_backend-0.0.53/popoll_backend/query/create_answer.py
+-rw-rw-rw-   0 root         (0) root         (0)      995 2024-05-16 21:55:44.000000 popoll_backend-0.0.53/popoll_backend/query/create_date.py
+-rw-rw-rw-   0 root         (0) root         (0)      636 2024-05-16 21:55:44.000000 popoll_backend-0.0.53/popoll_backend/query/create_instrument.py
+-rw-rw-rw-   0 root         (0) root         (0)     1624 2024-05-16 21:55:44.000000 popoll_backend-0.0.53/popoll_backend/query/create_poll.py
+-rw-rw-rw-   0 root         (0) root         (0)      789 2024-05-16 21:55:44.000000 popoll_backend-0.0.53/popoll_backend/query/create_session.py
+-rw-rw-rw-   0 root         (0) root         (0)     1349 2024-05-16 21:55:44.000000 popoll_backend-0.0.53/popoll_backend/query/create_user.py
+-rw-rw-rw-   0 root         (0) root         (0)      527 2024-05-16 21:55:44.000000 popoll_backend-0.0.53/popoll_backend/query/delete_answer.py
+-rw-rw-rw-   0 root         (0) root         (0)      523 2024-05-16 21:55:44.000000 popoll_backend-0.0.53/popoll_backend/query/delete_date.py
+-rw-rw-rw-   0 root         (0) root         (0)      523 2024-05-16 21:55:44.000000 popoll_backend-0.0.53/popoll_backend/query/delete_user.py
+-rw-rw-rw-   0 root         (0) root         (0)      535 2024-05-16 21:55:44.000000 popoll_backend-0.0.53/popoll_backend/query/get_answer.py
+-rw-rw-rw-   0 root         (0) root         (0)     1796 2024-05-16 21:55:44.000000 popoll_backend-0.0.53/popoll_backend/query/get_date.py
+-rw-rw-rw-   0 root         (0) root         (0)      630 2024-05-16 21:55:44.000000 popoll_backend-0.0.53/popoll_backend/query/get_dates.py
+-rw-rw-rw-   0 root         (0) root         (0)      686 2024-05-16 21:55:44.000000 popoll_backend-0.0.53/popoll_backend/query/get_instruments.py
+-rw-rw-rw-   0 root         (0) root         (0)      486 2024-05-16 21:55:44.000000 popoll_backend-0.0.53/popoll_backend/query/get_poll.py
+-rw-rw-rw-   0 root         (0) root         (0)      860 2024-05-16 21:55:44.000000 popoll_backend-0.0.53/popoll_backend/query/get_search_answer.py
+-rw-rw-rw-   0 root         (0) root         (0)      780 2024-05-16 21:55:44.000000 popoll_backend-0.0.53/popoll_backend/query/get_session.py
+-rw-rw-rw-   0 root         (0) root         (0)     1968 2024-05-16 21:55:44.000000 popoll_backend-0.0.53/popoll_backend/query/get_user.py
+-rw-rw-rw-   0 root         (0) root         (0)     1563 2024-05-16 21:55:44.000000 popoll_backend-0.0.53/popoll_backend/query/get_users.py
+-rw-rw-rw-   0 root         (0) root         (0)      732 2024-05-16 21:55:44.000000 popoll_backend-0.0.53/popoll_backend/query/update_answer.py
+-rw-rw-rw-   0 root         (0) root         (0)      991 2024-05-16 21:55:44.000000 popoll_backend-0.0.53/popoll_backend/query/update_date.py
+-rw-rw-rw-   0 root         (0) root         (0)      609 2024-05-16 21:55:44.000000 popoll_backend-0.0.53/popoll_backend/query/update_poll.py
+-rw-rw-rw-   0 root         (0) root         (0)     1415 2024-05-16 21:55:44.000000 popoll_backend-0.0.53/popoll_backend/query/update_user.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 21:56:04.754149 popoll_backend-0.0.53/popoll_backend.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      618 2024-05-16 21:56:04.000000 popoll_backend-0.0.53/popoll_backend.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2538 2024-05-16 21:56:04.000000 popoll_backend-0.0.53/popoll_backend.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-16 21:56:04.000000 popoll_backend-0.0.53/popoll_backend.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       51 2024-05-16 21:56:04.000000 popoll_backend-0.0.53/popoll_backend.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2024-05-16 21:56:04.000000 popoll_backend-0.0.53/popoll_backend.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      845 2024-05-16 21:55:59.000000 popoll_backend-0.0.53/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-16 21:56:04.755149 popoll_backend-0.0.53/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 21:56:04.754149 popoll_backend-0.0.53/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      536 2024-05-16 21:55:44.000000 popoll_backend-0.0.53/tests/test_01_db_creation.py
+-rw-rw-rw-   0 root         (0) root         (0)     1344 2024-05-16 21:55:44.000000 popoll_backend-0.0.53/tests/test_02_simple_adds.py
+-rw-rw-rw-   0 root         (0) root         (0)     1268 2024-05-16 21:55:44.000000 popoll_backend-0.0.53/tests/test_03_no_duplicates.py
+-rw-rw-rw-   0 root         (0) root         (0)     1668 2024-05-16 21:55:44.000000 popoll_backend-0.0.53/tests/test_04_update_user_entry.py
+-rw-rw-rw-   0 root         (0) root         (0)     1927 2024-05-16 21:55:44.000000 popoll_backend-0.0.53/tests/test_05_update_date_entry.py
+-rw-rw-rw-   0 root         (0) root         (0)     1201 2024-05-16 21:55:44.000000 popoll_backend-0.0.53/tests/test_06_update_answer_entry.py
+-rw-rw-rw-   0 root         (0) root         (0)      763 2024-05-16 21:55:44.000000 popoll_backend-0.0.53/tests/test_07_delete_user_entry.py
+-rw-rw-rw-   0 root         (0) root         (0)     1829 2024-05-16 21:55:44.000000 popoll_backend-0.0.53/tests/test_08_delete_date_entry.py
+-rw-rw-rw-   0 root         (0) root         (0)     2328 2024-05-16 21:55:44.000000 popoll_backend-0.0.53/tests/test_09_delete_user_date_entries.py
+-rw-rw-rw-   0 root         (0) root         (0)     1378 2024-05-16 21:55:44.000000 popoll_backend-0.0.53/tests/test_10_get_users.py
+-rw-rw-rw-   0 root         (0) root         (0)      628 2024-05-16 21:55:44.000000 popoll_backend-0.0.53/tests/test_11_get_users_sort_name.py
+-rw-rw-rw-   0 root         (0) root         (0)     1248 2024-05-16 21:55:44.000000 popoll_backend-0.0.53/tests/test_12_get_dates_sort_dateTime.py
+-rw-rw-rw-   0 root         (0) root         (0)     2887 2024-05-16 21:55:44.000000 popoll_backend-0.0.53/tests/test_13_history.py
+-rw-rw-rw-   0 root         (0) root         (0)     2167 2024-05-16 21:55:44.000000 popoll_backend-0.0.53/tests/test_14_get_answers_user.py
+-rw-rw-rw-   0 root         (0) root         (0)     2403 2024-05-16 21:55:44.000000 popoll_backend-0.0.53/tests/test_15_multi_instruments.py
+-rw-rw-rw-   0 root         (0) root         (0)     5145 2024-05-16 21:55:44.000000 popoll_backend-0.0.53/tests/test_16_get_date.py
+-rw-rw-rw-   0 root         (0) root         (0)      478 2024-05-16 21:55:44.000000 popoll_backend-0.0.53/tests/test_17_get_instruments.py
+-rw-rw-rw-   0 root         (0) root         (0)      444 2024-05-16 21:55:44.000000 popoll_backend-0.0.53/tests/test_18_post_instrument.py
+-rw-rw-rw-   0 root         (0) root         (0)      435 2024-05-16 21:55:44.000000 popoll_backend-0.0.53/tests/test_19_delete_database.py
+-rw-rw-rw-   0 root         (0) root         (0)      552 2024-05-16 21:55:44.000000 popoll_backend-0.0.53/tests/test_20_add_answer_no_dupe.py
+-rw-rw-rw-   0 root         (0) root         (0)      863 2024-05-16 21:55:44.000000 popoll_backend-0.0.53/tests/test_21_get_dates.py
```

### Comparing `popoll_backend-0.0.52/PKG-INFO` & `popoll_backend-0.0.53/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: popoll_backend
-Version: 0.0.52
+Version: 0.0.53
 Summary: A small example package
 Author-email: vivi5421 <pypi@villard.me>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `popoll_backend-0.0.52/popoll_backend/__main__.py` & `popoll_backend-0.0.53/popoll_backend/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,23 +108,23 @@
 
 
 
 class DatesEndpoint(Resource):
     def get(self, poll: str): return GetDates(poll).run()
     
     @history
-    def post(self, poll: str) -> int: return CreateDate(poll, body(flask.request, 'title'), body(flask.request, 'date'), body(flask.request, 'time', mandatory=False)).run()
+    def post(self, poll: str) -> int: return CreateDate(poll, body(flask.request, 'title'), body(flask.request, 'date'), body(flask.request, 'time', mandatory=False), body(flask.request, 'end_time', mandatory=False)).run()
 
 
 
 class DateEndpoint(Resource):
     def get(self, poll: str, id:int) -> Dict[str, Any]: return GetDate(poll, id, details=True).run()
     
     @history
-    def put(self, poll: str, id: int) -> int: return UpdateDate(poll, id, body(flask.request, 'title'), body(flask.request, 'date'), body(flask.request, 'time', mandatory=False)).run()
+    def put(self, poll: str, id: int) -> int: return UpdateDate(poll, id, body(flask.request, 'title'), body(flask.request, 'date'), body(flask.request, 'time', mandatory=False), body(flask.request, 'end_time', mandatory=False)).run()
     
     @history
     def delete(self, poll: str, id: int) -> int: return DeleteDate(poll, id).run()
```

### Comparing `popoll_backend-0.0.52/popoll_backend/model/db/answer.py` & `popoll_backend-0.0.53/popoll_backend/model/db/answer.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.52/popoll_backend/model/db/date.py` & `popoll_backend-0.0.53/popoll_backend/model/db/date.py`

 * *Files 18% similar despite different names*

```diff
@@ -7,16 +7,18 @@
 class Date(Payload):
     
     def __init__(self, data: List[Any]):
         self.id: int = data[0]
         self.title: str = data[1]
         self.date: datetime.date = datetime.date.fromisoformat(data[2])
         self.time: Optional[datetime.time] = datetime.time.fromisoformat(data[3]) if data[3] else None
+        self.end_time: Optional[datetime.time] = datetime.time.fromisoformat(data[4]) if data[4] else None
         
     @classmethod
     def create_table(cls):
         return """ CREATE TABLE IF NOT EXISTS dates (
             id integer PRIMARY KEY AUTOINCREMENT,
             title text NOT NULL,
             date text NOT NULL,
-            time text
+            time text,
+            end_time text
         ); """
```

### Comparing `popoll_backend-0.0.52/popoll_backend/model/db/session.py` & `popoll_backend-0.0.53/popoll_backend/model/db/session.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.52/popoll_backend/model/db/user_instruments.py` & `popoll_backend-0.0.53/popoll_backend/model/db/user_instruments.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.52/popoll_backend/model/payload/date_payload.py` & `popoll_backend-0.0.53/popoll_backend/model/payload/date_payload.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.52/popoll_backend/model/payload/history.py` & `popoll_backend-0.0.53/popoll_backend/model/payload/history.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.52/popoll_backend/model/payload/user.py` & `popoll_backend-0.0.53/popoll_backend/model/payload/user.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.52/popoll_backend/model/payload/user_payload.py` & `popoll_backend-0.0.53/popoll_backend/model/payload/user_payload.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.52/popoll_backend/query/__init__.py` & `popoll_backend-0.0.53/popoll_backend/query/__init__.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.52/popoll_backend/query/create_answer.py` & `popoll_backend-0.0.53/popoll_backend/query/create_answer.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.52/popoll_backend/query/create_date.py` & `popoll_backend-0.0.53/popoll_backend/query/update_answer.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,24 @@
-import datetime
 import sqlite3
 from typing import Optional
 
 from popoll_backend.model import Payload
+from popoll_backend.model.db.answer import Answer
 from popoll_backend.query import Query
-from popoll_backend.query.get_date import GetDate
+from popoll_backend.query.get_answer import GetAnswer
 
 
-class CreateDate(Query):
-    
-    title: str
-    date: datetime.date
-    time: Optional[datetime.time]
+class UpdateAnswer(Query):
     
     id: int
+    response: Optional[bool]
     
-    def __init__(self, poll: str, title: str, date: datetime.date, time: Optional[datetime.time]):
+    def __init__(self, poll:str, id: int, response: Optional[bool]):
         super().__init__(poll)
-        self.title = title
-        self.date = date
-        self.time = time
+        self.id = id
+        self.response = response
     
     def process(self, cursor: sqlite3.Cursor):
-        cursor.execute('INSERT INTO dates(title, date, time) VALUES (?, ?, ?)', (self.title, self.date, self.time))
-        self.id = cursor.lastrowid
-        
+        cursor.execute('UPDATE answers SET response=? WHERE id=?', (self.response, self.id))
+    
     def buildResponse(self, cursor: sqlite3.Cursor) -> Payload:
-        return GetDate(self.poll, self.id, False).run(cursor)
+        return GetAnswer(self.poll, self.id).run(cursor)
```

### Comparing `popoll_backend-0.0.52/popoll_backend/query/create_instrument.py` & `popoll_backend-0.0.53/popoll_backend/query/create_instrument.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.52/popoll_backend/query/create_poll.py` & `popoll_backend-0.0.53/popoll_backend/query/create_poll.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.52/popoll_backend/query/create_session.py` & `popoll_backend-0.0.53/popoll_backend/query/create_session.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.52/popoll_backend/query/create_user.py` & `popoll_backend-0.0.53/popoll_backend/query/create_user.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.52/popoll_backend/query/delete_answer.py` & `popoll_backend-0.0.53/popoll_backend/query/delete_answer.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.52/popoll_backend/query/delete_date.py` & `popoll_backend-0.0.53/popoll_backend/query/delete_date.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.52/popoll_backend/query/delete_user.py` & `popoll_backend-0.0.53/popoll_backend/query/delete_user.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.52/popoll_backend/query/get_answer.py` & `popoll_backend-0.0.53/popoll_backend/query/get_answer.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.52/popoll_backend/query/get_date.py` & `popoll_backend-0.0.53/popoll_backend/query/get_date.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.52/popoll_backend/query/get_dates.py` & `popoll_backend-0.0.53/popoll_backend/query/get_dates.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.52/popoll_backend/query/get_instruments.py` & `popoll_backend-0.0.53/popoll_backend/query/get_instruments.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.52/popoll_backend/query/get_search_answer.py` & `popoll_backend-0.0.53/popoll_backend/query/get_search_answer.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.52/popoll_backend/query/get_session.py` & `popoll_backend-0.0.53/popoll_backend/query/get_session.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.52/popoll_backend/query/get_user.py` & `popoll_backend-0.0.53/popoll_backend/query/get_user.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.52/popoll_backend/query/get_users.py` & `popoll_backend-0.0.53/popoll_backend/query/get_users.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.52/popoll_backend/query/update_answer.py` & `popoll_backend-0.0.53/popoll_backend/query/update_poll.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 import sqlite3
-from typing import Optional
 
 from popoll_backend.model import Payload
-from popoll_backend.model.db.answer import Answer
 from popoll_backend.query import Query
-from popoll_backend.query.get_answer import GetAnswer
+from popoll_backend.query.get_poll import GetPoll
 
 
-class UpdateAnswer(Query):
+class UpdatePoll(Query):
     
-    id: int
-    response: Optional[bool]
+    name: str
+    color: str
     
-    def __init__(self, poll:str, id: int, response: Optional[bool]):
+    def __init__(self, poll: str, name: str, color: str):
         super().__init__(poll)
-        self.id = id
-        self.response = response
-    
+        self.name = name
+        self.color = color
+        
     def process(self, cursor: sqlite3.Cursor):
-        cursor.execute('UPDATE answers SET response=? WHERE id=?', (self.response, self.id))
+        cursor.execute('UPDATE options SET name=?, color=?', (self.name, self.color))
     
     def buildResponse(self, cursor: sqlite3.Cursor) -> Payload:
-        return GetAnswer(self.poll, self.id).run(cursor)
+        return GetPoll(self.poll).run(cursor)
```

### Comparing `popoll_backend-0.0.52/popoll_backend/query/update_date.py` & `popoll_backend-0.0.53/popoll_backend/query/update_date.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,20 +9,22 @@
 
 class UpdateDate(Query):
     
     id: int
     title: str
     date: datetime.date
     time: Optional[datetime.time]
+    end_time: Optional[datetime.time]
     
-    def __init__(self, poll: str, id: int, title: str, date: datetime.date, time: Optional[datetime.time]):
+    def __init__(self, poll: str, id: int, title: str, date: datetime.date, time: Optional[datetime.time], end_time: Optional[datetime.time]):
         super().__init__(poll)
         self.id = id
         self.title = title
         self.date = date
         self.time = time
+        self.end_time = end_time
         
     def process(self, cursor: sqlite3.Cursor):
-        cursor.execute('UPDATE dates SET title=?, date=?, time=? WHERE id=?', (self.title, self.date, self.time, self.id))
+        cursor.execute('UPDATE dates SET title=?, date=?, time=?, end_time=? WHERE id=?', (self.title, self.date, self.time, self.end_time, self.id))
     
     def buildResponse(self, cursor: sqlite3.Cursor) -> Payload:
         return GetDate(self.poll, self.id, False).run(cursor)
```

### Comparing `popoll_backend-0.0.52/popoll_backend/query/update_user.py` & `popoll_backend-0.0.53/popoll_backend/query/update_user.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.52/popoll_backend.egg-info/PKG-INFO` & `popoll_backend-0.0.53/popoll_backend.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: popoll_backend
-Version: 0.0.52
+Version: 0.0.53
 Summary: A small example package
 Author-email: vivi5421 <pypi@villard.me>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `popoll_backend-0.0.52/popoll_backend.egg-info/SOURCES.txt` & `popoll_backend-0.0.53/popoll_backend.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.52/pyproject.toml` & `popoll_backend-0.0.53/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", 'wheel', 'flask', 'flask_cors', 'flask-restful', 'jsonpickle', 'sqlalchemy', 'sqlalchemy-utils', 'psycopg2-binary', 'pyyaml', 'pyopenssl']
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "popoll_backend"
-version = "0.0.52"
+version = "0.0.53"
 authors = [
   { name="vivi5421", email="pypi@villard.me" },
 ]
 description = "A small example package"
 readme = "README.md"
 license = { file = "LICENSE" }
 dependencies = [
```

### Comparing `popoll_backend-0.0.52/tests/test_01_db_creation.py` & `popoll_backend-0.0.53/tests/test_01_db_creation.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.52/tests/test_02_simple_adds.py` & `popoll_backend-0.0.53/tests/test_02_simple_adds.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from tests import IntegrationTest
 
 class TestSimpleAdds(IntegrationTest):
 
     def setUp(self):
         super().setUp()
         self.user1_id = self.create_user('user1', self.instru1_id, [])
-        self.date1_id = self.create_date(date='2025-03-10', time='15:00:00', title='firstDate')
+        self.date1_id = self.create_date(date='2025-03-10', time='15:00:00', title='firstDate', end_time='18:00:00')
         self.answer1_id = self.create_answer(user_id=self.user1_id, date_id=self.date1_id)
         
     def test_simple_adds(self):
         assert self.user1_id != None
         assert self.date1_id != None
         assert self.answer1_id != None
         _json = self.get_user(self.user1_id)
@@ -18,10 +18,11 @@
         assert _json['user']['main_instrument']['id'] == self.instru1_id
         assert len(_json['user']['instruments']) == 0
         assert len(_json['dates']) == 1
         assert _json['dates'][0]['date']['id'] == self.date1_id
         assert _json['dates'][0]['date']['title'] == 'firstDate'
         assert _json['dates'][0]['date']['date'] == '2025-03-10'
         assert _json['dates'][0]['date']['time'] == '15:00:00'
+        assert _json['dates'][0]['date']['end_time'] == '18:00:00'
         assert _json['dates'][0]['answer']['id'] == self.answer1_id
         assert _json['dates'][0]['answer']['response'] == True
```

### Comparing `popoll_backend-0.0.52/tests/test_03_no_duplicates.py` & `popoll_backend-0.0.53/tests/test_03_no_duplicates.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from tests import IntegrationTest, TestForwardError
 
 class TestNoDuplicates(IntegrationTest):
 
     def setUp(self):
         super().setUp()
         self.user1_id = self.create_user('user1', self.instru1_id, [])
-        self.date1_id = self.create_date(date='2025-03-10', time='15:00:00', title='firstDate')
+        self.date1_id = self.create_date(date='2025-03-10', time='15:00:00', title='firstDate', end_time=None)
         self.answer1_id = self.create_answer(user_id=self.user1_id, date_id=self.date1_id)
         
     def test_no_duplicate_user(self):
         rs = self.create_user('user1', self.instru1_id, [], fail=True)
         assert rs.status_code == 400
         # TODO assert json.loads(rs.json)["message"] == 'User with name user1 already exists.'
     
@@ -20,11 +20,11 @@
         assert rs.status_code == 400
         user2_id = self.create_user('user2', self.instru2_id, [])
         _json = self.get_users()
         assert len(_json['users']) == 2
 
             
     def test_can_duplicate_dates(self):
-        date2_id = self.create_date(date='2025-03-10', time='15:00:00', title='firstDate')
+        date2_id = self.create_date(date='2025-03-10', time='15:00:00', title='firstDate', end_time='18:00:00')
         _json = self.get_user(self.user1_id)
         assert len(_json['dates']) == 2
         assert self.date1_id != date2_id
```

### Comparing `popoll_backend-0.0.52/tests/test_04_update_user_entry.py` & `popoll_backend-0.0.53/tests/test_04_update_user_entry.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 class TestUpdateuserEntry(IntegrationTest):
 
     def setUp(self):
         super().setUp()
         self.user1_id = self.create_user('user1', self.instru1_id, [])
         self.user3_id = self.create_user('user3', self.instru1_id, [])
-        self.date1_id = self.create_date(date='2025-03-10', time='15:00:00', title='firstDate')
+        self.date1_id = self.create_date(date='2025-03-10', time='15:00:00', title='firstDate', end_time=None)
         self.answer1_id = self.create_answer(user_id=self.user1_id, date_id=self.date1_id)
         
     def test_update_user_entry(self):
         updated_user1_id = self.update_user(self.user1_id, 'user2', self.instru2_id, [])
         assert updated_user1_id == self.user1_id
         _json = self.get_user(updated_user1_id)
         assert _json['user']['user']['name'] == 'user2'
```

### Comparing `popoll_backend-0.0.52/tests/test_05_update_date_entry.py` & `popoll_backend-0.0.53/tests/test_05_update_date_entry.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 from tests import IntegrationTest, TestForwardError
 
 class TestUpdateDateEntry(IntegrationTest):
 
     def setUp(self):
         super().setUp()
         self.user1_id = self.create_user('user1', self.instru1_id, [])
-        self.date1_id = self.create_date(date='2025-03-10', time='15:00:00', title='firstDate')
-        self.date2_id = self.create_date(date='2025-03-12', time=None, title='secondDate')
+        self.date1_id = self.create_date(date='2025-03-10', time='15:00:00', title='firstDate', end_time=None)
+        self.date2_id = self.create_date(date='2025-03-12', time=None, title='secondDate', end_time=None)
         self.answer1_id = self.create_answer(user_id=self.user1_id, date_id=self.date1_id)
         
     def test_update_date_entry(self):
         updated_date1_id = self.udpate_date(self.date1_id, date='2025-03-10', time='18:00:00', title='firstDateUpdated')
         assert updated_date1_id == self.date1_id
         _json = self.get_user(self.user1_id)
         assert _json['dates'][0]['date']['date'] == '2025-03-10'
         assert _json['dates'][0]['date']['time'] == '18:00:00'
+        assert _json['dates'][0]['date']['end_time'] == None
         assert _json['dates'][0]['date']['title'] == 'firstDateUpdated'
         
     def test_update_date_entry_remove_time(self):
         updated_date1_id = self.udpate_date(self.date1_id, date='2025-03-10', time=None, title='firstDateUpdated')
         assert updated_date1_id == self.date1_id
         _json = self.get_user(self.user1_id)
         assert _json['dates'][0]['date']['date'] == '2025-03-10'
```

### Comparing `popoll_backend-0.0.52/tests/test_06_update_answer_entry.py` & `popoll_backend-0.0.53/tests/test_06_update_answer_entry.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 class TestUpdateAnswerEntry(IntegrationTest):
 
     def setUp(self):
         super().setUp()
         self.user1_id = self.create_user('user1', self.instru1_id, [])
         self.user2_id = self.create_user('user2', self.instru3_id, [])
-        self.date1_id = self.create_date(date='2025-03-10', time='15:00:00', title='firstDate')
+        self.date1_id = self.create_date(date='2025-03-10', time='15:00:00', title='firstDate', end_time=None)
         self.answer1_id = self.create_answer(user_id=self.user1_id, date_id=self.date1_id)
         
     def test_update_answer_entry(self):
         updated_answer1_id = self.update_answer(self.answer1_id, False)
         assert updated_answer1_id == self.answer1_id
         _json = self.get_user(self.user1_id)
         assert _json['dates'][0]['answer']['response'] == False
```

### Comparing `popoll_backend-0.0.52/tests/test_07_delete_user_entry.py` & `popoll_backend-0.0.53/tests/test_09_delete_user_date_entries.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,17 +1,46 @@
 from tests import IntegrationTest
 
-class TestDeleteUserEntry(IntegrationTest):
+class TestDeleteUserDateEntries(IntegrationTest):
 
     def setUp(self):
         super().setUp()
         self.user1_id = self.create_user('user1', self.instru1_id, [])
         self.user2_id = self.create_user('user2', self.instru2_id, [])
-        self.date1_id = self.create_date(date='2025-03-10', time='15:00:00', title='firstDate')
+        self.date1_id = self.create_date(date='2025-03-10', time='15:00:00', title='firstDate', end_time=None)
+        self.date2_id = self.create_date(date='2025-03-11', time='18:00:00', title='secondDate', end_time=None)
+        self.date3_id = self.create_date(date='2025-03-12', time=None, title='thirdDate', end_time=None)
         self.answer1_id = self.create_answer(user_id=self.user1_id, date_id=self.date1_id)
+        self.answer2_id = self.create_answer(user_id=self.user1_id, date_id=self.date2_id)
+        self.answer3_id = self.create_answer(user_id=self.user1_id, date_id=self.date3_id)
+        self.answer4_id = self.create_answer(user_id=self.user2_id, date_id=self.date1_id)
+        self.answer5_id = self.create_answer(user_id=self.user2_id, date_id=self.date2_id)
+        self.answer6_id = self.create_answer(user_id=self.user2_id, date_id=self.date3_id)
         
-    def test_delete_user_entry(self):
-        deleted_user_id = self.delete_user(self.user1_id)
-        assert deleted_user_id == self.user1_id
+    def test_delete_user_date_entries(self):
+        _json = self.get_users()
+        assert len(_json['users']) == 2
+        _json_user1 = self.get_user(self.user1_id)
+        assert len(_json_user1['dates']) == 3
+        assert _json_user1['dates'][0].get('answer', None) != None
+        
+        self.delete_date(self.date1_id)
+        _json = self.get_user(self.user1_id)
+        assert len(_json['dates']) == 2
+        
+        self.delete_user(self.user1_id)
         _json = self.get_users()
         assert len(_json['users']) == 1
-        assert _json['users'][0]['user']['name'] == 'user2'        
+        assert _json['users'][0]['user']['id'] == self.user2_id
+        
+        user3_id = self.create_user('user3', self.instru3_id, [])
+        assert self.user1_id != user3_id
+        _json = self.get_users()
+        assert len(_json['users']) == 2
+        _json = self.get_user(user3_id)
+        assert _json['dates'][1].get('answer', None) == None
+        
+        answer7_id = self.create_answer(user_id=user3_id, date_id=self.date2_id)
+        self.update_answer(answer7_id, False)
+        _json = self.get_user(user3_id)
+        assert len(_json['dates']) == 2
+        assert _json['dates'][0]['answer']['response'] == False
```

### Comparing `popoll_backend-0.0.52/tests/test_08_delete_date_entry.py` & `popoll_backend-0.0.53/tests/test_08_delete_date_entry.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 
 class TestDeleteDateEntry(IntegrationTest):
 
     def setUp(self):
         super().setUp()
         self.user1_id = self.create_user('user1', self.instru1_id, [])
         self.user2_id = self.create_user('user2', self.instru2_id, [])
-        self.date1_id = self.create_date(date='2025-03-10', time='15:00:00', title='firstDate')
-        self.date2_id = self.create_date(date='2025-03-11', time='18:00:00', title='secondDate')
-        self.date3_id = self.create_date(date='2025-03-12', time=None, title='thirdDate')
+        self.date1_id = self.create_date(date='2025-03-10', time='15:00:00', title='firstDate', end_time=None)
+        self.date2_id = self.create_date(date='2025-03-11', time='18:00:00', title='secondDate', end_time=None)
+        self.date3_id = self.create_date(date='2025-03-12', time=None, title='thirdDate', end_time=None)
         self.answer1_id = self.create_answer(user_id=self.user1_id, date_id=self.date1_id)
         self.answer2_id = self.create_answer(user_id=self.user1_id, date_id=self.date2_id)
         self.answer3_id = self.create_answer(user_id=self.user1_id, date_id=self.date3_id)
         self.answer4_id = self.create_answer(user_id=self.user2_id, date_id=self.date1_id)
         self.answer5_id = self.create_answer(user_id=self.user2_id, date_id=self.date2_id)
         self.answer6_id = self.create_answer(user_id=self.user2_id, date_id=self.date3_id)
```

### Comparing `popoll_backend-0.0.52/tests/test_09_delete_user_date_entries.py` & `popoll_backend-0.0.53/tests/test_14_get_answers_user.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,46 +1,40 @@
 from tests import IntegrationTest
 
-class TestDeleteUserDateEntries(IntegrationTest):
+class TestAnswersPerUser(IntegrationTest):
 
     def setUp(self):
         super().setUp()
         self.user1_id = self.create_user('user1', self.instru1_id, [])
         self.user2_id = self.create_user('user2', self.instru2_id, [])
-        self.date1_id = self.create_date(date='2025-03-10', time='15:00:00', title='firstDate')
-        self.date2_id = self.create_date(date='2025-03-11', time='18:00:00', title='secondDate')
-        self.date3_id = self.create_date(date='2025-03-12', time=None, title='thirdDate')
+        self.date1_id = self.create_date(date='2025-03-10', time='15:00:00', title='firstDate', end_time=None)
+        self.date2_id = self.create_date(date='2025-03-11', time='18:00:00', title='secondDate', end_time=None)
+        self.date3_id = self.create_date(date='2025-03-12', time=None, title='thirdDate', end_time=None)
         self.answer1_id = self.create_answer(user_id=self.user1_id, date_id=self.date1_id)
         self.answer2_id = self.create_answer(user_id=self.user1_id, date_id=self.date2_id)
         self.answer3_id = self.create_answer(user_id=self.user1_id, date_id=self.date3_id)
         self.answer4_id = self.create_answer(user_id=self.user2_id, date_id=self.date1_id)
         self.answer5_id = self.create_answer(user_id=self.user2_id, date_id=self.date2_id)
         self.answer6_id = self.create_answer(user_id=self.user2_id, date_id=self.date3_id)
         
-    def test_delete_user_date_entries(self):
-        _json = self.get_users()
-        assert len(_json['users']) == 2
-        _json_user1 = self.get_user(self.user1_id)
-        assert len(_json_user1['dates']) == 3
-        assert _json_user1['dates'][0].get('answer', None) != None
-        
-        self.delete_date(self.date1_id)
+    def test_get_answers_user(self):            
         _json = self.get_user(self.user1_id)
-        assert len(_json['dates']) == 2
-        
-        self.delete_user(self.user1_id)
-        _json = self.get_users()
-        assert len(_json['users']) == 1
-        assert _json['users'][0]['user']['id'] == self.user2_id
+        assert _json['user']['user']['id'] == self.user1_id
+        assert len(_json['dates']) == 3
+        assert _json['dates'][0].get('answer', None) != None
+        assert _json['dates'][0]['answer']['response'] == True
         
-        user3_id = self.create_user('user3', self.instru3_id, [])
-        assert self.user1_id != user3_id
-        _json = self.get_users()
-        assert len(_json['users']) == 2
-        _json = self.get_user(user3_id)
-        assert _json['dates'][1].get('answer', None) == None
+        assert _json['dates'][1].get('answer', None) != None
+        assert _json['dates'][1]['answer']['response'] == True
         
-        answer7_id = self.create_answer(user_id=user3_id, date_id=self.date2_id)
-        self.update_answer(answer7_id, False)
-        _json = self.get_user(user3_id)
-        assert len(_json['dates']) == 2
-        assert _json['dates'][0]['answer']['response'] == False
+        assert _json['dates'][2].get('answer', None) != None
+        assert _json['dates'][2]['answer']['response'] == True
+
+    # def test_get_answer_answerId(self):
+    #     _json = self.toJSON(self.get_answer(self.answer1_id))
+    #     assert len(_json['answers']) == 1
+    #     assert _json['answers'][0]['user_id'] == self.user1_id
+    #     assert _json['answers'][0]['date_id'] == self.date1_id
+    #     assert _json['answers'][0]['response'] == True
+
+    #     _json = self.toJSON(self.get_answer(999))
+    #     assert len(_json['answers']) == 0
```

### Comparing `popoll_backend-0.0.52/tests/test_10_get_users.py` & `popoll_backend-0.0.53/tests/test_10_get_users.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 
 class TestGetUsersEntries(IntegrationTest):
 
     def setUp(self):
         super().setUp()
         self.user1_id = self.create_user('user1', self.instru1_id, [])
         self.user2_id = self.create_user('user2', self.instru2_id, [])
-        self.date1_id = self.create_date(date='2025-03-10', time='15:00:00', title='firstDate')
-        self.date2_id = self.create_date(date='2025-03-11', time='18:00:00', title='secondDate')
-        self.date3_id = self.create_date(date='2025-03-12', time=None, title='thirdDate')
+        self.date1_id = self.create_date(date='2025-03-10', time='15:00:00', title='firstDate', end_time=None)
+        self.date2_id = self.create_date(date='2025-03-11', time='18:00:00', title='secondDate', end_time=None)
+        self.date3_id = self.create_date(date='2025-03-12', time=None, title='thirdDate', end_time=None)
         self.answer1_id = self.create_answer(user_id=self.user1_id, date_id=self.date1_id)
         self.answer2_id = self.create_answer(user_id=self.user1_id, date_id=self.date2_id)
         self.answer3_id = self.create_answer(user_id=self.user1_id, date_id=self.date3_id)
         self.answer4_id = self.create_answer(user_id=self.user2_id, date_id=self.date1_id)
         self.answer5_id = self.create_answer(user_id=self.user2_id, date_id=self.date2_id)
         self.answer6_id = self.create_answer(user_id=self.user2_id, date_id=self.date3_id)
```

### Comparing `popoll_backend-0.0.52/tests/test_11_get_users_sort_name.py` & `popoll_backend-0.0.53/tests/test_11_get_users_sort_name.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.52/tests/test_12_get_dates_sort_dateTime.py` & `popoll_backend-0.0.53/tests/test_12_get_dates_sort_dateTime.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,19 +5,19 @@
         assert expectedTime == actualDate['time']
 
 class TestGetDatesSortByDate(IntegrationTest):
 
     def setUp(self):
         super().setUp()
         self.user1_id = self.create_user(name='user1', main_instrument=self.instru1_id, instruments=[])
-        self.date1_id = self.create_date(date='2025-03-12', time='15:00:00', title='firstDate')
+        self.date1_id = self.create_date(date='2025-03-12', time='15:00:00', title='firstDate', end_time=None)
         self.create_answer(self.user1_id, self.date1_id)
-        self.date2_id = self.create_date(date='2025-03-11', time='18:00:00', title='secondDate')
+        self.date2_id = self.create_date(date='2025-03-11', time='18:00:00', title='secondDate', end_time=None)
         self.create_answer(self.user1_id, self.date2_id)
-        self.date3_id = self.create_date(date='2025-03-11', time=None, title='thirdDate')
+        self.date3_id = self.create_date(date='2025-03-11', time=None, title='thirdDate', end_time=None)
         self.create_answer(self.user1_id, self.date3_id)
         
     def test_get_user_sorted(self):
         _json = self.get_user(self.user1_id)
         assert len(_json['dates']) == 3
         _test_date_time('2025-03-11', None, _json['dates'][0]['date'])
         _test_date_time('2025-03-11', '18:00:00', _json['dates'][1]['date'])
```

### Comparing `popoll_backend-0.0.52/tests/test_13_history.py` & `popoll_backend-0.0.53/tests/test_13_history.py`

 * *Files identical despite different names*

### Comparing `popoll_backend-0.0.52/tests/test_15_multi_instruments.py` & `popoll_backend-0.0.53/tests/test_15_multi_instruments.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
         # assert isMain == actual['is_main']
 
 class TestMultiInstruments(IntegrationTest):
 
     def setUp(self):
         super().setUp()
         self.user1_id = self.create_user('user1', self.instru1_id, [self.instru2_id])
-        self.date1_id = self.create_date(date='2025-03-10', time='15:00:00', title='firstDate')
+        self.date1_id = self.create_date(date='2025-03-10', time='15:00:00', title='firstDate', end_time=None)
         self.answer1_id = self.create_answer(user_id=self.user1_id, date_id=self.date1_id)
         _json = self.get_user(self.user1_id)
         _test_instru(self.instru1_id, self.INSTRU1, True, _json['user']['main_instrument'])
         instruments = _json['user']['instruments']
         assert len(instruments) == 1
         _test_instru(self.instru2_id, self.INSTRU2, False, instruments[0])
```

### Comparing `popoll_backend-0.0.52/tests/test_16_get_date.py` & `popoll_backend-0.0.53/tests/test_16_get_date.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
         self.user6_id = self.create_user('user6', self.instru2_id, [])
         self.user7_id = self.create_user('user7', self.instru2_id, [])
         
         self.user8_id = self.create_user('user8', self.instru3_id, [self.instru1_id])
         self.user9_id = self.create_user('user9', self.instru3_id, [self.instru1_id, self.instru2_id])
         self.user10_id = self.create_user('user10', self.instru3_id, [])
         
-        self.date1_id = self.create_date(date='2025-03-10', time='15:00:00', title='firstDate')
+        self.date1_id = self.create_date(date='2025-03-10', time='15:00:00', title='firstDate', end_time=None)
         
         self.answer1_id = self.create_answer(user_id=self.user1_id, date_id=self.date1_id)
         self.answer2_id = self.create_answer_false(user_id=self.user2_id, date_id=self.date1_id)
         # self.answer3_id is None
         self.answer4_id = self.create_answer(self.user4_id, self.date1_id)
         self.answer5_id = self.create_answer(self.user5_id, self.date1_id)
         self.answer6_id = self.create_answer_false(self.user6_id, self.date1_id)
```

### Comparing `popoll_backend-0.0.52/tests/test_20_add_answer_no_dupe.py` & `popoll_backend-0.0.53/tests/test_20_add_answer_no_dupe.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from tests import IntegrationTest
 
 class TestAddAnswerNoDupe(IntegrationTest):
 
     def setUp(self):
         super().setUp()
         self.user1_id = self.create_user('user1', self.instru1_id, [])
-        self.date1_id = self.create_date(date='2025-03-10', time='15:00:00', title='firstDate')
+        self.date1_id = self.create_date(date='2025-03-10', time='15:00:00', title='firstDate', end_time=None)
         self.answer1_id = self.create_answer(self.user1_id, self.date1_id)
 
 
     def test_delete_database(self):            
         rs = self.create_answer(self.user1_id, self.date1_id, fail=True)
         assert rs.status_code == 400
```

### Comparing `popoll_backend-0.0.52/tests/test_21_get_dates.py` & `popoll_backend-0.0.53/tests/test_21_get_dates.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from tests import IntegrationTest
 
 class TestAddAnswerNoDupe(IntegrationTest):
 
     def setUp(self):
         super().setUp()
-        self.date1_id = self.create_date(date='2025-03-10', time='15:00:00', title='firstDate')
-        self.date2_id = self.create_date(date='2025-03-11', time=None, title='secondDate')
+        self.date1_id = self.create_date(date='2025-03-10', time='15:00:00', title='firstDate', end_time=None)
+        self.date2_id = self.create_date(date='2025-03-11', time=None, title='secondDate', end_time=None)
 
     def _assert_date(self, e_id, e_date, e_time, e_title, actual):
         assert e_id == actual['id']
         assert e_title == actual['title']
         assert e_date == actual['date']
         assert e_time == actual['time']
```

