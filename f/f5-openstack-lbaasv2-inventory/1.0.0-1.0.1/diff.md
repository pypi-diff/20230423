# Comparing `tmp/f5-openstack-lbaasv2-inventory-1.0.0.tar.gz` & `tmp/f5-openstack-lbaasv2-inventory-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/f5-openstack-lbaasv2-inventory-1.0.0.tar", last modified: Thu Mar 30 07:54:49 2023, max compression
+gzip compressed data, was "dist/f5-openstack-lbaasv2-inventory-1.0.1.tar", last modified: Sun Apr 23 06:51:43 2023, max compression
```

## Comparing `f5-openstack-lbaasv2-inventory-1.0.0.tar` & `f5-openstack-lbaasv2-inventory-1.0.1.tar`

### file list

```diff
@@ -1,45 +1,44 @@
-drwxr-xr-x   0 qzhao     (1001) users      (100)        0 2023-03-30 07:54:49.000000 f5-openstack-lbaasv2-inventory-1.0.0/
--rw-r--r--   0 qzhao     (1001) users      (100)      680 2023-03-30 07:54:49.000000 f5-openstack-lbaasv2-inventory-1.0.0/PKG-INFO
--rw-r--r--   0 qzhao     (1001) users      (100)     6279 2023-03-30 07:52:56.000000 f5-openstack-lbaasv2-inventory-1.0.0/README.md
-drwxr-xr-x   0 qzhao     (1001) users      (100)        0 2023-03-30 07:54:49.000000 f5-openstack-lbaasv2-inventory-1.0.0/etc/
-drwxr-xr-x   0 qzhao     (1001) users      (100)        0 2023-03-30 07:54:49.000000 f5-openstack-lbaasv2-inventory-1.0.0/etc/neutron/
-drwxr-xr-x   0 qzhao     (1001) users      (100)        0 2023-03-30 07:54:49.000000 f5-openstack-lbaasv2-inventory-1.0.0/etc/neutron/policy.d/
--rw-r--r--   0 qzhao     (1001) users      (100)      198 2023-03-30 07:52:56.000000 f5-openstack-lbaasv2-inventory-1.0.0/etc/neutron/policy.d/lbaas_device.json
--rw-r--r--   0 qzhao     (1001) users      (100)       46 2023-03-30 07:52:56.000000 f5-openstack-lbaasv2-inventory-1.0.0/MANIFEST.in
-drwxr-xr-x   0 qzhao     (1001) users      (100)        0 2023-03-30 07:54:49.000000 f5-openstack-lbaasv2-inventory-1.0.0/neutron_lbaas_inventory/
-drwxr-xr-x   0 qzhao     (1001) users      (100)        0 2023-03-30 07:54:49.000000 f5-openstack-lbaasv2-inventory-1.0.0/neutron_lbaas_inventory/common/
--rw-r--r--   0 qzhao     (1001) users      (100)      136 2023-03-30 07:52:56.000000 f5-openstack-lbaasv2-inventory-1.0.0/neutron_lbaas_inventory/common/constants.py
--rw-r--r--   0 qzhao     (1001) users      (100)      321 2023-03-30 07:52:56.000000 f5-openstack-lbaasv2-inventory-1.0.0/neutron_lbaas_inventory/common/exceptions.py
--rw-r--r--   0 qzhao     (1001) users      (100)        0 2023-03-30 07:52:56.000000 f5-openstack-lbaasv2-inventory-1.0.0/neutron_lbaas_inventory/common/__init__.py
-drwxr-xr-x   0 qzhao     (1001) users      (100)        0 2023-03-30 07:54:49.000000 f5-openstack-lbaasv2-inventory-1.0.0/neutron_lbaas_inventory/plugins/
--rw-r--r--   0 qzhao     (1001) users      (100)     1912 2023-03-30 07:52:56.000000 f5-openstack-lbaasv2-inventory-1.0.0/neutron_lbaas_inventory/plugins/lbaasdevice.py
--rw-r--r--   0 qzhao     (1001) users      (100)        0 2023-03-30 07:52:56.000000 f5-openstack-lbaasv2-inventory-1.0.0/neutron_lbaas_inventory/plugins/__init__.py
-drwxr-xr-x   0 qzhao     (1001) users      (100)        0 2023-03-30 07:54:49.000000 f5-openstack-lbaasv2-inventory-1.0.0/neutron_lbaas_inventory/extensions/
--rw-r--r--   0 qzhao     (1001) users      (100)     5442 2023-03-30 07:52:56.000000 f5-openstack-lbaasv2-inventory-1.0.0/neutron_lbaas_inventory/extensions/lbaasdevice.py
--rw-r--r--   0 qzhao     (1001) users      (100)        0 2023-03-30 07:52:56.000000 f5-openstack-lbaasv2-inventory-1.0.0/neutron_lbaas_inventory/extensions/__init__.py
-drwxr-xr-x   0 qzhao     (1001) users      (100)        0 2023-03-30 07:54:49.000000 f5-openstack-lbaasv2-inventory-1.0.0/neutron_lbaas_inventory/db/
-drwxr-xr-x   0 qzhao     (1001) users      (100)        0 2023-03-30 07:54:49.000000 f5-openstack-lbaasv2-inventory-1.0.0/neutron_lbaas_inventory/db/models/
--rw-r--r--   0 qzhao     (1001) users      (100)      110 2023-03-30 07:52:56.000000 f5-openstack-lbaasv2-inventory-1.0.0/neutron_lbaas_inventory/db/models/head.py
--rw-r--r--   0 qzhao     (1001) users      (100)      827 2023-03-30 07:52:56.000000 f5-openstack-lbaasv2-inventory-1.0.0/neutron_lbaas_inventory/db/models/inventory.py
--rw-r--r--   0 qzhao     (1001) users      (100)        0 2023-03-30 07:52:56.000000 f5-openstack-lbaasv2-inventory-1.0.0/neutron_lbaas_inventory/db/models/__init__.py
--rw-r--r--   0 qzhao     (1001) users      (100)      820 2023-03-30 07:52:56.000000 f5-openstack-lbaasv2-inventory-1.0.0/neutron_lbaas_inventory/db/lb_device_binding_db.py
-drwxr-xr-x   0 qzhao     (1001) users      (100)        0 2023-03-30 07:54:49.000000 f5-openstack-lbaasv2-inventory-1.0.0/neutron_lbaas_inventory/db/migration/
-drwxr-xr-x   0 qzhao     (1001) users      (100)        0 2023-03-30 07:54:49.000000 f5-openstack-lbaasv2-inventory-1.0.0/neutron_lbaas_inventory/db/migration/alembic_migrations/
--rw-r--r--   0 qzhao     (1001) users      (100)      991 2023-03-30 07:52:56.000000 f5-openstack-lbaasv2-inventory-1.0.0/neutron_lbaas_inventory/db/migration/alembic_migrations/inventory_init_ops.py
--rw-r--r--   0 qzhao     (1001) users      (100)     2076 2023-03-30 07:52:56.000000 f5-openstack-lbaasv2-inventory-1.0.0/neutron_lbaas_inventory/db/migration/alembic_migrations/env.py
--rw-r--r--   0 qzhao     (1001) users      (100)        0 2023-03-30 07:52:56.000000 f5-openstack-lbaasv2-inventory-1.0.0/neutron_lbaas_inventory/db/migration/alembic_migrations/__init__.py
-drwxr-xr-x   0 qzhao     (1001) users      (100)        0 2023-03-30 07:54:49.000000 f5-openstack-lbaasv2-inventory-1.0.0/neutron_lbaas_inventory/db/migration/alembic_migrations/versions/
--rw-r--r--   0 qzhao     (1001) users      (100)        0 2023-03-30 07:52:56.000000 f5-openstack-lbaasv2-inventory-1.0.0/neutron_lbaas_inventory/db/migration/alembic_migrations/versions/__init__.py
--rw-r--r--   0 qzhao     (1001) users      (100)      281 2023-03-30 07:52:56.000000 f5-openstack-lbaasv2-inventory-1.0.0/neutron_lbaas_inventory/db/migration/alembic_migrations/versions/pike_initial.py
--rw-r--r--   0 qzhao     (1001) users      (100)        0 2023-03-30 07:52:56.000000 f5-openstack-lbaasv2-inventory-1.0.0/neutron_lbaas_inventory/db/migration/__init__.py
--rw-r--r--   0 qzhao     (1001) users      (100)        0 2023-03-30 07:52:56.000000 f5-openstack-lbaasv2-inventory-1.0.0/neutron_lbaas_inventory/db/__init__.py
--rw-r--r--   0 qzhao     (1001) users      (100)     4560 2023-03-30 07:52:56.000000 f5-openstack-lbaasv2-inventory-1.0.0/neutron_lbaas_inventory/db/inventory_db.py
--rw-r--r--   0 qzhao     (1001) users      (100)       22 2023-03-30 07:52:56.000000 f5-openstack-lbaasv2-inventory-1.0.0/neutron_lbaas_inventory/__init__.py
--rw-r--r--   0 qzhao     (1001) users      (100)     1239 2023-03-30 07:52:56.000000 f5-openstack-lbaasv2-inventory-1.0.0/setup.py
--rw-r--r--   0 qzhao     (1001) users      (100)       38 2023-03-30 07:54:49.000000 f5-openstack-lbaasv2-inventory-1.0.0/setup.cfg
-drwxr-xr-x   0 qzhao     (1001) users      (100)        0 2023-03-30 07:54:49.000000 f5-openstack-lbaasv2-inventory-1.0.0/f5_openstack_lbaasv2_inventory.egg-info/
--rw-r--r--   0 qzhao     (1001) users      (100)      680 2023-03-30 07:54:49.000000 f5-openstack-lbaasv2-inventory-1.0.0/f5_openstack_lbaasv2_inventory.egg-info/PKG-INFO
--rw-r--r--   0 qzhao     (1001) users      (100)      219 2023-03-30 07:54:49.000000 f5-openstack-lbaasv2-inventory-1.0.0/f5_openstack_lbaasv2_inventory.egg-info/entry_points.txt
--rw-r--r--   0 qzhao     (1001) users      (100)     1382 2023-03-30 07:54:49.000000 f5-openstack-lbaasv2-inventory-1.0.0/f5_openstack_lbaasv2_inventory.egg-info/SOURCES.txt
--rw-r--r--   0 qzhao     (1001) users      (100)       24 2023-03-30 07:54:49.000000 f5-openstack-lbaasv2-inventory-1.0.0/f5_openstack_lbaasv2_inventory.egg-info/top_level.txt
--rw-r--r--   0 qzhao     (1001) users      (100)        1 2023-03-30 07:54:49.000000 f5-openstack-lbaasv2-inventory-1.0.0/f5_openstack_lbaasv2_inventory.egg-info/dependency_links.txt
+drwxr-xr-x   0 qzhao     (1001) users      (100)        0 2023-04-23 06:51:43.000000 f5-openstack-lbaasv2-inventory-1.0.1/
+-rw-r--r--   0 qzhao     (1001) users      (100)      680 2023-04-23 06:51:43.000000 f5-openstack-lbaasv2-inventory-1.0.1/PKG-INFO
+-rw-r--r--   0 qzhao     (1001) users      (100)     6279 2023-03-30 07:52:56.000000 f5-openstack-lbaasv2-inventory-1.0.1/README.md
+drwxr-xr-x   0 qzhao     (1001) users      (100)        0 2023-04-23 06:51:43.000000 f5-openstack-lbaasv2-inventory-1.0.1/etc/
+drwxr-xr-x   0 qzhao     (1001) users      (100)        0 2023-04-23 06:51:43.000000 f5-openstack-lbaasv2-inventory-1.0.1/etc/neutron/
+drwxr-xr-x   0 qzhao     (1001) users      (100)        0 2023-04-23 06:51:43.000000 f5-openstack-lbaasv2-inventory-1.0.1/etc/neutron/policy.d/
+-rw-r--r--   0 qzhao     (1001) users      (100)      484 2023-04-23 06:39:33.000000 f5-openstack-lbaasv2-inventory-1.0.1/etc/neutron/policy.d/lbaas_device.json
+-rw-r--r--   0 qzhao     (1001) users      (100)       46 2023-03-30 07:52:56.000000 f5-openstack-lbaasv2-inventory-1.0.1/MANIFEST.in
+drwxr-xr-x   0 qzhao     (1001) users      (100)        0 2023-04-23 06:51:43.000000 f5-openstack-lbaasv2-inventory-1.0.1/neutron_lbaas_inventory/
+drwxr-xr-x   0 qzhao     (1001) users      (100)        0 2023-04-23 06:51:43.000000 f5-openstack-lbaasv2-inventory-1.0.1/neutron_lbaas_inventory/common/
+-rw-r--r--   0 qzhao     (1001) users      (100)      136 2023-03-30 07:52:56.000000 f5-openstack-lbaasv2-inventory-1.0.1/neutron_lbaas_inventory/common/constants.py
+-rw-r--r--   0 qzhao     (1001) users      (100)      591 2023-04-23 06:39:33.000000 f5-openstack-lbaasv2-inventory-1.0.1/neutron_lbaas_inventory/common/exceptions.py
+-rw-r--r--   0 qzhao     (1001) users      (100)        0 2023-03-30 07:52:56.000000 f5-openstack-lbaasv2-inventory-1.0.1/neutron_lbaas_inventory/common/__init__.py
+drwxr-xr-x   0 qzhao     (1001) users      (100)        0 2023-04-23 06:51:43.000000 f5-openstack-lbaasv2-inventory-1.0.1/neutron_lbaas_inventory/plugins/
+-rw-r--r--   0 qzhao     (1001) users      (100)     3068 2023-04-23 06:39:33.000000 f5-openstack-lbaasv2-inventory-1.0.1/neutron_lbaas_inventory/plugins/lbaasdevice.py
+-rw-r--r--   0 qzhao     (1001) users      (100)        0 2023-03-30 07:52:56.000000 f5-openstack-lbaasv2-inventory-1.0.1/neutron_lbaas_inventory/plugins/__init__.py
+drwxr-xr-x   0 qzhao     (1001) users      (100)        0 2023-04-23 06:51:43.000000 f5-openstack-lbaasv2-inventory-1.0.1/neutron_lbaas_inventory/extensions/
+-rw-r--r--   0 qzhao     (1001) users      (100)     8462 2023-04-23 06:39:33.000000 f5-openstack-lbaasv2-inventory-1.0.1/neutron_lbaas_inventory/extensions/lbaasdevice.py
+-rw-r--r--   0 qzhao     (1001) users      (100)        0 2023-03-30 07:52:56.000000 f5-openstack-lbaasv2-inventory-1.0.1/neutron_lbaas_inventory/extensions/__init__.py
+drwxr-xr-x   0 qzhao     (1001) users      (100)        0 2023-04-23 06:51:43.000000 f5-openstack-lbaasv2-inventory-1.0.1/neutron_lbaas_inventory/db/
+drwxr-xr-x   0 qzhao     (1001) users      (100)        0 2023-04-23 06:51:43.000000 f5-openstack-lbaasv2-inventory-1.0.1/neutron_lbaas_inventory/db/models/
+-rw-r--r--   0 qzhao     (1001) users      (100)      110 2023-03-30 07:52:56.000000 f5-openstack-lbaasv2-inventory-1.0.1/neutron_lbaas_inventory/db/models/head.py
+-rw-r--r--   0 qzhao     (1001) users      (100)     1289 2023-04-23 06:39:33.000000 f5-openstack-lbaasv2-inventory-1.0.1/neutron_lbaas_inventory/db/models/inventory.py
+-rw-r--r--   0 qzhao     (1001) users      (100)        0 2023-03-30 07:52:56.000000 f5-openstack-lbaasv2-inventory-1.0.1/neutron_lbaas_inventory/db/models/__init__.py
+drwxr-xr-x   0 qzhao     (1001) users      (100)        0 2023-04-23 06:51:43.000000 f5-openstack-lbaasv2-inventory-1.0.1/neutron_lbaas_inventory/db/migration/
+drwxr-xr-x   0 qzhao     (1001) users      (100)        0 2023-04-23 06:51:43.000000 f5-openstack-lbaasv2-inventory-1.0.1/neutron_lbaas_inventory/db/migration/alembic_migrations/
+-rw-r--r--   0 qzhao     (1001) users      (100)     1483 2023-04-23 06:39:33.000000 f5-openstack-lbaasv2-inventory-1.0.1/neutron_lbaas_inventory/db/migration/alembic_migrations/inventory_init_ops.py
+-rw-r--r--   0 qzhao     (1001) users      (100)     2076 2023-03-30 07:52:56.000000 f5-openstack-lbaasv2-inventory-1.0.1/neutron_lbaas_inventory/db/migration/alembic_migrations/env.py
+-rw-r--r--   0 qzhao     (1001) users      (100)        0 2023-03-30 07:52:56.000000 f5-openstack-lbaasv2-inventory-1.0.1/neutron_lbaas_inventory/db/migration/alembic_migrations/__init__.py
+drwxr-xr-x   0 qzhao     (1001) users      (100)        0 2023-04-23 06:51:43.000000 f5-openstack-lbaasv2-inventory-1.0.1/neutron_lbaas_inventory/db/migration/alembic_migrations/versions/
+-rw-r--r--   0 qzhao     (1001) users      (100)        0 2023-03-30 07:52:56.000000 f5-openstack-lbaasv2-inventory-1.0.1/neutron_lbaas_inventory/db/migration/alembic_migrations/versions/__init__.py
+-rw-r--r--   0 qzhao     (1001) users      (100)      281 2023-03-30 07:52:56.000000 f5-openstack-lbaasv2-inventory-1.0.1/neutron_lbaas_inventory/db/migration/alembic_migrations/versions/pike_initial.py
+-rw-r--r--   0 qzhao     (1001) users      (100)        0 2023-03-30 07:52:56.000000 f5-openstack-lbaasv2-inventory-1.0.1/neutron_lbaas_inventory/db/migration/__init__.py
+-rw-r--r--   0 qzhao     (1001) users      (100)        0 2023-03-30 07:52:56.000000 f5-openstack-lbaasv2-inventory-1.0.1/neutron_lbaas_inventory/db/__init__.py
+-rw-r--r--   0 qzhao     (1001) users      (100)     9972 2023-04-23 06:39:33.000000 f5-openstack-lbaasv2-inventory-1.0.1/neutron_lbaas_inventory/db/inventory_db.py
+-rw-r--r--   0 qzhao     (1001) users      (100)       22 2023-04-23 06:51:22.000000 f5-openstack-lbaasv2-inventory-1.0.1/neutron_lbaas_inventory/__init__.py
+-rw-r--r--   0 qzhao     (1001) users      (100)     1239 2023-03-30 07:52:56.000000 f5-openstack-lbaasv2-inventory-1.0.1/setup.py
+-rw-r--r--   0 qzhao     (1001) users      (100)       38 2023-04-23 06:51:43.000000 f5-openstack-lbaasv2-inventory-1.0.1/setup.cfg
+drwxr-xr-x   0 qzhao     (1001) users      (100)        0 2023-04-23 06:51:43.000000 f5-openstack-lbaasv2-inventory-1.0.1/f5_openstack_lbaasv2_inventory.egg-info/
+-rw-r--r--   0 qzhao     (1001) users      (100)      680 2023-04-23 06:51:43.000000 f5-openstack-lbaasv2-inventory-1.0.1/f5_openstack_lbaasv2_inventory.egg-info/PKG-INFO
+-rw-r--r--   0 qzhao     (1001) users      (100)      219 2023-04-23 06:51:43.000000 f5-openstack-lbaasv2-inventory-1.0.1/f5_openstack_lbaasv2_inventory.egg-info/entry_points.txt
+-rw-r--r--   0 qzhao     (1001) users      (100)     1331 2023-04-23 06:51:43.000000 f5-openstack-lbaasv2-inventory-1.0.1/f5_openstack_lbaasv2_inventory.egg-info/SOURCES.txt
+-rw-r--r--   0 qzhao     (1001) users      (100)       24 2023-04-23 06:51:43.000000 f5-openstack-lbaasv2-inventory-1.0.1/f5_openstack_lbaasv2_inventory.egg-info/top_level.txt
+-rw-r--r--   0 qzhao     (1001) users      (100)        1 2023-04-23 06:51:43.000000 f5-openstack-lbaasv2-inventory-1.0.1/f5_openstack_lbaasv2_inventory.egg-info/dependency_links.txt
```

### Comparing `f5-openstack-lbaasv2-inventory-1.0.0/PKG-INFO` & `f5-openstack-lbaasv2-inventory-1.0.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: f5-openstack-lbaasv2-inventory
-Version: 1.0.0
+Version: 1.0.1
 Summary: F5 Networks device inventory for OpenStack services
 Home-page: UNKNOWN
 Author: F5 Networks
 Author-email: openstack@f5.com
 License: Apache License, Version 2.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `f5-openstack-lbaasv2-inventory-1.0.0/README.md` & `f5-openstack-lbaasv2-inventory-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `f5-openstack-lbaasv2-inventory-1.0.0/neutron_lbaas_inventory/plugins/lbaasdevice.py` & `f5-openstack-lbaasv2-inventory-1.0.1/neutron_lbaas_inventory/plugins/lbaasdevice.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,46 +1,68 @@
 from oslo_log import log
 
 from neutron_lbaas_inventory.db.inventory_db import InventoryDbPlugin
