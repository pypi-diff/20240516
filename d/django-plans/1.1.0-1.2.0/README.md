# Comparing `tmp/django-plans-1.1.0.tar.gz` & `tmp/django-plans-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-plans-1.1.0.tar", last modified: Fri Apr 12 12:33:50 2024, max compression
+gzip compressed data, was "django-plans-1.2.0.tar", last modified: Thu May 16 13:38:01 2024, max compression
```

## Comparing `django-plans-1.1.0.tar` & `django-plans-1.2.0.tar`

### file list

```diff
@@ -1,288 +1,288 @@
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.937353 django-plans-1.1.0/
--rw-rw-r--   0 petr      (1000) petr      (1000)      653 2024-04-12 12:33:50.000000 django-plans-1.1.0/.coveragerc
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.909355 django-plans-1.1.0/.github/
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.913355 django-plans-1.1.0/.github/workflows/
--rw-rw-r--   0 petr      (1000) petr      (1000)     4394 2024-04-12 12:33:50.000000 django-plans-1.1.0/.github/workflows/main.yml
--rw-rw-r--   0 petr      (1000) petr      (1000)      343 2024-04-12 12:33:50.000000 django-plans-1.1.0/.gitignore
--rw-rw-r--   0 petr      (1000) petr      (1000)      616 2024-04-12 12:33:50.000000 django-plans-1.1.0/.travis.yml
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.913355 django-plans-1.1.0/.tx/
--rw-rw-r--   0 petr      (1000) petr      (1000)      396 2024-04-12 12:33:50.000000 django-plans-1.1.0/.tx/config
--rw-rw-r--   0 petr      (1000) petr      (1000)       83 2024-04-12 12:33:50.000000 django-plans-1.1.0/AUTHORS
--rw-rw-r--   0 petr      (1000) petr      (1000)     6906 2024-04-12 12:33:50.000000 django-plans-1.1.0/CHANGELOG
--rw-rw-r--   0 petr      (1000) petr      (1000)     3215 2024-04-12 12:33:50.000000 django-plans-1.1.0/CODE_OF_CONDUCT.md
--rw-rw-r--   0 petr      (1000) petr      (1000)     1060 2024-04-12 12:33:50.000000 django-plans-1.1.0/LICENSE
--rw-rw-r--   0 petr      (1000) petr      (1000)      188 2024-04-12 12:33:50.000000 django-plans-1.1.0/MANIFEST.in
--rw-r--r--   0 petr      (1000) petr      (1000)     2054 2024-04-12 12:33:50.937353 django-plans-1.1.0/PKG-INFO
--rw-rw-r--   0 petr      (1000) petr      (1000)     1061 2024-04-12 12:33:50.000000 django-plans-1.1.0/README.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     1617 2024-04-12 12:33:50.000000 django-plans-1.1.0/conftest.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.913355 django-plans-1.1.0/demo/
--rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/__init__.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.917354 django-plans-1.1.0/demo/example/
--rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/__init__.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.917354 django-plans-1.1.0/demo/example/foo/
--rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/foo/__init__.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.917354 django-plans-1.1.0/demo/example/foo/fixtures/
--rw-rw-r--   0 petr      (1000) petr      (1000)     7641 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/foo/fixtures/initial_data.json
--rw-rw-r--   0 petr      (1000) petr      (1000)      428 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/foo/forms.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.917354 django-plans-1.1.0/demo/example/foo/migrations/
--rw-rw-r--   0 petr      (1000) petr      (1000)     1128 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/foo/migrations/0001_initial.py
--rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/foo/migrations/__init__.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      279 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/foo/models.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.909355 django-plans-1.1.0/demo/example/foo/templates/
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.917354 django-plans-1.1.0/demo/example/foo/templates/foo/
--rw-rw-r--   0 petr      (1000) petr      (1000)      591 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/foo/templates/foo/foo_confirm_delete.html
--rw-rw-r--   0 petr      (1000) petr      (1000)      650 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/foo/templates/foo/foo_form.html
--rw-rw-r--   0 petr      (1000) petr      (1000)     1044 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/foo/templates/foo/foo_list.html
--rw-rw-r--   0 petr      (1000) petr      (1000)      383 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/foo/tests.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      402 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/foo/urls.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      323 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/foo/validators.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     1530 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/foo/views.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.909355 django-plans-1.1.0/demo/example/locale/
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.909355 django-plans-1.1.0/demo/example/locale/en/
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.917354 django-plans-1.1.0/demo/example/locale/en/LC_MESSAGES/
--rw-rw-r--   0 petr      (1000) petr      (1000)      378 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/locale/en/LC_MESSAGES/django.mo
--rw-rw-r--   0 petr      (1000) petr      (1000)      714 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/locale/en/LC_MESSAGES/django.po
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.909355 django-plans-1.1.0/demo/example/locale/pl/
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.917354 django-plans-1.1.0/demo/example/locale/pl/LC_MESSAGES/
--rw-rw-r--   0 petr      (1000) petr      (1000)      603 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/locale/pl/LC_MESSAGES/django.mo
--rw-rw-r--   0 petr      (1000) petr      (1000)      904 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/locale/pl/LC_MESSAGES/django.po
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.909355 django-plans-1.1.0/demo/example/locale/pt_BR/
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.917354 django-plans-1.1.0/demo/example/locale/pt_BR/LC_MESSAGES/
--rw-rw-r--   0 petr      (1000) petr      (1000)      495 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/locale/pt_BR/LC_MESSAGES/django.mo
--rw-rw-r--   0 petr      (1000) petr      (1000)      804 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/locale/pt_BR/LC_MESSAGES/django.po
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.909355 django-plans-1.1.0/demo/example/locale/ru/
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.917354 django-plans-1.1.0/demo/example/locale/ru/LC_MESSAGES/
--rw-rw-r--   0 petr      (1000) petr      (1000)      549 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/locale/ru/LC_MESSAGES/django.mo
--rw-rw-r--   0 petr      (1000) petr      (1000)      858 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/locale/ru/LC_MESSAGES/django.po
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.917354 django-plans-1.1.0/demo/example/sample_plans/
--rw-rw-r--   0 petr      (1000) petr      (1000)      160 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/sample_plans/__init__.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      233 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/sample_plans/admin.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      190 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/sample_plans/apps.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.917354 django-plans-1.1.0/demo/example/sample_plans/fixtures/
--rw-rw-r--   0 petr      (1000) petr      (1000)      693 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/sample_plans/fixtures/initial_plan.json
--rw-rw-r--   0 petr      (1000) petr      (1000)     1187 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/sample_plans/fixtures/test_django-plans_auth.json
--rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/sample_plans/fixtures/test_django-plans_default_plans.json
--rw-rw-r--   0 petr      (1000) petr      (1000)     9864 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/sample_plans/fixtures/test_django-plans_plans.json
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.917354 django-plans-1.1.0/demo/example/sample_plans/management/
--rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/sample_plans/management/__init__.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.917354 django-plans-1.1.0/demo/example/sample_plans/management/commands/
--rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/sample_plans/management/commands/__init__.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      119 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/sample_plans/management/commands/autorenew_accounts.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      117 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/sample_plans/management/commands/create_userplans.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      116 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/sample_plans/management/commands/expire_accounts.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.921354 django-plans-1.1.0/demo/example/sample_plans/migrations/
--rw-rw-r--   0 petr      (1000) petr      (1000)    31516 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/sample_plans/migrations/0001_initial.py
--rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/sample_plans/migrations/__init__.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     1960 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/sample_plans/models.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.909355 django-plans-1.1.0/demo/example/sample_plans/templates/
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.921354 django-plans-1.1.0/demo/example/sample_plans/templates/mail/
--rw-rw-r--   0 petr      (1000) petr      (1000)      533 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/sample_plans/templates/mail/change_plan_body.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)      127 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/sample_plans/templates/mail/change_plan_title.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)      573 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/sample_plans/templates/mail/expired_account_body.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)       90 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/sample_plans/templates/mail/expired_account_title.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)      536 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/sample_plans/templates/mail/extend_account_body.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)      145 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/sample_plans/templates/mail/extend_account_title.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)      511 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/sample_plans/templates/mail/invoice_created_body.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)      225 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/sample_plans/templates/mail/invoice_created_title.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)      590 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/sample_plans/templates/mail/remind_expire_body.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)      188 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/sample_plans/templates/mail/remind_expire_title.txt
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.921354 django-plans-1.1.0/demo/example/sample_plans/templates/plans/
--rw-rw-r--   0 petr      (1000) petr      (1000)      668 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/sample_plans/templates/plans/account_activation.html
--rw-rw-r--   0 petr      (1000) petr      (1000)      305 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/sample_plans/templates/plans/base.html
--rw-rw-r--   0 petr      (1000) petr      (1000)      653 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/sample_plans/templates/plans/billing_info_create.html
--rw-rw-r--   0 petr      (1000) petr      (1000)      835 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/sample_plans/templates/plans/billing_info_create_or_update.html
--rw-rw-r--   0 petr      (1000) petr      (1000)      429 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/sample_plans/templates/plans/billing_info_delete.html
--rw-rw-r--   0 petr      (1000) petr      (1000)      744 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/sample_plans/templates/plans/billing_info_update.html
--rw-rw-r--   0 petr      (1000) petr      (1000)     2811 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/sample_plans/templates/plans/create_order.html
--rw-rw-r--   0 petr      (1000) petr      (1000)     1135 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/sample_plans/templates/plans/current.html
--rw-rw-r--   0 petr      (1000) petr      (1000)     1068 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/sample_plans/templates/plans/expiration_messages.html
--rw-rw-r--   0 petr      (1000) petr      (1000)     1992 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/sample_plans/templates/plans/extend.html
--rw-rw-r--   0 petr      (1000) petr      (1000)      396 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/sample_plans/templates/plans/fake_payments.html
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.921354 django-plans-1.1.0/demo/example/sample_plans/templates/plans/invoices/
--rw-rw-r--   0 petr      (1000) petr      (1000)      186 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/sample_plans/templates/plans/invoices/PL_EN.html
--rw-rw-r--   0 petr      (1000) petr      (1000)     8160 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/sample_plans/templates/plans/invoices/PL_EN_layout.html
--rw-rw-r--   0 petr      (1000) petr      (1000)     1729 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/sample_plans/templates/plans/invoices/invoice_base.html
--rw-rw-r--   0 petr      (1000) petr      (1000)     3358 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/sample_plans/templates/plans/order_detail.html
--rw-rw-r--   0 petr      (1000) petr      (1000)     1258 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/sample_plans/templates/plans/order_detail_table.html
--rw-rw-r--   0 petr      (1000) petr      (1000)     2046 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/sample_plans/templates/plans/order_list.html
--rw-rw-r--   0 petr      (1000) petr      (1000)      846 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/sample_plans/templates/plans/pagination.html
--rw-rw-r--   0 petr      (1000) petr      (1000)     5465 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/sample_plans/templates/plans/plan_table.html
--rw-rw-r--   0 petr      (1000) petr      (1000)      176 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/sample_plans/templates/plans/pricing.html
--rw-rw-r--   0 petr      (1000) petr      (1000)      162 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/sample_plans/templates/plans/upgrade.html
--rw-rw-r--   0 petr      (1000) petr      (1000)     2239 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/sample_plans/tests.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     5544 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/settings.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.909355 django-plans-1.1.0/demo/example/static/
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.921354 django-plans-1.1.0/demo/example/static/css/
--rw-rw-r--   0 petr      (1000) petr      (1000)     3961 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/static/css/example.css
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.909355 django-plans-1.1.0/demo/example/static/img/
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.921354 django-plans-1.1.0/demo/example/static/img/messages/
--rw-rw-r--   0 petr      (1000) petr      (1000)      294 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/static/img/messages/icon_alert.png
--rw-rw-r--   0 petr      (1000) petr      (1000)     3668 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/static/img/messages/icon_error.png
--rw-rw-r--   0 petr      (1000) petr      (1000)     3675 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/static/img/messages/icon_success.png
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.925354 django-plans-1.1.0/demo/example/templates/
--rw-rw-r--   0 petr      (1000) petr      (1000)     2746 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/templates/base.html
--rw-rw-r--   0 petr      (1000) petr      (1000)      823 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/templates/home.html
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.925354 django-plans-1.1.0/demo/example/templates/plans/
--rw-rw-r--   0 petr      (1000) petr      (1000)       25 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/templates/plans/base.html
--rw-rw-r--   0 petr      (1000) petr      (1000)      757 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/templates/plans/billing_info_create.html
--rw-rw-r--   0 petr      (1000) petr      (1000)      882 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/templates/plans/billing_info_update.html
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.925354 django-plans-1.1.0/demo/example/templates/registration/
--rw-rw-r--   0 petr      (1000) petr      (1000)      718 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/templates/registration/login.html
--rw-rw-r--   0 petr      (1000) petr      (1000)      605 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/urls.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     1132 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/example/wsgi.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      323 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/fabfile.py
--rwxrwxr-x   0 petr      (1000) petr      (1000)      813 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/manage.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      428 2024-04-12 12:33:50.000000 django-plans-1.1.0/demo/requirements.txt
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.937353 django-plans-1.1.0/django_plans.egg-info/
--rw-r--r--   0 petr      (1000) petr      (1000)     2054 2024-04-12 12:33:50.000000 django-plans-1.1.0/django_plans.egg-info/PKG-INFO
--rw-rw-r--   0 petr      (1000) petr      (1000)     8584 2024-04-12 12:33:50.000000 django-plans-1.1.0/django_plans.egg-info/SOURCES.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)        1 2024-04-12 12:33:50.000000 django-plans-1.1.0/django_plans.egg-info/dependency_links.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)        1 2024-04-12 12:33:50.000000 django-plans-1.1.0/django_plans.egg-info/not-zip-safe
--rw-rw-r--   0 petr      (1000) petr      (1000)      186 2024-04-12 12:33:50.000000 django-plans-1.1.0/django_plans.egg-info/requires.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)       22 2024-04-12 12:33:50.000000 django-plans-1.1.0/django_plans.egg-info/top_level.txt
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.925354 django-plans-1.1.0/docs/
--rw-rw-r--   0 petr      (1000) petr      (1000)     5597 2024-04-12 12:33:50.000000 django-plans-1.1.0/docs/Makefile
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.925354 django-plans-1.1.0/docs/source/
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.909355 django-plans-1.1.0/docs/source/_static/
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.925354 django-plans-1.1.0/docs/source/_static/images/
--rw-rw-r--   0 petr      (1000) petr      (1000)   176623 2024-04-12 12:33:50.000000 django-plans-1.1.0/docs/source/_static/images/django-plans-1.png
--rw-rw-r--   0 petr      (1000) petr      (1000)   193693 2024-04-12 12:33:50.000000 django-plans-1.1.0/docs/source/_static/images/django-plans-2.png
--rw-rw-r--   0 petr      (1000) petr      (1000)   146667 2024-04-12 12:33:50.000000 django-plans-1.1.0/docs/source/_static/images/django-plans-3.png
--rw-rw-r--   0 petr      (1000) petr      (1000)      860 2024-04-12 12:33:50.000000 django-plans-1.1.0/docs/source/caveats.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     8032 2024-04-12 12:33:50.000000 django-plans-1.1.0/docs/source/conf.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     1217 2024-04-12 12:33:50.000000 django-plans-1.1.0/docs/source/customize_models.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     1703 2024-04-12 12:33:50.000000 django-plans-1.1.0/docs/source/index.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     2316 2024-04-12 12:33:50.000000 django-plans-1.1.0/docs/source/installation.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     1966 2024-04-12 12:33:50.000000 django-plans-1.1.0/docs/source/integration.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     2588 2024-04-12 12:33:50.000000 django-plans-1.1.0/docs/source/invoicing.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     6661 2024-04-12 12:33:50.000000 django-plans-1.1.0/docs/source/plans.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     1024 2024-04-12 12:33:50.000000 django-plans-1.1.0/docs/source/plans_change.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)      847 2024-04-12 12:33:50.000000 django-plans-1.1.0/docs/source/plans_expiration.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     2417 2024-04-12 12:33:50.000000 django-plans-1.1.0/docs/source/plans_recurrence.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     5248 2024-04-12 12:33:50.000000 django-plans-1.1.0/docs/source/quota_validators.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     9824 2024-04-12 12:33:50.000000 django-plans-1.1.0/docs/source/settings.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     2388 2024-04-12 12:33:50.000000 django-plans-1.1.0/docs/source/south.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     1583 2024-04-12 12:33:50.000000 django-plans-1.1.0/docs/source/taxation.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     2302 2024-04-12 12:33:50.000000 django-plans-1.1.0/docs/source/templating.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)      296 2024-04-12 12:33:50.000000 django-plans-1.1.0/fabfile.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.929354 django-plans-1.1.0/plans/
--rw-rw-r--   0 petr      (1000) petr      (1000)      162 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/__init__.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     9022 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/admin.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      277 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/apps.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.929354 django-plans-1.1.0/plans/base/
--rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/base/__init__.py
--rw-rw-r--   0 petr      (1000) petr      (1000)    50345 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/base/models.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      273 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/conf.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     1299 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/context_processors.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     2488 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/contrib.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     1686 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/enumeration.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.929354 django-plans-1.1.0/plans/fixtures/
--rw-rw-r--   0 petr      (1000) petr      (1000)      678 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/fixtures/initial_plan.json
--rw-rw-r--   0 petr      (1000) petr      (1000)     1187 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/fixtures/test_django-plans_auth.json
--rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/fixtures/test_django-plans_default_plans.json
--rw-rw-r--   0 petr      (1000) petr      (1000)     9479 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/fixtures/test_django-plans_plans.json
--rw-rw-r--   0 petr      (1000) petr      (1000)     2127 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/forms.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      351 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/importer.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     2273 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/listeners.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.913355 django-plans-1.1.0/plans/locale/
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.913355 django-plans-1.1.0/plans/locale/en/
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.929354 django-plans-1.1.0/plans/locale/en/LC_MESSAGES/
--rw-rw-r--   0 petr      (1000) petr      (1000)    15215 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/locale/en/LC_MESSAGES/django.po
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.913355 django-plans-1.1.0/plans/locale/pl/
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.929354 django-plans-1.1.0/plans/locale/pl/LC_MESSAGES/
--rw-rw-r--   0 petr      (1000) petr      (1000)    10111 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/locale/pl/LC_MESSAGES/django.mo
--rw-rw-r--   0 petr      (1000) petr      (1000)    15132 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/locale/pl/LC_MESSAGES/django.po
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.913355 django-plans-1.1.0/plans/locale/pt_BR/
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.929354 django-plans-1.1.0/plans/locale/pt_BR/LC_MESSAGES/
--rw-rw-r--   0 petr      (1000) petr      (1000)     4374 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/locale/pt_BR/LC_MESSAGES/django.mo
--rw-rw-r--   0 petr      (1000) petr      (1000)    16542 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/locale/pt_BR/LC_MESSAGES/django.po
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.913355 django-plans-1.1.0/plans/locale/ru/
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.933354 django-plans-1.1.0/plans/locale/ru/LC_MESSAGES/
--rw-rw-r--   0 petr      (1000) petr      (1000)    11843 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/locale/ru/LC_MESSAGES/django.mo
--rw-rw-r--   0 petr      (1000) petr      (1000)    15021 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/locale/ru/LC_MESSAGES/django.po
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.933354 django-plans-1.1.0/plans/management/
--rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/management/__init__.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.933354 django-plans-1.1.0/plans/management/commands/
--rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/management/commands/__init__.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      930 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/management/commands/autorenew_accounts.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      417 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/management/commands/create_userplans.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      291 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/management/commands/expire_accounts.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.933354 django-plans-1.1.0/plans/migrations/
--rw-rw-r--   0 petr      (1000) petr      (1000)    22268 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/migrations/0001_initial.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      890 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/migrations/0002_auto_20180901_1744.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     1481 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/migrations/0003_make_plans_unique.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      480 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/migrations/0004_create_user_plans.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     4417 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/migrations/0005_recurring_payments.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      665 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/migrations/0006_auto_20200504_1541.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      428 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/migrations/0007_recurringuserplan_card_masked_number.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      625 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/migrations/0008_recurringuserplan_token_verified.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      456 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/migrations/0009_auto_20210303_1134.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     2715 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/migrations/0010_auto_20220113_1317.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     5735 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/migrations/0011_auto_20220208_1344.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      531 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/migrations/0012_planpricing_visible.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     1457 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/migrations/0013_alter_recurringuserplan_has_automatic_renewal_and_more.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     3085 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/migrations/0014_recurringuserplan_has_automatic_renewal_backup_deprecated_to_renewal_triggered_by.py
--rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/migrations/__init__.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      536 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/mixins.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     1903 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/models.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     3643 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/plan_change.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      308 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/quota.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     1721 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/signals.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     2176 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/tasks.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.933354 django-plans-1.1.0/plans/taxation/
--rw-rw-r--   0 petr      (1000) petr      (1000)     1266 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/taxation/__init__.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     6207 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/taxation/eu.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      553 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/taxation/ru.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.913355 django-plans-1.1.0/plans/templates/
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.933354 django-plans-1.1.0/plans/templates/mail/
--rw-rw-r--   0 petr      (1000) petr      (1000)      533 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/templates/mail/change_plan_body.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)      127 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/templates/mail/change_plan_title.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)      573 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/templates/mail/expired_account_body.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)       90 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/templates/mail/expired_account_title.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)      536 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/templates/mail/extend_account_body.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)      145 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/templates/mail/extend_account_title.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)      511 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/templates/mail/invoice_created_body.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)      225 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/templates/mail/invoice_created_title.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)      590 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/templates/mail/remind_expire_body.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)      188 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/templates/mail/remind_expire_title.txt
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.937353 django-plans-1.1.0/plans/templates/plans/
--rw-rw-r--   0 petr      (1000) petr      (1000)      668 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/templates/plans/account_activation.html
--rw-rw-r--   0 petr      (1000) petr      (1000)      305 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/templates/plans/base.html
--rw-rw-r--   0 petr      (1000) petr      (1000)      835 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/templates/plans/billing_info_create_or_update.html
--rw-rw-r--   0 petr      (1000) petr      (1000)      429 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/templates/plans/billing_info_delete.html
--rw-rw-r--   0 petr      (1000) petr      (1000)     2811 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/templates/plans/create_order.html
--rw-rw-r--   0 petr      (1000) petr      (1000)     1135 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/templates/plans/current.html
--rw-rw-r--   0 petr      (1000) petr      (1000)     1068 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/templates/plans/expiration_messages.html
--rw-rw-r--   0 petr      (1000) petr      (1000)     1992 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/templates/plans/extend.html
--rw-rw-r--   0 petr      (1000) petr      (1000)      396 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/templates/plans/fake_payments.html
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.937353 django-plans-1.1.0/plans/templates/plans/invoices/
--rw-rw-r--   0 petr      (1000) petr      (1000)      186 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/templates/plans/invoices/PL_EN.html
--rw-rw-r--   0 petr      (1000) petr      (1000)     8160 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/templates/plans/invoices/PL_EN_layout.html
--rw-rw-r--   0 petr      (1000) petr      (1000)     1729 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/templates/plans/invoices/invoice_base.html
--rw-rw-r--   0 petr      (1000) petr      (1000)     3358 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/templates/plans/order_detail.html
--rw-rw-r--   0 petr      (1000) petr      (1000)     1258 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/templates/plans/order_detail_table.html
--rw-rw-r--   0 petr      (1000) petr      (1000)     2046 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/templates/plans/order_list.html
--rw-rw-r--   0 petr      (1000) petr      (1000)      846 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/templates/plans/pagination.html
--rw-rw-r--   0 petr      (1000) petr      (1000)     5599 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/templates/plans/plan_table.html
--rw-rw-r--   0 petr      (1000) petr      (1000)      176 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/templates/plans/pricing.html
--rw-rw-r--   0 petr      (1000) petr      (1000)      162 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/templates/plans/upgrade.html
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.937353 django-plans-1.1.0/plans/tests/
--rw-rw-r--   0 petr      (1000) petr      (1000)       29 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/tests/__init__.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     3309 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/tests/test_autorenew_accounts.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     7224 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/tests/test_views.py
--rw-rw-r--   0 petr      (1000) petr      (1000)    68912 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/tests/tests.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     2375 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/urls.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     1316 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/utils.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     5946 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/validators.py
--rw-rw-r--   0 petr      (1000) petr      (1000)    19429 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans/views.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.937353 django-plans-1.1.0/plans_i18n/
--rw-rw-r--   0 petr      (1000) petr      (1000)     1427 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans_i18n/README.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans_i18n/__init__.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      815 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans_i18n/admin.py
--rw-rw-r--   0 petr      (1000) petr      (1000)       65 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans_i18n/models.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      383 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans_i18n/tests.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      764 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans_i18n/translation.py
--rw-rw-r--   0 petr      (1000) petr      (1000)       26 2024-04-12 12:33:50.000000 django-plans-1.1.0/plans_i18n/views.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      371 2024-04-12 12:33:50.937353 django-plans-1.1.0/setup.cfg
--rw-rw-r--   0 petr      (1000) petr      (1000)     1329 2024-04-12 12:33:50.000000 django-plans-1.1.0/setup.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      624 2024-04-12 12:33:50.000000 django-plans-1.1.0/tox.ini
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-05-16 13:38:01.508797 django-plans-1.2.0/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      653 2024-05-16 13:38:00.000000 django-plans-1.2.0/.coveragerc
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-05-16 13:38:01.460797 django-plans-1.2.0/.github/
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-05-16 13:38:01.472797 django-plans-1.2.0/.github/workflows/
+-rw-rw-r--   0 petr      (1000) petr      (1000)     4052 2024-05-16 13:38:00.000000 django-plans-1.2.0/.github/workflows/main.yml
+-rw-rw-r--   0 petr      (1000) petr      (1000)      343 2024-05-16 13:38:00.000000 django-plans-1.2.0/.gitignore
+-rw-rw-r--   0 petr      (1000) petr      (1000)      616 2024-05-16 13:38:00.000000 django-plans-1.2.0/.travis.yml
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-05-16 13:38:01.472797 django-plans-1.2.0/.tx/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      396 2024-05-16 13:38:00.000000 django-plans-1.2.0/.tx/config
+-rw-rw-r--   0 petr      (1000) petr      (1000)       83 2024-05-16 13:38:00.000000 django-plans-1.2.0/AUTHORS
+-rw-rw-r--   0 petr      (1000) petr      (1000)     6977 2024-05-16 13:38:00.000000 django-plans-1.2.0/CHANGELOG
+-rw-rw-r--   0 petr      (1000) petr      (1000)     3215 2024-05-16 13:38:00.000000 django-plans-1.2.0/CODE_OF_CONDUCT.md
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1060 2024-05-16 13:38:00.000000 django-plans-1.2.0/LICENSE
+-rw-rw-r--   0 petr      (1000) petr      (1000)      188 2024-05-16 13:38:00.000000 django-plans-1.2.0/MANIFEST.in
+-rw-r--r--   0 petr      (1000) petr      (1000)     2056 2024-05-16 13:38:01.508797 django-plans-1.2.0/PKG-INFO
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1063 2024-05-16 13:38:00.000000 django-plans-1.2.0/README.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1617 2024-05-16 13:38:00.000000 django-plans-1.2.0/conftest.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-05-16 13:38:01.472797 django-plans-1.2.0/demo/
+-rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-05-16 13:38:00.000000 django-plans-1.2.0/demo/__init__.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-05-16 13:38:01.472797 django-plans-1.2.0/demo/example/
+-rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-05-16 13:38:00.000000 django-plans-1.2.0/demo/example/__init__.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-05-16 13:38:01.472797 django-plans-1.2.0/demo/example/foo/
+-rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-05-16 13:38:00.000000 django-plans-1.2.0/demo/example/foo/__init__.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-05-16 13:38:01.476797 django-plans-1.2.0/demo/example/foo/fixtures/
+-rw-rw-r--   0 petr      (1000) petr      (1000)     7641 2024-05-16 13:38:00.000000 django-plans-1.2.0/demo/example/foo/fixtures/initial_data.json
+-rw-rw-r--   0 petr      (1000) petr      (1000)      428 2024-05-16 13:38:00.000000 django-plans-1.2.0/demo/example/foo/forms.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-05-16 13:38:01.476797 django-plans-1.2.0/demo/example/foo/migrations/
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1128 2024-05-16 13:38:00.000000 django-plans-1.2.0/demo/example/foo/migrations/0001_initial.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-05-16 13:38:00.000000 django-plans-1.2.0/demo/example/foo/migrations/__init__.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      279 2024-05-16 13:38:00.000000 django-plans-1.2.0/demo/example/foo/models.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-05-16 13:38:01.460797 django-plans-1.2.0/demo/example/foo/templates/
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-05-16 13:38:01.476797 django-plans-1.2.0/demo/example/foo/templates/foo/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      591 2024-05-16 13:38:00.000000 django-plans-1.2.0/demo/example/foo/templates/foo/foo_confirm_delete.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)      650 2024-05-16 13:38:00.000000 django-plans-1.2.0/demo/example/foo/templates/foo/foo_form.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1044 2024-05-16 13:38:00.000000 django-plans-1.2.0/demo/example/foo/templates/foo/foo_list.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)      383 2024-05-16 13:38:00.000000 django-plans-1.2.0/demo/example/foo/tests.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      402 2024-05-16 13:38:00.000000 django-plans-1.2.0/demo/example/foo/urls.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      323 2024-05-16 13:38:00.000000 django-plans-1.2.0/demo/example/foo/validators.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1530 2024-05-16 13:38:00.000000 django-plans-1.2.0/demo/example/foo/views.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-05-16 13:38:01.460797 django-plans-1.2.0/demo/example/locale/
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-05-16 13:38:01.460797 django-plans-1.2.0/demo/example/locale/en/
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-05-16 13:38:01.476797 django-plans-1.2.0/demo/example/locale/en/LC_MESSAGES/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      378 2024-05-16 13:38:00.000000 django-plans-1.2.0/demo/example/locale/en/LC_MESSAGES/django.mo
+-rw-rw-r--   0 petr      (1000) petr      (1000)      714 2024-05-16 13:38:00.000000 django-plans-1.2.0/demo/example/locale/en/LC_MESSAGES/django.po
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-05-16 13:38:01.460797 django-plans-1.2.0/demo/example/locale/pl/
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-05-16 13:38:01.476797 django-plans-1.2.0/demo/example/locale/pl/LC_MESSAGES/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      603 2024-05-16 13:38:00.000000 django-plans-1.2.0/demo/example/locale/pl/LC_MESSAGES/django.mo
+-rw-rw-r--   0 petr      (1000) petr      (1000)      904 2024-05-16 13:38:00.000000 django-plans-1.2.0/demo/example/locale/pl/LC_MESSAGES/django.po
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-05-16 13:38:01.460797 django-plans-1.2.0/demo/example/locale/pt_BR/
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-05-16 13:38:01.476797 django-plans-1.2.0/demo/example/locale/pt_BR/LC_MESSAGES/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      495 2024-05-16 13:38:00.000000 django-plans-1.2.0/demo/example/locale/pt_BR/LC_MESSAGES/django.mo
+-rw-rw-r--   0 petr      (1000) petr      (1000)      804 2024-05-16 13:38:00.000000 django-plans-1.2.0/demo/example/locale/pt_BR/LC_MESSAGES/django.po
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-05-16 13:38:01.464797 django-plans-1.2.0/demo/example/locale/ru/
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-05-16 13:38:01.476797 django-plans-1.2.0/demo/example/locale/ru/LC_MESSAGES/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      549 2024-05-16 13:38:00.000000 django-plans-1.2.0/demo/example/locale/ru/LC_MESSAGES/django.mo
+-rw-rw-r--   0 petr      (1000) petr      (1000)      858 2024-05-16 13:38:00.000000 django-plans-1.2.0/demo/example/locale/ru/LC_MESSAGES/django.po
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-05-16 13:38:01.476797 django-plans-1.2.0/demo/example/sample_plans/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      160 2024-05-16 13:38:00.000000 django-plans-1.2.0/demo/example/sample_plans/__init__.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      233 2024-05-16 13:38:00.000000 django-plans-1.2.0/demo/example/sample_plans/admin.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      190 2024-05-16 13:38:00.000000 django-plans-1.2.0/demo/example/sample_plans/apps.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-05-16 13:38:01.476797 django-plans-1.2.0/demo/example/sample_plans/fixtures/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      693 2024-05-16 13:38:00.000000 django-plans-1.2.0/demo/example/sample_plans/fixtures/initial_plan.json
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1187 2024-05-16 13:38:00.000000 django-plans-1.2.0/demo/example/sample_plans/fixtures/test_django-plans_auth.json
+-rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-05-16 13:38:00.000000 django-plans-1.2.0/demo/example/sample_plans/fixtures/test_django-plans_default_plans.json
+-rw-rw-r--   0 petr      (1000) petr      (1000)     9864 2024-05-16 13:38:00.000000 django-plans-1.2.0/demo/example/sample_plans/fixtures/test_django-plans_plans.json
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-05-16 13:38:01.476797 django-plans-1.2.0/demo/example/sample_plans/management/
+-rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-05-16 13:38:00.000000 django-plans-1.2.0/demo/example/sample_plans/management/__init__.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-05-16 13:38:01.480797 django-plans-1.2.0/demo/example/sample_plans/management/commands/
+-rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-05-16 13:38:00.000000 django-plans-1.2.0/demo/example/sample_plans/management/commands/__init__.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      119 2024-05-16 13:38:00.000000 django-plans-1.2.0/demo/example/sample_plans/management/commands/autorenew_accounts.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      117 2024-05-16 13:38:00.000000 django-plans-1.2.0/demo/example/sample_plans/management/commands/create_userplans.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      116 2024-05-16 13:38:00.000000 django-plans-1.2.0/demo/example/sample_plans/management/commands/expire_accounts.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-05-16 13:38:01.480797 django-plans-1.2.0/demo/example/sample_plans/migrations/
+-rw-rw-r--   0 petr      (1000) petr      (1000)    31516 2024-05-16 13:38:00.000000 django-plans-1.2.0/demo/example/sample_plans/migrations/0001_initial.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-05-16 13:38:00.000000 django-plans-1.2.0/demo/example/sample_plans/migrations/__init__.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1960 2024-05-16 13:38:00.000000 django-plans-1.2.0/demo/example/sample_plans/models.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-05-16 13:38:01.464797 django-plans-1.2.0/demo/example/sample_plans/templates/
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-05-16 13:38:01.480797 django-plans-1.2.0/demo/example/sample_plans/templates/mail/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      533 2024-05-16 13:38:00.000000 django-plans-1.2.0/demo/example/sample_plans/templates/mail/change_plan_body.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)      127 2024-05-16 13:38:00.000000 django-plans-1.2.0/demo/example/sample_plans/templates/mail/change_plan_title.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)      573 2024-05-16 13:38:00.000000 django-plans-1.2.0/demo/example/sample_plans/templates/mail/expired_account_body.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)       90 2024-05-16 13:38:00.000000 django-plans-1.2.0/demo/example/sample_plans/templates/mail/expired_account_title.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)      536 2024-05-16 13:38:00.000000 django-plans-1.2.0/demo/example/sample_plans/templates/mail/extend_account_body.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)      145 2024-05-16 13:38:00.000000 django-plans-1.2.0/demo/example/sample_plans/templates/mail/extend_account_title.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)      511 2024-05-16 13:38:00.000000 django-plans-1.2.0/demo/example/sample_plans/templates/mail/invoice_created_body.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)      225 2024-05-16 13:38:00.000000 django-plans-1.2.0/demo/example/sample_plans/templates/mail/invoice_created_title.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)      590 2024-05-16 13:38:00.000000 django-plans-1.2.0/demo/example/sample_plans/templates/mail/remind_expire_body.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)      188 2024-05-16 13:38:00.000000 django-plans-1.2.0/demo/example/sample_plans/templates/mail/remind_expire_title.txt
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-05-16 13:38:01.484797 django-plans-1.2.0/demo/example/sample_plans/templates/plans/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      668 2024-05-16 13:38:00.000000 django-plans-1.2.0/demo/example/sample_plans/templates/plans/account_activation.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)      305 2024-05-16 13:38:00.000000 django-plans-1.2.0/demo/example/sample_plans/templates/plans/base.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)      653 2024-05-16 13:38:00.000000 django-plans-1.2.0/demo/example/sample_plans/templates/plans/billing_info_create.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)      835 2024-05-16 13:38:00.000000 django-plans-1.2.0/demo/example/sample_plans/templates/plans/billing_info_create_or_update.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)      429 2024-05-16 13:38:00.000000 django-plans-1.2.0/demo/example/sample_plans/templates/plans/billing_info_delete.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)      744 2024-05-16 13:38:00.000000 django-plans-1.2.0/demo/example/sample_plans/templates/plans/billing_info_update.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2811 2024-05-16 13:38:00.000000 django-plans-1.2.0/demo/example/sample_plans/templates/plans/create_order.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1135 2024-05-16 13:38:00.000000 django-plans-1.2.0/demo/example/sample_plans/templates/plans/current.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1068 2024-05-16 13:38:00.000000 django-plans-1.2.0/demo/example/sample_plans/templates/plans/expiration_messages.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1992 2024-05-16 13:38:00.000000 django-plans-1.2.0/demo/example/sample_plans/templates/plans/extend.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)      396 2024-05-16 13:38:00.000000 django-plans-1.2.0/demo/example/sample_plans/templates/plans/fake_payments.html
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-05-16 13:38:01.484797 django-plans-1.2.0/demo/example/sample_plans/templates/plans/invoices/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      186 2024-05-16 13:38:00.000000 django-plans-1.2.0/demo/example/sample_plans/templates/plans/invoices/PL_EN.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)     8160 2024-05-16 13:38:00.000000 django-plans-1.2.0/demo/example/sample_plans/templates/plans/invoices/PL_EN_layout.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1729 2024-05-16 13:38:00.000000 django-plans-1.2.0/demo/example/sample_plans/templates/plans/invoices/invoice_base.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)     3358 2024-05-16 13:38:00.000000 django-plans-1.2.0/demo/example/sample_plans/templates/plans/order_detail.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1258 2024-05-16 13:38:00.000000 django-plans-1.2.0/demo/example/sample_plans/templates/plans/order_detail_table.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2046 2024-05-16 13:38:00.000000 django-plans-1.2.0/demo/example/sample_plans/templates/plans/order_list.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)      846 2024-05-16 13:38:00.000000 django-plans-1.2.0/demo/example/sample_plans/templates/plans/pagination.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)     5465 2024-05-16 13:38:00.000000 django-plans-1.2.0/demo/example/sample_plans/templates/plans/plan_table.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)      176 2024-05-16 13:38:00.000000 django-plans-1.2.0/demo/example/sample_plans/templates/plans/pricing.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)      162 2024-05-16 13:38:00.000000 django-plans-1.2.0/demo/example/sample_plans/templates/plans/upgrade.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2239 2024-05-16 13:38:00.000000 django-plans-1.2.0/demo/example/sample_plans/tests.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     5544 2024-05-16 13:38:00.000000 django-plans-1.2.0/demo/example/settings.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-05-16 13:38:01.464797 django-plans-1.2.0/demo/example/static/
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-05-16 13:38:01.488797 django-plans-1.2.0/demo/example/static/css/
+-rw-rw-r--   0 petr      (1000) petr      (1000)     3961 2024-05-16 13:38:00.000000 django-plans-1.2.0/demo/example/static/css/example.css
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-05-16 13:38:01.464797 django-plans-1.2.0/demo/example/static/img/
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-05-16 13:38:01.488797 django-plans-1.2.0/demo/example/static/img/messages/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      294 2024-05-16 13:38:00.000000 django-plans-1.2.0/demo/example/static/img/messages/icon_alert.png
+-rw-rw-r--   0 petr      (1000) petr      (1000)     3668 2024-05-16 13:38:00.000000 django-plans-1.2.0/demo/example/static/img/messages/icon_error.png
+-rw-rw-r--   0 petr      (1000) petr      (1000)     3675 2024-05-16 13:38:00.000000 django-plans-1.2.0/demo/example/static/img/messages/icon_success.png
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-05-16 13:38:01.488797 django-plans-1.2.0/demo/example/templates/
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2746 2024-05-16 13:38:00.000000 django-plans-1.2.0/demo/example/templates/base.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)      823 2024-05-16 13:38:00.000000 django-plans-1.2.0/demo/example/templates/home.html
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-05-16 13:38:01.488797 django-plans-1.2.0/demo/example/templates/plans/
+-rw-rw-r--   0 petr      (1000) petr      (1000)       25 2024-05-16 13:38:00.000000 django-plans-1.2.0/demo/example/templates/plans/base.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)      757 2024-05-16 13:38:00.000000 django-plans-1.2.0/demo/example/templates/plans/billing_info_create.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)      882 2024-05-16 13:38:00.000000 django-plans-1.2.0/demo/example/templates/plans/billing_info_update.html
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-05-16 13:38:01.488797 django-plans-1.2.0/demo/example/templates/registration/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      718 2024-05-16 13:38:00.000000 django-plans-1.2.0/demo/example/templates/registration/login.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)      605 2024-05-16 13:38:00.000000 django-plans-1.2.0/demo/example/urls.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1132 2024-05-16 13:38:00.000000 django-plans-1.2.0/demo/example/wsgi.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      323 2024-05-16 13:38:00.000000 django-plans-1.2.0/demo/fabfile.py
+-rwxrwxr-x   0 petr      (1000) petr      (1000)      813 2024-05-16 13:38:00.000000 django-plans-1.2.0/demo/manage.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      428 2024-05-16 13:38:00.000000 django-plans-1.2.0/demo/requirements.txt
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-05-16 13:38:01.508797 django-plans-1.2.0/django_plans.egg-info/
+-rw-r--r--   0 petr      (1000) petr      (1000)     2056 2024-05-16 13:38:01.000000 django-plans-1.2.0/django_plans.egg-info/PKG-INFO
+-rw-rw-r--   0 petr      (1000) petr      (1000)     8584 2024-05-16 13:38:01.000000 django-plans-1.2.0/django_plans.egg-info/SOURCES.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)        1 2024-05-16 13:38:01.000000 django-plans-1.2.0/django_plans.egg-info/dependency_links.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)        1 2024-05-16 13:38:01.000000 django-plans-1.2.0/django_plans.egg-info/not-zip-safe
+-rw-rw-r--   0 petr      (1000) petr      (1000)      186 2024-05-16 13:38:01.000000 django-plans-1.2.0/django_plans.egg-info/requires.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)       22 2024-05-16 13:38:01.000000 django-plans-1.2.0/django_plans.egg-info/top_level.txt
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-05-16 13:38:01.488797 django-plans-1.2.0/docs/
+-rw-rw-r--   0 petr      (1000) petr      (1000)     5597 2024-05-16 13:38:00.000000 django-plans-1.2.0/docs/Makefile
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-05-16 13:38:01.492797 django-plans-1.2.0/docs/source/
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-05-16 13:38:01.464797 django-plans-1.2.0/docs/source/_static/
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-05-16 13:38:01.492797 django-plans-1.2.0/docs/source/_static/images/
+-rw-rw-r--   0 petr      (1000) petr      (1000)   176623 2024-05-16 13:38:00.000000 django-plans-1.2.0/docs/source/_static/images/django-plans-1.png
+-rw-rw-r--   0 petr      (1000) petr      (1000)   193693 2024-05-16 13:38:00.000000 django-plans-1.2.0/docs/source/_static/images/django-plans-2.png
+-rw-rw-r--   0 petr      (1000) petr      (1000)   146667 2024-05-16 13:38:00.000000 django-plans-1.2.0/docs/source/_static/images/django-plans-3.png
+-rw-rw-r--   0 petr      (1000) petr      (1000)      860 2024-05-16 13:38:00.000000 django-plans-1.2.0/docs/source/caveats.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     8032 2024-05-16 13:38:00.000000 django-plans-1.2.0/docs/source/conf.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1217 2024-05-16 13:38:00.000000 django-plans-1.2.0/docs/source/customize_models.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1703 2024-05-16 13:38:00.000000 django-plans-1.2.0/docs/source/index.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2316 2024-05-16 13:38:00.000000 django-plans-1.2.0/docs/source/installation.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1966 2024-05-16 13:38:00.000000 django-plans-1.2.0/docs/source/integration.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2588 2024-05-16 13:38:00.000000 django-plans-1.2.0/docs/source/invoicing.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     6661 2024-05-16 13:38:00.000000 django-plans-1.2.0/docs/source/plans.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1024 2024-05-16 13:38:00.000000 django-plans-1.2.0/docs/source/plans_change.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)      847 2024-05-16 13:38:00.000000 django-plans-1.2.0/docs/source/plans_expiration.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2417 2024-05-16 13:38:00.000000 django-plans-1.2.0/docs/source/plans_recurrence.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     5248 2024-05-16 13:38:00.000000 django-plans-1.2.0/docs/source/quota_validators.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     9824 2024-05-16 13:38:00.000000 django-plans-1.2.0/docs/source/settings.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2388 2024-05-16 13:38:00.000000 django-plans-1.2.0/docs/source/south.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1583 2024-05-16 13:38:00.000000 django-plans-1.2.0/docs/source/taxation.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2302 2024-05-16 13:38:00.000000 django-plans-1.2.0/docs/source/templating.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)      296 2024-05-16 13:38:00.000000 django-plans-1.2.0/fabfile.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-05-16 13:38:01.496797 django-plans-1.2.0/plans/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      162 2024-05-16 13:38:00.000000 django-plans-1.2.0/plans/__init__.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     9022 2024-05-16 13:38:00.000000 django-plans-1.2.0/plans/admin.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      277 2024-05-16 13:38:00.000000 django-plans-1.2.0/plans/apps.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-05-16 13:38:01.496797 django-plans-1.2.0/plans/base/
+-rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-05-16 13:38:00.000000 django-plans-1.2.0/plans/base/__init__.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)    50345 2024-05-16 13:38:00.000000 django-plans-1.2.0/plans/base/models.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      273 2024-05-16 13:38:00.000000 django-plans-1.2.0/plans/conf.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1299 2024-05-16 13:38:00.000000 django-plans-1.2.0/plans/context_processors.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2488 2024-05-16 13:38:00.000000 django-plans-1.2.0/plans/contrib.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1686 2024-05-16 13:38:00.000000 django-plans-1.2.0/plans/enumeration.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-05-16 13:38:01.496797 django-plans-1.2.0/plans/fixtures/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      678 2024-05-16 13:38:00.000000 django-plans-1.2.0/plans/fixtures/initial_plan.json
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1187 2024-05-16 13:38:00.000000 django-plans-1.2.0/plans/fixtures/test_django-plans_auth.json
+-rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-05-16 13:38:00.000000 django-plans-1.2.0/plans/fixtures/test_django-plans_default_plans.json
+-rw-rw-r--   0 petr      (1000) petr      (1000)     9479 2024-05-16 13:38:00.000000 django-plans-1.2.0/plans/fixtures/test_django-plans_plans.json
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2127 2024-05-16 13:38:00.000000 django-plans-1.2.0/plans/forms.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      351 2024-05-16 13:38:00.000000 django-plans-1.2.0/plans/importer.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2273 2024-05-16 13:38:00.000000 django-plans-1.2.0/plans/listeners.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-05-16 13:38:01.468797 django-plans-1.2.0/plans/locale/
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-05-16 13:38:01.464797 django-plans-1.2.0/plans/locale/en/
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-05-16 13:38:01.496797 django-plans-1.2.0/plans/locale/en/LC_MESSAGES/
+-rw-rw-r--   0 petr      (1000) petr      (1000)    15215 2024-05-16 13:38:00.000000 django-plans-1.2.0/plans/locale/en/LC_MESSAGES/django.po
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-05-16 13:38:01.468797 django-plans-1.2.0/plans/locale/pl/
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-05-16 13:38:01.496797 django-plans-1.2.0/plans/locale/pl/LC_MESSAGES/
+-rw-rw-r--   0 petr      (1000) petr      (1000)    10111 2024-05-16 13:38:00.000000 django-plans-1.2.0/plans/locale/pl/LC_MESSAGES/django.mo
+-rw-rw-r--   0 petr      (1000) petr      (1000)    15132 2024-05-16 13:38:00.000000 django-plans-1.2.0/plans/locale/pl/LC_MESSAGES/django.po
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-05-16 13:38:01.468797 django-plans-1.2.0/plans/locale/pt_BR/
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-05-16 13:38:01.496797 django-plans-1.2.0/plans/locale/pt_BR/LC_MESSAGES/
+-rw-rw-r--   0 petr      (1000) petr      (1000)     4374 2024-05-16 13:38:00.000000 django-plans-1.2.0/plans/locale/pt_BR/LC_MESSAGES/django.mo
+-rw-rw-r--   0 petr      (1000) petr      (1000)    16542 2024-05-16 13:38:00.000000 django-plans-1.2.0/plans/locale/pt_BR/LC_MESSAGES/django.po
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-05-16 13:38:01.468797 django-plans-1.2.0/plans/locale/ru/
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-05-16 13:38:01.500797 django-plans-1.2.0/plans/locale/ru/LC_MESSAGES/
+-rw-rw-r--   0 petr      (1000) petr      (1000)    11843 2024-05-16 13:38:00.000000 django-plans-1.2.0/plans/locale/ru/LC_MESSAGES/django.mo
+-rw-rw-r--   0 petr      (1000) petr      (1000)    15021 2024-05-16 13:38:00.000000 django-plans-1.2.0/plans/locale/ru/LC_MESSAGES/django.po
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-05-16 13:38:01.500797 django-plans-1.2.0/plans/management/
+-rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-05-16 13:38:00.000000 django-plans-1.2.0/plans/management/__init__.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-05-16 13:38:01.500797 django-plans-1.2.0/plans/management/commands/
+-rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-05-16 13:38:00.000000 django-plans-1.2.0/plans/management/commands/__init__.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      930 2024-05-16 13:38:00.000000 django-plans-1.2.0/plans/management/commands/autorenew_accounts.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      417 2024-05-16 13:38:00.000000 django-plans-1.2.0/plans/management/commands/create_userplans.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      291 2024-05-16 13:38:00.000000 django-plans-1.2.0/plans/management/commands/expire_accounts.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-05-16 13:38:01.500797 django-plans-1.2.0/plans/migrations/
+-rw-rw-r--   0 petr      (1000) petr      (1000)    22268 2024-05-16 13:38:00.000000 django-plans-1.2.0/plans/migrations/0001_initial.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      890 2024-05-16 13:38:00.000000 django-plans-1.2.0/plans/migrations/0002_auto_20180901_1744.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1481 2024-05-16 13:38:00.000000 django-plans-1.2.0/plans/migrations/0003_make_plans_unique.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      480 2024-05-16 13:38:00.000000 django-plans-1.2.0/plans/migrations/0004_create_user_plans.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     4417 2024-05-16 13:38:00.000000 django-plans-1.2.0/plans/migrations/0005_recurring_payments.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      665 2024-05-16 13:38:00.000000 django-plans-1.2.0/plans/migrations/0006_auto_20200504_1541.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      428 2024-05-16 13:38:00.000000 django-plans-1.2.0/plans/migrations/0007_recurringuserplan_card_masked_number.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      625 2024-05-16 13:38:00.000000 django-plans-1.2.0/plans/migrations/0008_recurringuserplan_token_verified.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      456 2024-05-16 13:38:00.000000 django-plans-1.2.0/plans/migrations/0009_auto_20210303_1134.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2715 2024-05-16 13:38:00.000000 django-plans-1.2.0/plans/migrations/0010_auto_20220113_1317.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     5735 2024-05-16 13:38:00.000000 django-plans-1.2.0/plans/migrations/0011_auto_20220208_1344.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      531 2024-05-16 13:38:00.000000 django-plans-1.2.0/plans/migrations/0012_planpricing_visible.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1457 2024-05-16 13:38:00.000000 django-plans-1.2.0/plans/migrations/0013_alter_recurringuserplan_has_automatic_renewal_and_more.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     3085 2024-05-16 13:38:00.000000 django-plans-1.2.0/plans/migrations/0014_recurringuserplan_has_automatic_renewal_backup_deprecated_to_renewal_triggered_by.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-05-16 13:38:00.000000 django-plans-1.2.0/plans/migrations/__init__.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      536 2024-05-16 13:38:00.000000 django-plans-1.2.0/plans/mixins.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1903 2024-05-16 13:38:00.000000 django-plans-1.2.0/plans/models.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     4196 2024-05-16 13:38:00.000000 django-plans-1.2.0/plans/plan_change.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      308 2024-05-16 13:38:00.000000 django-plans-1.2.0/plans/quota.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1721 2024-05-16 13:38:00.000000 django-plans-1.2.0/plans/signals.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2176 2024-05-16 13:38:00.000000 django-plans-1.2.0/plans/tasks.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-05-16 13:38:01.504797 django-plans-1.2.0/plans/taxation/
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1266 2024-05-16 13:38:00.000000 django-plans-1.2.0/plans/taxation/__init__.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     6207 2024-05-16 13:38:00.000000 django-plans-1.2.0/plans/taxation/eu.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      553 2024-05-16 13:38:00.000000 django-plans-1.2.0/plans/taxation/ru.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-05-16 13:38:01.468797 django-plans-1.2.0/plans/templates/
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-05-16 13:38:01.504797 django-plans-1.2.0/plans/templates/mail/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      533 2024-05-16 13:38:00.000000 django-plans-1.2.0/plans/templates/mail/change_plan_body.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)      127 2024-05-16 13:38:00.000000 django-plans-1.2.0/plans/templates/mail/change_plan_title.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)      573 2024-05-16 13:38:00.000000 django-plans-1.2.0/plans/templates/mail/expired_account_body.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)       90 2024-05-16 13:38:00.000000 django-plans-1.2.0/plans/templates/mail/expired_account_title.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)      536 2024-05-16 13:38:00.000000 django-plans-1.2.0/plans/templates/mail/extend_account_body.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)      145 2024-05-16 13:38:00.000000 django-plans-1.2.0/plans/templates/mail/extend_account_title.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)      511 2024-05-16 13:38:00.000000 django-plans-1.2.0/plans/templates/mail/invoice_created_body.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)      225 2024-05-16 13:38:00.000000 django-plans-1.2.0/plans/templates/mail/invoice_created_title.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)      590 2024-05-16 13:38:00.000000 django-plans-1.2.0/plans/templates/mail/remind_expire_body.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)      188 2024-05-16 13:38:00.000000 django-plans-1.2.0/plans/templates/mail/remind_expire_title.txt
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-05-16 13:38:01.508797 django-plans-1.2.0/plans/templates/plans/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      668 2024-05-16 13:38:00.000000 django-plans-1.2.0/plans/templates/plans/account_activation.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)      305 2024-05-16 13:38:00.000000 django-plans-1.2.0/plans/templates/plans/base.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)      835 2024-05-16 13:38:00.000000 django-plans-1.2.0/plans/templates/plans/billing_info_create_or_update.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)      429 2024-05-16 13:38:00.000000 django-plans-1.2.0/plans/templates/plans/billing_info_delete.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2811 2024-05-16 13:38:00.000000 django-plans-1.2.0/plans/templates/plans/create_order.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1135 2024-05-16 13:38:00.000000 django-plans-1.2.0/plans/templates/plans/current.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1068 2024-05-16 13:38:00.000000 django-plans-1.2.0/plans/templates/plans/expiration_messages.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1992 2024-05-16 13:38:00.000000 django-plans-1.2.0/plans/templates/plans/extend.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)      396 2024-05-16 13:38:00.000000 django-plans-1.2.0/plans/templates/plans/fake_payments.html
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-05-16 13:38:01.508797 django-plans-1.2.0/plans/templates/plans/invoices/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      186 2024-05-16 13:38:00.000000 django-plans-1.2.0/plans/templates/plans/invoices/PL_EN.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)     8160 2024-05-16 13:38:00.000000 django-plans-1.2.0/plans/templates/plans/invoices/PL_EN_layout.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1729 2024-05-16 13:38:00.000000 django-plans-1.2.0/plans/templates/plans/invoices/invoice_base.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)     3358 2024-05-16 13:38:00.000000 django-plans-1.2.0/plans/templates/plans/order_detail.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1258 2024-05-16 13:38:00.000000 django-plans-1.2.0/plans/templates/plans/order_detail_table.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2046 2024-05-16 13:38:00.000000 django-plans-1.2.0/plans/templates/plans/order_list.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)      846 2024-05-16 13:38:00.000000 django-plans-1.2.0/plans/templates/plans/pagination.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)     5599 2024-05-16 13:38:00.000000 django-plans-1.2.0/plans/templates/plans/plan_table.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)      176 2024-05-16 13:38:00.000000 django-plans-1.2.0/plans/templates/plans/pricing.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)      162 2024-05-16 13:38:00.000000 django-plans-1.2.0/plans/templates/plans/upgrade.html
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-05-16 13:38:01.508797 django-plans-1.2.0/plans/tests/
+-rw-rw-r--   0 petr      (1000) petr      (1000)       29 2024-05-16 13:38:00.000000 django-plans-1.2.0/plans/tests/__init__.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     3309 2024-05-16 13:38:00.000000 django-plans-1.2.0/plans/tests/test_autorenew_accounts.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     7224 2024-05-16 13:38:00.000000 django-plans-1.2.0/plans/tests/test_views.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)    68912 2024-05-16 13:38:00.000000 django-plans-1.2.0/plans/tests/tests.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2375 2024-05-16 13:38:00.000000 django-plans-1.2.0/plans/urls.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1316 2024-05-16 13:38:00.000000 django-plans-1.2.0/plans/utils.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     5946 2024-05-16 13:38:00.000000 django-plans-1.2.0/plans/validators.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)    18933 2024-05-16 13:38:00.000000 django-plans-1.2.0/plans/views.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2024-05-16 13:38:01.508797 django-plans-1.2.0/plans_i18n/
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1427 2024-05-16 13:38:00.000000 django-plans-1.2.0/plans_i18n/README.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)        0 2024-05-16 13:38:00.000000 django-plans-1.2.0/plans_i18n/__init__.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      815 2024-05-16 13:38:00.000000 django-plans-1.2.0/plans_i18n/admin.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)       65 2024-05-16 13:38:00.000000 django-plans-1.2.0/plans_i18n/models.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      383 2024-05-16 13:38:00.000000 django-plans-1.2.0/plans_i18n/tests.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      764 2024-05-16 13:38:00.000000 django-plans-1.2.0/plans_i18n/translation.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)       26 2024-05-16 13:38:00.000000 django-plans-1.2.0/plans_i18n/views.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      371 2024-05-16 13:38:01.512797 django-plans-1.2.0/setup.cfg
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1329 2024-05-16 13:38:00.000000 django-plans-1.2.0/setup.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      624 2024-05-16 13:38:00.000000 django-plans-1.2.0/tox.ini
```

### Comparing `django-plans-1.1.0/.coveragerc` & `django-plans-1.2.0/.coveragerc`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/.github/workflows/main.yml` & `django-plans-1.2.0/.github/workflows/main.yml`

 * *Files 6% similar despite different names*

