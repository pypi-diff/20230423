# Comparing `tmp/prettycopy-0.1.2.tar.gz` & `tmp/prettycopy-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prettycopy-0.1.2.tar", last modified: Mon Apr  3 21:32:01 2023, max compression
+gzip compressed data, was "prettycopy-0.1.3.tar", last modified: Sun Apr 23 15:10:27 2023, max compression
```

## Comparing `prettycopy-0.1.2.tar` & `prettycopy-0.1.3.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-04-03 21:32:01.490438 prettycopy-0.1.2/
--rw-rw-rw-   0        0        0      408 2023-03-21 21:01:19.000000 prettycopy-0.1.2/.bumpversion.cfg
--rw-rw-rw-   0        0        0      772 2023-04-03 20:39:32.000000 prettycopy-0.1.2/.readthedocs.yaml
--rw-rw-rw-   0        0        0     2202 2023-03-31 21:48:57.000000 prettycopy-0.1.2/CONTRIBUTING.md
--rw-rw-rw-   0        0        0    11558 2023-02-08 23:02:52.000000 prettycopy-0.1.2/LICENSE
--rw-rw-rw-   0        0        0      555 2023-04-03 20:39:32.000000 prettycopy-0.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0     2254 2023-03-07 22:31:03.000000 prettycopy-0.1.2/Makefile
--rw-rw-rw-   0        0        0    17046 2023-04-03 21:32:01.488438 prettycopy-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     3002 2023-04-03 21:16:39.000000 prettycopy-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-03 21:32:01.442438 prettycopy-0.1.2/docs/
--rw-rw-rw-   0        0        0      634 2023-03-31 21:48:57.000000 prettycopy-0.1.2/docs/Makefile
--rw-rw-rw-   0        0        0     1302 2023-04-03 21:28:44.000000 prettycopy-0.1.2/docs/conf.py
--rw-rw-rw-   0        0        0     2196 2023-03-31 21:48:57.000000 prettycopy-0.1.2/docs/dev_intro.md
--rw-rw-rw-   0        0        0     2079 2023-03-31 22:26:59.000000 prettycopy-0.1.2/docs/index.md
--rwxrwxrwx   0        0        0      765 2023-03-31 21:48:57.000000 prettycopy-0.1.2/docs/make.bat
--rw-rw-rw-   0        0        0       64 2023-04-03 21:28:44.000000 prettycopy-0.1.2/docs/requirements.txt
-drwxrwxrwx   0        0        0        0 2023-04-03 21:32:01.461436 prettycopy-0.1.2/prettycopy/
--rw-rw-rw-   0        0        0      201 2023-04-03 21:28:44.000000 prettycopy-0.1.2/prettycopy/__init__.py
--rw-rw-rw-   0        0        0       82 2023-03-04 17:13:11.000000 prettycopy-0.1.2/prettycopy/__main__.py
--rw-rw-rw-   0        0        0       22 2023-04-03 21:28:44.000000 prettycopy-0.1.2/prettycopy/_version.py
--rw-rw-rw-   0        0        0     2146 2023-03-31 21:48:57.000000 prettycopy-0.1.2/prettycopy/gdocs.py
--rw-rw-rw-   0        0        0     5611 2023-03-31 21:48:57.000000 prettycopy-0.1.2/prettycopy/prettycopy.py
-drwxrwxrwx   0        0        0        0 2023-04-03 21:32:01.482440 prettycopy-0.1.2/prettycopy/tests/
--rw-rw-rw-   0        0        0    11311 2023-03-31 21:48:57.000000 prettycopy-0.1.2/prettycopy/tests/test_all.py
-drwxrwxrwx   0        0        0        0 2023-04-03 21:32:01.479435 prettycopy-0.1.2/prettycopy.egg-info/
--rw-rw-rw-   0        0        0    17046 2023-04-03 21:32:01.000000 prettycopy-0.1.2/prettycopy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      520 2023-04-03 21:32:01.000000 prettycopy-0.1.2/prettycopy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-03 21:32:01.000000 prettycopy-0.1.2/prettycopy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      224 2023-04-03 21:32:01.000000 prettycopy-0.1.2/prettycopy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-03 21:32:01.000000 prettycopy-0.1.2/prettycopy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2247 2023-04-03 21:28:44.000000 prettycopy-0.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-03 21:32:01.491438 prettycopy-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0       39 2023-03-02 04:28:18.000000 prettycopy-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-23 15:10:27.118782 prettycopy-0.1.3/
+-rw-rw-rw-   0        0        0      533 2023-04-23 00:51:02.000000 prettycopy-0.1.3/.bumpversion.cfg
+-rw-rw-rw-   0        0        0      772 2023-04-17 05:17:35.000000 prettycopy-0.1.3/.readthedocs.yaml
+-rw-rw-rw-   0        0        0     2197 2023-04-17 05:17:35.000000 prettycopy-0.1.3/CONTRIBUTING.md
+-rw-rw-rw-   0        0        0    11558 2023-02-08 23:02:52.000000 prettycopy-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0      584 2023-04-17 05:17:35.000000 prettycopy-0.1.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     2254 2023-04-22 23:54:45.000000 prettycopy-0.1.3/Makefile
+-rw-rw-rw-   0        0        0    17353 2023-04-23 15:10:27.115781 prettycopy-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3303 2023-04-22 23:35:54.000000 prettycopy-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-23 15:10:27.052800 prettycopy-0.1.3/docs/
+-rw-rw-rw-   0        0        0      634 2023-03-31 21:48:57.000000 prettycopy-0.1.3/docs/Makefile
+-rw-rw-rw-   0        0        0     1302 2023-04-23 00:51:02.000000 prettycopy-0.1.3/docs/conf.py
+-rw-rw-rw-   0        0        0     2198 2023-04-22 23:18:03.000000 prettycopy-0.1.3/docs/dev_intro.md
+drwxrwxrwx   0        0        0        0 2023-04-23 15:10:27.056795 prettycopy-0.1.3/docs/images/
+-rw-rw-rw-   0        0        0   185808 2023-04-17 05:17:35.000000 prettycopy-0.1.3/docs/images/bullettopar.gif
+-rw-rw-rw-   0        0        0     4749 2023-04-22 23:35:54.000000 prettycopy-0.1.3/docs/index.md
+-rwxrwxrwx   0        0        0      765 2023-03-31 21:48:57.000000 prettycopy-0.1.3/docs/make.bat
+-rw-rw-rw-   0        0        0       64 2023-04-23 00:24:41.000000 prettycopy-0.1.3/docs/requirements.txt
+drwxrwxrwx   0        0        0        0 2023-04-23 15:10:27.073796 prettycopy-0.1.3/prettycopy/
+-rw-rw-rw-   0        0        0      103 2023-04-23 00:51:02.000000 prettycopy-0.1.3/prettycopy/__init__.py
+-rw-rw-rw-   0        0        0       82 2023-03-04 17:13:11.000000 prettycopy-0.1.3/prettycopy/__main__.py
+-rw-rw-rw-   0        0        0       22 2023-04-23 00:51:02.000000 prettycopy-0.1.3/prettycopy/_version.py
+-rw-rw-rw-   0        0        0    11294 2023-04-22 23:35:54.000000 prettycopy-0.1.3/prettycopy/prettycopy.py
+drwxrwxrwx   0        0        0        0 2023-04-23 15:10:27.103947 prettycopy-0.1.3/prettycopy/tests/
+-rw-rw-rw-   0        0        0    16889 2023-04-22 23:35:54.000000 prettycopy-0.1.3/prettycopy/tests/test_all.py
+drwxrwxrwx   0        0        0        0 2023-04-23 15:10:27.100039 prettycopy-0.1.3/prettycopy.egg-info/
+-rw-rw-rw-   0        0        0    17353 2023-04-23 15:10:26.000000 prettycopy-0.1.3/prettycopy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      528 2023-04-23 15:10:26.000000 prettycopy-0.1.3/prettycopy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-23 15:10:26.000000 prettycopy-0.1.3/prettycopy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      253 2023-04-23 15:10:26.000000 prettycopy-0.1.3/prettycopy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-04-23 15:10:26.000000 prettycopy-0.1.3/prettycopy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2297 2023-04-23 00:51:02.000000 prettycopy-0.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-23 15:10:27.122780 prettycopy-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0       39 2023-03-02 04:28:18.000000 prettycopy-0.1.3/setup.py
```

### Comparing `prettycopy-0.1.2/.readthedocs.yaml` & `prettycopy-0.1.3/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `prettycopy-0.1.2/CONTRIBUTING.md` & `prettycopy-0.1.3/docs/dev_intro.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,64 +1,52 @@
-## Contributing
+# Intro to Developers
 Welcome to PrettyCopy! Thanks for your interest in contributing. We're happy to have you :)
 
-### Reporting Issues, Feature Requests
+## Reporting Issues, Feature Requests
 You have an issue or feature request? Great to know! Just head to the Issues page on our GitHub, [PrettyCopy Issues](https://github.com/hippothebrave/prettycopy/issues), open a "New Issue," and fill it out with whatever you have.
 
 A good bug report includes:
 
 - Expected behavior
 - Actual behavior
 - Steps to reproduce (preferably as minimal as possible)
 - Anything else you think is relevant.
 
 The more information you give us, the more likely it is that we can find a solution!
 
-### Developing
-Want to help with development? Wonderful! Here's how to begin.
+## Developing
+Want to help with development? Even better! Here's how to begin.
 
-#### Setup
-1. Prerequisites: Install Python. At the moment, PrettyCopy runs on Python version 3.7 and higher.
-2. Fork the repository on GitHub.
-3. Clone your forked repository to your local computer using `git clone https://github.com/[YOUR_USERNAME]/prettycopy.git`
-4. Navigate to the folder, and type `make develop` to install the development dependencies. (You can check the file *pyproject.toml* to see what they are.)
-5. Congrats, you're ready to get started coding!
+### Setup
+Prerequisites: Install Python. At the moment, PrettyCopy runs on Python version 3.7 and higher.
 
