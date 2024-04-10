# Comparing `tmp/airbyte_source_shopify-2.0.5.dev202404081102.tar.gz` & `tmp/airbyte_source_shopify-2.0.5.dev202404101100.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_shopify-2.0.5.dev202404081102.tar", max compression
+gzip compressed data, was "airbyte_source_shopify-2.0.5.dev202404101100.tar", max compression
```

## Comparing `airbyte_source_shopify-2.0.5.dev202404081102.tar` & `airbyte_source_shopify-2.0.5.dev202404101100.tar`

### file list

```diff
@@ -1,66 +1,66 @@
--rw-r--r--   0        0        0     4519 2024-04-08 10:39:25.000000 airbyte_source_shopify-2.0.5.dev202404081102/README.md
--rw-r--r--   0        0        0      812 2024-04-08 11:02:50.263613 airbyte_source_shopify-2.0.5.dev202404081102/pyproject.toml
--rw-r--r--   0        0        0     1136 2024-04-08 10:39:25.000000 airbyte_source_shopify-2.0.5.dev202404081102/source_shopify/__init__.py
--rw-r--r--   0        0        0     1538 2024-04-08 10:39:25.000000 airbyte_source_shopify-2.0.5.dev202404081102/source_shopify/auth.py
--rw-r--r--   0        0        0     3797 2024-04-08 10:39:25.000000 airbyte_source_shopify-2.0.5.dev202404081102/source_shopify/config_migrations.py
--rw-r--r--   0        0        0      398 2024-04-08 10:39:25.000000 airbyte_source_shopify-2.0.5.dev202404081102/source_shopify/run.py
--rw-r--r--   0        0        0    16103 2024-04-08 10:39:25.000000 airbyte_source_shopify-2.0.5.dev202404081102/source_shopify/schemas/abandoned_checkouts.json
--rw-r--r--   0        0        0     1272 2024-04-08 10:39:25.000000 airbyte_source_shopify-2.0.5.dev202404081102/source_shopify/schemas/articles.json
--rw-r--r--   0        0        0     1009 2024-04-08 10:39:25.000000 airbyte_source_shopify-2.0.5.dev202404081102/source_shopify/schemas/balance_transactions.json
--rw-r--r--   0        0        0     1109 2024-04-08 10:39:25.000000 airbyte_source_shopify-2.0.5.dev202404081102/source_shopify/schemas/blogs.json
--rw-r--r--   0        0        0      928 2024-04-08 10:39:25.000000 airbyte_source_shopify-2.0.5.dev202404081102/source_shopify/schemas/collections.json
--rw-r--r--   0        0        0      610 2024-04-08 10:39:25.000000 airbyte_source_shopify-2.0.5.dev202404081102/source_shopify/schemas/collects.json
--rw-r--r--   0        0        0     1170 2024-04-08 10:39:25.000000 airbyte_source_shopify-2.0.5.dev202404081102/source_shopify/schemas/countries.json
--rw-r--r--   0        0        0     1488 2024-04-08 10:39:25.000000 airbyte_source_shopify-2.0.5.dev202404081102/source_shopify/schemas/custom_collections.json
--rw-r--r--   0        0        0     1217 2024-04-08 10:39:25.000000 airbyte_source_shopify-2.0.5.dev202404081102/source_shopify/schemas/customer_address.json
--rw-r--r--   0        0        0      485 2024-04-08 10:39:25.000000 airbyte_source_shopify-2.0.5.dev202404081102/source_shopify/schemas/customer_saved_search.json
--rw-r--r--   0        0        0     5313 2024-04-08 10:39:25.000000 airbyte_source_shopify-2.0.5.dev202404081102/source_shopify/schemas/customers.json
--rw-r--r--   0        0        0      736 2024-04-08 10:39:25.000000 airbyte_source_shopify-2.0.5.dev202404081102/source_shopify/schemas/discount_codes.json
--rw-r--r--   0        0        0      909 2024-04-08 10:39:25.000000 airbyte_source_shopify-2.0.5.dev202404081102/source_shopify/schemas/disputes.json
--rw-r--r--   0        0        0    13381 2024-04-08 10:39:25.000000 airbyte_source_shopify-2.0.5.dev202404081102/source_shopify/schemas/draft_orders.json
--rw-r--r--   0        0        0     5226 2024-04-08 10:39:25.000000 airbyte_source_shopify-2.0.5.dev202404081102/source_shopify/schemas/fulfillment_orders.json
--rw-r--r--   0        0        0    14757 2024-04-08 10:39:25.000000 airbyte_source_shopify-2.0.5.dev202404081102/source_shopify/schemas/fulfillments.json
--rw-r--r--   0        0        0     1027 2024-04-08 10:39:25.000000 airbyte_source_shopify-2.0.5.dev202404081102/source_shopify/schemas/inventory_items.json
--rw-r--r--   0        0        0      536 2024-04-08 10:39:25.000000 airbyte_source_shopify-2.0.5.dev202404081102/source_shopify/schemas/inventory_levels.json
--rw-r--r--   0        0        0     1329 2024-04-08 10:39:25.000000 airbyte_source_shopify-2.0.5.dev202404081102/source_shopify/schemas/locations.json
--rw-r--r--   0        0        0      911 2024-04-08 10:39:25.000000 airbyte_source_shopify-2.0.5.dev202404081102/source_shopify/schemas/metafield_articles.json
--rw-r--r--   0        0        0      911 2024-04-08 10:39:25.000000 airbyte_source_shopify-2.0.5.dev202404081102/source_shopify/schemas/metafield_blogs.json
--rw-r--r--   0        0        0      911 2024-04-08 10:39:25.000000 airbyte_source_shopify-2.0.5.dev202404081102/source_shopify/schemas/metafield_collections.json
--rw-r--r--   0        0        0      911 2024-04-08 10:39:25.000000 airbyte_source_shopify-2.0.5.dev202404081102/source_shopify/schemas/metafield_customers.json
--rw-r--r--   0        0        0      911 2024-04-08 10:39:25.000000 airbyte_source_shopify-2.0.5.dev202404081102/source_shopify/schemas/metafield_draft_orders.json
--rw-r--r--   0        0        0      911 2024-04-08 10:39:25.000000 airbyte_source_shopify-2.0.5.dev202404081102/source_shopify/schemas/metafield_locations.json
--rw-r--r--   0        0        0      911 2024-04-08 10:39:25.000000 airbyte_source_shopify-2.0.5.dev202404081102/source_shopify/schemas/metafield_orders.json
--rw-r--r--   0        0        0      911 2024-04-08 10:39:25.000000 airbyte_source_shopify-2.0.5.dev202404081102/source_shopify/schemas/metafield_pages.json
--rw-r--r--   0        0        0      911 2024-04-08 10:39:25.000000 airbyte_source_shopify-2.0.5.dev202404081102/source_shopify/schemas/metafield_product_images.json
--rw-r--r--   0        0        0      911 2024-04-08 10:39:25.000000 airbyte_source_shopify-2.0.5.dev202404081102/source_shopify/schemas/metafield_product_variants.json
--rw-r--r--   0        0        0      911 2024-04-08 10:39:25.000000 airbyte_source_shopify-2.0.5.dev202404081102/source_shopify/schemas/metafield_products.json
--rw-r--r--   0        0        0      911 2024-04-08 10:39:25.000000 airbyte_source_shopify-2.0.5.dev202404081102/source_shopify/schemas/metafield_shops.json
--rw-r--r--   0        0        0      911 2024-04-08 10:39:25.000000 airbyte_source_shopify-2.0.5.dev202404081102/source_shopify/schemas/metafield_smart_collections.json
--rw-r--r--   0        0        0    17520 2024-04-08 10:39:25.000000 airbyte_source_shopify-2.0.5.dev202404081102/source_shopify/schemas/order_refunds.json
--rw-r--r--   0        0        0      728 2024-04-08 10:39:25.000000 airbyte_source_shopify-2.0.5.dev202404081102/source_shopify/schemas/order_risks.json
--rw-r--r--   0        0        0    80187 2024-04-08 10:39:25.000000 airbyte_source_shopify-2.0.5.dev202404081102/source_shopify/schemas/orders.json
--rw-r--r--   0        0        0     1104 2024-04-08 10:39:25.000000 airbyte_source_shopify-2.0.5.dev202404081102/source_shopify/schemas/pages.json
--rw-r--r--   0        0        0     3891 2024-04-08 10:39:25.000000 airbyte_source_shopify-2.0.5.dev202404081102/source_shopify/schemas/price_rules.json
--rw-r--r--   0        0        0      907 2024-04-08 10:39:25.000000 airbyte_source_shopify-2.0.5.dev202404081102/source_shopify/schemas/product_images.json
--rw-r--r--   0        0        0     2336 2024-04-08 10:39:25.000000 airbyte_source_shopify-2.0.5.dev202404081102/source_shopify/schemas/product_variants.json
--rw-r--r--   0        0        0     7060 2024-04-08 10:39:25.000000 airbyte_source_shopify-2.0.5.dev202404081102/source_shopify/schemas/products.json
--rw-r--r--   0        0        0     1675 2024-04-08 10:39:25.000000 airbyte_source_shopify-2.0.5.dev202404081102/source_shopify/schemas/products_graph_ql.json
--rw-r--r--   0        0        0     4059 2024-04-08 10:39:25.000000 airbyte_source_shopify-2.0.5.dev202404081102/source_shopify/schemas/shop.json
--rw-r--r--   0        0        0      985 2024-04-08 10:39:25.000000 airbyte_source_shopify-2.0.5.dev202404081102/source_shopify/schemas/smart_collections.json
--rw-r--r--   0        0        0      951 2024-04-08 10:39:25.000000 airbyte_source_shopify-2.0.5.dev202404081102/source_shopify/schemas/tender_transactions.json
--rw-r--r--   0        0        0     3750 2024-04-08 10:39:25.000000 airbyte_source_shopify-2.0.5.dev202404081102/source_shopify/schemas/transactions.json
--rw-r--r--   0        0        0     6367 2024-04-08 10:39:25.000000 airbyte_source_shopify-2.0.5.dev202404081102/source_shopify/scopes.py
--rw-r--r--   0        0        0     1734 2024-04-08 10:39:25.000000 airbyte_source_shopify-2.0.5.dev202404081102/source_shopify/shopify_graphql/bulk/exceptions.py
--rw-r--r--   0        0        0    15543 2024-04-08 10:39:25.000000 airbyte_source_shopify-2.0.5.dev202404081102/source_shopify/shopify_graphql/bulk/job.py
--rw-r--r--   0        0        0    55609 2024-04-08 10:39:25.000000 airbyte_source_shopify-2.0.5.dev202404081102/source_shopify/shopify_graphql/bulk/query.py
--rw-r--r--   0        0        0     6517 2024-04-08 10:39:25.000000 airbyte_source_shopify-2.0.5.dev202404081102/source_shopify/shopify_graphql/bulk/record.py
--rw-r--r--   0        0        0     3629 2024-04-08 10:39:25.000000 airbyte_source_shopify-2.0.5.dev202404081102/source_shopify/shopify_graphql/bulk/tools.py
--rw-r--r--   0        0        0     1969 2024-04-08 10:39:25.000000 airbyte_source_shopify-2.0.5.dev202404081102/source_shopify/shopify_graphql/graphql.py
--rw-r--r--   0        0        0  1354903 2024-04-08 10:39:25.000000 airbyte_source_shopify-2.0.5.dev202404081102/source_shopify/shopify_graphql/schema.py
--rw-r--r--   0        0        0     8540 2024-04-08 10:39:25.000000 airbyte_source_shopify-2.0.5.dev202404081102/source_shopify/source.py
--rw-r--r--   0        0        0     5118 2024-04-08 10:39:25.000000 airbyte_source_shopify-2.0.5.dev202404081102/source_shopify/spec.json
--rw-r--r--   0        0        0    35441 2024-04-08 10:39:25.000000 airbyte_source_shopify-2.0.5.dev202404081102/source_shopify/streams/base_streams.py
--rw-r--r--   0        0        0    11935 2024-04-08 10:39:25.000000 airbyte_source_shopify-2.0.5.dev202404081102/source_shopify/streams/streams.py
--rw-r--r--   0        0        0     4678 2024-04-08 10:39:25.000000 airbyte_source_shopify-2.0.5.dev202404081102/source_shopify/transform.py
--rw-r--r--   0        0        0    13056 2024-04-08 10:39:25.000000 airbyte_source_shopify-2.0.5.dev202404081102/source_shopify/utils.py
--rw-r--r--   0        0        0     5319 1970-01-01 00:00:00.000000 airbyte_source_shopify-2.0.5.dev202404081102/PKG-INFO
+-rw-r--r--   0        0        0     4519 2024-04-10 10:58:22.702597 airbyte_source_shopify-2.0.5.dev202404101100/README.md
+-rw-r--r--   0        0        0      812 2024-04-10 11:00:47.574229 airbyte_source_shopify-2.0.5.dev202404101100/pyproject.toml
+-rw-r--r--   0        0        0     1136 2024-04-10 10:58:22.702597 airbyte_source_shopify-2.0.5.dev202404101100/source_shopify/__init__.py
+-rw-r--r--   0        0        0     1538 2024-04-10 10:58:22.702597 airbyte_source_shopify-2.0.5.dev202404101100/source_shopify/auth.py
+-rw-r--r--   0        0        0     3797 2024-04-10 10:58:22.702597 airbyte_source_shopify-2.0.5.dev202404101100/source_shopify/config_migrations.py
+-rw-r--r--   0        0        0      398 2024-04-10 10:58:22.702597 airbyte_source_shopify-2.0.5.dev202404101100/source_shopify/run.py
+-rw-r--r--   0        0        0    16103 2024-04-10 10:58:22.706597 airbyte_source_shopify-2.0.5.dev202404101100/source_shopify/schemas/abandoned_checkouts.json
+-rw-r--r--   0        0        0     1272 2024-04-10 10:58:22.706597 airbyte_source_shopify-2.0.5.dev202404101100/source_shopify/schemas/articles.json
+-rw-r--r--   0        0        0     1009 2024-04-10 10:58:22.706597 airbyte_source_shopify-2.0.5.dev202404101100/source_shopify/schemas/balance_transactions.json
+-rw-r--r--   0        0        0     1109 2024-04-10 10:58:22.706597 airbyte_source_shopify-2.0.5.dev202404101100/source_shopify/schemas/blogs.json
+-rw-r--r--   0        0        0      928 2024-04-10 10:58:22.706597 airbyte_source_shopify-2.0.5.dev202404101100/source_shopify/schemas/collections.json
+-rw-r--r--   0        0        0      610 2024-04-10 10:58:22.706597 airbyte_source_shopify-2.0.5.dev202404101100/source_shopify/schemas/collects.json
+-rw-r--r--   0        0        0     1170 2024-04-10 10:58:22.706597 airbyte_source_shopify-2.0.5.dev202404101100/source_shopify/schemas/countries.json
+-rw-r--r--   0        0        0     1488 2024-04-10 10:58:22.706597 airbyte_source_shopify-2.0.5.dev202404101100/source_shopify/schemas/custom_collections.json
+-rw-r--r--   0        0        0     1217 2024-04-10 10:58:22.706597 airbyte_source_shopify-2.0.5.dev202404101100/source_shopify/schemas/customer_address.json
+-rw-r--r--   0        0        0      485 2024-04-10 10:58:22.706597 airbyte_source_shopify-2.0.5.dev202404101100/source_shopify/schemas/customer_saved_search.json
+-rw-r--r--   0        0        0     5313 2024-04-10 10:58:22.706597 airbyte_source_shopify-2.0.5.dev202404101100/source_shopify/schemas/customers.json
+-rw-r--r--   0        0        0      736 2024-04-10 10:58:22.706597 airbyte_source_shopify-2.0.5.dev202404101100/source_shopify/schemas/discount_codes.json
+-rw-r--r--   0        0        0      909 2024-04-10 10:58:22.706597 airbyte_source_shopify-2.0.5.dev202404101100/source_shopify/schemas/disputes.json
+-rw-r--r--   0        0        0    13381 2024-04-10 10:58:22.706597 airbyte_source_shopify-2.0.5.dev202404101100/source_shopify/schemas/draft_orders.json
+-rw-r--r--   0        0        0     5226 2024-04-10 10:58:22.706597 airbyte_source_shopify-2.0.5.dev202404101100/source_shopify/schemas/fulfillment_orders.json
+-rw-r--r--   0        0        0    14757 2024-04-10 10:58:22.706597 airbyte_source_shopify-2.0.5.dev202404101100/source_shopify/schemas/fulfillments.json
+-rw-r--r--   0        0        0     1027 2024-04-10 10:58:22.706597 airbyte_source_shopify-2.0.5.dev202404101100/source_shopify/schemas/inventory_items.json
+-rw-r--r--   0        0        0      536 2024-04-10 10:58:22.706597 airbyte_source_shopify-2.0.5.dev202404101100/source_shopify/schemas/inventory_levels.json
+-rw-r--r--   0        0        0     1329 2024-04-10 10:58:22.706597 airbyte_source_shopify-2.0.5.dev202404101100/source_shopify/schemas/locations.json
+-rw-r--r--   0        0        0      911 2024-04-10 10:58:22.706597 airbyte_source_shopify-2.0.5.dev202404101100/source_shopify/schemas/metafield_articles.json
+-rw-r--r--   0        0        0      911 2024-04-10 10:58:22.706597 airbyte_source_shopify-2.0.5.dev202404101100/source_shopify/schemas/metafield_blogs.json
+-rw-r--r--   0        0        0      911 2024-04-10 10:58:22.706597 airbyte_source_shopify-2.0.5.dev202404101100/source_shopify/schemas/metafield_collections.json
+-rw-r--r--   0        0        0      911 2024-04-10 10:58:22.706597 airbyte_source_shopify-2.0.5.dev202404101100/source_shopify/schemas/metafield_customers.json
+-rw-r--r--   0        0        0      911 2024-04-10 10:58:22.706597 airbyte_source_shopify-2.0.5.dev202404101100/source_shopify/schemas/metafield_draft_orders.json
+-rw-r--r--   0        0        0      911 2024-04-10 10:58:22.706597 airbyte_source_shopify-2.0.5.dev202404101100/source_shopify/schemas/metafield_locations.json
+-rw-r--r--   0        0        0      911 2024-04-10 10:58:22.706597 airbyte_source_shopify-2.0.5.dev202404101100/source_shopify/schemas/metafield_orders.json
+-rw-r--r--   0        0        0      911 2024-04-10 10:58:22.706597 airbyte_source_shopify-2.0.5.dev202404101100/source_shopify/schemas/metafield_pages.json
+-rw-r--r--   0        0        0      911 2024-04-10 10:58:22.706597 airbyte_source_shopify-2.0.5.dev202404101100/source_shopify/schemas/metafield_product_images.json
+-rw-r--r--   0        0        0      911 2024-04-10 10:58:22.706597 airbyte_source_shopify-2.0.5.dev202404101100/source_shopify/schemas/metafield_product_variants.json
+-rw-r--r--   0        0        0      911 2024-04-10 10:58:22.706597 airbyte_source_shopify-2.0.5.dev202404101100/source_shopify/schemas/metafield_products.json
+-rw-r--r--   0        0        0      911 2024-04-10 10:58:22.706597 airbyte_source_shopify-2.0.5.dev202404101100/source_shopify/schemas/metafield_shops.json
+-rw-r--r--   0        0        0      911 2024-04-10 10:58:22.706597 airbyte_source_shopify-2.0.5.dev202404101100/source_shopify/schemas/metafield_smart_collections.json
+-rw-r--r--   0        0        0    17520 2024-04-10 10:58:22.706597 airbyte_source_shopify-2.0.5.dev202404101100/source_shopify/schemas/order_refunds.json
+-rw-r--r--   0        0        0      728 2024-04-10 10:58:22.706597 airbyte_source_shopify-2.0.5.dev202404101100/source_shopify/schemas/order_risks.json
+-rw-r--r--   0        0        0    80187 2024-04-10 10:58:22.706597 airbyte_source_shopify-2.0.5.dev202404101100/source_shopify/schemas/orders.json
+-rw-r--r--   0        0        0     1104 2024-04-10 10:58:22.706597 airbyte_source_shopify-2.0.5.dev202404101100/source_shopify/schemas/pages.json
+-rw-r--r--   0        0        0     3891 2024-04-10 10:58:22.706597 airbyte_source_shopify-2.0.5.dev202404101100/source_shopify/schemas/price_rules.json
+-rw-r--r--   0        0        0      907 2024-04-10 10:58:22.706597 airbyte_source_shopify-2.0.5.dev202404101100/source_shopify/schemas/product_images.json
+-rw-r--r--   0        0        0     2336 2024-04-10 10:58:22.706597 airbyte_source_shopify-2.0.5.dev202404101100/source_shopify/schemas/product_variants.json
+-rw-r--r--   0        0        0     7060 2024-04-10 10:58:22.706597 airbyte_source_shopify-2.0.5.dev202404101100/source_shopify/schemas/products.json
+-rw-r--r--   0        0        0     1675 2024-04-10 10:58:22.706597 airbyte_source_shopify-2.0.5.dev202404101100/source_shopify/schemas/products_graph_ql.json
+-rw-r--r--   0        0        0     4059 2024-04-10 10:58:22.706597 airbyte_source_shopify-2.0.5.dev202404101100/source_shopify/schemas/shop.json
+-rw-r--r--   0        0        0      985 2024-04-10 10:58:22.706597 airbyte_source_shopify-2.0.5.dev202404101100/source_shopify/schemas/smart_collections.json
+-rw-r--r--   0        0        0      951 2024-04-10 10:58:22.706597 airbyte_source_shopify-2.0.5.dev202404101100/source_shopify/schemas/tender_transactions.json
+-rw-r--r--   0        0        0     3750 2024-04-10 10:58:22.706597 airbyte_source_shopify-2.0.5.dev202404101100/source_shopify/schemas/transactions.json
+-rw-r--r--   0        0        0     6367 2024-04-10 10:58:22.706597 airbyte_source_shopify-2.0.5.dev202404101100/source_shopify/scopes.py
+-rw-r--r--   0        0        0     1734 2024-04-10 10:58:22.706597 airbyte_source_shopify-2.0.5.dev202404101100/source_shopify/shopify_graphql/bulk/exceptions.py
+-rw-r--r--   0        0        0    15723 2024-04-10 10:58:22.706597 airbyte_source_shopify-2.0.5.dev202404101100/source_shopify/shopify_graphql/bulk/job.py
+-rw-r--r--   0        0        0    55609 2024-04-10 10:58:22.706597 airbyte_source_shopify-2.0.5.dev202404101100/source_shopify/shopify_graphql/bulk/query.py
+-rw-r--r--   0        0        0     6517 2024-04-10 10:58:22.706597 airbyte_source_shopify-2.0.5.dev202404101100/source_shopify/shopify_graphql/bulk/record.py
+-rw-r--r--   0        0        0     3629 2024-04-10 10:58:22.706597 airbyte_source_shopify-2.0.5.dev202404101100/source_shopify/shopify_graphql/bulk/tools.py
+-rw-r--r--   0        0        0     1969 2024-04-10 10:58:22.706597 airbyte_source_shopify-2.0.5.dev202404101100/source_shopify/shopify_graphql/graphql.py
+-rw-r--r--   0        0        0  1354903 2024-04-10 10:58:22.714598 airbyte_source_shopify-2.0.5.dev202404101100/source_shopify/shopify_graphql/schema.py
+-rw-r--r--   0        0        0     8540 2024-04-10 10:58:22.714598 airbyte_source_shopify-2.0.5.dev202404101100/source_shopify/source.py
+-rw-r--r--   0        0        0     5118 2024-04-10 10:58:22.714598 airbyte_source_shopify-2.0.5.dev202404101100/source_shopify/spec.json
+-rw-r--r--   0        0        0    35528 2024-04-10 10:58:22.714598 airbyte_source_shopify-2.0.5.dev202404101100/source_shopify/streams/base_streams.py
+-rw-r--r--   0        0        0    11935 2024-04-10 10:58:22.714598 airbyte_source_shopify-2.0.5.dev202404101100/source_shopify/streams/streams.py
+-rw-r--r--   0        0        0     4678 2024-04-10 10:58:22.714598 airbyte_source_shopify-2.0.5.dev202404101100/source_shopify/transform.py
+-rw-r--r--   0        0        0    13056 2024-04-10 10:58:22.714598 airbyte_source_shopify-2.0.5.dev202404101100/source_shopify/utils.py
+-rw-r--r--   0        0        0     5319 1970-01-01 00:00:00.000000 airbyte_source_shopify-2.0.5.dev202404101100/PKG-INFO
```

### Comparing `airbyte_source_shopify-2.0.5.dev202404081102/README.md` & `airbyte_source_shopify-2.0.5.dev202404101100/README.md`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404081102/pyproject.toml` & `airbyte_source_shopify-2.0.5.dev202404101100/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "2.0.5.dev202404081102"
+version = "2.0.5.dev202404101100"
 name = "airbyte-source-shopify"
 description = "Source CDK implementation for Shopify."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "ELv2"
 readme = "README.md"
```