-from neutron_lbaas_inventory.db.lb_device_binding_db \
-    import LbDeviceBindingDbPlugin
 from neutron_lbaas_inventory.extensions import lbaasdevice
 
 LOG = log.getLogger(__name__)
 
 
 class LbaasDevicePlugin(lbaasdevice.LbaasDevicePluginBase):
-
     supported_extension_aliases = ["lbaas-device"]
-    device_db = InventoryDbPlugin()
-    lb_device_db = LbDeviceBindingDbPlugin()
+    inventory_db = InventoryDbPlugin()
 
     def get_devices(self, context, filters=None, fields=None,
                     sorts=None, limit=None, marker=None,
                     page_reverse=False):
         LOG.debug("List lbaas devices")
-        devices = self.device_db.get_devices(context, filters=filters)
+        devices = self.inventory_db.get_devices(context, filters=filters)
         return devices
 
     def get_device(self, context, id, fields=None):
         LOG.debug("Get a lbaas device, id: {}".format(id))
-        return self.device_db.get_device(context, id)
+        return self.inventory_db.get_device(context, id)
 
     def create_device(self, context, device):
         LOG.debug("Create lbaas device, device_info: {}".format(device))
-        return self.device_db.create_device(context, device)
+        return self.inventory_db.create_device(context, device)
 
     def delete_device(self, context, id):
         LOG.debug("Delete lbaas device, id: {}".format(id))
