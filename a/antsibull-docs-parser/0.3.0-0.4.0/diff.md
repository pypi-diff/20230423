# Comparing `tmp/antsibull_docs_parser-0.3.0.tar.gz` & `tmp/antsibull_docs_parser-0.4.0.tar.gz`

## Comparing `antsibull_docs_parser-0.3.0.tar` & `antsibull_docs_parser-0.4.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.3.0/.flake8
--rw-r--r--   0        0        0    15727 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.3.0/.pylintrc.automated
--rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.3.0/CHANGELOG.rst
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.3.0/CHANGELOG.rst.license
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.3.0/LICENSE
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.3.0/codecov.yml
--rw-r--r--   0        0        0     6620 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.3.0/noxfile.py
--rw-r--r--   0        0        0   139609 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.3.0/test-vectors.yaml
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.3.0/.github/dependabot.yml
--rw-r--r--   0        0        0     2627 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.3.0/.github/workflows/nox.yml
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.3.0/.reuse/dep5
--rw-r--r--   0        0        0     2568 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.3.0/changelogs/changelog.yaml
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.3.0/changelogs/changelog.yaml.license
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.3.0/changelogs/config.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.3.0/changelogs/fragments/.keep
--rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.3.0/src/antsibull_docs_parser/__init__.py
--rw-r--r--   0        0        0     3595 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.3.0/src/antsibull_docs_parser/_parser_impl.py
--rw-r--r--   0        0        0     3480 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.3.0/src/antsibull_docs_parser/ansible_doc_text.py
--rw-r--r--   0        0        0     8831 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.3.0/src/antsibull_docs_parser/dom.py
--rw-r--r--   0        0        0     7858 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.3.0/src/antsibull_docs_parser/format.py
--rw-r--r--   0        0        0     8807 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.3.0/src/antsibull_docs_parser/html.py
--rw-r--r--   0        0        0     4080 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.3.0/src/antsibull_docs_parser/md.py
--rw-r--r--   0        0        0    14122 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.3.0/src/antsibull_docs_parser/parser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.3.0/src/antsibull_docs_parser/py.typed
--rw-r--r--   0        0        0     8419 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.3.0/src/antsibull_docs_parser/rst.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.3.0/tests/unit/__init__.py
--rwxr-xr-x   0        0        0     2586 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.3.0/tests/unit/create-vectors.py
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.3.0/tests/unit/test_ansible_doc_text.py
--rw-r--r--   0        0        0     4567 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.3.0/tests/unit/test_dom.py
--rw-r--r--   0        0        0     2234 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.3.0/tests/unit/test_format.py
--rw-r--r--   0        0        0     1388 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.3.0/tests/unit/test_html.py
--rw-r--r--   0        0        0      678 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.3.0/tests/unit/test_md.py
--rw-r--r--   0        0        0    24557 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.3.0/tests/unit/test_parser.py
--rw-r--r--   0        0        0     3320 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.3.0/tests/unit/test_parser_impl.py
--rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.3.0/tests/unit/test_rst.py
--rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.3.0/tests/unit/test_vectors.py
--rw-r--r--   0        0        0     4623 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.3.0/tests/unit/vectors.py
--rw-r--r--   0        0        0     2058 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.3.0/.gitignore
--rw-r--r--   0        0        0     2579 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.3.0/README.md
--rw-r--r--   0        0        0     2134 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.3.0/LICENSES/BSD-2-Clause.txt
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.3.0/LICENSES/GPL-3.0-or-later.txt -> ../LICENSE
--rw-r--r--   0        0        0     4694 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.4.0/.flake8
+-rw-r--r--   0        0        0    15727 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.4.0/.pylintrc.automated
+-rw-r--r--   0        0        0     2926 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.4.0/CHANGELOG.rst
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.4.0/CHANGELOG.rst.license
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.4.0/LICENSE
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.4.0/codecov.yml
+-rw-r--r--   0        0        0     6620 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.4.0/noxfile.py
+-rw-r--r--   0        0        0   141180 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.4.0/test-vectors.yaml
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.4.0/.github/dependabot.yml
+-rw-r--r--   0        0        0     2627 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.4.0/.github/workflows/nox.yml
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.4.0/.reuse/dep5
+-rw-r--r--   0        0        0     3125 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.4.0/changelogs/changelog.yaml
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.4.0/changelogs/changelog.yaml.license
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.4.0/changelogs/config.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.4.0/changelogs/fragments/.keep
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.4.0/src/antsibull_docs_parser/__init__.py
+-rw-r--r--   0        0        0     3595 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.4.0/src/antsibull_docs_parser/_parser_impl.py
+-rw-r--r--   0        0        0     3480 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.4.0/src/antsibull_docs_parser/ansible_doc_text.py
+-rw-r--r--   0        0        0     8831 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.4.0/src/antsibull_docs_parser/dom.py
+-rw-r--r--   0        0        0     7858 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.4.0/src/antsibull_docs_parser/format.py
+-rw-r--r--   0        0        0     8862 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.4.0/src/antsibull_docs_parser/html.py
+-rw-r--r--   0        0        0     4024 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.4.0/src/antsibull_docs_parser/md.py
+-rw-r--r--   0        0        0    14122 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.4.0/src/antsibull_docs_parser/parser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.4.0/src/antsibull_docs_parser/py.typed
+-rw-r--r--   0        0        0     8419 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.4.0/src/antsibull_docs_parser/rst.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.4.0/tests/unit/__init__.py
+-rwxr-xr-x   0        0        0     2561 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.4.0/tests/unit/create-vectors.py
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.4.0/tests/unit/test_ansible_doc_text.py
+-rw-r--r--   0        0        0     4567 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.4.0/tests/unit/test_dom.py
+-rw-r--r--   0        0        0     2234 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.4.0/tests/unit/test_format.py
+-rw-r--r--   0        0        0     1388 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.4.0/tests/unit/test_html.py
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.4.0/tests/unit/test_md.py
+-rw-r--r--   0        0        0    24557 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.4.0/tests/unit/test_parser.py
+-rw-r--r--   0        0        0     3320 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.4.0/tests/unit/test_parser_impl.py
+-rw-r--r--   0        0        0      841 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.4.0/tests/unit/test_rst.py
+-rw-r--r--   0        0        0     2713 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.4.0/tests/unit/test_vectors.py
+-rw-r--r--   0        0        0     4606 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.4.0/tests/unit/vectors.py
+-rw-r--r--   0        0        0     2058 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.4.0/.gitignore
+-rw-r--r--   0        0        0     2579 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.4.0/README.md
+-rw-r--r--   0        0        0     2134 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.4.0/LICENSES/BSD-2-Clause.txt
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.4.0/LICENSES/GPL-3.0-or-later.txt -> ../LICENSE
+-rw-r--r--   0        0        0     4694 2020-02-02 00:00:00.000000 antsibull_docs_parser-0.4.0/PKG-INFO
```

### Comparing `antsibull_docs_parser-0.3.0/.pylintrc.automated` & `antsibull_docs_parser-0.4.0/.pylintrc.automated`

 * *Files identical despite different names*

### Comparing `antsibull_docs_parser-0.3.0/CHANGELOG.rst` & `antsibull_docs_parser-0.4.0/CHANGELOG.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,33 @@
 =================================================================================================
 antsibull-docs-parser -- Python library for processing Ansible documentation markup Release Notes
 =================================================================================================
 
 .. contents:: Topics
 
 