### Comparing `airbyte_source_shopify-2.0.5.dev202404081102/source_shopify/__init__.py` & `airbyte_source_shopify-2.0.5.dev202404101100/source_shopify/__init__.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404081102/source_shopify/auth.py` & `airbyte_source_shopify-2.0.5.dev202404101100/source_shopify/auth.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404081102/source_shopify/config_migrations.py` & `airbyte_source_shopify-2.0.5.dev202404101100/source_shopify/config_migrations.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404081102/source_shopify/schemas/abandoned_checkouts.json` & `airbyte_source_shopify-2.0.5.dev202404101100/source_shopify/schemas/abandoned_checkouts.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404081102/source_shopify/schemas/articles.json` & `airbyte_source_shopify-2.0.5.dev202404101100/source_shopify/schemas/articles.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404081102/source_shopify/schemas/balance_transactions.json` & `airbyte_source_shopify-2.0.5.dev202404101100/source_shopify/schemas/balance_transactions.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404081102/source_shopify/schemas/blogs.json` & `airbyte_source_shopify-2.0.5.dev202404101100/source_shopify/schemas/blogs.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404081102/source_shopify/schemas/collections.json` & `airbyte_source_shopify-2.0.5.dev202404101100/source_shopify/schemas/collections.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404081102/source_shopify/schemas/collects.json` & `airbyte_source_shopify-2.0.5.dev202404101100/source_shopify/schemas/collects.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404081102/source_shopify/schemas/countries.json` & `airbyte_source_shopify-2.0.5.dev202404101100/source_shopify/schemas/countries.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404081102/source_shopify/schemas/custom_collections.json` & `airbyte_source_shopify-2.0.5.dev202404101100/source_shopify/schemas/custom_collections.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404081102/source_shopify/schemas/customer_address.json` & `airbyte_source_shopify-2.0.5.dev202404101100/source_shopify/schemas/customer_address.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404081102/source_shopify/schemas/customers.json` & `airbyte_source_shopify-2.0.5.dev202404101100/source_shopify/schemas/customers.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404081102/source_shopify/schemas/discount_codes.json` & `airbyte_source_shopify-2.0.5.dev202404101100/source_shopify/schemas/discount_codes.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404081102/source_shopify/schemas/disputes.json` & `airbyte_source_shopify-2.0.5.dev202404101100/source_shopify/schemas/disputes.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404081102/source_shopify/schemas/draft_orders.json` & `airbyte_source_shopify-2.0.5.dev202404101100/source_shopify/schemas/draft_orders.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404081102/source_shopify/schemas/fulfillment_orders.json` & `airbyte_source_shopify-2.0.5.dev202404101100/source_shopify/schemas/fulfillment_orders.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404081102/source_shopify/schemas/fulfillments.json` & `airbyte_source_shopify-2.0.5.dev202404101100/source_shopify/schemas/fulfillments.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404081102/source_shopify/schemas/inventory_items.json` & `airbyte_source_shopify-2.0.5.dev202404101100/source_shopify/schemas/inventory_items.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404081102/source_shopify/schemas/inventory_levels.json` & `airbyte_source_shopify-2.0.5.dev202404101100/source_shopify/schemas/inventory_levels.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404081102/source_shopify/schemas/locations.json` & `airbyte_source_shopify-2.0.5.dev202404101100/source_shopify/schemas/locations.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404081102/source_shopify/schemas/metafield_articles.json` & `airbyte_source_shopify-2.0.5.dev202404101100/source_shopify/schemas/metafield_articles.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404081102/source_shopify/schemas/metafield_blogs.json` & `airbyte_source_shopify-2.0.5.dev202404101100/source_shopify/schemas/metafield_blogs.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404081102/source_shopify/schemas/metafield_collections.json` & `airbyte_source_shopify-2.0.5.dev202404101100/source_shopify/schemas/metafield_collections.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404081102/source_shopify/schemas/metafield_customers.json` & `airbyte_source_shopify-2.0.5.dev202404101100/source_shopify/schemas/metafield_customers.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404081102/source_shopify/schemas/metafield_draft_orders.json` & `airbyte_source_shopify-2.0.5.dev202404101100/source_shopify/schemas/metafield_draft_orders.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404081102/source_shopify/schemas/metafield_locations.json` & `airbyte_source_shopify-2.0.5.dev202404101100/source_shopify/schemas/metafield_locations.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404081102/source_shopify/schemas/metafield_orders.json` & `airbyte_source_shopify-2.0.5.dev202404101100/source_shopify/schemas/metafield_orders.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404081102/source_shopify/schemas/metafield_pages.json` & `airbyte_source_shopify-2.0.5.dev202404101100/source_shopify/schemas/metafield_pages.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404081102/source_shopify/schemas/metafield_product_images.json` & `airbyte_source_shopify-2.0.5.dev202404101100/source_shopify/schemas/metafield_product_images.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404081102/source_shopify/schemas/metafield_product_variants.json` & `airbyte_source_shopify-2.0.5.dev202404101100/source_shopify/schemas/metafield_product_variants.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404081102/source_shopify/schemas/metafield_products.json` & `airbyte_source_shopify-2.0.5.dev202404101100/source_shopify/schemas/metafield_products.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404081102/source_shopify/schemas/metafield_shops.json` & `airbyte_source_shopify-2.0.5.dev202404101100/source_shopify/schemas/metafield_shops.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404081102/source_shopify/schemas/metafield_smart_collections.json` & `airbyte_source_shopify-2.0.5.dev202404101100/source_shopify/schemas/metafield_smart_collections.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404081102/source_shopify/schemas/order_refunds.json` & `airbyte_source_shopify-2.0.5.dev202404101100/source_shopify/schemas/order_refunds.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404081102/source_shopify/schemas/order_risks.json` & `airbyte_source_shopify-2.0.5.dev202404101100/source_shopify/schemas/order_risks.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404081102/source_shopify/schemas/orders.json` & `airbyte_source_shopify-2.0.5.dev202404101100/source_shopify/schemas/orders.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404081102/source_shopify/schemas/pages.json` & `airbyte_source_shopify-2.0.5.dev202404101100/source_shopify/schemas/pages.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404081102/source_shopify/schemas/price_rules.json` & `airbyte_source_shopify-2.0.5.dev202404101100/source_shopify/schemas/price_rules.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404081102/source_shopify/schemas/product_images.json` & `airbyte_source_shopify-2.0.5.dev202404101100/source_shopify/schemas/product_images.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404081102/source_shopify/schemas/product_variants.json` & `airbyte_source_shopify-2.0.5.dev202404101100/source_shopify/schemas/product_variants.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404081102/source_shopify/schemas/products.json` & `airbyte_source_shopify-2.0.5.dev202404101100/source_shopify/schemas/products.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404081102/source_shopify/schemas/products_graph_ql.json` & `airbyte_source_shopify-2.0.5.dev202404101100/source_shopify/schemas/products_graph_ql.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404081102/source_shopify/schemas/shop.json` & `airbyte_source_shopify-2.0.5.dev202404101100/source_shopify/schemas/shop.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404081102/source_shopify/schemas/smart_collections.json` & `airbyte_source_shopify-2.0.5.dev202404101100/source_shopify/schemas/smart_collections.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404081102/source_shopify/schemas/tender_transactions.json` & `airbyte_source_shopify-2.0.5.dev202404101100/source_shopify/schemas/tender_transactions.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404081102/source_shopify/schemas/transactions.json` & `airbyte_source_shopify-2.0.5.dev202404101100/source_shopify/schemas/transactions.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404081102/source_shopify/scopes.py` & `airbyte_source_shopify-2.0.5.dev202404101100/source_shopify/scopes.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404081102/source_shopify/shopify_graphql/bulk/exceptions.py` & `airbyte_source_shopify-2.0.5.dev202404101100/source_shopify/shopify_graphql/bulk/exceptions.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404081102/source_shopify/shopify_graphql/bulk/job.py` & `airbyte_source_shopify-2.0.5.dev202404101100/source_shopify/shopify_graphql/bulk/job.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     ACCESS_DENIED = "ACCESS_DENIED"
 
 
 @dataclass
 class ShopifyBulkManager:
     session: requests.Session
     base_url: str