-        self.device_db.delete_device(context, id)
+        self.inventory_db.delete_device(context, id)
 
     def update_device(self, context, id, device):
         LOG.debug("Update lbaas device, id: {}, device: {}".format(id, device))
-        return self.device_db.update_device(context, id, device)
+        return self.inventory_db.update_device(context, id, device)
 
     def get_loadbalanceragentbindings(self, context, filters=None, fields=None,
                                       sorts=None, limit=None, marker=None,
                                       page_reverse=False):
         LOG.debug("List loadbalancer device bindings")
-        lb_device_bindings = self.lb_device_db.get_bindings(context,
+        lb_device_bindings = self.inventory_db.get_bindings(context,
                                                             filters=filters)
         return lb_device_bindings
+
+    def get_device_members(self, context, device_id, filters=None,
+                           fields=None):
+        LOG.debug("Get lbaas device members, device_id: {}".format(device_id))
+        filters['device_id'] = [device_id]
+        return self.inventory_db.get_members(context, filters=filters)
+
+    def get_device_member(self, context, id, device_id, fields=None):
+        LOG.debug("Get lbaas device member, device_id: {}, id: {}"
+                  .format(device_id, id))
+        return self.inventory_db.get_member(context, id)
+
+    def create_device_member(self, context, device_id, member):
+        LOG.debug("Create lbaas device member, device_id: {}, member: {}"
+                  .format(device_id, member))
+        return self.inventory_db.create_member(context, device_id, member)
+
+    def update_device_member(self, context, id, device_id, member):
+        LOG.debug("Update lbaas device member, device_id: {}, id: {}"
+                  .format(device_id, id))
+        return self.inventory_db.update_member(context, id, member)
+
+    def delete_device_member(self, context, id, device_id):
+        LOG.debug("Delete lbaas device member, device_id: {}, id: {}"
+                  .format(device_id, id))
+        self.inventory_db.delete_member(context, id)
```

### Comparing `f5-openstack-lbaasv2-inventory-1.0.0/neutron_lbaas_inventory/extensions/lbaasdevice.py` & `f5-openstack-lbaasv2-inventory-1.0.1/neutron_lbaas_inventory/extensions/lbaasdevice.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,16 +2,19 @@
 import six
 
 from neutron.api import extensions as neutron_extensions
 from neutron.api.v2 import resource_helper
 from neutron_lib.api import converters
 from neutron_lib.api import extensions as api_extensions
 from neutron_lib.db import constants as db_const
+from neutron_lib.plugins import directory
 from neutron_lib.services import base as service_base
 from oslo_log import log as logging
+from neutron.api import extensions
+from neutron.api.v2 import base
 
 from neutron_lbaas_inventory import extensions as device_extensions
 from neutron_lbaas_inventory.common import constants
 
 # Ensure the extension is loaded at startup
 neutron_extensions.append_api_extensions_path(device_extensions.__path__)
 
@@ -31,46 +34,73 @@
                         'validate': {
                             'type:string': db_const.DESCRIPTION_FIELD_SIZE},
                         'is_visible': True, 'default': ''},
         'project_id': {'allow_post': True, 'allow_put': False,
                        'validate': {
                            'type:string': db_const.PROJECT_ID_FIELD_SIZE},
                        'is_visible': True},
