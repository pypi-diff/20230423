# Comparing `tmp/stac_api_validator-0.5.0.tar.gz` & `tmp/stac_api_validator-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stac_api_validator-0.5.0.tar", max compression
+gzip compressed data, was "stac_api_validator-0.6.0.tar", max compression
```

## Comparing `stac_api_validator-0.5.0.tar` & `stac_api_validator-0.6.0.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0    11342 2023-02-21 14:14:20.736492 stac_api_validator-0.5.0/LICENSE
--rw-r--r--   0        0        0     9874 2023-02-21 14:14:20.736492 stac_api_validator-0.5.0/README.md
--rw-r--r--   0        0        0     2450 2023-02-21 14:14:34.008688 stac_api_validator-0.5.0/pyproject.toml
--rw-r--r--   0        0        0       26 2023-02-21 14:14:20.736492 stac_api_validator-0.5.0/src/stac_api_validator/__init__.py
--rw-r--r--   0        0        0     2712 2023-02-21 14:14:20.736492 stac_api_validator-0.5.0/src/stac_api_validator/__main__.py
--rw-r--r--   0        0        0     9583 2023-02-21 14:14:20.736492 stac_api_validator-0.5.0/src/stac_api_validator/filters.py
--rw-r--r--   0        0        0     1303 2023-02-21 14:14:20.736492 stac_api_validator-0.5.0/src/stac_api_validator/geometries.py
--rw-r--r--   0        0        0        0 2023-02-21 14:14:20.736492 stac_api_validator-0.5.0/src/stac_api_validator/py.typed
--rw-r--r--   0        0        0    82722 2023-02-21 14:14:20.736492 stac_api_validator-0.5.0/src/stac_api_validator/validations.py
--rw-r--r--   0        0        0    11292 1970-01-01 00:00:00.000000 stac_api_validator-0.5.0/setup.py
--rw-r--r--   0        0        0    11158 1970-01-01 00:00:00.000000 stac_api_validator-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0    11342 2023-04-23 14:33:55.142043 stac_api_validator-0.6.0/LICENSE
+-rw-r--r--   0        0        0     9879 2023-04-23 14:33:55.142043 stac_api_validator-0.6.0/README.md
+-rw-r--r--   0        0        0     2450 2023-04-23 14:34:14.914210 stac_api_validator-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0       26 2023-04-23 14:33:55.146043 stac_api_validator-0.6.0/src/stac_api_validator/__init__.py
+-rw-r--r--   0        0        0     6329 2023-04-23 14:33:55.146043 stac_api_validator-0.6.0/src/stac_api_validator/__main__.py
+-rw-r--r--   0        0        0     9583 2023-04-23 14:33:55.146043 stac_api_validator-0.6.0/src/stac_api_validator/filters.py
+-rw-r--r--   0        0        0     1303 2023-04-23 14:33:55.146043 stac_api_validator-0.6.0/src/stac_api_validator/geometries.py
+-rw-r--r--   0        0        0        0 2023-04-23 14:33:55.146043 stac_api_validator-0.6.0/src/stac_api_validator/py.typed
+-rw-r--r--   0        0        0   130124 2023-04-23 14:33:55.146043 stac_api_validator-0.6.0/src/stac_api_validator/validations.py
+-rw-r--r--   0        0        0    11163 1970-01-01 00:00:00.000000 stac_api_validator-0.6.0/PKG-INFO
```

### Comparing `stac_api_validator-0.5.0/LICENSE` & `stac_api_validator-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `stac_api_validator-0.5.0/README.md` & `stac_api_validator-0.6.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)][pre-commit]
 [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)][black]
 
 [pypi_]: https://pypi.org/project/stac-api-validator/
 [status]: https://pypi.org/project/stac-api-validator/
 [python version]: https://pypi.org/project/stac-api-validator
-[read the docs]: https://stac-api-validator.readthedocs.io/
+[read the docs]: https://stac-api-validator.readthedocs.io/en/latest
 [tests]: https://github.com/stac-utils/stac-api-validator/actions?workflow=Tests
 [codecov]: https://app.codecov.io/gh/stac-utils/stac-api-validator
 [pre-commit]: https://github.com/pre-commit/pre-commit
 [black]: https://github.com/psf/black
 
 ## Introduction
 
@@ -34,21 +34,21 @@
 ## Installation
 
 STAC API Validator requires Python 3.10.
 
 You can install _STAC API Validator_ via [pip] from [PyPI]:
 
 ```console
