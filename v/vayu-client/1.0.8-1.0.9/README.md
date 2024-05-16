# Comparing `tmp/vayu_client-1.0.8.tar.gz` & `tmp/vayu_client-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vayu_client-1.0.8.tar", last modified: Thu May  9 14:51:05 2024, max compression
+gzip compressed data, was "vayu_client-1.0.9.tar", last modified: Thu May 16 13:21:05 2024, max compression
```

## Comparing `vayu_client-1.0.8.tar` & `vayu_client-1.0.9.tar`

### file list

```diff
@@ -1,105 +1,105 @@
-drwxr-xr-x   0 shaigross   (501) staff       (20)        0 2024-05-09 14:51:05.217110 vayu_client-1.0.8/
--rw-r--r--   0 shaigross   (501) staff       (20)     2539 2024-05-09 14:51:05.217195 vayu_client-1.0.8/PKG-INFO
--rw-r--r--   0 shaigross   (501) staff       (20)      481 2024-05-08 15:19:35.000000 vayu_client-1.0.8/README.md
-drwxr-xr-x   0 shaigross   (501) staff       (20)        0 2024-05-09 14:51:05.203408 vayu_client-1.0.8/entity_clients/
--rw-r--r--   0 shaigross   (501) staff       (20)       46 2024-05-08 13:47:16.000000 vayu_client-1.0.8/entity_clients/__init__.py
--rw-r--r--   0 shaigross   (501) staff       (20)     1383 2024-05-09 14:41:31.000000 vayu_client-1.0.8/entity_clients/contracts_client.py
--rw-r--r--   0 shaigross   (501) staff       (20)     1571 2024-05-09 14:40:19.000000 vayu_client-1.0.8/entity_clients/customers_client.py
--rw-r--r--   0 shaigross   (501) staff       (20)     1593 2024-05-09 14:43:56.000000 vayu_client-1.0.8/entity_clients/events_client.py
--rw-r--r--   0 shaigross   (501) staff       (20)      578 2024-05-09 14:44:20.000000 vayu_client-1.0.8/entity_clients/invoices_client.py
--rw-r--r--   0 shaigross   (501) staff       (20)     1984 2024-05-09 14:45:22.000000 vayu_client-1.0.8/entity_clients/meters_client.py
--rw-r--r--   0 shaigross   (501) staff       (20)      673 2024-05-09 14:45:51.000000 vayu_client-1.0.8/entity_clients/plans_client.py
-drwxr-xr-x   0 shaigross   (501) staff       (20)        0 2024-05-09 14:51:05.204360 vayu_client-1.0.8/openapi_client/
--rw-r--r--   0 shaigross   (501) staff       (20)     6785 2024-05-09 13:52:52.000000 vayu_client-1.0.8/openapi_client/__init__.py
-drwxr-xr-x   0 shaigross   (501) staff       (20)        0 2024-05-09 14:51:05.205723 vayu_client-1.0.8/openapi_client/api/
--rw-r--r--   0 shaigross   (501) staff       (20)      422 2024-05-09 13:52:52.000000 vayu_client-1.0.8/openapi_client/api/__init__.py
--rw-r--r--   0 shaigross   (501) staff       (20)    12591 2024-05-09 13:52:52.000000 vayu_client-1.0.8/openapi_client/api/auth_api.py
--rw-r--r--   0 shaigross   (501) staff       (20)    43742 2024-05-09 13:52:52.000000 vayu_client-1.0.8/openapi_client/api/contracts_api.py
--rw-r--r--   0 shaigross   (501) staff       (20)    55565 2024-05-09 13:52:52.000000 vayu_client-1.0.8/openapi_client/api/customers_api.py
--rw-r--r--   0 shaigross   (501) staff       (20)    61236 2024-05-09 13:52:52.000000 vayu_client-1.0.8/openapi_client/api/events_api.py
--rw-r--r--   0 shaigross   (501) staff       (20)    22281 2024-05-09 13:52:52.000000 vayu_client-1.0.8/openapi_client/api/invoices_api.py
--rw-r--r--   0 shaigross   (501) staff       (20)    43924 2024-05-09 13:52:52.000000 vayu_client-1.0.8/openapi_client/api/meters_api.py
--rw-r--r--   0 shaigross   (501) staff       (20)    32198 2024-05-09 13:52:52.000000 vayu_client-1.0.8/openapi_client/api/plans_api.py
--rw-r--r--   0 shaigross   (501) staff       (20)    26550 2024-05-09 13:52:52.000000 vayu_client-1.0.8/openapi_client/api_client.py
--rw-r--r--   0 shaigross   (501) staff       (20)      652 2024-05-09 13:52:52.000000 vayu_client-1.0.8/openapi_client/api_response.py
--rw-r--r--   0 shaigross   (501) staff       (20)    15152 2024-05-09 13:52:52.000000 vayu_client-1.0.8/openapi_client/configuration.py
--rw-r--r--   0 shaigross   (501) staff       (20)     6180 2024-05-09 13:52:52.000000 vayu_client-1.0.8/openapi_client/exceptions.py
-drwxr-xr-x   0 shaigross   (501) staff       (20)        0 2024-05-09 14:51:05.216303 vayu_client-1.0.8/openapi_client/models/
--rw-r--r--   0 shaigross   (501) staff       (20)     5867 2024-05-09 13:52:52.000000 vayu_client-1.0.8/openapi_client/models/__init__.py
--rw-r--r--   0 shaigross   (501) staff       (20)     3340 2024-05-09 13:52:51.000000 vayu_client-1.0.8/openapi_client/models/aggregation_method.py
--rw-r--r--   0 shaigross   (501) staff       (20)     1161 2024-05-09 13:52:51.000000 vayu_client-1.0.8/openapi_client/models/aggregation_operator.py
--rw-r--r--   0 shaigross   (501) staff       (20)     1052 2024-05-09 13:52:51.000000 vayu_client-1.0.8/openapi_client/models/billing_interval.py
--rw-r--r--   0 shaigross   (501) staff       (20)     3214 2024-05-09 13:52:51.000000 vayu_client-1.0.8/openapi_client/models/condition.py
--rw-r--r--   0 shaigross   (501) staff       (20)     4112 2024-05-09 13:52:51.000000 vayu_client-1.0.8/openapi_client/models/create_contract_request_schema.py
--rw-r--r--   0 shaigross   (501) staff       (20)     3126 2024-05-09 13:52:52.000000 vayu_client-1.0.8/openapi_client/models/create_contract_response_schema.py
--rw-r--r--   0 shaigross   (501) staff       (20)     3084 2024-05-09 13:52:52.000000 vayu_client-1.0.8/openapi_client/models/create_customer_request_schema.py
--rw-r--r--   0 shaigross   (501) staff       (20)     3138 2024-05-09 13:52:52.000000 vayu_client-1.0.8/openapi_client/models/create_customer_response_schema.py
--rw-r--r--   0 shaigross   (501) staff       (20)     3765 2024-05-09 13:52:52.000000 vayu_client-1.0.8/openapi_client/models/create_customer_response_schema_customer.py
--rw-r--r--   0 shaigross   (501) staff       (20)     3034 2024-05-09 13:52:52.000000 vayu_client-1.0.8/openapi_client/models/criterion.py
--rw-r--r--   0 shaigross   (501) staff       (20)     1202 2024-05-09 13:52:52.000000 vayu_client-1.0.8/openapi_client/models/criterion_operator.py
--rw-r--r--   0 shaigross   (501) staff       (20)     3138 2024-05-09 13:52:52.000000 vayu_client-1.0.8/openapi_client/models/delete_contract_response_schema.py
--rw-r--r--   0 shaigross   (501) staff       (20)     4870 2024-05-09 13:52:52.000000 vayu_client-1.0.8/openapi_client/models/delete_contract_response_schema_contract.py
--rw-r--r--   0 shaigross   (501) staff       (20)     3138 2024-05-09 13:52:52.000000 vayu_client-1.0.8/openapi_client/models/delete_customer_response_schema.py
--rw-r--r--   0 shaigross   (501) staff       (20)     3889 2024-05-09 13:52:52.000000 vayu_client-1.0.8/openapi_client/models/delete_customer_response_schema_customer.py
--rw-r--r--   0 shaigross   (501) staff       (20)     3134 2024-05-09 13:52:52.000000 vayu_client-1.0.8/openapi_client/models/delete_event_by_ref_id_response_schema.py
--rw-r--r--   0 shaigross   (501) staff       (20)     4983 2024-05-09 13:52:52.000000 vayu_client-1.0.8/openapi_client/models/delete_event_by_ref_id_response_schema_event.py
--rw-r--r--   0 shaigross   (501) staff       (20)     3075 2024-05-09 13:52:52.000000 vayu_client-1.0.8/openapi_client/models/delete_meter_response_schema.py
--rw-r--r--   0 shaigross   (501) staff       (20)     4732 2024-05-09 13:52:52.000000 vayu_client-1.0.8/openapi_client/models/delete_meter_response_schema_meter.py
--rw-r--r--   0 shaigross   (501) staff       (20)     3054 2024-05-09 13:52:52.000000 vayu_client-1.0.8/openapi_client/models/delete_plan_response_schema.py
--rw-r--r--   0 shaigross   (501) staff       (20)     4207 2024-05-09 13:52:52.000000 vayu_client-1.0.8/openapi_client/models/delete_plan_response_schema_plan.py
--rw-r--r--   0 shaigross   (501) staff       (20)     4127 2024-05-09 13:52:52.000000 vayu_client-1.0.8/openapi_client/models/event.py
--rw-r--r--   0 shaigross   (501) staff       (20)     3243 2024-05-09 13:52:52.000000 vayu_client-1.0.8/openapi_client/models/events_dry_run_request_schema.py
--rw-r--r--   0 shaigross   (501) staff       (20)     4380 2024-05-09 13:52:52.000000 vayu_client-1.0.8/openapi_client/models/events_dry_run_response_schema_inner.py
--rw-r--r--   0 shaigross   (501) staff       (20)     3921 2024-05-09 13:52:52.000000 vayu_client-1.0.8/openapi_client/models/events_dry_run_response_schema_inner_event.py
--rw-r--r--   0 shaigross   (501) staff       (20)     4556 2024-05-09 13:52:52.000000 vayu_client-1.0.8/openapi_client/models/events_dry_run_response_schema_inner_meter_with_values_inner.py
--rw-r--r--   0 shaigross   (501) staff       (20)     3461 2024-05-08 11:11:33.000000 vayu_client-1.0.8/openapi_client/models/events_dry_run_response_schema_inner_meter_with_values_inner_aggregation_method.py
--rw-r--r--   0 shaigross   (501) staff       (20)     3477 2024-05-09 13:52:52.000000 vayu_client-1.0.8/openapi_client/models/filter.py
--rw-r--r--   0 shaigross   (501) staff       (20)     3114 2024-05-09 13:52:52.000000 vayu_client-1.0.8/openapi_client/models/get_contract_response_schema.py
--rw-r--r--   0 shaigross   (501) staff       (20)     4734 2024-05-09 13:52:52.000000 vayu_client-1.0.8/openapi_client/models/get_contract_response_schema_contract.py
--rw-r--r--   0 shaigross   (501) staff       (20)     3126 2024-05-09 13:52:52.000000 vayu_client-1.0.8/openapi_client/models/get_customer_response_schema.py
--rw-r--r--   0 shaigross   (501) staff       (20)     3110 2024-05-09 13:52:52.000000 vayu_client-1.0.8/openapi_client/models/get_event_by_ref_id_response_schema.py
--rw-r--r--   0 shaigross   (501) staff       (20)     4861 2024-05-09 13:52:52.000000 vayu_client-1.0.8/openapi_client/models/get_event_by_ref_id_response_schema_event.py
--rw-r--r--   0 shaigross   (501) staff       (20)     3093 2024-05-09 13:52:52.000000 vayu_client-1.0.8/openapi_client/models/get_invoice_response_schema.py
--rw-r--r--   0 shaigross   (501) staff       (20)     6035 2024-05-09 13:52:52.000000 vayu_client-1.0.8/openapi_client/models/get_invoice_response_schema_invoice.py
--rw-r--r--   0 shaigross   (501) staff       (20)     3515 2024-05-09 13:52:52.000000 vayu_client-1.0.8/openapi_client/models/get_invoice_response_schema_invoice_line_items_inner.py
--rw-r--r--   0 shaigross   (501) staff       (20)     3051 2024-05-09 13:52:52.000000 vayu_client-1.0.8/openapi_client/models/get_meter_response_schema.py
--rw-r--r--   0 shaigross   (501) staff       (20)     4596 2024-05-09 13:52:52.000000 vayu_client-1.0.8/openapi_client/models/get_meter_response_schema_meter.py
--rw-r--r--   0 shaigross   (501) staff       (20)     3030 2024-05-09 13:52:52.000000 vayu_client-1.0.8/openapi_client/models/get_plan_response_schema.py
--rw-r--r--   0 shaigross   (501) staff       (20)     4071 2024-05-09 13:52:52.000000 vayu_client-1.0.8/openapi_client/models/get_plan_response_schema_plan.py
--rw-r--r--   0 shaigross   (501) staff       (20)     3704 2024-05-09 13:52:52.000000 vayu_client-1.0.8/openapi_client/models/list_contracts_response_schema.py
--rw-r--r--   0 shaigross   (501) staff       (20)     4766 2024-05-09 12:38:25.000000 vayu_client-1.0.8/openapi_client/models/list_contracts_response_schema_contracts_inner.py
--rw-r--r--   0 shaigross   (501) staff       (20)     3716 2024-05-09 13:52:52.000000 vayu_client-1.0.8/openapi_client/models/list_customers_response_schema.py
--rw-r--r--   0 shaigross   (501) staff       (20)     3785 2024-05-09 12:38:25.000000 vayu_client-1.0.8/openapi_client/models/list_customers_response_schema_customers_inner.py
--rw-r--r--   0 shaigross   (501) staff       (20)     3683 2024-05-09 13:52:52.000000 vayu_client-1.0.8/openapi_client/models/list_invoices_response_schema.py
--rw-r--r--   0 shaigross   (501) staff       (20)     6067 2024-05-09 12:38:25.000000 vayu_client-1.0.8/openapi_client/models/list_invoices_response_schema_invoices_inner.py
--rw-r--r--   0 shaigross   (501) staff       (20)     3641 2024-05-09 13:52:52.000000 vayu_client-1.0.8/openapi_client/models/list_meters_response_schema.py
--rw-r--r--   0 shaigross   (501) staff       (20)     4628 2024-05-09 12:38:25.000000 vayu_client-1.0.8/openapi_client/models/list_meters_response_schema_meters_inner.py
--rw-r--r--   0 shaigross   (501) staff       (20)     3620 2024-05-09 13:52:52.000000 vayu_client-1.0.8/openapi_client/models/list_plans_response_schema.py
--rw-r--r--   0 shaigross   (501) staff       (20)     4103 2024-05-09 12:38:25.000000 vayu_client-1.0.8/openapi_client/models/list_plans_response_schema_plans_inner.py
--rw-r--r--   0 shaigross   (501) staff       (20)     2883 2024-05-09 13:52:52.000000 vayu_client-1.0.8/openapi_client/models/login_request_schema.py
--rw-r--r--   0 shaigross   (501) staff       (20)     2870 2024-05-09 13:52:52.000000 vayu_client-1.0.8/openapi_client/models/login_response_schema.py
--rw-r--r--   0 shaigross   (501) staff       (20)     2883 2024-05-09 13:52:52.000000 vayu_client-1.0.8/openapi_client/models/period.py
--rw-r--r--   0 shaigross   (501) staff       (20)     3483 2024-05-09 13:52:52.000000 vayu_client-1.0.8/openapi_client/models/plan_billing_data.py
--rw-r--r--   0 shaigross   (501) staff       (20)     1023 2024-05-09 13:52:52.000000 vayu_client-1.0.8/openapi_client/models/plan_status.py
--rw-r--r--   0 shaigross   (501) staff       (20)      947 2024-05-09 13:52:52.000000 vayu_client-1.0.8/openapi_client/models/plan_type.py
--rw-r--r--   0 shaigross   (501) staff       (20)     3353 2024-05-09 13:52:52.000000 vayu_client-1.0.8/openapi_client/models/query_events_response_schema.py
--rw-r--r--   0 shaigross   (501) staff       (20)     4866 2024-05-09 13:52:52.000000 vayu_client-1.0.8/openapi_client/models/query_events_response_schema_events_inner.py
--rw-r--r--   0 shaigross   (501) staff       (20)     3235 2024-05-09 13:52:52.000000 vayu_client-1.0.8/openapi_client/models/send_events_request_schema.py
--rw-r--r--   0 shaigross   (501) staff       (20)     4230 2024-05-08 14:01:03.000000 vayu_client-1.0.8/openapi_client/models/send_events_request_schema_events_inner.py
--rw-r--r--   0 shaigross   (501) staff       (20)     4212 2024-05-09 13:52:52.000000 vayu_client-1.0.8/openapi_client/models/send_events_response_schema.py
--rw-r--r--   0 shaigross   (501) staff       (20)     3218 2024-05-09 13:52:52.000000 vayu_client-1.0.8/openapi_client/models/send_events_response_schema_invalid_events_inner.py
--rw-r--r--   0 shaigross   (501) staff       (20)     3108 2024-05-09 13:52:52.000000 vayu_client-1.0.8/openapi_client/models/update_customer_request_schema.py
--rw-r--r--   0 shaigross   (501) staff       (20)     3138 2024-05-09 13:52:52.000000 vayu_client-1.0.8/openapi_client/models/update_customer_response_schema.py
--rw-r--r--   0 shaigross   (501) staff       (20)     4011 2024-05-09 13:52:52.000000 vayu_client-1.0.8/openapi_client/models/update_meter_request_schema.py
--rw-r--r--   0 shaigross   (501) staff       (20)     3063 2024-05-09 13:52:52.000000 vayu_client-1.0.8/openapi_client/models/update_meter_response_schema.py
--rw-r--r--   0 shaigross   (501) staff       (20)     9616 2024-05-09 13:52:52.000000 vayu_client-1.0.8/openapi_client/rest.py
--rw-r--r--   0 shaigross   (501) staff       (20)      420 2024-05-09 14:51:05.217467 vayu_client-1.0.8/setup.cfg
--rw-r--r--   0 shaigross   (501) staff       (20)      296 2024-01-24 16:49:22.000000 vayu_client-1.0.8/setup.py
--rw-r--r--   0 shaigross   (501) staff       (20)     2208 2024-05-09 13:41:05.000000 vayu_client-1.0.8/vayu.py
-drwxr-xr-x   0 shaigross   (501) staff       (20)        0 2024-05-09 14:51:05.217006 vayu_client-1.0.8/vayu_client.egg-info/
--rw-r--r--   0 shaigross   (501) staff       (20)     2539 2024-05-09 14:51:05.000000 vayu_client-1.0.8/vayu_client.egg-info/PKG-INFO
--rw-r--r--   0 shaigross   (501) staff       (20)     4650 2024-05-09 14:51:05.000000 vayu_client-1.0.8/vayu_client.egg-info/SOURCES.txt
--rw-r--r--   0 shaigross   (501) staff       (20)        1 2024-05-09 14:51:05.000000 vayu_client-1.0.8/vayu_client.egg-info/dependency_links.txt
--rw-r--r--   0 shaigross   (501) staff       (20)      102 2024-05-09 14:51:05.000000 vayu_client-1.0.8/vayu_client.egg-info/requires.txt
--rw-r--r--   0 shaigross   (501) staff       (20)       47 2024-05-09 14:51:05.000000 vayu_client-1.0.8/vayu_client.egg-info/top_level.txt
--rw-r--r--   0 shaigross   (501) staff       (20)       41 2024-05-09 13:41:17.000000 vayu_client-1.0.8/vayu_consts.py
+drwxr-xr-x   0 shaigross   (501) staff       (20)        0 2024-05-16 13:21:05.991664 vayu_client-1.0.9/
+-rw-r--r--   0 shaigross   (501) staff       (20)     5676 2024-05-16 13:21:05.991772 vayu_client-1.0.9/PKG-INFO
+-rw-r--r--   0 shaigross   (501) staff       (20)      481 2024-05-09 14:54:07.000000 vayu_client-1.0.9/README.md
+drwxr-xr-x   0 shaigross   (501) staff       (20)        0 2024-05-16 13:21:05.970056 vayu_client-1.0.9/entity_clients/
+-rw-r--r--   0 shaigross   (501) staff       (20)       46 2024-05-09 14:54:07.000000 vayu_client-1.0.9/entity_clients/__init__.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     1383 2024-05-09 14:54:07.000000 vayu_client-1.0.9/entity_clients/contracts_client.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     1571 2024-05-09 14:54:07.000000 vayu_client-1.0.9/entity_clients/customers_client.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     1593 2024-05-09 14:54:07.000000 vayu_client-1.0.9/entity_clients/events_client.py
+-rw-r--r--   0 shaigross   (501) staff       (20)      578 2024-05-09 14:54:07.000000 vayu_client-1.0.9/entity_clients/invoices_client.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     1984 2024-05-09 14:54:07.000000 vayu_client-1.0.9/entity_clients/meters_client.py
+-rw-r--r--   0 shaigross   (501) staff       (20)      672 2024-05-15 07:12:52.000000 vayu_client-1.0.9/entity_clients/plans_client.py
+drwxr-xr-x   0 shaigross   (501) staff       (20)        0 2024-05-16 13:21:05.972073 vayu_client-1.0.9/openapi_client/
+-rw-r--r--   0 shaigross   (501) staff       (20)     6785 2024-05-09 13:52:52.000000 vayu_client-1.0.9/openapi_client/__init__.py
+drwxr-xr-x   0 shaigross   (501) staff       (20)        0 2024-05-16 13:21:05.975380 vayu_client-1.0.9/openapi_client/api/
+-rw-r--r--   0 shaigross   (501) staff       (20)      422 2024-05-09 13:52:52.000000 vayu_client-1.0.9/openapi_client/api/__init__.py
+-rw-r--r--   0 shaigross   (501) staff       (20)    12591 2024-05-09 13:52:52.000000 vayu_client-1.0.9/openapi_client/api/auth_api.py
+-rw-r--r--   0 shaigross   (501) staff       (20)    43742 2024-05-09 13:52:52.000000 vayu_client-1.0.9/openapi_client/api/contracts_api.py
+-rw-r--r--   0 shaigross   (501) staff       (20)    55565 2024-05-09 13:52:52.000000 vayu_client-1.0.9/openapi_client/api/customers_api.py
+-rw-r--r--   0 shaigross   (501) staff       (20)    61236 2024-05-09 13:52:52.000000 vayu_client-1.0.9/openapi_client/api/events_api.py
+-rw-r--r--   0 shaigross   (501) staff       (20)    22281 2024-05-09 13:52:52.000000 vayu_client-1.0.9/openapi_client/api/invoices_api.py
+-rw-r--r--   0 shaigross   (501) staff       (20)    43924 2024-05-09 13:52:52.000000 vayu_client-1.0.9/openapi_client/api/meters_api.py
+-rw-r--r--   0 shaigross   (501) staff       (20)    32198 2024-05-09 13:52:52.000000 vayu_client-1.0.9/openapi_client/api/plans_api.py
+-rw-r--r--   0 shaigross   (501) staff       (20)    26550 2024-05-09 13:52:52.000000 vayu_client-1.0.9/openapi_client/api_client.py
+-rw-r--r--   0 shaigross   (501) staff       (20)      652 2024-05-09 13:52:52.000000 vayu_client-1.0.9/openapi_client/api_response.py
+-rw-r--r--   0 shaigross   (501) staff       (20)    15152 2024-05-09 13:52:52.000000 vayu_client-1.0.9/openapi_client/configuration.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     6180 2024-05-09 13:52:52.000000 vayu_client-1.0.9/openapi_client/exceptions.py
+drwxr-xr-x   0 shaigross   (501) staff       (20)        0 2024-05-16 13:21:05.990635 vayu_client-1.0.9/openapi_client/models/
+-rw-r--r--   0 shaigross   (501) staff       (20)     5867 2024-05-09 13:52:52.000000 vayu_client-1.0.9/openapi_client/models/__init__.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3340 2024-05-09 13:52:51.000000 vayu_client-1.0.9/openapi_client/models/aggregation_method.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     1161 2024-05-09 13:52:51.000000 vayu_client-1.0.9/openapi_client/models/aggregation_operator.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     1052 2024-05-09 13:52:51.000000 vayu_client-1.0.9/openapi_client/models/billing_interval.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3214 2024-05-09 13:52:51.000000 vayu_client-1.0.9/openapi_client/models/condition.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     4112 2024-05-09 13:52:51.000000 vayu_client-1.0.9/openapi_client/models/create_contract_request_schema.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3126 2024-05-09 13:52:52.000000 vayu_client-1.0.9/openapi_client/models/create_contract_response_schema.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3084 2024-05-09 13:52:52.000000 vayu_client-1.0.9/openapi_client/models/create_customer_request_schema.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3138 2024-05-09 13:52:52.000000 vayu_client-1.0.9/openapi_client/models/create_customer_response_schema.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3765 2024-05-09 13:52:52.000000 vayu_client-1.0.9/openapi_client/models/create_customer_response_schema_customer.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3034 2024-05-09 13:52:52.000000 vayu_client-1.0.9/openapi_client/models/criterion.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     1202 2024-05-09 13:52:52.000000 vayu_client-1.0.9/openapi_client/models/criterion_operator.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3138 2024-05-09 13:52:52.000000 vayu_client-1.0.9/openapi_client/models/delete_contract_response_schema.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     4870 2024-05-09 13:52:52.000000 vayu_client-1.0.9/openapi_client/models/delete_contract_response_schema_contract.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3138 2024-05-09 13:52:52.000000 vayu_client-1.0.9/openapi_client/models/delete_customer_response_schema.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3889 2024-05-09 13:52:52.000000 vayu_client-1.0.9/openapi_client/models/delete_customer_response_schema_customer.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3134 2024-05-09 13:52:52.000000 vayu_client-1.0.9/openapi_client/models/delete_event_by_ref_id_response_schema.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     4983 2024-05-09 13:52:52.000000 vayu_client-1.0.9/openapi_client/models/delete_event_by_ref_id_response_schema_event.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3075 2024-05-09 13:52:52.000000 vayu_client-1.0.9/openapi_client/models/delete_meter_response_schema.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     4732 2024-05-09 13:52:52.000000 vayu_client-1.0.9/openapi_client/models/delete_meter_response_schema_meter.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3054 2024-05-09 13:52:52.000000 vayu_client-1.0.9/openapi_client/models/delete_plan_response_schema.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     4207 2024-05-09 13:52:52.000000 vayu_client-1.0.9/openapi_client/models/delete_plan_response_schema_plan.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     4127 2024-05-09 13:52:52.000000 vayu_client-1.0.9/openapi_client/models/event.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3243 2024-05-09 13:52:52.000000 vayu_client-1.0.9/openapi_client/models/events_dry_run_request_schema.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     4380 2024-05-09 13:52:52.000000 vayu_client-1.0.9/openapi_client/models/events_dry_run_response_schema_inner.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3921 2024-05-09 13:52:52.000000 vayu_client-1.0.9/openapi_client/models/events_dry_run_response_schema_inner_event.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     4556 2024-05-09 13:52:52.000000 vayu_client-1.0.9/openapi_client/models/events_dry_run_response_schema_inner_meter_with_values_inner.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3461 2024-05-08 11:11:33.000000 vayu_client-1.0.9/openapi_client/models/events_dry_run_response_schema_inner_meter_with_values_inner_aggregation_method.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3477 2024-05-09 13:52:52.000000 vayu_client-1.0.9/openapi_client/models/filter.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3114 2024-05-09 13:52:52.000000 vayu_client-1.0.9/openapi_client/models/get_contract_response_schema.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     4734 2024-05-09 13:52:52.000000 vayu_client-1.0.9/openapi_client/models/get_contract_response_schema_contract.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3126 2024-05-09 13:52:52.000000 vayu_client-1.0.9/openapi_client/models/get_customer_response_schema.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3110 2024-05-09 13:52:52.000000 vayu_client-1.0.9/openapi_client/models/get_event_by_ref_id_response_schema.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     4861 2024-05-09 13:52:52.000000 vayu_client-1.0.9/openapi_client/models/get_event_by_ref_id_response_schema_event.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3093 2024-05-09 13:52:52.000000 vayu_client-1.0.9/openapi_client/models/get_invoice_response_schema.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     6035 2024-05-09 13:52:52.000000 vayu_client-1.0.9/openapi_client/models/get_invoice_response_schema_invoice.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3515 2024-05-09 13:52:52.000000 vayu_client-1.0.9/openapi_client/models/get_invoice_response_schema_invoice_line_items_inner.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3051 2024-05-09 13:52:52.000000 vayu_client-1.0.9/openapi_client/models/get_meter_response_schema.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     4596 2024-05-09 13:52:52.000000 vayu_client-1.0.9/openapi_client/models/get_meter_response_schema_meter.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3030 2024-05-09 13:52:52.000000 vayu_client-1.0.9/openapi_client/models/get_plan_response_schema.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     4071 2024-05-09 13:52:52.000000 vayu_client-1.0.9/openapi_client/models/get_plan_response_schema_plan.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3704 2024-05-09 13:52:52.000000 vayu_client-1.0.9/openapi_client/models/list_contracts_response_schema.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     4766 2024-05-09 12:38:25.000000 vayu_client-1.0.9/openapi_client/models/list_contracts_response_schema_contracts_inner.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3716 2024-05-09 13:52:52.000000 vayu_client-1.0.9/openapi_client/models/list_customers_response_schema.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3785 2024-05-09 12:38:25.000000 vayu_client-1.0.9/openapi_client/models/list_customers_response_schema_customers_inner.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3683 2024-05-09 13:52:52.000000 vayu_client-1.0.9/openapi_client/models/list_invoices_response_schema.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     6067 2024-05-09 12:38:25.000000 vayu_client-1.0.9/openapi_client/models/list_invoices_response_schema_invoices_inner.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3641 2024-05-09 13:52:52.000000 vayu_client-1.0.9/openapi_client/models/list_meters_response_schema.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     4628 2024-05-09 12:38:25.000000 vayu_client-1.0.9/openapi_client/models/list_meters_response_schema_meters_inner.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3620 2024-05-09 13:52:52.000000 vayu_client-1.0.9/openapi_client/models/list_plans_response_schema.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     4103 2024-05-09 12:38:25.000000 vayu_client-1.0.9/openapi_client/models/list_plans_response_schema_plans_inner.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     2883 2024-05-09 13:52:52.000000 vayu_client-1.0.9/openapi_client/models/login_request_schema.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     2870 2024-05-09 13:52:52.000000 vayu_client-1.0.9/openapi_client/models/login_response_schema.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     2883 2024-05-09 13:52:52.000000 vayu_client-1.0.9/openapi_client/models/period.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3483 2024-05-09 13:52:52.000000 vayu_client-1.0.9/openapi_client/models/plan_billing_data.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     1023 2024-05-09 13:52:52.000000 vayu_client-1.0.9/openapi_client/models/plan_status.py
+-rw-r--r--   0 shaigross   (501) staff       (20)      947 2024-05-09 13:52:52.000000 vayu_client-1.0.9/openapi_client/models/plan_type.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3353 2024-05-09 13:52:52.000000 vayu_client-1.0.9/openapi_client/models/query_events_response_schema.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     4866 2024-05-09 13:52:52.000000 vayu_client-1.0.9/openapi_client/models/query_events_response_schema_events_inner.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3235 2024-05-09 13:52:52.000000 vayu_client-1.0.9/openapi_client/models/send_events_request_schema.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     4230 2024-05-08 14:01:03.000000 vayu_client-1.0.9/openapi_client/models/send_events_request_schema_events_inner.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     4212 2024-05-09 13:52:52.000000 vayu_client-1.0.9/openapi_client/models/send_events_response_schema.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3218 2024-05-09 13:52:52.000000 vayu_client-1.0.9/openapi_client/models/send_events_response_schema_invalid_events_inner.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3108 2024-05-09 13:52:52.000000 vayu_client-1.0.9/openapi_client/models/update_customer_request_schema.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3138 2024-05-09 13:52:52.000000 vayu_client-1.0.9/openapi_client/models/update_customer_response_schema.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     4011 2024-05-09 13:52:52.000000 vayu_client-1.0.9/openapi_client/models/update_meter_request_schema.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     3063 2024-05-09 13:52:52.000000 vayu_client-1.0.9/openapi_client/models/update_meter_response_schema.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     9616 2024-05-09 13:52:52.000000 vayu_client-1.0.9/openapi_client/rest.py
+-rw-r--r--   0 shaigross   (501) staff       (20)      420 2024-05-16 13:21:05.992026 vayu_client-1.0.9/setup.cfg
+-rw-r--r--   0 shaigross   (501) staff       (20)      296 2024-01-24 16:49:22.000000 vayu_client-1.0.9/setup.py
+-rw-r--r--   0 shaigross   (501) staff       (20)     2208 2024-05-09 14:54:07.000000 vayu_client-1.0.9/vayu.py
+drwxr-xr-x   0 shaigross   (501) staff       (20)        0 2024-05-16 13:21:05.991542 vayu_client-1.0.9/vayu_client.egg-info/
+-rw-r--r--   0 shaigross   (501) staff       (20)     5676 2024-05-16 13:21:05.000000 vayu_client-1.0.9/vayu_client.egg-info/PKG-INFO
+-rw-r--r--   0 shaigross   (501) staff       (20)     4650 2024-05-16 13:21:05.000000 vayu_client-1.0.9/vayu_client.egg-info/SOURCES.txt
+-rw-r--r--   0 shaigross   (501) staff       (20)        1 2024-05-16 13:21:05.000000 vayu_client-1.0.9/vayu_client.egg-info/dependency_links.txt
+-rw-r--r--   0 shaigross   (501) staff       (20)      102 2024-05-16 13:21:05.000000 vayu_client-1.0.9/vayu_client.egg-info/requires.txt
+-rw-r--r--   0 shaigross   (501) staff       (20)       47 2024-05-16 13:21:05.000000 vayu_client-1.0.9/vayu_client.egg-info/top_level.txt
+-rw-r--r--   0 shaigross   (501) staff       (20)       41 2024-05-09 14:54:07.000000 vayu_client-1.0.9/vayu_consts.py
```

### Comparing `vayu_client-1.0.8/entity_clients/contracts_client.py` & `vayu_client-1.0.9/entity_clients/contracts_client.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.8/entity_clients/customers_client.py` & `vayu_client-1.0.9/entity_clients/customers_client.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.8/entity_clients/events_client.py` & `vayu_client-1.0.9/entity_clients/events_client.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.8/entity_clients/invoices_client.py` & `vayu_client-1.0.9/entity_clients/invoices_client.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.8/entity_clients/meters_client.py` & `vayu_client-1.0.9/entity_clients/meters_client.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.8/entity_clients/plans_client.py` & `vayu_client-1.0.9/entity_clients/plans_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     def __init__(self, api_client: ApiClient):
         self.__plans_client = PlansApi(api_client)
 
     def get(self, plan_id: str):
         get_plans_response = self.__plans_client.get_plan(plan_id)
 
         return get_plans_response.plan