-        'type': {'allow_post': True, 'allow_put': True,
-                 'is_visible': True},
         'shared': {'allow_post': True, 'allow_put': True,
                    'default': True,
                    'convert_to': converters.convert_to_boolean,
                    'is_visible': True},
         'admin_state_up': {'allow_post': True, 'allow_put': True,
                            'default': True,
                            'convert_to': converters.convert_to_boolean,
                            'is_visible': True},
         'availability_zone': {'allow_post': True, 'allow_put': True,
                               'is_visible': True},
-        'provisioning_status': {'allow_post': False, 'allow_put': False,
-                                'is_visible': True},
-        'operating_status': {'allow_post': False, 'allow_put': False,
-                             'is_visible': True},
         'device_info': {'allow_post': True, 'allow_put': True,
                         'is_visible': True},
-        'last_error': {'allow_post': False, 'allow_put': False,
-                       'is_visible': True}
+        'provisioning_status': {'allow_post': False, 'allow_put': True,
+                                'is_visible': True},
     },
     'loadbalanceragentbindings': {
         'loadbalancer_id': {'allow_post': False, 'allow_put': False,
                             'validate': {'type:uuid': None},
                             'is_visible': True,
                             'primary_key': True},
         'agent_id': {'allow_post': False, 'allow_put': False,
                      'validate': {'type:uuid': None},
                      'is_visible': True},
         'device_id': {'allow_post': False, 'allow_put': False,
                       'validate': {'type:uuid': None},
                       'is_visible': True},
+    },
+}
+
+SUB_RESOURCE_ATTRIBUTE_MAP = {
+    'members': {
+        'parent': {'collection_name': 'devices',
+                   'member_name': 'device'},
+        'parameters': {
+            'id': {'allow_post': False, 'allow_put': False,
+                   'validate': {'type:uuid': None},
+                   'is_visible': True,
+                   'primary_key': True},
+            'device_id': {'allow_post': False, 'allow_put': False,
+                          'validate': {'type:uuid': None},
+                          'is_visible': True},
+            'tenant_id': {'allow_post': True, 'allow_put': False,
+                          'validate': {'type:not_empty_string':
+                                       db_const.PROJECT_ID_FIELD_SIZE},
+                          'required_by_policy': True,
+                          'is_visible': True},
+            'type': {'allow_post': True, 'allow_put': True,
+                     'is_visible': True},
+            'mgmt_ipv4': {'allow_post': True, 'allow_put': False,
+                          'is_visible': True},
+            'mgmt_ipv6': {'allow_post': True, 'allow_put': False,
+                          'is_visible': True},
+            'device_info': {'allow_post': True, 'allow_put': True,
+                            'is_visible': True},
+            'operating_status': {'allow_post': True, 'allow_put': True,
+                                 'is_visible': True},
+            'last_error': {'allow_post': False, 'allow_put': True,
+                           'is_visible': True}
+        }
     }
 }
 
 
 class Lbaasdevice(api_extensions.ExtensionDescriptor):
     """API extension for handling lbaas device."""
 
