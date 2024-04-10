# Comparing `tmp/airbyte_source_amazon_seller_partner-4.2.0.tar.gz` & `tmp/airbyte_source_amazon_seller_partner-4.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_amazon_seller_partner-4.2.0.tar", max compression
+gzip compressed data, was "airbyte_source_amazon_seller_partner-4.2.1.tar", max compression
```

## Comparing `airbyte_source_amazon_seller_partner-4.2.0.tar` & `airbyte_source_amazon_seller_partner-4.2.1.tar`

### file list

```diff
@@ -1,66 +1,66 @@
--rw-r--r--   0        0        0     4765 2024-03-21 01:47:20.313993 airbyte_source_amazon_seller_partner-4.2.0/README.md
--rw-r--r--   0        0        0      895 2024-03-21 02:44:24.607895 airbyte_source_amazon_seller_partner-4.2.0/pyproject.toml
--rw-r--r--   0        0        0     1191 2024-03-21 01:47:20.313993 airbyte_source_amazon_seller_partner-4.2.0/source_amazon_seller_partner/__init__.py
--rw-r--r--   0        0        0      638 2024-03-21 01:47:20.313993 airbyte_source_amazon_seller_partner-4.2.0/source_amazon_seller_partner/auth.py
--rw-r--r--   0        0        0     6322 2024-03-21 01:47:20.313993 airbyte_source_amazon_seller_partner-4.2.0/source_amazon_seller_partner/config_migrations.py
--rw-r--r--   0        0        0     3387 2024-03-21 01:47:20.313993 airbyte_source_amazon_seller_partner-4.2.0/source_amazon_seller_partner/constants.py
--rw-r--r--   0        0        0      479 2024-03-21 01:47:20.313993 airbyte_source_amazon_seller_partner-4.2.0/source_amazon_seller_partner/run.py
--rw-r--r--   0        0        0      576 2024-03-21 01:47:20.313993 airbyte_source_amazon_seller_partner-4.2.0/source_amazon_seller_partner/schemas/GET_AFN_INVENTORY_DATA.json
--rw-r--r--   0        0        0      568 2024-03-21 01:47:20.313993 airbyte_source_amazon_seller_partner-4.2.0/source_amazon_seller_partner/schemas/GET_AFN_INVENTORY_DATA_BY_COUNTRY.json
--rw-r--r--   0        0        0     2997 2024-03-21 01:47:20.313993 airbyte_source_amazon_seller_partner-4.2.0/source_amazon_seller_partner/schemas/GET_AMAZON_FULFILLED_SHIPMENTS_DATA_GENERAL.json
--rw-r--r--   0        0        0      799 2024-03-21 01:47:20.313993 airbyte_source_amazon_seller_partner-4.2.0/source_amazon_seller_partner/schemas/GET_BRAND_ANALYTICS_MARKET_BASKET_REPORT.json
--rw-r--r--   0        0        0     1112 2024-03-21 01:47:20.313993 airbyte_source_amazon_seller_partner-4.2.0/source_amazon_seller_partner/schemas/GET_BRAND_ANALYTICS_REPEAT_PURCHASE_REPORT.json
--rw-r--r--   0        0        0      823 2024-03-21 01:47:20.313993 airbyte_source_amazon_seller_partner-4.2.0/source_amazon_seller_partner/schemas/GET_BRAND_ANALYTICS_SEARCH_TERMS_REPORT.json
--rw-r--r--   0        0        0     2434 2024-03-21 01:47:20.313993 airbyte_source_amazon_seller_partner-4.2.0/source_amazon_seller_partner/schemas/GET_FBA_ESTIMATED_FBA_FEES_TXT_DATA.json
--rw-r--r--   0        0        0      950 2024-03-21 01:47:20.313993 airbyte_source_amazon_seller_partner-4.2.0/source_amazon_seller_partner/schemas/GET_FBA_FULFILLMENT_CUSTOMER_RETURNS_DATA.json
--rw-r--r--   0        0        0      744 2024-03-21 01:47:20.313993 airbyte_source_amazon_seller_partner-4.2.0/source_amazon_seller_partner/schemas/GET_FBA_FULFILLMENT_CUSTOMER_SHIPMENT_PROMOTION_DATA.json
--rw-r--r--   0        0        0     1816 2024-03-21 01:47:20.313993 airbyte_source_amazon_seller_partner-4.2.0/source_amazon_seller_partner/schemas/GET_FBA_FULFILLMENT_CUSTOMER_SHIPMENT_REPLACEMENT_DATA.json
--rw-r--r--   0        0        0     1305 2024-03-21 01:47:20.313993 airbyte_source_amazon_seller_partner-4.2.0/source_amazon_seller_partner/schemas/GET_FBA_FULFILLMENT_REMOVAL_ORDER_DETAIL_DATA.json
--rw-r--r--   0        0        0      916 2024-03-21 01:47:20.313993 airbyte_source_amazon_seller_partner-4.2.0/source_amazon_seller_partner/schemas/GET_FBA_FULFILLMENT_REMOVAL_SHIPMENT_DETAIL_DATA.json
--rw-r--r--   0        0        0     4986 2024-03-21 01:47:20.313993 airbyte_source_amazon_seller_partner-4.2.0/source_amazon_seller_partner/schemas/GET_FBA_INVENTORY_PLANNING_DATA.json
--rw-r--r--   0        0        0     1453 2024-03-21 01:47:20.313993 airbyte_source_amazon_seller_partner-4.2.0/source_amazon_seller_partner/schemas/GET_FBA_MYI_UNSUPPRESSED_INVENTORY_DATA.json
--rw-r--r--   0        0        0     1497 2024-03-21 01:47:20.313993 airbyte_source_amazon_seller_partner-4.2.0/source_amazon_seller_partner/schemas/GET_FBA_REIMBURSEMENTS_DATA.json
--rw-r--r--   0        0        0     1345 2024-03-21 01:47:20.313993 airbyte_source_amazon_seller_partner-4.2.0/source_amazon_seller_partner/schemas/GET_FBA_SNS_FORECAST_DATA.json
--rw-r--r--   0        0        0     1637 2024-03-21 01:47:20.313993 airbyte_source_amazon_seller_partner-4.2.0/source_amazon_seller_partner/schemas/GET_FBA_SNS_PERFORMANCE_DATA.json
--rw-r--r--   0        0        0     2397 2024-03-21 01:47:20.313993 airbyte_source_amazon_seller_partner-4.2.0/source_amazon_seller_partner/schemas/GET_FBA_STORAGE_FEE_CHARGES_DATA.json
--rw-r--r--   0        0        0     1999 2024-03-21 01:47:20.313993 airbyte_source_amazon_seller_partner-4.2.0/source_amazon_seller_partner/schemas/GET_FLAT_FILE_ACTIONABLE_ORDER_DATA_SHIPPING.json
--rw-r--r--   0        0        0     2464 2024-03-21 01:47:20.313993 airbyte_source_amazon_seller_partner-4.2.0/source_amazon_seller_partner/schemas/GET_FLAT_FILE_ALL_ORDERS_DATA_BY_LAST_UPDATE_GENERAL.json
--rw-r--r--   0        0        0     2471 2024-03-21 01:47:20.313993 airbyte_source_amazon_seller_partner-4.2.0/source_amazon_seller_partner/schemas/GET_FLAT_FILE_ALL_ORDERS_DATA_BY_ORDER_DATE_GENERAL.json
--rw-r--r--   0        0        0     1945 2024-03-21 01:47:20.313993 airbyte_source_amazon_seller_partner-4.2.0/source_amazon_seller_partner/schemas/GET_FLAT_FILE_ARCHIVED_ORDERS_DATA_BY_ORDER_DATE.json
--rw-r--r--   0        0        0     1833 2024-03-21 01:47:20.313993 airbyte_source_amazon_seller_partner-4.2.0/source_amazon_seller_partner/schemas/GET_FLAT_FILE_OPEN_LISTINGS_DATA.json
--rw-r--r--   0        0        0     2113 2024-03-21 01:47:20.313993 airbyte_source_amazon_seller_partner-4.2.0/source_amazon_seller_partner/schemas/GET_FLAT_FILE_RETURNS_DATA_BY_RETURN_DATE.json
--rw-r--r--   0        0        0     1033 2024-03-21 01:47:20.313993 airbyte_source_amazon_seller_partner-4.2.0/source_amazon_seller_partner/schemas/GET_LEDGER_DETAIL_VIEW_DATA.json
--rw-r--r--   0        0        0     1353 2024-03-21 01:47:20.313993 airbyte_source_amazon_seller_partner-4.2.0/source_amazon_seller_partner/schemas/GET_LEDGER_SUMMARY_VIEW_DATA.json
--rw-r--r--   0        0        0      645 2024-03-21 01:47:20.313993 airbyte_source_amazon_seller_partner-4.2.0/source_amazon_seller_partner/schemas/GET_MERCHANTS_LISTINGS_FYP_REPORT.json
--rw-r--r--   0        0        0     2590 2024-03-21 01:47:20.313993 airbyte_source_amazon_seller_partner-4.2.0/source_amazon_seller_partner/schemas/GET_MERCHANT_CANCELLED_LISTINGS_DATA.json
--rw-r--r--   0        0        0     2157 2024-03-21 01:47:20.313993 airbyte_source_amazon_seller_partner-4.2.0/source_amazon_seller_partner/schemas/GET_MERCHANT_LISTINGS_ALL_DATA.json
--rw-r--r--   0        0        0     2891 2024-03-21 01:47:20.313993 airbyte_source_amazon_seller_partner-4.2.0/source_amazon_seller_partner/schemas/GET_MERCHANT_LISTINGS_DATA.json
--rw-r--r--   0        0        0     2830 2024-03-21 01:47:20.317993 airbyte_source_amazon_seller_partner-4.2.0/source_amazon_seller_partner/schemas/GET_MERCHANT_LISTINGS_DATA_BACK_COMPAT.json
--rw-r--r--   0        0        0     1756 2024-03-21 01:47:20.317993 airbyte_source_amazon_seller_partner-4.2.0/source_amazon_seller_partner/schemas/GET_MERCHANT_LISTINGS_INACTIVE_DATA.json
--rw-r--r--   0        0        0     5258 2024-03-21 01:47:20.317993 airbyte_source_amazon_seller_partner-4.2.0/source_amazon_seller_partner/schemas/GET_ORDER_REPORT_DATA_SHIPPING.json
--rw-r--r--   0        0        0     2208 2024-03-21 01:47:20.317993 airbyte_source_amazon_seller_partner-4.2.0/source_amazon_seller_partner/schemas/GET_RESTOCK_INVENTORY_RECOMMENDATIONS_REPORT.json
--rw-r--r--   0        0        0     2235 2024-03-21 01:47:20.317993 airbyte_source_amazon_seller_partner-4.2.0/source_amazon_seller_partner/schemas/GET_SALES_AND_TRAFFIC_REPORT.json
--rw-r--r--   0        0        0      647 2024-03-21 01:47:20.317993 airbyte_source_amazon_seller_partner-4.2.0/source_amazon_seller_partner/schemas/GET_SELLER_FEEDBACK_DATA.json
--rw-r--r--   0        0        0     1250 2024-03-21 01:47:20.317993 airbyte_source_amazon_seller_partner-4.2.0/source_amazon_seller_partner/schemas/GET_STRANDED_INVENTORY_UI_DATA.json
--rw-r--r--   0        0        0     2408 2024-03-21 01:47:20.317993 airbyte_source_amazon_seller_partner-4.2.0/source_amazon_seller_partner/schemas/GET_V2_SETTLEMENT_REPORT_DATA_FLAT_FILE.json
--rw-r--r--   0        0        0      387 2024-03-21 01:47:20.317993 airbyte_source_amazon_seller_partner-4.2.0/source_amazon_seller_partner/schemas/GET_VENDOR_FORECASTING_FRESH_REPORT.json
--rw-r--r--   0        0        0      388 2024-03-21 01:47:20.317993 airbyte_source_amazon_seller_partner-4.2.0/source_amazon_seller_partner/schemas/GET_VENDOR_FORECASTING_RETAIL_REPORT.json
--rw-r--r--   0        0        0     2154 2024-03-21 01:47:20.317993 airbyte_source_amazon_seller_partner-4.2.0/source_amazon_seller_partner/schemas/GET_VENDOR_INVENTORY_REPORT.json
--rw-r--r--   0        0        0      979 2024-03-21 01:47:20.317993 airbyte_source_amazon_seller_partner-4.2.0/source_amazon_seller_partner/schemas/GET_VENDOR_NET_PURE_PRODUCT_MARGIN_REPORT.json
--rw-r--r--   0        0        0      812 2024-03-21 01:47:20.317993 airbyte_source_amazon_seller_partner-4.2.0/source_amazon_seller_partner/schemas/GET_VENDOR_REAL_TIME_INVENTORY_REPORT.json
--rw-r--r--   0        0        0     1269 2024-03-21 01:47:20.317993 airbyte_source_amazon_seller_partner-4.2.0/source_amazon_seller_partner/schemas/GET_VENDOR_SALES_REPORT.json
--rw-r--r--   0        0        0      940 2024-03-21 01:47:20.317993 airbyte_source_amazon_seller_partner-4.2.0/source_amazon_seller_partner/schemas/GET_VENDOR_TRAFFIC_REPORT.json
--rw-r--r--   0        0        0     2255 2024-03-21 01:47:20.317993 airbyte_source_amazon_seller_partner-4.2.0/source_amazon_seller_partner/schemas/GET_XML_ALL_ORDERS_DATA_BY_ORDER_DATE_GENERAL.json
--rw-r--r--   0        0        0     2266 2024-03-21 01:47:20.317993 airbyte_source_amazon_seller_partner-4.2.0/source_amazon_seller_partner/schemas/GET_XML_BROWSE_TREE_DATA.json
--rw-r--r--   0        0        0     1543 2024-03-21 01:47:20.317993 airbyte_source_amazon_seller_partner-4.2.0/source_amazon_seller_partner/schemas/ListFinancialEventGroups.json
--rw-r--r--   0        0        0    25722 2024-03-21 01:47:20.317993 airbyte_source_amazon_seller_partner-4.2.0/source_amazon_seller_partner/schemas/ListFinancialEvents.json
--rw-r--r--   0        0        0     6713 2024-03-21 01:47:20.317993 airbyte_source_amazon_seller_partner-4.2.0/source_amazon_seller_partner/schemas/OrderItems.json
--rw-r--r--   0        0        0     3950 2024-03-21 01:47:20.317993 airbyte_source_amazon_seller_partner-4.2.0/source_amazon_seller_partner/schemas/Orders.json
--rw-r--r--   0        0        0     6865 2024-03-21 01:47:20.317993 airbyte_source_amazon_seller_partner-4.2.0/source_amazon_seller_partner/schemas/VendorDirectFulfillmentShipping.json
--rw-r--r--   0        0        0    10312 2024-03-21 01:47:20.317993 airbyte_source_amazon_seller_partner-4.2.0/source_amazon_seller_partner/schemas/VendorOrders.json
--rw-r--r--   0        0        0      605 2024-03-21 01:47:20.317993 airbyte_source_amazon_seller_partner-4.2.0/source_amazon_seller_partner/schemas/shared/GET_VENDOR_FORECASTING_REPORT.json
--rw-r--r--   0        0        0    10019 2024-03-21 01:47:20.317993 airbyte_source_amazon_seller_partner-4.2.0/source_amazon_seller_partner/source.py
--rw-r--r--   0        0        0     8913 2024-03-21 01:47:20.317993 airbyte_source_amazon_seller_partner-4.2.0/source_amazon_seller_partner/spec.json
--rw-r--r--   0        0        0    57062 2024-03-21 01:47:20.317993 airbyte_source_amazon_seller_partner-4.2.0/source_amazon_seller_partner/streams.py
--rw-r--r--   0        0        0      403 2024-03-21 01:47:20.317993 airbyte_source_amazon_seller_partner-4.2.0/source_amazon_seller_partner/utils.py
--rw-r--r--   0        0        0     5587 1970-01-01 00:00:00.000000 airbyte_source_amazon_seller_partner-4.2.0/PKG-INFO
+-rw-r--r--   0        0        0     4765 2024-04-10 13:21:02.682068 airbyte_source_amazon_seller_partner-4.2.1/README.md
+-rw-r--r--   0        0        0      895 2024-04-10 13:24:04.473507 airbyte_source_amazon_seller_partner-4.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1191 2024-04-10 13:21:02.686068 airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/__init__.py
+-rw-r--r--   0        0        0      638 2024-04-10 13:21:02.686068 airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/auth.py
+-rw-r--r--   0        0        0     6322 2024-04-10 13:21:02.686068 airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/config_migrations.py
+-rw-r--r--   0        0        0     3387 2024-04-10 13:21:02.686068 airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/constants.py
+-rw-r--r--   0        0        0      479 2024-04-10 13:21:02.686068 airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/run.py
+-rw-r--r--   0        0        0      576 2024-04-10 13:21:02.686068 airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_AFN_INVENTORY_DATA.json
+-rw-r--r--   0        0        0      568 2024-04-10 13:21:02.686068 airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_AFN_INVENTORY_DATA_BY_COUNTRY.json
+-rw-r--r--   0        0        0     2997 2024-04-10 13:21:02.686068 airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_AMAZON_FULFILLED_SHIPMENTS_DATA_GENERAL.json
+-rw-r--r--   0        0        0      799 2024-04-10 13:21:02.686068 airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_BRAND_ANALYTICS_MARKET_BASKET_REPORT.json
+-rw-r--r--   0        0        0     1112 2024-04-10 13:21:02.686068 airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_BRAND_ANALYTICS_REPEAT_PURCHASE_REPORT.json
+-rw-r--r--   0        0        0      823 2024-04-10 13:21:02.686068 airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_BRAND_ANALYTICS_SEARCH_TERMS_REPORT.json
+-rw-r--r--   0        0        0     2434 2024-04-10 13:21:02.686068 airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_FBA_ESTIMATED_FBA_FEES_TXT_DATA.json
+-rw-r--r--   0        0        0      950 2024-04-10 13:21:02.686068 airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_FBA_FULFILLMENT_CUSTOMER_RETURNS_DATA.json
+-rw-r--r--   0        0        0      744 2024-04-10 13:21:02.686068 airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_FBA_FULFILLMENT_CUSTOMER_SHIPMENT_PROMOTION_DATA.json
+-rw-r--r--   0        0        0     1816 2024-04-10 13:21:02.686068 airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_FBA_FULFILLMENT_CUSTOMER_SHIPMENT_REPLACEMENT_DATA.json
+-rw-r--r--   0        0        0     1305 2024-04-10 13:21:02.686068 airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_FBA_FULFILLMENT_REMOVAL_ORDER_DETAIL_DATA.json
+-rw-r--r--   0        0        0      916 2024-04-10 13:21:02.686068 airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_FBA_FULFILLMENT_REMOVAL_SHIPMENT_DETAIL_DATA.json
+-rw-r--r--   0        0        0     4986 2024-04-10 13:21:02.686068 airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_FBA_INVENTORY_PLANNING_DATA.json
+-rw-r--r--   0        0        0     1453 2024-04-10 13:21:02.686068 airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_FBA_MYI_UNSUPPRESSED_INVENTORY_DATA.json
+-rw-r--r--   0        0        0     1497 2024-04-10 13:21:02.686068 airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_FBA_REIMBURSEMENTS_DATA.json
+-rw-r--r--   0        0        0     1345 2024-04-10 13:21:02.686068 airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_FBA_SNS_FORECAST_DATA.json
+-rw-r--r--   0        0        0     1637 2024-04-10 13:21:02.686068 airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_FBA_SNS_PERFORMANCE_DATA.json
+-rw-r--r--   0        0        0     2397 2024-04-10 13:21:02.686068 airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_FBA_STORAGE_FEE_CHARGES_DATA.json
+-rw-r--r--   0        0        0     1999 2024-04-10 13:21:02.686068 airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_FLAT_FILE_ACTIONABLE_ORDER_DATA_SHIPPING.json
+-rw-r--r--   0        0        0     2464 2024-04-10 13:21:02.686068 airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_FLAT_FILE_ALL_ORDERS_DATA_BY_LAST_UPDATE_GENERAL.json
+-rw-r--r--   0        0        0     2471 2024-04-10 13:21:02.686068 airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_FLAT_FILE_ALL_ORDERS_DATA_BY_ORDER_DATE_GENERAL.json
+-rw-r--r--   0        0        0     1945 2024-04-10 13:21:02.686068 airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_FLAT_FILE_ARCHIVED_ORDERS_DATA_BY_ORDER_DATE.json
+-rw-r--r--   0        0        0     1833 2024-04-10 13:21:02.686068 airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_FLAT_FILE_OPEN_LISTINGS_DATA.json
+-rw-r--r--   0        0        0     2113 2024-04-10 13:21:02.686068 airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_FLAT_FILE_RETURNS_DATA_BY_RETURN_DATE.json
+-rw-r--r--   0        0        0     1033 2024-04-10 13:21:02.686068 airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_LEDGER_DETAIL_VIEW_DATA.json
+-rw-r--r--   0        0        0     1353 2024-04-10 13:21:02.686068 airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_LEDGER_SUMMARY_VIEW_DATA.json
+-rw-r--r--   0        0        0      645 2024-04-10 13:21:02.686068 airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_MERCHANTS_LISTINGS_FYP_REPORT.json
+-rw-r--r--   0        0        0     2590 2024-04-10 13:21:02.686068 airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_MERCHANT_CANCELLED_LISTINGS_DATA.json
+-rw-r--r--   0        0        0     2157 2024-04-10 13:21:02.686068 airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_MERCHANT_LISTINGS_ALL_DATA.json
+-rw-r--r--   0        0        0     2891 2024-04-10 13:21:02.686068 airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_MERCHANT_LISTINGS_DATA.json
+-rw-r--r--   0        0        0     2830 2024-04-10 13:21:02.686068 airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_MERCHANT_LISTINGS_DATA_BACK_COMPAT.json
+-rw-r--r--   0        0        0     1756 2024-04-10 13:21:02.686068 airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_MERCHANT_LISTINGS_INACTIVE_DATA.json
+-rw-r--r--   0        0        0     5258 2024-04-10 13:21:02.686068 airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_ORDER_REPORT_DATA_SHIPPING.json
+-rw-r--r--   0        0        0     2208 2024-04-10 13:21:02.686068 airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_RESTOCK_INVENTORY_RECOMMENDATIONS_REPORT.json
+-rw-r--r--   0        0        0     2235 2024-04-10 13:21:02.686068 airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_SALES_AND_TRAFFIC_REPORT.json
+-rw-r--r--   0        0        0      647 2024-04-10 13:21:02.686068 airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_SELLER_FEEDBACK_DATA.json
+-rw-r--r--   0        0        0     1250 2024-04-10 13:21:02.686068 airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_STRANDED_INVENTORY_UI_DATA.json
+-rw-r--r--   0        0        0     2408 2024-04-10 13:21:02.686068 airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_V2_SETTLEMENT_REPORT_DATA_FLAT_FILE.json
+-rw-r--r--   0        0        0      387 2024-04-10 13:21:02.686068 airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_VENDOR_FORECASTING_FRESH_REPORT.json
+-rw-r--r--   0        0        0      388 2024-04-10 13:21:02.686068 airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_VENDOR_FORECASTING_RETAIL_REPORT.json
+-rw-r--r--   0        0        0     2154 2024-04-10 13:21:02.686068 airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_VENDOR_INVENTORY_REPORT.json
+-rw-r--r--   0        0        0      979 2024-04-10 13:21:02.686068 airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_VENDOR_NET_PURE_PRODUCT_MARGIN_REPORT.json
+-rw-r--r--   0        0        0      812 2024-04-10 13:21:02.686068 airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_VENDOR_REAL_TIME_INVENTORY_REPORT.json
+-rw-r--r--   0        0        0     1269 2024-04-10 13:21:02.686068 airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_VENDOR_SALES_REPORT.json
+-rw-r--r--   0        0        0      940 2024-04-10 13:21:02.686068 airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_VENDOR_TRAFFIC_REPORT.json
+-rw-r--r--   0        0        0     2255 2024-04-10 13:21:02.686068 airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_XML_ALL_ORDERS_DATA_BY_ORDER_DATE_GENERAL.json
+-rw-r--r--   0        0        0     2266 2024-04-10 13:21:02.686068 airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_XML_BROWSE_TREE_DATA.json
+-rw-r--r--   0        0        0     1543 2024-04-10 13:21:02.686068 airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/ListFinancialEventGroups.json
+-rw-r--r--   0        0        0    25722 2024-04-10 13:21:02.686068 airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/ListFinancialEvents.json
+-rw-r--r--   0        0        0     6713 2024-04-10 13:21:02.686068 airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/OrderItems.json
+-rw-r--r--   0        0        0     3950 2024-04-10 13:21:02.686068 airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/Orders.json
+-rw-r--r--   0        0        0     6865 2024-04-10 13:21:02.686068 airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/VendorDirectFulfillmentShipping.json
+-rw-r--r--   0        0        0    10312 2024-04-10 13:21:02.686068 airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/VendorOrders.json
+-rw-r--r--   0        0        0      605 2024-04-10 13:21:02.686068 airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/shared/GET_VENDOR_FORECASTING_REPORT.json
+-rw-r--r--   0        0        0    10019 2024-04-10 13:21:02.686068 airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/source.py
+-rw-r--r--   0        0        0     8913 2024-04-10 13:21:02.686068 airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/spec.json
+-rw-r--r--   0        0        0    56375 2024-04-10 13:21:02.690068 airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/streams.py
+-rw-r--r--   0        0        0      403 2024-04-10 13:21:02.690068 airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/utils.py
+-rw-r--r--   0        0        0     5587 1970-01-01 00:00:00.000000 airbyte_source_amazon_seller_partner-4.2.1/PKG-INFO
```

### Comparing `airbyte_source_amazon_seller_partner-4.2.0/README.md` & `airbyte_source_amazon_seller_partner-4.2.1/README.md`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.0/pyproject.toml` & `airbyte_source_amazon_seller_partner-4.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "4.2.0"
+version = "4.2.1"
 name = "airbyte-source-amazon-seller-partner"
 description = "Source implementation for Amazon Seller Partner."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "MIT"
 readme = "README.md"
```