-#### Make changes
-Now make your changes.
-
-Run tests to ensure that your changes does not break anything.
-
-```bash
-make test
-```
+1. Fork the repository on GitHub.
+2. Clone your forked repository to your local computer using `git clone https://github.com/[YOUR_USERNAME]/prettycopy.git`
+3. Navigate to the folder, and type `make develop` to install the development dependencies. (You can check the file *pyproject.toml* to see what they are.)
+4. Congrats, you're ready to get started coding!
 
-Edit or add to the existing tests to check that your changes work as expected. All test files should go under the *prettycopy/tests/* directory, and all test functions must begin with the prefix `test_`. You can run `make coverage` to see if there's any code left untested.
+### Make changes
+Now make your changes.
 
-Check the formatting of your code by running
+Create, add to, and run tests to ensure that your changes work as expected and do not break anything. Run tests with the command `make test`, and check if there's any code left untested with the command `make coverage`. All test files should go under the *prettycopy/tests/* directory, and all test functions must begin with the prefix `test_` in order to be recognized.
 
-```bash
-make lint
-```
+Check the formatting of your code by running `make lint`. As necessary, automatically fix the formatting by running `make format`.
 
-and if necessary, automatically fix the style by running
+Finally, as a last check, you may wish to try building your code before making the pull request. That means running, in order,
 
-```bash
-make format
 ```
+make develop
 
-Finally, as a last check, you may wish to try building your code before making the pull request. That means running, in order,
-> make develop
-
-> make build
+make build
 
-> make lint
+make lint
 
-> make checks
+make checks
 
-> make coverage
+make coverage
+```
 
-Commit your changes, and publish the branch to your GitHub repo.
+Commit your final changes, and publish the branch to your GitHub repo.
 
 Finally, head to [PrettyCopy PRs](https://github.com/hippothebrave/prettycopy/pulls) on the main repo and add a pull request linked to your forked repo. 
 
-Thank you so much for your contribution! 
+Thank you so much for your contribution!
```

### Comparing `prettycopy-0.1.2/LICENSE` & `prettycopy-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `prettycopy-0.1.2/Makefile` & `prettycopy-0.1.3/Makefile`

 * *Files identical despite different names*

### Comparing `prettycopy-0.1.2/PKG-INFO` & `prettycopy-0.1.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prettycopy
-Version: 0.1.2
+Version: 0.1.3
 Summary: A better copy-paster
 Author-email: Adi Gal <adigal03@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -267,8 +267,14 @@
 
 `prettycopy.quote(optional_end_punctuation, optional_text)`: Adds quotation marks around the text, ending in a punctuation mark. The default is a comma.
 
 > Example: *this is a test* --> prettycopy.quote() --> *"this is a test,"*
 
 > Example: *this is a test* --> prettycopy.quote('!') --> *"this is a test!"*
 
+`prettycopy.trimspacing(optional_text)`: Removes empty lines.
+
+`prettycopy.smartcopy(optional_text)`: Removes line breaks in an intelligent manner: adding spaces between words, but not inside words that have been split.
+
+> Example: *this\nis a te\nst* --> prettycopy.smartcopy() --> *this is a test*
+
 `prettycopy.betterbullets(docID)`: If you enter the document ID of an editable Google Doc (the long string of letters and numbers in the URL), this function will copy the text in your clipboard to the end of the document, replacing all bullet symbols (•) with correctly-formatted bullet points. Still under construction.
```

### Comparing `prettycopy-0.1.2/README.md` & `prettycopy-0.1.3/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -45,8 +45,14 @@
 
 `prettycopy.quote(optional_end_punctuation, optional_text)`: Adds quotation marks around the text, ending in a punctuation mark. The default is a comma.
 
 > Example: *this is a test* --> prettycopy.quote() --> *"this is a test,"*
 
 > Example: *this is a test* --> prettycopy.quote('!') --> *"this is a test!"*
 
+`prettycopy.trimspacing(optional_text)`: Removes empty lines.
+
+`prettycopy.smartcopy(optional_text)`: Removes line breaks in an intelligent manner: adding spaces between words, but not inside words that have been split.
+
+> Example: *this\nis a te\nst* --> prettycopy.smartcopy() --> *this is a test*
+
 `prettycopy.betterbullets(docID)`: If you enter the document ID of an editable Google Doc (the long string of letters and numbers in the URL), this function will copy the text in your clipboard to the end of the document, replacing all bullet symbols (•) with correctly-formatted bullet points. Still under construction.
```

### Comparing `prettycopy-0.1.2/docs/Makefile` & `prettycopy-0.1.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `prettycopy-0.1.2/docs/conf.py` & `prettycopy-0.1.3/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
 project = 'prettycopy'
 copyright = '2023, Adi Gal'
 author = 'Adi Gal'
-release = '0.1.2'
+release = "0.1.3"
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = ['myst_parser', 'sphinx.ext.autodoc', 'sphinx.ext.githubpages'] #prev, recommonmark
 source_suffix = ['.rst', '.md']
```

### Comparing `prettycopy-0.1.2/docs/dev_intro.md` & `prettycopy-0.1.3/CONTRIBUTING.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,55 +1,38 @@
-# Intro to Developers
+## Contributing
 Welcome to PrettyCopy! Thanks for your interest in contributing. We're happy to have you :)
 
-## Reporting Issues, Feature Requests
+### Reporting Issues, Feature Requests
 You have an issue or feature request? Great to know! Just head to the Issues page on our GitHub, [PrettyCopy Issues](https://github.com/hippothebrave/prettycopy/issues), open a "New Issue," and fill it out with whatever you have.
 
 A good bug report includes:
 
 - Expected behavior
 - Actual behavior
 - Steps to reproduce (preferably as minimal as possible)
 - Anything else you think is relevant.
 
 The more information you give us, the more likely it is that we can find a solution!
 
-## Developing
-Want to help with development? Even better! Here's how to begin.
+### Developing
+Want to help with development? Wonderful! Here's how to begin.
 
-### Setup
-Prerequisites: Install Python. At the moment, PrettyCopy runs on Python version 3.7 and higher.
+#### Setup
+1. Prerequisites: Install Python. At the moment, PrettyCopy runs on Python version 3.7 and higher.
+2. Fork the repository on GitHub.
+3. Clone your forked repository to your local computer using `git clone https://github.com/[YOUR_USERNAME]/prettycopy.git`
+4. Navigate to the folder, and type `make develop` to install the development dependencies. (You can check the file *pyproject.toml* to see what they are.)
+5. Congrats, you're ready to get started coding!
 
-1. Fork the repository on GitHub.
-2. Clone your forked repository to your local computer using `git clone https://github.com/[YOUR_USERNAME]/prettycopy.git`
-3. Navigate to the folder, and type `make develop` to install the development dependencies. (You can check the file *pyproject.toml* to see what they are.)
-4. Congrats, you're ready to get started coding!
-
-### Make changes
+#### Make changes
 Now make your changes.
 
-Run tests to ensure that your changes does not break anything.
-
-```
-make test
-```
+Create, add to, and run tests to ensure that your changes work as expected and do not break anything. Run tests with the command `make test`, and check if there's any code left untested with the command `make coverage`. All test files should go under the *prettycopy/tests/* directory, and all test functions must begin with the prefix `test_` in order to be recognized.
 
-Edit or add to the existing tests to check that your changes work as expected. All test files should go under the *prettycopy/tests/* directory, and all test functions must begin with the prefix `test_`. You can run `make coverage` to see if there's any code left untested.
-
-Check the formatting of your code by running
-
-```
-make lint
-```
-
-and if necessary, automatically fix the style by running
-
-```
-make format
-```
+Check the formatting of your code by running `make lint`. As necessary, automatically fix the formatting by running `make format`.
 
 Finally, as a last check, you may wish to try building your code before making the pull request. That means running, in order,
 
 ```
 make develop
 
 make build
@@ -61,8 +44,8 @@
 make coverage
 ```
 
 Commit your final changes, and publish the branch to your GitHub repo.
 
 Finally, head to [PrettyCopy PRs](https://github.com/hippothebrave/prettycopy/pulls) on the main repo and add a pull request linked to your forked repo. 
 
-Thank you so much for your contribution! 
+Thank you so much for your contribution!
```

### Comparing `prettycopy-0.1.2/docs/make.bat` & `prettycopy-0.1.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `prettycopy-0.1.2/prettycopy/tests/test_all.py` & `prettycopy-0.1.3/prettycopy/tests/test_all.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,95 +1,134 @@
-# import prettycopy as pc
 import prettycopy.prettycopy as pc
-from prettycopy.gdocs import getservice
 
-# from prettycopy import nonewlines, nobullets, bullettopar, quote, simplequote
 from unittest.mock import patch, MagicMock
 from googleapiclient.errors import HttpError
 
+import pytest
+
 
 def test_nonewlines():
     with patch("pyperclip.copy") as copy_mock, patch("pyperclip.paste") as paste_mock:
+        # Bad type
+        paste_mock.return_value = 77
+        with pytest.raises(ValueError):
+            ret = pc.nonewlines()
+
         # Text from clipboard
         paste_mock.return_value = "Testing\n line \nof text\n here."
         ret = pc.nonewlines()
         assert ret == "Testing line of text here."
         assert copy_mock.call_args.args == (ret,)
 
+        # Spacing
+        paste_mock.return_value = "Testing\nline\nof text\nhere."
+        ret = pc.nonewlines()
+        assert ret == "Testing line of text here."
+        assert copy_mock.call_args.args == (ret,)
+
         # Text from argument
         ret = pc.nonewlines("Another\n line \nof text\n here.")
         assert ret == "Another line of text here."
         assert copy_mock.call_args.args == (ret,)
 
 
 def test_nobullets():
     with patch("pyperclip.copy") as copy_mock, patch("pyperclip.paste") as paste_mock, patch(
         "prettycopy.prettycopy.nonewlines"
     ) as newline_mock:
+        # Bad type
+        paste_mock.return_value = 42
+        with pytest.raises(ValueError):
+            ret = pc.nobullets()
+
         # No spaces
         paste_mock.return_value = "•Test\n•Test"
-        newline_mock.return_value = "•Test•Test"
+        newline_mock.return_value = '•Test •Test'
         ret = pc.nobullets()
         newline_mock.assert_called_once()
         assert newline_mock.call_args.args == ()
         assert ret == "Test\nTest"
         assert copy_mock.call_args.args == (ret,)
 
         # Spaces between bullet and text
         paste_mock.return_value = "• Test\n• Test"
-        newline_mock.return_value = "• Test• Test"
+        newline_mock.return_value = '• Test • Test'
+        ret = pc.nobullets()
+        assert newline_mock.call_args.args == ()
+        assert ret == "Test\nTest"
+        assert copy_mock.call_args.args == (ret,)
+
+        # Spaces around bullet and text
+        paste_mock.return_value = "   • Test\n  •\tTest   •"
+        newline_mock.return_value = '• Test • Test •'
         ret = pc.nobullets()
         assert newline_mock.call_args.args == ()
         assert ret == "Test\nTest"
         assert copy_mock.call_args.args == (ret,)
 
         # Bullets within words
         paste_mock.return_value = "•   Te•st• Test"
-        newline_mock.return_value = "•   Te•st• Test"
+        newline_mock.return_value = '• Te•st• Test'
         ret = pc.nobullets()
         assert newline_mock.call_args.args == ()
         assert ret == "Te\nst\nTest"
         assert copy_mock.call_args.args == (ret,)
 
         # Text from argument
-        newline_mock.return_value = "•Another•Test"
+        newline_mock.return_value = '•Another •Test'
         ret = pc.nobullets("•Another\n•Test")
         assert newline_mock.call_args.args == ()
         assert ret == "Another\nTest"
         assert copy_mock.call_args.args == (ret,)
 
 
 def test_bullettopar():
     with patch("pyperclip.copy") as copy_mock, patch("pyperclip.paste") as paste_mock:
+        # Bad type
+        paste_mock.return_value = 77
+        with pytest.raises(ValueError):
+            pc.bullettopar()
+
         # No spaces
         paste_mock.return_value = "•Test\n•Test"
-        ret = pc.bullettopar()
-        assert ret == "Test Test"
-        assert copy_mock.call_args.args == (ret,)
+        ret1 = pc.bullettopar()
+        assert ret1 == "Test Test"
+        assert copy_mock.call_args.args == (ret1,)
 
         # Spaces after bullets
         paste_mock.return_value = "• Test\n• Test"
-        ret = pc.bullettopar()
-        assert ret == "Test Test"
-        assert copy_mock.call_args.args == (ret,)
+        ret2 = pc.bullettopar()
+        assert ret2 == "Test Test"
+        assert copy_mock.call_args.args == (ret2,)
+
+        # Spaces around bullet and text
+        paste_mock.return_value = "   • Test\n  •\tTest   •"
+        ret3 = pc.bullettopar()
+        assert ret3 == "Test Test"
+        assert copy_mock.call_args.args == (ret3,)
 
         # Bullets within words
         paste_mock.return_value = "•   Te•st• Test"
-        ret = pc.bullettopar()
-        assert ret == "Te st Test"
-        assert copy_mock.call_args.args == (ret,)
+        ret4 = pc.bullettopar()
+        assert ret4 == "Te st Test"
+        assert copy_mock.call_args.args == (ret4,)
 
         # Text from argument
-        ret = pc.bullettopar("•Another\n•Test")
-        assert ret == "Another Test"
-        assert copy_mock.call_args.args == (ret,)
+        ret5 = pc.bullettopar("•Another\n•Test")
+        assert ret5 == "Another Test"
+        assert copy_mock.call_args.args == (ret5,)
 
 
 def test_simplequote():
     with patch("pyperclip.copy") as copy_mock, patch("pyperclip.paste") as paste_mock:
+        # Bad type
+        paste_mock.return_value = 77
+        with pytest.raises(ValueError):
+            ret = pc.simplequote()
+
         # Argument from clipboard
         paste_mock.return_value = 'Test test'
         ret = pc.simplequote()
         assert ret == '"Test test"'
         assert copy_mock.call_args.args == (ret,)
 
         # Text from argument
@@ -97,14 +136,19 @@
         assert ret == '"Another test"'
         assert copy_mock.call_args.args == (ret,)
 
 
 # TODO: check ValueErrors
 def test_quote():
     with patch("pyperclip.copy") as copy_mock, patch("pyperclip.paste") as paste_mock:
+        # Bad type
+        paste_mock.return_value = 77
+        with pytest.raises(ValueError):
+            ret = pc.quote()
+
         # No arguments
         paste_mock.return_value = 'Test test'
         ret = pc.quote()
         assert ret == '"Test test,"'
         assert copy_mock.call_args.args == (ret,)
 
         # Punctuation argument
@@ -121,27 +165,54 @@
         # Text and punctuation argument
         ret = pc.quote('!', 'Another test')
         assert ret == '"Another test!"'
         assert copy_mock.call_args.args == (ret,)
 
         # Incorrect punctuation argument
         paste_mock.return_value = 'Test test'
-        try:
+        with pytest.raises(ValueError):
             ret = pc.quote('test')
-            assert True == False  # noqa E712
-        except ValueError:
-            assert len('test') > 1
+        assert len('test') > 1
 
         # Incorrect punctuation argument
         paste_mock.return_value = 'Test test'
-        try:
+        with pytest.raises(ValueError):
             ret = pc.quote(';')
-            assert True == False  # noqa E712
-        except ValueError:
-            assert ';' not in [',', '.', '!', '?']
+        assert ';' not in [',', '.', '!', '?']
+
+
+def test_trimspacing():
+    with patch("pyperclip.copy") as copy_mock, patch("pyperclip.paste") as paste_mock:
+        # Bad type
+        paste_mock.return_value = 77
+        with pytest.raises(ValueError):
+            ret = pc.trimspacing()
+
+        # multi-line break
+        paste_mock.return_value = "Test\n\n\nhere"
+        ret = pc.trimspacing()
+        assert ret == "Test\nhere"
+        assert copy_mock.call_args.args == (ret,)
+
+        # windows
+        paste_mock.return_value = "Test\r\n\r\nhere"
+        ret = pc.trimspacing()
+        assert ret == "Test\nhere"
+        assert copy_mock.call_args.args == (ret,)
+
+        # no repeats, spacing at beginning or end
+        paste_mock.return_value = "   Test\nhere\n"
+        ret = pc.trimspacing()
+        assert ret == "Test\nhere"
+        assert copy_mock.call_args.args == (ret,)
+
+        # text from argument
+        ret = pc.trimspacing("Another\r\n\r\n\r\ntest")
+        assert ret == "Another\ntest"
+        assert copy_mock.call_args.args == (ret,)
 
 
 # TODO: check that HTTPError is printed in Test 4
 def test_getservice():
     with patch("os.path.exists") as os_mock, patch(
         "google.oauth2.credentials.Credentials.from_authorized_user_file"
     ) as creds_file_mock, patch(
@@ -164,15 +235,15 @@
         fakecreds1 = MagicMock()
         fakecreds1.valid = True
         creds_file_mock.return_value = fakecreds1
         # build service
         fakeservice1 = MagicMock()
         build_mock.return_value = fakeservice1  # FIXME there was an issue here
 
-        ret = getservice('1yxH3v4zi82pEMKW41MbZRqKz8JXRbhrb5yJnEdSfJC0')
+        ret = pc._getservice('1yxH3v4zi82pEMKW41MbZRqKz8JXRbhrb5yJnEdSfJC0')
 
         assert os_mock.call_count == 1
         assert creds_file_mock.call_count == 1
         assert build_mock.call_args.args == (
             'docs',
             'v1',
         )
@@ -195,15 +266,15 @@
         # save refreshed creds
         faketoken2 = MagicMock()
         open_mock.return_value = faketoken2
         # build service
         fakeservice2 = MagicMock()
         build_mock.return_value = fakeservice2
 
-        ret = getservice('1yxH3v4zi82pEMKW41MbZRqKz8JXRbhrb5yJnEdSfJC0')
+        ret = pc._getservice('1yxH3v4zi82pEMKW41MbZRqKz8JXRbhrb5yJnEdSfJC0')
 
         assert os_mock.call_count == 1
         assert creds_file_mock.call_count == 2
         assert creds_file_mock.call_args.args == (
             '../token.json',
             SCOPES,
         )
@@ -229,15 +300,15 @@
         # save refreshed creds
         faketoken3 = MagicMock()
         open_mock.return_value = faketoken3
         # build service
         fakeservice3 = MagicMock()
         build_mock.return_value = fakeservice3
 
-        ret = getservice('1yxH3v4zi82pEMKW41MbZRqKz8JXRbhrb5yJnEdSfJC0', SCOPES)
+        ret = pc._getservice('1yxH3v4zi82pEMKW41MbZRqKz8JXRbhrb5yJnEdSfJC0', SCOPES)
 
         assert os_mock.call_count == 2
         assert get_secrets_mock.call_args.args == (
             '../credentials.json',
             SCOPES,
         )
         fakeflow3.run_local_server.assert_called_with(port=0)
@@ -262,15 +333,15 @@
         get_secrets_mock.return_value = fakeflow4
         # save refreshed creds
         faketoken4 = MagicMock()
         open_mock.return_value = faketoken4
         # raise error when building service
         build_mock.side_effect = HttpError(resp=MagicMock(), content=b'test')
 
-        ret = getservice('1yxH3v4zi82pEMKW41MbZRqKz8JXRbhrb5yJnEdSfJC0', SCOPES)
+        ret = pc._getservice('1yxH3v4zi82pEMKW41MbZRqKz8JXRbhrb5yJnEdSfJC0', SCOPES)
 
         assert os_remove_mock.call_count == 1
         assert os_mock.call_count == 2
         assert get_secrets_mock.call_args.args == (
             '../credentials.json',
             SCOPES,
         )
@@ -281,19 +352,107 @@
             'docs',
             'v1',
         )
         assert build_mock.call_args.kwargs == {'credentials': fakecreds4}
         print_mock.assert_called()
 
 
+# TODO implement test
+def test_smartcopy():
+    with patch("pyperclip.copy") as copy_mock, patch("pyperclip.paste") as paste_mock, patch(
+        "prettycopy.prettycopy.trimspacing"
+    ) as trim_mock, patch("nltk.tokenize.sent_tokenize") as tokenize_mock, patch(
+        "prettycopy.prettycopy._cleanlines"
+    ) as cleanlines_mock:
+        # Bad type
+        paste_mock.return_value = 77
+        with pytest.raises(ValueError):
+            pc.smartcopy()
+
+        # no newlines in the text
+        paste_mock.return_value = "lorem ipsum"
+        trim_mock.return_value = "Sentence one. Sentence two."
+        tokenize_mock.return_value = ["Sentence one.", "Sentence two."]
+        cleanlines_mock.side_effect = ["Sentence one.", "Sentence two."]
+        ret = pc.smartcopy()
+        assert ret == "Sentence one. Sentence two."
+        assert copy_mock.call_args.args == (ret,)
+
+        # newlines
+        paste_mock.return_value = "lorem ipsum"
+        trim_mock.return_value = "Sentence one.\n Sentence two."
+        tokenize_mock.return_value = ["Sentence one.", "Sentence two."]
+        cleanlines_mock.side_effect = ["Sentence one.", "Sentence two."]
+        ret = pc.smartcopy()
+        assert ret == "Sentence one.\nSentence two."
+        assert copy_mock.call_args.args == (ret,)
+
+        # text from argument
+        trim_mock.return_value = "Sentence one.\n Sentence two."
+        tokenize_mock.return_value = ["Sentence one.", "Sentence two."]
+        cleanlines_mock.side_effect = ["Sentence one.", "Sentence two."]
+        ret = pc.smartcopy("Sentence one.\n Sentence two.")
+        assert ret == "Sentence one.\nSentence two."
+        assert copy_mock.call_args.args == (ret,)
+
+        assert True
+
+
+# TODO implement test
+def test_cleanlines():
+    with patch("spellchecker.SpellChecker") as spellchecker_mock, patch("textblob.TextBlob") as textblob_mock, patch(
+        "nltk.corpus.words"
+    ) as words_mock:
+        # no space needed
+        spell = MagicMock()
+        spellchecker_mock.return_value = spell
+        spell.correction = MagicMock()
+        spell.correction.side_effect = ["sent", "nice", "go", "is"]
+        b1 = MagicMock()
+        b1.correct = MagicMock()
+        b2 = MagicMock()
+        b2.correct = MagicMock()
+        textblob_mock.side_effect = [b1, b2]
+        b1.correct.side_effect = ["sent", "go"]
+        b2.correct.side_effect = ["nice", "is"]
+        words_mock.return_value = False
+        line = "Sente\nnce 1 goe\ns here."
+        ret = pc._cleanlines(line)
+        assert ret == "Sentence 1 goes here."
+
+        # space needed
+        spell = MagicMock()
+        spellchecker_mock.return_value = spell
+        spell.correction = MagicMock()
+        spell.correction.side_effect = ["goes", "here"]
+        b1 = MagicMock()
+        b1.correct = MagicMock()
+        b2 = MagicMock()
+        b2.correct = MagicMock()
+        textblob_mock.side_effect = [b1, b2]
+        b1.correct.side_effect = ["goes"]
+        b2.correct.side_effect = ["here"]
+        words_mock.return_value = False
+        line = "Sentence 2 goes\nhere."
+        ret = pc._cleanlines(line)
+        assert ret == "Sentence 2 goes here."
+
+        # newline not within a word
+        line = "Sentence 3 goes \nhere."
+        ret = pc._cleanlines(line)
+        assert ret == "Sentence 3 goes here."
+
+        assert True
+
+
 # TODO: test for prettycopy.betterbullets
 # def test_betterbullets():
 #     with patch("prettycopy.nobullets") as nobullets_mock:
 #         nobullets_mock.return_value = "Test\ncontent\nhere"
-#         service = getservice()
+#         service = pc._getservice()
 
 #         # find end of current google doc content
 #         document = service.documents().get(documentId="1yxH3v4zi82pEMKW41MbZRqKz8JXRbhrb5yJnEdSfJC0").execute()
 #         doclines = document.get('body')['content']
 #         content = ""
 #         for line in doclines[1:]:
 #             content += line['paragraph']['elements'][0]['textRun']['content']
```

### Comparing `prettycopy-0.1.2/prettycopy.egg-info/PKG-INFO` & `prettycopy-0.1.3/prettycopy.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prettycopy
-Version: 0.1.2
+Version: 0.1.3
 Summary: A better copy-paster
 Author-email: Adi Gal <adigal03@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -267,8 +267,14 @@
 
 `prettycopy.quote(optional_end_punctuation, optional_text)`: Adds quotation marks around the text, ending in a punctuation mark. The default is a comma.
 
 > Example: *this is a test* --> prettycopy.quote() --> *"this is a test,"*
 
 > Example: *this is a test* --> prettycopy.quote('!') --> *"this is a test!"*
 
+`prettycopy.trimspacing(optional_text)`: Removes empty lines.
+
+`prettycopy.smartcopy(optional_text)`: Removes line breaks in an intelligent manner: adding spaces between words, but not inside words that have been split.
+
+> Example: *this\nis a te\nst* --> prettycopy.smartcopy() --> *this is a test*
+
 `prettycopy.betterbullets(docID)`: If you enter the document ID of an editable Google Doc (the long string of letters and numbers in the URL), this function will copy the text in your clipboard to the end of the document, replacing all bullet symbols (•) with correctly-formatted bullet points. Still under construction.
```

### Comparing `prettycopy-0.1.2/prettycopy.egg-info/SOURCES.txt` & `prettycopy-0.1.3/prettycopy.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -9,18 +9,18 @@
 setup.py
 docs/Makefile
 docs/conf.py
 docs/dev_intro.md
 docs/index.md
 docs/make.bat
 docs/requirements.txt
+docs/images/bullettopar.gif
 prettycopy/__init__.py
 prettycopy/__main__.py
 prettycopy/_version.py
-prettycopy/gdocs.py
 prettycopy/prettycopy.py
 prettycopy.egg-info/PKG-INFO
 prettycopy.egg-info/SOURCES.txt
 prettycopy.egg-info/dependency_links.txt
 prettycopy.egg-info/requires.txt
 prettycopy.egg-info/top_level.txt
 prettycopy/tests/test_all.py
```

### Comparing `prettycopy-0.1.2/pyproject.toml` & `prettycopy-0.1.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -7,22 +7,25 @@
 build-backend="setuptools.build_meta"
 
 [project]
 name = "prettycopy"
 authors = [{name = "Adi Gal", email = "adigal03@gmail.com"}]
 description="A better copy-paster"
 readme = "README.md"
-version = "0.1.2"
+version = "0.1.3"
 requires-python = ">=3.7"
 
 dependencies = [
     "pyperclip",
     "google-auth-oauthlib",
     "google-auth",
     "google-api-python-client",
+    "nltk",
+    "textblob",
+    "pyspellchecker",
 ]
 
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
     "Programming Language :: Python :: 3",
```

