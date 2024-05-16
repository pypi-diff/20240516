# Comparing `tmp/lago-python-client-1.2.0.tar.gz` & `tmp/lago-python-client-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/lago-python-client/lago-python-client/dist/.tmp-qs5bfr58/lago-python-client-1.2.0.tar", last modified: Mon Apr 22 08:44:34 2024, max compression
+gzip compressed data, was "/home/runner/work/lago-python-client/lago-python-client/dist/.tmp-s0vs_dq5/lago-python-client-1.3.0.tar", last modified: Thu May 16 18:03:09 2024, max compression
```

## Comparing `lago-python-client-1.2.0.tar` & `lago-python-client-1.3.0.tar`

### file list

```diff
@@ -1,141 +1,141 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:44:34.000000 lago-python-client-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3141 2024-04-22 08:44:34.000000 lago-python-client-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:44:34.000000 lago-python-client-1.2.0/lago_python_client/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:44:34.000000 lago-python-client-1.2.0/lago_python_client/add_ons/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/add_ons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/add_ons/clients.py
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/base_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/base_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:44:34.000000 lago-python-client-1.2.0/lago_python_client/billable_metrics/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/billable_metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/billable_metrics/clients.py
--rw-r--r--   0 runner    (1001) docker     (127)     4650 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:44:34.000000 lago-python-client-1.2.0/lago_python_client/coupons/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/coupons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/coupons/clients.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:44:34.000000 lago-python-client-1.2.0/lago_python_client/credit_notes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/credit_notes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2722 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/credit_notes/clients.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:44:34.000000 lago-python-client-1.2.0/lago_python_client/customers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/customers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3459 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/customers/clients.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:44:34.000000 lago-python-client-1.2.0/lago_python_client/events/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/events/clients.py
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:44:34.000000 lago-python-client-1.2.0/lago_python_client/fees/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/fees/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/fees/clients.py
--rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/functools_ext.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:44:34.000000 lago-python-client-1.2.0/lago_python_client/gross_revenues/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/gross_revenues/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/gross_revenues/clients.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:44:34.000000 lago-python-client-1.2.0/lago_python_client/invoice_collections/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/invoice_collections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/invoice_collections/clients.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:44:34.000000 lago-python-client-1.2.0/lago_python_client/invoiced_usages/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/invoiced_usages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/invoiced_usages/clients.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:44:34.000000 lago-python-client-1.2.0/lago_python_client/invoices/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/invoices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4069 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/invoices/clients.py
--rw-r--r--   0 runner    (1001) docker     (127)     5527 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/mixins.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:44:34.000000 lago-python-client-1.2.0/lago_python_client/models/
--rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/models/add_on.py
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/models/applied_coupon.py
--rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/models/billable_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/models/charge.py
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/models/coupon.py
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/models/credit.py
--rw-r--r--   0 runner    (1001) docker     (127)     3051 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/models/credit_note.py
--rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/models/customer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/models/customer_usage.py
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/models/event.py
--rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/models/fee.py
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/models/gross_revenue.py
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/models/group.py
--rw-r--r--   0 runner    (1001) docker     (127)     2521 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/models/invoice.py
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/models/invoice_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/models/invoice_item.py
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/models/invoiced_usage.py
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/models/minimum_commitment.py
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/models/mrr.py
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/models/organization.py
--rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/models/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/models/subscription.py
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/models/tax.py
--rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/models/wallet.py
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/models/wallet_transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/models/webhook_endpoint.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:44:34.000000 lago-python-client-1.2.0/lago_python_client/mrrs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/mrrs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/mrrs/clients.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:44:34.000000 lago-python-client-1.2.0/lago_python_client/organizations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/organizations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/organizations/clients.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:44:34.000000 lago-python-client-1.2.0/lago_python_client/plans/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/plans/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/plans/clients.py
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:44:34.000000 lago-python-client-1.2.0/lago_python_client/services/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/services/json.py
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/services/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     5405 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/services/response.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:44:34.000000 lago-python-client-1.2.0/lago_python_client/subscriptions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/subscriptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/subscriptions/clients.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:44:34.000000 lago-python-client-1.2.0/lago_python_client/taxes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/taxes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/taxes/clients.py
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:44:34.000000 lago-python-client-1.2.0/lago_python_client/wallets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/wallets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/wallets/clients.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:44:34.000000 lago-python-client-1.2.0/lago_python_client/webhook_endpoints/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/webhook_endpoints/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/webhook_endpoints/clients.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:44:34.000000 lago-python-client-1.2.0/lago_python_client/webhooks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/webhooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/lago_python_client/webhooks/clients.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:44:34.000000 lago-python-client-1.2.0/lago_python_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3141 2024-04-22 08:44:34.000000 lago-python-client-1.2.0/lago_python_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5227 2024-04-22 08:44:34.000000 lago-python-client-1.2.0/lago_python_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 08:44:34.000000 lago-python-client-1.2.0/lago_python_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-22 08:44:34.000000 lago-python-client-1.2.0/lago_python_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-22 08:44:34.000000 lago-python-client-1.2.0/lago_python_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-04-22 08:44:34.000000 lago-python-client-1.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 08:44:34.000000 lago-python-client-1.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5494 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/tests/test_add_on_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     4120 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/tests/test_applied_coupon_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     5774 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/tests/test_billable_metric_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     5437 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/tests/test_coupon_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     5888 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/tests/test_credit_note_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     7133 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/tests/test_customer_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     4340 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/tests/test_event_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      985 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/tests/test_fee_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/tests/test_functools_ext.py
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/tests/test_gross_revenue_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/tests/test_group_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     8220 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/tests/test_invoice_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/tests/test_invoice_collection_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/tests/test_invoiced_usage_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/tests/test_json_services.py
--rw-r--r--   0 runner    (1001) docker     (127)      933 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/tests/test_mrr_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/tests/test_organization_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     8762 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/tests/test_plan_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/tests/test_request_services.py
--rw-r--r--   0 runner    (1001) docker     (127)     5392 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/tests/test_response_services.py
--rw-r--r--   0 runner    (1001) docker     (127)     7142 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/tests/test_subscription_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     4985 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/tests/test_tax_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     5692 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/tests/test_wallet_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/tests/test_wallet_transaction_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/tests/test_webhook_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     4907 2024-04-22 08:44:28.000000 lago-python-client-1.2.0/tests/test_webhook_endpoint_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:03:09.000000 lago-python-client-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-16 18:03:00.000000 lago-python-client-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3141 2024-05-16 18:03:09.000000 lago-python-client-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-05-16 18:03:00.000000 lago-python-client-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:03:09.000000 lago-python-client-1.3.0/lago_python_client/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-16 18:03:00.000000 lago-python-client-1.3.0/lago_python_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:03:09.000000 lago-python-client-1.3.0/lago_python_client/add_ons/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 18:03:00.000000 lago-python-client-1.3.0/lago_python_client/add_ons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-16 18:03:00.000000 lago-python-client-1.3.0/lago_python_client/add_ons/clients.py
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-16 18:03:00.000000 lago-python-client-1.3.0/lago_python_client/base_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-16 18:03:00.000000 lago-python-client-1.3.0/lago_python_client/base_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:03:09.000000 lago-python-client-1.3.0/lago_python_client/billable_metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 18:03:00.000000 lago-python-client-1.3.0/lago_python_client/billable_metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-05-16 18:03:00.000000 lago-python-client-1.3.0/lago_python_client/billable_metrics/clients.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4650 2024-05-16 18:03:00.000000 lago-python-client-1.3.0/lago_python_client/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:03:09.000000 lago-python-client-1.3.0/lago_python_client/coupons/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 18:03:00.000000 lago-python-client-1.3.0/lago_python_client/coupons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-05-16 18:03:00.000000 lago-python-client-1.3.0/lago_python_client/coupons/clients.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:03:09.000000 lago-python-client-1.3.0/lago_python_client/credit_notes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 18:03:00.000000 lago-python-client-1.3.0/lago_python_client/credit_notes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2722 2024-05-16 18:03:00.000000 lago-python-client-1.3.0/lago_python_client/credit_notes/clients.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:03:09.000000 lago-python-client-1.3.0/lago_python_client/customers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 18:03:00.000000 lago-python-client-1.3.0/lago_python_client/customers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3459 2024-05-16 18:03:00.000000 lago-python-client-1.3.0/lago_python_client/customers/clients.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:03:09.000000 lago-python-client-1.3.0/lago_python_client/events/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 18:03:00.000000 lago-python-client-1.3.0/lago_python_client/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-05-16 18:03:00.000000 lago-python-client-1.3.0/lago_python_client/events/clients.py
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-05-16 18:03:00.000000 lago-python-client-1.3.0/lago_python_client/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:03:09.000000 lago-python-client-1.3.0/lago_python_client/fees/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 18:03:00.000000 lago-python-client-1.3.0/lago_python_client/fees/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-16 18:03:00.000000 lago-python-client-1.3.0/lago_python_client/fees/clients.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-05-16 18:03:00.000000 lago-python-client-1.3.0/lago_python_client/functools_ext.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:03:09.000000 lago-python-client-1.3.0/lago_python_client/gross_revenues/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 18:03:00.000000 lago-python-client-1.3.0/lago_python_client/gross_revenues/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-05-16 18:03:00.000000 lago-python-client-1.3.0/lago_python_client/gross_revenues/clients.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:03:09.000000 lago-python-client-1.3.0/lago_python_client/invoice_collections/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 18:03:00.000000 lago-python-client-1.3.0/lago_python_client/invoice_collections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-05-16 18:03:00.000000 lago-python-client-1.3.0/lago_python_client/invoice_collections/clients.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:03:09.000000 lago-python-client-1.3.0/lago_python_client/invoiced_usages/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 18:03:00.000000 lago-python-client-1.3.0/lago_python_client/invoiced_usages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-05-16 18:03:00.000000 lago-python-client-1.3.0/lago_python_client/invoiced_usages/clients.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:03:09.000000 lago-python-client-1.3.0/lago_python_client/invoices/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 18:03:00.000000 lago-python-client-1.3.0/lago_python_client/invoices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4069 2024-05-16 18:03:00.000000 lago-python-client-1.3.0/lago_python_client/invoices/clients.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5527 2024-05-16 18:03:00.000000 lago-python-client-1.3.0/lago_python_client/mixins.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:03:09.000000 lago-python-client-1.3.0/lago_python_client/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-05-16 18:03:00.000000 lago-python-client-1.3.0/lago_python_client/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-16 18:03:00.000000 lago-python-client-1.3.0/lago_python_client/models/add_on.py
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-16 18:03:00.000000 lago-python-client-1.3.0/lago_python_client/models/applied_coupon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-05-16 18:03:00.000000 lago-python-client-1.3.0/lago_python_client/models/billable_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-05-16 18:03:00.000000 lago-python-client-1.3.0/lago_python_client/models/charge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-05-16 18:03:00.000000 lago-python-client-1.3.0/lago_python_client/models/coupon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-16 18:03:00.000000 lago-python-client-1.3.0/lago_python_client/models/credit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3051 2024-05-16 18:03:00.000000 lago-python-client-1.3.0/lago_python_client/models/credit_note.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-05-16 18:03:00.000000 lago-python-client-1.3.0/lago_python_client/models/customer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-05-16 18:03:00.000000 lago-python-client-1.3.0/lago_python_client/models/customer_usage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-16 18:03:00.000000 lago-python-client-1.3.0/lago_python_client/models/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-05-16 18:03:00.000000 lago-python-client-1.3.0/lago_python_client/models/fee.py
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-16 18:03:00.000000 lago-python-client-1.3.0/lago_python_client/models/gross_revenue.py
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-16 18:03:00.000000 lago-python-client-1.3.0/lago_python_client/models/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2521 2024-05-16 18:03:00.000000 lago-python-client-1.3.0/lago_python_client/models/invoice.py
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-16 18:03:00.000000 lago-python-client-1.3.0/lago_python_client/models/invoice_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-16 18:03:00.000000 lago-python-client-1.3.0/lago_python_client/models/invoice_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-05-16 18:03:00.000000 lago-python-client-1.3.0/lago_python_client/models/invoiced_usage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-16 18:03:00.000000 lago-python-client-1.3.0/lago_python_client/models/minimum_commitment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-16 18:03:00.000000 lago-python-client-1.3.0/lago_python_client/models/mrr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-05-16 18:03:00.000000 lago-python-client-1.3.0/lago_python_client/models/organization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1751 2024-05-16 18:03:00.000000 lago-python-client-1.3.0/lago_python_client/models/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-05-16 18:03:00.000000 lago-python-client-1.3.0/lago_python_client/models/subscription.py
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-16 18:03:00.000000 lago-python-client-1.3.0/lago_python_client/models/tax.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-05-16 18:03:00.000000 lago-python-client-1.3.0/lago_python_client/models/wallet.py
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-16 18:03:00.000000 lago-python-client-1.3.0/lago_python_client/models/wallet_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-16 18:03:00.000000 lago-python-client-1.3.0/lago_python_client/models/webhook_endpoint.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:03:09.000000 lago-python-client-1.3.0/lago_python_client/mrrs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 18:03:00.000000 lago-python-client-1.3.0/lago_python_client/mrrs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-05-16 18:03:00.000000 lago-python-client-1.3.0/lago_python_client/mrrs/clients.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:03:09.000000 lago-python-client-1.3.0/lago_python_client/organizations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 18:03:00.000000 lago-python-client-1.3.0/lago_python_client/organizations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-16 18:03:00.000000 lago-python-client-1.3.0/lago_python_client/organizations/clients.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:03:09.000000 lago-python-client-1.3.0/lago_python_client/plans/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 18:03:00.000000 lago-python-client-1.3.0/lago_python_client/plans/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-16 18:03:00.000000 lago-python-client-1.3.0/lago_python_client/plans/clients.py
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-16 18:03:00.000000 lago-python-client-1.3.0/lago_python_client/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:03:09.000000 lago-python-client-1.3.0/lago_python_client/services/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 18:03:00.000000 lago-python-client-1.3.0/lago_python_client/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2270 2024-05-16 18:03:00.000000 lago-python-client-1.3.0/lago_python_client/services/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-05-16 18:03:00.000000 lago-python-client-1.3.0/lago_python_client/services/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5405 2024-05-16 18:03:00.000000 lago-python-client-1.3.0/lago_python_client/services/response.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:03:09.000000 lago-python-client-1.3.0/lago_python_client/subscriptions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 18:03:00.000000 lago-python-client-1.3.0/lago_python_client/subscriptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-16 18:03:00.000000 lago-python-client-1.3.0/lago_python_client/subscriptions/clients.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:03:09.000000 lago-python-client-1.3.0/lago_python_client/taxes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 18:03:00.000000 lago-python-client-1.3.0/lago_python_client/taxes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-16 18:03:00.000000 lago-python-client-1.3.0/lago_python_client/taxes/clients.py
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-16 18:03:00.000000 lago-python-client-1.3.0/lago_python_client/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:03:09.000000 lago-python-client-1.3.0/lago_python_client/wallets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 18:03:00.000000 lago-python-client-1.3.0/lago_python_client/wallets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-05-16 18:03:00.000000 lago-python-client-1.3.0/lago_python_client/wallets/clients.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:03:09.000000 lago-python-client-1.3.0/lago_python_client/webhook_endpoints/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 18:03:00.000000 lago-python-client-1.3.0/lago_python_client/webhook_endpoints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-16 18:03:00.000000 lago-python-client-1.3.0/lago_python_client/webhook_endpoints/clients.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:03:09.000000 lago-python-client-1.3.0/lago_python_client/webhooks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 18:03:00.000000 lago-python-client-1.3.0/lago_python_client/webhooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-05-16 18:03:00.000000 lago-python-client-1.3.0/lago_python_client/webhooks/clients.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:03:09.000000 lago-python-client-1.3.0/lago_python_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3141 2024-05-16 18:03:08.000000 lago-python-client-1.3.0/lago_python_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5227 2024-05-16 18:03:08.000000 lago-python-client-1.3.0/lago_python_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 18:03:08.000000 lago-python-client-1.3.0/lago_python_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-16 18:03:08.000000 lago-python-client-1.3.0/lago_python_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-16 18:03:08.000000 lago-python-client-1.3.0/lago_python_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-16 18:03:00.000000 lago-python-client-1.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-05-16 18:03:09.000000 lago-python-client-1.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 18:03:09.000000 lago-python-client-1.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 18:03:00.000000 lago-python-client-1.3.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5494 2024-05-16 18:03:00.000000 lago-python-client-1.3.0/tests/test_add_on_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4120 2024-05-16 18:03:00.000000 lago-python-client-1.3.0/tests/test_applied_coupon_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5774 2024-05-16 18:03:00.000000 lago-python-client-1.3.0/tests/test_billable_metric_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-16 18:03:00.000000 lago-python-client-1.3.0/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5437 2024-05-16 18:03:00.000000 lago-python-client-1.3.0/tests/test_coupon_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5888 2024-05-16 18:03:00.000000 lago-python-client-1.3.0/tests/test_credit_note_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7133 2024-05-16 18:03:00.000000 lago-python-client-1.3.0/tests/test_customer_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4340 2024-05-16 18:03:00.000000 lago-python-client-1.3.0/tests/test_event_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-05-16 18:03:00.000000 lago-python-client-1.3.0/tests/test_fee_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-05-16 18:03:00.000000 lago-python-client-1.3.0/tests/test_functools_ext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-05-16 18:03:00.000000 lago-python-client-1.3.0/tests/test_gross_revenue_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-05-16 18:03:00.000000 lago-python-client-1.3.0/tests/test_group_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8220 2024-05-16 18:03:00.000000 lago-python-client-1.3.0/tests/test_invoice_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-16 18:03:00.000000 lago-python-client-1.3.0/tests/test_invoice_collection_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-05-16 18:03:00.000000 lago-python-client-1.3.0/tests/test_invoiced_usage_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-05-16 18:03:00.000000 lago-python-client-1.3.0/tests/test_json_services.py
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-05-16 18:03:00.000000 lago-python-client-1.3.0/tests/test_mrr_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-05-16 18:03:00.000000 lago-python-client-1.3.0/tests/test_organization_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8762 2024-05-16 18:03:00.000000 lago-python-client-1.3.0/tests/test_plan_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-05-16 18:03:00.000000 lago-python-client-1.3.0/tests/test_request_services.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5392 2024-05-16 18:03:00.000000 lago-python-client-1.3.0/tests/test_response_services.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7142 2024-05-16 18:03:00.000000 lago-python-client-1.3.0/tests/test_subscription_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4985 2024-05-16 18:03:00.000000 lago-python-client-1.3.0/tests/test_tax_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5688 2024-05-16 18:03:00.000000 lago-python-client-1.3.0/tests/test_wallet_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-05-16 18:03:00.000000 lago-python-client-1.3.0/tests/test_wallet_transaction_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-05-16 18:03:00.000000 lago-python-client-1.3.0/tests/test_webhook_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4907 2024-05-16 18:03:00.000000 lago-python-client-1.3.0/tests/test_webhook_endpoint_client.py
```

### Comparing `lago-python-client-1.2.0/LICENSE` & `lago-python-client-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.2.0/PKG-INFO` & `lago-python-client-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lago-python-client
-Version: 1.2.0
+Version: 1.3.0
 Summary: Lago Python API Client
 Home-page: https://github.com/getlago/lago-python-client
 Author: Lovro Colic
 Author-email: lovro@getlago.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `lago-python-client-1.2.0/README.md` & `lago-python-client-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.2.0/lago_python_client/add_ons/clients.py` & `lago-python-client-1.3.0/lago_python_client/add_ons/clients.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.2.0/lago_python_client/base_client.py` & `lago-python-client-1.3.0/lago_python_client/base_client.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.2.0/lago_python_client/billable_metrics/clients.py` & `lago-python-client-1.3.0/lago_python_client/billable_metrics/clients.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.2.0/lago_python_client/client.py` & `lago-python-client-1.3.0/lago_python_client/client.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.2.0/lago_python_client/coupons/clients.py` & `lago-python-client-1.3.0/lago_python_client/coupons/clients.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.2.0/lago_python_client/credit_notes/clients.py` & `lago-python-client-1.3.0/lago_python_client/credit_notes/clients.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.2.0/lago_python_client/customers/clients.py` & `lago-python-client-1.3.0/lago_python_client/customers/clients.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.2.0/lago_python_client/events/clients.py` & `lago-python-client-1.3.0/lago_python_client/events/clients.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.2.0/lago_python_client/exceptions.py` & `lago-python-client-1.3.0/lago_python_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.2.0/lago_python_client/functools_ext.py` & `lago-python-client-1.3.0/lago_python_client/functools_ext.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.2.0/lago_python_client/gross_revenues/clients.py` & `lago-python-client-1.3.0/lago_python_client/gross_revenues/clients.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.2.0/lago_python_client/invoice_collections/clients.py` & `lago-python-client-1.3.0/lago_python_client/invoice_collections/clients.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.2.0/lago_python_client/invoiced_usages/clients.py` & `lago-python-client-1.3.0/lago_python_client/invoiced_usages/clients.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.2.0/lago_python_client/invoices/clients.py` & `lago-python-client-1.3.0/lago_python_client/invoices/clients.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.2.0/lago_python_client/mixins.py` & `lago-python-client-1.3.0/lago_python_client/mixins.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.2.0/lago_python_client/models/__init__.py` & `lago-python-client-1.3.0/lago_python_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.2.0/lago_python_client/models/add_on.py` & `lago-python-client-1.3.0/lago_python_client/models/add_on.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.2.0/lago_python_client/models/applied_coupon.py` & `lago-python-client-1.3.0/lago_python_client/models/applied_coupon.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.2.0/lago_python_client/models/billable_metric.py` & `lago-python-client-1.3.0/lago_python_client/models/billable_metric.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.2.0/lago_python_client/models/charge.py` & `lago-python-client-1.3.0/lago_python_client/models/charge.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.2.0/lago_python_client/models/coupon.py` & `lago-python-client-1.3.0/lago_python_client/models/coupon.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.2.0/lago_python_client/models/credit.py` & `lago-python-client-1.3.0/lago_python_client/models/credit.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.2.0/lago_python_client/models/credit_note.py` & `lago-python-client-1.3.0/lago_python_client/models/credit_note.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.2.0/lago_python_client/models/customer.py` & `lago-python-client-1.3.0/lago_python_client/models/customer.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.2.0/lago_python_client/models/customer_usage.py` & `lago-python-client-1.3.0/lago_python_client/models/customer_usage.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.2.0/lago_python_client/models/event.py` & `lago-python-client-1.3.0/lago_python_client/models/event.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.2.0/lago_python_client/models/fee.py` & `lago-python-client-1.3.0/lago_python_client/models/fee.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.2.0/lago_python_client/models/invoice.py` & `lago-python-client-1.3.0/lago_python_client/models/invoice.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.2.0/lago_python_client/models/minimum_commitment.py` & `lago-python-client-1.3.0/lago_python_client/models/minimum_commitment.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.2.0/lago_python_client/models/organization.py` & `lago-python-client-1.3.0/lago_python_client/models/organization.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.2.0/lago_python_client/models/plan.py` & `lago-python-client-1.3.0/lago_python_client/models/plan.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.2.0/lago_python_client/models/subscription.py` & `lago-python-client-1.3.0/lago_python_client/models/subscription.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.2.0/lago_python_client/models/tax.py` & `lago-python-client-1.3.0/lago_python_client/models/tax.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.2.0/lago_python_client/models/wallet.py` & `lago-python-client-1.3.0/lago_python_client/models/wallet.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,26 +3,26 @@
 from lago_python_client.base_model import BaseModel
 
 from ..base_model import BaseResponseModel
 
 
 class RecurringTransactionRule(BaseModel):
     lago_id: Optional[str]
-    rule_type: Optional[str]
     interval: Optional[str]
     threshold_credits: Optional[str]
+    trigger: Optional[str]
     paid_credits: Optional[str]
     granted_credits: Optional[str]
 
 
 class RecurringTransactionRuleResponse(BaseModel):
     lago_id: Optional[str]
-    rule_type: Optional[str]
     interval: Optional[str]
     threshold_credits: Optional[str]
+    trigger: Optional[str]
     paid_credits: Optional[str]
     granted_credits: Optional[str]
     created_at: Optional[str]
 
 
 class RecurringTransactionRuleList(BaseModel):
     __root__: List[RecurringTransactionRule]
```

