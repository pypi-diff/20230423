# Comparing `tmp/termcolor-2.2.0.tar.gz` & `tmp/termcolor-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, last modified: Sun Apr 23 19:40:30 2023, max compression
```

## Comparing `termcolor-2.2.0.tar` & `termcolor-2.3.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 termcolor-2.2.0/.coveragerc
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 termcolor-2.2.0/.editorconfig
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 termcolor-2.2.0/.flake8
--rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 termcolor-2.2.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 termcolor-2.2.0/CHANGES.md
--rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 termcolor-2.2.0/RELEASING.md
--rw-r--r--   0        0        0      401 2020-02-02 00:00:00.000000 termcolor-2.2.0/tox.ini
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 termcolor-2.2.0/.github/FUNDING.yml
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 termcolor-2.2.0/.github/SECURITY.md
--rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 termcolor-2.2.0/.github/labels.yml
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 termcolor-2.2.0/.github/release-drafter.yml
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 termcolor-2.2.0/.github/renovate.json
--rw-r--r--   0        0        0     1199 2020-02-02 00:00:00.000000 termcolor-2.2.0/.github/workflows/deploy.yml
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 termcolor-2.2.0/.github/workflows/labels.yml
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 termcolor-2.2.0/.github/workflows/lint.yml
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 termcolor-2.2.0/.github/workflows/release-drafter.yml
--rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 termcolor-2.2.0/.github/workflows/require-pr-label.yml
--rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 termcolor-2.2.0/.github/workflows/test.yml
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 termcolor-2.2.0/src/termcolor/__init__.py
--rw-r--r--   0        0        0     2657 2020-02-02 00:00:00.000000 termcolor-2.2.0/src/termcolor/__main__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 termcolor-2.2.0/src/termcolor/py.typed
--rw-r--r--   0        0        0     4627 2020-02-02 00:00:00.000000 termcolor-2.2.0/src/termcolor/termcolor.py
--rw-r--r--   0        0        0     6273 2020-02-02 00:00:00.000000 termcolor-2.2.0/tests/test_termcolor.py
--rw-r--r--   0        0        0     2035 2020-02-02 00:00:00.000000 termcolor-2.2.0/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 termcolor-2.2.0/COPYING.txt
--rw-r--r--   0        0        0     3784 2020-02-02 00:00:00.000000 termcolor-2.2.0/README.md
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 termcolor-2.2.0/pyproject.toml
--rw-r--r--   0        0        0     5267 2020-02-02 00:00:00.000000 termcolor-2.2.0/PKG-INFO
+-rw-r--r--   0        0        0      306 2023-04-23 19:40:30.000000 termcolor-2.3.0/.coveragerc
+-rw-r--r--   0        0        0      313 2023-04-23 19:40:30.000000 termcolor-2.3.0/.editorconfig
+-rw-r--r--   0        0        0       30 2023-04-23 19:40:30.000000 termcolor-2.3.0/.flake8
+-rw-r--r--   0        0        0     1713 2023-04-23 19:40:30.000000 termcolor-2.3.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      561 2023-04-23 19:40:30.000000 termcolor-2.3.0/CHANGES.md
+-rw-r--r--   0        0        0      891 2023-04-23 19:40:30.000000 termcolor-2.3.0/RELEASING.md
+-rw-r--r--   0        0        0      411 2023-04-23 19:40:30.000000 termcolor-2.3.0/tox.ini
+-rw-r--r--   0        0        0       42 2023-04-23 19:40:30.000000 termcolor-2.3.0/.github/FUNDING.yml
+-rw-r--r--   0        0        0      190 2023-04-23 19:40:30.000000 termcolor-2.3.0/.github/SECURITY.md
+-rw-r--r--   0        0        0     1823 2023-04-23 19:40:30.000000 termcolor-2.3.0/.github/labels.yml
+-rw-r--r--   0        0        0      900 2023-04-23 19:40:30.000000 termcolor-2.3.0/.github/release-drafter.yml
+-rw-r--r--   0        0        0      350 2023-04-23 19:40:30.000000 termcolor-2.3.0/.github/renovate.json
+-rw-r--r--   0        0        0     1755 2023-04-23 19:40:30.000000 termcolor-2.3.0/.github/workflows/deploy.yml
+-rw-r--r--   0        0        0      352 2023-04-23 19:40:30.000000 termcolor-2.3.0/.github/workflows/labels.yml
+-rw-r--r--   0        0        0      267 2023-04-23 19:40:30.000000 termcolor-2.3.0/.github/workflows/lint.yml
+-rw-r--r--   0        0        0     1087 2023-04-23 19:40:30.000000 termcolor-2.3.0/.github/workflows/release-drafter.yml
+-rw-r--r--   0        0        0      452 2023-04-23 19:40:30.000000 termcolor-2.3.0/.github/workflows/require-pr-label.yml
+-rw-r--r--   0        0        0     1164 2023-04-23 19:40:30.000000 termcolor-2.3.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0      282 2023-04-23 19:40:30.000000 termcolor-2.3.0/src/termcolor/__init__.py
+-rw-r--r--   0        0        0     2657 2023-04-23 19:40:30.000000 termcolor-2.3.0/src/termcolor/__main__.py
+-rw-r--r--   0        0        0        0 2023-04-23 19:40:30.000000 termcolor-2.3.0/src/termcolor/py.typed
+-rw-r--r--   0        0        0     5628 2023-04-23 19:40:30.000000 termcolor-2.3.0/src/termcolor/termcolor.py
+-rw-r--r--   0        0        0     7347 2023-04-23 19:40:30.000000 termcolor-2.3.0/tests/test_termcolor.py
+-rw-r--r--   0        0        0     2035 2023-04-23 19:40:30.000000 termcolor-2.3.0/.gitignore
+-rw-r--r--   0        0        0     1072 2023-04-23 19:40:30.000000 termcolor-2.3.0/COPYING.txt
+-rw-r--r--   0        0        0     3784 2023-04-23 19:40:30.000000 termcolor-2.3.0/README.md
+-rw-r--r--   0        0        0     1707 2023-04-23 19:40:30.000000 termcolor-2.3.0/pyproject.toml
+-rw-r--r--   0        0        0     5318 2023-04-23 19:40:30.000000 termcolor-2.3.0/PKG-INFO
```

### Comparing `termcolor-2.2.0/.pre-commit-config.yaml` & `termcolor-2.3.0/.pre-commit-config.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -2,69 +2,71 @@
   - repo: https://github.com/asottile/pyupgrade
     rev: v3.3.1
     hooks:
       - id: pyupgrade
         args: [--py37-plus]
 
   - repo: https://github.com/psf/black
