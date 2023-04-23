# Comparing `tmp/lcr-api-2-0.5.5.tar.gz` & `tmp/lcr-api-2-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lcr-api-2-0.5.5.tar", last modified: Mon Feb 13 18:30:45 2023, max compression
+gzip compressed data, was "lcr-api-2-0.5.6.tar", last modified: Sun Apr 23 18:19:13 2023, max compression
```

## Comparing `lcr-api-2-0.5.5.tar` & `lcr-api-2-0.5.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 sirsmith   (505) staff       (20)        0 2023-02-13 18:30:45.988515 lcr-api-2-0.5.5/
--rw-r--r--   0 sirsmith   (505) staff       (20)     1745 2023-02-13 18:30:45.988382 lcr-api-2-0.5.5/PKG-INFO
--rwxr-xr-x   0 sirsmith   (505) staff       (20)     1350 2022-08-07 14:17:59.000000 lcr-api-2-0.5.5/README.md
-drwxr-xr-x   0 sirsmith   (505) staff       (20)        0 2023-02-13 18:30:45.984889 lcr-api-2-0.5.5/lcr/
--rw-r--r--   0 sirsmith   (505) staff       (20)     9604 2023-02-12 19:38:57.000000 lcr-api-2-0.5.5/lcr/__init__.py
-drwxr-xr-x   0 sirsmith   (505) staff       (20)        0 2023-02-13 18:30:45.988189 lcr-api-2-0.5.5/lcr_api_2.egg-info/
--rw-r--r--   0 sirsmith   (505) staff       (20)     1745 2023-02-13 18:30:45.000000 lcr-api-2-0.5.5/lcr_api_2.egg-info/PKG-INFO
--rw-r--r--   0 sirsmith   (505) staff       (20)      230 2023-02-13 18:30:45.000000 lcr-api-2-0.5.5/lcr_api_2.egg-info/SOURCES.txt
--rw-r--r--   0 sirsmith   (505) staff       (20)        1 2023-02-13 18:30:45.000000 lcr-api-2-0.5.5/lcr_api_2.egg-info/dependency_links.txt
--rw-r--r--   0 sirsmith   (505) staff       (20)        1 2022-07-17 21:42:15.000000 lcr-api-2-0.5.5/lcr_api_2.egg-info/not-zip-safe
--rw-r--r--   0 sirsmith   (505) staff       (20)       15 2023-02-13 18:30:45.000000 lcr-api-2-0.5.5/lcr_api_2.egg-info/requires.txt
--rw-r--r--   0 sirsmith   (505) staff       (20)        4 2023-02-13 18:30:45.000000 lcr-api-2-0.5.5/lcr_api_2.egg-info/top_level.txt
--rw-r--r--   0 sirsmith   (505) staff       (20)       38 2023-02-13 18:30:45.988566 lcr-api-2-0.5.5/setup.cfg
--rwxr-xr-x   0 sirsmith   (505) staff       (20)     1092 2023-02-13 18:27:16.000000 lcr-api-2-0.5.5/setup.py
+drwxr-xr-x   0 sirsmith   (505) staff       (20)        0 2023-04-23 18:19:13.533292 lcr-api-2-0.5.6/
+-rw-r--r--   0 sirsmith   (505) staff       (20)     1745 2023-04-23 18:19:13.533082 lcr-api-2-0.5.6/PKG-INFO
+-rwxr-xr-x   0 sirsmith   (505) staff       (20)     1350 2022-08-07 14:17:59.000000 lcr-api-2-0.5.6/README.md
+drwxr-xr-x   0 sirsmith   (505) staff       (20)        0 2023-04-23 18:19:13.531022 lcr-api-2-0.5.6/lcr/
+-rw-r--r--   0 sirsmith   (505) staff       (20)     8052 2023-04-23 18:13:20.000000 lcr-api-2-0.5.6/lcr/__init__.py
+drwxr-xr-x   0 sirsmith   (505) staff       (20)        0 2023-04-23 18:19:13.532780 lcr-api-2-0.5.6/lcr_api_2.egg-info/
+-rw-r--r--   0 sirsmith   (505) staff       (20)     1745 2023-04-23 18:19:13.000000 lcr-api-2-0.5.6/lcr_api_2.egg-info/PKG-INFO
+-rw-r--r--   0 sirsmith   (505) staff       (20)      230 2023-04-23 18:19:13.000000 lcr-api-2-0.5.6/lcr_api_2.egg-info/SOURCES.txt
+-rw-r--r--   0 sirsmith   (505) staff       (20)        1 2023-04-23 18:19:13.000000 lcr-api-2-0.5.6/lcr_api_2.egg-info/dependency_links.txt
+-rw-r--r--   0 sirsmith   (505) staff       (20)        1 2022-07-17 21:42:15.000000 lcr-api-2-0.5.6/lcr_api_2.egg-info/not-zip-safe
+-rw-r--r--   0 sirsmith   (505) staff       (20)       15 2023-04-23 18:19:13.000000 lcr-api-2-0.5.6/lcr_api_2.egg-info/requires.txt
+-rw-r--r--   0 sirsmith   (505) staff       (20)        4 2023-04-23 18:19:13.000000 lcr-api-2-0.5.6/lcr_api_2.egg-info/top_level.txt
+-rw-r--r--   0 sirsmith   (505) staff       (20)       38 2023-04-23 18:19:13.533372 lcr-api-2-0.5.6/setup.cfg
+-rwxr-xr-x   0 sirsmith   (505) staff       (20)     1092 2023-04-23 18:19:10.000000 lcr-api-2-0.5.6/setup.py
```

### Comparing `lcr-api-2-0.5.5/PKG-INFO` & `lcr-api-2-0.5.6/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: lcr-api-2
-Version: 0.5.5
+Version: 0.5.6
 Summary: An API for the LDS churches Leader and Clerk Resources (LCR),
 Home-page: https://github.com/SpencerMKSmith/LCR-API-2
