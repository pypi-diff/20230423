# Comparing `tmp/hyperfast_python_template-0.2.8.tar.gz` & `tmp/hyperfast_python_template-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyperfast_python_template-0.2.8.tar", max compression
+gzip compressed data, was "hyperfast_python_template-0.2.9.tar", max compression
```

## Comparing `hyperfast_python_template-0.2.8.tar` & `hyperfast_python_template-0.2.9.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     1071 2023-04-20 23:47:25.428874 hyperfast_python_template-0.2.8/LICENSE
--rw-r--r--   0        0        0     5698 2023-04-20 23:47:20.320919 hyperfast_python_template-0.2.8/README.md
--rw-r--r--   0        0        0     2942 2023-04-20 23:47:42.180771 hyperfast_python_template-0.2.8/pyproject.toml
--rw-r--r--   0        0        0     6282 1970-01-01 00:00:00.000000 hyperfast_python_template-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-04-21 00:05:51.214146 hyperfast_python_template-0.2.9/LICENSE
+-rw-r--r--   0        0        0     5698 2023-04-21 00:05:44.734172 hyperfast_python_template-0.2.9/README.md
+-rw-r--r--   0        0        0     2942 2023-04-21 00:06:12.214193 hyperfast_python_template-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0     6282 1970-01-01 00:00:00.000000 hyperfast_python_template-0.2.9/PKG-INFO
```

### Comparing `hyperfast_python_template-0.2.8/LICENSE` & `hyperfast_python_template-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `hyperfast_python_template-0.2.8/README.md` & `hyperfast_python_template-0.2.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -14,23 +14,23 @@
 [version-image]: https://img.shields.io/github/v/release/entelecheia/hyperfast-python-template?sort=semver
 [release-date-image]: https://img.shields.io/github/release-date/entelecheia/hyperfast-python-template
 [release-url]: https://github.com/entelecheia/hyperfast-python-template/releases
 [conventional-commits-image]: https://img.shields.io/badge/Conventional%20Commits-1.0.0-%23FE5196?logo=conventionalcommits&logoColor=white
 [jupyter-book-image]: https://jupyterbook.org/en/stable/_images/badge.svg
 [repo-url]: https://github.com/entelecheia/hyperfast-python-template
 [pypi-url]: https://pypi.org/project/hyperfast-python-template
-[docs-url]: https://hyperfast-python.entelecheia.cc
+[docs-url]: https://hyperfast-python.entelecheia.ai
 [changelog]: https://github.com/entelecheia/hyperfast-python-template/blob/main/CHANGELOG.md
 [contributing guidelines]: https://github.com/entelecheia/hyperfast-python-template/blob/main/CONTRIBUTING.md
 
 <!-- Links: -->
 
 A python template that helps you jump start your project
 
-- Documentation: [https://hyperfast-python.entelecheia.cc][docs-url]
+- Documentation: [https://hyperfast-python.entelecheia.ai][docs-url]
 - GitHub: [https://github.com/entelecheia/hyperfast-python-template][repo-url]
 - PyPI: [https://pypi.org/project/hyperfast-python-template][pypi-url]
 
 Hyperfast Python Template is a self-contained template that helps you initialize your Python project inside the template. It is hyperfast in the sense that it helps you jump start your project with the best practices in the Python community.
 
 ## Quickstart
```

### Comparing `hyperfast_python_template-0.2.8/pyproject.toml` & `hyperfast_python_template-0.2.9/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [tool.poetry]
 name = "hyperfast-python-template"
-version = "0.2.8"
+version = "0.2.9"
 description = "A python template that helps you jump start your project"
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
-homepage = "https://hyperfast-python.entelecheia.cc"
+homepage = "https://hyperfast-python.entelecheia.ai"
 readme = "README.md"
 packages = [{ include = "hyperfastpy", from = "src" }]
 
 [tool.poetry.scripts]
 hyperfastpy = 'hyperfastpy.__cli__:main'
 
 [tool.poetry.dependencies]
```

### Comparing `hyperfast_python_template-0.2.8/PKG-INFO` & `hyperfast_python_template-0.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: hyperfast-python-template
-Version: 0.2.8
+Version: 0.2.9
 Summary: A python template that helps you jump start your project
-Home-page: https://hyperfast-python.entelecheia.cc
+Home-page: https://hyperfast-python.entelecheia.ai
 License: MIT
 Author: Young Joon Lee
 Author-email: entelecheia@hotmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -30,23 +30,23 @@
 [version-image]: https://img.shields.io/github/v/release/entelecheia/hyperfast-python-template?sort=semver
 [release-date-image]: https://img.shields.io/github/release-date/entelecheia/hyperfast-python-template
 [release-url]: https://github.com/entelecheia/hyperfast-python-template/releases
 [conventional-commits-image]: https://img.shields.io/badge/Conventional%20Commits-1.0.0-%23FE5196?logo=conventionalcommits&logoColor=white
 [jupyter-book-image]: https://jupyterbook.org/en/stable/_images/badge.svg
 [repo-url]: https://github.com/entelecheia/hyperfast-python-template
 [pypi-url]: https://pypi.org/project/hyperfast-python-template
-[docs-url]: https://hyperfast-python.entelecheia.cc
+[docs-url]: https://hyperfast-python.entelecheia.ai
 [changelog]: https://github.com/entelecheia/hyperfast-python-template/blob/main/CHANGELOG.md
 [contributing guidelines]: https://github.com/entelecheia/hyperfast-python-template/blob/main/CONTRIBUTING.md
 
 <!-- Links: -->
 
 A python template that helps you jump start your project
 
-- Documentation: [https://hyperfast-python.entelecheia.cc][docs-url]
+- Documentation: [https://hyperfast-python.entelecheia.ai][docs-url]
 - GitHub: [https://github.com/entelecheia/hyperfast-python-template][repo-url]
 - PyPI: [https://pypi.org/project/hyperfast-python-template][pypi-url]
 
 Hyperfast Python Template is a self-contained template that helps you initialize your Python project inside the template. It is hyperfast in the sense that it helps you jump start your project with the best practices in the Python community.
 
 ## Quickstart
```