-    rev: 22.12.0
+    rev: 23.3.0
     hooks:
       - id: black
-        args: [--target-version=py37]
 
   - repo: https://github.com/PyCQA/isort
-    rev: 5.11.4
+    rev: 5.12.0
     hooks:
       - id: isort
         args: [--add-import=from __future__ import annotations]
 
   - repo: https://github.com/PyCQA/flake8
     rev: 6.0.0
     hooks:
       - id: flake8
-        additional_dependencies: [flake8-2020, flake8-implicit-str-concat]
+        additional_dependencies:
+          [flake8-2020, flake8-errmsg, flake8-implicit-str-concat]
 
   - repo: https://github.com/pre-commit/pygrep-hooks
-    rev: v1.9.0
+    rev: v1.10.0
     hooks:
       - id: python-check-blanket-noqa
+      - id: python-no-log-warn
 
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.4.0
     hooks:
-      - id: check-json
+      - id: check-case-conflict
       - id: check-merge-conflict
+      - id: check-json
       - id: check-toml
       - id: check-yaml
       - id: end-of-file-fixer
       - id: trailing-whitespace
 
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v0.991
+    rev: v1.2.0
     hooks:
       - id: mypy
         args: [--strict, --pretty, --show-error-codes]
         additional_dependencies: [pytest]
 
   - repo: https://github.com/tox-dev/pyproject-fmt