@@ -96,14 +126,34 @@
         plural_mappings = resource_helper.build_plural_mappings(
             {}, RESOURCE_ATTRIBUTE_MAP)
         resources = resource_helper.build_resource_info(
             plural_mappings,
             RESOURCE_ATTRIBUTE_MAP,
             constants.LBAAS_DEVICE,
             register_quota=False)
+        plugin = directory.get_plugin(constants.LBAAS_DEVICE)
+        for collection_name in SUB_RESOURCE_ATTRIBUTE_MAP:
+            # Special handling needed for sub-resources with 'y' ending
+            # (e.g. proxies -> proxy)
+            resource_name = collection_name[:-1]
+            parent = SUB_RESOURCE_ATTRIBUTE_MAP[collection_name].get('parent')
+            params = SUB_RESOURCE_ATTRIBUTE_MAP[collection_name].get(
+                'parameters')
+            controller = base.create_resource(collection_name, resource_name,
+                                              plugin, params,
+                                              allow_bulk=True,
+                                              parent=parent,
+                                              allow_pagination=True,
+                                              allow_sorting=True)
+            resource = extensions.ResourceExtension(
+                collection_name,
+                controller, parent,
+                path_prefix=constants.LBAAS_DEVICE_PREFIX,
+                attr_map=params)
+            resources.append(resource)
         return resources
 
     @classmethod
     def get_plugin_interface(cls):
         return LbaasDevicePluginBase
 
     def get_extended_resources(self, version):
