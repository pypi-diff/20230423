# Comparing `tmp/ansible-variables-0.4.1.tar.gz` & `tmp/ansible-variables-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansible-variables-0.4.1.tar", last modified: Sun Apr 16 19:09:22 2023, max compression
+gzip compressed data, was "ansible-variables-0.4.2.tar", last modified: Sun Apr 23 15:32:04 2023, max compression
```

## Comparing `ansible-variables-0.4.1.tar` & `ansible-variables-0.4.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:09:22.641183 ansible-variables-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-16 19:09:11.000000 ansible-variables-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4932 2023-04-16 19:09:22.641183 ansible-variables-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3589 2023-04-16 19:09:11.000000 ansible-variables-0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:09:22.637183 ansible-variables-0.4.1/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:09:22.641183 ansible-variables-0.4.1/lib/ansible_variables/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 19:09:11.000000 ansible-variables-0.4.1/lib/ansible_variables/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:09:22.641183 ansible-variables-0.4.1/lib/ansible_variables/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 19:09:11.000000 ansible-variables-0.4.1/lib/ansible_variables/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-04-16 19:09:11.000000 ansible-variables-0.4.1/lib/ansible_variables/cli/variables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:09:22.641183 ansible-variables-0.4.1/lib/ansible_variables/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 19:09:11.000000 ansible-variables-0.4.1/lib/ansible_variables/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3949 2023-04-16 19:09:11.000000 ansible-variables-0.4.1/lib/ansible_variables/utils/vars.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:09:22.641183 ansible-variables-0.4.1/lib/ansible_variables.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4932 2023-04-16 19:09:22.000000 ansible-variables-0.4.1/lib/ansible_variables.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-04-16 19:09:22.000000 ansible-variables-0.4.1/lib/ansible_variables.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 19:09:22.000000 ansible-variables-0.4.1/lib/ansible_variables.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-16 19:09:22.000000 ansible-variables-0.4.1/lib/ansible_variables.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 19:09:22.000000 ansible-variables-0.4.1/lib/ansible_variables.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-16 19:09:22.000000 ansible-variables-0.4.1/lib/ansible_variables.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-16 19:09:22.000000 ansible-variables-0.4.1/lib/ansible_variables.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-16 19:09:11.000000 ansible-variables-0.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-04-16 19:09:22.641183 ansible-variables-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-16 19:09:11.000000 ansible-variables-0.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 19:09:22.641183 ansible-variables-0.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-04-16 19:09:11.000000 ansible-variables-0.4.1/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-04-16 19:09:11.000000 ansible-variables-0.4.1/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-04-16 19:09:11.000000 ansible-variables-0.4.1/tests/test_variablesource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 15:32:04.910076 ansible-variables-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-23 15:31:51.000000 ansible-variables-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4932 2023-04-23 15:32:04.910076 ansible-variables-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3589 2023-04-23 15:31:51.000000 ansible-variables-0.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 15:32:04.906076 ansible-variables-0.4.2/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 15:32:04.906076 ansible-variables-0.4.2/lib/ansible_variables/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 15:31:51.000000 ansible-variables-0.4.2/lib/ansible_variables/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 15:32:04.906076 ansible-variables-0.4.2/lib/ansible_variables/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 15:31:51.000000 ansible-variables-0.4.2/lib/ansible_variables/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3680 2023-04-23 15:31:51.000000 ansible-variables-0.4.2/lib/ansible_variables/cli/variables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 15:32:04.906076 ansible-variables-0.4.2/lib/ansible_variables/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 15:31:51.000000 ansible-variables-0.4.2/lib/ansible_variables/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-04-23 15:31:51.000000 ansible-variables-0.4.2/lib/ansible_variables/utils/vars.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 15:32:04.906076 ansible-variables-0.4.2/lib/ansible_variables.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4932 2023-04-23 15:32:04.000000 ansible-variables-0.4.2/lib/ansible_variables.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-04-23 15:32:04.000000 ansible-variables-0.4.2/lib/ansible_variables.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 15:32:04.000000 ansible-variables-0.4.2/lib/ansible_variables.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-23 15:32:04.000000 ansible-variables-0.4.2/lib/ansible_variables.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 15:32:04.000000 ansible-variables-0.4.2/lib/ansible_variables.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-23 15:32:04.000000 ansible-variables-0.4.2/lib/ansible_variables.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-23 15:32:04.000000 ansible-variables-0.4.2/lib/ansible_variables.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-04-23 15:31:51.000000 ansible-variables-0.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-04-23 15:32:04.910076 ansible-variables-0.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-23 15:31:51.000000 ansible-variables-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 15:32:04.910076 ansible-variables-0.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-04-23 15:31:51.000000 ansible-variables-0.4.2/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-04-23 15:31:51.000000 ansible-variables-0.4.2/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-04-23 15:31:51.000000 ansible-variables-0.4.2/tests/test_variablesource.py
```

### Comparing `ansible-variables-0.4.1/LICENSE` & `ansible-variables-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ansible-variables-0.4.1/PKG-INFO` & `ansible-variables-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansible-variables
-Version: 0.4.1
+Version: 0.4.2
 Summary: Keep track of Ansible host context variables
 Home-page: https://github.com/hille721/ansible-variables
 Author: Christoph Hille
 Author-email: hille721@gmail.com
 License: GPLv3+
 Project-URL: Bug Tracker, https://github.com/hille721/ansible-variables/issues
 Project-URL: Documentation, https://github.com/hille721/ansible-variables/blob/main/README.md