-    rev: 0.4.1
+    rev: 0.9.2
     hooks:
       - id: pyproject-fmt
 
   - repo: https://github.com/abravalheri/validate-pyproject
-    rev: v0.10.1
+    rev: v0.12.2
     hooks:
       - id: validate-pyproject
 
   - repo: https://github.com/tox-dev/tox-ini-fmt
-    rev: 0.5.2
+    rev: 1.3.0
     hooks:
       - id: tox-ini-fmt
 
   - repo: https://github.com/pre-commit/mirrors-prettier
-    rev: v3.0.0-alpha.4
+    rev: v3.0.0-alpha.6
     hooks:
       - id: prettier
         args: [--prose-wrap=always, --print-width=88]
 
 ci:
   autoupdate_schedule: quarterly
```

### Comparing `termcolor-2.2.0/CHANGES.md` & `termcolor-2.3.0/CHANGES.md`

 * *Files identical despite different names*

### Comparing `termcolor-2.2.0/RELEASING.md` & `termcolor-2.3.0/RELEASING.md`

 * *Files identical despite different names*

### Comparing `termcolor-2.2.0/.github/labels.yml` & `termcolor-2.3.0/.github/labels.yml`

 * *Files identical despite different names*

### Comparing `termcolor-2.2.0/.github/release-drafter.yml` & `termcolor-2.3.0/.github/release-drafter.yml`

 * *Files 20% similar despite different names*

```diff
@@ -18,14 +18,19 @@
       - "bug"
   - title: "Security"
     label: "changelog: Security"
 
 exclude-labels:
   - "changelog: skip"
 
+autolabeler:
+  - label: "changelog: skip"
+    branch:
+      - "/pre-commit-ci-update-config/"
+
 template: |
   $CHANGES
 
 version-resolver:
   major:
     labels:
       - "changelog: Removed"
```

### Comparing `termcolor-2.2.0/.github/workflows/test.yml` & `termcolor-2.3.0/.github/workflows/test.yml`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 jobs:
   test:
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
-        python-version: ["pypy-3.8", "3.7", "3.8", "3.9", "3.10", "3.11"]
+        python-version: ["pypy3.9", "3.7", "3.8", "3.9", "3.10", "3.11", "3.12-dev"]
         os: [windows-latest, macos-latest, ubuntu-latest]
 
     steps:
       - uses: actions/checkout@v3
 
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v4
```

### Comparing `termcolor-2.2.0/src/termcolor/__main__.py` & `termcolor-2.3.0/src/termcolor/__main__.py`

 * *Files identical despite different names*

### Comparing `termcolor-2.2.0/src/termcolor/termcolor.py` & `termcolor-2.3.0/src/termcolor/termcolor.py`

 * *Files 20% similar despite different names*