+    stream_name: str
 
     # default logger
     logger: Final[AirbyteLogger] = logging.getLogger("airbyte")
 
     # 10Mb chunk size to save the file
     retrieve_chunk_size: Final[int] = 1024 * 1024 * 10
     # time between job status checks
@@ -143,15 +144,15 @@
         if self.log_running_job_msg_count < self.log_running_job_msg_frequency:
             self.log_running_job_msg_count += 1
         else:
             self.log_state()
             self.log_running_job_msg_count = 0
 
     def log_state(self) -> None:
-        self.logger.info(f"The BULK Job: `{self.job_id}` is {self.job_state}.")
+        self.logger.info(f"Stream: `{self.stream_name}`, the BULK Job: `{self.job_id}` is {self.job_state}.")
 
     def job_get_state_args(self) -> Mapping[str, Any]:
         return {
             "method": "POST",
             "url": self.base_url,
             "data": ShopifyBulkTemplates.status(self.job_id),
             "headers": {"Content-Type": "application/graphql"},
@@ -219,15 +220,16 @@
                 f"Couldn't check the `response` for `errors`, status: {response.status_code}, response: `{response.text}`. Trace: {repr(e)}."
             )
 
     def job_track_running(self) -> Union[AirbyteTracedException, requests.Response]:
         # format Job state check args
         status_args = self.job_get_state_args()
         # re-use of `self._session(*, **)` to make BULK Job status checks
