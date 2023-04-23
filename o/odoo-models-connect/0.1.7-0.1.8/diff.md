# Comparing `tmp/odoo_models_connect-0.1.7.tar.gz` & `tmp/odoo_models_connect-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odoo_models_connect-0.1.7.tar", last modified: Tue Apr 18 21:28:04 2023, max compression
+gzip compressed data, was "odoo_models_connect-0.1.8.tar", last modified: Wed Apr 19 14:04:03 2023, max compression
```

## Comparing `odoo_models_connect-0.1.7.tar` & `odoo_models_connect-0.1.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 lsvtech2022   (501) staff       (20)        0 2023-04-18 21:28:04.814430 odoo_models_connect-0.1.7/
--rw-r--r--   0 lsvtech2022   (501) staff       (20)     4797 2023-04-18 21:28:04.813904 odoo_models_connect-0.1.7/PKG-INFO
--rw-r--r--   0 lsvtech2022   (501) staff       (20)     4429 2023-04-18 21:27:49.000000 odoo_models_connect-0.1.7/README.md
-drwxr-xr-x   0 lsvtech2022   (501) staff       (20)        0 2023-04-18 21:28:04.809363 odoo_models_connect-0.1.7/odoo_models_connect/
--rw-r--r--   0 lsvtech2022   (501) staff       (20)       72 2023-04-17 14:13:42.000000 odoo_models_connect-0.1.7/odoo_models_connect/__init__.py
--rw-r--r--   0 lsvtech2022   (501) staff       (20)     5738 2023-04-11 18:31:41.000000 odoo_models_connect-0.1.7/odoo_models_connect/connect_odoo.py
--rw-r--r--   0 lsvtech2022   (501) staff       (20)      648 2023-04-12 11:53:38.000000 odoo_models_connect-0.1.7/odoo_models_connect/fields.py
--rw-r--r--   0 lsvtech2022   (501) staff       (20)     4080 2023-04-18 19:29:41.000000 odoo_models_connect-0.1.7/odoo_models_connect/models.py
-drwxr-xr-x   0 lsvtech2022   (501) staff       (20)        0 2023-04-18 21:28:04.812727 odoo_models_connect-0.1.7/odoo_models_connect.egg-info/
--rw-r--r--   0 lsvtech2022   (501) staff       (20)     4797 2023-04-18 21:28:04.000000 odoo_models_connect-0.1.7/odoo_models_connect.egg-info/PKG-INFO
--rw-r--r--   0 lsvtech2022   (501) staff       (20)      360 2023-04-18 21:28:04.000000 odoo_models_connect-0.1.7/odoo_models_connect.egg-info/SOURCES.txt
--rw-r--r--   0 lsvtech2022   (501) staff       (20)        1 2023-04-18 21:28:04.000000 odoo_models_connect-0.1.7/odoo_models_connect.egg-info/dependency_links.txt
--rw-r--r--   0 lsvtech2022   (501) staff       (20)       21 2023-04-18 21:28:04.000000 odoo_models_connect-0.1.7/odoo_models_connect.egg-info/requires.txt
--rw-r--r--   0 lsvtech2022   (501) staff       (20)       20 2023-04-18 21:28:04.000000 odoo_models_connect-0.1.7/odoo_models_connect.egg-info/top_level.txt
--rw-r--r--   0 lsvtech2022   (501) staff       (20)       38 2023-04-18 21:28:04.814629 odoo_models_connect-0.1.7/setup.cfg
--rw-r--r--   0 lsvtech2022   (501) staff       (20)     1415 2023-04-18 21:27:56.000000 odoo_models_connect-0.1.7/setup.py
+drwxr-xr-x   0 lsvtech2022   (501) staff       (20)        0 2023-04-19 14:04:03.543528 odoo_models_connect-0.1.8/
+-rw-r--r--   0 lsvtech2022   (501) staff       (20)     4797 2023-04-19 14:04:03.542008 odoo_models_connect-0.1.8/PKG-INFO
+-rw-r--r--   0 lsvtech2022   (501) staff       (20)     4429 2023-04-18 21:27:49.000000 odoo_models_connect-0.1.8/README.md
+drwxr-xr-x   0 lsvtech2022   (501) staff       (20)        0 2023-04-19 14:04:03.531728 odoo_models_connect-0.1.8/odoo_models_connect/
+-rw-r--r--   0 lsvtech2022   (501) staff       (20)       72 2023-04-17 14:13:42.000000 odoo_models_connect-0.1.8/odoo_models_connect/__init__.py
+-rw-r--r--   0 lsvtech2022   (501) staff       (20)     5738 2023-04-11 18:31:41.000000 odoo_models_connect-0.1.8/odoo_models_connect/connect_odoo.py
+-rw-r--r--   0 lsvtech2022   (501) staff       (20)      648 2023-04-12 11:53:38.000000 odoo_models_connect-0.1.8/odoo_models_connect/fields.py
+-rw-r--r--   0 lsvtech2022   (501) staff       (20)     4124 2023-04-19 14:02:19.000000 odoo_models_connect-0.1.8/odoo_models_connect/models.py
+drwxr-xr-x   0 lsvtech2022   (501) staff       (20)        0 2023-04-19 14:04:03.539325 odoo_models_connect-0.1.8/odoo_models_connect.egg-info/
+-rw-r--r--   0 lsvtech2022   (501) staff       (20)     4797 2023-04-19 14:04:03.000000 odoo_models_connect-0.1.8/odoo_models_connect.egg-info/PKG-INFO
+-rw-r--r--   0 lsvtech2022   (501) staff       (20)      360 2023-04-19 14:04:03.000000 odoo_models_connect-0.1.8/odoo_models_connect.egg-info/SOURCES.txt
+-rw-r--r--   0 lsvtech2022   (501) staff       (20)        1 2023-04-19 14:04:03.000000 odoo_models_connect-0.1.8/odoo_models_connect.egg-info/dependency_links.txt
+-rw-r--r--   0 lsvtech2022   (501) staff       (20)       21 2023-04-19 14:04:03.000000 odoo_models_connect-0.1.8/odoo_models_connect.egg-info/requires.txt
+-rw-r--r--   0 lsvtech2022   (501) staff       (20)       20 2023-04-19 14:04:03.000000 odoo_models_connect-0.1.8/odoo_models_connect.egg-info/top_level.txt
+-rw-r--r--   0 lsvtech2022   (501) staff       (20)       38 2023-04-19 14:04:03.544533 odoo_models_connect-0.1.8/setup.cfg
+-rw-r--r--   0 lsvtech2022   (501) staff       (20)     1415 2023-04-19 14:03:50.000000 odoo_models_connect-0.1.8/setup.py
```

### Comparing `odoo_models_connect-0.1.7/PKG-INFO` & `odoo_models_connect-0.1.8/odoo_models_connect.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: odoo_models_connect
-Version: 0.1.7
+Name: odoo-models-connect
+Version: 0.1.8
 Summary: Library to improve interaction and communication with odoo for integration with other technologies.
 Home-page: https://github.com/DeijoseDevelop/odoo_models_connect
 Author: Deiver Jose Vazquez Moreno
 Author-email: estudiandovazmore@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
