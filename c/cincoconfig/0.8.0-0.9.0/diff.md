# Comparing `tmp/cincoconfig-0.8.0.tar.gz` & `tmp/cincoconfig-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\cincoconfig-0.8.0.tar", last modified: Sat Jul 17 14:36:56 2021, max compression
+gzip compressed data, was "cincoconfig-0.9.0.tar", max compression
```

## Comparing `cincoconfig-0.8.0.tar` & `cincoconfig-0.9.0.tar`

### file list

```diff
@@ -1,47 +1,76 @@
-drwxrwxrwx   0        0        0        0 2021-07-17 14:36:56.000000 cincoconfig-0.8.0/
--rw-rw-rw-   0        0        0    17691 2021-07-17 14:22:19.000000 cincoconfig-0.8.0/.pylintrc
--rw-rw-rw-   0        0        0      772 2019-06-26 21:17:11.000000 cincoconfig-0.8.0/LICENSE
--rw-rw-rw-   0        0        0       71 2019-06-26 21:17:11.000000 cincoconfig-0.8.0/MANIFEST.in
--rw-rw-rw-   0        0        0     6257 2021-07-17 14:36:56.000000 cincoconfig-0.8.0/PKG-INFO
--rw-rw-rw-   0        0        0     4134 2021-07-17 14:32:38.000000 cincoconfig-0.8.0/README.md
-drwxrwxrwx   0        0        0        0 2021-07-17 14:36:56.000000 cincoconfig-0.8.0/cincoconfig/
--rw-rw-rw-   0        0        0      642 2021-07-17 14:22:19.000000 cincoconfig-0.8.0/cincoconfig/__init__.py
--rw-rw-rw-   0        0        0    50508 2021-07-17 14:22:19.000000 cincoconfig-0.8.0/cincoconfig/core.py
--rw-rw-rw-   0        0        0     8763 2021-07-17 14:22:19.000000 cincoconfig-0.8.0/cincoconfig/encryption.py
-drwxrwxrwx   0        0        0        0 2021-07-17 14:36:56.000000 cincoconfig-0.8.0/cincoconfig/fields/
--rw-rw-rw-   0        0        0     1353 2021-07-17 14:22:19.000000 cincoconfig-0.8.0/cincoconfig/fields/__init__.py
--rw-rw-rw-   0        0        0     1589 2021-07-17 14:22:19.000000 cincoconfig-0.8.0/cincoconfig/fields/bool_field.py
--rw-rw-rw-   0        0        0     2338 2021-07-17 14:22:19.000000 cincoconfig-0.8.0/cincoconfig/fields/bytes_field.py
--rw-rw-rw-   0        0        0      984 2021-07-17 14:22:19.000000 cincoconfig-0.8.0/cincoconfig/fields/dict_field.py
--rw-rw-rw-   0        0        0     2707 2021-07-17 14:22:19.000000 cincoconfig-0.8.0/cincoconfig/fields/file_field.py
--rw-rw-rw-   0        0        0     3313 2021-07-17 14:22:19.000000 cincoconfig-0.8.0/cincoconfig/fields/include_field.py
--rw-rw-rw-   0        0        0     2344 2021-07-17 14:22:19.000000 cincoconfig-0.8.0/cincoconfig/fields/instance_method_field.py
--rw-rw-rw-   0        0        0     6853 2021-07-17 14:22:19.000000 cincoconfig-0.8.0/cincoconfig/fields/list_field.py
--rw-rw-rw-   0        0        0     4223 2021-07-17 14:22:19.000000 cincoconfig-0.8.0/cincoconfig/fields/net_field.py
--rw-rw-rw-   0        0        0     2344 2021-07-17 14:22:19.000000 cincoconfig-0.8.0/cincoconfig/fields/number_field.py
--rw-rw-rw-   0        0        0    11512 2021-07-17 14:22:19.000000 cincoconfig-0.8.0/cincoconfig/fields/secure_field.py
--rw-rw-rw-   0        0        0     5954 2021-07-17 14:22:19.000000 cincoconfig-0.8.0/cincoconfig/fields/string_field.py
--rw-rw-rw-   0        0        0      938 2021-07-17 14:22:19.000000 cincoconfig-0.8.0/cincoconfig/fields/url_field.py
--rw-rw-rw-   0        0        0     1489 2021-07-17 14:22:19.000000 cincoconfig-0.8.0/cincoconfig/fields/virtual_field.py
-drwxrwxrwx   0        0        0        0 2021-07-17 14:36:56.000000 cincoconfig-0.8.0/cincoconfig/formats/
--rw-rw-rw-   0        0        0      862 2021-07-17 14:22:19.000000 cincoconfig-0.8.0/cincoconfig/formats/__init__.py
--rw-rw-rw-   0        0        0     1645 2021-07-17 14:22:19.000000 cincoconfig-0.8.0/cincoconfig/formats/bson.py
--rw-rw-rw-   0        0        0     1569 2021-07-17 14:22:19.000000 cincoconfig-0.8.0/cincoconfig/formats/json.py
--rw-rw-rw-   0        0        0     1480 2021-07-17 14:22:19.000000 cincoconfig-0.8.0/cincoconfig/formats/pickle.py
--rw-rw-rw-   0        0        0     6310 2021-07-17 14:22:19.000000 cincoconfig-0.8.0/cincoconfig/formats/xml.py
--rw-rw-rw-   0        0        0     3340 2021-07-17 14:22:19.000000 cincoconfig-0.8.0/cincoconfig/formats/yaml.py
--rw-rw-rw-   0        0        0     6145 2021-07-17 14:22:19.000000 cincoconfig-0.8.0/cincoconfig/stubs.py
--rw-rw-rw-   0        0        0    11328 2021-07-17 14:22:19.000000 cincoconfig-0.8.0/cincoconfig/support.py
--rw-rw-rw-   0        0        0      216 2021-07-17 14:22:37.000000 cincoconfig-0.8.0/cincoconfig/version.py
-drwxrwxrwx   0        0        0        0 2021-07-17 14:36:56.000000 cincoconfig-0.8.0/cincoconfig.egg-info/
--rw-rw-rw-   0        0        0     6257 2021-07-17 14:36:55.000000 cincoconfig-0.8.0/cincoconfig.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1127 2021-07-17 14:36:55.000000 cincoconfig-0.8.0/cincoconfig.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-07-17 14:36:55.000000 cincoconfig-0.8.0/cincoconfig.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      166 2021-07-17 14:36:55.000000 cincoconfig-0.8.0/cincoconfig.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2021-07-17 14:36:55.000000 cincoconfig-0.8.0/cincoconfig.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2021-07-17 14:36:56.000000 cincoconfig-0.8.0/requirements/
--rw-rw-rw-   0        0        0      177 2021-07-17 14:22:19.000000 cincoconfig-0.8.0/requirements/requirements-dev.txt
--rw-rw-rw-   0        0        0       84 2019-08-14 12:47:56.000000 cincoconfig-0.8.0/requirements/requirements-features.txt
--rw-rw-rw-   0        0        0        0 2019-06-26 21:17:11.000000 cincoconfig-0.8.0/requirements/requirements.txt
--rw-rw-rw-   0        0        0      327 2021-07-17 14:36:56.000000 cincoconfig-0.8.0/setup.cfg
--rw-rw-rw-   0        0        0     1761 2021-07-17 14:36:01.000000 cincoconfig-0.8.0/setup.py
+-rw-r--r--   0        0        0     6083 2023-04-23 18:52:06.429041 cincoconfig-0.9.0/CHANGELOG.md
+-rw-r--r--   0        0        0      760 2023-04-22 21:27:06.093972 cincoconfig-0.9.0/cincoconfig/__init__.py
+-rw-r--r--   0        0        0    52491 2023-04-23 18:51:18.627860 cincoconfig-0.9.0/cincoconfig/core.py
+-rw-r--r--   0        0        0     8868 2023-04-23 18:51:18.629856 cincoconfig-0.9.0/cincoconfig/encryption.py
+-rw-r--r--   0        0        0     1449 2023-04-22 21:27:06.098958 cincoconfig-0.9.0/cincoconfig/fields/__init__.py
+-rw-r--r--   0        0        0     1590 2023-04-22 21:27:06.099955 cincoconfig-0.9.0/cincoconfig/fields/bool_field.py
+-rw-r--r--   0        0        0     2339 2023-04-22 21:27:06.100955 cincoconfig-0.9.0/cincoconfig/fields/bytes_field.py
+-rw-r--r--   0        0        0     7394 2023-04-23 18:51:18.631849 cincoconfig-0.9.0/cincoconfig/fields/dict_field.py
+-rw-r--r--   0        0        0     2849 2023-04-23 18:51:18.633844 cincoconfig-0.9.0/cincoconfig/fields/file_field.py
+-rw-r--r--   0        0        0     3365 2023-04-22 21:27:06.103947 cincoconfig-0.9.0/cincoconfig/fields/include_field.py
+-rw-r--r--   0        0        0     2349 2023-04-22 21:27:06.104943 cincoconfig-0.9.0/cincoconfig/fields/instance_method_field.py
+-rw-r--r--   0        0        0     7002 2023-04-22 21:27:06.106938 cincoconfig-0.9.0/cincoconfig/fields/list_field.py
+-rw-r--r--   0        0        0     4387 2023-04-22 21:27:06.108084 cincoconfig-0.9.0/cincoconfig/fields/net_field.py
+-rw-r--r--   0        0        0     2496 2023-04-22 21:27:06.108589 cincoconfig-0.9.0/cincoconfig/fields/number_field.py
+-rw-r--r--   0        0        0    11663 2023-04-23 18:51:18.635838 cincoconfig-0.9.0/cincoconfig/fields/secure_field.py
+-rw-r--r--   0        0        0     6105 2023-04-23 18:51:18.637833 cincoconfig-0.9.0/cincoconfig/fields/string_field.py
+-rw-r--r--   0        0        0      939 2023-04-22 21:27:06.113132 cincoconfig-0.9.0/cincoconfig/fields/url_field.py
+-rw-r--r--   0        0        0     1530 2023-04-22 21:27:06.113637 cincoconfig-0.9.0/cincoconfig/fields/virtual_field.py
+-rw-r--r--   0        0        0      895 2023-04-22 21:27:06.114640 cincoconfig-0.9.0/cincoconfig/formats/__init__.py
+-rw-r--r--   0        0        0     1645 2023-04-22 21:27:06.115637 cincoconfig-0.9.0/cincoconfig/formats/bson.py
+-rw-r--r--   0        0        0     1570 2023-04-22 21:27:06.116635 cincoconfig-0.9.0/cincoconfig/formats/json.py
+-rw-r--r--   0        0        0     1481 2023-04-22 21:27:06.117632 cincoconfig-0.9.0/cincoconfig/formats/pickle.py
+-rw-r--r--   0        0        0     6359 2023-04-22 21:27:06.118630 cincoconfig-0.9.0/cincoconfig/formats/xml.py
+-rw-r--r--   0        0        0     3379 2023-04-22 21:27:06.119626 cincoconfig-0.9.0/cincoconfig/formats/yaml.py
+-rw-r--r--   0        0        0     6224 2023-04-22 21:27:06.120623 cincoconfig-0.9.0/cincoconfig/stubs.py
+-rw-r--r--   0        0        0    12327 2023-04-23 14:28:38.080280 cincoconfig-0.9.0/cincoconfig/support.py
+-rw-r--r--   0        0        0        6 2023-04-23 18:51:29.060589 cincoconfig-0.9.0/cincoconfig/VERSION
+-rw-r--r--   0        0        0      290 2023-04-22 21:27:06.123616 cincoconfig-0.9.0/cincoconfig/version.py
+-rw-r--r--   0        0        0      997 2023-04-22 21:27:06.091978 cincoconfig-0.9.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0     5899 2021-07-17 14:22:19.908817 cincoconfig-0.9.0/docs/conf.py
+-rw-r--r--   0        0        0      876 2023-04-04 00:44:15.333389 cincoconfig-0.9.0/docs/configs.rst
+-rw-r--r--   0        0        0      468 2019-08-14 12:47:56.743119 cincoconfig-0.9.0/docs/encryption.rst
+-rw-r--r--   0        0        0     2098 2023-04-22 20:21:19.546570 cincoconfig-0.9.0/docs/fields.rst
+-rw-r--r--   0        0        0     1029 2021-07-17 14:22:19.912806 cincoconfig-0.9.0/docs/formats.rst
+-rw-r--r--   0        0        0     3542 2021-07-17 14:22:19.913803 cincoconfig-0.9.0/docs/index.rst
+-rwxr-xr-x   0        0        0      787 2019-06-26 21:17:11.446120 cincoconfig-0.9.0/docs/make.bat
+-rw-r--r--   0        0        0      580 2019-06-26 21:17:11.438679 cincoconfig-0.9.0/docs/Makefile
+-rw-r--r--   0        0        0     4644 2021-07-17 14:22:19.915798 cincoconfig-0.9.0/docs/recipes.rst
+-rw-r--r--   0        0        0       25 2023-04-23 03:27:32.268631 cincoconfig-0.9.0/docs/rtd-requirements.txt
+-rw-r--r--   0        0        0      454 2021-03-22 14:30:44.996976 cincoconfig-0.9.0/docs/stubs.rst
+-rw-r--r--   0        0        0      469 2023-04-04 00:44:15.335384 cincoconfig-0.9.0/docs/support.rst
+-rw-r--r--   0        0        0     2703 2019-08-23 12:16:01.921036 cincoconfig-0.9.0/example.py
+-rw-r--r--   0        0        0      772 2019-06-26 21:17:11.418620 cincoconfig-0.9.0/LICENSE
+-rw-r--r--   0        0        0     2740 2023-04-23 18:51:38.832142 cincoconfig-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     4134 2021-07-17 14:32:38.172220 cincoconfig-0.9.0/README.md
+-rw-r--r--   0        0        0        0 2019-06-26 21:17:11.460006 cincoconfig-0.9.0/tests/__init__.py
+-rw-r--r--   0        0        0    24574 2023-04-22 21:27:06.128603 cincoconfig-0.9.0/tests/test_config.py
+-rw-r--r--   0        0        0     6361 2023-04-22 21:27:06.129844 cincoconfig-0.9.0/tests/test_encryption.py
+-rw-r--r--   0        0        0      467 2023-04-22 21:27:06.130349 cincoconfig-0.9.0/tests/test_errors.py
+-rw-r--r--   0        0        0        0 2019-06-26 21:17:11.466949 cincoconfig-0.9.0/tests/test_fields/__init__.py
+-rw-r--r--   0        0        0     1990 2023-04-22 21:27:06.131494 cincoconfig-0.9.0/tests/test_fields/test_bool.py
+-rw-r--r--   0        0        0     2909 2023-04-22 21:27:06.132495 cincoconfig-0.9.0/tests/test_fields/test_bytes.py
+-rw-r--r--   0        0        0     6300 2023-04-22 21:27:06.133495 cincoconfig-0.9.0/tests/test_fields/test_challenge.py
+-rw-r--r--   0        0        0      740 2023-04-22 21:27:06.134491 cincoconfig-0.9.0/tests/test_fields/test_configtype_field.py
+-rw-r--r--   0        0        0     8430 2023-04-22 21:27:06.135487 cincoconfig-0.9.0/tests/test_fields/test_dict.py
+-rw-r--r--   0        0        0     7045 2023-04-22 21:27:06.136484 cincoconfig-0.9.0/tests/test_fields/test_field.py
+-rw-r--r--   0        0        0     3583 2023-04-22 21:27:06.137482 cincoconfig-0.9.0/tests/test_fields/test_filename.py
+-rw-r--r--   0        0        0     2140 2023-04-22 21:27:06.138479 cincoconfig-0.9.0/tests/test_fields/test_include.py
+-rw-r--r--   0        0        0     1977 2023-04-22 21:27:06.139476 cincoconfig-0.9.0/tests/test_fields/test_instance_method.py
+-rw-r--r--   0        0        0    10871 2023-04-22 21:27:06.140473 cincoconfig-0.9.0/tests/test_fields/test_list.py
+-rw-r--r--   0        0        0     3437 2023-04-22 21:27:06.141471 cincoconfig-0.9.0/tests/test_fields/test_net.py
+-rw-r--r--   0        0        0     1589 2023-04-22 21:27:06.143433 cincoconfig-0.9.0/tests/test_fields/test_number.py
+-rw-r--r--   0        0        0     3554 2023-04-22 21:27:06.143940 cincoconfig-0.9.0/tests/test_fields/test_secure.py
+-rw-r--r--   0        0        0     6698 2023-04-22 21:27:06.145379 cincoconfig-0.9.0/tests/test_fields/test_string.py
+-rw-r--r--   0        0        0     1587 2023-04-22 21:27:06.145886 cincoconfig-0.9.0/tests/test_fields/test_virtual.py
+-rw-r--r--   0        0        0      719 2023-04-22 21:27:06.148024 cincoconfig-0.9.0/tests/test_formats/test_bson.py
+-rw-r--r--   0        0        0      596 2023-04-22 21:27:06.149021 cincoconfig-0.9.0/tests/test_formats/test_json.py
+-rw-r--r--   0        0        0      407 2023-04-22 21:27:06.150018 cincoconfig-0.9.0/tests/test_formats/test_pickle.py
+-rw-r--r--   0        0        0     1989 2023-04-22 21:27:06.151015 cincoconfig-0.9.0/tests/test_formats/test_registry.py
+-rw-r--r--   0        0        0     1812 2023-04-22 21:27:06.153010 cincoconfig-0.9.0/tests/test_formats/test_xml.py
+-rw-r--r--   0        0        0     1325 2023-04-22 21:27:06.154007 cincoconfig-0.9.0/tests/test_formats/test_yaml.py
+-rw-r--r--   0        0        0     8494 2023-04-22 21:27:06.155005 cincoconfig-0.9.0/tests/test_schema.py
+-rw-r--r--   0        0        0     4935 2023-04-22 21:27:06.156999 cincoconfig-0.9.0/tests/test_stubs.py
+-rw-r--r--   0        0        0     9875 2023-04-22 21:27:06.157997 cincoconfig-0.9.0/tests/test_support.py
+-rw-r--r--   0        0        0     4938 1970-01-01 00:00:00.000000 cincoconfig-0.9.0/setup.py
+-rw-r--r--   0        0        0     5328 1970-01-01 00:00:00.000000 cincoconfig-0.9.0/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `cincoconfig-0.8.0/LICENSE` & `cincoconfig-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cincoconfig-0.8.0/PKG-INFO` & `cincoconfig-0.9.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,149 +1,154 @@
-Metadata-Version: 2.1
-Name: cincoconfig
-Version: 0.8.0
-Summary: Universal configuration file parser
-Home-page: https://cincoconfig.readthedocs.io/en/latest/
-Author: Adam Meily
-Author-email: meily.adam@gmail.com
-License: ISC
-Project-URL: Travis CI, https://travis-ci.com/github/ameily/cincoconfig
-Project-URL: Documentation, https://cincoconfig.readthedocs.io/en/latest/
-Project-URL: Source, https://github.com/ameily/cincoconfig/
-Description: # Cinco Config
-        
-        [![Build Status](https://travis-ci.com/ameily/cincoconfig.svg?branch=master)](https://travis-ci.com/github/ameily/cincoconfig)
-        [![Coverage Status](https://coveralls.io/repos/github/ameily/cincoconfig/badge.svg?branch=master)](https://coveralls.io/github/ameily/cincoconfig?branch=master)
-        [![Docs Status](https://readthedocs.org/projects/cincoconfig/badge/)](https://cincoconfig.readthedocs.io/en/latest/)
-        
-        Next generation universal configuration file parser. The config file structure is defined
-        programmatically and expressively, no need to create classes and inheritance.
-        
-        Let's get right to it:
-        
-        ```python
-        # app_config.py
-        import getpass
-        from cincoconfig import *
-        
-        # first, define the configuration's schema -- the fields available that
-        # customize the application's or library's behavior
-        schema = Schema()
-        schema.mode = ApplicationModeField(default='production')
-        
-        # nested configurations are built on the fly
-        # http is now a subconfig
-        schema.http.port = PortField(default=8080, required=True)
-        
-        # each field has its own validation rules that are run anytime the config
-        # value is loaded from disk or modified by the user.
-        # here, this field only accepts IPv4 network addresses and the user is
-        # required to define this field in the configuration file.
-        schema.http.address = IPv4AddressField(default='127.0.0.1', required=True)
-        
-        schema.http.ssl.enabled = BoolField(default=False)
-        schema.http.ssl.cafile = FilenameField()
-        schema.http.ssl.keyfile = FilenameField()
-        schema.http.ssl.certfile = FilenameField()
-        
-        schema.db.host = HostnameField(allow_ipv4=True, required=True, default='localhost')
-        schema.db.port = PortField(default=27017, required=True)
-        schema.db.name = StringField(default='my_app', required=True)
-        schema.db.user = StringField(default='admin')
-        
-        # some configuration values are sensitive, such as credentials, so
-        # cincoconfig provides config value encryption when the value is
-        # saved to disk via the SecureField
-        schema.db.password = SecureField()
-        
-        # get a field programmatically
-        print(schema['db.host']) # >>> schema.db.host
-        
-        # once a schema is defined, build the actual configuration object
-        # that can load config files from disk and interact with the values
-        config = schema()
-        
-        # print the http port
-        print(config.http.port) # >>> 8080
-        
-        # print the http port programmatically
-        print(config['http.port']) # >>> 8080
-        
-        config.db.password = getpass.getpass("Enter Password: ") # < 'password'
-        
-        # set a config value manually
-        if config.mode == 'production':
-            config.db.name = config.db.name + '_production'
-        
-        print(config.dumps(format='json', pretty=True).decode())
-        # {
-        #   "mode": "production",
-        #   "http": {
-        #     "port": 8080,
-        #     "address": "127.0.0.1"
-        #     "ssl": {
-        #       "enabled": false
-        #     }
-        #   },
-        #   "db": {
-        #     "host": "localhost",
-        #     "port": 27017,
-        #     "name": "my_app_production",
-        #     "user": "admin",
-        #     "password": {
-        #       "method": "best",
-        #       "ciphertext": "<ciphertext>"
-        #     }
-        #   }
-        # }
-        ```
-        
-        ### Override Configuration with Command Line Arguments (argparse)
-        
-        ```python
-        # config.py
-        schema = Schema()
-        schema.mode = ApplicationModeField(default='production', modes=['production', 'debug'])
-        schema.http.port = PortField(default=8080, required=True)
-        schema.http.address = IPv4AddressField(default='127.0.0.1', required=True)
-        
-        config = schema()
-        
-        # __main__.py
-        import argparse
-        from .config import config, schema
-        
-        parser = schema.generate_argparse_parser()
-        #
-        # The generate_argparse_parser() method auto generates the parser using --long-opts. For this
-        # configuration, the returned parser is equivalent to:
-        #
-        # parser = argparse.ArgumentParser()
-        #
-        # parser.add_argument('--http-address', action='store', dest='http.address')
-        # parser.add_argument('--http-port', action='store', dest='http.port')
-        # parser.add_argument('--mode', action='store', dest='mode')
-        #
-        
-        # new args can be added to the parser
-        parser.add_argument('-c', '--config', action='store')
-        args = parser.parse_args()
-        if args.config:
-            config.load(args.config, format='json')
-        
-        # update the configuration with arguments specified via the command line
-        config.cmdline_args_override(args, ignore=['config'])
-        ```
-        
-Keywords: config,configuration
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: ISC License (ISCL)
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
-Description-Content-Type: text/markdown
-Provides-Extra: features
-Provides-Extra: dev
+Metadata-Version: 2.1
+Name: cincoconfig
+Version: 0.9.0
+Summary: Universal configuration file parser
+Home-page: https://github.com/ameily/cincoconfig
+License: ISC
+Keywords: config,configuration
+Author: Adam Meily
+Author-email: meily.adam@gmail.com
+Requires-Python: >=3.7,<4.0
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved
+Classifier: License :: OSI Approved :: ISC License (ISCL)
+Classifier: Natural Language :: English
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
+Project-URL: Documentation, https://cincoconfig.readthedocs.io/en/latest/
+Project-URL: Repository, https://github.com/ameily/cincoconfig
+Description-Content-Type: text/markdown
+
+# Cinco Config
+
+[![Build Status](https://travis-ci.com/ameily/cincoconfig.svg?branch=master)](https://travis-ci.com/github/ameily/cincoconfig)
+[![Coverage Status](https://coveralls.io/repos/github/ameily/cincoconfig/badge.svg?branch=master)](https://coveralls.io/github/ameily/cincoconfig?branch=master)
+[![Docs Status](https://readthedocs.org/projects/cincoconfig/badge/)](https://cincoconfig.readthedocs.io/en/latest/)
+
+Next generation universal configuration file parser. The config file structure is defined
+programmatically and expressively, no need to create classes and inheritance.
+
+Let's get right to it:
+
+```python
+# app_config.py
+import getpass
+from cincoconfig import *
+
+# first, define the configuration's schema -- the fields available that
+# customize the application's or library's behavior
+schema = Schema()
+schema.mode = ApplicationModeField(default='production')
+
+# nested configurations are built on the fly
+# http is now a subconfig
+schema.http.port = PortField(default=8080, required=True)
+
+# each field has its own validation rules that are run anytime the config
+# value is loaded from disk or modified by the user.
+# here, this field only accepts IPv4 network addresses and the user is
+# required to define this field in the configuration file.
+schema.http.address = IPv4AddressField(default='127.0.0.1', required=True)
+
+schema.http.ssl.enabled = BoolField(default=False)
+schema.http.ssl.cafile = FilenameField()
+schema.http.ssl.keyfile = FilenameField()
+schema.http.ssl.certfile = FilenameField()
+
+schema.db.host = HostnameField(allow_ipv4=True, required=True, default='localhost')
+schema.db.port = PortField(default=27017, required=True)
+schema.db.name = StringField(default='my_app', required=True)
+schema.db.user = StringField(default='admin')
+
+# some configuration values are sensitive, such as credentials, so
+# cincoconfig provides config value encryption when the value is
+# saved to disk via the SecureField
+schema.db.password = SecureField()
+
+# get a field programmatically
+print(schema['db.host']) # >>> schema.db.host
+
+# once a schema is defined, build the actual configuration object
+# that can load config files from disk and interact with the values
+config = schema()
+
+# print the http port
+print(config.http.port) # >>> 8080
+
+# print the http port programmatically
+print(config['http.port']) # >>> 8080
+
+config.db.password = getpass.getpass("Enter Password: ") # < 'password'
+
+# set a config value manually
+if config.mode == 'production':
+    config.db.name = config.db.name + '_production'
+
+print(config.dumps(format='json', pretty=True).decode())
+# {
+#   "mode": "production",
+#   "http": {
+#     "port": 8080,
+#     "address": "127.0.0.1"
+#     "ssl": {
+#       "enabled": false
+#     }
+#   },
+#   "db": {
+#     "host": "localhost",
+#     "port": 27017,
+#     "name": "my_app_production",
+#     "user": "admin",
+#     "password": {
+#       "method": "best",
+#       "ciphertext": "<ciphertext>"
+#     }
+#   }
+# }
+```
+
+### Override Configuration with Command Line Arguments (argparse)
+
+```python
+# config.py
+schema = Schema()
+schema.mode = ApplicationModeField(default='production', modes=['production', 'debug'])
+schema.http.port = PortField(default=8080, required=True)
+schema.http.address = IPv4AddressField(default='127.0.0.1', required=True)
+
+config = schema()
+
+# __main__.py
+import argparse
+from .config import config, schema
+
+parser = schema.generate_argparse_parser()
+#
+# The generate_argparse_parser() method auto generates the parser using --long-opts. For this
+# configuration, the returned parser is equivalent to:
+#
+# parser = argparse.ArgumentParser()
+#
+# parser.add_argument('--http-address', action='store', dest='http.address')
+# parser.add_argument('--http-port', action='store', dest='http.port')
+# parser.add_argument('--mode', action='store', dest='mode')
+#
+
+# new args can be added to the parser
+parser.add_argument('-c', '--config', action='store')
+args = parser.parse_args()
+if args.config:
+    config.load(args.config, format='json')
+
+# update the configuration with arguments specified via the command line
+config.cmdline_args_override(args, ignore=['config'])
+```
+
```

