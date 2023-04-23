# Comparing `tmp/python-taiga-1.0.0b1.tar.gz` & `tmp/python-taiga-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/python-taiga-1.0.0b1.tar", last modified: Sun May  5 15:09:38 2019, max compression
+gzip compressed data, was "python-taiga-1.1.0.tar", last modified: Sun Apr 23 21:07:15 2023, max compression
```

## Comparing `python-taiga-1.0.0b1.tar` & `python-taiga-1.1.0.tar`

### file list

```diff
@@ -1,28 +1,58 @@
-drwxrwsr-x   0 yakky     (1000)     1004        0 2019-05-05 15:09:38.000000 python-taiga-1.0.0b1/
-drwxrwsr-x   0 yakky     (1000)     1004        0 2019-05-05 15:09:38.000000 python-taiga-1.0.0b1/python_taiga.egg-info/
--rw-rw-r--   0 yakky     (1000)     1004     8595 2019-05-05 15:09:38.000000 python-taiga-1.0.0b1/python_taiga.egg-info/PKG-INFO
--rw-rw-r--   0 yakky     (1000)     1004      477 2019-05-05 15:09:38.000000 python-taiga-1.0.0b1/python_taiga.egg-info/SOURCES.txt
--rw-rw-r--   0 yakky     (1000)     1004        1 2019-05-05 15:09:38.000000 python-taiga-1.0.0b1/python_taiga.egg-info/dependency_links.txt
--rw-rw-r--   0 yakky     (1000)     1004        1 2019-05-05 15:09:38.000000 python-taiga-1.0.0b1/python_taiga.egg-info/not-zip-safe
--rw-rw-r--   0 yakky     (1000)     1004       58 2019-05-05 15:09:38.000000 python-taiga-1.0.0b1/python_taiga.egg-info/requires.txt
--rw-rw-r--   0 yakky     (1000)     1004        6 2019-05-05 15:09:38.000000 python-taiga-1.0.0b1/python_taiga.egg-info/top_level.txt
-drwxrwsr-x   0 yakky     (1000)     1004        0 2019-05-05 15:09:38.000000 python-taiga-1.0.0b1/taiga/
-drwxrwsr-x   0 yakky     (1000)     1004        0 2019-05-05 15:09:38.000000 python-taiga-1.0.0b1/taiga/models/
--rw-rw-r--   0 yakky     (1000)     1004     1441 2019-05-05 11:07:42.000000 python-taiga-1.0.0b1/taiga/models/__init__.py
--rw-rw-r--   0 yakky     (1000)     1004     8146 2019-05-05 11:07:42.000000 python-taiga-1.0.0b1/taiga/models/base.py
--rw-rw-r--   0 yakky     (1000)     1004    60227 2019-05-05 14:30:20.000000 python-taiga-1.0.0b1/taiga/models/models.py
--rw-rw-r--   0 yakky     (1000)     1004      221 2019-05-05 14:52:23.000000 python-taiga-1.0.0b1/taiga/__init__.py
--rw-rw-r--   0 yakky     (1000)     1004     7499 2019-05-05 14:28:29.000000 python-taiga-1.0.0b1/taiga/client.py
--rw-rw-r--   0 yakky     (1000)     1004      623 2019-05-05 14:16:48.000000 python-taiga-1.0.0b1/taiga/exceptions.py
--rw-rw-r--   0 yakky     (1000)     1004     7505 2019-05-05 13:51:32.000000 python-taiga-1.0.0b1/taiga/requestmaker.py
--rw-rw-r--   0 yakky     (1000)     1004       77 2018-01-07 03:17:55.000000 python-taiga-1.0.0b1/taiga/utils.py
--rw-rw-r--   0 yakky     (1000)     1004      709 2018-05-26 10:12:32.000000 python-taiga-1.0.0b1/AUTHORS
--rw-rw-r--   0 yakky     (1000)     1004     3138 2018-05-26 10:12:32.000000 python-taiga-1.0.0b1/CONTRIBUTING.rst
--rw-rw-r--   0 yakky     (1000)     1004      762 2019-05-05 14:43:05.000000 python-taiga-1.0.0b1/HISTORY.rst
--rw-rw-r--   0 yakky     (1000)     1004     1068 2016-08-27 19:44:07.000000 python-taiga-1.0.0b1/LICENSE
--rw-rw-r--   0 yakky     (1000)     1004      227 2018-05-26 10:12:32.000000 python-taiga-1.0.0b1/MANIFEST.in
--rw-rw-r--   0 yakky     (1000)     1004     5881 2018-05-26 10:12:32.000000 python-taiga-1.0.0b1/README.rst
--rw-rw-r--   0 yakky     (1000)     1004       44 2018-05-26 10:12:32.000000 python-taiga-1.0.0b1/requirements.txt
--rw-rw-r--   0 yakky     (1000)     1004      422 2019-05-05 15:09:38.000000 python-taiga-1.0.0b1/setup.cfg
--rw-rw-r--   0 yakky     (1000)     1004     1240 2019-05-05 14:46:24.000000 python-taiga-1.0.0b1/setup.py
--rw-rw-r--   0 yakky     (1000)     1004     8595 2019-05-05 15:09:38.000000 python-taiga-1.0.0b1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 21:07:15.909267 python-taiga-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-04-23 21:06:40.000000 python-taiga-1.1.0/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)     5416 2023-04-23 21:06:40.000000 python-taiga-1.1.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-04-23 21:06:40.000000 python-taiga-1.1.0/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-23 21:06:40.000000 python-taiga-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-23 21:06:40.000000 python-taiga-1.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-04-23 21:07:15.909267 python-taiga-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-04-23 21:06:40.000000 python-taiga-1.1.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-04-23 21:06:40.000000 python-taiga-1.1.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 21:07:15.897267 python-taiga-1.1.0/python_taiga.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-04-23 21:07:15.000000 python-taiga-1.1.0/python_taiga.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-23 21:07:15.000000 python-taiga-1.1.0/python_taiga.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 21:07:15.000000 python-taiga-1.1.0/python_taiga.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 21:07:02.000000 python-taiga-1.1.0/python_taiga.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-23 21:07:15.000000 python-taiga-1.1.0/python_taiga.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-23 21:07:15.000000 python-taiga-1.1.0/python_taiga.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-23 21:06:40.000000 python-taiga-1.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-04-23 21:07:15.909267 python-taiga-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 21:06:40.000000 python-taiga-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 21:07:15.901267 python-taiga-1.1.0/taiga/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-23 21:06:40.000000 python-taiga-1.1.0/taiga/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6854 2023-04-23 21:06:40.000000 python-taiga-1.1.0/taiga/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-04-23 21:06:40.000000 python-taiga-1.1.0/taiga/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 21:07:15.901267 python-taiga-1.1.0/taiga/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-04-23 21:06:40.000000 python-taiga-1.1.0/taiga/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7535 2023-04-23 21:06:40.000000 python-taiga-1.1.0/taiga/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59220 2023-04-23 21:06:40.000000 python-taiga-1.1.0/taiga/models/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6204 2023-04-23 21:06:40.000000 python-taiga-1.1.0/taiga/requestmaker.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-23 21:06:40.000000 python-taiga-1.1.0/taiga/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 21:07:15.909267 python-taiga-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-04-23 21:06:40.000000 python-taiga-1.1.0/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-04-23 21:06:40.000000 python-taiga-1.1.0/tests/test_auth_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-04-23 21:06:40.000000 python-taiga-1.1.0/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-04-23 21:06:40.000000 python-taiga-1.1.0/tests/test_custom_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-04-23 21:06:40.000000 python-taiga-1.1.0/tests/test_epics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-04-23 21:06:40.000000 python-taiga-1.1.0/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-04-23 21:06:40.000000 python-taiga-1.1.0/tests/test_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-23 21:06:40.000000 python-taiga-1.1.0/tests/test_issue_statuses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-04-23 21:06:40.000000 python-taiga-1.1.0/tests/test_issue_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4248 2023-04-23 21:06:40.000000 python-taiga-1.1.0/tests/test_issues.py
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-04-23 21:06:40.000000 python-taiga-1.1.0/tests/test_memberships.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-04-23 21:06:40.000000 python-taiga-1.1.0/tests/test_milestones.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14396 2023-04-23 21:06:40.000000 python-taiga-1.1.0/tests/test_model_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-04-23 21:06:40.000000 python-taiga-1.1.0/tests/test_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-04-23 21:06:40.000000 python-taiga-1.1.0/tests/test_priorities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22340 2023-04-23 21:06:40.000000 python-taiga-1.1.0/tests/test_projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5872 2023-04-23 21:06:40.000000 python-taiga-1.1.0/tests/test_requestmaker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-04-23 21:06:40.000000 python-taiga-1.1.0/tests/test_roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-04-23 21:06:40.000000 python-taiga-1.1.0/tests/test_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-04-23 21:06:40.000000 python-taiga-1.1.0/tests/test_severities.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-04-23 21:06:40.000000 python-taiga-1.1.0/tests/test_task_statuses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-04-23 21:06:40.000000 python-taiga-1.1.0/tests/test_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6636 2023-04-23 21:06:40.000000 python-taiga-1.1.0/tests/test_user_stories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-04-23 21:06:40.000000 python-taiga-1.1.0/tests/test_users.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-04-23 21:06:40.000000 python-taiga-1.1.0/tests/test_userstory_statuses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-04-23 21:06:40.000000 python-taiga-1.1.0/tests/test_webhooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-04-23 21:06:40.000000 python-taiga-1.1.0/tests/test_wikilinks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-04-23 21:06:40.000000 python-taiga-1.1.0/tests/test_wikipages.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `python-taiga-1.0.0b1/taiga/models/base.py` & `python-taiga-1.1.0/taiga/models/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,44 +1,46 @@
 import re
 
-import six
-
 
 class SearchableList(list):
-
     def get(self, **query):
         for obj in self:
             ok_obj = True
-            for key, value in six.iteritems(query):
+            for key, value in query.items():
                 if key not in obj.__dict__ or obj.__dict__[key] != value:
                     ok_obj = False
             if ok_obj:
                 return obj
 
-    def filter(self, **query):
+    def filter(self, **query):  # noqa: A003
         result_objs = []
         for obj in self:
             ok_obj = True
-            for key, value in six.iteritems(query):
+            for key, value in query.items():
                 if key not in obj.__dict__ or obj.__dict__[key] != value:
                     ok_obj = False
             if ok_obj:
                 result_objs.append(obj)
         return result_objs
 
 
-class Resource(object):
-
+class Resource:
     def __init__(self, requester):
         self.requester = requester
 
 
 class ListResource(Resource):
+    """ListResource model
 
-    def list(self, pagination=True, page_size=None, page=None, **queryparams):
+    Base class for methods that operates on a list of resources (:py:meth:`list`, :py:meth:`get`, :py:meth:`delete`).
+
+    :param requester: :class:`Requester` instance
+    """
+
+    def list(self, pagination=True, page_size=None, page=None, **queryparams):  # noqa: A003
         """
         Retrieves a list of objects.
 
         By default uses local cache and remote pagination
 
         If pagination is used and no page is requested (the default), all the
         remote objects are retrieved and appended in a single list.
@@ -58,55 +60,48 @@
         :return: <SearchableList>
         """
         if page_size and pagination:
             try:
                 page_size = int(page_size)
             except (ValueError, TypeError):
                 page_size = 100
-            queryparams['page_size'] = page_size
-        result = self.requester.get(
-            self.instance.endpoint, query=queryparams, paginate=pagination
-        )
+            queryparams["page_size"] = page_size
+        if page and pagination:
+            queryparams["page"] = page
+        result = self.requester.get(self.instance.endpoint, query=queryparams, paginate=pagination)
         objects = SearchableList()
         objects.extend(self.parse_list(result.json()))
-        if result.headers.get('X-Pagination-Next', False) and not page:
+        if result.headers.get("X-Pagination-Next", False) and not page:
             next_page = 2
         else:
             next_page = None
         while next_page:
             pageparams = queryparams.copy()
-            pageparams['page'] = next_page
+            pageparams["page"] = next_page
             result = self.requester.get(
-                self.instance.endpoint, query=pageparams,
+                self.instance.endpoint,
+                query=pageparams,
             )
             objects.extend(self.parse_list(result.json()))
-            if result.headers.get('X-Pagination-Next', False):
+            if result.headers.get("X-Pagination-Next", False):
                 next_page += 1
             else:
                 next_page = None
         return objects
 
     def get(self, resource_id):
-        response = self.requester.get(
-            '/{endpoint}/{id}',
-            endpoint=self.instance.endpoint, id=resource_id
-        )
+        response = self.requester.get("/{endpoint}/{id}", endpoint=self.instance.endpoint, id=resource_id)
         return self.instance.parse(self.requester, response.json())
 
     def delete(self, resource_id):
-        self.requester.delete(
-            '/{endpoint}/{id}',
-            endpoint=self.instance.endpoint, id=resource_id
-        )
+        self.requester.delete("/{endpoint}/{id}", endpoint=self.instance.endpoint, id=resource_id)
         return self
 
     def _new_resource(self, **attrs):
-        response = self.requester.post(
-            self.instance.endpoint, **attrs
-        )
+        response = self.requester.post(self.instance.endpoint, **attrs)
         return self.instance.parse(self.requester, response.json())
 
     @classmethod
     def parse(cls, requester, entries):
         """Parse a JSON array into a list of model instances."""
         result_entries = SearchableList()
         for entry in entries:
@@ -120,132 +115,102 @@
             result_entries.append(self.instance.parse(self.requester, entry))
         return result_entries
 
 
 class InstanceResource(Resource):
     """InstanceResource model
 
+    Base class for methods that operates on a single resource (:py:meth:`update`, :py:meth:`patch`, :py:meth:`delete`).
+
     :param requester: :class:`Requester` instance
     :param params: :various parameters
     """
 
-    endpoint = ''
+    endpoint = ""
 
     parser = {}
 
     allowed_params = []
 
-    repr_attribute = 'name'
+    repr_attribute = "name"
 
     def __init__(self, requester, **params):
         import dateutil.parser
 
         self.requester = requester
-        for key, value in six.iteritems(params):
-            if key in ['created_date', 'modified_date']:
-                if re.compile(r'\d+-\d+-\d+T\d+:\d+:\d+\+0000').match(value):
+        for key, value in params.items():
+            if key in ["created_date", "modified_date"]:
+                if re.compile(r"\d+-\d+-\d+T\d+:\d+:\d+\+0000").match(value):
                     d = dateutil.parser.parse(value)
                     value = d.astimezone(dateutil.tz.tzlocal())
-            if six.PY2:
-                value = self._encode_element(value)
             setattr(self, key, value)
 
-    def _encode_element(self, element):
-        if isinstance(element, six.string_types):
-            return element.encode('utf-8')
-        elif isinstance(element, list):
-            for idx, value in enumerate(element):
-                element[idx] = self._encode_element(value)
-            return element
-        elif isinstance(element, dict):
-            for key, value in six.iteritems(element):
-                element[key] = self._encode_element(value)
-            return element
-        else:
-            return element
-
     def update(self, **args):
         """
         Update the current :class:`InstanceResource`
         """
         self_dict = self.to_dict()
         if args:
             self_dict = dict(list(self_dict.items()) + list(args.items()))
-        response = self.requester.put(
-            '/{endpoint}/{id}', endpoint=self.endpoint,
-            id=self.id, payload=self_dict
-        )
+        response = self.requester.put("/{endpoint}/{id}", endpoint=self.endpoint, id=self.id, payload=self_dict)
         obj_json = response.json()
-        if 'version' in obj_json:
-            self.__dict__['version'] = obj_json['version']
+        if "version" in obj_json:
+            self.__dict__["version"] = obj_json["version"]
         return self
 
     def patch(self, fields, **args):
         """
         Patch the current :class:`InstanceResource`
         """
-        self_dict = dict([(key, value) for (key, value) in
-                          self.to_dict().items()
-                          if key in fields])
+        self_dict = {key: value for (key, value) in self.to_dict().items() if key in fields}
         if args:
             self_dict = dict(list(self_dict.items()) + list(args.items()))
-        response = self.requester.patch(
-            '/{endpoint}/{id}', endpoint=self.endpoint,
-            id=self.id, payload=self_dict
-        )
+        response = self.requester.patch("/{endpoint}/{id}", endpoint=self.endpoint, id=self.id, payload=self_dict)
         obj_json = response.json()
-        if 'version' in obj_json:
-            self.__dict__['version'] = obj_json['version']
+        if "version" in obj_json:
+            self.__dict__["version"] = obj_json["version"]
         return self
 
     def delete(self):
         """
         Delete the current :class:`InstanceResource`
         """
-        self.requester.delete(
-            '/{endpoint}/{id}', endpoint=self.endpoint,
-            id=self.id
-        )
+        self.requester.delete("/{endpoint}/{id}", endpoint=self.endpoint, id=self.id)
         return self
 
     def to_dict(self):
         """
         Get a dictionary representation of :class:`InstanceResource`
         """
         self_dict = {}
-        for key, value in six.iteritems(self.__dict__):
+        for key, value in self.__dict__.items():
             if self.allowed_params and key in self.allowed_params:
                 self_dict[key] = value
         return self_dict
 
     @classmethod
     def parse(cls, requester, entry):
         """
         Turns a JSON object into a model instance.
         """
-        if not type(entry) is dict:
+        if type(entry) is not dict:
             return entry
-        for key_to_parse, cls_to_parse in six.iteritems(cls.parser):
+        for key_to_parse, cls_to_parse in cls.parser.items():
             if key_to_parse in entry:
-                entry[key_to_parse] = cls_to_parse.parse(
-                    requester, entry[key_to_parse]
-                )
+                entry[key_to_parse] = cls_to_parse.parse(requester, entry[key_to_parse])
         return cls(requester, **entry)
 
     def __repr__(self):
         try:
-            return '{0}({1})'.format(self.__class__.__name__, self.id)
+            return "{}({})".format(self.__class__.__name__, self.id)
         except AttributeError:
-            return '{0}({1})'.format(self.__class__.__name__, id(self))
+            return "{}({})".format(self.__class__.__name__, id(self))
 
     def __str__(self):
         return self._rp()
 
-    def __unicode__(self):
-        return self._rp().decode('utf-8')
-
     def _rp(self):
         attr = getattr(self, self.repr_attribute, None)
         if attr:
-            return '{0}'.format(attr)
+            return "{}".format(attr)
         else:
             return repr(self)
```

