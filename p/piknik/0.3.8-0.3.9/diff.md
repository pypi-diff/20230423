# Comparing `tmp/piknik-0.3.8.tar.gz` & `tmp/piknik-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "piknik-0.3.8.tar", last modified: Thu Apr 20 07:12:17 2023, max compression
+gzip compressed data, was "piknik-0.3.9.tar", last modified: Sat Apr 22 08:25:29 2023, max compression
```

## Comparing `piknik-0.3.8.tar` & `piknik-0.3.9.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-20 07:12:17.399977 piknik-0.3.8/
--rw-r--r--   0 lash      (1000) lash      (1000)     1685 2023-04-20 07:11:27.000000 piknik-0.3.8/CHANGELOG
--rw-r--r--   0 lash      (1000) lash      (1000)    35149 2022-11-15 04:36:48.000000 piknik-0.3.8/LICENSE
--rw-r--r--   0 lash      (1000) lash      (1000)       52 2022-11-15 08:02:24.000000 piknik-0.3.8/MANIFEST.in
--rw-r--r--   0 lash      (1000) lash      (1000)      646 2023-04-20 07:12:17.399977 piknik-0.3.8/PKG-INFO
--rw-r--r--   0 lash      (1000) lash      (1000)      602 2023-04-20 06:22:45.000000 piknik-0.3.8/ROADMAP
--rw-r--r--   0 lash      (1000) lash      (1000)       16 2022-12-05 09:13:24.000000 piknik-0.3.8/html_requirements.txt
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-20 07:12:17.396644 piknik-0.3.8/piknik/
--rw-r--r--   0 lash      (1000) lash      (1000)       52 2022-11-06 13:09:48.000000 piknik-0.3.8/piknik/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)     6120 2023-04-20 06:22:45.000000 piknik-0.3.8/piknik/basket.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-20 07:12:17.396644 piknik-0.3.8/piknik/cli/
--rw-r--r--   0 lash      (1000) lash      (1000)      869 2023-04-20 07:09:35.000000 piknik-0.3.8/piknik/cli/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)      485 2023-03-21 20:53:45.000000 piknik-0.3.8/piknik/cli/add.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1221 2023-03-21 20:53:45.000000 piknik-0.3.8/piknik/cli/comment.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2827 2023-03-21 20:53:45.000000 piknik-0.3.8/piknik/cli/mod.py
--rw-r--r--   0 lash      (1000) lash      (1000)        1 2023-03-21 20:53:45.000000 piknik-0.3.8/piknik/cli/session.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2932 2023-04-20 07:03:07.000000 piknik-0.3.8/piknik/cli/show.py
--rw-r--r--   0 lash      (1000) lash      (1000)     4107 2023-03-21 20:53:45.000000 piknik-0.3.8/piknik/crypto.py
--rw-r--r--   0 lash      (1000) lash      (1000)      169 2023-01-16 11:02:46.000000 piknik-0.3.8/piknik/error.py
--rw-r--r--   0 lash      (1000) lash      (1000)      443 2022-11-15 07:03:41.000000 piknik-0.3.8/piknik/identity.py
--rw-r--r--   0 lash      (1000) lash      (1000)     3443 2023-01-16 11:02:46.000000 piknik-0.3.8/piknik/issue.py
--rw-r--r--   0 lash      (1000) lash      (1000)     4381 2022-12-05 09:13:24.000000 piknik-0.3.8/piknik/msg.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-20 07:12:17.396644 piknik-0.3.8/piknik/render/
--rw-r--r--   0 lash      (1000) lash      (1000)     5505 2023-04-20 07:03:07.000000 piknik-0.3.8/piknik/render/base.py
--rw-r--r--   0 lash      (1000) lash      (1000)     6229 2023-04-20 07:03:07.000000 piknik-0.3.8/piknik/render/html.py
--rw-r--r--   0 lash      (1000) lash      (1000)     3860 2023-01-16 11:02:46.000000 piknik-0.3.8/piknik/render/plain.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-20 07:12:17.396644 piknik-0.3.8/piknik/runnable/
--rw-r--r--   0 lash      (1000) lash      (1000)     2001 2023-04-20 07:03:07.000000 piknik-0.3.8/piknik/runnable/cmd.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-20 07:12:17.396644 piknik-0.3.8/piknik/store/
--rw-r--r--   0 lash      (1000) lash      (1000)     2196 2023-04-20 06:22:45.000000 piknik-0.3.8/piknik/store/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2601 2022-12-05 09:13:24.000000 piknik-0.3.8/piknik/wrap.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-20 07:12:17.396644 piknik-0.3.8/piknik.egg-info/
--rw-r--r--   0 lash      (1000) lash      (1000)      646 2023-04-20 07:12:17.000000 piknik-0.3.8/piknik.egg-info/PKG-INFO
--rw-r--r--   0 lash      (1000) lash      (1000)      865 2023-04-20 07:12:17.000000 piknik-0.3.8/piknik.egg-info/SOURCES.txt
--rw-r--r--   0 lash      (1000) lash      (1000)        1 2023-04-20 07:12:17.000000 piknik-0.3.8/piknik.egg-info/dependency_links.txt
--rw-r--r--   0 lash      (1000) lash      (1000)       52 2023-04-20 07:12:17.000000 piknik-0.3.8/piknik.egg-info/entry_points.txt
--rw-r--r--   0 lash      (1000) lash      (1000)       88 2023-04-20 07:12:17.000000 piknik-0.3.8/piknik.egg-info/requires.txt
--rw-r--r--   0 lash      (1000) lash      (1000)        7 2023-04-20 07:12:17.000000 piknik-0.3.8/piknik.egg-info/top_level.txt
--rw-r--r--   0 lash      (1000) lash      (1000)       72 2023-04-20 06:22:45.000000 piknik-0.3.8/requirements.txt
--rw-r--r--   0 lash      (1000) lash      (1000)      826 2023-04-20 07:12:17.399977 piknik-0.3.8/setup.cfg
--rw-r--r--   0 lash      (1000) lash      (1000)      622 2022-12-05 09:16:06.000000 piknik-0.3.8/setup.py
--rw-r--r--   0 lash      (1000) lash      (1000)        0 2022-11-15 07:03:41.000000 piknik-0.3.8/test_requirements.txt
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-20 07:12:17.399977 piknik-0.3.8/tests/
--rw-r--r--   0 lash      (1000) lash      (1000)     2607 2022-11-15 07:03:41.000000 piknik-0.3.8/tests/test_assign.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2831 2022-11-07 08:29:09.000000 piknik-0.3.8/tests/test_basic.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2946 2022-12-05 09:13:24.000000 piknik-0.3.8/tests/test_crypto.py
--rw-r--r--   0 lash      (1000) lash      (1000)      782 2023-01-16 11:02:46.000000 piknik-0.3.8/tests/test_dep.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2845 2022-12-05 09:13:24.000000 piknik-0.3.8/tests/test_html.py
--rw-r--r--   0 lash      (1000) lash      (1000)      614 2022-11-15 07:03:41.000000 piknik-0.3.8/tests/test_issue.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2266 2022-12-05 09:13:24.000000 piknik-0.3.8/tests/test_msg.py
--rw-r--r--   0 lash      (1000) lash      (1000)     3547 2022-12-05 09:13:24.000000 piknik-0.3.8/tests/test_render.py
--rw-r--r--   0 lash      (1000) lash      (1000)     2992 2022-11-18 08:08:40.000000 piknik-0.3.8/tests/test_store.py
--rw-r--r--   0 lash      (1000) lash      (1000)      748 2022-11-06 23:15:22.000000 piknik-0.3.8/tests/test_tag.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-22 08:25:29.699960 piknik-0.3.9/
+-rw-r--r--   0 lash      (1000) lash      (1000)     1811 2023-04-22 08:24:29.000000 piknik-0.3.9/CHANGELOG
+-rw-r--r--   0 lash      (1000) lash      (1000)    35149 2022-11-15 04:36:48.000000 piknik-0.3.9/LICENSE
+-rw-r--r--   0 lash      (1000) lash      (1000)       52 2022-11-15 08:02:24.000000 piknik-0.3.9/MANIFEST.in
+-rw-r--r--   0 lash      (1000) lash      (1000)      646 2023-04-22 08:25:29.699960 piknik-0.3.9/PKG-INFO
+-rw-r--r--   0 lash      (1000) lash      (1000)      602 2023-04-20 06:22:45.000000 piknik-0.3.9/ROADMAP
+-rw-r--r--   0 lash      (1000) lash      (1000)       16 2022-12-05 09:13:24.000000 piknik-0.3.9/html_requirements.txt
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-22 08:25:29.696627 piknik-0.3.9/piknik/
+-rw-r--r--   0 lash      (1000) lash      (1000)       52 2022-11-06 13:09:48.000000 piknik-0.3.9/piknik/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     7012 2023-04-22 08:09:54.000000 piknik-0.3.9/piknik/basket.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-22 08:25:29.699960 piknik-0.3.9/piknik/cli/
+-rw-r--r--   0 lash      (1000) lash      (1000)      918 2023-04-22 07:26:33.000000 piknik-0.3.9/piknik/cli/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      502 2023-04-22 08:00:15.000000 piknik-0.3.9/piknik/cli/add.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1221 2023-03-21 20:53:45.000000 piknik-0.3.9/piknik/cli/comment.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2827 2023-03-21 20:53:45.000000 piknik-0.3.9/piknik/cli/mod.py
+-rw-r--r--   0 lash      (1000) lash      (1000)        1 2023-03-21 20:53:45.000000 piknik-0.3.9/piknik/cli/session.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2932 2023-04-20 07:21:36.000000 piknik-0.3.9/piknik/cli/show.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     4107 2023-03-21 20:53:45.000000 piknik-0.3.9/piknik/crypto.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      169 2023-01-16 11:02:46.000000 piknik-0.3.9/piknik/error.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      443 2022-11-15 07:03:41.000000 piknik-0.3.9/piknik/identity.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     3540 2023-04-22 07:11:57.000000 piknik-0.3.9/piknik/issue.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     4381 2022-12-05 09:13:24.000000 piknik-0.3.9/piknik/msg.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-22 08:25:29.699960 piknik-0.3.9/piknik/render/
+-rw-r--r--   0 lash      (1000) lash      (1000)     5505 2023-04-20 07:21:36.000000 piknik-0.3.9/piknik/render/base.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     6229 2023-04-20 07:21:36.000000 piknik-0.3.9/piknik/render/html.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     3950 2023-04-22 08:01:40.000000 piknik-0.3.9/piknik/render/plain.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-22 08:25:29.699960 piknik-0.3.9/piknik/runnable/
+-rw-r--r--   0 lash      (1000) lash      (1000)     2100 2023-04-22 07:59:23.000000 piknik-0.3.9/piknik/runnable/cmd.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-22 08:25:29.699960 piknik-0.3.9/piknik/store/
+-rw-r--r--   0 lash      (1000) lash      (1000)     3004 2023-04-22 08:08:48.000000 piknik-0.3.9/piknik/store/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2601 2022-12-05 09:13:24.000000 piknik-0.3.9/piknik/wrap.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-22 08:25:29.699960 piknik-0.3.9/piknik.egg-info/
+-rw-r--r--   0 lash      (1000) lash      (1000)      646 2023-04-22 08:25:29.000000 piknik-0.3.9/piknik.egg-info/PKG-INFO
+-rw-r--r--   0 lash      (1000) lash      (1000)      865 2023-04-22 08:25:29.000000 piknik-0.3.9/piknik.egg-info/SOURCES.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)        1 2023-04-22 08:25:29.000000 piknik-0.3.9/piknik.egg-info/dependency_links.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)       52 2023-04-22 08:25:29.000000 piknik-0.3.9/piknik.egg-info/entry_points.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)       88 2023-04-22 08:25:29.000000 piknik-0.3.9/piknik.egg-info/requires.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)        7 2023-04-22 08:25:29.000000 piknik-0.3.9/piknik.egg-info/top_level.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)       72 2023-04-20 06:22:45.000000 piknik-0.3.9/requirements.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)      826 2023-04-22 08:25:29.699960 piknik-0.3.9/setup.cfg
+-rw-r--r--   0 lash      (1000) lash      (1000)      622 2022-12-05 09:16:06.000000 piknik-0.3.9/setup.py
+-rw-r--r--   0 lash      (1000) lash      (1000)        0 2022-11-15 07:03:41.000000 piknik-0.3.9/test_requirements.txt
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-04-22 08:25:29.699960 piknik-0.3.9/tests/
+-rw-r--r--   0 lash      (1000) lash      (1000)     2607 2022-11-15 07:03:41.000000 piknik-0.3.9/tests/test_assign.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     3159 2023-04-22 07:21:10.000000 piknik-0.3.9/tests/test_basic.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2946 2022-12-05 09:13:24.000000 piknik-0.3.9/tests/test_crypto.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      782 2023-01-16 11:02:46.000000 piknik-0.3.9/tests/test_dep.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2845 2022-12-05 09:13:24.000000 piknik-0.3.9/tests/test_html.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      614 2022-11-15 07:03:41.000000 piknik-0.3.9/tests/test_issue.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2266 2022-12-05 09:13:24.000000 piknik-0.3.9/tests/test_msg.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     3547 2022-12-05 09:13:24.000000 piknik-0.3.9/tests/test_render.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     2992 2022-11-18 08:08:40.000000 piknik-0.3.9/tests/test_store.py
+-rw-r--r--   0 lash      (1000) lash      (1000)      748 2022-11-06 23:15:22.000000 piknik-0.3.9/tests/test_tag.py
```

### Comparing `piknik-0.3.8/CHANGELOG` & `piknik-0.3.9/CHANGELOG`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+- 0.3.9
+	* Add issue id alias for easier referencing when cli manipulation
+	* Auto-generate disposable gnupg key for cli test
 - 0.3.8
 	* Fix broken add tool
 	* Add minimal sanity cli tests
 - 0.3.7
 	* Complete incomplete change from 0.3.6
 - 0.3.6
 	* Enable --help display without subcommand
```