-        response = self.session.request(**status_args)
+        with self.session as track_running_job:
+            response = track_running_job.request(**status_args)
         # errors check
         errors = self.job_check_for_errors(response)
         if not errors:
             self.job_update_state(response)
             self.job_state_to_fn_map.get(self.job_state)(response=response)
             return response
         else:
@@ -263,34 +265,31 @@
         self.concurrent_attempt = 0
         return False
 
     def has_reached_max_concurrency_attempt(self) -> bool:
         return self.concurrent_attempt == self.concurrent_max_retry
 
     def job_retry_request(self, request: requests.PreparedRequest) -> Optional[requests.Response]:
-        # retry current `request`
-        return self.session.send(request)
+        with self.session.send(request) as retried_request:
+            return retried_request
 
     def job_retry_concurrent(self, request: requests.PreparedRequest) -> Optional[requests.Response]:
-        # increment attempt
         self.concurrent_attempt += 1
-        # try to execute previous request, it's handy because we can retry / each slice yielded
         self.logger.warning(
-            f"The BULK concurrency limit has reached. Waiting {self.concurrent_interval_sec} sec before retry, atttempt: {self.concurrent_attempt}.",
+            f"Stream: `{self.stream_name}`, the BULK concurrency limit has reached. Waiting {self.concurrent_interval_sec} sec before retry, atttempt: {self.concurrent_attempt}.",
         )
         sleep(self.concurrent_interval_sec)