### Comparing `cincoconfig-0.8.0/README.md` & `cincoconfig-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `cincoconfig-0.8.0/cincoconfig/__init__.py` & `cincoconfig-0.9.0/cincoconfig/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,39 @@
 #
 # Copyright (C) 2021 Adam Meily
 #
 # This file is subject to the terms and conditions defined in the file 'LICENSE', which is part of
 # this source code package.
 #
-'''
+"""
 Cincoconfig Public API
-'''
-from .core import Config, Field, Schema, ValidationError, AnyField, ConfigFormat, ConfigType
-from .support import (make_type, validator, get_all_fields, generate_argparse_parser,
-                      item_ref_path, cmdline_args_override, asdict, get_fields)
-from .fields import *
+"""
+# ruff: noqa: F401
+from .core import (
+    AnyField,
+    Config,
+    ConfigFormat,
+    ConfigType,
+    Field,
+    Schema,
+    ValidationError,
+)
 from .encryption import KeyFile
+from .fields import *  # noqa: F403
 from .stubs import generate_stub
+from .support import (
+    asdict,
+    cmdline_args_override,
+    generate_argparse_parser,
+    get_all_fields,
+    get_fields,
+    is_value_defined,
+    item_ref_path,
+    make_type,
+    reset_value,
+    validator,
+)
 from .version import __version__
 
 # DEPRECATED TYPE ALIASES
 BaseConfig = Config
 BaseSchema = Schema
```

### Comparing `cincoconfig-0.8.0/cincoconfig/core.py` & `cincoconfig-0.9.0/cincoconfig/core.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,57 +1,74 @@
 #
 # Copyright (C) 2021 Adam Meily
 #
 # This file is subject to the terms and conditions defined in the file 'LICENSE', which is part of
 # this source code package.
 #
-'''
+"""
 Core configuration classes and methods.
-'''
+"""
 # pylint: disable=too-many-lines
-import os
 import inspect
+import os
+import warnings
+from argparse import ArgumentParser, Namespace
 from collections import OrderedDict
 from functools import partial
-from typing import Union, Any, Optional, Dict, Iterator, Tuple, List, Callable, Type
-from argparse import ArgumentParser, Namespace
-import warnings
+from typing import (
+    Any,
+    Callable,
+    ClassVar,
+    Dict,
+    Iterator,
+    List,
+    Optional,
+    Set,
+    Tuple,
+    Type,
+    Union,
+)
 
 from .encryption import KeyFile
 
-ConfigValidator = Callable[['Config'], None]
-FieldValidator = Callable[['Config', Any], Any]
-SchemaField = Union['BaseField', 'ConfigType']
+ConfigValidator = Callable[["Config"], None]
+FieldValidator = Callable[["Config", Any], Any]
+SchemaField = Union["BaseField", "ConfigType"]
 TFormatFactory = Callable[[], "ConfigFormat"]
 
 
 def isconfigtype(obj: Any) -> bool:
-    '''
+    """
     Check if an object is configuration type (is class and is subclass of :class:`ConfigType`).
 
     :param obj: object to check
     :returns: the object is a configuration type
-    '''
+    """
     return inspect.isclass(obj) and issubclass(obj, ConfigType)
 
 
 class ValidationError(ValueError):
-    '''
+    """
     An error that occurs while validating a field's value or entire configuration.
-    '''
+    """
 
-    def __init__(self, config: 'Config', field: Optional['BaseField'], exc: Union[str, Exception],
-                 ref_path: str = None):
-        '''
+    def __init__(
+        self,
+        config: "Config",
+        field: Optional["BaseField"],
+        exc: Union[str, Exception],
+        ref_path: Optional[str] = None,
+    ):
+        """
         :param config: parent configuration
         :param field: field being validated, None if the entire config was being validated
         :param exc: original exception
         :param ref_path: override reference path to the field or configuration that failed
             validation
-        '''
+        """
         super().__init__(config, field, exc, ref_path)
         self.config = config
         self.field = field
         self.exc = exc
         self._ref_path = ref_path
 
     def __str__(self):
@@ -60,175 +77,186 @@
         else:
             msg = str(self.exc)
 
         path = self.ref_path
         if isinstance(self.field, Field) and self.field._name:
             path += " (%s)" % self.field._name
 
-        return '%s: %s' % (path, msg)
+        return "%s: %s" % (path, msg) if path else msg
 
     @property
     def ref_path(self) -> str:
-        '''
+        """
         :returns: the full path to the field or configuration that failed validation
-        '''
+        """
         if self._ref_path:
             return self._ref_path
 
         path = self.config._ref_path
         if self.field:
             if path:
                 path += "." + self.field._key
             else:
                 path = self.field._key
         return path
 
 
 class ContainerValueMixin:
-    '''
+    """
     An abstract base class for container value (list, dict, etc.)
-    '''
+    """
 
     def _get_item_position(self, item: Any) -> str:
-        '''
+        """
         Return the position for a given item. This method is called when generate the full path to
         a configuration item.
 
         :param item: container item
         :returns: the position of the item
-        '''
+        """
         raise NotImplementedError()
 
 
 class VirtualFieldMixin:
-    '''
+    """
     Field mixin to flag a field as virtual.
-    '''
+    """
 
 
 class InstanceMethodFieldMixin:
-    '''
+    """
     Field mixin to bind an instance method to a configuration object.
-    '''
+    """
 
 
 class FeatureFlagFieldMixin:
-    '''
+    """
     Field mixin to flag a the schema as enabled or disabled.
-    '''
-    def is_feature_enabled(self, cfg: 'Config') -> bool:
-        '''
+    """
+
+    def is_feature_enabled(self, cfg: "Config") -> bool:
+        """
         Check if the feature is enabled.
 
         :returns: ``True`` if the feature is enabled and ``False`` if it is not.
-        '''
+        """
         raise NotImplementedError()
 
 
 class IncludeFieldMixin:
-    '''
+    """
     Field mixin to include a configuration file.
-    '''
+    """
 
-    def include(self, config: 'Config', fmt: 'ConfigFormat', filename: str, base: dict) -> dict:
-        '''
+    def include(
+        self, config: "Config", fmt: "ConfigFormat", filename: str, base: dict
+    ) -> dict:
+        """
         Include a configuration file and combine it with an already parsed basic value tree. Values
         defined in the included file will overwrite values in the base tree. Nested trees (``dict``
         objects) will be combined using a :meth:`dict.update` like method, :meth:`combine_trees`.
 
         :param config: configuration object
         :param fmt: configuration file format that will parse the included file
         :param filename: included file path
         :param base: base config value tree
         :returns: the new basic value tree containing the base tree and the included tree
-        '''
+        """
         raise NotImplementedError()
 
 
 class BaseField:
-    '''
+    """
     Base class for all fields in a schema.
-    '''
+    """
 
-    def __init__(self, key: str = None, name: str = None, schema: 'Schema' = None):
-        '''
+    def __init__(
+        self,
+        key: Optional[str] = None,
+        name: Optional[str] = None,
+        schema: Optional["Schema"] = None,
+    ):
+        """
         :param key: field key
         :param name: descriptive name
         :param schema: owning schema
-        '''
-        self._key: str = key or ''
+        """
+        self._key: str = key or ""
         self._name = name
         self._schema = schema
 
-    def __setkey__(self, schema: 'Schema', key: str) -> None:
-        '''
+    def __setkey__(self, schema: "Schema", key: str) -> None:
+        """
         Set the field key and bind it to a schema.
 
         :param schema: owning schema
         :param key: field key
-        '''
+        """
         self._schema = schema
         self._key = key
 
-    def __getval__(self, cfg: 'Config') -> Any:
-        '''
+    def __getval__(self, cfg: "Config") -> Any:
+        """
         Retrieve the value from the config. The default implementation retrieves the value from the
         config by the field *key*.
 
         :param cfg: current config
         :returns: the value stored in the config
-        '''
+        """
         return cfg._data[self._key]
 
-    def __setdefault__(self, cfg: 'Config') -> None:
-        '''
+    def __setdefault__(self, cfg: "Config") -> None:
+        """
         Set the default value in the configuration. Subclasses should set the field's default value
-        directly in the ``cfg._data`` dictionary. For example:
+        using the :meth:`Config._set_default_value` method. For example:
 
         .. code-block:: python
 
             def __setdefault__(self, cfg: 'Config') -> None:
-                cfg._data[self._key] = "Hello, world!"
-        '''
+                cfg._set_default_value(self._key, "Hello, world!")
+        """
 
     @property
     def full_path(self) -> str:
-        '''
+        """
         **(Deprecated, will be removed in v1.0.0)** get the full path to the field
 
         :returns: the full path to this configuration
-        '''
-        warnings.warn("BaseField.full_path is deprecated and will be removed in v1.0.0, use "
-                      "cincoconfig.item_ref_path() instead", DeprecationWarning)
+        """
+        warnings.warn(
+            "BaseField.full_path is deprecated and will be removed in v1.0.0, use "
+            "cincoconfig.item_ref_path() instead",
+            DeprecationWarning,
+        )
         return self._ref_path
 
     @property
     def _ref_path(self) -> str:
-        '''
+        """
         Get the full reference path to the schema field. For example:
 
         .. code-block::
 
             >>> schema = Schema()
             >>> schema.x.y.z = Field()
             >>> schema.x.y.z._ref_path
             'x.y.z'
-        '''
+        """
         path = [self._key]
         schema = self._schema
         while schema:
             if schema._key:
                 path.append(schema._key)
             schema = schema._schema
 
-        return '.'.join(reversed(path))
+        return ".".join(reversed(path))
 
 
 class Field(BaseField):
-    '''
+    """
     The base configuration field. Fields provide validation and the mechanisms to retrieve and set
     values from a :class:`Config`. Field's are composable and reusable so they should not store
     state or store the field value.
 
     Validation errors should raise a :class:`ValueError` exception with a brief message.
 
     There are three steps to validating a value:
@@ -307,40 +335,51 @@
 
         schema.auth = Schema(env="SECRET")
         schema.auth.username = StringField()
 
     - The top-level schema is configured to autogenerate and load environment variables for all
       fields.
     - ``mode`` is loaded from the ``APP_MODE`` environment variable.
-    - ``port`` is not loaded from any the environment variabale.
+    - ``port`` is not loaded from any the environment variable.
     - ``db.host`` is loaded from the ``DB_HOST`` environment variable.
     - The ``auth`` schema has a environment variable prefix of ``SECRET``. All children and nested
       fields/schemas will start with ``SECRET_``.
     - The ``auth.username`` field is loaded from the ``SECRET_USERNAME`` environment variable.
-    '''
+    """
+
     storage_type = Any
 
-    def __init__(self, *, key: str = None, schema: 'Schema' = None, name: str = None,
-                 required: bool = False, default: Union[Callable, Any] = None,
-                 validator: FieldValidator = None, sensitive: bool = False,
-                 description: str = None, help: str = None, env: Union[bool, str] = None):
-        '''
+    def __init__(
+        self,
+        *,
+        key: Optional[str] = None,
+        schema: Optional["Schema"] = None,
+        name: Optional[str] = None,
+        required: bool = False,
+        default: Optional[Union[Callable, Any]] = None,
+        validator: Optional[FieldValidator] = None,
+        sensitive: bool = False,
+        description: Optional[str] = None,
+        help: Optional[str] = None,
+        env: Optional[Union[bool, str]] = None
+    ):
+        """
         All builtin Fields accept the following keyword parameters.
 
         :param name: field friendly name, used for error messages and documentation
         :param key: the key of the field in the config, this is typically not specified and,
             instead the :meth:`__setkey__` will be called by the config
         :param required: the field is required and a :class:`ValueError` will be raised if the
             value is ``None``
         :param default: the default value, which can be a called that is invoke with no arguments
             and should return the default value
         :param validator: an additional validator function that is invoked during validation
         :param sensitive: the field stores a sensitive value
         :param help: the field documentation
-        '''
+        """
         super().__init__(name=name, key=key, schema=schema)
         self.required = required
         self._default = default
         self.validator = validator
         self.sensitive = sensitive
         self.description = description
         self.help = help.strip() if help else None
@@ -364,96 +403,98 @@
             >>> print(field.short_help)
             this is a short description
             that can span multiple lines.
 
         :returns: the first paragraph of ``help``
         '''
         if self.help:
-            return self.help.split('\n\n', 1)[0]
+            return self.help.split("\n\n", 1)[0]
         return None
 
     @property
     def default(self) -> Any:
-        '''
+        """
         :returns: the field's default value
-        '''
+        """
         return self._default() if callable(self._default) else self._default
 
     @property
     def name(self):
-        '''
+        """
         :returns: the field's friendly name: ``name or key``
-        '''
+        """
         return self._name or self._key
 
-    def _validate(self, cfg: 'Config', value: Any) -> Any:
-        '''
+    def _validate(self, cfg: "Config", value: Any) -> Any:
+        """
         Subclass validation hook. The default implementation just returns ``value`` unchanged.
-        '''
+        """
         return value
 
-    def __setval__(self, cfg: 'Config', value: Any):
-        '''
+    def __setval__(self, cfg: "Config", value: Any):
+        """
         Set the validated value in the config. The default implementation passes the value through
         the validation chain and then set's the validated value int the config.
 
         :param cfg: current config
         :param value: value to validated
-        '''
+        """
         cfg._data[self._key] = value
 
-    def validate(self, cfg: 'Config', value: Any) -> Any:
-        '''
+    def validate(self, cfg: "Config", value: Any) -> Any:
+        """
         Start the validation chain and verify that the value is specified if *required=True*.
 
         :param cfg: current config
         :param value: value to validate
         :returns: the validated value
-        '''
+        """
         if self.required and value is None:
-            raise ValueError('value is required')
+            raise ValueError("value is required")
 
         if value is None:
             return value
 
         value = self._validate(cfg, value)
         if self.validator:
             value = self.validator(cfg, value)
 
         return value
 