```

### Comparing `odoo_models_connect-0.1.7/README.md` & `odoo_models_connect-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `odoo_models_connect-0.1.7/odoo_models_connect/connect_odoo.py` & `odoo_models_connect-0.1.8/odoo_models_connect/connect_odoo.py`

 * *Files identical despite different names*

### Comparing `odoo_models_connect-0.1.7/odoo_models_connect/fields.py` & `odoo_models_connect-0.1.8/odoo_models_connect/fields.py`

 * *Files identical despite different names*

### Comparing `odoo_models_connect-0.1.7/odoo_models_connect/models.py` & `odoo_models_connect-0.1.8/odoo_models_connect/models.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,56 +10,56 @@
 def load_env_vars(env_path):
     if not os.path.exists(env_path):
         raise FileNotFoundError(".env not found, wrong path")
     load_dotenv(env_path)
 
 
 class OdooModel(object):
-    DATABASE = None
-    USERNAME = None
-    PASSWORD = None
-    URL = None
-    UUID = None
-    MODELS = None
+    _DATABASE = None
+    _USERNAME = None
+    _PASSWORD = None
+    _URL = None
+    _UUID = None
+    _MODELS = None
 
-    COMMON = '/xmlrpc/2/common'
-    OBJECTS = '/xmlrpc/2/object'
+    _COMMON = '/xmlrpc/2/common'
+    _OBJECTS = '/xmlrpc/2/object'
 
-    FIELDS = {}
+    _FIELDS = {}
 
     _name = None
     id = None
 
     def __init__(self, **kwargs):
         if kwargs:
             for name, value in kwargs.items():
                 setattr(self, name, value)
-                self.FIELDS[name] = value
+                self._FIELDS[name] = value
 
     def __repr__(self):
         return f"<{self.__class__.__name__} id={self.id}>"
 
     class DoesNotExist(Exception):
 
         def __init__(self, obj_id):
             self.id = obj_id
 
         def __str__(self):
             return f'Element by id {self.id} does not exist'
 
     @classmethod
     def search_read(cls, query=[], **kwargs):
