# Comparing `tmp/chanfig-0.0.9.post5.tar.gz` & `tmp/chanfig-0.0.9.post7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chanfig-0.0.9.post5.tar", last modified: Mon May 16 11:25:24 2022, max compression
+gzip compressed data, was "chanfig-0.0.9.post7.tar", last modified: Tue May 17 07:58:17 2022, max compression
```

## Comparing `chanfig-0.0.9.post5.tar` & `chanfig-0.0.9.post7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 v-zhichen  (1000) v-zhichen  (1000)        0 2022-05-16 11:25:24.131473 chanfig-0.0.9.post5/
--rw-rw-r--   0 v-zhichen  (1000) v-zhichen  (1000)       58 2022-05-12 09:54:50.000000 chanfig-0.0.9.post5/LICENSE
--rw-rw-r--   0 v-zhichen  (1000) v-zhichen  (1000)      248 2022-05-16 11:25:24.131473 chanfig-0.0.9.post5/PKG-INFO
--rw-rw-r--   0 v-zhichen  (1000) v-zhichen  (1000)     3662 2022-05-05 11:07:08.000000 chanfig-0.0.9.post5/README.md
-drwxrwxr-x   0 v-zhichen  (1000) v-zhichen  (1000)        0 2022-05-16 11:25:24.131473 chanfig-0.0.9.post5/chanfig/
--rw-rw-r--   0 v-zhichen  (1000) v-zhichen  (1000)       79 2022-05-12 12:26:14.000000 chanfig-0.0.9.post5/chanfig/__init__.py
--rw-rw-r--   0 v-zhichen  (1000) v-zhichen  (1000)    10329 2022-05-16 11:24:18.000000 chanfig-0.0.9.post5/chanfig/config.py
-drwxrwxr-x   0 v-zhichen  (1000) v-zhichen  (1000)        0 2022-05-16 11:25:24.131473 chanfig-0.0.9.post5/chanfig.egg-info/
--rw-rw-r--   0 v-zhichen  (1000) v-zhichen  (1000)      248 2022-05-16 11:25:23.000000 chanfig-0.0.9.post5/chanfig.egg-info/PKG-INFO
--rw-rw-r--   0 v-zhichen  (1000) v-zhichen  (1000)      188 2022-05-16 11:25:23.000000 chanfig-0.0.9.post5/chanfig.egg-info/SOURCES.txt
--rw-rw-r--   0 v-zhichen  (1000) v-zhichen  (1000)        1 2022-05-16 11:25:23.000000 chanfig-0.0.9.post5/chanfig.egg-info/dependency_links.txt
--rw-rw-r--   0 v-zhichen  (1000) v-zhichen  (1000)        8 2022-05-16 11:25:23.000000 chanfig-0.0.9.post5/chanfig.egg-info/top_level.txt
--rw-rw-r--   0 v-zhichen  (1000) v-zhichen  (1000)       38 2022-05-16 11:25:24.131473 chanfig-0.0.9.post5/setup.cfg
--rw-rw-r--   0 v-zhichen  (1000) v-zhichen  (1000)      276 2022-05-16 11:24:27.000000 chanfig-0.0.9.post5/setup.py
+drwxrwxr-x   0 v-zhichen  (1000) v-zhichen  (1000)        0 2022-05-17 07:58:17.802893 chanfig-0.0.9.post7/
+-rw-rw-r--   0 v-zhichen  (1000) v-zhichen  (1000)       58 2022-05-12 09:54:50.000000 chanfig-0.0.9.post7/LICENSE
+-rw-rw-r--   0 v-zhichen  (1000) v-zhichen  (1000)      248 2022-05-17 07:58:17.802893 chanfig-0.0.9.post7/PKG-INFO
+-rw-rw-r--   0 v-zhichen  (1000) v-zhichen  (1000)     3662 2022-05-05 11:07:08.000000 chanfig-0.0.9.post7/README.md
+drwxrwxr-x   0 v-zhichen  (1000) v-zhichen  (1000)        0 2022-05-17 07:58:17.802893 chanfig-0.0.9.post7/chanfig/
+-rw-rw-r--   0 v-zhichen  (1000) v-zhichen  (1000)       79 2022-05-12 12:26:14.000000 chanfig-0.0.9.post7/chanfig/__init__.py
+-rw-rw-r--   0 v-zhichen  (1000) v-zhichen  (1000)    10810 2022-05-16 12:22:47.000000 chanfig-0.0.9.post7/chanfig/config.py
+drwxrwxr-x   0 v-zhichen  (1000) v-zhichen  (1000)        0 2022-05-17 07:58:17.802893 chanfig-0.0.9.post7/chanfig.egg-info/
+-rw-rw-r--   0 v-zhichen  (1000) v-zhichen  (1000)      248 2022-05-17 07:58:17.000000 chanfig-0.0.9.post7/chanfig.egg-info/PKG-INFO
+-rw-rw-r--   0 v-zhichen  (1000) v-zhichen  (1000)      188 2022-05-17 07:58:17.000000 chanfig-0.0.9.post7/chanfig.egg-info/SOURCES.txt
+-rw-rw-r--   0 v-zhichen  (1000) v-zhichen  (1000)        1 2022-05-17 07:58:17.000000 chanfig-0.0.9.post7/chanfig.egg-info/dependency_links.txt
+-rw-rw-r--   0 v-zhichen  (1000) v-zhichen  (1000)        8 2022-05-17 07:58:17.000000 chanfig-0.0.9.post7/chanfig.egg-info/top_level.txt
+-rw-rw-r--   0 v-zhichen  (1000) v-zhichen  (1000)       38 2022-05-17 07:58:17.802893 chanfig-0.0.9.post7/setup.cfg
+-rw-rw-r--   0 v-zhichen  (1000) v-zhichen  (1000)      276 2022-05-16 12:24:14.000000 chanfig-0.0.9.post7/setup.py
```

### Comparing `chanfig-0.0.9.post5/README.md` & `chanfig-0.0.9.post7/README.md`

 * *Files identical despite different names*

### Comparing `chanfig-0.0.9.post5/chanfig/config.py` & `chanfig-0.0.9.post7/chanfig/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,22 +29,46 @@
         return super().increase_indent(flow, False)
 
 
 class FileError(ValueError):
     pass
 
 