-    def __setkey__(self, schema: 'Schema', key: str):
-        '''
+    def __setkey__(self, schema: "Schema", key: str):
+        """
         Set the field's *_key*, which is called when the field is added to a schema. The default
         implementation just sets ``self._key = key``
 
         :param schema: the schema the field belongs to
         :param key: the field's unique key
-        '''
+        """
         super().__setkey__(schema, key)
 
         if self.env is False:
             return
 
-        if self.env is True or (self.env is None and isinstance(schema._env_prefix, str)):
+        if self.env is True or (
+            self.env is None and isinstance(schema._env_prefix, str)
+        ):
             # Set our environment variable name based on the schema's prefix and our key
             if isinstance(schema._env_prefix, str) and schema._env_prefix:
-                prefix = schema._env_prefix + '_'
+                prefix = schema._env_prefix + "_"
             else:
-                prefix = ''
+                prefix = ""
 
             self.env = prefix + self._key.upper()
 
-    def __setdefault__(self, cfg: 'Config') -> None:
-        '''
+    def __setdefault__(self, cfg: "Config") -> None:
+        """
         Set the default value of the field in the config. This is called when the config is first
         created.
 
         :param cfg: current config
-        '''
+        """
         value = None
 
         if isinstance(self.env, str) and self.env:
             env_value = os.environ.get(self.env)
             if env_value:
                 try:
                     env_value = self.validate(cfg, env_value)
@@ -463,18 +504,18 @@
                     raise ValidationError(cfg, self, exc) from exc
                 else:
                     value = env_value
 
         if value is None:
             value = self.default
 
-        cfg._data[self._key] = value
+        cfg._set_default_value(self._key, value)
 
-    def to_python(self, cfg: 'Config', value: Any) -> Any:
-        '''
+    def to_python(self, cfg: "Config", value: Any) -> Any:
+        """
         Convert the basic value to a Python value. Basic values are serializable (ie. not complex
         types). The following must hold true for config file saving and loading to work:
 
         .. code-block:: python
 
             assert field.to_python(field.to_basic(value)) == value
 
@@ -483,66 +524,71 @@
 
         In general, basic types are any types that can be represented in JSON: string, number,
         list, dict, boolean.
 
         :param cfg: current config
         :param value: value to convert to a Python type
         :returns: the converted Python type
-        '''
+        """
         return value
 
-    def to_basic(self, cfg: 'Config', value: Any) -> Any:
-        '''
+    def to_basic(self, cfg: "Config", value: Any) -> Any:
+        """
         Convert the Python value to the basic value.
 
         The default implementation just returns ``value``. This method is called when the config is
         saved to a file and will only be called with the value associated with this field.
 
         :param cfg: current config
         :param value: value to convert to a basic type
         :returns: the converted basic type
-        '''
+        """
         return value
 
 
 class AnyField(Field):
-    '''
+    """
     A field that accepts any value and does not perform any validation beyond the base Field's
     *required* check.
-    '''
+    """
 
 
 class ConfigTypeField(BaseField):
-    '''
+    """
     A field that wraps a :class:`ConfigType` object, created by the :meth:`~cincoconfig.make_type`
     method.
-    '''
+    """
 
-    def __init__(self, config_type: Type["ConfigType"], key: str = None, name: str = None):
-        '''
+    def __init__(
+        self,
+        config_type: Type["ConfigType"],
+        key: Optional[str] = None,
+        name: Optional[str] = None,
+    ):
+        """
         :param config_type: the ``ConfigType`` class
-        '''
+        """
         super().__init__(key=key, name=name)
         self.config_type = config_type
 
-    def __setdefault__(self, cfg: 'Config') -> None:
-        cfg._data[self._key] = self.config_type(cfg)
+    def __setdefault__(self, cfg: "Config") -> None:
+        cfg._set_default_value(self._key, self.config_type(cfg))
 
-    def __call__(self, cfg: 'Config' = None) -> 'ConfigType':
-        '''
+    def __call__(self, cfg: Optional["Config"] = None) -> "ConfigType":
+        """
         Create an instance of the wrapped ``ConfigType``.
 
         :param cfg: parent configuration
         :returns: the config type instance
-        '''
+        """
         return self.config_type(cfg)
 
 
 class Schema(BaseField):
-    '''
+    """
     A config schema containing all available configuration options. A schema's fields and hierarchy
     are built dynamically.
 
     .. code-block:: python
 
         schema = Schema()
         schema.mode = ApplicationModeField(default='production', required=True)
@@ -552,167 +598,178 @@
 
     Accessing a field that does not exist, such as ``schema.http`` in the above code, dynamically
     creates and adds a new ``Schema``.
 
     Once a schema is completely defined, a :class:`Config` is created by calling the schema. The
     config is populate with the default values specified for each field and can then load the
     configuration from a file.
-    '''
+    """
 
-    def __init__(self, key: str = None, name: str = None, dynamic: bool = False,
-                 env: Union[str, bool] = None, schema: 'Schema' = None):
+    def __init__(
+        self,
+        key: Optional[str] = None,
+        name: Optional[str] = None,
+        dynamic: bool = False,
+        env: Optional[Union[str, bool]] = None,
+        schema: Optional["Schema"] = None,
+    ):
         # pylint: disable=too-many-arguments
-        '''
+        """
         :param key: schema field key
         :param dynamic: configurations created from this schema are dynamic and can add fields not
             originally in the schema
             *_key*
         :param env: the environment variable prefix for this schema and all children schemas, for
             information, see :ref:`Field Environment Variables <field-env-variables>`
-        '''
+        """
         super().__init__(key=key, schema=schema, name=name)
         self._dynamic = dynamic
         self._fields: Dict[str, BaseField] = OrderedDict()
-        self._env_prefix = '' if env is True else env
+        self._env_prefix = "" if env is True else env
         self._validators: List[ConfigValidator] = []
 
     @property
     def _feature_flag_fields(self) -> Iterator[FeatureFlagFieldMixin]:
-        '''
+        """
         :returns: an iterator of all feature flag fields
-        '''
-        return (field for field in self._fields.values()
-                if isinstance(field, FeatureFlagFieldMixin))
+        """
+        return (
+            field
+            for field in self._fields.values()
+            if isinstance(field, FeatureFlagFieldMixin)
+        )
 
-    def _is_feature_enabled(self, cfg: 'Config') -> bool:
-        '''
+    def _is_feature_enabled(self, cfg: "Config") -> bool:
+        """
         :returns: the feature is enabled (all :class:`FeatureFlagFieldMixin` fields returned
             ``True``)
-        '''
+        """
         return all(field.is_feature_enabled(cfg) for field in self._feature_flag_fields)
 
-    def __setkey__(self, schema: 'Schema', key: str) -> None:
-        '''
+    def __setkey__(self, schema: "Schema", key: str) -> None:
+        """
         Field protocol, set the schema *_key* attribute.
-        '''
+        """
         super().__setkey__(schema, key)
 
         if self._env_prefix is False:
             return
 
         if self._env_prefix is None and isinstance(schema._env_prefix, str):
             # Set our environment variable prefix to be "{parent}_{key}"
-            prefix = (schema._env_prefix + '_') if schema._env_prefix else ''
+            prefix = (schema._env_prefix + "_") if schema._env_prefix else ""
             self._env_prefix = prefix + self._key.upper()
 
-    def __setdefault__(self, cfg: 'Config') -> None:
-        cfg._data[self._key] = Config(self, cfg)
+    def __setdefault__(self, cfg: "Config") -> None:
+        cfg._set_default_value(self._key, Config(self, cfg))
 
     def _get_field(self, key: str) -> Optional[BaseField]:
-        '''
+        """
         :returns: a field from the schema
-        '''
+        """
         return self._fields.get(key)
 
     def __setattr__(self, name: str, value: Any) -> Any:
-        '''
+        """
         :param name: attribute name
         :param value: field or schema to add to the schema
-        '''
-        if name.startswith('_'):
+        """
+        if name.startswith("_"):
             object.__setattr__(self, name, value)
         else:
             value = self._add_field(name, value)
 
         return value
 
     def _add_field(self, name: str, field: SchemaField) -> BaseField:
-        '''
+        """
         Add a field to the schema. This method will call ``field.__setkey__(self, key)``.
 
         :returns: the added field (``field``)
-        '''
+        """
 
         if isconfigtype(field):
             field = ConfigTypeField(field)  # type: ignore
         elif not isinstance(field, BaseField):
             raise TypeError("Schema fields must inherit from BaseField")
 
         self._fields[name] = field  # type: ignore
         field.__setkey__(self, name)
         return field  # type: ignore
 
     def __getattr__(self, name: str) -> BaseField:
-        '''
+        """
         Retrieve a field by key or create a new ``Schema`` if the field doesn't exist.
 
         :param name: field or schema key
-        '''
+        """
         return self._fields.get(name) or self._add_field(name, Schema())
 
-    def __call__(self, parent: 'Config' = None, **data):
-        '''
+    def __call__(self, parent: Optional["Config"] = None, **data):
+        """
         Compile the schema into an initial config with default values set.
-        '''
+        """
         return Config(self, **data)
 
     def __iter__(self) -> Iterator[Tuple[str, BaseField]]:
-        '''
+        """
         Iterate over schema fields, produces as a list of tuples ``(key, field)``.
-        '''
+        """
         yield from self._fields.items()
 
     def __getitem__(self, key: str) -> BaseField:
-        '''
+        """
         :returns: field, equivalent to ``getattr(schema, key)``, however his method handles
             retrieving nested values. For example:
 
             .. code-block:: python
 
                 >>> schema = Schema()
                 >>> schema.x.y = IntField(default=10)
                 >>> print(schema['x.y'])
                 IntField(key='y', ...)
-        '''
-        key, _, subkey = key.partition('.')
+        """
+        key, _, subkey = key.partition(".")
         field = self._get_field(key) or self._add_field(key, Schema())
         if subkey:
             if isinstance(field, Schema):
                 return field.__getitem__(subkey)
             raise TypeError("Field is not a schema: %s" % field._ref_path)
         return field
 
     def __setitem__(self, name: str, value: SchemaField) -> BaseField:
-        '''
+        """
         :returns: field, equivalent to ``setattr(schema, key)``, however his method handles
             setting  nested values. For example:
 
             .. code-block:: python
 
                 >>> schema = Schema()
                 >>> schema.x = Schema()
                 >>> schema['x.y'] = IntField(default=10)
                 >>> print(schema.x.y)
                 IntField(key='y', ...)
-        '''
-        key, _, subkey = name.partition('.')
+        """
+        key, _, subkey = name.partition(".")
         field = self._get_field(key) or self._add_field(key, Schema())
         if subkey:
             if isinstance(field, Schema):
                 return field.__setitem__(subkey, value)
             raise TypeError("Field is not a schema: %s" % field._ref_path)
 
         return self._add_field(name, value)
 
-    def _validate(self, config: 'Config', collect_errors: bool = False) -> List[ValidationError]:
-        '''
+    def _validate(
+        self, config: "Config", collect_errors: bool = False
+    ) -> List[ValidationError]:
+        """
         Validate the configuration by running any registered validators against it.
 
         :param config: config to validate
-        '''
+        """
         if not self._is_feature_enabled(config):
             return []
 
         ignore_types = (IncludeFieldMixin, VirtualFieldMixin, InstanceMethodFieldMixin)
         errors = []
 
         for field in self._fields.values():
@@ -742,90 +799,112 @@
                 exc = ValidationError(config, None, err)
                 if not collect_errors:
                     raise exc from err
                 errors.append(exc)
 
         return errors
 
-    def _validate_field(self, config: 'Config', field: BaseField) -> None:
-        '''
+    def _validate_field(self, config: "Config", field: BaseField) -> None:
+        """
         Validate a single field in the configuration.
 
         :param config: configuration
         :param field: the field to validate
-        '''
+        """
         val = field.__getval__(config)
         if isinstance(field, Field):
             field.validate(config, val)
         elif isinstance(val, Config):
             val.validate()
 
-    def get_all_fields(self) -> List[Tuple[str, 'Schema', BaseField]]:
-        '''
+    def get_all_fields(self) -> List[Tuple[str, "Schema", BaseField]]:
+        """
         **(Deprecated, will be removed in v1.0.0)** get all the fields in the configuration. Use
         :meth:`~cincoconfig.get_all_fields`.
 
         :returns: a list of tuples with ``(key, schema, field)``
-        '''
+        """
         # pylint: disable=import-outside-toplevel, cyclic-import
         from .support import get_all_fields
-        warnings.warn("Config.get_all_fields() is deprecated and will be removed in v1.0.0, use "
-                      "cincoconfig.get_all_fields() instead.", DeprecationWarning)
+
+        warnings.warn(
+            "Config.get_all_fields() is deprecated and will be removed in v1.0.0, use "
+            "cincoconfig.get_all_fields() instead.",
+            DeprecationWarning,
+        )
         return get_all_fields(self)
 
     def generate_argparse_parser(self, **parser_kwargs) -> ArgumentParser:
-        '''
+        """
         **(Deprecated, will be removed in v1.0.0)** generate an :class:`~argparse.ArgumentParser`
         for the schema. Use :meth:`~cincoconfig.generate_argparse_parser`.
 
         :returns: an ``ArgumentParser`` containing arguments that match the schema's fields
-        '''
+        """
         # pylint: disable=import-outside-toplevel, cyclic-import
         from .support import generate_argparse_parser
-        warnings.warn("Schema.generate_argparse_parser() is deprecated and will be removed in "
-                      "v1.0.0, use  cincoconfig.generate_argparse_parser instead.",
-                      DeprecationWarning)
+
+        warnings.warn(
+            "Schema.generate_argparse_parser() is deprecated and will be removed in "
+            "v1.0.0, use  cincoconfig.generate_argparse_parser instead.",
+            DeprecationWarning,
+        )
         return generate_argparse_parser(self, **parser_kwargs)
 
-    def instance_method(self, key: str) -> Callable[['Config'], None]:
-        '''
+    def instance_method(self, key: str) -> Callable[["Config"], None]:
+        """
         **(Deprecated, will be removed in v1.0.0)** decorator to register an instance method with
         the schema. Use :meth:`~cincoconfig.instance_method`.
-        '''
+        """
         # pylint: disable=import-outside-toplevel, cyclic-import
         from .fields import instance_method
-        warnings.warn("Schema.instance_method() is deprecated and will be removed in v1.0.0, use "
-                      "cincoconfig.instance_method() instead.", DeprecationWarning)
+
+        warnings.warn(
+            "Schema.instance_method() is deprecated and will be removed in v1.0.0, use "
+            "cincoconfig.instance_method() instead.",
+            DeprecationWarning,
+        )
         return instance_method(self, key)
 
     def validator(self, func: ConfigValidator) -> ConfigValidator:
-        '''
+        """
         **(Deprecated, will be removed in v1.0.0)** decorator to register a validator method with
         the schema. Use :meth:`~cincoconfig.validator`.
-        '''
-        warnings.warn("Schema.validator() is deprecated and will be removed in v1.0.0, use "
-                      "cincoconfig.validator() instead.", DeprecationWarning)
+        """
+        warnings.warn(
+            "Schema.validator() is deprecated and will be removed in v1.0.0, use "
+            "cincoconfig.validator() instead.",
+            DeprecationWarning,
+        )
         self._validators.append(func)
         return func
 
-    def make_type(self, name: str, module: str = None,
-                  key_filename: str = None) -> Type['ConfigType']:
-        '''
+    def make_type(
+        self,
+        name: str,
+        module: Optional[str] = None,
+        key_filename: Optional[str] = None,
+    ) -> Type["ConfigType"]:
+        """
         **(Deprecated, will be removed in v1.0.0)** create a new type from the schema. Use
         :meth:`~cincoconfig.make_type`.
-        '''
+        """
         # pylint: disable=import-outside-toplevel, cyclic-import
         from .support import make_type
-        warnings.warn("Schema.make_type() is deprecated and will be removed in v1.0.0, use "
-                      "cincoconfig.make_type() instead.", DeprecationWarning)
+
+        warnings.warn(
+            "Schema.make_type() is deprecated and will be removed in v1.0.0, use "
+            "cincoconfig.make_type() instead.",
+            DeprecationWarning,
+        )
         return make_type(self, name, module, key_filename)
 
 
 class Config:  # pylint: disable=too-many-instance-attributes
-    '''
+    """
     A configuration.
 
     Parsing and serializing the configuration is done via an intermediary object, a tree
     (:class:`dict`) containing only basic (serializable) values (see Field
     :meth:`~cincoconfig.abc.Field.to_basic`).
 
     When saving, the config will convert the current config values to a tree and then pass the
@@ -859,32 +938,40 @@
         # config = schema()
 
     Each config object can have an associated :class:`cincoconfig.KeyFile`, passed in the
     constructor as ``key_filename``. If the configuration file doesn't have a key file path set,
     the config object will use the parent config's key file. Requesting a key file will bubble up
     to the first config object that has the key filename set and, if no config has a keyfile, the
     default path will be used, :const:`DEFAULT_CINCOKEY_FILEPATH`.
-    '''
+    """
+
     DEFAULT_CINCOKEY_FILEPATH = os.path.join(os.path.expanduser("~"), ".cincokey")
 
-    def __init__(self, schema: Schema, parent: 'Config' = None, key_filename: str = None, **data):
-        '''
+    def __init__(
+        self,
+        schema: Schema,
+        parent: Optional["Config"] = None,
+        key_filename: Optional[str] = None,
+        **data
+    ):
+        """
         :param schema: backing schema, stored as *_schema*
         :param parent: parent config instance, only set when this config is a field of another
             config, stored as *_parent*
         :param key_filename: path to key file
         :param data: configuration values
-        '''
+        """
         self._schema = schema
         self._parent = parent
         self._container: Optional[ContainerValueMixin] = None
         self._data: Dict[str, Any] = OrderedDict()
         self._fields: Dict[str, BaseField] = OrderedDict()
         self._key = schema._key
         self.__keyfile = None  # type: Optional[KeyFile]
+        self._default_value_keys: Set[str] = set()
 
         if key_filename:
             self._key_filename = key_filename
 
         for key, value in data.items():
             self._set_value(key, value)
 
@@ -892,67 +979,78 @@
             if key in data:
                 continue
 
             field.__setdefault__(self)
 
     @property
     def _key_filename(self) -> str:
-        '''
+        """
         :return: the path to the cinco encryption key file (if not set, get the parent config's
             key filename)
-        '''
+        """
         if self.__keyfile:
             return self.__keyfile.filename
         if self._parent:
             return self._parent._key_filename
         return Config.DEFAULT_CINCOKEY_FILEPATH
 
     @_key_filename.setter
     def _key_filename(self, key_filename: str) -> None:
-        '''
+        """
         Set the cinco encryption key file
         :param key_filename: path to the cinco encryption key file
-        '''
+        """
         if not key_filename:
             self.__keyfile = None
         else:
             self.__keyfile = KeyFile(key_filename)
 
     @property
     def _keyfile(self) -> KeyFile:
-        '''
+        """
         :returns: the config's encryption key file (if not set, get the parent config's key file)
-        '''
+        """
         if not self.__keyfile:
             if self._parent:
                 # This will bubble up to the root config
                 self.__keyfile = self._parent._keyfile
             else:
                 self.__keyfile = KeyFile(Config.DEFAULT_CINCOKEY_FILEPATH)
         return self.__keyfile
 
     def _get_field(self, key: str) -> Optional[BaseField]:
-        '''
+        """
         :returns: a field from the schema or the dynamically added field if the schema is dynamic.
-        '''
+        """
         return self._schema._get_field(key) or self._fields.get(key)
 
+    def _set_default_value(self, key: str, value: Any) -> None:
+        """
+        Set a default value without performing any validation. The value is set and the field is
+        marked as having the initial default value.
+
+        :param key: field key
+        :param value: field default value
+        """
+        self._data[key] = value
+        self._default_value_keys.add(key)
+
     def _set_value(self, key: str, value: Any) -> Any:
-        '''
+        """
         Set a configuration value. This method passes the value through the field validation chain
         and then calls the target field's :meth:`~cincoconfig.abc.Field.__setval__` to actually
         set the value.
 
         Any exception that is raised by the field validation will be wrapped in an
         :class:`~cincoconfig.abc.ValidationError` and raised again.
 
         :param name: field key
         :param value: value to validate and set
         :raises ValidationError: setting the value failed
-        '''
+        """
         field = self._get_field(key)
         if not field:
             if not self._schema._dynamic:
                 raise AttributeError(key)
             field = self._fields[key] = AnyField()
             field.__setkey__(self._schema, key)
 
@@ -961,202 +1059,219 @@
                 value = field.validate(self, value)
             except ValidationError:
                 raise
             except Exception as err:
                 raise ValidationError(self, field, err) from err
             else:
                 field.__setval__(self, value)
+                self._default_value_keys.discard(key)
                 return value
 
         if isinstance(value, Config):
             value._parent = self
             value._key = key
         elif isinstance(value, dict) and isinstance(field, (Schema, ConfigTypeField)):
             # both Schema and ConfigTypeField implement __call__, which will return a Config object
             cfg = field(self)
             cfg._key = key
             cfg.load_tree(value)  # load_tree will raise a ValidationError on error
             value = cfg
         else:
-            raise ValidationError(self, field,
-                                  "Unable to coerce %s to Config" % type(value).__name__)
+            raise ValidationError(
+                self, field, "Unable to coerce %s to Config" % type(value).__name__
+            )
 
         self._data[key] = value
+        self._default_value_keys.discard(key)
         return value
 
     def __setattr__(self, name: str, value: Any) -> Any:
-        '''
+        """
         Validate a configuration value and set it.
 
         :param name: field key
         :param value: value
-        '''
+        """
         if name.startswith("_"):
             return object.__setattr__(self, name, value)
 
         return self._set_value(name, value)
 
     def __getattr__(self, name: str) -> Any:
-        '''
+        """
         Retrieve a config value.
 
         :param name: field key
-        '''
+        """
         return self._get_value(name)
 
     def _get_value(self, key: str) -> Any:
         field = self._get_field(key)
         if not field and not self._schema._dynamic:
             raise AttributeError(key)
 
         return field.__getval__(self) if field else None
 
     def __getitem__(self, key: str) -> Any:
-        '''
+        """
         :returns: field value, equivalent to ``getattr(config, key)``, however his method handles
             retrieving nested values. For example:
 
             .. code-block:: python
 
                 >>> schema = Schema()
                 >>> schema.x.y = IntField(default=10)
                 >>> config = schema()
                 >>> print(config['x.y'])
                 10
-        '''
-        key, _, subkey = key.partition('.')
+        """
+        key, _, subkey = key.partition(".")
         value = self._get_value(key)
         return value.__getitem__(subkey) if subkey else value
 
     def __iter__(self) -> Iterator[Tuple[str, Any]]:
+        # pylint: disable=superfluous-parens
         return ((key, self._get_value(key)) for key in self._data)
 
     def __setitem__(self, key: str, value: Any) -> Any:
-        '''
+        """
         Set a field value, equivalent to ``setattr(config, key)``, however this method handles
         setting nested values. For example:
 
         .. code-block:: python
 
             >>> schema = Schema()
             >>> schema.x.y = IntField(default=10)
             >>> config = schema()
             >>> config['x.y'] = 20
             >>> print(config.x.y)
             20
-        '''
-        key, _, subkey = key.partition('.')
+        """
+        key, _, subkey = key.partition(".")
         if subkey:
             return self._get_value(key).__setitem__(subkey, value)
 
         return self._set_value(key, value)
 
     def __contains__(self, key: str) -> bool:
-        '''
+        """
         Check if key is in the configuration. This method handles checking nested values. For
         example:
 
         .. code-block:: python
 
                 >>> schema = Schema()
                 >>> schema.x.y = IntField(default=10)
                 >>> config = schema()
                 >>> 'x.y' in config
                 True
-        '''
-        key, _, subkey = key.partition('.')
+        """
+        key, _, subkey = key.partition(".")
         if subkey:
             cfg = self._data.get(key)
             if isinstance(cfg, Config):
                 return cfg.__contains__(subkey)
             return False
 
         return key in self._data
 
     @property
     def full_path(self) -> str:
-        '''
+        """
         **(Deprecated, will be removed in v1.0.0)** get the full path to the configuration
         :returns: the full path to this configuration
-        '''
-        warnings.warn("Config.full_path is deprecated and will be removed in v1.0.0, use "
-                      "cincoconfig.item_ref_path() instead", DeprecationWarning)
+        """
+        warnings.warn(
+            "Config.full_path is deprecated and will be removed in v1.0.0, use "
+            "cincoconfig.item_ref_path() instead",
+            DeprecationWarning,
+        )
         return self._ref_path
 
     @property
     def _ref_path(self) -> str:
-        '''
+        """
         :returns: the full reference path to the configuration
-        '''
+        """
         if self._parent:
             root = self._parent._ref_path
         elif self._schema._schema:
             root = self._schema._schema._ref_path
         else:
-            root = ''
+            root = ""
 
         if root:
             path = root + "." + self._key
         else:
             path = self._key
 
         if self._container:
             try:
                 pos = self._container._get_item_position(self)
-            except:
-                pos = ''
+            except:  # noqa: E722
+                pos = ""
             else:
-                if pos not in ('', None):
+                if pos not in ("", None):
                     path += "[%s]" % pos
 
         return path
 
-    def save(self, filename: str, format: str):
-        '''
-        Save the configuration to a file.
+    def save(self, filename: str, format: str, **kwargs):
+        """
+        Save the configuration to a file. Additional keyword arguments are passed to :meth:`dumps`.
 
         :param filename: destination file path
         :param format: output format
-        '''
-        content = self.dumps(format)
+        :param: additional keyword arguments for :meth:`dumps`
+        """
+        content = self.dumps(format, **kwargs)
         filename = os.path.expanduser(filename)
-        with open(filename, 'wb') as file:
+        with open(filename, "wb") as file:
             file.write(content)
 
-    def dumps(self, format: str, virtual: bool = False, sensitive_mask: str = None,
-              **kwargs) -> bytes:
-        '''
+    def dumps(
+        self,
+        format: str,
+        virtual: bool = False,
+        sensitive_mask: Optional[str] = None,
+        **kwargs
+    ) -> bytes:
+        """
         Serialize the configuration to a string with the specified format.
 
         :param format: output format
         :param virtual: include virtual fields in the output
         :param sensitive_mask: replace secure values, see :meth:`to_tree`
         :param kwargs: additional keyword arguments to pass to the formatter's ``__init__()``
         :returns: serialized configuration file content
-        '''
+        """
         formatter = ConfigFormat.get(format, **kwargs)
-        return formatter.dumps(self, self.to_tree(virtual=virtual, sensitive_mask=sensitive_mask))
-
-    def to_tree(self, virtual: bool = False, sensitive_mask: str = None) -> dict:
-        '''
+        return formatter.dumps(
+            self, self.to_tree(virtual=virtual, sensitive_mask=sensitive_mask)
+        )
+
+    def to_tree(
+        self, virtual: bool = False, sensitive_mask: Optional[str] = None
+    ) -> dict:
+        """
         Convert the configuration values to a tree.
 
         The *sensitive_mask* parameter is an optional string that will replace sensitive values in
         the tree.
 
         - ``None`` (default) - include the value as-is in the tree
         - ``len(sensitive_mask) == 1`` (single character) - replace every character with the
           ``sensitive_mask`` character. ``value = sensitive_mask * len(value)``
-        - ``len(sensitive_mask) != 1`` (empty or multicharacter string) - replace the entire value
+        - ``len(sensitive_mask) != 1`` (empty or multi character string) - replace the entire value
           with the ``sensitive_mask``.
 
         :param virtual: include virtual field values in the tree
         :param sensitive_mask: mask secure values with a string
         :returns: the basic tree containing all set values
-        '''
+        """
         tree = {}
         fields: Dict[str, BaseField] = dict(self._schema._fields)
         fields.update(self._fields)
 
         for key, field in fields.items():
             is_virtual = virtual and isinstance(field, VirtualFieldMixin)
             if key not in self._data and not is_virtual:
@@ -1165,16 +1280,22 @@
             if isinstance(field, InstanceMethodFieldMixin):
                 continue
 
             field_value = field.__getval__(self)
             value: Any = None
 
             if isinstance(field_value, Config):
-                value = field_value.to_tree(virtual=virtual, sensitive_mask=sensitive_mask)
-            elif isinstance(field, Field) and field.sensitive and sensitive_mask is not None:
+                value = field_value.to_tree(
+                    virtual=virtual, sensitive_mask=sensitive_mask
+                )
+            elif (
+                isinstance(field, Field)
+                and field.sensitive
+                and sensitive_mask is not None
+            ):
                 if not field_value:
                     pass
                 elif len(sensitive_mask) == 1:
                     value = sensitive_mask * len(str(field_value))
                 else:
                     value = sensitive_mask
             elif isinstance(field, Field):
@@ -1186,23 +1307,27 @@
                     raise ValidationError(self, field, err) from err
 
             tree[key] = value
 
         return tree
 
     def load_tree(self, tree: dict, validate: bool = True) -> None:
-        '''
+        """
         Load a tree and then validate the values.
 
         :param tree: a basic value tree
-        '''
+        """
         for key, value in tree.items():
             field = self._get_field(key)
             if isinstance(field, Field):
-                if isinstance(field.env, str) and field.env and os.environ.get(field.env):
+                if (
+                    isinstance(field.env, str)
+                    and field.env
+                    and os.environ.get(field.env)
+                ):
                     continue
 
                 try:
                     value = field.to_python(self, value)
                 except ValidationError:
                     raise
                 except Exception as err:
@@ -1210,60 +1335,65 @@
 
             self._set_value(key, value)
 
         if validate:
             self.validate()
 
     def load(self, filename: str, format: str):
-        '''
+        """
         Load the configuration from a file.
 
         :param filename: source filename
         :param format: source format
-        '''
+        """
         filename = os.path.expanduser(filename)
-        with open(filename, 'rb') as file:
+        with open(filename, "rb") as file:
             content = file.read()
 
         return self.loads(content, format)
 
     def loads(self, content: Union[str, bytes], format: str, **kwargs):
-        '''
+        """
         Load a configuration from a str or bytes and process any
         :class:`~cincoconfig.IncludeField`.
 
         :param content: configuration content
         :param format: content format
         :param kwargs: additional keyword arguments to pass to the formatter's ``__init__()``
-        '''
+        """
         if isinstance(content, str):
             content = content.encode()
 
         format_factory = partial(ConfigFormat.get, format, **kwargs)
         formatter = format_factory()
 
         tree = formatter.loads(self, content)
         tree = self._process_includes(self._schema, tree, format_factory)
 
         self.load_tree(tree)
 
-    def _process_includes(self, schema: Schema, tree: dict,
-                          format_factory: 'TFormatFactory') -> dict:
-        '''
+    def _process_includes(
+        self, schema: Schema, tree: dict, format_factory: "TFormatFactory"
+    ) -> dict:
+        """
         Process include fields when loading when a configuration file. This method will load
         included fields for all ``IncludeField`` instances in the schema and all children schemas.
 
         :param schema: schema to load from
         :param tree: parsed tree
         :param format: config format
-        '''
-        sub_schemas = [(key, field) for key, field in schema._fields.items()
-                       if isinstance(field, Schema)]
+        """
+        sub_schemas = [
+            (key, field)
+            for key, field in schema._fields.items()
+            if isinstance(field, Schema)
+        ]
         includes: List[Tuple[str, IncludeFieldMixin]] = [
-            (key, field) for key, field in schema._fields.items()  # type: ignore
+            (key, field)
+            for key, field in schema._fields.items()  # type: ignore
             if isinstance(field, IncludeFieldMixin)
         ]
         for key, field in includes:
             # For each of the included field names, check if it has a value in the parsed tree
             # and, if it does, load the included file and combine it with the existing tree.
             filename = tree.get(key)
             if filename is None:
@@ -1272,124 +1402,138 @@
             # All included config files must have the same file format (you can't include XML from
             # a JSON file, for example).
             formatter = format_factory()
             tree = field.include(self, formatter, filename, tree)
 
         for key, sub_schema in sub_schemas:
             if tree.get(key):
-                tree[key] = self._process_includes(sub_schema, tree[key], format_factory)
+                tree[key] = self._process_includes(
+                    sub_schema, tree[key], format_factory
+                )
 
         return tree
 
     def validate(self, collect_errors: bool = False) -> List[ValidationError]:
-        '''
+        """
         Perform validation on the entire config.
-        '''
+        """
         return self._schema._validate(self, collect_errors=collect_errors)
 
-    def cmdline_args_override(self, args: Namespace, ignore: Union[str, List[str]] = None) -> None:
-        '''
+    def cmdline_args_override(
+        self, args: Namespace, ignore: Optional[Union[str, List[str]]] = None
+    ) -> None:
+        """
         **(Deprecated, will be removed in v1.0.0)** override configuration values from the command
         line arguments. Use :meth:`~cincoconfig.cmdline_args_override`.
 
         :param args: parsed arguments
         :param ignore: list of field keys to ignore
-        '''
+        """
         # pylint: disable=import-outside-toplevel, cyclic-import
         from .support import cmdline_args_override
-        warnings.warn("Schema.cmdline_args_override() is deprecated and will be removed in "
-                      "v1.0.0, use cincoconfig.cmdline_args_override() instead",
-                      DeprecationWarning)
+
+        warnings.warn(
+            "Schema.cmdline_args_override() is deprecated and will be removed in "
+            "v1.0.0, use cincoconfig.cmdline_args_override() instead",
+            DeprecationWarning,
+        )
         cmdline_args_override(self, args, ignore)
 
 
 class ConfigType(Config):
-    '''
+    """
     A base class for configuration types. A subclass of ``ConfigType`` is returned by the
     :meth:`~cincoconfig.make_type` function.
-    '''
-    __schema__ = None  # type: Schema
-    __key_filename__ = None  # type: str
+    """
 
-    def __init__(self, parent: Config = None, **kwargs):
-        '''
+    __schema__: ClassVar[Schema]
+    __key_filename__: ClassVar[Optional[str]] = None
+
+    def __init__(self, parent: Optional[Config] = None, **kwargs):
+        """
         :param parent: parent configuration
-        '''
-        super().__init__(self.__schema__, parent, key_filename=self.__key_filename__, **kwargs)
+        """
+        super().__init__(
+            self.__schema__, parent, key_filename=self.__key_filename__, **kwargs
+        )
 
     def __eq__(self, other: Any) -> bool:
         if other is None:
             return False
         if other.__class__ is not self.__class__:
             return False
 
         return self._data == other._data
 
 
 class ConfigFormat:
-    '''
+    """
     The base class for all configuration file formats.
-    '''
-    __registry: Dict[str, Type['ConfigFormat']] = {}
+    """
+
+    __registry: Dict[str, Type["ConfigFormat"]] = {}
     __initialized: bool = False
 
     @classmethod
-    def register(cls, name: str, format_cls: Type['ConfigFormat']) -> None:
-        '''
+    def register(cls, name: str, format_cls: Type["ConfigFormat"]) -> None:
+        """
         Register a new configuration format.
 
         :param name: format name
         :param format_cls: ``ConfigFormat`` subclass to register
-        '''
+        """
         cls.__registry[name] = format_cls
 
     @classmethod
-    def get(cls, name: str, **kwargs) -> 'ConfigFormat':
-        '''
+    def get(cls, name: str, **kwargs) -> "ConfigFormat":
+        """
         Get a registered configuration format.
 
         :param name: config format name
         :param kwargs: keyword arguments to pass into the config format ``__init__()`` method
         :returns: the config format instance
-        '''
+        """
         if not cls.__initialized:
             cls.initialize_registry()
 
         format_cls = cls.__registry[name]
         return format_cls(**kwargs)  # type: ignore
 
     @classmethod
     def initialize_registry(cls) -> None:
-        '''
+        """
         Initialize the format registry for built-in formats.
-        '''
+        """
         if cls.__initialized:
             return
 
-        from .formats import FORMATS  # pylint: disable=cyclic-import, import-outside-toplevel
+        from .formats import (
+            FORMATS,
+        )
+
         for name, format_cls in FORMATS:
             cls.__registry[name] = format_cls
 
         cls.__initialized = True
 
     def dumps(self, config: Config, tree: dict) -> bytes:
-        '''
+        """
         Convert the configuration value tree to a bytes object. This method is called to serialize
         the configuration to a buffer and eventually write to a file.
 
         :param config: current configuration
         :param tree: basic value tree, as returned by the Config
             :meth:`~cincoconfig.core.Config.to_tree` method.
         :returns: the serialized configuration
-        '''
+        """
         raise NotImplementedError()
 
     def loads(self, config: Config, content: bytes) -> dict:
-        '''
+        """
         Parse the serialized configuration to a basic value tree that can be parsed by the
         Config :meth:`~cincoconfig.core.Config.load_tree` method.
 
         :param config: current config
         :param content: serialized content
         :returns: the parsed basic value tree
-        '''
+        """
         raise NotImplementedError()
```

### Comparing `cincoconfig-0.8.0/cincoconfig/encryption.py` & `cincoconfig-0.9.0/cincoconfig/encryption.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 #
 # Copyright (C) 2021 Adam Meily
 #
 # This file is subject to the terms and conditions defined in the file 'LICENSE', which is part of
 # this source code package.
 #
-'''
+"""
 Encryption classes and methods.
-'''
+"""
+
+# spell-checker:ignore padder bindata
 import os
 from itertools import cycle
-from typing import NamedTuple, Optional, Union, Tuple
+from typing import NamedTuple, Optional, Tuple, Union
 
 try:
-    from cryptography.hazmat.primitives.ciphers import Cipher, algorithms, modes
-    from cryptography.hazmat.primitives import padding
     from cryptography.hazmat.backends import default_backend
+    from cryptography.hazmat.primitives import padding
+    from cryptography.hazmat.primitives.ciphers import Cipher, algorithms, modes
 except ImportError:  # pragma: no cover
     AES_AVAILABLE = False
 else:
     #: AES is available (``cryptography`` is installed)
     AES_AVAILABLE = True
 
 
@@ -29,58 +31,58 @@
 #:
 #:  the encryption method (:class:`str`)
 #:
 #: .. py:attribute:: ciphertext
 #:
 #:  the encrypted value (:class:`bytes`)
 #:
-SecureValue = NamedTuple('SecureValue', [('method', str), ('ciphertext', bytes)])
+SecureValue = NamedTuple("SecureValue", [("method", str), ("ciphertext", bytes)])
 
 
 class EncryptionError(Exception):
-    '''
+    """
     Exception raised whenever an error occurs during a encryption operation.
-    '''
+    """
 
 
 class IEncryptionProvider:
-    '''
+    """
     Interface class for an encryption algorithm provider. An encryption provider
     implements both encryption and decryption of string values.
 
     The encrypt and decrypt methods must be deterministic.
 
     .. code-block:: python
 
         b'message' == provider.decrypt(provider.decrypt(b'message'))
 
     The constructor for subclasses will receive a single argument: the encryption key.
-    '''
+    """
 
     def encrypt(self, text: bytes) -> bytes:
-        '''
+        """
         Encrypt a value.
 
         :param text: plain text value to encrypt
         :returns: encrypted value
-        '''
+        """
         raise NotImplementedError()
 
     def decrypt(self, ciphertext: bytes) -> bytes:
-        '''
+        """
         Decrypt a value.
 
         :param ciphertext: encrypted value to decrypt
         :returns: decrypted value
-        '''
+        """
         raise NotImplementedError()
 
 
 class KeyFile:
-    '''
+    """
     The cincoconfig key file, containing a randomly generated 32 byte encryption key. The cinco
     key file is used by :class:`~cincoconfig.SecureField` to encrypt and decrypt values as
     they are written to and read from the configuration file.
 
     The keyfile is loaded as needed by using this class as a context manager. The key has an
     internal reference count and is only freed once the reference count is 0 (all context managers
     exited). THe key is cached internally so that the keyfile only has to be open and read once
@@ -88,191 +90,197 @@
 
     To encrypt a value:
 
     .. code-block:: python
 
         with keyfile as ctx:
             secret = ctx.encrypt(method='xor', text='hello, world')
-    '''
+    """
 
     def __init__(self, filename: str):
-        '''
+        """
         :param filename: the cinco key filename
-        '''
+        """
         self.filename = filename
-        self.__key = None  # type: Optional[bytes]
+        self.__key: Optional[bytes] = None
         self.__refcount = 0
 
     def __load_key(self) -> None:
-        '''
+        """
         INTERNAL METHOD. Load configuration key.
-        '''
+        """
         filename = os.path.expanduser(self.filename)
         try:
-            with open(filename, 'rb') as fp:
+            with open(filename, "rb") as fp:
                 self.__key = fp.read()
         except OSError:
             self.__key = self.__generate_key()
         else:
             self._validate_key()
 
     def __generate_key(self) -> bytes:
-        '''
+        """
         Generate a random 32 byte key and save it to ``filename``.
 
         :returns: the generated key
-        '''
+        """
         key = os.urandom(32)
         filename = os.path.expanduser(self.filename)
-        with open(filename, 'wb') as fp:
+        with open(filename, "wb") as fp:
             fp.write(key)
         return key
 
     def generate_key(self) -> None:
-        '''
+        """
         Generate a random 32 byte key and save it to ``filename``.
-        '''
+        """
         # We generate the key but don't return the value in the public API so that we don't leak
         # the key outside of a with context.
         self.__generate_key()
 
     def _validate_key(self) -> None:
-        '''
+        """
         Validate the key.
 
         :raises EncryptionError: invalid key
-        '''
+        """
         if not self.__key or len(self.__key) != 32:
-            raise EncryptionError('invalid encryption key file: %s' % self.filename)
+            raise EncryptionError("invalid encryption key file: %s" % self.filename)
 
-    def __enter__(self) -> 'KeyFile':
+    def __enter__(self) -> "KeyFile":
         if not self.__key:
             self.__load_key()
 
         self.__refcount += 1
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.__refcount -= 1
         if self.__refcount == 0:
             self.__key = None
 
         return False
 
     def _get_provider(self, method: str) -> Tuple[IEncryptionProvider, str]:
-        '''
+        """
         Get the encryption provider. ``method`` must be one of
 
         - ``aes`` - returns :class:`AesProvider`
         - ``xor`` - returns :class:`XorProvider`
         - ``best`` - returns the best available encryption provider: :class:`AesProvider` if AES
           encryption is available (``cryptography`` is installed), :class:`XorProvider` if AES
           is not available
 
         The resolved method is returned. For example, if ``best`` if specified, the best encryption
         method will be resolved and returned.
 
         The return value is a tuple of encryption provider instance and the resolved method.
 
         :returns: a tuple of ``(provider, method)``
