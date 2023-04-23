# Comparing `tmp/pyllamacpp-1.0.5.tar.gz` & `tmp/pyllamacpp-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyllamacpp-1.0.5.tar", last modified: Mon Apr  3 04:43:48 2023, max compression
+gzip compressed data, was "pyllamacpp-1.0.6.tar", last modified: Tue Apr  4 22:27:14 2023, max compression
```

## Comparing `pyllamacpp-1.0.5.tar` & `pyllamacpp-1.0.6.tar`

### file list

```diff
@@ -1,114 +1,114 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 04:43:48.467522 pyllamacpp-1.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     8164 2023-04-03 04:43:32.000000 pyllamacpp-1.0.5/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-03 04:43:32.000000 pyllamacpp-1.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-03 04:43:32.000000 pyllamacpp-1.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-04-03 04:43:48.467522 pyllamacpp-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4303 2023-04-03 04:43:32.000000 pyllamacpp-1.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 04:43:48.459521 pyllamacpp-1.0.5/llama.cpp/
--rw-r--r--   0 runner    (1001) docker     (123)     7809 2023-04-03 04:43:33.000000 pyllamacpp-1.0.5/llama.cpp/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 04:43:48.459521 pyllamacpp-1.0.5/llama.cpp/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-04-03 04:43:33.000000 pyllamacpp-1.0.5/llama.cpp/examples/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 04:43:48.459521 pyllamacpp-1.0.5/llama.cpp/examples/embedding/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-03 04:43:33.000000 pyllamacpp-1.0.5/llama.cpp/examples/embedding/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 04:43:48.459521 pyllamacpp-1.0.5/llama.cpp/examples/main/
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-03 04:43:33.000000 pyllamacpp-1.0.5/llama.cpp/examples/main/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 04:43:48.459521 pyllamacpp-1.0.5/llama.cpp/examples/perplexity/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-03 04:43:33.000000 pyllamacpp-1.0.5/llama.cpp/examples/perplexity/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 04:43:48.459521 pyllamacpp-1.0.5/llama.cpp/examples/quantize/
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-03 04:43:33.000000 pyllamacpp-1.0.5/llama.cpp/examples/quantize/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 04:43:48.459521 pyllamacpp-1.0.5/llama.cpp/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-04-03 04:43:33.000000 pyllamacpp-1.0.5/llama.cpp/tests/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 04:43:48.459521 pyllamacpp-1.0.5/pybind11/
--rw-r--r--   0 runner    (1001) docker     (123)    10999 2023-04-03 04:43:32.000000 pyllamacpp-1.0.5/pybind11/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-04-03 04:43:32.000000 pyllamacpp-1.0.5/pybind11/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 04:43:48.455521 pyllamacpp-1.0.5/pybind11/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 04:43:48.463522 pyllamacpp-1.0.5/pybind11/include/pybind11/
--rw-r--r--   0 runner    (1001) docker     (123)    23920 2023-04-03 04:43:32.000000 pyllamacpp-1.0.5/pybind11/include/pybind11/attr.h
--rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-04-03 04:43:32.000000 pyllamacpp-1.0.5/pybind11/include/pybind11/buffer_info.h
--rw-r--r--   0 runner    (1001) docker     (123)    64793 2023-04-03 04:43:32.000000 pyllamacpp-1.0.5/pybind11/include/pybind11/cast.h
--rw-r--r--   0 runner    (1001) docker     (123)     8907 2023-04-03 04:43:32.000000 pyllamacpp-1.0.5/pybind11/include/pybind11/chrono.h
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-03 04:43:32.000000 pyllamacpp-1.0.5/pybind11/include/pybind11/common.h
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-04-03 04:43:32.000000 pyllamacpp-1.0.5/pybind11/include/pybind11/complex.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 04:43:48.463522 pyllamacpp-1.0.5/pybind11/include/pybind11/detail/
--rw-r--r--   0 runner    (1001) docker     (123)    28526 2023-04-03 04:43:32.000000 pyllamacpp-1.0.5/pybind11/include/pybind11/detail/class.h
--rw-r--r--   0 runner    (1001) docker     (123)    51655 2023-04-03 04:43:32.000000 pyllamacpp-1.0.5/pybind11/include/pybind11/detail/common.h
--rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-04-03 04:43:32.000000 pyllamacpp-1.0.5/pybind11/include/pybind11/detail/descr.h
--rw-r--r--   0 runner    (1001) docker     (123)    17971 2023-04-03 04:43:32.000000 pyllamacpp-1.0.5/pybind11/include/pybind11/detail/init.h
--rw-r--r--   0 runner    (1001) docker     (123)    24196 2023-04-03 04:43:32.000000 pyllamacpp-1.0.5/pybind11/include/pybind11/detail/internals.h
--rw-r--r--   0 runner    (1001) docker     (123)    44414 2023-04-03 04:43:32.000000 pyllamacpp-1.0.5/pybind11/include/pybind11/detail/type_caster_base.h
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-04-03 04:43:32.000000 pyllamacpp-1.0.5/pybind11/include/pybind11/detail/typeid.h
--rw-r--r--   0 runner    (1001) docker     (123)    31441 2023-04-03 04:43:32.000000 pyllamacpp-1.0.5/pybind11/include/pybind11/eigen.h
--rw-r--r--   0 runner    (1001) docker     (123)    12175 2023-04-03 04:43:32.000000 pyllamacpp-1.0.5/pybind11/include/pybind11/embed.h
--rw-r--r--   0 runner    (1001) docker     (123)     5589 2023-04-03 04:43:32.000000 pyllamacpp-1.0.5/pybind11/include/pybind11/eval.h
--rw-r--r--   0 runner    (1001) docker     (123)     4755 2023-04-03 04:43:32.000000 pyllamacpp-1.0.5/pybind11/include/pybind11/functional.h
--rw-r--r--   0 runner    (1001) docker     (123)     6848 2023-04-03 04:43:32.000000 pyllamacpp-1.0.5/pybind11/include/pybind11/gil.h
--rw-r--r--   0 runner    (1001) docker     (123)     8851 2023-04-03 04:43:32.000000 pyllamacpp-1.0.5/pybind11/include/pybind11/iostream.h
--rw-r--r--   0 runner    (1001) docker     (123)    78036 2023-04-03 04:43:32.000000 pyllamacpp-1.0.5/pybind11/include/pybind11/numpy.h
--rw-r--r--   0 runner    (1001) docker     (123)     9781 2023-04-03 04:43:32.000000 pyllamacpp-1.0.5/pybind11/include/pybind11/operators.h
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-04-03 04:43:32.000000 pyllamacpp-1.0.5/pybind11/include/pybind11/options.h
--rw-r--r--   0 runner    (1001) docker     (123)   125927 2023-04-03 04:43:32.000000 pyllamacpp-1.0.5/pybind11/include/pybind11/pybind11.h
--rw-r--r--   0 runner    (1001) docker     (123)    80901 2023-04-03 04:43:32.000000 pyllamacpp-1.0.5/pybind11/include/pybind11/pytypes.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 04:43:48.463522 pyllamacpp-1.0.5/pybind11/include/pybind11/stl/
--rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-04-03 04:43:32.000000 pyllamacpp-1.0.5/pybind11/include/pybind11/stl/filesystem.h
--rw-r--r--   0 runner    (1001) docker     (123)    14438 2023-04-03 04:43:32.000000 pyllamacpp-1.0.5/pybind11/include/pybind11/stl.h
--rw-r--r--   0 runner    (1001) docker     (123)    26992 2023-04-03 04:43:32.000000 pyllamacpp-1.0.5/pybind11/include/pybind11/stl_bind.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 04:43:48.463522 pyllamacpp-1.0.5/pybind11/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    21095 2023-04-03 04:43:32.000000 pyllamacpp-1.0.5/pybind11/tests/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 04:43:48.463522 pyllamacpp-1.0.5/pybind11/tests/test_cmake_build/
--rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-04-03 04:43:32.000000 pyllamacpp-1.0.5/pybind11/tests/test_cmake_build/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 04:43:48.463522 pyllamacpp-1.0.5/pybind11/tests/test_cmake_build/installed_embed/
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-04-03 04:43:32.000000 pyllamacpp-1.0.5/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 04:43:48.463522 pyllamacpp-1.0.5/pybind11/tests/test_cmake_build/installed_function/
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-04-03 04:43:32.000000 pyllamacpp-1.0.5/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 04:43:48.463522 pyllamacpp-1.0.5/pybind11/tests/test_cmake_build/installed_target/
--rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-04-03 04:43:32.000000 pyllamacpp-1.0.5/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 04:43:48.463522 pyllamacpp-1.0.5/pybind11/tests/test_cmake_build/subdirectory_embed/
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-04-03 04:43:32.000000 pyllamacpp-1.0.5/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 04:43:48.463522 pyllamacpp-1.0.5/pybind11/tests/test_cmake_build/subdirectory_function/
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-04-03 04:43:32.000000 pyllamacpp-1.0.5/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 04:43:48.463522 pyllamacpp-1.0.5/pybind11/tests/test_cmake_build/subdirectory_target/
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-04-03 04:43:32.000000 pyllamacpp-1.0.5/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 04:43:48.463522 pyllamacpp-1.0.5/pybind11/tests/test_embed/
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-04-03 04:43:32.000000 pyllamacpp-1.0.5/pybind11/tests/test_embed/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 04:43:48.467522 pyllamacpp-1.0.5/pybind11/tools/
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-04-03 04:43:32.000000 pyllamacpp-1.0.5/pybind11/tools/FindCatch.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-04-03 04:43:32.000000 pyllamacpp-1.0.5/pybind11/tools/FindEigen3.cmake
--rw-r--r--   0 runner    (1001) docker     (123)    10378 2023-04-03 04:43:32.000000 pyllamacpp-1.0.5/pybind11/tools/FindPythonLibsNew.cmake
--rwxr-xr-x   0 runner    (1001) docker     (123)     1423 2023-04-03 04:43:32.000000 pyllamacpp-1.0.5/pybind11/tools/check-style.sh
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-04-03 04:43:32.000000 pyllamacpp-1.0.5/pybind11/tools/cmake_uninstall.cmake.in
--rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-04-03 04:43:32.000000 pyllamacpp-1.0.5/pybind11/tools/libsize.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1306 2023-04-03 04:43:32.000000 pyllamacpp-1.0.5/pybind11/tools/make_changelog.py
--rw-r--r--   0 runner    (1001) docker     (123)    14579 2023-04-03 04:43:32.000000 pyllamacpp-1.0.5/pybind11/tools/pybind11Common.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     7063 2023-04-03 04:43:32.000000 pyllamacpp-1.0.5/pybind11/tools/pybind11Config.cmake.in
--rw-r--r--   0 runner    (1001) docker     (123)     9673 2023-04-03 04:43:32.000000 pyllamacpp-1.0.5/pybind11/tools/pybind11NewTools.cmake
--rw-r--r--   0 runner    (1001) docker     (123)     7447 2023-04-03 04:43:32.000000 pyllamacpp-1.0.5/pybind11/tools/pybind11Tools.cmake
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-03 04:43:32.000000 pyllamacpp-1.0.5/pybind11/tools/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-04-03 04:43:32.000000 pyllamacpp-1.0.5/pybind11/tools/setup_global.py.in
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-03 04:43:32.000000 pyllamacpp-1.0.5/pybind11/tools/setup_main.py.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 04:43:48.455521 pyllamacpp-1.0.5/pyllamacpp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-03 04:43:32.000000 pyllamacpp-1.0.5/pyllamacpp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-04-03 04:43:32.000000 pyllamacpp-1.0.5/pyllamacpp/_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-04-03 04:43:32.000000 pyllamacpp-1.0.5/pyllamacpp/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-04-03 04:43:32.000000 pyllamacpp-1.0.5/pyllamacpp/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 04:43:48.459521 pyllamacpp-1.0.5/pyllamacpp/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-03 04:43:32.000000 pyllamacpp-1.0.5/pyllamacpp/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-04-03 04:43:32.000000 pyllamacpp-1.0.5/pyllamacpp/scripts/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-04-03 04:43:32.000000 pyllamacpp-1.0.5/pyllamacpp/scripts/convert_gpt4all.py
--rw-r--r--   0 runner    (1001) docker     (123)     9597 2023-04-03 04:43:32.000000 pyllamacpp-1.0.5/pyllamacpp/scripts/migrate.py
--rw-r--r--   0 runner    (1001) docker     (123)     6346 2023-04-03 04:43:32.000000 pyllamacpp-1.0.5/pyllamacpp/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10835 2023-04-03 04:43:32.000000 pyllamacpp-1.0.5/pyllamacpp/webui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 04:43:48.467522 pyllamacpp-1.0.5/pyllamacpp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-04-03 04:43:48.000000 pyllamacpp-1.0.5/pyllamacpp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-04-03 04:43:48.000000 pyllamacpp-1.0.5/pyllamacpp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 04:43:48.000000 pyllamacpp-1.0.5/pyllamacpp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-03 04:43:48.000000 pyllamacpp-1.0.5/pyllamacpp.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 04:43:48.000000 pyllamacpp-1.0.5/pyllamacpp.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-03 04:43:48.000000 pyllamacpp-1.0.5/pyllamacpp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-03 04:43:48.000000 pyllamacpp-1.0.5/pyllamacpp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-04-03 04:43:32.000000 pyllamacpp-1.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-03 04:43:32.000000 pyllamacpp-1.0.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-03 04:43:48.467522 pyllamacpp-1.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     6475 2023-04-03 04:43:32.000000 pyllamacpp-1.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 04:43:48.467522 pyllamacpp-1.0.5/src/
--rw-r--r--   0 runner    (1001) docker     (123)    24434 2023-04-03 04:43:32.000000 pyllamacpp-1.0.5/src/main.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-04-03 04:43:32.000000 pyllamacpp-1.0.5/src/main.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 22:27:14.541493 pyllamacpp-1.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     8164 2023-04-04 22:26:59.000000 pyllamacpp-1.0.6/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-04 22:26:59.000000 pyllamacpp-1.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-04 22:26:59.000000 pyllamacpp-1.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-04-04 22:27:14.541493 pyllamacpp-1.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4543 2023-04-04 22:26:59.000000 pyllamacpp-1.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 22:27:14.529492 pyllamacpp-1.0.6/llama.cpp/
+-rw-r--r--   0 runner    (1001) docker     (123)     7809 2023-04-04 22:27:00.000000 pyllamacpp-1.0.6/llama.cpp/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 22:27:14.529492 pyllamacpp-1.0.6/llama.cpp/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-04-04 22:27:00.000000 pyllamacpp-1.0.6/llama.cpp/examples/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 22:27:14.529492 pyllamacpp-1.0.6/llama.cpp/examples/embedding/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-04 22:27:00.000000 pyllamacpp-1.0.6/llama.cpp/examples/embedding/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 22:27:14.529492 pyllamacpp-1.0.6/llama.cpp/examples/main/
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-04 22:27:00.000000 pyllamacpp-1.0.6/llama.cpp/examples/main/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 22:27:14.529492 pyllamacpp-1.0.6/llama.cpp/examples/perplexity/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-04 22:27:00.000000 pyllamacpp-1.0.6/llama.cpp/examples/perplexity/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 22:27:14.529492 pyllamacpp-1.0.6/llama.cpp/examples/quantize/
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-04 22:27:00.000000 pyllamacpp-1.0.6/llama.cpp/examples/quantize/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 22:27:14.529492 pyllamacpp-1.0.6/llama.cpp/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-04-04 22:27:00.000000 pyllamacpp-1.0.6/llama.cpp/tests/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 22:27:14.529492 pyllamacpp-1.0.6/pybind11/
+-rw-r--r--   0 runner    (1001) docker     (123)    10999 2023-04-04 22:26:59.000000 pyllamacpp-1.0.6/pybind11/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1684 2023-04-04 22:26:59.000000 pyllamacpp-1.0.6/pybind11/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 22:27:14.525493 pyllamacpp-1.0.6/pybind11/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 22:27:14.533493 pyllamacpp-1.0.6/pybind11/include/pybind11/
+-rw-r--r--   0 runner    (1001) docker     (123)    23920 2023-04-04 22:26:59.000000 pyllamacpp-1.0.6/pybind11/include/pybind11/attr.h
+-rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-04-04 22:26:59.000000 pyllamacpp-1.0.6/pybind11/include/pybind11/buffer_info.h
+-rw-r--r--   0 runner    (1001) docker     (123)    64793 2023-04-04 22:26:59.000000 pyllamacpp-1.0.6/pybind11/include/pybind11/cast.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8907 2023-04-04 22:26:59.000000 pyllamacpp-1.0.6/pybind11/include/pybind11/chrono.h
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-04 22:26:59.000000 pyllamacpp-1.0.6/pybind11/include/pybind11/common.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-04-04 22:26:59.000000 pyllamacpp-1.0.6/pybind11/include/pybind11/complex.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 22:27:14.533493 pyllamacpp-1.0.6/pybind11/include/pybind11/detail/
+-rw-r--r--   0 runner    (1001) docker     (123)    28526 2023-04-04 22:26:59.000000 pyllamacpp-1.0.6/pybind11/include/pybind11/detail/class.h
+-rw-r--r--   0 runner    (1001) docker     (123)    51655 2023-04-04 22:26:59.000000 pyllamacpp-1.0.6/pybind11/include/pybind11/detail/common.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5491 2023-04-04 22:26:59.000000 pyllamacpp-1.0.6/pybind11/include/pybind11/detail/descr.h
+-rw-r--r--   0 runner    (1001) docker     (123)    17971 2023-04-04 22:26:59.000000 pyllamacpp-1.0.6/pybind11/include/pybind11/detail/init.h
+-rw-r--r--   0 runner    (1001) docker     (123)    24196 2023-04-04 22:26:59.000000 pyllamacpp-1.0.6/pybind11/include/pybind11/detail/internals.h
+-rw-r--r--   0 runner    (1001) docker     (123)    44414 2023-04-04 22:26:59.000000 pyllamacpp-1.0.6/pybind11/include/pybind11/detail/type_caster_base.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-04-04 22:26:59.000000 pyllamacpp-1.0.6/pybind11/include/pybind11/detail/typeid.h
+-rw-r--r--   0 runner    (1001) docker     (123)    31441 2023-04-04 22:26:59.000000 pyllamacpp-1.0.6/pybind11/include/pybind11/eigen.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12175 2023-04-04 22:26:59.000000 pyllamacpp-1.0.6/pybind11/include/pybind11/embed.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5589 2023-04-04 22:26:59.000000 pyllamacpp-1.0.6/pybind11/include/pybind11/eval.h
+-rw-r--r--   0 runner    (1001) docker     (123)     4755 2023-04-04 22:26:59.000000 pyllamacpp-1.0.6/pybind11/include/pybind11/functional.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6848 2023-04-04 22:26:59.000000 pyllamacpp-1.0.6/pybind11/include/pybind11/gil.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8851 2023-04-04 22:26:59.000000 pyllamacpp-1.0.6/pybind11/include/pybind11/iostream.h
+-rw-r--r--   0 runner    (1001) docker     (123)    78036 2023-04-04 22:26:59.000000 pyllamacpp-1.0.6/pybind11/include/pybind11/numpy.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9781 2023-04-04 22:26:59.000000 pyllamacpp-1.0.6/pybind11/include/pybind11/operators.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-04-04 22:26:59.000000 pyllamacpp-1.0.6/pybind11/include/pybind11/options.h
+-rw-r--r--   0 runner    (1001) docker     (123)   125927 2023-04-04 22:26:59.000000 pyllamacpp-1.0.6/pybind11/include/pybind11/pybind11.h
+-rw-r--r--   0 runner    (1001) docker     (123)    80901 2023-04-04 22:26:59.000000 pyllamacpp-1.0.6/pybind11/include/pybind11/pytypes.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 22:27:14.533493 pyllamacpp-1.0.6/pybind11/include/pybind11/stl/
+-rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-04-04 22:26:59.000000 pyllamacpp-1.0.6/pybind11/include/pybind11/stl/filesystem.h
+-rw-r--r--   0 runner    (1001) docker     (123)    14438 2023-04-04 22:26:59.000000 pyllamacpp-1.0.6/pybind11/include/pybind11/stl.h
+-rw-r--r--   0 runner    (1001) docker     (123)    26992 2023-04-04 22:26:59.000000 pyllamacpp-1.0.6/pybind11/include/pybind11/stl_bind.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 22:27:14.533493 pyllamacpp-1.0.6/pybind11/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    21095 2023-04-04 22:26:59.000000 pyllamacpp-1.0.6/pybind11/tests/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 22:27:14.537493 pyllamacpp-1.0.6/pybind11/tests/test_cmake_build/
+-rw-r--r--   0 runner    (1001) docker     (123)     2639 2023-04-04 22:26:59.000000 pyllamacpp-1.0.6/pybind11/tests/test_cmake_build/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 22:27:14.537493 pyllamacpp-1.0.6/pybind11/tests/test_cmake_build/installed_embed/
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-04-04 22:26:59.000000 pyllamacpp-1.0.6/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 22:27:14.537493 pyllamacpp-1.0.6/pybind11/tests/test_cmake_build/installed_function/
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-04-04 22:26:59.000000 pyllamacpp-1.0.6/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 22:27:14.537493 pyllamacpp-1.0.6/pybind11/tests/test_cmake_build/installed_target/
+-rw-r--r--   0 runner    (1001) docker     (123)     1685 2023-04-04 22:26:59.000000 pyllamacpp-1.0.6/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 22:27:14.537493 pyllamacpp-1.0.6/pybind11/tests/test_cmake_build/subdirectory_embed/
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-04-04 22:26:59.000000 pyllamacpp-1.0.6/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 22:27:14.537493 pyllamacpp-1.0.6/pybind11/tests/test_cmake_build/subdirectory_function/
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-04-04 22:26:59.000000 pyllamacpp-1.0.6/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 22:27:14.537493 pyllamacpp-1.0.6/pybind11/tests/test_cmake_build/subdirectory_target/
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-04-04 22:26:59.000000 pyllamacpp-1.0.6/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 22:27:14.537493 pyllamacpp-1.0.6/pybind11/tests/test_embed/
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-04-04 22:26:59.000000 pyllamacpp-1.0.6/pybind11/tests/test_embed/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 22:27:14.541493 pyllamacpp-1.0.6/pybind11/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-04-04 22:26:59.000000 pyllamacpp-1.0.6/pybind11/tools/FindCatch.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-04-04 22:26:59.000000 pyllamacpp-1.0.6/pybind11/tools/FindEigen3.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)    10378 2023-04-04 22:26:59.000000 pyllamacpp-1.0.6/pybind11/tools/FindPythonLibsNew.cmake
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1423 2023-04-04 22:26:59.000000 pyllamacpp-1.0.6/pybind11/tools/check-style.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-04-04 22:26:59.000000 pyllamacpp-1.0.6/pybind11/tools/cmake_uninstall.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-04-04 22:26:59.000000 pyllamacpp-1.0.6/pybind11/tools/libsize.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1306 2023-04-04 22:26:59.000000 pyllamacpp-1.0.6/pybind11/tools/make_changelog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14579 2023-04-04 22:26:59.000000 pyllamacpp-1.0.6/pybind11/tools/pybind11Common.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     7063 2023-04-04 22:26:59.000000 pyllamacpp-1.0.6/pybind11/tools/pybind11Config.cmake.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9673 2023-04-04 22:26:59.000000 pyllamacpp-1.0.6/pybind11/tools/pybind11NewTools.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)     7447 2023-04-04 22:26:59.000000 pyllamacpp-1.0.6/pybind11/tools/pybind11Tools.cmake
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-04 22:26:59.000000 pyllamacpp-1.0.6/pybind11/tools/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-04-04 22:26:59.000000 pyllamacpp-1.0.6/pybind11/tools/setup_global.py.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-04 22:26:59.000000 pyllamacpp-1.0.6/pybind11/tools/setup_main.py.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 22:27:14.529492 pyllamacpp-1.0.6/pyllamacpp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-04 22:26:59.000000 pyllamacpp-1.0.6/pyllamacpp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-04-04 22:26:59.000000 pyllamacpp-1.0.6/pyllamacpp/_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-04-04 22:26:59.000000 pyllamacpp-1.0.6/pyllamacpp/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4397 2023-04-04 22:26:59.000000 pyllamacpp-1.0.6/pyllamacpp/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 22:27:14.529492 pyllamacpp-1.0.6/pyllamacpp/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-04 22:26:59.000000 pyllamacpp-1.0.6/pyllamacpp/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3257 2023-04-04 22:26:59.000000 pyllamacpp-1.0.6/pyllamacpp/scripts/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-04-04 22:26:59.000000 pyllamacpp-1.0.6/pyllamacpp/scripts/convert_gpt4all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9597 2023-04-04 22:26:59.000000 pyllamacpp-1.0.6/pyllamacpp/scripts/migrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6346 2023-04-04 22:26:59.000000 pyllamacpp-1.0.6/pyllamacpp/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10835 2023-04-04 22:26:59.000000 pyllamacpp-1.0.6/pyllamacpp/webui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 22:27:14.541493 pyllamacpp-1.0.6/pyllamacpp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-04-04 22:27:14.000000 pyllamacpp-1.0.6/pyllamacpp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-04-04 22:27:14.000000 pyllamacpp-1.0.6/pyllamacpp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 22:27:14.000000 pyllamacpp-1.0.6/pyllamacpp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-04 22:27:14.000000 pyllamacpp-1.0.6/pyllamacpp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 22:27:14.000000 pyllamacpp-1.0.6/pyllamacpp.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-04 22:27:14.000000 pyllamacpp-1.0.6/pyllamacpp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-04 22:27:14.000000 pyllamacpp-1.0.6/pyllamacpp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1221 2023-04-04 22:26:59.000000 pyllamacpp-1.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-04 22:26:59.000000 pyllamacpp-1.0.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-04 22:27:14.541493 pyllamacpp-1.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     6476 2023-04-04 22:26:59.000000 pyllamacpp-1.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 22:27:14.541493 pyllamacpp-1.0.6/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    24153 2023-04-04 22:26:59.000000 pyllamacpp-1.0.6/src/main.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-04-04 22:26:59.000000 pyllamacpp-1.0.6/src/main.h
```

### Comparing `pyllamacpp-1.0.5/CMakeLists.txt` & `pyllamacpp-1.0.6/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyllamacpp-1.0.5/LICENSE` & `pyllamacpp-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyllamacpp-1.0.5/PKG-INFO` & `pyllamacpp-1.0.6/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,9 @@
-Metadata-Version: 2.1
-Name: pyllamacpp
-Version: 1.0.5
-Summary: Python bindings for llama.cpp
-Author: abdeladim-s
-License: MIT
-Project-URL: Documentation, https://abdeladim-s.github.io/pyllamacpp
-Project-URL: Source, https://github.com/abdeladim-s/pyllamacpp
-Project-URL: Tracker, https://github.com/abdeladim-s/pyllamacpp/issues
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# PyLLaMaCpp
-Python bindings for [llama.cpp](https://github.com/ggerganov/llama.cpp) + A simple web UI
+# PyLLaMACpp
+Official supported Python bindings for [llama.cpp](https://github.com/ggerganov/llama.cpp) + gpt4all
 
 [![License: MIT](https://img.shields.io/badge/license-MIT-blue.svg)](https://opensource.org/licenses/MIT)
 [![PyPi version](https://badgen.net/pypi/v/pyllamacpp)](https://pypi.org/project/pyllamacpp/)
 
 [//]: # ([![Wheels]&#40;https://github.com/abdeladim-s/pyllamacpp/actions/workflows/wheels.yml/badge.svg?branch=main&event=push&#41;]&#40;https://github.com/abdeladim-s/pyllamacpp/actions/workflows/wheels.yml&#41;)
 
 [//]: # ([![Wheels-windows-mac]&#40;https://github.com/abdeladim-s/pyllamacpp/actions/workflows/wheels-windows_mac.yml/badge.svg&#41;]&#40;https://github.com/abdeladim-s/pyllamacpp/actions/workflows/wheels-windows_mac.yml&#41;)
@@ -43,16 +30,16 @@
 
 </blockquote>
 
 # Table of contents
 <!-- TOC -->
 * [Installation](#installation)
 * [Usage](#usage)
-    * [Web UI](#web-ui)
-    * [Python bindings](#python-bindings)
+* [Supported model](#supported-model)
+    * [GPT4All](#gpt4all)
 * [Discussions and contributions](#discussions-and-contributions)
 * [License](#license)
 <!-- TOC -->
 
 # Installation
 1. The easy way is to use the prebuilt wheels
 ```bash
@@ -65,71 +52,89 @@
 ```shell
 git clone --recursive https://github.com/abdeladim-s/pyllamacpp && cd pyllamacpp
 pip install .
 ```
 
 # Usage
 
-### Web UI
-The package contains a simple web UI to test the bindings:
+[//]: # ()
+[//]: # (### Web UI)
 
-- Lightweight, and easy to use.
-- Only needs Python.
-- Has the option to convert the models to `ggml` format.
-- A code like editor.
-- Different options to tweak the `llama.cpp` parameters.
-- Ability to export the generated text.
+[//]: # (The package contains a simple web UI to test the bindings:)
 
-From the command line, run:
-```shell
-pyllamacpp-webui
-```
+[//]: # ()
+[//]: # (- Lightweight, and easy to use.)
+
+[//]: # (- Only needs Python.)
+
+[//]: # (- Has the option to convert the models to `ggml` format.)
+
+[//]: # (- A code like editor.)
+
+[//]: # (- Different options to tweak the `llama.cpp` parameters.)
 
-That's it!<br>
-A web page will be opened on your default browser, otherwise navigate to the links provided by the command.
+[//]: # (- Ability to export the generated text.)
 
+[//]: # ()
+[//]: # (From the command line, run:)
 
-### Python bindings
+[//]: # (```shell)
+
+[//]: # (pyllamacpp-webui)
+
+[//]: # (```)
+
+[//]: # ()
+[//]: # (That's it!<br>)
+
+[//]: # (A web page will be opened on your default browser, otherwise navigate to the links provided by the command.)
+
+[//]: # ()
+[//]: # ()
+[//]: # (### Python bindings)
 
 A simple `Pythonic` API is built on top of `llama.cpp` C/C++ functions. You can call it from Python as follows:
 
 ```python
 from pyllamacpp.model import Model
 
 def new_text_callback(text: str):
     print(text, end="")
 
-model = Model(ggml_model='./models/ggml-model-f16-q4_0.bin', n_ctx=512, n_threads=8)
-model.generate("Once upon a time, ", n_predict=55, new_text_callback=new_text_callback)
+model = Model(ggml_model='./models/gpt4all-model.bin', n_ctx=512)
+model.generate("Once upon a time, ", n_predict=55, new_text_callback=new_text_callback, n_threads=8)
 ```
 If you don't want to use the `callback`, you can get the results from the `generate` method once the inference is finished:
 
 ```python
 generated_text = model.generate("Once upon a time, ", n_predict=55)
 print(generated_text)
 ```
-* You can pass any `llama context` [parameter](https://abdeladim-s.github.io/pyllamacpp/#pyllamacpp.constants.LLAMA_CONTEXT_PARAMS_SCHEMA) as a keyword argument to the `Model` class
-* You can pass any `gpt` [parameter](https://abdeladim-s.github.io/pyllamacpp/#pyllamacpp.constants.LLAMA_CONTEXT_PARAMS_SCHEMA) as a keyword argument to the `generarte` method
-* You can always refer to the [short documentation](https://abdeladim-s.github.io/pyllamacpp/) for more details.
 
-You can convert and quantize the models from Python as well:
+* You can pass any `llama context` [parameter](https://nomic-ai.github.io/pyllamacpp/#pyllamacpp.constants.LLAMA_CONTEXT_PARAMS_SCHEMA) as a keyword argument to the `Model` class
+* You can pass any `gpt` [parameter](https://nomic-ai.github.io/pyllamacpp/#pyllamacpp.constants.GPT_PARAMS_SCHEMA) as a keyword argument to the `generarte` method
+* You can always refer to the [short documentation](https://nomic-ai.github.io/pyllamacpp/) for more details.
+
 
 # Supported model
 
 ### GPT4All
 1. First [Get](https://github.com/nomic-ai/gpt4all#try-it-yourself) the gpt4all model.
 2. Convert it to the new `ggml` format
 
 On your terminal run: 
 ```shell
 pyllamacpp-convert-gpt4all path/to/gpt4all_model.bin path/to/llama_tokenizer path/to/gpt4all-converted.bin
 ```
 
+# FAQs
+* Where to find the llama tokenizer? [#5](https://github.com/nomic-ai/pyllamacpp/issues/5)
+
 # Discussions and contributions
-If you find any bug, please open an [issue](https://github.com/abdeladim-s/pyllamacpp/issues).
+If you find any bug, please open an [issue](https://github.com/nomic-ai/pyllamacpp/issues).
 
-If you have any feedback, or you want to share how you are using this project, feel free to use the [Discussions](https://github.com/abdeladim-s/pyllamacpp/discussions) and open a new topic.
+If you have any feedback, or you want to share how you are using this project, feel free to use the [Discussions](https://github.com/nomic-ai/pyllamacpp/discussions) and open a new topic.
 
 # License
 
-This project is licensed under the same license as [llama.cpp](https://github.com/ggerganov/whisper.cpp/blob/master/LICENSE) (MIT  [License](./LICENSE)).
+This project is licensed under the same license as [llama.cpp](https://github.com/ggerganov/llama.cpp/blob/master/LICENSE) (MIT  [License](./LICENSE)).
```

### Comparing `pyllamacpp-1.0.5/README.md` & `pyllamacpp-1.0.6/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,22 @@
-# PyLLaMaCpp
-Python bindings for [llama.cpp](https://github.com/ggerganov/llama.cpp) + A simple web UI
+Metadata-Version: 2.1
+Name: pyllamacpp
+Version: 1.0.6
+Summary: Python bindings for llama.cpp + gpt4all
+Author: abdeladim-s
+License: MIT
+Project-URL: Documentation, https://nomic-ai.github.io/pyllamacpp
+Project-URL: Source, https://github.com/nomic-ai/pyllamacpp
+Project-URL: Tracker, https://github.com/nomic-ai/pyllamacpp/issues
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# PyLLaMACpp
+Official supported Python bindings for [llama.cpp](https://github.com/ggerganov/llama.cpp) + gpt4all
 
 [![License: MIT](https://img.shields.io/badge/license-MIT-blue.svg)](https://opensource.org/licenses/MIT)
 [![PyPi version](https://badgen.net/pypi/v/pyllamacpp)](https://pypi.org/project/pyllamacpp/)
 
 [//]: # ([![Wheels]&#40;https://github.com/abdeladim-s/pyllamacpp/actions/workflows/wheels.yml/badge.svg?branch=main&event=push&#41;]&#40;https://github.com/abdeladim-s/pyllamacpp/actions/workflows/wheels.yml&#41;)
 
 [//]: # ([![Wheels-windows-mac]&#40;https://github.com/abdeladim-s/pyllamacpp/actions/workflows/wheels-windows_mac.yml/badge.svg&#41;]&#40;https://github.com/abdeladim-s/pyllamacpp/actions/workflows/wheels-windows_mac.yml&#41;)
@@ -30,16 +43,16 @@
 
 </blockquote>
 
 # Table of contents
 <!-- TOC -->
 * [Installation](#installation)
 * [Usage](#usage)
-    * [Web UI](#web-ui)
-    * [Python bindings](#python-bindings)
+* [Supported model](#supported-model)
+    * [GPT4All](#gpt4all)
 * [Discussions and contributions](#discussions-and-contributions)
 * [License](#license)
 <!-- TOC -->
 
 # Installation
 1. The easy way is to use the prebuilt wheels
 ```bash
@@ -52,71 +65,89 @@
 ```shell
 git clone --recursive https://github.com/abdeladim-s/pyllamacpp && cd pyllamacpp
 pip install .
 ```
 
 # Usage
 
-### Web UI
-The package contains a simple web UI to test the bindings:
+[//]: # ()
+[//]: # (### Web UI)
 
-- Lightweight, and easy to use.
-- Only needs Python.
-- Has the option to convert the models to `ggml` format.
-- A code like editor.
-- Different options to tweak the `llama.cpp` parameters.
-- Ability to export the generated text.
+[//]: # (The package contains a simple web UI to test the bindings:)
 
-From the command line, run:
-```shell
-pyllamacpp-webui
-```
+[//]: # ()
+[//]: # (- Lightweight, and easy to use.)
+
+[//]: # (- Only needs Python.)
+
+[//]: # (- Has the option to convert the models to `ggml` format.)
+
+[//]: # (- A code like editor.)
+
+[//]: # (- Different options to tweak the `llama.cpp` parameters.)
 
-That's it!<br>
-A web page will be opened on your default browser, otherwise navigate to the links provided by the command.
+[//]: # (- Ability to export the generated text.)
 
+[//]: # ()
+[//]: # (From the command line, run:)
 
-### Python bindings
+[//]: # (```shell)
+
+[//]: # (pyllamacpp-webui)
+
+[//]: # (```)
+
+[//]: # ()
+[//]: # (That's it!<br>)
+
+[//]: # (A web page will be opened on your default browser, otherwise navigate to the links provided by the command.)
+
+[//]: # ()
+[//]: # ()
+[//]: # (### Python bindings)
 
 A simple `Pythonic` API is built on top of `llama.cpp` C/C++ functions. You can call it from Python as follows:
 
 ```python
 from pyllamacpp.model import Model
 
 def new_text_callback(text: str):
     print(text, end="")
 
-model = Model(ggml_model='./models/ggml-model-f16-q4_0.bin', n_ctx=512, n_threads=8)
-model.generate("Once upon a time, ", n_predict=55, new_text_callback=new_text_callback)
+model = Model(ggml_model='./models/gpt4all-model.bin', n_ctx=512)
+model.generate("Once upon a time, ", n_predict=55, new_text_callback=new_text_callback, n_threads=8)
 ```
 If you don't want to use the `callback`, you can get the results from the `generate` method once the inference is finished:
 
 ```python
 generated_text = model.generate("Once upon a time, ", n_predict=55)
 print(generated_text)
 ```
-* You can pass any `llama context` [parameter](https://abdeladim-s.github.io/pyllamacpp/#pyllamacpp.constants.LLAMA_CONTEXT_PARAMS_SCHEMA) as a keyword argument to the `Model` class
-* You can pass any `gpt` [parameter](https://abdeladim-s.github.io/pyllamacpp/#pyllamacpp.constants.LLAMA_CONTEXT_PARAMS_SCHEMA) as a keyword argument to the `generarte` method
-* You can always refer to the [short documentation](https://abdeladim-s.github.io/pyllamacpp/) for more details.
 
-You can convert and quantize the models from Python as well:
+* You can pass any `llama context` [parameter](https://nomic-ai.github.io/pyllamacpp/#pyllamacpp.constants.LLAMA_CONTEXT_PARAMS_SCHEMA) as a keyword argument to the `Model` class
+* You can pass any `gpt` [parameter](https://nomic-ai.github.io/pyllamacpp/#pyllamacpp.constants.GPT_PARAMS_SCHEMA) as a keyword argument to the `generarte` method
+* You can always refer to the [short documentation](https://nomic-ai.github.io/pyllamacpp/) for more details.
+
 
 # Supported model
 
 ### GPT4All
 1. First [Get](https://github.com/nomic-ai/gpt4all#try-it-yourself) the gpt4all model.
 2. Convert it to the new `ggml` format
 
 On your terminal run: 
 ```shell
 pyllamacpp-convert-gpt4all path/to/gpt4all_model.bin path/to/llama_tokenizer path/to/gpt4all-converted.bin
 ```
 
+# FAQs
+* Where to find the llama tokenizer? [#5](https://github.com/nomic-ai/pyllamacpp/issues/5)
+
 # Discussions and contributions
-If you find any bug, please open an [issue](https://github.com/abdeladim-s/pyllamacpp/issues).
+If you find any bug, please open an [issue](https://github.com/nomic-ai/pyllamacpp/issues).
 
-If you have any feedback, or you want to share how you are using this project, feel free to use the [Discussions](https://github.com/abdeladim-s/pyllamacpp/discussions) and open a new topic.
+If you have any feedback, or you want to share how you are using this project, feel free to use the [Discussions](https://github.com/nomic-ai/pyllamacpp/discussions) and open a new topic.
 
 # License
 
-This project is licensed under the same license as [llama.cpp](https://github.com/ggerganov/whisper.cpp/blob/master/LICENSE) (MIT  [License](./LICENSE)).
+This project is licensed under the same license as [llama.cpp](https://github.com/ggerganov/llama.cpp/blob/master/LICENSE) (MIT  [License](./LICENSE)).
```

### Comparing `pyllamacpp-1.0.5/llama.cpp/CMakeLists.txt` & `pyllamacpp-1.0.6/llama.cpp/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyllamacpp-1.0.5/llama.cpp/examples/CMakeLists.txt` & `pyllamacpp-1.0.6/llama.cpp/examples/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyllamacpp-1.0.5/pybind11/CMakeLists.txt` & `pyllamacpp-1.0.6/pybind11/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyllamacpp-1.0.5/pybind11/LICENSE` & `pyllamacpp-1.0.6/pybind11/LICENSE`

 * *Files identical despite different names*

### Comparing `pyllamacpp-1.0.5/pybind11/include/pybind11/attr.h` & `pyllamacpp-1.0.6/pybind11/include/pybind11/attr.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-1.0.5/pybind11/include/pybind11/buffer_info.h` & `pyllamacpp-1.0.6/pybind11/include/pybind11/buffer_info.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-1.0.5/pybind11/include/pybind11/cast.h` & `pyllamacpp-1.0.6/pybind11/include/pybind11/cast.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-1.0.5/pybind11/include/pybind11/chrono.h` & `pyllamacpp-1.0.6/pybind11/include/pybind11/chrono.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-1.0.5/pybind11/include/pybind11/complex.h` & `pyllamacpp-1.0.6/pybind11/include/pybind11/complex.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-1.0.5/pybind11/include/pybind11/detail/class.h` & `pyllamacpp-1.0.6/pybind11/include/pybind11/detail/class.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-1.0.5/pybind11/include/pybind11/detail/common.h` & `pyllamacpp-1.0.6/pybind11/include/pybind11/detail/common.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-1.0.5/pybind11/include/pybind11/detail/descr.h` & `pyllamacpp-1.0.6/pybind11/include/pybind11/detail/descr.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-1.0.5/pybind11/include/pybind11/detail/init.h` & `pyllamacpp-1.0.6/pybind11/include/pybind11/detail/init.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-1.0.5/pybind11/include/pybind11/detail/internals.h` & `pyllamacpp-1.0.6/pybind11/include/pybind11/detail/internals.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-1.0.5/pybind11/include/pybind11/detail/type_caster_base.h` & `pyllamacpp-1.0.6/pybind11/include/pybind11/detail/type_caster_base.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-1.0.5/pybind11/include/pybind11/detail/typeid.h` & `pyllamacpp-1.0.6/pybind11/include/pybind11/detail/typeid.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-1.0.5/pybind11/include/pybind11/eigen.h` & `pyllamacpp-1.0.6/pybind11/include/pybind11/eigen.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-1.0.5/pybind11/include/pybind11/embed.h` & `pyllamacpp-1.0.6/pybind11/include/pybind11/embed.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-1.0.5/pybind11/include/pybind11/eval.h` & `pyllamacpp-1.0.6/pybind11/include/pybind11/eval.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-1.0.5/pybind11/include/pybind11/functional.h` & `pyllamacpp-1.0.6/pybind11/include/pybind11/functional.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-1.0.5/pybind11/include/pybind11/gil.h` & `pyllamacpp-1.0.6/pybind11/include/pybind11/gil.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-1.0.5/pybind11/include/pybind11/iostream.h` & `pyllamacpp-1.0.6/pybind11/include/pybind11/iostream.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-1.0.5/pybind11/include/pybind11/numpy.h` & `pyllamacpp-1.0.6/pybind11/include/pybind11/numpy.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-1.0.5/pybind11/include/pybind11/operators.h` & `pyllamacpp-1.0.6/pybind11/include/pybind11/operators.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-1.0.5/pybind11/include/pybind11/options.h` & `pyllamacpp-1.0.6/pybind11/include/pybind11/options.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-1.0.5/pybind11/include/pybind11/pybind11.h` & `pyllamacpp-1.0.6/pybind11/include/pybind11/pybind11.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-1.0.5/pybind11/include/pybind11/pytypes.h` & `pyllamacpp-1.0.6/pybind11/include/pybind11/pytypes.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-1.0.5/pybind11/include/pybind11/stl/filesystem.h` & `pyllamacpp-1.0.6/pybind11/include/pybind11/stl/filesystem.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-1.0.5/pybind11/include/pybind11/stl.h` & `pyllamacpp-1.0.6/pybind11/include/pybind11/stl.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-1.0.5/pybind11/include/pybind11/stl_bind.h` & `pyllamacpp-1.0.6/pybind11/include/pybind11/stl_bind.h`

 * *Files identical despite different names*

### Comparing `pyllamacpp-1.0.5/pybind11/tests/CMakeLists.txt` & `pyllamacpp-1.0.6/pybind11/tests/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyllamacpp-1.0.5/pybind11/tests/test_cmake_build/CMakeLists.txt` & `pyllamacpp-1.0.6/pybind11/tests/test_cmake_build/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyllamacpp-1.0.5/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt` & `pyllamacpp-1.0.6/pybind11/tests/test_cmake_build/installed_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyllamacpp-1.0.5/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt` & `pyllamacpp-1.0.6/pybind11/tests/test_cmake_build/installed_function/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyllamacpp-1.0.5/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt` & `pyllamacpp-1.0.6/pybind11/tests/test_cmake_build/installed_target/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyllamacpp-1.0.5/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt` & `pyllamacpp-1.0.6/pybind11/tests/test_cmake_build/subdirectory_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyllamacpp-1.0.5/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt` & `pyllamacpp-1.0.6/pybind11/tests/test_cmake_build/subdirectory_function/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyllamacpp-1.0.5/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt` & `pyllamacpp-1.0.6/pybind11/tests/test_cmake_build/subdirectory_target/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyllamacpp-1.0.5/pybind11/tests/test_embed/CMakeLists.txt` & `pyllamacpp-1.0.6/pybind11/tests/test_embed/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyllamacpp-1.0.5/pybind11/tools/FindCatch.cmake` & `pyllamacpp-1.0.6/pybind11/tools/FindCatch.cmake`

 * *Files identical despite different names*

### Comparing `pyllamacpp-1.0.5/pybind11/tools/FindEigen3.cmake` & `pyllamacpp-1.0.6/pybind11/tools/FindEigen3.cmake`

 * *Files identical despite different names*

### Comparing `pyllamacpp-1.0.5/pybind11/tools/FindPythonLibsNew.cmake` & `pyllamacpp-1.0.6/pybind11/tools/FindPythonLibsNew.cmake`

 * *Files identical despite different names*

### Comparing `pyllamacpp-1.0.5/pybind11/tools/check-style.sh` & `pyllamacpp-1.0.6/pybind11/tools/check-style.sh`

 * *Files identical despite different names*

### Comparing `pyllamacpp-1.0.5/pybind11/tools/cmake_uninstall.cmake.in` & `pyllamacpp-1.0.6/pybind11/tools/cmake_uninstall.cmake.in`

 * *Files identical despite different names*

### Comparing `pyllamacpp-1.0.5/pybind11/tools/libsize.py` & `pyllamacpp-1.0.6/pybind11/tools/libsize.py`

 * *Files identical despite different names*

### Comparing `pyllamacpp-1.0.5/pybind11/tools/make_changelog.py` & `pyllamacpp-1.0.6/pybind11/tools/make_changelog.py`

 * *Files identical despite different names*

### Comparing `pyllamacpp-1.0.5/pybind11/tools/pybind11Common.cmake` & `pyllamacpp-1.0.6/pybind11/tools/pybind11Common.cmake`

 * *Files identical despite different names*

### Comparing `pyllamacpp-1.0.5/pybind11/tools/pybind11Config.cmake.in` & `pyllamacpp-1.0.6/pybind11/tools/pybind11Config.cmake.in`

 * *Files identical despite different names*

### Comparing `pyllamacpp-1.0.5/pybind11/tools/pybind11NewTools.cmake` & `pyllamacpp-1.0.6/pybind11/tools/pybind11NewTools.cmake`

 * *Files identical despite different names*

### Comparing `pyllamacpp-1.0.5/pybind11/tools/pybind11Tools.cmake` & `pyllamacpp-1.0.6/pybind11/tools/pybind11Tools.cmake`

 * *Files identical despite different names*

### Comparing `pyllamacpp-1.0.5/pybind11/tools/setup_global.py.in` & `pyllamacpp-1.0.6/pybind11/tools/setup_global.py.in`

 * *Files identical despite different names*

### Comparing `pyllamacpp-1.0.5/pybind11/tools/setup_main.py.in` & `pyllamacpp-1.0.6/pybind11/tools/setup_main.py.in`

 * *Files identical despite different names*

### Comparing `pyllamacpp-1.0.5/pyllamacpp/_logger.py` & `pyllamacpp-1.0.6/pyllamacpp/_logger.py`

 * *Files identical despite different names*

### Comparing `pyllamacpp-1.0.5/pyllamacpp/constants.py` & `pyllamacpp-1.0.6/pyllamacpp/constants.py`

 * *Files identical despite different names*

### Comparing `pyllamacpp-1.0.5/pyllamacpp/model.py` & `pyllamacpp-1.0.6/pyllamacpp/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,14 +44,15 @@
         :param ggml_model: the path to the ggml model
         :param log_level: logging level, set to INFO by default
         :param llama_params: keyword arguments for different whisper.cpp parameters,
                         see [PARAMS_SCHEMA](/pyllamacpp/#pyllamacpp.constants.LLAMA_CONTEXT_PARAMS_SCHEMA)
         """
         # set logging level
         set_log_level(log_level)
+        self._ctx = None
 
         if not Path(ggml_model).is_file():
             raise Exception(f"File {ggml_model} not found!")
 
         self.llama_params = pp.llama_context_default_params()
         # update llama_params
         self._set_params(self.llama_params, llama_params)
@@ -129,9 +130,10 @@
         """
         A simple link to [PARAMS_SCHEMA](/pyllamacpp/#pyllamacpp.constants.PARAMS_SCHEMA)
         :return: dict of params schema
         """
         return constants.GPT_PARAMS_SCHEMA
 
     def __del__(self):
-        pp.llama_free(self._ctx)
+        if self._ctx:
+            pp.llama_free(self._ctx)
```

### Comparing `pyllamacpp-1.0.5/pyllamacpp/scripts/convert.py` & `pyllamacpp-1.0.6/pyllamacpp/scripts/convert.py`

 * *Files identical despite different names*

### Comparing `pyllamacpp-1.0.5/pyllamacpp/scripts/convert_gpt4all.py` & `pyllamacpp-1.0.6/pyllamacpp/scripts/convert_gpt4all.py`

 * *Files identical despite different names*

### Comparing `pyllamacpp-1.0.5/pyllamacpp/scripts/migrate.py` & `pyllamacpp-1.0.6/pyllamacpp/scripts/migrate.py`

 * *Files identical despite different names*

### Comparing `pyllamacpp-1.0.5/pyllamacpp/utils.py` & `pyllamacpp-1.0.6/pyllamacpp/utils.py`

 * *Files identical despite different names*

### Comparing `pyllamacpp-1.0.5/pyllamacpp/webui.py` & `pyllamacpp-1.0.6/pyllamacpp/webui.py`

 * *Files identical despite different names*

### Comparing `pyllamacpp-1.0.5/pyllamacpp.egg-info/PKG-INFO` & `pyllamacpp-1.0.6/pyllamacpp.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: pyllamacpp
-Version: 1.0.5
-Summary: Python bindings for llama.cpp
+Version: 1.0.6
+Summary: Python bindings for llama.cpp + gpt4all
 Author: abdeladim-s
 License: MIT
-Project-URL: Documentation, https://abdeladim-s.github.io/pyllamacpp
-Project-URL: Source, https://github.com/abdeladim-s/pyllamacpp
-Project-URL: Tracker, https://github.com/abdeladim-s/pyllamacpp/issues
+Project-URL: Documentation, https://nomic-ai.github.io/pyllamacpp
+Project-URL: Source, https://github.com/nomic-ai/pyllamacpp
+Project-URL: Tracker, https://github.com/nomic-ai/pyllamacpp/issues
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# PyLLaMaCpp
-Python bindings for [llama.cpp](https://github.com/ggerganov/llama.cpp) + A simple web UI
+# PyLLaMACpp
+Official supported Python bindings for [llama.cpp](https://github.com/ggerganov/llama.cpp) + gpt4all
 
 [![License: MIT](https://img.shields.io/badge/license-MIT-blue.svg)](https://opensource.org/licenses/MIT)
 [![PyPi version](https://badgen.net/pypi/v/pyllamacpp)](https://pypi.org/project/pyllamacpp/)
 
 [//]: # ([![Wheels]&#40;https://github.com/abdeladim-s/pyllamacpp/actions/workflows/wheels.yml/badge.svg?branch=main&event=push&#41;]&#40;https://github.com/abdeladim-s/pyllamacpp/actions/workflows/wheels.yml&#41;)
 
 [//]: # ([![Wheels-windows-mac]&#40;https://github.com/abdeladim-s/pyllamacpp/actions/workflows/wheels-windows_mac.yml/badge.svg&#41;]&#40;https://github.com/abdeladim-s/pyllamacpp/actions/workflows/wheels-windows_mac.yml&#41;)
@@ -43,16 +43,16 @@
 
 </blockquote>
 
 # Table of contents
 <!-- TOC -->
 * [Installation](#installation)
 * [Usage](#usage)
-    * [Web UI](#web-ui)
-    * [Python bindings](#python-bindings)
+* [Supported model](#supported-model)
+    * [GPT4All](#gpt4all)
 * [Discussions and contributions](#discussions-and-contributions)
 * [License](#license)
 <!-- TOC -->
 
 # Installation
 1. The easy way is to use the prebuilt wheels
 ```bash
@@ -65,71 +65,89 @@
 ```shell
 git clone --recursive https://github.com/abdeladim-s/pyllamacpp && cd pyllamacpp
 pip install .
 ```
 
 # Usage
 
-### Web UI
-The package contains a simple web UI to test the bindings:
+[//]: # ()
+[//]: # (### Web UI)
 
-- Lightweight, and easy to use.
-- Only needs Python.
-- Has the option to convert the models to `ggml` format.
-- A code like editor.
-- Different options to tweak the `llama.cpp` parameters.
-- Ability to export the generated text.
+[//]: # (The package contains a simple web UI to test the bindings:)
 
-From the command line, run:
-```shell
-pyllamacpp-webui
-```
+[//]: # ()
+[//]: # (- Lightweight, and easy to use.)
+
+[//]: # (- Only needs Python.)
+
+[//]: # (- Has the option to convert the models to `ggml` format.)
+
+[//]: # (- A code like editor.)
+
+[//]: # (- Different options to tweak the `llama.cpp` parameters.)
+
+[//]: # (- Ability to export the generated text.)
 
-That's it!<br>
-A web page will be opened on your default browser, otherwise navigate to the links provided by the command.
+[//]: # ()
+[//]: # (From the command line, run:)
 
+[//]: # (```shell)
 
-### Python bindings
+[//]: # (pyllamacpp-webui)
+
+[//]: # (```)
+
+[//]: # ()
+[//]: # (That's it!<br>)
+
+[//]: # (A web page will be opened on your default browser, otherwise navigate to the links provided by the command.)
+
+[//]: # ()
+[//]: # ()
+[//]: # (### Python bindings)
 
 A simple `Pythonic` API is built on top of `llama.cpp` C/C++ functions. You can call it from Python as follows:
 
 ```python
 from pyllamacpp.model import Model
 
 def new_text_callback(text: str):
     print(text, end="")
 
-model = Model(ggml_model='./models/ggml-model-f16-q4_0.bin', n_ctx=512, n_threads=8)
-model.generate("Once upon a time, ", n_predict=55, new_text_callback=new_text_callback)
+model = Model(ggml_model='./models/gpt4all-model.bin', n_ctx=512)
+model.generate("Once upon a time, ", n_predict=55, new_text_callback=new_text_callback, n_threads=8)
 ```
 If you don't want to use the `callback`, you can get the results from the `generate` method once the inference is finished:
 
 ```python
 generated_text = model.generate("Once upon a time, ", n_predict=55)
 print(generated_text)
 ```
-* You can pass any `llama context` [parameter](https://abdeladim-s.github.io/pyllamacpp/#pyllamacpp.constants.LLAMA_CONTEXT_PARAMS_SCHEMA) as a keyword argument to the `Model` class
-* You can pass any `gpt` [parameter](https://abdeladim-s.github.io/pyllamacpp/#pyllamacpp.constants.LLAMA_CONTEXT_PARAMS_SCHEMA) as a keyword argument to the `generarte` method
-* You can always refer to the [short documentation](https://abdeladim-s.github.io/pyllamacpp/) for more details.
 
-You can convert and quantize the models from Python as well:
+* You can pass any `llama context` [parameter](https://nomic-ai.github.io/pyllamacpp/#pyllamacpp.constants.LLAMA_CONTEXT_PARAMS_SCHEMA) as a keyword argument to the `Model` class
+* You can pass any `gpt` [parameter](https://nomic-ai.github.io/pyllamacpp/#pyllamacpp.constants.GPT_PARAMS_SCHEMA) as a keyword argument to the `generarte` method
+* You can always refer to the [short documentation](https://nomic-ai.github.io/pyllamacpp/) for more details.
+
 
 # Supported model
 
 ### GPT4All
 1. First [Get](https://github.com/nomic-ai/gpt4all#try-it-yourself) the gpt4all model.
 2. Convert it to the new `ggml` format
 
 On your terminal run: 
 ```shell
 pyllamacpp-convert-gpt4all path/to/gpt4all_model.bin path/to/llama_tokenizer path/to/gpt4all-converted.bin
 ```
 
+# FAQs
+* Where to find the llama tokenizer? [#5](https://github.com/nomic-ai/pyllamacpp/issues/5)
+
 # Discussions and contributions
-If you find any bug, please open an [issue](https://github.com/abdeladim-s/pyllamacpp/issues).
+If you find any bug, please open an [issue](https://github.com/nomic-ai/pyllamacpp/issues).
 
-If you have any feedback, or you want to share how you are using this project, feel free to use the [Discussions](https://github.com/abdeladim-s/pyllamacpp/discussions) and open a new topic.
+If you have any feedback, or you want to share how you are using this project, feel free to use the [Discussions](https://github.com/nomic-ai/pyllamacpp/discussions) and open a new topic.
 
 # License
 
-This project is licensed under the same license as [llama.cpp](https://github.com/ggerganov/whisper.cpp/blob/master/LICENSE) (MIT  [License](./LICENSE)).
+This project is licensed under the same license as [llama.cpp](https://github.com/ggerganov/llama.cpp/blob/master/LICENSE) (MIT  [License](./LICENSE)).
```

### Comparing `pyllamacpp-1.0.5/pyllamacpp.egg-info/SOURCES.txt` & `pyllamacpp-1.0.6/pyllamacpp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyllamacpp-1.0.5/pyproject.toml` & `pyllamacpp-1.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyllamacpp-1.0.5/setup.py` & `pyllamacpp-1.0.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -127,17 +127,17 @@
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 # The information here can also be placed in setup.cfg - better separation of
 # logic and declaration, and simpler if you include description/version in a file.
 setup(
     name="pyllamacpp",
-    version="1.0.5",
+    version="1.0.6",
     author="abdeladim-s",
-    description="Python bindings for llama.cpp",
+    description="Python bindings for llama.cpp + gpt4all",
     long_description=long_description,
     ext_modules=[CMakeExtension("_pyllamacpp")],
     cmdclass={"build_ext": CMakeBuild},
     zip_safe=False,
     # extras_require={"test": ["pytest>=6.0"]},
     python_requires=">=3.8",
     packages=find_packages('.'),
@@ -145,12 +145,12 @@
     long_description_content_type="text/markdown",
     license='MIT',
     entry_points={
         'console_scripts': ['pyllamacpp-webui=pyllamacpp.webui:run',
                             'pyllamacpp-convert-gpt4all=pyllamacpp.scripts.convert_gpt4all:main']
     },
     project_urls={
-        'Documentation': 'https://abdeladim-s.github.io/pyllamacpp',
-        'Source': 'https://github.com/abdeladim-s/pyllamacpp',
-        'Tracker': 'https://github.com/abdeladim-s/pyllamacpp/issues',
+        'Documentation': 'https://nomic-ai.github.io/pyllamacpp',
+        'Source': 'https://github.com/nomic-ai/pyllamacpp',
+        'Tracker': 'https://github.com/nomic-ai/pyllamacpp/issues',
     },
 )
```

### Comparing `pyllamacpp-1.0.5/src/main.cpp` & `pyllamacpp-1.0.6/src/main.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -348,16 +348,14 @@
     bool is_antiprompt = false;
     bool input_noecho  = false;
 
     int n_past     = 0;
     int n_remain   = params.n_predict;
     int n_consumed = 0;
 
-    // the first thing we will do is to output the prompt, so set color accordingly
-//    set_console_color(con_st, CONSOLE_COLOR_PROMPT);
 
     std::vector<llama_token> embd;
 
     while (n_remain != 0 || params.interactive) {
         // predict
         if (embd.size() > 0) {
             // infinite text generation via context swapping
@@ -556,22 +554,15 @@
         // In interactive mode, respect the maximum number of tokens and drop back to user input when reached.
         if (params.interactive && n_remain <= 0 && params.n_predict != -1) {
             n_remain = params.n_predict;
             is_interacting = true;
         }
     }
 
-//#if defined (_WIN32)
-//    signal(SIGINT, SIG_DFL);
-//#endif
-
     llama_print_timings(ctx);
-    llama_free(ctx);
-
-//    set_console_color(con_st, CONSOLE_COLOR_DEFAULT);
 
     return 0;
 }
 
 PYBIND11_MODULE(_pyllamacpp, m) {
     m.doc() = R"pbdoc(
         PyLlamaCpp: Python binding to llama.cpp
```

### Comparing `pyllamacpp-1.0.5/src/main.h` & `pyllamacpp-1.0.6/src/main.h`

 * *Files identical despite different names*