-    
+   
     def list(self, limit: int = None, cursor: int = None):
         return self.__plans_client.list_plans(limit=limit, cursor=cursor)
 
     def delete(self, id: str):
         delete_plan_response = self.__plans_client.delete_plan(id)
 
         return delete_plan_response.plan
```

### Comparing `vayu_client-1.0.8/openapi_client/__init__.py` & `vayu_client-1.0.9/openapi_client/__init__.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.8/openapi_client/api/auth_api.py` & `vayu_client-1.0.9/openapi_client/api/auth_api.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.8/openapi_client/api/contracts_api.py` & `vayu_client-1.0.9/openapi_client/api/contracts_api.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.8/openapi_client/api/customers_api.py` & `vayu_client-1.0.9/openapi_client/api/customers_api.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.8/openapi_client/api/events_api.py` & `vayu_client-1.0.9/openapi_client/api/events_api.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.8/openapi_client/api/invoices_api.py` & `vayu_client-1.0.9/openapi_client/api/invoices_api.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.8/openapi_client/api/meters_api.py` & `vayu_client-1.0.9/openapi_client/api/meters_api.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.8/openapi_client/api/plans_api.py` & `vayu_client-1.0.9/openapi_client/api/plans_api.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.8/openapi_client/api_client.py` & `vayu_client-1.0.9/openapi_client/api_client.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.8/openapi_client/api_response.py` & `vayu_client-1.0.9/openapi_client/api_response.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.8/openapi_client/configuration.py` & `vayu_client-1.0.9/openapi_client/configuration.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.8/openapi_client/exceptions.py` & `vayu_client-1.0.9/openapi_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.8/openapi_client/models/__init__.py` & `vayu_client-1.0.9/openapi_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.8/openapi_client/models/aggregation_method.py` & `vayu_client-1.0.9/openapi_client/models/aggregation_method.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.8/openapi_client/models/aggregation_operator.py` & `vayu_client-1.0.9/openapi_client/models/aggregation_operator.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.8/openapi_client/models/billing_interval.py` & `vayu_client-1.0.9/openapi_client/models/billing_interval.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.8/openapi_client/models/condition.py` & `vayu_client-1.0.9/openapi_client/models/condition.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.8/openapi_client/models/create_contract_request_schema.py` & `vayu_client-1.0.9/openapi_client/models/create_contract_request_schema.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.8/openapi_client/models/create_contract_response_schema.py` & `vayu_client-1.0.9/openapi_client/models/create_contract_response_schema.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.8/openapi_client/models/create_customer_request_schema.py` & `vayu_client-1.0.9/openapi_client/models/create_customer_request_schema.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.8/openapi_client/models/create_customer_response_schema.py` & `vayu_client-1.0.9/openapi_client/models/create_customer_response_schema.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.8/openapi_client/models/create_customer_response_schema_customer.py` & `vayu_client-1.0.9/openapi_client/models/create_customer_response_schema_customer.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.8/openapi_client/models/criterion.py` & `vayu_client-1.0.9/openapi_client/models/criterion.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.8/openapi_client/models/criterion_operator.py` & `vayu_client-1.0.9/openapi_client/models/criterion_operator.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.8/openapi_client/models/delete_contract_response_schema.py` & `vayu_client-1.0.9/openapi_client/models/delete_contract_response_schema.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.8/openapi_client/models/delete_contract_response_schema_contract.py` & `vayu_client-1.0.9/openapi_client/models/delete_contract_response_schema_contract.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.8/openapi_client/models/delete_customer_response_schema.py` & `vayu_client-1.0.9/openapi_client/models/delete_customer_response_schema.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.8/openapi_client/models/delete_customer_response_schema_customer.py` & `vayu_client-1.0.9/openapi_client/models/delete_customer_response_schema_customer.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.8/openapi_client/models/delete_event_by_ref_id_response_schema.py` & `vayu_client-1.0.9/openapi_client/models/delete_event_by_ref_id_response_schema.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.8/openapi_client/models/delete_event_by_ref_id_response_schema_event.py` & `vayu_client-1.0.9/openapi_client/models/delete_event_by_ref_id_response_schema_event.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.8/openapi_client/models/delete_meter_response_schema.py` & `vayu_client-1.0.9/openapi_client/models/delete_meter_response_schema.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.8/openapi_client/models/delete_meter_response_schema_meter.py` & `vayu_client-1.0.9/openapi_client/models/delete_meter_response_schema_meter.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.8/openapi_client/models/delete_plan_response_schema.py` & `vayu_client-1.0.9/openapi_client/models/delete_plan_response_schema.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.8/openapi_client/models/delete_plan_response_schema_plan.py` & `vayu_client-1.0.9/openapi_client/models/delete_plan_response_schema_plan.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.8/openapi_client/models/event.py` & `vayu_client-1.0.9/openapi_client/models/event.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.8/openapi_client/models/events_dry_run_request_schema.py` & `vayu_client-1.0.9/openapi_client/models/events_dry_run_request_schema.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.8/openapi_client/models/events_dry_run_response_schema_inner.py` & `vayu_client-1.0.9/openapi_client/models/events_dry_run_response_schema_inner.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.8/openapi_client/models/events_dry_run_response_schema_inner_event.py` & `vayu_client-1.0.9/openapi_client/models/events_dry_run_response_schema_inner_event.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.8/openapi_client/models/events_dry_run_response_schema_inner_meter_with_values_inner.py` & `vayu_client-1.0.9/openapi_client/models/events_dry_run_response_schema_inner_meter_with_values_inner.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.8/openapi_client/models/events_dry_run_response_schema_inner_meter_with_values_inner_aggregation_method.py` & `vayu_client-1.0.9/openapi_client/models/events_dry_run_response_schema_inner_meter_with_values_inner_aggregation_method.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.8/openapi_client/models/filter.py` & `vayu_client-1.0.9/openapi_client/models/filter.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.8/openapi_client/models/get_contract_response_schema.py` & `vayu_client-1.0.9/openapi_client/models/get_contract_response_schema.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.8/openapi_client/models/get_contract_response_schema_contract.py` & `vayu_client-1.0.9/openapi_client/models/get_contract_response_schema_contract.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.8/openapi_client/models/get_customer_response_schema.py` & `vayu_client-1.0.9/openapi_client/models/get_customer_response_schema.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.8/openapi_client/models/get_event_by_ref_id_response_schema.py` & `vayu_client-1.0.9/openapi_client/models/get_event_by_ref_id_response_schema.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.8/openapi_client/models/get_event_by_ref_id_response_schema_event.py` & `vayu_client-1.0.9/openapi_client/models/get_event_by_ref_id_response_schema_event.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.8/openapi_client/models/get_invoice_response_schema.py` & `vayu_client-1.0.9/openapi_client/models/get_invoice_response_schema.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.8/openapi_client/models/get_invoice_response_schema_invoice.py` & `vayu_client-1.0.9/openapi_client/models/get_invoice_response_schema_invoice.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.8/openapi_client/models/get_invoice_response_schema_invoice_line_items_inner.py` & `vayu_client-1.0.9/openapi_client/models/get_invoice_response_schema_invoice_line_items_inner.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.8/openapi_client/models/get_meter_response_schema.py` & `vayu_client-1.0.9/openapi_client/models/get_meter_response_schema.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.8/openapi_client/models/get_meter_response_schema_meter.py` & `vayu_client-1.0.9/openapi_client/models/get_meter_response_schema_meter.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.8/openapi_client/models/get_plan_response_schema.py` & `vayu_client-1.0.9/openapi_client/models/get_plan_response_schema.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.8/openapi_client/models/get_plan_response_schema_plan.py` & `vayu_client-1.0.9/openapi_client/models/get_plan_response_schema_plan.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.8/openapi_client/models/list_contracts_response_schema.py` & `vayu_client-1.0.9/openapi_client/models/list_contracts_response_schema.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.8/openapi_client/models/list_contracts_response_schema_contracts_inner.py` & `vayu_client-1.0.9/openapi_client/models/list_contracts_response_schema_contracts_inner.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.8/openapi_client/models/list_customers_response_schema.py` & `vayu_client-1.0.9/openapi_client/models/list_customers_response_schema.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.8/openapi_client/models/list_customers_response_schema_customers_inner.py` & `vayu_client-1.0.9/openapi_client/models/list_customers_response_schema_customers_inner.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.8/openapi_client/models/list_invoices_response_schema.py` & `vayu_client-1.0.9/openapi_client/models/list_invoices_response_schema.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.8/openapi_client/models/list_invoices_response_schema_invoices_inner.py` & `vayu_client-1.0.9/openapi_client/models/list_invoices_response_schema_invoices_inner.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.8/openapi_client/models/list_meters_response_schema.py` & `vayu_client-1.0.9/openapi_client/models/list_meters_response_schema.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.8/openapi_client/models/list_meters_response_schema_meters_inner.py` & `vayu_client-1.0.9/openapi_client/models/list_meters_response_schema_meters_inner.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.8/openapi_client/models/list_plans_response_schema.py` & `vayu_client-1.0.9/openapi_client/models/list_plans_response_schema.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.8/openapi_client/models/list_plans_response_schema_plans_inner.py` & `vayu_client-1.0.9/openapi_client/models/list_plans_response_schema_plans_inner.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.8/openapi_client/models/login_request_schema.py` & `vayu_client-1.0.9/openapi_client/models/login_request_schema.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.8/openapi_client/models/login_response_schema.py` & `vayu_client-1.0.9/openapi_client/models/login_response_schema.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.8/openapi_client/models/period.py` & `vayu_client-1.0.9/openapi_client/models/period.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.8/openapi_client/models/plan_billing_data.py` & `vayu_client-1.0.9/openapi_client/models/plan_billing_data.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.8/openapi_client/models/plan_status.py` & `vayu_client-1.0.9/openapi_client/models/plan_status.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.8/openapi_client/models/plan_type.py` & `vayu_client-1.0.9/openapi_client/models/plan_type.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.8/openapi_client/models/query_events_response_schema.py` & `vayu_client-1.0.9/openapi_client/models/query_events_response_schema.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.8/openapi_client/models/query_events_response_schema_events_inner.py` & `vayu_client-1.0.9/openapi_client/models/query_events_response_schema_events_inner.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.8/openapi_client/models/send_events_request_schema.py` & `vayu_client-1.0.9/openapi_client/models/send_events_request_schema.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.8/openapi_client/models/send_events_request_schema_events_inner.py` & `vayu_client-1.0.9/openapi_client/models/send_events_request_schema_events_inner.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.8/openapi_client/models/send_events_response_schema.py` & `vayu_client-1.0.9/openapi_client/models/send_events_response_schema.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.8/openapi_client/models/send_events_response_schema_invalid_events_inner.py` & `vayu_client-1.0.9/openapi_client/models/send_events_response_schema_invalid_events_inner.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.8/openapi_client/models/update_customer_request_schema.py` & `vayu_client-1.0.9/openapi_client/models/update_customer_request_schema.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.8/openapi_client/models/update_customer_response_schema.py` & `vayu_client-1.0.9/openapi_client/models/update_customer_response_schema.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.8/openapi_client/models/update_meter_request_schema.py` & `vayu_client-1.0.9/openapi_client/models/update_meter_request_schema.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.8/openapi_client/models/update_meter_response_schema.py` & `vayu_client-1.0.9/openapi_client/models/update_meter_response_schema.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.8/openapi_client/rest.py` & `vayu_client-1.0.9/openapi_client/rest.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.8/vayu.py` & `vayu_client-1.0.9/vayu.py`

 * *Files identical despite different names*

### Comparing `vayu_client-1.0.8/vayu_client.egg-info/SOURCES.txt` & `vayu_client-1.0.9/vayu_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

