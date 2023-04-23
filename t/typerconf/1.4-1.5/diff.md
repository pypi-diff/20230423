# Comparing `tmp/typerconf-1.4.tar.gz` & `tmp/typerconf-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typerconf-1.4.tar", max compression
+gzip compressed data, was "typerconf-1.5.tar", max compression
```

## Comparing `typerconf-1.4.tar` & `typerconf-1.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1074 2023-03-22 18:19:29.446288 typerconf-1.4/LICENSE
--rw-r--r--   0        0        0     1363 2023-03-24 07:02:49.103915 typerconf-1.4/README.md
--rw-r--r--   0        0        0      934 2023-04-20 07:42:25.027099 typerconf-1.4/pyproject.toml
--rw-r--r--   0        0        0       30 2023-03-23 10:49:11.282231 typerconf-1.4/src/typerconf/.gitignore
--rw-r--r--   0        0        0      258 2023-03-22 14:14:56.966915 typerconf-1.4/src/typerconf/Makefile
--rw-r--r--   0        0        0     6692 2023-04-20 07:42:46.010795 typerconf-1.4/src/typerconf/__init__.py
--rw-r--r--   0        0        0    16558 2023-04-20 07:40:09.981015 typerconf-1.4/src/typerconf/init.nw
--rw-r--r--   0        0        0     2508 1970-01-01 00:00:00.000000 typerconf-1.4/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-03-22 18:19:29.446288 typerconf-1.5/LICENSE
+-rw-r--r--   0        0        0     1363 2023-03-24 07:02:49.103915 typerconf-1.5/README.md
+-rw-r--r--   0        0        0      934 2023-04-23 09:48:23.436444 typerconf-1.5/pyproject.toml
+-rw-r--r--   0        0        0       30 2023-03-23 10:49:11.282231 typerconf-1.5/src/typerconf/.gitignore
+-rw-r--r--   0        0        0      258 2023-03-22 14:14:56.966915 typerconf-1.5/src/typerconf/Makefile
+-rw-r--r--   0        0        0     6567 2023-04-23 09:48:55.900330 typerconf-1.5/src/typerconf/__init__.py
+-rw-r--r--   0        0        0    19038 2023-04-23 09:43:51.934399 typerconf-1.5/src/typerconf/init.nw
+-rw-r--r--   0        0        0     2508 1970-01-01 00:00:00.000000 typerconf-1.5/PKG-INFO
```

### Comparing `typerconf-1.4/LICENSE` & `typerconf-1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `typerconf-1.4/README.md` & `typerconf-1.5/README.md`

 * *Files identical despite different names*

