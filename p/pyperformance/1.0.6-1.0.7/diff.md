# Comparing `tmp/pyperformance-1.0.6.tar.gz` & `tmp/pyperformance-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyperformance-1.0.6.tar", last modified: Sun Nov 20 19:57:43 2022, max compression
+gzip compressed data, was "pyperformance-1.0.7.tar", last modified: Sun Apr 23 06:21:09 2023, max compression
```

## Comparing `pyperformance-1.0.6.tar` & `pyperformance-1.0.7.tar`

### file list

```diff
@@ -1,399 +1,539 @@
-drwxr-xr-x   0 pgalindo3   (503) staff       (20)        0 2022-11-20 19:57:43.185930 pyperformance-1.0.6/
--rw-r--r--   0 pgalindo3   (503) staff       (20)      607 2022-11-20 19:47:21.000000 pyperformance-1.0.6/AUTHORS
--rw-r--r--   0 pgalindo3   (503) staff       (20)     1040 2022-11-20 19:47:21.000000 pyperformance-1.0.6/COPYING
--rw-r--r--   0 pgalindo3   (503) staff       (20)      649 2022-11-20 19:47:21.000000 pyperformance-1.0.6/MANIFEST.in
--rw-r--r--   0 pgalindo3   (503) staff       (20)     1744 2022-11-20 19:57:43.185792 pyperformance-1.0.6/PKG-INFO
--rw-r--r--   0 pgalindo3   (503) staff       (20)     1170 2022-11-20 19:47:21.000000 pyperformance-1.0.6/README.rst
--rw-r--r--   0 pgalindo3   (503) staff       (20)     4325 2022-11-20 19:47:21.000000 pyperformance-1.0.6/TODO.rst
-drwxr-xr-x   0 pgalindo3   (503) staff       (20)        0 2022-11-20 19:57:43.150020 pyperformance-1.0.6/doc/
--rw-r--r--   0 pgalindo3   (503) staff       (20)      628 2022-11-20 19:47:21.000000 pyperformance-1.0.6/doc/Makefile
--rw-r--r--   0 pgalindo3   (503) staff       (20)    20221 2022-11-20 19:47:21.000000 pyperformance-1.0.6/doc/benchmarks.rst
--rw-r--r--   0 pgalindo3   (503) staff       (20)    19152 2022-11-20 19:55:29.000000 pyperformance-1.0.6/doc/changelog.rst
--rw-r--r--   0 pgalindo3   (503) staff       (20)     4923 2022-11-20 19:50:03.000000 pyperformance-1.0.6/doc/conf.py
--rw-r--r--   0 pgalindo3   (503) staff       (20)    25473 2022-11-20 19:47:21.000000 pyperformance-1.0.6/doc/cpython_results_2017.rst
--rw-r--r--   0 pgalindo3   (503) staff       (20)    10342 2022-11-20 19:47:21.000000 pyperformance-1.0.6/doc/custom_benchmarks.rst
-drwxr-xr-x   0 pgalindo3   (503) staff       (20)        0 2022-11-20 19:57:43.150577 pyperformance-1.0.6/doc/images/
--rw-r--r--   0 pgalindo3   (503) staff       (20)     9302 2022-11-20 19:47:21.000000 pyperformance-1.0.6/doc/images/bm_chaos.png
--rw-r--r--   0 pgalindo3   (503) staff       (20)    55274 2022-11-20 19:47:21.000000 pyperformance-1.0.6/doc/images/bm_raytrace.jpg
--rw-r--r--   0 pgalindo3   (503) staff       (20)    48901 2022-11-20 19:47:21.000000 pyperformance-1.0.6/doc/images/html5lib.png
--rw-r--r--   0 pgalindo3   (503) staff       (20)    42433 2022-11-20 19:47:21.000000 pyperformance-1.0.6/doc/images/sympy_sum.png
--rw-r--r--   0 pgalindo3   (503) staff       (20)     1936 2022-11-20 19:47:21.000000 pyperformance-1.0.6/doc/index.rst
--rw-r--r--   0 pgalindo3   (503) staff       (20)      834 2022-11-20 19:47:21.000000 pyperformance-1.0.6/doc/make.bat
--rw-r--r--   0 pgalindo3   (503) staff       (20)    19415 2022-11-20 19:47:21.000000 pyperformance-1.0.6/doc/usage.rst
-drwxr-xr-x   0 pgalindo3   (503) staff       (20)        0 2022-11-20 19:57:43.152839 pyperformance-1.0.6/pyperformance/
--rw-r--r--   0 pgalindo3   (503) staff       (20)     1097 2022-11-20 19:49:45.000000 pyperformance-1.0.6/pyperformance/__init__.py
--rw-r--r--   0 pgalindo3   (503) staff       (20)       50 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/__main__.py
--rw-r--r--   0 pgalindo3   (503) staff       (20)     7829 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/_benchmark.py
--rw-r--r--   0 pgalindo3   (503) staff       (20)     7227 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/_benchmark_metadata.py
--rw-r--r--   0 pgalindo3   (503) staff       (20)     3833 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/_benchmark_selections.py
--rw-r--r--   0 pgalindo3   (503) staff       (20)    14510 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/_manifest.py
--rw-r--r--   0 pgalindo3   (503) staff       (20)     4724 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/_pip.py
--rw-r--r--   0 pgalindo3   (503) staff       (20)     9660 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/_pyproject_toml.py
--rw-r--r--   0 pgalindo3   (503) staff       (20)     1272 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/_python.py
--rw-r--r--   0 pgalindo3   (503) staff       (20)     5340 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/_pythoninfo.py
--rw-r--r--   0 pgalindo3   (503) staff       (20)     5898 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/_utils.py
--rw-r--r--   0 pgalindo3   (503) staff       (20)     7553 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/_venv.py
--rw-r--r--   0 pgalindo3   (503) staff       (20)    12132 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/cli.py
--rw-r--r--   0 pgalindo3   (503) staff       (20)     7759 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/commands.py
--rw-r--r--   0 pgalindo3   (503) staff       (20)    13019 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/compare.py
--rw-r--r--   0 pgalindo3   (503) staff       (20)    33030 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/compile.py
-drwxr-xr-x   0 pgalindo3   (503) staff       (20)        0 2022-11-20 19:57:43.153633 pyperformance-1.0.6/pyperformance/data-files/
-drwxr-xr-x   0 pgalindo3   (503) staff       (20)        0 2022-11-20 19:57:43.153738 pyperformance-1.0.6/pyperformance/data-files/benchmarks/
--rw-r--r--   0 pgalindo3   (503) staff       (20)     1513 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/MANIFEST
-drwxr-xr-x   0 pgalindo3   (503) staff       (20)        0 2022-11-20 19:57:43.153964 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_2to3/
-drwxr-xr-x   0 pgalindo3   (503) staff       (20)        0 2022-11-20 19:57:43.142743 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_2to3/data/
-drwxr-xr-x   0 pgalindo3   (503) staff       (20)        0 2022-11-20 19:57:43.155075 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_2to3/data/2to3/
--rw-r--r--   0 pgalindo3   (503) staff       (20)       48 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_2to3/data/2to3/README.txt
--rw-r--r--   0 pgalindo3   (503) staff       (20)        0 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_2to3/data/2to3/__init__.py.txt
--rw-r--r--   0 pgalindo3   (503) staff       (20)     3418 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_2to3/data/2to3/context_processors.py.txt
--rw-r--r--   0 pgalindo3   (503) staff       (20)      912 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_2to3/data/2to3/exceptions.py.txt
--rw-r--r--   0 pgalindo3   (503) staff       (20)    16817 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_2to3/data/2to3/mail.py.txt
--rw-r--r--   0 pgalindo3   (503) staff       (20)     4021 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_2to3/data/2to3/paginator.py.txt
--rw-r--r--   0 pgalindo3   (503) staff       (20)      150 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_2to3/data/2to3/signals.py.txt
--rw-r--r--   0 pgalindo3   (503) staff       (20)      165 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_2to3/data/2to3/template_loader.py.txt
--rw-r--r--   0 pgalindo3   (503) staff       (20)    15786 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_2to3/data/2to3/urlresolvers.py.txt
--rw-r--r--   0 pgalindo3   (503) staff       (20)     1166 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_2to3/data/2to3/xheaders.py.txt
--rw-r--r--   0 pgalindo3   (503) staff       (20)      229 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_2to3/pyproject.toml
--rw-r--r--   0 pgalindo3   (503) staff       (20)      465 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_2to3/run_benchmark.py
-drwxr-xr-x   0 pgalindo3   (503) staff       (20)        0 2022-11-20 19:57:43.155283 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_async_generators/
--rw-r--r--   0 pgalindo3   (503) staff       (20)      239 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_async_generators/pyproject.toml
--rw-r--r--   0 pgalindo3   (503) staff       (20)     1104 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_async_generators/run_benchmark.py
-drwxr-xr-x   0 pgalindo3   (503) staff       (20)        0 2022-11-20 19:57:43.155789 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_async_tree/
--rw-r--r--   0 pgalindo3   (503) staff       (20)       85 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_async_tree/bm_async_tree_cpu_io_mixed.toml
--rw-r--r--   0 pgalindo3   (503) staff       (20)       65 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_async_tree/bm_async_tree_io.toml
--rw-r--r--   0 pgalindo3   (503) staff       (20)       83 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_async_tree/bm_async_tree_memoization.toml
--rw-r--r--   0 pgalindo3   (503) staff       (20)      249 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_async_tree/pyproject.toml
--rw-r--r--   0 pgalindo3   (503) staff       (20)     4278 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_async_tree/run_benchmark.py
-drwxr-xr-x   0 pgalindo3   (503) staff       (20)        0 2022-11-20 19:57:43.156171 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_chameleon/
--rw-r--r--   0 pgalindo3   (503) staff       (20)      263 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_chameleon/pyproject.toml
--rw-r--r--   0 pgalindo3   (503) staff       (20)       17 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_chameleon/requirements.txt
--rw-r--r--   0 pgalindo3   (503) staff       (20)      814 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_chameleon/run_benchmark.py
-drwxr-xr-x   0 pgalindo3   (503) staff       (20)        0 2022-11-20 19:57:43.156405 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_chaos/
--rw-r--r--   0 pgalindo3   (503) staff       (20)      217 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_chaos/pyproject.toml
--rw-r--r--   0 pgalindo3   (503) staff       (20)    10709 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_chaos/run_benchmark.py
-drwxr-xr-x   0 pgalindo3   (503) staff       (20)        0 2022-11-20 19:57:43.156661 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_concurrent_imap/
--rw-r--r--   0 pgalindo3   (503) staff       (20)      237 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_concurrent_imap/pyproject.toml
--rw-r--r--   0 pgalindo3   (503) staff       (20)      813 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_concurrent_imap/run_benchmark.py
-drwxr-xr-x   0 pgalindo3   (503) staff       (20)        0 2022-11-20 19:57:43.156886 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_coroutines/
--rw-r--r--   0 pgalindo3   (503) staff       (20)      227 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_coroutines/pyproject.toml
--rw-r--r--   0 pgalindo3   (503) staff       (20)      697 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_coroutines/run_benchmark.py
-drwxr-xr-x   0 pgalindo3   (503) staff       (20)        0 2022-11-20 19:57:43.157241 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_coverage/
--rw-r--r--   0 pgalindo3   (503) staff       (20)      246 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_coverage/pyproject.toml
--rw-r--r--   0 pgalindo3   (503) staff       (20)       16 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_coverage/requirements.txt
--rw-r--r--   0 pgalindo3   (503) staff       (20)      634 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_coverage/run_benchmark.py
-drwxr-xr-x   0 pgalindo3   (503) staff       (20)        0 2022-11-20 19:57:43.157603 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_crypto_pyaes/
--rw-r--r--   0 pgalindo3   (503) staff       (20)      251 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_crypto_pyaes/pyproject.toml
--rw-r--r--   0 pgalindo3   (503) staff       (20)       13 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_crypto_pyaes/requirements.txt
--rw-r--r--   0 pgalindo3   (503) staff       (20)     1098 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_crypto_pyaes/run_benchmark.py
-drwxr-xr-x   0 pgalindo3   (503) staff       (20)        0 2022-11-20 19:57:43.157862 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_deepcopy/
--rw-r--r--   0 pgalindo3   (503) staff       (20)      223 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_deepcopy/pyproject.toml
--rw-r--r--   0 pgalindo3   (503) staff       (20)     2142 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_deepcopy/run_benchmark.py
-drwxr-xr-x   0 pgalindo3   (503) staff       (20)        0 2022-11-20 19:57:43.158099 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_deltablue/
--rw-r--r--   0 pgalindo3   (503) staff       (20)      225 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_deltablue/pyproject.toml
--rw-r--r--   0 pgalindo3   (503) staff       (20)    17136 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_deltablue/run_benchmark.py
-drwxr-xr-x   0 pgalindo3   (503) staff       (20)        0 2022-11-20 19:57:43.158454 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_django_template/
--rw-r--r--   0 pgalindo3   (503) staff       (20)      276 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_django_template/pyproject.toml
--rw-r--r--   0 pgalindo3   (503) staff       (20)       58 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_django_template/requirements.txt
--rw-r--r--   0 pgalindo3   (503) staff       (20)     1409 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_django_template/run_benchmark.py
-drwxr-xr-x   0 pgalindo3   (503) staff       (20)        0 2022-11-20 19:57:43.158793 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/
-drwxr-xr-x   0 pgalindo3   (503) staff       (20)        0 2022-11-20 19:57:43.143607 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/
-drwxr-xr-x   0 pgalindo3   (503) staff       (20)        0 2022-11-20 19:57:43.158903 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/
-drwxr-xr-x   0 pgalindo3   (503) staff       (20)        0 2022-11-20 19:57:43.159257 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/api/
--rw-r--r--   0 pgalindo3   (503) staff       (20)    10569 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/api/publisher.txt
--rw-r--r--   0 pgalindo3   (503) staff       (20)     6216 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/api/runtime-settings.txt
--rw-r--r--   0 pgalindo3   (503) staff       (20)     6334 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/api/transforms.txt
-drwxr-xr-x   0 pgalindo3   (503) staff       (20)        0 2022-11-20 19:57:43.160826 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/
--rw-r--r--   0 pgalindo3   (503) staff       (20)     4530 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/distributing.txt
--rw-r--r--   0 pgalindo3   (503) staff       (20)    16986 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/enthought-plan.txt
--rw-r--r--   0 pgalindo3   (503) staff       (20)     4531 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/enthought-rfp.txt
--rw-r--r--   0 pgalindo3   (503) staff       (20)     9172 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/hacking.txt
--rw-r--r--   0 pgalindo3   (503) staff       (20)    25780 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/policies.txt
--rw-r--r--   0 pgalindo3   (503) staff       (20)     4380 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/pysource.txt
--rw-r--r--   0 pgalindo3   (503) staff       (20)     3497 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/release.txt
--rw-r--r--   0 pgalindo3   (503) staff       (20)     9439 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/repository.txt
-drwxr-xr-x   0 pgalindo3   (503) staff       (20)        0 2022-11-20 19:57:43.161123 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/rst/
--rw-r--r--   0 pgalindo3   (503) staff       (20)   113263 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/rst/alternatives.txt
--rw-r--r--   0 pgalindo3   (503) staff       (20)    35463 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/rst/problems.txt
--rw-r--r--   0 pgalindo3   (503) staff       (20)    10664 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/runtime-settings-processing.txt
--rw-r--r--   0 pgalindo3   (503) staff       (20)     4511 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/semantics.txt
--rw-r--r--   0 pgalindo3   (503) staff       (20)     9504 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/testing.txt
--rw-r--r--   0 pgalindo3   (503) staff       (20)    98603 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/todo.txt
--rw-r--r--   0 pgalindo3   (503) staff       (20)     3274 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/website.txt
-drwxr-xr-x   0 pgalindo3   (503) staff       (20)        0 2022-11-20 19:57:43.161844 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/howto/
--rw-r--r--   0 pgalindo3   (503) staff       (20)     2219 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/howto/cmdline-tool.txt
--rw-r--r--   0 pgalindo3   (503) staff       (20)     3417 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/howto/html-stylesheets.txt
--rw-r--r--   0 pgalindo3   (503) staff       (20)     6869 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/howto/i18n.txt
--rw-r--r--   0 pgalindo3   (503) staff       (20)    16349 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/howto/rst-directives.txt
--rw-r--r--   0 pgalindo3   (503) staff       (20)     8907 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/howto/rst-roles.txt
--rw-r--r--   0 pgalindo3   (503) staff       (20)     6972 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/howto/security.txt
--rw-r--r--   0 pgalindo3   (503) staff       (20)     8264 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/index.txt
-drwxr-xr-x   0 pgalindo3   (503) staff       (20)        0 2022-11-20 19:57:43.162333 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/peps/
--rw-r--r--   0 pgalindo3   (503) staff       (20)    10437 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/peps/pep-0256.txt
--rw-r--r--   0 pgalindo3   (503) staff       (20)    11684 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/peps/pep-0257.txt
--rw-r--r--   0 pgalindo3   (503) staff       (20)    36399 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/peps/pep-0258.txt
--rw-r--r--   0 pgalindo3   (503) staff       (20)    32543 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/peps/pep-0287.txt
-drwxr-xr-x   0 pgalindo3   (503) staff       (20)        0 2022-11-20 19:57:43.162534 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/ref/
--rw-r--r--   0 pgalindo3   (503) staff       (20)   132076 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/ref/doctree.txt
-drwxr-xr-x   0 pgalindo3   (503) staff       (20)        0 2022-11-20 19:57:43.163432 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/ref/rst/
--rw-r--r--   0 pgalindo3   (503) staff       (20)     7613 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/ref/rst/definitions.txt
--rw-r--r--   0 pgalindo3   (503) staff       (20)    66717 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/ref/rst/directives.txt
--rw-r--r--   0 pgalindo3   (503) staff       (20)    13914 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/ref/rst/introduction.txt
--rw-r--r--   0 pgalindo3   (503) staff       (20)    51188 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/ref/rst/mathematics.txt
--rw-r--r--   0 pgalindo3   (503) staff       (20)   117454 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/ref/rst/restructuredtext.txt
--rw-r--r--   0 pgalindo3   (503) staff       (20)    10658 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/ref/rst/roles.txt
-drwxr-xr-x   0 pgalindo3   (503) staff       (20)        0 2022-11-20 19:57:43.164699 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/
--rw-r--r--   0 pgalindo3   (503) staff       (20)    64502 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/config.txt
--rw-r--r--   0 pgalindo3   (503) staff       (20)    31991 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/emacs.txt
--rw-r--r--   0 pgalindo3   (503) staff       (20)     8318 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/html.txt
-drwxr-xr-x   0 pgalindo3   (503) staff       (20)        0 2022-11-20 19:57:43.166494 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/images/
--rw-r--r--   0 pgalindo3   (503) staff       (20)        0 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/images/big-black.png
--rw-r--r--   0 pgalindo3   (503) staff       (20)        0 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/images/big-white.png
--rw-r--r--   0 pgalindo3   (503) staff       (20)        0 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/images/default.png
--rw-r--r--   0 pgalindo3   (503) staff       (20)        0 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/images/happy_monkey.png
--rw-r--r--   0 pgalindo3   (503) staff       (20)        0 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/images/medium-black.png
--rw-r--r--   0 pgalindo3   (503) staff       (20)        0 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/images/medium-white.png
--rw-r--r--   0 pgalindo3   (503) staff       (20)        0 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/images/rsp-all.png
--rw-r--r--   0 pgalindo3   (503) staff       (20)        0 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/images/rsp-breaks.png
--rw-r--r--   0 pgalindo3   (503) staff       (20)        0 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/images/rsp-covers.png
--rw-r--r--   0 pgalindo3   (503) staff       (20)        0 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/images/rsp-cuts.png
--rw-r--r--   0 pgalindo3   (503) staff       (20)        0 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/images/rsp-empty.png
--rw-r--r--   0 pgalindo3   (503) staff       (20)        0 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/images/rsp-objects.png
--rw-r--r--   0 pgalindo3   (503) staff       (20)        0 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/images/rsp.svg
--rw-r--r--   0 pgalindo3   (503) staff       (20)        0 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/images/s5-files.png
--rw-r--r--   0 pgalindo3   (503) staff       (20)        0 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/images/s5-files.svg
--rw-r--r--   0 pgalindo3   (503) staff       (20)        0 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/images/small-black.png
--rw-r--r--   0 pgalindo3   (503) staff       (20)        0 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/images/small-white.png
--rw-r--r--   0 pgalindo3   (503) staff       (20)    62611 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/latex.txt
--rw-r--r--   0 pgalindo3   (503) staff       (20)    15571 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/links.txt
--rw-r--r--   0 pgalindo3   (503) staff       (20)     5543 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/mailing-lists.txt
--rw-r--r--   0 pgalindo3   (503) staff       (20)     5202 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/manpage.txt
--rw-r--r--   0 pgalindo3   (503) staff       (20)    38313 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/odt.txt
-drwxr-xr-x   0 pgalindo3   (503) staff       (20)        0 2022-11-20 19:57:43.166929 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/rst/
--rw-r--r--   0 pgalindo3   (503) staff       (20)     7097 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/rst/cheatsheet.txt
--rw-r--r--   0 pgalindo3   (503) staff       (20)    15080 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/rst/demo.txt
-drwxr-xr-x   0 pgalindo3   (503) staff       (20)        0 2022-11-20 19:57:43.168113 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/rst/images/
--rw-r--r--   0 pgalindo3   (503) staff       (20)        0 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/rst/images/biohazard-bitmap-scaling.svg
--rw-r--r--   0 pgalindo3   (503) staff       (20)        0 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/rst/images/biohazard-bitmap.svg
--rw-r--r--   0 pgalindo3   (503) staff       (20)        0 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/rst/images/biohazard-scaling.svg
--rw-r--r--   0 pgalindo3   (503) staff       (20)        0 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/rst/images/biohazard.png
--rw-r--r--   0 pgalindo3   (503) staff       (20)        0 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/rst/images/biohazard.svg
--rw-r--r--   0 pgalindo3   (503) staff       (20)        0 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/rst/images/biohazard.swf
--rw-r--r--   0 pgalindo3   (503) staff       (20)        0 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/rst/images/pens.mp4
--rw-r--r--   0 pgalindo3   (503) staff       (20)        0 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/rst/images/title-scaling.svg
--rw-r--r--   0 pgalindo3   (503) staff       (20)        0 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/rst/images/title.png
--rw-r--r--   0 pgalindo3   (503) staff       (20)        0 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/rst/images/title.svg
--rw-r--r--   0 pgalindo3   (503) staff       (20)    11268 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/rst/quickstart.txt
--rw-r--r--   0 pgalindo3   (503) staff       (20)    12042 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/smartquotes.txt
--rw-r--r--   0 pgalindo3   (503) staff       (20)    17347 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/tools.txt
--rw-r--r--   0 pgalindo3   (503) staff       (20)      256 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/pyproject.toml
--rw-r--r--   0 pgalindo3   (503) staff       (20)       17 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/requirements.txt
--rw-r--r--   0 pgalindo3   (503) staff       (20)     1603 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/run_benchmark.py
-drwxr-xr-x   0 pgalindo3   (503) staff       (20)        0 2022-11-20 19:57:43.168459 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_dulwich_log/
-drwxr-xr-x   0 pgalindo3   (503) staff       (20)        0 2022-11-20 19:57:43.144482 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_dulwich_log/data/
-drwxr-xr-x   0 pgalindo3   (503) staff       (20)        0 2022-11-20 19:57:43.169480 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/
--rw-r--r--   0 pgalindo3   (503) staff       (20)     1452 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/COMMIT_EDITMSG
--rw-r--r--   0 pgalindo3   (503) staff       (20)       87 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/FETCH_HEAD
--rw-r--r--   0 pgalindo3   (503) staff       (20)       23 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/HEAD
--rw-r--r--   0 pgalindo3   (503) staff       (20)       41 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/ORIG_HEAD
--rw-r--r--   0 pgalindo3   (503) staff       (20)      258 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/config
--rw-r--r--   0 pgalindo3   (503) staff       (20)       73 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/description
-drwxr-xr-x   0 pgalindo3   (503) staff       (20)        0 2022-11-20 19:57:43.170627 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/hooks/
--rwxr-xr-x   0 pgalindo3   (503) staff       (20)      452 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/hooks/applypatch-msg.sample
--rwxr-xr-x   0 pgalindo3   (503) staff       (20)      896 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/hooks/commit-msg.sample
--rwxr-xr-x   0 pgalindo3   (503) staff       (20)      189 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/hooks/post-update.sample
--rwxr-xr-x   0 pgalindo3   (503) staff       (20)      398 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/hooks/pre-applypatch.sample
--rwxr-xr-x   0 pgalindo3   (503) staff       (20)     1642 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/hooks/pre-commit.sample
--rwxr-xr-x   0 pgalindo3   (503) staff       (20)     1348 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/hooks/pre-push.sample
--rwxr-xr-x   0 pgalindo3   (503) staff       (20)     4951 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/hooks/pre-rebase.sample
--rwxr-xr-x   0 pgalindo3   (503) staff       (20)     1239 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/hooks/prepare-commit-msg.sample
--rwxr-xr-x   0 pgalindo3   (503) staff       (20)     3611 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/hooks/update.sample
--rw-r--r--   0 pgalindo3   (503) staff       (20)     8508 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/index
-drwxr-xr-x   0 pgalindo3   (503) staff       (20)        0 2022-11-20 19:57:43.170866 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/info/
--rw-r--r--   0 pgalindo3   (503) staff       (20)      240 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/info/exclude
--rw-r--r--   0 pgalindo3   (503) staff       (20)     1538 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/info/refs
-drwxr-xr-x   0 pgalindo3   (503) staff       (20)        0 2022-11-20 19:57:43.170989 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/logs/
--rw-r--r--   0 pgalindo3   (503) staff       (20)      385 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/logs/HEAD
-drwxr-xr-x   0 pgalindo3   (503) staff       (20)        0 2022-11-20 19:57:43.144795 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/logs/refs/
-drwxr-xr-x   0 pgalindo3   (503) staff       (20)        0 2022-11-20 19:57:43.171097 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/logs/refs/heads/
--rw-r--r--   0 pgalindo3   (503) staff       (20)      217 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/logs/refs/heads/master
-drwxr-xr-x   0 pgalindo3   (503) staff       (20)        0 2022-11-20 19:57:43.144843 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/logs/refs/remotes/
-drwxr-xr-x   0 pgalindo3   (503) staff       (20)        0 2022-11-20 19:57:43.171502 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/logs/refs/remotes/origin/
--rw-r--r--   0 pgalindo3   (503) staff       (20)        0 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/logs/refs/remotes/origin/HEAD
--rw-r--r--   0 pgalindo3   (503) staff       (20)        0 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/logs/refs/remotes/origin/bind_modules
--rw-r--r--   0 pgalindo3   (503) staff       (20)      164 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/logs/refs/remotes/origin/master
--rw-r--r--   0 pgalindo3   (503) staff       (20)        0 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/logs/refs/remotes/origin/zero_timeout
-drwxr-xr-x   0 pgalindo3   (503) staff       (20)        0 2022-11-20 19:57:43.145022 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/objects/
-drwxr-xr-x   0 pgalindo3   (503) staff       (20)        0 2022-11-20 19:57:43.171604 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/objects/info/
--rw-r--r--   0 pgalindo3   (503) staff       (20)       54 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/objects/info/packs
-drwxr-xr-x   0 pgalindo3   (503) staff       (20)        0 2022-11-20 19:57:43.172040 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/objects/pack/
--rw-r--r--   0 pgalindo3   (503) staff       (20)   247416 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/objects/pack/pack-7e1b1ace85030071ca314cd565ae038bacc302a4.idx
--rw-r--r--   0 pgalindo3   (503) staff       (20)  1774473 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/objects/pack/pack-7e1b1ace85030071ca314cd565ae038bacc302a4.pack
--rw-r--r--   0 pgalindo3   (503) staff       (20)     1511 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/packed-refs
-drwxr-xr-x   0 pgalindo3   (503) staff       (20)        0 2022-11-20 19:57:43.145125 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/refs/
-drwxr-xr-x   0 pgalindo3   (503) staff       (20)        0 2022-11-20 19:57:43.145169 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/refs/remotes/
-drwxr-xr-x   0 pgalindo3   (503) staff       (20)        0 2022-11-20 19:57:43.173261 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/refs/remotes/origin/
--rw-r--r--   0 pgalindo3   (503) staff       (20)       32 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/refs/remotes/origin/HEAD
--rw-r--r--   0 pgalindo3   (503) staff       (20)      263 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_dulwich_log/pyproject.toml
--rw-r--r--   0 pgalindo3   (503) staff       (20)       52 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_dulwich_log/requirements.txt
--rw-r--r--   0 pgalindo3   (503) staff       (20)      672 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_dulwich_log/run_benchmark.py
-drwxr-xr-x   0 pgalindo3   (503) staff       (20)        0 2022-11-20 19:57:43.173536 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_fannkuch/
--rw-r--r--   0 pgalindo3   (503) staff       (20)      223 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_fannkuch/pyproject.toml
--rw-r--r--   0 pgalindo3   (503) staff       (20)     1118 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_fannkuch/run_benchmark.py
-drwxr-xr-x   0 pgalindo3   (503) staff       (20)        0 2022-11-20 19:57:43.173805 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_float/
--rw-r--r--   0 pgalindo3   (503) staff       (20)      231 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_float/pyproject.toml
--rw-r--r--   0 pgalindo3   (503) staff       (20)     1293 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_float/run_benchmark.py
-drwxr-xr-x   0 pgalindo3   (503) staff       (20)        0 2022-11-20 19:57:43.174017 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_gc_collect/
--rw-r--r--   0 pgalindo3   (503) staff       (20)      227 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_gc_collect/pyproject.toml
--rw-r--r--   0 pgalindo3   (503) staff       (20)     1394 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_gc_collect/run_benchmark.py
-drwxr-xr-x   0 pgalindo3   (503) staff       (20)        0 2022-11-20 19:57:43.174255 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_gc_traversal/
--rw-r--r--   0 pgalindo3   (503) staff       (20)      231 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_gc_traversal/pyproject.toml
--rw-r--r--   0 pgalindo3   (503) staff       (20)      866 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_gc_traversal/run_benchmark.py
-drwxr-xr-x   0 pgalindo3   (503) staff       (20)        0 2022-11-20 19:57:43.174478 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_generators/
--rw-r--r--   0 pgalindo3   (503) staff       (20)      227 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_generators/pyproject.toml
--rw-r--r--   0 pgalindo3   (503) staff       (20)     1201 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_generators/run_benchmark.py
-drwxr-xr-x   0 pgalindo3   (503) staff       (20)        0 2022-11-20 19:57:43.174842 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_genshi/
--rw-r--r--   0 pgalindo3   (503) staff       (20)      258 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_genshi/pyproject.toml
--rw-r--r--   0 pgalindo3   (503) staff       (20)       26 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_genshi/requirements.txt
--rw-r--r--   0 pgalindo3   (503) staff       (20)     1606 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_genshi/run_benchmark.py
-drwxr-xr-x   0 pgalindo3   (503) staff       (20)        0 2022-11-20 19:57:43.175114 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_go/
--rw-r--r--   0 pgalindo3   (503) staff       (20)      211 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_go/pyproject.toml
--rw-r--r--   0 pgalindo3   (503) staff       (20)    14055 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_go/run_benchmark.py
-drwxr-xr-x   0 pgalindo3   (503) staff       (20)        0 2022-11-20 19:57:43.175357 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_hexiom/
--rw-r--r--   0 pgalindo3   (503) staff       (20)      219 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_hexiom/pyproject.toml
--rw-r--r--   0 pgalindo3   (503) staff       (20)    17501 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_hexiom/run_benchmark.py
-drwxr-xr-x   0 pgalindo3   (503) staff       (20)        0 2022-11-20 19:57:43.175763 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_hg_startup/
--rw-r--r--   0 pgalindo3   (503) staff       (20)      268 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_hg_startup/pyproject.toml
--rw-r--r--   0 pgalindo3   (503) staff       (20)       15 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_hg_startup/requirements.txt
--rw-r--r--   0 pgalindo3   (503) staff       (20)     1150 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_hg_startup/run_benchmark.py
-drwxr-xr-x   0 pgalindo3   (503) staff       (20)        0 2022-11-20 19:57:43.176129 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_html5lib/
-drwxr-xr-x   0 pgalindo3   (503) staff       (20)        0 2022-11-20 19:57:43.176246 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_html5lib/data/
--rw-r--r--   0 pgalindo3   (503) staff       (20)   133837 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_html5lib/data/w3_tr_html5.html
--rw-r--r--   0 pgalindo3   (503) staff       (20)      260 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_html5lib/pyproject.toml
--rw-r--r--   0 pgalindo3   (503) staff       (20)       46 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_html5lib/requirements.txt
--rw-r--r--   0 pgalindo3   (503) staff       (20)      916 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_html5lib/run_benchmark.py
-drwxr-xr-x   0 pgalindo3   (503) staff       (20)        0 2022-11-20 19:57:43.176585 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_json_dumps/
--rw-r--r--   0 pgalindo3   (503) staff       (20)      246 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_json_dumps/pyproject.toml
--rw-r--r--   0 pgalindo3   (503) staff       (20)     1564 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_json_dumps/run_benchmark.py
-drwxr-xr-x   0 pgalindo3   (503) staff       (20)        0 2022-11-20 19:57:43.176834 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_json_loads/
--rw-r--r--   0 pgalindo3   (503) staff       (20)      246 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_json_loads/pyproject.toml
--rw-r--r--   0 pgalindo3   (503) staff       (20)     2812 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_json_loads/run_benchmark.py
-drwxr-xr-x   0 pgalindo3   (503) staff       (20)        0 2022-11-20 19:57:43.177090 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_logging/
--rw-r--r--   0 pgalindo3   (503) staff       (20)      221 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_logging/pyproject.toml
--rw-r--r--   0 pgalindo3   (503) staff       (20)     4156 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_logging/run_benchmark.py
-drwxr-xr-x   0 pgalindo3   (503) staff       (20)        0 2022-11-20 19:57:43.177476 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_mako/
--rw-r--r--   0 pgalindo3   (503) staff       (20)      253 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_mako/pyproject.toml
--rw-r--r--   0 pgalindo3   (503) staff       (20)       30 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_mako/requirements.txt
--rw-r--r--   0 pgalindo3   (503) staff       (20)     3742 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_mako/run_benchmark.py
-drwxr-xr-x   0 pgalindo3   (503) staff       (20)        0 2022-11-20 19:57:43.177755 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_mdp/
--rw-r--r--   0 pgalindo3   (503) staff       (20)      213 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_mdp/pyproject.toml
--rw-r--r--   0 pgalindo3   (503) staff       (20)     8797 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_mdp/run_benchmark.py
-drwxr-xr-x   0 pgalindo3   (503) staff       (20)        0 2022-11-20 19:57:43.178005 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_meteor_contest/
--rw-r--r--   0 pgalindo3   (503) staff       (20)      235 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_meteor_contest/pyproject.toml
--rw-r--r--   0 pgalindo3   (503) staff       (20)     8011 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_meteor_contest/run_benchmark.py
-drwxr-xr-x   0 pgalindo3   (503) staff       (20)        0 2022-11-20 19:57:43.178265 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_nbody/
--rw-r--r--   0 pgalindo3   (503) staff       (20)      231 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_nbody/pyproject.toml
--rw-r--r--   0 pgalindo3   (503) staff       (20)     5039 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_nbody/run_benchmark.py
-drwxr-xr-x   0 pgalindo3   (503) staff       (20)        0 2022-11-20 19:57:43.178477 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_nqueens/
--rw-r--r--   0 pgalindo3   (503) staff       (20)      221 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_nqueens/pyproject.toml
--rw-r--r--   0 pgalindo3   (503) staff       (20)     1861 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_nqueens/run_benchmark.py
-drwxr-xr-x   0 pgalindo3   (503) staff       (20)        0 2022-11-20 19:57:43.178696 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_pathlib/
--rw-r--r--   0 pgalindo3   (503) staff       (20)      221 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_pathlib/pyproject.toml
--rw-r--r--   0 pgalindo3   (503) staff       (20)     1851 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_pathlib/run_benchmark.py
-drwxr-xr-x   0 pgalindo3   (503) staff       (20)        0 2022-11-20 19:57:43.179530 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_pickle/
--rw-r--r--   0 pgalindo3   (503) staff       (20)      277 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_pickle/bm_pickle_dict.toml
--rw-r--r--   0 pgalindo3   (503) staff       (20)      277 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_pickle/bm_pickle_list.toml
--rw-r--r--   0 pgalindo3   (503) staff       (20)      303 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_pickle/bm_pickle_pure_python.toml
--rw-r--r--   0 pgalindo3   (503) staff       (20)      268 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_pickle/bm_unpickle.toml
--rw-r--r--   0 pgalindo3   (503) staff       (20)      283 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_pickle/bm_unpickle_list.toml
--rw-r--r--   0 pgalindo3   (503) staff       (20)      309 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_pickle/bm_unpickle_pure_python.toml
--rw-r--r--   0 pgalindo3   (503) staff       (20)      262 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_pickle/pyproject.toml
--rw-r--r--   0 pgalindo3   (503) staff       (20)     8216 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_pickle/run_benchmark.py
-drwxr-xr-x   0 pgalindo3   (503) staff       (20)        0 2022-11-20 19:57:43.179736 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_pidigits/
--rw-r--r--   0 pgalindo3   (503) staff       (20)      237 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_pidigits/pyproject.toml
--rw-r--r--   0 pgalindo3   (503) staff       (20)     1542 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_pidigits/run_benchmark.py
-drwxr-xr-x   0 pgalindo3   (503) staff       (20)        0 2022-11-20 19:57:43.179935 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_pprint/
--rw-r--r--   0 pgalindo3   (503) staff       (20)      219 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_pprint/pyproject.toml
--rw-r--r--   0 pgalindo3   (503) staff       (20)      647 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_pprint/run_benchmark.py
-drwxr-xr-x   0 pgalindo3   (503) staff       (20)        0 2022-11-20 19:57:43.180137 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_pyflate/
-drwxr-xr-x   0 pgalindo3   (503) staff       (20)        0 2022-11-20 19:57:43.180271 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_pyflate/data/
--rw-r--r--   0 pgalindo3   (503) staff       (20)    67562 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_pyflate/data/interpreter.tar.bz2
--rw-r--r--   0 pgalindo3   (503) staff       (20)      221 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_pyflate/pyproject.toml
--rwxr-xr-x   0 pgalindo3   (503) staff       (20)    20078 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_pyflate/run_benchmark.py
-drwxr-xr-x   0 pgalindo3   (503) staff       (20)        0 2022-11-20 19:57:43.180630 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_python_startup/
--rw-r--r--   0 pgalindo3   (503) staff       (20)      295 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_python_startup/bm_python_startup_no_site.toml
--rw-r--r--   0 pgalindo3   (503) staff       (20)      252 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_python_startup/pyproject.toml
--rw-r--r--   0 pgalindo3   (503) staff       (20)      900 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_python_startup/run_benchmark.py
-drwxr-xr-x   0 pgalindo3   (503) staff       (20)        0 2022-11-20 19:57:43.180841 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_raytrace/
--rw-r--r--   0 pgalindo3   (503) staff       (20)      223 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_raytrace/pyproject.toml
--rw-r--r--   0 pgalindo3   (503) staff       (20)    12042 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_raytrace/run_benchmark.py
-drwxr-xr-x   0 pgalindo3   (503) staff       (20)        0 2022-11-20 19:57:43.181326 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_regex_compile/
--rw-r--r--   0 pgalindo3   (503) staff       (20)     5325 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_regex_compile/bm_regex_effbot.py
--rw-r--r--   0 pgalindo3   (503) staff       (20)   125978 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_regex_compile/bm_regex_v8.py
--rw-r--r--   0 pgalindo3   (503) staff       (20)      248 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_regex_compile/pyproject.toml
--rw-r--r--   0 pgalindo3   (503) staff       (20)     1778 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_regex_compile/run_benchmark.py
-drwxr-xr-x   0 pgalindo3   (503) staff       (20)        0 2022-11-20 19:57:43.181530 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_regex_dna/
--rw-r--r--   0 pgalindo3   (503) staff       (20)      240 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_regex_dna/pyproject.toml
--rw-r--r--   0 pgalindo3   (503) staff       (20)     6731 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_regex_dna/run_benchmark.py
-drwxr-xr-x   0 pgalindo3   (503) staff       (20)        0 2022-11-20 19:57:43.181742 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_regex_effbot/
--rw-r--r--   0 pgalindo3   (503) staff       (20)      246 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_regex_effbot/pyproject.toml
--rw-r--r--   0 pgalindo3   (503) staff       (20)     5325 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_regex_effbot/run_benchmark.py
-drwxr-xr-x   0 pgalindo3   (503) staff       (20)        0 2022-11-20 19:57:43.181948 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_regex_v8/
--rw-r--r--   0 pgalindo3   (503) staff       (20)      238 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_regex_v8/pyproject.toml
--rw-r--r--   0 pgalindo3   (503) staff       (20)   125978 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_regex_v8/run_benchmark.py
-drwxr-xr-x   0 pgalindo3   (503) staff       (20)        0 2022-11-20 19:57:43.182237 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_richards/
--rw-r--r--   0 pgalindo3   (503) staff       (20)      223 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_richards/pyproject.toml
--rw-r--r--   0 pgalindo3   (503) staff       (20)     9539 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_richards/run_benchmark.py
-drwxr-xr-x   0 pgalindo3   (503) staff       (20)        0 2022-11-20 19:57:43.182450 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_scimark/
--rw-r--r--   0 pgalindo3   (503) staff       (20)      221 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_scimark/pyproject.toml
--rw-r--r--   0 pgalindo3   (503) staff       (20)    10173 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_scimark/run_benchmark.py
-drwxr-xr-x   0 pgalindo3   (503) staff       (20)        0 2022-11-20 19:57:43.182661 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_spectral_norm/
--rw-r--r--   0 pgalindo3   (503) staff       (20)      233 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_spectral_norm/pyproject.toml
--rw-r--r--   0 pgalindo3   (503) staff       (20)     1706 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_spectral_norm/run_benchmark.py
-drwxr-xr-x   0 pgalindo3   (503) staff       (20)        0 2022-11-20 19:57:43.183044 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_sqlalchemy_declarative/
--rw-r--r--   0 pgalindo3   (503) staff       (20)      276 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_sqlalchemy_declarative/pyproject.toml
--rw-r--r--   0 pgalindo3   (503) staff       (20)       37 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_sqlalchemy_declarative/requirements.txt
--rw-r--r--   0 pgalindo3   (503) staff       (20)     3388 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_sqlalchemy_declarative/run_benchmark.py
-drwxr-xr-x   0 pgalindo3   (503) staff       (20)        0 2022-11-20 19:57:43.183378 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_sqlalchemy_imperative/
--rw-r--r--   0 pgalindo3   (503) staff       (20)      274 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_sqlalchemy_imperative/pyproject.toml
--rw-r--r--   0 pgalindo3   (503) staff       (20)       37 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_sqlalchemy_imperative/requirements.txt
--rw-r--r--   0 pgalindo3   (503) staff       (20)     3033 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_sqlalchemy_imperative/run_benchmark.py
-drwxr-xr-x   0 pgalindo3   (503) staff       (20)        0 2022-11-20 19:57:43.183693 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_sqlglot/
--rw-r--r--   0 pgalindo3   (503) staff       (20)      243 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_sqlglot/pyproject.toml
--rw-r--r--   0 pgalindo3   (503) staff       (20)       15 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_sqlglot/requirements.txt
--rw-r--r--   0 pgalindo3   (503) staff       (20)     4892 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_sqlglot/run_benchmark.py
-drwxr-xr-x   0 pgalindo3   (503) staff       (20)        0 2022-11-20 19:57:43.183902 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_sqlite_synth/
--rw-r--r--   0 pgalindo3   (503) staff       (20)      231 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_sqlite_synth/pyproject.toml
--rw-r--r--   0 pgalindo3   (503) staff       (20)     1395 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_sqlite_synth/run_benchmark.py
-drwxr-xr-x   0 pgalindo3   (503) staff       (20)        0 2022-11-20 19:57:43.184211 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_sympy/
--rw-r--r--   0 pgalindo3   (503) staff       (20)      237 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_sympy/pyproject.toml
--rw-r--r--   0 pgalindo3   (503) staff       (20)       25 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_sympy/requirements.txt
--rw-r--r--   0 pgalindo3   (503) staff       (20)     1496 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_sympy/run_benchmark.py
-drwxr-xr-x   0 pgalindo3   (503) staff       (20)        0 2022-11-20 19:57:43.184439 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_telco/
-drwxr-xr-x   0 pgalindo3   (503) staff       (20)        0 2022-11-20 19:57:43.184609 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_telco/data/
--rw-r--r--   0 pgalindo3   (503) staff       (20)   160000 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_telco/data/telco-bench.b
--rw-r--r--   0 pgalindo3   (503) staff       (20)      217 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_telco/pyproject.toml
--rw-r--r--   0 pgalindo3   (503) staff       (20)     3001 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_telco/run_benchmark.py
-drwxr-xr-x   0 pgalindo3   (503) staff       (20)        0 2022-11-20 19:57:43.185089 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_tornado_http/
--rw-r--r--   0 pgalindo3   (503) staff       (20)      267 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_tornado_http/pyproject.toml
--rw-r--r--   0 pgalindo3   (503) staff       (20)       13 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_tornado_http/requirements.txt
--rw-r--r--   0 pgalindo3   (503) staff       (20)     2910 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_tornado_http/run_benchmark.py
-drwxr-xr-x   0 pgalindo3   (503) staff       (20)        0 2022-11-20 19:57:43.185352 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_unpack_sequence/
--rw-r--r--   0 pgalindo3   (503) staff       (20)      237 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_unpack_sequence/pyproject.toml
--rw-r--r--   0 pgalindo3   (503) staff       (20)    20968 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_unpack_sequence/run_benchmark.py
-drwxr-xr-x   0 pgalindo3   (503) staff       (20)        0 2022-11-20 19:57:43.185605 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_xml_etree/
--rw-r--r--   0 pgalindo3   (503) staff       (20)      244 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_xml_etree/pyproject.toml
--rw-r--r--   0 pgalindo3   (503) staff       (20)     9514 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_xml_etree/run_benchmark.py
--rw-r--r--   0 pgalindo3   (503) staff       (20)      359 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/data-files/requirements.txt
--rw-r--r--   0 pgalindo3   (503) staff       (20)     5965 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/run.py
--rw-r--r--   0 pgalindo3   (503) staff       (20)     7717 2022-11-20 19:47:21.000000 pyperformance-1.0.6/pyperformance/venv.py
-drwxr-xr-x   0 pgalindo3   (503) staff       (20)        0 2022-11-20 19:57:43.153529 pyperformance-1.0.6/pyperformance.egg-info/
--rw-r--r--   0 pgalindo3   (503) staff       (20)     1744 2022-11-20 19:57:43.000000 pyperformance-1.0.6/pyperformance.egg-info/PKG-INFO
--rw-r--r--   0 pgalindo3   (503) staff       (20)    19898 2022-11-20 19:57:43.000000 pyperformance-1.0.6/pyperformance.egg-info/SOURCES.txt
--rw-r--r--   0 pgalindo3   (503) staff       (20)        1 2022-11-20 19:57:43.000000 pyperformance-1.0.6/pyperformance.egg-info/dependency_links.txt
--rw-r--r--   0 pgalindo3   (503) staff       (20)       57 2022-11-20 19:57:43.000000 pyperformance-1.0.6/pyperformance.egg-info/entry_points.txt
--rw-r--r--   0 pgalindo3   (503) staff       (20)       22 2022-11-20 19:57:43.000000 pyperformance-1.0.6/pyperformance.egg-info/requires.txt
--rw-r--r--   0 pgalindo3   (503) staff       (20)       14 2022-11-20 19:57:43.000000 pyperformance-1.0.6/pyperformance.egg-info/top_level.txt
--rw-r--r--   0 pgalindo3   (503) staff       (20)      598 2022-11-20 19:47:21.000000 pyperformance-1.0.6/requirements.in
--rw-r--r--   0 pgalindo3   (503) staff       (20)      359 2022-11-20 19:47:21.000000 pyperformance-1.0.6/requirements.txt
--rw-r--r--   0 pgalindo3   (503) staff       (20)       38 2022-11-20 19:57:43.185965 pyperformance-1.0.6/setup.cfg
--rw-r--r--   0 pgalindo3   (503) staff       (20)     2338 2022-11-20 19:47:21.000000 pyperformance-1.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.877154 pyperformance-1.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-04-23 06:20:54.000000 pyperformance-1.0.7/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-04-23 06:20:54.000000 pyperformance-1.0.7/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-04-23 06:20:54.000000 pyperformance-1.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-04-23 06:21:09.877154 pyperformance-1.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-04-23 06:20:54.000000 pyperformance-1.0.7/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4325 2023-04-23 06:20:54.000000 pyperformance-1.0.7/TODO.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.801153 pyperformance-1.0.7/benchmarks/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.809153 pyperformance-1.0.7/benchmarks/bm_2to3/
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-23 06:20:54.000000 pyperformance-1.0.7/benchmarks/bm_2to3/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.809153 pyperformance-1.0.7/benchmarks/bm_async_generators/
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-04-23 06:20:54.000000 pyperformance-1.0.7/benchmarks/bm_async_generators/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.809153 pyperformance-1.0.7/benchmarks/bm_async_tree/
+-rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-04-23 06:20:54.000000 pyperformance-1.0.7/benchmarks/bm_async_tree/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.809153 pyperformance-1.0.7/benchmarks/bm_asyncio_tcp/
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-04-23 06:20:54.000000 pyperformance-1.0.7/benchmarks/bm_asyncio_tcp/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.809153 pyperformance-1.0.7/benchmarks/bm_chameleon/
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-04-23 06:20:54.000000 pyperformance-1.0.7/benchmarks/bm_chameleon/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.809153 pyperformance-1.0.7/benchmarks/bm_chaos/
+-rw-r--r--   0 runner    (1001) docker     (123)    10709 2023-04-23 06:20:54.000000 pyperformance-1.0.7/benchmarks/bm_chaos/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.809153 pyperformance-1.0.7/benchmarks/bm_comprehensions/
+-rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-04-23 06:20:54.000000 pyperformance-1.0.7/benchmarks/bm_comprehensions/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.809153 pyperformance-1.0.7/benchmarks/bm_concurrent_imap/
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-04-23 06:20:54.000000 pyperformance-1.0.7/benchmarks/bm_concurrent_imap/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.809153 pyperformance-1.0.7/benchmarks/bm_coroutines/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-23 06:20:54.000000 pyperformance-1.0.7/benchmarks/bm_coroutines/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.809153 pyperformance-1.0.7/benchmarks/bm_coverage/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-23 06:20:54.000000 pyperformance-1.0.7/benchmarks/bm_coverage/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.809153 pyperformance-1.0.7/benchmarks/bm_crypto_pyaes/
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-04-23 06:20:54.000000 pyperformance-1.0.7/benchmarks/bm_crypto_pyaes/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.809153 pyperformance-1.0.7/benchmarks/bm_dask/
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-04-23 06:20:54.000000 pyperformance-1.0.7/benchmarks/bm_dask/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.809153 pyperformance-1.0.7/benchmarks/bm_deepcopy/
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-04-23 06:20:54.000000 pyperformance-1.0.7/benchmarks/bm_deepcopy/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.809153 pyperformance-1.0.7/benchmarks/bm_deltablue/
+-rw-r--r--   0 runner    (1001) docker     (123)    17136 2023-04-23 06:20:54.000000 pyperformance-1.0.7/benchmarks/bm_deltablue/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.809153 pyperformance-1.0.7/benchmarks/bm_django_template/
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-04-23 06:20:54.000000 pyperformance-1.0.7/benchmarks/bm_django_template/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.809153 pyperformance-1.0.7/benchmarks/bm_docutils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-04-23 06:20:54.000000 pyperformance-1.0.7/benchmarks/bm_docutils/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.809153 pyperformance-1.0.7/benchmarks/bm_dulwich_log/
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-23 06:20:54.000000 pyperformance-1.0.7/benchmarks/bm_dulwich_log/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.809153 pyperformance-1.0.7/benchmarks/bm_fannkuch/
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-04-23 06:20:54.000000 pyperformance-1.0.7/benchmarks/bm_fannkuch/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.809153 pyperformance-1.0.7/benchmarks/bm_float/
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-04-23 06:20:54.000000 pyperformance-1.0.7/benchmarks/bm_float/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.809153 pyperformance-1.0.7/benchmarks/bm_gc_collect/
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-04-23 06:20:54.000000 pyperformance-1.0.7/benchmarks/bm_gc_collect/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.809153 pyperformance-1.0.7/benchmarks/bm_gc_traversal/
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-04-23 06:20:54.000000 pyperformance-1.0.7/benchmarks/bm_gc_traversal/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.809153 pyperformance-1.0.7/benchmarks/bm_generators/
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-04-23 06:20:54.000000 pyperformance-1.0.7/benchmarks/bm_generators/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.809153 pyperformance-1.0.7/benchmarks/bm_genshi/
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-04-23 06:20:54.000000 pyperformance-1.0.7/benchmarks/bm_genshi/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.813153 pyperformance-1.0.7/benchmarks/bm_go/
+-rw-r--r--   0 runner    (1001) docker     (123)    13911 2023-04-23 06:20:54.000000 pyperformance-1.0.7/benchmarks/bm_go/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.813153 pyperformance-1.0.7/benchmarks/bm_hexiom/
+-rw-r--r--   0 runner    (1001) docker     (123)    17354 2023-04-23 06:20:54.000000 pyperformance-1.0.7/benchmarks/bm_hexiom/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.813153 pyperformance-1.0.7/benchmarks/bm_hg_startup/
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-04-23 06:20:54.000000 pyperformance-1.0.7/benchmarks/bm_hg_startup/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.813153 pyperformance-1.0.7/benchmarks/bm_html5lib/
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-04-23 06:20:54.000000 pyperformance-1.0.7/benchmarks/bm_html5lib/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.813153 pyperformance-1.0.7/benchmarks/bm_json_dumps/
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-04-23 06:20:54.000000 pyperformance-1.0.7/benchmarks/bm_json_dumps/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.813153 pyperformance-1.0.7/benchmarks/bm_json_loads/
+-rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-04-23 06:20:54.000000 pyperformance-1.0.7/benchmarks/bm_json_loads/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.813153 pyperformance-1.0.7/benchmarks/bm_logging/
+-rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-04-23 06:20:54.000000 pyperformance-1.0.7/benchmarks/bm_logging/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.813153 pyperformance-1.0.7/benchmarks/bm_mako/
+-rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-04-23 06:20:54.000000 pyperformance-1.0.7/benchmarks/bm_mako/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.813153 pyperformance-1.0.7/benchmarks/bm_mdp/
+-rw-r--r--   0 runner    (1001) docker     (123)     8797 2023-04-23 06:20:54.000000 pyperformance-1.0.7/benchmarks/bm_mdp/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.813153 pyperformance-1.0.7/benchmarks/bm_meteor_contest/
+-rw-r--r--   0 runner    (1001) docker     (123)     8011 2023-04-23 06:20:54.000000 pyperformance-1.0.7/benchmarks/bm_meteor_contest/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.813153 pyperformance-1.0.7/benchmarks/bm_nbody/
+-rw-r--r--   0 runner    (1001) docker     (123)     5039 2023-04-23 06:20:54.000000 pyperformance-1.0.7/benchmarks/bm_nbody/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.813153 pyperformance-1.0.7/benchmarks/bm_nqueens/
+-rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-04-23 06:20:54.000000 pyperformance-1.0.7/benchmarks/bm_nqueens/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.813153 pyperformance-1.0.7/benchmarks/bm_pathlib/
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-04-23 06:20:54.000000 pyperformance-1.0.7/benchmarks/bm_pathlib/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.813153 pyperformance-1.0.7/benchmarks/bm_pickle/
+-rw-r--r--   0 runner    (1001) docker     (123)     8216 2023-04-23 06:20:54.000000 pyperformance-1.0.7/benchmarks/bm_pickle/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.813153 pyperformance-1.0.7/benchmarks/bm_pidigits/
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-04-23 06:20:54.000000 pyperformance-1.0.7/benchmarks/bm_pidigits/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.813153 pyperformance-1.0.7/benchmarks/bm_pprint/
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-04-23 06:20:54.000000 pyperformance-1.0.7/benchmarks/bm_pprint/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.813153 pyperformance-1.0.7/benchmarks/bm_pyflate/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    20078 2023-04-23 06:20:54.000000 pyperformance-1.0.7/benchmarks/bm_pyflate/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.813153 pyperformance-1.0.7/benchmarks/bm_python_startup/
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-04-23 06:20:54.000000 pyperformance-1.0.7/benchmarks/bm_python_startup/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.813153 pyperformance-1.0.7/benchmarks/bm_raytrace/
+-rw-r--r--   0 runner    (1001) docker     (123)    12042 2023-04-23 06:20:54.000000 pyperformance-1.0.7/benchmarks/bm_raytrace/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.813153 pyperformance-1.0.7/benchmarks/bm_regex_compile/
+-rw-r--r--   0 runner    (1001) docker     (123)     5325 2023-04-23 06:20:54.000000 pyperformance-1.0.7/benchmarks/bm_regex_compile/bm_regex_effbot.py
+-rw-r--r--   0 runner    (1001) docker     (123)   125978 2023-04-23 06:20:54.000000 pyperformance-1.0.7/benchmarks/bm_regex_compile/bm_regex_v8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-04-23 06:20:54.000000 pyperformance-1.0.7/benchmarks/bm_regex_compile/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.813153 pyperformance-1.0.7/benchmarks/bm_regex_dna/
+-rw-r--r--   0 runner    (1001) docker     (123)     6731 2023-04-23 06:20:54.000000 pyperformance-1.0.7/benchmarks/bm_regex_dna/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.813153 pyperformance-1.0.7/benchmarks/bm_regex_effbot/
+-rw-r--r--   0 runner    (1001) docker     (123)     5325 2023-04-23 06:20:54.000000 pyperformance-1.0.7/benchmarks/bm_regex_effbot/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.813153 pyperformance-1.0.7/benchmarks/bm_regex_v8/
+-rw-r--r--   0 runner    (1001) docker     (123)   125978 2023-04-23 06:20:54.000000 pyperformance-1.0.7/benchmarks/bm_regex_v8/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.813153 pyperformance-1.0.7/benchmarks/bm_richards/
+-rw-r--r--   0 runner    (1001) docker     (123)     9539 2023-04-23 06:20:54.000000 pyperformance-1.0.7/benchmarks/bm_richards/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.813153 pyperformance-1.0.7/benchmarks/bm_scimark/
+-rw-r--r--   0 runner    (1001) docker     (123)    10173 2023-04-23 06:20:54.000000 pyperformance-1.0.7/benchmarks/bm_scimark/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.813153 pyperformance-1.0.7/benchmarks/bm_spectral_norm/
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-04-23 06:20:54.000000 pyperformance-1.0.7/benchmarks/bm_spectral_norm/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.817154 pyperformance-1.0.7/benchmarks/bm_sqlalchemy_declarative/
+-rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-04-23 06:20:54.000000 pyperformance-1.0.7/benchmarks/bm_sqlalchemy_declarative/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.817154 pyperformance-1.0.7/benchmarks/bm_sqlalchemy_imperative/
+-rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-04-23 06:20:54.000000 pyperformance-1.0.7/benchmarks/bm_sqlalchemy_imperative/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.817154 pyperformance-1.0.7/benchmarks/bm_sqlglot/
+-rw-r--r--   0 runner    (1001) docker     (123)     4892 2023-04-23 06:20:54.000000 pyperformance-1.0.7/benchmarks/bm_sqlglot/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.817154 pyperformance-1.0.7/benchmarks/bm_sqlite_synth/
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-04-23 06:20:54.000000 pyperformance-1.0.7/benchmarks/bm_sqlite_synth/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.817154 pyperformance-1.0.7/benchmarks/bm_sympy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-04-23 06:20:54.000000 pyperformance-1.0.7/benchmarks/bm_sympy/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.817154 pyperformance-1.0.7/benchmarks/bm_telco/
+-rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-04-23 06:20:54.000000 pyperformance-1.0.7/benchmarks/bm_telco/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.817154 pyperformance-1.0.7/benchmarks/bm_tomli_loads/
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-23 06:20:55.000000 pyperformance-1.0.7/benchmarks/bm_tomli_loads/generate_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-04-23 06:20:55.000000 pyperformance-1.0.7/benchmarks/bm_tomli_loads/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.817154 pyperformance-1.0.7/benchmarks/bm_tornado_http/
+-rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-04-23 06:20:55.000000 pyperformance-1.0.7/benchmarks/bm_tornado_http/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.817154 pyperformance-1.0.7/benchmarks/bm_unpack_sequence/
+-rw-r--r--   0 runner    (1001) docker     (123)    20968 2023-04-23 06:20:55.000000 pyperformance-1.0.7/benchmarks/bm_unpack_sequence/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.817154 pyperformance-1.0.7/benchmarks/bm_xml_etree/
+-rw-r--r--   0 runner    (1001) docker     (123)     9514 2023-04-23 06:20:55.000000 pyperformance-1.0.7/benchmarks/bm_xml_etree/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.817154 pyperformance-1.0.7/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-23 06:20:54.000000 pyperformance-1.0.7/doc/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    20221 2023-04-23 06:20:54.000000 pyperformance-1.0.7/doc/benchmarks.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    19599 2023-04-23 06:20:54.000000 pyperformance-1.0.7/doc/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4923 2023-04-23 06:20:54.000000 pyperformance-1.0.7/doc/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25473 2023-04-23 06:20:54.000000 pyperformance-1.0.7/doc/cpython_results_2017.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10342 2023-04-23 06:20:54.000000 pyperformance-1.0.7/doc/custom_benchmarks.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.817154 pyperformance-1.0.7/doc/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     9302 2023-04-23 06:20:54.000000 pyperformance-1.0.7/doc/images/bm_chaos.png
+-rw-r--r--   0 runner    (1001) docker     (123)    55274 2023-04-23 06:20:54.000000 pyperformance-1.0.7/doc/images/bm_raytrace.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    48901 2023-04-23 06:20:54.000000 pyperformance-1.0.7/doc/images/html5lib.png
+-rw-r--r--   0 runner    (1001) docker     (123)    42433 2023-04-23 06:20:54.000000 pyperformance-1.0.7/doc/images/sympy_sum.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-04-23 06:20:54.000000 pyperformance-1.0.7/doc/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-04-23 06:20:54.000000 pyperformance-1.0.7/doc/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)    19415 2023-04-23 06:20:54.000000 pyperformance-1.0.7/doc/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.821153 pyperformance-1.0.7/pyperformance/
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7829 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7227 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/_benchmark_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/_benchmark_selections.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14475 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/_manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/_pip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9660 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/_pyproject_toml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/_python.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/_pythoninfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7553 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/_venv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12141 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7733 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13008 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33030 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/compile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.821153 pyperformance-1.0.7/pyperformance/data-files/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.821153 pyperformance-1.0.7/pyperformance/data-files/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/MANIFEST
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.821153 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_2to3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.801153 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_2to3/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.821153 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_2to3/data/2to3/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_2to3/data/2to3/README.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_2to3/data/2to3/__init__.py.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3418 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_2to3/data/2to3/context_processors.py.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_2to3/data/2to3/exceptions.py.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    16817 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_2to3/data/2to3/mail.py.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4021 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_2to3/data/2to3/paginator.py.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_2to3/data/2to3/signals.py.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_2to3/data/2to3/template_loader.py.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    15786 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_2to3/data/2to3/urlresolvers.py.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_2to3/data/2to3/xheaders.py.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_2to3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_2to3/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.825153 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_async_generators/
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_async_generators/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_async_generators/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.825153 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_async_tree/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_async_tree/bm_async_tree_cpu_io_mixed.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_async_tree/bm_async_tree_io.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_async_tree/bm_async_tree_memoization.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_async_tree/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_async_tree/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.825153 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_asyncio_tcp/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_asyncio_tcp/bm_asyncio_tcp_ssl.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_asyncio_tcp/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_asyncio_tcp/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.825153 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_chameleon/
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_chameleon/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_chameleon/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_chameleon/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.825153 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_chaos/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_chaos/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    10709 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_chaos/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.825153 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_comprehensions/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_comprehensions/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_comprehensions/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.825153 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_concurrent_imap/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_concurrent_imap/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_concurrent_imap/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.825153 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_coroutines/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_coroutines/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_coroutines/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.825153 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_coverage/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_coverage/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_coverage/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_coverage/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.825153 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_crypto_pyaes/
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_crypto_pyaes/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_crypto_pyaes/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_crypto_pyaes/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.825153 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dask/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dask/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dask/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dask/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.825153 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_deepcopy/
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_deepcopy/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_deepcopy/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.829154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_deltablue/
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_deltablue/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    17136 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_deltablue/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.829154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_django_template/
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_django_template/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_django_template/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_django_template/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.829154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.801153 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.829154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.829154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/api/
+-rw-r--r--   0 runner    (1001) docker     (123)    10569 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/api/publisher.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6216 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/api/runtime-settings.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6334 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/api/transforms.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.829154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/
+-rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/distributing.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    16986 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/enthought-plan.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4531 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/enthought-rfp.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9172 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/hacking.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    25780 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/policies.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4380 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/pysource.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/release.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9439 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/repository.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.829154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/rst/
+-rw-r--r--   0 runner    (1001) docker     (123)   113263 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/rst/alternatives.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35463 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/rst/problems.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10664 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/runtime-settings-processing.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/semantics.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9504 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/testing.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    98603 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/todo.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/website.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.833154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/howto/
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/howto/cmdline-tool.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3417 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/howto/html-stylesheets.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6869 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/howto/i18n.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    16349 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/howto/rst-directives.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8907 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/howto/rst-roles.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6972 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/howto/security.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8264 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/index.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.833154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/peps/
+-rw-r--r--   0 runner    (1001) docker     (123)    10437 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/peps/pep-0256.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11684 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/peps/pep-0257.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    36399 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/peps/pep-0258.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    32543 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/peps/pep-0287.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.833154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/ref/
+-rw-r--r--   0 runner    (1001) docker     (123)   132076 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/ref/doctree.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.833154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/ref/rst/
+-rw-r--r--   0 runner    (1001) docker     (123)     7613 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/ref/rst/definitions.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    66717 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/ref/rst/directives.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    13914 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/ref/rst/introduction.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    51188 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/ref/rst/mathematics.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   117454 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/ref/rst/restructuredtext.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10658 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/ref/rst/roles.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.833154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/
+-rw-r--r--   0 runner    (1001) docker     (123)    64502 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/config.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    31991 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/emacs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8318 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/html.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.837154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/images/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/images/big-black.png
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/images/big-white.png
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/images/default.png
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/images/happy_monkey.png
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/images/medium-black.png
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/images/medium-white.png
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/images/rsp-all.png
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/images/rsp-breaks.png
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/images/rsp-covers.png
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/images/rsp-cuts.png
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/images/rsp-empty.png
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/images/rsp-objects.png
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/images/rsp.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/images/s5-files.png
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/images/s5-files.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/images/small-black.png
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/images/small-white.png
+-rw-r--r--   0 runner    (1001) docker     (123)    62611 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/latex.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    15571 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5543 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/mailing-lists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5202 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/manpage.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    38313 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/odt.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.837154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/rst/
+-rw-r--r--   0 runner    (1001) docker     (123)     7097 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/rst/cheatsheet.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    15080 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/rst/demo.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.837154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/rst/images/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/rst/images/biohazard-bitmap-scaling.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/rst/images/biohazard-bitmap.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/rst/images/biohazard-scaling.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/rst/images/biohazard.png
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/rst/images/biohazard.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/rst/images/biohazard.swf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/rst/images/pens.mp4
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/rst/images/title-scaling.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/rst/images/title.png
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/rst/images/title.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    11268 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/rst/quickstart.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    12042 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/smartquotes.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    17347 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/tools.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.837154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dulwich_log/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.801153 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dulwich_log/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.841154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/COMMIT_EDITMSG
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/FETCH_HEAD
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/HEAD
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/ORIG_HEAD
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/config
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/description
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.841154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/hooks/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      452 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/hooks/applypatch-msg.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)      896 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/hooks/commit-msg.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)      189 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/hooks/post-update.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)      398 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/hooks/pre-applypatch.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1642 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/hooks/pre-commit.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1348 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/hooks/pre-push.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4951 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/hooks/pre-rebase.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1239 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/hooks/prepare-commit-msg.sample
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3611 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/hooks/update.sample
+-rw-r--r--   0 runner    (1001) docker     (123)     8508 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/index
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.841154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/info/
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/info/exclude
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/info/refs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.841154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/logs/
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/logs/HEAD
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.805153 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/logs/refs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.841154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/logs/refs/heads/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/logs/refs/heads/master
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.805153 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/logs/refs/remotes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.841154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/logs/refs/remotes/origin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/logs/refs/remotes/origin/HEAD
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/logs/refs/remotes/origin/bind_modules
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/logs/refs/remotes/origin/master
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/logs/refs/remotes/origin/zero_timeout
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.805153 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/objects/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.841154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/objects/info/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/objects/info/packs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.841154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/objects/pack/
+-rw-r--r--   0 runner    (1001) docker     (123)   247416 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/objects/pack/pack-7e1b1ace85030071ca314cd565ae038bacc302a4.idx
+-rw-r--r--   0 runner    (1001) docker     (123)  1774473 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/objects/pack/pack-7e1b1ace85030071ca314cd565ae038bacc302a4.pack
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/packed-refs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.805153 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/refs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.805153 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/refs/remotes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.845154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/refs/remotes/origin/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/refs/remotes/origin/HEAD
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dulwich_log/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dulwich_log/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dulwich_log/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.845154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_fannkuch/
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_fannkuch/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_fannkuch/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.845154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_float/
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_float/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_float/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.845154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_gc_collect/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_gc_collect/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_gc_collect/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.845154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_gc_traversal/
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_gc_traversal/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_gc_traversal/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.845154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_generators/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_generators/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_generators/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.845154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_genshi/
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_genshi/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_genshi/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_genshi/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.845154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_go/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_go/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    13911 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_go/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.845154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_hexiom/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_hexiom/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    17354 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_hexiom/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.845154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_hg_startup/
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_hg_startup/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_hg_startup/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_hg_startup/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.849154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_html5lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.849154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_html5lib/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   133837 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_html5lib/data/w3_tr_html5.html
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_html5lib/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_html5lib/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_html5lib/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.849154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_json_dumps/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_json_dumps/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_json_dumps/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.849154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_json_loads/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_json_loads/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_json_loads/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.849154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_logging/
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_logging/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_logging/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.849154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_mako/
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_mako/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_mako/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3742 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_mako/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.849154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_mdp/
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_mdp/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     8797 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_mdp/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.849154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_meteor_contest/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_meteor_contest/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     8011 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_meteor_contest/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.849154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_nbody/
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_nbody/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     5039 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_nbody/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.849154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_nqueens/
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_nqueens/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_nqueens/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.849154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_pathlib/
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_pathlib/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_pathlib/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.853154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_pickle/
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_pickle/bm_pickle_dict.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_pickle/bm_pickle_list.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_pickle/bm_pickle_pure_python.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_pickle/bm_unpickle.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_pickle/bm_unpickle_list.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_pickle/bm_unpickle_pure_python.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_pickle/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     8216 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_pickle/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.853154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_pidigits/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_pidigits/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_pidigits/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.853154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_pprint/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_pprint/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_pprint/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.853154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_pyflate/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.853154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_pyflate/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    67562 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_pyflate/data/interpreter.tar.bz2
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_pyflate/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (123)    20078 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_pyflate/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.853154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_python_startup/
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_python_startup/bm_python_startup_no_site.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_python_startup/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_python_startup/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.853154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_raytrace/
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_raytrace/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    12042 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_raytrace/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.853154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_regex_compile/
+-rw-r--r--   0 runner    (1001) docker     (123)     5325 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_regex_compile/bm_regex_effbot.py
+-rw-r--r--   0 runner    (1001) docker     (123)   125978 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_regex_compile/bm_regex_v8.py
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_regex_compile/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_regex_compile/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.853154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_regex_dna/
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_regex_dna/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     6731 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_regex_dna/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.853154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_regex_effbot/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_regex_effbot/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     5325 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_regex_effbot/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.853154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_regex_v8/
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_regex_v8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)   125978 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_regex_v8/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.853154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_richards/
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_richards/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     9539 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_richards/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.853154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_scimark/
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_scimark/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    10173 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_scimark/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.853154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_spectral_norm/
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_spectral_norm/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_spectral_norm/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.857154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_sqlalchemy_declarative/
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_sqlalchemy_declarative/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_sqlalchemy_declarative/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_sqlalchemy_declarative/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.857154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_sqlalchemy_imperative/
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_sqlalchemy_imperative/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_sqlalchemy_imperative/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_sqlalchemy_imperative/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.857154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_sqlglot/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_sqlglot/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_sqlglot/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4892 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_sqlglot/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.857154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_sqlite_synth/
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_sqlite_synth/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_sqlite_synth/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.857154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_sympy/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_sympy/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_sympy/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_sympy/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.857154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_telco/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.857154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_telco/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   160000 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_telco/data/telco-bench.b
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_telco/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-04-23 06:20:54.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_telco/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.857154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_tomli_loads/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.857154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_tomli_loads/data/
+-rw-r--r--   0 runner    (1001) docker     (123) 16824157 2023-04-23 06:20:55.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_tomli_loads/data/tomli-bench-data.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-04-23 06:20:55.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_tomli_loads/generate_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-23 06:20:55.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_tomli_loads/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-23 06:20:55.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_tomli_loads/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-04-23 06:20:55.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_tomli_loads/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.873154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_tornado_http/
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-23 06:20:55.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_tornado_http/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-23 06:20:55.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_tornado_http/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-04-23 06:20:55.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_tornado_http/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.877154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_unpack_sequence/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-23 06:20:55.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_unpack_sequence/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    20968 2023-04-23 06:20:55.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_unpack_sequence/run_benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.877154 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_xml_etree/
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-23 06:20:55.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_xml_etree/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     9514 2023-04-23 06:20:55.000000 pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_xml_etree/run_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-04-23 06:20:55.000000 pyperformance-1.0.7/pyperformance/data-files/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5965 2023-04-23 06:20:55.000000 pyperformance-1.0.7/pyperformance/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7717 2023-04-23 06:20:55.000000 pyperformance-1.0.7/pyperformance/venv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 06:21:09.821153 pyperformance-1.0.7/pyperformance.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-04-23 06:21:09.000000 pyperformance-1.0.7/pyperformance.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    23354 2023-04-23 06:21:09.000000 pyperformance-1.0.7/pyperformance.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 06:21:09.000000 pyperformance-1.0.7/pyperformance.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-23 06:21:09.000000 pyperformance-1.0.7/pyperformance.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-23 06:21:09.000000 pyperformance-1.0.7/pyperformance.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-23 06:21:09.000000 pyperformance-1.0.7/pyperformance.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-04-23 06:20:55.000000 pyperformance-1.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-04-23 06:20:55.000000 pyperformance-1.0.7/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-04-23 06:20:55.000000 pyperformance-1.0.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 06:21:09.877154 pyperformance-1.0.7/setup.cfg
```

### Comparing `pyperformance-1.0.6/AUTHORS` & `pyperformance-1.0.7/AUTHORS`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/COPYING` & `pyperformance-1.0.7/COPYING`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/MANIFEST.in` & `pyperformance-1.0.7/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/PKG-INFO` & `pyperformance-1.0.7/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 Metadata-Version: 2.1
 Name: pyperformance
