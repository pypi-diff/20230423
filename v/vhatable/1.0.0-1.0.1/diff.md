# Comparing `tmp/vhatable-1.0.0.tar.gz` & `tmp/vhatable-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vhatable-1.0.0.tar", last modified: Thu Sep  9 16:36:46 2021, max compression
+gzip compressed data, was "vhatable-1.0.1.tar", last modified: Sun Apr 23 17:45:48 2023, max compression
```

## Comparing `vhatable-1.0.0.tar` & `vhatable-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,19 @@
-drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2021-09-09 16:36:46.498991 vhatable-1.0.0/
--rw-rw-r--   0 fred      (1000) fred      (1000)      551 2021-09-09 16:36:46.498991 vhatable-1.0.0/PKG-INFO
--rw-rw-r--   0 fred      (1000) fred      (1000)      144 2021-07-17 18:05:01.000000 vhatable-1.0.0/README.rst
--rw-rw-r--   0 fred      (1000) fred      (1000)       38 2021-09-09 16:36:46.498991 vhatable-1.0.0/setup.cfg
--rwxrwxr-x   0 fred      (1000) fred      (1000)     2549 2021-09-09 11:56:00.000000 vhatable-1.0.0/setup.py
-drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2021-09-09 16:36:46.498991 vhatable-1.0.0/vhatable/
--rw-rw-r--   0 fred      (1000) fred      (1000)      958 2021-09-09 11:27:19.000000 vhatable-1.0.0/vhatable/__init__.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     9318 2021-09-09 11:27:19.000000 vhatable-1.0.0/vhatable/cell.py
--rw-rw-r--   0 fred      (1000) fred      (1000)    22345 2021-09-09 16:33:48.000000 vhatable-1.0.0/vhatable/core.py
--rw-rw-r--   0 fred      (1000) fred      (1000)     6691 2021-09-09 16:32:21.000000 vhatable-1.0.0/vhatable/filters.py
-drwxrwxr-x   0 fred      (1000) fred      (1000)        0 2021-09-09 16:36:46.498991 vhatable-1.0.0/vhatable.egg-info/
--rw-rw-r--   0 fred      (1000) fred      (1000)      551 2021-09-09 16:36:46.000000 vhatable-1.0.0/vhatable.egg-info/PKG-INFO
--rw-rw-r--   0 fred      (1000) fred      (1000)      253 2021-09-09 16:36:46.000000 vhatable-1.0.0/vhatable.egg-info/SOURCES.txt
--rw-rw-r--   0 fred      (1000) fred      (1000)        1 2021-09-09 16:36:46.000000 vhatable-1.0.0/vhatable.egg-info/dependency_links.txt
--rw-rw-r--   0 fred      (1000) fred      (1000)       42 2021-09-09 16:36:46.000000 vhatable-1.0.0/vhatable.egg-info/requires.txt
--rw-rw-r--   0 fred      (1000) fred      (1000)        9 2021-09-09 16:36:46.000000 vhatable-1.0.0/vhatable.egg-info/top_level.txt
+drwxr-xr-x   0 fred      (1000) fred      (1000)        0 2023-04-23 17:45:48.022043 vhatable-1.0.1/
+-rw-r--r--   0 fred      (1000) fred      (1000)    35138 2022-01-30 18:20:55.000000 vhatable-1.0.1/LICENSE.txt
+-rw-r--r--   0 fred      (1000) fred      (1000)      609 2023-04-23 17:45:48.018710 vhatable-1.0.1/PKG-INFO
+-rw-r--r--   0 fred      (1000) fred      (1000)      336 2022-01-30 18:20:55.000000 vhatable-1.0.1/README.rst
+-rw-r--r--   0 fred      (1000) fred      (1000)       38 2023-04-23 17:45:48.022043 vhatable-1.0.1/setup.cfg
+-rwxr-xr-x   0 fred      (1000) fred      (1000)     2840 2022-01-15 02:09:48.000000 vhatable-1.0.1/setup.py
+drwxr-xr-x   0 fred      (1000) fred      (1000)        0 2023-04-23 17:45:48.018710 vhatable-1.0.1/vhatable/
+-rw-r--r--   0 fred      (1000) fred      (1000)      958 2023-04-23 15:34:37.000000 vhatable-1.0.1/vhatable/__init__.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     9318 2023-04-23 15:34:41.000000 vhatable-1.0.1/vhatable/cell.py
+-rw-r--r--   0 fred      (1000) fred      (1000)    22474 2023-04-23 15:34:37.000000 vhatable-1.0.1/vhatable/core.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     6758 2023-04-23 15:39:49.000000 vhatable-1.0.1/vhatable/filters.py
+-rw-r--r--   0 fred      (1000) fred      (1000)    20587 2023-04-23 15:37:15.000000 vhatable-1.0.1/vhatable/sample.py
+drwxr-xr-x   0 fred      (1000) fred      (1000)        0 2023-04-23 17:45:48.018710 vhatable-1.0.1/vhatable.egg-info/
+-rwxr-xr-x   0 fred      (1000) fred      (1000)      609 2023-04-23 17:45:47.000000 vhatable-1.0.1/vhatable.egg-info/PKG-INFO
+-rwxr-xr-x   0 fred      (1000) fred      (1000)      319 2023-04-23 17:45:47.000000 vhatable-1.0.1/vhatable.egg-info/SOURCES.txt
+-rwxr-xr-x   0 fred      (1000) fred      (1000)        1 2023-04-23 17:45:47.000000 vhatable-1.0.1/vhatable.egg-info/dependency_links.txt
+-rwxr-xr-x   0 fred      (1000) fred      (1000)       67 2023-04-23 17:45:47.000000 vhatable-1.0.1/vhatable.egg-info/entry_points.txt
+-rwxr-xr-x   0 fred      (1000) fred      (1000)       84 2023-04-23 17:45:47.000000 vhatable-1.0.1/vhatable.egg-info/requires.txt
+-rwxr-xr-x   0 fred      (1000) fred      (1000)        9 2023-04-23 17:45:47.000000 vhatable-1.0.1/vhatable.egg-info/top_level.txt
```

### Comparing `vhatable-1.0.0/setup.py` & `vhatable-1.0.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -73,9 +73,23 @@
     packages=find_packages(exclude=["contrib", "docs", "tests*"]),
 
     # List run-time dependencies here.  These will be installed by pip when your
     # project is installed.
     install_requires=[
         'veryprettytable==0.8.1',
         'humanfriendly==9.0'
-    ]
+    ],
+    extras_require={
+        "SAMPLE": [],
+        'DEV': [
+            'pytest',
+            'flake8',
+            'tox',
+            'pylint',
+        ]
+    },
+    entry_points={
+        "console_scripts": [
+            "vhatable-sample = vhatable.sample:main [SAMPLE]"
+        ],
+    },
 )