```diff
@@ -35,15 +35,16 @@
         warnings.warn(
             "__ALL__ is deprecated and will be removed in termcolor 3. "
             "Use __all__ instead.",
             DeprecationWarning,
             stacklevel=2,
         )
         return ["colored", "cprint"]
-    raise AttributeError(f"module '{__name__}' has no attribute '{name}'")
+    msg = f"module '{__name__}' has no attribute '{name}'"
+    raise AttributeError(msg)
 
 
 ATTRIBUTES = {
     "bold": 1,
     "dark": 2,
     "underline": 4,
     "blink": 5,
@@ -92,16 +93,30 @@
     "white": 97,
 }
 
 
 RESET = "\033[0m"
 
 
-def _can_do_colour() -> bool:
+def _can_do_colour(
+    *, no_color: bool | None = None, force_color: bool | None = None
+) -> bool:
     """Check env vars and for tty/dumb terminal"""
+    # First check overrides:
+    # "User-level configuration files and per-instance command-line arguments should
+    # override $NO_COLOR. A user should be able to export $NO_COLOR in their shell
+    # configuration file as a default, but configure a specific program in its
+    # configuration file to specifically enable color."
+    # https://no-color.org
+    if no_color is not None and no_color:
+        return False
+    if force_color is not None and force_color:
+        return True
+
+    # Then check env vars:
     if "ANSI_COLORS_DISABLED" in os.environ:
         return False
     if "NO_COLOR" in os.environ:
         return False
     if "FORCE_COLOR" in os.environ:
         return True
     return (
@@ -112,14 +127,17 @@
 
 
 def colored(
     text: str,
     color: str | None = None,
     on_color: str | None = None,
     attrs: Iterable[str] | None = None,
+    *,
+    no_color: bool | None = None,
+    force_color: bool | None = None,
 ) -> str:
     """Colorize text.
 
     Available text colors:
         black, red, green, yellow, blue, magenta, cyan, white,
         light_grey, dark_grey, light_red, light_green, light_yellow, light_blue,
         light_magenta, light_cyan.
@@ -132,15 +150,15 @@
     Available attributes:
         bold, dark, underline, blink, reverse, concealed.
 
     Example:
         colored('Hello, World!', 'red', 'on_black', ['bold', 'blink'])
         colored('Hello, World!', 'green')
     """
-    if not _can_do_colour():
+    if not _can_do_colour(no_color=no_color, force_color=force_color):
         return text
 
     fmt_str = "\033[%dm%s"
     if color is not None:
         text = fmt_str % (COLORS[color], text)
 
     if on_color is not None:
@@ -154,15 +172,30 @@
 
 
 def cprint(
     text: str,
     color: str | None = None,
     on_color: str | None = None,
     attrs: Iterable[str] | None = None,
+    *,
+    no_color: bool | None = None,
+    force_color: bool | None = None,
     **kwargs: Any,
 ) -> None:
-    """Print colorize text.
+    """Print colorized text.
 
     It accepts arguments of print function.
     """
 
-    print((colored(text, color, on_color, attrs)), **kwargs)
+    print(
+        (
+            colored(
+                text,
+                color,
+                on_color,
+                attrs,
+                no_color=no_color,
+                force_color=force_color,
+            )
+        ),
+        **kwargs,
+    )
```

### Comparing `termcolor-2.2.0/tests/test_termcolor.py` & `termcolor-2.3.0/tests/test_termcolor.py`

 * *Files 27% similar despite different names*