```diff
@@ -18,38 +18,40 @@
   # This workflow contains a single job called "build"
   tests:
     # The type of runner that the job will run on
     runs-on: ubuntu-latest
 
     strategy:
       matrix:
-        DJANGO_VERSION: [ '2.2.*', '3.0.*', '3.1.*', '3.2.*', '4.0.*', '4.1.*', '4.2.*' ]
-        python-version: ['3.7', '3.8', '3.9', '3.10', '3.11']
+        DJANGO_VERSION: ['3.2.*', '4.0.*', '4.1.*', '4.2.*', '5.0.*']
+        python-version: ['3.7', '3.8', '3.9', '3.10', '3.11', '3.12']
         exclude:
+          - DJANGO_VERSION: '5.0.*'
+            python-version: '3.9'
+          - DJANGO_VERSION: '5.0.*'
+            python-version: '3.8'
+          - DJANGO_VERSION: '5.0.*'
+            python-version: '3.7'
+
           - DJANGO_VERSION: '4.2.*'
             python-version: '3.7'
+
           - DJANGO_VERSION: '4.1.*'
             python-version: '3.7'
+
           - DJANGO_VERSION: '4.0.*'
-            python-version: '3.7'
-          - DJANGO_VERSION: '3.1.*'
-            python-version: '3.10'
-          - DJANGO_VERSION: '3.0.*'
-            python-version: '3.10'
-          - DJANGO_VERSION: '2.2.*'
-            python-version: '3.10'
+            python-version: '3.12'
           - DJANGO_VERSION: '4.0.*'
             python-version: '3.11'
+          - DJANGO_VERSION: '4.0.*'
+            python-version: '3.7'
+
+          - DJANGO_VERSION: '3.2.*'
+            python-version: '3.12'
           - DJANGO_VERSION: '3.2.*'
-            python-version: '3.11'
-          - DJANGO_VERSION: '3.1.*'
-            python-version: '3.11'
-          - DJANGO_VERSION: '3.0.*'
-            python-version: '3.11'
-          - DJANGO_VERSION: '2.2.*'
             python-version: '3.11'
       fail-fast: false
     services:
       postgres:
         image: postgres
         env:
           POSTGRES_PASSWORD: postgres
@@ -76,18 +78,14 @@
       - name: Install
         run: |
            pip install -q -e .
            pip install -q --upgrade --upgrade-strategy eager -r demo/requirements.txt
            pip install -q Django==${{ matrix.DJANGO_VERSION }}
            pip install codecov
 
-      - name: Install django-sequences and psycopg2 for older Django versions
-        if: ${{ matrix.DJANGO_VERSION == '2.2.*' || matrix.DJANGO_VERSION == '3.0.*' }}
-        run: pip install "django-sequences<2.7" "psycopg2<2.9"
-
       - name: Run migration check
         run: |
           OUTPUT=$(python demo/manage.py makemigrations --dry-run plans)
           echo $OUTPUT | grep "No changes detected" &>/dev/null &&
             echo "SUCCESS: Migrations check successful!" ||
               {
                 echo $OUTPUT
@@ -96,15 +94,15 @@
               }
 
       - name: Testing
         run: |
           # Run tests for sample app used for testing extensibility
           PYTHONPATH="." MANAGE_PY_PATH="demo/manage.py" SAMPLE_APP=1 demo/manage.py test example
           case "${{ matrix.DJANGO_VERSION }},${{ matrix.python-version }}" in
-            2.2.*,3.7|3.0.*,3.7|3.1.*,3.7|3.2.*,3.7|4.0.*,3.8|4.0.*,3.9|4.0.*,3.10)  # Django runs with warnings in this python version
+            3.2.*,3.7|4.0.*,3.8|4.0.*,3.9|4.0.*,3.10)  # Django runs with warnings in this python version
               PYTHONPATH="." MANAGE_PY_PATH="demo/manage.py" coverage run demo/manage.py test plans
               ;;
             *)
               PYTHONPATH="." MANAGE_PY_PATH="demo/manage.py" PYTHONWARNINGS="error::DeprecationWarning" coverage run demo/manage.py test plans
               ;;
           esac
           coverage xml && codecov
```