### Comparing `piknik-0.3.8/LICENSE` & `piknik-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `piknik-0.3.8/PKG-INFO` & `piknik-0.3.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: piknik
-Version: 0.3.8
+Version: 0.3.9
 Summary: CLI issue tracker
 Home-page: https://git.defalsify.org/piknik
 Author: Louis Holbrook
 Author-email: dev@holbrook.no
 License: GPLv3+
 Keywords: bugs,issues,tracker,productivity,git,pgp
 Classifier: Programming Language :: Python :: 3
```

### Comparing `piknik-0.3.8/ROADMAP` & `piknik-0.3.9/ROADMAP`

 * *Files identical despite different names*

### Comparing `piknik-0.3.8/piknik/basket.py` & `piknik-0.3.9/piknik/basket.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # standard imports
 import logging
 
 # external imports
 import shep
+from shep.error import StateItemNotFound
 
 # local imports
 from .error import DeadIssue
 from .issue import Issue
 from .msg import IssueMessage
 from .identity import Identity
 
@@ -30,38 +31,49 @@
 
         self.__tags = state_factory.create_tags()
         self.__tags.sync(ignore_auto=False)
 
         self.__msg = state_factory.create_messages()
         self.__msg_wrap = message_wrapper
 
+        self.__alias = state_factory.create_aliases()
+
         self.issues_rev = {}
 
 
     def __check_resurrect(self, st, k, f, t):
         if self.no_resurrect:
             if f & self.state.FINISHED > 0:
                 raise DeadIssue(k)
 
 
     def add(self, issue):
         issue_id = str(issue.id)
