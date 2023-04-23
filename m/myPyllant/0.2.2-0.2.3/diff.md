# Comparing `tmp/mypyllant-0.2.2.tar.gz` & `tmp/mypyllant-0.2.3.tar.gz`

## Comparing `mypyllant-0.2.2.tar` & `mypyllant-0.2.3.tar`

### file list

```diff
@@ -1,33 +1,37 @@
--rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 mypyllant-0.2.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0    45426 2020-02-02 00:00:00.000000 mypyllant-0.2.2/logo.png
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 mypyllant-0.2.2/requirements-dev.txt
--rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 mypyllant-0.2.2/setup.cfg
--rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 mypyllant-0.2.2/.github/workflows/build-test.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mypyllant-0.2.2/src/myPyllant/__init__.py
--rw-r--r--   0        0        0    15667 2020-02-02 00:00:00.000000 mypyllant-0.2.2/src/myPyllant/api.py
--rw-r--r--   0        0        0     1888 2020-02-02 00:00:00.000000 mypyllant-0.2.2/src/myPyllant/const.py
--rwxr-xr-x   0        0        0     2687 2020-02-02 00:00:00.000000 mypyllant-0.2.2/src/myPyllant/export.py
--rw-r--r--   0        0        0     7731 2020-02-02 00:00:00.000000 mypyllant-0.2.2/src/myPyllant/models.py
--rw-r--r--   0        0        0     1935 2020-02-02 00:00:00.000000 mypyllant-0.2.2/src/myPyllant/sample.py
--rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 mypyllant-0.2.2/src/myPyllant/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mypyllant-0.2.2/tests/__init__.py
--rw-r--r--   0        0        0     2115 2020-02-02 00:00:00.000000 mypyllant-0.2.2/tests/conftest.py
--rwxr-xr-x   0        0        0     1060 2020-02-02 00:00:00.000000 mypyllant-0.2.2/tests/find_countries.py
--rw-r--r--   0        0        0     4742 2020-02-02 00:00:00.000000 mypyllant-0.2.2/tests/generate_test_data.py
--rw-r--r--   0        0        0     3484 2020-02-02 00:00:00.000000 mypyllant-0.2.2/tests/test_api.py
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 mypyllant-0.2.2/tests/test_countries.py
--rw-r--r--   0        0        0     4866 2020-02-02 00:00:00.000000 mypyllant-0.2.2/tests/test_generate_test_data.py
--rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 mypyllant-0.2.2/tests/json/064876fe84e6a872c97ac79ba1c2a7c71ff974ca/current_system.json
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 mypyllant-0.2.2/tests/json/064876fe84e6a872c97ac79ba1c2a7c71ff974ca/device_buckets.json
--rw-r--r--   0        0        0     6159 2020-02-02 00:00:00.000000 mypyllant-0.2.2/tests/json/064876fe84e6a872c97ac79ba1c2a7c71ff974ca/systems.json
--rw-r--r--   0        0        0     2783 2020-02-02 00:00:00.000000 mypyllant-0.2.2/tests/json/1cb8b8ad6bbd158eaca1527b3d5f852b8b473c0c/current_system.json
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 mypyllant-0.2.2/tests/json/1cb8b8ad6bbd158eaca1527b3d5f852b8b473c0c/device_buckets.json
--rw-r--r--   0        0        0     6354 2020-02-02 00:00:00.000000 mypyllant-0.2.2/tests/json/1cb8b8ad6bbd158eaca1527b3d5f852b8b473c0c/systems.json
--rw-r--r--   0        0        0     2783 2020-02-02 00:00:00.000000 mypyllant-0.2.2/tests/json/d121ac4dd73851053d557b1f8b6126bb1bf71a25/current_system.json
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 mypyllant-0.2.2/tests/json/d121ac4dd73851053d557b1f8b6126bb1bf71a25/device_buckets.json
--rw-r--r--   0        0        0     6400 2020-02-02 00:00:00.000000 mypyllant-0.2.2/tests/json/d121ac4dd73851053d557b1f8b6126bb1bf71a25/systems.json
--rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 mypyllant-0.2.2/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 mypyllant-0.2.2/LICENSE
--rw-r--r--   0        0        0     4617 2020-02-02 00:00:00.000000 mypyllant-0.2.2/README.md
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 mypyllant-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     5223 2020-02-02 00:00:00.000000 mypyllant-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 mypyllant-0.2.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    45426 2020-02-02 00:00:00.000000 mypyllant-0.2.3/logo.png
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 mypyllant-0.2.3/requirements-dev.txt
+-rwxr-xr-x   0        0        0      195 2020-02-02 00:00:00.000000 mypyllant-0.2.3/run_pytest.sh
+-rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 mypyllant-0.2.3/.github/workflows/build-test.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mypyllant-0.2.3/src/myPyllant/__init__.py
+-rw-r--r--   0        0        0    15957 2020-02-02 00:00:00.000000 mypyllant-0.2.3/src/myPyllant/api.py
+-rw-r--r--   0        0        0     1888 2020-02-02 00:00:00.000000 mypyllant-0.2.3/src/myPyllant/const.py
+-rwxr-xr-x   0        0        0     2687 2020-02-02 00:00:00.000000 mypyllant-0.2.3/src/myPyllant/export.py
+-rw-r--r--   0        0        0     7738 2020-02-02 00:00:00.000000 mypyllant-0.2.3/src/myPyllant/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mypyllant-0.2.3/src/myPyllant/py.typed
+-rw-r--r--   0        0        0     1882 2020-02-02 00:00:00.000000 mypyllant-0.2.3/src/myPyllant/sample.py
+-rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 mypyllant-0.2.3/src/myPyllant/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mypyllant-0.2.3/src/myPyllant/tests/__init__.py
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 mypyllant-0.2.3/src/myPyllant/tests/conftest.py
+-rwxr-xr-x   0        0        0      934 2020-02-02 00:00:00.000000 mypyllant-0.2.3/src/myPyllant/tests/find_countries.py
+-rw-r--r--   0        0        0     4812 2020-02-02 00:00:00.000000 mypyllant-0.2.3/src/myPyllant/tests/generate_test_data.py
+-rw-r--r--   0        0        0     7177 2020-02-02 00:00:00.000000 mypyllant-0.2.3/src/myPyllant/tests/test_api.py
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 mypyllant-0.2.3/src/myPyllant/tests/test_countries.py
+-rw-r--r--   0        0        0     4861 2020-02-02 00:00:00.000000 mypyllant-0.2.3/src/myPyllant/tests/test_generate_test_data.py
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 mypyllant-0.2.3/src/myPyllant/tests/test_sample.py
+-rwxr-xr-x   0        0        0      655 2020-02-02 00:00:00.000000 mypyllant-0.2.3/src/myPyllant/tests/update_sample.py
+-rw-r--r--   0        0        0     3983 2020-02-02 00:00:00.000000 mypyllant-0.2.3/src/myPyllant/tests/utils.py
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 mypyllant-0.2.3/src/myPyllant/tests/json/064876fe84e6a872c97ac79ba1c2a7c71ff974ca/current_system.json
+-rw-r--r--   0        0        0      552 2020-02-02 00:00:00.000000 mypyllant-0.2.3/src/myPyllant/tests/json/064876fe84e6a872c97ac79ba1c2a7c71ff974ca/device_buckets.json
+-rw-r--r--   0        0        0     6159 2020-02-02 00:00:00.000000 mypyllant-0.2.3/src/myPyllant/tests/json/064876fe84e6a872c97ac79ba1c2a7c71ff974ca/systems.json
+-rw-r--r--   0        0        0     2783 2020-02-02 00:00:00.000000 mypyllant-0.2.3/src/myPyllant/tests/json/1cb8b8ad6bbd158eaca1527b3d5f852b8b473c0c/current_system.json
+-rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 mypyllant-0.2.3/src/myPyllant/tests/json/1cb8b8ad6bbd158eaca1527b3d5f852b8b473c0c/device_buckets.json
+-rw-r--r--   0        0        0     6354 2020-02-02 00:00:00.000000 mypyllant-0.2.3/src/myPyllant/tests/json/1cb8b8ad6bbd158eaca1527b3d5f852b8b473c0c/systems.json
+-rw-r--r--   0        0        0     2783 2020-02-02 00:00:00.000000 mypyllant-0.2.3/src/myPyllant/tests/json/d121ac4dd73851053d557b1f8b6126bb1bf71a25/current_system.json
+-rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 mypyllant-0.2.3/src/myPyllant/tests/json/d121ac4dd73851053d557b1f8b6126bb1bf71a25/device_buckets.json
+-rw-r--r--   0        0        0     6400 2020-02-02 00:00:00.000000 mypyllant-0.2.3/src/myPyllant/tests/json/d121ac4dd73851053d557b1f8b6126bb1bf71a25/systems.json
+-rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 mypyllant-0.2.3/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 mypyllant-0.2.3/LICENSE
+-rw-r--r--   0        0        0     4581 2020-02-02 00:00:00.000000 mypyllant-0.2.3/README.md
+-rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 mypyllant-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     5187 2020-02-02 00:00:00.000000 mypyllant-0.2.3/PKG-INFO
```