```diff
@@ -32,14 +32,18 @@
 def test_sanity() -> None:
     for color in ALL_COLORS:
         for highlight in ALL_HIGHLIGHTS:
             for attribute in ALL_ATTRIBUTES:
                 attrs = None if attribute is None else [attribute]
                 colored("text", color, highlight, attrs)
                 cprint("text", color, highlight, attrs)
+                colored("text", color, highlight, attrs, no_color=True)
+                cprint("text", color, highlight, attrs, no_color=True)
+                colored("text", color, highlight, attrs, force_color=True)
+                cprint("text", color, highlight, attrs, force_color=True)
 
 
 def assert_cprint(
     capsys: pytest.CaptureFixture[str],
     expected: str,
     text: str,
     color: str | None = None,
@@ -180,33 +184,54 @@
 ) -> None:
     """Assert color applied when this env var set, regardless of value"""
     monkeypatch.setenv("FORCE_COLOR", test_value)
     assert colored("text", color="cyan") == "\x1b[36mtext\x1b[0m"
 
 
 @pytest.mark.parametrize(
-    "test_env_vars, expected",
+    "test_no_color, test_force_color, test_env_vars, expected",
     [
-        (["ANSI_COLORS_DISABLED=1"], False),
-        (["NO_COLOR=1"], False),
-        (["FORCE_COLOR=1"], True),
-        (["ANSI_COLORS_DISABLED=1", "NO_COLOR=1", "FORCE_COLOR=1"], False),
-        (["NO_COLOR=1", "FORCE_COLOR=1"], False),
+        # Set only env vars
+        (None, None, ["ANSI_COLORS_DISABLED=1"], False),
+        (None, None, ["NO_COLOR=1"], False),
+        (None, None, ["FORCE_COLOR=1"], True),
+        (None, None, ["ANSI_COLORS_DISABLED=1", "NO_COLOR=1", "FORCE_COLOR=1"], False),
+        (None, None, ["NO_COLOR=1", "FORCE_COLOR=1"], False),
+        # Set only parameter overrides
+        (True, None, [None], False),
+        (None, True, [None], True),
+        (True, True, [None], False),
+        # Set both parameter overrides and env vars
+        (True, None, ["NO_COLOR=1"], False),
+        (None, True, ["NO_COLOR=1"], True),
+        (True, True, ["NO_COLOR=1"], False),
+        (True, None, ["FORCE_COLOR=1"], False),
+        (None, True, ["FORCE_COLOR=1"], True),
+        (True, True, ["FORCE_COLOR=1"], False),
     ],
 )
 def test_environment_variables(
-    monkeypatch: pytest.MonkeyPatch, test_env_vars: str, expected: bool
+    monkeypatch: pytest.MonkeyPatch,
+    test_no_color: bool,
+    test_force_color: bool,
+    test_env_vars: str,
+    expected: bool,
 ) -> None:
     """Assert combinations do the right thing"""
     for env_var in test_env_vars:
+        if not env_var:
+            continue
         name, value = env_var.split("=")
         print(name, value)
         monkeypatch.setenv(name, value)
 
-    assert termcolor._can_do_colour() == expected
+    assert (
+        termcolor._can_do_colour(no_color=test_no_color, force_color=test_force_color)
+        == expected
+    )
 
 
 @pytest.mark.parametrize(
     "test_isatty, expected",
     [
         (True, "\x1b[36mtext\x1b[0m"),
         (False, "text"),
```

### Comparing `termcolor-2.2.0/.gitignore` & `termcolor-2.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `termcolor-2.2.0/COPYING.txt` & `termcolor-2.3.0/COPYING.txt`

 * *Files identical despite different names*

### Comparing `termcolor-2.2.0/README.md` & `termcolor-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `termcolor-2.2.0/pyproject.toml` & `termcolor-2.3.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -19,50 +19,46 @@
   "termcolor",
   "terminal",
 ]
 license = {text = "MIT"}
 maintainers = [{name = "Hugo van Kemenade"}]
 authors = [{name = "Konstantin Lepa", email = "konstantin.lepa@gmail.com"}]
 requires-python = ">=3.7"
-dynamic = [
-  "version",
-]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Console",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
     "Topic :: Terminals",
 ]
+dynamic = [
+  "version",
+]
 [project.optional-dependencies]
 tests = [
   "pytest",
   "pytest-cov",
 ]
-
 [project.urls]
 Changelog = "https://github.com/termcolor/termcolor/releases"
 Homepage = "https://github.com/termcolor/termcolor"
 Source = "https://github.com/termcolor/termcolor"
 
-
-[tool.black]
-target_version = ["py37"]
-
 [tool.hatch]
 version.source = "vcs"
 
 [tool.hatch.version.raw-options]
 local_scheme = "no-local-version"
 
 [tool.isort]
```

### Comparing `termcolor-2.2.0/PKG-INFO` & `termcolor-2.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: termcolor
-Version: 2.2.0
+Version: 2.3.0
 Summary: ANSI color formatting for output in terminal
 Project-URL: Changelog, https://github.com/termcolor/termcolor/releases
 Project-URL: Homepage, https://github.com/termcolor/termcolor
 Project-URL: Source, https://github.com/termcolor/termcolor
 Author-email: Konstantin Lepa <konstantin.lepa@gmail.com>
 Maintainer: Hugo van Kemenade
 License: MIT
@@ -19,14 +19,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Terminals
 Requires-Python: >=3.7
 Provides-Extra: tests
 Requires-Dist: pytest; extra == 'tests'
 Requires-Dist: pytest-cov; extra == 'tests'
```