-        self.state.put(issue_id, contents=str(issue))
+        j = str(issue)
+        if issue.alias != None:
+            self.__alias.put(issue.alias, issue.id)
+        self.state.put(issue_id, contents=j)
         self.__tags.put(issue_id)
         return issue_id
 
 
     def get(self, issue_id):
+        logg.debug("basked issue get {}".format(issue_id))
         r = self.state.get(issue_id)
+        if r == None:
+            aliased_issue_id = self.__alias.get(issue_id)
+            r = self.state.get(aliased_issue_id)
+            logg.debug("resolved issue {} from alias '{}': {}".format(aliased_issue_id, issue_id, r))
         o = Issue.from_str(r)
         return o
 
 
     def get_state(self, issue_id):
-        v = self.state.state(issue_id)
+        o = self.get(issue_id)
+        v = self.state.state(o.id)
         return self.state.name(v)
 
 
     def list(self, category=None):
         if category == None:
             category = self.state.BACKLOG
         else:
@@ -82,15 +94,18 @@
 
 
     def state_backlog(self, issue_id):
         self.state.move(issue_id, self.state.BACKLOG)
 
 
     def state_finish(self, issue_id):
-        self.state.move(issue_id, self.state.FINISHED)
+        o = self.get(issue_id)
+        self.state.move(o.id, self.state.FINISHED)
+        if o.alias != None:
+            self.__alias.purge(o.alias)
 
 
     def advance(self, issue_id):
         if self.state.state(issue_id) & self.limit > 0:
             raise DeadIssue(issue_id)
         self.unblock(issue_id)
         self.state.next(issue_id)