-$ pip install stac-api-validator
+pip install stac-api-validator
 ```
 
 and then run it:
 
 ```console
-$ stac-api-validator \
+stac-api-validator \
     --root-url https://planetarycomputer.microsoft.com/api/stac/v1/ \
     --conformance core \
     --conformance features \
     --conformance item-search \
     --collection sentinel-2-l2a \
     --geometry '{"type": "Polygon", "coordinates": [[[100.0, 0.0], [101.0, 0.0], [101.0, 1.0], [100.0, 1.0], [100.0, 0.0]]]}'
 ```
```

### Comparing `stac_api_validator-0.5.0/pyproject.toml` & `stac_api_validator-0.6.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "stac-api-validator"
-version = "0.5.0"
+version = "0.6.0"
 description = "STAC API Validator"
 authors = ["Phil Varner <phil@philvarner.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/stac-utils/stac-api-validator"
 repository = "https://github.com/stac-utils/stac-api-validator"
 documentation = "https://stac-api-validator.readthedocs.io"
@@ -15,17 +15,17 @@
 [tool.poetry.urls]
 Changelog = "https://github.com/stac-utils/stac-api-validator/releases"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 click = "^8.1.3"
 certifi = "^2022.12.07"  # CVE-2022-23491: https://github.com/certifi/python-certifi/security/advisories/GHSA-43fp-rhv2-5gv8
-pystac-client = "^0.5.1"
+pystac-client = "^0.6.1"
 requests = "^2.28.1"
-pystac = {extras = ["orjson"], version = "^1.6.1"}
+pystac = {extras = ["orjson"], version = "^1.7.1"}
 jsonschema = "^4.16.0"
 PyYAML = "6.0"
 Shapely = "1.8.4"
 more_itertools = "^8.14.0"
 stac-check = "^1.3.1"
 stac-validator = "^3.2.0"
 deepdiff = "^6.2.3"
```

### Comparing `stac_api_validator-0.5.0/src/stac_api_validator/filters.py` & `stac_api_validator-0.6.0/src/stac_api_validator/filters.py`

 * *Files identical despite different names*

### Comparing `stac_api_validator-0.5.0/src/stac_api_validator/geometries.py` & `stac_api_validator-0.6.0/src/stac_api_validator/geometries.py`

 * *Files identical despite different names*

### Comparing `stac_api_validator-0.5.0/setup.py` & `stac_api_validator-0.6.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,49 +1,247 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: stac-api-validator
+Version: 0.6.0
+Summary: STAC API Validator
+Home-page: https://github.com/stac-utils/stac-api-validator
+License: Apache-2.0
+Author: Phil Varner
+Author-email: phil@philvarner.com
+Requires-Python: >=3.10,<4.0
+Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: PyYAML (==6.0)
+Requires-Dist: Shapely (==1.8.4)
+Requires-Dist: certifi (>=2022.12.07,<2023.0.0)
+Requires-Dist: click (>=8.1.3,<9.0.0)
+Requires-Dist: deepdiff (>=6.2.3,<7.0.0)
+Requires-Dist: jsonschema (>=4.16.0,<5.0.0)
+Requires-Dist: more_itertools (>=8.14.0,<9.0.0)
+Requires-Dist: pystac-client (>=0.6.1,<0.7.0)
+Requires-Dist: pystac[orjson] (>=1.7.1,<2.0.0)
+Requires-Dist: requests (>=2.28.1,<3.0.0)
+Requires-Dist: stac-check (>=1.3.1,<2.0.0)
+Requires-Dist: stac-validator (>=3.2.0,<4.0.0)
+Project-URL: Changelog, https://github.com/stac-utils/stac-api-validator/releases
+Project-URL: Documentation, https://stac-api-validator.readthedocs.io
+Project-URL: Repository, https://github.com/stac-utils/stac-api-validator
+Description-Content-Type: text/markdown
+
+# STAC API Validator
+
+[![PyPI](https://img.shields.io/pypi/v/stac-api-validator.svg)][pypi_]
+[![Status](https://img.shields.io/pypi/status/stac-api-validator.svg)][status]
+[![Python Version](https://img.shields.io/pypi/pyversions/stac-api-validator)][python version]
+[![License](https://img.shields.io/pypi/l/stac-api-validator)][license]
+
+[![Read the documentation at https://stac-api-validator.readthedocs.io/](https://img.shields.io/readthedocs/stac-api-validator/latest.svg?label=Read%20the%20Docs)][read the docs]
+[![Tests](https://github.com/stac-utils/stac-api-validator/workflows/Tests/badge.svg)][tests]
+[![Codecov](https://codecov.io/gh/stac-utils/stac-api-validator/branch/main/graph/badge.svg)][codecov]
+
+[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)][pre-commit]
+[![Black](https://img.shields.io/badge/code%20style-black-000000.svg)][black]
+
+[pypi_]: https://pypi.org/project/stac-api-validator/
+[status]: https://pypi.org/project/stac-api-validator/
+[python version]: https://pypi.org/project/stac-api-validator
+[read the docs]: https://stac-api-validator.readthedocs.io/en/latest
+[tests]: https://github.com/stac-utils/stac-api-validator/actions?workflow=Tests
+[codecov]: https://app.codecov.io/gh/stac-utils/stac-api-validator
+[pre-commit]: https://github.com/pre-commit/pre-commit
+[black]: https://github.com/psf/black
+
+## Introduction
+
+The STAC API Validator is the official validation suite for the
+[STAC API](https://github.com/radiantearth/stac-api-spec/) family of specifications.
+
+## Documentation
+
+See the [stable](https://stac-api-validator.readthedocs.io/en/stable/) or
+[latest](https://stac-api-validator.readthedocs.io/en/latest) documentation pages.
+
+## Installation
+
+STAC API Validator requires Python 3.10.
+
+You can install _STAC API Validator_ via [pip] from [PyPI]:
+
+```console
+pip install stac-api-validator
+```
+
+and then run it:
+
+```console
+stac-api-validator \
+    --root-url https://planetarycomputer.microsoft.com/api/stac/v1/ \
+    --conformance core \
+    --conformance features \
+    --conformance item-search \
+    --collection sentinel-2-l2a \
+    --geometry '{"type": "Polygon", "coordinates": [[[100.0, 0.0], [101.0, 0.0], [101.0, 1.0], [100.0, 1.0], [100.0, 0.0]]]}'
+```
+
+## Contributing
+
+Contributions are very welcome.
+To learn more, see the [Contributor Guide].
+
+## Usage
+
+Please see the [Command-line Reference] for details.
+
+The conformance class validations to run are selected with the `--conformance` parameters. This parameter
+can be used more than once to specify multiple conformance classes to validate. The `STAC API - Core` conformance
+class will always be validated, even if not specified.
+
+If `item-search`, `collections`, and/or `features` are specified, the `--collection` and `--geometry` parameters must also
+be specified. The `--collection` parameter specifies the name of a collection to use for some of the validations.
+The `--geometry` should specify an AOI over which there are between 100 and 20,000 results for the collection (more
+results means longer time to run).
+
+## Features
+
+**Work in Progress** -- this currently only validates a subset of behavior
+
+This validation suite focuses on validating STAC API interactions. Tools such as
+[pystac](https://github.com/stac-utils/pystac) and [stac4s](https://github.com/azavea/stac4s) do a
+good job of validating STAC objects (Catalog, Collection, Item). This suite focuses on the STAC API behavior
+validation.
+
+The three key concepts within a STAC API are:
+
+1. _Conformance classes_ advertising the capabilities of the API
+2. _Link relations_ between resources within the web API (hypermedia)
+3. _Parameters_ that filter search results
+
+The conformance classes, as defined in the `conformsTo` field of the Landing Page (root, `/`), advertise to
+clients which capabilities are available in the API. Without this field, a client would not even be able to tell that a
+root URI was a STAC API.
+
+The link relations define how to navigate a STAC catalog through parent-child links and find resources such as the OpenAPI specification. While many OGC API and STAC API endpoint have a fixed value (e.g., `/collections`), it is preferable for clients discover the paths via hypermedia.
+
+The parameters that filter results apply to the Items resource and Item Search endpoints.
+
+The current validity status of several popular STAC API implementations can be found [here](COMPLIANCE_REPORT.md).
+
+## Command-line Reference
+
+Usage:
+
+```
+Usage: stac-api-validator [OPTIONS]
+
+  STAC API Validator.
+
+Options:
+  --version                       Show the version and exit.
+  --log-level TEXT                Logging level, one of DEBUG, INFO, WARN,
+                                  ERROR, CRITICAL
+  --root-url TEXT                 STAC API Root / Landing Page URL  [required]
+  --collection TEXT               The name of the collection to use for item-
+                                  search, collections, and features tests.
+  --geometry TEXT                 The GeoJSON geometry to use for intersection
+                                  tests.
+  --conformance [core|browseable|item-search|features|collections|children|filter]
+                                  The conformance classes to validate.
+                                  [required]
+  --auth-bearer-token TEXT        Authorization Bearer token value to append
+                                  to all requests.
+  --auth-query-parameter TEXT     Query pararmeter key and value to pass for
+                                  authorization, e.g., 'key=xyz'.
+  --help                          Show this message and exit.
+```
+
+Conformance classes item-search, features, and collections require the `--collection` parameter with the id of a
+collection to run some tests on.
+
+Conformance class `item-search` requires `--geometry` with a GeoJSON geometry that returns some items for
+the specified collection.
+
+Example:
+
+```
+stac-api-validator \
+    --root-url https://planetarycomputer.microsoft.com/api/stac/v1/ \
+    --conformance core \
+    --conformance item-search \
+    --conformance features \
+    --collection sentinel-2-l2a \
+    --geometry '{"type": "Polygon", "coordinates": [[[100.0, 0.0], [101.0, 0.0], [101.0, 1.0], [100.0, 1.0], [100.0, 0.0]]]}'
+```
+
+Example output:
+
+```
+Validating https://cmr.earthdata.nasa.gov/stac/LARC_ASDC ...
+STAC API - Core conformance class found.
+STAC API - Item Search conformance class found.
+warnings: none
+errors:
+- service-desc (https://api.stacspec.org/v1.0.0-beta.1/openapi.yaml): should have content-type header 'application/vnd.oai.openapi+json;version=3.0'', actually 'text/yaml'
+- service-desc (https://api.stacspec.org/v1.0.0-beta.1/openapi.yaml): should return JSON, instead got non-JSON text
+- GET Search with bbox=100.0, 0.0, 105.0, 1.0 returned status code 400
+- POST Search with bbox:[100.0, 0.0, 105.0, 1.0] returned status code 502
+- GET Search with bbox=100.0,0.0,0.0,105.0,1.0,1.0 returned status code 400
+- POST Search with bbox:[100.0, 0.0, 0.0, 105.0, 1.0, 1.0] returned status code 400
+```
+
+Example with authorization using parameters:
+
+```
+stac-api-validator --root-url https://api.radiant.earth/mlhub/v1 --conformance core --auth-query-parameter 'key=xxx'
+```
+
+## Validating OGC API Features - Part 1 compliance
+
+A STAC API that conforms to the "STAC API - Features" conformance class will also be a valid implementation
+of OGC API Features - Part 1. In general, this validator focuses on those aspects of API behavior that are
+different between STAC and OGC. It is recommended that implementers also use the [OGC API Features - Part 1
+validation test suite](https://cite.opengeospatial.org/teamengine/about/ogcapi-features-1.0/1.0/site/) to
+validate conformance.
+
+Full instructions are available at the link above, but the simplest way to run this is with:
+
+```
+docker run -p 8081:8080 ogccite/ets-ogcapi-features10
+```
+
+Then, open [http://localhost:8081/teamengine/](http://localhost:8081/teamengine/) and login with the
+username and password `ogctest`, `Create a new session`, with Organization `OGC`, Specification `OGC API - Features`, `Start a new test session`, input he root URL for the service, and `Start`.
+
+## Common Mistakes
+
+- incorrect `conformsTo` in the Landing Page. This was added between STAC API 0.9 and 1.0. It should be the same as the value in the `conformsTo` in the OAFeat `/conformance` endpoint.
+- OGC API Features uses `data` relation link relation at the root to point to the Collections endpoint (`/collections`), not `collections` relation
+- media type for link relation `service-desc` and endpoint is `application/vnd.oai.openapi+json;version=3.0` (not `application/json`) and link relation `search` and endpoint is `application/geo+json` (not `application/json`)
+- Use of OCG API "req" urls instead of "conf" urls, e.g. `http://www.opengis.net/spec/ogcapi-features-1/1.0/conf/core` should be used, not `http://www.opengis.net/spec/ogcapi-features-1/1.0/req/core`
+
+## License
+
+Distributed under the terms of the [Apache 2.0 license][license],
+_STAC API Validator_ is free and open source software.
+
+## Issues
+
+If you encounter any problems,
+please [file an issue] along with a detailed description.
+
+## Credits
+
+This project was generated from [@cjolowicz]'s [Hypermodern Python Cookiecutter] template.
+
+[@cjolowicz]: https://github.com/cjolowicz
+[pypi]: https://pypi.org/
+[hypermodern python cookiecutter]: https://github.com/cjolowicz/cookiecutter-hypermodern-python
+[file an issue]: https://github.com/stac-utils/stac-api-validator/issues
+[pip]: https://pip.pypa.io/
+
+<!-- github-only -->
+
+[license]: https://github.com/stac-utils/stac-api-validator/blob/main/LICENSE
+[contributor guide]: https://github.com/stac-utils/stac-api-validator/blob/main/CONTRIBUTING.md
+[command-line reference]: https://stac-api-validator.readthedocs.io/en/latest/usage.html
 
-package_dir = \
-{'': 'src'}
-
-packages = \
-['stac_api_validator']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['PyYAML==6.0',
- 'Shapely==1.8.4',
- 'certifi>=2022.12.07,<2023.0.0',
- 'click>=8.1.3,<9.0.0',
- 'deepdiff>=6.2.3,<7.0.0',
- 'jsonschema>=4.16.0,<5.0.0',
- 'more_itertools>=8.14.0,<9.0.0',
- 'pystac-client>=0.5.1,<0.6.0',
- 'pystac[orjson]>=1.6.1,<2.0.0',
- 'requests>=2.28.1,<3.0.0',
- 'stac-check>=1.3.1,<2.0.0',
- 'stac-validator>=3.2.0,<4.0.0']
-
-entry_points = \
-{'console_scripts': ['stac-api-validator = stac_api_validator.__main__:main']}
-
-setup_kwargs = {
-    'name': 'stac-api-validator',
-    'version': '0.5.0',
-    'description': 'STAC API Validator',
-    'long_description': '# STAC API Validator\n\n[![PyPI](https://img.shields.io/pypi/v/stac-api-validator.svg)][pypi_]\n[![Status](https://img.shields.io/pypi/status/stac-api-validator.svg)][status]\n[![Python Version](https://img.shields.io/pypi/pyversions/stac-api-validator)][python version]\n[![License](https://img.shields.io/pypi/l/stac-api-validator)][license]\n\n[![Read the documentation at https://stac-api-validator.readthedocs.io/](https://img.shields.io/readthedocs/stac-api-validator/latest.svg?label=Read%20the%20Docs)][read the docs]\n[![Tests](https://github.com/stac-utils/stac-api-validator/workflows/Tests/badge.svg)][tests]\n[![Codecov](https://codecov.io/gh/stac-utils/stac-api-validator/branch/main/graph/badge.svg)][codecov]\n\n[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)][pre-commit]\n[![Black](https://img.shields.io/badge/code%20style-black-000000.svg)][black]\n\n[pypi_]: https://pypi.org/project/stac-api-validator/\n[status]: https://pypi.org/project/stac-api-validator/\n[python version]: https://pypi.org/project/stac-api-validator\n[read the docs]: https://stac-api-validator.readthedocs.io/\n[tests]: https://github.com/stac-utils/stac-api-validator/actions?workflow=Tests\n[codecov]: https://app.codecov.io/gh/stac-utils/stac-api-validator\n[pre-commit]: https://github.com/pre-commit/pre-commit\n[black]: https://github.com/psf/black\n\n## Introduction\n\nThe STAC API Validator is the official validation suite for the\n[STAC API](https://github.com/radiantearth/stac-api-spec/) family of specifications.\n\n## Documentation\n\nSee the [stable](https://stac-api-validator.readthedocs.io/en/stable/) or\n[latest](https://stac-api-validator.readthedocs.io/en/latest) documentation pages.\n\n## Installation\n\nSTAC API Validator requires Python 3.10.\n\nYou can install _STAC API Validator_ via [pip] from [PyPI]:\n\n```console\n$ pip install stac-api-validator\n```\n\nand then run it:\n\n```console\n$ stac-api-validator \\\n    --root-url https://planetarycomputer.microsoft.com/api/stac/v1/ \\\n    --conformance core \\\n    --conformance features \\\n    --conformance item-search \\\n    --collection sentinel-2-l2a \\\n    --geometry \'{"type": "Polygon", "coordinates": [[[100.0, 0.0], [101.0, 0.0], [101.0, 1.0], [100.0, 1.0], [100.0, 0.0]]]}\'\n```\n\n## Contributing\n\nContributions are very welcome.\nTo learn more, see the [Contributor Guide].\n\n## Usage\n\nPlease see the [Command-line Reference] for details.\n\nThe conformance class validations to run are selected with the `--conformance` parameters. This parameter\ncan be used more than once to specify multiple conformance classes to validate. The `STAC API - Core` conformance\nclass will always be validated, even if not specified.\n\nIf `item-search`, `collections`, and/or `features` are specified, the `--collection` and `--geometry` parameters must also\nbe specified. The `--collection` parameter specifies the name of a collection to use for some of the validations.\nThe `--geometry` should specify an AOI over which there are between 100 and 20,000 results for the collection (more\nresults means longer time to run).\n\n## Features\n\n**Work in Progress** -- this currently only validates a subset of behavior\n\nThis validation suite focuses on validating STAC API interactions. Tools such as\n[pystac](https://github.com/stac-utils/pystac) and [stac4s](https://github.com/azavea/stac4s) do a\ngood job of validating STAC objects (Catalog, Collection, Item). This suite focuses on the STAC API behavior\nvalidation.\n\nThe three key concepts within a STAC API are:\n\n1. _Conformance classes_ advertising the capabilities of the API\n2. _Link relations_ between resources within the web API (hypermedia)\n3. _Parameters_ that filter search results\n\nThe conformance classes, as defined in the `conformsTo` field of the Landing Page (root, `/`), advertise to\nclients which capabilities are available in the API. Without this field, a client would not even be able to tell that a\nroot URI was a STAC API.\n\nThe link relations define how to navigate a STAC catalog through parent-child links and find resources such as the OpenAPI specification. While many OGC API and STAC API endpoint have a fixed value (e.g., `/collections`), it is preferable for clients discover the paths via hypermedia.\n\nThe parameters that filter results apply to the Items resource and Item Search endpoints.\n\nThe current validity status of several popular STAC API implementations can be found [here](COMPLIANCE_REPORT.md).\n\n## Command-line Reference\n\nUsage:\n\n```\nUsage: stac-api-validator [OPTIONS]\n\n  STAC API Validator.\n\nOptions:\n  --version                       Show the version and exit.\n  --log-level TEXT                Logging level, one of DEBUG, INFO, WARN,\n                                  ERROR, CRITICAL\n  --root-url TEXT                 STAC API Root / Landing Page URL  [required]\n  --collection TEXT               The name of the collection to use for item-\n                                  search, collections, and features tests.\n  --geometry TEXT                 The GeoJSON geometry to use for intersection\n                                  tests.\n  --conformance [core|browseable|item-search|features|collections|children|filter]\n                                  The conformance classes to validate.\n                                  [required]\n  --auth-bearer-token TEXT        Authorization Bearer token value to append\n                                  to all requests.\n  --auth-query-parameter TEXT     Query pararmeter key and value to pass for\n                                  authorization, e.g., \'key=xyz\'.\n  --help                          Show this message and exit.\n```\n\nConformance classes item-search, features, and collections require the `--collection` parameter with the id of a\ncollection to run some tests on.\n\nConformance class `item-search` requires `--geometry` with a GeoJSON geometry that returns some items for\nthe specified collection.\n\nExample:\n\n```\nstac-api-validator \\\n    --root-url https://planetarycomputer.microsoft.com/api/stac/v1/ \\\n    --conformance core \\\n    --conformance item-search \\\n    --conformance features \\\n    --collection sentinel-2-l2a \\\n    --geometry \'{"type": "Polygon", "coordinates": [[[100.0, 0.0], [101.0, 0.0], [101.0, 1.0], [100.0, 1.0], [100.0, 0.0]]]}\'\n```\n\nExample output:\n\n```\nValidating https://cmr.earthdata.nasa.gov/stac/LARC_ASDC ...\nSTAC API - Core conformance class found.\nSTAC API - Item Search conformance class found.\nwarnings: none\nerrors:\n- service-desc (https://api.stacspec.org/v1.0.0-beta.1/openapi.yaml): should have content-type header \'application/vnd.oai.openapi+json;version=3.0\'\', actually \'text/yaml\'\n- service-desc (https://api.stacspec.org/v1.0.0-beta.1/openapi.yaml): should return JSON, instead got non-JSON text\n- GET Search with bbox=100.0, 0.0, 105.0, 1.0 returned status code 400\n- POST Search with bbox:[100.0, 0.0, 105.0, 1.0] returned status code 502\n- GET Search with bbox=100.0,0.0,0.0,105.0,1.0,1.0 returned status code 400\n- POST Search with bbox:[100.0, 0.0, 0.0, 105.0, 1.0, 1.0] returned status code 400\n```\n\nExample with authorization using parameters:\n\n```\nstac-api-validator --root-url https://api.radiant.earth/mlhub/v1 --conformance core --auth-query-parameter \'key=xxx\'\n```\n\n## Validating OGC API Features - Part 1 compliance\n\nA STAC API that conforms to the "STAC API - Features" conformance class will also be a valid implementation\nof OGC API Features - Part 1. In general, this validator focuses on those aspects of API behavior that are\ndifferent between STAC and OGC. It is recommended that implementers also use the [OGC API Features - Part 1\nvalidation test suite](https://cite.opengeospatial.org/teamengine/about/ogcapi-features-1.0/1.0/site/) to\nvalidate conformance.\n\nFull instructions are available at the link above, but the simplest way to run this is with:\n\n```\ndocker run -p 8081:8080 ogccite/ets-ogcapi-features10\n```\n\nThen, open [http://localhost:8081/teamengine/](http://localhost:8081/teamengine/) and login with the\nusername and password `ogctest`, `Create a new session`, with Organization `OGC`, Specification `OGC API - Features`, `Start a new test session`, input he root URL for the service, and `Start`.\n\n## Common Mistakes\n\n- incorrect `conformsTo` in the Landing Page. This was added between STAC API 0.9 and 1.0. It should be the same as the value in the `conformsTo` in the OAFeat `/conformance` endpoint.\n- OGC API Features uses `data` relation link relation at the root to point to the Collections endpoint (`/collections`), not `collections` relation\n- media type for link relation `service-desc` and endpoint is `application/vnd.oai.openapi+json;version=3.0` (not `application/json`) and link relation `search` and endpoint is `application/geo+json` (not `application/json`)\n- Use of OCG API "req" urls instead of "conf" urls, e.g. `http://www.opengis.net/spec/ogcapi-features-1/1.0/conf/core` should be used, not `http://www.opengis.net/spec/ogcapi-features-1/1.0/req/core`\n\n## License\n\nDistributed under the terms of the [Apache 2.0 license][license],\n_STAC API Validator_ is free and open source software.\n\n## Issues\n\nIf you encounter any problems,\nplease [file an issue] along with a detailed description.\n\n## Credits\n\nThis project was generated from [@cjolowicz]\'s [Hypermodern Python Cookiecutter] template.\n\n[@cjolowicz]: https://github.com/cjolowicz\n[pypi]: https://pypi.org/\n[hypermodern python cookiecutter]: https://github.com/cjolowicz/cookiecutter-hypermodern-python\n[file an issue]: https://github.com/stac-utils/stac-api-validator/issues\n[pip]: https://pip.pypa.io/\n\n<!-- github-only -->\n\n[license]: https://github.com/stac-utils/stac-api-validator/blob/main/LICENSE\n[contributor guide]: https://github.com/stac-utils/stac-api-validator/blob/main/CONTRIBUTING.md\n[command-line reference]: https://stac-api-validator.readthedocs.io/en/latest/usage.html\n',
-    'author': 'Phil Varner',
-    'author_email': 'phil@philvarner.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/stac-utils/stac-api-validator',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.10,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