-Version: 1.0.6
+Version: 1.0.7
 Summary: Python benchmark suite
-Home-page: https://github.com/python/benchmarks
-Author: Collin Winter and Jeffrey Yasskin
-License: MIT license
+Author: Collin Winter, Jeffrey Yasskin
+License: MIT
+Project-URL: Homepage, https://github.com/python/pyperformance
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python
+Requires-Python: >=3.7
+Description-Content-Type: text/x-rst
+Provides-Extra: dev
 License-File: COPYING
 License-File: AUTHORS
 
 ##########################
 The Python Benchmark Suite
 ##########################
```

### Comparing `pyperformance-1.0.6/README.rst` & `pyperformance-1.0.7/README.rst`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/TODO.rst` & `pyperformance-1.0.7/TODO.rst`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/doc/Makefile` & `pyperformance-1.0.7/doc/Makefile`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/doc/benchmarks.rst` & `pyperformance-1.0.7/doc/benchmarks.rst`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/doc/changelog.rst` & `pyperformance-1.0.7/doc/changelog.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,24 @@
 Changelog
 =========
 
+Version 1.0.7 (2023-04-22)
+-------------
+
+* Upgrade pyperf from 2.5.0 to 2.6.0
+* Clean unused imports and other small code details
+* Migrage to the pyproject.toml based project
+* Fix the django_template benchmark due to lack of distutils
+* Add benchmark for toml
+* Add benchmark for comprehensions
+* Add benchmark for asyncio_tcp_ssl
+* Add benchmark for asyncio_tcp
+* Add benchmark for Dask scheduler
+* Add the gc benchmarks to the MANIFEST file
+
 Version 1.0.6 (2022-11-20)
 -------------
 
 * Upgrade pyperf from 2.4.1 to 2.5.0
 * Add a benchmark to measure gc traversal
 * Add jobs field in compile section to specify make -j param
 * Add benchmark for Docutils