+v0.4.0
+======
+
+Release Summary
+---------------
+
+Feature and bugfix release.
+
+Minor Changes
+-------------
+
+- Adjust URL escaping to be more similar to JavaScript's ``encodeURI()`` (https://github.com/ansible-community/antsibull-docs-parser/pull/24).
+- Also escape ``.`` in MarkDown (https://github.com/ansible-community/antsibull-docs-parser/pull/24).
+
+Bugfixes
+--------
+
+- Fix URL escaping in MarkDown (https://github.com/ansible-community/antsibull-docs-parser/pull/24).
+
 v0.3.0
 ======
 
 Release Summary
 ---------------
 
 Feature release.
```

### Comparing `antsibull_docs_parser-0.3.0/LICENSE` & `antsibull_docs_parser-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `antsibull_docs_parser-0.3.0/noxfile.py` & `antsibull_docs_parser-0.4.0/noxfile.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs_parser-0.3.0/test-vectors.yaml` & `antsibull_docs_parser-0.4.0/test-vectors.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     source: |-
       This is a C(test) I(module) B(markup).
     html: |-
       <p>This is a <code class='docutils literal notranslate'>test</code> <em>module</em> <b>markup</b>.</p>
     html_plain: |-
       <p>This is a <code>test</code> <em>module</em> <b>markup</b>.</p>
     md: |-
-      This is a <code>test</code> <em>module</em> <b>markup</b>.
+      This is a <code>test</code> <em>module</em> <b>markup</b>\.
     rst: |-
       This is a \ :literal:`test`\  \ :emphasis:`module`\  \ :strong:`markup`\ .
     ansible_doc_text: This is a `test' `module' *markup*.
     rst_plain: This is a \ :literal:`test`\  \ :emphasis:`module`\  \ :strong:`markup`\
       .
   module:
     source: |-
@@ -43,15 +43,15 @@
       pluginLink.js: |-
         (plugin_data) => `https://docs.ansible.com/ansible/devel/collections/${plugin_data.fqcn.replace(/\./g, '/')}_${plugin_data.type}.html`
       pluginLink.py: |-
         lambda plugin_data: f"https://docs.ansible.com/ansible/devel/collections/{plugin_data.fqcn.replace('.', '/')}_{plugin_data.type}.html"
     html_plain: |-
       <p>The <a href='https://docs.ansible.com/ansible/devel/collections/a/b/c_module.html'>a.b.c</a> module.</p>
     md: |-
-      The [a.b.c](https\://docs.ansible.com/ansible/devel/collections/a/b/c\_module.html) module.
+      The [a\.b\.c](https\://docs\.ansible\.com/ansible/devel/collections/a/b/c\_module\.html) module\.
     md_opts:
       pluginLink.js: |-
         (plugin_data) => `https://docs.ansible.com/ansible/devel/collections/${plugin_data.fqcn.replace(/\./g, '/')}_${plugin_data.type}.html`
       pluginLink.py: |-
         lambda plugin_data: f"https://docs.ansible.com/ansible/devel/collections/{plugin_data.fqcn.replace('.', '/')}_{plugin_data.type}.html"
     rst: |-
       The \ :ref:`a.b.c <ansible_collections.a.b.c_module>`\  module.
@@ -61,15 +61,15 @@
     source: |-
       The M(a.b.c) module.
     html: |-
       <p>The <span class='module'>a.b.c</span> module.</p>
     html_plain: |-
       <p>The <span>a.b.c</span> module.</p>
     md: |-
-      The a.b.c module.
+      The a\.b\.c module\.
     rst: |-
       The \ :ref:`a.b.c <ansible_collections.a.b.c_module>`\  module.
     ansible_doc_text: The [a.b.c] module.
     rst_plain: The \ :ref:`a.b.c <ansible_collections.a.b.c_module>`\  module.
   plugin:
     source: |-
       The P(a.b.c#lookup) lookup plugin.
@@ -79,15 +79,15 @@
       pluginLink.js: |-
         (plugin_data) => `https://docs.ansible.com/ansible/devel/collections/${plugin_data.fqcn.replace(/\./g, '/')}_${plugin_data.type}.html`
       pluginLink.py: |-
         lambda plugin_data: f"https://docs.ansible.com/ansible/devel/collections/{plugin_data.fqcn.replace('.', '/')}_{plugin_data.type}.html"
     html_plain: |-
       <p>The <a href='https://docs.ansible.com/ansible/devel/collections/a/b/c_lookup.html'>a.b.c</a> lookup plugin.</p>
     md: |-
-      The [a.b.c](https\://docs.ansible.com/ansible/devel/collections/a/b/c\_lookup.html) lookup plugin.
+      The [a\.b\.c](https\://docs\.ansible\.com/ansible/devel/collections/a/b/c\_lookup\.html) lookup plugin\.
     md_opts:
       pluginLink.js: |-
         (plugin_data) => `https://docs.ansible.com/ansible/devel/collections/${plugin_data.fqcn.replace(/\./g, '/')}_${plugin_data.type}.html`
       pluginLink.py: |-
         lambda plugin_data: f"https://docs.ansible.com/ansible/devel/collections/{plugin_data.fqcn.replace('.', '/')}_{plugin_data.type}.html"
     rst: |-
       The \ :ref:`a.b.c <ansible_collections.a.b.c_lookup>`\  lookup plugin.
@@ -97,42 +97,57 @@
     source: |-
       The P(a.b.c#lookup) lookup plugin.
     html: |-
       <p>The <span class='module'>a.b.c</span> lookup plugin.</p>
     html_plain: |-
       <p>The <span>a.b.c</span> lookup plugin.</p>
     md: |-
-      The a.b.c lookup plugin.
+      The a\.b\.c lookup plugin\.
     rst: |-
       The \ :ref:`a.b.c <ansible_collections.a.b.c_lookup>`\  lookup plugin.
     ansible_doc_text: The [a.b.c] lookup plugin.
     rst_plain: The \ :ref:`a.b.c <ansible_collections.a.b.c_lookup>`\  lookup plugin.
   link_and_url:
     source: |-
       An URL U(https://example.com) and L(a link, https://example.org).
+      With special characters: U(https://example.com/test.html?foo=b<a>r&find=\*#baz.bam%3Dboo)
+      and L(mee.boo, https://example.org/test.html?foo=b<a>r&find=\*#baz.bam%3Dboo)
     html: |-
-      <p>An URL <a href='https://example.com'>https://example.com</a> and <a href='https://example.org'>a link</a>.</p>
+      <p>An URL <a href='https://example.com'>https://example.com</a> and <a href='https://example.org'>a link</a>.
+      With special characters: <a href='https://example.com/test.html?foo=b%3Ca%3Er&amp;find=%5C*#baz.bam%253Dboo'>https://example.com/test.html?foo=b%3Ca%3Er&amp;find=%5C*#baz.bam%253Dboo</a>
+      and <a href='https://example.org/test.html?foo=b%3Ca%3Er&amp;find=%5C*#baz.bam%253Dboo'>mee.boo</a></p>
     html_plain: |-
-      <p>An URL <a href='https://example.com'>https://example.com</a> and <a href='https://example.org'>a link</a>.</p>
+      <p>An URL <a href='https://example.com'>https://example.com</a> and <a href='https://example.org'>a link</a>.
+      With special characters: <a href='https://example.com/test.html?foo=b%3Ca%3Er&amp;find=%5C*#baz.bam%253Dboo'>https://example.com/test.html?foo=b%3Ca%3Er&amp;find=%5C*#baz.bam%253Dboo</a>
+      and <a href='https://example.org/test.html?foo=b%3Ca%3Er&amp;find=%5C*#baz.bam%253Dboo'>mee.boo</a></p>
     md: |-
-      An URL [https\://example.com](https\://example.com) and [a link](https\://example.org).
+      An URL [https\://example\.com](https://example.com) and [a link](https://example.org)\.
+      With special characters\: [https\://example\.com/test\.html\?foo\=b\%3Ca\%3Er\&find\=\%5C\*\#baz\.bam\%253Dboo](https://example.com/test.html?foo=b%3Ca%3Er&find=%5C*#baz.bam%253Dboo)
+      and [mee\.boo](https://example.org/test.html?foo=b%3Ca%3Er&find=%5C*#baz.bam%253Dboo)
     rst: |-
       An URL \ https://example.com\  and \ `a link <https://example.org>`__\ .
-    ansible_doc_text: An URL https://example.com and a link <https://example.org>.
-    rst_plain: An URL \ https://example.com\  and \ `a link <https://example.org>`__\
-      .
+      With special characters: \ https://example.com/test.html?foo=b%3Ca%3Er&find=%5C*#baz.bam%253Dboo\ 
+      and \ `mee.boo <https://example.org/test.html?foo=b%3Ca%3Er&find=%5C*#baz.bam%253Dboo>`__\ 
+    ansible_doc_text: |-
+      An URL https://example.com and a link <https://example.org>.
+      With special characters: https://example.com/test.html?foo=b<a>r&find=\*#baz.bam%3Dboo
+      and mee.boo <https://example.org/test.html?foo=b<a>r&find=\*#baz.bam%3Dboo>
+    rst_plain: |-
+      An URL \ https://example.com\  and \ `a link <https://example.org>`__\ .
+      With special characters: \ https://example.com/test.html?foo=b%3Ca%3Er&find=%5C*#baz.bam%253Dboo\ 
+      and \ `mee.boo <https://example.org/test.html?foo=b%3Ca%3Er&find=%5C*#baz.bam%253Dboo>`__\ 
   rst_ref:
     source: |-
       A R(RST reference, ansible_collections.community.general.ufw_module).
     html: |-
       <p>A <span class='module'>RST reference</span>.</p>
     html_plain: |-
       <p>A <span>RST reference</span>.</p>
     md: |-
-      A RST reference.
+      A RST reference\.
     rst: |-
       A \ :ref:`RST reference <ansible_collections.community.general.ufw_module>`\ .
     ansible_doc_text: A RST reference.
     rst_plain: A \ :ref:`RST reference <ansible_collections.community.general.ufw_module>`\
       .
   horizontal_line:
     source: |-
@@ -165,15 +180,15 @@
     source: |-
       foo E(FOOBAR) bar P(foo.bar.baz#bam) has value V( foo\),bar\\bam ).
     html: |-
       <p>foo <code class="xref std std-envvar literal notranslate">FOOBAR</code> bar <span class='module'>foo.bar.baz</span> has value <code class="ansible-value literal notranslate"> foo),bar\bam </code>.</p>
     html_plain: |-
       <p>foo <code>FOOBAR</code> bar <span>foo.bar.baz</span> has value <code> foo),bar\bam </code>.</p>
     md: |-
-      foo <code>FOOBAR</code> bar foo.bar.baz has value <code> foo\)\,bar\\bam </code>.
+      foo <code>FOOBAR</code> bar foo\.bar\.baz has value <code> foo\)\,bar\\bam </code>\.
     rst: |-
       foo \ :envvar:`FOOBAR`\  bar \ :ref:`foo.bar.baz <ansible_collections.foo.bar.baz_bam>`\  has value \ :ansval:`\  foo),bar\\bam \ `\ .
     ansible_doc_text: foo `FOOBAR' bar [foo.bar.baz] has value ` foo),bar\bam '.
     rst_plain: foo \ :envvar:`FOOBAR`\  bar \ :ref:`foo.bar.baz <ansible_collections.foo.bar.baz_bam>`\  has
       value \ :literal:`\  foo),bar\\bam \ `\ .
   option_name_no_current_plugin:
     source:
@@ -202,37 +217,37 @@
       - |-
         O(ignore:foo=bar) O(ignore:bar.baz[123].bam[len(x\) - 1]=bar)
     html: |-
       <p><code class="ansible-option literal notranslate"><strong>foo</strong></code> <code class="ansible-option literal notranslate"><strong>bar.baz[123].bam[len(x) - 1]</strong></code></p><p><code class="ansible-option-value literal notranslate">foo=</code> <code class="ansible-option-value literal notranslate">bar.baz[123].bam[len(x) - 1]=</code></p><p><code class="ansible-option-value literal notranslate">foo=bar</code> <code class="ansible-option-value literal notranslate">bar.baz[123].bam[len(x) - 1]=bar</code></p><p><code class="ansible-option literal notranslate"><strong>foo</strong></code> <code class="ansible-option literal notranslate"><strong>bar.baz[123].bam[len(x) - 1]</strong></code></p><p><code class="ansible-option-value literal notranslate">foo=</code> <code class="ansible-option-value literal notranslate">bar.baz[123].bam[len(x) - 1]=</code></p><p><code class="ansible-option-value literal notranslate">foo=bar</code> <code class="ansible-option-value literal notranslate">bar.baz[123].bam[len(x) - 1]=bar</code></p><p><code class="ansible-option literal notranslate"><strong>foo</strong></code> <code class="ansible-option literal notranslate"><strong>bar.baz[123].bam[len(x) - 1]</strong></code></p><p><code class="ansible-option-value literal notranslate">foo=</code> <code class="ansible-option-value literal notranslate">bar.baz[123].bam[len(x) - 1]=</code></p><p><code class="ansible-option-value literal notranslate">foo=bar</code> <code class="ansible-option-value literal notranslate">bar.baz[123].bam[len(x) - 1]=bar</code></p><p><code class="ansible-option literal notranslate"><strong>foo</strong></code> <code class="ansible-option literal notranslate"><strong>bar.baz[123].bam[len(x) - 1]</strong></code></p><p><code class="ansible-option-value literal notranslate">foo=</code> <code class="ansible-option-value literal notranslate">bar.baz[123].bam[len(x) - 1]=</code></p><p><code class="ansible-option-value literal notranslate">foo=bar</code> <code class="ansible-option-value literal notranslate">bar.baz[123].bam[len(x) - 1]=bar</code></p>
     html_plain: |-
       <p><code><strong>foo</strong></code> <code><strong>bar.baz[123].bam[len(x) - 1]</strong></code></p><p><code>foo=</code> <code>bar.baz[123].bam[len(x) - 1]=</code></p><p><code>foo=bar</code> <code>bar.baz[123].bam[len(x) - 1]=bar</code></p><p><code><strong>foo</strong></code> <code><strong>bar.baz[123].bam[len(x) - 1]</strong></code></p><p><code>foo=</code> <code>bar.baz[123].bam[len(x) - 1]=</code></p><p><code>foo=bar</code> <code>bar.baz[123].bam[len(x) - 1]=bar</code></p><p><code><strong>foo</strong></code> <code><strong>bar.baz[123].bam[len(x) - 1]</strong></code></p><p><code>foo=</code> <code>bar.baz[123].bam[len(x) - 1]=</code></p><p><code>foo=bar</code> <code>bar.baz[123].bam[len(x) - 1]=bar</code></p><p><code><strong>foo</strong></code> <code><strong>bar.baz[123].bam[len(x) - 1]</strong></code></p><p><code>foo=</code> <code>bar.baz[123].bam[len(x) - 1]=</code></p><p><code>foo=bar</code> <code>bar.baz[123].bam[len(x) - 1]=bar</code></p>
     md: |-
-      <code><strong>foo</strong></code> <code><strong>bar.baz\[123\].bam\[len\(x\) \- 1\]</strong></code>
+      <code><strong>foo</strong></code> <code><strong>bar\.baz\[123\]\.bam\[len\(x\) \- 1\]</strong></code>
 
-      <code>foo\=</code> <code>bar.baz\[123\].bam\[len\(x\) \- 1\]\=</code>
+      <code>foo\=</code> <code>bar\.baz\[123\]\.bam\[len\(x\) \- 1\]\=</code>
 
-      <code>foo\=bar</code> <code>bar.baz\[123\].bam\[len\(x\) \- 1\]\=bar</code>
+      <code>foo\=bar</code> <code>bar\.baz\[123\]\.bam\[len\(x\) \- 1\]\=bar</code>
 
-      <code><strong>foo</strong></code> <code><strong>bar.baz\[123\].bam\[len\(x\) \- 1\]</strong></code>
+      <code><strong>foo</strong></code> <code><strong>bar\.baz\[123\]\.bam\[len\(x\) \- 1\]</strong></code>
 
-      <code>foo\=</code> <code>bar.baz\[123\].bam\[len\(x\) \- 1\]\=</code>
+      <code>foo\=</code> <code>bar\.baz\[123\]\.bam\[len\(x\) \- 1\]\=</code>
 
-      <code>foo\=bar</code> <code>bar.baz\[123\].bam\[len\(x\) \- 1\]\=bar</code>
+      <code>foo\=bar</code> <code>bar\.baz\[123\]\.bam\[len\(x\) \- 1\]\=bar</code>
 
-      <code><strong>foo</strong></code> <code><strong>bar.baz\[123\].bam\[len\(x\) \- 1\]</strong></code>
+      <code><strong>foo</strong></code> <code><strong>bar\.baz\[123\]\.bam\[len\(x\) \- 1\]</strong></code>
 
-      <code>foo\=</code> <code>bar.baz\[123\].bam\[len\(x\) \- 1\]\=</code>
+      <code>foo\=</code> <code>bar\.baz\[123\]\.bam\[len\(x\) \- 1\]\=</code>
 
-      <code>foo\=bar</code> <code>bar.baz\[123\].bam\[len\(x\) \- 1\]\=bar</code>
+      <code>foo\=bar</code> <code>bar\.baz\[123\]\.bam\[len\(x\) \- 1\]\=bar</code>
 
-      <code><strong>foo</strong></code> <code><strong>bar.baz\[123\].bam\[len\(x\) \- 1\]</strong></code>
+      <code><strong>foo</strong></code> <code><strong>bar\.baz\[123\]\.bam\[len\(x\) \- 1\]</strong></code>
 
-      <code>foo\=</code> <code>bar.baz\[123\].bam\[len\(x\) \- 1\]\=</code>
+      <code>foo\=</code> <code>bar\.baz\[123\]\.bam\[len\(x\) \- 1\]\=</code>
 
-      <code>foo\=bar</code> <code>bar.baz\[123\].bam\[len\(x\) \- 1\]\=bar</code>
+      <code>foo\=bar</code> <code>bar\.baz\[123\]\.bam\[len\(x\) \- 1\]\=bar</code>
     rst: |-
       \ :ansopt:`foo`\  \ :ansopt:`bar.baz[123].bam[len(x) - 1]`\ 
 
       \ :ansopt:`foo=`\  \ :ansopt:`bar.baz[123].bam[len(x) - 1]=`\ 
 
       \ :ansopt:`foo=bar`\  \ :ansopt:`bar.baz[123].bam[len(x) - 1]=bar`\ 
 
@@ -328,37 +343,37 @@
       - |-
         O(ignore:foo=bar) O(ignore:bar.baz[123].bam[len(x\) - 1]=bar)
     html: |-
       <p><code class="ansible-option literal notranslate"><strong>foo</strong></code> <code class="ansible-option literal notranslate"><strong>bar.baz[123].bam[len(x) - 1]</strong></code></p><p><code class="ansible-option-value literal notranslate">foo=</code> <code class="ansible-option-value literal notranslate">bar.baz[123].bam[len(x) - 1]=</code></p><p><code class="ansible-option-value literal notranslate">foo=bar</code> <code class="ansible-option-value literal notranslate">bar.baz[123].bam[len(x) - 1]=bar</code></p><p><code class="ansible-option literal notranslate"><strong>foo</strong></code> <code class="ansible-option literal notranslate"><strong>bar.baz[123].bam[len(x) - 1]</strong></code></p><p><code class="ansible-option-value literal notranslate">foo=</code> <code class="ansible-option-value literal notranslate">bar.baz[123].bam[len(x) - 1]=</code></p><p><code class="ansible-option-value literal notranslate">foo=bar</code> <code class="ansible-option-value literal notranslate">bar.baz[123].bam[len(x) - 1]=bar</code></p><p><code class="ansible-option literal notranslate"><strong>foo</strong></code> <code class="ansible-option literal notranslate"><strong>bar.baz[123].bam[len(x) - 1]</strong></code></p><p><code class="ansible-option-value literal notranslate">foo=</code> <code class="ansible-option-value literal notranslate">bar.baz[123].bam[len(x) - 1]=</code></p><p><code class="ansible-option-value literal notranslate">foo=bar</code> <code class="ansible-option-value literal notranslate">bar.baz[123].bam[len(x) - 1]=bar</code></p><p><code class="ansible-option literal notranslate"><strong>foo</strong></code> <code class="ansible-option literal notranslate"><strong>bar.baz[123].bam[len(x) - 1]</strong></code></p><p><code class="ansible-option-value literal notranslate">foo=</code> <code class="ansible-option-value literal notranslate">bar.baz[123].bam[len(x) - 1]=</code></p><p><code class="ansible-option-value literal notranslate">foo=bar</code> <code class="ansible-option-value literal notranslate">bar.baz[123].bam[len(x) - 1]=bar</code></p>
     html_plain: |-
       <p><code><strong>foo</strong></code> <code><strong>bar.baz[123].bam[len(x) - 1]</strong></code></p><p><code>foo=</code> <code>bar.baz[123].bam[len(x) - 1]=</code></p><p><code>foo=bar</code> <code>bar.baz[123].bam[len(x) - 1]=bar</code></p><p><code><strong>foo</strong></code> <code><strong>bar.baz[123].bam[len(x) - 1]</strong></code></p><p><code>foo=</code> <code>bar.baz[123].bam[len(x) - 1]=</code></p><p><code>foo=bar</code> <code>bar.baz[123].bam[len(x) - 1]=bar</code></p><p><code><strong>foo</strong></code> <code><strong>bar.baz[123].bam[len(x) - 1]</strong></code></p><p><code>foo=</code> <code>bar.baz[123].bam[len(x) - 1]=</code></p><p><code>foo=bar</code> <code>bar.baz[123].bam[len(x) - 1]=bar</code></p><p><code><strong>foo</strong></code> <code><strong>bar.baz[123].bam[len(x) - 1]</strong></code></p><p><code>foo=</code> <code>bar.baz[123].bam[len(x) - 1]=</code></p><p><code>foo=bar</code> <code>bar.baz[123].bam[len(x) - 1]=bar</code></p>
     md: |-
-      <code><strong>foo</strong></code> <code><strong>bar.baz\[123\].bam\[len\(x\) \- 1\]</strong></code>
+      <code><strong>foo</strong></code> <code><strong>bar\.baz\[123\]\.bam\[len\(x\) \- 1\]</strong></code>
 
-      <code>foo\=</code> <code>bar.baz\[123\].bam\[len\(x\) \- 1\]\=</code>
+      <code>foo\=</code> <code>bar\.baz\[123\]\.bam\[len\(x\) \- 1\]\=</code>
 
-      <code>foo\=bar</code> <code>bar.baz\[123\].bam\[len\(x\) \- 1\]\=bar</code>
+      <code>foo\=bar</code> <code>bar\.baz\[123\]\.bam\[len\(x\) \- 1\]\=bar</code>
 
-      <code><strong>foo</strong></code> <code><strong>bar.baz\[123\].bam\[len\(x\) \- 1\]</strong></code>
+      <code><strong>foo</strong></code> <code><strong>bar\.baz\[123\]\.bam\[len\(x\) \- 1\]</strong></code>
 
-      <code>foo\=</code> <code>bar.baz\[123\].bam\[len\(x\) \- 1\]\=</code>
+      <code>foo\=</code> <code>bar\.baz\[123\]\.bam\[len\(x\) \- 1\]\=</code>
 
-      <code>foo\=bar</code> <code>bar.baz\[123\].bam\[len\(x\) \- 1\]\=bar</code>
+      <code>foo\=bar</code> <code>bar\.baz\[123\]\.bam\[len\(x\) \- 1\]\=bar</code>
 
-      <code><strong>foo</strong></code> <code><strong>bar.baz\[123\].bam\[len\(x\) \- 1\]</strong></code>
+      <code><strong>foo</strong></code> <code><strong>bar\.baz\[123\]\.bam\[len\(x\) \- 1\]</strong></code>
 
-      <code>foo\=</code> <code>bar.baz\[123\].bam\[len\(x\) \- 1\]\=</code>
+      <code>foo\=</code> <code>bar\.baz\[123\]\.bam\[len\(x\) \- 1\]\=</code>
 
-      <code>foo\=bar</code> <code>bar.baz\[123\].bam\[len\(x\) \- 1\]\=bar</code>
+      <code>foo\=bar</code> <code>bar\.baz\[123\]\.bam\[len\(x\) \- 1\]\=bar</code>
 
-      <code><strong>foo</strong></code> <code><strong>bar.baz\[123\].bam\[len\(x\) \- 1\]</strong></code>
+      <code><strong>foo</strong></code> <code><strong>bar\.baz\[123\]\.bam\[len\(x\) \- 1\]</strong></code>
 
-      <code>foo\=</code> <code>bar.baz\[123\].bam\[len\(x\) \- 1\]\=</code>
+      <code>foo\=</code> <code>bar\.baz\[123\]\.bam\[len\(x\) \- 1\]\=</code>
 
-      <code>foo\=bar</code> <code>bar.baz\[123\].bam\[len\(x\) \- 1\]\=bar</code>
+      <code>foo\=bar</code> <code>bar\.baz\[123\]\.bam\[len\(x\) \- 1\]\=bar</code>
     rst: |-
       \ :ansopt:`foo.bar.baz.bam#boo:foo`\  \ :ansopt:`foo.bar.baz.bam#boo:bar.baz[123].bam[len(x) - 1]`\ 
 
       \ :ansopt:`foo.bar.baz.bam#boo:foo=`\  \ :ansopt:`foo.bar.baz.bam#boo:bar.baz[123].bam[len(x) - 1]=`\ 
 
       \ :ansopt:`foo.bar.baz.bam#boo:foo=bar`\  \ :ansopt:`foo.bar.baz.bam#boo:bar.baz[123].bam[len(x) - 1]=bar`\ 
 
@@ -376,15 +391,15 @@
 
       \ :ansopt:`foo`\  \ :ansopt:`bar.baz[123].bam[len(x) - 1]`\ 
 
       \ :ansopt:`foo=`\  \ :ansopt:`bar.baz[123].bam[len(x) - 1]=`\ 
 
       \ :ansopt:`foo=bar`\  \ :ansopt:`bar.baz[123].bam[len(x) - 1]=bar`\ 
     parse_opts:
-      current_plugin:
+      currentPlugin:
         fqcn: foo.bar.baz.bam
         type: boo
     ansible_doc_text: |-
       `foo' (of boo plugin foo.bar.baz.bam) `bar.baz[123].bam[len(x) - 1]' (of boo plugin foo.bar.baz.bam)
 
       `foo=' (of boo plugin foo.bar.baz.bam) `bar.baz[123].bam[len(x) - 1]=' (of boo plugin foo.bar.baz.bam)
 
@@ -464,43 +479,43 @@
       - |-
         O(ignore:foo=bar) O(ignore:bar.baz[123].bam[len(x\) - 1]=bar)
     html: |-
       <p><code class="ansible-option literal notranslate"><strong>foo</strong></code> <code class="ansible-option literal notranslate"><strong>bar.baz[123].bam[len(x) - 1]</strong></code></p><p><code class="ansible-option-value literal notranslate">foo=</code> <code class="ansible-option-value literal notranslate">bar.baz[123].bam[len(x) - 1]=</code></p><p><code class="ansible-option-value literal notranslate">foo=bar</code> <code class="ansible-option-value literal notranslate">bar.baz[123].bam[len(x) - 1]=bar</code></p><p><code class="ansible-option literal notranslate"><strong>foo</strong></code> <code class="ansible-option literal notranslate"><strong>bar.baz[123].bam[len(x) - 1]</strong></code></p><p><code class="ansible-option-value literal notranslate">foo=</code> <code class="ansible-option-value literal notranslate">bar.baz[123].bam[len(x) - 1]=</code></p><p><code class="ansible-option-value literal notranslate">foo=bar</code> <code class="ansible-option-value literal notranslate">bar.baz[123].bam[len(x) - 1]=bar</code></p><p><code class="ansible-option literal notranslate"><strong>foo</strong></code> <code class="ansible-option literal notranslate"><strong>bar.baz[123].bam[len(x) - 1]</strong></code></p><p><code class="ansible-option-value literal notranslate">foo=</code> <code class="ansible-option-value literal notranslate">bar.baz[123].bam[len(x) - 1]=</code></p><p><code class="ansible-option-value literal notranslate">foo=bar</code> <code class="ansible-option-value literal notranslate">bar.baz[123].bam[len(x) - 1]=bar</code></p><p><code class="ansible-option literal notranslate"><strong>foo</strong></code> <code class="ansible-option literal notranslate"><strong>bar.baz[123].bam[len(x) - 1]</strong></code></p><p><code class="ansible-option-value literal notranslate">foo=</code> <code class="ansible-option-value literal notranslate">bar.baz[123].bam[len(x) - 1]=</code></p><p><code class="ansible-option-value literal notranslate">foo=bar</code> <code class="ansible-option-value literal notranslate">bar.baz[123].bam[len(x) - 1]=bar</code></p><p><code class="ansible-option literal notranslate"><strong>foo</strong></code> <code class="ansible-option literal notranslate"><strong>bar.baz[123].bam[len(x) - 1]</strong></code></p><p><code class="ansible-option-value literal notranslate">foo=</code> <code class="ansible-option-value literal notranslate">bar.baz[123].bam[len(x) - 1]=</code></p><p><code class="ansible-option-value literal notranslate">foo=bar</code> <code class="ansible-option-value literal notranslate">bar.baz[123].bam[len(x) - 1]=bar</code></p>
     html_plain: |-
       <p><code><strong>foo</strong></code> <code><strong>bar.baz[123].bam[len(x) - 1]</strong></code></p><p><code>foo=</code> <code>bar.baz[123].bam[len(x) - 1]=</code></p><p><code>foo=bar</code> <code>bar.baz[123].bam[len(x) - 1]=bar</code></p><p><code><strong>foo</strong></code> <code><strong>bar.baz[123].bam[len(x) - 1]</strong></code></p><p><code>foo=</code> <code>bar.baz[123].bam[len(x) - 1]=</code></p><p><code>foo=bar</code> <code>bar.baz[123].bam[len(x) - 1]=bar</code></p><p><code><strong>foo</strong></code> <code><strong>bar.baz[123].bam[len(x) - 1]</strong></code></p><p><code>foo=</code> <code>bar.baz[123].bam[len(x) - 1]=</code></p><p><code>foo=bar</code> <code>bar.baz[123].bam[len(x) - 1]=bar</code></p><p><code><strong>foo</strong></code> <code><strong>bar.baz[123].bam[len(x) - 1]</strong></code></p><p><code>foo=</code> <code>bar.baz[123].bam[len(x) - 1]=</code></p><p><code>foo=bar</code> <code>bar.baz[123].bam[len(x) - 1]=bar</code></p><p><code><strong>foo</strong></code> <code><strong>bar.baz[123].bam[len(x) - 1]</strong></code></p><p><code>foo=</code> <code>bar.baz[123].bam[len(x) - 1]=</code></p><p><code>foo=bar</code> <code>bar.baz[123].bam[len(x) - 1]=bar</code></p>
     md: |-
-      <code><strong>foo</strong></code> <code><strong>bar.baz\[123\].bam\[len\(x\) \- 1\]</strong></code>
+      <code><strong>foo</strong></code> <code><strong>bar\.baz\[123\]\.bam\[len\(x\) \- 1\]</strong></code>
 
-      <code>foo\=</code> <code>bar.baz\[123\].bam\[len\(x\) \- 1\]\=</code>
+      <code>foo\=</code> <code>bar\.baz\[123\]\.bam\[len\(x\) \- 1\]\=</code>
 
-      <code>foo\=bar</code> <code>bar.baz\[123\].bam\[len\(x\) \- 1\]\=bar</code>
+      <code>foo\=bar</code> <code>bar\.baz\[123\]\.bam\[len\(x\) \- 1\]\=bar</code>
 
-      <code><strong>foo</strong></code> <code><strong>bar.baz\[123\].bam\[len\(x\) \- 1\]</strong></code>
+      <code><strong>foo</strong></code> <code><strong>bar\.baz\[123\]\.bam\[len\(x\) \- 1\]</strong></code>
 
-      <code>foo\=</code> <code>bar.baz\[123\].bam\[len\(x\) \- 1\]\=</code>
+      <code>foo\=</code> <code>bar\.baz\[123\]\.bam\[len\(x\) \- 1\]\=</code>
 
-      <code>foo\=bar</code> <code>bar.baz\[123\].bam\[len\(x\) \- 1\]\=bar</code>
+      <code>foo\=bar</code> <code>bar\.baz\[123\]\.bam\[len\(x\) \- 1\]\=bar</code>
 
-      <code><strong>foo</strong></code> <code><strong>bar.baz\[123\].bam\[len\(x\) \- 1\]</strong></code>
+      <code><strong>foo</strong></code> <code><strong>bar\.baz\[123\]\.bam\[len\(x\) \- 1\]</strong></code>
 
-      <code>foo\=</code> <code>bar.baz\[123\].bam\[len\(x\) \- 1\]\=</code>
+      <code>foo\=</code> <code>bar\.baz\[123\]\.bam\[len\(x\) \- 1\]\=</code>
 
-      <code>foo\=bar</code> <code>bar.baz\[123\].bam\[len\(x\) \- 1\]\=bar</code>
+      <code>foo\=bar</code> <code>bar\.baz\[123\]\.bam\[len\(x\) \- 1\]\=bar</code>
 
-      <code><strong>foo</strong></code> <code><strong>bar.baz\[123\].bam\[len\(x\) \- 1\]</strong></code>
+      <code><strong>foo</strong></code> <code><strong>bar\.baz\[123\]\.bam\[len\(x\) \- 1\]</strong></code>
 
-      <code>foo\=</code> <code>bar.baz\[123\].bam\[len\(x\) \- 1\]\=</code>
+      <code>foo\=</code> <code>bar\.baz\[123\]\.bam\[len\(x\) \- 1\]\=</code>
 
-      <code>foo\=bar</code> <code>bar.baz\[123\].bam\[len\(x\) \- 1\]\=bar</code>
+      <code>foo\=bar</code> <code>bar\.baz\[123\]\.bam\[len\(x\) \- 1\]\=bar</code>
 
-      <code><strong>foo</strong></code> <code><strong>bar.baz\[123\].bam\[len\(x\) \- 1\]</strong></code>
+      <code><strong>foo</strong></code> <code><strong>bar\.baz\[123\]\.bam\[len\(x\) \- 1\]</strong></code>
 
-      <code>foo\=</code> <code>bar.baz\[123\].bam\[len\(x\) \- 1\]\=</code>
+      <code>foo\=</code> <code>bar\.baz\[123\]\.bam\[len\(x\) \- 1\]\=</code>
 
-      <code>foo\=bar</code> <code>bar.baz\[123\].bam\[len\(x\) \- 1\]\=bar</code>
+      <code>foo\=bar</code> <code>bar\.baz\[123\]\.bam\[len\(x\) \- 1\]\=bar</code>
     rst: |-
       \ :ansopt:`foo.bar.baz#role:main:foo`\  \ :ansopt:`foo.bar.baz#role:main:bar.baz[123].bam[len(x) - 1]`\ 
 
       \ :ansopt:`foo.bar.baz#role:main:foo=`\  \ :ansopt:`foo.bar.baz#role:main:bar.baz[123].bam[len(x) - 1]=`\ 
 
       \ :ansopt:`foo.bar.baz#role:main:foo=bar`\  \ :ansopt:`foo.bar.baz#role:main:bar.baz[123].bam[len(x) - 1]=bar`\ 
 
@@ -524,18 +539,18 @@
 
       \ :ansopt:`foo`\  \ :ansopt:`bar.baz[123].bam[len(x) - 1]`\ 
 
       \ :ansopt:`foo=`\  \ :ansopt:`bar.baz[123].bam[len(x) - 1]=`\ 
 
       \ :ansopt:`foo=bar`\  \ :ansopt:`bar.baz[123].bam[len(x) - 1]=bar`\ 
     parse_opts:
-      current_plugin:
+      currentPlugin:
         fqcn: foo.bar.baz
         type: role
-      role_entrypoint: main
+      roleEntrypoint: main
     ansible_doc_text: |-
       `foo' (of role foo.bar.baz, main entrypoint) `bar.baz[123].bam[len(x) - 1]' (of role foo.bar.baz, main entrypoint)
 
       `foo=' (of role foo.bar.baz, main entrypoint) `bar.baz[123].bam[len(x) - 1]=' (of role foo.bar.baz, main entrypoint)
 
       `foo=bar' (of role foo.bar.baz, main entrypoint) `bar.baz[123].bam[len(x) - 1]=bar' (of role foo.bar.baz, main entrypoint)
 
@@ -624,37 +639,37 @@
       pluginOptionLikeLink.js: |-
         (plugin, entrypoint, what, name, current_plugin) => `https://docs.ansible.com/ansible/devel/collections/${plugin.fqcn.replace(/\./g, '/')}_${plugin.type}.html#${what}${entrypoint ? '-' + entrypoint : ''}-${name.join('/')}`
       pluginOptionLikeLink.py: |-
         lambda plugin, entrypoint, what, name, current_plugin: f"https://docs.ansible.com/ansible/devel/collections/{plugin.fqcn.replace('.', '/')}_{plugin.type}.html#{what}{'-' + entrypoint if entrypoint else ''}-{'/'.join(name)}"
     html_plain: |-
       <p><code><strong>foo</strong></code> <code><strong>bar.baz[123].bam[len(x) - 1]</strong></code></p><p><code>foo=</code> <code>bar.baz[123].bam[len(x) - 1]=</code></p><p><code>foo=bar</code> <code>bar.baz[123].bam[len(x) - 1]=bar</code></p><p><code><strong><a href="https://docs.ansible.com/ansible/devel/collections/bam/baz/foo_lookup.html#option-foo">foo</a></strong></code> <code><strong><a href="https://docs.ansible.com/ansible/devel/collections/bam/baz/foo_lookup.html#option-bar/baz/bam">bar.baz[123].bam[len(x) - 1]</a></strong></code></p><p><code><a href="https://docs.ansible.com/ansible/devel/collections/bam/baz/foo_lookup.html#option-foo">foo=</a></code> <code><a href="https://docs.ansible.com/ansible/devel/collections/bam/baz/foo_lookup.html#option-bar/baz/bam">bar.baz[123].bam[len(x) - 1]=</a></code></p><p><code><a href="https://docs.ansible.com/ansible/devel/collections/bam/baz/foo_lookup.html#option-foo">foo=bar</a></code> <code><a href="https://docs.ansible.com/ansible/devel/collections/bam/baz/foo_lookup.html#option-bar/baz/bam">bar.baz[123].bam[len(x) - 1]=bar</a></code></p><p><code><strong><a href="https://docs.ansible.com/ansible/devel/collections/bam/baz/foo_role.html#option-main-foo">foo</a></strong></code> <code><strong><a href="https://docs.ansible.com/ansible/devel/collections/bam/baz/foo_role.html#option-main-bar/baz/bam">bar.baz[123].bam[len(x) - 1]</a></strong></code></p><p><code><a href="https://docs.ansible.com/ansible/devel/collections/bam/baz/foo_role.html#option-main-foo">foo=</a></code> <code><a href="https://docs.ansible.com/ansible/devel/collections/bam/baz/foo_role.html#option-main-bar/baz/bam">bar.baz[123].bam[len(x) - 1]=</a></code></p><p><code><a href="https://docs.ansible.com/ansible/devel/collections/bam/baz/foo_role.html#option-main-foo">foo=bar</a></code> <code><a href="https://docs.ansible.com/ansible/devel/collections/bam/baz/foo_role.html#option-main-bar/baz/bam">bar.baz[123].bam[len(x) - 1]=bar</a></code></p><p><code><strong>foo</strong></code> <code><strong>bar.baz[123].bam[len(x) - 1]</strong></code></p><p><code>foo=</code> <code>bar.baz[123].bam[len(x) - 1]=</code></p><p><code>foo=bar</code> <code>bar.baz[123].bam[len(x) - 1]=bar</code></p>
     md: |-
-      <code><strong>foo</strong></code> <code><strong>bar.baz\[123\].bam\[len\(x\) \- 1\]</strong></code>
+      <code><strong>foo</strong></code> <code><strong>bar\.baz\[123\]\.bam\[len\(x\) \- 1\]</strong></code>
 
-      <code>foo\=</code> <code>bar.baz\[123\].bam\[len\(x\) \- 1\]\=</code>
+      <code>foo\=</code> <code>bar\.baz\[123\]\.bam\[len\(x\) \- 1\]\=</code>
 
-      <code>foo\=bar</code> <code>bar.baz\[123\].bam\[len\(x\) \- 1\]\=bar</code>
+      <code>foo\=bar</code> <code>bar\.baz\[123\]\.bam\[len\(x\) \- 1\]\=bar</code>
 
-      <code><strong><a href="https\://docs.ansible.com/ansible/devel/collections/bam/baz/foo\_lookup.html\#option\-foo">foo</a></strong></code> <code><strong><a href="https\://docs.ansible.com/ansible/devel/collections/bam/baz/foo\_lookup.html\#option\-bar/baz/bam">bar.baz\[123\].bam\[len\(x\) \- 1\]</a></strong></code>
+      <code><strong><a href="https://docs.ansible.com/ansible/devel/collections/bam/baz/foo_lookup.html#option-foo">foo</a></strong></code> <code><strong><a href="https://docs.ansible.com/ansible/devel/collections/bam/baz/foo_lookup.html#option-bar/baz/bam">bar\.baz\[123\]\.bam\[len\(x\) \- 1\]</a></strong></code>
 
-      <code><a href="https\://docs.ansible.com/ansible/devel/collections/bam/baz/foo\_lookup.html\#option\-foo">foo\=</a></code> <code><a href="https\://docs.ansible.com/ansible/devel/collections/bam/baz/foo\_lookup.html\#option\-bar/baz/bam">bar.baz\[123\].bam\[len\(x\) \- 1\]\=</a></code>
+      <code><a href="https://docs.ansible.com/ansible/devel/collections/bam/baz/foo_lookup.html#option-foo">foo\=</a></code> <code><a href="https://docs.ansible.com/ansible/devel/collections/bam/baz/foo_lookup.html#option-bar/baz/bam">bar\.baz\[123\]\.bam\[len\(x\) \- 1\]\=</a></code>
 
-      <code><a href="https\://docs.ansible.com/ansible/devel/collections/bam/baz/foo\_lookup.html\#option\-foo">foo\=bar</a></code> <code><a href="https\://docs.ansible.com/ansible/devel/collections/bam/baz/foo\_lookup.html\#option\-bar/baz/bam">bar.baz\[123\].bam\[len\(x\) \- 1\]\=bar</a></code>
+      <code><a href="https://docs.ansible.com/ansible/devel/collections/bam/baz/foo_lookup.html#option-foo">foo\=bar</a></code> <code><a href="https://docs.ansible.com/ansible/devel/collections/bam/baz/foo_lookup.html#option-bar/baz/bam">bar\.baz\[123\]\.bam\[len\(x\) \- 1\]\=bar</a></code>
 
-      <code><strong><a href="https\://docs.ansible.com/ansible/devel/collections/bam/baz/foo\_role.html\#option\-main\-foo">foo</a></strong></code> <code><strong><a href="https\://docs.ansible.com/ansible/devel/collections/bam/baz/foo\_role.html\#option\-main\-bar/baz/bam">bar.baz\[123\].bam\[len\(x\) \- 1\]</a></strong></code>
+      <code><strong><a href="https://docs.ansible.com/ansible/devel/collections/bam/baz/foo_role.html#option-main-foo">foo</a></strong></code> <code><strong><a href="https://docs.ansible.com/ansible/devel/collections/bam/baz/foo_role.html#option-main-bar/baz/bam">bar\.baz\[123\]\.bam\[len\(x\) \- 1\]</a></strong></code>
 
-      <code><a href="https\://docs.ansible.com/ansible/devel/collections/bam/baz/foo\_role.html\#option\-main\-foo">foo\=</a></code> <code><a href="https\://docs.ansible.com/ansible/devel/collections/bam/baz/foo\_role.html\#option\-main\-bar/baz/bam">bar.baz\[123\].bam\[len\(x\) \- 1\]\=</a></code>
+      <code><a href="https://docs.ansible.com/ansible/devel/collections/bam/baz/foo_role.html#option-main-foo">foo\=</a></code> <code><a href="https://docs.ansible.com/ansible/devel/collections/bam/baz/foo_role.html#option-main-bar/baz/bam">bar\.baz\[123\]\.bam\[len\(x\) \- 1\]\=</a></code>
 
-      <code><a href="https\://docs.ansible.com/ansible/devel/collections/bam/baz/foo\_role.html\#option\-main\-foo">foo\=bar</a></code> <code><a href="https\://docs.ansible.com/ansible/devel/collections/bam/baz/foo\_role.html\#option\-main\-bar/baz/bam">bar.baz\[123\].bam\[len\(x\) \- 1\]\=bar</a></code>
+      <code><a href="https://docs.ansible.com/ansible/devel/collections/bam/baz/foo_role.html#option-main-foo">foo\=bar</a></code> <code><a href="https://docs.ansible.com/ansible/devel/collections/bam/baz/foo_role.html#option-main-bar/baz/bam">bar\.baz\[123\]\.bam\[len\(x\) \- 1\]\=bar</a></code>
 
-      <code><strong>foo</strong></code> <code><strong>bar.baz\[123\].bam\[len\(x\) \- 1\]</strong></code>
+      <code><strong>foo</strong></code> <code><strong>bar\.baz\[123\]\.bam\[len\(x\) \- 1\]</strong></code>
 
-      <code>foo\=</code> <code>bar.baz\[123\].bam\[len\(x\) \- 1\]\=</code>
+      <code>foo\=</code> <code>bar\.baz\[123\]\.bam\[len\(x\) \- 1\]\=</code>
 
-      <code>foo\=bar</code> <code>bar.baz\[123\].bam\[len\(x\) \- 1\]\=bar</code>
+      <code>foo\=bar</code> <code>bar\.baz\[123\]\.bam\[len\(x\) \- 1\]\=bar</code>
     md_opts:
       pluginOptionLikeLink.js: |-
         (plugin, entrypoint, what, name, current_plugin) => `https://docs.ansible.com/ansible/devel/collections/${plugin.fqcn.replace(/\./g, '/')}_${plugin.type}.html#${what}${entrypoint ? '-' + entrypoint : ''}-${name.join('/')}`
       pluginOptionLikeLink.py: |-
         lambda plugin, entrypoint, what, name, current_plugin: f"https://docs.ansible.com/ansible/devel/collections/{plugin.fqcn.replace('.', '/')}_{plugin.type}.html#{what}{'-' + entrypoint if entrypoint else ''}-{'/'.join(name)}"
     rst: |-
       \ :ansopt:`foo`\  \ :ansopt:`bar.baz[123].bam[len(x) - 1]`\ 
@@ -760,37 +775,37 @@
       pluginOptionLikeLink.js: |-
         (plugin, entrypoint, what, name, current_plugin) => `https://docs.ansible.com/ansible/devel/collections/${plugin.fqcn.replace(/\./g, '/')}_${plugin.type}.html#${what}${entrypoint ? '-' + entrypoint : ''}-${name.join('/')}`
       pluginOptionLikeLink.py: |-
         lambda plugin, entrypoint, what, name, current_plugin: f"https://docs.ansible.com/ansible/devel/collections/{plugin.fqcn.replace('.', '/')}_{plugin.type}.html#{what}{'-' + entrypoint if entrypoint else ''}-{'/'.join(name)}"
     html_plain: |-
       <p><code><strong><a href="https://docs.ansible.com/ansible/devel/collections/foo/bar/baz/bam_boo.html#option-foo">foo</a></strong></code> <code><strong><a href="https://docs.ansible.com/ansible/devel/collections/foo/bar/baz/bam_boo.html#option-bar/baz/bam">bar.baz[123].bam[len(x) - 1]</a></strong></code></p><p><code><a href="https://docs.ansible.com/ansible/devel/collections/foo/bar/baz/bam_boo.html#option-foo">foo=</a></code> <code><a href="https://docs.ansible.com/ansible/devel/collections/foo/bar/baz/bam_boo.html#option-bar/baz/bam">bar.baz[123].bam[len(x) - 1]=</a></code></p><p><code><a href="https://docs.ansible.com/ansible/devel/collections/foo/bar/baz/bam_boo.html#option-foo">foo=bar</a></code> <code><a href="https://docs.ansible.com/ansible/devel/collections/foo/bar/baz/bam_boo.html#option-bar/baz/bam">bar.baz[123].bam[len(x) - 1]=bar</a></code></p><p><code><strong><a href="https://docs.ansible.com/ansible/devel/collections/bam/baz/foo_lookup.html#option-foo">foo</a></strong></code> <code><strong><a href="https://docs.ansible.com/ansible/devel/collections/bam/baz/foo_lookup.html#option-bar/baz/bam">bar.baz[123].bam[len(x) - 1]</a></strong></code></p><p><code><a href="https://docs.ansible.com/ansible/devel/collections/bam/baz/foo_lookup.html#option-foo">foo=</a></code> <code><a href="https://docs.ansible.com/ansible/devel/collections/bam/baz/foo_lookup.html#option-bar/baz/bam">bar.baz[123].bam[len(x) - 1]=</a></code></p><p><code><a href="https://docs.ansible.com/ansible/devel/collections/bam/baz/foo_lookup.html#option-foo">foo=bar</a></code> <code><a href="https://docs.ansible.com/ansible/devel/collections/bam/baz/foo_lookup.html#option-bar/baz/bam">bar.baz[123].bam[len(x) - 1]=bar</a></code></p><p><code><strong><a href="https://docs.ansible.com/ansible/devel/collections/bam/baz/foo_role.html#option-main-foo">foo</a></strong></code> <code><strong><a href="https://docs.ansible.com/ansible/devel/collections/bam/baz/foo_role.html#option-main-bar/baz/bam">bar.baz[123].bam[len(x) - 1]</a></strong></code></p><p><code><a href="https://docs.ansible.com/ansible/devel/collections/bam/baz/foo_role.html#option-main-foo">foo=</a></code> <code><a href="https://docs.ansible.com/ansible/devel/collections/bam/baz/foo_role.html#option-main-bar/baz/bam">bar.baz[123].bam[len(x) - 1]=</a></code></p><p><code><a href="https://docs.ansible.com/ansible/devel/collections/bam/baz/foo_role.html#option-main-foo">foo=bar</a></code> <code><a href="https://docs.ansible.com/ansible/devel/collections/bam/baz/foo_role.html#option-main-bar/baz/bam">bar.baz[123].bam[len(x) - 1]=bar</a></code></p><p><code><strong>foo</strong></code> <code><strong>bar.baz[123].bam[len(x) - 1]</strong></code></p><p><code>foo=</code> <code>bar.baz[123].bam[len(x) - 1]=</code></p><p><code>foo=bar</code> <code>bar.baz[123].bam[len(x) - 1]=bar</code></p>
     md: |-
-      <code><strong><a href="https\://docs.ansible.com/ansible/devel/collections/foo/bar/baz/bam\_boo.html\#option\-foo">foo</a></strong></code> <code><strong><a href="https\://docs.ansible.com/ansible/devel/collections/foo/bar/baz/bam\_boo.html\#option\-bar/baz/bam">bar.baz\[123\].bam\[len\(x\) \- 1\]</a></strong></code>
+      <code><strong><a href="https://docs.ansible.com/ansible/devel/collections/foo/bar/baz/bam_boo.html#option-foo">foo</a></strong></code> <code><strong><a href="https://docs.ansible.com/ansible/devel/collections/foo/bar/baz/bam_boo.html#option-bar/baz/bam">bar\.baz\[123\]\.bam\[len\(x\) \- 1\]</a></strong></code>
 
-      <code><a href="https\://docs.ansible.com/ansible/devel/collections/foo/bar/baz/bam\_boo.html\#option\-foo">foo\=</a></code> <code><a href="https\://docs.ansible.com/ansible/devel/collections/foo/bar/baz/bam\_boo.html\#option\-bar/baz/bam">bar.baz\[123\].bam\[len\(x\) \- 1\]\=</a></code>
+      <code><a href="https://docs.ansible.com/ansible/devel/collections/foo/bar/baz/bam_boo.html#option-foo">foo\=</a></code> <code><a href="https://docs.ansible.com/ansible/devel/collections/foo/bar/baz/bam_boo.html#option-bar/baz/bam">bar\.baz\[123\]\.bam\[len\(x\) \- 1\]\=</a></code>
 
-      <code><a href="https\://docs.ansible.com/ansible/devel/collections/foo/bar/baz/bam\_boo.html\#option\-foo">foo\=bar</a></code> <code><a href="https\://docs.ansible.com/ansible/devel/collections/foo/bar/baz/bam\_boo.html\#option\-bar/baz/bam">bar.baz\[123\].bam\[len\(x\) \- 1\]\=bar</a></code>
+      <code><a href="https://docs.ansible.com/ansible/devel/collections/foo/bar/baz/bam_boo.html#option-foo">foo\=bar</a></code> <code><a href="https://docs.ansible.com/ansible/devel/collections/foo/bar/baz/bam_boo.html#option-bar/baz/bam">bar\.baz\[123\]\.bam\[len\(x\) \- 1\]\=bar</a></code>
 
-      <code><strong><a href="https\://docs.ansible.com/ansible/devel/collections/bam/baz/foo\_lookup.html\#option\-foo">foo</a></strong></code> <code><strong><a href="https\://docs.ansible.com/ansible/devel/collections/bam/baz/foo\_lookup.html\#option\-bar/baz/bam">bar.baz\[123\].bam\[len\(x\) \- 1\]</a></strong></code>
+      <code><strong><a href="https://docs.ansible.com/ansible/devel/collections/bam/baz/foo_lookup.html#option-foo">foo</a></strong></code> <code><strong><a href="https://docs.ansible.com/ansible/devel/collections/bam/baz/foo_lookup.html#option-bar/baz/bam">bar\.baz\[123\]\.bam\[len\(x\) \- 1\]</a></strong></code>
 
-      <code><a href="https\://docs.ansible.com/ansible/devel/collections/bam/baz/foo\_lookup.html\#option\-foo">foo\=</a></code> <code><a href="https\://docs.ansible.com/ansible/devel/collections/bam/baz/foo\_lookup.html\#option\-bar/baz/bam">bar.baz\[123\].bam\[len\(x\) \- 1\]\=</a></code>
+      <code><a href="https://docs.ansible.com/ansible/devel/collections/bam/baz/foo_lookup.html#option-foo">foo\=</a></code> <code><a href="https://docs.ansible.com/ansible/devel/collections/bam/baz/foo_lookup.html#option-bar/baz/bam">bar\.baz\[123\]\.bam\[len\(x\) \- 1\]\=</a></code>
 
-      <code><a href="https\://docs.ansible.com/ansible/devel/collections/bam/baz/foo\_lookup.html\#option\-foo">foo\=bar</a></code> <code><a href="https\://docs.ansible.com/ansible/devel/collections/bam/baz/foo\_lookup.html\#option\-bar/baz/bam">bar.baz\[123\].bam\[len\(x\) \- 1\]\=bar</a></code>
+      <code><a href="https://docs.ansible.com/ansible/devel/collections/bam/baz/foo_lookup.html#option-foo">foo\=bar</a></code> <code><a href="https://docs.ansible.com/ansible/devel/collections/bam/baz/foo_lookup.html#option-bar/baz/bam">bar\.baz\[123\]\.bam\[len\(x\) \- 1\]\=bar</a></code>
 
-      <code><strong><a href="https\://docs.ansible.com/ansible/devel/collections/bam/baz/foo\_role.html\#option\-main\-foo">foo</a></strong></code> <code><strong><a href="https\://docs.ansible.com/ansible/devel/collections/bam/baz/foo\_role.html\#option\-main\-bar/baz/bam">bar.baz\[123\].bam\[len\(x\) \- 1\]</a></strong></code>
+      <code><strong><a href="https://docs.ansible.com/ansible/devel/collections/bam/baz/foo_role.html#option-main-foo">foo</a></strong></code> <code><strong><a href="https://docs.ansible.com/ansible/devel/collections/bam/baz/foo_role.html#option-main-bar/baz/bam">bar\.baz\[123\]\.bam\[len\(x\) \- 1\]</a></strong></code>
 
-      <code><a href="https\://docs.ansible.com/ansible/devel/collections/bam/baz/foo\_role.html\#option\-main\-foo">foo\=</a></code> <code><a href="https\://docs.ansible.com/ansible/devel/collections/bam/baz/foo\_role.html\#option\-main\-bar/baz/bam">bar.baz\[123\].bam\[len\(x\) \- 1\]\=</a></code>
+      <code><a href="https://docs.ansible.com/ansible/devel/collections/bam/baz/foo_role.html#option-main-foo">foo\=</a></code> <code><a href="https://docs.ansible.com/ansible/devel/collections/bam/baz/foo_role.html#option-main-bar/baz/bam">bar\.baz\[123\]\.bam\[len\(x\) \- 1\]\=</a></code>
 
-      <code><a href="https\://docs.ansible.com/ansible/devel/collections/bam/baz/foo\_role.html\#option\-main\-foo">foo\=bar</a></code> <code><a href="https\://docs.ansible.com/ansible/devel/collections/bam/baz/foo\_role.html\#option\-main\-bar/baz/bam">bar.baz\[123\].bam\[len\(x\) \- 1\]\=bar</a></code>
+      <code><a href="https://docs.ansible.com/ansible/devel/collections/bam/baz/foo_role.html#option-main-foo">foo\=bar</a></code> <code><a href="https://docs.ansible.com/ansible/devel/collections/bam/baz/foo_role.html#option-main-bar/baz/bam">bar\.baz\[123\]\.bam\[len\(x\) \- 1\]\=bar</a></code>
 
-      <code><strong>foo</strong></code> <code><strong>bar.baz\[123\].bam\[len\(x\) \- 1\]</strong></code>
+      <code><strong>foo</strong></code> <code><strong>bar\.baz\[123\]\.bam\[len\(x\) \- 1\]</strong></code>
 
-      <code>foo\=</code> <code>bar.baz\[123\].bam\[len\(x\) \- 1\]\=</code>
+      <code>foo\=</code> <code>bar\.baz\[123\]\.bam\[len\(x\) \- 1\]\=</code>
 
-      <code>foo\=bar</code> <code>bar.baz\[123\].bam\[len\(x\) \- 1\]\=bar</code>
+      <code>foo\=bar</code> <code>bar\.baz\[123\]\.bam\[len\(x\) \- 1\]\=bar</code>
     md_opts:
       pluginOptionLikeLink.js: |-
         (plugin, entrypoint, what, name, current_plugin) => `https://docs.ansible.com/ansible/devel/collections/${plugin.fqcn.replace(/\./g, '/')}_${plugin.type}.html#${what}${entrypoint ? '-' + entrypoint : ''}-${name.join('/')}`
       pluginOptionLikeLink.py: |-
         lambda plugin, entrypoint, what, name, current_plugin: f"https://docs.ansible.com/ansible/devel/collections/{plugin.fqcn.replace('.', '/')}_{plugin.type}.html#{what}{'-' + entrypoint if entrypoint else ''}-{'/'.join(name)}"
     rst: |-
       \ :ansopt:`foo.bar.baz.bam#boo:foo`\  \ :ansopt:`foo.bar.baz.bam#boo:bar.baz[123].bam[len(x) - 1]`\ 
@@ -813,15 +828,15 @@
 
       \ :ansopt:`foo`\  \ :ansopt:`bar.baz[123].bam[len(x) - 1]`\ 
 
       \ :ansopt:`foo=`\  \ :ansopt:`bar.baz[123].bam[len(x) - 1]=`\ 
 
       \ :ansopt:`foo=bar`\  \ :ansopt:`bar.baz[123].bam[len(x) - 1]=bar`\ 
     parse_opts:
-      current_plugin:
+      currentPlugin:
         fqcn: foo.bar.baz.bam
         type: boo
     ansible_doc_text: |-
       `foo' (of boo plugin foo.bar.baz.bam) `bar.baz[123].bam[len(x) - 1]' (of boo plugin foo.bar.baz.bam)
 
       `foo=' (of boo plugin foo.bar.baz.bam) `bar.baz[123].bam[len(x) - 1]=' (of boo plugin foo.bar.baz.bam)
 
@@ -906,43 +921,43 @@
       pluginOptionLikeLink.js: |-
         (plugin, entrypoint, what, name, current_plugin) => `https://docs.ansible.com/ansible/devel/collections/${plugin.fqcn.replace(/\./g, '/')}_${plugin.type}.html#${what}${entrypoint ? '-' + entrypoint : ''}-${name.join('/')}`
       pluginOptionLikeLink.py: |-
         lambda plugin, entrypoint, what, name, current_plugin: f"https://docs.ansible.com/ansible/devel/collections/{plugin.fqcn.replace('.', '/')}_{plugin.type}.html#{what}{'-' + entrypoint if entrypoint else ''}-{'/'.join(name)}"
     html_plain: |-
       <p><code><strong><a href="https://docs.ansible.com/ansible/devel/collections/foo/bar/baz_role.html#option-main-foo">foo</a></strong></code> <code><strong><a href="https://docs.ansible.com/ansible/devel/collections/foo/bar/baz_role.html#option-main-bar/baz/bam">bar.baz[123].bam[len(x) - 1]</a></strong></code></p><p><code><a href="https://docs.ansible.com/ansible/devel/collections/foo/bar/baz_role.html#option-main-foo">foo=</a></code> <code><a href="https://docs.ansible.com/ansible/devel/collections/foo/bar/baz_role.html#option-main-bar/baz/bam">bar.baz[123].bam[len(x) - 1]=</a></code></p><p><code><a href="https://docs.ansible.com/ansible/devel/collections/foo/bar/baz_role.html#option-main-foo">foo=bar</a></code> <code><a href="https://docs.ansible.com/ansible/devel/collections/foo/bar/baz_role.html#option-main-bar/baz/bam">bar.baz[123].bam[len(x) - 1]=bar</a></code></p><p><code><strong><a href="https://docs.ansible.com/ansible/devel/collections/foo/bar/baz_role.html#option-other_entrypoint-foo">foo</a></strong></code> <code><strong><a href="https://docs.ansible.com/ansible/devel/collections/foo/bar/baz_role.html#option-other_entrypoint-bar/baz/bam">bar.baz[123].bam[len(x) - 1]</a></strong></code></p><p><code><a href="https://docs.ansible.com/ansible/devel/collections/foo/bar/baz_role.html#option-other_entrypoint-foo">foo=</a></code> <code><a href="https://docs.ansible.com/ansible/devel/collections/foo/bar/baz_role.html#option-other_entrypoint-bar/baz/bam">bar.baz[123].bam[len(x) - 1]=</a></code></p><p><code><a href="https://docs.ansible.com/ansible/devel/collections/foo/bar/baz_role.html#option-other_entrypoint-foo">foo=bar</a></code> <code><a href="https://docs.ansible.com/ansible/devel/collections/foo/bar/baz_role.html#option-other_entrypoint-bar/baz/bam">bar.baz[123].bam[len(x) - 1]=bar</a></code></p><p><code><strong><a href="https://docs.ansible.com/ansible/devel/collections/bam/baz/foo_lookup.html#option-foo">foo</a></strong></code> <code><strong><a href="https://docs.ansible.com/ansible/devel/collections/bam/baz/foo_lookup.html#option-bar/baz/bam">bar.baz[123].bam[len(x) - 1]</a></strong></code></p><p><code><a href="https://docs.ansible.com/ansible/devel/collections/bam/baz/foo_lookup.html#option-foo">foo=</a></code> <code><a href="https://docs.ansible.com/ansible/devel/collections/bam/baz/foo_lookup.html#option-bar/baz/bam">bar.baz[123].bam[len(x) - 1]=</a></code></p><p><code><a href="https://docs.ansible.com/ansible/devel/collections/bam/baz/foo_lookup.html#option-foo">foo=bar</a></code> <code><a href="https://docs.ansible.com/ansible/devel/collections/bam/baz/foo_lookup.html#option-bar/baz/bam">bar.baz[123].bam[len(x) - 1]=bar</a></code></p><p><code><strong><a href="https://docs.ansible.com/ansible/devel/collections/bam/baz/foo_role.html#option-main-foo">foo</a></strong></code> <code><strong><a href="https://docs.ansible.com/ansible/devel/collections/bam/baz/foo_role.html#option-main-bar/baz/bam">bar.baz[123].bam[len(x) - 1]</a></strong></code></p><p><code><a href="https://docs.ansible.com/ansible/devel/collections/bam/baz/foo_role.html#option-main-foo">foo=</a></code> <code><a href="https://docs.ansible.com/ansible/devel/collections/bam/baz/foo_role.html#option-main-bar/baz/bam">bar.baz[123].bam[len(x) - 1]=</a></code></p><p><code><a href="https://docs.ansible.com/ansible/devel/collections/bam/baz/foo_role.html#option-main-foo">foo=bar</a></code> <code><a href="https://docs.ansible.com/ansible/devel/collections/bam/baz/foo_role.html#option-main-bar/baz/bam">bar.baz[123].bam[len(x) - 1]=bar</a></code></p><p><code><strong>foo</strong></code> <code><strong>bar.baz[123].bam[len(x) - 1]</strong></code></p><p><code>foo=</code> <code>bar.baz[123].bam[len(x) - 1]=</code></p><p><code>foo=bar</code> <code>bar.baz[123].bam[len(x) - 1]=bar</code></p>
     md: |-
-      <code><strong><a href="https\://docs.ansible.com/ansible/devel/collections/foo/bar/baz\_role.html\#option\-main\-foo">foo</a></strong></code> <code><strong><a href="https\://docs.ansible.com/ansible/devel/collections/foo/bar/baz\_role.html\#option\-main\-bar/baz/bam">bar.baz\[123\].bam\[len\(x\) \- 1\]</a></strong></code>
+      <code><strong><a href="https://docs.ansible.com/ansible/devel/collections/foo/bar/baz_role.html#option-main-foo">foo</a></strong></code> <code><strong><a href="https://docs.ansible.com/ansible/devel/collections/foo/bar/baz_role.html#option-main-bar/baz/bam">bar\.baz\[123\]\.bam\[len\(x\) \- 1\]</a></strong></code>
 
-      <code><a href="https\://docs.ansible.com/ansible/devel/collections/foo/bar/baz\_role.html\#option\-main\-foo">foo\=</a></code> <code><a href="https\://docs.ansible.com/ansible/devel/collections/foo/bar/baz\_role.html\#option\-main\-bar/baz/bam">bar.baz\[123\].bam\[len\(x\) \- 1\]\=</a></code>
+      <code><a href="https://docs.ansible.com/ansible/devel/collections/foo/bar/baz_role.html#option-main-foo">foo\=</a></code> <code><a href="https://docs.ansible.com/ansible/devel/collections/foo/bar/baz_role.html#option-main-bar/baz/bam">bar\.baz\[123\]\.bam\[len\(x\) \- 1\]\=</a></code>
 
-      <code><a href="https\://docs.ansible.com/ansible/devel/collections/foo/bar/baz\_role.html\#option\-main\-foo">foo\=bar</a></code> <code><a href="https\://docs.ansible.com/ansible/devel/collections/foo/bar/baz\_role.html\#option\-main\-bar/baz/bam">bar.baz\[123\].bam\[len\(x\) \- 1\]\=bar</a></code>
+      <code><a href="https://docs.ansible.com/ansible/devel/collections/foo/bar/baz_role.html#option-main-foo">foo\=bar</a></code> <code><a href="https://docs.ansible.com/ansible/devel/collections/foo/bar/baz_role.html#option-main-bar/baz/bam">bar\.baz\[123\]\.bam\[len\(x\) \- 1\]\=bar</a></code>
 
-      <code><strong><a href="https\://docs.ansible.com/ansible/devel/collections/foo/bar/baz\_role.html\#option\-other\_entrypoint\-foo">foo</a></strong></code> <code><strong><a href="https\://docs.ansible.com/ansible/devel/collections/foo/bar/baz\_role.html\#option\-other\_entrypoint\-bar/baz/bam">bar.baz\[123\].bam\[len\(x\) \- 1\]</a></strong></code>
+      <code><strong><a href="https://docs.ansible.com/ansible/devel/collections/foo/bar/baz_role.html#option-other_entrypoint-foo">foo</a></strong></code> <code><strong><a href="https://docs.ansible.com/ansible/devel/collections/foo/bar/baz_role.html#option-other_entrypoint-bar/baz/bam">bar\.baz\[123\]\.bam\[len\(x\) \- 1\]</a></strong></code>
 
-      <code><a href="https\://docs.ansible.com/ansible/devel/collections/foo/bar/baz\_role.html\#option\-other\_entrypoint\-foo">foo\=</a></code> <code><a href="https\://docs.ansible.com/ansible/devel/collections/foo/bar/baz\_role.html\#option\-other\_entrypoint\-bar/baz/bam">bar.baz\[123\].bam\[len\(x\) \- 1\]\=</a></code>
+      <code><a href="https://docs.ansible.com/ansible/devel/collections/foo/bar/baz_role.html#option-other_entrypoint-foo">foo\=</a></code> <code><a href="https://docs.ansible.com/ansible/devel/collections/foo/bar/baz_role.html#option-other_entrypoint-bar/baz/bam">bar\.baz\[123\]\.bam\[len\(x\) \- 1\]\=</a></code>
 
-      <code><a href="https\://docs.ansible.com/ansible/devel/collections/foo/bar/baz\_role.html\#option\-other\_entrypoint\-foo">foo\=bar</a></code> <code><a href="https\://docs.ansible.com/ansible/devel/collections/foo/bar/baz\_role.html\#option\-other\_entrypoint\-bar/baz/bam">bar.baz\[123\].bam\[len\(x\) \- 1\]\=bar</a></code>
+      <code><a href="https://docs.ansible.com/ansible/devel/collections/foo/bar/baz_role.html#option-other_entrypoint-foo">foo\=bar</a></code> <code><a href="https://docs.ansible.com/ansible/devel/collections/foo/bar/baz_role.html#option-other_entrypoint-bar/baz/bam">bar\.baz\[123\]\.bam\[len\(x\) \- 1\]\=bar</a></code>
 
-      <code><strong><a href="https\://docs.ansible.com/ansible/devel/collections/bam/baz/foo\_lookup.html\#option\-foo">foo</a></strong></code> <code><strong><a href="https\://docs.ansible.com/ansible/devel/collections/bam/baz/foo\_lookup.html\#option\-bar/baz/bam">bar.baz\[123\].bam\[len\(x\) \- 1\]</a></strong></code>
+      <code><strong><a href="https://docs.ansible.com/ansible/devel/collections/bam/baz/foo_lookup.html#option-foo">foo</a></strong></code> <code><strong><a href="https://docs.ansible.com/ansible/devel/collections/bam/baz/foo_lookup.html#option-bar/baz/bam">bar\.baz\[123\]\.bam\[len\(x\) \- 1\]</a></strong></code>
 
-      <code><a href="https\://docs.ansible.com/ansible/devel/collections/bam/baz/foo\_lookup.html\#option\-foo">foo\=</a></code> <code><a href="https\://docs.ansible.com/ansible/devel/collections/bam/baz/foo\_lookup.html\#option\-bar/baz/bam">bar.baz\[123\].bam\[len\(x\) \- 1\]\=</a></code>
+      <code><a href="https://docs.ansible.com/ansible/devel/collections/bam/baz/foo_lookup.html#option-foo">foo\=</a></code> <code><a href="https://docs.ansible.com/ansible/devel/collections/bam/baz/foo_lookup.html#option-bar/baz/bam">bar\.baz\[123\]\.bam\[len\(x\) \- 1\]\=</a></code>
 
-      <code><a href="https\://docs.ansible.com/ansible/devel/collections/bam/baz/foo\_lookup.html\#option\-foo">foo\=bar</a></code> <code><a href="https\://docs.ansible.com/ansible/devel/collections/bam/baz/foo\_lookup.html\#option\-bar/baz/bam">bar.baz\[123\].bam\[len\(x\) \- 1\]\=bar</a></code>
+      <code><a href="https://docs.ansible.com/ansible/devel/collections/bam/baz/foo_lookup.html#option-foo">foo\=bar</a></code> <code><a href="https://docs.ansible.com/ansible/devel/collections/bam/baz/foo_lookup.html#option-bar/baz/bam">bar\.baz\[123\]\.bam\[len\(x\) \- 1\]\=bar</a></code>
 
-      <code><strong><a href="https\://docs.ansible.com/ansible/devel/collections/bam/baz/foo\_role.html\#option\-main\-foo">foo</a></strong></code> <code><strong><a href="https\://docs.ansible.com/ansible/devel/collections/bam/baz/foo\_role.html\#option\-main\-bar/baz/bam">bar.baz\[123\].bam\[len\(x\) \- 1\]</a></strong></code>
+      <code><strong><a href="https://docs.ansible.com/ansible/devel/collections/bam/baz/foo_role.html#option-main-foo">foo</a></strong></code> <code><strong><a href="https://docs.ansible.com/ansible/devel/collections/bam/baz/foo_role.html#option-main-bar/baz/bam">bar\.baz\[123\]\.bam\[len\(x\) \- 1\]</a></strong></code>
 
-      <code><a href="https\://docs.ansible.com/ansible/devel/collections/bam/baz/foo\_role.html\#option\-main\-foo">foo\=</a></code> <code><a href="https\://docs.ansible.com/ansible/devel/collections/bam/baz/foo\_role.html\#option\-main\-bar/baz/bam">bar.baz\[123\].bam\[len\(x\) \- 1\]\=</a></code>
+      <code><a href="https://docs.ansible.com/ansible/devel/collections/bam/baz/foo_role.html#option-main-foo">foo\=</a></code> <code><a href="https://docs.ansible.com/ansible/devel/collections/bam/baz/foo_role.html#option-main-bar/baz/bam">bar\.baz\[123\]\.bam\[len\(x\) \- 1\]\=</a></code>
 
-      <code><a href="https\://docs.ansible.com/ansible/devel/collections/bam/baz/foo\_role.html\#option\-main\-foo">foo\=bar</a></code> <code><a href="https\://docs.ansible.com/ansible/devel/collections/bam/baz/foo\_role.html\#option\-main\-bar/baz/bam">bar.baz\[123\].bam\[len\(x\) \- 1\]\=bar</a></code>
+      <code><a href="https://docs.ansible.com/ansible/devel/collections/bam/baz/foo_role.html#option-main-foo">foo\=bar</a></code> <code><a href="https://docs.ansible.com/ansible/devel/collections/bam/baz/foo_role.html#option-main-bar/baz/bam">bar\.baz\[123\]\.bam\[len\(x\) \- 1\]\=bar</a></code>
 
-      <code><strong>foo</strong></code> <code><strong>bar.baz\[123\].bam\[len\(x\) \- 1\]</strong></code>
+      <code><strong>foo</strong></code> <code><strong>bar\.baz\[123\]\.bam\[len\(x\) \- 1\]</strong></code>
 
-      <code>foo\=</code> <code>bar.baz\[123\].bam\[len\(x\) \- 1\]\=</code>
+      <code>foo\=</code> <code>bar\.baz\[123\]\.bam\[len\(x\) \- 1\]\=</code>
 
-      <code>foo\=bar</code> <code>bar.baz\[123\].bam\[len\(x\) \- 1\]\=bar</code>
+      <code>foo\=bar</code> <code>bar\.baz\[123\]\.bam\[len\(x\) \- 1\]\=bar</code>
     md_opts:
       pluginOptionLikeLink.js: |-
         (plugin, entrypoint, what, name, current_plugin) => `https://docs.ansible.com/ansible/devel/collections/${plugin.fqcn.replace(/\./g, '/')}_${plugin.type}.html#${what}${entrypoint ? '-' + entrypoint : ''}-${name.join('/')}`
       pluginOptionLikeLink.py: |-
         lambda plugin, entrypoint, what, name, current_plugin: f"https://docs.ansible.com/ansible/devel/collections/{plugin.fqcn.replace('.', '/')}_{plugin.type}.html#{what}{'-' + entrypoint if entrypoint else ''}-{'/'.join(name)}"
     rst: |-
       \ :ansopt:`foo.bar.baz#role:main:foo`\  \ :ansopt:`foo.bar.baz#role:main:bar.baz[123].bam[len(x) - 1]`\ 
@@ -971,18 +986,18 @@
 
       \ :ansopt:`foo`\  \ :ansopt:`bar.baz[123].bam[len(x) - 1]`\ 
 
       \ :ansopt:`foo=`\  \ :ansopt:`bar.baz[123].bam[len(x) - 1]=`\ 
 
       \ :ansopt:`foo=bar`\  \ :ansopt:`bar.baz[123].bam[len(x) - 1]=bar`\ 
     parse_opts:
-      current_plugin:
+      currentPlugin:
         fqcn: foo.bar.baz
         type: role
-      role_entrypoint: main
+      roleEntrypoint: main
     ansible_doc_text: |-
       `foo' (of role foo.bar.baz, main entrypoint) `bar.baz[123].bam[len(x) - 1]' (of role foo.bar.baz, main entrypoint)
 
       `foo=' (of role foo.bar.baz, main entrypoint) `bar.baz[123].bam[len(x) - 1]=' (of role foo.bar.baz, main entrypoint)
 
       `foo=bar' (of role foo.bar.baz, main entrypoint) `bar.baz[123].bam[len(x) - 1]=bar' (of role foo.bar.baz, main entrypoint)
 
@@ -1060,31 +1075,31 @@
       - |-
         RV(ignore:foo=bar) RV(ignore:bar.baz[123].bam[len(x\) - 1]=bar)
     html: |-
       <p><code class="ansible-return-value literal notranslate">foo</code> <code class="ansible-return-value literal notranslate">bar.baz[123].bam[len(x) - 1]</code></p><p><code class="ansible-return-value literal notranslate">foo=</code> <code class="ansible-return-value literal notranslate">bar.baz[123].bam[len(x) - 1]=</code></p><p><code class="ansible-return-value literal notranslate">foo=bar</code> <code class="ansible-return-value literal notranslate">bar.baz[123].bam[len(x) - 1]=bar</code></p><p><code class="ansible-return-value literal notranslate">foo</code> <code class="ansible-return-value literal notranslate">bar.baz[123].bam[len(x) - 1]</code></p><p><code class="ansible-return-value literal notranslate">foo=</code> <code class="ansible-return-value literal notranslate">bar.baz[123].bam[len(x) - 1]=</code></p><p><code class="ansible-return-value literal notranslate">foo=bar</code> <code class="ansible-return-value literal notranslate">bar.baz[123].bam[len(x) - 1]=bar</code></p><p><code class="ansible-return-value literal notranslate">foo</code> <code class="ansible-return-value literal notranslate">bar.baz[123].bam[len(x) - 1]</code></p><p><code class="ansible-return-value literal notranslate">foo=</code> <code class="ansible-return-value literal notranslate">bar.baz[123].bam[len(x) - 1]=</code></p><p><code class="ansible-return-value literal notranslate">foo=bar</code> <code class="ansible-return-value literal notranslate">bar.baz[123].bam[len(x) - 1]=bar</code></p>
     html_plain: |-
       <p><code>foo</code> <code>bar.baz[123].bam[len(x) - 1]</code></p><p><code>foo=</code> <code>bar.baz[123].bam[len(x) - 1]=</code></p><p><code>foo=bar</code> <code>bar.baz[123].bam[len(x) - 1]=bar</code></p><p><code>foo</code> <code>bar.baz[123].bam[len(x) - 1]</code></p><p><code>foo=</code> <code>bar.baz[123].bam[len(x) - 1]=</code></p><p><code>foo=bar</code> <code>bar.baz[123].bam[len(x) - 1]=bar</code></p><p><code>foo</code> <code>bar.baz[123].bam[len(x) - 1]</code></p><p><code>foo=</code> <code>bar.baz[123].bam[len(x) - 1]=</code></p><p><code>foo=bar</code> <code>bar.baz[123].bam[len(x) - 1]=bar</code></p>
     md: |-
-      <code>foo</code> <code>bar.baz\[123\].bam\[len\(x\) \- 1\]</code>
+      <code>foo</code> <code>bar\.baz\[123\]\.bam\[len\(x\) \- 1\]</code>
 
-      <code>foo\=</code> <code>bar.baz\[123\].bam\[len\(x\) \- 1\]\=</code>
+      <code>foo\=</code> <code>bar\.baz\[123\]\.bam\[len\(x\) \- 1\]\=</code>
 
-      <code>foo\=bar</code> <code>bar.baz\[123\].bam\[len\(x\) \- 1\]\=bar</code>
+      <code>foo\=bar</code> <code>bar\.baz\[123\]\.bam\[len\(x\) \- 1\]\=bar</code>
 
-      <code>foo</code> <code>bar.baz\[123\].bam\[len\(x\) \- 1\]</code>
+      <code>foo</code> <code>bar\.baz\[123\]\.bam\[len\(x\) \- 1\]</code>
 
-      <code>foo\=</code> <code>bar.baz\[123\].bam\[len\(x\) \- 1\]\=</code>
+      <code>foo\=</code> <code>bar\.baz\[123\]\.bam\[len\(x\) \- 1\]\=</code>
 
-      <code>foo\=bar</code> <code>bar.baz\[123\].bam\[len\(x\) \- 1\]\=bar</code>
+      <code>foo\=bar</code> <code>bar\.baz\[123\]\.bam\[len\(x\) \- 1\]\=bar</code>
 
-      <code>foo</code> <code>bar.baz\[123\].bam\[len\(x\) \- 1\]</code>
+      <code>foo</code> <code>bar\.baz\[123\]\.bam\[len\(x\) \- 1\]</code>
 
-      <code>foo\=</code> <code>bar.baz\[123\].bam\[len\(x\) \- 1\]\=</code>
+      <code>foo\=</code> <code>bar\.baz\[123\]\.bam\[len\(x\) \- 1\]\=</code>
 
-      <code>foo\=bar</code> <code>bar.baz\[123\].bam\[len\(x\) \- 1\]\=bar</code>
+      <code>foo\=bar</code> <code>bar\.baz\[123\]\.bam\[len\(x\) \- 1\]\=bar</code>
     rst: |-
       \ :ansretval:`foo`\  \ :ansretval:`bar.baz[123].bam[len(x) - 1]`\ 
 
       \ :ansretval:`foo=`\  \ :ansretval:`bar.baz[123].bam[len(x) - 1]=`\ 
 
       \ :ansretval:`foo=bar`\  \ :ansretval:`bar.baz[123].bam[len(x) - 1]=bar`\ 
 
@@ -1156,31 +1171,31 @@
       - |-
         RV(ignore:foo=bar) RV(ignore:bar.baz[123].bam[len(x\) - 1]=bar)
     html: |-
       <p><code class="ansible-return-value literal notranslate">foo</code> <code class="ansible-return-value literal notranslate">bar.baz[123].bam[len(x) - 1]</code></p><p><code class="ansible-return-value literal notranslate">foo=</code> <code class="ansible-return-value literal notranslate">bar.baz[123].bam[len(x) - 1]=</code></p><p><code class="ansible-return-value literal notranslate">foo=bar</code> <code class="ansible-return-value literal notranslate">bar.baz[123].bam[len(x) - 1]=bar</code></p><p><code class="ansible-return-value literal notranslate">foo</code> <code class="ansible-return-value literal notranslate">bar.baz[123].bam[len(x) - 1]</code></p><p><code class="ansible-return-value literal notranslate">foo=</code> <code class="ansible-return-value literal notranslate">bar.baz[123].bam[len(x) - 1]=</code></p><p><code class="ansible-return-value literal notranslate">foo=bar</code> <code class="ansible-return-value literal notranslate">bar.baz[123].bam[len(x) - 1]=bar</code></p><p><code class="ansible-return-value literal notranslate">foo</code> <code class="ansible-return-value literal notranslate">bar.baz[123].bam[len(x) - 1]</code></p><p><code class="ansible-return-value literal notranslate">foo=</code> <code class="ansible-return-value literal notranslate">bar.baz[123].bam[len(x) - 1]=</code></p><p><code class="ansible-return-value literal notranslate">foo=bar</code> <code class="ansible-return-value literal notranslate">bar.baz[123].bam[len(x) - 1]=bar</code></p>
     html_plain: |-
       <p><code>foo</code> <code>bar.baz[123].bam[len(x) - 1]</code></p><p><code>foo=</code> <code>bar.baz[123].bam[len(x) - 1]=</code></p><p><code>foo=bar</code> <code>bar.baz[123].bam[len(x) - 1]=bar</code></p><p><code>foo</code> <code>bar.baz[123].bam[len(x) - 1]</code></p><p><code>foo=</code> <code>bar.baz[123].bam[len(x) - 1]=</code></p><p><code>foo=bar</code> <code>bar.baz[123].bam[len(x) - 1]=bar</code></p><p><code>foo</code> <code>bar.baz[123].bam[len(x) - 1]</code></p><p><code>foo=</code> <code>bar.baz[123].bam[len(x) - 1]=</code></p><p><code>foo=bar</code> <code>bar.baz[123].bam[len(x) - 1]=bar</code></p>
     md: |-
-      <code>foo</code> <code>bar.baz\[123\].bam\[len\(x\) \- 1\]</code>
+      <code>foo</code> <code>bar\.baz\[123\]\.bam\[len\(x\) \- 1\]</code>
 
-      <code>foo\=</code> <code>bar.baz\[123\].bam\[len\(x\) \- 1\]\=</code>
+      <code>foo\=</code> <code>bar\.baz\[123\]\.bam\[len\(x\) \- 1\]\=</code>
 
-      <code>foo\=bar</code> <code>bar.baz\[123\].bam\[len\(x\) \- 1\]\=bar</code>
+      <code>foo\=bar</code> <code>bar\.baz\[123\]\.bam\[len\(x\) \- 1\]\=bar</code>
 
-      <code>foo</code> <code>bar.baz\[123\].bam\[len\(x\) \- 1\]</code>
+      <code>foo</code> <code>bar\.baz\[123\]\.bam\[len\(x\) \- 1\]</code>
 
-      <code>foo\=</code> <code>bar.baz\[123\].bam\[len\(x\) \- 1\]\=</code>
+      <code>foo\=</code> <code>bar\.baz\[123\]\.bam\[len\(x\) \- 1\]\=</code>
 
-      <code>foo\=bar</code> <code>bar.baz\[123\].bam\[len\(x\) \- 1\]\=bar</code>
+      <code>foo\=bar</code> <code>bar\.baz\[123\]\.bam\[len\(x\) \- 1\]\=bar</code>
 
-      <code>foo</code> <code>bar.baz\[123\].bam\[len\(x\) \- 1\]</code>
+      <code>foo</code> <code>bar\.baz\[123\]\.bam\[len\(x\) \- 1\]</code>
 
-      <code>foo\=</code> <code>bar.baz\[123\].bam\[len\(x\) \- 1\]\=</code>
+      <code>foo\=</code> <code>bar\.baz\[123\]\.bam\[len\(x\) \- 1\]\=</code>
 
-      <code>foo\=bar</code> <code>bar.baz\[123\].bam\[len\(x\) \- 1\]\=bar</code>
+      <code>foo\=bar</code> <code>bar\.baz\[123\]\.bam\[len\(x\) \- 1\]\=bar</code>
     rst: |-
       \ :ansretval:`foo.bar.baz.bam#boo:foo`\  \ :ansretval:`foo.bar.baz.bam#boo:bar.baz[123].bam[len(x) - 1]`\ 
 
       \ :ansretval:`foo.bar.baz.bam#boo:foo=`\  \ :ansretval:`foo.bar.baz.bam#boo:bar.baz[123].bam[len(x) - 1]=`\ 
 
       \ :ansretval:`foo.bar.baz.bam#boo:foo=bar`\  \ :ansretval:`foo.bar.baz.bam#boo:bar.baz[123].bam[len(x) - 1]=bar`\ 
 
@@ -1192,15 +1207,15 @@
 
       \ :ansretval:`foo`\  \ :ansretval:`bar.baz[123].bam[len(x) - 1]`\ 
 
       \ :ansretval:`foo=`\  \ :ansretval:`bar.baz[123].bam[len(x) - 1]=`\ 
 
       \ :ansretval:`foo=bar`\  \ :ansretval:`bar.baz[123].bam[len(x) - 1]=bar`\ 
     parse_opts:
-      current_plugin:
+      currentPlugin:
         fqcn: foo.bar.baz.bam
         type: boo
     ansible_doc_text: |-
       `foo' (of boo plugin foo.bar.baz.bam) `bar.baz[123].bam[len(x) - 1]' (of boo plugin foo.bar.baz.bam)
 
       `foo=' (of boo plugin foo.bar.baz.bam) `bar.baz[123].bam[len(x) - 1]=' (of boo plugin foo.bar.baz.bam)
 
@@ -1261,31 +1276,31 @@
       pluginOptionLikeLink.js: |-
         (plugin, entrypoint, what, name, current_plugin) => `https://docs.ansible.com/ansible/devel/collections/${plugin.fqcn.replace(/\./g, '/')}_${plugin.type}.html#${what}${entrypoint ? '-' + entrypoint : ''}-${name.join('/')}`
       pluginOptionLikeLink.py: |-
         lambda plugin, entrypoint, what, name, current_plugin: f"https://docs.ansible.com/ansible/devel/collections/{plugin.fqcn.replace('.', '/')}_{plugin.type}.html#{what}{'-' + entrypoint if entrypoint else ''}-{'/'.join(name)}"
     html_plain: |-
       <p><code>foo</code> <code>bar.baz[123].bam[len(x) - 1]</code></p><p><code>foo=</code> <code>bar.baz[123].bam[len(x) - 1]=</code></p><p><code>foo=bar</code> <code>bar.baz[123].bam[len(x) - 1]=bar</code></p><p><code><a href="https://docs.ansible.com/ansible/devel/collections/bam/baz/foo_lookup.html#retval-foo">foo</a></code> <code><a href="https://docs.ansible.com/ansible/devel/collections/bam/baz/foo_lookup.html#retval-bar/baz/bam">bar.baz[123].bam[len(x) - 1]</a></code></p><p><code><a href="https://docs.ansible.com/ansible/devel/collections/bam/baz/foo_lookup.html#retval-foo">foo=</a></code> <code><a href="https://docs.ansible.com/ansible/devel/collections/bam/baz/foo_lookup.html#retval-bar/baz/bam">bar.baz[123].bam[len(x) - 1]=</a></code></p><p><code><a href="https://docs.ansible.com/ansible/devel/collections/bam/baz/foo_lookup.html#retval-foo">foo=bar</a></code> <code><a href="https://docs.ansible.com/ansible/devel/collections/bam/baz/foo_lookup.html#retval-bar/baz/bam">bar.baz[123].bam[len(x) - 1]=bar</a></code></p><p><code>foo</code> <code>bar.baz[123].bam[len(x) - 1]</code></p><p><code>foo=</code> <code>bar.baz[123].bam[len(x) - 1]=</code></p><p><code>foo=bar</code> <code>bar.baz[123].bam[len(x) - 1]=bar</code></p>
     md: |-
-      <code>foo</code> <code>bar.baz\[123\].bam\[len\(x\) \- 1\]</code>
+      <code>foo</code> <code>bar\.baz\[123\]\.bam\[len\(x\) \- 1\]</code>
 
-      <code>foo\=</code> <code>bar.baz\[123\].bam\[len\(x\) \- 1\]\=</code>
+      <code>foo\=</code> <code>bar\.baz\[123\]\.bam\[len\(x\) \- 1\]\=</code>
 
-      <code>foo\=bar</code> <code>bar.baz\[123\].bam\[len\(x\) \- 1\]\=bar</code>
+      <code>foo\=bar</code> <code>bar\.baz\[123\]\.bam\[len\(x\) \- 1\]\=bar</code>
 
-      <code><a href="https\://docs.ansible.com/ansible/devel/collections/bam/baz/foo\_lookup.html\#retval\-foo">foo</a></code> <code><a href="https\://docs.ansible.com/ansible/devel/collections/bam/baz/foo\_lookup.html\#retval\-bar/baz/bam">bar.baz\[123\].bam\[len\(x\) \- 1\]</a></code>
+      <code><a href="https://docs.ansible.com/ansible/devel/collections/bam/baz/foo_lookup.html#retval-foo">foo</a></code> <code><a href="https://docs.ansible.com/ansible/devel/collections/bam/baz/foo_lookup.html#retval-bar/baz/bam">bar\.baz\[123\]\.bam\[len\(x\) \- 1\]</a></code>
 
-      <code><a href="https\://docs.ansible.com/ansible/devel/collections/bam/baz/foo\_lookup.html\#retval\-foo">foo\=</a></code> <code><a href="https\://docs.ansible.com/ansible/devel/collections/bam/baz/foo\_lookup.html\#retval\-bar/baz/bam">bar.baz\[123\].bam\[len\(x\) \- 1\]\=</a></code>
+      <code><a href="https://docs.ansible.com/ansible/devel/collections/bam/baz/foo_lookup.html#retval-foo">foo\=</a></code> <code><a href="https://docs.ansible.com/ansible/devel/collections/bam/baz/foo_lookup.html#retval-bar/baz/bam">bar\.baz\[123\]\.bam\[len\(x\) \- 1\]\=</a></code>
 
-      <code><a href="https\://docs.ansible.com/ansible/devel/collections/bam/baz/foo\_lookup.html\#retval\-foo">foo\=bar</a></code> <code><a href="https\://docs.ansible.com/ansible/devel/collections/bam/baz/foo\_lookup.html\#retval\-bar/baz/bam">bar.baz\[123\].bam\[len\(x\) \- 1\]\=bar</a></code>
+      <code><a href="https://docs.ansible.com/ansible/devel/collections/bam/baz/foo_lookup.html#retval-foo">foo\=bar</a></code> <code><a href="https://docs.ansible.com/ansible/devel/collections/bam/baz/foo_lookup.html#retval-bar/baz/bam">bar\.baz\[123\]\.bam\[len\(x\) \- 1\]\=bar</a></code>
 
-      <code>foo</code> <code>bar.baz\[123\].bam\[len\(x\) \- 1\]</code>
+      <code>foo</code> <code>bar\.baz\[123\]\.bam\[len\(x\) \- 1\]</code>
 
-      <code>foo\=</code> <code>bar.baz\[123\].bam\[len\(x\) \- 1\]\=</code>
+      <code>foo\=</code> <code>bar\.baz\[123\]\.bam\[len\(x\) \- 1\]\=</code>
 
-      <code>foo\=bar</code> <code>bar.baz\[123\].bam\[len\(x\) \- 1\]\=bar</code>
+      <code>foo\=bar</code> <code>bar\.baz\[123\]\.bam\[len\(x\) \- 1\]\=bar</code>
     md_opts:
       pluginOptionLikeLink.js: |-
         (plugin, entrypoint, what, name, current_plugin) => `https://docs.ansible.com/ansible/devel/collections/${plugin.fqcn.replace(/\./g, '/')}_${plugin.type}.html#${what}${entrypoint ? '-' + entrypoint : ''}-${name.join('/')}`
       pluginOptionLikeLink.py: |-
         lambda plugin, entrypoint, what, name, current_plugin: f"https://docs.ansible.com/ansible/devel/collections/{plugin.fqcn.replace('.', '/')}_{plugin.type}.html#{what}{'-' + entrypoint if entrypoint else ''}-{'/'.join(name)}"
     rst: |-
       \ :ansretval:`foo`\  \ :ansretval:`bar.baz[123].bam[len(x) - 1]`\ 
@@ -1367,31 +1382,31 @@
       pluginOptionLikeLink.js: |-
         (plugin, entrypoint, what, name, current_plugin) => `https://docs.ansible.com/ansible/devel/collections/${plugin.fqcn.replace(/\./g, '/')}_${plugin.type}.html#${what}${entrypoint ? '-' + entrypoint : ''}-${name.join('/')}`
       pluginOptionLikeLink.py: |-
         lambda plugin, entrypoint, what, name, current_plugin: f"https://docs.ansible.com/ansible/devel/collections/{plugin.fqcn.replace('.', '/')}_{plugin.type}.html#{what}{'-' + entrypoint if entrypoint else ''}-{'/'.join(name)}"
     html_plain: |-
       <p><code><a href="https://docs.ansible.com/ansible/devel/collections/foo/bar/baz/bam_boo.html#retval-foo">foo</a></code> <code><a href="https://docs.ansible.com/ansible/devel/collections/foo/bar/baz/bam_boo.html#retval-bar/baz/bam">bar.baz[123].bam[len(x) - 1]</a></code></p><p><code><a href="https://docs.ansible.com/ansible/devel/collections/foo/bar/baz/bam_boo.html#retval-foo">foo=</a></code> <code><a href="https://docs.ansible.com/ansible/devel/collections/foo/bar/baz/bam_boo.html#retval-bar/baz/bam">bar.baz[123].bam[len(x) - 1]=</a></code></p><p><code><a href="https://docs.ansible.com/ansible/devel/collections/foo/bar/baz/bam_boo.html#retval-foo">foo=bar</a></code> <code><a href="https://docs.ansible.com/ansible/devel/collections/foo/bar/baz/bam_boo.html#retval-bar/baz/bam">bar.baz[123].bam[len(x) - 1]=bar</a></code></p><p><code><a href="https://docs.ansible.com/ansible/devel/collections/bam/baz/foo_lookup.html#retval-foo">foo</a></code> <code><a href="https://docs.ansible.com/ansible/devel/collections/bam/baz/foo_lookup.html#retval-bar/baz/bam">bar.baz[123].bam[len(x) - 1]</a></code></p><p><code><a href="https://docs.ansible.com/ansible/devel/collections/bam/baz/foo_lookup.html#retval-foo">foo=</a></code> <code><a href="https://docs.ansible.com/ansible/devel/collections/bam/baz/foo_lookup.html#retval-bar/baz/bam">bar.baz[123].bam[len(x) - 1]=</a></code></p><p><code><a href="https://docs.ansible.com/ansible/devel/collections/bam/baz/foo_lookup.html#retval-foo">foo=bar</a></code> <code><a href="https://docs.ansible.com/ansible/devel/collections/bam/baz/foo_lookup.html#retval-bar/baz/bam">bar.baz[123].bam[len(x) - 1]=bar</a></code></p><p><code>foo</code> <code>bar.baz[123].bam[len(x) - 1]</code></p><p><code>foo=</code> <code>bar.baz[123].bam[len(x) - 1]=</code></p><p><code>foo=bar</code> <code>bar.baz[123].bam[len(x) - 1]=bar</code></p>
     md: |-
-      <code><a href="https\://docs.ansible.com/ansible/devel/collections/foo/bar/baz/bam\_boo.html\#retval\-foo">foo</a></code> <code><a href="https\://docs.ansible.com/ansible/devel/collections/foo/bar/baz/bam\_boo.html\#retval\-bar/baz/bam">bar.baz\[123\].bam\[len\(x\) \- 1\]</a></code>
+      <code><a href="https://docs.ansible.com/ansible/devel/collections/foo/bar/baz/bam_boo.html#retval-foo">foo</a></code> <code><a href="https://docs.ansible.com/ansible/devel/collections/foo/bar/baz/bam_boo.html#retval-bar/baz/bam">bar\.baz\[123\]\.bam\[len\(x\) \- 1\]</a></code>
 
-      <code><a href="https\://docs.ansible.com/ansible/devel/collections/foo/bar/baz/bam\_boo.html\#retval\-foo">foo\=</a></code> <code><a href="https\://docs.ansible.com/ansible/devel/collections/foo/bar/baz/bam\_boo.html\#retval\-bar/baz/bam">bar.baz\[123\].bam\[len\(x\) \- 1\]\=</a></code>
+      <code><a href="https://docs.ansible.com/ansible/devel/collections/foo/bar/baz/bam_boo.html#retval-foo">foo\=</a></code> <code><a href="https://docs.ansible.com/ansible/devel/collections/foo/bar/baz/bam_boo.html#retval-bar/baz/bam">bar\.baz\[123\]\.bam\[len\(x\) \- 1\]\=</a></code>
 
-      <code><a href="https\://docs.ansible.com/ansible/devel/collections/foo/bar/baz/bam\_boo.html\#retval\-foo">foo\=bar</a></code> <code><a href="https\://docs.ansible.com/ansible/devel/collections/foo/bar/baz/bam\_boo.html\#retval\-bar/baz/bam">bar.baz\[123\].bam\[len\(x\) \- 1\]\=bar</a></code>
+      <code><a href="https://docs.ansible.com/ansible/devel/collections/foo/bar/baz/bam_boo.html#retval-foo">foo\=bar</a></code> <code><a href="https://docs.ansible.com/ansible/devel/collections/foo/bar/baz/bam_boo.html#retval-bar/baz/bam">bar\.baz\[123\]\.bam\[len\(x\) \- 1\]\=bar</a></code>
 
-      <code><a href="https\://docs.ansible.com/ansible/devel/collections/bam/baz/foo\_lookup.html\#retval\-foo">foo</a></code> <code><a href="https\://docs.ansible.com/ansible/devel/collections/bam/baz/foo\_lookup.html\#retval\-bar/baz/bam">bar.baz\[123\].bam\[len\(x\) \- 1\]</a></code>
+      <code><a href="https://docs.ansible.com/ansible/devel/collections/bam/baz/foo_lookup.html#retval-foo">foo</a></code> <code><a href="https://docs.ansible.com/ansible/devel/collections/bam/baz/foo_lookup.html#retval-bar/baz/bam">bar\.baz\[123\]\.bam\[len\(x\) \- 1\]</a></code>
 
-      <code><a href="https\://docs.ansible.com/ansible/devel/collections/bam/baz/foo\_lookup.html\#retval\-foo">foo\=</a></code> <code><a href="https\://docs.ansible.com/ansible/devel/collections/bam/baz/foo\_lookup.html\#retval\-bar/baz/bam">bar.baz\[123\].bam\[len\(x\) \- 1\]\=</a></code>
+      <code><a href="https://docs.ansible.com/ansible/devel/collections/bam/baz/foo_lookup.html#retval-foo">foo\=</a></code> <code><a href="https://docs.ansible.com/ansible/devel/collections/bam/baz/foo_lookup.html#retval-bar/baz/bam">bar\.baz\[123\]\.bam\[len\(x\) \- 1\]\=</a></code>
 
-      <code><a href="https\://docs.ansible.com/ansible/devel/collections/bam/baz/foo\_lookup.html\#retval\-foo">foo\=bar</a></code> <code><a href="https\://docs.ansible.com/ansible/devel/collections/bam/baz/foo\_lookup.html\#retval\-bar/baz/bam">bar.baz\[123\].bam\[len\(x\) \- 1\]\=bar</a></code>
+      <code><a href="https://docs.ansible.com/ansible/devel/collections/bam/baz/foo_lookup.html#retval-foo">foo\=bar</a></code> <code><a href="https://docs.ansible.com/ansible/devel/collections/bam/baz/foo_lookup.html#retval-bar/baz/bam">bar\.baz\[123\]\.bam\[len\(x\) \- 1\]\=bar</a></code>
 
-      <code>foo</code> <code>bar.baz\[123\].bam\[len\(x\) \- 1\]</code>
+      <code>foo</code> <code>bar\.baz\[123\]\.bam\[len\(x\) \- 1\]</code>
 
-      <code>foo\=</code> <code>bar.baz\[123\].bam\[len\(x\) \- 1\]\=</code>
+      <code>foo\=</code> <code>bar\.baz\[123\]\.bam\[len\(x\) \- 1\]\=</code>
 
-      <code>foo\=bar</code> <code>bar.baz\[123\].bam\[len\(x\) \- 1\]\=bar</code>
+      <code>foo\=bar</code> <code>bar\.baz\[123\]\.bam\[len\(x\) \- 1\]\=bar</code>
     md_opts:
       pluginOptionLikeLink.js: |-
         (plugin, entrypoint, what, name, current_plugin) => `https://docs.ansible.com/ansible/devel/collections/${plugin.fqcn.replace(/\./g, '/')}_${plugin.type}.html#${what}${entrypoint ? '-' + entrypoint : ''}-${name.join('/')}`
       pluginOptionLikeLink.py: |-
         lambda plugin, entrypoint, what, name, current_plugin: f"https://docs.ansible.com/ansible/devel/collections/{plugin.fqcn.replace('.', '/')}_{plugin.type}.html#{what}{'-' + entrypoint if entrypoint else ''}-{'/'.join(name)}"
     rst: |-
       \ :ansretval:`foo.bar.baz.bam#boo:foo`\  \ :ansretval:`foo.bar.baz.bam#boo:bar.baz[123].bam[len(x) - 1]`\ 
@@ -1408,15 +1423,15 @@
 
       \ :ansretval:`foo`\  \ :ansretval:`bar.baz[123].bam[len(x) - 1]`\ 
 
       \ :ansretval:`foo=`\  \ :ansretval:`bar.baz[123].bam[len(x) - 1]=`\ 
 
       \ :ansretval:`foo=bar`\  \ :ansretval:`bar.baz[123].bam[len(x) - 1]=bar`\ 
     parse_opts:
-      current_plugin:
+      currentPlugin:
         fqcn: foo.bar.baz.bam
         type: boo
     ansible_doc_text: |-
       `foo' (of boo plugin foo.bar.baz.bam) `bar.baz[123].bam[len(x) - 1]' (of boo plugin foo.bar.baz.bam)
 
       `foo=' (of boo plugin foo.bar.baz.bam) `bar.baz[123].bam[len(x) - 1]=' (of boo plugin foo.bar.baz.bam)
```

#### html2text {}

```diff
@@ -5,86 +5,101 @@
 empty_content: source: [''] html:
 html_plain:
 md: ' ' rst: '\ ' ansible_doc_text: '' rst_plain: '\ ' simple: source: |- This
 is a C(test) I(module) B(markup). html: |-
 This is a test module markup.
 html_plain: |-
 This is a test module markup.
-md: |- This is a test module markup. rst: |- This is a \ :literal:`test`\ \ :
+md: |- This is a test module markup\. rst: |- This is a \ :literal:`test`\ \ :
 emphasis:`module`\ \ :strong:`markup`\ . ansible_doc_text: This is a `test'
 `module' *markup*. rst_plain: This is a \ :literal:`test`\ \ :emphasis:
 `module`\ \ :strong:`markup`\ . module: source: |- The M(a.b.c) module. html:
 |-
 The a.b.c module.
 html_opts: pluginLink.js: |- (plugin_data) => `https://docs.ansible.com/
 ansible/devel/collections/${plugin_data.fqcn.replace(/\./g, '/')}_$
 {plugin_data.type}.html` pluginLink.py: |- lambda plugin_data: f"https://
 docs.ansible.com/ansible/devel/collections/{plugin_data.fqcn.replace('.', '/
 ')}_{plugin_data.type}.html" html_plain: |-
 The a.b.c module.
-md: |- The [a.b.c](https\://docs.ansible.com/ansible/devel/collections/a/b/
-c\_module.html) module. md_opts: pluginLink.js: |- (plugin_data) => `https://
+md: |- The [a\.b\.c](https\://docs\.ansible\.com/ansible/devel/collections/a/b/
+c\_module\.html) module\. md_opts: pluginLink.js: |- (plugin_data) => `https://
 docs.ansible.com/ansible/devel/collections/${plugin_data.fqcn.replace(/\./g, '/
 ')}_${plugin_data.type}.html` pluginLink.py: |- lambda plugin_data: f"https://
 docs.ansible.com/ansible/devel/collections/{plugin_data.fqcn.replace('.', '/
 ')}_{plugin_data.type}.html" rst: |- The \ :ref:`a.b.c
 a.b.c_module>`\ module. ansible_doc_text: The [a.b.c] module. rst_plain: The \
 :ref:`a.b.c
 a.b.c_module>`\ module. module_no_link: source: |- The M(a.b.c) module. html:
 |-
 The a.b.c module.
 html_plain: |-
 The a.b.c module.
-md: |- The a.b.c module. rst: |- The \ :ref:`a.b.c
+md: |- The a\.b\.c module\. rst: |- The \ :ref:`a.b.c
 a.b.c_module>`\ module. ansible_doc_text: The [a.b.c] module. rst_plain: The \
 :ref:`a.b.c
 a.b.c_module>`\ module. plugin: source: |- The P(a.b.c#lookup) lookup plugin.
 html: |-
 The a.b.c lookup plugin.
 html_opts: pluginLink.js: |- (plugin_data) => `https://docs.ansible.com/
 ansible/devel/collections/${plugin_data.fqcn.replace(/\./g, '/')}_$
 {plugin_data.type}.html` pluginLink.py: |- lambda plugin_data: f"https://
 docs.ansible.com/ansible/devel/collections/{plugin_data.fqcn.replace('.', '/
 ')}_{plugin_data.type}.html" html_plain: |-
 The a.b.c lookup plugin.
-md: |- The [a.b.c](https\://docs.ansible.com/ansible/devel/collections/a/b/
-c\_lookup.html) lookup plugin. md_opts: pluginLink.js: |- (plugin_data) =>
+md: |- The [a\.b\.c](https\://docs\.ansible\.com/ansible/devel/collections/a/b/
+c\_lookup\.html) lookup plugin\. md_opts: pluginLink.js: |- (plugin_data) =>
 `https://docs.ansible.com/ansible/devel/collections/${plugin_data.fqcn.replace
 (/\./g, '/')}_${plugin_data.type}.html` pluginLink.py: |- lambda plugin_data:
 f"https://docs.ansible.com/ansible/devel/collections/{plugin_data.fqcn.replace
 ('.', '/')}_{plugin_data.type}.html" rst: |- The \ :ref:`a.b.c
 a.b.c_lookup>`\ lookup plugin. ansible_doc_text: The [a.b.c] lookup plugin.
 rst_plain: The \ :ref:`a.b.c
 a.b.c_lookup>`\ lookup plugin. plugin_no_link: source: |- The P(a.b.c#lookup)
 lookup plugin. html: |-
 The a.b.c lookup plugin.
 html_plain: |-
 The a.b.c lookup plugin.
-md: |- The a.b.c lookup plugin. rst: |- The \ :ref:`a.b.c
+md: |- The a\.b\.c lookup plugin\. rst: |- The \ :ref:`a.b.c
 a.b.c_lookup>`\ lookup plugin. ansible_doc_text: The [a.b.c] lookup plugin.
 rst_plain: The \ :ref:`a.b.c
 a.b.c_lookup>`\ lookup plugin. link_and_url: source: |- An URL U(https://
-example.com) and L(a link, https://example.org). html: |-
-An URL https://example.com and a_link.
+example.com) and L(a link, https://example.org). With special characters: U
+(https://example.com/test.html?foo=b
+r&find=\*#baz.bam%3Dboo) and L(mee.boo, https://example.org/test.html?foo=b
+r&find=\*#baz.bam%3Dboo) html: |-
+An URL https://example.com and a_link. With special characters: https://
+example.com/test.html?foo=b%3Ca%3Er&find=%5C*#baz.bam%253Dboo and mee.boo
 html_plain: |-
-An URL https://example.com and a_link.
-md: |- An URL [https\://example.com](https\://example.com) and [a link](https\:
-//example.org). rst: |- An URL \ https://example.com\ and \ `a link
-example.org>`__\ . ansible_doc_text: An URL https://example.com and a link
-example.org>. rst_plain: An URL \ https://example.com\ and \ `a link
-example.org>`__\ . rst_ref: source: |- A R(RST reference,
-ansible_collections.community.general.ufw_module). html: |-
+An URL https://example.com and a_link. With special characters: https://
+example.com/test.html?foo=b%3Ca%3Er&find=%5C*#baz.bam%253Dboo and mee.boo
+md: |- An URL [https\://example\.com](https://example.com) and [a link](https:/
+/example.org)\. With special characters\: [https\://example\.com/
+test\.html\?foo\=b\%3Ca\%3Er\&find\=\%5C\*\#baz\.bam\%253Dboo](https://
+example.com/test.html?foo=b%3Ca%3Er&find=%5C*#baz.bam%253Dboo) and [mee\.boo]
+(https://example.org/test.html?foo=b%3Ca%3Er&find=%5C*#baz.bam%253Dboo) rst: |-
+An URL \ https://example.com\ and \ `a link example.org>`__\ . With special
+characters: \ https://example.com/
+test.html?foo=b%3Ca%3Er&find=%5C*#baz.bam%253Dboo\ and \ `mee.boo example.org/
+test.html?foo=b%3Ca%3Er&find=%5C*#baz.bam%253Dboo>`__\ ansible_doc_text: |- An
+URL https://example.com and a link example.org>. With special characters:
+https://example.com/test.html?foo=b
+r&find=\*#baz.bam%3Dboo and mee.boo example.org/test.html?foo=b
+r&find=\*#baz.bam%3Dboo> rst_plain: |- An URL \ https://example.com\ and \ `a
+link example.org>`__\ . With special characters: \ https://example.com/
+test.html?foo=b%3Ca%3Er&find=%5C*#baz.bam%253Dboo\ and \ `mee.boo example.org/
+test.html?foo=b%3Ca%3Er&find=%5C*#baz.bam%253Dboo>`__\ rst_ref: source: |- A R
+(RST reference, ansible_collections.community.general.ufw_module). html: |-
 A RST reference.
 html_plain: |-
 A RST reference.
-md: |- A RST reference. rst: |- A \ :ref:`RST reference
+md: |- A RST reference\. rst: |- A \ :ref:`RST reference
 community.general.ufw_module>`\ . ansible_doc_text: A RST reference. rst_plain:
-A \ :ref:`RST reference
-community.general.ufw_module>`\ . horizontal_line: source: |- foo
-HORIZONTALLINE bar html: |-
+A \ :ref:`RST reference community.general.ufw_module>`\ . horizontal_line:
+source: |- foo HORIZONTALLINE bar html: |-
 foo
 ===============================================================================
 bar
 html_plain: |-
 foo
 ===============================================================================
 bar
@@ -94,20 +109,19 @@
 ===============================================================================
 bar ansible_doc_text: |- foo ------------- bar rst_plain: |- foo -----------
 - bar semantic_markup: source: |- foo E(FOOBAR) bar P(foo.bar.baz#bam) has
 value V( foo\),bar\\bam ). html: |-
 foo FOOBAR bar foo.bar.baz has value foo),bar\bam.
 html_plain: |-
 foo FOOBAR bar foo.bar.baz has value foo),bar\bam.
-md: |- foo FOOBAR bar foo.bar.baz has value foo\)\,bar\\bam. rst: |- foo \ :
-envvar:`FOOBAR`\ bar \ :ref:`foo.bar.baz
-foo.bar.baz_bam>`\ has value \ :ansval:`\ foo),bar\\bam \ `\ .
-ansible_doc_text: foo `FOOBAR' bar [foo.bar.baz] has value ` foo),bar\bam '.
-rst_plain: foo \ :envvar:`FOOBAR`\ bar \ :ref:`foo.bar.baz
-foo.bar.baz_bam>`\ has value \ :literal:`\ foo),bar\\bam \ `\ .
+md: |- foo FOOBAR bar foo\.bar\.baz has value foo\)\,bar\\bam\. rst: |- foo \ :
+envvar:`FOOBAR`\ bar \ :ref:`foo.bar.baz foo.bar.baz_bam>`\ has value \ :
+ansval:`\ foo),bar\\bam \ `\ . ansible_doc_text: foo `FOOBAR' bar [foo.bar.baz]
+has value ` foo),bar\bam '. rst_plain: foo \ :envvar:`FOOBAR`\ bar \ :ref:
+`foo.bar.baz foo.bar.baz_bam>`\ has value \ :literal:`\ foo),bar\\bam \ `\ .
 option_name_no_current_plugin: source: - |- O(foo) O(bar.baz[123].bam[len(x\) -
 1]) - |- O(foo=) O(bar.baz[123].bam[len(x\) - 1]=) - |- O(foo=bar) O(bar.baz
 [123].bam[len(x\) - 1]=bar) - |- O(bam.baz.foo#lookup:foo) O
 (bam.baz.foo#lookup:bar.baz[123].bam[len(x\) - 1]) - |- O(bam.baz.foo#lookup:
 foo=) O(bam.baz.foo#lookup:bar.baz[123].bam[len(x\) - 1]=) - |- O
 (bam.baz.foo#lookup:foo=bar) O(bam.baz.foo#lookup:bar.baz[123].bam[len(x\) -
 1]=bar) - |- O(bam.baz.foo#role:main:foo) O(bam.baz.foo#role:main:bar.baz
@@ -138,86 +152,80 @@
 foo=bar bar.baz[123].bam[len(x) - 1]=bar
 foo bar.baz[123].bam[len(x) - 1]
 foo= bar.baz[123].bam[len(x) - 1]=
 foo=bar bar.baz[123].bam[len(x) - 1]=bar
 foo bar.baz[123].bam[len(x) - 1]
 foo= bar.baz[123].bam[len(x) - 1]=
 foo=bar bar.baz[123].bam[len(x) - 1]=bar
-md: |- foo bar.baz\[123\].bam\[len\(x\) \- 1\] foo\= bar.baz\[123\].bam\[len\
-(x\) \- 1\]\= foo\=bar bar.baz\[123\].bam\[len\(x\) \- 1\]\=bar foo bar.baz\
-[123\].bam\[len\(x\) \- 1\] foo\= bar.baz\[123\].bam\[len\(x\) \- 1\]\=
-foo\=bar bar.baz\[123\].bam\[len\(x\) \- 1\]\=bar foo bar.baz\[123\].bam\[len\
-(x\) \- 1\] foo\= bar.baz\[123\].bam\[len\(x\) \- 1\]\= foo\=bar bar.baz\
-[123\].bam\[len\(x\) \- 1\]\=bar foo bar.baz\[123\].bam\[len\(x\) \- 1\] foo\=
-bar.baz\[123\].bam\[len\(x\) \- 1\]\= foo\=bar bar.baz\[123\].bam\[len\(x\) \-
-1\]\=bar rst: |- \ :ansopt:`foo`\ \ :ansopt:`bar.baz[123].bam[len(x) - 1]`\ \ :
-ansopt:`foo=`\ \ :ansopt:`bar.baz[123].bam[len(x) - 1]=`\ \ :ansopt:`foo=bar`\
-\ :ansopt:`bar.baz[123].bam[len(x) - 1]=bar`\ \ :ansopt:`bam.baz.foo#lookup:
-foo`\ \ :ansopt:`bam.baz.foo#lookup:bar.baz[123].bam[len(x) - 1]`\ \ :ansopt:
-`bam.baz.foo#lookup:foo=`\ \ :ansopt:`bam.baz.foo#lookup:bar.baz[123].bam[len
-(x) - 1]=`\ \ :ansopt:`bam.baz.foo#lookup:foo=bar`\ \ :ansopt:
-`bam.baz.foo#lookup:bar.baz[123].bam[len(x) - 1]=bar`\ \ :ansopt:
-`bam.baz.foo#role:main:foo`\ \ :ansopt:`bam.baz.foo#role:main:bar.baz[123].bam
-[len(x) - 1]`\ \ :ansopt:`bam.baz.foo#role:main:foo=`\ \ :ansopt:
-`bam.baz.foo#role:main:bar.baz[123].bam[len(x) - 1]=`\ \ :ansopt:
-`bam.baz.foo#role:main:foo=bar`\ \ :ansopt:`bam.baz.foo#role:main:bar.baz
-[123].bam[len(x) - 1]=bar`\ \ :ansopt:`foo`\ \ :ansopt:`bar.baz[123].bam[len(x)
-- 1]`\ \ :ansopt:`foo=`\ \ :ansopt:`bar.baz[123].bam[len(x) - 1]=`\ \ :ansopt:
-`foo=bar`\ \ :ansopt:`bar.baz[123].bam[len(x) - 1]=bar`\ ansible_doc_text: |-
-`foo' `bar.baz[123].bam[len(x) - 1]' `foo=' `bar.baz[123].bam[len(x) - 1]='
-`foo=bar' `bar.baz[123].bam[len(x) - 1]=bar' `foo' (of lookup plugin
-bam.baz.foo) `bar.baz[123].bam[len(x) - 1]' (of lookup plugin bam.baz.foo)
-`foo=' (of lookup plugin bam.baz.foo) `bar.baz[123].bam[len(x) - 1]=' (of
-lookup plugin bam.baz.foo) `foo=bar' (of lookup plugin bam.baz.foo) `bar.baz
-[123].bam[len(x) - 1]=bar' (of lookup plugin bam.baz.foo) `foo' (of role
-bam.baz.foo, main entrypoint) `bar.baz[123].bam[len(x) - 1]' (of role
-bam.baz.foo, main entrypoint) `foo=' (of role bam.baz.foo, main entrypoint)
-`bar.baz[123].bam[len(x) - 1]=' (of role bam.baz.foo, main entrypoint)
-`foo=bar' (of role bam.baz.foo, main entrypoint) `bar.baz[123].bam[len(x) -
-1]=bar' (of role bam.baz.foo, main entrypoint) `foo' `bar.baz[123].bam[len(x) -
-1]' `foo=' `bar.baz[123].bam[len(x) - 1]=' `foo=bar' `bar.baz[123].bam[len(x) -
-1]=bar' rst_plain: |- \ :literal:`foo`\ \ :literal:`bar.baz[123].bam[len(x) -
-1]`\ \ :literal:`foo=`\ \ :literal:`bar.baz[123].bam[len(x) - 1]=`\ \ :literal:
-`foo=bar`\ \ :literal:`bar.baz[123].bam[len(x) - 1]=bar`\ \ :literal:`foo` (of
-lookup plugin :ref:`bam.baz.foo
+md: |- foo bar\.baz\[123\]\.bam\[len\(x\) \- 1\] foo\= bar\.baz\[123\]\.bam\
+[len\(x\) \- 1\]\= foo\=bar bar\.baz\[123\]\.bam\[len\(x\) \- 1\]\=bar foo
+bar\.baz\[123\]\.bam\[len\(x\) \- 1\] foo\= bar\.baz\[123\]\.bam\[len\(x\) \-
+1\]\= foo\=bar bar\.baz\[123\]\.bam\[len\(x\) \- 1\]\=bar foo bar\.baz\
+[123\]\.bam\[len\(x\) \- 1\] foo\= bar\.baz\[123\]\.bam\[len\(x\) \- 1\]\=
+foo\=bar bar\.baz\[123\]\.bam\[len\(x\) \- 1\]\=bar foo bar\.baz\[123\]\.bam\
+[len\(x\) \- 1\] foo\= bar\.baz\[123\]\.bam\[len\(x\) \- 1\]\= foo\=bar
+bar\.baz\[123\]\.bam\[len\(x\) \- 1\]\=bar rst: |- \ :ansopt:`foo`\ \ :ansopt:
+`bar.baz[123].bam[len(x) - 1]`\ \ :ansopt:`foo=`\ \ :ansopt:`bar.baz[123].bam
+[len(x) - 1]=`\ \ :ansopt:`foo=bar`\ \ :ansopt:`bar.baz[123].bam[len(x) -
+1]=bar`\ \ :ansopt:`bam.baz.foo#lookup:foo`\ \ :ansopt:`bam.baz.foo#lookup:
+bar.baz[123].bam[len(x) - 1]`\ \ :ansopt:`bam.baz.foo#lookup:foo=`\ \ :ansopt:
+`bam.baz.foo#lookup:bar.baz[123].bam[len(x) - 1]=`\ \ :ansopt:
+`bam.baz.foo#lookup:foo=bar`\ \ :ansopt:`bam.baz.foo#lookup:bar.baz[123].bam
+[len(x) - 1]=bar`\ \ :ansopt:`bam.baz.foo#role:main:foo`\ \ :ansopt:
+`bam.baz.foo#role:main:bar.baz[123].bam[len(x) - 1]`\ \ :ansopt:
+`bam.baz.foo#role:main:foo=`\ \ :ansopt:`bam.baz.foo#role:main:bar.baz[123].bam
+[len(x) - 1]=`\ \ :ansopt:`bam.baz.foo#role:main:foo=bar`\ \ :ansopt:
+`bam.baz.foo#role:main:bar.baz[123].bam[len(x) - 1]=bar`\ \ :ansopt:`foo`\ \ :
+ansopt:`bar.baz[123].bam[len(x) - 1]`\ \ :ansopt:`foo=`\ \ :ansopt:`bar.baz
+[123].bam[len(x) - 1]=`\ \ :ansopt:`foo=bar`\ \ :ansopt:`bar.baz[123].bam[len
+(x) - 1]=bar`\ ansible_doc_text: |- `foo' `bar.baz[123].bam[len(x) - 1]' `foo='
+`bar.baz[123].bam[len(x) - 1]=' `foo=bar' `bar.baz[123].bam[len(x) - 1]=bar'
+`foo' (of lookup plugin bam.baz.foo) `bar.baz[123].bam[len(x) - 1]' (of lookup
+plugin bam.baz.foo) `foo=' (of lookup plugin bam.baz.foo) `bar.baz[123].bam[len
+(x) - 1]=' (of lookup plugin bam.baz.foo) `foo=bar' (of lookup plugin
+bam.baz.foo) `bar.baz[123].bam[len(x) - 1]=bar' (of lookup plugin bam.baz.foo)
+`foo' (of role bam.baz.foo, main entrypoint) `bar.baz[123].bam[len(x) - 1]' (of
+role bam.baz.foo, main entrypoint) `foo=' (of role bam.baz.foo, main
+entrypoint) `bar.baz[123].bam[len(x) - 1]=' (of role bam.baz.foo, main
+entrypoint) `foo=bar' (of role bam.baz.foo, main entrypoint) `bar.baz[123].bam
+[len(x) - 1]=bar' (of role bam.baz.foo, main entrypoint) `foo' `bar.baz
+[123].bam[len(x) - 1]' `foo=' `bar.baz[123].bam[len(x) - 1]=' `foo=bar'
+`bar.baz[123].bam[len(x) - 1]=bar' rst_plain: |- \ :literal:`foo`\ \ :literal:
+`bar.baz[123].bam[len(x) - 1]`\ \ :literal:`foo=`\ \ :literal:`bar.baz[123].bam
+[len(x) - 1]=`\ \ :literal:`foo=bar`\ \ :literal:`bar.baz[123].bam[len(x) -
+1]=bar`\ \ :literal:`foo` (of lookup plugin :ref:`bam.baz.foo
 bam.baz.foo_lookup>`)\ \ :literal:`bar.baz[123].bam[len(x) - 1]` (of lookup
-plugin :ref:`bam.baz.foo
-bam.baz.foo_lookup>`)\ \ :literal:`foo=` (of lookup plugin :ref:`bam.baz.foo
-bam.baz.foo_lookup>`)\ \ :literal:`bar.baz[123].bam[len(x) - 1]=` (of lookup
-plugin :ref:`bam.baz.foo
-bam.baz.foo_lookup>`)\ \ :literal:`foo=bar` (of lookup plugin :ref:`bam.baz.foo
-bam.baz.foo_lookup>`)\ \ :literal:`bar.baz[123].bam[len(x) - 1]=bar` (of lookup
-plugin :ref:`bam.baz.foo
+plugin :ref:`bam.baz.foo bam.baz.foo_lookup>`)\ \ :literal:`foo=` (of lookup
+plugin :ref:`bam.baz.foo bam.baz.foo_lookup>`)\ \ :literal:`bar.baz[123].bam
+[len(x) - 1]=` (of lookup plugin :ref:`bam.baz.foo bam.baz.foo_lookup>`)\ \ :
+literal:`foo=bar` (of lookup plugin :ref:`bam.baz.foo bam.baz.foo_lookup>`)\ \
+:literal:`bar.baz[123].bam[len(x) - 1]=bar` (of lookup plugin :ref:`bam.baz.foo
 bam.baz.foo_lookup>`)\ \ :literal:`foo` (of role :ref:`bam.baz.foo
 bam.baz.foo_role>`, entrypoint main)\ \ :literal:`bar.baz[123].bam[len(x) - 1]`
-(of role :ref:`bam.baz.foo
-bam.baz.foo_role>`, entrypoint main)\ \ :literal:`foo=` (of role :ref:
-`bam.baz.foo
-bam.baz.foo_role>`, entrypoint main)\ \ :literal:`bar.baz[123].bam[len(x) -
-1]=` (of role :ref:`bam.baz.foo
+(of role :ref:`bam.baz.foo bam.baz.foo_role>`, entrypoint main)\ \ :literal:
+`foo=` (of role :ref:`bam.baz.foo bam.baz.foo_role>`, entrypoint main)\ \ :
+literal:`bar.baz[123].bam[len(x) - 1]=` (of role :ref:`bam.baz.foo
 bam.baz.foo_role>`, entrypoint main)\ \ :literal:`foo=bar` (of role :ref:
-`bam.baz.foo
-bam.baz.foo_role>`, entrypoint main)\ \ :literal:`bar.baz[123].bam[len(x) -
-1]=bar` (of role :ref:`bam.baz.foo
-bam.baz.foo_role>`, entrypoint main)\ \ :literal:`foo`\ \ :literal:`bar.baz
-[123].bam[len(x) - 1]`\ \ :literal:`foo=`\ \ :literal:`bar.baz[123].bam[len(x)
-- 1]=`\ \ :literal:`foo=bar`\ \ :literal:`bar.baz[123].bam[len(x) - 1]=bar`\
-option_name_current_plugin: source: - |- O(foo) O(bar.baz[123].bam[len(x\) -
-1]) - |- O(foo=) O(bar.baz[123].bam[len(x\) - 1]=) - |- O(foo=bar) O(bar.baz
-[123].bam[len(x\) - 1]=bar) - |- O(bam.baz.foo#lookup:foo) O
-(bam.baz.foo#lookup:bar.baz[123].bam[len(x\) - 1]) - |- O(bam.baz.foo#lookup:
-foo=) O(bam.baz.foo#lookup:bar.baz[123].bam[len(x\) - 1]=) - |- O
-(bam.baz.foo#lookup:foo=bar) O(bam.baz.foo#lookup:bar.baz[123].bam[len(x\) -
-1]=bar) - |- O(bam.baz.foo#role:main:foo) O(bam.baz.foo#role:main:bar.baz
-[123].bam[len(x\) - 1]) - |- O(bam.baz.foo#role:main:foo=) O(bam.baz.foo#role:
-main:bar.baz[123].bam[len(x\) - 1]=) - |- O(bam.baz.foo#role:main:foo=bar) O
-(bam.baz.foo#role:main:bar.baz[123].bam[len(x\) - 1]=bar) - |- O(ignore:foo) O
-(ignore:bar.baz[123].bam[len(x\) - 1]) - |- O(ignore:foo=) O(ignore:bar.baz
-[123].bam[len(x\) - 1]=) - |- O(ignore:foo=bar) O(ignore:bar.baz[123].bam[len
-(x\) - 1]=bar) html: |-
+`bam.baz.foo bam.baz.foo_role>`, entrypoint main)\ \ :literal:`bar.baz[123].bam
+[len(x) - 1]=bar` (of role :ref:`bam.baz.foo bam.baz.foo_role>`, entrypoint
+main)\ \ :literal:`foo`\ \ :literal:`bar.baz[123].bam[len(x) - 1]`\ \ :literal:
+`foo=`\ \ :literal:`bar.baz[123].bam[len(x) - 1]=`\ \ :literal:`foo=bar`\ \ :
+literal:`bar.baz[123].bam[len(x) - 1]=bar`\ option_name_current_plugin: source:
+- |- O(foo) O(bar.baz[123].bam[len(x\) - 1]) - |- O(foo=) O(bar.baz[123].bam
+[len(x\) - 1]=) - |- O(foo=bar) O(bar.baz[123].bam[len(x\) - 1]=bar) - |- O
+(bam.baz.foo#lookup:foo) O(bam.baz.foo#lookup:bar.baz[123].bam[len(x\) - 1]) -
+|- O(bam.baz.foo#lookup:foo=) O(bam.baz.foo#lookup:bar.baz[123].bam[len(x\) -
+1]=) - |- O(bam.baz.foo#lookup:foo=bar) O(bam.baz.foo#lookup:bar.baz[123].bam
+[len(x\) - 1]=bar) - |- O(bam.baz.foo#role:main:foo) O(bam.baz.foo#role:main:
+bar.baz[123].bam[len(x\) - 1]) - |- O(bam.baz.foo#role:main:foo=) O
+(bam.baz.foo#role:main:bar.baz[123].bam[len(x\) - 1]=) - |- O(bam.baz.foo#role:
+main:foo=bar) O(bam.baz.foo#role:main:bar.baz[123].bam[len(x\) - 1]=bar) - |- O
+(ignore:foo) O(ignore:bar.baz[123].bam[len(x\) - 1]) - |- O(ignore:foo=) O
+(ignore:bar.baz[123].bam[len(x\) - 1]=) - |- O(ignore:foo=bar) O(ignore:bar.baz
+[123].bam[len(x\) - 1]=bar) html: |-
 foo bar.baz[123].bam[len(x) - 1]
 foo= bar.baz[123].bam[len(x) - 1]=
 foo=bar bar.baz[123].bam[len(x) - 1]=bar
 foo bar.baz[123].bam[len(x) - 1]
 foo= bar.baz[123].bam[len(x) - 1]=
 foo=bar bar.baz[123].bam[len(x) - 1]=bar
 foo bar.baz[123].bam[len(x) - 1]
@@ -235,38 +243,39 @@
 foo=bar bar.baz[123].bam[len(x) - 1]=bar
 foo bar.baz[123].bam[len(x) - 1]
 foo= bar.baz[123].bam[len(x) - 1]=
 foo=bar bar.baz[123].bam[len(x) - 1]=bar
 foo bar.baz[123].bam[len(x) - 1]
 foo= bar.baz[123].bam[len(x) - 1]=
 foo=bar bar.baz[123].bam[len(x) - 1]=bar
-md: |- foo bar.baz\[123\].bam\[len\(x\) \- 1\] foo\= bar.baz\[123\].bam\[len\
-(x\) \- 1\]\= foo\=bar bar.baz\[123\].bam\[len\(x\) \- 1\]\=bar foo bar.baz\
-[123\].bam\[len\(x\) \- 1\] foo\= bar.baz\[123\].bam\[len\(x\) \- 1\]\=
-foo\=bar bar.baz\[123\].bam\[len\(x\) \- 1\]\=bar foo bar.baz\[123\].bam\[len\
-(x\) \- 1\] foo\= bar.baz\[123\].bam\[len\(x\) \- 1\]\= foo\=bar bar.baz\
-[123\].bam\[len\(x\) \- 1\]\=bar foo bar.baz\[123\].bam\[len\(x\) \- 1\] foo\=
-bar.baz\[123\].bam\[len\(x\) \- 1\]\= foo\=bar bar.baz\[123\].bam\[len\(x\) \-
-1\]\=bar rst: |- \ :ansopt:`foo.bar.baz.bam#boo:foo`\ \ :ansopt:
-`foo.bar.baz.bam#boo:bar.baz[123].bam[len(x) - 1]`\ \ :ansopt:
-`foo.bar.baz.bam#boo:foo=`\ \ :ansopt:`foo.bar.baz.bam#boo:bar.baz[123].bam[len
-(x) - 1]=`\ \ :ansopt:`foo.bar.baz.bam#boo:foo=bar`\ \ :ansopt:
-`foo.bar.baz.bam#boo:bar.baz[123].bam[len(x) - 1]=bar`\ \ :ansopt:
-`bam.baz.foo#lookup:foo`\ \ :ansopt:`bam.baz.foo#lookup:bar.baz[123].bam[len(x)
-- 1]`\ \ :ansopt:`bam.baz.foo#lookup:foo=`\ \ :ansopt:`bam.baz.foo#lookup:
-bar.baz[123].bam[len(x) - 1]=`\ \ :ansopt:`bam.baz.foo#lookup:foo=bar`\ \ :
-ansopt:`bam.baz.foo#lookup:bar.baz[123].bam[len(x) - 1]=bar`\ \ :ansopt:
+md: |- foo bar\.baz\[123\]\.bam\[len\(x\) \- 1\] foo\= bar\.baz\[123\]\.bam\
+[len\(x\) \- 1\]\= foo\=bar bar\.baz\[123\]\.bam\[len\(x\) \- 1\]\=bar foo
+bar\.baz\[123\]\.bam\[len\(x\) \- 1\] foo\= bar\.baz\[123\]\.bam\[len\(x\) \-
+1\]\= foo\=bar bar\.baz\[123\]\.bam\[len\(x\) \- 1\]\=bar foo bar\.baz\
+[123\]\.bam\[len\(x\) \- 1\] foo\= bar\.baz\[123\]\.bam\[len\(x\) \- 1\]\=
+foo\=bar bar\.baz\[123\]\.bam\[len\(x\) \- 1\]\=bar foo bar\.baz\[123\]\.bam\
+[len\(x\) \- 1\] foo\= bar\.baz\[123\]\.bam\[len\(x\) \- 1\]\= foo\=bar
+bar\.baz\[123\]\.bam\[len\(x\) \- 1\]\=bar rst: |- \ :ansopt:
+`foo.bar.baz.bam#boo:foo`\ \ :ansopt:`foo.bar.baz.bam#boo:bar.baz[123].bam[len
+(x) - 1]`\ \ :ansopt:`foo.bar.baz.bam#boo:foo=`\ \ :ansopt:
+`foo.bar.baz.bam#boo:bar.baz[123].bam[len(x) - 1]=`\ \ :ansopt:
+`foo.bar.baz.bam#boo:foo=bar`\ \ :ansopt:`foo.bar.baz.bam#boo:bar.baz[123].bam
+[len(x) - 1]=bar`\ \ :ansopt:`bam.baz.foo#lookup:foo`\ \ :ansopt:
+`bam.baz.foo#lookup:bar.baz[123].bam[len(x) - 1]`\ \ :ansopt:
+`bam.baz.foo#lookup:foo=`\ \ :ansopt:`bam.baz.foo#lookup:bar.baz[123].bam[len
+(x) - 1]=`\ \ :ansopt:`bam.baz.foo#lookup:foo=bar`\ \ :ansopt:
+`bam.baz.foo#lookup:bar.baz[123].bam[len(x) - 1]=bar`\ \ :ansopt:
 `bam.baz.foo#role:main:foo`\ \ :ansopt:`bam.baz.foo#role:main:bar.baz[123].bam
 [len(x) - 1]`\ \ :ansopt:`bam.baz.foo#role:main:foo=`\ \ :ansopt:
 `bam.baz.foo#role:main:bar.baz[123].bam[len(x) - 1]=`\ \ :ansopt:
 `bam.baz.foo#role:main:foo=bar`\ \ :ansopt:`bam.baz.foo#role:main:bar.baz
 [123].bam[len(x) - 1]=bar`\ \ :ansopt:`foo`\ \ :ansopt:`bar.baz[123].bam[len(x)
 - 1]`\ \ :ansopt:`foo=`\ \ :ansopt:`bar.baz[123].bam[len(x) - 1]=`\ \ :ansopt:
 `foo=bar`\ \ :ansopt:`bar.baz[123].bam[len(x) - 1]=bar`\ parse_opts:
-current_plugin: fqcn: foo.bar.baz.bam type: boo ansible_doc_text: |- `foo' (of
+currentPlugin: fqcn: foo.bar.baz.bam type: boo ansible_doc_text: |- `foo' (of
 boo plugin foo.bar.baz.bam) `bar.baz[123].bam[len(x) - 1]' (of boo plugin
 foo.bar.baz.bam) `foo=' (of boo plugin foo.bar.baz.bam) `bar.baz[123].bam[len
 (x) - 1]=' (of boo plugin foo.bar.baz.bam) `foo=bar' (of boo plugin
 foo.bar.baz.bam) `bar.baz[123].bam[len(x) - 1]=bar' (of boo plugin
 foo.bar.baz.bam) `foo' (of lookup plugin bam.baz.foo) `bar.baz[123].bam[len(x)
 - 1]' (of lookup plugin bam.baz.foo) `foo=' (of lookup plugin bam.baz.foo)
 `bar.baz[123].bam[len(x) - 1]=' (of lookup plugin bam.baz.foo) `foo=bar' (of
@@ -274,63 +283,54 @@
 bam.baz.foo) `foo' (of role bam.baz.foo, main entrypoint) `bar.baz[123].bam[len
 (x) - 1]' (of role bam.baz.foo, main entrypoint) `foo=' (of role bam.baz.foo,
 main entrypoint) `bar.baz[123].bam[len(x) - 1]=' (of role bam.baz.foo, main
 entrypoint) `foo=bar' (of role bam.baz.foo, main entrypoint) `bar.baz[123].bam
 [len(x) - 1]=bar' (of role bam.baz.foo, main entrypoint) `foo' `bar.baz
 [123].bam[len(x) - 1]' `foo=' `bar.baz[123].bam[len(x) - 1]=' `foo=bar'
 `bar.baz[123].bam[len(x) - 1]=bar' rst_plain: |- \ :literal:`foo` (of boo
-plugin :ref:`foo.bar.baz.bam
-foo.bar.baz.bam_boo>`)\ \ :literal:`bar.baz[123].bam[len(x) - 1]` (of boo
-plugin :ref:`foo.bar.baz.bam
+plugin :ref:`foo.bar.baz.bam foo.bar.baz.bam_boo>`)\ \ :literal:`bar.baz
+[123].bam[len(x) - 1]` (of boo plugin :ref:`foo.bar.baz.bam
 foo.bar.baz.bam_boo>`)\ \ :literal:`foo=` (of boo plugin :ref:`foo.bar.baz.bam
 foo.bar.baz.bam_boo>`)\ \ :literal:`bar.baz[123].bam[len(x) - 1]=` (of boo
-plugin :ref:`foo.bar.baz.bam
-foo.bar.baz.bam_boo>`)\ \ :literal:`foo=bar` (of boo plugin :ref:
-`foo.bar.baz.bam
-foo.bar.baz.bam_boo>`)\ \ :literal:`bar.baz[123].bam[len(x) - 1]=bar` (of boo
-plugin :ref:`foo.bar.baz.bam
+plugin :ref:`foo.bar.baz.bam foo.bar.baz.bam_boo>`)\ \ :literal:`foo=bar` (of
+boo plugin :ref:`foo.bar.baz.bam foo.bar.baz.bam_boo>`)\ \ :literal:`bar.baz
+[123].bam[len(x) - 1]=bar` (of boo plugin :ref:`foo.bar.baz.bam
 foo.bar.baz.bam_boo>`)\ \ :literal:`foo` (of lookup plugin :ref:`bam.baz.foo
 bam.baz.foo_lookup>`)\ \ :literal:`bar.baz[123].bam[len(x) - 1]` (of lookup
-plugin :ref:`bam.baz.foo
-bam.baz.foo_lookup>`)\ \ :literal:`foo=` (of lookup plugin :ref:`bam.baz.foo
-bam.baz.foo_lookup>`)\ \ :literal:`bar.baz[123].bam[len(x) - 1]=` (of lookup
-plugin :ref:`bam.baz.foo
-bam.baz.foo_lookup>`)\ \ :literal:`foo=bar` (of lookup plugin :ref:`bam.baz.foo
-bam.baz.foo_lookup>`)\ \ :literal:`bar.baz[123].bam[len(x) - 1]=bar` (of lookup
-plugin :ref:`bam.baz.foo
+plugin :ref:`bam.baz.foo bam.baz.foo_lookup>`)\ \ :literal:`foo=` (of lookup
+plugin :ref:`bam.baz.foo bam.baz.foo_lookup>`)\ \ :literal:`bar.baz[123].bam
+[len(x) - 1]=` (of lookup plugin :ref:`bam.baz.foo bam.baz.foo_lookup>`)\ \ :
+literal:`foo=bar` (of lookup plugin :ref:`bam.baz.foo bam.baz.foo_lookup>`)\ \
+:literal:`bar.baz[123].bam[len(x) - 1]=bar` (of lookup plugin :ref:`bam.baz.foo
 bam.baz.foo_lookup>`)\ \ :literal:`foo` (of role :ref:`bam.baz.foo
 bam.baz.foo_role>`, entrypoint main)\ \ :literal:`bar.baz[123].bam[len(x) - 1]`
-(of role :ref:`bam.baz.foo
-bam.baz.foo_role>`, entrypoint main)\ \ :literal:`foo=` (of role :ref:
-`bam.baz.foo
-bam.baz.foo_role>`, entrypoint main)\ \ :literal:`bar.baz[123].bam[len(x) -
-1]=` (of role :ref:`bam.baz.foo
+(of role :ref:`bam.baz.foo bam.baz.foo_role>`, entrypoint main)\ \ :literal:
+`foo=` (of role :ref:`bam.baz.foo bam.baz.foo_role>`, entrypoint main)\ \ :
+literal:`bar.baz[123].bam[len(x) - 1]=` (of role :ref:`bam.baz.foo
 bam.baz.foo_role>`, entrypoint main)\ \ :literal:`foo=bar` (of role :ref:
-`bam.baz.foo
-bam.baz.foo_role>`, entrypoint main)\ \ :literal:`bar.baz[123].bam[len(x) -
-1]=bar` (of role :ref:`bam.baz.foo
-bam.baz.foo_role>`, entrypoint main)\ \ :literal:`foo`\ \ :literal:`bar.baz
-[123].bam[len(x) - 1]`\ \ :literal:`foo=`\ \ :literal:`bar.baz[123].bam[len(x)
-- 1]=`\ \ :literal:`foo=bar`\ \ :literal:`bar.baz[123].bam[len(x) - 1]=bar`\
-option_name_current_role: source: - |- O(foo) O(bar.baz[123].bam[len(x\) - 1])
-- |- O(foo=) O(bar.baz[123].bam[len(x\) - 1]=) - |- O(foo=bar) O(bar.baz
-[123].bam[len(x\) - 1]=bar) - |- O(other_entrypoint:foo) O(other_entrypoint:
-bar.baz[123].bam[len(x\) - 1]) - |- O(other_entrypoint:foo=) O
-(other_entrypoint:bar.baz[123].bam[len(x\) - 1]=) - |- O(other_entrypoint:
-foo=bar) O(other_entrypoint:bar.baz[123].bam[len(x\) - 1]=bar) - |- O
-(bam.baz.foo#lookup:foo) O(bam.baz.foo#lookup:bar.baz[123].bam[len(x\) - 1]) -
-|- O(bam.baz.foo#lookup:foo=) O(bam.baz.foo#lookup:bar.baz[123].bam[len(x\) -
-1]=) - |- O(bam.baz.foo#lookup:foo=bar) O(bam.baz.foo#lookup:bar.baz[123].bam
-[len(x\) - 1]=bar) - |- O(bam.baz.foo#role:main:foo) O(bam.baz.foo#role:main:
-bar.baz[123].bam[len(x\) - 1]) - |- O(bam.baz.foo#role:main:foo=) O
-(bam.baz.foo#role:main:bar.baz[123].bam[len(x\) - 1]=) - |- O(bam.baz.foo#role:
-main:foo=bar) O(bam.baz.foo#role:main:bar.baz[123].bam[len(x\) - 1]=bar) - |- O
-(ignore:foo) O(ignore:bar.baz[123].bam[len(x\) - 1]) - |- O(ignore:foo=) O
-(ignore:bar.baz[123].bam[len(x\) - 1]=) - |- O(ignore:foo=bar) O(ignore:bar.baz
-[123].bam[len(x\) - 1]=bar) html: |-
+`bam.baz.foo bam.baz.foo_role>`, entrypoint main)\ \ :literal:`bar.baz[123].bam
+[len(x) - 1]=bar` (of role :ref:`bam.baz.foo bam.baz.foo_role>`, entrypoint
+main)\ \ :literal:`foo`\ \ :literal:`bar.baz[123].bam[len(x) - 1]`\ \ :literal:
+`foo=`\ \ :literal:`bar.baz[123].bam[len(x) - 1]=`\ \ :literal:`foo=bar`\ \ :
+literal:`bar.baz[123].bam[len(x) - 1]=bar`\ option_name_current_role: source: -
+|- O(foo) O(bar.baz[123].bam[len(x\) - 1]) - |- O(foo=) O(bar.baz[123].bam[len
+(x\) - 1]=) - |- O(foo=bar) O(bar.baz[123].bam[len(x\) - 1]=bar) - |- O
+(other_entrypoint:foo) O(other_entrypoint:bar.baz[123].bam[len(x\) - 1]) - |- O
+(other_entrypoint:foo=) O(other_entrypoint:bar.baz[123].bam[len(x\) - 1]=) - |-
+O(other_entrypoint:foo=bar) O(other_entrypoint:bar.baz[123].bam[len(x\) -
+1]=bar) - |- O(bam.baz.foo#lookup:foo) O(bam.baz.foo#lookup:bar.baz[123].bam
+[len(x\) - 1]) - |- O(bam.baz.foo#lookup:foo=) O(bam.baz.foo#lookup:bar.baz
+[123].bam[len(x\) - 1]=) - |- O(bam.baz.foo#lookup:foo=bar) O
+(bam.baz.foo#lookup:bar.baz[123].bam[len(x\) - 1]=bar) - |- O(bam.baz.foo#role:
+main:foo) O(bam.baz.foo#role:main:bar.baz[123].bam[len(x\) - 1]) - |- O
+(bam.baz.foo#role:main:foo=) O(bam.baz.foo#role:main:bar.baz[123].bam[len(x\) -
+1]=) - |- O(bam.baz.foo#role:main:foo=bar) O(bam.baz.foo#role:main:bar.baz
+[123].bam[len(x\) - 1]=bar) - |- O(ignore:foo) O(ignore:bar.baz[123].bam[len
+(x\) - 1]) - |- O(ignore:foo=) O(ignore:bar.baz[123].bam[len(x\) - 1]=) - |- O
+(ignore:foo=bar) O(ignore:bar.baz[123].bam[len(x\) - 1]=bar) html: |-
 foo bar.baz[123].bam[len(x) - 1]
 foo= bar.baz[123].bam[len(x) - 1]=
 foo=bar bar.baz[123].bam[len(x) - 1]=bar
 foo bar.baz[123].bam[len(x) - 1]
 foo= bar.baz[123].bam[len(x) - 1]=
 foo=bar bar.baz[123].bam[len(x) - 1]=bar
 foo bar.baz[123].bam[len(x) - 1]
@@ -354,113 +354,101 @@
 foo=bar bar.baz[123].bam[len(x) - 1]=bar
 foo bar.baz[123].bam[len(x) - 1]
 foo= bar.baz[123].bam[len(x) - 1]=
 foo=bar bar.baz[123].bam[len(x) - 1]=bar
 foo bar.baz[123].bam[len(x) - 1]
 foo= bar.baz[123].bam[len(x) - 1]=
 foo=bar bar.baz[123].bam[len(x) - 1]=bar
-md: |- foo bar.baz\[123\].bam\[len\(x\) \- 1\] foo\= bar.baz\[123\].bam\[len\
-(x\) \- 1\]\= foo\=bar bar.baz\[123\].bam\[len\(x\) \- 1\]\=bar foo bar.baz\
-[123\].bam\[len\(x\) \- 1\] foo\= bar.baz\[123\].bam\[len\(x\) \- 1\]\=
-foo\=bar bar.baz\[123\].bam\[len\(x\) \- 1\]\=bar foo bar.baz\[123\].bam\[len\
-(x\) \- 1\] foo\= bar.baz\[123\].bam\[len\(x\) \- 1\]\= foo\=bar bar.baz\
-[123\].bam\[len\(x\) \- 1\]\=bar foo bar.baz\[123\].bam\[len\(x\) \- 1\] foo\=
-bar.baz\[123\].bam\[len\(x\) \- 1\]\= foo\=bar bar.baz\[123\].bam\[len\(x\) \-
-1\]\=bar foo bar.baz\[123\].bam\[len\(x\) \- 1\] foo\= bar.baz\[123\].bam\[len\
-(x\) \- 1\]\= foo\=bar bar.baz\[123\].bam\[len\(x\) \- 1\]\=bar rst: |- \ :
-ansopt:`foo.bar.baz#role:main:foo`\ \ :ansopt:`foo.bar.baz#role:main:bar.baz
-[123].bam[len(x) - 1]`\ \ :ansopt:`foo.bar.baz#role:main:foo=`\ \ :ansopt:
-`foo.bar.baz#role:main:bar.baz[123].bam[len(x) - 1]=`\ \ :ansopt:
-`foo.bar.baz#role:main:foo=bar`\ \ :ansopt:`foo.bar.baz#role:main:bar.baz
-[123].bam[len(x) - 1]=bar`\ \ :ansopt:`foo.bar.baz#role:other\_entrypoint:foo`\
-\ :ansopt:`foo.bar.baz#role:other\_entrypoint:bar.baz[123].bam[len(x) - 1]`\ \
-:ansopt:`foo.bar.baz#role:other\_entrypoint:foo=`\ \ :ansopt:`foo.bar.baz#role:
-other\_entrypoint:bar.baz[123].bam[len(x) - 1]=`\ \ :ansopt:`foo.bar.baz#role:
-other\_entrypoint:foo=bar`\ \ :ansopt:`foo.bar.baz#role:other\_entrypoint:
-bar.baz[123].bam[len(x) - 1]=bar`\ \ :ansopt:`bam.baz.foo#lookup:foo`\ \ :
-ansopt:`bam.baz.foo#lookup:bar.baz[123].bam[len(x) - 1]`\ \ :ansopt:
-`bam.baz.foo#lookup:foo=`\ \ :ansopt:`bam.baz.foo#lookup:bar.baz[123].bam[len
-(x) - 1]=`\ \ :ansopt:`bam.baz.foo#lookup:foo=bar`\ \ :ansopt:
-`bam.baz.foo#lookup:bar.baz[123].bam[len(x) - 1]=bar`\ \ :ansopt:
-`bam.baz.foo#role:main:foo`\ \ :ansopt:`bam.baz.foo#role:main:bar.baz[123].bam
-[len(x) - 1]`\ \ :ansopt:`bam.baz.foo#role:main:foo=`\ \ :ansopt:
-`bam.baz.foo#role:main:bar.baz[123].bam[len(x) - 1]=`\ \ :ansopt:
-`bam.baz.foo#role:main:foo=bar`\ \ :ansopt:`bam.baz.foo#role:main:bar.baz
-[123].bam[len(x) - 1]=bar`\ \ :ansopt:`foo`\ \ :ansopt:`bar.baz[123].bam[len(x)
-- 1]`\ \ :ansopt:`foo=`\ \ :ansopt:`bar.baz[123].bam[len(x) - 1]=`\ \ :ansopt:
-`foo=bar`\ \ :ansopt:`bar.baz[123].bam[len(x) - 1]=bar`\ parse_opts:
-current_plugin: fqcn: foo.bar.baz type: role role_entrypoint: main
-ansible_doc_text: |- `foo' (of role foo.bar.baz, main entrypoint) `bar.baz
-[123].bam[len(x) - 1]' (of role foo.bar.baz, main entrypoint) `foo=' (of role
-foo.bar.baz, main entrypoint) `bar.baz[123].bam[len(x) - 1]=' (of role
-foo.bar.baz, main entrypoint) `foo=bar' (of role foo.bar.baz, main entrypoint)
-`bar.baz[123].bam[len(x) - 1]=bar' (of role foo.bar.baz, main entrypoint) `foo'
-(of role foo.bar.baz, other_entrypoint entrypoint) `bar.baz[123].bam[len(x) -
-1]' (of role foo.bar.baz, other_entrypoint entrypoint) `foo=' (of role
-foo.bar.baz, other_entrypoint entrypoint) `bar.baz[123].bam[len(x) - 1]=' (of
-role foo.bar.baz, other_entrypoint entrypoint) `foo=bar' (of role foo.bar.baz,
-other_entrypoint entrypoint) `bar.baz[123].bam[len(x) - 1]=bar' (of role
-foo.bar.baz, other_entrypoint entrypoint) `foo' (of lookup plugin bam.baz.foo)
-`bar.baz[123].bam[len(x) - 1]' (of lookup plugin bam.baz.foo) `foo=' (of lookup
-plugin bam.baz.foo) `bar.baz[123].bam[len(x) - 1]=' (of lookup plugin
-bam.baz.foo) `foo=bar' (of lookup plugin bam.baz.foo) `bar.baz[123].bam[len(x)
-- 1]=bar' (of lookup plugin bam.baz.foo) `foo' (of role bam.baz.foo, main
-entrypoint) `bar.baz[123].bam[len(x) - 1]' (of role bam.baz.foo, main
-entrypoint) `foo=' (of role bam.baz.foo, main entrypoint) `bar.baz[123].bam[len
-(x) - 1]=' (of role bam.baz.foo, main entrypoint) `foo=bar' (of role
-bam.baz.foo, main entrypoint) `bar.baz[123].bam[len(x) - 1]=bar' (of role
-bam.baz.foo, main entrypoint) `foo' `bar.baz[123].bam[len(x) - 1]' `foo='
-`bar.baz[123].bam[len(x) - 1]=' `foo=bar' `bar.baz[123].bam[len(x) - 1]=bar'
-rst_plain: |- \ :literal:`foo` (of role :ref:`foo.bar.baz
-foo.bar.baz_role>`, entrypoint main)\ \ :literal:`bar.baz[123].bam[len(x) - 1]`
-(of role :ref:`foo.bar.baz
-foo.bar.baz_role>`, entrypoint main)\ \ :literal:`foo=` (of role :ref:
-`foo.bar.baz
-foo.bar.baz_role>`, entrypoint main)\ \ :literal:`bar.baz[123].bam[len(x) -
-1]=` (of role :ref:`foo.bar.baz
-foo.bar.baz_role>`, entrypoint main)\ \ :literal:`foo=bar` (of role :ref:
-`foo.bar.baz
+md: |- foo bar\.baz\[123\]\.bam\[len\(x\) \- 1\] foo\= bar\.baz\[123\]\.bam\
+[len\(x\) \- 1\]\= foo\=bar bar\.baz\[123\]\.bam\[len\(x\) \- 1\]\=bar foo
+bar\.baz\[123\]\.bam\[len\(x\) \- 1\] foo\= bar\.baz\[123\]\.bam\[len\(x\) \-
+1\]\= foo\=bar bar\.baz\[123\]\.bam\[len\(x\) \- 1\]\=bar foo bar\.baz\
+[123\]\.bam\[len\(x\) \- 1\] foo\= bar\.baz\[123\]\.bam\[len\(x\) \- 1\]\=
+foo\=bar bar\.baz\[123\]\.bam\[len\(x\) \- 1\]\=bar foo bar\.baz\[123\]\.bam\
+[len\(x\) \- 1\] foo\= bar\.baz\[123\]\.bam\[len\(x\) \- 1\]\= foo\=bar
+bar\.baz\[123\]\.bam\[len\(x\) \- 1\]\=bar foo bar\.baz\[123\]\.bam\[len\(x\)
+\- 1\] foo\= bar\.baz\[123\]\.bam\[len\(x\) \- 1\]\= foo\=bar bar\.baz\
+[123\]\.bam\[len\(x\) \- 1\]\=bar rst: |- \ :ansopt:`foo.bar.baz#role:main:
+foo`\ \ :ansopt:`foo.bar.baz#role:main:bar.baz[123].bam[len(x) - 1]`\ \ :
+ansopt:`foo.bar.baz#role:main:foo=`\ \ :ansopt:`foo.bar.baz#role:main:bar.baz
+[123].bam[len(x) - 1]=`\ \ :ansopt:`foo.bar.baz#role:main:foo=bar`\ \ :ansopt:
+`foo.bar.baz#role:main:bar.baz[123].bam[len(x) - 1]=bar`\ \ :ansopt:
+`foo.bar.baz#role:other\_entrypoint:foo`\ \ :ansopt:`foo.bar.baz#role:
+other\_entrypoint:bar.baz[123].bam[len(x) - 1]`\ \ :ansopt:`foo.bar.baz#role:
+other\_entrypoint:foo=`\ \ :ansopt:`foo.bar.baz#role:other\_entrypoint:bar.baz
+[123].bam[len(x) - 1]=`\ \ :ansopt:`foo.bar.baz#role:other\_entrypoint:
+foo=bar`\ \ :ansopt:`foo.bar.baz#role:other\_entrypoint:bar.baz[123].bam[len(x)
+- 1]=bar`\ \ :ansopt:`bam.baz.foo#lookup:foo`\ \ :ansopt:`bam.baz.foo#lookup:
+bar.baz[123].bam[len(x) - 1]`\ \ :ansopt:`bam.baz.foo#lookup:foo=`\ \ :ansopt:
+`bam.baz.foo#lookup:bar.baz[123].bam[len(x) - 1]=`\ \ :ansopt:
+`bam.baz.foo#lookup:foo=bar`\ \ :ansopt:`bam.baz.foo#lookup:bar.baz[123].bam
+[len(x) - 1]=bar`\ \ :ansopt:`bam.baz.foo#role:main:foo`\ \ :ansopt:
+`bam.baz.foo#role:main:bar.baz[123].bam[len(x) - 1]`\ \ :ansopt:
+`bam.baz.foo#role:main:foo=`\ \ :ansopt:`bam.baz.foo#role:main:bar.baz[123].bam
+[len(x) - 1]=`\ \ :ansopt:`bam.baz.foo#role:main:foo=bar`\ \ :ansopt:
+`bam.baz.foo#role:main:bar.baz[123].bam[len(x) - 1]=bar`\ \ :ansopt:`foo`\ \ :
+ansopt:`bar.baz[123].bam[len(x) - 1]`\ \ :ansopt:`foo=`\ \ :ansopt:`bar.baz
+[123].bam[len(x) - 1]=`\ \ :ansopt:`foo=bar`\ \ :ansopt:`bar.baz[123].bam[len
+(x) - 1]=bar`\ parse_opts: currentPlugin: fqcn: foo.bar.baz type: role
+roleEntrypoint: main ansible_doc_text: |- `foo' (of role foo.bar.baz, main
+entrypoint) `bar.baz[123].bam[len(x) - 1]' (of role foo.bar.baz, main
+entrypoint) `foo=' (of role foo.bar.baz, main entrypoint) `bar.baz[123].bam[len
+(x) - 1]=' (of role foo.bar.baz, main entrypoint) `foo=bar' (of role
+foo.bar.baz, main entrypoint) `bar.baz[123].bam[len(x) - 1]=bar' (of role
+foo.bar.baz, main entrypoint) `foo' (of role foo.bar.baz, other_entrypoint
+entrypoint) `bar.baz[123].bam[len(x) - 1]' (of role foo.bar.baz,
+other_entrypoint entrypoint) `foo=' (of role foo.bar.baz, other_entrypoint
+entrypoint) `bar.baz[123].bam[len(x) - 1]=' (of role foo.bar.baz,
+other_entrypoint entrypoint) `foo=bar' (of role foo.bar.baz, other_entrypoint
+entrypoint) `bar.baz[123].bam[len(x) - 1]=bar' (of role foo.bar.baz,
+other_entrypoint entrypoint) `foo' (of lookup plugin bam.baz.foo) `bar.baz
+[123].bam[len(x) - 1]' (of lookup plugin bam.baz.foo) `foo=' (of lookup plugin
+bam.baz.foo) `bar.baz[123].bam[len(x) - 1]=' (of lookup plugin bam.baz.foo)
+`foo=bar' (of lookup plugin bam.baz.foo) `bar.baz[123].bam[len(x) - 1]=bar' (of
+lookup plugin bam.baz.foo) `foo' (of role bam.baz.foo, main entrypoint)
+`bar.baz[123].bam[len(x) - 1]' (of role bam.baz.foo, main entrypoint) `foo='
+(of role bam.baz.foo, main entrypoint) `bar.baz[123].bam[len(x) - 1]=' (of role
+bam.baz.foo, main entrypoint) `foo=bar' (of role bam.baz.foo, main entrypoint)
+`bar.baz[123].bam[len(x) - 1]=bar' (of role bam.baz.foo, main entrypoint) `foo'
+`bar.baz[123].bam[len(x) - 1]' `foo=' `bar.baz[123].bam[len(x) - 1]=' `foo=bar'
+`bar.baz[123].bam[len(x) - 1]=bar' rst_plain: |- \ :literal:`foo` (of role :
+ref:`foo.bar.baz foo.bar.baz_role>`, entrypoint main)\ \ :literal:`bar.baz
+[123].bam[len(x) - 1]` (of role :ref:`foo.bar.baz foo.bar.baz_role>`,
+entrypoint main)\ \ :literal:`foo=` (of role :ref:`foo.bar.baz
 foo.bar.baz_role>`, entrypoint main)\ \ :literal:`bar.baz[123].bam[len(x) -
-1]=bar` (of role :ref:`foo.bar.baz
+1]=` (of role :ref:`foo.bar.baz foo.bar.baz_role>`, entrypoint main)\ \ :
+literal:`foo=bar` (of role :ref:`foo.bar.baz foo.bar.baz_role>`, entrypoint
+main)\ \ :literal:`bar.baz[123].bam[len(x) - 1]=bar` (of role :ref:`foo.bar.baz
 foo.bar.baz_role>`, entrypoint main)\ \ :literal:`foo` (of role :ref:
-`foo.bar.baz
+`foo.bar.baz foo.bar.baz_role>`, entrypoint other\_entrypoint)\ \ :literal:
+`bar.baz[123].bam[len(x) - 1]` (of role :ref:`foo.bar.baz foo.bar.baz_role>`,
+entrypoint other\_entrypoint)\ \ :literal:`foo=` (of role :ref:`foo.bar.baz
 foo.bar.baz_role>`, entrypoint other\_entrypoint)\ \ :literal:`bar.baz[123].bam
-[len(x) - 1]` (of role :ref:`foo.bar.baz
-foo.bar.baz_role>`, entrypoint other\_entrypoint)\ \ :literal:`foo=` (of role :
-ref:`foo.bar.baz
+[len(x) - 1]=` (of role :ref:`foo.bar.baz foo.bar.baz_role>`, entrypoint
+other\_entrypoint)\ \ :literal:`foo=bar` (of role :ref:`foo.bar.baz
 foo.bar.baz_role>`, entrypoint other\_entrypoint)\ \ :literal:`bar.baz[123].bam
-[len(x) - 1]=` (of role :ref:`foo.bar.baz
-foo.bar.baz_role>`, entrypoint other\_entrypoint)\ \ :literal:`foo=bar` (of
-role :ref:`foo.bar.baz
-foo.bar.baz_role>`, entrypoint other\_entrypoint)\ \ :literal:`bar.baz[123].bam
-[len(x) - 1]=bar` (of role :ref:`foo.bar.baz
-foo.bar.baz_role>`, entrypoint other\_entrypoint)\ \ :literal:`foo` (of lookup
-plugin :ref:`bam.baz.foo
+[len(x) - 1]=bar` (of role :ref:`foo.bar.baz foo.bar.baz_role>`, entrypoint
+other\_entrypoint)\ \ :literal:`foo` (of lookup plugin :ref:`bam.baz.foo
 bam.baz.foo_lookup>`)\ \ :literal:`bar.baz[123].bam[len(x) - 1]` (of lookup
-plugin :ref:`bam.baz.foo
-bam.baz.foo_lookup>`)\ \ :literal:`foo=` (of lookup plugin :ref:`bam.baz.foo
-bam.baz.foo_lookup>`)\ \ :literal:`bar.baz[123].bam[len(x) - 1]=` (of lookup
-plugin :ref:`bam.baz.foo
-bam.baz.foo_lookup>`)\ \ :literal:`foo=bar` (of lookup plugin :ref:`bam.baz.foo
-bam.baz.foo_lookup>`)\ \ :literal:`bar.baz[123].bam[len(x) - 1]=bar` (of lookup
-plugin :ref:`bam.baz.foo
+plugin :ref:`bam.baz.foo bam.baz.foo_lookup>`)\ \ :literal:`foo=` (of lookup
+plugin :ref:`bam.baz.foo bam.baz.foo_lookup>`)\ \ :literal:`bar.baz[123].bam
+[len(x) - 1]=` (of lookup plugin :ref:`bam.baz.foo bam.baz.foo_lookup>`)\ \ :
+literal:`foo=bar` (of lookup plugin :ref:`bam.baz.foo bam.baz.foo_lookup>`)\ \
+:literal:`bar.baz[123].bam[len(x) - 1]=bar` (of lookup plugin :ref:`bam.baz.foo
 bam.baz.foo_lookup>`)\ \ :literal:`foo` (of role :ref:`bam.baz.foo
 bam.baz.foo_role>`, entrypoint main)\ \ :literal:`bar.baz[123].bam[len(x) - 1]`
-(of role :ref:`bam.baz.foo
-bam.baz.foo_role>`, entrypoint main)\ \ :literal:`foo=` (of role :ref:
-`bam.baz.foo
-bam.baz.foo_role>`, entrypoint main)\ \ :literal:`bar.baz[123].bam[len(x) -
-1]=` (of role :ref:`bam.baz.foo
+(of role :ref:`bam.baz.foo bam.baz.foo_role>`, entrypoint main)\ \ :literal:
+`foo=` (of role :ref:`bam.baz.foo bam.baz.foo_role>`, entrypoint main)\ \ :
+literal:`bar.baz[123].bam[len(x) - 1]=` (of role :ref:`bam.baz.foo
 bam.baz.foo_role>`, entrypoint main)\ \ :literal:`foo=bar` (of role :ref:
-`bam.baz.foo
-bam.baz.foo_role>`, entrypoint main)\ \ :literal:`bar.baz[123].bam[len(x) -
-1]=bar` (of role :ref:`bam.baz.foo
-bam.baz.foo_role>`, entrypoint main)\ \ :literal:`foo`\ \ :literal:`bar.baz
-[123].bam[len(x) - 1]`\ \ :literal:`foo=`\ \ :literal:`bar.baz[123].bam[len(x)
-- 1]=`\ \ :literal:`foo=bar`\ \ :literal:`bar.baz[123].bam[len(x) - 1]=bar`\
+`bam.baz.foo bam.baz.foo_role>`, entrypoint main)\ \ :literal:`bar.baz[123].bam
+[len(x) - 1]=bar` (of role :ref:`bam.baz.foo bam.baz.foo_role>`, entrypoint
+main)\ \ :literal:`foo`\ \ :literal:`bar.baz[123].bam[len(x) - 1]`\ \ :literal:
+`foo=`\ \ :literal:`bar.baz[123].bam[len(x) - 1]=`\ \ :literal:`foo=bar`\ \ :
+literal:`bar.baz[123].bam[len(x) - 1]=bar`\
 option_name_no_current_plugin_w_links: source: - |- O(foo) O(bar.baz[123].bam
 [len(x\) - 1]) - |- O(foo=) O(bar.baz[123].bam[len(x\) - 1]=) - |- O(foo=bar) O
 (bar.baz[123].bam[len(x\) - 1]=bar) - |- O(bam.baz.foo#lookup:foo) O
 (bam.baz.foo#lookup:bar.baz[123].bam[len(x\) - 1]) - |- O(bam.baz.foo#lookup:
 foo=) O(bam.baz.foo#lookup:bar.baz[123].bam[len(x\) - 1]=) - |- O
 (bam.baz.foo#lookup:foo=bar) O(bam.baz.foo#lookup:bar.baz[123].bam[len(x\) -
 1]=bar) - |- O(bam.baz.foo#role:main:foo) O(bam.baz.foo#role:main:bar.baz
@@ -497,93 +485,87 @@
 foo=bar bar.baz[123].bam[len(x)_-_1]=bar
 foo bar.baz[123].bam[len(x)_-_1]
 foo= bar.baz[123].bam[len(x)_-_1]=
 foo=bar bar.baz[123].bam[len(x)_-_1]=bar
 foo bar.baz[123].bam[len(x) - 1]
 foo= bar.baz[123].bam[len(x) - 1]=
 foo=bar bar.baz[123].bam[len(x) - 1]=bar
-md: |- foo bar.baz\[123\].bam\[len\(x\) \- 1\] foo\= bar.baz\[123\].bam\[len\
-(x\) \- 1\]\= foo\=bar bar.baz\[123\].bam\[len\(x\) \- 1\]\=bar foo bar.baz\
-[123\].bam\[len\(x\)_\-_1\] foo\= bar.baz\[123\].bam\[len\(x\)_\-_1\]\=
-foo\=bar bar.baz\[123\].bam\[len\(x\)_\-_1\]\=bar foo bar.baz\[123\].bam\[len\
-(x\)_\-_1\] foo\= bar.baz\[123\].bam\[len\(x\)_\-_1\]\= foo\=bar bar.baz\
-[123\].bam\[len\(x\)_\-_1\]\=bar foo bar.baz\[123\].bam\[len\(x\) \- 1\] foo\=
-bar.baz\[123\].bam\[len\(x\) \- 1\]\= foo\=bar bar.baz\[123\].bam\[len\(x\) \-
-1\]\=bar md_opts: pluginOptionLikeLink.js: |- (plugin, entrypoint, what, name,
-current_plugin) => `https://docs.ansible.com/ansible/devel/collections/$
-{plugin.fqcn.replace(/\./g, '/')}_${plugin.type}.html#${what}${entrypoint ? '-
-' + entrypoint : ''}-${name.join('/')}` pluginOptionLikeLink.py: |- lambda
-plugin, entrypoint, what, name, current_plugin: f"https://docs.ansible.com/
-ansible/devel/collections/{plugin.fqcn.replace('.', '/')}_{plugin.type}.html#
-{what}{'-' + entrypoint if entrypoint else ''}-{'/'.join(name)}" rst: |- \ :
-ansopt:`foo`\ \ :ansopt:`bar.baz[123].bam[len(x) - 1]`\ \ :ansopt:`foo=`\ \ :
-ansopt:`bar.baz[123].bam[len(x) - 1]=`\ \ :ansopt:`foo=bar`\ \ :ansopt:`bar.baz
-[123].bam[len(x) - 1]=bar`\ \ :ansopt:`bam.baz.foo#lookup:foo`\ \ :ansopt:
-`bam.baz.foo#lookup:bar.baz[123].bam[len(x) - 1]`\ \ :ansopt:
-`bam.baz.foo#lookup:foo=`\ \ :ansopt:`bam.baz.foo#lookup:bar.baz[123].bam[len
-(x) - 1]=`\ \ :ansopt:`bam.baz.foo#lookup:foo=bar`\ \ :ansopt:
-`bam.baz.foo#lookup:bar.baz[123].bam[len(x) - 1]=bar`\ \ :ansopt:
-`bam.baz.foo#role:main:foo`\ \ :ansopt:`bam.baz.foo#role:main:bar.baz[123].bam
-[len(x) - 1]`\ \ :ansopt:`bam.baz.foo#role:main:foo=`\ \ :ansopt:
-`bam.baz.foo#role:main:bar.baz[123].bam[len(x) - 1]=`\ \ :ansopt:
-`bam.baz.foo#role:main:foo=bar`\ \ :ansopt:`bam.baz.foo#role:main:bar.baz
-[123].bam[len(x) - 1]=bar`\ \ :ansopt:`foo`\ \ :ansopt:`bar.baz[123].bam[len(x)
-- 1]`\ \ :ansopt:`foo=`\ \ :ansopt:`bar.baz[123].bam[len(x) - 1]=`\ \ :ansopt:
-`foo=bar`\ \ :ansopt:`bar.baz[123].bam[len(x) - 1]=bar`\ ansible_doc_text: |-
-`foo' `bar.baz[123].bam[len(x) - 1]' `foo=' `bar.baz[123].bam[len(x) - 1]='
-`foo=bar' `bar.baz[123].bam[len(x) - 1]=bar' `foo' (of lookup plugin
-bam.baz.foo) `bar.baz[123].bam[len(x) - 1]' (of lookup plugin bam.baz.foo)
-`foo=' (of lookup plugin bam.baz.foo) `bar.baz[123].bam[len(x) - 1]=' (of
-lookup plugin bam.baz.foo) `foo=bar' (of lookup plugin bam.baz.foo) `bar.baz
-[123].bam[len(x) - 1]=bar' (of lookup plugin bam.baz.foo) `foo' (of role
-bam.baz.foo, main entrypoint) `bar.baz[123].bam[len(x) - 1]' (of role
-bam.baz.foo, main entrypoint) `foo=' (of role bam.baz.foo, main entrypoint)
-`bar.baz[123].bam[len(x) - 1]=' (of role bam.baz.foo, main entrypoint)
-`foo=bar' (of role bam.baz.foo, main entrypoint) `bar.baz[123].bam[len(x) -
-1]=bar' (of role bam.baz.foo, main entrypoint) `foo' `bar.baz[123].bam[len(x) -
-1]' `foo=' `bar.baz[123].bam[len(x) - 1]=' `foo=bar' `bar.baz[123].bam[len(x) -
-1]=bar' rst_plain: |- \ :literal:`foo`\ \ :literal:`bar.baz[123].bam[len(x) -
-1]`\ \ :literal:`foo=`\ \ :literal:`bar.baz[123].bam[len(x) - 1]=`\ \ :literal:
-`foo=bar`\ \ :literal:`bar.baz[123].bam[len(x) - 1]=bar`\ \ :literal:`foo` (of
-lookup plugin :ref:`bam.baz.foo
+md: |- foo bar\.baz\[123\]\.bam\[len\(x\) \- 1\] foo\= bar\.baz\[123\]\.bam\
+[len\(x\) \- 1\]\= foo\=bar bar\.baz\[123\]\.bam\[len\(x\) \- 1\]\=bar foo
+bar\.baz\[123\]\.bam\[len\(x\)_\-_1\] foo\= bar\.baz\[123\]\.bam\[len\(x\)_\-
+1\]\= foo\=bar bar\.baz\[123\]\.bam\[len\(x\)_\-_1\]\=bar foo bar\.baz\
+[123\]\.bam\[len\(x\)_\-_1\] foo\= bar\.baz\[123\]\.bam\[len\(x\)_\-_1\]\=
+foo\=bar bar\.baz\[123\]\.bam\[len\(x\)_\-_1\]\=bar foo bar\.baz\[123\]\.bam\
+[len\(x\) \- 1\] foo\= bar\.baz\[123\]\.bam\[len\(x\) \- 1\]\= foo\=bar
+bar\.baz\[123\]\.bam\[len\(x\) \- 1\]\=bar md_opts: pluginOptionLikeLink.js: |-
+(plugin, entrypoint, what, name, current_plugin) => `https://docs.ansible.com/
+ansible/devel/collections/${plugin.fqcn.replace(/\./g, '/')}_$
+{plugin.type}.html#${what}${entrypoint ? '-' + entrypoint : ''}-${name.join('/
+')}` pluginOptionLikeLink.py: |- lambda plugin, entrypoint, what, name,
+current_plugin: f"https://docs.ansible.com/ansible/devel/collections/
+{plugin.fqcn.replace('.', '/')}_{plugin.type}.html#{what}{'-' + entrypoint if
+entrypoint else ''}-{'/'.join(name)}" rst: |- \ :ansopt:`foo`\ \ :ansopt:
+`bar.baz[123].bam[len(x) - 1]`\ \ :ansopt:`foo=`\ \ :ansopt:`bar.baz[123].bam
+[len(x) - 1]=`\ \ :ansopt:`foo=bar`\ \ :ansopt:`bar.baz[123].bam[len(x) -
+1]=bar`\ \ :ansopt:`bam.baz.foo#lookup:foo`\ \ :ansopt:`bam.baz.foo#lookup:
+bar.baz[123].bam[len(x) - 1]`\ \ :ansopt:`bam.baz.foo#lookup:foo=`\ \ :ansopt:
+`bam.baz.foo#lookup:bar.baz[123].bam[len(x) - 1]=`\ \ :ansopt:
+`bam.baz.foo#lookup:foo=bar`\ \ :ansopt:`bam.baz.foo#lookup:bar.baz[123].bam
+[len(x) - 1]=bar`\ \ :ansopt:`bam.baz.foo#role:main:foo`\ \ :ansopt:
+`bam.baz.foo#role:main:bar.baz[123].bam[len(x) - 1]`\ \ :ansopt:
+`bam.baz.foo#role:main:foo=`\ \ :ansopt:`bam.baz.foo#role:main:bar.baz[123].bam
+[len(x) - 1]=`\ \ :ansopt:`bam.baz.foo#role:main:foo=bar`\ \ :ansopt:
+`bam.baz.foo#role:main:bar.baz[123].bam[len(x) - 1]=bar`\ \ :ansopt:`foo`\ \ :
+ansopt:`bar.baz[123].bam[len(x) - 1]`\ \ :ansopt:`foo=`\ \ :ansopt:`bar.baz
+[123].bam[len(x) - 1]=`\ \ :ansopt:`foo=bar`\ \ :ansopt:`bar.baz[123].bam[len
+(x) - 1]=bar`\ ansible_doc_text: |- `foo' `bar.baz[123].bam[len(x) - 1]' `foo='
+`bar.baz[123].bam[len(x) - 1]=' `foo=bar' `bar.baz[123].bam[len(x) - 1]=bar'
+`foo' (of lookup plugin bam.baz.foo) `bar.baz[123].bam[len(x) - 1]' (of lookup
+plugin bam.baz.foo) `foo=' (of lookup plugin bam.baz.foo) `bar.baz[123].bam[len
+(x) - 1]=' (of lookup plugin bam.baz.foo) `foo=bar' (of lookup plugin
+bam.baz.foo) `bar.baz[123].bam[len(x) - 1]=bar' (of lookup plugin bam.baz.foo)
+`foo' (of role bam.baz.foo, main entrypoint) `bar.baz[123].bam[len(x) - 1]' (of
+role bam.baz.foo, main entrypoint) `foo=' (of role bam.baz.foo, main
+entrypoint) `bar.baz[123].bam[len(x) - 1]=' (of role bam.baz.foo, main
+entrypoint) `foo=bar' (of role bam.baz.foo, main entrypoint) `bar.baz[123].bam
+[len(x) - 1]=bar' (of role bam.baz.foo, main entrypoint) `foo' `bar.baz
+[123].bam[len(x) - 1]' `foo=' `bar.baz[123].bam[len(x) - 1]=' `foo=bar'
+`bar.baz[123].bam[len(x) - 1]=bar' rst_plain: |- \ :literal:`foo`\ \ :literal:
+`bar.baz[123].bam[len(x) - 1]`\ \ :literal:`foo=`\ \ :literal:`bar.baz[123].bam
+[len(x) - 1]=`\ \ :literal:`foo=bar`\ \ :literal:`bar.baz[123].bam[len(x) -
+1]=bar`\ \ :literal:`foo` (of lookup plugin :ref:`bam.baz.foo
 bam.baz.foo_lookup>`)\ \ :literal:`bar.baz[123].bam[len(x) - 1]` (of lookup
-plugin :ref:`bam.baz.foo
-bam.baz.foo_lookup>`)\ \ :literal:`foo=` (of lookup plugin :ref:`bam.baz.foo
-bam.baz.foo_lookup>`)\ \ :literal:`bar.baz[123].bam[len(x) - 1]=` (of lookup
-plugin :ref:`bam.baz.foo
-bam.baz.foo_lookup>`)\ \ :literal:`foo=bar` (of lookup plugin :ref:`bam.baz.foo
-bam.baz.foo_lookup>`)\ \ :literal:`bar.baz[123].bam[len(x) - 1]=bar` (of lookup
-plugin :ref:`bam.baz.foo
+plugin :ref:`bam.baz.foo bam.baz.foo_lookup>`)\ \ :literal:`foo=` (of lookup
+plugin :ref:`bam.baz.foo bam.baz.foo_lookup>`)\ \ :literal:`bar.baz[123].bam
+[len(x) - 1]=` (of lookup plugin :ref:`bam.baz.foo bam.baz.foo_lookup>`)\ \ :
+literal:`foo=bar` (of lookup plugin :ref:`bam.baz.foo bam.baz.foo_lookup>`)\ \
+:literal:`bar.baz[123].bam[len(x) - 1]=bar` (of lookup plugin :ref:`bam.baz.foo
 bam.baz.foo_lookup>`)\ \ :literal:`foo` (of role :ref:`bam.baz.foo
 bam.baz.foo_role>`, entrypoint main)\ \ :literal:`bar.baz[123].bam[len(x) - 1]`
-(of role :ref:`bam.baz.foo
-bam.baz.foo_role>`, entrypoint main)\ \ :literal:`foo=` (of role :ref:
-`bam.baz.foo
-bam.baz.foo_role>`, entrypoint main)\ \ :literal:`bar.baz[123].bam[len(x) -
-1]=` (of role :ref:`bam.baz.foo
+(of role :ref:`bam.baz.foo bam.baz.foo_role>`, entrypoint main)\ \ :literal:
+`foo=` (of role :ref:`bam.baz.foo bam.baz.foo_role>`, entrypoint main)\ \ :
+literal:`bar.baz[123].bam[len(x) - 1]=` (of role :ref:`bam.baz.foo
 bam.baz.foo_role>`, entrypoint main)\ \ :literal:`foo=bar` (of role :ref:
-`bam.baz.foo
-bam.baz.foo_role>`, entrypoint main)\ \ :literal:`bar.baz[123].bam[len(x) -
-1]=bar` (of role :ref:`bam.baz.foo
-bam.baz.foo_role>`, entrypoint main)\ \ :literal:`foo`\ \ :literal:`bar.baz
-[123].bam[len(x) - 1]`\ \ :literal:`foo=`\ \ :literal:`bar.baz[123].bam[len(x)
-- 1]=`\ \ :literal:`foo=bar`\ \ :literal:`bar.baz[123].bam[len(x) - 1]=bar`\
-option_name_current_plugin_w_links: source: - |- O(foo) O(bar.baz[123].bam[len
-(x\) - 1]) - |- O(foo=) O(bar.baz[123].bam[len(x\) - 1]=) - |- O(foo=bar) O
-(bar.baz[123].bam[len(x\) - 1]=bar) - |- O(bam.baz.foo#lookup:foo) O
-(bam.baz.foo#lookup:bar.baz[123].bam[len(x\) - 1]) - |- O(bam.baz.foo#lookup:
-foo=) O(bam.baz.foo#lookup:bar.baz[123].bam[len(x\) - 1]=) - |- O
-(bam.baz.foo#lookup:foo=bar) O(bam.baz.foo#lookup:bar.baz[123].bam[len(x\) -
-1]=bar) - |- O(bam.baz.foo#role:main:foo) O(bam.baz.foo#role:main:bar.baz
-[123].bam[len(x\) - 1]) - |- O(bam.baz.foo#role:main:foo=) O(bam.baz.foo#role:
-main:bar.baz[123].bam[len(x\) - 1]=) - |- O(bam.baz.foo#role:main:foo=bar) O
-(bam.baz.foo#role:main:bar.baz[123].bam[len(x\) - 1]=bar) - |- O(ignore:foo) O
-(ignore:bar.baz[123].bam[len(x\) - 1]) - |- O(ignore:foo=) O(ignore:bar.baz
-[123].bam[len(x\) - 1]=) - |- O(ignore:foo=bar) O(ignore:bar.baz[123].bam[len
-(x\) - 1]=bar) html: |-
+`bam.baz.foo bam.baz.foo_role>`, entrypoint main)\ \ :literal:`bar.baz[123].bam
+[len(x) - 1]=bar` (of role :ref:`bam.baz.foo bam.baz.foo_role>`, entrypoint
+main)\ \ :literal:`foo`\ \ :literal:`bar.baz[123].bam[len(x) - 1]`\ \ :literal:
+`foo=`\ \ :literal:`bar.baz[123].bam[len(x) - 1]=`\ \ :literal:`foo=bar`\ \ :
+literal:`bar.baz[123].bam[len(x) - 1]=bar`\ option_name_current_plugin_w_links:
+source: - |- O(foo) O(bar.baz[123].bam[len(x\) - 1]) - |- O(foo=) O(bar.baz
+[123].bam[len(x\) - 1]=) - |- O(foo=bar) O(bar.baz[123].bam[len(x\) - 1]=bar) -
+|- O(bam.baz.foo#lookup:foo) O(bam.baz.foo#lookup:bar.baz[123].bam[len(x\) -
+1]) - |- O(bam.baz.foo#lookup:foo=) O(bam.baz.foo#lookup:bar.baz[123].bam[len
+(x\) - 1]=) - |- O(bam.baz.foo#lookup:foo=bar) O(bam.baz.foo#lookup:bar.baz
+[123].bam[len(x\) - 1]=bar) - |- O(bam.baz.foo#role:main:foo) O
+(bam.baz.foo#role:main:bar.baz[123].bam[len(x\) - 1]) - |- O(bam.baz.foo#role:
+main:foo=) O(bam.baz.foo#role:main:bar.baz[123].bam[len(x\) - 1]=) - |- O
+(bam.baz.foo#role:main:foo=bar) O(bam.baz.foo#role:main:bar.baz[123].bam[len
+(x\) - 1]=bar) - |- O(ignore:foo) O(ignore:bar.baz[123].bam[len(x\) - 1]) - |-
+O(ignore:foo=) O(ignore:bar.baz[123].bam[len(x\) - 1]=) - |- O(ignore:foo=bar)
+O(ignore:bar.baz[123].bam[len(x\) - 1]=bar) html: |-
 foo bar.baz[123].bam[len(x)_-_1]
 foo= bar.baz[123].bam[len(x)_-_1]=
 foo=bar bar.baz[123].bam[len(x)_-_1]=bar
 foo bar.baz[123].bam[len(x)_-_1]
 foo= bar.baz[123].bam[len(x)_-_1]=
 foo=bar bar.baz[123].bam[len(x)_-_1]=bar
 foo bar.baz[123].bam[len(x)_-_1]
@@ -607,45 +589,45 @@
 foo=bar bar.baz[123].bam[len(x)_-_1]=bar
 foo bar.baz[123].bam[len(x)_-_1]
 foo= bar.baz[123].bam[len(x)_-_1]=
 foo=bar bar.baz[123].bam[len(x)_-_1]=bar
 foo bar.baz[123].bam[len(x) - 1]
 foo= bar.baz[123].bam[len(x) - 1]=
 foo=bar bar.baz[123].bam[len(x) - 1]=bar
-md: |- foo bar.baz\[123\].bam\[len\(x\)_\-_1\] foo\= bar.baz\[123\].bam\[len\
-(x\)_\-_1\]\= foo\=bar bar.baz\[123\].bam\[len\(x\)_\-_1\]\=bar foo bar.baz\
-[123\].bam\[len\(x\)_\-_1\] foo\= bar.baz\[123\].bam\[len\(x\)_\-_1\]\=
-foo\=bar bar.baz\[123\].bam\[len\(x\)_\-_1\]\=bar foo bar.baz\[123\].bam\[len\
-(x\)_\-_1\] foo\= bar.baz\[123\].bam\[len\(x\)_\-_1\]\= foo\=bar bar.baz\
-[123\].bam\[len\(x\)_\-_1\]\=bar foo bar.baz\[123\].bam\[len\(x\) \- 1\] foo\=
-bar.baz\[123\].bam\[len\(x\) \- 1\]\= foo\=bar bar.baz\[123\].bam\[len\(x\) \-
-1\]\=bar md_opts: pluginOptionLikeLink.js: |- (plugin, entrypoint, what, name,
-current_plugin) => `https://docs.ansible.com/ansible/devel/collections/$
-{plugin.fqcn.replace(/\./g, '/')}_${plugin.type}.html#${what}${entrypoint ? '-
-' + entrypoint : ''}-${name.join('/')}` pluginOptionLikeLink.py: |- lambda
-plugin, entrypoint, what, name, current_plugin: f"https://docs.ansible.com/
-ansible/devel/collections/{plugin.fqcn.replace('.', '/')}_{plugin.type}.html#
-{what}{'-' + entrypoint if entrypoint else ''}-{'/'.join(name)}" rst: |- \ :
-ansopt:`foo.bar.baz.bam#boo:foo`\ \ :ansopt:`foo.bar.baz.bam#boo:bar.baz
-[123].bam[len(x) - 1]`\ \ :ansopt:`foo.bar.baz.bam#boo:foo=`\ \ :ansopt:
-`foo.bar.baz.bam#boo:bar.baz[123].bam[len(x) - 1]=`\ \ :ansopt:
-`foo.bar.baz.bam#boo:foo=bar`\ \ :ansopt:`foo.bar.baz.bam#boo:bar.baz[123].bam
-[len(x) - 1]=bar`\ \ :ansopt:`bam.baz.foo#lookup:foo`\ \ :ansopt:
-`bam.baz.foo#lookup:bar.baz[123].bam[len(x) - 1]`\ \ :ansopt:
-`bam.baz.foo#lookup:foo=`\ \ :ansopt:`bam.baz.foo#lookup:bar.baz[123].bam[len
-(x) - 1]=`\ \ :ansopt:`bam.baz.foo#lookup:foo=bar`\ \ :ansopt:
-`bam.baz.foo#lookup:bar.baz[123].bam[len(x) - 1]=bar`\ \ :ansopt:
+md: |- foo bar\.baz\[123\]\.bam\[len\(x\)_\-_1\] foo\= bar\.baz\[123\]\.bam\
+[len\(x\)_\-_1\]\= foo\=bar bar\.baz\[123\]\.bam\[len\(x\)_\-_1\]\=bar foo
+bar\.baz\[123\]\.bam\[len\(x\)_\-_1\] foo\= bar\.baz\[123\]\.bam\[len\(x\)_\-
+1\]\= foo\=bar bar\.baz\[123\]\.bam\[len\(x\)_\-_1\]\=bar foo bar\.baz\
+[123\]\.bam\[len\(x\)_\-_1\] foo\= bar\.baz\[123\]\.bam\[len\(x\)_\-_1\]\=
+foo\=bar bar\.baz\[123\]\.bam\[len\(x\)_\-_1\]\=bar foo bar\.baz\[123\]\.bam\
+[len\(x\) \- 1\] foo\= bar\.baz\[123\]\.bam\[len\(x\) \- 1\]\= foo\=bar
+bar\.baz\[123\]\.bam\[len\(x\) \- 1\]\=bar md_opts: pluginOptionLikeLink.js: |-
+(plugin, entrypoint, what, name, current_plugin) => `https://docs.ansible.com/
+ansible/devel/collections/${plugin.fqcn.replace(/\./g, '/')}_$
+{plugin.type}.html#${what}${entrypoint ? '-' + entrypoint : ''}-${name.join('/
+')}` pluginOptionLikeLink.py: |- lambda plugin, entrypoint, what, name,
+current_plugin: f"https://docs.ansible.com/ansible/devel/collections/
+{plugin.fqcn.replace('.', '/')}_{plugin.type}.html#{what}{'-' + entrypoint if
+entrypoint else ''}-{'/'.join(name)}" rst: |- \ :ansopt:`foo.bar.baz.bam#boo:
+foo`\ \ :ansopt:`foo.bar.baz.bam#boo:bar.baz[123].bam[len(x) - 1]`\ \ :ansopt:
+`foo.bar.baz.bam#boo:foo=`\ \ :ansopt:`foo.bar.baz.bam#boo:bar.baz[123].bam[len
+(x) - 1]=`\ \ :ansopt:`foo.bar.baz.bam#boo:foo=bar`\ \ :ansopt:
+`foo.bar.baz.bam#boo:bar.baz[123].bam[len(x) - 1]=bar`\ \ :ansopt:
+`bam.baz.foo#lookup:foo`\ \ :ansopt:`bam.baz.foo#lookup:bar.baz[123].bam[len(x)
+- 1]`\ \ :ansopt:`bam.baz.foo#lookup:foo=`\ \ :ansopt:`bam.baz.foo#lookup:
+bar.baz[123].bam[len(x) - 1]=`\ \ :ansopt:`bam.baz.foo#lookup:foo=bar`\ \ :
+ansopt:`bam.baz.foo#lookup:bar.baz[123].bam[len(x) - 1]=bar`\ \ :ansopt:
 `bam.baz.foo#role:main:foo`\ \ :ansopt:`bam.baz.foo#role:main:bar.baz[123].bam
 [len(x) - 1]`\ \ :ansopt:`bam.baz.foo#role:main:foo=`\ \ :ansopt:
 `bam.baz.foo#role:main:bar.baz[123].bam[len(x) - 1]=`\ \ :ansopt:
 `bam.baz.foo#role:main:foo=bar`\ \ :ansopt:`bam.baz.foo#role:main:bar.baz
 [123].bam[len(x) - 1]=bar`\ \ :ansopt:`foo`\ \ :ansopt:`bar.baz[123].bam[len(x)
 - 1]`\ \ :ansopt:`foo=`\ \ :ansopt:`bar.baz[123].bam[len(x) - 1]=`\ \ :ansopt:
 `foo=bar`\ \ :ansopt:`bar.baz[123].bam[len(x) - 1]=bar`\ parse_opts:
-current_plugin: fqcn: foo.bar.baz.bam type: boo ansible_doc_text: |- `foo' (of
+currentPlugin: fqcn: foo.bar.baz.bam type: boo ansible_doc_text: |- `foo' (of
 boo plugin foo.bar.baz.bam) `bar.baz[123].bam[len(x) - 1]' (of boo plugin
 foo.bar.baz.bam) `foo=' (of boo plugin foo.bar.baz.bam) `bar.baz[123].bam[len
 (x) - 1]=' (of boo plugin foo.bar.baz.bam) `foo=bar' (of boo plugin
 foo.bar.baz.bam) `bar.baz[123].bam[len(x) - 1]=bar' (of boo plugin
 foo.bar.baz.bam) `foo' (of lookup plugin bam.baz.foo) `bar.baz[123].bam[len(x)
 - 1]' (of lookup plugin bam.baz.foo) `foo=' (of lookup plugin bam.baz.foo)
 `bar.baz[123].bam[len(x) - 1]=' (of lookup plugin bam.baz.foo) `foo=bar' (of
@@ -653,63 +635,54 @@
 bam.baz.foo) `foo' (of role bam.baz.foo, main entrypoint) `bar.baz[123].bam[len
 (x) - 1]' (of role bam.baz.foo, main entrypoint) `foo=' (of role bam.baz.foo,
 main entrypoint) `bar.baz[123].bam[len(x) - 1]=' (of role bam.baz.foo, main
 entrypoint) `foo=bar' (of role bam.baz.foo, main entrypoint) `bar.baz[123].bam
 [len(x) - 1]=bar' (of role bam.baz.foo, main entrypoint) `foo' `bar.baz
 [123].bam[len(x) - 1]' `foo=' `bar.baz[123].bam[len(x) - 1]=' `foo=bar'
 `bar.baz[123].bam[len(x) - 1]=bar' rst_plain: |- \ :literal:`foo` (of boo
-plugin :ref:`foo.bar.baz.bam
-foo.bar.baz.bam_boo>`)\ \ :literal:`bar.baz[123].bam[len(x) - 1]` (of boo
-plugin :ref:`foo.bar.baz.bam
+plugin :ref:`foo.bar.baz.bam foo.bar.baz.bam_boo>`)\ \ :literal:`bar.baz
+[123].bam[len(x) - 1]` (of boo plugin :ref:`foo.bar.baz.bam
 foo.bar.baz.bam_boo>`)\ \ :literal:`foo=` (of boo plugin :ref:`foo.bar.baz.bam
 foo.bar.baz.bam_boo>`)\ \ :literal:`bar.baz[123].bam[len(x) - 1]=` (of boo
-plugin :ref:`foo.bar.baz.bam
-foo.bar.baz.bam_boo>`)\ \ :literal:`foo=bar` (of boo plugin :ref:
-`foo.bar.baz.bam
-foo.bar.baz.bam_boo>`)\ \ :literal:`bar.baz[123].bam[len(x) - 1]=bar` (of boo
-plugin :ref:`foo.bar.baz.bam
+plugin :ref:`foo.bar.baz.bam foo.bar.baz.bam_boo>`)\ \ :literal:`foo=bar` (of
+boo plugin :ref:`foo.bar.baz.bam foo.bar.baz.bam_boo>`)\ \ :literal:`bar.baz
+[123].bam[len(x) - 1]=bar` (of boo plugin :ref:`foo.bar.baz.bam
 foo.bar.baz.bam_boo>`)\ \ :literal:`foo` (of lookup plugin :ref:`bam.baz.foo
 bam.baz.foo_lookup>`)\ \ :literal:`bar.baz[123].bam[len(x) - 1]` (of lookup
-plugin :ref:`bam.baz.foo
-bam.baz.foo_lookup>`)\ \ :literal:`foo=` (of lookup plugin :ref:`bam.baz.foo
-bam.baz.foo_lookup>`)\ \ :literal:`bar.baz[123].bam[len(x) - 1]=` (of lookup
-plugin :ref:`bam.baz.foo
-bam.baz.foo_lookup>`)\ \ :literal:`foo=bar` (of lookup plugin :ref:`bam.baz.foo
-bam.baz.foo_lookup>`)\ \ :literal:`bar.baz[123].bam[len(x) - 1]=bar` (of lookup
-plugin :ref:`bam.baz.foo
+plugin :ref:`bam.baz.foo bam.baz.foo_lookup>`)\ \ :literal:`foo=` (of lookup
+plugin :ref:`bam.baz.foo bam.baz.foo_lookup>`)\ \ :literal:`bar.baz[123].bam
+[len(x) - 1]=` (of lookup plugin :ref:`bam.baz.foo bam.baz.foo_lookup>`)\ \ :
+literal:`foo=bar` (of lookup plugin :ref:`bam.baz.foo bam.baz.foo_lookup>`)\ \
+:literal:`bar.baz[123].bam[len(x) - 1]=bar` (of lookup plugin :ref:`bam.baz.foo
 bam.baz.foo_lookup>`)\ \ :literal:`foo` (of role :ref:`bam.baz.foo
 bam.baz.foo_role>`, entrypoint main)\ \ :literal:`bar.baz[123].bam[len(x) - 1]`
-(of role :ref:`bam.baz.foo
-bam.baz.foo_role>`, entrypoint main)\ \ :literal:`foo=` (of role :ref:
-`bam.baz.foo
-bam.baz.foo_role>`, entrypoint main)\ \ :literal:`bar.baz[123].bam[len(x) -
-1]=` (of role :ref:`bam.baz.foo
+(of role :ref:`bam.baz.foo bam.baz.foo_role>`, entrypoint main)\ \ :literal:
+`foo=` (of role :ref:`bam.baz.foo bam.baz.foo_role>`, entrypoint main)\ \ :
+literal:`bar.baz[123].bam[len(x) - 1]=` (of role :ref:`bam.baz.foo
 bam.baz.foo_role>`, entrypoint main)\ \ :literal:`foo=bar` (of role :ref:
-`bam.baz.foo
-bam.baz.foo_role>`, entrypoint main)\ \ :literal:`bar.baz[123].bam[len(x) -
-1]=bar` (of role :ref:`bam.baz.foo
-bam.baz.foo_role>`, entrypoint main)\ \ :literal:`foo`\ \ :literal:`bar.baz
-[123].bam[len(x) - 1]`\ \ :literal:`foo=`\ \ :literal:`bar.baz[123].bam[len(x)
-- 1]=`\ \ :literal:`foo=bar`\ \ :literal:`bar.baz[123].bam[len(x) - 1]=bar`\
-option_name_current_role_w_links: source: - |- O(foo) O(bar.baz[123].bam[len
-(x\) - 1]) - |- O(foo=) O(bar.baz[123].bam[len(x\) - 1]=) - |- O(foo=bar) O
-(bar.baz[123].bam[len(x\) - 1]=bar) - |- O(other_entrypoint:foo) O
-(other_entrypoint:bar.baz[123].bam[len(x\) - 1]) - |- O(other_entrypoint:foo=)
-O(other_entrypoint:bar.baz[123].bam[len(x\) - 1]=) - |- O(other_entrypoint:
-foo=bar) O(other_entrypoint:bar.baz[123].bam[len(x\) - 1]=bar) - |- O
-(bam.baz.foo#lookup:foo) O(bam.baz.foo#lookup:bar.baz[123].bam[len(x\) - 1]) -
-|- O(bam.baz.foo#lookup:foo=) O(bam.baz.foo#lookup:bar.baz[123].bam[len(x\) -
-1]=) - |- O(bam.baz.foo#lookup:foo=bar) O(bam.baz.foo#lookup:bar.baz[123].bam
-[len(x\) - 1]=bar) - |- O(bam.baz.foo#role:main:foo) O(bam.baz.foo#role:main:
-bar.baz[123].bam[len(x\) - 1]) - |- O(bam.baz.foo#role:main:foo=) O
-(bam.baz.foo#role:main:bar.baz[123].bam[len(x\) - 1]=) - |- O(bam.baz.foo#role:
-main:foo=bar) O(bam.baz.foo#role:main:bar.baz[123].bam[len(x\) - 1]=bar) - |- O
-(ignore:foo) O(ignore:bar.baz[123].bam[len(x\) - 1]) - |- O(ignore:foo=) O
-(ignore:bar.baz[123].bam[len(x\) - 1]=) - |- O(ignore:foo=bar) O(ignore:bar.baz
-[123].bam[len(x\) - 1]=bar) html: |-
+`bam.baz.foo bam.baz.foo_role>`, entrypoint main)\ \ :literal:`bar.baz[123].bam
+[len(x) - 1]=bar` (of role :ref:`bam.baz.foo bam.baz.foo_role>`, entrypoint
+main)\ \ :literal:`foo`\ \ :literal:`bar.baz[123].bam[len(x) - 1]`\ \ :literal:
+`foo=`\ \ :literal:`bar.baz[123].bam[len(x) - 1]=`\ \ :literal:`foo=bar`\ \ :
+literal:`bar.baz[123].bam[len(x) - 1]=bar`\ option_name_current_role_w_links:
+source: - |- O(foo) O(bar.baz[123].bam[len(x\) - 1]) - |- O(foo=) O(bar.baz
+[123].bam[len(x\) - 1]=) - |- O(foo=bar) O(bar.baz[123].bam[len(x\) - 1]=bar) -
+|- O(other_entrypoint:foo) O(other_entrypoint:bar.baz[123].bam[len(x\) - 1]) -
+|- O(other_entrypoint:foo=) O(other_entrypoint:bar.baz[123].bam[len(x\) - 1]=)
+- |- O(other_entrypoint:foo=bar) O(other_entrypoint:bar.baz[123].bam[len(x\) -
+1]=bar) - |- O(bam.baz.foo#lookup:foo) O(bam.baz.foo#lookup:bar.baz[123].bam
+[len(x\) - 1]) - |- O(bam.baz.foo#lookup:foo=) O(bam.baz.foo#lookup:bar.baz
+[123].bam[len(x\) - 1]=) - |- O(bam.baz.foo#lookup:foo=bar) O
+(bam.baz.foo#lookup:bar.baz[123].bam[len(x\) - 1]=bar) - |- O(bam.baz.foo#role:
+main:foo) O(bam.baz.foo#role:main:bar.baz[123].bam[len(x\) - 1]) - |- O
+(bam.baz.foo#role:main:foo=) O(bam.baz.foo#role:main:bar.baz[123].bam[len(x\) -
+1]=) - |- O(bam.baz.foo#role:main:foo=bar) O(bam.baz.foo#role:main:bar.baz
+[123].bam[len(x\) - 1]=bar) - |- O(ignore:foo) O(ignore:bar.baz[123].bam[len
+(x\) - 1]) - |- O(ignore:foo=) O(ignore:bar.baz[123].bam[len(x\) - 1]=) - |- O
+(ignore:foo=bar) O(ignore:bar.baz[123].bam[len(x\) - 1]=bar) html: |-
 foo bar.baz[123].bam[len(x)_-_1]
 foo= bar.baz[123].bam[len(x)_-_1]=
 foo=bar bar.baz[123].bam[len(x)_-_1]=bar
 foo bar.baz[123].bam[len(x)_-_1]
 foo= bar.baz[123].bam[len(x)_-_1]=
 foo=bar bar.baz[123].bam[len(x)_-_1]=bar
 foo bar.baz[123].bam[len(x)_-_1]
@@ -739,28 +712,29 @@
 foo=bar bar.baz[123].bam[len(x)_-_1]=bar
 foo bar.baz[123].bam[len(x)_-_1]
 foo= bar.baz[123].bam[len(x)_-_1]=
 foo=bar bar.baz[123].bam[len(x)_-_1]=bar
 foo bar.baz[123].bam[len(x) - 1]
 foo= bar.baz[123].bam[len(x) - 1]=
 foo=bar bar.baz[123].bam[len(x) - 1]=bar
-md: |- foo bar.baz\[123\].bam\[len\(x\)_\-_1\] foo\= bar.baz\[123\].bam\[len\
-(x\)_\-_1\]\= foo\=bar bar.baz\[123\].bam\[len\(x\)_\-_1\]\=bar foo bar.baz\
-[123\].bam\[len\(x\)_\-_1\] foo\= bar.baz\[123\].bam\[len\(x\)_\-_1\]\=
-foo\=bar bar.baz\[123\].bam\[len\(x\)_\-_1\]\=bar foo bar.baz\[123\].bam\[len\
-(x\)_\-_1\] foo\= bar.baz\[123\].bam\[len\(x\)_\-_1\]\= foo\=bar bar.baz\
-[123\].bam\[len\(x\)_\-_1\]\=bar foo bar.baz\[123\].bam\[len\(x\)_\-_1\] foo\=
-bar.baz\[123\].bam\[len\(x\)_\-_1\]\= foo\=bar bar.baz\[123\].bam\[len\(x\)_\-
-1\]\=bar foo bar.baz\[123\].bam\[len\(x\) \- 1\] foo\= bar.baz\[123\].bam\[len\
-(x\) \- 1\]\= foo\=bar bar.baz\[123\].bam\[len\(x\) \- 1\]\=bar md_opts:
-pluginOptionLikeLink.js: |- (plugin, entrypoint, what, name, current_plugin) =>
-`https://docs.ansible.com/ansible/devel/collections/${plugin.fqcn.replace(/\./
-g, '/')}_${plugin.type}.html#${what}${entrypoint ? '-' + entrypoint : ''}-$
-{name.join('/')}` pluginOptionLikeLink.py: |- lambda plugin, entrypoint, what,
-name, current_plugin: f"https://docs.ansible.com/ansible/devel/collections/
+md: |- foo bar\.baz\[123\]\.bam\[len\(x\)_\-_1\] foo\= bar\.baz\[123\]\.bam\
+[len\(x\)_\-_1\]\= foo\=bar bar\.baz\[123\]\.bam\[len\(x\)_\-_1\]\=bar foo
+bar\.baz\[123\]\.bam\[len\(x\)_\-_1\] foo\= bar\.baz\[123\]\.bam\[len\(x\)_\-
+1\]\= foo\=bar bar\.baz\[123\]\.bam\[len\(x\)_\-_1\]\=bar foo bar\.baz\
+[123\]\.bam\[len\(x\)_\-_1\] foo\= bar\.baz\[123\]\.bam\[len\(x\)_\-_1\]\=
+foo\=bar bar\.baz\[123\]\.bam\[len\(x\)_\-_1\]\=bar foo bar\.baz\[123\]\.bam\
+[len\(x\)_\-_1\] foo\= bar\.baz\[123\]\.bam\[len\(x\)_\-_1\]\= foo\=bar
+bar\.baz\[123\]\.bam\[len\(x\)_\-_1\]\=bar foo bar\.baz\[123\]\.bam\[len\(x\)
+\- 1\] foo\= bar\.baz\[123\]\.bam\[len\(x\) \- 1\]\= foo\=bar bar\.baz\
+[123\]\.bam\[len\(x\) \- 1\]\=bar md_opts: pluginOptionLikeLink.js: |- (plugin,
+entrypoint, what, name, current_plugin) => `https://docs.ansible.com/ansible/
+devel/collections/${plugin.fqcn.replace(/\./g, '/')}_${plugin.type}.html#$
+{what}${entrypoint ? '-' + entrypoint : ''}-${name.join('/')}`
+pluginOptionLikeLink.py: |- lambda plugin, entrypoint, what, name,
+current_plugin: f"https://docs.ansible.com/ansible/devel/collections/
 {plugin.fqcn.replace('.', '/')}_{plugin.type}.html#{what}{'-' + entrypoint if
 entrypoint else ''}-{'/'.join(name)}" rst: |- \ :ansopt:`foo.bar.baz#role:main:
 foo`\ \ :ansopt:`foo.bar.baz#role:main:bar.baz[123].bam[len(x) - 1]`\ \ :
 ansopt:`foo.bar.baz#role:main:foo=`\ \ :ansopt:`foo.bar.baz#role:main:bar.baz
 [123].bam[len(x) - 1]=`\ \ :ansopt:`foo.bar.baz#role:main:foo=bar`\ \ :ansopt:
 `foo.bar.baz#role:main:bar.baz[123].bam[len(x) - 1]=bar`\ \ :ansopt:
 `foo.bar.baz#role:other\_entrypoint:foo`\ \ :ansopt:`foo.bar.baz#role:
@@ -775,16 +749,16 @@
 [len(x) - 1]=bar`\ \ :ansopt:`bam.baz.foo#role:main:foo`\ \ :ansopt:
 `bam.baz.foo#role:main:bar.baz[123].bam[len(x) - 1]`\ \ :ansopt:
 `bam.baz.foo#role:main:foo=`\ \ :ansopt:`bam.baz.foo#role:main:bar.baz[123].bam
 [len(x) - 1]=`\ \ :ansopt:`bam.baz.foo#role:main:foo=bar`\ \ :ansopt:
 `bam.baz.foo#role:main:bar.baz[123].bam[len(x) - 1]=bar`\ \ :ansopt:`foo`\ \ :
 ansopt:`bar.baz[123].bam[len(x) - 1]`\ \ :ansopt:`foo=`\ \ :ansopt:`bar.baz
 [123].bam[len(x) - 1]=`\ \ :ansopt:`foo=bar`\ \ :ansopt:`bar.baz[123].bam[len
-(x) - 1]=bar`\ parse_opts: current_plugin: fqcn: foo.bar.baz type: role
-role_entrypoint: main ansible_doc_text: |- `foo' (of role foo.bar.baz, main
+(x) - 1]=bar`\ parse_opts: currentPlugin: fqcn: foo.bar.baz type: role
+roleEntrypoint: main ansible_doc_text: |- `foo' (of role foo.bar.baz, main
 entrypoint) `bar.baz[123].bam[len(x) - 1]' (of role foo.bar.baz, main
 entrypoint) `foo=' (of role foo.bar.baz, main entrypoint) `bar.baz[123].bam[len
 (x) - 1]=' (of role foo.bar.baz, main entrypoint) `foo=bar' (of role
 foo.bar.baz, main entrypoint) `bar.baz[123].bam[len(x) - 1]=bar' (of role
 foo.bar.baz, main entrypoint) `foo' (of role foo.bar.baz, other_entrypoint
 entrypoint) `bar.baz[123].bam[len(x) - 1]' (of role foo.bar.baz,
 other_entrypoint entrypoint) `foo=' (of role foo.bar.baz, other_entrypoint
@@ -798,70 +772,57 @@
 lookup plugin bam.baz.foo) `foo' (of role bam.baz.foo, main entrypoint)
 `bar.baz[123].bam[len(x) - 1]' (of role bam.baz.foo, main entrypoint) `foo='
 (of role bam.baz.foo, main entrypoint) `bar.baz[123].bam[len(x) - 1]=' (of role
 bam.baz.foo, main entrypoint) `foo=bar' (of role bam.baz.foo, main entrypoint)
 `bar.baz[123].bam[len(x) - 1]=bar' (of role bam.baz.foo, main entrypoint) `foo'
 `bar.baz[123].bam[len(x) - 1]' `foo=' `bar.baz[123].bam[len(x) - 1]=' `foo=bar'
 `bar.baz[123].bam[len(x) - 1]=bar' rst_plain: |- \ :literal:`foo` (of role :
