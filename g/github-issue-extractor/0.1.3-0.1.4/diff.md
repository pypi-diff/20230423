# Comparing `tmp/github_issue_extractor-0.1.3.tar.gz` & `tmp/github_issue_extractor-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "github_issue_extractor-0.1.3.tar", last modified: Sat Apr 22 21:44:49 2023, max compression
+gzip compressed data, was "github_issue_extractor-0.1.4.tar", last modified: Sat Apr 22 22:47:10 2023, max compression
```

## Comparing `github_issue_extractor-0.1.3.tar` & `github_issue_extractor-0.1.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 21:44:49.052898 github_issue_extractor-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-22 21:44:37.000000 github_issue_extractor-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-04-22 21:44:49.052898 github_issue_extractor-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-04-22 21:44:37.000000 github_issue_extractor-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 21:44:49.052898 github_issue_extractor-0.1.3/github_issue_extractor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2318 2023-04-22 21:44:49.000000 github_issue_extractor-0.1.3/github_issue_extractor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-22 21:44:49.000000 github_issue_extractor-0.1.3/github_issue_extractor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 21:44:49.000000 github_issue_extractor-0.1.3/github_issue_extractor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-22 21:44:49.000000 github_issue_extractor-0.1.3/github_issue_extractor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 21:44:49.000000 github_issue_extractor-0.1.3/github_issue_extractor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 21:44:49.052898 github_issue_extractor-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-04-22 21:44:37.000000 github_issue_extractor-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 22:47:10.708306 github_issue_extractor-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-22 22:46:59.000000 github_issue_extractor-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-04-22 22:47:10.708306 github_issue_extractor-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-04-22 22:46:59.000000 github_issue_extractor-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 22:47:10.704306 github_issue_extractor-0.1.4/github_issue_extractor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-04-22 22:47:10.000000 github_issue_extractor-0.1.4/github_issue_extractor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-22 22:47:10.000000 github_issue_extractor-0.1.4/github_issue_extractor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 22:47:10.000000 github_issue_extractor-0.1.4/github_issue_extractor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-22 22:47:10.000000 github_issue_extractor-0.1.4/github_issue_extractor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 22:47:10.000000 github_issue_extractor-0.1.4/github_issue_extractor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 22:47:10.708306 github_issue_extractor-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-04-22 22:46:59.000000 github_issue_extractor-0.1.4/setup.py
```

### Comparing `github_issue_extractor-0.1.3/LICENSE` & `github_issue_extractor-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `github_issue_extractor-0.1.3/PKG-INFO` & `github_issue_extractor-0.1.4/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,10 @@
-Metadata-Version: 2.1
-Name: github_issue_extractor
-Version: 0.1.3
-Summary: GitHubIssueExtractor
-Home-page: https://github.com/ssinha2103/github-issues_to_excel
-Author: Sudarshan Sinha
-Author-email: s.sinha2103@outlook.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # GitHub Issue Extractor
 
-GitHub Issue Extractor is a Python utility that helps you extract issues from a specific GitHub repository and milestone. This tool utilizes the GitHub API and requires an access token for authentication. 
+The GitHub Issue Extractor allows you to easily filter and extract issues from a GitHub repository based on a specified milestone number. It uses the GitHub API and requires an access token for authentication. This powerful utility writes the extracted information into an Excel file for convenient analysis and reporting.
 
 ## Features
 - Extract issues from a specific GitHub repository
 - Filter issues by milestone number
 - Requires a GitHub access token for authentication
 
 ## Prerequisites
@@ -57,8 +43,8 @@
 ## Parameters
 1. `milestone_number`: The milestone number you want to filter issues by.
 2. `access_token`: Your GitHub personal access token for authentication. Follow [these instructions](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token) to create a personal access token.
 3. `repo_name`: The name of the repository from which you want to extract issues.
 4. `owner`: The username of the repository owner.
 
 ## License
-This project is licensed under the MIT License. See the LICENSE file for details.
+This project is licensed under the MIT License. See the LICENSE file for details.
```

### Comparing `github_issue_extractor-0.1.3/github_issue_extractor.egg-info/PKG-INFO` & `github_issue_extractor-0.1.4/github_issue_extractor.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: github-issue-extractor
-Version: 0.1.3
+Version: 0.1.4
 Summary: GitHubIssueExtractor
 Home-page: https://github.com/ssinha2103/github-issues_to_excel
 Author: Sudarshan Sinha
 Author-email: s.sinha2103@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # GitHub Issue Extractor
 
-GitHub Issue Extractor is a Python utility that helps you extract issues from a specific GitHub repository and milestone. This tool utilizes the GitHub API and requires an access token for authentication. 
+The GitHub Issue Extractor allows you to easily filter and extract issues from a GitHub repository based on a specified milestone number. It uses the GitHub API and requires an access token for authentication. This powerful utility writes the extracted information into an Excel file for convenient analysis and reporting.
 
 ## Features
 - Extract issues from a specific GitHub repository
 - Filter issues by milestone number
 - Requires a GitHub access token for authentication
 
 ## Prerequisites
```

### Comparing `github_issue_extractor-0.1.3/setup.py` & `github_issue_extractor-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
     name="github_issue_extractor",
-    version="0.1.3",
+    version="0.1.4",
     author="Sudarshan Sinha",
     author_email="s.sinha2103@outlook.com",
     description="GitHubIssueExtractor",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ssinha2103/github-issues_to_excel",
     packages=setuptools.find_packages(),
```

