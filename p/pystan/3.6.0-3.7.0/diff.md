# Comparing `tmp/pystan-3.6.0.tar.gz` & `tmp/pystan-3.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pystan-3.6.0.tar", max compression
+gzip compressed data, was "pystan-3.7.0.tar", max compression
```

## Comparing `pystan-3.6.0.tar` & `pystan-3.7.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      749 2022-11-26 14:13:07.013835 pystan-3.6.0/LICENSE
--rw-r--r--   0        0        0     2708 2022-11-26 14:13:07.013835 pystan-3.6.0/README.rst
--rw-r--r--   0        0        0     1294 2022-11-26 14:13:07.017835 pystan-3.6.0/pyproject.toml
--rw-r--r--   0        0        0      160 2022-11-26 14:13:07.017835 pystan-3.6.0/stan/__init__.py
--rw-r--r--   0        0        0     1748 2022-11-26 14:13:07.017835 pystan-3.6.0/stan/common.py
--rw-r--r--   0        0        0    10014 2022-11-26 14:13:07.017835 pystan-3.6.0/stan/fit.py
--rw-r--r--   0        0        0    23351 2022-11-26 14:13:07.017835 pystan-3.6.0/stan/model.py
--rw-r--r--   0        0        0     1353 2022-11-26 14:13:07.017835 pystan-3.6.0/stan/plugins.py
--rw-r--r--   0        0        0     3550 2022-11-26 14:13:21.542238 pystan-3.6.0/setup.py
--rw-r--r--   0        0        0     3668 2022-11-26 14:13:21.542851 pystan-3.6.0/PKG-INFO
+-rw-r--r--   0        0        0      749 2023-04-23 19:40:14.273918 pystan-3.7.0/LICENSE
+-rw-r--r--   0        0        0     2708 2023-04-23 19:40:14.273918 pystan-3.7.0/README.rst
+-rw-r--r--   0        0        0     1295 2023-04-23 19:40:14.273918 pystan-3.7.0/pyproject.toml
+-rw-r--r--   0        0        0      160 2023-04-23 19:40:14.273918 pystan-3.7.0/stan/__init__.py
+-rw-r--r--   0        0        0     1748 2023-04-23 19:40:14.273918 pystan-3.7.0/stan/common.py
+-rw-r--r--   0        0        0    10014 2023-04-23 19:40:14.273918 pystan-3.7.0/stan/fit.py
+-rw-r--r--   0        0        0    23351 2023-04-23 19:40:14.273918 pystan-3.7.0/stan/model.py
+-rw-r--r--   0        0        0     1353 2023-04-23 19:40:14.273918 pystan-3.7.0/stan/plugins.py
+-rw-r--r--   0        0        0     3551 2023-04-23 19:40:27.615259 pystan-3.7.0/setup.py
+-rw-r--r--   0        0        0     3669 2023-04-23 19:40:27.615846 pystan-3.7.0/PKG-INFO
```

### Comparing `pystan-3.6.0/LICENSE` & `pystan-3.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pystan-3.6.0/README.rst` & `pystan-3.7.0/README.rst`

 * *Files identical despite different names*

### Comparing `pystan-3.6.0/pyproject.toml` & `pystan-3.7.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pystan"
-version = "3.6.0"
+version = "3.7.0"
 description = "Python interface to Stan, a package for Bayesian inference"
 authors = [
   "Allen Riddell <riddella@indiana.edu>",
   "Ari Hartikainen <ahartikainen@users.noreply.github.com>",
   "Matthew Carter <m.j.carter2@liverpool.ac.uk>",
 ]
 license = "ISC"
@@ -20,15 +20,15 @@
   "Intended Audience :: Science/Research",
   "License :: OSI Approved :: ISC License (ISCL)",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 aiohttp = "^3.6"
