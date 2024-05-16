# Comparing `tmp/airbyte_source_amazon_seller_partner-4.2.3.tar.gz` & `tmp/airbyte_source_amazon_seller_partner-4.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_amazon_seller_partner-4.2.3.tar", max compression
+gzip compressed data, was "airbyte_source_amazon_seller_partner-4.2.4.tar", max compression
```

## Comparing `airbyte_source_amazon_seller_partner-4.2.3.tar` & `airbyte_source_amazon_seller_partner-4.2.4.tar`

### file list

```diff
@@ -1,66 +1,66 @@
--rw-r--r--   0        0        0     4775 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/README.md
--rw-r--r--   0        0        0      899 2024-05-09 12:13:16.822048 airbyte_source_amazon_seller_partner-4.2.3/pyproject.toml
--rw-r--r--   0        0        0     1191 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/__init__.py
--rw-r--r--   0        0        0      638 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/auth.py
--rw-r--r--   0        0        0     6322 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/config_migrations.py
--rw-r--r--   0        0        0     3387 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/constants.py
--rw-r--r--   0        0        0      479 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/run.py
--rw-r--r--   0        0        0     1291 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_AFN_INVENTORY_DATA.json
--rw-r--r--   0        0        0     1221 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_AFN_INVENTORY_DATA_BY_COUNTRY.json
--rw-r--r--   0        0        0     6635 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_AMAZON_FULFILLED_SHIPMENTS_DATA_GENERAL.json
--rw-r--r--   0        0        0     1441 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_BRAND_ANALYTICS_MARKET_BASKET_REPORT.json
--rw-r--r--   0        0        0     2173 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_BRAND_ANALYTICS_REPEAT_PURCHASE_REPORT.json
--rw-r--r--   0        0        0     1729 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_BRAND_ANALYTICS_SEARCH_TERMS_REPORT.json
--rw-r--r--   0        0        0     5029 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_FBA_ESTIMATED_FBA_FEES_TXT_DATA.json
--rw-r--r--   0        0        0     2159 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_FBA_FULFILLMENT_CUSTOMER_RETURNS_DATA.json
--rw-r--r--   0        0        0     1613 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_FBA_FULFILLMENT_CUSTOMER_SHIPMENT_PROMOTION_DATA.json
--rw-r--r--   0        0        0     2036 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_FBA_FULFILLMENT_CUSTOMER_SHIPMENT_REPLACEMENT_DATA.json
--rw-r--r--   0        0        0     2446 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_FBA_FULFILLMENT_REMOVAL_ORDER_DETAIL_DATA.json
--rw-r--r--   0        0        0     1802 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_FBA_FULFILLMENT_REMOVAL_SHIPMENT_DETAIL_DATA.json
--rw-r--r--   0        0        0    11885 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_FBA_INVENTORY_PLANNING_DATA.json
--rw-r--r--   0        0        0     3678 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_FBA_MYI_UNSUPPRESSED_INVENTORY_DATA.json
--rw-r--r--   0        0        0     2965 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_FBA_REIMBURSEMENTS_DATA.json
--rw-r--r--   0        0        0     3066 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_FBA_SNS_FORECAST_DATA.json
--rw-r--r--   0        0        0     3349 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_FBA_SNS_PERFORMANCE_DATA.json
--rw-r--r--   0        0        0     4645 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_FBA_STORAGE_FEE_CHARGES_DATA.json
--rw-r--r--   0        0        0     3699 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_FLAT_FILE_ACTIONABLE_ORDER_DATA_SHIPPING.json
--rw-r--r--   0        0        0     4684 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_FLAT_FILE_ALL_ORDERS_DATA_BY_LAST_UPDATE_GENERAL.json
--rw-r--r--   0        0        0     4819 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_FLAT_FILE_ALL_ORDERS_DATA_BY_ORDER_DATE_GENERAL.json
--rw-r--r--   0        0        0     4125 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_FLAT_FILE_ARCHIVED_ORDERS_DATA_BY_ORDER_DATE.json
--rw-r--r--   0        0        0     3434 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_FLAT_FILE_OPEN_LISTINGS_DATA.json
--rw-r--r--   0        0        0     4629 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_FLAT_FILE_RETURNS_DATA_BY_RETURN_DATE.json
--rw-r--r--   0        0        0     2193 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_LEDGER_DETAIL_VIEW_DATA.json
--rw-r--r--   0        0        0     2823 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_LEDGER_SUMMARY_VIEW_DATA.json
--rw-r--r--   0        0        0     1381 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_MERCHANTS_LISTINGS_FYP_REPORT.json
--rw-r--r--   0        0        0     6146 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_MERCHANT_CANCELLED_LISTINGS_DATA.json
--rw-r--r--   0        0        0     3884 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_MERCHANT_LISTINGS_ALL_DATA.json
--rw-r--r--   0        0        0     6479 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_MERCHANT_LISTINGS_DATA.json
--rw-r--r--   0        0        0     6472 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_MERCHANT_LISTINGS_DATA_BACK_COMPAT.json
--rw-r--r--   0        0        0     3988 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_MERCHANT_LISTINGS_INACTIVE_DATA.json
--rw-r--r--   0        0        0     8105 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_ORDER_REPORT_DATA_SHIPPING.json
--rw-r--r--   0        0        0     4129 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_RESTOCK_INVENTORY_RECOMMENDATIONS_REPORT.json
--rw-r--r--   0        0        0     4223 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_SALES_AND_TRAFFIC_REPORT.json
--rw-r--r--   0        0        0     1185 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_SELLER_FEEDBACK_DATA.json
--rw-r--r--   0        0        0     2709 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_STRANDED_INVENTORY_UI_DATA.json
--rw-r--r--   0        0        0     5477 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_V2_SETTLEMENT_REPORT_DATA_FLAT_FILE.json
--rw-r--r--   0        0        0      387 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_VENDOR_FORECASTING_FRESH_REPORT.json
--rw-r--r--   0        0        0      388 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_VENDOR_FORECASTING_RETAIL_REPORT.json
--rw-r--r--   0        0        0     4217 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_VENDOR_INVENTORY_REPORT.json
--rw-r--r--   0        0        0     1550 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_VENDOR_NET_PURE_PRODUCT_MARGIN_REPORT.json
--rw-r--r--   0        0        0     1313 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_VENDOR_REAL_TIME_INVENTORY_REPORT.json
--rw-r--r--   0        0        0     2411 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_VENDOR_SALES_REPORT.json
--rw-r--r--   0        0        0     1384 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_VENDOR_TRAFFIC_REPORT.json
--rw-r--r--   0        0        0     4860 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_XML_ALL_ORDERS_DATA_BY_ORDER_DATE_GENERAL.json
--rw-r--r--   0        0        0     3786 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_XML_BROWSE_TREE_DATA.json
--rw-r--r--   0        0        0     2970 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/ListFinancialEventGroups.json
--rw-r--r--   0        0        0    44785 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/ListFinancialEvents.json
--rw-r--r--   0        0        0    11058 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/OrderItems.json
--rw-r--r--   0        0        0     7150 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/Orders.json
--rw-r--r--   0        0        0     9967 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/VendorDirectFulfillmentShipping.json
--rw-r--r--   0        0        0    16089 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/VendorOrders.json
--rw-r--r--   0        0        0      605 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/shared/GET_VENDOR_FORECASTING_REPORT.json
--rw-r--r--   0        0        0    10892 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/source.py
--rw-r--r--   0        0        0     8488 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/spec.json
--rw-r--r--   0        0        0    56375 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/streams.py
--rw-r--r--   0        0        0      403 2024-05-09 11:09:23.000000 airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/utils.py
--rw-r--r--   0        0        0     5599 1970-01-01 00:00:00.000000 airbyte_source_amazon_seller_partner-4.2.3/PKG-INFO
+-rw-r--r--   0        0        0     4775 2024-05-16 19:39:21.066241 airbyte_source_amazon_seller_partner-4.2.4/README.md
+-rw-r--r--   0        0        0      899 2024-05-16 19:44:20.326622 airbyte_source_amazon_seller_partner-4.2.4/pyproject.toml
+-rw-r--r--   0        0        0     1191 2024-05-16 19:39:21.070241 airbyte_source_amazon_seller_partner-4.2.4/source_amazon_seller_partner/__init__.py
+-rw-r--r--   0        0        0      638 2024-05-16 19:39:21.070241 airbyte_source_amazon_seller_partner-4.2.4/source_amazon_seller_partner/auth.py
+-rw-r--r--   0        0        0     6322 2024-05-16 19:39:21.070241 airbyte_source_amazon_seller_partner-4.2.4/source_amazon_seller_partner/config_migrations.py
+-rw-r--r--   0        0        0     3387 2024-05-16 19:39:21.070241 airbyte_source_amazon_seller_partner-4.2.4/source_amazon_seller_partner/constants.py
+-rw-r--r--   0        0        0      479 2024-05-16 19:39:21.070241 airbyte_source_amazon_seller_partner-4.2.4/source_amazon_seller_partner/run.py
+-rw-r--r--   0        0        0     1291 2024-05-16 19:39:21.070241 airbyte_source_amazon_seller_partner-4.2.4/source_amazon_seller_partner/schemas/GET_AFN_INVENTORY_DATA.json
+-rw-r--r--   0        0        0     1221 2024-05-16 19:39:21.070241 airbyte_source_amazon_seller_partner-4.2.4/source_amazon_seller_partner/schemas/GET_AFN_INVENTORY_DATA_BY_COUNTRY.json
+-rw-r--r--   0        0        0     6635 2024-05-16 19:39:21.070241 airbyte_source_amazon_seller_partner-4.2.4/source_amazon_seller_partner/schemas/GET_AMAZON_FULFILLED_SHIPMENTS_DATA_GENERAL.json
+-rw-r--r--   0        0        0     1441 2024-05-16 19:39:21.070241 airbyte_source_amazon_seller_partner-4.2.4/source_amazon_seller_partner/schemas/GET_BRAND_ANALYTICS_MARKET_BASKET_REPORT.json
+-rw-r--r--   0        0        0     2173 2024-05-16 19:39:21.070241 airbyte_source_amazon_seller_partner-4.2.4/source_amazon_seller_partner/schemas/GET_BRAND_ANALYTICS_REPEAT_PURCHASE_REPORT.json
+-rw-r--r--   0        0        0     1729 2024-05-16 19:39:21.070241 airbyte_source_amazon_seller_partner-4.2.4/source_amazon_seller_partner/schemas/GET_BRAND_ANALYTICS_SEARCH_TERMS_REPORT.json
+-rw-r--r--   0        0        0     5029 2024-05-16 19:39:21.070241 airbyte_source_amazon_seller_partner-4.2.4/source_amazon_seller_partner/schemas/GET_FBA_ESTIMATED_FBA_FEES_TXT_DATA.json
+-rw-r--r--   0        0        0     2159 2024-05-16 19:39:21.070241 airbyte_source_amazon_seller_partner-4.2.4/source_amazon_seller_partner/schemas/GET_FBA_FULFILLMENT_CUSTOMER_RETURNS_DATA.json
+-rw-r--r--   0        0        0     1613 2024-05-16 19:39:21.070241 airbyte_source_amazon_seller_partner-4.2.4/source_amazon_seller_partner/schemas/GET_FBA_FULFILLMENT_CUSTOMER_SHIPMENT_PROMOTION_DATA.json
+-rw-r--r--   0        0        0     2036 2024-05-16 19:39:21.070241 airbyte_source_amazon_seller_partner-4.2.4/source_amazon_seller_partner/schemas/GET_FBA_FULFILLMENT_CUSTOMER_SHIPMENT_REPLACEMENT_DATA.json
+-rw-r--r--   0        0        0     2446 2024-05-16 19:39:21.070241 airbyte_source_amazon_seller_partner-4.2.4/source_amazon_seller_partner/schemas/GET_FBA_FULFILLMENT_REMOVAL_ORDER_DETAIL_DATA.json
+-rw-r--r--   0        0        0     1802 2024-05-16 19:39:21.070241 airbyte_source_amazon_seller_partner-4.2.4/source_amazon_seller_partner/schemas/GET_FBA_FULFILLMENT_REMOVAL_SHIPMENT_DETAIL_DATA.json
+-rw-r--r--   0        0        0    11885 2024-05-16 19:39:21.070241 airbyte_source_amazon_seller_partner-4.2.4/source_amazon_seller_partner/schemas/GET_FBA_INVENTORY_PLANNING_DATA.json
+-rw-r--r--   0        0        0     3678 2024-05-16 19:39:21.070241 airbyte_source_amazon_seller_partner-4.2.4/source_amazon_seller_partner/schemas/GET_FBA_MYI_UNSUPPRESSED_INVENTORY_DATA.json
+-rw-r--r--   0        0        0     2965 2024-05-16 19:39:21.070241 airbyte_source_amazon_seller_partner-4.2.4/source_amazon_seller_partner/schemas/GET_FBA_REIMBURSEMENTS_DATA.json
+-rw-r--r--   0        0        0     3066 2024-05-16 19:39:21.070241 airbyte_source_amazon_seller_partner-4.2.4/source_amazon_seller_partner/schemas/GET_FBA_SNS_FORECAST_DATA.json
+-rw-r--r--   0        0        0     3349 2024-05-16 19:39:21.070241 airbyte_source_amazon_seller_partner-4.2.4/source_amazon_seller_partner/schemas/GET_FBA_SNS_PERFORMANCE_DATA.json
+-rw-r--r--   0        0        0     4645 2024-05-16 19:39:21.070241 airbyte_source_amazon_seller_partner-4.2.4/source_amazon_seller_partner/schemas/GET_FBA_STORAGE_FEE_CHARGES_DATA.json
+-rw-r--r--   0        0        0     3699 2024-05-16 19:39:21.070241 airbyte_source_amazon_seller_partner-4.2.4/source_amazon_seller_partner/schemas/GET_FLAT_FILE_ACTIONABLE_ORDER_DATA_SHIPPING.json
+-rw-r--r--   0        0        0     4684 2024-05-16 19:39:21.070241 airbyte_source_amazon_seller_partner-4.2.4/source_amazon_seller_partner/schemas/GET_FLAT_FILE_ALL_ORDERS_DATA_BY_LAST_UPDATE_GENERAL.json
+-rw-r--r--   0        0        0     4819 2024-05-16 19:39:21.070241 airbyte_source_amazon_seller_partner-4.2.4/source_amazon_seller_partner/schemas/GET_FLAT_FILE_ALL_ORDERS_DATA_BY_ORDER_DATE_GENERAL.json
+-rw-r--r--   0        0        0     4125 2024-05-16 19:39:21.070241 airbyte_source_amazon_seller_partner-4.2.4/source_amazon_seller_partner/schemas/GET_FLAT_FILE_ARCHIVED_ORDERS_DATA_BY_ORDER_DATE.json
+-rw-r--r--   0        0        0     3434 2024-05-16 19:39:21.070241 airbyte_source_amazon_seller_partner-4.2.4/source_amazon_seller_partner/schemas/GET_FLAT_FILE_OPEN_LISTINGS_DATA.json
+-rw-r--r--   0        0        0     4629 2024-05-16 19:39:21.070241 airbyte_source_amazon_seller_partner-4.2.4/source_amazon_seller_partner/schemas/GET_FLAT_FILE_RETURNS_DATA_BY_RETURN_DATE.json
+-rw-r--r--   0        0        0     2193 2024-05-16 19:39:21.070241 airbyte_source_amazon_seller_partner-4.2.4/source_amazon_seller_partner/schemas/GET_LEDGER_DETAIL_VIEW_DATA.json
+-rw-r--r--   0        0        0     2823 2024-05-16 19:39:21.070241 airbyte_source_amazon_seller_partner-4.2.4/source_amazon_seller_partner/schemas/GET_LEDGER_SUMMARY_VIEW_DATA.json
+-rw-r--r--   0        0        0     1381 2024-05-16 19:39:21.070241 airbyte_source_amazon_seller_partner-4.2.4/source_amazon_seller_partner/schemas/GET_MERCHANTS_LISTINGS_FYP_REPORT.json
+-rw-r--r--   0        0        0     6146 2024-05-16 19:39:21.070241 airbyte_source_amazon_seller_partner-4.2.4/source_amazon_seller_partner/schemas/GET_MERCHANT_CANCELLED_LISTINGS_DATA.json
+-rw-r--r--   0        0        0     3884 2024-05-16 19:39:21.070241 airbyte_source_amazon_seller_partner-4.2.4/source_amazon_seller_partner/schemas/GET_MERCHANT_LISTINGS_ALL_DATA.json
+-rw-r--r--   0        0        0     6479 2024-05-16 19:39:21.070241 airbyte_source_amazon_seller_partner-4.2.4/source_amazon_seller_partner/schemas/GET_MERCHANT_LISTINGS_DATA.json
+-rw-r--r--   0        0        0     6472 2024-05-16 19:39:21.070241 airbyte_source_amazon_seller_partner-4.2.4/source_amazon_seller_partner/schemas/GET_MERCHANT_LISTINGS_DATA_BACK_COMPAT.json
+-rw-r--r--   0        0        0     3988 2024-05-16 19:39:21.070241 airbyte_source_amazon_seller_partner-4.2.4/source_amazon_seller_partner/schemas/GET_MERCHANT_LISTINGS_INACTIVE_DATA.json
+-rw-r--r--   0        0        0     8105 2024-05-16 19:39:21.070241 airbyte_source_amazon_seller_partner-4.2.4/source_amazon_seller_partner/schemas/GET_ORDER_REPORT_DATA_SHIPPING.json
+-rw-r--r--   0        0        0     4129 2024-05-16 19:39:21.070241 airbyte_source_amazon_seller_partner-4.2.4/source_amazon_seller_partner/schemas/GET_RESTOCK_INVENTORY_RECOMMENDATIONS_REPORT.json
+-rw-r--r--   0        0        0     4223 2024-05-16 19:39:21.070241 airbyte_source_amazon_seller_partner-4.2.4/source_amazon_seller_partner/schemas/GET_SALES_AND_TRAFFIC_REPORT.json
+-rw-r--r--   0        0        0     1185 2024-05-16 19:39:21.070241 airbyte_source_amazon_seller_partner-4.2.4/source_amazon_seller_partner/schemas/GET_SELLER_FEEDBACK_DATA.json
+-rw-r--r--   0        0        0     2709 2024-05-16 19:39:21.070241 airbyte_source_amazon_seller_partner-4.2.4/source_amazon_seller_partner/schemas/GET_STRANDED_INVENTORY_UI_DATA.json
+-rw-r--r--   0        0        0     5477 2024-05-16 19:39:21.070241 airbyte_source_amazon_seller_partner-4.2.4/source_amazon_seller_partner/schemas/GET_V2_SETTLEMENT_REPORT_DATA_FLAT_FILE.json
+-rw-r--r--   0        0        0      387 2024-05-16 19:39:21.070241 airbyte_source_amazon_seller_partner-4.2.4/source_amazon_seller_partner/schemas/GET_VENDOR_FORECASTING_FRESH_REPORT.json
+-rw-r--r--   0        0        0      388 2024-05-16 19:39:21.070241 airbyte_source_amazon_seller_partner-4.2.4/source_amazon_seller_partner/schemas/GET_VENDOR_FORECASTING_RETAIL_REPORT.json
+-rw-r--r--   0        0        0     4217 2024-05-16 19:39:21.070241 airbyte_source_amazon_seller_partner-4.2.4/source_amazon_seller_partner/schemas/GET_VENDOR_INVENTORY_REPORT.json
+-rw-r--r--   0        0        0     1550 2024-05-16 19:39:21.070241 airbyte_source_amazon_seller_partner-4.2.4/source_amazon_seller_partner/schemas/GET_VENDOR_NET_PURE_PRODUCT_MARGIN_REPORT.json
+-rw-r--r--   0        0        0     1313 2024-05-16 19:39:21.070241 airbyte_source_amazon_seller_partner-4.2.4/source_amazon_seller_partner/schemas/GET_VENDOR_REAL_TIME_INVENTORY_REPORT.json
+-rw-r--r--   0        0        0     2411 2024-05-16 19:39:21.070241 airbyte_source_amazon_seller_partner-4.2.4/source_amazon_seller_partner/schemas/GET_VENDOR_SALES_REPORT.json
+-rw-r--r--   0        0        0     1384 2024-05-16 19:39:21.070241 airbyte_source_amazon_seller_partner-4.2.4/source_amazon_seller_partner/schemas/GET_VENDOR_TRAFFIC_REPORT.json
+-rw-r--r--   0        0        0     4860 2024-05-16 19:39:21.070241 airbyte_source_amazon_seller_partner-4.2.4/source_amazon_seller_partner/schemas/GET_XML_ALL_ORDERS_DATA_BY_ORDER_DATE_GENERAL.json
+-rw-r--r--   0        0        0     3786 2024-05-16 19:39:21.070241 airbyte_source_amazon_seller_partner-4.2.4/source_amazon_seller_partner/schemas/GET_XML_BROWSE_TREE_DATA.json
+-rw-r--r--   0        0        0     2970 2024-05-16 19:39:21.070241 airbyte_source_amazon_seller_partner-4.2.4/source_amazon_seller_partner/schemas/ListFinancialEventGroups.json
+-rw-r--r--   0        0        0    44785 2024-05-16 19:39:21.070241 airbyte_source_amazon_seller_partner-4.2.4/source_amazon_seller_partner/schemas/ListFinancialEvents.json
+-rw-r--r--   0        0        0    11058 2024-05-16 19:39:21.070241 airbyte_source_amazon_seller_partner-4.2.4/source_amazon_seller_partner/schemas/OrderItems.json
+-rw-r--r--   0        0        0     7150 2024-05-16 19:39:21.070241 airbyte_source_amazon_seller_partner-4.2.4/source_amazon_seller_partner/schemas/Orders.json
+-rw-r--r--   0        0        0     9967 2024-05-16 19:39:21.070241 airbyte_source_amazon_seller_partner-4.2.4/source_amazon_seller_partner/schemas/VendorDirectFulfillmentShipping.json
+-rw-r--r--   0        0        0    16089 2024-05-16 19:39:21.070241 airbyte_source_amazon_seller_partner-4.2.4/source_amazon_seller_partner/schemas/VendorOrders.json
+-rw-r--r--   0        0        0      605 2024-05-16 19:39:21.070241 airbyte_source_amazon_seller_partner-4.2.4/source_amazon_seller_partner/schemas/shared/GET_VENDOR_FORECASTING_REPORT.json
+-rw-r--r--   0        0        0    10892 2024-05-16 19:39:21.070241 airbyte_source_amazon_seller_partner-4.2.4/source_amazon_seller_partner/source.py
+-rw-r--r--   0        0        0     8488 2024-05-16 19:39:21.074241 airbyte_source_amazon_seller_partner-4.2.4/source_amazon_seller_partner/spec.json
+-rw-r--r--   0        0        0    56434 2024-05-16 19:39:21.074241 airbyte_source_amazon_seller_partner-4.2.4/source_amazon_seller_partner/streams.py
+-rw-r--r--   0        0        0      403 2024-05-16 19:39:21.074241 airbyte_source_amazon_seller_partner-4.2.4/source_amazon_seller_partner/utils.py
+-rw-r--r--   0        0        0     5599 1970-01-01 00:00:00.000000 airbyte_source_amazon_seller_partner-4.2.4/PKG-INFO
```

### Comparing `airbyte_source_amazon_seller_partner-4.2.3/README.md` & `airbyte_source_amazon_seller_partner-4.2.4/README.md`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.3/pyproject.toml` & `airbyte_source_amazon_seller_partner-4.2.4/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "4.2.3"
+version = "4.2.4"
 name = "airbyte-source-amazon-seller-partner"
 description = "Source implementation for Amazon Seller Partner."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "MIT"
 readme = "README.md"
```

