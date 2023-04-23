# Comparing `tmp/jit_env-0.1.1.tar.gz` & `tmp/jit_env-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/jit_env-0.1.1.tar", last modified: Thu Apr 13 07:54:52 2023, max compression
+gzip compressed data, was "dist/jit_env-0.1.2.tar", last modified: Sun Apr 23 09:51:22 2023, max compression
```

## Comparing `jit_env-0.1.1.tar` & `jit_env-0.1.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0 joery     (1000) joery     (1000)        0 2023-04-13 07:54:52.745051 jit_env-0.1.1/
--rwxrwxrwx   0 joery     (1000) joery     (1000)     1062 2023-04-07 11:59:34.000000 jit_env-0.1.1/LICENSE
--rwxrwxrwx   0 joery     (1000) joery     (1000)       29 2023-04-10 08:18:00.000000 jit_env-0.1.1/MANIFEST.in
--rwxrwxrwx   0 joery     (1000) joery     (1000)     5523 2023-04-13 07:54:52.745051 jit_env-0.1.1/PKG-INFO
--rwxrwxrwx   0 joery     (1000) joery     (1000)     4739 2023-04-11 07:42:07.000000 jit_env-0.1.1/README.md
-drwxrwxrwx   0 joery     (1000) joery     (1000)        0 2023-04-13 07:54:52.650741 jit_env-0.1.1/jit_env/
--rwxrwxrwx   0 joery     (1000) joery     (1000)     1057 2023-04-07 09:34:23.000000 jit_env-0.1.1/jit_env/__init__.py
--rwxrwxrwx   0 joery     (1000) joery     (1000)     4215 2023-04-11 07:18:45.000000 jit_env-0.1.1/jit_env/_compat_test.py
--rwxrwxrwx   0 joery     (1000) joery     (1000)    13759 2023-04-13 07:54:10.000000 jit_env-0.1.1/jit_env/_core.py
--rwxrwxrwx   0 joery     (1000) joery     (1000)     9289 2023-04-11 07:13:02.000000 jit_env-0.1.1/jit_env/_core_test.py
--rwxrwxrwx   0 joery     (1000) joery     (1000)    16484 2023-04-10 12:51:38.000000 jit_env-0.1.1/jit_env/_specs_test.py
--rwxrwxrwx   0 joery     (1000) joery     (1000)    13284 2023-04-13 07:54:10.000000 jit_env-0.1.1/jit_env/_wrappers_test.py
--rwxrwxrwx   0 joery     (1000) joery     (1000)     4532 2023-04-11 07:17:00.000000 jit_env-0.1.1/jit_env/compat.py
--rwxrwxrwx   0 joery     (1000) joery     (1000)        0 2023-04-13 07:54:10.000000 jit_env-0.1.1/jit_env/py.typed
--rwxrwxrwx   0 joery     (1000) joery     (1000)    23230 2023-04-10 13:11:26.000000 jit_env-0.1.1/jit_env/specs.py
--rwxrwxrwx   0 joery     (1000) joery     (1000)      304 2023-04-13 07:54:46.000000 jit_env-0.1.1/jit_env/version.py
--rwxrwxrwx   0 joery     (1000) joery     (1000)    14216 2023-04-13 07:54:10.000000 jit_env-0.1.1/jit_env/wrappers.py
-drwxrwxrwx   0 joery     (1000) joery     (1000)        0 2023-04-13 07:54:52.737495 jit_env-0.1.1/jit_env.egg-info/
--rwxrwxrwx   0 joery     (1000) joery     (1000)     5523 2023-04-13 07:54:51.000000 jit_env-0.1.1/jit_env.egg-info/PKG-INFO
--rwxrwxrwx   0 joery     (1000) joery     (1000)      453 2023-04-13 07:54:52.000000 jit_env-0.1.1/jit_env.egg-info/SOURCES.txt
--rwxrwxrwx   0 joery     (1000) joery     (1000)        1 2023-04-13 07:54:51.000000 jit_env-0.1.1/jit_env.egg-info/dependency_links.txt
--rwxrwxrwx   0 joery     (1000) joery     (1000)      157 2023-04-13 07:54:51.000000 jit_env-0.1.1/jit_env.egg-info/requires.txt
--rwxrwxrwx   0 joery     (1000) joery     (1000)        8 2023-04-13 07:54:51.000000 jit_env-0.1.1/jit_env.egg-info/top_level.txt
--rwxrwxrwx   0 joery     (1000) joery     (1000)       44 2023-04-08 05:46:44.000000 jit_env-0.1.1/requirements.txt
--rwxrwxrwx   0 joery     (1000) joery     (1000)      115 2023-04-10 08:18:00.000000 jit_env-0.1.1/requirements_dev.txt
--rwxrwxrwx   0 joery     (1000) joery     (1000)       38 2023-04-13 07:54:52.745051 jit_env-0.1.1/setup.cfg
--rwxrwxrwx   0 joery     (1000) joery     (1000)     1835 2023-04-13 07:54:10.000000 jit_env-0.1.1/setup.py
+drwxrwxrwx   0 joery     (1000) joery     (1000)        0 2023-04-23 09:51:22.969188 jit_env-0.1.2/
+-rwxrwxrwx   0 joery     (1000) joery     (1000)     1062 2023-04-07 11:59:34.000000 jit_env-0.1.2/LICENSE
+-rwxrwxrwx   0 joery     (1000) joery     (1000)       29 2023-04-10 08:18:00.000000 jit_env-0.1.2/MANIFEST.in
+-rwxrwxrwx   0 joery     (1000) joery     (1000)     5523 2023-04-23 09:51:22.962867 jit_env-0.1.2/PKG-INFO
+-rwxrwxrwx   0 joery     (1000) joery     (1000)     4739 2023-04-23 09:50:06.000000 jit_env-0.1.2/README.md
+drwxrwxrwx   0 joery     (1000) joery     (1000)        0 2023-04-23 09:51:22.676900 jit_env-0.1.2/jit_env/
+-rwxrwxrwx   0 joery     (1000) joery     (1000)     1057 2023-04-07 09:34:23.000000 jit_env-0.1.2/jit_env/__init__.py
+-rwxrwxrwx   0 joery     (1000) joery     (1000)     4215 2023-04-11 07:18:45.000000 jit_env-0.1.2/jit_env/_compat_test.py
+-rwxrwxrwx   0 joery     (1000) joery     (1000)    14702 2023-04-15 05:34:34.000000 jit_env-0.1.2/jit_env/_core.py
+-rwxrwxrwx   0 joery     (1000) joery     (1000)     9289 2023-04-11 07:13:02.000000 jit_env-0.1.2/jit_env/_core_test.py
+-rwxrwxrwx   0 joery     (1000) joery     (1000)    16484 2023-04-10 12:51:38.000000 jit_env-0.1.2/jit_env/_specs_test.py
+-rwxrwxrwx   0 joery     (1000) joery     (1000)    13301 2023-04-15 05:34:34.000000 jit_env-0.1.2/jit_env/_wrappers_test.py
+-rwxrwxrwx   0 joery     (1000) joery     (1000)     4532 2023-04-11 07:17:00.000000 jit_env-0.1.2/jit_env/compat.py
+-rwxrwxrwx   0 joery     (1000) joery     (1000)        0 2023-04-13 07:54:10.000000 jit_env-0.1.2/jit_env/py.typed
+-rwxrwxrwx   0 joery     (1000) joery     (1000)    23230 2023-04-10 13:11:26.000000 jit_env-0.1.2/jit_env/specs.py
+-rwxrwxrwx   0 joery     (1000) joery     (1000)      304 2023-04-23 09:50:06.000000 jit_env-0.1.2/jit_env/version.py
+-rwxrwxrwx   0 joery     (1000) joery     (1000)    14216 2023-04-13 07:54:10.000000 jit_env-0.1.2/jit_env/wrappers.py
+drwxrwxrwx   0 joery     (1000) joery     (1000)        0 2023-04-23 09:51:22.902842 jit_env-0.1.2/jit_env.egg-info/
+-rwxrwxrwx   0 joery     (1000) joery     (1000)     5523 2023-04-23 09:51:20.000000 jit_env-0.1.2/jit_env.egg-info/PKG-INFO
+-rwxrwxrwx   0 joery     (1000) joery     (1000)      453 2023-04-23 09:51:20.000000 jit_env-0.1.2/jit_env.egg-info/SOURCES.txt
+-rwxrwxrwx   0 joery     (1000) joery     (1000)        1 2023-04-23 09:51:20.000000 jit_env-0.1.2/jit_env.egg-info/dependency_links.txt
+-rwxrwxrwx   0 joery     (1000) joery     (1000)      157 2023-04-23 09:51:20.000000 jit_env-0.1.2/jit_env.egg-info/requires.txt
+-rwxrwxrwx   0 joery     (1000) joery     (1000)        8 2023-04-23 09:51:20.000000 jit_env-0.1.2/jit_env.egg-info/top_level.txt
+-rwxrwxrwx   0 joery     (1000) joery     (1000)       44 2023-04-08 05:46:44.000000 jit_env-0.1.2/requirements.txt
+-rwxrwxrwx   0 joery     (1000) joery     (1000)      115 2023-04-10 08:18:00.000000 jit_env-0.1.2/requirements_dev.txt
+-rwxrwxrwx   0 joery     (1000) joery     (1000)       38 2023-04-23 09:51:22.972656 jit_env-0.1.2/setup.cfg
+-rwxrwxrwx   0 joery     (1000) joery     (1000)     1835 2023-04-13 07:54:10.000000 jit_env-0.1.2/setup.py
```

### Comparing `jit_env-0.1.1/LICENSE` & `jit_env-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jit_env-0.1.1/PKG-INFO` & `jit_env-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jit_env
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Jax interface for Reinforcement Learning environments.
 Home-page: https://github.com/joeryjoery/jit_env
 Author: Joery A. de Vries
 Author-email: J.A.deVries@tudelft.nl
 License: MIT
 Keywords: reinforcement-learning python machine learning jax
 Classifier: Operating System :: OS Independent