### Comparing `airbyte_source_amazon_seller_partner-4.2.0/source_amazon_seller_partner/__init__.py` & `airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/__init__.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.0/source_amazon_seller_partner/auth.py` & `airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/auth.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.0/source_amazon_seller_partner/config_migrations.py` & `airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/config_migrations.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.0/source_amazon_seller_partner/constants.py` & `airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/constants.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.0/source_amazon_seller_partner/schemas/GET_AFN_INVENTORY_DATA.json` & `airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_AFN_INVENTORY_DATA.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.0/source_amazon_seller_partner/schemas/GET_AFN_INVENTORY_DATA_BY_COUNTRY.json` & `airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_AFN_INVENTORY_DATA_BY_COUNTRY.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.0/source_amazon_seller_partner/schemas/GET_AMAZON_FULFILLED_SHIPMENTS_DATA_GENERAL.json` & `airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_AMAZON_FULFILLED_SHIPMENTS_DATA_GENERAL.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.0/source_amazon_seller_partner/schemas/GET_BRAND_ANALYTICS_MARKET_BASKET_REPORT.json` & `airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_BRAND_ANALYTICS_MARKET_BASKET_REPORT.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.0/source_amazon_seller_partner/schemas/GET_BRAND_ANALYTICS_REPEAT_PURCHASE_REPORT.json` & `airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_BRAND_ANALYTICS_REPEAT_PURCHASE_REPORT.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.0/source_amazon_seller_partner/schemas/GET_BRAND_ANALYTICS_SEARCH_TERMS_REPORT.json` & `airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_BRAND_ANALYTICS_SEARCH_TERMS_REPORT.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.0/source_amazon_seller_partner/schemas/GET_FBA_ESTIMATED_FBA_FEES_TXT_DATA.json` & `airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_FBA_ESTIMATED_FBA_FEES_TXT_DATA.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.0/source_amazon_seller_partner/schemas/GET_FBA_FULFILLMENT_CUSTOMER_RETURNS_DATA.json` & `airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_FBA_FULFILLMENT_CUSTOMER_RETURNS_DATA.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.0/source_amazon_seller_partner/schemas/GET_FBA_FULFILLMENT_CUSTOMER_SHIPMENT_PROMOTION_DATA.json` & `airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_FBA_FULFILLMENT_CUSTOMER_SHIPMENT_PROMOTION_DATA.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.0/source_amazon_seller_partner/schemas/GET_FBA_FULFILLMENT_CUSTOMER_SHIPMENT_REPLACEMENT_DATA.json` & `airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_FBA_FULFILLMENT_CUSTOMER_SHIPMENT_REPLACEMENT_DATA.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.0/source_amazon_seller_partner/schemas/GET_FBA_FULFILLMENT_REMOVAL_ORDER_DETAIL_DATA.json` & `airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_FBA_FULFILLMENT_REMOVAL_ORDER_DETAIL_DATA.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.0/source_amazon_seller_partner/schemas/GET_FBA_FULFILLMENT_REMOVAL_SHIPMENT_DETAIL_DATA.json` & `airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_FBA_FULFILLMENT_REMOVAL_SHIPMENT_DETAIL_DATA.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.0/source_amazon_seller_partner/schemas/GET_FBA_INVENTORY_PLANNING_DATA.json` & `airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_FBA_INVENTORY_PLANNING_DATA.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.0/source_amazon_seller_partner/schemas/GET_FBA_MYI_UNSUPPRESSED_INVENTORY_DATA.json` & `airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_FBA_MYI_UNSUPPRESSED_INVENTORY_DATA.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.0/source_amazon_seller_partner/schemas/GET_FBA_REIMBURSEMENTS_DATA.json` & `airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_FBA_REIMBURSEMENTS_DATA.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.0/source_amazon_seller_partner/schemas/GET_FBA_SNS_FORECAST_DATA.json` & `airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_FBA_SNS_FORECAST_DATA.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.0/source_amazon_seller_partner/schemas/GET_FBA_SNS_PERFORMANCE_DATA.json` & `airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_FBA_SNS_PERFORMANCE_DATA.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.0/source_amazon_seller_partner/schemas/GET_FBA_STORAGE_FEE_CHARGES_DATA.json` & `airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_FBA_STORAGE_FEE_CHARGES_DATA.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.0/source_amazon_seller_partner/schemas/GET_FLAT_FILE_ACTIONABLE_ORDER_DATA_SHIPPING.json` & `airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_FLAT_FILE_ACTIONABLE_ORDER_DATA_SHIPPING.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.0/source_amazon_seller_partner/schemas/GET_FLAT_FILE_ALL_ORDERS_DATA_BY_LAST_UPDATE_GENERAL.json` & `airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_FLAT_FILE_ALL_ORDERS_DATA_BY_LAST_UPDATE_GENERAL.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.0/source_amazon_seller_partner/schemas/GET_FLAT_FILE_ALL_ORDERS_DATA_BY_ORDER_DATE_GENERAL.json` & `airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_FLAT_FILE_ALL_ORDERS_DATA_BY_ORDER_DATE_GENERAL.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.0/source_amazon_seller_partner/schemas/GET_FLAT_FILE_ARCHIVED_ORDERS_DATA_BY_ORDER_DATE.json` & `airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_FLAT_FILE_ARCHIVED_ORDERS_DATA_BY_ORDER_DATE.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.0/source_amazon_seller_partner/schemas/GET_FLAT_FILE_OPEN_LISTINGS_DATA.json` & `airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_FLAT_FILE_OPEN_LISTINGS_DATA.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.0/source_amazon_seller_partner/schemas/GET_FLAT_FILE_RETURNS_DATA_BY_RETURN_DATE.json` & `airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_FLAT_FILE_RETURNS_DATA_BY_RETURN_DATE.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.0/source_amazon_seller_partner/schemas/GET_LEDGER_DETAIL_VIEW_DATA.json` & `airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_LEDGER_DETAIL_VIEW_DATA.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.0/source_amazon_seller_partner/schemas/GET_LEDGER_SUMMARY_VIEW_DATA.json` & `airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_LEDGER_SUMMARY_VIEW_DATA.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.0/source_amazon_seller_partner/schemas/GET_MERCHANTS_LISTINGS_FYP_REPORT.json` & `airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_MERCHANTS_LISTINGS_FYP_REPORT.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.0/source_amazon_seller_partner/schemas/GET_MERCHANT_CANCELLED_LISTINGS_DATA.json` & `airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_MERCHANT_CANCELLED_LISTINGS_DATA.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.0/source_amazon_seller_partner/schemas/GET_MERCHANT_LISTINGS_ALL_DATA.json` & `airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_MERCHANT_LISTINGS_ALL_DATA.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.0/source_amazon_seller_partner/schemas/GET_MERCHANT_LISTINGS_DATA.json` & `airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_MERCHANT_LISTINGS_DATA.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.0/source_amazon_seller_partner/schemas/GET_MERCHANT_LISTINGS_DATA_BACK_COMPAT.json` & `airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_MERCHANT_LISTINGS_DATA_BACK_COMPAT.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.0/source_amazon_seller_partner/schemas/GET_MERCHANT_LISTINGS_INACTIVE_DATA.json` & `airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_MERCHANT_LISTINGS_INACTIVE_DATA.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.0/source_amazon_seller_partner/schemas/GET_ORDER_REPORT_DATA_SHIPPING.json` & `airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_ORDER_REPORT_DATA_SHIPPING.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.0/source_amazon_seller_partner/schemas/GET_RESTOCK_INVENTORY_RECOMMENDATIONS_REPORT.json` & `airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_RESTOCK_INVENTORY_RECOMMENDATIONS_REPORT.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.0/source_amazon_seller_partner/schemas/GET_SALES_AND_TRAFFIC_REPORT.json` & `airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_SALES_AND_TRAFFIC_REPORT.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.0/source_amazon_seller_partner/schemas/GET_SELLER_FEEDBACK_DATA.json` & `airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_SELLER_FEEDBACK_DATA.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.0/source_amazon_seller_partner/schemas/GET_STRANDED_INVENTORY_UI_DATA.json` & `airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_STRANDED_INVENTORY_UI_DATA.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.0/source_amazon_seller_partner/schemas/GET_V2_SETTLEMENT_REPORT_DATA_FLAT_FILE.json` & `airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_V2_SETTLEMENT_REPORT_DATA_FLAT_FILE.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.0/source_amazon_seller_partner/schemas/GET_VENDOR_INVENTORY_REPORT.json` & `airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_VENDOR_INVENTORY_REPORT.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.0/source_amazon_seller_partner/schemas/GET_VENDOR_NET_PURE_PRODUCT_MARGIN_REPORT.json` & `airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_VENDOR_NET_PURE_PRODUCT_MARGIN_REPORT.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.0/source_amazon_seller_partner/schemas/GET_VENDOR_REAL_TIME_INVENTORY_REPORT.json` & `airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_VENDOR_REAL_TIME_INVENTORY_REPORT.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.0/source_amazon_seller_partner/schemas/GET_VENDOR_SALES_REPORT.json` & `airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_VENDOR_SALES_REPORT.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.0/source_amazon_seller_partner/schemas/GET_VENDOR_TRAFFIC_REPORT.json` & `airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_VENDOR_TRAFFIC_REPORT.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.0/source_amazon_seller_partner/schemas/GET_XML_ALL_ORDERS_DATA_BY_ORDER_DATE_GENERAL.json` & `airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_XML_ALL_ORDERS_DATA_BY_ORDER_DATE_GENERAL.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.0/source_amazon_seller_partner/schemas/GET_XML_BROWSE_TREE_DATA.json` & `airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/GET_XML_BROWSE_TREE_DATA.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.0/source_amazon_seller_partner/schemas/ListFinancialEventGroups.json` & `airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/ListFinancialEventGroups.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.0/source_amazon_seller_partner/schemas/ListFinancialEvents.json` & `airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/ListFinancialEvents.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.0/source_amazon_seller_partner/schemas/OrderItems.json` & `airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/OrderItems.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.0/source_amazon_seller_partner/schemas/Orders.json` & `airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/Orders.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.0/source_amazon_seller_partner/schemas/VendorDirectFulfillmentShipping.json` & `airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/VendorDirectFulfillmentShipping.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.0/source_amazon_seller_partner/schemas/VendorOrders.json` & `airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/VendorOrders.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.0/source_amazon_seller_partner/schemas/shared/GET_VENDOR_FORECASTING_REPORT.json` & `airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/schemas/shared/GET_VENDOR_FORECASTING_REPORT.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.0/source_amazon_seller_partner/source.py` & `airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/source.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.0/source_amazon_seller_partner/spec.json` & `airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/spec.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_amazon_seller_partner-4.2.0/source_amazon_seller_partner/streams.py` & `airbyte_source_amazon_seller_partner-4.2.1/source_amazon_seller_partner/streams.py`

 * *Files 1% similar despite different names*

