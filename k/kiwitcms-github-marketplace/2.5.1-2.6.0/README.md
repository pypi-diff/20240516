# Comparing `tmp/kiwitcms-github-marketplace-2.5.1.tar.gz` & `tmp/kiwitcms-github-marketplace-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kiwitcms-github-marketplace-2.5.1.tar", last modified: Mon May  6 17:01:04 2024, max compression
+gzip compressed data, was "kiwitcms-github-marketplace-2.6.0.tar", last modified: Thu May 16 18:46:58 2024, max compression
```

## Comparing `kiwitcms-github-marketplace-2.5.1.tar` & `kiwitcms-github-marketplace-2.6.0.tar`

### file list

```diff
@@ -1,62 +1,67 @@
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-05-06 17:01:04.302157 kiwitcms-github-marketplace-2.5.1/
--rw-rw-r--   0 senko     (1001) senko     (1001)    35149 2021-04-27 19:25:31.000000 kiwitcms-github-marketplace-2.5.1/LICENSE
--rw-rw-r--   0 senko     (1001) senko     (1001)      208 2022-02-23 19:15:12.000000 kiwitcms-github-marketplace-2.5.1/MANIFEST.in
--rw-r--r--   0 senko     (1001) senko     (1001)    12979 2024-05-06 17:01:04.302157 kiwitcms-github-marketplace-2.5.1/PKG-INFO
--rw-r--r--   0 senko     (1001) senko     (1001)    12129 2024-05-06 17:00:42.000000 kiwitcms-github-marketplace-2.5.1/README.rst
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-05-06 17:01:04.301158 kiwitcms-github-marketplace-2.5.1/kiwitcms_github_marketplace.egg-info/
--rw-r--r--   0 senko     (1001) senko     (1001)    12979 2024-05-06 17:01:04.000000 kiwitcms-github-marketplace-2.5.1/kiwitcms_github_marketplace.egg-info/PKG-INFO
--rw-r--r--   0 senko     (1001) senko     (1001)     2055 2024-05-06 17:01:04.000000 kiwitcms-github-marketplace-2.5.1/kiwitcms_github_marketplace.egg-info/SOURCES.txt
--rw-r--r--   0 senko     (1001) senko     (1001)        1 2024-05-06 17:01:04.000000 kiwitcms-github-marketplace-2.5.1/kiwitcms_github_marketplace.egg-info/dependency_links.txt
--rw-r--r--   0 senko     (1001) senko     (1001)       64 2024-05-06 17:01:04.000000 kiwitcms-github-marketplace-2.5.1/kiwitcms_github_marketplace.egg-info/entry_points.txt
--rw-r--r--   0 senko     (1001) senko     (1001)        1 2024-05-06 17:01:04.000000 kiwitcms-github-marketplace-2.5.1/kiwitcms_github_marketplace.egg-info/not-zip-safe
--rw-r--r--   0 senko     (1001) senko     (1001)       68 2024-05-06 17:01:04.000000 kiwitcms-github-marketplace-2.5.1/kiwitcms_github_marketplace.egg-info/requires.txt
--rw-r--r--   0 senko     (1001) senko     (1001)       42 2024-05-06 17:01:04.000000 kiwitcms-github-marketplace-2.5.1/kiwitcms_github_marketplace.egg-info/top_level.txt
--rw-r--r--   0 senko     (1001) senko     (1001)      133 2024-05-06 12:49:10.000000 kiwitcms-github-marketplace-2.5.1/requirements.txt
--rw-rw-r--   0 senko     (1001) senko     (1001)      129 2024-05-06 17:01:04.302157 kiwitcms-github-marketplace-2.5.1/setup.cfg
--rw-r--r--   0 senko     (1001) senko     (1001)     1783 2024-05-06 17:00:42.000000 kiwitcms-github-marketplace-2.5.1/setup.py
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-05-06 17:01:04.301158 kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/
--rw-rw-r--   0 senko     (1001) senko     (1001)        0 2021-04-27 19:25:31.000000 kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/__init__.py
--rw-r--r--   0 senko     (1001) senko     (1001)     6031 2023-04-14 16:28:27.000000 kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/admin.py
--rw-rw-r--   0 senko     (1001) senko     (1001)      321 2022-02-20 13:20:22.000000 kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/apps.py
--rw-rw-r--   0 senko     (1001) senko     (1001)      553 2022-02-20 13:20:22.000000 kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/checks.py
--rw-rw-r--   0 senko     (1001) senko     (1001)     2613 2022-02-16 15:05:52.000000 kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/docker.py
--rw-rw-r--   0 senko     (1001) senko     (1001)      879 2022-02-21 15:47:58.000000 kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/mailchimp.py
--rw-rw-r--   0 senko     (1001) senko     (1001)      374 2022-02-09 11:11:58.000000 kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/menu.py
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-05-06 17:01:04.302157 kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/migrations/
--rw-r--r--   0 senko     (1001) senko     (1001)     1532 2024-01-05 12:16:28.000000 kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/migrations/0001_initial.py
--rw-r--r--   0 senko     (1001) senko     (1001)      965 2023-04-07 11:54:56.000000 kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/migrations/0002_update_fields.py
--rw-r--r--   0 senko     (1001) senko     (1001)      415 2023-04-07 11:54:56.000000 kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/migrations/0003_sender_email_field.py
--rw-r--r--   0 senko     (1001) senko     (1001)      391 2023-04-07 11:54:56.000000 kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/migrations/0004_models_jsonfield.py
--rw-r--r--   0 senko     (1001) senko     (1001)      613 2023-04-07 11:54:56.000000 kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/migrations/0005_add_support_and_tenant_flags.py
--rw-r--r--   0 senko     (1001) senko     (1001)     1039 2023-04-07 11:54:56.000000 kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/migrations/0006_add_subscription_field.py
--rw-r--r--   0 senko     (1001) senko     (1001)      694 2023-04-14 16:28:27.000000 kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/migrations/0007_manualpurchase.py
--rw-rw-r--   0 senko     (1001) senko     (1001)        0 2021-04-27 19:25:31.000000 kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/migrations/__init__.py
--rw-r--r--   0 senko     (1001) senko     (1001)     1712 2023-04-14 16:28:27.000000 kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/models.py
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-05-06 17:01:04.302157 kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/quay/
--rw-rw-r--   0 senko     (1001) senko     (1001)       57 2022-02-09 14:16:51.000000 kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/quay/__init__.py
--rw-rw-r--   0 senko     (1001) senko     (1001)     2353 2022-02-09 21:44:26.000000 kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/quay/quay_api_client.py
--rw-r--r--   0 senko     (1001) senko     (1001)     4708 2024-04-17 13:31:58.000000 kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/quay/quay_session.py
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-05-06 17:01:04.300158 kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/static/
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-05-06 17:01:04.300158 kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/static/tcms_github_marketplace/
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-05-06 17:01:04.302157 kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/static/tcms_github_marketplace/js/
--rw-rw-r--   0 senko     (1001) senko     (1001)      924 2022-02-16 15:05:52.000000 kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/static/tcms_github_marketplace/js/subscription.js
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-05-06 17:01:04.300158 kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/templates/
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-05-06 17:01:04.302157 kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/templates/email/
--rw-r--r--   0 senko     (1001) senko     (1001)     1450 2023-04-14 16:28:27.000000 kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/templates/email/manual_subscription_notification.txt
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-05-06 17:01:04.302157 kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/templates/tcms_github_marketplace/
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-05-06 17:01:04.302157 kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/templates/tcms_github_marketplace/email/
--rw-rw-r--   0 senko     (1001) senko     (1001)      270 2022-08-14 14:51:18.000000 kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/templates/tcms_github_marketplace/email/exit_poll.txt
--rw-rw-r--   0 senko     (1001) senko     (1001)    11048 2022-08-04 08:25:18.000000 kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/templates/tcms_github_marketplace/subscription.html
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-05-06 17:01:04.302157 kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/templates/tcms_tenants/
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-05-06 17:01:04.302157 kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/templates/tcms_tenants/include/
--rw-r--r--   0 senko     (1001) senko     (1001)     1030 2024-05-02 21:53:41.000000 kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/templates/tcms_tenants/include/tenant_extra_emails.html
--rw-r--r--   0 senko     (1001) senko     (1001)      163 2024-05-02 21:53:41.000000 kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/templates/tcms_tenants/override_edit.html
--rw-r--r--   0 senko     (1001) senko     (1001)     2629 2024-05-02 21:53:41.000000 kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/templates/tcms_tenants/override_new.html
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-05-06 17:01:04.302157 kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/templatetags/
--rw-rw-r--   0 senko     (1001) senko     (1001)        0 2021-04-27 19:25:31.000000 kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/templatetags/__init__.py
--rw-rw-r--   0 senko     (1001) senko     (1001)      373 2021-04-27 19:25:31.000000 kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/templatetags/github_marketplace.py
--rw-rw-r--   0 senko     (1001) senko     (1001)      804 2022-02-09 11:11:58.000000 kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/urls.py
--rw-r--r--   0 senko     (1001) senko     (1001)     5893 2024-05-06 17:00:42.000000 kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/utils.py
--rw-r--r--   0 senko     (1001) senko     (1001)    28284 2024-05-03 19:17:08.000000 kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/views.py
-drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-05-06 17:01:04.302157 kiwitcms-github-marketplace-2.5.1/tcms_settings_dir/
--rw-rw-r--   0 senko     (1001) senko     (1001)       65 2022-02-09 11:11:58.000000 kiwitcms-github-marketplace-2.5.1/tcms_settings_dir/__init__.py
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-05-16 18:46:58.546892 kiwitcms-github-marketplace-2.6.0/
+-rw-rw-r--   0 senko     (1001) senko     (1001)    35149 2021-04-27 19:25:31.000000 kiwitcms-github-marketplace-2.6.0/LICENSE
+-rw-rw-r--   0 senko     (1001) senko     (1001)      208 2022-02-23 19:15:12.000000 kiwitcms-github-marketplace-2.6.0/MANIFEST.in
+-rw-r--r--   0 senko     (1001) senko     (1001)    13509 2024-05-16 18:46:58.546892 kiwitcms-github-marketplace-2.6.0/PKG-INFO
+-rw-r--r--   0 senko     (1001) senko     (1001)    12659 2024-05-16 18:44:54.000000 kiwitcms-github-marketplace-2.6.0/README.rst
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-05-16 18:46:58.544892 kiwitcms-github-marketplace-2.6.0/kiwitcms_github_marketplace.egg-info/
+-rw-r--r--   0 senko     (1001) senko     (1001)    13509 2024-05-16 18:46:58.000000 kiwitcms-github-marketplace-2.6.0/kiwitcms_github_marketplace.egg-info/PKG-INFO
+-rw-r--r--   0 senko     (1001) senko     (1001)     2251 2024-05-16 18:46:58.000000 kiwitcms-github-marketplace-2.6.0/kiwitcms_github_marketplace.egg-info/SOURCES.txt
+-rw-r--r--   0 senko     (1001) senko     (1001)        1 2024-05-16 18:46:58.000000 kiwitcms-github-marketplace-2.6.0/kiwitcms_github_marketplace.egg-info/dependency_links.txt
+-rw-r--r--   0 senko     (1001) senko     (1001)       64 2024-05-16 18:46:58.000000 kiwitcms-github-marketplace-2.6.0/kiwitcms_github_marketplace.egg-info/entry_points.txt
+-rw-r--r--   0 senko     (1001) senko     (1001)        1 2024-05-16 18:46:58.000000 kiwitcms-github-marketplace-2.6.0/kiwitcms_github_marketplace.egg-info/not-zip-safe
+-rw-r--r--   0 senko     (1001) senko     (1001)       68 2024-05-16 18:46:58.000000 kiwitcms-github-marketplace-2.6.0/kiwitcms_github_marketplace.egg-info/requires.txt
+-rw-r--r--   0 senko     (1001) senko     (1001)       42 2024-05-16 18:46:58.000000 kiwitcms-github-marketplace-2.6.0/kiwitcms_github_marketplace.egg-info/top_level.txt
+-rw-r--r--   0 senko     (1001) senko     (1001)      133 2024-05-06 12:49:10.000000 kiwitcms-github-marketplace-2.6.0/requirements.txt
+-rw-rw-r--   0 senko     (1001) senko     (1001)      129 2024-05-16 18:46:58.547892 kiwitcms-github-marketplace-2.6.0/setup.cfg
+-rw-r--r--   0 senko     (1001) senko     (1001)     1783 2024-05-16 18:44:54.000000 kiwitcms-github-marketplace-2.6.0/setup.py
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-05-16 18:46:58.545892 kiwitcms-github-marketplace-2.6.0/tcms_github_marketplace/
+-rw-rw-r--   0 senko     (1001) senko     (1001)        0 2021-04-27 19:25:31.000000 kiwitcms-github-marketplace-2.6.0/tcms_github_marketplace/__init__.py
+-rw-r--r--   0 senko     (1001) senko     (1001)     6073 2024-05-07 18:50:52.000000 kiwitcms-github-marketplace-2.6.0/tcms_github_marketplace/admin.py
+-rw-r--r--   0 senko     (1001) senko     (1001)     1607 2024-05-08 20:12:21.000000 kiwitcms-github-marketplace-2.6.0/tcms_github_marketplace/api.py
+-rw-rw-r--   0 senko     (1001) senko     (1001)      321 2022-02-20 13:20:22.000000 kiwitcms-github-marketplace-2.6.0/tcms_github_marketplace/apps.py
+-rw-rw-r--   0 senko     (1001) senko     (1001)      553 2022-02-20 13:20:22.000000 kiwitcms-github-marketplace-2.6.0/tcms_github_marketplace/checks.py
+-rw-r--r--   0 senko     (1001) senko     (1001)     2626 2024-05-09 21:04:00.000000 kiwitcms-github-marketplace-2.6.0/tcms_github_marketplace/docker.py
+-rw-r--r--   0 senko     (1001) senko     (1001)     1508 2024-05-09 21:04:14.000000 kiwitcms-github-marketplace-2.6.0/tcms_github_marketplace/fastspring.py
+-rw-r--r--   0 senko     (1001) senko     (1001)     3563 2024-05-13 10:10:58.000000 kiwitcms-github-marketplace-2.6.0/tcms_github_marketplace/forms.py
+-rw-rw-r--   0 senko     (1001) senko     (1001)      879 2022-02-21 15:47:58.000000 kiwitcms-github-marketplace-2.6.0/tcms_github_marketplace/mailchimp.py
+-rw-rw-r--   0 senko     (1001) senko     (1001)      374 2022-02-09 11:11:58.000000 kiwitcms-github-marketplace-2.6.0/tcms_github_marketplace/menu.py
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-05-16 18:46:58.546892 kiwitcms-github-marketplace-2.6.0/tcms_github_marketplace/migrations/
+-rw-r--r--   0 senko     (1001) senko     (1001)     1532 2024-01-05 12:16:28.000000 kiwitcms-github-marketplace-2.6.0/tcms_github_marketplace/migrations/0001_initial.py
+-rw-r--r--   0 senko     (1001) senko     (1001)      965 2023-04-07 11:54:56.000000 kiwitcms-github-marketplace-2.6.0/tcms_github_marketplace/migrations/0002_update_fields.py
+-rw-r--r--   0 senko     (1001) senko     (1001)      415 2023-04-07 11:54:56.000000 kiwitcms-github-marketplace-2.6.0/tcms_github_marketplace/migrations/0003_sender_email_field.py
+-rw-r--r--   0 senko     (1001) senko     (1001)      391 2023-04-07 11:54:56.000000 kiwitcms-github-marketplace-2.6.0/tcms_github_marketplace/migrations/0004_models_jsonfield.py
+-rw-r--r--   0 senko     (1001) senko     (1001)      613 2023-04-07 11:54:56.000000 kiwitcms-github-marketplace-2.6.0/tcms_github_marketplace/migrations/0005_add_support_and_tenant_flags.py
+-rw-r--r--   0 senko     (1001) senko     (1001)     1039 2023-04-07 11:54:56.000000 kiwitcms-github-marketplace-2.6.0/tcms_github_marketplace/migrations/0006_add_subscription_field.py
+-rw-r--r--   0 senko     (1001) senko     (1001)      694 2023-04-14 16:28:27.000000 kiwitcms-github-marketplace-2.6.0/tcms_github_marketplace/migrations/0007_manualpurchase.py
+-rw-r--r--   0 senko     (1001) senko     (1001)      475 2024-05-07 18:50:52.000000 kiwitcms-github-marketplace-2.6.0/tcms_github_marketplace/migrations/0008_add_gitops_prefix.py
+-rw-rw-r--   0 senko     (1001) senko     (1001)        0 2021-04-27 19:25:31.000000 kiwitcms-github-marketplace-2.6.0/tcms_github_marketplace/migrations/__init__.py
+-rw-r--r--   0 senko     (1001) senko     (1001)     2884 2024-05-07 18:50:52.000000 kiwitcms-github-marketplace-2.6.0/tcms_github_marketplace/models.py
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-05-16 18:46:58.546892 kiwitcms-github-marketplace-2.6.0/tcms_github_marketplace/quay/
+-rw-rw-r--   0 senko     (1001) senko     (1001)       57 2022-02-09 14:16:51.000000 kiwitcms-github-marketplace-2.6.0/tcms_github_marketplace/quay/__init__.py
+-rw-rw-r--   0 senko     (1001) senko     (1001)     2353 2022-02-09 21:44:26.000000 kiwitcms-github-marketplace-2.6.0/tcms_github_marketplace/quay/quay_api_client.py
+-rw-r--r--   0 senko     (1001) senko     (1001)     4708 2024-04-17 13:31:58.000000 kiwitcms-github-marketplace-2.6.0/tcms_github_marketplace/quay/quay_session.py
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-05-16 18:46:58.543892 kiwitcms-github-marketplace-2.6.0/tcms_github_marketplace/static/
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-05-16 18:46:58.543892 kiwitcms-github-marketplace-2.6.0/tcms_github_marketplace/static/tcms_github_marketplace/
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-05-16 18:46:58.546892 kiwitcms-github-marketplace-2.6.0/tcms_github_marketplace/static/tcms_github_marketplace/js/
+-rw-rw-r--   0 senko     (1001) senko     (1001)      924 2022-02-16 15:05:52.000000 kiwitcms-github-marketplace-2.6.0/tcms_github_marketplace/static/tcms_github_marketplace/js/subscription.js
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-05-16 18:46:58.544892 kiwitcms-github-marketplace-2.6.0/tcms_github_marketplace/templates/
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-05-16 18:46:58.546892 kiwitcms-github-marketplace-2.6.0/tcms_github_marketplace/templates/email/
+-rw-r--r--   0 senko     (1001) senko     (1001)     1450 2023-04-14 16:28:27.000000 kiwitcms-github-marketplace-2.6.0/tcms_github_marketplace/templates/email/manual_subscription_notification.txt
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-05-16 18:46:58.546892 kiwitcms-github-marketplace-2.6.0/tcms_github_marketplace/templates/tcms_github_marketplace/
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-05-16 18:46:58.546892 kiwitcms-github-marketplace-2.6.0/tcms_github_marketplace/templates/tcms_github_marketplace/email/
+-rw-rw-r--   0 senko     (1001) senko     (1001)      270 2022-08-14 14:51:18.000000 kiwitcms-github-marketplace-2.6.0/tcms_github_marketplace/templates/tcms_github_marketplace/email/exit_poll.txt
+-rw-r--r--   0 senko     (1001) senko     (1001)    13203 2024-05-11 18:08:16.000000 kiwitcms-github-marketplace-2.6.0/tcms_github_marketplace/templates/tcms_github_marketplace/subscription.html
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-05-16 18:46:58.546892 kiwitcms-github-marketplace-2.6.0/tcms_github_marketplace/templates/tcms_tenants/
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-05-16 18:46:58.546892 kiwitcms-github-marketplace-2.6.0/tcms_github_marketplace/templates/tcms_tenants/include/
+-rw-r--r--   0 senko     (1001) senko     (1001)     1030 2024-05-02 21:53:41.000000 kiwitcms-github-marketplace-2.6.0/tcms_github_marketplace/templates/tcms_tenants/include/tenant_extra_emails.html
+-rw-r--r--   0 senko     (1001) senko     (1001)      163 2024-05-02 21:53:41.000000 kiwitcms-github-marketplace-2.6.0/tcms_github_marketplace/templates/tcms_tenants/override_edit.html
+-rw-r--r--   0 senko     (1001) senko     (1001)     2629 2024-05-02 21:53:41.000000 kiwitcms-github-marketplace-2.6.0/tcms_github_marketplace/templates/tcms_tenants/override_new.html
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-05-16 18:46:58.546892 kiwitcms-github-marketplace-2.6.0/tcms_github_marketplace/templatetags/
+-rw-rw-r--   0 senko     (1001) senko     (1001)        0 2021-04-27 19:25:31.000000 kiwitcms-github-marketplace-2.6.0/tcms_github_marketplace/templatetags/__init__.py
+-rw-rw-r--   0 senko     (1001) senko     (1001)      373 2021-04-27 19:25:31.000000 kiwitcms-github-marketplace-2.6.0/tcms_github_marketplace/templatetags/github_marketplace.py
+-rw-rw-r--   0 senko     (1001) senko     (1001)      804 2022-02-09 11:11:58.000000 kiwitcms-github-marketplace-2.6.0/tcms_github_marketplace/urls.py
+-rw-r--r--   0 senko     (1001) senko     (1001)     5893 2024-05-06 17:00:42.000000 kiwitcms-github-marketplace-2.6.0/tcms_github_marketplace/utils.py
+-rw-r--r--   0 senko     (1001) senko     (1001)    28301 2024-05-13 11:45:48.000000 kiwitcms-github-marketplace-2.6.0/tcms_github_marketplace/views.py
+drwxr-xr-x   0 senko     (1001) senko     (1001)        0 2024-05-16 18:46:58.546892 kiwitcms-github-marketplace-2.6.0/tcms_settings_dir/
+-rw-rw-r--   0 senko     (1001) senko     (1001)       65 2022-02-09 11:11:58.000000 kiwitcms-github-marketplace-2.6.0/tcms_settings_dir/__init__.py
+-rw-r--r--   0 senko     (1001) senko     (1001)      339 2024-05-08 20:12:21.000000 kiwitcms-github-marketplace-2.6.0/tcms_settings_dir/marketplace.py
```

### Comparing `kiwitcms-github-marketplace-2.5.1/LICENSE` & `kiwitcms-github-marketplace-2.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kiwitcms-github-marketplace-2.5.1/PKG-INFO` & `kiwitcms-github-marketplace-2.6.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kiwitcms-github-marketplace
-Version: 2.5.1
+Version: 2.6.0
 Summary: GitHub Marketplace integration for Kiwi TCMS
 Home-page: https://github.com/kiwitcms/github-marketplace/
 Author: Kiwi TCMS
 Author-email: info@kiwitcms.org
 License: GPLv3+
 Classifier: Framework :: Django
 Classifier: Development Status :: 5 - Production/Stable