### Comparing `mypyllant-0.2.2/.pre-commit-config.yaml` & `mypyllant-0.2.3/.pre-commit-config.yaml`

 * *Files 19% similar despite different names*

```diff
@@ -7,35 +7,71 @@
   - repo: https://github.com/psf/black
     rev: 23.1.0
     hooks:
       - id: black
         args:
           - --safe
           - --quiet
-        files: ^((src|tests)/.+)?[^/]+\.py$
   - repo: https://github.com/codespell-project/codespell
     rev: v2.2.2
     hooks:
       - id: codespell
         args:
           - --ignore-words-list=hass,alot,datas,dof,dur,farenheit,hist,iff,ines,ist,lightsensor,mut,nd,pres,referer,ser,serie,te,technik,ue,uint,visability,wan,wanna,withing
           - --skip="./.*,*.csv,*.json"
           - --quiet-level=2
         exclude_types: [csv, json]
+  - repo: https://github.com/pycqa/flake8
+    rev: 6.0.0
+    hooks:
+      - id: flake8
+        entry: pflake8
+        additional_dependencies:
+          - pydocstyle==5.0.2
+          - pyproject-flake8==6.0.0
+  - repo: https://github.com/PyCQA/bandit
+    rev: 1.7.4
+    hooks:
+      - id: bandit
+        args:
+          - --quiet
+          - --format=custom
+          - -lll
   - repo: https://github.com/pre-commit/mirrors-isort
     rev: v5.10.1
     hooks:
       - id: isort
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.4.0
     hooks:
       - id: check-executables-have-shebangs
-        stages: [manual]
       - id: check-json
   - repo: https://github.com/pre-commit/mirrors-mypy
     rev: v1.0.1
     hooks:
       - id: mypy
         args:
           - --pretty
           - --show-error-codes
           - --show-error-context
+        additional_dependencies:
+          - aiohttp
+          - aioresponses
+          - freezegun
+          - pydantic
+          - pytest
+          - types-requests
+  - repo: local
+    hooks:
+      - id: update-sample
+        name: update-sample
+        entry: python src/myPyllant/tests/update_sample.py
+        language: python
+        pass_filenames: false
+  - repo: local
+    hooks:
+    - id: pytest
+      name: pytest
+      entry: run_pytest.sh --no-cov
+      language: script
+      pass_filenames: false
+      always_run: true
```