@@ -144,11 +194,33 @@
     def delete_device(self, context, id):
         pass
 
     @abc.abstractmethod
     def update_device(self, context, id, device):
         pass
 
+    @abc.abstractmethod
     def get_loadbalanceragentbindings(self, context, filters=None, fields=None,
                                       sorts=None, limit=None, marker=None,
                                       page_reverse=False):
         pass
+
+    @abc.abstractmethod
+    def get_device_members(self, context, device_id, filters=None,
+                           fields=None):
+        pass
+
+    @abc.abstractmethod
+    def get_device_member(self, context, id, device_id, fields=None):
+        pass
+
+    @abc.abstractmethod
+    def create_device_member(self, context, device_id, member):
+        pass
+
+    @abc.abstractmethod
+    def update_device_member(self, context, id, device_id, member):
+        pass
+
+    @abc.abstractmethod
+    def delete_device_member(self, context, id, device_id):
+        pass
```

### Comparing `f5-openstack-lbaasv2-inventory-1.0.0/neutron_lbaas_inventory/db/migration/alembic_migrations/inventory_init_ops.py` & `f5-openstack-lbaasv2-inventory-1.0.1/neutron_lbaas_inventory/db/migration/alembic_migrations/inventory_init_ops.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,17 +7,28 @@
 def upgrade():
     op.create_table(
         u'lbaas_devices',
         sa.Column(u'project_id', sa.String(255), nullable=True),
         sa.Column(u'id', sa.String(36), nullable=False),
         sa.Column(u'name', sa.String(255), nullable=True),
         sa.Column(u'description', sa.String(255), nullable=True),
-        sa.Column(u'type', sa.String(16), nullable=False),
         sa.Column(u'shared', sa.Boolean(), nullable=False),
         sa.Column(u'admin_state_up', sa.Boolean(), nullable=False),
         sa.Column(u'availability_zone', sa.String(255), nullable=True),
+        sa.Column(u'device_info', sa.String(4095), nullable=False),
         sa.Column(u'provisioning_status', sa.String(255), nullable=True),
+        sa.PrimaryKeyConstraint(u'id')
+    )
+
+    op.create_table(
+        u'lbaas_device_members',
+        sa.Column(u'id', sa.String(36), nullable=False),
+        sa.Column(u'device_id', sa.String(36), nullable=False),
+        sa.Column(u'type', sa.String(16), nullable=False),
+        sa.Column(u'mgmt_ipv4', sa.String(255), nullable=False),
+        sa.Column(u'mgmt_ipv6', sa.String(255), nullable=True),
+        sa.Column(u'device_info', sa.String(4095), nullable=False),
         sa.Column(u'operating_status', sa.String(255), nullable=True),
-        sa.Column(u'device_info', sa.String(4095), nullable=True),
         sa.Column(u'last_error', sa.String(4095), nullable=True),
-        sa.PrimaryKeyConstraint(u'id')
+        sa.PrimaryKeyConstraint(u'id'),
+        sa.ForeignKeyConstraint([u'device_id'], [u'lbaas_devices.id']),
     )
