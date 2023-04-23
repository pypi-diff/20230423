# Comparing `tmp/python-amazon-sp-api-0.9.2.tar.gz` & `tmp/python-amazon-sp-api-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-amazon-sp-api-0.9.2.tar", last modified: Tue Dec 14 18:16:01 2021, max compression
+gzip compressed data, was "python-amazon-sp-api-0.9.4.tar", last modified: Sat Dec 18 12:09:40 2021, max compression
```

## Comparing `python-amazon-sp-api-0.9.2.tar` & `python-amazon-sp-api-0.9.4.tar`

### file list

```diff
@@ -1,189 +1,189 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 18:16:01.302678 python-amazon-sp-api-0.9.2/
--rw-r--r--   0 runner    (1001) docker     (121)     1071 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     3436 2021-12-14 18:16:01.302678 python-amazon-sp-api-0.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3105 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 18:16:01.278678 python-amazon-sp-api-0.9.2/python_amazon_sp_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3436 2021-12-14 18:16:01.000000 python-amazon-sp-api-0.9.2/python_amazon_sp_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4949 2021-12-14 18:16:01.000000 python-amazon-sp-api-0.9.2/python_amazon_sp_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-14 18:16:01.000000 python-amazon-sp-api-0.9.2/python_amazon_sp_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       91 2021-12-14 18:16:01.000000 python-amazon-sp-api-0.9.2/python_amazon_sp_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2021-12-14 18:16:01.000000 python-amazon-sp-api-0.9.2/python_amazon_sp_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      161 2021-12-14 18:16:01.302678 python-amazon-sp-api-0.9.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2595 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 18:16:01.278678 python-amazon-sp-api-0.9.2/sp_api/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/sp_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 18:16:01.278678 python-amazon-sp-api-0.9.2/sp_api/api/
--rw-r--r--   0 runner    (1001) docker     (121)     3726 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/sp_api/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 18:16:01.278678 python-amazon-sp-api-0.9.2/sp_api/api/aplus_content/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/sp_api/api/aplus_content/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    18034 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/sp_api/api/aplus_content/aplus_content.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 18:16:01.278678 python-amazon-sp-api-0.9.2/sp_api/api/authorization/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/sp_api/api/authorization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2804 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/sp_api/api/authorization/authorization.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 18:16:01.278678 python-amazon-sp-api-0.9.2/sp_api/api/catalog/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/sp_api/api/catalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3957 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/sp_api/api/catalog/catalog.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 18:16:01.278678 python-amazon-sp-api-0.9.2/sp_api/api/catalog_items/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/sp_api/api/catalog_items/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4048 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/sp_api/api/catalog_items/catalog_items.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 18:16:01.282678 python-amazon-sp-api-0.9.2/sp_api/api/fba_inbound_eligibility/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/sp_api/api/fba_inbound_eligibility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2183 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/sp_api/api/fba_inbound_eligibility/fba_inbound_eligibility.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 18:16:01.282678 python-amazon-sp-api-0.9.2/sp_api/api/fba_small_and_light/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/sp_api/api/fba_small_and_light/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8220 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/sp_api/api/fba_small_and_light/fba_small_and_light.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 18:16:01.282678 python-amazon-sp-api-0.9.2/sp_api/api/feeds/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/sp_api/api/feeds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7084 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/sp_api/api/feeds/feeds.py
--rw-r--r--   0 runner    (1001) docker     (121)     7975 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/sp_api/api/feeds/feeds_v2.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 18:16:01.282678 python-amazon-sp-api-0.9.2/sp_api/api/finances/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/sp_api/api/finances/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1856 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/sp_api/api/finances/finances.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 18:16:01.282678 python-amazon-sp-api-0.9.2/sp_api/api/fulfillment_inbound/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/sp_api/api/fulfillment_inbound/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12329 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/sp_api/api/fulfillment_inbound/fulfillment_inbound.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 18:16:01.282678 python-amazon-sp-api-0.9.2/sp_api/api/fulfillment_outbound/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/sp_api/api/fulfillment_outbound/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    28743 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/sp_api/api/fulfillment_outbound/fulfillment_outbound.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 18:16:01.282678 python-amazon-sp-api-0.9.2/sp_api/api/inventories/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/sp_api/api/inventories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4004 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/sp_api/api/inventories/inventories.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 18:16:01.282678 python-amazon-sp-api-0.9.2/sp_api/api/listings_items/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/sp_api/api/listings_items/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8497 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/sp_api/api/listings_items/listings_items.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 18:16:01.282678 python-amazon-sp-api-0.9.2/sp_api/api/listings_restrictions/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/sp_api/api/listings_restrictions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2430 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/sp_api/api/listings_restrictions/listings_restrictions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 18:16:01.282678 python-amazon-sp-api-0.9.2/sp_api/api/merchant_fulfillment/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/sp_api/api/merchant_fulfillment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    15301 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/sp_api/api/merchant_fulfillment/merchant_fulfillment.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 18:16:01.286678 python-amazon-sp-api-0.9.2/sp_api/api/messaging/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/sp_api/api/messaging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    16124 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/sp_api/api/messaging/messaging.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 18:16:01.286678 python-amazon-sp-api-0.9.2/sp_api/api/notifications/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/sp_api/api/notifications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10798 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/sp_api/api/notifications/notifications.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 18:16:01.286678 python-amazon-sp-api-0.9.2/sp_api/api/orders/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/sp_api/api/orders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9424 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/sp_api/api/orders/orders.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 18:16:01.286678 python-amazon-sp-api-0.9.2/sp_api/api/product_fees/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/sp_api/api/product_fees/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4545 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/sp_api/api/product_fees/product_fees.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 18:16:01.286678 python-amazon-sp-api-0.9.2/sp_api/api/product_type_definitions/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/sp_api/api/product_type_definitions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4471 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/sp_api/api/product_type_definitions/product_type_definitions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 18:16:01.286678 python-amazon-sp-api-0.9.2/sp_api/api/products/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/sp_api/api/products/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7402 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/sp_api/api/products/products.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 18:16:01.286678 python-amazon-sp-api-0.9.2/sp_api/api/reports/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/sp_api/api/reports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13954 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/sp_api/api/reports/reports.py
--rw-r--r--   0 runner    (1001) docker     (121)    15883 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/sp_api/api/reports/reports_v2.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 18:16:01.286678 python-amazon-sp-api-0.9.2/sp_api/api/sales/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/sp_api/api/sales/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5627 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/sp_api/api/sales/sales.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 18:16:01.286678 python-amazon-sp-api-0.9.2/sp_api/api/sellers/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/sp_api/api/sellers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      305 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/sp_api/api/sellers/sellers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 18:16:01.286678 python-amazon-sp-api-0.9.2/sp_api/api/services/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/sp_api/api/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9133 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/sp_api/api/services/services.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 18:16:01.290678 python-amazon-sp-api-0.9.2/sp_api/api/shipping/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/sp_api/api/shipping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    14506 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/sp_api/api/shipping/shipping.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 18:16:01.290678 python-amazon-sp-api-0.9.2/sp_api/api/solicitations/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/sp_api/api/solicitations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3854 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/sp_api/api/solicitations/solicitations.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 18:16:01.290678 python-amazon-sp-api-0.9.2/sp_api/api/tokens/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/sp_api/api/tokens/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3380 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/sp_api/api/tokens/tokens.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 18:16:01.290678 python-amazon-sp-api-0.9.2/sp_api/api/upload/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/sp_api/api/upload/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      596 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/sp_api/api/upload/upload.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 18:16:01.290678 python-amazon-sp-api-0.9.2/sp_api/api/vendor_direct_fulfillment_inventory/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/sp_api/api/vendor_direct_fulfillment_inventory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2286 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/sp_api/api/vendor_direct_fulfillment_inventory/vendor_direct_fulfillment_inventory.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 18:16:01.290678 python-amazon-sp-api-0.9.2/sp_api/api/vendor_direct_fulfillment_orders/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/sp_api/api/vendor_direct_fulfillment_orders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9463 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/sp_api/api/vendor_direct_fulfillment_orders/vendor_direct_fulfillment_orders.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 18:16:01.290678 python-amazon-sp-api-0.9.2/sp_api/api/vendor_direct_fulfillment_payments/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/sp_api/api/vendor_direct_fulfillment_payments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10146 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/sp_api/api/vendor_direct_fulfillment_payments/vendor_direct_fulfillment_payments.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 18:16:01.290678 python-amazon-sp-api-0.9.2/sp_api/api/vendor_direct_fulfillment_shipping/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/sp_api/api/vendor_direct_fulfillment_shipping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    28770 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/sp_api/api/vendor_direct_fulfillment_shipping/vendor_direct_fulfillment_shipping.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 18:16:01.290678 python-amazon-sp-api-0.9.2/sp_api/api/vendor_direct_fulfillment_transactions/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/sp_api/api/vendor_direct_fulfillment_transactions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1701 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/sp_api/api/vendor_direct_fulfillment_transactions/vendor_direct_fulfillment_transactions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 18:16:01.290678 python-amazon-sp-api-0.9.2/sp_api/api/vendor_invoices/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/sp_api/api/vendor_invoices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11192 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/sp_api/api/vendor_invoices/vendor_invoices.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 18:16:01.290678 python-amazon-sp-api-0.9.2/sp_api/api/vendor_orders/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/sp_api/api/vendor_orders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13391 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/sp_api/api/vendor_orders/vendor_orders.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 18:16:01.294678 python-amazon-sp-api-0.9.2/sp_api/api/vendor_shipments/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/sp_api/api/vendor_shipments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11627 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/sp_api/api/vendor_shipments/vendor_shipments.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 18:16:01.294678 python-amazon-sp-api-0.9.2/sp_api/api/vendor_transaction_status/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/sp_api/api/vendor_transaction_status/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1679 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/sp_api/api/vendor_transaction_status/vendor_transaction_status.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 18:16:01.294678 python-amazon-sp-api-0.9.2/sp_api/auth/
--rw-r--r--   0 runner    (1001) docker     (121)      229 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/sp_api/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6136 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/sp_api/auth/access_token_client.py
--rw-r--r--   0 runner    (1001) docker     (121)      272 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/sp_api/auth/access_token_response.py
--rw-r--r--   0 runner    (1001) docker     (121)      262 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/sp_api/auth/credentials.py
--rw-r--r--   0 runner    (1001) docker     (121)      424 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/sp_api/auth/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 18:16:01.298678 python-amazon-sp-api-0.9.2/sp_api/base/
--rw-r--r--   0 runner    (1001) docker     (121)      960 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/sp_api/base/ApiResponse.py
--rw-r--r--   0 runner    (1001) docker     (121)       90 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/sp_api/base/InventoryEnums.py
--rw-r--r--   0 runner    (1001) docker     (121)     1835 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/sp_api/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3722 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/sp_api/base/aws_sig_v4.py
--rw-r--r--   0 runner    (1001) docker     (121)      405 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/sp_api/base/base_client.py
--rw-r--r--   0 runner    (1001) docker     (121)     5783 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/sp_api/base/client.py
--rw-r--r--   0 runner    (1001) docker     (121)     3481 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/sp_api/base/config.py
--rw-r--r--   0 runner    (1001) docker     (121)    10481 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/sp_api/base/credential_provider.py
--rw-r--r--   0 runner    (1001) docker     (121)      656 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/sp_api/base/deprecated.py
--rw-r--r--   0 runner    (1001) docker     (121)     2969 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/sp_api/base/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)       93 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/sp_api/base/fulfillment_channel.py
--rw-r--r--   0 runner    (1001) docker     (121)     2713 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/sp_api/base/helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)     2926 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/sp_api/base/marketplaces.py
--rw-r--r--   0 runner    (1001) docker     (121)      613 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/sp_api/base/notifications.py
--rw-r--r--   0 runner    (1001) docker     (121)      183 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/sp_api/base/processing_status.py
--rw-r--r--   0 runner    (1001) docker     (121)     7651 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/sp_api/base/reportTypes.py
--rw-r--r--   0 runner    (1001) docker     (121)     2714 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/sp_api/base/report_headers.py
--rw-r--r--   0 runner    (1001) docker     (121)      179 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/sp_api/base/report_status.py
--rw-r--r--   0 runner    (1001) docker     (121)      379 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/sp_api/base/sales_enum.py
--rw-r--r--   0 runner    (1001) docker     (121)      433 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/sp_api/base/schedules.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 18:16:01.298678 python-amazon-sp-api-0.9.2/sp_api/util/
--rw-r--r--   0 runner    (1001) docker     (121)      229 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/sp_api/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2151 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/sp_api/util/key_maker.py
--rw-r--r--   0 runner    (1001) docker     (121)     1310 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/sp_api/util/load_all_pages.py
--rw-r--r--   0 runner    (1001) docker     (121)     2411 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/sp_api/util/retry.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 18:16:01.298678 python-amazon-sp-api-0.9.2/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 18:16:01.298678 python-amazon-sp-api-0.9.2/tests/api/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/tests/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 18:16:01.298678 python-amazon-sp-api-0.9.2/tests/api/finances/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/tests/api/finances/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      584 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/tests/api/finances/test_finances.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 18:16:01.298678 python-amazon-sp-api-0.9.2/tests/api/notifications/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/tests/api/notifications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1293 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/tests/api/notifications/test_notifications.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 18:16:01.302678 python-amazon-sp-api-0.9.2/tests/api/orders/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/tests/api/orders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1509 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/tests/api/orders/test_orders.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 18:16:01.302678 python-amazon-sp-api-0.9.2/tests/api/product_fees/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/tests/api/product_fees/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1610 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/tests/api/product_fees/product_fees.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 18:16:01.302678 python-amazon-sp-api-0.9.2/tests/api/reports/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/tests/api/reports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3600 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/tests/api/reports/test_reports.py
--rw-r--r--   0 runner    (1001) docker     (121)     3623 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/tests/api/reports/test_reports_v2.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 18:16:01.302678 python-amazon-sp-api-0.9.2/tests/api/sellers/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/tests/api/sellers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/tests/api/sellers/test_sellers.py
--rw-r--r--   0 runner    (1001) docker     (121)      185 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/tests/base.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-14 18:16:01.302678 python-amazon-sp-api-0.9.2/tests/client/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/tests/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/tests/client/auth.py
--rw-r--r--   0 runner    (1001) docker     (121)     1373 2021-12-14 18:15:46.000000 python-amazon-sp-api-0.9.2/tests/test_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-18 12:09:40.585704 python-amazon-sp-api-0.9.4/
+-rw-r--r--   0 runner    (1001) docker     (121)     1071 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     3436 2021-12-18 12:09:40.585704 python-amazon-sp-api-0.9.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3105 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-18 12:09:40.573704 python-amazon-sp-api-0.9.4/python_amazon_sp_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3436 2021-12-18 12:09:40.000000 python-amazon-sp-api-0.9.4/python_amazon_sp_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     4949 2021-12-18 12:09:40.000000 python-amazon-sp-api-0.9.4/python_amazon_sp_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-18 12:09:40.000000 python-amazon-sp-api-0.9.4/python_amazon_sp_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       91 2021-12-18 12:09:40.000000 python-amazon-sp-api-0.9.4/python_amazon_sp_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       13 2021-12-18 12:09:40.000000 python-amazon-sp-api-0.9.4/python_amazon_sp_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      161 2021-12-18 12:09:40.585704 python-amazon-sp-api-0.9.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2595 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-18 12:09:40.573704 python-amazon-sp-api-0.9.4/sp_api/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/sp_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-18 12:09:40.573704 python-amazon-sp-api-0.9.4/sp_api/api/
+-rw-r--r--   0 runner    (1001) docker     (121)     3726 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/sp_api/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-18 12:09:40.573704 python-amazon-sp-api-0.9.4/sp_api/api/aplus_content/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/sp_api/api/aplus_content/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18034 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/sp_api/api/aplus_content/aplus_content.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-18 12:09:40.573704 python-amazon-sp-api-0.9.4/sp_api/api/authorization/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/sp_api/api/authorization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2804 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/sp_api/api/authorization/authorization.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-18 12:09:40.577704 python-amazon-sp-api-0.9.4/sp_api/api/catalog/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/sp_api/api/catalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3957 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/sp_api/api/catalog/catalog.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-18 12:09:40.577704 python-amazon-sp-api-0.9.4/sp_api/api/catalog_items/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/sp_api/api/catalog_items/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4048 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/sp_api/api/catalog_items/catalog_items.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-18 12:09:40.577704 python-amazon-sp-api-0.9.4/sp_api/api/fba_inbound_eligibility/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/sp_api/api/fba_inbound_eligibility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2183 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/sp_api/api/fba_inbound_eligibility/fba_inbound_eligibility.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-18 12:09:40.577704 python-amazon-sp-api-0.9.4/sp_api/api/fba_small_and_light/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/sp_api/api/fba_small_and_light/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8220 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/sp_api/api/fba_small_and_light/fba_small_and_light.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-18 12:09:40.577704 python-amazon-sp-api-0.9.4/sp_api/api/feeds/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/sp_api/api/feeds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7084 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/sp_api/api/feeds/feeds.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8447 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/sp_api/api/feeds/feeds_v2.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-18 12:09:40.577704 python-amazon-sp-api-0.9.4/sp_api/api/finances/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/sp_api/api/finances/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1856 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/sp_api/api/finances/finances.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-18 12:09:40.577704 python-amazon-sp-api-0.9.4/sp_api/api/fulfillment_inbound/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/sp_api/api/fulfillment_inbound/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12641 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/sp_api/api/fulfillment_inbound/fulfillment_inbound.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-18 12:09:40.577704 python-amazon-sp-api-0.9.4/sp_api/api/fulfillment_outbound/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/sp_api/api/fulfillment_outbound/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    28743 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/sp_api/api/fulfillment_outbound/fulfillment_outbound.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-18 12:09:40.577704 python-amazon-sp-api-0.9.4/sp_api/api/inventories/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/sp_api/api/inventories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4004 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/sp_api/api/inventories/inventories.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-18 12:09:40.577704 python-amazon-sp-api-0.9.4/sp_api/api/listings_items/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/sp_api/api/listings_items/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8497 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/sp_api/api/listings_items/listings_items.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-18 12:09:40.577704 python-amazon-sp-api-0.9.4/sp_api/api/listings_restrictions/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/sp_api/api/listings_restrictions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1737 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/sp_api/api/listings_restrictions/listings_restrictions.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-18 12:09:40.577704 python-amazon-sp-api-0.9.4/sp_api/api/merchant_fulfillment/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/sp_api/api/merchant_fulfillment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15301 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/sp_api/api/merchant_fulfillment/merchant_fulfillment.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-18 12:09:40.577704 python-amazon-sp-api-0.9.4/sp_api/api/messaging/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/sp_api/api/messaging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16124 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/sp_api/api/messaging/messaging.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-18 12:09:40.577704 python-amazon-sp-api-0.9.4/sp_api/api/notifications/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/sp_api/api/notifications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10798 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/sp_api/api/notifications/notifications.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-18 12:09:40.577704 python-amazon-sp-api-0.9.4/sp_api/api/orders/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/sp_api/api/orders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9424 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/sp_api/api/orders/orders.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-18 12:09:40.577704 python-amazon-sp-api-0.9.4/sp_api/api/product_fees/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/sp_api/api/product_fees/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4545 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/sp_api/api/product_fees/product_fees.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-18 12:09:40.577704 python-amazon-sp-api-0.9.4/sp_api/api/product_type_definitions/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/sp_api/api/product_type_definitions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4471 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/sp_api/api/product_type_definitions/product_type_definitions.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-18 12:09:40.577704 python-amazon-sp-api-0.9.4/sp_api/api/products/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/sp_api/api/products/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7402 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/sp_api/api/products/products.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-18 12:09:40.577704 python-amazon-sp-api-0.9.4/sp_api/api/reports/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/sp_api/api/reports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13954 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/sp_api/api/reports/reports.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15883 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/sp_api/api/reports/reports_v2.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-18 12:09:40.577704 python-amazon-sp-api-0.9.4/sp_api/api/sales/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/sp_api/api/sales/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5627 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/sp_api/api/sales/sales.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-18 12:09:40.577704 python-amazon-sp-api-0.9.4/sp_api/api/sellers/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/sp_api/api/sellers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      305 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/sp_api/api/sellers/sellers.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-18 12:09:40.577704 python-amazon-sp-api-0.9.4/sp_api/api/services/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/sp_api/api/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9133 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/sp_api/api/services/services.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-18 12:09:40.577704 python-amazon-sp-api-0.9.4/sp_api/api/shipping/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/sp_api/api/shipping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14506 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/sp_api/api/shipping/shipping.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-18 12:09:40.577704 python-amazon-sp-api-0.9.4/sp_api/api/solicitations/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/sp_api/api/solicitations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3854 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/sp_api/api/solicitations/solicitations.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-18 12:09:40.581704 python-amazon-sp-api-0.9.4/sp_api/api/tokens/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/sp_api/api/tokens/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3380 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/sp_api/api/tokens/tokens.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-18 12:09:40.581704 python-amazon-sp-api-0.9.4/sp_api/api/upload/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/sp_api/api/upload/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      596 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/sp_api/api/upload/upload.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-18 12:09:40.581704 python-amazon-sp-api-0.9.4/sp_api/api/vendor_direct_fulfillment_inventory/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/sp_api/api/vendor_direct_fulfillment_inventory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2286 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/sp_api/api/vendor_direct_fulfillment_inventory/vendor_direct_fulfillment_inventory.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-18 12:09:40.581704 python-amazon-sp-api-0.9.4/sp_api/api/vendor_direct_fulfillment_orders/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/sp_api/api/vendor_direct_fulfillment_orders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9463 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/sp_api/api/vendor_direct_fulfillment_orders/vendor_direct_fulfillment_orders.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-18 12:09:40.581704 python-amazon-sp-api-0.9.4/sp_api/api/vendor_direct_fulfillment_payments/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/sp_api/api/vendor_direct_fulfillment_payments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10146 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/sp_api/api/vendor_direct_fulfillment_payments/vendor_direct_fulfillment_payments.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-18 12:09:40.581704 python-amazon-sp-api-0.9.4/sp_api/api/vendor_direct_fulfillment_shipping/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/sp_api/api/vendor_direct_fulfillment_shipping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    28770 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/sp_api/api/vendor_direct_fulfillment_shipping/vendor_direct_fulfillment_shipping.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-18 12:09:40.581704 python-amazon-sp-api-0.9.4/sp_api/api/vendor_direct_fulfillment_transactions/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/sp_api/api/vendor_direct_fulfillment_transactions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1701 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/sp_api/api/vendor_direct_fulfillment_transactions/vendor_direct_fulfillment_transactions.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-18 12:09:40.581704 python-amazon-sp-api-0.9.4/sp_api/api/vendor_invoices/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/sp_api/api/vendor_invoices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11192 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/sp_api/api/vendor_invoices/vendor_invoices.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-18 12:09:40.581704 python-amazon-sp-api-0.9.4/sp_api/api/vendor_orders/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/sp_api/api/vendor_orders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13391 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/sp_api/api/vendor_orders/vendor_orders.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-18 12:09:40.581704 python-amazon-sp-api-0.9.4/sp_api/api/vendor_shipments/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/sp_api/api/vendor_shipments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11627 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/sp_api/api/vendor_shipments/vendor_shipments.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-18 12:09:40.581704 python-amazon-sp-api-0.9.4/sp_api/api/vendor_transaction_status/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/sp_api/api/vendor_transaction_status/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1679 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/sp_api/api/vendor_transaction_status/vendor_transaction_status.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-18 12:09:40.581704 python-amazon-sp-api-0.9.4/sp_api/auth/
+-rw-r--r--   0 runner    (1001) docker     (121)      229 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/sp_api/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6136 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/sp_api/auth/access_token_client.py
+-rw-r--r--   0 runner    (1001) docker     (121)      272 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/sp_api/auth/access_token_response.py
+-rw-r--r--   0 runner    (1001) docker     (121)      262 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/sp_api/auth/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (121)      424 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/sp_api/auth/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-18 12:09:40.581704 python-amazon-sp-api-0.9.4/sp_api/base/
+-rw-r--r--   0 runner    (1001) docker     (121)      960 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/sp_api/base/ApiResponse.py
+-rw-r--r--   0 runner    (1001) docker     (121)       90 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/sp_api/base/InventoryEnums.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1835 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/sp_api/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3722 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/sp_api/base/aws_sig_v4.py
+-rw-r--r--   0 runner    (1001) docker     (121)      405 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/sp_api/base/base_client.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5783 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/sp_api/base/client.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3481 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/sp_api/base/config.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10481 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/sp_api/base/credential_provider.py
+-rw-r--r--   0 runner    (1001) docker     (121)      656 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/sp_api/base/deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2969 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/sp_api/base/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)       93 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/sp_api/base/fulfillment_channel.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2713 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/sp_api/base/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2926 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/sp_api/base/marketplaces.py
+-rw-r--r--   0 runner    (1001) docker     (121)      613 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/sp_api/base/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (121)      183 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/sp_api/base/processing_status.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7651 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/sp_api/base/reportTypes.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2714 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/sp_api/base/report_headers.py
+-rw-r--r--   0 runner    (1001) docker     (121)      179 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/sp_api/base/report_status.py
+-rw-r--r--   0 runner    (1001) docker     (121)      379 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/sp_api/base/sales_enum.py
+-rw-r--r--   0 runner    (1001) docker     (121)      433 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/sp_api/base/schedules.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-18 12:09:40.585704 python-amazon-sp-api-0.9.4/sp_api/util/
+-rw-r--r--   0 runner    (1001) docker     (121)      229 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/sp_api/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2151 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/sp_api/util/key_maker.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1310 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/sp_api/util/load_all_pages.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2411 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/sp_api/util/retry.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-18 12:09:40.585704 python-amazon-sp-api-0.9.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-18 12:09:40.585704 python-amazon-sp-api-0.9.4/tests/api/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/tests/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-18 12:09:40.585704 python-amazon-sp-api-0.9.4/tests/api/finances/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/tests/api/finances/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      584 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/tests/api/finances/test_finances.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-18 12:09:40.585704 python-amazon-sp-api-0.9.4/tests/api/notifications/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/tests/api/notifications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1293 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/tests/api/notifications/test_notifications.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-18 12:09:40.585704 python-amazon-sp-api-0.9.4/tests/api/orders/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/tests/api/orders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1509 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/tests/api/orders/test_orders.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-18 12:09:40.585704 python-amazon-sp-api-0.9.4/tests/api/product_fees/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/tests/api/product_fees/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1610 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/tests/api/product_fees/product_fees.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-18 12:09:40.585704 python-amazon-sp-api-0.9.4/tests/api/reports/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/tests/api/reports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3600 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/tests/api/reports/test_reports.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3623 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/tests/api/reports/test_reports_v2.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-18 12:09:40.585704 python-amazon-sp-api-0.9.4/tests/api/sellers/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/tests/api/sellers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/tests/api/sellers/test_sellers.py
+-rw-r--r--   0 runner    (1001) docker     (121)      185 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/tests/base.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-18 12:09:40.585704 python-amazon-sp-api-0.9.4/tests/client/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/tests/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/tests/client/auth.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1373 2021-12-18 12:09:32.000000 python-amazon-sp-api-0.9.4/tests/test_helpers.py
```

### Comparing `python-amazon-sp-api-0.9.2/LICENSE` & `python-amazon-sp-api-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-0.9.2/PKG-INFO` & `python-amazon-sp-api-0.9.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-amazon-sp-api
-Version: 0.9.2
+Version: 0.9.4
 Summary: Python wrapper for the Amazon Selling-Partner API
 Home-page: https://github.com/saleweaver/python-amazon-sp-api
 Author: Michael
 Author-email: info@saleweaver.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `python-amazon-sp-api-0.9.2/README.md` & `python-amazon-sp-api-0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-0.9.2/python_amazon_sp_api.egg-info/PKG-INFO` & `python-amazon-sp-api-0.9.4/python_amazon_sp_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-amazon-sp-api
-Version: 0.9.2
+Version: 0.9.4
 Summary: Python wrapper for the Amazon Selling-Partner API
 Home-page: https://github.com/saleweaver/python-amazon-sp-api
 Author: Michael
 Author-email: info@saleweaver.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `python-amazon-sp-api-0.9.2/python_amazon_sp_api.egg-info/SOURCES.txt` & `python-amazon-sp-api-0.9.4/python_amazon_sp_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-0.9.2/setup.py` & `python-amazon-sp-api-0.9.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='python-amazon-sp-api',