### Comparing `mypyllant-0.2.2/logo.png` & `mypyllant-0.2.3/logo.png`

 * *Files identical despite different names*

### Comparing `mypyllant-0.2.2/.github/workflows/build-test.yaml` & `mypyllant-0.2.3/.github/workflows/build-test.yaml`

 * *Files 19% similar despite different names*

```diff
@@ -11,19 +11,23 @@
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v3
       - name: Set up Python
         uses: actions/setup-python@v4
         with:
           python-version: "3.10"
+          cache: pip
+          cache-dependency-path: requirements-dev.txt
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           pip install -r requirements-dev.txt
       - uses: pre-commit/action@v3.0.0
+        env:
+          SKIP: pytest
       - name: set pythonpath
         run: |
           echo "PYTHONPATH=${PYTHONPATH}:${PWD}/src" >> $GITHUB_ENV
       - name: Test with pytest
         run: |
           pytest
       - name: Build a binary wheel and a source tarball
```

### Comparing `mypyllant-0.2.2/src/myPyllant/api.py` & `mypyllant-0.2.3/src/myPyllant/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
-from collections.abc import AsyncGenerator
 import datetime
-from html import unescape
 import logging
 import re
+from collections.abc import AsyncGenerator
+from html import unescape
 from urllib.parse import parse_qs, urlencode, urlparse
 
 import aiohttp
 from aiohttp import ClientResponseError
 
 from myPyllant.const import (
     API_URL_BASE,
@@ -55,17 +55,17 @@
     """
     See https://docs.aiohttp.org/en/stable/tracing_reference.html#aiohttp.TraceConfig.on_request_end
     """
     logger.debug(f"Got response {await params.response.text()}")
 
 
 class MyPyllantAPI:
-    username: str = None
-    password: str = None
-    aiohttp_session: aiohttp.ClientSession = None
+    username: str
+    password: str
+    aiohttp_session: aiohttp.ClientSession
     oauth_session: dict = {}
     oauth_session_expires: datetime.datetime | None = None
 
     def __init__(self, username: str, password: str, country: str, brand: str) -> None:
         if brand not in BRANDS.keys():
             raise ValueError(
                 f"Invalid brand, must be one of {', '.join(BRANDS.keys())}"
@@ -261,16 +261,24 @@
         self,
         device: Device,
         data_resolution: DeviceDataBucketResolution = DeviceDataBucketResolution.DAY,
         data_from: datetime.datetime | None = None,
         data_to: datetime.datetime | None = None,
     ) -> AsyncGenerator[DeviceData, None]:
         for data in device.data:
-            start_date = datetime_format(data_from if data_from else data.data_from)
-            end_date = datetime_format(data_to if data_to else data.data_to)
+            data_from = data_from or data.data_from
+            if not data_from:
+                raise ValueError(
+                    "No data_from set, and no data_from found in device data"
+                )
+            data_to = data_to or data.data_to
+            if not data_to:
+                raise ValueError("No data_to set, and no data_to found in device data")
+            start_date = datetime_format(data_from)
+            end_date = datetime_format(data_to)
             querystring = {
                 "resolution": str(data_resolution),
                 "operationMode": data.operation_mode,
                 "energyType": data.value_type,
                 "startDate": start_date,
                 "endDate": end_date,
             }
@@ -378,15 +386,15 @@
             url, headers=self.get_authorized_headers()
         )
 
     async def set_domestic_hot_water_temperature(
         self, domestic_hot_water: DomesticHotWater, temperature: int | float
     ):
         if isinstance(temperature, float):