-        # retry current `request`
         return self.job_healthcheck(self.job_retry_request(request))
 
     def job_get_id(self, response: requests.Response) -> Optional[str]:
         response_data = response.json()
         bulk_response = response_data.get("data", {}).get("bulkOperationRunQuery", {}).get("bulkOperation", {})
         if bulk_response and bulk_response.get("status") == ShopifyBulkStatus.CREATED.value:
             job_id = bulk_response.get("id")
-            self.logger.info(f"The BULK Job: `{job_id}` is {ShopifyBulkStatus.CREATED.value}")
+            self.logger.info(f"Stream: `{self.stream_name}`, the BULK Job: `{job_id}` is {ShopifyBulkStatus.CREATED.value}")
             return job_id
         else:
             return None
 
     def job_retry_on_concurrency(self, request: requests.PreparedRequest) -> Union[AirbyteTracedException, Optional[requests.Response]]:
         if self.has_reached_max_concurrency_attempt():
             # indicate we're out of attempts to retry with job creation
@@ -311,14 +310,15 @@
             if not self.has_running_concurrent_job(errors):
                 return response if not errors else None
             else:
                 return self.job_retry_on_concurrency(request)
         except (ShopifyBulkExceptions.BulkJobBadResponse, ShopifyBulkExceptions.BulkJobUnknownError) as err:
             # sometimes we face with `HTTP-500 Internal Server Error`
             # we should retry such at least once