### Comparing `django-plans-1.1.0/.travis.yml` & `django-plans-1.2.0/.travis.yml`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/CHANGELOG` & `django-plans-1.2.0/CHANGELOG`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 django-plans changelog
 ======================
 
+
+1.2.0
+------------------
+* make possible to reuse get_change_price()
+
 1.1.0
 ------------------
 * Add `AbstractRecurringUserPlan.renewal_triggered_by`
 * Use `AbstractRecurringUserPlan.renewal_triggered_by` instead of `has_automatic_renewal`; `has_automatic_renewal` is not used anywhere anymore; `has_automatic_renewal=True` is automatically migrated to `renewal_triggered_by=TASK` and `has_automatic_renewal=False` to `renewal_triggered_by=USER`
 * Rename `AbstractRecurringUserPlan.has_automatic_renewal` to `_has_automatic_renewal_backup_deprecated` so it can be used make your own data migration from the former `has_automatic_renewal` to `renewal_triggered_by` if the default one does not work for you
 * Add `AbstractRecurringUserPlan.has_automatic_renewal` property that issues a deprecation warning and uses `renewal_triggered_by` under the hood
 * Add `renewal_triggered_by` parameter to `AbstractUserPlan.set_plan_renewal`
@@ -60,15 +65,15 @@
 * UserPlans are now automatically created with initial migration or with `create_userplans` adminaction.
 * Added possibility to define `PLANS_APP_VERBOSE_NAME` to personalize plans' `verbose_name`
 * Return back to order after setting up billing info
 
 0.8.13
 ------
 * Supporting Django 2.0.6.
