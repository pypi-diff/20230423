# Comparing `tmp/cpggen-0.9.6.tar.gz` & `tmp/cpggen-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cpggen-0.9.6.tar", max compression
+gzip compressed data, was "cpggen-1.0.0.tar", max compression
```

## Comparing `cpggen-0.9.6.tar` & `cpggen-1.0.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11357 2023-04-21 12:22:08.046902 cpggen-0.9.6/LICENSE
--rw-r--r--   0        0        0     7487 2023-04-21 12:22:08.046902 cpggen-0.9.6/README.md
--rw-r--r--   0        0        0        0 2023-04-21 12:22:08.046902 cpggen-0.9.6/cpggen/__init__.py
--rw-r--r--   0        0        0    13069 2023-04-21 12:22:08.046902 cpggen-0.9.6/cpggen/cli.py
--rw-r--r--   0        0        0    33093 2023-04-21 12:22:08.050902 cpggen-0.9.6/cpggen/executor.py
--rw-r--r--   0        0        0      746 2023-04-21 12:22:08.050902 cpggen-0.9.6/cpggen/logger.py
--rw-r--r--   0        0        0    11219 2023-04-21 12:22:08.050902 cpggen-0.9.6/cpggen/utils.py
--rw-r--r--   0        0        0     1245 2023-04-21 12:22:08.050902 cpggen-0.9.6/pyproject.toml
--rw-r--r--   0        0        0     8815 1970-01-01 00:00:00.000000 cpggen-0.9.6/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-22 22:10:12.484381 cpggen-1.0.0/LICENSE
+-rw-r--r--   0        0        0     7673 2023-04-22 22:10:12.484381 cpggen-1.0.0/README.md
+-rw-r--r--   0        0        0        0 2023-04-22 22:10:12.488381 cpggen-1.0.0/cpggen/__init__.py
+-rw-r--r--   0        0        0    13335 2023-04-22 22:10:12.488381 cpggen-1.0.0/cpggen/cli.py
+-rw-r--r--   0        0        0    33224 2023-04-22 22:10:12.488381 cpggen-1.0.0/cpggen/executor.py
+-rw-r--r--   0        0        0     1015 2023-04-22 22:10:12.488381 cpggen-1.0.0/cpggen/logger.py
+-rw-r--r--   0        0        0    11219 2023-04-22 22:10:12.488381 cpggen-1.0.0/cpggen/utils.py
+-rw-r--r--   0        0        0     1245 2023-04-22 22:10:12.488381 cpggen-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     9001 1970-01-01 00:00:00.000000 cpggen-1.0.0/PKG-INFO
```

### Comparing `cpggen-0.9.6/LICENSE` & `cpggen-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cpggen-0.9.6/README.md` & `cpggen-1.0.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -16,59 +16,34 @@
 - JDK 11 or above
 - Python 3.10
 - Docker or podman (Windows, Linux or Mac) or
 - Joern [natively installed](https://docs.joern.io/installation) (Linux only)
 
 ## Installation
 
-cpggen is available as a [PyPI package](https://pypi.org/project/cpggen/) or as a [container image](https://github.com/AppThreat/cpggen/pkgs/container/cpggen).
-
-```
-pip install cpggen
-```
-
-Bundled container image
-
-```
-docker pull ghcr.io/appthreat/cpggen
-# podman pull ghcr.io/appthreat/cpggen
-```
-
-Almalinux 9 requires the CPU to support SSE4.2. For kvm64 VM use the Almalinux 8 version instead.
-
-```
-docker pull ghcr.io/appthreat/cpggen-alma8
-# podman pull ghcr.io/appthreat/cpggen-alma8
-```
-
-Or use the nightly to always get the latest joern and tools.
-
-```
-docker pull ghcr.io/appthreat/cpggen:nightly
-# podman pull ghcr.io/appthreat/cpggen:nightly
-```
+cpggen is available as a single executable binary, [PyPI package](https://pypi.org/project/cpggen/) or as a [container image](https://github.com/AppThreat/cpggen/pkgs/container/cpggen).
 
 ### Single executable binaries
 
 Download the executable binary for your operating system from the [releases page](https://github.com/appthreat/cpggen/releases). These binary bundle the following:
 
 - Joern with all the CPG frontends
 - cpggen with Python 3.10
 - cdxgen with Node.js 18 - Generates SBoM
 
 ```bash
-curl -LO https://github.com/AppThreat/cpggen/releases/download/v0.9.6/cpggen-linux-amd64
+curl -LO https://github.com/AppThreat/cpggen/releases/download/v1.0.0/cpggen-linux-amd64
 chmod +x cpggen-linux-amd64
 ./cpggen-linux-amd64 --help
 ```
 
 On Windows,
 
 ```powershell
-curl -LO https://github.com/appthreat/cpggen/releases/download/v0.9.6/cpggen.exe
+curl -LO https://github.com/appthreat/cpggen/releases/download/v1.0.0/cpggen.exe
 .\cpggen.exe --help
 ```
 
 NOTE: On Windows, antivirus and antimalware could prevent this single executable from functioning properly. Depending on the system, administrative privileges might also be required. Use container-based execution as a fallback.
 
 ### OCI Artifacts via ORAS cli
 
@@ -84,14 +59,43 @@
 
 ```powershell
 Invoke-WebRequest -Uri https://github.com/oras-project/oras/releases/download/v1.0.0/oras_1.0.0_windows_amd64.zip -UseBasicParsing -OutFile oras_1.0.0_windows_amd64.zip
 Expand-Archive -Path oras_1.0.0_windows_amd64.zip -DestinationPath .
 oras.exe pull ghcr.io/appthreat/cpggen-windows-bin:v1
 ```
 
+### PyPI package
+
+This would install just the python cli tool without any CPG language frontends. Joern must be installed separately to make the cli work.
+
+```
+pip install cpggen
+```
+
+### Bundled container image
+
+```
+docker pull ghcr.io/appthreat/cpggen
+# podman pull ghcr.io/appthreat/cpggen
+```
+
+Almalinux 9 requires the CPU to support SSE4.2. For kvm64 VM use the Almalinux 8 version instead.
+
+```
+docker pull ghcr.io/appthreat/cpggen-alma8
+# podman pull ghcr.io/appthreat/cpggen-alma8
+```
+
+Or use the nightly to always get the latest joern and tools.
+
+```
+docker pull ghcr.io/appthreat/cpggen:nightly
+# podman pull ghcr.io/appthreat/cpggen:nightly
+```
+
 ## Usage
 
 To auto detect the language from the current directory and generate CPG.
 
 ```
 cpggen
 ```
```

### Comparing `cpggen-0.9.6/cpggen/cli.py` & `cpggen-1.0.0/cpggen/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import tempfile
 from multiprocessing import Pool, freeze_support
 from pathlib import Path, PurePath
 
 from quart import Quart, request
 
 from cpggen import executor, utils
-from cpggen.logger import LOG, console
+from cpggen.logger import LOG, console, enable_debug
 
 try:
     os.environ["PYTHONIOENCODING"] = "utf-8"
     os.environ["PYTHONUTF8"] = 1
 except Exception:
     pass
 
@@ -120,14 +120,21 @@
         help="Export format",
     )
     parser.add_argument(
         "--export-out-dir",
         dest="export_out_dir",
         help="Export output directoru",
     )
+    parser.add_argument(
+        "--verbose",
+        action="store_true",
+        default=False,
+        dest="verbose_mode",
+        help="Run cpggen in verbose mode",
+    )
     return parser.parse_args()
 
 
 @app.get("/")
 async def index():
     return {}
 
@@ -309,14 +316,17 @@
                 pool.terminate()
             pool.join()
 
 
 def main():
     print(product_logo)
     args = build_args()
+    # Turn on verbose mode
+    if args.verbose_mode:
+        enable_debug()
     if args.server_mode:
         return run_server(args)
     src = args.src
     cpg_out_dir = args.cpg_out_dir
     export_out_dir = args.export_out_dir
     if not src.startswith("http") and not src.startswith("git://"):
         src = str(PurePath(args.src))
```

### Comparing `cpggen-0.9.6/cpggen/executor.py` & `cpggen-1.0.0/cpggen/executor.py`

 * *Files 2% similar despite different names*

```diff
@@ -194,36 +194,38 @@
 
 qwiet_lang_map = {
     "jar": "java",
     "jsp": "java",
     "scala": "java",
     "java": "javasrc",
     "python": "pythonsrc",
-    "js": "javascriptsrc",
-    "ts": "javascriptsrc",
-    "javascript": "javascriptsrc",
-    "typescript": "javascriptsrc",
+    "js": "js",
+    "ts": "js",
+    "javascript": "js",
+    "typescript": "js",
     "go": "go",
     "csharp": "csharp",
     "dotnet": "csharp",
 }
 
 
-def qwiet_analysis(app_manifest, cwd, env):
+def qwiet_analysis(app_manifest, src, cwd, env):
     try:
+        relative_path = os.path.relpath(cwd, src)
+        if relative_path and not relative_path.startswith(".."):
+            os.environ["SL_VCS_RELATIVE_PATH"] = relative_path
+            env["SL_VCS_RELATIVE_PATH"] = relative_path
         LOG.info(f"Submitting {app_manifest['app']} for Qwiet.AI analysis")
         build_args = cpg_tools_map["qwiet"]
         policy = ""
         vcs_correction = ""
         if os.getenv("SHIFTLEFT_POLICY"):
             policy = f"""--policy {os.getenv("SHIFTLEFT_POLICY")} """
         elif os.getenv("ENABLE_BEST_PRACTICES") in ("true", "1"):
-            policy = (
-                """--policy io%(bin_ext)siftleft/defaultWithDictAndBestPractices """
-            )
+            policy = """--policy io.shiftleft/defaultWithDictAndBestPractices """
 
         if app_manifest.get("tool_lang"):
             if "jar" in app_manifest.get("tool_lang") or "jsp" in app_manifest.get(
                 "tool_lang"
             ):
                 vcs_correction = '--vcs-prefix-correction "*=src/main/java" '
             if "scala" in app_manifest.get("tool_lang"):
@@ -239,18 +241,18 @@
             cwd=cwd,
             env=env,
             check=False,
             shell=use_shell,
             encoding="utf-8",
         )
         if cp:
-            if LOG.isEnabledFor(DEBUG) and cp.stdout:
-                LOG.debug(cp.stdout)
+            if cp.stdout:
+                LOG.info(cp.stdout)
             if cp.returncode and cp.stderr:
-                LOG.info(cp.stderr)
+                LOG.warn(cp.stderr)
             else:
                 LOG.info(f"{app_manifest['app']} uploaded successfully")
     except Exception as e:
         LOG.error(e)
 
 
 def dot_convert(export_out_dir, env):
@@ -720,15 +722,15 @@
                         if os.getenv("SHIFTLEFT_ACCESS_TOKEN"):
                             progress.update(
                                 task,
                                 description="Uploading to Qwiet AI for analysis",
                                 completed=90,
                                 total=100,
                             )
-                            qwiet_analysis(app_manifest, cwd, env)
+                            qwiet_analysis(app_manifest, src, cwd, env)
                         json.dump(app_manifest, mfp)
                 else:
                     LOG.info(f"CPG {cpg_out} was not generated for {tool_lang}")
                     if not os.getenv("AT_DEBUG_MODE"):
                         LOG.info(
                             "Set the environment variable AT_DEBUG_MODE to debug to see the debug logs"
                         )
```

### Comparing `cpggen-0.9.6/cpggen/logger.py` & `cpggen-1.0.0/cpggen/logger.py`

 * *Files 22% similar despite different names*

```diff
@@ -22,13 +22,25 @@
     handlers=[
         RichHandler(
             console=console, markup=True, show_path=False, enable_link_path=False
         )
     ],
 )
 LOG = logging.getLogger(__name__)
+USE_DEBUG = False
 
 # Set logging level
-if os.getenv("AT_DEBUG_MODE") in ("debug", "true", "1"):
+if (
+    USE_DEBUG
+    or os.getenv("AT_DEBUG_MODE") in ("debug", "true", "1")
+    or os.getenv("SHIFTLEFT_VERBOSE")
+    or os.getenv("SHIFTLEFT_DIAGNOSTIC")
+):
     LOG.setLevel(logging.DEBUG)
 
 DEBUG = logging.DEBUG
+
+
+def enable_debug():
+    LOG.setLevel(logging.DEBUG)
+    os.environ["SHIFTLEFT_VERBOSE"] = "true"
+    os.environ["SHIFTLEFT_DIAGNOSTIC"] = "true"
```

### Comparing `cpggen-0.9.6/cpggen/utils.py` & `cpggen-1.0.0/cpggen/utils.py`

 * *Files identical despite different names*

### Comparing `cpggen-0.9.6/pyproject.toml` & `cpggen-1.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cpggen"
-version = "0.9.6"
+version = "1.0.0"
 description = "Generate CPG for multiple languages for use with joern"
 authors = ["Team AppThreat <cloud@appthreat.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{include = "cpggen"}]
 homepage = "https://github.com/AppThreat/cpggen"
 repository = "https://github.com/AppThreat/cpggen"
```

### Comparing `cpggen-0.9.6/PKG-INFO` & `cpggen-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpggen
-Version: 0.9.6
+Version: 1.0.0
 Summary: Generate CPG for multiple languages for use with joern
 Home-page: https://github.com/AppThreat/cpggen
 License: Apache-2.0
 Keywords: joern,code analysis,static analysis,cpg,code property graph
 Author: Team AppThreat
 Author-email: cloud@appthreat.com
 Requires-Python: >=3.8,<3.12
@@ -48,59 +48,34 @@
 - JDK 11 or above
 - Python 3.10
 - Docker or podman (Windows, Linux or Mac) or
 - Joern [natively installed](https://docs.joern.io/installation) (Linux only)
 
 ## Installation
 
-cpggen is available as a [PyPI package](https://pypi.org/project/cpggen/) or as a [container image](https://github.com/AppThreat/cpggen/pkgs/container/cpggen).
-
-```
-pip install cpggen
-```
-
-Bundled container image
-
-```
-docker pull ghcr.io/appthreat/cpggen
-# podman pull ghcr.io/appthreat/cpggen
-```
-
-Almalinux 9 requires the CPU to support SSE4.2. For kvm64 VM use the Almalinux 8 version instead.
-
-```
-docker pull ghcr.io/appthreat/cpggen-alma8
-# podman pull ghcr.io/appthreat/cpggen-alma8
-```
-
-Or use the nightly to always get the latest joern and tools.
-
-```
-docker pull ghcr.io/appthreat/cpggen:nightly
-# podman pull ghcr.io/appthreat/cpggen:nightly
-```
+cpggen is available as a single executable binary, [PyPI package](https://pypi.org/project/cpggen/) or as a [container image](https://github.com/AppThreat/cpggen/pkgs/container/cpggen).
 
 ### Single executable binaries
 
 Download the executable binary for your operating system from the [releases page](https://github.com/appthreat/cpggen/releases). These binary bundle the following:
 
 - Joern with all the CPG frontends
 - cpggen with Python 3.10
 - cdxgen with Node.js 18 - Generates SBoM
 
 ```bash
-curl -LO https://github.com/AppThreat/cpggen/releases/download/v0.9.6/cpggen-linux-amd64
+curl -LO https://github.com/AppThreat/cpggen/releases/download/v1.0.0/cpggen-linux-amd64
 chmod +x cpggen-linux-amd64
 ./cpggen-linux-amd64 --help
 ```
 
 On Windows,
 
 ```powershell
-curl -LO https://github.com/appthreat/cpggen/releases/download/v0.9.6/cpggen.exe
+curl -LO https://github.com/appthreat/cpggen/releases/download/v1.0.0/cpggen.exe
 .\cpggen.exe --help
 ```
 
 NOTE: On Windows, antivirus and antimalware could prevent this single executable from functioning properly. Depending on the system, administrative privileges might also be required. Use container-based execution as a fallback.
 
 ### OCI Artifacts via ORAS cli
 
@@ -116,14 +91,43 @@
 
 ```powershell
 Invoke-WebRequest -Uri https://github.com/oras-project/oras/releases/download/v1.0.0/oras_1.0.0_windows_amd64.zip -UseBasicParsing -OutFile oras_1.0.0_windows_amd64.zip
 Expand-Archive -Path oras_1.0.0_windows_amd64.zip -DestinationPath .
 oras.exe pull ghcr.io/appthreat/cpggen-windows-bin:v1
 ```
 
+### PyPI package
+
+This would install just the python cli tool without any CPG language frontends. Joern must be installed separately to make the cli work.
+
+```
+pip install cpggen
+```
+
+### Bundled container image
+
+```
+docker pull ghcr.io/appthreat/cpggen
+# podman pull ghcr.io/appthreat/cpggen
+```
+
+Almalinux 9 requires the CPU to support SSE4.2. For kvm64 VM use the Almalinux 8 version instead.
+
+```
+docker pull ghcr.io/appthreat/cpggen-alma8
+# podman pull ghcr.io/appthreat/cpggen-alma8
+```
+
+Or use the nightly to always get the latest joern and tools.
+
+```
+docker pull ghcr.io/appthreat/cpggen:nightly
+# podman pull ghcr.io/appthreat/cpggen:nightly
+```
+
 ## Usage
 
 To auto detect the language from the current directory and generate CPG.
 
 ```
 cpggen
 ```
```