-Download-URL: https://github.com/SpencerMKSmith/LCR-API-2/archive/v0.5.5.zip
+Download-URL: https://github.com/SpencerMKSmith/LCR-API-2/archive/v0.5.6.zip
 Author: Spencer Smith
 Author-email: spencermksmith@gmail.com
 License: MIT License
 Platform: any
 Description-Content-Type: text/markdown
 
 # LCR API
```

### Comparing `lcr-api-2-0.5.5/README.md` & `lcr-api-2-0.5.6/README.md`

 * *Files identical despite different names*

### Comparing `lcr-api-2-0.5.5/lcr/__init__.py` & `lcr-api-2-0.5.6/lcr/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 #!/usr/bin/env python3
 
 import re
 import json
 import logging
 import requests
+import time
+
 
 from selenium import webdriver
 from selenium.webdriver.common.by import By
 from selenium.webdriver.support.ui import WebDriverWait
 from selenium.webdriver.support import expected_conditions as ec
 from webdriver_manager.chrome import ChromeDriverManager
 
@@ -15,15 +17,14 @@
 HOST = "churchofjesuschrist.org"
 BETA_HOST = f"beta.{HOST}"
 LCR_DOMAIN = f"lcr.{HOST}"
 CHROME_OPTIONS = webdriver.chrome.options.Options()
 CHROME_OPTIONS.add_argument("--headless")
 TIMEOUT = 10
 
-
 if _LOGGER.getEffectiveLevel() <= logging.DEBUG:
     import http.client as http_client
     http_client.HTTPConnection.debuglevel = 1
 
 
 class InvalidCredentialsError(Exception):
     pass
@@ -44,46 +45,52 @@
 
     def _login(self, user, password):
         _LOGGER.info("Logging in")
 
         # Navigate to the login page
         self.driver.get(f"https://{LCR_DOMAIN}")
 
+        _LOGGER.info("Entering username")
+
         # Enter the username
         login_input = WebDriverWait(self.driver, TIMEOUT).until(
                         ec.presence_of_element_located(
                             (By.CSS_SELECTOR, "input#okta-signin-username")
                             )
                         )
         login_input.send_keys(user)
         login_input.submit()
 
+        _LOGGER.info("Entering password")
+
         # Enter password
         password_input = WebDriverWait(self.driver, TIMEOUT).until(
                 ec.presence_of_element_located(
                     (By.CSS_SELECTOR, "input.password-with-toggle")
                     )
                 )
         password_input.send_keys(password)
         password_input.submit()
 
         # Wait until the page is loaded
         WebDriverWait(self.driver, TIMEOUT).until(
                 ec.presence_of_element_located(
-                    (By.CSS_SELECTOR, "churchofjesuschrist-eden-normalize")
+                    (By.CSS_SELECTOR, "platform-header.PFshowHeader")
                     )
                 )