@@ -58,14 +58,15 @@
 
 
 Configuration
 -------------
 
 Required settings:
 
+- ``KIWI_GITHUB_PAT_FOR_CHECKING_ORGS_AND_USERNAMES`` - string
 - ``KIWI_GITHUB_MARKETPLACE_SECRET`` - binary string
 - ``KIWI_FASTSPRING_SECRET`` - binary string
 - ``QUAY_IO_TOKEN`` - string
 - ``MAILCHIMP_USERNAME`` - string
 - ``MAILCHIMP_SECRET`` - string
 
 Product configuration
@@ -80,14 +81,26 @@
   to private docker repositories. Format is
   ``Docker repositories: quay.io/kiwitcms/<repo1>, quay.io/kiwitcms/<repo2>``
 
 
 Changelog
 ---------
 
+v2.6.0 (16 May 2024)
+~~~~~~~~~~~~~~~~~~~~
+
+- Require a new setting ``KIWI_GITHUB_PAT_FOR_CHECKING_ORGS_AND_USERNAMES``
+- Add ``Purchase.gitops_prefix`` field with a new DB migration
+- Record ``Purchase.gitops_prefix`` upon receiving incoming billing events
+  from GitHub
+- Allow the Subscription page to edit the new ``gitops_prefix`` field
+- Add the ``GitOps.allow()`` API method for usage in ``kiwitcms/gitops``
+- Replace inline style attributes with CSS classes
+
+
 v2.5.1 (06 May 2024)
 ~~~~~~~~~~~~~~~~~~~~
 
 - Adjust name of settings for ``revoke_oauth_token()`` to match production
   environment
 - Adjust arguments for newer versions of PyGithub