-        '''
+        """
         if not self.__key:
-            raise TypeError('keyfile is not open')
+            raise TypeError("keyfile is not open")
 
-        if method == 'aes' or (method == 'best' and AES_AVAILABLE):
-            return AesProvider(self.__key), 'aes'
-        if method in ('xor', 'best'):
-            return XorProvider(self.__key), 'xor'
-        raise TypeError('invalid encryption method: %s' % method)
+        if method == "aes" or (method == "best" and AES_AVAILABLE):
+            return AesProvider(self.__key), "aes"
+        if method in ("xor", "best"):
+            return XorProvider(self.__key), "xor"
+        raise TypeError("invalid encryption method: %s" % method)
 
-    def encrypt(self, text: Union[str, bytes], method: str = 'best') -> SecureValue:
-        '''
+    def encrypt(self, text: Union[str, bytes], method: str = "best") -> SecureValue:
+        """
         :param text: plaintext to encrypt
         :param method: encryption method to use
         :returns: the encrypted value
-        '''
+        """
         if not self.__key:
-            raise TypeError('key file is not open')
+            raise TypeError("key file is not open")
 
         bindata = text.encode() if isinstance(text, str) else text
 
         provider, method = self._get_provider(method)
         ciphertext = provider.encrypt(bindata)
         return SecureValue(method, ciphertext)
 
     def decrypt(self, secret: SecureValue) -> bytes:
-        '''
+        """
         :param secret: encrypted value
         :returns: decrypted value
-        '''
+        """
         if not self.__key:
-            raise TypeError('key file is not open')
+            raise TypeError("key file is not open")
 
         provider, _ = self._get_provider(secret.method)
         return provider.decrypt(secret.ciphertext)
 
 
 class XorProvider(IEncryptionProvider):
-    '''
+    """
     XOR-bitwise "encryption". The XOR provider should only be used to obfuscate, not encrypt, a
     value since XOR operations can be easily reversed.
-    '''
+    """
 
     def __init__(self, key: bytes):
         self.__key = key
 
     def encrypt(self, text: Union[str, bytes]) -> bytes:
-        '''
+        """
         :returns: the encrypted value
-        '''
+        """
         bindata = text.encode() if isinstance(text, str) else text
         buff = bytearray(bindata)
         for i, c in zip(range(len(buff)), cycle(self.__key)):
             buff[i] ^= c
         return bytes(buff)
 
     def decrypt(self, ciphertext: bytes) -> bytes:
-        '''
+        """
         :returns: the decrypted values
-        '''
+        """
         return self.encrypt(ciphertext)
 
 
 class AesProvider(IEncryptionProvider):
-    '''
+    """
     AES-256 encryption provider. This class requires the ``cryptography`` library. Each encrypted
     value has a randomly generated 16-byte IV.
-    '''
+    """
 
     def __init__(self, key: bytes):
         if not AES_AVAILABLE:
-            raise TypeError('AES encryption is not available; please install cryptography')
+            raise TypeError(
+                "AES encryption is not available; please install cryptography"
+            )
         self.__key = key
 
     def decrypt(self, ciphertext: bytes) -> bytes:
-        '''
+        """
         :returns: the plaintext value
-        '''
+        """
         if not ciphertext or len(ciphertext) < 32:
-            raise EncryptionError('invalid initialization vector')
+            raise EncryptionError("invalid initialization vector")
 
         iv = ciphertext[:16]
         ciphertext = ciphertext[16:]
-        cipher = Cipher(algorithms.AES(self.__key), modes.CBC(iv), backend=default_backend())
+        cipher = Cipher(
+            algorithms.AES(self.__key), modes.CBC(iv), backend=default_backend()
+        )
         decryptor = cipher.decryptor()
 
         unpadder = padding.PKCS7(128).unpadder()
         text = decryptor.update(ciphertext) + decryptor.finalize()
 
         return unpadder.update(text) + unpadder.finalize()
 
     def encrypt(self, text: bytes) -> bytes:
-        '''
+        """
         :returns: the encrypted value
-        '''
+        """
         iv = os.urandom(16)
-        cipher = Cipher(algorithms.AES(self.__key), modes.CBC(iv), backend=default_backend())
+        cipher = Cipher(
+            algorithms.AES(self.__key), modes.CBC(iv), backend=default_backend()
+        )
         encryptor = cipher.encryptor()
         padder = padding.PKCS7(128).padder()
 
         padded = padder.update(text) + padder.finalize()
         return iv + encryptor.update(padded) + encryptor.finalize()
```

### Comparing `cincoconfig-0.8.0/cincoconfig/fields/__init__.py` & `cincoconfig-0.9.0/cincoconfig/fields/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,53 @@
 #
 # Copyright (C) 2021 Adam Meily
 #
 # This file is subject to the terms and conditions defined in the file 'LICENSE', which is part of
 # this source code package.
 #
-'''
+"""
 Cinco Config Fields.
-'''
+"""
+# ruff: noqa: F401
+
 from .bool_field import BoolField, FeatureFlagField
 from .bytes_field import BytesField
-from .dict_field import DictField
+from .dict_field import DictField, DictProxy
 from .file_field import FilenameField
 from .include_field import IncludeField
 from .instance_method_field import InstanceMethodField, instance_method
 from .list_field import ListField, ListProxy
-from .net_field import IPv4AddressField, IPv4NetworkField, PortField, HostnameField
-from .number_field import IntField, NumberField, FloatField
-from .secure_field import SecureField, SecureValue, DigestValue, ChallengeField
-from .string_field import StringField, ApplicationModeField, LogLevelField
+from .net_field import HostnameField, IPv4AddressField, IPv4NetworkField, PortField
+from .number_field import FloatField, IntField, NumberField
+from .secure_field import ChallengeField, DigestValue, SecureField, SecureValue
+from .string_field import ApplicationModeField, LogLevelField, StringField
 from .url_field import UrlField
 from .virtual_field import VirtualField
 
-__all__ = ('StringField', 'IntField', 'FloatField', 'PortField', 'IPv4AddressField',
-           'IPv4NetworkField', 'FilenameField', 'BoolField', 'UrlField', 'ListField',
-           'HostnameField', 'DictField', 'ListProxy', 'VirtualField', 'ApplicationModeField',
-           'LogLevelField', 'NumberField', 'ChallengeField', 'DigestValue', 'SecureField',
-           'BytesField', 'IncludeField', 'InstanceMethodField', 'instance_method',
-           'FeatureFlagField')
+__all__ = (
+    "StringField",
+    "IntField",
+    "FloatField",
+    "PortField",
+    "IPv4AddressField",
+    "IPv4NetworkField",
+    "FilenameField",
+    "BoolField",
+    "UrlField",
+    "ListField",
+    "HostnameField",
+    "DictField",
+    "ListProxy",
+    "VirtualField",
+    "ApplicationModeField",
+    "LogLevelField",
+    "NumberField",
+    "ChallengeField",
+    "DigestValue",
+    "SecureField",
+    "BytesField",
+    "IncludeField",
+    "InstanceMethodField",
+    "instance_method",
+    "FeatureFlagField",
+    "DictProxy",
+)
```

### Comparing `cincoconfig-0.8.0/cincoconfig/fields/bool_field.py` & `cincoconfig-0.9.0/cincoconfig/fields/bool_field.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,54 +1,55 @@
 #
 # Copyright (C) 2021 Adam Meily
 #
 # This file is subject to the terms and conditions defined in the file 'LICENSE', which is part of
 # this source code package.
 #
-'''
+"""
 Boolean field.
-'''
-from ..core import Field, Config, FeatureFlagFieldMixin
+"""
+from ..core import Config, FeatureFlagFieldMixin, Field
 
 
 class BoolField(Field):
-    '''
+    """
     A boolean field.
-    '''
+    """
+
     storage_type = bool
     #: Accepted values that evaluate to ``True``
-    TRUE_VALUES = ('t', 'true', '1', 'on', 'yes', 'y')
+    TRUE_VALUES = ("t", "true", "1", "on", "yes", "y")
     #: Accepted values that evaluate to ``False``
-    FALSE_VALUES = ('f', 'false', '0', 'off', 'no', 'n')
+    FALSE_VALUES = ("f", "false", "0", "off", "no", "n")
 
     def _validate(self, cfg: Config, value: str) -> bool:
-        '''
+        """
         Validate a value.
 
         :param cfg: current config
         :param value: value to validate
-        '''
+        """
 
         if isinstance(value, bool):
             bool_val = value
         elif isinstance(value, (int, float)):
             bool_val = bool(value)
         elif isinstance(value, str):
             if value.lower() in self.TRUE_VALUES:
                 bool_val = True
             elif value.lower() in self.FALSE_VALUES:
                 bool_val = False
             else:
-                raise ValueError('value is not a valid boolean')
+                raise ValueError("value is not a valid boolean")
         else:
-            raise ValueError('value is not a valid boolean')
+            raise ValueError("value is not a valid boolean")
         return bool_val
 
 
 class FeatureFlagField(BoolField, FeatureFlagFieldMixin):
-    '''
+    """
     Concrete implementation of the feature flag field. When this field's value is set to ``False``,
     the bound configurations will not perform validation.
-    '''
+    """
 
-    def is_feature_enabled(self, cfg: 'Config') -> bool:
+    def is_feature_enabled(self, cfg: "Config") -> bool:
         return self.__getval__(cfg)
```

### Comparing `cincoconfig-0.8.0/cincoconfig/fields/bytes_field.py` & `cincoconfig-0.9.0/cincoconfig/fields/bytes_field.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,85 +1,86 @@
 #
 # Copyright (C) 2021 Adam Meily
 #
 # This file is subject to the terms and conditions defined in the file 'LICENSE', which is part of
 # this source code package.
 #
-'''
+"""
 Bytes field.
-'''
-from typing import Any, Optional
+"""
 import base64
 import binascii
+from typing import Any, Optional
 
-from ..core import Field, Config
+from ..core import Config, Field
 
 
 class BytesField(Field):
-    '''
+    """
     Store binary data in an encoded string.
-    '''
+    """
+
     storage_type = bytes
     #: Available encodings: base64 and hex
-    ENCODINGS = ('base64', 'hex')
+    ENCODINGS = ("base64", "hex")
 
-    def __init__(self, encoding: str = 'base64', **kwargs):
-        '''
+    def __init__(self, encoding: str = "base64", **kwargs):
+        """
         :param encoding: binary data encoding, must be one of :attr:`ENCODINGS`
-        '''
+        """
         super().__init__(**kwargs)
 
         if encoding not in BytesField.ENCODINGS:
-            raise TypeError('invalid encoding: %s' % encoding)
+            raise TypeError("invalid encoding: %s" % encoding)
         self.encoding = encoding
 
     def _validate(self, cfg: Config, value: Any) -> bytes:
         if isinstance(value, str):
             return value.encode()
 
         if isinstance(value, bytes):
             return value
 
-        raise ValueError('value must be bytes, not %s' % type(value).__name__)
+        raise ValueError("value must be bytes, not %s" % type(value).__name__)
 
     def to_basic(self, cfg: Config, value: bytes) -> str:
-        '''
+        """
         :returns: the encoded binary data
-        '''
+        """
         if value is None:
             return value
 
-        if self.encoding == 'base64':
+        if self.encoding == "base64":
             return base64.b64encode(value).decode()
 
-        if self.encoding == 'hex':
+        if self.encoding == "hex":
             return value.hex()
 
-        raise TypeError('invalid encoding: %s' % self.encoding)
+        raise TypeError("invalid encoding: %s" % self.encoding)
 
     def to_python(self, cfg: Config, value: Any) -> Optional[bytes]:
-        '''
+        """
         :returns: the decoded binary data
-        '''
+        """
         if value is None:
             return value
 
         if not isinstance(value, str):
-            raise ValueError('value is not a string')
+            raise ValueError("value is not a string")
 
-        if self.encoding == 'base64':
+        if self.encoding == "base64":
             try:
                 ret = base64.b64decode(value)
             except binascii.Error as err:
-                raise ValueError('invalid base64 encoding') from err
+                raise ValueError("invalid base64 encoding") from err
             else:
                 return ret
 
-        if self.encoding == 'hex':
+        if self.encoding == "hex":
             try:
                 ret = bytes.fromhex(value)
             except ValueError as err:
-                raise ValueError('invalid hex encoding') from err
+                raise ValueError("invalid hex encoding") from err
             else:
                 return ret
 
-        raise TypeError('invalid encoding: %s' % self.encoding)
+        raise TypeError("invalid encoding: %s" % self.encoding)
```

### Comparing `cincoconfig-0.8.0/cincoconfig/fields/file_field.py` & `cincoconfig-0.9.0/cincoconfig/fields/file_field.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,75 +1,88 @@
 #
 # Copyright (C) 2021 Adam Meily
 #
 # This file is subject to the terms and conditions defined in the file 'LICENSE', which is part of
 # this source code package.
 #
-'''
+"""
 File field.
-'''
+"""
 import os
-from typing import Union
+from typing import Optional, Union
 
-from .string_field import StringField
 from ..core import Config
+from .string_field import StringField
 
 
 class FilenameField(StringField):
-    '''
+    """
     A field for representing a filename on disk.
-    '''
+    """
+
     storage_type = str
 
-    def __init__(self, *, exists: Union[bool, str] = None, startdir: str = None, **kwargs):
-        '''
+    def __init__(
+        self,
+        *,
+        exists: Optional[Union[bool, str]] = None,
+        startdir: Optional[str] = None,
+        **kwargs
+    ):
+        """
         The *exists* parameter can be set to one of the following values:
 
         - ``None`` - don't check file's existence
         - ``False`` - validate that the filename does not exist
         - ``True`` - validate that the filename does exist
         - ``"dir"`` - validate that the filename is a directory that exists
         - ``"file"`` - validate that the filename is a file that exists
 
         The *startdir* parameter, if specified, will resolve filenames starting from a directory
-        and will cause all filenames to be validate to their abslute file path. If not specified,
+        and will cause all filenames to be validate to their absolute file path. If not specified,
         filename's will be resolve relative to :meth:`os.getcwd` and the relative file path will
         be validated.
 
         :param exists: validate the filename's existence on disk
         :param startdir: resolve relative paths to a start directory
-        '''
+        """
         super().__init__(**kwargs)
         self.exists = exists
         self.startdir = startdir
 
     def _validate(self, cfg: Config, value: str) -> str:
-        '''
+        """
         Validate a value.
 
         :param cfg: current config
         :param value: value to validate
-        '''
+        """
         value = super()._validate(cfg, value)
 
         if not value:
             return value
 
         if not os.path.isabs(value) and self.startdir:
-            value = os.path.abspath(os.path.expanduser(os.path.join(self.startdir, value)))
+            value = os.path.abspath(
+                os.path.expanduser(os.path.join(self.startdir, value))
+            )
 
-        if os.path.sep == '\\':
-            value = value.replace('/', '\\')
+        if os.path.sep == "\\":
+            value = value.replace("/", "\\")
 
         value_exists = os.path.exists(value)
         if self.exists is True and not value_exists:
-            raise ValueError('file or directory does not exist: %s' % value)
+            raise ValueError("file or directory does not exist: %s" % value)
         if self.exists is False and value_exists:
-            raise ValueError('file or directory already exists: %s' % value)
-        if self.exists == 'dir' and not os.path.isdir(value):
-            raise ValueError('directory %s: %s' %
-                             ('already exists' if value_exists else 'does not exist', value))
-        if self.exists == 'file' and not os.path.isfile(value):
-            raise ValueError('file %s: %s' %
-                             ('already exists' if value_exists else 'does not exist', value))
+            raise ValueError("file or directory already exists: %s" % value)
+        if self.exists == "dir" and not os.path.isdir(value):
+            raise ValueError(
+                "directory %s: %s"
+                % ("already exists" if value_exists else "does not exist", value)
+            )
+        if self.exists == "file" and not os.path.isfile(value):
+            raise ValueError(
+                "file %s: %s"
+                % ("already exists" if value_exists else "does not exist", value)
+            )
 
         return value
```

### Comparing `cincoconfig-0.8.0/cincoconfig/fields/instance_method_field.py` & `cincoconfig-0.9.0/cincoconfig/fields/instance_method_field.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,66 +1,69 @@
 #
 # Copyright (C) 2021 Adam Meily
 #
 # This file is subject to the terms and conditions defined in the file 'LICENSE', which is part of
 # this source code package.
 #
-'''
+"""
 Instance method
-'''
-from typing import Any, Callable
+"""
 from functools import wraps
-from ..core import Field, Config, InstanceMethodFieldMixin, Schema
+from typing import Any, Callable
+
+from ..core import Config, Field, InstanceMethodFieldMixin, Schema
 
 
 class InstanceMethodField(Field, InstanceMethodFieldMixin):
-    '''
+    """
     A configuration instance method.
-    '''
+    """
+
     storage_type = Callable
 
     def __init__(self, method: Callable[[Config], Any], **kwargs):
-        if kwargs.get('default') is not None:
-            raise TypeError('instance methods cannot have a default value')
+        if kwargs.get("default") is not None:
+            raise TypeError("instance methods cannot have a default value")
 
         super().__init__(**kwargs)
         self.method = method
 
     def __setdefault__(self, cfg: Config) -> None:
-        '''
+        """
         Bind the instance method to the configuration. This is a performance enhancement since the
         bound method, created in :meth:`_bind`, is config specific and this method will cache the
         result in the configuration.
 
         :param cfg: configuration
-        '''
+        """
         object.__setattr__(cfg, self._key, self._bind(cfg))
 
     def _bind(self, cfg: Config) -> Callable:
-        '''
+        """
         Create a bound instance method on the configuration.
 
         :param cfg: configuration
         :returns: the bound method
-        '''
+        """
+
         @wraps(self.method)
         def wrapper(*args, **kwargs) -> Any:
             return self.method(cfg, *args, **kwargs)  # type: ignore
 
         return wrapper
 
     def validate(self, cfg: Config, value: Any) -> Any:
         return value
 
     def __setval__(self, cfg: Config, value: Any) -> None:
-        raise TypeError('field is readonly')
+        raise TypeError("field is readonly")
 
 
 def instance_method(schema: Schema, name: str) -> Callable:
-    '''
+    """
     Bind a function to a schema as an instance method. Use this as a decorator:
 
     .. code-block:: python
 
         schema = Schema()
 
         @instance_method(schema, "say_hello")
@@ -68,12 +71,14 @@
             return "Hello, world!"
 
         config = schema()
         print(config.say_hello())  # "Hello, world!"
 
     :param schema: schema
     :param name: instance method name
-    '''
+    """
+
     def wrapper(func: Callable[[Config], Any]) -> Callable[[Config], Any]:
         schema._add_field(name, InstanceMethodField(method=func))
         return func
+
     return wrapper
```

### Comparing `cincoconfig-0.8.0/cincoconfig/fields/list_field.py` & `cincoconfig-0.9.0/cincoconfig/fields/list_field.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,197 +1,216 @@
 #
 # Copyright (C) 2021 Adam Meily
 #
 # This file is subject to the terms and conditions defined in the file 'LICENSE', which is part of
 # this source code package.
 #
-'''
+"""
 List field
-'''
+"""
 import inspect
-from typing import Iterable, TypeVar, Type, Union, Any, List
-from ..core import (ContainerValueMixin, Field, Config, BaseField, Schema, isconfigtype, AnyField,
-                    ConfigType)
+from typing import Any, Iterable, List, Optional, Type, Union
 
-
-_T = TypeVar('_T')
+from ..core import (
+    AnyField,
+    BaseField,
+    Config,
+    ConfigType,
+    ContainerValueMixin,
+    Field,
+    Schema,
+    isconfigtype,
+)
 
 
 class ListProxy(list, ContainerValueMixin):
-    '''
+    """
     A Field-validated :class:`list` proxy. This proxy supports all methods that the builtin
     ``list`` supports with the added ability to validate items against a :class:`Field`. This is
     the field returned by the :class:`ListField` validation chain.
-    '''
+    """
 
-    def __init__(self, cfg: Config, list_field: 'ListField', iterable: Iterable[_T] = None):
+    def __init__(
+        self, cfg: Config, list_field: "ListField", iterable: Optional[Iterable] = None
+    ):
         iterable = iterable or []
         self.cfg = cfg
         self.list_field = list_field
         if not self.list_field.field:
-            raise TypeError('ListProxy requires a parent ListField.field attribute')
+            raise TypeError("ListProxy requires a parent ListField.field attribute")
 
         if isinstance(iterable, ListProxy) and iterable.item_field is list_field.field:
             super().__init__(iterable)
         else:
-            super().__init__(self._validate(item)
-                             for index, item in enumerate(iterable))
+            super().__init__(
+                self._validate(item) for index, item in enumerate(iterable)
+            )
 
     @property
     def item_field(self) -> Union[BaseField, Type[Config]]:
-        '''
+        """
         :returns: the field for each item stored in the list.
