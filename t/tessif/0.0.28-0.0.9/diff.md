# Comparing `tmp/tessif-0.0.28.tar.gz` & `tmp/tessif-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tessif-0.0.28.tar", max compression
+gzip compressed data, was "tessif-0.0.9.tar", max compression
```

## Comparing `tessif-0.0.28.tar` & `tessif-0.0.9.tar`

### file list

```diff
@@ -1,27 +1,6 @@
--rw-r--r--   0        0        0     1062 2023-04-23 09:46:00.864442 tessif-0.0.28/LICENSE
--rw-r--r--   0        0        0     2709 2023-04-23 09:46:00.864442 tessif-0.0.28/README.rst
--rw-r--r--   0        0        0     1645 2023-04-23 09:46:00.876442 tessif-0.0.28/pyproject.toml
--rw-r--r--   0        0        0      169 2023-04-23 09:46:00.876442 tessif-0.0.28/src/tessif/__init__.py
--rw-r--r--   0        0        0     7347 2023-04-23 09:46:00.876442 tessif-0.0.28/src/tessif/cli.py
--rw-r--r--   0        0        0   145078 2023-04-23 09:46:00.876442 tessif-0.0.28/src/tessif/components.py
--rw-r--r--   0        0        0     9273 2023-04-23 09:46:00.876442 tessif-0.0.28/src/tessif/deserialize.py
--rw-r--r--   0        0        0       67 2023-04-23 09:46:00.876442 tessif-0.0.28/src/tessif/frused/__init__.py
--rw-r--r--   0        0        0     4460 2023-04-23 09:46:00.876442 tessif-0.0.28/src/tessif/frused/configurations.py
--rw-r--r--   0        0        0    13102 2023-04-23 09:46:00.876442 tessif-0.0.28/src/tessif/frused/defaults.py
--rw-r--r--   0        0        0    11230 2023-04-23 09:46:00.876442 tessif-0.0.28/src/tessif/frused/namedtuples.py
--rw-r--r--   0        0        0     2210 2023-04-23 09:46:00.876442 tessif-0.0.28/src/tessif/frused/paths.py
--rw-r--r--   0        0        0     1594 2023-04-23 09:46:00.876442 tessif-0.0.28/src/tessif/frused/resolutions.py
--rw-r--r--   0        0        0   101110 2023-04-23 09:46:00.876442 tessif-0.0.28/src/tessif/frused/spellings.py
--rw-r--r--   0        0        0    33455 2023-04-23 09:46:00.876442 tessif-0.0.28/src/tessif/frused/themes.py
--rw-r--r--   0        0        0     2195 2023-04-23 09:46:00.876442 tessif-0.0.28/src/tessif/frused/utils.py
--rw-r--r--   0        0        0      391 2023-04-23 09:46:00.876442 tessif-0.0.28/src/tessif/hooks/__init__.py
--rw-r--r--   0        0        0     9906 2023-04-23 09:46:00.876442 tessif-0.0.28/src/tessif/hooks/ppsa.py
--rw-r--r--   0        0        0     4919 2023-04-23 09:46:00.876442 tessif-0.0.28/src/tessif/hooks/tsf.py
--rw-r--r--   0        0        0     2560 2023-04-23 09:46:00.876442 tessif-0.0.28/src/tessif/logging.py
--rw-r--r--   0        0        0    11494 2023-04-23 09:46:00.876442 tessif-0.0.28/src/tessif/nxgraph.py
--rw-r--r--   0        0        0   123533 2023-04-23 09:46:00.876442 tessif-0.0.28/src/tessif/post_process.py
--rw-r--r--   0        0        0     2634 2023-04-23 09:46:00.876442 tessif-0.0.28/src/tessif/serialize.py
--rw-r--r--   0        0        0    26579 2023-04-23 09:46:00.876442 tessif-0.0.28/src/tessif/system_model.py
--rw-r--r--   0        0        0     2323 2023-04-23 09:46:00.876442 tessif-0.0.28/src/tessif/tropp.py
--rw-r--r--   0        0        0     3754 1970-01-01 00:00:00.000000 tessif-0.0.28/setup.py
--rw-r--r--   0        0        0     3611 1970-01-01 00:00:00.000000 tessif-0.0.28/PKG-INFO
+-rw-r--r--   0        0        0     1062 2022-05-24 13:48:54.900094 tessif-0.0.9/LICENSE
+-rw-r--r--   0        0        0     1985 2022-05-24 13:48:54.900094 tessif-0.0.9/README.rst
+-rw-r--r--   0        0        0     1341 2022-05-24 13:48:54.900094 tessif-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      168 2022-05-24 13:48:54.900094 tessif-0.0.9/src/tessif/__init__.py
+-rw-r--r--   0        0        0     2777 2022-05-24 13:49:04.202632 tessif-0.0.9/setup.py
+-rw-r--r--   0        0        0     2680 2022-05-24 13:49:04.202903 tessif-0.0.9/PKG-INFO
```

### Comparing `tessif-0.0.28/LICENSE` & `tessif-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `tessif-0.0.28/README.rst` & `tessif-0.0.9/README.rst`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-tessif (**T**\ ransforming **E**\ nergy **S**\ upply **S**\ ystem model\ **I**\ ng **F**\ ramework)
-===================================================================================================
+Tessif
+======
 
 |PyPI| |Status| |Python Version| |License|
 
 |Read the Docs| |Tests| |Codecov|
 
 |pre-commit| |Black|
 