@@ -139,80 +154,89 @@
 
     def untag(self, issue_id, tag):
         v = self.__tags.from_name(tag)
         self.__tags.unset(issue_id, v, allow_base=True)
 
 
     def tags(self, issue_id):
-        v = self.__tags.state(issue_id)
+        o = self.get(issue_id)
+        v = self.__tags.state(o.id) #issue_id)
         r = self.__tags.elements(v)
         if r == 'UNTAGGED':
             r = '(' + r + ')'
         return shep.state.split_elements(r)
 
 
     def __get_msg(self, issue_id, envelope_callback=None, message_callback=None, post_callback=None):
-        r = self.state.get(issue_id)
-        o = Issue.from_str(r)
+        #r = self.state.get(issue_id)
+        o = self.get(issue_id)
+        #o = Issue.from_str(r)
         try:
-            v = self.__msg.get(issue_id)
+            v = self.__msg.get(o.id)
             m = IssueMessage.parse(o, v.decode('utf-8'), envelope_callback=envelope_callback, message_callback=message_callback, post_callback=post_callback)
             return m
         except FileNotFoundError as e:
-            logg.debug('instantiating new message log for {} {}'.format(issue_id, e))
+            logg.debug('instantiating new message log for {} {}'.format(o.id, e))
 
         return IssueMessage(o)
 
 
     def get_msg(self, issue_id, envelope_callback=None, message_callback=None, post_callback=None):
         return self.__get_msg(issue_id, envelope_callback=envelope_callback, message_callback=message_callback, post_callback=post_callback)
  
     
     def dep(self, issue_id, dependency_issue_id):