```

### Comparing `f5-openstack-lbaasv2-inventory-1.0.0/neutron_lbaas_inventory/db/migration/alembic_migrations/env.py` & `f5-openstack-lbaasv2-inventory-1.0.1/neutron_lbaas_inventory/db/migration/alembic_migrations/env.py`

 * *Files identical despite different names*

### Comparing `f5-openstack-lbaasv2-inventory-1.0.0/setup.py` & `f5-openstack-lbaasv2-inventory-1.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `f5-openstack-lbaasv2-inventory-1.0.0/f5_openstack_lbaasv2_inventory.egg-info/PKG-INFO` & `f5-openstack-lbaasv2-inventory-1.0.1/f5_openstack_lbaasv2_inventory.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: f5-openstack-lbaasv2-inventory
-Version: 1.0.0
+Version: 1.0.1
 Summary: F5 Networks device inventory for OpenStack services
 Home-page: UNKNOWN
 Author: F5 Networks
 Author-email: openstack@f5.com
 License: Apache License, Version 2.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `f5-openstack-lbaasv2-inventory-1.0.0/f5_openstack_lbaasv2_inventory.egg-info/SOURCES.txt` & `f5-openstack-lbaasv2-inventory-1.0.1/f5_openstack_lbaasv2_inventory.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 f5_openstack_lbaasv2_inventory.egg-info/top_level.txt
 neutron_lbaas_inventory/__init__.py
 neutron_lbaas_inventory/common/__init__.py
 neutron_lbaas_inventory/common/constants.py
 neutron_lbaas_inventory/common/exceptions.py
 neutron_lbaas_inventory/db/__init__.py
 neutron_lbaas_inventory/db/inventory_db.py
-neutron_lbaas_inventory/db/lb_device_binding_db.py
 neutron_lbaas_inventory/db/migration/__init__.py
 neutron_lbaas_inventory/db/migration/alembic_migrations/__init__.py
 neutron_lbaas_inventory/db/migration/alembic_migrations/env.py
 neutron_lbaas_inventory/db/migration/alembic_migrations/inventory_init_ops.py
 neutron_lbaas_inventory/db/migration/alembic_migrations/versions/__init__.py
 neutron_lbaas_inventory/db/migration/alembic_migrations/versions/pike_initial.py
 neutron_lbaas_inventory/db/models/__init__.py
```