### Comparing `python-taiga-1.0.0b1/taiga/models/models.py` & `python-taiga-1.1.0/taiga/models/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,66 +1,60 @@
 import datetime
 import warnings
-
-import six
+from io import IOBase
 
 from .. import exceptions
 from .base import InstanceResource, ListResource
 
-if six.PY3:
-    from io import IOBase as file
-
 
 class CommentableResource(InstanceResource):
     """
     CommentableResource base class
     """
+
     def add_comment(self, comment):
         """
         Add a comment to the current element
 
         :param comment: the comment you want to insert
         """
         return self.update(comment=comment)
 
 
 class CustomAttributeResource(InstanceResource):
     """
     CustomAttributeResource base class
     """
-    def set_attribute(self, id, value, version=1):
+
+    def set_attribute(self, id, value, version=1):  # noqa: A002
         """
         Set attribute to a specific value
 
         :param id: id of the attribute
         :param value: value of the attribute
         :param version: version of the attribute (default = 1)
         """
         attributes = self._get_attributes(cache=True)
-        formatted_id = '{0}'.format(id)
-        attributes['attributes_values'][formatted_id] = value
+        formatted_id = "{}".format(id)
+        attributes["attributes_values"][formatted_id] = value
         response = self.requester.patch(
-            '/{endpoint}/custom-attributes-values/{id}',
-            endpoint=self.endpoint, id=self.id,
-            payload={
-                'attributes_values': attributes['attributes_values'],
-                'version': version
-            }
+            "/{endpoint}/custom-attributes-values/{id}",
+            endpoint=self.endpoint,
+            id=self.id,
+            payload={"attributes_values": attributes["attributes_values"], "version": version},
         )
         cache_key = self.requester.get_full_url(
-            '/{endpoint}/custom-attributes-values/{id}',
-            endpoint=self.endpoint, id=self.id
+            "/{endpoint}/custom-attributes-values/{id}", endpoint=self.endpoint, id=self.id
         )
         self.requester.cache.put(cache_key, response)
         return response.json()
 
     def _get_attributes(self, cache=False):
         response = self.requester.get(
-            '/{endpoint}/custom-attributes-values/{id}',
-            endpoint=self.endpoint, id=self.id, cache=cache
+            "/{endpoint}/custom-attributes-values/{id}", endpoint=self.endpoint, id=self.id, cache=cache
         )
         return response.json()
 
     def get_attributes(self):
         """
         Get all the attributes of the current object
         """
@@ -73,243 +67,245 @@
 
     :param requester: :class:`Requester` instance
     :param name: name of the custom attribute
     :param description: id of the current object
     :param order: order of the custom attribute
     :param project: :class:`Project` id
     """
-    repr_attribute = 'name'
 
-    allowed_params = [
-        'name', 'description', 'order', 'project'
-    ]
+    repr_attribute = "name"
+
+    allowed_params = ["name", "description", "order", "project"]
 
 
 class CustomAttributes(ListResource):
     """
     CustomAttributes factory base class
     """
+
     def create(self, project, name, **attrs):
         """
         Create a new :class:`CustomAttribute`.
 
         :param project: :class:`Project` id
         :param name: name of the custom attribute
         :param attrs: optional attributes of the custom attributes
         """
-        attrs.update(
-            {
-                'project': project, 'name': name
-            }
-        )
+        attrs.update({"project": project, "name": name})
         return self._new_resource(payload=attrs)
 
 
 class User(InstanceResource):
     """
     User model
     """
-    endpoint = 'users'
 
-    repr_attribute = 'full_name'
+    endpoint = "users"
+
+    repr_attribute = "full_name"
 
     def starred_projects(self):
         """
         Get a list of starred :class:`Project`.
         """
-        response = self.requester.get(
-            '/{endpoint}/{id}/starred', endpoint=self.endpoint,
-            id=self.id
-        )
+        response = self.requester.get("/{endpoint}/{id}/starred", endpoint=self.endpoint, id=self.id)
         return Projects.parse(self.requester, response.json())
 
 
 class Users(ListResource):
     """
     Users factory class
     """
+
     instance = User
 
 
 class Membership(InstanceResource):
     """
     Membership model
 
-    :param email: email of the :class:`Membership`
-    :param role: role of the :class:`Membership`
-    :param project: project of the :class:`Membership`
+    :param email: email of :class:`Membership`
+    :param role: role of :class:`Membership`
+    :param project: project of :class:`Membership`
     """
-    endpoint = 'memberships'
 
-    allowed_params = ['email', 'role', 'project']
+    endpoint = "memberships"
+
+    allowed_params = ["email", "role", "project"]
 
-    repr_attribute = 'email'
+    repr_attribute = "email"
 
 
 class Memberships(ListResource):
     """
     Memberships factory class
     """
+
     instance = Membership
 
     def create(self, project, email, role, **attrs):
         """
         Create a new :class:`Membership`.
 
         :param project: :class:`Project` id
-        :param email: email of the :class:`Membership`
-        :param role: role of the :class:`Membership`
-        :param attrs: optional attributes of the :class:`Membership`
+        :param email: email of :class:`Membership`
+        :param role: role of :class:`Membership`
+        :param attrs: optional attributes of :class:`Membership`
         """
-        attrs.update({'project': project, 'email': email, 'role': role})
+        attrs.update({"project": project, "email": email, "role": role})
         return self._new_resource(payload=attrs)
 
 
 class Priority(InstanceResource):
     """
     Priority model
 
-    :param name: name of the :class:`Priority`
+    :param name: name of :class:`Priority`
     :param color: color of the class:`Priority`
     :param order: order of the class:`Priority`
     :param project: project of the class:`Priority`
     """
-    endpoint = 'priorities'
 
-    allowed_params = ['name', 'color', 'order', 'project']
+    endpoint = "priorities"
+
+    allowed_params = ["name", "color", "order", "project"]
 
-    repr_attribute = 'name'
+    repr_attribute = "name"
 
 
 class Priorities(ListResource):
     """
     Priorities factory class
     """
+
     instance = Priority
 
     def create(self, project, name, **attrs):
         """
         Create a new :class:`Priority`.
 
         :param project: :class:`Project` id
         :param name: email of the priority
         :param attrs: optional attributes of the priority
         """
-        attrs.update({'project': project, 'name': name})
+        attrs.update({"project": project, "name": name})
         return self._new_resource(payload=attrs)
 
 
 class Attachment(InstanceResource):
     """
     Attachment base class
 
-    :param object_id: object_id of the :class:`Attachment`
-    :param project: project of the :class:`Attachment`
-    :param attached_file: attached_file of the :class:`Attachment`
-    :param description: description of the :class:`Attachment`
-    :param is_deprecated: is_deprecated of the :class:`Attachment`
+    :param object_id: object_id of :class:`Attachment`
+    :param project: project of :class:`Attachment`
+    :param attached_file: attached_file of :class:`Attachment`
+    :param description: description of :class:`Attachment`
+    :param is_deprecated: is_deprecated of :class:`Attachment`
     """
-    repr_attribute = 'subject'
 
-    allowed_params = [
-        'object_id', 'project', 'attached_file',
-        'description', 'is_deprecated', 'size',
-        'name', 'url'
-    ]
+    repr_attribute = "subject"
+
+    allowed_params = ["object_id", "project", "attached_file", "description", "is_deprecated", "size", "name", "url"]
 
 
 class Attachments(ListResource):
     """
     Attachments factory base class
     """
+
     def create(self, project, object_id, attached_file, **attrs):
         """
         Create a new :class:`Attachment`.
 
         :param project: :class:`Project` id
         :param object_id: id of the current object
         :param ref: :class:`Task` reference
         :param attached_file: file path that you want to upload
         :param attrs: optional attributes for the :class:`Attachment`
         """
-        attrs.update({'project': project, 'object_id': object_id})
+        attrs.update({"project": project, "object_id": object_id})
 
-        if isinstance(attached_file, file):
+        if isinstance(attached_file, IOBase):
             attachment = attached_file
-        elif isinstance(attached_file, six.string_types):
+        elif isinstance(attached_file, str):
             try:
-                attachment = open(attached_file, 'rb')
-            except IOError:
-                raise exceptions.TaigaException(
-                    "Attachment must be a IOBase or a path to an existing file"
-                )
+                attachment = open(attached_file, "rb")
+            except OSError:
+                raise exceptions.TaigaException("Attachment must be a IOBase or a path to an existing file")
         else:
-            raise exceptions.TaigaException(
-                "Attachment must be a IOBase or a path to an existing file"
-            )
-
-        return self._new_resource(
-            files={'attached_file': attachment},
-            payload=attrs
-        )
+            raise exceptions.TaigaException("Attachment must be a IOBase or a path to an existing file")
+
+        return self._new_resource(files={"attached_file": attachment}, payload=attrs)
 
 
 class UserStoryAttachment(Attachment):
     """
     UserStoryAttachment class
     """
-    endpoint = 'userstories/attachments'
+
+    endpoint = "userstories/attachments"
 
 
 class UserStoryAttachments(Attachments):
     """
     UserStoryAttachments factory class
     """
+
     instance = UserStoryAttachment
 
 
 class EpicAttachment(Attachment):
     """
     EpicAttachment class
     """
-    endpoint = 'epics/attachments'
+
+    endpoint = "epics/attachments"
 
 
 class EpicAttachments(Attachments):
     """
     EpicAttachments factory class
     """
+
     instance = EpicAttachment
 
 
 class Epic(CustomAttributeResource, CommentableResource):
     """
     Epic model
 
-    :param assigned_to: assigned to property of the :class:`Epic`
-    :param blocked_note: blocked note of the :class:`Epic`
-    :param description: description of of the :class:`Epic`
-    :param is_blocked: is blocked property of the :class:`Epic`
-    :param is_closed: is closed property of the :class:`Epic`
-    :param color: the color of the :class:`Epic`
-    :param project: the project of the :class:`TaskStatus`
-    :param subject: subject of the :class:`TaskStatus`
-    :param tags: tags of the :class:`TaskStatus`
-    :param watchers: watchers of the :class:`TaskStatus`
-    :param version: version of the :class:`Epic`
+    :param assigned_to: assigned to property of :class:`Epic`
+    :param blocked_note: blocked note of :class:`Epic`
+    :param description: description of :class:`Epic` (not available in the :py:meth:`Epics.list` response)
+    :param is_blocked: is blocked property of :class:`Epic`
+    :param is_closed: is closed property of :class:`Epic`
+    :param color: the color of :class:`Epic`
+    :param project: the project of :class:`TaskStatus`
+    :param subject: subject of :class:`TaskStatus`
+    :param tags: tags of :class:`TaskStatus`
+    :param watchers: watchers of :class:`TaskStatus`
+    :param version: version of :class:`Epic`
     """
 
-    endpoint = 'epics'
+    endpoint = "epics"
 
-    repr_attribute = 'subject'
+    repr_attribute = "subject"
 
     allowed_params = [
-        'assigned_to', 'blocked_note', 'description',
-        'is_blocked', 'is_closed', 'color', 'project',
-        'subject', 'tags', 'watchers', 'version'
+        "assigned_to",
+        "blocked_note",
+        "description",
+        "is_blocked",
+        "is_closed",
+        "color",
+        "project",
+        "subject",
+        "tags",
+        "watchers",
+        "version",
     ]
 
     def list_user_stories(self, **queryparams):
         """
         Returns the :class:`UserStory` list of the project.
         """
         return UserStories(self.requester).list(epic=self.id, **queryparams)
@@ -323,125 +319,137 @@
     def attach(self, attached_file, **attrs):
         """
         Attach a file to the :class:`Epic`
 
         :param attached_file: file path to attach
         :param attrs: optional attributes for the attached file
         """
-        return EpicAttachments(self.requester).create(
-            self.project, self.id,
-            attached_file, **attrs
-        )
+        return EpicAttachments(self.requester).create(self.project, self.id, attached_file, **attrs)
 
 
 class Epics(ListResource):
     """
     Epics factory class
     """
+
     instance = Epic
 
     def create(self, project, subject, **attrs):
         """
         Create a new :class:`Epic`.
 
         :param project: :class:`Project` id