-        '''
+        """
         return self.list_field.field  # type: ignore
 
-    def append(self, item: _T) -> None:
+    def append(self, item: Any) -> None:
         super().append(self._validate(item))
 
-    def extend(self, iterable: Iterable[_T]) -> None:
+    def extend(self, iterable: Iterable) -> None:
         if isinstance(iterable, ListProxy) and iterable.item_field is self.item_field:
             super().extend(iterable)
         else:
             super().extend(self._validate(item) for item in iterable)
 
-    def insert(self, index: int, item: _T) -> None:
+    def insert(self, index: int, item: Any) -> None:
         super().insert(index, self._validate(item))
 
-    def copy(self) -> 'ListProxy':
+    def copy(self) -> "ListProxy":
         return ListProxy(self.cfg, self.list_field, self)
 
-    def __iadd__(self, iterable: Iterable[_T]) -> 'ListProxy':
+    def __iadd__(self, iterable: Iterable) -> "ListProxy":
         self.extend(iterable)
         return self
 
-    def __add__(self, iterable: Iterable[_T]) -> 'ListProxy':
+    def __add__(self, iterable: Iterable) -> "ListProxy":
         ret = self.copy()
         ret.extend(iterable)
         return ret
 
-    def __setitem__(self, index: Union[int, slice],  # type: ignore[override]
-                    item: Union[_T, Iterable[_T]]) -> None:
+    def __setitem__(
+        self,
+        index: Union[int, slice],  # type: ignore[override]
+        item: Union[Any, Iterable],
+    ) -> None:
         if isinstance(index, slice) and isinstance(item, (list, tuple)):
             super().__setitem__(index, [self._validate(i) for i in item])
         elif isinstance(index, int):
             super().__setitem__(index, self._validate(item))
 
     def _validate(self, value: Any) -> Any:
-        '''
+        """
         Validate a value.
 
         :param value: value to validate
         :returns: the validated value
-        '''
+        """
         if isinstance(self.item_field, Schema) or isconfigtype(self.item_field):
             if isinstance(value, dict):
                 cfg = self.item_field()  # type: ignore
                 cfg._container = self
                 cfg._key = self.list_field._key
                 cfg._parent = self.cfg
                 cfg.load_tree(value)  # type: ignore
             elif isinstance(value, Config):
                 value._parent = self.cfg
                 value._key = self.list_field._key
                 value._container = self
                 value.validate()
                 cfg = value
             else:
-                raise ValueError('invalid configuration object')
+                raise ValueError("invalid configuration object")
 
             return cfg
 
         if isinstance(self.item_field, Field):
             return self.item_field.validate(self.cfg, value)
 
         # we should only hit this when item_field is not a field, schema, or ConfigType subclass
         # (which shouldn't happen)
-        raise TypeError('item field must be a Field, Schema, or ConfigType subclass: %s' %
-                        self.item_field)
+        raise TypeError(
+            "item field must be a Field, Schema, or ConfigType subclass: %s"
+            % self.item_field
+        )
 
     def _get_item_position(self, item: Any) -> str:
         try:
             return str(self.index(item))
-        except:
+        except:  # noqa: E722
             return str(len(self))
 
 
 class ListField(Field):
-    '''
+    """
     A list field that can optionally validate items against a ``Field``. If a field is specified,
     a :class:`ListProxy` will be returned by the ``_validate`` method, which handles individual
     item validation.
 
     Specifying *required=True* will cause the field validation to validate that the list is not
     ``None`` and is not empty.
-    '''
+    """
+
     storage_type = List
 
-    def __init__(self, field: Union[BaseField, Type[ConfigType]] = None, **kwargs):
-        '''
+    def __init__(
+        self, field: Optional[Union[BaseField, Type[ConfigType]]] = None, **kwargs
+    ):
+        """
         :param field: Field to validate values against
-        '''
+        """
         super().__init__(**kwargs)
         self.field = field
 
         if field:
             if isinstance(field, Field):
                 self.storage_type = List[field.storage_type]  # type: ignore
             elif inspect.isclass(field):
                 self.storage_type = List[field]  # type: ignore
             else:
                 self.storage_type = List[type(field)]  # type: ignore
 
     def __setdefault__(self, cfg: Config) -> None:
         default = self.default
-        if isinstance(default, list) and self.field:
-            default = ListProxy(cfg, self, default)
-
-        cfg._data[self._key] = default
+        if isinstance(default, list):
+            if self.field:
+                default = ListProxy(cfg, self, default)
+            else:
+                default = list(default)
+        cfg._set_default_value(self._key, default)
 
     def _validate(self, cfg: Config, value: list) -> Union[list, ListProxy]:
-        '''
+        """
         Validate the value.
 
         :param cfg: current config
         :param value: value to validate
         :returns: a :class:`list` if not field is specified, a :class:`ListProxy` otherwise
-        '''
+        """
         if not isinstance(value, (list, tuple)):
-            raise ValueError('value is not a list')
+            raise ValueError("value is not a list")
 
         if self.required and not value:
-            raise ValueError('value is required')
+            raise ValueError("value is required")
 
         if not self.field or isinstance(self.field, AnyField):
             return value
 
         proxy = ListProxy(cfg, self, value)
         return proxy
 
     def to_basic(self, cfg: Config, value: Union[list, ListProxy]) -> list:
-        '''
+        """
         Convert to basic type.
 
         :param cfg: current config
         :param value: value to convert
-        '''
+        """
         if value is None:
             return value
         if not value:
             return []
 
         if isinstance(self.field, Schema) or isconfigtype(self.field):
             return [item.to_tree() for item in value]
         if isinstance(self.field, Field):
             return [self.field.to_basic(cfg, item) for item in value]
         return list(value)
 
     def to_python(self, cfg: Config, value: list) -> Union[list, ListProxy]:
-        '''
+        """
         Convert to Pythonic type.
 
         :param cfg: current config
         :param value: basic type value
-        '''
+        """
         if self.field is None or isinstance(self.field, AnyField):
             return value
         return ListProxy(cfg, self, value)
```

### Comparing `cincoconfig-0.8.0/cincoconfig/fields/number_field.py` & `cincoconfig-0.9.0/cincoconfig/fields/number_field.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,77 +1,93 @@
 #
 # Copyright (C) 2021 Adam Meily
 #
 # This file is subject to the terms and conditions defined in the file 'LICENSE', which is part of
 # this source code package.
 #
-'''
+"""
 Number fields
-'''
-from typing import Union
+"""
+from typing import Optional, Union
 
-from ..core import Field, Config
+from ..core import Config, Field
 
 
 class NumberField(Field):
-    '''
+    """
     Base class for all number fields. This field should not be used directly, instead consider
     using :class:`~cincoconfig.IntField` or :class:`~cincoconfig.FloatField`.
-    '''
+    """
 
-    def __init__(self, type_cls: type, *, min: Union[int, float] = None,
-                 max: Union[int, float] = None, **kwargs):
-        '''
+    def __init__(
+        self,
+        type_cls: type,
+        *,
+        min: Optional[Union[int, float]] = None,
+        max: Optional[Union[int, float]] = None,
+        **kwargs
+    ):
+        """
         :param type_cls: number type class that values will be converted to
         :param min: minimum value (inclusive)
         :param max: maximum value (inclusive)
-        '''
+        """
         super().__init__(**kwargs)
         self.type_cls = type_cls
         self.min = min
         self.max = max
         self.storage_type = type_cls
 
-    def _validate(self, cfg: Config, value: Union[str, int, float]) -> Union[int, float]:
-        '''
+    def _validate(
+        self, cfg: Config, value: Union[str, int, float]
+    ) -> Union[int, float]:
+        """
         Validate the value. This method first converts the value to ``type_class`` and then checks
         the value against ``min`` and ``max`` if they are specified.
 
         :param cfg: current Config
         :param value: value to validate
-        '''
-        if not isinstance(value, (str, int, float, self.type_cls)) or isinstance(value, bool):
-            raise ValueError('value type %s cannot be converted to %s' %
-                             (type(value).__name__, self.type_cls.__name__))
+        """
+        if not isinstance(value, (str, int, float, self.type_cls)) or isinstance(
+            value, bool
+        ):
+            raise ValueError(
+                "value type %s cannot be converted to %s"
+                % (type(value).__name__, self.type_cls.__name__)
+            )
 
         try:
             num = self.type_cls(value)  # type: Union[int, float]
         except (ValueError, TypeError) as err:
-            raise ValueError('value is not a valid %s' % self.type_cls.__name__) from err
+            raise ValueError(
+                "value is not a valid %s" % self.type_cls.__name__
+            ) from err
 
         if self.min is not None and num < self.min:
-            raise ValueError('value must be >= %s' % self.min)
+            raise ValueError("value must be >= %s" % self.min)
 
         if self.max is not None and num > self.max:
-            raise ValueError('value must be <= %s' % self.max)
+            raise ValueError("value must be <= %s" % self.max)
 
         return num
 
 
 class IntField(NumberField):
-    '''
+    """
     Integer field.
-    '''
+    """
+
     storage_type = int
 
     def __init__(self, **kwargs):
         super().__init__(int, **kwargs)
 
 
 class FloatField(NumberField):
-    '''
+    """
     Float field.
-    '''
+    """
+
     storage_type = float
 
     def __init__(self, **kwargs):
         super().__init__(float, **kwargs)
```

### Comparing `cincoconfig-0.8.0/cincoconfig/fields/secure_field.py` & `cincoconfig-0.9.0/cincoconfig/fields/secure_field.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,114 +1,118 @@
 #
 # Copyright (C) 2021 Adam Meily
 #
 # This file is subject to the terms and conditions defined in the file 'LICENSE', which is part of
 # this source code package.
 #
-'''
+"""
 Secure fields.
-'''
-import os
-import hashlib
+"""
 import base64
 import binascii
-from typing import Union, Any, Optional, Callable, NamedTuple, Dict
+import hashlib
+import os
+from typing import Any, Callable, Dict, NamedTuple, Optional, Union
 
 from ..core import Config, Field
 from ..encryption import EncryptionError, SecureValue
 
 #: Hash algorithm, as returned by hashlib.new()
-HashAlgorithm = Callable[[Optional[bytes]], 'hashlib._Hash']
+HashAlgorithm = Callable[[bytes], "hashlib._Hash"]
 
 #: Named tuple for digest, value, algorithm
-TDigestValue = NamedTuple('TDigestValue', [
-    ('salt', bytes),
-    ('digest', bytes),
-    ('algorithm', HashAlgorithm)
-])
+TDigestValue = NamedTuple(
+    "TDigestValue", [("salt", bytes), ("digest", bytes), ("algorithm", HashAlgorithm)]
+)
 
 
 class DigestValue(TDigestValue):
-    '''
+    """
     Digest value tuple storing hashed value: (salt, digest, algorithm). The digest is the hash
     of the concatenated salt and plaintext value (``hash(salt + plaintext)``).
-    '''
+    """
 
     def __str__(self) -> str:
-        '''
+        """
         :returns: the salt and digest pair, both base64 encoded, separated by a ``:``.
-        '''
-        return (base64.b64encode(self.salt) + b':' + base64.b64encode(self.digest)).decode()
+        """
+        return (
+            base64.b64encode(self.salt) + b":" + base64.b64encode(self.digest)
+        ).decode()
 
     @classmethod
-    def parse(cls, value: str, algorithm: HashAlgorithm) -> 'DigestValue':
-        '''
+    def parse(cls, value: str, algorithm: HashAlgorithm) -> "DigestValue":
+        """
         Parse a base64-encoded salt/digest pair, as returned by :meth:`__str__`
-        '''
+        """
         try:
-            salt_b64, digest_b64 = value.split(':', 1)
+            salt_b64, digest_b64 = value.split(":", 1)
             salt = base64.b64decode(salt_b64)
             digest = base64.b64decode(digest_b64)
         except (ValueError, binascii.Error) as err:
-            raise ValueError('invalid salt/digest tuple value') from err
+            raise ValueError("invalid salt/digest tuple value") from err
 
         return DigestValue(salt, digest, algorithm)
 
     @classmethod
-    def create(cls, plaintext: Union[str, bytes], algorithm: HashAlgorithm,
-               salt: bytes = None) -> 'DigestValue':
-        '''
+    def create(
+        cls,
+        plaintext: Union[str, bytes],
+        algorithm: HashAlgorithm,
+        salt: Optional[bytes] = None,
+    ) -> "DigestValue":
+        """
         Hash a plaintext value and return the new digest value. The digest is calculated as:
 
         .. code-block:: python
 
             salt[:digest_size] + plaintext
 
         The *salt* will be randomly generated if not specified. If the salt is specified and it is
         larger than the algorithm ``digest_size``, the salt will be truncated to the
         ``digest_size``.
 
         :param plaintext: string to hash
         :param algorithm: hashlib algorithm to use
         :param salt: hash salt
         :returns: the created digest value
-        '''
+        """
 
         hasher = algorithm()  # type: ignore
         if salt and len(salt) < hasher.digest_size:
-            raise TypeError('salt must be at least %d bytes' % hasher.digest_size)
+            raise TypeError("salt must be at least %d bytes" % hasher.digest_size)
 
         if salt:
-            salt = salt[:hasher.digest_size]
+            salt = salt[: hasher.digest_size]
         else:
             salt = os.urandom(hasher.digest_size)
 
         if isinstance(plaintext, str):
             plaintext = plaintext.encode()
 
         hasher.update(salt + plaintext)
         return DigestValue(salt, hasher.digest(), algorithm)
 
     def challenge(self, plaintext: Union[str, bytes]) -> None:
-        '''
+        """
         Challenge a plaintext value against the digest value. This will raise a :class:`ValueError`
         if the challenge is unsuccessful.
 
         :raises ValueError: the challenge was unsuccessful
-        '''
+        """
         if isinstance(plaintext, str):
             plaintext = plaintext.encode()
 
         challenge = self.algorithm(self.salt + plaintext).digest()
         if self.digest != challenge:
-            raise ValueError('challenge failed')
+            raise ValueError("challenge failed")
 
 
 class ChallengeField(Field):
-    '''
+    """
     A field whose value is securely stored as a hash (:class:`DigestValue`). This field can be
     used as a secure method of password storage and comparison, since the password is only stored
     in hashed form and not in plaintext. A digest value is pair of salt and
     ``hash(salt + plaintext)`` values.
 
     Values are stored in memory as :class:`DigestValue` instances. For example:
 
@@ -150,189 +154,197 @@
 
     Digest values are saved to disk as a :class:`dict` containing two keys:
 
     - ``salt`` - base64 encoded salt
     - ``digest`` - base64 encoded digest
 
     The challenge field supports loading plaintext string values from the configuration file. So,
-    when manually writting the config file, the user does not need to create the salt and digest
+    when manually writing the config file, the user does not need to create the salt and digest
     pair but, instead, just specify a plaintext string to hash. The value will be properly saved
     as a salt/digest pair the next time the config file is saved to disk.
 
     Available hash algorithms are:
 
     - md5
     - sha1
     - sha224
     - sha256
     - sha384
     - sha512
-    '''
+    """
+
     storage_type = DigestValue
 
     #: Available hashing algorithms
-    ALGORITHMS = {
-        'md5': hashlib.md5,
-        'sha1': hashlib.sha1,
-        'sha224': hashlib.sha224,
-        'sha256': hashlib.sha256,
-        'sha384': hashlib.sha384,
-        'sha512': hashlib.sha512
-    }  # type: Dict[str, Callable]
+    ALGORITHMS: Dict[str, HashAlgorithm] = {
+        "md5": hashlib.md5,
+        "sha1": hashlib.sha1,
+        "sha224": hashlib.sha224,
+        "sha256": hashlib.sha256,
+        "sha384": hashlib.sha384,
+        "sha512": hashlib.sha512,
+    }
 
-    def __init__(self, hash_algorithm: str = 'sha256', **kwargs):
-        '''
+    def __init__(self, hash_algorithm: str = "sha256", **kwargs):
+        """
         :param hash_algorithm: hash algorithm to use, must be a key of :attr:`ALGORITHMS`
-        '''
+        """
         super().__init__(**kwargs)
         algorithm = self.ALGORITHMS.get(hash_algorithm.lower())
         if not algorithm:
-            raise TypeError('Unknown hash algorithm: ' + hash_algorithm)
+            raise TypeError("Unknown hash algorithm: " + hash_algorithm)
         self.algorithm = algorithm
 
     def __setdefault__(self, cfg: Config) -> None:
-        '''
+        """
         Set default value by creating a :class:`DigestValue` if the default value is a string.
-        '''
+        """
         if self.default is None:
             super().__setdefault__(cfg)
             return
 
         if isinstance(self.default, str):
             val = DigestValue.create(self.default, self.algorithm)
         elif isinstance(self.default, DigestValue):
             val = self.default
         else:
-            raise TypeError('invalid default value: %r' % self.default)
-        cfg._data[self._key] = val
+            raise TypeError("invalid default value: %r" % self.default)
+        cfg._set_default_value(self._key, val)
 
     def _validate(self, cfg: Config, value: Any) -> DigestValue:
-        '''
+        """
         Validate the value. If the value is a plaintext string, a :class:`DigestValue`
-        '''
+        """
         if isinstance(value, (str, bytes)):
             val = self._hash(value)
         elif isinstance(value, DigestValue):
             val = value
         else:
-            raise ValueError('value must be a string, not a %s' % type(value).__name__)
+            raise ValueError("value must be a string, not a %s" % type(value).__name__)
         return val
 
-    def _hash(self, plaintext: Union[str, bytes], salt: bytes = None) -> DigestValue:
-        '''
+    def _hash(
+        self, plaintext: Union[str, bytes], salt: Optional[bytes] = None
+    ) -> DigestValue:
+        """
         Private method that performs the actual hash. This method does not
         check if the value has already been hashed.
 
         :param value: the value to be hashed
         :param salt: specify the salt to use. Used by :meth:`check_hash`
         :raise TypeError: if the action is invalid
-        '''
+        """
 
         return DigestValue.create(plaintext, self.algorithm, salt=salt)
 
     def to_basic(self, cfg: Config, value: DigestValue) -> dict:
-        '''
+        """
         Convert to a dict and indicate the type so we know
         on load whether we've already dealt with the field
 
         :param cfg: current config
         :param value: value to encrypt/hash
         :returns: encrypted/hashed value
-        '''
+        """
         if value is None:
             return value
 
         return {
-            'salt': base64.b64encode(value.salt).decode(),
-            'digest': base64.b64encode(value.digest).decode(),
+            "salt": base64.b64encode(value.salt).decode(),
+            "digest": base64.b64encode(value.digest).decode(),
         }
 
     def to_python(self, cfg: Config, value: Union[dict, str]) -> DigestValue:
-        '''
+        """
         Decrypt the value if loading something we've already handled.
         Hash the value if it hasn't been hashed yet.
 
         :param cfg: current config
         :param value: value to decrypt/load
         :returns: decrypted value or unmodified hash
         :raises ValueError: if the value read from the config is neither a dict nor a string
-        '''
+        """
         if value is None:
             return value
 
         if isinstance(value, dict):
             try:
-                salt = base64.b64decode(value['salt'])
+                salt = base64.b64decode(value["salt"])
             except (KeyError, binascii.Error) as err:
-                raise ValueError('invalid salt: salt must be base64-encoded value') from err
+                raise ValueError(
+                    "invalid salt: salt must be base64-encoded value"
+                ) from err
 
             try:
-                digest = base64.b64decode(value['digest'])
+                digest = base64.b64decode(value["digest"])
             except (KeyError, binascii.Error) as err:
-                raise ValueError('invalid digest: digest must be base64-encoded value') from err
+                raise ValueError(
+                    "invalid digest: digest must be base64-encoded value"
+                ) from err
 
             return DigestValue(salt, digest, self.algorithm)
 
         if isinstance(value, str):
             return self._hash(value)
 
-        raise ValueError('invalid salt-digest tuple')
+        raise ValueError("invalid salt-digest tuple")
 
 
 class SecureField(Field):
-    '''
+    """
     A secure storage field where the plaintext configuration value is encrypted on disk and
     decrypted in memory when the configuration file is loaded.
-    '''
+    """
+
     storage_type = str
 
-    def __init__(self, method: str = 'best', sensitive: bool = True, **kwargs):
-        '''
+    def __init__(self, method: str = "best", sensitive: bool = True, **kwargs):
+        """
         :param method: encryption method, see
             :meth:`~cincoconfig.KeyFile._get_provider`