### Comparing `lago-python-client-1.2.0/lago_python_client/mrrs/clients.py` & `lago-python-client-1.3.0/lago_python_client/mrrs/clients.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.2.0/lago_python_client/plans/clients.py` & `lago-python-client-1.3.0/lago_python_client/plans/clients.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.2.0/lago_python_client/services/json.py` & `lago-python-client-1.3.0/lago_python_client/services/json.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.2.0/lago_python_client/services/request.py` & `lago-python-client-1.3.0/lago_python_client/services/request.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.2.0/lago_python_client/services/response.py` & `lago-python-client-1.3.0/lago_python_client/services/response.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.2.0/lago_python_client/subscriptions/clients.py` & `lago-python-client-1.3.0/lago_python_client/subscriptions/clients.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.2.0/lago_python_client/taxes/clients.py` & `lago-python-client-1.3.0/lago_python_client/taxes/clients.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.2.0/lago_python_client/wallets/clients.py` & `lago-python-client-1.3.0/lago_python_client/wallets/clients.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.2.0/lago_python_client/webhook_endpoints/clients.py` & `lago-python-client-1.3.0/lago_python_client/webhook_endpoints/clients.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.2.0/lago_python_client/webhooks/clients.py` & `lago-python-client-1.3.0/lago_python_client/webhooks/clients.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.2.0/lago_python_client.egg-info/PKG-INFO` & `lago-python-client-1.3.0/lago_python_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lago-python-client
-Version: 1.2.0
+Version: 1.3.0
 Summary: Lago Python API Client
 Home-page: https://github.com/getlago/lago-python-client
 Author: Lovro Colic
 Author-email: lovro@getlago.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `lago-python-client-1.2.0/lago_python_client.egg-info/SOURCES.txt` & `lago-python-client-1.3.0/lago_python_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.2.0/setup.cfg` & `lago-python-client-1.3.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.2.0/tests/test_add_on_client.py` & `lago-python-client-1.3.0/tests/test_add_on_client.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.2.0/tests/test_applied_coupon_client.py` & `lago-python-client-1.3.0/tests/test_applied_coupon_client.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.2.0/tests/test_billable_metric_client.py` & `lago-python-client-1.3.0/tests/test_billable_metric_client.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.2.0/tests/test_coupon_client.py` & `lago-python-client-1.3.0/tests/test_coupon_client.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.2.0/tests/test_credit_note_client.py` & `lago-python-client-1.3.0/tests/test_credit_note_client.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.2.0/tests/test_customer_client.py` & `lago-python-client-1.3.0/tests/test_customer_client.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.2.0/tests/test_event_client.py` & `lago-python-client-1.3.0/tests/test_event_client.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.2.0/tests/test_fee_client.py` & `lago-python-client-1.3.0/tests/test_fee_client.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.2.0/tests/test_functools_ext.py` & `lago-python-client-1.3.0/tests/test_functools_ext.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.2.0/tests/test_gross_revenue_client.py` & `lago-python-client-1.3.0/tests/test_gross_revenue_client.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.2.0/tests/test_group_client.py` & `lago-python-client-1.3.0/tests/test_group_client.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.2.0/tests/test_invoice_client.py` & `lago-python-client-1.3.0/tests/test_invoice_client.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.2.0/tests/test_invoice_collection_client.py` & `lago-python-client-1.3.0/tests/test_invoice_collection_client.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.2.0/tests/test_invoiced_usage_client.py` & `lago-python-client-1.3.0/tests/test_invoiced_usage_client.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.2.0/tests/test_json_services.py` & `lago-python-client-1.3.0/tests/test_json_services.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.2.0/tests/test_mrr_client.py` & `lago-python-client-1.3.0/tests/test_mrr_client.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.2.0/tests/test_organization_client.py` & `lago-python-client-1.3.0/tests/test_organization_client.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.2.0/tests/test_plan_client.py` & `lago-python-client-1.3.0/tests/test_plan_client.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.2.0/tests/test_request_services.py` & `lago-python-client-1.3.0/tests/test_request_services.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.2.0/tests/test_response_services.py` & `lago-python-client-1.3.0/tests/test_response_services.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.2.0/tests/test_subscription_client.py` & `lago-python-client-1.3.0/tests/test_subscription_client.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.2.0/tests/test_tax_client.py` & `lago-python-client-1.3.0/tests/test_tax_client.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.2.0/tests/test_wallet_client.py` & `lago-python-client-1.3.0/tests/test_wallet_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from lago_python_client.client import Client
 from lago_python_client.exceptions import LagoApiError
 from lago_python_client.models import Wallet, RecurringTransactionRule, RecurringTransactionRuleList
 
 
 def wallet_object():
     rule = RecurringTransactionRule(
-        rule_type='interval',
+        trigger='interval',
         interval='monthly',
         paid_credits='105.0',
         granted_credits='105.0',
     )
     rules_list = RecurringTransactionRuleList(__root__=[rule])
     return Wallet(
         name='name',
@@ -46,15 +46,15 @@
     client = Client(api_key='886fe239-927d-4072-ab72-6dd345e8dd0d')
 
     httpx_mock.add_response(method='POST', url='https://api.getlago.com/api/v1/wallets', content=mock_response())
     response = client.wallets.create(wallet_object())
 
     assert response.lago_id == 'b7ab2926-1de8-4428-9bcd-779314ac129b'
     assert response.recurring_transaction_rules.__root__[0].lago_id == '12345'
-    assert response.recurring_transaction_rules.__root__[0].rule_type == 'interval'
+    assert response.recurring_transaction_rules.__root__[0].trigger == 'interval'
     assert response.recurring_transaction_rules.__root__[0].interval == 'monthly'
 
 
 def test_invalid_create_wallet_request(httpx_mock: HTTPXMock):
     client = Client(api_key='invalid')
 
     httpx_mock.add_response(method='POST', url='https://api.getlago.com/api/v1/wallets', status_code=401, content=b'')
```

### Comparing `lago-python-client-1.2.0/tests/test_wallet_transaction_client.py` & `lago-python-client-1.3.0/tests/test_wallet_transaction_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 from lago_python_client.models import WalletTransaction
 
 
 def wallet_transaction_object():
     return WalletTransaction(
         wallet_id='123',
         paid_credits='10',
-        granted_credits='10'
+        granted_credits='10',
+        voided_credits='0'
     )
 
 
 def mock_response():
     this_dir = os.path.dirname(os.path.abspath(__file__))
     data_path = os.path.join(this_dir, 'fixtures/wallet_transaction.json')
```

### Comparing `lago-python-client-1.2.0/tests/test_webhook_client.py` & `lago-python-client-1.3.0/tests/test_webhook_client.py`

 * *Files identical despite different names*

### Comparing `lago-python-client-1.2.0/tests/test_webhook_endpoint_client.py` & `lago-python-client-1.3.0/tests/test_webhook_endpoint_client.py`

 * *Files identical despite different names*