-        :param subject: subject of the :class:`Epic`
-        :param attrs: optional attributes of the :class:`Epic`
+        :param subject: subject of :class:`Epic`
+        :param attrs: optional attributes of :class:`Epic`
         """
-        attrs.update({'project': project, 'subject': subject})
+        attrs.update({"project": project, "subject": subject})
         return self._new_resource(payload=attrs)
 
 
 class EpicStatus(InstanceResource):
     """
     Taiga Epic Status model
 
-    :param color: the color of the :class:`EpicStatus`
-    :param is_closed: closed property of the :class:`EpicStatus`
-    :param name: The name of the :class:`EpicStatus`
-    :param order: order of the :class:`EpicStatus`
-    :param project: the Taiga project of the :class:`EpicStatus`
-    :param slug: the slug of the :class:`EpicStatus`
+    :param color: the color of :class:`EpicStatus`
+    :param is_closed: closed property of :class:`EpicStatus`
+    :param name: The name of :class:`EpicStatus`
+    :param order: order of :class:`EpicStatus`
+    :param project: the Taiga project of :class:`EpicStatus`
+    :param slug: the slug of :class:`EpicStatus`
     """
 
-    repr_attribute = 'subject'
+    repr_attribute = "subject"
 
-    endpoint = 'epic-statuses'
+    endpoint = "epic-statuses"
 
-    allowed_params = [
-        'color', 'is_closed', 'name', 'order', 'project', 'slug`'
-    ]
+    allowed_params = ["color", "is_closed", "name", "order", "project", "slug`"]
 
 
 class EpicStatuses(ListResource):
-
     instance = EpicStatus
 
     def create(self, project, name, **attrs):
         """
         Create a new :class:`EpicStatus`.
 
         :param project: :class:`Project` id
-        :param name: name of the :class:`EpicStatus`
-        :param attrs: optional attributes of the :class:`EpicStatus`
+        :param name: name of :class:`EpicStatus`
+        :param attrs: optional attributes of :class:`EpicStatus`
         """
-        attrs.update({'project': project, 'name': name})
+        attrs.update({"project": project, "name": name})
         return self._new_resource(payload=attrs)
 
 
 class UserStory(CustomAttributeResource, CommentableResource):
     """
     User Story model
 
-    :param assigned_to: assigned to of the :class:`UserStory`
-    :param assigned_users: additional users assigned to of the :class:`UserStory`
-    :param backlog_order: backlog order of the :class:`UserStory`
-    :param blocked_note: blocked note of the :class:`UserStory`
-    :param version: version of the :class:`UserStory`
-    :param client_requirement: client requirement of the :class:`UserStory`
-    :param description: description of the :class:`UserStory`
-    :param is_blocked: is blocked of the :class:`UserStory`
-    :param kanban_order: kanban order of the :class:`UserStory`
-    :param milestone: milestone of the :class:`UserStory`
-    :param points: points of the :class:`UserStory`
-    :param project: project of the :class:`UserStory`
-    :param sprint_order: sprint order of the :class:`UserStory`
-    :param status: status of the :class:`UserStory`
-    :param subject: subject of the :class:`UserStory`
-    :param tags: tags of the :class:`UserStory`
-    :param team_requirement: team requirement of the :class:`UserStory`
-    :param watchers: watchers of the :class:`UserStory`
+    :param assigned_to: assigned to of :class:`UserStory`
+    :param assigned_users: additional users assigned to of :class:`UserStory`
+    :param backlog_order: backlog order of :class:`UserStory`
+    :param blocked_note: blocked note of :class:`UserStory`
+    :param version: version of :class:`UserStory`
+    :param client_requirement: client requirement of :class:`UserStory`
+    :param description: description of :class:`UserStory` (not available in the :py:meth:`UserStories.list` response)
+    :param is_blocked: is blocked of :class:`UserStory`
+    :param kanban_order: kanban order of :class:`UserStory`
+    :param milestone: milestone of :class:`UserStory`
+    :param points: points of :class:`UserStory`
+    :param project: project of :class:`UserStory`
+    :param sprint_order: sprint order of :class:`UserStory`
+    :param status: status of :class:`UserStory`
+    :param subject: subject of :class:`UserStory`
+    :param tags: tags of :class:`UserStory`
+    :param team_requirement: team requirement of :class:`UserStory`
+    :param watchers: watchers of :class:`UserStory`
     :param due_date: :class:`UserStory` due date
+    :param generated_from_issue: :class:`UserStory` parent issue
+    :param generated_from_task: :class:`UserStory` parent task
     """
-    endpoint = 'userstories'
 
-    repr_attribute = 'subject'
-    element_type = 'User Story'
-    element_shortcut = 'us'
+    endpoint = "userstories"
 
-    allowed_params = [
-        'assigned_to', 'assigned_users', 'backlog_order', 'blocked_note', 'version',
-        'client_requirement', 'description', 'is_blocked', 'is_closed',
-        'kanban_order', 'milestone', 'points', 'project', 'sprint_order',
-        'status', 'subject', 'tags', 'team_requirement', 'watchers', 'due_date',
+    repr_attribute = "subject"
+    element_type = "User Story"
+    element_shortcut = "us"
 
+    allowed_params = [
+        "assigned_to",
+        "assigned_users",
+        "backlog_order",
+        "blocked_note",
+        "version",
+        "client_requirement",
+        "description",
+        "is_blocked",
+        "is_closed",
+        "kanban_order",
+        "milestone",
+        "points",
+        "project",
+        "sprint_order",
+        "status",
+        "subject",
+        "tags",
+        "team_requirement",
+        "watchers",
+        "due_date",
+        "generated_from_issue",
+        "generated_from_task",
     ]
 
     def add_task(self, subject, status, **attrs):
         """
         Add a :class:`Task` to the current :class:`UserStory` and return it.
-        :param subject: subject of the :class:`Task`
-        :param status: status of the :class:`Task`
+        :param subject: subject of :class:`Task`
+        :param status: status of :class:`Task`
         :param attrs: optional attributes for :class:`Task`
 
         """
-        return Tasks(self.requester).create(
-            self.project, subject, status,
-            user_story=self.id, **attrs
-        )
+        return Tasks(self.requester).create(self.project, subject, status, user_story=self.id, **attrs)
 
     def list_tasks(self):
         """
         Get a list of :class:`Task` in the current :class:`UserStory`.
         """
         return Tasks(self.requester).list(user_story=self.id)
 
@@ -454,283 +462,295 @@
     def attach(self, attached_file, **attrs):
         """
         Attach a file to the :class:`UserStory`
 
         :param attached_file: file path to attach
         :param attrs: optional attributes for the attached file
         """
-        return UserStoryAttachments(self.requester).create(
-            self.project, self.id,
-            attached_file, **attrs
-        )
+        return UserStoryAttachments(self.requester).create(self.project, self.id, attached_file, **attrs)
 
 
 class UserStories(ListResource):
     """
     UserStories factory class
     """
+
     instance = UserStory
 
     def create(self, project, subject, **attrs):
         """
         Create a new :class:`UserStory`.
 
         :param project: :class:`Project` id
-        :param subject: subject of the :class:`UserStory`
-        :param attrs: optional attributes of the :class:`UserStory`
+        :param subject: subject of :class:`UserStory`
+        :param attrs: optional attributes of :class:`UserStory`
         """
-        attrs.update({'project': project, 'subject': subject})
+        attrs.update({"project": project, "subject": subject})
         return self._new_resource(payload=attrs)
 
     def import_(self, project, subject, status, **attrs):
-        attrs.update(
-            {
-                'project': project,
-                'subject': subject,
-                'status': status
-            }
+        attrs.update({"project": project, "subject": subject, "status": status})
+        response = self.requester.post(
+            "/{endpoint}/{id}/{type}", endpoint="importer", id=project, type="us", payload=attrs
         )
-        response = self.requester.post('/{endpoint}/{id}/{type}',
-                                       endpoint="importer", id=project,
-                                       type="us", payload=attrs)
         return self.instance.parse(self.requester, response.json())
 
 
 class UserStoryStatus(InstanceResource):
     """
     Taiga User Story Status model
 
-    :param color: the color of the :class:`UserStoryStatus`
-    :param is_closed: closed property of the :class:`UserStoryStatus`
-    :param name: The name of the :class:`UserStoryStatus`
-    :param order: order of the :class:`UserStoryStatus`
-    :param project: the Taiga project of the :class:`UserStoryStatus`
-    :param wip_limit: wip limit of the :class:`UserStoryStatus`
+    :param color: the color of :class:`UserStoryStatus`
+    :param is_closed: closed property of :class:`UserStoryStatus`
+    :param name: The name of :class:`UserStoryStatus`
+    :param order: order of :class:`UserStoryStatus`
+    :param project: the Taiga project of :class:`UserStoryStatus`
+    :param wip_limit: wip limit of :class:`UserStoryStatus`
     """
 
-    repr_attribute = 'subject'
+    repr_attribute = "subject"
 
-    endpoint = 'userstory-statuses'
+    endpoint = "userstory-statuses"
 
-    allowed_params = [
-        'color', 'is_closed', 'name', 'order', 'project', 'wip_limit'
-    ]
+    allowed_params = ["color", "is_closed", "name", "order", "project", "wip_limit"]
 
 
 class UserStoryStatuses(ListResource):
-
     instance = UserStoryStatus
 
     def create(self, project, name, **attrs):
         """
         Create a new :class:`UserStoryStatus`.
 
         :param project: :class:`Project` id
-        :param name: name of the :class:`UserStoryStatus`
-        :param attrs: optional attributes of the :class:`UserStoryStatus`
+        :param name: name of :class:`UserStoryStatus`
+        :param attrs: optional attributes of :class:`UserStoryStatus`
         """
-        attrs.update({'project': project, 'name': name})
+        attrs.update({"project": project, "name": name})
         return self._new_resource(payload=attrs)
 
 
 class Point(InstanceResource):
     """
     Taiga Point model
 
-    :param color: the color of the :class:`Point`
-    :param value: value of the :class:`Point`
-    :param name: name of the :class:`Point`
-    :param order: the order of the :class:`Point`
-    :param project: the Taiga project of the :class:`Point`
+    :param color: the color of :class:`Point`
+    :param value: value of :class:`Point`
+    :param name: name of :class:`Point`
+    :param order: the order of :class:`Point`
+    :param project: the Taiga project of :class:`Point`
     """
 
-    endpoint = 'points'
+    endpoint = "points"
 
-    repr_attribute = 'subject'
+    repr_attribute = "subject"
 
-    allowed_params = ['color', 'value', 'name', 'order', 'project']
+    allowed_params = ["color", "value", "name", "order", "project"]
 
 
 class Points(ListResource):
     """
     Points factory
     """
+
     instance = Point
 
     def create(self, project, name, value, **attrs):
         """
         Create a new :class:`UserStoryStatus`.
 
         :param project: :class:`Project` id
-        :param name: name of the :class:`Point`
-        :param value: value of the :class:`Point`
-        :param attrs: optional attributes of the :class:`Point`
+        :param name: name of :class:`Point`
+        :param value: value of :class:`Point`
+        :param attrs: optional attributes of :class:`Point`
         """
-        attrs.update({'project': project, 'name': name, 'value': value})
+        attrs.update({"project": project, "name": name, "value": value})
         return self._new_resource(payload=attrs)
 
 
 class Milestone(InstanceResource):
     """
     Milestone model
 
-    :param name: the name of the :class:`Milestone`
-    :param project: the Taiga project  of the :class:`Milestone`
-    :param estimated_start: the estimated start of the :class:`Milestone`
-    :param estimated_finish: the estimated finish  of the :class:`Milestone`
-    :param disponibility: the disponibility  of the :class:`Milestone`
+    :param name: the name of :class:`Milestone`
+    :param project: the Taiga project  of :class:`Milestone`
+    :param estimated_start: the estimated start of :class:`Milestone`
+    :param estimated_finish: the estimated finish  of :class:`Milestone`
+    :param disponibility: the disponibility  of :class:`Milestone`
     """
-    endpoint = 'milestones'
+
+    endpoint = "milestones"
 
     allowed_params = [
-        'name', 'project', 'estimated_start', 'estimated_finish',
-        'disponibility', 'slug', 'order', 'watchers'
+        "name",
+        "project",
+        "estimated_start",
+        "estimated_finish",
+        "disponibility",
+        "slug",
+        "order",
+        "watchers",
     ]
 
     parser = {
-        'user_stories': UserStories,
+        "user_stories": UserStories,
     }
 
     def stats(self):
         """
         Get the stats for the current :class:`Milestone`
         """
-        response = self.requester.get(
-            '/{endpoint}/{id}/stats',
-            endpoint=self.endpoint, id=self.id
-        )
+        response = self.requester.get("/{endpoint}/{id}/stats", endpoint=self.endpoint, id=self.id)
         return response.json()
 
 
 class Milestones(ListResource):
     """
     Milestones factory
     """
+
     instance = Milestone
 
-    def create(self, project, name, estimated_start,
-               estimated_finish, **attrs):
+    def create(self, project, name, estimated_start, estimated_finish, **attrs):
         """
         Create a new :class:`Milestone`.
 
         :param project: :class:`Project` id