```

### Comparing `vhatable-1.0.0/vhatable/__init__.py` & `vhatable-1.0.1/vhatable/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 """TODO"""
 
 
-# This file is part of Linshare api.
+# This file is part of Vhatable api.
 #
-# LinShare api is free software: you can redistribute it and/or modify
+# Vhatable api is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# LinShare api is distributed in the hope that it will be useful,
+# Vhatable api is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with LinShare api.  If not, see <http://www.gnu.org/licenses/>.
+# along with Vhatable api.  If not, see <http://www.gnu.org/licenses/>.
 #
 # Copyright 2014-2016 Frédéric MARTIN
 #
 # Contributors list :
 #
 #  Frédéric MARTIN frederic.martin.fma@gmail.com
 #
 
-__version__ = '1.0.0'
+__version__ = '1.0.1'
 # from .core import *
 from . import core
 from . import cell
 from . import filters
```

### Comparing `vhatable-1.0.0/vhatable/cell.py` & `vhatable-1.0.1/vhatable/cell.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 #! /usr/bin/env python
 # -*- coding: utf-8 -*-
 """TODO"""
 
 
-# This file is part of Linshare cli.
+# This file is part of Vhatable cli.
 #
-# LinShare cli is free software: you can redistribute it and/or modify
+# Vhatable cli is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# LinShare cli is distributed in the hope that it will be useful,
+# Vhatable cli is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with LinShare cli.  If not, see <http://www.gnu.org/licenses/>.
+# along with Vhatable cli.  If not, see <http://www.gnu.org/licenses/>.
 #
 # Copyright 2019 Frédéric MARTIN
 #
 # Contributors list :
 #
 #  Frédéric MARTIN frederic.martin.fma@gmail.com
 #