+        
+        time.sleep(5) # Unable to find a better item above to wait on, but the above still needs some of the page to load.
+
+        _LOGGER.info("Successfully logged in, getting cookies")
 
-        # Get authState parameter.
+        # Get authState parameter.  Copy all cookies from the session rather than looking for a specific one.
         cookies = self.driver.get_cookies()
-        potential_cookie = [c for c in cookies if "ChurchSSO" in c['name']]
-        real_cookie = next(iter(potential_cookie))
-        churchcookie = real_cookie['value']
+        for cookie in cookies:
+            self.session.cookies.set(cookie['name'], cookie['value'])
 
-        self.session.cookies['ChurchSSO'] = churchcookie
         self.driver.close()
         self.driver.quit()
 
     def _make_request(self, request):
         if self.beta:
             request['cookies'] = {'clerk-resources-beta-terms': '4.1',
                                   'clerk-resources-beta-eula': '4.2'}
@@ -91,52 +98,52 @@
         response = self.session.get(**request)
         response.raise_for_status()  # break on any non 200 status
         return response
 
     def birthday_list(self, month, months=1):
         _LOGGER.info("Getting birthday list")
         request = {
-                'url': 'https://{}/services/report/birthday-list'.format(
+                'url': 'https://{}/api/report/birthday-list'.format(
                     LCR_DOMAIN
                     ),
                 'params': {
                     'lang': 'eng',
                     'month': month,
                     'months': months
                     }
                 }
 
         result = self._make_request(request)
         return result.json()
 
     def members_moved_in(self, months):
         _LOGGER.info("Getting members moved in")
-        request = {'url': 'https://{}/services/report/members-moved-in/unit/{}/{}'.format(LCR_DOMAIN,
+        request = {'url': 'https://{}/api/report/members-moved-in/unit/{}/{}'.format(LCR_DOMAIN,
                                                                                                   self.unit_number,
                                                                                                   months),
                    'params': {'lang': 'eng'}}
 
         result = self._make_request(request)
         return result.json()
 
 
     def members_moved_out(self, months):
         _LOGGER.info("Getting members moved out")
-        request = {'url': 'https://{}/services/report/members-moved-out/unit/{}/{}'.format(LCR_DOMAIN,
+        request = {'url': 'https://{}/api/report/members-moved-out/unit/{}/{}'.format(LCR_DOMAIN,
                                                                                                    self.unit_number,
                                                                                                    months),
                    'params': {'lang': 'eng'}}
 
         result = self._make_request(request)
         return result.json()
 
 
     def member_list(self):
         _LOGGER.info("Getting member list")
-        request = {'url': 'https://{}/services/umlu/report/member-list'.format(LCR_DOMAIN),
+        request = {'url': 'https://{}/api/umlu/report/member-list'.format(LCR_DOMAIN),
                    'params': {'lang': 'eng',
                               'unitNumber': self.unit_number}}
 
         result = self._make_request(request)
         return result.json()
 
 
@@ -152,103 +159,70 @@
         result = self._make_request(request)
         scdn_url = result.json()['tokenUrl']
         return self._make_request({'url': scdn_url}).content
 
 
     def callings(self):
         _LOGGER.info("Getting callings for all organizations")
-        request = {'url': 'https://{}/services/orgs/sub-orgs-with-callings'.format(LCR_DOMAIN),
+        request = {'url': 'https://{}/api/orgs/sub-orgs-with-callings'.format(LCR_DOMAIN),
                    'params': {'lang': 'eng'}}
 
         result = self._make_request(request)
         return result.json()
 
 
     def members_with_callings_list(self):
         _LOGGER.info("Getting callings for all organizations")
-        request = {'url': 'https://{}/services/report/members-with-callings'.format(LCR_DOMAIN),
+        request = {'url': 'https://{}/api/report/members-with-callings'.format(LCR_DOMAIN),
                    'params': {'lang': 'eng'}}
 
         result = self._make_request(request)
         return result.json()
 
 
     def ministering(self):
         """
         API parameters known to be accepted are lang type unitNumber and quarter.
         """
         _LOGGER.info("Getting ministering data")
-        request = {'url': 'https://{}/services/umlu/v1/ministering/data-full'.format(LCR_DOMAIN),
+        request = {'url': 'https://{}/api/umlu/v1/ministering/data-full'.format(LCR_DOMAIN),
                    'params': {'lang': 'eng',
                               'unitNumber': self.unit_number}}
 
         result = self._make_request(request)
         return result.json()
 
 
     def access_table(self):
         """
         Once the users role id is known this table could be checked to selectively enable or disable methods for API endpoints.
         """
         _LOGGER.info("Getting info for data access")
-        request = {'url': 'https://{}/services/access-table'.format(LCR_DOMAIN),
+        request = {'url': 'https://{}/api/access-table'.format(LCR_DOMAIN),
                    'params': {'lang': 'eng'}}
 
         result = self._make_request(request)
         return result.json()
 
 
     def recommend_status(self):
         """
         Obtain member information on recommend status
         """
         _LOGGER.info("Getting recommend status")
         request = {
-                'url': 'https://{}/services/recommend/recommend-status'.format(LCR_DOMAIN),
+                'url': 'https://{}/api/recommend/recommend-status'.format(LCR_DOMAIN),
                 'params': {
                     'lang': 'eng',
                     'unitNumber': self.unit_number
                     }
                 }
         result = self._make_request(request)
         return result.json()
 
-    def aggregated_member_data():
-        """
-        Returns list of members including recommend and calling data.  Returned using the MemberData object.
-        """
-
-        print("Getting entire member list")
-        allMemberList = self.member_list()
-
-        allMemberIdToMemberMap = {member['legacyCmisId']: member for member in allMemberList}
-        print("Pulling members with calling list")
-        membersWithCallingMap = {member['id']: member for member in self.members_with_callings_list()}
-        print("Pulling recommend status list")
-        recommendStatusMap = {member['id']: member for member in self.recommend_status()}
-
-        memberDataObjectList = []
-        for member in allMemberList:
-            legacyMemberId = member['legacyCmisId']
-            firstName = member['nameFormats'].get('givenPreferredLocal', "").split(" ", 1)[0]
-            lastName = member['nameFormats'].get('familyPreferredLocal') or ""
-            fullName = firstName + " " + lastName
-            age = member['age']
-            callings = membersWithCallingMap.get(legacyMemberId, {}).get('position', "")
-            recommendStatus = recommendStatusMap.get(legacyMemberId, {}).get('status', "")
-            memberDataObject = MemberData(legacyMemberId, fullName, age, callings, recommendStatus)
-            memberDataObjectList.append(memberDataObject)
-
-    def getReadableName(name):
-        """
-        Helper method to take names like "Smith, Joseph A." and convert to "Joseph Smith"
-        """
-        splitBySpaces = name.replace(',', '').split(" ")            # Remove the comma and split by spaces
-        readableName = splitBySpaces[1] + " " + splitBySpaces[0]    # Keep only the first and last names
-        return readableName
 
 class MemberData():
     def __init__(self, fullName, age, callings, recommendStatus, legacyMemberId):
         self.fullName = fullName
         self.age = age
         self.callings = callings
         self.recommendStatus = recommendStatus
```

### Comparing `lcr-api-2-0.5.5/lcr_api_2.egg-info/PKG-INFO` & `lcr-api-2-0.5.6/lcr_api_2.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: lcr-api-2
-Version: 0.5.5
+Version: 0.5.6
 Summary: An API for the LDS churches Leader and Clerk Resources (LCR),
 Home-page: https://github.com/SpencerMKSmith/LCR-API-2
-Download-URL: https://github.com/SpencerMKSmith/LCR-API-2/archive/v0.5.5.zip
+Download-URL: https://github.com/SpencerMKSmith/LCR-API-2/archive/v0.5.6.zip
 Author: Spencer Smith
 Author-email: spencermksmith@gmail.com
 License: MIT License
 Platform: any
 Description-Content-Type: text/markdown
 
 # LCR API
```

### Comparing `lcr-api-2-0.5.5/setup.py` & `lcr-api-2-0.5.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3
 import os
 from setuptools import setup, find_packages
 
-VERSION = 'v0.5.5'
+VERSION = 'v0.5.6'
 PACKAGE_NAME = 'lcr-api-2'
 HERE = os.path.abspath(os.path.dirname(__file__))
 DOWNLOAD_URL = ('https://github.com/SpencerMKSmith/LCR-API-2/archive/'
                 '{}.zip'.format(VERSION))
 
 PACKAGES = find_packages(exclude=['tests', 'tests.*'])
```