-        :param name: name of the :class:`Milestone`
-        :param estimated_start: est. start time of the :class:`Milestone`
-        :param estimated_finish: est. finish time of the :class:`Milestone`
-        :param attrs: optional attributes of the :class:`Milestone`
+        :param name: name of :class:`Milestone`
+        :param estimated_start: est. start time of :class:`Milestone`
+        :param estimated_finish: est. finish time of :class:`Milestone`
+        :param attrs: optional attributes of :class:`Milestone`
         """
         if isinstance(estimated_start, datetime.datetime):
-            estimated_start = estimated_start.strftime('%Y-%m-%d')
+            estimated_start = estimated_start.strftime("%Y-%m-%d")
         if isinstance(estimated_finish, datetime.datetime):
-            estimated_finish = estimated_finish.strftime('%Y-%m-%d')
-        attrs.update({
-            'project': project,
-            'name': name,
-            'estimated_start': estimated_start,
-            'estimated_finish': estimated_finish
-        })
+            estimated_finish = estimated_finish.strftime("%Y-%m-%d")
+        attrs.update(
+            {
+                "project": project,
+                "name": name,
+                "estimated_start": estimated_start,
+                "estimated_finish": estimated_finish,
+            }
+        )
         return self._new_resource(payload=attrs)
 
-    def import_(self, project, name, estimated_start,
-                estimated_finish, **attrs):
+    def import_(self, project, name, estimated_start, estimated_finish, **attrs):
         if isinstance(estimated_start, datetime.datetime):
-            estimated_start = estimated_start.strftime('%Y-%m-%d')
+            estimated_start = estimated_start.strftime("%Y-%m-%d")
         if isinstance(estimated_finish, datetime.datetime):
-            estimated_finish = estimated_finish.strftime('%Y-%m-%d')
-        attrs.update({
-            'project': project,
-            'name': name,
-            'estimated_start': estimated_start,
-            'estimated_finish': estimated_finish
-        })
-        response = self.requester.post('/{endpoint}/{id}/{type}',
-                                       endpoint="importer", id=project,
-                                       type="milestone", payload=attrs)
+            estimated_finish = estimated_finish.strftime("%Y-%m-%d")
+        attrs.update(
+            {
+                "project": project,
+                "name": name,
+                "estimated_start": estimated_start,
+                "estimated_finish": estimated_finish,
+            }
+        )
+        response = self.requester.post(
+            "/{endpoint}/{id}/{type}", endpoint="importer", id=project, type="milestone", payload=attrs
+        )
         return self.instance.parse(self.requester, response.json())
 
 
 class TaskStatus(InstanceResource):
     """
     Task Status model
 
-    :param name: the name of the :class:`TaskStatus`
-    :param color: the color of the :class:`TaskStatus`
-    :param order: the order of the :class:`TaskStatus`
-    :param project: the project  of the :class:`TaskStatus`
-    :param is_closed: the is closed property of the :class:`TaskStatus`
+    :param name: the name of :class:`TaskStatus`
+    :param color: the color of :class:`TaskStatus`
+    :param order: the order of :class:`TaskStatus`
+    :param project: the project  of :class:`TaskStatus`
+    :param is_closed: the is closed property of :class:`TaskStatus`
     """
-    endpoint = 'task-statuses'
 
-    allowed_params = ['name', 'color', 'order', 'project', 'is_closed']
+    endpoint = "task-statuses"
 
+    allowed_params = ["name", "color", "order", "project", "is_closed"]
 
-class TaskStatuses(ListResource):
 
+class TaskStatuses(ListResource):
     instance = TaskStatus
 
     def create(self, project, name, **attrs):
         """
         Create a new :class:`TaskStatus`.
 
         :param project: :class:`Project` id
-        :param name: name of the :class:`TaskStatus`
-        :param attrs: optional attributes of the :class:`TaskStatus`
+        :param name: name of :class:`TaskStatus`
+        :param attrs: optional attributes of :class:`TaskStatus`
         """
-        attrs.update({'project': project, 'name': name})
+        attrs.update({"project": project, "name": name})
         return self._new_resource(payload=attrs)
 
 
 class TaskAttachment(Attachment):
     """
     TaskAttachment model
     """
-    endpoint = 'tasks/attachments'
+
+    endpoint = "tasks/attachments"
 
 
 class TaskAttachments(Attachments):
     """
     TaskAttachments factory
     """
+
     instance = TaskAttachment
 
 
 class Task(CustomAttributeResource, CommentableResource):
     """
     Task model
 
-    :param assigned_to: assigned to property of the :class:`TaskStatus`
-    :param blocked_note: blocked note of the :class:`TaskStatus`
-    :param description: description of of the :class:`TaskStatus`
-    :param version: version of the :class:`TaskStatus`
-    :param is_blocked: is blocked property of the :class:`TaskStatus`
-    :param milestone: milestone property of the :class:`TaskStatus`
-    :param project: the project of the :class:`TaskStatus`
-    :param user_story: the user story of the :class:`TaskStatus`
-    :param status: status of the :class:`TaskStatus`
-    :param subject: subject of the :class:`TaskStatus`
-    :param tags: tags of the :class:`TaskStatus`
-    :param us_order: the use order of the :class:`TaskStatus`
-    :param taskboard_order: the taskboard order of the :class:`TaskStatus`
-    :param is_iocaine: the is iocaine of the :class:`TaskStatus`
-    :param external_reference: external reference of the :class:`TaskStatus`
-    :param watchers: watchers of the :class:`TaskStatus`
+    :param assigned_to: assigned to property of :class:`TaskStatus`
+    :param blocked_note: blocked note of :class:`TaskStatus`
+    :param description: description of of :class:`TaskStatus` (not available in the :py:meth:`Tasks.list` response)
+    :param version: version of :class:`TaskStatus`
+    :param is_blocked: is blocked property of :class:`TaskStatus`
+    :param milestone: milestone property of :class:`TaskStatus`
+    :param project: the project of :class:`TaskStatus`
+    :param user_story: the user story of :class:`TaskStatus`
+    :param status: status of :class:`TaskStatus`
+    :param subject: subject of :class:`TaskStatus`
+    :param tags: tags of :class:`TaskStatus`
+    :param us_order: the use order of :class:`TaskStatus`
+    :param taskboard_order: the taskboard order of :class:`TaskStatus`
+    :param is_iocaine: the is iocaine of :class:`TaskStatus`
+    :param external_reference: external reference of :class:`TaskStatus`
+    :param watchers: watchers of :class:`TaskStatus`
     :param due_date: :class:`Task` due date
     """
 
-    endpoint = 'tasks'
+    endpoint = "tasks"
 
-    repr_attribute = 'subject'
-    element_type = 'Task'
-    element_shortcut = 'task'
+    repr_attribute = "subject"
+    element_type = "Task"
+    element_shortcut = "task"
 
     allowed_params = [
-        'assigned_to', 'blocked_note', 'description', 'version',
-        'is_blocked', 'is_closed', 'milestone', 'project', 'user_story',
-        'status', 'subject', 'tags', 'us_order', 'taskboard_order',
-        'is_iocaine', 'external_reference', 'watchers'
+        "assigned_to",
+        "blocked_note",
+        "description",
+        "version",
+        "is_blocked",
+        "is_closed",
+        "milestone",
+        "project",
+        "user_story",
+        "status",
+        "subject",
+        "tags",
+        "us_order",
+        "taskboard_order",
+        "is_iocaine",
+        "external_reference",
+        "watchers",
     ]
 
     def list_attachments(self):
         """
         Get a list of :class:`TaskAttachment`.
         """
         return TaskAttachments(self.requester).list(object_id=self.id)
@@ -738,728 +758,708 @@
     def attach(self, attached_file, **attrs):
         """
         Attach a file to the :class:`Task`
 
         :param attached_file: file path to attach
         :param attrs: optional attributes for the attached file
         """
-        return TaskAttachments(self.requester).create(
-            self.project, self.id,
-            attached_file, **attrs
-        )
+        return TaskAttachments(self.requester).create(self.project, self.id, attached_file, **attrs)
 
 
 class Tasks(ListResource):
     """
     Tasks factory
     """
+
     instance = Task
 
     def create(self, project, subject, status, **attrs):
         """
         Create a new :class:`Task`.
 
         :param project: :class:`Project` id
-        :param subject: subject of the :class:`Task`
-        :param status: status of the :class:`Task`
-        :param attrs: optional attributes of the :class:`Task`
+        :param subject: subject of :class:`Task`
+        :param status: status of :class:`Task`
+        :param attrs: optional attributes of :class:`Task`
         """
-        attrs.update(
-            {
-                'project': project, 'subject': subject,
-                'status': status
-            }
-        )
+        attrs.update({"project": project, "subject": subject, "status": status})
         return self._new_resource(payload=attrs)
 
     def import_(self, project, subject, status, **attrs):
-        attrs.update(
-            {
-                'project': project,
-                'subject': subject,
-                'status': status
-            }
+        attrs.update({"project": project, "subject": subject, "status": status})
+        response = self.requester.post(
+            "/{endpoint}/{id}/{type}", endpoint="importer", id=project, type="task", payload=attrs
         )
-        response = self.requester.post('/{endpoint}/{id}/{type}',
-                                       endpoint="importer", id=project,
-                                       type="task", payload=attrs)
         return self.instance.parse(self.requester, response.json())
 
 
 class IssueType(InstanceResource):
     """
     IssueType model
 
-    :param name: name of the :class:`IssueType`
-    :param color: color of the :class:`IssueType`
-    :param order: order of the :class:`IssueType`
-    :param project: the taiga project of the :class:`IssueType`
+    :param name: name of :class:`IssueType`
+    :param color: color of :class:`IssueType`
+    :param order: order of :class:`IssueType`
+    :param project: the taiga project of :class:`IssueType`
     """
-    endpoint = 'issue-types'
 
-    allowed_params = ['name', 'color', 'order', 'project']
+    endpoint = "issue-types"
+
+    allowed_params = ["name", "color", "order", "project"]
 
 
 class IssueTypes(ListResource):
     """
     IssueTypes factory
     """
+
     instance = IssueType
 
     def create(self, project, name, **attrs):
-        attrs.update({'project': project, 'name': name})
+        attrs.update({"project": project, "name": name})
         return self._new_resource(payload=attrs)
 
 
 class IssueStatus(InstanceResource):
     """
     Issue Status model
 
-    :param name: name of the :class:`IssueStatus`
-    :param color: color of the :class:`IssueStatus`
-    :param order: order of the :class:`IssueStatus`
-    :param project: the taiga project of the :class:`IssueStatus`
-    :param is_closed: is closed property of the :class:`IssueStatus`
+    :param name: name of :class:`IssueStatus`
+    :param color: color of :class:`IssueStatus`
+    :param order: order of :class:`IssueStatus`
+    :param project: the taiga project of :class:`IssueStatus`
+    :param is_closed: is closed property of :class:`IssueStatus`
     """
 
-    endpoint = 'issue-statuses'
+    endpoint = "issue-statuses"
 
-    allowed_params = ['name', 'color', 'order', 'project', 'is_closed']
+    allowed_params = ["name", "color", "order", "project", "is_closed"]
 
 
 class IssueStatuses(ListResource):
     """
     IssueStatuses factory
     """
+
     instance = IssueStatus
 
     def create(self, project, name, **attrs):
-        attrs.update({'project': project, 'name': name})
+        attrs.update({"project": project, "name": name})
         return self._new_resource(payload=attrs)
 
 
 class IssueAttachment(Attachment):
     """
     IssueAttachment model
     """
-    endpoint = 'issues/attachments'
+
+    endpoint = "issues/attachments"
 
 
 class IssueAttachments(Attachments):
     """
     IssueAttachments factory
     """
+
     instance = IssueAttachment
 
 
 class Issue(CustomAttributeResource, CommentableResource):
     """Issue model
 
     :param requester: :class:`Requester` instance
     :param assigned_to: :class:`User` id this issue is assigned to
-    :param description: description of the issue
+    :param description: description of the issue (not available in the :py:meth:`Issues.list` response)
     :param is_blocked: set if this issue is blocked or not
     :param milestone: :class:`Milestone` id
     :param project: :class:`Project` id
     :param status: :class:`Status` id
     :param severity: class:`Severity` id
     :param priority: class:`Priority` id
     :param type: class:`Type` id
     :param subject: subject of the issue
     :param tags: array of tags
     :param watchers: array of watchers id
     :param due_date: :class:`Issue` due date
     """
 
-    endpoint = 'issues'
+    endpoint = "issues"
 
-    repr_attribute = 'subject'
-    element_type = 'Issue'
-    element_shortcut = 'issue'
+    repr_attribute = "subject"
+    element_type = "Issue"
+    element_shortcut = "issue"
 
     allowed_params = [
-        'assigned_to', 'blocked_note', 'description', 'version',
-        'is_blocked', 'is_closed', 'milestone', 'project', 'status',
-        'severity', 'priority', 'type', 'subject', 'tags', 'watchers',
+        "assigned_to",
+        "blocked_note",
+        "description",
+        "version",
+        "is_blocked",
+        "is_closed",
+        "milestone",
+        "project",
+        "status",
+        "severity",
+        "priority",
+        "type",
+        "subject",
+        "tags",
+        "watchers",
     ]
 
     def list_attachments(self):
         """
         Get a list of :class:`IssueAttachment`.
         """
         return IssueAttachments(self.requester).list(object_id=self.id)
 
     def upvote(self):
         """
         Upvote :class:`Issue`.
         """
-        self.requester.post(
-            '/{endpoint}/{id}/upvote',
-            endpoint=self.endpoint, id=self.id
-        )
+        self.requester.post("/{endpoint}/{id}/upvote", endpoint=self.endpoint, id=self.id)
         return self
 
     def downvote(self):
         """
         Downvote :class:`Issue`.
         """
-        self.requester.post(
-            '/{endpoint}/{id}/downvote',
-            endpoint=self.endpoint, id=self.id
-        )
+        self.requester.post("/{endpoint}/{id}/downvote", endpoint=self.endpoint, id=self.id)
         return self
 
     def attach(self, attached_file, **attrs):
         """
         Attach a file to the :class:`Issue`
 
         :param attached_file: file path to attach
         :param attrs: optional attributes for the attached file
         """
-        return IssueAttachments(self.requester).create(
-            self.project, self.id,
-            attached_file, **attrs
-        )
+        return IssueAttachments(self.requester).create(self.project, self.id, attached_file, **attrs)
 
 
 class Issues(ListResource):
-
     instance = Issue
 
-    def create(self, project, subject, priority, status,
-               issue_type, severity, **attrs):
+    def create(self, project, subject, priority, status, issue_type, severity, **attrs):
         """
         Create a new :class:`Task`.
 
         :param project: :class:`Project` id