-        '''
+        """
         super().__init__(sensitive=sensitive, **kwargs)
         self.method = method
 
     def to_basic(self, cfg: Config, value: str) -> Optional[dict]:
         if not value:
             return None
 
         with cfg._keyfile as ctx:
             secret = ctx.encrypt(value, method=self.method)
 
         return {
-            'method': secret.method,
-            'ciphertext': base64.b64encode(secret.ciphertext).decode()
+            "method": secret.method,
+            "ciphertext": base64.b64encode(secret.ciphertext).decode(),
         }
 
     def to_python(self, cfg: Config, value: Any) -> Optional[str]:
         if value is None:
             return value
 
         if isinstance(value, str):
             return value
 
         if isinstance(value, dict):
-            method = value.get('method')
-            ciphertext_b64 = value.get('ciphertext')
+            method = value.get("method")
+            ciphertext_b64 = value.get("ciphertext")
 
             if not method:
-                raise ValueError('no encryption method specified')
+                raise ValueError("no encryption method specified")
 
             if not isinstance(ciphertext_b64, str):
-                raise ValueError('invalid ciphertext')
+                raise ValueError("invalid ciphertext")
 
             try:
                 ciphertext = base64.b64decode(ciphertext_b64)
             except binascii.Error as err:
-                raise ValueError('invalid ciphertext') from err
+                raise ValueError("invalid ciphertext") from err
 
             try:
                 with cfg._keyfile as ctx:
                     text = ctx.decrypt(SecureValue(method, ciphertext))
             except (TypeError, EncryptionError) as err:
-                raise ValueError('decryption failed: %s' % str(err)) from err
+                raise ValueError("decryption failed: %s" % str(err)) from err
             else:
                 return text.decode()
 
-        raise ValueError('invalid encrypted value')
+        raise ValueError("invalid encrypted value")
```

### Comparing `cincoconfig-0.8.0/cincoconfig/fields/string_field.py` & `cincoconfig-0.9.0/cincoconfig/fields/string_field.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,160 +1,173 @@
 #
 # Copyright (C) 2021 Adam Meily
 #
 # This file is subject to the terms and conditions defined in the file 'LICENSE', which is part of
 # this source code package.
 #
-'''
+"""
 String fields.
-'''
+"""
 import re
-from typing import List, Union
+from typing import List, Optional, Union
 
-from ..core import Field, Config, Schema
+from ..core import Config, Field, Schema
 from .virtual_field import VirtualField
 
 
 class StringField(Field):
-    '''
+    """
     A string field.
-    '''
+    """
+
     storage_type = str
 
-    def __init__(self, *, min_len: int = None, max_len: int = None, regex: str = None,
-                 choices: List[str] = None, transform_case: str = None,
-                 transform_strip: Union[bool, str] = None, **kwargs):
-        '''
+    def __init__(
+        self,
+        *,
+        min_len: Optional[int] = None,
+        max_len: Optional[int] = None,
+        regex: Optional[str] = None,
+        choices: Optional[List[str]] = None,
+        transform_case: Optional[str] = None,
+        transform_strip: Optional[Union[bool, str]] = None,
+        **kwargs
+    ):
+        """
         The string field can perform transformations on the value prior to validating it if either
         *transform_case* or *transform_strip* are specified.
 
         :param min_len: minimum allowed length
         :param max_len: maximum allowed length
         :param regex: regex pattern that the value must match
         :param choices: list of valid choices
         :param transform_case: transform the value's case to either ``upper`` or ``lower`` case
         :param transform_strip: strip the value by calling :meth:`str.strip`.
             Setting this to ``True`` will call :meth:`str.strip` without any arguments (ie.
             striping all whitespace characters) and if this is a ``str``, then :meth:`str.strip`
             will be called with ``transform_strip``.
-        '''
+        """
         super().__init__(**kwargs)
         self.min_len = min_len
         self.max_len = max_len
         self.regex = re.compile(regex) if regex else None
         self.choices = choices
         self.transform_case = transform_case.lower() if transform_case else None
         self.transform_strip = transform_strip
 
-        if self.transform_case and self.transform_case not in ('lower', 'upper'):
+        if self.transform_case and self.transform_case not in ("lower", "upper"):
             raise TypeError('transform_case must be "lower" or "upper"')
 
     def _validate(self, cfg: Config, value: str) -> str:
-        '''
+        """
         Validate a value.
 
         :param cfg: current Config
         :param value: value to validate
-        '''
+        """
         if not isinstance(value, str):
-            raise ValueError('value must be a string, not a %s' % type(value).__name__)
+            raise ValueError("value must be a string, not a %s" % type(value).__name__)
 
         if self.transform_strip:
             if isinstance(self.transform_strip, str):
                 value = value.strip(self.transform_strip)
             else:
                 value = value.strip()
 
         if self.required and not value:
-            raise ValueError('value is required')
+            raise ValueError("value is required")
 
         if self.transform_case:
-            value = value.lower() if self.transform_case == 'lower' else value.upper()
+            value = value.lower() if self.transform_case == "lower" else value.upper()
 
         if self.min_len is not None and len(value) < self.min_len:
-            raise ValueError('value must be at least %d characters' % self.min_len)
+            raise ValueError("value must be at least %d characters" % self.min_len)
 
         if self.max_len is not None and len(value) > self.max_len:
-            raise ValueError('value must not be more than %d chatacters' % self.max_len)
+            raise ValueError("value must not be more than %d characters" % self.max_len)
 
         if self.regex and not self.regex.match(value):
-            raise ValueError('value does not match pattern %s' % self.regex.pattern)
+            raise ValueError("value does not match pattern %s" % self.regex.pattern)
 
         if self.choices and value not in self.choices:
             if len(self.choices) < 6:
-                postfix = ': must be one of: ' + ', '.join(self.choices)
+                postfix = ": must be one of: " + ", ".join(self.choices)
             else:
-                postfix = ''
-            raise ValueError('value is not a valid choice' + postfix)
+                postfix = ""
+            raise ValueError("value is not a valid choice" + postfix)
 
         return value
 
 
 class LogLevelField(StringField):
-    '''
+    """
     A field representing the Python log level.
-    '''
+    """
+
     storage_type = str
 
-    def __init__(self, levels: List[str] = None, **kwargs):
-        '''
+    def __init__(self, levels: Optional[List[str]] = None, **kwargs):
+        """
         :param levels: list of log levels. If not specified, the default Python log levels will be
             used: ``debug``, ``info``, ``warning``, ``error``, and ``critical``.
-        '''
+        """
         if not levels:
-            levels = ['debug', 'info', 'warning', 'error', 'critical']
+            levels = ["debug", "info", "warning", "error", "critical"]
 
         self.levels = levels
-        kwargs.setdefault('transform_case', 'lower')
-        kwargs.setdefault('transform_strip', True)
-        kwargs['choices'] = levels
+        kwargs.setdefault("transform_case", "lower")
+        kwargs.setdefault("transform_strip", True)
+        kwargs["choices"] = levels
         super().__init__(**kwargs)
 
 
 class ApplicationModeField(StringField):
-    '''
+    """
     A field representing the application operating mode.
-    '''
+    """
+
     storage_type = str
-    HELPER_MODE_PATTERN = re.compile('^[a-zA-Z0-9_]+$')
+    HELPER_MODE_PATTERN = re.compile("^[a-zA-Z0-9_]+$")
 
-    def __init__(self, modes: List[str] = None, create_helpers: bool = True, **kwargs):
-        '''
+    def __init__(
+        self, modes: Optional[List[str]] = None, create_helpers: bool = True, **kwargs
+    ):
+        """
         The *create_helpers* parameter will create a boolean :class:`VirtualField` for each
         ``mode`` named ``is_<mode>_mode``, that returns ``True`` when the mode is active. When
         *create_helpers=True* then each mode name must be a valid Python variable name.
 
         :param modes: application modes, if not specified the default modes will be used:
             ``production`` and ``development``
         :param create_helpers: create helper a bool ``VirtualField`` for each mode
-        '''
+        """
         if not modes:
-            modes = ['development', 'production']
+            modes = ["development", "production"]
 
         self.modes = modes
         self.create_helpers = create_helpers
 
         if create_helpers:
             for mode in modes:
                 if not self.HELPER_MODE_PATTERN.match(mode):
-                    raise TypeError('invalid mode name: %s' % mode)
+                    raise TypeError("invalid mode name: %s" % mode)
 
-        kwargs.setdefault('transform_case', 'lower')
-        kwargs.setdefault('transform_strip', True)
-        kwargs['choices'] = modes
+        kwargs.setdefault("transform_case", "lower")
+        kwargs.setdefault("transform_strip", True)
+        kwargs["choices"] = modes
         super().__init__(**kwargs)
 
-    def _create_helper(self, mode: str) -> 'VirtualField':
-        '''
+    def _create_helper(self, mode: str) -> "VirtualField":
+        """
         Create helper VirtualField.
-        '''
+        """
         return VirtualField(lambda cfg: self.__getval__(cfg) == mode)
 
     def __setkey__(self, schema: Schema, key: str) -> None:
-        '''
+        """
         Set the key and optionally add ``VirtualField`` helpers to the schema if
         *create_helpers=True*.
-        '''
+        """
         super().__setkey__(schema, key)
         if self.create_helpers:
             for mode in self.modes:
-                schema._add_field('is_%s_mode' % mode, self._create_helper(mode))
+                schema._add_field("is_%s_mode" % mode, self._create_helper(mode))
```

### Comparing `cincoconfig-0.8.0/cincoconfig/fields/url_field.py` & `cincoconfig-0.9.0/cincoconfig/fields/url_field.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 #
 # Copyright (C) 2021 Adam Meily
 #
 # This file is subject to the terms and conditions defined in the file 'LICENSE', which is part of
 # this source code package.
 #
-'''
+"""
 URL field.
-'''
+"""
 from urllib.parse import urlparse
 
-from .string_field import StringField
 from ..core import Config
+from .string_field import StringField
 
 
 class UrlField(StringField):
-    '''
+    """
     A URL field. Values are validated that they are both a valid URL and contain a valid scheme.
-    '''
+    """
+
     storage_type = str
 
     def _validate(self, cfg: Config, value: str) -> str:
-        '''
+        """
         Validate the value.
 
         :param cfg: current config
         :param value: value to validate
-        '''
+        """
         value = super()._validate(cfg, value)
 
         try:
             url = urlparse(value)
             if not url.scheme:
-                raise ValueError('no scheme url scheme')
+                raise ValueError("no scheme url scheme")
         except Exception as err:
-            raise ValueError('value is not a valid URL') from err
+            raise ValueError("value is not a valid URL") from err
         return value
```

### Comparing `cincoconfig-0.8.0/cincoconfig/formats/json.py` & `cincoconfig-0.9.0/cincoconfig/formats/json.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,53 +1,54 @@
 #
 # Copyright (C) 2021 Adam Meily
 #
 # This file is subject to the terms and conditions defined in the file 'LICENSE', which is part of
 # this source code package.
 #
-'''
+"""
 JSON config file format.
-'''
+"""
 import json
-from ..core import ConfigFormat, Config
+
+from ..core import Config, ConfigFormat
 
 
 class JsonConfigFormat(ConfigFormat):
-    '''
+    """
     JSON configuration file format.
 
     This class should not be directly referenced. Instead, use the config
     :meth:`~cincoconfig.Config.load` and :meth:`~cincoconfig.Config.save` methods, passing
     *format='json'*.
 
     .. code-block:: python
 
         config.save('filename.json', format='json')
         # or
         config.load('filename.json', format='json')
-    '''
+    """
 
     def __init__(self, pretty: bool = True):
-        '''
+        """
         :param pretty: pretty-print the JSON document in the call to :meth:`json.dumps`
-        '''
+        """
         self.pretty = pretty
 
     def dumps(self, config: Config, tree: dict) -> bytes:
-        '''
+        """
         Deserialize the ``content`` (a :class:`bytes` instance containing a JSON document) to a
         Python basic value tree.
 
         :param config: current config
         :param content: content to serialize
         :returns: the deserialized basic value tree
-        '''
+        """
         return json.dumps(tree, indent=2 if self.pretty else None).encode()
 
     def loads(self, config: Config, content: bytes) -> dict:
-        '''
+        """
         Serialize the basic value ``tree`` to JSON :class:`bytes` document.
 
         :param config: current config
         :param tree: basic value tree
-        '''
+        """
         return json.loads(content.decode())
```

### Comparing `cincoconfig-0.8.0/cincoconfig/formats/pickle.py` & `cincoconfig-0.9.0/cincoconfig/formats/pickle.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,48 +1,49 @@
 #
 # Copyright (C) 2021 Adam Meily
 #
 # This file is subject to the terms and conditions defined in the file 'LICENSE', which is part of
 # this source code package.
 #
-'''
+"""
 Python pickle binary config file format.
-'''
+"""
 import pickle
-from ..core import ConfigFormat, Config
+
+from ..core import Config, ConfigFormat
 
 
 class PickleConfigFormat(ConfigFormat):
-    '''
+    """
     Python pickle configuration file format. This format uses the :mod:`pickle` module to serialize
     and deserialize the configuration basic value tree.
 
     This class should not be directly referenced. Instead, use the config
     :meth:`~cincoconfig.Config.load` and :meth:`~cincoconfig.Config.save` methods, passing
     *format='pickle'*.
 
     .. code-block:: python
 
         config.save('filename.cfg', format='pickle')
         # or
         config.load('filename.cfg', format='pickle')
-    '''
+    """
 
     def dumps(self, config: Config, tree: dict) -> bytes:
-        '''
+        """
         Deserialize the ``content`` (a :class:`bytes` instance containing a Pickled object) to a
         Python basic value tree.
 
         :param config: current config
         :param content: content to serialize
         :returns: the deserialized basic value tree
-        '''
+        """
         return pickle.dumps(tree)
 
     def loads(self, config: Config, content: bytes) -> dict:
-        '''
+        """
         Serialize the basic value ``tree`` to PIckle :class:`bytes` document.
 
         :param config: current config
         :param tree: basic value tree
-        '''
+        """
         return pickle.loads(content)
```

### Comparing `cincoconfig-0.8.0/cincoconfig/formats/xml.py` & `cincoconfig-0.9.0/cincoconfig/formats/xml.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 #
 # Copyright (C) 2021 Adam Meily
 #
 # This file is subject to the terms and conditions defined in the file 'LICENSE', which is part of
 # this source code package.
 #
-'''
+"""
 XML config file format.
-'''
-from xml.etree import ElementTree as ET
+"""
+from typing import Any, Optional
 from xml.dom import minidom
-from typing import Any
-from ..core import ConfigFormat, Config
+from xml.etree import ElementTree as ET
+
+from ..core import Config, ConfigFormat
 from ..fields import BoolField
 
 
 class XmlConfigFormat(ConfigFormat):
-    '''
+    """
     XML configuration file format.
 
     This class should not be directly referenced. Instead, use the config
     :meth:`~cincoconfig.Config.load` and :meth:`~cincoconfig.Config.save` methods, passing
     *format='xml'*.
 
     .. code-block:: python
@@ -33,62 +34,62 @@
 
     .. code-block:: xml
 
         <x type="int">1024</x>
 
     When the configuration file is loaded, the formatter will attempt to parse the original Python
     type. If the parsing fails then the original string value is stored in the basic value tree.
-    '''
+    """
 
-    def __init__(self, root_tag: str = 'config'):
-        '''
+    def __init__(self, root_tag: str = "config"):
+        """
         :param root_tag: root configuration tag name
-        '''
+        """
         self.root_tag = root_tag
 
     def _to_element(self, key: str, value: Any) -> ET.Element:
-        '''
+        """
         Convert the key/value pair to an XML element.
 
         :param key: the field key (becomes the tag name)
         :param value: the field valid
         :returns: the element containing the XML encoded key/value pair
-        '''
+        """
         ele = ET.Element(key)
         if isinstance(value, str):
-            ele.attrib['type'] = 'str'
+            ele.attrib["type"] = "str"
             ele.text = value
         elif isinstance(value, bool):
-            ele.attrib['type'] = 'bool'
-            ele.text = 'true' if value else 'false'
+            ele.attrib["type"] = "bool"
+            ele.text = "true" if value else "false"
         elif isinstance(value, int):
-            ele.attrib['type'] = 'int'
+            ele.attrib["type"] = "int"
             ele.text = str(value)
         elif isinstance(value, float):
-            ele.attrib['type'] = 'float'
+            ele.attrib["type"] = "float"
             ele.text = str(value)
         elif value is None:
-            ele.attrib['type'] = 'none'
+            ele.attrib["type"] = "none"
         elif isinstance(value, list):
-            ele.attrib['type'] = 'list'
+            ele.attrib["type"] = "list"
             for item in value:
-                sub = self._to_element('item', item)
+                sub = self._to_element("item", item)
                 ele.append(sub)
         elif isinstance(value, dict):
-            ele.attrib['type'] = 'dict'
+            ele.attrib["type"] = "dict"
             for subkey, subval in value.items():
                 sub = self._to_element(subkey, subval)
                 ele.append(sub)
         else:
-            raise TypeError('non-basic type: %s' % str(type(value)))
+            raise TypeError("non-basic type: %s" % str(type(value)))
 
         return ele
 
-    def _from_element(self, ele: ET.Element, py_type: str = None) -> Any:
-        '''
+    def _from_element(self, ele: ET.Element, py_type: Optional[str] = None) -> Any:
+        """
         Parse the XML element to the original Python type. This method will attempt to convert any
         basic types to their original Python type and, if conversion fails, will use the original
         string value. For example:
 
         .. code-block:: xml
 
             <x type="int">blah</x>
@@ -99,90 +100,90 @@
         .. code-block:: python
 
             tree = {
                 'x': 'blah'
             }
 
         :param ele: the XML element to convert
-        :param py_type: force the Python type attribute rather than reading the Python type from the
-            *type* attribute
+        :param py_type: force the Python type attribute rather than reading the Python type from
+            the *type* attribute
         :returns: the parsed Python value
-        '''
+        """
         # pylint: disable=too-many-branches
-        py_type = py_type or ele.attrib.get('type')
-        text = ele.text or ''
+        py_type = py_type or ele.attrib.get("type")
+        text = ele.text or ""
         value = None  # type: Any
-        if py_type == 'str':
+        if py_type == "str":
             value = text
-        elif py_type == 'bool':
+        elif py_type == "bool":
             if text.lower() in BoolField.TRUE_VALUES:
                 value = True
             elif text.lower() in BoolField.FALSE_VALUES:
                 value = False
             else:
                 value = text
-        elif py_type == 'int':
+        elif py_type == "int":
             try:
                 value = int(text)
-            except:
+            except:  # noqa: E722
                 value = text
-        elif py_type == 'float':
+        elif py_type == "float":
             try:
                 value = float(text)
-            except:
+            except:  # noqa: E722
                 value = text
-        elif py_type == 'none':
+        elif py_type == "none":
             value = None
-        elif py_type == 'list':
+        elif py_type == "list":
             value = []
             for sub in ele:
                 item = self._from_element(sub)
                 value.append(item)
-        elif py_type == 'dict':
+        elif py_type == "dict":
             value = {}
             for sub in ele:
                 item = self._from_element(sub)
                 value[sub.tag] = item
         else:
             value = text
 
         return value
 
     def _prettify(self, ele: ET.Element) -> bytes:
-        '''
+        """
         Pretty print the XML element.
 
         :param ele: XML element to pretty print
         :returns: the pretty printed XML element
-        '''
-        rough_string = ET.tostring(ele, 'utf-8')
+        """
+        rough_string = ET.tostring(ele, "utf-8")
         reparsed = minidom.parseString(rough_string)
         return reparsed.toprettyxml(indent="  ").encode()
 
     def dumps(self, config: Config, tree: dict) -> bytes:
-        '''
+        """
         Serialize the basic value ``tree`` to an XML :class:`bytes` document. The returned XML
         document will contain a single top-level tag named *root_key* that all other values are
         stored under.
 
         :param config: current config
         :param tree: basic value tree
         :returns: the serialized basic value tree
-        '''
+        """
         ele = self._to_element(self.root_tag, tree)
         return self._prettify(ele)
 
     def loads(self, config: Config, content: bytes) -> dict:
-        '''
+        """
         Deserialize the ``content`` (a :class:`bytes` instance containing an XML document) to a
         Python basic value tree. The returned basic value tree will be scoped to *root_tag*, if it
         exists in the deserialized :class:`dict`.
 
         :param config: current config
         :param content: content to deserialize
         :returns: deserialized basic value tree
-        '''
+        """
         root = ET.fromstring(content.decode())
         if root.tag != self.root_tag:
-            raise ValueError('unexpected root tag: %s' % root.tag)
+            raise ValueError("unexpected root tag: %s" % root.tag)
 
-        return self._from_element(root, 'dict')
+        return self._from_element(root, "dict")
```

### Comparing `cincoconfig-0.8.0/cincoconfig/formats/yaml.py` & `cincoconfig-0.9.0/cincoconfig/formats/yaml.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,44 +1,46 @@
 #
 # Copyright (C) 2021 Adam Meily
 #
 # This file is subject to the terms and conditions defined in the file 'LICENSE', which is part of
 # this source code package.
 #
-'''
+"""
 YAML config file format.
-'''
+"""
+from typing import Optional
+
 try:
     import yaml
 except ImportError:  # pragma: no cover
     IS_AVAILABLE = False
 else:
     IS_AVAILABLE = True
 
-from ..core import ConfigFormat, Config
+from ..core import Config, ConfigFormat
 
 
 class YamlConfigFormat(ConfigFormat):