```

### Comparing `ansible-variables-0.4.1/README.md` & `ansible-variables-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `ansible-variables-0.4.1/lib/ansible_variables/cli/variables.py` & `ansible-variables-0.4.2/lib/ansible_variables/cli/variables.py`

 * *Files 4% similar despite different names*

```diff
@@ -93,15 +93,15 @@
         return options
 
     def run(self):
         super().run()
 
         # Initialize needed objects
         self.loader, self.inventory, self.vm = self._play_prereqs()
-        verbosity = context.CLIARGS["verbosity"]
+        verbosity = display.verbosity
 
         host = self.inventory.get_host(context.CLIARGS["host"])
         if not host:
             raise AnsibleOptionsError("You must pass a single valid host to ansible-variables")
 
         for variable in variable_sources(
             variable_manager=self.vm,
```

### Comparing `ansible-variables-0.4.1/lib/ansible_variables/utils/vars.py` & `ansible-variables-0.4.2/lib/ansible_variables/utils/vars.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,15 +78,15 @@
 
     def file_occurrences(self, loader: DataLoader):
         """Open the files and check if the variables occur in it"""
         occurrences = []
 
         for ffile in self.files:
             display.vvv("Checking file %s for occurrence of variable %s" % (ffile, self.name))
-            if self.name in loader.load_from_file(ffile):
+            if loader.load_from_file(ffile) and self.name in loader.load_from_file(ffile):
                 occurrences.append(ffile)
 
         return occurrences
 
 
 def variable_sources(
     variable_manager: VariableManager,
```

### Comparing `ansible-variables-0.4.1/lib/ansible_variables.egg-info/PKG-INFO` & `ansible-variables-0.4.2/lib/ansible_variables.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansible-variables
-Version: 0.4.1
+Version: 0.4.2
 Summary: Keep track of Ansible host context variables
 Home-page: https://github.com/hille721/ansible-variables
 Author: Christoph Hille
 Author-email: hille721@gmail.com
 License: GPLv3+
 Project-URL: Bug Tracker, https://github.com/hille721/ansible-variables/issues
 Project-URL: Documentation, https://github.com/hille721/ansible-variables/blob/main/README.md
```

### Comparing `ansible-variables-0.4.1/lib/ansible_variables.egg-info/SOURCES.txt` & `ansible-variables-0.4.2/lib/ansible_variables.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ansible-variables-0.4.1/setup.cfg` & `ansible-variables-0.4.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ansible-variables
-version = 0.4.1
+version = 0.4.2
 description = Keep track of Ansible host context variables
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Christoph Hille
 author_email = hille721@gmail.com
 url = https://github.com/hille721/ansible-variables
 project_urls =
```

### Comparing `ansible-variables-0.4.1/tests/test_utils.py` & `ansible-variables-0.4.2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `ansible-variables-0.4.1/tests/test_variablesource.py` & `ansible-variables-0.4.2/tests/test_variablesource.py`

 * *Files 11% similar despite different names*

```diff
@@ -47,19 +47,35 @@
 def test_occurrence():
     C.set_constant("CONFIG_FILE", "tests/test_data/ansible.cfg")
 
     var_source = VariableSource(
         name="from_all",
         value="bar",
         source="foobar",
-        debuglog="""\x1b[1;30m  5108 1681472141.30319: Loading data from tests/test_data/inventory/group_vars/all\x1b[0m
-        \x1b[1;30m  5108 1681472141.30388: Loading data from tests/test_data/inventory/group_vars/groupA.yml\x1b[0m
+        debuglog="""\x1b[1;30m  5108 81472141.303: Loading data from tests/test_data/inventory/group_vars/all/all\x1b[0m
+        \x1b[1;30m  5108 81472141.30388: Loading data from tests/test_data/inventory/group_vars/groupA.yml\x1b[0m
         """,
     )
 
     assert var_source.value == "bar"
     assert var_source.source_mapped == "foobar"
     assert var_source.files == [
-        "tests/test_data/inventory/group_vars/all",
+        "tests/test_data/inventory/group_vars/all/all",
         "tests/test_data/inventory/group_vars/groupA.yml",
     ]
-    assert var_source.file_occurrences(loader=loader) == ["tests/test_data/inventory/group_vars/all"]
+    assert var_source.file_occurrences(loader=loader) == ["tests/test_data/inventory/group_vars/all/all"]
+
+
+def test_empty_file():
+    C.set_constant("CONFIG_FILE", "tests/test_data/ansible.cfg")
+
+    var_source = VariableSource(
+        name="from_all",
+        value="bar",
+        source="foobar",
+        debuglog="Loading data from tests/test_data/inventory/group_vars/all/empty",
+    )
+
+    assert var_source.files == [
+        "tests/test_data/inventory/group_vars/all/empty",
+    ]
+    assert not var_source.file_occurrences(loader=loader)
```