-        :param subject: subject of the :class:`Issue`
-        :param priority: priority of the :class:`Issue`
-        :param status: status of the :class:`Issue`
-        :param issue_type: Issue type of the :class:`Issue`
-        :param severity: severity of the :class:`Issue`
-        :param attrs: optional attributes of the :class:`Task`
+        :param subject: subject of :class:`Issue`
+        :param priority: priority of :class:`Issue`
+        :param status: status of :class:`Issue`
+        :param issue_type: Issue type of :class:`Issue`
+        :param severity: severity of :class:`Issue`
+        :param attrs: optional attributes of :class:`Task`
         """
         attrs.update(
             {
-                'project': project, 'subject': subject,
-                'priority': priority, 'status': status,
-                'type': issue_type, 'severity': severity
+                "project": project,
+                "subject": subject,
+                "priority": priority,
+                "status": status,
+                "type": issue_type,
+                "severity": severity,
             }
         )
         return self._new_resource(payload=attrs)
 
-    def import_(self, project, subject, priority, status,
-                issue_type, severity, **attrs):
+    def import_(self, project, subject, priority, status, issue_type, severity, **attrs):
         attrs.update(
             {
-                'project': project, 'subject': subject,
-                'priority': priority, 'status': status,
-                'type': issue_type, 'severity': severity
+                "project": project,
+                "subject": subject,
+                "priority": priority,
+                "status": status,
+                "type": issue_type,
+                "severity": severity,
             }
         )
-        response = self.requester.post('/{endpoint}/{id}/{type}',
-                                       endpoint="importer", id=project,
-                                       type="issue", payload=attrs)
+        response = self.requester.post(
+            "/{endpoint}/{id}/{type}", endpoint="importer", id=project, type="issue", payload=attrs
+        )
         return self.instance.parse(self.requester, response.json())
 
 
 class IssueAttribute(CustomAttribute):
     """
     IssueAttribute model
     """
-    endpoint = 'issue-custom-attributes'
+
+    endpoint = "issue-custom-attributes"
 
 
 class IssueAttributes(CustomAttributes):
     """
     IssueAttributes factory
     """
+
     instance = IssueAttribute
 
 
 class TaskAttribute(CustomAttribute):
     """
     TaskAttribute model
     """
-    endpoint = 'task-custom-attributes'
+
+    endpoint = "task-custom-attributes"
 
 
 class TaskAttributes(CustomAttributes):
     """
     TaskAttributes factory
     """
+
     instance = TaskAttribute
 
 
 class UserStoryAttribute(CustomAttribute):
     """
     UserStoryAttribute model
     """
-    endpoint = 'userstory-custom-attributes'
+
+    endpoint = "userstory-custom-attributes"
 
 
 class UserStoryAttributes(CustomAttributes):
     """
     UserStoryAttributes factory
     """
+
     instance = UserStoryAttribute
 
 
+class EpicAttribute(CustomAttribute):
+    """
+    EpicAttribute model
+    """
+
+    endpoint = "epic-custom-attributes"
+
+
+class EpicAttributes(CustomAttributes):
+    """
+    EpicAttributes factory
+    """
+
+    instance = EpicAttribute
+
+
 class Severity(InstanceResource):
     """
     Severity model
 
     :param requester: :class:`Requester` instance
-    :param name: name of the :class:`Severity`
-    :param order: order of the :class:`Severity`
+    :param name: name of :class:`Severity`
+    :param order: order of :class:`Severity`
     :param project: :class:`Project` id
     """
-    endpoint = 'severities'
 
-    allowed_params = ['name', 'color', 'order', 'project']
+    endpoint = "severities"
+
+    allowed_params = ["name", "color", "order", "project"]
 
 
 class Severities(ListResource):
     """
     Severities factory
     """
+
     instance = Severity
 
     def create(self, project, name, **attrs):
         """
         Create a new :class:`Severity`
 
         :param project: :class:`Project` id
-        :param name: name of the :class:`Severity`
+        :param name: name of :class:`Severity`
         :param attrs: optional attributes for :class:`Role`
         """
-        attrs.update({'project': project, 'name': name})
+        attrs.update({"project": project, "name": name})
         return self._new_resource(payload=attrs)
 
 
 class Role(InstanceResource):
     """
     Role model
 
     :param requester: :class:`Requester` instance
-    :param name: name of the :class:`Role`
-    :param slug: slug of the :class:`Role`
-    :param order: order of the :class:`Role`
+    :param name: name of :class:`Role`
+    :param slug: slug of :class:`Role`
+    :param order: order of :class:`Role`
     :param computable: choose if :class:`Role` is computable or not
 
     """
-    endpoint = 'roles'
 
-    allowed_params = ['name', 'slug', 'order', 'computable']
+    endpoint = "roles"
+
+    allowed_params = ["name", "slug", "order", "computable"]
 
 
 class Roles(ListResource):
     """
     Roles factory
     """
+
     instance = Role
 
     def create(self, project, name, **attrs):
         """
         Create a new :class:`Role`
 
         :param project: :class:`Project` id
-        :param name: name of the :class:`Role`
+        :param name: name of :class:`Role`
         :param attrs: optional attributes for :class:`Role`
         """
-        attrs.update({'project': project, 'name': name})
+        attrs.update({"project": project, "name": name})
         return self._new_resource(payload=attrs)
 
 
 class Project(InstanceResource):
     """Taiga project model
 
     :param requester: :class:`Requester` instance
     :param name: name of the project
-    :param description: description of the project
+    :param description: description of the project (not available in the :py:meth:`Projects.list` response)
     :param creation_template: base template for the project
     :param is_backlog_activated: name of the project
     :param is_issues_activated: name of the project
     :param is_kanban_activated: name of the project
     :param is_wiki_activated: determines if the project is private or not
     :param is_private: determines if the project is private or not
     :param videoconferences: appear-in or talky
     :param videoconferences_salt: for videoconference chat url generation
     :param total_milestones: missing
     :param total_story_points: missing
 
     """
 
-    endpoint = 'projects'
+    endpoint = "projects"
 
     allowed_params = [
-        'name', 'description', 'creation_template',
-        'is_backlog_activated', 'is_issues_activated',
-        'is_kanban_activated', 'is_private', 'is_wiki_activated',
-        'videoconferences', 'videoconferences_salt', 'total_milestones',
-        'total_story_points'
+        "name",
+        "description",
+        "creation_template",
+        "is_backlog_activated",
+        "is_issues_activated",
+        "is_kanban_activated",
+        "is_private",
+        "is_wiki_activated",
+        "videoconferences",
+        "videoconferences_salt",
+        "total_milestones",
+        "total_story_points",
     ]
 
     parser = {
-        'members': Users,
-        'priorities': Priorities,
-        'issue_statuses': IssueStatuses,
-        'issue_types': IssueTypes,
-        'task_statuses': TaskStatuses,
-        'severities': Severities,
-        'roles': Roles,
-        'points': Points,
-        'us_statuses': UserStoryStatuses,
-        'milestones': Milestones
+        "members": Users,
+        "priorities": Priorities,
+        "issue_statuses": IssueStatuses,
+        "issue_types": IssueTypes,
+        "task_statuses": TaskStatuses,
+        "severities": Severities,
+        "roles": Roles,
+        "points": Points,
+        "us_statuses": UserStoryStatuses,
+        "milestones": Milestones,
     }
 
     def get_item_by_ref(self, ref):
         response = self.requester.get(
-            '/resolver?project={project_id}&ref={task_ref}',
-            task_ref=ref,
-            project_id=self.slug
+            "/resolver?project={project_id}&ref={task_ref}", task_ref=ref, project_id=self.slug
         )
         response_json = response.json()
 
-        if response_json and 'task' in response_json:
+        if response_json and "task" in response_json:
             return self.get_task_by_ref(ref)
-        elif response_json and 'us' in response_json:
+        elif response_json and "us" in response_json:
             return self.get_userstory_by_ref(ref)
-        elif response_json and 'issue' in response_json:
+        elif response_json and "issue" in response_json:
             return self.get_issue_by_ref(ref)
         else:
             return None
 
     def get_task_by_ref(self, ref):
         """
         Get a :class:`Task` by ref.
 
         :param ref: :class:`Task` reference
         """
         response = self.requester.get(
-            '/{endpoint}/by_ref?ref={task_ref}&project={project_id}',
+            "/{endpoint}/by_ref?ref={task_ref}&project={project_id}",
             endpoint=Task.endpoint,
             task_ref=ref,
-            project_id=self.id
+            project_id=self.id,
         )
         return Task.parse(self.requester, response.json())
 
     def get_epic_by_ref(self, ref):
         """
         Get a :class:`Epic` by ref.
 
         :param ref: :class:`Epic` reference
         """
         response = self.requester.get(
-            '/{endpoint}/by_ref?ref={ep_ref}&project={project_id}',
+            "/{endpoint}/by_ref?ref={ep_ref}&project={project_id}",
             endpoint=Epic.endpoint,
             ep_ref=ref,
-            project_id=self.id
+            project_id=self.id,
         )
         return Epic.parse(self.requester, response.json())
 
     def get_userstory_by_ref(self, ref):
         """
         Get a :class:`UserStory` by ref.
 
         :param ref: :class:`UserStory` reference
         """
         response = self.requester.get(
-            '/{endpoint}/by_ref?ref={us_ref}&project={project_id}',
+            "/{endpoint}/by_ref?ref={us_ref}&project={project_id}",
             endpoint=UserStory.endpoint,
             us_ref=ref,
-            project_id=self.id
+            project_id=self.id,
         )
         return UserStory.parse(self.requester, response.json())
 
     def get_issue_by_ref(self, ref):
         """
         Get a :class:`Issue` by ref.
 
         :param ref: :class:`Issue` reference
         """
         response = self.requester.get(
-            '/{endpoint}/by_ref?ref={us_ref}&project={project_id}',
+            "/{endpoint}/by_ref?ref={us_ref}&project={project_id}",
             endpoint=Issue.endpoint,
             us_ref=ref,
-            project_id=self.id
+            project_id=self.id,
         )
         return Issue.parse(self.requester, response.json())
 
     def stats(self):
         """
         Get the stats of the project
         """
-        response = self.requester.get(
-            '/{endpoint}/{id}/stats',
-            endpoint=self.endpoint, id=self.id
-        )
+        response = self.requester.get("/{endpoint}/{id}/stats", endpoint=self.endpoint, id=self.id)
         return response.json()
 
     def issues_stats(self):
         """
         Get stats for issues of the project
         """
-        response = self.requester.get(
-            '/{endpoint}/{id}/issues_stats',
-            endpoint=self.endpoint, id=self.id
-        )
+        response = self.requester.get("/{endpoint}/{id}/issues_stats", endpoint=self.endpoint, id=self.id)
         return response.json()
 
     def like(self):
         """
         Like the project
         """
-        self.requester.post(
-            '/{endpoint}/{id}/like',
-            endpoint=self.endpoint, id=self.id
-        )
+        self.requester.post("/{endpoint}/{id}/like", endpoint=self.endpoint, id=self.id)
         return self
 
     def unlike(self):
         """
         Unlike the project
         """
-        self.requester.post(
-            '/{endpoint}/{id}/unlike',
-            endpoint=self.endpoint, id=self.id
-        )
+        self.requester.post("/{endpoint}/{id}/unlike", endpoint=self.endpoint, id=self.id)
         return self
 
     def star(self):
         """
         Stars the project
 
         .. deprecated:: 0.8.5
 
             Update Taiga and use like instead
         """
-        warnings.warn(
-            "Deprecated! Update Taiga and use .like() instead",
-            DeprecationWarning
-        )
-        self.requester.post(
-            '/{endpoint}/{id}/star',
-            endpoint=self.endpoint, id=self.id
-        )
+        warnings.warn("Deprecated! Update Taiga and use .like() instead", DeprecationWarning)
+        self.requester.post("/{endpoint}/{id}/star", endpoint=self.endpoint, id=self.id)
         return self
 
     def unstar(self):
         """
         Unstars the project
 
         .. deprecated:: 0.8.5
 
             Update Taiga and use unlike instead
         """
-        warnings.warn(
-            "Deprecated! Update Taiga and use .unlike() instead",
-            DeprecationWarning
-        )
-        self.requester.post(
-            '/{endpoint}/{id}/unstar',
-            endpoint=self.endpoint, id=self.id
-        )
+        warnings.warn("Deprecated! Update Taiga and use .unlike() instead", DeprecationWarning)
+        self.requester.post("/{endpoint}/{id}/unstar", endpoint=self.endpoint, id=self.id)
         return self
 
     def add_membership(self, email, role, **attrs):
         """
         Add a Membership to the project and returns a
         :class:`Membership` resource.
 
         :param email: email for :class:`Membership`
         :param role: role for :class:`Membership`
         :param attrs: role for :class:`Membership`
         :param attrs: optional :class:`Membership` attributes
         """
-        return Memberships(self.requester).create(
-            self.id, email, role, **attrs
-        )
+        return Memberships(self.requester).create(self.id, email, role, **attrs)
 
     def list_memberships(self):
         """
         Get the list of :class:`Membership` resources for the project.
         """
         return Memberships(self.requester).list(project=self.id)
 
     def add_user_story(self, subject, **attrs):
         """
         Adds a :class:`UserStory` and returns a :class:`UserStory` resource.
 
-        :param subject: subject of the :class:`UserStory`
+        :param subject: subject of :class:`UserStory`
         :param attrs: other :class:`UserStory` attributes
         """
-        return UserStories(self.requester).create(
-            self.id, subject, **attrs
-        )
+        return UserStories(self.requester).create(self.id, subject, **attrs)
 
     def import_user_story(self, subject, status, **attrs):
         """
         Import an user story and returns a :class:`UserStory` resource.
 
-        :param subject: subject of the :class:`UserStory`
-        :param status: status of the :class:`UserStory`
+        :param subject: subject of :class:`UserStory`
+        :param status: status of :class:`UserStory`
         :param attrs: optional :class:`UserStory` attributes
         """
-        return UserStories(self.requester).import_(
-            self.id, subject, status, **attrs
-        )
+        return UserStories(self.requester).import_(self.id, subject, status, **attrs)
 
-    def list_user_stories(self):
+    def list_user_stories(self, **queryparams):
         """
         Returns the :class:`UserStory` list of the project.
         """
-        return UserStories(self.requester).list(project=self.id)
+        return UserStories(self.requester).list(project=self.id, **queryparams)
 
-    def add_issue(self, subject, priority, status,
-                  issue_type, severity, **attrs):
+    def add_issue(self, subject, priority, status, issue_type, severity, **attrs):
         """
         Adds a Issue and returns a :class:`Issue` resource.
 
-        :param subject: subject of the :class:`Issue`
-        :param priority: priority of the :class:`Issue`
-        :param priority: status of the :class:`Issue`
-        :param issue_type: type of the :class:`Issue`
-        :param severity: severity of the :class:`Issue`
+        :param subject: subject of :class:`Issue`
+        :param priority: priority of :class:`Issue`
+        :param priority: status of :class:`Issue`
+        :param issue_type: type of :class:`Issue`
+        :param severity: severity of :class:`Issue`
         :param attrs: other :class:`Issue` attributes
         """
-        return Issues(self.requester).create(
-            self.id, subject, priority, status,
-            issue_type, severity, **attrs
-        )
+        return Issues(self.requester).create(self.id, subject, priority, status, issue_type, severity, **attrs)
 
-    def import_issue(self, subject, priority, status,
-                     issue_type, severity, **attrs):
+    def import_issue(self, subject, priority, status, issue_type, severity, **attrs):
         """
         Import and issue and returns a :class:`Issue` resource.
 
         :param subject: subject of :class:`Issue`
         :param priority: priority of :class:`Issue`
         :param status: status of :class:`Issue`
         :param issue_type: issue type of :class:`Issue`
         :param severity: severity of :class:`Issue`
         :param attrs: optional :class:`Issue` attributes
         """
-        return Issues(self.requester).import_(
-            self.id, subject, priority, status,
-            issue_type, severity, **attrs
-        )
+        return Issues(self.requester).import_(self.id, subject, priority, status, issue_type, severity, **attrs)
 
     def list_issues(self):
         """
         Returns the :class:`Issue` list of the project.
         """
         return Issues(self.requester).list(project=self.id)
 
     def add_milestone(self, name, estimated_start, estimated_finish, **attrs):
         """
         Add a Milestone to the project and returns a :class:`Milestone` object.
 