-        records = cls.MODELS.execute_kw(
-            cls.DATABASE,
-            cls.UUID,
-            cls.PASSWORD,
+        records = cls._MODELS.execute_kw(
+            cls._DATABASE,
+            cls._UUID,
+            cls._PASSWORD,
             cls._name,
             'search_read',
             [query],
-            {'fields': list(cls.FIELDS.keys())}
+            {'fields': list(cls._FIELDS.keys())}
         )
         instances = cls._instances_from_list(records)
         return instances
 
     @classmethod
     def search_count(cls, query=[]):
         records = cls.search_read(query=query)
@@ -79,64 +79,64 @@
         return [cls._create_instance_from_dict(record) for record in records]
 
     @classmethod
     def _create_instance_from_dict(cls, obj):
         return cls(**obj)
 
     def create(self):
-        return self.MODELS.execute_kw(self.DATABASE, self.UUID, self.PASSWORD, self._name, 'create', [self.FIELDS])
+        return self._MODELS.execute_kw(self._DATABASE, self._UUID, self._PASSWORD, self._name, 'create', [self._FIELDS])
 
     def update(self):
-        return self.MODELS.execute_kw(self.DATABASE, self.UUID, self.PASSWORD, self._name, 'write', [[self.id], self.FIELDS])
+        return self._MODELS.execute_kw(self._DATABASE, self._UUID, self._PASSWORD, self._name, 'write', [[self.id], self._FIELDS])
 
     def delete(self):
-        return self.MODELS.execute_kw(self.DATABASE, self.UUID, self.PASSWORD, self._name, 'unlink', [[self.id]])
+        return self._MODELS.execute_kw(self._DATABASE, self._UUID, self._PASSWORD, self._name, 'unlink', [[self.id]])
 
     def __init_subclass__(cls):
         cls._set_config_envs()
         cls._fill_fields()
         cls._set_attributes_initialized_none()
         super().__init_subclass__()
 
     @classmethod
     def _set_attributes_initialized_none(cls):
         cls._set_models_attribute()
         cls._set_uuid_attribute()
 
     @classmethod
     def _set_config_envs(cls):
-        cls.DATABASE = os.getenv('DATABASE')
-        cls.USERNAME = os.getenv('USERNAME')
-        cls.PASSWORD = os.getenv('PASSWORD')
-        cls.URL = os.getenv('URL')
+        cls._DATABASE = os.getenv('DATABASE')
+        cls._USERNAME = os.getenv('USERNAME')
+        cls._PASSWORD = os.getenv('PASSWORD')
+        cls._URL = os.getenv('URL')
 
     @classmethod
     def _set_uuid_attribute(cls):
-        common = xmlrpc.client.ServerProxy('{}{}'.format(cls.URL, cls.COMMON))
-        cls.UUID = common.authenticate(
-            cls.DATABASE, cls.USERNAME, cls.PASSWORD, {})
+        common = xmlrpc.client.ServerProxy('{}{}'.format(cls._URL, cls._COMMON))
+        cls._UUID = common.authenticate(
+            cls._DATABASE, cls._USERNAME, cls._PASSWORD, {})
 
     @classmethod
     def _set_models_attribute(cls):
-        cls.MODELS = xmlrpc.client.ServerProxy(
-            '{}{}'.format(cls.URL, cls.OBJECTS))
+        cls._MODELS = xmlrpc.client.ServerProxy(
+            '{}{}'.format(cls._URL, cls._OBJECTS))
 
     @classmethod
     def _fill_fields(cls):
-        cls.FIELDS = {}
+        cls._FIELDS = {}
         cls._iterate_dir_class()
 
     @classmethod
     def _iterate_dir_class(cls):
         for attr_name in dir(cls):
             attr = cls._is_not_abstract_method_attribute(attr_name)
             cls._add_field_if_is_odoo_field(attr, attr_name)
 
     @classmethod
     def _add_field_if_is_odoo_field(cls, attr, attr_name):
         if isinstance(attr, OdooField):
-            cls.FIELDS[attr_name] = attr._type
+            cls._FIELDS[attr_name] = attr._type
 
     @classmethod
     def _is_not_abstract_method_attribute(cls, attr_name):
         if attr_name != '__abstractmethods__':
             return getattr(cls, attr_name)
```

### Comparing `odoo_models_connect-0.1.7/odoo_models_connect.egg-info/PKG-INFO` & `odoo_models_connect-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: odoo-models-connect
-Version: 0.1.7
+Name: odoo_models_connect
+Version: 0.1.8
 Summary: Library to improve interaction and communication with odoo for integration with other technologies.
 Home-page: https://github.com/DeijoseDevelop/odoo_models_connect
 Author: Deiver Jose Vazquez Moreno
 Author-email: estudiandovazmore@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
```

### Comparing `odoo_models_connect-0.1.7/setup.py` & `odoo_models_connect-0.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pathlib
 from setuptools import find_packages, setup
 
 HERE = pathlib.Path(__file__).parent
 
-VERSION = '0.1.7'  # Muy importante, deberéis ir cambiando la versión de vuestra librería según incluyáis nuevas funcionalidades
+VERSION = '0.1.8'  # Muy importante, deberéis ir cambiando la versión de vuestra librería según incluyáis nuevas funcionalidades
 # Debe coincidir con el nombre de la carpeta
 PACKAGE_NAME = 'odoo_models_connect'
 AUTHOR = 'Deiver Jose Vazquez Moreno'  # Modificar con vuestros datos
 AUTHOR_EMAIL = 'estudiandovazmore@gmail.com'  # Modificar con vuestros datos
 # Modificar con vuestros datos
 URL = 'https://github.com/DeijoseDevelop/odoo_models_connect'
```