-        r = self.state.get(issue_id)
-        self.state.get(dependency_issue_id)
-        o = Issue.from_str(r)
+        #r = self.state.get(issue_id)
+        o = self.get(issue_id)
+        #self.state.get(dependency_issue_id)
+        self.get(dependency_issue_id)
+        #o = Issue.from_str(r)
         r = o.dep(dependency_issue_id)
-        self.state.replace(issue_id, contents=str(o))
+        self.state.replace(o.id, contents=str(o))
         return r
 
 
     def undep(self, issue_id, dependency_issue_id):
-        r = self.state.get(issue_id)
-        self.state.get(dependency_issue_id)
-        o = Issue.from_str(r)
+        #r = self.state.get(issue_id)
+        o = self.get(issue_id)
+        #self.state.get(dependency_issue_id)
+        self.get(dependency_issue_id)
+        #o = Issue.from_str(r)
         r = o.undep(dependency_issue_id)
-        self.state.replace(issue_id, contents=str(o))
+        self.state.replace(o.id, contents=str(o))
         return r
 
 
     def assign(self, issue_id, identity):
-        r = self.state.get(issue_id)
-        o = Issue.from_str(r)
+        #r = self.state.get(issue_id)
+        o = self.get(issue_id)
+        #o = Issue.from_str(r)
         v = Identity(identity)
         r = o.assign(v)