-        :param name: name of the :class:`Milestone`
+        :param name: name of :class:`Milestone`
         :param estimated_start: estimated start time of the
                                 :class:`Milestone`
         :param estimated_finish: estimated finish time of the
                                  :class:`Milestone`
         :param attrs: optional attributes for :class:`Milestone`
         """
-        return Milestones(self.requester).create(
-            self.id, name, estimated_start,
-            estimated_finish, **attrs
-        )
+        return Milestones(self.requester).create(self.id, name, estimated_start, estimated_finish, **attrs)
 
-    def import_milestone(self, name, estimated_start, estimated_finish,
-                         **attrs):
+    def import_milestone(self, name, estimated_start, estimated_finish, **attrs):
         """
         Import a Milestone and returns a :class:`Milestone` object.
 
-        :param name: name of the :class:`Milestone`
+        :param name: name of :class:`Milestone`
         :param estimated_start: estimated start time of the
                                 :class:`Milestone`
         :param estimated_finish: estimated finish time of the
                                  :class:`Milestone`
         :param attrs: optional attributes for :class:`Milestone`
         """
-        return Milestones(self.requester).import_(
-            self.id, name, estimated_start,
-            estimated_finish, **attrs
-        )
+        return Milestones(self.requester).import_(self.id, name, estimated_start, estimated_finish, **attrs)
 
     def list_milestones(self, **queryparams):
         """
         Get the list of :class:`Milestone` resources for the project.
         """
         return Milestones(self.requester).list(project=self.id, **queryparams)
 
     def add_point(self, name, value, **attrs):
         """
         Add a Point to the project and returns a :class:`Point` object.
 
-        :param name: name of the :class:`Point`
-        :param value: value of the :class:`Point`
+        :param name: name of :class:`Point`
+        :param value: value of :class:`Point`
         :param attrs: optional attributes for :class:`Point`
         """
         return Points(self.requester).create(self.id, name, value, **attrs)
 
     def list_points(self):
         """
         Get the list of :class:`Point` resources for the project.
         """
         return Points(self.requester).list(project=self.id)
 
     def add_epic(self, subject, **attrs):
         """
         Adds a :class:`UserStory` and returns a :class:`UserStory` resource.
 
-        :param subject: subject of the :class:`UserStory`
+        :param subject: subject of :class:`UserStory`
         :param attrs: other :class:`UserStory` attributes
         """
-        return Epics(self.requester).create(
-            self.id, subject, **attrs
-        )
+        return Epics(self.requester).create(self.id, subject, **attrs)
 
     def list_epics(self):
         """
         Get the list of :class:`Epic` resources for the project.
         """
         return Epics(self.requester).list(project=self.id)
 
     def add_task_status(self, name, **attrs):
         """
         Add a Task status to the project and returns a
         :class:`TaskStatus` object.
 
-        :param name: name of the :class:`TaskStatus`
+        :param name: name of :class:`TaskStatus`
         :param attrs: optional attributes for :class:`TaskStatus`
         """
         return TaskStatuses(self.requester).create(self.id, name, **attrs)
 
     def list_task_statuses(self):
         """
         Get the list of :class:`Task` resources for the project.
         """
         return TaskStatuses(self.requester).list(project=self.id)
 
     def import_task(self, subject, status, **attrs):
         """
         Import a Task and return a :class:`Task` object.
 
-        :param subject: subject of the :class:`Task`
-        :param status: status of the :class:`Task`
+        :param subject: subject of :class:`Task`
+        :param status: status of :class:`Task`
         :param attrs: optional attributes for :class:`Task`
         """
-        return Tasks(self.requester).import_(
-            self.id, subject, status, **attrs
-        )
+        return Tasks(self.requester).import_(self.id, subject, status, **attrs)
 
     def add_user_story_status(self, name, **attrs):
         """
         Add a UserStory status to the project and returns a
         :class:`UserStoryStatus` object.
 
-        :param name: name of the :class:`UserStoryStatus`
+        :param name: name of :class:`UserStoryStatus`
         :param attrs: optional attributes for :class:`UserStoryStatus`
         """
         return UserStoryStatuses(self.requester).create(self.id, name, **attrs)
 
     def list_user_story_statuses(self):
         """
         Get the list of :class:`UserStoryStatus` resources for the project.
@@ -1467,60 +1467,60 @@
         return UserStoryStatuses(self.requester).list(project=self.id)
 
     def add_issue_type(self, name, **attrs):
         """
         Add a Issue type to the project and returns a
         :class:`IssueType` object.
 
-        :param name: name of the :class:`IssueType`
+        :param name: name of :class:`IssueType`
         :param attrs: optional attributes for :class:`IssueType`
         """
         return IssueTypes(self.requester).create(self.id, name, **attrs)
 
     def list_issue_types(self):
         """
         Get the list of :class:`IssueType` resources for the project.
         """
         return IssueTypes(self.requester).list(project=self.id)
 
     def add_severity(self, name, **attrs):
         """
         Add a Severity to the project and returns a :class:`Severity` object.
 
-        :param name: name of the :class:`Severity`
+        :param name: name of :class:`Severity`
         :param attrs: optional attributes for :class:`Severity`
         """
         return Severities(self.requester).create(self.id, name, **attrs)
 
     def list_severities(self):
         """
         Get the list of :class:`Severity` resources for the project.
         """
         return Severities(self.requester).list(project=self.id)
 
     def add_role(self, name, **attrs):
         """
         Add a Role to the project and returns a :class:`Role` object.
 
-        :param name: name of the :class:`Role`
+        :param name: name of :class:`Role`
         :param attrs: optional attributes for :class:`Role`
         """
         return Roles(self.requester).create(self.id, name, **attrs)
 
     def list_roles(self):
         """
         Get the list of :class:`Role` resources for the project.
         """
         return Roles(self.requester).list(project=self.id)
 
     def add_priority(self, name, **attrs):
         """
         Add a Priority to the project and returns a :class:`Priority` object.
 
-        :param name: name of the :class:`Priority`
+        :param name: name of :class:`Priority`
         :param attrs: optional attributes for :class:`Priority`
         """
         return Priorities(self.requester).create(self.id, name, **attrs)
 
     def list_priorities(self):
         """
         Get the list of :class:`Priority` resources for the project.
@@ -1528,470 +1528,456 @@
         return Priorities(self.requester).list(project=self.id)
 
     def add_issue_status(self, name, **attrs):
         """
         Add a Issue status to the project and returns a
         :class:`IssueStatus` object.
 
-        :param name: name of the :class:`IssueStatus`
+        :param name: name of :class:`IssueStatus`
         :param attrs: optional attributes for :class:`IssueStatus`
         """
         return IssueStatuses(self.requester).create(self.id, name, **attrs)
 
     def list_issue_statuses(self):
         """
         Get the list of :class:`IssueStatus` resources for the project.
         """
         return IssueStatuses(self.requester).list(project=self.id)
 
     def add_wikipage(self, slug, content, **attrs):
         """
         Add a Wiki page to the project and returns a :class:`WikiPage` object.
 
-        :param name: name of the :class:`WikiPage`
+        :param name: name of :class:`WikiPage`
         :param attrs: optional attributes for :class:`WikiPage`
         """
-        return WikiPages(self.requester).create(
-            self.id, slug, content, **attrs
-        )
+        return WikiPages(self.requester).create(self.id, slug, content, **attrs)
 
     def import_wikipage(self, slug, content, **attrs):
         """
         Import a Wiki page and return a :class:`WikiPage` object.
 
-        :param slug: slug of the :class:`WikiPage`
-        :param content: content of the :class:`WikiPage`
+        :param slug: slug of :class:`WikiPage`
+        :param content: content of :class:`WikiPage`
         :param attrs: optional attributes for :class:`Task`
         """
-        return WikiPages(self.requester).import_(
-            self.id, slug, content, **attrs
-        )
+        return WikiPages(self.requester).import_(self.id, slug, content, **attrs)
 
     def list_wikipages(self):
         """
         Get the list of :class:`WikiPage` resources for the project.
         """
         return WikiPages(self.requester).list(project=self.id)
 
     def add_wikilink(self, title, href, **attrs):
         """
         Add a Wiki link to the project and returns a :class:`WikiLink` object.
 
-        :param title: title of the :class:`WikiLink`
-        :param href: href of the :class:`WikiLink`
+        :param title: title of :class:`WikiLink`
+        :param href: href of :class:`WikiLink`
         :param attrs: optional attributes for :class:`WikiLink`
         """
         return WikiLinks(self.requester).create(self.id, title, href, **attrs)
 
     def import_wikilink(self, title, href, **attrs):
         """
         Import a Wiki link and return a :class:`WikiLink` object.
 
-        :param title: title of the :class:`WikiLink`
-        :param href: href of the :class:`WikiLink`
+        :param title: title of :class:`WikiLink`
+        :param href: href of :class:`WikiLink`
         :param attrs: optional attributes for :class:`WikiLink`
         """
         return WikiLinks(self.requester).import_(self.id, title, href, **attrs)
 
     def list_wikilinks(self):
         """
         Get the list of :class:`WikiLink` resources for the project.
         """
         return WikiLinks(self.requester).list(project=self.id)
 
     def add_issue_attribute(self, name, **attrs):
         """
         Add a new Issue attribute and return a :class:`IssueAttribute` object.
 
-        :param name: name of the :class:`IssueAttribute`
+        :param name: name of :class:`IssueAttribute`
         :param attrs: optional attributes for :class:`IssueAttribute`
         """
-        return IssueAttributes(self.requester).create(
-            self.id, name, **attrs
-        )
+        return IssueAttributes(self.requester).create(self.id, name, **attrs)
 
     def list_issue_attributes(self):
         """
         Get the list of :class:`IssueAttribute` resources for the project.
         """
         return IssueAttributes(self.requester).list(project=self.id)
 
     def add_task_attribute(self, name, **attrs):
         """
         Add a new Task attribute and return a :class:`TaskAttribute` object.
 
-        :param name: name of the :class:`TaskAttribute`
+        :param name: name of :class:`TaskAttribute`
         :param attrs: optional attributes for :class:`TaskAttribute`
         """
-        return TaskAttributes(self.requester).create(
-            self.id, name, **attrs
-        )
+        return TaskAttributes(self.requester).create(self.id, name, **attrs)
 
     def list_task_attributes(self):
         """
         Get the list of :class:`TaskAttribute` resources for the project.
         """
         return TaskAttributes(self.requester).list(project=self.id)
 
     def add_user_story_attribute(self, name, **attrs):
         """
         Add a new User Story attribute and return a
         :class:`UserStoryAttribute` object.
 
-        :param name: name of the :class:`UserStoryAttribute`
+        :param name: name of :class:`UserStoryAttribute`
         :param attrs: optional attributes for :class:`UserStoryAttribute`
         """
-        return UserStoryAttributes(self.requester).create(
-            self.id, name, **attrs
-        )
+        return UserStoryAttributes(self.requester).create(self.id, name, **attrs)
 
     def list_user_story_attributes(self):
         """
         Get the list of :class:`UserStoryAttribute` resources for the project.
         """
         return UserStoryAttributes(self.requester).list(project=self.id)
 
+    def list_epic_attributes(self):
+        """
+        Get the list of :class:`EpicAttribute` resources for the project.
+        """
+        return EpicAttributes(self.requester).list(project=self.id)
+
     def add_webhook(self, name, url, key, **attrs):
         """
         Add a new Webhook and return a :class:`Webhook` object.
 
-        :param name: name of the :class:`Webhook`
-        :param url: payload url of the :class:`Webhook`
-        :param key: secret key of the :class:`Webhook`
+        :param name: name of :class:`Webhook`
+        :param url: payload url of :class:`Webhook`
+        :param key: secret key of :class:`Webhook`
         :param attrs: optional attributes for :class:`Webhook`
         """
-        return Webhooks(self.requester).create(
-            self.id, name, url, key, **attrs
-        )
+        return Webhooks(self.requester).create(self.id, name, url, key, **attrs)
 
     def list_webhooks(self):
         """
         Get the list of :class:`Webhook` resources for the project.
         """
         return Webhooks(self.requester).list(project=self.id)
 
     def add_tag(self, tag, color=None):
         """
         Add a new tag and return a response object.
 
         :param tag: name of the tag
         :param color: optional color of the tag
         """
-        attrs = {'tag': tag}
+        attrs = {"tag": tag}
         if color:
-            attrs['color'] = color
-        response = self.requester.post(
-            "/{}/{}/create_tag".format(self.endpoint, self.id), payload=attrs
-        )
+            attrs["color"] = color
+        response = self.requester.post("/{}/{}/create_tag".format(self.endpoint, self.id), payload=attrs)
         return response
 
     def list_tags(self):
         """
         Get the list of tags for the project.
         """
-        response = self.requester.get(
-            "/{}/{}/tags_colors".format(self.endpoint, self.id)
-        )
+        response = self.requester.get("/{}/{}/tags_colors".format(self.endpoint, self.id))
         return response.json()
 
 
 class Projects(ListResource):
     """
     Projects factory
     """
 
     instance = Project
 
     def create(self, name, description, **attrs):
         """
         Create a new :class:`Project`
 
-        :param name: name of the :class:`Project`
-        :param description: description of the :class:`Project`
+        :param name: name of :class:`Project`
+        :param description: description of :class:`Project`
         :param attrs: optional attributes for :class:`Project`
         """
-        attrs.update({'name': name, 'description': description})
+        attrs.update({"name": name, "description": description})
         return self._new_resource(payload=attrs)
 
     def import_(self, name, description, roles, **attrs):
-        attrs.update(
-            {
-                'name': name,
-                'description': description,
-                'roles': roles
-            }
-        )
-        response = self.requester.post('/{endpoint}', endpoint="importer",
-                                       payload=attrs)
+        attrs.update({"name": name, "description": description, "roles": roles})
+        response = self.requester.post("/{endpoint}", endpoint="importer", payload=attrs)
         return self.instance.parse(self.requester, response.json())
 
     def get_by_slug(self, slug):
         """
         Get a :class:`Project` by slug
 