-            logger.warning(f"Domestic hot water can only be set to whole numbers")
+            logger.warning("Domestic hot water can only be set to whole numbers")
             temperature = int(round(temperature, 0))
         url = (
             f"{API_URL_BASE}/systems/{domestic_hot_water.system_id}/"
             f"domesticHotWater/{domestic_hot_water.index}/temperature"
         )
         return await self.aiohttp_session.post(
             url, json={"setPoint": temperature}, headers=self.get_authorized_headers()
```

### Comparing `mypyllant-0.2.2/src/myPyllant/const.py` & `mypyllant-0.2.3/src/myPyllant/const.py`

 * *Files identical despite different names*

### Comparing `mypyllant-0.2.2/src/myPyllant/export.py` & `mypyllant-0.2.3/src/myPyllant/export.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python3
 
 import argparse
 import asyncio
-from datetime import datetime
 import json
 import sys
+from datetime import datetime
 
 from myPyllant.api import MyPyllantAPI
 from myPyllant.const import BRANDS, COUNTRIES, DEFAULT_BRAND
 from myPyllant.models import DeviceDataBucketResolution
 
 parser = argparse.ArgumentParser(description="Export data from myVaillant API.")
 parser.add_argument("user", help="Username (email address) for the myVaillant app")
```

### Comparing `mypyllant-0.2.2/src/myPyllant/models.py` & `mypyllant-0.2.3/src/myPyllant/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import datetime
-from enum import Enum
 import logging
+from enum import Enum
 from typing import Any
 
 from pydantic import BaseModel
 
 logger = logging.getLogger(__name__)
 
 
@@ -249,15 +249,15 @@
 class DeviceDataBucket(BaseModel):
     start_date: datetime.datetime
     end_date: datetime.datetime
     value: float
 
 
 class DeviceData(BaseModel):
-    def __init__(self, device: Device = None, **kwargs: Any) -> None:
+    def __init__(self, device: Device | None = None, **kwargs: Any) -> None:
         kwargs["data_from"] = kwargs.pop("from") if "from" in kwargs else None
         kwargs["data_to"] = kwargs.pop("to") if "to" in kwargs else None
         super().__init__(device=device, **kwargs)
 
     device: Device | None
     data_from: datetime.datetime | None
     data_to: datetime.datetime | None
```

### Comparing `mypyllant-0.2.2/src/myPyllant/sample.py` & `mypyllant-0.2.3/src/myPyllant/sample.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+#!/usr/bin/env python3
+
 import argparse
 import asyncio
 from datetime import datetime, timedelta
 
 from myPyllant.api import MyPyllantAPI
 from myPyllant.const import BRANDS, COUNTRIES, DEFAULT_BRAND
 
@@ -20,21 +22,19 @@
     choices=BRANDS.keys(),
 )
 
 
 async def main(user, password, country, brand):
     async with MyPyllantAPI(user, password, country, brand) as api:
         async for system in api.get_systems():