+class ConfigParser(ArgumentParser):
+    def parse(self, args: Iterable[str] = None, config: Config = None, config_name: str = 'config') -> Config:
+        if args is None:
+            args = sys.argv[1:]
+        for arg in args:
+            if arg.startswith('--') and args != '--' and arg not in self._option_string_actions:
+                self.add_argument(arg)
+        if config is None:
+            config = Config()
+        if (path := getattr(config, config_name, None)) is not None:
+            raise ValueError(f"--{config_name} is reserved for auto loading config file, but got {path}")
+        config, _ = self.parse_known_args(args, config)
+        if (path := getattr(config, config_name, None)) is not None:
+            config = config.update(path)
+        return config
+
+    parse_config = parse
+
+
 class Config(Namespace):
     """
     Basic Config
     """
 
     delimiter: str = '.'
     indent: int = 2
     frozen: bool = False
+    parser: ConfigParser = ConfigParser()
+
+    def __init__(self, **kwargs):
+        for key, value in kwargs.items():
+            self.set(key, value, convert_mapping=True)
 
     def __getattr__(self, name: str) -> Any:
         if self.delimiter in name:
             name, rest = name.split(self.delimiter, 1)
             return getattr(self[name], rest)
         else:
             return super().__getattribute__(name)
@@ -53,22 +77,24 @@
 
     def get(self, name: str, default: Optional[Any] = None) -> Any:
         try:
             return getattr(self, name)
         except AttributeError:
             return default
 
-    def set(self, name: str, value: Any) -> None:
+    def set(self, name: str, value: Any, convert_mapping: bool = False) -> None:
         if self.frozen:
             raise AttributeError(f"Attempting to set {name}={value} on a frozen config. Run config.defrost() to defrost first")
         if self.delimiter in name:
             name, rest = name.split(self.delimiter, 1)
             if not hasattr(self, name):
                 setattr(self, name, Config())
-            setattr(getattr(self, name), rest, value)
+            setattr(self[name], rest, value)
+        elif convert_mapping and isinstance(value, MutableMapping):
+            setattr(self, name, Config(**value))
         else:
             if isinstance(value, str):
                 try:
                     value = literal_eval(value)
                 except (ValueError, SyntaxError):
                     pass
             super().__setattr__(name, value)
@@ -144,15 +170,18 @@
         return dic
 
     def update(self, other: Union[str, Config, MutableMapping, Iterable], **kwargs) -> Config:
         if isinstance(other, str):
             other = self.load(other)
         if isinstance(other, (Config, MutableMapping)):
             for key, value in other.items():
-                self[key] = value
+                if isinstance(value, (Config, MutableMapping)) and isinstance(self[key], (Config, MutableMapping)):
+                    self[key].update(value)
+                else:
+                    self[key] = value
         elif isinstance(other, Iterable):
             for key, value in other:
                 self[key] = value
         for key, value in kwargs.items():
             self[key] = value
         return self
 
@@ -231,17 +260,17 @@
             raise FileError(f"method {method} should be in {JSON} or {YAML}")
 
     @classmethod
     def load(cls, path: str, **kwargs) -> Config:
         path = path.lower()
         with cls.open(path) as fp:
             if path.endswith(JSON):
-                config = cls(**json_load(fp, **kwargs))
+                config = cls.from_json(fp.read(), **kwargs)
             elif path.endswith(YAML):
-                config = cls.load(fp.read(), **kwargs)
+                config = cls.from_yaml(fp.read(), **kwargs)
             else:
                 raise FileError(f"file {path} should have extensions {JSON} or {YAML}")
         return config
 
     @staticmethod
     @contextmanager
     def open(file: File, *args, **kwargs):
@@ -253,16 +282,15 @@
                 file.close()
         elif isinstance(file, (IO, )):
             yield file
         else:
             raise ValueError(f"file {file} should be of type (str, os.PathLike) or (io.IOBase), but got {type(file)}")
 
     def parse(self) -> Config:
-        parser = ConfigParser()
-        return parser.parse_config(config=self)
+        return self.parser.parse_config(config=self)
 
     parse_config = parse
 
     def apply(self, func: Callable) -> Config:
         for value in self.__dict__.values():
             if isinstance(value, Config):
                 value.apply(func)
@@ -291,26 +319,7 @@
         return self.dict() == other.dict()
 
     def __bool__(self):
         return bool(self)
 
     def __str__(self) -> str:
         return self.yamls()
-
-
-class ConfigParser(ArgumentParser):
-    def parse(self, args: Iterable[str] = None, config: Config = None, config_name: str = 'config') -> Config:
-        if args is None:
-            args = sys.argv[1:]
-        for arg in args:
-            if arg.startswith('--') and args != '--' and arg not in self._option_string_actions:
-                self.add_argument(arg)
-        if config is None:
-            config = Config()
-        if (path := getattr(config, config_name, None)) is not None:
-            raise ValueError(f"--{config_name} is reserved for auto loading config file, but got {path}")
-        config, _ = self.parse_known_args(args, config)
-        if (path := getattr(config, config_name, None)) is not None:
-            config = config.update(path)
-        return config
-
-    parse_config = parse
```