@@ -39,15 +39,15 @@
     # pylint: disable=too-many-instance-attributes
 
     def __init__(self, raw=False, vertical=False, debug=0):
         self.raw = raw
         self.debug = debug
         self.vertical = vertical
         classname = str(self.__class__.__name__.lower())
-        self.log = logging.getLogger("linsharecli.cell." + classname)
+        self.log = logging.getLogger("vhatablecli.cell." + classname)
         self.date_cells = [
             "creationDate",
             "modificationDate",
             "expirationDate",
             "uploadDate"
         ]
         self.size_cells = ["size"]
```

### Comparing `vhatable-1.0.0/vhatable/core.py` & `vhatable-1.0.1/vhatable/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 #! /usr/bin/env python
 # -*- coding: utf-8 -*-
 """TODO"""
 
 
-# This file is part of Linshare api.
+# This file is part of Vhatable api.
 #
-# LinShare api is free software: you can redistribute it and/or modify
+# Vhatable api is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# LinShare api is distributed in the hope that it will be useful,
+# Vhatable api is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with LinShare api.  If not, see <http://www.gnu.org/licenses/>.
+# along with Vhatable api.  If not, see <http://www.gnu.org/licenses/>.
 #
 # Copyright 2014 Frédéric MARTIN
 #
 # Contributors list :
 #
 #  Frédéric MARTIN frederic.martin.fma@gmail.com
 #
@@ -218,15 +218,15 @@
     _pref_limit = 0
     raw_json = False
     _pref_no_csv_headers = False
 
     def __init__(self, keys=[], reverse=False, debug=0):
         self.debug = debug
         classname = str(self.__class__.__name__.lower())
-        self.log = logging.getLogger('linsharecli.' + classname)
+        self.log = logging.getLogger('vhatable.' + classname)
         self.keys = keys
         # field only use for compatibility with HTable
         self.align = {}
         self.start = None
         self.end = None
         self._rows = []
         self._maxlengthkey = 0
@@ -371,15 +371,15 @@
             header += "".join(["-" for i in range(max_length_line - len(header))])
             out.append(header)
             out.append(record)
         return "\n".join(out)
 
     def add_row(self, row):
         """TODO"""
-        super(VTable, self).add_row(row)
+        super().add_row(row)
         self.update_max_lengthkey(row)
 
     def update_max_lengthkey(self, row):
         """TODO"""
         for k in row:
             self._maxlengthkey = max((len(repr(k)), self._maxlengthkey))
 
@@ -445,15 +445,15 @@
 
     def __init__(self):
         self.cli_mode = False
         self.verbose = False
         self.dry_run = False
         self.debug = 0
         classname = str(self.__class__.__name__.lower())
-        self.log = logging.getLogger('linsharecli.' + classname)
+        self.log = logging.getLogger('vhatable.' + classname)
         self.cli = None
         self.endpoint = None
 
     def init(self, args, cli, endpoint):
         """Init object members with values in args object"""
         self.cli = cli
         self.endpoint = endpoint
@@ -511,15 +511,15 @@
 
 
 class CliModeAction(Action):
     """TODO"""
     # pylint: disable=too-few-public-methods
 
     def __init__(self, identifier="uuid"):