@@ -32,40 +32,31 @@
    :target: https://github.com/pre-commit/pre-commit
    :alt: pre-commit
 .. |Black| image:: https://img.shields.io/badge/code%20style-black-000000.svg
    :target: https://github.com/psf/black
    :alt: Black
 
 
-Latest Stable Version
----------------------
-You can install *Tessif* via pip_ from PyPI_.
-Install using a console with your virtual environment activated:
 
-.. code-block:: console
+Transforming Energy Suppy System modellIng Framework
 
-   $ pip install tessif
-
-Latest Development Version (potentially unstable)
--------------------------------------------------
-
-You can install the development version of *Tessif* via pip_ from TestPyPI_.
-Install using a console with your virtual environment activated:
+Installation
+------------
 
-.. code-block:: console
+You can install *Tessif* via pip_ from PyPI_:
 
-   $ pip install --index-url https://test.pypi.org/simple/ --extra-index-url https://pypi.org/simple/ tessif
+.. code:: console
 
-This installs the TestPyPI_ version of tessif while resolving the dependencies on PyPI_.
+   $ pip install tessif
 
 License
 -------
+
 Distributed under the terms of the `MIT license`_,
 *Tessif* is free and open source software.
 
 .. _MIT license: https://opensource.org/licenses/MIT
 .. _PyPI: https://pypi.org/
-.. _TestPyPI: https://test.pypi.org/
 .. _pip: https://pip.pypa.io/
 .. github-only
 .. _Contributor Guide: CONTRIBUTING.rst
 .. _Usage: https://tessif.readthedocs.io/en/latest/usage.html
```

### Comparing `tessif-0.0.28/setup.py` & `tessif-0.0.9/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,42 +1,34 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 package_dir = \
 {'': 'src'}
 
 packages = \