-ref:`foo.bar.baz
-foo.bar.baz_role>`, entrypoint main)\ \ :literal:`bar.baz[123].bam[len(x) - 1]`
-(of role :ref:`foo.bar.baz
-foo.bar.baz_role>`, entrypoint main)\ \ :literal:`foo=` (of role :ref:
-`foo.bar.baz
+ref:`foo.bar.baz foo.bar.baz_role>`, entrypoint main)\ \ :literal:`bar.baz
+[123].bam[len(x) - 1]` (of role :ref:`foo.bar.baz foo.bar.baz_role>`,
+entrypoint main)\ \ :literal:`foo=` (of role :ref:`foo.bar.baz
 foo.bar.baz_role>`, entrypoint main)\ \ :literal:`bar.baz[123].bam[len(x) -
-1]=` (of role :ref:`foo.bar.baz
-foo.bar.baz_role>`, entrypoint main)\ \ :literal:`foo=bar` (of role :ref:
-`foo.bar.baz
-foo.bar.baz_role>`, entrypoint main)\ \ :literal:`bar.baz[123].bam[len(x) -
-1]=bar` (of role :ref:`foo.bar.baz
+1]=` (of role :ref:`foo.bar.baz foo.bar.baz_role>`, entrypoint main)\ \ :
+literal:`foo=bar` (of role :ref:`foo.bar.baz foo.bar.baz_role>`, entrypoint
+main)\ \ :literal:`bar.baz[123].bam[len(x) - 1]=bar` (of role :ref:`foo.bar.baz
 foo.bar.baz_role>`, entrypoint main)\ \ :literal:`foo` (of role :ref:
-`foo.bar.baz
-foo.bar.baz_role>`, entrypoint other\_entrypoint)\ \ :literal:`bar.baz[123].bam
-[len(x) - 1]` (of role :ref:`foo.bar.baz
-foo.bar.baz_role>`, entrypoint other\_entrypoint)\ \ :literal:`foo=` (of role :
-ref:`foo.bar.baz
+`foo.bar.baz foo.bar.baz_role>`, entrypoint other\_entrypoint)\ \ :literal:
+`bar.baz[123].bam[len(x) - 1]` (of role :ref:`foo.bar.baz foo.bar.baz_role>`,
+entrypoint other\_entrypoint)\ \ :literal:`foo=` (of role :ref:`foo.bar.baz
 foo.bar.baz_role>`, entrypoint other\_entrypoint)\ \ :literal:`bar.baz[123].bam
-[len(x) - 1]=` (of role :ref:`foo.bar.baz
-foo.bar.baz_role>`, entrypoint other\_entrypoint)\ \ :literal:`foo=bar` (of
-role :ref:`foo.bar.baz
+[len(x) - 1]=` (of role :ref:`foo.bar.baz foo.bar.baz_role>`, entrypoint
+other\_entrypoint)\ \ :literal:`foo=bar` (of role :ref:`foo.bar.baz
 foo.bar.baz_role>`, entrypoint other\_entrypoint)\ \ :literal:`bar.baz[123].bam
-[len(x) - 1]=bar` (of role :ref:`foo.bar.baz
-foo.bar.baz_role>`, entrypoint other\_entrypoint)\ \ :literal:`foo` (of lookup
-plugin :ref:`bam.baz.foo
+[len(x) - 1]=bar` (of role :ref:`foo.bar.baz foo.bar.baz_role>`, entrypoint
+other\_entrypoint)\ \ :literal:`foo` (of lookup plugin :ref:`bam.baz.foo
 bam.baz.foo_lookup>`)\ \ :literal:`bar.baz[123].bam[len(x) - 1]` (of lookup
-plugin :ref:`bam.baz.foo
-bam.baz.foo_lookup>`)\ \ :literal:`foo=` (of lookup plugin :ref:`bam.baz.foo
-bam.baz.foo_lookup>`)\ \ :literal:`bar.baz[123].bam[len(x) - 1]=` (of lookup
-plugin :ref:`bam.baz.foo
-bam.baz.foo_lookup>`)\ \ :literal:`foo=bar` (of lookup plugin :ref:`bam.baz.foo
-bam.baz.foo_lookup>`)\ \ :literal:`bar.baz[123].bam[len(x) - 1]=bar` (of lookup
-plugin :ref:`bam.baz.foo
+plugin :ref:`bam.baz.foo bam.baz.foo_lookup>`)\ \ :literal:`foo=` (of lookup
+plugin :ref:`bam.baz.foo bam.baz.foo_lookup>`)\ \ :literal:`bar.baz[123].bam
+[len(x) - 1]=` (of lookup plugin :ref:`bam.baz.foo bam.baz.foo_lookup>`)\ \ :
+literal:`foo=bar` (of lookup plugin :ref:`bam.baz.foo bam.baz.foo_lookup>`)\ \
+:literal:`bar.baz[123].bam[len(x) - 1]=bar` (of lookup plugin :ref:`bam.baz.foo
 bam.baz.foo_lookup>`)\ \ :literal:`foo` (of role :ref:`bam.baz.foo
 bam.baz.foo_role>`, entrypoint main)\ \ :literal:`bar.baz[123].bam[len(x) - 1]`
-(of role :ref:`bam.baz.foo
-bam.baz.foo_role>`, entrypoint main)\ \ :literal:`foo=` (of role :ref:
-`bam.baz.foo
-bam.baz.foo_role>`, entrypoint main)\ \ :literal:`bar.baz[123].bam[len(x) -
-1]=` (of role :ref:`bam.baz.foo
+(of role :ref:`bam.baz.foo bam.baz.foo_role>`, entrypoint main)\ \ :literal:
+`foo=` (of role :ref:`bam.baz.foo bam.baz.foo_role>`, entrypoint main)\ \ :
+literal:`bar.baz[123].bam[len(x) - 1]=` (of role :ref:`bam.baz.foo
 bam.baz.foo_role>`, entrypoint main)\ \ :literal:`foo=bar` (of role :ref:
-`bam.baz.foo
-bam.baz.foo_role>`, entrypoint main)\ \ :literal:`bar.baz[123].bam[len(x) -
-1]=bar` (of role :ref:`bam.baz.foo
-bam.baz.foo_role>`, entrypoint main)\ \ :literal:`foo`\ \ :literal:`bar.baz
-[123].bam[len(x) - 1]`\ \ :literal:`foo=`\ \ :literal:`bar.baz[123].bam[len(x)
-- 1]=`\ \ :literal:`foo=bar`\ \ :literal:`bar.baz[123].bam[len(x) - 1]=bar`\
-return_value_no_current_plugin: source: - |- RV(foo) RV(bar.baz[123].bam[len
-(x\) - 1]) - |- RV(foo=) RV(bar.baz[123].bam[len(x\) - 1]=) - |- RV(foo=bar) RV
-(bar.baz[123].bam[len(x\) - 1]=bar) - |- RV(bam.baz.foo#lookup:foo) RV
-(bam.baz.foo#lookup:bar.baz[123].bam[len(x\) - 1]) - |- RV(bam.baz.foo#lookup:
-foo=) RV(bam.baz.foo#lookup:bar.baz[123].bam[len(x\) - 1]=) - |- RV
-(bam.baz.foo#lookup:foo=bar) RV(bam.baz.foo#lookup:bar.baz[123].bam[len(x\) -
-1]=bar) - |- RV(ignore:foo) RV(ignore:bar.baz[123].bam[len(x\) - 1]) - |- RV
-(ignore:foo=) RV(ignore:bar.baz[123].bam[len(x\) - 1]=) - |- RV(ignore:foo=bar)
-RV(ignore:bar.baz[123].bam[len(x\) - 1]=bar) html: |-
+`bam.baz.foo bam.baz.foo_role>`, entrypoint main)\ \ :literal:`bar.baz[123].bam
+[len(x) - 1]=bar` (of role :ref:`bam.baz.foo bam.baz.foo_role>`, entrypoint
+main)\ \ :literal:`foo`\ \ :literal:`bar.baz[123].bam[len(x) - 1]`\ \ :literal:
+`foo=`\ \ :literal:`bar.baz[123].bam[len(x) - 1]=`\ \ :literal:`foo=bar`\ \ :
+literal:`bar.baz[123].bam[len(x) - 1]=bar`\ return_value_no_current_plugin:
+source: - |- RV(foo) RV(bar.baz[123].bam[len(x\) - 1]) - |- RV(foo=) RV(bar.baz
+[123].bam[len(x\) - 1]=) - |- RV(foo=bar) RV(bar.baz[123].bam[len(x\) - 1]=bar)
+- |- RV(bam.baz.foo#lookup:foo) RV(bam.baz.foo#lookup:bar.baz[123].bam[len(x\)
+- 1]) - |- RV(bam.baz.foo#lookup:foo=) RV(bam.baz.foo#lookup:bar.baz[123].bam
+[len(x\) - 1]=) - |- RV(bam.baz.foo#lookup:foo=bar) RV(bam.baz.foo#lookup:
+bar.baz[123].bam[len(x\) - 1]=bar) - |- RV(ignore:foo) RV(ignore:bar.baz
+[123].bam[len(x\) - 1]) - |- RV(ignore:foo=) RV(ignore:bar.baz[123].bam[len(x\)
+- 1]=) - |- RV(ignore:foo=bar) RV(ignore:bar.baz[123].bam[len(x\) - 1]=bar)
+html: |-
 foo bar.baz[123].bam[len(x) - 1]
 foo= bar.baz[123].bam[len(x) - 1]=
 foo=bar bar.baz[123].bam[len(x) - 1]=bar
 foo bar.baz[123].bam[len(x) - 1]
 foo= bar.baz[123].bam[len(x) - 1]=
 foo=bar bar.baz[123].bam[len(x) - 1]=bar
 foo bar.baz[123].bam[len(x) - 1]
@@ -873,24 +834,24 @@
 foo=bar bar.baz[123].bam[len(x) - 1]=bar
 foo bar.baz[123].bam[len(x) - 1]
 foo= bar.baz[123].bam[len(x) - 1]=
 foo=bar bar.baz[123].bam[len(x) - 1]=bar
 foo bar.baz[123].bam[len(x) - 1]
 foo= bar.baz[123].bam[len(x) - 1]=
 foo=bar bar.baz[123].bam[len(x) - 1]=bar
-md: |- foo bar.baz\[123\].bam\[len\(x\) \- 1\] foo\= bar.baz\[123\].bam\[len\
-(x\) \- 1\]\= foo\=bar bar.baz\[123\].bam\[len\(x\) \- 1\]\=bar foo bar.baz\
-[123\].bam\[len\(x\) \- 1\] foo\= bar.baz\[123\].bam\[len\(x\) \- 1\]\=
-foo\=bar bar.baz\[123\].bam\[len\(x\) \- 1\]\=bar foo bar.baz\[123\].bam\[len\
-(x\) \- 1\] foo\= bar.baz\[123\].bam\[len\(x\) \- 1\]\= foo\=bar bar.baz\
-[123\].bam\[len\(x\) \- 1\]\=bar rst: |- \ :ansretval:`foo`\ \ :ansretval:
-`bar.baz[123].bam[len(x) - 1]`\ \ :ansretval:`foo=`\ \ :ansretval:`bar.baz
-[123].bam[len(x) - 1]=`\ \ :ansretval:`foo=bar`\ \ :ansretval:`bar.baz[123].bam
-[len(x) - 1]=bar`\ \ :ansretval:`bam.baz.foo#lookup:foo`\ \ :ansretval:
-`bam.baz.foo#lookup:bar.baz[123].bam[len(x) - 1]`\ \ :ansretval:
+md: |- foo bar\.baz\[123\]\.bam\[len\(x\) \- 1\] foo\= bar\.baz\[123\]\.bam\
+[len\(x\) \- 1\]\= foo\=bar bar\.baz\[123\]\.bam\[len\(x\) \- 1\]\=bar foo
+bar\.baz\[123\]\.bam\[len\(x\) \- 1\] foo\= bar\.baz\[123\]\.bam\[len\(x\) \-
+1\]\= foo\=bar bar\.baz\[123\]\.bam\[len\(x\) \- 1\]\=bar foo bar\.baz\
+[123\]\.bam\[len\(x\) \- 1\] foo\= bar\.baz\[123\]\.bam\[len\(x\) \- 1\]\=
+foo\=bar bar\.baz\[123\]\.bam\[len\(x\) \- 1\]\=bar rst: |- \ :ansretval:`foo`\
+\ :ansretval:`bar.baz[123].bam[len(x) - 1]`\ \ :ansretval:`foo=`\ \ :ansretval:
+`bar.baz[123].bam[len(x) - 1]=`\ \ :ansretval:`foo=bar`\ \ :ansretval:`bar.baz
+[123].bam[len(x) - 1]=bar`\ \ :ansretval:`bam.baz.foo#lookup:foo`\ \ :
+ansretval:`bam.baz.foo#lookup:bar.baz[123].bam[len(x) - 1]`\ \ :ansretval:
 `bam.baz.foo#lookup:foo=`\ \ :ansretval:`bam.baz.foo#lookup:bar.baz[123].bam
 [len(x) - 1]=`\ \ :ansretval:`bam.baz.foo#lookup:foo=bar`\ \ :ansretval:
 `bam.baz.foo#lookup:bar.baz[123].bam[len(x) - 1]=bar`\ \ :ansretval:`foo`\ \ :
 ansretval:`bar.baz[123].bam[len(x) - 1]`\ \ :ansretval:`foo=`\ \ :ansretval:
 `bar.baz[123].bam[len(x) - 1]=`\ \ :ansretval:`foo=bar`\ \ :ansretval:`bar.baz
 [123].bam[len(x) - 1]=bar`\ ansible_doc_text: |- `foo' `bar.baz[123].bam[len(x)
 - 1]' `foo=' `bar.baz[123].bam[len(x) - 1]=' `foo=bar' `bar.baz[123].bam[len(x)
@@ -899,35 +860,32 @@
 [123].bam[len(x) - 1]=' (of lookup plugin bam.baz.foo) `foo=bar' (of lookup
 plugin bam.baz.foo) `bar.baz[123].bam[len(x) - 1]=bar' (of lookup plugin
 bam.baz.foo) `foo' `bar.baz[123].bam[len(x) - 1]' `foo=' `bar.baz[123].bam[len
 (x) - 1]=' `foo=bar' `bar.baz[123].bam[len(x) - 1]=bar' rst_plain: |- \ :
 literal:`foo`\ \ :literal:`bar.baz[123].bam[len(x) - 1]`\ \ :literal:`foo=`\ \
 :literal:`bar.baz[123].bam[len(x) - 1]=`\ \ :literal:`foo=bar`\ \ :literal:
 `bar.baz[123].bam[len(x) - 1]=bar`\ \ :literal:`foo` (of lookup plugin :ref:
-`bam.baz.foo
-bam.baz.foo_lookup>`)\ \ :literal:`bar.baz[123].bam[len(x) - 1]` (of lookup
-plugin :ref:`bam.baz.foo
-bam.baz.foo_lookup>`)\ \ :literal:`foo=` (of lookup plugin :ref:`bam.baz.foo
-bam.baz.foo_lookup>`)\ \ :literal:`bar.baz[123].bam[len(x) - 1]=` (of lookup
-plugin :ref:`bam.baz.foo
+`bam.baz.foo bam.baz.foo_lookup>`)\ \ :literal:`bar.baz[123].bam[len(x) - 1]`
+(of lookup plugin :ref:`bam.baz.foo bam.baz.foo_lookup>`)\ \ :literal:`foo=`
+(of lookup plugin :ref:`bam.baz.foo bam.baz.foo_lookup>`)\ \ :literal:`bar.baz
+[123].bam[len(x) - 1]=` (of lookup plugin :ref:`bam.baz.foo
 bam.baz.foo_lookup>`)\ \ :literal:`foo=bar` (of lookup plugin :ref:`bam.baz.foo
 bam.baz.foo_lookup>`)\ \ :literal:`bar.baz[123].bam[len(x) - 1]=bar` (of lookup
-plugin :ref:`bam.baz.foo
-bam.baz.foo_lookup>`)\ \ :literal:`foo`\ \ :literal:`bar.baz[123].bam[len(x) -
-1]`\ \ :literal:`foo=`\ \ :literal:`bar.baz[123].bam[len(x) - 1]=`\ \ :literal:
-`foo=bar`\ \ :literal:`bar.baz[123].bam[len(x) - 1]=bar`\
-return_value_current_plugin: source: - |- RV(foo) RV(bar.baz[123].bam[len(x\) -
-1]) - |- RV(foo=) RV(bar.baz[123].bam[len(x\) - 1]=) - |- RV(foo=bar) RV
-(bar.baz[123].bam[len(x\) - 1]=bar) - |- RV(bam.baz.foo#lookup:foo) RV
-(bam.baz.foo#lookup:bar.baz[123].bam[len(x\) - 1]) - |- RV(bam.baz.foo#lookup:
-foo=) RV(bam.baz.foo#lookup:bar.baz[123].bam[len(x\) - 1]=) - |- RV
-(bam.baz.foo#lookup:foo=bar) RV(bam.baz.foo#lookup:bar.baz[123].bam[len(x\) -
-1]=bar) - |- RV(ignore:foo) RV(ignore:bar.baz[123].bam[len(x\) - 1]) - |- RV
-(ignore:foo=) RV(ignore:bar.baz[123].bam[len(x\) - 1]=) - |- RV(ignore:foo=bar)
-RV(ignore:bar.baz[123].bam[len(x\) - 1]=bar) html: |-
+plugin :ref:`bam.baz.foo bam.baz.foo_lookup>`)\ \ :literal:`foo`\ \ :literal:
+`bar.baz[123].bam[len(x) - 1]`\ \ :literal:`foo=`\ \ :literal:`bar.baz[123].bam
+[len(x) - 1]=`\ \ :literal:`foo=bar`\ \ :literal:`bar.baz[123].bam[len(x) -
+1]=bar`\ return_value_current_plugin: source: - |- RV(foo) RV(bar.baz[123].bam
+[len(x\) - 1]) - |- RV(foo=) RV(bar.baz[123].bam[len(x\) - 1]=) - |- RV
+(foo=bar) RV(bar.baz[123].bam[len(x\) - 1]=bar) - |- RV(bam.baz.foo#lookup:foo)
+RV(bam.baz.foo#lookup:bar.baz[123].bam[len(x\) - 1]) - |- RV
+(bam.baz.foo#lookup:foo=) RV(bam.baz.foo#lookup:bar.baz[123].bam[len(x\) - 1]=)
+- |- RV(bam.baz.foo#lookup:foo=bar) RV(bam.baz.foo#lookup:bar.baz[123].bam[len
+(x\) - 1]=bar) - |- RV(ignore:foo) RV(ignore:bar.baz[123].bam[len(x\) - 1]) -
+|- RV(ignore:foo=) RV(ignore:bar.baz[123].bam[len(x\) - 1]=) - |- RV(ignore:
+foo=bar) RV(ignore:bar.baz[123].bam[len(x\) - 1]=bar) html: |-
 foo bar.baz[123].bam[len(x) - 1]
 foo= bar.baz[123].bam[len(x) - 1]=
 foo=bar bar.baz[123].bam[len(x) - 1]=bar
 foo bar.baz[123].bam[len(x) - 1]
 foo= bar.baz[123].bam[len(x) - 1]=
 foo=bar bar.baz[123].bam[len(x) - 1]=bar
 foo bar.baz[123].bam[len(x) - 1]
@@ -939,61 +897,57 @@
 foo=bar bar.baz[123].bam[len(x) - 1]=bar
 foo bar.baz[123].bam[len(x) - 1]
 foo= bar.baz[123].bam[len(x) - 1]=
 foo=bar bar.baz[123].bam[len(x) - 1]=bar
 foo bar.baz[123].bam[len(x) - 1]
 foo= bar.baz[123].bam[len(x) - 1]=
 foo=bar bar.baz[123].bam[len(x) - 1]=bar
-md: |- foo bar.baz\[123\].bam\[len\(x\) \- 1\] foo\= bar.baz\[123\].bam\[len\
-(x\) \- 1\]\= foo\=bar bar.baz\[123\].bam\[len\(x\) \- 1\]\=bar foo bar.baz\
-[123\].bam\[len\(x\) \- 1\] foo\= bar.baz\[123\].bam\[len\(x\) \- 1\]\=
-foo\=bar bar.baz\[123\].bam\[len\(x\) \- 1\]\=bar foo bar.baz\[123\].bam\[len\
-(x\) \- 1\] foo\= bar.baz\[123\].bam\[len\(x\) \- 1\]\= foo\=bar bar.baz\
-[123\].bam\[len\(x\) \- 1\]\=bar rst: |- \ :ansretval:`foo.bar.baz.bam#boo:
-foo`\ \ :ansretval:`foo.bar.baz.bam#boo:bar.baz[123].bam[len(x) - 1]`\ \ :
-ansretval:`foo.bar.baz.bam#boo:foo=`\ \ :ansretval:`foo.bar.baz.bam#boo:bar.baz
-[123].bam[len(x) - 1]=`\ \ :ansretval:`foo.bar.baz.bam#boo:foo=bar`\ \ :
-ansretval:`foo.bar.baz.bam#boo:bar.baz[123].bam[len(x) - 1]=bar`\ \ :ansretval:
-`bam.baz.foo#lookup:foo`\ \ :ansretval:`bam.baz.foo#lookup:bar.baz[123].bam[len
-(x) - 1]`\ \ :ansretval:`bam.baz.foo#lookup:foo=`\ \ :ansretval:
-`bam.baz.foo#lookup:bar.baz[123].bam[len(x) - 1]=`\ \ :ansretval:
-`bam.baz.foo#lookup:foo=bar`\ \ :ansretval:`bam.baz.foo#lookup:bar.baz[123].bam
-[len(x) - 1]=bar`\ \ :ansretval:`foo`\ \ :ansretval:`bar.baz[123].bam[len(x) -
-1]`\ \ :ansretval:`foo=`\ \ :ansretval:`bar.baz[123].bam[len(x) - 1]=`\ \ :
-ansretval:`foo=bar`\ \ :ansretval:`bar.baz[123].bam[len(x) - 1]=bar`\
-parse_opts: current_plugin: fqcn: foo.bar.baz.bam type: boo ansible_doc_text:
-|- `foo' (of boo plugin foo.bar.baz.bam) `bar.baz[123].bam[len(x) - 1]' (of boo
-plugin foo.bar.baz.bam) `foo=' (of boo plugin foo.bar.baz.bam) `bar.baz
-[123].bam[len(x) - 1]=' (of boo plugin foo.bar.baz.bam) `foo=bar' (of boo
-plugin foo.bar.baz.bam) `bar.baz[123].bam[len(x) - 1]=bar' (of boo plugin
-foo.bar.baz.bam) `foo' (of lookup plugin bam.baz.foo) `bar.baz[123].bam[len(x)
-- 1]' (of lookup plugin bam.baz.foo) `foo=' (of lookup plugin bam.baz.foo)
-`bar.baz[123].bam[len(x) - 1]=' (of lookup plugin bam.baz.foo) `foo=bar' (of
-lookup plugin bam.baz.foo) `bar.baz[123].bam[len(x) - 1]=bar' (of lookup plugin
-bam.baz.foo) `foo' `bar.baz[123].bam[len(x) - 1]' `foo=' `bar.baz[123].bam[len
-(x) - 1]=' `foo=bar' `bar.baz[123].bam[len(x) - 1]=bar' rst_plain: |- \ :
-literal:`foo` (of boo plugin :ref:`foo.bar.baz.bam
-foo.bar.baz.bam_boo>`)\ \ :literal:`bar.baz[123].bam[len(x) - 1]` (of boo
-plugin :ref:`foo.bar.baz.bam
+md: |- foo bar\.baz\[123\]\.bam\[len\(x\) \- 1\] foo\= bar\.baz\[123\]\.bam\
+[len\(x\) \- 1\]\= foo\=bar bar\.baz\[123\]\.bam\[len\(x\) \- 1\]\=bar foo
+bar\.baz\[123\]\.bam\[len\(x\) \- 1\] foo\= bar\.baz\[123\]\.bam\[len\(x\) \-
+1\]\= foo\=bar bar\.baz\[123\]\.bam\[len\(x\) \- 1\]\=bar foo bar\.baz\
+[123\]\.bam\[len\(x\) \- 1\] foo\= bar\.baz\[123\]\.bam\[len\(x\) \- 1\]\=
+foo\=bar bar\.baz\[123\]\.bam\[len\(x\) \- 1\]\=bar rst: |- \ :ansretval:
+`foo.bar.baz.bam#boo:foo`\ \ :ansretval:`foo.bar.baz.bam#boo:bar.baz[123].bam
+[len(x) - 1]`\ \ :ansretval:`foo.bar.baz.bam#boo:foo=`\ \ :ansretval:
+`foo.bar.baz.bam#boo:bar.baz[123].bam[len(x) - 1]=`\ \ :ansretval:
+`foo.bar.baz.bam#boo:foo=bar`\ \ :ansretval:`foo.bar.baz.bam#boo:bar.baz
+[123].bam[len(x) - 1]=bar`\ \ :ansretval:`bam.baz.foo#lookup:foo`\ \ :
+ansretval:`bam.baz.foo#lookup:bar.baz[123].bam[len(x) - 1]`\ \ :ansretval:
+`bam.baz.foo#lookup:foo=`\ \ :ansretval:`bam.baz.foo#lookup:bar.baz[123].bam
+[len(x) - 1]=`\ \ :ansretval:`bam.baz.foo#lookup:foo=bar`\ \ :ansretval:
+`bam.baz.foo#lookup:bar.baz[123].bam[len(x) - 1]=bar`\ \ :ansretval:`foo`\ \ :
+ansretval:`bar.baz[123].bam[len(x) - 1]`\ \ :ansretval:`foo=`\ \ :ansretval:
+`bar.baz[123].bam[len(x) - 1]=`\ \ :ansretval:`foo=bar`\ \ :ansretval:`bar.baz
+[123].bam[len(x) - 1]=bar`\ parse_opts: currentPlugin: fqcn: foo.bar.baz.bam
+type: boo ansible_doc_text: |- `foo' (of boo plugin foo.bar.baz.bam) `bar.baz
+[123].bam[len(x) - 1]' (of boo plugin foo.bar.baz.bam) `foo=' (of boo plugin
+foo.bar.baz.bam) `bar.baz[123].bam[len(x) - 1]=' (of boo plugin
+foo.bar.baz.bam) `foo=bar' (of boo plugin foo.bar.baz.bam) `bar.baz[123].bam
+[len(x) - 1]=bar' (of boo plugin foo.bar.baz.bam) `foo' (of lookup plugin
+bam.baz.foo) `bar.baz[123].bam[len(x) - 1]' (of lookup plugin bam.baz.foo)
+`foo=' (of lookup plugin bam.baz.foo) `bar.baz[123].bam[len(x) - 1]=' (of
+lookup plugin bam.baz.foo) `foo=bar' (of lookup plugin bam.baz.foo) `bar.baz
+[123].bam[len(x) - 1]=bar' (of lookup plugin bam.baz.foo) `foo' `bar.baz
+[123].bam[len(x) - 1]' `foo=' `bar.baz[123].bam[len(x) - 1]=' `foo=bar'
+`bar.baz[123].bam[len(x) - 1]=bar' rst_plain: |- \ :literal:`foo` (of boo
+plugin :ref:`foo.bar.baz.bam foo.bar.baz.bam_boo>`)\ \ :literal:`bar.baz
+[123].bam[len(x) - 1]` (of boo plugin :ref:`foo.bar.baz.bam
 foo.bar.baz.bam_boo>`)\ \ :literal:`foo=` (of boo plugin :ref:`foo.bar.baz.bam
 foo.bar.baz.bam_boo>`)\ \ :literal:`bar.baz[123].bam[len(x) - 1]=` (of boo
-plugin :ref:`foo.bar.baz.bam
-foo.bar.baz.bam_boo>`)\ \ :literal:`foo=bar` (of boo plugin :ref:
-`foo.bar.baz.bam
-foo.bar.baz.bam_boo>`)\ \ :literal:`bar.baz[123].bam[len(x) - 1]=bar` (of boo
-plugin :ref:`foo.bar.baz.bam
+plugin :ref:`foo.bar.baz.bam foo.bar.baz.bam_boo>`)\ \ :literal:`foo=bar` (of
+boo plugin :ref:`foo.bar.baz.bam foo.bar.baz.bam_boo>`)\ \ :literal:`bar.baz
+[123].bam[len(x) - 1]=bar` (of boo plugin :ref:`foo.bar.baz.bam
 foo.bar.baz.bam_boo>`)\ \ :literal:`foo` (of lookup plugin :ref:`bam.baz.foo
 bam.baz.foo_lookup>`)\ \ :literal:`bar.baz[123].bam[len(x) - 1]` (of lookup
-plugin :ref:`bam.baz.foo
-bam.baz.foo_lookup>`)\ \ :literal:`foo=` (of lookup plugin :ref:`bam.baz.foo
-bam.baz.foo_lookup>`)\ \ :literal:`bar.baz[123].bam[len(x) - 1]=` (of lookup
-plugin :ref:`bam.baz.foo
-bam.baz.foo_lookup>`)\ \ :literal:`foo=bar` (of lookup plugin :ref:`bam.baz.foo
-bam.baz.foo_lookup>`)\ \ :literal:`bar.baz[123].bam[len(x) - 1]=bar` (of lookup
-plugin :ref:`bam.baz.foo
+plugin :ref:`bam.baz.foo bam.baz.foo_lookup>`)\ \ :literal:`foo=` (of lookup
+plugin :ref:`bam.baz.foo bam.baz.foo_lookup>`)\ \ :literal:`bar.baz[123].bam
+[len(x) - 1]=` (of lookup plugin :ref:`bam.baz.foo bam.baz.foo_lookup>`)\ \ :
+literal:`foo=bar` (of lookup plugin :ref:`bam.baz.foo bam.baz.foo_lookup>`)\ \
+:literal:`bar.baz[123].bam[len(x) - 1]=bar` (of lookup plugin :ref:`bam.baz.foo
 bam.baz.foo_lookup>`)\ \ :literal:`foo`\ \ :literal:`bar.baz[123].bam[len(x) -
 1]`\ \ :literal:`foo=`\ \ :literal:`bar.baz[123].bam[len(x) - 1]=`\ \ :literal:
 `foo=bar`\ \ :literal:`bar.baz[123].bam[len(x) - 1]=bar`\
 return_value_no_current_plugin_w_links: source: - |- RV(foo) RV(bar.baz
 [123].bam[len(x\) - 1]) - |- RV(foo=) RV(bar.baz[123].bam[len(x\) - 1]=) - |-
 RV(foo=bar) RV(bar.baz[123].bam[len(x\) - 1]=bar) - |- RV(bam.baz.foo#lookup:
 foo) RV(bam.baz.foo#lookup:bar.baz[123].bam[len(x\) - 1]) - |- RV
@@ -1023,25 +977,25 @@
 foo=bar bar.baz[123].bam[len(x) - 1]=bar
 foo bar.baz[123].bam[len(x)_-_1]
 foo= bar.baz[123].bam[len(x)_-_1]=
 foo=bar bar.baz[123].bam[len(x)_-_1]=bar
 foo bar.baz[123].bam[len(x) - 1]
 foo= bar.baz[123].bam[len(x) - 1]=
 foo=bar bar.baz[123].bam[len(x) - 1]=bar
-md: |- foo bar.baz\[123\].bam\[len\(x\) \- 1\] foo\= bar.baz\[123\].bam\[len\
-(x\) \- 1\]\= foo\=bar bar.baz\[123\].bam\[len\(x\) \- 1\]\=bar foo bar.baz\
-[123\].bam\[len\(x\)_\-_1\] foo\= bar.baz\[123\].bam\[len\(x\)_\-_1\]\=
-foo\=bar bar.baz\[123\].bam\[len\(x\)_\-_1\]\=bar foo bar.baz\[123\].bam\[len\
-(x\) \- 1\] foo\= bar.baz\[123\].bam\[len\(x\) \- 1\]\= foo\=bar bar.baz\
-[123\].bam\[len\(x\) \- 1\]\=bar md_opts: pluginOptionLikeLink.js: |- (plugin,
-entrypoint, what, name, current_plugin) => `https://docs.ansible.com/ansible/
-devel/collections/${plugin.fqcn.replace(/\./g, '/')}_${plugin.type}.html#$
-{what}${entrypoint ? '-' + entrypoint : ''}-${name.join('/')}`
-pluginOptionLikeLink.py: |- lambda plugin, entrypoint, what, name,
-current_plugin: f"https://docs.ansible.com/ansible/devel/collections/
+md: |- foo bar\.baz\[123\]\.bam\[len\(x\) \- 1\] foo\= bar\.baz\[123\]\.bam\
+[len\(x\) \- 1\]\= foo\=bar bar\.baz\[123\]\.bam\[len\(x\) \- 1\]\=bar foo
+bar\.baz\[123\]\.bam\[len\(x\)_\-_1\] foo\= bar\.baz\[123\]\.bam\[len\(x\)_\-
+1\]\= foo\=bar bar\.baz\[123\]\.bam\[len\(x\)_\-_1\]\=bar foo bar\.baz\
+[123\]\.bam\[len\(x\) \- 1\] foo\= bar\.baz\[123\]\.bam\[len\(x\) \- 1\]\=
+foo\=bar bar\.baz\[123\]\.bam\[len\(x\) \- 1\]\=bar md_opts:
+pluginOptionLikeLink.js: |- (plugin, entrypoint, what, name, current_plugin) =>
+`https://docs.ansible.com/ansible/devel/collections/${plugin.fqcn.replace(/\./
+g, '/')}_${plugin.type}.html#${what}${entrypoint ? '-' + entrypoint : ''}-$
+{name.join('/')}` pluginOptionLikeLink.py: |- lambda plugin, entrypoint, what,
+name, current_plugin: f"https://docs.ansible.com/ansible/devel/collections/
 {plugin.fqcn.replace('.', '/')}_{plugin.type}.html#{what}{'-' + entrypoint if
 entrypoint else ''}-{'/'.join(name)}" rst: |- \ :ansretval:`foo`\ \ :ansretval:
 `bar.baz[123].bam[len(x) - 1]`\ \ :ansretval:`foo=`\ \ :ansretval:`bar.baz
 [123].bam[len(x) - 1]=`\ \ :ansretval:`foo=bar`\ \ :ansretval:`bar.baz[123].bam
 [len(x) - 1]=bar`\ \ :ansretval:`bam.baz.foo#lookup:foo`\ \ :ansretval:
 `bam.baz.foo#lookup:bar.baz[123].bam[len(x) - 1]`\ \ :ansretval:
 `bam.baz.foo#lookup:foo=`\ \ :ansretval:`bam.baz.foo#lookup:bar.baz[123].bam
@@ -1056,30 +1010,27 @@
 [123].bam[len(x) - 1]=' (of lookup plugin bam.baz.foo) `foo=bar' (of lookup
 plugin bam.baz.foo) `bar.baz[123].bam[len(x) - 1]=bar' (of lookup plugin
 bam.baz.foo) `foo' `bar.baz[123].bam[len(x) - 1]' `foo=' `bar.baz[123].bam[len
 (x) - 1]=' `foo=bar' `bar.baz[123].bam[len(x) - 1]=bar' rst_plain: |- \ :
 literal:`foo`\ \ :literal:`bar.baz[123].bam[len(x) - 1]`\ \ :literal:`foo=`\ \
 :literal:`bar.baz[123].bam[len(x) - 1]=`\ \ :literal:`foo=bar`\ \ :literal:
 `bar.baz[123].bam[len(x) - 1]=bar`\ \ :literal:`foo` (of lookup plugin :ref:
-`bam.baz.foo
-bam.baz.foo_lookup>`)\ \ :literal:`bar.baz[123].bam[len(x) - 1]` (of lookup
-plugin :ref:`bam.baz.foo
-bam.baz.foo_lookup>`)\ \ :literal:`foo=` (of lookup plugin :ref:`bam.baz.foo
-bam.baz.foo_lookup>`)\ \ :literal:`bar.baz[123].bam[len(x) - 1]=` (of lookup
-plugin :ref:`bam.baz.foo
+`bam.baz.foo bam.baz.foo_lookup>`)\ \ :literal:`bar.baz[123].bam[len(x) - 1]`
+(of lookup plugin :ref:`bam.baz.foo bam.baz.foo_lookup>`)\ \ :literal:`foo=`
+(of lookup plugin :ref:`bam.baz.foo bam.baz.foo_lookup>`)\ \ :literal:`bar.baz
+[123].bam[len(x) - 1]=` (of lookup plugin :ref:`bam.baz.foo
 bam.baz.foo_lookup>`)\ \ :literal:`foo=bar` (of lookup plugin :ref:`bam.baz.foo
 bam.baz.foo_lookup>`)\ \ :literal:`bar.baz[123].bam[len(x) - 1]=bar` (of lookup
-plugin :ref:`bam.baz.foo
-bam.baz.foo_lookup>`)\ \ :literal:`foo`\ \ :literal:`bar.baz[123].bam[len(x) -
-1]`\ \ :literal:`foo=`\ \ :literal:`bar.baz[123].bam[len(x) - 1]=`\ \ :literal:
-`foo=bar`\ \ :literal:`bar.baz[123].bam[len(x) - 1]=bar`\
-return_value_current_plugin_w_links: source: - |- RV(foo) RV(bar.baz[123].bam
-[len(x\) - 1]) - |- RV(foo=) RV(bar.baz[123].bam[len(x\) - 1]=) - |- RV
-(foo=bar) RV(bar.baz[123].bam[len(x\) - 1]=bar) - |- RV(bam.baz.foo#lookup:foo)
-RV(bam.baz.foo#lookup:bar.baz[123].bam[len(x\) - 1]) - |- RV
+plugin :ref:`bam.baz.foo bam.baz.foo_lookup>`)\ \ :literal:`foo`\ \ :literal:
+`bar.baz[123].bam[len(x) - 1]`\ \ :literal:`foo=`\ \ :literal:`bar.baz[123].bam
+[len(x) - 1]=`\ \ :literal:`foo=bar`\ \ :literal:`bar.baz[123].bam[len(x) -
+1]=bar`\ return_value_current_plugin_w_links: source: - |- RV(foo) RV(bar.baz
+[123].bam[len(x\) - 1]) - |- RV(foo=) RV(bar.baz[123].bam[len(x\) - 1]=) - |-
+RV(foo=bar) RV(bar.baz[123].bam[len(x\) - 1]=bar) - |- RV(bam.baz.foo#lookup:
+foo) RV(bam.baz.foo#lookup:bar.baz[123].bam[len(x\) - 1]) - |- RV
 (bam.baz.foo#lookup:foo=) RV(bam.baz.foo#lookup:bar.baz[123].bam[len(x\) - 1]=)
 - |- RV(bam.baz.foo#lookup:foo=bar) RV(bam.baz.foo#lookup:bar.baz[123].bam[len
 (x\) - 1]=bar) - |- RV(ignore:foo) RV(ignore:bar.baz[123].bam[len(x\) - 1]) -
 |- RV(ignore:foo=) RV(ignore:bar.baz[123].bam[len(x\) - 1]=) - |- RV(ignore:
 foo=bar) RV(ignore:bar.baz[123].bam[len(x\) - 1]=bar) html: |-
 foo bar.baz[123].bam[len(x)_-_1]
 foo= bar.baz[123].bam[len(x)_-_1]=
@@ -1102,69 +1053,64 @@
 foo=bar bar.baz[123].bam[len(x)_-_1]=bar
 foo bar.baz[123].bam[len(x)_-_1]
 foo= bar.baz[123].bam[len(x)_-_1]=
 foo=bar bar.baz[123].bam[len(x)_-_1]=bar
 foo bar.baz[123].bam[len(x) - 1]
 foo= bar.baz[123].bam[len(x) - 1]=
 foo=bar bar.baz[123].bam[len(x) - 1]=bar
-md: |- foo bar.baz\[123\].bam\[len\(x\)_\-_1\] foo\= bar.baz\[123\].bam\[len\
-(x\)_\-_1\]\= foo\=bar bar.baz\[123\].bam\[len\(x\)_\-_1\]\=bar foo bar.baz\
-[123\].bam\[len\(x\)_\-_1\] foo\= bar.baz\[123\].bam\[len\(x\)_\-_1\]\=
-foo\=bar bar.baz\[123\].bam\[len\(x\)_\-_1\]\=bar foo bar.baz\[123\].bam\[len\
-(x\) \- 1\] foo\= bar.baz\[123\].bam\[len\(x\) \- 1\]\= foo\=bar bar.baz\
-[123\].bam\[len\(x\) \- 1\]\=bar md_opts: pluginOptionLikeLink.js: |- (plugin,
-entrypoint, what, name, current_plugin) => `https://docs.ansible.com/ansible/
-devel/collections/${plugin.fqcn.replace(/\./g, '/')}_${plugin.type}.html#$
-{what}${entrypoint ? '-' + entrypoint : ''}-${name.join('/')}`
-pluginOptionLikeLink.py: |- lambda plugin, entrypoint, what, name,
-current_plugin: f"https://docs.ansible.com/ansible/devel/collections/
+md: |- foo bar\.baz\[123\]\.bam\[len\(x\)_\-_1\] foo\= bar\.baz\[123\]\.bam\
+[len\(x\)_\-_1\]\= foo\=bar bar\.baz\[123\]\.bam\[len\(x\)_\-_1\]\=bar foo
+bar\.baz\[123\]\.bam\[len\(x\)_\-_1\] foo\= bar\.baz\[123\]\.bam\[len\(x\)_\-
+1\]\= foo\=bar bar\.baz\[123\]\.bam\[len\(x\)_\-_1\]\=bar foo bar\.baz\
+[123\]\.bam\[len\(x\) \- 1\] foo\= bar\.baz\[123\]\.bam\[len\(x\) \- 1\]\=
+foo\=bar bar\.baz\[123\]\.bam\[len\(x\) \- 1\]\=bar md_opts:
+pluginOptionLikeLink.js: |- (plugin, entrypoint, what, name, current_plugin) =>
+`https://docs.ansible.com/ansible/devel/collections/${plugin.fqcn.replace(/\./
+g, '/')}_${plugin.type}.html#${what}${entrypoint ? '-' + entrypoint : ''}-$
+{name.join('/')}` pluginOptionLikeLink.py: |- lambda plugin, entrypoint, what,
+name, current_plugin: f"https://docs.ansible.com/ansible/devel/collections/
 {plugin.fqcn.replace('.', '/')}_{plugin.type}.html#{what}{'-' + entrypoint if
 entrypoint else ''}-{'/'.join(name)}" rst: |- \ :ansretval:
 `foo.bar.baz.bam#boo:foo`\ \ :ansretval:`foo.bar.baz.bam#boo:bar.baz[123].bam
 [len(x) - 1]`\ \ :ansretval:`foo.bar.baz.bam#boo:foo=`\ \ :ansretval:
 `foo.bar.baz.bam#boo:bar.baz[123].bam[len(x) - 1]=`\ \ :ansretval:
 `foo.bar.baz.bam#boo:foo=bar`\ \ :ansretval:`foo.bar.baz.bam#boo:bar.baz
 [123].bam[len(x) - 1]=bar`\ \ :ansretval:`bam.baz.foo#lookup:foo`\ \ :
 ansretval:`bam.baz.foo#lookup:bar.baz[123].bam[len(x) - 1]`\ \ :ansretval:
 `bam.baz.foo#lookup:foo=`\ \ :ansretval:`bam.baz.foo#lookup:bar.baz[123].bam
 [len(x) - 1]=`\ \ :ansretval:`bam.baz.foo#lookup:foo=bar`\ \ :ansretval:
 `bam.baz.foo#lookup:bar.baz[123].bam[len(x) - 1]=bar`\ \ :ansretval:`foo`\ \ :
 ansretval:`bar.baz[123].bam[len(x) - 1]`\ \ :ansretval:`foo=`\ \ :ansretval:
 `bar.baz[123].bam[len(x) - 1]=`\ \ :ansretval:`foo=bar`\ \ :ansretval:`bar.baz
-[123].bam[len(x) - 1]=bar`\ parse_opts: current_plugin: fqcn: foo.bar.baz.bam
+[123].bam[len(x) - 1]=bar`\ parse_opts: currentPlugin: fqcn: foo.bar.baz.bam
 type: boo ansible_doc_text: |- `foo' (of boo plugin foo.bar.baz.bam) `bar.baz
 [123].bam[len(x) - 1]' (of boo plugin foo.bar.baz.bam) `foo=' (of boo plugin
 foo.bar.baz.bam) `bar.baz[123].bam[len(x) - 1]=' (of boo plugin
 foo.bar.baz.bam) `foo=bar' (of boo plugin foo.bar.baz.bam) `bar.baz[123].bam
 [len(x) - 1]=bar' (of boo plugin foo.bar.baz.bam) `foo' (of lookup plugin
 bam.baz.foo) `bar.baz[123].bam[len(x) - 1]' (of lookup plugin bam.baz.foo)
 `foo=' (of lookup plugin bam.baz.foo) `bar.baz[123].bam[len(x) - 1]=' (of
 lookup plugin bam.baz.foo) `foo=bar' (of lookup plugin bam.baz.foo) `bar.baz
 [123].bam[len(x) - 1]=bar' (of lookup plugin bam.baz.foo) `foo' `bar.baz
 [123].bam[len(x) - 1]' `foo=' `bar.baz[123].bam[len(x) - 1]=' `foo=bar'
 `bar.baz[123].bam[len(x) - 1]=bar' rst_plain: |- \ :literal:`foo` (of boo
-plugin :ref:`foo.bar.baz.bam
-foo.bar.baz.bam_boo>`)\ \ :literal:`bar.baz[123].bam[len(x) - 1]` (of boo
-plugin :ref:`foo.bar.baz.bam
+plugin :ref:`foo.bar.baz.bam foo.bar.baz.bam_boo>`)\ \ :literal:`bar.baz
+[123].bam[len(x) - 1]` (of boo plugin :ref:`foo.bar.baz.bam
 foo.bar.baz.bam_boo>`)\ \ :literal:`foo=` (of boo plugin :ref:`foo.bar.baz.bam
 foo.bar.baz.bam_boo>`)\ \ :literal:`bar.baz[123].bam[len(x) - 1]=` (of boo
-plugin :ref:`foo.bar.baz.bam
-foo.bar.baz.bam_boo>`)\ \ :literal:`foo=bar` (of boo plugin :ref:
-`foo.bar.baz.bam
-foo.bar.baz.bam_boo>`)\ \ :literal:`bar.baz[123].bam[len(x) - 1]=bar` (of boo
-plugin :ref:`foo.bar.baz.bam
+plugin :ref:`foo.bar.baz.bam foo.bar.baz.bam_boo>`)\ \ :literal:`foo=bar` (of
+boo plugin :ref:`foo.bar.baz.bam foo.bar.baz.bam_boo>`)\ \ :literal:`bar.baz
+[123].bam[len(x) - 1]=bar` (of boo plugin :ref:`foo.bar.baz.bam
 foo.bar.baz.bam_boo>`)\ \ :literal:`foo` (of lookup plugin :ref:`bam.baz.foo
 bam.baz.foo_lookup>`)\ \ :literal:`bar.baz[123].bam[len(x) - 1]` (of lookup
-plugin :ref:`bam.baz.foo
-bam.baz.foo_lookup>`)\ \ :literal:`foo=` (of lookup plugin :ref:`bam.baz.foo
-bam.baz.foo_lookup>`)\ \ :literal:`bar.baz[123].bam[len(x) - 1]=` (of lookup
-plugin :ref:`bam.baz.foo
-bam.baz.foo_lookup>`)\ \ :literal:`foo=bar` (of lookup plugin :ref:`bam.baz.foo
-bam.baz.foo_lookup>`)\ \ :literal:`bar.baz[123].bam[len(x) - 1]=bar` (of lookup
-plugin :ref:`bam.baz.foo
+plugin :ref:`bam.baz.foo bam.baz.foo_lookup>`)\ \ :literal:`foo=` (of lookup
+plugin :ref:`bam.baz.foo bam.baz.foo_lookup>`)\ \ :literal:`bar.baz[123].bam
+[len(x) - 1]=` (of lookup plugin :ref:`bam.baz.foo bam.baz.foo_lookup>`)\ \ :
+literal:`foo=bar` (of lookup plugin :ref:`bam.baz.foo bam.baz.foo_lookup>`)\ \
+:literal:`bar.baz[123].bam[len(x) - 1]=bar` (of lookup plugin :ref:`bam.baz.foo
 bam.baz.foo_lookup>`)\ \ :literal:`foo`\ \ :literal:`bar.baz[123].bam[len(x) -
 1]`\ \ :literal:`foo=`\ \ :literal:`bar.baz[123].bam[len(x) - 1]=`\ \ :literal:
 `foo=bar`\ \ :literal:`bar.baz[123].bam[len(x) - 1]=bar`\ unhelpful_errors:
 source: - P(foo) - C(foo - R(foo,bar parse_opts: helpfulErrors: false html: |-
 ERROR while parsing: While parsing P() at index 1 of paragraph 1: Parameter
 "foo" is not of the form FQCN#type
 ERROR while parsing: While parsing C() at index 1 of paragraph 2: Cannot find
```

### Comparing `antsibull_docs_parser-0.3.0/.github/workflows/nox.yml` & `antsibull_docs_parser-0.4.0/.github/workflows/nox.yml`

 * *Files identical despite different names*

### Comparing `antsibull_docs_parser-0.3.0/changelogs/changelog.yaml` & `antsibull_docs_parser-0.4.0/changelogs/changelog.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -41,7 +41,19 @@
       minor_changes:
       - Add support for plain RST rendering (https://github.com/ansible-community/antsibull-docs-parser/pull/20).
       release_summary: Feature release.
     fragments:
     - 0.3.0.yml
     - 20-rst-plain.yml
     release_date: '2023-04-14'
+  0.4.0:
+    changes:
+      bugfixes:
+      - Fix URL escaping in MarkDown (https://github.com/ansible-community/antsibull-docs-parser/pull/24).
+      minor_changes:
+      - Adjust URL escaping to be more similar to JavaScript's ``encodeURI()`` (https://github.com/ansible-community/antsibull-docs-parser/pull/24).
+      - Also escape ``.`` in MarkDown (https://github.com/ansible-community/antsibull-docs-parser/pull/24).
+      release_summary: Feature and bugfix release.
+    fragments:
+    - 0.4.0.yml
+    - 24-urls-md.yml
+    release_date: '2023-04-23'
```

### Comparing `antsibull_docs_parser-0.3.0/changelogs/config.yaml` & `antsibull_docs_parser-0.4.0/changelogs/config.yaml`

 * *Files identical despite different names*

### Comparing `antsibull_docs_parser-0.3.0/src/antsibull_docs_parser/_parser_impl.py` & `antsibull_docs_parser-0.4.0/src/antsibull_docs_parser/_parser_impl.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs_parser-0.3.0/src/antsibull_docs_parser/ansible_doc_text.py` & `antsibull_docs_parser-0.4.0/src/antsibull_docs_parser/ansible_doc_text.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs_parser-0.3.0/src/antsibull_docs_parser/dom.py` & `antsibull_docs_parser-0.4.0/src/antsibull_docs_parser/dom.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs_parser-0.3.0/src/antsibull_docs_parser/format.py` & `antsibull_docs_parser-0.4.0/src/antsibull_docs_parser/format.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs_parser-0.3.0/src/antsibull_docs_parser/html.py` & `antsibull_docs_parser-0.4.0/src/antsibull_docs_parser/html.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,18 +17,17 @@
 
 
 def html_escape(text: str) -> str:
     return _html_escape(text).replace("&quot;", '"')
 
 
 def _url_escape(url: str) -> str:
-    # We include '<>[]{}' in safe to allow urls such as
-    # 'https://<HOST>:[PORT]/v{version}/' to remain unmangled by percent
-    # encoding
-    return quote(url, safe=":/#?%<>[]{}")
+    # We include several characters in safe to be compatible to JavaScript's encodeURI() method.
+    # https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/encodeURI
+    return quote(url, safe=":/#?!*'();@&=+$,")
 
 
 class AntsibullHTMLFormatter(Formatter):
     @staticmethod
     def _format_option_like(
         part: t.Union[dom.OptionNamePart, dom.ReturnValuePart], url: t.Optional[str]
     ) -> str:
```

### Comparing `antsibull_docs_parser-0.3.0/src/antsibull_docs_parser/md.py` & `antsibull_docs_parser-0.4.0/src/antsibull_docs_parser/md.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,30 +12,30 @@
 
 from . import dom
 from .format import Formatter, LinkProvider
 from .format import format_paragraphs as _format_paragraphs
 from .html import _url_escape
 from .html import html_escape as _html_escape
 
-_MD_ESCAPE = re.compile(r"""([!"#$%&'()*+,:;<=>?@[\\\]^_`{|}~-])""")
+_MD_ESCAPE = re.compile(r"""([!"#$%&'()*+,:;<=>?@[\\\]^_`{|}~.-])""")
 
 
 def md_escape(text: str) -> str:
     return _MD_ESCAPE.sub(r"\\\1", text)
 
 
 class MDFormatter(Formatter):
     @staticmethod
     def _format_option_like(
         part: t.Union[dom.OptionNamePart, dom.ReturnValuePart], url: t.Optional[str]
     ) -> str:
         link_start = ""
         link_end = ""
         if url:
-            link_start = f'<a href="{md_escape(_html_escape(_url_escape(url)))}">'
+            link_start = f'<a href="{_html_escape(_url_escape(url))}">'
             link_end = "</a>"
         strong_start = ""
         strong_end = ""
         if part.type == dom.PartType.OPTION_NAME and part.value is None:
             strong_start = "<strong>"
             strong_end = "</strong>"
         if part.value is None:
@@ -56,28 +56,26 @@
     def format_horizontal_line(self, part: dom.HorizontalLinePart) -> str:
         return "<hr>"
 
     def format_italic(self, part: dom.ItalicPart) -> str:
         return f"<em>{md_escape(part.text)}</em>"
 
     def format_link(self, part: dom.LinkPart) -> str:
-        return f"[{md_escape(part.text)}]({md_escape(_url_escape(part.url))})"
+        return f"[{md_escape(part.text)}]({_url_escape(part.url)})"
 
     def format_module(self, part: dom.ModulePart, url: t.Optional[str]) -> str:
         if url:
             return f"[{md_escape(part.fqcn)}]({md_escape(_url_escape(url))})"
         return md_escape(part.fqcn)
 
     def format_rst_ref(self, part: dom.RSTRefPart) -> str:
         return md_escape(part.text)
 
     def format_url(self, part: dom.URLPart) -> str:
-        return (
-            f"[{md_escape(_url_escape(part.url))}]({md_escape(_url_escape(part.url))})"
-        )
+        return f"[{md_escape(_url_escape(part.url))}]({_url_escape(part.url)})"
 
     def format_text(self, part: dom.TextPart) -> str:
         return md_escape(part.text)
 
     def format_env_variable(self, part: dom.EnvVariablePart) -> str:
         return f"<code>{md_escape(part.name)}</code>"
```

### Comparing `antsibull_docs_parser-0.3.0/src/antsibull_docs_parser/parser.py` & `antsibull_docs_parser-0.4.0/src/antsibull_docs_parser/parser.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs_parser-0.3.0/src/antsibull_docs_parser/rst.py` & `antsibull_docs_parser-0.4.0/src/antsibull_docs_parser/rst.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs_parser-0.3.0/tests/unit/create-vectors.py` & `antsibull_docs_parser-0.4.0/tests/unit/create-vectors.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from antsibull_docs_parser.md import to_md
 from antsibull_docs_parser.parser import parse
 from antsibull_docs_parser.rst import to_rst, to_rst_plain
 
 
 def add(test_data: t.Dict[str, t.Any], key: str, value: t.Any) -> None:
     if isinstance(value, str):
-        if key not in test_data and "\n" in value:
+        if "\n" in value:
             value = LiteralScalarString(value)
     test_data[key] = value
 
 
 def update(test_name: str, test_data: t.Dict[str, t.Any]) -> None:
     context, parse_opts = get_context_parse_opts(test_data)
     parsed = parse(test_data["source"], context, **parse_opts)
```

### Comparing `antsibull_docs_parser-0.3.0/tests/unit/test_dom.py` & `antsibull_docs_parser-0.4.0/tests/unit/test_dom.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs_parser-0.3.0/tests/unit/test_format.py` & `antsibull_docs_parser-0.4.0/tests/unit/test_format.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs_parser-0.3.0/tests/unit/test_html.py` & `antsibull_docs_parser-0.4.0/tests/unit/test_html.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs_parser-0.3.0/tests/unit/test_md.py` & `antsibull_docs_parser-0.4.0/tests/unit/test_md.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from antsibull_docs_parser.md import md_escape, to_md
 
 
 def test_md_escape():
     assert md_escape("") == ""
     assert md_escape("  foo  ") == "  foo  "
     assert (
-        md_escape(r"[]!.()-\@<>?[]!.()-\@<>?")
-        == r"\[\]\!.\(\)\-\\\@\<\>\?\[\]\!.\(\)\-\\\@\<\>\?"
+        md_escape(r"[]!.()-\@<>?[]!.()-\@<>?&")
+        == r"\[\]\!\.\(\)\-\\\@\<\>\?\[\]\!\.\(\)\-\\\@\<\>\?\&"
     )
 
 
 def test_to_rst():
     assert to_md([]) == ""
     assert to_md([[dom.TextPart(text="test")]]) == "test"
```

### Comparing `antsibull_docs_parser-0.3.0/tests/unit/test_parser.py` & `antsibull_docs_parser-0.4.0/tests/unit/test_parser.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs_parser-0.3.0/tests/unit/test_parser_impl.py` & `antsibull_docs_parser-0.4.0/tests/unit/test_parser_impl.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs_parser-0.3.0/tests/unit/test_rst.py` & `antsibull_docs_parser-0.4.0/tests/unit/test_rst.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs_parser-0.3.0/tests/unit/test_vectors.py` & `antsibull_docs_parser-0.4.0/tests/unit/test_vectors.py`

 * *Files identical despite different names*

### Comparing `antsibull_docs_parser-0.3.0/tests/unit/vectors.py` & `antsibull_docs_parser-0.4.0/tests/unit/vectors.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,21 +42,21 @@
             self._plugin_option_like_link = eval(config["pluginOptionLikeLink.py"])
 
 
 def get_context_parse_opts(test_data: t.Mapping[str, t.Any]):
     parse_opts = {}
     context_opts = {}
     if test_data.get("parse_opts"):
-        if "current_plugin" in test_data["parse_opts"]:
+        if "currentPlugin" in test_data["parse_opts"]:
             context_opts["current_plugin"] = dom.PluginIdentifier(
-                fqcn=test_data["parse_opts"]["current_plugin"]["fqcn"],
-                type=test_data["parse_opts"]["current_plugin"]["type"],
+                fqcn=test_data["parse_opts"]["currentPlugin"]["fqcn"],
+                type=test_data["parse_opts"]["currentPlugin"]["type"],
             )
-        if "role_entrypoint" in test_data["parse_opts"]:
-            context_opts["role_entrypoint"] = test_data["parse_opts"]["role_entrypoint"]
+        if "roleEntrypoint" in test_data["parse_opts"]:
+            context_opts["role_entrypoint"] = test_data["parse_opts"]["roleEntrypoint"]
         if "errors" in test_data["parse_opts"]:
             parse_opts["errors"] = test_data["parse_opts"]["errors"]
         if "onlyClassicMarkup" in test_data["parse_opts"]:
             parse_opts["only_classic_markup"] = test_data["parse_opts"][
                 "onlyClassicMarkup"
             ]
         if "helpfulErrors" in test_data["parse_opts"]:
@@ -68,49 +68,49 @@
     opts = {}
     link_provider = _TestLinkProvider()
     if test_data.get("html_opts"):
         if "parStart" in test_data["html_opts"]:
             opts["par_start"] = test_data["html_opts"]["parStart"]
         if "parEnd" in test_data["html_opts"]:
             opts["par_end"] = test_data["html_opts"]["parEnd"]
-        if "current_plugin" in test_data["html_opts"]:
+        if "currentPlugin" in test_data["html_opts"]:
             opts["current_plugin"] = dom.PluginIdentifier(
-                fqcn=test_data["html_opts"]["current_plugin"]["fqcn"],
-                type=test_data["html_opts"]["current_plugin"]["type"],
+                fqcn=test_data["html_opts"]["currentPlugin"]["fqcn"],
+                type=test_data["html_opts"]["currentPlugin"]["type"],
             )
         link_provider._update(test_data["html_opts"])
     return opts, link_provider
 
 
 def get_md_opts_link_provider(test_data: t.Mapping[str, t.Any]):
     opts = {}
     link_provider = _TestLinkProvider()
     if test_data.get("md_opts"):
-        if "current_plugin" in test_data["md_opts"]:
+        if "currentPlugin" in test_data["md_opts"]:
             opts["current_plugin"] = dom.PluginIdentifier(
-                fqcn=test_data["md_opts"]["current_plugin"]["fqcn"],
-                type=test_data["md_opts"]["current_plugin"]["type"],
+                fqcn=test_data["md_opts"]["currentPlugin"]["fqcn"],
+                type=test_data["md_opts"]["currentPlugin"]["type"],
             )
         link_provider._update(test_data["md_opts"])
     return opts, link_provider
 
 
 def get_rst_opts(test_data: t.Mapping[str, t.Any]):
     opts = {}
     if test_data.get("rst_opts"):
-        if "current_plugin" in test_data["rst_opts"]:
+        if "currentPlugin" in test_data["rst_opts"]:
             opts["current_plugin"] = dom.PluginIdentifier(
-                fqcn=test_data["rst_opts"]["current_plugin"]["fqcn"],
-                type=test_data["rst_opts"]["current_plugin"]["type"],
+                fqcn=test_data["rst_opts"]["currentPlugin"]["fqcn"],
+                type=test_data["rst_opts"]["currentPlugin"]["type"],
             )
     return opts
 
 
 def get_ansible_doc_text_opts(test_data: t.Mapping[str, t.Any]):
     opts = {}
     if test_data.get("ansible_doc_text_opts"):
-        if "current_plugin" in test_data["ansible_doc_text_opts"]:
+        if "currentPlugin" in test_data["ansible_doc_text_opts"]:
             opts["current_plugin"] = dom.PluginIdentifier(
-                fqcn=test_data["ansible_doc_text_opts"]["current_plugin"]["fqcn"],
-                type=test_data["ansible_doc_text_opts"]["current_plugin"]["type"],
+                fqcn=test_data["ansible_doc_text_opts"]["currentPlugin"]["fqcn"],
+                type=test_data["ansible_doc_text_opts"]["currentPlugin"]["type"],
             )
     return opts
```

### Comparing `antsibull_docs_parser-0.3.0/.gitignore` & `antsibull_docs_parser-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `antsibull_docs_parser-0.3.0/README.md` & `antsibull_docs_parser-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `antsibull_docs_parser-0.3.0/pyproject.toml` & `antsibull_docs_parser-0.4.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "antsibull-docs-parser"
-version = "0.3.0"
+version = "0.4.0"
 description = "Python library for processing Ansible documentation markup"
 readme = "README.md"
 requires-python = ">=3.6.1"
 license = "GPL-3.0-or-later AND BSD-2-Clause"
 license-files.globs = ["LICENSES/*.txt"]
 authors = [
   { name = "Felix Fontein", email = "felix@fontein.de" },
```

### Comparing `antsibull_docs_parser-0.3.0/LICENSES/BSD-2-Clause.txt` & `antsibull_docs_parser-0.4.0/LICENSES/BSD-2-Clause.txt`

 * *Files identical despite different names*

### Comparing `antsibull_docs_parser-0.3.0/PKG-INFO` & `antsibull_docs_parser-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antsibull-docs-parser
-Version: 0.3.0
+Version: 0.4.0
 Summary: Python library for processing Ansible documentation markup
 Project-URL: Source code, https://github.com/ansible-community/antsibull-docs-parser/
 Author-email: Felix Fontein <felix@fontein.de>
 Maintainer-email: Felix Fontein <felix@fontein.de>, Maxwell G <maxwell@gtmx.me>
 License-Expression: GPL-3.0-or-later AND BSD-2-Clause
 License-File: LICENSES/BSD-2-Clause.txt
 License-File: LICENSES/GPL-3.0-or-later.txt
```