@@ -17,15 +17,15 @@
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 ![Run Tox Tests](https://github.com/joeryjoery/jit_env/actions/workflows/tests.yml/badge.svg)
 ![Python Version](https://img.shields.io/badge/Python-3.9%20%7C%203.10%20%7C%203.11-blue)
-![Package Version](https://img.shields.io/badge/jit__env-0.1.0-blue)
+![Package Version](https://img.shields.io/badge/jit__env-0.1.2-blue)
 # `jit_env`: A Jax Compatible RL Environment API
 `jit_env` is a library that aims to adhere closely to the `dm_env` interface
 while allowing for `jax` transformations inside Environment implementations
 and defining clear type annotations.
 
 Like `dm_env` our API consists of the main components:
```

### Comparing `jit_env-0.1.1/README.md` & `jit_env-0.1.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ![Run Tox Tests](https://github.com/joeryjoery/jit_env/actions/workflows/tests.yml/badge.svg)
 ![Python Version](https://img.shields.io/badge/Python-3.9%20%7C%203.10%20%7C%203.11-blue)
-![Package Version](https://img.shields.io/badge/jit__env-0.1.0-blue)
+![Package Version](https://img.shields.io/badge/jit__env-0.1.2-blue)
 # `jit_env`: A Jax Compatible RL Environment API
 `jit_env` is a library that aims to adhere closely to the `dm_env` interface
 while allowing for `jax` transformations inside Environment implementations
 and defining clear type annotations.
 
 Like `dm_env` our API consists of the main components:
```

### Comparing `jit_env-0.1.1/jit_env/__init__.py` & `jit_env-0.1.2/jit_env/__init__.py`

 * *Files identical despite different names*

### Comparing `jit_env-0.1.1/jit_env/_compat_test.py` & `jit_env-0.1.2/jit_env/_compat_test.py`

 * *Files identical despite different names*

### Comparing `jit_env-0.1.1/jit_env/_core.py` & `jit_env-0.1.2/jit_env/_core.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,17 @@
     - An interface for defining Environment Logic
     - An interface for composing Environment Logic
     - Helper functions to initialize Types communicated to the Agent.
 """
 from __future__ import annotations
 import abc
 
-from typing import Any, TYPE_CHECKING, TypeVar, Generic, Sequence, Protocol
+from typing import (
+    Any, TYPE_CHECKING, TypeVar, Generic, Sequence, Protocol, Callable
+)
 from dataclasses import field
 
 if TYPE_CHECKING:  # pragma: no cover
     # See: https://github.com/python/mypy/issues/6239
     from dataclasses import dataclass
 else:
     from chex import dataclass
@@ -104,14 +106,31 @@
 
 
 # Define Environment and Wrapper
 
 class Environment(Generic[State, Action, Observation], metaclass=abc.ABCMeta):
     """Interface for defining Environment logic for RL-Agents. """
 
+    def __init__(self, *, renderer: Callable[[State], Any] | None = None):
+        """
+        Initializes the Environment by optionally providing a renderer.
+
+        The renderer should be separated from the Environment logic itself
+        to reduce coupling. The Agent's behaviour should not depend
+        on rendered images, this is to provide a visualization for the user.
+
+        Args:
+            renderer:
+                A callable from States to a visually rendered object of State.
+                The visuals are for the user, and not the agent. If renderer
+                is None, then calling Environment.render will raise a
+                NotImplementedError.
+        """
+        self._renderer = renderer
+
     def __str__(self) -> str:
         """Returns a minimal representation of the Environment Structure."""
         return self.__class__.__name__
 
     def __repr__(self) -> str:
         """Returns a complete informative representation of self.
 
@@ -226,28 +245,30 @@
             with Env(...) as env:
               # Use env.
         """
 
     def render(self, state: State) -> Any:
         """Generate a pixel-observation based on the given state.
 
-        This method is not annotated as abstract as implementing a render
-        is not neccesary to perform experiments. However it will raise
-        an Error if called without an implementation.
+        To support rendering environments, this should be provided within
+        the Environment's constructor. Otherwise, calling this function
+        will raise a NotImplementedError.
 
         Args:
             state: A state object to generate a visualization of.
 
         Raises:
             NotImplementedError:
-                If subclass does not implement this method.
-         """
-        raise NotImplementedError(  # pragma: no cover
-            "Render Function not Implemented"
-        )
+                If no renderer is provided to Environment.
+        """
+        if self._renderer is None:
+            raise NotImplementedError(  # pragma: no cover
+                "Render Function not Implemented"
+            )
+        return self._renderer(state)
 
     def __enter__(self) -> Environment:
         """Allows the environment to be used in a with-statement context."""
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         """Allows the environment to be used in a with-statement context."""
@@ -258,24 +279,27 @@
 class Wrapper(
     Environment[State, Action, Observation],
     Generic[State, Action, Observation],
     metaclass=abc.ABCMeta
 ):
     """Interface for Composing Environment logic for RL-Agents. """
 
-    def __init__(self, env: Environment):
+    def __init__(self, env: Environment, *args, **kwargs):
         """Initializes the Composite Environment with a base Environment.
 
         The `env` attribute can be accessed for reading out attributes, but it
         should not be modified.
 
         Args:
             env: The base environment to extend with functionality.
+
+            args: See Environment
+            kwargs: See Environment
         """
-        super().__init__()
+        super().__init__(*args, **kwargs)
         self._env = env
 
     def __str__(self) -> str:
         """Returns a recursive composition structure of all Wrappers."""
         return f"{self.__class__.__name__}({str(self.env)})"
 
     def __repr__(self) -> str:
```

### Comparing `jit_env-0.1.1/jit_env/_core_test.py` & `jit_env-0.1.2/jit_env/_core_test.py`

 * *Files identical despite different names*

### Comparing `jit_env-0.1.1/jit_env/_specs_test.py` & `jit_env-0.1.2/jit_env/_specs_test.py`

 * *Files identical despite different names*

### Comparing `jit_env-0.1.1/jit_env/_wrappers_test.py` & `jit_env-0.1.2/jit_env/_wrappers_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import jit_env
 from jit_env import wrappers, specs
 
 
 class TestRepr:
 
     def test_empty(self, dummy_env: jit_env.Environment):
-        wrapped = jit_env.Wrapper(dummy_env)
+        wrapped: jit_env.Wrapper = jit_env.Wrapper(dummy_env)
 
         assert str(wrapped) == f'{wrapped.__class__.__name__}(' \
                                f'{dummy_env.__class__.__name__})'
         assert repr(wrapped) == f'{wrapped.__class__.__name__}(' \
                                 f'env={dummy_env.__class__.__name__})'
 
     @pytest.mark.usefixtures('dummy_env')
```

### Comparing `jit_env-0.1.1/jit_env/compat.py` & `jit_env-0.1.2/jit_env/compat.py`

 * *Files identical despite different names*

### Comparing `jit_env-0.1.1/jit_env/specs.py` & `jit_env-0.1.2/jit_env/specs.py`

 * *Files identical despite different names*

### Comparing `jit_env-0.1.1/jit_env/wrappers.py` & `jit_env-0.1.2/jit_env/wrappers.py`

 * *Files identical despite different names*

### Comparing `jit_env-0.1.1/jit_env.egg-info/PKG-INFO` & `jit_env-0.1.2/jit_env.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jit-env
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Jax interface for Reinforcement Learning environments.
 Home-page: https://github.com/joeryjoery/jit_env
 Author: Joery A. de Vries
 Author-email: J.A.deVries@tudelft.nl
 License: MIT
 Keywords: reinforcement-learning python machine learning jax
 Classifier: Operating System :: OS Independent
@@ -17,15 +17,15 @@
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 ![Run Tox Tests](https://github.com/joeryjoery/jit_env/actions/workflows/tests.yml/badge.svg)
 ![Python Version](https://img.shields.io/badge/Python-3.9%20%7C%203.10%20%7C%203.11-blue)
-![Package Version](https://img.shields.io/badge/jit__env-0.1.0-blue)
+![Package Version](https://img.shields.io/badge/jit__env-0.1.2-blue)
 # `jit_env`: A Jax Compatible RL Environment API
 `jit_env` is a library that aims to adhere closely to the `dm_env` interface
 while allowing for `jax` transformations inside Environment implementations
 and defining clear type annotations.
 
 Like `dm_env` our API consists of the main components:
```

### Comparing `jit_env-0.1.1/setup.py` & `jit_env-0.1.2/setup.py`

 * *Files identical despite different names*

