# Comparing `tmp/pylibacl-0.6.0.tar.gz` & `tmp/pylibacl-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylibacl-0.6.0.tar", last modified: Sun Nov 29 01:44:24 2020, max compression
+gzip compressed data, was "pylibacl-0.7.0.tar", last modified: Sun Apr 23 20:19:45 2023, max compression
```

## Comparing `pylibacl-0.6.0.tar` & `pylibacl-0.7.0.tar`

### file list

```diff
@@ -1,25 +1,30 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-11-29 01:44:24.751806 pylibacl-0.6.0/
--rw-r--r--   0 root         (0) root         (0)    26436 2012-05-12 11:29:27.000000 pylibacl-0.6.0/COPYING
--rw-r--r--   0 root         (0) root         (0)      191 2019-11-29 18:21:02.000000 pylibacl-0.6.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2115 2020-11-29 01:41:29.000000 pylibacl-0.6.0/Makefile
--rw-r--r--   0 root         (0) root         (0)     5945 2020-11-29 01:39:49.000000 pylibacl-0.6.0/NEWS
--rw-r--r--   0 root         (0) root         (0)     1088 2020-11-29 01:44:24.751806 pylibacl-0.6.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3057 2020-11-29 01:41:40.000000 pylibacl-0.6.0/README.md
--rw-r--r--   0 root         (0) root         (0)    59684 2020-06-19 22:49:21.000000 pylibacl-0.6.0/acl.c
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-11-29 01:44:24.751806 pylibacl-0.6.0/doc/
--rw-r--r--   0 root         (0) root         (0)     8197 2020-11-29 01:42:29.000000 pylibacl-0.6.0/doc/conf.py
--rw-r--r--   0 root         (0) root         (0)     3985 2012-05-13 01:44:03.000000 pylibacl-0.6.0/doc/implementation.rst
--rw-r--r--   0 root         (0) root         (0)      351 2019-11-29 19:03:02.000000 pylibacl-0.6.0/doc/index.rst
--rw-r--r--   0 root         (0) root         (0)       57 2012-05-13 02:07:41.000000 pylibacl-0.6.0/doc/module.rst
--rw-r--r--   0 root         (0) root         (0)     2151 2019-11-29 18:54:18.000000 pylibacl-0.6.0/posix1e.pyi
--rw-r--r--   0 root         (0) root         (0)        0 2019-11-29 16:21:35.000000 pylibacl-0.6.0/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-11-29 01:44:24.751806 pylibacl-0.6.0/pylibacl.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1088 2020-11-29 01:44:24.000000 pylibacl-0.6.0/pylibacl.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      331 2020-11-29 01:44:24.000000 pylibacl-0.6.0/pylibacl.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2020-11-29 01:44:24.000000 pylibacl-0.6.0/pylibacl.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2019-11-29 16:29:38.000000 pylibacl-0.6.0/pylibacl.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)        8 2020-11-29 01:44:24.000000 pylibacl-0.6.0/pylibacl.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       81 2020-11-29 01:44:24.751806 pylibacl-0.6.0/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)     2418 2020-11-29 01:40:33.000000 pylibacl-0.6.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-11-29 01:44:24.751806 pylibacl-0.6.0/tests/
--rw-r--r--   0 root         (0) root         (0)    32403 2019-12-16 23:45:59.000000 pylibacl-0.6.0/tests/test_acls.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 20:19:45.971453 pylibacl-0.7.0/
+-rw-r--r--   0 root         (0) root         (0)    26436 2012-05-12 11:29:27.000000 pylibacl-0.7.0/COPYING
+-rw-r--r--   0 root         (0) root         (0)      231 2023-04-22 21:16:17.000000 pylibacl-0.7.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1975 2023-04-23 20:06:01.000000 pylibacl-0.7.0/Makefile
+-rw-r--r--   0 root         (0) root         (0)     6376 2023-04-23 20:16:22.000000 pylibacl-0.7.0/NEWS.md
+-rw-r--r--   0 root         (0) root         (0)     1064 2023-04-23 20:19:45.974786 pylibacl-0.7.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3312 2023-04-23 20:16:34.000000 pylibacl-0.7.0/README.md
+-rw-r--r--   0 root         (0) root         (0)      648 2023-04-16 19:23:22.000000 pylibacl-0.7.0/SECURITY.md
+-rw-r--r--   0 root         (0) root         (0)    57491 2023-04-22 20:55:38.000000 pylibacl-0.7.0/acl.c
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 20:19:45.971453 pylibacl-0.7.0/doc/
+-rw-r--r--   0 root         (0) root         (0)     8014 2023-04-23 20:06:38.000000 pylibacl-0.7.0/doc/conf.py
+-rw-r--r--   0 root         (0) root         (0)     2192 2023-04-23 20:11:13.000000 pylibacl-0.7.0/doc/contributing.md
+-rw-r--r--   0 root         (0) root         (0)     3985 2012-05-13 01:44:03.000000 pylibacl-0.7.0/doc/implementation.rst
+-rw-r--r--   0 root         (0) root         (0)      384 2023-04-23 20:13:57.000000 pylibacl-0.7.0/doc/index.rst
+-rw-r--r--   0 root         (0) root         (0)       57 2012-05-13 02:07:41.000000 pylibacl-0.7.0/doc/module.rst
+-rw-r--r--   0 root         (0) root         (0)     6376 2023-04-23 20:16:22.000000 pylibacl-0.7.0/doc/news.md
+-rw-r--r--   0 root         (0) root         (0)     3312 2023-04-23 20:16:34.000000 pylibacl-0.7.0/doc/readme.md
+-rw-r--r--   0 root         (0) root         (0)      648 2023-04-16 19:23:22.000000 pylibacl-0.7.0/doc/security.md
+-rw-r--r--   0 root         (0) root         (0)     2151 2019-11-29 18:54:18.000000 pylibacl-0.7.0/posix1e.pyi
+-rw-r--r--   0 root         (0) root         (0)        0 2019-11-29 16:21:35.000000 pylibacl-0.7.0/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 20:19:45.971453 pylibacl-0.7.0/pylibacl.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1064 2023-04-23 20:19:45.000000 pylibacl-0.7.0/pylibacl.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      408 2023-04-23 20:19:45.000000 pylibacl-0.7.0/pylibacl.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-23 20:19:45.000000 pylibacl-0.7.0/pylibacl.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2019-11-29 16:29:38.000000 pylibacl-0.7.0/pylibacl.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)        8 2023-04-23 20:19:45.000000 pylibacl-0.7.0/pylibacl.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       81 2023-04-23 20:19:45.974786 pylibacl-0.7.0/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)     2418 2023-04-23 20:06:24.000000 pylibacl-0.7.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-23 20:19:45.971453 pylibacl-0.7.0/tests/
+-rw-r--r--   0 root         (0) root         (0)    34040 2023-04-22 00:15:30.000000 pylibacl-0.7.0/tests/test_acls.py
```

### Comparing `pylibacl-0.6.0/COPYING` & `pylibacl-0.7.0/COPYING`

 * *Files identical despite different names*

### Comparing `pylibacl-0.6.0/Makefile` & `pylibacl-0.7.0/Makefile`

 * *Files 5% similar despite different names*

```diff
@@ -1,52 +1,46 @@
 PYTHON        = python3
 SPHINXOPTS    = -W
 SPHINXBUILD   = $(PYTHON) -m sphinx
 DOCDIR        = doc
 DOCHTML       = $(DOCDIR)/html
 DOCTREES      = $(DOCDIR)/doctrees
 ALLSPHINXOPTS = -d $(DOCTREES) $(SPHINXOPTS) $(DOCDIR)