```

### Comparing `pyperformance-1.0.6/doc/conf.py` & `pyperformance-1.0.7/doc/conf.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/doc/cpython_results_2017.rst` & `pyperformance-1.0.7/doc/cpython_results_2017.rst`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/doc/custom_benchmarks.rst` & `pyperformance-1.0.7/doc/custom_benchmarks.rst`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/doc/images/bm_chaos.png` & `pyperformance-1.0.7/doc/images/bm_chaos.png`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/doc/images/bm_raytrace.jpg` & `pyperformance-1.0.7/doc/images/bm_raytrace.jpg`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/doc/images/html5lib.png` & `pyperformance-1.0.7/doc/images/html5lib.png`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/doc/images/sympy_sum.png` & `pyperformance-1.0.7/doc/images/sympy_sum.png`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/doc/index.rst` & `pyperformance-1.0.7/doc/index.rst`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/doc/make.bat` & `pyperformance-1.0.7/doc/make.bat`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/doc/usage.rst` & `pyperformance-1.0.7/doc/usage.rst`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/__init__.py` & `pyperformance-1.0.7/pyperformance/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os.path
 import sys
 
 
-VERSION = (1, 0, 6)
+VERSION = (1, 0, 7)
 __version__ = '.'.join(map(str, VERSION))
 
 
 PKG_ROOT = os.path.dirname(__file__)
 DATA_DIR = os.path.join(PKG_ROOT, 'data-files')
```

