# Comparing `tmp/chronus-0.2.2.tar.gz` & `tmp/chronus-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chronus-0.2.2.tar", max compression
+gzip compressed data, was "chronus-0.2.3.tar", max compression
```

## Comparing `chronus-0.2.2.tar` & `chronus-0.2.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1072 2023-02-28 09:33:02.453690 chronus-0.2.2/LICENSE
--rw-r--r--   0        0        0    10481 2023-04-17 11:01:17.462307 chronus-0.2.2/README.md
--rw-r--r--   0        0        0     1122 2023-04-21 06:57:23.169699 chronus-0.2.2/chronus/SystemIntegration/FileRepository.py
--rw-r--r--   0        0        0        1 2023-04-17 10:44:37.558827 chronus-0.2.2/chronus/SystemIntegration/__init__.py
--rw-r--r--   0        0        0     1977 2023-04-21 13:37:43.020958 chronus-0.2.2/chronus/SystemIntegration/cpu_info_service.py
--rw-r--r--   0        0        0     1551 2023-04-21 06:57:23.179206 chronus-0.2.2/chronus/SystemIntegration/hpcg.py
--rw-r--r--   0        0        0      200 2023-04-21 11:06:34.779261 chronus-0.2.2/chronus/SystemIntegration/repository.py
--rw-r--r--   0        0        0      330 2023-04-17 10:14:26.979910 chronus-0.2.2/chronus/__init__.py
--rw-r--r--   0        0        0     4044 2023-04-21 13:37:40.245593 chronus-0.2.2/chronus/__main__.py
--rw-r--r--   0        0        0     1497 2023-04-21 06:57:23.157333 chronus-0.2.2/chronus/cli/__init__.py
--rw-r--r--   0        0        0     1224 2023-04-21 13:37:43.015999 chronus-0.2.2/chronus/domain/Run.py
--rw-r--r--   0        0        0        0 2023-04-17 10:14:26.980936 chronus-0.2.2/chronus/domain/__init__.py
--rw-r--r--   0        0        0     2075 2023-04-21 13:37:43.018032 chronus-0.2.2/chronus/domain/benchmark_service.py
--rw-r--r--   0        0        0      975 2023-04-21 13:37:40.293638 chronus-0.2.2/chronus/domain/configuration.py
--rw-r--r--   0        0        0        0 2023-04-21 06:56:28.522159 chronus-0.2.2/chronus/domain/interfaces/__init__.py
--rw-r--r--   0        0        0      163 2023-04-21 06:53:32.150630 chronus-0.2.2/chronus/domain/interfaces/application_runner_interface.py
--rw-r--r--   0        0        0       91 2023-04-21 06:54:31.741981 chronus-0.2.2/chronus/domain/interfaces/benchmark_run_repository_interface.py
--rw-r--r--   0        0        0      300 2023-04-21 13:37:42.986739 chronus-0.2.2/chronus/domain/interfaces/cpu_info_service_interface.py
--rw-r--r--   0        0        0      137 2023-04-21 06:56:09.236466 chronus-0.2.2/chronus/domain/interfaces/system_service_interface.py
--rw-r--r--   0        0        0      146 2023-04-21 06:38:37.130694 chronus-0.2.2/chronus/domain/system_sample.py
--rw-r--r--   0        0        0      313 2023-02-28 09:33:02.456874 chronus-0.2.2/chronus/example.py
--rw-r--r--   0        0        0        0 2023-04-17 10:32:37.222095 chronus-0.2.2/chronus/model/__init__.py
--rw-r--r--   0        0        0     2092 2023-04-21 06:57:22.994327 chronus-0.2.2/chronus/model/svm.py
--rw-r--r--   0        0        0     3611 2023-04-21 13:41:43.715379 chronus-0.2.2/pyproject.toml
--rw-r--r--   0        0        0    11620 1970-01-01 00:00:00.000000 chronus-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-02-28 09:33:02.453690 chronus-0.2.3/LICENSE
+-rw-r--r--   0        0        0    10481 2023-04-17 11:01:17.462307 chronus-0.2.3/README.md
+-rw-r--r--   0        0        0     1122 2023-04-21 06:57:23.169699 chronus-0.2.3/chronus/SystemIntegration/FileRepository.py
+-rw-r--r--   0        0        0        1 2023-04-17 10:44:37.558827 chronus-0.2.3/chronus/SystemIntegration/__init__.py
+-rw-r--r--   0        0        0     1781 2023-04-23 12:23:42.096207 chronus-0.2.3/chronus/SystemIntegration/cpu_info_service.py
+-rw-r--r--   0        0        0     1551 2023-04-21 06:57:23.179206 chronus-0.2.3/chronus/SystemIntegration/hpcg.py
+-rw-r--r--   0        0        0      200 2023-04-21 11:06:34.779261 chronus-0.2.3/chronus/SystemIntegration/repository.py
+-rw-r--r--   0        0        0      330 2023-04-17 10:14:26.979910 chronus-0.2.3/chronus/__init__.py
+-rw-r--r--   0        0        0     4251 2023-04-21 13:45:31.416762 chronus-0.2.3/chronus/__main__.py
+-rw-r--r--   0        0        0     1497 2023-04-21 06:57:23.157333 chronus-0.2.3/chronus/cli/__init__.py
+-rw-r--r--   0        0        0     1224 2023-04-21 13:37:43.015999 chronus-0.2.3/chronus/domain/Run.py
+-rw-r--r--   0        0        0        0 2023-04-17 10:14:26.980936 chronus-0.2.3/chronus/domain/__init__.py
+-rw-r--r--   0        0        0     2075 2023-04-21 13:37:43.018032 chronus-0.2.3/chronus/domain/benchmark_service.py
+-rw-r--r--   0        0        0      975 2023-04-21 13:37:40.293638 chronus-0.2.3/chronus/domain/configuration.py
+-rw-r--r--   0        0        0        0 2023-04-21 06:56:28.522159 chronus-0.2.3/chronus/domain/interfaces/__init__.py
+-rw-r--r--   0        0        0      163 2023-04-21 06:53:32.150630 chronus-0.2.3/chronus/domain/interfaces/application_runner_interface.py
+-rw-r--r--   0        0        0       91 2023-04-21 06:54:31.741981 chronus-0.2.3/chronus/domain/interfaces/benchmark_run_repository_interface.py
+-rw-r--r--   0        0        0      300 2023-04-21 13:37:42.986739 chronus-0.2.3/chronus/domain/interfaces/cpu_info_service_interface.py
+-rw-r--r--   0        0        0      137 2023-04-21 06:56:09.236466 chronus-0.2.3/chronus/domain/interfaces/system_service_interface.py
+-rw-r--r--   0        0        0      146 2023-04-21 06:38:37.130694 chronus-0.2.3/chronus/domain/system_sample.py
+-rw-r--r--   0        0        0      313 2023-02-28 09:33:02.456874 chronus-0.2.3/chronus/example.py
+-rw-r--r--   0        0        0        0 2023-04-17 10:32:37.222095 chronus-0.2.3/chronus/model/__init__.py
+-rw-r--r--   0        0        0     2092 2023-04-21 06:57:22.994327 chronus-0.2.3/chronus/model/svm.py
+-rw-r--r--   0        0        0     3611 2023-04-23 12:37:07.821085 chronus-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0    11620 1970-01-01 00:00:00.000000 chronus-0.2.3/PKG-INFO
```

### Comparing `chronus-0.2.2/LICENSE` & `chronus-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `chronus-0.2.2/README.md` & `chronus-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `chronus-0.2.2/chronus/SystemIntegration/FileRepository.py` & `chronus-0.2.3/chronus/SystemIntegration/FileRepository.py`

 * *Files identical despite different names*

### Comparing `chronus-0.2.2/chronus/SystemIntegration/cpu_info_service.py` & `chronus-0.2.3/chronus/SystemIntegration/cpu_info_service.py`

 * *Files 18% similar despite different names*

```diff
@@ -19,33 +19,28 @@
 
         if model_name is None:
             return CpuInfo("Unknown")
 
         return CpuInfo(model_name.group(1))
 
     def get_frequencies(self) -> List[float]:
-        output = subprocess.run(
-            "cat /sys/devices/system/cpu/cpu*/cpufreq/scaling_available_frequencies",
-            stdout=subprocess.PIPE,
-            stderr=subprocess.PIPE,
-            text=True,
-        )
 
-        if output.returncode != 0:
+        try:
+            file = open("/sys/devices/system/cpu/cpu0/cpufreq/scaling_available_frequencies", "r")
+            output = file.read()
+            file.close()
+        except IOError:
             raise RuntimeError(
                 "Failed to read /sys/devices/system/cpu/cpu*/cpufreq/scaling_available_frequencies"
             )
 
-        rows = output.stdout.split("\n")
-        frequencies_str = [row.split(" ") for row in rows]
+        # Regex that finds all frequencies
+        frequencies = re.findall(r"(\d+)", output)
 
-        # find the intersection of all the frequencies
-        intersection = set.intersection(*map(set, frequencies_str))
-
-        frequencies = [float(frequency) for frequency in intersection]
+        frequencies = [float(frequency) for frequency in frequencies]
         frequencies.sort()
 
         return frequencies
 
     def get_cores(self) -> int:
         output = subprocess.run("lscpu", stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True)
```

### Comparing `chronus-0.2.2/chronus/SystemIntegration/hpcg.py` & `chronus-0.2.3/chronus/SystemIntegration/hpcg.py`

 * *Files identical despite different names*

### Comparing `chronus-0.2.2/chronus/__main__.py` & `chronus-0.2.3/chronus/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -147,15 +147,22 @@
         "frequency": 2_200_000,
     }
 
     print(json.dumps(config))
 
 
 @app.command(name="cpu")