```

### Comparing `kiwitcms-github-marketplace-2.5.1/README.rst` & `kiwitcms-github-marketplace-2.6.0/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 
 
 Configuration
 -------------
 
 Required settings:
 
+- ``KIWI_GITHUB_PAT_FOR_CHECKING_ORGS_AND_USERNAMES`` - string
 - ``KIWI_GITHUB_MARKETPLACE_SECRET`` - binary string
 - ``KIWI_FASTSPRING_SECRET`` - binary string
 - ``QUAY_IO_TOKEN`` - string
 - ``MAILCHIMP_USERNAME`` - string
 - ``MAILCHIMP_SECRET`` - string
 
 Product configuration
@@ -59,14 +60,26 @@
   to private docker repositories. Format is
   ``Docker repositories: quay.io/kiwitcms/<repo1>, quay.io/kiwitcms/<repo2>``
 
 
 Changelog
 ---------
 
+v2.6.0 (16 May 2024)
+~~~~~~~~~~~~~~~~~~~~
+
+- Require a new setting ``KIWI_GITHUB_PAT_FOR_CHECKING_ORGS_AND_USERNAMES``
+- Add ``Purchase.gitops_prefix`` field with a new DB migration
+- Record ``Purchase.gitops_prefix`` upon receiving incoming billing events
+  from GitHub
+- Allow the Subscription page to edit the new ``gitops_prefix`` field
+- Add the ``GitOps.allow()`` API method for usage in ``kiwitcms/gitops``
+- Replace inline style attributes with CSS classes
+
+
 v2.5.1 (06 May 2024)
 ~~~~~~~~~~~~~~~~~~~~
 
 - Adjust name of settings for ``revoke_oauth_token()`` to match production
   environment
 - Adjust arguments for newer versions of PyGithub