-['tessif', 'tessif.frused', 'tessif.hooks']
+['tessif']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['click>7',
- 'dcttools>=0.1.4,<0.2.0',
- 'matplotlib>=3,<4',
- 'networkx>=3,<4',
- 'strutils>=0.1.1,<0.2.0']
-
-entry_points = \
-{'console_scripts': ['tessif = tessif.cli:main_cli_entry']}
+['requests>=2.27.1,<3.0.0']
 
 setup_kwargs = {
     'name': 'tessif',
-    'version': '0.0.28',
+    'version': '0.0.9',
     'description': 'Transforming Energy Supply System modell*I*ng Framework',
-    'long_description': 'tessif (**T**\\ ransforming **E**\\ nergy **S**\\ upply **S**\\ ystem model\\ **I**\\ ng **F**\\ ramework)\n===================================================================================================\n\n|PyPI| |Status| |Python Version| |License|\n\n|Read the Docs| |Tests| |Codecov|\n\n|pre-commit| |Black|\n\n.. |PyPI| image:: https://img.shields.io/pypi/v/tessif.svg\n   :target: https://pypi.org/project/tessif/\n   :alt: PyPI\n.. |Status| image:: https://img.shields.io/pypi/status/tessif.svg\n   :target: https://pypi.org/project/tessif/\n   :alt: Status\n.. |Python Version| image:: https://img.shields.io/pypi/pyversions/tessif\n   :target: https://pypi.org/project/tessif\n   :alt: Python Version\n.. |License| image:: https://img.shields.io/pypi/l/tessif\n   :target: https://opensource.org/licenses/MIT\n   :alt: License\n.. |Read the Docs| image:: https://img.shields.io/readthedocs/tessif/latest.svg?label=Read%20the%20Docs\n   :target: https://tessif.readthedocs.io/\n   :alt: Read the documentation at https://tessif.readthedocs.io/\n.. |Tests| image:: https://github.com/tZ3ma/tessif/workflows/Tests/badge.svg\n   :target: https://github.com/tZ3ma/tessif/actions?workflow=Tests\n   :alt: Tests\n.. |Codecov| image:: https://codecov.io/gh/tZ3ma/tessif/branch/main/graph/badge.svg\n   :target: https://codecov.io/gh/tZ3ma/tessif\n   :alt: Codecov\n.. |pre-commit| image:: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white\n   :target: https://github.com/pre-commit/pre-commit\n   :alt: pre-commit\n.. |Black| image:: https://img.shields.io/badge/code%20style-black-000000.svg\n   :target: https://github.com/psf/black\n   :alt: Black\n\n\nLatest Stable Version\n---------------------\nYou can install *Tessif* via pip_ from PyPI_.\nInstall using a console with your virtual environment activated:\n\n.. code-block:: console\n\n   $ pip install tessif\n\nLatest Development Version (potentially unstable)\n-------------------------------------------------\n\nYou can install the development version of *Tessif* via pip_ from TestPyPI_.\nInstall using a console with your virtual environment activated:\n\n.. code-block:: console\n\n   $ pip install --index-url https://test.pypi.org/simple/ --extra-index-url https://pypi.org/simple/ tessif\n\nThis installs the TestPyPI_ version of tessif while resolving the dependencies on PyPI_.\n\nLicense\n-------\nDistributed under the terms of the `MIT license`_,\n*Tessif* is free and open source software.\n\n.. _MIT license: https://opensource.org/licenses/MIT\n.. _PyPI: https://pypi.org/\n.. _TestPyPI: https://test.pypi.org/\n.. _pip: https://pip.pypa.io/\n.. github-only\n.. _Contributor Guide: CONTRIBUTING.rst\n.. _Usage: https://tessif.readthedocs.io/en/latest/usage.html\n',
+    'long_description': 'Tessif\n======\n\n|PyPI| |Status| |Python Version| |License|\n\n|Read the Docs| |Tests| |Codecov|\n\n|pre-commit| |Black|\n\n.. |PyPI| image:: https://img.shields.io/pypi/v/tessif.svg\n   :target: https://pypi.org/project/tessif/\n   :alt: PyPI\n.. |Status| image:: https://img.shields.io/pypi/status/tessif.svg\n   :target: https://pypi.org/project/tessif/\n   :alt: Status\n.. |Python Version| image:: https://img.shields.io/pypi/pyversions/tessif\n   :target: https://pypi.org/project/tessif\n   :alt: Python Version\n.. |License| image:: https://img.shields.io/pypi/l/tessif\n   :target: https://opensource.org/licenses/MIT\n   :alt: License\n.. |Read the Docs| image:: https://img.shields.io/readthedocs/tessif/latest.svg?label=Read%20the%20Docs\n   :target: https://tessif.readthedocs.io/\n   :alt: Read the documentation at https://tessif.readthedocs.io/\n.. |Tests| image:: https://github.com/tZ3ma/tessif/workflows/Tests/badge.svg\n   :target: https://github.com/tZ3ma/tessif/actions?workflow=Tests\n   :alt: Tests\n.. |Codecov| image:: https://codecov.io/gh/tZ3ma/tessif/branch/main/graph/badge.svg\n   :target: https://codecov.io/gh/tZ3ma/tessif\n   :alt: Codecov\n.. |pre-commit| image:: https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white\n   :target: https://github.com/pre-commit/pre-commit\n   :alt: pre-commit\n.. |Black| image:: https://img.shields.io/badge/code%20style-black-000000.svg\n   :target: https://github.com/psf/black\n   :alt: Black\n\n\n\nTransforming Energy Suppy System modellIng Framework\n\nInstallation\n------------\n\nYou can install *Tessif* via pip_ from PyPI_:\n\n.. code:: console\n\n   $ pip install tessif\n\nLicense\n-------\n\nDistributed under the terms of the `MIT license`_,\n*Tessif* is free and open source software.\n\n.. _MIT license: https://opensource.org/licenses/MIT\n.. _PyPI: https://pypi.org/\n.. _pip: https://pip.pypa.io/\n.. github-only\n.. _Contributor Guide: CONTRIBUTING.rst\n.. _Usage: https://tessif.readthedocs.io/en/latest/usage.html\n',
     'author': 'Mathias Ammon',
-    'author_email': 'tz3ma.coding@use.startmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
+    'author_email': 'mathias.ammon@tuhh.de',
+    'maintainer': None,
+    'maintainer_email': None,
     'url': 'https://github.com/tZ3ma/tessif',
     'package_dir': package_dir,
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
-    'entry_points': entry_points,
     'python_requires': '>=3.8,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