-        self.state.replace(issue_id, contents=str(o))
+        self.state.replace(o.id, contents=str(o))
         return r
 
 
     def owner(self, issue_id, identity):
-        r = self.state.get(issue_id)
-        o = Issue.from_str(r)
+        #r = self.state.get(issue_id)
+        o = self.get(issue_id)
+        #o = Issue.from_str(r)
         v = Identity(identity)
         r = o.set_owner(v)
-        self.state.replace(issue_id, contents=str(o))
+        self.state.replace(o.id, contents=str(o))
         return r
 
 
     def unassign(self, issue_id, identity):
-        r = self.state.get(issue_id)
-        o = Issue.from_str(r)
+        #r = self.state.get(issue_id)
+        o = self.get(issue_id)
+        #o = Issue.from_str(r)
         v = Identity(identity)
         r = o.unassign(v)
-        self.state.replace(issue_id, contents=str(o))
+        self.state.replace(o.id, contents=str(o))
         return r
 
 
     def msg(self, issue_id, *args):
         m = self.__get_msg(issue_id)
         m.add(*args, wrapper=self.__msg_wrap)
         ms = m.as_bytes()
```

### Comparing `piknik-0.3.8/piknik/cli/__init__.py` & `piknik-0.3.9/piknik/cli/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from piknik.crypto import PGPSigner
 
 class Context:
 
     def __init__(self, arg, assembler, mode=0, gpg_home=os.environ.get('GPGHOME')):
         self.issue_id = arg.issue_id
         self.files_dir = arg.files_dir
+        self.alias = getattr(arg, 'alias', None)
         self.show_finished = getattr(arg, 'show_finished', False)
         self.show_states = getattr(arg, 'state', [])
         #self.store_factory = FileStoreFactory(arg.d)
         store_factory = FileStoreFactory(arg.d)
         self.signer = None
         sign_fn = None
         if hasattr(arg, 's'):
```

### Comparing `piknik-0.3.8/piknik/cli/comment.py` & `piknik-0.3.9/piknik/cli/comment.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.8/piknik/cli/mod.py` & `piknik-0.3.9/piknik/cli/mod.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.8/piknik/cli/show.py` & `piknik-0.3.9/piknik/cli/show.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.8/piknik/crypto.py` & `piknik-0.3.9/piknik/crypto.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.8/piknik/issue.py` & `piknik-0.3.9/piknik/issue.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,22 +7,23 @@
 from piknik.identity import Identity
 from piknik.error import UnknownIdentityError
 from piknik.error import ExistsError
 
 
 class Issue:
 
-    def __init__(self, title, issue_id=None):
+    def __init__(self, title, issue_id=None, alias=None):
         if issue_id == None:
             issue_id = str(uuid.uuid4())
         self.id = issue_id
         self.title = title
         self.assigned = []
         self.assigned_time = []
         self.dependencies = []
+        self.alias = alias
         self.owner_idx = 0
 
 
     @staticmethod
     def from_str(s):
         r = json.loads(s)
         o = Issue(title=r['title'], issue_id=r['id'])
