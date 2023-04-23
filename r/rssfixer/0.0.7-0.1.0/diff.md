# Comparing `tmp/rssfixer-0.0.7.tar.gz` & `tmp/rssfixer-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rssfixer-0.0.7.tar", last modified: Sat Apr 22 07:41:52 2023, max compression
+gzip compressed data, was "rssfixer-0.1.0.tar", last modified: Sun Apr 23 11:36:05 2023, max compression
```

## Comparing `rssfixer-0.0.7.tar` & `rssfixer-0.1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 reuteras   (501) staff       (20)        0 2023-04-22 07:41:52.402802 rssfixer-0.0.7/
--rw-r--r--   0 reuteras   (501) staff       (20)     1058 2023-04-16 10:16:56.000000 rssfixer-0.0.7/LICENSE
--rw-r--r--   0 reuteras   (501) staff       (20)     5336 2023-04-22 07:41:52.402645 rssfixer-0.0.7/PKG-INFO
--rw-r--r--   0 reuteras   (501) staff       (20)     4533 2023-04-22 07:29:10.000000 rssfixer-0.0.7/README.md
--rw-r--r--   0 reuteras   (501) staff       (20)     1110 2023-04-22 07:36:07.000000 rssfixer-0.0.7/pyproject.toml
--rw-r--r--   0 reuteras   (501) staff       (20)       38 2023-04-22 07:41:52.402849 rssfixer-0.0.7/setup.cfg
-drwxr-xr-x   0 reuteras   (501) staff       (20)        0 2023-04-22 07:41:52.399063 rssfixer-0.0.7/src/
-drwxr-xr-x   0 reuteras   (501) staff       (20)        0 2023-04-22 07:41:52.400534 rssfixer-0.0.7/src/rssfixer/
--rw-r--r--   0 reuteras   (501) staff       (20)       81 2023-04-22 06:11:44.000000 rssfixer-0.0.7/src/rssfixer/__init__.py
--rw-r--r--   0 reuteras   (501) staff       (20)     9165 2023-04-22 07:06:07.000000 rssfixer-0.0.7/src/rssfixer/rss.py
-drwxr-xr-x   0 reuteras   (501) staff       (20)        0 2023-04-22 07:41:52.402034 rssfixer-0.0.7/src/rssfixer.egg-info/
--rw-r--r--   0 reuteras   (501) staff       (20)     5336 2023-04-22 07:41:52.000000 rssfixer-0.0.7/src/rssfixer.egg-info/PKG-INFO
--rw-r--r--   0 reuteras   (501) staff       (20)      317 2023-04-22 07:41:52.000000 rssfixer-0.0.7/src/rssfixer.egg-info/SOURCES.txt
--rw-r--r--   0 reuteras   (501) staff       (20)        1 2023-04-22 07:41:52.000000 rssfixer-0.0.7/src/rssfixer.egg-info/dependency_links.txt
--rw-r--r--   0 reuteras   (501) staff       (20)       43 2023-04-22 07:41:52.000000 rssfixer-0.0.7/src/rssfixer.egg-info/entry_points.txt
--rw-r--r--   0 reuteras   (501) staff       (20)      203 2023-04-22 07:41:52.000000 rssfixer-0.0.7/src/rssfixer.egg-info/requires.txt
--rw-r--r--   0 reuteras   (501) staff       (20)       15 2023-04-22 07:41:52.000000 rssfixer-0.0.7/src/rssfixer.egg-info/top_level.txt
-drwxr-xr-x   0 reuteras   (501) staff       (20)        0 2023-04-22 07:41:52.402183 rssfixer-0.0.7/src/tests/
--rw-r--r--   0 reuteras   (501) staff       (20)     4314 2023-04-22 07:25:23.000000 rssfixer-0.0.7/src/tests/test_rss.py
+drwxr-xr-x   0 reuteras   (501) staff       (20)        0 2023-04-23 11:36:05.510625 rssfixer-0.1.0/
+-rw-r--r--   0 reuteras   (501) staff       (20)     1058 2023-04-16 10:16:56.000000 rssfixer-0.1.0/LICENSE
+-rw-r--r--   0 reuteras   (501) staff       (20)     7797 2023-04-23 11:36:05.510489 rssfixer-0.1.0/PKG-INFO
+-rw-r--r--   0 reuteras   (501) staff       (20)     6994 2023-04-23 08:48:37.000000 rssfixer-0.1.0/README.md
+-rw-r--r--   0 reuteras   (501) staff       (20)     1110 2023-04-23 11:34:36.000000 rssfixer-0.1.0/pyproject.toml
+-rw-r--r--   0 reuteras   (501) staff       (20)       38 2023-04-23 11:36:05.510675 rssfixer-0.1.0/setup.cfg
+drwxr-xr-x   0 reuteras   (501) staff       (20)        0 2023-04-23 11:36:05.508005 rssfixer-0.1.0/src/
+drwxr-xr-x   0 reuteras   (501) staff       (20)        0 2023-04-23 11:36:05.509257 rssfixer-0.1.0/src/rssfixer/
+-rw-r--r--   0 reuteras   (501) staff       (20)       81 2023-04-22 06:11:44.000000 rssfixer-0.1.0/src/rssfixer/__init__.py
+-rw-r--r--   0 reuteras   (501) staff       (20)     9423 2023-04-23 06:15:20.000000 rssfixer-0.1.0/src/rssfixer/rss.py
+drwxr-xr-x   0 reuteras   (501) staff       (20)        0 2023-04-23 11:36:05.510030 rssfixer-0.1.0/src/rssfixer.egg-info/
+-rw-r--r--   0 reuteras   (501) staff       (20)     7797 2023-04-23 11:36:05.000000 rssfixer-0.1.0/src/rssfixer.egg-info/PKG-INFO
+-rw-r--r--   0 reuteras   (501) staff       (20)      317 2023-04-23 11:36:05.000000 rssfixer-0.1.0/src/rssfixer.egg-info/SOURCES.txt
+-rw-r--r--   0 reuteras   (501) staff       (20)        1 2023-04-23 11:36:05.000000 rssfixer-0.1.0/src/rssfixer.egg-info/dependency_links.txt
+-rw-r--r--   0 reuteras   (501) staff       (20)       43 2023-04-23 11:36:05.000000 rssfixer-0.1.0/src/rssfixer.egg-info/entry_points.txt
+-rw-r--r--   0 reuteras   (501) staff       (20)      203 2023-04-23 11:36:05.000000 rssfixer-0.1.0/src/rssfixer.egg-info/requires.txt
+-rw-r--r--   0 reuteras   (501) staff       (20)       15 2023-04-23 11:36:05.000000 rssfixer-0.1.0/src/rssfixer.egg-info/top_level.txt
+drwxr-xr-x   0 reuteras   (501) staff       (20)        0 2023-04-23 11:36:05.510149 rssfixer-0.1.0/src/tests/
+-rw-r--r--   0 reuteras   (501) staff       (20)     4362 2023-04-23 08:49:18.000000 rssfixer-0.1.0/src/tests/test_rss.py
```

### Comparing `rssfixer-0.0.7/LICENSE` & `rssfixer-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rssfixer-0.0.7/PKG-INFO` & `rssfixer-0.1.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,36 +1,43 @@
 Metadata-Version: 2.1
 Name: rssfixer