### Comparing `pyperformance-1.0.6/pyperformance/_benchmark.py` & `pyperformance-1.0.7/pyperformance/_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/_benchmark_metadata.py` & `pyperformance-1.0.7/pyperformance/_benchmark_metadata.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/_benchmark_selections.py` & `pyperformance-1.0.7/pyperformance/_benchmark_selections.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 __all__ = [
     'parse_selection',
     'iter_selections',
 ]
 
 
-from . import _utils, _manifest, _benchmark
+from . import _utils, _benchmark
 
 
 def parse_selection(selection, *, op=None):
     # "selection" is one of the following:
     # * a benchmark string
     # * a benchmark name
     # * a benchmark pattern
```

### Comparing `pyperformance-1.0.6/pyperformance/_manifest.py` & `pyperformance-1.0.7/pyperformance/_manifest.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 __all__ = [
     'BenchmarksManifest',
     'load_manifest',
     'parse_manifest',
 ]
 
 
-from collections import namedtuple
 import os.path
 
 
 from . import __version__, DATA_DIR
 from . import _benchmark, _utils
```

### Comparing `pyperformance-1.0.6/pyperformance/_pip.py` & `pyperformance-1.0.7/pyperformance/_pip.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 import os
 import os.path
-import shlex
-import subprocess
 import sys
 
 from . import _utils, _pythoninfo
 
 
 GET_PIP_URL = 'https://bootstrap.pypa.io/get-pip.py'
 # pip 6 is the first version supporting environment markers