-            print(await api.set_holiday(system, datetime.now()))
+            print(await api.set_holiday(system))
             print(
-                await (
-                    await api.set_holiday(
-                        system, datetime.now(), datetime.now() + timedelta(days=1)
-                    )
-                ).json()
+                await api.set_holiday(
+                    system, datetime.now(), datetime.now() + timedelta(days=7)
+                )
             )
             print(await api.cancel_holiday(system))
             print(await api.boost_domestic_hot_water(system.domestic_hot_water[0]))
             print(await api.cancel_hot_water_boost(system.domestic_hot_water[0]))
             print(
                 await api.set_domestic_hot_water_temperature(
                     system.domestic_hot_water[0], 46
```

### Comparing `mypyllant-0.2.2/src/myPyllant/utils.py` & `mypyllant-0.2.3/src/myPyllant/utils.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import base64
-from datetime import datetime
 import hashlib
 import random
 import re
 import string
+from datetime import datetime
 
 
 def dict_to_snake_case(d):
     """
     Convert {'camelCase': value} to {'camel_case': value} recursively
     """
```

### Comparing `mypyllant-0.2.2/tests/generate_test_data.py` & `mypyllant-0.2.3/src/myPyllant/tests/generate_test_data.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 #!/usr/bin/env python3
 
 import argparse
 import asyncio
 import copy
-from datetime import datetime, timedelta
 import hashlib
 import json
 import logging
-from pathlib import Path
 import secrets
-import sys
+from datetime import datetime, timedelta
+from pathlib import Path
 from urllib.parse import urlencode
 
-logger = logging.getLogger(__name__)
+from myPyllant.const import BRANDS, COUNTRIES, DEFAULT_BRAND
 
-sys.path.append((Path(__file__).resolve().parent / "src").name)
+logger = logging.getLogger(__name__)
 
-from myPyllant.const import BRANDS, COUNTRIES, DEFAULT_BRAND
 
 parser = argparse.ArgumentParser(
     description="Generates test data necessary to run integration tests."
 )
 parser.add_argument("user", help="Username (email address) for the myVaillant app")
 parser.add_argument("password", help="Password for the myVaillant app")
 parser.add_argument(
@@ -52,22 +50,26 @@
 async def main(user, password, country, brand):
     """
     Generate json data for running testcases.
 
     :param user:
     :param password:
     :param country:
+    :param brand:
     :return:
     """
     from myPyllant.api import MyPyllantAPI
     from myPyllant.const import API_URL_BASE
     from myPyllant.models import DeviceDataBucketResolution
     from myPyllant.utils import datetime_format
 
-    user_json_dir = JSON_DIR / hashlib.sha1(user.encode("UTF-8") + SALT).hexdigest()
+    user_json_dir = (
+        JSON_DIR
+        / hashlib.sha1(user.encode("UTF-8") + SALT, usedforsecurity=False).hexdigest()
+    )
     user_json_dir.mkdir(parents=True, exist_ok=True)
 
     async with MyPyllantAPI(user, password, country, brand) as api:
         systems_url = f"{API_URL_BASE}/systems"
         async with api.aiohttp_session.get(
             systems_url, headers=api.get_authorized_headers()
         ) as systems_resp:
@@ -109,23 +111,27 @@
             device_buckets_url, headers=api.get_authorized_headers()
         ) as device_buckets_resp:
             with open(user_json_dir / "device_buckets.json", "w") as fh:
                 device_buckets = await device_buckets_resp.json()
                 fh.write(json.dumps(device_buckets, indent=2))
 
 
-def _recursive_data_anonymize(data: str | dict | list, salt: bytes = b"") -> dict:
+def _recursive_data_anonymize(
+    data: str | dict | list, salt: bytes = b""
+) -> str | dict | list:
     if isinstance(data, list):
         for elem in data:
             _recursive_data_anonymize(elem, salt)
 
     elif isinstance(data, dict):
         for elem in data.keys():
             if elem in ANONYMIZE_ATTRIBUTES:
-                data[elem] = hashlib.sha1(data[elem].encode("UTF-8") + salt).hexdigest()
+                data[elem] = hashlib.sha1(
+                    data[elem].encode("UTF-8") + salt, usedforsecurity=False
+                ).hexdigest()
                 continue
             _recursive_data_anonymize(data[elem], salt)
 
     return data
 
 
 if __name__ == "__main__":
```

### Comparing `mypyllant-0.2.2/tests/test_generate_test_data.py` & `mypyllant-0.2.3/src/myPyllant/tests/test_generate_test_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from tests.generate_test_data import _recursive_data_anonymize
+from .generate_test_data import _recursive_data_anonymize
 
 
 def test_anonymize_systems_data():
     original_systems_data = [
         {
             "gateway": {
                 "deviceId": "PRIVATE_deviceId",
```

### Comparing `mypyllant-0.2.2/tests/json/064876fe84e6a872c97ac79ba1c2a7c71ff974ca/current_system.json` & `mypyllant-0.2.3/src/myPyllant/tests/json/064876fe84e6a872c97ac79ba1c2a7c71ff974ca/current_system.json`

 * *Files identical despite different names*

### Comparing `mypyllant-0.2.2/tests/json/064876fe84e6a872c97ac79ba1c2a7c71ff974ca/systems.json` & `mypyllant-0.2.3/src/myPyllant/tests/json/064876fe84e6a872c97ac79ba1c2a7c71ff974ca/systems.json`

 * *Files identical despite different names*

### Comparing `mypyllant-0.2.2/tests/json/1cb8b8ad6bbd158eaca1527b3d5f852b8b473c0c/current_system.json` & `mypyllant-0.2.3/src/myPyllant/tests/json/1cb8b8ad6bbd158eaca1527b3d5f852b8b473c0c/current_system.json`

 * *Files identical despite different names*

### Comparing `mypyllant-0.2.2/tests/json/1cb8b8ad6bbd158eaca1527b3d5f852b8b473c0c/systems.json` & `mypyllant-0.2.3/src/myPyllant/tests/json/1cb8b8ad6bbd158eaca1527b3d5f852b8b473c0c/systems.json`

 * *Files identical despite different names*

### Comparing `mypyllant-0.2.2/tests/json/d121ac4dd73851053d557b1f8b6126bb1bf71a25/current_system.json` & `mypyllant-0.2.3/src/myPyllant/tests/json/d121ac4dd73851053d557b1f8b6126bb1bf71a25/current_system.json`

 * *Files identical despite different names*

### Comparing `mypyllant-0.2.2/tests/json/d121ac4dd73851053d557b1f8b6126bb1bf71a25/systems.json` & `mypyllant-0.2.3/src/myPyllant/tests/json/d121ac4dd73851053d557b1f8b6126bb1bf71a25/systems.json`

 * *Files identical despite different names*

### Comparing `mypyllant-0.2.2/.gitignore` & `mypyllant-0.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `mypyllant-0.2.2/LICENSE` & `mypyllant-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mypyllant-0.2.2/README.md` & `mypyllant-0.2.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -23,14 +23,16 @@
 
 The `--data` argument exports historical data of the devices in your system.
 Without this keyword, information about your system will be exported as JSON.
 
 ## Usage
 
 ```python
+#!/usr/bin/env python3
+
 import argparse
 import asyncio
 from datetime import datetime, timedelta
 
 from myPyllant.api import MyPyllantAPI
 from myPyllant.const import BRANDS, COUNTRIES, DEFAULT_BRAND
 
@@ -49,21 +51,19 @@
     choices=BRANDS.keys(),
 )
 
 
 async def main(user, password, country, brand):
     async with MyPyllantAPI(user, password, country, brand) as api:
         async for system in api.get_systems():
-            print(await api.set_holiday(system, datetime.now()))
+            print(await api.set_holiday(system))
             print(
-                await (
-                    await api.set_holiday(
-                        system, datetime.now(), datetime.now() + timedelta(days=1)
-                    )
-                ).json()
+                await api.set_holiday(
+                    system, datetime.now(), datetime.now() + timedelta(days=7)
+                )
             )
             print(await api.cancel_holiday(system))
             print(await api.boost_domestic_hot_water(system.domestic_hot_water[0]))
             print(await api.cancel_hot_water_boost(system.domestic_hot_water[0]))
             print(
                 await api.set_domestic_hot_water_temperature(
                     system.domestic_hot_water[0], 46
@@ -92,14 +92,15 @@
 
 I'm happy to accept PRs, if you run the pre-commit checks and test your changes:
 
 ```shell
 python3 -m venv .venv
 source .venv/bin/activate
 pip install -r requirements-dev.txt
+pip install -e .
 pre-commit install
 pytest
 ```
 
 ### Supporting new Countries
 
 The myVAILLANT app uses Keycloak and OIDC for authentication, with a realm for each country and brand.
```

### Comparing `mypyllant-0.2.2/PKG-INFO` & `mypyllant-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myPyllant
-Version: 0.2.2
+Version: 0.2.3
 Summary: A Python library to interact with the API behind the myVAILLANT app
 Project-URL: Homepage, https://github.com/signalkraft/myPyllant
 Project-URL: Bug Tracker, https://github.com/signalkraft/myPyllant/issues
 Author-email: Philipp <pd@signalkraft.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -39,14 +39,16 @@
 
 The `--data` argument exports historical data of the devices in your system.
 Without this keyword, information about your system will be exported as JSON.
 
 ## Usage
 
 ```python
+#!/usr/bin/env python3
+
 import argparse
 import asyncio
 from datetime import datetime, timedelta
 
 from myPyllant.api import MyPyllantAPI
 from myPyllant.const import BRANDS, COUNTRIES, DEFAULT_BRAND
 
@@ -65,21 +67,19 @@
     choices=BRANDS.keys(),
 )
 
 
 async def main(user, password, country, brand):
     async with MyPyllantAPI(user, password, country, brand) as api:
         async for system in api.get_systems():
-            print(await api.set_holiday(system, datetime.now()))
+            print(await api.set_holiday(system))
             print(
-                await (
-                    await api.set_holiday(
-                        system, datetime.now(), datetime.now() + timedelta(days=1)
-                    )
-                ).json()
+                await api.set_holiday(
+                    system, datetime.now(), datetime.now() + timedelta(days=7)
+                )
             )
             print(await api.cancel_holiday(system))
             print(await api.boost_domestic_hot_water(system.domestic_hot_water[0]))
             print(await api.cancel_hot_water_boost(system.domestic_hot_water[0]))
             print(
                 await api.set_domestic_hot_water_temperature(
                     system.domestic_hot_water[0], 46
@@ -108,14 +108,15 @@
 
 I'm happy to accept PRs, if you run the pre-commit checks and test your changes:
 
 ```shell
 python3 -m venv .venv
 source .venv/bin/activate
 pip install -r requirements-dev.txt
+pip install -e .
 pre-commit install
 pytest
 ```
 
 ### Supporting new Countries
 
 The myVAILLANT app uses Keycloak and OIDC for authentication, with a realm for each country and brand.
```