### Comparing `typerconf-1.4/pyproject.toml` & `typerconf-1.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "typerconf"
-version = "1.4"
+version = "1.5"
 description = "Library to read and write configs using API and CLI with Typer"
 authors = ["Daniel Bosk <daniel@bosk.se>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/dbosk/typerconf"
 keywords = ["typer", "conf", "config", "git-like", "config lib", "write conf"]
 classifiers = [
```

### Comparing `typerconf-1.4/src/typerconf/__init__.py` & `typerconf-1.5/src/typerconf/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,15 +38,14 @@
       return structure
 
     for part in path.split("."):
       try:
         part = int(part)
       except ValueError:
         pass
-
       try:
         structure = structure[part]
       except KeyError:
         raise KeyError(f"{part} along {path} doesn't exist")
 
     return structure
 
@@ -94,15 +93,14 @@
     if value is None:
       try:
         del structure[part]
       except KeyError:
         pass
     else:
       structure[part] = value
-
   def paths(self, from_root=""):
     """
     Returns all existing paths.
 
     The optional argument `from_root` is a path and the method return all 
     subpaths rooted at that point.
     """
@@ -118,101 +116,91 @@
 
         paths.append(path)
         paths += self.paths(from_root=path)
     elif isinstance(root, list):
       paths += [f"{from_root}.{x}" for x in range(len(root))]
 
     return paths
+  def read_config(self, conf_path=f"{dirs.user_config_dir}/config.json"):
+    """
+    Reads the config data structure (JSON) into the Config object.
+    `conf_path` is an optional argument providing the path to the config file.
+
+    
+    """
+    try:
+      with open(conf_path) as conf_file:
+        self.__data = json.load(conf_file)
+        return
+    except FileNotFoundError as err:
+      logging.warning(f"Config file {conf_path} could not be found: {err}")
+    except NotADirectoryError as err:
+      logging.error(f"A part of the path is a file, but used as directory: {err}")
+      raise err
+    except json.decoder.JSONDecodeError as err:
+      logging.warning(f"Config file {conf_path} could not be decoded: {err}")
+  def write_config(self, conf_path=f"{dirs.user_config_dir}/config.json"):
+    """
+    Stores the config data (as JSON) in the config file.
+    `conf_path` is an optional argument providing the path to the config file.
+    """
+    conf_dir = os.path.dirname(conf_path)
+    if not os.path.isdir(conf_dir):
+      os.makedirs(conf_dir)
+
+    with open(conf_path, "w") as conf_file:
+      json.dump(self.__data, conf_file)
 def add_config_cmd(cli: typer.Typer):
   """
   Add config command to Typer cli
   """
   path_arg = typer.Argument(...,
                             help="Path in config, e.g. 'courses.datintro22'. "
                                  "Empty string is root of config.",
-                            autocompletion=complete_path_callback)
+                            shell_complete=complete_path_callback)
   value_arg = typer.Option([], "-s", "--set",
                            help="Values to store. "
                                 "More than one value makes a list. "
                                 "Values are treated as JSON if possible.")
 
   @cli.command(name="config")
   def config_cmd(path: str = path_arg,
                  values: typing.List[str] = value_arg):
     """
     Reads values from or writes values to the config.
     """
     if values:
+      if len(values) == 1:
+        values = values[0]
       set(path, values)
     else:
       print_config(get(path), path)
 def get(path: str = "") -> typing.Any:
   """
   Returns the value stored at `path` in the config.
 
   By default, `path = ""`, which returns the entire configuration as a Config 
   object.
   """
-  conf = read_config()
+  conf = Config()
+  conf.read_config()
   return conf.get(path)
 
 def set(path: str, value: typing.Any):
   """
   Sets `value` at `path` in the config. `value` will be interpreted as JSON, if 
   conversion to JSON fails, it will be used as is.
 
   If `value` is `None`, the entry referenced by `path` will be deleted, if it 
   exists.
   """
-  conf = read_config()
-  if isinstance(value, list):
-    for i in range(len(value)):
-      try:
-        value[i] = json.loads(value[i])
-      except:
-        pass
-    if len(value) == 1:
-      value = value[0]
-  else:
-    try:
-      value = json.loads(value)
-    except:
-      pass
-
+  conf = Config()
+  conf.read_config()
   conf.set(path, value)
-  write_config(conf)
-def read_config(conf_path=f"{dirs.user_config_dir}/config.json"):
-  """
-  Returns the config data structure (JSON).
-  `conf_path` is an optional argument providing the path to the config file.
-  """
-  try:
-    with open(conf_path) as conf_file:
-      return Config(json.load(conf_file))
-  except FileNotFoundError as err:
-    logging.warning(f"Config file {conf_path} could not be found: {err}")
-  except NotADirectoryError as err:
-    logging.error(f"A part of the path is a file, but used as directory: {err}")
-    raise err
-  except json.decoder.JSONDecodeError as err:
-    logging.warning(f"Config file {conf_path} could not be decoded: {err}")
-
-  return Config()
-def write_config(conf,
-                 conf_path=f"{dirs.user_config_dir}/config.json"):
-  """
-  Stores the config data `conf` (extracts JSON) in the config file.
-  `conf_path` is an optional argument providing the path to the config file.
-  """
-  conf_dir = os.path.dirname(conf_path)
-  if not os.path.isdir(conf_dir):
-    os.makedirs(conf_dir)
-
-  with open(conf_path, "w") as conf_file:
-    json.dump(conf.get(), conf_file)
+  conf.write_config()
 def complete_path(initial_path: str, conf: Config = None):
   """
   Returns all valid paths in the config starting with `initial_path`.
   If `conf` is not None, use that instead of the actual config.
   """
   if not conf:
     conf = Config(get())
@@ -231,14 +219,15 @@
       if path:
         print_config(conf[key], f"{path}.{key}")
       else:
         print_config(conf[key], key)
   except AttributeError:
     print(f"{path} = {conf}")
 
+
 def main():
   cli = typer.Typer()
   add_config_cmd(cli)
   cli()
 
 if __name__ == "__main__":
   main()
```

### Comparing `typerconf-1.4/src/typerconf/init.nw` & `typerconf-1.5/src/typerconf/init.nw`

 * *Files 8% similar despite different names*

```diff
@@ -67,19 +67,25 @@
 
 \subsection{Testing}
 
 We also want to test all functions we provide in this module.
 These test functions are all prepended [[test_]] to the function name.
 We will run them using [[pytest]].
 <<test init.py>>=
+import sys
+sys.argv[0] = "typerconf"
+
 import typer
 from typerconf import *
 
 <<test imports>>
 
+cli = typer.Typer()
+add_config_cmd(cli)
+
 <<test functions>>
 @
 
 Let's test the [[add_config_cmd]] function from above.
 <<test functions>>=
 def test_add_config_cmd():
   cli = typer.Typer()
@@ -100,195 +106,14 @@
 <<set up appdirs dirs>>=
 normalized_path = os.path.normpath(sys.argv[0])
 basename = os.path.basename(normalized_path)
 dirs = appdirs.AppDirs(basename)
 @
 
 
-\section{Accessing the configuration: the [[get]] and [[set]] functions}
-
-We will provide two functions, [[get]] and [[set]], that modifies the config, 
-immediately syncing to the file system.
-This is the API to be used by any part of a program using this module to manage 
-the configuration.
-<<helper functions>>=
-def get(path: str = "") -> typing.Any:
-  """
-  Returns the value stored at `path` in the config.
-
-  By default, `path = ""`, which returns the entire configuration as a Config 
-  object.
-  """
-  <<read config from file>>
-  <<return the value at path in config>>
-
-def set(path: str, value: typing.Any):
-  """
-  Sets `value` at `path` in the config. `value` will be interpreted as JSON, if 
-  conversion to JSON fails, it will be used as is.
-
-  If `value` is `None`, the entry referenced by `path` will be deleted, if it 
-  exists.
-  """
-  <<read config from file>>
-  <<set the value at path in config>>
-  <<write config back to file>>
-@
-
-Let's start with reading and writing the config file.
-<<read config from file>>=
-conf = read_config()
-<<write config back to file>>=
-write_config(conf)
-@ We'll see these functions in \cref{ConfigFile}.
-
-Now that we have the config structure in [[conf]] we can use it.
-Let's start with getting a value.
-<<return the value at path in config>>=
-return conf.get(path)
-@
-
-Now, to set a value, we have several cases.
-If the user supplied more than one value, we want a list.
-If only one value, we don't want to store a list with only one value in it.
-Also, we want to try interpret any value as JSON.
-If that fails, we'll use the value as-is.
-<<set the value at path in config>>=
-if isinstance(value, list):
-  <<try to convert each element to JSON>>
-  if len(value) == 1:
-    value = value[0]
-else:
-  try:
-    value = json.loads(value)
-  except:
-    pass
-
-conf.set(path, value)
-@
-
-When we try to convert each element to JSON, we do it in place; hence iterate 
-over the index rather than the elements directly.
-<<try to convert each element to JSON>>=
-for i in range(len(value)):
-  try:
-    value[i] = json.loads(value[i])
-  except:
-    pass
-@
-
-Now let's cover [[read_config]], [[write_config]], [[set_path]] and 
-[[get_path]] below.
-
-
-\section{Reading and writing the config file}\label{ConfigFile}
-
-The configuration file is stored in a suitable system location.
-For this we use the AppDirs package, we have the [[dirs]] instance above.
-We want to read the config and return a JSON structure as outlined above 
-(\cref{ConfigStructure}).
-<<helper functions>>=
-def read_config(conf_path=f"{dirs.user_config_dir}/config.json"):
-  """
-  Returns the config data structure (JSON).
-  `conf_path` is an optional argument providing the path to the config file.
-  """
-  try:
-    with open(conf_path) as conf_file:
-      return Config(json.load(conf_file))
-  <<handle read config file errors>>
-
-  return Config()
-@
-
-And conversely, write one to the config file as well.
-Here it's important to use the [[os.makedirs]] (not [[os.mkdir]]) to create the 
-entire hierarchy of parent directories too, if they don't exist.
-We don't need any error handling for writing though, because all errors a 
-fatal, we can't recover from any of the possible errors.
-<<helper functions>>=
-def write_config(conf,
-                 conf_path=f"{dirs.user_config_dir}/config.json"):
-  """
-  Stores the config data `conf` (extracts JSON) in the config file.
-  `conf_path` is an optional argument providing the path to the config file.
-  """
-  conf_dir = os.path.dirname(conf_path)
-  if not os.path.isdir(conf_dir):
-    os.makedirs(conf_dir)
-
-  with open(conf_path, "w") as conf_file:
-    json.dump(conf.get(), conf_file)
-@
-
-When reading the config file there are some errors that can occur.
-The first is that the file doesn't exist ([[FileNotFoundError]]).
-There is also a related one, [[NotADirectoryError]].
-The problem of [[NotADirectoryError]] occurs when a file on the path is used as 
-a directory --- but only for reading, when trying to create a directory 
-hierarchy, it will yield [[FileExistsError]].
-We can't recover from this error, as an attempt to write to the file will also 
-fail.
-Finally, the file exists, but it's not proper JSON ([[JSONDecodeError]]).
-<<handle read config file errors>>=
-except FileNotFoundError as err:
-  logging.warning(f"Config file {conf_path} could not be found: {err}")
-except NotADirectoryError as err:
-  logging.error(f"A part of the path is a file, but used as directory: {err}")
-  raise err
-except json.decoder.JSONDecodeError as err:
-  logging.warning(f"Config file {conf_path} could not be decoded: {err}")
-@
-
-Now, let's test the read errors.
-<<test functions>>=
-def test_conf_read_errors():
-  """FileNotFoundError"""
-  conf = read_config("/this/path/should/never/exist/config.json")
-  """JSONDecodeError"""
-  conf = read_config("/dev/null")
-  """NotADirectoryError"""
-  try:
-    conf = read_config("/dev/null/config.json")
-  except NotADirectoryError:
-    assert True
-  else:
-    assert False
-@
-
-Writing to the config file can also yield errors.
-<<test functions>>=
-def test_conf_write_errors():
-  conf = Config({})
-  """Should succeed"""
-  write_config(conf, "/dev/null")
-  """Should yield FileExistsError"""
-  try:
-    write_config(conf, "/dev/null/config.json")
-  except NotADirectoryError:
-    assert False
-  except FileExistsError:
-    assert True
-  else:
-    assert False
-  """Should yield permission error"""
-  try:
-    write_config(conf, "/this/path/should/never/exist/config.json")
-  except PermissionError:
-    assert True
-  else:
-    assert False
-  """Should succeed"""
-  path = tempfile.mkdtemp()
-  write_config(conf, f"{path}/this/is/a/new/path/config.json")
-<<test imports>>=
-import tempfile
-@
-
-
 \section{Navigating config structures}\label{ConfigClass}
 
 We provide the class [[Config]] to navigate the config structure.
 This class has two methods that are central:
 The first gets a value out, the other sets a value in.
 Both work with these dot-separated addresses.
 <<classes>>=
@@ -297,191 +122,225 @@
 
   def __init__(self, json_data={}):
     """
     Constructs a config object to navigate from JSON data `json_data`.
     """
     self.__data = json_data
 
-  def get(self, path: str = "") -> typing.Any:
-    """
-    Returns object at `path`.
-    Example:
-    - `path = "courses.datintro22.url"` and
-    - Config contains `{"courses": {"datintro22": {"url": "https://..."}}}` 
-      will return "https://...".
-
-    Any part of the path that can be converted to an integer, will be converted 
-    to an integer. This way we can access elements of lists too.
-    """
-    <<get value at path>>
-
-  def set(self, path: str, value: typing.Any):
-    """
-    Sets `value` at `path`. Any parts along the path that don't exist will be 
-    created.
-
-    Example:
-    - `value = "https://..."`,
-    - `path = "courses.datintro22.url"`
-    will create `{"courses": {"datintro22": {"url": "https://..."}}}`.
-
-    Any part of the path that can be converted to an integer, will be converted 
-    to an integer. This way we can access elements of lists too. However, we 
-    cannot create index 3 in a list if it doesn't exist (we can't expand 
-    lists).
-
-    If `value` is `None`, the entry at `path` will be deleted, if it exists.
-    """
-    <<set value at path>>
-
-  def paths(self, from_root=""):
-    """
-    Returns all existing paths.
-
-    The optional argument `from_root` is a path and the method return all 
-    subpaths rooted at that point.
-    """
-    <<return list of all paths>>
+  <<Config methods for get and set>>
+  <<Config methods for available paths>>
+  <<Config methods for reading from and writing to file>>
 @
 
-We test these methods with the examples from the docstrings.
+We will use the following test data for the test functions.
 <<test functions>>=
 conf = Config({
   "courses": {
     "datintro22": {
       "url": "https://...",
       "TAs": ["Asse", "Assa"]
     }
   }
 })
+@
 
-def test_get_path():
-  assert conf.get("courses.datintro22.url") == "https://..."
-  assert conf.get("courses.datintro22.TAs.0") == "Asse"
+\subsection{Getting and setting values}
 
-def test_set_path():
-  value = "Asselina"
-  path = "courses.datintro22.TAs.0"
-  conf.set(path, value)
-  assert conf.get(path) == value
+We want to be able to get and set values at different paths in the config.
+<<Config methods for get and set>>=
+def get(self, path: str = "") -> typing.Any:
+  """
+  Returns object at `path`.
+  Example:
+  - `path = "courses.datintro22.url"` and
+  - Config contains `{"courses": {"datintro22": {"url": "https://..."}}}` 
+    will return "https://...".
 
-  value = ["Asse", "Assa", "Asselina"]
-  path = "courses.prgx22.TAs"
-  conf.set(path, value)
-  gotten_value = conf.get(path)
-  assert isinstance(gotten_value, list)
-  assert len(gotten_value) == len(value)
+  Any part of the path that can be converted to an integer, will be converted 
+  to an integer. This way we can access elements of lists too.
+  """
+  <<get value at path>>
 
-  value = {"A": 1, "B": 2}
-  conf.set("test", value)
-  gotten_value = conf.get("test")
-  assert value == gotten_value
+def set(self, path: str, value: typing.Any):
+  """
+  Sets `value` at `path`. Any parts along the path that don't exist will be 
+  created.
 
-  conf.set("test", None)
-  try:
-    conf.get("test")
-  except KeyError:
-    assert True
-  else:
-    assert False
+  Example:
+  - `value = "https://..."`,
+  - `path = "courses.datintro22.url"`
+  will create `{"courses": {"datintro22": {"url": "https://..."}}}`.
 
-def test_paths():
-  assert "courses.datintro22.TAs" in conf.paths()
-  for path in conf.paths():
-    assert conf.get(path)
+  Any part of the path that can be converted to an integer, will be converted 
+  to an integer. This way we can access elements of lists too. However, we 
+  cannot create index 3 in a list if it doesn't exist (we can't expand 
+  lists).
+
+  If `value` is `None`, the entry at `path` will be deleted, if it exists.
+  """
+  <<set value at path>>
 @
 
-\subsection{Getting values}
+\subsubsection{Getting values}
 
 To get the value, we simply walk along the path and returns what remains.
 <<get value at path>>=
 structure = self.__data
 
 if not path:
   return structure
 
 for part in path.split("."):
-  try:
-    part = int(part)
-  except ValueError:
-    pass
-
+  <<check if part is an integer, if so, convert it>>
   try:
     structure = structure[part]
   except KeyError:
     raise KeyError(f"{part} along {path} doesn't exist")
 
 return structure
 @
 
-\subsection{Setting values}
+We can test this as follows.
+<<test functions>>=
+def test_get_path():
+  assert conf.get("courses.datintro22.url") == "https://..."
+@
+
+To handle integers on the path, we do it in the pythonic way: we try to convert 
+it, if it fails, we just continue with the non-integer value.
+<<check if part is an integer, if so, convert it>>=
+try:
+  part = int(part)
+except ValueError:
+  pass
+@
+
+We can test this as follows.
+<<test functions>>=
+def test_get_path_int():
+  assert conf.get("courses.datintro22.TAs.0") == "Asse"
+@
+
+\subsubsection{Setting values}
 
 To set a value is a bit more complex.
 We want to be able to specify a path and create all parents along the path if 
 they don't exist.
 However, if the value is [[None]], we don't want to create an entry that 
 doesn't exist, but we want to delete one if it already exists.
 <<set value at path>>=
 structure = self.__data
 
 parts = path.split(".")
 
 <<update structure to parent node, create parents if they don't exist>>
 
 part = parts[-1]
+<<check if part is an integer, if so, convert it>>
+
+if value is None:
+  <<remove part from the config>>
+else:
+  structure[part] = value
+@
+
+We can test this as follows.
+<<test functions>>=
+def test_set_path_in_list():
+  value = "Asselina"
+  path = "courses.datintro22.TAs.0"
+  conf.set(path, value)
+  assert conf.get(path) == value
+
+def test_set_path_list():
+  value = ["Asse", "Assa", "Asselina"]
+  path = "courses.prgx22.TAs"
+  conf.set(path, value)
+  gotten_value = conf.get(path)
+  assert isinstance(gotten_value, list)
+  assert gotten_value == value
+@
+
+When we want to remove a node, the pythonic way is to simply try to remove it.
+If it doesn't exist, we silently fail.
+The reasoning is as follows: the goal is to remove something; if it doesn't 
+exist, we have already achieved our goal.
+(However, giving an error, as the rm(1) command does, helps in debugging.
+But we consider this silently failing most beneficial at the moment.)
+<<remove part from the config>>=
 try:
-  part = int(part)
-except ValueError:
+  del structure[part]
+except KeyError:
   pass
+@
 
-if value is None:
+We can test this as follows.
+<<test functions>>=
+def test_set_path_remove():
+  conf.set("test", "test")
+  assert conf.get("test") == "test"
+
+  conf.set("test", None)
   try:
-    del structure[part]
+    conf.get("test")
   except KeyError:
-    pass
-else:
-  structure[part] = value
+    assert True
+  else:
+    assert False
 @
 
 We want to traverse the tree, we want to go to the immediate parent of the leaf 
 that we want to set a value for (or delete).
 We iterate through the path.
 <<update structure to parent node, create parents if they don't exist>>=
 for part in parts[:-1]:
   <<check if part is an integer, if so, convert it>>
   try:
     structure = structure[part]
   except KeyError:
     <<handle node that doesn't exist>>
 @
 
-To handle integers on the path, we do it in the pythonic way: we try to convert 
-it, if it fails, we just continue with the non-integer value.
-<<check if part is an integer, if so, convert it>>=
-try:
-  part = int(part)
-except ValueError:
-  pass
-@
-
 If a node along the path doesn't exist, we want to create it.
 However, if [[value]] is [[None]], we actually want to delete the leaf, then we 
 don't create the parents if they don't exist either.
 <<handle node that doesn't exist>>=
 if value is None:
   return
 else:
   structure[part] = {}
   structure = structure[part]
 @
 
-\subsection{All existing paths}
+We can test this as follows.
+<<test functions>>=
+def test_set_path_create_parents():
+  path = "test.some.nonexisting.parents"
+  value = {"A": 1, "B": 2}
+  conf.set(path, value)
+  gotten_value = conf.get(path)
+  assert value == gotten_value
+@
+
+\subsection{Listing all existing paths}
 
 Lastly, what we want to do is to create a list containing all paths in the 
 config.
+<<Config methods for available paths>>=
+def paths(self, from_root=""):
+  """
+  Returns all existing paths.
+
+  The optional argument `from_root` is a path and the method return all 
+  subpaths rooted at that point.
+  """
+  <<return list of all paths>>
+@
+
+What we want to do is to create a list containing all paths in the config.
 We will simply traverse the config tree and add paths as we go.
 We need to treat dictionaries and lists differently.
 And anything else is a leaf.
 <<return list of all paths>>=
 paths = []
 root = self.get(from_root)
 
@@ -496,42 +355,231 @@
     paths += self.paths(from_root=path)
 elif isinstance(root, list):
   paths += [f"{from_root}.{x}" for x in range(len(root))]
 
 return paths
 @
 
+We can test it like this.
+<<test functions>>=
+def test_paths():
+  assert "courses.datintro22.TAs" in conf.paths()
+  for path in conf.paths():
+    assert conf.get(path)
+@
+
+\subsection{Reading and writing the config file}\label{ConfigFile}
+
+The configuration file is stored in a suitable system location.
+We use the AppDirs package for the default location, we have the [[dirs]] 
+instance above.
+We want to read the config and load the JSON structure as outlined above 
+(\cref{ConfigStructure}).
+<<Config methods for reading from and writing to file>>=
+def read_config(self, conf_path=f"{dirs.user_config_dir}/config.json"):
+  """
+  Reads the config data structure (JSON) into the Config object.
+  `conf_path` is an optional argument providing the path to the config file.
+
+  <<documentation of config read error handling>>
+  """
+  try:
+    with open(conf_path) as conf_file:
+      self.__data = json.load(conf_file)
+      return
+  <<handle read config file errors>>
+@
+
+And conversely, write one to the config file as well.
+Here it's important to use the [[os.makedirs]] (not [[os.mkdir]]) to create the 
+entire hierarchy of parent directories too, if they don't exist.
+We don't need any error handling for writing though, because all errors are 
+fatal, we can't recover from any of the possible errors.
+<<Config methods for reading from and writing to file>>=
+def write_config(self, conf_path=f"{dirs.user_config_dir}/config.json"):
+  """
+  Stores the config data (as JSON) in the config file.
+  `conf_path` is an optional argument providing the path to the config file.
+  """
+  conf_dir = os.path.dirname(conf_path)
+  if not os.path.isdir(conf_dir):
+    os.makedirs(conf_dir)
+
+  with open(conf_path, "w") as conf_file:
+    json.dump(self.__data, conf_file)
+@
+
+When reading the config file there are some errors that can occur.
+The first is that the file doesn't exist ([[FileNotFoundError]]).
+There is also a related one, [[NotADirectoryError]].
+The problem of [[NotADirectoryError]] occurs when a file on the path is used as 
+a directory --- but only for reading, when trying to create a directory 
+hierarchy, it will yield [[FileExistsError]].
+We can't recover from this error, as an attempt to write to the file will also 
+fail.
+Finally, the file exists, but it's not proper JSON ([[JSONDecodeError]]).
+<<handle read config file errors>>=
+except FileNotFoundError as err:
+  logging.warning(f"Config file {conf_path} could not be found: {err}")
+except NotADirectoryError as err:
+  logging.error(f"A part of the path is a file, but used as directory: {err}")
+  raise err
+except json.decoder.JSONDecodeError as err:
+  logging.warning(f"Config file {conf_path} could not be decoded: {err}")
+@
+
+<<documentation of config read error handling>>=
+@
+
+Now, let's test the read errors.
+<<test functions>>=
+def test_conf_read_errors():
+  """FileNotFoundError"""
+  conf = Config()
+  conf.read_config("/this/path/should/never/exist/config.json")
+  """JSONDecodeError"""
+  conf.read_config("/dev/null")
+  """NotADirectoryError"""
+  try:
+    conf.read_config("/dev/null/config.json")
+  except NotADirectoryError:
+    assert True
+  else:
+    assert False
+@
+
+Writing to the config file can also yield errors.
+<<test functions>>=
+def test_conf_write_errors():
+  conf = Config({})
+  """Should succeed"""
+  conf.write_config("/dev/null")
+  """Should yield FileExistsError"""
+  try:
+    conf.write_config("/dev/null/config.json")
+  except NotADirectoryError:
+    assert False
+  except FileExistsError:
+    assert True
+  else:
+    assert False
+  """Should yield permission error"""
+  try:
+    conf.write_config("/this/path/should/never/exist/config.json")
+  except PermissionError:
+    assert True
+  else:
+    assert False
+  """Should succeed"""
+  path = tempfile.mkdtemp()
+  conf.write_config(f"{path}/this/is/a/new/path/config.json")
+<<test imports>>=
+import tempfile
+@
+
+
+\section{Accessing the default configuration:
+  the [[get]] and [[set]] functions}
+
+We will provide two module-level functions, [[get]] and [[set]], that allows 
+access to the default config, immediately syncing to the file system.
+<<helper functions>>=
+def get(path: str = "") -> typing.Any:
+  """
+  Returns the value stored at `path` in the config.
+
+  By default, `path = ""`, which returns the entire configuration as a Config 
+  object.
+  """
+  conf = Config()
+  conf.read_config()
+  return conf.get(path)
+
+def set(path: str, value: typing.Any):
+  """
+  Sets `value` at `path` in the config. `value` will be interpreted as JSON, if 
+  conversion to JSON fails, it will be used as is.
+
+  If `value` is `None`, the entry referenced by `path` will be deleted, if it 
+  exists.
+  """
+  conf = Config()
+  conf.read_config()
+  conf.set(path, value)
+  conf.write_config()
+@
+
 
 \section{The [[config]] command}
 
 We will provide the [[config]] command as outlined above.
 If it gets a value, it will set it as the value at path.
 Otherwise, it will print the current value at path.
 <<config subcommands>>=
 path_arg = typer.Argument(...,
                           help="Path in config, e.g. 'courses.datintro22'. "
                                "Empty string is root of config.",
-                          autocompletion=complete_path_callback)
+                          shell_complete=complete_path_callback)
 value_arg = typer.Option([], "-s", "--set",
                          help="Values to store. "
                               "More than one value makes a list. "
                               "Values are treated as JSON if possible.")
 
 @cli.command(name="config")
 def config_cmd(path: str = path_arg,
                values: typing.List[str] = value_arg):
   """
   Reads values from or writes values to the config.
   """
   if values:
+    <<change [[values]] to non-list if one-element list>>
     set(path, values)
   else:
     print_config(get(path), path)
 @
 
+If the user supplies only one argument on the command line, we don't want it to 
+be interpreted as a one-element list, but rather as a value that is not a list.
+Hence, we check and convert if necessary.
+<<change [[values]] to non-list if one-element list>>=
+if len(values) == 1:
+  values = values[0]
+@
+
+Let's test this command.
+<<test functions>>=
+runner = CliRunner()
+
+def test_cli():
+  # set example data
+  result = runner.invoke(cli,
+                         ["courses.datintro22.url", "--set", "https://..."])
+  assert result.exit_code == 0
+
+  # try access nonexisting
+  result = runner.invoke(cli, ["courses.datintro.url"])
+  assert result.exit_code == 1
+
+  # access existing
+  result = runner.invoke(cli, ["courses.datintro22.url"])
+  assert "courses.datintro22.url = https://..." in result.stdout
+
+  # clear config
+  result = runner.invoke(cli,
+                         ["courses", "--set", None])
+  assert result.exit_code == 0
+
+  # check that it's cleared
+  result = runner.invoke(cli, ["courses"])
+  assert "courses" not in result.stdout
+<<test imports>>=
+from typer.testing import CliRunner
+@
+
+
 \subsection{Autocompleting the path}
 
 The [[complete_path]] function returns the possible completions for an 
 incomplete path from the command line.
 <<helper functions>>=
 def complete_path(initial_path: str, conf: Config = None):
   """
@@ -575,22 +623,45 @@
 
 That [[print_config]] function should print the remaining levels of the config 
 tree.
 And we want it to print on the format of
 [[courses.datintro22.url = https://...]].
 This function will do a depth-first traversal through the config to print all 
 values.
+The idea is that the config path will move from the dictionary representation 
+in [[conf]] to the string representation in [[path]].
+When at the leaf, [[conf]] will contain the value and [[path]] the entire path.
 <<helper functions>>=
 def print_config(conf, path=""):
   """
   Prints the config tree contained in `conf` to stdout.
   Optional `path` is prepended.
   """
   try:
     for key in conf.keys():
-      if path:
-        print_config(conf[key], f"{path}.{key}")
-      else:
-        print_config(conf[key], key)
-  except AttributeError:
-    print(f"{path} = {conf}")
+      <<recurse deeper into the config tree>>
+  <<print the leaf of config tree and return>>
 @
+
+The recursive step is quite straight-forward, we just call [[print_config]] 
+with the subtree ([[conf[key]]]) as an argument.
+However, we must check whether to prepend anything ([[path]]).
+The deeper we progress, the more we want to prepend.
+For instance, at the [[courses.datintro22]] level, [[print_config]] only knows 
+[[datintro22]], not the [[courses]] parent.
+Hence, we must supply [[courses]] to prepend to [[datintro22]] to get 
+[[courses.datintro22]].
+<<recurse deeper into the config tree>>=
+if path:
+  print_config(conf[key], f"{path}.{key}")
+else:
+  print_config(conf[key], key)
+@
+
+Finally, we get the base-case by exception.
+When a node ([[conf]]) doesn't have an attribute [[.keys()]], we know we're at 
+a leaf, so we print it.
+Then the complete path is in [[path]], the value in [[conf]].
+<<print the leaf of config tree and return>>=
+except AttributeError:
+  print(f"{path} = {conf}")
+
```

### Comparing `typerconf-1.4/PKG-INFO` & `typerconf-1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typerconf
-Version: 1.4
+Version: 1.5
 Summary: Library to read and write configs using API and CLI with Typer
 Home-page: https://github.com/dbosk/typerconf
 License: MIT
 Keywords: typer,conf,config,git-like,config lib,write conf
 Author: Daniel Bosk
 Author-email: daniel@bosk.se
 Requires-Python: >=3.7,<4.0
```