-VERSION       = 0.6.0
+VERSION       = 0.7.0
 FULLVER       = pylibacl-$(VERSION)
 DISTFILE      = $(FULLVER).tar.gz
 
 MODNAME = posix1e.so
-RSTFILES = doc/index.rst doc/module.rst doc/news.rst doc/readme.md doc/conf.py
+DOCFILES = doc/index.rst doc/module.rst doc/news.md doc/readme.md doc/conf.py
 
 all: doc test
 
 $(MODNAME): acl.c
 	$(PYTHON) ./setup.py build_ext --inplace
 
-$(DOCHTML)/index.html: $(MODNAME) $(RSTFILES) acl.c
+$(DOCHTML)/index.html: $(MODNAME) $(DOCFILES) acl.c
 	$(SPHINXBUILD) -b html $(ALLSPHINXOPTS) $(DOCHTML)
 	touch $@
 
 doc: $(DOCHTML)/index.html
 
-doc/readme.md: README.md
-	ln -s ../README.md doc/readme.md
-
-doc/news.rst: NEWS
-	ln -s ../NEWS doc/news.rst
-
 dist:
 	fakeroot $(PYTHON) ./setup.py sdist
 
 distcheck: dist
 	set -e; \
 	TDIR=$$(mktemp -d) && \
 	trap "rm -rf $$TDIR" EXIT; \
 	tar xzf dist/$(DISTFILE) -C $$TDIR && \
 	(cd $$TDIR/$(FULLVER) && make doc && make test && make dist) && \
 	echo "All good, you can upload $(DISTFILE)!"
 
 test:
 	@set -e; \
-	for ver in 3.4 3.5 3.6 3.7 3.8 3.9; do \
+	for ver in 3.7 3.8 3.9 3.10 3.11 3.12; do \
 	  for flavour in "" "-dbg"; do \
 	    if type python$$ver$$flavour >/dev/null; then \
 	      echo Testing with python$$ver$$flavour; \
 	      python$$ver$$flavour ./setup.py build_ext -i; \
 	      python$$ver$$flavour -m pytest tests ;\
 	    fi; \
 	  done; \
@@ -72,15 +66,14 @@
 	$(MAKE) clean
 	$(MAKE) test CFLAGS="-coverage"
 	lcov --capture --no-external --directory . --output-file coverage.info
 	genhtml coverage.info --output-directory out
 
 clean:
 	rm -rf $(DOCHTML) $(DOCTREES)
-	rm -f doc/readme.md doc/news.rst
 	rm -f $(MODNAME)
 	rm -f *.so
 	rm -rf build
 
 types:
 	MYPYPATH=. mypy --check-untyped-defs --warn-incomplete-stub tests/test_acls.py
```

### Comparing `pylibacl-0.6.0/NEWS` & `pylibacl-0.7.0/NEWS.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,29 @@
-News
-====
+# News
 
-Version 0.6.0
--------------
+## Version 0.7.0
 
-*Sun, 29 Nov 2020*
+*released Sun, 23 Apr 2023*
+
+Important: Python 3.7 is the minimum supported version, due to
+difficulty of testing old releases, and the fact that everything older
+has been deprecated a long time ago (e.g. 3.6 at the end of 2021).
+
+Otherwise, a minor release:
+
+- Improve error handling in some corner cases (not expected to have
+  any real-life impact, but who knows).
+- Improved testing coverage and test infrastructure.
+- Modernise parts of the C code based on recent Python version
+  guidelines.
+- Add a simple security policy and contribution guidelines.
+
+## Version 0.6.0
+
+*released Sun, 29 Nov 2020*
 
 Major release removing Python 2 support. This allow both code cleanup
 and new features, such as:
 
 - Support for pathlib objects in `apply_to` and `has_extended`
   functions when running with Python 3.6 and newer.
 - Use of built-in C API functions for bytes/unicode/pathlib conversion
@@ -48,16 +63,15 @@
   which should simplify some uses cases (`a = ACL(); a.__set
   state__(…)`).
 - When available, add the file path to I/O error messages, which should
   lead to easier debugging.
 - The test suite has changed to `pytest`, which allows increased
   coverage via parameterisation.
 
-Version 0.5.4
--------------
+## Version 0.5.4
 
 *released Thu, 14 Nov 2019*
 
 Maintenance release:
 
 - Switch build system to Python 3 by default (can be overridden if
   needed).