```

### Comparing `pyperformance-1.0.6/pyperformance/_pyproject_toml.py` & `pyperformance-1.0.7/pyperformance/_pyproject_toml.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/_python.py` & `pyperformance-1.0.7/pyperformance/_python.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/_pythoninfo.py` & `pyperformance-1.0.7/pyperformance/_pythoninfo.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/_utils.py` & `pyperformance-1.0.7/pyperformance/_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,16 +21,14 @@
 
 import contextlib
 import errno
 import os
 import os.path
 import shlex
 import shutil
-import subprocess
-import sys
 import tempfile
 import urllib.request
 
 
 @contextlib.contextmanager
 def temporary_file():
     tmp_filename = tempfile.mktemp()
@@ -80,15 +78,14 @@
     shutil.rmtree(path)
     return True
 
 
 #######################################
 # platform utils
 
-import logging
 import subprocess
 import sys
 
 
 MS_WINDOWS = (sys.platform == 'win32')
 
 
@@ -212,15 +209,16 @@
     return tag
 
 
 def parse_selections(selections, parse_entry=None):
     if isinstance(selections, str):
         selections = selections.split(',')
     if parse_entry is None:
-        parse_entry = (lambda o, e: (o, e, None, e))
+        def parse_entry(o, e):
+            return (o, e, None, e)
 
     for entry in selections:
         entry = entry.strip()
         if not entry:
             continue
 
         op = '+'