@@ -32,14 +33,15 @@
             t = datetime.datetime.utcfromtimestamp(r['assigned'][k])
             o.assigned_time.append(t)
             if r['owner'] == None or k == r['owner']:
                 r['owner'] = k
                 o.owner_idx = i
         for v in r['dependencies']:
             o.dep(v)
+        o.alias = r['alias']
         return o
 
 
     def assign(self, identity, t=None):
         if identity in self.assigned:
             raise ExistsError(identity)
         if t == None:
@@ -95,22 +97,23 @@
 
         for i, v in enumerate(self.assigned):
             if v == identity:
                 self.owner_idx = i
                 return True
 
         raise UnknownIdentityError(identity)
-        
 
+    
     def __str__(self):
         o = {
             'id': str(self.id),
             'title': self.title,
             'assigned': {},
             'dependencies': self.dependencies,
+            'alias': self.alias,
             'owner': None,
             }
 
         for i, v in enumerate(self.get_assigned()):
             aid = v[0].id()
             o['assigned'][aid] = v[1].timestamp()
             if self.owner_idx == i:
```

### Comparing `piknik-0.3.8/piknik/msg.py` & `piknik-0.3.9/piknik/msg.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.8/piknik/render/base.py` & `piknik-0.3.9/piknik/render/base.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.8/piknik/render/html.py` & `piknik-0.3.9/piknik/render/html.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.8/piknik/render/plain.py` & `piknik-0.3.9/piknik/render/plain.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,19 +46,22 @@
         self.dump_dir = dump_dir
 
 
     def apply_issue(self, state, issue, tags, accumulator=None):
         if self.render_mode == 0:
             return self.apply_issue_standalone(state, issue, tags, accumulator=accumulator)
 