-Version: 0.0.7
+Version: 0.1.0
 Summary: Generate RSS feed for Wordpress blog without it.
 Author-email: Peter Reuterås <peter@reuteras.net>
 Project-URL: Homepage, https://github.com/reuteras/rssfixer
 Project-URL: Bug Tracker, https://github.com/reuteras/rssfixer/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Information Technology
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: audit
 Provides-Extra: build
 Provides-Extra: lint
 Provides-Extra: test
 Provides-Extra: dev
 License-File: LICENSE
 
 # rssfixer
 
 [![GitHub Super-Linter](https://github.com/reuteras/rssfixer/actions/workflows/linter.yml/badge.svg)](https://github.com/marketplace/actions/super-linter)
 ![PyPI](https://img.shields.io/pypi/v/rssfixer?color=green)
 [![CodeQL](https://github.com/reuteras/rssfixer/workflows/CodeQL/badge.svg)](https://github.com/reuteras/rssfixer/actions?query=workflow%3ACodeQL)
 [![Coverage](https://raw.githubusercontent.com/reuteras/rssfixer/main/resources/coverage.svg)](https://github.com/reuteras/rssfixer/)
+<!-- CODE:BASH:START -->
+<!-- if jq '.metrics._totals | ."SEVERITY.HIGH"' resources/bandit.json | grep -vE '^0' > /dev/null ; then echo -n '[![security: bandit](https://img.shields.io/badge/security-bandit-red.svg)](https://github.com/PyCQA/bandit)' ; elif jq '.metrics._totals' resources/bandit.json | grep "SEVERITY" | grep -E ' 0,' | wc -l | grep -vE '4$' > /dev/null ; then echo -n '[![security: bandit](https://img.shields.io/badge/security-bandit-yellow.svg)](https://github.com/PyCQA/bandit)'; else echo -n '[![security: bandit](https://img.shields.io/badge/security-bandit-green.svg)](https://github.com/PyCQA/bandit)' ;fi -->
+<!-- CODE:END -->
+<!-- OUTPUT:START -->
+<!-- ⚠️ This content is auto-generated by `markdown-code-runner`. -->
+[![security: bandit](https://img.shields.io/badge/security-bandit-green.svg)](https://github.com/PyCQA/bandit)
+<!-- OUTPUT:END -->
 
 A small tool to generate an [RSS][rss] feed from some [WordPress][wor] blogs that for some reason don't generate their own feeds. This tool uses [BeautifulSoup][bso] to parse the HTML and [feedgen][fge] to generate the feed.
 
 ## Installation
 
 ```bash
 python3 -m venv venv
@@ -81,24 +88,40 @@
 rssfixer --title Tripwire --output tripwire.xml --quiet --html --base-url https://www.tripwire.com http://www.tripwire.com/state-of-security
 
 ```
 
 
 ### Usage
 
+Command-line options:
+
+<!-- CODE:BASH:START -->
+<!-- echo '```Text' -->
+<!-- rssfixer --help -->
+<!-- echo '```' -->
+<!-- CODE:END -->
+
+<!-- OUTPUT:START -->
+<!-- ⚠️ This content is auto-generated by `markdown-code-runner`. -->
 ```Text
-usage: rssfixer [-h] [--version] [--atom] [--base-url BASE_URL] [--html] [--html-entries HTML_ENTRIES]
-                [--html-url HTML_URL] [--html-title HTML_TITLE] [--html-title-class HTML_TITLE_CLASS]
-                [--html-description HTML_DESCRIPTION] [--html-description-class HTML_DESCRIPTION_CLASS]
-                [--json] [--json-entries JSON_ENTRIES] [--json-url JSON_URL] [--json-title JSON_TITLE]
-                [--json-description JSON_DESCRIPTION] [--output OUTPUT] [--title TITLE] [-q] [--list]
+usage: rssfixer [-h] [--version] [--atom] [--base-url BASE_URL] [--html]
+                [--html-entries HTML_ENTRIES] [--html-url HTML_URL]
+                [--html-title HTML_TITLE]
+                [--html-title-class HTML_TITLE_CLASS]
+                [--html-description HTML_DESCRIPTION]
+                [--html-description-class HTML_DESCRIPTION_CLASS] [--json]
+                [--json-entries JSON_ENTRIES] [--json-url JSON_URL]
+                [--json-title JSON_TITLE]
+                [--json-description JSON_DESCRIPTION] [--output OUTPUT]
+                [--title TITLE] [-q] [--list] [--stdout]
                 url
 
-Generate RSS feed for blog that don't publish a feed. Default is to find links in a simple <ul>-list.
-Options are available to find links in other HTML elements or JSON strings.
+Generate RSS feed for blog that don't publish a feed. Default is to find links
+in a simple <ul>-list. Options are available to find links in other HTML
+elements or JSON strings.
 
 positional arguments:
   url                   URL for the blog
 
 options:
   -h, --help            show this help message and exit
   --version             show program's version number and exit
@@ -124,17 +147,65 @@
                         JSON key for title
   --json-description JSON_DESCRIPTION
                         JSON key for description
   --output OUTPUT       Name of the output file
   --title TITLE         Title of the RSS feed (default: "My RSS Feed")
   -q, --quiet           Suppress output
   --list                Find entries in HTML <ul>-list (default)
+  --stdout              Print to stdout
+```
+
+<!-- OUTPUT:END -->
+
+## Command-line examples for some blogs
+
+### Apple Security Blog
+
+Url: [https://security.apple.com/blog/][app]
+
+```bash
+rssfixer --title "Apple Security" --output apple.xml --quiet --json --json-entries blogs --json-url slug --base-url https://security.apple.com/blog/ https://security.apple.com/blog
+```
+
+### nccgroup
+
+Url: [https://research.nccgroup.com/][ncc]
+
+```bash
+rssfixer --title nccgroup --output nccgroup.xml --quiet https://research.nccgroup.com
 ```
 
+or you can specify _--list__ to find the links in a list which is the default:
+
+```bash
+rssfixer --title nccgroup --output nccgroup.xml --quiet --list https://research.nccgroup.com
+```
+
+### Tripwire
+
+Url: [https://www.tripwire.com/state-of-security][tri]
+
+```bash
+rssfixer --title Tripwire --output tripwire.xml --quiet --html --base-url https://www.tripwire.com http://www.tripwire.com/state-of-security
+```
+
+### TrueSec
+
+Url: [https://www.truesec.com/hub/blog][tru]
+
+```bash
+rssfixer --title Truesec --output truesec.xml --quiet --json --json-description preamble https://www.truesec.com/hub/blog
+```
+
+## Setup blogs
+
+During testing it is useful to use --stdout to see the generated feed.
+
 
+  [app]: https://security.apple.com/blog/
   [bso]: https://www.crummy.com/software/BeautifulSoup/
   [exa]: https://github.com/reuteras/rssfixer/blob/main/src/tests/data/output/nccgroup.xml
   [fge]: https://feedgen.kiesow.be/
   [ncc]: https://research.nccgroup.com/
   [rss]: https://www.rssboard.org/
   [tri]: https://www.tripwire.com/state-of-security
   [tru]: https://www.truesec.com/hub/blog
```

### Comparing `rssfixer-0.0.7/pyproject.toml` & `rssfixer-0.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [project]
 name = "rssfixer"
-version = "0.0.7"
+version = "0.1.0"
 authors = [
   { name="Peter Reuterås", email="peter@reuteras.net" },
 ]
 description = "Generate RSS feed for Wordpress blog without it."
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Natural Language :: English",
     "Intended Audience :: Information Technology",
     "Development Status :: 4 - Beta",
```

### Comparing `rssfixer-0.0.7/src/rssfixer/rss.py` & `rssfixer-0.1.0/src/rssfixer/rss.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,14 +110,18 @@
     # Find the JSON string in the page
     for json_text in soup.find_all("script", type="application/json"):
         json_object = json.loads(json_text.text)
         entries = find_entries(json_object, arguments.json_entries)
         if entries is not None:
             break
 
+    if entries is None:  # pragma: no cover
+        print("ERROR: Unable to find JSON object")
+        sys.exit(1)
+
     # Extract the links from the JSON object
     for entry in entries:
         try:
             url = entry[arguments.json_url]
             title = entry[arguments.json_title]
         except KeyError:  # pragma: no cover
             print("ERROR: Unable to find URL or title in JSON object")
@@ -212,15 +216,15 @@
     parser.add_argument(
         "--json-title",
         default="title",
         help="JSON key for title",
     )
     parser.add_argument(
         "--json-description",
-        default="preamble",
+        default="description",
         help="JSON key for description",
     )
     parser.add_argument(
         "--output",
         default="rss_feed.xml",
         help="Name of the output file",
     )
@@ -229,14 +233,15 @@
         default="My RSS Feed",
         help='Title of the RSS feed (default: "My RSS Feed")',
     )
     parser.add_argument("-q", "--quiet", action="store_true", help="Suppress output")
     parser.add_argument(
         "--list", action="store_true", help="Find entries in HTML <ul>-list (default)"
     )
+    parser.add_argument("--stdout", action="store_true", help="Print to stdout")
 
     return parser.parse_args(arguments)
 
 
 def save_rss_feed(rss_feed, arguments):
     """Save the RSS feed to a file."""
     try:
@@ -273,12 +278,15 @@
     elif args.list:
         links = extract_links_ul(soup)
     else:
         links = extract_links_ul(soup)
 
     # Create RSS feed and save to file
     rss_feed = create_rss_feed(links, args)
-    save_rss_feed(rss_feed, args)
+    if args.stdout:
+        print(rss_feed)
+    else:
+        save_rss_feed(rss_feed, args)
 
 
 if __name__ == "__main__":
     main()  # pragma: no cover
```

### Comparing `rssfixer-0.0.7/src/rssfixer.egg-info/PKG-INFO` & `rssfixer-0.1.0/src/rssfixer.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,36 +1,43 @@
 Metadata-Version: 2.1
 Name: rssfixer
-Version: 0.0.7
+Version: 0.1.0
 Summary: Generate RSS feed for Wordpress blog without it.
 Author-email: Peter Reuterås <peter@reuteras.net>
 Project-URL: Homepage, https://github.com/reuteras/rssfixer
 Project-URL: Bug Tracker, https://github.com/reuteras/rssfixer/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Information Technology
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: audit
 Provides-Extra: build
 Provides-Extra: lint
 Provides-Extra: test
 Provides-Extra: dev
 License-File: LICENSE
 
 # rssfixer
 
 [![GitHub Super-Linter](https://github.com/reuteras/rssfixer/actions/workflows/linter.yml/badge.svg)](https://github.com/marketplace/actions/super-linter)
 ![PyPI](https://img.shields.io/pypi/v/rssfixer?color=green)
 [![CodeQL](https://github.com/reuteras/rssfixer/workflows/CodeQL/badge.svg)](https://github.com/reuteras/rssfixer/actions?query=workflow%3ACodeQL)
 [![Coverage](https://raw.githubusercontent.com/reuteras/rssfixer/main/resources/coverage.svg)](https://github.com/reuteras/rssfixer/)
+<!-- CODE:BASH:START -->
+<!-- if jq '.metrics._totals | ."SEVERITY.HIGH"' resources/bandit.json | grep -vE '^0' > /dev/null ; then echo -n '[![security: bandit](https://img.shields.io/badge/security-bandit-red.svg)](https://github.com/PyCQA/bandit)' ; elif jq '.metrics._totals' resources/bandit.json | grep "SEVERITY" | grep -E ' 0,' | wc -l | grep -vE '4$' > /dev/null ; then echo -n '[![security: bandit](https://img.shields.io/badge/security-bandit-yellow.svg)](https://github.com/PyCQA/bandit)'; else echo -n '[![security: bandit](https://img.shields.io/badge/security-bandit-green.svg)](https://github.com/PyCQA/bandit)' ;fi -->
+<!-- CODE:END -->
+<!-- OUTPUT:START -->
+<!-- ⚠️ This content is auto-generated by `markdown-code-runner`. -->
+[![security: bandit](https://img.shields.io/badge/security-bandit-green.svg)](https://github.com/PyCQA/bandit)
+<!-- OUTPUT:END -->
 
 A small tool to generate an [RSS][rss] feed from some [WordPress][wor] blogs that for some reason don't generate their own feeds. This tool uses [BeautifulSoup][bso] to parse the HTML and [feedgen][fge] to generate the feed.
 
 ## Installation
 
 ```bash
 python3 -m venv venv
@@ -81,24 +88,40 @@
 rssfixer --title Tripwire --output tripwire.xml --quiet --html --base-url https://www.tripwire.com http://www.tripwire.com/state-of-security
 
 ```
 
 
 ### Usage
 
+Command-line options:
+
+<!-- CODE:BASH:START -->
+<!-- echo '```Text' -->
+<!-- rssfixer --help -->
+<!-- echo '```' -->
+<!-- CODE:END -->
+
+<!-- OUTPUT:START -->
+<!-- ⚠️ This content is auto-generated by `markdown-code-runner`. -->
 ```Text
-usage: rssfixer [-h] [--version] [--atom] [--base-url BASE_URL] [--html] [--html-entries HTML_ENTRIES]
-                [--html-url HTML_URL] [--html-title HTML_TITLE] [--html-title-class HTML_TITLE_CLASS]
-                [--html-description HTML_DESCRIPTION] [--html-description-class HTML_DESCRIPTION_CLASS]
-                [--json] [--json-entries JSON_ENTRIES] [--json-url JSON_URL] [--json-title JSON_TITLE]
-                [--json-description JSON_DESCRIPTION] [--output OUTPUT] [--title TITLE] [-q] [--list]
+usage: rssfixer [-h] [--version] [--atom] [--base-url BASE_URL] [--html]
+                [--html-entries HTML_ENTRIES] [--html-url HTML_URL]
+                [--html-title HTML_TITLE]
+                [--html-title-class HTML_TITLE_CLASS]
+                [--html-description HTML_DESCRIPTION]
+                [--html-description-class HTML_DESCRIPTION_CLASS] [--json]
+                [--json-entries JSON_ENTRIES] [--json-url JSON_URL]
+                [--json-title JSON_TITLE]
+                [--json-description JSON_DESCRIPTION] [--output OUTPUT]
+                [--title TITLE] [-q] [--list] [--stdout]
                 url
 
-Generate RSS feed for blog that don't publish a feed. Default is to find links in a simple <ul>-list.
-Options are available to find links in other HTML elements or JSON strings.
+Generate RSS feed for blog that don't publish a feed. Default is to find links
+in a simple <ul>-list. Options are available to find links in other HTML
+elements or JSON strings.
 
 positional arguments:
   url                   URL for the blog
 
 options:
   -h, --help            show this help message and exit
   --version             show program's version number and exit
@@ -124,17 +147,65 @@
                         JSON key for title
   --json-description JSON_DESCRIPTION
                         JSON key for description
   --output OUTPUT       Name of the output file
   --title TITLE         Title of the RSS feed (default: "My RSS Feed")
   -q, --quiet           Suppress output
   --list                Find entries in HTML <ul>-list (default)
+  --stdout              Print to stdout
+```
+
+<!-- OUTPUT:END -->
+
+## Command-line examples for some blogs
+
+### Apple Security Blog
+
+Url: [https://security.apple.com/blog/][app]
+
+```bash
+rssfixer --title "Apple Security" --output apple.xml --quiet --json --json-entries blogs --json-url slug --base-url https://security.apple.com/blog/ https://security.apple.com/blog
+```
+
+### nccgroup
+
+Url: [https://research.nccgroup.com/][ncc]
+
+```bash
+rssfixer --title nccgroup --output nccgroup.xml --quiet https://research.nccgroup.com
 ```
 
+or you can specify _--list__ to find the links in a list which is the default:
+
+```bash
+rssfixer --title nccgroup --output nccgroup.xml --quiet --list https://research.nccgroup.com
+```
+
+### Tripwire
+
+Url: [https://www.tripwire.com/state-of-security][tri]
+
+```bash
+rssfixer --title Tripwire --output tripwire.xml --quiet --html --base-url https://www.tripwire.com http://www.tripwire.com/state-of-security
+```
+
+### TrueSec
+
+Url: [https://www.truesec.com/hub/blog][tru]
+
+```bash
+rssfixer --title Truesec --output truesec.xml --quiet --json --json-description preamble https://www.truesec.com/hub/blog
+```
+
+## Setup blogs
+
+During testing it is useful to use --stdout to see the generated feed.
+
 
+  [app]: https://security.apple.com/blog/
   [bso]: https://www.crummy.com/software/BeautifulSoup/
   [exa]: https://github.com/reuteras/rssfixer/blob/main/src/tests/data/output/nccgroup.xml
   [fge]: https://feedgen.kiesow.be/
   [ncc]: https://research.nccgroup.com/
   [rss]: https://www.rssboard.org/
   [tri]: https://www.tripwire.com/state-of-security
   [tru]: https://www.truesec.com/hub/blog
```

### Comparing `rssfixer-0.0.7/src/tests/test_rss.py` & `rssfixer-0.1.0/src/tests/test_rss.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,15 +109,17 @@
 
 
 def test_extract_links_json():
     """Test extract_links_json()."""
     with open("src/tests/data/input/truesec.html", "r", encoding="utf-8") as f:
         content = f.read()
     soup = BeautifulSoup(content, "html.parser")
-    arguments = rss.parse_arguments(["--json", "https://www.truesec.com/hub/blog"])
+    arguments = rss.parse_arguments(
+        ["--json", "--json-description", "preamble", "https://www.truesec.com/hub/blog"]
+    )
     links = rss.extract_links_json(soup, arguments)
     with open("src/tests/data/output/truesec", "rb") as f:
         correct_links = pickle.load(f)
     assert links == correct_links
 
 
 def test_create_rss_feed():
```