-1.1.0 (unreleased)
+1.2.0 (unreleased)
 * New VAT standard rates 2017
 * Remove dependency on `django.contrib.sites`.
 * Feature #53: Cleaner and more explicit exception handling on `Plan.get_default_plan `.
 * Feature #59: Adding code coverage to code base.
 * Support customised user models by using `django.contrib.auth.get_user_model()`.
 * Add Database migrations.
```

### Comparing `django-plans-1.1.0/CODE_OF_CONDUCT.md` & `django-plans-1.2.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/LICENSE` & `django-plans-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/PKG-INFO` & `django-plans-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-plans
-Version: 1.1.0
+Version: 1.2.0
 Summary: Pluggable django app for managing pricing plans with quotas and accounts expiration
 Home-page: https://github.com/cypreess/django-plans
 Author: Krzysztof Dorosz
 Author-email: cypreess@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Django
@@ -44,15 +44,15 @@
 * Customizable billing periods (plan pricing),
 * Order total calculation using customizable taxation policy (e.g. in EU calculating VAT based on seller/buyer countries and VIES)
 * Invoicing,
 * Account expiratons + E-mail remainders.
 
 Documentation: https://django-plans.readthedocs.org/
 
-Master branch: Support for Django +2.2, support for Python +3.6
+Master branch: Support for Django >=3.2, support for Python >=3.7
 
 .. image:: docs/source/_static/images/django-plans-1.png
 
 .. image:: docs/source/_static/images/django-plans-2.png
 
 .. image:: docs/source/_static/images/django-plans-3.png