-httpstan = "~4.9"
+httpstan = "~4.10"
 pysimdjson = "^5.0.2"
 numpy = "^1.19"
 clikit = "^0.6"
 setuptools = "*"
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.2"
```

### Comparing `pystan-3.6.0/stan/common.py` & `pystan-3.7.0/stan/common.py`

 * *Files identical despite different names*

### Comparing `pystan-3.6.0/stan/fit.py` & `pystan-3.7.0/stan/fit.py`

 * *Files identical despite different names*

### Comparing `pystan-3.6.0/stan/model.py` & `pystan-3.7.0/stan/model.py`

 * *Files identical despite different names*

### Comparing `pystan-3.6.0/stan/plugins.py` & `pystan-3.7.0/stan/plugins.py`

 * *Files identical despite different names*

### Comparing `pystan-3.6.0/setup.py` & `pystan-3.7.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['aiohttp>=3.6,<4.0',
  'clikit>=0.6,<0.7',
- 'httpstan>=4.9,<4.10',
+ 'httpstan>=4.10,<4.11',
  'numpy>=1.19,<2.0',
  'pysimdjson>=5.0.2,<6.0.0',
  'setuptools']
 
 setup_kwargs = {
     'name': 'pystan',
-    'version': '3.6.0',
+    'version': '3.7.0',
     'description': 'Python interface to Stan, a package for Bayesian inference',
     'long_description': '******\nPyStan\n******\n\n**PyStan** is a Python interface to Stan, a package for Bayesian inference.\n\nStan® is a state-of-the-art platform for statistical modeling and\nhigh-performance statistical computation. Thousands of users rely on Stan for\nstatistical modeling, data analysis, and prediction in the social, biological,\nand physical sciences, engineering, and business.\n\nNotable features of PyStan include:\n\n* Automatic caching of compiled Stan models\n* Automatic caching of samples from Stan models\n* An interface similar to that of RStan\n* Open source software: ISC License\n\nGetting started\n===============\n\nInstall PyStan with ``pip install pystan``. PyStan runs on Linux and macOS. You will also need a C++ compiler such as gcc ≥9.0 or clang ≥10.0.\n\nThe following block of code shows how to use PyStan with a model which studied coaching effects across eight schools (see Section 5.5 of Gelman et al (2003)). This hierarchical model is often called the "eight schools" model.\n\n.. code-block:: python\n\n    import stan\n\n    schools_code = """\n    data {\n      int<lower=0> J;         // number of schools\n      real y[J];              // estimated treatment effects\n      real<lower=0> sigma[J]; // standard error of effect estimates\n    }\n    parameters {\n      real mu;                // population treatment effect\n      real<lower=0> tau;      // standard deviation in treatment effects\n      vector[J] eta;          // unscaled deviation from mu by school\n    }\n    transformed parameters {\n      vector[J] theta = mu + tau * eta;        // school treatment effects\n    }\n    model {\n      target += normal_lpdf(eta | 0, 1);       // prior log-density\n      target += normal_lpdf(y | theta, sigma); // log-likelihood\n    }\n    """\n\n    schools_data = {"J": 8,\n                    "y": [28,  8, -3,  7, -1,  1, 18, 12],\n                    "sigma": [15, 10, 16, 11,  9, 11, 10, 18]}\n\n    posterior = stan.build(schools_code, data=schools_data)\n    fit = posterior.sample(num_chains=4, num_samples=1000)\n    eta = fit["eta"]  # array with shape (8, 4000)\n    df = fit.to_frame()  # pandas `DataFrame`\n\n\nCitation\n========\n\nWe appreciate citations as they let us discover what people have been doing\nwith the software. Citations also provide evidence of use which can help in\nobtaining grant funding.\n\nTo cite PyStan in publications use:\n\nRiddell, A., Hartikainen, A., & Carter, M. (2021). PyStan (3.0.0). https://pypi.org/project/pystan\n\nOr use the following BibTeX entry::\n\n    @misc{pystan,\n      title = {pystan (3.0.0)},\n      author = {Riddell, Allen and Hartikainen, Ari and Carter, Matthew},\n      year = {2021},\n      month = mar,\n      howpublished = {PyPI}\n    }\n\nPlease also cite Stan.\n',
     'author': 'Allen Riddell',
     'author_email': 'riddella@indiana.edu',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://mc-stan.org',
```

### Comparing `pystan-3.6.0/PKG-INFO` & `pystan-3.7.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pystan
-Version: 3.6.0
+Version: 3.7.0
 Summary: Python interface to Stan, a package for Bayesian inference
 Home-page: https://mc-stan.org
 License: ISC
 Author: Allen Riddell
 Author-email: riddella@indiana.edu
 Requires-Python: >=3.8,<4.0
 Classifier: Intended Audience :: Science/Research
@@ -12,15 +12,15 @@
 Classifier: License :: OSI Approved :: ISC License (ISCL)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: aiohttp (>=3.6,<4.0)
 Requires-Dist: clikit (>=0.6,<0.7)
-Requires-Dist: httpstan (>=4.9,<4.10)
+Requires-Dist: httpstan (>=4.10,<4.11)
 Requires-Dist: numpy (>=1.19,<2.0)
 Requires-Dist: pysimdjson (>=5.0.2,<6.0.0)
 Requires-Dist: setuptools
 Project-URL: Documentation, https://pystan.readthedocs.io
 Project-URL: Repository, https://github.com/stan-dev/pystan
 Description-Content-Type: text/x-rst
```