```

### Comparing `pyperformance-1.0.6/pyperformance/_venv.py` & `pyperformance-1.0.7/pyperformance/_venv.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/cli.py` & `pyperformance-1.0.7/pyperformance/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -222,15 +222,16 @@
 
 
 def _select_benchmarks(raw, manifest):
     from pyperformance import _benchmark_selections
 
     # Get the raw list of benchmarks.
     entries = raw.lower()
-    parse_entry = (lambda o, s: _benchmark_selections.parse_selection(s, op=o))
+    def parse_entry(o, s):
+        return _benchmark_selections.parse_selection(s, op=o)
     parsed = _utils.parse_selections(entries, parse_entry)
     parsed_infos = list(parsed)
 
     # Disallow negative groups.
     for op, _, kind, parsed in parsed_infos:
         if callable(parsed):
             continue
```

### Comparing `pyperformance-1.0.6/pyperformance/commands.py` & `pyperformance-1.0.7/pyperformance/commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
                 print("%s (%s):" % (tag, len(specs)))
                 for spec in sorted(specs):
                     print("- %s" % spec.name)
                 print()
 
 
 def cmd_venv_create(options, root, python, benchmarks):
-    from . import _pythoninfo, _venv
+    from . import _venv
     from .venv import Requirements, VenvForBenchmarks
 
     if _venv.venv_exists(root):
         sys.exit(f'ERROR: the virtual environment already exists at {root}')
 
     requirements = Requirements.from_benchmarks(benchmarks)
     venv = VenvForBenchmarks.ensure(
@@ -69,15 +69,15 @@
         venv.ensure_reqs(requirements)
     except _venv.RequirementsInstallationFailedError:
         sys.exit(1)
     print("The virtual environment %s has been created" % root)
 
 
 def cmd_venv_recreate(options, root, python, benchmarks):
-    from . import _pythoninfo, _venv, _utils
+    from . import _venv, _utils
     from .venv import Requirements, VenvForBenchmarks
 
     requirements = Requirements.from_benchmarks(benchmarks)
     if _venv.venv_exists(root):
         venv_python = _venv.resolve_venv_python(root)
         if venv_python == sys.executable:
             print("The virtual environment %s already exists" % root)
```

### Comparing `pyperformance-1.0.6/pyperformance/compare.py` & `pyperformance-1.0.7/pyperformance/compare.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import csv
 import os.path
 import math
-import sys
 
 import pyperf
 import statistics
 
 
 NO_VERSION = "<not set>"
```

### Comparing `pyperformance-1.0.6/pyperformance/compile.py` & `pyperformance-1.0.7/pyperformance/compile.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/MANIFEST` & `pyperformance-1.0.7/pyperformance/data-files/benchmarks/MANIFEST`

 * *Files 27% similar despite different names*

```diff
@@ -3,21 +3,27 @@
 name	metafile
 2to3	<local>
 async_generators	<local>
 async_tree	<local>
 async_tree_cpu_io_mixed	<local:async_tree>
 async_tree_io	<local:async_tree>
 async_tree_memoization	<local:async_tree>
+asyncio_tcp	<local>
+asyncio_tcp_ssl	<local:asyncio_tcp>
 concurrent_imap	<local>
 coroutines	<local>
 coverage	<local>
+gc_traversal	<local>
+gc_collect	<local>
 generators	<local>
 chameleon	<local>
 chaos	<local>
+comprehensions	<local>
 crypto_pyaes	<local>
+dask	<local>
 deepcopy	<local>
 deltablue	<local>
 django_template	<local>
 dulwich_log	<local>
 docutils	<local>
 fannkuch	<local>
 float	<local>
@@ -56,14 +62,15 @@
 spectral_norm	<local>
 sqlalchemy_declarative	<local>
 sqlalchemy_imperative	<local>
 sqlglot	<local>
 sqlite_synth	<local>
 sympy	<local>
 telco	<local>
+tomli_loads	<local>
 tornado_http	<local>
 unpack_sequence	<local>
 unpickle	<local:pickle>
 unpickle_list	<local:pickle>
 unpickle_pure_python	<local:pickle>
 xml_etree	<local>
```

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_2to3/data/2to3/context_processors.py.txt` & `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_2to3/data/2to3/context_processors.py.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_2to3/data/2to3/exceptions.py.txt` & `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_2to3/data/2to3/exceptions.py.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_2to3/data/2to3/mail.py.txt` & `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_2to3/data/2to3/mail.py.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_2to3/data/2to3/paginator.py.txt` & `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_2to3/data/2to3/paginator.py.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_2to3/data/2to3/urlresolvers.py.txt` & `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_2to3/data/2to3/urlresolvers.py.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_2to3/data/2to3/xheaders.py.txt` & `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_2to3/data/2to3/xheaders.py.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_async_generators/run_benchmark.py` & `pyperformance-1.0.7/benchmarks/bm_async_generators/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_async_tree/run_benchmark.py` & `pyperformance-1.0.7/benchmarks/bm_async_tree/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_chameleon/run_benchmark.py` & `pyperformance-1.0.7/benchmarks/bm_chameleon/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_chaos/run_benchmark.py` & `pyperformance-1.0.7/benchmarks/bm_chaos/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_concurrent_imap/run_benchmark.py` & `pyperformance-1.0.7/benchmarks/bm_concurrent_imap/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_coroutines/run_benchmark.py` & `pyperformance-1.0.7/benchmarks/bm_coroutines/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_coverage/run_benchmark.py` & `pyperformance-1.0.7/benchmarks/bm_coverage/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_crypto_pyaes/run_benchmark.py` & `pyperformance-1.0.7/benchmarks/bm_crypto_pyaes/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_deepcopy/run_benchmark.py` & `pyperformance-1.0.7/benchmarks/bm_deepcopy/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_deltablue/run_benchmark.py` & `pyperformance-1.0.7/benchmarks/bm_deltablue/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_django_template/run_benchmark.py` & `pyperformance-1.0.7/benchmarks/bm_django_template/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/api/publisher.txt` & `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/api/publisher.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/api/runtime-settings.txt` & `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/api/runtime-settings.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/api/transforms.txt` & `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/api/transforms.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/distributing.txt` & `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/distributing.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/enthought-plan.txt` & `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/enthought-plan.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/enthought-rfp.txt` & `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/enthought-rfp.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/hacking.txt` & `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/hacking.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/policies.txt` & `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/policies.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/pysource.txt` & `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/pysource.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/release.txt` & `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/release.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/repository.txt` & `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/repository.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/rst/alternatives.txt` & `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/rst/alternatives.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/rst/problems.txt` & `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/rst/problems.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/runtime-settings-processing.txt` & `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/runtime-settings-processing.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/semantics.txt` & `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/semantics.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/testing.txt` & `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/testing.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/todo.txt` & `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/todo.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/website.txt` & `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/dev/website.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/howto/cmdline-tool.txt` & `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/howto/cmdline-tool.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/howto/html-stylesheets.txt` & `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/howto/html-stylesheets.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/howto/i18n.txt` & `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/howto/i18n.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/howto/rst-directives.txt` & `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/howto/rst-directives.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/howto/rst-roles.txt` & `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/howto/rst-roles.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/howto/security.txt` & `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/howto/security.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/index.txt` & `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/index.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/peps/pep-0256.txt` & `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/peps/pep-0256.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/peps/pep-0257.txt` & `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/peps/pep-0257.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/peps/pep-0258.txt` & `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/peps/pep-0258.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/peps/pep-0287.txt` & `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/peps/pep-0287.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/ref/doctree.txt` & `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/ref/doctree.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/ref/rst/definitions.txt` & `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/ref/rst/definitions.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/ref/rst/directives.txt` & `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/ref/rst/directives.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/ref/rst/introduction.txt` & `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/ref/rst/introduction.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/ref/rst/mathematics.txt` & `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/ref/rst/mathematics.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/ref/rst/restructuredtext.txt` & `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/ref/rst/restructuredtext.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/ref/rst/roles.txt` & `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/ref/rst/roles.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/config.txt` & `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/config.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/emacs.txt` & `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/emacs.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/html.txt` & `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/html.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/latex.txt` & `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/latex.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/links.txt` & `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/links.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/mailing-lists.txt` & `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/mailing-lists.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/manpage.txt` & `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/manpage.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/odt.txt` & `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/odt.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/rst/cheatsheet.txt` & `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/rst/cheatsheet.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/rst/demo.txt` & `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/rst/demo.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/rst/quickstart.txt` & `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/rst/quickstart.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/smartquotes.txt` & `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/smartquotes.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/tools.txt` & `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_docutils/data/docs/user/tools.txt`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_docutils/run_benchmark.py` & `pyperformance-1.0.7/benchmarks/bm_docutils/run_benchmark.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """
 Convert Docutils' documentation from reStructuredText to <format>.
 """
 
 import contextlib
 from pathlib import Path
-import time
 
 import docutils
 from docutils import core
 import pyperf
 
 try:
     from docutils.utils.math.math2html import Trace
```

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/COMMIT_EDITMSG` & `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/COMMIT_EDITMSG`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/hooks/commit-msg.sample` & `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/hooks/commit-msg.sample`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/hooks/pre-commit.sample` & `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/hooks/pre-commit.sample`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/hooks/pre-push.sample` & `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/hooks/pre-push.sample`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/hooks/pre-rebase.sample` & `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/hooks/pre-rebase.sample`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/hooks/prepare-commit-msg.sample` & `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/hooks/prepare-commit-msg.sample`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/hooks/update.sample` & `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/hooks/update.sample`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/index` & `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/index`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/info/refs` & `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/info/refs`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/objects/pack/pack-7e1b1ace85030071ca314cd565ae038bacc302a4.idx` & `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/objects/pack/pack-7e1b1ace85030071ca314cd565ae038bacc302a4.idx`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/objects/pack/pack-7e1b1ace85030071ca314cd565ae038bacc302a4.pack` & `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/objects/pack/pack-7e1b1ace85030071ca314cd565ae038bacc302a4.pack`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/packed-refs` & `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_dulwich_log/data/asyncio.git/packed-refs`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_dulwich_log/run_benchmark.py` & `pyperformance-1.0.7/benchmarks/bm_dulwich_log/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_fannkuch/run_benchmark.py` & `pyperformance-1.0.7/benchmarks/bm_fannkuch/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_float/run_benchmark.py` & `pyperformance-1.0.7/benchmarks/bm_float/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_gc_collect/run_benchmark.py` & `pyperformance-1.0.7/benchmarks/bm_gc_collect/run_benchmark.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 
         # Main loop to measure
         del all_cycles
         t0 = pyperf.perf_counter()
         collected = gc.collect()
         total_time += pyperf.perf_counter() - t0
 
-        assert collected >= cycles * (links + 1)
+        assert collected is None or collected >= cycles * (links + 1)
 
     return total_time
 
 
 if __name__ == "__main__":
     runner = pyperf.Runner()
     runner.metadata["description"] = "GC link benchmark"
```

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_gc_traversal/run_benchmark.py` & `pyperformance-1.0.7/benchmarks/bm_gc_traversal/run_benchmark.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     for _ in range(loops):
         gc.collect()
         # Main loop to measure
         t0 = pyperf.perf_counter()
         collected = gc.collect()
         total_time += pyperf.perf_counter() - t0
 
-        assert collected == 0
+        assert collected is None or collected == 0
 
     return total_time
 
 
 if __name__ == "__main__":
     runner = pyperf.Runner()
     runner.metadata["description"] = "GC traversal benchmark"
```

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_generators/run_benchmark.py` & `pyperformance-1.0.7/benchmarks/bm_generators/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_genshi/run_benchmark.py` & `pyperformance-1.0.7/benchmarks/bm_genshi/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_go/run_benchmark.py` & `pyperformance-1.0.7/benchmarks/bm_go/run_benchmark.py`

 * *Files 2% similar despite different names*

```diff
@@ -448,14 +448,10 @@
 def versus_cpu():
     random.seed(1)
     board = Board()
     return computer_move(board)
 
 
 if __name__ == "__main__":
-    kw = {}
-    if pyperf.python_has_jit():
-        # PyPy needs to compute more warmup values to warmup its JIT
-        kw['warmups'] = 50
-    runner = pyperf.Runner(**kw)
+    runner = pyperf.Runner()
     runner.metadata['description'] = "Test the performance of the Go benchmark"
     runner.bench_func('go', versus_cpu)
```

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_hexiom/run_benchmark.py` & `pyperformance-1.0.7/benchmarks/bm_hexiom/run_benchmark.py`

 * *Files 1% similar despite different names*

```diff
@@ -647,19 +647,15 @@
 
 
 def add_cmdline_args(cmd, args):
     cmd.extend(("--level", str(args.level)))
 
 
 if __name__ == "__main__":
-    kw = {'add_cmdline_args': add_cmdline_args}
-    if pyperf.python_has_jit():
-        # PyPy needs to compute more warmup values to warmup its JIT
-        kw['warmups'] = 15
-    runner = pyperf.Runner(**kw)
+    runner = pyperf.Runner(add_cmdline_args=add_cmdline_args)
     levels = sorted(LEVELS)
     runner.argparser.add_argument("--level", type=int,
                                   choices=levels,
                                   default=DEFAULT_LEVEL,
                                   help="Hexiom board level (default: %s)"
                                        % DEFAULT_LEVEL)
```

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_hg_startup/run_benchmark.py` & `pyperformance-1.0.7/benchmarks/bm_hg_startup/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_html5lib/data/w3_tr_html5.html` & `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_html5lib/data/w3_tr_html5.html`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_html5lib/run_benchmark.py` & `pyperformance-1.0.7/benchmarks/bm_html5lib/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_json_dumps/run_benchmark.py` & `pyperformance-1.0.7/benchmarks/bm_json_dumps/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_json_loads/run_benchmark.py` & `pyperformance-1.0.7/benchmarks/bm_json_loads/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_logging/run_benchmark.py` & `pyperformance-1.0.7/benchmarks/bm_logging/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_mako/run_benchmark.py` & `pyperformance-1.0.7/benchmarks/bm_mako/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_mdp/run_benchmark.py` & `pyperformance-1.0.7/benchmarks/bm_mdp/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_meteor_contest/run_benchmark.py` & `pyperformance-1.0.7/benchmarks/bm_meteor_contest/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_nbody/run_benchmark.py` & `pyperformance-1.0.7/benchmarks/bm_nbody/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_nqueens/run_benchmark.py` & `pyperformance-1.0.7/benchmarks/bm_nqueens/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_pathlib/run_benchmark.py` & `pyperformance-1.0.7/benchmarks/bm_pathlib/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_pickle/run_benchmark.py` & `pyperformance-1.0.7/benchmarks/bm_pickle/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_pidigits/run_benchmark.py` & `pyperformance-1.0.7/benchmarks/bm_pidigits/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_pprint/run_benchmark.py` & `pyperformance-1.0.7/benchmarks/bm_pprint/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_pyflate/data/interpreter.tar.bz2` & `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_pyflate/data/interpreter.tar.bz2`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_pyflate/run_benchmark.py` & `pyperformance-1.0.7/benchmarks/bm_pyflate/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_python_startup/run_benchmark.py` & `pyperformance-1.0.7/benchmarks/bm_python_startup/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_raytrace/run_benchmark.py` & `pyperformance-1.0.7/benchmarks/bm_raytrace/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_regex_compile/bm_regex_effbot.py` & `pyperformance-1.0.7/benchmarks/bm_regex_compile/bm_regex_effbot.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_regex_compile/bm_regex_v8.py` & `pyperformance-1.0.7/benchmarks/bm_regex_compile/bm_regex_v8.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_regex_compile/run_benchmark.py` & `pyperformance-1.0.7/benchmarks/bm_regex_compile/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_regex_dna/run_benchmark.py` & `pyperformance-1.0.7/benchmarks/bm_regex_dna/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_regex_effbot/run_benchmark.py` & `pyperformance-1.0.7/benchmarks/bm_regex_effbot/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_regex_v8/run_benchmark.py` & `pyperformance-1.0.7/benchmarks/bm_regex_v8/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_richards/run_benchmark.py` & `pyperformance-1.0.7/benchmarks/bm_richards/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_scimark/run_benchmark.py` & `pyperformance-1.0.7/benchmarks/bm_scimark/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_spectral_norm/run_benchmark.py` & `pyperformance-1.0.7/benchmarks/bm_spectral_norm/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_sqlalchemy_declarative/run_benchmark.py` & `pyperformance-1.0.7/benchmarks/bm_sqlalchemy_declarative/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_sqlalchemy_imperative/run_benchmark.py` & `pyperformance-1.0.7/benchmarks/bm_sqlalchemy_imperative/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_sqlglot/run_benchmark.py` & `pyperformance-1.0.7/benchmarks/bm_sqlglot/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_sqlite_synth/run_benchmark.py` & `pyperformance-1.0.7/benchmarks/bm_sqlite_synth/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_sympy/run_benchmark.py` & `pyperformance-1.0.7/benchmarks/bm_sympy/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_telco/data/telco-bench.b` & `pyperformance-1.0.7/pyperformance/data-files/benchmarks/bm_telco/data/telco-bench.b`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_telco/run_benchmark.py` & `pyperformance-1.0.7/benchmarks/bm_telco/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_tornado_http/run_benchmark.py` & `pyperformance-1.0.7/benchmarks/bm_tornado_http/run_benchmark.py`

 * *Files 4% similar despite different names*

```diff
@@ -92,15 +92,11 @@
     # https://bugs.python.org/issue37373
     # https://github.com/python/pyperformance/issues/61
     # https://github.com/tornadoweb/tornado/pull/2686
     if sys.platform == 'win32' and sys.version_info[:2] >= (3, 8):
         import asyncio
         asyncio.set_event_loop_policy(asyncio.WindowsSelectorEventLoopPolicy())
 
-    kw = {}
-    if pyperf.python_has_jit():
-        # PyPy needs to compute more warmup values to warmup its JIT
-        kw['warmups'] = 30
-    runner = pyperf.Runner(**kw)
+    runner = pyperf.Runner()
     runner.metadata['description'] = ("Test the performance of HTTP requests "
                                       "with Tornado.")
     runner.bench_time_func('tornado_http', bench_tornado)
```

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_unpack_sequence/run_benchmark.py` & `pyperformance-1.0.7/benchmarks/bm_unpack_sequence/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/data-files/benchmarks/bm_xml_etree/run_benchmark.py` & `pyperformance-1.0.7/benchmarks/bm_xml_etree/run_benchmark.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/run.py` & `pyperformance-1.0.7/pyperformance/run.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance/venv.py` & `pyperformance-1.0.7/pyperformance/venv.py`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/pyperformance.egg-info/PKG-INFO` & `pyperformance-1.0.7/pyperformance.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 Metadata-Version: 2.1
 Name: pyperformance
-Version: 1.0.6
+Version: 1.0.7
 Summary: Python benchmark suite
-Home-page: https://github.com/python/benchmarks
-Author: Collin Winter and Jeffrey Yasskin
-License: MIT license
+Author: Collin Winter, Jeffrey Yasskin
+License: MIT
+Project-URL: Homepage, https://github.com/python/pyperformance
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python
+Requires-Python: >=3.7
+Description-Content-Type: text/x-rst
+Provides-Extra: dev
 License-File: COPYING
 License-File: AUTHORS
 
 ##########################
 The Python Benchmark Suite
 ##########################
```

### Comparing `pyperformance-1.0.6/pyperformance.egg-info/SOURCES.txt` & `pyperformance-1.0.7/pyperformance.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,77 @@
 AUTHORS
 COPYING
 MANIFEST.in
 README.rst
 TODO.rst
+pyproject.toml
 requirements.in
 requirements.txt
-setup.py
+benchmarks/bm_2to3/run_benchmark.py
+benchmarks/bm_async_generators/run_benchmark.py
+benchmarks/bm_async_tree/run_benchmark.py
+benchmarks/bm_asyncio_tcp/run_benchmark.py
+benchmarks/bm_chameleon/run_benchmark.py
+benchmarks/bm_chaos/run_benchmark.py
+benchmarks/bm_comprehensions/run_benchmark.py
+benchmarks/bm_concurrent_imap/run_benchmark.py
+benchmarks/bm_coroutines/run_benchmark.py
+benchmarks/bm_coverage/run_benchmark.py
+benchmarks/bm_crypto_pyaes/run_benchmark.py
+benchmarks/bm_dask/run_benchmark.py
+benchmarks/bm_deepcopy/run_benchmark.py
+benchmarks/bm_deltablue/run_benchmark.py
+benchmarks/bm_django_template/run_benchmark.py
+benchmarks/bm_docutils/run_benchmark.py
+benchmarks/bm_dulwich_log/run_benchmark.py
+benchmarks/bm_fannkuch/run_benchmark.py
+benchmarks/bm_float/run_benchmark.py
+benchmarks/bm_gc_collect/run_benchmark.py
+benchmarks/bm_gc_traversal/run_benchmark.py
+benchmarks/bm_generators/run_benchmark.py
+benchmarks/bm_genshi/run_benchmark.py
+benchmarks/bm_go/run_benchmark.py
+benchmarks/bm_hexiom/run_benchmark.py
+benchmarks/bm_hg_startup/run_benchmark.py
+benchmarks/bm_html5lib/run_benchmark.py
+benchmarks/bm_json_dumps/run_benchmark.py
+benchmarks/bm_json_loads/run_benchmark.py
+benchmarks/bm_logging/run_benchmark.py
+benchmarks/bm_mako/run_benchmark.py
+benchmarks/bm_mdp/run_benchmark.py
+benchmarks/bm_meteor_contest/run_benchmark.py
+benchmarks/bm_nbody/run_benchmark.py
+benchmarks/bm_nqueens/run_benchmark.py
+benchmarks/bm_pathlib/run_benchmark.py
+benchmarks/bm_pickle/run_benchmark.py
+benchmarks/bm_pidigits/run_benchmark.py
+benchmarks/bm_pprint/run_benchmark.py
+benchmarks/bm_pyflate/run_benchmark.py
+benchmarks/bm_python_startup/run_benchmark.py
+benchmarks/bm_raytrace/run_benchmark.py
+benchmarks/bm_regex_compile/bm_regex_effbot.py
+benchmarks/bm_regex_compile/bm_regex_v8.py
+benchmarks/bm_regex_compile/run_benchmark.py
+benchmarks/bm_regex_dna/run_benchmark.py
+benchmarks/bm_regex_effbot/run_benchmark.py
+benchmarks/bm_regex_v8/run_benchmark.py
+benchmarks/bm_richards/run_benchmark.py
+benchmarks/bm_scimark/run_benchmark.py
+benchmarks/bm_spectral_norm/run_benchmark.py
+benchmarks/bm_sqlalchemy_declarative/run_benchmark.py
+benchmarks/bm_sqlalchemy_imperative/run_benchmark.py
+benchmarks/bm_sqlglot/run_benchmark.py
+benchmarks/bm_sqlite_synth/run_benchmark.py
+benchmarks/bm_sympy/run_benchmark.py
+benchmarks/bm_telco/run_benchmark.py
+benchmarks/bm_tomli_loads/generate_data.py
+benchmarks/bm_tomli_loads/run_benchmark.py
+benchmarks/bm_tornado_http/run_benchmark.py
+benchmarks/bm_unpack_sequence/run_benchmark.py
+benchmarks/bm_xml_etree/run_benchmark.py
 doc/Makefile
 doc/benchmarks.rst
 doc/changelog.rst
 doc/conf.py
 doc/cpython_results_2017.rst
 doc/custom_benchmarks.rst
 doc/index.rst
@@ -60,29 +122,37 @@
 pyperformance/data-files/benchmarks/bm_async_generators/pyproject.toml
 pyperformance/data-files/benchmarks/bm_async_generators/run_benchmark.py
 pyperformance/data-files/benchmarks/bm_async_tree/bm_async_tree_cpu_io_mixed.toml
 pyperformance/data-files/benchmarks/bm_async_tree/bm_async_tree_io.toml
 pyperformance/data-files/benchmarks/bm_async_tree/bm_async_tree_memoization.toml
 pyperformance/data-files/benchmarks/bm_async_tree/pyproject.toml
 pyperformance/data-files/benchmarks/bm_async_tree/run_benchmark.py
+pyperformance/data-files/benchmarks/bm_asyncio_tcp/bm_asyncio_tcp_ssl.toml
+pyperformance/data-files/benchmarks/bm_asyncio_tcp/pyproject.toml
+pyperformance/data-files/benchmarks/bm_asyncio_tcp/run_benchmark.py
 pyperformance/data-files/benchmarks/bm_chameleon/pyproject.toml
 pyperformance/data-files/benchmarks/bm_chameleon/requirements.txt
 pyperformance/data-files/benchmarks/bm_chameleon/run_benchmark.py
 pyperformance/data-files/benchmarks/bm_chaos/pyproject.toml
 pyperformance/data-files/benchmarks/bm_chaos/run_benchmark.py
+pyperformance/data-files/benchmarks/bm_comprehensions/pyproject.toml
+pyperformance/data-files/benchmarks/bm_comprehensions/run_benchmark.py
 pyperformance/data-files/benchmarks/bm_concurrent_imap/pyproject.toml
 pyperformance/data-files/benchmarks/bm_concurrent_imap/run_benchmark.py
 pyperformance/data-files/benchmarks/bm_coroutines/pyproject.toml
 pyperformance/data-files/benchmarks/bm_coroutines/run_benchmark.py
 pyperformance/data-files/benchmarks/bm_coverage/pyproject.toml
 pyperformance/data-files/benchmarks/bm_coverage/requirements.txt
 pyperformance/data-files/benchmarks/bm_coverage/run_benchmark.py
 pyperformance/data-files/benchmarks/bm_crypto_pyaes/pyproject.toml
 pyperformance/data-files/benchmarks/bm_crypto_pyaes/requirements.txt
 pyperformance/data-files/benchmarks/bm_crypto_pyaes/run_benchmark.py
+pyperformance/data-files/benchmarks/bm_dask/pyproject.toml
+pyperformance/data-files/benchmarks/bm_dask/requirements.txt
+pyperformance/data-files/benchmarks/bm_dask/run_benchmark.py
 pyperformance/data-files/benchmarks/bm_deepcopy/pyproject.toml
 pyperformance/data-files/benchmarks/bm_deepcopy/run_benchmark.py
 pyperformance/data-files/benchmarks/bm_deltablue/pyproject.toml
 pyperformance/data-files/benchmarks/bm_deltablue/run_benchmark.py
 pyperformance/data-files/benchmarks/bm_django_template/pyproject.toml
 pyperformance/data-files/benchmarks/bm_django_template/requirements.txt
 pyperformance/data-files/benchmarks/bm_django_template/run_benchmark.py
@@ -289,14 +359,19 @@
 pyperformance/data-files/benchmarks/bm_sqlite_synth/run_benchmark.py
 pyperformance/data-files/benchmarks/bm_sympy/pyproject.toml
 pyperformance/data-files/benchmarks/bm_sympy/requirements.txt
 pyperformance/data-files/benchmarks/bm_sympy/run_benchmark.py
 pyperformance/data-files/benchmarks/bm_telco/pyproject.toml
 pyperformance/data-files/benchmarks/bm_telco/run_benchmark.py
 pyperformance/data-files/benchmarks/bm_telco/data/telco-bench.b
+pyperformance/data-files/benchmarks/bm_tomli_loads/generate_data.py
+pyperformance/data-files/benchmarks/bm_tomli_loads/pyproject.toml
+pyperformance/data-files/benchmarks/bm_tomli_loads/requirements.txt
+pyperformance/data-files/benchmarks/bm_tomli_loads/run_benchmark.py
+pyperformance/data-files/benchmarks/bm_tomli_loads/data/tomli-bench-data.toml
 pyperformance/data-files/benchmarks/bm_tornado_http/pyproject.toml
 pyperformance/data-files/benchmarks/bm_tornado_http/requirements.txt
 pyperformance/data-files/benchmarks/bm_tornado_http/run_benchmark.py
 pyperformance/data-files/benchmarks/bm_unpack_sequence/pyproject.toml
 pyperformance/data-files/benchmarks/bm_unpack_sequence/run_benchmark.py
 pyperformance/data-files/benchmarks/bm_xml_etree/pyproject.toml
 pyperformance/data-files/benchmarks/bm_xml_etree/run_benchmark.py
```

### Comparing `pyperformance-1.0.6/requirements.in` & `pyperformance-1.0.7/requirements.in`

 * *Files identical despite different names*

### Comparing `pyperformance-1.0.6/setup.py` & `pyperformance-1.0.7/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,10 @@
-#!/usr/bin/env python3
-
-# FIXME:
-#
-# - REENABLE HG_STARTUP BENCHMARK.
-#
 # Update dependencies:
 #
-#  - python3 -m pip install --user --upgrade pip-tools
+#  - python3 -m pip install --user --upgrade pip-tools build
 #  - git clean -fdx  # remove all untracked files!
 #  - (pip-compile --upgrade -o requirements.txt requirements.in)
 #
 # Prepare a release:
 #
 #  - git pull --rebase
 #  - Remove untracked files/dirs: git clean -fdx
@@ -18,68 +12,68 @@
 #  - set release date in doc/changelog.rst
 #  - git commit -a -m "prepare release x.y"
 #  - run tests: tox --parallel auto
 #  - git push
 #  - check the CI status:
 #    https://github.com/python/pyperformance/actions
 #
-# Release a new version:
+# Release a new version with GitHub (preferred):
+#
+#  - go to the GitHub release tab: https://github.com/python/pyperformance/releases
+#  - click "Draft a new release" and fill the contents
+#  - finally click the "Publish release" button! Done!
+#  - monitor the publish status: https://github.com/python/pyperformance/actions/workflows/publish.yml
+#
+# Release a new version manually:
 #
 #  - git tag VERSION
 #  - git push --tags
 #  - Remove untracked files/dirs: git clean -fdx
-#  - python3 setup.py sdist bdist_wheel
+#  - python -m build
 #  - twine upload dist/*
 #
 # After the release:
 #
 #  - set version to n+1: pyperformance/__init__.py and doc/conf.py
 #  - git commit -a -m "post-release"
 #  - git push
 
-# Import just to get the version
-import pyperformance
-
-VERSION = pyperformance.__version__
-
-DESCRIPTION = 'Python benchmark suite'
-CLASSIFIERS = [
+[build-system]
+requires = ["setuptools >= 61"]
+build-backend = "setuptools.build_meta"
+
+[project]
+name = "pyperformance"
+dynamic = ["version"]
+license = {text = "MIT"}
+description = "Python benchmark suite"
+readme = "README.rst"
+urls = {Homepage = "https://github.com/python/pyperformance"}
+authors= [{name = "Collin Winter"}, {name= "Jeffrey Yasskin"}]
+classifiers = [
     'Development Status :: 5 - Production/Stable',
     'Intended Audience :: Developers',
     'License :: OSI Approved :: MIT License',
     'Natural Language :: English',
     'Operating System :: OS Independent',
     'Programming Language :: Python :: 3',
     'Programming Language :: Python',
 ]
+requires-python = ">=3.7"
+dependencies = ["pyperf", "toml", "packaging"]
+
+[project.optional-dependencies]
+dev = [
+    'tox',
+]
 
+[project.scripts]
+pyperformance = "pyperformance.cli:main"
 
-# put most of the code inside main() to be able to import setup.py in
-# unit tests
-def main():
-    import os.path
-    from setuptools import setup, find_packages
-
-    with open('README.rst', encoding="utf8") as fp:
-        long_description = fp.read().strip()
-
-    options = {
-        'name': 'pyperformance',
-        'version': VERSION,
-        'author': 'Collin Winter and Jeffrey Yasskin',
-        'license': 'MIT license',
-        'description': DESCRIPTION,
-        'long_description': long_description,
-        'url': 'https://github.com/python/benchmarks',
-        'classifiers': CLASSIFIERS,
-        'packages': find_packages(),
-        'include_package_data': True,
-        'entry_points': {
-            'console_scripts': ['pyperformance=pyperformance.cli:main']
-        },
-        'install_requires': ["pyperf", "toml", "packaging"],
-    }
-    setup(**options)
+[tool.setuptools]
+include-package-data = true
 
+[tool.setuptools.packages]
+find = {}  # Scanning implicit namespaces is active by default
 
-if __name__ == '__main__':
-    main()
+[tool.setuptools.dynamic]
+version = {attr = "pyperformance.__version__"}
```