```

### Comparing `kiwitcms-github-marketplace-2.5.1/kiwitcms_github_marketplace.egg-info/PKG-INFO` & `kiwitcms-github-marketplace-2.6.0/kiwitcms_github_marketplace.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kiwitcms-github-marketplace
-Version: 2.5.1
+Version: 2.6.0
 Summary: GitHub Marketplace integration for Kiwi TCMS
 Home-page: https://github.com/kiwitcms/github-marketplace/
 Author: Kiwi TCMS
 Author-email: info@kiwitcms.org
 License: GPLv3+
 Classifier: Framework :: Django
 Classifier: Development Status :: 5 - Production/Stable
@@ -58,14 +58,15 @@
 
 
 Configuration
 -------------
 
 Required settings:
 
+- ``KIWI_GITHUB_PAT_FOR_CHECKING_ORGS_AND_USERNAMES`` - string
 - ``KIWI_GITHUB_MARKETPLACE_SECRET`` - binary string
 - ``KIWI_FASTSPRING_SECRET`` - binary string
 - ``QUAY_IO_TOKEN`` - string
 - ``MAILCHIMP_USERNAME`` - string
 - ``MAILCHIMP_SECRET`` - string
 
 Product configuration
@@ -80,14 +81,26 @@
   to private docker repositories. Format is
   ``Docker repositories: quay.io/kiwitcms/<repo1>, quay.io/kiwitcms/<repo2>``
 
 
 Changelog
 ---------
 
+v2.6.0 (16 May 2024)
+~~~~~~~~~~~~~~~~~~~~
+
+- Require a new setting ``KIWI_GITHUB_PAT_FOR_CHECKING_ORGS_AND_USERNAMES``
+- Add ``Purchase.gitops_prefix`` field with a new DB migration
+- Record ``Purchase.gitops_prefix`` upon receiving incoming billing events
+  from GitHub
+- Allow the Subscription page to edit the new ``gitops_prefix`` field
+- Add the ``GitOps.allow()`` API method for usage in ``kiwitcms/gitops``
+- Replace inline style attributes with CSS classes
+
+
 v2.5.1 (06 May 2024)
 ~~~~~~~~~~~~~~~~~~~~
 
 - Adjust name of settings for ``revoke_oauth_token()`` to match production
   environment
 - Adjust arguments for newer versions of PyGithub