-        super(CliModeAction, self).__init__()
+        super().__init__()
         self.identifier = identifier
 
     def __call__(self, args, cli, endpoint, data):
         """TODO"""
         self.init(args, cli, endpoint)
         for row in data:
             print((str(row.get(self.identifier))))
@@ -527,23 +527,23 @@
 
 
 class SampleAction(Action):
     """TODO"""
     # pylint: disable=too-many-instance-attributes
 
     def __init__(self, name):
-        super(SampleAction, self).__init__()
+        super().__init__()
         self.name = name
 
     def __call__(self, args, cli, endpoint, data):
         """TODO"""
         self.init(args, cli, endpoint)
         print(("ACTION:", self.name))
-        print(cli)
-        print(endpoint)
+        print("CLI:", cli)
+        print("endpoint:", endpoint)
         print(">--- Filtered data ----")
         for row in data:
             print(row)
         print("---- Filtered data ---<")
         return True
 
 
@@ -564,15 +564,15 @@
     # pylint: disable=too-many-instance-attributes
 
     def __init__(self, cli, endpoint, default_sort_column=None,
                  default_actions=True, cli_mode_identifier="uuid"):
         """TODO"""
         # pylint: disable=too-many-arguments
         classname = str(self.__class__.__name__.lower())
-        self.log = logging.getLogger('linsharecli.' + classname)
+        self.log = logging.getLogger('vhatable.' + classname)
         self.cli = cli
         self.endpoint = endpoint
         self.args = None
         self.columns = None
         self.fields = None
         self.cli_mode = False
         self.cli_mode_identifier = cli_mode_identifier
@@ -628,17 +628,17 @@
         """Add specific cell class to format a column."""
         self._custom_cells[column] = clazz
 
     def add_action(self, flag, clazz):
         """Add some custom action class trigger by a flag."""
         self._action_classes[flag] = clazz
 
-    def add_filter_cond(self, cond, *filters):
-        """Add some filters only if cond is true"""
-        if cond:
+    def add_filter_cond(self, condition, *filters):
+        """Add some filters only if condition is true"""
+        if condition:
             for filterr in filters:
                 self.filters.append(filterr)
 
     def add_filters(self, *filters):
         """Add some filters."""
         for filterr in filters:
             self.filters.append(filterr)
@@ -652,50 +652,55 @@
         # This method is a little bit diry, need some refactoring.
         """Build table object"""
         if self.json or self.csv:
             self.vertical = True
         if self.json:
             self.raw = True
             self.no_cell = True
-        if self.fields:
-            self.columns = self.fields
-        if not self.columns:
-            self.columns = self.endpoint.get_rbu().get_keys(self.extended)
+        columns = self.fields
+        if not columns:
+            if not self.columns:
+                if hasattr(self.endpoint, "get_rbu"):
+                    columns = self.endpoint.get_rbu().get_keys(self.extended)
+            else:
+                columns = self.columns
+        if not columns:
+            raise ValueError("Missing columns")
         table = None
         action_classes = OrderedDict(self._action_classes)
         action_classes['cli_mode'] = CliModeAction(self.cli_mode_identifier)
         self.log.debug("action_classes: %s", action_classes)
         for flag, action in list(action_classes.items()):
             if getattr(self.args, flag, False):
-                table = self._action_table(self.columns)
+                table = self._action_table(columns)
                 # a little bit ugly. :(
                 table.action = action
                 # if no_cell property does not exist, we keep the old behaviour
                 self.no_cell = getattr(action, 'no_cell', True)
                 self.raw = True
                 break
         if table is None:
             if self.vertical:
-                table = self._vertical_clazz(self.columns)
+                table = self._vertical_clazz(columns)
             else:
-                table = self._horizontal_clazz(self.columns)
+                table = self._horizontal_clazz(columns)
                 table.padding_width = 1
             for clazz in self._pre_render_classes:
                 table.add_pre_render_class(clazz)
         attrs = [
             "vertical", "json", "raw", "raw_json", "csv", "cli", "endpoint",
             "reverse", "extended", "no_cell", "debug", "verbose", "cli_mode",
         ]
         for attr in attrs:
             setattr(table, attr, getattr(self, attr))
         if self.sort_by is None:
-            if self.default_sort_column and self.default_sort_column in self.columns:
+            if self.default_sort_column and self.default_sort_column in columns:
                 table.sortby = self.default_sort_column
         else:
-            if self.sort_by in self.columns:
+            if self.sort_by in columns:
                 table.sortby = self.sort_by
         self.log.debug("default_sort_column: %s", self.default_sort_column)
         self.log.debug("sort_by: %s", self.sort_by)
         self.log.debug("final sortby: %s", table.sortby)
         # very ugly. need big refactoring of all tables.
         table.reversesort = self.reverse
         table._pref_start = self.start
@@ -707,9 +712,9 @@
                 table.cfa.custom_cells[column] = clazz
         table.cfa.raw = self.raw
         table.cfa.vertical = self.vertical
         table.cfa.debug = self.debug
         table._filters = self.filters
         # compat
         table.args = self.args
-        table.keys = self.columns
+        table.keys = columns
         return table
```

### Comparing `vhatable-1.0.0/vhatable/filters.py` & `vhatable-1.0.1/vhatable/filters.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,55 +1,55 @@
 #! /usr/bin/env python
 # -*- coding: utf-8 -*-
 """This module contains only filters, they are design to be apply to a row
 of a Vertical or Horizotal table."""
 
 
-# This file is part of Linshare cli.
+# This file is part of Vhatable cli.
 #
-# LinShare cli is free software: you can redistribute it and/or modify
+# Vhatable cli is free software: you can redistribute it and/or modify
 # it under the terms of the GNU General Public License as published by
 # the Free Software Foundation, either version 3 of the License, or
 # (at your option) any later version.
 #
-# LinShare cli is distributed in the hope that it will be useful,
+# Vhatable cli is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with LinShare cli.  If not, see <http://www.gnu.org/licenses/>.
+# along with Vhatable cli.  If not, see <http://www.gnu.org/licenses/>.
 #
 # Copyright 2014 Frédéric MARTIN
 #
 # Contributors list :
 #
 #  Frédéric MARTIN frederic.martin.fma@gmail.com
 #
 
 
-
 import datetime
 import re
 import logging
+
 from .cell import BaseCell
 
 
 class Filter:
     """TODO"""
 
     def __init__(self, prop, values=None):
         """ prop name and value(s)"""
         self.prop = prop
         self.values = values
         classname = self.__class__.__name__.lower()
-        self.log = logging.getLogger("linsharecli.filters." + classname)
+        self.log = logging.getLogger("vhatablecli.filters." + classname)
 
     def is_enable(self):
-        """Return true is the current filter is enabled and should be applied."""
+        """Return true is the filter is enabled and should be applied."""
         if self.values is None:
             return False
         if isinstance(self.values, list):
             # pylint: disable=len-as-condition
             if len(self.values) == 0:
                 return False
             for i in self.values:
@@ -90,14 +90,15 @@
             self.log.debug("values: %s", self.values)
             pattern = r"^.*(" + "|".join(self.values) + ").*$"
             self.log.debug("raw pattern: %s", pattern)
             if ignorecase:
                 self.regex = re.compile(pattern, re.IGNORECASE)
             else:
                 self.regex = re.compile(pattern)
+
     def __str__(self):
         return "PartialOr: " + str(self.values)
 
     def __call__(self, row):
         # pylint: disable=too-many-return-statements
         if not self.is_enable():
             return True
@@ -153,15 +154,17 @@
                 if not self.regex[key].match(val):
                     return False
         return True
 
 
 class PartialDate(Filter):
     """Get the current property into the current row, and match the result with
-     a list of values"""
+     a list of values.
+     This filter will be activated/enabled if 'value' is not None.
+     """
 
     def __init__(self, prop, value):
         super().__init__(prop, value)
         if self.is_enable():
             pattern = r"^.*" + value + ".*$"
             self.regex = re.compile(pattern)
```