```

### Comparing `django-plans-1.1.0/README.rst` & `django-plans-1.2.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 * Customizable billing periods (plan pricing),
 * Order total calculation using customizable taxation policy (e.g. in EU calculating VAT based on seller/buyer countries and VIES)
 * Invoicing,
 * Account expiratons + E-mail remainders.
 
 Documentation: https://django-plans.readthedocs.org/
 
-Master branch: Support for Django +2.2, support for Python +3.6
+Master branch: Support for Django >=3.2, support for Python >=3.7
 
 .. image:: docs/source/_static/images/django-plans-1.png
 
 .. image:: docs/source/_static/images/django-plans-2.png
 
 .. image:: docs/source/_static/images/django-plans-3.png
```

### Comparing `django-plans-1.1.0/conftest.py` & `django-plans-1.2.0/conftest.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/demo/example/foo/fixtures/initial_data.json` & `django-plans-1.2.0/demo/example/foo/fixtures/initial_data.json`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/demo/example/foo/migrations/0001_initial.py` & `django-plans-1.2.0/demo/example/foo/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/demo/example/foo/templates/foo/foo_confirm_delete.html` & `django-plans-1.2.0/demo/example/foo/templates/foo/foo_confirm_delete.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/demo/example/foo/templates/foo/foo_form.html` & `django-plans-1.2.0/demo/example/foo/templates/foo/foo_form.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/demo/example/foo/templates/foo/foo_list.html` & `django-plans-1.2.0/demo/example/foo/templates/foo/foo_list.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/demo/example/foo/views.py` & `django-plans-1.2.0/demo/example/foo/views.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/demo/example/locale/en/LC_MESSAGES/django.po` & `django-plans-1.2.0/demo/example/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/demo/example/locale/pl/LC_MESSAGES/django.mo` & `django-plans-1.2.0/demo/example/locale/pl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/demo/example/locale/pl/LC_MESSAGES/django.po` & `django-plans-1.2.0/demo/example/locale/pl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/demo/example/locale/pt_BR/LC_MESSAGES/django.po` & `django-plans-1.2.0/demo/example/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/demo/example/locale/ru/LC_MESSAGES/django.mo` & `django-plans-1.2.0/demo/example/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/demo/example/locale/ru/LC_MESSAGES/django.po` & `django-plans-1.2.0/demo/example/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/demo/example/sample_plans/fixtures/initial_plan.json` & `django-plans-1.2.0/demo/example/sample_plans/fixtures/initial_plan.json`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/demo/example/sample_plans/fixtures/test_django-plans_auth.json` & `django-plans-1.2.0/demo/example/sample_plans/fixtures/test_django-plans_auth.json`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/demo/example/sample_plans/fixtures/test_django-plans_plans.json` & `django-plans-1.2.0/demo/example/sample_plans/fixtures/test_django-plans_plans.json`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/demo/example/sample_plans/migrations/0001_initial.py` & `django-plans-1.2.0/demo/example/sample_plans/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/demo/example/sample_plans/models.py` & `django-plans-1.2.0/demo/example/sample_plans/models.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/demo/example/sample_plans/templates/mail/change_plan_body.txt` & `django-plans-1.2.0/demo/example/sample_plans/templates/mail/change_plan_body.txt`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/demo/example/sample_plans/templates/mail/expired_account_body.txt` & `django-plans-1.2.0/demo/example/sample_plans/templates/mail/expired_account_body.txt`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/demo/example/sample_plans/templates/mail/extend_account_body.txt` & `django-plans-1.2.0/demo/example/sample_plans/templates/mail/extend_account_body.txt`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/demo/example/sample_plans/templates/mail/remind_expire_body.txt` & `django-plans-1.2.0/demo/example/sample_plans/templates/mail/remind_expire_body.txt`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/demo/example/sample_plans/templates/plans/account_activation.html` & `django-plans-1.2.0/demo/example/sample_plans/templates/plans/account_activation.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/demo/example/sample_plans/templates/plans/billing_info_create.html` & `django-plans-1.2.0/demo/example/sample_plans/templates/plans/billing_info_create.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/demo/example/sample_plans/templates/plans/billing_info_create_or_update.html` & `django-plans-1.2.0/demo/example/sample_plans/templates/plans/billing_info_create_or_update.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/demo/example/sample_plans/templates/plans/billing_info_update.html` & `django-plans-1.2.0/demo/example/sample_plans/templates/plans/billing_info_update.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/demo/example/sample_plans/templates/plans/create_order.html` & `django-plans-1.2.0/demo/example/sample_plans/templates/plans/create_order.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/demo/example/sample_plans/templates/plans/current.html` & `django-plans-1.2.0/demo/example/sample_plans/templates/plans/current.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/demo/example/sample_plans/templates/plans/expiration_messages.html` & `django-plans-1.2.0/demo/example/sample_plans/templates/plans/expiration_messages.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/demo/example/sample_plans/templates/plans/extend.html` & `django-plans-1.2.0/demo/example/sample_plans/templates/plans/extend.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/demo/example/sample_plans/templates/plans/invoices/PL_EN_layout.html` & `django-plans-1.2.0/demo/example/sample_plans/templates/plans/invoices/PL_EN_layout.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/demo/example/sample_plans/templates/plans/invoices/invoice_base.html` & `django-plans-1.2.0/demo/example/sample_plans/templates/plans/invoices/invoice_base.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/demo/example/sample_plans/templates/plans/order_detail.html` & `django-plans-1.2.0/demo/example/sample_plans/templates/plans/order_detail.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/demo/example/sample_plans/templates/plans/order_detail_table.html` & `django-plans-1.2.0/demo/example/sample_plans/templates/plans/order_detail_table.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/demo/example/sample_plans/templates/plans/order_list.html` & `django-plans-1.2.0/demo/example/sample_plans/templates/plans/order_list.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/demo/example/sample_plans/templates/plans/pagination.html` & `django-plans-1.2.0/demo/example/sample_plans/templates/plans/pagination.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/demo/example/sample_plans/templates/plans/plan_table.html` & `django-plans-1.2.0/demo/example/sample_plans/templates/plans/plan_table.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/demo/example/sample_plans/tests.py` & `django-plans-1.2.0/demo/example/sample_plans/tests.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/demo/example/settings.py` & `django-plans-1.2.0/demo/example/settings.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/demo/example/static/css/example.css` & `django-plans-1.2.0/demo/example/static/css/example.css`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/demo/example/static/img/messages/icon_error.png` & `django-plans-1.2.0/demo/example/static/img/messages/icon_error.png`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/demo/example/static/img/messages/icon_success.png` & `django-plans-1.2.0/demo/example/static/img/messages/icon_success.png`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/demo/example/templates/base.html` & `django-plans-1.2.0/demo/example/templates/base.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/demo/example/templates/home.html` & `django-plans-1.2.0/demo/example/templates/home.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/demo/example/templates/plans/billing_info_create.html` & `django-plans-1.2.0/demo/example/templates/plans/billing_info_create.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/demo/example/templates/plans/billing_info_update.html` & `django-plans-1.2.0/demo/example/templates/plans/billing_info_update.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/demo/example/templates/registration/login.html` & `django-plans-1.2.0/demo/example/templates/registration/login.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/demo/example/urls.py` & `django-plans-1.2.0/demo/example/urls.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/demo/example/wsgi.py` & `django-plans-1.2.0/demo/example/wsgi.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/demo/manage.py` & `django-plans-1.2.0/demo/manage.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/django_plans.egg-info/PKG-INFO` & `django-plans-1.2.0/django_plans.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-plans
-Version: 1.1.0
+Version: 1.2.0
 Summary: Pluggable django app for managing pricing plans with quotas and accounts expiration
 Home-page: https://github.com/cypreess/django-plans
 Author: Krzysztof Dorosz
 Author-email: cypreess@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Django
@@ -44,15 +44,15 @@
 * Customizable billing periods (plan pricing),
 * Order total calculation using customizable taxation policy (e.g. in EU calculating VAT based on seller/buyer countries and VIES)
 * Invoicing,
 * Account expiratons + E-mail remainders.
 
 Documentation: https://django-plans.readthedocs.org/
 
-Master branch: Support for Django +2.2, support for Python +3.6
+Master branch: Support for Django >=3.2, support for Python >=3.7
 
 .. image:: docs/source/_static/images/django-plans-1.png
 
 .. image:: docs/source/_static/images/django-plans-2.png
 
 .. image:: docs/source/_static/images/django-plans-3.png
```