-        :param slug: the slug of the :class:`Project`
+        :param slug: the slug of :class:`Project`
         """
-        response = self.requester.get(
-            '/{endpoint}/by_slug?slug={slug}',
-            endpoint=self.instance.endpoint,
-            slug=slug
-        )
+        response = self.requester.get("/{endpoint}/by_slug?slug={slug}", endpoint=self.instance.endpoint, slug=slug)
         return self.instance.parse(self.requester, response.json())
 
 
 class WikiAttachment(Attachment):
     """
     WikiAttachment model
     """
-    endpoint = 'wiki/attachments'
+
+    endpoint = "wiki/attachments"
 
 
 class WikiAttachments(Attachments):
     """
     WikiAttachments factory
     """
+
     instance = WikiAttachment
 
 
 class WikiPage(InstanceResource):
     """
     WikiPage model
 
     :param project: :class:`Project` id
     :param slug: slug of the wiki page
     :param content: content of the wiki page
     :param watchers: list of watchers id
     """
-    endpoint = 'wiki'
 
-    repr_attribute = 'slug'
+    endpoint = "wiki"
+
+    repr_attribute = "slug"
 
-    allowed_params = ['project', 'slug', 'content', 'watchers']
+    allowed_params = ["project", "slug", "content", "watchers"]
 
     def attach(self, attached_file, **attrs):
         """
         Attach a file to the :class:`WikiPage`
 
         :param attached_file: file path to attach
         :param attrs: optional attributes for the attached file
         """
-        return WikiAttachments(self.requester).create(
-            self.project, self.id,
-            attached_file, **attrs
-        )
+        return WikiAttachments(self.requester).create(self.project, self.id, attached_file, **attrs)
 
 
 class WikiPages(ListResource):
     """
     WikiPages factory
     """
+
     instance = WikiPage
 
     def create(self, project, slug, content, **attrs):
         """
         create a new :class:`WikiPage`
 
         :param project: :class:`Project` id
         :param slug: slug of the wiki page
         :param content: content of the wiki page
         :param attrs: optional attributes for the :class:`WikiPage`
         """
-        attrs.update({'project': project, 'slug': slug, 'content': content})
+        attrs.update({"project": project, "slug": slug, "content": content})
         return self._new_resource(payload=attrs)
 
     def import_(self, project, slug, content, **attrs):
-        attrs.update({'project': project, 'slug': slug, 'content': content})
-        response = self.requester.post('/{endpoint}/{id}/{type}',
-                                       endpoint="importer", id=project,
-                                       type="wiki_page", payload=attrs)
+        attrs.update({"project": project, "slug": slug, "content": content})
+        response = self.requester.post(
+            "/{endpoint}/{id}/{type}", endpoint="importer", id=project, type="wiki_page", payload=attrs
+        )
         return self.instance.parse(self.requester, response.json())
 
 
 class WikiLink(InstanceResource):
     """
     WikiLink model
 
     :param project: :class:`Project` id
     :param title: title of the wiki link
     :param href: href for the wiki link
     :param order: order of the wiki link
     """
-    endpoint = 'wiki-links'
 
-    repr_attribute = 'title'
+    endpoint = "wiki-links"
 
-    allowed_params = ['project', 'title', 'href', 'order']
+    repr_attribute = "title"
+
+    allowed_params = ["project", "title", "href", "order"]
 
 
 class WikiLinks(ListResource):
     """
     WikiLinks factory
     """
+
     instance = WikiLink
 
     def create(self, project, title, href, **attrs):
         """
         Create a new :class:`WikiLink`
 
         :param project: :class:`Project` id
         :param title: title of the wiki link
         :param href: href for the wiki link
         :param attrs: optional attributes for the :class:`WikiLink`
         """
-        attrs.update({'project': project, 'title': title, 'href': href})
+        attrs.update({"project": project, "title": title, "href": href})
         return self._new_resource(payload=attrs)
 
     def import_(self, project, title, href, **attrs):
-        attrs.update({'project': project, 'title': title, 'href': href})
-        response = self.requester.post('/{endpoint}/{id}/{type}',
-                                       endpoint="importer", id=project,
-                                       type="wiki_link", payload=attrs)
+        attrs.update({"project": project, "title": title, "href": href})
+        response = self.requester.post(
+            "/{endpoint}/{id}/{type}", endpoint="importer", id=project, type="wiki_link", payload=attrs
+        )
         return self.instance.parse(self.requester, response.json())
 
 
 class History(InstanceResource):
     """
     History model
     """
+
     def __init__(self, *args, **kwargs):
-        super(History, self).__init__(*args, **kwargs)
+        super().__init__(*args, **kwargs)
         self.issue = HistoryIssue(self.requester)
         self.task = HistoryTask(self.requester)
         self.user_story = HistoryUserStory(self.requester)
         self.wiki = HistoryWiki(self.requester)
         self.epic = HistoryEpic(self.requester)
 
 
-class HistoryEntity(object):
+class HistoryEntity:
     """
     HistoryEntity model
     """
-    endpoint = 'history'
+
+    endpoint = "history"
 
     def __init__(self, requester):
         self.requester = requester
 
     def get(self, resource_id):
         """
         Get a history element
 
-        :param resource_id: ...
+        :param resource_id: id of the resource object (resource type is defined by the HistoryEntity subclass used)
         """
         response = self.requester.get(
-            '/{endpoint}/{entity}/{id}',
-            endpoint=self.endpoint, entity=self.entity, id=resource_id,
-            paginate=False
+            "/{endpoint}/{entity}/{id}", endpoint=self.endpoint, entity=self.entity, id=resource_id, paginate=False
         )
         return response.json()
 
-    def delete_comment(self, resource_id, ent_id):
+    def delete_comment(self, resource_id, comment_id):
         """
         Delete a comment
 
-        :param resource_id: ...
-        :param ent_id: ...
+        :param resource_id: id of the resource object (resource type is defined by the HistoryEntity subclass used)
+        :param comment_id: id of the comment to delete
         """
         self.requester.post(
-            '/{endpoint}/{entity}/{id}/delete_comment?id={ent_id}',
-            endpoint=self.endpoint, entity=self.entity,
-            id=resource_id, ent_id=ent_id
+            "/{endpoint}/{entity}/{id}/delete_comment?id={comment_id}",
+            endpoint=self.endpoint,
+            entity=self.entity,
+            id=resource_id,
+            comment_id=comment_id,
         )
 
-    def undelete_comment(self, resource_id, ent_id):
+    def undelete_comment(self, resource_id, comment_id):
         """
         Undelete a comment
 
-        :param resource_id: ...
-        :param ent_id: ...
+        :param resource_id: id of the resource object (resource type is defined by the HistoryEntity subclass used)
+        :param comment_id: id of the comment to undelete
         """
         self.requester.post(
-            '/{endpoint}/{entity}/{id}/undelete_comment?id={ent_id}',
-            endpoint=self.endpoint, entity=self.entity,
-            id=resource_id, ent_id=ent_id
+            "/{endpoint}/{entity}/{id}/undelete_comment?id={comment_id}",
+            endpoint=self.endpoint,
+            entity=self.entity,
+            id=resource_id,
+            comment_id=comment_id,
         )
 
 
 class HistoryIssue(HistoryEntity):
     """
     HistoryIssue model
     """
+
     def __init__(self, *args, **kwargs):
         super(type(self), self).__init__(*args, **kwargs)
-        self.entity = 'issue'
+        self.entity = "issue"
 
 
 class HistoryEpic(HistoryEntity):
     """
     HistoryEpic model
     """
+
     def __init__(self, *args, **kwargs):
         super(type(self), self).__init__(*args, **kwargs)
-        self.entity = 'epic'
+        self.entity = "epic"
 
 
 class HistoryTask(HistoryEntity):
     """
     HistoryTask model
     """
+
     def __init__(self, *args, **kwargs):
         super(type(self), self).__init__(*args, **kwargs)
-        self.entity = 'task'
+        self.entity = "task"
 
 
 class HistoryUserStory(HistoryEntity):
     """
     HistoryUserStory model
     """
+
     def __init__(self, *args, **kwargs):
         super(type(self), self).__init__(*args, **kwargs)
-        self.entity = 'userstory'
+        self.entity = "userstory"
 
 
 class HistoryWiki(HistoryEntity):
     """
     HistoryWiki model
     """
+
     def __init__(self, *args, **kwargs):
         super(type(self), self).__init__(*args, **kwargs)
-        self.entity = 'wiki'
+        self.entity = "wiki"
 
 
 class Webhook(InstanceResource):
     """
     Webhook model
 
     :param requester: :class:`Requester` instance
-    :param name: name of the :class:`Webhook`
-    :param url: payload url of the :class:`Webhook`
-    :param key: secret key of the :class:`Webhook`
+    :param name: name of :class:`Webhook`
+    :param url: payload url of :class:`Webhook`
+    :param key: secret key of :class:`Webhook`
 
     """
-    endpoint = 'webhooks'
 
-    allowed_params = ['name', 'url', 'key']
+    endpoint = "webhooks"
+
+    allowed_params = ["name", "url", "key"]
 
 
 class Webhooks(ListResource):
     """
     Webhooks factory
     """
+
     instance = Webhook
 
     def create(self, project, name, url, key, **attrs):
         """
         Create a new :class:`Webhook`
 
         :param project: :class:`Project` id
-        :param name: name of the :class:`Webhook`
-        :param url: payload url of the :class:`Webhook`
-        :param key: secret key of the :class:`Webhook`
+        :param name: name of :class:`Webhook`
+        :param url: payload url of :class:`Webhook`
+        :param key: secret key of :class:`Webhook`
         :param attrs: optional attributes for :class:`Webhook`
         """
-        attrs.update(
-            {
-                'project': project,
-                'name': name,
-                'url': url,
-                'key': key
-            }
-        )
+        attrs.update({"project": project, "name": name, "url": url, "key": key})
         return self._new_resource(payload=attrs)
```

### Comparing `python-taiga-1.0.0b1/taiga/client.py` & `python-taiga-1.1.0/taiga/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,48 @@
 import json
 
-import requests
-from requests.exceptions import RequestException
-from requests.packages.urllib3.exceptions import InsecureRequestWarning
+try:
+    import requests
+    from requests.exceptions import RequestException
+    from requests.packages.urllib3.exceptions import InsecureRequestWarning
+except ImportError:  # pragma: no cover
+    pass
 
 from . import exceptions, utils
 from .models import (
-    Epics, History, IssueAttachments, IssueAttributes, Issues, IssueStatuses, IssueTypes, Milestones, Points,
-    Priorities, Projects, Roles, Severities, TaskAttachments, TaskAttributes, Tasks, TaskStatuses, Users, UserStories,
-    UserStoryAttachments, UserStoryAttributes, UserStoryStatuses, Webhooks, WikiLinks, WikiPages,
+    Epics,
+    History,
+    IssueAttachments,
+    IssueAttributes,
+    Issues,
+    IssueStatuses,
+    IssueTypes,
+    Milestones,
+    Points,
+    Priorities,
+    Projects,
+    Roles,
+    Severities,
+    TaskAttachments,
+    TaskAttributes,
+    Tasks,
+    TaskStatuses,
+    Users,
+    UserStories,
+    UserStoryAttachments,
+    UserStoryAttributes,
+    UserStoryStatuses,
+    Webhooks,
+    WikiLinks,
+    WikiPages,
 )
 from .requestmaker import RequestMaker
 
 
-class SearchResult(object):
-
+class SearchResult:
     count = 0
     tasks = []
     issues = []
     user_stories = []
     wiki_pages = []
 
 
@@ -28,26 +52,27 @@
 
     :param host: the host of your Taiga.io instance
     :param token: the token you may provide
     :param token_type: the token type
     :param tls_verify: verify server certificate
     :param auth_type: authentication type identifier
     """
-    def __init__(self, host='https://api.taiga.io', token=None,
-                 token_type='Bearer', tls_verify=True, auth_type='normal'):
+
+    def __init__(
+        self, host="https://api.taiga.io", token=None, token_type="Bearer", tls_verify=True, auth_type="normal"
+    ):
         self.host = host
         self.token = token
         self.token_type = token_type
         self.tls_verify = tls_verify
         self.auth_type = auth_type
         if not self.tls_verify:
             requests.packages.urllib3.disable_warnings(InsecureRequestWarning)
         if token:
-            self.raw_request = RequestMaker('/api/v1', self.host, self.token,
-                                            self.token_type, self.tls_verify)
+            self.raw_request = RequestMaker("/api/v1", self.host, self.token, self.token_type, self.tls_verify)
             self._init_resources()
 
     def _init_resources(self):
         self.projects = Projects(self.raw_request)
         self.user_stories = UserStories(self.raw_request)
         self.user_story_attachments = UserStoryAttachments(self.raw_request)
         self.users = Users(self.raw_request)
@@ -73,140 +98,87 @@
         self.webhooks = Webhooks(self.raw_request)
         self.epics = Epics(self.raw_request)
 
     def me(self):
         """
         Get a :class:`taiga.models.models.User` representing me
         """
-        return self.users.get('me')
+        return self.users.get("me")
 
-    def search(self, project, text=''):
+    def search(self, project, text=""):
         """
         Search in your Taiga.io instance
 
         :param project: the project id
         :param text: the query of your search
         """
-        result = self.raw_request.get(
-            'search', query={'project': project, 'text': text}
-        )
+        result = self.raw_request.get("search", query={"project": project, "text": text})
         result = result.json()
         search_result = SearchResult()
-        search_result.tasks = self.tasks.parse_list(result['tasks'])
-        search_result.issues = self.issues.parse_list(result['issues'])
-        search_result.user_stories = self.user_stories.parse_list(
-            result['userstories']
-        )
-        search_result.wikipages = self.wikipages.parse_list(
-            result['wikipages']
-        )
-        search_result.epics = self.epics.parse_list(
-            result['epics']
-        )
+        search_result.tasks = self.tasks.parse_list(result["tasks"])
+        search_result.issues = self.issues.parse_list(result["issues"])
+        search_result.user_stories = self.user_stories.parse_list(result["userstories"])
+        search_result.wikipages = self.wikipages.parse_list(result["wikipages"])
+        search_result.epics = self.epics.parse_list(result["epics"])
         return search_result
 
     def auth(self, username, password):
         """
         Authenticate you
 
         :param username: your username
         :param password: your password
         """
-        headers = {
-            'Content-type': 'application/json'
-        }
-        payload = {
-            'type': self.auth_type,
-            'username': username,
-            'password': password
-        }
+        headers = {"Content-type": "application/json"}
+        payload = {"type": self.auth_type, "username": username, "password": password}
         try:
-            full_url = utils.urljoin(self.host, '/api/v1/auth')
-            response = requests.post(
-                full_url,
-                data=json.dumps(payload),
-                headers=headers,
-                verify=self.tls_verify
-            )
+            full_url = utils.urljoin(self.host, "/api/v1/auth")
+            response = requests.post(full_url, data=json.dumps(payload), headers=headers, verify=self.tls_verify)
         except RequestException:
-            raise exceptions.TaigaRestException(
-                full_url, 400,
-                'NETWORK ERROR', 'POST'
-            )
+            raise exceptions.TaigaRestException(full_url, 400, "NETWORK ERROR", "POST")
         if response.status_code != 200:
-            raise exceptions.TaigaRestException(
-                full_url,
-                response.status_code,
-                response.text,
-                'POST'
-            )
-        self.token = response.json()['auth_token']
-        self.raw_request = RequestMaker('/api/v1', self.host, self.token,
-                                        'Bearer', self.tls_verify)
+            raise exceptions.TaigaRestException(full_url, response.status_code, response.text, "POST")
+        self.token = response.json()["auth_token"]
+        self.token_refresh = response.json()["refresh"]
+        self.raw_request = RequestMaker("/api/v1", self.host, self.token, "Bearer", self.tls_verify)
         self._init_resources()
 
-    def auth_app(self, app_id, app_secret, auth_code, state=''):
+    def auth_app(self, app_id, app_secret, auth_code, state=""):
         """
         Authenticate an app
 
         :param app_id: the app id
         :param app_secret: the app secret
         :param auth_code: the app auth code
         """
-        headers = {
-            'Content-type': 'application/json'
-        }
-        payload = {
-            'application': app_id,
-            'auth_code': auth_code,
-            'state': state
-        }
+        headers = {"Content-type": "application/json"}
+        payload = {"application": app_id, "auth_code": auth_code, "state": state}
         try:
-            full_url = utils.urljoin(
-                self.host,
-                '/api/v1/application-tokens/validate'
-            )
-            response = requests.post(
-                full_url,
-                data=json.dumps(payload),
-                headers=headers,
-                verify=self.tls_verify
-            )
+            full_url = utils.urljoin(self.host, "/api/v1/application-tokens/validate")
+            response = requests.post(full_url, data=json.dumps(payload), headers=headers, verify=self.tls_verify)
         except RequestException:
-            raise exceptions.TaigaRestException(
-                full_url, 400,
-                'NETWORK ERROR', 'POST'
-            )
+            raise exceptions.TaigaRestException(full_url, 400, "NETWORK ERROR", "POST")
         if response.status_code != 200:
-            raise exceptions.TaigaRestException(
-                full_url,
-                response.status_code,
-                response.text,
-                'POST'
-            )
-        cyphered_token = response.json().get('cyphered_token', '')
+            raise exceptions.TaigaRestException(full_url, response.status_code, response.text, "POST")
+        cyphered_token = response.json().get("cyphered_token", "")
         if cyphered_token:
-            from jwkest.jwk import SYMKey
             from jwkest.jwe import JWE
+            from jwkest.jwk import SYMKey
 
-            sym_key = SYMKey(key=app_secret, alg='A128KW')
+            sym_key = SYMKey(key=app_secret, alg="A128KW")
             data, success = JWE().decrypt(cyphered_token, keys=[sym_key]), True
             if isinstance(data, tuple):
                 data, success = data
             try:
-                self.token = json.loads(data.decode('utf-8')).get('token', None)
+                self.token = json.loads(data.decode("utf-8")).get("token", None)
             except ValueError:  # pragma: no cover
                 self.token = None
             if not success:
                 self.token = None
         else:
             self.token = None
 
         if self.token is None:
-            raise exceptions.TaigaRestException(
-                full_url, 400,
-                'INVALID TOKEN', 'POST'
-            )
+            raise exceptions.TaigaRestException(full_url, 400, "INVALID TOKEN", "POST")
 
-        self.raw_request = RequestMaker('/api/v1', self.host, self.token,
-                                        'Application', self.tls_verify)
+        self.raw_request = RequestMaker("/api/v1", self.host, self.token, "Application", self.tls_verify)
         self._init_resources()
```

### Comparing `python-taiga-1.0.0b1/taiga/exceptions.py` & `python-taiga-1.1.0/taiga/exceptions.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 import json
 
 
-class TaigaException(Exception):
+class TaigaException(Exception):  # noqa: N818
     pass
 
 
-class TaigaRestException(TaigaException):
-
-    def __init__(self, uri, status_code, message="", method='GET'):
+class TaigaRestException(TaigaException):  # noqa: N818
+    def __init__(self, uri, status_code, message="", method="GET"):
         self.uri = uri
         self.status_code = status_code
         self.method = method
         try:
             json_message = json.loads(message)
-            if '_error_message' in json_message:
-                message = json_message['_error_message']
+            if "_error_message" in json_message:
+                message = json_message["_error_message"]
         except ValueError:
             pass
         if not message:
-            message = 'Status: {} on URI: {}'.format(status_code, uri)
-        super(TaigaRestException, self).__init__(message)
+            message = "Status: {} on URI: {}".format(status_code, uri)
+        super().__init__(message)
```

### Comparing `python-taiga-1.0.0b1/taiga/requestmaker.py` & `python-taiga-1.1.0/taiga/requestmaker.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,75 +1,59 @@
 import json
 import time
-from distutils.version import LooseVersion
 
-import requests
-from requests.exceptions import RequestException
-from requests.packages.urllib3.exceptions import InsecureRequestWarning
+try:
+    import requests
+    from requests.exceptions import RequestException
+    from requests.packages.urllib3.exceptions import InsecureRequestWarning
+except ImportError:  # pragma: no cover
+    pass
 
 from . import exceptions, utils
 
 
-def _requests_compatible_true():
-    if LooseVersion(requests.__version__) >= LooseVersion('2.11.0'):
-        return 'True'
-    else:
-        return True
-
-
-class RequestCacheException(Exception):
+class RequestCacheException(Exception):  # noqa: N818
     pass
 
 
-class RequestCacheMissingException(RequestCacheException):
+class RequestCacheMissingException(RequestCacheException):  # noqa: N818
     pass
 
 
-class RequestCacheInvalidException(RequestCacheException):
+class RequestCacheInvalidException(RequestCacheException):  # noqa: N818
     pass
 
 
-class RequestCache(object):
-
+class RequestCache:
     def __init__(self, valid_time=60):
         self._valid_time = valid_time
         self._cache = {}
 
     def put(self, key, value):
-        self._cache[key] = {
-            'time': time.time(),
-            'value': value
-        }
+        self._cache[key] = {"time": time.time(), "value": value}
 
     def remove(self, key):
         if key in self._cache:
             del self._cache[key]
 
     def get(self, key):
         if key not in self._cache:
             raise RequestCacheMissingException()
-        if time.time() > self._cache[key]['time'] + self._valid_time:
+        if time.time() > self._cache[key]["time"] + self._valid_time:
             self.remove(key)
             raise RequestCacheInvalidException()
-        return self._cache[key]['value']
+        return self._cache[key]["value"]
 
 
-class RequestMakerException(Exception):
+class RequestMakerException(Exception):  # noqa: N818
     pass
 
 
-class RequestMaker(object):
-
-    def __init__(self,
-                 api_path, host,
-                 token,
-                 token_type='Bearer',
-                 tls_verify=True,
-                 enable_pagination=True
-                 ):
+class RequestMaker:
+    def __init__(self, api_path, host, token, token_type="Bearer", tls_verify=True, enable_pagination=True):
         self.api_path = api_path
         self.host = host
         self.token = token
         self.token_type = token_type
         self.tls_verify = tls_verify
         self.enable_pagination = enable_pagination
         self._cache = RequestCache()
@@ -81,175 +65,107 @@
         return self._cache
 
     def is_bad_response(self, response):
         return 400 <= response.status_code <= 500
 
     def headers(self, paginate=True):
         headers = {
-            'Content-type': 'application/json',
-            'Authorization': '{0} {1}'.format(self.token_type, self.token),
+            "Content-type": "application/json",
+            "Authorization": "{} {}".format(self.token_type, self.token),
         }
         if self.enable_pagination and paginate:
-            headers['x-lazy-pagination'] = _requests_compatible_true()
+            headers["x-lazy-pagination"] = "True"
         else:
-            headers['x-disable-pagination'] = _requests_compatible_true()
+            headers["x-disable-pagination"] = "True"
         return headers
 
     def urljoin(self, *parts):
         return utils.urljoin(*parts)
 
-    def get_full_url(self, uri, query={}, **parameters):
-        full_url = self.urljoin(
-            self.host, self.api_path,
-            uri.format(**parameters)
-        )
+    def get_full_url(self, uri, query=None, **parameters):
+        full_url = self.urljoin(self.host, self.api_path, uri.format(**parameters))
         return full_url
 
-    def get(self, uri, query={}, cache=False, paginate=True, **parameters):
+    def get(self, uri, query=None, cache=False, paginate=True, **parameters):
         try:
-            full_url = self.urljoin(
-                self.host, self.api_path,
-                uri.format(**parameters)
-            )
+            full_url = self.urljoin(self.host, self.api_path, uri.format(**parameters))
 
             result = None
 
             if cache:
                 try:
                     result = self._cache.get(full_url)
                 except RequestCacheException:
                     pass
 
             if not result:
                 result = requests.get(
-                    full_url,
-                    headers=self.headers(paginate),
-                    params=query,
-                    verify=self.tls_verify
+                    full_url, headers=self.headers(paginate), params=query or {}, verify=self.tls_verify
                 )
             if cache:
                 self._cache.put(full_url, result)
         except RequestException:
-            raise exceptions.TaigaRestException(
-                full_url, 400,
-                'Network error!', 'GET'
-            )
+            raise exceptions.TaigaRestException(full_url, 400, "Network error!", "GET")
         if not self.is_bad_response(result):
             return result
         else:
-            raise exceptions.TaigaRestException(
-                full_url, result.status_code,
-                result.text, 'GET'
-            )
+            raise exceptions.TaigaRestException(full_url, result.status_code, result.text, "GET")
 
-    def post(self, uri, payload=None, query={}, files={}, **parameters):
+    def post(self, uri, payload=None, query=None, files=None, **parameters):
         if files:
             headers = {
-                'Authorization': '{0} {1}'.format(self.token_type, self.token),
-                'x-disable-pagination': _requests_compatible_true()
+                "Authorization": "{} {}".format(self.token_type, self.token),
+                "x-disable-pagination": "True",
             }
             data = payload
         else:
             headers = self.headers()
             data = json.dumps(payload)
+            files = {}
         try:
-            full_url = self.urljoin(
-                self.host, self.api_path,
-                uri.format(**parameters)
-            )
+            full_url = self.urljoin(self.host, self.api_path, uri.format(**parameters))
             result = requests.post(
-                full_url,
-                headers=headers,
-                data=data,
-                params=query,
-                files=files,
-                verify=self.tls_verify
+                full_url, headers=headers, data=data, params=query or {}, files=files, verify=self.tls_verify
             )
         except RequestException:
-            raise exceptions.TaigaRestException(
-                full_url, 400,
-                'Network error!', 'POST'
-            )
+            raise exceptions.TaigaRestException(full_url, 400, "Network error!", "POST")
         if not self.is_bad_response(result):
             return result
         else:
-            raise exceptions.TaigaRestException(
-                full_url, result.status_code,
-                result.text, 'POST'
-            )
+            raise exceptions.TaigaRestException(full_url, result.status_code, result.text, "POST")
 
-    def delete(self, uri, query={}, **parameters):
+    def delete(self, uri, query=None, **parameters):
         try:
-            full_url = self.urljoin(
-                self.host, self.api_path,
-                uri.format(**parameters)
-            )
-            result = requests.delete(
-                full_url,
-                headers=self.headers(),
-                params=query,
-                verify=self.tls_verify
-            )
+            full_url = self.urljoin(self.host, self.api_path, uri.format(**parameters))
+            result = requests.delete(full_url, headers=self.headers(), params=query or {}, verify=self.tls_verify)
         except RequestException:
-            raise exceptions.TaigaRestException(
-                full_url, 400,
-                'Network error!', 'DELETE'
-            )
+            raise exceptions.TaigaRestException(full_url, 400, "Network error!", "DELETE")
         if not self.is_bad_response(result):
             return result
         else:
-            raise exceptions.TaigaRestException(
-                full_url, result.status_code,
-                result.text, 'DELETE'
-            )
+            raise exceptions.TaigaRestException(full_url, result.status_code, result.text, "DELETE")
 
-    def put(self, uri, payload=None, query={}, **parameters):
+    def put(self, uri, payload=None, query=None, **parameters):
         try:
-            full_url = self.urljoin(
-                self.host, self.api_path,
-                uri.format(**parameters)
-            )
+            full_url = self.urljoin(self.host, self.api_path, uri.format(**parameters))
             result = requests.put(
-                full_url,
-                headers=self.headers(),
-                data=json.dumps(payload),
-                params=query,
-                verify=self.tls_verify
+                full_url, headers=self.headers(), data=json.dumps(payload), params=query or {}, verify=self.tls_verify
             )
         except RequestException:
-            raise exceptions.TaigaRestException(
-                full_url, 400,
-                'Network error!', 'PUT'
-            )
+            raise exceptions.TaigaRestException(full_url, 400, "Network error!", "PUT")
         if not self.is_bad_response(result):
             return result
         else:
-            raise exceptions.TaigaRestException(
-                full_url, result.status_code,
-                result.text, 'PUT'
-            )
+            raise exceptions.TaigaRestException(full_url, result.status_code, result.text, "PUT")
 
-    def patch(self, uri, payload=None, query={}, **parameters):
+    def patch(self, uri, payload=None, query=None, **parameters):
         try:
-            full_url = self.urljoin(
-                self.host, self.api_path,
-                uri.format(**parameters)
-            )
+            full_url = self.urljoin(self.host, self.api_path, uri.format(**parameters))
             result = requests.patch(
-                full_url,
-                headers=self.headers(),
-                data=json.dumps(payload),
-                params=query,
-                verify=self.tls_verify
+                full_url, headers=self.headers(), data=json.dumps(payload), params=query or {}, verify=self.tls_verify
             )
         except RequestException:
-            raise exceptions.TaigaRestException(
-                full_url, 400,
-                'Network error!', 'PATCH'
-            )
+            raise exceptions.TaigaRestException(full_url, 400, "Network error!", "PATCH")
         if not self.is_bad_response(result):
             return result
         else:
-            raise exceptions.TaigaRestException(
-                full_url, result.status_code,
-                result.text, 'PATCH'
-            )
+            raise exceptions.TaigaRestException(full_url, result.status_code, result.text, "PATCH")
```

### Comparing `python-taiga-1.0.0b1/AUTHORS` & `python-taiga-1.1.0/AUTHORS`

 * *Files identical despite different names*

### Comparing `python-taiga-1.0.0b1/LICENSE` & `python-taiga-1.1.0/LICENSE`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -14,8 +14,8 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
-THE SOFTWARE.
+THE SOFTWARE.
```