```

### Comparing `kiwitcms-github-marketplace-2.5.1/kiwitcms_github_marketplace.egg-info/SOURCES.txt` & `kiwitcms-github-marketplace-2.6.0/kiwitcms_github_marketplace.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -9,37 +9,42 @@
 kiwitcms_github_marketplace.egg-info/dependency_links.txt
 kiwitcms_github_marketplace.egg-info/entry_points.txt
 kiwitcms_github_marketplace.egg-info/not-zip-safe
 kiwitcms_github_marketplace.egg-info/requires.txt
 kiwitcms_github_marketplace.egg-info/top_level.txt
 tcms_github_marketplace/__init__.py
 tcms_github_marketplace/admin.py
+tcms_github_marketplace/api.py
 tcms_github_marketplace/apps.py
 tcms_github_marketplace/checks.py
 tcms_github_marketplace/docker.py
+tcms_github_marketplace/fastspring.py
+tcms_github_marketplace/forms.py
 tcms_github_marketplace/mailchimp.py
 tcms_github_marketplace/menu.py
 tcms_github_marketplace/models.py
 tcms_github_marketplace/urls.py
 tcms_github_marketplace/utils.py
 tcms_github_marketplace/views.py
 tcms_github_marketplace/migrations/0001_initial.py
 tcms_github_marketplace/migrations/0002_update_fields.py
 tcms_github_marketplace/migrations/0003_sender_email_field.py
 tcms_github_marketplace/migrations/0004_models_jsonfield.py
 tcms_github_marketplace/migrations/0005_add_support_and_tenant_flags.py
 tcms_github_marketplace/migrations/0006_add_subscription_field.py
 tcms_github_marketplace/migrations/0007_manualpurchase.py
+tcms_github_marketplace/migrations/0008_add_gitops_prefix.py
 tcms_github_marketplace/migrations/__init__.py
 tcms_github_marketplace/quay/__init__.py
 tcms_github_marketplace/quay/quay_api_client.py
 tcms_github_marketplace/quay/quay_session.py
 tcms_github_marketplace/static/tcms_github_marketplace/js/subscription.js
 tcms_github_marketplace/templates/email/manual_subscription_notification.txt
 tcms_github_marketplace/templates/tcms_github_marketplace/subscription.html
 tcms_github_marketplace/templates/tcms_github_marketplace/email/exit_poll.txt
 tcms_github_marketplace/templates/tcms_tenants/override_edit.html
 tcms_github_marketplace/templates/tcms_tenants/override_new.html
 tcms_github_marketplace/templates/tcms_tenants/include/tenant_extra_emails.html
 tcms_github_marketplace/templatetags/__init__.py
 tcms_github_marketplace/templatetags/github_marketplace.py
-tcms_settings_dir/__init__.py
+tcms_settings_dir/__init__.py
+tcms_settings_dir/marketplace.py
```

### Comparing `kiwitcms-github-marketplace-2.5.1/setup.py` & `kiwitcms-github-marketplace-2.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
                 continue
             requires.append(line.strip())
         return requires
 
 
 setup(
     name="kiwitcms-github-marketplace",
-    version="2.5.1",
+    version="2.6.0",
     description="GitHub Marketplace integration for Kiwi TCMS",
     long_description=get_long_description(),
     author="Kiwi TCMS",
     author_email="info@kiwitcms.org",
     url="https://github.com/kiwitcms/github-marketplace/",
     license="GPLv3+",
     install_requires=get_install_requires("requirements.txt"),
```

### Comparing `kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/admin.py` & `kiwitcms-github-marketplace-2.6.0/tcms_github_marketplace/admin.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2019-2023 Alexander Todorov <atodorov@MrSenko.com>
+# Copyright (c) 2019-2024 Alexander Todorov <atodorov@MrSenko.com>
 
 # Licensed under the GPL 3.0: https://www.gnu.org/licenses/gpl-3.0.txt
 
 import json
 
 from django import forms
 from django import http
@@ -23,17 +23,18 @@
         "action",
         "sender",
         "subscription",
         "effective_date",
         "received_on",
         "should_have_tenant",
         "should_have_support",
+        "gitops_prefix",
     )
     list_filter = ("action", "vendor", "sender")