### Comparing `django-plans-1.1.0/django_plans.egg-info/SOURCES.txt` & `django-plans-1.2.0/django_plans.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/docs/Makefile` & `django-plans-1.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/docs/source/_static/images/django-plans-1.png` & `django-plans-1.2.0/docs/source/_static/images/django-plans-1.png`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/docs/source/_static/images/django-plans-2.png` & `django-plans-1.2.0/docs/source/_static/images/django-plans-2.png`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/docs/source/_static/images/django-plans-3.png` & `django-plans-1.2.0/docs/source/_static/images/django-plans-3.png`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/docs/source/caveats.rst` & `django-plans-1.2.0/docs/source/caveats.rst`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/docs/source/conf.py` & `django-plans-1.2.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/docs/source/customize_models.rst` & `django-plans-1.2.0/docs/source/customize_models.rst`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/docs/source/index.rst` & `django-plans-1.2.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/docs/source/installation.rst` & `django-plans-1.2.0/docs/source/installation.rst`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/docs/source/integration.rst` & `django-plans-1.2.0/docs/source/integration.rst`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/docs/source/invoicing.rst` & `django-plans-1.2.0/docs/source/invoicing.rst`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/docs/source/plans.rst` & `django-plans-1.2.0/docs/source/plans.rst`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/docs/source/plans_change.rst` & `django-plans-1.2.0/docs/source/plans_change.rst`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/docs/source/plans_expiration.rst` & `django-plans-1.2.0/docs/source/plans_expiration.rst`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/docs/source/plans_recurrence.rst` & `django-plans-1.2.0/docs/source/plans_recurrence.rst`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/docs/source/quota_validators.rst` & `django-plans-1.2.0/docs/source/quota_validators.rst`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/docs/source/settings.rst` & `django-plans-1.2.0/docs/source/settings.rst`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/docs/source/south.rst` & `django-plans-1.2.0/docs/source/south.rst`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/docs/source/taxation.rst` & `django-plans-1.2.0/docs/source/taxation.rst`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/docs/source/templating.rst` & `django-plans-1.2.0/docs/source/templating.rst`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/plans/admin.py` & `django-plans-1.2.0/plans/admin.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/plans/base/models.py` & `django-plans-1.2.0/plans/base/models.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/plans/context_processors.py` & `django-plans-1.2.0/plans/context_processors.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/plans/contrib.py` & `django-plans-1.2.0/plans/contrib.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/plans/enumeration.py` & `django-plans-1.2.0/plans/enumeration.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/plans/fixtures/initial_plan.json` & `django-plans-1.2.0/plans/fixtures/initial_plan.json`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/plans/fixtures/test_django-plans_auth.json` & `django-plans-1.2.0/plans/fixtures/test_django-plans_auth.json`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/plans/fixtures/test_django-plans_plans.json` & `django-plans-1.2.0/plans/fixtures/test_django-plans_plans.json`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/plans/forms.py` & `django-plans-1.2.0/plans/forms.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/plans/listeners.py` & `django-plans-1.2.0/plans/listeners.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/plans/locale/en/LC_MESSAGES/django.po` & `django-plans-1.2.0/plans/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/plans/locale/pl/LC_MESSAGES/django.mo` & `django-plans-1.2.0/plans/locale/pl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/plans/locale/pl/LC_MESSAGES/django.po` & `django-plans-1.2.0/plans/locale/pl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/plans/locale/pt_BR/LC_MESSAGES/django.mo` & `django-plans-1.2.0/plans/locale/pt_BR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/plans/locale/pt_BR/LC_MESSAGES/django.po` & `django-plans-1.2.0/plans/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/plans/locale/ru/LC_MESSAGES/django.mo` & `django-plans-1.2.0/plans/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/plans/locale/ru/LC_MESSAGES/django.po` & `django-plans-1.2.0/plans/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/plans/management/commands/autorenew_accounts.py` & `django-plans-1.2.0/plans/management/commands/autorenew_accounts.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/plans/migrations/0001_initial.py` & `django-plans-1.2.0/plans/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/plans/migrations/0002_auto_20180901_1744.py` & `django-plans-1.2.0/plans/migrations/0002_auto_20180901_1744.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/plans/migrations/0003_make_plans_unique.py` & `django-plans-1.2.0/plans/migrations/0003_make_plans_unique.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/plans/migrations/0005_recurring_payments.py` & `django-plans-1.2.0/plans/migrations/0005_recurring_payments.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/plans/migrations/0006_auto_20200504_1541.py` & `django-plans-1.2.0/plans/migrations/0006_auto_20200504_1541.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/plans/migrations/0008_recurringuserplan_token_verified.py` & `django-plans-1.2.0/plans/migrations/0008_recurringuserplan_token_verified.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/plans/migrations/0010_auto_20220113_1317.py` & `django-plans-1.2.0/plans/migrations/0010_auto_20220113_1317.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/plans/migrations/0011_auto_20220208_1344.py` & `django-plans-1.2.0/plans/migrations/0011_auto_20220208_1344.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/plans/migrations/0012_planpricing_visible.py` & `django-plans-1.2.0/plans/migrations/0012_planpricing_visible.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/plans/migrations/0013_alter_recurringuserplan_has_automatic_renewal_and_more.py` & `django-plans-1.2.0/plans/migrations/0013_alter_recurringuserplan_has_automatic_renewal_and_more.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/plans/migrations/0014_recurringuserplan_has_automatic_renewal_backup_deprecated_to_renewal_triggered_by.py` & `django-plans-1.2.0/plans/migrations/0014_recurringuserplan_has_automatic_renewal_backup_deprecated_to_renewal_triggered_by.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/plans/mixins.py` & `django-plans-1.2.0/plans/mixins.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/plans/models.py` & `django-plans-1.2.0/plans/models.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/plans/plan_change.py` & `django-plans-1.2.0/plans/plan_change.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # coding=utf-8
 from decimal import Decimal