+            self.logger.info(f"Stream: `{self.stream_name}`, retrying Bad Request: {request.body}, error: {repr(err)}.")
             return self.job_retry_request(request)
 
     @limiter.balance_rate_limit(api_type=ApiTypeEnum.graphql.value)
     def job_check(self, created_job_response: requests.Response) -> Optional[str]:
         """
         This method checks the status for the BULK Job created, using it's `ID`.
         The time spent for the Job execution is tracked to understand the effort.
@@ -334,12 +334,12 @@
             ShopifyBulkExceptions.BulkJobTimout,
             ShopifyBulkExceptions.BulkJobAccessDenied,
             ShopifyBulkExceptions.BulkJobUnknownError,
         ) as bulk_job_error:
             raise bulk_job_error
         finally:
             job_current_elapsed_time = round((time() - job_started), 3)
-            self.logger.info(f"The BULK Job: `{self.job_id}` time elapsed: {job_current_elapsed_time} sec.")
+            self.logger.info(f"Stream: `{self.stream_name}`, the BULK Job: `{self.job_id}` time elapsed: {job_current_elapsed_time} sec.")
             # check whether or not we should expand or reduce the size of the slice
             self.__adjust_job_size(job_current_elapsed_time)
             # reset the state for COMPLETED job
             self.__reset_state()
```

### Comparing `airbyte_source_shopify-2.0.5.dev202404081102/source_shopify/shopify_graphql/bulk/query.py` & `airbyte_source_shopify-2.0.5.dev202404101100/source_shopify/shopify_graphql/bulk/query.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404081102/source_shopify/shopify_graphql/bulk/record.py` & `airbyte_source_shopify-2.0.5.dev202404101100/source_shopify/shopify_graphql/bulk/record.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404081102/source_shopify/shopify_graphql/bulk/tools.py` & `airbyte_source_shopify-2.0.5.dev202404101100/source_shopify/shopify_graphql/bulk/tools.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404081102/source_shopify/shopify_graphql/graphql.py` & `airbyte_source_shopify-2.0.5.dev202404101100/source_shopify/shopify_graphql/graphql.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404081102/source_shopify/shopify_graphql/schema.py` & `airbyte_source_shopify-2.0.5.dev202404101100/source_shopify/shopify_graphql/schema.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404081102/source_shopify/source.py` & `airbyte_source_shopify-2.0.5.dev202404101100/source_shopify/source.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404081102/source_shopify/spec.json` & `airbyte_source_shopify-2.0.5.dev202404101100/source_shopify/spec.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404081102/source_shopify/streams/base_streams.py` & `airbyte_source_shopify-2.0.5.dev202404101100/source_shopify/streams/base_streams.py`

 * *Files 0% similar despite different names*

```diff
@@ -593,15 +593,19 @@
     parent_stream_class: Optional[Union[ShopifyStream, IncrementalShopifyStream]] = None
 
     def __init__(self, config: Dict) -> None:
         super().__init__(config)
         # init BULK Query instance, pass `shop_id` from config
         self.query = self.bulk_query(shop_id=config.get("shop_id"))
         # define BULK Manager instance
-        self.job_manager: ShopifyBulkManager = ShopifyBulkManager(self._session, f"{self.url_base}/{self.path()}")
+        self.job_manager: ShopifyBulkManager = ShopifyBulkManager(
+            session=self._session,
+            base_url=f"{self.url_base}/{self.path()}",
+            stream_name=self.name,
+        )
         # overide the default job slice size, if provided (it's auto-adjusted, later on)
         self.bulk_window_in_days = config.get("bulk_window_in_days")
         if self.bulk_window_in_days:
             self.job_manager.job_size = self.bulk_window_in_days
         # define Record Producer instance
         self.record_producer: ShopifyBulkRecord = ShopifyBulkRecord(self.query)
```

### Comparing `airbyte_source_shopify-2.0.5.dev202404081102/source_shopify/streams/streams.py` & `airbyte_source_shopify-2.0.5.dev202404101100/source_shopify/streams/streams.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404081102/source_shopify/transform.py` & `airbyte_source_shopify-2.0.5.dev202404101100/source_shopify/transform.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404081102/source_shopify/utils.py` & `airbyte_source_shopify-2.0.5.dev202404101100/source_shopify/utils.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_shopify-2.0.5.dev202404081102/PKG-INFO` & `airbyte_source_shopify-2.0.5.dev202404101100/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airbyte-source-shopify
-Version: 2.0.5.dev202404081102
+Version: 2.0.5.dev202404101100
 Summary: Source CDK implementation for Shopify.
 Home-page: https://airbyte.com
 License: ELv2
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<3.12
 Classifier: License :: Other/Proprietary License
```