@@ -65,36 +79,33 @@
 - Fix compatibility with PyPy.
 - Test improvements (both local and on Travis), testing more variations
   (debug, PyPy).
 - Improve test coverage, and allow gathering test coverage results.
 - Drop support (well, drop testing) for Python lower than 2.7.
 - Minor documentation improvements (closes #9, #12).
 
-Version 0.5.3
--------------
+## Version 0.5.3
 
 *released Thu, 30 Apr 2015*
 
 FreeBSD fixes:
 
 - Enable all FreeBSD versions after 7.x at level 2 (thanks to Garrett
   Cooper).
 - Make test suite pass under FreeBSD, which has a stricter behaviour
   with regards to invalid ACLs (which we do exercise in the test suite),
   thanks again to Garret for the bug reports.
 
-Version 0.5.2
--------------
+## Version 0.5.2
 
 *released Sat, 24 May 2014*
 
 No visible changes release: just fix tests when running under pypy.
 
-Version 0.5.1
--------------
+## Version 0.5.1
 
 *released Sun, 13 May 2012*
 
 A bug-fix only release. Critical bugs (memory leaks and possible
 segmentation faults) have been fixed thanks to Dave Malcolm and his
 ``cpychecker`` tool. Additionally, some compatibility issues with Python
 3.x have been fixed (str() methods returning bytes).
@@ -102,91 +113,79 @@
 The documentation has been improved and changed from epydoc to sphinx;
 note however that the documentation is still auto-generated from the
 docstrings.
 
 Project reorganisation: the project home page has been moved from
 SourceForge to GitHub.
 
-Version 0.5
------------
+## Version 0.5
 
 *released Sun, 27 Dec 2009*
 
 Added support for Python 3.x and improved support for Unicode filenames.
 
-Version 0.4
------------
+## Version 0.4
 
 *released Sat, 28 Jun 2008*
 
-License
-~~~~~~~
+### License
+
 
 Starting with this version, pylibacl is licensed under LGPL 2.1,
 Febryary 1999 or any later versions (see README.rst and COPYING).
 
-Linux support
-~~~~~~~~~~~~~
+### Linux support
 
 A few more Linux-specific functions:
 
 - add the ACL.equiv_mode() method, which will return the equivalent
   octal mode if this is a basic ACL and raise an IOError exception
   otherwise
 
 - add the acl_extended(...) function, which will check if an fd or path
   has an extended ACL
 
-FreeBSD support
-~~~~~~~~~~~~~~~
+### FreeBSD support
 
 FreeBSD 7.x will have almost all the acl manipulation functions that
 Linux has, with the exception of __getstate__/__setstate__. As a
 workaround, use the str() and ACL(text=...) methods to pass around
 textual representations.
 
-Interface
-~~~~~~~~~
+### Interface
 
 At module level there are now a few constants exported for easy-checking
 at runtime what features have been compiled in:
 
-- HAS_ACL_FROM_MODE, denoting whether the ACL constructor supports the
-  mode=0xxx parameter
+- `HAS_ACL_FROM_MODE`, denoting whether the ACL constructor supports
+  the `mode=0xxx` parameter
 
-- HAS_ACL_CHECK, denoting whether ACL instances support the check()
-  method
+- `HAS_ACL_CHECK`, denoting whether ACL instances support the
+  `check()` method
 
-- HAS_ACL_ENTRY, denoting whether ACL manipulation is possible and the
-  Entry and Permset classes are available
+- `HAS_ACL_ENTRY`, denoting whether ACL manipulation is possible and
+  the Entry and Permset classes are available
 
-- HAS_EXTENEDED_CHECK, denoting whether the acl_extended function is
-  supported
+- `HAS_EXTENEDED_CHECK`, denoting whether the `acl_extended()`
+  function is supported
 
-- HAS_EQUIV_MODE, denoting whether ACL instances support the
-  equiv_mode() method
+- `HAS_EQUIV_MODE`, denoting whether ACL instances support the
+  `equiv_mode()` method
 
-Internals
-~~~~~~~~~
+### Internals
 
 Many functions have now unittests, which is a good thing.
 
 
-Version 0.3
------------
+## Version 0.3
 
 *released Sun, 21 Oct 2007*
 
-Linux support
-~~~~~~~~~~~~~
+### Linux support
 
 Under Linux, implement more functions from libacl:
 
-- add ACL(mode=...), implementing acl_from_mode
-- add ACL().to_any_text, implementing acl_to_any_text
-- add ACL comparison, using acl_cmp
-- add ACL().check, which is a more descriptive function than validate
-
-.. Local Variables:
-.. mode: rst
-.. fill-column: 72
-.. End:
+- add `ACL(mode=...)`, implementing `acl_from_mode`.
+- add `ACL.to_any_text()`, implementing `acl_to_any_text`.
+- add ACL comparison, using `acl_cmp`.
+- add `ACL.check()`, which is a more descriptive function than
+  validate.
```

### Comparing `pylibacl-0.6.0/PKG-INFO` & `pylibacl-0.7.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,25 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: pylibacl
-Version: 0.6.0
+Version: 0.7.0
 Summary: POSIX.1e ACLs for python
 Home-page: https://pylibacl.k1024.org/
 Author: Iustin Pop
 Author-email: iustin@k1024.org
 License: LGPL
 Project-URL: Bug Tracker, https://github.com/iustin/pylibacl/issues
-Description: This is a C extension module for Python which
-        implements POSIX ACLs manipulation. It is a wrapper on top
-        of the systems's acl C library - see acl(5).
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Operating System :: POSIX :: BSD :: FreeBSD
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Filesystems
-Requires-Python: >=3.4
+Requires-Python: >=3.7
+License-File: COPYING
+
+This is a C extension module for Python which
+implements POSIX ACLs manipulation. It is a wrapper on top
+of the systems's acl C library - see acl(5).
```

### Comparing `pylibacl-0.6.0/README.md` & `pylibacl-0.7.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 # pylibacl
 
-This is a Python 3.4+ extension module allows you to manipulate the
+This is a Python 3.7+ extension module allows you to manipulate the
 POSIX.1e Access Control Lists present in some OS/file-systems
 combinations.
 
-Downloads: go to <http://pylibacl.k1024.org/downloads>. Latest version
-is 0.6.0. The source repository is either at
+Downloads: go to <https://pylibacl.k1024.org/downloads>. Latest
+version is 0.7.0. The source repository is either at
 <https://git.k1024.org/pylibacl.git> or at
 <https://github.com/iustin/pylibacl>.
 
 For any issues, please file bugs at
 <https://github.com/iustin/pylibacl/issues>.
 
-[![Travis](https://img.shields.io/travis/iustin/pylibacl)](https://travis-ci.org/iustin/pylibacl)
+See the `CONTRIBUTING.md` file for details on how to contribute.
+
+[![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/iustin/pylibacl/ci.yml?branch=main)](https://github.com/iustin/pylibacl/actions/workflows/ci.yml)
 [![Codecov](https://img.shields.io/codecov/c/github/iustin/pylibacl)](https://codecov.io/gh/iustin/pylibacl)
 [![Read the Docs](https://img.shields.io/readthedocs/pylibacl)](http://pylibacl.readthedocs.io/en/latest/?badge=latest)
 [![GitHub issues](https://img.shields.io/github/issues/iustin/pylibacl)](https://github.com/iustin/pylibacl/issues)
 ![GitHub tag (latest by date)](https://img.shields.io/github/v/tag/iustin/pylibacl)
 [![GitHub release (latest by date)](https://img.shields.io/github/v/release/iustin/pylibacl)](https://github.com/iustin/pylibacl/releases)
 [![PyPI](https://img.shields.io/pypi/v/pylibacl)](https://pypi.org/project/pylibacl/)
 ![Debian package](https://img.shields.io/debian/v/python-pylibacl)
@@ -29,15 +31,16 @@
 
 pylibacl has been written and tested on Linux, kernel v2.4 or newer,
 with XFS filesystems; ext2/ext3 should also work. Since release 0.4.0,
 FreeBSD 7 also has quite good support. If any other platform
 implements the POSIX.1e draft, pylibacl can be used. I heard that
 Solaris does, but I can't test it.
 
-- Python 3.4 or newer. Python 2.4+ was supported in the 0.5.x branch.
+- Python 3.7 or newer. Python 2.4+ was supported in the 0.5.x branch,
+  Python 3.4+ in the 0.6 branch.
 - Operating system:
     - Linux, kernel v2.4 or newer, and the libacl library and
       development packages (all modern distributions should have this,
       under various names); also the file-systems you use must have
       ACLs turned on, either as a compile or mount option.
     - FreeBSD 7.0 or newer.
 - The sphinx python module, for your python version, if building the
@@ -51,17 +54,19 @@
 
 - `pkg install py36-setuptools py36-sphinx`
 
 or:
 
 - `pkg install py37-setuptools`
 
+## Security
+
+For reporting security vulnerabilities, please see `SECURITY.md`.
 
-License
--------
+## License
 
 pylibacl is Copyright (C) 2002-2009, 2012, 2014, 2015 Iustin Pop.
 
 pylibacl is free software; you can redistribute it and/or modify it under the
 terms of the GNU Lesser General Public License as published by the Free
 Software Foundation; either version 2.1 of the License, or (at your option) any
 later version. See the COPYING file for the full license terms.
```

### Comparing `pylibacl-0.6.0/acl.c` & `pylibacl-0.7.0/acl.c`

 * *Files 4% similar despite different names*

```diff
@@ -112,17 +112,19 @@
     if(newacl == NULL) {
         return NULL;
     }
     acl = (ACL_Object*) newacl;
 
     acl->acl = acl_init(0);
     if (acl->acl == NULL) {
+        /* LCOV_EXCL_START */
         PyErr_SetFromErrno(PyExc_IOError);
         Py_DECREF(newacl);
         return NULL;
+        /* LCOV_EXCL_STOP */
     }
 #ifdef HAVE_LEVEL2
     acl->entry_id = ACL_FIRST_ENTRY;
 #endif
 
     return newacl;
 }
@@ -239,39 +241,40 @@
     return 0;
 }
 
 /* Standard type functions */
 static void ACL_dealloc(PyObject* obj) {
     ACL_Object *self = (ACL_Object*) obj;
     PyObject *err_type, *err_value, *err_traceback;
-    int have_error = PyErr_Occurred() ? 1 : 0;
 
-    if (have_error)
-        PyErr_Fetch(&err_type, &err_value, &err_traceback);
+    PyErr_Fetch(&err_type, &err_value, &err_traceback);
     if(self->acl != NULL && acl_free(self->acl) != 0)
-        PyErr_WriteUnraisable(obj);
-    if (have_error)
-        PyErr_Restore(err_type, err_value, err_traceback);
-    PyObject_DEL(self);
+        PyErr_WriteUnraisable(obj);  /* LCOV_EXCL_LINE */
+    PyErr_Restore(err_type, err_value, err_traceback);
+    Py_TYPE(obj)->tp_free(obj);
 }
 
 /* Converts the acl to a text format */
 static PyObject* ACL_str(PyObject *obj) {
     char *text;
     ACL_Object *self = (ACL_Object*) obj;
     PyObject *ret;
 
     text = acl_to_text(self->acl, NULL);
     if(text == NULL) {
+        /* LCOV_EXCL_START */
         return PyErr_SetFromErrno(PyExc_IOError);
+        /* LCOV_EXCL_STOP */
     }
     ret = PyUnicode_FromString(text);
     if(acl_free(text) != 0) {
+        /* LCOV_EXCL_START */
         Py_XDECREF(ret);
         return PyErr_SetFromErrno(PyExc_IOError);
+        /* LCOV_EXCL_STOP */
     }
     return ret;
 }
 
 #ifdef HAVE_LINUX
 static char __to_any_text_doc__[] =
   "to_any_text([prefix='', separator='n', options=0])\n"
@@ -313,20 +316,22 @@
 
     if (!PyArg_ParseTupleAndKeywords(args, kwds, "|sci", kwlist, &arg_prefix,
                                      &arg_separator, &arg_options))
       return NULL;
 
     text = acl_to_any_text(self->acl, arg_prefix, arg_separator, arg_options);
     if(text == NULL) {
-        return PyErr_SetFromErrno(PyExc_IOError);
+        return PyErr_SetFromErrno(PyExc_IOError);  /* LCOV_EXCL_LINE */
     }
     ret = PyBytes_FromString(text);
     if(acl_free(text) != 0) {
+        /* LCOV_EXCL_START */
         Py_XDECREF(ret);
         return PyErr_SetFromErrno(PyExc_IOError);
+        /* LCOV_EXCL_STOP */
     }
     return ret;
 }
 
 static char __check_doc__[] =
     "Check the ACL validity.\n"
     "\n"
@@ -353,15 +358,15 @@
 /* The acl_check method */
 static PyObject* ACL_check(PyObject* obj, PyObject* args) {
     ACL_Object *self = (ACL_Object*) obj;
     int result;
     int eindex;
 
     if((result = acl_check(self->acl, &eindex)) == -1)
-        return PyErr_SetFromErrno(PyExc_IOError);
+        return PyErr_SetFromErrno(PyExc_IOError);  /* LCOV_EXCL_LINE */
     if(result == 0) {
         Py_RETURN_FALSE;
     }
     return Py_BuildValue("(ii)", result, eindex);
 }
 
 /* Implementation of the rich compare for ACLs */
@@ -378,15 +383,15 @@
         PyErr_SetString(PyExc_TypeError, "can only compare to an ACL");
         return NULL;
     }
 
     acl1 = (ACL_Object*)o1;
     acl2 = (ACL_Object*)o2;
     if((n=acl_cmp(acl1->acl, acl2->acl))==-1)
-        return PyErr_SetFromErrno(PyExc_IOError);
+        return PyErr_SetFromErrno(PyExc_IOError);  /* LCOV_EXCL_LINE */
     switch(op) {
     case Py_EQ:
         ret = n == 0 ? Py_True : Py_False;
         break;
     case Py_NE:
         ret = n == 1 ? Py_True : Py_False;
         break;
@@ -411,15 +416,15 @@
 
 /* The acl_equiv_mode method */
 static PyObject* ACL_equiv_mode(PyObject* obj, PyObject* args) {
     ACL_Object *self = (ACL_Object*) obj;
     mode_t mode;
 
     if(acl_equiv_mode(self->acl, &mode) == -1)
-        return PyErr_SetFromErrno(PyExc_IOError);
+        return PyErr_SetFromErrno(PyExc_IOError);  /* LCOV_EXCL_LINE */
     return PyLong_FromLong(mode);
 }
 #endif
 
 /* Custom methods */
 static char __applyto_doc__[] =
     "applyto(item[, flag=ACL_TYPE_ACCESS])\n"
@@ -516,23 +521,25 @@
     ACL_Object *self = (ACL_Object*) obj;
     PyObject *ret;
     ssize_t size, nsize;
     char *buf;
 
     size = acl_size(self->acl);
     if(size == -1)
-        return PyErr_SetFromErrno(PyExc_IOError);
+        return PyErr_SetFromErrno(PyExc_IOError);  /* LCOV_EXCL_LINE */
 
     if((ret = PyBytes_FromStringAndSize(NULL, size)) == NULL)
         return NULL;
     buf = PyBytes_AsString(ret);
 
     if((nsize = acl_copy_ext(buf, self->acl, size)) == -1) {
+        /* LCOV_EXCL_START */
         Py_DECREF(ret);
         return PyErr_SetFromErrno(PyExc_IOError);
+        /* LCOV_EXCL_STOP */
     }
 
     return ret;
 }
 
 static PyObject* ACL_set_state(PyObject *obj, PyObject* args) {
     ACL_Object *self = (ACL_Object*) obj;
@@ -544,18 +551,21 @@
     if (!PyArg_ParseTuple(args, "y#", &buf, &bufsize))
         return NULL;
 
     /* Try to import the external representation */
     if((ptr = acl_copy_int(buf)) == NULL)
         return PyErr_SetFromErrno(PyExc_IOError);
 
-    /* Free the old acl. Should we ignore errors here? */
     if(self->acl != NULL) {
-        if(acl_free(self->acl) == -1)
-            return PyErr_SetFromErrno(PyExc_IOError);
+        /* Ignore errors in freeing the previous acl. We already
+           allocated the new acl, and the state of the previous one is
+           suspect if freeing failed (in Linux's libacl, deallocating
+           a valid ACL can't actually happen, so this path is
+           unlikely. */
+        acl_free(self->acl); /* LCOV_EXCL_LINE */
     }
 
     self->acl = ptr;
 
     Py_RETURN_NONE;
 }
 #endif
@@ -578,15 +588,15 @@
     acl_entry_t the_entry_t;
     Entry_Object *the_entry_obj;
     int nerr;
 
     nerr = acl_get_entry(self->acl, self->entry_id, &the_entry_t);
     self->entry_id = ACL_NEXT_ENTRY;
     if(nerr == -1)
-        return PyErr_SetFromErrno(PyExc_IOError);
+        return PyErr_SetFromErrno(PyExc_IOError);  /* LCOV_EXCL_LINE */
     else if(nerr == 0) {
         /* Docs says this is not needed */
         /*PyErr_SetObject(PyExc_StopIteration, Py_None);*/
         return NULL;
     }
 
     the_entry_obj = (Entry_Object*) PyType_GenericNew(&Entry_Type, NULL, NULL);
@@ -691,16 +701,18 @@
     if(newentry == NULL) {
         return NULL;
     }
 
     if(oldentry != NULL) {
         nret = acl_copy_entry(newentry->entry, oldentry->entry);
         if(nret == -1) {
+            /* LCOV_EXCL_START */
             Py_DECREF(newentry);
             return PyErr_SetFromErrno(PyExc_IOError);
+           /* LCOV_EXCL_STOP */
         }
     }
 
     return (PyObject*)newentry;
 }
 
 /***** Entry type *****/
@@ -727,21 +739,25 @@
    qualifier (if any) to either the uid or the gid entry in the
    tag_qual structure, and the return value is 0.
 */
 static int get_tag_qualifier(acl_entry_t entry, tag_qual *tq) {
     void *p;
 
     if(acl_get_tag_type(entry, &tq->tag) == -1) {
+        /* LCOV_EXCL_START */
         PyErr_SetFromErrno(PyExc_IOError);
         return -1;
+        /* LCOV_EXCL_STOP */
     }
     if (tq->tag == ACL_USER || tq->tag == ACL_GROUP) {
         if((p = acl_get_qualifier(entry)) == NULL) {
+            /* LCOV_EXCL_START */
             PyErr_SetFromErrno(PyExc_IOError);
             return -1;
+            /* LCOV_EXCL_STOP */
         }
         if (tq->tag == ACL_USER) {
             tq->uid = *(uid_t*)p;
         } else {
             tq->gid = *(gid_t*)p;
         }
         acl_free(p);
@@ -771,17 +787,19 @@
     if(newentry == NULL) {
         return NULL;
     }
 
     entry = (Entry_Object*)newentry;
 
     if(acl_create_entry(&parent->acl, &entry->entry) == -1) {
+        /* LCOV_EXCL_START */
         PyErr_SetFromErrno(PyExc_IOError);
         Py_DECREF(newentry);
         return NULL;
+        /* LCOV_EXCL_STOP */
     }
     Py_INCREF(parent);
     entry->parent_acl = (PyObject*)parent;
     return newentry;
 }
 
 /* Initialization of a new Entry instance */
@@ -800,25 +818,22 @@
     return 0;
 }
 
 /* Free the Entry instance */
 static void Entry_dealloc(PyObject* obj) {
     Entry_Object *self = (Entry_Object*) obj;
     PyObject *err_type, *err_value, *err_traceback;
-    int have_error = PyErr_Occurred() ? 1 : 0;
 
-    if (have_error)
-        PyErr_Fetch(&err_type, &err_value, &err_traceback);
+    PyErr_Fetch(&err_type, &err_value, &err_traceback);
     if(self->parent_acl != NULL) {
         Py_DECREF(self->parent_acl);
         self->parent_acl = NULL;
     }
-    if (have_error)
-        PyErr_Restore(err_type, err_value, err_traceback);
-    PyObject_DEL(self);
+    PyErr_Restore(err_type, err_value, err_traceback);
+    Py_TYPE(obj)->tp_free(obj);
 }
 
 /* Converts the entry to a text format */
 static PyObject* Entry_str(PyObject *obj) {
     PyObject *format, *kind;
     Entry_Object *self = (Entry_Object*) obj;
     tag_qual tq;
@@ -852,21 +867,24 @@
         break;
     case ACL_GROUP:
         kind = PyUnicode_FromFormat("group with gid %u", tq.gid);
         break;
     case ACL_MASK:
         kind = PyUnicode_FromString("the mask");
         break;
-    default:
+    default: /* LCOV_EXCL_START */
         kind = PyUnicode_FromString("UNKNOWN_TAG_TYPE!");
         break;
+        /* LCOV_EXCL_STOP */
     }
     if (kind == NULL) {
+        /* LCOV_EXCL_START */
         Py_DECREF(format);
         return NULL;
+        /* LCOV_EXCL_STOP */
     }
     PyObject *ret = PyUnicode_Concat(format, kind);
     Py_DECREF(format);
     Py_DECREF(kind);
     return ret;
 }
 
@@ -891,16 +909,18 @@
 
 /* Returns the tag type of the entry */
 static PyObject* Entry_get_tag_type(PyObject *obj, void* arg) {
     Entry_Object *self = (Entry_Object*) obj;
     acl_tag_t value;
 
     if(acl_get_tag_type(self->entry, &value) == -1) {
+        /* LCOV_EXCL_START */
         PyErr_SetFromErrno(PyExc_IOError);
         return NULL;
+        /* LCOV_EXCL_STOP */
     }
 
     return PyLong_FromLong(value);
 }
 
 /* Sets the qualifier (either uid_t or gid_t) for the entry,
  * usable only if the tag type if ACL_USER or ACL_GROUP
@@ -928,16 +948,18 @@
             return -1;
         }
     }
     /* Due to how acl_set_qualifier takes its argument, we have to do
        this ugly dance with two variables and a pointer that will
        point to one of them. */
     if(acl_get_tag_type(self->entry, &tag) == -1) {
+        /* LCOV_EXCL_START */
         PyErr_SetFromErrno(PyExc_IOError);
         return -1;
+        /* LCOV_EXCL_STOP */
     }
     uid = uidgid;
     gid = uidgid;
     /* This is an extra overflow check, in case uid_t/gid_t are
        int-sized (and int size smaller than long size). */
     switch(tag) {
     case ACL_USER:
@@ -958,16 +980,18 @@
       break;
     default:
       PyErr_SetString(PyExc_TypeError,
                       "Can only set qualifiers on ACL_USER or ACL_GROUP entries");
       return -1;
     }
     if(acl_set_qualifier(self->entry, p) == -1) {
+        /* LCOV_EXCL_START */
         PyErr_SetFromErrno(PyExc_IOError);
         return -1;
+        /* LCOV_EXCL_STOP */
     }
 
     return 0;
 }
 
 /* Returns the qualifier of the entry */
 static PyObject* Entry_get_qualifier(PyObject *obj, void* arg) {
@@ -1024,16 +1048,18 @@
 
     if(!PyObject_IsInstance(value, (PyObject*)&Permset_Type)) {
         PyErr_SetString(PyExc_TypeError, "argument 1 must be posix1e.Permset");
         return -1;
     }
     p = (Permset_Object*)value;
     if(acl_set_permset(self->entry, p->permset) == -1) {
+        /* LCOV_EXCL_START */
         PyErr_SetFromErrno(PyExc_IOError);
         return -1;
+        /* LCOV_EXCL_STOP */
     }
     return 0;
 }
 
 static char __Entry_copy_doc__[] =
     "copy(src)\n"
     "Copies an ACL entry.\n"
@@ -1049,15 +1075,15 @@
     Entry_Object *self = (Entry_Object*)obj;
     Entry_Object *other;
 
     if(!PyArg_ParseTuple(args, "O!", &Entry_Type, &other))
         return NULL;
 
     if(acl_copy_entry(self->entry, other->entry) == -1)
-        return PyErr_SetFromErrno(PyExc_IOError);
+        return PyErr_SetFromErrno(PyExc_IOError);  /* LCOV_EXCL_LINE */
 
     Py_RETURN_NONE;
 }
 
 /**** Permset type *****/
 
 /* Creation of a new Permset instance */
@@ -1108,25 +1134,22 @@
     return 0;
 }
 
 /* Free the Permset instance */
 static void Permset_dealloc(PyObject* obj) {
     Permset_Object *self = (Permset_Object*) obj;
     PyObject *err_type, *err_value, *err_traceback;
-    int have_error = PyErr_Occurred() ? 1 : 0;
 
-    if (have_error)
-        PyErr_Fetch(&err_type, &err_value, &err_traceback);
+    PyErr_Fetch(&err_type, &err_value, &err_traceback);
     if(self->parent_entry != NULL) {
         Py_DECREF(self->parent_entry);
         self->parent_entry = NULL;
     }
-    if (have_error)
-        PyErr_Restore(err_type, err_value, err_traceback);
-    PyObject_DEL(self);
+    PyErr_Restore(err_type, err_value, err_traceback);
+    Py_TYPE(obj)->tp_free((PyObject *)obj);
 }
 
 /* Permset string representation */
 static PyObject* Permset_str(PyObject *obj) {
     Permset_Object *self = (Permset_Object*) obj;
     char pstr[3];
 
@@ -1141,15 +1164,15 @@
     ;
 
 /* Clears all permissions from the permset */
 static PyObject* Permset_clear(PyObject* obj, PyObject* args) {
     Permset_Object *self = (Permset_Object*) obj;
 
     if(acl_clear_perms(self->permset) == -1)
-        return PyErr_SetFromErrno(PyExc_IOError);
+        return PyErr_SetFromErrno(PyExc_IOError);  /* LCOV_EXCL_LINE */
 
     Py_RETURN_NONE;
 }
 
 static PyObject* Permset_get_right(PyObject *obj, void* arg) {
     Permset_Object *self = (Permset_Object*) obj;
 
@@ -1172,16 +1195,18 @@
     }
     on = PyLong_AsLong(value);
     if(on)
         nerr = acl_add_perm(self->permset, *(acl_perm_t*)arg);
     else
         nerr = acl_delete_perm(self->permset, *(acl_perm_t*)arg);
     if(nerr == -1) {
+        /* LCOV_EXCL_START */
         PyErr_SetFromErrno(PyExc_IOError);
         return -1;
+        /* LCOV_EXCL_STOP */
     }
     return 0;
 }
 
 static char __Permset_add_doc__[] =
     "add(perm)\n"
     "Add a permission to the permission set.\n"
@@ -1200,15 +1225,15 @@
     Permset_Object *self = (Permset_Object*) obj;
     int right;
 
     if (!PyArg_ParseTuple(args, "i", &right))
         return NULL;
 
     if(acl_add_perm(self->permset, (acl_perm_t) right) == -1)
-        return PyErr_SetFromErrno(PyExc_IOError);
+        return PyErr_SetFromErrno(PyExc_IOError);  /* LCOV_EXCL_LINE */
 
     Py_RETURN_NONE;
 }
 
 static char __Permset_delete_doc__[] =
     "delete(perm)\n"
     "Delete a permission from the permission set.\n"
@@ -1227,15 +1252,15 @@
     Permset_Object *self = (Permset_Object*) obj;
     int right;
 
     if (!PyArg_ParseTuple(args, "i", &right))
         return NULL;
 
     if(acl_delete_perm(self->permset, (acl_perm_t) right) == -1)
-        return PyErr_SetFromErrno(PyExc_IOError);
+        return PyErr_SetFromErrno(PyExc_IOError);  /* LCOV_EXCL_LINE */
 
     Py_RETURN_NONE;
 }
 
 static char __Permset_test_doc__[] =
     "test(perm)\n"
     "Test if a permission exists in the permission set.\n"
@@ -1255,15 +1280,15 @@
     int ret;
 
     if (!PyArg_ParseTuple(args, "i", &right))
         return NULL;
 
     ret = get_perm(self->permset, (acl_perm_t) right);
     if(ret == -1)
-        return PyErr_SetFromErrno(PyExc_IOError);
+        return PyErr_SetFromErrno(PyExc_IOError);  /* LCOV_EXCL_LINE */
 
     if(ret) {
         Py_RETURN_TRUE;
     } else {
         Py_RETURN_FALSE;
     }
 }
@@ -1323,61 +1348,31 @@
     {NULL, NULL, 0, NULL}
 };
 
 
 /* The definition of the ACL Type */
 static PyTypeObject ACL_Type = {
     PyVarObject_HEAD_INIT(NULL, 0)
-    "posix1e.ACL",
-    sizeof(ACL_Object),
-    0,
-    ACL_dealloc,        /* tp_dealloc */
-    0,                  /* tp_print */
-    0,                  /* tp_getattr */
-    0,                  /* tp_setattr */
-    0,                  /* formerly tp_compare, in 3.0 deprecated, in
-                           3.5 tp_as_async */
-    0,                  /* tp_repr */
-    0,                  /* tp_as_number */
-    0,                  /* tp_as_sequence */
-    0,                  /* tp_as_mapping */
-    0,                  /* tp_hash */
-    0,                  /* tp_call */
-    ACL_str,            /* tp_str */
-    0,                  /* tp_getattro */
-    0,                  /* tp_setattro */
-    0,                  /* tp_as_buffer */
-    Py_TPFLAGS_DEFAULT, /* tp_flags */
-    __ACL_Type_doc__,   /* tp_doc */
-    0,                  /* tp_traverse */
-    0,                  /* tp_clear */
+    .tp_name = "posix1e.ACL",
+    .tp_basicsize = sizeof(ACL_Object),
+    .tp_itemsize = 0,
+    .tp_dealloc = ACL_dealloc,
+    .tp_str = ACL_str,
+    .tp_flags = Py_TPFLAGS_DEFAULT,
+    .tp_doc = __ACL_Type_doc__,
 #ifdef HAVE_LINUX
-    ACL_richcompare,    /* tp_richcompare */
-#else
-    0,                  /* tp_richcompare */
+    .tp_richcompare = ACL_richcompare,
 #endif
-    0,                  /* tp_weaklistoffset */
 #ifdef HAVE_LEVEL2
-    ACL_iter,
-    ACL_iternext,
-#else
-    0,                  /* tp_iter */
-    0,                  /* tp_iternext */
-#endif
-    ACL_methods,        /* tp_methods */
-    0,                  /* tp_members */
-    0,                  /* tp_getset */
-    0,                  /* tp_base */
-    0,                  /* tp_dict */
-    0,                  /* tp_descr_get */
-    0,                  /* tp_descr_set */
-    0,                  /* tp_dictoffset */
-    ACL_init,           /* tp_init */
-    0,                  /* tp_alloc */
-    ACL_new,            /* tp_new */
+    .tp_iter = ACL_iter,
+    .tp_iternext = ACL_iternext,
+#endif
+    .tp_methods = ACL_methods,
+    .tp_init = ACL_init,
+    .tp_new = ACL_new,
 };
 
 #ifdef HAVE_LEVEL2
 
 /* Entry type methods */
 static PyMethodDef Entry_methods[] = {
     {"copy", Entry_copy, METH_VARARGS, __Entry_copy_doc__},
@@ -1441,51 +1436,25 @@
     "Note that the Entry keeps a reference to its ACL, so even if \n"
     "you delete the ACL, it won't be cleaned up and will continue to \n"
     "exist until its Entry(ies) will be deleted.\n"
     ;
 /* The definition of the Entry Type */
 static PyTypeObject Entry_Type = {
     PyVarObject_HEAD_INIT(NULL, 0)
-    "posix1e.Entry",
-    sizeof(Entry_Object),
-    0,
-    Entry_dealloc,      /* tp_dealloc */
-    0,                  /* tp_print */
-    0,                  /* tp_getattr */
-    0,                  /* tp_setattr */
-    0,                  /* tp_compare */
-    0,                  /* tp_repr */
-    0,                  /* tp_as_number */
-    0,                  /* tp_as_sequence */
-    0,                  /* tp_as_mapping */
-    0,                  /* tp_hash */
-    0,                  /* tp_call */
-    Entry_str,          /* tp_str */
-    0,                  /* tp_getattro */
-    0,                  /* tp_setattro */
-    0,                  /* tp_as_buffer */
-    Py_TPFLAGS_DEFAULT, /* tp_flags */
-    __Entry_Type_doc__, /* tp_doc */
-    0,                  /* tp_traverse */
-    0,                  /* tp_clear */
-    0,                  /* tp_richcompare */
-    0,                  /* tp_weaklistoffset */
-    0,                  /* tp_iter */
-    0,                  /* tp_iternext */
-    Entry_methods,      /* tp_methods */
-    0,                  /* tp_members */
-    Entry_getsets,      /* tp_getset */
-    0,                  /* tp_base */
-    0,                  /* tp_dict */
-    0,                  /* tp_descr_get */
-    0,                  /* tp_descr_set */
-    0,                  /* tp_dictoffset */
-    Entry_init,         /* tp_init */
-    0,                  /* tp_alloc */
-    Entry_new,          /* tp_new */
+    .tp_name = "posix1e.Entry",
+    .tp_basicsize = sizeof(Entry_Object),
+    .tp_itemsize = 0,
+    .tp_dealloc = Entry_dealloc,
+    .tp_str = Entry_str,
+    .tp_flags = Py_TPFLAGS_DEFAULT,
+    .tp_doc = __Entry_Type_doc__,
+    .tp_methods = Entry_methods,
+    .tp_getset = Entry_getsets,
+    .tp_init = Entry_init,
+    .tp_new = Entry_new
 };
 
 /* Permset type methods */
 static PyMethodDef Permset_methods[] = {
     {"clear", Permset_clear, METH_NOARGS, __Permset_clear_doc__, },
     {"add", Permset_add, METH_VARARGS, __Permset_add_doc__, },
     {"delete", Permset_delete, METH_VARARGS, __Permset_delete_doc__, },
@@ -1548,51 +1517,25 @@
     "you delete the entry, it won't be cleaned up and will continue to \n"
     "exist until its Permset will be deleted.\n"
     ;
 
 /* The definition of the Permset Type */
 static PyTypeObject Permset_Type = {
     PyVarObject_HEAD_INIT(NULL, 0)
-    "posix1e.Permset",
-    sizeof(Permset_Object),
-    0,
-    Permset_dealloc,    /* tp_dealloc */
-    0,                  /* tp_print */
-    0,                  /* tp_getattr */
-    0,                  /* tp_setattr */
-    0,                  /* tp_compare */
-    0,                  /* tp_repr */
-    0,                  /* tp_as_number */
-    0,                  /* tp_as_sequence */
-    0,                  /* tp_as_mapping */
-    0,                  /* tp_hash */
-    0,                  /* tp_call */
-    Permset_str,        /* tp_str */
-    0,                  /* tp_getattro */
-    0,                  /* tp_setattro */
-    0,                  /* tp_as_buffer */
-    Py_TPFLAGS_DEFAULT, /* tp_flags */
-    __Permset_Type_doc__,/* tp_doc */
-    0,                  /* tp_traverse */
-    0,                  /* tp_clear */
-    0,                  /* tp_richcompare */
-    0,                  /* tp_weaklistoffset */
-    0,                  /* tp_iter */
-    0,                  /* tp_iternext */
-    Permset_methods,    /* tp_methods */
-    0,                  /* tp_members */
-    Permset_getsets,    /* tp_getset */
-    0,                  /* tp_base */
-    0,                  /* tp_dict */
-    0,                  /* tp_descr_get */
-    0,                  /* tp_descr_set */
-    0,                  /* tp_dictoffset */
-    Permset_init,       /* tp_init */
-    0,                  /* tp_alloc */
-    Permset_new,        /* tp_new */
+    .tp_name = "posix1e.Permset",
+    .tp_basicsize = sizeof(Permset_Object),
+    .tp_itemsize = 0,
+    .tp_dealloc = Permset_dealloc,
+    .tp_str = Permset_str,
+    .tp_flags = Py_TPFLAGS_DEFAULT,
+    .tp_doc = __Permset_Type_doc__,
+    .tp_methods = Permset_methods,
+    .tp_getset = Permset_getsets,
+    .tp_init = Permset_init,
+    .tp_new = Permset_new,
 };
 
 #endif
 
 /* Module methods */
 
 static char __deletedef_doc__[] =
@@ -1778,18 +1721,18 @@
     ".. py:data:: HAS_COPY_EXT\n\n"
     "   denotes support for __getstate__()/__setstate__() on an ACL\n"
     "\n"
     ;
 
 static struct PyModuleDef posix1emodule = {
     PyModuleDef_HEAD_INIT,
-    "posix1e",
-    __posix1e_doc__,
-    0,
-    aclmodule_methods,
+    .m_name = "posix1e",
+    .m_doc = __posix1e_doc__,
+    .m_size = 0,
+    .m_methods = aclmodule_methods,
 };
 
 PyMODINIT_FUNC
 PyInit_posix1e(void)
 {
     PyObject *m, *d;
```

### Comparing `pylibacl-0.6.0/doc/conf.py` & `pylibacl-0.7.0/doc/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 # -- General configuration -----------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #needs_sphinx = '1.0'
 
 # Add any Sphinx extension module names here, as strings. They can be extensions
 # coming with Sphinx (named 'sphinx.ext.*') or your custom ones.
-extensions = ['sphinx.ext.autodoc', 'sphinx.ext.todo']
+extensions = ['sphinx.ext.autodoc', 'sphinx.ext.todo', 'recommonmark']
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ['_templates']
 
 # The suffix of source filenames.
 source_suffix = ['.rst', '.md']
 
@@ -44,17 +44,17 @@
 copyright = u'2002-2009, 2012, 2014, 2015, Iustin Pop'
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
-version = '0.6.0'
+version = '0.7.0'
 # The full version, including alpha/beta/rc tags.
-release = '0.6.0'
+release = '0.7.0'
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #language = None
 
 # There are two options for replacing |today|: either, you set today to some
 # non-false value, then it is used:
@@ -86,20 +86,14 @@
 pygments_style = 'sphinx'
 
 # A list of ignored prefixes for module index sorting.
 #modindex_common_prefix = []
 
 keep_warnings = True
 
-# Note: this is still needed in Sphinx 1.8 with recommonmark 0.4.0
-# (https://github.com/readthedocs/recommonmark/issues/119):
-source_parsers = {
-   '.md': 'recommonmark.parser.CommonMarkParser',
-}
-
 # -- Options for HTML output ---------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 html_theme = 'default'
 
 # Theme options are theme-specific and customize the look and feel of a theme
```

### Comparing `pylibacl-0.6.0/doc/implementation.rst` & `pylibacl-0.7.0/doc/implementation.rst`

 * *Files identical despite different names*

### Comparing `pylibacl-0.6.0/posix1e.pyi` & `pylibacl-0.7.0/posix1e.pyi`

 * *Files identical despite different names*

### Comparing `pylibacl-0.6.0/pylibacl.egg-info/PKG-INFO` & `pylibacl-0.7.0/pylibacl.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,25 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: pylibacl
-Version: 0.6.0
+Version: 0.7.0
 Summary: POSIX.1e ACLs for python
 Home-page: https://pylibacl.k1024.org/
 Author: Iustin Pop
 Author-email: iustin@k1024.org
 License: LGPL
 Project-URL: Bug Tracker, https://github.com/iustin/pylibacl/issues
-Description: This is a C extension module for Python which
-        implements POSIX ACLs manipulation. It is a wrapper on top
-        of the systems's acl C library - see acl(5).
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Operating System :: POSIX :: BSD :: FreeBSD
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Filesystems
-Requires-Python: >=3.4
+Requires-Python: >=3.7
+License-File: COPYING
+
+This is a C extension module for Python which
+implements POSIX ACLs manipulation. It is a wrapper on top
+of the systems's acl C library - see acl(5).
```

### Comparing `pylibacl-0.6.0/setup.py` & `pylibacl-0.7.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,29 +27,29 @@
     raise ValueError("I don't know your system '%s'."
                      " Please contact the author" % u_sysname)
 
 long_desc = """This is a C extension module for Python which
 implements POSIX ACLs manipulation. It is a wrapper on top
 of the systems's acl C library - see acl(5)."""
 
-version = "0.6.0"
+version = "0.7.0"
 
 setup(name="pylibacl",
       version=version,
       description="POSIX.1e ACLs for python",
       long_description=long_desc,
       author="Iustin Pop",
       author_email="iustin@k1024.org",
       url="https://pylibacl.k1024.org/",
       license="LGPL",
       ext_modules=[Extension("posix1e", ["acl.c"],
                              libraries=libs,
                              define_macros=macros,
                              )],
-      python_requires = ">=3.4",
+      python_requires = ">=3.7",
       # Note: doesn't work since it's not a package. Sigh.
       package_data = {
           '': ['py.typed', 'posix1e.pyi'],
       },
       zip_safe=False,
       project_urls={
         "Bug Tracker": "https://github.com/iustin/pylibacl/issues",
```

### Comparing `pylibacl-0.6.0/tests/test_acls.py` & `pylibacl-0.7.0/tests/test_acls.py`

 * *Files 2% similar despite different names*

```diff
@@ -216,44 +216,61 @@
 
 FD_D = [
     "file FD",
     "file object",
     "file io stream",
 ]
 
+DIR_D = [
+    "directory",
+    "directory (bytes)",
+    "directory (path object)",
+]
+
+DIR_P = [
+    get_dir,
+    as_bytes(get_dir),
+    pytest.param(as_fspath(get_dir),
+                 marks=[NOT_BEFORE_36, NOT_PYPY]),
+]
+
 ALL_P = FILE_P + FD_P
 ALL_D = FILE_D + FD_D
 
 @pytest.fixture(params=FILE_P, ids=FILE_D)
 def file_subject(testdir, request):
     with request.param(testdir) as value:
         yield value
 
 @pytest.fixture(params=FD_P, ids=FD_D)
 def fd_subject(testdir, request):
     with request.param(testdir) as value:
         yield value
 
+@pytest.fixture(params=DIR_P, ids=DIR_D)
+def dir_subject(testdir, request):
+    with request.param(testdir) as value:
+        yield value
+
 @pytest.fixture(params=ALL_P, ids=ALL_D)
 def subject(testdir, request):
     with request.param(testdir) as value:
         yield value
 
 
 class TestLoad:
     """Load/create tests"""
     def test_from_file(self, file_subject):
         """Test loading ACLs from a file/directory"""
         acl = posix1e.ACL(file=file_subject)
         assert acl.valid()
 
-    def test_from_dir(self, testdir):
+    def test_from_dir(self, dir_subject):
         """Test loading ACLs from a directory"""
-        with get_dir(testdir) as dname:
-          acl2 = posix1e.ACL(filedef=dname)
+        acl2 = posix1e.ACL(filedef=dir_subject)
         # default ACLs might or might not be valid; missing ones are
         # not valid, so we don't test acl2 for validity
 
     def test_from_fd(self, fd_subject):
         """Test loading ACLs from a file descriptor"""
         acl = posix1e.ACL(fd=fd_subject)
         assert acl.valid()
@@ -503,14 +520,47 @@
         assert b == c
         state = a.__getstate__()
         b.__setstate__(state)
         assert a == b
         assert b != c
 
     @require_copy_ext
+    def test_acl_copy_ext_failure(self):
+        a = posix1e.ACL()
+        state = a.__getstate__()
+        # This is a dangerous test. The acl_copy_int() C function gets
+        # a void * buffer, and then casts that to an ACL structure,
+        # irrespective of buffer length; this can lead to segfaults
+        # (via unallocated memory indexing)
+        #
+        # To mitigate this, pass same buffer size as returned from the
+        # state, just nulled out - in the Linux version of the
+        # library, the first byte is the structure size and is tested
+        # for correct size, and a null byte will cause failure.
+        nulled = b'\x00' * len(state)
+        with pytest.raises(IOError):
+            a.__setstate__(nulled)
+
+    @require_copy_ext
+    def test_acl_copy_ext_failure(self):
+        a = posix1e.ACL(text=BASIC_ACL_TEXT)
+        b = posix1e.ACL()
+        c = posix1e.ACL(acl=a)
+        assert a == c
+        assert a != b
+        state = b.__getstate__()
+        # See notes in the test_acl_copy_ext_failure() for how tricky this is.
+        nulled = b'\x00' * len(state)
+        with pytest.raises(IOError):
+            a.__setstate__(nulled)
+        # Assert that 'a' didn't change in the attempt to restore
+        # invalid state.
+        assert a == c
+
+    @require_copy_ext
     def test_acl_copy_ext_args(self):
         a = posix1e.ACL()
         with pytest.raises(TypeError):
             a.__setstate__(None)
 
     @require_copy_ext
     def test_acl_init_copy_ext(self):
```