+from django.conf import settings
+from plans.importer import import_name
 
 
 class PlanChangePolicy(object):
     def _calculate_day_cost(self, plan, period):
         """
         Finds most fitted plan pricing for a given period, and calculate day cost
         """
@@ -92,7 +94,28 @@
             period * day_cost_diff * (self.UPGRADE_PERCENT_RATE / 100 + 1)
             + self.UPGRADE_CHARGE
         ).quantize(Decimal("1.00"))
         if cost is None or cost < self.FREE_UPGRADE:
             return None
         else:
             return cost
+
+
+def get_policy():
+    policy_class = getattr(
+        settings,
+        "PLANS_CHANGE_POLICY",
+        "plans.plan_change.StandardPlanChangePolicy",
+    )
+    return import_name(policy_class)()
+
+
+def get_change_price(userplan, plan):
+    policy = get_policy()
+
+    if userplan.expire is not None:
+        period = userplan.days_left()
+    else:
+        # Use the default period of the new plan
+        period = 30
+
+    return policy.get_change_price(userplan.plan, plan, period)
```

### Comparing `django-plans-1.1.0/plans/signals.py` & `django-plans-1.2.0/plans/signals.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/plans/tasks.py` & `django-plans-1.2.0/plans/tasks.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/plans/taxation/__init__.py` & `django-plans-1.2.0/plans/taxation/__init__.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/plans/taxation/eu.py` & `django-plans-1.2.0/plans/taxation/eu.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/plans/taxation/ru.py` & `django-plans-1.2.0/plans/taxation/ru.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/plans/templates/mail/change_plan_body.txt` & `django-plans-1.2.0/plans/templates/mail/change_plan_body.txt`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/plans/templates/mail/expired_account_body.txt` & `django-plans-1.2.0/plans/templates/mail/expired_account_body.txt`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/plans/templates/mail/extend_account_body.txt` & `django-plans-1.2.0/plans/templates/mail/extend_account_body.txt`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/plans/templates/mail/remind_expire_body.txt` & `django-plans-1.2.0/plans/templates/mail/remind_expire_body.txt`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/plans/templates/plans/account_activation.html` & `django-plans-1.2.0/plans/templates/plans/account_activation.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/plans/templates/plans/billing_info_create_or_update.html` & `django-plans-1.2.0/plans/templates/plans/billing_info_create_or_update.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/plans/templates/plans/create_order.html` & `django-plans-1.2.0/plans/templates/plans/create_order.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/plans/templates/plans/current.html` & `django-plans-1.2.0/plans/templates/plans/current.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/plans/templates/plans/expiration_messages.html` & `django-plans-1.2.0/plans/templates/plans/expiration_messages.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/plans/templates/plans/extend.html` & `django-plans-1.2.0/plans/templates/plans/extend.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/plans/templates/plans/invoices/PL_EN_layout.html` & `django-plans-1.2.0/plans/templates/plans/invoices/PL_EN_layout.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/plans/templates/plans/invoices/invoice_base.html` & `django-plans-1.2.0/plans/templates/plans/invoices/invoice_base.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/plans/templates/plans/order_detail.html` & `django-plans-1.2.0/plans/templates/plans/order_detail.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/plans/templates/plans/order_detail_table.html` & `django-plans-1.2.0/plans/templates/plans/order_detail_table.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/plans/templates/plans/order_list.html` & `django-plans-1.2.0/plans/templates/plans/order_list.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/plans/templates/plans/pagination.html` & `django-plans-1.2.0/plans/templates/plans/pagination.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/plans/templates/plans/plan_table.html` & `django-plans-1.2.0/plans/templates/plans/plan_table.html`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/plans/tests/test_autorenew_accounts.py` & `django-plans-1.2.0/plans/tests/test_autorenew_accounts.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/plans/tests/test_views.py` & `django-plans-1.2.0/plans/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/plans/tests/tests.py` & `django-plans-1.2.0/plans/tests/tests.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/plans/urls.py` & `django-plans-1.2.0/plans/urls.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/plans/utils.py` & `django-plans-1.2.0/plans/utils.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/plans/validators.py` & `django-plans-1.2.0/plans/validators.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/plans/views.py` & `django-plans-1.2.0/plans/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 )
 from plans.forms import BillingInfoForm, CreateOrderForm, FakePaymentsForm
 from plans.importer import import_name
 from plans.mixins import LoginRequired
 from plans.signals import order_started
 from plans.utils import get_currency
 from plans.validators import plan_validation
+from plans.plan_change import get_change_price
 
 UserPlan = AbstractUserPlan.get_concrete_model()
 PlanPricing = AbstractPlanPricing.get_concrete_model()
 Plan = AbstractPlan.get_concrete_model()
 Order = AbstractOrder.get_concrete_model()
 BillingInfo = AbstractBillingInfo.get_concrete_model()
 Quota = AbstractQuota.get_concrete_model()
@@ -336,35 +337,16 @@
             Plan,
             Q(pk=self.kwargs["pk"])
             & Q(available=True, visible=True)
             & (Q(customized=self.request.user) | Q(customized__isnull=True)),
         )
         self.pricing = None
 
-    def get_policy(self):
-        policy_class = getattr(
-            settings,
-            "PLANS_CHANGE_POLICY",
-            "plans.plan_change.StandardPlanChangePolicy",
-        )
-        return import_name(policy_class)()
-
     def get_price(self):
-        policy = self.get_policy()
-        userplan = self.request.user.userplan
-
-        if userplan.expire is not None:
-            period = self.request.user.userplan.days_left()
-        else:
-            # Use the default period of the new plan
-            period = 30
-
-        return policy.get_change_price(
-            self.request.user.userplan.plan, self.plan, period
-        )
+        return get_change_price(self.request.user.userplan, self.plan)
 
     def get_context_data(self, **kwargs):
         context = super(CreateOrderView, self).get_context_data(**kwargs)
         self.get_all_context()
 
         price = self.get_price()
         context["plan"] = self.plan
```

### Comparing `django-plans-1.1.0/plans_i18n/README.rst` & `django-plans-1.2.0/plans_i18n/README.rst`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/plans_i18n/admin.py` & `django-plans-1.2.0/plans_i18n/admin.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/plans_i18n/translation.py` & `django-plans-1.2.0/plans_i18n/translation.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/setup.py` & `django-plans-1.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `django-plans-1.1.0/tox.ini` & `django-plans-1.2.0/tox.ini`

 * *Files identical despite different names*