-def debug():
+def debug(print_version: bool = typer.Option(
+        None,
+        "-v",
+        "--version",
+        callback=version_callback,
+        is_eager=True,
+        help="Prints the version of the chronus package.",
+    )):
     cpu_service = LsCpuInfoService()
     pprint(f"CPU:         {cpu_service.get_cpu_info().cpu}")
     pprint(f"Frequencies: {cpu_service.get_frequencies()}")
     pprint(f"Cores:       {cpu_service.get_cores()}")
 
 
 if __name__ == "__main__":
```

### Comparing `chronus-0.2.2/chronus/cli/__init__.py` & `chronus-0.2.3/chronus/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `chronus-0.2.2/chronus/domain/Run.py` & `chronus-0.2.3/chronus/domain/Run.py`

 * *Files identical despite different names*

### Comparing `chronus-0.2.2/chronus/domain/benchmark_service.py` & `chronus-0.2.3/chronus/domain/benchmark_service.py`

 * *Files identical despite different names*

### Comparing `chronus-0.2.2/chronus/domain/configuration.py` & `chronus-0.2.3/chronus/domain/configuration.py`

 * *Files identical despite different names*

### Comparing `chronus-0.2.2/chronus/model/svm.py` & `chronus-0.2.3/chronus/model/svm.py`

 * *Files identical despite different names*

### Comparing `chronus-0.2.2/pyproject.toml` & `chronus-0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Poetry pyproject.toml: https://python-poetry.org/docs/pyproject/
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "chronus"
-version = "0.2.2"
+version = "0.2.3"
 description = "A energy scheduling model, build for HPC."
 readme = "README.md"
 authors = ["chronus <aaspringborg@gmail.com>"]
 license = "MIT"
 repository = "https://github.com/AndersSpringborg/chronus"
 homepage = "https://github.com/AndersSpringborg/chronus"
```

### Comparing `chronus-0.2.2/PKG-INFO` & `chronus-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chronus
-Version: 0.2.2
+Version: 0.2.3
 Summary: A energy scheduling model, build for HPC.
 Home-page: https://github.com/AndersSpringborg/chronus
 License: MIT
 Author: chronus
 Author-email: aaspringborg@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
```