```diff
@@ -704,15 +704,15 @@
         sync_mode: SyncMode,
         cursor_field: List[str] = None,
         stream_slice: Mapping[str, Any] = None,
         stream_state: Mapping[str, Any] = None,
     ) -> Mapping[str, Any]:
         data = super()._report_data(sync_mode, cursor_field, stream_slice, stream_state)
         options = self.report_options()
-        if options and options.get("reportPeriod") is not None:
+        if options and options.get("reportPeriod"):
             data.update(self._augmented_data(options))
         return data
 
     def _augmented_data(self, report_options) -> Mapping[str, Any]:
         now = pendulum.now("utc")
         if report_options["reportPeriod"] == "DAY":
             now = now.subtract(days=self.availability_sla_days)
@@ -748,32 +748,14 @@
 class IncrementalAnalyticsStream(AnalyticsStream):
     fixed_period_in_days = 0
 
     @property
     def cursor_field(self) -> Union[str, List[str]]:
         return "endDate"
 
-    def _report_data(
-        self,
-        sync_mode: SyncMode,
-        cursor_field: List[str] = None,
-        stream_slice: Mapping[str, Any] = None,
-        stream_state: Mapping[str, Any] = None,
-    ) -> Mapping[str, Any]:
-        data = super()._report_data(sync_mode, cursor_field, stream_slice, stream_state)
-        if stream_slice:
-            data_times = {}
-            if stream_slice.get("dataStartTime"):
-                data_times["dataStartTime"] = stream_slice["dataStartTime"]
-            if stream_slice.get("dataEndTime"):
-                data_times["dataEndTime"] = stream_slice["dataEndTime"]
-            data.update(data_times)
-
-        return data
-
     def parse_response(
         self,
         response: requests.Response,
         stream_state: Mapping[str, Any] = None,
         stream_slice: Mapping[str, Any] = None,
         **kwargs: Any,
     ) -> Iterable[Mapping]:
```

### Comparing `airbyte_source_amazon_seller_partner-4.2.0/PKG-INFO` & `airbyte_source_amazon_seller_partner-4.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airbyte-source-amazon-seller-partner
-Version: 4.2.0
+Version: 4.2.1
 Summary: Source implementation for Amazon Seller Partner.
 Home-page: https://airbyte.com
 License: MIT
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
```