-    search_fields = ("action", "vendor", "sender", "subscription")
+    search_fields = ("action", "vendor", "sender", "subscription", "gitops_prefix")
     ordering = ["-pk"]
 
     def monthly_price(self, purchase):  # pylint: disable=no-self-use
         return int(
             purchase.payload["marketplace_purchase"]["plan"].get(
                 "monthly_price_in_cents", 0
             )
```

### Comparing `kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/checks.py` & `kiwitcms-github-marketplace-2.6.0/tcms_github_marketplace/checks.py`

 * *Files identical despite different names*

### Comparing `kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/docker.py` & `kiwitcms-github-marketplace-2.6.0/tcms_github_marketplace/docker.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2022 Alexander Todorov <atodorov@MrSenko.com>
+# Copyright (c) 2022-2024 Alexander Todorov <atodorov@MrSenko.com>
 
 # Licensed under the GPL 3.0: https://www.gnu.org/licenses/gpl-3.0.txt
 
 from django.conf import settings
 from .quay import QuayApiClient
 
 
@@ -60,16 +60,16 @@
     def _update_token_and_username(self, response=None):
         if not response:
             response = self.api.get_robot_from_organization(
                 self.name, self.organization
             )
 
         if response:
-            self._token = response["token"]
-            self._username = response["name"]
+            self._token = response.get("token")
+            self._username = response.get("name")
 
     def create(self):
         """
         Will create a robot account if it doesn't exist. Will not crash if a
         robot account with this name already exists.
         """
         return self.api.create_robot_in_organization(self.name, self.organization)
```

### Comparing `kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/mailchimp.py` & `kiwitcms-github-marketplace-2.6.0/tcms_github_marketplace/mailchimp.py`

 * *Files identical despite different names*

### Comparing `kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/migrations/0001_initial.py` & `kiwitcms-github-marketplace-2.6.0/tcms_github_marketplace/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/migrations/0002_update_fields.py` & `kiwitcms-github-marketplace-2.6.0/tcms_github_marketplace/migrations/0002_update_fields.py`

 * *Files identical despite different names*

### Comparing `kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/migrations/0005_add_support_and_tenant_flags.py` & `kiwitcms-github-marketplace-2.6.0/tcms_github_marketplace/migrations/0005_add_support_and_tenant_flags.py`

 * *Files identical despite different names*

### Comparing `kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/migrations/0006_add_subscription_field.py` & `kiwitcms-github-marketplace-2.6.0/tcms_github_marketplace/migrations/0006_add_subscription_field.py`

 * *Files identical despite different names*

### Comparing `kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/migrations/0007_manualpurchase.py` & `kiwitcms-github-marketplace-2.6.0/tcms_github_marketplace/migrations/0007_manualpurchase.py`

 * *Files identical despite different names*

### Comparing `kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/models.py` & `kiwitcms-github-marketplace-2.6.0/tcms_github_marketplace/models.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2019-2023 Alexander Todorov <atodorov@MrSenko.com>
+# Copyright (c) 2019-2024 Alexander Todorov <atodorov@MrSenko.com>
 
 # Licensed under the GPL 3.0: https://www.gnu.org/licenses/gpl-3.0.txt
 
 from django.db import models
 from django.contrib.postgres.indexes import GinIndex
 
 
@@ -11,27 +11,62 @@
     A model class without any fields which is needed in order to
     generate an admin page. The admin page will be used to record
     manual purchases which will be processed on the fly and recorded
     inside the standard Purchase model.
     """
 
 
+@models.CharField.register_lookup
+class IPrefixFor(models.lookups.StartsWith):  # pylint: disable=abstract-method
+    """
+    The reverse of ``_startswith``. Selects records where the
+    DB column value acts as a prefix for the supplied lookup argument!
+    https://dba.stackexchange.com/a/149632
+
+    SELECT * FROM my_table WHERE 'value' ILIKE model_field || '%';
+
+
+    .. warning::
+
+        We achieve the results by swapping the left-hand and right-hand side operators
+        for a regular PatternLookup, e.g IStartsWith
+    """
+
+    lookup_name = "iprefix_for"
+    param_pattern = "%s"
+
+    # WARNING: internally process the other side of the expression
+    def process_lhs(self, compiler, connection, lhs=None):
+        return super().process_rhs(compiler, connection)
+
+    # WARNING: internally process the other side of the expression
+    def process_rhs(self, qn, connection):
+        return super().process_lhs(qn, connection)
+
+    def get_rhs_op(self, connection, rhs):
+        # WARNING: Postgresql specific
+        return f"ILIKE {rhs}::text || '%%'"
+
+
 class Purchase(models.Model):
     """
     Holds information about GitHub ``marketplace_purchase`` events:
     https://developer.github.com/marketplace/integrating-with-the-github-marketplace-api/github-marketplace-webhook-events/
     """
 
     vendor = models.CharField(max_length=16, db_index=True, blank=True, null=True)
     action = models.CharField(max_length=64, db_index=True)
     sender = models.EmailField(db_index=True)
     subscription = models.CharField(max_length=32, db_index=True, blank=True, null=True)
     effective_date = models.DateTimeField(db_index=True)
     should_have_tenant = models.BooleanField(default=False, db_index=True)
     should_have_support = models.BooleanField(default=False, db_index=True)
+    gitops_prefix = models.CharField(
+        null=True, blank=True, db_index=True, max_length=256
+    )
 
     # this is for internal purposes
     received_on = models.DateTimeField(db_index=True, auto_now_add=True)
 
     payload = models.JSONField()
 
     class Meta:
```

### Comparing `kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/quay/quay_api_client.py` & `kiwitcms-github-marketplace-2.6.0/tcms_github_marketplace/quay/quay_api_client.py`

 * *Files identical despite different names*

### Comparing `kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/quay/quay_session.py` & `kiwitcms-github-marketplace-2.6.0/tcms_github_marketplace/quay/quay_session.py`

 * *Files identical despite different names*

### Comparing `kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/static/tcms_github_marketplace/js/subscription.js` & `kiwitcms-github-marketplace-2.6.0/tcms_github_marketplace/static/tcms_github_marketplace/js/subscription.js`

 * *Files identical despite different names*

### Comparing `kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/templates/email/manual_subscription_notification.txt` & `kiwitcms-github-marketplace-2.6.0/tcms_github_marketplace/templates/email/manual_subscription_notification.txt`

 * *Files identical despite different names*

### Comparing `kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/templates/tcms_github_marketplace/subscription.html` & `kiwitcms-github-marketplace-2.6.0/tcms_github_marketplace/templates/tcms_github_marketplace/subscription.html`

 * *Files 14% similar despite different names*

```diff
@@ -7,68 +7,109 @@
 
 {% block contents %}
 
 <div class="container-fluid container-cards-pf">
     <div class="row row-cards-pf">
         <div class="col-xs-12 col-sm-12 col-md-6">
             <div class="card-pf card-pf-accented card-pf-aggregate-status">
-                <h2 class="card-pf-title" style="text-align: left">
+                <h2 class="card-pf-title kiwi-text-align-left">
                     {% trans "You can access the following tenants" %}
                 </h2>
 
             {% for tenant in access_tenants %}
-                <h2 class="card-pf-title" style="text-align: left">
+                <h2 class="card-pf-title kiwi-text-align-left">
                     <span class="pficon pficon-tenant"></span>{% trans 'Tenant' %}:
                     <a href="{% tenant_url request tenant.schema_name %}">{% tenant_url request tenant.schema_name %}</a>
                 </h2>
 
-                <h2 class="card-pf-title" style="text-align: left">
+                <h2 class="card-pf-title kiwi-text-align-left">
                     <span class="pficon pficon-user"></span>{% trans 'Owner' %}:
                     <a href="{% url "tcms-profile" tenant.owner.username %}">{{ tenant.owner }}</a>
                 </h2>
 
                 {% if tenant.organization %}
-                <h2 class="card-pf-title" style="text-align: left">
+                <h2 class="card-pf-title kiwi-text-align-left">
                     <span class="pficon pficon-users"></span>{% trans 'Organization' %}:
                     {{ tenant.organization }}
                 </h2>
                 {% endif %}
             {% endfor %}
 
                 <div class="card-pf-body"></div>
             </div>
         </div>
 
         <div class="col-xs-12 col-sm-12 col-md-6">
             <div class="card-pf card-pf-accented card-pf-aggregate-status">
-                <h2 class="card-pf-title" style="text-align: left">
+                <h2 class="card-pf-title kiwi-text-align-left">
                     {% trans 'Docker credentials' %}
                 </h2>
 
-                <div class="card-pf-body" style="text-align: left">
+                <div class="card-pf-body kiwi-text-align-left">
                     <div class="input-group">
                         <span class="input-group-addon">{% trans 'Username' %} </span>
                         <input type="text" id="docker_username" value="{{ quay_io_account.username }}" class="form-control" disabled>
                     </div>
 
                     <div class="input-group">
-                        <span class="input-group-addon" style="cursor: pointer" id="show-docker-password">{% trans 'Password' %}</span>
+                        <span class="input-group-addon kiwi-cursor-pointer" id="show-docker-password">{% trans 'Password' %}</span>
                         <input type="password" id="docker_password" value="{{ quay_io_account.token }}" class="form-control" disabled>
                     </div>
 
                     <p class="help-block">
-                        <span class="fa fa-exclamation-triangle" style="color: #ec7a08;"></span>
+                        <span class="fa fa-exclamation-triangle kiwi-color-warning"></span>
                         <span class="fa fa-sign-in" aria-hidden="true"></span>
                         {% trans 'Private containers instructions' %}:
                         <a href="https://kiwitcms.org/containers/">https://kiwitcms.org/containers/</a>
                     </p>
                 </div>
             </div>
         </div>
 
+        {% if object %}
+        <div class="col-xs-12 col-sm-12 col-md-6">
+            <div class="card-pf card-pf-accented card-pf-aggregate-status">
+                <h2 class="card-pf-title kiwi-text-align-left">
+                    {% trans 'kiwitcms/gitops prefix' %}
+                </h2>
+
+                <div class="card-pf-body kiwi-text-align-left">
+                    <form class="form-horizontal" method="post" action="{% url 'github_marketplace_plans' %}">
+                        <div class="form-group">
+                            <div class="col-xs-10 col-sm-10 col-md-10 col-lg-10 {% if form.gitops_prefix.errors %}has-error{% endif %} kiwi-padding-right-0">
+                                <input type="text" name="gitops_prefix"
+                                    value="{{ form.gitops_prefix.value|default:'' }}"
+                                    class="form-control" required
+                                    maxlength="{{ form.fields.gitops_prefix.max_length }}"
+                                    placeholder="https://github.com/your-account-or-organization"
+                                    {% if object.gitops_prefix %}disabled{% endif %}
+                                >
+
+                                {{ form.gitops_prefix.errors }}
+                            </div>
+
+                        {% if not object.gitops_prefix %}
+                            {% csrf_token %}
+                            <div class="col-xs-1 col-sm-1 col-md-1 col-lg-1 kiwi-padding-left-0">
+                                <button type="submit" class="btn btn-default btn-md">{% trans "Save" %}</button>
+                            </div>
+                        {% endif %}
+                        </div>
+
+                        <p class="help-block">
+                            <span class="fa fa-exclamation-triangle kiwi-color-warning"></span>
+                            <span class="fa fa-sign-in" aria-hidden="true"></span>
+                            <a href="https://kiwitcms.org/gitops/">https://kiwitcms.org/gitops/</a>
+                        </p>
+                    </form>
+                </div>
+            </div>
+        </div>
+        {% endif %}
+
     </div>
 
     <div class="row row-cards-pf">
         <div class="col-xs-12 col-sm-12 col-md-12">
             <div class="card-pf card-pf-accented">
                 <h2 class="card-pf-title">
                     <span class="pficon pficon-topology"></span>
```

#### html2text {}

```diff
@@ -8,14 +8,23 @@
 {% if tenant.organization %}
 ********** {{%% ttrraannss ''OOrrggaanniizzaattiioonn'' %%}}:: {{{{ tteennaanntt..oorrggaanniizzaattiioonn }}}} **********
 {% endif %} {% endfor %}
 ********** {{%% ttrraannss ''DDoocckkeerr ccrreeddeennttiiaallss'' %%}} **********
 {% trans 'Username' %}[{{ quay_io_account.username }}]
 {% trans 'Password' %}[********************]
 {% trans 'Private containers instructions' %}: _h_t_t_p_s_:_/_/_k_i_w_i_t_c_m_s_._o_r_g_/_c_o_n_t_a_i_n_e_r_s_/
+{% if object %}
+********** {{%% ttrraannss ''kkiiwwiittccmmss//ggiittooppss pprreeffiixx'' %%}} **********
+% if object.gitops_prefix %}disabled{% endif %} > {{ form.gitops_prefix.errors
+}}
+{% if not object.gitops_prefix %} {% csrf_token %}
+{% trans "Save" %}
+{% endif %}
+_h_t_t_p_s_:_/_/_k_i_w_i_t_c_m_s_._o_r_g_/_g_i_t_o_p_s_/
+{% endif %}
 ********** {{%% ttrraannss ''YYoouu oowwnn tthhee ffoolllloowwiinngg tteennaannttss'' %%}} **********
 {% for tenant in own_tenants %}
 _{_%_ _t_e_n_a_n_t___u_r_l_ _r_e_q_u_e_s_t_ _t_e_n_a_n_t_._s_c_h_e_m_a___n_a_m_e_ _%_} {% if tenant.organization %} {%
 trans 'Organization' %}: {{ tenant.organization }} {% endif %}
 {{{{ ssuubbssccrriippttiioonn__pprriiccee }}}} // {{{{ ssuubbssccrriippttiioonn__ppeerriioodd }}}}
 PPrriivvaattee TTeennaanntt
 {{{{ tteennaanntt..ppaaiidd__uunnttiill }}}}
```

### Comparing `kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/templates/tcms_tenants/include/tenant_extra_emails.html` & `kiwitcms-github-marketplace-2.6.0/tcms_github_marketplace/templates/tcms_tenants/include/tenant_extra_emails.html`

 * *Files identical despite different names*

### Comparing `kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/templates/tcms_tenants/override_new.html` & `kiwitcms-github-marketplace-2.6.0/tcms_github_marketplace/templates/tcms_tenants/override_new.html`

 * *Files identical despite different names*

### Comparing `kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/urls.py` & `kiwitcms-github-marketplace-2.6.0/tcms_github_marketplace/urls.py`

 * *Files identical despite different names*

### Comparing `kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/utils.py` & `kiwitcms-github-marketplace-2.6.0/tcms_github_marketplace/utils.py`

 * *Files identical despite different names*

### Comparing `kiwitcms-github-marketplace-2.5.1/tcms_github_marketplace/views.py` & `kiwitcms-github-marketplace-2.6.0/tcms_github_marketplace/views.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,31 +6,35 @@
 
 import json
 import os
 from datetime import datetime
 
 from django.db.models import Q
 from django.conf import settings
-from django.urls import reverse
+from django.core.cache import cache
+from django.urls import reverse, reverse_lazy
 from django.http import HttpResponse, HttpResponseRedirect
 from django.views.decorators.csrf import csrf_exempt
-from django.views.generic.base import View, TemplateView
+from django.views.generic.base import View
+from django.views.generic.edit import UpdateView
 from django.utils.decorators import method_decorator
 from django.utils.translation import gettext_lazy as _
 from django.contrib.auth.decorators import login_required
 
 from tcms.core.utils.mailto import mailto
 from tcms.utils import github
 
 from django_tenants.utils import get_public_schema_name
 from tcms_tenants.models import Tenant
 from tcms_tenants.views import NewTenantView
 from tcms_tenants import utils as tcms_tenants_utils
 
 from tcms_github_marketplace import docker
+from tcms_github_marketplace import fastspring
+from tcms_github_marketplace import forms
 from tcms_github_marketplace import mailchimp
 from tcms_github_marketplace import utils
 from tcms_github_marketplace.models import Purchase
 
 
 class GenericPurchaseNotificationView(View):
     """
@@ -72,25 +76,34 @@
 
     def purchase_action(self, event):
         raise NotImplementedError
 
     def purchase_effective_date(self, event):
         raise NotImplementedError
 
+    def purchase_gitops_prefix(self, event):  # pylint: disable=unused-argument
+        return None
+
     def purchase_sender(self, event):
         raise NotImplementedError
 
     def purchase_should_have_tenant(self, event):
         raise NotImplementedError
 
     def purchase_subscription(self, event):  # pylint: disable=unused-argument
         return None
 
     def record_purchase(self, **kwargs):
-        return Purchase.objects.create(**kwargs)
+        purchase = Purchase.objects.create(**kwargs)
+
+        # remove possible stale state
+        if purchase.gitops_prefix:
+            cache.clear()
+
+        return purchase
 
     def request_verify_signature(self, request):
         raise NotImplementedError
 
     def vendor_pre_process_payload(self, payload):  # pylint: disable=unused-argument
         """
         Perform any vendor specific pre-processing of payload before beginning
@@ -137,14 +150,15 @@
                 action=self.purchase_action(event),
                 effective_date=self.purchase_effective_date(event),
                 payload=event,
                 sender=self.purchase_sender(event),
                 should_have_tenant=self.purchase_should_have_tenant(event),
                 subscription=self.purchase_subscription(event),
                 vendor=self.purchase_vendor,
+                gitops_prefix=self.purchase_gitops_prefix(event),
             )
 
             if self.action_is_cancelled(purchase):
                 return utils.cancel_plan(purchase)
 
             if self.action_is_activated(purchase) and not os.environ.get(
                 "SKIP_QUAY_IO", False
@@ -234,14 +248,20 @@
     def purchase_action(self, event):
         return event["action"]
 
     def purchase_effective_date(self, event):
         # format is 2017-10-25T00:00:00+00:00
         return datetime.strptime(event["effective_date"][:19], "%Y-%m-%dT%H:%M:%S")
 
+    def purchase_gitops_prefix(self, event):
+        # Note: works for both organizations and users
+        login = event["marketplace_purchase"]["account"]["login"]
+
+        return f"https://github.com/{login}"
+
     def purchase_sender(self, event):
         return event["sender"]["email"]
 
     def purchase_should_have_tenant(self, event):
         """
         https://github.com/marketplace/kiwi-tcms/ doesn't list the full range of products.
         The products currently available are:
@@ -312,58 +332,15 @@
         return query.filter(
             Q(owner__email__in=all_senders)
             | Q(owner__username__in=all_senders)
             | Q(extra_emails__icontains=purchase.sender),
         )
 
     def find_sku(self, purchase):
-        """
-        SKU can be found in several different places
-        """
-        # this method is also called from purchase_should_have_tenant() which
-        # only passes event JSON b/c the Purchase object hasn't been created yet
-        event = purchase
-        if isinstance(purchase, Purchase):
-            event = purchase.payload
-        assert isinstance(event, dict)
-
-        # begin looking for SKU
-        if "sku" in event["data"] and event["data"]["sku"]:
-            return event["data"]["sku"]
-
-        if (
-            "product" in event["data"]
-            and "sku" in event["data"]["product"]
-            and event["data"]["product"]["sku"]
-        ):
-            return event["data"]["product"]["sku"]
-
-        if (
-            "subscription" in event["data"]
-            and "sku" in event["data"]["subscription"]
-            and event["data"]["subscription"]["sku"]
-        ):
-            return event["data"]["subscription"]["sku"]
-
-        sku = ""
-        if "items" in event["data"]:
-            for item in event["data"]["items"]:
-                if "sku" in item:
-                    sku += item["sku"] or ""
-
-            if sku:
-                return sku
-
-        if "kiwitcms-private-tenant" in json.dumps(event):
-            sku = "x-tenant+version"
-
-        if "kiwitcms-enterprise" in json.dumps(event):
-            sku = "x-tenant+version+enterprise"
-
-        return sku
+        return fastspring.find_sku(purchase)
 
     def purchase_action(self, event):
         # Adjust to GitHub's format b/c we have legacy records in the DB
         if event["type"] in ["subscription.activated", "subscription.charge.completed"]:
             return "purchased"
 
         if event["type"] == "subscription.deactivated":
@@ -712,61 +689,84 @@
     def get_context_data(self, **kwargs):
         context = super().get_context_data(**kwargs)
         context["form_action_url"] = reverse("github_marketplace_create_tenant")
         return context
 
 
 @method_decorator(login_required, name="dispatch")
-class ViewSubscriptionPlan(TemplateView):
+class ViewSubscriptionPlan(UpdateView):
     """
-    This view shows information about current subscription plan.
+    This view shows information about current subscription plan and allows
+    user to edit Purchase.gitops_prefix field if not set!
     """
 
+    model = Purchase
+    form_class = forms.UpdateGitopsPrefixForm
+    success_url = reverse_lazy("github_marketplace_plans")
     template_name = "tcms_github_marketplace/subscription.html"
 
-    def get_context_data(self, **kwargs):
-        own_tenants = Tenant.objects.filter(owner=self.request.user)
-        purchases = Purchase.objects.filter(
+    def form_valid(self, form):
+        # clear gitops_prefix cache!
+        cache.clear()
+
+        return super().form_valid(form)
+
+    def get_queryset(self):
+        """
+        All purchases for the currently logged-in user
+        """
+        return Purchase.objects.filter(
             sender=self.request.user.email,
         ).order_by("-received_on")
 
-        mp_purchase = purchases.first()
+    def get_object(self, queryset=None):
+        """
+        Always returns the latest purchase for the current user
+        """
+        return self.get_queryset().first()
+
+    def get_context_data(self, **kwargs):
+        context = super().get_context_data(**kwargs)
 
         cancel_url = None
         quay_io_account = None
 
         subscription_price = "-"
         subscription_period = "-"
 
-        if mp_purchase is not None:
+        if self.object is not None:
             subscription_price = "0"
-            quay_io_account = docker.QuayIOAccount(mp_purchase.sender)
+            quay_io_account = docker.QuayIOAccount(self.object.sender)
 
-            if mp_purchase.vendor.lower() == "github":
+            if self.object.vendor.lower() == "github":
                 cancel_url = "https://github.com/settings/billing"
 
-            if mp_purchase.vendor.lower() == "fastspring":
-                cancel_url = mp_purchase.payload["data"]["account"]["url"]
+            if self.object.vendor.lower() == "fastspring":
+                cancel_url = self.object.payload["data"]["account"]["url"]
 
-            mp_purchase = mp_purchase.payload["marketplace_purchase"]
-            if mp_purchase["billing_cycle"] == "monthly":
+            purchase_data = self.object.payload["marketplace_purchase"]
+            if purchase_data["billing_cycle"] == "monthly":
                 subscription_price = (
-                    mp_purchase["plan"]["monthly_price_in_cents"] // 100
+                    purchase_data["plan"]["monthly_price_in_cents"] // 100
                 )
                 subscription_period = _("mo")
-            elif mp_purchase["billing_cycle"] == "yearly":
-                subscription_price = mp_purchase["plan"]["yearly_price_in_cents"] // 100
+            elif purchase_data["billing_cycle"] == "yearly":
+                subscription_price = (
+                    purchase_data["plan"]["yearly_price_in_cents"] // 100
+                )
                 subscription_period = _("yr")
 
             subscription_price = int(subscription_price)
 
-        context = {
-            "access_tenants": self.request.user.tenant_set.all(),
-            "own_tenants": own_tenants,
-            "purchases": purchases,
-            "subscription_price": subscription_price,
-            "subscription_period": subscription_period,
-            "cancel_url": cancel_url,
-            "quay_io_account": quay_io_account,
-        }
+        context.update(
+            {
+                "access_tenants": self.request.user.tenant_set.all(),
+                "own_tenants": Tenant.objects.filter(owner=self.request.user),
+                "purchases": self.get_queryset(),
+                "subscription_price": subscription_price,
+                "subscription_period": subscription_period,
+                "cancel_url": cancel_url,
+                "quay_io_account": quay_io_account,
+            }
+        )
 
         return context
```