### Comparing `airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/__init__.py` & `airbyte_source_amazon_seller_partner-4.2.4/source_amazon_seller_partner/__init__.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/auth.py` & `airbyte_source_amazon_seller_partner-4.2.4/source_amazon_seller_partner/auth.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/config_migrations.py` & `airbyte_source_amazon_seller_partner-4.2.4/source_amazon_seller_partner/config_migrations.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/constants.py` & `airbyte_source_amazon_seller_partner-4.2.4/source_amazon_seller_partner/constants.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_AFN_INVENTORY_DATA.json` & `airbyte_source_amazon_seller_partner-4.2.4/source_amazon_seller_partner/schemas/GET_AFN_INVENTORY_DATA.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_AFN_INVENTORY_DATA_BY_COUNTRY.json` & `airbyte_source_amazon_seller_partner-4.2.4/source_amazon_seller_partner/schemas/GET_AFN_INVENTORY_DATA_BY_COUNTRY.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_AMAZON_FULFILLED_SHIPMENTS_DATA_GENERAL.json` & `airbyte_source_amazon_seller_partner-4.2.4/source_amazon_seller_partner/schemas/GET_AMAZON_FULFILLED_SHIPMENTS_DATA_GENERAL.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_BRAND_ANALYTICS_MARKET_BASKET_REPORT.json` & `airbyte_source_amazon_seller_partner-4.2.4/source_amazon_seller_partner/schemas/GET_BRAND_ANALYTICS_MARKET_BASKET_REPORT.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_BRAND_ANALYTICS_REPEAT_PURCHASE_REPORT.json` & `airbyte_source_amazon_seller_partner-4.2.4/source_amazon_seller_partner/schemas/GET_BRAND_ANALYTICS_REPEAT_PURCHASE_REPORT.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_BRAND_ANALYTICS_SEARCH_TERMS_REPORT.json` & `airbyte_source_amazon_seller_partner-4.2.4/source_amazon_seller_partner/schemas/GET_BRAND_ANALYTICS_SEARCH_TERMS_REPORT.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_FBA_ESTIMATED_FBA_FEES_TXT_DATA.json` & `airbyte_source_amazon_seller_partner-4.2.4/source_amazon_seller_partner/schemas/GET_FBA_ESTIMATED_FBA_FEES_TXT_DATA.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_FBA_FULFILLMENT_CUSTOMER_RETURNS_DATA.json` & `airbyte_source_amazon_seller_partner-4.2.4/source_amazon_seller_partner/schemas/GET_FBA_FULFILLMENT_CUSTOMER_RETURNS_DATA.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_FBA_FULFILLMENT_CUSTOMER_SHIPMENT_PROMOTION_DATA.json` & `airbyte_source_amazon_seller_partner-4.2.4/source_amazon_seller_partner/schemas/GET_FBA_FULFILLMENT_CUSTOMER_SHIPMENT_PROMOTION_DATA.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_FBA_FULFILLMENT_CUSTOMER_SHIPMENT_REPLACEMENT_DATA.json` & `airbyte_source_amazon_seller_partner-4.2.4/source_amazon_seller_partner/schemas/GET_FBA_FULFILLMENT_CUSTOMER_SHIPMENT_REPLACEMENT_DATA.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_FBA_FULFILLMENT_REMOVAL_ORDER_DETAIL_DATA.json` & `airbyte_source_amazon_seller_partner-4.2.4/source_amazon_seller_partner/schemas/GET_FBA_FULFILLMENT_REMOVAL_ORDER_DETAIL_DATA.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_FBA_FULFILLMENT_REMOVAL_SHIPMENT_DETAIL_DATA.json` & `airbyte_source_amazon_seller_partner-4.2.4/source_amazon_seller_partner/schemas/GET_FBA_FULFILLMENT_REMOVAL_SHIPMENT_DETAIL_DATA.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_FBA_INVENTORY_PLANNING_DATA.json` & `airbyte_source_amazon_seller_partner-4.2.4/source_amazon_seller_partner/schemas/GET_FBA_INVENTORY_PLANNING_DATA.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_FBA_MYI_UNSUPPRESSED_INVENTORY_DATA.json` & `airbyte_source_amazon_seller_partner-4.2.4/source_amazon_seller_partner/schemas/GET_FBA_MYI_UNSUPPRESSED_INVENTORY_DATA.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_FBA_REIMBURSEMENTS_DATA.json` & `airbyte_source_amazon_seller_partner-4.2.4/source_amazon_seller_partner/schemas/GET_FBA_REIMBURSEMENTS_DATA.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_FBA_SNS_FORECAST_DATA.json` & `airbyte_source_amazon_seller_partner-4.2.4/source_amazon_seller_partner/schemas/GET_FBA_SNS_FORECAST_DATA.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_FBA_SNS_PERFORMANCE_DATA.json` & `airbyte_source_amazon_seller_partner-4.2.4/source_amazon_seller_partner/schemas/GET_FBA_SNS_PERFORMANCE_DATA.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_FBA_STORAGE_FEE_CHARGES_DATA.json` & `airbyte_source_amazon_seller_partner-4.2.4/source_amazon_seller_partner/schemas/GET_FBA_STORAGE_FEE_CHARGES_DATA.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_FLAT_FILE_ACTIONABLE_ORDER_DATA_SHIPPING.json` & `airbyte_source_amazon_seller_partner-4.2.4/source_amazon_seller_partner/schemas/GET_FLAT_FILE_ACTIONABLE_ORDER_DATA_SHIPPING.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_FLAT_FILE_ALL_ORDERS_DATA_BY_LAST_UPDATE_GENERAL.json` & `airbyte_source_amazon_seller_partner-4.2.4/source_amazon_seller_partner/schemas/GET_FLAT_FILE_ALL_ORDERS_DATA_BY_LAST_UPDATE_GENERAL.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_FLAT_FILE_ALL_ORDERS_DATA_BY_ORDER_DATE_GENERAL.json` & `airbyte_source_amazon_seller_partner-4.2.4/source_amazon_seller_partner/schemas/GET_FLAT_FILE_ALL_ORDERS_DATA_BY_ORDER_DATE_GENERAL.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_FLAT_FILE_ARCHIVED_ORDERS_DATA_BY_ORDER_DATE.json` & `airbyte_source_amazon_seller_partner-4.2.4/source_amazon_seller_partner/schemas/GET_FLAT_FILE_ARCHIVED_ORDERS_DATA_BY_ORDER_DATE.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_FLAT_FILE_OPEN_LISTINGS_DATA.json` & `airbyte_source_amazon_seller_partner-4.2.4/source_amazon_seller_partner/schemas/GET_FLAT_FILE_OPEN_LISTINGS_DATA.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_FLAT_FILE_RETURNS_DATA_BY_RETURN_DATE.json` & `airbyte_source_amazon_seller_partner-4.2.4/source_amazon_seller_partner/schemas/GET_FLAT_FILE_RETURNS_DATA_BY_RETURN_DATE.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_LEDGER_DETAIL_VIEW_DATA.json` & `airbyte_source_amazon_seller_partner-4.2.4/source_amazon_seller_partner/schemas/GET_LEDGER_DETAIL_VIEW_DATA.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_LEDGER_SUMMARY_VIEW_DATA.json` & `airbyte_source_amazon_seller_partner-4.2.4/source_amazon_seller_partner/schemas/GET_LEDGER_SUMMARY_VIEW_DATA.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_MERCHANTS_LISTINGS_FYP_REPORT.json` & `airbyte_source_amazon_seller_partner-4.2.4/source_amazon_seller_partner/schemas/GET_MERCHANTS_LISTINGS_FYP_REPORT.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_MERCHANT_CANCELLED_LISTINGS_DATA.json` & `airbyte_source_amazon_seller_partner-4.2.4/source_amazon_seller_partner/schemas/GET_MERCHANT_CANCELLED_LISTINGS_DATA.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_MERCHANT_LISTINGS_ALL_DATA.json` & `airbyte_source_amazon_seller_partner-4.2.4/source_amazon_seller_partner/schemas/GET_MERCHANT_LISTINGS_ALL_DATA.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_MERCHANT_LISTINGS_DATA.json` & `airbyte_source_amazon_seller_partner-4.2.4/source_amazon_seller_partner/schemas/GET_MERCHANT_LISTINGS_DATA.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_MERCHANT_LISTINGS_DATA_BACK_COMPAT.json` & `airbyte_source_amazon_seller_partner-4.2.4/source_amazon_seller_partner/schemas/GET_MERCHANT_LISTINGS_DATA_BACK_COMPAT.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_MERCHANT_LISTINGS_INACTIVE_DATA.json` & `airbyte_source_amazon_seller_partner-4.2.4/source_amazon_seller_partner/schemas/GET_MERCHANT_LISTINGS_INACTIVE_DATA.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_ORDER_REPORT_DATA_SHIPPING.json` & `airbyte_source_amazon_seller_partner-4.2.4/source_amazon_seller_partner/schemas/GET_ORDER_REPORT_DATA_SHIPPING.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_RESTOCK_INVENTORY_RECOMMENDATIONS_REPORT.json` & `airbyte_source_amazon_seller_partner-4.2.4/source_amazon_seller_partner/schemas/GET_RESTOCK_INVENTORY_RECOMMENDATIONS_REPORT.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_SALES_AND_TRAFFIC_REPORT.json` & `airbyte_source_amazon_seller_partner-4.2.4/source_amazon_seller_partner/schemas/GET_SALES_AND_TRAFFIC_REPORT.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_SELLER_FEEDBACK_DATA.json` & `airbyte_source_amazon_seller_partner-4.2.4/source_amazon_seller_partner/schemas/GET_SELLER_FEEDBACK_DATA.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_STRANDED_INVENTORY_UI_DATA.json` & `airbyte_source_amazon_seller_partner-4.2.4/source_amazon_seller_partner/schemas/GET_STRANDED_INVENTORY_UI_DATA.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_V2_SETTLEMENT_REPORT_DATA_FLAT_FILE.json` & `airbyte_source_amazon_seller_partner-4.2.4/source_amazon_seller_partner/schemas/GET_V2_SETTLEMENT_REPORT_DATA_FLAT_FILE.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_VENDOR_INVENTORY_REPORT.json` & `airbyte_source_amazon_seller_partner-4.2.4/source_amazon_seller_partner/schemas/GET_VENDOR_INVENTORY_REPORT.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_VENDOR_NET_PURE_PRODUCT_MARGIN_REPORT.json` & `airbyte_source_amazon_seller_partner-4.2.4/source_amazon_seller_partner/schemas/GET_VENDOR_NET_PURE_PRODUCT_MARGIN_REPORT.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_VENDOR_REAL_TIME_INVENTORY_REPORT.json` & `airbyte_source_amazon_seller_partner-4.2.4/source_amazon_seller_partner/schemas/GET_VENDOR_REAL_TIME_INVENTORY_REPORT.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_VENDOR_SALES_REPORT.json` & `airbyte_source_amazon_seller_partner-4.2.4/source_amazon_seller_partner/schemas/GET_VENDOR_SALES_REPORT.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_VENDOR_TRAFFIC_REPORT.json` & `airbyte_source_amazon_seller_partner-4.2.4/source_amazon_seller_partner/schemas/GET_VENDOR_TRAFFIC_REPORT.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_XML_ALL_ORDERS_DATA_BY_ORDER_DATE_GENERAL.json` & `airbyte_source_amazon_seller_partner-4.2.4/source_amazon_seller_partner/schemas/GET_XML_ALL_ORDERS_DATA_BY_ORDER_DATE_GENERAL.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/GET_XML_BROWSE_TREE_DATA.json` & `airbyte_source_amazon_seller_partner-4.2.4/source_amazon_seller_partner/schemas/GET_XML_BROWSE_TREE_DATA.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/ListFinancialEventGroups.json` & `airbyte_source_amazon_seller_partner-4.2.4/source_amazon_seller_partner/schemas/ListFinancialEventGroups.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/ListFinancialEvents.json` & `airbyte_source_amazon_seller_partner-4.2.4/source_amazon_seller_partner/schemas/ListFinancialEvents.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/OrderItems.json` & `airbyte_source_amazon_seller_partner-4.2.4/source_amazon_seller_partner/schemas/OrderItems.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/Orders.json` & `airbyte_source_amazon_seller_partner-4.2.4/source_amazon_seller_partner/schemas/Orders.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/VendorDirectFulfillmentShipping.json` & `airbyte_source_amazon_seller_partner-4.2.4/source_amazon_seller_partner/schemas/VendorDirectFulfillmentShipping.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/VendorOrders.json` & `airbyte_source_amazon_seller_partner-4.2.4/source_amazon_seller_partner/schemas/VendorOrders.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/schemas/shared/GET_VENDOR_FORECASTING_REPORT.json` & `airbyte_source_amazon_seller_partner-4.2.4/source_amazon_seller_partner/schemas/shared/GET_VENDOR_FORECASTING_REPORT.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/source.py` & `airbyte_source_amazon_seller_partner-4.2.4/source_amazon_seller_partner/source.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/spec.json` & `airbyte_source_amazon_seller_partner-4.2.4/source_amazon_seller_partner/spec.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.3/source_amazon_seller_partner/streams.py` & `airbyte_source_amazon_seller_partner-4.2.4/source_amazon_seller_partner/streams.py`

 * *Files 0% similar despite different names*

```diff
@@ -850,14 +850,16 @@
     result_key = "inventoryByAsin"
     availability_sla_days = 3
 
 
 class VendorTrafficReport(IncrementalAnalyticsStream):
     name = "GET_VENDOR_TRAFFIC_REPORT"
     result_key = "trafficByAsin"
+    availability_sla_days = 3
+    fixed_period_in_days = 1
 
 
 class SellerAnalyticsSalesAndTrafficReports(IncrementalAnalyticsStream):
     """
     Field definitions: https://developer-docs.amazon.com/sp-api/docs/report-type-values#seller-retail-analytics-reports
     """
```

### Comparing `airbyte_source_amazon_seller_partner-4.2.3/PKG-INFO` & `airbyte_source_amazon_seller_partner-4.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airbyte-source-amazon-seller-partner
-Version: 4.2.3
+Version: 4.2.4
 Summary: Source implementation for Amazon Seller Partner.
 Home-page: https://airbyte.com
 License: MIT
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
```