-    version='0.9.2',
+    version='0.9.4',
     install_requires=[
         "requests",
         "six>=1.15,<2",
         "boto3>=1.16.39,<2",
         "cachetools~=4.2.0",
         "pycryptodome",
         "pytz",
```

### Comparing `python-amazon-sp-api-0.9.2/sp_api/api/__init__.py` & `python-amazon-sp-api-0.9.4/sp_api/api/__init__.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-0.9.2/sp_api/api/aplus_content/aplus_content.py` & `python-amazon-sp-api-0.9.4/sp_api/api/aplus_content/aplus_content.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-0.9.2/sp_api/api/authorization/authorization.py` & `python-amazon-sp-api-0.9.4/sp_api/api/authorization/authorization.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-0.9.2/sp_api/api/catalog/catalog.py` & `python-amazon-sp-api-0.9.4/sp_api/api/catalog/catalog.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-0.9.2/sp_api/api/catalog_items/catalog_items.py` & `python-amazon-sp-api-0.9.4/sp_api/api/catalog_items/catalog_items.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-0.9.2/sp_api/api/fba_inbound_eligibility/fba_inbound_eligibility.py` & `python-amazon-sp-api-0.9.4/sp_api/api/fba_inbound_eligibility/fba_inbound_eligibility.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-0.9.2/sp_api/api/fba_small_and_light/fba_small_and_light.py` & `python-amazon-sp-api-0.9.4/sp_api/api/fba_small_and_light/fba_small_and_light.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-0.9.2/sp_api/api/feeds/feeds.py` & `python-amazon-sp-api-0.9.4/sp_api/api/feeds/feeds.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-0.9.2/sp_api/api/feeds/feeds_v2.py` & `python-amazon-sp-api-0.9.4/sp_api/api/feeds/feeds_v2.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,45 +17,63 @@
     @sp_endpoint('/feeds/2021-06-30/feeds', method='GET')
     def get_feeds(self, **kwargs) -> ApiResponse:
         """
         get_feeds(self, **kwargs) -> ApiResponse
 
         Returns feed details for the feeds that match the filters that you specify.
 
-**Usage Plan:**
-
-| Rate (requests per second) | Burst |
-| ---- | ---- |
-| 0.0222 | 10 |
-
-For more information, see "Usage Plans and Rate Limits" in the Selling Partner API documentation.
-
-         Args:
-        
+        Args:
             key feedTypes:array |  A list of feed types used to filter feeds. When feedTypes is provided, the other filter parameters (processingStatuses, marketplaceIds, createdSince, createdUntil) and pageSize may also be provided. Either feedTypes or nextToken is required.
-        
             key marketplaceIds:array |  A list of marketplace identifiers used to filter feeds. The feeds returned will match at least one of the marketplaces that you specify.
-        
             key pageSize:integer |  The maximum number of feeds to return in a single call.
-        
             key processingStatuses:array |  A list of processing statuses used to filter feeds.
-        
             key createdSince:string |  The earliest feed creation date and time for feeds included in the response, in ISO 8601 format. The default is 90 days ago. Feeds are retained for a maximum of 90 days.
-        
             key createdUntil:string |  The latest feed creation date and time for feeds included in the response, in ISO 8601 format. The default is now.
-        
             key nextToken:string |  A string token returned in the response to your previous request. nextToken is returned when the number of results exceeds the specified pageSize value. To get the next page of results, call the getFeeds operation and include this token as the only parameter. Specifying nextToken with any other parameters will cause the request to fail.
         
 
-         Returns:
+        Returns:
             ApiResponse:
         """
     
         return self._request(kwargs.pop('path'),  params=kwargs)
     
+    def submit_feed(self, feed_type, file, content_type='text/tsv', **kwargs) -> [ApiResponse, ApiResponse]:
+        """
+        submit_feed(self, feed_type: str, file: File or File like, content_type='text/tsv', **kwargs) -> [ApiResponse, ApiResponse]
+        Combines `create_feed_document` and `create_feed`, uploads the file and sends the feed to amazon.
+
+        **Usage Plan:**
+
+        ======================================  ==============
+        Rate (requests per second)               Burst
+        ======================================  ==============
+        0.0083                                  15
+        ======================================  ==============
+
+        Examples:
+            literal blocks::
+
+                feed = BytesIO
+                feed.write(<your feed>)
+                feed.seek(0)
+                Feeds().submit_feed('POST_FBA_INBOUND_CARTON_CONTENTS', feed, 'text/xml')
+
+
+        Args:
+            feed_type:
+            file:
+            content_type:
+            **kwargs:
+
+        Returns:
+            [CreateFeedDocumentResponse, CreateFeedResponse]:
+        """
+        document_response = self.create_feed_document(file, content_type)
+        return document_response, self.create_feed(feed_type, document_response.payload.get('feedDocumentId'), **kwargs)
 
     @sp_endpoint('/feeds/2021-06-30/feeds', method='POST')
     def create_feed(self, feed_type, input_feed_document_id, **kwargs) -> ApiResponse:
         """
         create_feed(self, feed_type: str, input_feed_document_id: str, **kwargs) -> ApiResponse
 
         Creates a feed. Call `create_feed_document` to upload the feed first.
@@ -96,74 +114,52 @@
     @sp_endpoint('/feeds/2021-06-30/feeds/{}', method='DELETE')
     def cancel_feed(self, feedId, **kwargs) -> ApiResponse:
         """
         cancel_feed(self, feedId, **kwargs) -> ApiResponse
 
         Cancels the feed that you specify. Only feeds with processingStatus=IN_QUEUE can be cancelled. Cancelled feeds are returned in subsequent calls to the getFeed and getFeeds operations.
 
-**Usage Plan:**
-
-| Rate (requests per second) | Burst |
-| ---- | ---- |
-| 0.0222 | 10 |
-
-For more information, see "Usage Plans and Rate Limits" in the Selling Partner API documentation.
-
-         Args:
+        Args:
         
             feedId:string | * REQUIRED The identifier for the feed. This identifier is unique only in combination with a seller ID.
         
 
-         Returns:
+        Returns:
             ApiResponse:
         """
     
         return self._request(fill_query_params(kwargs.pop('path'), feedId), data=kwargs)
     
 
     @sp_endpoint('/feeds/2021-06-30/feeds/{}', method='GET')
     def get_feed(self, feedId, **kwargs) -> ApiResponse:
         """
         get_feed(self, feedId, **kwargs) -> ApiResponse
 
         Returns feed details (including the resultDocumentId, if available) for the feed that you specify.
 
-**Usage Plan:**
-
-| Rate (requests per second) | Burst |
-| ---- | ---- |
-| 2.0 | 15 |
-
-For more information, see "Usage Plans and Rate Limits" in the Selling Partner API documentation.
-
-         Args:
+        Args:
         
             feedId:string | * REQUIRED The identifier for the feed. This identifier is unique only in combination with a seller ID.
         
 
-         Returns:
+        Returns:
             ApiResponse:
         """
     
         return self._request(fill_query_params(kwargs.pop('path'), feedId), params=kwargs)
     
 
     @sp_endpoint('/feeds/2021-06-30/documents', method='POST')
     def create_feed_document(self, file, content_type, **kwargs) -> ApiResponse:
         """
         create_feed_document(self, **kwargs) -> ApiResponse
 
         Creates a feed document for the feed type that you specify. This operation returns a presigned URL for uploading the feed document contents. It also returns a feedDocumentId value that you can pass in with a subsequent call to the createFeed operation.
 
-        **Usage Plan:**
-
-        | Rate (requests per second) | Burst |
-        | ---- | ---- |
-        | 0.0083 | 15 |
-
         For more information, see "Usage Plans and Rate Limits" in the Selling Partner API documentation.
 
         Args:
             file: File or File like object
             content_type: str
             body: | * REQUIRED {'description': 'Specifies the content type for the createFeedDocument operation.', 'properties': {'contentType': {'description': 'The content type of the feed.', 'type': 'string'}}, 'required': ['contentType'], 'type': 'object'}
         
@@ -188,26 +184,19 @@
     @sp_endpoint('/feeds/2021-06-30/documents/{}', method='GET')
     def get_feed_document(self, feedDocumentId, **kwargs) -> ApiResponse:
         """
         get_feed_document(self, feedDocumentId, **kwargs) -> ApiResponse
 
         Returns the information required for retrieving a feed document's contents.
 
-**Usage Plan:**
-
-| Rate (requests per second) | Burst |
-| ---- | ---- |
-| 0.0222 | 10 |
-
-For more information, see "Usage Plans and Rate Limits" in the Selling Partner API documentation.
+        For more information, see "Usage Plans and Rate Limits" in the Selling Partner API documentation.
 
-         Args:
+        Args:
         
             feedDocumentId:string | * REQUIRED The identifier of the feed document.
         
 
-         Returns:
+        Returns:
             ApiResponse:
         """
     
         return self._request(fill_query_params(kwargs.pop('path'), feedDocumentId), params=kwargs)
-
```

### Comparing `python-amazon-sp-api-0.9.2/sp_api/api/finances/finances.py` & `python-amazon-sp-api-0.9.4/sp_api/api/finances/finances.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-0.9.2/sp_api/api/fulfillment_inbound/fulfillment_inbound.py` & `python-amazon-sp-api-0.9.4/sp_api/api/fulfillment_inbound/fulfillment_inbound.py`

 * *Files 4% similar despite different names*

```diff
@@ -171,14 +171,24 @@
         Returns:
             ApiResponse
         """
         return self._request(fill_query_params(kwargs.pop('path'), shipment_id), params=kwargs)
 
     @sp_endpoint("/fba/inbound/v0/shipments/{}/preorder/confirm", method='PUT')
     def confirm_preorder(self, shipment_id, **kwargs):
+        """
+        confirm_preorder(self, shipment_id, **kwargs)
+
+        Args:
+            shipment_id:
+            **kwargs:
+
+        Returns:
+
+        """
         return self._request(fill_query_params(kwargs.pop('path'), shipment_id), params=kwargs)
 
     @sp_endpoint("/fba/inbound/v0/prepInstructions")
     def prep_instruction(self, data, **kwargs):
         """
         prep_instruction(self, data, **kwargs) -> ApiResponse
 
@@ -269,14 +279,24 @@
 
     @sp_endpoint("/fba/inbound/v0/shipments/{}/transport/confirm", method='POST')
     def confirm_transport(self, shipment_id, **kwargs):
         return self._request(fill_query_params(kwargs.pop('path'), shipment_id), data=kwargs, add_marketplace=False)
 
     @sp_endpoint("/fba/inbound/v0/shipments/{}/labels")
     def get_labels(self, shipment_id, **kwargs):
+        """
+        get_labels(self, shipment_id, **kwargs)
+
+        Args:
+            shipment_id:
+            **kwargs:
+
+        Returns:
+
+        """
         return self._request(fill_query_params(kwargs.pop('path'), shipment_id), params=kwargs, add_marketplace=False)
 
     @sp_endpoint("/fba/inbound/v0/shipments/{}/billOfLading")
     def bill_of_lading(self, shipment_id, **kwargs):
         """
         bill_of_lading(self, shipment_id, **kwargs) -> ApiResponse
```

### Comparing `python-amazon-sp-api-0.9.2/sp_api/api/fulfillment_outbound/fulfillment_outbound.py` & `python-amazon-sp-api-0.9.4/sp_api/api/fulfillment_outbound/fulfillment_outbound.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-0.9.2/sp_api/api/inventories/inventories.py` & `python-amazon-sp-api-0.9.4/sp_api/api/inventories/inventories.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-0.9.2/sp_api/api/listings_items/listings_items.py` & `python-amazon-sp-api-0.9.4/sp_api/api/listings_items/listings_items.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-0.9.2/sp_api/api/merchant_fulfillment/merchant_fulfillment.py` & `python-amazon-sp-api-0.9.4/sp_api/api/merchant_fulfillment/merchant_fulfillment.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-0.9.2/sp_api/api/messaging/messaging.py` & `python-amazon-sp-api-0.9.4/sp_api/api/messaging/messaging.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-0.9.2/sp_api/api/notifications/notifications.py` & `python-amazon-sp-api-0.9.4/sp_api/api/notifications/notifications.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-0.9.2/sp_api/api/orders/orders.py` & `python-amazon-sp-api-0.9.4/sp_api/api/orders/orders.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-0.9.2/sp_api/api/product_fees/product_fees.py` & `python-amazon-sp-api-0.9.4/sp_api/api/product_fees/product_fees.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-0.9.2/sp_api/api/product_type_definitions/product_type_definitions.py` & `python-amazon-sp-api-0.9.4/sp_api/api/product_type_definitions/product_type_definitions.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-0.9.2/sp_api/api/products/products.py` & `python-amazon-sp-api-0.9.4/sp_api/api/products/products.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-0.9.2/sp_api/api/reports/reports.py` & `python-amazon-sp-api-0.9.4/sp_api/api/reports/reports.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-0.9.2/sp_api/api/reports/reports_v2.py` & `python-amazon-sp-api-0.9.4/sp_api/api/reports/reports_v2.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-0.9.2/sp_api/api/sales/sales.py` & `python-amazon-sp-api-0.9.4/sp_api/api/sales/sales.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-0.9.2/sp_api/api/services/services.py` & `python-amazon-sp-api-0.9.4/sp_api/api/services/services.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-0.9.2/sp_api/api/shipping/shipping.py` & `python-amazon-sp-api-0.9.4/sp_api/api/shipping/shipping.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-0.9.2/sp_api/api/solicitations/solicitations.py` & `python-amazon-sp-api-0.9.4/sp_api/api/solicitations/solicitations.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-0.9.2/sp_api/api/tokens/tokens.py` & `python-amazon-sp-api-0.9.4/sp_api/api/tokens/tokens.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-0.9.2/sp_api/api/upload/upload.py` & `python-amazon-sp-api-0.9.4/sp_api/api/upload/upload.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-0.9.2/sp_api/api/vendor_direct_fulfillment_inventory/vendor_direct_fulfillment_inventory.py` & `python-amazon-sp-api-0.9.4/sp_api/api/vendor_direct_fulfillment_inventory/vendor_direct_fulfillment_inventory.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-0.9.2/sp_api/api/vendor_direct_fulfillment_orders/vendor_direct_fulfillment_orders.py` & `python-amazon-sp-api-0.9.4/sp_api/api/vendor_direct_fulfillment_orders/vendor_direct_fulfillment_orders.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-0.9.2/sp_api/api/vendor_direct_fulfillment_payments/vendor_direct_fulfillment_payments.py` & `python-amazon-sp-api-0.9.4/sp_api/api/vendor_direct_fulfillment_payments/vendor_direct_fulfillment_payments.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-0.9.2/sp_api/api/vendor_direct_fulfillment_shipping/vendor_direct_fulfillment_shipping.py` & `python-amazon-sp-api-0.9.4/sp_api/api/vendor_direct_fulfillment_shipping/vendor_direct_fulfillment_shipping.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-0.9.2/sp_api/api/vendor_direct_fulfillment_transactions/vendor_direct_fulfillment_transactions.py` & `python-amazon-sp-api-0.9.4/sp_api/api/vendor_direct_fulfillment_transactions/vendor_direct_fulfillment_transactions.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-0.9.2/sp_api/api/vendor_invoices/vendor_invoices.py` & `python-amazon-sp-api-0.9.4/sp_api/api/vendor_invoices/vendor_invoices.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-0.9.2/sp_api/api/vendor_orders/vendor_orders.py` & `python-amazon-sp-api-0.9.4/sp_api/api/vendor_orders/vendor_orders.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-0.9.2/sp_api/api/vendor_shipments/vendor_shipments.py` & `python-amazon-sp-api-0.9.4/sp_api/api/vendor_shipments/vendor_shipments.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-0.9.2/sp_api/api/vendor_transaction_status/vendor_transaction_status.py` & `python-amazon-sp-api-0.9.4/sp_api/api/vendor_transaction_status/vendor_transaction_status.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-0.9.2/sp_api/auth/access_token_client.py` & `python-amazon-sp-api-0.9.4/sp_api/auth/access_token_client.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-0.9.2/sp_api/base/ApiResponse.py` & `python-amazon-sp-api-0.9.4/sp_api/base/ApiResponse.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-0.9.2/sp_api/base/__init__.py` & `python-amazon-sp-api-0.9.4/sp_api/base/__init__.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-0.9.2/sp_api/base/aws_sig_v4.py` & `python-amazon-sp-api-0.9.4/sp_api/base/aws_sig_v4.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-0.9.2/sp_api/base/client.py` & `python-amazon-sp-api-0.9.4/sp_api/base/client.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-0.9.2/sp_api/base/config.py` & `python-amazon-sp-api-0.9.4/sp_api/base/config.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-0.9.2/sp_api/base/credential_provider.py` & `python-amazon-sp-api-0.9.4/sp_api/base/credential_provider.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-0.9.2/sp_api/base/deprecated.py` & `python-amazon-sp-api-0.9.4/sp_api/base/deprecated.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-0.9.2/sp_api/base/exceptions.py` & `python-amazon-sp-api-0.9.4/sp_api/base/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-0.9.2/sp_api/base/helpers.py` & `python-amazon-sp-api-0.9.4/sp_api/base/helpers.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-0.9.2/sp_api/base/marketplaces.py` & `python-amazon-sp-api-0.9.4/sp_api/base/marketplaces.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-0.9.2/sp_api/base/notifications.py` & `python-amazon-sp-api-0.9.4/sp_api/base/notifications.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-0.9.2/sp_api/base/reportTypes.py` & `python-amazon-sp-api-0.9.4/sp_api/base/reportTypes.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-0.9.2/sp_api/base/report_headers.py` & `python-amazon-sp-api-0.9.4/sp_api/base/report_headers.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-0.9.2/sp_api/util/key_maker.py` & `python-amazon-sp-api-0.9.4/sp_api/util/key_maker.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-0.9.2/sp_api/util/load_all_pages.py` & `python-amazon-sp-api-0.9.4/sp_api/util/load_all_pages.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-0.9.2/sp_api/util/retry.py` & `python-amazon-sp-api-0.9.4/sp_api/util/retry.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-0.9.2/tests/api/finances/test_finances.py` & `python-amazon-sp-api-0.9.4/tests/api/finances/test_finances.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-0.9.2/tests/api/notifications/test_notifications.py` & `python-amazon-sp-api-0.9.4/tests/api/notifications/test_notifications.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-0.9.2/tests/api/orders/test_orders.py` & `python-amazon-sp-api-0.9.4/tests/api/orders/test_orders.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-0.9.2/tests/api/product_fees/product_fees.py` & `python-amazon-sp-api-0.9.4/tests/api/product_fees/product_fees.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-0.9.2/tests/api/reports/test_reports.py` & `python-amazon-sp-api-0.9.4/tests/api/reports/test_reports.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-0.9.2/tests/api/reports/test_reports_v2.py` & `python-amazon-sp-api-0.9.4/tests/api/reports/test_reports_v2.py`

 * *Files identical despite different names*

### Comparing `python-amazon-sp-api-0.9.2/tests/test_helpers.py` & `python-amazon-sp-api-0.9.4/tests/test_helpers.py`

 * *Files identical despite different names*