-    '''
+    """
     YAML configuration file format. This format is only available when the ``PyYAML`` package is
     installed.
 
     This class should not be directly referenced. Instead, use the config
     :meth:`~cincoconfig.Config.load` and :meth:`~cincoconfig.Config.save` methods, passing
     *format='yaml'*.
 
     .. code-block:: python
 
         config.save('filename.yml', format='yaml')
         # or
         config.load('filename.yml', format='yaml')
-    '''
+    """
 
-    def __init__(self, root_key: str = None):
-        '''
+    def __init__(self, root_key: Optional[str] = None):
+        """
         By default, the basic value tree is serialized to YAML document as-is, where top-level
         configuration values are placed at the top level of the config file. For example:
 
         .. code-block:: python
 
             >>> # assume tree = {'x': 1, 'y': 2}
             >>> print(config.dumps(format='yaml'))
@@ -55,47 +57,47 @@
             CONFIG:
                 x: 1
                 y: 2
 
         The *root_key* argument affects both how :meth:`loads` and :meth:`dumps` behave.
 
         :param root_key: the root config key that the configuration values should be stored under
-        '''
+        """
         if not IS_AVAILABLE:
             raise TypeError('YAML format is not available, please install "PyYAML"')
 
         self.root_key = root_key
 
     def dumps(self, config: Config, tree: dict) -> bytes:
-        '''
+        """
         Serialize the basic value ``tree`` to YAML :class:`bytes` document. If *root_key* was
         specified, the returned YAML document will contain a single top-level field named
         *root_key* that all other values are stored under.
 
         :param config: current config
         :param tree: basic value tree
         :returns: the serialized basic value tree
-        '''
+        """
         if self.root_key:
             tree = {self.root_key: tree}
         return yaml.dump(tree, Dumper=yaml.Dumper).encode()
 
     def loads(self, config: Config, content: bytes) -> dict:
-        '''
+        """
         Deserialize the ``content`` (a :class:`bytes` instance containing a YAML document) to a
         Python basic value tree.  If *root_key* was specified, the returned basic value tree will
         be scoped to *root_key*, if it exists in the deserialized :class:`dict`. This is
         equivalent to:
 
         .. code-block:: python
 
             tree = yaml.load(content)
             return tree[self.root_key]
 
         :param config: current config
         :param content: content to deserialize
         :returns: deserialized basic value tree
-        '''
+        """
         tree = yaml.load(content.decode(), Loader=yaml.Loader)
         if self.root_key and self.root_key in tree:
             tree = tree[self.root_key]
         return tree
```

### Comparing `cincoconfig-0.8.0/cincoconfig/stubs.py` & `cincoconfig-0.9.0/cincoconfig/stubs.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,184 +1,193 @@
 #
 # Copyright (C) 2021 Adam Meily
 #
 # This file is subject to the terms and conditions defined in the file 'LICENSE', which is part of
 # this source code package.
 #
-'''
+"""
 Generate type stubs for configurations.
-'''
+"""
 import inspect
-from typing import Type, Union, Any, Dict
-from .core import Config, Schema, ConfigType, Field, BaseField
+from typing import Any, Dict, Optional, Type, Union
+
+from .core import BaseField, Config, ConfigType, Field, Schema
 from .fields import InstanceMethodField, VirtualField
 
 
 def get_annotation_typestr(field: Union[BaseField, Type, str]) -> str:
-    '''
+    """
     Get the annotation type string for the provided argument. This method accepts a
     :class:`cincoconfig.Field` and returns the ``storage_type`` annotation.
 
     :param field: the field, schema, type, or string annotation
     :returns: the annotation type string, or ``typing.Any`` if no annotation is specified.
-    '''
+    """
     if isinstance(field, Field):
         storage_type = field.storage_type
     elif isinstance(field, Schema):
         storage_type = Schema
     elif isinstance(field, type):
         storage_type = field
     elif isinstance(field, str):
         storage_type = field
     elif field is None:
-        storage_type = 'None'
+        storage_type = "None"
     else:
-        raise TypeError('Unknown storage_type: %s' % type(field))
+        raise TypeError("Unknown storage_type: %s" % type(field))
 
     if isinstance(storage_type, type):
-        modname = getattr(storage_type, '__module__', None)
-        if modname and modname != 'builtins':
-            retval = '%s.%s' % (modname, storage_type.__name__)
+        modname = getattr(storage_type, "__module__", None)
+        if modname and modname != "builtins":
+            retval = "%s.%s" % (modname, storage_type.__name__)
         else:
             retval = storage_type.__name__
     else:
         retval = str(storage_type)
 
-    return retval or 'typing.Any'
+    return retval or "typing.Any"
 
 
 def get_arg_annotation(key: str, field: Union[BaseField, Type, str]) -> str:
-    '''
+    """
     Get the argument annotation, ``arg: typestr``, for an argument.
 
     :param key: argument name
     :param field: the argument type
     :returns: the argument annotation
-    '''
+    """
     typestr = get_annotation_typestr(field)
-    return '%s: %s' % (key, typestr)
+    return "%s: %s" % (key, typestr)
 
 
 def get_retval_annotation(annotation: Any) -> str:
-    '''
+    """
     Get the return value annotation, `` -> typestr``, of the annotation type.
 
     :param annotation: the return value type or annotation
     :returns: the return value annotation
-    '''
+    """
     try:
         typestr = get_annotation_typestr(annotation)
-    except:
-        return ''
+    except:  # noqa: E722
+        return ""
 
-    print('retval:', repr(annotation), '-', repr(typestr))
-    return ' -> %s' % typestr if typestr else ''
+    print("retval:", repr(annotation), "-", repr(typestr))
+    return " -> %s" % typestr if typestr else ""
 
 
 def get_method_annotation(key: str, field: InstanceMethodField) -> str:
-    '''
+    """
     Get the instance method annotation, ``def key(self, ...): -> typestr: ...``.
 
     :param key: method name
     :param field: the instance method field
     :returns: the instance method annotation
-    '''
+    """
     # pylint: disable=too-many-locals
     # spell-checker:ignore varargs, varkw, kwonlyargs
-    args, varargs, varkw, _, kwonlyargs, _, annotations = inspect.getfullargspec(field.method)
-    has_ret_annotation = 'return' in annotations
+    args, varargs, varkw, _, kwonlyargs, _, annotations = inspect.getfullargspec(
+        field.method
+    )
+    has_ret_annotation = "return" in annotations
     if kwonlyargs:
         if not varargs:
-            args.append('*')
+            args.append("*")
         else:
-            args.append('*%s' % varargs)
+            args.append("*%s" % varargs)
             varargs = None
         args += kwonlyargs
 
     items = []
     for arg in args:
         has_annotation = arg in annotations
         if has_annotation:
             typestr = get_annotation_typestr(annotations[arg])
-        elif not arg.startswith('*'):
-            typestr = 'typing.Any'
+        elif not arg.startswith("*"):
+            typestr = "typing.Any"
         else:
-            typestr = ''
+            typestr = ""
 
         if typestr:
-            item = '%s: %s' % (arg, typestr)
+            item = "%s: %s" % (arg, typestr)
         else:
             item = arg
 
         items.append(item)
 
     if varargs:
-        items.append('*%s' % varargs)
+        items.append("*%s" % varargs)
     if varkw:
-        items.append('**%s' % varkw)
+        items.append("**%s" % varkw)
 
-    items[0] = 'self'
-    annotation = 'def %s(%s)' % (key, ', '.join(items))
+    items[0] = "self"
+    annotation = "def %s(%s)" % (key, ", ".join(items))
     if has_ret_annotation:
-        retval = get_retval_annotation(annotations['return'])
+        retval = get_retval_annotation(annotations["return"])
         annotation += retval
-    annotation += ': ...'
+    annotation += ": ..."
 
     return annotation
 
 
-def generate_stub(config: Union[Schema, ConfigType, Config], class_name: str = None) -> str:
-    '''
+def generate_stub(
+    config: Union[Schema, ConfigType, Config], class_name: Optional[str] = None
+) -> str:
+    """
     Generate the Python stub class (pyi file) for a provided Schema instance, Config instance, or
     ConfigType class. Generating a pyi stub file is useful when developing in an IDE, such as
     VSCode, to make the autocompleter / Intellisense / Language Server understand the structure of
     the configuration and properly show autocomplete results and perform type checking / linting.
 
     Save the generated pyi stub file to a location in your project repository and then configure
     the IDE / type checked (MyPy) to use the directory to load additional type information from.
 
     :param config: the configuration to generate the stub file from
     :param class_name: the configuration class name
     :returns: the content of the pyi stub file for the provided configuration
-    '''
+    """
     if isinstance(config, type) and issubclass(config, ConfigType):
         schema = config.__schema__
         class_name = class_name or config.__name__
     elif isinstance(config, Config):
         schema = config._schema
     elif isinstance(config, Schema):
         schema = config
     else:
-        raise TypeError('must be Schema, ConfigType, or Config')
+        raise TypeError("must be Schema, ConfigType, or Config")
 
     if not class_name:
-        raise TypeError('class_name is required when config is not a ConfigType subclass')
-
-    properties = {}  # type: Dict[str, str]
-    methods = {}  # type: Dict[str, InstanceMethodField]
-    attrs = {}  # type: Dict[str, str]
+        raise TypeError(
+            "class_name is required when config is not a ConfigType subclass"
+        )
+
+    properties: Dict[str, str] = {}
+    methods: Dict[str, InstanceMethodField] = {}
+    attrs: Dict[str, str] = {}
 
     for key, field in schema._fields.items():
         if isinstance(field, VirtualField):
             properties[key] = get_arg_annotation(key, field)
         elif isinstance(field, InstanceMethodField):
             methods[key] = field
         else:
             attrs[key] = properties[key] = get_arg_annotation(key, field)
 
-    blocks = [
-        'class %s(cincoconfig.core.ConfigType):' % class_name,
-    ] + ['    %s' % attr for attr in properties.values()] + ['']
-
-    attr_list = ['self'] + list(attrs.values())
-    blocks.append(
-        '    def __init__(%s): ...' % ', '.join(attr_list)
+    blocks = (
+        [
+            "class %s(cincoconfig.core.ConfigType):" % class_name,
+        ]
+        + ["    %s" % attr for attr in properties.values()]
+        + [""]
     )
 
+    attr_list = ["self"] + list(attrs.values())
+    blocks.append("    def __init__(%s): ..." % ", ".join(attr_list))
+
     if methods:
-        blocks.append('')
+        blocks.append("")
 
     for key, method_field in methods.items():
         annotation = get_method_annotation(key, method_field)
-        blocks.append('    %s' % annotation)
+        blocks.append("    %s" % annotation)
 
-    return '\n'.join(blocks)
+    return "\n".join(blocks)
```

### Comparing `cincoconfig-0.8.0/cincoconfig/support.py` & `cincoconfig-0.9.0/cincoconfig/support.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,39 @@
 #
 # Copyright (C) 2021 Adam Meily
 #
 # This file is subject to the terms and conditions defined in the file 'LICENSE', which is part of
 # this source code package.
 #
-'''
+"""
 Support functions.
-'''
+"""
 import sys
 from argparse import ArgumentParser, Namespace
-from typing import Callable, List, Tuple, Union, Type
-from .core import (Schema, BaseField, Config, ConfigType, FieldValidator, ConfigValidator, Field,
-                   VirtualFieldMixin)
+from typing import Callable, List, Optional, Tuple, Type, Union
 
-
-def make_type(schema: Schema, name: str, module: str = None,
-              key_filename: str = None) -> Type[ConfigType]:
-    '''
+from .core import (
+    BaseField,
+    Config,
+    ConfigType,
+    ConfigValidator,
+    Field,
+    FieldValidator,
+    Schema,
+    VirtualFieldMixin,
+)
+
+
+def make_type(
+    schema: Schema,
+    name: str,
+    module: Optional[str] = None,
+    key_filename: Optional[str] = None,
+) -> Type[ConfigType]:
+    """
     Create a new type that wraps this schema. This method should only be called once per
     schema object.
 
     Use this method when to create reusable configuration objects that can be used multiple
     times  in code in a more traditional Pythonic manner. For example, consider the following:
 
     .. code-block:: python
@@ -56,62 +69,66 @@
     The new class inherits from :class:`Config`.
 
     :param name: the new class name
     :param module: the owning module
     :param key_filename: the key file name passed to each new config object,
     :param validator: config validator callback method
     :returns: the new type
-    '''
-    result = type(name, (ConfigType,), {
-        '__schema__': schema,
-        '__key_filename__': key_filename
-    })
+    """
+    result = type(
+        name, (ConfigType,), {"__schema__": schema, "__key_filename__": key_filename}
+    )
     # This is copied from the namedtuple method. We try to set the module of the new
     # class to the calling module.
     if module is None:
         try:
-            module = sys._getframe(1).f_globals.get('__name__', '__main__')
+            module = sys._getframe(1).f_globals.get("__name__", "__main__")
         except (AttributeError, ValueError):  # pragma: no cover
             pass
     if module is not None:
         result.__module__ = module
 
     return result
 
 
-def generate_argparse_parser(schema, **parser_kwargs) -> ArgumentParser:
-    '''
+def generate_argparse_parser(
+    schema: Union[Config, Schema], **parser_kwargs
+) -> ArgumentParser:
+    """
     Generate a :class:`argparse.ArgumentParser` based on the schema. This method generates
     ``--long-arguments`` for each field that stores a string, integer, float, or bool (based
     on the field's ``storage_type``). Boolean fields have two long arguments created, one to
     store a ``True`` value and another, ``--no-[x]``, to disable it.
 
     :param kwargs: keyword arguments to pass to the generated ``ArgumentParser`` constructor
     :returns: the generated argument parser
-    '''
+    """
     parser = ArgumentParser(**parser_kwargs)
     for name, _, field in get_all_fields(schema):
         if not isinstance(field, Field):
             continue
 
-        arg = '--' + name.replace('.', '-').replace('_', '-').lower()
-        metavar = name.replace('.', '_').upper()
+        arg = "--" + name.replace(".", "-").replace("_", "-").lower()
+        metavar = name.replace(".", "_").upper()
         if field.storage_type in (str, float, int):
-            parser.add_argument(arg, action='store', dest=name, help=field.short_help,
-                                metavar=metavar)
+            parser.add_argument(
+                arg, action="store", dest=name, help=field.short_help, metavar=metavar
+            )
         elif field.storage_type is bool:
-            off_arg = '--no-' + name.replace('.', '-').replace('_', '-').lower()
-            parser.add_argument(arg, dest=name, action='store_true', help=field.short_help)
-            parser.add_argument(off_arg, dest=name, action='store_false')
+            off_arg = "--no-" + name.replace(".", "-").replace("_", "-").lower()
+            parser.add_argument(
+                arg, dest=name, action="store_true", help=field.short_help
+            )
+            parser.add_argument(off_arg, dest=name, action="store_false")
 
     return parser
 
 
 def validator(field: BaseField) -> Callable:
-    '''
+    """
     Decorator to register a new validator with the schema or field. All validators will be run
     against the configuration whenever the configuration is loaded from disk. Multiple validators
     can be registered by using the decorator multiple times. Subconfigs can also be validated by
     using the decorator on the sub schema.
 
     .. code-block:: python
 
@@ -136,28 +153,31 @@
         # .....
 
     The validator function needs to raise an exception, preferably a :class:`ValueError`, if
     the validation fails.
 
     :param func: validator function that accepts a single argument: :class:`Config`.
     :returns: ``func``
-    '''
+    """
+
     def inner(func: Union[ConfigValidator, FieldValidator]) -> Callable:
         if isinstance(field, Field):
             field.validator = func  # type: ignore
         elif isinstance(field, Schema):
             field._validators.append(func)  # type: ignore
 
         return func
 
     return inner
 
 
-def get_all_fields(schema: Union[Schema, Config]) -> List[Tuple[str, Schema, BaseField]]:
-    '''
+def get_all_fields(
+    schema: Union[Schema, Config]
+) -> List[Tuple[str, Schema, BaseField]]:
+    """
     Get all the fields and nested fields of the schema or config, including the nested
     schemas/configs.
 
     .. code-block:: python
 
         >>> schema = Schema()
         >>> schema.x = IntField()
@@ -176,31 +196,36 @@
     2. `schema` - the schema that the field belongs to.
     3. `field` - the field.
 
     The order of the fields will be the same order in which the fields were added to the
     schema.
 
     :returns: all the fields as a list of tuples: ``(path, schema, field)``
-    '''
+    """
     if isinstance(schema, Config):
         schema = schema._schema
 
     ret = []
-    prefix = schema._key + '.' if schema._key else ''
+    prefix = schema._key + "." if schema._key else ""
     for key, field in schema._fields.items():
         ret.append((prefix + key, schema, field))
         if isinstance(field, Schema):
-            ret.extend([(prefix + subkey, schema, subfield)
-                        for subkey, schema, subfield in get_all_fields(field)])
+            ret.extend(
+                [
+                    (prefix + subkey, schema, subfield)
+                    for subkey, schema, subfield in get_all_fields(field)
+                ]
+            )
     return ret
 
 
-def cmdline_args_override(config: Config, args: Namespace,
-                          ignore: Union[str, List[str]] = None) -> None:
-    '''
+def cmdline_args_override(
+    config: Config, args: Namespace, ignore: Optional[Union[str, List[str]]] = None
+) -> None:
+    """
     Override configuration setting based on command line arguments, parsed from the
     :mod:`argparse` module. This method is useful when loading a configuration but allowing the
     user the option to override or extend the configuration via command line arguments.
 
     .. code-block:: python
 
         parser = argparse.ArgumentParser()
@@ -225,87 +250,88 @@
             config.http.address = getattr(args, 'http.address')
 
     This method is compatible with manually created argument parser and an autogenerated one
     from the Schema :meth:`~Schema.generate_argparse_parser` method.
 
     :param args: parsed command line arguments from :meth:`~argparse.ArgumentParser.parse_args`
     :param ignore: list of arguments to ignore and not process
-    '''
+    """
     if isinstance(ignore, str):
         ignore = [ignore]
     else:
         ignore = ignore or []
 
     for key, value in vars(args).items():
         if key not in ignore and value is not None:
             config.__setitem__(key, value)
 
 
 def item_ref_path(item: Union[BaseField, Config]) -> str:
-    '''
+    """
     Get the full reference path to a field or configuration.
 
     :param item: field, schema, or configuration
     :returns: full reference path to the item
-    '''
+    """
     return item._ref_path
 
 
-def get_fields(schema: Union[Config, Schema],
-               types: Union[Type, Tuple[Type]] = None) -> List[Tuple[str, BaseField]]:
-    '''
+def get_fields(
+    schema: Union[Config, Schema], types: Union[Type, Tuple[Type]] = None
+) -> List[Tuple[str, BaseField]]:
+    """
     Get all fields within a configuration or schema. This method does not recurse into nested
     schemas/configs, unlike :meth:`~get_all_fields`. The return value is a list of fields as tuples
     ``(key, field)``.
 
     :param schema: schema or configuration object
     :param types: only return fields of a specific type
     :returns: the list of fields
-    '''
+    """
 
     fields = list(schema._fields.items())
     if isinstance(schema, Config):
         fields += list(schema._schema._fields.items())
 
     if types:
         fields = [item for item in fields if isinstance(item[1], types)]
     return fields
 
 
 def _list_asdict(items: list, virtual: bool) -> list:
-    '''
+    """
     Handle nested lists and nested Config object for :meth:`asdict`.
 
     :param items: list
     :param virtual: include configuration virtual values
     :returns: converted list
-    '''
+    """
     value = []
     for item in items:
         if isinstance(item, list):
             item = _list_asdict(item, virtual=virtual)
         elif isinstance(item, Config):
             item = asdict(item, virtual=virtual)
         elif isinstance(item, dict):
             item = dict(item)
         value.append(item)
     return value
 
 
 def asdict(config: Config, virtual: bool = False) -> dict:
-    '''
+    """
     Converts the configuration object to a dict. Whereas :meth:`~Config.to_tree` converts the
     configuration to a basic value tree suitable for saving to disk, the ``asdict`` method converts
     the configuration, and all nested configuration objects, to a dict, preserving each value
     as-is.
 
-    :param config: the configuration to conver to a dict
+    :param config: the configuration to convert to a dict
     :param virtual: include virtual field values in the dict
     :returns: the converted configuration dict
-    '''
+    """
     data = {}
     for key, value in config._data.items():
         if isinstance(value, list):
             value = _list_asdict(value, virtual=virtual)
         elif isinstance(value, Config):
             value = asdict(value, virtual=virtual)
         elif isinstance(value, dict):
@@ -313,7 +339,41 @@
         data[key] = value
 
     if virtual:
         fields = get_fields(config, VirtualFieldMixin)
         data.update({key: field.__getval__(config) for key, field in fields})
 
     return data
+
+
+def is_value_defined(config: Config, key: str) -> bool:
+    """
+    Check if the given field has been set by the user through either loading a configuration file
+    or using the API to set the field value.
+
+    :param config: configuration object
+    :param key: field key
+    :returns: the field is set by the user
+    """
+    path, _, key = key.rpartition(".")
+    if path:
+        config = config[path]
+
+    return key not in config._default_value_keys
+
+
+def reset_value(config: Config, key: str) -> None:
+    """
+    Reset a config value back to the default.
+
+    :param config: configuration object
+    :param key: field key
+    """
+    path, _, key = key.rpartition(".")
+    if path:
+        config = config[path]
+
+    field = config._get_field(key)
+    if not field:
+        raise AttributeError(key)
+
+    field.__setdefault__(config)
```

