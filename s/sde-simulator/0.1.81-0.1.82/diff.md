# Comparing `tmp/sde_simulator-0.1.81.tar.gz` & `tmp/sde_simulator-0.1.82.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sde_simulator-0.1.81.tar", last modified: Wed Mar  1 06:56:02 2023, max compression
+gzip compressed data, was "sde_simulator-0.1.82.tar", last modified: Sun Apr 23 11:13:54 2023, max compression
```

## Comparing `sde_simulator-0.1.81.tar` & `sde_simulator-0.1.82.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0 odedwer   (1000) odedwer   (1000)        0 2023-03-01 06:56:02.668467 sde_simulator-0.1.81/
--rwxrwxrwx   0 odedwer   (1000) odedwer   (1000)      809 2023-03-01 06:56:02.668467 sde_simulator-0.1.81/PKG-INFO
--rwxrwxrwx   0 odedwer   (1000) odedwer   (1000)      338 2022-12-25 10:46:48.000000 sde_simulator-0.1.81/README.md
-drwxrwxrwx   0 odedwer   (1000) odedwer   (1000)        0 2023-03-01 06:56:02.636833 sde_simulator-0.1.81/sde_simulator/
--rwxrwxrwx   0 odedwer   (1000) odedwer   (1000)       28 2022-12-25 11:10:17.000000 sde_simulator-0.1.81/sde_simulator/__init__.py
--rwxrwxrwx   0 odedwer   (1000) odedwer   (1000)     3571 2023-03-01 06:55:39.000000 sde_simulator-0.1.81/sde_simulator/sde_simulator.py
-drwxrwxrwx   0 odedwer   (1000) odedwer   (1000)        0 2023-03-01 06:56:02.668467 sde_simulator-0.1.81/sde_simulator.egg-info/
--rwxrwxrwx   0 odedwer   (1000) odedwer   (1000)      809 2023-03-01 06:56:02.000000 sde_simulator-0.1.81/sde_simulator.egg-info/PKG-INFO
--rwxrwxrwx   0 odedwer   (1000) odedwer   (1000)      259 2023-03-01 06:56:02.000000 sde_simulator-0.1.81/sde_simulator.egg-info/SOURCES.txt
--rwxrwxrwx   0 odedwer   (1000) odedwer   (1000)        1 2023-03-01 06:56:02.000000 sde_simulator-0.1.81/sde_simulator.egg-info/dependency_links.txt
--rwxrwxrwx   0 odedwer   (1000) odedwer   (1000)       11 2023-03-01 06:56:02.000000 sde_simulator-0.1.81/sde_simulator.egg-info/requires.txt
--rwxrwxrwx   0 odedwer   (1000) odedwer   (1000)       14 2023-03-01 06:56:02.000000 sde_simulator-0.1.81/sde_simulator.egg-info/top_level.txt
--rwxrwxrwx   0 odedwer   (1000) odedwer   (1000)       38 2023-03-01 06:56:02.668467 sde_simulator-0.1.81/setup.cfg
--rwxrwxrwx   0 odedwer   (1000) odedwer   (1000)     1028 2023-03-01 06:55:39.000000 sde_simulator-0.1.81/setup.py
+drwxrwxrwx   0 odedwer   (1000) odedwer   (1000)        0 2023-04-23 11:13:54.231567 sde_simulator-0.1.82/
+-rwxrwxrwx   0 odedwer   (1000) odedwer   (1000)      809 2023-04-23 11:13:54.230616 sde_simulator-0.1.82/PKG-INFO
+-rwxrwxrwx   0 odedwer   (1000) odedwer   (1000)      338 2022-12-25 10:46:48.000000 sde_simulator-0.1.82/README.md
+drwxrwxrwx   0 odedwer   (1000) odedwer   (1000)        0 2023-04-23 11:13:54.219382 sde_simulator-0.1.82/sde_simulator/
+-rwxrwxrwx   0 odedwer   (1000) odedwer   (1000)       28 2022-12-25 11:10:17.000000 sde_simulator-0.1.82/sde_simulator/__init__.py
+-rwxrwxrwx   0 odedwer   (1000) odedwer   (1000)     3612 2023-04-23 11:12:56.000000 sde_simulator-0.1.82/sde_simulator/sde_simulator.py
+drwxrwxrwx   0 odedwer   (1000) odedwer   (1000)        0 2023-04-23 11:13:54.228615 sde_simulator-0.1.82/sde_simulator.egg-info/
+-rwxrwxrwx   0 odedwer   (1000) odedwer   (1000)      809 2023-04-23 11:13:54.000000 sde_simulator-0.1.82/sde_simulator.egg-info/PKG-INFO
+-rwxrwxrwx   0 odedwer   (1000) odedwer   (1000)      259 2023-04-23 11:13:54.000000 sde_simulator-0.1.82/sde_simulator.egg-info/SOURCES.txt
+-rwxrwxrwx   0 odedwer   (1000) odedwer   (1000)        1 2023-04-23 11:13:54.000000 sde_simulator-0.1.82/sde_simulator.egg-info/dependency_links.txt
+-rwxrwxrwx   0 odedwer   (1000) odedwer   (1000)       11 2023-04-23 11:13:54.000000 sde_simulator-0.1.82/sde_simulator.egg-info/requires.txt
+-rwxrwxrwx   0 odedwer   (1000) odedwer   (1000)       14 2023-04-23 11:13:54.000000 sde_simulator-0.1.82/sde_simulator.egg-info/top_level.txt
+-rwxrwxrwx   0 odedwer   (1000) odedwer   (1000)       38 2023-04-23 11:13:54.231567 sde_simulator-0.1.82/setup.cfg
+-rwxrwxrwx   0 odedwer   (1000) odedwer   (1000)     1028 2023-04-23 11:12:56.000000 sde_simulator-0.1.82/setup.py
```

### Comparing `sde_simulator-0.1.81/PKG-INFO` & `sde_simulator-0.1.82/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sde_simulator
-Version: 0.1.81
+Version: 0.1.82
 Summary: General base class implementation of Rung-Kutta SDE solver
 Home-page: https://github.com/odedwer/sde_simulator
 Author: Oded Wertheimer
 Author-email: oded.wertheimer@mail.huji.ac.il
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sde_simulator-0.1.81/sde_simulator/sde_simulator.py` & `sde_simulator-0.1.82/sde_simulator/sde_simulator.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     """
     This is a base class for dynamic models, implementing a stochastic Rung-Kutta solver:
     y(t+1) = y(t) + a(y(t))*dt + b(y(t))*dW + 0.5*(b(y(t) + a(y(t)*dt + b(y(t)*sqrt(dt)) - b(Y(t))*(dW^2 - dt)/sqrt(dt)
     """
 
     @abstractmethod
     def __init__(self, y0: npt.NDArray, tau: [float, int] = 1., max_t: [float, int] = 1., dt: float = 1e-2,
-                 noise: float = 0., n_sim: int = 10000, verbose: bool = True):
+                 noise: float = 0., n_sim: int = 10000, verbose: bool = True, **kwargs):
         """
         @param y0: Iterable convertible to numpy array. The initial value of the simulation variables.
                    Should be 1D of size #variables.
         @param tau: integer/float. The time constant of the simulation.
         @param max_t: integer/float. Determines the number of steps in the simulation together with dt.
         @param dt: float. The time between two steps in the simulation.
         @param noise: float. The standard deviation of the Wiener process
@@ -32,18 +32,19 @@
         self._time = np.arange(0, max_t + self._dt, self._dt)
         self._sqrtdt = np.sqrt(self._dt)
         # shape of (time, # variables, # simulations)
         self._y = np.zeros(self.time.shape + self.y0.shape + (n_sim,), dtype=float)
         self._y[0, :, :] = self._y0[:, None]
         self.print_str("generating noise sequences...")
         self._noise = noise
-        self._generated_dw = np.random.normal(loc=0.0, scale=noise*self.sqrtdt, size=self.y.shape)
+        self._generated_dw = np.random.normal(loc=0.0, scale=noise * self.sqrtdt, size=self.y.shape)
         self._generated_dw_squared = self._generated_dw ** 2
         self._simulated = False
         self._simulation_kwargs = dict()
+        self.kwargs = kwargs
 
     def print_str(self, string):
         if self._verbose:
             print(string)
 
     @property
     def y0(self):
```

### Comparing `sde_simulator-0.1.81/sde_simulator.egg-info/PKG-INFO` & `sde_simulator-0.1.82/sde_simulator.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sde-simulator
-Version: 0.1.81
+Version: 0.1.82
 Summary: General base class implementation of Rung-Kutta SDE solver
 Home-page: https://github.com/odedwer/sde_simulator
 Author: Oded Wertheimer
 Author-email: oded.wertheimer@mail.huji.ac.il
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sde_simulator-0.1.81/setup.py` & `sde_simulator-0.1.82/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='sde_simulator',
-    version='0.1.81',
+    version='0.1.82',
     description="General base class implementation of Rung-Kutta SDE solver",
     long_description="This package provides a base class for simulating SDE using Rung-Kutta method.\n"
                      "The base class implements the simulation and requires the override of the deterministic and "
                      "stochastic methods of the model.",
     author="Oded Wertheimer",
     author_email="oded.wertheimer@mail.huji.ac.il",
     packages=["sde_simulator"],
```