-        s = '{}\t{}\t{}\n'.format(
+        s = '{}\t{}\t{}'.format(
                 issue.title,
                 ','.join(tags),
                 issue.id,
                 )
+        if issue.alias != None:
+            s += " (" + issue.alias + ")"
+        s += "\n"
         self.add(s, accumulator=accumulator)
         super(Renderer, self).apply_issue(state, issue, tags, accumulator=accumulator)
 
 
     def apply_issue_standalone(self, state, issue, tags, accumulator=None):
         s = """title: {}
 id: {}
```

### Comparing `piknik-0.3.8/piknik/runnable/cmd.py` & `piknik-0.3.9/piknik/runnable/cmd.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 
 argp = argparse.ArgumentParser()
 argp.add_argument('-d', type=str, help='Data directory')
 argp.add_argument('-f', '--files', dest='f', action='store_true', help='Save attachments to filesystem')
 argp.add_argument('-o', '--files-dir', dest='files_dir', type=str, help='Directory to output saved files to')
 argp.add_argument('-v', action='store_true', help='Turn on debug logs')
 argp.add_argument('-i','--issue-id',  type=str, help='Issue id to show')
+argp.add_argument('--alias', type=str, help='alias string to refer to issue to with cli commands')
 argp.add_argument('cmd', type=str, nargs='?', choices=['show', 'add', 'mod', 'comment'], help='subcommand to execute')
 strargs = copy.copy(sys.argv[1:])
 
 have_help = False
 try:
     strargs.remove('-h')
     have_help = True
```

### Comparing `piknik-0.3.8/piknik/store/__init__.py` & `piknik-0.3.9/piknik/store/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -24,15 +24,14 @@
     def __check(self, key, content, prefix):
         pass
 
 
     def get(self, k):
         u = uuid.UUID(k)
         fp = self.to_filepath(u.hex)
-        f = None
         f = open(fp, 'rb')
         r = f.read()
         f.close()
         return r
 
 
     def key_to_string(self, k):
@@ -42,14 +41,49 @@
 
     def put(self, k, v):
         u = uuid.UUID(k)
         logg.debug('putting {}'.format(u.bytes.hex()))
         return self.add(u.bytes, v)
 
 
+class AliasDir:
+
+    def __init__(self, root_path):
+        self.dir = root_path
+        os.makedirs(self.dir, exist_ok=True)
+
+
+    def get(self, k):
+        fp = os.path.join(self.dir, k)
+        f = open(fp, 'rb')
+        r = f.read()
+        f.close()
+        u = uuid.UUID(r.hex())
+        return str(u)
+
+
+    def key_to_string(self, k):
+        u = uuid.UUID(bytes=k)
+        return u.bytes.hex()
+
+
+    def put(self, k, v):
+        u = uuid.UUID(v)
+        fp = os.path.join(self.dir, k)
+        logg.debug('putting {} {}'.format(u.bytes.hex(), fp))
+        f = open(fp, 'xb')
+        f.write(u.bytes)
+        f.close()
+
+
+    def purge(self, k):
+        fp = os.path.join(self.dir, k)
+        os.remove(fp)
+
+
 class FileStoreFactory:
 
     def __init__(self, directory=None):
         if directory == None:
             directory = os.path.join('.', '.piknik')
         self.directory = directory
 
@@ -79,7 +113,12 @@
                 
         return state
 
 
     def create_messages(self):
         d = os.path.join(self.directory, '.msg')
         return MsgDir(d)
+
+
+    def create_aliases(self):
+        d = os.path.join(self.directory, '.alias')
+        return AliasDir(d)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `piknik-0.3.8/piknik/wrap.py` & `piknik-0.3.9/piknik/wrap.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.8/piknik.egg-info/PKG-INFO` & `piknik-0.3.9/piknik.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: piknik
-Version: 0.3.8
+Version: 0.3.9
 Summary: CLI issue tracker
 Home-page: https://git.defalsify.org/piknik
 Author: Louis Holbrook
 Author-email: dev@holbrook.no
 License: GPLv3+
 Keywords: bugs,issues,tracker,productivity,git,pgp
 Classifier: Programming Language :: Python :: 3
```

### Comparing `piknik-0.3.8/piknik.egg-info/SOURCES.txt` & `piknik-0.3.9/piknik.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `piknik-0.3.8/setup.cfg` & `piknik-0.3.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = piknik
-version = 0.3.8
+version = 0.3.9
 description = CLI issue tracker
 author = Louis Holbrook
 author_email = dev@holbrook.no
 url = https://git.defalsify.org/piknik
 keywords = 
 	bugs
 	issues
```

### Comparing `piknik-0.3.8/setup.py` & `piknik-0.3.9/setup.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.8/tests/test_assign.py` & `piknik-0.3.9/tests/test_assign.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.8/tests/test_basic.py` & `piknik-0.3.9/tests/test_basic.py`

 * *Files 10% similar despite different names*

```diff
@@ -112,9 +112,20 @@
 
 
     def test_states_list(self):
         r = self.b.states()
         self.assertEqual(len(r), 7)
 
 
+    def test_alias(self):
+        o = Issue('The first issue', alias="first")
+        issue_id = o.id
+        v = self.b.add(o)
+        o = self.b.get("first")
+        self.assertEqual(o.id, issue_id)
+        self.b.state_finish(issue_id)
+        with self.assertRaises(FileNotFoundError):
+            o = self.b.get("first")
+
+
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `piknik-0.3.8/tests/test_crypto.py` & `piknik-0.3.9/tests/test_crypto.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.8/tests/test_dep.py` & `piknik-0.3.9/tests/test_dep.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.8/tests/test_html.py` & `piknik-0.3.9/tests/test_html.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.8/tests/test_issue.py` & `piknik-0.3.9/tests/test_issue.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.8/tests/test_msg.py` & `piknik-0.3.9/tests/test_msg.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.8/tests/test_render.py` & `piknik-0.3.9/tests/test_render.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.8/tests/test_store.py` & `piknik-0.3.9/tests/test_store.py`

 * *Files identical despite different names*

### Comparing `piknik-0.3.8/tests/test_tag.py` & `piknik-0.3.9/tests/test_tag.py`

 * *Files identical despite different names*

